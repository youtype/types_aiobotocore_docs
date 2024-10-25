# Type definitions

> [Index](../README.md) > [Panorama](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Panorama](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
    type annotations stubs module [types-aiobotocore-panorama](https://pypi.org/project/types-aiobotocore-panorama/).

## JobResourceTagsUnionTypeDef

```python
# JobResourceTagsUnionTypeDef definition

JobResourceTagsUnionTypeDef = Union[
    JobResourceTagsTypeDef,  # (1)
    JobResourceTagsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: JobResourceTagsTypeDef](./type_defs.md#jobresourcetagstypedef) 
2. See [:material-code-braces: JobResourceTagsOutputTypeDef](./type_defs.md#jobresourcetagsoutputtypedef) 

## NtpPayloadUnionTypeDef

```python
# NtpPayloadUnionTypeDef definition

NtpPayloadUnionTypeDef = Union[
    NtpPayloadTypeDef,  # (1)
    NtpPayloadOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NtpPayloadTypeDef](./type_defs.md#ntppayloadtypedef) 
2. See [:material-code-braces: NtpPayloadOutputTypeDef](./type_defs.md#ntppayloadoutputtypedef) 

## StaticIpConnectionInfoUnionTypeDef

```python
# StaticIpConnectionInfoUnionTypeDef definition

StaticIpConnectionInfoUnionTypeDef = Union[
    StaticIpConnectionInfoTypeDef,  # (1)
    StaticIpConnectionInfoOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: StaticIpConnectionInfoTypeDef](./type_defs.md#staticipconnectioninfotypedef) 
2. See [:material-code-braces: StaticIpConnectionInfoOutputTypeDef](./type_defs.md#staticipconnectioninfooutputtypedef) 

## EthernetPayloadUnionTypeDef

```python
# EthernetPayloadUnionTypeDef definition

EthernetPayloadUnionTypeDef = Union[
    EthernetPayloadTypeDef,  # (1)
    EthernetPayloadOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EthernetPayloadTypeDef](./type_defs.md#ethernetpayloadtypedef) 
2. See [:material-code-braces: EthernetPayloadOutputTypeDef](./type_defs.md#ethernetpayloadoutputtypedef) 



## AlternateSoftwareMetadataTypeDef

```python
# AlternateSoftwareMetadataTypeDef definition

class AlternateSoftwareMetadataTypeDef(TypedDict):
    Version: NotRequired[str],
```

## ReportedRuntimeContextStateTypeDef

```python
# ReportedRuntimeContextStateTypeDef definition

class ReportedRuntimeContextStateTypeDef(TypedDict):
    DesiredState: DesiredStateType,  # (1)
    DeviceReportedStatus: DeviceReportedStatusType,  # (2)
    DeviceReportedTime: datetime,
    RuntimeContextName: str,
```

1. See [:material-code-brackets: DesiredStateType](./literals.md#desiredstatetype) 
2. See [:material-code-brackets: DeviceReportedStatusType](./literals.md#devicereportedstatustype) 
## ManifestOverridesPayloadTypeDef

```python
# ManifestOverridesPayloadTypeDef definition

class ManifestOverridesPayloadTypeDef(TypedDict):
    PayloadData: NotRequired[str],
```

## ManifestPayloadTypeDef

```python
# ManifestPayloadTypeDef definition

class ManifestPayloadTypeDef(TypedDict):
    PayloadData: NotRequired[str],
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

## JobTypeDef

```python
# JobTypeDef definition

class JobTypeDef(TypedDict):
    DeviceId: NotRequired[str],
    JobId: NotRequired[str],
```

## JobResourceTagsTypeDef

```python
# JobResourceTagsTypeDef definition

class JobResourceTagsTypeDef(TypedDict):
    ResourceType: JobResourceTypeType,  # (1)
    Tags: Mapping[str, str],
```

1. See [:material-code-brackets: JobResourceTypeType](./literals.md#jobresourcetypetype) 
## CreatePackageRequestRequestTypeDef

```python
# CreatePackageRequestRequestTypeDef definition

class CreatePackageRequestRequestTypeDef(TypedDict):
    PackageName: str,
    Tags: NotRequired[Mapping[str, str]],
```

## StorageLocationTypeDef

```python
# StorageLocationTypeDef definition

class StorageLocationTypeDef(TypedDict):
    BinaryPrefixLocation: str,
    Bucket: str,
    GeneratedPrefixLocation: str,
    ManifestPrefixLocation: str,
    RepoPrefixLocation: str,
```

## DeleteDeviceRequestRequestTypeDef

```python
# DeleteDeviceRequestRequestTypeDef definition

class DeleteDeviceRequestRequestTypeDef(TypedDict):
    DeviceId: str,
```

## DeletePackageRequestRequestTypeDef

```python
# DeletePackageRequestRequestTypeDef definition

class DeletePackageRequestRequestTypeDef(TypedDict):
    PackageId: str,
    ForceDelete: NotRequired[bool],
```

## DeregisterPackageVersionRequestRequestTypeDef

```python
# DeregisterPackageVersionRequestRequestTypeDef definition

class DeregisterPackageVersionRequestRequestTypeDef(TypedDict):
    PackageId: str,
    PackageVersion: str,
    PatchVersion: str,
    OwnerAccount: NotRequired[str],
    UpdatedLatestPatchVersion: NotRequired[str],
```

## DescribeApplicationInstanceDetailsRequestRequestTypeDef

```python
# DescribeApplicationInstanceDetailsRequestRequestTypeDef definition

class DescribeApplicationInstanceDetailsRequestRequestTypeDef(TypedDict):
    ApplicationInstanceId: str,
```

## DescribeApplicationInstanceRequestRequestTypeDef

```python
# DescribeApplicationInstanceRequestRequestTypeDef definition

class DescribeApplicationInstanceRequestRequestTypeDef(TypedDict):
    ApplicationInstanceId: str,
```

## DescribeDeviceJobRequestRequestTypeDef

```python
# DescribeDeviceJobRequestRequestTypeDef definition

class DescribeDeviceJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## DescribeDeviceRequestRequestTypeDef

```python
# DescribeDeviceRequestRequestTypeDef definition

class DescribeDeviceRequestRequestTypeDef(TypedDict):
    DeviceId: str,
```

## LatestDeviceJobTypeDef

```python
# LatestDeviceJobTypeDef definition

class LatestDeviceJobTypeDef(TypedDict):
    ImageVersion: NotRequired[str],
    JobType: NotRequired[JobTypeType],  # (1)
    Status: NotRequired[UpdateProgressType],  # (2)
```

1. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
2. See [:material-code-brackets: UpdateProgressType](./literals.md#updateprogresstype) 
## DescribeNodeFromTemplateJobRequestRequestTypeDef

```python
# DescribeNodeFromTemplateJobRequestRequestTypeDef definition

class DescribeNodeFromTemplateJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## JobResourceTagsOutputTypeDef

```python
# JobResourceTagsOutputTypeDef definition

class JobResourceTagsOutputTypeDef(TypedDict):
    ResourceType: JobResourceTypeType,  # (1)
    Tags: Dict[str, str],
```

1. See [:material-code-brackets: JobResourceTypeType](./literals.md#jobresourcetypetype) 
## DescribeNodeRequestRequestTypeDef

```python
# DescribeNodeRequestRequestTypeDef definition

class DescribeNodeRequestRequestTypeDef(TypedDict):
    NodeId: str,
    OwnerAccount: NotRequired[str],
```

## DescribePackageImportJobRequestRequestTypeDef

```python
# DescribePackageImportJobRequestRequestTypeDef definition

class DescribePackageImportJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## DescribePackageRequestRequestTypeDef

```python
# DescribePackageRequestRequestTypeDef definition

class DescribePackageRequestRequestTypeDef(TypedDict):
    PackageId: str,
```

## DescribePackageVersionRequestRequestTypeDef

```python
# DescribePackageVersionRequestRequestTypeDef definition

class DescribePackageVersionRequestRequestTypeDef(TypedDict):
    PackageId: str,
    PackageVersion: str,
    OwnerAccount: NotRequired[str],
    PatchVersion: NotRequired[str],
```

## OTAJobConfigTypeDef

```python
# OTAJobConfigTypeDef definition

class OTAJobConfigTypeDef(TypedDict):
    ImageVersion: str,
    AllowMajorVersionUpdate: NotRequired[bool],
```

## DeviceJobTypeDef

```python
# DeviceJobTypeDef definition

class DeviceJobTypeDef(TypedDict):
    CreatedTime: NotRequired[datetime],
    DeviceId: NotRequired[str],
    DeviceName: NotRequired[str],
    JobId: NotRequired[str],
    JobType: NotRequired[JobTypeType],  # (1)
```

1. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
## StaticIpConnectionInfoOutputTypeDef

```python
# StaticIpConnectionInfoOutputTypeDef definition

class StaticIpConnectionInfoOutputTypeDef(TypedDict):
    DefaultGateway: str,
    Dns: List[str],
    IpAddress: str,
    Mask: str,
```

## EthernetStatusTypeDef

```python
# EthernetStatusTypeDef definition

class EthernetStatusTypeDef(TypedDict):
    ConnectionStatus: NotRequired[NetworkConnectionStatusType],  # (1)
    HwAddress: NotRequired[str],
    IpAddress: NotRequired[str],
```

1. See [:material-code-brackets: NetworkConnectionStatusType](./literals.md#networkconnectionstatustype) 
## ListApplicationInstanceDependenciesRequestRequestTypeDef

```python
# ListApplicationInstanceDependenciesRequestRequestTypeDef definition

class ListApplicationInstanceDependenciesRequestRequestTypeDef(TypedDict):
    ApplicationInstanceId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## PackageObjectTypeDef

```python
# PackageObjectTypeDef definition

class PackageObjectTypeDef(TypedDict):
    Name: str,
    PackageVersion: str,
    PatchVersion: str,
```

## ListApplicationInstanceNodeInstancesRequestRequestTypeDef

```python
# ListApplicationInstanceNodeInstancesRequestRequestTypeDef definition

class ListApplicationInstanceNodeInstancesRequestRequestTypeDef(TypedDict):
    ApplicationInstanceId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## NodeInstanceTypeDef

```python
# NodeInstanceTypeDef definition

class NodeInstanceTypeDef(TypedDict):
    CurrentStatus: NodeInstanceStatusType,  # (1)
    NodeInstanceId: str,
    NodeId: NotRequired[str],
    NodeName: NotRequired[str],
    PackageName: NotRequired[str],
    PackagePatchVersion: NotRequired[str],
    PackageVersion: NotRequired[str],
```

1. See [:material-code-brackets: NodeInstanceStatusType](./literals.md#nodeinstancestatustype) 
## ListApplicationInstancesRequestRequestTypeDef

```python
# ListApplicationInstancesRequestRequestTypeDef definition

class ListApplicationInstancesRequestRequestTypeDef(TypedDict):
    DeviceId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    StatusFilter: NotRequired[StatusFilterType],  # (1)
```

1. See [:material-code-brackets: StatusFilterType](./literals.md#statusfiltertype) 
## ListDevicesJobsRequestRequestTypeDef

```python
# ListDevicesJobsRequestRequestTypeDef definition

class ListDevicesJobsRequestRequestTypeDef(TypedDict):
    DeviceId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListDevicesRequestRequestTypeDef

```python
# ListDevicesRequestRequestTypeDef definition

class ListDevicesRequestRequestTypeDef(TypedDict):
    DeviceAggregatedStatusFilter: NotRequired[DeviceAggregatedStatusType],  # (1)
    MaxResults: NotRequired[int],
    NameFilter: NotRequired[str],
    NextToken: NotRequired[str],
    SortBy: NotRequired[ListDevicesSortByType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
```

1. See [:material-code-brackets: DeviceAggregatedStatusType](./literals.md#deviceaggregatedstatustype) 
2. See [:material-code-brackets: ListDevicesSortByType](./literals.md#listdevicessortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListNodeFromTemplateJobsRequestRequestTypeDef

```python
# ListNodeFromTemplateJobsRequestRequestTypeDef definition

class ListNodeFromTemplateJobsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## NodeFromTemplateJobTypeDef

```python
# NodeFromTemplateJobTypeDef definition

class NodeFromTemplateJobTypeDef(TypedDict):
    CreatedTime: NotRequired[datetime],
    JobId: NotRequired[str],
    NodeName: NotRequired[str],
    Status: NotRequired[NodeFromTemplateJobStatusType],  # (1)
    StatusMessage: NotRequired[str],
    TemplateType: NotRequired[TemplateTypeType],  # (2)
```

1. See [:material-code-brackets: NodeFromTemplateJobStatusType](./literals.md#nodefromtemplatejobstatustype) 
2. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
## ListNodesRequestRequestTypeDef

```python
# ListNodesRequestRequestTypeDef definition

class ListNodesRequestRequestTypeDef(TypedDict):
    Category: NotRequired[NodeCategoryType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    OwnerAccount: NotRequired[str],
    PackageName: NotRequired[str],
    PackageVersion: NotRequired[str],
    PatchVersion: NotRequired[str],
```

1. See [:material-code-brackets: NodeCategoryType](./literals.md#nodecategorytype) 
## NodeTypeDef

```python
# NodeTypeDef definition

class NodeTypeDef(TypedDict):
    Category: NodeCategoryType,  # (1)
    CreatedTime: datetime,
    Name: str,
    NodeId: str,
    PackageId: str,
    PackageName: str,
    PackageVersion: str,
    PatchVersion: str,
    Description: NotRequired[str],
    OwnerAccount: NotRequired[str],
    PackageArn: NotRequired[str],
```

1. See [:material-code-brackets: NodeCategoryType](./literals.md#nodecategorytype) 
## ListPackageImportJobsRequestRequestTypeDef

```python
# ListPackageImportJobsRequestRequestTypeDef definition

class ListPackageImportJobsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## PackageImportJobTypeDef

```python
# PackageImportJobTypeDef definition

class PackageImportJobTypeDef(TypedDict):
    CreatedTime: NotRequired[datetime],
    JobId: NotRequired[str],
    JobType: NotRequired[PackageImportJobTypeType],  # (1)
    LastUpdatedTime: NotRequired[datetime],
    Status: NotRequired[PackageImportJobStatusType],  # (2)
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: PackageImportJobTypeType](./literals.md#packageimportjobtypetype) 
2. See [:material-code-brackets: PackageImportJobStatusType](./literals.md#packageimportjobstatustype) 
## ListPackagesRequestRequestTypeDef

```python
# ListPackagesRequestRequestTypeDef definition

class ListPackagesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## PackageListItemTypeDef

```python
# PackageListItemTypeDef definition

class PackageListItemTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    PackageId: NotRequired[str],
    PackageName: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## NtpPayloadOutputTypeDef

```python
# NtpPayloadOutputTypeDef definition

class NtpPayloadOutputTypeDef(TypedDict):
    NtpServers: List[str],
```

## NtpStatusTypeDef

```python
# NtpStatusTypeDef definition

class NtpStatusTypeDef(TypedDict):
    ConnectionStatus: NotRequired[NetworkConnectionStatusType],  # (1)
    IpAddress: NotRequired[str],
    NtpServerName: NotRequired[str],
```

1. See [:material-code-brackets: NetworkConnectionStatusType](./literals.md#networkconnectionstatustype) 
## NodeInputPortTypeDef

```python
# NodeInputPortTypeDef definition

class NodeInputPortTypeDef(TypedDict):
    DefaultValue: NotRequired[str],
    Description: NotRequired[str],
    MaxConnections: NotRequired[int],
    Name: NotRequired[str],
    Type: NotRequired[PortTypeType],  # (1)
```

1. See [:material-code-brackets: PortTypeType](./literals.md#porttypetype) 
## NodeOutputPortTypeDef

```python
# NodeOutputPortTypeDef definition

class NodeOutputPortTypeDef(TypedDict):
    Description: NotRequired[str],
    Name: NotRequired[str],
    Type: NotRequired[PortTypeType],  # (1)
```

1. See [:material-code-brackets: PortTypeType](./literals.md#porttypetype) 
## NodeSignalTypeDef

```python
# NodeSignalTypeDef definition

class NodeSignalTypeDef(TypedDict):
    NodeInstanceId: str,
    Signal: NodeSignalValueType,  # (1)
```

1. See [:material-code-brackets: NodeSignalValueType](./literals.md#nodesignalvaluetype) 
## NtpPayloadTypeDef

```python
# NtpPayloadTypeDef definition

class NtpPayloadTypeDef(TypedDict):
    NtpServers: Sequence[str],
```

## OutPutS3LocationTypeDef

```python
# OutPutS3LocationTypeDef definition

class OutPutS3LocationTypeDef(TypedDict):
    BucketName: str,
    ObjectKey: str,
```

## PackageVersionOutputConfigTypeDef

```python
# PackageVersionOutputConfigTypeDef definition

class PackageVersionOutputConfigTypeDef(TypedDict):
    PackageName: str,
    PackageVersion: str,
    MarkLatest: NotRequired[bool],
```

## S3LocationTypeDef

```python
# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    BucketName: str,
    ObjectKey: str,
    Region: NotRequired[str],
```

## RegisterPackageVersionRequestRequestTypeDef

```python
# RegisterPackageVersionRequestRequestTypeDef definition

class RegisterPackageVersionRequestRequestTypeDef(TypedDict):
    PackageId: str,
    PackageVersion: str,
    PatchVersion: str,
    MarkLatest: NotRequired[bool],
    OwnerAccount: NotRequired[str],
```

## RemoveApplicationInstanceRequestRequestTypeDef

```python
# RemoveApplicationInstanceRequestRequestTypeDef definition

class RemoveApplicationInstanceRequestRequestTypeDef(TypedDict):
    ApplicationInstanceId: str,
```

## StaticIpConnectionInfoTypeDef

```python
# StaticIpConnectionInfoTypeDef definition

class StaticIpConnectionInfoTypeDef(TypedDict):
    DefaultGateway: str,
    Dns: Sequence[str],
    IpAddress: str,
    Mask: str,
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

## UpdateDeviceMetadataRequestRequestTypeDef

```python
# UpdateDeviceMetadataRequestRequestTypeDef definition

class UpdateDeviceMetadataRequestRequestTypeDef(TypedDict):
    DeviceId: str,
    Description: NotRequired[str],
```

## ApplicationInstanceTypeDef

```python
# ApplicationInstanceTypeDef definition

class ApplicationInstanceTypeDef(TypedDict):
    ApplicationInstanceId: NotRequired[str],
    Arn: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    DefaultRuntimeContextDevice: NotRequired[str],
    DefaultRuntimeContextDeviceName: NotRequired[str],
    Description: NotRequired[str],
    HealthStatus: NotRequired[ApplicationInstanceHealthStatusType],  # (1)
    Name: NotRequired[str],
    RuntimeContextStates: NotRequired[List[ReportedRuntimeContextStateTypeDef]],  # (2)
    Status: NotRequired[ApplicationInstanceStatusType],  # (3)
    StatusDescription: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ApplicationInstanceHealthStatusType](./literals.md#applicationinstancehealthstatustype) 
2. See [:material-code-braces: ReportedRuntimeContextStateTypeDef](./type_defs.md#reportedruntimecontextstatetypedef) 
3. See [:material-code-brackets: ApplicationInstanceStatusType](./literals.md#applicationinstancestatustype) 
## CreateApplicationInstanceRequestRequestTypeDef

```python
# CreateApplicationInstanceRequestRequestTypeDef definition

class CreateApplicationInstanceRequestRequestTypeDef(TypedDict):
    DefaultRuntimeContextDevice: str,
    ManifestPayload: ManifestPayloadTypeDef,  # (1)
    ApplicationInstanceIdToReplace: NotRequired[str],
    Description: NotRequired[str],
    ManifestOverridesPayload: NotRequired[ManifestOverridesPayloadTypeDef],  # (2)
    Name: NotRequired[str],
    RuntimeRoleArn: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ManifestPayloadTypeDef](./type_defs.md#manifestpayloadtypedef) 
2. See [:material-code-braces: ManifestOverridesPayloadTypeDef](./type_defs.md#manifestoverridespayloadtypedef) 
## CreateApplicationInstanceResponseTypeDef

```python
# CreateApplicationInstanceResponseTypeDef definition

class CreateApplicationInstanceResponseTypeDef(TypedDict):
    ApplicationInstanceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateNodeFromTemplateJobResponseTypeDef

```python
# CreateNodeFromTemplateJobResponseTypeDef definition

class CreateNodeFromTemplateJobResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePackageImportJobResponseTypeDef

```python
# CreatePackageImportJobResponseTypeDef definition

class CreatePackageImportJobResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDeviceResponseTypeDef

```python
# DeleteDeviceResponseTypeDef definition

class DeleteDeviceResponseTypeDef(TypedDict):
    DeviceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeApplicationInstanceDetailsResponseTypeDef

```python
# DescribeApplicationInstanceDetailsResponseTypeDef definition

class DescribeApplicationInstanceDetailsResponseTypeDef(TypedDict):
    ApplicationInstanceId: str,
    ApplicationInstanceIdToReplace: str,
    CreatedTime: datetime,
    DefaultRuntimeContextDevice: str,
    Description: str,
    ManifestOverridesPayload: ManifestOverridesPayloadTypeDef,  # (1)
    ManifestPayload: ManifestPayloadTypeDef,  # (2)
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ManifestOverridesPayloadTypeDef](./type_defs.md#manifestoverridespayloadtypedef) 
2. See [:material-code-braces: ManifestPayloadTypeDef](./type_defs.md#manifestpayloadtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeApplicationInstanceResponseTypeDef

```python
# DescribeApplicationInstanceResponseTypeDef definition

class DescribeApplicationInstanceResponseTypeDef(TypedDict):
    ApplicationInstanceId: str,
    ApplicationInstanceIdToReplace: str,
    Arn: str,
    CreatedTime: datetime,
    DefaultRuntimeContextDevice: str,
    DefaultRuntimeContextDeviceName: str,
    Description: str,
    HealthStatus: ApplicationInstanceHealthStatusType,  # (1)
    LastUpdatedTime: datetime,
    Name: str,
    RuntimeContextStates: List[ReportedRuntimeContextStateTypeDef],  # (2)
    RuntimeRoleArn: str,
    Status: ApplicationInstanceStatusType,  # (3)
    StatusDescription: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ApplicationInstanceHealthStatusType](./literals.md#applicationinstancehealthstatustype) 
2. See [:material-code-braces: ReportedRuntimeContextStateTypeDef](./type_defs.md#reportedruntimecontextstatetypedef) 
3. See [:material-code-brackets: ApplicationInstanceStatusType](./literals.md#applicationinstancestatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDeviceJobResponseTypeDef

```python
# DescribeDeviceJobResponseTypeDef definition

class DescribeDeviceJobResponseTypeDef(TypedDict):
    CreatedTime: datetime,
    DeviceArn: str,
    DeviceId: str,
    DeviceName: str,
    DeviceType: DeviceTypeType,  # (1)
    ImageVersion: str,
    JobId: str,
    JobType: JobTypeType,  # (2)
    Status: UpdateProgressType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: DeviceTypeType](./literals.md#devicetypetype) 
2. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
3. See [:material-code-brackets: UpdateProgressType](./literals.md#updateprogresstype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePackageVersionResponseTypeDef

```python
# DescribePackageVersionResponseTypeDef definition

class DescribePackageVersionResponseTypeDef(TypedDict):
    IsLatestPatch: bool,
    OwnerAccount: str,
    PackageArn: str,
    PackageId: str,
    PackageName: str,
    PackageVersion: str,
    PatchVersion: str,
    RegisteredTime: datetime,
    Status: PackageVersionStatusType,  # (1)
    StatusDescription: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: PackageVersionStatusType](./literals.md#packageversionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProvisionDeviceResponseTypeDef

```python
# ProvisionDeviceResponseTypeDef definition

class ProvisionDeviceResponseTypeDef(TypedDict):
    Arn: str,
    Certificates: bytes,
    DeviceId: str,
    IotThingName: str,
    Status: DeviceStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DeviceStatusType](./literals.md#devicestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SignalApplicationInstanceNodeInstancesResponseTypeDef

```python
# SignalApplicationInstanceNodeInstancesResponseTypeDef definition

class SignalApplicationInstanceNodeInstancesResponseTypeDef(TypedDict):
    ApplicationInstanceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDeviceMetadataResponseTypeDef

```python
# UpdateDeviceMetadataResponseTypeDef definition

class UpdateDeviceMetadataResponseTypeDef(TypedDict):
    DeviceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobForDevicesResponseTypeDef

```python
# CreateJobForDevicesResponseTypeDef definition

class CreateJobForDevicesResponseTypeDef(TypedDict):
    Jobs: List[JobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePackageResponseTypeDef

```python
# CreatePackageResponseTypeDef definition

class CreatePackageResponseTypeDef(TypedDict):
    Arn: str,
    PackageId: str,
    StorageLocation: StorageLocationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StorageLocationTypeDef](./type_defs.md#storagelocationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePackageResponseTypeDef

```python
# DescribePackageResponseTypeDef definition

class DescribePackageResponseTypeDef(TypedDict):
    Arn: str,
    CreatedTime: datetime,
    PackageId: str,
    PackageName: str,
    ReadAccessPrincipalArns: List[str],
    StorageLocation: StorageLocationTypeDef,  # (1)
    Tags: Dict[str, str],
    WriteAccessPrincipalArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StorageLocationTypeDef](./type_defs.md#storagelocationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeviceTypeDef

```python
# DeviceTypeDef definition

class DeviceTypeDef(TypedDict):
    Brand: NotRequired[DeviceBrandType],  # (1)
    CreatedTime: NotRequired[datetime],
    CurrentSoftware: NotRequired[str],
    Description: NotRequired[str],
    DeviceAggregatedStatus: NotRequired[DeviceAggregatedStatusType],  # (2)
    DeviceId: NotRequired[str],
    LastUpdatedTime: NotRequired[datetime],
    LatestDeviceJob: NotRequired[LatestDeviceJobTypeDef],  # (3)
    LeaseExpirationTime: NotRequired[datetime],
    Name: NotRequired[str],
    ProvisioningStatus: NotRequired[DeviceStatusType],  # (4)
    Tags: NotRequired[Dict[str, str]],
    Type: NotRequired[DeviceTypeType],  # (5)
```

1. See [:material-code-brackets: DeviceBrandType](./literals.md#devicebrandtype) 
2. See [:material-code-brackets: DeviceAggregatedStatusType](./literals.md#deviceaggregatedstatustype) 
3. See [:material-code-braces: LatestDeviceJobTypeDef](./type_defs.md#latestdevicejobtypedef) 
4. See [:material-code-brackets: DeviceStatusType](./literals.md#devicestatustype) 
5. See [:material-code-brackets: DeviceTypeType](./literals.md#devicetypetype) 
## DescribeNodeFromTemplateJobResponseTypeDef

```python
# DescribeNodeFromTemplateJobResponseTypeDef definition

class DescribeNodeFromTemplateJobResponseTypeDef(TypedDict):
    CreatedTime: datetime,
    JobId: str,
    JobTags: List[JobResourceTagsOutputTypeDef],  # (1)
    LastUpdatedTime: datetime,
    NodeDescription: str,
    NodeName: str,
    OutputPackageName: str,
    OutputPackageVersion: str,
    Status: NodeFromTemplateJobStatusType,  # (2)
    StatusMessage: str,
    TemplateParameters: Dict[str, str],
    TemplateType: TemplateTypeType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: JobResourceTagsOutputTypeDef](./type_defs.md#jobresourcetagsoutputtypedef) 
2. See [:material-code-brackets: NodeFromTemplateJobStatusType](./literals.md#nodefromtemplatejobstatustype) 
3. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeviceJobConfigTypeDef

```python
# DeviceJobConfigTypeDef definition

class DeviceJobConfigTypeDef(TypedDict):
    OTAJobConfig: NotRequired[OTAJobConfigTypeDef],  # (1)
```

1. See [:material-code-braces: OTAJobConfigTypeDef](./type_defs.md#otajobconfigtypedef) 
## ListDevicesJobsResponseTypeDef

```python
# ListDevicesJobsResponseTypeDef definition

class ListDevicesJobsResponseTypeDef(TypedDict):
    DeviceJobs: List[DeviceJobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DeviceJobTypeDef](./type_defs.md#devicejobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EthernetPayloadOutputTypeDef

```python
# EthernetPayloadOutputTypeDef definition

class EthernetPayloadOutputTypeDef(TypedDict):
    ConnectionType: ConnectionTypeType,  # (1)
    StaticIpConnectionInfo: NotRequired[StaticIpConnectionInfoOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
2. See [:material-code-braces: StaticIpConnectionInfoOutputTypeDef](./type_defs.md#staticipconnectioninfooutputtypedef) 
## ListApplicationInstanceDependenciesResponseTypeDef

```python
# ListApplicationInstanceDependenciesResponseTypeDef definition

class ListApplicationInstanceDependenciesResponseTypeDef(TypedDict):
    PackageObjects: List[PackageObjectTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PackageObjectTypeDef](./type_defs.md#packageobjecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationInstanceNodeInstancesResponseTypeDef

```python
# ListApplicationInstanceNodeInstancesResponseTypeDef definition

class ListApplicationInstanceNodeInstancesResponseTypeDef(TypedDict):
    NodeInstances: List[NodeInstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: NodeInstanceTypeDef](./type_defs.md#nodeinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNodeFromTemplateJobsResponseTypeDef

```python
# ListNodeFromTemplateJobsResponseTypeDef definition

class ListNodeFromTemplateJobsResponseTypeDef(TypedDict):
    NodeFromTemplateJobs: List[NodeFromTemplateJobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: NodeFromTemplateJobTypeDef](./type_defs.md#nodefromtemplatejobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNodesResponseTypeDef

```python
# ListNodesResponseTypeDef definition

class ListNodesResponseTypeDef(TypedDict):
    Nodes: List[NodeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: NodeTypeDef](./type_defs.md#nodetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPackageImportJobsResponseTypeDef

```python
# ListPackageImportJobsResponseTypeDef definition

class ListPackageImportJobsResponseTypeDef(TypedDict):
    PackageImportJobs: List[PackageImportJobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PackageImportJobTypeDef](./type_defs.md#packageimportjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPackagesResponseTypeDef

```python
# ListPackagesResponseTypeDef definition

class ListPackagesResponseTypeDef(TypedDict):
    Packages: List[PackageListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PackageListItemTypeDef](./type_defs.md#packagelistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NetworkStatusTypeDef

```python
# NetworkStatusTypeDef definition

class NetworkStatusTypeDef(TypedDict):
    Ethernet0Status: NotRequired[EthernetStatusTypeDef],  # (1)
    Ethernet1Status: NotRequired[EthernetStatusTypeDef],  # (1)
    LastUpdatedTime: NotRequired[datetime],
    NtpStatus: NotRequired[NtpStatusTypeDef],  # (3)
```

1. See [:material-code-braces: EthernetStatusTypeDef](./type_defs.md#ethernetstatustypedef) 
2. See [:material-code-braces: EthernetStatusTypeDef](./type_defs.md#ethernetstatustypedef) 
3. See [:material-code-braces: NtpStatusTypeDef](./type_defs.md#ntpstatustypedef) 
## NodeInterfaceTypeDef

```python
# NodeInterfaceTypeDef definition

class NodeInterfaceTypeDef(TypedDict):
    Inputs: List[NodeInputPortTypeDef],  # (1)
    Outputs: List[NodeOutputPortTypeDef],  # (2)
```

1. See [:material-code-braces: NodeInputPortTypeDef](./type_defs.md#nodeinputporttypedef) 
2. See [:material-code-braces: NodeOutputPortTypeDef](./type_defs.md#nodeoutputporttypedef) 
## SignalApplicationInstanceNodeInstancesRequestRequestTypeDef

```python
# SignalApplicationInstanceNodeInstancesRequestRequestTypeDef definition

class SignalApplicationInstanceNodeInstancesRequestRequestTypeDef(TypedDict):
    ApplicationInstanceId: str,
    NodeSignals: Sequence[NodeSignalTypeDef],  # (1)
```

1. See [:material-code-braces: NodeSignalTypeDef](./type_defs.md#nodesignaltypedef) 
## PackageImportJobOutputTypeDef

```python
# PackageImportJobOutputTypeDef definition

class PackageImportJobOutputTypeDef(TypedDict):
    OutputS3Location: OutPutS3LocationTypeDef,  # (1)
    PackageId: str,
    PackageVersion: str,
    PatchVersion: str,
```

1. See [:material-code-braces: OutPutS3LocationTypeDef](./type_defs.md#outputs3locationtypedef) 
## PackageImportJobOutputConfigTypeDef

```python
# PackageImportJobOutputConfigTypeDef definition

class PackageImportJobOutputConfigTypeDef(TypedDict):
    PackageVersionOutputConfig: NotRequired[PackageVersionOutputConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PackageVersionOutputConfigTypeDef](./type_defs.md#packageversionoutputconfigtypedef) 
## PackageVersionInputConfigTypeDef

```python
# PackageVersionInputConfigTypeDef definition

class PackageVersionInputConfigTypeDef(TypedDict):
    S3Location: S3LocationTypeDef,  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## ListApplicationInstancesResponseTypeDef

```python
# ListApplicationInstancesResponseTypeDef definition

class ListApplicationInstancesResponseTypeDef(TypedDict):
    ApplicationInstances: List[ApplicationInstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationInstanceTypeDef](./type_defs.md#applicationinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDevicesResponseTypeDef

```python
# ListDevicesResponseTypeDef definition

class ListDevicesResponseTypeDef(TypedDict):
    Devices: List[DeviceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DeviceTypeDef](./type_defs.md#devicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateNodeFromTemplateJobRequestRequestTypeDef

```python
# CreateNodeFromTemplateJobRequestRequestTypeDef definition

class CreateNodeFromTemplateJobRequestRequestTypeDef(TypedDict):
    NodeName: str,
    OutputPackageName: str,
    OutputPackageVersion: str,
    TemplateParameters: Mapping[str, str],
    TemplateType: TemplateTypeType,  # (1)
    JobTags: NotRequired[Sequence[JobResourceTagsUnionTypeDef]],  # (2)
    NodeDescription: NotRequired[str],
```

1. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
2. See [:material-code-braces: JobResourceTagsTypeDef](./type_defs.md#jobresourcetagstypedef) [:material-code-braces: JobResourceTagsOutputTypeDef](./type_defs.md#jobresourcetagsoutputtypedef) 
## CreateJobForDevicesRequestRequestTypeDef

```python
# CreateJobForDevicesRequestRequestTypeDef definition

class CreateJobForDevicesRequestRequestTypeDef(TypedDict):
    DeviceIds: Sequence[str],
    JobType: JobTypeType,  # (1)
    DeviceJobConfig: NotRequired[DeviceJobConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
2. See [:material-code-braces: DeviceJobConfigTypeDef](./type_defs.md#devicejobconfigtypedef) 
## NetworkPayloadOutputTypeDef

```python
# NetworkPayloadOutputTypeDef definition

class NetworkPayloadOutputTypeDef(TypedDict):
    Ethernet0: NotRequired[EthernetPayloadOutputTypeDef],  # (1)
    Ethernet1: NotRequired[EthernetPayloadOutputTypeDef],  # (1)
    Ntp: NotRequired[NtpPayloadOutputTypeDef],  # (3)
```

1. See [:material-code-braces: EthernetPayloadOutputTypeDef](./type_defs.md#ethernetpayloadoutputtypedef) 
2. See [:material-code-braces: EthernetPayloadOutputTypeDef](./type_defs.md#ethernetpayloadoutputtypedef) 
3. See [:material-code-braces: NtpPayloadOutputTypeDef](./type_defs.md#ntppayloadoutputtypedef) 
## DescribeNodeResponseTypeDef

```python
# DescribeNodeResponseTypeDef definition

class DescribeNodeResponseTypeDef(TypedDict):
    AssetName: str,
    Category: NodeCategoryType,  # (1)
    CreatedTime: datetime,
    Description: str,
    LastUpdatedTime: datetime,
    Name: str,
    NodeId: str,
    NodeInterface: NodeInterfaceTypeDef,  # (2)
    OwnerAccount: str,
    PackageArn: str,
    PackageId: str,
    PackageName: str,
    PackageVersion: str,
    PatchVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: NodeCategoryType](./literals.md#nodecategorytype) 
2. See [:material-code-braces: NodeInterfaceTypeDef](./type_defs.md#nodeinterfacetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PackageImportJobInputConfigTypeDef

```python
# PackageImportJobInputConfigTypeDef definition

class PackageImportJobInputConfigTypeDef(TypedDict):
    PackageVersionInputConfig: NotRequired[PackageVersionInputConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PackageVersionInputConfigTypeDef](./type_defs.md#packageversioninputconfigtypedef) 
## EthernetPayloadTypeDef

```python
# EthernetPayloadTypeDef definition

class EthernetPayloadTypeDef(TypedDict):
    ConnectionType: ConnectionTypeType,  # (1)
    StaticIpConnectionInfo: NotRequired[StaticIpConnectionInfoUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
2. See [:material-code-braces: StaticIpConnectionInfoTypeDef](./type_defs.md#staticipconnectioninfotypedef) [:material-code-braces: StaticIpConnectionInfoOutputTypeDef](./type_defs.md#staticipconnectioninfooutputtypedef) 
## DescribeDeviceResponseTypeDef

```python
# DescribeDeviceResponseTypeDef definition

class DescribeDeviceResponseTypeDef(TypedDict):
    AlternateSoftwares: List[AlternateSoftwareMetadataTypeDef],  # (1)
    Arn: str,
    Brand: DeviceBrandType,  # (2)
    CreatedTime: datetime,
    CurrentNetworkingStatus: NetworkStatusTypeDef,  # (3)
    CurrentSoftware: str,
    Description: str,
    DeviceAggregatedStatus: DeviceAggregatedStatusType,  # (4)
    DeviceConnectionStatus: DeviceConnectionStatusType,  # (5)
    DeviceId: str,
    LatestAlternateSoftware: str,
    LatestDeviceJob: LatestDeviceJobTypeDef,  # (6)
    LatestSoftware: str,
    LeaseExpirationTime: datetime,
    Name: str,
    NetworkingConfiguration: NetworkPayloadOutputTypeDef,  # (7)
    ProvisioningStatus: DeviceStatusType,  # (8)
    SerialNumber: str,
    Tags: Dict[str, str],
    Type: DeviceTypeType,  # (9)
    ResponseMetadata: ResponseMetadataTypeDef,  # (10)
```

1. See [:material-code-braces: AlternateSoftwareMetadataTypeDef](./type_defs.md#alternatesoftwaremetadatatypedef) 
2. See [:material-code-brackets: DeviceBrandType](./literals.md#devicebrandtype) 
3. See [:material-code-braces: NetworkStatusTypeDef](./type_defs.md#networkstatustypedef) 
4. See [:material-code-brackets: DeviceAggregatedStatusType](./literals.md#deviceaggregatedstatustype) 
5. See [:material-code-brackets: DeviceConnectionStatusType](./literals.md#deviceconnectionstatustype) 
6. See [:material-code-braces: LatestDeviceJobTypeDef](./type_defs.md#latestdevicejobtypedef) 
7. See [:material-code-braces: NetworkPayloadOutputTypeDef](./type_defs.md#networkpayloadoutputtypedef) 
8. See [:material-code-brackets: DeviceStatusType](./literals.md#devicestatustype) 
9. See [:material-code-brackets: DeviceTypeType](./literals.md#devicetypetype) 
10. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePackageImportJobRequestRequestTypeDef

```python
# CreatePackageImportJobRequestRequestTypeDef definition

class CreatePackageImportJobRequestRequestTypeDef(TypedDict):
    ClientToken: str,
    InputConfig: PackageImportJobInputConfigTypeDef,  # (1)
    JobType: PackageImportJobTypeType,  # (2)
    OutputConfig: PackageImportJobOutputConfigTypeDef,  # (3)
    JobTags: NotRequired[Sequence[JobResourceTagsTypeDef]],  # (4)
```

1. See [:material-code-braces: PackageImportJobInputConfigTypeDef](./type_defs.md#packageimportjobinputconfigtypedef) 
2. See [:material-code-brackets: PackageImportJobTypeType](./literals.md#packageimportjobtypetype) 
3. See [:material-code-braces: PackageImportJobOutputConfigTypeDef](./type_defs.md#packageimportjoboutputconfigtypedef) 
4. See [:material-code-braces: JobResourceTagsTypeDef](./type_defs.md#jobresourcetagstypedef) 
## DescribePackageImportJobResponseTypeDef

```python
# DescribePackageImportJobResponseTypeDef definition

class DescribePackageImportJobResponseTypeDef(TypedDict):
    ClientToken: str,
    CreatedTime: datetime,
    InputConfig: PackageImportJobInputConfigTypeDef,  # (1)
    JobId: str,
    JobTags: List[JobResourceTagsOutputTypeDef],  # (2)
    JobType: PackageImportJobTypeType,  # (3)
    LastUpdatedTime: datetime,
    Output: PackageImportJobOutputTypeDef,  # (4)
    OutputConfig: PackageImportJobOutputConfigTypeDef,  # (5)
    Status: PackageImportJobStatusType,  # (6)
    StatusMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-braces: PackageImportJobInputConfigTypeDef](./type_defs.md#packageimportjobinputconfigtypedef) 
2. See [:material-code-braces: JobResourceTagsOutputTypeDef](./type_defs.md#jobresourcetagsoutputtypedef) 
3. See [:material-code-brackets: PackageImportJobTypeType](./literals.md#packageimportjobtypetype) 
4. See [:material-code-braces: PackageImportJobOutputTypeDef](./type_defs.md#packageimportjoboutputtypedef) 
5. See [:material-code-braces: PackageImportJobOutputConfigTypeDef](./type_defs.md#packageimportjoboutputconfigtypedef) 
6. See [:material-code-brackets: PackageImportJobStatusType](./literals.md#packageimportjobstatustype) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NetworkPayloadTypeDef

```python
# NetworkPayloadTypeDef definition

class NetworkPayloadTypeDef(TypedDict):
    Ethernet0: NotRequired[EthernetPayloadUnionTypeDef],  # (1)
    Ethernet1: NotRequired[EthernetPayloadUnionTypeDef],  # (1)
    Ntp: NotRequired[NtpPayloadUnionTypeDef],  # (3)
```

1. See [:material-code-braces: EthernetPayloadTypeDef](./type_defs.md#ethernetpayloadtypedef) [:material-code-braces: EthernetPayloadOutputTypeDef](./type_defs.md#ethernetpayloadoutputtypedef) 
2. See [:material-code-braces: EthernetPayloadTypeDef](./type_defs.md#ethernetpayloadtypedef) [:material-code-braces: EthernetPayloadOutputTypeDef](./type_defs.md#ethernetpayloadoutputtypedef) 
3. See [:material-code-braces: NtpPayloadTypeDef](./type_defs.md#ntppayloadtypedef) [:material-code-braces: NtpPayloadOutputTypeDef](./type_defs.md#ntppayloadoutputtypedef) 
## ProvisionDeviceRequestRequestTypeDef

```python
# ProvisionDeviceRequestRequestTypeDef definition

class ProvisionDeviceRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    NetworkingConfiguration: NotRequired[NetworkPayloadTypeDef],  # (1)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: NetworkPayloadTypeDef](./type_defs.md#networkpayloadtypedef) 
