# WellArchitected module

> [Index](../README.md) > WellArchitected


!!! note ""

    Auto-generated documentation for [WellArchitected](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#wellarchitected)
    type annotations stubs module [types-aiobotocore-wellarchitected](https://pypi.org/project/types-aiobotocore-wellarchitected/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
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
- [AssociateLensesInputRequestTypeDef](./type_defs.md#associatelensesinputrequesttypedef)
- [AssociateProfilesInputRequestTypeDef](./type_defs.md#associateprofilesinputrequesttypedef)
- [BestPracticeTypeDef](./type_defs.md#bestpracticetypedef)
- [CheckDetailTypeDef](./type_defs.md#checkdetailtypedef)
- [CheckSummaryTypeDef](./type_defs.md#checksummarytypedef)
- [ChoiceImprovementPlanTypeDef](./type_defs.md#choiceimprovementplantypedef)
- [ChoiceUpdateTypeDef](./type_defs.md#choiceupdatetypedef)
- [CreateLensShareInputRequestTypeDef](./type_defs.md#createlensshareinputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateLensVersionInputRequestTypeDef](./type_defs.md#createlensversioninputrequesttypedef)
- [CreateMilestoneInputRequestTypeDef](./type_defs.md#createmilestoneinputrequesttypedef)
- [ProfileQuestionUpdateTypeDef](./type_defs.md#profilequestionupdatetypedef)
- [CreateProfileShareInputRequestTypeDef](./type_defs.md#createprofileshareinputrequesttypedef)
- [CreateReviewTemplateInputRequestTypeDef](./type_defs.md#createreviewtemplateinputrequesttypedef)
- [CreateTemplateShareInputRequestTypeDef](./type_defs.md#createtemplateshareinputrequesttypedef)
- [WorkloadDiscoveryConfigTypeDef](./type_defs.md#workloaddiscoveryconfigtypedef)
- [WorkloadJiraConfigurationInputTypeDef](./type_defs.md#workloadjiraconfigurationinputtypedef)
- [CreateWorkloadShareInputRequestTypeDef](./type_defs.md#createworkloadshareinputrequesttypedef)
- [DeleteLensInputRequestTypeDef](./type_defs.md#deletelensinputrequesttypedef)
- [DeleteLensShareInputRequestTypeDef](./type_defs.md#deletelensshareinputrequesttypedef)
- [DeleteProfileInputRequestTypeDef](./type_defs.md#deleteprofileinputrequesttypedef)
- [DeleteProfileShareInputRequestTypeDef](./type_defs.md#deleteprofileshareinputrequesttypedef)
- [DeleteReviewTemplateInputRequestTypeDef](./type_defs.md#deletereviewtemplateinputrequesttypedef)
- [DeleteTemplateShareInputRequestTypeDef](./type_defs.md#deletetemplateshareinputrequesttypedef)
- [DeleteWorkloadInputRequestTypeDef](./type_defs.md#deleteworkloadinputrequesttypedef)
- [DeleteWorkloadShareInputRequestTypeDef](./type_defs.md#deleteworkloadshareinputrequesttypedef)
- [DisassociateLensesInputRequestTypeDef](./type_defs.md#disassociatelensesinputrequesttypedef)
- [DisassociateProfilesInputRequestTypeDef](./type_defs.md#disassociateprofilesinputrequesttypedef)
- [ExportLensInputRequestTypeDef](./type_defs.md#exportlensinputrequesttypedef)
- [GetAnswerInputRequestTypeDef](./type_defs.md#getanswerinputrequesttypedef)
- [GetConsolidatedReportInputRequestTypeDef](./type_defs.md#getconsolidatedreportinputrequesttypedef)
- [GetLensInputRequestTypeDef](./type_defs.md#getlensinputrequesttypedef)
- [LensTypeDef](./type_defs.md#lenstypedef)
- [GetLensReviewInputRequestTypeDef](./type_defs.md#getlensreviewinputrequesttypedef)
- [GetLensReviewReportInputRequestTypeDef](./type_defs.md#getlensreviewreportinputrequesttypedef)
- [LensReviewReportTypeDef](./type_defs.md#lensreviewreporttypedef)
- [GetLensVersionDifferenceInputRequestTypeDef](./type_defs.md#getlensversiondifferenceinputrequesttypedef)
- [GetMilestoneInputRequestTypeDef](./type_defs.md#getmilestoneinputrequesttypedef)
- [GetProfileInputRequestTypeDef](./type_defs.md#getprofileinputrequesttypedef)
- [GetReviewTemplateAnswerInputRequestTypeDef](./type_defs.md#getreviewtemplateanswerinputrequesttypedef)
- [GetReviewTemplateInputRequestTypeDef](./type_defs.md#getreviewtemplateinputrequesttypedef)
- [GetReviewTemplateLensReviewInputRequestTypeDef](./type_defs.md#getreviewtemplatelensreviewinputrequesttypedef)
- [ReviewTemplateTypeDef](./type_defs.md#reviewtemplatetypedef)
- [GetWorkloadInputRequestTypeDef](./type_defs.md#getworkloadinputrequesttypedef)
- [ImportLensInputRequestTypeDef](./type_defs.md#importlensinputrequesttypedef)
- [SelectedPillarOutputTypeDef](./type_defs.md#selectedpillaroutputtypedef)
- [WorkloadProfileTypeDef](./type_defs.md#workloadprofiletypedef)
- [PillarReviewSummaryTypeDef](./type_defs.md#pillarreviewsummarytypedef)
- [LensShareSummaryTypeDef](./type_defs.md#lenssharesummarytypedef)
- [LensSummaryTypeDef](./type_defs.md#lenssummarytypedef)
- [LensUpgradeSummaryTypeDef](./type_defs.md#lensupgradesummarytypedef)
- [ListAnswersInputRequestTypeDef](./type_defs.md#listanswersinputrequesttypedef)
- [ListCheckDetailsInputRequestTypeDef](./type_defs.md#listcheckdetailsinputrequesttypedef)
- [ListCheckSummariesInputRequestTypeDef](./type_defs.md#listchecksummariesinputrequesttypedef)
- [ListLensReviewImprovementsInputRequestTypeDef](./type_defs.md#listlensreviewimprovementsinputrequesttypedef)
- [ListLensReviewsInputRequestTypeDef](./type_defs.md#listlensreviewsinputrequesttypedef)
- [ListLensSharesInputRequestTypeDef](./type_defs.md#listlenssharesinputrequesttypedef)
- [ListLensesInputRequestTypeDef](./type_defs.md#listlensesinputrequesttypedef)
- [ListMilestonesInputRequestTypeDef](./type_defs.md#listmilestonesinputrequesttypedef)
- [ListNotificationsInputRequestTypeDef](./type_defs.md#listnotificationsinputrequesttypedef)
- [ListProfileNotificationsInputRequestTypeDef](./type_defs.md#listprofilenotificationsinputrequesttypedef)
- [ProfileNotificationSummaryTypeDef](./type_defs.md#profilenotificationsummarytypedef)
- [ListProfileSharesInputRequestTypeDef](./type_defs.md#listprofilesharesinputrequesttypedef)
- [ProfileShareSummaryTypeDef](./type_defs.md#profilesharesummarytypedef)
- [ListProfilesInputRequestTypeDef](./type_defs.md#listprofilesinputrequesttypedef)
- [ProfileSummaryTypeDef](./type_defs.md#profilesummarytypedef)
- [ListReviewTemplateAnswersInputRequestTypeDef](./type_defs.md#listreviewtemplateanswersinputrequesttypedef)
- [ListReviewTemplatesInputRequestTypeDef](./type_defs.md#listreviewtemplatesinputrequesttypedef)
- [ReviewTemplateSummaryTypeDef](./type_defs.md#reviewtemplatesummarytypedef)
- [ListShareInvitationsInputRequestTypeDef](./type_defs.md#listshareinvitationsinputrequesttypedef)
- [ShareInvitationSummaryTypeDef](./type_defs.md#shareinvitationsummarytypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [ListTemplateSharesInputRequestTypeDef](./type_defs.md#listtemplatesharesinputrequesttypedef)
- [TemplateShareSummaryTypeDef](./type_defs.md#templatesharesummarytypedef)
- [ListWorkloadSharesInputRequestTypeDef](./type_defs.md#listworkloadsharesinputrequesttypedef)
- [WorkloadShareSummaryTypeDef](./type_defs.md#workloadsharesummarytypedef)
- [ListWorkloadsInputRequestTypeDef](./type_defs.md#listworkloadsinputrequesttypedef)
- [QuestionDifferenceTypeDef](./type_defs.md#questiondifferencetypedef)
- [ProfileChoiceTypeDef](./type_defs.md#profilechoicetypedef)
- [ProfileTemplateChoiceTypeDef](./type_defs.md#profiletemplatechoicetypedef)
- [ReviewTemplatePillarReviewSummaryTypeDef](./type_defs.md#reviewtemplatepillarreviewsummarytypedef)
- [SelectedPillarTypeDef](./type_defs.md#selectedpillartypedef)
- [ShareInvitationTypeDef](./type_defs.md#shareinvitationtypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [UpdateIntegrationInputRequestTypeDef](./type_defs.md#updateintegrationinputrequesttypedef)
- [UpdateReviewTemplateInputRequestTypeDef](./type_defs.md#updatereviewtemplateinputrequesttypedef)
- [UpdateReviewTemplateLensReviewInputRequestTypeDef](./type_defs.md#updatereviewtemplatelensreviewinputrequesttypedef)
- [UpdateShareInvitationInputRequestTypeDef](./type_defs.md#updateshareinvitationinputrequesttypedef)
- [UpdateWorkloadShareInputRequestTypeDef](./type_defs.md#updateworkloadshareinputrequesttypedef)
- [WorkloadShareTypeDef](./type_defs.md#workloadsharetypedef)
- [UpgradeLensReviewInputRequestTypeDef](./type_defs.md#upgradelensreviewinputrequesttypedef)
- [UpgradeProfileVersionInputRequestTypeDef](./type_defs.md#upgradeprofileversioninputrequesttypedef)
- [UpgradeReviewTemplateLensReviewInputRequestTypeDef](./type_defs.md#upgradereviewtemplatelensreviewinputrequesttypedef)
- [WorkloadDiscoveryConfigOutputTypeDef](./type_defs.md#workloaddiscoveryconfigoutputtypedef)
- [WorkloadJiraConfigurationOutputTypeDef](./type_defs.md#workloadjiraconfigurationoutputtypedef)
- [UpdateGlobalSettingsInputRequestTypeDef](./type_defs.md#updateglobalsettingsinputrequesttypedef)
- [AdditionalResourcesTypeDef](./type_defs.md#additionalresourcestypedef)
- [QuestionMetricTypeDef](./type_defs.md#questionmetrictypedef)
- [ImprovementSummaryTypeDef](./type_defs.md#improvementsummarytypedef)
- [UpdateAnswerInputRequestTypeDef](./type_defs.md#updateanswerinputrequesttypedef)
- [UpdateReviewTemplateAnswerInputRequestTypeDef](./type_defs.md#updatereviewtemplateanswerinputrequesttypedef)
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
- [CreateProfileInputRequestTypeDef](./type_defs.md#createprofileinputrequesttypedef)
- [UpdateProfileInputRequestTypeDef](./type_defs.md#updateprofileinputrequesttypedef)
- [CreateWorkloadInputRequestTypeDef](./type_defs.md#createworkloadinputrequesttypedef)
- [UpdateWorkloadInputRequestTypeDef](./type_defs.md#updateworkloadinputrequesttypedef)
- [GetLensOutputTypeDef](./type_defs.md#getlensoutputtypedef)
- [GetLensReviewReportOutputTypeDef](./type_defs.md#getlensreviewreportoutputtypedef)
- [GetReviewTemplateOutputTypeDef](./type_defs.md#getreviewtemplateoutputtypedef)
- [UpdateReviewTemplateOutputTypeDef](./type_defs.md#updatereviewtemplateoutputtypedef)
- [JiraSelectedQuestionConfigurationOutputTypeDef](./type_defs.md#jiraselectedquestionconfigurationoutputtypedef)
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
- [SelectedPillarUnionTypeDef](./type_defs.md#selectedpillaruniontypedef)
- [UpdateShareInvitationOutputTypeDef](./type_defs.md#updateshareinvitationoutputtypedef)
- [UpdateWorkloadShareOutputTypeDef](./type_defs.md#updateworkloadshareoutputtypedef)
- [WorkloadTypeDef](./type_defs.md#workloadtypedef)
- [ChoiceTypeDef](./type_defs.md#choicetypedef)
- [PillarMetricTypeDef](./type_defs.md#pillarmetrictypedef)
- [ListLensReviewImprovementsOutputTypeDef](./type_defs.md#listlensreviewimprovementsoutputtypedef)
- [LensReviewTypeDef](./type_defs.md#lensreviewtypedef)
- [ListLensReviewsOutputTypeDef](./type_defs.md#listlensreviewsoutputtypedef)
- [ListWorkloadsOutputTypeDef](./type_defs.md#listworkloadsoutputtypedef)
- [MilestoneSummaryTypeDef](./type_defs.md#milestonesummarytypedef)
- [ListNotificationsOutputTypeDef](./type_defs.md#listnotificationsoutputtypedef)
- [VersionDifferencesTypeDef](./type_defs.md#versiondifferencestypedef)
- [ProfileTypeDef](./type_defs.md#profiletypedef)
- [ProfileTemplateTypeDef](./type_defs.md#profiletemplatetypedef)
- [GetReviewTemplateLensReviewOutputTypeDef](./type_defs.md#getreviewtemplatelensreviewoutputtypedef)
- [UpdateReviewTemplateLensReviewOutputTypeDef](./type_defs.md#updatereviewtemplatelensreviewoutputtypedef)
- [JiraSelectedQuestionConfigurationTypeDef](./type_defs.md#jiraselectedquestionconfigurationtypedef)
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
- [ListMilestonesOutputTypeDef](./type_defs.md#listmilestonesoutputtypedef)
- [GetLensVersionDifferenceOutputTypeDef](./type_defs.md#getlensversiondifferenceoutputtypedef)
- [GetProfileOutputTypeDef](./type_defs.md#getprofileoutputtypedef)
- [UpdateProfileOutputTypeDef](./type_defs.md#updateprofileoutputtypedef)
- [GetProfileTemplateOutputTypeDef](./type_defs.md#getprofiletemplateoutputtypedef)
- [UpdateLensReviewInputRequestTypeDef](./type_defs.md#updatelensreviewinputrequesttypedef)
- [GetMilestoneOutputTypeDef](./type_defs.md#getmilestoneoutputtypedef)
- [ListAnswersOutputTypeDef](./type_defs.md#listanswersoutputtypedef)
- [GetAnswerOutputTypeDef](./type_defs.md#getansweroutputtypedef)
- [UpdateAnswerOutputTypeDef](./type_defs.md#updateansweroutputtypedef)
- [ListReviewTemplateAnswersOutputTypeDef](./type_defs.md#listreviewtemplateanswersoutputtypedef)
- [GetReviewTemplateAnswerOutputTypeDef](./type_defs.md#getreviewtemplateansweroutputtypedef)
- [UpdateReviewTemplateAnswerOutputTypeDef](./type_defs.md#updatereviewtemplateansweroutputtypedef)
- [ConsolidatedReportMetricTypeDef](./type_defs.md#consolidatedreportmetrictypedef)
- [GetConsolidatedReportOutputTypeDef](./type_defs.md#getconsolidatedreportoutputtypedef)

