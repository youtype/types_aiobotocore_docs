# Type definitions

> [Index](../README.md) > [Backup](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Backup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#backup)
    type annotations stubs module [types-aiobotocore-backup](https://pypi.org/project/types-aiobotocore-backup/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## AdvancedBackupSettingUnionTypeDef

```python
# AdvancedBackupSettingUnionTypeDef definition

AdvancedBackupSettingUnionTypeDef = Union[
    AdvancedBackupSettingTypeDef,  # (1)
    AdvancedBackupSettingOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AdvancedBackupSettingTypeDef](./type_defs.md#advancedbackupsettingtypedef) 
2. See [:material-code-braces: AdvancedBackupSettingOutputTypeDef](./type_defs.md#advancedbackupsettingoutputtypedef) 

## ControlScopeUnionTypeDef

```python
# ControlScopeUnionTypeDef definition

ControlScopeUnionTypeDef = Union[
    ControlScopeTypeDef,  # (1)
    ControlScopeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ControlScopeTypeDef](./type_defs.md#controlscopetypedef) 
2. See [:material-code-braces: ControlScopeOutputTypeDef](./type_defs.md#controlscopeoutputtypedef) 

## IndexActionUnionTypeDef

```python
# IndexActionUnionTypeDef definition

IndexActionUnionTypeDef = Union[
    IndexActionTypeDef,  # (1)
    IndexActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IndexActionTypeDef](./type_defs.md#indexactiontypedef) 
2. See [:material-code-braces: IndexActionOutputTypeDef](./type_defs.md#indexactionoutputtypedef) 

## RestoreTestingRecoveryPointSelectionUnionTypeDef

```python
# RestoreTestingRecoveryPointSelectionUnionTypeDef definition

RestoreTestingRecoveryPointSelectionUnionTypeDef = Union[
    RestoreTestingRecoveryPointSelectionTypeDef,  # (1)
    RestoreTestingRecoveryPointSelectionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RestoreTestingRecoveryPointSelectionTypeDef](./type_defs.md#restoretestingrecoverypointselectiontypedef) 
2. See [:material-code-braces: RestoreTestingRecoveryPointSelectionOutputTypeDef](./type_defs.md#restoretestingrecoverypointselectionoutputtypedef) 

## ConditionsUnionTypeDef

```python
# ConditionsUnionTypeDef definition

ConditionsUnionTypeDef = Union[
    ConditionsTypeDef,  # (1)
    ConditionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConditionsTypeDef](./type_defs.md#conditionstypedef) 
2. See [:material-code-braces: ConditionsOutputTypeDef](./type_defs.md#conditionsoutputtypedef) 

## DateRangeUnionTypeDef

```python
# DateRangeUnionTypeDef definition

DateRangeUnionTypeDef = Union[
    DateRangeTypeDef,  # (1)
    DateRangeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DateRangeTypeDef](./type_defs.md#daterangetypedef) 
2. See [:material-code-braces: DateRangeOutputTypeDef](./type_defs.md#daterangeoutputtypedef) 

## ProtectedResourceConditionsUnionTypeDef

```python
# ProtectedResourceConditionsUnionTypeDef definition

ProtectedResourceConditionsUnionTypeDef = Union[
    ProtectedResourceConditionsTypeDef,  # (1)
    ProtectedResourceConditionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ProtectedResourceConditionsTypeDef](./type_defs.md#protectedresourceconditionstypedef) 
2. See [:material-code-braces: ProtectedResourceConditionsOutputTypeDef](./type_defs.md#protectedresourceconditionsoutputtypedef) 

## FrameworkControlUnionTypeDef

```python
# FrameworkControlUnionTypeDef definition

FrameworkControlUnionTypeDef = Union[
    FrameworkControlTypeDef,  # (1)
    FrameworkControlOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FrameworkControlTypeDef](./type_defs.md#frameworkcontroltypedef) 
2. See [:material-code-braces: FrameworkControlOutputTypeDef](./type_defs.md#frameworkcontroloutputtypedef) 



## AdvancedBackupSettingOutputTypeDef

```python
# AdvancedBackupSettingOutputTypeDef definition

class AdvancedBackupSettingOutputTypeDef(TypedDict):
    ResourceType: NotRequired[str],
    BackupOptions: NotRequired[Dict[str, str]],
```

## AdvancedBackupSettingTypeDef

```python
# AdvancedBackupSettingTypeDef definition

class AdvancedBackupSettingTypeDef(TypedDict):
    ResourceType: NotRequired[str],
    BackupOptions: NotRequired[Mapping[str, str]],
```

## BackupJobSummaryTypeDef

```python
# BackupJobSummaryTypeDef definition

class BackupJobSummaryTypeDef(TypedDict):
    Region: NotRequired[str],
    AccountId: NotRequired[str],
    State: NotRequired[BackupJobStatusType],  # (1)
    ResourceType: NotRequired[str],
    MessageCategory: NotRequired[str],
    Count: NotRequired[int],
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
```

1. See [:material-code-brackets: BackupJobStatusType](./literals.md#backupjobstatustype) 
## RecoveryPointCreatorTypeDef

```python
# RecoveryPointCreatorTypeDef definition

class RecoveryPointCreatorTypeDef(TypedDict):
    BackupPlanId: NotRequired[str],
    BackupPlanArn: NotRequired[str],
    BackupPlanVersion: NotRequired[str],
    BackupRuleId: NotRequired[str],
```

## BackupPlanTemplatesListMemberTypeDef

```python
# BackupPlanTemplatesListMemberTypeDef definition

class BackupPlanTemplatesListMemberTypeDef(TypedDict):
    BackupPlanTemplateId: NotRequired[str],
    BackupPlanTemplateName: NotRequired[str],
```

## LifecycleTypeDef

```python
# LifecycleTypeDef definition

class LifecycleTypeDef(TypedDict):
    MoveToColdStorageAfterDays: NotRequired[int],
    DeleteAfterDays: NotRequired[int],
    OptInToArchiveForSupportedResources: NotRequired[bool],
```

## IndexActionOutputTypeDef

```python
# IndexActionOutputTypeDef definition

class IndexActionOutputTypeDef(TypedDict):
    ResourceTypes: NotRequired[List[str]],
```

## ConditionTypeDef

```python
# ConditionTypeDef definition

class ConditionTypeDef(TypedDict):
    ConditionType: ConditionTypeType,  # (1)
    ConditionKey: str,
    ConditionValue: str,
```

1. See [:material-code-brackets: ConditionTypeType](./literals.md#conditiontypetype) 
## BackupSelectionsListMemberTypeDef

```python
# BackupSelectionsListMemberTypeDef definition

class BackupSelectionsListMemberTypeDef(TypedDict):
    SelectionId: NotRequired[str],
    SelectionName: NotRequired[str],
    BackupPlanId: NotRequired[str],
    CreationDate: NotRequired[datetime],
    CreatorRequestId: NotRequired[str],
    IamRoleArn: NotRequired[str],
```

## BackupVaultListMemberTypeDef

```python
# BackupVaultListMemberTypeDef definition

class BackupVaultListMemberTypeDef(TypedDict):
    BackupVaultName: NotRequired[str],
    BackupVaultArn: NotRequired[str],
    VaultType: NotRequired[VaultTypeType],  # (1)
    VaultState: NotRequired[VaultStateType],  # (2)
    CreationDate: NotRequired[datetime],
    EncryptionKeyArn: NotRequired[str],
    CreatorRequestId: NotRequired[str],
    NumberOfRecoveryPoints: NotRequired[int],
    Locked: NotRequired[bool],
    MinRetentionDays: NotRequired[int],
    MaxRetentionDays: NotRequired[int],
    LockDate: NotRequired[datetime],
```

1. See [:material-code-brackets: VaultTypeType](./literals.md#vaulttypetype) 
2. See [:material-code-brackets: VaultStateType](./literals.md#vaultstatetype) 
## CalculatedLifecycleTypeDef

```python
# CalculatedLifecycleTypeDef definition

class CalculatedLifecycleTypeDef(TypedDict):
    MoveToColdStorageAt: NotRequired[datetime],
    DeleteAt: NotRequired[datetime],
```

## CancelLegalHoldInputRequestTypeDef

```python
# CancelLegalHoldInputRequestTypeDef definition

class CancelLegalHoldInputRequestTypeDef(TypedDict):
    LegalHoldId: str,
    CancelDescription: str,
    RetainRecordInDays: NotRequired[int],
```

## ConditionParameterTypeDef

```python
# ConditionParameterTypeDef definition

class ConditionParameterTypeDef(TypedDict):
    ConditionKey: NotRequired[str],
    ConditionValue: NotRequired[str],
```

## ControlInputParameterTypeDef

```python
# ControlInputParameterTypeDef definition

class ControlInputParameterTypeDef(TypedDict):
    ParameterName: NotRequired[str],
    ParameterValue: NotRequired[str],
```

## ControlScopeOutputTypeDef

```python
# ControlScopeOutputTypeDef definition

class ControlScopeOutputTypeDef(TypedDict):
    ComplianceResourceIds: NotRequired[List[str]],
    ComplianceResourceTypes: NotRequired[List[str]],
    Tags: NotRequired[Dict[str, str]],
```

## ControlScopeTypeDef

```python
# ControlScopeTypeDef definition

class ControlScopeTypeDef(TypedDict):
    ComplianceResourceIds: NotRequired[Sequence[str]],
    ComplianceResourceTypes: NotRequired[Sequence[str]],
    Tags: NotRequired[Mapping[str, str]],
```

## CopyJobSummaryTypeDef

```python
# CopyJobSummaryTypeDef definition

class CopyJobSummaryTypeDef(TypedDict):
    Region: NotRequired[str],
    AccountId: NotRequired[str],
    State: NotRequired[CopyJobStatusType],  # (1)
    ResourceType: NotRequired[str],
    MessageCategory: NotRequired[str],
    Count: NotRequired[int],
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
```

1. See [:material-code-brackets: CopyJobStatusType](./literals.md#copyjobstatustype) 
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

## CreateBackupVaultInputRequestTypeDef

```python
# CreateBackupVaultInputRequestTypeDef definition

class CreateBackupVaultInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
    BackupVaultTags: NotRequired[Mapping[str, str]],
    EncryptionKeyArn: NotRequired[str],
    CreatorRequestId: NotRequired[str],
```

## CreateLogicallyAirGappedBackupVaultInputRequestTypeDef

```python
# CreateLogicallyAirGappedBackupVaultInputRequestTypeDef definition

class CreateLogicallyAirGappedBackupVaultInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
    MinRetentionDays: int,
    MaxRetentionDays: int,
    BackupVaultTags: NotRequired[Mapping[str, str]],
    CreatorRequestId: NotRequired[str],
```

## ReportDeliveryChannelTypeDef

```python
# ReportDeliveryChannelTypeDef definition

class ReportDeliveryChannelTypeDef(TypedDict):
    S3BucketName: str,
    S3KeyPrefix: NotRequired[str],
    Formats: NotRequired[Sequence[str]],
```

## ReportSettingTypeDef

```python
# ReportSettingTypeDef definition

class ReportSettingTypeDef(TypedDict):
    ReportTemplate: str,
    FrameworkArns: NotRequired[Sequence[str]],
    NumberOfFrameworks: NotRequired[int],
    Accounts: NotRequired[Sequence[str]],
    OrganizationUnits: NotRequired[Sequence[str]],
    Regions: NotRequired[Sequence[str]],
```

## DateRangeOutputTypeDef

```python
# DateRangeOutputTypeDef definition

class DateRangeOutputTypeDef(TypedDict):
    FromDate: datetime,
    ToDate: datetime,
```

## DeleteBackupPlanInputRequestTypeDef

```python
# DeleteBackupPlanInputRequestTypeDef definition

class DeleteBackupPlanInputRequestTypeDef(TypedDict):
    BackupPlanId: str,
```

## DeleteBackupSelectionInputRequestTypeDef

```python
# DeleteBackupSelectionInputRequestTypeDef definition

class DeleteBackupSelectionInputRequestTypeDef(TypedDict):
    BackupPlanId: str,
    SelectionId: str,
```

## DeleteBackupVaultAccessPolicyInputRequestTypeDef

```python
# DeleteBackupVaultAccessPolicyInputRequestTypeDef definition

class DeleteBackupVaultAccessPolicyInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
```

## DeleteBackupVaultInputRequestTypeDef

```python
# DeleteBackupVaultInputRequestTypeDef definition

class DeleteBackupVaultInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
```

## DeleteBackupVaultLockConfigurationInputRequestTypeDef

```python
# DeleteBackupVaultLockConfigurationInputRequestTypeDef definition

class DeleteBackupVaultLockConfigurationInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
```

## DeleteBackupVaultNotificationsInputRequestTypeDef

```python
# DeleteBackupVaultNotificationsInputRequestTypeDef definition

class DeleteBackupVaultNotificationsInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
```

## DeleteFrameworkInputRequestTypeDef

```python
# DeleteFrameworkInputRequestTypeDef definition

class DeleteFrameworkInputRequestTypeDef(TypedDict):
    FrameworkName: str,
```

## DeleteRecoveryPointInputRequestTypeDef

```python
# DeleteRecoveryPointInputRequestTypeDef definition

class DeleteRecoveryPointInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
    RecoveryPointArn: str,
```

## DeleteReportPlanInputRequestTypeDef

```python
# DeleteReportPlanInputRequestTypeDef definition

class DeleteReportPlanInputRequestTypeDef(TypedDict):
    ReportPlanName: str,
```

## DeleteRestoreTestingPlanInputRequestTypeDef

```python
# DeleteRestoreTestingPlanInputRequestTypeDef definition

class DeleteRestoreTestingPlanInputRequestTypeDef(TypedDict):
    RestoreTestingPlanName: str,
```

## DeleteRestoreTestingSelectionInputRequestTypeDef

```python
# DeleteRestoreTestingSelectionInputRequestTypeDef definition

class DeleteRestoreTestingSelectionInputRequestTypeDef(TypedDict):
    RestoreTestingPlanName: str,
    RestoreTestingSelectionName: str,
```

## DescribeBackupJobInputRequestTypeDef

```python
# DescribeBackupJobInputRequestTypeDef definition

class DescribeBackupJobInputRequestTypeDef(TypedDict):
    BackupJobId: str,
```

## DescribeBackupVaultInputRequestTypeDef

```python
# DescribeBackupVaultInputRequestTypeDef definition

class DescribeBackupVaultInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
    BackupVaultAccountId: NotRequired[str],
```

## DescribeCopyJobInputRequestTypeDef

```python
# DescribeCopyJobInputRequestTypeDef definition

class DescribeCopyJobInputRequestTypeDef(TypedDict):
    CopyJobId: str,
```

## DescribeFrameworkInputRequestTypeDef

```python
# DescribeFrameworkInputRequestTypeDef definition

class DescribeFrameworkInputRequestTypeDef(TypedDict):
    FrameworkName: str,
```

## DescribeProtectedResourceInputRequestTypeDef

```python
# DescribeProtectedResourceInputRequestTypeDef definition

class DescribeProtectedResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## DescribeRecoveryPointInputRequestTypeDef

```python
# DescribeRecoveryPointInputRequestTypeDef definition

class DescribeRecoveryPointInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
    RecoveryPointArn: str,
    BackupVaultAccountId: NotRequired[str],
```

## DescribeReportJobInputRequestTypeDef

```python
# DescribeReportJobInputRequestTypeDef definition

class DescribeReportJobInputRequestTypeDef(TypedDict):
    ReportJobId: str,
```

## DescribeReportPlanInputRequestTypeDef

```python
# DescribeReportPlanInputRequestTypeDef definition

class DescribeReportPlanInputRequestTypeDef(TypedDict):
    ReportPlanName: str,
```

## DescribeRestoreJobInputRequestTypeDef

```python
# DescribeRestoreJobInputRequestTypeDef definition

class DescribeRestoreJobInputRequestTypeDef(TypedDict):
    RestoreJobId: str,
```

## RestoreJobCreatorTypeDef

```python
# RestoreJobCreatorTypeDef definition

class RestoreJobCreatorTypeDef(TypedDict):
    RestoreTestingPlanArn: NotRequired[str],
```

## DisassociateRecoveryPointFromParentInputRequestTypeDef

```python
# DisassociateRecoveryPointFromParentInputRequestTypeDef definition

class DisassociateRecoveryPointFromParentInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
    RecoveryPointArn: str,
```

## DisassociateRecoveryPointInputRequestTypeDef

```python
# DisassociateRecoveryPointInputRequestTypeDef definition

class DisassociateRecoveryPointInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
    RecoveryPointArn: str,
```

## ExportBackupPlanTemplateInputRequestTypeDef

```python
# ExportBackupPlanTemplateInputRequestTypeDef definition

class ExportBackupPlanTemplateInputRequestTypeDef(TypedDict):
    BackupPlanId: str,
```

## FrameworkTypeDef

```python
# FrameworkTypeDef definition

class FrameworkTypeDef(TypedDict):
    FrameworkName: NotRequired[str],
    FrameworkArn: NotRequired[str],
    FrameworkDescription: NotRequired[str],
    NumberOfControls: NotRequired[int],
    CreationTime: NotRequired[datetime],
    DeploymentStatus: NotRequired[str],
```

## GetBackupPlanFromJSONInputRequestTypeDef

```python
# GetBackupPlanFromJSONInputRequestTypeDef definition

class GetBackupPlanFromJSONInputRequestTypeDef(TypedDict):
    BackupPlanTemplateJson: str,
```

## GetBackupPlanFromTemplateInputRequestTypeDef

```python
# GetBackupPlanFromTemplateInputRequestTypeDef definition

class GetBackupPlanFromTemplateInputRequestTypeDef(TypedDict):
    BackupPlanTemplateId: str,
```

## GetBackupPlanInputRequestTypeDef

```python
# GetBackupPlanInputRequestTypeDef definition

class GetBackupPlanInputRequestTypeDef(TypedDict):
    BackupPlanId: str,
    VersionId: NotRequired[str],
```

## GetBackupSelectionInputRequestTypeDef

```python
# GetBackupSelectionInputRequestTypeDef definition

class GetBackupSelectionInputRequestTypeDef(TypedDict):
    BackupPlanId: str,
    SelectionId: str,
```

## GetBackupVaultAccessPolicyInputRequestTypeDef

```python
# GetBackupVaultAccessPolicyInputRequestTypeDef definition

class GetBackupVaultAccessPolicyInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
```

## GetBackupVaultNotificationsInputRequestTypeDef

```python
# GetBackupVaultNotificationsInputRequestTypeDef definition

class GetBackupVaultNotificationsInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
```

## GetLegalHoldInputRequestTypeDef

```python
# GetLegalHoldInputRequestTypeDef definition

class GetLegalHoldInputRequestTypeDef(TypedDict):
    LegalHoldId: str,
```

## GetRecoveryPointIndexDetailsInputRequestTypeDef

```python
# GetRecoveryPointIndexDetailsInputRequestTypeDef definition

class GetRecoveryPointIndexDetailsInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
    RecoveryPointArn: str,
```

## GetRecoveryPointRestoreMetadataInputRequestTypeDef

```python
# GetRecoveryPointRestoreMetadataInputRequestTypeDef definition

class GetRecoveryPointRestoreMetadataInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
    RecoveryPointArn: str,
    BackupVaultAccountId: NotRequired[str],
```

## GetRestoreJobMetadataInputRequestTypeDef

```python
# GetRestoreJobMetadataInputRequestTypeDef definition

class GetRestoreJobMetadataInputRequestTypeDef(TypedDict):
    RestoreJobId: str,
```

## GetRestoreTestingInferredMetadataInputRequestTypeDef

```python
# GetRestoreTestingInferredMetadataInputRequestTypeDef definition

class GetRestoreTestingInferredMetadataInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
    RecoveryPointArn: str,
    BackupVaultAccountId: NotRequired[str],
```

## GetRestoreTestingPlanInputRequestTypeDef

```python
# GetRestoreTestingPlanInputRequestTypeDef definition

class GetRestoreTestingPlanInputRequestTypeDef(TypedDict):
    RestoreTestingPlanName: str,
```

## GetRestoreTestingSelectionInputRequestTypeDef

```python
# GetRestoreTestingSelectionInputRequestTypeDef definition

class GetRestoreTestingSelectionInputRequestTypeDef(TypedDict):
    RestoreTestingPlanName: str,
    RestoreTestingSelectionName: str,
```

## IndexActionTypeDef

```python
# IndexActionTypeDef definition

class IndexActionTypeDef(TypedDict):
    ResourceTypes: NotRequired[Sequence[str]],
```

## IndexedRecoveryPointTypeDef

```python
# IndexedRecoveryPointTypeDef definition

class IndexedRecoveryPointTypeDef(TypedDict):
    RecoveryPointArn: NotRequired[str],
    SourceResourceArn: NotRequired[str],
    IamRoleArn: NotRequired[str],
    BackupCreationDate: NotRequired[datetime],
    ResourceType: NotRequired[str],
    IndexCreationDate: NotRequired[datetime],
    IndexStatus: NotRequired[IndexStatusType],  # (1)
    IndexStatusMessage: NotRequired[str],
    BackupVaultArn: NotRequired[str],
```

1. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
## KeyValueTypeDef

```python
# KeyValueTypeDef definition

class KeyValueTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## LegalHoldTypeDef

```python
# LegalHoldTypeDef definition

class LegalHoldTypeDef(TypedDict):
    Title: NotRequired[str],
    Status: NotRequired[LegalHoldStatusType],  # (1)
    Description: NotRequired[str],
    LegalHoldId: NotRequired[str],
    LegalHoldArn: NotRequired[str],
    CreationDate: NotRequired[datetime],
    CancellationDate: NotRequired[datetime],
```

1. See [:material-code-brackets: LegalHoldStatusType](./literals.md#legalholdstatustype) 
## ListBackupJobSummariesInputRequestTypeDef

```python
# ListBackupJobSummariesInputRequestTypeDef definition

class ListBackupJobSummariesInputRequestTypeDef(TypedDict):
    AccountId: NotRequired[str],
    State: NotRequired[BackupJobStatusType],  # (1)
    ResourceType: NotRequired[str],
    MessageCategory: NotRequired[str],
    AggregationPeriod: NotRequired[AggregationPeriodType],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: BackupJobStatusType](./literals.md#backupjobstatustype) 
2. See [:material-code-brackets: AggregationPeriodType](./literals.md#aggregationperiodtype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListBackupPlanTemplatesInputRequestTypeDef

```python
# ListBackupPlanTemplatesInputRequestTypeDef definition

class ListBackupPlanTemplatesInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListBackupPlanVersionsInputRequestTypeDef

```python
# ListBackupPlanVersionsInputRequestTypeDef definition

class ListBackupPlanVersionsInputRequestTypeDef(TypedDict):
    BackupPlanId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListBackupPlansInputRequestTypeDef

```python
# ListBackupPlansInputRequestTypeDef definition

class ListBackupPlansInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    IncludeDeleted: NotRequired[bool],
```

## ListBackupSelectionsInputRequestTypeDef

```python
# ListBackupSelectionsInputRequestTypeDef definition

class ListBackupSelectionsInputRequestTypeDef(TypedDict):
    BackupPlanId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListBackupVaultsInputRequestTypeDef

```python
# ListBackupVaultsInputRequestTypeDef definition

class ListBackupVaultsInputRequestTypeDef(TypedDict):
    ByVaultType: NotRequired[VaultTypeType],  # (1)
    ByShared: NotRequired[bool],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: VaultTypeType](./literals.md#vaulttypetype) 
## ListCopyJobSummariesInputRequestTypeDef

```python
# ListCopyJobSummariesInputRequestTypeDef definition

class ListCopyJobSummariesInputRequestTypeDef(TypedDict):
    AccountId: NotRequired[str],
    State: NotRequired[CopyJobStatusType],  # (1)
    ResourceType: NotRequired[str],
    MessageCategory: NotRequired[str],
    AggregationPeriod: NotRequired[AggregationPeriodType],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: CopyJobStatusType](./literals.md#copyjobstatustype) 
2. See [:material-code-brackets: AggregationPeriodType](./literals.md#aggregationperiodtype) 
## ListFrameworksInputRequestTypeDef

```python
# ListFrameworksInputRequestTypeDef definition

class ListFrameworksInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListLegalHoldsInputRequestTypeDef

```python
# ListLegalHoldsInputRequestTypeDef definition

class ListLegalHoldsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListProtectedResourcesByBackupVaultInputRequestTypeDef

```python
# ListProtectedResourcesByBackupVaultInputRequestTypeDef definition

class ListProtectedResourcesByBackupVaultInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
    BackupVaultAccountId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ProtectedResourceTypeDef

```python
# ProtectedResourceTypeDef definition

class ProtectedResourceTypeDef(TypedDict):
    ResourceArn: NotRequired[str],
    ResourceType: NotRequired[str],
    LastBackupTime: NotRequired[datetime],
    ResourceName: NotRequired[str],
    LastBackupVaultArn: NotRequired[str],
    LastRecoveryPointArn: NotRequired[str],
```

## ListProtectedResourcesInputRequestTypeDef

```python
# ListProtectedResourcesInputRequestTypeDef definition

class ListProtectedResourcesInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListRecoveryPointsByLegalHoldInputRequestTypeDef

```python
# ListRecoveryPointsByLegalHoldInputRequestTypeDef definition

class ListRecoveryPointsByLegalHoldInputRequestTypeDef(TypedDict):
    LegalHoldId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## RecoveryPointMemberTypeDef

```python
# RecoveryPointMemberTypeDef definition

class RecoveryPointMemberTypeDef(TypedDict):
    RecoveryPointArn: NotRequired[str],
    ResourceArn: NotRequired[str],
    ResourceType: NotRequired[str],
    BackupVaultName: NotRequired[str],
```

## ListRecoveryPointsByResourceInputRequestTypeDef

```python
# ListRecoveryPointsByResourceInputRequestTypeDef definition

class ListRecoveryPointsByResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ManagedByAWSBackupOnly: NotRequired[bool],
```

## RecoveryPointByResourceTypeDef

```python
# RecoveryPointByResourceTypeDef definition

class RecoveryPointByResourceTypeDef(TypedDict):
    RecoveryPointArn: NotRequired[str],
    CreationDate: NotRequired[datetime],
    Status: NotRequired[RecoveryPointStatusType],  # (1)
    StatusMessage: NotRequired[str],
    EncryptionKeyArn: NotRequired[str],
    BackupSizeBytes: NotRequired[int],
    BackupVaultName: NotRequired[str],
    IsParent: NotRequired[bool],
    ParentRecoveryPointArn: NotRequired[str],
    ResourceName: NotRequired[str],
    VaultType: NotRequired[VaultTypeType],  # (2)
    IndexStatus: NotRequired[IndexStatusType],  # (3)
    IndexStatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: RecoveryPointStatusType](./literals.md#recoverypointstatustype) 
2. See [:material-code-brackets: VaultTypeType](./literals.md#vaulttypetype) 
3. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
## ListReportPlansInputRequestTypeDef

```python
# ListReportPlansInputRequestTypeDef definition

class ListReportPlansInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListRestoreJobSummariesInputRequestTypeDef

```python
# ListRestoreJobSummariesInputRequestTypeDef definition

class ListRestoreJobSummariesInputRequestTypeDef(TypedDict):
    AccountId: NotRequired[str],
    State: NotRequired[RestoreJobStateType],  # (1)
    ResourceType: NotRequired[str],
    AggregationPeriod: NotRequired[AggregationPeriodType],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: RestoreJobStateType](./literals.md#restorejobstatetype) 
2. See [:material-code-brackets: AggregationPeriodType](./literals.md#aggregationperiodtype) 
## RestoreJobSummaryTypeDef

```python
# RestoreJobSummaryTypeDef definition

class RestoreJobSummaryTypeDef(TypedDict):
    Region: NotRequired[str],
    AccountId: NotRequired[str],
    State: NotRequired[RestoreJobStateType],  # (1)
    ResourceType: NotRequired[str],
    Count: NotRequired[int],
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
```

1. See [:material-code-brackets: RestoreJobStateType](./literals.md#restorejobstatetype) 
## ListRestoreTestingPlansInputRequestTypeDef

```python
# ListRestoreTestingPlansInputRequestTypeDef definition

class ListRestoreTestingPlansInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## RestoreTestingPlanForListTypeDef

```python
# RestoreTestingPlanForListTypeDef definition

class RestoreTestingPlanForListTypeDef(TypedDict):
    CreationTime: datetime,
    RestoreTestingPlanArn: str,
    RestoreTestingPlanName: str,
    ScheduleExpression: str,
    LastExecutionTime: NotRequired[datetime],
    LastUpdateTime: NotRequired[datetime],
    ScheduleExpressionTimezone: NotRequired[str],
    StartWindowHours: NotRequired[int],
```

## ListRestoreTestingSelectionsInputRequestTypeDef

```python
# ListRestoreTestingSelectionsInputRequestTypeDef definition

class ListRestoreTestingSelectionsInputRequestTypeDef(TypedDict):
    RestoreTestingPlanName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## RestoreTestingSelectionForListTypeDef

```python
# RestoreTestingSelectionForListTypeDef definition

class RestoreTestingSelectionForListTypeDef(TypedDict):
    CreationTime: datetime,
    IamRoleArn: str,
    ProtectedResourceType: str,
    RestoreTestingPlanName: str,
    RestoreTestingSelectionName: str,
    ValidationWindowHours: NotRequired[int],
```

## ListTagsInputRequestTypeDef

```python
# ListTagsInputRequestTypeDef definition

class ListTagsInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## PutBackupVaultAccessPolicyInputRequestTypeDef

```python
# PutBackupVaultAccessPolicyInputRequestTypeDef definition

class PutBackupVaultAccessPolicyInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
    Policy: NotRequired[str],
```

## PutBackupVaultLockConfigurationInputRequestTypeDef

```python
# PutBackupVaultLockConfigurationInputRequestTypeDef definition

class PutBackupVaultLockConfigurationInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
    MinRetentionDays: NotRequired[int],
    MaxRetentionDays: NotRequired[int],
    ChangeableForDays: NotRequired[int],
```

## PutBackupVaultNotificationsInputRequestTypeDef

```python
# PutBackupVaultNotificationsInputRequestTypeDef definition

class PutBackupVaultNotificationsInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
    SNSTopicArn: str,
    BackupVaultEvents: Sequence[BackupVaultEventType],  # (1)
```

1. See [:material-code-brackets: BackupVaultEventType](./literals.md#backupvaulteventtype) 
## PutRestoreValidationResultInputRequestTypeDef

```python
# PutRestoreValidationResultInputRequestTypeDef definition

class PutRestoreValidationResultInputRequestTypeDef(TypedDict):
    RestoreJobId: str,
    ValidationStatus: RestoreValidationStatusType,  # (1)
    ValidationStatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: RestoreValidationStatusType](./literals.md#restorevalidationstatustype) 
## ReportDeliveryChannelOutputTypeDef

```python
# ReportDeliveryChannelOutputTypeDef definition

class ReportDeliveryChannelOutputTypeDef(TypedDict):
    S3BucketName: str,
    S3KeyPrefix: NotRequired[str],
    Formats: NotRequired[List[str]],
```

## ReportDestinationTypeDef

```python
# ReportDestinationTypeDef definition

class ReportDestinationTypeDef(TypedDict):
    S3BucketName: NotRequired[str],
    S3Keys: NotRequired[List[str]],
```

## ReportSettingOutputTypeDef

```python
# ReportSettingOutputTypeDef definition

class ReportSettingOutputTypeDef(TypedDict):
    ReportTemplate: str,
    FrameworkArns: NotRequired[List[str]],
    NumberOfFrameworks: NotRequired[int],
    Accounts: NotRequired[List[str]],
    OrganizationUnits: NotRequired[List[str]],
    Regions: NotRequired[List[str]],
```

## RestoreTestingRecoveryPointSelectionOutputTypeDef

```python
# RestoreTestingRecoveryPointSelectionOutputTypeDef definition

class RestoreTestingRecoveryPointSelectionOutputTypeDef(TypedDict):
    Algorithm: NotRequired[RestoreTestingRecoveryPointSelectionAlgorithmType],  # (1)
    ExcludeVaults: NotRequired[List[str]],
    IncludeVaults: NotRequired[List[str]],
    RecoveryPointTypes: NotRequired[List[RestoreTestingRecoveryPointTypeType]],  # (2)
    SelectionWindowDays: NotRequired[int],
```

1. See [:material-code-brackets: RestoreTestingRecoveryPointSelectionAlgorithmType](./literals.md#restoretestingrecoverypointselectionalgorithmtype) 
2. See [:material-code-brackets: RestoreTestingRecoveryPointTypeType](./literals.md#restoretestingrecoverypointtypetype) 
## RestoreTestingRecoveryPointSelectionTypeDef

```python
# RestoreTestingRecoveryPointSelectionTypeDef definition

class RestoreTestingRecoveryPointSelectionTypeDef(TypedDict):
    Algorithm: NotRequired[RestoreTestingRecoveryPointSelectionAlgorithmType],  # (1)
    ExcludeVaults: NotRequired[Sequence[str]],
    IncludeVaults: NotRequired[Sequence[str]],
    RecoveryPointTypes: NotRequired[Sequence[RestoreTestingRecoveryPointTypeType]],  # (2)
    SelectionWindowDays: NotRequired[int],
```

1. See [:material-code-brackets: RestoreTestingRecoveryPointSelectionAlgorithmType](./literals.md#restoretestingrecoverypointselectionalgorithmtype) 
2. See [:material-code-brackets: RestoreTestingRecoveryPointTypeType](./literals.md#restoretestingrecoverypointtypetype) 
## StartReportJobInputRequestTypeDef

```python
# StartReportJobInputRequestTypeDef definition

class StartReportJobInputRequestTypeDef(TypedDict):
    ReportPlanName: str,
    IdempotencyToken: NotRequired[str],
```

## StartRestoreJobInputRequestTypeDef

```python
# StartRestoreJobInputRequestTypeDef definition

class StartRestoreJobInputRequestTypeDef(TypedDict):
    RecoveryPointArn: str,
    Metadata: Mapping[str, str],
    IamRoleArn: NotRequired[str],
    IdempotencyToken: NotRequired[str],
    ResourceType: NotRequired[str],
    CopySourceTagsToRestoredResource: NotRequired[bool],
```

## StopBackupJobInputRequestTypeDef

```python
# StopBackupJobInputRequestTypeDef definition

class StopBackupJobInputRequestTypeDef(TypedDict):
    BackupJobId: str,
```

## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeyList: Sequence[str],
```

## UpdateGlobalSettingsInputRequestTypeDef

```python
# UpdateGlobalSettingsInputRequestTypeDef definition

class UpdateGlobalSettingsInputRequestTypeDef(TypedDict):
    GlobalSettings: NotRequired[Mapping[str, str]],
```

## UpdateRecoveryPointIndexSettingsInputRequestTypeDef

```python
# UpdateRecoveryPointIndexSettingsInputRequestTypeDef definition

class UpdateRecoveryPointIndexSettingsInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
    RecoveryPointArn: str,
    Index: IndexType,  # (1)
    IamRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: IndexType](./literals.md#indextype) 
## UpdateRegionSettingsInputRequestTypeDef

```python
# UpdateRegionSettingsInputRequestTypeDef definition

class UpdateRegionSettingsInputRequestTypeDef(TypedDict):
    ResourceTypeOptInPreference: NotRequired[Mapping[str, bool]],
    ResourceTypeManagementPreference: NotRequired[Mapping[str, bool]],
```

## BackupPlansListMemberTypeDef

```python
# BackupPlansListMemberTypeDef definition

class BackupPlansListMemberTypeDef(TypedDict):
    BackupPlanArn: NotRequired[str],
    BackupPlanId: NotRequired[str],
    CreationDate: NotRequired[datetime],
    DeletionDate: NotRequired[datetime],
    VersionId: NotRequired[str],
    BackupPlanName: NotRequired[str],
    CreatorRequestId: NotRequired[str],
    LastExecutionDate: NotRequired[datetime],
    AdvancedBackupSettings: NotRequired[List[AdvancedBackupSettingOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: AdvancedBackupSettingOutputTypeDef](./type_defs.md#advancedbackupsettingoutputtypedef) 
## BackupJobTypeDef

```python
# BackupJobTypeDef definition

class BackupJobTypeDef(TypedDict):
    AccountId: NotRequired[str],
    BackupJobId: NotRequired[str],
    BackupVaultName: NotRequired[str],
    BackupVaultArn: NotRequired[str],
    RecoveryPointArn: NotRequired[str],
    ResourceArn: NotRequired[str],
    CreationDate: NotRequired[datetime],
    CompletionDate: NotRequired[datetime],
    State: NotRequired[BackupJobStateType],  # (1)
    StatusMessage: NotRequired[str],
    PercentDone: NotRequired[str],
    BackupSizeInBytes: NotRequired[int],
    IamRoleArn: NotRequired[str],
    CreatedBy: NotRequired[RecoveryPointCreatorTypeDef],  # (2)
    ExpectedCompletionDate: NotRequired[datetime],
    StartBy: NotRequired[datetime],
    ResourceType: NotRequired[str],
    BytesTransferred: NotRequired[int],
    BackupOptions: NotRequired[Dict[str, str]],
    BackupType: NotRequired[str],
    ParentJobId: NotRequired[str],
    IsParent: NotRequired[bool],
    ResourceName: NotRequired[str],
    InitiationDate: NotRequired[datetime],
    MessageCategory: NotRequired[str],
```

1. See [:material-code-brackets: BackupJobStateType](./literals.md#backupjobstatetype) 
2. See [:material-code-braces: RecoveryPointCreatorTypeDef](./type_defs.md#recoverypointcreatortypedef) 
## CopyJobTypeDef

```python
# CopyJobTypeDef definition

class CopyJobTypeDef(TypedDict):
    AccountId: NotRequired[str],
    CopyJobId: NotRequired[str],
    SourceBackupVaultArn: NotRequired[str],
    SourceRecoveryPointArn: NotRequired[str],
    DestinationBackupVaultArn: NotRequired[str],
    DestinationRecoveryPointArn: NotRequired[str],
    ResourceArn: NotRequired[str],
    CreationDate: NotRequired[datetime],
    CompletionDate: NotRequired[datetime],
    State: NotRequired[CopyJobStateType],  # (1)
    StatusMessage: NotRequired[str],
    BackupSizeInBytes: NotRequired[int],
    IamRoleArn: NotRequired[str],
    CreatedBy: NotRequired[RecoveryPointCreatorTypeDef],  # (2)
    ResourceType: NotRequired[str],
    ParentJobId: NotRequired[str],
    IsParent: NotRequired[bool],
    CompositeMemberIdentifier: NotRequired[str],
    NumberOfChildJobs: NotRequired[int],
    ChildJobsInState: NotRequired[Dict[CopyJobStateType, int]],  # (3)
    ResourceName: NotRequired[str],
    MessageCategory: NotRequired[str],
```

1. See [:material-code-brackets: CopyJobStateType](./literals.md#copyjobstatetype) 
2. See [:material-code-braces: RecoveryPointCreatorTypeDef](./type_defs.md#recoverypointcreatortypedef) 
3. See [:material-code-brackets: CopyJobStateType](./literals.md#copyjobstatetype) 
## CopyActionTypeDef

```python
# CopyActionTypeDef definition

class CopyActionTypeDef(TypedDict):
    DestinationBackupVaultArn: str,
    Lifecycle: NotRequired[LifecycleTypeDef],  # (1)
```

1. See [:material-code-braces: LifecycleTypeDef](./type_defs.md#lifecycletypedef) 
## StartBackupJobInputRequestTypeDef

```python
# StartBackupJobInputRequestTypeDef definition

class StartBackupJobInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
    ResourceArn: str,
    IamRoleArn: str,
    IdempotencyToken: NotRequired[str],
    StartWindowMinutes: NotRequired[int],
    CompleteWindowMinutes: NotRequired[int],
    Lifecycle: NotRequired[LifecycleTypeDef],  # (1)
    RecoveryPointTags: NotRequired[Mapping[str, str]],
    BackupOptions: NotRequired[Mapping[str, str]],
    Index: NotRequired[IndexType],  # (2)
```

1. See [:material-code-braces: LifecycleTypeDef](./type_defs.md#lifecycletypedef) 
2. See [:material-code-brackets: IndexType](./literals.md#indextype) 
## StartCopyJobInputRequestTypeDef

```python
# StartCopyJobInputRequestTypeDef definition

class StartCopyJobInputRequestTypeDef(TypedDict):
    RecoveryPointArn: str,
    SourceBackupVaultName: str,
    DestinationBackupVaultArn: str,
    IamRoleArn: str,
    IdempotencyToken: NotRequired[str],
    Lifecycle: NotRequired[LifecycleTypeDef],  # (1)
```

1. See [:material-code-braces: LifecycleTypeDef](./type_defs.md#lifecycletypedef) 
## UpdateRecoveryPointLifecycleInputRequestTypeDef

```python
# UpdateRecoveryPointLifecycleInputRequestTypeDef definition

class UpdateRecoveryPointLifecycleInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
    RecoveryPointArn: str,
    Lifecycle: NotRequired[LifecycleTypeDef],  # (1)
```

1. See [:material-code-braces: LifecycleTypeDef](./type_defs.md#lifecycletypedef) 
## RecoveryPointByBackupVaultTypeDef

```python
# RecoveryPointByBackupVaultTypeDef definition

class RecoveryPointByBackupVaultTypeDef(TypedDict):
    RecoveryPointArn: NotRequired[str],
    BackupVaultName: NotRequired[str],
    BackupVaultArn: NotRequired[str],
    SourceBackupVaultArn: NotRequired[str],
    ResourceArn: NotRequired[str],
    ResourceType: NotRequired[str],
    CreatedBy: NotRequired[RecoveryPointCreatorTypeDef],  # (1)
    IamRoleArn: NotRequired[str],
    Status: NotRequired[RecoveryPointStatusType],  # (2)
    StatusMessage: NotRequired[str],
    CreationDate: NotRequired[datetime],
    CompletionDate: NotRequired[datetime],
    BackupSizeInBytes: NotRequired[int],
    CalculatedLifecycle: NotRequired[CalculatedLifecycleTypeDef],  # (3)
    Lifecycle: NotRequired[LifecycleTypeDef],  # (4)
    EncryptionKeyArn: NotRequired[str],
    IsEncrypted: NotRequired[bool],
    LastRestoreTime: NotRequired[datetime],
    ParentRecoveryPointArn: NotRequired[str],
    CompositeMemberIdentifier: NotRequired[str],
    IsParent: NotRequired[bool],
    ResourceName: NotRequired[str],
    VaultType: NotRequired[VaultTypeType],  # (5)
    IndexStatus: NotRequired[IndexStatusType],  # (6)
    IndexStatusMessage: NotRequired[str],
```

1. See [:material-code-braces: RecoveryPointCreatorTypeDef](./type_defs.md#recoverypointcreatortypedef) 
2. See [:material-code-brackets: RecoveryPointStatusType](./literals.md#recoverypointstatustype) 
3. See [:material-code-braces: CalculatedLifecycleTypeDef](./type_defs.md#calculatedlifecycletypedef) 
4. See [:material-code-braces: LifecycleTypeDef](./type_defs.md#lifecycletypedef) 
5. See [:material-code-brackets: VaultTypeType](./literals.md#vaulttypetype) 
6. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
## ConditionsOutputTypeDef

```python
# ConditionsOutputTypeDef definition

class ConditionsOutputTypeDef(TypedDict):
    StringEquals: NotRequired[List[ConditionParameterTypeDef]],  # (1)
    StringNotEquals: NotRequired[List[ConditionParameterTypeDef]],  # (1)
    StringLike: NotRequired[List[ConditionParameterTypeDef]],  # (1)
    StringNotLike: NotRequired[List[ConditionParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: ConditionParameterTypeDef](./type_defs.md#conditionparametertypedef) 
2. See [:material-code-braces: ConditionParameterTypeDef](./type_defs.md#conditionparametertypedef) 
3. See [:material-code-braces: ConditionParameterTypeDef](./type_defs.md#conditionparametertypedef) 
4. See [:material-code-braces: ConditionParameterTypeDef](./type_defs.md#conditionparametertypedef) 
## ConditionsTypeDef

```python
# ConditionsTypeDef definition

class ConditionsTypeDef(TypedDict):
    StringEquals: NotRequired[Sequence[ConditionParameterTypeDef]],  # (1)
    StringNotEquals: NotRequired[Sequence[ConditionParameterTypeDef]],  # (1)
    StringLike: NotRequired[Sequence[ConditionParameterTypeDef]],  # (1)
    StringNotLike: NotRequired[Sequence[ConditionParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: ConditionParameterTypeDef](./type_defs.md#conditionparametertypedef) 
2. See [:material-code-braces: ConditionParameterTypeDef](./type_defs.md#conditionparametertypedef) 
3. See [:material-code-braces: ConditionParameterTypeDef](./type_defs.md#conditionparametertypedef) 
4. See [:material-code-braces: ConditionParameterTypeDef](./type_defs.md#conditionparametertypedef) 
## FrameworkControlOutputTypeDef

```python
# FrameworkControlOutputTypeDef definition

class FrameworkControlOutputTypeDef(TypedDict):
    ControlName: str,
    ControlInputParameters: NotRequired[List[ControlInputParameterTypeDef]],  # (1)
    ControlScope: NotRequired[ControlScopeOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ControlInputParameterTypeDef](./type_defs.md#controlinputparametertypedef) 
2. See [:material-code-braces: ControlScopeOutputTypeDef](./type_defs.md#controlscopeoutputtypedef) 
## CreateBackupPlanOutputTypeDef

```python
# CreateBackupPlanOutputTypeDef definition

class CreateBackupPlanOutputTypeDef(TypedDict):
    BackupPlanId: str,
    BackupPlanArn: str,
    CreationDate: datetime,
    VersionId: str,
    AdvancedBackupSettings: List[AdvancedBackupSettingOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AdvancedBackupSettingOutputTypeDef](./type_defs.md#advancedbackupsettingoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBackupSelectionOutputTypeDef

```python
# CreateBackupSelectionOutputTypeDef definition

class CreateBackupSelectionOutputTypeDef(TypedDict):
    SelectionId: str,
    BackupPlanId: str,
    CreationDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBackupVaultOutputTypeDef

```python
# CreateBackupVaultOutputTypeDef definition

class CreateBackupVaultOutputTypeDef(TypedDict):
    BackupVaultName: str,
    BackupVaultArn: str,
    CreationDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFrameworkOutputTypeDef

```python
# CreateFrameworkOutputTypeDef definition

class CreateFrameworkOutputTypeDef(TypedDict):
    FrameworkName: str,
    FrameworkArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLogicallyAirGappedBackupVaultOutputTypeDef

```python
# CreateLogicallyAirGappedBackupVaultOutputTypeDef definition

class CreateLogicallyAirGappedBackupVaultOutputTypeDef(TypedDict):
    BackupVaultName: str,
    BackupVaultArn: str,
    CreationDate: datetime,
    VaultState: VaultStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: VaultStateType](./literals.md#vaultstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateReportPlanOutputTypeDef

```python
# CreateReportPlanOutputTypeDef definition

class CreateReportPlanOutputTypeDef(TypedDict):
    ReportPlanName: str,
    ReportPlanArn: str,
    CreationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRestoreTestingPlanOutputTypeDef

```python
# CreateRestoreTestingPlanOutputTypeDef definition

class CreateRestoreTestingPlanOutputTypeDef(TypedDict):
    CreationTime: datetime,
    RestoreTestingPlanArn: str,
    RestoreTestingPlanName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRestoreTestingSelectionOutputTypeDef

```python
# CreateRestoreTestingSelectionOutputTypeDef definition

class CreateRestoreTestingSelectionOutputTypeDef(TypedDict):
    CreationTime: datetime,
    RestoreTestingPlanArn: str,
    RestoreTestingPlanName: str,
    RestoreTestingSelectionName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBackupPlanOutputTypeDef

```python
# DeleteBackupPlanOutputTypeDef definition

class DeleteBackupPlanOutputTypeDef(TypedDict):
    BackupPlanId: str,
    BackupPlanArn: str,
    DeletionDate: datetime,
    VersionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBackupJobOutputTypeDef

```python
# DescribeBackupJobOutputTypeDef definition

class DescribeBackupJobOutputTypeDef(TypedDict):
    AccountId: str,
    BackupJobId: str,
    BackupVaultName: str,
    BackupVaultArn: str,
    RecoveryPointArn: str,
    ResourceArn: str,
    CreationDate: datetime,
    CompletionDate: datetime,
    State: BackupJobStateType,  # (1)
    StatusMessage: str,
    PercentDone: str,
    BackupSizeInBytes: int,
    IamRoleArn: str,
    CreatedBy: RecoveryPointCreatorTypeDef,  # (2)
    ResourceType: str,
    BytesTransferred: int,
    ExpectedCompletionDate: datetime,
    StartBy: datetime,
    BackupOptions: Dict[str, str],
    BackupType: str,
    ParentJobId: str,
    IsParent: bool,
    NumberOfChildJobs: int,
    ChildJobsInState: Dict[BackupJobStateType, int],  # (3)
    ResourceName: str,
    InitiationDate: datetime,
    MessageCategory: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: BackupJobStateType](./literals.md#backupjobstatetype) 
2. See [:material-code-braces: RecoveryPointCreatorTypeDef](./type_defs.md#recoverypointcreatortypedef) 
3. See [:material-code-brackets: BackupJobStateType](./literals.md#backupjobstatetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBackupVaultOutputTypeDef

```python
# DescribeBackupVaultOutputTypeDef definition

class DescribeBackupVaultOutputTypeDef(TypedDict):
    BackupVaultName: str,
    BackupVaultArn: str,
    VaultType: VaultTypeType,  # (1)
    VaultState: VaultStateType,  # (2)
    EncryptionKeyArn: str,
    CreationDate: datetime,
    CreatorRequestId: str,
    NumberOfRecoveryPoints: int,
    Locked: bool,
    MinRetentionDays: int,
    MaxRetentionDays: int,
    LockDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: VaultTypeType](./literals.md#vaulttypetype) 
2. See [:material-code-brackets: VaultStateType](./literals.md#vaultstatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGlobalSettingsOutputTypeDef

```python
# DescribeGlobalSettingsOutputTypeDef definition

class DescribeGlobalSettingsOutputTypeDef(TypedDict):
    GlobalSettings: Dict[str, str],
    LastUpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeProtectedResourceOutputTypeDef

```python
# DescribeProtectedResourceOutputTypeDef definition

class DescribeProtectedResourceOutputTypeDef(TypedDict):
    ResourceArn: str,
    ResourceType: str,
    LastBackupTime: datetime,
    ResourceName: str,
    LastBackupVaultArn: str,
    LastRecoveryPointArn: str,
    LatestRestoreExecutionTimeMinutes: int,
    LatestRestoreJobCreationDate: datetime,
    LatestRestoreRecoveryPointCreationDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRecoveryPointOutputTypeDef

```python
# DescribeRecoveryPointOutputTypeDef definition

class DescribeRecoveryPointOutputTypeDef(TypedDict):
    RecoveryPointArn: str,
    BackupVaultName: str,
    BackupVaultArn: str,
    SourceBackupVaultArn: str,
    ResourceArn: str,
    ResourceType: str,
    CreatedBy: RecoveryPointCreatorTypeDef,  # (1)
    IamRoleArn: str,
    Status: RecoveryPointStatusType,  # (2)
    StatusMessage: str,
    CreationDate: datetime,
    CompletionDate: datetime,
    BackupSizeInBytes: int,
    CalculatedLifecycle: CalculatedLifecycleTypeDef,  # (3)
    Lifecycle: LifecycleTypeDef,  # (4)
    EncryptionKeyArn: str,
    IsEncrypted: bool,
    StorageClass: StorageClassType,  # (5)
    LastRestoreTime: datetime,
    ParentRecoveryPointArn: str,
    CompositeMemberIdentifier: str,
    IsParent: bool,
    ResourceName: str,
    VaultType: VaultTypeType,  # (6)
    IndexStatus: IndexStatusType,  # (7)
    IndexStatusMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-braces: RecoveryPointCreatorTypeDef](./type_defs.md#recoverypointcreatortypedef) 
2. See [:material-code-brackets: RecoveryPointStatusType](./literals.md#recoverypointstatustype) 
3. See [:material-code-braces: CalculatedLifecycleTypeDef](./type_defs.md#calculatedlifecycletypedef) 
4. See [:material-code-braces: LifecycleTypeDef](./type_defs.md#lifecycletypedef) 
5. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
6. See [:material-code-brackets: VaultTypeType](./literals.md#vaulttypetype) 
7. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRegionSettingsOutputTypeDef

```python
# DescribeRegionSettingsOutputTypeDef definition

class DescribeRegionSettingsOutputTypeDef(TypedDict):
    ResourceTypeOptInPreference: Dict[str, bool],
    ResourceTypeManagementPreference: Dict[str, bool],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportBackupPlanTemplateOutputTypeDef

```python
# ExportBackupPlanTemplateOutputTypeDef definition

class ExportBackupPlanTemplateOutputTypeDef(TypedDict):
    BackupPlanTemplateJson: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBackupVaultAccessPolicyOutputTypeDef

```python
# GetBackupVaultAccessPolicyOutputTypeDef definition

class GetBackupVaultAccessPolicyOutputTypeDef(TypedDict):
    BackupVaultName: str,
    BackupVaultArn: str,
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBackupVaultNotificationsOutputTypeDef

```python
# GetBackupVaultNotificationsOutputTypeDef definition

class GetBackupVaultNotificationsOutputTypeDef(TypedDict):
    BackupVaultName: str,
    BackupVaultArn: str,
    SNSTopicArn: str,
    BackupVaultEvents: List[BackupVaultEventType],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: BackupVaultEventType](./literals.md#backupvaulteventtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRecoveryPointIndexDetailsOutputTypeDef

```python
# GetRecoveryPointIndexDetailsOutputTypeDef definition

class GetRecoveryPointIndexDetailsOutputTypeDef(TypedDict):
    RecoveryPointArn: str,
    BackupVaultArn: str,
    SourceResourceArn: str,
    IndexCreationDate: datetime,
    IndexDeletionDate: datetime,
    IndexCompletionDate: datetime,
    IndexStatus: IndexStatusType,  # (1)
    IndexStatusMessage: str,
    TotalItemsIndexed: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRecoveryPointRestoreMetadataOutputTypeDef

```python
# GetRecoveryPointRestoreMetadataOutputTypeDef definition

class GetRecoveryPointRestoreMetadataOutputTypeDef(TypedDict):
    BackupVaultArn: str,
    RecoveryPointArn: str,
    RestoreMetadata: Dict[str, str],
    ResourceType: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRestoreJobMetadataOutputTypeDef

```python
# GetRestoreJobMetadataOutputTypeDef definition

class GetRestoreJobMetadataOutputTypeDef(TypedDict):
    RestoreJobId: str,
    Metadata: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRestoreTestingInferredMetadataOutputTypeDef

```python
# GetRestoreTestingInferredMetadataOutputTypeDef definition

class GetRestoreTestingInferredMetadataOutputTypeDef(TypedDict):
    InferredMetadata: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSupportedResourceTypesOutputTypeDef

```python
# GetSupportedResourceTypesOutputTypeDef definition

class GetSupportedResourceTypesOutputTypeDef(TypedDict):
    ResourceTypes: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBackupJobSummariesOutputTypeDef

```python
# ListBackupJobSummariesOutputTypeDef definition

class ListBackupJobSummariesOutputTypeDef(TypedDict):
    BackupJobSummaries: List[BackupJobSummaryTypeDef],  # (1)
    AggregationPeriod: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BackupJobSummaryTypeDef](./type_defs.md#backupjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBackupPlanTemplatesOutputTypeDef

```python
# ListBackupPlanTemplatesOutputTypeDef definition

class ListBackupPlanTemplatesOutputTypeDef(TypedDict):
    BackupPlanTemplatesList: List[BackupPlanTemplatesListMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BackupPlanTemplatesListMemberTypeDef](./type_defs.md#backupplantemplateslistmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBackupSelectionsOutputTypeDef

```python
# ListBackupSelectionsOutputTypeDef definition

class ListBackupSelectionsOutputTypeDef(TypedDict):
    BackupSelectionsList: List[BackupSelectionsListMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BackupSelectionsListMemberTypeDef](./type_defs.md#backupselectionslistmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBackupVaultsOutputTypeDef

```python
# ListBackupVaultsOutputTypeDef definition

class ListBackupVaultsOutputTypeDef(TypedDict):
    BackupVaultList: List[BackupVaultListMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BackupVaultListMemberTypeDef](./type_defs.md#backupvaultlistmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCopyJobSummariesOutputTypeDef

```python
# ListCopyJobSummariesOutputTypeDef definition

class ListCopyJobSummariesOutputTypeDef(TypedDict):
    CopyJobSummaries: List[CopyJobSummaryTypeDef],  # (1)
    AggregationPeriod: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CopyJobSummaryTypeDef](./type_defs.md#copyjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsOutputTypeDef

```python
# ListTagsOutputTypeDef definition

class ListTagsOutputTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartBackupJobOutputTypeDef

```python
# StartBackupJobOutputTypeDef definition

class StartBackupJobOutputTypeDef(TypedDict):
    BackupJobId: str,
    RecoveryPointArn: str,
    CreationDate: datetime,
    IsParent: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartCopyJobOutputTypeDef

```python
# StartCopyJobOutputTypeDef definition

class StartCopyJobOutputTypeDef(TypedDict):
    CopyJobId: str,
    CreationDate: datetime,
    IsParent: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartReportJobOutputTypeDef

```python
# StartReportJobOutputTypeDef definition

class StartReportJobOutputTypeDef(TypedDict):
    ReportJobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartRestoreJobOutputTypeDef

```python
# StartRestoreJobOutputTypeDef definition

class StartRestoreJobOutputTypeDef(TypedDict):
    RestoreJobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBackupPlanOutputTypeDef

```python
# UpdateBackupPlanOutputTypeDef definition

class UpdateBackupPlanOutputTypeDef(TypedDict):
    BackupPlanId: str,
    BackupPlanArn: str,
    CreationDate: datetime,
    VersionId: str,
    AdvancedBackupSettings: List[AdvancedBackupSettingOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AdvancedBackupSettingOutputTypeDef](./type_defs.md#advancedbackupsettingoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFrameworkOutputTypeDef

```python
# UpdateFrameworkOutputTypeDef definition

class UpdateFrameworkOutputTypeDef(TypedDict):
    FrameworkName: str,
    FrameworkArn: str,
    CreationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRecoveryPointIndexSettingsOutputTypeDef

```python
# UpdateRecoveryPointIndexSettingsOutputTypeDef definition

class UpdateRecoveryPointIndexSettingsOutputTypeDef(TypedDict):
    BackupVaultName: str,
    RecoveryPointArn: str,
    IndexStatus: IndexStatusType,  # (1)
    Index: IndexType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
2. See [:material-code-brackets: IndexType](./literals.md#indextype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRecoveryPointLifecycleOutputTypeDef

```python
# UpdateRecoveryPointLifecycleOutputTypeDef definition

class UpdateRecoveryPointLifecycleOutputTypeDef(TypedDict):
    BackupVaultArn: str,
    RecoveryPointArn: str,
    Lifecycle: LifecycleTypeDef,  # (1)
    CalculatedLifecycle: CalculatedLifecycleTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: LifecycleTypeDef](./type_defs.md#lifecycletypedef) 
2. See [:material-code-braces: CalculatedLifecycleTypeDef](./type_defs.md#calculatedlifecycletypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateReportPlanOutputTypeDef

```python
# UpdateReportPlanOutputTypeDef definition

class UpdateReportPlanOutputTypeDef(TypedDict):
    ReportPlanName: str,
    ReportPlanArn: str,
    CreationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRestoreTestingPlanOutputTypeDef

```python
# UpdateRestoreTestingPlanOutputTypeDef definition

class UpdateRestoreTestingPlanOutputTypeDef(TypedDict):
    CreationTime: datetime,
    RestoreTestingPlanArn: str,
    RestoreTestingPlanName: str,
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRestoreTestingSelectionOutputTypeDef

```python
# UpdateRestoreTestingSelectionOutputTypeDef definition

class UpdateRestoreTestingSelectionOutputTypeDef(TypedDict):
    CreationTime: datetime,
    RestoreTestingPlanArn: str,
    RestoreTestingPlanName: str,
    RestoreTestingSelectionName: str,
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateReportPlanInputRequestTypeDef

```python
# CreateReportPlanInputRequestTypeDef definition

class CreateReportPlanInputRequestTypeDef(TypedDict):
    ReportPlanName: str,
    ReportDeliveryChannel: ReportDeliveryChannelTypeDef,  # (1)
    ReportSetting: ReportSettingTypeDef,  # (2)
    ReportPlanDescription: NotRequired[str],
    ReportPlanTags: NotRequired[Mapping[str, str]],
    IdempotencyToken: NotRequired[str],
```

1. See [:material-code-braces: ReportDeliveryChannelTypeDef](./type_defs.md#reportdeliverychanneltypedef) 
2. See [:material-code-braces: ReportSettingTypeDef](./type_defs.md#reportsettingtypedef) 
## UpdateReportPlanInputRequestTypeDef

```python
# UpdateReportPlanInputRequestTypeDef definition

class UpdateReportPlanInputRequestTypeDef(TypedDict):
    ReportPlanName: str,
    ReportPlanDescription: NotRequired[str],
    ReportDeliveryChannel: NotRequired[ReportDeliveryChannelTypeDef],  # (1)
    ReportSetting: NotRequired[ReportSettingTypeDef],  # (2)
    IdempotencyToken: NotRequired[str],
```

1. See [:material-code-braces: ReportDeliveryChannelTypeDef](./type_defs.md#reportdeliverychanneltypedef) 
2. See [:material-code-braces: ReportSettingTypeDef](./type_defs.md#reportsettingtypedef) 
## RecoveryPointSelectionOutputTypeDef

```python
# RecoveryPointSelectionOutputTypeDef definition

class RecoveryPointSelectionOutputTypeDef(TypedDict):
    VaultNames: NotRequired[List[str]],
    ResourceIdentifiers: NotRequired[List[str]],
    DateRange: NotRequired[DateRangeOutputTypeDef],  # (1)
```

1. See [:material-code-braces: DateRangeOutputTypeDef](./type_defs.md#daterangeoutputtypedef) 
## DateRangeTypeDef

```python
# DateRangeTypeDef definition

class DateRangeTypeDef(TypedDict):
    FromDate: TimestampTypeDef,
    ToDate: TimestampTypeDef,
```

## ListBackupJobsInputRequestTypeDef

```python
# ListBackupJobsInputRequestTypeDef definition

class ListBackupJobsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ByResourceArn: NotRequired[str],
    ByState: NotRequired[BackupJobStateType],  # (1)
    ByBackupVaultName: NotRequired[str],
    ByCreatedBefore: NotRequired[TimestampTypeDef],
    ByCreatedAfter: NotRequired[TimestampTypeDef],
    ByResourceType: NotRequired[str],
    ByAccountId: NotRequired[str],
    ByCompleteAfter: NotRequired[TimestampTypeDef],
    ByCompleteBefore: NotRequired[TimestampTypeDef],
    ByParentJobId: NotRequired[str],
    ByMessageCategory: NotRequired[str],
```

1. See [:material-code-brackets: BackupJobStateType](./literals.md#backupjobstatetype) 
## ListCopyJobsInputRequestTypeDef

```python
# ListCopyJobsInputRequestTypeDef definition

class ListCopyJobsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ByResourceArn: NotRequired[str],
    ByState: NotRequired[CopyJobStateType],  # (1)
    ByCreatedBefore: NotRequired[TimestampTypeDef],
    ByCreatedAfter: NotRequired[TimestampTypeDef],
    ByResourceType: NotRequired[str],
    ByDestinationVaultArn: NotRequired[str],
    ByAccountId: NotRequired[str],
    ByCompleteBefore: NotRequired[TimestampTypeDef],
    ByCompleteAfter: NotRequired[TimestampTypeDef],
    ByParentJobId: NotRequired[str],
    ByMessageCategory: NotRequired[str],
```

1. See [:material-code-brackets: CopyJobStateType](./literals.md#copyjobstatetype) 
## ListIndexedRecoveryPointsInputRequestTypeDef

```python
# ListIndexedRecoveryPointsInputRequestTypeDef definition

class ListIndexedRecoveryPointsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SourceResourceArn: NotRequired[str],
    CreatedBefore: NotRequired[TimestampTypeDef],
    CreatedAfter: NotRequired[TimestampTypeDef],
    ResourceType: NotRequired[str],
    IndexStatus: NotRequired[IndexStatusType],  # (1)
```

1. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
## ListRecoveryPointsByBackupVaultInputRequestTypeDef

```python
# ListRecoveryPointsByBackupVaultInputRequestTypeDef definition

class ListRecoveryPointsByBackupVaultInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
    BackupVaultAccountId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ByResourceArn: NotRequired[str],
    ByResourceType: NotRequired[str],
    ByBackupPlanId: NotRequired[str],
    ByCreatedBefore: NotRequired[TimestampTypeDef],
    ByCreatedAfter: NotRequired[TimestampTypeDef],
    ByParentRecoveryPointArn: NotRequired[str],
```

## ListReportJobsInputRequestTypeDef

```python
# ListReportJobsInputRequestTypeDef definition

class ListReportJobsInputRequestTypeDef(TypedDict):
    ByReportPlanName: NotRequired[str],
    ByCreationBefore: NotRequired[TimestampTypeDef],
    ByCreationAfter: NotRequired[TimestampTypeDef],
    ByStatus: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListRestoreJobsByProtectedResourceInputRequestTypeDef

```python
# ListRestoreJobsByProtectedResourceInputRequestTypeDef definition

class ListRestoreJobsByProtectedResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    ByStatus: NotRequired[RestoreJobStatusType],  # (1)
    ByRecoveryPointCreationDateAfter: NotRequired[TimestampTypeDef],
    ByRecoveryPointCreationDateBefore: NotRequired[TimestampTypeDef],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: RestoreJobStatusType](./literals.md#restorejobstatustype) 
## ListRestoreJobsInputRequestTypeDef

```python
# ListRestoreJobsInputRequestTypeDef definition

class ListRestoreJobsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ByAccountId: NotRequired[str],
    ByResourceType: NotRequired[str],
    ByCreatedBefore: NotRequired[TimestampTypeDef],
    ByCreatedAfter: NotRequired[TimestampTypeDef],
    ByStatus: NotRequired[RestoreJobStatusType],  # (1)
    ByCompleteBefore: NotRequired[TimestampTypeDef],
    ByCompleteAfter: NotRequired[TimestampTypeDef],
    ByRestoreTestingPlanArn: NotRequired[str],
```

1. See [:material-code-brackets: RestoreJobStatusType](./literals.md#restorejobstatustype) 
## DescribeRestoreJobOutputTypeDef

```python
# DescribeRestoreJobOutputTypeDef definition

class DescribeRestoreJobOutputTypeDef(TypedDict):
    AccountId: str,
    RestoreJobId: str,
    RecoveryPointArn: str,
    CreationDate: datetime,
    CompletionDate: datetime,
    Status: RestoreJobStatusType,  # (1)
    StatusMessage: str,
    PercentDone: str,
    BackupSizeInBytes: int,
    IamRoleArn: str,
    ExpectedCompletionTimeMinutes: int,
    CreatedResourceArn: str,
    ResourceType: str,
    RecoveryPointCreationDate: datetime,
    CreatedBy: RestoreJobCreatorTypeDef,  # (2)
    ValidationStatus: RestoreValidationStatusType,  # (3)
    ValidationStatusMessage: str,
    DeletionStatus: RestoreDeletionStatusType,  # (4)
    DeletionStatusMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: RestoreJobStatusType](./literals.md#restorejobstatustype) 
2. See [:material-code-braces: RestoreJobCreatorTypeDef](./type_defs.md#restorejobcreatortypedef) 
3. See [:material-code-brackets: RestoreValidationStatusType](./literals.md#restorevalidationstatustype) 
4. See [:material-code-brackets: RestoreDeletionStatusType](./literals.md#restoredeletionstatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreJobsListMemberTypeDef

```python
# RestoreJobsListMemberTypeDef definition

class RestoreJobsListMemberTypeDef(TypedDict):
    AccountId: NotRequired[str],
    RestoreJobId: NotRequired[str],
    RecoveryPointArn: NotRequired[str],
    CreationDate: NotRequired[datetime],
    CompletionDate: NotRequired[datetime],
    Status: NotRequired[RestoreJobStatusType],  # (1)
    StatusMessage: NotRequired[str],
    PercentDone: NotRequired[str],
    BackupSizeInBytes: NotRequired[int],
    IamRoleArn: NotRequired[str],
    ExpectedCompletionTimeMinutes: NotRequired[int],
    CreatedResourceArn: NotRequired[str],
    ResourceType: NotRequired[str],
    RecoveryPointCreationDate: NotRequired[datetime],
    CreatedBy: NotRequired[RestoreJobCreatorTypeDef],  # (2)
    ValidationStatus: NotRequired[RestoreValidationStatusType],  # (3)
    ValidationStatusMessage: NotRequired[str],
    DeletionStatus: NotRequired[RestoreDeletionStatusType],  # (4)
    DeletionStatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: RestoreJobStatusType](./literals.md#restorejobstatustype) 
2. See [:material-code-braces: RestoreJobCreatorTypeDef](./type_defs.md#restorejobcreatortypedef) 
3. See [:material-code-brackets: RestoreValidationStatusType](./literals.md#restorevalidationstatustype) 
4. See [:material-code-brackets: RestoreDeletionStatusType](./literals.md#restoredeletionstatustype) 
## ListFrameworksOutputTypeDef

```python
# ListFrameworksOutputTypeDef definition

class ListFrameworksOutputTypeDef(TypedDict):
    Frameworks: List[FrameworkTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FrameworkTypeDef](./type_defs.md#frameworktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIndexedRecoveryPointsOutputTypeDef

```python
# ListIndexedRecoveryPointsOutputTypeDef definition

class ListIndexedRecoveryPointsOutputTypeDef(TypedDict):
    IndexedRecoveryPoints: List[IndexedRecoveryPointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IndexedRecoveryPointTypeDef](./type_defs.md#indexedrecoverypointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProtectedResourceConditionsOutputTypeDef

```python
# ProtectedResourceConditionsOutputTypeDef definition

class ProtectedResourceConditionsOutputTypeDef(TypedDict):
    StringEquals: NotRequired[List[KeyValueTypeDef]],  # (1)
    StringNotEquals: NotRequired[List[KeyValueTypeDef]],  # (1)
```

1. See [:material-code-braces: KeyValueTypeDef](./type_defs.md#keyvaluetypedef) 
2. See [:material-code-braces: KeyValueTypeDef](./type_defs.md#keyvaluetypedef) 
## ProtectedResourceConditionsTypeDef

```python
# ProtectedResourceConditionsTypeDef definition

class ProtectedResourceConditionsTypeDef(TypedDict):
    StringEquals: NotRequired[Sequence[KeyValueTypeDef]],  # (1)
    StringNotEquals: NotRequired[Sequence[KeyValueTypeDef]],  # (1)
```

1. See [:material-code-braces: KeyValueTypeDef](./type_defs.md#keyvaluetypedef) 
2. See [:material-code-braces: KeyValueTypeDef](./type_defs.md#keyvaluetypedef) 
## ListLegalHoldsOutputTypeDef

```python
# ListLegalHoldsOutputTypeDef definition

class ListLegalHoldsOutputTypeDef(TypedDict):
    LegalHolds: List[LegalHoldTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LegalHoldTypeDef](./type_defs.md#legalholdtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBackupJobsInputPaginateTypeDef

```python
# ListBackupJobsInputPaginateTypeDef definition

class ListBackupJobsInputPaginateTypeDef(TypedDict):
    ByResourceArn: NotRequired[str],
    ByState: NotRequired[BackupJobStateType],  # (1)
    ByBackupVaultName: NotRequired[str],
    ByCreatedBefore: NotRequired[TimestampTypeDef],
    ByCreatedAfter: NotRequired[TimestampTypeDef],
    ByResourceType: NotRequired[str],
    ByAccountId: NotRequired[str],
    ByCompleteAfter: NotRequired[TimestampTypeDef],
    ByCompleteBefore: NotRequired[TimestampTypeDef],
    ByParentJobId: NotRequired[str],
    ByMessageCategory: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: BackupJobStateType](./literals.md#backupjobstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBackupPlanTemplatesInputPaginateTypeDef

```python
# ListBackupPlanTemplatesInputPaginateTypeDef definition

class ListBackupPlanTemplatesInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBackupPlanVersionsInputPaginateTypeDef

```python
# ListBackupPlanVersionsInputPaginateTypeDef definition

class ListBackupPlanVersionsInputPaginateTypeDef(TypedDict):
    BackupPlanId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBackupPlansInputPaginateTypeDef

```python
# ListBackupPlansInputPaginateTypeDef definition

class ListBackupPlansInputPaginateTypeDef(TypedDict):
    IncludeDeleted: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBackupSelectionsInputPaginateTypeDef

```python
# ListBackupSelectionsInputPaginateTypeDef definition

class ListBackupSelectionsInputPaginateTypeDef(TypedDict):
    BackupPlanId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBackupVaultsInputPaginateTypeDef

```python
# ListBackupVaultsInputPaginateTypeDef definition

class ListBackupVaultsInputPaginateTypeDef(TypedDict):
    ByVaultType: NotRequired[VaultTypeType],  # (1)
    ByShared: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: VaultTypeType](./literals.md#vaulttypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCopyJobsInputPaginateTypeDef

```python
# ListCopyJobsInputPaginateTypeDef definition

class ListCopyJobsInputPaginateTypeDef(TypedDict):
    ByResourceArn: NotRequired[str],
    ByState: NotRequired[CopyJobStateType],  # (1)
    ByCreatedBefore: NotRequired[TimestampTypeDef],
    ByCreatedAfter: NotRequired[TimestampTypeDef],
    ByResourceType: NotRequired[str],
    ByDestinationVaultArn: NotRequired[str],
    ByAccountId: NotRequired[str],
    ByCompleteBefore: NotRequired[TimestampTypeDef],
    ByCompleteAfter: NotRequired[TimestampTypeDef],
    ByParentJobId: NotRequired[str],
    ByMessageCategory: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: CopyJobStateType](./literals.md#copyjobstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIndexedRecoveryPointsInputPaginateTypeDef

```python
# ListIndexedRecoveryPointsInputPaginateTypeDef definition

class ListIndexedRecoveryPointsInputPaginateTypeDef(TypedDict):
    SourceResourceArn: NotRequired[str],
    CreatedBefore: NotRequired[TimestampTypeDef],
    CreatedAfter: NotRequired[TimestampTypeDef],
    ResourceType: NotRequired[str],
    IndexStatus: NotRequired[IndexStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLegalHoldsInputPaginateTypeDef

```python
# ListLegalHoldsInputPaginateTypeDef definition

class ListLegalHoldsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProtectedResourcesByBackupVaultInputPaginateTypeDef

```python
# ListProtectedResourcesByBackupVaultInputPaginateTypeDef definition

class ListProtectedResourcesByBackupVaultInputPaginateTypeDef(TypedDict):
    BackupVaultName: str,
    BackupVaultAccountId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProtectedResourcesInputPaginateTypeDef

```python
# ListProtectedResourcesInputPaginateTypeDef definition

class ListProtectedResourcesInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecoveryPointsByBackupVaultInputPaginateTypeDef

```python
# ListRecoveryPointsByBackupVaultInputPaginateTypeDef definition

class ListRecoveryPointsByBackupVaultInputPaginateTypeDef(TypedDict):
    BackupVaultName: str,
    BackupVaultAccountId: NotRequired[str],
    ByResourceArn: NotRequired[str],
    ByResourceType: NotRequired[str],
    ByBackupPlanId: NotRequired[str],
    ByCreatedBefore: NotRequired[TimestampTypeDef],
    ByCreatedAfter: NotRequired[TimestampTypeDef],
    ByParentRecoveryPointArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecoveryPointsByLegalHoldInputPaginateTypeDef

```python
# ListRecoveryPointsByLegalHoldInputPaginateTypeDef definition

class ListRecoveryPointsByLegalHoldInputPaginateTypeDef(TypedDict):
    LegalHoldId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecoveryPointsByResourceInputPaginateTypeDef

```python
# ListRecoveryPointsByResourceInputPaginateTypeDef definition

class ListRecoveryPointsByResourceInputPaginateTypeDef(TypedDict):
    ResourceArn: str,
    ManagedByAWSBackupOnly: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRestoreJobsByProtectedResourceInputPaginateTypeDef

```python
# ListRestoreJobsByProtectedResourceInputPaginateTypeDef definition

class ListRestoreJobsByProtectedResourceInputPaginateTypeDef(TypedDict):
    ResourceArn: str,
    ByStatus: NotRequired[RestoreJobStatusType],  # (1)
    ByRecoveryPointCreationDateAfter: NotRequired[TimestampTypeDef],
    ByRecoveryPointCreationDateBefore: NotRequired[TimestampTypeDef],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: RestoreJobStatusType](./literals.md#restorejobstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRestoreJobsInputPaginateTypeDef

```python
# ListRestoreJobsInputPaginateTypeDef definition

class ListRestoreJobsInputPaginateTypeDef(TypedDict):
    ByAccountId: NotRequired[str],
    ByResourceType: NotRequired[str],
    ByCreatedBefore: NotRequired[TimestampTypeDef],
    ByCreatedAfter: NotRequired[TimestampTypeDef],
    ByStatus: NotRequired[RestoreJobStatusType],  # (1)
    ByCompleteBefore: NotRequired[TimestampTypeDef],
    ByCompleteAfter: NotRequired[TimestampTypeDef],
    ByRestoreTestingPlanArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: RestoreJobStatusType](./literals.md#restorejobstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRestoreTestingPlansInputPaginateTypeDef

```python
# ListRestoreTestingPlansInputPaginateTypeDef definition

class ListRestoreTestingPlansInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRestoreTestingSelectionsInputPaginateTypeDef

```python
# ListRestoreTestingSelectionsInputPaginateTypeDef definition

class ListRestoreTestingSelectionsInputPaginateTypeDef(TypedDict):
    RestoreTestingPlanName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProtectedResourcesByBackupVaultOutputTypeDef

```python
# ListProtectedResourcesByBackupVaultOutputTypeDef definition

class ListProtectedResourcesByBackupVaultOutputTypeDef(TypedDict):
    Results: List[ProtectedResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProtectedResourceTypeDef](./type_defs.md#protectedresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProtectedResourcesOutputTypeDef

```python
# ListProtectedResourcesOutputTypeDef definition

class ListProtectedResourcesOutputTypeDef(TypedDict):
    Results: List[ProtectedResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProtectedResourceTypeDef](./type_defs.md#protectedresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRecoveryPointsByLegalHoldOutputTypeDef

```python
# ListRecoveryPointsByLegalHoldOutputTypeDef definition

class ListRecoveryPointsByLegalHoldOutputTypeDef(TypedDict):
    RecoveryPoints: List[RecoveryPointMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RecoveryPointMemberTypeDef](./type_defs.md#recoverypointmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRecoveryPointsByResourceOutputTypeDef

```python
# ListRecoveryPointsByResourceOutputTypeDef definition

class ListRecoveryPointsByResourceOutputTypeDef(TypedDict):
    RecoveryPoints: List[RecoveryPointByResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RecoveryPointByResourceTypeDef](./type_defs.md#recoverypointbyresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRestoreJobSummariesOutputTypeDef

```python
# ListRestoreJobSummariesOutputTypeDef definition

class ListRestoreJobSummariesOutputTypeDef(TypedDict):
    RestoreJobSummaries: List[RestoreJobSummaryTypeDef],  # (1)
    AggregationPeriod: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RestoreJobSummaryTypeDef](./type_defs.md#restorejobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRestoreTestingPlansOutputTypeDef

```python
# ListRestoreTestingPlansOutputTypeDef definition

class ListRestoreTestingPlansOutputTypeDef(TypedDict):
    RestoreTestingPlans: List[RestoreTestingPlanForListTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RestoreTestingPlanForListTypeDef](./type_defs.md#restoretestingplanforlisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRestoreTestingSelectionsOutputTypeDef

```python
# ListRestoreTestingSelectionsOutputTypeDef definition

class ListRestoreTestingSelectionsOutputTypeDef(TypedDict):
    RestoreTestingSelections: List[RestoreTestingSelectionForListTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RestoreTestingSelectionForListTypeDef](./type_defs.md#restoretestingselectionforlisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReportJobTypeDef

```python
# ReportJobTypeDef definition

class ReportJobTypeDef(TypedDict):
    ReportJobId: NotRequired[str],
    ReportPlanArn: NotRequired[str],
    ReportTemplate: NotRequired[str],
    CreationTime: NotRequired[datetime],
    CompletionTime: NotRequired[datetime],
    Status: NotRequired[str],
    StatusMessage: NotRequired[str],
    ReportDestination: NotRequired[ReportDestinationTypeDef],  # (1)
```

1. See [:material-code-braces: ReportDestinationTypeDef](./type_defs.md#reportdestinationtypedef) 
## ReportPlanTypeDef

```python
# ReportPlanTypeDef definition

class ReportPlanTypeDef(TypedDict):
    ReportPlanArn: NotRequired[str],
    ReportPlanName: NotRequired[str],
    ReportPlanDescription: NotRequired[str],
    ReportSetting: NotRequired[ReportSettingOutputTypeDef],  # (1)
    ReportDeliveryChannel: NotRequired[ReportDeliveryChannelOutputTypeDef],  # (2)
    DeploymentStatus: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastAttemptedExecutionTime: NotRequired[datetime],
    LastSuccessfulExecutionTime: NotRequired[datetime],
```

1. See [:material-code-braces: ReportSettingOutputTypeDef](./type_defs.md#reportsettingoutputtypedef) 
2. See [:material-code-braces: ReportDeliveryChannelOutputTypeDef](./type_defs.md#reportdeliverychanneloutputtypedef) 
## RestoreTestingPlanForGetTypeDef

```python
# RestoreTestingPlanForGetTypeDef definition

class RestoreTestingPlanForGetTypeDef(TypedDict):
    CreationTime: datetime,
    RecoveryPointSelection: RestoreTestingRecoveryPointSelectionOutputTypeDef,  # (1)
    RestoreTestingPlanArn: str,
    RestoreTestingPlanName: str,
    ScheduleExpression: str,
    CreatorRequestId: NotRequired[str],
    LastExecutionTime: NotRequired[datetime],
    LastUpdateTime: NotRequired[datetime],
    ScheduleExpressionTimezone: NotRequired[str],
    StartWindowHours: NotRequired[int],
```

1. See [:material-code-braces: RestoreTestingRecoveryPointSelectionOutputTypeDef](./type_defs.md#restoretestingrecoverypointselectionoutputtypedef) 
## ListBackupPlanVersionsOutputTypeDef

```python
# ListBackupPlanVersionsOutputTypeDef definition

class ListBackupPlanVersionsOutputTypeDef(TypedDict):
    BackupPlanVersionsList: List[BackupPlansListMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BackupPlansListMemberTypeDef](./type_defs.md#backupplanslistmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBackupPlansOutputTypeDef

```python
# ListBackupPlansOutputTypeDef definition

class ListBackupPlansOutputTypeDef(TypedDict):
    BackupPlansList: List[BackupPlansListMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BackupPlansListMemberTypeDef](./type_defs.md#backupplanslistmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBackupJobsOutputTypeDef

```python
# ListBackupJobsOutputTypeDef definition

class ListBackupJobsOutputTypeDef(TypedDict):
    BackupJobs: List[BackupJobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BackupJobTypeDef](./type_defs.md#backupjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCopyJobOutputTypeDef

```python
# DescribeCopyJobOutputTypeDef definition

class DescribeCopyJobOutputTypeDef(TypedDict):
    CopyJob: CopyJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CopyJobTypeDef](./type_defs.md#copyjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCopyJobsOutputTypeDef

```python
# ListCopyJobsOutputTypeDef definition

class ListCopyJobsOutputTypeDef(TypedDict):
    CopyJobs: List[CopyJobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CopyJobTypeDef](./type_defs.md#copyjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BackupRuleTypeDef

```python
# BackupRuleTypeDef definition

class BackupRuleTypeDef(TypedDict):
    RuleName: str,
    TargetBackupVaultName: str,
    ScheduleExpression: NotRequired[str],
    StartWindowMinutes: NotRequired[int],
    CompletionWindowMinutes: NotRequired[int],
    Lifecycle: NotRequired[LifecycleTypeDef],  # (1)
    RecoveryPointTags: NotRequired[Dict[str, str]],
    RuleId: NotRequired[str],
    CopyActions: NotRequired[List[CopyActionTypeDef]],  # (2)
    EnableContinuousBackup: NotRequired[bool],
    ScheduleExpressionTimezone: NotRequired[str],
    IndexActions: NotRequired[List[IndexActionOutputTypeDef]],  # (3)
```

1. See [:material-code-braces: LifecycleTypeDef](./type_defs.md#lifecycletypedef) 
2. See [:material-code-braces: CopyActionTypeDef](./type_defs.md#copyactiontypedef) 
3. See [:material-code-braces: IndexActionOutputTypeDef](./type_defs.md#indexactionoutputtypedef) 
## ListRecoveryPointsByBackupVaultOutputTypeDef

```python
# ListRecoveryPointsByBackupVaultOutputTypeDef definition

class ListRecoveryPointsByBackupVaultOutputTypeDef(TypedDict):
    RecoveryPoints: List[RecoveryPointByBackupVaultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RecoveryPointByBackupVaultTypeDef](./type_defs.md#recoverypointbybackupvaulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BackupSelectionOutputTypeDef

```python
# BackupSelectionOutputTypeDef definition

class BackupSelectionOutputTypeDef(TypedDict):
    SelectionName: str,
    IamRoleArn: str,
    Resources: NotRequired[List[str]],
    ListOfTags: NotRequired[List[ConditionTypeDef]],  # (1)
    NotResources: NotRequired[List[str]],
    Conditions: NotRequired[ConditionsOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
2. See [:material-code-braces: ConditionsOutputTypeDef](./type_defs.md#conditionsoutputtypedef) 
## DescribeFrameworkOutputTypeDef

```python
# DescribeFrameworkOutputTypeDef definition

class DescribeFrameworkOutputTypeDef(TypedDict):
    FrameworkName: str,
    FrameworkArn: str,
    FrameworkDescription: str,
    FrameworkControls: List[FrameworkControlOutputTypeDef],  # (1)
    CreationTime: datetime,
    DeploymentStatus: str,
    FrameworkStatus: str,
    IdempotencyToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FrameworkControlOutputTypeDef](./type_defs.md#frameworkcontroloutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FrameworkControlTypeDef

```python
# FrameworkControlTypeDef definition

class FrameworkControlTypeDef(TypedDict):
    ControlName: str,
    ControlInputParameters: NotRequired[Sequence[ControlInputParameterTypeDef]],  # (1)
    ControlScope: NotRequired[ControlScopeUnionTypeDef],  # (2)
```

1. See [:material-code-braces: ControlInputParameterTypeDef](./type_defs.md#controlinputparametertypedef) 
2. See [:material-code-braces: ControlScopeTypeDef](./type_defs.md#controlscopetypedef) [:material-code-braces: ControlScopeOutputTypeDef](./type_defs.md#controlscopeoutputtypedef) 
## CreateLegalHoldOutputTypeDef

```python
# CreateLegalHoldOutputTypeDef definition

class CreateLegalHoldOutputTypeDef(TypedDict):
    Title: str,
    Status: LegalHoldStatusType,  # (1)
    Description: str,
    LegalHoldId: str,
    LegalHoldArn: str,
    CreationDate: datetime,
    RecoveryPointSelection: RecoveryPointSelectionOutputTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: LegalHoldStatusType](./literals.md#legalholdstatustype) 
2. See [:material-code-braces: RecoveryPointSelectionOutputTypeDef](./type_defs.md#recoverypointselectionoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLegalHoldOutputTypeDef

```python
# GetLegalHoldOutputTypeDef definition

class GetLegalHoldOutputTypeDef(TypedDict):
    Title: str,
    Status: LegalHoldStatusType,  # (1)
    Description: str,
    CancelDescription: str,
    LegalHoldId: str,
    LegalHoldArn: str,
    CreationDate: datetime,
    CancellationDate: datetime,
    RetainRecordUntil: datetime,
    RecoveryPointSelection: RecoveryPointSelectionOutputTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: LegalHoldStatusType](./literals.md#legalholdstatustype) 
2. See [:material-code-braces: RecoveryPointSelectionOutputTypeDef](./type_defs.md#recoverypointselectionoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRestoreJobsByProtectedResourceOutputTypeDef

```python
# ListRestoreJobsByProtectedResourceOutputTypeDef definition

class ListRestoreJobsByProtectedResourceOutputTypeDef(TypedDict):
    RestoreJobs: List[RestoreJobsListMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RestoreJobsListMemberTypeDef](./type_defs.md#restorejobslistmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRestoreJobsOutputTypeDef

```python
# ListRestoreJobsOutputTypeDef definition

class ListRestoreJobsOutputTypeDef(TypedDict):
    RestoreJobs: List[RestoreJobsListMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RestoreJobsListMemberTypeDef](./type_defs.md#restorejobslistmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BackupRuleInputTypeDef

```python
# BackupRuleInputTypeDef definition

class BackupRuleInputTypeDef(TypedDict):
    RuleName: str,
    TargetBackupVaultName: str,
    ScheduleExpression: NotRequired[str],
    StartWindowMinutes: NotRequired[int],
    CompletionWindowMinutes: NotRequired[int],
    Lifecycle: NotRequired[LifecycleTypeDef],  # (1)
    RecoveryPointTags: NotRequired[Mapping[str, str]],
    CopyActions: NotRequired[Sequence[CopyActionTypeDef]],  # (2)
    EnableContinuousBackup: NotRequired[bool],
    ScheduleExpressionTimezone: NotRequired[str],
    IndexActions: NotRequired[Sequence[IndexActionUnionTypeDef]],  # (3)
```

1. See [:material-code-braces: LifecycleTypeDef](./type_defs.md#lifecycletypedef) 
2. See [:material-code-braces: CopyActionTypeDef](./type_defs.md#copyactiontypedef) 
3. See [:material-code-braces: IndexActionTypeDef](./type_defs.md#indexactiontypedef) [:material-code-braces: IndexActionOutputTypeDef](./type_defs.md#indexactionoutputtypedef) 
## RestoreTestingSelectionForGetTypeDef

```python
# RestoreTestingSelectionForGetTypeDef definition

class RestoreTestingSelectionForGetTypeDef(TypedDict):
    CreationTime: datetime,
    IamRoleArn: str,
    ProtectedResourceType: str,
    RestoreTestingPlanName: str,
    RestoreTestingSelectionName: str,
    CreatorRequestId: NotRequired[str],
    ProtectedResourceArns: NotRequired[List[str]],
    ProtectedResourceConditions: NotRequired[ProtectedResourceConditionsOutputTypeDef],  # (1)
    RestoreMetadataOverrides: NotRequired[Dict[str, str]],
    ValidationWindowHours: NotRequired[int],
```

1. See [:material-code-braces: ProtectedResourceConditionsOutputTypeDef](./type_defs.md#protectedresourceconditionsoutputtypedef) 
## DescribeReportJobOutputTypeDef

```python
# DescribeReportJobOutputTypeDef definition

class DescribeReportJobOutputTypeDef(TypedDict):
    ReportJob: ReportJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReportJobTypeDef](./type_defs.md#reportjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReportJobsOutputTypeDef

```python
# ListReportJobsOutputTypeDef definition

class ListReportJobsOutputTypeDef(TypedDict):
    ReportJobs: List[ReportJobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ReportJobTypeDef](./type_defs.md#reportjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeReportPlanOutputTypeDef

```python
# DescribeReportPlanOutputTypeDef definition

class DescribeReportPlanOutputTypeDef(TypedDict):
    ReportPlan: ReportPlanTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReportPlanTypeDef](./type_defs.md#reportplantypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReportPlansOutputTypeDef

```python
# ListReportPlansOutputTypeDef definition

class ListReportPlansOutputTypeDef(TypedDict):
    ReportPlans: List[ReportPlanTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ReportPlanTypeDef](./type_defs.md#reportplantypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRestoreTestingPlanOutputTypeDef

```python
# GetRestoreTestingPlanOutputTypeDef definition

class GetRestoreTestingPlanOutputTypeDef(TypedDict):
    RestoreTestingPlan: RestoreTestingPlanForGetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RestoreTestingPlanForGetTypeDef](./type_defs.md#restoretestingplanforgettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreTestingPlanForCreateTypeDef

```python
# RestoreTestingPlanForCreateTypeDef definition

class RestoreTestingPlanForCreateTypeDef(TypedDict):
    RecoveryPointSelection: RestoreTestingRecoveryPointSelectionUnionTypeDef,  # (1)
    RestoreTestingPlanName: str,
    ScheduleExpression: str,
    ScheduleExpressionTimezone: NotRequired[str],
    StartWindowHours: NotRequired[int],
```

1. See [:material-code-braces: RestoreTestingRecoveryPointSelectionTypeDef](./type_defs.md#restoretestingrecoverypointselectiontypedef) [:material-code-braces: RestoreTestingRecoveryPointSelectionOutputTypeDef](./type_defs.md#restoretestingrecoverypointselectionoutputtypedef) 
## RestoreTestingPlanForUpdateTypeDef

```python
# RestoreTestingPlanForUpdateTypeDef definition

class RestoreTestingPlanForUpdateTypeDef(TypedDict):
    RecoveryPointSelection: NotRequired[RestoreTestingRecoveryPointSelectionUnionTypeDef],  # (1)
    ScheduleExpression: NotRequired[str],
    ScheduleExpressionTimezone: NotRequired[str],
    StartWindowHours: NotRequired[int],
```

1. See [:material-code-braces: RestoreTestingRecoveryPointSelectionTypeDef](./type_defs.md#restoretestingrecoverypointselectiontypedef) [:material-code-braces: RestoreTestingRecoveryPointSelectionOutputTypeDef](./type_defs.md#restoretestingrecoverypointselectionoutputtypedef) 
## BackupPlanTypeDef

```python
# BackupPlanTypeDef definition

class BackupPlanTypeDef(TypedDict):
    BackupPlanName: str,
    Rules: List[BackupRuleTypeDef],  # (1)
    AdvancedBackupSettings: NotRequired[List[AdvancedBackupSettingOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: BackupRuleTypeDef](./type_defs.md#backupruletypedef) 
2. See [:material-code-braces: AdvancedBackupSettingOutputTypeDef](./type_defs.md#advancedbackupsettingoutputtypedef) 
## GetBackupSelectionOutputTypeDef

```python
# GetBackupSelectionOutputTypeDef definition

class GetBackupSelectionOutputTypeDef(TypedDict):
    BackupSelection: BackupSelectionOutputTypeDef,  # (1)
    SelectionId: str,
    BackupPlanId: str,
    CreationDate: datetime,
    CreatorRequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupSelectionOutputTypeDef](./type_defs.md#backupselectionoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BackupSelectionTypeDef

```python
# BackupSelectionTypeDef definition

class BackupSelectionTypeDef(TypedDict):
    SelectionName: str,
    IamRoleArn: str,
    Resources: NotRequired[Sequence[str]],
    ListOfTags: NotRequired[Sequence[ConditionTypeDef]],  # (1)
    NotResources: NotRequired[Sequence[str]],
    Conditions: NotRequired[ConditionsUnionTypeDef],  # (2)
```

1. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
2. See [:material-code-braces: ConditionsTypeDef](./type_defs.md#conditionstypedef) [:material-code-braces: ConditionsOutputTypeDef](./type_defs.md#conditionsoutputtypedef) 
## UpdateFrameworkInputRequestTypeDef

```python
# UpdateFrameworkInputRequestTypeDef definition

class UpdateFrameworkInputRequestTypeDef(TypedDict):
    FrameworkName: str,
    FrameworkDescription: NotRequired[str],
    FrameworkControls: NotRequired[Sequence[FrameworkControlTypeDef]],  # (1)
    IdempotencyToken: NotRequired[str],
```

1. See [:material-code-braces: FrameworkControlTypeDef](./type_defs.md#frameworkcontroltypedef) 
## RecoveryPointSelectionTypeDef

```python
# RecoveryPointSelectionTypeDef definition

class RecoveryPointSelectionTypeDef(TypedDict):
    VaultNames: NotRequired[Sequence[str]],
    ResourceIdentifiers: NotRequired[Sequence[str]],
    DateRange: NotRequired[DateRangeUnionTypeDef],  # (1)
```

1. See [:material-code-braces: DateRangeTypeDef](./type_defs.md#daterangetypedef) [:material-code-braces: DateRangeOutputTypeDef](./type_defs.md#daterangeoutputtypedef) 
## BackupPlanInputTypeDef

```python
# BackupPlanInputTypeDef definition

class BackupPlanInputTypeDef(TypedDict):
    BackupPlanName: str,
    Rules: Sequence[BackupRuleInputTypeDef],  # (1)
    AdvancedBackupSettings: NotRequired[Sequence[AdvancedBackupSettingUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: BackupRuleInputTypeDef](./type_defs.md#backupruleinputtypedef) 
2. See [:material-code-braces: AdvancedBackupSettingTypeDef](./type_defs.md#advancedbackupsettingtypedef) [:material-code-braces: AdvancedBackupSettingOutputTypeDef](./type_defs.md#advancedbackupsettingoutputtypedef) 
## GetRestoreTestingSelectionOutputTypeDef

```python
# GetRestoreTestingSelectionOutputTypeDef definition

class GetRestoreTestingSelectionOutputTypeDef(TypedDict):
    RestoreTestingSelection: RestoreTestingSelectionForGetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RestoreTestingSelectionForGetTypeDef](./type_defs.md#restoretestingselectionforgettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreTestingSelectionForCreateTypeDef

```python
# RestoreTestingSelectionForCreateTypeDef definition

class RestoreTestingSelectionForCreateTypeDef(TypedDict):
    IamRoleArn: str,
    ProtectedResourceType: str,
    RestoreTestingSelectionName: str,
    ProtectedResourceArns: NotRequired[Sequence[str]],
    ProtectedResourceConditions: NotRequired[ProtectedResourceConditionsUnionTypeDef],  # (1)
    RestoreMetadataOverrides: NotRequired[Mapping[str, str]],
    ValidationWindowHours: NotRequired[int],
```

1. See [:material-code-braces: ProtectedResourceConditionsTypeDef](./type_defs.md#protectedresourceconditionstypedef) [:material-code-braces: ProtectedResourceConditionsOutputTypeDef](./type_defs.md#protectedresourceconditionsoutputtypedef) 
## RestoreTestingSelectionForUpdateTypeDef

```python
# RestoreTestingSelectionForUpdateTypeDef definition

class RestoreTestingSelectionForUpdateTypeDef(TypedDict):
    IamRoleArn: NotRequired[str],
    ProtectedResourceArns: NotRequired[Sequence[str]],
    ProtectedResourceConditions: NotRequired[ProtectedResourceConditionsUnionTypeDef],  # (1)
    RestoreMetadataOverrides: NotRequired[Mapping[str, str]],
    ValidationWindowHours: NotRequired[int],
```

1. See [:material-code-braces: ProtectedResourceConditionsTypeDef](./type_defs.md#protectedresourceconditionstypedef) [:material-code-braces: ProtectedResourceConditionsOutputTypeDef](./type_defs.md#protectedresourceconditionsoutputtypedef) 
## CreateRestoreTestingPlanInputRequestTypeDef

```python
# CreateRestoreTestingPlanInputRequestTypeDef definition

class CreateRestoreTestingPlanInputRequestTypeDef(TypedDict):
    RestoreTestingPlan: RestoreTestingPlanForCreateTypeDef,  # (1)
    CreatorRequestId: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: RestoreTestingPlanForCreateTypeDef](./type_defs.md#restoretestingplanforcreatetypedef) 
## UpdateRestoreTestingPlanInputRequestTypeDef

```python
# UpdateRestoreTestingPlanInputRequestTypeDef definition

class UpdateRestoreTestingPlanInputRequestTypeDef(TypedDict):
    RestoreTestingPlan: RestoreTestingPlanForUpdateTypeDef,  # (1)
    RestoreTestingPlanName: str,
```

1. See [:material-code-braces: RestoreTestingPlanForUpdateTypeDef](./type_defs.md#restoretestingplanforupdatetypedef) 
## GetBackupPlanFromJSONOutputTypeDef

```python
# GetBackupPlanFromJSONOutputTypeDef definition

class GetBackupPlanFromJSONOutputTypeDef(TypedDict):
    BackupPlan: BackupPlanTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupPlanTypeDef](./type_defs.md#backupplantypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBackupPlanFromTemplateOutputTypeDef

```python
# GetBackupPlanFromTemplateOutputTypeDef definition

class GetBackupPlanFromTemplateOutputTypeDef(TypedDict):
    BackupPlanDocument: BackupPlanTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupPlanTypeDef](./type_defs.md#backupplantypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBackupPlanOutputTypeDef

```python
# GetBackupPlanOutputTypeDef definition

class GetBackupPlanOutputTypeDef(TypedDict):
    BackupPlan: BackupPlanTypeDef,  # (1)
    BackupPlanId: str,
    BackupPlanArn: str,
    VersionId: str,
    CreatorRequestId: str,
    CreationDate: datetime,
    DeletionDate: datetime,
    LastExecutionDate: datetime,
    AdvancedBackupSettings: List[AdvancedBackupSettingOutputTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BackupPlanTypeDef](./type_defs.md#backupplantypedef) 
2. See [:material-code-braces: AdvancedBackupSettingOutputTypeDef](./type_defs.md#advancedbackupsettingoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBackupSelectionInputRequestTypeDef

```python
# CreateBackupSelectionInputRequestTypeDef definition

class CreateBackupSelectionInputRequestTypeDef(TypedDict):
    BackupPlanId: str,
    BackupSelection: BackupSelectionTypeDef,  # (1)
    CreatorRequestId: NotRequired[str],
```

1. See [:material-code-braces: BackupSelectionTypeDef](./type_defs.md#backupselectiontypedef) 
## CreateFrameworkInputRequestTypeDef

```python
# CreateFrameworkInputRequestTypeDef definition

class CreateFrameworkInputRequestTypeDef(TypedDict):
    FrameworkName: str,
    FrameworkControls: Sequence[FrameworkControlUnionTypeDef],  # (1)
    FrameworkDescription: NotRequired[str],
    IdempotencyToken: NotRequired[str],
    FrameworkTags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: FrameworkControlTypeDef](./type_defs.md#frameworkcontroltypedef) [:material-code-braces: FrameworkControlOutputTypeDef](./type_defs.md#frameworkcontroloutputtypedef) 
## CreateLegalHoldInputRequestTypeDef

```python
# CreateLegalHoldInputRequestTypeDef definition

class CreateLegalHoldInputRequestTypeDef(TypedDict):
    Title: str,
    Description: str,
    IdempotencyToken: NotRequired[str],
    RecoveryPointSelection: NotRequired[RecoveryPointSelectionTypeDef],  # (1)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: RecoveryPointSelectionTypeDef](./type_defs.md#recoverypointselectiontypedef) 
## CreateBackupPlanInputRequestTypeDef

```python
# CreateBackupPlanInputRequestTypeDef definition

class CreateBackupPlanInputRequestTypeDef(TypedDict):
    BackupPlan: BackupPlanInputTypeDef,  # (1)
    BackupPlanTags: NotRequired[Mapping[str, str]],
    CreatorRequestId: NotRequired[str],
```

1. See [:material-code-braces: BackupPlanInputTypeDef](./type_defs.md#backupplaninputtypedef) 
## UpdateBackupPlanInputRequestTypeDef

```python
# UpdateBackupPlanInputRequestTypeDef definition

class UpdateBackupPlanInputRequestTypeDef(TypedDict):
    BackupPlanId: str,
    BackupPlan: BackupPlanInputTypeDef,  # (1)
```

1. See [:material-code-braces: BackupPlanInputTypeDef](./type_defs.md#backupplaninputtypedef) 
## CreateRestoreTestingSelectionInputRequestTypeDef

```python
# CreateRestoreTestingSelectionInputRequestTypeDef definition

class CreateRestoreTestingSelectionInputRequestTypeDef(TypedDict):
    RestoreTestingPlanName: str,
    RestoreTestingSelection: RestoreTestingSelectionForCreateTypeDef,  # (1)
    CreatorRequestId: NotRequired[str],
```

1. See [:material-code-braces: RestoreTestingSelectionForCreateTypeDef](./type_defs.md#restoretestingselectionforcreatetypedef) 
## UpdateRestoreTestingSelectionInputRequestTypeDef

```python
# UpdateRestoreTestingSelectionInputRequestTypeDef definition

class UpdateRestoreTestingSelectionInputRequestTypeDef(TypedDict):
    RestoreTestingPlanName: str,
    RestoreTestingSelection: RestoreTestingSelectionForUpdateTypeDef,  # (1)
    RestoreTestingSelectionName: str,
```

1. See [:material-code-braces: RestoreTestingSelectionForUpdateTypeDef](./type_defs.md#restoretestingselectionforupdatetypedef) 
