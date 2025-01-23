# Type definitions

> [Index](../README.md) > [PartnerCentralSellingAPI](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [PartnerCentralSellingAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#partnercentralsellingapi)
    type annotations stubs module [types-aiobotocore-partnercentral-selling](https://pypi.org/project/types-aiobotocore-partnercentral-selling/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## ProjectDetailsUnionTypeDef

```python
# ProjectDetailsUnionTypeDef definition

ProjectDetailsUnionTypeDef = Union[
    ProjectDetailsTypeDef,  # (1)
    ProjectDetailsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ProjectDetailsTypeDef](./type_defs.md#projectdetailstypedef) 
2. See [:material-code-braces: ProjectDetailsOutputTypeDef](./type_defs.md#projectdetailsoutputtypedef) 

## NextStepsHistoryUnionTypeDef

```python
# NextStepsHistoryUnionTypeDef definition

NextStepsHistoryUnionTypeDef = Union[
    NextStepsHistoryTypeDef,  # (1)
    NextStepsHistoryOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NextStepsHistoryTypeDef](./type_defs.md#nextstepshistorytypedef) 
2. See [:material-code-braces: NextStepsHistoryOutputTypeDef](./type_defs.md#nextstepshistoryoutputtypedef) 

## OpportunityInvitationPayloadUnionTypeDef

```python
# OpportunityInvitationPayloadUnionTypeDef definition

OpportunityInvitationPayloadUnionTypeDef = Union[
    OpportunityInvitationPayloadTypeDef,  # (1)
    OpportunityInvitationPayloadOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OpportunityInvitationPayloadTypeDef](./type_defs.md#opportunityinvitationpayloadtypedef) 
2. See [:material-code-braces: OpportunityInvitationPayloadOutputTypeDef](./type_defs.md#opportunityinvitationpayloadoutputtypedef) 

## PayloadUnionTypeDef

```python
# PayloadUnionTypeDef definition

PayloadUnionTypeDef = Union[
    PayloadTypeDef,  # (1)
    PayloadOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PayloadTypeDef](./type_defs.md#payloadtypedef) 
2. See [:material-code-braces: PayloadOutputTypeDef](./type_defs.md#payloadoutputtypedef) 



## AcceptEngagementInvitationRequestRequestTypeDef

```python
# AcceptEngagementInvitationRequestRequestTypeDef definition

class AcceptEngagementInvitationRequestRequestTypeDef(TypedDict):
    Catalog: str,
    Identifier: str,
```

## AccountReceiverTypeDef

```python
# AccountReceiverTypeDef definition

class AccountReceiverTypeDef(TypedDict):
    AwsAccountId: str,
    Alias: NotRequired[str],
```

## AddressSummaryTypeDef

```python
# AddressSummaryTypeDef definition

class AddressSummaryTypeDef(TypedDict):
    City: NotRequired[str],
    CountryCode: NotRequired[CountryCodeType],  # (1)
    PostalCode: NotRequired[str],
    StateOrRegion: NotRequired[str],
```

1. See [:material-code-brackets: CountryCodeType](./literals.md#countrycodetype) 
## AddressTypeDef

```python
# AddressTypeDef definition

class AddressTypeDef(TypedDict):
    City: NotRequired[str],
    CountryCode: NotRequired[CountryCodeType],  # (1)
    PostalCode: NotRequired[str],
    StateOrRegion: NotRequired[str],
    StreetAddress: NotRequired[str],
```

1. See [:material-code-brackets: CountryCodeType](./literals.md#countrycodetype) 
## AssigneeContactTypeDef

```python
# AssigneeContactTypeDef definition

class AssigneeContactTypeDef(TypedDict):
    BusinessTitle: str,
    Email: str,
    FirstName: str,
    LastName: str,
```

## AssociateOpportunityRequestRequestTypeDef

```python
# AssociateOpportunityRequestRequestTypeDef definition

class AssociateOpportunityRequestRequestTypeDef(TypedDict):
    Catalog: str,
    OpportunityIdentifier: str,
    RelatedEntityIdentifier: str,
    RelatedEntityType: RelatedEntityTypeType,  # (1)
```

1. See [:material-code-brackets: RelatedEntityTypeType](./literals.md#relatedentitytypetype) 
## ContactTypeDef

```python
# ContactTypeDef definition

class ContactTypeDef(TypedDict):
    BusinessTitle: NotRequired[str],
    Email: NotRequired[str],
    FirstName: NotRequired[str],
    LastName: NotRequired[str],
    Phone: NotRequired[str],
```

## AwsOpportunityInsightsTypeDef

```python
# AwsOpportunityInsightsTypeDef definition

class AwsOpportunityInsightsTypeDef(TypedDict):
    EngagementScore: NotRequired[EngagementScoreType],  # (1)
    NextBestActions: NotRequired[str],
```

1. See [:material-code-brackets: EngagementScoreType](./literals.md#engagementscoretype) 
## ProfileNextStepsHistoryTypeDef

```python
# ProfileNextStepsHistoryTypeDef definition

class ProfileNextStepsHistoryTypeDef(TypedDict):
    Time: datetime,
    Value: str,
```

## ExpectedCustomerSpendTypeDef

```python
# ExpectedCustomerSpendTypeDef definition

class ExpectedCustomerSpendTypeDef(TypedDict):
    Amount: str,
    CurrencyCode: ExpectedCustomerSpendCurrencyCodeEnumType,  # (1)
    Frequency: PaymentFrequencyType,  # (2)
    TargetCompany: str,
    EstimationUrl: NotRequired[str],
```

1. See [:material-code-brackets: ExpectedCustomerSpendCurrencyCodeEnumType](./literals.md#expectedcustomerspendcurrencycodeenumtype) 
2. See [:material-code-brackets: PaymentFrequencyType](./literals.md#paymentfrequencytype) 
## AwsOpportunityRelatedEntitiesTypeDef

```python
# AwsOpportunityRelatedEntitiesTypeDef definition

class AwsOpportunityRelatedEntitiesTypeDef(TypedDict):
    AwsProducts: NotRequired[List[str]],
    Solutions: NotRequired[List[str]],
```

## AwsSubmissionTypeDef

```python
# AwsSubmissionTypeDef definition

class AwsSubmissionTypeDef(TypedDict):
    InvolvementType: SalesInvolvementTypeType,  # (1)
    Visibility: NotRequired[VisibilityType],  # (2)
```

1. See [:material-code-brackets: SalesInvolvementTypeType](./literals.md#salesinvolvementtypetype) 
2. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## AwsTeamMemberTypeDef

```python
# AwsTeamMemberTypeDef definition

class AwsTeamMemberTypeDef(TypedDict):
    BusinessTitle: NotRequired[AwsMemberBusinessTitleType],  # (1)
    Email: NotRequired[str],
    FirstName: NotRequired[str],
    LastName: NotRequired[str],
```

1. See [:material-code-brackets: AwsMemberBusinessTitleType](./literals.md#awsmemberbusinesstitletype) 
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

## MarketingTypeDef

```python
# MarketingTypeDef definition

class MarketingTypeDef(TypedDict):
    AwsFundingUsed: NotRequired[AwsFundingUsedType],  # (1)
    CampaignName: NotRequired[str],
    Channels: NotRequired[Sequence[ChannelType]],  # (2)
    Source: NotRequired[MarketingSourceType],  # (3)
    UseCases: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: AwsFundingUsedType](./literals.md#awsfundingusedtype) 
2. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
3. See [:material-code-brackets: MarketingSourceType](./literals.md#marketingsourcetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## CreateResourceSnapshotRequestRequestTypeDef

```python
# CreateResourceSnapshotRequestRequestTypeDef definition

class CreateResourceSnapshotRequestRequestTypeDef(TypedDict):
    Catalog: str,
    ClientToken: str,
    EngagementIdentifier: str,
    ResourceIdentifier: str,
    ResourceSnapshotTemplateIdentifier: str,
    ResourceType: ResourceTypeType,  # (1)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## EngagementCustomerProjectDetailsTypeDef

```python
# EngagementCustomerProjectDetailsTypeDef definition

class EngagementCustomerProjectDetailsTypeDef(TypedDict):
    BusinessProblem: str,
    TargetCompletionDate: str,
    Title: str,
```

## EngagementCustomerTypeDef

```python
# EngagementCustomerTypeDef definition

class EngagementCustomerTypeDef(TypedDict):
    CompanyName: str,
    CountryCode: CountryCodeType,  # (1)
    Industry: IndustryType,  # (2)
    WebsiteUrl: str,
```

1. See [:material-code-brackets: CountryCodeType](./literals.md#countrycodetype) 
2. See [:material-code-brackets: IndustryType](./literals.md#industrytype) 
## DeleteResourceSnapshotJobRequestRequestTypeDef

```python
# DeleteResourceSnapshotJobRequestRequestTypeDef definition

class DeleteResourceSnapshotJobRequestRequestTypeDef(TypedDict):
    Catalog: str,
    ResourceSnapshotJobIdentifier: str,
```

## DisassociateOpportunityRequestRequestTypeDef

```python
# DisassociateOpportunityRequestRequestTypeDef definition

class DisassociateOpportunityRequestRequestTypeDef(TypedDict):
    Catalog: str,
    OpportunityIdentifier: str,
    RelatedEntityIdentifier: str,
    RelatedEntityType: RelatedEntityTypeType,  # (1)
```

1. See [:material-code-brackets: RelatedEntityTypeType](./literals.md#relatedentitytypetype) 
## EngagementMemberSummaryTypeDef

```python
# EngagementMemberSummaryTypeDef definition

class EngagementMemberSummaryTypeDef(TypedDict):
    CompanyName: NotRequired[str],
    WebsiteUrl: NotRequired[str],
```

## EngagementMemberTypeDef

```python
# EngagementMemberTypeDef definition

class EngagementMemberTypeDef(TypedDict):
    AccountId: NotRequired[str],
    CompanyName: NotRequired[str],
    WebsiteUrl: NotRequired[str],
```

## EngagementResourceAssociationSummaryTypeDef

```python
# EngagementResourceAssociationSummaryTypeDef definition

class EngagementResourceAssociationSummaryTypeDef(TypedDict):
    Catalog: str,
    CreatedBy: NotRequired[str],
    EngagementId: NotRequired[str],
    ResourceId: NotRequired[str],
    ResourceType: NotRequired[ResourceTypeType],  # (1)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## EngagementSortTypeDef

```python
# EngagementSortTypeDef definition

class EngagementSortTypeDef(TypedDict):
    SortBy: EngagementSortNameType,  # (1)
    SortOrder: SortOrderType,  # (2)
```

1. See [:material-code-brackets: EngagementSortNameType](./literals.md#engagementsortnametype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## EngagementSummaryTypeDef

```python
# EngagementSummaryTypeDef definition

class EngagementSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    CreatedBy: NotRequired[str],
    Id: NotRequired[str],
    MemberCount: NotRequired[int],
    Title: NotRequired[str],
```

## GetAwsOpportunitySummaryRequestRequestTypeDef

```python
# GetAwsOpportunitySummaryRequestRequestTypeDef definition

class GetAwsOpportunitySummaryRequestRequestTypeDef(TypedDict):
    Catalog: str,
    RelatedOpportunityIdentifier: str,
```

## GetEngagementInvitationRequestRequestTypeDef

```python
# GetEngagementInvitationRequestRequestTypeDef definition

class GetEngagementInvitationRequestRequestTypeDef(TypedDict):
    Catalog: str,
    Identifier: str,
```

## GetEngagementRequestRequestTypeDef

```python
# GetEngagementRequestRequestTypeDef definition

class GetEngagementRequestRequestTypeDef(TypedDict):
    Catalog: str,
    Identifier: str,
```

## GetOpportunityRequestRequestTypeDef

```python
# GetOpportunityRequestRequestTypeDef definition

class GetOpportunityRequestRequestTypeDef(TypedDict):
    Catalog: str,
    Identifier: str,
```

## MarketingOutputTypeDef

```python
# MarketingOutputTypeDef definition

class MarketingOutputTypeDef(TypedDict):
    AwsFundingUsed: NotRequired[AwsFundingUsedType],  # (1)
    CampaignName: NotRequired[str],
    Channels: NotRequired[List[ChannelType]],  # (2)
    Source: NotRequired[MarketingSourceType],  # (3)
    UseCases: NotRequired[List[str]],
```

1. See [:material-code-brackets: AwsFundingUsedType](./literals.md#awsfundingusedtype) 
2. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
3. See [:material-code-brackets: MarketingSourceType](./literals.md#marketingsourcetype) 
## RelatedEntityIdentifiersTypeDef

```python
# RelatedEntityIdentifiersTypeDef definition

class RelatedEntityIdentifiersTypeDef(TypedDict):
    AwsMarketplaceOffers: NotRequired[List[str]],
    AwsProducts: NotRequired[List[str]],
    Solutions: NotRequired[List[str]],
```

## GetResourceSnapshotJobRequestRequestTypeDef

```python
# GetResourceSnapshotJobRequestRequestTypeDef definition

class GetResourceSnapshotJobRequestRequestTypeDef(TypedDict):
    Catalog: str,
    ResourceSnapshotJobIdentifier: str,
```

## GetResourceSnapshotRequestRequestTypeDef

```python
# GetResourceSnapshotRequestRequestTypeDef definition

class GetResourceSnapshotRequestRequestTypeDef(TypedDict):
    Catalog: str,
    EngagementIdentifier: str,
    ResourceIdentifier: str,
    ResourceSnapshotTemplateIdentifier: str,
    ResourceType: ResourceTypeType,  # (1)
    Revision: NotRequired[int],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## GetSellingSystemSettingsRequestRequestTypeDef

```python
# GetSellingSystemSettingsRequestRequestTypeDef definition

class GetSellingSystemSettingsRequestRequestTypeDef(TypedDict):
    Catalog: str,
```

## LifeCycleForViewTypeDef

```python
# LifeCycleForViewTypeDef definition

class LifeCycleForViewTypeDef(TypedDict):
    NextSteps: NotRequired[str],
    ReviewStatus: NotRequired[ReviewStatusType],  # (1)
    Stage: NotRequired[StageType],  # (2)
    TargetCloseDate: NotRequired[str],
```

1. See [:material-code-brackets: ReviewStatusType](./literals.md#reviewstatustype) 
2. See [:material-code-brackets: StageType](./literals.md#stagetype) 
## NextStepsHistoryOutputTypeDef

```python
# NextStepsHistoryOutputTypeDef definition

class NextStepsHistoryOutputTypeDef(TypedDict):
    Time: datetime,
    Value: str,
```

## LifeCycleSummaryTypeDef

```python
# LifeCycleSummaryTypeDef definition

class LifeCycleSummaryTypeDef(TypedDict):
    ClosedLostReason: NotRequired[ClosedLostReasonType],  # (1)
    NextSteps: NotRequired[str],
    ReviewComments: NotRequired[str],
    ReviewStatus: NotRequired[ReviewStatusType],  # (2)
    ReviewStatusReason: NotRequired[str],
    Stage: NotRequired[StageType],  # (3)
    TargetCloseDate: NotRequired[str],
```

1. See [:material-code-brackets: ClosedLostReasonType](./literals.md#closedlostreasontype) 
2. See [:material-code-brackets: ReviewStatusType](./literals.md#reviewstatustype) 
3. See [:material-code-brackets: StageType](./literals.md#stagetype) 
## ListEngagementByAcceptingInvitationTaskSummaryTypeDef

```python
# ListEngagementByAcceptingInvitationTaskSummaryTypeDef definition

class ListEngagementByAcceptingInvitationTaskSummaryTypeDef(TypedDict):
    EngagementInvitationId: NotRequired[str],
    Message: NotRequired[str],
    OpportunityId: NotRequired[str],
    ReasonCode: NotRequired[ReasonCodeType],  # (1)
    ResourceSnapshotJobId: NotRequired[str],
    StartTime: NotRequired[datetime],
    TaskArn: NotRequired[str],
    TaskId: NotRequired[str],
    TaskStatus: NotRequired[TaskStatusType],  # (2)
```

1. See [:material-code-brackets: ReasonCodeType](./literals.md#reasoncodetype) 
2. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
## ListTasksSortBaseTypeDef

```python
# ListTasksSortBaseTypeDef definition

class ListTasksSortBaseTypeDef(TypedDict):
    SortBy: ListTasksSortNameType,  # (1)
    SortOrder: SortOrderType,  # (2)
```

1. See [:material-code-brackets: ListTasksSortNameType](./literals.md#listtaskssortnametype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListEngagementFromOpportunityTaskSummaryTypeDef

```python
# ListEngagementFromOpportunityTaskSummaryTypeDef definition

class ListEngagementFromOpportunityTaskSummaryTypeDef(TypedDict):
    EngagementId: NotRequired[str],
    EngagementInvitationId: NotRequired[str],
    Message: NotRequired[str],
    OpportunityId: NotRequired[str],
    ReasonCode: NotRequired[ReasonCodeType],  # (1)
    ResourceSnapshotJobId: NotRequired[str],
    StartTime: NotRequired[datetime],
    TaskArn: NotRequired[str],
    TaskId: NotRequired[str],
    TaskStatus: NotRequired[TaskStatusType],  # (2)
```

1. See [:material-code-brackets: ReasonCodeType](./literals.md#reasoncodetype) 
2. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
## OpportunityEngagementInvitationSortTypeDef

```python
# OpportunityEngagementInvitationSortTypeDef definition

class OpportunityEngagementInvitationSortTypeDef(TypedDict):
    SortBy: OpportunityEngagementInvitationSortNameType,  # (1)
    SortOrder: SortOrderType,  # (2)
```

1. See [:material-code-brackets: OpportunityEngagementInvitationSortNameType](./literals.md#opportunityengagementinvitationsortnametype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListEngagementMembersRequestRequestTypeDef

```python
# ListEngagementMembersRequestRequestTypeDef definition

class ListEngagementMembersRequestRequestTypeDef(TypedDict):
    Catalog: str,
    Identifier: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListEngagementResourceAssociationsRequestRequestTypeDef

```python
# ListEngagementResourceAssociationsRequestRequestTypeDef definition

class ListEngagementResourceAssociationsRequestRequestTypeDef(TypedDict):
    Catalog: str,
    CreatedBy: NotRequired[str],
    EngagementIdentifier: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ResourceIdentifier: NotRequired[str],
    ResourceType: NotRequired[ResourceTypeType],  # (1)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## OpportunitySortTypeDef

```python
# OpportunitySortTypeDef definition

class OpportunitySortTypeDef(TypedDict):
    SortBy: OpportunitySortNameType,  # (1)
    SortOrder: SortOrderType,  # (2)
```

1. See [:material-code-brackets: OpportunitySortNameType](./literals.md#opportunitysortnametype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## SortObjectTypeDef

```python
# SortObjectTypeDef definition

class SortObjectTypeDef(TypedDict):
    SortBy: NotRequired[SortByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: SortByType](./literals.md#sortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ResourceSnapshotJobSummaryTypeDef

```python
# ResourceSnapshotJobSummaryTypeDef definition

class ResourceSnapshotJobSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    EngagementId: NotRequired[str],
    Id: NotRequired[str],
    Status: NotRequired[ResourceSnapshotJobStatusType],  # (1)
```

1. See [:material-code-brackets: ResourceSnapshotJobStatusType](./literals.md#resourcesnapshotjobstatustype) 
## ListResourceSnapshotsRequestRequestTypeDef

```python
# ListResourceSnapshotsRequestRequestTypeDef definition

class ListResourceSnapshotsRequestRequestTypeDef(TypedDict):
    Catalog: str,
    EngagementIdentifier: str,
    CreatedBy: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ResourceIdentifier: NotRequired[str],
    ResourceSnapshotTemplateIdentifier: NotRequired[str],
    ResourceType: NotRequired[ResourceTypeType],  # (1)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## ResourceSnapshotSummaryTypeDef

```python
# ResourceSnapshotSummaryTypeDef definition

class ResourceSnapshotSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreatedBy: NotRequired[str],
    ResourceId: NotRequired[str],
    ResourceSnapshotTemplateName: NotRequired[str],
    ResourceType: NotRequired[ResourceTypeType],  # (1)
    Revision: NotRequired[int],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## SolutionSortTypeDef

```python
# SolutionSortTypeDef definition

class SolutionSortTypeDef(TypedDict):
    SortBy: SolutionSortNameType,  # (1)
    SortOrder: SortOrderType,  # (2)
```

1. See [:material-code-brackets: SolutionSortNameType](./literals.md#solutionsortnametype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## SolutionBaseTypeDef

```python
# SolutionBaseTypeDef definition

class SolutionBaseTypeDef(TypedDict):
    Catalog: str,
    Category: str,
    CreatedDate: datetime,
    Id: str,
    Name: str,
    Status: SolutionStatusType,  # (1)
    Arn: NotRequired[str],
```

1. See [:material-code-brackets: SolutionStatusType](./literals.md#solutionstatustype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## MonetaryValueTypeDef

```python
# MonetaryValueTypeDef definition

class MonetaryValueTypeDef(TypedDict):
    Amount: str,
    CurrencyCode: CurrencyCodeType,  # (1)
```

1. See [:material-code-brackets: CurrencyCodeType](./literals.md#currencycodetype) 
## SenderContactTypeDef

```python
# SenderContactTypeDef definition

class SenderContactTypeDef(TypedDict):
    Email: str,
    BusinessTitle: NotRequired[str],
    FirstName: NotRequired[str],
    LastName: NotRequired[str],
    Phone: NotRequired[str],
```

## PutSellingSystemSettingsRequestRequestTypeDef

```python
# PutSellingSystemSettingsRequestRequestTypeDef definition

class PutSellingSystemSettingsRequestRequestTypeDef(TypedDict):
    Catalog: str,
    ResourceSnapshotJobRoleIdentifier: NotRequired[str],
```

## RejectEngagementInvitationRequestRequestTypeDef

```python
# RejectEngagementInvitationRequestRequestTypeDef definition

class RejectEngagementInvitationRequestRequestTypeDef(TypedDict):
    Catalog: str,
    Identifier: str,
    RejectionReason: NotRequired[str],
```

## StartResourceSnapshotJobRequestRequestTypeDef

```python
# StartResourceSnapshotJobRequestRequestTypeDef definition

class StartResourceSnapshotJobRequestRequestTypeDef(TypedDict):
    Catalog: str,
    ResourceSnapshotJobIdentifier: str,
```

## StopResourceSnapshotJobRequestRequestTypeDef

```python
# StopResourceSnapshotJobRequestRequestTypeDef definition

class StopResourceSnapshotJobRequestRequestTypeDef(TypedDict):
    Catalog: str,
    ResourceSnapshotJobIdentifier: str,
```

## SubmitOpportunityRequestRequestTypeDef

```python
# SubmitOpportunityRequestRequestTypeDef definition

class SubmitOpportunityRequestRequestTypeDef(TypedDict):
    Catalog: str,
    Identifier: str,
    InvolvementType: SalesInvolvementTypeType,  # (1)
    Visibility: NotRequired[VisibilityType],  # (2)
```

1. See [:material-code-brackets: SalesInvolvementTypeType](./literals.md#salesinvolvementtypetype) 
2. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## ReceiverTypeDef

```python
# ReceiverTypeDef definition

class ReceiverTypeDef(TypedDict):
    Account: NotRequired[AccountReceiverTypeDef],  # (1)
```

1. See [:material-code-braces: AccountReceiverTypeDef](./type_defs.md#accountreceivertypedef) 
## AccountSummaryTypeDef

```python
# AccountSummaryTypeDef definition

class AccountSummaryTypeDef(TypedDict):
    CompanyName: str,
    Address: NotRequired[AddressSummaryTypeDef],  # (1)
    Industry: NotRequired[IndustryType],  # (2)
    OtherIndustry: NotRequired[str],
    WebsiteUrl: NotRequired[str],
```

1. See [:material-code-braces: AddressSummaryTypeDef](./type_defs.md#addresssummarytypedef) 
2. See [:material-code-brackets: IndustryType](./literals.md#industrytype) 
## AccountTypeDef

```python
# AccountTypeDef definition

class AccountTypeDef(TypedDict):
    CompanyName: str,
    Address: NotRequired[AddressTypeDef],  # (1)
    AwsAccountId: NotRequired[str],
    Duns: NotRequired[str],
    Industry: NotRequired[IndustryType],  # (2)
    OtherIndustry: NotRequired[str],
    WebsiteUrl: NotRequired[str],
```

1. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
2. See [:material-code-brackets: IndustryType](./literals.md#industrytype) 
## AssignOpportunityRequestRequestTypeDef

```python
# AssignOpportunityRequestRequestTypeDef definition

class AssignOpportunityRequestRequestTypeDef(TypedDict):
    Assignee: AssigneeContactTypeDef,  # (1)
    Catalog: str,
    Identifier: str,
```

1. See [:material-code-braces: AssigneeContactTypeDef](./type_defs.md#assigneecontacttypedef) 
## AwsOpportunityCustomerTypeDef

```python
# AwsOpportunityCustomerTypeDef definition

class AwsOpportunityCustomerTypeDef(TypedDict):
    Contacts: NotRequired[List[ContactTypeDef]],  # (1)
```

1. See [:material-code-braces: ContactTypeDef](./type_defs.md#contacttypedef) 
## AwsOpportunityLifeCycleTypeDef

```python
# AwsOpportunityLifeCycleTypeDef definition

class AwsOpportunityLifeCycleTypeDef(TypedDict):
    ClosedLostReason: NotRequired[AwsClosedLostReasonType],  # (1)
    NextSteps: NotRequired[str],
    NextStepsHistory: NotRequired[List[ProfileNextStepsHistoryTypeDef]],  # (2)
    Stage: NotRequired[AwsOpportunityStageType],  # (3)
    TargetCloseDate: NotRequired[str],
```

1. See [:material-code-brackets: AwsClosedLostReasonType](./literals.md#awsclosedlostreasontype) 
2. See [:material-code-braces: ProfileNextStepsHistoryTypeDef](./type_defs.md#profilenextstepshistorytypedef) 
3. See [:material-code-brackets: AwsOpportunityStageType](./literals.md#awsopportunitystagetype) 
## AwsOpportunityProjectTypeDef

```python
# AwsOpportunityProjectTypeDef definition

class AwsOpportunityProjectTypeDef(TypedDict):
    ExpectedCustomerSpend: NotRequired[List[ExpectedCustomerSpendTypeDef]],  # (1)
```

1. See [:material-code-braces: ExpectedCustomerSpendTypeDef](./type_defs.md#expectedcustomerspendtypedef) 
## ProjectDetailsOutputTypeDef

```python
# ProjectDetailsOutputTypeDef definition

class ProjectDetailsOutputTypeDef(TypedDict):
    BusinessProblem: str,
    ExpectedCustomerSpend: List[ExpectedCustomerSpendTypeDef],  # (1)
    TargetCompletionDate: str,
    Title: str,
```

1. See [:material-code-braces: ExpectedCustomerSpendTypeDef](./type_defs.md#expectedcustomerspendtypedef) 
## ProjectDetailsTypeDef

```python
# ProjectDetailsTypeDef definition

class ProjectDetailsTypeDef(TypedDict):
    BusinessProblem: str,
    ExpectedCustomerSpend: Sequence[ExpectedCustomerSpendTypeDef],  # (1)
    TargetCompletionDate: str,
    Title: str,
```

1. See [:material-code-braces: ExpectedCustomerSpendTypeDef](./type_defs.md#expectedcustomerspendtypedef) 
## ProjectOutputTypeDef

```python
# ProjectOutputTypeDef definition

class ProjectOutputTypeDef(TypedDict):
    AdditionalComments: NotRequired[str],
    ApnPrograms: NotRequired[List[str]],
    CompetitorName: NotRequired[CompetitorNameType],  # (1)
    CustomerBusinessProblem: NotRequired[str],
    CustomerUseCase: NotRequired[str],
    DeliveryModels: NotRequired[List[DeliveryModelType]],  # (2)
    ExpectedCustomerSpend: NotRequired[List[ExpectedCustomerSpendTypeDef]],  # (3)
    OtherCompetitorNames: NotRequired[str],
    OtherSolutionDescription: NotRequired[str],
    RelatedOpportunityIdentifier: NotRequired[str],
    SalesActivities: NotRequired[List[SalesActivityType]],  # (4)
    Title: NotRequired[str],
```

1. See [:material-code-brackets: CompetitorNameType](./literals.md#competitornametype) 
2. See [:material-code-brackets: DeliveryModelType](./literals.md#deliverymodeltype) 
3. See [:material-code-braces: ExpectedCustomerSpendTypeDef](./type_defs.md#expectedcustomerspendtypedef) 
4. See [:material-code-brackets: SalesActivityType](./literals.md#salesactivitytype) 
## ProjectSummaryTypeDef

```python
# ProjectSummaryTypeDef definition

class ProjectSummaryTypeDef(TypedDict):
    DeliveryModels: NotRequired[List[DeliveryModelType]],  # (1)
    ExpectedCustomerSpend: NotRequired[List[ExpectedCustomerSpendTypeDef]],  # (2)
```

1. See [:material-code-brackets: DeliveryModelType](./literals.md#deliverymodeltype) 
2. See [:material-code-braces: ExpectedCustomerSpendTypeDef](./type_defs.md#expectedcustomerspendtypedef) 
## ProjectTypeDef

```python
# ProjectTypeDef definition

class ProjectTypeDef(TypedDict):
    AdditionalComments: NotRequired[str],
    ApnPrograms: NotRequired[Sequence[str]],
    CompetitorName: NotRequired[CompetitorNameType],  # (1)
    CustomerBusinessProblem: NotRequired[str],
    CustomerUseCase: NotRequired[str],
    DeliveryModels: NotRequired[Sequence[DeliveryModelType]],  # (2)
    ExpectedCustomerSpend: NotRequired[Sequence[ExpectedCustomerSpendTypeDef]],  # (3)
    OtherCompetitorNames: NotRequired[str],
    OtherSolutionDescription: NotRequired[str],
    RelatedOpportunityIdentifier: NotRequired[str],
    SalesActivities: NotRequired[Sequence[SalesActivityType]],  # (4)
    Title: NotRequired[str],
```

1. See [:material-code-brackets: CompetitorNameType](./literals.md#competitornametype) 
2. See [:material-code-brackets: DeliveryModelType](./literals.md#deliverymodeltype) 
3. See [:material-code-braces: ExpectedCustomerSpendTypeDef](./type_defs.md#expectedcustomerspendtypedef) 
4. See [:material-code-brackets: SalesActivityType](./literals.md#salesactivitytype) 
## ProjectViewTypeDef

```python
# ProjectViewTypeDef definition

class ProjectViewTypeDef(TypedDict):
    CustomerUseCase: NotRequired[str],
    DeliveryModels: NotRequired[List[DeliveryModelType]],  # (1)
    ExpectedCustomerSpend: NotRequired[List[ExpectedCustomerSpendTypeDef]],  # (2)
    OtherSolutionDescription: NotRequired[str],
    SalesActivities: NotRequired[List[SalesActivityType]],  # (3)
```

1. See [:material-code-brackets: DeliveryModelType](./literals.md#deliverymodeltype) 
2. See [:material-code-braces: ExpectedCustomerSpendTypeDef](./type_defs.md#expectedcustomerspendtypedef) 
3. See [:material-code-brackets: SalesActivityType](./literals.md#salesactivitytype) 
## CreateEngagementInvitationResponseTypeDef

```python
# CreateEngagementInvitationResponseTypeDef definition

class CreateEngagementInvitationResponseTypeDef(TypedDict):
    Arn: str,
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEngagementResponseTypeDef

```python
# CreateEngagementResponseTypeDef definition

class CreateEngagementResponseTypeDef(TypedDict):
    Arn: str,
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateOpportunityResponseTypeDef

```python
# CreateOpportunityResponseTypeDef definition

class CreateOpportunityResponseTypeDef(TypedDict):
    Id: str,
    LastModifiedDate: datetime,
    PartnerOpportunityIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateResourceSnapshotJobResponseTypeDef

```python
# CreateResourceSnapshotJobResponseTypeDef definition

class CreateResourceSnapshotJobResponseTypeDef(TypedDict):
    Arn: str,
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateResourceSnapshotResponseTypeDef

```python
# CreateResourceSnapshotResponseTypeDef definition

class CreateResourceSnapshotResponseTypeDef(TypedDict):
    Arn: str,
    Revision: int,
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
## GetResourceSnapshotJobResponseTypeDef

```python
# GetResourceSnapshotJobResponseTypeDef definition

class GetResourceSnapshotJobResponseTypeDef(TypedDict):
    Arn: str,
    Catalog: str,
    CreatedAt: datetime,
    EngagementId: str,
    Id: str,
    LastFailure: str,
    LastSuccessfulExecutionDate: datetime,
    ResourceArn: str,
    ResourceId: str,
    ResourceSnapshotTemplateName: str,
    ResourceType: ResourceTypeType,  # (1)
    Status: ResourceSnapshotJobStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: ResourceSnapshotJobStatusType](./literals.md#resourcesnapshotjobstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSellingSystemSettingsResponseTypeDef

```python
# GetSellingSystemSettingsResponseTypeDef definition

class GetSellingSystemSettingsResponseTypeDef(TypedDict):
    Catalog: str,
    ResourceSnapshotJobRoleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutSellingSystemSettingsResponseTypeDef

```python
# PutSellingSystemSettingsResponseTypeDef definition

class PutSellingSystemSettingsResponseTypeDef(TypedDict):
    Catalog: str,
    ResourceSnapshotJobRoleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartEngagementByAcceptingInvitationTaskResponseTypeDef

```python
# StartEngagementByAcceptingInvitationTaskResponseTypeDef definition

class StartEngagementByAcceptingInvitationTaskResponseTypeDef(TypedDict):
    EngagementInvitationId: str,
    Message: str,
    OpportunityId: str,
    ReasonCode: ReasonCodeType,  # (1)
    ResourceSnapshotJobId: str,
    StartTime: datetime,
    TaskArn: str,
    TaskId: str,
    TaskStatus: TaskStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ReasonCodeType](./literals.md#reasoncodetype) 
2. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartEngagementFromOpportunityTaskResponseTypeDef

```python
# StartEngagementFromOpportunityTaskResponseTypeDef definition

class StartEngagementFromOpportunityTaskResponseTypeDef(TypedDict):
    EngagementId: str,
    EngagementInvitationId: str,
    Message: str,
    OpportunityId: str,
    ReasonCode: ReasonCodeType,  # (1)
    ResourceSnapshotJobId: str,
    StartTime: datetime,
    TaskArn: str,
    TaskId: str,
    TaskStatus: TaskStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ReasonCodeType](./literals.md#reasoncodetype) 
2. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateOpportunityResponseTypeDef

```python
# UpdateOpportunityResponseTypeDef definition

class UpdateOpportunityResponseTypeDef(TypedDict):
    Id: str,
    LastModifiedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateResourceSnapshotJobRequestRequestTypeDef

```python
# CreateResourceSnapshotJobRequestRequestTypeDef definition

class CreateResourceSnapshotJobRequestRequestTypeDef(TypedDict):
    Catalog: str,
    ClientToken: str,
    EngagementIdentifier: str,
    ResourceIdentifier: str,
    ResourceSnapshotTemplateIdentifier: str,
    ResourceType: ResourceTypeType,  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartEngagementByAcceptingInvitationTaskRequestRequestTypeDef

```python
# StartEngagementByAcceptingInvitationTaskRequestRequestTypeDef definition

class StartEngagementByAcceptingInvitationTaskRequestRequestTypeDef(TypedDict):
    Catalog: str,
    ClientToken: str,
    Identifier: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StartEngagementFromOpportunityTaskRequestRequestTypeDef

```python
# StartEngagementFromOpportunityTaskRequestRequestTypeDef definition

class StartEngagementFromOpportunityTaskRequestRequestTypeDef(TypedDict):
    AwsSubmission: AwsSubmissionTypeDef,  # (1)
    Catalog: str,
    ClientToken: str,
    Identifier: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: AwsSubmissionTypeDef](./type_defs.md#awssubmissiontypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CustomerProjectsContextTypeDef

```python
# CustomerProjectsContextTypeDef definition

class CustomerProjectsContextTypeDef(TypedDict):
    Customer: NotRequired[EngagementCustomerTypeDef],  # (1)
    Project: NotRequired[EngagementCustomerProjectDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: EngagementCustomerTypeDef](./type_defs.md#engagementcustomertypedef) 
2. See [:material-code-braces: EngagementCustomerProjectDetailsTypeDef](./type_defs.md#engagementcustomerprojectdetailstypedef) 
## ListEngagementMembersResponseTypeDef

```python
# ListEngagementMembersResponseTypeDef definition

class ListEngagementMembersResponseTypeDef(TypedDict):
    EngagementMemberList: List[EngagementMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EngagementMemberTypeDef](./type_defs.md#engagementmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEngagementResourceAssociationsResponseTypeDef

```python
# ListEngagementResourceAssociationsResponseTypeDef definition

class ListEngagementResourceAssociationsResponseTypeDef(TypedDict):
    EngagementResourceAssociationSummaries: List[EngagementResourceAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EngagementResourceAssociationSummaryTypeDef](./type_defs.md#engagementresourceassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEngagementsRequestRequestTypeDef

```python
# ListEngagementsRequestRequestTypeDef definition

class ListEngagementsRequestRequestTypeDef(TypedDict):
    Catalog: str,
    CreatedBy: NotRequired[Sequence[str]],
    EngagementIdentifier: NotRequired[Sequence[str]],
    ExcludeCreatedBy: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Sort: NotRequired[EngagementSortTypeDef],  # (1)
```

1. See [:material-code-braces: EngagementSortTypeDef](./type_defs.md#engagementsorttypedef) 
## ListEngagementsResponseTypeDef

```python
# ListEngagementsResponseTypeDef definition

class ListEngagementsResponseTypeDef(TypedDict):
    EngagementSummaryList: List[EngagementSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EngagementSummaryTypeDef](./type_defs.md#engagementsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LastModifiedDateTypeDef

```python
# LastModifiedDateTypeDef definition

class LastModifiedDateTypeDef(TypedDict):
    AfterLastModifiedDate: NotRequired[TimestampTypeDef],
    BeforeLastModifiedDate: NotRequired[TimestampTypeDef],
```

## NextStepsHistoryTypeDef

```python
# NextStepsHistoryTypeDef definition

class NextStepsHistoryTypeDef(TypedDict):
    Time: TimestampTypeDef,
    Value: str,
```

## LifeCycleOutputTypeDef

```python
# LifeCycleOutputTypeDef definition

class LifeCycleOutputTypeDef(TypedDict):
    ClosedLostReason: NotRequired[ClosedLostReasonType],  # (1)
    NextSteps: NotRequired[str],
    NextStepsHistory: NotRequired[List[NextStepsHistoryOutputTypeDef]],  # (2)
    ReviewComments: NotRequired[str],
    ReviewStatus: NotRequired[ReviewStatusType],  # (3)
    ReviewStatusReason: NotRequired[str],
    Stage: NotRequired[StageType],  # (4)
    TargetCloseDate: NotRequired[str],
```

1. See [:material-code-brackets: ClosedLostReasonType](./literals.md#closedlostreasontype) 
2. See [:material-code-braces: NextStepsHistoryOutputTypeDef](./type_defs.md#nextstepshistoryoutputtypedef) 
3. See [:material-code-brackets: ReviewStatusType](./literals.md#reviewstatustype) 
4. See [:material-code-brackets: StageType](./literals.md#stagetype) 
## ListEngagementByAcceptingInvitationTasksResponseTypeDef

```python
# ListEngagementByAcceptingInvitationTasksResponseTypeDef definition

class ListEngagementByAcceptingInvitationTasksResponseTypeDef(TypedDict):
    TaskSummaries: List[ListEngagementByAcceptingInvitationTaskSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListEngagementByAcceptingInvitationTaskSummaryTypeDef](./type_defs.md#listengagementbyacceptinginvitationtasksummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEngagementByAcceptingInvitationTasksRequestRequestTypeDef

```python
# ListEngagementByAcceptingInvitationTasksRequestRequestTypeDef definition

class ListEngagementByAcceptingInvitationTasksRequestRequestTypeDef(TypedDict):
    Catalog: str,
    EngagementInvitationIdentifier: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    OpportunityIdentifier: NotRequired[Sequence[str]],
    Sort: NotRequired[ListTasksSortBaseTypeDef],  # (1)
    TaskIdentifier: NotRequired[Sequence[str]],
    TaskStatus: NotRequired[Sequence[TaskStatusType]],  # (2)
```

1. See [:material-code-braces: ListTasksSortBaseTypeDef](./type_defs.md#listtaskssortbasetypedef) 
2. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
## ListEngagementFromOpportunityTasksRequestRequestTypeDef

```python
# ListEngagementFromOpportunityTasksRequestRequestTypeDef definition

class ListEngagementFromOpportunityTasksRequestRequestTypeDef(TypedDict):
    Catalog: str,
    EngagementIdentifier: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    OpportunityIdentifier: NotRequired[Sequence[str]],
    Sort: NotRequired[ListTasksSortBaseTypeDef],  # (1)
    TaskIdentifier: NotRequired[Sequence[str]],
    TaskStatus: NotRequired[Sequence[TaskStatusType]],  # (2)
```

1. See [:material-code-braces: ListTasksSortBaseTypeDef](./type_defs.md#listtaskssortbasetypedef) 
2. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
## ListEngagementByAcceptingInvitationTasksRequestPaginateTypeDef

```python
# ListEngagementByAcceptingInvitationTasksRequestPaginateTypeDef definition

class ListEngagementByAcceptingInvitationTasksRequestPaginateTypeDef(TypedDict):
    Catalog: str,
    EngagementInvitationIdentifier: NotRequired[Sequence[str]],
    OpportunityIdentifier: NotRequired[Sequence[str]],
    Sort: NotRequired[ListTasksSortBaseTypeDef],  # (1)
    TaskIdentifier: NotRequired[Sequence[str]],
    TaskStatus: NotRequired[Sequence[TaskStatusType]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: ListTasksSortBaseTypeDef](./type_defs.md#listtaskssortbasetypedef) 
2. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEngagementFromOpportunityTasksRequestPaginateTypeDef

```python
# ListEngagementFromOpportunityTasksRequestPaginateTypeDef definition

class ListEngagementFromOpportunityTasksRequestPaginateTypeDef(TypedDict):
    Catalog: str,
    EngagementIdentifier: NotRequired[Sequence[str]],
    OpportunityIdentifier: NotRequired[Sequence[str]],
    Sort: NotRequired[ListTasksSortBaseTypeDef],  # (1)
    TaskIdentifier: NotRequired[Sequence[str]],
    TaskStatus: NotRequired[Sequence[TaskStatusType]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: ListTasksSortBaseTypeDef](./type_defs.md#listtaskssortbasetypedef) 
2. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEngagementMembersRequestPaginateTypeDef

```python
# ListEngagementMembersRequestPaginateTypeDef definition

class ListEngagementMembersRequestPaginateTypeDef(TypedDict):
    Catalog: str,
    Identifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEngagementResourceAssociationsRequestPaginateTypeDef

```python
# ListEngagementResourceAssociationsRequestPaginateTypeDef definition

class ListEngagementResourceAssociationsRequestPaginateTypeDef(TypedDict):
    Catalog: str,
    CreatedBy: NotRequired[str],
    EngagementIdentifier: NotRequired[str],
    ResourceIdentifier: NotRequired[str],
    ResourceType: NotRequired[ResourceTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEngagementsRequestPaginateTypeDef

```python
# ListEngagementsRequestPaginateTypeDef definition

class ListEngagementsRequestPaginateTypeDef(TypedDict):
    Catalog: str,
    CreatedBy: NotRequired[Sequence[str]],
    EngagementIdentifier: NotRequired[Sequence[str]],
    ExcludeCreatedBy: NotRequired[Sequence[str]],
    Sort: NotRequired[EngagementSortTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: EngagementSortTypeDef](./type_defs.md#engagementsorttypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceSnapshotsRequestPaginateTypeDef

```python
# ListResourceSnapshotsRequestPaginateTypeDef definition

class ListResourceSnapshotsRequestPaginateTypeDef(TypedDict):
    Catalog: str,
    EngagementIdentifier: str,
    CreatedBy: NotRequired[str],
    ResourceIdentifier: NotRequired[str],
    ResourceSnapshotTemplateIdentifier: NotRequired[str],
    ResourceType: NotRequired[ResourceTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEngagementFromOpportunityTasksResponseTypeDef

```python
# ListEngagementFromOpportunityTasksResponseTypeDef definition

class ListEngagementFromOpportunityTasksResponseTypeDef(TypedDict):
    TaskSummaries: List[ListEngagementFromOpportunityTaskSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListEngagementFromOpportunityTaskSummaryTypeDef](./type_defs.md#listengagementfromopportunitytasksummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEngagementInvitationsRequestPaginateTypeDef

```python
# ListEngagementInvitationsRequestPaginateTypeDef definition

class ListEngagementInvitationsRequestPaginateTypeDef(TypedDict):
    Catalog: str,
    ParticipantType: ParticipantTypeType,  # (1)
    EngagementIdentifier: NotRequired[Sequence[str]],
    PayloadType: NotRequired[Sequence[EngagementInvitationPayloadTypeType]],  # (2)
    SenderAwsAccountId: NotRequired[Sequence[str]],
    Sort: NotRequired[OpportunityEngagementInvitationSortTypeDef],  # (3)
    Status: NotRequired[Sequence[InvitationStatusType]],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: ParticipantTypeType](./literals.md#participanttypetype) 
2. See [:material-code-brackets: EngagementInvitationPayloadTypeType](./literals.md#engagementinvitationpayloadtypetype) 
3. See [:material-code-braces: OpportunityEngagementInvitationSortTypeDef](./type_defs.md#opportunityengagementinvitationsorttypedef) 
4. See [:material-code-brackets: InvitationStatusType](./literals.md#invitationstatustype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEngagementInvitationsRequestRequestTypeDef

```python
# ListEngagementInvitationsRequestRequestTypeDef definition

class ListEngagementInvitationsRequestRequestTypeDef(TypedDict):
    Catalog: str,
    ParticipantType: ParticipantTypeType,  # (1)
    EngagementIdentifier: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    PayloadType: NotRequired[Sequence[EngagementInvitationPayloadTypeType]],  # (2)
    SenderAwsAccountId: NotRequired[Sequence[str]],
    Sort: NotRequired[OpportunityEngagementInvitationSortTypeDef],  # (3)
    Status: NotRequired[Sequence[InvitationStatusType]],  # (4)
```

1. See [:material-code-brackets: ParticipantTypeType](./literals.md#participanttypetype) 
2. See [:material-code-brackets: EngagementInvitationPayloadTypeType](./literals.md#engagementinvitationpayloadtypetype) 
3. See [:material-code-braces: OpportunityEngagementInvitationSortTypeDef](./type_defs.md#opportunityengagementinvitationsorttypedef) 
4. See [:material-code-brackets: InvitationStatusType](./literals.md#invitationstatustype) 
## ListResourceSnapshotJobsRequestPaginateTypeDef

```python
# ListResourceSnapshotJobsRequestPaginateTypeDef definition

class ListResourceSnapshotJobsRequestPaginateTypeDef(TypedDict):
    Catalog: str,
    EngagementIdentifier: NotRequired[str],
    Sort: NotRequired[SortObjectTypeDef],  # (1)
    Status: NotRequired[ResourceSnapshotJobStatusType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: SortObjectTypeDef](./type_defs.md#sortobjecttypedef) 
2. See [:material-code-brackets: ResourceSnapshotJobStatusType](./literals.md#resourcesnapshotjobstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceSnapshotJobsRequestRequestTypeDef

```python
# ListResourceSnapshotJobsRequestRequestTypeDef definition

class ListResourceSnapshotJobsRequestRequestTypeDef(TypedDict):
    Catalog: str,
    EngagementIdentifier: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Sort: NotRequired[SortObjectTypeDef],  # (1)
    Status: NotRequired[ResourceSnapshotJobStatusType],  # (2)
```

1. See [:material-code-braces: SortObjectTypeDef](./type_defs.md#sortobjecttypedef) 
2. See [:material-code-brackets: ResourceSnapshotJobStatusType](./literals.md#resourcesnapshotjobstatustype) 
## ListResourceSnapshotJobsResponseTypeDef

```python
# ListResourceSnapshotJobsResponseTypeDef definition

class ListResourceSnapshotJobsResponseTypeDef(TypedDict):
    ResourceSnapshotJobSummaries: List[ResourceSnapshotJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceSnapshotJobSummaryTypeDef](./type_defs.md#resourcesnapshotjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourceSnapshotsResponseTypeDef

```python
# ListResourceSnapshotsResponseTypeDef definition

class ListResourceSnapshotsResponseTypeDef(TypedDict):
    ResourceSnapshotSummaries: List[ResourceSnapshotSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceSnapshotSummaryTypeDef](./type_defs.md#resourcesnapshotsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSolutionsRequestPaginateTypeDef

```python
# ListSolutionsRequestPaginateTypeDef definition

class ListSolutionsRequestPaginateTypeDef(TypedDict):
    Catalog: str,
    Category: NotRequired[Sequence[str]],
    Identifier: NotRequired[Sequence[str]],
    Sort: NotRequired[SolutionSortTypeDef],  # (1)
    Status: NotRequired[Sequence[SolutionStatusType]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: SolutionSortTypeDef](./type_defs.md#solutionsorttypedef) 
2. See [:material-code-brackets: SolutionStatusType](./literals.md#solutionstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSolutionsRequestRequestTypeDef

```python
# ListSolutionsRequestRequestTypeDef definition

class ListSolutionsRequestRequestTypeDef(TypedDict):
    Catalog: str,
    Category: NotRequired[Sequence[str]],
    Identifier: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Sort: NotRequired[SolutionSortTypeDef],  # (1)
    Status: NotRequired[Sequence[SolutionStatusType]],  # (2)
```

1. See [:material-code-braces: SolutionSortTypeDef](./type_defs.md#solutionsorttypedef) 
2. See [:material-code-brackets: SolutionStatusType](./literals.md#solutionstatustype) 
## ListSolutionsResponseTypeDef

```python
# ListSolutionsResponseTypeDef definition

class ListSolutionsResponseTypeDef(TypedDict):
    SolutionSummaries: List[SolutionBaseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SolutionBaseTypeDef](./type_defs.md#solutionbasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SoftwareRevenueTypeDef

```python
# SoftwareRevenueTypeDef definition

class SoftwareRevenueTypeDef(TypedDict):
    DeliveryModel: NotRequired[RevenueModelType],  # (1)
    EffectiveDate: NotRequired[str],
    ExpirationDate: NotRequired[str],
    Value: NotRequired[MonetaryValueTypeDef],  # (2)
```

1. See [:material-code-brackets: RevenueModelType](./literals.md#revenuemodeltype) 
2. See [:material-code-braces: MonetaryValueTypeDef](./type_defs.md#monetaryvaluetypedef) 
## EngagementInvitationSummaryTypeDef

```python
# EngagementInvitationSummaryTypeDef definition

class EngagementInvitationSummaryTypeDef(TypedDict):
    Catalog: str,
    Id: str,
    Arn: NotRequired[str],
    EngagementId: NotRequired[str],
    EngagementTitle: NotRequired[str],
    ExpirationDate: NotRequired[datetime],
    InvitationDate: NotRequired[datetime],
    ParticipantType: NotRequired[ParticipantTypeType],  # (1)
    PayloadType: NotRequired[EngagementInvitationPayloadTypeType],  # (2)
    Receiver: NotRequired[ReceiverTypeDef],  # (3)
    SenderAwsAccountId: NotRequired[str],
    SenderCompanyName: NotRequired[str],
    Status: NotRequired[InvitationStatusType],  # (4)
```

1. See [:material-code-brackets: ParticipantTypeType](./literals.md#participanttypetype) 
2. See [:material-code-brackets: EngagementInvitationPayloadTypeType](./literals.md#engagementinvitationpayloadtypetype) 
3. See [:material-code-braces: ReceiverTypeDef](./type_defs.md#receivertypedef) 
4. See [:material-code-brackets: InvitationStatusType](./literals.md#invitationstatustype) 
## CustomerSummaryTypeDef

```python
# CustomerSummaryTypeDef definition

class CustomerSummaryTypeDef(TypedDict):
    Account: NotRequired[AccountSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: AccountSummaryTypeDef](./type_defs.md#accountsummarytypedef) 
## CustomerOutputTypeDef

```python
# CustomerOutputTypeDef definition

class CustomerOutputTypeDef(TypedDict):
    Account: NotRequired[AccountTypeDef],  # (1)
    Contacts: NotRequired[List[ContactTypeDef]],  # (2)
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 
2. See [:material-code-braces: ContactTypeDef](./type_defs.md#contacttypedef) 
## CustomerTypeDef

```python
# CustomerTypeDef definition

class CustomerTypeDef(TypedDict):
    Account: NotRequired[AccountTypeDef],  # (1)
    Contacts: NotRequired[Sequence[ContactTypeDef]],  # (2)
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 
2. See [:material-code-braces: ContactTypeDef](./type_defs.md#contacttypedef) 
## GetAwsOpportunitySummaryResponseTypeDef

```python
# GetAwsOpportunitySummaryResponseTypeDef definition

class GetAwsOpportunitySummaryResponseTypeDef(TypedDict):
    Catalog: str,
    Customer: AwsOpportunityCustomerTypeDef,  # (1)
    Insights: AwsOpportunityInsightsTypeDef,  # (2)
    InvolvementType: SalesInvolvementTypeType,  # (3)
    InvolvementTypeChangeReason: InvolvementTypeChangeReasonType,  # (4)
    LifeCycle: AwsOpportunityLifeCycleTypeDef,  # (5)
    OpportunityTeam: List[AwsTeamMemberTypeDef],  # (6)
    Origin: OpportunityOriginType,  # (7)
    Project: AwsOpportunityProjectTypeDef,  # (8)
    RelatedEntityIds: AwsOpportunityRelatedEntitiesTypeDef,  # (9)
    RelatedOpportunityId: str,
    Visibility: VisibilityType,  # (10)
    ResponseMetadata: ResponseMetadataTypeDef,  # (11)
```

1. See [:material-code-braces: AwsOpportunityCustomerTypeDef](./type_defs.md#awsopportunitycustomertypedef) 
2. See [:material-code-braces: AwsOpportunityInsightsTypeDef](./type_defs.md#awsopportunityinsightstypedef) 
3. See [:material-code-brackets: SalesInvolvementTypeType](./literals.md#salesinvolvementtypetype) 
4. See [:material-code-brackets: InvolvementTypeChangeReasonType](./literals.md#involvementtypechangereasontype) 
5. See [:material-code-braces: AwsOpportunityLifeCycleTypeDef](./type_defs.md#awsopportunitylifecycletypedef) 
6. See [:material-code-braces: AwsTeamMemberTypeDef](./type_defs.md#awsteammembertypedef) 
7. See [:material-code-brackets: OpportunityOriginType](./literals.md#opportunityorigintype) 
8. See [:material-code-braces: AwsOpportunityProjectTypeDef](./type_defs.md#awsopportunityprojecttypedef) 
9. See [:material-code-braces: AwsOpportunityRelatedEntitiesTypeDef](./type_defs.md#awsopportunityrelatedentitiestypedef) 
10. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
11. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OpportunityInvitationPayloadOutputTypeDef

```python
# OpportunityInvitationPayloadOutputTypeDef definition

class OpportunityInvitationPayloadOutputTypeDef(TypedDict):
    Customer: EngagementCustomerTypeDef,  # (1)
    Project: ProjectDetailsOutputTypeDef,  # (2)
    ReceiverResponsibilities: List[ReceiverResponsibilityType],  # (3)
    SenderContacts: NotRequired[List[SenderContactTypeDef]],  # (4)
```

1. See [:material-code-braces: EngagementCustomerTypeDef](./type_defs.md#engagementcustomertypedef) 
2. See [:material-code-braces: ProjectDetailsOutputTypeDef](./type_defs.md#projectdetailsoutputtypedef) 
3. See [:material-code-brackets: ReceiverResponsibilityType](./literals.md#receiverresponsibilitytype) 
4. See [:material-code-braces: SenderContactTypeDef](./type_defs.md#sendercontacttypedef) 
## EngagementContextPayloadTypeDef

```python
# EngagementContextPayloadTypeDef definition

class EngagementContextPayloadTypeDef(TypedDict):
    CustomerProject: NotRequired[CustomerProjectsContextTypeDef],  # (1)
```

1. See [:material-code-braces: CustomerProjectsContextTypeDef](./type_defs.md#customerprojectscontexttypedef) 
## ListOpportunitiesRequestPaginateTypeDef

```python
# ListOpportunitiesRequestPaginateTypeDef definition

class ListOpportunitiesRequestPaginateTypeDef(TypedDict):
    Catalog: str,
    CustomerCompanyName: NotRequired[Sequence[str]],
    Identifier: NotRequired[Sequence[str]],
    LastModifiedDate: NotRequired[LastModifiedDateTypeDef],  # (1)
    LifeCycleReviewStatus: NotRequired[Sequence[ReviewStatusType]],  # (2)
    LifeCycleStage: NotRequired[Sequence[StageType]],  # (3)
    Sort: NotRequired[OpportunitySortTypeDef],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-braces: LastModifiedDateTypeDef](./type_defs.md#lastmodifieddatetypedef) 
2. See [:material-code-brackets: ReviewStatusType](./literals.md#reviewstatustype) 
3. See [:material-code-brackets: StageType](./literals.md#stagetype) 
4. See [:material-code-braces: OpportunitySortTypeDef](./type_defs.md#opportunitysorttypedef) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOpportunitiesRequestRequestTypeDef

```python
# ListOpportunitiesRequestRequestTypeDef definition

class ListOpportunitiesRequestRequestTypeDef(TypedDict):
    Catalog: str,
    CustomerCompanyName: NotRequired[Sequence[str]],
    Identifier: NotRequired[Sequence[str]],
    LastModifiedDate: NotRequired[LastModifiedDateTypeDef],  # (1)
    LifeCycleReviewStatus: NotRequired[Sequence[ReviewStatusType]],  # (2)
    LifeCycleStage: NotRequired[Sequence[StageType]],  # (3)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Sort: NotRequired[OpportunitySortTypeDef],  # (4)
```

1. See [:material-code-braces: LastModifiedDateTypeDef](./type_defs.md#lastmodifieddatetypedef) 
2. See [:material-code-brackets: ReviewStatusType](./literals.md#reviewstatustype) 
3. See [:material-code-brackets: StageType](./literals.md#stagetype) 
4. See [:material-code-braces: OpportunitySortTypeDef](./type_defs.md#opportunitysorttypedef) 
## ListEngagementInvitationsResponseTypeDef

```python
# ListEngagementInvitationsResponseTypeDef definition

class ListEngagementInvitationsResponseTypeDef(TypedDict):
    EngagementInvitationSummaries: List[EngagementInvitationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EngagementInvitationSummaryTypeDef](./type_defs.md#engagementinvitationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OpportunitySummaryTypeDef

```python
# OpportunitySummaryTypeDef definition

class OpportunitySummaryTypeDef(TypedDict):
    Catalog: str,
    Arn: NotRequired[str],
    CreatedDate: NotRequired[datetime],
    Customer: NotRequired[CustomerSummaryTypeDef],  # (1)
    Id: NotRequired[str],
    LastModifiedDate: NotRequired[datetime],
    LifeCycle: NotRequired[LifeCycleSummaryTypeDef],  # (2)
    OpportunityType: NotRequired[OpportunityTypeType],  # (3)
    PartnerOpportunityIdentifier: NotRequired[str],
    Project: NotRequired[ProjectSummaryTypeDef],  # (4)
```

1. See [:material-code-braces: CustomerSummaryTypeDef](./type_defs.md#customersummarytypedef) 
2. See [:material-code-braces: LifeCycleSummaryTypeDef](./type_defs.md#lifecyclesummarytypedef) 
3. See [:material-code-brackets: OpportunityTypeType](./literals.md#opportunitytypetype) 
4. See [:material-code-braces: ProjectSummaryTypeDef](./type_defs.md#projectsummarytypedef) 
## GetOpportunityResponseTypeDef

```python
# GetOpportunityResponseTypeDef definition

class GetOpportunityResponseTypeDef(TypedDict):
    Arn: str,
    Catalog: str,
    CreatedDate: datetime,
    Customer: CustomerOutputTypeDef,  # (1)
    Id: str,
    LastModifiedDate: datetime,
    LifeCycle: LifeCycleOutputTypeDef,  # (2)
    Marketing: MarketingOutputTypeDef,  # (3)
    NationalSecurity: NationalSecurityType,  # (4)
    OpportunityTeam: List[ContactTypeDef],  # (5)
    OpportunityType: OpportunityTypeType,  # (6)
    PartnerOpportunityIdentifier: str,
    PrimaryNeedsFromAws: List[PrimaryNeedFromAwsType],  # (7)
    Project: ProjectOutputTypeDef,  # (8)
    RelatedEntityIdentifiers: RelatedEntityIdentifiersTypeDef,  # (9)
    SoftwareRevenue: SoftwareRevenueTypeDef,  # (10)
    ResponseMetadata: ResponseMetadataTypeDef,  # (11)
```

1. See [:material-code-braces: CustomerOutputTypeDef](./type_defs.md#customeroutputtypedef) 
2. See [:material-code-braces: LifeCycleOutputTypeDef](./type_defs.md#lifecycleoutputtypedef) 
3. See [:material-code-braces: MarketingOutputTypeDef](./type_defs.md#marketingoutputtypedef) 
4. See [:material-code-brackets: NationalSecurityType](./literals.md#nationalsecuritytype) 
5. See [:material-code-braces: ContactTypeDef](./type_defs.md#contacttypedef) 
6. See [:material-code-brackets: OpportunityTypeType](./literals.md#opportunitytypetype) 
7. See [:material-code-brackets: PrimaryNeedFromAwsType](./literals.md#primaryneedfromawstype) 
8. See [:material-code-braces: ProjectOutputTypeDef](./type_defs.md#projectoutputtypedef) 
9. See [:material-code-braces: RelatedEntityIdentifiersTypeDef](./type_defs.md#relatedentityidentifierstypedef) 
10. See [:material-code-braces: SoftwareRevenueTypeDef](./type_defs.md#softwarerevenuetypedef) 
11. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OpportunitySummaryViewTypeDef

```python
# OpportunitySummaryViewTypeDef definition

class OpportunitySummaryViewTypeDef(TypedDict):
    Customer: NotRequired[CustomerOutputTypeDef],  # (1)
    Lifecycle: NotRequired[LifeCycleForViewTypeDef],  # (2)
    OpportunityTeam: NotRequired[List[ContactTypeDef]],  # (3)
    OpportunityType: NotRequired[OpportunityTypeType],  # (4)
    PrimaryNeedsFromAws: NotRequired[List[PrimaryNeedFromAwsType]],  # (5)
    Project: NotRequired[ProjectViewTypeDef],  # (6)
    RelatedEntityIdentifiers: NotRequired[RelatedEntityIdentifiersTypeDef],  # (7)
```

1. See [:material-code-braces: CustomerOutputTypeDef](./type_defs.md#customeroutputtypedef) 
2. See [:material-code-braces: LifeCycleForViewTypeDef](./type_defs.md#lifecycleforviewtypedef) 
3. See [:material-code-braces: ContactTypeDef](./type_defs.md#contacttypedef) 
4. See [:material-code-brackets: OpportunityTypeType](./literals.md#opportunitytypetype) 
5. See [:material-code-brackets: PrimaryNeedFromAwsType](./literals.md#primaryneedfromawstype) 
6. See [:material-code-braces: ProjectViewTypeDef](./type_defs.md#projectviewtypedef) 
7. See [:material-code-braces: RelatedEntityIdentifiersTypeDef](./type_defs.md#relatedentityidentifierstypedef) 
## PayloadOutputTypeDef

```python
# PayloadOutputTypeDef definition

class PayloadOutputTypeDef(TypedDict):
    OpportunityInvitation: NotRequired[OpportunityInvitationPayloadOutputTypeDef],  # (1)
```

1. See [:material-code-braces: OpportunityInvitationPayloadOutputTypeDef](./type_defs.md#opportunityinvitationpayloadoutputtypedef) 
## OpportunityInvitationPayloadTypeDef

```python
# OpportunityInvitationPayloadTypeDef definition

class OpportunityInvitationPayloadTypeDef(TypedDict):
    Customer: EngagementCustomerTypeDef,  # (1)
    Project: ProjectDetailsUnionTypeDef,  # (2)
    ReceiverResponsibilities: Sequence[ReceiverResponsibilityType],  # (3)
    SenderContacts: NotRequired[Sequence[SenderContactTypeDef]],  # (4)
```

1. See [:material-code-braces: EngagementCustomerTypeDef](./type_defs.md#engagementcustomertypedef) 
2. See [:material-code-braces: ProjectDetailsTypeDef](./type_defs.md#projectdetailstypedef) [:material-code-braces: ProjectDetailsOutputTypeDef](./type_defs.md#projectdetailsoutputtypedef) 
3. See [:material-code-brackets: ReceiverResponsibilityType](./literals.md#receiverresponsibilitytype) 
4. See [:material-code-braces: SenderContactTypeDef](./type_defs.md#sendercontacttypedef) 
## EngagementContextDetailsTypeDef

```python
# EngagementContextDetailsTypeDef definition

class EngagementContextDetailsTypeDef(TypedDict):
    Type: EngagementContextTypeType,  # (2)
    Payload: NotRequired[EngagementContextPayloadTypeDef],  # (1)
```

1. See [:material-code-braces: EngagementContextPayloadTypeDef](./type_defs.md#engagementcontextpayloadtypedef) 
2. See [:material-code-brackets: EngagementContextTypeType](./literals.md#engagementcontexttypetype) 
## LifeCycleTypeDef

```python
# LifeCycleTypeDef definition

class LifeCycleTypeDef(TypedDict):
    ClosedLostReason: NotRequired[ClosedLostReasonType],  # (1)
    NextSteps: NotRequired[str],
    NextStepsHistory: NotRequired[Sequence[NextStepsHistoryUnionTypeDef]],  # (2)
    ReviewComments: NotRequired[str],
    ReviewStatus: NotRequired[ReviewStatusType],  # (3)
    ReviewStatusReason: NotRequired[str],
    Stage: NotRequired[StageType],  # (4)
    TargetCloseDate: NotRequired[str],
```

1. See [:material-code-brackets: ClosedLostReasonType](./literals.md#closedlostreasontype) 
2. See [:material-code-braces: NextStepsHistoryTypeDef](./type_defs.md#nextstepshistorytypedef) [:material-code-braces: NextStepsHistoryOutputTypeDef](./type_defs.md#nextstepshistoryoutputtypedef) 
3. See [:material-code-brackets: ReviewStatusType](./literals.md#reviewstatustype) 
4. See [:material-code-brackets: StageType](./literals.md#stagetype) 
## ListOpportunitiesResponseTypeDef

```python
# ListOpportunitiesResponseTypeDef definition

class ListOpportunitiesResponseTypeDef(TypedDict):
    OpportunitySummaries: List[OpportunitySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OpportunitySummaryTypeDef](./type_defs.md#opportunitysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResourceSnapshotPayloadTypeDef

```python
# ResourceSnapshotPayloadTypeDef definition

class ResourceSnapshotPayloadTypeDef(TypedDict):
    OpportunitySummary: NotRequired[OpportunitySummaryViewTypeDef],  # (1)
```

1. See [:material-code-braces: OpportunitySummaryViewTypeDef](./type_defs.md#opportunitysummaryviewtypedef) 
## GetEngagementInvitationResponseTypeDef

```python
# GetEngagementInvitationResponseTypeDef definition

class GetEngagementInvitationResponseTypeDef(TypedDict):
    Arn: str,
    Catalog: str,
    EngagementDescription: str,
    EngagementId: str,
    EngagementTitle: str,
    ExistingMembers: List[EngagementMemberSummaryTypeDef],  # (1)
    ExpirationDate: datetime,
    Id: str,
    InvitationDate: datetime,
    InvitationMessage: str,
    Payload: PayloadOutputTypeDef,  # (2)
    PayloadType: EngagementInvitationPayloadTypeType,  # (3)
    Receiver: ReceiverTypeDef,  # (4)
    RejectionReason: str,
    SenderAwsAccountId: str,
    SenderCompanyName: str,
    Status: InvitationStatusType,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: EngagementMemberSummaryTypeDef](./type_defs.md#engagementmembersummarytypedef) 
2. See [:material-code-braces: PayloadOutputTypeDef](./type_defs.md#payloadoutputtypedef) 
3. See [:material-code-brackets: EngagementInvitationPayloadTypeType](./literals.md#engagementinvitationpayloadtypetype) 
4. See [:material-code-braces: ReceiverTypeDef](./type_defs.md#receivertypedef) 
5. See [:material-code-brackets: InvitationStatusType](./literals.md#invitationstatustype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEngagementRequestRequestTypeDef

```python
# CreateEngagementRequestRequestTypeDef definition

class CreateEngagementRequestRequestTypeDef(TypedDict):
    Catalog: str,
    ClientToken: str,
    Description: str,
    Title: str,
    Contexts: NotRequired[Sequence[EngagementContextDetailsTypeDef]],  # (1)
```

1. See [:material-code-braces: EngagementContextDetailsTypeDef](./type_defs.md#engagementcontextdetailstypedef) 
## GetEngagementResponseTypeDef

```python
# GetEngagementResponseTypeDef definition

class GetEngagementResponseTypeDef(TypedDict):
    Arn: str,
    Contexts: List[EngagementContextDetailsTypeDef],  # (1)
    CreatedAt: datetime,
    CreatedBy: str,
    Description: str,
    Id: str,
    MemberCount: int,
    Title: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EngagementContextDetailsTypeDef](./type_defs.md#engagementcontextdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateOpportunityRequestRequestTypeDef

```python
# CreateOpportunityRequestRequestTypeDef definition

class CreateOpportunityRequestRequestTypeDef(TypedDict):
    Catalog: str,
    ClientToken: str,
    Customer: NotRequired[CustomerTypeDef],  # (1)
    LifeCycle: NotRequired[LifeCycleTypeDef],  # (2)
    Marketing: NotRequired[MarketingTypeDef],  # (3)
    NationalSecurity: NotRequired[NationalSecurityType],  # (4)
    OpportunityTeam: NotRequired[Sequence[ContactTypeDef]],  # (5)
    OpportunityType: NotRequired[OpportunityTypeType],  # (6)
    Origin: NotRequired[OpportunityOriginType],  # (7)
    PartnerOpportunityIdentifier: NotRequired[str],
    PrimaryNeedsFromAws: NotRequired[Sequence[PrimaryNeedFromAwsType]],  # (8)
    Project: NotRequired[ProjectTypeDef],  # (9)
    SoftwareRevenue: NotRequired[SoftwareRevenueTypeDef],  # (10)
```

1. See [:material-code-braces: CustomerTypeDef](./type_defs.md#customertypedef) 
2. See [:material-code-braces: LifeCycleTypeDef](./type_defs.md#lifecycletypedef) 
3. See [:material-code-braces: MarketingTypeDef](./type_defs.md#marketingtypedef) 
4. See [:material-code-brackets: NationalSecurityType](./literals.md#nationalsecuritytype) 
5. See [:material-code-braces: ContactTypeDef](./type_defs.md#contacttypedef) 
6. See [:material-code-brackets: OpportunityTypeType](./literals.md#opportunitytypetype) 
7. See [:material-code-brackets: OpportunityOriginType](./literals.md#opportunityorigintype) 
8. See [:material-code-brackets: PrimaryNeedFromAwsType](./literals.md#primaryneedfromawstype) 
9. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) 
10. See [:material-code-braces: SoftwareRevenueTypeDef](./type_defs.md#softwarerevenuetypedef) 
## UpdateOpportunityRequestRequestTypeDef

```python
# UpdateOpportunityRequestRequestTypeDef definition

class UpdateOpportunityRequestRequestTypeDef(TypedDict):
    Catalog: str,
    Identifier: str,
    LastModifiedDate: TimestampTypeDef,
    Customer: NotRequired[CustomerTypeDef],  # (1)
    LifeCycle: NotRequired[LifeCycleTypeDef],  # (2)
    Marketing: NotRequired[MarketingTypeDef],  # (3)
    NationalSecurity: NotRequired[NationalSecurityType],  # (4)
    OpportunityType: NotRequired[OpportunityTypeType],  # (5)
    PartnerOpportunityIdentifier: NotRequired[str],
    PrimaryNeedsFromAws: NotRequired[Sequence[PrimaryNeedFromAwsType]],  # (6)
    Project: NotRequired[ProjectTypeDef],  # (7)
    SoftwareRevenue: NotRequired[SoftwareRevenueTypeDef],  # (8)
```

1. See [:material-code-braces: CustomerTypeDef](./type_defs.md#customertypedef) 
2. See [:material-code-braces: LifeCycleTypeDef](./type_defs.md#lifecycletypedef) 
3. See [:material-code-braces: MarketingTypeDef](./type_defs.md#marketingtypedef) 
4. See [:material-code-brackets: NationalSecurityType](./literals.md#nationalsecuritytype) 
5. See [:material-code-brackets: OpportunityTypeType](./literals.md#opportunitytypetype) 
6. See [:material-code-brackets: PrimaryNeedFromAwsType](./literals.md#primaryneedfromawstype) 
7. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) 
8. See [:material-code-braces: SoftwareRevenueTypeDef](./type_defs.md#softwarerevenuetypedef) 
## GetResourceSnapshotResponseTypeDef

```python
# GetResourceSnapshotResponseTypeDef definition

class GetResourceSnapshotResponseTypeDef(TypedDict):
    Arn: str,
    Catalog: str,
    CreatedAt: datetime,
    CreatedBy: str,
    EngagementId: str,
    Payload: ResourceSnapshotPayloadTypeDef,  # (1)
    ResourceId: str,
    ResourceSnapshotTemplateName: str,
    ResourceType: ResourceTypeType,  # (2)
    Revision: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ResourceSnapshotPayloadTypeDef](./type_defs.md#resourcesnapshotpayloadtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PayloadTypeDef

```python
# PayloadTypeDef definition

class PayloadTypeDef(TypedDict):
    OpportunityInvitation: NotRequired[OpportunityInvitationPayloadUnionTypeDef],  # (1)
```

1. See [:material-code-braces: OpportunityInvitationPayloadTypeDef](./type_defs.md#opportunityinvitationpayloadtypedef) [:material-code-braces: OpportunityInvitationPayloadOutputTypeDef](./type_defs.md#opportunityinvitationpayloadoutputtypedef) 
## InvitationTypeDef

```python
# InvitationTypeDef definition

class InvitationTypeDef(TypedDict):
    Message: str,
    Payload: PayloadUnionTypeDef,  # (1)
    Receiver: ReceiverTypeDef,  # (2)
```

1. See [:material-code-braces: PayloadTypeDef](./type_defs.md#payloadtypedef) [:material-code-braces: PayloadOutputTypeDef](./type_defs.md#payloadoutputtypedef) 
2. See [:material-code-braces: ReceiverTypeDef](./type_defs.md#receivertypedef) 
## CreateEngagementInvitationRequestRequestTypeDef

```python
# CreateEngagementInvitationRequestRequestTypeDef definition

class CreateEngagementInvitationRequestRequestTypeDef(TypedDict):
    Catalog: str,
    ClientToken: str,
    EngagementIdentifier: str,
    Invitation: InvitationTypeDef,  # (1)
```

1. See [:material-code-braces: InvitationTypeDef](./type_defs.md#invitationtypedef) 
