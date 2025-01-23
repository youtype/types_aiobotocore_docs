# FSx module

> [Index](../README.md) > FSx


!!! note ""

    Auto-generated documentation for [FSx](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#fsx)
    type annotations stubs module [types-aiobotocore-fsx](https://pypi.org/project/types-aiobotocore-fsx/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `FSx` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `FSx` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[fsx]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[fsx]'

# standalone installation
python -m pip install types-aiobotocore-fsx
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-fsx
```

## Usage

Code samples can be found in [Examples](./usage.md).

## FSxClient

Type annotations and code completion for  `#!python session.create_client("fsx")` as [FSxClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# FSxClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_fsx.client import FSxClient


session = get_session()
async with session.create_client("fsx") as client:
    client: FSxClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("fsx").get_paginator("...")`.

```python
# DescribeBackupsPaginator usage example

from types_aiobotocore_fsx.paginator import DescribeBackupsPaginator

def get_describe_backups_paginator() -> DescribeBackupsPaginator:
    return client.get_paginator("describe_backups"))
```

- [DescribeBackupsPaginator](./paginators.md#describebackupspaginator)
- [DescribeFileSystemsPaginator](./paginators.md#describefilesystemspaginator)
- [DescribeStorageVirtualMachinesPaginator](./paginators.md#describestoragevirtualmachinespaginator)
- [DescribeVolumesPaginator](./paginators.md#describevolumespaginator)
- [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AdministrativeActionTypeType usage example

from types_aiobotocore_fsx.literals import AdministrativeActionTypeType

def get_value() -> AdministrativeActionTypeType:
    return "DOWNLOAD_DATA_FROM_BACKUP"
```

- [AdministrativeActionTypeType](./literals.md#administrativeactiontypetype)
- [AliasLifecycleType](./literals.md#aliaslifecycletype)
- [AutoImportPolicyTypeType](./literals.md#autoimportpolicytypetype)
- [AutocommitPeriodTypeType](./literals.md#autocommitperiodtypetype)
- [BackupLifecycleType](./literals.md#backuplifecycletype)
- [BackupTypeType](./literals.md#backuptypetype)
- [DataCompressionTypeType](./literals.md#datacompressiontypetype)
- [DataRepositoryLifecycleType](./literals.md#datarepositorylifecycletype)
- [DataRepositoryTaskFilterNameType](./literals.md#datarepositorytaskfilternametype)
- [DataRepositoryTaskLifecycleType](./literals.md#datarepositorytasklifecycletype)
- [DataRepositoryTaskTypeType](./literals.md#datarepositorytasktypetype)
- [DeleteFileSystemOpenZFSOptionType](./literals.md#deletefilesystemopenzfsoptiontype)
- [DeleteOpenZFSVolumeOptionType](./literals.md#deleteopenzfsvolumeoptiontype)
- [DescribeBackupsPaginatorName](./literals.md#describebackupspaginatorname)
- [DescribeFileSystemsPaginatorName](./literals.md#describefilesystemspaginatorname)
- [DescribeStorageVirtualMachinesPaginatorName](./literals.md#describestoragevirtualmachinespaginatorname)
- [DescribeVolumesPaginatorName](./literals.md#describevolumespaginatorname)
- [DiskIopsConfigurationModeType](./literals.md#diskiopsconfigurationmodetype)
- [DriveCacheTypeType](./literals.md#drivecachetypetype)
- [EventTypeType](./literals.md#eventtypetype)
- [FileCacheLifecycleType](./literals.md#filecachelifecycletype)
- [FileCacheLustreDeploymentTypeType](./literals.md#filecachelustredeploymenttypetype)
- [FileCacheTypeType](./literals.md#filecachetypetype)
- [FileSystemLifecycleType](./literals.md#filesystemlifecycletype)
- [FileSystemMaintenanceOperationType](./literals.md#filesystemmaintenanceoperationtype)
- [FileSystemTypeType](./literals.md#filesystemtypetype)
- [FilterNameType](./literals.md#filternametype)
- [FlexCacheEndpointTypeType](./literals.md#flexcacheendpointtypetype)
- [InputOntapVolumeTypeType](./literals.md#inputontapvolumetypetype)
- [ListTagsForResourcePaginatorName](./literals.md#listtagsforresourcepaginatorname)
- [LustreAccessAuditLogLevelType](./literals.md#lustreaccessauditlogleveltype)
- [LustreDeploymentTypeType](./literals.md#lustredeploymenttypetype)
- [MetadataConfigurationModeType](./literals.md#metadataconfigurationmodetype)
- [NfsVersionType](./literals.md#nfsversiontype)
- [OntapDeploymentTypeType](./literals.md#ontapdeploymenttypetype)
- [OntapVolumeTypeType](./literals.md#ontapvolumetypetype)
- [OpenZFSCopyStrategyType](./literals.md#openzfscopystrategytype)
- [OpenZFSDataCompressionTypeType](./literals.md#openzfsdatacompressiontypetype)
- [OpenZFSDeploymentTypeType](./literals.md#openzfsdeploymenttypetype)
- [OpenZFSQuotaTypeType](./literals.md#openzfsquotatypetype)
- [OpenZFSReadCacheSizingModeType](./literals.md#openzfsreadcachesizingmodetype)
- [PrivilegedDeleteType](./literals.md#privilegeddeletetype)
- [ReportFormatType](./literals.md#reportformattype)
- [ReportScopeType](./literals.md#reportscopetype)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [RestoreOpenZFSVolumeOptionType](./literals.md#restoreopenzfsvolumeoptiontype)
- [RetentionPeriodTypeType](./literals.md#retentionperiodtypetype)
- [SecurityStyleType](./literals.md#securitystyletype)
- [SnaplockTypeType](./literals.md#snaplocktypetype)
- [SnapshotFilterNameType](./literals.md#snapshotfilternametype)
- [SnapshotLifecycleType](./literals.md#snapshotlifecycletype)
- [StatusType](./literals.md#statustype)
- [StorageTypeType](./literals.md#storagetypetype)
- [StorageVirtualMachineFilterNameType](./literals.md#storagevirtualmachinefilternametype)
- [StorageVirtualMachineLifecycleType](./literals.md#storagevirtualmachinelifecycletype)
- [StorageVirtualMachineRootVolumeSecurityStyleType](./literals.md#storagevirtualmachinerootvolumesecuritystyletype)
- [StorageVirtualMachineSubtypeType](./literals.md#storagevirtualmachinesubtypetype)
- [TieringPolicyNameType](./literals.md#tieringpolicynametype)
- [UnitType](./literals.md#unittype)
- [UpdateOpenZFSVolumeOptionType](./literals.md#updateopenzfsvolumeoptiontype)
- [VolumeFilterNameType](./literals.md#volumefilternametype)
- [VolumeLifecycleType](./literals.md#volumelifecycletype)
- [VolumeStyleType](./literals.md#volumestyletype)
- [VolumeTypeType](./literals.md#volumetypetype)
- [WindowsAccessAuditLogLevelType](./literals.md#windowsaccessauditlogleveltype)
- [WindowsDeploymentTypeType](./literals.md#windowsdeploymenttypetype)
- [FSxServiceName](./literals.md#fsxservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ActiveDirectoryBackupAttributesTypeDef](./type_defs.md#activedirectorybackupattributestypedef)
- [AdministrativeActionFailureDetailsTypeDef](./type_defs.md#administrativeactionfailuredetailstypedef)
- [AggregateConfigurationTypeDef](./type_defs.md#aggregateconfigurationtypedef)
- [AliasTypeDef](./type_defs.md#aliastypedef)
- [AssociateFileSystemAliasesRequestRequestTypeDef](./type_defs.md#associatefilesystemaliasesrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AutoExportPolicyOutputTypeDef](./type_defs.md#autoexportpolicyoutputtypedef)
- [AutoExportPolicyTypeDef](./type_defs.md#autoexportpolicytypedef)
- [AutoImportPolicyOutputTypeDef](./type_defs.md#autoimportpolicyoutputtypedef)
- [AutoImportPolicyTypeDef](./type_defs.md#autoimportpolicytypedef)
- [AutocommitPeriodTypeDef](./type_defs.md#autocommitperiodtypedef)
- [BackupFailureDetailsTypeDef](./type_defs.md#backupfailuredetailstypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [CancelDataRepositoryTaskRequestRequestTypeDef](./type_defs.md#canceldatarepositorytaskrequestrequesttypedef)
- [CompletionReportTypeDef](./type_defs.md#completionreporttypedef)
- [CopySnapshotAndUpdateVolumeRequestRequestTypeDef](./type_defs.md#copysnapshotandupdatevolumerequestrequesttypedef)
- [CreateAggregateConfigurationTypeDef](./type_defs.md#createaggregateconfigurationtypedef)
- [FileCacheLustreMetadataConfigurationTypeDef](./type_defs.md#filecachelustremetadataconfigurationtypedef)
- [CreateFileSystemLustreMetadataConfigurationTypeDef](./type_defs.md#createfilesystemlustremetadataconfigurationtypedef)
- [LustreLogCreateConfigurationTypeDef](./type_defs.md#lustrelogcreateconfigurationtypedef)
- [DiskIopsConfigurationTypeDef](./type_defs.md#diskiopsconfigurationtypedef)
- [OpenZFSReadCacheConfigurationTypeDef](./type_defs.md#openzfsreadcacheconfigurationtypedef)
- [SelfManagedActiveDirectoryConfigurationTypeDef](./type_defs.md#selfmanagedactivedirectoryconfigurationtypedef)
- [WindowsAuditLogCreateConfigurationTypeDef](./type_defs.md#windowsauditlogcreateconfigurationtypedef)
- [TieringPolicyTypeDef](./type_defs.md#tieringpolicytypedef)
- [CreateOpenZFSOriginSnapshotConfigurationTypeDef](./type_defs.md#createopenzfsoriginsnapshotconfigurationtypedef)
- [OpenZFSUserOrGroupQuotaTypeDef](./type_defs.md#openzfsuserorgroupquotatypedef)
- [DataRepositoryFailureDetailsTypeDef](./type_defs.md#datarepositoryfailuredetailstypedef)
- [DataRepositoryTaskFailureDetailsTypeDef](./type_defs.md#datarepositorytaskfailuredetailstypedef)
- [DataRepositoryTaskFilterTypeDef](./type_defs.md#datarepositorytaskfiltertypedef)
- [DataRepositoryTaskStatusTypeDef](./type_defs.md#datarepositorytaskstatustypedef)
- [DeleteBackupRequestRequestTypeDef](./type_defs.md#deletebackuprequestrequesttypedef)
- [DeleteDataRepositoryAssociationRequestRequestTypeDef](./type_defs.md#deletedatarepositoryassociationrequestrequesttypedef)
- [DeleteFileCacheRequestRequestTypeDef](./type_defs.md#deletefilecacherequestrequesttypedef)
- [DeleteSnapshotRequestRequestTypeDef](./type_defs.md#deletesnapshotrequestrequesttypedef)
- [DeleteStorageVirtualMachineRequestRequestTypeDef](./type_defs.md#deletestoragevirtualmachinerequestrequesttypedef)
- [DeleteVolumeOpenZFSConfigurationTypeDef](./type_defs.md#deletevolumeopenzfsconfigurationtypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeFileCachesRequestRequestTypeDef](./type_defs.md#describefilecachesrequestrequesttypedef)
- [DescribeFileSystemAliasesRequestRequestTypeDef](./type_defs.md#describefilesystemaliasesrequestrequesttypedef)
- [DescribeFileSystemsRequestRequestTypeDef](./type_defs.md#describefilesystemsrequestrequesttypedef)
- [SnapshotFilterTypeDef](./type_defs.md#snapshotfiltertypedef)
- [StorageVirtualMachineFilterTypeDef](./type_defs.md#storagevirtualmachinefiltertypedef)
- [VolumeFilterTypeDef](./type_defs.md#volumefiltertypedef)
- [DisassociateFileSystemAliasesRequestRequestTypeDef](./type_defs.md#disassociatefilesystemaliasesrequestrequesttypedef)
- [DurationSinceLastAccessTypeDef](./type_defs.md#durationsincelastaccesstypedef)
- [FileCacheFailureDetailsTypeDef](./type_defs.md#filecachefailuredetailstypedef)
- [FileCacheNFSConfigurationTypeDef](./type_defs.md#filecachenfsconfigurationtypedef)
- [LustreLogConfigurationTypeDef](./type_defs.md#lustrelogconfigurationtypedef)
- [FileSystemEndpointTypeDef](./type_defs.md#filesystemendpointtypedef)
- [FileSystemFailureDetailsTypeDef](./type_defs.md#filesystemfailuredetailstypedef)
- [FileSystemLustreMetadataConfigurationTypeDef](./type_defs.md#filesystemlustremetadataconfigurationtypedef)
- [LifecycleTransitionReasonTypeDef](./type_defs.md#lifecycletransitionreasontypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [LustreRootSquashConfigurationOutputTypeDef](./type_defs.md#lustrerootsquashconfigurationoutputtypedef)
- [LustreRootSquashConfigurationTypeDef](./type_defs.md#lustrerootsquashconfigurationtypedef)
- [OpenZFSClientConfigurationOutputTypeDef](./type_defs.md#openzfsclientconfigurationoutputtypedef)
- [OpenZFSClientConfigurationTypeDef](./type_defs.md#openzfsclientconfigurationtypedef)
- [OpenZFSOriginSnapshotConfigurationTypeDef](./type_defs.md#openzfsoriginsnapshotconfigurationtypedef)
- [ReleaseFileSystemNfsV3LocksRequestRequestTypeDef](./type_defs.md#releasefilesystemnfsv3locksrequestrequesttypedef)
- [RestoreVolumeFromSnapshotRequestRequestTypeDef](./type_defs.md#restorevolumefromsnapshotrequestrequesttypedef)
- [RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef)
- [SelfManagedActiveDirectoryAttributesTypeDef](./type_defs.md#selfmanagedactivedirectoryattributestypedef)
- [SelfManagedActiveDirectoryConfigurationUpdatesTypeDef](./type_defs.md#selfmanagedactivedirectoryconfigurationupdatestypedef)
- [StartMisconfiguredStateRecoveryRequestRequestTypeDef](./type_defs.md#startmisconfiguredstaterecoveryrequestrequesttypedef)
- [SvmEndpointTypeDef](./type_defs.md#svmendpointtypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateFileCacheLustreConfigurationTypeDef](./type_defs.md#updatefilecachelustreconfigurationtypedef)
- [UpdateFileSystemLustreMetadataConfigurationTypeDef](./type_defs.md#updatefilesystemlustremetadataconfigurationtypedef)
- [UpdateSharedVpcConfigurationRequestRequestTypeDef](./type_defs.md#updatesharedvpcconfigurationrequestrequesttypedef)
- [UpdateSnapshotRequestRequestTypeDef](./type_defs.md#updatesnapshotrequestrequesttypedef)
- [WindowsAuditLogConfigurationTypeDef](./type_defs.md#windowsauditlogconfigurationtypedef)
- [AssociateFileSystemAliasesResponseTypeDef](./type_defs.md#associatefilesystemaliasesresponsetypedef)
- [CancelDataRepositoryTaskResponseTypeDef](./type_defs.md#canceldatarepositorytaskresponsetypedef)
- [DeleteBackupResponseTypeDef](./type_defs.md#deletebackupresponsetypedef)
- [DeleteDataRepositoryAssociationResponseTypeDef](./type_defs.md#deletedatarepositoryassociationresponsetypedef)
- [DeleteFileCacheResponseTypeDef](./type_defs.md#deletefilecacheresponsetypedef)
- [DeleteSnapshotResponseTypeDef](./type_defs.md#deletesnapshotresponsetypedef)
- [DeleteStorageVirtualMachineResponseTypeDef](./type_defs.md#deletestoragevirtualmachineresponsetypedef)
- [DescribeFileSystemAliasesResponseTypeDef](./type_defs.md#describefilesystemaliasesresponsetypedef)
- [DescribeSharedVpcConfigurationResponseTypeDef](./type_defs.md#describesharedvpcconfigurationresponsetypedef)
- [DisassociateFileSystemAliasesResponseTypeDef](./type_defs.md#disassociatefilesystemaliasesresponsetypedef)
- [UpdateSharedVpcConfigurationResponseTypeDef](./type_defs.md#updatesharedvpcconfigurationresponsetypedef)
- [NFSDataRepositoryConfigurationTypeDef](./type_defs.md#nfsdatarepositoryconfigurationtypedef)
- [AutoExportPolicyUnionTypeDef](./type_defs.md#autoexportpolicyuniontypedef)
- [S3DataRepositoryConfigurationOutputTypeDef](./type_defs.md#s3datarepositoryconfigurationoutputtypedef)
- [AutoImportPolicyUnionTypeDef](./type_defs.md#autoimportpolicyuniontypedef)
- [CopyBackupRequestRequestTypeDef](./type_defs.md#copybackuprequestrequesttypedef)
- [CreateBackupRequestRequestTypeDef](./type_defs.md#createbackuprequestrequesttypedef)
- [CreateSnapshotRequestRequestTypeDef](./type_defs.md#createsnapshotrequestrequesttypedef)
- [DeleteFileSystemLustreConfigurationTypeDef](./type_defs.md#deletefilesystemlustreconfigurationtypedef)
- [DeleteFileSystemLustreResponseTypeDef](./type_defs.md#deletefilesystemlustreresponsetypedef)
- [DeleteFileSystemOpenZFSConfigurationTypeDef](./type_defs.md#deletefilesystemopenzfsconfigurationtypedef)
- [DeleteFileSystemOpenZFSResponseTypeDef](./type_defs.md#deletefilesystemopenzfsresponsetypedef)
- [DeleteFileSystemWindowsConfigurationTypeDef](./type_defs.md#deletefilesystemwindowsconfigurationtypedef)
- [DeleteFileSystemWindowsResponseTypeDef](./type_defs.md#deletefilesystemwindowsresponsetypedef)
- [DeleteVolumeOntapConfigurationTypeDef](./type_defs.md#deletevolumeontapconfigurationtypedef)
- [DeleteVolumeOntapResponseTypeDef](./type_defs.md#deletevolumeontapresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateFileCacheLustreConfigurationTypeDef](./type_defs.md#createfilecachelustreconfigurationtypedef)
- [CreateFileSystemOntapConfigurationTypeDef](./type_defs.md#createfilesystemontapconfigurationtypedef)
- [UpdateFileSystemOntapConfigurationTypeDef](./type_defs.md#updatefilesystemontapconfigurationtypedef)
- [OpenZFSFileSystemConfigurationTypeDef](./type_defs.md#openzfsfilesystemconfigurationtypedef)
- [UpdateFileSystemOpenZFSConfigurationTypeDef](./type_defs.md#updatefilesystemopenzfsconfigurationtypedef)
- [CreateSvmActiveDirectoryConfigurationTypeDef](./type_defs.md#createsvmactivedirectoryconfigurationtypedef)
- [CreateFileSystemWindowsConfigurationTypeDef](./type_defs.md#createfilesystemwindowsconfigurationtypedef)
- [DataRepositoryConfigurationTypeDef](./type_defs.md#datarepositoryconfigurationtypedef)
- [DescribeDataRepositoryTasksRequestRequestTypeDef](./type_defs.md#describedatarepositorytasksrequestrequesttypedef)
- [DescribeBackupsRequestRequestTypeDef](./type_defs.md#describebackupsrequestrequesttypedef)
- [DescribeDataRepositoryAssociationsRequestRequestTypeDef](./type_defs.md#describedatarepositoryassociationsrequestrequesttypedef)
- [DescribeBackupsRequestPaginateTypeDef](./type_defs.md#describebackupsrequestpaginatetypedef)
- [DescribeFileSystemsRequestPaginateTypeDef](./type_defs.md#describefilesystemsrequestpaginatetypedef)
- [ListTagsForResourceRequestPaginateTypeDef](./type_defs.md#listtagsforresourcerequestpaginatetypedef)
- [DescribeSnapshotsRequestRequestTypeDef](./type_defs.md#describesnapshotsrequestrequesttypedef)
- [DescribeStorageVirtualMachinesRequestPaginateTypeDef](./type_defs.md#describestoragevirtualmachinesrequestpaginatetypedef)
- [DescribeStorageVirtualMachinesRequestRequestTypeDef](./type_defs.md#describestoragevirtualmachinesrequestrequesttypedef)
- [DescribeVolumesRequestPaginateTypeDef](./type_defs.md#describevolumesrequestpaginatetypedef)
- [DescribeVolumesRequestRequestTypeDef](./type_defs.md#describevolumesrequestrequesttypedef)
- [ReleaseConfigurationTypeDef](./type_defs.md#releaseconfigurationtypedef)
- [FileCacheDataRepositoryAssociationTypeDef](./type_defs.md#filecachedatarepositoryassociationtypedef)
- [FileCacheLustreConfigurationTypeDef](./type_defs.md#filecachelustreconfigurationtypedef)
- [FileSystemEndpointsTypeDef](./type_defs.md#filesystemendpointstypedef)
- [SnapshotPaginatorTypeDef](./type_defs.md#snapshotpaginatortypedef)
- [SnapshotTypeDef](./type_defs.md#snapshottypedef)
- [LustreRootSquashConfigurationUnionTypeDef](./type_defs.md#lustrerootsquashconfigurationuniontypedef)
- [OpenZFSNfsExportOutputTypeDef](./type_defs.md#openzfsnfsexportoutputtypedef)
- [OpenZFSClientConfigurationUnionTypeDef](./type_defs.md#openzfsclientconfigurationuniontypedef)
- [SnaplockRetentionPeriodTypeDef](./type_defs.md#snaplockretentionperiodtypedef)
- [SvmActiveDirectoryConfigurationTypeDef](./type_defs.md#svmactivedirectoryconfigurationtypedef)
- [UpdateFileSystemWindowsConfigurationTypeDef](./type_defs.md#updatefilesystemwindowsconfigurationtypedef)
- [UpdateSvmActiveDirectoryConfigurationTypeDef](./type_defs.md#updatesvmactivedirectoryconfigurationtypedef)
- [SvmEndpointsTypeDef](./type_defs.md#svmendpointstypedef)
- [UpdateFileCacheRequestRequestTypeDef](./type_defs.md#updatefilecacherequestrequesttypedef)
- [WindowsFileSystemConfigurationTypeDef](./type_defs.md#windowsfilesystemconfigurationtypedef)
- [DataRepositoryAssociationTypeDef](./type_defs.md#datarepositoryassociationtypedef)
- [S3DataRepositoryConfigurationTypeDef](./type_defs.md#s3datarepositoryconfigurationtypedef)
- [DeleteFileSystemRequestRequestTypeDef](./type_defs.md#deletefilesystemrequestrequesttypedef)
- [DeleteFileSystemResponseTypeDef](./type_defs.md#deletefilesystemresponsetypedef)
- [DeleteVolumeRequestRequestTypeDef](./type_defs.md#deletevolumerequestrequesttypedef)
- [DeleteVolumeResponseTypeDef](./type_defs.md#deletevolumeresponsetypedef)
- [CreateStorageVirtualMachineRequestRequestTypeDef](./type_defs.md#createstoragevirtualmachinerequestrequesttypedef)
- [LustreFileSystemConfigurationTypeDef](./type_defs.md#lustrefilesystemconfigurationtypedef)
- [CreateDataRepositoryTaskRequestRequestTypeDef](./type_defs.md#createdatarepositorytaskrequestrequesttypedef)
- [DataRepositoryTaskTypeDef](./type_defs.md#datarepositorytasktypedef)
- [CreateFileCacheRequestRequestTypeDef](./type_defs.md#createfilecacherequestrequesttypedef)
- [FileCacheCreatingTypeDef](./type_defs.md#filecachecreatingtypedef)
- [FileCacheTypeDef](./type_defs.md#filecachetypedef)
- [OntapFileSystemConfigurationTypeDef](./type_defs.md#ontapfilesystemconfigurationtypedef)
- [CreateSnapshotResponseTypeDef](./type_defs.md#createsnapshotresponsetypedef)
- [DescribeSnapshotsResponseTypeDef](./type_defs.md#describesnapshotsresponsetypedef)
- [UpdateSnapshotResponseTypeDef](./type_defs.md#updatesnapshotresponsetypedef)
- [CreateFileSystemLustreConfigurationTypeDef](./type_defs.md#createfilesystemlustreconfigurationtypedef)
- [UpdateFileSystemLustreConfigurationTypeDef](./type_defs.md#updatefilesystemlustreconfigurationtypedef)
- [OpenZFSVolumeConfigurationTypeDef](./type_defs.md#openzfsvolumeconfigurationtypedef)
- [OpenZFSNfsExportTypeDef](./type_defs.md#openzfsnfsexporttypedef)
- [CreateSnaplockConfigurationTypeDef](./type_defs.md#createsnaplockconfigurationtypedef)
- [SnaplockConfigurationTypeDef](./type_defs.md#snaplockconfigurationtypedef)
- [UpdateSnaplockConfigurationTypeDef](./type_defs.md#updatesnaplockconfigurationtypedef)
- [UpdateStorageVirtualMachineRequestRequestTypeDef](./type_defs.md#updatestoragevirtualmachinerequestrequesttypedef)
- [StorageVirtualMachineTypeDef](./type_defs.md#storagevirtualmachinetypedef)
- [CreateDataRepositoryAssociationResponseTypeDef](./type_defs.md#createdatarepositoryassociationresponsetypedef)
- [DescribeDataRepositoryAssociationsResponseTypeDef](./type_defs.md#describedatarepositoryassociationsresponsetypedef)
- [UpdateDataRepositoryAssociationResponseTypeDef](./type_defs.md#updatedatarepositoryassociationresponsetypedef)
- [CreateDataRepositoryAssociationRequestRequestTypeDef](./type_defs.md#createdatarepositoryassociationrequestrequesttypedef)
- [UpdateDataRepositoryAssociationRequestRequestTypeDef](./type_defs.md#updatedatarepositoryassociationrequestrequesttypedef)
- [CreateDataRepositoryTaskResponseTypeDef](./type_defs.md#createdatarepositorytaskresponsetypedef)
- [DescribeDataRepositoryTasksResponseTypeDef](./type_defs.md#describedatarepositorytasksresponsetypedef)
- [CreateFileCacheResponseTypeDef](./type_defs.md#createfilecacheresponsetypedef)
- [DescribeFileCachesResponseTypeDef](./type_defs.md#describefilecachesresponsetypedef)
- [UpdateFileCacheResponseTypeDef](./type_defs.md#updatefilecacheresponsetypedef)
- [UpdateFileSystemRequestRequestTypeDef](./type_defs.md#updatefilesystemrequestrequesttypedef)
- [OpenZFSNfsExportUnionTypeDef](./type_defs.md#openzfsnfsexportuniontypedef)
- [CreateOntapVolumeConfigurationTypeDef](./type_defs.md#createontapvolumeconfigurationtypedef)
- [OntapVolumeConfigurationTypeDef](./type_defs.md#ontapvolumeconfigurationtypedef)
- [UpdateOntapVolumeConfigurationTypeDef](./type_defs.md#updateontapvolumeconfigurationtypedef)
- [CreateStorageVirtualMachineResponseTypeDef](./type_defs.md#createstoragevirtualmachineresponsetypedef)
- [DescribeStorageVirtualMachinesResponseTypeDef](./type_defs.md#describestoragevirtualmachinesresponsetypedef)
- [UpdateStorageVirtualMachineResponseTypeDef](./type_defs.md#updatestoragevirtualmachineresponsetypedef)
- [CreateOpenZFSVolumeConfigurationTypeDef](./type_defs.md#createopenzfsvolumeconfigurationtypedef)
- [OpenZFSCreateRootVolumeConfigurationTypeDef](./type_defs.md#openzfscreaterootvolumeconfigurationtypedef)
- [UpdateOpenZFSVolumeConfigurationTypeDef](./type_defs.md#updateopenzfsvolumeconfigurationtypedef)
- [CreateVolumeFromBackupRequestRequestTypeDef](./type_defs.md#createvolumefrombackuprequestrequesttypedef)
- [VolumePaginatorTypeDef](./type_defs.md#volumepaginatortypedef)
- [VolumeTypeDef](./type_defs.md#volumetypedef)
- [CreateVolumeRequestRequestTypeDef](./type_defs.md#createvolumerequestrequesttypedef)
- [CreateFileSystemOpenZFSConfigurationTypeDef](./type_defs.md#createfilesystemopenzfsconfigurationtypedef)
- [UpdateVolumeRequestRequestTypeDef](./type_defs.md#updatevolumerequestrequesttypedef)
- [AdministrativeActionPaginatorTypeDef](./type_defs.md#administrativeactionpaginatortypedef)
- [DescribeVolumesResponsePaginatorTypeDef](./type_defs.md#describevolumesresponsepaginatortypedef)
- [AdministrativeActionTypeDef](./type_defs.md#administrativeactiontypedef)
- [CreateVolumeFromBackupResponseTypeDef](./type_defs.md#createvolumefrombackupresponsetypedef)
- [CreateVolumeResponseTypeDef](./type_defs.md#createvolumeresponsetypedef)
- [DescribeVolumesResponseTypeDef](./type_defs.md#describevolumesresponsetypedef)
- [UpdateVolumeResponseTypeDef](./type_defs.md#updatevolumeresponsetypedef)
- [CreateFileSystemFromBackupRequestRequestTypeDef](./type_defs.md#createfilesystemfrombackuprequestrequesttypedef)
- [CreateFileSystemRequestRequestTypeDef](./type_defs.md#createfilesystemrequestrequesttypedef)
- [FileSystemPaginatorTypeDef](./type_defs.md#filesystempaginatortypedef)
- [CopySnapshotAndUpdateVolumeResponseTypeDef](./type_defs.md#copysnapshotandupdatevolumeresponsetypedef)
- [FileSystemTypeDef](./type_defs.md#filesystemtypedef)
- [RestoreVolumeFromSnapshotResponseTypeDef](./type_defs.md#restorevolumefromsnapshotresponsetypedef)
- [BackupPaginatorTypeDef](./type_defs.md#backuppaginatortypedef)
- [DescribeFileSystemsResponsePaginatorTypeDef](./type_defs.md#describefilesystemsresponsepaginatortypedef)
- [BackupTypeDef](./type_defs.md#backuptypedef)
- [CreateFileSystemFromBackupResponseTypeDef](./type_defs.md#createfilesystemfrombackupresponsetypedef)
- [CreateFileSystemResponseTypeDef](./type_defs.md#createfilesystemresponsetypedef)
- [DescribeFileSystemsResponseTypeDef](./type_defs.md#describefilesystemsresponsetypedef)
- [ReleaseFileSystemNfsV3LocksResponseTypeDef](./type_defs.md#releasefilesystemnfsv3locksresponsetypedef)
- [StartMisconfiguredStateRecoveryResponseTypeDef](./type_defs.md#startmisconfiguredstaterecoveryresponsetypedef)
- [UpdateFileSystemResponseTypeDef](./type_defs.md#updatefilesystemresponsetypedef)
- [DescribeBackupsResponsePaginatorTypeDef](./type_defs.md#describebackupsresponsepaginatortypedef)
- [CopyBackupResponseTypeDef](./type_defs.md#copybackupresponsetypedef)
- [CreateBackupResponseTypeDef](./type_defs.md#createbackupresponsetypedef)
- [DescribeBackupsResponseTypeDef](./type_defs.md#describebackupsresponsetypedef)

