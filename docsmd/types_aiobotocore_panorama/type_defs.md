# Type definitions

> [Index](../README.md) > [Panorama](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Panorama](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#panorama)
    type annotations stubs module [types-aiobotocore-panorama](https://pypi.org/project/types-aiobotocore-panorama/).

## JobResourceTagsUnionTypeDef

```python
# JobResourceTagsUnionTypeDef Union usage example

from types_aiobotocore_panorama.type_defs import JobResourceTagsUnionTypeDef


def get_value() -> JobResourceTagsUnionTypeDef:
    return ...


# JobResourceTagsUnionTypeDef definition

JobResourceTagsUnionTypeDef = Union[
    JobResourceTagsTypeDef,  # (1)
    JobResourceTagsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: JobResourceTagsTypeDef](./type_defs.md#jobresourcetagstypedef) 
2. See [:material-code-braces: JobResourceTagsOutputTypeDef](./type_defs.md#jobresourcetagsoutputtypedef) 

## NetworkPayloadUnionTypeDef

```python
# NetworkPayloadUnionTypeDef Union usage example

from types_aiobotocore_panorama.type_defs import NetworkPayloadUnionTypeDef


def get_value() -> NetworkPayloadUnionTypeDef:
    return ...


# NetworkPayloadUnionTypeDef definition

NetworkPayloadUnionTypeDef = Union[
    NetworkPayloadTypeDef,  # (1)
    NetworkPayloadOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NetworkPayloadTypeDef](./type_defs.md#networkpayloadtypedef) 
2. See [:material-code-braces: NetworkPayloadOutputTypeDef](./type_defs.md#networkpayloadoutputtypedef) 



## AlternateSoftwareMetadataTypeDef

```python
# AlternateSoftwareMetadataTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import AlternateSoftwareMetadataTypeDef


def get_value() -> AlternateSoftwareMetadataTypeDef:
    return {
        "Version": ...,
    }


# AlternateSoftwareMetadataTypeDef definition

class AlternateSoftwareMetadataTypeDef(TypedDict):
    Version: NotRequired[str],
```

## ReportedRuntimeContextStateTypeDef

```python
# ReportedRuntimeContextStateTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ReportedRuntimeContextStateTypeDef


def get_value() -> ReportedRuntimeContextStateTypeDef:
    return {
        "DesiredState": ...,
    }


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
# ManifestOverridesPayloadTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ManifestOverridesPayloadTypeDef


def get_value() -> ManifestOverridesPayloadTypeDef:
    return {
        "PayloadData": ...,
    }


# ManifestOverridesPayloadTypeDef definition

class ManifestOverridesPayloadTypeDef(TypedDict):
    PayloadData: NotRequired[str],
```

## ManifestPayloadTypeDef

```python
# ManifestPayloadTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ManifestPayloadTypeDef


def get_value() -> ManifestPayloadTypeDef:
    return {
        "PayloadData": ...,
    }


# ManifestPayloadTypeDef definition

class ManifestPayloadTypeDef(TypedDict):
    PayloadData: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ResponseMetadataTypeDef


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

## JobTypeDef

```python
# JobTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import JobTypeDef


def get_value() -> JobTypeDef:
    return {
        "DeviceId": ...,
    }


# JobTypeDef definition

class JobTypeDef(TypedDict):
    DeviceId: NotRequired[str],
    JobId: NotRequired[str],
```

## CreatePackageRequestTypeDef

```python
# CreatePackageRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import CreatePackageRequestTypeDef


def get_value() -> CreatePackageRequestTypeDef:
    return {
        "PackageName": ...,
    }


# CreatePackageRequestTypeDef definition

class CreatePackageRequestTypeDef(TypedDict):
    PackageName: str,
    Tags: NotRequired[Mapping[str, str]],
```

## StorageLocationTypeDef

```python
# StorageLocationTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import StorageLocationTypeDef


def get_value() -> StorageLocationTypeDef:
    return {
        "BinaryPrefixLocation": ...,
    }


# StorageLocationTypeDef definition

class StorageLocationTypeDef(TypedDict):
    BinaryPrefixLocation: str,
    Bucket: str,
    GeneratedPrefixLocation: str,
    ManifestPrefixLocation: str,
    RepoPrefixLocation: str,
```

## DeleteDeviceRequestTypeDef

```python
# DeleteDeviceRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DeleteDeviceRequestTypeDef


def get_value() -> DeleteDeviceRequestTypeDef:
    return {
        "DeviceId": ...,
    }


# DeleteDeviceRequestTypeDef definition

class DeleteDeviceRequestTypeDef(TypedDict):
    DeviceId: str,
```

## DeletePackageRequestTypeDef

```python
# DeletePackageRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DeletePackageRequestTypeDef


def get_value() -> DeletePackageRequestTypeDef:
    return {
        "PackageId": ...,
    }


# DeletePackageRequestTypeDef definition

class DeletePackageRequestTypeDef(TypedDict):
    PackageId: str,
    ForceDelete: NotRequired[bool],
```

## DeregisterPackageVersionRequestTypeDef

```python
# DeregisterPackageVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DeregisterPackageVersionRequestTypeDef


def get_value() -> DeregisterPackageVersionRequestTypeDef:
    return {
        "PackageId": ...,
    }


# DeregisterPackageVersionRequestTypeDef definition

class DeregisterPackageVersionRequestTypeDef(TypedDict):
    PackageId: str,
    PackageVersion: str,
    PatchVersion: str,
    OwnerAccount: NotRequired[str],
    UpdatedLatestPatchVersion: NotRequired[str],
```

## DescribeApplicationInstanceDetailsRequestTypeDef

```python
# DescribeApplicationInstanceDetailsRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DescribeApplicationInstanceDetailsRequestTypeDef


def get_value() -> DescribeApplicationInstanceDetailsRequestTypeDef:
    return {
        "ApplicationInstanceId": ...,
    }


# DescribeApplicationInstanceDetailsRequestTypeDef definition

class DescribeApplicationInstanceDetailsRequestTypeDef(TypedDict):
    ApplicationInstanceId: str,
```

## DescribeApplicationInstanceRequestTypeDef

```python
# DescribeApplicationInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DescribeApplicationInstanceRequestTypeDef


def get_value() -> DescribeApplicationInstanceRequestTypeDef:
    return {
        "ApplicationInstanceId": ...,
    }


# DescribeApplicationInstanceRequestTypeDef definition

class DescribeApplicationInstanceRequestTypeDef(TypedDict):
    ApplicationInstanceId: str,
```

## DescribeDeviceJobRequestTypeDef

```python
# DescribeDeviceJobRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DescribeDeviceJobRequestTypeDef


def get_value() -> DescribeDeviceJobRequestTypeDef:
    return {
        "JobId": ...,
    }


# DescribeDeviceJobRequestTypeDef definition

class DescribeDeviceJobRequestTypeDef(TypedDict):
    JobId: str,
```

## DescribeDeviceRequestTypeDef

```python
# DescribeDeviceRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DescribeDeviceRequestTypeDef


def get_value() -> DescribeDeviceRequestTypeDef:
    return {
        "DeviceId": ...,
    }


# DescribeDeviceRequestTypeDef definition

class DescribeDeviceRequestTypeDef(TypedDict):
    DeviceId: str,
```

## LatestDeviceJobTypeDef

```python
# LatestDeviceJobTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import LatestDeviceJobTypeDef


def get_value() -> LatestDeviceJobTypeDef:
    return {
        "ImageVersion": ...,
    }


# LatestDeviceJobTypeDef definition

class LatestDeviceJobTypeDef(TypedDict):
    ImageVersion: NotRequired[str],
    JobType: NotRequired[JobTypeType],  # (1)
    Status: NotRequired[UpdateProgressType],  # (2)
```

1. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
2. See [:material-code-brackets: UpdateProgressType](./literals.md#updateprogresstype) 
## DescribeNodeFromTemplateJobRequestTypeDef

```python
# DescribeNodeFromTemplateJobRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DescribeNodeFromTemplateJobRequestTypeDef


def get_value() -> DescribeNodeFromTemplateJobRequestTypeDef:
    return {
        "JobId": ...,
    }


# DescribeNodeFromTemplateJobRequestTypeDef definition

class DescribeNodeFromTemplateJobRequestTypeDef(TypedDict):
    JobId: str,
```

## JobResourceTagsOutputTypeDef

```python
# JobResourceTagsOutputTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import JobResourceTagsOutputTypeDef


def get_value() -> JobResourceTagsOutputTypeDef:
    return {
        "ResourceType": ...,
    }


# JobResourceTagsOutputTypeDef definition

class JobResourceTagsOutputTypeDef(TypedDict):
    ResourceType: JobResourceTypeType,  # (1)
    Tags: Dict[str, str],
```

1. See [:material-code-brackets: JobResourceTypeType](./literals.md#jobresourcetypetype) 
## DescribeNodeRequestTypeDef

```python
# DescribeNodeRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DescribeNodeRequestTypeDef


def get_value() -> DescribeNodeRequestTypeDef:
    return {
        "NodeId": ...,
    }


# DescribeNodeRequestTypeDef definition

class DescribeNodeRequestTypeDef(TypedDict):
    NodeId: str,
    OwnerAccount: NotRequired[str],
```

## DescribePackageImportJobRequestTypeDef

```python
# DescribePackageImportJobRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DescribePackageImportJobRequestTypeDef


def get_value() -> DescribePackageImportJobRequestTypeDef:
    return {
        "JobId": ...,
    }


# DescribePackageImportJobRequestTypeDef definition

class DescribePackageImportJobRequestTypeDef(TypedDict):
    JobId: str,
```

## DescribePackageRequestTypeDef

```python
# DescribePackageRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DescribePackageRequestTypeDef


def get_value() -> DescribePackageRequestTypeDef:
    return {
        "PackageId": ...,
    }


# DescribePackageRequestTypeDef definition

class DescribePackageRequestTypeDef(TypedDict):
    PackageId: str,
```

## DescribePackageVersionRequestTypeDef

```python
# DescribePackageVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DescribePackageVersionRequestTypeDef


def get_value() -> DescribePackageVersionRequestTypeDef:
    return {
        "PackageId": ...,
    }


# DescribePackageVersionRequestTypeDef definition

class DescribePackageVersionRequestTypeDef(TypedDict):
    PackageId: str,
    PackageVersion: str,
    OwnerAccount: NotRequired[str],
    PatchVersion: NotRequired[str],
```

## OTAJobConfigTypeDef

```python
# OTAJobConfigTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import OTAJobConfigTypeDef


def get_value() -> OTAJobConfigTypeDef:
    return {
        "AllowMajorVersionUpdate": ...,
    }


# OTAJobConfigTypeDef definition

class OTAJobConfigTypeDef(TypedDict):
    ImageVersion: str,
    AllowMajorVersionUpdate: NotRequired[bool],
```

## DeviceJobTypeDef

```python
# DeviceJobTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DeviceJobTypeDef


def get_value() -> DeviceJobTypeDef:
    return {
        "CreatedTime": ...,
    }


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
# StaticIpConnectionInfoOutputTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import StaticIpConnectionInfoOutputTypeDef


def get_value() -> StaticIpConnectionInfoOutputTypeDef:
    return {
        "DefaultGateway": ...,
    }


# StaticIpConnectionInfoOutputTypeDef definition

class StaticIpConnectionInfoOutputTypeDef(TypedDict):
    DefaultGateway: str,
    Dns: List[str],
    IpAddress: str,
    Mask: str,
```

## StaticIpConnectionInfoTypeDef

```python
# StaticIpConnectionInfoTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import StaticIpConnectionInfoTypeDef


def get_value() -> StaticIpConnectionInfoTypeDef:
    return {
        "DefaultGateway": ...,
    }


# StaticIpConnectionInfoTypeDef definition

class StaticIpConnectionInfoTypeDef(TypedDict):
    DefaultGateway: str,
    Dns: Sequence[str],
    IpAddress: str,
    Mask: str,
```

## EthernetStatusTypeDef

```python
# EthernetStatusTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import EthernetStatusTypeDef


def get_value() -> EthernetStatusTypeDef:
    return {
        "ConnectionStatus": ...,
    }


# EthernetStatusTypeDef definition

class EthernetStatusTypeDef(TypedDict):
    ConnectionStatus: NotRequired[NetworkConnectionStatusType],  # (1)
    HwAddress: NotRequired[str],
    IpAddress: NotRequired[str],
```

1. See [:material-code-brackets: NetworkConnectionStatusType](./literals.md#networkconnectionstatustype) 
## JobResourceTagsTypeDef

```python
# JobResourceTagsTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import JobResourceTagsTypeDef


def get_value() -> JobResourceTagsTypeDef:
    return {
        "ResourceType": ...,
    }


# JobResourceTagsTypeDef definition

class JobResourceTagsTypeDef(TypedDict):
    ResourceType: JobResourceTypeType,  # (1)
    Tags: Mapping[str, str],
```

1. See [:material-code-brackets: JobResourceTypeType](./literals.md#jobresourcetypetype) 
## ListApplicationInstanceDependenciesRequestTypeDef

```python
# ListApplicationInstanceDependenciesRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ListApplicationInstanceDependenciesRequestTypeDef


def get_value() -> ListApplicationInstanceDependenciesRequestTypeDef:
    return {
        "ApplicationInstanceId": ...,
    }


# ListApplicationInstanceDependenciesRequestTypeDef definition

class ListApplicationInstanceDependenciesRequestTypeDef(TypedDict):
    ApplicationInstanceId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## PackageObjectTypeDef

```python
# PackageObjectTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import PackageObjectTypeDef


def get_value() -> PackageObjectTypeDef:
    return {
        "Name": ...,
    }


# PackageObjectTypeDef definition

class PackageObjectTypeDef(TypedDict):
    Name: str,
    PackageVersion: str,
    PatchVersion: str,
```

## ListApplicationInstanceNodeInstancesRequestTypeDef

```python
# ListApplicationInstanceNodeInstancesRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ListApplicationInstanceNodeInstancesRequestTypeDef


def get_value() -> ListApplicationInstanceNodeInstancesRequestTypeDef:
    return {
        "ApplicationInstanceId": ...,
    }


# ListApplicationInstanceNodeInstancesRequestTypeDef definition

class ListApplicationInstanceNodeInstancesRequestTypeDef(TypedDict):
    ApplicationInstanceId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## NodeInstanceTypeDef

```python
# NodeInstanceTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import NodeInstanceTypeDef


def get_value() -> NodeInstanceTypeDef:
    return {
        "CurrentStatus": ...,
    }


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
## ListApplicationInstancesRequestTypeDef

```python
# ListApplicationInstancesRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ListApplicationInstancesRequestTypeDef


def get_value() -> ListApplicationInstancesRequestTypeDef:
    return {
        "DeviceId": ...,
    }


# ListApplicationInstancesRequestTypeDef definition

class ListApplicationInstancesRequestTypeDef(TypedDict):
    DeviceId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    StatusFilter: NotRequired[StatusFilterType],  # (1)
```

1. See [:material-code-brackets: StatusFilterType](./literals.md#statusfiltertype) 
## ListDevicesJobsRequestTypeDef

```python
# ListDevicesJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ListDevicesJobsRequestTypeDef


def get_value() -> ListDevicesJobsRequestTypeDef:
    return {
        "DeviceId": ...,
    }


# ListDevicesJobsRequestTypeDef definition

class ListDevicesJobsRequestTypeDef(TypedDict):
    DeviceId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListDevicesRequestTypeDef

```python
# ListDevicesRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ListDevicesRequestTypeDef


def get_value() -> ListDevicesRequestTypeDef:
    return {
        "DeviceAggregatedStatusFilter": ...,
    }


# ListDevicesRequestTypeDef definition

class ListDevicesRequestTypeDef(TypedDict):
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
## ListNodeFromTemplateJobsRequestTypeDef

```python
# ListNodeFromTemplateJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ListNodeFromTemplateJobsRequestTypeDef


def get_value() -> ListNodeFromTemplateJobsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListNodeFromTemplateJobsRequestTypeDef definition

class ListNodeFromTemplateJobsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## NodeFromTemplateJobTypeDef

```python
# NodeFromTemplateJobTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import NodeFromTemplateJobTypeDef


def get_value() -> NodeFromTemplateJobTypeDef:
    return {
        "CreatedTime": ...,
    }


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
## ListNodesRequestTypeDef

```python
# ListNodesRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ListNodesRequestTypeDef


def get_value() -> ListNodesRequestTypeDef:
    return {
        "Category": ...,
    }


# ListNodesRequestTypeDef definition

class ListNodesRequestTypeDef(TypedDict):
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
# NodeTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import NodeTypeDef


def get_value() -> NodeTypeDef:
    return {
        "Category": ...,
    }


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
## ListPackageImportJobsRequestTypeDef

```python
# ListPackageImportJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ListPackageImportJobsRequestTypeDef


def get_value() -> ListPackageImportJobsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListPackageImportJobsRequestTypeDef definition

class ListPackageImportJobsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## PackageImportJobTypeDef

```python
# PackageImportJobTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import PackageImportJobTypeDef


def get_value() -> PackageImportJobTypeDef:
    return {
        "CreatedTime": ...,
    }


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
## ListPackagesRequestTypeDef

```python
# ListPackagesRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ListPackagesRequestTypeDef


def get_value() -> ListPackagesRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListPackagesRequestTypeDef definition

class ListPackagesRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## PackageListItemTypeDef

```python
# PackageListItemTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import PackageListItemTypeDef


def get_value() -> PackageListItemTypeDef:
    return {
        "Arn": ...,
    }


# PackageListItemTypeDef definition

class PackageListItemTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    PackageId: NotRequired[str],
    PackageName: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## NtpPayloadOutputTypeDef

```python
# NtpPayloadOutputTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import NtpPayloadOutputTypeDef


def get_value() -> NtpPayloadOutputTypeDef:
    return {
        "NtpServers": ...,
    }


# NtpPayloadOutputTypeDef definition

class NtpPayloadOutputTypeDef(TypedDict):
    NtpServers: List[str],
```

## NtpPayloadTypeDef

```python
# NtpPayloadTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import NtpPayloadTypeDef


def get_value() -> NtpPayloadTypeDef:
    return {
        "NtpServers": ...,
    }


# NtpPayloadTypeDef definition

class NtpPayloadTypeDef(TypedDict):
    NtpServers: Sequence[str],
```

## NtpStatusTypeDef

```python
# NtpStatusTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import NtpStatusTypeDef


def get_value() -> NtpStatusTypeDef:
    return {
        "ConnectionStatus": ...,
    }


# NtpStatusTypeDef definition

class NtpStatusTypeDef(TypedDict):
    ConnectionStatus: NotRequired[NetworkConnectionStatusType],  # (1)
    IpAddress: NotRequired[str],
    NtpServerName: NotRequired[str],
```

1. See [:material-code-brackets: NetworkConnectionStatusType](./literals.md#networkconnectionstatustype) 
## NodeInputPortTypeDef

```python
# NodeInputPortTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import NodeInputPortTypeDef


def get_value() -> NodeInputPortTypeDef:
    return {
        "DefaultValue": ...,
    }


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
# NodeOutputPortTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import NodeOutputPortTypeDef


def get_value() -> NodeOutputPortTypeDef:
    return {
        "Description": ...,
    }


# NodeOutputPortTypeDef definition

class NodeOutputPortTypeDef(TypedDict):
    Description: NotRequired[str],
    Name: NotRequired[str],
    Type: NotRequired[PortTypeType],  # (1)
```

1. See [:material-code-brackets: PortTypeType](./literals.md#porttypetype) 
## NodeSignalTypeDef

```python
# NodeSignalTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import NodeSignalTypeDef


def get_value() -> NodeSignalTypeDef:
    return {
        "NodeInstanceId": ...,
    }


# NodeSignalTypeDef definition

class NodeSignalTypeDef(TypedDict):
    NodeInstanceId: str,
    Signal: NodeSignalValueType,  # (1)
```

1. See [:material-code-brackets: NodeSignalValueType](./literals.md#nodesignalvaluetype) 
## OutPutS3LocationTypeDef

```python
# OutPutS3LocationTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import OutPutS3LocationTypeDef


def get_value() -> OutPutS3LocationTypeDef:
    return {
        "BucketName": ...,
    }


# OutPutS3LocationTypeDef definition

class OutPutS3LocationTypeDef(TypedDict):
    BucketName: str,
    ObjectKey: str,
```

## PackageVersionOutputConfigTypeDef

```python
# PackageVersionOutputConfigTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import PackageVersionOutputConfigTypeDef


def get_value() -> PackageVersionOutputConfigTypeDef:
    return {
        "MarkLatest": ...,
    }


# PackageVersionOutputConfigTypeDef definition

class PackageVersionOutputConfigTypeDef(TypedDict):
    PackageName: str,
    PackageVersion: str,
    MarkLatest: NotRequired[bool],
```

## S3LocationTypeDef

```python
# S3LocationTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import S3LocationTypeDef


def get_value() -> S3LocationTypeDef:
    return {
        "BucketName": ...,
    }


# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    BucketName: str,
    ObjectKey: str,
    Region: NotRequired[str],
```

## RegisterPackageVersionRequestTypeDef

```python
# RegisterPackageVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import RegisterPackageVersionRequestTypeDef


def get_value() -> RegisterPackageVersionRequestTypeDef:
    return {
        "PackageId": ...,
    }


# RegisterPackageVersionRequestTypeDef definition

class RegisterPackageVersionRequestTypeDef(TypedDict):
    PackageId: str,
    PackageVersion: str,
    PatchVersion: str,
    MarkLatest: NotRequired[bool],
    OwnerAccount: NotRequired[str],
```

## RemoveApplicationInstanceRequestTypeDef

```python
# RemoveApplicationInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import RemoveApplicationInstanceRequestTypeDef


def get_value() -> RemoveApplicationInstanceRequestTypeDef:
    return {
        "ApplicationInstanceId": ...,
    }


# RemoveApplicationInstanceRequestTypeDef definition

class RemoveApplicationInstanceRequestTypeDef(TypedDict):
    ApplicationInstanceId: str,
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import TagResourceRequestTypeDef


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

from types_aiobotocore_panorama.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateDeviceMetadataRequestTypeDef

```python
# UpdateDeviceMetadataRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import UpdateDeviceMetadataRequestTypeDef


def get_value() -> UpdateDeviceMetadataRequestTypeDef:
    return {
        "DeviceId": ...,
    }


# UpdateDeviceMetadataRequestTypeDef definition

class UpdateDeviceMetadataRequestTypeDef(TypedDict):
    DeviceId: str,
    Description: NotRequired[str],
```

## ApplicationInstanceTypeDef

```python
# ApplicationInstanceTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ApplicationInstanceTypeDef


def get_value() -> ApplicationInstanceTypeDef:
    return {
        "ApplicationInstanceId": ...,
    }


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
## CreateApplicationInstanceRequestTypeDef

```python
# CreateApplicationInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import CreateApplicationInstanceRequestTypeDef


def get_value() -> CreateApplicationInstanceRequestTypeDef:
    return {
        "DefaultRuntimeContextDevice": ...,
    }


# CreateApplicationInstanceRequestTypeDef definition

class CreateApplicationInstanceRequestTypeDef(TypedDict):
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
# CreateApplicationInstanceResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import CreateApplicationInstanceResponseTypeDef


def get_value() -> CreateApplicationInstanceResponseTypeDef:
    return {
        "ApplicationInstanceId": ...,
    }


# CreateApplicationInstanceResponseTypeDef definition

class CreateApplicationInstanceResponseTypeDef(TypedDict):
    ApplicationInstanceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateNodeFromTemplateJobResponseTypeDef

```python
# CreateNodeFromTemplateJobResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import CreateNodeFromTemplateJobResponseTypeDef


def get_value() -> CreateNodeFromTemplateJobResponseTypeDef:
    return {
        "JobId": ...,
    }


# CreateNodeFromTemplateJobResponseTypeDef definition

class CreateNodeFromTemplateJobResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePackageImportJobResponseTypeDef

```python
# CreatePackageImportJobResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import CreatePackageImportJobResponseTypeDef


def get_value() -> CreatePackageImportJobResponseTypeDef:
    return {
        "JobId": ...,
    }


# CreatePackageImportJobResponseTypeDef definition

class CreatePackageImportJobResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDeviceResponseTypeDef

```python
# DeleteDeviceResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DeleteDeviceResponseTypeDef


def get_value() -> DeleteDeviceResponseTypeDef:
    return {
        "DeviceId": ...,
    }


# DeleteDeviceResponseTypeDef definition

class DeleteDeviceResponseTypeDef(TypedDict):
    DeviceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeApplicationInstanceDetailsResponseTypeDef

```python
# DescribeApplicationInstanceDetailsResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DescribeApplicationInstanceDetailsResponseTypeDef


def get_value() -> DescribeApplicationInstanceDetailsResponseTypeDef:
    return {
        "ApplicationInstanceId": ...,
    }


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
# DescribeApplicationInstanceResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DescribeApplicationInstanceResponseTypeDef


def get_value() -> DescribeApplicationInstanceResponseTypeDef:
    return {
        "ApplicationInstanceId": ...,
    }


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
# DescribeDeviceJobResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DescribeDeviceJobResponseTypeDef


def get_value() -> DescribeDeviceJobResponseTypeDef:
    return {
        "CreatedTime": ...,
    }


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
# DescribePackageVersionResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DescribePackageVersionResponseTypeDef


def get_value() -> DescribePackageVersionResponseTypeDef:
    return {
        "IsLatestPatch": ...,
    }


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
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ListTagsForResourceResponseTypeDef


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
## ProvisionDeviceResponseTypeDef

```python
# ProvisionDeviceResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ProvisionDeviceResponseTypeDef


def get_value() -> ProvisionDeviceResponseTypeDef:
    return {
        "Arn": ...,
    }


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
# SignalApplicationInstanceNodeInstancesResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import SignalApplicationInstanceNodeInstancesResponseTypeDef


def get_value() -> SignalApplicationInstanceNodeInstancesResponseTypeDef:
    return {
        "ApplicationInstanceId": ...,
    }


# SignalApplicationInstanceNodeInstancesResponseTypeDef definition

class SignalApplicationInstanceNodeInstancesResponseTypeDef(TypedDict):
    ApplicationInstanceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDeviceMetadataResponseTypeDef

```python
# UpdateDeviceMetadataResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import UpdateDeviceMetadataResponseTypeDef


def get_value() -> UpdateDeviceMetadataResponseTypeDef:
    return {
        "DeviceId": ...,
    }


# UpdateDeviceMetadataResponseTypeDef definition

class UpdateDeviceMetadataResponseTypeDef(TypedDict):
    DeviceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobForDevicesResponseTypeDef

```python
# CreateJobForDevicesResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import CreateJobForDevicesResponseTypeDef


def get_value() -> CreateJobForDevicesResponseTypeDef:
    return {
        "Jobs": ...,
    }


# CreateJobForDevicesResponseTypeDef definition

class CreateJobForDevicesResponseTypeDef(TypedDict):
    Jobs: List[JobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePackageResponseTypeDef

```python
# CreatePackageResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import CreatePackageResponseTypeDef


def get_value() -> CreatePackageResponseTypeDef:
    return {
        "Arn": ...,
    }


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
# DescribePackageResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DescribePackageResponseTypeDef


def get_value() -> DescribePackageResponseTypeDef:
    return {
        "Arn": ...,
    }


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
# DeviceTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DeviceTypeDef


def get_value() -> DeviceTypeDef:
    return {
        "Brand": ...,
    }


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
# DescribeNodeFromTemplateJobResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DescribeNodeFromTemplateJobResponseTypeDef


def get_value() -> DescribeNodeFromTemplateJobResponseTypeDef:
    return {
        "CreatedTime": ...,
    }


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
# DeviceJobConfigTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DeviceJobConfigTypeDef


def get_value() -> DeviceJobConfigTypeDef:
    return {
        "OTAJobConfig": ...,
    }


# DeviceJobConfigTypeDef definition

class DeviceJobConfigTypeDef(TypedDict):
    OTAJobConfig: NotRequired[OTAJobConfigTypeDef],  # (1)
```

1. See [:material-code-braces: OTAJobConfigTypeDef](./type_defs.md#otajobconfigtypedef) 
## ListDevicesJobsResponseTypeDef

```python
# ListDevicesJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ListDevicesJobsResponseTypeDef


def get_value() -> ListDevicesJobsResponseTypeDef:
    return {
        "DeviceJobs": ...,
    }


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
# EthernetPayloadOutputTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import EthernetPayloadOutputTypeDef


def get_value() -> EthernetPayloadOutputTypeDef:
    return {
        "ConnectionType": ...,
    }


# EthernetPayloadOutputTypeDef definition

class EthernetPayloadOutputTypeDef(TypedDict):
    ConnectionType: ConnectionTypeType,  # (1)
    StaticIpConnectionInfo: NotRequired[StaticIpConnectionInfoOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
2. See [:material-code-braces: StaticIpConnectionInfoOutputTypeDef](./type_defs.md#staticipconnectioninfooutputtypedef) 
## EthernetPayloadTypeDef

```python
# EthernetPayloadTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import EthernetPayloadTypeDef


def get_value() -> EthernetPayloadTypeDef:
    return {
        "ConnectionType": ...,
    }


# EthernetPayloadTypeDef definition

class EthernetPayloadTypeDef(TypedDict):
    ConnectionType: ConnectionTypeType,  # (1)
    StaticIpConnectionInfo: NotRequired[StaticIpConnectionInfoTypeDef],  # (2)
```

1. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
2. See [:material-code-braces: StaticIpConnectionInfoTypeDef](./type_defs.md#staticipconnectioninfotypedef) 
## ListApplicationInstanceDependenciesResponseTypeDef

```python
# ListApplicationInstanceDependenciesResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ListApplicationInstanceDependenciesResponseTypeDef


def get_value() -> ListApplicationInstanceDependenciesResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# ListApplicationInstanceNodeInstancesResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ListApplicationInstanceNodeInstancesResponseTypeDef


def get_value() -> ListApplicationInstanceNodeInstancesResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# ListNodeFromTemplateJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ListNodeFromTemplateJobsResponseTypeDef


def get_value() -> ListNodeFromTemplateJobsResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# ListNodesResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ListNodesResponseTypeDef


def get_value() -> ListNodesResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# ListPackageImportJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ListPackageImportJobsResponseTypeDef


def get_value() -> ListPackageImportJobsResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# ListPackagesResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ListPackagesResponseTypeDef


def get_value() -> ListPackagesResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# NetworkStatusTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import NetworkStatusTypeDef


def get_value() -> NetworkStatusTypeDef:
    return {
        "Ethernet0Status": ...,
    }


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
# NodeInterfaceTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import NodeInterfaceTypeDef


def get_value() -> NodeInterfaceTypeDef:
    return {
        "Inputs": ...,
    }


# NodeInterfaceTypeDef definition

class NodeInterfaceTypeDef(TypedDict):
    Inputs: List[NodeInputPortTypeDef],  # (1)
    Outputs: List[NodeOutputPortTypeDef],  # (2)
```

1. See [:material-code-braces: NodeInputPortTypeDef](./type_defs.md#nodeinputporttypedef) 
2. See [:material-code-braces: NodeOutputPortTypeDef](./type_defs.md#nodeoutputporttypedef) 
## SignalApplicationInstanceNodeInstancesRequestTypeDef

```python
# SignalApplicationInstanceNodeInstancesRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import SignalApplicationInstanceNodeInstancesRequestTypeDef


def get_value() -> SignalApplicationInstanceNodeInstancesRequestTypeDef:
    return {
        "ApplicationInstanceId": ...,
    }


# SignalApplicationInstanceNodeInstancesRequestTypeDef definition

class SignalApplicationInstanceNodeInstancesRequestTypeDef(TypedDict):
    ApplicationInstanceId: str,
    NodeSignals: Sequence[NodeSignalTypeDef],  # (1)
```

1. See [:material-code-braces: NodeSignalTypeDef](./type_defs.md#nodesignaltypedef) 
## PackageImportJobOutputTypeDef

```python
# PackageImportJobOutputTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import PackageImportJobOutputTypeDef


def get_value() -> PackageImportJobOutputTypeDef:
    return {
        "OutputS3Location": ...,
    }


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
# PackageImportJobOutputConfigTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import PackageImportJobOutputConfigTypeDef


def get_value() -> PackageImportJobOutputConfigTypeDef:
    return {
        "PackageVersionOutputConfig": ...,
    }


# PackageImportJobOutputConfigTypeDef definition

class PackageImportJobOutputConfigTypeDef(TypedDict):
    PackageVersionOutputConfig: NotRequired[PackageVersionOutputConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PackageVersionOutputConfigTypeDef](./type_defs.md#packageversionoutputconfigtypedef) 
## PackageVersionInputConfigTypeDef

```python
# PackageVersionInputConfigTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import PackageVersionInputConfigTypeDef


def get_value() -> PackageVersionInputConfigTypeDef:
    return {
        "S3Location": ...,
    }


# PackageVersionInputConfigTypeDef definition

class PackageVersionInputConfigTypeDef(TypedDict):
    S3Location: S3LocationTypeDef,  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## ListApplicationInstancesResponseTypeDef

```python
# ListApplicationInstancesResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ListApplicationInstancesResponseTypeDef


def get_value() -> ListApplicationInstancesResponseTypeDef:
    return {
        "ApplicationInstances": ...,
    }


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
# ListDevicesResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ListDevicesResponseTypeDef


def get_value() -> ListDevicesResponseTypeDef:
    return {
        "Devices": ...,
    }


# ListDevicesResponseTypeDef definition

class ListDevicesResponseTypeDef(TypedDict):
    Devices: List[DeviceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DeviceTypeDef](./type_defs.md#devicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobForDevicesRequestTypeDef

```python
# CreateJobForDevicesRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import CreateJobForDevicesRequestTypeDef


def get_value() -> CreateJobForDevicesRequestTypeDef:
    return {
        "DeviceIds": ...,
    }


# CreateJobForDevicesRequestTypeDef definition

class CreateJobForDevicesRequestTypeDef(TypedDict):
    DeviceIds: Sequence[str],
    JobType: JobTypeType,  # (1)
    DeviceJobConfig: NotRequired[DeviceJobConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
2. See [:material-code-braces: DeviceJobConfigTypeDef](./type_defs.md#devicejobconfigtypedef) 
## NetworkPayloadOutputTypeDef

```python
# NetworkPayloadOutputTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import NetworkPayloadOutputTypeDef


def get_value() -> NetworkPayloadOutputTypeDef:
    return {
        "Ethernet0": ...,
    }


# NetworkPayloadOutputTypeDef definition

class NetworkPayloadOutputTypeDef(TypedDict):
    Ethernet0: NotRequired[EthernetPayloadOutputTypeDef],  # (1)
    Ethernet1: NotRequired[EthernetPayloadOutputTypeDef],  # (1)
    Ntp: NotRequired[NtpPayloadOutputTypeDef],  # (3)
```

1. See [:material-code-braces: EthernetPayloadOutputTypeDef](./type_defs.md#ethernetpayloadoutputtypedef) 
2. See [:material-code-braces: EthernetPayloadOutputTypeDef](./type_defs.md#ethernetpayloadoutputtypedef) 
3. See [:material-code-braces: NtpPayloadOutputTypeDef](./type_defs.md#ntppayloadoutputtypedef) 
## NetworkPayloadTypeDef

```python
# NetworkPayloadTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import NetworkPayloadTypeDef


def get_value() -> NetworkPayloadTypeDef:
    return {
        "Ethernet0": ...,
    }


# NetworkPayloadTypeDef definition

class NetworkPayloadTypeDef(TypedDict):
    Ethernet0: NotRequired[EthernetPayloadTypeDef],  # (1)
    Ethernet1: NotRequired[EthernetPayloadTypeDef],  # (1)
    Ntp: NotRequired[NtpPayloadTypeDef],  # (3)
```

1. See [:material-code-braces: EthernetPayloadTypeDef](./type_defs.md#ethernetpayloadtypedef) 
2. See [:material-code-braces: EthernetPayloadTypeDef](./type_defs.md#ethernetpayloadtypedef) 
3. See [:material-code-braces: NtpPayloadTypeDef](./type_defs.md#ntppayloadtypedef) 
## CreateNodeFromTemplateJobRequestTypeDef

```python
# CreateNodeFromTemplateJobRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import CreateNodeFromTemplateJobRequestTypeDef


def get_value() -> CreateNodeFromTemplateJobRequestTypeDef:
    return {
        "NodeName": ...,
    }


# CreateNodeFromTemplateJobRequestTypeDef definition

class CreateNodeFromTemplateJobRequestTypeDef(TypedDict):
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
## DescribeNodeResponseTypeDef

```python
# DescribeNodeResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DescribeNodeResponseTypeDef


def get_value() -> DescribeNodeResponseTypeDef:
    return {
        "AssetName": ...,
    }


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
# PackageImportJobInputConfigTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import PackageImportJobInputConfigTypeDef


def get_value() -> PackageImportJobInputConfigTypeDef:
    return {
        "PackageVersionInputConfig": ...,
    }


# PackageImportJobInputConfigTypeDef definition

class PackageImportJobInputConfigTypeDef(TypedDict):
    PackageVersionInputConfig: NotRequired[PackageVersionInputConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PackageVersionInputConfigTypeDef](./type_defs.md#packageversioninputconfigtypedef) 
## DescribeDeviceResponseTypeDef

```python
# DescribeDeviceResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DescribeDeviceResponseTypeDef


def get_value() -> DescribeDeviceResponseTypeDef:
    return {
        "AlternateSoftwares": ...,
    }


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
## CreatePackageImportJobRequestTypeDef

```python
# CreatePackageImportJobRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import CreatePackageImportJobRequestTypeDef


def get_value() -> CreatePackageImportJobRequestTypeDef:
    return {
        "ClientToken": ...,
    }


# CreatePackageImportJobRequestTypeDef definition

class CreatePackageImportJobRequestTypeDef(TypedDict):
    ClientToken: str,
    InputConfig: PackageImportJobInputConfigTypeDef,  # (1)
    JobType: PackageImportJobTypeType,  # (2)
    OutputConfig: PackageImportJobOutputConfigTypeDef,  # (3)
    JobTags: NotRequired[Sequence[JobResourceTagsUnionTypeDef]],  # (4)
```

1. See [:material-code-braces: PackageImportJobInputConfigTypeDef](./type_defs.md#packageimportjobinputconfigtypedef) 
2. See [:material-code-brackets: PackageImportJobTypeType](./literals.md#packageimportjobtypetype) 
3. See [:material-code-braces: PackageImportJobOutputConfigTypeDef](./type_defs.md#packageimportjoboutputconfigtypedef) 
4. See [:material-code-braces: JobResourceTagsTypeDef](./type_defs.md#jobresourcetagstypedef) [:material-code-braces: JobResourceTagsOutputTypeDef](./type_defs.md#jobresourcetagsoutputtypedef) 
## DescribePackageImportJobResponseTypeDef

```python
# DescribePackageImportJobResponseTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import DescribePackageImportJobResponseTypeDef


def get_value() -> DescribePackageImportJobResponseTypeDef:
    return {
        "ClientToken": ...,
    }


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
## ProvisionDeviceRequestTypeDef

```python
# ProvisionDeviceRequestTypeDef TypedDict usage example

from types_aiobotocore_panorama.type_defs import ProvisionDeviceRequestTypeDef


def get_value() -> ProvisionDeviceRequestTypeDef:
    return {
        "Name": ...,
    }


# ProvisionDeviceRequestTypeDef definition

class ProvisionDeviceRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    NetworkingConfiguration: NotRequired[NetworkPayloadUnionTypeDef],  # (1)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: NetworkPayloadTypeDef](./type_defs.md#networkpayloadtypedef) [:material-code-braces: NetworkPayloadOutputTypeDef](./type_defs.md#networkpayloadoutputtypedef) 
