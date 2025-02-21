# Type definitions

> [Index](../README.md) > [MediaConnect](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MediaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#mediaconnect)
    type annotations stubs module [types-aiobotocore-mediaconnect](https://pypi.org/project/types-aiobotocore-mediaconnect/).

## MonitoringConfigUnionTypeDef

```python
# MonitoringConfigUnionTypeDef Union usage example

from types_aiobotocore_mediaconnect.type_defs import MonitoringConfigUnionTypeDef


def get_value() -> MonitoringConfigUnionTypeDef:
    return ...


# MonitoringConfigUnionTypeDef definition

MonitoringConfigUnionTypeDef = Union[
    MonitoringConfigTypeDef,  # (1)
    MonitoringConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MonitoringConfigTypeDef](./type_defs.md#monitoringconfigtypedef) 
2. See [:material-code-braces: MonitoringConfigOutputTypeDef](./type_defs.md#monitoringconfigoutputtypedef) 



## VpcInterfaceAttachmentTypeDef

```python
# VpcInterfaceAttachmentTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import VpcInterfaceAttachmentTypeDef


def get_value() -> VpcInterfaceAttachmentTypeDef:
    return {
        "VpcInterfaceName": ...,
    }


# VpcInterfaceAttachmentTypeDef definition

class VpcInterfaceAttachmentTypeDef(TypedDict):
    VpcInterfaceName: NotRequired[str],
```

## AddBridgeNetworkOutputRequestTypeDef

```python
# AddBridgeNetworkOutputRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AddBridgeNetworkOutputRequestTypeDef


def get_value() -> AddBridgeNetworkOutputRequestTypeDef:
    return {
        "IpAddress": ...,
    }


# AddBridgeNetworkOutputRequestTypeDef definition

class AddBridgeNetworkOutputRequestTypeDef(TypedDict):
    IpAddress: str,
    Name: str,
    NetworkName: str,
    Port: int,
    Protocol: ProtocolType,  # (1)
    Ttl: int,
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
## MulticastSourceSettingsTypeDef

```python
# MulticastSourceSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import MulticastSourceSettingsTypeDef


def get_value() -> MulticastSourceSettingsTypeDef:
    return {
        "MulticastSourceIp": ...,
    }


# MulticastSourceSettingsTypeDef definition

class MulticastSourceSettingsTypeDef(TypedDict):
    MulticastSourceIp: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ResponseMetadataTypeDef


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

## AddEgressGatewayBridgeRequestTypeDef

```python
# AddEgressGatewayBridgeRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AddEgressGatewayBridgeRequestTypeDef


def get_value() -> AddEgressGatewayBridgeRequestTypeDef:
    return {
        "MaxBitrate": ...,
    }


# AddEgressGatewayBridgeRequestTypeDef definition

class AddEgressGatewayBridgeRequestTypeDef(TypedDict):
    MaxBitrate: int,
```

## VpcInterfaceRequestTypeDef

```python
# VpcInterfaceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import VpcInterfaceRequestTypeDef


def get_value() -> VpcInterfaceRequestTypeDef:
    return {
        "Name": ...,
    }


# VpcInterfaceRequestTypeDef definition

class VpcInterfaceRequestTypeDef(TypedDict):
    Name: str,
    RoleArn: str,
    SecurityGroupIds: Sequence[str],
    SubnetId: str,
    NetworkInterfaceType: NotRequired[NetworkInterfaceTypeType],  # (1)
```

1. See [:material-code-brackets: NetworkInterfaceTypeType](./literals.md#networkinterfacetypetype) 
## VpcInterfaceTypeDef

```python
# VpcInterfaceTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import VpcInterfaceTypeDef


def get_value() -> VpcInterfaceTypeDef:
    return {
        "Name": ...,
    }


# VpcInterfaceTypeDef definition

class VpcInterfaceTypeDef(TypedDict):
    Name: str,
    NetworkInterfaceIds: List[str],
    NetworkInterfaceType: NetworkInterfaceTypeType,  # (1)
    RoleArn: str,
    SecurityGroupIds: List[str],
    SubnetId: str,
```

1. See [:material-code-brackets: NetworkInterfaceTypeType](./literals.md#networkinterfacetypetype) 
## AddIngressGatewayBridgeRequestTypeDef

```python
# AddIngressGatewayBridgeRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AddIngressGatewayBridgeRequestTypeDef


def get_value() -> AddIngressGatewayBridgeRequestTypeDef:
    return {
        "MaxBitrate": ...,
    }


# AddIngressGatewayBridgeRequestTypeDef definition

class AddIngressGatewayBridgeRequestTypeDef(TypedDict):
    MaxBitrate: int,
    MaxOutputs: int,
```

## AddMaintenanceTypeDef

```python
# AddMaintenanceTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AddMaintenanceTypeDef


def get_value() -> AddMaintenanceTypeDef:
    return {
        "MaintenanceDay": ...,
    }


# AddMaintenanceTypeDef definition

class AddMaintenanceTypeDef(TypedDict):
    MaintenanceDay: MaintenanceDayType,  # (1)
    MaintenanceStartHour: str,
```

1. See [:material-code-brackets: MaintenanceDayType](./literals.md#maintenancedaytype) 
## EncryptionTypeDef

```python
# EncryptionTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import EncryptionTypeDef


def get_value() -> EncryptionTypeDef:
    return {
        "Algorithm": ...,
    }


# EncryptionTypeDef definition

class EncryptionTypeDef(TypedDict):
    RoleArn: str,
    Algorithm: NotRequired[AlgorithmType],  # (1)
    ConstantInitializationVector: NotRequired[str],
    DeviceId: NotRequired[str],
    KeyType: NotRequired[KeyTypeType],  # (2)
    Region: NotRequired[str],
    ResourceId: NotRequired[str],
    SecretArn: NotRequired[str],
    Url: NotRequired[str],
```

1. See [:material-code-brackets: AlgorithmType](./literals.md#algorithmtype) 
2. See [:material-code-brackets: KeyTypeType](./literals.md#keytypetype) 
## SilentAudioTypeDef

```python
# SilentAudioTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import SilentAudioTypeDef


def get_value() -> SilentAudioTypeDef:
    return {
        "State": ...,
    }


# SilentAudioTypeDef definition

class SilentAudioTypeDef(TypedDict):
    State: NotRequired[StateType],  # (1)
    ThresholdSeconds: NotRequired[int],
```

1. See [:material-code-brackets: StateType](./literals.md#statetype) 
## BlackFramesTypeDef

```python
# BlackFramesTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import BlackFramesTypeDef


def get_value() -> BlackFramesTypeDef:
    return {
        "State": ...,
    }


# BlackFramesTypeDef definition

class BlackFramesTypeDef(TypedDict):
    State: NotRequired[StateType],  # (1)
    ThresholdSeconds: NotRequired[int],
```

1. See [:material-code-brackets: StateType](./literals.md#statetype) 
## BridgeFlowOutputTypeDef

```python
# BridgeFlowOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import BridgeFlowOutputTypeDef


def get_value() -> BridgeFlowOutputTypeDef:
    return {
        "FlowArn": ...,
    }


# BridgeFlowOutputTypeDef definition

class BridgeFlowOutputTypeDef(TypedDict):
    FlowArn: str,
    FlowSourceArn: str,
    Name: str,
```

## BridgeNetworkOutputTypeDef

```python
# BridgeNetworkOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import BridgeNetworkOutputTypeDef


def get_value() -> BridgeNetworkOutputTypeDef:
    return {
        "IpAddress": ...,
    }


# BridgeNetworkOutputTypeDef definition

class BridgeNetworkOutputTypeDef(TypedDict):
    IpAddress: str,
    Name: str,
    NetworkName: str,
    Port: int,
    Protocol: ProtocolType,  # (1)
    Ttl: int,
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
## EgressGatewayBridgeTypeDef

```python
# EgressGatewayBridgeTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import EgressGatewayBridgeTypeDef


def get_value() -> EgressGatewayBridgeTypeDef:
    return {
        "InstanceId": ...,
    }


# EgressGatewayBridgeTypeDef definition

class EgressGatewayBridgeTypeDef(TypedDict):
    MaxBitrate: int,
    InstanceId: NotRequired[str],
```

## IngressGatewayBridgeTypeDef

```python
# IngressGatewayBridgeTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import IngressGatewayBridgeTypeDef


def get_value() -> IngressGatewayBridgeTypeDef:
    return {
        "InstanceId": ...,
    }


# IngressGatewayBridgeTypeDef definition

class IngressGatewayBridgeTypeDef(TypedDict):
    MaxBitrate: int,
    MaxOutputs: int,
    InstanceId: NotRequired[str],
```

## MessageDetailTypeDef

```python
# MessageDetailTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import MessageDetailTypeDef


def get_value() -> MessageDetailTypeDef:
    return {
        "Code": ...,
    }


# MessageDetailTypeDef definition

class MessageDetailTypeDef(TypedDict):
    Code: str,
    Message: str,
    ResourceName: NotRequired[str],
```

## GatewayNetworkTypeDef

```python
# GatewayNetworkTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import GatewayNetworkTypeDef


def get_value() -> GatewayNetworkTypeDef:
    return {
        "CidrBlock": ...,
    }


# GatewayNetworkTypeDef definition

class GatewayNetworkTypeDef(TypedDict):
    CidrBlock: str,
    Name: str,
```

## DeleteBridgeRequestTypeDef

```python
# DeleteBridgeRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DeleteBridgeRequestTypeDef


def get_value() -> DeleteBridgeRequestTypeDef:
    return {
        "BridgeArn": ...,
    }


# DeleteBridgeRequestTypeDef definition

class DeleteBridgeRequestTypeDef(TypedDict):
    BridgeArn: str,
```

## DeleteFlowRequestTypeDef

```python
# DeleteFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DeleteFlowRequestTypeDef


def get_value() -> DeleteFlowRequestTypeDef:
    return {
        "FlowArn": ...,
    }


# DeleteFlowRequestTypeDef definition

class DeleteFlowRequestTypeDef(TypedDict):
    FlowArn: str,
```

## DeleteGatewayRequestTypeDef

```python
# DeleteGatewayRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DeleteGatewayRequestTypeDef


def get_value() -> DeleteGatewayRequestTypeDef:
    return {
        "GatewayArn": ...,
    }


# DeleteGatewayRequestTypeDef definition

class DeleteGatewayRequestTypeDef(TypedDict):
    GatewayArn: str,
```

## DeregisterGatewayInstanceRequestTypeDef

```python
# DeregisterGatewayInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DeregisterGatewayInstanceRequestTypeDef


def get_value() -> DeregisterGatewayInstanceRequestTypeDef:
    return {
        "GatewayInstanceArn": ...,
    }


# DeregisterGatewayInstanceRequestTypeDef definition

class DeregisterGatewayInstanceRequestTypeDef(TypedDict):
    GatewayInstanceArn: str,
    Force: NotRequired[bool],
```

## DescribeBridgeRequestTypeDef

```python
# DescribeBridgeRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DescribeBridgeRequestTypeDef


def get_value() -> DescribeBridgeRequestTypeDef:
    return {
        "BridgeArn": ...,
    }


# DescribeBridgeRequestTypeDef definition

class DescribeBridgeRequestTypeDef(TypedDict):
    BridgeArn: str,
```

## DescribeFlowRequestTypeDef

```python
# DescribeFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DescribeFlowRequestTypeDef


def get_value() -> DescribeFlowRequestTypeDef:
    return {
        "FlowArn": ...,
    }


# DescribeFlowRequestTypeDef definition

class DescribeFlowRequestTypeDef(TypedDict):
    FlowArn: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import WaiterConfigTypeDef


def get_value() -> WaiterConfigTypeDef:
    return {
        "Delay": ...,
    }


# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## MessagesTypeDef

```python
# MessagesTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import MessagesTypeDef


def get_value() -> MessagesTypeDef:
    return {
        "Errors": ...,
    }


# MessagesTypeDef definition

class MessagesTypeDef(TypedDict):
    Errors: List[str],
```

## DescribeFlowSourceMetadataRequestTypeDef

```python
# DescribeFlowSourceMetadataRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DescribeFlowSourceMetadataRequestTypeDef


def get_value() -> DescribeFlowSourceMetadataRequestTypeDef:
    return {
        "FlowArn": ...,
    }


# DescribeFlowSourceMetadataRequestTypeDef definition

class DescribeFlowSourceMetadataRequestTypeDef(TypedDict):
    FlowArn: str,
```

## DescribeFlowSourceThumbnailRequestTypeDef

```python
# DescribeFlowSourceThumbnailRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DescribeFlowSourceThumbnailRequestTypeDef


def get_value() -> DescribeFlowSourceThumbnailRequestTypeDef:
    return {
        "FlowArn": ...,
    }


# DescribeFlowSourceThumbnailRequestTypeDef definition

class DescribeFlowSourceThumbnailRequestTypeDef(TypedDict):
    FlowArn: str,
```

## DescribeGatewayInstanceRequestTypeDef

```python
# DescribeGatewayInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DescribeGatewayInstanceRequestTypeDef


def get_value() -> DescribeGatewayInstanceRequestTypeDef:
    return {
        "GatewayInstanceArn": ...,
    }


# DescribeGatewayInstanceRequestTypeDef definition

class DescribeGatewayInstanceRequestTypeDef(TypedDict):
    GatewayInstanceArn: str,
```

## DescribeGatewayRequestTypeDef

```python
# DescribeGatewayRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DescribeGatewayRequestTypeDef


def get_value() -> DescribeGatewayRequestTypeDef:
    return {
        "GatewayArn": ...,
    }


# DescribeGatewayRequestTypeDef definition

class DescribeGatewayRequestTypeDef(TypedDict):
    GatewayArn: str,
```

## DescribeOfferingRequestTypeDef

```python
# DescribeOfferingRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DescribeOfferingRequestTypeDef


def get_value() -> DescribeOfferingRequestTypeDef:
    return {
        "OfferingArn": ...,
    }


# DescribeOfferingRequestTypeDef definition

class DescribeOfferingRequestTypeDef(TypedDict):
    OfferingArn: str,
```

## DescribeReservationRequestTypeDef

```python
# DescribeReservationRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DescribeReservationRequestTypeDef


def get_value() -> DescribeReservationRequestTypeDef:
    return {
        "ReservationArn": ...,
    }


# DescribeReservationRequestTypeDef definition

class DescribeReservationRequestTypeDef(TypedDict):
    ReservationArn: str,
```

## InterfaceRequestTypeDef

```python
# InterfaceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import InterfaceRequestTypeDef


def get_value() -> InterfaceRequestTypeDef:
    return {
        "Name": ...,
    }


# InterfaceRequestTypeDef definition

class InterfaceRequestTypeDef(TypedDict):
    Name: str,
```

## InterfaceTypeDef

```python
# InterfaceTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import InterfaceTypeDef


def get_value() -> InterfaceTypeDef:
    return {
        "Name": ...,
    }


# InterfaceTypeDef definition

class InterfaceTypeDef(TypedDict):
    Name: str,
```

## EncodingParametersRequestTypeDef

```python
# EncodingParametersRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import EncodingParametersRequestTypeDef


def get_value() -> EncodingParametersRequestTypeDef:
    return {
        "CompressionFactor": ...,
    }


# EncodingParametersRequestTypeDef definition

class EncodingParametersRequestTypeDef(TypedDict):
    CompressionFactor: float,
    EncoderProfile: EncoderProfileType,  # (1)
```

1. See [:material-code-brackets: EncoderProfileType](./literals.md#encoderprofiletype) 
## EncodingParametersTypeDef

```python
# EncodingParametersTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import EncodingParametersTypeDef


def get_value() -> EncodingParametersTypeDef:
    return {
        "CompressionFactor": ...,
    }


# EncodingParametersTypeDef definition

class EncodingParametersTypeDef(TypedDict):
    CompressionFactor: float,
    EncoderProfile: EncoderProfileType,  # (1)
```

1. See [:material-code-brackets: EncoderProfileType](./literals.md#encoderprofiletype) 
## SourcePriorityTypeDef

```python
# SourcePriorityTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import SourcePriorityTypeDef


def get_value() -> SourcePriorityTypeDef:
    return {
        "PrimarySource": ...,
    }


# SourcePriorityTypeDef definition

class SourcePriorityTypeDef(TypedDict):
    PrimarySource: NotRequired[str],
```

## MaintenanceTypeDef

```python
# MaintenanceTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import MaintenanceTypeDef


def get_value() -> MaintenanceTypeDef:
    return {
        "MaintenanceDay": ...,
    }


# MaintenanceTypeDef definition

class MaintenanceTypeDef(TypedDict):
    MaintenanceDay: NotRequired[MaintenanceDayType],  # (1)
    MaintenanceDeadline: NotRequired[str],
    MaintenanceScheduledDate: NotRequired[str],
    MaintenanceStartHour: NotRequired[str],
```

1. See [:material-code-brackets: MaintenanceDayType](./literals.md#maintenancedaytype) 
## FmtpRequestTypeDef

```python
# FmtpRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import FmtpRequestTypeDef


def get_value() -> FmtpRequestTypeDef:
    return {
        "ChannelOrder": ...,
    }


# FmtpRequestTypeDef definition

class FmtpRequestTypeDef(TypedDict):
    ChannelOrder: NotRequired[str],
    Colorimetry: NotRequired[ColorimetryType],  # (1)
    ExactFramerate: NotRequired[str],
    Par: NotRequired[str],
    Range: NotRequired[RangeType],  # (2)
    ScanMode: NotRequired[ScanModeType],  # (3)
    Tcs: NotRequired[TcsType],  # (4)
```

1. See [:material-code-brackets: ColorimetryType](./literals.md#colorimetrytype) 
2. See [:material-code-brackets: RangeType](./literals.md#rangetype) 
3. See [:material-code-brackets: ScanModeType](./literals.md#scanmodetype) 
4. See [:material-code-brackets: TcsType](./literals.md#tcstype) 
## FmtpTypeDef

```python
# FmtpTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import FmtpTypeDef


def get_value() -> FmtpTypeDef:
    return {
        "ChannelOrder": ...,
    }


# FmtpTypeDef definition

class FmtpTypeDef(TypedDict):
    ChannelOrder: NotRequired[str],
    Colorimetry: NotRequired[ColorimetryType],  # (1)
    ExactFramerate: NotRequired[str],
    Par: NotRequired[str],
    Range: NotRequired[RangeType],  # (2)
    ScanMode: NotRequired[ScanModeType],  # (3)
    Tcs: NotRequired[TcsType],  # (4)
```

1. See [:material-code-brackets: ColorimetryType](./literals.md#colorimetrytype) 
2. See [:material-code-brackets: RangeType](./literals.md#rangetype) 
3. See [:material-code-brackets: ScanModeType](./literals.md#scanmodetype) 
4. See [:material-code-brackets: TcsType](./literals.md#tcstype) 
## FrameResolutionTypeDef

```python
# FrameResolutionTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import FrameResolutionTypeDef


def get_value() -> FrameResolutionTypeDef:
    return {
        "FrameHeight": ...,
    }


# FrameResolutionTypeDef definition

class FrameResolutionTypeDef(TypedDict):
    FrameHeight: int,
    FrameWidth: int,
```

## FrozenFramesTypeDef

```python
# FrozenFramesTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import FrozenFramesTypeDef


def get_value() -> FrozenFramesTypeDef:
    return {
        "State": ...,
    }


# FrozenFramesTypeDef definition

class FrozenFramesTypeDef(TypedDict):
    State: NotRequired[StateType],  # (1)
    ThresholdSeconds: NotRequired[int],
```

1. See [:material-code-brackets: StateType](./literals.md#statetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import PaginatorConfigTypeDef


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

## ListBridgesRequestTypeDef

```python
# ListBridgesRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListBridgesRequestTypeDef


def get_value() -> ListBridgesRequestTypeDef:
    return {
        "FilterArn": ...,
    }


# ListBridgesRequestTypeDef definition

class ListBridgesRequestTypeDef(TypedDict):
    FilterArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListedBridgeTypeDef

```python
# ListedBridgeTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListedBridgeTypeDef


def get_value() -> ListedBridgeTypeDef:
    return {
        "BridgeArn": ...,
    }


# ListedBridgeTypeDef definition

class ListedBridgeTypeDef(TypedDict):
    BridgeArn: str,
    BridgeState: BridgeStateType,  # (1)
    BridgeType: str,
    Name: str,
    PlacementArn: str,
```

1. See [:material-code-brackets: BridgeStateType](./literals.md#bridgestatetype) 
## ListEntitlementsRequestTypeDef

```python
# ListEntitlementsRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListEntitlementsRequestTypeDef


def get_value() -> ListEntitlementsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListEntitlementsRequestTypeDef definition

class ListEntitlementsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListedEntitlementTypeDef

```python
# ListedEntitlementTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListedEntitlementTypeDef


def get_value() -> ListedEntitlementTypeDef:
    return {
        "DataTransferSubscriberFeePercent": ...,
    }


# ListedEntitlementTypeDef definition

class ListedEntitlementTypeDef(TypedDict):
    EntitlementArn: str,
    EntitlementName: str,
    DataTransferSubscriberFeePercent: NotRequired[int],
```

## ListFlowsRequestTypeDef

```python
# ListFlowsRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListFlowsRequestTypeDef


def get_value() -> ListFlowsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListFlowsRequestTypeDef definition

class ListFlowsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListGatewayInstancesRequestTypeDef

```python
# ListGatewayInstancesRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListGatewayInstancesRequestTypeDef


def get_value() -> ListGatewayInstancesRequestTypeDef:
    return {
        "FilterArn": ...,
    }


# ListGatewayInstancesRequestTypeDef definition

class ListGatewayInstancesRequestTypeDef(TypedDict):
    FilterArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListedGatewayInstanceTypeDef

```python
# ListedGatewayInstanceTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListedGatewayInstanceTypeDef


def get_value() -> ListedGatewayInstanceTypeDef:
    return {
        "GatewayArn": ...,
    }


# ListedGatewayInstanceTypeDef definition

class ListedGatewayInstanceTypeDef(TypedDict):
    GatewayArn: str,
    GatewayInstanceArn: str,
    InstanceId: str,
    InstanceState: NotRequired[InstanceStateType],  # (1)
```

1. See [:material-code-brackets: InstanceStateType](./literals.md#instancestatetype) 
## ListGatewaysRequestTypeDef

```python
# ListGatewaysRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListGatewaysRequestTypeDef


def get_value() -> ListGatewaysRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListGatewaysRequestTypeDef definition

class ListGatewaysRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListedGatewayTypeDef

```python
# ListedGatewayTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListedGatewayTypeDef


def get_value() -> ListedGatewayTypeDef:
    return {
        "GatewayArn": ...,
    }


# ListedGatewayTypeDef definition

class ListedGatewayTypeDef(TypedDict):
    GatewayArn: str,
    GatewayState: GatewayStateType,  # (1)
    Name: str,
```

1. See [:material-code-brackets: GatewayStateType](./literals.md#gatewaystatetype) 
## ListOfferingsRequestTypeDef

```python
# ListOfferingsRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListOfferingsRequestTypeDef


def get_value() -> ListOfferingsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListOfferingsRequestTypeDef definition

class ListOfferingsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListReservationsRequestTypeDef

```python
# ListReservationsRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListReservationsRequestTypeDef


def get_value() -> ListReservationsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListReservationsRequestTypeDef definition

class ListReservationsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ResourceSpecificationTypeDef

```python
# ResourceSpecificationTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ResourceSpecificationTypeDef


def get_value() -> ResourceSpecificationTypeDef:
    return {
        "ReservedBitrate": ...,
    }


# ResourceSpecificationTypeDef definition

class ResourceSpecificationTypeDef(TypedDict):
    ResourceType: ResourceTypeType,  # (1)
    ReservedBitrate: NotRequired[int],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## TransportTypeDef

```python
# TransportTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import TransportTypeDef


def get_value() -> TransportTypeDef:
    return {
        "CidrAllowList": ...,
    }


# TransportTypeDef definition

class TransportTypeDef(TypedDict):
    Protocol: ProtocolType,  # (1)
    CidrAllowList: NotRequired[List[str]],
    MaxBitrate: NotRequired[int],
    MaxLatency: NotRequired[int],
    MaxSyncBuffer: NotRequired[int],
    MinLatency: NotRequired[int],
    RemoteId: NotRequired[str],
    SenderControlPort: NotRequired[int],
    SenderIpAddress: NotRequired[str],
    SmoothingLatency: NotRequired[int],
    SourceListenerAddress: NotRequired[str],
    SourceListenerPort: NotRequired[int],
    StreamId: NotRequired[str],
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
## PurchaseOfferingRequestTypeDef

```python
# PurchaseOfferingRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import PurchaseOfferingRequestTypeDef


def get_value() -> PurchaseOfferingRequestTypeDef:
    return {
        "OfferingArn": ...,
    }


# PurchaseOfferingRequestTypeDef definition

class PurchaseOfferingRequestTypeDef(TypedDict):
    OfferingArn: str,
    ReservationName: str,
    Start: str,
```

## RemoveBridgeOutputRequestTypeDef

```python
# RemoveBridgeOutputRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import RemoveBridgeOutputRequestTypeDef


def get_value() -> RemoveBridgeOutputRequestTypeDef:
    return {
        "BridgeArn": ...,
    }


# RemoveBridgeOutputRequestTypeDef definition

class RemoveBridgeOutputRequestTypeDef(TypedDict):
    BridgeArn: str,
    OutputName: str,
```

## RemoveBridgeSourceRequestTypeDef

```python
# RemoveBridgeSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import RemoveBridgeSourceRequestTypeDef


def get_value() -> RemoveBridgeSourceRequestTypeDef:
    return {
        "BridgeArn": ...,
    }


# RemoveBridgeSourceRequestTypeDef definition

class RemoveBridgeSourceRequestTypeDef(TypedDict):
    BridgeArn: str,
    SourceName: str,
```

## RemoveFlowMediaStreamRequestTypeDef

```python
# RemoveFlowMediaStreamRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import RemoveFlowMediaStreamRequestTypeDef


def get_value() -> RemoveFlowMediaStreamRequestTypeDef:
    return {
        "FlowArn": ...,
    }


# RemoveFlowMediaStreamRequestTypeDef definition

class RemoveFlowMediaStreamRequestTypeDef(TypedDict):
    FlowArn: str,
    MediaStreamName: str,
```

## RemoveFlowOutputRequestTypeDef

```python
# RemoveFlowOutputRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import RemoveFlowOutputRequestTypeDef


def get_value() -> RemoveFlowOutputRequestTypeDef:
    return {
        "FlowArn": ...,
    }


# RemoveFlowOutputRequestTypeDef definition

class RemoveFlowOutputRequestTypeDef(TypedDict):
    FlowArn: str,
    OutputArn: str,
```

## RemoveFlowSourceRequestTypeDef

```python
# RemoveFlowSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import RemoveFlowSourceRequestTypeDef


def get_value() -> RemoveFlowSourceRequestTypeDef:
    return {
        "FlowArn": ...,
    }


# RemoveFlowSourceRequestTypeDef definition

class RemoveFlowSourceRequestTypeDef(TypedDict):
    FlowArn: str,
    SourceArn: str,
```

## RemoveFlowVpcInterfaceRequestTypeDef

```python
# RemoveFlowVpcInterfaceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import RemoveFlowVpcInterfaceRequestTypeDef


def get_value() -> RemoveFlowVpcInterfaceRequestTypeDef:
    return {
        "FlowArn": ...,
    }


# RemoveFlowVpcInterfaceRequestTypeDef definition

class RemoveFlowVpcInterfaceRequestTypeDef(TypedDict):
    FlowArn: str,
    VpcInterfaceName: str,
```

## RevokeFlowEntitlementRequestTypeDef

```python
# RevokeFlowEntitlementRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import RevokeFlowEntitlementRequestTypeDef


def get_value() -> RevokeFlowEntitlementRequestTypeDef:
    return {
        "EntitlementArn": ...,
    }


# RevokeFlowEntitlementRequestTypeDef definition

class RevokeFlowEntitlementRequestTypeDef(TypedDict):
    EntitlementArn: str,
    FlowArn: str,
```

## StartFlowRequestTypeDef

```python
# StartFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import StartFlowRequestTypeDef


def get_value() -> StartFlowRequestTypeDef:
    return {
        "FlowArn": ...,
    }


# StartFlowRequestTypeDef definition

class StartFlowRequestTypeDef(TypedDict):
    FlowArn: str,
```

## StopFlowRequestTypeDef

```python
# StopFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import StopFlowRequestTypeDef


def get_value() -> StopFlowRequestTypeDef:
    return {
        "FlowArn": ...,
    }


# StopFlowRequestTypeDef definition

class StopFlowRequestTypeDef(TypedDict):
    FlowArn: str,
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateBridgeNetworkOutputRequestTypeDef

```python
# UpdateBridgeNetworkOutputRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateBridgeNetworkOutputRequestTypeDef


def get_value() -> UpdateBridgeNetworkOutputRequestTypeDef:
    return {
        "IpAddress": ...,
    }


# UpdateBridgeNetworkOutputRequestTypeDef definition

class UpdateBridgeNetworkOutputRequestTypeDef(TypedDict):
    IpAddress: NotRequired[str],
    NetworkName: NotRequired[str],
    Port: NotRequired[int],
    Protocol: NotRequired[ProtocolType],  # (1)
    Ttl: NotRequired[int],
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
## UpdateEgressGatewayBridgeRequestTypeDef

```python
# UpdateEgressGatewayBridgeRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateEgressGatewayBridgeRequestTypeDef


def get_value() -> UpdateEgressGatewayBridgeRequestTypeDef:
    return {
        "MaxBitrate": ...,
    }


# UpdateEgressGatewayBridgeRequestTypeDef definition

class UpdateEgressGatewayBridgeRequestTypeDef(TypedDict):
    MaxBitrate: NotRequired[int],
```

## UpdateIngressGatewayBridgeRequestTypeDef

```python
# UpdateIngressGatewayBridgeRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateIngressGatewayBridgeRequestTypeDef


def get_value() -> UpdateIngressGatewayBridgeRequestTypeDef:
    return {
        "MaxBitrate": ...,
    }


# UpdateIngressGatewayBridgeRequestTypeDef definition

class UpdateIngressGatewayBridgeRequestTypeDef(TypedDict):
    MaxBitrate: NotRequired[int],
    MaxOutputs: NotRequired[int],
```

## UpdateBridgeStateRequestTypeDef

```python
# UpdateBridgeStateRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateBridgeStateRequestTypeDef


def get_value() -> UpdateBridgeStateRequestTypeDef:
    return {
        "BridgeArn": ...,
    }


# UpdateBridgeStateRequestTypeDef definition

class UpdateBridgeStateRequestTypeDef(TypedDict):
    BridgeArn: str,
    DesiredState: DesiredStateType,  # (1)
```

1. See [:material-code-brackets: DesiredStateType](./literals.md#desiredstatetype) 
## UpdateEncryptionTypeDef

```python
# UpdateEncryptionTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateEncryptionTypeDef


def get_value() -> UpdateEncryptionTypeDef:
    return {
        "Algorithm": ...,
    }


# UpdateEncryptionTypeDef definition

class UpdateEncryptionTypeDef(TypedDict):
    Algorithm: NotRequired[AlgorithmType],  # (1)
    ConstantInitializationVector: NotRequired[str],
    DeviceId: NotRequired[str],
    KeyType: NotRequired[KeyTypeType],  # (2)
    Region: NotRequired[str],
    ResourceId: NotRequired[str],
    RoleArn: NotRequired[str],
    SecretArn: NotRequired[str],
    Url: NotRequired[str],
```

1. See [:material-code-brackets: AlgorithmType](./literals.md#algorithmtype) 
2. See [:material-code-brackets: KeyTypeType](./literals.md#keytypetype) 
## UpdateMaintenanceTypeDef

```python
# UpdateMaintenanceTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateMaintenanceTypeDef


def get_value() -> UpdateMaintenanceTypeDef:
    return {
        "MaintenanceDay": ...,
    }


# UpdateMaintenanceTypeDef definition

class UpdateMaintenanceTypeDef(TypedDict):
    MaintenanceDay: NotRequired[MaintenanceDayType],  # (1)
    MaintenanceScheduledDate: NotRequired[str],
    MaintenanceStartHour: NotRequired[str],
```

1. See [:material-code-brackets: MaintenanceDayType](./literals.md#maintenancedaytype) 
## UpdateGatewayInstanceRequestTypeDef

```python
# UpdateGatewayInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateGatewayInstanceRequestTypeDef


def get_value() -> UpdateGatewayInstanceRequestTypeDef:
    return {
        "GatewayInstanceArn": ...,
    }


# UpdateGatewayInstanceRequestTypeDef definition

class UpdateGatewayInstanceRequestTypeDef(TypedDict):
    GatewayInstanceArn: str,
    BridgePlacement: NotRequired[BridgePlacementType],  # (1)
```

1. See [:material-code-brackets: BridgePlacementType](./literals.md#bridgeplacementtype) 
## AddBridgeFlowSourceRequestTypeDef

```python
# AddBridgeFlowSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AddBridgeFlowSourceRequestTypeDef


def get_value() -> AddBridgeFlowSourceRequestTypeDef:
    return {
        "FlowArn": ...,
    }


# AddBridgeFlowSourceRequestTypeDef definition

class AddBridgeFlowSourceRequestTypeDef(TypedDict):
    FlowArn: str,
    Name: str,
    FlowVpcInterfaceAttachment: NotRequired[VpcInterfaceAttachmentTypeDef],  # (1)
```

1. See [:material-code-braces: VpcInterfaceAttachmentTypeDef](./type_defs.md#vpcinterfaceattachmenttypedef) 
## BridgeFlowSourceTypeDef

```python
# BridgeFlowSourceTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import BridgeFlowSourceTypeDef


def get_value() -> BridgeFlowSourceTypeDef:
    return {
        "FlowArn": ...,
    }


# BridgeFlowSourceTypeDef definition

class BridgeFlowSourceTypeDef(TypedDict):
    FlowArn: str,
    Name: str,
    FlowVpcInterfaceAttachment: NotRequired[VpcInterfaceAttachmentTypeDef],  # (1)
    OutputArn: NotRequired[str],
```

1. See [:material-code-braces: VpcInterfaceAttachmentTypeDef](./type_defs.md#vpcinterfaceattachmenttypedef) 
## GatewayBridgeSourceTypeDef

```python
# GatewayBridgeSourceTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import GatewayBridgeSourceTypeDef


def get_value() -> GatewayBridgeSourceTypeDef:
    return {
        "BridgeArn": ...,
    }


# GatewayBridgeSourceTypeDef definition

class GatewayBridgeSourceTypeDef(TypedDict):
    BridgeArn: str,
    VpcInterfaceAttachment: NotRequired[VpcInterfaceAttachmentTypeDef],  # (1)
```

1. See [:material-code-braces: VpcInterfaceAttachmentTypeDef](./type_defs.md#vpcinterfaceattachmenttypedef) 
## SetGatewayBridgeSourceRequestTypeDef

```python
# SetGatewayBridgeSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import SetGatewayBridgeSourceRequestTypeDef


def get_value() -> SetGatewayBridgeSourceRequestTypeDef:
    return {
        "BridgeArn": ...,
    }


# SetGatewayBridgeSourceRequestTypeDef definition

class SetGatewayBridgeSourceRequestTypeDef(TypedDict):
    BridgeArn: str,
    VpcInterfaceAttachment: NotRequired[VpcInterfaceAttachmentTypeDef],  # (1)
```

1. See [:material-code-braces: VpcInterfaceAttachmentTypeDef](./type_defs.md#vpcinterfaceattachmenttypedef) 
## UpdateBridgeFlowSourceRequestTypeDef

```python
# UpdateBridgeFlowSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateBridgeFlowSourceRequestTypeDef


def get_value() -> UpdateBridgeFlowSourceRequestTypeDef:
    return {
        "FlowArn": ...,
    }


# UpdateBridgeFlowSourceRequestTypeDef definition

class UpdateBridgeFlowSourceRequestTypeDef(TypedDict):
    FlowArn: NotRequired[str],
    FlowVpcInterfaceAttachment: NotRequired[VpcInterfaceAttachmentTypeDef],  # (1)
```

1. See [:material-code-braces: VpcInterfaceAttachmentTypeDef](./type_defs.md#vpcinterfaceattachmenttypedef) 
## UpdateGatewayBridgeSourceRequestTypeDef

```python
# UpdateGatewayBridgeSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateGatewayBridgeSourceRequestTypeDef


def get_value() -> UpdateGatewayBridgeSourceRequestTypeDef:
    return {
        "BridgeArn": ...,
    }


# UpdateGatewayBridgeSourceRequestTypeDef definition

class UpdateGatewayBridgeSourceRequestTypeDef(TypedDict):
    BridgeArn: NotRequired[str],
    VpcInterfaceAttachment: NotRequired[VpcInterfaceAttachmentTypeDef],  # (1)
```

1. See [:material-code-braces: VpcInterfaceAttachmentTypeDef](./type_defs.md#vpcinterfaceattachmenttypedef) 
## AddBridgeOutputRequestTypeDef

```python
# AddBridgeOutputRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AddBridgeOutputRequestTypeDef


def get_value() -> AddBridgeOutputRequestTypeDef:
    return {
        "NetworkOutput": ...,
    }


# AddBridgeOutputRequestTypeDef definition

class AddBridgeOutputRequestTypeDef(TypedDict):
    NetworkOutput: NotRequired[AddBridgeNetworkOutputRequestTypeDef],  # (1)
```

1. See [:material-code-braces: AddBridgeNetworkOutputRequestTypeDef](./type_defs.md#addbridgenetworkoutputrequesttypedef) 
## AddBridgeNetworkSourceRequestTypeDef

```python
# AddBridgeNetworkSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AddBridgeNetworkSourceRequestTypeDef


def get_value() -> AddBridgeNetworkSourceRequestTypeDef:
    return {
        "MulticastIp": ...,
    }


# AddBridgeNetworkSourceRequestTypeDef definition

class AddBridgeNetworkSourceRequestTypeDef(TypedDict):
    MulticastIp: str,
    Name: str,
    NetworkName: str,
    Port: int,
    Protocol: ProtocolType,  # (2)
    MulticastSourceSettings: NotRequired[MulticastSourceSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: MulticastSourceSettingsTypeDef](./type_defs.md#multicastsourcesettingstypedef) 
2. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
## BridgeNetworkSourceTypeDef

```python
# BridgeNetworkSourceTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import BridgeNetworkSourceTypeDef


def get_value() -> BridgeNetworkSourceTypeDef:
    return {
        "MulticastIp": ...,
    }


# BridgeNetworkSourceTypeDef definition

class BridgeNetworkSourceTypeDef(TypedDict):
    MulticastIp: str,
    Name: str,
    NetworkName: str,
    Port: int,
    Protocol: ProtocolType,  # (2)
    MulticastSourceSettings: NotRequired[MulticastSourceSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: MulticastSourceSettingsTypeDef](./type_defs.md#multicastsourcesettingstypedef) 
2. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
## UpdateBridgeNetworkSourceRequestTypeDef

```python
# UpdateBridgeNetworkSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateBridgeNetworkSourceRequestTypeDef


def get_value() -> UpdateBridgeNetworkSourceRequestTypeDef:
    return {
        "MulticastIp": ...,
    }


# UpdateBridgeNetworkSourceRequestTypeDef definition

class UpdateBridgeNetworkSourceRequestTypeDef(TypedDict):
    MulticastIp: NotRequired[str],
    MulticastSourceSettings: NotRequired[MulticastSourceSettingsTypeDef],  # (1)
    NetworkName: NotRequired[str],
    Port: NotRequired[int],
    Protocol: NotRequired[ProtocolType],  # (2)
```

1. See [:material-code-braces: MulticastSourceSettingsTypeDef](./type_defs.md#multicastsourcesettingstypedef) 
2. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
## DeleteBridgeResponseTypeDef

```python
# DeleteBridgeResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DeleteBridgeResponseTypeDef


def get_value() -> DeleteBridgeResponseTypeDef:
    return {
        "BridgeArn": ...,
    }


# DeleteBridgeResponseTypeDef definition

class DeleteBridgeResponseTypeDef(TypedDict):
    BridgeArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteFlowResponseTypeDef

```python
# DeleteFlowResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DeleteFlowResponseTypeDef


def get_value() -> DeleteFlowResponseTypeDef:
    return {
        "FlowArn": ...,
    }


# DeleteFlowResponseTypeDef definition

class DeleteFlowResponseTypeDef(TypedDict):
    FlowArn: str,
    Status: StatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteGatewayResponseTypeDef

```python
# DeleteGatewayResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DeleteGatewayResponseTypeDef


def get_value() -> DeleteGatewayResponseTypeDef:
    return {
        "GatewayArn": ...,
    }


# DeleteGatewayResponseTypeDef definition

class DeleteGatewayResponseTypeDef(TypedDict):
    GatewayArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeregisterGatewayInstanceResponseTypeDef

```python
# DeregisterGatewayInstanceResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DeregisterGatewayInstanceResponseTypeDef


def get_value() -> DeregisterGatewayInstanceResponseTypeDef:
    return {
        "GatewayInstanceArn": ...,
    }


# DeregisterGatewayInstanceResponseTypeDef definition

class DeregisterGatewayInstanceResponseTypeDef(TypedDict):
    GatewayInstanceArn: str,
    InstanceState: InstanceStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: InstanceStateType](./literals.md#instancestatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveBridgeOutputResponseTypeDef

```python
# RemoveBridgeOutputResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import RemoveBridgeOutputResponseTypeDef


def get_value() -> RemoveBridgeOutputResponseTypeDef:
    return {
        "BridgeArn": ...,
    }


# RemoveBridgeOutputResponseTypeDef definition

class RemoveBridgeOutputResponseTypeDef(TypedDict):
    BridgeArn: str,
    OutputName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveBridgeSourceResponseTypeDef

```python
# RemoveBridgeSourceResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import RemoveBridgeSourceResponseTypeDef


def get_value() -> RemoveBridgeSourceResponseTypeDef:
    return {
        "BridgeArn": ...,
    }


# RemoveBridgeSourceResponseTypeDef definition

class RemoveBridgeSourceResponseTypeDef(TypedDict):
    BridgeArn: str,
    SourceName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveFlowMediaStreamResponseTypeDef

```python
# RemoveFlowMediaStreamResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import RemoveFlowMediaStreamResponseTypeDef


def get_value() -> RemoveFlowMediaStreamResponseTypeDef:
    return {
        "FlowArn": ...,
    }


# RemoveFlowMediaStreamResponseTypeDef definition

class RemoveFlowMediaStreamResponseTypeDef(TypedDict):
    FlowArn: str,
    MediaStreamName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveFlowOutputResponseTypeDef

```python
# RemoveFlowOutputResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import RemoveFlowOutputResponseTypeDef


def get_value() -> RemoveFlowOutputResponseTypeDef:
    return {
        "FlowArn": ...,
    }


# RemoveFlowOutputResponseTypeDef definition

class RemoveFlowOutputResponseTypeDef(TypedDict):
    FlowArn: str,
    OutputArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveFlowSourceResponseTypeDef

```python
# RemoveFlowSourceResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import RemoveFlowSourceResponseTypeDef


def get_value() -> RemoveFlowSourceResponseTypeDef:
    return {
        "FlowArn": ...,
    }


# RemoveFlowSourceResponseTypeDef definition

class RemoveFlowSourceResponseTypeDef(TypedDict):
    FlowArn: str,
    SourceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveFlowVpcInterfaceResponseTypeDef

```python
# RemoveFlowVpcInterfaceResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import RemoveFlowVpcInterfaceResponseTypeDef


def get_value() -> RemoveFlowVpcInterfaceResponseTypeDef:
    return {
        "FlowArn": ...,
    }


# RemoveFlowVpcInterfaceResponseTypeDef definition

class RemoveFlowVpcInterfaceResponseTypeDef(TypedDict):
    FlowArn: str,
    NonDeletedNetworkInterfaceIds: List[str],
    VpcInterfaceName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RevokeFlowEntitlementResponseTypeDef

```python
# RevokeFlowEntitlementResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import RevokeFlowEntitlementResponseTypeDef


def get_value() -> RevokeFlowEntitlementResponseTypeDef:
    return {
        "EntitlementArn": ...,
    }


# RevokeFlowEntitlementResponseTypeDef definition

class RevokeFlowEntitlementResponseTypeDef(TypedDict):
    EntitlementArn: str,
    FlowArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartFlowResponseTypeDef

```python
# StartFlowResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import StartFlowResponseTypeDef


def get_value() -> StartFlowResponseTypeDef:
    return {
        "FlowArn": ...,
    }


# StartFlowResponseTypeDef definition

class StartFlowResponseTypeDef(TypedDict):
    FlowArn: str,
    Status: StatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopFlowResponseTypeDef

```python
# StopFlowResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import StopFlowResponseTypeDef


def get_value() -> StopFlowResponseTypeDef:
    return {
        "FlowArn": ...,
    }


# StopFlowResponseTypeDef definition

class StopFlowResponseTypeDef(TypedDict):
    FlowArn: str,
    Status: StatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBridgeStateResponseTypeDef

```python
# UpdateBridgeStateResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateBridgeStateResponseTypeDef


def get_value() -> UpdateBridgeStateResponseTypeDef:
    return {
        "BridgeArn": ...,
    }


# UpdateBridgeStateResponseTypeDef definition

class UpdateBridgeStateResponseTypeDef(TypedDict):
    BridgeArn: str,
    DesiredState: DesiredStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DesiredStateType](./literals.md#desiredstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGatewayInstanceResponseTypeDef

```python
# UpdateGatewayInstanceResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateGatewayInstanceResponseTypeDef


def get_value() -> UpdateGatewayInstanceResponseTypeDef:
    return {
        "BridgePlacement": ...,
    }


# UpdateGatewayInstanceResponseTypeDef definition

class UpdateGatewayInstanceResponseTypeDef(TypedDict):
    BridgePlacement: BridgePlacementType,  # (1)
    GatewayInstanceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: BridgePlacementType](./literals.md#bridgeplacementtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddFlowVpcInterfacesRequestTypeDef

```python
# AddFlowVpcInterfacesRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AddFlowVpcInterfacesRequestTypeDef


def get_value() -> AddFlowVpcInterfacesRequestTypeDef:
    return {
        "FlowArn": ...,
    }


# AddFlowVpcInterfacesRequestTypeDef definition

class AddFlowVpcInterfacesRequestTypeDef(TypedDict):
    FlowArn: str,
    VpcInterfaces: Sequence[VpcInterfaceRequestTypeDef],  # (1)
```

1. See [:material-code-braces: VpcInterfaceRequestTypeDef](./type_defs.md#vpcinterfacerequesttypedef) 
## AddFlowVpcInterfacesResponseTypeDef

```python
# AddFlowVpcInterfacesResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AddFlowVpcInterfacesResponseTypeDef


def get_value() -> AddFlowVpcInterfacesResponseTypeDef:
    return {
        "FlowArn": ...,
    }


# AddFlowVpcInterfacesResponseTypeDef definition

class AddFlowVpcInterfacesResponseTypeDef(TypedDict):
    FlowArn: str,
    VpcInterfaces: List[VpcInterfaceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VpcInterfaceTypeDef](./type_defs.md#vpcinterfacetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EntitlementTypeDef

```python
# EntitlementTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import EntitlementTypeDef


def get_value() -> EntitlementTypeDef:
    return {
        "DataTransferSubscriberFeePercent": ...,
    }


# EntitlementTypeDef definition

class EntitlementTypeDef(TypedDict):
    EntitlementArn: str,
    Name: str,
    Subscribers: List[str],
    DataTransferSubscriberFeePercent: NotRequired[int],
    Description: NotRequired[str],
    Encryption: NotRequired[EncryptionTypeDef],  # (1)
    EntitlementStatus: NotRequired[EntitlementStatusType],  # (2)
```

1. See [:material-code-braces: EncryptionTypeDef](./type_defs.md#encryptiontypedef) 
2. See [:material-code-brackets: EntitlementStatusType](./literals.md#entitlementstatustype) 
## GrantEntitlementRequestTypeDef

```python
# GrantEntitlementRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import GrantEntitlementRequestTypeDef


def get_value() -> GrantEntitlementRequestTypeDef:
    return {
        "DataTransferSubscriberFeePercent": ...,
    }


# GrantEntitlementRequestTypeDef definition

class GrantEntitlementRequestTypeDef(TypedDict):
    Subscribers: Sequence[str],
    DataTransferSubscriberFeePercent: NotRequired[int],
    Description: NotRequired[str],
    Encryption: NotRequired[EncryptionTypeDef],  # (1)
    EntitlementStatus: NotRequired[EntitlementStatusType],  # (2)
    Name: NotRequired[str],
```

1. See [:material-code-braces: EncryptionTypeDef](./type_defs.md#encryptiontypedef) 
2. See [:material-code-brackets: EntitlementStatusType](./literals.md#entitlementstatustype) 
## AudioMonitoringSettingTypeDef

```python
# AudioMonitoringSettingTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AudioMonitoringSettingTypeDef


def get_value() -> AudioMonitoringSettingTypeDef:
    return {
        "SilentAudio": ...,
    }


# AudioMonitoringSettingTypeDef definition

class AudioMonitoringSettingTypeDef(TypedDict):
    SilentAudio: NotRequired[SilentAudioTypeDef],  # (1)
```

1. See [:material-code-braces: SilentAudioTypeDef](./type_defs.md#silentaudiotypedef) 
## BridgeOutputTypeDef

```python
# BridgeOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import BridgeOutputTypeDef


def get_value() -> BridgeOutputTypeDef:
    return {
        "FlowOutput": ...,
    }


# BridgeOutputTypeDef definition

class BridgeOutputTypeDef(TypedDict):
    FlowOutput: NotRequired[BridgeFlowOutputTypeDef],  # (1)
    NetworkOutput: NotRequired[BridgeNetworkOutputTypeDef],  # (2)
```

1. See [:material-code-braces: BridgeFlowOutputTypeDef](./type_defs.md#bridgeflowoutputtypedef) 
2. See [:material-code-braces: BridgeNetworkOutputTypeDef](./type_defs.md#bridgenetworkoutputtypedef) 
## GatewayInstanceTypeDef

```python
# GatewayInstanceTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import GatewayInstanceTypeDef


def get_value() -> GatewayInstanceTypeDef:
    return {
        "BridgePlacement": ...,
    }


# GatewayInstanceTypeDef definition

class GatewayInstanceTypeDef(TypedDict):
    BridgePlacement: BridgePlacementType,  # (1)
    ConnectionStatus: ConnectionStatusType,  # (2)
    GatewayArn: str,
    GatewayInstanceArn: str,
    InstanceId: str,
    InstanceState: InstanceStateType,  # (4)
    RunningBridgeCount: int,
    InstanceMessages: NotRequired[List[MessageDetailTypeDef]],  # (3)
```

1. See [:material-code-brackets: BridgePlacementType](./literals.md#bridgeplacementtype) 
2. See [:material-code-brackets: ConnectionStatusType](./literals.md#connectionstatustype) 
3. See [:material-code-braces: MessageDetailTypeDef](./type_defs.md#messagedetailtypedef) 
4. See [:material-code-brackets: InstanceStateType](./literals.md#instancestatetype) 
## ThumbnailDetailsTypeDef

```python
# ThumbnailDetailsTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ThumbnailDetailsTypeDef


def get_value() -> ThumbnailDetailsTypeDef:
    return {
        "FlowArn": ...,
    }


# ThumbnailDetailsTypeDef definition

class ThumbnailDetailsTypeDef(TypedDict):
    FlowArn: str,
    ThumbnailMessages: List[MessageDetailTypeDef],  # (1)
    Thumbnail: NotRequired[str],
    Timecode: NotRequired[str],
    Timestamp: NotRequired[datetime],
```

1. See [:material-code-braces: MessageDetailTypeDef](./type_defs.md#messagedetailtypedef) 
## CreateGatewayRequestTypeDef

```python
# CreateGatewayRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import CreateGatewayRequestTypeDef


def get_value() -> CreateGatewayRequestTypeDef:
    return {
        "EgressCidrBlocks": ...,
    }


# CreateGatewayRequestTypeDef definition

class CreateGatewayRequestTypeDef(TypedDict):
    EgressCidrBlocks: Sequence[str],
    Name: str,
    Networks: Sequence[GatewayNetworkTypeDef],  # (1)
```

1. See [:material-code-braces: GatewayNetworkTypeDef](./type_defs.md#gatewaynetworktypedef) 
## GatewayTypeDef

```python
# GatewayTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import GatewayTypeDef


def get_value() -> GatewayTypeDef:
    return {
        "EgressCidrBlocks": ...,
    }


# GatewayTypeDef definition

class GatewayTypeDef(TypedDict):
    EgressCidrBlocks: List[str],
    GatewayArn: str,
    Name: str,
    Networks: List[GatewayNetworkTypeDef],  # (3)
    GatewayMessages: NotRequired[List[MessageDetailTypeDef]],  # (1)
    GatewayState: NotRequired[GatewayStateType],  # (2)
```

1. See [:material-code-braces: MessageDetailTypeDef](./type_defs.md#messagedetailtypedef) 
2. See [:material-code-brackets: GatewayStateType](./literals.md#gatewaystatetype) 
3. See [:material-code-braces: GatewayNetworkTypeDef](./type_defs.md#gatewaynetworktypedef) 
## DescribeFlowRequestWaitExtraExtraTypeDef

```python
# DescribeFlowRequestWaitExtraExtraTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DescribeFlowRequestWaitExtraExtraTypeDef


def get_value() -> DescribeFlowRequestWaitExtraExtraTypeDef:
    return {
        "FlowArn": ...,
    }


# DescribeFlowRequestWaitExtraExtraTypeDef definition

class DescribeFlowRequestWaitExtraExtraTypeDef(TypedDict):
    FlowArn: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeFlowRequestWaitExtraTypeDef

```python
# DescribeFlowRequestWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DescribeFlowRequestWaitExtraTypeDef


def get_value() -> DescribeFlowRequestWaitExtraTypeDef:
    return {
        "FlowArn": ...,
    }


# DescribeFlowRequestWaitExtraTypeDef definition

class DescribeFlowRequestWaitExtraTypeDef(TypedDict):
    FlowArn: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeFlowRequestWaitTypeDef

```python
# DescribeFlowRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DescribeFlowRequestWaitTypeDef


def get_value() -> DescribeFlowRequestWaitTypeDef:
    return {
        "FlowArn": ...,
    }


# DescribeFlowRequestWaitTypeDef definition

class DescribeFlowRequestWaitTypeDef(TypedDict):
    FlowArn: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DestinationConfigurationRequestTypeDef

```python
# DestinationConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DestinationConfigurationRequestTypeDef


def get_value() -> DestinationConfigurationRequestTypeDef:
    return {
        "DestinationIp": ...,
    }


# DestinationConfigurationRequestTypeDef definition

class DestinationConfigurationRequestTypeDef(TypedDict):
    DestinationIp: str,
    DestinationPort: int,
    Interface: InterfaceRequestTypeDef,  # (1)
```

1. See [:material-code-braces: InterfaceRequestTypeDef](./type_defs.md#interfacerequesttypedef) 
## InputConfigurationRequestTypeDef

```python
# InputConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import InputConfigurationRequestTypeDef


def get_value() -> InputConfigurationRequestTypeDef:
    return {
        "InputPort": ...,
    }


# InputConfigurationRequestTypeDef definition

class InputConfigurationRequestTypeDef(TypedDict):
    InputPort: int,
    Interface: InterfaceRequestTypeDef,  # (1)
```

1. See [:material-code-braces: InterfaceRequestTypeDef](./type_defs.md#interfacerequesttypedef) 
## DestinationConfigurationTypeDef

```python
# DestinationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DestinationConfigurationTypeDef


def get_value() -> DestinationConfigurationTypeDef:
    return {
        "DestinationIp": ...,
    }


# DestinationConfigurationTypeDef definition

class DestinationConfigurationTypeDef(TypedDict):
    DestinationIp: str,
    DestinationPort: int,
    Interface: InterfaceTypeDef,  # (1)
    OutboundIp: str,
```

1. See [:material-code-braces: InterfaceTypeDef](./type_defs.md#interfacetypedef) 
## InputConfigurationTypeDef

```python
# InputConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import InputConfigurationTypeDef


def get_value() -> InputConfigurationTypeDef:
    return {
        "InputIp": ...,
    }


# InputConfigurationTypeDef definition

class InputConfigurationTypeDef(TypedDict):
    InputIp: str,
    InputPort: int,
    Interface: InterfaceTypeDef,  # (1)
```

1. See [:material-code-braces: InterfaceTypeDef](./type_defs.md#interfacetypedef) 
## FailoverConfigTypeDef

```python
# FailoverConfigTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import FailoverConfigTypeDef


def get_value() -> FailoverConfigTypeDef:
    return {
        "FailoverMode": ...,
    }


# FailoverConfigTypeDef definition

class FailoverConfigTypeDef(TypedDict):
    FailoverMode: NotRequired[FailoverModeType],  # (1)
    RecoveryWindow: NotRequired[int],
    SourcePriority: NotRequired[SourcePriorityTypeDef],  # (2)
    State: NotRequired[StateType],  # (3)
```

1. See [:material-code-brackets: FailoverModeType](./literals.md#failovermodetype) 
2. See [:material-code-braces: SourcePriorityTypeDef](./type_defs.md#sourceprioritytypedef) 
3. See [:material-code-brackets: StateType](./literals.md#statetype) 
## UpdateFailoverConfigTypeDef

```python
# UpdateFailoverConfigTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateFailoverConfigTypeDef


def get_value() -> UpdateFailoverConfigTypeDef:
    return {
        "FailoverMode": ...,
    }


# UpdateFailoverConfigTypeDef definition

class UpdateFailoverConfigTypeDef(TypedDict):
    FailoverMode: NotRequired[FailoverModeType],  # (1)
    RecoveryWindow: NotRequired[int],
    SourcePriority: NotRequired[SourcePriorityTypeDef],  # (2)
    State: NotRequired[StateType],  # (3)
```

1. See [:material-code-brackets: FailoverModeType](./literals.md#failovermodetype) 
2. See [:material-code-braces: SourcePriorityTypeDef](./type_defs.md#sourceprioritytypedef) 
3. See [:material-code-brackets: StateType](./literals.md#statetype) 
## ListedFlowTypeDef

```python
# ListedFlowTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListedFlowTypeDef


def get_value() -> ListedFlowTypeDef:
    return {
        "AvailabilityZone": ...,
    }


# ListedFlowTypeDef definition

class ListedFlowTypeDef(TypedDict):
    AvailabilityZone: str,
    Description: str,
    FlowArn: str,
    Name: str,
    SourceType: SourceTypeType,  # (1)
    Status: StatusType,  # (2)
    Maintenance: NotRequired[MaintenanceTypeDef],  # (3)
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
3. See [:material-code-braces: MaintenanceTypeDef](./type_defs.md#maintenancetypedef) 
## MediaStreamAttributesRequestTypeDef

```python
# MediaStreamAttributesRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import MediaStreamAttributesRequestTypeDef


def get_value() -> MediaStreamAttributesRequestTypeDef:
    return {
        "Fmtp": ...,
    }


# MediaStreamAttributesRequestTypeDef definition

class MediaStreamAttributesRequestTypeDef(TypedDict):
    Fmtp: NotRequired[FmtpRequestTypeDef],  # (1)
    Lang: NotRequired[str],
```

1. See [:material-code-braces: FmtpRequestTypeDef](./type_defs.md#fmtprequesttypedef) 
## MediaStreamAttributesTypeDef

```python
# MediaStreamAttributesTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import MediaStreamAttributesTypeDef


def get_value() -> MediaStreamAttributesTypeDef:
    return {
        "Fmtp": ...,
    }


# MediaStreamAttributesTypeDef definition

class MediaStreamAttributesTypeDef(TypedDict):
    Fmtp: FmtpTypeDef,  # (1)
    Lang: NotRequired[str],
```

1. See [:material-code-braces: FmtpTypeDef](./type_defs.md#fmtptypedef) 
## TransportStreamTypeDef

```python
# TransportStreamTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import TransportStreamTypeDef


def get_value() -> TransportStreamTypeDef:
    return {
        "Channels": ...,
    }


# TransportStreamTypeDef definition

class TransportStreamTypeDef(TypedDict):
    Pid: int,
    StreamType: str,
    Channels: NotRequired[int],
    Codec: NotRequired[str],
    FrameRate: NotRequired[str],
    FrameResolution: NotRequired[FrameResolutionTypeDef],  # (1)
    SampleRate: NotRequired[int],
    SampleSize: NotRequired[int],
```

1. See [:material-code-braces: FrameResolutionTypeDef](./type_defs.md#frameresolutiontypedef) 
## VideoMonitoringSettingTypeDef

```python
# VideoMonitoringSettingTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import VideoMonitoringSettingTypeDef


def get_value() -> VideoMonitoringSettingTypeDef:
    return {
        "BlackFrames": ...,
    }


# VideoMonitoringSettingTypeDef definition

class VideoMonitoringSettingTypeDef(TypedDict):
    BlackFrames: NotRequired[BlackFramesTypeDef],  # (1)
    FrozenFrames: NotRequired[FrozenFramesTypeDef],  # (2)
```

1. See [:material-code-braces: BlackFramesTypeDef](./type_defs.md#blackframestypedef) 
2. See [:material-code-braces: FrozenFramesTypeDef](./type_defs.md#frozenframestypedef) 
## ListBridgesRequestPaginateTypeDef

```python
# ListBridgesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListBridgesRequestPaginateTypeDef


def get_value() -> ListBridgesRequestPaginateTypeDef:
    return {
        "FilterArn": ...,
    }


# ListBridgesRequestPaginateTypeDef definition

class ListBridgesRequestPaginateTypeDef(TypedDict):
    FilterArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEntitlementsRequestPaginateTypeDef

```python
# ListEntitlementsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListEntitlementsRequestPaginateTypeDef


def get_value() -> ListEntitlementsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListEntitlementsRequestPaginateTypeDef definition

class ListEntitlementsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFlowsRequestPaginateTypeDef

```python
# ListFlowsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListFlowsRequestPaginateTypeDef


def get_value() -> ListFlowsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListFlowsRequestPaginateTypeDef definition

class ListFlowsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGatewayInstancesRequestPaginateTypeDef

```python
# ListGatewayInstancesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListGatewayInstancesRequestPaginateTypeDef


def get_value() -> ListGatewayInstancesRequestPaginateTypeDef:
    return {
        "FilterArn": ...,
    }


# ListGatewayInstancesRequestPaginateTypeDef definition

class ListGatewayInstancesRequestPaginateTypeDef(TypedDict):
    FilterArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGatewaysRequestPaginateTypeDef

```python
# ListGatewaysRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListGatewaysRequestPaginateTypeDef


def get_value() -> ListGatewaysRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListGatewaysRequestPaginateTypeDef definition

class ListGatewaysRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOfferingsRequestPaginateTypeDef

```python
# ListOfferingsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListOfferingsRequestPaginateTypeDef


def get_value() -> ListOfferingsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListOfferingsRequestPaginateTypeDef definition

class ListOfferingsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReservationsRequestPaginateTypeDef

```python
# ListReservationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListReservationsRequestPaginateTypeDef


def get_value() -> ListReservationsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListReservationsRequestPaginateTypeDef definition

class ListReservationsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBridgesResponseTypeDef

```python
# ListBridgesResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListBridgesResponseTypeDef


def get_value() -> ListBridgesResponseTypeDef:
    return {
        "Bridges": ...,
    }


# ListBridgesResponseTypeDef definition

class ListBridgesResponseTypeDef(TypedDict):
    Bridges: List[ListedBridgeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListedBridgeTypeDef](./type_defs.md#listedbridgetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEntitlementsResponseTypeDef

```python
# ListEntitlementsResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListEntitlementsResponseTypeDef


def get_value() -> ListEntitlementsResponseTypeDef:
    return {
        "Entitlements": ...,
    }


# ListEntitlementsResponseTypeDef definition

class ListEntitlementsResponseTypeDef(TypedDict):
    Entitlements: List[ListedEntitlementTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListedEntitlementTypeDef](./type_defs.md#listedentitlementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGatewayInstancesResponseTypeDef

```python
# ListGatewayInstancesResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListGatewayInstancesResponseTypeDef


def get_value() -> ListGatewayInstancesResponseTypeDef:
    return {
        "Instances": ...,
    }


# ListGatewayInstancesResponseTypeDef definition

class ListGatewayInstancesResponseTypeDef(TypedDict):
    Instances: List[ListedGatewayInstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListedGatewayInstanceTypeDef](./type_defs.md#listedgatewayinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGatewaysResponseTypeDef

```python
# ListGatewaysResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListGatewaysResponseTypeDef


def get_value() -> ListGatewaysResponseTypeDef:
    return {
        "Gateways": ...,
    }


# ListGatewaysResponseTypeDef definition

class ListGatewaysResponseTypeDef(TypedDict):
    Gateways: List[ListedGatewayTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListedGatewayTypeDef](./type_defs.md#listedgatewaytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OfferingTypeDef

```python
# OfferingTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import OfferingTypeDef


def get_value() -> OfferingTypeDef:
    return {
        "CurrencyCode": ...,
    }


# OfferingTypeDef definition

class OfferingTypeDef(TypedDict):
    CurrencyCode: str,
    Duration: int,
    DurationUnits: DurationUnitsType,  # (1)
    OfferingArn: str,
    OfferingDescription: str,
    PricePerUnit: str,
    PriceUnits: PriceUnitsType,  # (2)
    ResourceSpecification: ResourceSpecificationTypeDef,  # (3)
```

1. See [:material-code-brackets: DurationUnitsType](./literals.md#durationunitstype) 
2. See [:material-code-brackets: PriceUnitsType](./literals.md#priceunitstype) 
3. See [:material-code-braces: ResourceSpecificationTypeDef](./type_defs.md#resourcespecificationtypedef) 
## ReservationTypeDef

```python
# ReservationTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ReservationTypeDef


def get_value() -> ReservationTypeDef:
    return {
        "CurrencyCode": ...,
    }


# ReservationTypeDef definition

class ReservationTypeDef(TypedDict):
    CurrencyCode: str,
    Duration: int,
    DurationUnits: DurationUnitsType,  # (1)
    End: str,
    OfferingArn: str,
    OfferingDescription: str,
    PricePerUnit: str,
    PriceUnits: PriceUnitsType,  # (2)
    ReservationArn: str,
    ReservationName: str,
    ReservationState: ReservationStateType,  # (3)
    ResourceSpecification: ResourceSpecificationTypeDef,  # (4)
    Start: str,
```

1. See [:material-code-brackets: DurationUnitsType](./literals.md#durationunitstype) 
2. See [:material-code-brackets: PriceUnitsType](./literals.md#priceunitstype) 
3. See [:material-code-brackets: ReservationStateType](./literals.md#reservationstatetype) 
4. See [:material-code-braces: ResourceSpecificationTypeDef](./type_defs.md#resourcespecificationtypedef) 
## UpdateBridgeOutputRequestTypeDef

```python
# UpdateBridgeOutputRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateBridgeOutputRequestTypeDef


def get_value() -> UpdateBridgeOutputRequestTypeDef:
    return {
        "BridgeArn": ...,
    }


# UpdateBridgeOutputRequestTypeDef definition

class UpdateBridgeOutputRequestTypeDef(TypedDict):
    BridgeArn: str,
    OutputName: str,
    NetworkOutput: NotRequired[UpdateBridgeNetworkOutputRequestTypeDef],  # (1)
```

1. See [:material-code-braces: UpdateBridgeNetworkOutputRequestTypeDef](./type_defs.md#updatebridgenetworkoutputrequesttypedef) 
## UpdateFlowEntitlementRequestTypeDef

```python
# UpdateFlowEntitlementRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateFlowEntitlementRequestTypeDef


def get_value() -> UpdateFlowEntitlementRequestTypeDef:
    return {
        "EntitlementArn": ...,
    }


# UpdateFlowEntitlementRequestTypeDef definition

class UpdateFlowEntitlementRequestTypeDef(TypedDict):
    EntitlementArn: str,
    FlowArn: str,
    Description: NotRequired[str],
    Encryption: NotRequired[UpdateEncryptionTypeDef],  # (1)
    EntitlementStatus: NotRequired[EntitlementStatusType],  # (2)
    Subscribers: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: UpdateEncryptionTypeDef](./type_defs.md#updateencryptiontypedef) 
2. See [:material-code-brackets: EntitlementStatusType](./literals.md#entitlementstatustype) 
## AddBridgeOutputsRequestTypeDef

```python
# AddBridgeOutputsRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AddBridgeOutputsRequestTypeDef


def get_value() -> AddBridgeOutputsRequestTypeDef:
    return {
        "BridgeArn": ...,
    }


# AddBridgeOutputsRequestTypeDef definition

class AddBridgeOutputsRequestTypeDef(TypedDict):
    BridgeArn: str,
    Outputs: Sequence[AddBridgeOutputRequestTypeDef],  # (1)
```

1. See [:material-code-braces: AddBridgeOutputRequestTypeDef](./type_defs.md#addbridgeoutputrequesttypedef) 
## AddBridgeSourceRequestTypeDef

```python
# AddBridgeSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AddBridgeSourceRequestTypeDef


def get_value() -> AddBridgeSourceRequestTypeDef:
    return {
        "FlowSource": ...,
    }


# AddBridgeSourceRequestTypeDef definition

class AddBridgeSourceRequestTypeDef(TypedDict):
    FlowSource: NotRequired[AddBridgeFlowSourceRequestTypeDef],  # (1)
    NetworkSource: NotRequired[AddBridgeNetworkSourceRequestTypeDef],  # (2)
```

1. See [:material-code-braces: AddBridgeFlowSourceRequestTypeDef](./type_defs.md#addbridgeflowsourcerequesttypedef) 
2. See [:material-code-braces: AddBridgeNetworkSourceRequestTypeDef](./type_defs.md#addbridgenetworksourcerequesttypedef) 
## BridgeSourceTypeDef

```python
# BridgeSourceTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import BridgeSourceTypeDef


def get_value() -> BridgeSourceTypeDef:
    return {
        "FlowSource": ...,
    }


# BridgeSourceTypeDef definition

class BridgeSourceTypeDef(TypedDict):
    FlowSource: NotRequired[BridgeFlowSourceTypeDef],  # (1)
    NetworkSource: NotRequired[BridgeNetworkSourceTypeDef],  # (2)
```

1. See [:material-code-braces: BridgeFlowSourceTypeDef](./type_defs.md#bridgeflowsourcetypedef) 
2. See [:material-code-braces: BridgeNetworkSourceTypeDef](./type_defs.md#bridgenetworksourcetypedef) 
## UpdateBridgeSourceRequestTypeDef

```python
# UpdateBridgeSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateBridgeSourceRequestTypeDef


def get_value() -> UpdateBridgeSourceRequestTypeDef:
    return {
        "BridgeArn": ...,
    }


# UpdateBridgeSourceRequestTypeDef definition

class UpdateBridgeSourceRequestTypeDef(TypedDict):
    BridgeArn: str,
    SourceName: str,
    FlowSource: NotRequired[UpdateBridgeFlowSourceRequestTypeDef],  # (1)
    NetworkSource: NotRequired[UpdateBridgeNetworkSourceRequestTypeDef],  # (2)
```

1. See [:material-code-braces: UpdateBridgeFlowSourceRequestTypeDef](./type_defs.md#updatebridgeflowsourcerequesttypedef) 
2. See [:material-code-braces: UpdateBridgeNetworkSourceRequestTypeDef](./type_defs.md#updatebridgenetworksourcerequesttypedef) 
## GrantFlowEntitlementsResponseTypeDef

```python
# GrantFlowEntitlementsResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import GrantFlowEntitlementsResponseTypeDef


def get_value() -> GrantFlowEntitlementsResponseTypeDef:
    return {
        "Entitlements": ...,
    }


# GrantFlowEntitlementsResponseTypeDef definition

class GrantFlowEntitlementsResponseTypeDef(TypedDict):
    Entitlements: List[EntitlementTypeDef],  # (1)
    FlowArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EntitlementTypeDef](./type_defs.md#entitlementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFlowEntitlementResponseTypeDef

```python
# UpdateFlowEntitlementResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateFlowEntitlementResponseTypeDef


def get_value() -> UpdateFlowEntitlementResponseTypeDef:
    return {
        "Entitlement": ...,
    }


# UpdateFlowEntitlementResponseTypeDef definition

class UpdateFlowEntitlementResponseTypeDef(TypedDict):
    Entitlement: EntitlementTypeDef,  # (1)
    FlowArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EntitlementTypeDef](./type_defs.md#entitlementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GrantFlowEntitlementsRequestTypeDef

```python
# GrantFlowEntitlementsRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import GrantFlowEntitlementsRequestTypeDef


def get_value() -> GrantFlowEntitlementsRequestTypeDef:
    return {
        "Entitlements": ...,
    }


# GrantFlowEntitlementsRequestTypeDef definition

class GrantFlowEntitlementsRequestTypeDef(TypedDict):
    Entitlements: Sequence[GrantEntitlementRequestTypeDef],  # (1)
    FlowArn: str,
```

1. See [:material-code-braces: GrantEntitlementRequestTypeDef](./type_defs.md#grantentitlementrequesttypedef) 
## AddBridgeOutputsResponseTypeDef

```python
# AddBridgeOutputsResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AddBridgeOutputsResponseTypeDef


def get_value() -> AddBridgeOutputsResponseTypeDef:
    return {
        "BridgeArn": ...,
    }


# AddBridgeOutputsResponseTypeDef definition

class AddBridgeOutputsResponseTypeDef(TypedDict):
    BridgeArn: str,
    Outputs: List[BridgeOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BridgeOutputTypeDef](./type_defs.md#bridgeoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBridgeOutputResponseTypeDef

```python
# UpdateBridgeOutputResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateBridgeOutputResponseTypeDef


def get_value() -> UpdateBridgeOutputResponseTypeDef:
    return {
        "BridgeArn": ...,
    }


# UpdateBridgeOutputResponseTypeDef definition

class UpdateBridgeOutputResponseTypeDef(TypedDict):
    BridgeArn: str,
    Output: BridgeOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BridgeOutputTypeDef](./type_defs.md#bridgeoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGatewayInstanceResponseTypeDef

```python
# DescribeGatewayInstanceResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DescribeGatewayInstanceResponseTypeDef


def get_value() -> DescribeGatewayInstanceResponseTypeDef:
    return {
        "GatewayInstance": ...,
    }


# DescribeGatewayInstanceResponseTypeDef definition

class DescribeGatewayInstanceResponseTypeDef(TypedDict):
    GatewayInstance: GatewayInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GatewayInstanceTypeDef](./type_defs.md#gatewayinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFlowSourceThumbnailResponseTypeDef

```python
# DescribeFlowSourceThumbnailResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DescribeFlowSourceThumbnailResponseTypeDef


def get_value() -> DescribeFlowSourceThumbnailResponseTypeDef:
    return {
        "ThumbnailDetails": ...,
    }


# DescribeFlowSourceThumbnailResponseTypeDef definition

class DescribeFlowSourceThumbnailResponseTypeDef(TypedDict):
    ThumbnailDetails: ThumbnailDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThumbnailDetailsTypeDef](./type_defs.md#thumbnaildetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGatewayResponseTypeDef

```python
# CreateGatewayResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import CreateGatewayResponseTypeDef


def get_value() -> CreateGatewayResponseTypeDef:
    return {
        "Gateway": ...,
    }


# CreateGatewayResponseTypeDef definition

class CreateGatewayResponseTypeDef(TypedDict):
    Gateway: GatewayTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GatewayTypeDef](./type_defs.md#gatewaytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGatewayResponseTypeDef

```python
# DescribeGatewayResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DescribeGatewayResponseTypeDef


def get_value() -> DescribeGatewayResponseTypeDef:
    return {
        "Gateway": ...,
    }


# DescribeGatewayResponseTypeDef definition

class DescribeGatewayResponseTypeDef(TypedDict):
    Gateway: GatewayTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GatewayTypeDef](./type_defs.md#gatewaytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MediaStreamOutputConfigurationRequestTypeDef

```python
# MediaStreamOutputConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import MediaStreamOutputConfigurationRequestTypeDef


def get_value() -> MediaStreamOutputConfigurationRequestTypeDef:
    return {
        "DestinationConfigurations": ...,
    }


# MediaStreamOutputConfigurationRequestTypeDef definition

class MediaStreamOutputConfigurationRequestTypeDef(TypedDict):
    EncodingName: EncodingNameType,  # (2)
    MediaStreamName: str,
    DestinationConfigurations: NotRequired[Sequence[DestinationConfigurationRequestTypeDef]],  # (1)
    EncodingParameters: NotRequired[EncodingParametersRequestTypeDef],  # (3)
```

1. See [:material-code-braces: DestinationConfigurationRequestTypeDef](./type_defs.md#destinationconfigurationrequesttypedef) 
2. See [:material-code-brackets: EncodingNameType](./literals.md#encodingnametype) 
3. See [:material-code-braces: EncodingParametersRequestTypeDef](./type_defs.md#encodingparametersrequesttypedef) 
## MediaStreamSourceConfigurationRequestTypeDef

```python
# MediaStreamSourceConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import MediaStreamSourceConfigurationRequestTypeDef


def get_value() -> MediaStreamSourceConfigurationRequestTypeDef:
    return {
        "EncodingName": ...,
    }


# MediaStreamSourceConfigurationRequestTypeDef definition

class MediaStreamSourceConfigurationRequestTypeDef(TypedDict):
    EncodingName: EncodingNameType,  # (1)
    MediaStreamName: str,
    InputConfigurations: NotRequired[Sequence[InputConfigurationRequestTypeDef]],  # (2)
```

1. See [:material-code-brackets: EncodingNameType](./literals.md#encodingnametype) 
2. See [:material-code-braces: InputConfigurationRequestTypeDef](./type_defs.md#inputconfigurationrequesttypedef) 
## MediaStreamOutputConfigurationTypeDef

```python
# MediaStreamOutputConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import MediaStreamOutputConfigurationTypeDef


def get_value() -> MediaStreamOutputConfigurationTypeDef:
    return {
        "DestinationConfigurations": ...,
    }


# MediaStreamOutputConfigurationTypeDef definition

class MediaStreamOutputConfigurationTypeDef(TypedDict):
    EncodingName: EncodingNameType,  # (2)
    MediaStreamName: str,
    DestinationConfigurations: NotRequired[List[DestinationConfigurationTypeDef]],  # (1)
    EncodingParameters: NotRequired[EncodingParametersTypeDef],  # (3)
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
2. See [:material-code-brackets: EncodingNameType](./literals.md#encodingnametype) 
3. See [:material-code-braces: EncodingParametersTypeDef](./type_defs.md#encodingparameterstypedef) 
## MediaStreamSourceConfigurationTypeDef

```python
# MediaStreamSourceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import MediaStreamSourceConfigurationTypeDef


def get_value() -> MediaStreamSourceConfigurationTypeDef:
    return {
        "EncodingName": ...,
    }


# MediaStreamSourceConfigurationTypeDef definition

class MediaStreamSourceConfigurationTypeDef(TypedDict):
    EncodingName: EncodingNameType,  # (1)
    MediaStreamName: str,
    InputConfigurations: NotRequired[List[InputConfigurationTypeDef]],  # (2)
```

1. See [:material-code-brackets: EncodingNameType](./literals.md#encodingnametype) 
2. See [:material-code-braces: InputConfigurationTypeDef](./type_defs.md#inputconfigurationtypedef) 
## UpdateBridgeRequestTypeDef

```python
# UpdateBridgeRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateBridgeRequestTypeDef


def get_value() -> UpdateBridgeRequestTypeDef:
    return {
        "BridgeArn": ...,
    }


# UpdateBridgeRequestTypeDef definition

class UpdateBridgeRequestTypeDef(TypedDict):
    BridgeArn: str,
    EgressGatewayBridge: NotRequired[UpdateEgressGatewayBridgeRequestTypeDef],  # (1)
    IngressGatewayBridge: NotRequired[UpdateIngressGatewayBridgeRequestTypeDef],  # (2)
    SourceFailoverConfig: NotRequired[UpdateFailoverConfigTypeDef],  # (3)
```

1. See [:material-code-braces: UpdateEgressGatewayBridgeRequestTypeDef](./type_defs.md#updateegressgatewaybridgerequesttypedef) 
2. See [:material-code-braces: UpdateIngressGatewayBridgeRequestTypeDef](./type_defs.md#updateingressgatewaybridgerequesttypedef) 
3. See [:material-code-braces: UpdateFailoverConfigTypeDef](./type_defs.md#updatefailoverconfigtypedef) 
## ListFlowsResponseTypeDef

```python
# ListFlowsResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListFlowsResponseTypeDef


def get_value() -> ListFlowsResponseTypeDef:
    return {
        "Flows": ...,
    }


# ListFlowsResponseTypeDef definition

class ListFlowsResponseTypeDef(TypedDict):
    Flows: List[ListedFlowTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListedFlowTypeDef](./type_defs.md#listedflowtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddMediaStreamRequestTypeDef

```python
# AddMediaStreamRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AddMediaStreamRequestTypeDef


def get_value() -> AddMediaStreamRequestTypeDef:
    return {
        "Attributes": ...,
    }


# AddMediaStreamRequestTypeDef definition

class AddMediaStreamRequestTypeDef(TypedDict):
    MediaStreamId: int,
    MediaStreamName: str,
    MediaStreamType: MediaStreamTypeType,  # (2)
    Attributes: NotRequired[MediaStreamAttributesRequestTypeDef],  # (1)
    ClockRate: NotRequired[int],
    Description: NotRequired[str],
    VideoFormat: NotRequired[str],
```

1. See [:material-code-braces: MediaStreamAttributesRequestTypeDef](./type_defs.md#mediastreamattributesrequesttypedef) 
2. See [:material-code-brackets: MediaStreamTypeType](./literals.md#mediastreamtypetype) 
## UpdateFlowMediaStreamRequestTypeDef

```python
# UpdateFlowMediaStreamRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateFlowMediaStreamRequestTypeDef


def get_value() -> UpdateFlowMediaStreamRequestTypeDef:
    return {
        "FlowArn": ...,
    }


# UpdateFlowMediaStreamRequestTypeDef definition

class UpdateFlowMediaStreamRequestTypeDef(TypedDict):
    FlowArn: str,
    MediaStreamName: str,
    Attributes: NotRequired[MediaStreamAttributesRequestTypeDef],  # (1)
    ClockRate: NotRequired[int],
    Description: NotRequired[str],
    MediaStreamType: NotRequired[MediaStreamTypeType],  # (2)
    VideoFormat: NotRequired[str],
```

1. See [:material-code-braces: MediaStreamAttributesRequestTypeDef](./type_defs.md#mediastreamattributesrequesttypedef) 
2. See [:material-code-brackets: MediaStreamTypeType](./literals.md#mediastreamtypetype) 
## MediaStreamTypeDef

```python
# MediaStreamTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import MediaStreamTypeDef


def get_value() -> MediaStreamTypeDef:
    return {
        "Attributes": ...,
    }


# MediaStreamTypeDef definition

class MediaStreamTypeDef(TypedDict):
    Fmt: int,
    MediaStreamId: int,
    MediaStreamName: str,
    MediaStreamType: MediaStreamTypeType,  # (2)
    Attributes: NotRequired[MediaStreamAttributesTypeDef],  # (1)
    ClockRate: NotRequired[int],
    Description: NotRequired[str],
    VideoFormat: NotRequired[str],
```

1. See [:material-code-braces: MediaStreamAttributesTypeDef](./type_defs.md#mediastreamattributestypedef) 
2. See [:material-code-brackets: MediaStreamTypeType](./literals.md#mediastreamtypetype) 
## TransportStreamProgramTypeDef

```python
# TransportStreamProgramTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import TransportStreamProgramTypeDef


def get_value() -> TransportStreamProgramTypeDef:
    return {
        "PcrPid": ...,
    }


# TransportStreamProgramTypeDef definition

class TransportStreamProgramTypeDef(TypedDict):
    PcrPid: int,
    ProgramNumber: int,
    ProgramPid: int,
    Streams: List[TransportStreamTypeDef],  # (1)
    ProgramName: NotRequired[str],
```

1. See [:material-code-braces: TransportStreamTypeDef](./type_defs.md#transportstreamtypedef) 
## MonitoringConfigOutputTypeDef

```python
# MonitoringConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import MonitoringConfigOutputTypeDef


def get_value() -> MonitoringConfigOutputTypeDef:
    return {
        "ThumbnailState": ...,
    }


# MonitoringConfigOutputTypeDef definition

class MonitoringConfigOutputTypeDef(TypedDict):
    ThumbnailState: NotRequired[ThumbnailStateType],  # (1)
    AudioMonitoringSettings: NotRequired[List[AudioMonitoringSettingTypeDef]],  # (2)
    ContentQualityAnalysisState: NotRequired[ContentQualityAnalysisStateType],  # (3)
    VideoMonitoringSettings: NotRequired[List[VideoMonitoringSettingTypeDef]],  # (4)
```

1. See [:material-code-brackets: ThumbnailStateType](./literals.md#thumbnailstatetype) 
2. See [:material-code-braces: AudioMonitoringSettingTypeDef](./type_defs.md#audiomonitoringsettingtypedef) 
3. See [:material-code-brackets: ContentQualityAnalysisStateType](./literals.md#contentqualityanalysisstatetype) 
4. See [:material-code-braces: VideoMonitoringSettingTypeDef](./type_defs.md#videomonitoringsettingtypedef) 
## MonitoringConfigTypeDef

```python
# MonitoringConfigTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import MonitoringConfigTypeDef


def get_value() -> MonitoringConfigTypeDef:
    return {
        "ThumbnailState": ...,
    }


# MonitoringConfigTypeDef definition

class MonitoringConfigTypeDef(TypedDict):
    ThumbnailState: NotRequired[ThumbnailStateType],  # (1)
    AudioMonitoringSettings: NotRequired[Sequence[AudioMonitoringSettingTypeDef]],  # (2)
    ContentQualityAnalysisState: NotRequired[ContentQualityAnalysisStateType],  # (3)
    VideoMonitoringSettings: NotRequired[Sequence[VideoMonitoringSettingTypeDef]],  # (4)
```

1. See [:material-code-brackets: ThumbnailStateType](./literals.md#thumbnailstatetype) 
2. See [:material-code-braces: AudioMonitoringSettingTypeDef](./type_defs.md#audiomonitoringsettingtypedef) 
3. See [:material-code-brackets: ContentQualityAnalysisStateType](./literals.md#contentqualityanalysisstatetype) 
4. See [:material-code-braces: VideoMonitoringSettingTypeDef](./type_defs.md#videomonitoringsettingtypedef) 
## DescribeOfferingResponseTypeDef

```python
# DescribeOfferingResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DescribeOfferingResponseTypeDef


def get_value() -> DescribeOfferingResponseTypeDef:
    return {
        "Offering": ...,
    }


# DescribeOfferingResponseTypeDef definition

class DescribeOfferingResponseTypeDef(TypedDict):
    Offering: OfferingTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OfferingTypeDef](./type_defs.md#offeringtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOfferingsResponseTypeDef

```python
# ListOfferingsResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListOfferingsResponseTypeDef


def get_value() -> ListOfferingsResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListOfferingsResponseTypeDef definition

class ListOfferingsResponseTypeDef(TypedDict):
    Offerings: List[OfferingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OfferingTypeDef](./type_defs.md#offeringtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeReservationResponseTypeDef

```python
# DescribeReservationResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DescribeReservationResponseTypeDef


def get_value() -> DescribeReservationResponseTypeDef:
    return {
        "Reservation": ...,
    }


# DescribeReservationResponseTypeDef definition

class DescribeReservationResponseTypeDef(TypedDict):
    Reservation: ReservationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservationTypeDef](./type_defs.md#reservationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReservationsResponseTypeDef

```python
# ListReservationsResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import ListReservationsResponseTypeDef


def get_value() -> ListReservationsResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListReservationsResponseTypeDef definition

class ListReservationsResponseTypeDef(TypedDict):
    Reservations: List[ReservationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ReservationTypeDef](./type_defs.md#reservationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PurchaseOfferingResponseTypeDef

```python
# PurchaseOfferingResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import PurchaseOfferingResponseTypeDef


def get_value() -> PurchaseOfferingResponseTypeDef:
    return {
        "Reservation": ...,
    }


# PurchaseOfferingResponseTypeDef definition

class PurchaseOfferingResponseTypeDef(TypedDict):
    Reservation: ReservationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservationTypeDef](./type_defs.md#reservationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddBridgeSourcesRequestTypeDef

```python
# AddBridgeSourcesRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AddBridgeSourcesRequestTypeDef


def get_value() -> AddBridgeSourcesRequestTypeDef:
    return {
        "BridgeArn": ...,
    }


# AddBridgeSourcesRequestTypeDef definition

class AddBridgeSourcesRequestTypeDef(TypedDict):
    BridgeArn: str,
    Sources: Sequence[AddBridgeSourceRequestTypeDef],  # (1)
```

1. See [:material-code-braces: AddBridgeSourceRequestTypeDef](./type_defs.md#addbridgesourcerequesttypedef) 
## CreateBridgeRequestTypeDef

```python
# CreateBridgeRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import CreateBridgeRequestTypeDef


def get_value() -> CreateBridgeRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateBridgeRequestTypeDef definition

class CreateBridgeRequestTypeDef(TypedDict):
    Name: str,
    PlacementArn: str,
    Sources: Sequence[AddBridgeSourceRequestTypeDef],  # (1)
    EgressGatewayBridge: NotRequired[AddEgressGatewayBridgeRequestTypeDef],  # (2)
    IngressGatewayBridge: NotRequired[AddIngressGatewayBridgeRequestTypeDef],  # (3)
    Outputs: NotRequired[Sequence[AddBridgeOutputRequestTypeDef]],  # (4)
    SourceFailoverConfig: NotRequired[FailoverConfigTypeDef],  # (5)
```

1. See [:material-code-braces: AddBridgeSourceRequestTypeDef](./type_defs.md#addbridgesourcerequesttypedef) 
2. See [:material-code-braces: AddEgressGatewayBridgeRequestTypeDef](./type_defs.md#addegressgatewaybridgerequesttypedef) 
3. See [:material-code-braces: AddIngressGatewayBridgeRequestTypeDef](./type_defs.md#addingressgatewaybridgerequesttypedef) 
4. See [:material-code-braces: AddBridgeOutputRequestTypeDef](./type_defs.md#addbridgeoutputrequesttypedef) 
5. See [:material-code-braces: FailoverConfigTypeDef](./type_defs.md#failoverconfigtypedef) 
## AddBridgeSourcesResponseTypeDef

```python
# AddBridgeSourcesResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AddBridgeSourcesResponseTypeDef


def get_value() -> AddBridgeSourcesResponseTypeDef:
    return {
        "BridgeArn": ...,
    }


# AddBridgeSourcesResponseTypeDef definition

class AddBridgeSourcesResponseTypeDef(TypedDict):
    BridgeArn: str,
    Sources: List[BridgeSourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BridgeSourceTypeDef](./type_defs.md#bridgesourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BridgeTypeDef

```python
# BridgeTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import BridgeTypeDef


def get_value() -> BridgeTypeDef:
    return {
        "BridgeArn": ...,
    }


# BridgeTypeDef definition

class BridgeTypeDef(TypedDict):
    BridgeArn: str,
    BridgeState: BridgeStateType,  # (2)
    Name: str,
    PlacementArn: str,
    BridgeMessages: NotRequired[List[MessageDetailTypeDef]],  # (1)
    EgressGatewayBridge: NotRequired[EgressGatewayBridgeTypeDef],  # (3)
    IngressGatewayBridge: NotRequired[IngressGatewayBridgeTypeDef],  # (4)
    Outputs: NotRequired[List[BridgeOutputTypeDef]],  # (5)
    SourceFailoverConfig: NotRequired[FailoverConfigTypeDef],  # (6)
    Sources: NotRequired[List[BridgeSourceTypeDef]],  # (7)
```

1. See [:material-code-braces: MessageDetailTypeDef](./type_defs.md#messagedetailtypedef) 
2. See [:material-code-brackets: BridgeStateType](./literals.md#bridgestatetype) 
3. See [:material-code-braces: EgressGatewayBridgeTypeDef](./type_defs.md#egressgatewaybridgetypedef) 
4. See [:material-code-braces: IngressGatewayBridgeTypeDef](./type_defs.md#ingressgatewaybridgetypedef) 
5. See [:material-code-braces: BridgeOutputTypeDef](./type_defs.md#bridgeoutputtypedef) 
6. See [:material-code-braces: FailoverConfigTypeDef](./type_defs.md#failoverconfigtypedef) 
7. See [:material-code-braces: BridgeSourceTypeDef](./type_defs.md#bridgesourcetypedef) 
## UpdateBridgeSourceResponseTypeDef

```python
# UpdateBridgeSourceResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateBridgeSourceResponseTypeDef


def get_value() -> UpdateBridgeSourceResponseTypeDef:
    return {
        "BridgeArn": ...,
    }


# UpdateBridgeSourceResponseTypeDef definition

class UpdateBridgeSourceResponseTypeDef(TypedDict):
    BridgeArn: str,
    Source: BridgeSourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BridgeSourceTypeDef](./type_defs.md#bridgesourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddOutputRequestTypeDef

```python
# AddOutputRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AddOutputRequestTypeDef


def get_value() -> AddOutputRequestTypeDef:
    return {
        "CidrAllowList": ...,
    }


# AddOutputRequestTypeDef definition

class AddOutputRequestTypeDef(TypedDict):
    Protocol: ProtocolType,  # (3)
    CidrAllowList: NotRequired[Sequence[str]],
    Description: NotRequired[str],
    Destination: NotRequired[str],
    Encryption: NotRequired[EncryptionTypeDef],  # (1)
    MaxLatency: NotRequired[int],
    MediaStreamOutputConfigurations: NotRequired[Sequence[MediaStreamOutputConfigurationRequestTypeDef]],  # (2)
    MinLatency: NotRequired[int],
    Name: NotRequired[str],
    Port: NotRequired[int],
    RemoteId: NotRequired[str],
    SenderControlPort: NotRequired[int],
    SmoothingLatency: NotRequired[int],
    StreamId: NotRequired[str],
    VpcInterfaceAttachment: NotRequired[VpcInterfaceAttachmentTypeDef],  # (4)
    OutputStatus: NotRequired[OutputStatusType],  # (5)
```

1. See [:material-code-braces: EncryptionTypeDef](./type_defs.md#encryptiontypedef) 
2. See [:material-code-braces: MediaStreamOutputConfigurationRequestTypeDef](./type_defs.md#mediastreamoutputconfigurationrequesttypedef) 
3. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
4. See [:material-code-braces: VpcInterfaceAttachmentTypeDef](./type_defs.md#vpcinterfaceattachmenttypedef) 
5. See [:material-code-brackets: OutputStatusType](./literals.md#outputstatustype) 
## UpdateFlowOutputRequestTypeDef

```python
# UpdateFlowOutputRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateFlowOutputRequestTypeDef


def get_value() -> UpdateFlowOutputRequestTypeDef:
    return {
        "FlowArn": ...,
    }


# UpdateFlowOutputRequestTypeDef definition

class UpdateFlowOutputRequestTypeDef(TypedDict):
    FlowArn: str,
    OutputArn: str,
    CidrAllowList: NotRequired[Sequence[str]],
    Description: NotRequired[str],
    Destination: NotRequired[str],
    Encryption: NotRequired[UpdateEncryptionTypeDef],  # (1)
    MaxLatency: NotRequired[int],
    MediaStreamOutputConfigurations: NotRequired[Sequence[MediaStreamOutputConfigurationRequestTypeDef]],  # (2)
    MinLatency: NotRequired[int],
    Port: NotRequired[int],
    Protocol: NotRequired[ProtocolType],  # (3)
    RemoteId: NotRequired[str],
    SenderControlPort: NotRequired[int],
    SenderIpAddress: NotRequired[str],
    SmoothingLatency: NotRequired[int],
    StreamId: NotRequired[str],
    VpcInterfaceAttachment: NotRequired[VpcInterfaceAttachmentTypeDef],  # (4)
    OutputStatus: NotRequired[OutputStatusType],  # (5)
```

1. See [:material-code-braces: UpdateEncryptionTypeDef](./type_defs.md#updateencryptiontypedef) 
2. See [:material-code-braces: MediaStreamOutputConfigurationRequestTypeDef](./type_defs.md#mediastreamoutputconfigurationrequesttypedef) 
3. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
4. See [:material-code-braces: VpcInterfaceAttachmentTypeDef](./type_defs.md#vpcinterfaceattachmenttypedef) 
5. See [:material-code-brackets: OutputStatusType](./literals.md#outputstatustype) 
## SetSourceRequestTypeDef

```python
# SetSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import SetSourceRequestTypeDef


def get_value() -> SetSourceRequestTypeDef:
    return {
        "Decryption": ...,
    }


# SetSourceRequestTypeDef definition

class SetSourceRequestTypeDef(TypedDict):
    Decryption: NotRequired[EncryptionTypeDef],  # (1)
    Description: NotRequired[str],
    EntitlementArn: NotRequired[str],
    IngestPort: NotRequired[int],
    MaxBitrate: NotRequired[int],
    MaxLatency: NotRequired[int],
    MaxSyncBuffer: NotRequired[int],
    MediaStreamSourceConfigurations: NotRequired[Sequence[MediaStreamSourceConfigurationRequestTypeDef]],  # (2)
    MinLatency: NotRequired[int],
    Name: NotRequired[str],
    Protocol: NotRequired[ProtocolType],  # (3)
    SenderControlPort: NotRequired[int],
    SenderIpAddress: NotRequired[str],
    SourceListenerAddress: NotRequired[str],
    SourceListenerPort: NotRequired[int],
    StreamId: NotRequired[str],
    VpcInterfaceName: NotRequired[str],
    WhitelistCidr: NotRequired[str],
    GatewayBridgeSource: NotRequired[SetGatewayBridgeSourceRequestTypeDef],  # (4)
```

1. See [:material-code-braces: EncryptionTypeDef](./type_defs.md#encryptiontypedef) 
2. See [:material-code-braces: MediaStreamSourceConfigurationRequestTypeDef](./type_defs.md#mediastreamsourceconfigurationrequesttypedef) 
3. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
4. See [:material-code-braces: SetGatewayBridgeSourceRequestTypeDef](./type_defs.md#setgatewaybridgesourcerequesttypedef) 
## UpdateFlowSourceRequestTypeDef

```python
# UpdateFlowSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateFlowSourceRequestTypeDef


def get_value() -> UpdateFlowSourceRequestTypeDef:
    return {
        "FlowArn": ...,
    }


# UpdateFlowSourceRequestTypeDef definition

class UpdateFlowSourceRequestTypeDef(TypedDict):
    FlowArn: str,
    SourceArn: str,
    Decryption: NotRequired[UpdateEncryptionTypeDef],  # (1)
    Description: NotRequired[str],
    EntitlementArn: NotRequired[str],
    IngestPort: NotRequired[int],
    MaxBitrate: NotRequired[int],
    MaxLatency: NotRequired[int],
    MaxSyncBuffer: NotRequired[int],
    MediaStreamSourceConfigurations: NotRequired[Sequence[MediaStreamSourceConfigurationRequestTypeDef]],  # (2)
    MinLatency: NotRequired[int],
    Protocol: NotRequired[ProtocolType],  # (3)
    SenderControlPort: NotRequired[int],
    SenderIpAddress: NotRequired[str],
    SourceListenerAddress: NotRequired[str],
    SourceListenerPort: NotRequired[int],
    StreamId: NotRequired[str],
    VpcInterfaceName: NotRequired[str],
    WhitelistCidr: NotRequired[str],
    GatewayBridgeSource: NotRequired[UpdateGatewayBridgeSourceRequestTypeDef],  # (4)
```

1. See [:material-code-braces: UpdateEncryptionTypeDef](./type_defs.md#updateencryptiontypedef) 
2. See [:material-code-braces: MediaStreamSourceConfigurationRequestTypeDef](./type_defs.md#mediastreamsourceconfigurationrequesttypedef) 
3. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
4. See [:material-code-braces: UpdateGatewayBridgeSourceRequestTypeDef](./type_defs.md#updategatewaybridgesourcerequesttypedef) 
## OutputTypeDef

```python
# OutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import OutputTypeDef


def get_value() -> OutputTypeDef:
    return {
        "DataTransferSubscriberFeePercent": ...,
    }


# OutputTypeDef definition

class OutputTypeDef(TypedDict):
    Name: str,
    OutputArn: str,
    DataTransferSubscriberFeePercent: NotRequired[int],
    Description: NotRequired[str],
    Destination: NotRequired[str],
    Encryption: NotRequired[EncryptionTypeDef],  # (1)
    EntitlementArn: NotRequired[str],
    ListenerAddress: NotRequired[str],
    MediaLiveInputArn: NotRequired[str],
    MediaStreamOutputConfigurations: NotRequired[List[MediaStreamOutputConfigurationTypeDef]],  # (2)
    Port: NotRequired[int],
    Transport: NotRequired[TransportTypeDef],  # (3)
    VpcInterfaceAttachment: NotRequired[VpcInterfaceAttachmentTypeDef],  # (4)
    BridgeArn: NotRequired[str],
    BridgePorts: NotRequired[List[int]],
    OutputStatus: NotRequired[OutputStatusType],  # (5)
```

1. See [:material-code-braces: EncryptionTypeDef](./type_defs.md#encryptiontypedef) 
2. See [:material-code-braces: MediaStreamOutputConfigurationTypeDef](./type_defs.md#mediastreamoutputconfigurationtypedef) 
3. See [:material-code-braces: TransportTypeDef](./type_defs.md#transporttypedef) 
4. See [:material-code-braces: VpcInterfaceAttachmentTypeDef](./type_defs.md#vpcinterfaceattachmenttypedef) 
5. See [:material-code-brackets: OutputStatusType](./literals.md#outputstatustype) 
## SourceTypeDef

```python
# SourceTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import SourceTypeDef


def get_value() -> SourceTypeDef:
    return {
        "DataTransferSubscriberFeePercent": ...,
    }


# SourceTypeDef definition

class SourceTypeDef(TypedDict):
    Name: str,
    SourceArn: str,
    DataTransferSubscriberFeePercent: NotRequired[int],
    Decryption: NotRequired[EncryptionTypeDef],  # (1)
    Description: NotRequired[str],
    EntitlementArn: NotRequired[str],
    IngestIp: NotRequired[str],
    IngestPort: NotRequired[int],
    MediaStreamSourceConfigurations: NotRequired[List[MediaStreamSourceConfigurationTypeDef]],  # (2)
    SenderControlPort: NotRequired[int],
    SenderIpAddress: NotRequired[str],
    Transport: NotRequired[TransportTypeDef],  # (3)
    VpcInterfaceName: NotRequired[str],
    WhitelistCidr: NotRequired[str],
    GatewayBridgeSource: NotRequired[GatewayBridgeSourceTypeDef],  # (4)
```

1. See [:material-code-braces: EncryptionTypeDef](./type_defs.md#encryptiontypedef) 
2. See [:material-code-braces: MediaStreamSourceConfigurationTypeDef](./type_defs.md#mediastreamsourceconfigurationtypedef) 
3. See [:material-code-braces: TransportTypeDef](./type_defs.md#transporttypedef) 
4. See [:material-code-braces: GatewayBridgeSourceTypeDef](./type_defs.md#gatewaybridgesourcetypedef) 
## AddFlowMediaStreamsRequestTypeDef

```python
# AddFlowMediaStreamsRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AddFlowMediaStreamsRequestTypeDef


def get_value() -> AddFlowMediaStreamsRequestTypeDef:
    return {
        "FlowArn": ...,
    }


# AddFlowMediaStreamsRequestTypeDef definition

class AddFlowMediaStreamsRequestTypeDef(TypedDict):
    FlowArn: str,
    MediaStreams: Sequence[AddMediaStreamRequestTypeDef],  # (1)
```

1. See [:material-code-braces: AddMediaStreamRequestTypeDef](./type_defs.md#addmediastreamrequesttypedef) 
## AddFlowMediaStreamsResponseTypeDef

```python
# AddFlowMediaStreamsResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AddFlowMediaStreamsResponseTypeDef


def get_value() -> AddFlowMediaStreamsResponseTypeDef:
    return {
        "FlowArn": ...,
    }


# AddFlowMediaStreamsResponseTypeDef definition

class AddFlowMediaStreamsResponseTypeDef(TypedDict):
    FlowArn: str,
    MediaStreams: List[MediaStreamTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MediaStreamTypeDef](./type_defs.md#mediastreamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFlowMediaStreamResponseTypeDef

```python
# UpdateFlowMediaStreamResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateFlowMediaStreamResponseTypeDef


def get_value() -> UpdateFlowMediaStreamResponseTypeDef:
    return {
        "FlowArn": ...,
    }


# UpdateFlowMediaStreamResponseTypeDef definition

class UpdateFlowMediaStreamResponseTypeDef(TypedDict):
    FlowArn: str,
    MediaStream: MediaStreamTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MediaStreamTypeDef](./type_defs.md#mediastreamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TransportMediaInfoTypeDef

```python
# TransportMediaInfoTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import TransportMediaInfoTypeDef


def get_value() -> TransportMediaInfoTypeDef:
    return {
        "Programs": ...,
    }


# TransportMediaInfoTypeDef definition

class TransportMediaInfoTypeDef(TypedDict):
    Programs: List[TransportStreamProgramTypeDef],  # (1)
```

1. See [:material-code-braces: TransportStreamProgramTypeDef](./type_defs.md#transportstreamprogramtypedef) 
## CreateBridgeResponseTypeDef

```python
# CreateBridgeResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import CreateBridgeResponseTypeDef


def get_value() -> CreateBridgeResponseTypeDef:
    return {
        "Bridge": ...,
    }


# CreateBridgeResponseTypeDef definition

class CreateBridgeResponseTypeDef(TypedDict):
    Bridge: BridgeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BridgeTypeDef](./type_defs.md#bridgetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBridgeResponseTypeDef

```python
# DescribeBridgeResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DescribeBridgeResponseTypeDef


def get_value() -> DescribeBridgeResponseTypeDef:
    return {
        "Bridge": ...,
    }


# DescribeBridgeResponseTypeDef definition

class DescribeBridgeResponseTypeDef(TypedDict):
    Bridge: BridgeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BridgeTypeDef](./type_defs.md#bridgetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBridgeResponseTypeDef

```python
# UpdateBridgeResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateBridgeResponseTypeDef


def get_value() -> UpdateBridgeResponseTypeDef:
    return {
        "Bridge": ...,
    }


# UpdateBridgeResponseTypeDef definition

class UpdateBridgeResponseTypeDef(TypedDict):
    Bridge: BridgeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BridgeTypeDef](./type_defs.md#bridgetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddFlowOutputsRequestTypeDef

```python
# AddFlowOutputsRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AddFlowOutputsRequestTypeDef


def get_value() -> AddFlowOutputsRequestTypeDef:
    return {
        "FlowArn": ...,
    }


# AddFlowOutputsRequestTypeDef definition

class AddFlowOutputsRequestTypeDef(TypedDict):
    FlowArn: str,
    Outputs: Sequence[AddOutputRequestTypeDef],  # (1)
```

1. See [:material-code-braces: AddOutputRequestTypeDef](./type_defs.md#addoutputrequesttypedef) 
## AddFlowSourcesRequestTypeDef

```python
# AddFlowSourcesRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AddFlowSourcesRequestTypeDef


def get_value() -> AddFlowSourcesRequestTypeDef:
    return {
        "FlowArn": ...,
    }


# AddFlowSourcesRequestTypeDef definition

class AddFlowSourcesRequestTypeDef(TypedDict):
    FlowArn: str,
    Sources: Sequence[SetSourceRequestTypeDef],  # (1)
```

1. See [:material-code-braces: SetSourceRequestTypeDef](./type_defs.md#setsourcerequesttypedef) 
## AddFlowOutputsResponseTypeDef

```python
# AddFlowOutputsResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AddFlowOutputsResponseTypeDef


def get_value() -> AddFlowOutputsResponseTypeDef:
    return {
        "FlowArn": ...,
    }


# AddFlowOutputsResponseTypeDef definition

class AddFlowOutputsResponseTypeDef(TypedDict):
    FlowArn: str,
    Outputs: List[OutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OutputTypeDef](./type_defs.md#outputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFlowOutputResponseTypeDef

```python
# UpdateFlowOutputResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateFlowOutputResponseTypeDef


def get_value() -> UpdateFlowOutputResponseTypeDef:
    return {
        "FlowArn": ...,
    }


# UpdateFlowOutputResponseTypeDef definition

class UpdateFlowOutputResponseTypeDef(TypedDict):
    FlowArn: str,
    Output: OutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OutputTypeDef](./type_defs.md#outputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddFlowSourcesResponseTypeDef

```python
# AddFlowSourcesResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import AddFlowSourcesResponseTypeDef


def get_value() -> AddFlowSourcesResponseTypeDef:
    return {
        "FlowArn": ...,
    }


# AddFlowSourcesResponseTypeDef definition

class AddFlowSourcesResponseTypeDef(TypedDict):
    FlowArn: str,
    Sources: List[SourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FlowTypeDef

```python
# FlowTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import FlowTypeDef


def get_value() -> FlowTypeDef:
    return {
        "AvailabilityZone": ...,
    }


# FlowTypeDef definition

class FlowTypeDef(TypedDict):
    AvailabilityZone: str,
    Entitlements: List[EntitlementTypeDef],  # (1)
    FlowArn: str,
    Name: str,
    Outputs: List[OutputTypeDef],  # (3)
    Source: SourceTypeDef,  # (4)
    Status: StatusType,  # (7)
    Description: NotRequired[str],
    EgressIp: NotRequired[str],
    MediaStreams: NotRequired[List[MediaStreamTypeDef]],  # (2)
    SourceFailoverConfig: NotRequired[FailoverConfigTypeDef],  # (5)
    Sources: NotRequired[List[SourceTypeDef]],  # (6)
    VpcInterfaces: NotRequired[List[VpcInterfaceTypeDef]],  # (8)
    Maintenance: NotRequired[MaintenanceTypeDef],  # (9)
    SourceMonitoringConfig: NotRequired[MonitoringConfigOutputTypeDef],  # (10)
```

1. See [:material-code-braces: EntitlementTypeDef](./type_defs.md#entitlementtypedef) 
2. See [:material-code-braces: MediaStreamTypeDef](./type_defs.md#mediastreamtypedef) 
3. See [:material-code-braces: OutputTypeDef](./type_defs.md#outputtypedef) 
4. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
5. See [:material-code-braces: FailoverConfigTypeDef](./type_defs.md#failoverconfigtypedef) 
6. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
7. See [:material-code-brackets: StatusType](./literals.md#statustype) 
8. See [:material-code-braces: VpcInterfaceTypeDef](./type_defs.md#vpcinterfacetypedef) 
9. See [:material-code-braces: MaintenanceTypeDef](./type_defs.md#maintenancetypedef) 
10. See [:material-code-braces: MonitoringConfigOutputTypeDef](./type_defs.md#monitoringconfigoutputtypedef) 
## UpdateFlowSourceResponseTypeDef

```python
# UpdateFlowSourceResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateFlowSourceResponseTypeDef


def get_value() -> UpdateFlowSourceResponseTypeDef:
    return {
        "FlowArn": ...,
    }


# UpdateFlowSourceResponseTypeDef definition

class UpdateFlowSourceResponseTypeDef(TypedDict):
    FlowArn: str,
    Source: SourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFlowSourceMetadataResponseTypeDef

```python
# DescribeFlowSourceMetadataResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DescribeFlowSourceMetadataResponseTypeDef


def get_value() -> DescribeFlowSourceMetadataResponseTypeDef:
    return {
        "FlowArn": ...,
    }


# DescribeFlowSourceMetadataResponseTypeDef definition

class DescribeFlowSourceMetadataResponseTypeDef(TypedDict):
    FlowArn: str,
    Messages: List[MessageDetailTypeDef],  # (1)
    Timestamp: datetime,
    TransportMediaInfo: TransportMediaInfoTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MessageDetailTypeDef](./type_defs.md#messagedetailtypedef) 
2. See [:material-code-braces: TransportMediaInfoTypeDef](./type_defs.md#transportmediainfotypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFlowRequestTypeDef

```python
# CreateFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import CreateFlowRequestTypeDef


def get_value() -> CreateFlowRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateFlowRequestTypeDef definition

class CreateFlowRequestTypeDef(TypedDict):
    Name: str,
    AvailabilityZone: NotRequired[str],
    Entitlements: NotRequired[Sequence[GrantEntitlementRequestTypeDef]],  # (1)
    MediaStreams: NotRequired[Sequence[AddMediaStreamRequestTypeDef]],  # (2)
    Outputs: NotRequired[Sequence[AddOutputRequestTypeDef]],  # (3)
    Source: NotRequired[SetSourceRequestTypeDef],  # (4)
    SourceFailoverConfig: NotRequired[FailoverConfigTypeDef],  # (5)
    Sources: NotRequired[Sequence[SetSourceRequestTypeDef]],  # (6)
    VpcInterfaces: NotRequired[Sequence[VpcInterfaceRequestTypeDef]],  # (7)
    Maintenance: NotRequired[AddMaintenanceTypeDef],  # (8)
    SourceMonitoringConfig: NotRequired[MonitoringConfigUnionTypeDef],  # (9)
```

1. See [:material-code-braces: GrantEntitlementRequestTypeDef](./type_defs.md#grantentitlementrequesttypedef) 
2. See [:material-code-braces: AddMediaStreamRequestTypeDef](./type_defs.md#addmediastreamrequesttypedef) 
3. See [:material-code-braces: AddOutputRequestTypeDef](./type_defs.md#addoutputrequesttypedef) 
4. See [:material-code-braces: SetSourceRequestTypeDef](./type_defs.md#setsourcerequesttypedef) 
5. See [:material-code-braces: FailoverConfigTypeDef](./type_defs.md#failoverconfigtypedef) 
6. See [:material-code-braces: SetSourceRequestTypeDef](./type_defs.md#setsourcerequesttypedef) 
7. See [:material-code-braces: VpcInterfaceRequestTypeDef](./type_defs.md#vpcinterfacerequesttypedef) 
8. See [:material-code-braces: AddMaintenanceTypeDef](./type_defs.md#addmaintenancetypedef) 
9. See [:material-code-braces: MonitoringConfigTypeDef](./type_defs.md#monitoringconfigtypedef) [:material-code-braces: MonitoringConfigOutputTypeDef](./type_defs.md#monitoringconfigoutputtypedef) 
## UpdateFlowRequestTypeDef

```python
# UpdateFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateFlowRequestTypeDef


def get_value() -> UpdateFlowRequestTypeDef:
    return {
        "FlowArn": ...,
    }


# UpdateFlowRequestTypeDef definition

class UpdateFlowRequestTypeDef(TypedDict):
    FlowArn: str,
    SourceFailoverConfig: NotRequired[UpdateFailoverConfigTypeDef],  # (1)
    Maintenance: NotRequired[UpdateMaintenanceTypeDef],  # (2)
    SourceMonitoringConfig: NotRequired[MonitoringConfigUnionTypeDef],  # (3)
```

1. See [:material-code-braces: UpdateFailoverConfigTypeDef](./type_defs.md#updatefailoverconfigtypedef) 
2. See [:material-code-braces: UpdateMaintenanceTypeDef](./type_defs.md#updatemaintenancetypedef) 
3. See [:material-code-braces: MonitoringConfigTypeDef](./type_defs.md#monitoringconfigtypedef) [:material-code-braces: MonitoringConfigOutputTypeDef](./type_defs.md#monitoringconfigoutputtypedef) 
## CreateFlowResponseTypeDef

```python
# CreateFlowResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import CreateFlowResponseTypeDef


def get_value() -> CreateFlowResponseTypeDef:
    return {
        "Flow": ...,
    }


# CreateFlowResponseTypeDef definition

class CreateFlowResponseTypeDef(TypedDict):
    Flow: FlowTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlowTypeDef](./type_defs.md#flowtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFlowResponseTypeDef

```python
# DescribeFlowResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import DescribeFlowResponseTypeDef


def get_value() -> DescribeFlowResponseTypeDef:
    return {
        "Flow": ...,
    }


# DescribeFlowResponseTypeDef definition

class DescribeFlowResponseTypeDef(TypedDict):
    Flow: FlowTypeDef,  # (1)
    Messages: MessagesTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FlowTypeDef](./type_defs.md#flowtypedef) 
2. See [:material-code-braces: MessagesTypeDef](./type_defs.md#messagestypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFlowResponseTypeDef

```python
# UpdateFlowResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconnect.type_defs import UpdateFlowResponseTypeDef


def get_value() -> UpdateFlowResponseTypeDef:
    return {
        "Flow": ...,
    }


# UpdateFlowResponseTypeDef definition

class UpdateFlowResponseTypeDef(TypedDict):
    Flow: FlowTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlowTypeDef](./type_defs.md#flowtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
