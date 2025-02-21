# Type definitions

> [Index](../README.md) > [SSM](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SSM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#ssm)
    type annotations stubs module [types-aiobotocore-ssm](https://pypi.org/project/types-aiobotocore-ssm/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_ssm.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_ssm.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## NotificationConfigUnionTypeDef

```python
# NotificationConfigUnionTypeDef Union usage example

from types_aiobotocore_ssm.type_defs import NotificationConfigUnionTypeDef


def get_value() -> NotificationConfigUnionTypeDef:
    return ...


# NotificationConfigUnionTypeDef definition

NotificationConfigUnionTypeDef = Union[
    NotificationConfigTypeDef,  # (1)
    NotificationConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NotificationConfigTypeDef](./type_defs.md#notificationconfigtypedef) 
2. See [:material-code-braces: NotificationConfigOutputTypeDef](./type_defs.md#notificationconfigoutputtypedef) 

## MaintenanceWindowTaskParameterValueExpressionUnionTypeDef

```python
# MaintenanceWindowTaskParameterValueExpressionUnionTypeDef Union usage example

from types_aiobotocore_ssm.type_defs import MaintenanceWindowTaskParameterValueExpressionUnionTypeDef


def get_value() -> MaintenanceWindowTaskParameterValueExpressionUnionTypeDef:
    return ...


# MaintenanceWindowTaskParameterValueExpressionUnionTypeDef definition

MaintenanceWindowTaskParameterValueExpressionUnionTypeDef = Union[
    MaintenanceWindowTaskParameterValueExpressionTypeDef,  # (1)
    MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MaintenanceWindowTaskParameterValueExpressionTypeDef](./type_defs.md#maintenancewindowtaskparametervalueexpressiontypedef) 
2. See [:material-code-braces: MaintenanceWindowTaskParameterValueExpressionOutputTypeDef](./type_defs.md#maintenancewindowtaskparametervalueexpressionoutputtypedef) 

## PatchFilterUnionTypeDef

```python
# PatchFilterUnionTypeDef Union usage example

from types_aiobotocore_ssm.type_defs import PatchFilterUnionTypeDef


def get_value() -> PatchFilterUnionTypeDef:
    return ...


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
# PatchSourceUnionTypeDef Union usage example

from types_aiobotocore_ssm.type_defs import PatchSourceUnionTypeDef


def get_value() -> PatchSourceUnionTypeDef:
    return ...


# PatchSourceUnionTypeDef definition

PatchSourceUnionTypeDef = Union[
    PatchSourceTypeDef,  # (1)
    PatchSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PatchSourceTypeDef](./type_defs.md#patchsourcetypedef) 
2. See [:material-code-braces: PatchSourceOutputTypeDef](./type_defs.md#patchsourceoutputtypedef) 

## TargetUnionTypeDef

```python
# TargetUnionTypeDef Union usage example

from types_aiobotocore_ssm.type_defs import TargetUnionTypeDef


def get_value() -> TargetUnionTypeDef:
    return ...


# TargetUnionTypeDef definition

TargetUnionTypeDef = Union[
    TargetTypeDef,  # (1)
    TargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
2. See [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 

## AlarmConfigurationUnionTypeDef

```python
# AlarmConfigurationUnionTypeDef Union usage example

from types_aiobotocore_ssm.type_defs import AlarmConfigurationUnionTypeDef


def get_value() -> AlarmConfigurationUnionTypeDef:
    return ...


# AlarmConfigurationUnionTypeDef definition

AlarmConfigurationUnionTypeDef = Union[
    AlarmConfigurationTypeDef,  # (1)
    AlarmConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) 
2. See [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 

## AssociationStatusUnionTypeDef

```python
# AssociationStatusUnionTypeDef Union usage example

from types_aiobotocore_ssm.type_defs import AssociationStatusUnionTypeDef


def get_value() -> AssociationStatusUnionTypeDef:
    return ...


# AssociationStatusUnionTypeDef definition

AssociationStatusUnionTypeDef = Union[
    AssociationStatusTypeDef,  # (1)
    AssociationStatusOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AssociationStatusTypeDef](./type_defs.md#associationstatustypedef) 
2. See [:material-code-braces: AssociationStatusOutputTypeDef](./type_defs.md#associationstatusoutputtypedef) 

## ComplianceExecutionSummaryUnionTypeDef

```python
# ComplianceExecutionSummaryUnionTypeDef Union usage example

from types_aiobotocore_ssm.type_defs import ComplianceExecutionSummaryUnionTypeDef


def get_value() -> ComplianceExecutionSummaryUnionTypeDef:
    return ...


# ComplianceExecutionSummaryUnionTypeDef definition

ComplianceExecutionSummaryUnionTypeDef = Union[
    ComplianceExecutionSummaryTypeDef,  # (1)
    ComplianceExecutionSummaryOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ComplianceExecutionSummaryTypeDef](./type_defs.md#complianceexecutionsummarytypedef) 
2. See [:material-code-braces: ComplianceExecutionSummaryOutputTypeDef](./type_defs.md#complianceexecutionsummaryoutputtypedef) 

## ResourceDataSyncAwsOrganizationsSourceUnionTypeDef

```python
# ResourceDataSyncAwsOrganizationsSourceUnionTypeDef Union usage example

from types_aiobotocore_ssm.type_defs import ResourceDataSyncAwsOrganizationsSourceUnionTypeDef


def get_value() -> ResourceDataSyncAwsOrganizationsSourceUnionTypeDef:
    return ...


# ResourceDataSyncAwsOrganizationsSourceUnionTypeDef definition

ResourceDataSyncAwsOrganizationsSourceUnionTypeDef = Union[
    ResourceDataSyncAwsOrganizationsSourceTypeDef,  # (1)
    ResourceDataSyncAwsOrganizationsSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ResourceDataSyncAwsOrganizationsSourceTypeDef](./type_defs.md#resourcedatasyncawsorganizationssourcetypedef) 
2. See [:material-code-braces: ResourceDataSyncAwsOrganizationsSourceOutputTypeDef](./type_defs.md#resourcedatasyncawsorganizationssourceoutputtypedef) 

## MaintenanceWindowTaskInvocationParametersUnionTypeDef

```python
# MaintenanceWindowTaskInvocationParametersUnionTypeDef Union usage example

from types_aiobotocore_ssm.type_defs import MaintenanceWindowTaskInvocationParametersUnionTypeDef


def get_value() -> MaintenanceWindowTaskInvocationParametersUnionTypeDef:
    return ...


# MaintenanceWindowTaskInvocationParametersUnionTypeDef definition

MaintenanceWindowTaskInvocationParametersUnionTypeDef = Union[
    MaintenanceWindowTaskInvocationParametersTypeDef,  # (1)
    MaintenanceWindowTaskInvocationParametersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MaintenanceWindowTaskInvocationParametersTypeDef](./type_defs.md#maintenancewindowtaskinvocationparameterstypedef) 
2. See [:material-code-braces: MaintenanceWindowTaskInvocationParametersOutputTypeDef](./type_defs.md#maintenancewindowtaskinvocationparametersoutputtypedef) 

## PatchFilterGroupUnionTypeDef

```python
# PatchFilterGroupUnionTypeDef Union usage example

from types_aiobotocore_ssm.type_defs import PatchFilterGroupUnionTypeDef


def get_value() -> PatchFilterGroupUnionTypeDef:
    return ...


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
# TargetLocationUnionTypeDef Union usage example

from types_aiobotocore_ssm.type_defs import TargetLocationUnionTypeDef


def get_value() -> TargetLocationUnionTypeDef:
    return ...


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
# PatchRuleUnionTypeDef Union usage example

from types_aiobotocore_ssm.type_defs import PatchRuleUnionTypeDef


def get_value() -> PatchRuleUnionTypeDef:
    return ...


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
# CreateAssociationBatchRequestEntryUnionTypeDef Union usage example

from types_aiobotocore_ssm.type_defs import CreateAssociationBatchRequestEntryUnionTypeDef


def get_value() -> CreateAssociationBatchRequestEntryUnionTypeDef:
    return ...


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
# RunbookUnionTypeDef Union usage example

from types_aiobotocore_ssm.type_defs import RunbookUnionTypeDef


def get_value() -> RunbookUnionTypeDef:
    return ...


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
# PatchRuleGroupUnionTypeDef Union usage example

from types_aiobotocore_ssm.type_defs import PatchRuleGroupUnionTypeDef


def get_value() -> PatchRuleGroupUnionTypeDef:
    return ...


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
# AccountSharingInfoTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AccountSharingInfoTypeDef


def get_value() -> AccountSharingInfoTypeDef:
    return {
        "AccountId": ...,
    }


# AccountSharingInfoTypeDef definition

class AccountSharingInfoTypeDef(TypedDict):
    AccountId: NotRequired[str],
    SharedDocumentVersion: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "Key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## AlarmTypeDef

```python
# AlarmTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AlarmTypeDef


def get_value() -> AlarmTypeDef:
    return {
        "Name": ...,
    }


# AlarmTypeDef definition

class AlarmTypeDef(TypedDict):
    Name: str,
```

## AlarmStateInformationTypeDef

```python
# AlarmStateInformationTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AlarmStateInformationTypeDef


def get_value() -> AlarmStateInformationTypeDef:
    return {
        "Name": ...,
    }


# AlarmStateInformationTypeDef definition

class AlarmStateInformationTypeDef(TypedDict):
    Name: str,
    State: ExternalAlarmStateType,  # (1)
```

1. See [:material-code-brackets: ExternalAlarmStateType](./literals.md#externalalarmstatetype) 
## AssociateOpsItemRelatedItemRequestTypeDef

```python
# AssociateOpsItemRelatedItemRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AssociateOpsItemRelatedItemRequestTypeDef


def get_value() -> AssociateOpsItemRelatedItemRequestTypeDef:
    return {
        "OpsItemId": ...,
    }


# AssociateOpsItemRelatedItemRequestTypeDef definition

class AssociateOpsItemRelatedItemRequestTypeDef(TypedDict):
    OpsItemId: str,
    AssociationType: str,
    ResourceType: str,
    ResourceUri: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ResponseMetadataTypeDef


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

## AssociationOverviewTypeDef

```python
# AssociationOverviewTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AssociationOverviewTypeDef


def get_value() -> AssociationOverviewTypeDef:
    return {
        "Status": ...,
    }


# AssociationOverviewTypeDef definition

class AssociationOverviewTypeDef(TypedDict):
    Status: NotRequired[str],
    DetailedStatus: NotRequired[str],
    AssociationStatusAggregatedCount: NotRequired[Dict[str, int]],
```

## AssociationStatusOutputTypeDef

```python
# AssociationStatusOutputTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AssociationStatusOutputTypeDef


def get_value() -> AssociationStatusOutputTypeDef:
    return {
        "Date": ...,
    }


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
# TargetOutputTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import TargetOutputTypeDef


def get_value() -> TargetOutputTypeDef:
    return {
        "Key": ...,
    }


# TargetOutputTypeDef definition

class TargetOutputTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[List[str]],
```

## AssociationExecutionFilterTypeDef

```python
# AssociationExecutionFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AssociationExecutionFilterTypeDef


def get_value() -> AssociationExecutionFilterTypeDef:
    return {
        "Key": ...,
    }


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
# OutputSourceTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import OutputSourceTypeDef


def get_value() -> OutputSourceTypeDef:
    return {
        "OutputSourceId": ...,
    }


# OutputSourceTypeDef definition

class OutputSourceTypeDef(TypedDict):
    OutputSourceId: NotRequired[str],
    OutputSourceType: NotRequired[str],
```

## AssociationExecutionTargetsFilterTypeDef

```python
# AssociationExecutionTargetsFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AssociationExecutionTargetsFilterTypeDef


def get_value() -> AssociationExecutionTargetsFilterTypeDef:
    return {
        "Key": ...,
    }


# AssociationExecutionTargetsFilterTypeDef definition

class AssociationExecutionTargetsFilterTypeDef(TypedDict):
    Key: AssociationExecutionTargetsFilterKeyType,  # (1)
    Value: str,
```

1. See [:material-code-brackets: AssociationExecutionTargetsFilterKeyType](./literals.md#associationexecutiontargetsfilterkeytype) 
## AssociationFilterTypeDef

```python
# AssociationFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AssociationFilterTypeDef


def get_value() -> AssociationFilterTypeDef:
    return {
        "key": ...,
    }


# AssociationFilterTypeDef definition

class AssociationFilterTypeDef(TypedDict):
    key: AssociationFilterKeyType,  # (1)
    value: str,
```

1. See [:material-code-brackets: AssociationFilterKeyType](./literals.md#associationfilterkeytype) 
## AttachmentContentTypeDef

```python
# AttachmentContentTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AttachmentContentTypeDef


def get_value() -> AttachmentContentTypeDef:
    return {
        "Name": ...,
    }


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
# AttachmentInformationTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AttachmentInformationTypeDef


def get_value() -> AttachmentInformationTypeDef:
    return {
        "Name": ...,
    }


# AttachmentInformationTypeDef definition

class AttachmentInformationTypeDef(TypedDict):
    Name: NotRequired[str],
```

## AttachmentsSourceTypeDef

```python
# AttachmentsSourceTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AttachmentsSourceTypeDef


def get_value() -> AttachmentsSourceTypeDef:
    return {
        "Key": ...,
    }


# AttachmentsSourceTypeDef definition

class AttachmentsSourceTypeDef(TypedDict):
    Key: NotRequired[AttachmentsSourceKeyType],  # (1)
    Values: NotRequired[Sequence[str]],
    Name: NotRequired[str],
```

1. See [:material-code-brackets: AttachmentsSourceKeyType](./literals.md#attachmentssourcekeytype) 
## AutomationExecutionFilterTypeDef

```python
# AutomationExecutionFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AutomationExecutionFilterTypeDef


def get_value() -> AutomationExecutionFilterTypeDef:
    return {
        "Key": ...,
    }


# AutomationExecutionFilterTypeDef definition

class AutomationExecutionFilterTypeDef(TypedDict):
    Key: AutomationExecutionFilterKeyType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: AutomationExecutionFilterKeyType](./literals.md#automationexecutionfilterkeytype) 
## ResolvedTargetsTypeDef

```python
# ResolvedTargetsTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ResolvedTargetsTypeDef


def get_value() -> ResolvedTargetsTypeDef:
    return {
        "ParameterValues": ...,
    }


# ResolvedTargetsTypeDef definition

class ResolvedTargetsTypeDef(TypedDict):
    ParameterValues: NotRequired[List[str]],
    Truncated: NotRequired[bool],
```

## TargetPreviewTypeDef

```python
# TargetPreviewTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import TargetPreviewTypeDef


def get_value() -> TargetPreviewTypeDef:
    return {
        "Count": ...,
    }


# TargetPreviewTypeDef definition

class TargetPreviewTypeDef(TypedDict):
    Count: NotRequired[int],
    TargetType: NotRequired[str],
```

## ProgressCountersTypeDef

```python
# ProgressCountersTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ProgressCountersTypeDef


def get_value() -> ProgressCountersTypeDef:
    return {
        "TotalSteps": ...,
    }


# ProgressCountersTypeDef definition

class ProgressCountersTypeDef(TypedDict):
    TotalSteps: NotRequired[int],
    SuccessSteps: NotRequired[int],
    FailedSteps: NotRequired[int],
    CancelledSteps: NotRequired[int],
    TimedOutSteps: NotRequired[int],
```

## CancelCommandRequestTypeDef

```python
# CancelCommandRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CancelCommandRequestTypeDef


def get_value() -> CancelCommandRequestTypeDef:
    return {
        "CommandId": ...,
    }


# CancelCommandRequestTypeDef definition

class CancelCommandRequestTypeDef(TypedDict):
    CommandId: str,
    InstanceIds: NotRequired[Sequence[str]],
```

## CancelMaintenanceWindowExecutionRequestTypeDef

```python
# CancelMaintenanceWindowExecutionRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CancelMaintenanceWindowExecutionRequestTypeDef


def get_value() -> CancelMaintenanceWindowExecutionRequestTypeDef:
    return {
        "WindowExecutionId": ...,
    }


# CancelMaintenanceWindowExecutionRequestTypeDef definition

class CancelMaintenanceWindowExecutionRequestTypeDef(TypedDict):
    WindowExecutionId: str,
```

## CloudWatchOutputConfigTypeDef

```python
# CloudWatchOutputConfigTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CloudWatchOutputConfigTypeDef


def get_value() -> CloudWatchOutputConfigTypeDef:
    return {
        "CloudWatchLogGroupName": ...,
    }


# CloudWatchOutputConfigTypeDef definition

class CloudWatchOutputConfigTypeDef(TypedDict):
    CloudWatchLogGroupName: NotRequired[str],
    CloudWatchOutputEnabled: NotRequired[bool],
```

## CommandFilterTypeDef

```python
# CommandFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CommandFilterTypeDef


def get_value() -> CommandFilterTypeDef:
    return {
        "key": ...,
    }


# CommandFilterTypeDef definition

class CommandFilterTypeDef(TypedDict):
    key: CommandFilterKeyType,  # (1)
    value: str,
```

1. See [:material-code-brackets: CommandFilterKeyType](./literals.md#commandfilterkeytype) 
## CommandPluginTypeDef

```python
# CommandPluginTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CommandPluginTypeDef


def get_value() -> CommandPluginTypeDef:
    return {
        "Name": ...,
    }


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
# NotificationConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import NotificationConfigOutputTypeDef


def get_value() -> NotificationConfigOutputTypeDef:
    return {
        "NotificationArn": ...,
    }


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
# ComplianceExecutionSummaryOutputTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ComplianceExecutionSummaryOutputTypeDef


def get_value() -> ComplianceExecutionSummaryOutputTypeDef:
    return {
        "ExecutionTime": ...,
    }


# ComplianceExecutionSummaryOutputTypeDef definition

class ComplianceExecutionSummaryOutputTypeDef(TypedDict):
    ExecutionTime: datetime,
    ExecutionId: NotRequired[str],
    ExecutionType: NotRequired[str],
```

## ComplianceItemEntryTypeDef

```python
# ComplianceItemEntryTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ComplianceItemEntryTypeDef


def get_value() -> ComplianceItemEntryTypeDef:
    return {
        "Id": ...,
    }


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
# ComplianceStringFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ComplianceStringFilterTypeDef


def get_value() -> ComplianceStringFilterTypeDef:
    return {
        "Key": ...,
    }


# ComplianceStringFilterTypeDef definition

class ComplianceStringFilterTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[Sequence[str]],
    Type: NotRequired[ComplianceQueryOperatorTypeType],  # (1)
```

1. See [:material-code-brackets: ComplianceQueryOperatorTypeType](./literals.md#compliancequeryoperatortypetype) 
## SeveritySummaryTypeDef

```python
# SeveritySummaryTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import SeveritySummaryTypeDef


def get_value() -> SeveritySummaryTypeDef:
    return {
        "CriticalCount": ...,
    }


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
# RegistrationMetadataItemTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import RegistrationMetadataItemTypeDef


def get_value() -> RegistrationMetadataItemTypeDef:
    return {
        "Key": ...,
    }


# RegistrationMetadataItemTypeDef definition

class RegistrationMetadataItemTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## DocumentRequiresTypeDef

```python
# DocumentRequiresTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DocumentRequiresTypeDef


def get_value() -> DocumentRequiresTypeDef:
    return {
        "Name": ...,
    }


# DocumentRequiresTypeDef definition

class DocumentRequiresTypeDef(TypedDict):
    Name: str,
    Version: NotRequired[str],
    RequireType: NotRequired[str],
    VersionName: NotRequired[str],
```

## OpsItemDataValueTypeDef

```python
# OpsItemDataValueTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import OpsItemDataValueTypeDef


def get_value() -> OpsItemDataValueTypeDef:
    return {
        "Value": ...,
    }


# OpsItemDataValueTypeDef definition

class OpsItemDataValueTypeDef(TypedDict):
    Value: NotRequired[str],
    Type: NotRequired[OpsItemDataTypeType],  # (1)
```

1. See [:material-code-brackets: OpsItemDataTypeType](./literals.md#opsitemdatatypetype) 
## OpsItemNotificationTypeDef

```python
# OpsItemNotificationTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import OpsItemNotificationTypeDef


def get_value() -> OpsItemNotificationTypeDef:
    return {
        "Arn": ...,
    }


# OpsItemNotificationTypeDef definition

class OpsItemNotificationTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## RelatedOpsItemTypeDef

```python
# RelatedOpsItemTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import RelatedOpsItemTypeDef


def get_value() -> RelatedOpsItemTypeDef:
    return {
        "OpsItemId": ...,
    }


# RelatedOpsItemTypeDef definition

class RelatedOpsItemTypeDef(TypedDict):
    OpsItemId: str,
```

## MetadataValueTypeDef

```python
# MetadataValueTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import MetadataValueTypeDef


def get_value() -> MetadataValueTypeDef:
    return {
        "Value": ...,
    }


# MetadataValueTypeDef definition

class MetadataValueTypeDef(TypedDict):
    Value: NotRequired[str],
```

## DeleteActivationRequestTypeDef

```python
# DeleteActivationRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeleteActivationRequestTypeDef


def get_value() -> DeleteActivationRequestTypeDef:
    return {
        "ActivationId": ...,
    }


# DeleteActivationRequestTypeDef definition

class DeleteActivationRequestTypeDef(TypedDict):
    ActivationId: str,
```

## DeleteAssociationRequestTypeDef

```python
# DeleteAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeleteAssociationRequestTypeDef


def get_value() -> DeleteAssociationRequestTypeDef:
    return {
        "Name": ...,
    }


# DeleteAssociationRequestTypeDef definition

class DeleteAssociationRequestTypeDef(TypedDict):
    Name: NotRequired[str],
    InstanceId: NotRequired[str],
    AssociationId: NotRequired[str],
```

## DeleteDocumentRequestTypeDef

```python
# DeleteDocumentRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeleteDocumentRequestTypeDef


def get_value() -> DeleteDocumentRequestTypeDef:
    return {
        "Name": ...,
    }


# DeleteDocumentRequestTypeDef definition

class DeleteDocumentRequestTypeDef(TypedDict):
    Name: str,
    DocumentVersion: NotRequired[str],
    VersionName: NotRequired[str],
    Force: NotRequired[bool],
```

## DeleteInventoryRequestTypeDef

```python
# DeleteInventoryRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeleteInventoryRequestTypeDef


def get_value() -> DeleteInventoryRequestTypeDef:
    return {
        "TypeName": ...,
    }


# DeleteInventoryRequestTypeDef definition

class DeleteInventoryRequestTypeDef(TypedDict):
    TypeName: str,
    SchemaDeleteOption: NotRequired[InventorySchemaDeleteOptionType],  # (1)
    DryRun: NotRequired[bool],
    ClientToken: NotRequired[str],
```

1. See [:material-code-brackets: InventorySchemaDeleteOptionType](./literals.md#inventoryschemadeleteoptiontype) 
## DeleteMaintenanceWindowRequestTypeDef

```python
# DeleteMaintenanceWindowRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeleteMaintenanceWindowRequestTypeDef


def get_value() -> DeleteMaintenanceWindowRequestTypeDef:
    return {
        "WindowId": ...,
    }


# DeleteMaintenanceWindowRequestTypeDef definition

class DeleteMaintenanceWindowRequestTypeDef(TypedDict):
    WindowId: str,
```

## DeleteOpsItemRequestTypeDef

```python
# DeleteOpsItemRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeleteOpsItemRequestTypeDef


def get_value() -> DeleteOpsItemRequestTypeDef:
    return {
        "OpsItemId": ...,
    }


# DeleteOpsItemRequestTypeDef definition

class DeleteOpsItemRequestTypeDef(TypedDict):
    OpsItemId: str,
```

## DeleteOpsMetadataRequestTypeDef

```python
# DeleteOpsMetadataRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeleteOpsMetadataRequestTypeDef


def get_value() -> DeleteOpsMetadataRequestTypeDef:
    return {
        "OpsMetadataArn": ...,
    }


# DeleteOpsMetadataRequestTypeDef definition

class DeleteOpsMetadataRequestTypeDef(TypedDict):
    OpsMetadataArn: str,
```

## DeleteParameterRequestTypeDef

```python
# DeleteParameterRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeleteParameterRequestTypeDef


def get_value() -> DeleteParameterRequestTypeDef:
    return {
        "Name": ...,
    }


# DeleteParameterRequestTypeDef definition

class DeleteParameterRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteParametersRequestTypeDef

```python
# DeleteParametersRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeleteParametersRequestTypeDef


def get_value() -> DeleteParametersRequestTypeDef:
    return {
        "Names": ...,
    }


# DeleteParametersRequestTypeDef definition

class DeleteParametersRequestTypeDef(TypedDict):
    Names: Sequence[str],
```

## DeletePatchBaselineRequestTypeDef

```python
# DeletePatchBaselineRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeletePatchBaselineRequestTypeDef


def get_value() -> DeletePatchBaselineRequestTypeDef:
    return {
        "BaselineId": ...,
    }


# DeletePatchBaselineRequestTypeDef definition

class DeletePatchBaselineRequestTypeDef(TypedDict):
    BaselineId: str,
```

## DeleteResourceDataSyncRequestTypeDef

```python
# DeleteResourceDataSyncRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeleteResourceDataSyncRequestTypeDef


def get_value() -> DeleteResourceDataSyncRequestTypeDef:
    return {
        "SyncName": ...,
    }


# DeleteResourceDataSyncRequestTypeDef definition

class DeleteResourceDataSyncRequestTypeDef(TypedDict):
    SyncName: str,
    SyncType: NotRequired[str],
```

## DeleteResourcePolicyRequestTypeDef

```python
# DeleteResourcePolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeleteResourcePolicyRequestTypeDef


def get_value() -> DeleteResourcePolicyRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# DeleteResourcePolicyRequestTypeDef definition

class DeleteResourcePolicyRequestTypeDef(TypedDict):
    ResourceArn: str,
    PolicyId: str,
    PolicyHash: str,
```

## DeregisterManagedInstanceRequestTypeDef

```python
# DeregisterManagedInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeregisterManagedInstanceRequestTypeDef


def get_value() -> DeregisterManagedInstanceRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeregisterManagedInstanceRequestTypeDef definition

class DeregisterManagedInstanceRequestTypeDef(TypedDict):
    InstanceId: str,
```

## DeregisterPatchBaselineForPatchGroupRequestTypeDef

```python
# DeregisterPatchBaselineForPatchGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeregisterPatchBaselineForPatchGroupRequestTypeDef


def get_value() -> DeregisterPatchBaselineForPatchGroupRequestTypeDef:
    return {
        "BaselineId": ...,
    }


# DeregisterPatchBaselineForPatchGroupRequestTypeDef definition

class DeregisterPatchBaselineForPatchGroupRequestTypeDef(TypedDict):
    BaselineId: str,
    PatchGroup: str,
```

## DeregisterTargetFromMaintenanceWindowRequestTypeDef

```python
# DeregisterTargetFromMaintenanceWindowRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeregisterTargetFromMaintenanceWindowRequestTypeDef


def get_value() -> DeregisterTargetFromMaintenanceWindowRequestTypeDef:
    return {
        "WindowId": ...,
    }


# DeregisterTargetFromMaintenanceWindowRequestTypeDef definition

class DeregisterTargetFromMaintenanceWindowRequestTypeDef(TypedDict):
    WindowId: str,
    WindowTargetId: str,
    Safe: NotRequired[bool],
```

## DeregisterTaskFromMaintenanceWindowRequestTypeDef

```python
# DeregisterTaskFromMaintenanceWindowRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeregisterTaskFromMaintenanceWindowRequestTypeDef


def get_value() -> DeregisterTaskFromMaintenanceWindowRequestTypeDef:
    return {
        "WindowId": ...,
    }


# DeregisterTaskFromMaintenanceWindowRequestTypeDef definition

class DeregisterTaskFromMaintenanceWindowRequestTypeDef(TypedDict):
    WindowId: str,
    WindowTaskId: str,
```

## DescribeActivationsFilterTypeDef

```python
# DescribeActivationsFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeActivationsFilterTypeDef


def get_value() -> DescribeActivationsFilterTypeDef:
    return {
        "FilterKey": ...,
    }


# DescribeActivationsFilterTypeDef definition

class DescribeActivationsFilterTypeDef(TypedDict):
    FilterKey: NotRequired[DescribeActivationsFilterKeysType],  # (1)
    FilterValues: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: DescribeActivationsFilterKeysType](./literals.md#describeactivationsfilterkeystype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeAssociationRequestTypeDef

```python
# DescribeAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeAssociationRequestTypeDef


def get_value() -> DescribeAssociationRequestTypeDef:
    return {
        "Name": ...,
    }


# DescribeAssociationRequestTypeDef definition

class DescribeAssociationRequestTypeDef(TypedDict):
    Name: NotRequired[str],
    InstanceId: NotRequired[str],
    AssociationId: NotRequired[str],
    AssociationVersion: NotRequired[str],
```

## StepExecutionFilterTypeDef

```python
# StepExecutionFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import StepExecutionFilterTypeDef


def get_value() -> StepExecutionFilterTypeDef:
    return {
        "Key": ...,
    }


# StepExecutionFilterTypeDef definition

class StepExecutionFilterTypeDef(TypedDict):
    Key: StepExecutionFilterKeyType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: StepExecutionFilterKeyType](./literals.md#stepexecutionfilterkeytype) 
## PatchOrchestratorFilterTypeDef

```python
# PatchOrchestratorFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PatchOrchestratorFilterTypeDef


def get_value() -> PatchOrchestratorFilterTypeDef:
    return {
        "Key": ...,
    }


# PatchOrchestratorFilterTypeDef definition

class PatchOrchestratorFilterTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## PatchTypeDef

```python
# PatchTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PatchTypeDef


def get_value() -> PatchTypeDef:
    return {
        "Id": ...,
    }


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

## DescribeDocumentPermissionRequestTypeDef

```python
# DescribeDocumentPermissionRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeDocumentPermissionRequestTypeDef


def get_value() -> DescribeDocumentPermissionRequestTypeDef:
    return {
        "Name": ...,
    }


# DescribeDocumentPermissionRequestTypeDef definition

class DescribeDocumentPermissionRequestTypeDef(TypedDict):
    Name: str,
    PermissionType: DocumentPermissionTypeType,  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: DocumentPermissionTypeType](./literals.md#documentpermissiontypetype) 
## DescribeDocumentRequestTypeDef

```python
# DescribeDocumentRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeDocumentRequestTypeDef


def get_value() -> DescribeDocumentRequestTypeDef:
    return {
        "Name": ...,
    }


# DescribeDocumentRequestTypeDef definition

class DescribeDocumentRequestTypeDef(TypedDict):
    Name: str,
    DocumentVersion: NotRequired[str],
    VersionName: NotRequired[str],
```

## DescribeEffectiveInstanceAssociationsRequestTypeDef

```python
# DescribeEffectiveInstanceAssociationsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeEffectiveInstanceAssociationsRequestTypeDef


def get_value() -> DescribeEffectiveInstanceAssociationsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeEffectiveInstanceAssociationsRequestTypeDef definition

class DescribeEffectiveInstanceAssociationsRequestTypeDef(TypedDict):
    InstanceId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## InstanceAssociationTypeDef

```python
# InstanceAssociationTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InstanceAssociationTypeDef


def get_value() -> InstanceAssociationTypeDef:
    return {
        "AssociationId": ...,
    }


# InstanceAssociationTypeDef definition

class InstanceAssociationTypeDef(TypedDict):
    AssociationId: NotRequired[str],
    InstanceId: NotRequired[str],
    Content: NotRequired[str],
    AssociationVersion: NotRequired[str],
```

## DescribeEffectivePatchesForPatchBaselineRequestTypeDef

```python
# DescribeEffectivePatchesForPatchBaselineRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeEffectivePatchesForPatchBaselineRequestTypeDef


def get_value() -> DescribeEffectivePatchesForPatchBaselineRequestTypeDef:
    return {
        "BaselineId": ...,
    }


# DescribeEffectivePatchesForPatchBaselineRequestTypeDef definition

class DescribeEffectivePatchesForPatchBaselineRequestTypeDef(TypedDict):
    BaselineId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeInstanceAssociationsStatusRequestTypeDef

```python
# DescribeInstanceAssociationsStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeInstanceAssociationsStatusRequestTypeDef


def get_value() -> DescribeInstanceAssociationsStatusRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeInstanceAssociationsStatusRequestTypeDef definition

class DescribeInstanceAssociationsStatusRequestTypeDef(TypedDict):
    InstanceId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## InstanceInformationFilterTypeDef

```python
# InstanceInformationFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InstanceInformationFilterTypeDef


def get_value() -> InstanceInformationFilterTypeDef:
    return {
        "key": ...,
    }


# InstanceInformationFilterTypeDef definition

class InstanceInformationFilterTypeDef(TypedDict):
    key: InstanceInformationFilterKeyType,  # (1)
    valueSet: Sequence[str],
```

1. See [:material-code-brackets: InstanceInformationFilterKeyType](./literals.md#instanceinformationfilterkeytype) 
## InstanceInformationStringFilterTypeDef

```python
# InstanceInformationStringFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InstanceInformationStringFilterTypeDef


def get_value() -> InstanceInformationStringFilterTypeDef:
    return {
        "Key": ...,
    }


# InstanceInformationStringFilterTypeDef definition

class InstanceInformationStringFilterTypeDef(TypedDict):
    Key: str,
    Values: Sequence[str],
```

## InstancePatchStateFilterTypeDef

```python
# InstancePatchStateFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InstancePatchStateFilterTypeDef


def get_value() -> InstancePatchStateFilterTypeDef:
    return {
        "Key": ...,
    }


# InstancePatchStateFilterTypeDef definition

class InstancePatchStateFilterTypeDef(TypedDict):
    Key: str,
    Values: Sequence[str],
    Type: InstancePatchStateOperatorTypeType,  # (1)
```

1. See [:material-code-brackets: InstancePatchStateOperatorTypeType](./literals.md#instancepatchstateoperatortypetype) 
## InstancePatchStateTypeDef

```python
# InstancePatchStateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InstancePatchStateTypeDef


def get_value() -> InstancePatchStateTypeDef:
    return {
        "InstanceId": ...,
    }


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
## DescribeInstancePatchStatesRequestTypeDef

```python
# DescribeInstancePatchStatesRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeInstancePatchStatesRequestTypeDef


def get_value() -> DescribeInstancePatchStatesRequestTypeDef:
    return {
        "InstanceIds": ...,
    }


# DescribeInstancePatchStatesRequestTypeDef definition

class DescribeInstancePatchStatesRequestTypeDef(TypedDict):
    InstanceIds: Sequence[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## PatchComplianceDataTypeDef

```python
# PatchComplianceDataTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PatchComplianceDataTypeDef


def get_value() -> PatchComplianceDataTypeDef:
    return {
        "Title": ...,
    }


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
# InstancePropertyFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InstancePropertyFilterTypeDef


def get_value() -> InstancePropertyFilterTypeDef:
    return {
        "key": ...,
    }


# InstancePropertyFilterTypeDef definition

class InstancePropertyFilterTypeDef(TypedDict):
    key: InstancePropertyFilterKeyType,  # (1)
    valueSet: Sequence[str],
```

1. See [:material-code-brackets: InstancePropertyFilterKeyType](./literals.md#instancepropertyfilterkeytype) 
## InstancePropertyStringFilterTypeDef

```python
# InstancePropertyStringFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InstancePropertyStringFilterTypeDef


def get_value() -> InstancePropertyStringFilterTypeDef:
    return {
        "Key": ...,
    }


# InstancePropertyStringFilterTypeDef definition

class InstancePropertyStringFilterTypeDef(TypedDict):
    Key: str,
    Values: Sequence[str],
    Operator: NotRequired[InstancePropertyFilterOperatorType],  # (1)
```

1. See [:material-code-brackets: InstancePropertyFilterOperatorType](./literals.md#instancepropertyfilteroperatortype) 
## DescribeInventoryDeletionsRequestTypeDef

```python
# DescribeInventoryDeletionsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeInventoryDeletionsRequestTypeDef


def get_value() -> DescribeInventoryDeletionsRequestTypeDef:
    return {
        "DeletionId": ...,
    }


# DescribeInventoryDeletionsRequestTypeDef definition

class DescribeInventoryDeletionsRequestTypeDef(TypedDict):
    DeletionId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## MaintenanceWindowFilterTypeDef

```python
# MaintenanceWindowFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import MaintenanceWindowFilterTypeDef


def get_value() -> MaintenanceWindowFilterTypeDef:
    return {
        "Key": ...,
    }


# MaintenanceWindowFilterTypeDef definition

class MaintenanceWindowFilterTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## MaintenanceWindowExecutionTaskInvocationIdentityTypeDef

```python
# MaintenanceWindowExecutionTaskInvocationIdentityTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import MaintenanceWindowExecutionTaskInvocationIdentityTypeDef


def get_value() -> MaintenanceWindowExecutionTaskInvocationIdentityTypeDef:
    return {
        "WindowExecutionId": ...,
    }


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
# MaintenanceWindowExecutionTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import MaintenanceWindowExecutionTypeDef


def get_value() -> MaintenanceWindowExecutionTypeDef:
    return {
        "WindowId": ...,
    }


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
## ScheduledWindowExecutionTypeDef

```python
# ScheduledWindowExecutionTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ScheduledWindowExecutionTypeDef


def get_value() -> ScheduledWindowExecutionTypeDef:
    return {
        "WindowId": ...,
    }


# ScheduledWindowExecutionTypeDef definition

class ScheduledWindowExecutionTypeDef(TypedDict):
    WindowId: NotRequired[str],
    Name: NotRequired[str],
    ExecutionTime: NotRequired[str],
```

## MaintenanceWindowIdentityForTargetTypeDef

```python
# MaintenanceWindowIdentityForTargetTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import MaintenanceWindowIdentityForTargetTypeDef


def get_value() -> MaintenanceWindowIdentityForTargetTypeDef:
    return {
        "WindowId": ...,
    }


# MaintenanceWindowIdentityForTargetTypeDef definition

class MaintenanceWindowIdentityForTargetTypeDef(TypedDict):
    WindowId: NotRequired[str],
    Name: NotRequired[str],
```

## MaintenanceWindowIdentityTypeDef

```python
# MaintenanceWindowIdentityTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import MaintenanceWindowIdentityTypeDef


def get_value() -> MaintenanceWindowIdentityTypeDef:
    return {
        "WindowId": ...,
    }


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
# OpsItemFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import OpsItemFilterTypeDef


def get_value() -> OpsItemFilterTypeDef:
    return {
        "Key": ...,
    }


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
# ParameterStringFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ParameterStringFilterTypeDef


def get_value() -> ParameterStringFilterTypeDef:
    return {
        "Key": ...,
    }


# ParameterStringFilterTypeDef definition

class ParameterStringFilterTypeDef(TypedDict):
    Key: str,
    Option: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## ParametersFilterTypeDef

```python
# ParametersFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ParametersFilterTypeDef


def get_value() -> ParametersFilterTypeDef:
    return {
        "Key": ...,
    }


# ParametersFilterTypeDef definition

class ParametersFilterTypeDef(TypedDict):
    Key: ParametersFilterKeyType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: ParametersFilterKeyType](./literals.md#parametersfilterkeytype) 
## PatchBaselineIdentityTypeDef

```python
# PatchBaselineIdentityTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PatchBaselineIdentityTypeDef


def get_value() -> PatchBaselineIdentityTypeDef:
    return {
        "BaselineId": ...,
    }


# PatchBaselineIdentityTypeDef definition

class PatchBaselineIdentityTypeDef(TypedDict):
    BaselineId: NotRequired[str],
    BaselineName: NotRequired[str],
    OperatingSystem: NotRequired[OperatingSystemType],  # (1)
    BaselineDescription: NotRequired[str],
    DefaultBaseline: NotRequired[bool],
```

1. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
## DescribePatchGroupStateRequestTypeDef

```python
# DescribePatchGroupStateRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribePatchGroupStateRequestTypeDef


def get_value() -> DescribePatchGroupStateRequestTypeDef:
    return {
        "PatchGroup": ...,
    }


# DescribePatchGroupStateRequestTypeDef definition

class DescribePatchGroupStateRequestTypeDef(TypedDict):
    PatchGroup: str,
```

## DescribePatchPropertiesRequestTypeDef

```python
# DescribePatchPropertiesRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribePatchPropertiesRequestTypeDef


def get_value() -> DescribePatchPropertiesRequestTypeDef:
    return {
        "OperatingSystem": ...,
    }


# DescribePatchPropertiesRequestTypeDef definition

class DescribePatchPropertiesRequestTypeDef(TypedDict):
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
# SessionFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import SessionFilterTypeDef


def get_value() -> SessionFilterTypeDef:
    return {
        "key": ...,
    }


# SessionFilterTypeDef definition

class SessionFilterTypeDef(TypedDict):
    key: SessionFilterKeyType,  # (1)
    value: str,
```

1. See [:material-code-brackets: SessionFilterKeyType](./literals.md#sessionfilterkeytype) 
## DisassociateOpsItemRelatedItemRequestTypeDef

```python
# DisassociateOpsItemRelatedItemRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DisassociateOpsItemRelatedItemRequestTypeDef


def get_value() -> DisassociateOpsItemRelatedItemRequestTypeDef:
    return {
        "OpsItemId": ...,
    }


# DisassociateOpsItemRelatedItemRequestTypeDef definition

class DisassociateOpsItemRelatedItemRequestTypeDef(TypedDict):
    OpsItemId: str,
    AssociationId: str,
```

## DocumentDefaultVersionDescriptionTypeDef

```python
# DocumentDefaultVersionDescriptionTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DocumentDefaultVersionDescriptionTypeDef


def get_value() -> DocumentDefaultVersionDescriptionTypeDef:
    return {
        "Name": ...,
    }


# DocumentDefaultVersionDescriptionTypeDef definition

class DocumentDefaultVersionDescriptionTypeDef(TypedDict):
    Name: NotRequired[str],
    DefaultVersion: NotRequired[str],
    DefaultVersionName: NotRequired[str],
```

## DocumentParameterTypeDef

```python
# DocumentParameterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DocumentParameterTypeDef


def get_value() -> DocumentParameterTypeDef:
    return {
        "Name": ...,
    }


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
# ReviewInformationTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ReviewInformationTypeDef


def get_value() -> ReviewInformationTypeDef:
    return {
        "ReviewedTime": ...,
    }


# ReviewInformationTypeDef definition

class ReviewInformationTypeDef(TypedDict):
    ReviewedTime: NotRequired[datetime],
    Status: NotRequired[ReviewStatusType],  # (1)
    Reviewer: NotRequired[str],
```

1. See [:material-code-brackets: ReviewStatusType](./literals.md#reviewstatustype) 
## DocumentFilterTypeDef

```python
# DocumentFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DocumentFilterTypeDef


def get_value() -> DocumentFilterTypeDef:
    return {
        "key": ...,
    }


# DocumentFilterTypeDef definition

class DocumentFilterTypeDef(TypedDict):
    key: DocumentFilterKeyType,  # (1)
    value: str,
```

1. See [:material-code-brackets: DocumentFilterKeyType](./literals.md#documentfilterkeytype) 
## DocumentKeyValuesFilterTypeDef

```python
# DocumentKeyValuesFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DocumentKeyValuesFilterTypeDef


def get_value() -> DocumentKeyValuesFilterTypeDef:
    return {
        "Key": ...,
    }


# DocumentKeyValuesFilterTypeDef definition

class DocumentKeyValuesFilterTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## DocumentReviewCommentSourceTypeDef

```python
# DocumentReviewCommentSourceTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DocumentReviewCommentSourceTypeDef


def get_value() -> DocumentReviewCommentSourceTypeDef:
    return {
        "Type": ...,
    }


# DocumentReviewCommentSourceTypeDef definition

class DocumentReviewCommentSourceTypeDef(TypedDict):
    Type: NotRequired[DocumentReviewCommentTypeType],  # (1)
    Content: NotRequired[str],
```

1. See [:material-code-brackets: DocumentReviewCommentTypeType](./literals.md#documentreviewcommenttypetype) 
## DocumentVersionInfoTypeDef

```python
# DocumentVersionInfoTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DocumentVersionInfoTypeDef


def get_value() -> DocumentVersionInfoTypeDef:
    return {
        "Name": ...,
    }


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
# PatchStatusTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PatchStatusTypeDef


def get_value() -> PatchStatusTypeDef:
    return {
        "DeploymentStatus": ...,
    }


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
# FailureDetailsTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import FailureDetailsTypeDef


def get_value() -> FailureDetailsTypeDef:
    return {
        "FailureStage": ...,
    }


# FailureDetailsTypeDef definition

class FailureDetailsTypeDef(TypedDict):
    FailureStage: NotRequired[str],
    FailureType: NotRequired[str],
    Details: NotRequired[Dict[str, List[str]]],
```

## GetAutomationExecutionRequestTypeDef

```python
# GetAutomationExecutionRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetAutomationExecutionRequestTypeDef


def get_value() -> GetAutomationExecutionRequestTypeDef:
    return {
        "AutomationExecutionId": ...,
    }


# GetAutomationExecutionRequestTypeDef definition

class GetAutomationExecutionRequestTypeDef(TypedDict):
    AutomationExecutionId: str,
```

## GetCalendarStateRequestTypeDef

```python
# GetCalendarStateRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetCalendarStateRequestTypeDef


def get_value() -> GetCalendarStateRequestTypeDef:
    return {
        "CalendarNames": ...,
    }


# GetCalendarStateRequestTypeDef definition

class GetCalendarStateRequestTypeDef(TypedDict):
    CalendarNames: Sequence[str],
    AtTime: NotRequired[str],
```

## GetCommandInvocationRequestTypeDef

```python
# GetCommandInvocationRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetCommandInvocationRequestTypeDef


def get_value() -> GetCommandInvocationRequestTypeDef:
    return {
        "CommandId": ...,
    }


# GetCommandInvocationRequestTypeDef definition

class GetCommandInvocationRequestTypeDef(TypedDict):
    CommandId: str,
    InstanceId: str,
    PluginName: NotRequired[str],
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import WaiterConfigTypeDef


def get_value() -> WaiterConfigTypeDef:
    return {
        "Delay": ...,
    }


# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## GetConnectionStatusRequestTypeDef

```python
# GetConnectionStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetConnectionStatusRequestTypeDef


def get_value() -> GetConnectionStatusRequestTypeDef:
    return {
        "Target": ...,
    }


# GetConnectionStatusRequestTypeDef definition

class GetConnectionStatusRequestTypeDef(TypedDict):
    Target: str,
```

## GetDefaultPatchBaselineRequestTypeDef

```python
# GetDefaultPatchBaselineRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetDefaultPatchBaselineRequestTypeDef


def get_value() -> GetDefaultPatchBaselineRequestTypeDef:
    return {
        "OperatingSystem": ...,
    }


# GetDefaultPatchBaselineRequestTypeDef definition

class GetDefaultPatchBaselineRequestTypeDef(TypedDict):
    OperatingSystem: NotRequired[OperatingSystemType],  # (1)
```

1. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
## GetDocumentRequestTypeDef

```python
# GetDocumentRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetDocumentRequestTypeDef


def get_value() -> GetDocumentRequestTypeDef:
    return {
        "Name": ...,
    }


# GetDocumentRequestTypeDef definition

class GetDocumentRequestTypeDef(TypedDict):
    Name: str,
    VersionName: NotRequired[str],
    DocumentVersion: NotRequired[str],
    DocumentFormat: NotRequired[DocumentFormatType],  # (1)
```

1. See [:material-code-brackets: DocumentFormatType](./literals.md#documentformattype) 
## GetExecutionPreviewRequestTypeDef

```python
# GetExecutionPreviewRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetExecutionPreviewRequestTypeDef


def get_value() -> GetExecutionPreviewRequestTypeDef:
    return {
        "ExecutionPreviewId": ...,
    }


# GetExecutionPreviewRequestTypeDef definition

class GetExecutionPreviewRequestTypeDef(TypedDict):
    ExecutionPreviewId: str,
```

## InventoryFilterTypeDef

```python
# InventoryFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InventoryFilterTypeDef


def get_value() -> InventoryFilterTypeDef:
    return {
        "Key": ...,
    }


# InventoryFilterTypeDef definition

class InventoryFilterTypeDef(TypedDict):
    Key: str,
    Values: Sequence[str],
    Type: NotRequired[InventoryQueryOperatorTypeType],  # (1)
```

1. See [:material-code-brackets: InventoryQueryOperatorTypeType](./literals.md#inventoryqueryoperatortypetype) 
## ResultAttributeTypeDef

```python
# ResultAttributeTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ResultAttributeTypeDef


def get_value() -> ResultAttributeTypeDef:
    return {
        "TypeName": ...,
    }


# ResultAttributeTypeDef definition

class ResultAttributeTypeDef(TypedDict):
    TypeName: str,
```

## GetInventorySchemaRequestTypeDef

```python
# GetInventorySchemaRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetInventorySchemaRequestTypeDef


def get_value() -> GetInventorySchemaRequestTypeDef:
    return {
        "TypeName": ...,
    }


# GetInventorySchemaRequestTypeDef definition

class GetInventorySchemaRequestTypeDef(TypedDict):
    TypeName: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Aggregator: NotRequired[bool],
    SubType: NotRequired[bool],
```

## GetMaintenanceWindowExecutionRequestTypeDef

```python
# GetMaintenanceWindowExecutionRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetMaintenanceWindowExecutionRequestTypeDef


def get_value() -> GetMaintenanceWindowExecutionRequestTypeDef:
    return {
        "WindowExecutionId": ...,
    }


# GetMaintenanceWindowExecutionRequestTypeDef definition

class GetMaintenanceWindowExecutionRequestTypeDef(TypedDict):
    WindowExecutionId: str,
```

## GetMaintenanceWindowExecutionTaskInvocationRequestTypeDef

```python
# GetMaintenanceWindowExecutionTaskInvocationRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetMaintenanceWindowExecutionTaskInvocationRequestTypeDef


def get_value() -> GetMaintenanceWindowExecutionTaskInvocationRequestTypeDef:
    return {
        "WindowExecutionId": ...,
    }


# GetMaintenanceWindowExecutionTaskInvocationRequestTypeDef definition

class GetMaintenanceWindowExecutionTaskInvocationRequestTypeDef(TypedDict):
    WindowExecutionId: str,
    TaskId: str,
    InvocationId: str,
```

## GetMaintenanceWindowExecutionTaskRequestTypeDef

```python
# GetMaintenanceWindowExecutionTaskRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetMaintenanceWindowExecutionTaskRequestTypeDef


def get_value() -> GetMaintenanceWindowExecutionTaskRequestTypeDef:
    return {
        "WindowExecutionId": ...,
    }


# GetMaintenanceWindowExecutionTaskRequestTypeDef definition

class GetMaintenanceWindowExecutionTaskRequestTypeDef(TypedDict):
    WindowExecutionId: str,
    TaskId: str,
```

## MaintenanceWindowTaskParameterValueExpressionOutputTypeDef

```python
# MaintenanceWindowTaskParameterValueExpressionOutputTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import MaintenanceWindowTaskParameterValueExpressionOutputTypeDef


def get_value() -> MaintenanceWindowTaskParameterValueExpressionOutputTypeDef:
    return {
        "Values": ...,
    }


# MaintenanceWindowTaskParameterValueExpressionOutputTypeDef definition

class MaintenanceWindowTaskParameterValueExpressionOutputTypeDef(TypedDict):
    Values: NotRequired[List[str]],
```

## GetMaintenanceWindowRequestTypeDef

```python
# GetMaintenanceWindowRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetMaintenanceWindowRequestTypeDef


def get_value() -> GetMaintenanceWindowRequestTypeDef:
    return {
        "WindowId": ...,
    }


# GetMaintenanceWindowRequestTypeDef definition

class GetMaintenanceWindowRequestTypeDef(TypedDict):
    WindowId: str,
```

## GetMaintenanceWindowTaskRequestTypeDef

```python
# GetMaintenanceWindowTaskRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetMaintenanceWindowTaskRequestTypeDef


def get_value() -> GetMaintenanceWindowTaskRequestTypeDef:
    return {
        "WindowId": ...,
    }


# GetMaintenanceWindowTaskRequestTypeDef definition

class GetMaintenanceWindowTaskRequestTypeDef(TypedDict):
    WindowId: str,
    WindowTaskId: str,
```

## LoggingInfoTypeDef

```python
# LoggingInfoTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import LoggingInfoTypeDef


def get_value() -> LoggingInfoTypeDef:
    return {
        "S3BucketName": ...,
    }


# LoggingInfoTypeDef definition

class LoggingInfoTypeDef(TypedDict):
    S3BucketName: str,
    S3Region: str,
    S3KeyPrefix: NotRequired[str],
```

## GetOpsItemRequestTypeDef

```python
# GetOpsItemRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetOpsItemRequestTypeDef


def get_value() -> GetOpsItemRequestTypeDef:
    return {
        "OpsItemId": ...,
    }


# GetOpsItemRequestTypeDef definition

class GetOpsItemRequestTypeDef(TypedDict):
    OpsItemId: str,
    OpsItemArn: NotRequired[str],
```

## GetOpsMetadataRequestTypeDef

```python
# GetOpsMetadataRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetOpsMetadataRequestTypeDef


def get_value() -> GetOpsMetadataRequestTypeDef:
    return {
        "OpsMetadataArn": ...,
    }


# GetOpsMetadataRequestTypeDef definition

class GetOpsMetadataRequestTypeDef(TypedDict):
    OpsMetadataArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## OpsFilterTypeDef

```python
# OpsFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import OpsFilterTypeDef


def get_value() -> OpsFilterTypeDef:
    return {
        "Key": ...,
    }


# OpsFilterTypeDef definition

class OpsFilterTypeDef(TypedDict):
    Key: str,
    Values: Sequence[str],
    Type: NotRequired[OpsFilterOperatorTypeType],  # (1)
```

1. See [:material-code-brackets: OpsFilterOperatorTypeType](./literals.md#opsfilteroperatortypetype) 
## OpsResultAttributeTypeDef

```python
# OpsResultAttributeTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import OpsResultAttributeTypeDef


def get_value() -> OpsResultAttributeTypeDef:
    return {
        "TypeName": ...,
    }


# OpsResultAttributeTypeDef definition

class OpsResultAttributeTypeDef(TypedDict):
    TypeName: str,
```

## GetParameterHistoryRequestTypeDef

```python
# GetParameterHistoryRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetParameterHistoryRequestTypeDef


def get_value() -> GetParameterHistoryRequestTypeDef:
    return {
        "Name": ...,
    }


# GetParameterHistoryRequestTypeDef definition

class GetParameterHistoryRequestTypeDef(TypedDict):
    Name: str,
    WithDecryption: NotRequired[bool],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetParameterRequestTypeDef

```python
# GetParameterRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetParameterRequestTypeDef


def get_value() -> GetParameterRequestTypeDef:
    return {
        "Name": ...,
    }


# GetParameterRequestTypeDef definition

class GetParameterRequestTypeDef(TypedDict):
    Name: str,
    WithDecryption: NotRequired[bool],
```

## ParameterTypeDef

```python
# ParameterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ParameterTypeDef


def get_value() -> ParameterTypeDef:
    return {
        "Name": ...,
    }


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
## GetParametersRequestTypeDef

```python
# GetParametersRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetParametersRequestTypeDef


def get_value() -> GetParametersRequestTypeDef:
    return {
        "Names": ...,
    }


# GetParametersRequestTypeDef definition

class GetParametersRequestTypeDef(TypedDict):
    Names: Sequence[str],
    WithDecryption: NotRequired[bool],
```

## GetPatchBaselineForPatchGroupRequestTypeDef

```python
# GetPatchBaselineForPatchGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetPatchBaselineForPatchGroupRequestTypeDef


def get_value() -> GetPatchBaselineForPatchGroupRequestTypeDef:
    return {
        "PatchGroup": ...,
    }


# GetPatchBaselineForPatchGroupRequestTypeDef definition

class GetPatchBaselineForPatchGroupRequestTypeDef(TypedDict):
    PatchGroup: str,
    OperatingSystem: NotRequired[OperatingSystemType],  # (1)
```

1. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
## GetPatchBaselineRequestTypeDef

```python
# GetPatchBaselineRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetPatchBaselineRequestTypeDef


def get_value() -> GetPatchBaselineRequestTypeDef:
    return {
        "BaselineId": ...,
    }


# GetPatchBaselineRequestTypeDef definition

class GetPatchBaselineRequestTypeDef(TypedDict):
    BaselineId: str,
```

## PatchSourceOutputTypeDef

```python
# PatchSourceOutputTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PatchSourceOutputTypeDef


def get_value() -> PatchSourceOutputTypeDef:
    return {
        "Name": ...,
    }


# PatchSourceOutputTypeDef definition

class PatchSourceOutputTypeDef(TypedDict):
    Name: str,
    Products: List[str],
    Configuration: str,
```

## GetResourcePoliciesRequestTypeDef

```python
# GetResourcePoliciesRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetResourcePoliciesRequestTypeDef


def get_value() -> GetResourcePoliciesRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# GetResourcePoliciesRequestTypeDef definition

class GetResourcePoliciesRequestTypeDef(TypedDict):
    ResourceArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetResourcePoliciesResponseEntryTypeDef

```python
# GetResourcePoliciesResponseEntryTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetResourcePoliciesResponseEntryTypeDef


def get_value() -> GetResourcePoliciesResponseEntryTypeDef:
    return {
        "PolicyId": ...,
    }


# GetResourcePoliciesResponseEntryTypeDef definition

class GetResourcePoliciesResponseEntryTypeDef(TypedDict):
    PolicyId: NotRequired[str],
    PolicyHash: NotRequired[str],
    Policy: NotRequired[str],
```

## GetServiceSettingRequestTypeDef

```python
# GetServiceSettingRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetServiceSettingRequestTypeDef


def get_value() -> GetServiceSettingRequestTypeDef:
    return {
        "SettingId": ...,
    }


# GetServiceSettingRequestTypeDef definition

class GetServiceSettingRequestTypeDef(TypedDict):
    SettingId: str,
```

## ServiceSettingTypeDef

```python
# ServiceSettingTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ServiceSettingTypeDef


def get_value() -> ServiceSettingTypeDef:
    return {
        "SettingId": ...,
    }


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
# InstanceAggregatedAssociationOverviewTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InstanceAggregatedAssociationOverviewTypeDef


def get_value() -> InstanceAggregatedAssociationOverviewTypeDef:
    return {
        "DetailedStatus": ...,
    }


# InstanceAggregatedAssociationOverviewTypeDef definition

class InstanceAggregatedAssociationOverviewTypeDef(TypedDict):
    DetailedStatus: NotRequired[str],
    InstanceAssociationStatusAggregatedCount: NotRequired[Dict[str, int]],
```

## S3OutputLocationTypeDef

```python
# S3OutputLocationTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import S3OutputLocationTypeDef


def get_value() -> S3OutputLocationTypeDef:
    return {
        "OutputS3Region": ...,
    }


# S3OutputLocationTypeDef definition

class S3OutputLocationTypeDef(TypedDict):
    OutputS3Region: NotRequired[str],
    OutputS3BucketName: NotRequired[str],
    OutputS3KeyPrefix: NotRequired[str],
```

## S3OutputUrlTypeDef

```python
# S3OutputUrlTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import S3OutputUrlTypeDef


def get_value() -> S3OutputUrlTypeDef:
    return {
        "OutputUrl": ...,
    }


# S3OutputUrlTypeDef definition

class S3OutputUrlTypeDef(TypedDict):
    OutputUrl: NotRequired[str],
```

## InstanceInfoTypeDef

```python
# InstanceInfoTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InstanceInfoTypeDef


def get_value() -> InstanceInfoTypeDef:
    return {
        "AgentType": ...,
    }


# InstanceInfoTypeDef definition

class InstanceInfoTypeDef(TypedDict):
    AgentType: NotRequired[str],
    AgentVersion: NotRequired[str],
    ComputerName: NotRequired[str],
    InstanceStatus: NotRequired[str],
    IpAddress: NotRequired[str],
    ManagedStatus: NotRequired[ManagedStatusType],  # (1)
    PlatformType: NotRequired[PlatformTypeType],  # (2)
    PlatformName: NotRequired[str],
    PlatformVersion: NotRequired[str],
    ResourceType: NotRequired[ResourceTypeType],  # (3)
```

1. See [:material-code-brackets: ManagedStatusType](./literals.md#managedstatustype) 
2. See [:material-code-brackets: PlatformTypeType](./literals.md#platformtypetype) 
3. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## InventoryDeletionSummaryItemTypeDef

```python
# InventoryDeletionSummaryItemTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InventoryDeletionSummaryItemTypeDef


def get_value() -> InventoryDeletionSummaryItemTypeDef:
    return {
        "Version": ...,
    }


# InventoryDeletionSummaryItemTypeDef definition

class InventoryDeletionSummaryItemTypeDef(TypedDict):
    Version: NotRequired[str],
    Count: NotRequired[int],
    RemainingCount: NotRequired[int],
```

## InventoryItemAttributeTypeDef

```python
# InventoryItemAttributeTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InventoryItemAttributeTypeDef


def get_value() -> InventoryItemAttributeTypeDef:
    return {
        "Name": ...,
    }


# InventoryItemAttributeTypeDef definition

class InventoryItemAttributeTypeDef(TypedDict):
    Name: str,
    DataType: InventoryAttributeDataTypeType,  # (1)
```

1. See [:material-code-brackets: InventoryAttributeDataTypeType](./literals.md#inventoryattributedatatypetype) 
## InventoryItemTypeDef

```python
# InventoryItemTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InventoryItemTypeDef


def get_value() -> InventoryItemTypeDef:
    return {
        "TypeName": ...,
    }


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
# InventoryResultItemTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InventoryResultItemTypeDef


def get_value() -> InventoryResultItemTypeDef:
    return {
        "TypeName": ...,
    }


# InventoryResultItemTypeDef definition

class InventoryResultItemTypeDef(TypedDict):
    TypeName: str,
    SchemaVersion: str,
    Content: List[Dict[str, str]],
    CaptureTime: NotRequired[str],
    ContentHash: NotRequired[str],
```

## LabelParameterVersionRequestTypeDef

```python
# LabelParameterVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import LabelParameterVersionRequestTypeDef


def get_value() -> LabelParameterVersionRequestTypeDef:
    return {
        "Name": ...,
    }


# LabelParameterVersionRequestTypeDef definition

class LabelParameterVersionRequestTypeDef(TypedDict):
    Name: str,
    Labels: Sequence[str],
    ParameterVersion: NotRequired[int],
```

## ListAssociationVersionsRequestTypeDef

```python
# ListAssociationVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListAssociationVersionsRequestTypeDef


def get_value() -> ListAssociationVersionsRequestTypeDef:
    return {
        "AssociationId": ...,
    }


# ListAssociationVersionsRequestTypeDef definition

class ListAssociationVersionsRequestTypeDef(TypedDict):
    AssociationId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListDocumentMetadataHistoryRequestTypeDef

```python
# ListDocumentMetadataHistoryRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListDocumentMetadataHistoryRequestTypeDef


def get_value() -> ListDocumentMetadataHistoryRequestTypeDef:
    return {
        "Name": ...,
    }


# ListDocumentMetadataHistoryRequestTypeDef definition

class ListDocumentMetadataHistoryRequestTypeDef(TypedDict):
    Name: str,
    Metadata: DocumentMetadataEnumType,  # (1)
    DocumentVersion: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: DocumentMetadataEnumType](./literals.md#documentmetadataenumtype) 
## ListDocumentVersionsRequestTypeDef

```python
# ListDocumentVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListDocumentVersionsRequestTypeDef


def get_value() -> ListDocumentVersionsRequestTypeDef:
    return {
        "Name": ...,
    }


# ListDocumentVersionsRequestTypeDef definition

class ListDocumentVersionsRequestTypeDef(TypedDict):
    Name: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## NodeFilterTypeDef

```python
# NodeFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import NodeFilterTypeDef


def get_value() -> NodeFilterTypeDef:
    return {
        "Key": ...,
    }


# NodeFilterTypeDef definition

class NodeFilterTypeDef(TypedDict):
    Key: NodeFilterKeyType,  # (1)
    Values: Sequence[str],
    Type: NotRequired[NodeFilterOperatorTypeType],  # (2)
```

1. See [:material-code-brackets: NodeFilterKeyType](./literals.md#nodefilterkeytype) 
2. See [:material-code-brackets: NodeFilterOperatorTypeType](./literals.md#nodefilteroperatortypetype) 
## NodeAggregatorPaginatorTypeDef

```python
# NodeAggregatorPaginatorTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import NodeAggregatorPaginatorTypeDef


def get_value() -> NodeAggregatorPaginatorTypeDef:
    return {
        "AggregatorType": ...,
    }


# NodeAggregatorPaginatorTypeDef definition

class NodeAggregatorPaginatorTypeDef(TypedDict):
    AggregatorType: NodeAggregatorTypeType,  # (1)
    TypeName: NodeTypeNameType,  # (2)
    AttributeName: NodeAttributeNameType,  # (3)
    Aggregators: NotRequired[Sequence[Mapping[str, Any]]],
```

1. See [:material-code-brackets: NodeAggregatorTypeType](./literals.md#nodeaggregatortypetype) 
2. See [:material-code-brackets: NodeTypeNameType](./literals.md#nodetypenametype) 
3. See [:material-code-brackets: NodeAttributeNameType](./literals.md#nodeattributenametype) 
## NodeAggregatorTypeDef

```python
# NodeAggregatorTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import NodeAggregatorTypeDef


def get_value() -> NodeAggregatorTypeDef:
    return {
        "AggregatorType": ...,
    }


# NodeAggregatorTypeDef definition

class NodeAggregatorTypeDef(TypedDict):
    AggregatorType: NodeAggregatorTypeType,  # (1)
    TypeName: NodeTypeNameType,  # (2)
    AttributeName: NodeAttributeNameType,  # (3)
    Aggregators: NotRequired[Sequence[Mapping[str, Any]]],
```

1. See [:material-code-brackets: NodeAggregatorTypeType](./literals.md#nodeaggregatortypetype) 
2. See [:material-code-brackets: NodeTypeNameType](./literals.md#nodetypenametype) 
3. See [:material-code-brackets: NodeAttributeNameType](./literals.md#nodeattributenametype) 
## OpsItemEventFilterTypeDef

```python
# OpsItemEventFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import OpsItemEventFilterTypeDef


def get_value() -> OpsItemEventFilterTypeDef:
    return {
        "Key": ...,
    }


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
# OpsItemRelatedItemsFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import OpsItemRelatedItemsFilterTypeDef


def get_value() -> OpsItemRelatedItemsFilterTypeDef:
    return {
        "Key": ...,
    }


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
# OpsMetadataFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import OpsMetadataFilterTypeDef


def get_value() -> OpsMetadataFilterTypeDef:
    return {
        "Key": ...,
    }


# OpsMetadataFilterTypeDef definition

class OpsMetadataFilterTypeDef(TypedDict):
    Key: str,
    Values: Sequence[str],
```

## OpsMetadataTypeDef

```python
# OpsMetadataTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import OpsMetadataTypeDef


def get_value() -> OpsMetadataTypeDef:
    return {
        "ResourceId": ...,
    }


# OpsMetadataTypeDef definition

class OpsMetadataTypeDef(TypedDict):
    ResourceId: NotRequired[str],
    OpsMetadataArn: NotRequired[str],
    LastModifiedDate: NotRequired[datetime],
    LastModifiedUser: NotRequired[str],
    CreationDate: NotRequired[datetime],
```

## ListResourceDataSyncRequestTypeDef

```python
# ListResourceDataSyncRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListResourceDataSyncRequestTypeDef


def get_value() -> ListResourceDataSyncRequestTypeDef:
    return {
        "SyncType": ...,
    }


# ListResourceDataSyncRequestTypeDef definition

class ListResourceDataSyncRequestTypeDef(TypedDict):
    SyncType: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "ResourceType": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    ResourceType: ResourceTypeForTaggingType,  # (1)
    ResourceId: str,
```

1. See [:material-code-brackets: ResourceTypeForTaggingType](./literals.md#resourcetypefortaggingtype) 
## MaintenanceWindowAutomationParametersOutputTypeDef

```python
# MaintenanceWindowAutomationParametersOutputTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import MaintenanceWindowAutomationParametersOutputTypeDef


def get_value() -> MaintenanceWindowAutomationParametersOutputTypeDef:
    return {
        "DocumentVersion": ...,
    }


# MaintenanceWindowAutomationParametersOutputTypeDef definition

class MaintenanceWindowAutomationParametersOutputTypeDef(TypedDict):
    DocumentVersion: NotRequired[str],
    Parameters: NotRequired[Dict[str, List[str]]],
```

## MaintenanceWindowAutomationParametersTypeDef

```python
# MaintenanceWindowAutomationParametersTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import MaintenanceWindowAutomationParametersTypeDef


def get_value() -> MaintenanceWindowAutomationParametersTypeDef:
    return {
        "DocumentVersion": ...,
    }


# MaintenanceWindowAutomationParametersTypeDef definition

class MaintenanceWindowAutomationParametersTypeDef(TypedDict):
    DocumentVersion: NotRequired[str],
    Parameters: NotRequired[Mapping[str, Sequence[str]]],
```

## MaintenanceWindowLambdaParametersOutputTypeDef

```python
# MaintenanceWindowLambdaParametersOutputTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import MaintenanceWindowLambdaParametersOutputTypeDef


def get_value() -> MaintenanceWindowLambdaParametersOutputTypeDef:
    return {
        "ClientContext": ...,
    }


# MaintenanceWindowLambdaParametersOutputTypeDef definition

class MaintenanceWindowLambdaParametersOutputTypeDef(TypedDict):
    ClientContext: NotRequired[str],
    Qualifier: NotRequired[str],
    Payload: NotRequired[bytes],
```

## NotificationConfigTypeDef

```python
# NotificationConfigTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import NotificationConfigTypeDef


def get_value() -> NotificationConfigTypeDef:
    return {
        "NotificationArn": ...,
    }


# NotificationConfigTypeDef definition

class NotificationConfigTypeDef(TypedDict):
    NotificationArn: NotRequired[str],
    NotificationEvents: NotRequired[Sequence[NotificationEventType]],  # (1)
    NotificationType: NotRequired[NotificationTypeType],  # (2)
```

1. See [:material-code-brackets: NotificationEventType](./literals.md#notificationeventtype) 
2. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
## MaintenanceWindowStepFunctionsParametersTypeDef

```python
# MaintenanceWindowStepFunctionsParametersTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import MaintenanceWindowStepFunctionsParametersTypeDef


def get_value() -> MaintenanceWindowStepFunctionsParametersTypeDef:
    return {
        "Input": ...,
    }


# MaintenanceWindowStepFunctionsParametersTypeDef definition

class MaintenanceWindowStepFunctionsParametersTypeDef(TypedDict):
    Input: NotRequired[str],
    Name: NotRequired[str],
```

## MaintenanceWindowTaskParameterValueExpressionTypeDef

```python
# MaintenanceWindowTaskParameterValueExpressionTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import MaintenanceWindowTaskParameterValueExpressionTypeDef


def get_value() -> MaintenanceWindowTaskParameterValueExpressionTypeDef:
    return {
        "Values": ...,
    }


# MaintenanceWindowTaskParameterValueExpressionTypeDef definition

class MaintenanceWindowTaskParameterValueExpressionTypeDef(TypedDict):
    Values: NotRequired[Sequence[str]],
```

## ModifyDocumentPermissionRequestTypeDef

```python
# ModifyDocumentPermissionRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ModifyDocumentPermissionRequestTypeDef


def get_value() -> ModifyDocumentPermissionRequestTypeDef:
    return {
        "Name": ...,
    }


# ModifyDocumentPermissionRequestTypeDef definition

class ModifyDocumentPermissionRequestTypeDef(TypedDict):
    Name: str,
    PermissionType: DocumentPermissionTypeType,  # (1)
    AccountIdsToAdd: NotRequired[Sequence[str]],
    AccountIdsToRemove: NotRequired[Sequence[str]],
    SharedDocumentVersion: NotRequired[str],
```

1. See [:material-code-brackets: DocumentPermissionTypeType](./literals.md#documentpermissiontypetype) 
## NodeOwnerInfoTypeDef

```python
# NodeOwnerInfoTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import NodeOwnerInfoTypeDef


def get_value() -> NodeOwnerInfoTypeDef:
    return {
        "AccountId": ...,
    }


# NodeOwnerInfoTypeDef definition

class NodeOwnerInfoTypeDef(TypedDict):
    AccountId: NotRequired[str],
    OrganizationalUnitId: NotRequired[str],
    OrganizationalUnitPath: NotRequired[str],
```

## OpsEntityItemTypeDef

```python
# OpsEntityItemTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import OpsEntityItemTypeDef


def get_value() -> OpsEntityItemTypeDef:
    return {
        "CaptureTime": ...,
    }


# OpsEntityItemTypeDef definition

class OpsEntityItemTypeDef(TypedDict):
    CaptureTime: NotRequired[str],
    Content: NotRequired[List[Dict[str, str]]],
```

## OpsItemIdentityTypeDef

```python
# OpsItemIdentityTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import OpsItemIdentityTypeDef


def get_value() -> OpsItemIdentityTypeDef:
    return {
        "Arn": ...,
    }


# OpsItemIdentityTypeDef definition

class OpsItemIdentityTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## ParameterInlinePolicyTypeDef

```python
# ParameterInlinePolicyTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ParameterInlinePolicyTypeDef


def get_value() -> ParameterInlinePolicyTypeDef:
    return {
        "PolicyText": ...,
    }


# ParameterInlinePolicyTypeDef definition

class ParameterInlinePolicyTypeDef(TypedDict):
    PolicyText: NotRequired[str],
    PolicyType: NotRequired[str],
    PolicyStatus: NotRequired[str],
```

## ParentStepDetailsTypeDef

```python
# ParentStepDetailsTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ParentStepDetailsTypeDef


def get_value() -> ParentStepDetailsTypeDef:
    return {
        "StepExecutionId": ...,
    }


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
# PatchFilterOutputTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PatchFilterOutputTypeDef


def get_value() -> PatchFilterOutputTypeDef:
    return {
        "Key": ...,
    }


# PatchFilterOutputTypeDef definition

class PatchFilterOutputTypeDef(TypedDict):
    Key: PatchFilterKeyType,  # (1)
    Values: List[str],
```

1. See [:material-code-brackets: PatchFilterKeyType](./literals.md#patchfilterkeytype) 
## PatchFilterTypeDef

```python
# PatchFilterTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PatchFilterTypeDef


def get_value() -> PatchFilterTypeDef:
    return {
        "Key": ...,
    }


# PatchFilterTypeDef definition

class PatchFilterTypeDef(TypedDict):
    Key: PatchFilterKeyType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: PatchFilterKeyType](./literals.md#patchfilterkeytype) 
## PatchSourceTypeDef

```python
# PatchSourceTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PatchSourceTypeDef


def get_value() -> PatchSourceTypeDef:
    return {
        "Name": ...,
    }


# PatchSourceTypeDef definition

class PatchSourceTypeDef(TypedDict):
    Name: str,
    Products: Sequence[str],
    Configuration: str,
```

## PutResourcePolicyRequestTypeDef

```python
# PutResourcePolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PutResourcePolicyRequestTypeDef


def get_value() -> PutResourcePolicyRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# PutResourcePolicyRequestTypeDef definition

class PutResourcePolicyRequestTypeDef(TypedDict):
    ResourceArn: str,
    Policy: str,
    PolicyId: NotRequired[str],
    PolicyHash: NotRequired[str],
```

## RegisterDefaultPatchBaselineRequestTypeDef

```python
# RegisterDefaultPatchBaselineRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import RegisterDefaultPatchBaselineRequestTypeDef


def get_value() -> RegisterDefaultPatchBaselineRequestTypeDef:
    return {
        "BaselineId": ...,
    }


# RegisterDefaultPatchBaselineRequestTypeDef definition

class RegisterDefaultPatchBaselineRequestTypeDef(TypedDict):
    BaselineId: str,
```

## RegisterPatchBaselineForPatchGroupRequestTypeDef

```python
# RegisterPatchBaselineForPatchGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import RegisterPatchBaselineForPatchGroupRequestTypeDef


def get_value() -> RegisterPatchBaselineForPatchGroupRequestTypeDef:
    return {
        "BaselineId": ...,
    }


# RegisterPatchBaselineForPatchGroupRequestTypeDef definition

class RegisterPatchBaselineForPatchGroupRequestTypeDef(TypedDict):
    BaselineId: str,
    PatchGroup: str,
```

## RemoveTagsFromResourceRequestTypeDef

```python
# RemoveTagsFromResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import RemoveTagsFromResourceRequestTypeDef


def get_value() -> RemoveTagsFromResourceRequestTypeDef:
    return {
        "ResourceType": ...,
    }


# RemoveTagsFromResourceRequestTypeDef definition

class RemoveTagsFromResourceRequestTypeDef(TypedDict):
    ResourceType: ResourceTypeForTaggingType,  # (1)
    ResourceId: str,
    TagKeys: Sequence[str],
```

1. See [:material-code-brackets: ResourceTypeForTaggingType](./literals.md#resourcetypefortaggingtype) 
## ResetServiceSettingRequestTypeDef

```python
# ResetServiceSettingRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ResetServiceSettingRequestTypeDef


def get_value() -> ResetServiceSettingRequestTypeDef:
    return {
        "SettingId": ...,
    }


# ResetServiceSettingRequestTypeDef definition

class ResetServiceSettingRequestTypeDef(TypedDict):
    SettingId: str,
```

## ResourceDataSyncOrganizationalUnitTypeDef

```python
# ResourceDataSyncOrganizationalUnitTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ResourceDataSyncOrganizationalUnitTypeDef


def get_value() -> ResourceDataSyncOrganizationalUnitTypeDef:
    return {
        "OrganizationalUnitId": ...,
    }


# ResourceDataSyncOrganizationalUnitTypeDef definition

class ResourceDataSyncOrganizationalUnitTypeDef(TypedDict):
    OrganizationalUnitId: NotRequired[str],
```

## ResourceDataSyncDestinationDataSharingTypeDef

```python
# ResourceDataSyncDestinationDataSharingTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ResourceDataSyncDestinationDataSharingTypeDef


def get_value() -> ResourceDataSyncDestinationDataSharingTypeDef:
    return {
        "DestinationDataSharingType": ...,
    }


# ResourceDataSyncDestinationDataSharingTypeDef definition

class ResourceDataSyncDestinationDataSharingTypeDef(TypedDict):
    DestinationDataSharingType: NotRequired[str],
```

## ResumeSessionRequestTypeDef

```python
# ResumeSessionRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ResumeSessionRequestTypeDef


def get_value() -> ResumeSessionRequestTypeDef:
    return {
        "SessionId": ...,
    }


# ResumeSessionRequestTypeDef definition

class ResumeSessionRequestTypeDef(TypedDict):
    SessionId: str,
```

## SendAutomationSignalRequestTypeDef

```python
# SendAutomationSignalRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import SendAutomationSignalRequestTypeDef


def get_value() -> SendAutomationSignalRequestTypeDef:
    return {
        "AutomationExecutionId": ...,
    }


# SendAutomationSignalRequestTypeDef definition

class SendAutomationSignalRequestTypeDef(TypedDict):
    AutomationExecutionId: str,
    SignalType: SignalTypeType,  # (1)
    Payload: NotRequired[Mapping[str, Sequence[str]]],
```

1. See [:material-code-brackets: SignalTypeType](./literals.md#signaltypetype) 
## SessionManagerOutputUrlTypeDef

```python
# SessionManagerOutputUrlTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import SessionManagerOutputUrlTypeDef


def get_value() -> SessionManagerOutputUrlTypeDef:
    return {
        "S3OutputUrl": ...,
    }


# SessionManagerOutputUrlTypeDef definition

class SessionManagerOutputUrlTypeDef(TypedDict):
    S3OutputUrl: NotRequired[str],
    CloudWatchOutputUrl: NotRequired[str],
```

## StartAssociationsOnceRequestTypeDef

```python
# StartAssociationsOnceRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import StartAssociationsOnceRequestTypeDef


def get_value() -> StartAssociationsOnceRequestTypeDef:
    return {
        "AssociationIds": ...,
    }


# StartAssociationsOnceRequestTypeDef definition

class StartAssociationsOnceRequestTypeDef(TypedDict):
    AssociationIds: Sequence[str],
```

## StartSessionRequestTypeDef

```python
# StartSessionRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import StartSessionRequestTypeDef


def get_value() -> StartSessionRequestTypeDef:
    return {
        "Target": ...,
    }


# StartSessionRequestTypeDef definition

class StartSessionRequestTypeDef(TypedDict):
    Target: str,
    DocumentName: NotRequired[str],
    Reason: NotRequired[str],
    Parameters: NotRequired[Mapping[str, Sequence[str]]],
```

## StopAutomationExecutionRequestTypeDef

```python
# StopAutomationExecutionRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import StopAutomationExecutionRequestTypeDef


def get_value() -> StopAutomationExecutionRequestTypeDef:
    return {
        "AutomationExecutionId": ...,
    }


# StopAutomationExecutionRequestTypeDef definition

class StopAutomationExecutionRequestTypeDef(TypedDict):
    AutomationExecutionId: str,
    Type: NotRequired[StopTypeType],  # (1)
```

1. See [:material-code-brackets: StopTypeType](./literals.md#stoptypetype) 
## TargetTypeDef

```python
# TargetTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import TargetTypeDef


def get_value() -> TargetTypeDef:
    return {
        "Key": ...,
    }


# TargetTypeDef definition

class TargetTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## TerminateSessionRequestTypeDef

```python
# TerminateSessionRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import TerminateSessionRequestTypeDef


def get_value() -> TerminateSessionRequestTypeDef:
    return {
        "SessionId": ...,
    }


# TerminateSessionRequestTypeDef definition

class TerminateSessionRequestTypeDef(TypedDict):
    SessionId: str,
```

## UnlabelParameterVersionRequestTypeDef

```python
# UnlabelParameterVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UnlabelParameterVersionRequestTypeDef


def get_value() -> UnlabelParameterVersionRequestTypeDef:
    return {
        "Name": ...,
    }


# UnlabelParameterVersionRequestTypeDef definition

class UnlabelParameterVersionRequestTypeDef(TypedDict):
    Name: str,
    ParameterVersion: int,
    Labels: Sequence[str],
```

## UpdateDocumentDefaultVersionRequestTypeDef

```python
# UpdateDocumentDefaultVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdateDocumentDefaultVersionRequestTypeDef


def get_value() -> UpdateDocumentDefaultVersionRequestTypeDef:
    return {
        "Name": ...,
    }


# UpdateDocumentDefaultVersionRequestTypeDef definition

class UpdateDocumentDefaultVersionRequestTypeDef(TypedDict):
    Name: str,
    DocumentVersion: str,
```

## UpdateMaintenanceWindowRequestTypeDef

```python
# UpdateMaintenanceWindowRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdateMaintenanceWindowRequestTypeDef


def get_value() -> UpdateMaintenanceWindowRequestTypeDef:
    return {
        "WindowId": ...,
    }


# UpdateMaintenanceWindowRequestTypeDef definition

class UpdateMaintenanceWindowRequestTypeDef(TypedDict):
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

## UpdateManagedInstanceRoleRequestTypeDef

```python
# UpdateManagedInstanceRoleRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdateManagedInstanceRoleRequestTypeDef


def get_value() -> UpdateManagedInstanceRoleRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateManagedInstanceRoleRequestTypeDef definition

class UpdateManagedInstanceRoleRequestTypeDef(TypedDict):
    InstanceId: str,
    IamRole: str,
```

## UpdateServiceSettingRequestTypeDef

```python
# UpdateServiceSettingRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdateServiceSettingRequestTypeDef


def get_value() -> UpdateServiceSettingRequestTypeDef:
    return {
        "SettingId": ...,
    }


# UpdateServiceSettingRequestTypeDef definition

class UpdateServiceSettingRequestTypeDef(TypedDict):
    SettingId: str,
    SettingValue: str,
```

## ActivationTypeDef

```python
# ActivationTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ActivationTypeDef


def get_value() -> ActivationTypeDef:
    return {
        "ActivationId": ...,
    }


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
## AddTagsToResourceRequestTypeDef

```python
# AddTagsToResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AddTagsToResourceRequestTypeDef


def get_value() -> AddTagsToResourceRequestTypeDef:
    return {
        "ResourceType": ...,
    }


# AddTagsToResourceRequestTypeDef definition

class AddTagsToResourceRequestTypeDef(TypedDict):
    ResourceType: ResourceTypeForTaggingType,  # (1)
    ResourceId: str,
    Tags: Sequence[TagTypeDef],  # (2)
```

1. See [:material-code-brackets: ResourceTypeForTaggingType](./literals.md#resourcetypefortaggingtype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateMaintenanceWindowRequestTypeDef

```python
# CreateMaintenanceWindowRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CreateMaintenanceWindowRequestTypeDef


def get_value() -> CreateMaintenanceWindowRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateMaintenanceWindowRequestTypeDef definition

class CreateMaintenanceWindowRequestTypeDef(TypedDict):
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
## PutParameterRequestTypeDef

```python
# PutParameterRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PutParameterRequestTypeDef


def get_value() -> PutParameterRequestTypeDef:
    return {
        "Name": ...,
    }


# PutParameterRequestTypeDef definition

class PutParameterRequestTypeDef(TypedDict):
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
# AlarmConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AlarmConfigurationOutputTypeDef


def get_value() -> AlarmConfigurationOutputTypeDef:
    return {
        "IgnorePollAlarmFailure": ...,
    }


# AlarmConfigurationOutputTypeDef definition

class AlarmConfigurationOutputTypeDef(TypedDict):
    Alarms: List[AlarmTypeDef],  # (1)
    IgnorePollAlarmFailure: NotRequired[bool],
```

1. See [:material-code-braces: AlarmTypeDef](./type_defs.md#alarmtypedef) 
## AlarmConfigurationTypeDef

```python
# AlarmConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AlarmConfigurationTypeDef


def get_value() -> AlarmConfigurationTypeDef:
    return {
        "IgnorePollAlarmFailure": ...,
    }


# AlarmConfigurationTypeDef definition

class AlarmConfigurationTypeDef(TypedDict):
    Alarms: Sequence[AlarmTypeDef],  # (1)
    IgnorePollAlarmFailure: NotRequired[bool],
```

1. See [:material-code-braces: AlarmTypeDef](./type_defs.md#alarmtypedef) 
## AssociateOpsItemRelatedItemResponseTypeDef

```python
# AssociateOpsItemRelatedItemResponseTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AssociateOpsItemRelatedItemResponseTypeDef


def get_value() -> AssociateOpsItemRelatedItemResponseTypeDef:
    return {
        "AssociationId": ...,
    }


# AssociateOpsItemRelatedItemResponseTypeDef definition

class AssociateOpsItemRelatedItemResponseTypeDef(TypedDict):
    AssociationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelMaintenanceWindowExecutionResultTypeDef

```python
# CancelMaintenanceWindowExecutionResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CancelMaintenanceWindowExecutionResultTypeDef


def get_value() -> CancelMaintenanceWindowExecutionResultTypeDef:
    return {
        "WindowExecutionId": ...,
    }


# CancelMaintenanceWindowExecutionResultTypeDef definition

class CancelMaintenanceWindowExecutionResultTypeDef(TypedDict):
    WindowExecutionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateActivationResultTypeDef

```python
# CreateActivationResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CreateActivationResultTypeDef


def get_value() -> CreateActivationResultTypeDef:
    return {
        "ActivationId": ...,
    }


# CreateActivationResultTypeDef definition

class CreateActivationResultTypeDef(TypedDict):
    ActivationId: str,
    ActivationCode: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMaintenanceWindowResultTypeDef

```python
# CreateMaintenanceWindowResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CreateMaintenanceWindowResultTypeDef


def get_value() -> CreateMaintenanceWindowResultTypeDef:
    return {
        "WindowId": ...,
    }


# CreateMaintenanceWindowResultTypeDef definition

class CreateMaintenanceWindowResultTypeDef(TypedDict):
    WindowId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateOpsItemResponseTypeDef

```python
# CreateOpsItemResponseTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CreateOpsItemResponseTypeDef


def get_value() -> CreateOpsItemResponseTypeDef:
    return {
        "OpsItemId": ...,
    }


# CreateOpsItemResponseTypeDef definition

class CreateOpsItemResponseTypeDef(TypedDict):
    OpsItemId: str,
    OpsItemArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateOpsMetadataResultTypeDef

```python
# CreateOpsMetadataResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CreateOpsMetadataResultTypeDef


def get_value() -> CreateOpsMetadataResultTypeDef:
    return {
        "OpsMetadataArn": ...,
    }


# CreateOpsMetadataResultTypeDef definition

class CreateOpsMetadataResultTypeDef(TypedDict):
    OpsMetadataArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePatchBaselineResultTypeDef

```python
# CreatePatchBaselineResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CreatePatchBaselineResultTypeDef


def get_value() -> CreatePatchBaselineResultTypeDef:
    return {
        "BaselineId": ...,
    }


# CreatePatchBaselineResultTypeDef definition

class CreatePatchBaselineResultTypeDef(TypedDict):
    BaselineId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteMaintenanceWindowResultTypeDef

```python
# DeleteMaintenanceWindowResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeleteMaintenanceWindowResultTypeDef


def get_value() -> DeleteMaintenanceWindowResultTypeDef:
    return {
        "WindowId": ...,
    }


# DeleteMaintenanceWindowResultTypeDef definition

class DeleteMaintenanceWindowResultTypeDef(TypedDict):
    WindowId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteParametersResultTypeDef

```python
# DeleteParametersResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeleteParametersResultTypeDef


def get_value() -> DeleteParametersResultTypeDef:
    return {
        "DeletedParameters": ...,
    }


# DeleteParametersResultTypeDef definition

class DeleteParametersResultTypeDef(TypedDict):
    DeletedParameters: List[str],
    InvalidParameters: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePatchBaselineResultTypeDef

```python
# DeletePatchBaselineResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeletePatchBaselineResultTypeDef


def get_value() -> DeletePatchBaselineResultTypeDef:
    return {
        "BaselineId": ...,
    }


# DeletePatchBaselineResultTypeDef definition

class DeletePatchBaselineResultTypeDef(TypedDict):
    BaselineId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeregisterPatchBaselineForPatchGroupResultTypeDef

```python
# DeregisterPatchBaselineForPatchGroupResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeregisterPatchBaselineForPatchGroupResultTypeDef


def get_value() -> DeregisterPatchBaselineForPatchGroupResultTypeDef:
    return {
        "BaselineId": ...,
    }


# DeregisterPatchBaselineForPatchGroupResultTypeDef definition

class DeregisterPatchBaselineForPatchGroupResultTypeDef(TypedDict):
    BaselineId: str,
    PatchGroup: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeregisterTargetFromMaintenanceWindowResultTypeDef

```python
# DeregisterTargetFromMaintenanceWindowResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeregisterTargetFromMaintenanceWindowResultTypeDef


def get_value() -> DeregisterTargetFromMaintenanceWindowResultTypeDef:
    return {
        "WindowId": ...,
    }


# DeregisterTargetFromMaintenanceWindowResultTypeDef definition

class DeregisterTargetFromMaintenanceWindowResultTypeDef(TypedDict):
    WindowId: str,
    WindowTargetId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeregisterTaskFromMaintenanceWindowResultTypeDef

```python
# DeregisterTaskFromMaintenanceWindowResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeregisterTaskFromMaintenanceWindowResultTypeDef


def get_value() -> DeregisterTaskFromMaintenanceWindowResultTypeDef:
    return {
        "WindowId": ...,
    }


# DeregisterTaskFromMaintenanceWindowResultTypeDef definition

class DeregisterTaskFromMaintenanceWindowResultTypeDef(TypedDict):
    WindowId: str,
    WindowTaskId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDocumentPermissionResponseTypeDef

```python
# DescribeDocumentPermissionResponseTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeDocumentPermissionResponseTypeDef


def get_value() -> DescribeDocumentPermissionResponseTypeDef:
    return {
        "AccountIds": ...,
    }


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
# DescribePatchGroupStateResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribePatchGroupStateResultTypeDef


def get_value() -> DescribePatchGroupStateResultTypeDef:
    return {
        "Instances": ...,
    }


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
# DescribePatchPropertiesResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribePatchPropertiesResultTypeDef


def get_value() -> DescribePatchPropertiesResultTypeDef:
    return {
        "Properties": ...,
    }


# DescribePatchPropertiesResultTypeDef definition

class DescribePatchPropertiesResultTypeDef(TypedDict):
    Properties: List[Dict[str, str]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCalendarStateResponseTypeDef

```python
# GetCalendarStateResponseTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetCalendarStateResponseTypeDef


def get_value() -> GetCalendarStateResponseTypeDef:
    return {
        "State": ...,
    }


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
# GetConnectionStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetConnectionStatusResponseTypeDef


def get_value() -> GetConnectionStatusResponseTypeDef:
    return {
        "Target": ...,
    }


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
# GetDefaultPatchBaselineResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetDefaultPatchBaselineResultTypeDef


def get_value() -> GetDefaultPatchBaselineResultTypeDef:
    return {
        "BaselineId": ...,
    }


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
# GetDeployablePatchSnapshotForInstanceResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetDeployablePatchSnapshotForInstanceResultTypeDef


def get_value() -> GetDeployablePatchSnapshotForInstanceResultTypeDef:
    return {
        "InstanceId": ...,
    }


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
# GetMaintenanceWindowExecutionResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetMaintenanceWindowExecutionResultTypeDef


def get_value() -> GetMaintenanceWindowExecutionResultTypeDef:
    return {
        "WindowExecutionId": ...,
    }


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
# GetMaintenanceWindowExecutionTaskInvocationResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetMaintenanceWindowExecutionTaskInvocationResultTypeDef


def get_value() -> GetMaintenanceWindowExecutionTaskInvocationResultTypeDef:
    return {
        "WindowExecutionId": ...,
    }


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
# GetMaintenanceWindowResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetMaintenanceWindowResultTypeDef


def get_value() -> GetMaintenanceWindowResultTypeDef:
    return {
        "WindowId": ...,
    }


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
# GetPatchBaselineForPatchGroupResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetPatchBaselineForPatchGroupResultTypeDef


def get_value() -> GetPatchBaselineForPatchGroupResultTypeDef:
    return {
        "BaselineId": ...,
    }


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
# LabelParameterVersionResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import LabelParameterVersionResultTypeDef


def get_value() -> LabelParameterVersionResultTypeDef:
    return {
        "InvalidLabels": ...,
    }


# LabelParameterVersionResultTypeDef definition

class LabelParameterVersionResultTypeDef(TypedDict):
    InvalidLabels: List[str],
    ParameterVersion: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInventoryEntriesResultTypeDef

```python
# ListInventoryEntriesResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListInventoryEntriesResultTypeDef


def get_value() -> ListInventoryEntriesResultTypeDef:
    return {
        "TypeName": ...,
    }


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
## ListNodesSummaryResultTypeDef

```python
# ListNodesSummaryResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListNodesSummaryResultTypeDef


def get_value() -> ListNodesSummaryResultTypeDef:
    return {
        "Summary": ...,
    }


# ListNodesSummaryResultTypeDef definition

class ListNodesSummaryResultTypeDef(TypedDict):
    Summary: List[Dict[str, str]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResultTypeDef

```python
# ListTagsForResourceResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListTagsForResourceResultTypeDef


def get_value() -> ListTagsForResourceResultTypeDef:
    return {
        "TagList": ...,
    }


# ListTagsForResourceResultTypeDef definition

class ListTagsForResourceResultTypeDef(TypedDict):
    TagList: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutInventoryResultTypeDef

```python
# PutInventoryResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PutInventoryResultTypeDef


def get_value() -> PutInventoryResultTypeDef:
    return {
        "Message": ...,
    }


# PutInventoryResultTypeDef definition

class PutInventoryResultTypeDef(TypedDict):
    Message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutParameterResultTypeDef

```python
# PutParameterResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PutParameterResultTypeDef


def get_value() -> PutParameterResultTypeDef:
    return {
        "Version": ...,
    }


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
# PutResourcePolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PutResourcePolicyResponseTypeDef


def get_value() -> PutResourcePolicyResponseTypeDef:
    return {
        "PolicyId": ...,
    }


# PutResourcePolicyResponseTypeDef definition

class PutResourcePolicyResponseTypeDef(TypedDict):
    PolicyId: str,
    PolicyHash: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterDefaultPatchBaselineResultTypeDef

```python
# RegisterDefaultPatchBaselineResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import RegisterDefaultPatchBaselineResultTypeDef


def get_value() -> RegisterDefaultPatchBaselineResultTypeDef:
    return {
        "BaselineId": ...,
    }


# RegisterDefaultPatchBaselineResultTypeDef definition

class RegisterDefaultPatchBaselineResultTypeDef(TypedDict):
    BaselineId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterPatchBaselineForPatchGroupResultTypeDef

```python
# RegisterPatchBaselineForPatchGroupResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import RegisterPatchBaselineForPatchGroupResultTypeDef


def get_value() -> RegisterPatchBaselineForPatchGroupResultTypeDef:
    return {
        "BaselineId": ...,
    }


# RegisterPatchBaselineForPatchGroupResultTypeDef definition

class RegisterPatchBaselineForPatchGroupResultTypeDef(TypedDict):
    BaselineId: str,
    PatchGroup: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterTargetWithMaintenanceWindowResultTypeDef

```python
# RegisterTargetWithMaintenanceWindowResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import RegisterTargetWithMaintenanceWindowResultTypeDef


def get_value() -> RegisterTargetWithMaintenanceWindowResultTypeDef:
    return {
        "WindowTargetId": ...,
    }


# RegisterTargetWithMaintenanceWindowResultTypeDef definition

class RegisterTargetWithMaintenanceWindowResultTypeDef(TypedDict):
    WindowTargetId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterTaskWithMaintenanceWindowResultTypeDef

```python
# RegisterTaskWithMaintenanceWindowResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import RegisterTaskWithMaintenanceWindowResultTypeDef


def get_value() -> RegisterTaskWithMaintenanceWindowResultTypeDef:
    return {
        "WindowTaskId": ...,
    }


# RegisterTaskWithMaintenanceWindowResultTypeDef definition

class RegisterTaskWithMaintenanceWindowResultTypeDef(TypedDict):
    WindowTaskId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResumeSessionResponseTypeDef

```python
# ResumeSessionResponseTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ResumeSessionResponseTypeDef


def get_value() -> ResumeSessionResponseTypeDef:
    return {
        "SessionId": ...,
    }


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
# StartAutomationExecutionResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import StartAutomationExecutionResultTypeDef


def get_value() -> StartAutomationExecutionResultTypeDef:
    return {
        "AutomationExecutionId": ...,
    }


# StartAutomationExecutionResultTypeDef definition

class StartAutomationExecutionResultTypeDef(TypedDict):
    AutomationExecutionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartChangeRequestExecutionResultTypeDef

```python
# StartChangeRequestExecutionResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import StartChangeRequestExecutionResultTypeDef


def get_value() -> StartChangeRequestExecutionResultTypeDef:
    return {
        "AutomationExecutionId": ...,
    }


# StartChangeRequestExecutionResultTypeDef definition

class StartChangeRequestExecutionResultTypeDef(TypedDict):
    AutomationExecutionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartExecutionPreviewResponseTypeDef

```python
# StartExecutionPreviewResponseTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import StartExecutionPreviewResponseTypeDef


def get_value() -> StartExecutionPreviewResponseTypeDef:
    return {
        "ExecutionPreviewId": ...,
    }


# StartExecutionPreviewResponseTypeDef definition

class StartExecutionPreviewResponseTypeDef(TypedDict):
    ExecutionPreviewId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSessionResponseTypeDef

```python
# StartSessionResponseTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import StartSessionResponseTypeDef


def get_value() -> StartSessionResponseTypeDef:
    return {
        "SessionId": ...,
    }


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
# TerminateSessionResponseTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import TerminateSessionResponseTypeDef


def get_value() -> TerminateSessionResponseTypeDef:
    return {
        "SessionId": ...,
    }


# TerminateSessionResponseTypeDef definition

class TerminateSessionResponseTypeDef(TypedDict):
    SessionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UnlabelParameterVersionResultTypeDef

```python
# UnlabelParameterVersionResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UnlabelParameterVersionResultTypeDef


def get_value() -> UnlabelParameterVersionResultTypeDef:
    return {
        "RemovedLabels": ...,
    }


# UnlabelParameterVersionResultTypeDef definition

class UnlabelParameterVersionResultTypeDef(TypedDict):
    RemovedLabels: List[str],
    InvalidLabels: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMaintenanceWindowResultTypeDef

```python
# UpdateMaintenanceWindowResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdateMaintenanceWindowResultTypeDef


def get_value() -> UpdateMaintenanceWindowResultTypeDef:
    return {
        "WindowId": ...,
    }


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
# UpdateOpsMetadataResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdateOpsMetadataResultTypeDef


def get_value() -> UpdateOpsMetadataResultTypeDef:
    return {
        "OpsMetadataArn": ...,
    }


# UpdateOpsMetadataResultTypeDef definition

class UpdateOpsMetadataResultTypeDef(TypedDict):
    OpsMetadataArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociationTypeDef

```python
# AssociationTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AssociationTypeDef


def get_value() -> AssociationTypeDef:
    return {
        "Name": ...,
    }


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
# MaintenanceWindowTargetTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import MaintenanceWindowTargetTypeDef


def get_value() -> MaintenanceWindowTargetTypeDef:
    return {
        "WindowId": ...,
    }


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
# UpdateMaintenanceWindowTargetResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdateMaintenanceWindowTargetResultTypeDef


def get_value() -> UpdateMaintenanceWindowTargetResultTypeDef:
    return {
        "WindowId": ...,
    }


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
## DescribeAssociationExecutionsRequestTypeDef

```python
# DescribeAssociationExecutionsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeAssociationExecutionsRequestTypeDef


def get_value() -> DescribeAssociationExecutionsRequestTypeDef:
    return {
        "AssociationId": ...,
    }


# DescribeAssociationExecutionsRequestTypeDef definition

class DescribeAssociationExecutionsRequestTypeDef(TypedDict):
    AssociationId: str,
    Filters: NotRequired[Sequence[AssociationExecutionFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AssociationExecutionFilterTypeDef](./type_defs.md#associationexecutionfiltertypedef) 
## AssociationExecutionTargetTypeDef

```python
# AssociationExecutionTargetTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AssociationExecutionTargetTypeDef


def get_value() -> AssociationExecutionTargetTypeDef:
    return {
        "AssociationId": ...,
    }


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
## DescribeAssociationExecutionTargetsRequestTypeDef

```python
# DescribeAssociationExecutionTargetsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeAssociationExecutionTargetsRequestTypeDef


def get_value() -> DescribeAssociationExecutionTargetsRequestTypeDef:
    return {
        "AssociationId": ...,
    }


# DescribeAssociationExecutionTargetsRequestTypeDef definition

class DescribeAssociationExecutionTargetsRequestTypeDef(TypedDict):
    AssociationId: str,
    ExecutionId: str,
    Filters: NotRequired[Sequence[AssociationExecutionTargetsFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AssociationExecutionTargetsFilterTypeDef](./type_defs.md#associationexecutiontargetsfiltertypedef) 
## ListAssociationsRequestTypeDef

```python
# ListAssociationsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListAssociationsRequestTypeDef


def get_value() -> ListAssociationsRequestTypeDef:
    return {
        "AssociationFilterList": ...,
    }


# ListAssociationsRequestTypeDef definition

class ListAssociationsRequestTypeDef(TypedDict):
    AssociationFilterList: NotRequired[Sequence[AssociationFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AssociationFilterTypeDef](./type_defs.md#associationfiltertypedef) 
## AssociationStatusTypeDef

```python
# AssociationStatusTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AssociationStatusTypeDef


def get_value() -> AssociationStatusTypeDef:
    return {
        "Date": ...,
    }


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
# ComplianceExecutionSummaryTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ComplianceExecutionSummaryTypeDef


def get_value() -> ComplianceExecutionSummaryTypeDef:
    return {
        "ExecutionTime": ...,
    }


# ComplianceExecutionSummaryTypeDef definition

class ComplianceExecutionSummaryTypeDef(TypedDict):
    ExecutionTime: TimestampTypeDef,
    ExecutionId: NotRequired[str],
    ExecutionType: NotRequired[str],
```

## UpdateDocumentRequestTypeDef

```python
# UpdateDocumentRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdateDocumentRequestTypeDef


def get_value() -> UpdateDocumentRequestTypeDef:
    return {
        "Content": ...,
    }


# UpdateDocumentRequestTypeDef definition

class UpdateDocumentRequestTypeDef(TypedDict):
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
## DescribeAutomationExecutionsRequestTypeDef

```python
# DescribeAutomationExecutionsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeAutomationExecutionsRequestTypeDef


def get_value() -> DescribeAutomationExecutionsRequestTypeDef:
    return {
        "Filters": ...,
    }


# DescribeAutomationExecutionsRequestTypeDef definition

class DescribeAutomationExecutionsRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[AutomationExecutionFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AutomationExecutionFilterTypeDef](./type_defs.md#automationexecutionfiltertypedef) 
## AutomationExecutionPreviewTypeDef

```python
# AutomationExecutionPreviewTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AutomationExecutionPreviewTypeDef


def get_value() -> AutomationExecutionPreviewTypeDef:
    return {
        "StepPreviews": ...,
    }


# AutomationExecutionPreviewTypeDef definition

class AutomationExecutionPreviewTypeDef(TypedDict):
    StepPreviews: NotRequired[Dict[ImpactTypeType, int]],  # (1)
    Regions: NotRequired[List[str]],
    TargetPreviews: NotRequired[List[TargetPreviewTypeDef]],  # (2)
    TotalAccounts: NotRequired[int],
```

1. See [:material-code-brackets: ImpactTypeType](./literals.md#impacttypetype) 
2. See [:material-code-braces: TargetPreviewTypeDef](./type_defs.md#targetpreviewtypedef) 
## MaintenanceWindowLambdaParametersTypeDef

```python
# MaintenanceWindowLambdaParametersTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import MaintenanceWindowLambdaParametersTypeDef


def get_value() -> MaintenanceWindowLambdaParametersTypeDef:
    return {
        "ClientContext": ...,
    }


# MaintenanceWindowLambdaParametersTypeDef definition

class MaintenanceWindowLambdaParametersTypeDef(TypedDict):
    ClientContext: NotRequired[str],
    Qualifier: NotRequired[str],
    Payload: NotRequired[BlobTypeDef],
```

## GetCommandInvocationResultTypeDef

```python
# GetCommandInvocationResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetCommandInvocationResultTypeDef


def get_value() -> GetCommandInvocationResultTypeDef:
    return {
        "CommandId": ...,
    }


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
## ListCommandInvocationsRequestTypeDef

```python
# ListCommandInvocationsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListCommandInvocationsRequestTypeDef


def get_value() -> ListCommandInvocationsRequestTypeDef:
    return {
        "CommandId": ...,
    }


# ListCommandInvocationsRequestTypeDef definition

class ListCommandInvocationsRequestTypeDef(TypedDict):
    CommandId: NotRequired[str],
    InstanceId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[CommandFilterTypeDef]],  # (1)
    Details: NotRequired[bool],
```

1. See [:material-code-braces: CommandFilterTypeDef](./type_defs.md#commandfiltertypedef) 
## ListCommandsRequestTypeDef

```python
# ListCommandsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListCommandsRequestTypeDef


def get_value() -> ListCommandsRequestTypeDef:
    return {
        "CommandId": ...,
    }


# ListCommandsRequestTypeDef definition

class ListCommandsRequestTypeDef(TypedDict):
    CommandId: NotRequired[str],
    InstanceId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[CommandFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: CommandFilterTypeDef](./type_defs.md#commandfiltertypedef) 
## CommandInvocationTypeDef

```python
# CommandInvocationTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CommandInvocationTypeDef


def get_value() -> CommandInvocationTypeDef:
    return {
        "CommandId": ...,
    }


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
# MaintenanceWindowRunCommandParametersOutputTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import MaintenanceWindowRunCommandParametersOutputTypeDef


def get_value() -> MaintenanceWindowRunCommandParametersOutputTypeDef:
    return {
        "Comment": ...,
    }


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
# ComplianceItemTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ComplianceItemTypeDef


def get_value() -> ComplianceItemTypeDef:
    return {
        "ComplianceType": ...,
    }


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
## ListComplianceItemsRequestTypeDef

```python
# ListComplianceItemsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListComplianceItemsRequestTypeDef


def get_value() -> ListComplianceItemsRequestTypeDef:
    return {
        "Filters": ...,
    }


# ListComplianceItemsRequestTypeDef definition

class ListComplianceItemsRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ComplianceStringFilterTypeDef]],  # (1)
    ResourceIds: NotRequired[Sequence[str]],
    ResourceTypes: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ComplianceStringFilterTypeDef](./type_defs.md#compliancestringfiltertypedef) 
## ListComplianceSummariesRequestTypeDef

```python
# ListComplianceSummariesRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListComplianceSummariesRequestTypeDef


def get_value() -> ListComplianceSummariesRequestTypeDef:
    return {
        "Filters": ...,
    }


# ListComplianceSummariesRequestTypeDef definition

class ListComplianceSummariesRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ComplianceStringFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ComplianceStringFilterTypeDef](./type_defs.md#compliancestringfiltertypedef) 
## ListResourceComplianceSummariesRequestTypeDef

```python
# ListResourceComplianceSummariesRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListResourceComplianceSummariesRequestTypeDef


def get_value() -> ListResourceComplianceSummariesRequestTypeDef:
    return {
        "Filters": ...,
    }


# ListResourceComplianceSummariesRequestTypeDef definition

class ListResourceComplianceSummariesRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ComplianceStringFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ComplianceStringFilterTypeDef](./type_defs.md#compliancestringfiltertypedef) 
## CompliantSummaryTypeDef

```python
# CompliantSummaryTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CompliantSummaryTypeDef


def get_value() -> CompliantSummaryTypeDef:
    return {
        "CompliantCount": ...,
    }


# CompliantSummaryTypeDef definition

class CompliantSummaryTypeDef(TypedDict):
    CompliantCount: NotRequired[int],
    SeveritySummary: NotRequired[SeveritySummaryTypeDef],  # (1)
```

1. See [:material-code-braces: SeveritySummaryTypeDef](./type_defs.md#severitysummarytypedef) 
## NonCompliantSummaryTypeDef

```python
# NonCompliantSummaryTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import NonCompliantSummaryTypeDef


def get_value() -> NonCompliantSummaryTypeDef:
    return {
        "NonCompliantCount": ...,
    }


# NonCompliantSummaryTypeDef definition

class NonCompliantSummaryTypeDef(TypedDict):
    NonCompliantCount: NotRequired[int],
    SeveritySummary: NotRequired[SeveritySummaryTypeDef],  # (1)
```

1. See [:material-code-braces: SeveritySummaryTypeDef](./type_defs.md#severitysummarytypedef) 
## CreateActivationRequestTypeDef

```python
# CreateActivationRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CreateActivationRequestTypeDef


def get_value() -> CreateActivationRequestTypeDef:
    return {
        "IamRole": ...,
    }


# CreateActivationRequestTypeDef definition

class CreateActivationRequestTypeDef(TypedDict):
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
## CreateDocumentRequestTypeDef

```python
# CreateDocumentRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CreateDocumentRequestTypeDef


def get_value() -> CreateDocumentRequestTypeDef:
    return {
        "Content": ...,
    }


# CreateDocumentRequestTypeDef definition

class CreateDocumentRequestTypeDef(TypedDict):
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
# DocumentIdentifierTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DocumentIdentifierTypeDef


def get_value() -> DocumentIdentifierTypeDef:
    return {
        "Name": ...,
    }


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
# GetDocumentResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetDocumentResultTypeDef


def get_value() -> GetDocumentResultTypeDef:
    return {
        "Name": ...,
    }


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
# OpsItemSummaryTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import OpsItemSummaryTypeDef


def get_value() -> OpsItemSummaryTypeDef:
    return {
        "CreatedBy": ...,
    }


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
## CreateOpsItemRequestTypeDef

```python
# CreateOpsItemRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CreateOpsItemRequestTypeDef


def get_value() -> CreateOpsItemRequestTypeDef:
    return {
        "Description": ...,
    }


# CreateOpsItemRequestTypeDef definition

class CreateOpsItemRequestTypeDef(TypedDict):
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
# OpsItemTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import OpsItemTypeDef


def get_value() -> OpsItemTypeDef:
    return {
        "CreatedBy": ...,
    }


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
## UpdateOpsItemRequestTypeDef

```python
# UpdateOpsItemRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdateOpsItemRequestTypeDef


def get_value() -> UpdateOpsItemRequestTypeDef:
    return {
        "OpsItemId": ...,
    }


# UpdateOpsItemRequestTypeDef definition

class UpdateOpsItemRequestTypeDef(TypedDict):
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
## CreateOpsMetadataRequestTypeDef

```python
# CreateOpsMetadataRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CreateOpsMetadataRequestTypeDef


def get_value() -> CreateOpsMetadataRequestTypeDef:
    return {
        "ResourceId": ...,
    }


# CreateOpsMetadataRequestTypeDef definition

class CreateOpsMetadataRequestTypeDef(TypedDict):
    ResourceId: str,
    Metadata: NotRequired[Mapping[str, MetadataValueTypeDef]],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: MetadataValueTypeDef](./type_defs.md#metadatavaluetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetOpsMetadataResultTypeDef

```python
# GetOpsMetadataResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetOpsMetadataResultTypeDef


def get_value() -> GetOpsMetadataResultTypeDef:
    return {
        "ResourceId": ...,
    }


# GetOpsMetadataResultTypeDef definition

class GetOpsMetadataResultTypeDef(TypedDict):
    ResourceId: str,
    Metadata: Dict[str, MetadataValueTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MetadataValueTypeDef](./type_defs.md#metadatavaluetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateOpsMetadataRequestTypeDef

```python
# UpdateOpsMetadataRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdateOpsMetadataRequestTypeDef


def get_value() -> UpdateOpsMetadataRequestTypeDef:
    return {
        "OpsMetadataArn": ...,
    }


# UpdateOpsMetadataRequestTypeDef definition

class UpdateOpsMetadataRequestTypeDef(TypedDict):
    OpsMetadataArn: str,
    MetadataToUpdate: NotRequired[Mapping[str, MetadataValueTypeDef]],  # (1)
    KeysToDelete: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: MetadataValueTypeDef](./type_defs.md#metadatavaluetypedef) 
## DescribeActivationsRequestTypeDef

```python
# DescribeActivationsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeActivationsRequestTypeDef


def get_value() -> DescribeActivationsRequestTypeDef:
    return {
        "Filters": ...,
    }


# DescribeActivationsRequestTypeDef definition

class DescribeActivationsRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[DescribeActivationsFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DescribeActivationsFilterTypeDef](./type_defs.md#describeactivationsfiltertypedef) 
## DescribeActivationsRequestPaginateTypeDef

```python
# DescribeActivationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeActivationsRequestPaginateTypeDef


def get_value() -> DescribeActivationsRequestPaginateTypeDef:
    return {
        "Filters": ...,
    }


# DescribeActivationsRequestPaginateTypeDef definition

class DescribeActivationsRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[DescribeActivationsFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DescribeActivationsFilterTypeDef](./type_defs.md#describeactivationsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAssociationExecutionTargetsRequestPaginateTypeDef

```python
# DescribeAssociationExecutionTargetsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeAssociationExecutionTargetsRequestPaginateTypeDef


def get_value() -> DescribeAssociationExecutionTargetsRequestPaginateTypeDef:
    return {
        "AssociationId": ...,
    }


# DescribeAssociationExecutionTargetsRequestPaginateTypeDef definition

class DescribeAssociationExecutionTargetsRequestPaginateTypeDef(TypedDict):
    AssociationId: str,
    ExecutionId: str,
    Filters: NotRequired[Sequence[AssociationExecutionTargetsFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: AssociationExecutionTargetsFilterTypeDef](./type_defs.md#associationexecutiontargetsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAssociationExecutionsRequestPaginateTypeDef

```python
# DescribeAssociationExecutionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeAssociationExecutionsRequestPaginateTypeDef


def get_value() -> DescribeAssociationExecutionsRequestPaginateTypeDef:
    return {
        "AssociationId": ...,
    }


# DescribeAssociationExecutionsRequestPaginateTypeDef definition

class DescribeAssociationExecutionsRequestPaginateTypeDef(TypedDict):
    AssociationId: str,
    Filters: NotRequired[Sequence[AssociationExecutionFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: AssociationExecutionFilterTypeDef](./type_defs.md#associationexecutionfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAutomationExecutionsRequestPaginateTypeDef

```python
# DescribeAutomationExecutionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeAutomationExecutionsRequestPaginateTypeDef


def get_value() -> DescribeAutomationExecutionsRequestPaginateTypeDef:
    return {
        "Filters": ...,
    }


# DescribeAutomationExecutionsRequestPaginateTypeDef definition

class DescribeAutomationExecutionsRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[AutomationExecutionFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: AutomationExecutionFilterTypeDef](./type_defs.md#automationexecutionfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEffectiveInstanceAssociationsRequestPaginateTypeDef

```python
# DescribeEffectiveInstanceAssociationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeEffectiveInstanceAssociationsRequestPaginateTypeDef


def get_value() -> DescribeEffectiveInstanceAssociationsRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeEffectiveInstanceAssociationsRequestPaginateTypeDef definition

class DescribeEffectiveInstanceAssociationsRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEffectivePatchesForPatchBaselineRequestPaginateTypeDef

```python
# DescribeEffectivePatchesForPatchBaselineRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeEffectivePatchesForPatchBaselineRequestPaginateTypeDef


def get_value() -> DescribeEffectivePatchesForPatchBaselineRequestPaginateTypeDef:
    return {
        "BaselineId": ...,
    }


# DescribeEffectivePatchesForPatchBaselineRequestPaginateTypeDef definition

class DescribeEffectivePatchesForPatchBaselineRequestPaginateTypeDef(TypedDict):
    BaselineId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeInstanceAssociationsStatusRequestPaginateTypeDef

```python
# DescribeInstanceAssociationsStatusRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeInstanceAssociationsStatusRequestPaginateTypeDef


def get_value() -> DescribeInstanceAssociationsStatusRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeInstanceAssociationsStatusRequestPaginateTypeDef definition

class DescribeInstanceAssociationsStatusRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeInstancePatchStatesRequestPaginateTypeDef

```python
# DescribeInstancePatchStatesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeInstancePatchStatesRequestPaginateTypeDef


def get_value() -> DescribeInstancePatchStatesRequestPaginateTypeDef:
    return {
        "InstanceIds": ...,
    }


# DescribeInstancePatchStatesRequestPaginateTypeDef definition

class DescribeInstancePatchStatesRequestPaginateTypeDef(TypedDict):
    InstanceIds: Sequence[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeInventoryDeletionsRequestPaginateTypeDef

```python
# DescribeInventoryDeletionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeInventoryDeletionsRequestPaginateTypeDef


def get_value() -> DescribeInventoryDeletionsRequestPaginateTypeDef:
    return {
        "DeletionId": ...,
    }


# DescribeInventoryDeletionsRequestPaginateTypeDef definition

class DescribeInventoryDeletionsRequestPaginateTypeDef(TypedDict):
    DeletionId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribePatchPropertiesRequestPaginateTypeDef

```python
# DescribePatchPropertiesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribePatchPropertiesRequestPaginateTypeDef


def get_value() -> DescribePatchPropertiesRequestPaginateTypeDef:
    return {
        "OperatingSystem": ...,
    }


# DescribePatchPropertiesRequestPaginateTypeDef definition

class DescribePatchPropertiesRequestPaginateTypeDef(TypedDict):
    OperatingSystem: OperatingSystemType,  # (1)
    Property: PatchPropertyType,  # (2)
    PatchSet: NotRequired[PatchSetType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
2. See [:material-code-brackets: PatchPropertyType](./literals.md#patchpropertytype) 
3. See [:material-code-brackets: PatchSetType](./literals.md#patchsettype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetInventorySchemaRequestPaginateTypeDef

```python
# GetInventorySchemaRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetInventorySchemaRequestPaginateTypeDef


def get_value() -> GetInventorySchemaRequestPaginateTypeDef:
    return {
        "TypeName": ...,
    }


# GetInventorySchemaRequestPaginateTypeDef definition

class GetInventorySchemaRequestPaginateTypeDef(TypedDict):
    TypeName: NotRequired[str],
    Aggregator: NotRequired[bool],
    SubType: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetParameterHistoryRequestPaginateTypeDef

```python
# GetParameterHistoryRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetParameterHistoryRequestPaginateTypeDef


def get_value() -> GetParameterHistoryRequestPaginateTypeDef:
    return {
        "Name": ...,
    }


# GetParameterHistoryRequestPaginateTypeDef definition

class GetParameterHistoryRequestPaginateTypeDef(TypedDict):
    Name: str,
    WithDecryption: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetResourcePoliciesRequestPaginateTypeDef

```python
# GetResourcePoliciesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetResourcePoliciesRequestPaginateTypeDef


def get_value() -> GetResourcePoliciesRequestPaginateTypeDef:
    return {
        "ResourceArn": ...,
    }


# GetResourcePoliciesRequestPaginateTypeDef definition

class GetResourcePoliciesRequestPaginateTypeDef(TypedDict):
    ResourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssociationVersionsRequestPaginateTypeDef

```python
# ListAssociationVersionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListAssociationVersionsRequestPaginateTypeDef


def get_value() -> ListAssociationVersionsRequestPaginateTypeDef:
    return {
        "AssociationId": ...,
    }


# ListAssociationVersionsRequestPaginateTypeDef definition

class ListAssociationVersionsRequestPaginateTypeDef(TypedDict):
    AssociationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssociationsRequestPaginateTypeDef

```python
# ListAssociationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListAssociationsRequestPaginateTypeDef


def get_value() -> ListAssociationsRequestPaginateTypeDef:
    return {
        "AssociationFilterList": ...,
    }


# ListAssociationsRequestPaginateTypeDef definition

class ListAssociationsRequestPaginateTypeDef(TypedDict):
    AssociationFilterList: NotRequired[Sequence[AssociationFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: AssociationFilterTypeDef](./type_defs.md#associationfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCommandInvocationsRequestPaginateTypeDef

```python
# ListCommandInvocationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListCommandInvocationsRequestPaginateTypeDef


def get_value() -> ListCommandInvocationsRequestPaginateTypeDef:
    return {
        "CommandId": ...,
    }


# ListCommandInvocationsRequestPaginateTypeDef definition

class ListCommandInvocationsRequestPaginateTypeDef(TypedDict):
    CommandId: NotRequired[str],
    InstanceId: NotRequired[str],
    Filters: NotRequired[Sequence[CommandFilterTypeDef]],  # (1)
    Details: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: CommandFilterTypeDef](./type_defs.md#commandfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCommandsRequestPaginateTypeDef

```python
# ListCommandsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListCommandsRequestPaginateTypeDef


def get_value() -> ListCommandsRequestPaginateTypeDef:
    return {
        "CommandId": ...,
    }


# ListCommandsRequestPaginateTypeDef definition

class ListCommandsRequestPaginateTypeDef(TypedDict):
    CommandId: NotRequired[str],
    InstanceId: NotRequired[str],
    Filters: NotRequired[Sequence[CommandFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: CommandFilterTypeDef](./type_defs.md#commandfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListComplianceItemsRequestPaginateTypeDef

```python
# ListComplianceItemsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListComplianceItemsRequestPaginateTypeDef


def get_value() -> ListComplianceItemsRequestPaginateTypeDef:
    return {
        "Filters": ...,
    }


# ListComplianceItemsRequestPaginateTypeDef definition

class ListComplianceItemsRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ComplianceStringFilterTypeDef]],  # (1)
    ResourceIds: NotRequired[Sequence[str]],
    ResourceTypes: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ComplianceStringFilterTypeDef](./type_defs.md#compliancestringfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListComplianceSummariesRequestPaginateTypeDef

```python
# ListComplianceSummariesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListComplianceSummariesRequestPaginateTypeDef


def get_value() -> ListComplianceSummariesRequestPaginateTypeDef:
    return {
        "Filters": ...,
    }


# ListComplianceSummariesRequestPaginateTypeDef definition

class ListComplianceSummariesRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ComplianceStringFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ComplianceStringFilterTypeDef](./type_defs.md#compliancestringfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDocumentVersionsRequestPaginateTypeDef

```python
# ListDocumentVersionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListDocumentVersionsRequestPaginateTypeDef


def get_value() -> ListDocumentVersionsRequestPaginateTypeDef:
    return {
        "Name": ...,
    }


# ListDocumentVersionsRequestPaginateTypeDef definition

class ListDocumentVersionsRequestPaginateTypeDef(TypedDict):
    Name: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceComplianceSummariesRequestPaginateTypeDef

```python
# ListResourceComplianceSummariesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListResourceComplianceSummariesRequestPaginateTypeDef


def get_value() -> ListResourceComplianceSummariesRequestPaginateTypeDef:
    return {
        "Filters": ...,
    }


# ListResourceComplianceSummariesRequestPaginateTypeDef definition

class ListResourceComplianceSummariesRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ComplianceStringFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ComplianceStringFilterTypeDef](./type_defs.md#compliancestringfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceDataSyncRequestPaginateTypeDef

```python
# ListResourceDataSyncRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListResourceDataSyncRequestPaginateTypeDef


def get_value() -> ListResourceDataSyncRequestPaginateTypeDef:
    return {
        "SyncType": ...,
    }


# ListResourceDataSyncRequestPaginateTypeDef definition

class ListResourceDataSyncRequestPaginateTypeDef(TypedDict):
    SyncType: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAutomationStepExecutionsRequestPaginateTypeDef

```python
# DescribeAutomationStepExecutionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeAutomationStepExecutionsRequestPaginateTypeDef


def get_value() -> DescribeAutomationStepExecutionsRequestPaginateTypeDef:
    return {
        "AutomationExecutionId": ...,
    }


# DescribeAutomationStepExecutionsRequestPaginateTypeDef definition

class DescribeAutomationStepExecutionsRequestPaginateTypeDef(TypedDict):
    AutomationExecutionId: str,
    Filters: NotRequired[Sequence[StepExecutionFilterTypeDef]],  # (1)
    ReverseOrder: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: StepExecutionFilterTypeDef](./type_defs.md#stepexecutionfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAutomationStepExecutionsRequestTypeDef

```python
# DescribeAutomationStepExecutionsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeAutomationStepExecutionsRequestTypeDef


def get_value() -> DescribeAutomationStepExecutionsRequestTypeDef:
    return {
        "AutomationExecutionId": ...,
    }


# DescribeAutomationStepExecutionsRequestTypeDef definition

class DescribeAutomationStepExecutionsRequestTypeDef(TypedDict):
    AutomationExecutionId: str,
    Filters: NotRequired[Sequence[StepExecutionFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ReverseOrder: NotRequired[bool],
```

1. See [:material-code-braces: StepExecutionFilterTypeDef](./type_defs.md#stepexecutionfiltertypedef) 
## DescribeAvailablePatchesRequestPaginateTypeDef

```python
# DescribeAvailablePatchesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeAvailablePatchesRequestPaginateTypeDef


def get_value() -> DescribeAvailablePatchesRequestPaginateTypeDef:
    return {
        "Filters": ...,
    }


# DescribeAvailablePatchesRequestPaginateTypeDef definition

class DescribeAvailablePatchesRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[PatchOrchestratorFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAvailablePatchesRequestTypeDef

```python
# DescribeAvailablePatchesRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeAvailablePatchesRequestTypeDef


def get_value() -> DescribeAvailablePatchesRequestTypeDef:
    return {
        "Filters": ...,
    }


# DescribeAvailablePatchesRequestTypeDef definition

class DescribeAvailablePatchesRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[PatchOrchestratorFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
## DescribeInstancePatchesRequestPaginateTypeDef

```python
# DescribeInstancePatchesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeInstancePatchesRequestPaginateTypeDef


def get_value() -> DescribeInstancePatchesRequestPaginateTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeInstancePatchesRequestPaginateTypeDef definition

class DescribeInstancePatchesRequestPaginateTypeDef(TypedDict):
    InstanceId: str,
    Filters: NotRequired[Sequence[PatchOrchestratorFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeInstancePatchesRequestTypeDef

```python
# DescribeInstancePatchesRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeInstancePatchesRequestTypeDef


def get_value() -> DescribeInstancePatchesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeInstancePatchesRequestTypeDef definition

class DescribeInstancePatchesRequestTypeDef(TypedDict):
    InstanceId: str,
    Filters: NotRequired[Sequence[PatchOrchestratorFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
## DescribePatchBaselinesRequestPaginateTypeDef

```python
# DescribePatchBaselinesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribePatchBaselinesRequestPaginateTypeDef


def get_value() -> DescribePatchBaselinesRequestPaginateTypeDef:
    return {
        "Filters": ...,
    }


# DescribePatchBaselinesRequestPaginateTypeDef definition

class DescribePatchBaselinesRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[PatchOrchestratorFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribePatchBaselinesRequestTypeDef

```python
# DescribePatchBaselinesRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribePatchBaselinesRequestTypeDef


def get_value() -> DescribePatchBaselinesRequestTypeDef:
    return {
        "Filters": ...,
    }


# DescribePatchBaselinesRequestTypeDef definition

class DescribePatchBaselinesRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[PatchOrchestratorFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
## DescribePatchGroupsRequestPaginateTypeDef

```python
# DescribePatchGroupsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribePatchGroupsRequestPaginateTypeDef


def get_value() -> DescribePatchGroupsRequestPaginateTypeDef:
    return {
        "Filters": ...,
    }


# DescribePatchGroupsRequestPaginateTypeDef definition

class DescribePatchGroupsRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[PatchOrchestratorFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribePatchGroupsRequestTypeDef

```python
# DescribePatchGroupsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribePatchGroupsRequestTypeDef


def get_value() -> DescribePatchGroupsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# DescribePatchGroupsRequestTypeDef definition

class DescribePatchGroupsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    Filters: NotRequired[Sequence[PatchOrchestratorFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
## DescribeAvailablePatchesResultTypeDef

```python
# DescribeAvailablePatchesResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeAvailablePatchesResultTypeDef


def get_value() -> DescribeAvailablePatchesResultTypeDef:
    return {
        "Patches": ...,
    }


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
# DescribeEffectiveInstanceAssociationsResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeEffectiveInstanceAssociationsResultTypeDef


def get_value() -> DescribeEffectiveInstanceAssociationsResultTypeDef:
    return {
        "Associations": ...,
    }


# DescribeEffectiveInstanceAssociationsResultTypeDef definition

class DescribeEffectiveInstanceAssociationsResultTypeDef(TypedDict):
    Associations: List[InstanceAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InstanceAssociationTypeDef](./type_defs.md#instanceassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInstanceInformationRequestPaginateTypeDef

```python
# DescribeInstanceInformationRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeInstanceInformationRequestPaginateTypeDef


def get_value() -> DescribeInstanceInformationRequestPaginateTypeDef:
    return {
        "InstanceInformationFilterList": ...,
    }


# DescribeInstanceInformationRequestPaginateTypeDef definition

class DescribeInstanceInformationRequestPaginateTypeDef(TypedDict):
    InstanceInformationFilterList: NotRequired[Sequence[InstanceInformationFilterTypeDef]],  # (1)
    Filters: NotRequired[Sequence[InstanceInformationStringFilterTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: InstanceInformationFilterTypeDef](./type_defs.md#instanceinformationfiltertypedef) 
2. See [:material-code-braces: InstanceInformationStringFilterTypeDef](./type_defs.md#instanceinformationstringfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeInstanceInformationRequestTypeDef

```python
# DescribeInstanceInformationRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeInstanceInformationRequestTypeDef


def get_value() -> DescribeInstanceInformationRequestTypeDef:
    return {
        "InstanceInformationFilterList": ...,
    }


# DescribeInstanceInformationRequestTypeDef definition

class DescribeInstanceInformationRequestTypeDef(TypedDict):
    InstanceInformationFilterList: NotRequired[Sequence[InstanceInformationFilterTypeDef]],  # (1)
    Filters: NotRequired[Sequence[InstanceInformationStringFilterTypeDef]],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InstanceInformationFilterTypeDef](./type_defs.md#instanceinformationfiltertypedef) 
2. See [:material-code-braces: InstanceInformationStringFilterTypeDef](./type_defs.md#instanceinformationstringfiltertypedef) 
## DescribeInstancePatchStatesForPatchGroupRequestPaginateTypeDef

```python
# DescribeInstancePatchStatesForPatchGroupRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeInstancePatchStatesForPatchGroupRequestPaginateTypeDef


def get_value() -> DescribeInstancePatchStatesForPatchGroupRequestPaginateTypeDef:
    return {
        "PatchGroup": ...,
    }


# DescribeInstancePatchStatesForPatchGroupRequestPaginateTypeDef definition

class DescribeInstancePatchStatesForPatchGroupRequestPaginateTypeDef(TypedDict):
    PatchGroup: str,
    Filters: NotRequired[Sequence[InstancePatchStateFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: InstancePatchStateFilterTypeDef](./type_defs.md#instancepatchstatefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeInstancePatchStatesForPatchGroupRequestTypeDef

```python
# DescribeInstancePatchStatesForPatchGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeInstancePatchStatesForPatchGroupRequestTypeDef


def get_value() -> DescribeInstancePatchStatesForPatchGroupRequestTypeDef:
    return {
        "PatchGroup": ...,
    }


# DescribeInstancePatchStatesForPatchGroupRequestTypeDef definition

class DescribeInstancePatchStatesForPatchGroupRequestTypeDef(TypedDict):
    PatchGroup: str,
    Filters: NotRequired[Sequence[InstancePatchStateFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: InstancePatchStateFilterTypeDef](./type_defs.md#instancepatchstatefiltertypedef) 
## DescribeInstancePatchStatesForPatchGroupResultTypeDef

```python
# DescribeInstancePatchStatesForPatchGroupResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeInstancePatchStatesForPatchGroupResultTypeDef


def get_value() -> DescribeInstancePatchStatesForPatchGroupResultTypeDef:
    return {
        "InstancePatchStates": ...,
    }


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
# DescribeInstancePatchStatesResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeInstancePatchStatesResultTypeDef


def get_value() -> DescribeInstancePatchStatesResultTypeDef:
    return {
        "InstancePatchStates": ...,
    }


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
# DescribeInstancePatchesResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeInstancePatchesResultTypeDef


def get_value() -> DescribeInstancePatchesResultTypeDef:
    return {
        "Patches": ...,
    }


# DescribeInstancePatchesResultTypeDef definition

class DescribeInstancePatchesResultTypeDef(TypedDict):
    Patches: List[PatchComplianceDataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PatchComplianceDataTypeDef](./type_defs.md#patchcompliancedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInstancePropertiesRequestPaginateTypeDef

```python
# DescribeInstancePropertiesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeInstancePropertiesRequestPaginateTypeDef


def get_value() -> DescribeInstancePropertiesRequestPaginateTypeDef:
    return {
        "InstancePropertyFilterList": ...,
    }


# DescribeInstancePropertiesRequestPaginateTypeDef definition

class DescribeInstancePropertiesRequestPaginateTypeDef(TypedDict):
    InstancePropertyFilterList: NotRequired[Sequence[InstancePropertyFilterTypeDef]],  # (1)
    FiltersWithOperator: NotRequired[Sequence[InstancePropertyStringFilterTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: InstancePropertyFilterTypeDef](./type_defs.md#instancepropertyfiltertypedef) 
2. See [:material-code-braces: InstancePropertyStringFilterTypeDef](./type_defs.md#instancepropertystringfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeInstancePropertiesRequestTypeDef

```python
# DescribeInstancePropertiesRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeInstancePropertiesRequestTypeDef


def get_value() -> DescribeInstancePropertiesRequestTypeDef:
    return {
        "InstancePropertyFilterList": ...,
    }


# DescribeInstancePropertiesRequestTypeDef definition

class DescribeInstancePropertiesRequestTypeDef(TypedDict):
    InstancePropertyFilterList: NotRequired[Sequence[InstancePropertyFilterTypeDef]],  # (1)
    FiltersWithOperator: NotRequired[Sequence[InstancePropertyStringFilterTypeDef]],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InstancePropertyFilterTypeDef](./type_defs.md#instancepropertyfiltertypedef) 
2. See [:material-code-braces: InstancePropertyStringFilterTypeDef](./type_defs.md#instancepropertystringfiltertypedef) 
## DescribeMaintenanceWindowExecutionTaskInvocationsRequestPaginateTypeDef

```python
# DescribeMaintenanceWindowExecutionTaskInvocationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowExecutionTaskInvocationsRequestPaginateTypeDef


def get_value() -> DescribeMaintenanceWindowExecutionTaskInvocationsRequestPaginateTypeDef:
    return {
        "WindowExecutionId": ...,
    }


# DescribeMaintenanceWindowExecutionTaskInvocationsRequestPaginateTypeDef definition

class DescribeMaintenanceWindowExecutionTaskInvocationsRequestPaginateTypeDef(TypedDict):
    WindowExecutionId: str,
    TaskId: str,
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeMaintenanceWindowExecutionTaskInvocationsRequestTypeDef

```python
# DescribeMaintenanceWindowExecutionTaskInvocationsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowExecutionTaskInvocationsRequestTypeDef


def get_value() -> DescribeMaintenanceWindowExecutionTaskInvocationsRequestTypeDef:
    return {
        "WindowExecutionId": ...,
    }


# DescribeMaintenanceWindowExecutionTaskInvocationsRequestTypeDef definition

class DescribeMaintenanceWindowExecutionTaskInvocationsRequestTypeDef(TypedDict):
    WindowExecutionId: str,
    TaskId: str,
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
## DescribeMaintenanceWindowExecutionTasksRequestPaginateTypeDef

```python
# DescribeMaintenanceWindowExecutionTasksRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowExecutionTasksRequestPaginateTypeDef


def get_value() -> DescribeMaintenanceWindowExecutionTasksRequestPaginateTypeDef:
    return {
        "WindowExecutionId": ...,
    }


# DescribeMaintenanceWindowExecutionTasksRequestPaginateTypeDef definition

class DescribeMaintenanceWindowExecutionTasksRequestPaginateTypeDef(TypedDict):
    WindowExecutionId: str,
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeMaintenanceWindowExecutionTasksRequestTypeDef

```python
# DescribeMaintenanceWindowExecutionTasksRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowExecutionTasksRequestTypeDef


def get_value() -> DescribeMaintenanceWindowExecutionTasksRequestTypeDef:
    return {
        "WindowExecutionId": ...,
    }


# DescribeMaintenanceWindowExecutionTasksRequestTypeDef definition

class DescribeMaintenanceWindowExecutionTasksRequestTypeDef(TypedDict):
    WindowExecutionId: str,
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
## DescribeMaintenanceWindowExecutionsRequestPaginateTypeDef

```python
# DescribeMaintenanceWindowExecutionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowExecutionsRequestPaginateTypeDef


def get_value() -> DescribeMaintenanceWindowExecutionsRequestPaginateTypeDef:
    return {
        "WindowId": ...,
    }


# DescribeMaintenanceWindowExecutionsRequestPaginateTypeDef definition

class DescribeMaintenanceWindowExecutionsRequestPaginateTypeDef(TypedDict):
    WindowId: str,
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeMaintenanceWindowExecutionsRequestTypeDef

```python
# DescribeMaintenanceWindowExecutionsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowExecutionsRequestTypeDef


def get_value() -> DescribeMaintenanceWindowExecutionsRequestTypeDef:
    return {
        "WindowId": ...,
    }


# DescribeMaintenanceWindowExecutionsRequestTypeDef definition

class DescribeMaintenanceWindowExecutionsRequestTypeDef(TypedDict):
    WindowId: str,
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
## DescribeMaintenanceWindowTargetsRequestPaginateTypeDef

```python
# DescribeMaintenanceWindowTargetsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowTargetsRequestPaginateTypeDef


def get_value() -> DescribeMaintenanceWindowTargetsRequestPaginateTypeDef:
    return {
        "WindowId": ...,
    }


# DescribeMaintenanceWindowTargetsRequestPaginateTypeDef definition

class DescribeMaintenanceWindowTargetsRequestPaginateTypeDef(TypedDict):
    WindowId: str,
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeMaintenanceWindowTargetsRequestTypeDef

```python
# DescribeMaintenanceWindowTargetsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowTargetsRequestTypeDef


def get_value() -> DescribeMaintenanceWindowTargetsRequestTypeDef:
    return {
        "WindowId": ...,
    }


# DescribeMaintenanceWindowTargetsRequestTypeDef definition

class DescribeMaintenanceWindowTargetsRequestTypeDef(TypedDict):
    WindowId: str,
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
## DescribeMaintenanceWindowTasksRequestPaginateTypeDef

```python
# DescribeMaintenanceWindowTasksRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowTasksRequestPaginateTypeDef


def get_value() -> DescribeMaintenanceWindowTasksRequestPaginateTypeDef:
    return {
        "WindowId": ...,
    }


# DescribeMaintenanceWindowTasksRequestPaginateTypeDef definition

class DescribeMaintenanceWindowTasksRequestPaginateTypeDef(TypedDict):
    WindowId: str,
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeMaintenanceWindowTasksRequestTypeDef

```python
# DescribeMaintenanceWindowTasksRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowTasksRequestTypeDef


def get_value() -> DescribeMaintenanceWindowTasksRequestTypeDef:
    return {
        "WindowId": ...,
    }


# DescribeMaintenanceWindowTasksRequestTypeDef definition

class DescribeMaintenanceWindowTasksRequestTypeDef(TypedDict):
    WindowId: str,
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
## DescribeMaintenanceWindowsRequestPaginateTypeDef

```python
# DescribeMaintenanceWindowsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowsRequestPaginateTypeDef


def get_value() -> DescribeMaintenanceWindowsRequestPaginateTypeDef:
    return {
        "Filters": ...,
    }


# DescribeMaintenanceWindowsRequestPaginateTypeDef definition

class DescribeMaintenanceWindowsRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeMaintenanceWindowsRequestTypeDef

```python
# DescribeMaintenanceWindowsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowsRequestTypeDef


def get_value() -> DescribeMaintenanceWindowsRequestTypeDef:
    return {
        "Filters": ...,
    }


# DescribeMaintenanceWindowsRequestTypeDef definition

class DescribeMaintenanceWindowsRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
## DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef

```python
# DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef


def get_value() -> DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef:
    return {
        "WindowExecutionTaskInvocationIdentities": ...,
    }


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
# DescribeMaintenanceWindowExecutionsResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowExecutionsResultTypeDef


def get_value() -> DescribeMaintenanceWindowExecutionsResultTypeDef:
    return {
        "WindowExecutions": ...,
    }


# DescribeMaintenanceWindowExecutionsResultTypeDef definition

class DescribeMaintenanceWindowExecutionsResultTypeDef(TypedDict):
    WindowExecutions: List[MaintenanceWindowExecutionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MaintenanceWindowExecutionTypeDef](./type_defs.md#maintenancewindowexecutiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMaintenanceWindowScheduleResultTypeDef

```python
# DescribeMaintenanceWindowScheduleResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowScheduleResultTypeDef


def get_value() -> DescribeMaintenanceWindowScheduleResultTypeDef:
    return {
        "ScheduledWindowExecutions": ...,
    }


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
# DescribeMaintenanceWindowsForTargetResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowsForTargetResultTypeDef


def get_value() -> DescribeMaintenanceWindowsForTargetResultTypeDef:
    return {
        "WindowIdentities": ...,
    }


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
# DescribeMaintenanceWindowsResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowsResultTypeDef


def get_value() -> DescribeMaintenanceWindowsResultTypeDef:
    return {
        "WindowIdentities": ...,
    }


# DescribeMaintenanceWindowsResultTypeDef definition

class DescribeMaintenanceWindowsResultTypeDef(TypedDict):
    WindowIdentities: List[MaintenanceWindowIdentityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MaintenanceWindowIdentityTypeDef](./type_defs.md#maintenancewindowidentitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOpsItemsRequestPaginateTypeDef

```python
# DescribeOpsItemsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeOpsItemsRequestPaginateTypeDef


def get_value() -> DescribeOpsItemsRequestPaginateTypeDef:
    return {
        "OpsItemFilters": ...,
    }


# DescribeOpsItemsRequestPaginateTypeDef definition

class DescribeOpsItemsRequestPaginateTypeDef(TypedDict):
    OpsItemFilters: NotRequired[Sequence[OpsItemFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: OpsItemFilterTypeDef](./type_defs.md#opsitemfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeOpsItemsRequestTypeDef

```python
# DescribeOpsItemsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeOpsItemsRequestTypeDef


def get_value() -> DescribeOpsItemsRequestTypeDef:
    return {
        "OpsItemFilters": ...,
    }


# DescribeOpsItemsRequestTypeDef definition

class DescribeOpsItemsRequestTypeDef(TypedDict):
    OpsItemFilters: NotRequired[Sequence[OpsItemFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OpsItemFilterTypeDef](./type_defs.md#opsitemfiltertypedef) 
## GetParametersByPathRequestPaginateTypeDef

```python
# GetParametersByPathRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetParametersByPathRequestPaginateTypeDef


def get_value() -> GetParametersByPathRequestPaginateTypeDef:
    return {
        "Path": ...,
    }


# GetParametersByPathRequestPaginateTypeDef definition

class GetParametersByPathRequestPaginateTypeDef(TypedDict):
    Path: str,
    Recursive: NotRequired[bool],
    ParameterFilters: NotRequired[Sequence[ParameterStringFilterTypeDef]],  # (1)
    WithDecryption: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ParameterStringFilterTypeDef](./type_defs.md#parameterstringfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetParametersByPathRequestTypeDef

```python
# GetParametersByPathRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetParametersByPathRequestTypeDef


def get_value() -> GetParametersByPathRequestTypeDef:
    return {
        "Path": ...,
    }


# GetParametersByPathRequestTypeDef definition

class GetParametersByPathRequestTypeDef(TypedDict):
    Path: str,
    Recursive: NotRequired[bool],
    ParameterFilters: NotRequired[Sequence[ParameterStringFilterTypeDef]],  # (1)
    WithDecryption: NotRequired[bool],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ParameterStringFilterTypeDef](./type_defs.md#parameterstringfiltertypedef) 
## DescribeParametersRequestPaginateTypeDef

```python
# DescribeParametersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeParametersRequestPaginateTypeDef


def get_value() -> DescribeParametersRequestPaginateTypeDef:
    return {
        "Filters": ...,
    }


# DescribeParametersRequestPaginateTypeDef definition

class DescribeParametersRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ParametersFilterTypeDef]],  # (1)
    ParameterFilters: NotRequired[Sequence[ParameterStringFilterTypeDef]],  # (2)
    Shared: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: ParametersFilterTypeDef](./type_defs.md#parametersfiltertypedef) 
2. See [:material-code-braces: ParameterStringFilterTypeDef](./type_defs.md#parameterstringfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeParametersRequestTypeDef

```python
# DescribeParametersRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeParametersRequestTypeDef


def get_value() -> DescribeParametersRequestTypeDef:
    return {
        "Filters": ...,
    }


# DescribeParametersRequestTypeDef definition

class DescribeParametersRequestTypeDef(TypedDict):
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
# DescribePatchBaselinesResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribePatchBaselinesResultTypeDef


def get_value() -> DescribePatchBaselinesResultTypeDef:
    return {
        "BaselineIdentities": ...,
    }


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
# PatchGroupPatchBaselineMappingTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PatchGroupPatchBaselineMappingTypeDef


def get_value() -> PatchGroupPatchBaselineMappingTypeDef:
    return {
        "PatchGroup": ...,
    }


# PatchGroupPatchBaselineMappingTypeDef definition

class PatchGroupPatchBaselineMappingTypeDef(TypedDict):
    PatchGroup: NotRequired[str],
    BaselineIdentity: NotRequired[PatchBaselineIdentityTypeDef],  # (1)
```

1. See [:material-code-braces: PatchBaselineIdentityTypeDef](./type_defs.md#patchbaselineidentitytypedef) 
## DescribeSessionsRequestPaginateTypeDef

```python
# DescribeSessionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeSessionsRequestPaginateTypeDef


def get_value() -> DescribeSessionsRequestPaginateTypeDef:
    return {
        "State": ...,
    }


# DescribeSessionsRequestPaginateTypeDef definition

class DescribeSessionsRequestPaginateTypeDef(TypedDict):
    State: SessionStateType,  # (1)
    Filters: NotRequired[Sequence[SessionFilterTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SessionStateType](./literals.md#sessionstatetype) 
2. See [:material-code-braces: SessionFilterTypeDef](./type_defs.md#sessionfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSessionsRequestTypeDef

```python
# DescribeSessionsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeSessionsRequestTypeDef


def get_value() -> DescribeSessionsRequestTypeDef:
    return {
        "State": ...,
    }


# DescribeSessionsRequestTypeDef definition

class DescribeSessionsRequestTypeDef(TypedDict):
    State: SessionStateType,  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[SessionFilterTypeDef]],  # (2)
```

1. See [:material-code-brackets: SessionStateType](./literals.md#sessionstatetype) 
2. See [:material-code-braces: SessionFilterTypeDef](./type_defs.md#sessionfiltertypedef) 
## UpdateDocumentDefaultVersionResultTypeDef

```python
# UpdateDocumentDefaultVersionResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdateDocumentDefaultVersionResultTypeDef


def get_value() -> UpdateDocumentDefaultVersionResultTypeDef:
    return {
        "Description": ...,
    }


# UpdateDocumentDefaultVersionResultTypeDef definition

class UpdateDocumentDefaultVersionResultTypeDef(TypedDict):
    Description: DocumentDefaultVersionDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DocumentDefaultVersionDescriptionTypeDef](./type_defs.md#documentdefaultversiondescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DocumentDescriptionTypeDef

```python
# DocumentDescriptionTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DocumentDescriptionTypeDef


def get_value() -> DocumentDescriptionTypeDef:
    return {
        "Sha1": ...,
    }


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
## ListDocumentsRequestPaginateTypeDef

```python
# ListDocumentsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListDocumentsRequestPaginateTypeDef


def get_value() -> ListDocumentsRequestPaginateTypeDef:
    return {
        "DocumentFilterList": ...,
    }


# ListDocumentsRequestPaginateTypeDef definition

class ListDocumentsRequestPaginateTypeDef(TypedDict):
    DocumentFilterList: NotRequired[Sequence[DocumentFilterTypeDef]],  # (1)
    Filters: NotRequired[Sequence[DocumentKeyValuesFilterTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: DocumentFilterTypeDef](./type_defs.md#documentfiltertypedef) 
2. See [:material-code-braces: DocumentKeyValuesFilterTypeDef](./type_defs.md#documentkeyvaluesfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDocumentsRequestTypeDef

```python
# ListDocumentsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListDocumentsRequestTypeDef


def get_value() -> ListDocumentsRequestTypeDef:
    return {
        "DocumentFilterList": ...,
    }


# ListDocumentsRequestTypeDef definition

class ListDocumentsRequestTypeDef(TypedDict):
    DocumentFilterList: NotRequired[Sequence[DocumentFilterTypeDef]],  # (1)
    Filters: NotRequired[Sequence[DocumentKeyValuesFilterTypeDef]],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DocumentFilterTypeDef](./type_defs.md#documentfiltertypedef) 
2. See [:material-code-braces: DocumentKeyValuesFilterTypeDef](./type_defs.md#documentkeyvaluesfiltertypedef) 
## DocumentReviewerResponseSourceTypeDef

```python
# DocumentReviewerResponseSourceTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DocumentReviewerResponseSourceTypeDef


def get_value() -> DocumentReviewerResponseSourceTypeDef:
    return {
        "CreateTime": ...,
    }


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
# DocumentReviewsTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DocumentReviewsTypeDef


def get_value() -> DocumentReviewsTypeDef:
    return {
        "Action": ...,
    }


# DocumentReviewsTypeDef definition

class DocumentReviewsTypeDef(TypedDict):
    Action: DocumentReviewActionType,  # (1)
    Comment: NotRequired[Sequence[DocumentReviewCommentSourceTypeDef]],  # (2)
```

1. See [:material-code-brackets: DocumentReviewActionType](./literals.md#documentreviewactiontype) 
2. See [:material-code-braces: DocumentReviewCommentSourceTypeDef](./type_defs.md#documentreviewcommentsourcetypedef) 
## ListDocumentVersionsResultTypeDef

```python
# ListDocumentVersionsResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListDocumentVersionsResultTypeDef


def get_value() -> ListDocumentVersionsResultTypeDef:
    return {
        "DocumentVersions": ...,
    }


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
# EffectivePatchTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import EffectivePatchTypeDef


def get_value() -> EffectivePatchTypeDef:
    return {
        "Patch": ...,
    }


# EffectivePatchTypeDef definition

class EffectivePatchTypeDef(TypedDict):
    Patch: NotRequired[PatchTypeDef],  # (1)
    PatchStatus: NotRequired[PatchStatusTypeDef],  # (2)
```

1. See [:material-code-braces: PatchTypeDef](./type_defs.md#patchtypedef) 
2. See [:material-code-braces: PatchStatusTypeDef](./type_defs.md#patchstatustypedef) 
## GetCommandInvocationRequestWaitTypeDef

```python
# GetCommandInvocationRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetCommandInvocationRequestWaitTypeDef


def get_value() -> GetCommandInvocationRequestWaitTypeDef:
    return {
        "CommandId": ...,
    }


# GetCommandInvocationRequestWaitTypeDef definition

class GetCommandInvocationRequestWaitTypeDef(TypedDict):
    CommandId: str,
    InstanceId: str,
    PluginName: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## InventoryGroupTypeDef

```python
# InventoryGroupTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InventoryGroupTypeDef


def get_value() -> InventoryGroupTypeDef:
    return {
        "Name": ...,
    }


# InventoryGroupTypeDef definition

class InventoryGroupTypeDef(TypedDict):
    Name: str,
    Filters: Sequence[InventoryFilterTypeDef],  # (1)
```

1. See [:material-code-braces: InventoryFilterTypeDef](./type_defs.md#inventoryfiltertypedef) 
## ListInventoryEntriesRequestTypeDef

```python
# ListInventoryEntriesRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListInventoryEntriesRequestTypeDef


def get_value() -> ListInventoryEntriesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# ListInventoryEntriesRequestTypeDef definition

class ListInventoryEntriesRequestTypeDef(TypedDict):
    InstanceId: str,
    TypeName: str,
    Filters: NotRequired[Sequence[InventoryFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: InventoryFilterTypeDef](./type_defs.md#inventoryfiltertypedef) 
## OpsAggregatorPaginatorTypeDef

```python
# OpsAggregatorPaginatorTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import OpsAggregatorPaginatorTypeDef


def get_value() -> OpsAggregatorPaginatorTypeDef:
    return {
        "AggregatorType": ...,
    }


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
# OpsAggregatorTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import OpsAggregatorTypeDef


def get_value() -> OpsAggregatorTypeDef:
    return {
        "AggregatorType": ...,
    }


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
# GetParameterResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetParameterResultTypeDef


def get_value() -> GetParameterResultTypeDef:
    return {
        "Parameter": ...,
    }


# GetParameterResultTypeDef definition

class GetParameterResultTypeDef(TypedDict):
    Parameter: ParameterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetParametersByPathResultTypeDef

```python
# GetParametersByPathResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetParametersByPathResultTypeDef


def get_value() -> GetParametersByPathResultTypeDef:
    return {
        "Parameters": ...,
    }


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
# GetParametersResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetParametersResultTypeDef


def get_value() -> GetParametersResultTypeDef:
    return {
        "Parameters": ...,
    }


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
# GetResourcePoliciesResponseTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetResourcePoliciesResponseTypeDef


def get_value() -> GetResourcePoliciesResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# GetServiceSettingResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetServiceSettingResultTypeDef


def get_value() -> GetServiceSettingResultTypeDef:
    return {
        "ServiceSetting": ...,
    }


# GetServiceSettingResultTypeDef definition

class GetServiceSettingResultTypeDef(TypedDict):
    ServiceSetting: ServiceSettingTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceSettingTypeDef](./type_defs.md#servicesettingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResetServiceSettingResultTypeDef

```python
# ResetServiceSettingResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ResetServiceSettingResultTypeDef


def get_value() -> ResetServiceSettingResultTypeDef:
    return {
        "ServiceSetting": ...,
    }


# ResetServiceSettingResultTypeDef definition

class ResetServiceSettingResultTypeDef(TypedDict):
    ServiceSetting: ServiceSettingTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceSettingTypeDef](./type_defs.md#servicesettingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstanceInformationTypeDef

```python
# InstanceInformationTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InstanceInformationTypeDef


def get_value() -> InstanceInformationTypeDef:
    return {
        "InstanceId": ...,
    }


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
# InstancePropertyTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InstancePropertyTypeDef


def get_value() -> InstancePropertyTypeDef:
    return {
        "Name": ...,
    }


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
# InstanceAssociationOutputLocationTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InstanceAssociationOutputLocationTypeDef


def get_value() -> InstanceAssociationOutputLocationTypeDef:
    return {
        "S3Location": ...,
    }


# InstanceAssociationOutputLocationTypeDef definition

class InstanceAssociationOutputLocationTypeDef(TypedDict):
    S3Location: NotRequired[S3OutputLocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3OutputLocationTypeDef](./type_defs.md#s3outputlocationtypedef) 
## InstanceAssociationOutputUrlTypeDef

```python
# InstanceAssociationOutputUrlTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InstanceAssociationOutputUrlTypeDef


def get_value() -> InstanceAssociationOutputUrlTypeDef:
    return {
        "S3OutputUrl": ...,
    }


# InstanceAssociationOutputUrlTypeDef definition

class InstanceAssociationOutputUrlTypeDef(TypedDict):
    S3OutputUrl: NotRequired[S3OutputUrlTypeDef],  # (1)
```

1. See [:material-code-braces: S3OutputUrlTypeDef](./type_defs.md#s3outputurltypedef) 
## NodeTypeTypeDef

```python
# NodeTypeTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import NodeTypeTypeDef


def get_value() -> NodeTypeTypeDef:
    return {
        "Instance": ...,
    }


# NodeTypeTypeDef definition

class NodeTypeTypeDef(TypedDict):
    Instance: NotRequired[InstanceInfoTypeDef],  # (1)
```

1. See [:material-code-braces: InstanceInfoTypeDef](./type_defs.md#instanceinfotypedef) 
## InventoryDeletionSummaryTypeDef

```python
# InventoryDeletionSummaryTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InventoryDeletionSummaryTypeDef


def get_value() -> InventoryDeletionSummaryTypeDef:
    return {
        "TotalCount": ...,
    }


# InventoryDeletionSummaryTypeDef definition

class InventoryDeletionSummaryTypeDef(TypedDict):
    TotalCount: NotRequired[int],
    RemainingCount: NotRequired[int],
    SummaryItems: NotRequired[List[InventoryDeletionSummaryItemTypeDef]],  # (1)
```

1. See [:material-code-braces: InventoryDeletionSummaryItemTypeDef](./type_defs.md#inventorydeletionsummaryitemtypedef) 
## InventoryItemSchemaTypeDef

```python
# InventoryItemSchemaTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InventoryItemSchemaTypeDef


def get_value() -> InventoryItemSchemaTypeDef:
    return {
        "TypeName": ...,
    }


# InventoryItemSchemaTypeDef definition

class InventoryItemSchemaTypeDef(TypedDict):
    TypeName: str,
    Attributes: List[InventoryItemAttributeTypeDef],  # (1)
    Version: NotRequired[str],
    DisplayName: NotRequired[str],
```

1. See [:material-code-braces: InventoryItemAttributeTypeDef](./type_defs.md#inventoryitemattributetypedef) 
## PutInventoryRequestTypeDef

```python
# PutInventoryRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PutInventoryRequestTypeDef


def get_value() -> PutInventoryRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# PutInventoryRequestTypeDef definition

class PutInventoryRequestTypeDef(TypedDict):
    InstanceId: str,
    Items: Sequence[InventoryItemTypeDef],  # (1)
```

1. See [:material-code-braces: InventoryItemTypeDef](./type_defs.md#inventoryitemtypedef) 
## InventoryResultEntityTypeDef

```python
# InventoryResultEntityTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InventoryResultEntityTypeDef


def get_value() -> InventoryResultEntityTypeDef:
    return {
        "Id": ...,
    }


# InventoryResultEntityTypeDef definition

class InventoryResultEntityTypeDef(TypedDict):
    Id: NotRequired[str],
    Data: NotRequired[Dict[str, InventoryResultItemTypeDef]],  # (1)
```

1. See [:material-code-braces: InventoryResultItemTypeDef](./type_defs.md#inventoryresultitemtypedef) 
## ListNodesRequestPaginateTypeDef

```python
# ListNodesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListNodesRequestPaginateTypeDef


def get_value() -> ListNodesRequestPaginateTypeDef:
    return {
        "SyncName": ...,
    }


# ListNodesRequestPaginateTypeDef definition

class ListNodesRequestPaginateTypeDef(TypedDict):
    SyncName: NotRequired[str],
    Filters: NotRequired[Sequence[NodeFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: NodeFilterTypeDef](./type_defs.md#nodefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNodesRequestTypeDef

```python
# ListNodesRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListNodesRequestTypeDef


def get_value() -> ListNodesRequestTypeDef:
    return {
        "SyncName": ...,
    }


# ListNodesRequestTypeDef definition

class ListNodesRequestTypeDef(TypedDict):
    SyncName: NotRequired[str],
    Filters: NotRequired[Sequence[NodeFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: NodeFilterTypeDef](./type_defs.md#nodefiltertypedef) 
## ListNodesSummaryRequestPaginateTypeDef

```python
# ListNodesSummaryRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListNodesSummaryRequestPaginateTypeDef


def get_value() -> ListNodesSummaryRequestPaginateTypeDef:
    return {
        "Aggregators": ...,
    }


# ListNodesSummaryRequestPaginateTypeDef definition

class ListNodesSummaryRequestPaginateTypeDef(TypedDict):
    Aggregators: Sequence[NodeAggregatorPaginatorTypeDef],  # (1)
    SyncName: NotRequired[str],
    Filters: NotRequired[Sequence[NodeFilterTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: NodeAggregatorPaginatorTypeDef](./type_defs.md#nodeaggregatorpaginatortypedef) 
2. See [:material-code-braces: NodeFilterTypeDef](./type_defs.md#nodefiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNodesSummaryRequestTypeDef

```python
# ListNodesSummaryRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListNodesSummaryRequestTypeDef


def get_value() -> ListNodesSummaryRequestTypeDef:
    return {
        "Aggregators": ...,
    }


# ListNodesSummaryRequestTypeDef definition

class ListNodesSummaryRequestTypeDef(TypedDict):
    Aggregators: Sequence[NodeAggregatorTypeDef],  # (1)
    SyncName: NotRequired[str],
    Filters: NotRequired[Sequence[NodeFilterTypeDef]],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: NodeAggregatorTypeDef](./type_defs.md#nodeaggregatortypedef) 
2. See [:material-code-braces: NodeFilterTypeDef](./type_defs.md#nodefiltertypedef) 
## ListOpsItemEventsRequestPaginateTypeDef

```python
# ListOpsItemEventsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListOpsItemEventsRequestPaginateTypeDef


def get_value() -> ListOpsItemEventsRequestPaginateTypeDef:
    return {
        "Filters": ...,
    }


# ListOpsItemEventsRequestPaginateTypeDef definition

class ListOpsItemEventsRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[OpsItemEventFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: OpsItemEventFilterTypeDef](./type_defs.md#opsitemeventfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOpsItemEventsRequestTypeDef

```python
# ListOpsItemEventsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListOpsItemEventsRequestTypeDef


def get_value() -> ListOpsItemEventsRequestTypeDef:
    return {
        "Filters": ...,
    }


# ListOpsItemEventsRequestTypeDef definition

class ListOpsItemEventsRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[OpsItemEventFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OpsItemEventFilterTypeDef](./type_defs.md#opsitemeventfiltertypedef) 
## ListOpsItemRelatedItemsRequestPaginateTypeDef

```python
# ListOpsItemRelatedItemsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListOpsItemRelatedItemsRequestPaginateTypeDef


def get_value() -> ListOpsItemRelatedItemsRequestPaginateTypeDef:
    return {
        "OpsItemId": ...,
    }


# ListOpsItemRelatedItemsRequestPaginateTypeDef definition

class ListOpsItemRelatedItemsRequestPaginateTypeDef(TypedDict):
    OpsItemId: NotRequired[str],
    Filters: NotRequired[Sequence[OpsItemRelatedItemsFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: OpsItemRelatedItemsFilterTypeDef](./type_defs.md#opsitemrelateditemsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOpsItemRelatedItemsRequestTypeDef

```python
# ListOpsItemRelatedItemsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListOpsItemRelatedItemsRequestTypeDef


def get_value() -> ListOpsItemRelatedItemsRequestTypeDef:
    return {
        "OpsItemId": ...,
    }


# ListOpsItemRelatedItemsRequestTypeDef definition

class ListOpsItemRelatedItemsRequestTypeDef(TypedDict):
    OpsItemId: NotRequired[str],
    Filters: NotRequired[Sequence[OpsItemRelatedItemsFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OpsItemRelatedItemsFilterTypeDef](./type_defs.md#opsitemrelateditemsfiltertypedef) 
## ListOpsMetadataRequestPaginateTypeDef

```python
# ListOpsMetadataRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListOpsMetadataRequestPaginateTypeDef


def get_value() -> ListOpsMetadataRequestPaginateTypeDef:
    return {
        "Filters": ...,
    }


# ListOpsMetadataRequestPaginateTypeDef definition

class ListOpsMetadataRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[OpsMetadataFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: OpsMetadataFilterTypeDef](./type_defs.md#opsmetadatafiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOpsMetadataRequestTypeDef

```python
# ListOpsMetadataRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListOpsMetadataRequestTypeDef


def get_value() -> ListOpsMetadataRequestTypeDef:
    return {
        "Filters": ...,
    }


# ListOpsMetadataRequestTypeDef definition

class ListOpsMetadataRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[OpsMetadataFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OpsMetadataFilterTypeDef](./type_defs.md#opsmetadatafiltertypedef) 
## ListOpsMetadataResultTypeDef

```python
# ListOpsMetadataResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListOpsMetadataResultTypeDef


def get_value() -> ListOpsMetadataResultTypeDef:
    return {
        "OpsMetadataList": ...,
    }


# ListOpsMetadataResultTypeDef definition

class ListOpsMetadataResultTypeDef(TypedDict):
    OpsMetadataList: List[OpsMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OpsMetadataTypeDef](./type_defs.md#opsmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MaintenanceWindowRunCommandParametersTypeDef

```python
# MaintenanceWindowRunCommandParametersTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import MaintenanceWindowRunCommandParametersTypeDef


def get_value() -> MaintenanceWindowRunCommandParametersTypeDef:
    return {
        "Comment": ...,
    }


# MaintenanceWindowRunCommandParametersTypeDef definition

class MaintenanceWindowRunCommandParametersTypeDef(TypedDict):
    Comment: NotRequired[str],
    CloudWatchOutputConfig: NotRequired[CloudWatchOutputConfigTypeDef],  # (1)
    DocumentHash: NotRequired[str],
    DocumentHashType: NotRequired[DocumentHashTypeType],  # (2)
    DocumentVersion: NotRequired[str],
    NotificationConfig: NotRequired[NotificationConfigTypeDef],  # (3)
    OutputS3BucketName: NotRequired[str],
    OutputS3KeyPrefix: NotRequired[str],
    Parameters: NotRequired[Mapping[str, Sequence[str]]],
    ServiceRoleArn: NotRequired[str],
    TimeoutSeconds: NotRequired[int],
```

1. See [:material-code-braces: CloudWatchOutputConfigTypeDef](./type_defs.md#cloudwatchoutputconfigtypedef) 
2. See [:material-code-brackets: DocumentHashTypeType](./literals.md#documenthashtypetype) 
3. See [:material-code-braces: NotificationConfigTypeDef](./type_defs.md#notificationconfigtypedef) 
## OpsEntityTypeDef

```python
# OpsEntityTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import OpsEntityTypeDef


def get_value() -> OpsEntityTypeDef:
    return {
        "Id": ...,
    }


# OpsEntityTypeDef definition

class OpsEntityTypeDef(TypedDict):
    Id: NotRequired[str],
    Data: NotRequired[Dict[str, OpsEntityItemTypeDef]],  # (1)
```

1. See [:material-code-braces: OpsEntityItemTypeDef](./type_defs.md#opsentityitemtypedef) 
## OpsItemEventSummaryTypeDef

```python
# OpsItemEventSummaryTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import OpsItemEventSummaryTypeDef


def get_value() -> OpsItemEventSummaryTypeDef:
    return {
        "OpsItemId": ...,
    }


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
# OpsItemRelatedItemSummaryTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import OpsItemRelatedItemSummaryTypeDef


def get_value() -> OpsItemRelatedItemSummaryTypeDef:
    return {
        "OpsItemId": ...,
    }


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
# ParameterHistoryTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ParameterHistoryTypeDef


def get_value() -> ParameterHistoryTypeDef:
    return {
        "Name": ...,
    }


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
# ParameterMetadataTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ParameterMetadataTypeDef


def get_value() -> ParameterMetadataTypeDef:
    return {
        "Name": ...,
    }


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
# PatchFilterGroupOutputTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PatchFilterGroupOutputTypeDef


def get_value() -> PatchFilterGroupOutputTypeDef:
    return {
        "PatchFilters": ...,
    }


# PatchFilterGroupOutputTypeDef definition

class PatchFilterGroupOutputTypeDef(TypedDict):
    PatchFilters: List[PatchFilterOutputTypeDef],  # (1)
```

1. See [:material-code-braces: PatchFilterOutputTypeDef](./type_defs.md#patchfilteroutputtypedef) 
## ResourceDataSyncAwsOrganizationsSourceOutputTypeDef

```python
# ResourceDataSyncAwsOrganizationsSourceOutputTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ResourceDataSyncAwsOrganizationsSourceOutputTypeDef


def get_value() -> ResourceDataSyncAwsOrganizationsSourceOutputTypeDef:
    return {
        "OrganizationSourceType": ...,
    }


# ResourceDataSyncAwsOrganizationsSourceOutputTypeDef definition

class ResourceDataSyncAwsOrganizationsSourceOutputTypeDef(TypedDict):
    OrganizationSourceType: str,
    OrganizationalUnits: NotRequired[List[ResourceDataSyncOrganizationalUnitTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourceDataSyncOrganizationalUnitTypeDef](./type_defs.md#resourcedatasyncorganizationalunittypedef) 
## ResourceDataSyncAwsOrganizationsSourceTypeDef

```python
# ResourceDataSyncAwsOrganizationsSourceTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ResourceDataSyncAwsOrganizationsSourceTypeDef


def get_value() -> ResourceDataSyncAwsOrganizationsSourceTypeDef:
    return {
        "OrganizationSourceType": ...,
    }


# ResourceDataSyncAwsOrganizationsSourceTypeDef definition

class ResourceDataSyncAwsOrganizationsSourceTypeDef(TypedDict):
    OrganizationSourceType: str,
    OrganizationalUnits: NotRequired[Sequence[ResourceDataSyncOrganizationalUnitTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourceDataSyncOrganizationalUnitTypeDef](./type_defs.md#resourcedatasyncorganizationalunittypedef) 
## ResourceDataSyncS3DestinationTypeDef

```python
# ResourceDataSyncS3DestinationTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ResourceDataSyncS3DestinationTypeDef


def get_value() -> ResourceDataSyncS3DestinationTypeDef:
    return {
        "BucketName": ...,
    }


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
# SessionTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import SessionTypeDef


def get_value() -> SessionTypeDef:
    return {
        "SessionId": ...,
    }


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
# DescribeActivationsResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeActivationsResultTypeDef


def get_value() -> DescribeActivationsResultTypeDef:
    return {
        "ActivationList": ...,
    }


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
# AssociationExecutionTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AssociationExecutionTypeDef


def get_value() -> AssociationExecutionTypeDef:
    return {
        "AssociationId": ...,
    }


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
# CommandTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CommandTypeDef


def get_value() -> CommandTypeDef:
    return {
        "CommandId": ...,
    }


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
# GetMaintenanceWindowExecutionTaskResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetMaintenanceWindowExecutionTaskResultTypeDef


def get_value() -> GetMaintenanceWindowExecutionTaskResultTypeDef:
    return {
        "WindowExecutionId": ...,
    }


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
# MaintenanceWindowExecutionTaskIdentityTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import MaintenanceWindowExecutionTaskIdentityTypeDef


def get_value() -> MaintenanceWindowExecutionTaskIdentityTypeDef:
    return {
        "WindowExecutionId": ...,
    }


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
# MaintenanceWindowTaskTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import MaintenanceWindowTaskTypeDef


def get_value() -> MaintenanceWindowTaskTypeDef:
    return {
        "WindowId": ...,
    }


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
# TargetLocationOutputTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import TargetLocationOutputTypeDef


def get_value() -> TargetLocationOutputTypeDef:
    return {
        "Accounts": ...,
    }


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
## ListAssociationsResultTypeDef

```python
# ListAssociationsResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListAssociationsResultTypeDef


def get_value() -> ListAssociationsResultTypeDef:
    return {
        "Associations": ...,
    }


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
# DescribeMaintenanceWindowTargetsResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowTargetsResultTypeDef


def get_value() -> DescribeMaintenanceWindowTargetsResultTypeDef:
    return {
        "Targets": ...,
    }


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
# DescribeAssociationExecutionTargetsResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeAssociationExecutionTargetsResultTypeDef


def get_value() -> DescribeAssociationExecutionTargetsResultTypeDef:
    return {
        "AssociationExecutionTargets": ...,
    }


# DescribeAssociationExecutionTargetsResultTypeDef definition

class DescribeAssociationExecutionTargetsResultTypeDef(TypedDict):
    AssociationExecutionTargets: List[AssociationExecutionTargetTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AssociationExecutionTargetTypeDef](./type_defs.md#associationexecutiontargettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecutionPreviewTypeDef

```python
# ExecutionPreviewTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ExecutionPreviewTypeDef


def get_value() -> ExecutionPreviewTypeDef:
    return {
        "Automation": ...,
    }


# ExecutionPreviewTypeDef definition

class ExecutionPreviewTypeDef(TypedDict):
    Automation: NotRequired[AutomationExecutionPreviewTypeDef],  # (1)
```

1. See [:material-code-braces: AutomationExecutionPreviewTypeDef](./type_defs.md#automationexecutionpreviewtypedef) 
## ListCommandInvocationsResultTypeDef

```python
# ListCommandInvocationsResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListCommandInvocationsResultTypeDef


def get_value() -> ListCommandInvocationsResultTypeDef:
    return {
        "CommandInvocations": ...,
    }


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
# MaintenanceWindowTaskInvocationParametersOutputTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import MaintenanceWindowTaskInvocationParametersOutputTypeDef


def get_value() -> MaintenanceWindowTaskInvocationParametersOutputTypeDef:
    return {
        "RunCommand": ...,
    }


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
# ListComplianceItemsResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListComplianceItemsResultTypeDef


def get_value() -> ListComplianceItemsResultTypeDef:
    return {
        "ComplianceItems": ...,
    }


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
# ComplianceSummaryItemTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ComplianceSummaryItemTypeDef


def get_value() -> ComplianceSummaryItemTypeDef:
    return {
        "ComplianceType": ...,
    }


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
# ResourceComplianceSummaryItemTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ResourceComplianceSummaryItemTypeDef


def get_value() -> ResourceComplianceSummaryItemTypeDef:
    return {
        "ComplianceType": ...,
    }


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
# ListDocumentsResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListDocumentsResultTypeDef


def get_value() -> ListDocumentsResultTypeDef:
    return {
        "DocumentIdentifiers": ...,
    }


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
# DescribeOpsItemsResponseTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeOpsItemsResponseTypeDef


def get_value() -> DescribeOpsItemsResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# GetOpsItemResponseTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetOpsItemResponseTypeDef


def get_value() -> GetOpsItemResponseTypeDef:
    return {
        "OpsItem": ...,
    }


# GetOpsItemResponseTypeDef definition

class GetOpsItemResponseTypeDef(TypedDict):
    OpsItem: OpsItemTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OpsItemTypeDef](./type_defs.md#opsitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePatchGroupsResultTypeDef

```python
# DescribePatchGroupsResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribePatchGroupsResultTypeDef


def get_value() -> DescribePatchGroupsResultTypeDef:
    return {
        "Mappings": ...,
    }


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
# CreateDocumentResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CreateDocumentResultTypeDef


def get_value() -> CreateDocumentResultTypeDef:
    return {
        "DocumentDescription": ...,
    }


# CreateDocumentResultTypeDef definition

class CreateDocumentResultTypeDef(TypedDict):
    DocumentDescription: DocumentDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DocumentDescriptionTypeDef](./type_defs.md#documentdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDocumentResultTypeDef

```python
# DescribeDocumentResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeDocumentResultTypeDef


def get_value() -> DescribeDocumentResultTypeDef:
    return {
        "Document": ...,
    }


# DescribeDocumentResultTypeDef definition

class DescribeDocumentResultTypeDef(TypedDict):
    Document: DocumentDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DocumentDescriptionTypeDef](./type_defs.md#documentdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDocumentResultTypeDef

```python
# UpdateDocumentResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdateDocumentResultTypeDef


def get_value() -> UpdateDocumentResultTypeDef:
    return {
        "DocumentDescription": ...,
    }


# UpdateDocumentResultTypeDef definition

class UpdateDocumentResultTypeDef(TypedDict):
    DocumentDescription: DocumentDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DocumentDescriptionTypeDef](./type_defs.md#documentdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DocumentMetadataResponseInfoTypeDef

```python
# DocumentMetadataResponseInfoTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DocumentMetadataResponseInfoTypeDef


def get_value() -> DocumentMetadataResponseInfoTypeDef:
    return {
        "ReviewerResponse": ...,
    }


# DocumentMetadataResponseInfoTypeDef definition

class DocumentMetadataResponseInfoTypeDef(TypedDict):
    ReviewerResponse: NotRequired[List[DocumentReviewerResponseSourceTypeDef]],  # (1)
```

1. See [:material-code-braces: DocumentReviewerResponseSourceTypeDef](./type_defs.md#documentreviewerresponsesourcetypedef) 
## UpdateDocumentMetadataRequestTypeDef

```python
# UpdateDocumentMetadataRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdateDocumentMetadataRequestTypeDef


def get_value() -> UpdateDocumentMetadataRequestTypeDef:
    return {
        "Name": ...,
    }


# UpdateDocumentMetadataRequestTypeDef definition

class UpdateDocumentMetadataRequestTypeDef(TypedDict):
    Name: str,
    DocumentReviews: DocumentReviewsTypeDef,  # (1)
    DocumentVersion: NotRequired[str],
```

1. See [:material-code-braces: DocumentReviewsTypeDef](./type_defs.md#documentreviewstypedef) 
## DescribeEffectivePatchesForPatchBaselineResultTypeDef

```python
# DescribeEffectivePatchesForPatchBaselineResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeEffectivePatchesForPatchBaselineResultTypeDef


def get_value() -> DescribeEffectivePatchesForPatchBaselineResultTypeDef:
    return {
        "EffectivePatches": ...,
    }


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
# InventoryAggregatorPaginatorTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InventoryAggregatorPaginatorTypeDef


def get_value() -> InventoryAggregatorPaginatorTypeDef:
    return {
        "Expression": ...,
    }


# InventoryAggregatorPaginatorTypeDef definition

class InventoryAggregatorPaginatorTypeDef(TypedDict):
    Expression: NotRequired[str],
    Aggregators: NotRequired[Sequence[Mapping[str, Any]]],
    Groups: NotRequired[Sequence[InventoryGroupTypeDef]],  # (1)
```

1. See [:material-code-braces: InventoryGroupTypeDef](./type_defs.md#inventorygrouptypedef) 
## InventoryAggregatorTypeDef

```python
# InventoryAggregatorTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InventoryAggregatorTypeDef


def get_value() -> InventoryAggregatorTypeDef:
    return {
        "Expression": ...,
    }


# InventoryAggregatorTypeDef definition

class InventoryAggregatorTypeDef(TypedDict):
    Expression: NotRequired[str],
    Aggregators: NotRequired[Sequence[Mapping[str, Any]]],
    Groups: NotRequired[Sequence[InventoryGroupTypeDef]],  # (1)
```

1. See [:material-code-braces: InventoryGroupTypeDef](./type_defs.md#inventorygrouptypedef) 
## GetOpsSummaryRequestPaginateTypeDef

```python
# GetOpsSummaryRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetOpsSummaryRequestPaginateTypeDef


def get_value() -> GetOpsSummaryRequestPaginateTypeDef:
    return {
        "SyncName": ...,
    }


# GetOpsSummaryRequestPaginateTypeDef definition

class GetOpsSummaryRequestPaginateTypeDef(TypedDict):
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
## GetOpsSummaryRequestTypeDef

```python
# GetOpsSummaryRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetOpsSummaryRequestTypeDef


def get_value() -> GetOpsSummaryRequestTypeDef:
    return {
        "SyncName": ...,
    }


# GetOpsSummaryRequestTypeDef definition

class GetOpsSummaryRequestTypeDef(TypedDict):
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
# DescribeInstanceInformationResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeInstanceInformationResultTypeDef


def get_value() -> DescribeInstanceInformationResultTypeDef:
    return {
        "InstanceInformationList": ...,
    }


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
# DescribeInstancePropertiesResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeInstancePropertiesResultTypeDef


def get_value() -> DescribeInstancePropertiesResultTypeDef:
    return {
        "InstanceProperties": ...,
    }


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
# InstanceAssociationStatusInfoTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InstanceAssociationStatusInfoTypeDef


def get_value() -> InstanceAssociationStatusInfoTypeDef:
    return {
        "AssociationId": ...,
    }


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
## NodeTypeDef

```python
# NodeTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import NodeTypeDef


def get_value() -> NodeTypeDef:
    return {
        "CaptureTime": ...,
    }


# NodeTypeDef definition

class NodeTypeDef(TypedDict):
    CaptureTime: NotRequired[datetime],
    Id: NotRequired[str],
    Owner: NotRequired[NodeOwnerInfoTypeDef],  # (1)
    Region: NotRequired[str],
    NodeType: NotRequired[NodeTypeTypeDef],  # (2)
```

1. See [:material-code-braces: NodeOwnerInfoTypeDef](./type_defs.md#nodeownerinfotypedef) 
2. See [:material-code-braces: NodeTypeTypeDef](./type_defs.md#nodetypetypedef) 
## DeleteInventoryResultTypeDef

```python
# DeleteInventoryResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DeleteInventoryResultTypeDef


def get_value() -> DeleteInventoryResultTypeDef:
    return {
        "DeletionId": ...,
    }


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
# InventoryDeletionStatusItemTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import InventoryDeletionStatusItemTypeDef


def get_value() -> InventoryDeletionStatusItemTypeDef:
    return {
        "DeletionId": ...,
    }


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
# GetInventorySchemaResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetInventorySchemaResultTypeDef


def get_value() -> GetInventorySchemaResultTypeDef:
    return {
        "Schemas": ...,
    }


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
# GetInventoryResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetInventoryResultTypeDef


def get_value() -> GetInventoryResultTypeDef:
    return {
        "Entities": ...,
    }


# GetInventoryResultTypeDef definition

class GetInventoryResultTypeDef(TypedDict):
    Entities: List[InventoryResultEntityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InventoryResultEntityTypeDef](./type_defs.md#inventoryresultentitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MaintenanceWindowTaskInvocationParametersTypeDef

```python
# MaintenanceWindowTaskInvocationParametersTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import MaintenanceWindowTaskInvocationParametersTypeDef


def get_value() -> MaintenanceWindowTaskInvocationParametersTypeDef:
    return {
        "RunCommand": ...,
    }


# MaintenanceWindowTaskInvocationParametersTypeDef definition

class MaintenanceWindowTaskInvocationParametersTypeDef(TypedDict):
    RunCommand: NotRequired[MaintenanceWindowRunCommandParametersTypeDef],  # (1)
    Automation: NotRequired[MaintenanceWindowAutomationParametersTypeDef],  # (2)
    StepFunctions: NotRequired[MaintenanceWindowStepFunctionsParametersTypeDef],  # (3)
    Lambda: NotRequired[MaintenanceWindowLambdaParametersTypeDef],  # (4)
```

1. See [:material-code-braces: MaintenanceWindowRunCommandParametersTypeDef](./type_defs.md#maintenancewindowruncommandparameterstypedef) 
2. See [:material-code-braces: MaintenanceWindowAutomationParametersTypeDef](./type_defs.md#maintenancewindowautomationparameterstypedef) 
3. See [:material-code-braces: MaintenanceWindowStepFunctionsParametersTypeDef](./type_defs.md#maintenancewindowstepfunctionsparameterstypedef) 
4. See [:material-code-braces: MaintenanceWindowLambdaParametersTypeDef](./type_defs.md#maintenancewindowlambdaparameterstypedef) 
## GetOpsSummaryResultTypeDef

```python
# GetOpsSummaryResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetOpsSummaryResultTypeDef


def get_value() -> GetOpsSummaryResultTypeDef:
    return {
        "Entities": ...,
    }


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
# ListOpsItemEventsResponseTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListOpsItemEventsResponseTypeDef


def get_value() -> ListOpsItemEventsResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# ListOpsItemRelatedItemsResponseTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListOpsItemRelatedItemsResponseTypeDef


def get_value() -> ListOpsItemRelatedItemsResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# GetParameterHistoryResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetParameterHistoryResultTypeDef


def get_value() -> GetParameterHistoryResultTypeDef:
    return {
        "Parameters": ...,
    }


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
# DescribeParametersResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeParametersResultTypeDef


def get_value() -> DescribeParametersResultTypeDef:
    return {
        "Parameters": ...,
    }


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
# PatchRuleOutputTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PatchRuleOutputTypeDef


def get_value() -> PatchRuleOutputTypeDef:
    return {
        "PatchFilterGroup": ...,
    }


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
# PatchFilterGroupTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PatchFilterGroupTypeDef


def get_value() -> PatchFilterGroupTypeDef:
    return {
        "PatchFilters": ...,
    }


# PatchFilterGroupTypeDef definition

class PatchFilterGroupTypeDef(TypedDict):
    PatchFilters: Sequence[PatchFilterUnionTypeDef],  # (1)
```

1. See [:material-code-braces: PatchFilterTypeDef](./type_defs.md#patchfiltertypedef) [:material-code-braces: PatchFilterOutputTypeDef](./type_defs.md#patchfilteroutputtypedef) 
## ResourceDataSyncSourceWithStateTypeDef

```python
# ResourceDataSyncSourceWithStateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ResourceDataSyncSourceWithStateTypeDef


def get_value() -> ResourceDataSyncSourceWithStateTypeDef:
    return {
        "SourceType": ...,
    }


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
# DescribeSessionsResponseTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeSessionsResponseTypeDef


def get_value() -> DescribeSessionsResponseTypeDef:
    return {
        "Sessions": ...,
    }


# DescribeSessionsResponseTypeDef definition

class DescribeSessionsResponseTypeDef(TypedDict):
    Sessions: List[SessionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SessionTypeDef](./type_defs.md#sessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMaintenanceWindowScheduleRequestPaginateTypeDef

```python
# DescribeMaintenanceWindowScheduleRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowScheduleRequestPaginateTypeDef


def get_value() -> DescribeMaintenanceWindowScheduleRequestPaginateTypeDef:
    return {
        "WindowId": ...,
    }


# DescribeMaintenanceWindowScheduleRequestPaginateTypeDef definition

class DescribeMaintenanceWindowScheduleRequestPaginateTypeDef(TypedDict):
    WindowId: NotRequired[str],
    Targets: NotRequired[Sequence[TargetUnionTypeDef]],  # (1)
    ResourceType: NotRequired[MaintenanceWindowResourceTypeType],  # (2)
    Filters: NotRequired[Sequence[PatchOrchestratorFilterTypeDef]],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-brackets: MaintenanceWindowResourceTypeType](./literals.md#maintenancewindowresourcetypetype) 
3. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeMaintenanceWindowScheduleRequestTypeDef

```python
# DescribeMaintenanceWindowScheduleRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowScheduleRequestTypeDef


def get_value() -> DescribeMaintenanceWindowScheduleRequestTypeDef:
    return {
        "WindowId": ...,
    }


# DescribeMaintenanceWindowScheduleRequestTypeDef definition

class DescribeMaintenanceWindowScheduleRequestTypeDef(TypedDict):
    WindowId: NotRequired[str],
    Targets: NotRequired[Sequence[TargetUnionTypeDef]],  # (1)
    ResourceType: NotRequired[MaintenanceWindowResourceTypeType],  # (2)
    Filters: NotRequired[Sequence[PatchOrchestratorFilterTypeDef]],  # (3)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-brackets: MaintenanceWindowResourceTypeType](./literals.md#maintenancewindowresourcetypetype) 
3. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
## DescribeMaintenanceWindowsForTargetRequestPaginateTypeDef

```python
# DescribeMaintenanceWindowsForTargetRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowsForTargetRequestPaginateTypeDef


def get_value() -> DescribeMaintenanceWindowsForTargetRequestPaginateTypeDef:
    return {
        "Targets": ...,
    }


# DescribeMaintenanceWindowsForTargetRequestPaginateTypeDef definition

class DescribeMaintenanceWindowsForTargetRequestPaginateTypeDef(TypedDict):
    Targets: Sequence[TargetUnionTypeDef],  # (1)
    ResourceType: MaintenanceWindowResourceTypeType,  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-brackets: MaintenanceWindowResourceTypeType](./literals.md#maintenancewindowresourcetypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeMaintenanceWindowsForTargetRequestTypeDef

```python
# DescribeMaintenanceWindowsForTargetRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowsForTargetRequestTypeDef


def get_value() -> DescribeMaintenanceWindowsForTargetRequestTypeDef:
    return {
        "Targets": ...,
    }


# DescribeMaintenanceWindowsForTargetRequestTypeDef definition

class DescribeMaintenanceWindowsForTargetRequestTypeDef(TypedDict):
    Targets: Sequence[TargetUnionTypeDef],  # (1)
    ResourceType: MaintenanceWindowResourceTypeType,  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-brackets: MaintenanceWindowResourceTypeType](./literals.md#maintenancewindowresourcetypetype) 
## RegisterTargetWithMaintenanceWindowRequestTypeDef

```python
# RegisterTargetWithMaintenanceWindowRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import RegisterTargetWithMaintenanceWindowRequestTypeDef


def get_value() -> RegisterTargetWithMaintenanceWindowRequestTypeDef:
    return {
        "WindowId": ...,
    }


# RegisterTargetWithMaintenanceWindowRequestTypeDef definition

class RegisterTargetWithMaintenanceWindowRequestTypeDef(TypedDict):
    WindowId: str,
    ResourceType: MaintenanceWindowResourceTypeType,  # (1)
    Targets: Sequence[TargetUnionTypeDef],  # (2)
    OwnerInformation: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    ClientToken: NotRequired[str],
```

1. See [:material-code-brackets: MaintenanceWindowResourceTypeType](./literals.md#maintenancewindowresourcetypetype) 
2. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
## UpdateMaintenanceWindowTargetRequestTypeDef

```python
# UpdateMaintenanceWindowTargetRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdateMaintenanceWindowTargetRequestTypeDef


def get_value() -> UpdateMaintenanceWindowTargetRequestTypeDef:
    return {
        "WindowId": ...,
    }


# UpdateMaintenanceWindowTargetRequestTypeDef definition

class UpdateMaintenanceWindowTargetRequestTypeDef(TypedDict):
    WindowId: str,
    WindowTargetId: str,
    Targets: NotRequired[Sequence[TargetUnionTypeDef]],  # (1)
    OwnerInformation: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    Replace: NotRequired[bool],
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
## DescribeAssociationExecutionsResultTypeDef

```python
# DescribeAssociationExecutionsResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeAssociationExecutionsResultTypeDef


def get_value() -> DescribeAssociationExecutionsResultTypeDef:
    return {
        "AssociationExecutions": ...,
    }


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
# ListCommandsResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListCommandsResultTypeDef


def get_value() -> ListCommandsResultTypeDef:
    return {
        "Commands": ...,
    }


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
# SendCommandResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import SendCommandResultTypeDef


def get_value() -> SendCommandResultTypeDef:
    return {
        "Command": ...,
    }


# SendCommandResultTypeDef definition

class SendCommandResultTypeDef(TypedDict):
    Command: CommandTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CommandTypeDef](./type_defs.md#commandtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMaintenanceWindowExecutionTasksResultTypeDef

```python
# DescribeMaintenanceWindowExecutionTasksResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowExecutionTasksResultTypeDef


def get_value() -> DescribeMaintenanceWindowExecutionTasksResultTypeDef:
    return {
        "WindowExecutionTaskIdentities": ...,
    }


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
# DescribeMaintenanceWindowTasksResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeMaintenanceWindowTasksResultTypeDef


def get_value() -> DescribeMaintenanceWindowTasksResultTypeDef:
    return {
        "Tasks": ...,
    }


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
# AssociationDescriptionTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AssociationDescriptionTypeDef


def get_value() -> AssociationDescriptionTypeDef:
    return {
        "Name": ...,
    }


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
# AssociationVersionInfoTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AssociationVersionInfoTypeDef


def get_value() -> AssociationVersionInfoTypeDef:
    return {
        "AssociationId": ...,
    }


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
# CreateAssociationBatchRequestEntryOutputTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CreateAssociationBatchRequestEntryOutputTypeDef


def get_value() -> CreateAssociationBatchRequestEntryOutputTypeDef:
    return {
        "Name": ...,
    }


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
# RunbookOutputTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import RunbookOutputTypeDef


def get_value() -> RunbookOutputTypeDef:
    return {
        "DocumentName": ...,
    }


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
# StepExecutionTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import StepExecutionTypeDef


def get_value() -> StepExecutionTypeDef:
    return {
        "StepName": ...,
    }


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
## SendCommandRequestTypeDef

```python
# SendCommandRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import SendCommandRequestTypeDef


def get_value() -> SendCommandRequestTypeDef:
    return {
        "DocumentName": ...,
    }


# SendCommandRequestTypeDef definition

class SendCommandRequestTypeDef(TypedDict):
    DocumentName: str,
    InstanceIds: NotRequired[Sequence[str]],
    Targets: NotRequired[Sequence[TargetUnionTypeDef]],  # (1)
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
    NotificationConfig: NotRequired[NotificationConfigUnionTypeDef],  # (3)
    CloudWatchOutputConfig: NotRequired[CloudWatchOutputConfigTypeDef],  # (4)
    AlarmConfiguration: NotRequired[AlarmConfigurationUnionTypeDef],  # (5)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-brackets: DocumentHashTypeType](./literals.md#documenthashtypetype) 
3. See [:material-code-braces: NotificationConfigTypeDef](./type_defs.md#notificationconfigtypedef) [:material-code-braces: NotificationConfigOutputTypeDef](./type_defs.md#notificationconfigoutputtypedef) 
4. See [:material-code-braces: CloudWatchOutputConfigTypeDef](./type_defs.md#cloudwatchoutputconfigtypedef) 
5. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
## TargetLocationTypeDef

```python
# TargetLocationTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import TargetLocationTypeDef


def get_value() -> TargetLocationTypeDef:
    return {
        "Accounts": ...,
    }


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
## UpdateAssociationStatusRequestTypeDef

```python
# UpdateAssociationStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdateAssociationStatusRequestTypeDef


def get_value() -> UpdateAssociationStatusRequestTypeDef:
    return {
        "Name": ...,
    }


# UpdateAssociationStatusRequestTypeDef definition

class UpdateAssociationStatusRequestTypeDef(TypedDict):
    Name: str,
    InstanceId: str,
    AssociationStatus: AssociationStatusUnionTypeDef,  # (1)
```

1. See [:material-code-braces: AssociationStatusTypeDef](./type_defs.md#associationstatustypedef) [:material-code-braces: AssociationStatusOutputTypeDef](./type_defs.md#associationstatusoutputtypedef) 
## PutComplianceItemsRequestTypeDef

```python
# PutComplianceItemsRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PutComplianceItemsRequestTypeDef


def get_value() -> PutComplianceItemsRequestTypeDef:
    return {
        "ResourceId": ...,
    }


# PutComplianceItemsRequestTypeDef definition

class PutComplianceItemsRequestTypeDef(TypedDict):
    ResourceId: str,
    ResourceType: str,
    ComplianceType: str,
    ExecutionSummary: ComplianceExecutionSummaryUnionTypeDef,  # (1)
    Items: Sequence[ComplianceItemEntryTypeDef],  # (2)
    ItemContentHash: NotRequired[str],
    UploadType: NotRequired[ComplianceUploadTypeType],  # (3)
```

1. See [:material-code-braces: ComplianceExecutionSummaryTypeDef](./type_defs.md#complianceexecutionsummarytypedef) [:material-code-braces: ComplianceExecutionSummaryOutputTypeDef](./type_defs.md#complianceexecutionsummaryoutputtypedef) 
2. See [:material-code-braces: ComplianceItemEntryTypeDef](./type_defs.md#complianceitementrytypedef) 
3. See [:material-code-brackets: ComplianceUploadTypeType](./literals.md#complianceuploadtypetype) 
## GetExecutionPreviewResponseTypeDef

```python
# GetExecutionPreviewResponseTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetExecutionPreviewResponseTypeDef


def get_value() -> GetExecutionPreviewResponseTypeDef:
    return {
        "ExecutionPreviewId": ...,
    }


# GetExecutionPreviewResponseTypeDef definition

class GetExecutionPreviewResponseTypeDef(TypedDict):
    ExecutionPreviewId: str,
    EndedAt: datetime,
    Status: ExecutionPreviewStatusType,  # (1)
    StatusMessage: str,
    ExecutionPreview: ExecutionPreviewTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ExecutionPreviewStatusType](./literals.md#executionpreviewstatustype) 
2. See [:material-code-braces: ExecutionPreviewTypeDef](./type_defs.md#executionpreviewtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMaintenanceWindowTaskResultTypeDef

```python
# GetMaintenanceWindowTaskResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetMaintenanceWindowTaskResultTypeDef


def get_value() -> GetMaintenanceWindowTaskResultTypeDef:
    return {
        "WindowId": ...,
    }


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
# UpdateMaintenanceWindowTaskResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdateMaintenanceWindowTaskResultTypeDef


def get_value() -> UpdateMaintenanceWindowTaskResultTypeDef:
    return {
        "WindowId": ...,
    }


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
# ListComplianceSummariesResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListComplianceSummariesResultTypeDef


def get_value() -> ListComplianceSummariesResultTypeDef:
    return {
        "ComplianceSummaryItems": ...,
    }


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
# ListResourceComplianceSummariesResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListResourceComplianceSummariesResultTypeDef


def get_value() -> ListResourceComplianceSummariesResultTypeDef:
    return {
        "ResourceComplianceSummaryItems": ...,
    }


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
# ListDocumentMetadataHistoryResponseTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListDocumentMetadataHistoryResponseTypeDef


def get_value() -> ListDocumentMetadataHistoryResponseTypeDef:
    return {
        "Name": ...,
    }


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
## GetInventoryRequestPaginateTypeDef

```python
# GetInventoryRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetInventoryRequestPaginateTypeDef


def get_value() -> GetInventoryRequestPaginateTypeDef:
    return {
        "Filters": ...,
    }


# GetInventoryRequestPaginateTypeDef definition

class GetInventoryRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[InventoryFilterTypeDef]],  # (1)
    Aggregators: NotRequired[Sequence[InventoryAggregatorPaginatorTypeDef]],  # (2)
    ResultAttributes: NotRequired[Sequence[ResultAttributeTypeDef]],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: InventoryFilterTypeDef](./type_defs.md#inventoryfiltertypedef) 
2. See [:material-code-braces: InventoryAggregatorPaginatorTypeDef](./type_defs.md#inventoryaggregatorpaginatortypedef) 
3. See [:material-code-braces: ResultAttributeTypeDef](./type_defs.md#resultattributetypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetInventoryRequestTypeDef

```python
# GetInventoryRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetInventoryRequestTypeDef


def get_value() -> GetInventoryRequestTypeDef:
    return {
        "Filters": ...,
    }


# GetInventoryRequestTypeDef definition

class GetInventoryRequestTypeDef(TypedDict):
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
# DescribeInstanceAssociationsStatusResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeInstanceAssociationsStatusResultTypeDef


def get_value() -> DescribeInstanceAssociationsStatusResultTypeDef:
    return {
        "InstanceAssociationStatusInfos": ...,
    }


# DescribeInstanceAssociationsStatusResultTypeDef definition

class DescribeInstanceAssociationsStatusResultTypeDef(TypedDict):
    InstanceAssociationStatusInfos: List[InstanceAssociationStatusInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InstanceAssociationStatusInfoTypeDef](./type_defs.md#instanceassociationstatusinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNodesResultTypeDef

```python
# ListNodesResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListNodesResultTypeDef


def get_value() -> ListNodesResultTypeDef:
    return {
        "Nodes": ...,
    }


# ListNodesResultTypeDef definition

class ListNodesResultTypeDef(TypedDict):
    Nodes: List[NodeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: NodeTypeDef](./type_defs.md#nodetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInventoryDeletionsResultTypeDef

```python
# DescribeInventoryDeletionsResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeInventoryDeletionsResultTypeDef


def get_value() -> DescribeInventoryDeletionsResultTypeDef:
    return {
        "InventoryDeletions": ...,
    }


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
# PatchRuleGroupOutputTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PatchRuleGroupOutputTypeDef


def get_value() -> PatchRuleGroupOutputTypeDef:
    return {
        "PatchRules": ...,
    }


# PatchRuleGroupOutputTypeDef definition

class PatchRuleGroupOutputTypeDef(TypedDict):
    PatchRules: List[PatchRuleOutputTypeDef],  # (1)
```

1. See [:material-code-braces: PatchRuleOutputTypeDef](./type_defs.md#patchruleoutputtypedef) 
## ResourceDataSyncItemTypeDef

```python
# ResourceDataSyncItemTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ResourceDataSyncItemTypeDef


def get_value() -> ResourceDataSyncItemTypeDef:
    return {
        "SyncName": ...,
    }


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
# ResourceDataSyncSourceTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ResourceDataSyncSourceTypeDef


def get_value() -> ResourceDataSyncSourceTypeDef:
    return {
        "SourceType": ...,
    }


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
# CreateAssociationResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CreateAssociationResultTypeDef


def get_value() -> CreateAssociationResultTypeDef:
    return {
        "AssociationDescription": ...,
    }


# CreateAssociationResultTypeDef definition

class CreateAssociationResultTypeDef(TypedDict):
    AssociationDescription: AssociationDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssociationDescriptionTypeDef](./type_defs.md#associationdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAssociationResultTypeDef

```python
# DescribeAssociationResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeAssociationResultTypeDef


def get_value() -> DescribeAssociationResultTypeDef:
    return {
        "AssociationDescription": ...,
    }


# DescribeAssociationResultTypeDef definition

class DescribeAssociationResultTypeDef(TypedDict):
    AssociationDescription: AssociationDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssociationDescriptionTypeDef](./type_defs.md#associationdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAssociationResultTypeDef

```python
# UpdateAssociationResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdateAssociationResultTypeDef


def get_value() -> UpdateAssociationResultTypeDef:
    return {
        "AssociationDescription": ...,
    }


# UpdateAssociationResultTypeDef definition

class UpdateAssociationResultTypeDef(TypedDict):
    AssociationDescription: AssociationDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssociationDescriptionTypeDef](./type_defs.md#associationdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAssociationStatusResultTypeDef

```python
# UpdateAssociationStatusResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdateAssociationStatusResultTypeDef


def get_value() -> UpdateAssociationStatusResultTypeDef:
    return {
        "AssociationDescription": ...,
    }


# UpdateAssociationStatusResultTypeDef definition

class UpdateAssociationStatusResultTypeDef(TypedDict):
    AssociationDescription: AssociationDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssociationDescriptionTypeDef](./type_defs.md#associationdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssociationVersionsResultTypeDef

```python
# ListAssociationVersionsResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListAssociationVersionsResultTypeDef


def get_value() -> ListAssociationVersionsResultTypeDef:
    return {
        "AssociationVersions": ...,
    }


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
# FailedCreateAssociationTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import FailedCreateAssociationTypeDef


def get_value() -> FailedCreateAssociationTypeDef:
    return {
        "Entry": ...,
    }


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
# AutomationExecutionMetadataTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AutomationExecutionMetadataTypeDef


def get_value() -> AutomationExecutionMetadataTypeDef:
    return {
        "AutomationExecutionId": ...,
    }


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
# AutomationExecutionTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AutomationExecutionTypeDef


def get_value() -> AutomationExecutionTypeDef:
    return {
        "AutomationExecutionId": ...,
    }


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
# DescribeAutomationStepExecutionsResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeAutomationStepExecutionsResultTypeDef


def get_value() -> DescribeAutomationStepExecutionsResultTypeDef:
    return {
        "StepExecutions": ...,
    }


# DescribeAutomationStepExecutionsResultTypeDef definition

class DescribeAutomationStepExecutionsResultTypeDef(TypedDict):
    StepExecutions: List[StepExecutionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: StepExecutionTypeDef](./type_defs.md#stepexecutiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterTaskWithMaintenanceWindowRequestTypeDef

```python
# RegisterTaskWithMaintenanceWindowRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import RegisterTaskWithMaintenanceWindowRequestTypeDef


def get_value() -> RegisterTaskWithMaintenanceWindowRequestTypeDef:
    return {
        "WindowId": ...,
    }


# RegisterTaskWithMaintenanceWindowRequestTypeDef definition

class RegisterTaskWithMaintenanceWindowRequestTypeDef(TypedDict):
    WindowId: str,
    TaskArn: str,
    TaskType: MaintenanceWindowTaskTypeType,  # (1)
    Targets: NotRequired[Sequence[TargetUnionTypeDef]],  # (2)
    ServiceRoleArn: NotRequired[str],
    TaskParameters: NotRequired[Mapping[str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef]],  # (3)
    TaskInvocationParameters: NotRequired[MaintenanceWindowTaskInvocationParametersUnionTypeDef],  # (4)
    Priority: NotRequired[int],
    MaxConcurrency: NotRequired[str],
    MaxErrors: NotRequired[str],
    LoggingInfo: NotRequired[LoggingInfoTypeDef],  # (5)
    Name: NotRequired[str],
    Description: NotRequired[str],
    ClientToken: NotRequired[str],
    CutoffBehavior: NotRequired[MaintenanceWindowTaskCutoffBehaviorType],  # (6)
    AlarmConfiguration: NotRequired[AlarmConfigurationUnionTypeDef],  # (7)
```

1. See [:material-code-brackets: MaintenanceWindowTaskTypeType](./literals.md#maintenancewindowtasktypetype) 
2. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
3. See [:material-code-braces: MaintenanceWindowTaskParameterValueExpressionTypeDef](./type_defs.md#maintenancewindowtaskparametervalueexpressiontypedef) [:material-code-braces: MaintenanceWindowTaskParameterValueExpressionOutputTypeDef](./type_defs.md#maintenancewindowtaskparametervalueexpressionoutputtypedef) 
4. See [:material-code-braces: MaintenanceWindowTaskInvocationParametersTypeDef](./type_defs.md#maintenancewindowtaskinvocationparameterstypedef) [:material-code-braces: MaintenanceWindowTaskInvocationParametersOutputTypeDef](./type_defs.md#maintenancewindowtaskinvocationparametersoutputtypedef) 
5. See [:material-code-braces: LoggingInfoTypeDef](./type_defs.md#logginginfotypedef) 
6. See [:material-code-brackets: MaintenanceWindowTaskCutoffBehaviorType](./literals.md#maintenancewindowtaskcutoffbehaviortype) 
7. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
## UpdateMaintenanceWindowTaskRequestTypeDef

```python
# UpdateMaintenanceWindowTaskRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdateMaintenanceWindowTaskRequestTypeDef


def get_value() -> UpdateMaintenanceWindowTaskRequestTypeDef:
    return {
        "WindowId": ...,
    }


# UpdateMaintenanceWindowTaskRequestTypeDef definition

class UpdateMaintenanceWindowTaskRequestTypeDef(TypedDict):
    WindowId: str,
    WindowTaskId: str,
    Targets: NotRequired[Sequence[TargetUnionTypeDef]],  # (1)
    TaskArn: NotRequired[str],
    ServiceRoleArn: NotRequired[str],
    TaskParameters: NotRequired[Mapping[str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef]],  # (2)
    TaskInvocationParameters: NotRequired[MaintenanceWindowTaskInvocationParametersUnionTypeDef],  # (3)
    Priority: NotRequired[int],
    MaxConcurrency: NotRequired[str],
    MaxErrors: NotRequired[str],
    LoggingInfo: NotRequired[LoggingInfoTypeDef],  # (4)
    Name: NotRequired[str],
    Description: NotRequired[str],
    Replace: NotRequired[bool],
    CutoffBehavior: NotRequired[MaintenanceWindowTaskCutoffBehaviorType],  # (5)
    AlarmConfiguration: NotRequired[AlarmConfigurationUnionTypeDef],  # (6)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-braces: MaintenanceWindowTaskParameterValueExpressionTypeDef](./type_defs.md#maintenancewindowtaskparametervalueexpressiontypedef) [:material-code-braces: MaintenanceWindowTaskParameterValueExpressionOutputTypeDef](./type_defs.md#maintenancewindowtaskparametervalueexpressionoutputtypedef) 
3. See [:material-code-braces: MaintenanceWindowTaskInvocationParametersTypeDef](./type_defs.md#maintenancewindowtaskinvocationparameterstypedef) [:material-code-braces: MaintenanceWindowTaskInvocationParametersOutputTypeDef](./type_defs.md#maintenancewindowtaskinvocationparametersoutputtypedef) 
4. See [:material-code-braces: LoggingInfoTypeDef](./type_defs.md#logginginfotypedef) 
5. See [:material-code-brackets: MaintenanceWindowTaskCutoffBehaviorType](./literals.md#maintenancewindowtaskcutoffbehaviortype) 
6. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
## GetPatchBaselineResultTypeDef

```python
# GetPatchBaselineResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetPatchBaselineResultTypeDef


def get_value() -> GetPatchBaselineResultTypeDef:
    return {
        "BaselineId": ...,
    }


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
# UpdatePatchBaselineResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdatePatchBaselineResultTypeDef


def get_value() -> UpdatePatchBaselineResultTypeDef:
    return {
        "BaselineId": ...,
    }


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
# PatchRuleTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PatchRuleTypeDef


def get_value() -> PatchRuleTypeDef:
    return {
        "PatchFilterGroup": ...,
    }


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
# ListResourceDataSyncResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ListResourceDataSyncResultTypeDef


def get_value() -> ListResourceDataSyncResultTypeDef:
    return {
        "ResourceDataSyncItems": ...,
    }


# ListResourceDataSyncResultTypeDef definition

class ListResourceDataSyncResultTypeDef(TypedDict):
    ResourceDataSyncItems: List[ResourceDataSyncItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceDataSyncItemTypeDef](./type_defs.md#resourcedatasyncitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateResourceDataSyncRequestTypeDef

```python
# CreateResourceDataSyncRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CreateResourceDataSyncRequestTypeDef


def get_value() -> CreateResourceDataSyncRequestTypeDef:
    return {
        "SyncName": ...,
    }


# CreateResourceDataSyncRequestTypeDef definition

class CreateResourceDataSyncRequestTypeDef(TypedDict):
    SyncName: str,
    S3Destination: NotRequired[ResourceDataSyncS3DestinationTypeDef],  # (1)
    SyncType: NotRequired[str],
    SyncSource: NotRequired[ResourceDataSyncSourceTypeDef],  # (2)
```

1. See [:material-code-braces: ResourceDataSyncS3DestinationTypeDef](./type_defs.md#resourcedatasyncs3destinationtypedef) 
2. See [:material-code-braces: ResourceDataSyncSourceTypeDef](./type_defs.md#resourcedatasyncsourcetypedef) 
## UpdateResourceDataSyncRequestTypeDef

```python
# UpdateResourceDataSyncRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdateResourceDataSyncRequestTypeDef


def get_value() -> UpdateResourceDataSyncRequestTypeDef:
    return {
        "SyncName": ...,
    }


# UpdateResourceDataSyncRequestTypeDef definition

class UpdateResourceDataSyncRequestTypeDef(TypedDict):
    SyncName: str,
    SyncType: str,
    SyncSource: ResourceDataSyncSourceTypeDef,  # (1)
```

1. See [:material-code-braces: ResourceDataSyncSourceTypeDef](./type_defs.md#resourcedatasyncsourcetypedef) 
## CreateAssociationBatchResultTypeDef

```python
# CreateAssociationBatchResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CreateAssociationBatchResultTypeDef


def get_value() -> CreateAssociationBatchResultTypeDef:
    return {
        "Successful": ...,
    }


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
# DescribeAutomationExecutionsResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import DescribeAutomationExecutionsResultTypeDef


def get_value() -> DescribeAutomationExecutionsResultTypeDef:
    return {
        "AutomationExecutionMetadataList": ...,
    }


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
# GetAutomationExecutionResultTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetAutomationExecutionResultTypeDef


def get_value() -> GetAutomationExecutionResultTypeDef:
    return {
        "AutomationExecution": ...,
    }


# GetAutomationExecutionResultTypeDef definition

class GetAutomationExecutionResultTypeDef(TypedDict):
    AutomationExecution: AutomationExecutionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AutomationExecutionTypeDef](./type_defs.md#automationexecutiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AutomationExecutionInputsTypeDef

```python
# AutomationExecutionInputsTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import AutomationExecutionInputsTypeDef


def get_value() -> AutomationExecutionInputsTypeDef:
    return {
        "Parameters": ...,
    }


# AutomationExecutionInputsTypeDef definition

class AutomationExecutionInputsTypeDef(TypedDict):
    Parameters: NotRequired[Mapping[str, Sequence[str]]],
    TargetParameterName: NotRequired[str],
    Targets: NotRequired[Sequence[TargetUnionTypeDef]],  # (1)
    TargetMaps: NotRequired[Sequence[Mapping[str, Sequence[str]]]],
    TargetLocations: NotRequired[Sequence[TargetLocationUnionTypeDef]],  # (2)
    TargetLocationsURL: NotRequired[str],
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-braces: TargetLocationTypeDef](./type_defs.md#targetlocationtypedef) [:material-code-braces: TargetLocationOutputTypeDef](./type_defs.md#targetlocationoutputtypedef) 
## CreateAssociationBatchRequestEntryTypeDef

```python
# CreateAssociationBatchRequestEntryTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CreateAssociationBatchRequestEntryTypeDef


def get_value() -> CreateAssociationBatchRequestEntryTypeDef:
    return {
        "Name": ...,
    }


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
## CreateAssociationRequestTypeDef

```python
# CreateAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CreateAssociationRequestTypeDef


def get_value() -> CreateAssociationRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateAssociationRequestTypeDef definition

class CreateAssociationRequestTypeDef(TypedDict):
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
    AlarmConfiguration: NotRequired[AlarmConfigurationUnionTypeDef],  # (7)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-braces: InstanceAssociationOutputLocationTypeDef](./type_defs.md#instanceassociationoutputlocationtypedef) 
3. See [:material-code-brackets: AssociationComplianceSeverityType](./literals.md#associationcomplianceseveritytype) 
4. See [:material-code-brackets: AssociationSyncComplianceType](./literals.md#associationsynccompliancetype) 
5. See [:material-code-braces: TargetLocationTypeDef](./type_defs.md#targetlocationtypedef) [:material-code-braces: TargetLocationOutputTypeDef](./type_defs.md#targetlocationoutputtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
## RunbookTypeDef

```python
# RunbookTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import RunbookTypeDef


def get_value() -> RunbookTypeDef:
    return {
        "DocumentName": ...,
    }


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
## StartAutomationExecutionRequestTypeDef

```python
# StartAutomationExecutionRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import StartAutomationExecutionRequestTypeDef


def get_value() -> StartAutomationExecutionRequestTypeDef:
    return {
        "DocumentName": ...,
    }


# StartAutomationExecutionRequestTypeDef definition

class StartAutomationExecutionRequestTypeDef(TypedDict):
    DocumentName: str,
    DocumentVersion: NotRequired[str],
    Parameters: NotRequired[Mapping[str, Sequence[str]]],
    ClientToken: NotRequired[str],
    Mode: NotRequired[ExecutionModeType],  # (1)
    TargetParameterName: NotRequired[str],
    Targets: NotRequired[Sequence[TargetUnionTypeDef]],  # (2)
    TargetMaps: NotRequired[Sequence[Mapping[str, Sequence[str]]]],
    MaxConcurrency: NotRequired[str],
    MaxErrors: NotRequired[str],
    TargetLocations: NotRequired[Sequence[TargetLocationUnionTypeDef]],  # (3)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    AlarmConfiguration: NotRequired[AlarmConfigurationUnionTypeDef],  # (5)
    TargetLocationsURL: NotRequired[str],
```

1. See [:material-code-brackets: ExecutionModeType](./literals.md#executionmodetype) 
2. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
3. See [:material-code-braces: TargetLocationTypeDef](./type_defs.md#targetlocationtypedef) [:material-code-braces: TargetLocationOutputTypeDef](./type_defs.md#targetlocationoutputtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
## UpdateAssociationRequestTypeDef

```python
# UpdateAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdateAssociationRequestTypeDef


def get_value() -> UpdateAssociationRequestTypeDef:
    return {
        "AssociationId": ...,
    }


# UpdateAssociationRequestTypeDef definition

class UpdateAssociationRequestTypeDef(TypedDict):
    AssociationId: str,
    Parameters: NotRequired[Mapping[str, Sequence[str]]],
    DocumentVersion: NotRequired[str],
    ScheduleExpression: NotRequired[str],
    OutputLocation: NotRequired[InstanceAssociationOutputLocationTypeDef],  # (1)
    Name: NotRequired[str],
    Targets: NotRequired[Sequence[TargetUnionTypeDef]],  # (2)
    AssociationName: NotRequired[str],
    AssociationVersion: NotRequired[str],
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
    AlarmConfiguration: NotRequired[AlarmConfigurationUnionTypeDef],  # (6)
```

1. See [:material-code-braces: InstanceAssociationOutputLocationTypeDef](./type_defs.md#instanceassociationoutputlocationtypedef) 
2. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
3. See [:material-code-brackets: AssociationComplianceSeverityType](./literals.md#associationcomplianceseveritytype) 
4. See [:material-code-brackets: AssociationSyncComplianceType](./literals.md#associationsynccompliancetype) 
5. See [:material-code-braces: TargetLocationTypeDef](./type_defs.md#targetlocationtypedef) [:material-code-braces: TargetLocationOutputTypeDef](./type_defs.md#targetlocationoutputtypedef) 
6. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
## ExecutionInputsTypeDef

```python
# ExecutionInputsTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import ExecutionInputsTypeDef


def get_value() -> ExecutionInputsTypeDef:
    return {
        "Automation": ...,
    }


# ExecutionInputsTypeDef definition

class ExecutionInputsTypeDef(TypedDict):
    Automation: NotRequired[AutomationExecutionInputsTypeDef],  # (1)
```

1. See [:material-code-braces: AutomationExecutionInputsTypeDef](./type_defs.md#automationexecutioninputstypedef) 
## PatchRuleGroupTypeDef

```python
# PatchRuleGroupTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import PatchRuleGroupTypeDef


def get_value() -> PatchRuleGroupTypeDef:
    return {
        "PatchRules": ...,
    }


# PatchRuleGroupTypeDef definition

class PatchRuleGroupTypeDef(TypedDict):
    PatchRules: Sequence[PatchRuleUnionTypeDef],  # (1)
```

1. See [:material-code-braces: PatchRuleTypeDef](./type_defs.md#patchruletypedef) [:material-code-braces: PatchRuleOutputTypeDef](./type_defs.md#patchruleoutputtypedef) 
## StartExecutionPreviewRequestTypeDef

```python
# StartExecutionPreviewRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import StartExecutionPreviewRequestTypeDef


def get_value() -> StartExecutionPreviewRequestTypeDef:
    return {
        "DocumentName": ...,
    }


# StartExecutionPreviewRequestTypeDef definition

class StartExecutionPreviewRequestTypeDef(TypedDict):
    DocumentName: str,
    DocumentVersion: NotRequired[str],
    ExecutionInputs: NotRequired[ExecutionInputsTypeDef],  # (1)
```

1. See [:material-code-braces: ExecutionInputsTypeDef](./type_defs.md#executioninputstypedef) 
## CreateAssociationBatchRequestTypeDef

```python
# CreateAssociationBatchRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CreateAssociationBatchRequestTypeDef


def get_value() -> CreateAssociationBatchRequestTypeDef:
    return {
        "Entries": ...,
    }


# CreateAssociationBatchRequestTypeDef definition

class CreateAssociationBatchRequestTypeDef(TypedDict):
    Entries: Sequence[CreateAssociationBatchRequestEntryUnionTypeDef],  # (1)
```

1. See [:material-code-braces: CreateAssociationBatchRequestEntryTypeDef](./type_defs.md#createassociationbatchrequestentrytypedef) [:material-code-braces: CreateAssociationBatchRequestEntryOutputTypeDef](./type_defs.md#createassociationbatchrequestentryoutputtypedef) 
## StartChangeRequestExecutionRequestTypeDef

```python
# StartChangeRequestExecutionRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import StartChangeRequestExecutionRequestTypeDef


def get_value() -> StartChangeRequestExecutionRequestTypeDef:
    return {
        "DocumentName": ...,
    }


# StartChangeRequestExecutionRequestTypeDef definition

class StartChangeRequestExecutionRequestTypeDef(TypedDict):
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
## BaselineOverrideTypeDef

```python
# BaselineOverrideTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import BaselineOverrideTypeDef


def get_value() -> BaselineOverrideTypeDef:
    return {
        "OperatingSystem": ...,
    }


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
## CreatePatchBaselineRequestTypeDef

```python
# CreatePatchBaselineRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import CreatePatchBaselineRequestTypeDef


def get_value() -> CreatePatchBaselineRequestTypeDef:
    return {
        "Name": ...,
    }


# CreatePatchBaselineRequestTypeDef definition

class CreatePatchBaselineRequestTypeDef(TypedDict):
    Name: str,
    OperatingSystem: NotRequired[OperatingSystemType],  # (1)
    GlobalFilters: NotRequired[PatchFilterGroupUnionTypeDef],  # (2)
    ApprovalRules: NotRequired[PatchRuleGroupUnionTypeDef],  # (3)
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
2. See [:material-code-braces: PatchFilterGroupTypeDef](./type_defs.md#patchfiltergrouptypedef) [:material-code-braces: PatchFilterGroupOutputTypeDef](./type_defs.md#patchfiltergroupoutputtypedef) 
3. See [:material-code-braces: PatchRuleGroupTypeDef](./type_defs.md#patchrulegrouptypedef) [:material-code-braces: PatchRuleGroupOutputTypeDef](./type_defs.md#patchrulegroupoutputtypedef) 
4. See [:material-code-brackets: PatchComplianceLevelType](./literals.md#patchcomplianceleveltype) 
5. See [:material-code-brackets: PatchActionType](./literals.md#patchactiontype) 
6. See [:material-code-braces: PatchSourceTypeDef](./type_defs.md#patchsourcetypedef) [:material-code-braces: PatchSourceOutputTypeDef](./type_defs.md#patchsourceoutputtypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdatePatchBaselineRequestTypeDef

```python
# UpdatePatchBaselineRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import UpdatePatchBaselineRequestTypeDef


def get_value() -> UpdatePatchBaselineRequestTypeDef:
    return {
        "BaselineId": ...,
    }


# UpdatePatchBaselineRequestTypeDef definition

class UpdatePatchBaselineRequestTypeDef(TypedDict):
    BaselineId: str,
    Name: NotRequired[str],
    GlobalFilters: NotRequired[PatchFilterGroupUnionTypeDef],  # (1)
    ApprovalRules: NotRequired[PatchRuleGroupUnionTypeDef],  # (2)
    ApprovedPatches: NotRequired[Sequence[str]],
    ApprovedPatchesComplianceLevel: NotRequired[PatchComplianceLevelType],  # (3)
    ApprovedPatchesEnableNonSecurity: NotRequired[bool],
    RejectedPatches: NotRequired[Sequence[str]],
    RejectedPatchesAction: NotRequired[PatchActionType],  # (4)
    Description: NotRequired[str],
    Sources: NotRequired[Sequence[PatchSourceUnionTypeDef]],  # (5)
    Replace: NotRequired[bool],
```

1. See [:material-code-braces: PatchFilterGroupTypeDef](./type_defs.md#patchfiltergrouptypedef) [:material-code-braces: PatchFilterGroupOutputTypeDef](./type_defs.md#patchfiltergroupoutputtypedef) 
2. See [:material-code-braces: PatchRuleGroupTypeDef](./type_defs.md#patchrulegrouptypedef) [:material-code-braces: PatchRuleGroupOutputTypeDef](./type_defs.md#patchrulegroupoutputtypedef) 
3. See [:material-code-brackets: PatchComplianceLevelType](./literals.md#patchcomplianceleveltype) 
4. See [:material-code-brackets: PatchActionType](./literals.md#patchactiontype) 
5. See [:material-code-braces: PatchSourceTypeDef](./type_defs.md#patchsourcetypedef) [:material-code-braces: PatchSourceOutputTypeDef](./type_defs.md#patchsourceoutputtypedef) 
## GetDeployablePatchSnapshotForInstanceRequestTypeDef

```python
# GetDeployablePatchSnapshotForInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_ssm.type_defs import GetDeployablePatchSnapshotForInstanceRequestTypeDef


def get_value() -> GetDeployablePatchSnapshotForInstanceRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# GetDeployablePatchSnapshotForInstanceRequestTypeDef definition

class GetDeployablePatchSnapshotForInstanceRequestTypeDef(TypedDict):
    InstanceId: str,
    SnapshotId: str,
    BaselineOverride: NotRequired[BaselineOverrideTypeDef],  # (1)
```

1. See [:material-code-braces: BaselineOverrideTypeDef](./type_defs.md#baselineoverridetypedef) 
