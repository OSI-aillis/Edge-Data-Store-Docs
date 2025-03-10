---
uid: index
---

# OSIsoft Edge Data Store

=======

- [Overview](xref:EdgeDataStoreOverview)
  - [OMF Quick Start](xref:omfQuickStart)
  - [Modbus Quick Start](xref:modbusQuickStart)
  - [Opc Ua Quick Start](xref:opcUaQuickStart)
  - [OCS Egress Quick Start](xref:ocsEgressQuickStart)
  - [PI Egress Quick Start](xref:piEgressQuickStart)
  - [SDS Read/Write Quick Start](xref:sdsQuickStart)
  - [Visualization Quick Start](xref:visualizationQuickStart)
  - [Analytics Quick Start](xref:analyticsQuickStart)
  - [Command Line Quick Start - Linux](xref:commandLineLinuxQuickStart)
  - [Command Line Quick Start - Windows](xref:commandLineWindowsQuickStart)
- [Design](xref:scalePerformance)
- [Installation](xref:installationOverview)
- [Security](xref:security)
- [System Configuration](xref:EdgeDataStoreConfiguration)
- [EDS data ingress](xref:EDSDataIngress)
  - [OPC UA adapter](xref:opcUaOverview)
    - [Supported Features](xref:SupportedFeaturesOPCUA)
    - [Principles of operation](xref:PrinciplesOfOperationOPCUA.md)
    - [Data source configuration](xref:OPCUADataSourceConfiguration)
    - [Data selection configuration](xref:OPCUADataSelectionConfiguration)
      - [Opc Ua Data Selection](xref:opcUaDataSelection)
    - [Adapter security](xref:OPCUAAdapterSecurityConfiguration)
  - [Modbus TCP adapter](xref:modbusOverview)
    - [Supported Features](xref:SupportedFeaturesModbus)
    - [Principles of operation](xref:PrinciplesOfOperationModbus)
    - [Data source configuration](xref:ModbusTCPDataSourceConfiguration)
    - [Data selection configuration](xref:ModbusTCPDataSelectionConfiguration)
    - [Adapter security](xref:ModbusTCPAdapterSecurity)
  - [OMF](xref:omfOverview)
- [Storage](xref:storage)
  - [Sequential Data Store](xref:sdsOverview)
    - [Types](xref:sdsTypes)
    - [Streams](xref:sdsStreams)
    - [Stream Views](xref:sdsStreamViews)
    - [Indexes](xref:sdsIndexes)
    - [Writing Data](xref:sdsWritingData)
      - [Write Data API](xref:sdsWritingDataApi)
    - [Reading Data](xref:sdsReadingData)
      - [Reading Data API](xref:sdsReadingDataApi)
      - [Filter Expressions](xref:sdsFilterExpressions)
      - [Table Format](xref:sdsTableFormat)
    - [Units of Measure](xref:unitsOfMeasure)
    - [Request/Response Compression](xref:sdsCompression)
    - [Searching](xref:sdsSearching)
    - [Stream Tags and Metadata](xref:sdsStreamExtra)
  - [Egress](xref:egress)
- [Administration](xref:EdgeDataStoreAdministration)
  - [Management Tools](xref:managementTools)
  - [Logging Configuration](xref:loggingConfiguration)
- [Configuration Schemas](xref:configurationSchemaList)
  - [Edge Data Store Schema](xref:edge_system_schema)
  - [System](xref:system)
    - [System Schema](xref:system_schema)
    - [System Port Schema](xref:system_Port_schema)
  - [EDS Modbus TCP adapter](xref:edsmodbustcpadapter)
    - [Modbus Data Source Schema](xref:modbus_DataSource_schema)
    - [Modbus Data Selection Schema](xref:modbus_DataSelection_schema)
    - [Modbus Logging Schema](xref:modbus_Logging_schema)
  - [EDS OPC UA adapter](xref:edsopcuaadapter)
    - [OPC UA Data Source Schema](xref:opcUa_DataSource_Schema)
    - [OPC UA Data Selection Schema](xref:opcUa_DataSelection_schema)
    - [OPC UA Logging Schema](xref:opcUa_Logging_schema)
  - [Storage](xref:storage)
    - [Storage Schema](xref:storage_schema)
    - [Storage Logging Schema](xref:Storage_Logging_schema)
    - [Storage Periodic Egress Endpoints Schema](xref:storage_PeriodicEgressEndpoints_schema)
    - [Storage Runtime Schema](xref:storage_Runtime_schema)
- [Health](xref:EdgeDataStoreHealth)
- [Diagnostics](xref:EdgeDataStoreDiagnostics)
- [Platforms](xref:linuxWindows)
- [Docker](xref:edgeDocker)
- [Command Line](xref:commandLine)
- [Troubleshooting](xref:troubleShooting)
- [Release Notes](xref:releaseNotes)
