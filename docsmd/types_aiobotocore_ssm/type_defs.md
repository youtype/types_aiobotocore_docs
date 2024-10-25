# Type definitions

> [Index](../README.md) > [SSM](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SSM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
    type annotations stubs module [types-aiobotocore-ssm](https://pypi.org/project/types-aiobotocore-ssm/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## TargetUnionTypeDef

```python
# TargetUnionTypeDef definition

TargetUnionTypeDef = Union[
    TargetTypeDef,  # (1)
    TargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
2. See [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 

## MaintenanceWindowAutomationParametersUnionTypeDef

```python
# MaintenanceWindowAutomationParametersUnionTypeDef definition

MaintenanceWindowAutomationParametersUnionTypeDef = Union[
    MaintenanceWindowAutomationParametersTypeDef,  # (1)
    MaintenanceWindowAutomationParametersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MaintenanceWindowAutomationParametersTypeDef](./type_defs.md#maintenancewindowautomationparameterstypedef) 
2. See [:material-code-braces: MaintenanceWindowAutomationParametersOutputTypeDef](./type_defs.md#maintenancewindowautomationparametersoutputtypedef) 

## MaintenanceWindowTaskParameterValueExpressionUnionTypeDef

```python
# MaintenanceWindowTaskParameterValueExpressionUnionTypeDef definition

MaintenanceWindowTaskParameterValueExpressionUnionTypeDef = Union[
    MaintenanceWindowTaskParameterValueExpressionTypeDef,  # (1)
    MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MaintenanceWindowTaskParameterValueExpressionTypeDef](./type_defs.md#maintenancewindowtaskparametervalueexpressiontypedef) 
2. See [:material-code-braces: MaintenanceWindowTaskParameterValueExpressionOutputTypeDef](./type_defs.md#maintenancewindowtaskparametervalueexpressionoutputtypedef) 

## NotificationConfigUnionTypeDef

```python
# NotificationConfigUnionTypeDef definition

NotificationConfigUnionTypeDef = Union[
    NotificationConfigTypeDef,  # (1)
    NotificationConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NotificationConfigTypeDef](./type_defs.md#notificationconfigtypedef) 
2. See [:material-code-braces: NotificationConfigOutputTypeDef](./type_defs.md#notificationconfigoutputtypedef) 

## PatchFilterUnionTypeDef

```python
# PatchFilterUnionTypeDef definition

PatchFilterUnionTypeDef = Union[
    PatchFilterTypeDef,  # (1)
    PatchFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PatchFilterTypeDef](./type_defs.md#patchfiltertypedef) 
2. See [:material-code-braces: PatchFilterOutputTypeDef](./type_defs.md#patchfilteroutputtypedef) 

## PatchSourceUnionTypeDef

```python
# PatchSourceUnionTypeDef definition

PatchSourceUnionTypeDef = Union[
    PatchSourceTypeDef,  # (1)
    PatchSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PatchSourceTypeDef](./type_defs.md#patchsourcetypedef) 
2. See [:material-code-braces: PatchSourceOutputTypeDef](./type_defs.md#patchsourceoutputtypedef) 

## AlarmConfigurationUnionTypeDef

```python
# AlarmConfigurationUnionTypeDef definition

AlarmConfigurationUnionTypeDef = Union[
    AlarmConfigurationTypeDef,  # (1)
    AlarmConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) 
2. See [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 

## MaintenanceWindowLambdaParametersUnionTypeDef

```python
# MaintenanceWindowLambdaParametersUnionTypeDef definition

MaintenanceWindowLambdaParametersUnionTypeDef = Union[
    MaintenanceWindowLambdaParametersTypeDef,  # (1)
    MaintenanceWindowLambdaParametersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MaintenanceWindowLambdaParametersTypeDef](./type_defs.md#maintenancewindowlambdaparameterstypedef) 
2. See [:material-code-braces: MaintenanceWindowLambdaParametersOutputTypeDef](./type_defs.md#maintenancewindowlambdaparametersoutputtypedef) 

## ResourceDataSyncAwsOrganizationsSourceUnionTypeDef

```python
# ResourceDataSyncAwsOrganizationsSourceUnionTypeDef definition

ResourceDataSyncAwsOrganizationsSourceUnionTypeDef = Union[
    ResourceDataSyncAwsOrganizationsSourceTypeDef,  # (1)
    ResourceDataSyncAwsOrganizationsSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ResourceDataSyncAwsOrganizationsSourceTypeDef](./type_defs.md#resourcedatasyncawsorganizationssourcetypedef) 
2. See [:material-code-braces: ResourceDataSyncAwsOrganizationsSourceOutputTypeDef](./type_defs.md#resourcedatasyncawsorganizationssourceoutputtypedef) 

## MaintenanceWindowRunCommandParametersUnionTypeDef

```python
# MaintenanceWindowRunCommandParametersUnionTypeDef definition

MaintenanceWindowRunCommandParametersUnionTypeDef = Union[
    MaintenanceWindowRunCommandParametersTypeDef,  # (1)
    MaintenanceWindowRunCommandParametersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MaintenanceWindowRunCommandParametersTypeDef](./type_defs.md#maintenancewindowruncommandparameterstypedef) 
2. See [:material-code-braces: MaintenanceWindowRunCommandParametersOutputTypeDef](./type_defs.md#maintenancewindowruncommandparametersoutputtypedef) 

## PatchFilterGroupUnionTypeDef

```python
# PatchFilterGroupUnionTypeDef definition

PatchFilterGroupUnionTypeDef = Union[
    PatchFilterGroupTypeDef,  # (1)
    PatchFilterGroupOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PatchFilterGroupTypeDef](./type_defs.md#patchfiltergrouptypedef) 
2. See [:material-code-braces: PatchFilterGroupOutputTypeDef](./type_defs.md#patchfiltergroupoutputtypedef) 

## TargetLocationUnionTypeDef

```python
# TargetLocationUnionTypeDef definition

TargetLocationUnionTypeDef = Union[
    TargetLocationTypeDef,  # (1)
    TargetLocationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TargetLocationTypeDef](./type_defs.md#targetlocationtypedef) 
2. See [:material-code-braces: TargetLocationOutputTypeDef](./type_defs.md#targetlocationoutputtypedef) 

## PatchRuleUnionTypeDef

```python
# PatchRuleUnionTypeDef definition

PatchRuleUnionTypeDef = Union[
    PatchRuleTypeDef,  # (1)
    PatchRuleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PatchRuleTypeDef](./type_defs.md#patchruletypedef) 
2. See [:material-code-braces: PatchRuleOutputTypeDef](./type_defs.md#patchruleoutputtypedef) 

## CreateAssociationBatchRequestEntryUnionTypeDef

```python
# CreateAssociationBatchRequestEntryUnionTypeDef definition

CreateAssociationBatchRequestEntryUnionTypeDef = Union[
    CreateAssociationBatchRequestEntryTypeDef,  # (1)
    CreateAssociationBatchRequestEntryOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CreateAssociationBatchRequestEntryTypeDef](./type_defs.md#createassociationbatchrequestentrytypedef) 
2. See [:material-code-braces: CreateAssociationBatchRequestEntryOutputTypeDef](./type_defs.md#createassociationbatchrequestentryoutputtypedef) 

## RunbookUnionTypeDef

```python
# RunbookUnionTypeDef definition

RunbookUnionTypeDef = Union[
    RunbookTypeDef,  # (1)
    RunbookOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RunbookTypeDef](./type_defs.md#runbooktypedef) 
2. See [:material-code-braces: RunbookOutputTypeDef](./type_defs.md#runbookoutputtypedef) 

## PatchRuleGroupUnionTypeDef

```python
# PatchRuleGroupUnionTypeDef definition

PatchRuleGroupUnionTypeDef = Union[
    PatchRuleGroupTypeDef,  # (1)
    PatchRuleGroupOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PatchRuleGroupTypeDef](./type_defs.md#patchrulegrouptypedef) 
2. See [:material-code-braces: PatchRuleGroupOutputTypeDef](./type_defs.md#patchrulegroupoutputtypedef) 



## AccountSharingInfoTypeDef

```python
# AccountSharingInfoTypeDef definition

class AccountSharingInfoTypeDef(TypedDict):
    AccountId: NotRequired[str],
    SharedDocumentVersion: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## AlarmTypeDef

```python
# AlarmTypeDef definition

class AlarmTypeDef(TypedDict):
    Name: str,
```

## AlarmStateInformationTypeDef

```python
# AlarmStateInformationTypeDef definition

class AlarmStateInformationTypeDef(TypedDict):
    Name: str,
    State: ExternalAlarmStateType,  # (1)
```

1. See [:material-code-brackets: ExternalAlarmStateType](./literals.md#externalalarmstatetype) 
## AssociateOpsItemRelatedItemRequestRequestTypeDef

```python
# AssociateOpsItemRelatedItemRequestRequestTypeDef definition

class AssociateOpsItemRelatedItemRequestRequestTypeDef(TypedDict):
    OpsItemId: str,
    AssociationType: str,
    ResourceType: str,
    ResourceUri: str,
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

## AssociationOverviewTypeDef

```python
# AssociationOverviewTypeDef definition

class AssociationOverviewTypeDef(TypedDict):
    Status: NotRequired[str],
    DetailedStatus: NotRequired[str],
    AssociationStatusAggregatedCount: NotRequired[Dict[str, int]],
```

## AssociationStatusOutputTypeDef

```python
# AssociationStatusOutputTypeDef definition

class AssociationStatusOutputTypeDef(TypedDict):
    Date: datetime,
    Name: AssociationStatusNameType,  # (1)
    Message: str,
    AdditionalInfo: NotRequired[str],
```

1. See [:material-code-brackets: AssociationStatusNameType](./literals.md#associationstatusnametype) 
## TargetOutputTypeDef

```python
# TargetOutputTypeDef definition

class TargetOutputTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[List[str]],
```

## AssociationExecutionFilterTypeDef

```python
# AssociationExecutionFilterTypeDef definition

class AssociationExecutionFilterTypeDef(TypedDict):
    Key: AssociationExecutionFilterKeyType,  # (1)
    Value: str,
    Type: AssociationFilterOperatorTypeType,  # (2)
```

1. See [:material-code-brackets: AssociationExecutionFilterKeyType](./literals.md#associationexecutionfilterkeytype) 
2. See [:material-code-brackets: AssociationFilterOperatorTypeType](./literals.md#associationfilteroperatortypetype) 
## OutputSourceTypeDef

```python
# OutputSourceTypeDef definition

class OutputSourceTypeDef(TypedDict):
    OutputSourceId: NotRequired[str],
    OutputSourceType: NotRequired[str],
```

## AssociationExecutionTargetsFilterTypeDef

```python
# AssociationExecutionTargetsFilterTypeDef definition

class AssociationExecutionTargetsFilterTypeDef(TypedDict):
    Key: AssociationExecutionTargetsFilterKeyType,  # (1)
    Value: str,
```

1. See [:material-code-brackets: AssociationExecutionTargetsFilterKeyType](./literals.md#associationexecutiontargetsfilterkeytype) 
## AssociationFilterTypeDef

```python
# AssociationFilterTypeDef definition

class AssociationFilterTypeDef(TypedDict):
    key: AssociationFilterKeyType,  # (1)
    value: str,
```

1. See [:material-code-brackets: AssociationFilterKeyType](./literals.md#associationfilterkeytype) 
## AttachmentContentTypeDef

```python
# AttachmentContentTypeDef definition

class AttachmentContentTypeDef(TypedDict):
    Name: NotRequired[str],
    Size: NotRequired[int],
    Hash: NotRequired[str],
    HashType: NotRequired[AttachmentHashTypeType],  # (1)
    Url: NotRequired[str],
```

1. See [:material-code-brackets: AttachmentHashTypeType](./literals.md#attachmenthashtypetype) 
## AttachmentInformationTypeDef

```python
# AttachmentInformationTypeDef definition

class AttachmentInformationTypeDef(TypedDict):
    Name: NotRequired[str],
```

## AttachmentsSourceTypeDef

```python
# AttachmentsSourceTypeDef definition

class AttachmentsSourceTypeDef(TypedDict):
    Key: NotRequired[AttachmentsSourceKeyType],  # (1)
    Values: NotRequired[Sequence[str]],
    Name: NotRequired[str],
```

1. See [:material-code-brackets: AttachmentsSourceKeyType](./literals.md#attachmentssourcekeytype) 
## AutomationExecutionFilterTypeDef

```python
# AutomationExecutionFilterTypeDef definition

class AutomationExecutionFilterTypeDef(TypedDict):
    Key: AutomationExecutionFilterKeyType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: AutomationExecutionFilterKeyType](./literals.md#automationexecutionfilterkeytype) 
## ResolvedTargetsTypeDef

```python
# ResolvedTargetsTypeDef definition

class ResolvedTargetsTypeDef(TypedDict):
    ParameterValues: NotRequired[List[str]],
    Truncated: NotRequired[bool],
```

## ProgressCountersTypeDef

```python
# ProgressCountersTypeDef definition

class ProgressCountersTypeDef(TypedDict):
    TotalSteps: NotRequired[int],
    SuccessSteps: NotRequired[int],
    FailedSteps: NotRequired[int],
    CancelledSteps: NotRequired[int],
    TimedOutSteps: NotRequired[int],
```

## CancelCommandRequestRequestTypeDef

```python
# CancelCommandRequestRequestTypeDef definition

class CancelCommandRequestRequestTypeDef(TypedDict):
    CommandId: str,
    InstanceIds: NotRequired[Sequence[str]],
```

## CancelMaintenanceWindowExecutionRequestRequestTypeDef

```python
# CancelMaintenanceWindowExecutionRequestRequestTypeDef definition

class CancelMaintenanceWindowExecutionRequestRequestTypeDef(TypedDict):
    WindowExecutionId: str,
```

## CloudWatchOutputConfigTypeDef

```python
# CloudWatchOutputConfigTypeDef definition

class CloudWatchOutputConfigTypeDef(TypedDict):
    CloudWatchLogGroupName: NotRequired[str],
    CloudWatchOutputEnabled: NotRequired[bool],
```

## CommandFilterTypeDef

```python
# CommandFilterTypeDef definition

class CommandFilterTypeDef(TypedDict):
    key: CommandFilterKeyType,  # (1)
    value: str,
```

1. See [:material-code-brackets: CommandFilterKeyType](./literals.md#commandfilterkeytype) 
## CommandPluginTypeDef

```python
# CommandPluginTypeDef definition

class CommandPluginTypeDef(TypedDict):
    Name: NotRequired[str],
    Status: NotRequired[CommandPluginStatusType],  # (1)
    StatusDetails: NotRequired[str],
    ResponseCode: NotRequired[int],
    ResponseStartDateTime: NotRequired[datetime],
    ResponseFinishDateTime: NotRequired[datetime],
    Output: NotRequired[str],
    StandardOutputUrl: NotRequired[str],
    StandardErrorUrl: NotRequired[str],
    OutputS3Region: NotRequired[str],
    OutputS3BucketName: NotRequired[str],
    OutputS3KeyPrefix: NotRequired[str],
```

1. See [:material-code-brackets: CommandPluginStatusType](./literals.md#commandpluginstatustype) 
## NotificationConfigOutputTypeDef

```python
# NotificationConfigOutputTypeDef definition

class NotificationConfigOutputTypeDef(TypedDict):
    NotificationArn: NotRequired[str],
    NotificationEvents: NotRequired[List[NotificationEventType]],  # (1)
    NotificationType: NotRequired[NotificationTypeType],  # (2)
```

1. See [:material-code-brackets: NotificationEventType](./literals.md#notificationeventtype) 
2. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
## ComplianceExecutionSummaryOutputTypeDef

```python
# ComplianceExecutionSummaryOutputTypeDef definition

class ComplianceExecutionSummaryOutputTypeDef(TypedDict):
    ExecutionTime: datetime,
    ExecutionId: NotRequired[str],
    ExecutionType: NotRequired[str],
```

## ComplianceItemEntryTypeDef

```python
# ComplianceItemEntryTypeDef definition

class ComplianceItemEntryTypeDef(TypedDict):
    Severity: ComplianceSeverityType,  # (1)
    Status: ComplianceStatusType,  # (2)
    Id: NotRequired[str],
    Title: NotRequired[str],
    Details: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ComplianceSeverityType](./literals.md#complianceseveritytype) 
2. See [:material-code-brackets: ComplianceStatusType](./literals.md#compliancestatustype) 
## ComplianceStringFilterTypeDef

```python
# ComplianceStringFilterTypeDef definition

class ComplianceStringFilterTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[Sequence[str]],
    Type: NotRequired[ComplianceQueryOperatorTypeType],  # (1)
```

1. See [:material-code-brackets: ComplianceQueryOperatorTypeType](./literals.md#compliancequeryoperatortypetype) 
## SeveritySummaryTypeDef

```python
# SeveritySummaryTypeDef definition

class SeveritySummaryTypeDef(TypedDict):
    CriticalCount: NotRequired[int],
    HighCount: NotRequired[int],
    MediumCount: NotRequired[int],
    LowCount: NotRequired[int],
    InformationalCount: NotRequired[int],
    UnspecifiedCount: NotRequired[int],
```

## RegistrationMetadataItemTypeDef

```python
# RegistrationMetadataItemTypeDef definition

class RegistrationMetadataItemTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## DocumentRequiresTypeDef

```python
# DocumentRequiresTypeDef definition

class DocumentRequiresTypeDef(TypedDict):
    Name: str,
    Version: NotRequired[str],
    RequireType: NotRequired[str],
    VersionName: NotRequired[str],
```

## OpsItemDataValueTypeDef

```python
# OpsItemDataValueTypeDef definition

class OpsItemDataValueTypeDef(TypedDict):
    Value: NotRequired[str],
    Type: NotRequired[OpsItemDataTypeType],  # (1)
```

1. See [:material-code-brackets: OpsItemDataTypeType](./literals.md#opsitemdatatypetype) 
## OpsItemNotificationTypeDef

```python
# OpsItemNotificationTypeDef definition

class OpsItemNotificationTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## RelatedOpsItemTypeDef

```python
# RelatedOpsItemTypeDef definition

class RelatedOpsItemTypeDef(TypedDict):
    OpsItemId: str,
```

## MetadataValueTypeDef

```python
# MetadataValueTypeDef definition

class MetadataValueTypeDef(TypedDict):
    Value: NotRequired[str],
```

## DeleteActivationRequestRequestTypeDef

```python
# DeleteActivationRequestRequestTypeDef definition

class DeleteActivationRequestRequestTypeDef(TypedDict):
    ActivationId: str,
```

## DeleteAssociationRequestRequestTypeDef

```python
# DeleteAssociationRequestRequestTypeDef definition

class DeleteAssociationRequestRequestTypeDef(TypedDict):
    Name: NotRequired[str],
    InstanceId: NotRequired[str],
    AssociationId: NotRequired[str],
```

## DeleteDocumentRequestRequestTypeDef

```python
# DeleteDocumentRequestRequestTypeDef definition

class DeleteDocumentRequestRequestTypeDef(TypedDict):
    Name: str,
    DocumentVersion: NotRequired[str],
    VersionName: NotRequired[str],
    Force: NotRequired[bool],
```

## DeleteInventoryRequestRequestTypeDef

```python
# DeleteInventoryRequestRequestTypeDef definition

class DeleteInventoryRequestRequestTypeDef(TypedDict):
    TypeName: str,
    SchemaDeleteOption: NotRequired[InventorySchemaDeleteOptionType],  # (1)
    DryRun: NotRequired[bool],
    ClientToken: NotRequired[str],
```

1. See [:material-code-brackets: InventorySchemaDeleteOptionType](./literals.md#inventoryschemadeleteoptiontype) 
## DeleteMaintenanceWindowRequestRequestTypeDef

```python
# DeleteMaintenanceWindowRequestRequestTypeDef definition

class DeleteMaintenanceWindowRequestRequestTypeDef(TypedDict):
    WindowId: str,
```

## DeleteOpsItemRequestRequestTypeDef

```python
# DeleteOpsItemRequestRequestTypeDef definition

class DeleteOpsItemRequestRequestTypeDef(TypedDict):
    OpsItemId: str,
```

## DeleteOpsMetadataRequestRequestTypeDef

```python
# DeleteOpsMetadataRequestRequestTypeDef definition

class DeleteOpsMetadataRequestRequestTypeDef(TypedDict):
    OpsMetadataArn: str,
```

## DeleteParameterRequestRequestTypeDef

```python
# DeleteParameterRequestRequestTypeDef definition

class DeleteParameterRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteParametersRequestRequestTypeDef

```python
# DeleteParametersRequestRequestTypeDef definition

class DeleteParametersRequestRequestTypeDef(TypedDict):
    Names: Sequence[str],
```

## DeletePatchBaselineRequestRequestTypeDef

```python
# DeletePatchBaselineRequestRequestTypeDef definition

class DeletePatchBaselineRequestRequestTypeDef(TypedDict):
    BaselineId: str,
```

## DeleteResourceDataSyncRequestRequestTypeDef

```python
# DeleteResourceDataSyncRequestRequestTypeDef definition

class DeleteResourceDataSyncRequestRequestTypeDef(TypedDict):
    SyncName: str,
    SyncType: NotRequired[str],
```

## DeleteResourcePolicyRequestRequestTypeDef

```python
# DeleteResourcePolicyRequestRequestTypeDef definition

class DeleteResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    PolicyId: str,
    PolicyHash: str,
```

## DeregisterManagedInstanceRequestRequestTypeDef

```python
# DeregisterManagedInstanceRequestRequestTypeDef definition

class DeregisterManagedInstanceRequestRequestTypeDef(TypedDict):
    InstanceId: str,
```

## DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef

```python
# DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef definition

class DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef(TypedDict):
    BaselineId: str,
    PatchGroup: str,
```

## DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef

```python
# DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef definition

class DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef(TypedDict):
    WindowId: str,
    WindowTargetId: str,
    Safe: NotRequired[bool],
```

## DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef

```python
# DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef definition

class DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef(TypedDict):
    WindowId: str,
    WindowTaskId: str,
```

## DescribeActivationsFilterTypeDef

```python
# DescribeActivationsFilterTypeDef definition

class DescribeActivationsFilterTypeDef(TypedDict):
    FilterKey: NotRequired[DescribeActivationsFilterKeysType],  # (1)
    FilterValues: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: DescribeActivationsFilterKeysType](./literals.md#describeactivationsfilterkeystype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeAssociationRequestRequestTypeDef

```python
# DescribeAssociationRequestRequestTypeDef definition

class DescribeAssociationRequestRequestTypeDef(TypedDict):
    Name: NotRequired[str],
    InstanceId: NotRequired[str],
    AssociationId: NotRequired[str],
    AssociationVersion: NotRequired[str],
```

## StepExecutionFilterTypeDef

```python
# StepExecutionFilterTypeDef definition

class StepExecutionFilterTypeDef(TypedDict):
    Key: StepExecutionFilterKeyType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: StepExecutionFilterKeyType](./literals.md#stepexecutionfilterkeytype) 
## PatchOrchestratorFilterTypeDef

```python
# PatchOrchestratorFilterTypeDef definition

class PatchOrchestratorFilterTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## PatchTypeDef

```python
# PatchTypeDef definition

class PatchTypeDef(TypedDict):
    Id: NotRequired[str],
    ReleaseDate: NotRequired[datetime],
    Title: NotRequired[str],
    Description: NotRequired[str],
    ContentUrl: NotRequired[str],
    Vendor: NotRequired[str],
    ProductFamily: NotRequired[str],
    Product: NotRequired[str],
    Classification: NotRequired[str],
    MsrcSeverity: NotRequired[str],
    KbNumber: NotRequired[str],
    MsrcNumber: NotRequired[str],
    Language: NotRequired[str],
    AdvisoryIds: NotRequired[List[str]],
    BugzillaIds: NotRequired[List[str]],
    CVEIds: NotRequired[List[str]],
    Name: NotRequired[str],
    Epoch: NotRequired[int],
    Version: NotRequired[str],
    Release: NotRequired[str],
    Arch: NotRequired[str],
    Severity: NotRequired[str],
    Repository: NotRequired[str],
```

## DescribeDocumentPermissionRequestRequestTypeDef

```python
# DescribeDocumentPermissionRequestRequestTypeDef definition

class DescribeDocumentPermissionRequestRequestTypeDef(TypedDict):
    Name: str,
    PermissionType: DocumentPermissionTypeType,  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: DocumentPermissionTypeType](./literals.md#documentpermissiontypetype) 
## DescribeDocumentRequestRequestTypeDef

```python
# DescribeDocumentRequestRequestTypeDef definition

class DescribeDocumentRequestRequestTypeDef(TypedDict):
    Name: str,
    DocumentVersion: NotRequired[str],
    VersionName: NotRequired[str],
```

## DescribeEffectiveInstanceAssociationsRequestRequestTypeDef

```python
# DescribeEffectiveInstanceAssociationsRequestRequestTypeDef definition

class DescribeEffectiveInstanceAssociationsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## InstanceAssociationTypeDef

```python
# InstanceAssociationTypeDef definition

class InstanceAssociationTypeDef(TypedDict):
    AssociationId: NotRequired[str],
    InstanceId: NotRequired[str],
    Content: NotRequired[str],
    AssociationVersion: NotRequired[str],
```

## DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef

```python
# DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef definition

class DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef(TypedDict):
    BaselineId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeInstanceAssociationsStatusRequestRequestTypeDef

```python
# DescribeInstanceAssociationsStatusRequestRequestTypeDef definition

class DescribeInstanceAssociationsStatusRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## InstanceInformationFilterTypeDef

```python
# InstanceInformationFilterTypeDef definition

class InstanceInformationFilterTypeDef(TypedDict):
    key: InstanceInformationFilterKeyType,  # (1)
    valueSet: Sequence[str],
```

1. See [:material-code-brackets: InstanceInformationFilterKeyType](./literals.md#instanceinformationfilterkeytype) 
## InstanceInformationStringFilterTypeDef

```python
# InstanceInformationStringFilterTypeDef definition

class InstanceInformationStringFilterTypeDef(TypedDict):
    Key: str,
    Values: Sequence[str],
```

## InstancePatchStateFilterTypeDef

```python
# InstancePatchStateFilterTypeDef definition

class InstancePatchStateFilterTypeDef(TypedDict):
    Key: str,
    Values: Sequence[str],
    Type: InstancePatchStateOperatorTypeType,  # (1)
```

1. See [:material-code-brackets: InstancePatchStateOperatorTypeType](./literals.md#instancepatchstateoperatortypetype) 
## InstancePatchStateTypeDef

```python
# InstancePatchStateTypeDef definition

class InstancePatchStateTypeDef(TypedDict):
    InstanceId: str,
    PatchGroup: str,
    BaselineId: str,
    OperationStartTime: datetime,
    OperationEndTime: datetime,
    Operation: PatchOperationTypeType,  # (1)
    SnapshotId: NotRequired[str],
    InstallOverrideList: NotRequired[str],
    OwnerInformation: NotRequired[str],
    InstalledCount: NotRequired[int],
    InstalledOtherCount: NotRequired[int],
    InstalledPendingRebootCount: NotRequired[int],
    InstalledRejectedCount: NotRequired[int],
    MissingCount: NotRequired[int],
    FailedCount: NotRequired[int],
    UnreportedNotApplicableCount: NotRequired[int],
    NotApplicableCount: NotRequired[int],
    LastNoRebootInstallOperationTime: NotRequired[datetime],
    RebootOption: NotRequired[RebootOptionType],  # (2)
    CriticalNonCompliantCount: NotRequired[int],
    SecurityNonCompliantCount: NotRequired[int],
    OtherNonCompliantCount: NotRequired[int],
```

1. See [:material-code-brackets: PatchOperationTypeType](./literals.md#patchoperationtypetype) 
2. See [:material-code-brackets: RebootOptionType](./literals.md#rebootoptiontype) 
## DescribeInstancePatchStatesRequestRequestTypeDef

```python
# DescribeInstancePatchStatesRequestRequestTypeDef definition

class DescribeInstancePatchStatesRequestRequestTypeDef(TypedDict):
    InstanceIds: Sequence[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## PatchComplianceDataTypeDef

```python
# PatchComplianceDataTypeDef definition

class PatchComplianceDataTypeDef(TypedDict):
    Title: str,
    KBId: str,
    Classification: str,
    Severity: str,
    State: PatchComplianceDataStateType,  # (1)
    InstalledTime: datetime,
    CVEIds: NotRequired[str],
```

1. See [:material-code-brackets: PatchComplianceDataStateType](./literals.md#patchcompliancedatastatetype) 
## InstancePropertyFilterTypeDef

```python
# InstancePropertyFilterTypeDef definition

class InstancePropertyFilterTypeDef(TypedDict):
    key: InstancePropertyFilterKeyType,  # (1)
    valueSet: Sequence[str],
```

1. See [:material-code-brackets: InstancePropertyFilterKeyType](./literals.md#instancepropertyfilterkeytype) 
## InstancePropertyStringFilterTypeDef

```python
# InstancePropertyStringFilterTypeDef definition

class InstancePropertyStringFilterTypeDef(TypedDict):
    Key: str,
    Values: Sequence[str],
    Operator: NotRequired[InstancePropertyFilterOperatorType],  # (1)
```

1. See [:material-code-brackets: InstancePropertyFilterOperatorType](./literals.md#instancepropertyfilteroperatortype) 
## DescribeInventoryDeletionsRequestRequestTypeDef

```python
# DescribeInventoryDeletionsRequestRequestTypeDef definition

class DescribeInventoryDeletionsRequestRequestTypeDef(TypedDict):
    DeletionId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## MaintenanceWindowFilterTypeDef

```python
# MaintenanceWindowFilterTypeDef definition

class MaintenanceWindowFilterTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## MaintenanceWindowExecutionTaskInvocationIdentityTypeDef

```python
# MaintenanceWindowExecutionTaskInvocationIdentityTypeDef definition

class MaintenanceWindowExecutionTaskInvocationIdentityTypeDef(TypedDict):
    WindowExecutionId: NotRequired[str],
    TaskExecutionId: NotRequired[str],
    InvocationId: NotRequired[str],
    ExecutionId: NotRequired[str],
    TaskType: NotRequired[MaintenanceWindowTaskTypeType],  # (1)
    Parameters: NotRequired[str],
    Status: NotRequired[MaintenanceWindowExecutionStatusType],  # (2)
    StatusDetails: NotRequired[str],
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    OwnerInformation: NotRequired[str],
    WindowTargetId: NotRequired[str],
```

1. See [:material-code-brackets: MaintenanceWindowTaskTypeType](./literals.md#maintenancewindowtasktypetype) 
2. See [:material-code-brackets: MaintenanceWindowExecutionStatusType](./literals.md#maintenancewindowexecutionstatustype) 
## MaintenanceWindowExecutionTypeDef

```python
# MaintenanceWindowExecutionTypeDef definition

class MaintenanceWindowExecutionTypeDef(TypedDict):
    WindowId: NotRequired[str],
    WindowExecutionId: NotRequired[str],
    Status: NotRequired[MaintenanceWindowExecutionStatusType],  # (1)
    StatusDetails: NotRequired[str],
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
```

1. See [:material-code-brackets: MaintenanceWindowExecutionStatusType](./literals.md#maintenancewindowexecutionstatustype) 
## TargetTypeDef

```python
# TargetTypeDef definition

class TargetTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## ScheduledWindowExecutionTypeDef

```python
# ScheduledWindowExecutionTypeDef definition

class ScheduledWindowExecutionTypeDef(TypedDict):
    WindowId: NotRequired[str],
    Name: NotRequired[str],
    ExecutionTime: NotRequired[str],
```

## MaintenanceWindowIdentityForTargetTypeDef

```python
# MaintenanceWindowIdentityForTargetTypeDef definition

class MaintenanceWindowIdentityForTargetTypeDef(TypedDict):
    WindowId: NotRequired[str],
    Name: NotRequired[str],
```

## MaintenanceWindowIdentityTypeDef

```python
# MaintenanceWindowIdentityTypeDef definition

class MaintenanceWindowIdentityTypeDef(TypedDict):
    WindowId: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    Enabled: NotRequired[bool],
    Duration: NotRequired[int],
    Cutoff: NotRequired[int],
    Schedule: NotRequired[str],
    ScheduleTimezone: NotRequired[str],
    ScheduleOffset: NotRequired[int],
    EndDate: NotRequired[str],
    StartDate: NotRequired[str],
    NextExecutionTime: NotRequired[str],
```

## OpsItemFilterTypeDef

```python
# OpsItemFilterTypeDef definition

class OpsItemFilterTypeDef(TypedDict):
    Key: OpsItemFilterKeyType,  # (1)
    Values: Sequence[str],
    Operator: OpsItemFilterOperatorType,  # (2)
```

1. See [:material-code-brackets: OpsItemFilterKeyType](./literals.md#opsitemfilterkeytype) 
2. See [:material-code-brackets: OpsItemFilterOperatorType](./literals.md#opsitemfilteroperatortype) 
## ParameterStringFilterTypeDef

```python
# ParameterStringFilterTypeDef definition

class ParameterStringFilterTypeDef(TypedDict):
    Key: str,
    Option: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## ParametersFilterTypeDef

```python
# ParametersFilterTypeDef definition

class ParametersFilterTypeDef(TypedDict):
    Key: ParametersFilterKeyType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: ParametersFilterKeyType](./literals.md#parametersfilterkeytype) 
## PatchBaselineIdentityTypeDef

```python
# PatchBaselineIdentityTypeDef definition

class PatchBaselineIdentityTypeDef(TypedDict):
    BaselineId: NotRequired[str],
    BaselineName: NotRequired[str],
    OperatingSystem: NotRequired[OperatingSystemType],  # (1)
    BaselineDescription: NotRequired[str],
    DefaultBaseline: NotRequired[bool],
```

1. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
## DescribePatchGroupStateRequestRequestTypeDef

```python
# DescribePatchGroupStateRequestRequestTypeDef definition

class DescribePatchGroupStateRequestRequestTypeDef(TypedDict):
    PatchGroup: str,
```

## DescribePatchPropertiesRequestRequestTypeDef

```python
# DescribePatchPropertiesRequestRequestTypeDef definition

class DescribePatchPropertiesRequestRequestTypeDef(TypedDict):
    OperatingSystem: OperatingSystemType,  # (1)
    Property: PatchPropertyType,  # (2)
    PatchSet: NotRequired[PatchSetType],  # (3)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
2. See [:material-code-brackets: PatchPropertyType](./literals.md#patchpropertytype) 
3. See [:material-code-brackets: PatchSetType](./literals.md#patchsettype) 
## SessionFilterTypeDef

```python
# SessionFilterTypeDef definition

class SessionFilterTypeDef(TypedDict):
    key: SessionFilterKeyType,  # (1)
    value: str,
```

1. See [:material-code-brackets: SessionFilterKeyType](./literals.md#sessionfilterkeytype) 
## DisassociateOpsItemRelatedItemRequestRequestTypeDef

```python
# DisassociateOpsItemRelatedItemRequestRequestTypeDef definition

class DisassociateOpsItemRelatedItemRequestRequestTypeDef(TypedDict):
    OpsItemId: str,
    AssociationId: str,
```

## DocumentDefaultVersionDescriptionTypeDef

```python
# DocumentDefaultVersionDescriptionTypeDef definition

class DocumentDefaultVersionDescriptionTypeDef(TypedDict):
    Name: NotRequired[str],
    DefaultVersion: NotRequired[str],
    DefaultVersionName: NotRequired[str],
```

## DocumentParameterTypeDef

```python
# DocumentParameterTypeDef definition

class DocumentParameterTypeDef(TypedDict):
    Name: NotRequired[str],
    Type: NotRequired[DocumentParameterTypeType],  # (1)
    Description: NotRequired[str],
    DefaultValue: NotRequired[str],
```

1. See [:material-code-brackets: DocumentParameterTypeType](./literals.md#documentparametertypetype) 
## ReviewInformationTypeDef

```python
# ReviewInformationTypeDef definition

class ReviewInformationTypeDef(TypedDict):
    ReviewedTime: NotRequired[datetime],
    Status: NotRequired[ReviewStatusType],  # (1)
    Reviewer: NotRequired[str],
```

1. See [:material-code-brackets: ReviewStatusType](./literals.md#reviewstatustype) 
## DocumentFilterTypeDef

```python
# DocumentFilterTypeDef definition

class DocumentFilterTypeDef(TypedDict):
    key: DocumentFilterKeyType,  # (1)
    value: str,
```

1. See [:material-code-brackets: DocumentFilterKeyType](./literals.md#documentfilterkeytype) 
## DocumentKeyValuesFilterTypeDef

```python
# DocumentKeyValuesFilterTypeDef definition

class DocumentKeyValuesFilterTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## DocumentReviewCommentSourceTypeDef

```python
# DocumentReviewCommentSourceTypeDef definition

class DocumentReviewCommentSourceTypeDef(TypedDict):
    Type: NotRequired[DocumentReviewCommentTypeType],  # (1)
    Content: NotRequired[str],
```

1. See [:material-code-brackets: DocumentReviewCommentTypeType](./literals.md#documentreviewcommenttypetype) 
## DocumentVersionInfoTypeDef

```python
# DocumentVersionInfoTypeDef definition

class DocumentVersionInfoTypeDef(TypedDict):
    Name: NotRequired[str],
    DisplayName: NotRequired[str],
    DocumentVersion: NotRequired[str],
    VersionName: NotRequired[str],
    CreatedDate: NotRequired[datetime],
    IsDefaultVersion: NotRequired[bool],
    DocumentFormat: NotRequired[DocumentFormatType],  # (1)
    Status: NotRequired[DocumentStatusType],  # (2)
    StatusInformation: NotRequired[str],
    ReviewStatus: NotRequired[ReviewStatusType],  # (3)
```

1. See [:material-code-brackets: DocumentFormatType](./literals.md#documentformattype) 
2. See [:material-code-brackets: DocumentStatusType](./literals.md#documentstatustype) 
3. See [:material-code-brackets: ReviewStatusType](./literals.md#reviewstatustype) 
## PatchStatusTypeDef

```python
# PatchStatusTypeDef definition

class PatchStatusTypeDef(TypedDict):
    DeploymentStatus: NotRequired[PatchDeploymentStatusType],  # (1)
    ComplianceLevel: NotRequired[PatchComplianceLevelType],  # (2)
    ApprovalDate: NotRequired[datetime],
```

1. See [:material-code-brackets: PatchDeploymentStatusType](./literals.md#patchdeploymentstatustype) 
2. See [:material-code-brackets: PatchComplianceLevelType](./literals.md#patchcomplianceleveltype) 
## FailureDetailsTypeDef

```python
# FailureDetailsTypeDef definition

class FailureDetailsTypeDef(TypedDict):
    FailureStage: NotRequired[str],
    FailureType: NotRequired[str],
    Details: NotRequired[Dict[str, List[str]]],
```

## GetAutomationExecutionRequestRequestTypeDef

```python
# GetAutomationExecutionRequestRequestTypeDef definition

class GetAutomationExecutionRequestRequestTypeDef(TypedDict):
    AutomationExecutionId: str,
```

## GetCalendarStateRequestRequestTypeDef

```python
# GetCalendarStateRequestRequestTypeDef definition

class GetCalendarStateRequestRequestTypeDef(TypedDict):
    CalendarNames: Sequence[str],
    AtTime: NotRequired[str],
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## GetCommandInvocationRequestRequestTypeDef

```python
# GetCommandInvocationRequestRequestTypeDef definition

class GetCommandInvocationRequestRequestTypeDef(TypedDict):
    CommandId: str,
    InstanceId: str,
    PluginName: NotRequired[str],
```

## GetConnectionStatusRequestRequestTypeDef

```python
# GetConnectionStatusRequestRequestTypeDef definition

class GetConnectionStatusRequestRequestTypeDef(TypedDict):
    Target: str,
```

## GetDefaultPatchBaselineRequestRequestTypeDef

```python
# GetDefaultPatchBaselineRequestRequestTypeDef definition

class GetDefaultPatchBaselineRequestRequestTypeDef(TypedDict):
    OperatingSystem: NotRequired[OperatingSystemType],  # (1)
```

1. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
## GetDocumentRequestRequestTypeDef

```python
# GetDocumentRequestRequestTypeDef definition

class GetDocumentRequestRequestTypeDef(TypedDict):
    Name: str,
    VersionName: NotRequired[str],
    DocumentVersion: NotRequired[str],
    DocumentFormat: NotRequired[DocumentFormatType],  # (1)
```

1. See [:material-code-brackets: DocumentFormatType](./literals.md#documentformattype) 
## InventoryFilterTypeDef

```python
# InventoryFilterTypeDef definition

class InventoryFilterTypeDef(TypedDict):
    Key: str,
    Values: Sequence[str],
    Type: NotRequired[InventoryQueryOperatorTypeType],  # (1)
```

1. See [:material-code-brackets: InventoryQueryOperatorTypeType](./literals.md#inventoryqueryoperatortypetype) 
## ResultAttributeTypeDef

```python
# ResultAttributeTypeDef definition

class ResultAttributeTypeDef(TypedDict):
    TypeName: str,
```

## GetInventorySchemaRequestRequestTypeDef

```python
# GetInventorySchemaRequestRequestTypeDef definition

class GetInventorySchemaRequestRequestTypeDef(TypedDict):
    TypeName: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Aggregator: NotRequired[bool],
    SubType: NotRequired[bool],
```

## GetMaintenanceWindowExecutionRequestRequestTypeDef

```python
# GetMaintenanceWindowExecutionRequestRequestTypeDef definition

class GetMaintenanceWindowExecutionRequestRequestTypeDef(TypedDict):
    WindowExecutionId: str,
```

## GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef

```python
# GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef definition

class GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef(TypedDict):
    WindowExecutionId: str,
    TaskId: str,
    InvocationId: str,
```

## GetMaintenanceWindowExecutionTaskRequestRequestTypeDef

```python
# GetMaintenanceWindowExecutionTaskRequestRequestTypeDef definition

class GetMaintenanceWindowExecutionTaskRequestRequestTypeDef(TypedDict):
    WindowExecutionId: str,
    TaskId: str,
```

## MaintenanceWindowTaskParameterValueExpressionOutputTypeDef

```python
# MaintenanceWindowTaskParameterValueExpressionOutputTypeDef definition

class MaintenanceWindowTaskParameterValueExpressionOutputTypeDef(TypedDict):
    Values: NotRequired[List[str]],
```

## GetMaintenanceWindowRequestRequestTypeDef

```python
# GetMaintenanceWindowRequestRequestTypeDef definition

class GetMaintenanceWindowRequestRequestTypeDef(TypedDict):
    WindowId: str,
```

## GetMaintenanceWindowTaskRequestRequestTypeDef

```python
# GetMaintenanceWindowTaskRequestRequestTypeDef definition

class GetMaintenanceWindowTaskRequestRequestTypeDef(TypedDict):
    WindowId: str,
    WindowTaskId: str,
```

## LoggingInfoTypeDef

```python
# LoggingInfoTypeDef definition

class LoggingInfoTypeDef(TypedDict):
    S3BucketName: str,
    S3Region: str,
    S3KeyPrefix: NotRequired[str],
```

## GetOpsItemRequestRequestTypeDef

```python
# GetOpsItemRequestRequestTypeDef definition

class GetOpsItemRequestRequestTypeDef(TypedDict):
    OpsItemId: str,
    OpsItemArn: NotRequired[str],
```

## GetOpsMetadataRequestRequestTypeDef

```python
# GetOpsMetadataRequestRequestTypeDef definition

class GetOpsMetadataRequestRequestTypeDef(TypedDict):
    OpsMetadataArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## OpsFilterTypeDef

```python
# OpsFilterTypeDef definition

class OpsFilterTypeDef(TypedDict):
    Key: str,
    Values: Sequence[str],
    Type: NotRequired[OpsFilterOperatorTypeType],  # (1)
```

1. See [:material-code-brackets: OpsFilterOperatorTypeType](./literals.md#opsfilteroperatortypetype) 
## OpsResultAttributeTypeDef

```python
# OpsResultAttributeTypeDef definition

class OpsResultAttributeTypeDef(TypedDict):
    TypeName: str,
```

## GetParameterHistoryRequestRequestTypeDef

```python
# GetParameterHistoryRequestRequestTypeDef definition

class GetParameterHistoryRequestRequestTypeDef(TypedDict):
    Name: str,
    WithDecryption: NotRequired[bool],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetParameterRequestRequestTypeDef

```python
# GetParameterRequestRequestTypeDef definition

class GetParameterRequestRequestTypeDef(TypedDict):
    Name: str,
    WithDecryption: NotRequired[bool],
```

## ParameterTypeDef

```python
# ParameterTypeDef definition

class ParameterTypeDef(TypedDict):
    Name: NotRequired[str],
    Type: NotRequired[ParameterTypeType],  # (1)
    Value: NotRequired[str],
    Version: NotRequired[int],
    Selector: NotRequired[str],
    SourceResult: NotRequired[str],
    LastModifiedDate: NotRequired[datetime],
    ARN: NotRequired[str],
    DataType: NotRequired[str],
```

1. See [:material-code-brackets: ParameterTypeType](./literals.md#parametertypetype) 
## GetParametersRequestRequestTypeDef

```python
# GetParametersRequestRequestTypeDef definition

class GetParametersRequestRequestTypeDef(TypedDict):
    Names: Sequence[str],
    WithDecryption: NotRequired[bool],
```

## GetPatchBaselineForPatchGroupRequestRequestTypeDef

```python
# GetPatchBaselineForPatchGroupRequestRequestTypeDef definition

class GetPatchBaselineForPatchGroupRequestRequestTypeDef(TypedDict):
    PatchGroup: str,
    OperatingSystem: NotRequired[OperatingSystemType],  # (1)
```

1. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
## GetPatchBaselineRequestRequestTypeDef

```python
# GetPatchBaselineRequestRequestTypeDef definition

class GetPatchBaselineRequestRequestTypeDef(TypedDict):
    BaselineId: str,
```

## PatchSourceOutputTypeDef

```python
# PatchSourceOutputTypeDef definition

class PatchSourceOutputTypeDef(TypedDict):
    Name: str,
    Products: List[str],
    Configuration: str,
```

## GetResourcePoliciesRequestRequestTypeDef

```python
# GetResourcePoliciesRequestRequestTypeDef definition

class GetResourcePoliciesRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetResourcePoliciesResponseEntryTypeDef

```python
# GetResourcePoliciesResponseEntryTypeDef definition

class GetResourcePoliciesResponseEntryTypeDef(TypedDict):
    PolicyId: NotRequired[str],
    PolicyHash: NotRequired[str],
    Policy: NotRequired[str],
```

## GetServiceSettingRequestRequestTypeDef

```python
# GetServiceSettingRequestRequestTypeDef definition

class GetServiceSettingRequestRequestTypeDef(TypedDict):
    SettingId: str,
```

## ServiceSettingTypeDef

```python
# ServiceSettingTypeDef definition

class ServiceSettingTypeDef(TypedDict):
    SettingId: NotRequired[str],
    SettingValue: NotRequired[str],
    LastModifiedDate: NotRequired[datetime],
    LastModifiedUser: NotRequired[str],
    ARN: NotRequired[str],
    Status: NotRequired[str],
```

## InstanceAggregatedAssociationOverviewTypeDef

```python
# InstanceAggregatedAssociationOverviewTypeDef definition

class InstanceAggregatedAssociationOverviewTypeDef(TypedDict):
    DetailedStatus: NotRequired[str],
    InstanceAssociationStatusAggregatedCount: NotRequired[Dict[str, int]],
```

## S3OutputLocationTypeDef

```python
# S3OutputLocationTypeDef definition

class S3OutputLocationTypeDef(TypedDict):
    OutputS3Region: NotRequired[str],
    OutputS3BucketName: NotRequired[str],
    OutputS3KeyPrefix: NotRequired[str],
```

## S3OutputUrlTypeDef

```python
# S3OutputUrlTypeDef definition

class S3OutputUrlTypeDef(TypedDict):
    OutputUrl: NotRequired[str],
```

## InventoryDeletionSummaryItemTypeDef

```python
# InventoryDeletionSummaryItemTypeDef definition

class InventoryDeletionSummaryItemTypeDef(TypedDict):
    Version: NotRequired[str],
    Count: NotRequired[int],
    RemainingCount: NotRequired[int],
```

## InventoryItemAttributeTypeDef

```python
# InventoryItemAttributeTypeDef definition

class InventoryItemAttributeTypeDef(TypedDict):
    Name: str,
    DataType: InventoryAttributeDataTypeType,  # (1)
```

1. See [:material-code-brackets: InventoryAttributeDataTypeType](./literals.md#inventoryattributedatatypetype) 
## InventoryItemTypeDef

```python
# InventoryItemTypeDef definition

class InventoryItemTypeDef(TypedDict):
    TypeName: str,
    SchemaVersion: str,
    CaptureTime: str,
    ContentHash: NotRequired[str],
    Content: NotRequired[Sequence[Mapping[str, str]]],
    Context: NotRequired[Mapping[str, str]],
```

## InventoryResultItemTypeDef

```python
# InventoryResultItemTypeDef definition

class InventoryResultItemTypeDef(TypedDict):
    TypeName: str,
    SchemaVersion: str,
    Content: List[Dict[str, str]],
    CaptureTime: NotRequired[str],
    ContentHash: NotRequired[str],
```

## LabelParameterVersionRequestRequestTypeDef

```python
# LabelParameterVersionRequestRequestTypeDef definition

class LabelParameterVersionRequestRequestTypeDef(TypedDict):
    Name: str,
    Labels: Sequence[str],
    ParameterVersion: NotRequired[int],
```

## ListAssociationVersionsRequestRequestTypeDef

```python
# ListAssociationVersionsRequestRequestTypeDef definition

class ListAssociationVersionsRequestRequestTypeDef(TypedDict):
    AssociationId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListDocumentMetadataHistoryRequestRequestTypeDef

```python
# ListDocumentMetadataHistoryRequestRequestTypeDef definition

class ListDocumentMetadataHistoryRequestRequestTypeDef(TypedDict):
    Name: str,
    Metadata: DocumentMetadataEnumType,  # (1)
    DocumentVersion: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: DocumentMetadataEnumType](./literals.md#documentmetadataenumtype) 
## ListDocumentVersionsRequestRequestTypeDef

```python
# ListDocumentVersionsRequestRequestTypeDef definition

class ListDocumentVersionsRequestRequestTypeDef(TypedDict):
    Name: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## OpsItemEventFilterTypeDef

```python
# OpsItemEventFilterTypeDef definition

class OpsItemEventFilterTypeDef(TypedDict):
    Key: OpsItemEventFilterKeyType,  # (1)
    Values: Sequence[str],
    Operator: OpsItemEventFilterOperatorType,  # (2)
```

1. See [:material-code-brackets: OpsItemEventFilterKeyType](./literals.md#opsitemeventfilterkeytype) 
2. See [:material-code-brackets: OpsItemEventFilterOperatorType](./literals.md#opsitemeventfilteroperatortype) 
## OpsItemRelatedItemsFilterTypeDef

```python
# OpsItemRelatedItemsFilterTypeDef definition

class OpsItemRelatedItemsFilterTypeDef(TypedDict):
    Key: OpsItemRelatedItemsFilterKeyType,  # (1)
    Values: Sequence[str],
    Operator: OpsItemRelatedItemsFilterOperatorType,  # (2)
```

1. See [:material-code-brackets: OpsItemRelatedItemsFilterKeyType](./literals.md#opsitemrelateditemsfilterkeytype) 
2. See [:material-code-brackets: OpsItemRelatedItemsFilterOperatorType](./literals.md#opsitemrelateditemsfilteroperatortype) 
## OpsMetadataFilterTypeDef

```python
# OpsMetadataFilterTypeDef definition

class OpsMetadataFilterTypeDef(TypedDict):
    Key: str,
    Values: Sequence[str],
```

## OpsMetadataTypeDef

```python
# OpsMetadataTypeDef definition

class OpsMetadataTypeDef(TypedDict):
    ResourceId: NotRequired[str],
    OpsMetadataArn: NotRequired[str],
    LastModifiedDate: NotRequired[datetime],
    LastModifiedUser: NotRequired[str],
    CreationDate: NotRequired[datetime],
```

## ListResourceDataSyncRequestRequestTypeDef

```python
# ListResourceDataSyncRequestRequestTypeDef definition

class ListResourceDataSyncRequestRequestTypeDef(TypedDict):
    SyncType: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceType: ResourceTypeForTaggingType,  # (1)
    ResourceId: str,
```

1. See [:material-code-brackets: ResourceTypeForTaggingType](./literals.md#resourcetypefortaggingtype) 
## MaintenanceWindowAutomationParametersOutputTypeDef

```python
# MaintenanceWindowAutomationParametersOutputTypeDef definition

class MaintenanceWindowAutomationParametersOutputTypeDef(TypedDict):
    DocumentVersion: NotRequired[str],
    Parameters: NotRequired[Dict[str, List[str]]],
```

## MaintenanceWindowAutomationParametersTypeDef

```python
# MaintenanceWindowAutomationParametersTypeDef definition

class MaintenanceWindowAutomationParametersTypeDef(TypedDict):
    DocumentVersion: NotRequired[str],
    Parameters: NotRequired[Mapping[str, Sequence[str]]],
```

## MaintenanceWindowLambdaParametersOutputTypeDef

```python
# MaintenanceWindowLambdaParametersOutputTypeDef definition

class MaintenanceWindowLambdaParametersOutputTypeDef(TypedDict):
    ClientContext: NotRequired[str],
    Qualifier: NotRequired[str],
    Payload: NotRequired[bytes],
```

## MaintenanceWindowStepFunctionsParametersTypeDef

```python
# MaintenanceWindowStepFunctionsParametersTypeDef definition

class MaintenanceWindowStepFunctionsParametersTypeDef(TypedDict):
    Input: NotRequired[str],
    Name: NotRequired[str],
```

## MaintenanceWindowTaskParameterValueExpressionTypeDef

```python
# MaintenanceWindowTaskParameterValueExpressionTypeDef definition

class MaintenanceWindowTaskParameterValueExpressionTypeDef(TypedDict):
    Values: NotRequired[Sequence[str]],
```

## ModifyDocumentPermissionRequestRequestTypeDef

```python
# ModifyDocumentPermissionRequestRequestTypeDef definition

class ModifyDocumentPermissionRequestRequestTypeDef(TypedDict):
    Name: str,
    PermissionType: DocumentPermissionTypeType,  # (1)
    AccountIdsToAdd: NotRequired[Sequence[str]],
    AccountIdsToRemove: NotRequired[Sequence[str]],
    SharedDocumentVersion: NotRequired[str],
```

1. See [:material-code-brackets: DocumentPermissionTypeType](./literals.md#documentpermissiontypetype) 
## NotificationConfigTypeDef

```python
# NotificationConfigTypeDef definition

class NotificationConfigTypeDef(TypedDict):
    NotificationArn: NotRequired[str],
    NotificationEvents: NotRequired[Sequence[NotificationEventType]],  # (1)
    NotificationType: NotRequired[NotificationTypeType],  # (2)
```

1. See [:material-code-brackets: NotificationEventType](./literals.md#notificationeventtype) 
2. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
## OpsEntityItemTypeDef

```python
# OpsEntityItemTypeDef definition

class OpsEntityItemTypeDef(TypedDict):
    CaptureTime: NotRequired[str],
    Content: NotRequired[List[Dict[str, str]]],
```

## OpsItemIdentityTypeDef

```python
# OpsItemIdentityTypeDef definition

class OpsItemIdentityTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## ParameterInlinePolicyTypeDef

```python
# ParameterInlinePolicyTypeDef definition

class ParameterInlinePolicyTypeDef(TypedDict):
    PolicyText: NotRequired[str],
    PolicyType: NotRequired[str],
    PolicyStatus: NotRequired[str],
```

## ParentStepDetailsTypeDef

```python
# ParentStepDetailsTypeDef definition

class ParentStepDetailsTypeDef(TypedDict):
    StepExecutionId: NotRequired[str],
    StepName: NotRequired[str],
    Action: NotRequired[str],
    Iteration: NotRequired[int],
    IteratorValue: NotRequired[str],
```

## PatchFilterOutputTypeDef

```python
# PatchFilterOutputTypeDef definition

class PatchFilterOutputTypeDef(TypedDict):
    Key: PatchFilterKeyType,  # (1)
    Values: List[str],
```

1. See [:material-code-brackets: PatchFilterKeyType](./literals.md#patchfilterkeytype) 
## PatchFilterTypeDef

```python
# PatchFilterTypeDef definition

class PatchFilterTypeDef(TypedDict):
    Key: PatchFilterKeyType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: PatchFilterKeyType](./literals.md#patchfilterkeytype) 
## PatchSourceTypeDef

```python
# PatchSourceTypeDef definition

class PatchSourceTypeDef(TypedDict):
    Name: str,
    Products: Sequence[str],
    Configuration: str,
```

## PutResourcePolicyRequestRequestTypeDef

```python
# PutResourcePolicyRequestRequestTypeDef definition

class PutResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Policy: str,
    PolicyId: NotRequired[str],
    PolicyHash: NotRequired[str],
```

## RegisterDefaultPatchBaselineRequestRequestTypeDef

```python
# RegisterDefaultPatchBaselineRequestRequestTypeDef definition

class RegisterDefaultPatchBaselineRequestRequestTypeDef(TypedDict):
    BaselineId: str,
```

## RegisterPatchBaselineForPatchGroupRequestRequestTypeDef

```python
# RegisterPatchBaselineForPatchGroupRequestRequestTypeDef definition

class RegisterPatchBaselineForPatchGroupRequestRequestTypeDef(TypedDict):
    BaselineId: str,
    PatchGroup: str,
```

## RemoveTagsFromResourceRequestRequestTypeDef

```python
# RemoveTagsFromResourceRequestRequestTypeDef definition

class RemoveTagsFromResourceRequestRequestTypeDef(TypedDict):
    ResourceType: ResourceTypeForTaggingType,  # (1)
    ResourceId: str,
    TagKeys: Sequence[str],
```

1. See [:material-code-brackets: ResourceTypeForTaggingType](./literals.md#resourcetypefortaggingtype) 
## ResetServiceSettingRequestRequestTypeDef

```python
# ResetServiceSettingRequestRequestTypeDef definition

class ResetServiceSettingRequestRequestTypeDef(TypedDict):
    SettingId: str,
```

## ResourceDataSyncOrganizationalUnitTypeDef

```python
# ResourceDataSyncOrganizationalUnitTypeDef definition

class ResourceDataSyncOrganizationalUnitTypeDef(TypedDict):
    OrganizationalUnitId: NotRequired[str],
```

## ResourceDataSyncDestinationDataSharingTypeDef

```python
# ResourceDataSyncDestinationDataSharingTypeDef definition

class ResourceDataSyncDestinationDataSharingTypeDef(TypedDict):
    DestinationDataSharingType: NotRequired[str],
```

## ResumeSessionRequestRequestTypeDef

```python
# ResumeSessionRequestRequestTypeDef definition

class ResumeSessionRequestRequestTypeDef(TypedDict):
    SessionId: str,
```

## SendAutomationSignalRequestRequestTypeDef

```python
# SendAutomationSignalRequestRequestTypeDef definition

class SendAutomationSignalRequestRequestTypeDef(TypedDict):
    AutomationExecutionId: str,
    SignalType: SignalTypeType,  # (1)
    Payload: NotRequired[Mapping[str, Sequence[str]]],
```

1. See [:material-code-brackets: SignalTypeType](./literals.md#signaltypetype) 
## SessionManagerOutputUrlTypeDef

```python
# SessionManagerOutputUrlTypeDef definition

class SessionManagerOutputUrlTypeDef(TypedDict):
    S3OutputUrl: NotRequired[str],
    CloudWatchOutputUrl: NotRequired[str],
```

## StartAssociationsOnceRequestRequestTypeDef

```python
# StartAssociationsOnceRequestRequestTypeDef definition

class StartAssociationsOnceRequestRequestTypeDef(TypedDict):
    AssociationIds: Sequence[str],
```

## StartSessionRequestRequestTypeDef

```python
# StartSessionRequestRequestTypeDef definition

class StartSessionRequestRequestTypeDef(TypedDict):
    Target: str,
    DocumentName: NotRequired[str],
    Reason: NotRequired[str],
    Parameters: NotRequired[Mapping[str, Sequence[str]]],
```

## StopAutomationExecutionRequestRequestTypeDef

```python
# StopAutomationExecutionRequestRequestTypeDef definition

class StopAutomationExecutionRequestRequestTypeDef(TypedDict):
    AutomationExecutionId: str,
    Type: NotRequired[StopTypeType],  # (1)
```

1. See [:material-code-brackets: StopTypeType](./literals.md#stoptypetype) 
## TerminateSessionRequestRequestTypeDef

```python
# TerminateSessionRequestRequestTypeDef definition

class TerminateSessionRequestRequestTypeDef(TypedDict):
    SessionId: str,
```

## UnlabelParameterVersionRequestRequestTypeDef

```python
# UnlabelParameterVersionRequestRequestTypeDef definition

class UnlabelParameterVersionRequestRequestTypeDef(TypedDict):
    Name: str,
    ParameterVersion: int,
    Labels: Sequence[str],
```

## UpdateDocumentDefaultVersionRequestRequestTypeDef

```python
# UpdateDocumentDefaultVersionRequestRequestTypeDef definition

class UpdateDocumentDefaultVersionRequestRequestTypeDef(TypedDict):
    Name: str,
    DocumentVersion: str,
```

## UpdateMaintenanceWindowRequestRequestTypeDef

```python
# UpdateMaintenanceWindowRequestRequestTypeDef definition

class UpdateMaintenanceWindowRequestRequestTypeDef(TypedDict):
    WindowId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    StartDate: NotRequired[str],
    EndDate: NotRequired[str],
    Schedule: NotRequired[str],
    ScheduleTimezone: NotRequired[str],
    ScheduleOffset: NotRequired[int],
    Duration: NotRequired[int],
    Cutoff: NotRequired[int],
    AllowUnassociatedTargets: NotRequired[bool],
    Enabled: NotRequired[bool],
    Replace: NotRequired[bool],
```

## UpdateManagedInstanceRoleRequestRequestTypeDef

```python
# UpdateManagedInstanceRoleRequestRequestTypeDef definition

class UpdateManagedInstanceRoleRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    IamRole: str,
```

## UpdateServiceSettingRequestRequestTypeDef

```python
# UpdateServiceSettingRequestRequestTypeDef definition

class UpdateServiceSettingRequestRequestTypeDef(TypedDict):
    SettingId: str,
    SettingValue: str,
```

## ActivationTypeDef

```python
# ActivationTypeDef definition

class ActivationTypeDef(TypedDict):
    ActivationId: NotRequired[str],
    Description: NotRequired[str],
    DefaultInstanceName: NotRequired[str],
    IamRole: NotRequired[str],
    RegistrationLimit: NotRequired[int],
    RegistrationsCount: NotRequired[int],
    ExpirationDate: NotRequired[datetime],
    Expired: NotRequired[bool],
    CreatedDate: NotRequired[datetime],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## AddTagsToResourceRequestRequestTypeDef

```python
# AddTagsToResourceRequestRequestTypeDef definition

class AddTagsToResourceRequestRequestTypeDef(TypedDict):
    ResourceType: ResourceTypeForTaggingType,  # (1)
    ResourceId: str,
    Tags: Sequence[TagTypeDef],  # (2)
```

1. See [:material-code-brackets: ResourceTypeForTaggingType](./literals.md#resourcetypefortaggingtype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateMaintenanceWindowRequestRequestTypeDef

```python
# CreateMaintenanceWindowRequestRequestTypeDef definition

class CreateMaintenanceWindowRequestRequestTypeDef(TypedDict):
    Name: str,
    Schedule: str,
    Duration: int,
    Cutoff: int,
    AllowUnassociatedTargets: bool,
    Description: NotRequired[str],
    StartDate: NotRequired[str],
    EndDate: NotRequired[str],
    ScheduleTimezone: NotRequired[str],
    ScheduleOffset: NotRequired[int],
    ClientToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PutParameterRequestRequestTypeDef

```python
# PutParameterRequestRequestTypeDef definition

class PutParameterRequestRequestTypeDef(TypedDict):
    Name: str,
    Value: str,
    Description: NotRequired[str],
    Type: NotRequired[ParameterTypeType],  # (1)
    KeyId: NotRequired[str],
    Overwrite: NotRequired[bool],
    AllowedPattern: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    Tier: NotRequired[ParameterTierType],  # (3)
    Policies: NotRequired[str],
    DataType: NotRequired[str],
```

1. See [:material-code-brackets: ParameterTypeType](./literals.md#parametertypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: ParameterTierType](./literals.md#parametertiertype) 
## AlarmConfigurationOutputTypeDef

```python
# AlarmConfigurationOutputTypeDef definition

class AlarmConfigurationOutputTypeDef(TypedDict):
    Alarms: List[AlarmTypeDef],  # (1)
    IgnorePollAlarmFailure: NotRequired[bool],
```

1. See [:material-code-braces: AlarmTypeDef](./type_defs.md#alarmtypedef) 
## AlarmConfigurationTypeDef

```python
# AlarmConfigurationTypeDef definition

class AlarmConfigurationTypeDef(TypedDict):
    Alarms: Sequence[AlarmTypeDef],  # (1)
    IgnorePollAlarmFailure: NotRequired[bool],
```

1. See [:material-code-braces: AlarmTypeDef](./type_defs.md#alarmtypedef) 
## AssociateOpsItemRelatedItemResponseTypeDef

```python
# AssociateOpsItemRelatedItemResponseTypeDef definition

class AssociateOpsItemRelatedItemResponseTypeDef(TypedDict):
    AssociationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelMaintenanceWindowExecutionResultTypeDef

```python
# CancelMaintenanceWindowExecutionResultTypeDef definition

class CancelMaintenanceWindowExecutionResultTypeDef(TypedDict):
    WindowExecutionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateActivationResultTypeDef

```python
# CreateActivationResultTypeDef definition

class CreateActivationResultTypeDef(TypedDict):
    ActivationId: str,
    ActivationCode: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMaintenanceWindowResultTypeDef

```python
# CreateMaintenanceWindowResultTypeDef definition

class CreateMaintenanceWindowResultTypeDef(TypedDict):
    WindowId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateOpsItemResponseTypeDef

```python
# CreateOpsItemResponseTypeDef definition

class CreateOpsItemResponseTypeDef(TypedDict):
    OpsItemId: str,
    OpsItemArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateOpsMetadataResultTypeDef

```python
# CreateOpsMetadataResultTypeDef definition

class CreateOpsMetadataResultTypeDef(TypedDict):
    OpsMetadataArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePatchBaselineResultTypeDef

```python
# CreatePatchBaselineResultTypeDef definition

class CreatePatchBaselineResultTypeDef(TypedDict):
    BaselineId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteMaintenanceWindowResultTypeDef

```python
# DeleteMaintenanceWindowResultTypeDef definition

class DeleteMaintenanceWindowResultTypeDef(TypedDict):
    WindowId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteParametersResultTypeDef

```python
# DeleteParametersResultTypeDef definition

class DeleteParametersResultTypeDef(TypedDict):
    DeletedParameters: List[str],
    InvalidParameters: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePatchBaselineResultTypeDef

```python
# DeletePatchBaselineResultTypeDef definition

class DeletePatchBaselineResultTypeDef(TypedDict):
    BaselineId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeregisterPatchBaselineForPatchGroupResultTypeDef

```python
# DeregisterPatchBaselineForPatchGroupResultTypeDef definition

class DeregisterPatchBaselineForPatchGroupResultTypeDef(TypedDict):
    BaselineId: str,
    PatchGroup: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeregisterTargetFromMaintenanceWindowResultTypeDef

```python
# DeregisterTargetFromMaintenanceWindowResultTypeDef definition

class DeregisterTargetFromMaintenanceWindowResultTypeDef(TypedDict):
    WindowId: str,
    WindowTargetId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeregisterTaskFromMaintenanceWindowResultTypeDef

```python
# DeregisterTaskFromMaintenanceWindowResultTypeDef definition

class DeregisterTaskFromMaintenanceWindowResultTypeDef(TypedDict):
    WindowId: str,
    WindowTaskId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDocumentPermissionResponseTypeDef

```python
# DescribeDocumentPermissionResponseTypeDef definition

class DescribeDocumentPermissionResponseTypeDef(TypedDict):
    AccountIds: List[str],
    AccountSharingInfoList: List[AccountSharingInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AccountSharingInfoTypeDef](./type_defs.md#accountsharinginfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePatchGroupStateResultTypeDef

```python
# DescribePatchGroupStateResultTypeDef definition

class DescribePatchGroupStateResultTypeDef(TypedDict):
    Instances: int,
    InstancesWithInstalledPatches: int,
    InstancesWithInstalledOtherPatches: int,
    InstancesWithInstalledPendingRebootPatches: int,
    InstancesWithInstalledRejectedPatches: int,
    InstancesWithMissingPatches: int,
    InstancesWithFailedPatches: int,
    InstancesWithNotApplicablePatches: int,
    InstancesWithUnreportedNotApplicablePatches: int,
    InstancesWithCriticalNonCompliantPatches: int,
    InstancesWithSecurityNonCompliantPatches: int,
    InstancesWithOtherNonCompliantPatches: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePatchPropertiesResultTypeDef

```python
# DescribePatchPropertiesResultTypeDef definition

class DescribePatchPropertiesResultTypeDef(TypedDict):
    Properties: List[Dict[str, str]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCalendarStateResponseTypeDef

```python
# GetCalendarStateResponseTypeDef definition

class GetCalendarStateResponseTypeDef(TypedDict):
    State: CalendarStateType,  # (1)
    AtTime: str,
    NextTransitionTime: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: CalendarStateType](./literals.md#calendarstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConnectionStatusResponseTypeDef

```python
# GetConnectionStatusResponseTypeDef definition

class GetConnectionStatusResponseTypeDef(TypedDict):
    Target: str,
    Status: ConnectionStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ConnectionStatusType](./literals.md#connectionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDefaultPatchBaselineResultTypeDef

```python
# GetDefaultPatchBaselineResultTypeDef definition

class GetDefaultPatchBaselineResultTypeDef(TypedDict):
    BaselineId: str,
    OperatingSystem: OperatingSystemType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeployablePatchSnapshotForInstanceResultTypeDef

```python
# GetDeployablePatchSnapshotForInstanceResultTypeDef definition

class GetDeployablePatchSnapshotForInstanceResultTypeDef(TypedDict):
    InstanceId: str,
    SnapshotId: str,
    SnapshotDownloadUrl: str,
    Product: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMaintenanceWindowExecutionResultTypeDef

```python
# GetMaintenanceWindowExecutionResultTypeDef definition

class GetMaintenanceWindowExecutionResultTypeDef(TypedDict):
    WindowExecutionId: str,
    TaskIds: List[str],
    Status: MaintenanceWindowExecutionStatusType,  # (1)
    StatusDetails: str,
    StartTime: datetime,
    EndTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: MaintenanceWindowExecutionStatusType](./literals.md#maintenancewindowexecutionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMaintenanceWindowExecutionTaskInvocationResultTypeDef

```python
# GetMaintenanceWindowExecutionTaskInvocationResultTypeDef definition

class GetMaintenanceWindowExecutionTaskInvocationResultTypeDef(TypedDict):
    WindowExecutionId: str,
    TaskExecutionId: str,
    InvocationId: str,
    ExecutionId: str,
    TaskType: MaintenanceWindowTaskTypeType,  # (1)
    Parameters: str,
    Status: MaintenanceWindowExecutionStatusType,  # (2)
    StatusDetails: str,
    StartTime: datetime,
    EndTime: datetime,
    OwnerInformation: str,
    WindowTargetId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: MaintenanceWindowTaskTypeType](./literals.md#maintenancewindowtasktypetype) 
2. See [:material-code-brackets: MaintenanceWindowExecutionStatusType](./literals.md#maintenancewindowexecutionstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMaintenanceWindowResultTypeDef

```python
# GetMaintenanceWindowResultTypeDef definition

class GetMaintenanceWindowResultTypeDef(TypedDict):
    WindowId: str,
    Name: str,
    Description: str,
    StartDate: str,
    EndDate: str,
    Schedule: str,
    ScheduleTimezone: str,
    ScheduleOffset: int,
    NextExecutionTime: str,
    Duration: int,
    Cutoff: int,
    AllowUnassociatedTargets: bool,
    Enabled: bool,
    CreatedDate: datetime,
    ModifiedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPatchBaselineForPatchGroupResultTypeDef

```python
# GetPatchBaselineForPatchGroupResultTypeDef definition

class GetPatchBaselineForPatchGroupResultTypeDef(TypedDict):
    BaselineId: str,
    PatchGroup: str,
    OperatingSystem: OperatingSystemType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LabelParameterVersionResultTypeDef

```python
# LabelParameterVersionResultTypeDef definition

class LabelParameterVersionResultTypeDef(TypedDict):
    InvalidLabels: List[str],
    ParameterVersion: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInventoryEntriesResultTypeDef

```python
# ListInventoryEntriesResultTypeDef definition

class ListInventoryEntriesResultTypeDef(TypedDict):
    TypeName: str,
    InstanceId: str,
    SchemaVersion: str,
    CaptureTime: str,
    Entries: List[Dict[str, str]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResultTypeDef

```python
# ListTagsForResourceResultTypeDef definition

class ListTagsForResourceResultTypeDef(TypedDict):
    TagList: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutInventoryResultTypeDef

```python
# PutInventoryResultTypeDef definition

class PutInventoryResultTypeDef(TypedDict):
    Message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutParameterResultTypeDef

```python
# PutParameterResultTypeDef definition

class PutParameterResultTypeDef(TypedDict):
    Version: int,
    Tier: ParameterTierType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ParameterTierType](./literals.md#parametertiertype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResourcePolicyResponseTypeDef

```python
# PutResourcePolicyResponseTypeDef definition

class PutResourcePolicyResponseTypeDef(TypedDict):
    PolicyId: str,
    PolicyHash: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterDefaultPatchBaselineResultTypeDef

```python
# RegisterDefaultPatchBaselineResultTypeDef definition

class RegisterDefaultPatchBaselineResultTypeDef(TypedDict):
    BaselineId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterPatchBaselineForPatchGroupResultTypeDef

```python
# RegisterPatchBaselineForPatchGroupResultTypeDef definition

class RegisterPatchBaselineForPatchGroupResultTypeDef(TypedDict):
    BaselineId: str,
    PatchGroup: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterTargetWithMaintenanceWindowResultTypeDef

```python
# RegisterTargetWithMaintenanceWindowResultTypeDef definition

class RegisterTargetWithMaintenanceWindowResultTypeDef(TypedDict):
    WindowTargetId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterTaskWithMaintenanceWindowResultTypeDef

```python
# RegisterTaskWithMaintenanceWindowResultTypeDef definition

class RegisterTaskWithMaintenanceWindowResultTypeDef(TypedDict):
    WindowTaskId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResumeSessionResponseTypeDef

```python
# ResumeSessionResponseTypeDef definition

class ResumeSessionResponseTypeDef(TypedDict):
    SessionId: str,
    TokenValue: str,
    StreamUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartAutomationExecutionResultTypeDef

```python
# StartAutomationExecutionResultTypeDef definition

class StartAutomationExecutionResultTypeDef(TypedDict):
    AutomationExecutionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartChangeRequestExecutionResultTypeDef

```python
# StartChangeRequestExecutionResultTypeDef definition

class StartChangeRequestExecutionResultTypeDef(TypedDict):
    AutomationExecutionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSessionResponseTypeDef

```python
# StartSessionResponseTypeDef definition

class StartSessionResponseTypeDef(TypedDict):
    SessionId: str,
    TokenValue: str,
    StreamUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TerminateSessionResponseTypeDef

```python
# TerminateSessionResponseTypeDef definition

class TerminateSessionResponseTypeDef(TypedDict):
    SessionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UnlabelParameterVersionResultTypeDef

```python
# UnlabelParameterVersionResultTypeDef definition

class UnlabelParameterVersionResultTypeDef(TypedDict):
    RemovedLabels: List[str],
    InvalidLabels: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMaintenanceWindowResultTypeDef

```python
# UpdateMaintenanceWindowResultTypeDef definition

class UpdateMaintenanceWindowResultTypeDef(TypedDict):
    WindowId: str,
    Name: str,
    Description: str,
    StartDate: str,
    EndDate: str,
    Schedule: str,
    ScheduleTimezone: str,
    ScheduleOffset: int,
    Duration: int,
    Cutoff: int,
    AllowUnassociatedTargets: bool,
    Enabled: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateOpsMetadataResultTypeDef

```python
# UpdateOpsMetadataResultTypeDef definition

class UpdateOpsMetadataResultTypeDef(TypedDict):
    OpsMetadataArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociationTypeDef

```python
# AssociationTypeDef definition

class AssociationTypeDef(TypedDict):
    Name: NotRequired[str],
    InstanceId: NotRequired[str],
    AssociationId: NotRequired[str],
    AssociationVersion: NotRequired[str],
    DocumentVersion: NotRequired[str],
    Targets: NotRequired[List[TargetOutputTypeDef]],  # (1)
    LastExecutionDate: NotRequired[datetime],
    Overview: NotRequired[AssociationOverviewTypeDef],  # (2)
    ScheduleExpression: NotRequired[str],
    AssociationName: NotRequired[str],
    ScheduleOffset: NotRequired[int],
    Duration: NotRequired[int],
    TargetMaps: NotRequired[List[Dict[str, List[str]]]],
```

1. See [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-braces: AssociationOverviewTypeDef](./type_defs.md#associationoverviewtypedef) 
## MaintenanceWindowTargetTypeDef

```python
# MaintenanceWindowTargetTypeDef definition

class MaintenanceWindowTargetTypeDef(TypedDict):
    WindowId: NotRequired[str],
    WindowTargetId: NotRequired[str],
    ResourceType: NotRequired[MaintenanceWindowResourceTypeType],  # (1)
    Targets: NotRequired[List[TargetOutputTypeDef]],  # (2)
    OwnerInformation: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
```

1. See [:material-code-brackets: MaintenanceWindowResourceTypeType](./literals.md#maintenancewindowresourcetypetype) 
2. See [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
## UpdateMaintenanceWindowTargetResultTypeDef

```python
# UpdateMaintenanceWindowTargetResultTypeDef definition

class UpdateMaintenanceWindowTargetResultTypeDef(TypedDict):
    WindowId: str,
    WindowTargetId: str,
    Targets: List[TargetOutputTypeDef],  # (1)
    OwnerInformation: str,
    Name: str,
    Description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAssociationExecutionsRequestRequestTypeDef

```python
# DescribeAssociationExecutionsRequestRequestTypeDef definition

class DescribeAssociationExecutionsRequestRequestTypeDef(TypedDict):
    AssociationId: str,
    Filters: NotRequired[Sequence[AssociationExecutionFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AssociationExecutionFilterTypeDef](./type_defs.md#associationexecutionfiltertypedef) 
## AssociationExecutionTargetTypeDef

```python
# AssociationExecutionTargetTypeDef definition

class AssociationExecutionTargetTypeDef(TypedDict):
    AssociationId: NotRequired[str],
    AssociationVersion: NotRequired[str],
    ExecutionId: NotRequired[str],
    ResourceId: NotRequired[str],
    ResourceType: NotRequired[str],
    Status: NotRequired[str],
    DetailedStatus: NotRequired[str],
    LastExecutionDate: NotRequired[datetime],
    OutputSource: NotRequired[OutputSourceTypeDef],  # (1)
```

1. See [:material-code-braces: OutputSourceTypeDef](./type_defs.md#outputsourcetypedef) 
## DescribeAssociationExecutionTargetsRequestRequestTypeDef

```python
# DescribeAssociationExecutionTargetsRequestRequestTypeDef definition

class DescribeAssociationExecutionTargetsRequestRequestTypeDef(TypedDict):
    AssociationId: str,
    ExecutionId: str,
    Filters: NotRequired[Sequence[AssociationExecutionTargetsFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AssociationExecutionTargetsFilterTypeDef](./type_defs.md#associationexecutiontargetsfiltertypedef) 
## ListAssociationsRequestRequestTypeDef

```python
# ListAssociationsRequestRequestTypeDef definition

class ListAssociationsRequestRequestTypeDef(TypedDict):
    AssociationFilterList: NotRequired[Sequence[AssociationFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AssociationFilterTypeDef](./type_defs.md#associationfiltertypedef) 
## AssociationStatusTypeDef

```python
# AssociationStatusTypeDef definition

class AssociationStatusTypeDef(TypedDict):
    Date: TimestampTypeDef,
    Name: AssociationStatusNameType,  # (1)
    Message: str,
    AdditionalInfo: NotRequired[str],
```

1. See [:material-code-brackets: AssociationStatusNameType](./literals.md#associationstatusnametype) 
## ComplianceExecutionSummaryTypeDef

```python
# ComplianceExecutionSummaryTypeDef definition

class ComplianceExecutionSummaryTypeDef(TypedDict):
    ExecutionTime: TimestampTypeDef,
    ExecutionId: NotRequired[str],
    ExecutionType: NotRequired[str],
```

## UpdateDocumentRequestRequestTypeDef

```python
# UpdateDocumentRequestRequestTypeDef definition

class UpdateDocumentRequestRequestTypeDef(TypedDict):
    Content: str,
    Name: str,
    Attachments: NotRequired[Sequence[AttachmentsSourceTypeDef]],  # (1)
    DisplayName: NotRequired[str],
    VersionName: NotRequired[str],
    DocumentVersion: NotRequired[str],
    DocumentFormat: NotRequired[DocumentFormatType],  # (2)
    TargetType: NotRequired[str],
```

1. See [:material-code-braces: AttachmentsSourceTypeDef](./type_defs.md#attachmentssourcetypedef) 
2. See [:material-code-brackets: DocumentFormatType](./literals.md#documentformattype) 
## DescribeAutomationExecutionsRequestRequestTypeDef

```python
# DescribeAutomationExecutionsRequestRequestTypeDef definition

class DescribeAutomationExecutionsRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[AutomationExecutionFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AutomationExecutionFilterTypeDef](./type_defs.md#automationexecutionfiltertypedef) 
## MaintenanceWindowLambdaParametersTypeDef

```python
# MaintenanceWindowLambdaParametersTypeDef definition

class MaintenanceWindowLambdaParametersTypeDef(TypedDict):
    ClientContext: NotRequired[str],
    Qualifier: NotRequired[str],
    Payload: NotRequired[BlobTypeDef],
```

## GetCommandInvocationResultTypeDef

```python
# GetCommandInvocationResultTypeDef definition

class GetCommandInvocationResultTypeDef(TypedDict):
    CommandId: str,
    InstanceId: str,
    Comment: str,
    DocumentName: str,
    DocumentVersion: str,
    PluginName: str,
    ResponseCode: int,
    ExecutionStartDateTime: str,
    ExecutionElapsedTime: str,
    ExecutionEndDateTime: str,
    Status: CommandInvocationStatusType,  # (1)
    StatusDetails: str,
    StandardOutputContent: str,
    StandardOutputUrl: str,
    StandardErrorContent: str,
    StandardErrorUrl: str,
    CloudWatchOutputConfig: CloudWatchOutputConfigTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: CommandInvocationStatusType](./literals.md#commandinvocationstatustype) 
2. See [:material-code-braces: CloudWatchOutputConfigTypeDef](./type_defs.md#cloudwatchoutputconfigtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCommandInvocationsRequestRequestTypeDef

```python
# ListCommandInvocationsRequestRequestTypeDef definition

class ListCommandInvocationsRequestRequestTypeDef(TypedDict):
    CommandId: NotRequired[str],
    InstanceId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[CommandFilterTypeDef]],  # (1)
    Details: NotRequired[bool],
```

1. See [:material-code-braces: CommandFilterTypeDef](./type_defs.md#commandfiltertypedef) 
## ListCommandsRequestRequestTypeDef

```python
# ListCommandsRequestRequestTypeDef definition

class ListCommandsRequestRequestTypeDef(TypedDict):
    CommandId: NotRequired[str],
    InstanceId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[CommandFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: CommandFilterTypeDef](./type_defs.md#commandfiltertypedef) 
## CommandInvocationTypeDef

```python
# CommandInvocationTypeDef definition

class CommandInvocationTypeDef(TypedDict):
    CommandId: NotRequired[str],
    InstanceId: NotRequired[str],
    InstanceName: NotRequired[str],
    Comment: NotRequired[str],
    DocumentName: NotRequired[str],
    DocumentVersion: NotRequired[str],
    RequestedDateTime: NotRequired[datetime],
    Status: NotRequired[CommandInvocationStatusType],  # (1)
    StatusDetails: NotRequired[str],
    TraceOutput: NotRequired[str],
    StandardOutputUrl: NotRequired[str],
    StandardErrorUrl: NotRequired[str],
    CommandPlugins: NotRequired[List[CommandPluginTypeDef]],  # (2)
    ServiceRole: NotRequired[str],
    NotificationConfig: NotRequired[NotificationConfigOutputTypeDef],  # (3)
    CloudWatchOutputConfig: NotRequired[CloudWatchOutputConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: CommandInvocationStatusType](./literals.md#commandinvocationstatustype) 
2. See [:material-code-braces: CommandPluginTypeDef](./type_defs.md#commandplugintypedef) 
3. See [:material-code-braces: NotificationConfigOutputTypeDef](./type_defs.md#notificationconfigoutputtypedef) 
4. See [:material-code-braces: CloudWatchOutputConfigTypeDef](./type_defs.md#cloudwatchoutputconfigtypedef) 
## MaintenanceWindowRunCommandParametersOutputTypeDef

```python
# MaintenanceWindowRunCommandParametersOutputTypeDef definition

class MaintenanceWindowRunCommandParametersOutputTypeDef(TypedDict):
    Comment: NotRequired[str],
    CloudWatchOutputConfig: NotRequired[CloudWatchOutputConfigTypeDef],  # (1)
    DocumentHash: NotRequired[str],
    DocumentHashType: NotRequired[DocumentHashTypeType],  # (2)
    DocumentVersion: NotRequired[str],
    NotificationConfig: NotRequired[NotificationConfigOutputTypeDef],  # (3)
    OutputS3BucketName: NotRequired[str],
    OutputS3KeyPrefix: NotRequired[str],
    Parameters: NotRequired[Dict[str, List[str]]],
    ServiceRoleArn: NotRequired[str],
    TimeoutSeconds: NotRequired[int],
```

1. See [:material-code-braces: CloudWatchOutputConfigTypeDef](./type_defs.md#cloudwatchoutputconfigtypedef) 
2. See [:material-code-brackets: DocumentHashTypeType](./literals.md#documenthashtypetype) 
3. See [:material-code-braces: NotificationConfigOutputTypeDef](./type_defs.md#notificationconfigoutputtypedef) 
## ComplianceItemTypeDef

```python
# ComplianceItemTypeDef definition

class ComplianceItemTypeDef(TypedDict):
    ComplianceType: NotRequired[str],
    ResourceType: NotRequired[str],
    ResourceId: NotRequired[str],
    Id: NotRequired[str],
    Title: NotRequired[str],
    Status: NotRequired[ComplianceStatusType],  # (1)
    Severity: NotRequired[ComplianceSeverityType],  # (2)
    ExecutionSummary: NotRequired[ComplianceExecutionSummaryOutputTypeDef],  # (3)
    Details: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ComplianceStatusType](./literals.md#compliancestatustype) 
2. See [:material-code-brackets: ComplianceSeverityType](./literals.md#complianceseveritytype) 
3. See [:material-code-braces: ComplianceExecutionSummaryOutputTypeDef](./type_defs.md#complianceexecutionsummaryoutputtypedef) 
## ListComplianceItemsRequestRequestTypeDef

```python
# ListComplianceItemsRequestRequestTypeDef definition

class ListComplianceItemsRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ComplianceStringFilterTypeDef]],  # (1)
    ResourceIds: NotRequired[Sequence[str]],
    ResourceTypes: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ComplianceStringFilterTypeDef](./type_defs.md#compliancestringfiltertypedef) 
## ListComplianceSummariesRequestRequestTypeDef

```python
# ListComplianceSummariesRequestRequestTypeDef definition

class ListComplianceSummariesRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ComplianceStringFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ComplianceStringFilterTypeDef](./type_defs.md#compliancestringfiltertypedef) 
## ListResourceComplianceSummariesRequestRequestTypeDef

```python
# ListResourceComplianceSummariesRequestRequestTypeDef definition

class ListResourceComplianceSummariesRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ComplianceStringFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ComplianceStringFilterTypeDef](./type_defs.md#compliancestringfiltertypedef) 
## CompliantSummaryTypeDef

```python
# CompliantSummaryTypeDef definition

class CompliantSummaryTypeDef(TypedDict):
    CompliantCount: NotRequired[int],
    SeveritySummary: NotRequired[SeveritySummaryTypeDef],  # (1)
```

1. See [:material-code-braces: SeveritySummaryTypeDef](./type_defs.md#severitysummarytypedef) 
## NonCompliantSummaryTypeDef

```python
# NonCompliantSummaryTypeDef definition

class NonCompliantSummaryTypeDef(TypedDict):
    NonCompliantCount: NotRequired[int],
    SeveritySummary: NotRequired[SeveritySummaryTypeDef],  # (1)
```

1. See [:material-code-braces: SeveritySummaryTypeDef](./type_defs.md#severitysummarytypedef) 
## CreateActivationRequestRequestTypeDef

```python
# CreateActivationRequestRequestTypeDef definition

class CreateActivationRequestRequestTypeDef(TypedDict):
    IamRole: str,
    Description: NotRequired[str],
    DefaultInstanceName: NotRequired[str],
    RegistrationLimit: NotRequired[int],
    ExpirationDate: NotRequired[TimestampTypeDef],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    RegistrationMetadata: NotRequired[Sequence[RegistrationMetadataItemTypeDef]],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: RegistrationMetadataItemTypeDef](./type_defs.md#registrationmetadataitemtypedef) 
## CreateDocumentRequestRequestTypeDef

```python
# CreateDocumentRequestRequestTypeDef definition

class CreateDocumentRequestRequestTypeDef(TypedDict):
    Content: str,
    Name: str,
    Requires: NotRequired[Sequence[DocumentRequiresTypeDef]],  # (1)
    Attachments: NotRequired[Sequence[AttachmentsSourceTypeDef]],  # (2)
    DisplayName: NotRequired[str],
    VersionName: NotRequired[str],
    DocumentType: NotRequired[DocumentTypeType],  # (3)
    DocumentFormat: NotRequired[DocumentFormatType],  # (4)
    TargetType: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (5)
```

1. See [:material-code-braces: DocumentRequiresTypeDef](./type_defs.md#documentrequirestypedef) 
2. See [:material-code-braces: AttachmentsSourceTypeDef](./type_defs.md#attachmentssourcetypedef) 
3. See [:material-code-brackets: DocumentTypeType](./literals.md#documenttypetype) 
4. See [:material-code-brackets: DocumentFormatType](./literals.md#documentformattype) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DocumentIdentifierTypeDef

```python
# DocumentIdentifierTypeDef definition

class DocumentIdentifierTypeDef(TypedDict):
    Name: NotRequired[str],
    CreatedDate: NotRequired[datetime],
    DisplayName: NotRequired[str],
    Owner: NotRequired[str],
    VersionName: NotRequired[str],
    PlatformTypes: NotRequired[List[PlatformTypeType]],  # (1)
    DocumentVersion: NotRequired[str],
    DocumentType: NotRequired[DocumentTypeType],  # (2)
    SchemaVersion: NotRequired[str],
    DocumentFormat: NotRequired[DocumentFormatType],  # (3)
    TargetType: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (4)
    Requires: NotRequired[List[DocumentRequiresTypeDef]],  # (5)
    ReviewStatus: NotRequired[ReviewStatusType],  # (6)
    Author: NotRequired[str],
```

1. See [:material-code-brackets: PlatformTypeType](./literals.md#platformtypetype) 
2. See [:material-code-brackets: DocumentTypeType](./literals.md#documenttypetype) 
3. See [:material-code-brackets: DocumentFormatType](./literals.md#documentformattype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: DocumentRequiresTypeDef](./type_defs.md#documentrequirestypedef) 
6. See [:material-code-brackets: ReviewStatusType](./literals.md#reviewstatustype) 
## GetDocumentResultTypeDef

```python
# GetDocumentResultTypeDef definition

class GetDocumentResultTypeDef(TypedDict):
    Name: str,
    CreatedDate: datetime,
    DisplayName: str,
    VersionName: str,
    DocumentVersion: str,
    Status: DocumentStatusType,  # (1)
    StatusInformation: str,
    Content: str,
    DocumentType: DocumentTypeType,  # (2)
    DocumentFormat: DocumentFormatType,  # (3)
    Requires: List[DocumentRequiresTypeDef],  # (4)
    AttachmentsContent: List[AttachmentContentTypeDef],  # (5)
    ReviewStatus: ReviewStatusType,  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: DocumentStatusType](./literals.md#documentstatustype) 
2. See [:material-code-brackets: DocumentTypeType](./literals.md#documenttypetype) 
3. See [:material-code-brackets: DocumentFormatType](./literals.md#documentformattype) 
4. See [:material-code-braces: DocumentRequiresTypeDef](./type_defs.md#documentrequirestypedef) 
5. See [:material-code-braces: AttachmentContentTypeDef](./type_defs.md#attachmentcontenttypedef) 
6. See [:material-code-brackets: ReviewStatusType](./literals.md#reviewstatustype) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OpsItemSummaryTypeDef

```python
# OpsItemSummaryTypeDef definition

class OpsItemSummaryTypeDef(TypedDict):
    CreatedBy: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    LastModifiedBy: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
    Priority: NotRequired[int],
    Source: NotRequired[str],
    Status: NotRequired[OpsItemStatusType],  # (1)
    OpsItemId: NotRequired[str],
    Title: NotRequired[str],
    OperationalData: NotRequired[Dict[str, OpsItemDataValueTypeDef]],  # (2)
    Category: NotRequired[str],
    Severity: NotRequired[str],
    OpsItemType: NotRequired[str],
    ActualStartTime: NotRequired[datetime],
    ActualEndTime: NotRequired[datetime],
    PlannedStartTime: NotRequired[datetime],
    PlannedEndTime: NotRequired[datetime],
```

1. See [:material-code-brackets: OpsItemStatusType](./literals.md#opsitemstatustype) 
2. See [:material-code-braces: OpsItemDataValueTypeDef](./type_defs.md#opsitemdatavaluetypedef) 
## CreateOpsItemRequestRequestTypeDef

```python
# CreateOpsItemRequestRequestTypeDef definition

class CreateOpsItemRequestRequestTypeDef(TypedDict):
    Description: str,
    Source: str,
    Title: str,
    OpsItemType: NotRequired[str],
    OperationalData: NotRequired[Mapping[str, OpsItemDataValueTypeDef]],  # (1)
    Notifications: NotRequired[Sequence[OpsItemNotificationTypeDef]],  # (2)
    Priority: NotRequired[int],
    RelatedOpsItems: NotRequired[Sequence[RelatedOpsItemTypeDef]],  # (3)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    Category: NotRequired[str],
    Severity: NotRequired[str],
    ActualStartTime: NotRequired[TimestampTypeDef],
    ActualEndTime: NotRequired[TimestampTypeDef],
    PlannedStartTime: NotRequired[TimestampTypeDef],
    PlannedEndTime: NotRequired[TimestampTypeDef],
    AccountId: NotRequired[str],
```

1. See [:material-code-braces: OpsItemDataValueTypeDef](./type_defs.md#opsitemdatavaluetypedef) 
2. See [:material-code-braces: OpsItemNotificationTypeDef](./type_defs.md#opsitemnotificationtypedef) 
3. See [:material-code-braces: RelatedOpsItemTypeDef](./type_defs.md#relatedopsitemtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## OpsItemTypeDef

```python
# OpsItemTypeDef definition

class OpsItemTypeDef(TypedDict):
    CreatedBy: NotRequired[str],
    OpsItemType: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    Description: NotRequired[str],
    LastModifiedBy: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
    Notifications: NotRequired[List[OpsItemNotificationTypeDef]],  # (1)
    Priority: NotRequired[int],
    RelatedOpsItems: NotRequired[List[RelatedOpsItemTypeDef]],  # (2)
    Status: NotRequired[OpsItemStatusType],  # (3)
    OpsItemId: NotRequired[str],
    Version: NotRequired[str],
    Title: NotRequired[str],
    Source: NotRequired[str],
    OperationalData: NotRequired[Dict[str, OpsItemDataValueTypeDef]],  # (4)
    Category: NotRequired[str],
    Severity: NotRequired[str],
    ActualStartTime: NotRequired[datetime],
    ActualEndTime: NotRequired[datetime],
    PlannedStartTime: NotRequired[datetime],
    PlannedEndTime: NotRequired[datetime],
    OpsItemArn: NotRequired[str],
```

1. See [:material-code-braces: OpsItemNotificationTypeDef](./type_defs.md#opsitemnotificationtypedef) 
2. See [:material-code-braces: RelatedOpsItemTypeDef](./type_defs.md#relatedopsitemtypedef) 
3. See [:material-code-brackets: OpsItemStatusType](./literals.md#opsitemstatustype) 
4. See [:material-code-braces: OpsItemDataValueTypeDef](./type_defs.md#opsitemdatavaluetypedef) 
## UpdateOpsItemRequestRequestTypeDef

```python
# UpdateOpsItemRequestRequestTypeDef definition

class UpdateOpsItemRequestRequestTypeDef(TypedDict):
    OpsItemId: str,
    Description: NotRequired[str],
    OperationalData: NotRequired[Mapping[str, OpsItemDataValueTypeDef]],  # (1)
    OperationalDataToDelete: NotRequired[Sequence[str]],
    Notifications: NotRequired[Sequence[OpsItemNotificationTypeDef]],  # (2)
    Priority: NotRequired[int],
    RelatedOpsItems: NotRequired[Sequence[RelatedOpsItemTypeDef]],  # (3)
    Status: NotRequired[OpsItemStatusType],  # (4)
    Title: NotRequired[str],
    Category: NotRequired[str],
    Severity: NotRequired[str],
    ActualStartTime: NotRequired[TimestampTypeDef],
    ActualEndTime: NotRequired[TimestampTypeDef],
    PlannedStartTime: NotRequired[TimestampTypeDef],
    PlannedEndTime: NotRequired[TimestampTypeDef],
    OpsItemArn: NotRequired[str],
```

1. See [:material-code-braces: OpsItemDataValueTypeDef](./type_defs.md#opsitemdatavaluetypedef) 
2. See [:material-code-braces: OpsItemNotificationTypeDef](./type_defs.md#opsitemnotificationtypedef) 
3. See [:material-code-braces: RelatedOpsItemTypeDef](./type_defs.md#relatedopsitemtypedef) 
4. See [:material-code-brackets: OpsItemStatusType](./literals.md#opsitemstatustype) 
## CreateOpsMetadataRequestRequestTypeDef

```python
# CreateOpsMetadataRequestRequestTypeDef definition

class CreateOpsMetadataRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    Metadata: NotRequired[Mapping[str, MetadataValueTypeDef]],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: MetadataValueTypeDef](./type_defs.md#metadatavaluetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetOpsMetadataResultTypeDef

```python
# GetOpsMetadataResultTypeDef definition

class GetOpsMetadataResultTypeDef(TypedDict):
    ResourceId: str,
    Metadata: Dict[str, MetadataValueTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MetadataValueTypeDef](./type_defs.md#metadatavaluetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateOpsMetadataRequestRequestTypeDef

```python
# UpdateOpsMetadataRequestRequestTypeDef definition

class UpdateOpsMetadataRequestRequestTypeDef(TypedDict):
    OpsMetadataArn: str,
    MetadataToUpdate: NotRequired[Mapping[str, MetadataValueTypeDef]],  # (1)
    KeysToDelete: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: MetadataValueTypeDef](./type_defs.md#metadatavaluetypedef) 
## DescribeActivationsRequestRequestTypeDef

```python
# DescribeActivationsRequestRequestTypeDef definition

class DescribeActivationsRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[DescribeActivationsFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DescribeActivationsFilterTypeDef](./type_defs.md#describeactivationsfiltertypedef) 
## DescribeActivationsRequestDescribeActivationsPaginateTypeDef

```python
# DescribeActivationsRequestDescribeActivationsPaginateTypeDef definition

class DescribeActivationsRequestDescribeActivationsPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[DescribeActivationsFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DescribeActivationsFilterTypeDef](./type_defs.md#describeactivationsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef

```python
# DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef definition

class DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef(TypedDict):
    AssociationId: str,
    ExecutionId: str,
    Filters: NotRequired[Sequence[AssociationExecutionTargetsFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: AssociationExecutionTargetsFilterTypeDef](./type_defs.md#associationexecutiontargetsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef

```python
# DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef definition

class DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef(TypedDict):
    AssociationId: str,
    Filters: NotRequired[Sequence[AssociationExecutionFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: AssociationExecutionFilterTypeDef](./type_defs.md#associationexecutionfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef

```python
# DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef definition

class DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[AutomationExecutionFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: AutomationExecutionFilterTypeDef](./type_defs.md#automationexecutionfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef

```python
# DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef definition

class DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef

```python
# DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef definition

class DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef(TypedDict):
    BaselineId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef

```python
# DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef definition

class DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef

```python
# DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef definition

class DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef(TypedDict):
    InstanceIds: Sequence[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef

```python
# DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef definition

class DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef(TypedDict):
    DeletionId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef

```python
# DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef definition

class DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef(TypedDict):
    OperatingSystem: OperatingSystemType,  # (1)
    Property: PatchPropertyType,  # (2)
    PatchSet: NotRequired[PatchSetType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
2. See [:material-code-brackets: PatchPropertyType](./literals.md#patchpropertytype) 
3. See [:material-code-brackets: PatchSetType](./literals.md#patchsettype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef

```python
# GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef definition

class GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef(TypedDict):
    TypeName: NotRequired[str],
    Aggregator: NotRequired[bool],
    SubType: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef

```python
# GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef definition

class GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef(TypedDict):
    Name: str,
    WithDecryption: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef

```python
# GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef definition

class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(TypedDict):
    ResourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef

```python
# ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef definition

class ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef(TypedDict):
    AssociationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssociationsRequestListAssociationsPaginateTypeDef

```python
# ListAssociationsRequestListAssociationsPaginateTypeDef definition

class ListAssociationsRequestListAssociationsPaginateTypeDef(TypedDict):
    AssociationFilterList: NotRequired[Sequence[AssociationFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: AssociationFilterTypeDef](./type_defs.md#associationfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef

```python
# ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef definition

class ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef(TypedDict):
    CommandId: NotRequired[str],
    InstanceId: NotRequired[str],
    Filters: NotRequired[Sequence[CommandFilterTypeDef]],  # (1)
    Details: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: CommandFilterTypeDef](./type_defs.md#commandfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCommandsRequestListCommandsPaginateTypeDef

```python
# ListCommandsRequestListCommandsPaginateTypeDef definition

class ListCommandsRequestListCommandsPaginateTypeDef(TypedDict):
    CommandId: NotRequired[str],
    InstanceId: NotRequired[str],
    Filters: NotRequired[Sequence[CommandFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: CommandFilterTypeDef](./type_defs.md#commandfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListComplianceItemsRequestListComplianceItemsPaginateTypeDef

```python
# ListComplianceItemsRequestListComplianceItemsPaginateTypeDef definition

class ListComplianceItemsRequestListComplianceItemsPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ComplianceStringFilterTypeDef]],  # (1)
    ResourceIds: NotRequired[Sequence[str]],
    ResourceTypes: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ComplianceStringFilterTypeDef](./type_defs.md#compliancestringfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef

```python
# ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef definition

class ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ComplianceStringFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ComplianceStringFilterTypeDef](./type_defs.md#compliancestringfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef

```python
# ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef definition

class ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef(TypedDict):
    Name: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef

```python
# ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef definition

class ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ComplianceStringFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ComplianceStringFilterTypeDef](./type_defs.md#compliancestringfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef

```python
# ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef definition

class ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef(TypedDict):
    SyncType: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef

```python
# DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef definition

class DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef(TypedDict):
    AutomationExecutionId: str,
    Filters: NotRequired[Sequence[StepExecutionFilterTypeDef]],  # (1)
    ReverseOrder: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: StepExecutionFilterTypeDef](./type_defs.md#stepexecutionfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAutomationStepExecutionsRequestRequestTypeDef

```python
# DescribeAutomationStepExecutionsRequestRequestTypeDef definition

class DescribeAutomationStepExecutionsRequestRequestTypeDef(TypedDict):
    AutomationExecutionId: str,
    Filters: NotRequired[Sequence[StepExecutionFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ReverseOrder: NotRequired[bool],
```

1. See [:material-code-braces: StepExecutionFilterTypeDef](./type_defs.md#stepexecutionfiltertypedef) 
## DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef

```python
# DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef definition

class DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[PatchOrchestratorFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAvailablePatchesRequestRequestTypeDef

```python
# DescribeAvailablePatchesRequestRequestTypeDef definition

class DescribeAvailablePatchesRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[PatchOrchestratorFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
## DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef

```python
# DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef definition

class DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef(TypedDict):
    InstanceId: str,
    Filters: NotRequired[Sequence[PatchOrchestratorFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeInstancePatchesRequestRequestTypeDef

```python
# DescribeInstancePatchesRequestRequestTypeDef definition

class DescribeInstancePatchesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Filters: NotRequired[Sequence[PatchOrchestratorFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
## DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef

```python
# DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef definition

class DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[PatchOrchestratorFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribePatchBaselinesRequestRequestTypeDef

```python
# DescribePatchBaselinesRequestRequestTypeDef definition

class DescribePatchBaselinesRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[PatchOrchestratorFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
## DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef

```python
# DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef definition

class DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[PatchOrchestratorFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribePatchGroupsRequestRequestTypeDef

```python
# DescribePatchGroupsRequestRequestTypeDef definition

class DescribePatchGroupsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    Filters: NotRequired[Sequence[PatchOrchestratorFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
## DescribeAvailablePatchesResultTypeDef

```python
# DescribeAvailablePatchesResultTypeDef definition

class DescribeAvailablePatchesResultTypeDef(TypedDict):
    Patches: List[PatchTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PatchTypeDef](./type_defs.md#patchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEffectiveInstanceAssociationsResultTypeDef

```python
# DescribeEffectiveInstanceAssociationsResultTypeDef definition

class DescribeEffectiveInstanceAssociationsResultTypeDef(TypedDict):
    Associations: List[InstanceAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InstanceAssociationTypeDef](./type_defs.md#instanceassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef

```python
# DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef definition

class DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef(TypedDict):
    InstanceInformationFilterList: NotRequired[Sequence[InstanceInformationFilterTypeDef]],  # (1)
    Filters: NotRequired[Sequence[InstanceInformationStringFilterTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: InstanceInformationFilterTypeDef](./type_defs.md#instanceinformationfiltertypedef) 
2. See [:material-code-braces: InstanceInformationStringFilterTypeDef](./type_defs.md#instanceinformationstringfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeInstanceInformationRequestRequestTypeDef

```python
# DescribeInstanceInformationRequestRequestTypeDef definition

class DescribeInstanceInformationRequestRequestTypeDef(TypedDict):
    InstanceInformationFilterList: NotRequired[Sequence[InstanceInformationFilterTypeDef]],  # (1)
    Filters: NotRequired[Sequence[InstanceInformationStringFilterTypeDef]],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InstanceInformationFilterTypeDef](./type_defs.md#instanceinformationfiltertypedef) 
2. See [:material-code-braces: InstanceInformationStringFilterTypeDef](./type_defs.md#instanceinformationstringfiltertypedef) 
## DescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef

```python
# DescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef definition

class DescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef(TypedDict):
    PatchGroup: str,
    Filters: NotRequired[Sequence[InstancePatchStateFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: InstancePatchStateFilterTypeDef](./type_defs.md#instancepatchstatefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef

```python
# DescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef definition

class DescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef(TypedDict):
    PatchGroup: str,
    Filters: NotRequired[Sequence[InstancePatchStateFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: InstancePatchStateFilterTypeDef](./type_defs.md#instancepatchstatefiltertypedef) 
## DescribeInstancePatchStatesForPatchGroupResultTypeDef

```python
# DescribeInstancePatchStatesForPatchGroupResultTypeDef definition

class DescribeInstancePatchStatesForPatchGroupResultTypeDef(TypedDict):
    InstancePatchStates: List[InstancePatchStateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InstancePatchStateTypeDef](./type_defs.md#instancepatchstatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInstancePatchStatesResultTypeDef

```python
# DescribeInstancePatchStatesResultTypeDef definition

class DescribeInstancePatchStatesResultTypeDef(TypedDict):
    InstancePatchStates: List[InstancePatchStateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InstancePatchStateTypeDef](./type_defs.md#instancepatchstatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInstancePatchesResultTypeDef

```python
# DescribeInstancePatchesResultTypeDef definition

class DescribeInstancePatchesResultTypeDef(TypedDict):
    Patches: List[PatchComplianceDataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PatchComplianceDataTypeDef](./type_defs.md#patchcompliancedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInstancePropertiesRequestDescribeInstancePropertiesPaginateTypeDef

```python
# DescribeInstancePropertiesRequestDescribeInstancePropertiesPaginateTypeDef definition

class DescribeInstancePropertiesRequestDescribeInstancePropertiesPaginateTypeDef(TypedDict):
    InstancePropertyFilterList: NotRequired[Sequence[InstancePropertyFilterTypeDef]],  # (1)
    FiltersWithOperator: NotRequired[Sequence[InstancePropertyStringFilterTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: InstancePropertyFilterTypeDef](./type_defs.md#instancepropertyfiltertypedef) 
2. See [:material-code-braces: InstancePropertyStringFilterTypeDef](./type_defs.md#instancepropertystringfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeInstancePropertiesRequestRequestTypeDef

```python
# DescribeInstancePropertiesRequestRequestTypeDef definition

class DescribeInstancePropertiesRequestRequestTypeDef(TypedDict):
    InstancePropertyFilterList: NotRequired[Sequence[InstancePropertyFilterTypeDef]],  # (1)
    FiltersWithOperator: NotRequired[Sequence[InstancePropertyStringFilterTypeDef]],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InstancePropertyFilterTypeDef](./type_defs.md#instancepropertyfiltertypedef) 
2. See [:material-code-braces: InstancePropertyStringFilterTypeDef](./type_defs.md#instancepropertystringfiltertypedef) 
## DescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef

```python
# DescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef definition

class DescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef(TypedDict):
    WindowExecutionId: str,
    TaskId: str,
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef

```python
# DescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef definition

class DescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef(TypedDict):
    WindowExecutionId: str,
    TaskId: str,
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
## DescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef

```python
# DescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef definition

class DescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef(TypedDict):
    WindowExecutionId: str,
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef

```python
# DescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef definition

class DescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef(TypedDict):
    WindowExecutionId: str,
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
## DescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef

```python
# DescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef definition

class DescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef(TypedDict):
    WindowId: str,
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeMaintenanceWindowExecutionsRequestRequestTypeDef

```python
# DescribeMaintenanceWindowExecutionsRequestRequestTypeDef definition

class DescribeMaintenanceWindowExecutionsRequestRequestTypeDef(TypedDict):
    WindowId: str,
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
## DescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef

```python
# DescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef definition

class DescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef(TypedDict):
    WindowId: str,
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeMaintenanceWindowTargetsRequestRequestTypeDef

```python
# DescribeMaintenanceWindowTargetsRequestRequestTypeDef definition

class DescribeMaintenanceWindowTargetsRequestRequestTypeDef(TypedDict):
    WindowId: str,
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
## DescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef

```python
# DescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef definition

class DescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef(TypedDict):
    WindowId: str,
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeMaintenanceWindowTasksRequestRequestTypeDef

```python
# DescribeMaintenanceWindowTasksRequestRequestTypeDef definition

class DescribeMaintenanceWindowTasksRequestRequestTypeDef(TypedDict):
    WindowId: str,
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
## DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef

```python
# DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef definition

class DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeMaintenanceWindowsRequestRequestTypeDef

```python
# DescribeMaintenanceWindowsRequestRequestTypeDef definition

class DescribeMaintenanceWindowsRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
## DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef

```python
# DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef definition

class DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef(TypedDict):
    WindowExecutionTaskInvocationIdentities: List[MaintenanceWindowExecutionTaskInvocationIdentityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MaintenanceWindowExecutionTaskInvocationIdentityTypeDef](./type_defs.md#maintenancewindowexecutiontaskinvocationidentitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMaintenanceWindowExecutionsResultTypeDef

```python
# DescribeMaintenanceWindowExecutionsResultTypeDef definition

class DescribeMaintenanceWindowExecutionsResultTypeDef(TypedDict):
    WindowExecutions: List[MaintenanceWindowExecutionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MaintenanceWindowExecutionTypeDef](./type_defs.md#maintenancewindowexecutiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef

```python
# DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef definition

class DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef(TypedDict):
    WindowId: NotRequired[str],
    Targets: NotRequired[Sequence[TargetTypeDef]],  # (1)
    ResourceType: NotRequired[MaintenanceWindowResourceTypeType],  # (2)
    Filters: NotRequired[Sequence[PatchOrchestratorFilterTypeDef]],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
2. See [:material-code-brackets: MaintenanceWindowResourceTypeType](./literals.md#maintenancewindowresourcetypetype) 
3. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeMaintenanceWindowScheduleRequestRequestTypeDef

```python
# DescribeMaintenanceWindowScheduleRequestRequestTypeDef definition

class DescribeMaintenanceWindowScheduleRequestRequestTypeDef(TypedDict):
    WindowId: NotRequired[str],
    Targets: NotRequired[Sequence[TargetTypeDef]],  # (1)
    ResourceType: NotRequired[MaintenanceWindowResourceTypeType],  # (2)
    Filters: NotRequired[Sequence[PatchOrchestratorFilterTypeDef]],  # (3)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
2. See [:material-code-brackets: MaintenanceWindowResourceTypeType](./literals.md#maintenancewindowresourcetypetype) 
3. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
## DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef

```python
# DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef definition

class DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef(TypedDict):
    Targets: Sequence[TargetTypeDef],  # (1)
    ResourceType: MaintenanceWindowResourceTypeType,  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
2. See [:material-code-brackets: MaintenanceWindowResourceTypeType](./literals.md#maintenancewindowresourcetypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeMaintenanceWindowsForTargetRequestRequestTypeDef

```python
# DescribeMaintenanceWindowsForTargetRequestRequestTypeDef definition

class DescribeMaintenanceWindowsForTargetRequestRequestTypeDef(TypedDict):
    Targets: Sequence[TargetTypeDef],  # (1)
    ResourceType: MaintenanceWindowResourceTypeType,  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
2. See [:material-code-brackets: MaintenanceWindowResourceTypeType](./literals.md#maintenancewindowresourcetypetype) 
## RegisterTargetWithMaintenanceWindowRequestRequestTypeDef

```python
# RegisterTargetWithMaintenanceWindowRequestRequestTypeDef definition

class RegisterTargetWithMaintenanceWindowRequestRequestTypeDef(TypedDict):
    WindowId: str,
    ResourceType: MaintenanceWindowResourceTypeType,  # (1)
    Targets: Sequence[TargetTypeDef],  # (2)
    OwnerInformation: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    ClientToken: NotRequired[str],
```

1. See [:material-code-brackets: MaintenanceWindowResourceTypeType](./literals.md#maintenancewindowresourcetypetype) 
2. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
## UpdateMaintenanceWindowTargetRequestRequestTypeDef

```python
# UpdateMaintenanceWindowTargetRequestRequestTypeDef definition

class UpdateMaintenanceWindowTargetRequestRequestTypeDef(TypedDict):
    WindowId: str,
    WindowTargetId: str,
    Targets: NotRequired[Sequence[TargetTypeDef]],  # (1)
    OwnerInformation: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    Replace: NotRequired[bool],
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
## DescribeMaintenanceWindowScheduleResultTypeDef

```python
# DescribeMaintenanceWindowScheduleResultTypeDef definition

class DescribeMaintenanceWindowScheduleResultTypeDef(TypedDict):
    ScheduledWindowExecutions: List[ScheduledWindowExecutionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ScheduledWindowExecutionTypeDef](./type_defs.md#scheduledwindowexecutiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMaintenanceWindowsForTargetResultTypeDef

```python
# DescribeMaintenanceWindowsForTargetResultTypeDef definition

class DescribeMaintenanceWindowsForTargetResultTypeDef(TypedDict):
    WindowIdentities: List[MaintenanceWindowIdentityForTargetTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MaintenanceWindowIdentityForTargetTypeDef](./type_defs.md#maintenancewindowidentityfortargettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMaintenanceWindowsResultTypeDef

```python
# DescribeMaintenanceWindowsResultTypeDef definition

class DescribeMaintenanceWindowsResultTypeDef(TypedDict):
    WindowIdentities: List[MaintenanceWindowIdentityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MaintenanceWindowIdentityTypeDef](./type_defs.md#maintenancewindowidentitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOpsItemsRequestDescribeOpsItemsPaginateTypeDef

```python
# DescribeOpsItemsRequestDescribeOpsItemsPaginateTypeDef definition

class DescribeOpsItemsRequestDescribeOpsItemsPaginateTypeDef(TypedDict):
    OpsItemFilters: NotRequired[Sequence[OpsItemFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: OpsItemFilterTypeDef](./type_defs.md#opsitemfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeOpsItemsRequestRequestTypeDef

```python
# DescribeOpsItemsRequestRequestTypeDef definition

class DescribeOpsItemsRequestRequestTypeDef(TypedDict):
    OpsItemFilters: NotRequired[Sequence[OpsItemFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OpsItemFilterTypeDef](./type_defs.md#opsitemfiltertypedef) 
## GetParametersByPathRequestGetParametersByPathPaginateTypeDef

```python
# GetParametersByPathRequestGetParametersByPathPaginateTypeDef definition

class GetParametersByPathRequestGetParametersByPathPaginateTypeDef(TypedDict):
    Path: str,
    Recursive: NotRequired[bool],
    ParameterFilters: NotRequired[Sequence[ParameterStringFilterTypeDef]],  # (1)
    WithDecryption: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ParameterStringFilterTypeDef](./type_defs.md#parameterstringfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetParametersByPathRequestRequestTypeDef

```python
# GetParametersByPathRequestRequestTypeDef definition

class GetParametersByPathRequestRequestTypeDef(TypedDict):
    Path: str,
    Recursive: NotRequired[bool],
    ParameterFilters: NotRequired[Sequence[ParameterStringFilterTypeDef]],  # (1)
    WithDecryption: NotRequired[bool],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ParameterStringFilterTypeDef](./type_defs.md#parameterstringfiltertypedef) 
## DescribeParametersRequestDescribeParametersPaginateTypeDef

```python
# DescribeParametersRequestDescribeParametersPaginateTypeDef definition

class DescribeParametersRequestDescribeParametersPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ParametersFilterTypeDef]],  # (1)
    ParameterFilters: NotRequired[Sequence[ParameterStringFilterTypeDef]],  # (2)
    Shared: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: ParametersFilterTypeDef](./type_defs.md#parametersfiltertypedef) 
2. See [:material-code-braces: ParameterStringFilterTypeDef](./type_defs.md#parameterstringfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeParametersRequestRequestTypeDef

```python
# DescribeParametersRequestRequestTypeDef definition

class DescribeParametersRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ParametersFilterTypeDef]],  # (1)
    ParameterFilters: NotRequired[Sequence[ParameterStringFilterTypeDef]],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Shared: NotRequired[bool],
```

1. See [:material-code-braces: ParametersFilterTypeDef](./type_defs.md#parametersfiltertypedef) 
2. See [:material-code-braces: ParameterStringFilterTypeDef](./type_defs.md#parameterstringfiltertypedef) 
## DescribePatchBaselinesResultTypeDef

```python
# DescribePatchBaselinesResultTypeDef definition

class DescribePatchBaselinesResultTypeDef(TypedDict):
    BaselineIdentities: List[PatchBaselineIdentityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PatchBaselineIdentityTypeDef](./type_defs.md#patchbaselineidentitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PatchGroupPatchBaselineMappingTypeDef

```python
# PatchGroupPatchBaselineMappingTypeDef definition

class PatchGroupPatchBaselineMappingTypeDef(TypedDict):
    PatchGroup: NotRequired[str],
    BaselineIdentity: NotRequired[PatchBaselineIdentityTypeDef],  # (1)
```

1. See [:material-code-braces: PatchBaselineIdentityTypeDef](./type_defs.md#patchbaselineidentitytypedef) 
## DescribeSessionsRequestDescribeSessionsPaginateTypeDef

```python
# DescribeSessionsRequestDescribeSessionsPaginateTypeDef definition

class DescribeSessionsRequestDescribeSessionsPaginateTypeDef(TypedDict):
    State: SessionStateType,  # (1)
    Filters: NotRequired[Sequence[SessionFilterTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SessionStateType](./literals.md#sessionstatetype) 
2. See [:material-code-braces: SessionFilterTypeDef](./type_defs.md#sessionfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSessionsRequestRequestTypeDef

```python
# DescribeSessionsRequestRequestTypeDef definition

class DescribeSessionsRequestRequestTypeDef(TypedDict):
    State: SessionStateType,  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[SessionFilterTypeDef]],  # (2)
```

1. See [:material-code-brackets: SessionStateType](./literals.md#sessionstatetype) 
2. See [:material-code-braces: SessionFilterTypeDef](./type_defs.md#sessionfiltertypedef) 
## UpdateDocumentDefaultVersionResultTypeDef

```python
# UpdateDocumentDefaultVersionResultTypeDef definition

class UpdateDocumentDefaultVersionResultTypeDef(TypedDict):
    Description: DocumentDefaultVersionDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DocumentDefaultVersionDescriptionTypeDef](./type_defs.md#documentdefaultversiondescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DocumentDescriptionTypeDef

```python
# DocumentDescriptionTypeDef definition

class DocumentDescriptionTypeDef(TypedDict):
    Sha1: NotRequired[str],
    Hash: NotRequired[str],
    HashType: NotRequired[DocumentHashTypeType],  # (1)
    Name: NotRequired[str],
    DisplayName: NotRequired[str],
    VersionName: NotRequired[str],
    Owner: NotRequired[str],
    CreatedDate: NotRequired[datetime],
    Status: NotRequired[DocumentStatusType],  # (2)
    StatusInformation: NotRequired[str],
    DocumentVersion: NotRequired[str],
    Description: NotRequired[str],
    Parameters: NotRequired[List[DocumentParameterTypeDef]],  # (3)
    PlatformTypes: NotRequired[List[PlatformTypeType]],  # (4)
    DocumentType: NotRequired[DocumentTypeType],  # (5)
    SchemaVersion: NotRequired[str],
    LatestVersion: NotRequired[str],
    DefaultVersion: NotRequired[str],
    DocumentFormat: NotRequired[DocumentFormatType],  # (6)
    TargetType: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (7)
    AttachmentsInformation: NotRequired[List[AttachmentInformationTypeDef]],  # (8)
    Requires: NotRequired[List[DocumentRequiresTypeDef]],  # (9)
    Author: NotRequired[str],
    ReviewInformation: NotRequired[List[ReviewInformationTypeDef]],  # (10)
    ApprovedVersion: NotRequired[str],
    PendingReviewVersion: NotRequired[str],
    ReviewStatus: NotRequired[ReviewStatusType],  # (11)
    Category: NotRequired[List[str]],
    CategoryEnum: NotRequired[List[str]],
```

1. See [:material-code-brackets: DocumentHashTypeType](./literals.md#documenthashtypetype) 
2. See [:material-code-brackets: DocumentStatusType](./literals.md#documentstatustype) 
3. See [:material-code-braces: DocumentParameterTypeDef](./type_defs.md#documentparametertypedef) 
4. See [:material-code-brackets: PlatformTypeType](./literals.md#platformtypetype) 
5. See [:material-code-brackets: DocumentTypeType](./literals.md#documenttypetype) 
6. See [:material-code-brackets: DocumentFormatType](./literals.md#documentformattype) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
8. See [:material-code-braces: AttachmentInformationTypeDef](./type_defs.md#attachmentinformationtypedef) 
9. See [:material-code-braces: DocumentRequiresTypeDef](./type_defs.md#documentrequirestypedef) 
10. See [:material-code-braces: ReviewInformationTypeDef](./type_defs.md#reviewinformationtypedef) 
11. See [:material-code-brackets: ReviewStatusType](./literals.md#reviewstatustype) 
## ListDocumentsRequestListDocumentsPaginateTypeDef

```python
# ListDocumentsRequestListDocumentsPaginateTypeDef definition

class ListDocumentsRequestListDocumentsPaginateTypeDef(TypedDict):
    DocumentFilterList: NotRequired[Sequence[DocumentFilterTypeDef]],  # (1)
    Filters: NotRequired[Sequence[DocumentKeyValuesFilterTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: DocumentFilterTypeDef](./type_defs.md#documentfiltertypedef) 
2. See [:material-code-braces: DocumentKeyValuesFilterTypeDef](./type_defs.md#documentkeyvaluesfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDocumentsRequestRequestTypeDef

```python
# ListDocumentsRequestRequestTypeDef definition

class ListDocumentsRequestRequestTypeDef(TypedDict):
    DocumentFilterList: NotRequired[Sequence[DocumentFilterTypeDef]],  # (1)
    Filters: NotRequired[Sequence[DocumentKeyValuesFilterTypeDef]],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DocumentFilterTypeDef](./type_defs.md#documentfiltertypedef) 
2. See [:material-code-braces: DocumentKeyValuesFilterTypeDef](./type_defs.md#documentkeyvaluesfiltertypedef) 
## DocumentReviewerResponseSourceTypeDef

```python
# DocumentReviewerResponseSourceTypeDef definition

class DocumentReviewerResponseSourceTypeDef(TypedDict):
    CreateTime: NotRequired[datetime],
    UpdatedTime: NotRequired[datetime],
    ReviewStatus: NotRequired[ReviewStatusType],  # (1)
    Comment: NotRequired[List[DocumentReviewCommentSourceTypeDef]],  # (2)
    Reviewer: NotRequired[str],
```

1. See [:material-code-brackets: ReviewStatusType](./literals.md#reviewstatustype) 
2. See [:material-code-braces: DocumentReviewCommentSourceTypeDef](./type_defs.md#documentreviewcommentsourcetypedef) 
## DocumentReviewsTypeDef

```python
# DocumentReviewsTypeDef definition

class DocumentReviewsTypeDef(TypedDict):
    Action: DocumentReviewActionType,  # (1)
    Comment: NotRequired[Sequence[DocumentReviewCommentSourceTypeDef]],  # (2)
```

1. See [:material-code-brackets: DocumentReviewActionType](./literals.md#documentreviewactiontype) 
2. See [:material-code-braces: DocumentReviewCommentSourceTypeDef](./type_defs.md#documentreviewcommentsourcetypedef) 
## ListDocumentVersionsResultTypeDef

```python
# ListDocumentVersionsResultTypeDef definition

class ListDocumentVersionsResultTypeDef(TypedDict):
    DocumentVersions: List[DocumentVersionInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DocumentVersionInfoTypeDef](./type_defs.md#documentversioninfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EffectivePatchTypeDef

```python
# EffectivePatchTypeDef definition

class EffectivePatchTypeDef(TypedDict):
    Patch: NotRequired[PatchTypeDef],  # (1)
    PatchStatus: NotRequired[PatchStatusTypeDef],  # (2)
```

1. See [:material-code-braces: PatchTypeDef](./type_defs.md#patchtypedef) 
2. See [:material-code-braces: PatchStatusTypeDef](./type_defs.md#patchstatustypedef) 
## GetCommandInvocationRequestCommandExecutedWaitTypeDef

```python
# GetCommandInvocationRequestCommandExecutedWaitTypeDef definition

class GetCommandInvocationRequestCommandExecutedWaitTypeDef(TypedDict):
    CommandId: str,
    InstanceId: str,
    PluginName: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## InventoryGroupTypeDef

```python
# InventoryGroupTypeDef definition

class InventoryGroupTypeDef(TypedDict):
    Name: str,
    Filters: Sequence[InventoryFilterTypeDef],  # (1)
```

1. See [:material-code-braces: InventoryFilterTypeDef](./type_defs.md#inventoryfiltertypedef) 
## ListInventoryEntriesRequestRequestTypeDef

```python
# ListInventoryEntriesRequestRequestTypeDef definition

class ListInventoryEntriesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    TypeName: str,
    Filters: NotRequired[Sequence[InventoryFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: InventoryFilterTypeDef](./type_defs.md#inventoryfiltertypedef) 
## OpsAggregatorPaginatorTypeDef

```python
# OpsAggregatorPaginatorTypeDef definition

class OpsAggregatorPaginatorTypeDef(TypedDict):
    AggregatorType: NotRequired[str],
    TypeName: NotRequired[str],
    AttributeName: NotRequired[str],
    Values: NotRequired[Mapping[str, str]],
    Filters: NotRequired[Sequence[OpsFilterTypeDef]],  # (1)
    Aggregators: NotRequired[Sequence[Mapping[str, Any]]],
```

1. See [:material-code-braces: OpsFilterTypeDef](./type_defs.md#opsfiltertypedef) 
## OpsAggregatorTypeDef

```python
# OpsAggregatorTypeDef definition

class OpsAggregatorTypeDef(TypedDict):
    AggregatorType: NotRequired[str],
    TypeName: NotRequired[str],
    AttributeName: NotRequired[str],
    Values: NotRequired[Mapping[str, str]],
    Filters: NotRequired[Sequence[OpsFilterTypeDef]],  # (1)
    Aggregators: NotRequired[Sequence[Mapping[str, Any]]],
```

1. See [:material-code-braces: OpsFilterTypeDef](./type_defs.md#opsfiltertypedef) 
## GetParameterResultTypeDef

```python
# GetParameterResultTypeDef definition

class GetParameterResultTypeDef(TypedDict):
    Parameter: ParameterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetParametersByPathResultTypeDef

```python
# GetParametersByPathResultTypeDef definition

class GetParametersByPathResultTypeDef(TypedDict):
    Parameters: List[ParameterTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetParametersResultTypeDef

```python
# GetParametersResultTypeDef definition

class GetParametersResultTypeDef(TypedDict):
    Parameters: List[ParameterTypeDef],  # (1)
    InvalidParameters: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePoliciesResponseTypeDef

```python
# GetResourcePoliciesResponseTypeDef definition

class GetResourcePoliciesResponseTypeDef(TypedDict):
    Policies: List[GetResourcePoliciesResponseEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GetResourcePoliciesResponseEntryTypeDef](./type_defs.md#getresourcepoliciesresponseentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceSettingResultTypeDef

```python
# GetServiceSettingResultTypeDef definition

class GetServiceSettingResultTypeDef(TypedDict):
    ServiceSetting: ServiceSettingTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceSettingTypeDef](./type_defs.md#servicesettingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResetServiceSettingResultTypeDef

```python
# ResetServiceSettingResultTypeDef definition

class ResetServiceSettingResultTypeDef(TypedDict):
    ServiceSetting: ServiceSettingTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceSettingTypeDef](./type_defs.md#servicesettingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstanceInformationTypeDef

```python
# InstanceInformationTypeDef definition

class InstanceInformationTypeDef(TypedDict):
    InstanceId: NotRequired[str],
    PingStatus: NotRequired[PingStatusType],  # (1)
    LastPingDateTime: NotRequired[datetime],
    AgentVersion: NotRequired[str],
    IsLatestVersion: NotRequired[bool],
    PlatformType: NotRequired[PlatformTypeType],  # (2)
    PlatformName: NotRequired[str],
    PlatformVersion: NotRequired[str],
    ActivationId: NotRequired[str],
    IamRole: NotRequired[str],
    RegistrationDate: NotRequired[datetime],
    ResourceType: NotRequired[ResourceTypeType],  # (3)
    Name: NotRequired[str],
    IPAddress: NotRequired[str],
    ComputerName: NotRequired[str],
    AssociationStatus: NotRequired[str],
    LastAssociationExecutionDate: NotRequired[datetime],
    LastSuccessfulAssociationExecutionDate: NotRequired[datetime],
    AssociationOverview: NotRequired[InstanceAggregatedAssociationOverviewTypeDef],  # (4)
    SourceId: NotRequired[str],
    SourceType: NotRequired[SourceTypeType],  # (5)
```

1. See [:material-code-brackets: PingStatusType](./literals.md#pingstatustype) 
2. See [:material-code-brackets: PlatformTypeType](./literals.md#platformtypetype) 
3. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
4. See [:material-code-braces: InstanceAggregatedAssociationOverviewTypeDef](./type_defs.md#instanceaggregatedassociationoverviewtypedef) 
5. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
## InstancePropertyTypeDef

```python
# InstancePropertyTypeDef definition

class InstancePropertyTypeDef(TypedDict):
    Name: NotRequired[str],
    InstanceId: NotRequired[str],
    InstanceType: NotRequired[str],
    InstanceRole: NotRequired[str],
    KeyName: NotRequired[str],
    InstanceState: NotRequired[str],
    Architecture: NotRequired[str],
    IPAddress: NotRequired[str],
    LaunchTime: NotRequired[datetime],
    PingStatus: NotRequired[PingStatusType],  # (1)
    LastPingDateTime: NotRequired[datetime],
    AgentVersion: NotRequired[str],
    PlatformType: NotRequired[PlatformTypeType],  # (2)
    PlatformName: NotRequired[str],
    PlatformVersion: NotRequired[str],
    ActivationId: NotRequired[str],
    IamRole: NotRequired[str],
    RegistrationDate: NotRequired[datetime],
    ResourceType: NotRequired[str],
    ComputerName: NotRequired[str],
    AssociationStatus: NotRequired[str],
    LastAssociationExecutionDate: NotRequired[datetime],
    LastSuccessfulAssociationExecutionDate: NotRequired[datetime],
    AssociationOverview: NotRequired[InstanceAggregatedAssociationOverviewTypeDef],  # (3)
    SourceId: NotRequired[str],
    SourceType: NotRequired[SourceTypeType],  # (4)
```

1. See [:material-code-brackets: PingStatusType](./literals.md#pingstatustype) 
2. See [:material-code-brackets: PlatformTypeType](./literals.md#platformtypetype) 
3. See [:material-code-braces: InstanceAggregatedAssociationOverviewTypeDef](./type_defs.md#instanceaggregatedassociationoverviewtypedef) 
4. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
## InstanceAssociationOutputLocationTypeDef

```python
# InstanceAssociationOutputLocationTypeDef definition

class InstanceAssociationOutputLocationTypeDef(TypedDict):
    S3Location: NotRequired[S3OutputLocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3OutputLocationTypeDef](./type_defs.md#s3outputlocationtypedef) 
## InstanceAssociationOutputUrlTypeDef

```python
# InstanceAssociationOutputUrlTypeDef definition

class InstanceAssociationOutputUrlTypeDef(TypedDict):
    S3OutputUrl: NotRequired[S3OutputUrlTypeDef],  # (1)
```

1. See [:material-code-braces: S3OutputUrlTypeDef](./type_defs.md#s3outputurltypedef) 
## InventoryDeletionSummaryTypeDef

```python
# InventoryDeletionSummaryTypeDef definition

class InventoryDeletionSummaryTypeDef(TypedDict):
    TotalCount: NotRequired[int],
    RemainingCount: NotRequired[int],
    SummaryItems: NotRequired[List[InventoryDeletionSummaryItemTypeDef]],  # (1)
```

1. See [:material-code-braces: InventoryDeletionSummaryItemTypeDef](./type_defs.md#inventorydeletionsummaryitemtypedef) 
## InventoryItemSchemaTypeDef

```python
# InventoryItemSchemaTypeDef definition

class InventoryItemSchemaTypeDef(TypedDict):
    TypeName: str,
    Attributes: List[InventoryItemAttributeTypeDef],  # (1)
    Version: NotRequired[str],
    DisplayName: NotRequired[str],
```

1. See [:material-code-braces: InventoryItemAttributeTypeDef](./type_defs.md#inventoryitemattributetypedef) 
## PutInventoryRequestRequestTypeDef

```python
# PutInventoryRequestRequestTypeDef definition

class PutInventoryRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Items: Sequence[InventoryItemTypeDef],  # (1)
```

1. See [:material-code-braces: InventoryItemTypeDef](./type_defs.md#inventoryitemtypedef) 
## InventoryResultEntityTypeDef

```python
# InventoryResultEntityTypeDef definition

class InventoryResultEntityTypeDef(TypedDict):
    Id: NotRequired[str],
    Data: NotRequired[Dict[str, InventoryResultItemTypeDef]],  # (1)
```

1. See [:material-code-braces: InventoryResultItemTypeDef](./type_defs.md#inventoryresultitemtypedef) 
## ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef

```python
# ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef definition

class ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[OpsItemEventFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: OpsItemEventFilterTypeDef](./type_defs.md#opsitemeventfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOpsItemEventsRequestRequestTypeDef

```python
# ListOpsItemEventsRequestRequestTypeDef definition

class ListOpsItemEventsRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[OpsItemEventFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OpsItemEventFilterTypeDef](./type_defs.md#opsitemeventfiltertypedef) 
## ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef

```python
# ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef definition

class ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef(TypedDict):
    OpsItemId: NotRequired[str],
    Filters: NotRequired[Sequence[OpsItemRelatedItemsFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: OpsItemRelatedItemsFilterTypeDef](./type_defs.md#opsitemrelateditemsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOpsItemRelatedItemsRequestRequestTypeDef

```python
# ListOpsItemRelatedItemsRequestRequestTypeDef definition

class ListOpsItemRelatedItemsRequestRequestTypeDef(TypedDict):
    OpsItemId: NotRequired[str],
    Filters: NotRequired[Sequence[OpsItemRelatedItemsFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OpsItemRelatedItemsFilterTypeDef](./type_defs.md#opsitemrelateditemsfiltertypedef) 
## ListOpsMetadataRequestListOpsMetadataPaginateTypeDef

```python
# ListOpsMetadataRequestListOpsMetadataPaginateTypeDef definition

class ListOpsMetadataRequestListOpsMetadataPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[OpsMetadataFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: OpsMetadataFilterTypeDef](./type_defs.md#opsmetadatafiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOpsMetadataRequestRequestTypeDef

```python
# ListOpsMetadataRequestRequestTypeDef definition

class ListOpsMetadataRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[OpsMetadataFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OpsMetadataFilterTypeDef](./type_defs.md#opsmetadatafiltertypedef) 
## ListOpsMetadataResultTypeDef

```python
# ListOpsMetadataResultTypeDef definition

class ListOpsMetadataResultTypeDef(TypedDict):
    OpsMetadataList: List[OpsMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OpsMetadataTypeDef](./type_defs.md#opsmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OpsEntityTypeDef

```python
# OpsEntityTypeDef definition

class OpsEntityTypeDef(TypedDict):
    Id: NotRequired[str],
    Data: NotRequired[Dict[str, OpsEntityItemTypeDef]],  # (1)
```

1. See [:material-code-braces: OpsEntityItemTypeDef](./type_defs.md#opsentityitemtypedef) 
## OpsItemEventSummaryTypeDef

```python
# OpsItemEventSummaryTypeDef definition

class OpsItemEventSummaryTypeDef(TypedDict):
    OpsItemId: NotRequired[str],
    EventId: NotRequired[str],
    Source: NotRequired[str],
    DetailType: NotRequired[str],
    Detail: NotRequired[str],
    CreatedBy: NotRequired[OpsItemIdentityTypeDef],  # (1)
    CreatedTime: NotRequired[datetime],
```

1. See [:material-code-braces: OpsItemIdentityTypeDef](./type_defs.md#opsitemidentitytypedef) 
## OpsItemRelatedItemSummaryTypeDef

```python
# OpsItemRelatedItemSummaryTypeDef definition

class OpsItemRelatedItemSummaryTypeDef(TypedDict):
    OpsItemId: NotRequired[str],
    AssociationId: NotRequired[str],
    ResourceType: NotRequired[str],
    AssociationType: NotRequired[str],
    ResourceUri: NotRequired[str],
    CreatedBy: NotRequired[OpsItemIdentityTypeDef],  # (1)
    CreatedTime: NotRequired[datetime],
    LastModifiedBy: NotRequired[OpsItemIdentityTypeDef],  # (1)
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-braces: OpsItemIdentityTypeDef](./type_defs.md#opsitemidentitytypedef) 
2. See [:material-code-braces: OpsItemIdentityTypeDef](./type_defs.md#opsitemidentitytypedef) 
## ParameterHistoryTypeDef

```python
# ParameterHistoryTypeDef definition

class ParameterHistoryTypeDef(TypedDict):
    Name: NotRequired[str],
    Type: NotRequired[ParameterTypeType],  # (1)
    KeyId: NotRequired[str],
    LastModifiedDate: NotRequired[datetime],
    LastModifiedUser: NotRequired[str],
    Description: NotRequired[str],
    Value: NotRequired[str],
    AllowedPattern: NotRequired[str],
    Version: NotRequired[int],
    Labels: NotRequired[List[str]],
    Tier: NotRequired[ParameterTierType],  # (2)
    Policies: NotRequired[List[ParameterInlinePolicyTypeDef]],  # (3)
    DataType: NotRequired[str],
```

1. See [:material-code-brackets: ParameterTypeType](./literals.md#parametertypetype) 
2. See [:material-code-brackets: ParameterTierType](./literals.md#parametertiertype) 
3. See [:material-code-braces: ParameterInlinePolicyTypeDef](./type_defs.md#parameterinlinepolicytypedef) 
## ParameterMetadataTypeDef

```python
# ParameterMetadataTypeDef definition

class ParameterMetadataTypeDef(TypedDict):
    Name: NotRequired[str],
    ARN: NotRequired[str],
    Type: NotRequired[ParameterTypeType],  # (1)
    KeyId: NotRequired[str],
    LastModifiedDate: NotRequired[datetime],
    LastModifiedUser: NotRequired[str],
    Description: NotRequired[str],
    AllowedPattern: NotRequired[str],
    Version: NotRequired[int],
    Tier: NotRequired[ParameterTierType],  # (2)
    Policies: NotRequired[List[ParameterInlinePolicyTypeDef]],  # (3)
    DataType: NotRequired[str],
```

1. See [:material-code-brackets: ParameterTypeType](./literals.md#parametertypetype) 
2. See [:material-code-brackets: ParameterTierType](./literals.md#parametertiertype) 
3. See [:material-code-braces: ParameterInlinePolicyTypeDef](./type_defs.md#parameterinlinepolicytypedef) 
## PatchFilterGroupOutputTypeDef

```python
# PatchFilterGroupOutputTypeDef definition

class PatchFilterGroupOutputTypeDef(TypedDict):
    PatchFilters: List[PatchFilterOutputTypeDef],  # (1)
```

1. See [:material-code-braces: PatchFilterOutputTypeDef](./type_defs.md#patchfilteroutputtypedef) 
## ResourceDataSyncAwsOrganizationsSourceOutputTypeDef

```python
# ResourceDataSyncAwsOrganizationsSourceOutputTypeDef definition

class ResourceDataSyncAwsOrganizationsSourceOutputTypeDef(TypedDict):
    OrganizationSourceType: str,
    OrganizationalUnits: NotRequired[List[ResourceDataSyncOrganizationalUnitTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourceDataSyncOrganizationalUnitTypeDef](./type_defs.md#resourcedatasyncorganizationalunittypedef) 
## ResourceDataSyncAwsOrganizationsSourceTypeDef

```python
# ResourceDataSyncAwsOrganizationsSourceTypeDef definition

class ResourceDataSyncAwsOrganizationsSourceTypeDef(TypedDict):
    OrganizationSourceType: str,
    OrganizationalUnits: NotRequired[Sequence[ResourceDataSyncOrganizationalUnitTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourceDataSyncOrganizationalUnitTypeDef](./type_defs.md#resourcedatasyncorganizationalunittypedef) 
## ResourceDataSyncS3DestinationTypeDef

```python
# ResourceDataSyncS3DestinationTypeDef definition

class ResourceDataSyncS3DestinationTypeDef(TypedDict):
    BucketName: str,
    SyncFormat: ResourceDataSyncS3FormatType,  # (1)
    Region: str,
    Prefix: NotRequired[str],
    AWSKMSKeyARN: NotRequired[str],
    DestinationDataSharing: NotRequired[ResourceDataSyncDestinationDataSharingTypeDef],  # (2)
```

1. See [:material-code-brackets: ResourceDataSyncS3FormatType](./literals.md#resourcedatasyncs3formattype) 
2. See [:material-code-braces: ResourceDataSyncDestinationDataSharingTypeDef](./type_defs.md#resourcedatasyncdestinationdatasharingtypedef) 
## SessionTypeDef

```python
# SessionTypeDef definition

class SessionTypeDef(TypedDict):
    SessionId: NotRequired[str],
    Target: NotRequired[str],
    Status: NotRequired[SessionStatusType],  # (1)
    StartDate: NotRequired[datetime],
    EndDate: NotRequired[datetime],
    DocumentName: NotRequired[str],
    Owner: NotRequired[str],
    Reason: NotRequired[str],
    Details: NotRequired[str],
    OutputUrl: NotRequired[SessionManagerOutputUrlTypeDef],  # (2)
    MaxSessionDuration: NotRequired[str],
```

1. See [:material-code-brackets: SessionStatusType](./literals.md#sessionstatustype) 
2. See [:material-code-braces: SessionManagerOutputUrlTypeDef](./type_defs.md#sessionmanageroutputurltypedef) 
## DescribeActivationsResultTypeDef

```python
# DescribeActivationsResultTypeDef definition

class DescribeActivationsResultTypeDef(TypedDict):
    ActivationList: List[ActivationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ActivationTypeDef](./type_defs.md#activationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociationExecutionTypeDef

```python
# AssociationExecutionTypeDef definition

class AssociationExecutionTypeDef(TypedDict):
    AssociationId: NotRequired[str],
    AssociationVersion: NotRequired[str],
    ExecutionId: NotRequired[str],
    Status: NotRequired[str],
    DetailedStatus: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    LastExecutionDate: NotRequired[datetime],
    ResourceCountByStatus: NotRequired[str],
    AlarmConfiguration: NotRequired[AlarmConfigurationOutputTypeDef],  # (1)
    TriggeredAlarms: NotRequired[List[AlarmStateInformationTypeDef]],  # (2)
```

1. See [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
2. See [:material-code-braces: AlarmStateInformationTypeDef](./type_defs.md#alarmstateinformationtypedef) 
## CommandTypeDef

```python
# CommandTypeDef definition

class CommandTypeDef(TypedDict):
    CommandId: NotRequired[str],
    DocumentName: NotRequired[str],
    DocumentVersion: NotRequired[str],
    Comment: NotRequired[str],
    ExpiresAfter: NotRequired[datetime],
    Parameters: NotRequired[Dict[str, List[str]]],
    InstanceIds: NotRequired[List[str]],
    Targets: NotRequired[List[TargetOutputTypeDef]],  # (1)
    RequestedDateTime: NotRequired[datetime],
    Status: NotRequired[CommandStatusType],  # (2)
    StatusDetails: NotRequired[str],
    OutputS3Region: NotRequired[str],
    OutputS3BucketName: NotRequired[str],
    OutputS3KeyPrefix: NotRequired[str],
    MaxConcurrency: NotRequired[str],
    MaxErrors: NotRequired[str],
    TargetCount: NotRequired[int],
    CompletedCount: NotRequired[int],
    ErrorCount: NotRequired[int],
    DeliveryTimedOutCount: NotRequired[int],
    ServiceRole: NotRequired[str],
    NotificationConfig: NotRequired[NotificationConfigOutputTypeDef],  # (3)
    CloudWatchOutputConfig: NotRequired[CloudWatchOutputConfigTypeDef],  # (4)
    TimeoutSeconds: NotRequired[int],
    AlarmConfiguration: NotRequired[AlarmConfigurationOutputTypeDef],  # (5)
    TriggeredAlarms: NotRequired[List[AlarmStateInformationTypeDef]],  # (6)
```

1. See [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-brackets: CommandStatusType](./literals.md#commandstatustype) 
3. See [:material-code-braces: NotificationConfigOutputTypeDef](./type_defs.md#notificationconfigoutputtypedef) 
4. See [:material-code-braces: CloudWatchOutputConfigTypeDef](./type_defs.md#cloudwatchoutputconfigtypedef) 
5. See [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
6. See [:material-code-braces: AlarmStateInformationTypeDef](./type_defs.md#alarmstateinformationtypedef) 
## GetMaintenanceWindowExecutionTaskResultTypeDef

```python
# GetMaintenanceWindowExecutionTaskResultTypeDef definition

class GetMaintenanceWindowExecutionTaskResultTypeDef(TypedDict):
    WindowExecutionId: str,
    TaskExecutionId: str,
    TaskArn: str,
    ServiceRole: str,
    Type: MaintenanceWindowTaskTypeType,  # (1)
    TaskParameters: List[Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef]],  # (2)
    Priority: int,
    MaxConcurrency: str,
    MaxErrors: str,
    Status: MaintenanceWindowExecutionStatusType,  # (3)
    StatusDetails: str,
    StartTime: datetime,
    EndTime: datetime,
    AlarmConfiguration: AlarmConfigurationOutputTypeDef,  # (4)
    TriggeredAlarms: List[AlarmStateInformationTypeDef],  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: MaintenanceWindowTaskTypeType](./literals.md#maintenancewindowtasktypetype) 
2. See [:material-code-braces: MaintenanceWindowTaskParameterValueExpressionOutputTypeDef](./type_defs.md#maintenancewindowtaskparametervalueexpressionoutputtypedef) 
3. See [:material-code-brackets: MaintenanceWindowExecutionStatusType](./literals.md#maintenancewindowexecutionstatustype) 
4. See [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
5. See [:material-code-braces: AlarmStateInformationTypeDef](./type_defs.md#alarmstateinformationtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MaintenanceWindowExecutionTaskIdentityTypeDef

```python
# MaintenanceWindowExecutionTaskIdentityTypeDef definition

class MaintenanceWindowExecutionTaskIdentityTypeDef(TypedDict):
    WindowExecutionId: NotRequired[str],
    TaskExecutionId: NotRequired[str],
    Status: NotRequired[MaintenanceWindowExecutionStatusType],  # (1)
    StatusDetails: NotRequired[str],
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    TaskArn: NotRequired[str],
    TaskType: NotRequired[MaintenanceWindowTaskTypeType],  # (2)
    AlarmConfiguration: NotRequired[AlarmConfigurationOutputTypeDef],  # (3)
    TriggeredAlarms: NotRequired[List[AlarmStateInformationTypeDef]],  # (4)
```

1. See [:material-code-brackets: MaintenanceWindowExecutionStatusType](./literals.md#maintenancewindowexecutionstatustype) 
2. See [:material-code-brackets: MaintenanceWindowTaskTypeType](./literals.md#maintenancewindowtasktypetype) 
3. See [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
4. See [:material-code-braces: AlarmStateInformationTypeDef](./type_defs.md#alarmstateinformationtypedef) 
## MaintenanceWindowTaskTypeDef

```python
# MaintenanceWindowTaskTypeDef definition

class MaintenanceWindowTaskTypeDef(TypedDict):
    WindowId: NotRequired[str],
    WindowTaskId: NotRequired[str],
    TaskArn: NotRequired[str],
    Type: NotRequired[MaintenanceWindowTaskTypeType],  # (1)
    Targets: NotRequired[List[TargetOutputTypeDef]],  # (2)
    TaskParameters: NotRequired[Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef]],  # (3)
    Priority: NotRequired[int],
    LoggingInfo: NotRequired[LoggingInfoTypeDef],  # (4)
    ServiceRoleArn: NotRequired[str],
    MaxConcurrency: NotRequired[str],
    MaxErrors: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    CutoffBehavior: NotRequired[MaintenanceWindowTaskCutoffBehaviorType],  # (5)
    AlarmConfiguration: NotRequired[AlarmConfigurationOutputTypeDef],  # (6)
```

1. See [:material-code-brackets: MaintenanceWindowTaskTypeType](./literals.md#maintenancewindowtasktypetype) 
2. See [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
3. See [:material-code-braces: MaintenanceWindowTaskParameterValueExpressionOutputTypeDef](./type_defs.md#maintenancewindowtaskparametervalueexpressionoutputtypedef) 
4. See [:material-code-braces: LoggingInfoTypeDef](./type_defs.md#logginginfotypedef) 
5. See [:material-code-brackets: MaintenanceWindowTaskCutoffBehaviorType](./literals.md#maintenancewindowtaskcutoffbehaviortype) 
6. See [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
## TargetLocationOutputTypeDef

```python
# TargetLocationOutputTypeDef definition

class TargetLocationOutputTypeDef(TypedDict):
    Accounts: NotRequired[List[str]],
    Regions: NotRequired[List[str]],
    TargetLocationMaxConcurrency: NotRequired[str],
    TargetLocationMaxErrors: NotRequired[str],
    ExecutionRoleName: NotRequired[str],
    TargetLocationAlarmConfiguration: NotRequired[AlarmConfigurationOutputTypeDef],  # (1)
    IncludeChildOrganizationUnits: NotRequired[bool],
    ExcludeAccounts: NotRequired[List[str]],
    Targets: NotRequired[List[TargetOutputTypeDef]],  # (2)
    TargetsMaxConcurrency: NotRequired[str],
    TargetsMaxErrors: NotRequired[str],
```

1. See [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
2. See [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
## SendCommandRequestRequestTypeDef

```python
# SendCommandRequestRequestTypeDef definition

class SendCommandRequestRequestTypeDef(TypedDict):
    DocumentName: str,
    InstanceIds: NotRequired[Sequence[str]],
    Targets: NotRequired[Sequence[TargetTypeDef]],  # (1)
    DocumentVersion: NotRequired[str],
    DocumentHash: NotRequired[str],
    DocumentHashType: NotRequired[DocumentHashTypeType],  # (2)
    TimeoutSeconds: NotRequired[int],
    Comment: NotRequired[str],
    Parameters: NotRequired[Mapping[str, Sequence[str]]],
    OutputS3Region: NotRequired[str],
    OutputS3BucketName: NotRequired[str],
    OutputS3KeyPrefix: NotRequired[str],
    MaxConcurrency: NotRequired[str],
    MaxErrors: NotRequired[str],
    ServiceRoleArn: NotRequired[str],
    NotificationConfig: NotRequired[NotificationConfigTypeDef],  # (3)
    CloudWatchOutputConfig: NotRequired[CloudWatchOutputConfigTypeDef],  # (4)
    AlarmConfiguration: NotRequired[AlarmConfigurationTypeDef],  # (5)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
2. See [:material-code-brackets: DocumentHashTypeType](./literals.md#documenthashtypetype) 
3. See [:material-code-braces: NotificationConfigTypeDef](./type_defs.md#notificationconfigtypedef) 
4. See [:material-code-braces: CloudWatchOutputConfigTypeDef](./type_defs.md#cloudwatchoutputconfigtypedef) 
5. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) 
## ListAssociationsResultTypeDef

```python
# ListAssociationsResultTypeDef definition

class ListAssociationsResultTypeDef(TypedDict):
    Associations: List[AssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AssociationTypeDef](./type_defs.md#associationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMaintenanceWindowTargetsResultTypeDef

```python
# DescribeMaintenanceWindowTargetsResultTypeDef definition

class DescribeMaintenanceWindowTargetsResultTypeDef(TypedDict):
    Targets: List[MaintenanceWindowTargetTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MaintenanceWindowTargetTypeDef](./type_defs.md#maintenancewindowtargettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAssociationExecutionTargetsResultTypeDef

```python
# DescribeAssociationExecutionTargetsResultTypeDef definition

class DescribeAssociationExecutionTargetsResultTypeDef(TypedDict):
    AssociationExecutionTargets: List[AssociationExecutionTargetTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AssociationExecutionTargetTypeDef](./type_defs.md#associationexecutiontargettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAssociationStatusRequestRequestTypeDef

```python
# UpdateAssociationStatusRequestRequestTypeDef definition

class UpdateAssociationStatusRequestRequestTypeDef(TypedDict):
    Name: str,
    InstanceId: str,
    AssociationStatus: AssociationStatusTypeDef,  # (1)
```

1. See [:material-code-braces: AssociationStatusTypeDef](./type_defs.md#associationstatustypedef) 
## PutComplianceItemsRequestRequestTypeDef

```python
# PutComplianceItemsRequestRequestTypeDef definition

class PutComplianceItemsRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    ResourceType: str,
    ComplianceType: str,
    ExecutionSummary: ComplianceExecutionSummaryTypeDef,  # (1)
    Items: Sequence[ComplianceItemEntryTypeDef],  # (2)
    ItemContentHash: NotRequired[str],
    UploadType: NotRequired[ComplianceUploadTypeType],  # (3)
```

1. See [:material-code-braces: ComplianceExecutionSummaryTypeDef](./type_defs.md#complianceexecutionsummarytypedef) 
2. See [:material-code-braces: ComplianceItemEntryTypeDef](./type_defs.md#complianceitementrytypedef) 
3. See [:material-code-brackets: ComplianceUploadTypeType](./literals.md#complianceuploadtypetype) 
## ListCommandInvocationsResultTypeDef

```python
# ListCommandInvocationsResultTypeDef definition

class ListCommandInvocationsResultTypeDef(TypedDict):
    CommandInvocations: List[CommandInvocationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CommandInvocationTypeDef](./type_defs.md#commandinvocationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MaintenanceWindowTaskInvocationParametersOutputTypeDef

```python
# MaintenanceWindowTaskInvocationParametersOutputTypeDef definition

class MaintenanceWindowTaskInvocationParametersOutputTypeDef(TypedDict):
    RunCommand: NotRequired[MaintenanceWindowRunCommandParametersOutputTypeDef],  # (1)
    Automation: NotRequired[MaintenanceWindowAutomationParametersOutputTypeDef],  # (2)
    StepFunctions: NotRequired[MaintenanceWindowStepFunctionsParametersTypeDef],  # (3)
    Lambda: NotRequired[MaintenanceWindowLambdaParametersOutputTypeDef],  # (4)
```

1. See [:material-code-braces: MaintenanceWindowRunCommandParametersOutputTypeDef](./type_defs.md#maintenancewindowruncommandparametersoutputtypedef) 
2. See [:material-code-braces: MaintenanceWindowAutomationParametersOutputTypeDef](./type_defs.md#maintenancewindowautomationparametersoutputtypedef) 
3. See [:material-code-braces: MaintenanceWindowStepFunctionsParametersTypeDef](./type_defs.md#maintenancewindowstepfunctionsparameterstypedef) 
4. See [:material-code-braces: MaintenanceWindowLambdaParametersOutputTypeDef](./type_defs.md#maintenancewindowlambdaparametersoutputtypedef) 
## ListComplianceItemsResultTypeDef

```python
# ListComplianceItemsResultTypeDef definition

class ListComplianceItemsResultTypeDef(TypedDict):
    ComplianceItems: List[ComplianceItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ComplianceItemTypeDef](./type_defs.md#complianceitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ComplianceSummaryItemTypeDef

```python
# ComplianceSummaryItemTypeDef definition

class ComplianceSummaryItemTypeDef(TypedDict):
    ComplianceType: NotRequired[str],
    CompliantSummary: NotRequired[CompliantSummaryTypeDef],  # (1)
    NonCompliantSummary: NotRequired[NonCompliantSummaryTypeDef],  # (2)
```

1. See [:material-code-braces: CompliantSummaryTypeDef](./type_defs.md#compliantsummarytypedef) 
2. See [:material-code-braces: NonCompliantSummaryTypeDef](./type_defs.md#noncompliantsummarytypedef) 
## ResourceComplianceSummaryItemTypeDef

```python
# ResourceComplianceSummaryItemTypeDef definition

class ResourceComplianceSummaryItemTypeDef(TypedDict):
    ComplianceType: NotRequired[str],
    ResourceType: NotRequired[str],
    ResourceId: NotRequired[str],
    Status: NotRequired[ComplianceStatusType],  # (1)
    OverallSeverity: NotRequired[ComplianceSeverityType],  # (2)
    ExecutionSummary: NotRequired[ComplianceExecutionSummaryOutputTypeDef],  # (3)
    CompliantSummary: NotRequired[CompliantSummaryTypeDef],  # (4)
    NonCompliantSummary: NotRequired[NonCompliantSummaryTypeDef],  # (5)
```

1. See [:material-code-brackets: ComplianceStatusType](./literals.md#compliancestatustype) 
2. See [:material-code-brackets: ComplianceSeverityType](./literals.md#complianceseveritytype) 
3. See [:material-code-braces: ComplianceExecutionSummaryOutputTypeDef](./type_defs.md#complianceexecutionsummaryoutputtypedef) 
4. See [:material-code-braces: CompliantSummaryTypeDef](./type_defs.md#compliantsummarytypedef) 
5. See [:material-code-braces: NonCompliantSummaryTypeDef](./type_defs.md#noncompliantsummarytypedef) 
## ListDocumentsResultTypeDef

```python
# ListDocumentsResultTypeDef definition

class ListDocumentsResultTypeDef(TypedDict):
    DocumentIdentifiers: List[DocumentIdentifierTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DocumentIdentifierTypeDef](./type_defs.md#documentidentifiertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOpsItemsResponseTypeDef

```python
# DescribeOpsItemsResponseTypeDef definition

class DescribeOpsItemsResponseTypeDef(TypedDict):
    OpsItemSummaries: List[OpsItemSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OpsItemSummaryTypeDef](./type_defs.md#opsitemsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOpsItemResponseTypeDef

```python
# GetOpsItemResponseTypeDef definition

class GetOpsItemResponseTypeDef(TypedDict):
    OpsItem: OpsItemTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OpsItemTypeDef](./type_defs.md#opsitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePatchGroupsResultTypeDef

```python
# DescribePatchGroupsResultTypeDef definition

class DescribePatchGroupsResultTypeDef(TypedDict):
    Mappings: List[PatchGroupPatchBaselineMappingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PatchGroupPatchBaselineMappingTypeDef](./type_defs.md#patchgrouppatchbaselinemappingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDocumentResultTypeDef

```python
# CreateDocumentResultTypeDef definition

class CreateDocumentResultTypeDef(TypedDict):
    DocumentDescription: DocumentDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DocumentDescriptionTypeDef](./type_defs.md#documentdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDocumentResultTypeDef

```python
# DescribeDocumentResultTypeDef definition

class DescribeDocumentResultTypeDef(TypedDict):
    Document: DocumentDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DocumentDescriptionTypeDef](./type_defs.md#documentdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDocumentResultTypeDef

```python
# UpdateDocumentResultTypeDef definition

class UpdateDocumentResultTypeDef(TypedDict):
    DocumentDescription: DocumentDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DocumentDescriptionTypeDef](./type_defs.md#documentdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DocumentMetadataResponseInfoTypeDef

```python
# DocumentMetadataResponseInfoTypeDef definition

class DocumentMetadataResponseInfoTypeDef(TypedDict):
    ReviewerResponse: NotRequired[List[DocumentReviewerResponseSourceTypeDef]],  # (1)
```

1. See [:material-code-braces: DocumentReviewerResponseSourceTypeDef](./type_defs.md#documentreviewerresponsesourcetypedef) 
## UpdateDocumentMetadataRequestRequestTypeDef

```python
# UpdateDocumentMetadataRequestRequestTypeDef definition

class UpdateDocumentMetadataRequestRequestTypeDef(TypedDict):
    Name: str,
    DocumentReviews: DocumentReviewsTypeDef,  # (1)
    DocumentVersion: NotRequired[str],
```

1. See [:material-code-braces: DocumentReviewsTypeDef](./type_defs.md#documentreviewstypedef) 
## DescribeEffectivePatchesForPatchBaselineResultTypeDef

```python
# DescribeEffectivePatchesForPatchBaselineResultTypeDef definition

class DescribeEffectivePatchesForPatchBaselineResultTypeDef(TypedDict):
    EffectivePatches: List[EffectivePatchTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EffectivePatchTypeDef](./type_defs.md#effectivepatchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InventoryAggregatorPaginatorTypeDef

```python
# InventoryAggregatorPaginatorTypeDef definition

class InventoryAggregatorPaginatorTypeDef(TypedDict):
    Expression: NotRequired[str],
    Aggregators: NotRequired[Sequence[Mapping[str, Any]]],
    Groups: NotRequired[Sequence[InventoryGroupTypeDef]],  # (1)
```

1. See [:material-code-braces: InventoryGroupTypeDef](./type_defs.md#inventorygrouptypedef) 
## InventoryAggregatorTypeDef

```python
# InventoryAggregatorTypeDef definition

class InventoryAggregatorTypeDef(TypedDict):
    Expression: NotRequired[str],
    Aggregators: NotRequired[Sequence[Mapping[str, Any]]],
    Groups: NotRequired[Sequence[InventoryGroupTypeDef]],  # (1)
```

1. See [:material-code-braces: InventoryGroupTypeDef](./type_defs.md#inventorygrouptypedef) 
## GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef

```python
# GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef definition

class GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef(TypedDict):
    SyncName: NotRequired[str],
    Filters: NotRequired[Sequence[OpsFilterTypeDef]],  # (1)
    Aggregators: NotRequired[Sequence[OpsAggregatorPaginatorTypeDef]],  # (2)
    ResultAttributes: NotRequired[Sequence[OpsResultAttributeTypeDef]],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: OpsFilterTypeDef](./type_defs.md#opsfiltertypedef) 
2. See [:material-code-braces: OpsAggregatorPaginatorTypeDef](./type_defs.md#opsaggregatorpaginatortypedef) 
3. See [:material-code-braces: OpsResultAttributeTypeDef](./type_defs.md#opsresultattributetypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetOpsSummaryRequestRequestTypeDef

```python
# GetOpsSummaryRequestRequestTypeDef definition

class GetOpsSummaryRequestRequestTypeDef(TypedDict):
    SyncName: NotRequired[str],
    Filters: NotRequired[Sequence[OpsFilterTypeDef]],  # (1)
    Aggregators: NotRequired[Sequence[OpsAggregatorTypeDef]],  # (2)
    ResultAttributes: NotRequired[Sequence[OpsResultAttributeTypeDef]],  # (3)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: OpsFilterTypeDef](./type_defs.md#opsfiltertypedef) 
2. See [:material-code-braces: OpsAggregatorTypeDef](./type_defs.md#opsaggregatortypedef) 
3. See [:material-code-braces: OpsResultAttributeTypeDef](./type_defs.md#opsresultattributetypedef) 
## DescribeInstanceInformationResultTypeDef

```python
# DescribeInstanceInformationResultTypeDef definition

class DescribeInstanceInformationResultTypeDef(TypedDict):
    InstanceInformationList: List[InstanceInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InstanceInformationTypeDef](./type_defs.md#instanceinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInstancePropertiesResultTypeDef

```python
# DescribeInstancePropertiesResultTypeDef definition

class DescribeInstancePropertiesResultTypeDef(TypedDict):
    InstanceProperties: List[InstancePropertyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InstancePropertyTypeDef](./type_defs.md#instancepropertytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstanceAssociationStatusInfoTypeDef

```python
# InstanceAssociationStatusInfoTypeDef definition

class InstanceAssociationStatusInfoTypeDef(TypedDict):
    AssociationId: NotRequired[str],
    Name: NotRequired[str],
    DocumentVersion: NotRequired[str],
    AssociationVersion: NotRequired[str],
    InstanceId: NotRequired[str],
    ExecutionDate: NotRequired[datetime],
    Status: NotRequired[str],
    DetailedStatus: NotRequired[str],
    ExecutionSummary: NotRequired[str],
    ErrorCode: NotRequired[str],
    OutputUrl: NotRequired[InstanceAssociationOutputUrlTypeDef],  # (1)
    AssociationName: NotRequired[str],
```

1. See [:material-code-braces: InstanceAssociationOutputUrlTypeDef](./type_defs.md#instanceassociationoutputurltypedef) 
## DeleteInventoryResultTypeDef

```python
# DeleteInventoryResultTypeDef definition

class DeleteInventoryResultTypeDef(TypedDict):
    DeletionId: str,
    TypeName: str,
    DeletionSummary: InventoryDeletionSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InventoryDeletionSummaryTypeDef](./type_defs.md#inventorydeletionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InventoryDeletionStatusItemTypeDef

```python
# InventoryDeletionStatusItemTypeDef definition

class InventoryDeletionStatusItemTypeDef(TypedDict):
    DeletionId: NotRequired[str],
    TypeName: NotRequired[str],
    DeletionStartTime: NotRequired[datetime],
    LastStatus: NotRequired[InventoryDeletionStatusType],  # (1)
    LastStatusMessage: NotRequired[str],
    DeletionSummary: NotRequired[InventoryDeletionSummaryTypeDef],  # (2)
    LastStatusUpdateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: InventoryDeletionStatusType](./literals.md#inventorydeletionstatustype) 
2. See [:material-code-braces: InventoryDeletionSummaryTypeDef](./type_defs.md#inventorydeletionsummarytypedef) 
## GetInventorySchemaResultTypeDef

```python
# GetInventorySchemaResultTypeDef definition

class GetInventorySchemaResultTypeDef(TypedDict):
    Schemas: List[InventoryItemSchemaTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InventoryItemSchemaTypeDef](./type_defs.md#inventoryitemschematypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInventoryResultTypeDef

```python
# GetInventoryResultTypeDef definition

class GetInventoryResultTypeDef(TypedDict):
    Entities: List[InventoryResultEntityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InventoryResultEntityTypeDef](./type_defs.md#inventoryresultentitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MaintenanceWindowRunCommandParametersTypeDef

```python
# MaintenanceWindowRunCommandParametersTypeDef definition

class MaintenanceWindowRunCommandParametersTypeDef(TypedDict):
    Comment: NotRequired[str],
    CloudWatchOutputConfig: NotRequired[CloudWatchOutputConfigTypeDef],  # (1)
    DocumentHash: NotRequired[str],
    DocumentHashType: NotRequired[DocumentHashTypeType],  # (2)
    DocumentVersion: NotRequired[str],
    NotificationConfig: NotRequired[NotificationConfigUnionTypeDef],  # (3)
    OutputS3BucketName: NotRequired[str],
    OutputS3KeyPrefix: NotRequired[str],
    Parameters: NotRequired[Mapping[str, Sequence[str]]],
    ServiceRoleArn: NotRequired[str],
    TimeoutSeconds: NotRequired[int],
```

1. See [:material-code-braces: CloudWatchOutputConfigTypeDef](./type_defs.md#cloudwatchoutputconfigtypedef) 
2. See [:material-code-brackets: DocumentHashTypeType](./literals.md#documenthashtypetype) 
3. See [:material-code-braces: NotificationConfigTypeDef](./type_defs.md#notificationconfigtypedef) [:material-code-braces: NotificationConfigOutputTypeDef](./type_defs.md#notificationconfigoutputtypedef) 
## GetOpsSummaryResultTypeDef

```python
# GetOpsSummaryResultTypeDef definition

class GetOpsSummaryResultTypeDef(TypedDict):
    Entities: List[OpsEntityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OpsEntityTypeDef](./type_defs.md#opsentitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOpsItemEventsResponseTypeDef

```python
# ListOpsItemEventsResponseTypeDef definition

class ListOpsItemEventsResponseTypeDef(TypedDict):
    Summaries: List[OpsItemEventSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OpsItemEventSummaryTypeDef](./type_defs.md#opsitemeventsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOpsItemRelatedItemsResponseTypeDef

```python
# ListOpsItemRelatedItemsResponseTypeDef definition

class ListOpsItemRelatedItemsResponseTypeDef(TypedDict):
    Summaries: List[OpsItemRelatedItemSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OpsItemRelatedItemSummaryTypeDef](./type_defs.md#opsitemrelateditemsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetParameterHistoryResultTypeDef

```python
# GetParameterHistoryResultTypeDef definition

class GetParameterHistoryResultTypeDef(TypedDict):
    Parameters: List[ParameterHistoryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ParameterHistoryTypeDef](./type_defs.md#parameterhistorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeParametersResultTypeDef

```python
# DescribeParametersResultTypeDef definition

class DescribeParametersResultTypeDef(TypedDict):
    Parameters: List[ParameterMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ParameterMetadataTypeDef](./type_defs.md#parametermetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PatchRuleOutputTypeDef

```python
# PatchRuleOutputTypeDef definition

class PatchRuleOutputTypeDef(TypedDict):
    PatchFilterGroup: PatchFilterGroupOutputTypeDef,  # (1)
    ComplianceLevel: NotRequired[PatchComplianceLevelType],  # (2)
    ApproveAfterDays: NotRequired[int],
    ApproveUntilDate: NotRequired[str],
    EnableNonSecurity: NotRequired[bool],
```

1. See [:material-code-braces: PatchFilterGroupOutputTypeDef](./type_defs.md#patchfiltergroupoutputtypedef) 
2. See [:material-code-brackets: PatchComplianceLevelType](./literals.md#patchcomplianceleveltype) 
## PatchFilterGroupTypeDef

```python
# PatchFilterGroupTypeDef definition

class PatchFilterGroupTypeDef(TypedDict):
    PatchFilters: Sequence[PatchFilterUnionTypeDef],  # (1)
```

1. See [:material-code-braces: PatchFilterTypeDef](./type_defs.md#patchfiltertypedef) [:material-code-braces: PatchFilterOutputTypeDef](./type_defs.md#patchfilteroutputtypedef) 
## ResourceDataSyncSourceWithStateTypeDef

```python
# ResourceDataSyncSourceWithStateTypeDef definition

class ResourceDataSyncSourceWithStateTypeDef(TypedDict):
    SourceType: NotRequired[str],
    AwsOrganizationsSource: NotRequired[ResourceDataSyncAwsOrganizationsSourceOutputTypeDef],  # (1)
    SourceRegions: NotRequired[List[str]],
    IncludeFutureRegions: NotRequired[bool],
    State: NotRequired[str],
    EnableAllOpsDataSources: NotRequired[bool],
```

1. See [:material-code-braces: ResourceDataSyncAwsOrganizationsSourceOutputTypeDef](./type_defs.md#resourcedatasyncawsorganizationssourceoutputtypedef) 
## DescribeSessionsResponseTypeDef

```python
# DescribeSessionsResponseTypeDef definition

class DescribeSessionsResponseTypeDef(TypedDict):
    Sessions: List[SessionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SessionTypeDef](./type_defs.md#sessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAssociationExecutionsResultTypeDef

```python
# DescribeAssociationExecutionsResultTypeDef definition

class DescribeAssociationExecutionsResultTypeDef(TypedDict):
    AssociationExecutions: List[AssociationExecutionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AssociationExecutionTypeDef](./type_defs.md#associationexecutiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCommandsResultTypeDef

```python
# ListCommandsResultTypeDef definition

class ListCommandsResultTypeDef(TypedDict):
    Commands: List[CommandTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CommandTypeDef](./type_defs.md#commandtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendCommandResultTypeDef

```python
# SendCommandResultTypeDef definition

class SendCommandResultTypeDef(TypedDict):
    Command: CommandTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CommandTypeDef](./type_defs.md#commandtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMaintenanceWindowExecutionTasksResultTypeDef

```python
# DescribeMaintenanceWindowExecutionTasksResultTypeDef definition

class DescribeMaintenanceWindowExecutionTasksResultTypeDef(TypedDict):
    WindowExecutionTaskIdentities: List[MaintenanceWindowExecutionTaskIdentityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MaintenanceWindowExecutionTaskIdentityTypeDef](./type_defs.md#maintenancewindowexecutiontaskidentitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMaintenanceWindowTasksResultTypeDef

```python
# DescribeMaintenanceWindowTasksResultTypeDef definition

class DescribeMaintenanceWindowTasksResultTypeDef(TypedDict):
    Tasks: List[MaintenanceWindowTaskTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MaintenanceWindowTaskTypeDef](./type_defs.md#maintenancewindowtasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociationDescriptionTypeDef

```python
# AssociationDescriptionTypeDef definition

class AssociationDescriptionTypeDef(TypedDict):
    Name: NotRequired[str],
    InstanceId: NotRequired[str],
    AssociationVersion: NotRequired[str],
    Date: NotRequired[datetime],
    LastUpdateAssociationDate: NotRequired[datetime],
    Status: NotRequired[AssociationStatusOutputTypeDef],  # (1)
    Overview: NotRequired[AssociationOverviewTypeDef],  # (2)
    DocumentVersion: NotRequired[str],
    AutomationTargetParameterName: NotRequired[str],
    Parameters: NotRequired[Dict[str, List[str]]],
    AssociationId: NotRequired[str],
    Targets: NotRequired[List[TargetOutputTypeDef]],  # (3)
    ScheduleExpression: NotRequired[str],
    OutputLocation: NotRequired[InstanceAssociationOutputLocationTypeDef],  # (4)
    LastExecutionDate: NotRequired[datetime],
    LastSuccessfulExecutionDate: NotRequired[datetime],
    AssociationName: NotRequired[str],
    MaxErrors: NotRequired[str],
    MaxConcurrency: NotRequired[str],
    ComplianceSeverity: NotRequired[AssociationComplianceSeverityType],  # (5)
    SyncCompliance: NotRequired[AssociationSyncComplianceType],  # (6)
    ApplyOnlyAtCronInterval: NotRequired[bool],
    CalendarNames: NotRequired[List[str]],
    TargetLocations: NotRequired[List[TargetLocationOutputTypeDef]],  # (7)
    ScheduleOffset: NotRequired[int],
    Duration: NotRequired[int],
    TargetMaps: NotRequired[List[Dict[str, List[str]]]],
    AlarmConfiguration: NotRequired[AlarmConfigurationOutputTypeDef],  # (8)
    TriggeredAlarms: NotRequired[List[AlarmStateInformationTypeDef]],  # (9)
```

1. See [:material-code-braces: AssociationStatusOutputTypeDef](./type_defs.md#associationstatusoutputtypedef) 
2. See [:material-code-braces: AssociationOverviewTypeDef](./type_defs.md#associationoverviewtypedef) 
3. See [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
4. See [:material-code-braces: InstanceAssociationOutputLocationTypeDef](./type_defs.md#instanceassociationoutputlocationtypedef) 
5. See [:material-code-brackets: AssociationComplianceSeverityType](./literals.md#associationcomplianceseveritytype) 
6. See [:material-code-brackets: AssociationSyncComplianceType](./literals.md#associationsynccompliancetype) 
7. See [:material-code-braces: TargetLocationOutputTypeDef](./type_defs.md#targetlocationoutputtypedef) 
8. See [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
9. See [:material-code-braces: AlarmStateInformationTypeDef](./type_defs.md#alarmstateinformationtypedef) 
## AssociationVersionInfoTypeDef

```python
# AssociationVersionInfoTypeDef definition

class AssociationVersionInfoTypeDef(TypedDict):
    AssociationId: NotRequired[str],
    AssociationVersion: NotRequired[str],
    CreatedDate: NotRequired[datetime],
    Name: NotRequired[str],
    DocumentVersion: NotRequired[str],
    Parameters: NotRequired[Dict[str, List[str]]],
    Targets: NotRequired[List[TargetOutputTypeDef]],  # (1)
    ScheduleExpression: NotRequired[str],
    OutputLocation: NotRequired[InstanceAssociationOutputLocationTypeDef],  # (2)
    AssociationName: NotRequired[str],
    MaxErrors: NotRequired[str],
    MaxConcurrency: NotRequired[str],
    ComplianceSeverity: NotRequired[AssociationComplianceSeverityType],  # (3)
    SyncCompliance: NotRequired[AssociationSyncComplianceType],  # (4)
    ApplyOnlyAtCronInterval: NotRequired[bool],
    CalendarNames: NotRequired[List[str]],
    TargetLocations: NotRequired[List[TargetLocationOutputTypeDef]],  # (5)
    ScheduleOffset: NotRequired[int],
    Duration: NotRequired[int],
    TargetMaps: NotRequired[List[Dict[str, List[str]]]],
```

1. See [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-braces: InstanceAssociationOutputLocationTypeDef](./type_defs.md#instanceassociationoutputlocationtypedef) 
3. See [:material-code-brackets: AssociationComplianceSeverityType](./literals.md#associationcomplianceseveritytype) 
4. See [:material-code-brackets: AssociationSyncComplianceType](./literals.md#associationsynccompliancetype) 
5. See [:material-code-braces: TargetLocationOutputTypeDef](./type_defs.md#targetlocationoutputtypedef) 
## CreateAssociationBatchRequestEntryOutputTypeDef

```python
# CreateAssociationBatchRequestEntryOutputTypeDef definition

class CreateAssociationBatchRequestEntryOutputTypeDef(TypedDict):
    Name: str,
    InstanceId: NotRequired[str],
    Parameters: NotRequired[Dict[str, List[str]]],
    AutomationTargetParameterName: NotRequired[str],
    DocumentVersion: NotRequired[str],
    Targets: NotRequired[List[TargetOutputTypeDef]],  # (1)
    ScheduleExpression: NotRequired[str],
    OutputLocation: NotRequired[InstanceAssociationOutputLocationTypeDef],  # (2)
    AssociationName: NotRequired[str],
    MaxErrors: NotRequired[str],
    MaxConcurrency: NotRequired[str],
    ComplianceSeverity: NotRequired[AssociationComplianceSeverityType],  # (3)
    SyncCompliance: NotRequired[AssociationSyncComplianceType],  # (4)
    ApplyOnlyAtCronInterval: NotRequired[bool],
    CalendarNames: NotRequired[List[str]],
    TargetLocations: NotRequired[List[TargetLocationOutputTypeDef]],  # (5)
    ScheduleOffset: NotRequired[int],
    Duration: NotRequired[int],
    TargetMaps: NotRequired[List[Dict[str, List[str]]]],
    AlarmConfiguration: NotRequired[AlarmConfigurationOutputTypeDef],  # (6)
```

1. See [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-braces: InstanceAssociationOutputLocationTypeDef](./type_defs.md#instanceassociationoutputlocationtypedef) 
3. See [:material-code-brackets: AssociationComplianceSeverityType](./literals.md#associationcomplianceseveritytype) 
4. See [:material-code-brackets: AssociationSyncComplianceType](./literals.md#associationsynccompliancetype) 
5. See [:material-code-braces: TargetLocationOutputTypeDef](./type_defs.md#targetlocationoutputtypedef) 
6. See [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
## RunbookOutputTypeDef

```python
# RunbookOutputTypeDef definition

class RunbookOutputTypeDef(TypedDict):
    DocumentName: str,
    DocumentVersion: NotRequired[str],
    Parameters: NotRequired[Dict[str, List[str]]],
    TargetParameterName: NotRequired[str],
    Targets: NotRequired[List[TargetOutputTypeDef]],  # (1)
    TargetMaps: NotRequired[List[Dict[str, List[str]]]],
    MaxConcurrency: NotRequired[str],
    MaxErrors: NotRequired[str],
    TargetLocations: NotRequired[List[TargetLocationOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-braces: TargetLocationOutputTypeDef](./type_defs.md#targetlocationoutputtypedef) 
## StepExecutionTypeDef

```python
# StepExecutionTypeDef definition

class StepExecutionTypeDef(TypedDict):
    StepName: NotRequired[str],
    Action: NotRequired[str],
    TimeoutSeconds: NotRequired[int],
    OnFailure: NotRequired[str],
    MaxAttempts: NotRequired[int],
    ExecutionStartTime: NotRequired[datetime],
    ExecutionEndTime: NotRequired[datetime],
    StepStatus: NotRequired[AutomationExecutionStatusType],  # (1)
    ResponseCode: NotRequired[str],
    Inputs: NotRequired[Dict[str, str]],
    Outputs: NotRequired[Dict[str, List[str]]],
    Response: NotRequired[str],
    FailureMessage: NotRequired[str],
    FailureDetails: NotRequired[FailureDetailsTypeDef],  # (2)
    StepExecutionId: NotRequired[str],
    OverriddenParameters: NotRequired[Dict[str, List[str]]],
    IsEnd: NotRequired[bool],
    NextStep: NotRequired[str],
    IsCritical: NotRequired[bool],
    ValidNextSteps: NotRequired[List[str]],
    Targets: NotRequired[List[TargetOutputTypeDef]],  # (3)
    TargetLocation: NotRequired[TargetLocationOutputTypeDef],  # (4)
    TriggeredAlarms: NotRequired[List[AlarmStateInformationTypeDef]],  # (5)
    ParentStepDetails: NotRequired[ParentStepDetailsTypeDef],  # (6)
```

1. See [:material-code-brackets: AutomationExecutionStatusType](./literals.md#automationexecutionstatustype) 
2. See [:material-code-braces: FailureDetailsTypeDef](./type_defs.md#failuredetailstypedef) 
3. See [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
4. See [:material-code-braces: TargetLocationOutputTypeDef](./type_defs.md#targetlocationoutputtypedef) 
5. See [:material-code-braces: AlarmStateInformationTypeDef](./type_defs.md#alarmstateinformationtypedef) 
6. See [:material-code-braces: ParentStepDetailsTypeDef](./type_defs.md#parentstepdetailstypedef) 
## TargetLocationTypeDef

```python
# TargetLocationTypeDef definition

class TargetLocationTypeDef(TypedDict):
    Accounts: NotRequired[Sequence[str]],
    Regions: NotRequired[Sequence[str]],
    TargetLocationMaxConcurrency: NotRequired[str],
    TargetLocationMaxErrors: NotRequired[str],
    ExecutionRoleName: NotRequired[str],
    TargetLocationAlarmConfiguration: NotRequired[AlarmConfigurationUnionTypeDef],  # (1)
    IncludeChildOrganizationUnits: NotRequired[bool],
    ExcludeAccounts: NotRequired[Sequence[str]],
    Targets: NotRequired[Sequence[TargetUnionTypeDef]],  # (2)
    TargetsMaxConcurrency: NotRequired[str],
    TargetsMaxErrors: NotRequired[str],
```

1. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
2. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
## GetMaintenanceWindowTaskResultTypeDef

```python
# GetMaintenanceWindowTaskResultTypeDef definition

class GetMaintenanceWindowTaskResultTypeDef(TypedDict):
    WindowId: str,
    WindowTaskId: str,
    Targets: List[TargetOutputTypeDef],  # (1)
    TaskArn: str,
    ServiceRoleArn: str,
    TaskType: MaintenanceWindowTaskTypeType,  # (2)
    TaskParameters: Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],  # (3)
    TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersOutputTypeDef,  # (4)
    Priority: int,
    MaxConcurrency: str,
    MaxErrors: str,
    LoggingInfo: LoggingInfoTypeDef,  # (5)
    Name: str,
    Description: str,
    CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType,  # (6)
    AlarmConfiguration: AlarmConfigurationOutputTypeDef,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-brackets: MaintenanceWindowTaskTypeType](./literals.md#maintenancewindowtasktypetype) 
3. See [:material-code-braces: MaintenanceWindowTaskParameterValueExpressionOutputTypeDef](./type_defs.md#maintenancewindowtaskparametervalueexpressionoutputtypedef) 
4. See [:material-code-braces: MaintenanceWindowTaskInvocationParametersOutputTypeDef](./type_defs.md#maintenancewindowtaskinvocationparametersoutputtypedef) 
5. See [:material-code-braces: LoggingInfoTypeDef](./type_defs.md#logginginfotypedef) 
6. See [:material-code-brackets: MaintenanceWindowTaskCutoffBehaviorType](./literals.md#maintenancewindowtaskcutoffbehaviortype) 
7. See [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMaintenanceWindowTaskResultTypeDef

```python
# UpdateMaintenanceWindowTaskResultTypeDef definition

class UpdateMaintenanceWindowTaskResultTypeDef(TypedDict):
    WindowId: str,
    WindowTaskId: str,
    Targets: List[TargetOutputTypeDef],  # (1)
    TaskArn: str,
    ServiceRoleArn: str,
    TaskParameters: Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],  # (2)
    TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersOutputTypeDef,  # (3)
    Priority: int,
    MaxConcurrency: str,
    MaxErrors: str,
    LoggingInfo: LoggingInfoTypeDef,  # (4)
    Name: str,
    Description: str,
    CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType,  # (5)
    AlarmConfiguration: AlarmConfigurationOutputTypeDef,  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-braces: MaintenanceWindowTaskParameterValueExpressionOutputTypeDef](./type_defs.md#maintenancewindowtaskparametervalueexpressionoutputtypedef) 
3. See [:material-code-braces: MaintenanceWindowTaskInvocationParametersOutputTypeDef](./type_defs.md#maintenancewindowtaskinvocationparametersoutputtypedef) 
4. See [:material-code-braces: LoggingInfoTypeDef](./type_defs.md#logginginfotypedef) 
5. See [:material-code-brackets: MaintenanceWindowTaskCutoffBehaviorType](./literals.md#maintenancewindowtaskcutoffbehaviortype) 
6. See [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListComplianceSummariesResultTypeDef

```python
# ListComplianceSummariesResultTypeDef definition

class ListComplianceSummariesResultTypeDef(TypedDict):
    ComplianceSummaryItems: List[ComplianceSummaryItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ComplianceSummaryItemTypeDef](./type_defs.md#compliancesummaryitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourceComplianceSummariesResultTypeDef

```python
# ListResourceComplianceSummariesResultTypeDef definition

class ListResourceComplianceSummariesResultTypeDef(TypedDict):
    ResourceComplianceSummaryItems: List[ResourceComplianceSummaryItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceComplianceSummaryItemTypeDef](./type_defs.md#resourcecompliancesummaryitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDocumentMetadataHistoryResponseTypeDef

```python
# ListDocumentMetadataHistoryResponseTypeDef definition

class ListDocumentMetadataHistoryResponseTypeDef(TypedDict):
    Name: str,
    DocumentVersion: str,
    Author: str,
    Metadata: DocumentMetadataResponseInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DocumentMetadataResponseInfoTypeDef](./type_defs.md#documentmetadataresponseinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInventoryRequestGetInventoryPaginateTypeDef

```python
# GetInventoryRequestGetInventoryPaginateTypeDef definition

class GetInventoryRequestGetInventoryPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[InventoryFilterTypeDef]],  # (1)
    Aggregators: NotRequired[Sequence[InventoryAggregatorPaginatorTypeDef]],  # (2)
    ResultAttributes: NotRequired[Sequence[ResultAttributeTypeDef]],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: InventoryFilterTypeDef](./type_defs.md#inventoryfiltertypedef) 
2. See [:material-code-braces: InventoryAggregatorPaginatorTypeDef](./type_defs.md#inventoryaggregatorpaginatortypedef) 
3. See [:material-code-braces: ResultAttributeTypeDef](./type_defs.md#resultattributetypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetInventoryRequestRequestTypeDef

```python
# GetInventoryRequestRequestTypeDef definition

class GetInventoryRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[InventoryFilterTypeDef]],  # (1)
    Aggregators: NotRequired[Sequence[InventoryAggregatorTypeDef]],  # (2)
    ResultAttributes: NotRequired[Sequence[ResultAttributeTypeDef]],  # (3)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: InventoryFilterTypeDef](./type_defs.md#inventoryfiltertypedef) 
2. See [:material-code-braces: InventoryAggregatorTypeDef](./type_defs.md#inventoryaggregatortypedef) 
3. See [:material-code-braces: ResultAttributeTypeDef](./type_defs.md#resultattributetypedef) 
## DescribeInstanceAssociationsStatusResultTypeDef

```python
# DescribeInstanceAssociationsStatusResultTypeDef definition

class DescribeInstanceAssociationsStatusResultTypeDef(TypedDict):
    InstanceAssociationStatusInfos: List[InstanceAssociationStatusInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InstanceAssociationStatusInfoTypeDef](./type_defs.md#instanceassociationstatusinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInventoryDeletionsResultTypeDef

```python
# DescribeInventoryDeletionsResultTypeDef definition

class DescribeInventoryDeletionsResultTypeDef(TypedDict):
    InventoryDeletions: List[InventoryDeletionStatusItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InventoryDeletionStatusItemTypeDef](./type_defs.md#inventorydeletionstatusitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PatchRuleGroupOutputTypeDef

```python
# PatchRuleGroupOutputTypeDef definition

class PatchRuleGroupOutputTypeDef(TypedDict):
    PatchRules: List[PatchRuleOutputTypeDef],  # (1)
```

1. See [:material-code-braces: PatchRuleOutputTypeDef](./type_defs.md#patchruleoutputtypedef) 
## ResourceDataSyncItemTypeDef

```python
# ResourceDataSyncItemTypeDef definition

class ResourceDataSyncItemTypeDef(TypedDict):
    SyncName: NotRequired[str],
    SyncType: NotRequired[str],
    SyncSource: NotRequired[ResourceDataSyncSourceWithStateTypeDef],  # (1)
    S3Destination: NotRequired[ResourceDataSyncS3DestinationTypeDef],  # (2)
    LastSyncTime: NotRequired[datetime],
    LastSuccessfulSyncTime: NotRequired[datetime],
    SyncLastModifiedTime: NotRequired[datetime],
    LastStatus: NotRequired[LastResourceDataSyncStatusType],  # (3)
    SyncCreatedTime: NotRequired[datetime],
    LastSyncStatusMessage: NotRequired[str],
```

1. See [:material-code-braces: ResourceDataSyncSourceWithStateTypeDef](./type_defs.md#resourcedatasyncsourcewithstatetypedef) 
2. See [:material-code-braces: ResourceDataSyncS3DestinationTypeDef](./type_defs.md#resourcedatasyncs3destinationtypedef) 
3. See [:material-code-brackets: LastResourceDataSyncStatusType](./literals.md#lastresourcedatasyncstatustype) 
## ResourceDataSyncSourceTypeDef

```python
# ResourceDataSyncSourceTypeDef definition

class ResourceDataSyncSourceTypeDef(TypedDict):
    SourceType: str,
    SourceRegions: Sequence[str],
    AwsOrganizationsSource: NotRequired[ResourceDataSyncAwsOrganizationsSourceUnionTypeDef],  # (1)
    IncludeFutureRegions: NotRequired[bool],
    EnableAllOpsDataSources: NotRequired[bool],
```

1. See [:material-code-braces: ResourceDataSyncAwsOrganizationsSourceTypeDef](./type_defs.md#resourcedatasyncawsorganizationssourcetypedef) [:material-code-braces: ResourceDataSyncAwsOrganizationsSourceOutputTypeDef](./type_defs.md#resourcedatasyncawsorganizationssourceoutputtypedef) 
## CreateAssociationResultTypeDef

```python
# CreateAssociationResultTypeDef definition

class CreateAssociationResultTypeDef(TypedDict):
    AssociationDescription: AssociationDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssociationDescriptionTypeDef](./type_defs.md#associationdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAssociationResultTypeDef

```python
# DescribeAssociationResultTypeDef definition

class DescribeAssociationResultTypeDef(TypedDict):
    AssociationDescription: AssociationDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssociationDescriptionTypeDef](./type_defs.md#associationdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAssociationResultTypeDef

```python
# UpdateAssociationResultTypeDef definition

class UpdateAssociationResultTypeDef(TypedDict):
    AssociationDescription: AssociationDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssociationDescriptionTypeDef](./type_defs.md#associationdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAssociationStatusResultTypeDef

```python
# UpdateAssociationStatusResultTypeDef definition

class UpdateAssociationStatusResultTypeDef(TypedDict):
    AssociationDescription: AssociationDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssociationDescriptionTypeDef](./type_defs.md#associationdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssociationVersionsResultTypeDef

```python
# ListAssociationVersionsResultTypeDef definition

class ListAssociationVersionsResultTypeDef(TypedDict):
    AssociationVersions: List[AssociationVersionInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AssociationVersionInfoTypeDef](./type_defs.md#associationversioninfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FailedCreateAssociationTypeDef

```python
# FailedCreateAssociationTypeDef definition

class FailedCreateAssociationTypeDef(TypedDict):
    Entry: NotRequired[CreateAssociationBatchRequestEntryOutputTypeDef],  # (1)
    Message: NotRequired[str],
    Fault: NotRequired[FaultType],  # (2)
```

1. See [:material-code-braces: CreateAssociationBatchRequestEntryOutputTypeDef](./type_defs.md#createassociationbatchrequestentryoutputtypedef) 
2. See [:material-code-brackets: FaultType](./literals.md#faulttype) 
## AutomationExecutionMetadataTypeDef

```python
# AutomationExecutionMetadataTypeDef definition

class AutomationExecutionMetadataTypeDef(TypedDict):
    AutomationExecutionId: NotRequired[str],
    DocumentName: NotRequired[str],
    DocumentVersion: NotRequired[str],
    AutomationExecutionStatus: NotRequired[AutomationExecutionStatusType],  # (1)
    ExecutionStartTime: NotRequired[datetime],
    ExecutionEndTime: NotRequired[datetime],
    ExecutedBy: NotRequired[str],
    LogFile: NotRequired[str],
    Outputs: NotRequired[Dict[str, List[str]]],
    Mode: NotRequired[ExecutionModeType],  # (2)
    ParentAutomationExecutionId: NotRequired[str],
    CurrentStepName: NotRequired[str],
    CurrentAction: NotRequired[str],
    FailureMessage: NotRequired[str],
    TargetParameterName: NotRequired[str],
    Targets: NotRequired[List[TargetOutputTypeDef]],  # (3)
    TargetMaps: NotRequired[List[Dict[str, List[str]]]],
    ResolvedTargets: NotRequired[ResolvedTargetsTypeDef],  # (4)
    MaxConcurrency: NotRequired[str],
    MaxErrors: NotRequired[str],
    Target: NotRequired[str],
    AutomationType: NotRequired[AutomationTypeType],  # (5)
    AlarmConfiguration: NotRequired[AlarmConfigurationOutputTypeDef],  # (6)
    TriggeredAlarms: NotRequired[List[AlarmStateInformationTypeDef]],  # (7)
    TargetLocationsURL: NotRequired[str],
    AutomationSubtype: NotRequired[AutomationSubtypeType],  # (8)
    ScheduledTime: NotRequired[datetime],
    Runbooks: NotRequired[List[RunbookOutputTypeDef]],  # (9)
    OpsItemId: NotRequired[str],
    AssociationId: NotRequired[str],
    ChangeRequestName: NotRequired[str],
```

1. See [:material-code-brackets: AutomationExecutionStatusType](./literals.md#automationexecutionstatustype) 
2. See [:material-code-brackets: ExecutionModeType](./literals.md#executionmodetype) 
3. See [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
4. See [:material-code-braces: ResolvedTargetsTypeDef](./type_defs.md#resolvedtargetstypedef) 
5. See [:material-code-brackets: AutomationTypeType](./literals.md#automationtypetype) 
6. See [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
7. See [:material-code-braces: AlarmStateInformationTypeDef](./type_defs.md#alarmstateinformationtypedef) 
8. See [:material-code-brackets: AutomationSubtypeType](./literals.md#automationsubtypetype) 
9. See [:material-code-braces: RunbookOutputTypeDef](./type_defs.md#runbookoutputtypedef) 
## AutomationExecutionTypeDef

```python
# AutomationExecutionTypeDef definition

class AutomationExecutionTypeDef(TypedDict):
    AutomationExecutionId: NotRequired[str],
    DocumentName: NotRequired[str],
    DocumentVersion: NotRequired[str],
    ExecutionStartTime: NotRequired[datetime],
    ExecutionEndTime: NotRequired[datetime],
    AutomationExecutionStatus: NotRequired[AutomationExecutionStatusType],  # (1)
    StepExecutions: NotRequired[List[StepExecutionTypeDef]],  # (2)
    StepExecutionsTruncated: NotRequired[bool],
    Parameters: NotRequired[Dict[str, List[str]]],
    Outputs: NotRequired[Dict[str, List[str]]],
    FailureMessage: NotRequired[str],
    Mode: NotRequired[ExecutionModeType],  # (3)
    ParentAutomationExecutionId: NotRequired[str],
    ExecutedBy: NotRequired[str],
    CurrentStepName: NotRequired[str],
    CurrentAction: NotRequired[str],
    TargetParameterName: NotRequired[str],
    Targets: NotRequired[List[TargetOutputTypeDef]],  # (4)
    TargetMaps: NotRequired[List[Dict[str, List[str]]]],
    ResolvedTargets: NotRequired[ResolvedTargetsTypeDef],  # (5)
    MaxConcurrency: NotRequired[str],
    MaxErrors: NotRequired[str],
    Target: NotRequired[str],
    TargetLocations: NotRequired[List[TargetLocationOutputTypeDef]],  # (6)
    ProgressCounters: NotRequired[ProgressCountersTypeDef],  # (7)
    AlarmConfiguration: NotRequired[AlarmConfigurationOutputTypeDef],  # (8)
    TriggeredAlarms: NotRequired[List[AlarmStateInformationTypeDef]],  # (9)
    TargetLocationsURL: NotRequired[str],
    AutomationSubtype: NotRequired[AutomationSubtypeType],  # (10)
    ScheduledTime: NotRequired[datetime],
    Runbooks: NotRequired[List[RunbookOutputTypeDef]],  # (11)
    OpsItemId: NotRequired[str],
    AssociationId: NotRequired[str],
    ChangeRequestName: NotRequired[str],
    Variables: NotRequired[Dict[str, List[str]]],
```

1. See [:material-code-brackets: AutomationExecutionStatusType](./literals.md#automationexecutionstatustype) 
2. See [:material-code-braces: StepExecutionTypeDef](./type_defs.md#stepexecutiontypedef) 
3. See [:material-code-brackets: ExecutionModeType](./literals.md#executionmodetype) 
4. See [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
5. See [:material-code-braces: ResolvedTargetsTypeDef](./type_defs.md#resolvedtargetstypedef) 
6. See [:material-code-braces: TargetLocationOutputTypeDef](./type_defs.md#targetlocationoutputtypedef) 
7. See [:material-code-braces: ProgressCountersTypeDef](./type_defs.md#progresscounterstypedef) 
8. See [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
9. See [:material-code-braces: AlarmStateInformationTypeDef](./type_defs.md#alarmstateinformationtypedef) 
10. See [:material-code-brackets: AutomationSubtypeType](./literals.md#automationsubtypetype) 
11. See [:material-code-braces: RunbookOutputTypeDef](./type_defs.md#runbookoutputtypedef) 
## DescribeAutomationStepExecutionsResultTypeDef

```python
# DescribeAutomationStepExecutionsResultTypeDef definition

class DescribeAutomationStepExecutionsResultTypeDef(TypedDict):
    StepExecutions: List[StepExecutionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: StepExecutionTypeDef](./type_defs.md#stepexecutiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartAutomationExecutionRequestRequestTypeDef

```python
# StartAutomationExecutionRequestRequestTypeDef definition

class StartAutomationExecutionRequestRequestTypeDef(TypedDict):
    DocumentName: str,
    DocumentVersion: NotRequired[str],
    Parameters: NotRequired[Mapping[str, Sequence[str]]],
    ClientToken: NotRequired[str],
    Mode: NotRequired[ExecutionModeType],  # (1)
    TargetParameterName: NotRequired[str],
    Targets: NotRequired[Sequence[TargetTypeDef]],  # (2)
    TargetMaps: NotRequired[Sequence[Mapping[str, Sequence[str]]]],
    MaxConcurrency: NotRequired[str],
    MaxErrors: NotRequired[str],
    TargetLocations: NotRequired[Sequence[TargetLocationTypeDef]],  # (3)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    AlarmConfiguration: NotRequired[AlarmConfigurationTypeDef],  # (5)
    TargetLocationsURL: NotRequired[str],
```

1. See [:material-code-brackets: ExecutionModeType](./literals.md#executionmodetype) 
2. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
3. See [:material-code-braces: TargetLocationTypeDef](./type_defs.md#targetlocationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) 
## UpdateAssociationRequestRequestTypeDef

```python
# UpdateAssociationRequestRequestTypeDef definition

class UpdateAssociationRequestRequestTypeDef(TypedDict):
    AssociationId: str,
    Parameters: NotRequired[Mapping[str, Sequence[str]]],
    DocumentVersion: NotRequired[str],
    ScheduleExpression: NotRequired[str],
    OutputLocation: NotRequired[InstanceAssociationOutputLocationTypeDef],  # (1)
    Name: NotRequired[str],
    Targets: NotRequired[Sequence[TargetTypeDef]],  # (2)
    AssociationName: NotRequired[str],
    AssociationVersion: NotRequired[str],
    AutomationTargetParameterName: NotRequired[str],
    MaxErrors: NotRequired[str],
    MaxConcurrency: NotRequired[str],
    ComplianceSeverity: NotRequired[AssociationComplianceSeverityType],  # (3)
    SyncCompliance: NotRequired[AssociationSyncComplianceType],  # (4)
    ApplyOnlyAtCronInterval: NotRequired[bool],
    CalendarNames: NotRequired[Sequence[str]],
    TargetLocations: NotRequired[Sequence[TargetLocationTypeDef]],  # (5)
    ScheduleOffset: NotRequired[int],
    Duration: NotRequired[int],
    TargetMaps: NotRequired[Sequence[Mapping[str, Sequence[str]]]],
    AlarmConfiguration: NotRequired[AlarmConfigurationTypeDef],  # (6)
```

1. See [:material-code-braces: InstanceAssociationOutputLocationTypeDef](./type_defs.md#instanceassociationoutputlocationtypedef) 
2. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
3. See [:material-code-brackets: AssociationComplianceSeverityType](./literals.md#associationcomplianceseveritytype) 
4. See [:material-code-brackets: AssociationSyncComplianceType](./literals.md#associationsynccompliancetype) 
5. See [:material-code-braces: TargetLocationTypeDef](./type_defs.md#targetlocationtypedef) 
6. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) 
## MaintenanceWindowTaskInvocationParametersTypeDef

```python
# MaintenanceWindowTaskInvocationParametersTypeDef definition

class MaintenanceWindowTaskInvocationParametersTypeDef(TypedDict):
    RunCommand: NotRequired[MaintenanceWindowRunCommandParametersUnionTypeDef],  # (1)
    Automation: NotRequired[MaintenanceWindowAutomationParametersUnionTypeDef],  # (2)
    StepFunctions: NotRequired[MaintenanceWindowStepFunctionsParametersTypeDef],  # (3)
    Lambda: NotRequired[MaintenanceWindowLambdaParametersUnionTypeDef],  # (4)
```

1. See [:material-code-braces: MaintenanceWindowRunCommandParametersTypeDef](./type_defs.md#maintenancewindowruncommandparameterstypedef) [:material-code-braces: MaintenanceWindowRunCommandParametersOutputTypeDef](./type_defs.md#maintenancewindowruncommandparametersoutputtypedef) 
2. See [:material-code-braces: MaintenanceWindowAutomationParametersTypeDef](./type_defs.md#maintenancewindowautomationparameterstypedef) [:material-code-braces: MaintenanceWindowAutomationParametersOutputTypeDef](./type_defs.md#maintenancewindowautomationparametersoutputtypedef) 
3. See [:material-code-braces: MaintenanceWindowStepFunctionsParametersTypeDef](./type_defs.md#maintenancewindowstepfunctionsparameterstypedef) 
4. See [:material-code-braces: MaintenanceWindowLambdaParametersTypeDef](./type_defs.md#maintenancewindowlambdaparameterstypedef) [:material-code-braces: MaintenanceWindowLambdaParametersOutputTypeDef](./type_defs.md#maintenancewindowlambdaparametersoutputtypedef) 
## GetPatchBaselineResultTypeDef

```python
# GetPatchBaselineResultTypeDef definition

class GetPatchBaselineResultTypeDef(TypedDict):
    BaselineId: str,
    Name: str,
    OperatingSystem: OperatingSystemType,  # (1)
    GlobalFilters: PatchFilterGroupOutputTypeDef,  # (2)
    ApprovalRules: PatchRuleGroupOutputTypeDef,  # (3)
    ApprovedPatches: List[str],
    ApprovedPatchesComplianceLevel: PatchComplianceLevelType,  # (4)
    ApprovedPatchesEnableNonSecurity: bool,
    RejectedPatches: List[str],
    RejectedPatchesAction: PatchActionType,  # (5)
    PatchGroups: List[str],
    CreatedDate: datetime,
    ModifiedDate: datetime,
    Description: str,
    Sources: List[PatchSourceOutputTypeDef],  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
2. See [:material-code-braces: PatchFilterGroupOutputTypeDef](./type_defs.md#patchfiltergroupoutputtypedef) 
3. See [:material-code-braces: PatchRuleGroupOutputTypeDef](./type_defs.md#patchrulegroupoutputtypedef) 
4. See [:material-code-brackets: PatchComplianceLevelType](./literals.md#patchcomplianceleveltype) 
5. See [:material-code-brackets: PatchActionType](./literals.md#patchactiontype) 
6. See [:material-code-braces: PatchSourceOutputTypeDef](./type_defs.md#patchsourceoutputtypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePatchBaselineResultTypeDef

```python
# UpdatePatchBaselineResultTypeDef definition

class UpdatePatchBaselineResultTypeDef(TypedDict):
    BaselineId: str,
    Name: str,
    OperatingSystem: OperatingSystemType,  # (1)
    GlobalFilters: PatchFilterGroupOutputTypeDef,  # (2)
    ApprovalRules: PatchRuleGroupOutputTypeDef,  # (3)
    ApprovedPatches: List[str],
    ApprovedPatchesComplianceLevel: PatchComplianceLevelType,  # (4)
    ApprovedPatchesEnableNonSecurity: bool,
    RejectedPatches: List[str],
    RejectedPatchesAction: PatchActionType,  # (5)
    CreatedDate: datetime,
    ModifiedDate: datetime,
    Description: str,
    Sources: List[PatchSourceOutputTypeDef],  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
2. See [:material-code-braces: PatchFilterGroupOutputTypeDef](./type_defs.md#patchfiltergroupoutputtypedef) 
3. See [:material-code-braces: PatchRuleGroupOutputTypeDef](./type_defs.md#patchrulegroupoutputtypedef) 
4. See [:material-code-brackets: PatchComplianceLevelType](./literals.md#patchcomplianceleveltype) 
5. See [:material-code-brackets: PatchActionType](./literals.md#patchactiontype) 
6. See [:material-code-braces: PatchSourceOutputTypeDef](./type_defs.md#patchsourceoutputtypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PatchRuleTypeDef

```python
# PatchRuleTypeDef definition

class PatchRuleTypeDef(TypedDict):
    PatchFilterGroup: PatchFilterGroupUnionTypeDef,  # (1)
    ComplianceLevel: NotRequired[PatchComplianceLevelType],  # (2)
    ApproveAfterDays: NotRequired[int],
    ApproveUntilDate: NotRequired[str],
    EnableNonSecurity: NotRequired[bool],
```

1. See [:material-code-braces: PatchFilterGroupTypeDef](./type_defs.md#patchfiltergrouptypedef) [:material-code-braces: PatchFilterGroupOutputTypeDef](./type_defs.md#patchfiltergroupoutputtypedef) 
2. See [:material-code-brackets: PatchComplianceLevelType](./literals.md#patchcomplianceleveltype) 
## ListResourceDataSyncResultTypeDef

```python
# ListResourceDataSyncResultTypeDef definition

class ListResourceDataSyncResultTypeDef(TypedDict):
    ResourceDataSyncItems: List[ResourceDataSyncItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceDataSyncItemTypeDef](./type_defs.md#resourcedatasyncitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateResourceDataSyncRequestRequestTypeDef

```python
# CreateResourceDataSyncRequestRequestTypeDef definition

class CreateResourceDataSyncRequestRequestTypeDef(TypedDict):
    SyncName: str,
    S3Destination: NotRequired[ResourceDataSyncS3DestinationTypeDef],  # (1)
    SyncType: NotRequired[str],
    SyncSource: NotRequired[ResourceDataSyncSourceTypeDef],  # (2)
```

1. See [:material-code-braces: ResourceDataSyncS3DestinationTypeDef](./type_defs.md#resourcedatasyncs3destinationtypedef) 
2. See [:material-code-braces: ResourceDataSyncSourceTypeDef](./type_defs.md#resourcedatasyncsourcetypedef) 
## UpdateResourceDataSyncRequestRequestTypeDef

```python
# UpdateResourceDataSyncRequestRequestTypeDef definition

class UpdateResourceDataSyncRequestRequestTypeDef(TypedDict):
    SyncName: str,
    SyncType: str,
    SyncSource: ResourceDataSyncSourceTypeDef,  # (1)
```

1. See [:material-code-braces: ResourceDataSyncSourceTypeDef](./type_defs.md#resourcedatasyncsourcetypedef) 
## CreateAssociationBatchResultTypeDef

```python
# CreateAssociationBatchResultTypeDef definition

class CreateAssociationBatchResultTypeDef(TypedDict):
    Successful: List[AssociationDescriptionTypeDef],  # (1)
    Failed: List[FailedCreateAssociationTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AssociationDescriptionTypeDef](./type_defs.md#associationdescriptiontypedef) 
2. See [:material-code-braces: FailedCreateAssociationTypeDef](./type_defs.md#failedcreateassociationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAutomationExecutionsResultTypeDef

```python
# DescribeAutomationExecutionsResultTypeDef definition

class DescribeAutomationExecutionsResultTypeDef(TypedDict):
    AutomationExecutionMetadataList: List[AutomationExecutionMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AutomationExecutionMetadataTypeDef](./type_defs.md#automationexecutionmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAutomationExecutionResultTypeDef

```python
# GetAutomationExecutionResultTypeDef definition

class GetAutomationExecutionResultTypeDef(TypedDict):
    AutomationExecution: AutomationExecutionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AutomationExecutionTypeDef](./type_defs.md#automationexecutiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAssociationBatchRequestEntryTypeDef

```python
# CreateAssociationBatchRequestEntryTypeDef definition

class CreateAssociationBatchRequestEntryTypeDef(TypedDict):
    Name: str,
    InstanceId: NotRequired[str],
    Parameters: NotRequired[Mapping[str, Sequence[str]]],
    AutomationTargetParameterName: NotRequired[str],
    DocumentVersion: NotRequired[str],
    Targets: NotRequired[Sequence[TargetUnionTypeDef]],  # (1)
    ScheduleExpression: NotRequired[str],
    OutputLocation: NotRequired[InstanceAssociationOutputLocationTypeDef],  # (2)
    AssociationName: NotRequired[str],
    MaxErrors: NotRequired[str],
    MaxConcurrency: NotRequired[str],
    ComplianceSeverity: NotRequired[AssociationComplianceSeverityType],  # (3)
    SyncCompliance: NotRequired[AssociationSyncComplianceType],  # (4)
    ApplyOnlyAtCronInterval: NotRequired[bool],
    CalendarNames: NotRequired[Sequence[str]],
    TargetLocations: NotRequired[Sequence[TargetLocationUnionTypeDef]],  # (5)
    ScheduleOffset: NotRequired[int],
    Duration: NotRequired[int],
    TargetMaps: NotRequired[Sequence[Mapping[str, Sequence[str]]]],
    AlarmConfiguration: NotRequired[AlarmConfigurationUnionTypeDef],  # (6)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-braces: InstanceAssociationOutputLocationTypeDef](./type_defs.md#instanceassociationoutputlocationtypedef) 
3. See [:material-code-brackets: AssociationComplianceSeverityType](./literals.md#associationcomplianceseveritytype) 
4. See [:material-code-brackets: AssociationSyncComplianceType](./literals.md#associationsynccompliancetype) 
5. See [:material-code-braces: TargetLocationTypeDef](./type_defs.md#targetlocationtypedef) [:material-code-braces: TargetLocationOutputTypeDef](./type_defs.md#targetlocationoutputtypedef) 
6. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
## CreateAssociationRequestRequestTypeDef

```python
# CreateAssociationRequestRequestTypeDef definition

class CreateAssociationRequestRequestTypeDef(TypedDict):
    Name: str,
    DocumentVersion: NotRequired[str],
    InstanceId: NotRequired[str],
    Parameters: NotRequired[Mapping[str, Sequence[str]]],
    Targets: NotRequired[Sequence[TargetUnionTypeDef]],  # (1)
    ScheduleExpression: NotRequired[str],
    OutputLocation: NotRequired[InstanceAssociationOutputLocationTypeDef],  # (2)
    AssociationName: NotRequired[str],
    AutomationTargetParameterName: NotRequired[str],
    MaxErrors: NotRequired[str],
    MaxConcurrency: NotRequired[str],
    ComplianceSeverity: NotRequired[AssociationComplianceSeverityType],  # (3)
    SyncCompliance: NotRequired[AssociationSyncComplianceType],  # (4)
    ApplyOnlyAtCronInterval: NotRequired[bool],
    CalendarNames: NotRequired[Sequence[str]],
    TargetLocations: NotRequired[Sequence[TargetLocationUnionTypeDef]],  # (5)
    ScheduleOffset: NotRequired[int],
    Duration: NotRequired[int],
    TargetMaps: NotRequired[Sequence[Mapping[str, Sequence[str]]]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (6)
    AlarmConfiguration: NotRequired[AlarmConfigurationTypeDef],  # (7)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-braces: InstanceAssociationOutputLocationTypeDef](./type_defs.md#instanceassociationoutputlocationtypedef) 
3. See [:material-code-brackets: AssociationComplianceSeverityType](./literals.md#associationcomplianceseveritytype) 
4. See [:material-code-brackets: AssociationSyncComplianceType](./literals.md#associationsynccompliancetype) 
5. See [:material-code-braces: TargetLocationTypeDef](./type_defs.md#targetlocationtypedef) [:material-code-braces: TargetLocationOutputTypeDef](./type_defs.md#targetlocationoutputtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) 
## RunbookTypeDef

```python
# RunbookTypeDef definition

class RunbookTypeDef(TypedDict):
    DocumentName: str,
    DocumentVersion: NotRequired[str],
    Parameters: NotRequired[Mapping[str, Sequence[str]]],
    TargetParameterName: NotRequired[str],
    Targets: NotRequired[Sequence[TargetUnionTypeDef]],  # (1)
    TargetMaps: NotRequired[Sequence[Mapping[str, Sequence[str]]]],
    MaxConcurrency: NotRequired[str],
    MaxErrors: NotRequired[str],
    TargetLocations: NotRequired[Sequence[TargetLocationUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-braces: TargetLocationTypeDef](./type_defs.md#targetlocationtypedef) [:material-code-braces: TargetLocationOutputTypeDef](./type_defs.md#targetlocationoutputtypedef) 
## RegisterTaskWithMaintenanceWindowRequestRequestTypeDef

```python
# RegisterTaskWithMaintenanceWindowRequestRequestTypeDef definition

class RegisterTaskWithMaintenanceWindowRequestRequestTypeDef(TypedDict):
    WindowId: str,
    TaskArn: str,
    TaskType: MaintenanceWindowTaskTypeType,  # (1)
    Targets: NotRequired[Sequence[TargetTypeDef]],  # (2)
    ServiceRoleArn: NotRequired[str],
    TaskParameters: NotRequired[Mapping[str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef]],  # (3)
    TaskInvocationParameters: NotRequired[MaintenanceWindowTaskInvocationParametersTypeDef],  # (4)
    Priority: NotRequired[int],
    MaxConcurrency: NotRequired[str],
    MaxErrors: NotRequired[str],
    LoggingInfo: NotRequired[LoggingInfoTypeDef],  # (5)
    Name: NotRequired[str],
    Description: NotRequired[str],
    ClientToken: NotRequired[str],
    CutoffBehavior: NotRequired[MaintenanceWindowTaskCutoffBehaviorType],  # (6)
    AlarmConfiguration: NotRequired[AlarmConfigurationTypeDef],  # (7)
```

1. See [:material-code-brackets: MaintenanceWindowTaskTypeType](./literals.md#maintenancewindowtasktypetype) 
2. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
3. See [:material-code-braces: MaintenanceWindowTaskParameterValueExpressionTypeDef](./type_defs.md#maintenancewindowtaskparametervalueexpressiontypedef) [:material-code-braces: MaintenanceWindowTaskParameterValueExpressionOutputTypeDef](./type_defs.md#maintenancewindowtaskparametervalueexpressionoutputtypedef) 
4. See [:material-code-braces: MaintenanceWindowTaskInvocationParametersTypeDef](./type_defs.md#maintenancewindowtaskinvocationparameterstypedef) 
5. See [:material-code-braces: LoggingInfoTypeDef](./type_defs.md#logginginfotypedef) 
6. See [:material-code-brackets: MaintenanceWindowTaskCutoffBehaviorType](./literals.md#maintenancewindowtaskcutoffbehaviortype) 
7. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) 
## UpdateMaintenanceWindowTaskRequestRequestTypeDef

```python
# UpdateMaintenanceWindowTaskRequestRequestTypeDef definition

class UpdateMaintenanceWindowTaskRequestRequestTypeDef(TypedDict):
    WindowId: str,
    WindowTaskId: str,
    Targets: NotRequired[Sequence[TargetTypeDef]],  # (1)
    TaskArn: NotRequired[str],
    ServiceRoleArn: NotRequired[str],
    TaskParameters: NotRequired[Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef]],  # (2)
    TaskInvocationParameters: NotRequired[MaintenanceWindowTaskInvocationParametersTypeDef],  # (3)
    Priority: NotRequired[int],
    MaxConcurrency: NotRequired[str],
    MaxErrors: NotRequired[str],
    LoggingInfo: NotRequired[LoggingInfoTypeDef],  # (4)
    Name: NotRequired[str],
    Description: NotRequired[str],
    Replace: NotRequired[bool],
    CutoffBehavior: NotRequired[MaintenanceWindowTaskCutoffBehaviorType],  # (5)
    AlarmConfiguration: NotRequired[AlarmConfigurationTypeDef],  # (6)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
2. See [:material-code-braces: MaintenanceWindowTaskParameterValueExpressionTypeDef](./type_defs.md#maintenancewindowtaskparametervalueexpressiontypedef) 
3. See [:material-code-braces: MaintenanceWindowTaskInvocationParametersTypeDef](./type_defs.md#maintenancewindowtaskinvocationparameterstypedef) 
4. See [:material-code-braces: LoggingInfoTypeDef](./type_defs.md#logginginfotypedef) 
5. See [:material-code-brackets: MaintenanceWindowTaskCutoffBehaviorType](./literals.md#maintenancewindowtaskcutoffbehaviortype) 
6. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) 
## PatchRuleGroupTypeDef

```python
# PatchRuleGroupTypeDef definition

class PatchRuleGroupTypeDef(TypedDict):
    PatchRules: Sequence[PatchRuleUnionTypeDef],  # (1)
```

1. See [:material-code-braces: PatchRuleTypeDef](./type_defs.md#patchruletypedef) [:material-code-braces: PatchRuleOutputTypeDef](./type_defs.md#patchruleoutputtypedef) 
## CreateAssociationBatchRequestRequestTypeDef

```python
# CreateAssociationBatchRequestRequestTypeDef definition

class CreateAssociationBatchRequestRequestTypeDef(TypedDict):
    Entries: Sequence[CreateAssociationBatchRequestEntryUnionTypeDef],  # (1)
```

1. See [:material-code-braces: CreateAssociationBatchRequestEntryTypeDef](./type_defs.md#createassociationbatchrequestentrytypedef) [:material-code-braces: CreateAssociationBatchRequestEntryOutputTypeDef](./type_defs.md#createassociationbatchrequestentryoutputtypedef) 
## StartChangeRequestExecutionRequestRequestTypeDef

```python
# StartChangeRequestExecutionRequestRequestTypeDef definition

class StartChangeRequestExecutionRequestRequestTypeDef(TypedDict):
    DocumentName: str,
    Runbooks: Sequence[RunbookUnionTypeDef],  # (1)
    ScheduledTime: NotRequired[TimestampTypeDef],
    DocumentVersion: NotRequired[str],
    Parameters: NotRequired[Mapping[str, Sequence[str]]],
    ChangeRequestName: NotRequired[str],
    ClientToken: NotRequired[str],
    AutoApprove: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    ScheduledEndTime: NotRequired[TimestampTypeDef],
    ChangeDetails: NotRequired[str],
```

1. See [:material-code-braces: RunbookTypeDef](./type_defs.md#runbooktypedef) [:material-code-braces: RunbookOutputTypeDef](./type_defs.md#runbookoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePatchBaselineRequestRequestTypeDef

```python
# CreatePatchBaselineRequestRequestTypeDef definition

class CreatePatchBaselineRequestRequestTypeDef(TypedDict):
    Name: str,
    OperatingSystem: NotRequired[OperatingSystemType],  # (1)
    GlobalFilters: NotRequired[PatchFilterGroupTypeDef],  # (2)
    ApprovalRules: NotRequired[PatchRuleGroupTypeDef],  # (3)
    ApprovedPatches: NotRequired[Sequence[str]],
    ApprovedPatchesComplianceLevel: NotRequired[PatchComplianceLevelType],  # (4)
    ApprovedPatchesEnableNonSecurity: NotRequired[bool],
    RejectedPatches: NotRequired[Sequence[str]],
    RejectedPatchesAction: NotRequired[PatchActionType],  # (5)
    Description: NotRequired[str],
    Sources: NotRequired[Sequence[PatchSourceUnionTypeDef]],  # (6)
    ClientToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (7)
```

1. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
2. See [:material-code-braces: PatchFilterGroupTypeDef](./type_defs.md#patchfiltergrouptypedef) 
3. See [:material-code-braces: PatchRuleGroupTypeDef](./type_defs.md#patchrulegrouptypedef) 
4. See [:material-code-brackets: PatchComplianceLevelType](./literals.md#patchcomplianceleveltype) 
5. See [:material-code-brackets: PatchActionType](./literals.md#patchactiontype) 
6. See [:material-code-braces: PatchSourceTypeDef](./type_defs.md#patchsourcetypedef) [:material-code-braces: PatchSourceOutputTypeDef](./type_defs.md#patchsourceoutputtypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdatePatchBaselineRequestRequestTypeDef

```python
# UpdatePatchBaselineRequestRequestTypeDef definition

class UpdatePatchBaselineRequestRequestTypeDef(TypedDict):
    BaselineId: str,
    Name: NotRequired[str],
    GlobalFilters: NotRequired[PatchFilterGroupTypeDef],  # (1)
    ApprovalRules: NotRequired[PatchRuleGroupTypeDef],  # (2)
    ApprovedPatches: NotRequired[Sequence[str]],
    ApprovedPatchesComplianceLevel: NotRequired[PatchComplianceLevelType],  # (3)
    ApprovedPatchesEnableNonSecurity: NotRequired[bool],
    RejectedPatches: NotRequired[Sequence[str]],
    RejectedPatchesAction: NotRequired[PatchActionType],  # (4)
    Description: NotRequired[str],
    Sources: NotRequired[Sequence[PatchSourceTypeDef]],  # (5)
    Replace: NotRequired[bool],
```

1. See [:material-code-braces: PatchFilterGroupTypeDef](./type_defs.md#patchfiltergrouptypedef) 
2. See [:material-code-braces: PatchRuleGroupTypeDef](./type_defs.md#patchrulegrouptypedef) 
3. See [:material-code-brackets: PatchComplianceLevelType](./literals.md#patchcomplianceleveltype) 
4. See [:material-code-brackets: PatchActionType](./literals.md#patchactiontype) 
5. See [:material-code-braces: PatchSourceTypeDef](./type_defs.md#patchsourcetypedef) 
## BaselineOverrideTypeDef

```python
# BaselineOverrideTypeDef definition

class BaselineOverrideTypeDef(TypedDict):
    OperatingSystem: NotRequired[OperatingSystemType],  # (1)
    GlobalFilters: NotRequired[PatchFilterGroupUnionTypeDef],  # (2)
    ApprovalRules: NotRequired[PatchRuleGroupUnionTypeDef],  # (3)
    ApprovedPatches: NotRequired[Sequence[str]],
    ApprovedPatchesComplianceLevel: NotRequired[PatchComplianceLevelType],  # (4)
    RejectedPatches: NotRequired[Sequence[str]],
    RejectedPatchesAction: NotRequired[PatchActionType],  # (5)
    ApprovedPatchesEnableNonSecurity: NotRequired[bool],
    Sources: NotRequired[Sequence[PatchSourceUnionTypeDef]],  # (6)
```

1. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
2. See [:material-code-braces: PatchFilterGroupTypeDef](./type_defs.md#patchfiltergrouptypedef) [:material-code-braces: PatchFilterGroupOutputTypeDef](./type_defs.md#patchfiltergroupoutputtypedef) 
3. See [:material-code-braces: PatchRuleGroupTypeDef](./type_defs.md#patchrulegrouptypedef) [:material-code-braces: PatchRuleGroupOutputTypeDef](./type_defs.md#patchrulegroupoutputtypedef) 
4. See [:material-code-brackets: PatchComplianceLevelType](./literals.md#patchcomplianceleveltype) 
5. See [:material-code-brackets: PatchActionType](./literals.md#patchactiontype) 
6. See [:material-code-braces: PatchSourceTypeDef](./type_defs.md#patchsourcetypedef) [:material-code-braces: PatchSourceOutputTypeDef](./type_defs.md#patchsourceoutputtypedef) 
## GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef

```python
# GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef definition

class GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    SnapshotId: str,
    BaselineOverride: NotRequired[BaselineOverrideTypeDef],  # (1)
```

1. See [:material-code-braces: BaselineOverrideTypeDef](./type_defs.md#baselineoverridetypedef) 
