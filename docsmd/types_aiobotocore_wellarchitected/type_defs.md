# Type definitions

> [Index](../README.md) > [WellArchitected](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [WellArchitected](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#wellarchitected)
    type annotations stubs module [types-aiobotocore-wellarchitected](https://pypi.org/project/types-aiobotocore-wellarchitected/).

## WorkloadDiscoveryConfigUnionTypeDef

```python
# WorkloadDiscoveryConfigUnionTypeDef Union usage example

from types_aiobotocore_wellarchitected.type_defs import WorkloadDiscoveryConfigUnionTypeDef


def get_value() -> WorkloadDiscoveryConfigUnionTypeDef:
    return ...


# WorkloadDiscoveryConfigUnionTypeDef definition

WorkloadDiscoveryConfigUnionTypeDef = Union[
    WorkloadDiscoveryConfigTypeDef,  # (1)
    WorkloadDiscoveryConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: WorkloadDiscoveryConfigTypeDef](./type_defs.md#workloaddiscoveryconfigtypedef) 
2. See [:material-code-braces: WorkloadDiscoveryConfigOutputTypeDef](./type_defs.md#workloaddiscoveryconfigoutputtypedef) 

## JiraSelectedQuestionConfigurationUnionTypeDef

```python
# JiraSelectedQuestionConfigurationUnionTypeDef Union usage example

from types_aiobotocore_wellarchitected.type_defs import JiraSelectedQuestionConfigurationUnionTypeDef


def get_value() -> JiraSelectedQuestionConfigurationUnionTypeDef:
    return ...


# JiraSelectedQuestionConfigurationUnionTypeDef definition

JiraSelectedQuestionConfigurationUnionTypeDef = Union[
    JiraSelectedQuestionConfigurationTypeDef,  # (1)
    JiraSelectedQuestionConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: JiraSelectedQuestionConfigurationTypeDef](./type_defs.md#jiraselectedquestionconfigurationtypedef) 
2. See [:material-code-braces: JiraSelectedQuestionConfigurationOutputTypeDef](./type_defs.md#jiraselectedquestionconfigurationoutputtypedef) 



## AccountJiraConfigurationInputTypeDef

```python
# AccountJiraConfigurationInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import AccountJiraConfigurationInputTypeDef


def get_value() -> AccountJiraConfigurationInputTypeDef:
    return {
        "IssueManagementStatus": ...,
    }


# AccountJiraConfigurationInputTypeDef definition

class AccountJiraConfigurationInputTypeDef(TypedDict):
    IssueManagementStatus: NotRequired[AccountJiraIssueManagementStatusType],  # (1)
    IssueManagementType: NotRequired[IssueManagementTypeType],  # (2)
    JiraProjectKey: NotRequired[str],
    IntegrationStatus: NotRequired[IntegrationStatusInputType],  # (3)
```

1. See [:material-code-brackets: AccountJiraIssueManagementStatusType](./literals.md#accountjiraissuemanagementstatustype) 
2. See [:material-code-brackets: IssueManagementTypeType](./literals.md#issuemanagementtypetype) 
3. See [:material-code-brackets: IntegrationStatusInputType](./literals.md#integrationstatusinputtype) 
## AccountJiraConfigurationOutputTypeDef

```python
# AccountJiraConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import AccountJiraConfigurationOutputTypeDef


def get_value() -> AccountJiraConfigurationOutputTypeDef:
    return {
        "IntegrationStatus": ...,
    }


# AccountJiraConfigurationOutputTypeDef definition

class AccountJiraConfigurationOutputTypeDef(TypedDict):
    IntegrationStatus: NotRequired[IntegrationStatusType],  # (1)
    IssueManagementStatus: NotRequired[AccountJiraIssueManagementStatusType],  # (2)
    IssueManagementType: NotRequired[IssueManagementTypeType],  # (3)
    Subdomain: NotRequired[str],
    JiraProjectKey: NotRequired[str],
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: IntegrationStatusType](./literals.md#integrationstatustype) 
2. See [:material-code-brackets: AccountJiraIssueManagementStatusType](./literals.md#accountjiraissuemanagementstatustype) 
3. See [:material-code-brackets: IssueManagementTypeType](./literals.md#issuemanagementtypetype) 
## ChoiceContentTypeDef

```python
# ChoiceContentTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ChoiceContentTypeDef


def get_value() -> ChoiceContentTypeDef:
    return {
        "DisplayText": ...,
    }


# ChoiceContentTypeDef definition

class ChoiceContentTypeDef(TypedDict):
    DisplayText: NotRequired[str],
    Url: NotRequired[str],
```

## ChoiceAnswerSummaryTypeDef

```python
# ChoiceAnswerSummaryTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ChoiceAnswerSummaryTypeDef


def get_value() -> ChoiceAnswerSummaryTypeDef:
    return {
        "ChoiceId": ...,
    }


# ChoiceAnswerSummaryTypeDef definition

class ChoiceAnswerSummaryTypeDef(TypedDict):
    ChoiceId: NotRequired[str],
    Status: NotRequired[ChoiceStatusType],  # (1)
    Reason: NotRequired[ChoiceReasonType],  # (2)
```

1. See [:material-code-brackets: ChoiceStatusType](./literals.md#choicestatustype) 
2. See [:material-code-brackets: ChoiceReasonType](./literals.md#choicereasontype) 
## JiraConfigurationTypeDef

```python
# JiraConfigurationTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import JiraConfigurationTypeDef


def get_value() -> JiraConfigurationTypeDef:
    return {
        "JiraIssueUrl": ...,
    }


# JiraConfigurationTypeDef definition

class JiraConfigurationTypeDef(TypedDict):
    JiraIssueUrl: NotRequired[str],
    LastSyncedTime: NotRequired[datetime],
```

## ChoiceAnswerTypeDef

```python
# ChoiceAnswerTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ChoiceAnswerTypeDef


def get_value() -> ChoiceAnswerTypeDef:
    return {
        "ChoiceId": ...,
    }


# ChoiceAnswerTypeDef definition

class ChoiceAnswerTypeDef(TypedDict):
    ChoiceId: NotRequired[str],
    Status: NotRequired[ChoiceStatusType],  # (1)
    Reason: NotRequired[ChoiceReasonType],  # (2)
    Notes: NotRequired[str],
```

1. See [:material-code-brackets: ChoiceStatusType](./literals.md#choicestatustype) 
2. See [:material-code-brackets: ChoiceReasonType](./literals.md#choicereasontype) 
## AssociateLensesInputTypeDef

```python
# AssociateLensesInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import AssociateLensesInputTypeDef


def get_value() -> AssociateLensesInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# AssociateLensesInputTypeDef definition

class AssociateLensesInputTypeDef(TypedDict):
    WorkloadId: str,
    LensAliases: Sequence[str],
```

## AssociateProfilesInputTypeDef

```python
# AssociateProfilesInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import AssociateProfilesInputTypeDef


def get_value() -> AssociateProfilesInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# AssociateProfilesInputTypeDef definition

class AssociateProfilesInputTypeDef(TypedDict):
    WorkloadId: str,
    ProfileArns: Sequence[str],
```

## BestPracticeTypeDef

```python
# BestPracticeTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import BestPracticeTypeDef


def get_value() -> BestPracticeTypeDef:
    return {
        "ChoiceId": ...,
    }


# BestPracticeTypeDef definition

class BestPracticeTypeDef(TypedDict):
    ChoiceId: NotRequired[str],
    ChoiceTitle: NotRequired[str],
```

## CheckDetailTypeDef

```python
# CheckDetailTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import CheckDetailTypeDef


def get_value() -> CheckDetailTypeDef:
    return {
        "Id": ...,
    }


# CheckDetailTypeDef definition

class CheckDetailTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    Provider: NotRequired[CheckProviderType],  # (1)
    LensArn: NotRequired[str],
    PillarId: NotRequired[str],
    QuestionId: NotRequired[str],
    ChoiceId: NotRequired[str],
    Status: NotRequired[CheckStatusType],  # (2)
    AccountId: NotRequired[str],
    FlaggedResources: NotRequired[int],
    Reason: NotRequired[CheckFailureReasonType],  # (3)
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: CheckProviderType](./literals.md#checkprovidertype) 
2. See [:material-code-brackets: CheckStatusType](./literals.md#checkstatustype) 
3. See [:material-code-brackets: CheckFailureReasonType](./literals.md#checkfailurereasontype) 
## CheckSummaryTypeDef

```python
# CheckSummaryTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import CheckSummaryTypeDef


def get_value() -> CheckSummaryTypeDef:
    return {
        "Id": ...,
    }


# CheckSummaryTypeDef definition

class CheckSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Provider: NotRequired[CheckProviderType],  # (1)
    Description: NotRequired[str],
    UpdatedAt: NotRequired[datetime],
    LensArn: NotRequired[str],
    PillarId: NotRequired[str],
    QuestionId: NotRequired[str],
    ChoiceId: NotRequired[str],
    Status: NotRequired[CheckStatusType],  # (2)
    AccountSummary: NotRequired[Dict[CheckStatusType, int]],  # (3)
```

1. See [:material-code-brackets: CheckProviderType](./literals.md#checkprovidertype) 
2. See [:material-code-brackets: CheckStatusType](./literals.md#checkstatustype) 
3. See [:material-code-brackets: CheckStatusType](./literals.md#checkstatustype) 
## ChoiceImprovementPlanTypeDef

```python
# ChoiceImprovementPlanTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ChoiceImprovementPlanTypeDef


def get_value() -> ChoiceImprovementPlanTypeDef:
    return {
        "ChoiceId": ...,
    }


# ChoiceImprovementPlanTypeDef definition

class ChoiceImprovementPlanTypeDef(TypedDict):
    ChoiceId: NotRequired[str],
    DisplayText: NotRequired[str],
    ImprovementPlanUrl: NotRequired[str],
```

## ChoiceUpdateTypeDef

```python
# ChoiceUpdateTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ChoiceUpdateTypeDef


def get_value() -> ChoiceUpdateTypeDef:
    return {
        "Status": ...,
    }


# ChoiceUpdateTypeDef definition

class ChoiceUpdateTypeDef(TypedDict):
    Status: ChoiceStatusType,  # (1)
    Reason: NotRequired[ChoiceReasonType],  # (2)
    Notes: NotRequired[str],
```

1. See [:material-code-brackets: ChoiceStatusType](./literals.md#choicestatustype) 
2. See [:material-code-brackets: ChoiceReasonType](./literals.md#choicereasontype) 
## CreateLensShareInputTypeDef

```python
# CreateLensShareInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import CreateLensShareInputTypeDef


def get_value() -> CreateLensShareInputTypeDef:
    return {
        "LensAlias": ...,
    }


# CreateLensShareInputTypeDef definition

class CreateLensShareInputTypeDef(TypedDict):
    LensAlias: str,
    SharedWith: str,
    ClientRequestToken: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ResponseMetadataTypeDef


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

## CreateLensVersionInputTypeDef

```python
# CreateLensVersionInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import CreateLensVersionInputTypeDef


def get_value() -> CreateLensVersionInputTypeDef:
    return {
        "LensAlias": ...,
    }


# CreateLensVersionInputTypeDef definition

class CreateLensVersionInputTypeDef(TypedDict):
    LensAlias: str,
    LensVersion: str,
    ClientRequestToken: str,
    IsMajorVersion: NotRequired[bool],
```

## CreateMilestoneInputTypeDef

```python
# CreateMilestoneInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import CreateMilestoneInputTypeDef


def get_value() -> CreateMilestoneInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# CreateMilestoneInputTypeDef definition

class CreateMilestoneInputTypeDef(TypedDict):
    WorkloadId: str,
    MilestoneName: str,
    ClientRequestToken: str,
```

## ProfileQuestionUpdateTypeDef

```python
# ProfileQuestionUpdateTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ProfileQuestionUpdateTypeDef


def get_value() -> ProfileQuestionUpdateTypeDef:
    return {
        "QuestionId": ...,
    }


# ProfileQuestionUpdateTypeDef definition

class ProfileQuestionUpdateTypeDef(TypedDict):
    QuestionId: NotRequired[str],
    SelectedChoiceIds: NotRequired[Sequence[str]],
```

## CreateProfileShareInputTypeDef

```python
# CreateProfileShareInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import CreateProfileShareInputTypeDef


def get_value() -> CreateProfileShareInputTypeDef:
    return {
        "ProfileArn": ...,
    }


# CreateProfileShareInputTypeDef definition

class CreateProfileShareInputTypeDef(TypedDict):
    ProfileArn: str,
    SharedWith: str,
    ClientRequestToken: str,
```

## CreateReviewTemplateInputTypeDef

```python
# CreateReviewTemplateInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import CreateReviewTemplateInputTypeDef


def get_value() -> CreateReviewTemplateInputTypeDef:
    return {
        "TemplateName": ...,
    }


# CreateReviewTemplateInputTypeDef definition

class CreateReviewTemplateInputTypeDef(TypedDict):
    TemplateName: str,
    Description: str,
    Lenses: Sequence[str],
    ClientRequestToken: str,
    Notes: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## CreateTemplateShareInputTypeDef

```python
# CreateTemplateShareInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import CreateTemplateShareInputTypeDef


def get_value() -> CreateTemplateShareInputTypeDef:
    return {
        "TemplateArn": ...,
    }


# CreateTemplateShareInputTypeDef definition

class CreateTemplateShareInputTypeDef(TypedDict):
    TemplateArn: str,
    SharedWith: str,
    ClientRequestToken: str,
```

## WorkloadJiraConfigurationInputTypeDef

```python
# WorkloadJiraConfigurationInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import WorkloadJiraConfigurationInputTypeDef


def get_value() -> WorkloadJiraConfigurationInputTypeDef:
    return {
        "IssueManagementStatus": ...,
    }


# WorkloadJiraConfigurationInputTypeDef definition

class WorkloadJiraConfigurationInputTypeDef(TypedDict):
    IssueManagementStatus: NotRequired[WorkloadIssueManagementStatusType],  # (1)
    IssueManagementType: NotRequired[IssueManagementTypeType],  # (2)
    JiraProjectKey: NotRequired[str],
```

1. See [:material-code-brackets: WorkloadIssueManagementStatusType](./literals.md#workloadissuemanagementstatustype) 
2. See [:material-code-brackets: IssueManagementTypeType](./literals.md#issuemanagementtypetype) 
## CreateWorkloadShareInputTypeDef

```python
# CreateWorkloadShareInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import CreateWorkloadShareInputTypeDef


def get_value() -> CreateWorkloadShareInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# CreateWorkloadShareInputTypeDef definition

class CreateWorkloadShareInputTypeDef(TypedDict):
    WorkloadId: str,
    SharedWith: str,
    PermissionType: PermissionTypeType,  # (1)
    ClientRequestToken: str,
```

1. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
## DeleteLensInputTypeDef

```python
# DeleteLensInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import DeleteLensInputTypeDef


def get_value() -> DeleteLensInputTypeDef:
    return {
        "LensAlias": ...,
    }


# DeleteLensInputTypeDef definition

class DeleteLensInputTypeDef(TypedDict):
    LensAlias: str,
    ClientRequestToken: str,
    LensStatus: LensStatusTypeType,  # (1)
```

1. See [:material-code-brackets: LensStatusTypeType](./literals.md#lensstatustypetype) 
## DeleteLensShareInputTypeDef

```python
# DeleteLensShareInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import DeleteLensShareInputTypeDef


def get_value() -> DeleteLensShareInputTypeDef:
    return {
        "ShareId": ...,
    }


# DeleteLensShareInputTypeDef definition

class DeleteLensShareInputTypeDef(TypedDict):
    ShareId: str,
    LensAlias: str,
    ClientRequestToken: str,
```

## DeleteProfileInputTypeDef

```python
# DeleteProfileInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import DeleteProfileInputTypeDef


def get_value() -> DeleteProfileInputTypeDef:
    return {
        "ProfileArn": ...,
    }


# DeleteProfileInputTypeDef definition

class DeleteProfileInputTypeDef(TypedDict):
    ProfileArn: str,
    ClientRequestToken: str,
```

## DeleteProfileShareInputTypeDef

```python
# DeleteProfileShareInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import DeleteProfileShareInputTypeDef


def get_value() -> DeleteProfileShareInputTypeDef:
    return {
        "ShareId": ...,
    }


# DeleteProfileShareInputTypeDef definition

class DeleteProfileShareInputTypeDef(TypedDict):
    ShareId: str,
    ProfileArn: str,
    ClientRequestToken: str,
```

## DeleteReviewTemplateInputTypeDef

```python
# DeleteReviewTemplateInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import DeleteReviewTemplateInputTypeDef


def get_value() -> DeleteReviewTemplateInputTypeDef:
    return {
        "TemplateArn": ...,
    }


# DeleteReviewTemplateInputTypeDef definition

class DeleteReviewTemplateInputTypeDef(TypedDict):
    TemplateArn: str,
    ClientRequestToken: str,
```

## DeleteTemplateShareInputTypeDef

```python
# DeleteTemplateShareInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import DeleteTemplateShareInputTypeDef


def get_value() -> DeleteTemplateShareInputTypeDef:
    return {
        "ShareId": ...,
    }


# DeleteTemplateShareInputTypeDef definition

class DeleteTemplateShareInputTypeDef(TypedDict):
    ShareId: str,
    TemplateArn: str,
    ClientRequestToken: str,
```

## DeleteWorkloadInputTypeDef

```python
# DeleteWorkloadInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import DeleteWorkloadInputTypeDef


def get_value() -> DeleteWorkloadInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# DeleteWorkloadInputTypeDef definition

class DeleteWorkloadInputTypeDef(TypedDict):
    WorkloadId: str,
    ClientRequestToken: str,
```

## DeleteWorkloadShareInputTypeDef

```python
# DeleteWorkloadShareInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import DeleteWorkloadShareInputTypeDef


def get_value() -> DeleteWorkloadShareInputTypeDef:
    return {
        "ShareId": ...,
    }


# DeleteWorkloadShareInputTypeDef definition

class DeleteWorkloadShareInputTypeDef(TypedDict):
    ShareId: str,
    WorkloadId: str,
    ClientRequestToken: str,
```

## DisassociateLensesInputTypeDef

```python
# DisassociateLensesInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import DisassociateLensesInputTypeDef


def get_value() -> DisassociateLensesInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# DisassociateLensesInputTypeDef definition

class DisassociateLensesInputTypeDef(TypedDict):
    WorkloadId: str,
    LensAliases: Sequence[str],
```

## DisassociateProfilesInputTypeDef

```python
# DisassociateProfilesInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import DisassociateProfilesInputTypeDef


def get_value() -> DisassociateProfilesInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# DisassociateProfilesInputTypeDef definition

class DisassociateProfilesInputTypeDef(TypedDict):
    WorkloadId: str,
    ProfileArns: Sequence[str],
```

## ExportLensInputTypeDef

```python
# ExportLensInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ExportLensInputTypeDef


def get_value() -> ExportLensInputTypeDef:
    return {
        "LensAlias": ...,
    }


# ExportLensInputTypeDef definition

class ExportLensInputTypeDef(TypedDict):
    LensAlias: str,
    LensVersion: NotRequired[str],
```

## GetAnswerInputTypeDef

```python
# GetAnswerInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetAnswerInputTypeDef


def get_value() -> GetAnswerInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# GetAnswerInputTypeDef definition

class GetAnswerInputTypeDef(TypedDict):
    WorkloadId: str,
    LensAlias: str,
    QuestionId: str,
    MilestoneNumber: NotRequired[int],
```

## GetConsolidatedReportInputTypeDef

```python
# GetConsolidatedReportInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetConsolidatedReportInputTypeDef


def get_value() -> GetConsolidatedReportInputTypeDef:
    return {
        "Format": ...,
    }


# GetConsolidatedReportInputTypeDef definition

class GetConsolidatedReportInputTypeDef(TypedDict):
    Format: ReportFormatType,  # (1)
    IncludeSharedResources: NotRequired[bool],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: ReportFormatType](./literals.md#reportformattype) 
## GetLensInputTypeDef

```python
# GetLensInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetLensInputTypeDef


def get_value() -> GetLensInputTypeDef:
    return {
        "LensAlias": ...,
    }


# GetLensInputTypeDef definition

class GetLensInputTypeDef(TypedDict):
    LensAlias: str,
    LensVersion: NotRequired[str],
```

## LensTypeDef

```python
# LensTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import LensTypeDef


def get_value() -> LensTypeDef:
    return {
        "LensArn": ...,
    }


# LensTypeDef definition

class LensTypeDef(TypedDict):
    LensArn: NotRequired[str],
    LensVersion: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    Owner: NotRequired[str],
    ShareInvitationId: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

## GetLensReviewInputTypeDef

```python
# GetLensReviewInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetLensReviewInputTypeDef


def get_value() -> GetLensReviewInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# GetLensReviewInputTypeDef definition

class GetLensReviewInputTypeDef(TypedDict):
    WorkloadId: str,
    LensAlias: str,
    MilestoneNumber: NotRequired[int],
```

## GetLensReviewReportInputTypeDef

```python
# GetLensReviewReportInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetLensReviewReportInputTypeDef


def get_value() -> GetLensReviewReportInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# GetLensReviewReportInputTypeDef definition

class GetLensReviewReportInputTypeDef(TypedDict):
    WorkloadId: str,
    LensAlias: str,
    MilestoneNumber: NotRequired[int],
```

## LensReviewReportTypeDef

```python
# LensReviewReportTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import LensReviewReportTypeDef


def get_value() -> LensReviewReportTypeDef:
    return {
        "LensAlias": ...,
    }


# LensReviewReportTypeDef definition

class LensReviewReportTypeDef(TypedDict):
    LensAlias: NotRequired[str],
    LensArn: NotRequired[str],
    Base64String: NotRequired[str],
```

## GetLensVersionDifferenceInputTypeDef

```python
# GetLensVersionDifferenceInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetLensVersionDifferenceInputTypeDef


def get_value() -> GetLensVersionDifferenceInputTypeDef:
    return {
        "LensAlias": ...,
    }


# GetLensVersionDifferenceInputTypeDef definition

class GetLensVersionDifferenceInputTypeDef(TypedDict):
    LensAlias: str,
    BaseLensVersion: NotRequired[str],
    TargetLensVersion: NotRequired[str],
```

## GetMilestoneInputTypeDef

```python
# GetMilestoneInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetMilestoneInputTypeDef


def get_value() -> GetMilestoneInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# GetMilestoneInputTypeDef definition

class GetMilestoneInputTypeDef(TypedDict):
    WorkloadId: str,
    MilestoneNumber: int,
```

## GetProfileInputTypeDef

```python
# GetProfileInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetProfileInputTypeDef


def get_value() -> GetProfileInputTypeDef:
    return {
        "ProfileArn": ...,
    }


# GetProfileInputTypeDef definition

class GetProfileInputTypeDef(TypedDict):
    ProfileArn: str,
    ProfileVersion: NotRequired[str],
```

## GetReviewTemplateAnswerInputTypeDef

```python
# GetReviewTemplateAnswerInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetReviewTemplateAnswerInputTypeDef


def get_value() -> GetReviewTemplateAnswerInputTypeDef:
    return {
        "TemplateArn": ...,
    }


# GetReviewTemplateAnswerInputTypeDef definition

class GetReviewTemplateAnswerInputTypeDef(TypedDict):
    TemplateArn: str,
    LensAlias: str,
    QuestionId: str,
```

## GetReviewTemplateInputTypeDef

```python
# GetReviewTemplateInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetReviewTemplateInputTypeDef


def get_value() -> GetReviewTemplateInputTypeDef:
    return {
        "TemplateArn": ...,
    }


# GetReviewTemplateInputTypeDef definition

class GetReviewTemplateInputTypeDef(TypedDict):
    TemplateArn: str,
```

## GetReviewTemplateLensReviewInputTypeDef

```python
# GetReviewTemplateLensReviewInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetReviewTemplateLensReviewInputTypeDef


def get_value() -> GetReviewTemplateLensReviewInputTypeDef:
    return {
        "TemplateArn": ...,
    }


# GetReviewTemplateLensReviewInputTypeDef definition

class GetReviewTemplateLensReviewInputTypeDef(TypedDict):
    TemplateArn: str,
    LensAlias: str,
```

## ReviewTemplateTypeDef

```python
# ReviewTemplateTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ReviewTemplateTypeDef


def get_value() -> ReviewTemplateTypeDef:
    return {
        "Description": ...,
    }


# ReviewTemplateTypeDef definition

class ReviewTemplateTypeDef(TypedDict):
    Description: NotRequired[str],
    Lenses: NotRequired[List[str]],
    Notes: NotRequired[str],
    QuestionCounts: NotRequired[Dict[QuestionType, int]],  # (1)
    Owner: NotRequired[str],
    UpdatedAt: NotRequired[datetime],
    TemplateArn: NotRequired[str],
    TemplateName: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
    UpdateStatus: NotRequired[ReviewTemplateUpdateStatusType],  # (2)
    ShareInvitationId: NotRequired[str],
```

1. See [:material-code-brackets: QuestionType](./literals.md#questiontype) 
2. See [:material-code-brackets: ReviewTemplateUpdateStatusType](./literals.md#reviewtemplateupdatestatustype) 
## GetWorkloadInputTypeDef

```python
# GetWorkloadInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetWorkloadInputTypeDef


def get_value() -> GetWorkloadInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# GetWorkloadInputTypeDef definition

class GetWorkloadInputTypeDef(TypedDict):
    WorkloadId: str,
```

## ImportLensInputTypeDef

```python
# ImportLensInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ImportLensInputTypeDef


def get_value() -> ImportLensInputTypeDef:
    return {
        "JSONString": ...,
    }


# ImportLensInputTypeDef definition

class ImportLensInputTypeDef(TypedDict):
    JSONString: str,
    ClientRequestToken: str,
    LensAlias: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## SelectedPillarOutputTypeDef

```python
# SelectedPillarOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import SelectedPillarOutputTypeDef


def get_value() -> SelectedPillarOutputTypeDef:
    return {
        "PillarId": ...,
    }


# SelectedPillarOutputTypeDef definition

class SelectedPillarOutputTypeDef(TypedDict):
    PillarId: NotRequired[str],
    SelectedQuestionIds: NotRequired[List[str]],
```

## SelectedPillarTypeDef

```python
# SelectedPillarTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import SelectedPillarTypeDef


def get_value() -> SelectedPillarTypeDef:
    return {
        "PillarId": ...,
    }


# SelectedPillarTypeDef definition

class SelectedPillarTypeDef(TypedDict):
    PillarId: NotRequired[str],
    SelectedQuestionIds: NotRequired[Sequence[str]],
```

## WorkloadProfileTypeDef

```python
# WorkloadProfileTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import WorkloadProfileTypeDef


def get_value() -> WorkloadProfileTypeDef:
    return {
        "ProfileArn": ...,
    }


# WorkloadProfileTypeDef definition

class WorkloadProfileTypeDef(TypedDict):
    ProfileArn: NotRequired[str],
    ProfileVersion: NotRequired[str],
```

## PillarReviewSummaryTypeDef

```python
# PillarReviewSummaryTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import PillarReviewSummaryTypeDef


def get_value() -> PillarReviewSummaryTypeDef:
    return {
        "PillarId": ...,
    }


# PillarReviewSummaryTypeDef definition

class PillarReviewSummaryTypeDef(TypedDict):
    PillarId: NotRequired[str],
    PillarName: NotRequired[str],
    Notes: NotRequired[str],
    RiskCounts: NotRequired[Dict[RiskType, int]],  # (1)
    PrioritizedRiskCounts: NotRequired[Dict[RiskType, int]],  # (1)
```

1. See [:material-code-brackets: RiskType](./literals.md#risktype) 
2. See [:material-code-brackets: RiskType](./literals.md#risktype) 
## LensShareSummaryTypeDef

```python
# LensShareSummaryTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import LensShareSummaryTypeDef


def get_value() -> LensShareSummaryTypeDef:
    return {
        "ShareId": ...,
    }


# LensShareSummaryTypeDef definition

class LensShareSummaryTypeDef(TypedDict):
    ShareId: NotRequired[str],
    SharedWith: NotRequired[str],
    Status: NotRequired[ShareStatusType],  # (1)
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
## LensSummaryTypeDef

```python
# LensSummaryTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import LensSummaryTypeDef


def get_value() -> LensSummaryTypeDef:
    return {
        "LensArn": ...,
    }


# LensSummaryTypeDef definition

class LensSummaryTypeDef(TypedDict):
    LensArn: NotRequired[str],
    LensAlias: NotRequired[str],
    LensName: NotRequired[str],
    LensType: NotRequired[LensTypeType],  # (1)
    Description: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    UpdatedAt: NotRequired[datetime],
    LensVersion: NotRequired[str],
    Owner: NotRequired[str],
    LensStatus: NotRequired[LensStatusType],  # (2)
```

1. See [:material-code-brackets: LensTypeType](./literals.md#lenstypetype) 
2. See [:material-code-brackets: LensStatusType](./literals.md#lensstatustype) 
## LensUpgradeSummaryTypeDef

```python
# LensUpgradeSummaryTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import LensUpgradeSummaryTypeDef


def get_value() -> LensUpgradeSummaryTypeDef:
    return {
        "WorkloadId": ...,
    }


# LensUpgradeSummaryTypeDef definition

class LensUpgradeSummaryTypeDef(TypedDict):
    WorkloadId: NotRequired[str],
    WorkloadName: NotRequired[str],
    LensAlias: NotRequired[str],
    LensArn: NotRequired[str],
    CurrentLensVersion: NotRequired[str],
    LatestLensVersion: NotRequired[str],
    ResourceArn: NotRequired[str],
    ResourceName: NotRequired[str],
```

## ListAnswersInputTypeDef

```python
# ListAnswersInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListAnswersInputTypeDef


def get_value() -> ListAnswersInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# ListAnswersInputTypeDef definition

class ListAnswersInputTypeDef(TypedDict):
    WorkloadId: str,
    LensAlias: str,
    PillarId: NotRequired[str],
    MilestoneNumber: NotRequired[int],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    QuestionPriority: NotRequired[QuestionPriorityType],  # (1)
```

1. See [:material-code-brackets: QuestionPriorityType](./literals.md#questionprioritytype) 
## ListCheckDetailsInputTypeDef

```python
# ListCheckDetailsInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListCheckDetailsInputTypeDef


def get_value() -> ListCheckDetailsInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# ListCheckDetailsInputTypeDef definition

class ListCheckDetailsInputTypeDef(TypedDict):
    WorkloadId: str,
    LensArn: str,
    PillarId: str,
    QuestionId: str,
    ChoiceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListCheckSummariesInputTypeDef

```python
# ListCheckSummariesInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListCheckSummariesInputTypeDef


def get_value() -> ListCheckSummariesInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# ListCheckSummariesInputTypeDef definition

class ListCheckSummariesInputTypeDef(TypedDict):
    WorkloadId: str,
    LensArn: str,
    PillarId: str,
    QuestionId: str,
    ChoiceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListLensReviewImprovementsInputTypeDef

```python
# ListLensReviewImprovementsInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListLensReviewImprovementsInputTypeDef


def get_value() -> ListLensReviewImprovementsInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# ListLensReviewImprovementsInputTypeDef definition

class ListLensReviewImprovementsInputTypeDef(TypedDict):
    WorkloadId: str,
    LensAlias: str,
    PillarId: NotRequired[str],
    MilestoneNumber: NotRequired[int],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    QuestionPriority: NotRequired[QuestionPriorityType],  # (1)
```

1. See [:material-code-brackets: QuestionPriorityType](./literals.md#questionprioritytype) 
## ListLensReviewsInputTypeDef

```python
# ListLensReviewsInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListLensReviewsInputTypeDef


def get_value() -> ListLensReviewsInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# ListLensReviewsInputTypeDef definition

class ListLensReviewsInputTypeDef(TypedDict):
    WorkloadId: str,
    MilestoneNumber: NotRequired[int],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListLensSharesInputTypeDef

```python
# ListLensSharesInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListLensSharesInputTypeDef


def get_value() -> ListLensSharesInputTypeDef:
    return {
        "LensAlias": ...,
    }


# ListLensSharesInputTypeDef definition

class ListLensSharesInputTypeDef(TypedDict):
    LensAlias: str,
    SharedWithPrefix: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Status: NotRequired[ShareStatusType],  # (1)
```

1. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
## ListLensesInputTypeDef

```python
# ListLensesInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListLensesInputTypeDef


def get_value() -> ListLensesInputTypeDef:
    return {
        "NextToken": ...,
    }


# ListLensesInputTypeDef definition

class ListLensesInputTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    LensType: NotRequired[LensTypeType],  # (1)
    LensStatus: NotRequired[LensStatusTypeType],  # (2)
    LensName: NotRequired[str],
```

1. See [:material-code-brackets: LensTypeType](./literals.md#lenstypetype) 
2. See [:material-code-brackets: LensStatusTypeType](./literals.md#lensstatustypetype) 
## ListMilestonesInputTypeDef

```python
# ListMilestonesInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListMilestonesInputTypeDef


def get_value() -> ListMilestonesInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# ListMilestonesInputTypeDef definition

class ListMilestonesInputTypeDef(TypedDict):
    WorkloadId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListNotificationsInputTypeDef

```python
# ListNotificationsInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListNotificationsInputTypeDef


def get_value() -> ListNotificationsInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# ListNotificationsInputTypeDef definition

class ListNotificationsInputTypeDef(TypedDict):
    WorkloadId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ResourceArn: NotRequired[str],
```

## ListProfileNotificationsInputTypeDef

```python
# ListProfileNotificationsInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListProfileNotificationsInputTypeDef


def get_value() -> ListProfileNotificationsInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# ListProfileNotificationsInputTypeDef definition

class ListProfileNotificationsInputTypeDef(TypedDict):
    WorkloadId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ProfileNotificationSummaryTypeDef

```python
# ProfileNotificationSummaryTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ProfileNotificationSummaryTypeDef


def get_value() -> ProfileNotificationSummaryTypeDef:
    return {
        "CurrentProfileVersion": ...,
    }


# ProfileNotificationSummaryTypeDef definition

class ProfileNotificationSummaryTypeDef(TypedDict):
    CurrentProfileVersion: NotRequired[str],
    LatestProfileVersion: NotRequired[str],
    Type: NotRequired[ProfileNotificationTypeType],  # (1)
    ProfileArn: NotRequired[str],
    ProfileName: NotRequired[str],
    WorkloadId: NotRequired[str],
    WorkloadName: NotRequired[str],
```

1. See [:material-code-brackets: ProfileNotificationTypeType](./literals.md#profilenotificationtypetype) 
## ListProfileSharesInputTypeDef

```python
# ListProfileSharesInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListProfileSharesInputTypeDef


def get_value() -> ListProfileSharesInputTypeDef:
    return {
        "ProfileArn": ...,
    }


# ListProfileSharesInputTypeDef definition

class ListProfileSharesInputTypeDef(TypedDict):
    ProfileArn: str,
    SharedWithPrefix: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Status: NotRequired[ShareStatusType],  # (1)
```

1. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
## ProfileShareSummaryTypeDef

```python
# ProfileShareSummaryTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ProfileShareSummaryTypeDef


def get_value() -> ProfileShareSummaryTypeDef:
    return {
        "ShareId": ...,
    }


# ProfileShareSummaryTypeDef definition

class ProfileShareSummaryTypeDef(TypedDict):
    ShareId: NotRequired[str],
    SharedWith: NotRequired[str],
    Status: NotRequired[ShareStatusType],  # (1)
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
## ListProfilesInputTypeDef

```python
# ListProfilesInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListProfilesInputTypeDef


def get_value() -> ListProfilesInputTypeDef:
    return {
        "ProfileNamePrefix": ...,
    }


# ListProfilesInputTypeDef definition

class ListProfilesInputTypeDef(TypedDict):
    ProfileNamePrefix: NotRequired[str],
    ProfileOwnerType: NotRequired[ProfileOwnerTypeType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: ProfileOwnerTypeType](./literals.md#profileownertypetype) 
## ProfileSummaryTypeDef

```python
# ProfileSummaryTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ProfileSummaryTypeDef


def get_value() -> ProfileSummaryTypeDef:
    return {
        "ProfileArn": ...,
    }


# ProfileSummaryTypeDef definition

class ProfileSummaryTypeDef(TypedDict):
    ProfileArn: NotRequired[str],
    ProfileVersion: NotRequired[str],
    ProfileName: NotRequired[str],
    ProfileDescription: NotRequired[str],
    Owner: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    UpdatedAt: NotRequired[datetime],
```

## ListReviewTemplateAnswersInputTypeDef

```python
# ListReviewTemplateAnswersInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListReviewTemplateAnswersInputTypeDef


def get_value() -> ListReviewTemplateAnswersInputTypeDef:
    return {
        "TemplateArn": ...,
    }


# ListReviewTemplateAnswersInputTypeDef definition

class ListReviewTemplateAnswersInputTypeDef(TypedDict):
    TemplateArn: str,
    LensAlias: str,
    PillarId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListReviewTemplatesInputTypeDef

```python
# ListReviewTemplatesInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListReviewTemplatesInputTypeDef


def get_value() -> ListReviewTemplatesInputTypeDef:
    return {
        "NextToken": ...,
    }


# ListReviewTemplatesInputTypeDef definition

class ListReviewTemplatesInputTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ReviewTemplateSummaryTypeDef

```python
# ReviewTemplateSummaryTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ReviewTemplateSummaryTypeDef


def get_value() -> ReviewTemplateSummaryTypeDef:
    return {
        "Description": ...,
    }


# ReviewTemplateSummaryTypeDef definition

class ReviewTemplateSummaryTypeDef(TypedDict):
    Description: NotRequired[str],
    Lenses: NotRequired[List[str]],
    Owner: NotRequired[str],
    UpdatedAt: NotRequired[datetime],
    TemplateArn: NotRequired[str],
    TemplateName: NotRequired[str],
    UpdateStatus: NotRequired[ReviewTemplateUpdateStatusType],  # (1)
```

1. See [:material-code-brackets: ReviewTemplateUpdateStatusType](./literals.md#reviewtemplateupdatestatustype) 
## ListShareInvitationsInputTypeDef

```python
# ListShareInvitationsInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListShareInvitationsInputTypeDef


def get_value() -> ListShareInvitationsInputTypeDef:
    return {
        "WorkloadNamePrefix": ...,
    }


# ListShareInvitationsInputTypeDef definition

class ListShareInvitationsInputTypeDef(TypedDict):
    WorkloadNamePrefix: NotRequired[str],
    LensNamePrefix: NotRequired[str],
    ShareResourceType: NotRequired[ShareResourceTypeType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ProfileNamePrefix: NotRequired[str],
    TemplateNamePrefix: NotRequired[str],
```

1. See [:material-code-brackets: ShareResourceTypeType](./literals.md#shareresourcetypetype) 
## ShareInvitationSummaryTypeDef

```python
# ShareInvitationSummaryTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ShareInvitationSummaryTypeDef


def get_value() -> ShareInvitationSummaryTypeDef:
    return {
        "ShareInvitationId": ...,
    }


# ShareInvitationSummaryTypeDef definition

class ShareInvitationSummaryTypeDef(TypedDict):
    ShareInvitationId: NotRequired[str],
    SharedBy: NotRequired[str],
    SharedWith: NotRequired[str],
    PermissionType: NotRequired[PermissionTypeType],  # (1)
    ShareResourceType: NotRequired[ShareResourceTypeType],  # (2)
    WorkloadName: NotRequired[str],
    WorkloadId: NotRequired[str],
    LensName: NotRequired[str],
    LensArn: NotRequired[str],
    ProfileName: NotRequired[str],
    ProfileArn: NotRequired[str],
    TemplateName: NotRequired[str],
    TemplateArn: NotRequired[str],
```

1. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
2. See [:material-code-brackets: ShareResourceTypeType](./literals.md#shareresourcetypetype) 
## ListTagsForResourceInputTypeDef

```python
# ListTagsForResourceInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListTagsForResourceInputTypeDef


def get_value() -> ListTagsForResourceInputTypeDef:
    return {
        "WorkloadArn": ...,
    }


# ListTagsForResourceInputTypeDef definition

class ListTagsForResourceInputTypeDef(TypedDict):
    WorkloadArn: str,
```

## ListTemplateSharesInputTypeDef

```python
# ListTemplateSharesInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListTemplateSharesInputTypeDef


def get_value() -> ListTemplateSharesInputTypeDef:
    return {
        "TemplateArn": ...,
    }


# ListTemplateSharesInputTypeDef definition

class ListTemplateSharesInputTypeDef(TypedDict):
    TemplateArn: str,
    SharedWithPrefix: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Status: NotRequired[ShareStatusType],  # (1)
```

1. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
## TemplateShareSummaryTypeDef

```python
# TemplateShareSummaryTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import TemplateShareSummaryTypeDef


def get_value() -> TemplateShareSummaryTypeDef:
    return {
        "ShareId": ...,
    }


# TemplateShareSummaryTypeDef definition

class TemplateShareSummaryTypeDef(TypedDict):
    ShareId: NotRequired[str],
    SharedWith: NotRequired[str],
    Status: NotRequired[ShareStatusType],  # (1)
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
## ListWorkloadSharesInputTypeDef

```python
# ListWorkloadSharesInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListWorkloadSharesInputTypeDef


def get_value() -> ListWorkloadSharesInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# ListWorkloadSharesInputTypeDef definition

class ListWorkloadSharesInputTypeDef(TypedDict):
    WorkloadId: str,
    SharedWithPrefix: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Status: NotRequired[ShareStatusType],  # (1)
```

1. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
## WorkloadShareSummaryTypeDef

```python
# WorkloadShareSummaryTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import WorkloadShareSummaryTypeDef


def get_value() -> WorkloadShareSummaryTypeDef:
    return {
        "ShareId": ...,
    }


# WorkloadShareSummaryTypeDef definition

class WorkloadShareSummaryTypeDef(TypedDict):
    ShareId: NotRequired[str],
    SharedWith: NotRequired[str],
    PermissionType: NotRequired[PermissionTypeType],  # (1)
    Status: NotRequired[ShareStatusType],  # (2)
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
2. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
## ListWorkloadsInputTypeDef

```python
# ListWorkloadsInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListWorkloadsInputTypeDef


def get_value() -> ListWorkloadsInputTypeDef:
    return {
        "WorkloadNamePrefix": ...,
    }


# ListWorkloadsInputTypeDef definition

class ListWorkloadsInputTypeDef(TypedDict):
    WorkloadNamePrefix: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## QuestionDifferenceTypeDef

```python
# QuestionDifferenceTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import QuestionDifferenceTypeDef


def get_value() -> QuestionDifferenceTypeDef:
    return {
        "QuestionId": ...,
    }


# QuestionDifferenceTypeDef definition

class QuestionDifferenceTypeDef(TypedDict):
    QuestionId: NotRequired[str],
    QuestionTitle: NotRequired[str],
    DifferenceStatus: NotRequired[DifferenceStatusType],  # (1)
```

1. See [:material-code-brackets: DifferenceStatusType](./literals.md#differencestatustype) 
## ProfileChoiceTypeDef

```python
# ProfileChoiceTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ProfileChoiceTypeDef


def get_value() -> ProfileChoiceTypeDef:
    return {
        "ChoiceId": ...,
    }


# ProfileChoiceTypeDef definition

class ProfileChoiceTypeDef(TypedDict):
    ChoiceId: NotRequired[str],
    ChoiceTitle: NotRequired[str],
    ChoiceDescription: NotRequired[str],
```

## ProfileTemplateChoiceTypeDef

```python
# ProfileTemplateChoiceTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ProfileTemplateChoiceTypeDef


def get_value() -> ProfileTemplateChoiceTypeDef:
    return {
        "ChoiceId": ...,
    }


# ProfileTemplateChoiceTypeDef definition

class ProfileTemplateChoiceTypeDef(TypedDict):
    ChoiceId: NotRequired[str],
    ChoiceTitle: NotRequired[str],
    ChoiceDescription: NotRequired[str],
```

## ReviewTemplatePillarReviewSummaryTypeDef

```python
# ReviewTemplatePillarReviewSummaryTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ReviewTemplatePillarReviewSummaryTypeDef


def get_value() -> ReviewTemplatePillarReviewSummaryTypeDef:
    return {
        "PillarId": ...,
    }


# ReviewTemplatePillarReviewSummaryTypeDef definition

class ReviewTemplatePillarReviewSummaryTypeDef(TypedDict):
    PillarId: NotRequired[str],
    PillarName: NotRequired[str],
    Notes: NotRequired[str],
    QuestionCounts: NotRequired[Dict[QuestionType, int]],  # (1)
```

1. See [:material-code-brackets: QuestionType](./literals.md#questiontype) 
## ShareInvitationTypeDef

```python
# ShareInvitationTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ShareInvitationTypeDef


def get_value() -> ShareInvitationTypeDef:
    return {
        "ShareInvitationId": ...,
    }


# ShareInvitationTypeDef definition

class ShareInvitationTypeDef(TypedDict):
    ShareInvitationId: NotRequired[str],
    ShareResourceType: NotRequired[ShareResourceTypeType],  # (1)
    WorkloadId: NotRequired[str],
    LensAlias: NotRequired[str],
    LensArn: NotRequired[str],
    ProfileArn: NotRequired[str],
    TemplateArn: NotRequired[str],
```

1. See [:material-code-brackets: ShareResourceTypeType](./literals.md#shareresourcetypetype) 
## TagResourceInputTypeDef

```python
# TagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import TagResourceInputTypeDef


def get_value() -> TagResourceInputTypeDef:
    return {
        "WorkloadArn": ...,
    }


# TagResourceInputTypeDef definition

class TagResourceInputTypeDef(TypedDict):
    WorkloadArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceInputTypeDef

```python
# UntagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UntagResourceInputTypeDef


def get_value() -> UntagResourceInputTypeDef:
    return {
        "WorkloadArn": ...,
    }


# UntagResourceInputTypeDef definition

class UntagResourceInputTypeDef(TypedDict):
    WorkloadArn: str,
    TagKeys: Sequence[str],
```

## UpdateIntegrationInputTypeDef

```python
# UpdateIntegrationInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpdateIntegrationInputTypeDef


def get_value() -> UpdateIntegrationInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# UpdateIntegrationInputTypeDef definition

class UpdateIntegrationInputTypeDef(TypedDict):
    WorkloadId: str,
    ClientRequestToken: str,
    IntegratingService: IntegratingServiceType,  # (1)
```

1. See [:material-code-brackets: IntegratingServiceType](./literals.md#integratingservicetype) 
## UpdateReviewTemplateInputTypeDef

```python
# UpdateReviewTemplateInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpdateReviewTemplateInputTypeDef


def get_value() -> UpdateReviewTemplateInputTypeDef:
    return {
        "TemplateArn": ...,
    }


# UpdateReviewTemplateInputTypeDef definition

class UpdateReviewTemplateInputTypeDef(TypedDict):
    TemplateArn: str,
    TemplateName: NotRequired[str],
    Description: NotRequired[str],
    Notes: NotRequired[str],
    LensesToAssociate: NotRequired[Sequence[str]],
    LensesToDisassociate: NotRequired[Sequence[str]],
```

## UpdateReviewTemplateLensReviewInputTypeDef

```python
# UpdateReviewTemplateLensReviewInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpdateReviewTemplateLensReviewInputTypeDef


def get_value() -> UpdateReviewTemplateLensReviewInputTypeDef:
    return {
        "TemplateArn": ...,
    }


# UpdateReviewTemplateLensReviewInputTypeDef definition

class UpdateReviewTemplateLensReviewInputTypeDef(TypedDict):
    TemplateArn: str,
    LensAlias: str,
    LensNotes: NotRequired[str],
    PillarNotes: NotRequired[Mapping[str, str]],
```

## UpdateShareInvitationInputTypeDef

```python
# UpdateShareInvitationInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpdateShareInvitationInputTypeDef


def get_value() -> UpdateShareInvitationInputTypeDef:
    return {
        "ShareInvitationId": ...,
    }


# UpdateShareInvitationInputTypeDef definition

class UpdateShareInvitationInputTypeDef(TypedDict):
    ShareInvitationId: str,
    ShareInvitationAction: ShareInvitationActionType,  # (1)
```

1. See [:material-code-brackets: ShareInvitationActionType](./literals.md#shareinvitationactiontype) 
## UpdateWorkloadShareInputTypeDef

```python
# UpdateWorkloadShareInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpdateWorkloadShareInputTypeDef


def get_value() -> UpdateWorkloadShareInputTypeDef:
    return {
        "ShareId": ...,
    }


# UpdateWorkloadShareInputTypeDef definition

class UpdateWorkloadShareInputTypeDef(TypedDict):
    ShareId: str,
    WorkloadId: str,
    PermissionType: PermissionTypeType,  # (1)
```

1. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
## WorkloadShareTypeDef

```python
# WorkloadShareTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import WorkloadShareTypeDef


def get_value() -> WorkloadShareTypeDef:
    return {
        "ShareId": ...,
    }


# WorkloadShareTypeDef definition

class WorkloadShareTypeDef(TypedDict):
    ShareId: NotRequired[str],
    SharedBy: NotRequired[str],
    SharedWith: NotRequired[str],
    PermissionType: NotRequired[PermissionTypeType],  # (1)
    Status: NotRequired[ShareStatusType],  # (2)
    WorkloadName: NotRequired[str],
    WorkloadId: NotRequired[str],
```

1. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
2. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
## UpgradeLensReviewInputTypeDef

```python
# UpgradeLensReviewInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpgradeLensReviewInputTypeDef


def get_value() -> UpgradeLensReviewInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# UpgradeLensReviewInputTypeDef definition

class UpgradeLensReviewInputTypeDef(TypedDict):
    WorkloadId: str,
    LensAlias: str,
    MilestoneName: str,
    ClientRequestToken: NotRequired[str],
```

## UpgradeProfileVersionInputTypeDef

```python
# UpgradeProfileVersionInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpgradeProfileVersionInputTypeDef


def get_value() -> UpgradeProfileVersionInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# UpgradeProfileVersionInputTypeDef definition

class UpgradeProfileVersionInputTypeDef(TypedDict):
    WorkloadId: str,
    ProfileArn: str,
    MilestoneName: NotRequired[str],
    ClientRequestToken: NotRequired[str],
```

## UpgradeReviewTemplateLensReviewInputTypeDef

```python
# UpgradeReviewTemplateLensReviewInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpgradeReviewTemplateLensReviewInputTypeDef


def get_value() -> UpgradeReviewTemplateLensReviewInputTypeDef:
    return {
        "TemplateArn": ...,
    }


# UpgradeReviewTemplateLensReviewInputTypeDef definition

class UpgradeReviewTemplateLensReviewInputTypeDef(TypedDict):
    TemplateArn: str,
    LensAlias: str,
    ClientRequestToken: NotRequired[str],
```

## WorkloadDiscoveryConfigOutputTypeDef

```python
# WorkloadDiscoveryConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import WorkloadDiscoveryConfigOutputTypeDef


def get_value() -> WorkloadDiscoveryConfigOutputTypeDef:
    return {
        "TrustedAdvisorIntegrationStatus": ...,
    }


# WorkloadDiscoveryConfigOutputTypeDef definition

class WorkloadDiscoveryConfigOutputTypeDef(TypedDict):
    TrustedAdvisorIntegrationStatus: NotRequired[TrustedAdvisorIntegrationStatusType],  # (1)
    WorkloadResourceDefinition: NotRequired[List[DefinitionTypeType]],  # (2)
```

1. See [:material-code-brackets: TrustedAdvisorIntegrationStatusType](./literals.md#trustedadvisorintegrationstatustype) 
2. See [:material-code-brackets: DefinitionTypeType](./literals.md#definitiontypetype) 
## WorkloadDiscoveryConfigTypeDef

```python
# WorkloadDiscoveryConfigTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import WorkloadDiscoveryConfigTypeDef


def get_value() -> WorkloadDiscoveryConfigTypeDef:
    return {
        "TrustedAdvisorIntegrationStatus": ...,
    }


# WorkloadDiscoveryConfigTypeDef definition

class WorkloadDiscoveryConfigTypeDef(TypedDict):
    TrustedAdvisorIntegrationStatus: NotRequired[TrustedAdvisorIntegrationStatusType],  # (1)
    WorkloadResourceDefinition: NotRequired[Sequence[DefinitionTypeType]],  # (2)
```

1. See [:material-code-brackets: TrustedAdvisorIntegrationStatusType](./literals.md#trustedadvisorintegrationstatustype) 
2. See [:material-code-brackets: DefinitionTypeType](./literals.md#definitiontypetype) 
## WorkloadJiraConfigurationOutputTypeDef

```python
# WorkloadJiraConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import WorkloadJiraConfigurationOutputTypeDef


def get_value() -> WorkloadJiraConfigurationOutputTypeDef:
    return {
        "IssueManagementStatus": ...,
    }


# WorkloadJiraConfigurationOutputTypeDef definition

class WorkloadJiraConfigurationOutputTypeDef(TypedDict):
    IssueManagementStatus: NotRequired[WorkloadIssueManagementStatusType],  # (1)
    IssueManagementType: NotRequired[IssueManagementTypeType],  # (2)
    JiraProjectKey: NotRequired[str],
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: WorkloadIssueManagementStatusType](./literals.md#workloadissuemanagementstatustype) 
2. See [:material-code-brackets: IssueManagementTypeType](./literals.md#issuemanagementtypetype) 
## UpdateGlobalSettingsInputTypeDef

```python
# UpdateGlobalSettingsInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpdateGlobalSettingsInputTypeDef


def get_value() -> UpdateGlobalSettingsInputTypeDef:
    return {
        "OrganizationSharingStatus": ...,
    }


# UpdateGlobalSettingsInputTypeDef definition

class UpdateGlobalSettingsInputTypeDef(TypedDict):
    OrganizationSharingStatus: NotRequired[OrganizationSharingStatusType],  # (1)
    DiscoveryIntegrationStatus: NotRequired[DiscoveryIntegrationStatusType],  # (2)
    JiraConfiguration: NotRequired[AccountJiraConfigurationInputTypeDef],  # (3)
```

1. See [:material-code-brackets: OrganizationSharingStatusType](./literals.md#organizationsharingstatustype) 
2. See [:material-code-brackets: DiscoveryIntegrationStatusType](./literals.md#discoveryintegrationstatustype) 
3. See [:material-code-braces: AccountJiraConfigurationInputTypeDef](./type_defs.md#accountjiraconfigurationinputtypedef) 
## AdditionalResourcesTypeDef

```python
# AdditionalResourcesTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import AdditionalResourcesTypeDef


def get_value() -> AdditionalResourcesTypeDef:
    return {
        "Type": ...,
    }


# AdditionalResourcesTypeDef definition

class AdditionalResourcesTypeDef(TypedDict):
    Type: NotRequired[AdditionalResourceTypeType],  # (1)
    Content: NotRequired[List[ChoiceContentTypeDef]],  # (2)
```

1. See [:material-code-brackets: AdditionalResourceTypeType](./literals.md#additionalresourcetypetype) 
2. See [:material-code-braces: ChoiceContentTypeDef](./type_defs.md#choicecontenttypedef) 
## QuestionMetricTypeDef

```python
# QuestionMetricTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import QuestionMetricTypeDef


def get_value() -> QuestionMetricTypeDef:
    return {
        "QuestionId": ...,
    }


# QuestionMetricTypeDef definition

class QuestionMetricTypeDef(TypedDict):
    QuestionId: NotRequired[str],
    Risk: NotRequired[RiskType],  # (1)
    BestPractices: NotRequired[List[BestPracticeTypeDef]],  # (2)
```

1. See [:material-code-brackets: RiskType](./literals.md#risktype) 
2. See [:material-code-braces: BestPracticeTypeDef](./type_defs.md#bestpracticetypedef) 
## ImprovementSummaryTypeDef

```python
# ImprovementSummaryTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ImprovementSummaryTypeDef


def get_value() -> ImprovementSummaryTypeDef:
    return {
        "QuestionId": ...,
    }


# ImprovementSummaryTypeDef definition

class ImprovementSummaryTypeDef(TypedDict):
    QuestionId: NotRequired[str],
    PillarId: NotRequired[str],
    QuestionTitle: NotRequired[str],
    Risk: NotRequired[RiskType],  # (1)
    ImprovementPlanUrl: NotRequired[str],
    ImprovementPlans: NotRequired[List[ChoiceImprovementPlanTypeDef]],  # (2)
    JiraConfiguration: NotRequired[JiraConfigurationTypeDef],  # (3)
```

1. See [:material-code-brackets: RiskType](./literals.md#risktype) 
2. See [:material-code-braces: ChoiceImprovementPlanTypeDef](./type_defs.md#choiceimprovementplantypedef) 
3. See [:material-code-braces: JiraConfigurationTypeDef](./type_defs.md#jiraconfigurationtypedef) 
## UpdateAnswerInputTypeDef

```python
# UpdateAnswerInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpdateAnswerInputTypeDef


def get_value() -> UpdateAnswerInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# UpdateAnswerInputTypeDef definition

class UpdateAnswerInputTypeDef(TypedDict):
    WorkloadId: str,
    LensAlias: str,
    QuestionId: str,
    SelectedChoices: NotRequired[Sequence[str]],
    ChoiceUpdates: NotRequired[Mapping[str, ChoiceUpdateTypeDef]],  # (1)
    Notes: NotRequired[str],
    IsApplicable: NotRequired[bool],
    Reason: NotRequired[AnswerReasonType],  # (2)
```

1. See [:material-code-braces: ChoiceUpdateTypeDef](./type_defs.md#choiceupdatetypedef) 
2. See [:material-code-brackets: AnswerReasonType](./literals.md#answerreasontype) 
## UpdateReviewTemplateAnswerInputTypeDef

```python
# UpdateReviewTemplateAnswerInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpdateReviewTemplateAnswerInputTypeDef


def get_value() -> UpdateReviewTemplateAnswerInputTypeDef:
    return {
        "TemplateArn": ...,
    }


# UpdateReviewTemplateAnswerInputTypeDef definition

class UpdateReviewTemplateAnswerInputTypeDef(TypedDict):
    TemplateArn: str,
    LensAlias: str,
    QuestionId: str,
    SelectedChoices: NotRequired[Sequence[str]],
    ChoiceUpdates: NotRequired[Mapping[str, ChoiceUpdateTypeDef]],  # (1)
    Notes: NotRequired[str],
    IsApplicable: NotRequired[bool],
    Reason: NotRequired[AnswerReasonType],  # (2)
```

1. See [:material-code-braces: ChoiceUpdateTypeDef](./type_defs.md#choiceupdatetypedef) 
2. See [:material-code-brackets: AnswerReasonType](./literals.md#answerreasontype) 
## CreateLensShareOutputTypeDef

```python
# CreateLensShareOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import CreateLensShareOutputTypeDef


def get_value() -> CreateLensShareOutputTypeDef:
    return {
        "ShareId": ...,
    }


# CreateLensShareOutputTypeDef definition

class CreateLensShareOutputTypeDef(TypedDict):
    ShareId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLensVersionOutputTypeDef

```python
# CreateLensVersionOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import CreateLensVersionOutputTypeDef


def get_value() -> CreateLensVersionOutputTypeDef:
    return {
        "LensArn": ...,
    }


# CreateLensVersionOutputTypeDef definition

class CreateLensVersionOutputTypeDef(TypedDict):
    LensArn: str,
    LensVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMilestoneOutputTypeDef

```python
# CreateMilestoneOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import CreateMilestoneOutputTypeDef


def get_value() -> CreateMilestoneOutputTypeDef:
    return {
        "WorkloadId": ...,
    }


# CreateMilestoneOutputTypeDef definition

class CreateMilestoneOutputTypeDef(TypedDict):
    WorkloadId: str,
    MilestoneNumber: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProfileOutputTypeDef

```python
# CreateProfileOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import CreateProfileOutputTypeDef


def get_value() -> CreateProfileOutputTypeDef:
    return {
        "ProfileArn": ...,
    }


# CreateProfileOutputTypeDef definition

class CreateProfileOutputTypeDef(TypedDict):
    ProfileArn: str,
    ProfileVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProfileShareOutputTypeDef

```python
# CreateProfileShareOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import CreateProfileShareOutputTypeDef


def get_value() -> CreateProfileShareOutputTypeDef:
    return {
        "ShareId": ...,
    }


# CreateProfileShareOutputTypeDef definition

class CreateProfileShareOutputTypeDef(TypedDict):
    ShareId: str,
    ProfileArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateReviewTemplateOutputTypeDef

```python
# CreateReviewTemplateOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import CreateReviewTemplateOutputTypeDef


def get_value() -> CreateReviewTemplateOutputTypeDef:
    return {
        "TemplateArn": ...,
    }


# CreateReviewTemplateOutputTypeDef definition

class CreateReviewTemplateOutputTypeDef(TypedDict):
    TemplateArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTemplateShareOutputTypeDef

```python
# CreateTemplateShareOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import CreateTemplateShareOutputTypeDef


def get_value() -> CreateTemplateShareOutputTypeDef:
    return {
        "TemplateArn": ...,
    }


# CreateTemplateShareOutputTypeDef definition

class CreateTemplateShareOutputTypeDef(TypedDict):
    TemplateArn: str,
    ShareId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkloadOutputTypeDef

```python
# CreateWorkloadOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import CreateWorkloadOutputTypeDef


def get_value() -> CreateWorkloadOutputTypeDef:
    return {
        "WorkloadId": ...,
    }


# CreateWorkloadOutputTypeDef definition

class CreateWorkloadOutputTypeDef(TypedDict):
    WorkloadId: str,
    WorkloadArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkloadShareOutputTypeDef

```python
# CreateWorkloadShareOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import CreateWorkloadShareOutputTypeDef


def get_value() -> CreateWorkloadShareOutputTypeDef:
    return {
        "WorkloadId": ...,
    }


# CreateWorkloadShareOutputTypeDef definition

class CreateWorkloadShareOutputTypeDef(TypedDict):
    WorkloadId: str,
    ShareId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportLensOutputTypeDef

```python
# ExportLensOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ExportLensOutputTypeDef


def get_value() -> ExportLensOutputTypeDef:
    return {
        "LensJSON": ...,
    }


# ExportLensOutputTypeDef definition

class ExportLensOutputTypeDef(TypedDict):
    LensJSON: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGlobalSettingsOutputTypeDef

```python
# GetGlobalSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetGlobalSettingsOutputTypeDef


def get_value() -> GetGlobalSettingsOutputTypeDef:
    return {
        "OrganizationSharingStatus": ...,
    }


# GetGlobalSettingsOutputTypeDef definition

class GetGlobalSettingsOutputTypeDef(TypedDict):
    OrganizationSharingStatus: OrganizationSharingStatusType,  # (1)
    DiscoveryIntegrationStatus: DiscoveryIntegrationStatusType,  # (2)
    JiraConfiguration: AccountJiraConfigurationOutputTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: OrganizationSharingStatusType](./literals.md#organizationsharingstatustype) 
2. See [:material-code-brackets: DiscoveryIntegrationStatusType](./literals.md#discoveryintegrationstatustype) 
3. See [:material-code-braces: AccountJiraConfigurationOutputTypeDef](./type_defs.md#accountjiraconfigurationoutputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportLensOutputTypeDef

```python
# ImportLensOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ImportLensOutputTypeDef


def get_value() -> ImportLensOutputTypeDef:
    return {
        "LensArn": ...,
    }


# ImportLensOutputTypeDef definition

class ImportLensOutputTypeDef(TypedDict):
    LensArn: str,
    Status: ImportLensStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ImportLensStatusType](./literals.md#importlensstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCheckDetailsOutputTypeDef

```python
# ListCheckDetailsOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListCheckDetailsOutputTypeDef


def get_value() -> ListCheckDetailsOutputTypeDef:
    return {
        "CheckDetails": ...,
    }


# ListCheckDetailsOutputTypeDef definition

class ListCheckDetailsOutputTypeDef(TypedDict):
    CheckDetails: List[CheckDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CheckDetailTypeDef](./type_defs.md#checkdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCheckSummariesOutputTypeDef

```python
# ListCheckSummariesOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListCheckSummariesOutputTypeDef


def get_value() -> ListCheckSummariesOutputTypeDef:
    return {
        "CheckSummaries": ...,
    }


# ListCheckSummariesOutputTypeDef definition

class ListCheckSummariesOutputTypeDef(TypedDict):
    CheckSummaries: List[CheckSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CheckSummaryTypeDef](./type_defs.md#checksummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListTagsForResourceOutputTypeDef


def get_value() -> ListTagsForResourceOutputTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProfileInputTypeDef

```python
# CreateProfileInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import CreateProfileInputTypeDef


def get_value() -> CreateProfileInputTypeDef:
    return {
        "ProfileName": ...,
    }


# CreateProfileInputTypeDef definition

class CreateProfileInputTypeDef(TypedDict):
    ProfileName: str,
    ProfileDescription: str,
    ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef],  # (1)
    ClientRequestToken: str,
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ProfileQuestionUpdateTypeDef](./type_defs.md#profilequestionupdatetypedef) 
## UpdateProfileInputTypeDef

```python
# UpdateProfileInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpdateProfileInputTypeDef


def get_value() -> UpdateProfileInputTypeDef:
    return {
        "ProfileArn": ...,
    }


# UpdateProfileInputTypeDef definition

class UpdateProfileInputTypeDef(TypedDict):
    ProfileArn: str,
    ProfileDescription: NotRequired[str],
    ProfileQuestions: NotRequired[Sequence[ProfileQuestionUpdateTypeDef]],  # (1)
```

1. See [:material-code-braces: ProfileQuestionUpdateTypeDef](./type_defs.md#profilequestionupdatetypedef) 
## GetLensOutputTypeDef

```python
# GetLensOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetLensOutputTypeDef


def get_value() -> GetLensOutputTypeDef:
    return {
        "Lens": ...,
    }


# GetLensOutputTypeDef definition

class GetLensOutputTypeDef(TypedDict):
    Lens: LensTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LensTypeDef](./type_defs.md#lenstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLensReviewReportOutputTypeDef

```python
# GetLensReviewReportOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetLensReviewReportOutputTypeDef


def get_value() -> GetLensReviewReportOutputTypeDef:
    return {
        "WorkloadId": ...,
    }


# GetLensReviewReportOutputTypeDef definition

class GetLensReviewReportOutputTypeDef(TypedDict):
    WorkloadId: str,
    MilestoneNumber: int,
    LensReviewReport: LensReviewReportTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LensReviewReportTypeDef](./type_defs.md#lensreviewreporttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetReviewTemplateOutputTypeDef

```python
# GetReviewTemplateOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetReviewTemplateOutputTypeDef


def get_value() -> GetReviewTemplateOutputTypeDef:
    return {
        "ReviewTemplate": ...,
    }


# GetReviewTemplateOutputTypeDef definition

class GetReviewTemplateOutputTypeDef(TypedDict):
    ReviewTemplate: ReviewTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReviewTemplateTypeDef](./type_defs.md#reviewtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateReviewTemplateOutputTypeDef

```python
# UpdateReviewTemplateOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpdateReviewTemplateOutputTypeDef


def get_value() -> UpdateReviewTemplateOutputTypeDef:
    return {
        "ReviewTemplate": ...,
    }


# UpdateReviewTemplateOutputTypeDef definition

class UpdateReviewTemplateOutputTypeDef(TypedDict):
    ReviewTemplate: ReviewTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReviewTemplateTypeDef](./type_defs.md#reviewtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JiraSelectedQuestionConfigurationOutputTypeDef

```python
# JiraSelectedQuestionConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import JiraSelectedQuestionConfigurationOutputTypeDef


def get_value() -> JiraSelectedQuestionConfigurationOutputTypeDef:
    return {
        "SelectedPillars": ...,
    }


# JiraSelectedQuestionConfigurationOutputTypeDef definition

class JiraSelectedQuestionConfigurationOutputTypeDef(TypedDict):
    SelectedPillars: NotRequired[List[SelectedPillarOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: SelectedPillarOutputTypeDef](./type_defs.md#selectedpillaroutputtypedef) 
## JiraSelectedQuestionConfigurationTypeDef

```python
# JiraSelectedQuestionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import JiraSelectedQuestionConfigurationTypeDef


def get_value() -> JiraSelectedQuestionConfigurationTypeDef:
    return {
        "SelectedPillars": ...,
    }


# JiraSelectedQuestionConfigurationTypeDef definition

class JiraSelectedQuestionConfigurationTypeDef(TypedDict):
    SelectedPillars: NotRequired[Sequence[SelectedPillarTypeDef]],  # (1)
```

1. See [:material-code-braces: SelectedPillarTypeDef](./type_defs.md#selectedpillartypedef) 
## LensReviewSummaryTypeDef

```python
# LensReviewSummaryTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import LensReviewSummaryTypeDef


def get_value() -> LensReviewSummaryTypeDef:
    return {
        "LensAlias": ...,
    }


# LensReviewSummaryTypeDef definition

class LensReviewSummaryTypeDef(TypedDict):
    LensAlias: NotRequired[str],
    LensArn: NotRequired[str],
    LensVersion: NotRequired[str],
    LensName: NotRequired[str],
    LensStatus: NotRequired[LensStatusType],  # (1)
    UpdatedAt: NotRequired[datetime],
    RiskCounts: NotRequired[Dict[RiskType, int]],  # (2)
    Profiles: NotRequired[List[WorkloadProfileTypeDef]],  # (3)
    PrioritizedRiskCounts: NotRequired[Dict[RiskType, int]],  # (2)
```

1. See [:material-code-brackets: LensStatusType](./literals.md#lensstatustype) 
2. See [:material-code-brackets: RiskType](./literals.md#risktype) 
3. See [:material-code-braces: WorkloadProfileTypeDef](./type_defs.md#workloadprofiletypedef) 
4. See [:material-code-brackets: RiskType](./literals.md#risktype) 
## WorkloadSummaryTypeDef

```python
# WorkloadSummaryTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import WorkloadSummaryTypeDef


def get_value() -> WorkloadSummaryTypeDef:
    return {
        "WorkloadId": ...,
    }


# WorkloadSummaryTypeDef definition

class WorkloadSummaryTypeDef(TypedDict):
    WorkloadId: NotRequired[str],
    WorkloadArn: NotRequired[str],
    WorkloadName: NotRequired[str],
    Owner: NotRequired[str],
    UpdatedAt: NotRequired[datetime],
    Lenses: NotRequired[List[str]],
    RiskCounts: NotRequired[Dict[RiskType, int]],  # (1)
    ImprovementStatus: NotRequired[WorkloadImprovementStatusType],  # (2)
    Profiles: NotRequired[List[WorkloadProfileTypeDef]],  # (3)
    PrioritizedRiskCounts: NotRequired[Dict[RiskType, int]],  # (1)
```

1. See [:material-code-brackets: RiskType](./literals.md#risktype) 
2. See [:material-code-brackets: WorkloadImprovementStatusType](./literals.md#workloadimprovementstatustype) 
3. See [:material-code-braces: WorkloadProfileTypeDef](./type_defs.md#workloadprofiletypedef) 
4. See [:material-code-brackets: RiskType](./literals.md#risktype) 
## ListLensSharesOutputTypeDef

```python
# ListLensSharesOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListLensSharesOutputTypeDef


def get_value() -> ListLensSharesOutputTypeDef:
    return {
        "LensShareSummaries": ...,
    }


# ListLensSharesOutputTypeDef definition

class ListLensSharesOutputTypeDef(TypedDict):
    LensShareSummaries: List[LensShareSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LensShareSummaryTypeDef](./type_defs.md#lenssharesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLensesOutputTypeDef

```python
# ListLensesOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListLensesOutputTypeDef


def get_value() -> ListLensesOutputTypeDef:
    return {
        "LensSummaries": ...,
    }


# ListLensesOutputTypeDef definition

class ListLensesOutputTypeDef(TypedDict):
    LensSummaries: List[LensSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LensSummaryTypeDef](./type_defs.md#lenssummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NotificationSummaryTypeDef

```python
# NotificationSummaryTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import NotificationSummaryTypeDef


def get_value() -> NotificationSummaryTypeDef:
    return {
        "Type": ...,
    }


# NotificationSummaryTypeDef definition

class NotificationSummaryTypeDef(TypedDict):
    Type: NotRequired[NotificationTypeType],  # (1)
    LensUpgradeSummary: NotRequired[LensUpgradeSummaryTypeDef],  # (2)
```

1. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
2. See [:material-code-braces: LensUpgradeSummaryTypeDef](./type_defs.md#lensupgradesummarytypedef) 
## ListProfileNotificationsOutputTypeDef

```python
# ListProfileNotificationsOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListProfileNotificationsOutputTypeDef


def get_value() -> ListProfileNotificationsOutputTypeDef:
    return {
        "NotificationSummaries": ...,
    }


# ListProfileNotificationsOutputTypeDef definition

class ListProfileNotificationsOutputTypeDef(TypedDict):
    NotificationSummaries: List[ProfileNotificationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProfileNotificationSummaryTypeDef](./type_defs.md#profilenotificationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProfileSharesOutputTypeDef

```python
# ListProfileSharesOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListProfileSharesOutputTypeDef


def get_value() -> ListProfileSharesOutputTypeDef:
    return {
        "ProfileShareSummaries": ...,
    }


# ListProfileSharesOutputTypeDef definition

class ListProfileSharesOutputTypeDef(TypedDict):
    ProfileShareSummaries: List[ProfileShareSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProfileShareSummaryTypeDef](./type_defs.md#profilesharesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProfilesOutputTypeDef

```python
# ListProfilesOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListProfilesOutputTypeDef


def get_value() -> ListProfilesOutputTypeDef:
    return {
        "ProfileSummaries": ...,
    }


# ListProfilesOutputTypeDef definition

class ListProfilesOutputTypeDef(TypedDict):
    ProfileSummaries: List[ProfileSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProfileSummaryTypeDef](./type_defs.md#profilesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReviewTemplatesOutputTypeDef

```python
# ListReviewTemplatesOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListReviewTemplatesOutputTypeDef


def get_value() -> ListReviewTemplatesOutputTypeDef:
    return {
        "ReviewTemplates": ...,
    }


# ListReviewTemplatesOutputTypeDef definition

class ListReviewTemplatesOutputTypeDef(TypedDict):
    ReviewTemplates: List[ReviewTemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ReviewTemplateSummaryTypeDef](./type_defs.md#reviewtemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListShareInvitationsOutputTypeDef

```python
# ListShareInvitationsOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListShareInvitationsOutputTypeDef


def get_value() -> ListShareInvitationsOutputTypeDef:
    return {
        "ShareInvitationSummaries": ...,
    }


# ListShareInvitationsOutputTypeDef definition

class ListShareInvitationsOutputTypeDef(TypedDict):
    ShareInvitationSummaries: List[ShareInvitationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ShareInvitationSummaryTypeDef](./type_defs.md#shareinvitationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTemplateSharesOutputTypeDef

```python
# ListTemplateSharesOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListTemplateSharesOutputTypeDef


def get_value() -> ListTemplateSharesOutputTypeDef:
    return {
        "TemplateArn": ...,
    }


# ListTemplateSharesOutputTypeDef definition

class ListTemplateSharesOutputTypeDef(TypedDict):
    TemplateArn: str,
    TemplateShareSummaries: List[TemplateShareSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TemplateShareSummaryTypeDef](./type_defs.md#templatesharesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkloadSharesOutputTypeDef

```python
# ListWorkloadSharesOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListWorkloadSharesOutputTypeDef


def get_value() -> ListWorkloadSharesOutputTypeDef:
    return {
        "WorkloadId": ...,
    }


# ListWorkloadSharesOutputTypeDef definition

class ListWorkloadSharesOutputTypeDef(TypedDict):
    WorkloadId: str,
    WorkloadShareSummaries: List[WorkloadShareSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkloadShareSummaryTypeDef](./type_defs.md#workloadsharesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PillarDifferenceTypeDef

```python
# PillarDifferenceTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import PillarDifferenceTypeDef


def get_value() -> PillarDifferenceTypeDef:
    return {
        "PillarId": ...,
    }


# PillarDifferenceTypeDef definition

class PillarDifferenceTypeDef(TypedDict):
    PillarId: NotRequired[str],
    PillarName: NotRequired[str],
    DifferenceStatus: NotRequired[DifferenceStatusType],  # (1)
    QuestionDifferences: NotRequired[List[QuestionDifferenceTypeDef]],  # (2)
```

1. See [:material-code-brackets: DifferenceStatusType](./literals.md#differencestatustype) 
2. See [:material-code-braces: QuestionDifferenceTypeDef](./type_defs.md#questiondifferencetypedef) 
## ProfileQuestionTypeDef

```python
# ProfileQuestionTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ProfileQuestionTypeDef


def get_value() -> ProfileQuestionTypeDef:
    return {
        "QuestionId": ...,
    }


# ProfileQuestionTypeDef definition

class ProfileQuestionTypeDef(TypedDict):
    QuestionId: NotRequired[str],
    QuestionTitle: NotRequired[str],
    QuestionDescription: NotRequired[str],
    QuestionChoices: NotRequired[List[ProfileChoiceTypeDef]],  # (1)
    SelectedChoiceIds: NotRequired[List[str]],
    MinSelectedChoices: NotRequired[int],
    MaxSelectedChoices: NotRequired[int],
```

1. See [:material-code-braces: ProfileChoiceTypeDef](./type_defs.md#profilechoicetypedef) 
## ProfileTemplateQuestionTypeDef

```python
# ProfileTemplateQuestionTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ProfileTemplateQuestionTypeDef


def get_value() -> ProfileTemplateQuestionTypeDef:
    return {
        "QuestionId": ...,
    }


# ProfileTemplateQuestionTypeDef definition

class ProfileTemplateQuestionTypeDef(TypedDict):
    QuestionId: NotRequired[str],
    QuestionTitle: NotRequired[str],
    QuestionDescription: NotRequired[str],
    QuestionChoices: NotRequired[List[ProfileTemplateChoiceTypeDef]],  # (1)
    MinSelectedChoices: NotRequired[int],
    MaxSelectedChoices: NotRequired[int],
```

1. See [:material-code-braces: ProfileTemplateChoiceTypeDef](./type_defs.md#profiletemplatechoicetypedef) 
## ReviewTemplateLensReviewTypeDef

```python
# ReviewTemplateLensReviewTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ReviewTemplateLensReviewTypeDef


def get_value() -> ReviewTemplateLensReviewTypeDef:
    return {
        "LensAlias": ...,
    }


# ReviewTemplateLensReviewTypeDef definition

class ReviewTemplateLensReviewTypeDef(TypedDict):
    LensAlias: NotRequired[str],
    LensArn: NotRequired[str],
    LensVersion: NotRequired[str],
    LensName: NotRequired[str],
    LensStatus: NotRequired[LensStatusType],  # (1)
    PillarReviewSummaries: NotRequired[List[ReviewTemplatePillarReviewSummaryTypeDef]],  # (2)
    UpdatedAt: NotRequired[datetime],
    Notes: NotRequired[str],
    QuestionCounts: NotRequired[Dict[QuestionType, int]],  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: LensStatusType](./literals.md#lensstatustype) 
2. See [:material-code-braces: ReviewTemplatePillarReviewSummaryTypeDef](./type_defs.md#reviewtemplatepillarreviewsummarytypedef) 
3. See [:material-code-brackets: QuestionType](./literals.md#questiontype) 
## UpdateShareInvitationOutputTypeDef

```python
# UpdateShareInvitationOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpdateShareInvitationOutputTypeDef


def get_value() -> UpdateShareInvitationOutputTypeDef:
    return {
        "ShareInvitation": ...,
    }


# UpdateShareInvitationOutputTypeDef definition

class UpdateShareInvitationOutputTypeDef(TypedDict):
    ShareInvitation: ShareInvitationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ShareInvitationTypeDef](./type_defs.md#shareinvitationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorkloadShareOutputTypeDef

```python
# UpdateWorkloadShareOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpdateWorkloadShareOutputTypeDef


def get_value() -> UpdateWorkloadShareOutputTypeDef:
    return {
        "WorkloadId": ...,
    }


# UpdateWorkloadShareOutputTypeDef definition

class UpdateWorkloadShareOutputTypeDef(TypedDict):
    WorkloadId: str,
    WorkloadShare: WorkloadShareTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkloadShareTypeDef](./type_defs.md#workloadsharetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkloadTypeDef

```python
# WorkloadTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import WorkloadTypeDef


def get_value() -> WorkloadTypeDef:
    return {
        "WorkloadId": ...,
    }


# WorkloadTypeDef definition

class WorkloadTypeDef(TypedDict):
    WorkloadId: NotRequired[str],
    WorkloadArn: NotRequired[str],
    WorkloadName: NotRequired[str],
    Description: NotRequired[str],
    Environment: NotRequired[WorkloadEnvironmentType],  # (1)
    UpdatedAt: NotRequired[datetime],
    AccountIds: NotRequired[List[str]],
    AwsRegions: NotRequired[List[str]],
    NonAwsRegions: NotRequired[List[str]],
    ArchitecturalDesign: NotRequired[str],
    ReviewOwner: NotRequired[str],
    ReviewRestrictionDate: NotRequired[datetime],
    IsReviewOwnerUpdateAcknowledged: NotRequired[bool],
    IndustryType: NotRequired[str],
    Industry: NotRequired[str],
    Notes: NotRequired[str],
    ImprovementStatus: NotRequired[WorkloadImprovementStatusType],  # (2)
    RiskCounts: NotRequired[Dict[RiskType, int]],  # (3)
    PillarPriorities: NotRequired[List[str]],
    Lenses: NotRequired[List[str]],
    Owner: NotRequired[str],
    ShareInvitationId: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
    DiscoveryConfig: NotRequired[WorkloadDiscoveryConfigOutputTypeDef],  # (4)
    Applications: NotRequired[List[str]],
    Profiles: NotRequired[List[WorkloadProfileTypeDef]],  # (5)
    PrioritizedRiskCounts: NotRequired[Dict[RiskType, int]],  # (3)
    JiraConfiguration: NotRequired[WorkloadJiraConfigurationOutputTypeDef],  # (7)
```

1. See [:material-code-brackets: WorkloadEnvironmentType](./literals.md#workloadenvironmenttype) 
2. See [:material-code-brackets: WorkloadImprovementStatusType](./literals.md#workloadimprovementstatustype) 
3. See [:material-code-brackets: RiskType](./literals.md#risktype) 
4. See [:material-code-braces: WorkloadDiscoveryConfigOutputTypeDef](./type_defs.md#workloaddiscoveryconfigoutputtypedef) 
5. See [:material-code-braces: WorkloadProfileTypeDef](./type_defs.md#workloadprofiletypedef) 
6. See [:material-code-brackets: RiskType](./literals.md#risktype) 
7. See [:material-code-braces: WorkloadJiraConfigurationOutputTypeDef](./type_defs.md#workloadjiraconfigurationoutputtypedef) 
## ChoiceTypeDef

```python
# ChoiceTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ChoiceTypeDef


def get_value() -> ChoiceTypeDef:
    return {
        "ChoiceId": ...,
    }


# ChoiceTypeDef definition

class ChoiceTypeDef(TypedDict):
    ChoiceId: NotRequired[str],
    Title: NotRequired[str],
    Description: NotRequired[str],
    HelpfulResource: NotRequired[ChoiceContentTypeDef],  # (1)
    ImprovementPlan: NotRequired[ChoiceContentTypeDef],  # (1)
    AdditionalResources: NotRequired[List[AdditionalResourcesTypeDef]],  # (3)
```

1. See [:material-code-braces: ChoiceContentTypeDef](./type_defs.md#choicecontenttypedef) 
2. See [:material-code-braces: ChoiceContentTypeDef](./type_defs.md#choicecontenttypedef) 
3. See [:material-code-braces: AdditionalResourcesTypeDef](./type_defs.md#additionalresourcestypedef) 
## PillarMetricTypeDef

```python
# PillarMetricTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import PillarMetricTypeDef


def get_value() -> PillarMetricTypeDef:
    return {
        "PillarId": ...,
    }


# PillarMetricTypeDef definition

class PillarMetricTypeDef(TypedDict):
    PillarId: NotRequired[str],
    RiskCounts: NotRequired[Dict[RiskType, int]],  # (1)
    Questions: NotRequired[List[QuestionMetricTypeDef]],  # (2)
```

1. See [:material-code-brackets: RiskType](./literals.md#risktype) 
2. See [:material-code-braces: QuestionMetricTypeDef](./type_defs.md#questionmetrictypedef) 
## ListLensReviewImprovementsOutputTypeDef

```python
# ListLensReviewImprovementsOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListLensReviewImprovementsOutputTypeDef


def get_value() -> ListLensReviewImprovementsOutputTypeDef:
    return {
        "WorkloadId": ...,
    }


# ListLensReviewImprovementsOutputTypeDef definition

class ListLensReviewImprovementsOutputTypeDef(TypedDict):
    WorkloadId: str,
    MilestoneNumber: int,
    LensAlias: str,
    LensArn: str,
    ImprovementSummaries: List[ImprovementSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ImprovementSummaryTypeDef](./type_defs.md#improvementsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LensReviewTypeDef

```python
# LensReviewTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import LensReviewTypeDef


def get_value() -> LensReviewTypeDef:
    return {
        "LensAlias": ...,
    }


# LensReviewTypeDef definition

class LensReviewTypeDef(TypedDict):
    LensAlias: NotRequired[str],
    LensArn: NotRequired[str],
    LensVersion: NotRequired[str],
    LensName: NotRequired[str],
    LensStatus: NotRequired[LensStatusType],  # (1)
    PillarReviewSummaries: NotRequired[List[PillarReviewSummaryTypeDef]],  # (2)
    JiraConfiguration: NotRequired[JiraSelectedQuestionConfigurationOutputTypeDef],  # (3)
    UpdatedAt: NotRequired[datetime],
    Notes: NotRequired[str],
    RiskCounts: NotRequired[Dict[RiskType, int]],  # (4)
    NextToken: NotRequired[str],
    Profiles: NotRequired[List[WorkloadProfileTypeDef]],  # (5)
    PrioritizedRiskCounts: NotRequired[Dict[RiskType, int]],  # (4)
```

1. See [:material-code-brackets: LensStatusType](./literals.md#lensstatustype) 
2. See [:material-code-braces: PillarReviewSummaryTypeDef](./type_defs.md#pillarreviewsummarytypedef) 
3. See [:material-code-braces: JiraSelectedQuestionConfigurationOutputTypeDef](./type_defs.md#jiraselectedquestionconfigurationoutputtypedef) 
4. See [:material-code-brackets: RiskType](./literals.md#risktype) 
5. See [:material-code-braces: WorkloadProfileTypeDef](./type_defs.md#workloadprofiletypedef) 
6. See [:material-code-brackets: RiskType](./literals.md#risktype) 
## ListLensReviewsOutputTypeDef

```python
# ListLensReviewsOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListLensReviewsOutputTypeDef


def get_value() -> ListLensReviewsOutputTypeDef:
    return {
        "WorkloadId": ...,
    }


# ListLensReviewsOutputTypeDef definition

class ListLensReviewsOutputTypeDef(TypedDict):
    WorkloadId: str,
    MilestoneNumber: int,
    LensReviewSummaries: List[LensReviewSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LensReviewSummaryTypeDef](./type_defs.md#lensreviewsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkloadsOutputTypeDef

```python
# ListWorkloadsOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListWorkloadsOutputTypeDef


def get_value() -> ListWorkloadsOutputTypeDef:
    return {
        "WorkloadSummaries": ...,
    }


# ListWorkloadsOutputTypeDef definition

class ListWorkloadsOutputTypeDef(TypedDict):
    WorkloadSummaries: List[WorkloadSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkloadSummaryTypeDef](./type_defs.md#workloadsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MilestoneSummaryTypeDef

```python
# MilestoneSummaryTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import MilestoneSummaryTypeDef


def get_value() -> MilestoneSummaryTypeDef:
    return {
        "MilestoneNumber": ...,
    }


# MilestoneSummaryTypeDef definition

class MilestoneSummaryTypeDef(TypedDict):
    MilestoneNumber: NotRequired[int],
    MilestoneName: NotRequired[str],
    RecordedAt: NotRequired[datetime],
    WorkloadSummary: NotRequired[WorkloadSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: WorkloadSummaryTypeDef](./type_defs.md#workloadsummarytypedef) 
## ListNotificationsOutputTypeDef

```python
# ListNotificationsOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListNotificationsOutputTypeDef


def get_value() -> ListNotificationsOutputTypeDef:
    return {
        "NotificationSummaries": ...,
    }


# ListNotificationsOutputTypeDef definition

class ListNotificationsOutputTypeDef(TypedDict):
    NotificationSummaries: List[NotificationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: NotificationSummaryTypeDef](./type_defs.md#notificationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VersionDifferencesTypeDef

```python
# VersionDifferencesTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import VersionDifferencesTypeDef


def get_value() -> VersionDifferencesTypeDef:
    return {
        "PillarDifferences": ...,
    }


# VersionDifferencesTypeDef definition

class VersionDifferencesTypeDef(TypedDict):
    PillarDifferences: NotRequired[List[PillarDifferenceTypeDef]],  # (1)
```

1. See [:material-code-braces: PillarDifferenceTypeDef](./type_defs.md#pillardifferencetypedef) 
## ProfileTypeDef

```python
# ProfileTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ProfileTypeDef


def get_value() -> ProfileTypeDef:
    return {
        "ProfileArn": ...,
    }


# ProfileTypeDef definition

class ProfileTypeDef(TypedDict):
    ProfileArn: NotRequired[str],
    ProfileVersion: NotRequired[str],
    ProfileName: NotRequired[str],
    ProfileDescription: NotRequired[str],
    ProfileQuestions: NotRequired[List[ProfileQuestionTypeDef]],  # (1)
    Owner: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    UpdatedAt: NotRequired[datetime],
    ShareInvitationId: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ProfileQuestionTypeDef](./type_defs.md#profilequestiontypedef) 
## ProfileTemplateTypeDef

```python
# ProfileTemplateTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ProfileTemplateTypeDef


def get_value() -> ProfileTemplateTypeDef:
    return {
        "TemplateName": ...,
    }


# ProfileTemplateTypeDef definition

class ProfileTemplateTypeDef(TypedDict):
    TemplateName: NotRequired[str],
    TemplateQuestions: NotRequired[List[ProfileTemplateQuestionTypeDef]],  # (1)
    CreatedAt: NotRequired[datetime],
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: ProfileTemplateQuestionTypeDef](./type_defs.md#profiletemplatequestiontypedef) 
## GetReviewTemplateLensReviewOutputTypeDef

```python
# GetReviewTemplateLensReviewOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetReviewTemplateLensReviewOutputTypeDef


def get_value() -> GetReviewTemplateLensReviewOutputTypeDef:
    return {
        "TemplateArn": ...,
    }


# GetReviewTemplateLensReviewOutputTypeDef definition

class GetReviewTemplateLensReviewOutputTypeDef(TypedDict):
    TemplateArn: str,
    LensReview: ReviewTemplateLensReviewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReviewTemplateLensReviewTypeDef](./type_defs.md#reviewtemplatelensreviewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateReviewTemplateLensReviewOutputTypeDef

```python
# UpdateReviewTemplateLensReviewOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpdateReviewTemplateLensReviewOutputTypeDef


def get_value() -> UpdateReviewTemplateLensReviewOutputTypeDef:
    return {
        "TemplateArn": ...,
    }


# UpdateReviewTemplateLensReviewOutputTypeDef definition

class UpdateReviewTemplateLensReviewOutputTypeDef(TypedDict):
    TemplateArn: str,
    LensReview: ReviewTemplateLensReviewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReviewTemplateLensReviewTypeDef](./type_defs.md#reviewtemplatelensreviewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkloadInputTypeDef

```python
# CreateWorkloadInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import CreateWorkloadInputTypeDef


def get_value() -> CreateWorkloadInputTypeDef:
    return {
        "WorkloadName": ...,
    }


# CreateWorkloadInputTypeDef definition

class CreateWorkloadInputTypeDef(TypedDict):
    WorkloadName: str,
    Description: str,
    Environment: WorkloadEnvironmentType,  # (1)
    Lenses: Sequence[str],
    ClientRequestToken: str,
    AccountIds: NotRequired[Sequence[str]],
    AwsRegions: NotRequired[Sequence[str]],
    NonAwsRegions: NotRequired[Sequence[str]],
    PillarPriorities: NotRequired[Sequence[str]],
    ArchitecturalDesign: NotRequired[str],
    ReviewOwner: NotRequired[str],
    IndustryType: NotRequired[str],
    Industry: NotRequired[str],
    Notes: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    DiscoveryConfig: NotRequired[WorkloadDiscoveryConfigUnionTypeDef],  # (2)
    Applications: NotRequired[Sequence[str]],
    ProfileArns: NotRequired[Sequence[str]],
    ReviewTemplateArns: NotRequired[Sequence[str]],
    JiraConfiguration: NotRequired[WorkloadJiraConfigurationInputTypeDef],  # (3)
```

1. See [:material-code-brackets: WorkloadEnvironmentType](./literals.md#workloadenvironmenttype) 
2. See [:material-code-braces: WorkloadDiscoveryConfigTypeDef](./type_defs.md#workloaddiscoveryconfigtypedef) [:material-code-braces: WorkloadDiscoveryConfigOutputTypeDef](./type_defs.md#workloaddiscoveryconfigoutputtypedef) 
3. See [:material-code-braces: WorkloadJiraConfigurationInputTypeDef](./type_defs.md#workloadjiraconfigurationinputtypedef) 
## UpdateWorkloadInputTypeDef

```python
# UpdateWorkloadInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpdateWorkloadInputTypeDef


def get_value() -> UpdateWorkloadInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# UpdateWorkloadInputTypeDef definition

class UpdateWorkloadInputTypeDef(TypedDict):
    WorkloadId: str,
    WorkloadName: NotRequired[str],
    Description: NotRequired[str],
    Environment: NotRequired[WorkloadEnvironmentType],  # (1)
    AccountIds: NotRequired[Sequence[str]],
    AwsRegions: NotRequired[Sequence[str]],
    NonAwsRegions: NotRequired[Sequence[str]],
    PillarPriorities: NotRequired[Sequence[str]],
    ArchitecturalDesign: NotRequired[str],
    ReviewOwner: NotRequired[str],
    IsReviewOwnerUpdateAcknowledged: NotRequired[bool],
    IndustryType: NotRequired[str],
    Industry: NotRequired[str],
    Notes: NotRequired[str],
    ImprovementStatus: NotRequired[WorkloadImprovementStatusType],  # (2)
    DiscoveryConfig: NotRequired[WorkloadDiscoveryConfigUnionTypeDef],  # (3)
    Applications: NotRequired[Sequence[str]],
    JiraConfiguration: NotRequired[WorkloadJiraConfigurationInputTypeDef],  # (4)
```

1. See [:material-code-brackets: WorkloadEnvironmentType](./literals.md#workloadenvironmenttype) 
2. See [:material-code-brackets: WorkloadImprovementStatusType](./literals.md#workloadimprovementstatustype) 
3. See [:material-code-braces: WorkloadDiscoveryConfigTypeDef](./type_defs.md#workloaddiscoveryconfigtypedef) [:material-code-braces: WorkloadDiscoveryConfigOutputTypeDef](./type_defs.md#workloaddiscoveryconfigoutputtypedef) 
4. See [:material-code-braces: WorkloadJiraConfigurationInputTypeDef](./type_defs.md#workloadjiraconfigurationinputtypedef) 
## GetWorkloadOutputTypeDef

```python
# GetWorkloadOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetWorkloadOutputTypeDef


def get_value() -> GetWorkloadOutputTypeDef:
    return {
        "Workload": ...,
    }


# GetWorkloadOutputTypeDef definition

class GetWorkloadOutputTypeDef(TypedDict):
    Workload: WorkloadTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkloadTypeDef](./type_defs.md#workloadtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MilestoneTypeDef

```python
# MilestoneTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import MilestoneTypeDef


def get_value() -> MilestoneTypeDef:
    return {
        "MilestoneNumber": ...,
    }


# MilestoneTypeDef definition

class MilestoneTypeDef(TypedDict):
    MilestoneNumber: NotRequired[int],
    MilestoneName: NotRequired[str],
    RecordedAt: NotRequired[datetime],
    Workload: NotRequired[WorkloadTypeDef],  # (1)
```

1. See [:material-code-braces: WorkloadTypeDef](./type_defs.md#workloadtypedef) 
## UpdateWorkloadOutputTypeDef

```python
# UpdateWorkloadOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpdateWorkloadOutputTypeDef


def get_value() -> UpdateWorkloadOutputTypeDef:
    return {
        "Workload": ...,
    }


# UpdateWorkloadOutputTypeDef definition

class UpdateWorkloadOutputTypeDef(TypedDict):
    Workload: WorkloadTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkloadTypeDef](./type_defs.md#workloadtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AnswerSummaryTypeDef

```python
# AnswerSummaryTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import AnswerSummaryTypeDef


def get_value() -> AnswerSummaryTypeDef:
    return {
        "QuestionId": ...,
    }


# AnswerSummaryTypeDef definition

class AnswerSummaryTypeDef(TypedDict):
    QuestionId: NotRequired[str],
    PillarId: NotRequired[str],
    QuestionTitle: NotRequired[str],
    Choices: NotRequired[List[ChoiceTypeDef]],  # (1)
    SelectedChoices: NotRequired[List[str]],
    ChoiceAnswerSummaries: NotRequired[List[ChoiceAnswerSummaryTypeDef]],  # (2)
    IsApplicable: NotRequired[bool],
    Risk: NotRequired[RiskType],  # (3)
    Reason: NotRequired[AnswerReasonType],  # (4)
    QuestionType: NotRequired[QuestionTypeType],  # (5)
    JiraConfiguration: NotRequired[JiraConfigurationTypeDef],  # (6)
```

1. See [:material-code-braces: ChoiceTypeDef](./type_defs.md#choicetypedef) 
2. See [:material-code-braces: ChoiceAnswerSummaryTypeDef](./type_defs.md#choiceanswersummarytypedef) 
3. See [:material-code-brackets: RiskType](./literals.md#risktype) 
4. See [:material-code-brackets: AnswerReasonType](./literals.md#answerreasontype) 
5. See [:material-code-brackets: QuestionTypeType](./literals.md#questiontypetype) 
6. See [:material-code-braces: JiraConfigurationTypeDef](./type_defs.md#jiraconfigurationtypedef) 
## AnswerTypeDef

```python
# AnswerTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import AnswerTypeDef


def get_value() -> AnswerTypeDef:
    return {
        "QuestionId": ...,
    }


# AnswerTypeDef definition

class AnswerTypeDef(TypedDict):
    QuestionId: NotRequired[str],
    PillarId: NotRequired[str],
    QuestionTitle: NotRequired[str],
    QuestionDescription: NotRequired[str],
    ImprovementPlanUrl: NotRequired[str],
    HelpfulResourceUrl: NotRequired[str],
    HelpfulResourceDisplayText: NotRequired[str],
    Choices: NotRequired[List[ChoiceTypeDef]],  # (1)
    SelectedChoices: NotRequired[List[str]],
    ChoiceAnswers: NotRequired[List[ChoiceAnswerTypeDef]],  # (2)
    IsApplicable: NotRequired[bool],
    Risk: NotRequired[RiskType],  # (3)
    Notes: NotRequired[str],
    Reason: NotRequired[AnswerReasonType],  # (4)
    JiraConfiguration: NotRequired[JiraConfigurationTypeDef],  # (5)
```

1. See [:material-code-braces: ChoiceTypeDef](./type_defs.md#choicetypedef) 
2. See [:material-code-braces: ChoiceAnswerTypeDef](./type_defs.md#choiceanswertypedef) 
3. See [:material-code-brackets: RiskType](./literals.md#risktype) 
4. See [:material-code-brackets: AnswerReasonType](./literals.md#answerreasontype) 
5. See [:material-code-braces: JiraConfigurationTypeDef](./type_defs.md#jiraconfigurationtypedef) 
## ReviewTemplateAnswerSummaryTypeDef

```python
# ReviewTemplateAnswerSummaryTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ReviewTemplateAnswerSummaryTypeDef


def get_value() -> ReviewTemplateAnswerSummaryTypeDef:
    return {
        "QuestionId": ...,
    }


# ReviewTemplateAnswerSummaryTypeDef definition

class ReviewTemplateAnswerSummaryTypeDef(TypedDict):
    QuestionId: NotRequired[str],
    PillarId: NotRequired[str],
    QuestionTitle: NotRequired[str],
    Choices: NotRequired[List[ChoiceTypeDef]],  # (1)
    SelectedChoices: NotRequired[List[str]],
    ChoiceAnswerSummaries: NotRequired[List[ChoiceAnswerSummaryTypeDef]],  # (2)
    IsApplicable: NotRequired[bool],
    AnswerStatus: NotRequired[ReviewTemplateAnswerStatusType],  # (3)
    Reason: NotRequired[AnswerReasonType],  # (4)
    QuestionType: NotRequired[QuestionTypeType],  # (5)
```

1. See [:material-code-braces: ChoiceTypeDef](./type_defs.md#choicetypedef) 
2. See [:material-code-braces: ChoiceAnswerSummaryTypeDef](./type_defs.md#choiceanswersummarytypedef) 
3. See [:material-code-brackets: ReviewTemplateAnswerStatusType](./literals.md#reviewtemplateanswerstatustype) 
4. See [:material-code-brackets: AnswerReasonType](./literals.md#answerreasontype) 
5. See [:material-code-brackets: QuestionTypeType](./literals.md#questiontypetype) 
## ReviewTemplateAnswerTypeDef

```python
# ReviewTemplateAnswerTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ReviewTemplateAnswerTypeDef


def get_value() -> ReviewTemplateAnswerTypeDef:
    return {
        "QuestionId": ...,
    }


# ReviewTemplateAnswerTypeDef definition

class ReviewTemplateAnswerTypeDef(TypedDict):
    QuestionId: NotRequired[str],
    PillarId: NotRequired[str],
    QuestionTitle: NotRequired[str],
    QuestionDescription: NotRequired[str],
    ImprovementPlanUrl: NotRequired[str],
    HelpfulResourceUrl: NotRequired[str],
    HelpfulResourceDisplayText: NotRequired[str],
    Choices: NotRequired[List[ChoiceTypeDef]],  # (1)
    SelectedChoices: NotRequired[List[str]],
    ChoiceAnswers: NotRequired[List[ChoiceAnswerTypeDef]],  # (2)
    IsApplicable: NotRequired[bool],
    AnswerStatus: NotRequired[ReviewTemplateAnswerStatusType],  # (3)
    Notes: NotRequired[str],
    Reason: NotRequired[AnswerReasonType],  # (4)
```

1. See [:material-code-braces: ChoiceTypeDef](./type_defs.md#choicetypedef) 
2. See [:material-code-braces: ChoiceAnswerTypeDef](./type_defs.md#choiceanswertypedef) 
3. See [:material-code-brackets: ReviewTemplateAnswerStatusType](./literals.md#reviewtemplateanswerstatustype) 
4. See [:material-code-brackets: AnswerReasonType](./literals.md#answerreasontype) 
## LensMetricTypeDef

```python
# LensMetricTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import LensMetricTypeDef


def get_value() -> LensMetricTypeDef:
    return {
        "LensArn": ...,
    }


# LensMetricTypeDef definition

class LensMetricTypeDef(TypedDict):
    LensArn: NotRequired[str],
    Pillars: NotRequired[List[PillarMetricTypeDef]],  # (1)
    RiskCounts: NotRequired[Dict[RiskType, int]],  # (2)
```

1. See [:material-code-braces: PillarMetricTypeDef](./type_defs.md#pillarmetrictypedef) 
2. See [:material-code-brackets: RiskType](./literals.md#risktype) 
## GetLensReviewOutputTypeDef

```python
# GetLensReviewOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetLensReviewOutputTypeDef


def get_value() -> GetLensReviewOutputTypeDef:
    return {
        "WorkloadId": ...,
    }


# GetLensReviewOutputTypeDef definition

class GetLensReviewOutputTypeDef(TypedDict):
    WorkloadId: str,
    MilestoneNumber: int,
    LensReview: LensReviewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LensReviewTypeDef](./type_defs.md#lensreviewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLensReviewOutputTypeDef

```python
# UpdateLensReviewOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpdateLensReviewOutputTypeDef


def get_value() -> UpdateLensReviewOutputTypeDef:
    return {
        "WorkloadId": ...,
    }


# UpdateLensReviewOutputTypeDef definition

class UpdateLensReviewOutputTypeDef(TypedDict):
    WorkloadId: str,
    LensReview: LensReviewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LensReviewTypeDef](./type_defs.md#lensreviewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLensReviewInputTypeDef

```python
# UpdateLensReviewInputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpdateLensReviewInputTypeDef


def get_value() -> UpdateLensReviewInputTypeDef:
    return {
        "WorkloadId": ...,
    }


# UpdateLensReviewInputTypeDef definition

class UpdateLensReviewInputTypeDef(TypedDict):
    WorkloadId: str,
    LensAlias: str,
    LensNotes: NotRequired[str],
    PillarNotes: NotRequired[Mapping[str, str]],
    JiraConfiguration: NotRequired[JiraSelectedQuestionConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: JiraSelectedQuestionConfigurationTypeDef](./type_defs.md#jiraselectedquestionconfigurationtypedef) [:material-code-braces: JiraSelectedQuestionConfigurationOutputTypeDef](./type_defs.md#jiraselectedquestionconfigurationoutputtypedef) 
## ListMilestonesOutputTypeDef

```python
# ListMilestonesOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListMilestonesOutputTypeDef


def get_value() -> ListMilestonesOutputTypeDef:
    return {
        "WorkloadId": ...,
    }


# ListMilestonesOutputTypeDef definition

class ListMilestonesOutputTypeDef(TypedDict):
    WorkloadId: str,
    MilestoneSummaries: List[MilestoneSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MilestoneSummaryTypeDef](./type_defs.md#milestonesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLensVersionDifferenceOutputTypeDef

```python
# GetLensVersionDifferenceOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetLensVersionDifferenceOutputTypeDef


def get_value() -> GetLensVersionDifferenceOutputTypeDef:
    return {
        "LensAlias": ...,
    }


# GetLensVersionDifferenceOutputTypeDef definition

class GetLensVersionDifferenceOutputTypeDef(TypedDict):
    LensAlias: str,
    LensArn: str,
    BaseLensVersion: str,
    TargetLensVersion: str,
    LatestLensVersion: str,
    VersionDifferences: VersionDifferencesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VersionDifferencesTypeDef](./type_defs.md#versiondifferencestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProfileOutputTypeDef

```python
# GetProfileOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetProfileOutputTypeDef


def get_value() -> GetProfileOutputTypeDef:
    return {
        "Profile": ...,
    }


# GetProfileOutputTypeDef definition

class GetProfileOutputTypeDef(TypedDict):
    Profile: ProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfileTypeDef](./type_defs.md#profiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProfileOutputTypeDef

```python
# UpdateProfileOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpdateProfileOutputTypeDef


def get_value() -> UpdateProfileOutputTypeDef:
    return {
        "Profile": ...,
    }


# UpdateProfileOutputTypeDef definition

class UpdateProfileOutputTypeDef(TypedDict):
    Profile: ProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfileTypeDef](./type_defs.md#profiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProfileTemplateOutputTypeDef

```python
# GetProfileTemplateOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetProfileTemplateOutputTypeDef


def get_value() -> GetProfileTemplateOutputTypeDef:
    return {
        "ProfileTemplate": ...,
    }


# GetProfileTemplateOutputTypeDef definition

class GetProfileTemplateOutputTypeDef(TypedDict):
    ProfileTemplate: ProfileTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfileTemplateTypeDef](./type_defs.md#profiletemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMilestoneOutputTypeDef

```python
# GetMilestoneOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetMilestoneOutputTypeDef


def get_value() -> GetMilestoneOutputTypeDef:
    return {
        "WorkloadId": ...,
    }


# GetMilestoneOutputTypeDef definition

class GetMilestoneOutputTypeDef(TypedDict):
    WorkloadId: str,
    Milestone: MilestoneTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MilestoneTypeDef](./type_defs.md#milestonetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAnswersOutputTypeDef

```python
# ListAnswersOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListAnswersOutputTypeDef


def get_value() -> ListAnswersOutputTypeDef:
    return {
        "WorkloadId": ...,
    }


# ListAnswersOutputTypeDef definition

class ListAnswersOutputTypeDef(TypedDict):
    WorkloadId: str,
    MilestoneNumber: int,
    LensAlias: str,
    LensArn: str,
    AnswerSummaries: List[AnswerSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AnswerSummaryTypeDef](./type_defs.md#answersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAnswerOutputTypeDef

```python
# GetAnswerOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetAnswerOutputTypeDef


def get_value() -> GetAnswerOutputTypeDef:
    return {
        "WorkloadId": ...,
    }


# GetAnswerOutputTypeDef definition

class GetAnswerOutputTypeDef(TypedDict):
    WorkloadId: str,
    MilestoneNumber: int,
    LensAlias: str,
    LensArn: str,
    Answer: AnswerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnswerTypeDef](./type_defs.md#answertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAnswerOutputTypeDef

```python
# UpdateAnswerOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpdateAnswerOutputTypeDef


def get_value() -> UpdateAnswerOutputTypeDef:
    return {
        "WorkloadId": ...,
    }


# UpdateAnswerOutputTypeDef definition

class UpdateAnswerOutputTypeDef(TypedDict):
    WorkloadId: str,
    LensAlias: str,
    LensArn: str,
    Answer: AnswerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnswerTypeDef](./type_defs.md#answertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReviewTemplateAnswersOutputTypeDef

```python
# ListReviewTemplateAnswersOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ListReviewTemplateAnswersOutputTypeDef


def get_value() -> ListReviewTemplateAnswersOutputTypeDef:
    return {
        "TemplateArn": ...,
    }


# ListReviewTemplateAnswersOutputTypeDef definition

class ListReviewTemplateAnswersOutputTypeDef(TypedDict):
    TemplateArn: str,
    LensAlias: str,
    AnswerSummaries: List[ReviewTemplateAnswerSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ReviewTemplateAnswerSummaryTypeDef](./type_defs.md#reviewtemplateanswersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetReviewTemplateAnswerOutputTypeDef

```python
# GetReviewTemplateAnswerOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetReviewTemplateAnswerOutputTypeDef


def get_value() -> GetReviewTemplateAnswerOutputTypeDef:
    return {
        "TemplateArn": ...,
    }


# GetReviewTemplateAnswerOutputTypeDef definition

class GetReviewTemplateAnswerOutputTypeDef(TypedDict):
    TemplateArn: str,
    LensAlias: str,
    Answer: ReviewTemplateAnswerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReviewTemplateAnswerTypeDef](./type_defs.md#reviewtemplateanswertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateReviewTemplateAnswerOutputTypeDef

```python
# UpdateReviewTemplateAnswerOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import UpdateReviewTemplateAnswerOutputTypeDef


def get_value() -> UpdateReviewTemplateAnswerOutputTypeDef:
    return {
        "TemplateArn": ...,
    }


# UpdateReviewTemplateAnswerOutputTypeDef definition

class UpdateReviewTemplateAnswerOutputTypeDef(TypedDict):
    TemplateArn: str,
    LensAlias: str,
    Answer: ReviewTemplateAnswerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReviewTemplateAnswerTypeDef](./type_defs.md#reviewtemplateanswertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConsolidatedReportMetricTypeDef

```python
# ConsolidatedReportMetricTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import ConsolidatedReportMetricTypeDef


def get_value() -> ConsolidatedReportMetricTypeDef:
    return {
        "MetricType": ...,
    }


# ConsolidatedReportMetricTypeDef definition

class ConsolidatedReportMetricTypeDef(TypedDict):
    MetricType: NotRequired[MetricTypeType],  # (1)
    RiskCounts: NotRequired[Dict[RiskType, int]],  # (2)
    WorkloadId: NotRequired[str],
    WorkloadName: NotRequired[str],
    WorkloadArn: NotRequired[str],
    UpdatedAt: NotRequired[datetime],
    Lenses: NotRequired[List[LensMetricTypeDef]],  # (3)
    LensesAppliedCount: NotRequired[int],
```

1. See [:material-code-brackets: MetricTypeType](./literals.md#metrictypetype) 
2. See [:material-code-brackets: RiskType](./literals.md#risktype) 
3. See [:material-code-braces: LensMetricTypeDef](./type_defs.md#lensmetrictypedef) 
## GetConsolidatedReportOutputTypeDef

```python
# GetConsolidatedReportOutputTypeDef TypedDict usage example

from types_aiobotocore_wellarchitected.type_defs import GetConsolidatedReportOutputTypeDef


def get_value() -> GetConsolidatedReportOutputTypeDef:
    return {
        "Metrics": ...,
    }


# GetConsolidatedReportOutputTypeDef definition

class GetConsolidatedReportOutputTypeDef(TypedDict):
    Metrics: List[ConsolidatedReportMetricTypeDef],  # (1)
    Base64String: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConsolidatedReportMetricTypeDef](./type_defs.md#consolidatedreportmetrictypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
