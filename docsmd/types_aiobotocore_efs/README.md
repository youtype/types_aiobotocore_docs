# EFS module

> [Index](../README.md) > EFS


!!! note ""

    Auto-generated documentation for [EFS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#efs)
    type annotations stubs module [types-aiobotocore-efs](https://pypi.org/project/types-aiobotocore-efs/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `EFS` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `EFS` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[efs]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[efs]'

# standalone installation
python -m pip install types-aiobotocore-efs
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-efs
```

## Usage

Code samples can be found in [Examples](./usage.md).

## EFSClient

Type annotations and code completion for  `#!python session.create_client("efs")` as [EFSClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client)

```python
# EFSClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_efs.client import EFSClient


session = get_session()
async with session.create_client("efs") as client:
    client: EFSClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("efs").get_paginator("...")`.

```python
# DescribeAccessPointsPaginator usage example

from types_aiobotocore_efs.paginator import DescribeAccessPointsPaginator

def get_describe_access_points_paginator() -> DescribeAccessPointsPaginator:
    return client.get_paginator("describe_access_points"))
```

- [DescribeAccessPointsPaginator](./paginators.md#describeaccesspointspaginator)
- [DescribeFileSystemsPaginator](./paginators.md#describefilesystemspaginator)
- [DescribeMountTargetsPaginator](./paginators.md#describemounttargetspaginator)
- [DescribeReplicationConfigurationsPaginator](./paginators.md#describereplicationconfigurationspaginator)
- [DescribeTagsPaginator](./paginators.md#describetagspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DeletionModeType usage example

from types_aiobotocore_efs.literals import DeletionModeType

def get_value() -> DeletionModeType:
    return "ALL_CONFIGURATIONS"
```

- [DeletionModeType](./literals.md#deletionmodetype)
- [DescribeAccessPointsPaginatorName](./literals.md#describeaccesspointspaginatorname)
- [DescribeFileSystemsPaginatorName](./literals.md#describefilesystemspaginatorname)
- [DescribeMountTargetsPaginatorName](./literals.md#describemounttargetspaginatorname)
- [DescribeReplicationConfigurationsPaginatorName](./literals.md#describereplicationconfigurationspaginatorname)
- [DescribeTagsPaginatorName](./literals.md#describetagspaginatorname)
- [LifeCycleStateType](./literals.md#lifecyclestatetype)
- [PerformanceModeType](./literals.md#performancemodetype)
- [ReplicationOverwriteProtectionType](./literals.md#replicationoverwriteprotectiontype)
- [ReplicationStatusType](./literals.md#replicationstatustype)
- [ResourceIdTypeType](./literals.md#resourceidtypetype)
- [ResourceType](./literals.md#resourcetype)
- [StatusType](./literals.md#statustype)
- [ThroughputModeType](./literals.md#throughputmodetype)
- [TransitionToArchiveRulesType](./literals.md#transitiontoarchiverulestype)
- [TransitionToIARulesType](./literals.md#transitiontoiarulestype)
- [TransitionToPrimaryStorageClassRulesType](./literals.md#transitiontoprimarystorageclassrulestype)
- [EFSServiceName](./literals.md#efsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [PosixUserOutputTypeDef](./type_defs.md#posixuseroutputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [BackupPolicyTypeDef](./type_defs.md#backuppolicytypedef)
- [PosixUserTypeDef](./type_defs.md#posixusertypedef)
- [CreateMountTargetRequestRequestTypeDef](./type_defs.md#createmounttargetrequestrequesttypedef)
- [DestinationToCreateTypeDef](./type_defs.md#destinationtocreatetypedef)
- [CreationInfoTypeDef](./type_defs.md#creationinfotypedef)
- [DeleteAccessPointRequestRequestTypeDef](./type_defs.md#deleteaccesspointrequestrequesttypedef)
- [DeleteFileSystemPolicyRequestRequestTypeDef](./type_defs.md#deletefilesystempolicyrequestrequesttypedef)
- [DeleteFileSystemRequestRequestTypeDef](./type_defs.md#deletefilesystemrequestrequesttypedef)
- [DeleteMountTargetRequestRequestTypeDef](./type_defs.md#deletemounttargetrequestrequesttypedef)
- [DeleteReplicationConfigurationRequestRequestTypeDef](./type_defs.md#deletereplicationconfigurationrequestrequesttypedef)
- [DeleteTagsRequestRequestTypeDef](./type_defs.md#deletetagsrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeAccessPointsRequestRequestTypeDef](./type_defs.md#describeaccesspointsrequestrequesttypedef)
- [DescribeAccountPreferencesRequestRequestTypeDef](./type_defs.md#describeaccountpreferencesrequestrequesttypedef)
- [ResourceIdPreferenceTypeDef](./type_defs.md#resourceidpreferencetypedef)
- [DescribeBackupPolicyRequestRequestTypeDef](./type_defs.md#describebackuppolicyrequestrequesttypedef)
- [DescribeFileSystemPolicyRequestRequestTypeDef](./type_defs.md#describefilesystempolicyrequestrequesttypedef)
- [DescribeFileSystemsRequestRequestTypeDef](./type_defs.md#describefilesystemsrequestrequesttypedef)
- [DescribeLifecycleConfigurationRequestRequestTypeDef](./type_defs.md#describelifecycleconfigurationrequestrequesttypedef)
- [DescribeMountTargetSecurityGroupsRequestRequestTypeDef](./type_defs.md#describemounttargetsecuritygroupsrequestrequesttypedef)
- [DescribeMountTargetsRequestRequestTypeDef](./type_defs.md#describemounttargetsrequestrequesttypedef)
- [MountTargetDescriptionTypeDef](./type_defs.md#mounttargetdescriptiontypedef)
- [DescribeReplicationConfigurationsRequestRequestTypeDef](./type_defs.md#describereplicationconfigurationsrequestrequesttypedef)
- [DescribeTagsRequestRequestTypeDef](./type_defs.md#describetagsrequestrequesttypedef)
- [DestinationTypeDef](./type_defs.md#destinationtypedef)
- [FileSystemProtectionDescriptionTypeDef](./type_defs.md#filesystemprotectiondescriptiontypedef)
- [FileSystemSizeTypeDef](./type_defs.md#filesystemsizetypedef)
- [LifecyclePolicyTypeDef](./type_defs.md#lifecyclepolicytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ModifyMountTargetSecurityGroupsRequestRequestTypeDef](./type_defs.md#modifymounttargetsecuritygroupsrequestrequesttypedef)
- [PutAccountPreferencesRequestRequestTypeDef](./type_defs.md#putaccountpreferencesrequestrequesttypedef)
- [PutFileSystemPolicyRequestRequestTypeDef](./type_defs.md#putfilesystempolicyrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateFileSystemProtectionRequestRequestTypeDef](./type_defs.md#updatefilesystemprotectionrequestrequesttypedef)
- [UpdateFileSystemRequestRequestTypeDef](./type_defs.md#updatefilesystemrequestrequesttypedef)
- [DescribeMountTargetSecurityGroupsResponseTypeDef](./type_defs.md#describemounttargetsecuritygroupsresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [FileSystemPolicyDescriptionTypeDef](./type_defs.md#filesystempolicydescriptiontypedef)
- [FileSystemProtectionDescriptionResponseTypeDef](./type_defs.md#filesystemprotectiondescriptionresponsetypedef)
- [MountTargetDescriptionResponseTypeDef](./type_defs.md#mounttargetdescriptionresponsetypedef)
- [CreateFileSystemRequestRequestTypeDef](./type_defs.md#createfilesystemrequestrequesttypedef)
- [CreateTagsRequestRequestTypeDef](./type_defs.md#createtagsrequestrequesttypedef)
- [DescribeTagsResponseTypeDef](./type_defs.md#describetagsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [BackupPolicyDescriptionTypeDef](./type_defs.md#backuppolicydescriptiontypedef)
- [PutBackupPolicyRequestRequestTypeDef](./type_defs.md#putbackuppolicyrequestrequesttypedef)
- [CreateReplicationConfigurationRequestRequestTypeDef](./type_defs.md#createreplicationconfigurationrequestrequesttypedef)
- [RootDirectoryTypeDef](./type_defs.md#rootdirectorytypedef)
- [DescribeAccessPointsRequestPaginateTypeDef](./type_defs.md#describeaccesspointsrequestpaginatetypedef)
- [DescribeFileSystemsRequestPaginateTypeDef](./type_defs.md#describefilesystemsrequestpaginatetypedef)
- [DescribeMountTargetsRequestPaginateTypeDef](./type_defs.md#describemounttargetsrequestpaginatetypedef)
- [DescribeReplicationConfigurationsRequestPaginateTypeDef](./type_defs.md#describereplicationconfigurationsrequestpaginatetypedef)
- [DescribeTagsRequestPaginateTypeDef](./type_defs.md#describetagsrequestpaginatetypedef)
- [DescribeAccountPreferencesResponseTypeDef](./type_defs.md#describeaccountpreferencesresponsetypedef)
- [PutAccountPreferencesResponseTypeDef](./type_defs.md#putaccountpreferencesresponsetypedef)
- [DescribeMountTargetsResponseTypeDef](./type_defs.md#describemounttargetsresponsetypedef)
- [ReplicationConfigurationDescriptionResponseTypeDef](./type_defs.md#replicationconfigurationdescriptionresponsetypedef)
- [ReplicationConfigurationDescriptionTypeDef](./type_defs.md#replicationconfigurationdescriptiontypedef)
- [FileSystemDescriptionResponseTypeDef](./type_defs.md#filesystemdescriptionresponsetypedef)
- [FileSystemDescriptionTypeDef](./type_defs.md#filesystemdescriptiontypedef)
- [LifecycleConfigurationDescriptionTypeDef](./type_defs.md#lifecycleconfigurationdescriptiontypedef)
- [PutLifecycleConfigurationRequestRequestTypeDef](./type_defs.md#putlifecycleconfigurationrequestrequesttypedef)
- [AccessPointDescriptionResponseTypeDef](./type_defs.md#accesspointdescriptionresponsetypedef)
- [AccessPointDescriptionTypeDef](./type_defs.md#accesspointdescriptiontypedef)
- [CreateAccessPointRequestRequestTypeDef](./type_defs.md#createaccesspointrequestrequesttypedef)
- [DescribeReplicationConfigurationsResponseTypeDef](./type_defs.md#describereplicationconfigurationsresponsetypedef)
- [DescribeFileSystemsResponseTypeDef](./type_defs.md#describefilesystemsresponsetypedef)
- [DescribeAccessPointsResponseTypeDef](./type_defs.md#describeaccesspointsresponsetypedef)

