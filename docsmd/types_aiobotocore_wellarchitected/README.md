# WellArchitected module

> [Index](../README.md) > WellArchitected


!!! note ""

    Auto-generated documentation for [WellArchitected](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
    type annotations stubs module [types-aiobotocore-wellarchitected](https://pypi.org/project/types-aiobotocore-wellarchitected/).

## How to install



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
# AdditionalResourceTypeType usage example

from types_aiobotocore_wellarchitected.literals import AdditionalResourceTypeType

def get_value() -> AdditionalResourceTypeType:
    return "HELPFUL_RESOURCE"
```

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
- [QuestionTypeType](./literals.md#questiontypetype)
- [ReportFormatType](./literals.md#reportformattype)
- [RiskType](./literals.md#risktype)
- [ShareInvitationActionType](./literals.md#shareinvitationactiontype)
- [ShareResourceTypeType](./literals.md#shareresourcetypetype)
- [ShareStatusType](./literals.md#sharestatustype)
- [TrustedAdvisorIntegrationStatusType](./literals.md#trustedadvisorintegrationstatustype)
- [WorkloadEnvironmentType](./literals.md#workloadenvironmenttype)
- [WorkloadImprovementStatusType](./literals.md#workloadimprovementstatustype)
- [WellArchitectedServiceName](./literals.md#wellarchitectedservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ChoiceContentTypeDef](./type_defs.md#choicecontenttypedef)
- [ChoiceAnswerSummaryTypeDef](./type_defs.md#choiceanswersummarytypedef)
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
- [WorkloadDiscoveryConfigTypeDef](./type_defs.md#workloaddiscoveryconfigtypedef)
- [CreateWorkloadShareInputRequestTypeDef](./type_defs.md#createworkloadshareinputrequesttypedef)
- [DeleteLensInputRequestTypeDef](./type_defs.md#deletelensinputrequesttypedef)
- [DeleteLensShareInputRequestTypeDef](./type_defs.md#deletelensshareinputrequesttypedef)
- [DeleteProfileInputRequestTypeDef](./type_defs.md#deleteprofileinputrequesttypedef)
- [DeleteProfileShareInputRequestTypeDef](./type_defs.md#deleteprofileshareinputrequesttypedef)
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
- [GetWorkloadInputRequestTypeDef](./type_defs.md#getworkloadinputrequesttypedef)
- [ImportLensInputRequestTypeDef](./type_defs.md#importlensinputrequesttypedef)
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
- [ListShareInvitationsInputRequestTypeDef](./type_defs.md#listshareinvitationsinputrequesttypedef)
- [ShareInvitationSummaryTypeDef](./type_defs.md#shareinvitationsummarytypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [ListWorkloadSharesInputRequestTypeDef](./type_defs.md#listworkloadsharesinputrequesttypedef)
- [WorkloadShareSummaryTypeDef](./type_defs.md#workloadsharesummarytypedef)
- [ListWorkloadsInputRequestTypeDef](./type_defs.md#listworkloadsinputrequesttypedef)
- [QuestionDifferenceTypeDef](./type_defs.md#questiondifferencetypedef)
- [ProfileChoiceTypeDef](./type_defs.md#profilechoicetypedef)
- [ProfileTemplateChoiceTypeDef](./type_defs.md#profiletemplatechoicetypedef)
- [ShareInvitationTypeDef](./type_defs.md#shareinvitationtypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [UpdateGlobalSettingsInputRequestTypeDef](./type_defs.md#updateglobalsettingsinputrequesttypedef)
- [UpdateLensReviewInputRequestTypeDef](./type_defs.md#updatelensreviewinputrequesttypedef)
- [UpdateShareInvitationInputRequestTypeDef](./type_defs.md#updateshareinvitationinputrequesttypedef)
- [UpdateWorkloadShareInputRequestTypeDef](./type_defs.md#updateworkloadshareinputrequesttypedef)
- [WorkloadShareTypeDef](./type_defs.md#workloadsharetypedef)
- [UpgradeLensReviewInputRequestTypeDef](./type_defs.md#upgradelensreviewinputrequesttypedef)
- [UpgradeProfileVersionInputRequestTypeDef](./type_defs.md#upgradeprofileversioninputrequesttypedef)
- [AdditionalResourcesTypeDef](./type_defs.md#additionalresourcestypedef)
- [QuestionMetricTypeDef](./type_defs.md#questionmetrictypedef)
- [ImprovementSummaryTypeDef](./type_defs.md#improvementsummarytypedef)
- [UpdateAnswerInputRequestTypeDef](./type_defs.md#updateanswerinputrequesttypedef)
- [CreateLensShareOutputTypeDef](./type_defs.md#createlensshareoutputtypedef)
- [CreateLensVersionOutputTypeDef](./type_defs.md#createlensversionoutputtypedef)
- [CreateMilestoneOutputTypeDef](./type_defs.md#createmilestoneoutputtypedef)
- [CreateProfileOutputTypeDef](./type_defs.md#createprofileoutputtypedef)
- [CreateProfileShareOutputTypeDef](./type_defs.md#createprofileshareoutputtypedef)
- [CreateWorkloadOutputTypeDef](./type_defs.md#createworkloadoutputtypedef)
- [CreateWorkloadShareOutputTypeDef](./type_defs.md#createworkloadshareoutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ExportLensOutputTypeDef](./type_defs.md#exportlensoutputtypedef)
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
- [LensReviewSummaryTypeDef](./type_defs.md#lensreviewsummarytypedef)
- [WorkloadSummaryTypeDef](./type_defs.md#workloadsummarytypedef)
- [WorkloadTypeDef](./type_defs.md#workloadtypedef)
- [LensReviewTypeDef](./type_defs.md#lensreviewtypedef)
- [ListLensSharesOutputTypeDef](./type_defs.md#listlenssharesoutputtypedef)
- [ListLensesOutputTypeDef](./type_defs.md#listlensesoutputtypedef)
- [NotificationSummaryTypeDef](./type_defs.md#notificationsummarytypedef)
- [ListProfileNotificationsOutputTypeDef](./type_defs.md#listprofilenotificationsoutputtypedef)
- [ListProfileSharesOutputTypeDef](./type_defs.md#listprofilesharesoutputtypedef)
- [ListProfilesOutputTypeDef](./type_defs.md#listprofilesoutputtypedef)
- [ListShareInvitationsOutputTypeDef](./type_defs.md#listshareinvitationsoutputtypedef)
- [ListWorkloadSharesOutputTypeDef](./type_defs.md#listworkloadsharesoutputtypedef)
- [PillarDifferenceTypeDef](./type_defs.md#pillardifferencetypedef)
- [ProfileQuestionTypeDef](./type_defs.md#profilequestiontypedef)
- [ProfileTemplateQuestionTypeDef](./type_defs.md#profiletemplatequestiontypedef)
- [UpdateShareInvitationOutputTypeDef](./type_defs.md#updateshareinvitationoutputtypedef)
- [UpdateWorkloadShareOutputTypeDef](./type_defs.md#updateworkloadshareoutputtypedef)
- [ChoiceTypeDef](./type_defs.md#choicetypedef)
- [PillarMetricTypeDef](./type_defs.md#pillarmetrictypedef)
- [ListLensReviewImprovementsOutputTypeDef](./type_defs.md#listlensreviewimprovementsoutputtypedef)
- [ListLensReviewsOutputTypeDef](./type_defs.md#listlensreviewsoutputtypedef)
- [ListWorkloadsOutputTypeDef](./type_defs.md#listworkloadsoutputtypedef)
- [MilestoneSummaryTypeDef](./type_defs.md#milestonesummarytypedef)
- [GetWorkloadOutputTypeDef](./type_defs.md#getworkloadoutputtypedef)
- [MilestoneTypeDef](./type_defs.md#milestonetypedef)
- [UpdateWorkloadOutputTypeDef](./type_defs.md#updateworkloadoutputtypedef)
- [GetLensReviewOutputTypeDef](./type_defs.md#getlensreviewoutputtypedef)
- [UpdateLensReviewOutputTypeDef](./type_defs.md#updatelensreviewoutputtypedef)
- [ListNotificationsOutputTypeDef](./type_defs.md#listnotificationsoutputtypedef)
- [VersionDifferencesTypeDef](./type_defs.md#versiondifferencestypedef)
- [ProfileTypeDef](./type_defs.md#profiletypedef)
- [ProfileTemplateTypeDef](./type_defs.md#profiletemplatetypedef)
- [AnswerSummaryTypeDef](./type_defs.md#answersummarytypedef)
- [AnswerTypeDef](./type_defs.md#answertypedef)
- [LensMetricTypeDef](./type_defs.md#lensmetrictypedef)
- [ListMilestonesOutputTypeDef](./type_defs.md#listmilestonesoutputtypedef)
- [GetMilestoneOutputTypeDef](./type_defs.md#getmilestoneoutputtypedef)
- [GetLensVersionDifferenceOutputTypeDef](./type_defs.md#getlensversiondifferenceoutputtypedef)
- [GetProfileOutputTypeDef](./type_defs.md#getprofileoutputtypedef)
- [UpdateProfileOutputTypeDef](./type_defs.md#updateprofileoutputtypedef)
- [GetProfileTemplateOutputTypeDef](./type_defs.md#getprofiletemplateoutputtypedef)
- [ListAnswersOutputTypeDef](./type_defs.md#listanswersoutputtypedef)
- [GetAnswerOutputTypeDef](./type_defs.md#getansweroutputtypedef)
- [UpdateAnswerOutputTypeDef](./type_defs.md#updateansweroutputtypedef)
- [ConsolidatedReportMetricTypeDef](./type_defs.md#consolidatedreportmetrictypedef)
- [GetConsolidatedReportOutputTypeDef](./type_defs.md#getconsolidatedreportoutputtypedef)

