# Type definitions

> [Index](../README.md) > [GroundStation](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [GroundStation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#groundstation)
    type annotations stubs module [types-aiobotocore-groundstation](https://pypi.org/project/types-aiobotocore-groundstation/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_groundstation.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## SecurityDetailsUnionTypeDef

```python
# SecurityDetailsUnionTypeDef Union usage example

from types_aiobotocore_groundstation.type_defs import SecurityDetailsUnionTypeDef


def get_value() -> SecurityDetailsUnionTypeDef:
    return ...


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
# EndpointDetailsUnionTypeDef Union usage example

from types_aiobotocore_groundstation.type_defs import EndpointDetailsUnionTypeDef


def get_value() -> EndpointDetailsUnionTypeDef:
    return ...


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
# ComponentVersionTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ComponentVersionTypeDef


def get_value() -> ComponentVersionTypeDef:
    return {
        "componentType": ...,
    }


# ComponentVersionTypeDef definition

class ComponentVersionTypeDef(TypedDict):
    componentType: str,
    versions: Sequence[str],
```

## AggregateStatusTypeDef

```python
# AggregateStatusTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import AggregateStatusTypeDef


def get_value() -> AggregateStatusTypeDef:
    return {
        "signatureMap": ...,
    }


# AggregateStatusTypeDef definition

class AggregateStatusTypeDef(TypedDict):
    status: AgentStatusType,  # (1)
    signatureMap: NotRequired[Mapping[str, bool]],
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype) 
## AntennaDemodDecodeDetailsTypeDef

```python
# AntennaDemodDecodeDetailsTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import AntennaDemodDecodeDetailsTypeDef


def get_value() -> AntennaDemodDecodeDetailsTypeDef:
    return {
        "outputNode": ...,
    }


# AntennaDemodDecodeDetailsTypeDef definition

class AntennaDemodDecodeDetailsTypeDef(TypedDict):
    outputNode: NotRequired[str],
```

## DecodeConfigTypeDef

```python
# DecodeConfigTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import DecodeConfigTypeDef


def get_value() -> DecodeConfigTypeDef:
    return {
        "unvalidatedJSON": ...,
    }


# DecodeConfigTypeDef definition

class DecodeConfigTypeDef(TypedDict):
    unvalidatedJSON: str,
```

## DemodulationConfigTypeDef

```python
# DemodulationConfigTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import DemodulationConfigTypeDef


def get_value() -> DemodulationConfigTypeDef:
    return {
        "unvalidatedJSON": ...,
    }


# DemodulationConfigTypeDef definition

class DemodulationConfigTypeDef(TypedDict):
    unvalidatedJSON: str,
```

## EirpTypeDef

```python
# EirpTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import EirpTypeDef


def get_value() -> EirpTypeDef:
    return {
        "units": ...,
    }


# EirpTypeDef definition

class EirpTypeDef(TypedDict):
    units: EirpUnitsType,  # (1)
    value: float,
```

1. See [:material-code-brackets: EirpUnitsType](./literals.md#eirpunitstype) 
## CancelContactRequestTypeDef

```python
# CancelContactRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import CancelContactRequestTypeDef


def get_value() -> CancelContactRequestTypeDef:
    return {
        "contactId": ...,
    }


# CancelContactRequestTypeDef definition

class CancelContactRequestTypeDef(TypedDict):
    contactId: str,
```

## ComponentStatusDataTypeDef

```python
# ComponentStatusDataTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ComponentStatusDataTypeDef


def get_value() -> ComponentStatusDataTypeDef:
    return {
        "bytesReceived": ...,
    }


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
# S3RecordingDetailsTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import S3RecordingDetailsTypeDef


def get_value() -> S3RecordingDetailsTypeDef:
    return {
        "bucketArn": ...,
    }


# S3RecordingDetailsTypeDef definition

class S3RecordingDetailsTypeDef(TypedDict):
    bucketArn: NotRequired[str],
    keyTemplate: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


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
# ConfigListItemTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ConfigListItemTypeDef


def get_value() -> ConfigListItemTypeDef:
    return {
        "configArn": ...,
    }


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
# DataflowEndpointConfigTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import DataflowEndpointConfigTypeDef


def get_value() -> DataflowEndpointConfigTypeDef:
    return {
        "dataflowEndpointName": ...,
    }


# DataflowEndpointConfigTypeDef definition

class DataflowEndpointConfigTypeDef(TypedDict):
    dataflowEndpointName: str,
    dataflowEndpointRegion: NotRequired[str],
```

## S3RecordingConfigTypeDef

```python
# S3RecordingConfigTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import S3RecordingConfigTypeDef


def get_value() -> S3RecordingConfigTypeDef:
    return {
        "bucketArn": ...,
    }


# S3RecordingConfigTypeDef definition

class S3RecordingConfigTypeDef(TypedDict):
    bucketArn: str,
    roleArn: str,
    prefix: NotRequired[str],
```

## TrackingConfigTypeDef

```python
# TrackingConfigTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import TrackingConfigTypeDef


def get_value() -> TrackingConfigTypeDef:
    return {
        "autotrack": ...,
    }


# TrackingConfigTypeDef definition

class TrackingConfigTypeDef(TypedDict):
    autotrack: CriticalityType,  # (1)
```

1. See [:material-code-brackets: CriticalityType](./literals.md#criticalitytype) 
## UplinkEchoConfigTypeDef

```python
# UplinkEchoConfigTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import UplinkEchoConfigTypeDef


def get_value() -> UplinkEchoConfigTypeDef:
    return {
        "antennaUplinkConfigArn": ...,
    }


# UplinkEchoConfigTypeDef definition

class UplinkEchoConfigTypeDef(TypedDict):
    antennaUplinkConfigArn: str,
    enabled: bool,
```

## SocketAddressTypeDef

```python
# SocketAddressTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import SocketAddressTypeDef


def get_value() -> SocketAddressTypeDef:
    return {
        "name": ...,
    }


# SocketAddressTypeDef definition

class SocketAddressTypeDef(TypedDict):
    name: str,
    port: int,
```

## ElevationTypeDef

```python
# ElevationTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ElevationTypeDef


def get_value() -> ElevationTypeDef:
    return {
        "unit": ...,
    }


# ElevationTypeDef definition

class ElevationTypeDef(TypedDict):
    unit: AngleUnitsType,  # (1)
    value: float,
```

1. See [:material-code-brackets: AngleUnitsType](./literals.md#angleunitstype) 
## KmsKeyTypeDef

```python
# KmsKeyTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import KmsKeyTypeDef


def get_value() -> KmsKeyTypeDef:
    return {
        "kmsAliasArn": ...,
    }


# KmsKeyTypeDef definition

class KmsKeyTypeDef(TypedDict):
    kmsAliasArn: NotRequired[str],
    kmsAliasName: NotRequired[str],
    kmsKeyArn: NotRequired[str],
```

## DataflowEndpointListItemTypeDef

```python
# DataflowEndpointListItemTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import DataflowEndpointListItemTypeDef


def get_value() -> DataflowEndpointListItemTypeDef:
    return {
        "dataflowEndpointGroupArn": ...,
    }


# DataflowEndpointListItemTypeDef definition

class DataflowEndpointListItemTypeDef(TypedDict):
    dataflowEndpointGroupArn: NotRequired[str],
    dataflowEndpointGroupId: NotRequired[str],
```

## DeleteConfigRequestTypeDef

```python
# DeleteConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import DeleteConfigRequestTypeDef


def get_value() -> DeleteConfigRequestTypeDef:
    return {
        "configId": ...,
    }


# DeleteConfigRequestTypeDef definition

class DeleteConfigRequestTypeDef(TypedDict):
    configId: str,
    configType: ConfigCapabilityTypeType,  # (1)
```

1. See [:material-code-brackets: ConfigCapabilityTypeType](./literals.md#configcapabilitytypetype) 
## DeleteDataflowEndpointGroupRequestTypeDef

```python
# DeleteDataflowEndpointGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import DeleteDataflowEndpointGroupRequestTypeDef


def get_value() -> DeleteDataflowEndpointGroupRequestTypeDef:
    return {
        "dataflowEndpointGroupId": ...,
    }


# DeleteDataflowEndpointGroupRequestTypeDef definition

class DeleteDataflowEndpointGroupRequestTypeDef(TypedDict):
    dataflowEndpointGroupId: str,
```

## DeleteEphemerisRequestTypeDef

```python
# DeleteEphemerisRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import DeleteEphemerisRequestTypeDef


def get_value() -> DeleteEphemerisRequestTypeDef:
    return {
        "ephemerisId": ...,
    }


# DeleteEphemerisRequestTypeDef definition

class DeleteEphemerisRequestTypeDef(TypedDict):
    ephemerisId: str,
```

## DeleteMissionProfileRequestTypeDef

```python
# DeleteMissionProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import DeleteMissionProfileRequestTypeDef


def get_value() -> DeleteMissionProfileRequestTypeDef:
    return {
        "missionProfileId": ...,
    }


# DeleteMissionProfileRequestTypeDef definition

class DeleteMissionProfileRequestTypeDef(TypedDict):
    missionProfileId: str,
```

## DescribeContactRequestTypeDef

```python
# DescribeContactRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import DescribeContactRequestTypeDef


def get_value() -> DescribeContactRequestTypeDef:
    return {
        "contactId": ...,
    }


# DescribeContactRequestTypeDef definition

class DescribeContactRequestTypeDef(TypedDict):
    contactId: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import WaiterConfigTypeDef


def get_value() -> WaiterConfigTypeDef:
    return {
        "Delay": ...,
    }


# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeEphemerisRequestTypeDef

```python
# DescribeEphemerisRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import DescribeEphemerisRequestTypeDef


def get_value() -> DescribeEphemerisRequestTypeDef:
    return {
        "ephemerisId": ...,
    }


# DescribeEphemerisRequestTypeDef definition

class DescribeEphemerisRequestTypeDef(TypedDict):
    ephemerisId: str,
```

## DiscoveryDataTypeDef

```python
# DiscoveryDataTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import DiscoveryDataTypeDef


def get_value() -> DiscoveryDataTypeDef:
    return {
        "capabilityArns": ...,
    }


# DiscoveryDataTypeDef definition

class DiscoveryDataTypeDef(TypedDict):
    capabilityArns: Sequence[str],
    privateIpAddresses: Sequence[str],
    publicIpAddresses: Sequence[str],
```

## SecurityDetailsOutputTypeDef

```python
# SecurityDetailsOutputTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import SecurityDetailsOutputTypeDef


def get_value() -> SecurityDetailsOutputTypeDef:
    return {
        "roleArn": ...,
    }


# SecurityDetailsOutputTypeDef definition

class SecurityDetailsOutputTypeDef(TypedDict):
    roleArn: str,
    securityGroupIds: List[str],
    subnetIds: List[str],
```

## S3ObjectTypeDef

```python
# S3ObjectTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import S3ObjectTypeDef


def get_value() -> S3ObjectTypeDef:
    return {
        "bucket": ...,
    }


# S3ObjectTypeDef definition

class S3ObjectTypeDef(TypedDict):
    bucket: NotRequired[str],
    key: NotRequired[str],
    version: NotRequired[str],
```

## EphemerisMetaDataTypeDef

```python
# EphemerisMetaDataTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import EphemerisMetaDataTypeDef


def get_value() -> EphemerisMetaDataTypeDef:
    return {
        "ephemerisId": ...,
    }


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
# FrequencyBandwidthTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import FrequencyBandwidthTypeDef


def get_value() -> FrequencyBandwidthTypeDef:
    return {
        "units": ...,
    }


# FrequencyBandwidthTypeDef definition

class FrequencyBandwidthTypeDef(TypedDict):
    units: BandwidthUnitsType,  # (1)
    value: float,
```

1. See [:material-code-brackets: BandwidthUnitsType](./literals.md#bandwidthunitstype) 
## FrequencyTypeDef

```python
# FrequencyTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import FrequencyTypeDef


def get_value() -> FrequencyTypeDef:
    return {
        "units": ...,
    }


# FrequencyTypeDef definition

class FrequencyTypeDef(TypedDict):
    units: FrequencyUnitsType,  # (1)
    value: float,
```

1. See [:material-code-brackets: FrequencyUnitsType](./literals.md#frequencyunitstype) 
## GetAgentConfigurationRequestTypeDef

```python
# GetAgentConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import GetAgentConfigurationRequestTypeDef


def get_value() -> GetAgentConfigurationRequestTypeDef:
    return {
        "agentId": ...,
    }


# GetAgentConfigurationRequestTypeDef definition

class GetAgentConfigurationRequestTypeDef(TypedDict):
    agentId: str,
```

## GetConfigRequestTypeDef

```python
# GetConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import GetConfigRequestTypeDef


def get_value() -> GetConfigRequestTypeDef:
    return {
        "configId": ...,
    }


# GetConfigRequestTypeDef definition

class GetConfigRequestTypeDef(TypedDict):
    configId: str,
    configType: ConfigCapabilityTypeType,  # (1)
```

1. See [:material-code-brackets: ConfigCapabilityTypeType](./literals.md#configcapabilitytypetype) 
## GetDataflowEndpointGroupRequestTypeDef

```python
# GetDataflowEndpointGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import GetDataflowEndpointGroupRequestTypeDef


def get_value() -> GetDataflowEndpointGroupRequestTypeDef:
    return {
        "dataflowEndpointGroupId": ...,
    }


# GetDataflowEndpointGroupRequestTypeDef definition

class GetDataflowEndpointGroupRequestTypeDef(TypedDict):
    dataflowEndpointGroupId: str,
```

## GetMinuteUsageRequestTypeDef

```python
# GetMinuteUsageRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import GetMinuteUsageRequestTypeDef


def get_value() -> GetMinuteUsageRequestTypeDef:
    return {
        "month": ...,
    }


# GetMinuteUsageRequestTypeDef definition

class GetMinuteUsageRequestTypeDef(TypedDict):
    month: int,
    year: int,
```

## GetMissionProfileRequestTypeDef

```python
# GetMissionProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import GetMissionProfileRequestTypeDef


def get_value() -> GetMissionProfileRequestTypeDef:
    return {
        "missionProfileId": ...,
    }


# GetMissionProfileRequestTypeDef definition

class GetMissionProfileRequestTypeDef(TypedDict):
    missionProfileId: str,
```

## GetSatelliteRequestTypeDef

```python
# GetSatelliteRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import GetSatelliteRequestTypeDef


def get_value() -> GetSatelliteRequestTypeDef:
    return {
        "satelliteId": ...,
    }


# GetSatelliteRequestTypeDef definition

class GetSatelliteRequestTypeDef(TypedDict):
    satelliteId: str,
```

## GroundStationDataTypeDef

```python
# GroundStationDataTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import GroundStationDataTypeDef


def get_value() -> GroundStationDataTypeDef:
    return {
        "groundStationId": ...,
    }


# GroundStationDataTypeDef definition

class GroundStationDataTypeDef(TypedDict):
    groundStationId: NotRequired[str],
    groundStationName: NotRequired[str],
    region: NotRequired[str],
```

## IntegerRangeTypeDef

```python
# IntegerRangeTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import IntegerRangeTypeDef


def get_value() -> IntegerRangeTypeDef:
    return {
        "maximum": ...,
    }


# IntegerRangeTypeDef definition

class IntegerRangeTypeDef(TypedDict):
    maximum: int,
    minimum: int,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListConfigsRequestTypeDef

```python
# ListConfigsRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListConfigsRequestTypeDef


def get_value() -> ListConfigsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListConfigsRequestTypeDef definition

class ListConfigsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListDataflowEndpointGroupsRequestTypeDef

```python
# ListDataflowEndpointGroupsRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListDataflowEndpointGroupsRequestTypeDef


def get_value() -> ListDataflowEndpointGroupsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListDataflowEndpointGroupsRequestTypeDef definition

class ListDataflowEndpointGroupsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListGroundStationsRequestTypeDef

```python
# ListGroundStationsRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListGroundStationsRequestTypeDef


def get_value() -> ListGroundStationsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListGroundStationsRequestTypeDef definition

class ListGroundStationsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    satelliteId: NotRequired[str],
```

## ListMissionProfilesRequestTypeDef

```python
# ListMissionProfilesRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListMissionProfilesRequestTypeDef


def get_value() -> ListMissionProfilesRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListMissionProfilesRequestTypeDef definition

class ListMissionProfilesRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## MissionProfileListItemTypeDef

```python
# MissionProfileListItemTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import MissionProfileListItemTypeDef


def get_value() -> MissionProfileListItemTypeDef:
    return {
        "missionProfileArn": ...,
    }


# MissionProfileListItemTypeDef definition

class MissionProfileListItemTypeDef(TypedDict):
    missionProfileArn: NotRequired[str],
    missionProfileId: NotRequired[str],
    name: NotRequired[str],
    region: NotRequired[str],
```

## ListSatellitesRequestTypeDef

```python
# ListSatellitesRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListSatellitesRequestTypeDef


def get_value() -> ListSatellitesRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListSatellitesRequestTypeDef definition

class ListSatellitesRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## SecurityDetailsTypeDef

```python
# SecurityDetailsTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import SecurityDetailsTypeDef


def get_value() -> SecurityDetailsTypeDef:
    return {
        "roleArn": ...,
    }


# SecurityDetailsTypeDef definition

class SecurityDetailsTypeDef(TypedDict):
    roleArn: str,
    securityGroupIds: Sequence[str],
    subnetIds: Sequence[str],
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateEphemerisRequestTypeDef

```python
# UpdateEphemerisRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import UpdateEphemerisRequestTypeDef


def get_value() -> UpdateEphemerisRequestTypeDef:
    return {
        "enabled": ...,
    }


# UpdateEphemerisRequestTypeDef definition

class UpdateEphemerisRequestTypeDef(TypedDict):
    enabled: bool,
    ephemerisId: str,
    name: NotRequired[str],
    priority: NotRequired[int],
```

## AgentDetailsTypeDef

```python
# AgentDetailsTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import AgentDetailsTypeDef


def get_value() -> AgentDetailsTypeDef:
    return {
        "agentCpuCores": ...,
    }


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
## UpdateAgentStatusRequestTypeDef

```python
# UpdateAgentStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import UpdateAgentStatusRequestTypeDef


def get_value() -> UpdateAgentStatusRequestTypeDef:
    return {
        "agentId": ...,
    }


# UpdateAgentStatusRequestTypeDef definition

class UpdateAgentStatusRequestTypeDef(TypedDict):
    agentId: str,
    aggregateStatus: AggregateStatusTypeDef,  # (1)
    componentStatuses: Sequence[ComponentStatusDataTypeDef],  # (2)
    taskId: str,
```

1. See [:material-code-braces: AggregateStatusTypeDef](./type_defs.md#aggregatestatustypedef) 
2. See [:material-code-braces: ComponentStatusDataTypeDef](./type_defs.md#componentstatusdatatypedef) 
## ConfigIdResponseTypeDef

```python
# ConfigIdResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ConfigIdResponseTypeDef


def get_value() -> ConfigIdResponseTypeDef:
    return {
        "configArn": ...,
    }


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
# ContactIdResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ContactIdResponseTypeDef


def get_value() -> ContactIdResponseTypeDef:
    return {
        "contactId": ...,
    }


# ContactIdResponseTypeDef definition

class ContactIdResponseTypeDef(TypedDict):
    contactId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataflowEndpointGroupIdResponseTypeDef

```python
# DataflowEndpointGroupIdResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import DataflowEndpointGroupIdResponseTypeDef


def get_value() -> DataflowEndpointGroupIdResponseTypeDef:
    return {
        "dataflowEndpointGroupId": ...,
    }


# DataflowEndpointGroupIdResponseTypeDef definition

class DataflowEndpointGroupIdResponseTypeDef(TypedDict):
    dataflowEndpointGroupId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EphemerisIdResponseTypeDef

```python
# EphemerisIdResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import EphemerisIdResponseTypeDef


def get_value() -> EphemerisIdResponseTypeDef:
    return {
        "ephemerisId": ...,
    }


# EphemerisIdResponseTypeDef definition

class EphemerisIdResponseTypeDef(TypedDict):
    ephemerisId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAgentConfigurationResponseTypeDef

```python
# GetAgentConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import GetAgentConfigurationResponseTypeDef


def get_value() -> GetAgentConfigurationResponseTypeDef:
    return {
        "agentId": ...,
    }


# GetAgentConfigurationResponseTypeDef definition

class GetAgentConfigurationResponseTypeDef(TypedDict):
    agentId: str,
    taskingDocument: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMinuteUsageResponseTypeDef

```python
# GetMinuteUsageResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import GetMinuteUsageResponseTypeDef


def get_value() -> GetMinuteUsageResponseTypeDef:
    return {
        "estimatedMinutesRemaining": ...,
    }


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
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MissionProfileIdResponseTypeDef

```python
# MissionProfileIdResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import MissionProfileIdResponseTypeDef


def get_value() -> MissionProfileIdResponseTypeDef:
    return {
        "missionProfileId": ...,
    }


# MissionProfileIdResponseTypeDef definition

class MissionProfileIdResponseTypeDef(TypedDict):
    missionProfileId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterAgentResponseTypeDef

```python
# RegisterAgentResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import RegisterAgentResponseTypeDef


def get_value() -> RegisterAgentResponseTypeDef:
    return {
        "agentId": ...,
    }


# RegisterAgentResponseTypeDef definition

class RegisterAgentResponseTypeDef(TypedDict):
    agentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAgentStatusResponseTypeDef

```python
# UpdateAgentStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import UpdateAgentStatusResponseTypeDef


def get_value() -> UpdateAgentStatusResponseTypeDef:
    return {
        "agentId": ...,
    }


# UpdateAgentStatusResponseTypeDef definition

class UpdateAgentStatusResponseTypeDef(TypedDict):
    agentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfigsResponseTypeDef

```python
# ListConfigsResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListConfigsResponseTypeDef


def get_value() -> ListConfigsResponseTypeDef:
    return {
        "configList": ...,
    }


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
# ConnectionDetailsTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ConnectionDetailsTypeDef


def get_value() -> ConnectionDetailsTypeDef:
    return {
        "mtu": ...,
    }


# ConnectionDetailsTypeDef definition

class ConnectionDetailsTypeDef(TypedDict):
    socketAddress: SocketAddressTypeDef,  # (1)
    mtu: NotRequired[int],
```

1. See [:material-code-braces: SocketAddressTypeDef](./type_defs.md#socketaddresstypedef) 
## DataflowEndpointTypeDef

```python
# DataflowEndpointTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import DataflowEndpointTypeDef


def get_value() -> DataflowEndpointTypeDef:
    return {
        "address": ...,
    }


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
# ContactDataTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ContactDataTypeDef


def get_value() -> ContactDataTypeDef:
    return {
        "contactId": ...,
    }


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
## ListContactsRequestTypeDef

```python
# ListContactsRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListContactsRequestTypeDef


def get_value() -> ListContactsRequestTypeDef:
    return {
        "endTime": ...,
    }


# ListContactsRequestTypeDef definition

class ListContactsRequestTypeDef(TypedDict):
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
## ListEphemeridesRequestTypeDef

```python
# ListEphemeridesRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListEphemeridesRequestTypeDef


def get_value() -> ListEphemeridesRequestTypeDef:
    return {
        "endTime": ...,
    }


# ListEphemeridesRequestTypeDef definition

class ListEphemeridesRequestTypeDef(TypedDict):
    endTime: TimestampTypeDef,
    satelliteId: str,
    startTime: TimestampTypeDef,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    statusList: NotRequired[Sequence[EphemerisStatusType]],  # (1)
```

1. See [:material-code-brackets: EphemerisStatusType](./literals.md#ephemerisstatustype) 
## ReserveContactRequestTypeDef

```python
# ReserveContactRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ReserveContactRequestTypeDef


def get_value() -> ReserveContactRequestTypeDef:
    return {
        "endTime": ...,
    }


# ReserveContactRequestTypeDef definition

class ReserveContactRequestTypeDef(TypedDict):
    endTime: TimestampTypeDef,
    groundStation: str,
    missionProfileArn: str,
    satelliteArn: str,
    startTime: TimestampTypeDef,
    tags: NotRequired[Mapping[str, str]],
```

## TimeRangeTypeDef

```python
# TimeRangeTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import TimeRangeTypeDef


def get_value() -> TimeRangeTypeDef:
    return {
        "endTime": ...,
    }


# TimeRangeTypeDef definition

class TimeRangeTypeDef(TypedDict):
    endTime: TimestampTypeDef,
    startTime: TimestampTypeDef,
```

## CreateMissionProfileRequestTypeDef

```python
# CreateMissionProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import CreateMissionProfileRequestTypeDef


def get_value() -> CreateMissionProfileRequestTypeDef:
    return {
        "dataflowEdges": ...,
    }


# CreateMissionProfileRequestTypeDef definition

class CreateMissionProfileRequestTypeDef(TypedDict):
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
# GetMissionProfileResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import GetMissionProfileResponseTypeDef


def get_value() -> GetMissionProfileResponseTypeDef:
    return {
        "contactPostPassDurationSeconds": ...,
    }


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
## UpdateMissionProfileRequestTypeDef

```python
# UpdateMissionProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import UpdateMissionProfileRequestTypeDef


def get_value() -> UpdateMissionProfileRequestTypeDef:
    return {
        "missionProfileId": ...,
    }


# UpdateMissionProfileRequestTypeDef definition

class UpdateMissionProfileRequestTypeDef(TypedDict):
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
# ListDataflowEndpointGroupsResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListDataflowEndpointGroupsResponseTypeDef


def get_value() -> ListDataflowEndpointGroupsResponseTypeDef:
    return {
        "dataflowEndpointGroupList": ...,
    }


# ListDataflowEndpointGroupsResponseTypeDef definition

class ListDataflowEndpointGroupsResponseTypeDef(TypedDict):
    dataflowEndpointGroupList: List[DataflowEndpointListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DataflowEndpointListItemTypeDef](./type_defs.md#dataflowendpointlistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeContactRequestWaitTypeDef

```python
# DescribeContactRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import DescribeContactRequestWaitTypeDef


def get_value() -> DescribeContactRequestWaitTypeDef:
    return {
        "contactId": ...,
    }


# DescribeContactRequestWaitTypeDef definition

class DescribeContactRequestWaitTypeDef(TypedDict):
    contactId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## EphemerisDescriptionTypeDef

```python
# EphemerisDescriptionTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import EphemerisDescriptionTypeDef


def get_value() -> EphemerisDescriptionTypeDef:
    return {
        "ephemerisData": ...,
    }


# EphemerisDescriptionTypeDef definition

class EphemerisDescriptionTypeDef(TypedDict):
    ephemerisData: NotRequired[str],
    sourceS3Object: NotRequired[S3ObjectTypeDef],  # (1)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
## EphemerisItemTypeDef

```python
# EphemerisItemTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import EphemerisItemTypeDef


def get_value() -> EphemerisItemTypeDef:
    return {
        "creationTime": ...,
    }


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
# OEMEphemerisTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import OEMEphemerisTypeDef


def get_value() -> OEMEphemerisTypeDef:
    return {
        "oemData": ...,
    }


# OEMEphemerisTypeDef definition

class OEMEphemerisTypeDef(TypedDict):
    oemData: NotRequired[str],
    s3Object: NotRequired[S3ObjectTypeDef],  # (1)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
## GetSatelliteResponseTypeDef

```python
# GetSatelliteResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import GetSatelliteResponseTypeDef


def get_value() -> GetSatelliteResponseTypeDef:
    return {
        "currentEphemeris": ...,
    }


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
# SatelliteListItemTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import SatelliteListItemTypeDef


def get_value() -> SatelliteListItemTypeDef:
    return {
        "currentEphemeris": ...,
    }


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
# SpectrumConfigTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import SpectrumConfigTypeDef


def get_value() -> SpectrumConfigTypeDef:
    return {
        "bandwidth": ...,
    }


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
# UplinkSpectrumConfigTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import UplinkSpectrumConfigTypeDef


def get_value() -> UplinkSpectrumConfigTypeDef:
    return {
        "centerFrequency": ...,
    }


# UplinkSpectrumConfigTypeDef definition

class UplinkSpectrumConfigTypeDef(TypedDict):
    centerFrequency: FrequencyTypeDef,  # (1)
    polarization: NotRequired[PolarizationType],  # (2)
```

1. See [:material-code-braces: FrequencyTypeDef](./type_defs.md#frequencytypedef) 
2. See [:material-code-brackets: PolarizationType](./literals.md#polarizationtype) 
## ListGroundStationsResponseTypeDef

```python
# ListGroundStationsResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListGroundStationsResponseTypeDef


def get_value() -> ListGroundStationsResponseTypeDef:
    return {
        "groundStationList": ...,
    }


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
# RangedSocketAddressTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import RangedSocketAddressTypeDef


def get_value() -> RangedSocketAddressTypeDef:
    return {
        "name": ...,
    }


# RangedSocketAddressTypeDef definition

class RangedSocketAddressTypeDef(TypedDict):
    name: str,
    portRange: IntegerRangeTypeDef,  # (1)
```

1. See [:material-code-braces: IntegerRangeTypeDef](./type_defs.md#integerrangetypedef) 
## ListConfigsRequestPaginateTypeDef

```python
# ListConfigsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListConfigsRequestPaginateTypeDef


def get_value() -> ListConfigsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListConfigsRequestPaginateTypeDef definition

class ListConfigsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListContactsRequestPaginateTypeDef

```python
# ListContactsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListContactsRequestPaginateTypeDef


def get_value() -> ListContactsRequestPaginateTypeDef:
    return {
        "endTime": ...,
    }


# ListContactsRequestPaginateTypeDef definition

class ListContactsRequestPaginateTypeDef(TypedDict):
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
## ListDataflowEndpointGroupsRequestPaginateTypeDef

```python
# ListDataflowEndpointGroupsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListDataflowEndpointGroupsRequestPaginateTypeDef


def get_value() -> ListDataflowEndpointGroupsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListDataflowEndpointGroupsRequestPaginateTypeDef definition

class ListDataflowEndpointGroupsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEphemeridesRequestPaginateTypeDef

```python
# ListEphemeridesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListEphemeridesRequestPaginateTypeDef


def get_value() -> ListEphemeridesRequestPaginateTypeDef:
    return {
        "endTime": ...,
    }


# ListEphemeridesRequestPaginateTypeDef definition

class ListEphemeridesRequestPaginateTypeDef(TypedDict):
    endTime: TimestampTypeDef,
    satelliteId: str,
    startTime: TimestampTypeDef,
    statusList: NotRequired[Sequence[EphemerisStatusType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: EphemerisStatusType](./literals.md#ephemerisstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroundStationsRequestPaginateTypeDef

```python
# ListGroundStationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListGroundStationsRequestPaginateTypeDef


def get_value() -> ListGroundStationsRequestPaginateTypeDef:
    return {
        "satelliteId": ...,
    }


# ListGroundStationsRequestPaginateTypeDef definition

class ListGroundStationsRequestPaginateTypeDef(TypedDict):
    satelliteId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMissionProfilesRequestPaginateTypeDef

```python
# ListMissionProfilesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListMissionProfilesRequestPaginateTypeDef


def get_value() -> ListMissionProfilesRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListMissionProfilesRequestPaginateTypeDef definition

class ListMissionProfilesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSatellitesRequestPaginateTypeDef

```python
# ListSatellitesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListSatellitesRequestPaginateTypeDef


def get_value() -> ListSatellitesRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListSatellitesRequestPaginateTypeDef definition

class ListSatellitesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMissionProfilesResponseTypeDef

```python
# ListMissionProfilesResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListMissionProfilesResponseTypeDef


def get_value() -> ListMissionProfilesResponseTypeDef:
    return {
        "missionProfileList": ...,
    }


# ListMissionProfilesResponseTypeDef definition

class ListMissionProfilesResponseTypeDef(TypedDict):
    missionProfileList: List[MissionProfileListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MissionProfileListItemTypeDef](./type_defs.md#missionprofilelistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterAgentRequestTypeDef

```python
# RegisterAgentRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import RegisterAgentRequestTypeDef


def get_value() -> RegisterAgentRequestTypeDef:
    return {
        "agentDetails": ...,
    }


# RegisterAgentRequestTypeDef definition

class RegisterAgentRequestTypeDef(TypedDict):
    agentDetails: AgentDetailsTypeDef,  # (1)
    discoveryData: DiscoveryDataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentDetailsTypeDef](./type_defs.md#agentdetailstypedef) 
2. See [:material-code-braces: DiscoveryDataTypeDef](./type_defs.md#discoverydatatypedef) 
## ListContactsResponseTypeDef

```python
# ListContactsResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListContactsResponseTypeDef


def get_value() -> ListContactsResponseTypeDef:
    return {
        "contactList": ...,
    }


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
# TLEDataTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import TLEDataTypeDef


def get_value() -> TLEDataTypeDef:
    return {
        "tleLine1": ...,
    }


# TLEDataTypeDef definition

class TLEDataTypeDef(TypedDict):
    tleLine1: str,
    tleLine2: str,
    validTimeRange: TimeRangeTypeDef,  # (1)
```

1. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
## EphemerisTypeDescriptionTypeDef

```python
# EphemerisTypeDescriptionTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import EphemerisTypeDescriptionTypeDef


def get_value() -> EphemerisTypeDescriptionTypeDef:
    return {
        "oem": ...,
    }


# EphemerisTypeDescriptionTypeDef definition

class EphemerisTypeDescriptionTypeDef(TypedDict):
    oem: NotRequired[EphemerisDescriptionTypeDef],  # (1)
    tle: NotRequired[EphemerisDescriptionTypeDef],  # (1)
```

1. See [:material-code-braces: EphemerisDescriptionTypeDef](./type_defs.md#ephemerisdescriptiontypedef) 
2. See [:material-code-braces: EphemerisDescriptionTypeDef](./type_defs.md#ephemerisdescriptiontypedef) 
## ListEphemeridesResponseTypeDef

```python
# ListEphemeridesResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListEphemeridesResponseTypeDef


def get_value() -> ListEphemeridesResponseTypeDef:
    return {
        "ephemerides": ...,
    }


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
# ListSatellitesResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ListSatellitesResponseTypeDef


def get_value() -> ListSatellitesResponseTypeDef:
    return {
        "nextToken": ...,
    }


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
# AntennaDownlinkConfigTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import AntennaDownlinkConfigTypeDef


def get_value() -> AntennaDownlinkConfigTypeDef:
    return {
        "spectrumConfig": ...,
    }


# AntennaDownlinkConfigTypeDef definition

class AntennaDownlinkConfigTypeDef(TypedDict):
    spectrumConfig: SpectrumConfigTypeDef,  # (1)
```

1. See [:material-code-braces: SpectrumConfigTypeDef](./type_defs.md#spectrumconfigtypedef) 
## AntennaDownlinkDemodDecodeConfigTypeDef

```python
# AntennaDownlinkDemodDecodeConfigTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import AntennaDownlinkDemodDecodeConfigTypeDef


def get_value() -> AntennaDownlinkDemodDecodeConfigTypeDef:
    return {
        "decodeConfig": ...,
    }


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
# AntennaUplinkConfigTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import AntennaUplinkConfigTypeDef


def get_value() -> AntennaUplinkConfigTypeDef:
    return {
        "spectrumConfig": ...,
    }


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
# RangedConnectionDetailsTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import RangedConnectionDetailsTypeDef


def get_value() -> RangedConnectionDetailsTypeDef:
    return {
        "mtu": ...,
    }


# RangedConnectionDetailsTypeDef definition

class RangedConnectionDetailsTypeDef(TypedDict):
    socketAddress: RangedSocketAddressTypeDef,  # (1)
    mtu: NotRequired[int],
```

1. See [:material-code-braces: RangedSocketAddressTypeDef](./type_defs.md#rangedsocketaddresstypedef) 
## TLEEphemerisTypeDef

```python
# TLEEphemerisTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import TLEEphemerisTypeDef


def get_value() -> TLEEphemerisTypeDef:
    return {
        "s3Object": ...,
    }


# TLEEphemerisTypeDef definition

class TLEEphemerisTypeDef(TypedDict):
    s3Object: NotRequired[S3ObjectTypeDef],  # (1)
    tleData: NotRequired[Sequence[TLEDataTypeDef]],  # (2)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
2. See [:material-code-braces: TLEDataTypeDef](./type_defs.md#tledatatypedef) 
## DescribeEphemerisResponseTypeDef

```python
# DescribeEphemerisResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import DescribeEphemerisResponseTypeDef


def get_value() -> DescribeEphemerisResponseTypeDef:
    return {
        "creationTime": ...,
    }


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
# ConfigTypeDataTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ConfigTypeDataTypeDef


def get_value() -> ConfigTypeDataTypeDef:
    return {
        "antennaDownlinkConfig": ...,
    }


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
# AwsGroundStationAgentEndpointTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import AwsGroundStationAgentEndpointTypeDef


def get_value() -> AwsGroundStationAgentEndpointTypeDef:
    return {
        "agentStatus": ...,
    }


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
# EphemerisDataTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import EphemerisDataTypeDef


def get_value() -> EphemerisDataTypeDef:
    return {
        "oem": ...,
    }


# EphemerisDataTypeDef definition

class EphemerisDataTypeDef(TypedDict):
    oem: NotRequired[OEMEphemerisTypeDef],  # (1)
    tle: NotRequired[TLEEphemerisTypeDef],  # (2)
```

1. See [:material-code-braces: OEMEphemerisTypeDef](./type_defs.md#oemephemeristypedef) 
2. See [:material-code-braces: TLEEphemerisTypeDef](./type_defs.md#tleephemeristypedef) 
## CreateConfigRequestTypeDef

```python
# CreateConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import CreateConfigRequestTypeDef


def get_value() -> CreateConfigRequestTypeDef:
    return {
        "configData": ...,
    }


# CreateConfigRequestTypeDef definition

class CreateConfigRequestTypeDef(TypedDict):
    configData: ConfigTypeDataTypeDef,  # (1)
    name: str,
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ConfigTypeDataTypeDef](./type_defs.md#configtypedatatypedef) 
## GetConfigResponseTypeDef

```python
# GetConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import GetConfigResponseTypeDef


def get_value() -> GetConfigResponseTypeDef:
    return {
        "configArn": ...,
    }


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
## UpdateConfigRequestTypeDef

```python
# UpdateConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import UpdateConfigRequestTypeDef


def get_value() -> UpdateConfigRequestTypeDef:
    return {
        "configData": ...,
    }


# UpdateConfigRequestTypeDef definition

class UpdateConfigRequestTypeDef(TypedDict):
    configData: ConfigTypeDataTypeDef,  # (1)
    configId: str,
    configType: ConfigCapabilityTypeType,  # (2)
    name: str,
```

1. See [:material-code-braces: ConfigTypeDataTypeDef](./type_defs.md#configtypedatatypedef) 
2. See [:material-code-brackets: ConfigCapabilityTypeType](./literals.md#configcapabilitytypetype) 
## EndpointDetailsOutputTypeDef

```python
# EndpointDetailsOutputTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import EndpointDetailsOutputTypeDef


def get_value() -> EndpointDetailsOutputTypeDef:
    return {
        "awsGroundStationAgentEndpoint": ...,
    }


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
# EndpointDetailsTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import EndpointDetailsTypeDef


def get_value() -> EndpointDetailsTypeDef:
    return {
        "awsGroundStationAgentEndpoint": ...,
    }


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
## CreateEphemerisRequestTypeDef

```python
# CreateEphemerisRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import CreateEphemerisRequestTypeDef


def get_value() -> CreateEphemerisRequestTypeDef:
    return {
        "name": ...,
    }


# CreateEphemerisRequestTypeDef definition

class CreateEphemerisRequestTypeDef(TypedDict):
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
# ConfigDetailsTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import ConfigDetailsTypeDef


def get_value() -> ConfigDetailsTypeDef:
    return {
        "antennaDemodDecodeDetails": ...,
    }


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
# GetDataflowEndpointGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import GetDataflowEndpointGroupResponseTypeDef


def get_value() -> GetDataflowEndpointGroupResponseTypeDef:
    return {
        "contactPostPassDurationSeconds": ...,
    }


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
# DestinationTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import DestinationTypeDef


def get_value() -> DestinationTypeDef:
    return {
        "configDetails": ...,
    }


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
# SourceTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import SourceTypeDef


def get_value() -> SourceTypeDef:
    return {
        "configDetails": ...,
    }


# SourceTypeDef definition

class SourceTypeDef(TypedDict):
    configDetails: NotRequired[ConfigDetailsTypeDef],  # (1)
    configId: NotRequired[str],
    configType: NotRequired[ConfigCapabilityTypeType],  # (2)
    dataflowSourceRegion: NotRequired[str],
```

1. See [:material-code-braces: ConfigDetailsTypeDef](./type_defs.md#configdetailstypedef) 
2. See [:material-code-brackets: ConfigCapabilityTypeType](./literals.md#configcapabilitytypetype) 
## CreateDataflowEndpointGroupRequestTypeDef

```python
# CreateDataflowEndpointGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import CreateDataflowEndpointGroupRequestTypeDef


def get_value() -> CreateDataflowEndpointGroupRequestTypeDef:
    return {
        "endpointDetails": ...,
    }


# CreateDataflowEndpointGroupRequestTypeDef definition

class CreateDataflowEndpointGroupRequestTypeDef(TypedDict):
    endpointDetails: Sequence[EndpointDetailsUnionTypeDef],  # (1)
    contactPostPassDurationSeconds: NotRequired[int],
    contactPrePassDurationSeconds: NotRequired[int],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: EndpointDetailsTypeDef](./type_defs.md#endpointdetailstypedef) [:material-code-braces: EndpointDetailsOutputTypeDef](./type_defs.md#endpointdetailsoutputtypedef) 
## DataflowDetailTypeDef

```python
# DataflowDetailTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import DataflowDetailTypeDef


def get_value() -> DataflowDetailTypeDef:
    return {
        "destination": ...,
    }


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
# DescribeContactResponseTypeDef TypedDict usage example

from types_aiobotocore_groundstation.type_defs import DescribeContactResponseTypeDef


def get_value() -> DescribeContactResponseTypeDef:
    return {
        "contactId": ...,
    }


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
