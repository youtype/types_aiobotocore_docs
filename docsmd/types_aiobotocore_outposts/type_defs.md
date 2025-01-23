# Type definitions

> [Index](../README.md) > [Outposts](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Outposts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#outposts)
    type annotations stubs module [types-aiobotocore-outposts](https://pypi.org/project/types-aiobotocore-outposts/).



## AddressTypeDef

```python
# AddressTypeDef definition

class AddressTypeDef(TypedDict):
    AddressLine1: str,
    City: str,
    StateOrRegion: str,
    PostalCode: str,
    CountryCode: str,
    ContactName: NotRequired[str],
    ContactPhoneNumber: NotRequired[str],
    AddressLine2: NotRequired[str],
    AddressLine3: NotRequired[str],
    DistrictOrCounty: NotRequired[str],
    Municipality: NotRequired[str],
```

## AssetLocationTypeDef

```python
# AssetLocationTypeDef definition

class AssetLocationTypeDef(TypedDict):
    RackElevation: NotRequired[float],
```

## AssetInstanceTypeCapacityTypeDef

```python
# AssetInstanceTypeCapacityTypeDef definition

class AssetInstanceTypeCapacityTypeDef(TypedDict):
    InstanceType: str,
    Count: int,
```

## AssetInstanceTypeDef

```python
# AssetInstanceTypeDef definition

class AssetInstanceTypeDef(TypedDict):
    InstanceId: NotRequired[str],
    InstanceType: NotRequired[str],
    AssetId: NotRequired[str],
    AccountId: NotRequired[str],
    AwsServiceName: NotRequired[AWSServiceNameType],  # (1)
```

1. See [:material-code-brackets: AWSServiceNameType](./literals.md#awsservicenametype) 
## BlockingInstanceTypeDef

```python
# BlockingInstanceTypeDef definition

class BlockingInstanceTypeDef(TypedDict):
    InstanceId: NotRequired[str],
    AccountId: NotRequired[str],
    AwsServiceName: NotRequired[AWSServiceNameType],  # (1)
```

1. See [:material-code-brackets: AWSServiceNameType](./literals.md#awsservicenametype) 
## CancelCapacityTaskInputRequestTypeDef

```python
# CancelCapacityTaskInputRequestTypeDef definition

class CancelCapacityTaskInputRequestTypeDef(TypedDict):
    CapacityTaskId: str,
    OutpostIdentifier: str,
```

## CancelOrderInputRequestTypeDef

```python
# CancelOrderInputRequestTypeDef definition

class CancelOrderInputRequestTypeDef(TypedDict):
    OrderId: str,
```

## CapacityTaskFailureTypeDef

```python
# CapacityTaskFailureTypeDef definition

class CapacityTaskFailureTypeDef(TypedDict):
    Reason: str,
    Type: NotRequired[CapacityTaskFailureTypeType],  # (1)
```

1. See [:material-code-brackets: CapacityTaskFailureTypeType](./literals.md#capacitytaskfailuretypetype) 
## CapacityTaskSummaryTypeDef

```python
# CapacityTaskSummaryTypeDef definition

class CapacityTaskSummaryTypeDef(TypedDict):
    CapacityTaskId: NotRequired[str],
    OutpostId: NotRequired[str],
    OrderId: NotRequired[str],
    CapacityTaskStatus: NotRequired[CapacityTaskStatusType],  # (1)
    CreationDate: NotRequired[datetime],
    CompletionDate: NotRequired[datetime],
    LastModifiedDate: NotRequired[datetime],
```

1. See [:material-code-brackets: CapacityTaskStatusType](./literals.md#capacitytaskstatustype) 
## EC2CapacityTypeDef

```python
# EC2CapacityTypeDef definition

class EC2CapacityTypeDef(TypedDict):
    Family: NotRequired[str],
    MaxSize: NotRequired[str],
    Quantity: NotRequired[str],
```

## ConnectionDetailsTypeDef

```python
# ConnectionDetailsTypeDef definition

class ConnectionDetailsTypeDef(TypedDict):
    ClientPublicKey: NotRequired[str],
    ServerPublicKey: NotRequired[str],
    ServerEndpoint: NotRequired[str],
    ClientTunnelAddress: NotRequired[str],
    ServerTunnelAddress: NotRequired[str],
    AllowedIps: NotRequired[List[str]],
```

## LineItemRequestTypeDef

```python
# LineItemRequestTypeDef definition

class LineItemRequestTypeDef(TypedDict):
    CatalogItemId: NotRequired[str],
    Quantity: NotRequired[int],
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

## CreateOutpostInputRequestTypeDef

```python
# CreateOutpostInputRequestTypeDef definition

class CreateOutpostInputRequestTypeDef(TypedDict):
    Name: str,
    SiteId: str,
    Description: NotRequired[str],
    AvailabilityZone: NotRequired[str],
    AvailabilityZoneId: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    SupportedHardwareType: NotRequired[SupportedHardwareTypeType],  # (1)
```

1. See [:material-code-brackets: SupportedHardwareTypeType](./literals.md#supportedhardwaretypetype) 
## OutpostTypeDef

```python
# OutpostTypeDef definition

class OutpostTypeDef(TypedDict):
    OutpostId: NotRequired[str],
    OwnerId: NotRequired[str],
    OutpostArn: NotRequired[str],
    SiteId: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    LifeCycleStatus: NotRequired[str],
    AvailabilityZone: NotRequired[str],
    AvailabilityZoneId: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
    SiteArn: NotRequired[str],
    SupportedHardwareType: NotRequired[SupportedHardwareTypeType],  # (1)
```

1. See [:material-code-brackets: SupportedHardwareTypeType](./literals.md#supportedhardwaretypetype) 
## RackPhysicalPropertiesTypeDef

```python
# RackPhysicalPropertiesTypeDef definition

class RackPhysicalPropertiesTypeDef(TypedDict):
    PowerDrawKva: NotRequired[PowerDrawKvaType],  # (1)
    PowerPhase: NotRequired[PowerPhaseType],  # (2)
    PowerConnector: NotRequired[PowerConnectorType],  # (3)
    PowerFeedDrop: NotRequired[PowerFeedDropType],  # (4)
    UplinkGbps: NotRequired[UplinkGbpsType],  # (5)
    UplinkCount: NotRequired[UplinkCountType],  # (6)
    FiberOpticCableType: NotRequired[FiberOpticCableTypeType],  # (7)
    OpticalStandard: NotRequired[OpticalStandardType],  # (8)
    MaximumSupportedWeightLbs: NotRequired[MaximumSupportedWeightLbsType],  # (9)
```

1. See [:material-code-brackets: PowerDrawKvaType](./literals.md#powerdrawkvatype) 
2. See [:material-code-brackets: PowerPhaseType](./literals.md#powerphasetype) 
3. See [:material-code-brackets: PowerConnectorType](./literals.md#powerconnectortype) 
4. See [:material-code-brackets: PowerFeedDropType](./literals.md#powerfeeddroptype) 
5. See [:material-code-brackets: UplinkGbpsType](./literals.md#uplinkgbpstype) 
6. See [:material-code-brackets: UplinkCountType](./literals.md#uplinkcounttype) 
7. See [:material-code-brackets: FiberOpticCableTypeType](./literals.md#fiberopticcabletypetype) 
8. See [:material-code-brackets: OpticalStandardType](./literals.md#opticalstandardtype) 
9. See [:material-code-brackets: MaximumSupportedWeightLbsType](./literals.md#maximumsupportedweightlbstype) 
## DeleteOutpostInputRequestTypeDef

```python
# DeleteOutpostInputRequestTypeDef definition

class DeleteOutpostInputRequestTypeDef(TypedDict):
    OutpostId: str,
```

## DeleteSiteInputRequestTypeDef

```python
# DeleteSiteInputRequestTypeDef definition

class DeleteSiteInputRequestTypeDef(TypedDict):
    SiteId: str,
```

## GetCapacityTaskInputRequestTypeDef

```python
# GetCapacityTaskInputRequestTypeDef definition

class GetCapacityTaskInputRequestTypeDef(TypedDict):
    CapacityTaskId: str,
    OutpostIdentifier: str,
```

## InstanceTypeCapacityTypeDef

```python
# InstanceTypeCapacityTypeDef definition

class InstanceTypeCapacityTypeDef(TypedDict):
    InstanceType: str,
    Count: int,
```

## InstancesToExcludeOutputTypeDef

```python
# InstancesToExcludeOutputTypeDef definition

class InstancesToExcludeOutputTypeDef(TypedDict):
    Instances: NotRequired[List[str]],
    AccountIds: NotRequired[List[str]],
    Services: NotRequired[List[AWSServiceNameType]],  # (1)
```

1. See [:material-code-brackets: AWSServiceNameType](./literals.md#awsservicenametype) 
## GetCatalogItemInputRequestTypeDef

```python
# GetCatalogItemInputRequestTypeDef definition

class GetCatalogItemInputRequestTypeDef(TypedDict):
    CatalogItemId: str,
```

## GetConnectionRequestRequestTypeDef

```python
# GetConnectionRequestRequestTypeDef definition

class GetConnectionRequestRequestTypeDef(TypedDict):
    ConnectionId: str,
```

## GetOrderInputRequestTypeDef

```python
# GetOrderInputRequestTypeDef definition

class GetOrderInputRequestTypeDef(TypedDict):
    OrderId: str,
```

## GetOutpostInputRequestTypeDef

```python
# GetOutpostInputRequestTypeDef definition

class GetOutpostInputRequestTypeDef(TypedDict):
    OutpostId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetOutpostInstanceTypesInputRequestTypeDef

```python
# GetOutpostInstanceTypesInputRequestTypeDef definition

class GetOutpostInstanceTypesInputRequestTypeDef(TypedDict):
    OutpostId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## InstanceTypeItemTypeDef

```python
# InstanceTypeItemTypeDef definition

class InstanceTypeItemTypeDef(TypedDict):
    InstanceType: NotRequired[str],
    VCPUs: NotRequired[int],
```

## GetOutpostSupportedInstanceTypesInputRequestTypeDef

```python
# GetOutpostSupportedInstanceTypesInputRequestTypeDef definition

class GetOutpostSupportedInstanceTypesInputRequestTypeDef(TypedDict):
    OutpostIdentifier: str,
    OrderId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetSiteAddressInputRequestTypeDef

```python
# GetSiteAddressInputRequestTypeDef definition

class GetSiteAddressInputRequestTypeDef(TypedDict):
    SiteId: str,
    AddressType: AddressTypeType,  # (1)
```

1. See [:material-code-brackets: AddressTypeType](./literals.md#addresstypetype) 
## GetSiteInputRequestTypeDef

```python
# GetSiteInputRequestTypeDef definition

class GetSiteInputRequestTypeDef(TypedDict):
    SiteId: str,
```

## InstancesToExcludeTypeDef

```python
# InstancesToExcludeTypeDef definition

class InstancesToExcludeTypeDef(TypedDict):
    Instances: NotRequired[Sequence[str]],
    AccountIds: NotRequired[Sequence[str]],
    Services: NotRequired[Sequence[AWSServiceNameType]],  # (1)
```

1. See [:material-code-brackets: AWSServiceNameType](./literals.md#awsservicenametype) 
## LineItemAssetInformationTypeDef

```python
# LineItemAssetInformationTypeDef definition

class LineItemAssetInformationTypeDef(TypedDict):
    AssetId: NotRequired[str],
    MacAddressList: NotRequired[List[str]],
```

## ShipmentInformationTypeDef

```python
# ShipmentInformationTypeDef definition

class ShipmentInformationTypeDef(TypedDict):
    ShipmentTrackingNumber: NotRequired[str],
    ShipmentCarrier: NotRequired[ShipmentCarrierType],  # (1)
```

1. See [:material-code-brackets: ShipmentCarrierType](./literals.md#shipmentcarriertype) 
## ListAssetInstancesInputRequestTypeDef

```python
# ListAssetInstancesInputRequestTypeDef definition

class ListAssetInstancesInputRequestTypeDef(TypedDict):
    OutpostIdentifier: str,
    AssetIdFilter: NotRequired[Sequence[str]],
    InstanceTypeFilter: NotRequired[Sequence[str]],
    AccountIdFilter: NotRequired[Sequence[str]],
    AwsServiceFilter: NotRequired[Sequence[AWSServiceNameType]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: AWSServiceNameType](./literals.md#awsservicenametype) 
## ListAssetsInputRequestTypeDef

```python
# ListAssetsInputRequestTypeDef definition

class ListAssetsInputRequestTypeDef(TypedDict):
    OutpostIdentifier: str,
    HostIdFilter: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    StatusFilter: NotRequired[Sequence[AssetStateType]],  # (1)
```

1. See [:material-code-brackets: AssetStateType](./literals.md#assetstatetype) 
## ListBlockingInstancesForCapacityTaskInputRequestTypeDef

```python
# ListBlockingInstancesForCapacityTaskInputRequestTypeDef definition

class ListBlockingInstancesForCapacityTaskInputRequestTypeDef(TypedDict):
    OutpostIdentifier: str,
    CapacityTaskId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListCapacityTasksInputRequestTypeDef

```python
# ListCapacityTasksInputRequestTypeDef definition

class ListCapacityTasksInputRequestTypeDef(TypedDict):
    OutpostIdentifierFilter: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    CapacityTaskStatusFilter: NotRequired[Sequence[CapacityTaskStatusType]],  # (1)
```

1. See [:material-code-brackets: CapacityTaskStatusType](./literals.md#capacitytaskstatustype) 
## ListCatalogItemsInputRequestTypeDef

```python
# ListCatalogItemsInputRequestTypeDef definition

class ListCatalogItemsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ItemClassFilter: NotRequired[Sequence[CatalogItemClassType]],  # (1)
    SupportedStorageFilter: NotRequired[Sequence[SupportedStorageEnumType]],  # (2)
    EC2FamilyFilter: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: CatalogItemClassType](./literals.md#catalogitemclasstype) 
2. See [:material-code-brackets: SupportedStorageEnumType](./literals.md#supportedstorageenumtype) 
## ListOrdersInputRequestTypeDef

```python
# ListOrdersInputRequestTypeDef definition

class ListOrdersInputRequestTypeDef(TypedDict):
    OutpostIdentifierFilter: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## OrderSummaryTypeDef

```python
# OrderSummaryTypeDef definition

class OrderSummaryTypeDef(TypedDict):
    OutpostId: NotRequired[str],
    OrderId: NotRequired[str],
    OrderType: NotRequired[OrderTypeType],  # (1)
    Status: NotRequired[OrderStatusType],  # (2)
    LineItemCountsByStatus: NotRequired[Dict[LineItemStatusType, int]],  # (3)
    OrderSubmissionDate: NotRequired[datetime],
    OrderFulfilledDate: NotRequired[datetime],
```

1. See [:material-code-brackets: OrderTypeType](./literals.md#ordertypetype) 
2. See [:material-code-brackets: OrderStatusType](./literals.md#orderstatustype) 
3. See [:material-code-brackets: LineItemStatusType](./literals.md#lineitemstatustype) 
## ListOutpostsInputRequestTypeDef

```python
# ListOutpostsInputRequestTypeDef definition

class ListOutpostsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    LifeCycleStatusFilter: NotRequired[Sequence[str]],
    AvailabilityZoneFilter: NotRequired[Sequence[str]],
    AvailabilityZoneIdFilter: NotRequired[Sequence[str]],
```

## ListSitesInputRequestTypeDef

```python
# ListSitesInputRequestTypeDef definition

class ListSitesInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    OperatingAddressCountryCodeFilter: NotRequired[Sequence[str]],
    OperatingAddressStateOrRegionFilter: NotRequired[Sequence[str]],
    OperatingAddressCityFilter: NotRequired[Sequence[str]],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## StartConnectionRequestRequestTypeDef

```python
# StartConnectionRequestRequestTypeDef definition

class StartConnectionRequestRequestTypeDef(TypedDict):
    AssetId: str,
    ClientPublicKey: str,
    NetworkInterfaceDeviceIndex: int,
    DeviceSerialNumber: NotRequired[str],
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

## UpdateOutpostInputRequestTypeDef

```python
# UpdateOutpostInputRequestTypeDef definition

class UpdateOutpostInputRequestTypeDef(TypedDict):
    OutpostId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    SupportedHardwareType: NotRequired[SupportedHardwareTypeType],  # (1)
```

1. See [:material-code-brackets: SupportedHardwareTypeType](./literals.md#supportedhardwaretypetype) 
## UpdateSiteInputRequestTypeDef

```python
# UpdateSiteInputRequestTypeDef definition

class UpdateSiteInputRequestTypeDef(TypedDict):
    SiteId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    Notes: NotRequired[str],
```

## UpdateSiteRackPhysicalPropertiesInputRequestTypeDef

```python
# UpdateSiteRackPhysicalPropertiesInputRequestTypeDef definition

class UpdateSiteRackPhysicalPropertiesInputRequestTypeDef(TypedDict):
    SiteId: str,
    PowerDrawKva: NotRequired[PowerDrawKvaType],  # (1)
    PowerPhase: NotRequired[PowerPhaseType],  # (2)
    PowerConnector: NotRequired[PowerConnectorType],  # (3)
    PowerFeedDrop: NotRequired[PowerFeedDropType],  # (4)
    UplinkGbps: NotRequired[UplinkGbpsType],  # (5)
    UplinkCount: NotRequired[UplinkCountType],  # (6)
    FiberOpticCableType: NotRequired[FiberOpticCableTypeType],  # (7)
    OpticalStandard: NotRequired[OpticalStandardType],  # (8)
    MaximumSupportedWeightLbs: NotRequired[MaximumSupportedWeightLbsType],  # (9)
```

1. See [:material-code-brackets: PowerDrawKvaType](./literals.md#powerdrawkvatype) 
2. See [:material-code-brackets: PowerPhaseType](./literals.md#powerphasetype) 
3. See [:material-code-brackets: PowerConnectorType](./literals.md#powerconnectortype) 
4. See [:material-code-brackets: PowerFeedDropType](./literals.md#powerfeeddroptype) 
5. See [:material-code-brackets: UplinkGbpsType](./literals.md#uplinkgbpstype) 
6. See [:material-code-brackets: UplinkCountType](./literals.md#uplinkcounttype) 
7. See [:material-code-brackets: FiberOpticCableTypeType](./literals.md#fiberopticcabletypetype) 
8. See [:material-code-brackets: OpticalStandardType](./literals.md#opticalstandardtype) 
9. See [:material-code-brackets: MaximumSupportedWeightLbsType](./literals.md#maximumsupportedweightlbstype) 
## UpdateSiteAddressInputRequestTypeDef

```python
# UpdateSiteAddressInputRequestTypeDef definition

class UpdateSiteAddressInputRequestTypeDef(TypedDict):
    SiteId: str,
    AddressType: AddressTypeType,  # (1)
    Address: AddressTypeDef,  # (2)
```

1. See [:material-code-brackets: AddressTypeType](./literals.md#addresstypetype) 
2. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
## ComputeAttributesTypeDef

```python
# ComputeAttributesTypeDef definition

class ComputeAttributesTypeDef(TypedDict):
    HostId: NotRequired[str],
    State: NotRequired[ComputeAssetStateType],  # (1)
    InstanceFamilies: NotRequired[List[str]],
    InstanceTypeCapacities: NotRequired[List[AssetInstanceTypeCapacityTypeDef]],  # (2)
    MaxVcpus: NotRequired[int],
```

1. See [:material-code-brackets: ComputeAssetStateType](./literals.md#computeassetstatetype) 
2. See [:material-code-braces: AssetInstanceTypeCapacityTypeDef](./type_defs.md#assetinstancetypecapacitytypedef) 
## CatalogItemTypeDef

```python
# CatalogItemTypeDef definition

class CatalogItemTypeDef(TypedDict):
    CatalogItemId: NotRequired[str],
    ItemStatus: NotRequired[CatalogItemStatusType],  # (1)
    EC2Capacities: NotRequired[List[EC2CapacityTypeDef]],  # (2)
    PowerKva: NotRequired[float],
    WeightLbs: NotRequired[int],
    SupportedUplinkGbps: NotRequired[List[int]],
    SupportedStorage: NotRequired[List[SupportedStorageEnumType]],  # (3)
```

1. See [:material-code-brackets: CatalogItemStatusType](./literals.md#catalogitemstatustype) 
2. See [:material-code-braces: EC2CapacityTypeDef](./type_defs.md#ec2capacitytypedef) 
3. See [:material-code-brackets: SupportedStorageEnumType](./literals.md#supportedstorageenumtype) 
## CreateOrderInputRequestTypeDef

```python
# CreateOrderInputRequestTypeDef definition

class CreateOrderInputRequestTypeDef(TypedDict):
    OutpostIdentifier: str,
    LineItems: Sequence[LineItemRequestTypeDef],  # (1)
    PaymentOption: PaymentOptionType,  # (2)
    PaymentTerm: NotRequired[PaymentTermType],  # (3)
```

1. See [:material-code-braces: LineItemRequestTypeDef](./type_defs.md#lineitemrequesttypedef) 
2. See [:material-code-brackets: PaymentOptionType](./literals.md#paymentoptiontype) 
3. See [:material-code-brackets: PaymentTermType](./literals.md#paymenttermtype) 
## GetConnectionResponseTypeDef

```python
# GetConnectionResponseTypeDef definition

class GetConnectionResponseTypeDef(TypedDict):
    ConnectionId: str,
    ConnectionDetails: ConnectionDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConnectionDetailsTypeDef](./type_defs.md#connectiondetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSiteAddressOutputTypeDef

```python
# GetSiteAddressOutputTypeDef definition

class GetSiteAddressOutputTypeDef(TypedDict):
    SiteId: str,
    AddressType: AddressTypeType,  # (1)
    Address: AddressTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AddressTypeType](./literals.md#addresstypetype) 
2. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssetInstancesOutputTypeDef

```python
# ListAssetInstancesOutputTypeDef definition

class ListAssetInstancesOutputTypeDef(TypedDict):
    AssetInstances: List[AssetInstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AssetInstanceTypeDef](./type_defs.md#assetinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBlockingInstancesForCapacityTaskOutputTypeDef

```python
# ListBlockingInstancesForCapacityTaskOutputTypeDef definition

class ListBlockingInstancesForCapacityTaskOutputTypeDef(TypedDict):
    BlockingInstances: List[BlockingInstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BlockingInstanceTypeDef](./type_defs.md#blockinginstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCapacityTasksOutputTypeDef

```python
# ListCapacityTasksOutputTypeDef definition

class ListCapacityTasksOutputTypeDef(TypedDict):
    CapacityTasks: List[CapacityTaskSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CapacityTaskSummaryTypeDef](./type_defs.md#capacitytasksummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartConnectionResponseTypeDef

```python
# StartConnectionResponseTypeDef definition

class StartConnectionResponseTypeDef(TypedDict):
    ConnectionId: str,
    UnderlayIpAddress: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSiteAddressOutputTypeDef

```python
# UpdateSiteAddressOutputTypeDef definition

class UpdateSiteAddressOutputTypeDef(TypedDict):
    AddressType: AddressTypeType,  # (1)
    Address: AddressTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AddressTypeType](./literals.md#addresstypetype) 
2. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateOutpostOutputTypeDef

```python
# CreateOutpostOutputTypeDef definition

class CreateOutpostOutputTypeDef(TypedDict):
    Outpost: OutpostTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OutpostTypeDef](./type_defs.md#outposttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOutpostOutputTypeDef

```python
# GetOutpostOutputTypeDef definition

class GetOutpostOutputTypeDef(TypedDict):
    Outpost: OutpostTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OutpostTypeDef](./type_defs.md#outposttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOutpostsOutputTypeDef

```python
# ListOutpostsOutputTypeDef definition

class ListOutpostsOutputTypeDef(TypedDict):
    Outposts: List[OutpostTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OutpostTypeDef](./type_defs.md#outposttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateOutpostOutputTypeDef

```python
# UpdateOutpostOutputTypeDef definition

class UpdateOutpostOutputTypeDef(TypedDict):
    Outpost: OutpostTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OutpostTypeDef](./type_defs.md#outposttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSiteInputRequestTypeDef

```python
# CreateSiteInputRequestTypeDef definition

class CreateSiteInputRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    Notes: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    OperatingAddress: NotRequired[AddressTypeDef],  # (1)
    ShippingAddress: NotRequired[AddressTypeDef],  # (1)
    RackPhysicalProperties: NotRequired[RackPhysicalPropertiesTypeDef],  # (3)
```

1. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
2. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
3. See [:material-code-braces: RackPhysicalPropertiesTypeDef](./type_defs.md#rackphysicalpropertiestypedef) 
## SiteTypeDef

```python
# SiteTypeDef definition

class SiteTypeDef(TypedDict):
    SiteId: NotRequired[str],
    AccountId: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
    SiteArn: NotRequired[str],
    Notes: NotRequired[str],
    OperatingAddressCountryCode: NotRequired[str],
    OperatingAddressStateOrRegion: NotRequired[str],
    OperatingAddressCity: NotRequired[str],
    RackPhysicalProperties: NotRequired[RackPhysicalPropertiesTypeDef],  # (1)
```

1. See [:material-code-braces: RackPhysicalPropertiesTypeDef](./type_defs.md#rackphysicalpropertiestypedef) 
## GetCapacityTaskOutputTypeDef

```python
# GetCapacityTaskOutputTypeDef definition

class GetCapacityTaskOutputTypeDef(TypedDict):
    CapacityTaskId: str,
    OutpostId: str,
    OrderId: str,
    RequestedInstancePools: List[InstanceTypeCapacityTypeDef],  # (1)
    InstancesToExclude: InstancesToExcludeOutputTypeDef,  # (2)
    DryRun: bool,
    CapacityTaskStatus: CapacityTaskStatusType,  # (3)
    Failed: CapacityTaskFailureTypeDef,  # (4)
    CreationDate: datetime,
    CompletionDate: datetime,
    LastModifiedDate: datetime,
    TaskActionOnBlockingInstances: TaskActionOnBlockingInstancesType,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: InstanceTypeCapacityTypeDef](./type_defs.md#instancetypecapacitytypedef) 
2. See [:material-code-braces: InstancesToExcludeOutputTypeDef](./type_defs.md#instancestoexcludeoutputtypedef) 
3. See [:material-code-brackets: CapacityTaskStatusType](./literals.md#capacitytaskstatustype) 
4. See [:material-code-braces: CapacityTaskFailureTypeDef](./type_defs.md#capacitytaskfailuretypedef) 
5. See [:material-code-brackets: TaskActionOnBlockingInstancesType](./literals.md#taskactiononblockinginstancestype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartCapacityTaskOutputTypeDef

```python
# StartCapacityTaskOutputTypeDef definition

class StartCapacityTaskOutputTypeDef(TypedDict):
    CapacityTaskId: str,
    OutpostId: str,
    OrderId: str,
    RequestedInstancePools: List[InstanceTypeCapacityTypeDef],  # (1)
    InstancesToExclude: InstancesToExcludeOutputTypeDef,  # (2)
    DryRun: bool,
    CapacityTaskStatus: CapacityTaskStatusType,  # (3)
    Failed: CapacityTaskFailureTypeDef,  # (4)
    CreationDate: datetime,
    CompletionDate: datetime,
    LastModifiedDate: datetime,
    TaskActionOnBlockingInstances: TaskActionOnBlockingInstancesType,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: InstanceTypeCapacityTypeDef](./type_defs.md#instancetypecapacitytypedef) 
2. See [:material-code-braces: InstancesToExcludeOutputTypeDef](./type_defs.md#instancestoexcludeoutputtypedef) 
3. See [:material-code-brackets: CapacityTaskStatusType](./literals.md#capacitytaskstatustype) 
4. See [:material-code-braces: CapacityTaskFailureTypeDef](./type_defs.md#capacitytaskfailuretypedef) 
5. See [:material-code-brackets: TaskActionOnBlockingInstancesType](./literals.md#taskactiononblockinginstancestype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOutpostInstanceTypesInputPaginateTypeDef

```python
# GetOutpostInstanceTypesInputPaginateTypeDef definition

class GetOutpostInstanceTypesInputPaginateTypeDef(TypedDict):
    OutpostId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetOutpostSupportedInstanceTypesInputPaginateTypeDef

```python
# GetOutpostSupportedInstanceTypesInputPaginateTypeDef definition

class GetOutpostSupportedInstanceTypesInputPaginateTypeDef(TypedDict):
    OutpostIdentifier: str,
    OrderId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssetInstancesInputPaginateTypeDef

```python
# ListAssetInstancesInputPaginateTypeDef definition

class ListAssetInstancesInputPaginateTypeDef(TypedDict):
    OutpostIdentifier: str,
    AssetIdFilter: NotRequired[Sequence[str]],
    InstanceTypeFilter: NotRequired[Sequence[str]],
    AccountIdFilter: NotRequired[Sequence[str]],
    AwsServiceFilter: NotRequired[Sequence[AWSServiceNameType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AWSServiceNameType](./literals.md#awsservicenametype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssetsInputPaginateTypeDef

```python
# ListAssetsInputPaginateTypeDef definition

class ListAssetsInputPaginateTypeDef(TypedDict):
    OutpostIdentifier: str,
    HostIdFilter: NotRequired[Sequence[str]],
    StatusFilter: NotRequired[Sequence[AssetStateType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AssetStateType](./literals.md#assetstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBlockingInstancesForCapacityTaskInputPaginateTypeDef

```python
# ListBlockingInstancesForCapacityTaskInputPaginateTypeDef definition

class ListBlockingInstancesForCapacityTaskInputPaginateTypeDef(TypedDict):
    OutpostIdentifier: str,
    CapacityTaskId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCapacityTasksInputPaginateTypeDef

```python
# ListCapacityTasksInputPaginateTypeDef definition

class ListCapacityTasksInputPaginateTypeDef(TypedDict):
    OutpostIdentifierFilter: NotRequired[str],
    CapacityTaskStatusFilter: NotRequired[Sequence[CapacityTaskStatusType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: CapacityTaskStatusType](./literals.md#capacitytaskstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCatalogItemsInputPaginateTypeDef

```python
# ListCatalogItemsInputPaginateTypeDef definition

class ListCatalogItemsInputPaginateTypeDef(TypedDict):
    ItemClassFilter: NotRequired[Sequence[CatalogItemClassType]],  # (1)
    SupportedStorageFilter: NotRequired[Sequence[SupportedStorageEnumType]],  # (2)
    EC2FamilyFilter: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: CatalogItemClassType](./literals.md#catalogitemclasstype) 
2. See [:material-code-brackets: SupportedStorageEnumType](./literals.md#supportedstorageenumtype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOrdersInputPaginateTypeDef

```python
# ListOrdersInputPaginateTypeDef definition

class ListOrdersInputPaginateTypeDef(TypedDict):
    OutpostIdentifierFilter: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOutpostsInputPaginateTypeDef

```python
# ListOutpostsInputPaginateTypeDef definition

class ListOutpostsInputPaginateTypeDef(TypedDict):
    LifeCycleStatusFilter: NotRequired[Sequence[str]],
    AvailabilityZoneFilter: NotRequired[Sequence[str]],
    AvailabilityZoneIdFilter: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSitesInputPaginateTypeDef

```python
# ListSitesInputPaginateTypeDef definition

class ListSitesInputPaginateTypeDef(TypedDict):
    OperatingAddressCountryCodeFilter: NotRequired[Sequence[str]],
    OperatingAddressStateOrRegionFilter: NotRequired[Sequence[str]],
    OperatingAddressCityFilter: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetOutpostInstanceTypesOutputTypeDef

```python
# GetOutpostInstanceTypesOutputTypeDef definition

class GetOutpostInstanceTypesOutputTypeDef(TypedDict):
    InstanceTypes: List[InstanceTypeItemTypeDef],  # (1)
    OutpostId: str,
    OutpostArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InstanceTypeItemTypeDef](./type_defs.md#instancetypeitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOutpostSupportedInstanceTypesOutputTypeDef

```python
# GetOutpostSupportedInstanceTypesOutputTypeDef definition

class GetOutpostSupportedInstanceTypesOutputTypeDef(TypedDict):
    InstanceTypes: List[InstanceTypeItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InstanceTypeItemTypeDef](./type_defs.md#instancetypeitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartCapacityTaskInputRequestTypeDef

```python
# StartCapacityTaskInputRequestTypeDef definition

class StartCapacityTaskInputRequestTypeDef(TypedDict):
    OutpostIdentifier: str,
    InstancePools: Sequence[InstanceTypeCapacityTypeDef],  # (1)
    OrderId: NotRequired[str],
    InstancesToExclude: NotRequired[InstancesToExcludeTypeDef],  # (2)
    DryRun: NotRequired[bool],
    TaskActionOnBlockingInstances: NotRequired[TaskActionOnBlockingInstancesType],  # (3)
```

1. See [:material-code-braces: InstanceTypeCapacityTypeDef](./type_defs.md#instancetypecapacitytypedef) 
2. See [:material-code-braces: InstancesToExcludeTypeDef](./type_defs.md#instancestoexcludetypedef) 
3. See [:material-code-brackets: TaskActionOnBlockingInstancesType](./literals.md#taskactiononblockinginstancestype) 
## LineItemTypeDef

```python
# LineItemTypeDef definition

class LineItemTypeDef(TypedDict):
    CatalogItemId: NotRequired[str],
    LineItemId: NotRequired[str],
    Quantity: NotRequired[int],
    Status: NotRequired[LineItemStatusType],  # (1)
    ShipmentInformation: NotRequired[ShipmentInformationTypeDef],  # (2)
    AssetInformationList: NotRequired[List[LineItemAssetInformationTypeDef]],  # (3)
    PreviousLineItemId: NotRequired[str],
    PreviousOrderId: NotRequired[str],
```

1. See [:material-code-brackets: LineItemStatusType](./literals.md#lineitemstatustype) 
2. See [:material-code-braces: ShipmentInformationTypeDef](./type_defs.md#shipmentinformationtypedef) 
3. See [:material-code-braces: LineItemAssetInformationTypeDef](./type_defs.md#lineitemassetinformationtypedef) 
## ListOrdersOutputTypeDef

```python
# ListOrdersOutputTypeDef definition

class ListOrdersOutputTypeDef(TypedDict):
    Orders: List[OrderSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OrderSummaryTypeDef](./type_defs.md#ordersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssetInfoTypeDef

```python
# AssetInfoTypeDef definition

class AssetInfoTypeDef(TypedDict):
    AssetId: NotRequired[str],
    RackId: NotRequired[str],
    AssetType: NotRequired[AssetTypeType],  # (1)
    ComputeAttributes: NotRequired[ComputeAttributesTypeDef],  # (2)
    AssetLocation: NotRequired[AssetLocationTypeDef],  # (3)
```

1. See [:material-code-brackets: AssetTypeType](./literals.md#assettypetype) 
2. See [:material-code-braces: ComputeAttributesTypeDef](./type_defs.md#computeattributestypedef) 
3. See [:material-code-braces: AssetLocationTypeDef](./type_defs.md#assetlocationtypedef) 
## GetCatalogItemOutputTypeDef

```python
# GetCatalogItemOutputTypeDef definition

class GetCatalogItemOutputTypeDef(TypedDict):
    CatalogItem: CatalogItemTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CatalogItemTypeDef](./type_defs.md#catalogitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCatalogItemsOutputTypeDef

```python
# ListCatalogItemsOutputTypeDef definition

class ListCatalogItemsOutputTypeDef(TypedDict):
    CatalogItems: List[CatalogItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CatalogItemTypeDef](./type_defs.md#catalogitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSiteOutputTypeDef

```python
# CreateSiteOutputTypeDef definition

class CreateSiteOutputTypeDef(TypedDict):
    Site: SiteTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SiteTypeDef](./type_defs.md#sitetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSiteOutputTypeDef

```python
# GetSiteOutputTypeDef definition

class GetSiteOutputTypeDef(TypedDict):
    Site: SiteTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SiteTypeDef](./type_defs.md#sitetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSitesOutputTypeDef

```python
# ListSitesOutputTypeDef definition

class ListSitesOutputTypeDef(TypedDict):
    Sites: List[SiteTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SiteTypeDef](./type_defs.md#sitetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSiteOutputTypeDef

```python
# UpdateSiteOutputTypeDef definition

class UpdateSiteOutputTypeDef(TypedDict):
    Site: SiteTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SiteTypeDef](./type_defs.md#sitetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSiteRackPhysicalPropertiesOutputTypeDef

```python
# UpdateSiteRackPhysicalPropertiesOutputTypeDef definition

class UpdateSiteRackPhysicalPropertiesOutputTypeDef(TypedDict):
    Site: SiteTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SiteTypeDef](./type_defs.md#sitetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OrderTypeDef

```python
# OrderTypeDef definition

class OrderTypeDef(TypedDict):
    OutpostId: NotRequired[str],
    OrderId: NotRequired[str],
    Status: NotRequired[OrderStatusType],  # (1)
    LineItems: NotRequired[List[LineItemTypeDef]],  # (2)
    PaymentOption: NotRequired[PaymentOptionType],  # (3)
    OrderSubmissionDate: NotRequired[datetime],
    OrderFulfilledDate: NotRequired[datetime],
    PaymentTerm: NotRequired[PaymentTermType],  # (4)
    OrderType: NotRequired[OrderTypeType],  # (5)
```

1. See [:material-code-brackets: OrderStatusType](./literals.md#orderstatustype) 
2. See [:material-code-braces: LineItemTypeDef](./type_defs.md#lineitemtypedef) 
3. See [:material-code-brackets: PaymentOptionType](./literals.md#paymentoptiontype) 
4. See [:material-code-brackets: PaymentTermType](./literals.md#paymenttermtype) 
5. See [:material-code-brackets: OrderTypeType](./literals.md#ordertypetype) 
## ListAssetsOutputTypeDef

```python
# ListAssetsOutputTypeDef definition

class ListAssetsOutputTypeDef(TypedDict):
    Assets: List[AssetInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AssetInfoTypeDef](./type_defs.md#assetinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateOrderOutputTypeDef

```python
# CreateOrderOutputTypeDef definition

class CreateOrderOutputTypeDef(TypedDict):
    Order: OrderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrderTypeDef](./type_defs.md#ordertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOrderOutputTypeDef

```python
# GetOrderOutputTypeDef definition

class GetOrderOutputTypeDef(TypedDict):
    Order: OrderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrderTypeDef](./type_defs.md#ordertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
