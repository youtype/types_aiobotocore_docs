# Type definitions

> [Index](../README.md) > [MediaConnect](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MediaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
    type annotations stubs module [types-aiobotocore-mediaconnect](https://pypi.org/project/types-aiobotocore-mediaconnect/).



## VpcInterfaceAttachmentTypeDef

```python
# VpcInterfaceAttachmentTypeDef definition

class VpcInterfaceAttachmentTypeDef(TypedDict):
    VpcInterfaceName: NotRequired[str],
```

## AddBridgeNetworkOutputRequestTypeDef

```python
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
## AddBridgeNetworkSourceRequestTypeDef

```python
# AddBridgeNetworkSourceRequestTypeDef definition

class AddBridgeNetworkSourceRequestTypeDef(TypedDict):
    MulticastIp: str,
    Name: str,
    NetworkName: str,
    Port: int,
    Protocol: ProtocolType,  # (1)
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
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

## AddEgressGatewayBridgeRequestTypeDef

```python
# AddEgressGatewayBridgeRequestTypeDef definition

class AddEgressGatewayBridgeRequestTypeDef(TypedDict):
    MaxBitrate: int,
```

## VpcInterfaceRequestTypeDef

```python
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
# AddIngressGatewayBridgeRequestTypeDef definition

class AddIngressGatewayBridgeRequestTypeDef(TypedDict):
    MaxBitrate: int,
    MaxOutputs: int,
```

## AddMaintenanceTypeDef

```python
# AddMaintenanceTypeDef definition

class AddMaintenanceTypeDef(TypedDict):
    MaintenanceDay: MaintenanceDayType,  # (1)
    MaintenanceStartHour: str,
```

1. See [:material-code-brackets: MaintenanceDayType](./literals.md#maintenancedaytype) 
## EncryptionTypeDef

```python
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
## BridgeFlowOutputTypeDef

```python
# BridgeFlowOutputTypeDef definition

class BridgeFlowOutputTypeDef(TypedDict):
    FlowArn: str,
    FlowSourceArn: str,
    Name: str,
```

## BridgeNetworkOutputTypeDef

```python
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
## BridgeNetworkSourceTypeDef

```python
# BridgeNetworkSourceTypeDef definition

class BridgeNetworkSourceTypeDef(TypedDict):
    MulticastIp: str,
    Name: str,
    NetworkName: str,
    Port: int,
    Protocol: ProtocolType,  # (1)
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
## EgressGatewayBridgeTypeDef

```python
# EgressGatewayBridgeTypeDef definition

class EgressGatewayBridgeTypeDef(TypedDict):
    MaxBitrate: int,
    InstanceId: NotRequired[str],
```

## IngressGatewayBridgeTypeDef

```python
# IngressGatewayBridgeTypeDef definition

class IngressGatewayBridgeTypeDef(TypedDict):
    MaxBitrate: int,
    MaxOutputs: int,
    InstanceId: NotRequired[str],
```

## MessageDetailTypeDef

```python
# MessageDetailTypeDef definition

class MessageDetailTypeDef(TypedDict):
    Code: str,
    Message: str,
    ResourceName: NotRequired[str],
```

## MonitoringConfigTypeDef

```python
# MonitoringConfigTypeDef definition

class MonitoringConfigTypeDef(TypedDict):
    ThumbnailState: NotRequired[ThumbnailStateType],  # (1)
```

1. See [:material-code-brackets: ThumbnailStateType](./literals.md#thumbnailstatetype) 
## GatewayNetworkTypeDef

```python
# GatewayNetworkTypeDef definition

class GatewayNetworkTypeDef(TypedDict):
    CidrBlock: str,
    Name: str,
```

## DeleteBridgeRequestRequestTypeDef

```python
# DeleteBridgeRequestRequestTypeDef definition

class DeleteBridgeRequestRequestTypeDef(TypedDict):
    BridgeArn: str,
```

## DeleteFlowRequestRequestTypeDef

```python
# DeleteFlowRequestRequestTypeDef definition

class DeleteFlowRequestRequestTypeDef(TypedDict):
    FlowArn: str,
```

## DeleteGatewayRequestRequestTypeDef

```python
# DeleteGatewayRequestRequestTypeDef definition

class DeleteGatewayRequestRequestTypeDef(TypedDict):
    GatewayArn: str,
```

## DeregisterGatewayInstanceRequestRequestTypeDef

```python
# DeregisterGatewayInstanceRequestRequestTypeDef definition

class DeregisterGatewayInstanceRequestRequestTypeDef(TypedDict):
    GatewayInstanceArn: str,
    Force: NotRequired[bool],
```

## DescribeBridgeRequestRequestTypeDef

```python
# DescribeBridgeRequestRequestTypeDef definition

class DescribeBridgeRequestRequestTypeDef(TypedDict):
    BridgeArn: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeFlowRequestRequestTypeDef

```python
# DescribeFlowRequestRequestTypeDef definition

class DescribeFlowRequestRequestTypeDef(TypedDict):
    FlowArn: str,
```

## MessagesTypeDef

```python
# MessagesTypeDef definition

class MessagesTypeDef(TypedDict):
    Errors: List[str],
```

## DescribeFlowSourceMetadataRequestRequestTypeDef

```python
# DescribeFlowSourceMetadataRequestRequestTypeDef definition

class DescribeFlowSourceMetadataRequestRequestTypeDef(TypedDict):
    FlowArn: str,
```

## DescribeFlowSourceThumbnailRequestRequestTypeDef

```python
# DescribeFlowSourceThumbnailRequestRequestTypeDef definition

class DescribeFlowSourceThumbnailRequestRequestTypeDef(TypedDict):
    FlowArn: str,
```

## DescribeGatewayInstanceRequestRequestTypeDef

```python
# DescribeGatewayInstanceRequestRequestTypeDef definition

class DescribeGatewayInstanceRequestRequestTypeDef(TypedDict):
    GatewayInstanceArn: str,
```

## DescribeGatewayRequestRequestTypeDef

```python
# DescribeGatewayRequestRequestTypeDef definition

class DescribeGatewayRequestRequestTypeDef(TypedDict):
    GatewayArn: str,
```

## DescribeOfferingRequestRequestTypeDef

```python
# DescribeOfferingRequestRequestTypeDef definition

class DescribeOfferingRequestRequestTypeDef(TypedDict):
    OfferingArn: str,
```

## DescribeReservationRequestRequestTypeDef

```python
# DescribeReservationRequestRequestTypeDef definition

class DescribeReservationRequestRequestTypeDef(TypedDict):
    ReservationArn: str,
```

## InterfaceRequestTypeDef

```python
# InterfaceRequestTypeDef definition

class InterfaceRequestTypeDef(TypedDict):
    Name: str,
```

## InterfaceTypeDef

```python
# InterfaceTypeDef definition

class InterfaceTypeDef(TypedDict):
    Name: str,
```

## EncodingParametersRequestTypeDef

```python
# EncodingParametersRequestTypeDef definition

class EncodingParametersRequestTypeDef(TypedDict):
    CompressionFactor: float,
    EncoderProfile: EncoderProfileType,  # (1)
```

1. See [:material-code-brackets: EncoderProfileType](./literals.md#encoderprofiletype) 
## EncodingParametersTypeDef

```python
# EncodingParametersTypeDef definition

class EncodingParametersTypeDef(TypedDict):
    CompressionFactor: float,
    EncoderProfile: EncoderProfileType,  # (1)
```

1. See [:material-code-brackets: EncoderProfileType](./literals.md#encoderprofiletype) 
## SourcePriorityTypeDef

```python
# SourcePriorityTypeDef definition

class SourcePriorityTypeDef(TypedDict):
    PrimarySource: NotRequired[str],
```

## MaintenanceTypeDef

```python
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
# FrameResolutionTypeDef definition

class FrameResolutionTypeDef(TypedDict):
    FrameHeight: int,
    FrameWidth: int,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListBridgesRequestRequestTypeDef

```python
# ListBridgesRequestRequestTypeDef definition

class ListBridgesRequestRequestTypeDef(TypedDict):
    FilterArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListedBridgeTypeDef

```python
# ListedBridgeTypeDef definition

class ListedBridgeTypeDef(TypedDict):
    BridgeArn: str,
    BridgeState: BridgeStateType,  # (1)
    BridgeType: str,
    Name: str,
    PlacementArn: str,
```

1. See [:material-code-brackets: BridgeStateType](./literals.md#bridgestatetype) 
## ListEntitlementsRequestRequestTypeDef

```python
# ListEntitlementsRequestRequestTypeDef definition

class ListEntitlementsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListedEntitlementTypeDef

```python
# ListedEntitlementTypeDef definition

class ListedEntitlementTypeDef(TypedDict):
    EntitlementArn: str,
    EntitlementName: str,
    DataTransferSubscriberFeePercent: NotRequired[int],
```

## ListFlowsRequestRequestTypeDef

```python
# ListFlowsRequestRequestTypeDef definition

class ListFlowsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListGatewayInstancesRequestRequestTypeDef

```python
# ListGatewayInstancesRequestRequestTypeDef definition

class ListGatewayInstancesRequestRequestTypeDef(TypedDict):
    FilterArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListedGatewayInstanceTypeDef

```python
# ListedGatewayInstanceTypeDef definition

class ListedGatewayInstanceTypeDef(TypedDict):
    GatewayArn: str,
    GatewayInstanceArn: str,
    InstanceId: str,
    InstanceState: NotRequired[InstanceStateType],  # (1)
```

1. See [:material-code-brackets: InstanceStateType](./literals.md#instancestatetype) 
## ListGatewaysRequestRequestTypeDef

```python
# ListGatewaysRequestRequestTypeDef definition

class ListGatewaysRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListedGatewayTypeDef

```python
# ListedGatewayTypeDef definition

class ListedGatewayTypeDef(TypedDict):
    GatewayArn: str,
    GatewayState: GatewayStateType,  # (1)
    Name: str,
```

1. See [:material-code-brackets: GatewayStateType](./literals.md#gatewaystatetype) 
## ListOfferingsRequestRequestTypeDef

```python
# ListOfferingsRequestRequestTypeDef definition

class ListOfferingsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListReservationsRequestRequestTypeDef

```python
# ListReservationsRequestRequestTypeDef definition

class ListReservationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ResourceSpecificationTypeDef

```python
# ResourceSpecificationTypeDef definition

class ResourceSpecificationTypeDef(TypedDict):
    ResourceType: ResourceTypeType,  # (1)
    ReservedBitrate: NotRequired[int],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## TransportTypeDef

```python
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
## PurchaseOfferingRequestRequestTypeDef

```python
# PurchaseOfferingRequestRequestTypeDef definition

class PurchaseOfferingRequestRequestTypeDef(TypedDict):
    OfferingArn: str,
    ReservationName: str,
    Start: str,
```

## RemoveBridgeOutputRequestRequestTypeDef

```python
# RemoveBridgeOutputRequestRequestTypeDef definition

class RemoveBridgeOutputRequestRequestTypeDef(TypedDict):
    BridgeArn: str,
    OutputName: str,
```

## RemoveBridgeSourceRequestRequestTypeDef

```python
# RemoveBridgeSourceRequestRequestTypeDef definition

class RemoveBridgeSourceRequestRequestTypeDef(TypedDict):
    BridgeArn: str,
    SourceName: str,
```

## RemoveFlowMediaStreamRequestRequestTypeDef

```python
# RemoveFlowMediaStreamRequestRequestTypeDef definition

class RemoveFlowMediaStreamRequestRequestTypeDef(TypedDict):
    FlowArn: str,
    MediaStreamName: str,
```

## RemoveFlowOutputRequestRequestTypeDef

```python
# RemoveFlowOutputRequestRequestTypeDef definition

class RemoveFlowOutputRequestRequestTypeDef(TypedDict):
    FlowArn: str,
    OutputArn: str,
```

## RemoveFlowSourceRequestRequestTypeDef

```python
# RemoveFlowSourceRequestRequestTypeDef definition

class RemoveFlowSourceRequestRequestTypeDef(TypedDict):
    FlowArn: str,
    SourceArn: str,
```

## RemoveFlowVpcInterfaceRequestRequestTypeDef

```python
# RemoveFlowVpcInterfaceRequestRequestTypeDef definition

class RemoveFlowVpcInterfaceRequestRequestTypeDef(TypedDict):
    FlowArn: str,
    VpcInterfaceName: str,
```

## RevokeFlowEntitlementRequestRequestTypeDef

```python
# RevokeFlowEntitlementRequestRequestTypeDef definition

class RevokeFlowEntitlementRequestRequestTypeDef(TypedDict):
    EntitlementArn: str,
    FlowArn: str,
```

## StartFlowRequestRequestTypeDef

```python
# StartFlowRequestRequestTypeDef definition

class StartFlowRequestRequestTypeDef(TypedDict):
    FlowArn: str,
```

## StopFlowRequestRequestTypeDef

```python
# StopFlowRequestRequestTypeDef definition

class StopFlowRequestRequestTypeDef(TypedDict):
    FlowArn: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateBridgeNetworkOutputRequestTypeDef

```python
# UpdateBridgeNetworkOutputRequestTypeDef definition

class UpdateBridgeNetworkOutputRequestTypeDef(TypedDict):
    IpAddress: NotRequired[str],
    NetworkName: NotRequired[str],
    Port: NotRequired[int],
    Protocol: NotRequired[ProtocolType],  # (1)
    Ttl: NotRequired[int],
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
## UpdateBridgeNetworkSourceRequestTypeDef

```python
# UpdateBridgeNetworkSourceRequestTypeDef definition

class UpdateBridgeNetworkSourceRequestTypeDef(TypedDict):
    MulticastIp: NotRequired[str],
    NetworkName: NotRequired[str],
    Port: NotRequired[int],
    Protocol: NotRequired[ProtocolType],  # (1)
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
## UpdateEgressGatewayBridgeRequestTypeDef

```python
# UpdateEgressGatewayBridgeRequestTypeDef definition

class UpdateEgressGatewayBridgeRequestTypeDef(TypedDict):
    MaxBitrate: NotRequired[int],
```

## UpdateIngressGatewayBridgeRequestTypeDef

```python
# UpdateIngressGatewayBridgeRequestTypeDef definition

class UpdateIngressGatewayBridgeRequestTypeDef(TypedDict):
    MaxBitrate: NotRequired[int],
    MaxOutputs: NotRequired[int],
```

## UpdateBridgeStateRequestRequestTypeDef

```python
# UpdateBridgeStateRequestRequestTypeDef definition

class UpdateBridgeStateRequestRequestTypeDef(TypedDict):
    BridgeArn: str,
    DesiredState: DesiredStateType,  # (1)
```

1. See [:material-code-brackets: DesiredStateType](./literals.md#desiredstatetype) 
## UpdateEncryptionTypeDef

```python
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
# UpdateMaintenanceTypeDef definition

class UpdateMaintenanceTypeDef(TypedDict):
    MaintenanceDay: NotRequired[MaintenanceDayType],  # (1)
    MaintenanceScheduledDate: NotRequired[str],
    MaintenanceStartHour: NotRequired[str],
```

1. See [:material-code-brackets: MaintenanceDayType](./literals.md#maintenancedaytype) 
## UpdateGatewayInstanceRequestRequestTypeDef

```python
# UpdateGatewayInstanceRequestRequestTypeDef definition

class UpdateGatewayInstanceRequestRequestTypeDef(TypedDict):
    GatewayInstanceArn: str,
    BridgePlacement: NotRequired[BridgePlacementType],  # (1)
```

1. See [:material-code-brackets: BridgePlacementType](./literals.md#bridgeplacementtype) 
## AddBridgeFlowSourceRequestTypeDef

```python
# AddBridgeFlowSourceRequestTypeDef definition

class AddBridgeFlowSourceRequestTypeDef(TypedDict):
    FlowArn: str,
    Name: str,
    FlowVpcInterfaceAttachment: NotRequired[VpcInterfaceAttachmentTypeDef],  # (1)
```

1. See [:material-code-braces: VpcInterfaceAttachmentTypeDef](./type_defs.md#vpcinterfaceattachmenttypedef) 
## BridgeFlowSourceTypeDef

```python
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
# GatewayBridgeSourceTypeDef definition

class GatewayBridgeSourceTypeDef(TypedDict):
    BridgeArn: str,
    VpcInterfaceAttachment: NotRequired[VpcInterfaceAttachmentTypeDef],  # (1)
```

1. See [:material-code-braces: VpcInterfaceAttachmentTypeDef](./type_defs.md#vpcinterfaceattachmenttypedef) 
## SetGatewayBridgeSourceRequestTypeDef

```python
# SetGatewayBridgeSourceRequestTypeDef definition

class SetGatewayBridgeSourceRequestTypeDef(TypedDict):
    BridgeArn: str,
    VpcInterfaceAttachment: NotRequired[VpcInterfaceAttachmentTypeDef],  # (1)
```

1. See [:material-code-braces: VpcInterfaceAttachmentTypeDef](./type_defs.md#vpcinterfaceattachmenttypedef) 
## UpdateBridgeFlowSourceRequestTypeDef

```python
# UpdateBridgeFlowSourceRequestTypeDef definition

class UpdateBridgeFlowSourceRequestTypeDef(TypedDict):
    FlowArn: NotRequired[str],
    FlowVpcInterfaceAttachment: NotRequired[VpcInterfaceAttachmentTypeDef],  # (1)
```

1. See [:material-code-braces: VpcInterfaceAttachmentTypeDef](./type_defs.md#vpcinterfaceattachmenttypedef) 
## UpdateGatewayBridgeSourceRequestTypeDef

```python
# UpdateGatewayBridgeSourceRequestTypeDef definition

class UpdateGatewayBridgeSourceRequestTypeDef(TypedDict):
    BridgeArn: NotRequired[str],
    VpcInterfaceAttachment: NotRequired[VpcInterfaceAttachmentTypeDef],  # (1)
```

1. See [:material-code-braces: VpcInterfaceAttachmentTypeDef](./type_defs.md#vpcinterfaceattachmenttypedef) 
## AddBridgeOutputRequestTypeDef

```python
# AddBridgeOutputRequestTypeDef definition

class AddBridgeOutputRequestTypeDef(TypedDict):
    NetworkOutput: NotRequired[AddBridgeNetworkOutputRequestTypeDef],  # (1)
```

1. See [:material-code-braces: AddBridgeNetworkOutputRequestTypeDef](./type_defs.md#addbridgenetworkoutputrequesttypedef) 
## DeleteBridgeResponseTypeDef

```python
# DeleteBridgeResponseTypeDef definition

class DeleteBridgeResponseTypeDef(TypedDict):
    BridgeArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteFlowResponseTypeDef

```python
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
# DeleteGatewayResponseTypeDef definition

class DeleteGatewayResponseTypeDef(TypedDict):
    GatewayArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeregisterGatewayInstanceResponseTypeDef

```python
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
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveBridgeOutputResponseTypeDef

```python
# RemoveBridgeOutputResponseTypeDef definition

class RemoveBridgeOutputResponseTypeDef(TypedDict):
    BridgeArn: str,
    OutputName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveBridgeSourceResponseTypeDef

```python
# RemoveBridgeSourceResponseTypeDef definition

class RemoveBridgeSourceResponseTypeDef(TypedDict):
    BridgeArn: str,
    SourceName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveFlowMediaStreamResponseTypeDef

```python
# RemoveFlowMediaStreamResponseTypeDef definition

class RemoveFlowMediaStreamResponseTypeDef(TypedDict):
    FlowArn: str,
    MediaStreamName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveFlowOutputResponseTypeDef

```python
# RemoveFlowOutputResponseTypeDef definition

class RemoveFlowOutputResponseTypeDef(TypedDict):
    FlowArn: str,
    OutputArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveFlowSourceResponseTypeDef

```python
# RemoveFlowSourceResponseTypeDef definition

class RemoveFlowSourceResponseTypeDef(TypedDict):
    FlowArn: str,
    SourceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveFlowVpcInterfaceResponseTypeDef

```python
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
# RevokeFlowEntitlementResponseTypeDef definition

class RevokeFlowEntitlementResponseTypeDef(TypedDict):
    EntitlementArn: str,
    FlowArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartFlowResponseTypeDef

```python
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
# UpdateGatewayInstanceResponseTypeDef definition

class UpdateGatewayInstanceResponseTypeDef(TypedDict):
    BridgePlacement: BridgePlacementType,  # (1)
    GatewayInstanceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: BridgePlacementType](./literals.md#bridgeplacementtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddFlowVpcInterfacesRequestRequestTypeDef

```python
# AddFlowVpcInterfacesRequestRequestTypeDef definition

class AddFlowVpcInterfacesRequestRequestTypeDef(TypedDict):
    FlowArn: str,
    VpcInterfaces: Sequence[VpcInterfaceRequestTypeDef],  # (1)
```

1. See [:material-code-braces: VpcInterfaceRequestTypeDef](./type_defs.md#vpcinterfacerequesttypedef) 
## AddFlowVpcInterfacesResponseTypeDef

```python
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
## BridgeOutputTypeDef

```python
# BridgeOutputTypeDef definition

class BridgeOutputTypeDef(TypedDict):
    FlowOutput: NotRequired[BridgeFlowOutputTypeDef],  # (1)
    NetworkOutput: NotRequired[BridgeNetworkOutputTypeDef],  # (2)
```

1. See [:material-code-braces: BridgeFlowOutputTypeDef](./type_defs.md#bridgeflowoutputtypedef) 
2. See [:material-code-braces: BridgeNetworkOutputTypeDef](./type_defs.md#bridgenetworkoutputtypedef) 
## GatewayInstanceTypeDef

```python
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
# ThumbnailDetailsTypeDef definition

class ThumbnailDetailsTypeDef(TypedDict):
    FlowArn: str,
    ThumbnailMessages: List[MessageDetailTypeDef],  # (1)
    Thumbnail: NotRequired[str],
    Timecode: NotRequired[str],
    Timestamp: NotRequired[datetime],
```

1. See [:material-code-braces: MessageDetailTypeDef](./type_defs.md#messagedetailtypedef) 
## CreateGatewayRequestRequestTypeDef

```python
# CreateGatewayRequestRequestTypeDef definition

class CreateGatewayRequestRequestTypeDef(TypedDict):
    EgressCidrBlocks: Sequence[str],
    Name: str,
    Networks: Sequence[GatewayNetworkTypeDef],  # (1)
```

1. See [:material-code-braces: GatewayNetworkTypeDef](./type_defs.md#gatewaynetworktypedef) 
## GatewayTypeDef

```python
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
## DescribeFlowRequestFlowActiveWaitTypeDef

```python
# DescribeFlowRequestFlowActiveWaitTypeDef definition

class DescribeFlowRequestFlowActiveWaitTypeDef(TypedDict):
    FlowArn: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeFlowRequestFlowDeletedWaitTypeDef

```python
# DescribeFlowRequestFlowDeletedWaitTypeDef definition

class DescribeFlowRequestFlowDeletedWaitTypeDef(TypedDict):
    FlowArn: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeFlowRequestFlowStandbyWaitTypeDef

```python
# DescribeFlowRequestFlowStandbyWaitTypeDef definition

class DescribeFlowRequestFlowStandbyWaitTypeDef(TypedDict):
    FlowArn: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DestinationConfigurationRequestTypeDef

```python
# DestinationConfigurationRequestTypeDef definition

class DestinationConfigurationRequestTypeDef(TypedDict):
    DestinationIp: str,
    DestinationPort: int,
    Interface: InterfaceRequestTypeDef,  # (1)
```

1. See [:material-code-braces: InterfaceRequestTypeDef](./type_defs.md#interfacerequesttypedef) 
## InputConfigurationRequestTypeDef

```python
# InputConfigurationRequestTypeDef definition

class InputConfigurationRequestTypeDef(TypedDict):
    InputPort: int,
    Interface: InterfaceRequestTypeDef,  # (1)
```

1. See [:material-code-braces: InterfaceRequestTypeDef](./type_defs.md#interfacerequesttypedef) 
## DestinationConfigurationTypeDef

```python
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
# InputConfigurationTypeDef definition

class InputConfigurationTypeDef(TypedDict):
    InputIp: str,
    InputPort: int,
    Interface: InterfaceTypeDef,  # (1)
```

1. See [:material-code-braces: InterfaceTypeDef](./type_defs.md#interfacetypedef) 
## FailoverConfigTypeDef

```python
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
# MediaStreamAttributesRequestTypeDef definition

class MediaStreamAttributesRequestTypeDef(TypedDict):
    Fmtp: NotRequired[FmtpRequestTypeDef],  # (1)
    Lang: NotRequired[str],
```

1. See [:material-code-braces: FmtpRequestTypeDef](./type_defs.md#fmtprequesttypedef) 
## MediaStreamAttributesTypeDef

```python
# MediaStreamAttributesTypeDef definition

class MediaStreamAttributesTypeDef(TypedDict):
    Fmtp: FmtpTypeDef,  # (1)
    Lang: NotRequired[str],
```

1. See [:material-code-braces: FmtpTypeDef](./type_defs.md#fmtptypedef) 
## TransportStreamTypeDef

```python
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
## ListBridgesRequestListBridgesPaginateTypeDef

```python
# ListBridgesRequestListBridgesPaginateTypeDef definition

class ListBridgesRequestListBridgesPaginateTypeDef(TypedDict):
    FilterArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEntitlementsRequestListEntitlementsPaginateTypeDef

```python
# ListEntitlementsRequestListEntitlementsPaginateTypeDef definition

class ListEntitlementsRequestListEntitlementsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFlowsRequestListFlowsPaginateTypeDef

```python
# ListFlowsRequestListFlowsPaginateTypeDef definition

class ListFlowsRequestListFlowsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef

```python
# ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef definition

class ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef(TypedDict):
    FilterArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGatewaysRequestListGatewaysPaginateTypeDef

```python
# ListGatewaysRequestListGatewaysPaginateTypeDef definition

class ListGatewaysRequestListGatewaysPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOfferingsRequestListOfferingsPaginateTypeDef

```python
# ListOfferingsRequestListOfferingsPaginateTypeDef definition

class ListOfferingsRequestListOfferingsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReservationsRequestListReservationsPaginateTypeDef

```python
# ListReservationsRequestListReservationsPaginateTypeDef definition

class ListReservationsRequestListReservationsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBridgesResponseTypeDef

```python
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
## UpdateBridgeOutputRequestRequestTypeDef

```python
# UpdateBridgeOutputRequestRequestTypeDef definition

class UpdateBridgeOutputRequestRequestTypeDef(TypedDict):
    BridgeArn: str,
    OutputName: str,
    NetworkOutput: NotRequired[UpdateBridgeNetworkOutputRequestTypeDef],  # (1)
```

1. See [:material-code-braces: UpdateBridgeNetworkOutputRequestTypeDef](./type_defs.md#updatebridgenetworkoutputrequesttypedef) 
## UpdateFlowEntitlementRequestRequestTypeDef

```python
# UpdateFlowEntitlementRequestRequestTypeDef definition

class UpdateFlowEntitlementRequestRequestTypeDef(TypedDict):
    EntitlementArn: str,
    FlowArn: str,
    Description: NotRequired[str],
    Encryption: NotRequired[UpdateEncryptionTypeDef],  # (1)
    EntitlementStatus: NotRequired[EntitlementStatusType],  # (2)
    Subscribers: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: UpdateEncryptionTypeDef](./type_defs.md#updateencryptiontypedef) 
2. See [:material-code-brackets: EntitlementStatusType](./literals.md#entitlementstatustype) 
## AddBridgeSourceRequestTypeDef

```python
# AddBridgeSourceRequestTypeDef definition

class AddBridgeSourceRequestTypeDef(TypedDict):
    FlowSource: NotRequired[AddBridgeFlowSourceRequestTypeDef],  # (1)
    NetworkSource: NotRequired[AddBridgeNetworkSourceRequestTypeDef],  # (2)
```

1. See [:material-code-braces: AddBridgeFlowSourceRequestTypeDef](./type_defs.md#addbridgeflowsourcerequesttypedef) 
2. See [:material-code-braces: AddBridgeNetworkSourceRequestTypeDef](./type_defs.md#addbridgenetworksourcerequesttypedef) 
## BridgeSourceTypeDef

```python
# BridgeSourceTypeDef definition

class BridgeSourceTypeDef(TypedDict):
    FlowSource: NotRequired[BridgeFlowSourceTypeDef],  # (1)
    NetworkSource: NotRequired[BridgeNetworkSourceTypeDef],  # (2)
```

1. See [:material-code-braces: BridgeFlowSourceTypeDef](./type_defs.md#bridgeflowsourcetypedef) 
2. See [:material-code-braces: BridgeNetworkSourceTypeDef](./type_defs.md#bridgenetworksourcetypedef) 
## UpdateBridgeSourceRequestRequestTypeDef

```python
# UpdateBridgeSourceRequestRequestTypeDef definition

class UpdateBridgeSourceRequestRequestTypeDef(TypedDict):
    BridgeArn: str,
    SourceName: str,
    FlowSource: NotRequired[UpdateBridgeFlowSourceRequestTypeDef],  # (1)
    NetworkSource: NotRequired[UpdateBridgeNetworkSourceRequestTypeDef],  # (2)
```

1. See [:material-code-braces: UpdateBridgeFlowSourceRequestTypeDef](./type_defs.md#updatebridgeflowsourcerequesttypedef) 
2. See [:material-code-braces: UpdateBridgeNetworkSourceRequestTypeDef](./type_defs.md#updatebridgenetworksourcerequesttypedef) 
## AddBridgeOutputsRequestRequestTypeDef

```python
# AddBridgeOutputsRequestRequestTypeDef definition

class AddBridgeOutputsRequestRequestTypeDef(TypedDict):
    BridgeArn: str,
    Outputs: Sequence[AddBridgeOutputRequestTypeDef],  # (1)
```

1. See [:material-code-braces: AddBridgeOutputRequestTypeDef](./type_defs.md#addbridgeoutputrequesttypedef) 
## GrantFlowEntitlementsResponseTypeDef

```python
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
# UpdateFlowEntitlementResponseTypeDef definition

class UpdateFlowEntitlementResponseTypeDef(TypedDict):
    Entitlement: EntitlementTypeDef,  # (1)
    FlowArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EntitlementTypeDef](./type_defs.md#entitlementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GrantFlowEntitlementsRequestRequestTypeDef

```python
# GrantFlowEntitlementsRequestRequestTypeDef definition

class GrantFlowEntitlementsRequestRequestTypeDef(TypedDict):
    Entitlements: Sequence[GrantEntitlementRequestTypeDef],  # (1)
    FlowArn: str,
```

1. See [:material-code-braces: GrantEntitlementRequestTypeDef](./type_defs.md#grantentitlementrequesttypedef) 
## AddBridgeOutputsResponseTypeDef

```python
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
# DescribeGatewayInstanceResponseTypeDef definition

class DescribeGatewayInstanceResponseTypeDef(TypedDict):
    GatewayInstance: GatewayInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GatewayInstanceTypeDef](./type_defs.md#gatewayinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFlowSourceThumbnailResponseTypeDef

```python
# DescribeFlowSourceThumbnailResponseTypeDef definition

class DescribeFlowSourceThumbnailResponseTypeDef(TypedDict):
    ThumbnailDetails: ThumbnailDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThumbnailDetailsTypeDef](./type_defs.md#thumbnaildetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGatewayResponseTypeDef

```python
# CreateGatewayResponseTypeDef definition

class CreateGatewayResponseTypeDef(TypedDict):
    Gateway: GatewayTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GatewayTypeDef](./type_defs.md#gatewaytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGatewayResponseTypeDef

```python
# DescribeGatewayResponseTypeDef definition

class DescribeGatewayResponseTypeDef(TypedDict):
    Gateway: GatewayTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GatewayTypeDef](./type_defs.md#gatewaytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MediaStreamOutputConfigurationRequestTypeDef

```python
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
# MediaStreamSourceConfigurationTypeDef definition

class MediaStreamSourceConfigurationTypeDef(TypedDict):
    EncodingName: EncodingNameType,  # (1)
    MediaStreamName: str,
    InputConfigurations: NotRequired[List[InputConfigurationTypeDef]],  # (2)
```

1. See [:material-code-brackets: EncodingNameType](./literals.md#encodingnametype) 
2. See [:material-code-braces: InputConfigurationTypeDef](./type_defs.md#inputconfigurationtypedef) 
## UpdateBridgeRequestRequestTypeDef

```python
# UpdateBridgeRequestRequestTypeDef definition

class UpdateBridgeRequestRequestTypeDef(TypedDict):
    BridgeArn: str,
    EgressGatewayBridge: NotRequired[UpdateEgressGatewayBridgeRequestTypeDef],  # (1)
    IngressGatewayBridge: NotRequired[UpdateIngressGatewayBridgeRequestTypeDef],  # (2)
    SourceFailoverConfig: NotRequired[UpdateFailoverConfigTypeDef],  # (3)
```

1. See [:material-code-braces: UpdateEgressGatewayBridgeRequestTypeDef](./type_defs.md#updateegressgatewaybridgerequesttypedef) 
2. See [:material-code-braces: UpdateIngressGatewayBridgeRequestTypeDef](./type_defs.md#updateingressgatewaybridgerequesttypedef) 
3. See [:material-code-braces: UpdateFailoverConfigTypeDef](./type_defs.md#updatefailoverconfigtypedef) 
## UpdateFlowRequestRequestTypeDef

```python
# UpdateFlowRequestRequestTypeDef definition

class UpdateFlowRequestRequestTypeDef(TypedDict):
    FlowArn: str,
    SourceFailoverConfig: NotRequired[UpdateFailoverConfigTypeDef],  # (1)
    Maintenance: NotRequired[UpdateMaintenanceTypeDef],  # (2)
    SourceMonitoringConfig: NotRequired[MonitoringConfigTypeDef],  # (3)
```

1. See [:material-code-braces: UpdateFailoverConfigTypeDef](./type_defs.md#updatefailoverconfigtypedef) 
2. See [:material-code-braces: UpdateMaintenanceTypeDef](./type_defs.md#updatemaintenancetypedef) 
3. See [:material-code-braces: MonitoringConfigTypeDef](./type_defs.md#monitoringconfigtypedef) 
## ListFlowsResponseTypeDef

```python
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
## UpdateFlowMediaStreamRequestRequestTypeDef

```python
# UpdateFlowMediaStreamRequestRequestTypeDef definition

class UpdateFlowMediaStreamRequestRequestTypeDef(TypedDict):
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
# TransportStreamProgramTypeDef definition

class TransportStreamProgramTypeDef(TypedDict):
    PcrPid: int,
    ProgramNumber: int,
    ProgramPid: int,
    Streams: List[TransportStreamTypeDef],  # (1)
    ProgramName: NotRequired[str],
```

1. See [:material-code-braces: TransportStreamTypeDef](./type_defs.md#transportstreamtypedef) 
## DescribeOfferingResponseTypeDef

```python
# DescribeOfferingResponseTypeDef definition

class DescribeOfferingResponseTypeDef(TypedDict):
    Offering: OfferingTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OfferingTypeDef](./type_defs.md#offeringtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOfferingsResponseTypeDef

```python
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
# DescribeReservationResponseTypeDef definition

class DescribeReservationResponseTypeDef(TypedDict):
    Reservation: ReservationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservationTypeDef](./type_defs.md#reservationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReservationsResponseTypeDef

```python
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
# PurchaseOfferingResponseTypeDef definition

class PurchaseOfferingResponseTypeDef(TypedDict):
    Reservation: ReservationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservationTypeDef](./type_defs.md#reservationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddBridgeSourcesRequestRequestTypeDef

```python
# AddBridgeSourcesRequestRequestTypeDef definition

class AddBridgeSourcesRequestRequestTypeDef(TypedDict):
    BridgeArn: str,
    Sources: Sequence[AddBridgeSourceRequestTypeDef],  # (1)
```

1. See [:material-code-braces: AddBridgeSourceRequestTypeDef](./type_defs.md#addbridgesourcerequesttypedef) 
## CreateBridgeRequestRequestTypeDef

```python
# CreateBridgeRequestRequestTypeDef definition

class CreateBridgeRequestRequestTypeDef(TypedDict):
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
## UpdateFlowOutputRequestRequestTypeDef

```python
# UpdateFlowOutputRequestRequestTypeDef definition

class UpdateFlowOutputRequestRequestTypeDef(TypedDict):
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
## UpdateFlowSourceRequestRequestTypeDef

```python
# UpdateFlowSourceRequestRequestTypeDef definition

class UpdateFlowSourceRequestRequestTypeDef(TypedDict):
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
## AddFlowMediaStreamsRequestRequestTypeDef

```python
# AddFlowMediaStreamsRequestRequestTypeDef definition

class AddFlowMediaStreamsRequestRequestTypeDef(TypedDict):
    FlowArn: str,
    MediaStreams: Sequence[AddMediaStreamRequestTypeDef],  # (1)
```

1. See [:material-code-braces: AddMediaStreamRequestTypeDef](./type_defs.md#addmediastreamrequesttypedef) 
## AddFlowMediaStreamsResponseTypeDef

```python
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
# TransportMediaInfoTypeDef definition

class TransportMediaInfoTypeDef(TypedDict):
    Programs: List[TransportStreamProgramTypeDef],  # (1)
```

1. See [:material-code-braces: TransportStreamProgramTypeDef](./type_defs.md#transportstreamprogramtypedef) 
## CreateBridgeResponseTypeDef

```python
# CreateBridgeResponseTypeDef definition

class CreateBridgeResponseTypeDef(TypedDict):
    Bridge: BridgeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BridgeTypeDef](./type_defs.md#bridgetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBridgeResponseTypeDef

```python
# DescribeBridgeResponseTypeDef definition

class DescribeBridgeResponseTypeDef(TypedDict):
    Bridge: BridgeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BridgeTypeDef](./type_defs.md#bridgetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBridgeResponseTypeDef

```python
# UpdateBridgeResponseTypeDef definition

class UpdateBridgeResponseTypeDef(TypedDict):
    Bridge: BridgeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BridgeTypeDef](./type_defs.md#bridgetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddFlowOutputsRequestRequestTypeDef

```python
# AddFlowOutputsRequestRequestTypeDef definition

class AddFlowOutputsRequestRequestTypeDef(TypedDict):
    FlowArn: str,
    Outputs: Sequence[AddOutputRequestTypeDef],  # (1)
```

1. See [:material-code-braces: AddOutputRequestTypeDef](./type_defs.md#addoutputrequesttypedef) 
## AddFlowSourcesRequestRequestTypeDef

```python
# AddFlowSourcesRequestRequestTypeDef definition

class AddFlowSourcesRequestRequestTypeDef(TypedDict):
    FlowArn: str,
    Sources: Sequence[SetSourceRequestTypeDef],  # (1)
```

1. See [:material-code-braces: SetSourceRequestTypeDef](./type_defs.md#setsourcerequesttypedef) 
## CreateFlowRequestRequestTypeDef

```python
# CreateFlowRequestRequestTypeDef definition

class CreateFlowRequestRequestTypeDef(TypedDict):
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
    SourceMonitoringConfig: NotRequired[MonitoringConfigTypeDef],  # (9)
```

1. See [:material-code-braces: GrantEntitlementRequestTypeDef](./type_defs.md#grantentitlementrequesttypedef) 
2. See [:material-code-braces: AddMediaStreamRequestTypeDef](./type_defs.md#addmediastreamrequesttypedef) 
3. See [:material-code-braces: AddOutputRequestTypeDef](./type_defs.md#addoutputrequesttypedef) 
4. See [:material-code-braces: SetSourceRequestTypeDef](./type_defs.md#setsourcerequesttypedef) 
5. See [:material-code-braces: FailoverConfigTypeDef](./type_defs.md#failoverconfigtypedef) 
6. See [:material-code-braces: SetSourceRequestTypeDef](./type_defs.md#setsourcerequesttypedef) 
7. See [:material-code-braces: VpcInterfaceRequestTypeDef](./type_defs.md#vpcinterfacerequesttypedef) 
8. See [:material-code-braces: AddMaintenanceTypeDef](./type_defs.md#addmaintenancetypedef) 
9. See [:material-code-braces: MonitoringConfigTypeDef](./type_defs.md#monitoringconfigtypedef) 
## AddFlowOutputsResponseTypeDef

```python
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
    SourceMonitoringConfig: NotRequired[MonitoringConfigTypeDef],  # (10)
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
10. See [:material-code-braces: MonitoringConfigTypeDef](./type_defs.md#monitoringconfigtypedef) 
## UpdateFlowSourceResponseTypeDef

```python
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
## CreateFlowResponseTypeDef

```python
# CreateFlowResponseTypeDef definition

class CreateFlowResponseTypeDef(TypedDict):
    Flow: FlowTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlowTypeDef](./type_defs.md#flowtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFlowResponseTypeDef

```python
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
# UpdateFlowResponseTypeDef definition

class UpdateFlowResponseTypeDef(TypedDict):
    Flow: FlowTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlowTypeDef](./type_defs.md#flowtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
