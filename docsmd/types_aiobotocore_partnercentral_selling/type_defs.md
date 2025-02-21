# Type definitions

> [Index](../README.md) > [PartnerCentralSellingAPI](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [PartnerCentralSellingAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#partnercentralsellingapi)
    type annotations stubs module [types-aiobotocore-partnercentral-selling](https://pypi.org/project/types-aiobotocore-partnercentral-selling/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_partnercentral_selling.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## MarketingUnionTypeDef

```python
# MarketingUnionTypeDef Union usage example

from types_aiobotocore_partnercentral_selling.type_defs import MarketingUnionTypeDef


def get_value() -> MarketingUnionTypeDef:
    return ...


# MarketingUnionTypeDef definition

MarketingUnionTypeDef = Union[
    MarketingTypeDef,  # (1)
    MarketingOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MarketingTypeDef](./type_defs.md#marketingtypedef) 
2. See [:material-code-braces: MarketingOutputTypeDef](./type_defs.md#marketingoutputtypedef) 

## ProjectDetailsUnionTypeDef

```python
# ProjectDetailsUnionTypeDef Union usage example

from types_aiobotocore_partnercentral_selling.type_defs import ProjectDetailsUnionTypeDef


def get_value() -> ProjectDetailsUnionTypeDef:
    return ...


# ProjectDetailsUnionTypeDef definition

ProjectDetailsUnionTypeDef = Union[
    ProjectDetailsTypeDef,  # (1)
    ProjectDetailsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ProjectDetailsTypeDef](./type_defs.md#projectdetailstypedef) 
2. See [:material-code-braces: ProjectDetailsOutputTypeDef](./type_defs.md#projectdetailsoutputtypedef) 

## ProjectUnionTypeDef

```python
# ProjectUnionTypeDef Union usage example

from types_aiobotocore_partnercentral_selling.type_defs import ProjectUnionTypeDef


def get_value() -> ProjectUnionTypeDef:
    return ...


# ProjectUnionTypeDef definition

ProjectUnionTypeDef = Union[
    ProjectTypeDef,  # (1)
    ProjectOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) 
2. See [:material-code-braces: ProjectOutputTypeDef](./type_defs.md#projectoutputtypedef) 

## CustomerUnionTypeDef

```python
# CustomerUnionTypeDef Union usage example

from types_aiobotocore_partnercentral_selling.type_defs import CustomerUnionTypeDef


def get_value() -> CustomerUnionTypeDef:
    return ...


# CustomerUnionTypeDef definition

CustomerUnionTypeDef = Union[
    CustomerTypeDef,  # (1)
    CustomerOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CustomerTypeDef](./type_defs.md#customertypedef) 
2. See [:material-code-braces: CustomerOutputTypeDef](./type_defs.md#customeroutputtypedef) 

## LifeCycleUnionTypeDef

```python
# LifeCycleUnionTypeDef Union usage example

from types_aiobotocore_partnercentral_selling.type_defs import LifeCycleUnionTypeDef


def get_value() -> LifeCycleUnionTypeDef:
    return ...


# LifeCycleUnionTypeDef definition

LifeCycleUnionTypeDef = Union[
    LifeCycleTypeDef,  # (1)
    LifeCycleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: LifeCycleTypeDef](./type_defs.md#lifecycletypedef) 
2. See [:material-code-braces: LifeCycleOutputTypeDef](./type_defs.md#lifecycleoutputtypedef) 

## OpportunityInvitationPayloadUnionTypeDef

```python
# OpportunityInvitationPayloadUnionTypeDef Union usage example

from types_aiobotocore_partnercentral_selling.type_defs import OpportunityInvitationPayloadUnionTypeDef


def get_value() -> OpportunityInvitationPayloadUnionTypeDef:
    return ...


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
# PayloadUnionTypeDef Union usage example

from types_aiobotocore_partnercentral_selling.type_defs import PayloadUnionTypeDef


def get_value() -> PayloadUnionTypeDef:
    return ...


# PayloadUnionTypeDef definition

PayloadUnionTypeDef = Union[
    PayloadTypeDef,  # (1)
    PayloadOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PayloadTypeDef](./type_defs.md#payloadtypedef) 
2. See [:material-code-braces: PayloadOutputTypeDef](./type_defs.md#payloadoutputtypedef) 



## AcceptEngagementInvitationRequestTypeDef

```python
# AcceptEngagementInvitationRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import AcceptEngagementInvitationRequestTypeDef


def get_value() -> AcceptEngagementInvitationRequestTypeDef:
    return {
        "Catalog": ...,
    }


# AcceptEngagementInvitationRequestTypeDef definition

class AcceptEngagementInvitationRequestTypeDef(TypedDict):
    Catalog: str,
    Identifier: str,
```

## AccountReceiverTypeDef

```python
# AccountReceiverTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import AccountReceiverTypeDef


def get_value() -> AccountReceiverTypeDef:
    return {
        "Alias": ...,
    }


# AccountReceiverTypeDef definition

class AccountReceiverTypeDef(TypedDict):
    AwsAccountId: str,
    Alias: NotRequired[str],
```

## AddressSummaryTypeDef

```python
# AddressSummaryTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import AddressSummaryTypeDef


def get_value() -> AddressSummaryTypeDef:
    return {
        "City": ...,
    }


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
# AddressTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import AddressTypeDef


def get_value() -> AddressTypeDef:
    return {
        "City": ...,
    }


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
# AssigneeContactTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import AssigneeContactTypeDef


def get_value() -> AssigneeContactTypeDef:
    return {
        "BusinessTitle": ...,
    }


# AssigneeContactTypeDef definition

class AssigneeContactTypeDef(TypedDict):
    BusinessTitle: str,
    Email: str,
    FirstName: str,
    LastName: str,
```

## AssociateOpportunityRequestTypeDef

```python
# AssociateOpportunityRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import AssociateOpportunityRequestTypeDef


def get_value() -> AssociateOpportunityRequestTypeDef:
    return {
        "Catalog": ...,
    }


# AssociateOpportunityRequestTypeDef definition

class AssociateOpportunityRequestTypeDef(TypedDict):
    Catalog: str,
    OpportunityIdentifier: str,
    RelatedEntityIdentifier: str,
    RelatedEntityType: RelatedEntityTypeType,  # (1)
```

1. See [:material-code-brackets: RelatedEntityTypeType](./literals.md#relatedentitytypetype) 
## ContactTypeDef

```python
# ContactTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ContactTypeDef


def get_value() -> ContactTypeDef:
    return {
        "BusinessTitle": ...,
    }


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
# AwsOpportunityInsightsTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import AwsOpportunityInsightsTypeDef


def get_value() -> AwsOpportunityInsightsTypeDef:
    return {
        "EngagementScore": ...,
    }


# AwsOpportunityInsightsTypeDef definition

class AwsOpportunityInsightsTypeDef(TypedDict):
    EngagementScore: NotRequired[EngagementScoreType],  # (1)
    NextBestActions: NotRequired[str],
```

1. See [:material-code-brackets: EngagementScoreType](./literals.md#engagementscoretype) 
## ProfileNextStepsHistoryTypeDef

```python
# ProfileNextStepsHistoryTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ProfileNextStepsHistoryTypeDef


def get_value() -> ProfileNextStepsHistoryTypeDef:
    return {
        "Time": ...,
    }


# ProfileNextStepsHistoryTypeDef definition

class ProfileNextStepsHistoryTypeDef(TypedDict):
    Time: datetime,
    Value: str,
```

## ExpectedCustomerSpendTypeDef

```python
# ExpectedCustomerSpendTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ExpectedCustomerSpendTypeDef


def get_value() -> ExpectedCustomerSpendTypeDef:
    return {
        "Amount": ...,
    }


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
# AwsOpportunityRelatedEntitiesTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import AwsOpportunityRelatedEntitiesTypeDef


def get_value() -> AwsOpportunityRelatedEntitiesTypeDef:
    return {
        "AwsProducts": ...,
    }


# AwsOpportunityRelatedEntitiesTypeDef definition

class AwsOpportunityRelatedEntitiesTypeDef(TypedDict):
    AwsProducts: NotRequired[List[str]],
    Solutions: NotRequired[List[str]],
```

## AwsSubmissionTypeDef

```python
# AwsSubmissionTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import AwsSubmissionTypeDef


def get_value() -> AwsSubmissionTypeDef:
    return {
        "InvolvementType": ...,
    }


# AwsSubmissionTypeDef definition

class AwsSubmissionTypeDef(TypedDict):
    InvolvementType: SalesInvolvementTypeType,  # (1)
    Visibility: NotRequired[VisibilityType],  # (2)
```

1. See [:material-code-brackets: SalesInvolvementTypeType](./literals.md#salesinvolvementtypetype) 
2. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## AwsTeamMemberTypeDef

```python
# AwsTeamMemberTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import AwsTeamMemberTypeDef


def get_value() -> AwsTeamMemberTypeDef:
    return {
        "BusinessTitle": ...,
    }


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
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ResponseMetadataTypeDef


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

## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "Key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## CreateResourceSnapshotRequestTypeDef

```python
# CreateResourceSnapshotRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import CreateResourceSnapshotRequestTypeDef


def get_value() -> CreateResourceSnapshotRequestTypeDef:
    return {
        "Catalog": ...,
    }


# CreateResourceSnapshotRequestTypeDef definition

class CreateResourceSnapshotRequestTypeDef(TypedDict):
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
# EngagementCustomerProjectDetailsTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import EngagementCustomerProjectDetailsTypeDef


def get_value() -> EngagementCustomerProjectDetailsTypeDef:
    return {
        "BusinessProblem": ...,
    }


# EngagementCustomerProjectDetailsTypeDef definition

class EngagementCustomerProjectDetailsTypeDef(TypedDict):
    BusinessProblem: str,
    TargetCompletionDate: str,
    Title: str,
```

## EngagementCustomerTypeDef

```python
# EngagementCustomerTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import EngagementCustomerTypeDef


def get_value() -> EngagementCustomerTypeDef:
    return {
        "CompanyName": ...,
    }


# EngagementCustomerTypeDef definition

class EngagementCustomerTypeDef(TypedDict):
    CompanyName: str,
    CountryCode: CountryCodeType,  # (1)
    Industry: IndustryType,  # (2)
    WebsiteUrl: str,
```

1. See [:material-code-brackets: CountryCodeType](./literals.md#countrycodetype) 
2. See [:material-code-brackets: IndustryType](./literals.md#industrytype) 
## DeleteResourceSnapshotJobRequestTypeDef

```python
# DeleteResourceSnapshotJobRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import DeleteResourceSnapshotJobRequestTypeDef


def get_value() -> DeleteResourceSnapshotJobRequestTypeDef:
    return {
        "Catalog": ...,
    }


# DeleteResourceSnapshotJobRequestTypeDef definition

class DeleteResourceSnapshotJobRequestTypeDef(TypedDict):
    Catalog: str,
    ResourceSnapshotJobIdentifier: str,
```

## DisassociateOpportunityRequestTypeDef

```python
# DisassociateOpportunityRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import DisassociateOpportunityRequestTypeDef


def get_value() -> DisassociateOpportunityRequestTypeDef:
    return {
        "Catalog": ...,
    }


# DisassociateOpportunityRequestTypeDef definition

class DisassociateOpportunityRequestTypeDef(TypedDict):
    Catalog: str,
    OpportunityIdentifier: str,
    RelatedEntityIdentifier: str,
    RelatedEntityType: RelatedEntityTypeType,  # (1)
```

1. See [:material-code-brackets: RelatedEntityTypeType](./literals.md#relatedentitytypetype) 
## EngagementMemberSummaryTypeDef

```python
# EngagementMemberSummaryTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import EngagementMemberSummaryTypeDef


def get_value() -> EngagementMemberSummaryTypeDef:
    return {
        "CompanyName": ...,
    }


# EngagementMemberSummaryTypeDef definition

class EngagementMemberSummaryTypeDef(TypedDict):
    CompanyName: NotRequired[str],
    WebsiteUrl: NotRequired[str],
```

## EngagementMemberTypeDef

```python
# EngagementMemberTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import EngagementMemberTypeDef


def get_value() -> EngagementMemberTypeDef:
    return {
        "AccountId": ...,
    }


# EngagementMemberTypeDef definition

class EngagementMemberTypeDef(TypedDict):
    AccountId: NotRequired[str],
    CompanyName: NotRequired[str],
    WebsiteUrl: NotRequired[str],
```

## EngagementResourceAssociationSummaryTypeDef

```python
# EngagementResourceAssociationSummaryTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import EngagementResourceAssociationSummaryTypeDef


def get_value() -> EngagementResourceAssociationSummaryTypeDef:
    return {
        "Catalog": ...,
    }


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
# EngagementSortTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import EngagementSortTypeDef


def get_value() -> EngagementSortTypeDef:
    return {
        "SortBy": ...,
    }


# EngagementSortTypeDef definition

class EngagementSortTypeDef(TypedDict):
    SortBy: EngagementSortNameType,  # (1)
    SortOrder: SortOrderType,  # (2)
```

1. See [:material-code-brackets: EngagementSortNameType](./literals.md#engagementsortnametype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## EngagementSummaryTypeDef

```python
# EngagementSummaryTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import EngagementSummaryTypeDef


def get_value() -> EngagementSummaryTypeDef:
    return {
        "Arn": ...,
    }


# EngagementSummaryTypeDef definition

class EngagementSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    CreatedBy: NotRequired[str],
    Id: NotRequired[str],
    MemberCount: NotRequired[int],
    Title: NotRequired[str],
```

## GetAwsOpportunitySummaryRequestTypeDef

```python
# GetAwsOpportunitySummaryRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import GetAwsOpportunitySummaryRequestTypeDef


def get_value() -> GetAwsOpportunitySummaryRequestTypeDef:
    return {
        "Catalog": ...,
    }


# GetAwsOpportunitySummaryRequestTypeDef definition

class GetAwsOpportunitySummaryRequestTypeDef(TypedDict):
    Catalog: str,
    RelatedOpportunityIdentifier: str,
```

## GetEngagementInvitationRequestTypeDef

```python
# GetEngagementInvitationRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import GetEngagementInvitationRequestTypeDef


def get_value() -> GetEngagementInvitationRequestTypeDef:
    return {
        "Catalog": ...,
    }


# GetEngagementInvitationRequestTypeDef definition

class GetEngagementInvitationRequestTypeDef(TypedDict):
    Catalog: str,
    Identifier: str,
```

## GetEngagementRequestTypeDef

```python
# GetEngagementRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import GetEngagementRequestTypeDef


def get_value() -> GetEngagementRequestTypeDef:
    return {
        "Catalog": ...,
    }


# GetEngagementRequestTypeDef definition

class GetEngagementRequestTypeDef(TypedDict):
    Catalog: str,
    Identifier: str,
```

## GetOpportunityRequestTypeDef

```python
# GetOpportunityRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import GetOpportunityRequestTypeDef


def get_value() -> GetOpportunityRequestTypeDef:
    return {
        "Catalog": ...,
    }


# GetOpportunityRequestTypeDef definition

class GetOpportunityRequestTypeDef(TypedDict):
    Catalog: str,
    Identifier: str,
```

## MarketingOutputTypeDef

```python
# MarketingOutputTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import MarketingOutputTypeDef


def get_value() -> MarketingOutputTypeDef:
    return {
        "AwsFundingUsed": ...,
    }


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
# RelatedEntityIdentifiersTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import RelatedEntityIdentifiersTypeDef


def get_value() -> RelatedEntityIdentifiersTypeDef:
    return {
        "AwsMarketplaceOffers": ...,
    }


# RelatedEntityIdentifiersTypeDef definition

class RelatedEntityIdentifiersTypeDef(TypedDict):
    AwsMarketplaceOffers: NotRequired[List[str]],
    AwsProducts: NotRequired[List[str]],
    Solutions: NotRequired[List[str]],
```

## GetResourceSnapshotJobRequestTypeDef

```python
# GetResourceSnapshotJobRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import GetResourceSnapshotJobRequestTypeDef


def get_value() -> GetResourceSnapshotJobRequestTypeDef:
    return {
        "Catalog": ...,
    }


# GetResourceSnapshotJobRequestTypeDef definition

class GetResourceSnapshotJobRequestTypeDef(TypedDict):
    Catalog: str,
    ResourceSnapshotJobIdentifier: str,
```

## GetResourceSnapshotRequestTypeDef

```python
# GetResourceSnapshotRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import GetResourceSnapshotRequestTypeDef


def get_value() -> GetResourceSnapshotRequestTypeDef:
    return {
        "Catalog": ...,
    }


# GetResourceSnapshotRequestTypeDef definition

class GetResourceSnapshotRequestTypeDef(TypedDict):
    Catalog: str,
    EngagementIdentifier: str,
    ResourceIdentifier: str,
    ResourceSnapshotTemplateIdentifier: str,
    ResourceType: ResourceTypeType,  # (1)
    Revision: NotRequired[int],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## GetSellingSystemSettingsRequestTypeDef

```python
# GetSellingSystemSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import GetSellingSystemSettingsRequestTypeDef


def get_value() -> GetSellingSystemSettingsRequestTypeDef:
    return {
        "Catalog": ...,
    }


# GetSellingSystemSettingsRequestTypeDef definition

class GetSellingSystemSettingsRequestTypeDef(TypedDict):
    Catalog: str,
```

## LifeCycleForViewTypeDef

```python
# LifeCycleForViewTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import LifeCycleForViewTypeDef


def get_value() -> LifeCycleForViewTypeDef:
    return {
        "NextSteps": ...,
    }


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
# NextStepsHistoryOutputTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import NextStepsHistoryOutputTypeDef


def get_value() -> NextStepsHistoryOutputTypeDef:
    return {
        "Time": ...,
    }


# NextStepsHistoryOutputTypeDef definition

class NextStepsHistoryOutputTypeDef(TypedDict):
    Time: datetime,
    Value: str,
```

## LifeCycleSummaryTypeDef

```python
# LifeCycleSummaryTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import LifeCycleSummaryTypeDef


def get_value() -> LifeCycleSummaryTypeDef:
    return {
        "ClosedLostReason": ...,
    }


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
# ListEngagementByAcceptingInvitationTaskSummaryTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListEngagementByAcceptingInvitationTaskSummaryTypeDef


def get_value() -> ListEngagementByAcceptingInvitationTaskSummaryTypeDef:
    return {
        "EngagementInvitationId": ...,
    }


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
# ListTasksSortBaseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListTasksSortBaseTypeDef


def get_value() -> ListTasksSortBaseTypeDef:
    return {
        "SortBy": ...,
    }


# ListTasksSortBaseTypeDef definition

class ListTasksSortBaseTypeDef(TypedDict):
    SortBy: ListTasksSortNameType,  # (1)
    SortOrder: SortOrderType,  # (2)
```

1. See [:material-code-brackets: ListTasksSortNameType](./literals.md#listtaskssortnametype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import PaginatorConfigTypeDef


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

## ListEngagementFromOpportunityTaskSummaryTypeDef

```python
# ListEngagementFromOpportunityTaskSummaryTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListEngagementFromOpportunityTaskSummaryTypeDef


def get_value() -> ListEngagementFromOpportunityTaskSummaryTypeDef:
    return {
        "EngagementId": ...,
    }


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
# OpportunityEngagementInvitationSortTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import OpportunityEngagementInvitationSortTypeDef


def get_value() -> OpportunityEngagementInvitationSortTypeDef:
    return {
        "SortBy": ...,
    }


# OpportunityEngagementInvitationSortTypeDef definition

class OpportunityEngagementInvitationSortTypeDef(TypedDict):
    SortBy: OpportunityEngagementInvitationSortNameType,  # (1)
    SortOrder: SortOrderType,  # (2)
```

1. See [:material-code-brackets: OpportunityEngagementInvitationSortNameType](./literals.md#opportunityengagementinvitationsortnametype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListEngagementMembersRequestTypeDef

```python
# ListEngagementMembersRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListEngagementMembersRequestTypeDef


def get_value() -> ListEngagementMembersRequestTypeDef:
    return {
        "Catalog": ...,
    }


# ListEngagementMembersRequestTypeDef definition

class ListEngagementMembersRequestTypeDef(TypedDict):
    Catalog: str,
    Identifier: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListEngagementResourceAssociationsRequestTypeDef

```python
# ListEngagementResourceAssociationsRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListEngagementResourceAssociationsRequestTypeDef


def get_value() -> ListEngagementResourceAssociationsRequestTypeDef:
    return {
        "Catalog": ...,
    }


# ListEngagementResourceAssociationsRequestTypeDef definition

class ListEngagementResourceAssociationsRequestTypeDef(TypedDict):
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
# OpportunitySortTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import OpportunitySortTypeDef


def get_value() -> OpportunitySortTypeDef:
    return {
        "SortBy": ...,
    }


# OpportunitySortTypeDef definition

class OpportunitySortTypeDef(TypedDict):
    SortBy: OpportunitySortNameType,  # (1)
    SortOrder: SortOrderType,  # (2)
```

1. See [:material-code-brackets: OpportunitySortNameType](./literals.md#opportunitysortnametype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## SortObjectTypeDef

```python
# SortObjectTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import SortObjectTypeDef


def get_value() -> SortObjectTypeDef:
    return {
        "SortBy": ...,
    }


# SortObjectTypeDef definition

class SortObjectTypeDef(TypedDict):
    SortBy: NotRequired[SortByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: SortByType](./literals.md#sortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ResourceSnapshotJobSummaryTypeDef

```python
# ResourceSnapshotJobSummaryTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ResourceSnapshotJobSummaryTypeDef


def get_value() -> ResourceSnapshotJobSummaryTypeDef:
    return {
        "Arn": ...,
    }


# ResourceSnapshotJobSummaryTypeDef definition

class ResourceSnapshotJobSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    EngagementId: NotRequired[str],
    Id: NotRequired[str],
    Status: NotRequired[ResourceSnapshotJobStatusType],  # (1)
```

1. See [:material-code-brackets: ResourceSnapshotJobStatusType](./literals.md#resourcesnapshotjobstatustype) 
## ListResourceSnapshotsRequestTypeDef

```python
# ListResourceSnapshotsRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListResourceSnapshotsRequestTypeDef


def get_value() -> ListResourceSnapshotsRequestTypeDef:
    return {
        "Catalog": ...,
    }


# ListResourceSnapshotsRequestTypeDef definition

class ListResourceSnapshotsRequestTypeDef(TypedDict):
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
# ResourceSnapshotSummaryTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ResourceSnapshotSummaryTypeDef


def get_value() -> ResourceSnapshotSummaryTypeDef:
    return {
        "Arn": ...,
    }


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
# SolutionSortTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import SolutionSortTypeDef


def get_value() -> SolutionSortTypeDef:
    return {
        "SortBy": ...,
    }


# SolutionSortTypeDef definition

class SolutionSortTypeDef(TypedDict):
    SortBy: SolutionSortNameType,  # (1)
    SortOrder: SortOrderType,  # (2)
```

1. See [:material-code-brackets: SolutionSortNameType](./literals.md#solutionsortnametype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## SolutionBaseTypeDef

```python
# SolutionBaseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import SolutionBaseTypeDef


def get_value() -> SolutionBaseTypeDef:
    return {
        "Arn": ...,
    }


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
## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## MarketingTypeDef

```python
# MarketingTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import MarketingTypeDef


def get_value() -> MarketingTypeDef:
    return {
        "AwsFundingUsed": ...,
    }


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
## MonetaryValueTypeDef

```python
# MonetaryValueTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import MonetaryValueTypeDef


def get_value() -> MonetaryValueTypeDef:
    return {
        "Amount": ...,
    }


# MonetaryValueTypeDef definition

class MonetaryValueTypeDef(TypedDict):
    Amount: str,
    CurrencyCode: CurrencyCodeType,  # (1)
```

1. See [:material-code-brackets: CurrencyCodeType](./literals.md#currencycodetype) 
## SenderContactTypeDef

```python
# SenderContactTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import SenderContactTypeDef


def get_value() -> SenderContactTypeDef:
    return {
        "BusinessTitle": ...,
    }


# SenderContactTypeDef definition

class SenderContactTypeDef(TypedDict):
    Email: str,
    BusinessTitle: NotRequired[str],
    FirstName: NotRequired[str],
    LastName: NotRequired[str],
    Phone: NotRequired[str],
```

## PutSellingSystemSettingsRequestTypeDef

```python
# PutSellingSystemSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import PutSellingSystemSettingsRequestTypeDef


def get_value() -> PutSellingSystemSettingsRequestTypeDef:
    return {
        "Catalog": ...,
    }


# PutSellingSystemSettingsRequestTypeDef definition

class PutSellingSystemSettingsRequestTypeDef(TypedDict):
    Catalog: str,
    ResourceSnapshotJobRoleIdentifier: NotRequired[str],
```

## RejectEngagementInvitationRequestTypeDef

```python
# RejectEngagementInvitationRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import RejectEngagementInvitationRequestTypeDef


def get_value() -> RejectEngagementInvitationRequestTypeDef:
    return {
        "Catalog": ...,
    }


# RejectEngagementInvitationRequestTypeDef definition

class RejectEngagementInvitationRequestTypeDef(TypedDict):
    Catalog: str,
    Identifier: str,
    RejectionReason: NotRequired[str],
```

## StartResourceSnapshotJobRequestTypeDef

```python
# StartResourceSnapshotJobRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import StartResourceSnapshotJobRequestTypeDef


def get_value() -> StartResourceSnapshotJobRequestTypeDef:
    return {
        "Catalog": ...,
    }


# StartResourceSnapshotJobRequestTypeDef definition

class StartResourceSnapshotJobRequestTypeDef(TypedDict):
    Catalog: str,
    ResourceSnapshotJobIdentifier: str,
```

## StopResourceSnapshotJobRequestTypeDef

```python
# StopResourceSnapshotJobRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import StopResourceSnapshotJobRequestTypeDef


def get_value() -> StopResourceSnapshotJobRequestTypeDef:
    return {
        "Catalog": ...,
    }


# StopResourceSnapshotJobRequestTypeDef definition

class StopResourceSnapshotJobRequestTypeDef(TypedDict):
    Catalog: str,
    ResourceSnapshotJobIdentifier: str,
```

## SubmitOpportunityRequestTypeDef

```python
# SubmitOpportunityRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import SubmitOpportunityRequestTypeDef


def get_value() -> SubmitOpportunityRequestTypeDef:
    return {
        "Catalog": ...,
    }


# SubmitOpportunityRequestTypeDef definition

class SubmitOpportunityRequestTypeDef(TypedDict):
    Catalog: str,
    Identifier: str,
    InvolvementType: SalesInvolvementTypeType,  # (1)
    Visibility: NotRequired[VisibilityType],  # (2)
```

1. See [:material-code-brackets: SalesInvolvementTypeType](./literals.md#salesinvolvementtypetype) 
2. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## ReceiverTypeDef

```python
# ReceiverTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ReceiverTypeDef


def get_value() -> ReceiverTypeDef:
    return {
        "Account": ...,
    }


# ReceiverTypeDef definition

class ReceiverTypeDef(TypedDict):
    Account: NotRequired[AccountReceiverTypeDef],  # (1)
```

1. See [:material-code-braces: AccountReceiverTypeDef](./type_defs.md#accountreceivertypedef) 
## AccountSummaryTypeDef

```python
# AccountSummaryTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import AccountSummaryTypeDef


def get_value() -> AccountSummaryTypeDef:
    return {
        "Address": ...,
    }


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
# AccountTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import AccountTypeDef


def get_value() -> AccountTypeDef:
    return {
        "Address": ...,
    }


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
## AssignOpportunityRequestTypeDef

```python
# AssignOpportunityRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import AssignOpportunityRequestTypeDef


def get_value() -> AssignOpportunityRequestTypeDef:
    return {
        "Assignee": ...,
    }


# AssignOpportunityRequestTypeDef definition

class AssignOpportunityRequestTypeDef(TypedDict):
    Assignee: AssigneeContactTypeDef,  # (1)
    Catalog: str,
    Identifier: str,
```

1. See [:material-code-braces: AssigneeContactTypeDef](./type_defs.md#assigneecontacttypedef) 
## AwsOpportunityCustomerTypeDef

```python
# AwsOpportunityCustomerTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import AwsOpportunityCustomerTypeDef


def get_value() -> AwsOpportunityCustomerTypeDef:
    return {
        "Contacts": ...,
    }


# AwsOpportunityCustomerTypeDef definition

class AwsOpportunityCustomerTypeDef(TypedDict):
    Contacts: NotRequired[List[ContactTypeDef]],  # (1)
```

1. See [:material-code-braces: ContactTypeDef](./type_defs.md#contacttypedef) 
## AwsOpportunityLifeCycleTypeDef

```python
# AwsOpportunityLifeCycleTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import AwsOpportunityLifeCycleTypeDef


def get_value() -> AwsOpportunityLifeCycleTypeDef:
    return {
        "ClosedLostReason": ...,
    }


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
# AwsOpportunityProjectTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import AwsOpportunityProjectTypeDef


def get_value() -> AwsOpportunityProjectTypeDef:
    return {
        "ExpectedCustomerSpend": ...,
    }


# AwsOpportunityProjectTypeDef definition

class AwsOpportunityProjectTypeDef(TypedDict):
    ExpectedCustomerSpend: NotRequired[List[ExpectedCustomerSpendTypeDef]],  # (1)
```

1. See [:material-code-braces: ExpectedCustomerSpendTypeDef](./type_defs.md#expectedcustomerspendtypedef) 
## ProjectDetailsOutputTypeDef

```python
# ProjectDetailsOutputTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ProjectDetailsOutputTypeDef


def get_value() -> ProjectDetailsOutputTypeDef:
    return {
        "BusinessProblem": ...,
    }


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
# ProjectDetailsTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ProjectDetailsTypeDef


def get_value() -> ProjectDetailsTypeDef:
    return {
        "BusinessProblem": ...,
    }


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
# ProjectOutputTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ProjectOutputTypeDef


def get_value() -> ProjectOutputTypeDef:
    return {
        "AdditionalComments": ...,
    }


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
# ProjectSummaryTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ProjectSummaryTypeDef


def get_value() -> ProjectSummaryTypeDef:
    return {
        "DeliveryModels": ...,
    }


# ProjectSummaryTypeDef definition

class ProjectSummaryTypeDef(TypedDict):
    DeliveryModels: NotRequired[List[DeliveryModelType]],  # (1)
    ExpectedCustomerSpend: NotRequired[List[ExpectedCustomerSpendTypeDef]],  # (2)
```

1. See [:material-code-brackets: DeliveryModelType](./literals.md#deliverymodeltype) 
2. See [:material-code-braces: ExpectedCustomerSpendTypeDef](./type_defs.md#expectedcustomerspendtypedef) 
## ProjectTypeDef

```python
# ProjectTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ProjectTypeDef


def get_value() -> ProjectTypeDef:
    return {
        "AdditionalComments": ...,
    }


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
# ProjectViewTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ProjectViewTypeDef


def get_value() -> ProjectViewTypeDef:
    return {
        "CustomerUseCase": ...,
    }


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
# CreateEngagementInvitationResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import CreateEngagementInvitationResponseTypeDef


def get_value() -> CreateEngagementInvitationResponseTypeDef:
    return {
        "Arn": ...,
    }


# CreateEngagementInvitationResponseTypeDef definition

class CreateEngagementInvitationResponseTypeDef(TypedDict):
    Arn: str,
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEngagementResponseTypeDef

```python
# CreateEngagementResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import CreateEngagementResponseTypeDef


def get_value() -> CreateEngagementResponseTypeDef:
    return {
        "Arn": ...,
    }


# CreateEngagementResponseTypeDef definition

class CreateEngagementResponseTypeDef(TypedDict):
    Arn: str,
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateOpportunityResponseTypeDef

```python
# CreateOpportunityResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import CreateOpportunityResponseTypeDef


def get_value() -> CreateOpportunityResponseTypeDef:
    return {
        "Id": ...,
    }


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
# CreateResourceSnapshotJobResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import CreateResourceSnapshotJobResponseTypeDef


def get_value() -> CreateResourceSnapshotJobResponseTypeDef:
    return {
        "Arn": ...,
    }


# CreateResourceSnapshotJobResponseTypeDef definition

class CreateResourceSnapshotJobResponseTypeDef(TypedDict):
    Arn: str,
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateResourceSnapshotResponseTypeDef

```python
# CreateResourceSnapshotResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import CreateResourceSnapshotResponseTypeDef


def get_value() -> CreateResourceSnapshotResponseTypeDef:
    return {
        "Arn": ...,
    }


# CreateResourceSnapshotResponseTypeDef definition

class CreateResourceSnapshotResponseTypeDef(TypedDict):
    Arn: str,
    Revision: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourceSnapshotJobResponseTypeDef

```python
# GetResourceSnapshotJobResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import GetResourceSnapshotJobResponseTypeDef


def get_value() -> GetResourceSnapshotJobResponseTypeDef:
    return {
        "Arn": ...,
    }


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
# GetSellingSystemSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import GetSellingSystemSettingsResponseTypeDef


def get_value() -> GetSellingSystemSettingsResponseTypeDef:
    return {
        "Catalog": ...,
    }


# GetSellingSystemSettingsResponseTypeDef definition

class GetSellingSystemSettingsResponseTypeDef(TypedDict):
    Catalog: str,
    ResourceSnapshotJobRoleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutSellingSystemSettingsResponseTypeDef

```python
# PutSellingSystemSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import PutSellingSystemSettingsResponseTypeDef


def get_value() -> PutSellingSystemSettingsResponseTypeDef:
    return {
        "Catalog": ...,
    }


# PutSellingSystemSettingsResponseTypeDef definition

class PutSellingSystemSettingsResponseTypeDef(TypedDict):
    Catalog: str,
    ResourceSnapshotJobRoleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartEngagementByAcceptingInvitationTaskResponseTypeDef

```python
# StartEngagementByAcceptingInvitationTaskResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import StartEngagementByAcceptingInvitationTaskResponseTypeDef


def get_value() -> StartEngagementByAcceptingInvitationTaskResponseTypeDef:
    return {
        "EngagementInvitationId": ...,
    }


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
# StartEngagementFromOpportunityTaskResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import StartEngagementFromOpportunityTaskResponseTypeDef


def get_value() -> StartEngagementFromOpportunityTaskResponseTypeDef:
    return {
        "EngagementId": ...,
    }


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
# UpdateOpportunityResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import UpdateOpportunityResponseTypeDef


def get_value() -> UpdateOpportunityResponseTypeDef:
    return {
        "Id": ...,
    }


# UpdateOpportunityResponseTypeDef definition

class UpdateOpportunityResponseTypeDef(TypedDict):
    Id: str,
    LastModifiedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateResourceSnapshotJobRequestTypeDef

```python
# CreateResourceSnapshotJobRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import CreateResourceSnapshotJobRequestTypeDef


def get_value() -> CreateResourceSnapshotJobRequestTypeDef:
    return {
        "Catalog": ...,
    }


# CreateResourceSnapshotJobRequestTypeDef definition

class CreateResourceSnapshotJobRequestTypeDef(TypedDict):
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
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartEngagementByAcceptingInvitationTaskRequestTypeDef

```python
# StartEngagementByAcceptingInvitationTaskRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import StartEngagementByAcceptingInvitationTaskRequestTypeDef


def get_value() -> StartEngagementByAcceptingInvitationTaskRequestTypeDef:
    return {
        "Catalog": ...,
    }


# StartEngagementByAcceptingInvitationTaskRequestTypeDef definition

class StartEngagementByAcceptingInvitationTaskRequestTypeDef(TypedDict):
    Catalog: str,
    ClientToken: str,
    Identifier: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StartEngagementFromOpportunityTaskRequestTypeDef

```python
# StartEngagementFromOpportunityTaskRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import StartEngagementFromOpportunityTaskRequestTypeDef


def get_value() -> StartEngagementFromOpportunityTaskRequestTypeDef:
    return {
        "AwsSubmission": ...,
    }


# StartEngagementFromOpportunityTaskRequestTypeDef definition

class StartEngagementFromOpportunityTaskRequestTypeDef(TypedDict):
    AwsSubmission: AwsSubmissionTypeDef,  # (1)
    Catalog: str,
    ClientToken: str,
    Identifier: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: AwsSubmissionTypeDef](./type_defs.md#awssubmissiontypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CustomerProjectsContextTypeDef

```python
# CustomerProjectsContextTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import CustomerProjectsContextTypeDef


def get_value() -> CustomerProjectsContextTypeDef:
    return {
        "Customer": ...,
    }


# CustomerProjectsContextTypeDef definition

class CustomerProjectsContextTypeDef(TypedDict):
    Customer: NotRequired[EngagementCustomerTypeDef],  # (1)
    Project: NotRequired[EngagementCustomerProjectDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: EngagementCustomerTypeDef](./type_defs.md#engagementcustomertypedef) 
2. See [:material-code-braces: EngagementCustomerProjectDetailsTypeDef](./type_defs.md#engagementcustomerprojectdetailstypedef) 
## ListEngagementMembersResponseTypeDef

```python
# ListEngagementMembersResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListEngagementMembersResponseTypeDef


def get_value() -> ListEngagementMembersResponseTypeDef:
    return {
        "EngagementMemberList": ...,
    }


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
# ListEngagementResourceAssociationsResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListEngagementResourceAssociationsResponseTypeDef


def get_value() -> ListEngagementResourceAssociationsResponseTypeDef:
    return {
        "EngagementResourceAssociationSummaries": ...,
    }


# ListEngagementResourceAssociationsResponseTypeDef definition

class ListEngagementResourceAssociationsResponseTypeDef(TypedDict):
    EngagementResourceAssociationSummaries: List[EngagementResourceAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EngagementResourceAssociationSummaryTypeDef](./type_defs.md#engagementresourceassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEngagementsRequestTypeDef

```python
# ListEngagementsRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListEngagementsRequestTypeDef


def get_value() -> ListEngagementsRequestTypeDef:
    return {
        "Catalog": ...,
    }


# ListEngagementsRequestTypeDef definition

class ListEngagementsRequestTypeDef(TypedDict):
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
# ListEngagementsResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListEngagementsResponseTypeDef


def get_value() -> ListEngagementsResponseTypeDef:
    return {
        "EngagementSummaryList": ...,
    }


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
# LastModifiedDateTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import LastModifiedDateTypeDef


def get_value() -> LastModifiedDateTypeDef:
    return {
        "AfterLastModifiedDate": ...,
    }


# LastModifiedDateTypeDef definition

class LastModifiedDateTypeDef(TypedDict):
    AfterLastModifiedDate: NotRequired[TimestampTypeDef],
    BeforeLastModifiedDate: NotRequired[TimestampTypeDef],
```

## NextStepsHistoryTypeDef

```python
# NextStepsHistoryTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import NextStepsHistoryTypeDef


def get_value() -> NextStepsHistoryTypeDef:
    return {
        "Time": ...,
    }


# NextStepsHistoryTypeDef definition

class NextStepsHistoryTypeDef(TypedDict):
    Time: TimestampTypeDef,
    Value: str,
```

## LifeCycleOutputTypeDef

```python
# LifeCycleOutputTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import LifeCycleOutputTypeDef


def get_value() -> LifeCycleOutputTypeDef:
    return {
        "ClosedLostReason": ...,
    }


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
# ListEngagementByAcceptingInvitationTasksResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListEngagementByAcceptingInvitationTasksResponseTypeDef


def get_value() -> ListEngagementByAcceptingInvitationTasksResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListEngagementByAcceptingInvitationTasksResponseTypeDef definition

class ListEngagementByAcceptingInvitationTasksResponseTypeDef(TypedDict):
    TaskSummaries: List[ListEngagementByAcceptingInvitationTaskSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListEngagementByAcceptingInvitationTaskSummaryTypeDef](./type_defs.md#listengagementbyacceptinginvitationtasksummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEngagementByAcceptingInvitationTasksRequestTypeDef

```python
# ListEngagementByAcceptingInvitationTasksRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListEngagementByAcceptingInvitationTasksRequestTypeDef


def get_value() -> ListEngagementByAcceptingInvitationTasksRequestTypeDef:
    return {
        "Catalog": ...,
    }


# ListEngagementByAcceptingInvitationTasksRequestTypeDef definition

class ListEngagementByAcceptingInvitationTasksRequestTypeDef(TypedDict):
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
## ListEngagementFromOpportunityTasksRequestTypeDef

```python
# ListEngagementFromOpportunityTasksRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListEngagementFromOpportunityTasksRequestTypeDef


def get_value() -> ListEngagementFromOpportunityTasksRequestTypeDef:
    return {
        "Catalog": ...,
    }


# ListEngagementFromOpportunityTasksRequestTypeDef definition

class ListEngagementFromOpportunityTasksRequestTypeDef(TypedDict):
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
# ListEngagementByAcceptingInvitationTasksRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListEngagementByAcceptingInvitationTasksRequestPaginateTypeDef


def get_value() -> ListEngagementByAcceptingInvitationTasksRequestPaginateTypeDef:
    return {
        "Catalog": ...,
    }


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
# ListEngagementFromOpportunityTasksRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListEngagementFromOpportunityTasksRequestPaginateTypeDef


def get_value() -> ListEngagementFromOpportunityTasksRequestPaginateTypeDef:
    return {
        "Catalog": ...,
    }


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
# ListEngagementMembersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListEngagementMembersRequestPaginateTypeDef


def get_value() -> ListEngagementMembersRequestPaginateTypeDef:
    return {
        "Catalog": ...,
    }


# ListEngagementMembersRequestPaginateTypeDef definition

class ListEngagementMembersRequestPaginateTypeDef(TypedDict):
    Catalog: str,
    Identifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEngagementResourceAssociationsRequestPaginateTypeDef

```python
# ListEngagementResourceAssociationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListEngagementResourceAssociationsRequestPaginateTypeDef


def get_value() -> ListEngagementResourceAssociationsRequestPaginateTypeDef:
    return {
        "Catalog": ...,
    }


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
# ListEngagementsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListEngagementsRequestPaginateTypeDef


def get_value() -> ListEngagementsRequestPaginateTypeDef:
    return {
        "Catalog": ...,
    }


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
# ListResourceSnapshotsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListResourceSnapshotsRequestPaginateTypeDef


def get_value() -> ListResourceSnapshotsRequestPaginateTypeDef:
    return {
        "Catalog": ...,
    }


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
# ListEngagementFromOpportunityTasksResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListEngagementFromOpportunityTasksResponseTypeDef


def get_value() -> ListEngagementFromOpportunityTasksResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# ListEngagementInvitationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListEngagementInvitationsRequestPaginateTypeDef


def get_value() -> ListEngagementInvitationsRequestPaginateTypeDef:
    return {
        "Catalog": ...,
    }


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
## ListEngagementInvitationsRequestTypeDef

```python
# ListEngagementInvitationsRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListEngagementInvitationsRequestTypeDef


def get_value() -> ListEngagementInvitationsRequestTypeDef:
    return {
        "Catalog": ...,
    }


# ListEngagementInvitationsRequestTypeDef definition

class ListEngagementInvitationsRequestTypeDef(TypedDict):
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
# ListResourceSnapshotJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListResourceSnapshotJobsRequestPaginateTypeDef


def get_value() -> ListResourceSnapshotJobsRequestPaginateTypeDef:
    return {
        "Catalog": ...,
    }


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
## ListResourceSnapshotJobsRequestTypeDef

```python
# ListResourceSnapshotJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListResourceSnapshotJobsRequestTypeDef


def get_value() -> ListResourceSnapshotJobsRequestTypeDef:
    return {
        "Catalog": ...,
    }


# ListResourceSnapshotJobsRequestTypeDef definition

class ListResourceSnapshotJobsRequestTypeDef(TypedDict):
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
# ListResourceSnapshotJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListResourceSnapshotJobsResponseTypeDef


def get_value() -> ListResourceSnapshotJobsResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# ListResourceSnapshotsResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListResourceSnapshotsResponseTypeDef


def get_value() -> ListResourceSnapshotsResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# ListSolutionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListSolutionsRequestPaginateTypeDef


def get_value() -> ListSolutionsRequestPaginateTypeDef:
    return {
        "Catalog": ...,
    }


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
## ListSolutionsRequestTypeDef

```python
# ListSolutionsRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListSolutionsRequestTypeDef


def get_value() -> ListSolutionsRequestTypeDef:
    return {
        "Catalog": ...,
    }


# ListSolutionsRequestTypeDef definition

class ListSolutionsRequestTypeDef(TypedDict):
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
# ListSolutionsResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListSolutionsResponseTypeDef


def get_value() -> ListSolutionsResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# SoftwareRevenueTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import SoftwareRevenueTypeDef


def get_value() -> SoftwareRevenueTypeDef:
    return {
        "DeliveryModel": ...,
    }


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
# EngagementInvitationSummaryTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import EngagementInvitationSummaryTypeDef


def get_value() -> EngagementInvitationSummaryTypeDef:
    return {
        "Arn": ...,
    }


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
# CustomerSummaryTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import CustomerSummaryTypeDef


def get_value() -> CustomerSummaryTypeDef:
    return {
        "Account": ...,
    }


# CustomerSummaryTypeDef definition

class CustomerSummaryTypeDef(TypedDict):
    Account: NotRequired[AccountSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: AccountSummaryTypeDef](./type_defs.md#accountsummarytypedef) 
## CustomerOutputTypeDef

```python
# CustomerOutputTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import CustomerOutputTypeDef


def get_value() -> CustomerOutputTypeDef:
    return {
        "Account": ...,
    }


# CustomerOutputTypeDef definition

class CustomerOutputTypeDef(TypedDict):
    Account: NotRequired[AccountTypeDef],  # (1)
    Contacts: NotRequired[List[ContactTypeDef]],  # (2)
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 
2. See [:material-code-braces: ContactTypeDef](./type_defs.md#contacttypedef) 
## CustomerTypeDef

```python
# CustomerTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import CustomerTypeDef


def get_value() -> CustomerTypeDef:
    return {
        "Account": ...,
    }


# CustomerTypeDef definition

class CustomerTypeDef(TypedDict):
    Account: NotRequired[AccountTypeDef],  # (1)
    Contacts: NotRequired[Sequence[ContactTypeDef]],  # (2)
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 
2. See [:material-code-braces: ContactTypeDef](./type_defs.md#contacttypedef) 
## GetAwsOpportunitySummaryResponseTypeDef

```python
# GetAwsOpportunitySummaryResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import GetAwsOpportunitySummaryResponseTypeDef


def get_value() -> GetAwsOpportunitySummaryResponseTypeDef:
    return {
        "Catalog": ...,
    }


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
# OpportunityInvitationPayloadOutputTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import OpportunityInvitationPayloadOutputTypeDef


def get_value() -> OpportunityInvitationPayloadOutputTypeDef:
    return {
        "Customer": ...,
    }


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
# EngagementContextPayloadTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import EngagementContextPayloadTypeDef


def get_value() -> EngagementContextPayloadTypeDef:
    return {
        "CustomerProject": ...,
    }


# EngagementContextPayloadTypeDef definition

class EngagementContextPayloadTypeDef(TypedDict):
    CustomerProject: NotRequired[CustomerProjectsContextTypeDef],  # (1)
```

1. See [:material-code-braces: CustomerProjectsContextTypeDef](./type_defs.md#customerprojectscontexttypedef) 
## ListOpportunitiesRequestPaginateTypeDef

```python
# ListOpportunitiesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListOpportunitiesRequestPaginateTypeDef


def get_value() -> ListOpportunitiesRequestPaginateTypeDef:
    return {
        "Catalog": ...,
    }


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
## ListOpportunitiesRequestTypeDef

```python
# ListOpportunitiesRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListOpportunitiesRequestTypeDef


def get_value() -> ListOpportunitiesRequestTypeDef:
    return {
        "Catalog": ...,
    }


# ListOpportunitiesRequestTypeDef definition

class ListOpportunitiesRequestTypeDef(TypedDict):
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
## LifeCycleTypeDef

```python
# LifeCycleTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import LifeCycleTypeDef


def get_value() -> LifeCycleTypeDef:
    return {
        "ClosedLostReason": ...,
    }


# LifeCycleTypeDef definition

class LifeCycleTypeDef(TypedDict):
    ClosedLostReason: NotRequired[ClosedLostReasonType],  # (1)
    NextSteps: NotRequired[str],
    NextStepsHistory: NotRequired[Sequence[NextStepsHistoryTypeDef]],  # (2)
    ReviewComments: NotRequired[str],
    ReviewStatus: NotRequired[ReviewStatusType],  # (3)
    ReviewStatusReason: NotRequired[str],
    Stage: NotRequired[StageType],  # (4)
    TargetCloseDate: NotRequired[str],
```

1. See [:material-code-brackets: ClosedLostReasonType](./literals.md#closedlostreasontype) 
2. See [:material-code-braces: NextStepsHistoryTypeDef](./type_defs.md#nextstepshistorytypedef) 
3. See [:material-code-brackets: ReviewStatusType](./literals.md#reviewstatustype) 
4. See [:material-code-brackets: StageType](./literals.md#stagetype) 
## ListEngagementInvitationsResponseTypeDef

```python
# ListEngagementInvitationsResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListEngagementInvitationsResponseTypeDef


def get_value() -> ListEngagementInvitationsResponseTypeDef:
    return {
        "EngagementInvitationSummaries": ...,
    }


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
# OpportunitySummaryTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import OpportunitySummaryTypeDef


def get_value() -> OpportunitySummaryTypeDef:
    return {
        "Arn": ...,
    }


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
# GetOpportunityResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import GetOpportunityResponseTypeDef


def get_value() -> GetOpportunityResponseTypeDef:
    return {
        "Arn": ...,
    }


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
# OpportunitySummaryViewTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import OpportunitySummaryViewTypeDef


def get_value() -> OpportunitySummaryViewTypeDef:
    return {
        "Customer": ...,
    }


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
# PayloadOutputTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import PayloadOutputTypeDef


def get_value() -> PayloadOutputTypeDef:
    return {
        "OpportunityInvitation": ...,
    }


# PayloadOutputTypeDef definition

class PayloadOutputTypeDef(TypedDict):
    OpportunityInvitation: NotRequired[OpportunityInvitationPayloadOutputTypeDef],  # (1)
```

1. See [:material-code-braces: OpportunityInvitationPayloadOutputTypeDef](./type_defs.md#opportunityinvitationpayloadoutputtypedef) 
## OpportunityInvitationPayloadTypeDef

```python
# OpportunityInvitationPayloadTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import OpportunityInvitationPayloadTypeDef


def get_value() -> OpportunityInvitationPayloadTypeDef:
    return {
        "Customer": ...,
    }


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
# EngagementContextDetailsTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import EngagementContextDetailsTypeDef


def get_value() -> EngagementContextDetailsTypeDef:
    return {
        "Payload": ...,
    }


# EngagementContextDetailsTypeDef definition

class EngagementContextDetailsTypeDef(TypedDict):
    Type: EngagementContextTypeType,  # (2)
    Payload: NotRequired[EngagementContextPayloadTypeDef],  # (1)
```

1. See [:material-code-braces: EngagementContextPayloadTypeDef](./type_defs.md#engagementcontextpayloadtypedef) 
2. See [:material-code-brackets: EngagementContextTypeType](./literals.md#engagementcontexttypetype) 
## ListOpportunitiesResponseTypeDef

```python
# ListOpportunitiesResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ListOpportunitiesResponseTypeDef


def get_value() -> ListOpportunitiesResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# ResourceSnapshotPayloadTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import ResourceSnapshotPayloadTypeDef


def get_value() -> ResourceSnapshotPayloadTypeDef:
    return {
        "OpportunitySummary": ...,
    }


# ResourceSnapshotPayloadTypeDef definition

class ResourceSnapshotPayloadTypeDef(TypedDict):
    OpportunitySummary: NotRequired[OpportunitySummaryViewTypeDef],  # (1)
```

1. See [:material-code-braces: OpportunitySummaryViewTypeDef](./type_defs.md#opportunitysummaryviewtypedef) 
## GetEngagementInvitationResponseTypeDef

```python
# GetEngagementInvitationResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import GetEngagementInvitationResponseTypeDef


def get_value() -> GetEngagementInvitationResponseTypeDef:
    return {
        "Arn": ...,
    }


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
## CreateEngagementRequestTypeDef

```python
# CreateEngagementRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import CreateEngagementRequestTypeDef


def get_value() -> CreateEngagementRequestTypeDef:
    return {
        "Catalog": ...,
    }


# CreateEngagementRequestTypeDef definition

class CreateEngagementRequestTypeDef(TypedDict):
    Catalog: str,
    ClientToken: str,
    Description: str,
    Title: str,
    Contexts: NotRequired[Sequence[EngagementContextDetailsTypeDef]],  # (1)
```

1. See [:material-code-braces: EngagementContextDetailsTypeDef](./type_defs.md#engagementcontextdetailstypedef) 
## GetEngagementResponseTypeDef

```python
# GetEngagementResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import GetEngagementResponseTypeDef


def get_value() -> GetEngagementResponseTypeDef:
    return {
        "Arn": ...,
    }


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
## CreateOpportunityRequestTypeDef

```python
# CreateOpportunityRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import CreateOpportunityRequestTypeDef


def get_value() -> CreateOpportunityRequestTypeDef:
    return {
        "Catalog": ...,
    }


# CreateOpportunityRequestTypeDef definition

class CreateOpportunityRequestTypeDef(TypedDict):
    Catalog: str,
    ClientToken: str,
    Customer: NotRequired[CustomerUnionTypeDef],  # (1)
    LifeCycle: NotRequired[LifeCycleUnionTypeDef],  # (2)
    Marketing: NotRequired[MarketingUnionTypeDef],  # (3)
    NationalSecurity: NotRequired[NationalSecurityType],  # (4)
    OpportunityTeam: NotRequired[Sequence[ContactTypeDef]],  # (5)
    OpportunityType: NotRequired[OpportunityTypeType],  # (6)
    Origin: NotRequired[OpportunityOriginType],  # (7)
    PartnerOpportunityIdentifier: NotRequired[str],
    PrimaryNeedsFromAws: NotRequired[Sequence[PrimaryNeedFromAwsType]],  # (8)
    Project: NotRequired[ProjectUnionTypeDef],  # (9)
    SoftwareRevenue: NotRequired[SoftwareRevenueTypeDef],  # (10)
```

1. See [:material-code-braces: CustomerTypeDef](./type_defs.md#customertypedef) [:material-code-braces: CustomerOutputTypeDef](./type_defs.md#customeroutputtypedef) 
2. See [:material-code-braces: LifeCycleTypeDef](./type_defs.md#lifecycletypedef) [:material-code-braces: LifeCycleOutputTypeDef](./type_defs.md#lifecycleoutputtypedef) 
3. See [:material-code-braces: MarketingTypeDef](./type_defs.md#marketingtypedef) [:material-code-braces: MarketingOutputTypeDef](./type_defs.md#marketingoutputtypedef) 
4. See [:material-code-brackets: NationalSecurityType](./literals.md#nationalsecuritytype) 
5. See [:material-code-braces: ContactTypeDef](./type_defs.md#contacttypedef) 
6. See [:material-code-brackets: OpportunityTypeType](./literals.md#opportunitytypetype) 
7. See [:material-code-brackets: OpportunityOriginType](./literals.md#opportunityorigintype) 
8. See [:material-code-brackets: PrimaryNeedFromAwsType](./literals.md#primaryneedfromawstype) 
9. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) [:material-code-braces: ProjectOutputTypeDef](./type_defs.md#projectoutputtypedef) 
10. See [:material-code-braces: SoftwareRevenueTypeDef](./type_defs.md#softwarerevenuetypedef) 
## UpdateOpportunityRequestTypeDef

```python
# UpdateOpportunityRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import UpdateOpportunityRequestTypeDef


def get_value() -> UpdateOpportunityRequestTypeDef:
    return {
        "Catalog": ...,
    }


# UpdateOpportunityRequestTypeDef definition

class UpdateOpportunityRequestTypeDef(TypedDict):
    Catalog: str,
    Identifier: str,
    LastModifiedDate: TimestampTypeDef,
    Customer: NotRequired[CustomerUnionTypeDef],  # (1)
    LifeCycle: NotRequired[LifeCycleUnionTypeDef],  # (2)
    Marketing: NotRequired[MarketingUnionTypeDef],  # (3)
    NationalSecurity: NotRequired[NationalSecurityType],  # (4)
    OpportunityType: NotRequired[OpportunityTypeType],  # (5)
    PartnerOpportunityIdentifier: NotRequired[str],
    PrimaryNeedsFromAws: NotRequired[Sequence[PrimaryNeedFromAwsType]],  # (6)
    Project: NotRequired[ProjectUnionTypeDef],  # (7)
    SoftwareRevenue: NotRequired[SoftwareRevenueTypeDef],  # (8)
```

1. See [:material-code-braces: CustomerTypeDef](./type_defs.md#customertypedef) [:material-code-braces: CustomerOutputTypeDef](./type_defs.md#customeroutputtypedef) 
2. See [:material-code-braces: LifeCycleTypeDef](./type_defs.md#lifecycletypedef) [:material-code-braces: LifeCycleOutputTypeDef](./type_defs.md#lifecycleoutputtypedef) 
3. See [:material-code-braces: MarketingTypeDef](./type_defs.md#marketingtypedef) [:material-code-braces: MarketingOutputTypeDef](./type_defs.md#marketingoutputtypedef) 
4. See [:material-code-brackets: NationalSecurityType](./literals.md#nationalsecuritytype) 
5. See [:material-code-brackets: OpportunityTypeType](./literals.md#opportunitytypetype) 
6. See [:material-code-brackets: PrimaryNeedFromAwsType](./literals.md#primaryneedfromawstype) 
7. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) [:material-code-braces: ProjectOutputTypeDef](./type_defs.md#projectoutputtypedef) 
8. See [:material-code-braces: SoftwareRevenueTypeDef](./type_defs.md#softwarerevenuetypedef) 
## GetResourceSnapshotResponseTypeDef

```python
# GetResourceSnapshotResponseTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import GetResourceSnapshotResponseTypeDef


def get_value() -> GetResourceSnapshotResponseTypeDef:
    return {
        "Arn": ...,
    }


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
# PayloadTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import PayloadTypeDef


def get_value() -> PayloadTypeDef:
    return {
        "OpportunityInvitation": ...,
    }


# PayloadTypeDef definition

class PayloadTypeDef(TypedDict):
    OpportunityInvitation: NotRequired[OpportunityInvitationPayloadUnionTypeDef],  # (1)
```

1. See [:material-code-braces: OpportunityInvitationPayloadTypeDef](./type_defs.md#opportunityinvitationpayloadtypedef) [:material-code-braces: OpportunityInvitationPayloadOutputTypeDef](./type_defs.md#opportunityinvitationpayloadoutputtypedef) 
## InvitationTypeDef

```python
# InvitationTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import InvitationTypeDef


def get_value() -> InvitationTypeDef:
    return {
        "Message": ...,
    }


# InvitationTypeDef definition

class InvitationTypeDef(TypedDict):
    Message: str,
    Payload: PayloadUnionTypeDef,  # (1)
    Receiver: ReceiverTypeDef,  # (2)
```

1. See [:material-code-braces: PayloadTypeDef](./type_defs.md#payloadtypedef) [:material-code-braces: PayloadOutputTypeDef](./type_defs.md#payloadoutputtypedef) 
2. See [:material-code-braces: ReceiverTypeDef](./type_defs.md#receivertypedef) 
## CreateEngagementInvitationRequestTypeDef

```python
# CreateEngagementInvitationRequestTypeDef TypedDict usage example

from types_aiobotocore_partnercentral_selling.type_defs import CreateEngagementInvitationRequestTypeDef


def get_value() -> CreateEngagementInvitationRequestTypeDef:
    return {
        "Catalog": ...,
    }


# CreateEngagementInvitationRequestTypeDef definition

class CreateEngagementInvitationRequestTypeDef(TypedDict):
    Catalog: str,
    ClientToken: str,
    EngagementIdentifier: str,
    Invitation: InvitationTypeDef,  # (1)
```

1. See [:material-code-braces: InvitationTypeDef](./type_defs.md#invitationtypedef) 
