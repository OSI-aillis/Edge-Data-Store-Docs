---
uid: piEgressQuickStart
---

# PI System (PI Web API) egress quick start

This document is a quick tour of getting data stored in the Edge Data Store into a remote PI System. This is accomplished using PI Web API which is configured for Basic authentication.

## Create a periodic egress configuration

Complete the following to configure Edge Storage periodic egress for the PI Web API endpoint and credentials:

1. Use the following example to create a JSON file.

```json
[{
    "Id": "PWA",
    "ExecutionPeriod": "00:00:50",
    "Name": null,
    "NamespaceId": "default",
    "Description": null,
    "Enabled": true,
    "Backfill": false,
    "EgressFilter": "",
    "StreamPrefix": "<unique stream prefix>",
    "TypePrefix": "<unique type prefix>",
    "Endpoint": "https://<your PI Web API Server>/piwebapi/omf/",
    "ClientId": null,
    "ClientSecret": null,
    "UserName": "<username>",
    "Password": "<password>",
    "DebugExpiration": null,
    "ValidateEndpointCertificate": true,
    "TokenEndpoint": null
}]
```

2. Add the server name, username and password of your PI Web API server into the "Endpoint" definition.  You must specify a valid user account that can write data via PI Web API using Basic authentication.

**Note:** StreamPrefix and TypePrefix values can be used to ensure uniqueness on the destination system, if required. The StreamPrefix value will create unique PI Points on the PI System. If you wish to only send specific streams, edit the "EgressFilter" value. Examples of more advanced scenarios are in the Egress section of this documentation.

3. Save the JSON with the file name PeriodicEgressEndpoints.json.
4. Run the following curl script, from the same directory where you saved the JSON file, to configure Edge Storage to send data to the PI System. 

**Note:** The file and curl script can be run from any directory on the device as long as the file and the curl script are run from the same directory:

```bash
curl -i -d "@PeriodicEgressEndpoints.json" -H "Content-Type: application/json" -X PUT http://localhost:5590/api/v1/configuration/storage/PeriodicEgressEndpoints/
```

When the command completes successfully, data will start being sent to the PI System.
