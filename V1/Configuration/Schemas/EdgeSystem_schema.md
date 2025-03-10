---
uid: edge_system_schema
---

# Edge Data Store configuration schema

The Edge Data Store configuration schema specifies how to formally describe the system parameters (logging, components, health endpoints, port). 

```json
   "System": {
        "Logging": {
            "logLevel": "Information",
            "logFileSizeLimitBytes": 34636833,
            "logFileCountLimit": 31
        },
        "Components": [{
                "componentId": "OpcUa1",
                "componentType": "OpcUa"
            },
            {
                "componentId": "Modbus1",
                "componentType": "Modbus"
            },
            {
                "componentId": "Storage",
                "componentType": "EDS.Component"
            }
        ],
        "HealthEndpoints": [],
        "Port": {
            "port": 5590
        }
    }
```

## Properties

| Property                                        | Type      | Required | Nullable | Defined by                            |
| ----------------------------------------------- | --------- | -------- | -------- | ------------------------------------- |
| [Storage](#storage)         | [`StorageConfiguration`](xref:storage_schema) | Optional | Yes      | StorageConfiguration |
| [System](#system) | [`SystemConfiguration`](xref:system_schema) | Optional | Yes      | SystemConfiguration |
| [{ComponentName}](#system) | [`{ComponentConfiguration}`](#system) | Optional | Yes      | {ComponentConfiguration} |

## Storage

- is optional
- type: [`StorageConfiguration`](xref:storage_schema)

## System

- is optional
- type: [`SystemConfiguration`](xref:system_schema)

## {ComponentName}
- [EdgeDataStoreConfiguration Schema](#EdgeDataStoreconfiguration-schema)
- [Edge Data Store Configuration Schema](#edge-system-configuration-schema)
  - [Properties](#properties)
  - [Storage](#storage)
  - [System](#system)
  - [{ComponentName}](#componentname)

