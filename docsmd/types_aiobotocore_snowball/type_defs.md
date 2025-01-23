# Type definitions

> [Index](../README.md) > [Snowball](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Snowball](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#snowball)
    type annotations stubs module [types-aiobotocore-snowball](https://pypi.org/project/types-aiobotocore-snowball/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## LambdaResourceUnionTypeDef

```python
# LambdaResourceUnionTypeDef definition

LambdaResourceUnionTypeDef = Union[
    LambdaResourceTypeDef,  # (1)
    LambdaResourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: LambdaResourceTypeDef](./type_defs.md#lambdaresourcetypedef) 
2. See [:material-code-braces: LambdaResourceOutputTypeDef](./type_defs.md#lambdaresourceoutputtypedef) 

## S3ResourceUnionTypeDef

```python
# S3ResourceUnionTypeDef definition

S3ResourceUnionTypeDef = Union[
    S3ResourceTypeDef,  # (1)
    S3ResourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: S3ResourceTypeDef](./type_defs.md#s3resourcetypedef) 
2. See [:material-code-braces: S3ResourceOutputTypeDef](./type_defs.md#s3resourceoutputtypedef) 



## AddressTypeDef

```python
# AddressTypeDef definition

class AddressTypeDef(TypedDict):
    AddressId: NotRequired[str],
    Name: NotRequired[str],
    Company: NotRequired[str],
    Street1: NotRequired[str],
    Street2: NotRequired[str],
    Street3: NotRequired[str],
    City: NotRequired[str],
    StateOrProvince: NotRequired[str],
    PrefectureOrDistrict: NotRequired[str],
    Landmark: NotRequired[str],
    Country: NotRequired[str],
    PostalCode: NotRequired[str],
    PhoneNumber: NotRequired[str],
    IsRestricted: NotRequired[bool],
    Type: NotRequired[AddressTypeType],  # (1)
```

1. See [:material-code-brackets: AddressTypeType](./literals.md#addresstypetype) 
## CancelClusterRequestRequestTypeDef

```python
# CancelClusterRequestRequestTypeDef definition

class CancelClusterRequestRequestTypeDef(TypedDict):
    ClusterId: str,
```

## CancelJobRequestRequestTypeDef

```python
# CancelJobRequestRequestTypeDef definition

class CancelJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## ClusterListEntryTypeDef

```python
# ClusterListEntryTypeDef definition

class ClusterListEntryTypeDef(TypedDict):
    ClusterId: NotRequired[str],
    ClusterState: NotRequired[ClusterStateType],  # (1)
    CreationDate: NotRequired[datetime],
    Description: NotRequired[str],
```

1. See [:material-code-brackets: ClusterStateType](./literals.md#clusterstatetype) 
## NotificationOutputTypeDef

```python
# NotificationOutputTypeDef definition

class NotificationOutputTypeDef(TypedDict):
    SnsTopicARN: NotRequired[str],
    JobStatesToNotify: NotRequired[List[JobStateType]],  # (1)
    NotifyAll: NotRequired[bool],
    DevicePickupSnsTopicARN: NotRequired[str],
```

1. See [:material-code-brackets: JobStateType](./literals.md#jobstatetype) 
## CompatibleImageTypeDef

```python
# CompatibleImageTypeDef definition

class CompatibleImageTypeDef(TypedDict):
    AmiId: NotRequired[str],
    Name: NotRequired[str],
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

## NotificationTypeDef

```python
# NotificationTypeDef definition

class NotificationTypeDef(TypedDict):
    SnsTopicARN: NotRequired[str],
    JobStatesToNotify: NotRequired[Sequence[JobStateType]],  # (1)
    NotifyAll: NotRequired[bool],
    DevicePickupSnsTopicARN: NotRequired[str],
```

1. See [:material-code-brackets: JobStateType](./literals.md#jobstatetype) 
## JobListEntryTypeDef

```python
# JobListEntryTypeDef definition

class JobListEntryTypeDef(TypedDict):
    JobId: NotRequired[str],
    JobState: NotRequired[JobStateType],  # (1)
    IsMaster: NotRequired[bool],
    JobType: NotRequired[JobTypeType],  # (2)
    SnowballType: NotRequired[SnowballTypeType],  # (3)
    CreationDate: NotRequired[datetime],
    Description: NotRequired[str],
```

1. See [:material-code-brackets: JobStateType](./literals.md#jobstatetype) 
2. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
3. See [:material-code-brackets: SnowballTypeType](./literals.md#snowballtypetype) 
## CreateLongTermPricingRequestRequestTypeDef

```python
# CreateLongTermPricingRequestRequestTypeDef definition

class CreateLongTermPricingRequestRequestTypeDef(TypedDict):
    LongTermPricingType: LongTermPricingTypeType,  # (1)
    SnowballType: SnowballTypeType,  # (2)
    IsLongTermPricingAutoRenew: NotRequired[bool],
```

1. See [:material-code-brackets: LongTermPricingTypeType](./literals.md#longtermpricingtypetype) 
2. See [:material-code-brackets: SnowballTypeType](./literals.md#snowballtypetype) 
## CreateReturnShippingLabelRequestRequestTypeDef

```python
# CreateReturnShippingLabelRequestRequestTypeDef definition

class CreateReturnShippingLabelRequestRequestTypeDef(TypedDict):
    JobId: str,
    ShippingOption: NotRequired[ShippingOptionType],  # (1)
```

1. See [:material-code-brackets: ShippingOptionType](./literals.md#shippingoptiontype) 
## DataTransferTypeDef

```python
# DataTransferTypeDef definition

class DataTransferTypeDef(TypedDict):
    BytesTransferred: NotRequired[int],
    ObjectsTransferred: NotRequired[int],
    TotalBytes: NotRequired[int],
    TotalObjects: NotRequired[int],
```

## ServiceVersionTypeDef

```python
# ServiceVersionTypeDef definition

class ServiceVersionTypeDef(TypedDict):
    Version: NotRequired[str],
```

## DescribeAddressRequestRequestTypeDef

```python
# DescribeAddressRequestRequestTypeDef definition

class DescribeAddressRequestRequestTypeDef(TypedDict):
    AddressId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeAddressesRequestRequestTypeDef

```python
# DescribeAddressesRequestRequestTypeDef definition

class DescribeAddressesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeClusterRequestRequestTypeDef

```python
# DescribeClusterRequestRequestTypeDef definition

class DescribeClusterRequestRequestTypeDef(TypedDict):
    ClusterId: str,
```

## DescribeJobRequestRequestTypeDef

```python
# DescribeJobRequestRequestTypeDef definition

class DescribeJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## DescribeReturnShippingLabelRequestRequestTypeDef

```python
# DescribeReturnShippingLabelRequestRequestTypeDef definition

class DescribeReturnShippingLabelRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## EKSOnDeviceServiceConfigurationTypeDef

```python
# EKSOnDeviceServiceConfigurationTypeDef definition

class EKSOnDeviceServiceConfigurationTypeDef(TypedDict):
    KubernetesVersion: NotRequired[str],
    EKSAnywhereVersion: NotRequired[str],
```

## Ec2AmiResourceTypeDef

```python
# Ec2AmiResourceTypeDef definition

class Ec2AmiResourceTypeDef(TypedDict):
    AmiId: str,
    SnowballAmiId: NotRequired[str],
```

## EventTriggerDefinitionTypeDef

```python
# EventTriggerDefinitionTypeDef definition

class EventTriggerDefinitionTypeDef(TypedDict):
    EventResourceARN: NotRequired[str],
```

## GetJobManifestRequestRequestTypeDef

```python
# GetJobManifestRequestRequestTypeDef definition

class GetJobManifestRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## GetJobUnlockCodeRequestRequestTypeDef

```python
# GetJobUnlockCodeRequestRequestTypeDef definition

class GetJobUnlockCodeRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## GetSoftwareUpdatesRequestRequestTypeDef

```python
# GetSoftwareUpdatesRequestRequestTypeDef definition

class GetSoftwareUpdatesRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## INDTaxDocumentsTypeDef

```python
# INDTaxDocumentsTypeDef definition

class INDTaxDocumentsTypeDef(TypedDict):
    GSTIN: NotRequired[str],
```

## JobLogsTypeDef

```python
# JobLogsTypeDef definition

class JobLogsTypeDef(TypedDict):
    JobCompletionReportURI: NotRequired[str],
    JobSuccessLogURI: NotRequired[str],
    JobFailureLogURI: NotRequired[str],
```

## PickupDetailsOutputTypeDef

```python
# PickupDetailsOutputTypeDef definition

class PickupDetailsOutputTypeDef(TypedDict):
    Name: NotRequired[str],
    PhoneNumber: NotRequired[str],
    Email: NotRequired[str],
    IdentificationNumber: NotRequired[str],
    IdentificationExpirationDate: NotRequired[datetime],
    IdentificationIssuingOrg: NotRequired[str],
    DevicePickupId: NotRequired[str],
```

## KeyRangeTypeDef

```python
# KeyRangeTypeDef definition

class KeyRangeTypeDef(TypedDict):
    BeginMarker: NotRequired[str],
    EndMarker: NotRequired[str],
```

## ListClusterJobsRequestRequestTypeDef

```python
# ListClusterJobsRequestRequestTypeDef definition

class ListClusterJobsRequestRequestTypeDef(TypedDict):
    ClusterId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListClustersRequestRequestTypeDef

```python
# ListClustersRequestRequestTypeDef definition

class ListClustersRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListCompatibleImagesRequestRequestTypeDef

```python
# ListCompatibleImagesRequestRequestTypeDef definition

class ListCompatibleImagesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListJobsRequestRequestTypeDef

```python
# ListJobsRequestRequestTypeDef definition

class ListJobsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListLongTermPricingRequestRequestTypeDef

```python
# ListLongTermPricingRequestRequestTypeDef definition

class ListLongTermPricingRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## LongTermPricingListEntryTypeDef

```python
# LongTermPricingListEntryTypeDef definition

class LongTermPricingListEntryTypeDef(TypedDict):
    LongTermPricingId: NotRequired[str],
    LongTermPricingEndDate: NotRequired[datetime],
    LongTermPricingStartDate: NotRequired[datetime],
    LongTermPricingType: NotRequired[LongTermPricingTypeType],  # (1)
    CurrentActiveJob: NotRequired[str],
    ReplacementJob: NotRequired[str],
    IsLongTermPricingAutoRenew: NotRequired[bool],
    LongTermPricingStatus: NotRequired[str],
    SnowballType: NotRequired[SnowballTypeType],  # (2)
    JobIds: NotRequired[List[str]],
```

1. See [:material-code-brackets: LongTermPricingTypeType](./literals.md#longtermpricingtypetype) 
2. See [:material-code-brackets: SnowballTypeType](./literals.md#snowballtypetype) 
## ListPickupLocationsRequestRequestTypeDef

```python
# ListPickupLocationsRequestRequestTypeDef definition

class ListPickupLocationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## NFSOnDeviceServiceConfigurationTypeDef

```python
# NFSOnDeviceServiceConfigurationTypeDef definition

class NFSOnDeviceServiceConfigurationTypeDef(TypedDict):
    StorageLimit: NotRequired[int],
    StorageUnit: NotRequired[StorageUnitType],  # (1)
```

1. See [:material-code-brackets: StorageUnitType](./literals.md#storageunittype) 
## S3OnDeviceServiceConfigurationTypeDef

```python
# S3OnDeviceServiceConfigurationTypeDef definition

class S3OnDeviceServiceConfigurationTypeDef(TypedDict):
    StorageLimit: NotRequired[float],
    StorageUnit: NotRequired[StorageUnitType],  # (1)
    ServiceSize: NotRequired[int],
    FaultTolerance: NotRequired[int],
```

1. See [:material-code-brackets: StorageUnitType](./literals.md#storageunittype) 
## TGWOnDeviceServiceConfigurationTypeDef

```python
# TGWOnDeviceServiceConfigurationTypeDef definition

class TGWOnDeviceServiceConfigurationTypeDef(TypedDict):
    StorageLimit: NotRequired[int],
    StorageUnit: NotRequired[StorageUnitType],  # (1)
```

1. See [:material-code-brackets: StorageUnitType](./literals.md#storageunittype) 
## TargetOnDeviceServiceTypeDef

```python
# TargetOnDeviceServiceTypeDef definition

class TargetOnDeviceServiceTypeDef(TypedDict):
    ServiceName: NotRequired[DeviceServiceNameType],  # (1)
    TransferOption: NotRequired[TransferOptionType],  # (2)
```

1. See [:material-code-brackets: DeviceServiceNameType](./literals.md#deviceservicenametype) 
2. See [:material-code-brackets: TransferOptionType](./literals.md#transferoptiontype) 
## ShipmentTypeDef

```python
# ShipmentTypeDef definition

class ShipmentTypeDef(TypedDict):
    Status: NotRequired[str],
    TrackingNumber: NotRequired[str],
```

## WirelessConnectionTypeDef

```python
# WirelessConnectionTypeDef definition

class WirelessConnectionTypeDef(TypedDict):
    IsWifiEnabled: NotRequired[bool],
```

## UpdateJobShipmentStateRequestRequestTypeDef

```python
# UpdateJobShipmentStateRequestRequestTypeDef definition

class UpdateJobShipmentStateRequestRequestTypeDef(TypedDict):
    JobId: str,
    ShipmentState: ShipmentStateType,  # (1)
```

1. See [:material-code-brackets: ShipmentStateType](./literals.md#shipmentstatetype) 
## UpdateLongTermPricingRequestRequestTypeDef

```python
# UpdateLongTermPricingRequestRequestTypeDef definition

class UpdateLongTermPricingRequestRequestTypeDef(TypedDict):
    LongTermPricingId: str,
    ReplacementJob: NotRequired[str],
    IsLongTermPricingAutoRenew: NotRequired[bool],
```

## CreateAddressRequestRequestTypeDef

```python
# CreateAddressRequestRequestTypeDef definition

class CreateAddressRequestRequestTypeDef(TypedDict):
    Address: AddressTypeDef,  # (1)
```

1. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
## CreateAddressResultTypeDef

```python
# CreateAddressResultTypeDef definition

class CreateAddressResultTypeDef(TypedDict):
    AddressId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobResultTypeDef

```python
# CreateJobResultTypeDef definition

class CreateJobResultTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLongTermPricingResultTypeDef

```python
# CreateLongTermPricingResultTypeDef definition

class CreateLongTermPricingResultTypeDef(TypedDict):
    LongTermPricingId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateReturnShippingLabelResultTypeDef

```python
# CreateReturnShippingLabelResultTypeDef definition

class CreateReturnShippingLabelResultTypeDef(TypedDict):
    Status: ShippingLabelStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ShippingLabelStatusType](./literals.md#shippinglabelstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAddressResultTypeDef

```python
# DescribeAddressResultTypeDef definition

class DescribeAddressResultTypeDef(TypedDict):
    Address: AddressTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAddressesResultTypeDef

```python
# DescribeAddressesResultTypeDef definition

class DescribeAddressesResultTypeDef(TypedDict):
    Addresses: List[AddressTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeReturnShippingLabelResultTypeDef

```python
# DescribeReturnShippingLabelResultTypeDef definition

class DescribeReturnShippingLabelResultTypeDef(TypedDict):
    Status: ShippingLabelStatusType,  # (1)
    ExpirationDate: datetime,
    ReturnShippingLabelURI: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ShippingLabelStatusType](./literals.md#shippinglabelstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJobManifestResultTypeDef

```python
# GetJobManifestResultTypeDef definition

class GetJobManifestResultTypeDef(TypedDict):
    ManifestURI: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJobUnlockCodeResultTypeDef

```python
# GetJobUnlockCodeResultTypeDef definition

class GetJobUnlockCodeResultTypeDef(TypedDict):
    UnlockCode: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSnowballUsageResultTypeDef

```python
# GetSnowballUsageResultTypeDef definition

class GetSnowballUsageResultTypeDef(TypedDict):
    SnowballLimit: int,
    SnowballsInUse: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSoftwareUpdatesResultTypeDef

```python
# GetSoftwareUpdatesResultTypeDef definition

class GetSoftwareUpdatesResultTypeDef(TypedDict):
    UpdatesURI: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListClustersResultTypeDef

```python
# ListClustersResultTypeDef definition

class ListClustersResultTypeDef(TypedDict):
    ClusterListEntries: List[ClusterListEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ClusterListEntryTypeDef](./type_defs.md#clusterlistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCompatibleImagesResultTypeDef

```python
# ListCompatibleImagesResultTypeDef definition

class ListCompatibleImagesResultTypeDef(TypedDict):
    CompatibleImages: List[CompatibleImageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CompatibleImageTypeDef](./type_defs.md#compatibleimagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPickupLocationsResultTypeDef

```python
# ListPickupLocationsResultTypeDef definition

class ListPickupLocationsResultTypeDef(TypedDict):
    Addresses: List[AddressTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateClusterResultTypeDef

```python
# CreateClusterResultTypeDef definition

class CreateClusterResultTypeDef(TypedDict):
    ClusterId: str,
    JobListEntries: List[JobListEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobListEntryTypeDef](./type_defs.md#joblistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListClusterJobsResultTypeDef

```python
# ListClusterJobsResultTypeDef definition

class ListClusterJobsResultTypeDef(TypedDict):
    JobListEntries: List[JobListEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: JobListEntryTypeDef](./type_defs.md#joblistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJobsResultTypeDef

```python
# ListJobsResultTypeDef definition

class ListJobsResultTypeDef(TypedDict):
    JobListEntries: List[JobListEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: JobListEntryTypeDef](./type_defs.md#joblistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DependentServiceTypeDef

```python
# DependentServiceTypeDef definition

class DependentServiceTypeDef(TypedDict):
    ServiceName: NotRequired[ServiceNameType],  # (1)
    ServiceVersion: NotRequired[ServiceVersionTypeDef],  # (2)
```

1. See [:material-code-brackets: ServiceNameType](./literals.md#servicenametype) 
2. See [:material-code-braces: ServiceVersionTypeDef](./type_defs.md#serviceversiontypedef) 
## DescribeAddressesRequestPaginateTypeDef

```python
# DescribeAddressesRequestPaginateTypeDef definition

class DescribeAddressesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListClusterJobsRequestPaginateTypeDef

```python
# ListClusterJobsRequestPaginateTypeDef definition

class ListClusterJobsRequestPaginateTypeDef(TypedDict):
    ClusterId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListClustersRequestPaginateTypeDef

```python
# ListClustersRequestPaginateTypeDef definition

class ListClustersRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCompatibleImagesRequestPaginateTypeDef

```python
# ListCompatibleImagesRequestPaginateTypeDef definition

class ListCompatibleImagesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobsRequestPaginateTypeDef

```python
# ListJobsRequestPaginateTypeDef definition

class ListJobsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLongTermPricingRequestPaginateTypeDef

```python
# ListLongTermPricingRequestPaginateTypeDef definition

class ListLongTermPricingRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## LambdaResourceOutputTypeDef

```python
# LambdaResourceOutputTypeDef definition

class LambdaResourceOutputTypeDef(TypedDict):
    LambdaArn: NotRequired[str],
    EventTriggers: NotRequired[List[EventTriggerDefinitionTypeDef]],  # (1)
```

1. See [:material-code-braces: EventTriggerDefinitionTypeDef](./type_defs.md#eventtriggerdefinitiontypedef) 
## LambdaResourceTypeDef

```python
# LambdaResourceTypeDef definition

class LambdaResourceTypeDef(TypedDict):
    LambdaArn: NotRequired[str],
    EventTriggers: NotRequired[Sequence[EventTriggerDefinitionTypeDef]],  # (1)
```

1. See [:material-code-braces: EventTriggerDefinitionTypeDef](./type_defs.md#eventtriggerdefinitiontypedef) 
## TaxDocumentsTypeDef

```python
# TaxDocumentsTypeDef definition

class TaxDocumentsTypeDef(TypedDict):
    IND: NotRequired[INDTaxDocumentsTypeDef],  # (1)
```

1. See [:material-code-braces: INDTaxDocumentsTypeDef](./type_defs.md#indtaxdocumentstypedef) 
## ListLongTermPricingResultTypeDef

```python
# ListLongTermPricingResultTypeDef definition

class ListLongTermPricingResultTypeDef(TypedDict):
    LongTermPricingEntries: List[LongTermPricingListEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LongTermPricingListEntryTypeDef](./type_defs.md#longtermpricinglistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OnDeviceServiceConfigurationTypeDef

```python
# OnDeviceServiceConfigurationTypeDef definition

class OnDeviceServiceConfigurationTypeDef(TypedDict):
    NFSOnDeviceService: NotRequired[NFSOnDeviceServiceConfigurationTypeDef],  # (1)
    TGWOnDeviceService: NotRequired[TGWOnDeviceServiceConfigurationTypeDef],  # (2)
    EKSOnDeviceService: NotRequired[EKSOnDeviceServiceConfigurationTypeDef],  # (3)
    S3OnDeviceService: NotRequired[S3OnDeviceServiceConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: NFSOnDeviceServiceConfigurationTypeDef](./type_defs.md#nfsondeviceserviceconfigurationtypedef) 
2. See [:material-code-braces: TGWOnDeviceServiceConfigurationTypeDef](./type_defs.md#tgwondeviceserviceconfigurationtypedef) 
3. See [:material-code-braces: EKSOnDeviceServiceConfigurationTypeDef](./type_defs.md#eksondeviceserviceconfigurationtypedef) 
4. See [:material-code-braces: S3OnDeviceServiceConfigurationTypeDef](./type_defs.md#s3ondeviceserviceconfigurationtypedef) 
## PickupDetailsTypeDef

```python
# PickupDetailsTypeDef definition

class PickupDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    PhoneNumber: NotRequired[str],
    Email: NotRequired[str],
    IdentificationNumber: NotRequired[str],
    IdentificationExpirationDate: NotRequired[TimestampTypeDef],
    IdentificationIssuingOrg: NotRequired[str],
    DevicePickupId: NotRequired[str],
```

## S3ResourceOutputTypeDef

```python
# S3ResourceOutputTypeDef definition

class S3ResourceOutputTypeDef(TypedDict):
    BucketArn: NotRequired[str],
    KeyRange: NotRequired[KeyRangeTypeDef],  # (1)
    TargetOnDeviceServices: NotRequired[List[TargetOnDeviceServiceTypeDef]],  # (2)
```

1. See [:material-code-braces: KeyRangeTypeDef](./type_defs.md#keyrangetypedef) 
2. See [:material-code-braces: TargetOnDeviceServiceTypeDef](./type_defs.md#targetondeviceservicetypedef) 
## S3ResourceTypeDef

```python
# S3ResourceTypeDef definition

class S3ResourceTypeDef(TypedDict):
    BucketArn: NotRequired[str],
    KeyRange: NotRequired[KeyRangeTypeDef],  # (1)
    TargetOnDeviceServices: NotRequired[Sequence[TargetOnDeviceServiceTypeDef]],  # (2)
```

1. See [:material-code-braces: KeyRangeTypeDef](./type_defs.md#keyrangetypedef) 
2. See [:material-code-braces: TargetOnDeviceServiceTypeDef](./type_defs.md#targetondeviceservicetypedef) 
## ShippingDetailsTypeDef

```python
# ShippingDetailsTypeDef definition

class ShippingDetailsTypeDef(TypedDict):
    ShippingOption: NotRequired[ShippingOptionType],  # (1)
    InboundShipment: NotRequired[ShipmentTypeDef],  # (2)
    OutboundShipment: NotRequired[ShipmentTypeDef],  # (2)
```

1. See [:material-code-brackets: ShippingOptionType](./literals.md#shippingoptiontype) 
2. See [:material-code-braces: ShipmentTypeDef](./type_defs.md#shipmenttypedef) 
3. See [:material-code-braces: ShipmentTypeDef](./type_defs.md#shipmenttypedef) 
## SnowconeDeviceConfigurationTypeDef

```python
# SnowconeDeviceConfigurationTypeDef definition

class SnowconeDeviceConfigurationTypeDef(TypedDict):
    WirelessConnection: NotRequired[WirelessConnectionTypeDef],  # (1)
```

1. See [:material-code-braces: WirelessConnectionTypeDef](./type_defs.md#wirelessconnectiontypedef) 
## ListServiceVersionsRequestRequestTypeDef

```python
# ListServiceVersionsRequestRequestTypeDef definition

class ListServiceVersionsRequestRequestTypeDef(TypedDict):
    ServiceName: ServiceNameType,  # (1)
    DependentServices: NotRequired[Sequence[DependentServiceTypeDef]],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ServiceNameType](./literals.md#servicenametype) 
2. See [:material-code-braces: DependentServiceTypeDef](./type_defs.md#dependentservicetypedef) 
## ListServiceVersionsResultTypeDef

```python
# ListServiceVersionsResultTypeDef definition

class ListServiceVersionsResultTypeDef(TypedDict):
    ServiceVersions: List[ServiceVersionTypeDef],  # (1)
    ServiceName: ServiceNameType,  # (2)
    DependentServices: List[DependentServiceTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceVersionTypeDef](./type_defs.md#serviceversiontypedef) 
2. See [:material-code-brackets: ServiceNameType](./literals.md#servicenametype) 
3. See [:material-code-braces: DependentServiceTypeDef](./type_defs.md#dependentservicetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JobResourceOutputTypeDef

```python
# JobResourceOutputTypeDef definition

class JobResourceOutputTypeDef(TypedDict):
    S3Resources: NotRequired[List[S3ResourceOutputTypeDef]],  # (1)
    LambdaResources: NotRequired[List[LambdaResourceOutputTypeDef]],  # (2)
    Ec2AmiResources: NotRequired[List[Ec2AmiResourceTypeDef]],  # (3)
```

1. See [:material-code-braces: S3ResourceOutputTypeDef](./type_defs.md#s3resourceoutputtypedef) 
2. See [:material-code-braces: LambdaResourceOutputTypeDef](./type_defs.md#lambdaresourceoutputtypedef) 
3. See [:material-code-braces: Ec2AmiResourceTypeDef](./type_defs.md#ec2amiresourcetypedef) 
## DeviceConfigurationTypeDef

```python
# DeviceConfigurationTypeDef definition

class DeviceConfigurationTypeDef(TypedDict):
    SnowconeDeviceConfiguration: NotRequired[SnowconeDeviceConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: SnowconeDeviceConfigurationTypeDef](./type_defs.md#snowconedeviceconfigurationtypedef) 
## ClusterMetadataTypeDef

```python
# ClusterMetadataTypeDef definition

class ClusterMetadataTypeDef(TypedDict):
    ClusterId: NotRequired[str],
    Description: NotRequired[str],
    KmsKeyARN: NotRequired[str],
    RoleARN: NotRequired[str],
    ClusterState: NotRequired[ClusterStateType],  # (1)
    JobType: NotRequired[JobTypeType],  # (2)
    SnowballType: NotRequired[SnowballTypeType],  # (3)
    CreationDate: NotRequired[datetime],
    Resources: NotRequired[JobResourceOutputTypeDef],  # (4)
    AddressId: NotRequired[str],
    ShippingOption: NotRequired[ShippingOptionType],  # (5)
    Notification: NotRequired[NotificationOutputTypeDef],  # (6)
    ForwardingAddressId: NotRequired[str],
    TaxDocuments: NotRequired[TaxDocumentsTypeDef],  # (7)
    OnDeviceServiceConfiguration: NotRequired[OnDeviceServiceConfigurationTypeDef],  # (8)
```

1. See [:material-code-brackets: ClusterStateType](./literals.md#clusterstatetype) 
2. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
3. See [:material-code-brackets: SnowballTypeType](./literals.md#snowballtypetype) 
4. See [:material-code-braces: JobResourceOutputTypeDef](./type_defs.md#jobresourceoutputtypedef) 
5. See [:material-code-brackets: ShippingOptionType](./literals.md#shippingoptiontype) 
6. See [:material-code-braces: NotificationOutputTypeDef](./type_defs.md#notificationoutputtypedef) 
7. See [:material-code-braces: TaxDocumentsTypeDef](./type_defs.md#taxdocumentstypedef) 
8. See [:material-code-braces: OnDeviceServiceConfigurationTypeDef](./type_defs.md#ondeviceserviceconfigurationtypedef) 
## JobResourceTypeDef

```python
# JobResourceTypeDef definition

class JobResourceTypeDef(TypedDict):
    S3Resources: NotRequired[Sequence[S3ResourceUnionTypeDef]],  # (1)
    LambdaResources: NotRequired[Sequence[LambdaResourceUnionTypeDef]],  # (2)
    Ec2AmiResources: NotRequired[Sequence[Ec2AmiResourceTypeDef]],  # (3)
```

1. See [:material-code-braces: S3ResourceTypeDef](./type_defs.md#s3resourcetypedef) [:material-code-braces: S3ResourceOutputTypeDef](./type_defs.md#s3resourceoutputtypedef) 
2. See [:material-code-braces: LambdaResourceTypeDef](./type_defs.md#lambdaresourcetypedef) [:material-code-braces: LambdaResourceOutputTypeDef](./type_defs.md#lambdaresourceoutputtypedef) 
3. See [:material-code-braces: Ec2AmiResourceTypeDef](./type_defs.md#ec2amiresourcetypedef) 
## JobMetadataTypeDef

```python
# JobMetadataTypeDef definition

class JobMetadataTypeDef(TypedDict):
    JobId: NotRequired[str],
    JobState: NotRequired[JobStateType],  # (1)
    JobType: NotRequired[JobTypeType],  # (2)
    SnowballType: NotRequired[SnowballTypeType],  # (3)
    CreationDate: NotRequired[datetime],
    Resources: NotRequired[JobResourceOutputTypeDef],  # (4)
    Description: NotRequired[str],
    KmsKeyARN: NotRequired[str],
    RoleARN: NotRequired[str],
    AddressId: NotRequired[str],
    ShippingDetails: NotRequired[ShippingDetailsTypeDef],  # (5)
    SnowballCapacityPreference: NotRequired[SnowballCapacityType],  # (6)
    Notification: NotRequired[NotificationOutputTypeDef],  # (7)
    DataTransferProgress: NotRequired[DataTransferTypeDef],  # (8)
    JobLogInfo: NotRequired[JobLogsTypeDef],  # (9)
    ClusterId: NotRequired[str],
    ForwardingAddressId: NotRequired[str],
    TaxDocuments: NotRequired[TaxDocumentsTypeDef],  # (10)
    DeviceConfiguration: NotRequired[DeviceConfigurationTypeDef],  # (11)
    RemoteManagement: NotRequired[RemoteManagementType],  # (12)
    LongTermPricingId: NotRequired[str],
    OnDeviceServiceConfiguration: NotRequired[OnDeviceServiceConfigurationTypeDef],  # (13)
    ImpactLevel: NotRequired[ImpactLevelType],  # (14)
    PickupDetails: NotRequired[PickupDetailsOutputTypeDef],  # (15)
    SnowballId: NotRequired[str],
```

1. See [:material-code-brackets: JobStateType](./literals.md#jobstatetype) 
2. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
3. See [:material-code-brackets: SnowballTypeType](./literals.md#snowballtypetype) 
4. See [:material-code-braces: JobResourceOutputTypeDef](./type_defs.md#jobresourceoutputtypedef) 
5. See [:material-code-braces: ShippingDetailsTypeDef](./type_defs.md#shippingdetailstypedef) 
6. See [:material-code-brackets: SnowballCapacityType](./literals.md#snowballcapacitytype) 
7. See [:material-code-braces: NotificationOutputTypeDef](./type_defs.md#notificationoutputtypedef) 
8. See [:material-code-braces: DataTransferTypeDef](./type_defs.md#datatransfertypedef) 
9. See [:material-code-braces: JobLogsTypeDef](./type_defs.md#joblogstypedef) 
10. See [:material-code-braces: TaxDocumentsTypeDef](./type_defs.md#taxdocumentstypedef) 
11. See [:material-code-braces: DeviceConfigurationTypeDef](./type_defs.md#deviceconfigurationtypedef) 
12. See [:material-code-brackets: RemoteManagementType](./literals.md#remotemanagementtype) 
13. See [:material-code-braces: OnDeviceServiceConfigurationTypeDef](./type_defs.md#ondeviceserviceconfigurationtypedef) 
14. See [:material-code-brackets: ImpactLevelType](./literals.md#impactleveltype) 
15. See [:material-code-braces: PickupDetailsOutputTypeDef](./type_defs.md#pickupdetailsoutputtypedef) 
## DescribeClusterResultTypeDef

```python
# DescribeClusterResultTypeDef definition

class DescribeClusterResultTypeDef(TypedDict):
    ClusterMetadata: ClusterMetadataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterMetadataTypeDef](./type_defs.md#clustermetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateClusterRequestRequestTypeDef

```python
# CreateClusterRequestRequestTypeDef definition

class CreateClusterRequestRequestTypeDef(TypedDict):
    JobType: JobTypeType,  # (1)
    AddressId: str,
    SnowballType: SnowballTypeType,  # (2)
    ShippingOption: ShippingOptionType,  # (3)
    Resources: NotRequired[JobResourceTypeDef],  # (4)
    OnDeviceServiceConfiguration: NotRequired[OnDeviceServiceConfigurationTypeDef],  # (5)
    Description: NotRequired[str],
    KmsKeyARN: NotRequired[str],
    RoleARN: NotRequired[str],
    Notification: NotRequired[NotificationTypeDef],  # (6)
    ForwardingAddressId: NotRequired[str],
    TaxDocuments: NotRequired[TaxDocumentsTypeDef],  # (7)
    RemoteManagement: NotRequired[RemoteManagementType],  # (8)
    InitialClusterSize: NotRequired[int],
    ForceCreateJobs: NotRequired[bool],
    LongTermPricingIds: NotRequired[Sequence[str]],
    SnowballCapacityPreference: NotRequired[SnowballCapacityType],  # (9)
```

1. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
2. See [:material-code-brackets: SnowballTypeType](./literals.md#snowballtypetype) 
3. See [:material-code-brackets: ShippingOptionType](./literals.md#shippingoptiontype) 
4. See [:material-code-braces: JobResourceTypeDef](./type_defs.md#jobresourcetypedef) 
5. See [:material-code-braces: OnDeviceServiceConfigurationTypeDef](./type_defs.md#ondeviceserviceconfigurationtypedef) 
6. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
7. See [:material-code-braces: TaxDocumentsTypeDef](./type_defs.md#taxdocumentstypedef) 
8. See [:material-code-brackets: RemoteManagementType](./literals.md#remotemanagementtype) 
9. See [:material-code-brackets: SnowballCapacityType](./literals.md#snowballcapacitytype) 
## CreateJobRequestRequestTypeDef

```python
# CreateJobRequestRequestTypeDef definition

class CreateJobRequestRequestTypeDef(TypedDict):
    JobType: NotRequired[JobTypeType],  # (1)
    Resources: NotRequired[JobResourceTypeDef],  # (2)
    OnDeviceServiceConfiguration: NotRequired[OnDeviceServiceConfigurationTypeDef],  # (3)
    Description: NotRequired[str],
    AddressId: NotRequired[str],
    KmsKeyARN: NotRequired[str],
    RoleARN: NotRequired[str],
    SnowballCapacityPreference: NotRequired[SnowballCapacityType],  # (4)
    ShippingOption: NotRequired[ShippingOptionType],  # (5)
    Notification: NotRequired[NotificationTypeDef],  # (6)
    ClusterId: NotRequired[str],
    SnowballType: NotRequired[SnowballTypeType],  # (7)
    ForwardingAddressId: NotRequired[str],
    TaxDocuments: NotRequired[TaxDocumentsTypeDef],  # (8)
    DeviceConfiguration: NotRequired[DeviceConfigurationTypeDef],  # (9)
    RemoteManagement: NotRequired[RemoteManagementType],  # (10)
    LongTermPricingId: NotRequired[str],
    ImpactLevel: NotRequired[ImpactLevelType],  # (11)
    PickupDetails: NotRequired[PickupDetailsTypeDef],  # (12)
```

1. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
2. See [:material-code-braces: JobResourceTypeDef](./type_defs.md#jobresourcetypedef) 
3. See [:material-code-braces: OnDeviceServiceConfigurationTypeDef](./type_defs.md#ondeviceserviceconfigurationtypedef) 
4. See [:material-code-brackets: SnowballCapacityType](./literals.md#snowballcapacitytype) 
5. See [:material-code-brackets: ShippingOptionType](./literals.md#shippingoptiontype) 
6. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
7. See [:material-code-brackets: SnowballTypeType](./literals.md#snowballtypetype) 
8. See [:material-code-braces: TaxDocumentsTypeDef](./type_defs.md#taxdocumentstypedef) 
9. See [:material-code-braces: DeviceConfigurationTypeDef](./type_defs.md#deviceconfigurationtypedef) 
10. See [:material-code-brackets: RemoteManagementType](./literals.md#remotemanagementtype) 
11. See [:material-code-brackets: ImpactLevelType](./literals.md#impactleveltype) 
12. See [:material-code-braces: PickupDetailsTypeDef](./type_defs.md#pickupdetailstypedef) 
## UpdateClusterRequestRequestTypeDef

```python
# UpdateClusterRequestRequestTypeDef definition

class UpdateClusterRequestRequestTypeDef(TypedDict):
    ClusterId: str,
    RoleARN: NotRequired[str],
    Description: NotRequired[str],
    Resources: NotRequired[JobResourceTypeDef],  # (1)
    OnDeviceServiceConfiguration: NotRequired[OnDeviceServiceConfigurationTypeDef],  # (2)
    AddressId: NotRequired[str],
    ShippingOption: NotRequired[ShippingOptionType],  # (3)
    Notification: NotRequired[NotificationTypeDef],  # (4)
    ForwardingAddressId: NotRequired[str],
```

1. See [:material-code-braces: JobResourceTypeDef](./type_defs.md#jobresourcetypedef) 
2. See [:material-code-braces: OnDeviceServiceConfigurationTypeDef](./type_defs.md#ondeviceserviceconfigurationtypedef) 
3. See [:material-code-brackets: ShippingOptionType](./literals.md#shippingoptiontype) 
4. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
## UpdateJobRequestRequestTypeDef

```python
# UpdateJobRequestRequestTypeDef definition

class UpdateJobRequestRequestTypeDef(TypedDict):
    JobId: str,
    RoleARN: NotRequired[str],
    Notification: NotRequired[NotificationTypeDef],  # (1)
    Resources: NotRequired[JobResourceTypeDef],  # (2)
    OnDeviceServiceConfiguration: NotRequired[OnDeviceServiceConfigurationTypeDef],  # (3)
    AddressId: NotRequired[str],
    ShippingOption: NotRequired[ShippingOptionType],  # (4)
    Description: NotRequired[str],
    SnowballCapacityPreference: NotRequired[SnowballCapacityType],  # (5)
    ForwardingAddressId: NotRequired[str],
    PickupDetails: NotRequired[PickupDetailsTypeDef],  # (6)
```

1. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
2. See [:material-code-braces: JobResourceTypeDef](./type_defs.md#jobresourcetypedef) 
3. See [:material-code-braces: OnDeviceServiceConfigurationTypeDef](./type_defs.md#ondeviceserviceconfigurationtypedef) 
4. See [:material-code-brackets: ShippingOptionType](./literals.md#shippingoptiontype) 
5. See [:material-code-brackets: SnowballCapacityType](./literals.md#snowballcapacitytype) 
6. See [:material-code-braces: PickupDetailsTypeDef](./type_defs.md#pickupdetailstypedef) 
## DescribeJobResultTypeDef

```python
# DescribeJobResultTypeDef definition

class DescribeJobResultTypeDef(TypedDict):
    JobMetadata: JobMetadataTypeDef,  # (1)
    SubJobMetadata: List[JobMetadataTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: JobMetadataTypeDef](./type_defs.md#jobmetadatatypedef) 
2. See [:material-code-braces: JobMetadataTypeDef](./type_defs.md#jobmetadatatypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
