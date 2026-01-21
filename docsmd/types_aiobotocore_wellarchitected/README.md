# WellArchitected module

> [Index](../README.md) > WellArchitected


!!! note ""

    Auto-generated documentation for [WellArchitected](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#wellarchitected)
    type annotations stubs module [types-aiobotocore-wellarchitected](https://pypi.org/project/types-aiobotocore-wellarchitected/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `WellArchitected` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `WellArchitected` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[wellarchitected]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[wellarchitected]'

# standalone installation
python -m pip install types-aiobotocore-wellarchitected
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-wellarchitected
```

## Usage

Code samples can be found in [Examples](./usage.md).

## WellArchitectedClient

Type annotations and code completion for  `#!python session.create_client("wellarchitected")` as [WellArchitectedClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client)

```python
# WellArchitectedClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_wellarchitected.client import WellArchitectedClient


session = get_session()
async with session.create_client("wellarchitected") as client:
    client: WellArchitectedClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccountJiraIssueManagementStatusType usage example

from types_aiobotocore_wellarchitected.literals import AccountJiraIssueManagementStatusType

def get_value() -> AccountJiraIssueManagementStatusType:
    return "DISABLED"
```

- [AccountJiraIssueManagementStatusType](./literals.md#accountjiraissuemanagementstatustype)
- [AdditionalResourceTypeType](./literals.md#additionalresourcetypetype)
- [AnswerReasonType](./literals.md#answerreasontype)
- [CheckFailureReasonType](./literals.md#checkfailurereasontype)
- [CheckProviderType](./literals.md#checkprovidertype)
- [CheckStatusType](./literals.md#checkstatustype)
- [ChoiceReasonType](./literals.md#choicereasontype)
- [ChoiceStatusType](./literals.md#choicestatustype)
- [DefinitionTypeType](./literals.md#definitiontypetype)
- [DifferenceStatusType](./literals.md#differencestatustype)
- [DiscoveryIntegrationStatusType](./literals.md#discoveryintegrationstatustype)
- [ImportLensStatusType](./literals.md#importlensstatustype)
- [IntegratingServiceType](./literals.md#integratingservicetype)
- [IntegrationStatusInputType](./literals.md#integrationstatusinputtype)
- [IntegrationStatusType](./literals.md#integrationstatustype)
- [IssueManagementTypeType](./literals.md#issuemanagementtypetype)
- [LensStatusType](./literals.md#lensstatustype)
- [LensStatusTypeType](./literals.md#lensstatustypetype)
- [LensTypeType](./literals.md#lenstypetype)
- [MetricTypeType](./literals.md#metrictypetype)
- [NotificationTypeType](./literals.md#notificationtypetype)
- [OrganizationSharingStatusType](./literals.md#organizationsharingstatustype)
- [PermissionTypeType](./literals.md#permissiontypetype)
- [ProfileNotificationTypeType](./literals.md#profilenotificationtypetype)
- [ProfileOwnerTypeType](./literals.md#profileownertypetype)
- [QuestionPriorityType](./literals.md#questionprioritytype)
- [QuestionType](./literals.md#questiontype)
- [QuestionTypeType](./literals.md#questiontypetype)
- [ReportFormatType](./literals.md#reportformattype)
- [ReviewTemplateAnswerStatusType](./literals.md#reviewtemplateanswerstatustype)
- [ReviewTemplateUpdateStatusType](./literals.md#reviewtemplateupdatestatustype)
- [RiskType](./literals.md#risktype)
- [ShareInvitationActionType](./literals.md#shareinvitationactiontype)
- [ShareResourceTypeType](./literals.md#shareresourcetypetype)
- [ShareStatusType](./literals.md#sharestatustype)
- [TrustedAdvisorIntegrationStatusType](./literals.md#trustedadvisorintegrationstatustype)
- [WorkloadEnvironmentType](./literals.md#workloadenvironmenttype)
- [WorkloadImprovementStatusType](./literals.md#workloadimprovementstatustype)
- [WorkloadIssueManagementStatusType](./literals.md#workloadissuemanagementstatustype)
- [WellArchitectedServiceName](./literals.md#wellarchitectedservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccountJiraConfigurationInputTypeDef](./type_defs.md#accountjiraconfigurationinputtypedef)
- [AccountJiraConfigurationOutputTypeDef](./type_defs.md#accountjiraconfigurationoutputtypedef)
- [ChoiceContentTypeDef](./type_defs.md#choicecontenttypedef)
- [ChoiceAnswerSummaryTypeDef](./type_defs.md#choiceanswersummarytypedef)
- [JiraConfigurationTypeDef](./type_defs.md#jiraconfigurationtypedef)
- [ChoiceAnswerTypeDef](./type_defs.md#choiceanswertypedef)
- [AssociateLensesInputTypeDef](./type_defs.md#associatelensesinputtypedef)
- [AssociateProfilesInputTypeDef](./type_defs.md#associateprofilesinputtypedef)
- [BestPracticeTypeDef](./type_defs.md#bestpracticetypedef)
- [CheckDetailTypeDef](./type_defs.md#checkdetailtypedef)
- [CheckSummaryTypeDef](./type_defs.md#checksummarytypedef)
- [ChoiceImprovementPlanTypeDef](./type_defs.md#choiceimprovementplantypedef)
- [ChoiceUpdateTypeDef](./type_defs.md#choiceupdatetypedef)
- [CreateLensShareInputTypeDef](./type_defs.md#createlensshareinputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateLensVersionInputTypeDef](./type_defs.md#createlensversioninputtypedef)
- [CreateMilestoneInputTypeDef](./type_defs.md#createmilestoneinputtypedef)
- [ProfileQuestionUpdateTypeDef](./type_defs.md#profilequestionupdatetypedef)
- [CreateProfileShareInputTypeDef](./type_defs.md#createprofileshareinputtypedef)
- [CreateReviewTemplateInputTypeDef](./type_defs.md#createreviewtemplateinputtypedef)
- [CreateTemplateShareInputTypeDef](./type_defs.md#createtemplateshareinputtypedef)
- [WorkloadJiraConfigurationInputTypeDef](./type_defs.md#workloadjiraconfigurationinputtypedef)
- [CreateWorkloadShareInputTypeDef](./type_defs.md#createworkloadshareinputtypedef)
- [DeleteLensInputTypeDef](./type_defs.md#deletelensinputtypedef)
- [DeleteLensShareInputTypeDef](./type_defs.md#deletelensshareinputtypedef)
- [DeleteProfileInputTypeDef](./type_defs.md#deleteprofileinputtypedef)
- [DeleteProfileShareInputTypeDef](./type_defs.md#deleteprofileshareinputtypedef)
- [DeleteReviewTemplateInputTypeDef](./type_defs.md#deletereviewtemplateinputtypedef)
- [DeleteTemplateShareInputTypeDef](./type_defs.md#deletetemplateshareinputtypedef)
- [DeleteWorkloadInputTypeDef](./type_defs.md#deleteworkloadinputtypedef)
- [DeleteWorkloadShareInputTypeDef](./type_defs.md#deleteworkloadshareinputtypedef)
- [DisassociateLensesInputTypeDef](./type_defs.md#disassociatelensesinputtypedef)
- [DisassociateProfilesInputTypeDef](./type_defs.md#disassociateprofilesinputtypedef)
- [ExportLensInputTypeDef](./type_defs.md#exportlensinputtypedef)
- [GetAnswerInputTypeDef](./type_defs.md#getanswerinputtypedef)
- [GetConsolidatedReportInputTypeDef](./type_defs.md#getconsolidatedreportinputtypedef)
- [GetLensInputTypeDef](./type_defs.md#getlensinputtypedef)
- [LensTypeDef](./type_defs.md#lenstypedef)
- [GetLensReviewInputTypeDef](./type_defs.md#getlensreviewinputtypedef)
- [GetLensReviewReportInputTypeDef](./type_defs.md#getlensreviewreportinputtypedef)
- [LensReviewReportTypeDef](./type_defs.md#lensreviewreporttypedef)
- [GetLensVersionDifferenceInputTypeDef](./type_defs.md#getlensversiondifferenceinputtypedef)
- [GetMilestoneInputTypeDef](./type_defs.md#getmilestoneinputtypedef)
- [GetProfileInputTypeDef](./type_defs.md#getprofileinputtypedef)
- [GetReviewTemplateAnswerInputTypeDef](./type_defs.md#getreviewtemplateanswerinputtypedef)
- [GetReviewTemplateInputTypeDef](./type_defs.md#getreviewtemplateinputtypedef)
- [GetReviewTemplateLensReviewInputTypeDef](./type_defs.md#getreviewtemplatelensreviewinputtypedef)
- [ReviewTemplateTypeDef](./type_defs.md#reviewtemplatetypedef)
- [GetWorkloadInputTypeDef](./type_defs.md#getworkloadinputtypedef)
- [ImportLensInputTypeDef](./type_defs.md#importlensinputtypedef)
- [SelectedPillarOutputTypeDef](./type_defs.md#selectedpillaroutputtypedef)
- [SelectedPillarTypeDef](./type_defs.md#selectedpillartypedef)
- [WorkloadProfileTypeDef](./type_defs.md#workloadprofiletypedef)
- [PillarReviewSummaryTypeDef](./type_defs.md#pillarreviewsummarytypedef)
- [LensShareSummaryTypeDef](./type_defs.md#lenssharesummarytypedef)
- [LensSummaryTypeDef](./type_defs.md#lenssummarytypedef)
- [LensUpgradeSummaryTypeDef](./type_defs.md#lensupgradesummarytypedef)
- [ListAnswersInputTypeDef](./type_defs.md#listanswersinputtypedef)
- [ListCheckDetailsInputTypeDef](./type_defs.md#listcheckdetailsinputtypedef)
- [ListCheckSummariesInputTypeDef](./type_defs.md#listchecksummariesinputtypedef)
- [ListLensReviewImprovementsInputTypeDef](./type_defs.md#listlensreviewimprovementsinputtypedef)
- [ListLensReviewsInputTypeDef](./type_defs.md#listlensreviewsinputtypedef)
- [ListLensSharesInputTypeDef](./type_defs.md#listlenssharesinputtypedef)
- [ListLensesInputTypeDef](./type_defs.md#listlensesinputtypedef)
- [ListMilestonesInputTypeDef](./type_defs.md#listmilestonesinputtypedef)
- [ListNotificationsInputTypeDef](./type_defs.md#listnotificationsinputtypedef)
- [ListProfileNotificationsInputTypeDef](./type_defs.md#listprofilenotificationsinputtypedef)
- [ProfileNotificationSummaryTypeDef](./type_defs.md#profilenotificationsummarytypedef)
- [ListProfileSharesInputTypeDef](./type_defs.md#listprofilesharesinputtypedef)
- [ProfileShareSummaryTypeDef](./type_defs.md#profilesharesummarytypedef)
- [ListProfilesInputTypeDef](./type_defs.md#listprofilesinputtypedef)
- [ProfileSummaryTypeDef](./type_defs.md#profilesummarytypedef)
- [ListReviewTemplateAnswersInputTypeDef](./type_defs.md#listreviewtemplateanswersinputtypedef)
- [ListReviewTemplatesInputTypeDef](./type_defs.md#listreviewtemplatesinputtypedef)
- [ReviewTemplateSummaryTypeDef](./type_defs.md#reviewtemplatesummarytypedef)
- [ListShareInvitationsInputTypeDef](./type_defs.md#listshareinvitationsinputtypedef)
- [ShareInvitationSummaryTypeDef](./type_defs.md#shareinvitationsummarytypedef)
- [ListTagsForResourceInputTypeDef](./type_defs.md#listtagsforresourceinputtypedef)
- [ListTemplateSharesInputTypeDef](./type_defs.md#listtemplatesharesinputtypedef)
- [TemplateShareSummaryTypeDef](./type_defs.md#templatesharesummarytypedef)
- [ListWorkloadSharesInputTypeDef](./type_defs.md#listworkloadsharesinputtypedef)
- [WorkloadShareSummaryTypeDef](./type_defs.md#workloadsharesummarytypedef)
- [ListWorkloadsInputTypeDef](./type_defs.md#listworkloadsinputtypedef)
- [QuestionDifferenceTypeDef](./type_defs.md#questiondifferencetypedef)
- [ProfileChoiceTypeDef](./type_defs.md#profilechoicetypedef)
- [ProfileTemplateChoiceTypeDef](./type_defs.md#profiletemplatechoicetypedef)
- [ReviewTemplatePillarReviewSummaryTypeDef](./type_defs.md#reviewtemplatepillarreviewsummarytypedef)
- [ShareInvitationTypeDef](./type_defs.md#shareinvitationtypedef)
- [TagResourceInputTypeDef](./type_defs.md#tagresourceinputtypedef)
- [UntagResourceInputTypeDef](./type_defs.md#untagresourceinputtypedef)
- [UpdateIntegrationInputTypeDef](./type_defs.md#updateintegrationinputtypedef)
- [UpdateReviewTemplateInputTypeDef](./type_defs.md#updatereviewtemplateinputtypedef)
- [UpdateReviewTemplateLensReviewInputTypeDef](./type_defs.md#updatereviewtemplatelensreviewinputtypedef)
- [UpdateShareInvitationInputTypeDef](./type_defs.md#updateshareinvitationinputtypedef)
- [UpdateWorkloadShareInputTypeDef](./type_defs.md#updateworkloadshareinputtypedef)
- [WorkloadShareTypeDef](./type_defs.md#workloadsharetypedef)
- [UpgradeLensReviewInputTypeDef](./type_defs.md#upgradelensreviewinputtypedef)
- [UpgradeProfileVersionInputTypeDef](./type_defs.md#upgradeprofileversioninputtypedef)
- [UpgradeReviewTemplateLensReviewInputTypeDef](./type_defs.md#upgradereviewtemplatelensreviewinputtypedef)
- [WorkloadDiscoveryConfigOutputTypeDef](./type_defs.md#workloaddiscoveryconfigoutputtypedef)
- [WorkloadDiscoveryConfigTypeDef](./type_defs.md#workloaddiscoveryconfigtypedef)
- [WorkloadJiraConfigurationOutputTypeDef](./type_defs.md#workloadjiraconfigurationoutputtypedef)
- [UpdateGlobalSettingsInputTypeDef](./type_defs.md#updateglobalsettingsinputtypedef)
- [AdditionalResourcesTypeDef](./type_defs.md#additionalresourcestypedef)
- [QuestionMetricTypeDef](./type_defs.md#questionmetrictypedef)
- [ImprovementSummaryTypeDef](./type_defs.md#improvementsummarytypedef)
- [UpdateAnswerInputTypeDef](./type_defs.md#updateanswerinputtypedef)
- [UpdateReviewTemplateAnswerInputTypeDef](./type_defs.md#updatereviewtemplateanswerinputtypedef)
- [CreateLensShareOutputTypeDef](./type_defs.md#createlensshareoutputtypedef)
- [CreateLensVersionOutputTypeDef](./type_defs.md#createlensversionoutputtypedef)
- [CreateMilestoneOutputTypeDef](./type_defs.md#createmilestoneoutputtypedef)
- [CreateProfileOutputTypeDef](./type_defs.md#createprofileoutputtypedef)
- [CreateProfileShareOutputTypeDef](./type_defs.md#createprofileshareoutputtypedef)
- [CreateReviewTemplateOutputTypeDef](./type_defs.md#createreviewtemplateoutputtypedef)
- [CreateTemplateShareOutputTypeDef](./type_defs.md#createtemplateshareoutputtypedef)
- [CreateWorkloadOutputTypeDef](./type_defs.md#createworkloadoutputtypedef)
- [CreateWorkloadShareOutputTypeDef](./type_defs.md#createworkloadshareoutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ExportLensOutputTypeDef](./type_defs.md#exportlensoutputtypedef)
- [GetGlobalSettingsOutputTypeDef](./type_defs.md#getglobalsettingsoutputtypedef)
- [ImportLensOutputTypeDef](./type_defs.md#importlensoutputtypedef)
- [ListCheckDetailsOutputTypeDef](./type_defs.md#listcheckdetailsoutputtypedef)
- [ListCheckSummariesOutputTypeDef](./type_defs.md#listchecksummariesoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [CreateProfileInputTypeDef](./type_defs.md#createprofileinputtypedef)
- [UpdateProfileInputTypeDef](./type_defs.md#updateprofileinputtypedef)
- [GetLensOutputTypeDef](./type_defs.md#getlensoutputtypedef)
- [GetLensReviewReportOutputTypeDef](./type_defs.md#getlensreviewreportoutputtypedef)
- [GetReviewTemplateOutputTypeDef](./type_defs.md#getreviewtemplateoutputtypedef)
- [UpdateReviewTemplateOutputTypeDef](./type_defs.md#updatereviewtemplateoutputtypedef)
- [JiraSelectedQuestionConfigurationOutputTypeDef](./type_defs.md#jiraselectedquestionconfigurationoutputtypedef)
- [JiraSelectedQuestionConfigurationTypeDef](./type_defs.md#jiraselectedquestionconfigurationtypedef)
- [LensReviewSummaryTypeDef](./type_defs.md#lensreviewsummarytypedef)
- [WorkloadSummaryTypeDef](./type_defs.md#workloadsummarytypedef)
- [ListLensSharesOutputTypeDef](./type_defs.md#listlenssharesoutputtypedef)
- [ListLensesOutputTypeDef](./type_defs.md#listlensesoutputtypedef)
- [NotificationSummaryTypeDef](./type_defs.md#notificationsummarytypedef)
- [ListProfileNotificationsOutputTypeDef](./type_defs.md#listprofilenotificationsoutputtypedef)
- [ListProfileSharesOutputTypeDef](./type_defs.md#listprofilesharesoutputtypedef)
- [ListProfilesOutputTypeDef](./type_defs.md#listprofilesoutputtypedef)
- [ListReviewTemplatesOutputTypeDef](./type_defs.md#listreviewtemplatesoutputtypedef)
- [ListShareInvitationsOutputTypeDef](./type_defs.md#listshareinvitationsoutputtypedef)
- [ListTemplateSharesOutputTypeDef](./type_defs.md#listtemplatesharesoutputtypedef)
- [ListWorkloadSharesOutputTypeDef](./type_defs.md#listworkloadsharesoutputtypedef)
- [PillarDifferenceTypeDef](./type_defs.md#pillardifferencetypedef)
- [ProfileQuestionTypeDef](./type_defs.md#profilequestiontypedef)
- [ProfileTemplateQuestionTypeDef](./type_defs.md#profiletemplatequestiontypedef)
- [ReviewTemplateLensReviewTypeDef](./type_defs.md#reviewtemplatelensreviewtypedef)
- [UpdateShareInvitationOutputTypeDef](./type_defs.md#updateshareinvitationoutputtypedef)
- [UpdateWorkloadShareOutputTypeDef](./type_defs.md#updateworkloadshareoutputtypedef)
- [WorkloadDiscoveryConfigUnionTypeDef](./type_defs.md#workloaddiscoveryconfiguniontypedef)
- [WorkloadTypeDef](./type_defs.md#workloadtypedef)
- [ChoiceTypeDef](./type_defs.md#choicetypedef)
- [PillarMetricTypeDef](./type_defs.md#pillarmetrictypedef)
- [ListLensReviewImprovementsOutputTypeDef](./type_defs.md#listlensreviewimprovementsoutputtypedef)
- [LensReviewTypeDef](./type_defs.md#lensreviewtypedef)
- [JiraSelectedQuestionConfigurationUnionTypeDef](./type_defs.md#jiraselectedquestionconfigurationuniontypedef)
- [ListLensReviewsOutputTypeDef](./type_defs.md#listlensreviewsoutputtypedef)
- [ListWorkloadsOutputTypeDef](./type_defs.md#listworkloadsoutputtypedef)
- [MilestoneSummaryTypeDef](./type_defs.md#milestonesummarytypedef)
- [ListNotificationsOutputTypeDef](./type_defs.md#listnotificationsoutputtypedef)
- [VersionDifferencesTypeDef](./type_defs.md#versiondifferencestypedef)
- [ProfileTypeDef](./type_defs.md#profiletypedef)
- [ProfileTemplateTypeDef](./type_defs.md#profiletemplatetypedef)
- [GetReviewTemplateLensReviewOutputTypeDef](./type_defs.md#getreviewtemplatelensreviewoutputtypedef)
- [UpdateReviewTemplateLensReviewOutputTypeDef](./type_defs.md#updatereviewtemplatelensreviewoutputtypedef)
- [CreateWorkloadInputTypeDef](./type_defs.md#createworkloadinputtypedef)
- [UpdateWorkloadInputTypeDef](./type_defs.md#updateworkloadinputtypedef)
- [GetWorkloadOutputTypeDef](./type_defs.md#getworkloadoutputtypedef)
- [MilestoneTypeDef](./type_defs.md#milestonetypedef)
- [UpdateWorkloadOutputTypeDef](./type_defs.md#updateworkloadoutputtypedef)
- [AnswerSummaryTypeDef](./type_defs.md#answersummarytypedef)
- [AnswerTypeDef](./type_defs.md#answertypedef)
- [ReviewTemplateAnswerSummaryTypeDef](./type_defs.md#reviewtemplateanswersummarytypedef)
- [ReviewTemplateAnswerTypeDef](./type_defs.md#reviewtemplateanswertypedef)
- [LensMetricTypeDef](./type_defs.md#lensmetrictypedef)
- [GetLensReviewOutputTypeDef](./type_defs.md#getlensreviewoutputtypedef)
- [UpdateLensReviewOutputTypeDef](./type_defs.md#updatelensreviewoutputtypedef)
- [UpdateLensReviewInputTypeDef](./type_defs.md#updatelensreviewinputtypedef)
- [ListMilestonesOutputTypeDef](./type_defs.md#listmilestonesoutputtypedef)
- [GetLensVersionDifferenceOutputTypeDef](./type_defs.md#getlensversiondifferenceoutputtypedef)
- [GetProfileOutputTypeDef](./type_defs.md#getprofileoutputtypedef)
- [UpdateProfileOutputTypeDef](./type_defs.md#updateprofileoutputtypedef)
- [GetProfileTemplateOutputTypeDef](./type_defs.md#getprofiletemplateoutputtypedef)
- [GetMilestoneOutputTypeDef](./type_defs.md#getmilestoneoutputtypedef)
- [ListAnswersOutputTypeDef](./type_defs.md#listanswersoutputtypedef)
- [GetAnswerOutputTypeDef](./type_defs.md#getansweroutputtypedef)
- [UpdateAnswerOutputTypeDef](./type_defs.md#updateansweroutputtypedef)
- [ListReviewTemplateAnswersOutputTypeDef](./type_defs.md#listreviewtemplateanswersoutputtypedef)
- [GetReviewTemplateAnswerOutputTypeDef](./type_defs.md#getreviewtemplateansweroutputtypedef)
- [UpdateReviewTemplateAnswerOutputTypeDef](./type_defs.md#updatereviewtemplateansweroutputtypedef)
- [ConsolidatedReportMetricTypeDef](./type_defs.md#consolidatedreportmetrictypedef)
- [GetConsolidatedReportOutputTypeDef](./type_defs.md#getconsolidatedreportoutputtypedef)

