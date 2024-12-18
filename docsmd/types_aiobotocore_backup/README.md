# Backup module

> [Index](../README.md) > Backup


!!! note ""

    Auto-generated documentation for [Backup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#backup)
    type annotations stubs module [types-aiobotocore-backup](https://pypi.org/project/types-aiobotocore-backup/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Backup` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Backup` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[backup]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[backup]'

# standalone installation
python -m pip install types-aiobotocore-backup
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-backup
```

## Usage

Code samples can be found in [Examples](./usage.md).

## BackupClient

Type annotations and code completion for  `#!python session.create_client("backup")` as [BackupClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client)

```python
# BackupClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_backup.client import BackupClient


session = get_session()
async with session.create_client("backup") as client:
    client: BackupClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("backup").get_paginator("...")`.

```python
# ListBackupJobsPaginator usage example

from types_aiobotocore_backup.paginator import ListBackupJobsPaginator

def get_list_backup_jobs_paginator() -> ListBackupJobsPaginator:
    return client.get_paginator("list_backup_jobs"))
```

- [ListBackupJobsPaginator](./paginators.md#listbackupjobspaginator)
- [ListBackupPlanTemplatesPaginator](./paginators.md#listbackupplantemplatespaginator)
- [ListBackupPlanVersionsPaginator](./paginators.md#listbackupplanversionspaginator)
- [ListBackupPlansPaginator](./paginators.md#listbackupplanspaginator)
- [ListBackupSelectionsPaginator](./paginators.md#listbackupselectionspaginator)
- [ListBackupVaultsPaginator](./paginators.md#listbackupvaultspaginator)
- [ListCopyJobsPaginator](./paginators.md#listcopyjobspaginator)
- [ListIndexedRecoveryPointsPaginator](./paginators.md#listindexedrecoverypointspaginator)
- [ListLegalHoldsPaginator](./paginators.md#listlegalholdspaginator)
- [ListProtectedResourcesByBackupVaultPaginator](./paginators.md#listprotectedresourcesbybackupvaultpaginator)
- [ListProtectedResourcesPaginator](./paginators.md#listprotectedresourcespaginator)
- [ListRecoveryPointsByBackupVaultPaginator](./paginators.md#listrecoverypointsbybackupvaultpaginator)
- [ListRecoveryPointsByLegalHoldPaginator](./paginators.md#listrecoverypointsbylegalholdpaginator)
- [ListRecoveryPointsByResourcePaginator](./paginators.md#listrecoverypointsbyresourcepaginator)
- [ListRestoreJobsByProtectedResourcePaginator](./paginators.md#listrestorejobsbyprotectedresourcepaginator)
- [ListRestoreJobsPaginator](./paginators.md#listrestorejobspaginator)
- [ListRestoreTestingPlansPaginator](./paginators.md#listrestoretestingplanspaginator)
- [ListRestoreTestingSelectionsPaginator](./paginators.md#listrestoretestingselectionspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AggregationPeriodType usage example

from types_aiobotocore_backup.literals import AggregationPeriodType

def get_value() -> AggregationPeriodType:
    return "FOURTEEN_DAYS"
```

- [AggregationPeriodType](./literals.md#aggregationperiodtype)
- [BackupJobStateType](./literals.md#backupjobstatetype)
- [BackupJobStatusType](./literals.md#backupjobstatustype)
- [BackupVaultEventType](./literals.md#backupvaulteventtype)
- [ConditionTypeType](./literals.md#conditiontypetype)
- [CopyJobStateType](./literals.md#copyjobstatetype)
- [CopyJobStatusType](./literals.md#copyjobstatustype)
- [IndexStatusType](./literals.md#indexstatustype)
- [IndexType](./literals.md#indextype)
- [LegalHoldStatusType](./literals.md#legalholdstatustype)
- [ListBackupJobsPaginatorName](./literals.md#listbackupjobspaginatorname)
- [ListBackupPlanTemplatesPaginatorName](./literals.md#listbackupplantemplatespaginatorname)
- [ListBackupPlanVersionsPaginatorName](./literals.md#listbackupplanversionspaginatorname)
- [ListBackupPlansPaginatorName](./literals.md#listbackupplanspaginatorname)
- [ListBackupSelectionsPaginatorName](./literals.md#listbackupselectionspaginatorname)
- [ListBackupVaultsPaginatorName](./literals.md#listbackupvaultspaginatorname)
- [ListCopyJobsPaginatorName](./literals.md#listcopyjobspaginatorname)
- [ListIndexedRecoveryPointsPaginatorName](./literals.md#listindexedrecoverypointspaginatorname)
- [ListLegalHoldsPaginatorName](./literals.md#listlegalholdspaginatorname)
- [ListProtectedResourcesByBackupVaultPaginatorName](./literals.md#listprotectedresourcesbybackupvaultpaginatorname)
- [ListProtectedResourcesPaginatorName](./literals.md#listprotectedresourcespaginatorname)
- [ListRecoveryPointsByBackupVaultPaginatorName](./literals.md#listrecoverypointsbybackupvaultpaginatorname)
- [ListRecoveryPointsByLegalHoldPaginatorName](./literals.md#listrecoverypointsbylegalholdpaginatorname)
- [ListRecoveryPointsByResourcePaginatorName](./literals.md#listrecoverypointsbyresourcepaginatorname)
- [ListRestoreJobsByProtectedResourcePaginatorName](./literals.md#listrestorejobsbyprotectedresourcepaginatorname)
- [ListRestoreJobsPaginatorName](./literals.md#listrestorejobspaginatorname)
- [ListRestoreTestingPlansPaginatorName](./literals.md#listrestoretestingplanspaginatorname)
- [ListRestoreTestingSelectionsPaginatorName](./literals.md#listrestoretestingselectionspaginatorname)
- [RecoveryPointStatusType](./literals.md#recoverypointstatustype)
- [RestoreDeletionStatusType](./literals.md#restoredeletionstatustype)
- [RestoreJobStateType](./literals.md#restorejobstatetype)
- [RestoreJobStatusType](./literals.md#restorejobstatustype)
- [RestoreTestingRecoveryPointSelectionAlgorithmType](./literals.md#restoretestingrecoverypointselectionalgorithmtype)
- [RestoreTestingRecoveryPointTypeType](./literals.md#restoretestingrecoverypointtypetype)
- [RestoreValidationStatusType](./literals.md#restorevalidationstatustype)
- [StorageClassType](./literals.md#storageclasstype)
- [VaultStateType](./literals.md#vaultstatetype)
- [VaultTypeType](./literals.md#vaulttypetype)
- [BackupServiceName](./literals.md#backupservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AdvancedBackupSettingOutputTypeDef](./type_defs.md#advancedbackupsettingoutputtypedef)
- [AdvancedBackupSettingTypeDef](./type_defs.md#advancedbackupsettingtypedef)
- [BackupJobSummaryTypeDef](./type_defs.md#backupjobsummarytypedef)
- [RecoveryPointCreatorTypeDef](./type_defs.md#recoverypointcreatortypedef)
- [BackupPlanTemplatesListMemberTypeDef](./type_defs.md#backupplantemplateslistmembertypedef)
- [LifecycleTypeDef](./type_defs.md#lifecycletypedef)
- [IndexActionOutputTypeDef](./type_defs.md#indexactionoutputtypedef)
- [ConditionTypeDef](./type_defs.md#conditiontypedef)
- [BackupSelectionsListMemberTypeDef](./type_defs.md#backupselectionslistmembertypedef)
- [BackupVaultListMemberTypeDef](./type_defs.md#backupvaultlistmembertypedef)
- [CalculatedLifecycleTypeDef](./type_defs.md#calculatedlifecycletypedef)
- [CancelLegalHoldInputRequestTypeDef](./type_defs.md#cancellegalholdinputrequesttypedef)
- [ConditionParameterTypeDef](./type_defs.md#conditionparametertypedef)
- [ControlInputParameterTypeDef](./type_defs.md#controlinputparametertypedef)
- [ControlScopeOutputTypeDef](./type_defs.md#controlscopeoutputtypedef)
- [ControlScopeTypeDef](./type_defs.md#controlscopetypedef)
- [CopyJobSummaryTypeDef](./type_defs.md#copyjobsummarytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateBackupVaultInputRequestTypeDef](./type_defs.md#createbackupvaultinputrequesttypedef)
- [CreateLogicallyAirGappedBackupVaultInputRequestTypeDef](./type_defs.md#createlogicallyairgappedbackupvaultinputrequesttypedef)
- [ReportDeliveryChannelTypeDef](./type_defs.md#reportdeliverychanneltypedef)
- [ReportSettingTypeDef](./type_defs.md#reportsettingtypedef)
- [DateRangeOutputTypeDef](./type_defs.md#daterangeoutputtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [DeleteBackupPlanInputRequestTypeDef](./type_defs.md#deletebackupplaninputrequesttypedef)
- [DeleteBackupSelectionInputRequestTypeDef](./type_defs.md#deletebackupselectioninputrequesttypedef)
- [DeleteBackupVaultAccessPolicyInputRequestTypeDef](./type_defs.md#deletebackupvaultaccesspolicyinputrequesttypedef)
- [DeleteBackupVaultInputRequestTypeDef](./type_defs.md#deletebackupvaultinputrequesttypedef)
- [DeleteBackupVaultLockConfigurationInputRequestTypeDef](./type_defs.md#deletebackupvaultlockconfigurationinputrequesttypedef)
- [DeleteBackupVaultNotificationsInputRequestTypeDef](./type_defs.md#deletebackupvaultnotificationsinputrequesttypedef)
- [DeleteFrameworkInputRequestTypeDef](./type_defs.md#deleteframeworkinputrequesttypedef)
- [DeleteRecoveryPointInputRequestTypeDef](./type_defs.md#deleterecoverypointinputrequesttypedef)
- [DeleteReportPlanInputRequestTypeDef](./type_defs.md#deletereportplaninputrequesttypedef)
- [DeleteRestoreTestingPlanInputRequestTypeDef](./type_defs.md#deleterestoretestingplaninputrequesttypedef)
- [DeleteRestoreTestingSelectionInputRequestTypeDef](./type_defs.md#deleterestoretestingselectioninputrequesttypedef)
- [DescribeBackupJobInputRequestTypeDef](./type_defs.md#describebackupjobinputrequesttypedef)
- [DescribeBackupVaultInputRequestTypeDef](./type_defs.md#describebackupvaultinputrequesttypedef)
- [DescribeCopyJobInputRequestTypeDef](./type_defs.md#describecopyjobinputrequesttypedef)
- [DescribeFrameworkInputRequestTypeDef](./type_defs.md#describeframeworkinputrequesttypedef)
- [DescribeProtectedResourceInputRequestTypeDef](./type_defs.md#describeprotectedresourceinputrequesttypedef)
- [DescribeRecoveryPointInputRequestTypeDef](./type_defs.md#describerecoverypointinputrequesttypedef)
- [DescribeReportJobInputRequestTypeDef](./type_defs.md#describereportjobinputrequesttypedef)
- [DescribeReportPlanInputRequestTypeDef](./type_defs.md#describereportplaninputrequesttypedef)
- [DescribeRestoreJobInputRequestTypeDef](./type_defs.md#describerestorejobinputrequesttypedef)
- [RestoreJobCreatorTypeDef](./type_defs.md#restorejobcreatortypedef)
- [DisassociateRecoveryPointFromParentInputRequestTypeDef](./type_defs.md#disassociaterecoverypointfromparentinputrequesttypedef)
- [DisassociateRecoveryPointInputRequestTypeDef](./type_defs.md#disassociaterecoverypointinputrequesttypedef)
- [ExportBackupPlanTemplateInputRequestTypeDef](./type_defs.md#exportbackupplantemplateinputrequesttypedef)
- [FrameworkTypeDef](./type_defs.md#frameworktypedef)
- [GetBackupPlanFromJSONInputRequestTypeDef](./type_defs.md#getbackupplanfromjsoninputrequesttypedef)
- [GetBackupPlanFromTemplateInputRequestTypeDef](./type_defs.md#getbackupplanfromtemplateinputrequesttypedef)
- [GetBackupPlanInputRequestTypeDef](./type_defs.md#getbackupplaninputrequesttypedef)
- [GetBackupSelectionInputRequestTypeDef](./type_defs.md#getbackupselectioninputrequesttypedef)
- [GetBackupVaultAccessPolicyInputRequestTypeDef](./type_defs.md#getbackupvaultaccesspolicyinputrequesttypedef)
- [GetBackupVaultNotificationsInputRequestTypeDef](./type_defs.md#getbackupvaultnotificationsinputrequesttypedef)
- [GetLegalHoldInputRequestTypeDef](./type_defs.md#getlegalholdinputrequesttypedef)
- [GetRecoveryPointIndexDetailsInputRequestTypeDef](./type_defs.md#getrecoverypointindexdetailsinputrequesttypedef)
- [GetRecoveryPointRestoreMetadataInputRequestTypeDef](./type_defs.md#getrecoverypointrestoremetadatainputrequesttypedef)
- [GetRestoreJobMetadataInputRequestTypeDef](./type_defs.md#getrestorejobmetadatainputrequesttypedef)
- [GetRestoreTestingInferredMetadataInputRequestTypeDef](./type_defs.md#getrestoretestinginferredmetadatainputrequesttypedef)
- [GetRestoreTestingPlanInputRequestTypeDef](./type_defs.md#getrestoretestingplaninputrequesttypedef)
- [GetRestoreTestingSelectionInputRequestTypeDef](./type_defs.md#getrestoretestingselectioninputrequesttypedef)
- [IndexActionTypeDef](./type_defs.md#indexactiontypedef)
- [IndexedRecoveryPointTypeDef](./type_defs.md#indexedrecoverypointtypedef)
- [KeyValueTypeDef](./type_defs.md#keyvaluetypedef)
- [LegalHoldTypeDef](./type_defs.md#legalholdtypedef)
- [ListBackupJobSummariesInputRequestTypeDef](./type_defs.md#listbackupjobsummariesinputrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListBackupPlanTemplatesInputRequestTypeDef](./type_defs.md#listbackupplantemplatesinputrequesttypedef)
- [ListBackupPlanVersionsInputRequestTypeDef](./type_defs.md#listbackupplanversionsinputrequesttypedef)
- [ListBackupPlansInputRequestTypeDef](./type_defs.md#listbackupplansinputrequesttypedef)
- [ListBackupSelectionsInputRequestTypeDef](./type_defs.md#listbackupselectionsinputrequesttypedef)
- [ListBackupVaultsInputRequestTypeDef](./type_defs.md#listbackupvaultsinputrequesttypedef)
- [ListCopyJobSummariesInputRequestTypeDef](./type_defs.md#listcopyjobsummariesinputrequesttypedef)
- [ListFrameworksInputRequestTypeDef](./type_defs.md#listframeworksinputrequesttypedef)
- [ListLegalHoldsInputRequestTypeDef](./type_defs.md#listlegalholdsinputrequesttypedef)
- [ListProtectedResourcesByBackupVaultInputRequestTypeDef](./type_defs.md#listprotectedresourcesbybackupvaultinputrequesttypedef)
- [ProtectedResourceTypeDef](./type_defs.md#protectedresourcetypedef)
- [ListProtectedResourcesInputRequestTypeDef](./type_defs.md#listprotectedresourcesinputrequesttypedef)
- [ListRecoveryPointsByLegalHoldInputRequestTypeDef](./type_defs.md#listrecoverypointsbylegalholdinputrequesttypedef)
- [RecoveryPointMemberTypeDef](./type_defs.md#recoverypointmembertypedef)
- [ListRecoveryPointsByResourceInputRequestTypeDef](./type_defs.md#listrecoverypointsbyresourceinputrequesttypedef)
- [RecoveryPointByResourceTypeDef](./type_defs.md#recoverypointbyresourcetypedef)
- [ListReportPlansInputRequestTypeDef](./type_defs.md#listreportplansinputrequesttypedef)
- [ListRestoreJobSummariesInputRequestTypeDef](./type_defs.md#listrestorejobsummariesinputrequesttypedef)
- [RestoreJobSummaryTypeDef](./type_defs.md#restorejobsummarytypedef)
- [ListRestoreTestingPlansInputRequestTypeDef](./type_defs.md#listrestoretestingplansinputrequesttypedef)
- [RestoreTestingPlanForListTypeDef](./type_defs.md#restoretestingplanforlisttypedef)
- [ListRestoreTestingSelectionsInputRequestTypeDef](./type_defs.md#listrestoretestingselectionsinputrequesttypedef)
- [RestoreTestingSelectionForListTypeDef](./type_defs.md#restoretestingselectionforlisttypedef)
- [ListTagsInputRequestTypeDef](./type_defs.md#listtagsinputrequesttypedef)
- [PutBackupVaultAccessPolicyInputRequestTypeDef](./type_defs.md#putbackupvaultaccesspolicyinputrequesttypedef)
- [PutBackupVaultLockConfigurationInputRequestTypeDef](./type_defs.md#putbackupvaultlockconfigurationinputrequesttypedef)
- [PutBackupVaultNotificationsInputRequestTypeDef](./type_defs.md#putbackupvaultnotificationsinputrequesttypedef)
- [PutRestoreValidationResultInputRequestTypeDef](./type_defs.md#putrestorevalidationresultinputrequesttypedef)
- [ReportDeliveryChannelOutputTypeDef](./type_defs.md#reportdeliverychanneloutputtypedef)
- [ReportDestinationTypeDef](./type_defs.md#reportdestinationtypedef)
- [ReportSettingOutputTypeDef](./type_defs.md#reportsettingoutputtypedef)
- [RestoreTestingRecoveryPointSelectionOutputTypeDef](./type_defs.md#restoretestingrecoverypointselectionoutputtypedef)
- [RestoreTestingRecoveryPointSelectionTypeDef](./type_defs.md#restoretestingrecoverypointselectiontypedef)
- [StartReportJobInputRequestTypeDef](./type_defs.md#startreportjobinputrequesttypedef)
- [StartRestoreJobInputRequestTypeDef](./type_defs.md#startrestorejobinputrequesttypedef)
- [StopBackupJobInputRequestTypeDef](./type_defs.md#stopbackupjobinputrequesttypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [UpdateGlobalSettingsInputRequestTypeDef](./type_defs.md#updateglobalsettingsinputrequesttypedef)
- [UpdateRecoveryPointIndexSettingsInputRequestTypeDef](./type_defs.md#updaterecoverypointindexsettingsinputrequesttypedef)
- [UpdateRegionSettingsInputRequestTypeDef](./type_defs.md#updateregionsettingsinputrequesttypedef)
- [BackupPlansListMemberTypeDef](./type_defs.md#backupplanslistmembertypedef)
- [AdvancedBackupSettingUnionTypeDef](./type_defs.md#advancedbackupsettinguniontypedef)
- [BackupJobTypeDef](./type_defs.md#backupjobtypedef)
- [CopyJobTypeDef](./type_defs.md#copyjobtypedef)
- [CopyActionTypeDef](./type_defs.md#copyactiontypedef)
- [StartBackupJobInputRequestTypeDef](./type_defs.md#startbackupjobinputrequesttypedef)
- [StartCopyJobInputRequestTypeDef](./type_defs.md#startcopyjobinputrequesttypedef)
- [UpdateRecoveryPointLifecycleInputRequestTypeDef](./type_defs.md#updaterecoverypointlifecycleinputrequesttypedef)
- [RecoveryPointByBackupVaultTypeDef](./type_defs.md#recoverypointbybackupvaulttypedef)
- [ConditionsOutputTypeDef](./type_defs.md#conditionsoutputtypedef)
- [ConditionsTypeDef](./type_defs.md#conditionstypedef)
- [FrameworkControlOutputTypeDef](./type_defs.md#frameworkcontroloutputtypedef)
- [ControlScopeUnionTypeDef](./type_defs.md#controlscopeuniontypedef)
- [CreateBackupPlanOutputTypeDef](./type_defs.md#createbackupplanoutputtypedef)
- [CreateBackupSelectionOutputTypeDef](./type_defs.md#createbackupselectionoutputtypedef)
- [CreateBackupVaultOutputTypeDef](./type_defs.md#createbackupvaultoutputtypedef)
- [CreateFrameworkOutputTypeDef](./type_defs.md#createframeworkoutputtypedef)
- [CreateLogicallyAirGappedBackupVaultOutputTypeDef](./type_defs.md#createlogicallyairgappedbackupvaultoutputtypedef)
- [CreateReportPlanOutputTypeDef](./type_defs.md#createreportplanoutputtypedef)
- [CreateRestoreTestingPlanOutputTypeDef](./type_defs.md#createrestoretestingplanoutputtypedef)
- [CreateRestoreTestingSelectionOutputTypeDef](./type_defs.md#createrestoretestingselectionoutputtypedef)
- [DeleteBackupPlanOutputTypeDef](./type_defs.md#deletebackupplanoutputtypedef)
- [DescribeBackupJobOutputTypeDef](./type_defs.md#describebackupjoboutputtypedef)
- [DescribeBackupVaultOutputTypeDef](./type_defs.md#describebackupvaultoutputtypedef)
- [DescribeGlobalSettingsOutputTypeDef](./type_defs.md#describeglobalsettingsoutputtypedef)
- [DescribeProtectedResourceOutputTypeDef](./type_defs.md#describeprotectedresourceoutputtypedef)
- [DescribeRecoveryPointOutputTypeDef](./type_defs.md#describerecoverypointoutputtypedef)
- [DescribeRegionSettingsOutputTypeDef](./type_defs.md#describeregionsettingsoutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ExportBackupPlanTemplateOutputTypeDef](./type_defs.md#exportbackupplantemplateoutputtypedef)
- [GetBackupVaultAccessPolicyOutputTypeDef](./type_defs.md#getbackupvaultaccesspolicyoutputtypedef)
- [GetBackupVaultNotificationsOutputTypeDef](./type_defs.md#getbackupvaultnotificationsoutputtypedef)
- [GetRecoveryPointIndexDetailsOutputTypeDef](./type_defs.md#getrecoverypointindexdetailsoutputtypedef)
- [GetRecoveryPointRestoreMetadataOutputTypeDef](./type_defs.md#getrecoverypointrestoremetadataoutputtypedef)
- [GetRestoreJobMetadataOutputTypeDef](./type_defs.md#getrestorejobmetadataoutputtypedef)
- [GetRestoreTestingInferredMetadataOutputTypeDef](./type_defs.md#getrestoretestinginferredmetadataoutputtypedef)
- [GetSupportedResourceTypesOutputTypeDef](./type_defs.md#getsupportedresourcetypesoutputtypedef)
- [ListBackupJobSummariesOutputTypeDef](./type_defs.md#listbackupjobsummariesoutputtypedef)
- [ListBackupPlanTemplatesOutputTypeDef](./type_defs.md#listbackupplantemplatesoutputtypedef)
- [ListBackupSelectionsOutputTypeDef](./type_defs.md#listbackupselectionsoutputtypedef)
- [ListBackupVaultsOutputTypeDef](./type_defs.md#listbackupvaultsoutputtypedef)
- [ListCopyJobSummariesOutputTypeDef](./type_defs.md#listcopyjobsummariesoutputtypedef)
- [ListTagsOutputTypeDef](./type_defs.md#listtagsoutputtypedef)
- [StartBackupJobOutputTypeDef](./type_defs.md#startbackupjoboutputtypedef)
- [StartCopyJobOutputTypeDef](./type_defs.md#startcopyjoboutputtypedef)
- [StartReportJobOutputTypeDef](./type_defs.md#startreportjoboutputtypedef)
- [StartRestoreJobOutputTypeDef](./type_defs.md#startrestorejoboutputtypedef)
- [UpdateBackupPlanOutputTypeDef](./type_defs.md#updatebackupplanoutputtypedef)
- [UpdateFrameworkOutputTypeDef](./type_defs.md#updateframeworkoutputtypedef)
- [UpdateRecoveryPointIndexSettingsOutputTypeDef](./type_defs.md#updaterecoverypointindexsettingsoutputtypedef)
- [UpdateRecoveryPointLifecycleOutputTypeDef](./type_defs.md#updaterecoverypointlifecycleoutputtypedef)
- [UpdateReportPlanOutputTypeDef](./type_defs.md#updatereportplanoutputtypedef)
- [UpdateRestoreTestingPlanOutputTypeDef](./type_defs.md#updaterestoretestingplanoutputtypedef)
- [UpdateRestoreTestingSelectionOutputTypeDef](./type_defs.md#updaterestoretestingselectionoutputtypedef)
- [CreateReportPlanInputRequestTypeDef](./type_defs.md#createreportplaninputrequesttypedef)
- [UpdateReportPlanInputRequestTypeDef](./type_defs.md#updatereportplaninputrequesttypedef)
- [RecoveryPointSelectionOutputTypeDef](./type_defs.md#recoverypointselectionoutputtypedef)
- [DateRangeTypeDef](./type_defs.md#daterangetypedef)
- [ListBackupJobsInputRequestTypeDef](./type_defs.md#listbackupjobsinputrequesttypedef)
- [ListCopyJobsInputRequestTypeDef](./type_defs.md#listcopyjobsinputrequesttypedef)
- [ListIndexedRecoveryPointsInputRequestTypeDef](./type_defs.md#listindexedrecoverypointsinputrequesttypedef)
- [ListRecoveryPointsByBackupVaultInputRequestTypeDef](./type_defs.md#listrecoverypointsbybackupvaultinputrequesttypedef)
- [ListReportJobsInputRequestTypeDef](./type_defs.md#listreportjobsinputrequesttypedef)
- [ListRestoreJobsByProtectedResourceInputRequestTypeDef](./type_defs.md#listrestorejobsbyprotectedresourceinputrequesttypedef)
- [ListRestoreJobsInputRequestTypeDef](./type_defs.md#listrestorejobsinputrequesttypedef)
- [DescribeRestoreJobOutputTypeDef](./type_defs.md#describerestorejoboutputtypedef)
- [RestoreJobsListMemberTypeDef](./type_defs.md#restorejobslistmembertypedef)
- [ListFrameworksOutputTypeDef](./type_defs.md#listframeworksoutputtypedef)
- [IndexActionUnionTypeDef](./type_defs.md#indexactionuniontypedef)
- [ListIndexedRecoveryPointsOutputTypeDef](./type_defs.md#listindexedrecoverypointsoutputtypedef)
- [ProtectedResourceConditionsOutputTypeDef](./type_defs.md#protectedresourceconditionsoutputtypedef)
- [ProtectedResourceConditionsTypeDef](./type_defs.md#protectedresourceconditionstypedef)
- [ListLegalHoldsOutputTypeDef](./type_defs.md#listlegalholdsoutputtypedef)
- [ListBackupJobsInputListBackupJobsPaginateTypeDef](./type_defs.md#listbackupjobsinputlistbackupjobspaginatetypedef)
- [ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef](./type_defs.md#listbackupplantemplatesinputlistbackupplantemplatespaginatetypedef)
- [ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef](./type_defs.md#listbackupplanversionsinputlistbackupplanversionspaginatetypedef)
- [ListBackupPlansInputListBackupPlansPaginateTypeDef](./type_defs.md#listbackupplansinputlistbackupplanspaginatetypedef)
- [ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef](./type_defs.md#listbackupselectionsinputlistbackupselectionspaginatetypedef)
- [ListBackupVaultsInputListBackupVaultsPaginateTypeDef](./type_defs.md#listbackupvaultsinputlistbackupvaultspaginatetypedef)
- [ListCopyJobsInputListCopyJobsPaginateTypeDef](./type_defs.md#listcopyjobsinputlistcopyjobspaginatetypedef)
- [ListIndexedRecoveryPointsInputListIndexedRecoveryPointsPaginateTypeDef](./type_defs.md#listindexedrecoverypointsinputlistindexedrecoverypointspaginatetypedef)
- [ListLegalHoldsInputListLegalHoldsPaginateTypeDef](./type_defs.md#listlegalholdsinputlistlegalholdspaginatetypedef)
- [ListProtectedResourcesByBackupVaultInputListProtectedResourcesByBackupVaultPaginateTypeDef](./type_defs.md#listprotectedresourcesbybackupvaultinputlistprotectedresourcesbybackupvaultpaginatetypedef)
- [ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef](./type_defs.md#listprotectedresourcesinputlistprotectedresourcespaginatetypedef)
- [ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef](./type_defs.md#listrecoverypointsbybackupvaultinputlistrecoverypointsbybackupvaultpaginatetypedef)
- [ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef](./type_defs.md#listrecoverypointsbylegalholdinputlistrecoverypointsbylegalholdpaginatetypedef)
- [ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef](./type_defs.md#listrecoverypointsbyresourceinputlistrecoverypointsbyresourcepaginatetypedef)
- [ListRestoreJobsByProtectedResourceInputListRestoreJobsByProtectedResourcePaginateTypeDef](./type_defs.md#listrestorejobsbyprotectedresourceinputlistrestorejobsbyprotectedresourcepaginatetypedef)
- [ListRestoreJobsInputListRestoreJobsPaginateTypeDef](./type_defs.md#listrestorejobsinputlistrestorejobspaginatetypedef)
- [ListRestoreTestingPlansInputListRestoreTestingPlansPaginateTypeDef](./type_defs.md#listrestoretestingplansinputlistrestoretestingplanspaginatetypedef)
- [ListRestoreTestingSelectionsInputListRestoreTestingSelectionsPaginateTypeDef](./type_defs.md#listrestoretestingselectionsinputlistrestoretestingselectionspaginatetypedef)
- [ListProtectedResourcesByBackupVaultOutputTypeDef](./type_defs.md#listprotectedresourcesbybackupvaultoutputtypedef)
- [ListProtectedResourcesOutputTypeDef](./type_defs.md#listprotectedresourcesoutputtypedef)
- [ListRecoveryPointsByLegalHoldOutputTypeDef](./type_defs.md#listrecoverypointsbylegalholdoutputtypedef)
- [ListRecoveryPointsByResourceOutputTypeDef](./type_defs.md#listrecoverypointsbyresourceoutputtypedef)
- [ListRestoreJobSummariesOutputTypeDef](./type_defs.md#listrestorejobsummariesoutputtypedef)
- [ListRestoreTestingPlansOutputTypeDef](./type_defs.md#listrestoretestingplansoutputtypedef)
- [ListRestoreTestingSelectionsOutputTypeDef](./type_defs.md#listrestoretestingselectionsoutputtypedef)
- [ReportJobTypeDef](./type_defs.md#reportjobtypedef)
- [ReportPlanTypeDef](./type_defs.md#reportplantypedef)
- [RestoreTestingPlanForGetTypeDef](./type_defs.md#restoretestingplanforgettypedef)
- [RestoreTestingRecoveryPointSelectionUnionTypeDef](./type_defs.md#restoretestingrecoverypointselectionuniontypedef)
- [ListBackupPlanVersionsOutputTypeDef](./type_defs.md#listbackupplanversionsoutputtypedef)
- [ListBackupPlansOutputTypeDef](./type_defs.md#listbackupplansoutputtypedef)
- [ListBackupJobsOutputTypeDef](./type_defs.md#listbackupjobsoutputtypedef)
- [DescribeCopyJobOutputTypeDef](./type_defs.md#describecopyjoboutputtypedef)
- [ListCopyJobsOutputTypeDef](./type_defs.md#listcopyjobsoutputtypedef)
- [BackupRuleTypeDef](./type_defs.md#backupruletypedef)
- [ListRecoveryPointsByBackupVaultOutputTypeDef](./type_defs.md#listrecoverypointsbybackupvaultoutputtypedef)
- [BackupSelectionOutputTypeDef](./type_defs.md#backupselectionoutputtypedef)
- [ConditionsUnionTypeDef](./type_defs.md#conditionsuniontypedef)
- [DescribeFrameworkOutputTypeDef](./type_defs.md#describeframeworkoutputtypedef)
- [FrameworkControlTypeDef](./type_defs.md#frameworkcontroltypedef)
- [CreateLegalHoldOutputTypeDef](./type_defs.md#createlegalholdoutputtypedef)
- [GetLegalHoldOutputTypeDef](./type_defs.md#getlegalholdoutputtypedef)
- [DateRangeUnionTypeDef](./type_defs.md#daterangeuniontypedef)
- [ListRestoreJobsByProtectedResourceOutputTypeDef](./type_defs.md#listrestorejobsbyprotectedresourceoutputtypedef)
- [ListRestoreJobsOutputTypeDef](./type_defs.md#listrestorejobsoutputtypedef)
- [BackupRuleInputTypeDef](./type_defs.md#backupruleinputtypedef)
- [RestoreTestingSelectionForGetTypeDef](./type_defs.md#restoretestingselectionforgettypedef)
- [ProtectedResourceConditionsUnionTypeDef](./type_defs.md#protectedresourceconditionsuniontypedef)
- [DescribeReportJobOutputTypeDef](./type_defs.md#describereportjoboutputtypedef)
- [ListReportJobsOutputTypeDef](./type_defs.md#listreportjobsoutputtypedef)
- [DescribeReportPlanOutputTypeDef](./type_defs.md#describereportplanoutputtypedef)
- [ListReportPlansOutputTypeDef](./type_defs.md#listreportplansoutputtypedef)
- [GetRestoreTestingPlanOutputTypeDef](./type_defs.md#getrestoretestingplanoutputtypedef)
- [RestoreTestingPlanForCreateTypeDef](./type_defs.md#restoretestingplanforcreatetypedef)
- [RestoreTestingPlanForUpdateTypeDef](./type_defs.md#restoretestingplanforupdatetypedef)
- [BackupPlanTypeDef](./type_defs.md#backupplantypedef)
- [GetBackupSelectionOutputTypeDef](./type_defs.md#getbackupselectionoutputtypedef)
- [BackupSelectionTypeDef](./type_defs.md#backupselectiontypedef)
- [FrameworkControlUnionTypeDef](./type_defs.md#frameworkcontroluniontypedef)
- [UpdateFrameworkInputRequestTypeDef](./type_defs.md#updateframeworkinputrequesttypedef)
- [RecoveryPointSelectionTypeDef](./type_defs.md#recoverypointselectiontypedef)
- [BackupPlanInputTypeDef](./type_defs.md#backupplaninputtypedef)
- [GetRestoreTestingSelectionOutputTypeDef](./type_defs.md#getrestoretestingselectionoutputtypedef)
- [RestoreTestingSelectionForCreateTypeDef](./type_defs.md#restoretestingselectionforcreatetypedef)
- [RestoreTestingSelectionForUpdateTypeDef](./type_defs.md#restoretestingselectionforupdatetypedef)
- [CreateRestoreTestingPlanInputRequestTypeDef](./type_defs.md#createrestoretestingplaninputrequesttypedef)
- [UpdateRestoreTestingPlanInputRequestTypeDef](./type_defs.md#updaterestoretestingplaninputrequesttypedef)
- [GetBackupPlanFromJSONOutputTypeDef](./type_defs.md#getbackupplanfromjsonoutputtypedef)
- [GetBackupPlanFromTemplateOutputTypeDef](./type_defs.md#getbackupplanfromtemplateoutputtypedef)
- [GetBackupPlanOutputTypeDef](./type_defs.md#getbackupplanoutputtypedef)
- [CreateBackupSelectionInputRequestTypeDef](./type_defs.md#createbackupselectioninputrequesttypedef)
- [CreateFrameworkInputRequestTypeDef](./type_defs.md#createframeworkinputrequesttypedef)
- [CreateLegalHoldInputRequestTypeDef](./type_defs.md#createlegalholdinputrequesttypedef)
- [CreateBackupPlanInputRequestTypeDef](./type_defs.md#createbackupplaninputrequesttypedef)
- [UpdateBackupPlanInputRequestTypeDef](./type_defs.md#updatebackupplaninputrequesttypedef)
- [CreateRestoreTestingSelectionInputRequestTypeDef](./type_defs.md#createrestoretestingselectioninputrequesttypedef)
- [UpdateRestoreTestingSelectionInputRequestTypeDef](./type_defs.md#updaterestoretestingselectioninputrequesttypedef)

