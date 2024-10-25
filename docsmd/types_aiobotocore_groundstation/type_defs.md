# Type definitions

> [Index](../README.md) > [GroundStation](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [GroundStation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
    type annotations stubs module [types-aiobotocore-groundstation](https://pypi.org/project/types-aiobotocore-groundstation/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## SecurityDetailsUnionTypeDef

```python
# SecurityDetailsUnionTypeDef definition

SecurityDetailsUnionTypeDef = Union[
    SecurityDetailsTypeDef,  # (1)
    SecurityDetailsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SecurityDetailsTypeDef](./type_defs.md#securitydetailstypedef) 
2. See [:material-code-braces: SecurityDetailsOutputTypeDef](./type_defs.md#securitydetailsoutputtypedef) 

## EndpointDetailsUnionTypeDef

```python
# EndpointDetailsUnionTypeDef definition

EndpointDetailsUnionTypeDef = Union[
    EndpointDetailsTypeDef,  # (1)
    EndpointDetailsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EndpointDetailsTypeDef](./type_defs.md#endpointdetailstypedef) 
2. See [:material-code-braces: EndpointDetailsOutputTypeDef](./type_defs.md#endpointdetailsoutputtypedef) 



## ComponentVersionTypeDef

```python
# ComponentVersionTypeDef definition

class ComponentVersionTypeDef(TypedDict):
    componentType: str,
    versions: Sequence[str],
```

## AggregateStatusTypeDef

```python
# AggregateStatusTypeDef definition

class AggregateStatusTypeDef(TypedDict):
    status: AgentStatusType,  # (1)
    signatureMap: NotRequired[Mapping[str, bool]],
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype) 
## AntennaDemodDecodeDetailsTypeDef

```python
# AntennaDemodDecodeDetailsTypeDef definition

class AntennaDemodDecodeDetailsTypeDef(TypedDict):
    outputNode: NotRequired[str],
```

## DecodeConfigTypeDef

```python
# DecodeConfigTypeDef definition

class DecodeConfigTypeDef(TypedDict):
    unvalidatedJSON: str,
```

## DemodulationConfigTypeDef

```python
# DemodulationConfigTypeDef definition

class DemodulationConfigTypeDef(TypedDict):
    unvalidatedJSON: str,
```

## EirpTypeDef

```python
# EirpTypeDef definition

class EirpTypeDef(TypedDict):
    units: EirpUnitsType,  # (1)
    value: float,
```

1. See [:material-code-brackets: EirpUnitsType](./literals.md#eirpunitstype) 
## CancelContactRequestRequestTypeDef

```python
# CancelContactRequestRequestTypeDef definition

class CancelContactRequestRequestTypeDef(TypedDict):
    contactId: str,
```

## ComponentStatusDataTypeDef

```python
# ComponentStatusDataTypeDef definition

class ComponentStatusDataTypeDef(TypedDict):
    capabilityArn: str,
    componentType: str,
    dataflowId: str,
    status: AgentStatusType,  # (1)
    bytesReceived: NotRequired[int],
    bytesSent: NotRequired[int],
    packetsDropped: NotRequired[int],
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype) 
## S3RecordingDetailsTypeDef

```python
# S3RecordingDetailsTypeDef definition

class S3RecordingDetailsTypeDef(TypedDict):
    bucketArn: NotRequired[str],
    keyTemplate: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## ConfigListItemTypeDef

```python
# ConfigListItemTypeDef definition

class ConfigListItemTypeDef(TypedDict):
    configArn: NotRequired[str],
    configId: NotRequired[str],
    configType: NotRequired[ConfigCapabilityTypeType],  # (1)
    name: NotRequired[str],
```

1. See [:material-code-brackets: ConfigCapabilityTypeType](./literals.md#configcapabilitytypetype) 
## DataflowEndpointConfigTypeDef

```python
# DataflowEndpointConfigTypeDef definition

class DataflowEndpointConfigTypeDef(TypedDict):
    dataflowEndpointName: str,
    dataflowEndpointRegion: NotRequired[str],
```

## S3RecordingConfigTypeDef

```python
# S3RecordingConfigTypeDef definition

class S3RecordingConfigTypeDef(TypedDict):
    bucketArn: str,
    roleArn: str,
    prefix: NotRequired[str],
```

## TrackingConfigTypeDef

```python
# TrackingConfigTypeDef definition

class TrackingConfigTypeDef(TypedDict):
    autotrack: CriticalityType,  # (1)
```

1. See [:material-code-brackets: CriticalityType](./literals.md#criticalitytype) 
## UplinkEchoConfigTypeDef

```python
# UplinkEchoConfigTypeDef definition

class UplinkEchoConfigTypeDef(TypedDict):
    antennaUplinkConfigArn: str,
    enabled: bool,
```

## SocketAddressTypeDef

```python
# SocketAddressTypeDef definition

class SocketAddressTypeDef(TypedDict):
    name: str,
    port: int,
```

## ElevationTypeDef

```python
# ElevationTypeDef definition

class ElevationTypeDef(TypedDict):
    unit: AngleUnitsType,  # (1)
    value: float,
```

1. See [:material-code-brackets: AngleUnitsType](./literals.md#angleunitstype) 
## KmsKeyTypeDef

```python
# KmsKeyTypeDef definition

class KmsKeyTypeDef(TypedDict):
    kmsAliasArn: NotRequired[str],
    kmsAliasName: NotRequired[str],
    kmsKeyArn: NotRequired[str],
```

## DataflowEndpointListItemTypeDef

```python
# DataflowEndpointListItemTypeDef definition

class DataflowEndpointListItemTypeDef(TypedDict):
    dataflowEndpointGroupArn: NotRequired[str],
    dataflowEndpointGroupId: NotRequired[str],
```

## DeleteConfigRequestRequestTypeDef

```python
# DeleteConfigRequestRequestTypeDef definition

class DeleteConfigRequestRequestTypeDef(TypedDict):
    configId: str,
    configType: ConfigCapabilityTypeType,  # (1)
```

1. See [:material-code-brackets: ConfigCapabilityTypeType](./literals.md#configcapabilitytypetype) 
## DeleteDataflowEndpointGroupRequestRequestTypeDef

```python
# DeleteDataflowEndpointGroupRequestRequestTypeDef definition

class DeleteDataflowEndpointGroupRequestRequestTypeDef(TypedDict):
    dataflowEndpointGroupId: str,
```

## DeleteEphemerisRequestRequestTypeDef

```python
# DeleteEphemerisRequestRequestTypeDef definition

class DeleteEphemerisRequestRequestTypeDef(TypedDict):
    ephemerisId: str,
```

## DeleteMissionProfileRequestRequestTypeDef

```python
# DeleteMissionProfileRequestRequestTypeDef definition

class DeleteMissionProfileRequestRequestTypeDef(TypedDict):
    missionProfileId: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeContactRequestRequestTypeDef

```python
# DescribeContactRequestRequestTypeDef definition

class DescribeContactRequestRequestTypeDef(TypedDict):
    contactId: str,
```

## DescribeEphemerisRequestRequestTypeDef

```python
# DescribeEphemerisRequestRequestTypeDef definition

class DescribeEphemerisRequestRequestTypeDef(TypedDict):
    ephemerisId: str,
```

## DiscoveryDataTypeDef

```python
# DiscoveryDataTypeDef definition

class DiscoveryDataTypeDef(TypedDict):
    capabilityArns: Sequence[str],
    privateIpAddresses: Sequence[str],
    publicIpAddresses: Sequence[str],
```

## SecurityDetailsOutputTypeDef

```python
# SecurityDetailsOutputTypeDef definition

class SecurityDetailsOutputTypeDef(TypedDict):
    roleArn: str,
    securityGroupIds: List[str],
    subnetIds: List[str],
```

## S3ObjectTypeDef

```python
# S3ObjectTypeDef definition

class S3ObjectTypeDef(TypedDict):
    bucket: NotRequired[str],
    key: NotRequired[str],
    version: NotRequired[str],
```

## EphemerisMetaDataTypeDef

```python
# EphemerisMetaDataTypeDef definition

class EphemerisMetaDataTypeDef(TypedDict):
    source: EphemerisSourceType,  # (1)
    ephemerisId: NotRequired[str],
    epoch: NotRequired[datetime],
    name: NotRequired[str],
```

1. See [:material-code-brackets: EphemerisSourceType](./literals.md#ephemerissourcetype) 
## FrequencyBandwidthTypeDef

```python
# FrequencyBandwidthTypeDef definition

class FrequencyBandwidthTypeDef(TypedDict):
    units: BandwidthUnitsType,  # (1)
    value: float,
```

1. See [:material-code-brackets: BandwidthUnitsType](./literals.md#bandwidthunitstype) 
## FrequencyTypeDef

```python
# FrequencyTypeDef definition

class FrequencyTypeDef(TypedDict):
    units: FrequencyUnitsType,  # (1)
    value: float,
```

1. See [:material-code-brackets: FrequencyUnitsType](./literals.md#frequencyunitstype) 
## GetAgentConfigurationRequestRequestTypeDef

```python
# GetAgentConfigurationRequestRequestTypeDef definition

class GetAgentConfigurationRequestRequestTypeDef(TypedDict):
    agentId: str,
```

## GetConfigRequestRequestTypeDef

```python
# GetConfigRequestRequestTypeDef definition

class GetConfigRequestRequestTypeDef(TypedDict):
    configId: str,
    configType: ConfigCapabilityTypeType,  # (1)
```

1. See [:material-code-brackets: ConfigCapabilityTypeType](./literals.md#configcapabilitytypetype) 
## GetDataflowEndpointGroupRequestRequestTypeDef

```python
# GetDataflowEndpointGroupRequestRequestTypeDef definition

class GetDataflowEndpointGroupRequestRequestTypeDef(TypedDict):
    dataflowEndpointGroupId: str,
```

## GetMinuteUsageRequestRequestTypeDef

```python
# GetMinuteUsageRequestRequestTypeDef definition

class GetMinuteUsageRequestRequestTypeDef(TypedDict):
    month: int,
    year: int,
```

## GetMissionProfileRequestRequestTypeDef

```python
# GetMissionProfileRequestRequestTypeDef definition

class GetMissionProfileRequestRequestTypeDef(TypedDict):
    missionProfileId: str,
```

## GetSatelliteRequestRequestTypeDef

```python
# GetSatelliteRequestRequestTypeDef definition

class GetSatelliteRequestRequestTypeDef(TypedDict):
    satelliteId: str,
```

## GroundStationDataTypeDef

```python
# GroundStationDataTypeDef definition

class GroundStationDataTypeDef(TypedDict):
    groundStationId: NotRequired[str],
    groundStationName: NotRequired[str],
    region: NotRequired[str],
```

## IntegerRangeTypeDef

```python
# IntegerRangeTypeDef definition

class IntegerRangeTypeDef(TypedDict):
    maximum: int,
    minimum: int,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListConfigsRequestRequestTypeDef

```python
# ListConfigsRequestRequestTypeDef definition

class ListConfigsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListDataflowEndpointGroupsRequestRequestTypeDef

```python
# ListDataflowEndpointGroupsRequestRequestTypeDef definition

class ListDataflowEndpointGroupsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListGroundStationsRequestRequestTypeDef

```python
# ListGroundStationsRequestRequestTypeDef definition

class ListGroundStationsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    satelliteId: NotRequired[str],
```

## ListMissionProfilesRequestRequestTypeDef

```python
# ListMissionProfilesRequestRequestTypeDef definition

class ListMissionProfilesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## MissionProfileListItemTypeDef

```python
# MissionProfileListItemTypeDef definition

class MissionProfileListItemTypeDef(TypedDict):
    missionProfileArn: NotRequired[str],
    missionProfileId: NotRequired[str],
    name: NotRequired[str],
    region: NotRequired[str],
```

## ListSatellitesRequestRequestTypeDef

```python
# ListSatellitesRequestRequestTypeDef definition

class ListSatellitesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## SecurityDetailsTypeDef

```python
# SecurityDetailsTypeDef definition

class SecurityDetailsTypeDef(TypedDict):
    roleArn: str,
    securityGroupIds: Sequence[str],
    subnetIds: Sequence[str],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateEphemerisRequestRequestTypeDef

```python
# UpdateEphemerisRequestRequestTypeDef definition

class UpdateEphemerisRequestRequestTypeDef(TypedDict):
    enabled: bool,
    ephemerisId: str,
    name: NotRequired[str],
    priority: NotRequired[int],
```

## AgentDetailsTypeDef

```python
# AgentDetailsTypeDef definition

class AgentDetailsTypeDef(TypedDict):
    agentVersion: str,
    componentVersions: Sequence[ComponentVersionTypeDef],  # (1)
    instanceId: str,
    instanceType: str,
    agentCpuCores: NotRequired[Sequence[int]],
    reservedCpuCores: NotRequired[Sequence[int]],
```

1. See [:material-code-braces: ComponentVersionTypeDef](./type_defs.md#componentversiontypedef) 
## UpdateAgentStatusRequestRequestTypeDef

```python
# UpdateAgentStatusRequestRequestTypeDef definition

class UpdateAgentStatusRequestRequestTypeDef(TypedDict):
    agentId: str,
    aggregateStatus: AggregateStatusTypeDef,  # (1)
    componentStatuses: Sequence[ComponentStatusDataTypeDef],  # (2)
    taskId: str,
```

1. See [:material-code-braces: AggregateStatusTypeDef](./type_defs.md#aggregatestatustypedef) 
2. See [:material-code-braces: ComponentStatusDataTypeDef](./type_defs.md#componentstatusdatatypedef) 
## ConfigIdResponseTypeDef

```python
# ConfigIdResponseTypeDef definition

class ConfigIdResponseTypeDef(TypedDict):
    configArn: str,
    configId: str,
    configType: ConfigCapabilityTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ConfigCapabilityTypeType](./literals.md#configcapabilitytypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ContactIdResponseTypeDef

```python
# ContactIdResponseTypeDef definition

class ContactIdResponseTypeDef(TypedDict):
    contactId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataflowEndpointGroupIdResponseTypeDef

```python
# DataflowEndpointGroupIdResponseTypeDef definition

class DataflowEndpointGroupIdResponseTypeDef(TypedDict):
    dataflowEndpointGroupId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EphemerisIdResponseTypeDef

```python
# EphemerisIdResponseTypeDef definition

class EphemerisIdResponseTypeDef(TypedDict):
    ephemerisId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAgentConfigurationResponseTypeDef

```python
# GetAgentConfigurationResponseTypeDef definition

class GetAgentConfigurationResponseTypeDef(TypedDict):
    agentId: str,
    taskingDocument: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMinuteUsageResponseTypeDef

```python
# GetMinuteUsageResponseTypeDef definition

class GetMinuteUsageResponseTypeDef(TypedDict):
    estimatedMinutesRemaining: int,
    isReservedMinutesCustomer: bool,
    totalReservedMinuteAllocation: int,
    totalScheduledMinutes: int,
    upcomingMinutesScheduled: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MissionProfileIdResponseTypeDef

```python
# MissionProfileIdResponseTypeDef definition

class MissionProfileIdResponseTypeDef(TypedDict):
    missionProfileId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterAgentResponseTypeDef

```python
# RegisterAgentResponseTypeDef definition

class RegisterAgentResponseTypeDef(TypedDict):
    agentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAgentStatusResponseTypeDef

```python
# UpdateAgentStatusResponseTypeDef definition

class UpdateAgentStatusResponseTypeDef(TypedDict):
    agentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfigsResponseTypeDef

```python
# ListConfigsResponseTypeDef definition

class ListConfigsResponseTypeDef(TypedDict):
    configList: List[ConfigListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfigListItemTypeDef](./type_defs.md#configlistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConnectionDetailsTypeDef

```python
# ConnectionDetailsTypeDef definition

class ConnectionDetailsTypeDef(TypedDict):
    socketAddress: SocketAddressTypeDef,  # (1)
    mtu: NotRequired[int],
```

1. See [:material-code-braces: SocketAddressTypeDef](./type_defs.md#socketaddresstypedef) 
## DataflowEndpointTypeDef

```python
# DataflowEndpointTypeDef definition

class DataflowEndpointTypeDef(TypedDict):
    address: NotRequired[SocketAddressTypeDef],  # (1)
    mtu: NotRequired[int],
    name: NotRequired[str],
    status: NotRequired[EndpointStatusType],  # (2)
```

1. See [:material-code-braces: SocketAddressTypeDef](./type_defs.md#socketaddresstypedef) 
2. See [:material-code-brackets: EndpointStatusType](./literals.md#endpointstatustype) 
## ContactDataTypeDef

```python
# ContactDataTypeDef definition

class ContactDataTypeDef(TypedDict):
    contactId: NotRequired[str],
    contactStatus: NotRequired[ContactStatusType],  # (1)
    endTime: NotRequired[datetime],
    errorMessage: NotRequired[str],
    groundStation: NotRequired[str],
    maximumElevation: NotRequired[ElevationTypeDef],  # (2)
    missionProfileArn: NotRequired[str],
    postPassEndTime: NotRequired[datetime],
    prePassStartTime: NotRequired[datetime],
    region: NotRequired[str],
    satelliteArn: NotRequired[str],
    startTime: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
    visibilityEndTime: NotRequired[datetime],
    visibilityStartTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ContactStatusType](./literals.md#contactstatustype) 
2. See [:material-code-braces: ElevationTypeDef](./type_defs.md#elevationtypedef) 
## ListContactsRequestRequestTypeDef

```python
# ListContactsRequestRequestTypeDef definition

class ListContactsRequestRequestTypeDef(TypedDict):
    endTime: TimestampTypeDef,
    startTime: TimestampTypeDef,
    statusList: Sequence[ContactStatusType],  # (1)
    groundStation: NotRequired[str],
    maxResults: NotRequired[int],
    missionProfileArn: NotRequired[str],
    nextToken: NotRequired[str],
    satelliteArn: NotRequired[str],
```

1. See [:material-code-brackets: ContactStatusType](./literals.md#contactstatustype) 
## ListEphemeridesRequestRequestTypeDef

```python
# ListEphemeridesRequestRequestTypeDef definition

class ListEphemeridesRequestRequestTypeDef(TypedDict):
    endTime: TimestampTypeDef,
    satelliteId: str,
    startTime: TimestampTypeDef,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    statusList: NotRequired[Sequence[EphemerisStatusType]],  # (1)
```

1. See [:material-code-brackets: EphemerisStatusType](./literals.md#ephemerisstatustype) 
## ReserveContactRequestRequestTypeDef

```python
# ReserveContactRequestRequestTypeDef definition

class ReserveContactRequestRequestTypeDef(TypedDict):
    endTime: TimestampTypeDef,
    groundStation: str,
    missionProfileArn: str,
    satelliteArn: str,
    startTime: TimestampTypeDef,
    tags: NotRequired[Mapping[str, str]],
```

## TimeRangeTypeDef

```python
# TimeRangeTypeDef definition

class TimeRangeTypeDef(TypedDict):
    endTime: TimestampTypeDef,
    startTime: TimestampTypeDef,
```

## CreateMissionProfileRequestRequestTypeDef

```python
# CreateMissionProfileRequestRequestTypeDef definition

class CreateMissionProfileRequestRequestTypeDef(TypedDict):
    dataflowEdges: Sequence[Sequence[str]],
    minimumViableContactDurationSeconds: int,
    name: str,
    trackingConfigArn: str,
    contactPostPassDurationSeconds: NotRequired[int],
    contactPrePassDurationSeconds: NotRequired[int],
    streamsKmsKey: NotRequired[KmsKeyTypeDef],  # (1)
    streamsKmsRole: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: KmsKeyTypeDef](./type_defs.md#kmskeytypedef) 
## GetMissionProfileResponseTypeDef

```python
# GetMissionProfileResponseTypeDef definition

class GetMissionProfileResponseTypeDef(TypedDict):
    contactPostPassDurationSeconds: int,
    contactPrePassDurationSeconds: int,
    dataflowEdges: List[List[str]],
    minimumViableContactDurationSeconds: int,
    missionProfileArn: str,
    missionProfileId: str,
    name: str,
    region: str,
    streamsKmsKey: KmsKeyTypeDef,  # (1)
    streamsKmsRole: str,
    tags: Dict[str, str],
    trackingConfigArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KmsKeyTypeDef](./type_defs.md#kmskeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMissionProfileRequestRequestTypeDef

```python
# UpdateMissionProfileRequestRequestTypeDef definition

class UpdateMissionProfileRequestRequestTypeDef(TypedDict):
    missionProfileId: str,
    contactPostPassDurationSeconds: NotRequired[int],
    contactPrePassDurationSeconds: NotRequired[int],
    dataflowEdges: NotRequired[Sequence[Sequence[str]]],
    minimumViableContactDurationSeconds: NotRequired[int],
    name: NotRequired[str],
    streamsKmsKey: NotRequired[KmsKeyTypeDef],  # (1)
    streamsKmsRole: NotRequired[str],
    trackingConfigArn: NotRequired[str],
```

1. See [:material-code-braces: KmsKeyTypeDef](./type_defs.md#kmskeytypedef) 
## ListDataflowEndpointGroupsResponseTypeDef

```python
# ListDataflowEndpointGroupsResponseTypeDef definition

class ListDataflowEndpointGroupsResponseTypeDef(TypedDict):
    dataflowEndpointGroupList: List[DataflowEndpointListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DataflowEndpointListItemTypeDef](./type_defs.md#dataflowendpointlistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeContactRequestContactScheduledWaitTypeDef

```python
# DescribeContactRequestContactScheduledWaitTypeDef definition

class DescribeContactRequestContactScheduledWaitTypeDef(TypedDict):
    contactId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## EphemerisDescriptionTypeDef

```python
# EphemerisDescriptionTypeDef definition

class EphemerisDescriptionTypeDef(TypedDict):
    ephemerisData: NotRequired[str],
    sourceS3Object: NotRequired[S3ObjectTypeDef],  # (1)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
## EphemerisItemTypeDef

```python
# EphemerisItemTypeDef definition

class EphemerisItemTypeDef(TypedDict):
    creationTime: NotRequired[datetime],
    enabled: NotRequired[bool],
    ephemerisId: NotRequired[str],
    name: NotRequired[str],
    priority: NotRequired[int],
    sourceS3Object: NotRequired[S3ObjectTypeDef],  # (1)
    status: NotRequired[EphemerisStatusType],  # (2)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
2. See [:material-code-brackets: EphemerisStatusType](./literals.md#ephemerisstatustype) 
## OEMEphemerisTypeDef

```python
# OEMEphemerisTypeDef definition

class OEMEphemerisTypeDef(TypedDict):
    oemData: NotRequired[str],
    s3Object: NotRequired[S3ObjectTypeDef],  # (1)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
## GetSatelliteResponseTypeDef

```python
# GetSatelliteResponseTypeDef definition

class GetSatelliteResponseTypeDef(TypedDict):
    currentEphemeris: EphemerisMetaDataTypeDef,  # (1)
    groundStations: List[str],
    noradSatelliteID: int,
    satelliteArn: str,
    satelliteId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EphemerisMetaDataTypeDef](./type_defs.md#ephemerismetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SatelliteListItemTypeDef

```python
# SatelliteListItemTypeDef definition

class SatelliteListItemTypeDef(TypedDict):
    currentEphemeris: NotRequired[EphemerisMetaDataTypeDef],  # (1)
    groundStations: NotRequired[List[str]],
    noradSatelliteID: NotRequired[int],
    satelliteArn: NotRequired[str],
    satelliteId: NotRequired[str],
```

1. See [:material-code-braces: EphemerisMetaDataTypeDef](./type_defs.md#ephemerismetadatatypedef) 
## SpectrumConfigTypeDef

```python
# SpectrumConfigTypeDef definition

class SpectrumConfigTypeDef(TypedDict):
    bandwidth: FrequencyBandwidthTypeDef,  # (1)
    centerFrequency: FrequencyTypeDef,  # (2)
    polarization: NotRequired[PolarizationType],  # (3)
```

1. See [:material-code-braces: FrequencyBandwidthTypeDef](./type_defs.md#frequencybandwidthtypedef) 
2. See [:material-code-braces: FrequencyTypeDef](./type_defs.md#frequencytypedef) 
3. See [:material-code-brackets: PolarizationType](./literals.md#polarizationtype) 
## UplinkSpectrumConfigTypeDef

```python
# UplinkSpectrumConfigTypeDef definition

class UplinkSpectrumConfigTypeDef(TypedDict):
    centerFrequency: FrequencyTypeDef,  # (1)
    polarization: NotRequired[PolarizationType],  # (2)
```

1. See [:material-code-braces: FrequencyTypeDef](./type_defs.md#frequencytypedef) 
2. See [:material-code-brackets: PolarizationType](./literals.md#polarizationtype) 
## ListGroundStationsResponseTypeDef

```python
# ListGroundStationsResponseTypeDef definition

class ListGroundStationsResponseTypeDef(TypedDict):
    groundStationList: List[GroundStationDataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: GroundStationDataTypeDef](./type_defs.md#groundstationdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RangedSocketAddressTypeDef

```python
# RangedSocketAddressTypeDef definition

class RangedSocketAddressTypeDef(TypedDict):
    name: str,
    portRange: IntegerRangeTypeDef,  # (1)
```

1. See [:material-code-braces: IntegerRangeTypeDef](./type_defs.md#integerrangetypedef) 
## ListConfigsRequestListConfigsPaginateTypeDef

```python
# ListConfigsRequestListConfigsPaginateTypeDef definition

class ListConfigsRequestListConfigsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListContactsRequestListContactsPaginateTypeDef

```python
# ListContactsRequestListContactsPaginateTypeDef definition

class ListContactsRequestListContactsPaginateTypeDef(TypedDict):
    endTime: TimestampTypeDef,
    startTime: TimestampTypeDef,
    statusList: Sequence[ContactStatusType],  # (1)
    groundStation: NotRequired[str],
    missionProfileArn: NotRequired[str],
    satelliteArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ContactStatusType](./literals.md#contactstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef

```python
# ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef definition

class ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEphemeridesRequestListEphemeridesPaginateTypeDef

```python
# ListEphemeridesRequestListEphemeridesPaginateTypeDef definition

class ListEphemeridesRequestListEphemeridesPaginateTypeDef(TypedDict):
    endTime: TimestampTypeDef,
    satelliteId: str,
    startTime: TimestampTypeDef,
    statusList: NotRequired[Sequence[EphemerisStatusType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: EphemerisStatusType](./literals.md#ephemerisstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroundStationsRequestListGroundStationsPaginateTypeDef

```python
# ListGroundStationsRequestListGroundStationsPaginateTypeDef definition

class ListGroundStationsRequestListGroundStationsPaginateTypeDef(TypedDict):
    satelliteId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMissionProfilesRequestListMissionProfilesPaginateTypeDef

```python
# ListMissionProfilesRequestListMissionProfilesPaginateTypeDef definition

class ListMissionProfilesRequestListMissionProfilesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSatellitesRequestListSatellitesPaginateTypeDef

```python
# ListSatellitesRequestListSatellitesPaginateTypeDef definition

class ListSatellitesRequestListSatellitesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMissionProfilesResponseTypeDef

```python
# ListMissionProfilesResponseTypeDef definition

class ListMissionProfilesResponseTypeDef(TypedDict):
    missionProfileList: List[MissionProfileListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MissionProfileListItemTypeDef](./type_defs.md#missionprofilelistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterAgentRequestRequestTypeDef

```python
# RegisterAgentRequestRequestTypeDef definition

class RegisterAgentRequestRequestTypeDef(TypedDict):
    agentDetails: AgentDetailsTypeDef,  # (1)
    discoveryData: DiscoveryDataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentDetailsTypeDef](./type_defs.md#agentdetailstypedef) 
2. See [:material-code-braces: DiscoveryDataTypeDef](./type_defs.md#discoverydatatypedef) 
## ListContactsResponseTypeDef

```python
# ListContactsResponseTypeDef definition

class ListContactsResponseTypeDef(TypedDict):
    contactList: List[ContactDataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ContactDataTypeDef](./type_defs.md#contactdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TLEDataTypeDef

```python
# TLEDataTypeDef definition

class TLEDataTypeDef(TypedDict):
    tleLine1: str,
    tleLine2: str,
    validTimeRange: TimeRangeTypeDef,  # (1)
```

1. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
## EphemerisTypeDescriptionTypeDef

```python
# EphemerisTypeDescriptionTypeDef definition

class EphemerisTypeDescriptionTypeDef(TypedDict):
    oem: NotRequired[EphemerisDescriptionTypeDef],  # (1)
    tle: NotRequired[EphemerisDescriptionTypeDef],  # (1)
```

1. See [:material-code-braces: EphemerisDescriptionTypeDef](./type_defs.md#ephemerisdescriptiontypedef) 
2. See [:material-code-braces: EphemerisDescriptionTypeDef](./type_defs.md#ephemerisdescriptiontypedef) 
## ListEphemeridesResponseTypeDef

```python
# ListEphemeridesResponseTypeDef definition

class ListEphemeridesResponseTypeDef(TypedDict):
    ephemerides: List[EphemerisItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EphemerisItemTypeDef](./type_defs.md#ephemerisitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSatellitesResponseTypeDef

```python
# ListSatellitesResponseTypeDef definition

class ListSatellitesResponseTypeDef(TypedDict):
    satellites: List[SatelliteListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SatelliteListItemTypeDef](./type_defs.md#satellitelistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AntennaDownlinkConfigTypeDef

```python
# AntennaDownlinkConfigTypeDef definition

class AntennaDownlinkConfigTypeDef(TypedDict):
    spectrumConfig: SpectrumConfigTypeDef,  # (1)
```

1. See [:material-code-braces: SpectrumConfigTypeDef](./type_defs.md#spectrumconfigtypedef) 
## AntennaDownlinkDemodDecodeConfigTypeDef

```python
# AntennaDownlinkDemodDecodeConfigTypeDef definition

class AntennaDownlinkDemodDecodeConfigTypeDef(TypedDict):
    decodeConfig: DecodeConfigTypeDef,  # (1)
    demodulationConfig: DemodulationConfigTypeDef,  # (2)
    spectrumConfig: SpectrumConfigTypeDef,  # (3)
```

1. See [:material-code-braces: DecodeConfigTypeDef](./type_defs.md#decodeconfigtypedef) 
2. See [:material-code-braces: DemodulationConfigTypeDef](./type_defs.md#demodulationconfigtypedef) 
3. See [:material-code-braces: SpectrumConfigTypeDef](./type_defs.md#spectrumconfigtypedef) 
## AntennaUplinkConfigTypeDef

```python
# AntennaUplinkConfigTypeDef definition

class AntennaUplinkConfigTypeDef(TypedDict):
    spectrumConfig: UplinkSpectrumConfigTypeDef,  # (1)
    targetEirp: EirpTypeDef,  # (2)
    transmitDisabled: NotRequired[bool],
```

1. See [:material-code-braces: UplinkSpectrumConfigTypeDef](./type_defs.md#uplinkspectrumconfigtypedef) 
2. See [:material-code-braces: EirpTypeDef](./type_defs.md#eirptypedef) 
## RangedConnectionDetailsTypeDef

```python
# RangedConnectionDetailsTypeDef definition

class RangedConnectionDetailsTypeDef(TypedDict):
    socketAddress: RangedSocketAddressTypeDef,  # (1)
    mtu: NotRequired[int],
```

1. See [:material-code-braces: RangedSocketAddressTypeDef](./type_defs.md#rangedsocketaddresstypedef) 
## TLEEphemerisTypeDef

```python
# TLEEphemerisTypeDef definition

class TLEEphemerisTypeDef(TypedDict):
    s3Object: NotRequired[S3ObjectTypeDef],  # (1)
    tleData: NotRequired[Sequence[TLEDataTypeDef]],  # (2)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
2. See [:material-code-braces: TLEDataTypeDef](./type_defs.md#tledatatypedef) 
## DescribeEphemerisResponseTypeDef

```python
# DescribeEphemerisResponseTypeDef definition

class DescribeEphemerisResponseTypeDef(TypedDict):
    creationTime: datetime,
    enabled: bool,
    ephemerisId: str,
    invalidReason: EphemerisInvalidReasonType,  # (1)
    name: str,
    priority: int,
    satelliteId: str,
    status: EphemerisStatusType,  # (2)
    suppliedData: EphemerisTypeDescriptionTypeDef,  # (3)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: EphemerisInvalidReasonType](./literals.md#ephemerisinvalidreasontype) 
2. See [:material-code-brackets: EphemerisStatusType](./literals.md#ephemerisstatustype) 
3. See [:material-code-braces: EphemerisTypeDescriptionTypeDef](./type_defs.md#ephemeristypedescriptiontypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfigTypeDataTypeDef

```python
# ConfigTypeDataTypeDef definition

class ConfigTypeDataTypeDef(TypedDict):
    antennaDownlinkConfig: NotRequired[AntennaDownlinkConfigTypeDef],  # (1)
    antennaDownlinkDemodDecodeConfig: NotRequired[AntennaDownlinkDemodDecodeConfigTypeDef],  # (2)
    antennaUplinkConfig: NotRequired[AntennaUplinkConfigTypeDef],  # (3)
    dataflowEndpointConfig: NotRequired[DataflowEndpointConfigTypeDef],  # (4)
    s3RecordingConfig: NotRequired[S3RecordingConfigTypeDef],  # (5)
    trackingConfig: NotRequired[TrackingConfigTypeDef],  # (6)
    uplinkEchoConfig: NotRequired[UplinkEchoConfigTypeDef],  # (7)
```

1. See [:material-code-braces: AntennaDownlinkConfigTypeDef](./type_defs.md#antennadownlinkconfigtypedef) 
2. See [:material-code-braces: AntennaDownlinkDemodDecodeConfigTypeDef](./type_defs.md#antennadownlinkdemoddecodeconfigtypedef) 
3. See [:material-code-braces: AntennaUplinkConfigTypeDef](./type_defs.md#antennauplinkconfigtypedef) 
4. See [:material-code-braces: DataflowEndpointConfigTypeDef](./type_defs.md#dataflowendpointconfigtypedef) 
5. See [:material-code-braces: S3RecordingConfigTypeDef](./type_defs.md#s3recordingconfigtypedef) 
6. See [:material-code-braces: TrackingConfigTypeDef](./type_defs.md#trackingconfigtypedef) 
7. See [:material-code-braces: UplinkEchoConfigTypeDef](./type_defs.md#uplinkechoconfigtypedef) 
## AwsGroundStationAgentEndpointTypeDef

```python
# AwsGroundStationAgentEndpointTypeDef definition

class AwsGroundStationAgentEndpointTypeDef(TypedDict):
    egressAddress: ConnectionDetailsTypeDef,  # (3)
    ingressAddress: RangedConnectionDetailsTypeDef,  # (4)
    name: str,
    agentStatus: NotRequired[AgentStatusType],  # (1)
    auditResults: NotRequired[AuditResultsType],  # (2)
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype) 
2. See [:material-code-brackets: AuditResultsType](./literals.md#auditresultstype) 
3. See [:material-code-braces: ConnectionDetailsTypeDef](./type_defs.md#connectiondetailstypedef) 
4. See [:material-code-braces: RangedConnectionDetailsTypeDef](./type_defs.md#rangedconnectiondetailstypedef) 
## EphemerisDataTypeDef

```python
# EphemerisDataTypeDef definition

class EphemerisDataTypeDef(TypedDict):
    oem: NotRequired[OEMEphemerisTypeDef],  # (1)
    tle: NotRequired[TLEEphemerisTypeDef],  # (2)
```

1. See [:material-code-braces: OEMEphemerisTypeDef](./type_defs.md#oemephemeristypedef) 
2. See [:material-code-braces: TLEEphemerisTypeDef](./type_defs.md#tleephemeristypedef) 
## CreateConfigRequestRequestTypeDef

```python
# CreateConfigRequestRequestTypeDef definition

class CreateConfigRequestRequestTypeDef(TypedDict):
    configData: ConfigTypeDataTypeDef,  # (1)
    name: str,
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ConfigTypeDataTypeDef](./type_defs.md#configtypedatatypedef) 
## GetConfigResponseTypeDef

```python
# GetConfigResponseTypeDef definition

class GetConfigResponseTypeDef(TypedDict):
    configArn: str,
    configData: ConfigTypeDataTypeDef,  # (1)
    configId: str,
    configType: ConfigCapabilityTypeType,  # (2)
    name: str,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConfigTypeDataTypeDef](./type_defs.md#configtypedatatypedef) 
2. See [:material-code-brackets: ConfigCapabilityTypeType](./literals.md#configcapabilitytypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConfigRequestRequestTypeDef

```python
# UpdateConfigRequestRequestTypeDef definition

class UpdateConfigRequestRequestTypeDef(TypedDict):
    configData: ConfigTypeDataTypeDef,  # (1)
    configId: str,
    configType: ConfigCapabilityTypeType,  # (2)
    name: str,
```

1. See [:material-code-braces: ConfigTypeDataTypeDef](./type_defs.md#configtypedatatypedef) 
2. See [:material-code-brackets: ConfigCapabilityTypeType](./literals.md#configcapabilitytypetype) 
## EndpointDetailsOutputTypeDef

```python
# EndpointDetailsOutputTypeDef definition

class EndpointDetailsOutputTypeDef(TypedDict):
    awsGroundStationAgentEndpoint: NotRequired[AwsGroundStationAgentEndpointTypeDef],  # (1)
    endpoint: NotRequired[DataflowEndpointTypeDef],  # (2)
    healthReasons: NotRequired[List[CapabilityHealthReasonType]],  # (3)
    healthStatus: NotRequired[CapabilityHealthType],  # (4)
    securityDetails: NotRequired[SecurityDetailsOutputTypeDef],  # (5)
```

1. See [:material-code-braces: AwsGroundStationAgentEndpointTypeDef](./type_defs.md#awsgroundstationagentendpointtypedef) 
2. See [:material-code-braces: DataflowEndpointTypeDef](./type_defs.md#dataflowendpointtypedef) 
3. See [:material-code-brackets: CapabilityHealthReasonType](./literals.md#capabilityhealthreasontype) 
4. See [:material-code-brackets: CapabilityHealthType](./literals.md#capabilityhealthtype) 
5. See [:material-code-braces: SecurityDetailsOutputTypeDef](./type_defs.md#securitydetailsoutputtypedef) 
## EndpointDetailsTypeDef

```python
# EndpointDetailsTypeDef definition

class EndpointDetailsTypeDef(TypedDict):
    awsGroundStationAgentEndpoint: NotRequired[AwsGroundStationAgentEndpointTypeDef],  # (1)
    endpoint: NotRequired[DataflowEndpointTypeDef],  # (2)
    healthReasons: NotRequired[Sequence[CapabilityHealthReasonType]],  # (3)
    healthStatus: NotRequired[CapabilityHealthType],  # (4)
    securityDetails: NotRequired[SecurityDetailsUnionTypeDef],  # (5)
```

1. See [:material-code-braces: AwsGroundStationAgentEndpointTypeDef](./type_defs.md#awsgroundstationagentendpointtypedef) 
2. See [:material-code-braces: DataflowEndpointTypeDef](./type_defs.md#dataflowendpointtypedef) 
3. See [:material-code-brackets: CapabilityHealthReasonType](./literals.md#capabilityhealthreasontype) 
4. See [:material-code-brackets: CapabilityHealthType](./literals.md#capabilityhealthtype) 
5. See [:material-code-braces: SecurityDetailsTypeDef](./type_defs.md#securitydetailstypedef) [:material-code-braces: SecurityDetailsOutputTypeDef](./type_defs.md#securitydetailsoutputtypedef) 
## CreateEphemerisRequestRequestTypeDef

```python
# CreateEphemerisRequestRequestTypeDef definition

class CreateEphemerisRequestRequestTypeDef(TypedDict):
    name: str,
    satelliteId: str,
    enabled: NotRequired[bool],
    ephemeris: NotRequired[EphemerisDataTypeDef],  # (1)
    expirationTime: NotRequired[TimestampTypeDef],
    kmsKeyArn: NotRequired[str],
    priority: NotRequired[int],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: EphemerisDataTypeDef](./type_defs.md#ephemerisdatatypedef) 
## ConfigDetailsTypeDef

```python
# ConfigDetailsTypeDef definition

class ConfigDetailsTypeDef(TypedDict):
    antennaDemodDecodeDetails: NotRequired[AntennaDemodDecodeDetailsTypeDef],  # (1)
    endpointDetails: NotRequired[EndpointDetailsOutputTypeDef],  # (2)
    s3RecordingDetails: NotRequired[S3RecordingDetailsTypeDef],  # (3)
```

1. See [:material-code-braces: AntennaDemodDecodeDetailsTypeDef](./type_defs.md#antennademoddecodedetailstypedef) 
2. See [:material-code-braces: EndpointDetailsOutputTypeDef](./type_defs.md#endpointdetailsoutputtypedef) 
3. See [:material-code-braces: S3RecordingDetailsTypeDef](./type_defs.md#s3recordingdetailstypedef) 
## GetDataflowEndpointGroupResponseTypeDef

```python
# GetDataflowEndpointGroupResponseTypeDef definition

class GetDataflowEndpointGroupResponseTypeDef(TypedDict):
    contactPostPassDurationSeconds: int,
    contactPrePassDurationSeconds: int,
    dataflowEndpointGroupArn: str,
    dataflowEndpointGroupId: str,
    endpointsDetails: List[EndpointDetailsOutputTypeDef],  # (1)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointDetailsOutputTypeDef](./type_defs.md#endpointdetailsoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DestinationTypeDef

```python
# DestinationTypeDef definition

class DestinationTypeDef(TypedDict):
    configDetails: NotRequired[ConfigDetailsTypeDef],  # (1)
    configId: NotRequired[str],
    configType: NotRequired[ConfigCapabilityTypeType],  # (2)
    dataflowDestinationRegion: NotRequired[str],
```

1. See [:material-code-braces: ConfigDetailsTypeDef](./type_defs.md#configdetailstypedef) 
2. See [:material-code-brackets: ConfigCapabilityTypeType](./literals.md#configcapabilitytypetype) 
## SourceTypeDef

```python
# SourceTypeDef definition

class SourceTypeDef(TypedDict):
    configDetails: NotRequired[ConfigDetailsTypeDef],  # (1)
    configId: NotRequired[str],
    configType: NotRequired[ConfigCapabilityTypeType],  # (2)
    dataflowSourceRegion: NotRequired[str],
```

1. See [:material-code-braces: ConfigDetailsTypeDef](./type_defs.md#configdetailstypedef) 
2. See [:material-code-brackets: ConfigCapabilityTypeType](./literals.md#configcapabilitytypetype) 
## CreateDataflowEndpointGroupRequestRequestTypeDef

```python
# CreateDataflowEndpointGroupRequestRequestTypeDef definition

class CreateDataflowEndpointGroupRequestRequestTypeDef(TypedDict):
    endpointDetails: Sequence[EndpointDetailsUnionTypeDef],  # (1)
    contactPostPassDurationSeconds: NotRequired[int],
    contactPrePassDurationSeconds: NotRequired[int],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: EndpointDetailsTypeDef](./type_defs.md#endpointdetailstypedef) [:material-code-braces: EndpointDetailsOutputTypeDef](./type_defs.md#endpointdetailsoutputtypedef) 
## DataflowDetailTypeDef

```python
# DataflowDetailTypeDef definition

class DataflowDetailTypeDef(TypedDict):
    destination: NotRequired[DestinationTypeDef],  # (1)
    errorMessage: NotRequired[str],
    source: NotRequired[SourceTypeDef],  # (2)
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
## DescribeContactResponseTypeDef

```python
# DescribeContactResponseTypeDef definition

class DescribeContactResponseTypeDef(TypedDict):
    contactId: str,
    contactStatus: ContactStatusType,  # (1)
    dataflowList: List[DataflowDetailTypeDef],  # (2)
    endTime: datetime,
    errorMessage: str,
    groundStation: str,
    maximumElevation: ElevationTypeDef,  # (3)
    missionProfileArn: str,
    postPassEndTime: datetime,
    prePassStartTime: datetime,
    region: str,
    satelliteArn: str,
    startTime: datetime,
    tags: Dict[str, str],
    visibilityEndTime: datetime,
    visibilityStartTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ContactStatusType](./literals.md#contactstatustype) 
2. See [:material-code-braces: DataflowDetailTypeDef](./type_defs.md#dataflowdetailtypedef) 
3. See [:material-code-braces: ElevationTypeDef](./type_defs.md#elevationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
