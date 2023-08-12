# Type definitions

> [Index](../README.md) > [Backup](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Backup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
    type annotations stubs module [types-aiobotocore-backup](https://pypi.org/project/types-aiobotocore-backup/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AdvancedBackupSettingTypeDef

```python
# AdvancedBackupSettingTypeDef definition

class AdvancedBackupSettingTypeDef(TypedDict):
    ResourceType: NotRequired[str],
    BackupOptions: NotRequired[Mapping[str, str]],
```

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
    CreationDate: NotRequired[datetime],
    EncryptionKeyArn: NotRequired[str],
    CreatorRequestId: NotRequired[str],
    NumberOfRecoveryPoints: NotRequired[int],
    Locked: NotRequired[bool],
    MinRetentionDays: NotRequired[int],
    MaxRetentionDays: NotRequired[int],
    LockDate: NotRequired[datetime],
```

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

## ControlScopeTypeDef

```python
# ControlScopeTypeDef definition

class ControlScopeTypeDef(TypedDict):
    ComplianceResourceIds: NotRequired[Sequence[str]],
    ComplianceResourceTypes: NotRequired[Sequence[str]],
    Tags: NotRequired[Mapping[str, str]],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
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

## GetRecoveryPointRestoreMetadataInputRequestTypeDef

```python
# GetRecoveryPointRestoreMetadataInputRequestTypeDef definition

class GetRecoveryPointRestoreMetadataInputRequestTypeDef(TypedDict):
    BackupVaultName: str,
    RecoveryPointArn: str,
    BackupVaultAccountId: NotRequired[str],
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
```

1. See [:material-code-brackets: RecoveryPointStatusType](./literals.md#recoverypointstatustype) 
## ListReportPlansInputRequestTypeDef

```python
# ListReportPlansInputRequestTypeDef definition

class ListReportPlansInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

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
```

1. See [:material-code-brackets: RestoreJobStatusType](./literals.md#restorejobstatustype) 
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
## ReportDestinationTypeDef

```python
# ReportDestinationTypeDef definition

class ReportDestinationTypeDef(TypedDict):
    S3BucketName: NotRequired[str],
    S3Keys: NotRequired[List[str]],
```

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
    AdvancedBackupSettings: NotRequired[List[AdvancedBackupSettingTypeDef]],  # (1)
```

1. See [:material-code-braces: AdvancedBackupSettingTypeDef](./type_defs.md#advancedbackupsettingtypedef) 
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
```

1. See [:material-code-braces: LifecycleTypeDef](./type_defs.md#lifecycletypedef) 
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
```

1. See [:material-code-braces: RecoveryPointCreatorTypeDef](./type_defs.md#recoverypointcreatortypedef) 
2. See [:material-code-brackets: RecoveryPointStatusType](./literals.md#recoverypointstatustype) 
3. See [:material-code-braces: CalculatedLifecycleTypeDef](./type_defs.md#calculatedlifecycletypedef) 
4. See [:material-code-braces: LifecycleTypeDef](./type_defs.md#lifecycletypedef) 
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
## FrameworkControlTypeDef

```python
# FrameworkControlTypeDef definition

class FrameworkControlTypeDef(TypedDict):
    ControlName: str,
    ControlInputParameters: NotRequired[Sequence[ControlInputParameterTypeDef]],  # (1)
    ControlScope: NotRequired[ControlScopeTypeDef],  # (2)
```

1. See [:material-code-braces: ControlInputParameterTypeDef](./type_defs.md#controlinputparametertypedef) 
2. See [:material-code-braces: ControlScopeTypeDef](./type_defs.md#controlscopetypedef) 
## CreateBackupPlanOutputTypeDef

```python
# CreateBackupPlanOutputTypeDef definition

class CreateBackupPlanOutputTypeDef(TypedDict):
    BackupPlanId: str,
    BackupPlanArn: str,
    CreationDate: datetime,
    VersionId: str,
    AdvancedBackupSettings: List[AdvancedBackupSettingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AdvancedBackupSettingTypeDef](./type_defs.md#advancedbackupsettingtypedef) 
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
    EncryptionKeyArn: str,
    CreationDate: datetime,
    CreatorRequestId: str,
    NumberOfRecoveryPoints: int,
    Locked: bool,
    MinRetentionDays: int,
    MaxRetentionDays: int,
    LockDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: VaultTypeType](./literals.md#vaulttypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: RecoveryPointCreatorTypeDef](./type_defs.md#recoverypointcreatortypedef) 
2. See [:material-code-brackets: RecoveryPointStatusType](./literals.md#recoverypointstatustype) 
3. See [:material-code-braces: CalculatedLifecycleTypeDef](./type_defs.md#calculatedlifecycletypedef) 
4. See [:material-code-braces: LifecycleTypeDef](./type_defs.md#lifecycletypedef) 
5. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRegionSettingsOutputTypeDef

```python
# DescribeRegionSettingsOutputTypeDef definition

class DescribeRegionSettingsOutputTypeDef(TypedDict):
    ResourceTypeOptInPreference: Dict[str, bool],
    ResourceTypeManagementPreference: Dict[str, bool],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RestoreJobStatusType](./literals.md#restorejobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## GetRecoveryPointRestoreMetadataOutputTypeDef

```python
# GetRecoveryPointRestoreMetadataOutputTypeDef definition

class GetRecoveryPointRestoreMetadataOutputTypeDef(TypedDict):
    BackupVaultArn: str,
    RecoveryPointArn: str,
    RestoreMetadata: Dict[str, str],
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
## ListBackupPlanTemplatesOutputTypeDef

```python
# ListBackupPlanTemplatesOutputTypeDef definition

class ListBackupPlanTemplatesOutputTypeDef(TypedDict):
    NextToken: str,
    BackupPlanTemplatesList: List[BackupPlanTemplatesListMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupPlanTemplatesListMemberTypeDef](./type_defs.md#backupplantemplateslistmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBackupSelectionsOutputTypeDef

```python
# ListBackupSelectionsOutputTypeDef definition

class ListBackupSelectionsOutputTypeDef(TypedDict):
    NextToken: str,
    BackupSelectionsList: List[BackupSelectionsListMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupSelectionsListMemberTypeDef](./type_defs.md#backupselectionslistmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBackupVaultsOutputTypeDef

```python
# ListBackupVaultsOutputTypeDef definition

class ListBackupVaultsOutputTypeDef(TypedDict):
    BackupVaultList: List[BackupVaultListMemberTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupVaultListMemberTypeDef](./type_defs.md#backupvaultlistmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsOutputTypeDef

```python
# ListTagsOutputTypeDef definition

class ListTagsOutputTypeDef(TypedDict):
    NextToken: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
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
    AdvancedBackupSettings: List[AdvancedBackupSettingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AdvancedBackupSettingTypeDef](./type_defs.md#advancedbackupsettingtypedef) 
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
## ReportPlanTypeDef

```python
# ReportPlanTypeDef definition

class ReportPlanTypeDef(TypedDict):
    ReportPlanArn: NotRequired[str],
    ReportPlanName: NotRequired[str],
    ReportPlanDescription: NotRequired[str],
    ReportSetting: NotRequired[ReportSettingTypeDef],  # (1)
    ReportDeliveryChannel: NotRequired[ReportDeliveryChannelTypeDef],  # (2)
    DeploymentStatus: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastAttemptedExecutionTime: NotRequired[datetime],
    LastSuccessfulExecutionTime: NotRequired[datetime],
```

1. See [:material-code-braces: ReportSettingTypeDef](./type_defs.md#reportsettingtypedef) 
2. See [:material-code-braces: ReportDeliveryChannelTypeDef](./type_defs.md#reportdeliverychanneltypedef) 
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
## DateRangeTypeDef

```python
# DateRangeTypeDef definition

class DateRangeTypeDef(TypedDict):
    FromDate: Union[datetime, str],
    ToDate: Union[datetime, str],
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
    ByCreatedBefore: NotRequired[Union[datetime, str]],
    ByCreatedAfter: NotRequired[Union[datetime, str]],
    ByResourceType: NotRequired[str],
    ByAccountId: NotRequired[str],
    ByCompleteAfter: NotRequired[Union[datetime, str]],
    ByCompleteBefore: NotRequired[Union[datetime, str]],
    ByParentJobId: NotRequired[str],
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
    ByCreatedBefore: NotRequired[Union[datetime, str]],
    ByCreatedAfter: NotRequired[Union[datetime, str]],
    ByResourceType: NotRequired[str],
    ByDestinationVaultArn: NotRequired[str],
    ByAccountId: NotRequired[str],
    ByCompleteBefore: NotRequired[Union[datetime, str]],
    ByCompleteAfter: NotRequired[Union[datetime, str]],
    ByParentJobId: NotRequired[str],
```

1. See [:material-code-brackets: CopyJobStateType](./literals.md#copyjobstatetype) 
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
    ByCreatedBefore: NotRequired[Union[datetime, str]],
    ByCreatedAfter: NotRequired[Union[datetime, str]],
    ByParentRecoveryPointArn: NotRequired[str],
```

## ListReportJobsInputRequestTypeDef

```python
# ListReportJobsInputRequestTypeDef definition

class ListReportJobsInputRequestTypeDef(TypedDict):
    ByReportPlanName: NotRequired[str],
    ByCreationBefore: NotRequired[Union[datetime, str]],
    ByCreationAfter: NotRequired[Union[datetime, str]],
    ByStatus: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListRestoreJobsInputRequestTypeDef

```python
# ListRestoreJobsInputRequestTypeDef definition

class ListRestoreJobsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ByAccountId: NotRequired[str],
    ByCreatedBefore: NotRequired[Union[datetime, str]],
    ByCreatedAfter: NotRequired[Union[datetime, str]],
    ByStatus: NotRequired[RestoreJobStatusType],  # (1)
    ByCompleteBefore: NotRequired[Union[datetime, str]],
    ByCompleteAfter: NotRequired[Union[datetime, str]],
```

1. See [:material-code-brackets: RestoreJobStatusType](./literals.md#restorejobstatustype) 
## ListFrameworksOutputTypeDef

```python
# ListFrameworksOutputTypeDef definition

class ListFrameworksOutputTypeDef(TypedDict):
    Frameworks: List[FrameworkTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FrameworkTypeDef](./type_defs.md#frameworktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLegalHoldsOutputTypeDef

```python
# ListLegalHoldsOutputTypeDef definition

class ListLegalHoldsOutputTypeDef(TypedDict):
    NextToken: str,
    LegalHolds: List[LegalHoldTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LegalHoldTypeDef](./type_defs.md#legalholdtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBackupJobsInputListBackupJobsPaginateTypeDef

```python
# ListBackupJobsInputListBackupJobsPaginateTypeDef definition

class ListBackupJobsInputListBackupJobsPaginateTypeDef(TypedDict):
    ByResourceArn: NotRequired[str],
    ByState: NotRequired[BackupJobStateType],  # (1)
    ByBackupVaultName: NotRequired[str],
    ByCreatedBefore: NotRequired[Union[datetime, str]],
    ByCreatedAfter: NotRequired[Union[datetime, str]],
    ByResourceType: NotRequired[str],
    ByAccountId: NotRequired[str],
    ByCompleteAfter: NotRequired[Union[datetime, str]],
    ByCompleteBefore: NotRequired[Union[datetime, str]],
    ByParentJobId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: BackupJobStateType](./literals.md#backupjobstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef

```python
# ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef definition

class ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef

```python
# ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef definition

class ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef(TypedDict):
    BackupPlanId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBackupPlansInputListBackupPlansPaginateTypeDef

```python
# ListBackupPlansInputListBackupPlansPaginateTypeDef definition

class ListBackupPlansInputListBackupPlansPaginateTypeDef(TypedDict):
    IncludeDeleted: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef

```python
# ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef definition

class ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef(TypedDict):
    BackupPlanId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBackupVaultsInputListBackupVaultsPaginateTypeDef

```python
# ListBackupVaultsInputListBackupVaultsPaginateTypeDef definition

class ListBackupVaultsInputListBackupVaultsPaginateTypeDef(TypedDict):
    ByVaultType: NotRequired[VaultTypeType],  # (1)
    ByShared: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: VaultTypeType](./literals.md#vaulttypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCopyJobsInputListCopyJobsPaginateTypeDef

```python
# ListCopyJobsInputListCopyJobsPaginateTypeDef definition

class ListCopyJobsInputListCopyJobsPaginateTypeDef(TypedDict):
    ByResourceArn: NotRequired[str],
    ByState: NotRequired[CopyJobStateType],  # (1)
    ByCreatedBefore: NotRequired[Union[datetime, str]],
    ByCreatedAfter: NotRequired[Union[datetime, str]],
    ByResourceType: NotRequired[str],
    ByDestinationVaultArn: NotRequired[str],
    ByAccountId: NotRequired[str],
    ByCompleteBefore: NotRequired[Union[datetime, str]],
    ByCompleteAfter: NotRequired[Union[datetime, str]],
    ByParentJobId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: CopyJobStateType](./literals.md#copyjobstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLegalHoldsInputListLegalHoldsPaginateTypeDef

```python
# ListLegalHoldsInputListLegalHoldsPaginateTypeDef definition

class ListLegalHoldsInputListLegalHoldsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProtectedResourcesByBackupVaultInputListProtectedResourcesByBackupVaultPaginateTypeDef

```python
# ListProtectedResourcesByBackupVaultInputListProtectedResourcesByBackupVaultPaginateTypeDef definition

class ListProtectedResourcesByBackupVaultInputListProtectedResourcesByBackupVaultPaginateTypeDef(TypedDict):
    BackupVaultName: str,
    BackupVaultAccountId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef

```python
# ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef definition

class ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef

```python
# ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef definition

class ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef(TypedDict):
    BackupVaultName: str,
    BackupVaultAccountId: NotRequired[str],
    ByResourceArn: NotRequired[str],
    ByResourceType: NotRequired[str],
    ByBackupPlanId: NotRequired[str],
    ByCreatedBefore: NotRequired[Union[datetime, str]],
    ByCreatedAfter: NotRequired[Union[datetime, str]],
    ByParentRecoveryPointArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef

```python
# ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef definition

class ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef(TypedDict):
    LegalHoldId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef

```python
# ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef definition

class ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef(TypedDict):
    ResourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRestoreJobsInputListRestoreJobsPaginateTypeDef

```python
# ListRestoreJobsInputListRestoreJobsPaginateTypeDef definition

class ListRestoreJobsInputListRestoreJobsPaginateTypeDef(TypedDict):
    ByAccountId: NotRequired[str],
    ByCreatedBefore: NotRequired[Union[datetime, str]],
    ByCreatedAfter: NotRequired[Union[datetime, str]],
    ByStatus: NotRequired[RestoreJobStatusType],  # (1)
    ByCompleteBefore: NotRequired[Union[datetime, str]],
    ByCompleteAfter: NotRequired[Union[datetime, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: RestoreJobStatusType](./literals.md#restorejobstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProtectedResourcesByBackupVaultOutputTypeDef

```python
# ListProtectedResourcesByBackupVaultOutputTypeDef definition

class ListProtectedResourcesByBackupVaultOutputTypeDef(TypedDict):
    Results: List[ProtectedResourceTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProtectedResourceTypeDef](./type_defs.md#protectedresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProtectedResourcesOutputTypeDef

```python
# ListProtectedResourcesOutputTypeDef definition

class ListProtectedResourcesOutputTypeDef(TypedDict):
    Results: List[ProtectedResourceTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProtectedResourceTypeDef](./type_defs.md#protectedresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRecoveryPointsByLegalHoldOutputTypeDef

```python
# ListRecoveryPointsByLegalHoldOutputTypeDef definition

class ListRecoveryPointsByLegalHoldOutputTypeDef(TypedDict):
    RecoveryPoints: List[RecoveryPointMemberTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecoveryPointMemberTypeDef](./type_defs.md#recoverypointmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRecoveryPointsByResourceOutputTypeDef

```python
# ListRecoveryPointsByResourceOutputTypeDef definition

class ListRecoveryPointsByResourceOutputTypeDef(TypedDict):
    NextToken: str,
    RecoveryPoints: List[RecoveryPointByResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecoveryPointByResourceTypeDef](./type_defs.md#recoverypointbyresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRestoreJobsOutputTypeDef

```python
# ListRestoreJobsOutputTypeDef definition

class ListRestoreJobsOutputTypeDef(TypedDict):
    RestoreJobs: List[RestoreJobsListMemberTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RestoreJobsListMemberTypeDef](./type_defs.md#restorejobslistmembertypedef) 
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
## ListBackupPlanVersionsOutputTypeDef

```python
# ListBackupPlanVersionsOutputTypeDef definition

class ListBackupPlanVersionsOutputTypeDef(TypedDict):
    NextToken: str,
    BackupPlanVersionsList: List[BackupPlansListMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupPlansListMemberTypeDef](./type_defs.md#backupplanslistmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBackupPlansOutputTypeDef

```python
# ListBackupPlansOutputTypeDef definition

class ListBackupPlansOutputTypeDef(TypedDict):
    NextToken: str,
    BackupPlansList: List[BackupPlansListMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupPlansListMemberTypeDef](./type_defs.md#backupplanslistmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBackupJobsOutputTypeDef

```python
# ListBackupJobsOutputTypeDef definition

class ListBackupJobsOutputTypeDef(TypedDict):
    BackupJobs: List[BackupJobTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CopyJobTypeDef](./type_defs.md#copyjobtypedef) 
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
```

1. See [:material-code-braces: LifecycleTypeDef](./type_defs.md#lifecycletypedef) 
2. See [:material-code-braces: CopyActionTypeDef](./type_defs.md#copyactiontypedef) 
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
```

1. See [:material-code-braces: LifecycleTypeDef](./type_defs.md#lifecycletypedef) 
2. See [:material-code-braces: CopyActionTypeDef](./type_defs.md#copyactiontypedef) 
## ListRecoveryPointsByBackupVaultOutputTypeDef

```python
# ListRecoveryPointsByBackupVaultOutputTypeDef definition

class ListRecoveryPointsByBackupVaultOutputTypeDef(TypedDict):
    NextToken: str,
    RecoveryPoints: List[RecoveryPointByBackupVaultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecoveryPointByBackupVaultTypeDef](./type_defs.md#recoverypointbybackupvaulttypedef) 
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
    Conditions: NotRequired[ConditionsTypeDef],  # (2)
```

1. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
2. See [:material-code-braces: ConditionsTypeDef](./type_defs.md#conditionstypedef) 
## CreateFrameworkInputRequestTypeDef

```python
# CreateFrameworkInputRequestTypeDef definition

class CreateFrameworkInputRequestTypeDef(TypedDict):
    FrameworkName: str,
    FrameworkControls: Sequence[FrameworkControlTypeDef],  # (1)
    FrameworkDescription: NotRequired[str],
    IdempotencyToken: NotRequired[str],
    FrameworkTags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: FrameworkControlTypeDef](./type_defs.md#frameworkcontroltypedef) 
## DescribeFrameworkOutputTypeDef

```python
# DescribeFrameworkOutputTypeDef definition

class DescribeFrameworkOutputTypeDef(TypedDict):
    FrameworkName: str,
    FrameworkArn: str,
    FrameworkDescription: str,
    FrameworkControls: List[FrameworkControlTypeDef],  # (1)
    CreationTime: datetime,
    DeploymentStatus: str,
    FrameworkStatus: str,
    IdempotencyToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FrameworkControlTypeDef](./type_defs.md#frameworkcontroltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReportPlanTypeDef](./type_defs.md#reportplantypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RecoveryPointSelectionTypeDef

```python
# RecoveryPointSelectionTypeDef definition

class RecoveryPointSelectionTypeDef(TypedDict):
    VaultNames: NotRequired[Sequence[str]],
    ResourceIdentifiers: NotRequired[Sequence[str]],
    DateRange: NotRequired[DateRangeTypeDef],  # (1)
```

1. See [:material-code-braces: DateRangeTypeDef](./type_defs.md#daterangetypedef) 
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
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReportJobTypeDef](./type_defs.md#reportjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BackupPlanInputTypeDef

```python
# BackupPlanInputTypeDef definition

class BackupPlanInputTypeDef(TypedDict):
    BackupPlanName: str,
    Rules: Sequence[BackupRuleInputTypeDef],  # (1)
    AdvancedBackupSettings: NotRequired[Sequence[AdvancedBackupSettingTypeDef]],  # (2)
```

1. See [:material-code-braces: BackupRuleInputTypeDef](./type_defs.md#backupruleinputtypedef) 
2. See [:material-code-braces: AdvancedBackupSettingTypeDef](./type_defs.md#advancedbackupsettingtypedef) 
## BackupPlanTypeDef

```python
# BackupPlanTypeDef definition

class BackupPlanTypeDef(TypedDict):
    BackupPlanName: str,
    Rules: List[BackupRuleTypeDef],  # (1)
    AdvancedBackupSettings: NotRequired[List[AdvancedBackupSettingTypeDef]],  # (2)
```

1. See [:material-code-braces: BackupRuleTypeDef](./type_defs.md#backupruletypedef) 
2. See [:material-code-braces: AdvancedBackupSettingTypeDef](./type_defs.md#advancedbackupsettingtypedef) 
## CreateBackupSelectionInputRequestTypeDef

```python
# CreateBackupSelectionInputRequestTypeDef definition

class CreateBackupSelectionInputRequestTypeDef(TypedDict):
    BackupPlanId: str,
    BackupSelection: BackupSelectionTypeDef,  # (1)
    CreatorRequestId: NotRequired[str],
```

1. See [:material-code-braces: BackupSelectionTypeDef](./type_defs.md#backupselectiontypedef) 
## GetBackupSelectionOutputTypeDef

```python
# GetBackupSelectionOutputTypeDef definition

class GetBackupSelectionOutputTypeDef(TypedDict):
    BackupSelection: BackupSelectionTypeDef,  # (1)
    SelectionId: str,
    BackupPlanId: str,
    CreationDate: datetime,
    CreatorRequestId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupSelectionTypeDef](./type_defs.md#backupselectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    RecoveryPointSelection: RecoveryPointSelectionTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: LegalHoldStatusType](./literals.md#legalholdstatustype) 
2. See [:material-code-braces: RecoveryPointSelectionTypeDef](./type_defs.md#recoverypointselectiontypedef) 
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
    RecoveryPointSelection: RecoveryPointSelectionTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: LegalHoldStatusType](./literals.md#legalholdstatustype) 
2. See [:material-code-braces: RecoveryPointSelectionTypeDef](./type_defs.md#recoverypointselectiontypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    AdvancedBackupSettings: List[AdvancedBackupSettingTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BackupPlanTypeDef](./type_defs.md#backupplantypedef) 
2. See [:material-code-braces: AdvancedBackupSettingTypeDef](./type_defs.md#advancedbackupsettingtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
