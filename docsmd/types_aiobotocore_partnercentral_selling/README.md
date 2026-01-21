# PartnerCentralSellingAPI module

> [Index](../README.md) > PartnerCentralSellingAPI


!!! note ""

    Auto-generated documentation for [PartnerCentralSellingAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#partnercentralsellingapi)
    type annotations stubs module [types-aiobotocore-partnercentral-selling](https://pypi.org/project/types-aiobotocore-partnercentral-selling/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `PartnerCentralSellingAPI` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `PartnerCentralSellingAPI` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[partnercentral-selling]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[partnercentral-selling]'

# standalone installation
python -m pip install types-aiobotocore-partnercentral-selling
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-partnercentral-selling
```

## Usage

Code samples can be found in [Examples](./usage.md).

## PartnerCentralSellingAPIClient

Type annotations and code completion for  `#!python session.create_client("partnercentral-selling")` as [PartnerCentralSellingAPIClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# PartnerCentralSellingAPIClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_selling.client import PartnerCentralSellingAPIClient


session = get_session()
async with session.create_client("partnercentral-selling") as client:
    client: PartnerCentralSellingAPIClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("partnercentral-selling").get_paginator("...")`.

```python
# ListEngagementByAcceptingInvitationTasksPaginator usage example

from types_aiobotocore_partnercentral_selling.paginator import ListEngagementByAcceptingInvitationTasksPaginator

def get_list_engagement_by_accepting_invitation_tasks_paginator() -> ListEngagementByAcceptingInvitationTasksPaginator:
    return client.get_paginator("list_engagement_by_accepting_invitation_tasks"))
```

- [ListEngagementByAcceptingInvitationTasksPaginator](./paginators.md#listengagementbyacceptinginvitationtaskspaginator)
- [ListEngagementFromOpportunityTasksPaginator](./paginators.md#listengagementfromopportunitytaskspaginator)
- [ListEngagementInvitationsPaginator](./paginators.md#listengagementinvitationspaginator)
- [ListEngagementMembersPaginator](./paginators.md#listengagementmemberspaginator)
- [ListEngagementResourceAssociationsPaginator](./paginators.md#listengagementresourceassociationspaginator)
- [ListEngagementsPaginator](./paginators.md#listengagementspaginator)
- [ListOpportunitiesPaginator](./paginators.md#listopportunitiespaginator)
- [ListOpportunityFromEngagementTasksPaginator](./paginators.md#listopportunityfromengagementtaskspaginator)
- [ListResourceSnapshotJobsPaginator](./paginators.md#listresourcesnapshotjobspaginator)
- [ListResourceSnapshotsPaginator](./paginators.md#listresourcesnapshotspaginator)
- [ListSolutionsPaginator](./paginators.md#listsolutionspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AwsClosedLostReasonType usage example

from types_aiobotocore_partnercentral_selling.literals import AwsClosedLostReasonType

def get_value() -> AwsClosedLostReasonType:
    return "Administrative"
```

- [AwsClosedLostReasonType](./literals.md#awsclosedlostreasontype)
- [AwsFundingUsedType](./literals.md#awsfundingusedtype)
- [AwsMemberBusinessTitleType](./literals.md#awsmemberbusinesstitletype)
- [AwsOpportunityStageType](./literals.md#awsopportunitystagetype)
- [AwsPartitionType](./literals.md#awspartitiontype)
- [AwsProductInsightsCurrencyCodeEnumType](./literals.md#awsproductinsightscurrencycodeenumtype)
- [ChannelType](./literals.md#channeltype)
- [ClosedLostReasonType](./literals.md#closedlostreasontype)
- [CompetitorNameType](./literals.md#competitornametype)
- [CountryCodeType](./literals.md#countrycodetype)
- [CurrencyCodeType](./literals.md#currencycodetype)
- [DeliveryModelType](./literals.md#deliverymodeltype)
- [EngagementContextTypeType](./literals.md#engagementcontexttypetype)
- [EngagementInvitationPayloadTypeType](./literals.md#engagementinvitationpayloadtypetype)
- [EngagementScoreType](./literals.md#engagementscoretype)
- [EngagementSortNameType](./literals.md#engagementsortnametype)
- [ExpectedCustomerSpendCurrencyCodeEnumType](./literals.md#expectedcustomerspendcurrencycodeenumtype)
- [IndustryType](./literals.md#industrytype)
- [InvitationStatusType](./literals.md#invitationstatustype)
- [InvolvementTypeChangeReasonType](./literals.md#involvementtypechangereasontype)
- [ListEngagementByAcceptingInvitationTasksPaginatorName](./literals.md#listengagementbyacceptinginvitationtaskspaginatorname)
- [ListEngagementFromOpportunityTasksPaginatorName](./literals.md#listengagementfromopportunitytaskspaginatorname)
- [ListEngagementInvitationsPaginatorName](./literals.md#listengagementinvitationspaginatorname)
- [ListEngagementMembersPaginatorName](./literals.md#listengagementmemberspaginatorname)
- [ListEngagementResourceAssociationsPaginatorName](./literals.md#listengagementresourceassociationspaginatorname)
- [ListEngagementsPaginatorName](./literals.md#listengagementspaginatorname)
- [ListOpportunitiesPaginatorName](./literals.md#listopportunitiespaginatorname)
- [ListOpportunityFromEngagementTasksPaginatorName](./literals.md#listopportunityfromengagementtaskspaginatorname)
- [ListResourceSnapshotJobsPaginatorName](./literals.md#listresourcesnapshotjobspaginatorname)
- [ListResourceSnapshotsPaginatorName](./literals.md#listresourcesnapshotspaginatorname)
- [ListSolutionsPaginatorName](./literals.md#listsolutionspaginatorname)
- [ListTasksSortNameType](./literals.md#listtaskssortnametype)
- [MarketSegmentType](./literals.md#marketsegmenttype)
- [MarketingSourceType](./literals.md#marketingsourcetype)
- [NationalSecurityType](./literals.md#nationalsecuritytype)
- [OpportunityEngagementInvitationSortNameType](./literals.md#opportunityengagementinvitationsortnametype)
- [OpportunityOriginType](./literals.md#opportunityorigintype)
- [OpportunitySortNameType](./literals.md#opportunitysortnametype)
- [OpportunityTypeType](./literals.md#opportunitytypetype)
- [ParticipantTypeType](./literals.md#participanttypetype)
- [PaymentFrequencyType](./literals.md#paymentfrequencytype)
- [PrimaryNeedFromAwsType](./literals.md#primaryneedfromawstype)
- [ReasonCodeType](./literals.md#reasoncodetype)
- [ReceiverResponsibilityType](./literals.md#receiverresponsibilitytype)
- [RelatedEntityTypeType](./literals.md#relatedentitytypetype)
- [ResourceSnapshotJobStatusType](./literals.md#resourcesnapshotjobstatustype)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [RevenueModelType](./literals.md#revenuemodeltype)
- [ReviewStatusType](./literals.md#reviewstatustype)
- [SalesActivityType](./literals.md#salesactivitytype)
- [SalesInvolvementTypeType](./literals.md#salesinvolvementtypetype)
- [SolutionSortNameType](./literals.md#solutionsortnametype)
- [SolutionStatusType](./literals.md#solutionstatustype)
- [SortByType](./literals.md#sortbytype)
- [SortOrderType](./literals.md#sortordertype)
- [StageType](./literals.md#stagetype)
- [TaskStatusType](./literals.md#taskstatustype)
- [VisibilityType](./literals.md#visibilitytype)
- [PartnerCentralSellingAPIServiceName](./literals.md#partnercentralsellingapiservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AcceptEngagementInvitationRequestTypeDef](./type_defs.md#acceptengagementinvitationrequesttypedef)
- [AccountReceiverTypeDef](./type_defs.md#accountreceivertypedef)
- [AddressSummaryTypeDef](./type_defs.md#addresssummarytypedef)
- [AddressTypeDef](./type_defs.md#addresstypedef)
- [AssigneeContactTypeDef](./type_defs.md#assigneecontacttypedef)
- [AssociateOpportunityRequestTypeDef](./type_defs.md#associateopportunityrequesttypedef)
- [ContactTypeDef](./type_defs.md#contacttypedef)
- [ProfileNextStepsHistoryTypeDef](./type_defs.md#profilenextstepshistorytypedef)
- [ExpectedCustomerSpendTypeDef](./type_defs.md#expectedcustomerspendtypedef)
- [AwsOpportunityRelatedEntitiesTypeDef](./type_defs.md#awsopportunityrelatedentitiestypedef)
- [AwsProductOptimizationTypeDef](./type_defs.md#awsproductoptimizationtypedef)
- [AwsSubmissionTypeDef](./type_defs.md#awssubmissiontypedef)
- [AwsTeamMemberTypeDef](./type_defs.md#awsteammembertypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [CreateResourceSnapshotRequestTypeDef](./type_defs.md#createresourcesnapshotrequesttypedef)
- [EngagementCustomerProjectDetailsTypeDef](./type_defs.md#engagementcustomerprojectdetailstypedef)
- [EngagementCustomerTypeDef](./type_defs.md#engagementcustomertypedef)
- [DeleteResourceSnapshotJobRequestTypeDef](./type_defs.md#deleteresourcesnapshotjobrequesttypedef)
- [DisassociateOpportunityRequestTypeDef](./type_defs.md#disassociateopportunityrequesttypedef)
- [EngagementMemberSummaryTypeDef](./type_defs.md#engagementmembersummarytypedef)
- [EngagementMemberTypeDef](./type_defs.md#engagementmembertypedef)
- [EngagementResourceAssociationSummaryTypeDef](./type_defs.md#engagementresourceassociationsummarytypedef)
- [EngagementSortTypeDef](./type_defs.md#engagementsorttypedef)
- [EngagementSummaryTypeDef](./type_defs.md#engagementsummarytypedef)
- [GetAwsOpportunitySummaryRequestTypeDef](./type_defs.md#getawsopportunitysummaryrequesttypedef)
- [GetEngagementInvitationRequestTypeDef](./type_defs.md#getengagementinvitationrequesttypedef)
- [GetEngagementRequestTypeDef](./type_defs.md#getengagementrequesttypedef)
- [GetOpportunityRequestTypeDef](./type_defs.md#getopportunityrequesttypedef)
- [MarketingOutputTypeDef](./type_defs.md#marketingoutputtypedef)
- [RelatedEntityIdentifiersTypeDef](./type_defs.md#relatedentityidentifierstypedef)
- [GetResourceSnapshotJobRequestTypeDef](./type_defs.md#getresourcesnapshotjobrequesttypedef)
- [GetResourceSnapshotRequestTypeDef](./type_defs.md#getresourcesnapshotrequesttypedef)
- [GetSellingSystemSettingsRequestTypeDef](./type_defs.md#getsellingsystemsettingsrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [LeadContactTypeDef](./type_defs.md#leadcontacttypedef)
- [LeadInvitationCustomerTypeDef](./type_defs.md#leadinvitationcustomertypedef)
- [LeadInvitationInteractionTypeDef](./type_defs.md#leadinvitationinteractiontypedef)
- [LifeCycleForViewTypeDef](./type_defs.md#lifecycleforviewtypedef)
- [NextStepsHistoryOutputTypeDef](./type_defs.md#nextstepshistoryoutputtypedef)
- [LifeCycleSummaryTypeDef](./type_defs.md#lifecyclesummarytypedef)
- [ListEngagementByAcceptingInvitationTaskSummaryTypeDef](./type_defs.md#listengagementbyacceptinginvitationtasksummarytypedef)
- [ListTasksSortBaseTypeDef](./type_defs.md#listtaskssortbasetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListEngagementFromOpportunityTaskSummaryTypeDef](./type_defs.md#listengagementfromopportunitytasksummarytypedef)
- [OpportunityEngagementInvitationSortTypeDef](./type_defs.md#opportunityengagementinvitationsorttypedef)
- [ListEngagementMembersRequestTypeDef](./type_defs.md#listengagementmembersrequesttypedef)
- [ListEngagementResourceAssociationsRequestTypeDef](./type_defs.md#listengagementresourceassociationsrequesttypedef)
- [OpportunitySortTypeDef](./type_defs.md#opportunitysorttypedef)
- [ListOpportunityFromEngagementTaskSummaryTypeDef](./type_defs.md#listopportunityfromengagementtasksummarytypedef)
- [SortObjectTypeDef](./type_defs.md#sortobjecttypedef)
- [ResourceSnapshotJobSummaryTypeDef](./type_defs.md#resourcesnapshotjobsummarytypedef)
- [ListResourceSnapshotsRequestTypeDef](./type_defs.md#listresourcesnapshotsrequesttypedef)
- [ResourceSnapshotSummaryTypeDef](./type_defs.md#resourcesnapshotsummarytypedef)
- [SolutionSortTypeDef](./type_defs.md#solutionsorttypedef)
- [SolutionBaseTypeDef](./type_defs.md#solutionbasetypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [MarketingTypeDef](./type_defs.md#marketingtypedef)
- [MonetaryValueTypeDef](./type_defs.md#monetaryvaluetypedef)
- [SenderContactTypeDef](./type_defs.md#sendercontacttypedef)
- [PutSellingSystemSettingsRequestTypeDef](./type_defs.md#putsellingsystemsettingsrequesttypedef)
- [RejectEngagementInvitationRequestTypeDef](./type_defs.md#rejectengagementinvitationrequesttypedef)
- [StartResourceSnapshotJobRequestTypeDef](./type_defs.md#startresourcesnapshotjobrequesttypedef)
- [StopResourceSnapshotJobRequestTypeDef](./type_defs.md#stopresourcesnapshotjobrequesttypedef)
- [SubmitOpportunityRequestTypeDef](./type_defs.md#submitopportunityrequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [ReceiverTypeDef](./type_defs.md#receivertypedef)
- [AccountSummaryTypeDef](./type_defs.md#accountsummarytypedef)
- [LeadCustomerTypeDef](./type_defs.md#leadcustomertypedef)
- [AccountTypeDef](./type_defs.md#accounttypedef)
- [AssignOpportunityRequestTypeDef](./type_defs.md#assignopportunityrequesttypedef)
- [AwsOpportunityCustomerTypeDef](./type_defs.md#awsopportunitycustomertypedef)
- [AwsOpportunityLifeCycleTypeDef](./type_defs.md#awsopportunitylifecycletypedef)
- [AwsOpportunityProjectTypeDef](./type_defs.md#awsopportunityprojecttypedef)
- [ProjectDetailsOutputTypeDef](./type_defs.md#projectdetailsoutputtypedef)
- [ProjectDetailsTypeDef](./type_defs.md#projectdetailstypedef)
- [ProjectOutputTypeDef](./type_defs.md#projectoutputtypedef)
- [ProjectSummaryTypeDef](./type_defs.md#projectsummarytypedef)
- [ProjectTypeDef](./type_defs.md#projecttypedef)
- [ProjectViewTypeDef](./type_defs.md#projectviewtypedef)
- [AwsProductDetailsTypeDef](./type_defs.md#awsproductdetailstypedef)
- [CreateEngagementContextResponseTypeDef](./type_defs.md#createengagementcontextresponsetypedef)
- [CreateEngagementInvitationResponseTypeDef](./type_defs.md#createengagementinvitationresponsetypedef)
- [CreateEngagementResponseTypeDef](./type_defs.md#createengagementresponsetypedef)
- [CreateOpportunityResponseTypeDef](./type_defs.md#createopportunityresponsetypedef)
- [CreateResourceSnapshotJobResponseTypeDef](./type_defs.md#createresourcesnapshotjobresponsetypedef)
- [CreateResourceSnapshotResponseTypeDef](./type_defs.md#createresourcesnapshotresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetResourceSnapshotJobResponseTypeDef](./type_defs.md#getresourcesnapshotjobresponsetypedef)
- [GetSellingSystemSettingsResponseTypeDef](./type_defs.md#getsellingsystemsettingsresponsetypedef)
- [PutSellingSystemSettingsResponseTypeDef](./type_defs.md#putsellingsystemsettingsresponsetypedef)
- [StartEngagementByAcceptingInvitationTaskResponseTypeDef](./type_defs.md#startengagementbyacceptinginvitationtaskresponsetypedef)
- [StartEngagementFromOpportunityTaskResponseTypeDef](./type_defs.md#startengagementfromopportunitytaskresponsetypedef)
- [StartOpportunityFromEngagementTaskResponseTypeDef](./type_defs.md#startopportunityfromengagementtaskresponsetypedef)
- [UpdateEngagementContextResponseTypeDef](./type_defs.md#updateengagementcontextresponsetypedef)
- [UpdateOpportunityResponseTypeDef](./type_defs.md#updateopportunityresponsetypedef)
- [CreateResourceSnapshotJobRequestTypeDef](./type_defs.md#createresourcesnapshotjobrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartEngagementByAcceptingInvitationTaskRequestTypeDef](./type_defs.md#startengagementbyacceptinginvitationtaskrequesttypedef)
- [StartEngagementFromOpportunityTaskRequestTypeDef](./type_defs.md#startengagementfromopportunitytaskrequesttypedef)
- [StartOpportunityFromEngagementTaskRequestTypeDef](./type_defs.md#startopportunityfromengagementtaskrequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [CustomerProjectsContextTypeDef](./type_defs.md#customerprojectscontexttypedef)
- [ListEngagementMembersResponseTypeDef](./type_defs.md#listengagementmembersresponsetypedef)
- [ListEngagementResourceAssociationsResponseTypeDef](./type_defs.md#listengagementresourceassociationsresponsetypedef)
- [ListEngagementsRequestTypeDef](./type_defs.md#listengagementsrequesttypedef)
- [ListEngagementsResponseTypeDef](./type_defs.md#listengagementsresponsetypedef)
- [LastModifiedDateTypeDef](./type_defs.md#lastmodifieddatetypedef)
- [NextStepsHistoryTypeDef](./type_defs.md#nextstepshistorytypedef)
- [LeadInteractionOutputTypeDef](./type_defs.md#leadinteractionoutputtypedef)
- [LeadInteractionTypeDef](./type_defs.md#leadinteractiontypedef)
- [LeadInvitationPayloadTypeDef](./type_defs.md#leadinvitationpayloadtypedef)
- [LifeCycleOutputTypeDef](./type_defs.md#lifecycleoutputtypedef)
- [ListEngagementByAcceptingInvitationTasksResponseTypeDef](./type_defs.md#listengagementbyacceptinginvitationtasksresponsetypedef)
- [ListEngagementByAcceptingInvitationTasksRequestTypeDef](./type_defs.md#listengagementbyacceptinginvitationtasksrequesttypedef)
- [ListEngagementFromOpportunityTasksRequestTypeDef](./type_defs.md#listengagementfromopportunitytasksrequesttypedef)
- [ListOpportunityFromEngagementTasksRequestTypeDef](./type_defs.md#listopportunityfromengagementtasksrequesttypedef)
- [ListEngagementByAcceptingInvitationTasksRequestPaginateTypeDef](./type_defs.md#listengagementbyacceptinginvitationtasksrequestpaginatetypedef)
- [ListEngagementFromOpportunityTasksRequestPaginateTypeDef](./type_defs.md#listengagementfromopportunitytasksrequestpaginatetypedef)
- [ListEngagementMembersRequestPaginateTypeDef](./type_defs.md#listengagementmembersrequestpaginatetypedef)
- [ListEngagementResourceAssociationsRequestPaginateTypeDef](./type_defs.md#listengagementresourceassociationsrequestpaginatetypedef)
- [ListEngagementsRequestPaginateTypeDef](./type_defs.md#listengagementsrequestpaginatetypedef)
- [ListOpportunityFromEngagementTasksRequestPaginateTypeDef](./type_defs.md#listopportunityfromengagementtasksrequestpaginatetypedef)
- [ListResourceSnapshotsRequestPaginateTypeDef](./type_defs.md#listresourcesnapshotsrequestpaginatetypedef)
- [ListEngagementFromOpportunityTasksResponseTypeDef](./type_defs.md#listengagementfromopportunitytasksresponsetypedef)
- [ListEngagementInvitationsRequestPaginateTypeDef](./type_defs.md#listengagementinvitationsrequestpaginatetypedef)
- [ListEngagementInvitationsRequestTypeDef](./type_defs.md#listengagementinvitationsrequesttypedef)
- [ListOpportunityFromEngagementTasksResponseTypeDef](./type_defs.md#listopportunityfromengagementtasksresponsetypedef)
- [ListResourceSnapshotJobsRequestPaginateTypeDef](./type_defs.md#listresourcesnapshotjobsrequestpaginatetypedef)
- [ListResourceSnapshotJobsRequestTypeDef](./type_defs.md#listresourcesnapshotjobsrequesttypedef)
- [ListResourceSnapshotJobsResponseTypeDef](./type_defs.md#listresourcesnapshotjobsresponsetypedef)
- [ListResourceSnapshotsResponseTypeDef](./type_defs.md#listresourcesnapshotsresponsetypedef)
- [ListSolutionsRequestPaginateTypeDef](./type_defs.md#listsolutionsrequestpaginatetypedef)
- [ListSolutionsRequestTypeDef](./type_defs.md#listsolutionsrequesttypedef)
- [ListSolutionsResponseTypeDef](./type_defs.md#listsolutionsresponsetypedef)
- [MarketingUnionTypeDef](./type_defs.md#marketinguniontypedef)
- [SoftwareRevenueTypeDef](./type_defs.md#softwarerevenuetypedef)
- [EngagementInvitationSummaryTypeDef](./type_defs.md#engagementinvitationsummarytypedef)
- [CustomerSummaryTypeDef](./type_defs.md#customersummarytypedef)
- [CustomerOutputTypeDef](./type_defs.md#customeroutputtypedef)
- [CustomerTypeDef](./type_defs.md#customertypedef)
- [OpportunityInvitationPayloadOutputTypeDef](./type_defs.md#opportunityinvitationpayloadoutputtypedef)
- [ProjectDetailsUnionTypeDef](./type_defs.md#projectdetailsuniontypedef)
- [ProjectUnionTypeDef](./type_defs.md#projectuniontypedef)
- [AwsProductInsightsTypeDef](./type_defs.md#awsproductinsightstypedef)
- [ListOpportunitiesRequestPaginateTypeDef](./type_defs.md#listopportunitiesrequestpaginatetypedef)
- [ListOpportunitiesRequestTypeDef](./type_defs.md#listopportunitiesrequesttypedef)
- [LifeCycleTypeDef](./type_defs.md#lifecycletypedef)
- [LeadContextOutputTypeDef](./type_defs.md#leadcontextoutputtypedef)
- [LeadInteractionUnionTypeDef](./type_defs.md#leadinteractionuniontypedef)
- [ListEngagementInvitationsResponseTypeDef](./type_defs.md#listengagementinvitationsresponsetypedef)
- [OpportunitySummaryTypeDef](./type_defs.md#opportunitysummarytypedef)
- [GetOpportunityResponseTypeDef](./type_defs.md#getopportunityresponsetypedef)
- [OpportunitySummaryViewTypeDef](./type_defs.md#opportunitysummaryviewtypedef)
- [CustomerUnionTypeDef](./type_defs.md#customeruniontypedef)
- [PayloadOutputTypeDef](./type_defs.md#payloadoutputtypedef)
- [OpportunityInvitationPayloadTypeDef](./type_defs.md#opportunityinvitationpayloadtypedef)
- [AwsProductsSpendInsightsBySourceTypeDef](./type_defs.md#awsproductsspendinsightsbysourcetypedef)
- [LifeCycleUnionTypeDef](./type_defs.md#lifecycleuniontypedef)
- [EngagementContextPayloadOutputTypeDef](./type_defs.md#engagementcontextpayloadoutputtypedef)
- [LeadContextTypeDef](./type_defs.md#leadcontexttypedef)
- [UpdateLeadContextTypeDef](./type_defs.md#updateleadcontexttypedef)
- [ListOpportunitiesResponseTypeDef](./type_defs.md#listopportunitiesresponsetypedef)
- [ResourceSnapshotPayloadTypeDef](./type_defs.md#resourcesnapshotpayloadtypedef)
- [GetEngagementInvitationResponseTypeDef](./type_defs.md#getengagementinvitationresponsetypedef)
- [OpportunityInvitationPayloadUnionTypeDef](./type_defs.md#opportunityinvitationpayloaduniontypedef)
- [AwsOpportunityInsightsTypeDef](./type_defs.md#awsopportunityinsightstypedef)
- [CreateOpportunityRequestTypeDef](./type_defs.md#createopportunityrequesttypedef)
- [UpdateOpportunityRequestTypeDef](./type_defs.md#updateopportunityrequesttypedef)
- [EngagementContextDetailsOutputTypeDef](./type_defs.md#engagementcontextdetailsoutputtypedef)
- [LeadContextUnionTypeDef](./type_defs.md#leadcontextuniontypedef)
- [UpdateEngagementContextPayloadTypeDef](./type_defs.md#updateengagementcontextpayloadtypedef)
- [GetResourceSnapshotResponseTypeDef](./type_defs.md#getresourcesnapshotresponsetypedef)
- [PayloadTypeDef](./type_defs.md#payloadtypedef)
- [GetAwsOpportunitySummaryResponseTypeDef](./type_defs.md#getawsopportunitysummaryresponsetypedef)
- [GetEngagementResponseTypeDef](./type_defs.md#getengagementresponsetypedef)
- [EngagementContextPayloadTypeDef](./type_defs.md#engagementcontextpayloadtypedef)
- [UpdateEngagementContextRequestTypeDef](./type_defs.md#updateengagementcontextrequesttypedef)
- [PayloadUnionTypeDef](./type_defs.md#payloaduniontypedef)
- [EngagementContextPayloadUnionTypeDef](./type_defs.md#engagementcontextpayloaduniontypedef)
- [InvitationTypeDef](./type_defs.md#invitationtypedef)
- [CreateEngagementContextRequestTypeDef](./type_defs.md#createengagementcontextrequesttypedef)
- [EngagementContextDetailsTypeDef](./type_defs.md#engagementcontextdetailstypedef)
- [CreateEngagementInvitationRequestTypeDef](./type_defs.md#createengagementinvitationrequesttypedef)
- [EngagementContextDetailsUnionTypeDef](./type_defs.md#engagementcontextdetailsuniontypedef)
- [CreateEngagementRequestTypeDef](./type_defs.md#createengagementrequesttypedef)

