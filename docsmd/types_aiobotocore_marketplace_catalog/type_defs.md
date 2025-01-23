# Type definitions

> [Index](../README.md) > [MarketplaceCatalog](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MarketplaceCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#marketplacecatalog)
    type annotations stubs module [types-aiobotocore-marketplace-catalog](https://pypi.org/project/types-aiobotocore-marketplace-catalog/).



## AmiProductEntityIdFilterTypeDef

```python
# AmiProductEntityIdFilterTypeDef definition

class AmiProductEntityIdFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[str]],
```

## AmiProductTitleFilterTypeDef

```python
# AmiProductTitleFilterTypeDef definition

class AmiProductTitleFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[str]],
    WildCardValue: NotRequired[str],
```

## AmiProductVisibilityFilterTypeDef

```python
# AmiProductVisibilityFilterTypeDef definition

class AmiProductVisibilityFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[AmiProductVisibilityStringType]],  # (1)
```

1. See [:material-code-brackets: AmiProductVisibilityStringType](./literals.md#amiproductvisibilitystringtype) 
## AmiProductLastModifiedDateFilterDateRangeTypeDef

```python
# AmiProductLastModifiedDateFilterDateRangeTypeDef definition

class AmiProductLastModifiedDateFilterDateRangeTypeDef(TypedDict):
    AfterValue: NotRequired[str],
    BeforeValue: NotRequired[str],
```

## AmiProductSortTypeDef

```python
# AmiProductSortTypeDef definition

class AmiProductSortTypeDef(TypedDict):
    SortBy: NotRequired[AmiProductSortByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: AmiProductSortByType](./literals.md#amiproductsortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## AmiProductSummaryTypeDef

```python
# AmiProductSummaryTypeDef definition

class AmiProductSummaryTypeDef(TypedDict):
    ProductTitle: NotRequired[str],
    Visibility: NotRequired[AmiProductVisibilityStringType],  # (1)
```

1. See [:material-code-brackets: AmiProductVisibilityStringType](./literals.md#amiproductvisibilitystringtype) 
## EntityRequestTypeDef

```python
# EntityRequestTypeDef definition

class EntityRequestTypeDef(TypedDict):
    Catalog: str,
    EntityId: str,
```

## BatchDescribeErrorDetailTypeDef

```python
# BatchDescribeErrorDetailTypeDef definition

class BatchDescribeErrorDetailTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## EntityDetailTypeDef

```python
# EntityDetailTypeDef definition

class EntityDetailTypeDef(TypedDict):
    EntityType: NotRequired[str],
    EntityArn: NotRequired[str],
    EntityIdentifier: NotRequired[str],
    LastModifiedDate: NotRequired[str],
    DetailsDocument: NotRequired[Dict[str, Any]],
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

## CancelChangeSetRequestRequestTypeDef

```python
# CancelChangeSetRequestRequestTypeDef definition

class CancelChangeSetRequestRequestTypeDef(TypedDict):
    Catalog: str,
    ChangeSetId: str,
```

## ChangeSetSummaryListItemTypeDef

```python
# ChangeSetSummaryListItemTypeDef definition

class ChangeSetSummaryListItemTypeDef(TypedDict):
    ChangeSetId: NotRequired[str],
    ChangeSetArn: NotRequired[str],
    ChangeSetName: NotRequired[str],
    StartTime: NotRequired[str],
    EndTime: NotRequired[str],
    Status: NotRequired[ChangeStatusType],  # (1)
    EntityIdList: NotRequired[List[str]],
    FailureCode: NotRequired[FailureCodeType],  # (2)
```

1. See [:material-code-brackets: ChangeStatusType](./literals.md#changestatustype) 
2. See [:material-code-brackets: FailureCodeType](./literals.md#failurecodetype) 
## EntityTypeDef

```python
# EntityTypeDef definition

class EntityTypeDef(TypedDict):
    Type: str,
    Identifier: NotRequired[str],
```

## ErrorDetailTypeDef

```python
# ErrorDetailTypeDef definition

class ErrorDetailTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## ContainerProductEntityIdFilterTypeDef

```python
# ContainerProductEntityIdFilterTypeDef definition

class ContainerProductEntityIdFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[str]],
```

## ContainerProductTitleFilterTypeDef

```python
# ContainerProductTitleFilterTypeDef definition

class ContainerProductTitleFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[str]],
    WildCardValue: NotRequired[str],
```

## ContainerProductVisibilityFilterTypeDef

```python
# ContainerProductVisibilityFilterTypeDef definition

class ContainerProductVisibilityFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[ContainerProductVisibilityStringType]],  # (1)
```

1. See [:material-code-brackets: ContainerProductVisibilityStringType](./literals.md#containerproductvisibilitystringtype) 
## ContainerProductLastModifiedDateFilterDateRangeTypeDef

```python
# ContainerProductLastModifiedDateFilterDateRangeTypeDef definition

class ContainerProductLastModifiedDateFilterDateRangeTypeDef(TypedDict):
    AfterValue: NotRequired[str],
    BeforeValue: NotRequired[str],
```

## ContainerProductSortTypeDef

```python
# ContainerProductSortTypeDef definition

class ContainerProductSortTypeDef(TypedDict):
    SortBy: NotRequired[ContainerProductSortByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: ContainerProductSortByType](./literals.md#containerproductsortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ContainerProductSummaryTypeDef

```python
# ContainerProductSummaryTypeDef definition

class ContainerProductSummaryTypeDef(TypedDict):
    ProductTitle: NotRequired[str],
    Visibility: NotRequired[ContainerProductVisibilityStringType],  # (1)
```

1. See [:material-code-brackets: ContainerProductVisibilityStringType](./literals.md#containerproductvisibilitystringtype) 
## DataProductEntityIdFilterTypeDef

```python
# DataProductEntityIdFilterTypeDef definition

class DataProductEntityIdFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[str]],
```

## DataProductTitleFilterTypeDef

```python
# DataProductTitleFilterTypeDef definition

class DataProductTitleFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[str]],
    WildCardValue: NotRequired[str],
```

## DataProductVisibilityFilterTypeDef

```python
# DataProductVisibilityFilterTypeDef definition

class DataProductVisibilityFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[DataProductVisibilityStringType]],  # (1)
```

1. See [:material-code-brackets: DataProductVisibilityStringType](./literals.md#dataproductvisibilitystringtype) 
## DataProductLastModifiedDateFilterDateRangeTypeDef

```python
# DataProductLastModifiedDateFilterDateRangeTypeDef definition

class DataProductLastModifiedDateFilterDateRangeTypeDef(TypedDict):
    AfterValue: NotRequired[str],
    BeforeValue: NotRequired[str],
```

## DataProductSortTypeDef

```python
# DataProductSortTypeDef definition

class DataProductSortTypeDef(TypedDict):
    SortBy: NotRequired[DataProductSortByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: DataProductSortByType](./literals.md#dataproductsortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## DataProductSummaryTypeDef

```python
# DataProductSummaryTypeDef definition

class DataProductSummaryTypeDef(TypedDict):
    ProductTitle: NotRequired[str],
    Visibility: NotRequired[DataProductVisibilityStringType],  # (1)
```

1. See [:material-code-brackets: DataProductVisibilityStringType](./literals.md#dataproductvisibilitystringtype) 
## DeleteResourcePolicyRequestRequestTypeDef

```python
# DeleteResourcePolicyRequestRequestTypeDef definition

class DeleteResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## DescribeChangeSetRequestRequestTypeDef

```python
# DescribeChangeSetRequestRequestTypeDef definition

class DescribeChangeSetRequestRequestTypeDef(TypedDict):
    Catalog: str,
    ChangeSetId: str,
```

## DescribeEntityRequestRequestTypeDef

```python
# DescribeEntityRequestRequestTypeDef definition

class DescribeEntityRequestRequestTypeDef(TypedDict):
    Catalog: str,
    EntityId: str,
```

## OfferSummaryTypeDef

```python
# OfferSummaryTypeDef definition

class OfferSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    ProductId: NotRequired[str],
    ResaleAuthorizationId: NotRequired[str],
    ReleaseDate: NotRequired[str],
    AvailabilityEndDate: NotRequired[str],
    BuyerAccounts: NotRequired[List[str]],
    State: NotRequired[OfferStateStringType],  # (1)
    Targeting: NotRequired[List[OfferTargetingStringType]],  # (2)
```

1. See [:material-code-brackets: OfferStateStringType](./literals.md#offerstatestringtype) 
2. See [:material-code-brackets: OfferTargetingStringType](./literals.md#offertargetingstringtype) 
## ResaleAuthorizationSummaryTypeDef

```python
# ResaleAuthorizationSummaryTypeDef definition

class ResaleAuthorizationSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    ProductId: NotRequired[str],
    ProductName: NotRequired[str],
    ManufacturerAccountId: NotRequired[str],
    ManufacturerLegalName: NotRequired[str],
    ResellerAccountID: NotRequired[str],
    ResellerLegalName: NotRequired[str],
    Status: NotRequired[ResaleAuthorizationStatusStringType],  # (1)
    OfferExtendedStatus: NotRequired[str],
    CreatedDate: NotRequired[str],
    AvailabilityEndDate: NotRequired[str],
```

1. See [:material-code-brackets: ResaleAuthorizationStatusStringType](./literals.md#resaleauthorizationstatusstringtype) 
## SaaSProductSummaryTypeDef

```python
# SaaSProductSummaryTypeDef definition

class SaaSProductSummaryTypeDef(TypedDict):
    ProductTitle: NotRequired[str],
    Visibility: NotRequired[SaaSProductVisibilityStringType],  # (1)
```

1. See [:material-code-brackets: SaaSProductVisibilityStringType](./literals.md#saasproductvisibilitystringtype) 
## OfferSortTypeDef

```python
# OfferSortTypeDef definition

class OfferSortTypeDef(TypedDict):
    SortBy: NotRequired[OfferSortByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: OfferSortByType](./literals.md#offersortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ResaleAuthorizationSortTypeDef

```python
# ResaleAuthorizationSortTypeDef definition

class ResaleAuthorizationSortTypeDef(TypedDict):
    SortBy: NotRequired[ResaleAuthorizationSortByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: ResaleAuthorizationSortByType](./literals.md#resaleauthorizationsortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## SaaSProductSortTypeDef

```python
# SaaSProductSortTypeDef definition

class SaaSProductSortTypeDef(TypedDict):
    SortBy: NotRequired[SaaSProductSortByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: SaaSProductSortByType](./literals.md#saasproductsortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Name: NotRequired[str],
    ValueList: NotRequired[Sequence[str]],
```

## GetResourcePolicyRequestRequestTypeDef

```python
# GetResourcePolicyRequestRequestTypeDef definition

class GetResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## SortTypeDef

```python
# SortTypeDef definition

class SortTypeDef(TypedDict):
    SortBy: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (1)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## OfferAvailabilityEndDateFilterDateRangeTypeDef

```python
# OfferAvailabilityEndDateFilterDateRangeTypeDef definition

class OfferAvailabilityEndDateFilterDateRangeTypeDef(TypedDict):
    AfterValue: NotRequired[str],
    BeforeValue: NotRequired[str],
```

## OfferBuyerAccountsFilterTypeDef

```python
# OfferBuyerAccountsFilterTypeDef definition

class OfferBuyerAccountsFilterTypeDef(TypedDict):
    WildCardValue: NotRequired[str],
```

## OfferEntityIdFilterTypeDef

```python
# OfferEntityIdFilterTypeDef definition

class OfferEntityIdFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[str]],
```

## OfferNameFilterTypeDef

```python
# OfferNameFilterTypeDef definition

class OfferNameFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[str]],
    WildCardValue: NotRequired[str],
```

## OfferProductIdFilterTypeDef

```python
# OfferProductIdFilterTypeDef definition

class OfferProductIdFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[str]],
```

## OfferResaleAuthorizationIdFilterTypeDef

```python
# OfferResaleAuthorizationIdFilterTypeDef definition

class OfferResaleAuthorizationIdFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[str]],
```

## OfferStateFilterTypeDef

```python
# OfferStateFilterTypeDef definition

class OfferStateFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[OfferStateStringType]],  # (1)
```

1. See [:material-code-brackets: OfferStateStringType](./literals.md#offerstatestringtype) 
## OfferTargetingFilterTypeDef

```python
# OfferTargetingFilterTypeDef definition

class OfferTargetingFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[OfferTargetingStringType]],  # (1)
```

1. See [:material-code-brackets: OfferTargetingStringType](./literals.md#offertargetingstringtype) 
## OfferLastModifiedDateFilterDateRangeTypeDef

```python
# OfferLastModifiedDateFilterDateRangeTypeDef definition

class OfferLastModifiedDateFilterDateRangeTypeDef(TypedDict):
    AfterValue: NotRequired[str],
    BeforeValue: NotRequired[str],
```

## OfferReleaseDateFilterDateRangeTypeDef

```python
# OfferReleaseDateFilterDateRangeTypeDef definition

class OfferReleaseDateFilterDateRangeTypeDef(TypedDict):
    AfterValue: NotRequired[str],
    BeforeValue: NotRequired[str],
```

## PutResourcePolicyRequestRequestTypeDef

```python
# PutResourcePolicyRequestRequestTypeDef definition

class PutResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Policy: str,
```

## ResaleAuthorizationAvailabilityEndDateFilterDateRangeTypeDef

```python
# ResaleAuthorizationAvailabilityEndDateFilterDateRangeTypeDef definition

class ResaleAuthorizationAvailabilityEndDateFilterDateRangeTypeDef(TypedDict):
    AfterValue: NotRequired[str],
    BeforeValue: NotRequired[str],
```

## ResaleAuthorizationCreatedDateFilterDateRangeTypeDef

```python
# ResaleAuthorizationCreatedDateFilterDateRangeTypeDef definition

class ResaleAuthorizationCreatedDateFilterDateRangeTypeDef(TypedDict):
    AfterValue: NotRequired[str],
    BeforeValue: NotRequired[str],
```

## ResaleAuthorizationEntityIdFilterTypeDef

```python
# ResaleAuthorizationEntityIdFilterTypeDef definition

class ResaleAuthorizationEntityIdFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[str]],
```

## ResaleAuthorizationManufacturerAccountIdFilterTypeDef

```python
# ResaleAuthorizationManufacturerAccountIdFilterTypeDef definition

class ResaleAuthorizationManufacturerAccountIdFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[str]],
    WildCardValue: NotRequired[str],
```

## ResaleAuthorizationManufacturerLegalNameFilterTypeDef

```python
# ResaleAuthorizationManufacturerLegalNameFilterTypeDef definition

class ResaleAuthorizationManufacturerLegalNameFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[str]],
    WildCardValue: NotRequired[str],
```

## ResaleAuthorizationNameFilterTypeDef

```python
# ResaleAuthorizationNameFilterTypeDef definition

class ResaleAuthorizationNameFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[str]],
    WildCardValue: NotRequired[str],
```

## ResaleAuthorizationOfferExtendedStatusFilterTypeDef

```python
# ResaleAuthorizationOfferExtendedStatusFilterTypeDef definition

class ResaleAuthorizationOfferExtendedStatusFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[str]],
```

## ResaleAuthorizationProductIdFilterTypeDef

```python
# ResaleAuthorizationProductIdFilterTypeDef definition

class ResaleAuthorizationProductIdFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[str]],
    WildCardValue: NotRequired[str],
```

## ResaleAuthorizationProductNameFilterTypeDef

```python
# ResaleAuthorizationProductNameFilterTypeDef definition

class ResaleAuthorizationProductNameFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[str]],
    WildCardValue: NotRequired[str],
```

## ResaleAuthorizationResellerAccountIDFilterTypeDef

```python
# ResaleAuthorizationResellerAccountIDFilterTypeDef definition

class ResaleAuthorizationResellerAccountIDFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[str]],
    WildCardValue: NotRequired[str],
```

## ResaleAuthorizationResellerLegalNameFilterTypeDef

```python
# ResaleAuthorizationResellerLegalNameFilterTypeDef definition

class ResaleAuthorizationResellerLegalNameFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[str]],
    WildCardValue: NotRequired[str],
```

## ResaleAuthorizationStatusFilterTypeDef

```python
# ResaleAuthorizationStatusFilterTypeDef definition

class ResaleAuthorizationStatusFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[ResaleAuthorizationStatusStringType]],  # (1)
```

1. See [:material-code-brackets: ResaleAuthorizationStatusStringType](./literals.md#resaleauthorizationstatusstringtype) 
## ResaleAuthorizationLastModifiedDateFilterDateRangeTypeDef

```python
# ResaleAuthorizationLastModifiedDateFilterDateRangeTypeDef definition

class ResaleAuthorizationLastModifiedDateFilterDateRangeTypeDef(TypedDict):
    AfterValue: NotRequired[str],
    BeforeValue: NotRequired[str],
```

## SaaSProductEntityIdFilterTypeDef

```python
# SaaSProductEntityIdFilterTypeDef definition

class SaaSProductEntityIdFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[str]],
```

## SaaSProductTitleFilterTypeDef

```python
# SaaSProductTitleFilterTypeDef definition

class SaaSProductTitleFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[str]],
    WildCardValue: NotRequired[str],
```

## SaaSProductVisibilityFilterTypeDef

```python
# SaaSProductVisibilityFilterTypeDef definition

class SaaSProductVisibilityFilterTypeDef(TypedDict):
    ValueList: NotRequired[Sequence[SaaSProductVisibilityStringType]],  # (1)
```

1. See [:material-code-brackets: SaaSProductVisibilityStringType](./literals.md#saasproductvisibilitystringtype) 
## SaaSProductLastModifiedDateFilterDateRangeTypeDef

```python
# SaaSProductLastModifiedDateFilterDateRangeTypeDef definition

class SaaSProductLastModifiedDateFilterDateRangeTypeDef(TypedDict):
    AfterValue: NotRequired[str],
    BeforeValue: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## AmiProductLastModifiedDateFilterTypeDef

```python
# AmiProductLastModifiedDateFilterTypeDef definition

class AmiProductLastModifiedDateFilterTypeDef(TypedDict):
    DateRange: NotRequired[AmiProductLastModifiedDateFilterDateRangeTypeDef],  # (1)
```

1. See [:material-code-braces: AmiProductLastModifiedDateFilterDateRangeTypeDef](./type_defs.md#amiproductlastmodifieddatefilterdaterangetypedef) 
## BatchDescribeEntitiesRequestRequestTypeDef

```python
# BatchDescribeEntitiesRequestRequestTypeDef definition

class BatchDescribeEntitiesRequestRequestTypeDef(TypedDict):
    EntityRequestList: Sequence[EntityRequestTypeDef],  # (1)
```

1. See [:material-code-braces: EntityRequestTypeDef](./type_defs.md#entityrequesttypedef) 
## BatchDescribeEntitiesResponseTypeDef

```python
# BatchDescribeEntitiesResponseTypeDef definition

class BatchDescribeEntitiesResponseTypeDef(TypedDict):
    EntityDetails: Dict[str, EntityDetailTypeDef],  # (1)
    Errors: Dict[str, BatchDescribeErrorDetailTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: EntityDetailTypeDef](./type_defs.md#entitydetailtypedef) 
2. See [:material-code-braces: BatchDescribeErrorDetailTypeDef](./type_defs.md#batchdescribeerrordetailtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelChangeSetResponseTypeDef

```python
# CancelChangeSetResponseTypeDef definition

class CancelChangeSetResponseTypeDef(TypedDict):
    ChangeSetId: str,
    ChangeSetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEntityResponseTypeDef

```python
# DescribeEntityResponseTypeDef definition

class DescribeEntityResponseTypeDef(TypedDict):
    EntityType: str,
    EntityIdentifier: str,
    EntityArn: str,
    LastModifiedDate: str,
    Details: str,
    DetailsDocument: Dict[str, Any],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePolicyResponseTypeDef

```python
# GetResourcePolicyResponseTypeDef definition

class GetResourcePolicyResponseTypeDef(TypedDict):
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartChangeSetResponseTypeDef

```python
# StartChangeSetResponseTypeDef definition

class StartChangeSetResponseTypeDef(TypedDict):
    ChangeSetId: str,
    ChangeSetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChangeSetsResponseTypeDef

```python
# ListChangeSetsResponseTypeDef definition

class ListChangeSetsResponseTypeDef(TypedDict):
    ChangeSetSummaryList: List[ChangeSetSummaryListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ChangeSetSummaryListItemTypeDef](./type_defs.md#changesetsummarylistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ChangeSummaryTypeDef

```python
# ChangeSummaryTypeDef definition

class ChangeSummaryTypeDef(TypedDict):
    ChangeType: NotRequired[str],
    Entity: NotRequired[EntityTypeDef],  # (1)
    Details: NotRequired[str],
    DetailsDocument: NotRequired[Dict[str, Any]],
    ErrorDetailList: NotRequired[List[ErrorDetailTypeDef]],  # (2)
    ChangeName: NotRequired[str],
```

1. See [:material-code-braces: EntityTypeDef](./type_defs.md#entitytypedef) 
2. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## ChangeTypeDef

```python
# ChangeTypeDef definition

class ChangeTypeDef(TypedDict):
    ChangeType: str,
    Entity: EntityTypeDef,  # (1)
    EntityTags: NotRequired[Sequence[TagTypeDef]],  # (2)
    Details: NotRequired[str],
    DetailsDocument: NotRequired[Mapping[str, Any]],
    ChangeName: NotRequired[str],
```

1. See [:material-code-braces: EntityTypeDef](./type_defs.md#entitytypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    ResourceArn: str,
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ContainerProductLastModifiedDateFilterTypeDef

```python
# ContainerProductLastModifiedDateFilterTypeDef definition

class ContainerProductLastModifiedDateFilterTypeDef(TypedDict):
    DateRange: NotRequired[ContainerProductLastModifiedDateFilterDateRangeTypeDef],  # (1)
```

1. See [:material-code-braces: ContainerProductLastModifiedDateFilterDateRangeTypeDef](./type_defs.md#containerproductlastmodifieddatefilterdaterangetypedef) 
## DataProductLastModifiedDateFilterTypeDef

```python
# DataProductLastModifiedDateFilterTypeDef definition

class DataProductLastModifiedDateFilterTypeDef(TypedDict):
    DateRange: NotRequired[DataProductLastModifiedDateFilterDateRangeTypeDef],  # (1)
```

1. See [:material-code-braces: DataProductLastModifiedDateFilterDateRangeTypeDef](./type_defs.md#dataproductlastmodifieddatefilterdaterangetypedef) 
## EntitySummaryTypeDef

```python
# EntitySummaryTypeDef definition

class EntitySummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    EntityType: NotRequired[str],
    EntityId: NotRequired[str],
    EntityArn: NotRequired[str],
    LastModifiedDate: NotRequired[str],
    Visibility: NotRequired[str],
    AmiProductSummary: NotRequired[AmiProductSummaryTypeDef],  # (1)
    ContainerProductSummary: NotRequired[ContainerProductSummaryTypeDef],  # (2)
    DataProductSummary: NotRequired[DataProductSummaryTypeDef],  # (3)
    SaaSProductSummary: NotRequired[SaaSProductSummaryTypeDef],  # (4)
    OfferSummary: NotRequired[OfferSummaryTypeDef],  # (5)
    ResaleAuthorizationSummary: NotRequired[ResaleAuthorizationSummaryTypeDef],  # (6)
```

1. See [:material-code-braces: AmiProductSummaryTypeDef](./type_defs.md#amiproductsummarytypedef) 
2. See [:material-code-braces: ContainerProductSummaryTypeDef](./type_defs.md#containerproductsummarytypedef) 
3. See [:material-code-braces: DataProductSummaryTypeDef](./type_defs.md#dataproductsummarytypedef) 
4. See [:material-code-braces: SaaSProductSummaryTypeDef](./type_defs.md#saasproductsummarytypedef) 
5. See [:material-code-braces: OfferSummaryTypeDef](./type_defs.md#offersummarytypedef) 
6. See [:material-code-braces: ResaleAuthorizationSummaryTypeDef](./type_defs.md#resaleauthorizationsummarytypedef) 
## EntityTypeSortTypeDef

```python
# EntityTypeSortTypeDef definition

class EntityTypeSortTypeDef(TypedDict):
    DataProductSort: NotRequired[DataProductSortTypeDef],  # (1)
    SaaSProductSort: NotRequired[SaaSProductSortTypeDef],  # (2)
    AmiProductSort: NotRequired[AmiProductSortTypeDef],  # (3)
    OfferSort: NotRequired[OfferSortTypeDef],  # (4)
    ContainerProductSort: NotRequired[ContainerProductSortTypeDef],  # (5)
    ResaleAuthorizationSort: NotRequired[ResaleAuthorizationSortTypeDef],  # (6)
```

1. See [:material-code-braces: DataProductSortTypeDef](./type_defs.md#dataproductsorttypedef) 
2. See [:material-code-braces: SaaSProductSortTypeDef](./type_defs.md#saasproductsorttypedef) 
3. See [:material-code-braces: AmiProductSortTypeDef](./type_defs.md#amiproductsorttypedef) 
4. See [:material-code-braces: OfferSortTypeDef](./type_defs.md#offersorttypedef) 
5. See [:material-code-braces: ContainerProductSortTypeDef](./type_defs.md#containerproductsorttypedef) 
6. See [:material-code-braces: ResaleAuthorizationSortTypeDef](./type_defs.md#resaleauthorizationsorttypedef) 
## ListChangeSetsRequestPaginateTypeDef

```python
# ListChangeSetsRequestPaginateTypeDef definition

class ListChangeSetsRequestPaginateTypeDef(TypedDict):
    Catalog: str,
    FilterList: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Sort: NotRequired[SortTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListChangeSetsRequestRequestTypeDef

```python
# ListChangeSetsRequestRequestTypeDef definition

class ListChangeSetsRequestRequestTypeDef(TypedDict):
    Catalog: str,
    FilterList: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Sort: NotRequired[SortTypeDef],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
## OfferAvailabilityEndDateFilterTypeDef

```python
# OfferAvailabilityEndDateFilterTypeDef definition

class OfferAvailabilityEndDateFilterTypeDef(TypedDict):
    DateRange: NotRequired[OfferAvailabilityEndDateFilterDateRangeTypeDef],  # (1)
```

1. See [:material-code-braces: OfferAvailabilityEndDateFilterDateRangeTypeDef](./type_defs.md#offeravailabilityenddatefilterdaterangetypedef) 
## OfferLastModifiedDateFilterTypeDef

```python
# OfferLastModifiedDateFilterTypeDef definition

class OfferLastModifiedDateFilterTypeDef(TypedDict):
    DateRange: NotRequired[OfferLastModifiedDateFilterDateRangeTypeDef],  # (1)
```

1. See [:material-code-braces: OfferLastModifiedDateFilterDateRangeTypeDef](./type_defs.md#offerlastmodifieddatefilterdaterangetypedef) 
## OfferReleaseDateFilterTypeDef

```python
# OfferReleaseDateFilterTypeDef definition

class OfferReleaseDateFilterTypeDef(TypedDict):
    DateRange: NotRequired[OfferReleaseDateFilterDateRangeTypeDef],  # (1)
```

1. See [:material-code-braces: OfferReleaseDateFilterDateRangeTypeDef](./type_defs.md#offerreleasedatefilterdaterangetypedef) 
## ResaleAuthorizationAvailabilityEndDateFilterTypeDef

```python
# ResaleAuthorizationAvailabilityEndDateFilterTypeDef definition

class ResaleAuthorizationAvailabilityEndDateFilterTypeDef(TypedDict):
    DateRange: NotRequired[ResaleAuthorizationAvailabilityEndDateFilterDateRangeTypeDef],  # (1)
    ValueList: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: ResaleAuthorizationAvailabilityEndDateFilterDateRangeTypeDef](./type_defs.md#resaleauthorizationavailabilityenddatefilterdaterangetypedef) 
## ResaleAuthorizationCreatedDateFilterTypeDef

```python
# ResaleAuthorizationCreatedDateFilterTypeDef definition

class ResaleAuthorizationCreatedDateFilterTypeDef(TypedDict):
    DateRange: NotRequired[ResaleAuthorizationCreatedDateFilterDateRangeTypeDef],  # (1)
    ValueList: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: ResaleAuthorizationCreatedDateFilterDateRangeTypeDef](./type_defs.md#resaleauthorizationcreateddatefilterdaterangetypedef) 
## ResaleAuthorizationLastModifiedDateFilterTypeDef

```python
# ResaleAuthorizationLastModifiedDateFilterTypeDef definition

class ResaleAuthorizationLastModifiedDateFilterTypeDef(TypedDict):
    DateRange: NotRequired[ResaleAuthorizationLastModifiedDateFilterDateRangeTypeDef],  # (1)
```

1. See [:material-code-braces: ResaleAuthorizationLastModifiedDateFilterDateRangeTypeDef](./type_defs.md#resaleauthorizationlastmodifieddatefilterdaterangetypedef) 
## SaaSProductLastModifiedDateFilterTypeDef

```python
# SaaSProductLastModifiedDateFilterTypeDef definition

class SaaSProductLastModifiedDateFilterTypeDef(TypedDict):
    DateRange: NotRequired[SaaSProductLastModifiedDateFilterDateRangeTypeDef],  # (1)
```

1. See [:material-code-braces: SaaSProductLastModifiedDateFilterDateRangeTypeDef](./type_defs.md#saasproductlastmodifieddatefilterdaterangetypedef) 
## AmiProductFiltersTypeDef

```python
# AmiProductFiltersTypeDef definition

class AmiProductFiltersTypeDef(TypedDict):
    EntityId: NotRequired[AmiProductEntityIdFilterTypeDef],  # (1)
    LastModifiedDate: NotRequired[AmiProductLastModifiedDateFilterTypeDef],  # (2)
    ProductTitle: NotRequired[AmiProductTitleFilterTypeDef],  # (3)
    Visibility: NotRequired[AmiProductVisibilityFilterTypeDef],  # (4)
```

1. See [:material-code-braces: AmiProductEntityIdFilterTypeDef](./type_defs.md#amiproductentityidfiltertypedef) 
2. See [:material-code-braces: AmiProductLastModifiedDateFilterTypeDef](./type_defs.md#amiproductlastmodifieddatefiltertypedef) 
3. See [:material-code-braces: AmiProductTitleFilterTypeDef](./type_defs.md#amiproducttitlefiltertypedef) 
4. See [:material-code-braces: AmiProductVisibilityFilterTypeDef](./type_defs.md#amiproductvisibilityfiltertypedef) 
## DescribeChangeSetResponseTypeDef

```python
# DescribeChangeSetResponseTypeDef definition

class DescribeChangeSetResponseTypeDef(TypedDict):
    ChangeSetId: str,
    ChangeSetArn: str,
    ChangeSetName: str,
    Intent: IntentType,  # (1)
    StartTime: str,
    EndTime: str,
    Status: ChangeStatusType,  # (2)
    FailureCode: FailureCodeType,  # (3)
    FailureDescription: str,
    ChangeSet: List[ChangeSummaryTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: IntentType](./literals.md#intenttype) 
2. See [:material-code-brackets: ChangeStatusType](./literals.md#changestatustype) 
3. See [:material-code-brackets: FailureCodeType](./literals.md#failurecodetype) 
4. See [:material-code-braces: ChangeSummaryTypeDef](./type_defs.md#changesummarytypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartChangeSetRequestRequestTypeDef

```python
# StartChangeSetRequestRequestTypeDef definition

class StartChangeSetRequestRequestTypeDef(TypedDict):
    Catalog: str,
    ChangeSet: Sequence[ChangeTypeDef],  # (1)
    ChangeSetName: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    ChangeSetTags: NotRequired[Sequence[TagTypeDef]],  # (2)
    Intent: NotRequired[IntentType],  # (3)
```

1. See [:material-code-braces: ChangeTypeDef](./type_defs.md#changetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: IntentType](./literals.md#intenttype) 
## ContainerProductFiltersTypeDef

```python
# ContainerProductFiltersTypeDef definition

class ContainerProductFiltersTypeDef(TypedDict):
    EntityId: NotRequired[ContainerProductEntityIdFilterTypeDef],  # (1)
    LastModifiedDate: NotRequired[ContainerProductLastModifiedDateFilterTypeDef],  # (2)
    ProductTitle: NotRequired[ContainerProductTitleFilterTypeDef],  # (3)
    Visibility: NotRequired[ContainerProductVisibilityFilterTypeDef],  # (4)
```

1. See [:material-code-braces: ContainerProductEntityIdFilterTypeDef](./type_defs.md#containerproductentityidfiltertypedef) 
2. See [:material-code-braces: ContainerProductLastModifiedDateFilterTypeDef](./type_defs.md#containerproductlastmodifieddatefiltertypedef) 
3. See [:material-code-braces: ContainerProductTitleFilterTypeDef](./type_defs.md#containerproducttitlefiltertypedef) 
4. See [:material-code-braces: ContainerProductVisibilityFilterTypeDef](./type_defs.md#containerproductvisibilityfiltertypedef) 
## DataProductFiltersTypeDef

```python
# DataProductFiltersTypeDef definition

class DataProductFiltersTypeDef(TypedDict):
    EntityId: NotRequired[DataProductEntityIdFilterTypeDef],  # (1)
    ProductTitle: NotRequired[DataProductTitleFilterTypeDef],  # (2)
    Visibility: NotRequired[DataProductVisibilityFilterTypeDef],  # (3)
    LastModifiedDate: NotRequired[DataProductLastModifiedDateFilterTypeDef],  # (4)
```

1. See [:material-code-braces: DataProductEntityIdFilterTypeDef](./type_defs.md#dataproductentityidfiltertypedef) 
2. See [:material-code-braces: DataProductTitleFilterTypeDef](./type_defs.md#dataproducttitlefiltertypedef) 
3. See [:material-code-braces: DataProductVisibilityFilterTypeDef](./type_defs.md#dataproductvisibilityfiltertypedef) 
4. See [:material-code-braces: DataProductLastModifiedDateFilterTypeDef](./type_defs.md#dataproductlastmodifieddatefiltertypedef) 
## ListEntitiesResponseTypeDef

```python
# ListEntitiesResponseTypeDef definition

class ListEntitiesResponseTypeDef(TypedDict):
    EntitySummaryList: List[EntitySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EntitySummaryTypeDef](./type_defs.md#entitysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OfferFiltersTypeDef

```python
# OfferFiltersTypeDef definition

class OfferFiltersTypeDef(TypedDict):
    EntityId: NotRequired[OfferEntityIdFilterTypeDef],  # (1)
    Name: NotRequired[OfferNameFilterTypeDef],  # (2)
    ProductId: NotRequired[OfferProductIdFilterTypeDef],  # (3)
    ResaleAuthorizationId: NotRequired[OfferResaleAuthorizationIdFilterTypeDef],  # (4)
    ReleaseDate: NotRequired[OfferReleaseDateFilterTypeDef],  # (5)
    AvailabilityEndDate: NotRequired[OfferAvailabilityEndDateFilterTypeDef],  # (6)
    BuyerAccounts: NotRequired[OfferBuyerAccountsFilterTypeDef],  # (7)
    State: NotRequired[OfferStateFilterTypeDef],  # (8)
    Targeting: NotRequired[OfferTargetingFilterTypeDef],  # (9)
    LastModifiedDate: NotRequired[OfferLastModifiedDateFilterTypeDef],  # (10)
```

1. See [:material-code-braces: OfferEntityIdFilterTypeDef](./type_defs.md#offerentityidfiltertypedef) 
2. See [:material-code-braces: OfferNameFilterTypeDef](./type_defs.md#offernamefiltertypedef) 
3. See [:material-code-braces: OfferProductIdFilterTypeDef](./type_defs.md#offerproductidfiltertypedef) 
4. See [:material-code-braces: OfferResaleAuthorizationIdFilterTypeDef](./type_defs.md#offerresaleauthorizationidfiltertypedef) 
5. See [:material-code-braces: OfferReleaseDateFilterTypeDef](./type_defs.md#offerreleasedatefiltertypedef) 
6. See [:material-code-braces: OfferAvailabilityEndDateFilterTypeDef](./type_defs.md#offeravailabilityenddatefiltertypedef) 
7. See [:material-code-braces: OfferBuyerAccountsFilterTypeDef](./type_defs.md#offerbuyeraccountsfiltertypedef) 
8. See [:material-code-braces: OfferStateFilterTypeDef](./type_defs.md#offerstatefiltertypedef) 
9. See [:material-code-braces: OfferTargetingFilterTypeDef](./type_defs.md#offertargetingfiltertypedef) 
10. See [:material-code-braces: OfferLastModifiedDateFilterTypeDef](./type_defs.md#offerlastmodifieddatefiltertypedef) 
## ResaleAuthorizationFiltersTypeDef

```python
# ResaleAuthorizationFiltersTypeDef definition

class ResaleAuthorizationFiltersTypeDef(TypedDict):
    EntityId: NotRequired[ResaleAuthorizationEntityIdFilterTypeDef],  # (1)
    Name: NotRequired[ResaleAuthorizationNameFilterTypeDef],  # (2)
    ProductId: NotRequired[ResaleAuthorizationProductIdFilterTypeDef],  # (3)
    CreatedDate: NotRequired[ResaleAuthorizationCreatedDateFilterTypeDef],  # (4)
    AvailabilityEndDate: NotRequired[ResaleAuthorizationAvailabilityEndDateFilterTypeDef],  # (5)
    ManufacturerAccountId: NotRequired[ResaleAuthorizationManufacturerAccountIdFilterTypeDef],  # (6)
    ProductName: NotRequired[ResaleAuthorizationProductNameFilterTypeDef],  # (7)
    ManufacturerLegalName: NotRequired[ResaleAuthorizationManufacturerLegalNameFilterTypeDef],  # (8)
    ResellerAccountID: NotRequired[ResaleAuthorizationResellerAccountIDFilterTypeDef],  # (9)
    ResellerLegalName: NotRequired[ResaleAuthorizationResellerLegalNameFilterTypeDef],  # (10)
    Status: NotRequired[ResaleAuthorizationStatusFilterTypeDef],  # (11)
    OfferExtendedStatus: NotRequired[ResaleAuthorizationOfferExtendedStatusFilterTypeDef],  # (12)
    LastModifiedDate: NotRequired[ResaleAuthorizationLastModifiedDateFilterTypeDef],  # (13)
```

1. See [:material-code-braces: ResaleAuthorizationEntityIdFilterTypeDef](./type_defs.md#resaleauthorizationentityidfiltertypedef) 
2. See [:material-code-braces: ResaleAuthorizationNameFilterTypeDef](./type_defs.md#resaleauthorizationnamefiltertypedef) 
3. See [:material-code-braces: ResaleAuthorizationProductIdFilterTypeDef](./type_defs.md#resaleauthorizationproductidfiltertypedef) 
4. See [:material-code-braces: ResaleAuthorizationCreatedDateFilterTypeDef](./type_defs.md#resaleauthorizationcreateddatefiltertypedef) 
5. See [:material-code-braces: ResaleAuthorizationAvailabilityEndDateFilterTypeDef](./type_defs.md#resaleauthorizationavailabilityenddatefiltertypedef) 
6. See [:material-code-braces: ResaleAuthorizationManufacturerAccountIdFilterTypeDef](./type_defs.md#resaleauthorizationmanufactureraccountidfiltertypedef) 
7. See [:material-code-braces: ResaleAuthorizationProductNameFilterTypeDef](./type_defs.md#resaleauthorizationproductnamefiltertypedef) 
8. See [:material-code-braces: ResaleAuthorizationManufacturerLegalNameFilterTypeDef](./type_defs.md#resaleauthorizationmanufacturerlegalnamefiltertypedef) 
9. See [:material-code-braces: ResaleAuthorizationResellerAccountIDFilterTypeDef](./type_defs.md#resaleauthorizationreselleraccountidfiltertypedef) 
10. See [:material-code-braces: ResaleAuthorizationResellerLegalNameFilterTypeDef](./type_defs.md#resaleauthorizationresellerlegalnamefiltertypedef) 
11. See [:material-code-braces: ResaleAuthorizationStatusFilterTypeDef](./type_defs.md#resaleauthorizationstatusfiltertypedef) 
12. See [:material-code-braces: ResaleAuthorizationOfferExtendedStatusFilterTypeDef](./type_defs.md#resaleauthorizationofferextendedstatusfiltertypedef) 
13. See [:material-code-braces: ResaleAuthorizationLastModifiedDateFilterTypeDef](./type_defs.md#resaleauthorizationlastmodifieddatefiltertypedef) 
## SaaSProductFiltersTypeDef

```python
# SaaSProductFiltersTypeDef definition

class SaaSProductFiltersTypeDef(TypedDict):
    EntityId: NotRequired[SaaSProductEntityIdFilterTypeDef],  # (1)
    ProductTitle: NotRequired[SaaSProductTitleFilterTypeDef],  # (2)
    Visibility: NotRequired[SaaSProductVisibilityFilterTypeDef],  # (3)
    LastModifiedDate: NotRequired[SaaSProductLastModifiedDateFilterTypeDef],  # (4)
```

1. See [:material-code-braces: SaaSProductEntityIdFilterTypeDef](./type_defs.md#saasproductentityidfiltertypedef) 
2. See [:material-code-braces: SaaSProductTitleFilterTypeDef](./type_defs.md#saasproducttitlefiltertypedef) 
3. See [:material-code-braces: SaaSProductVisibilityFilterTypeDef](./type_defs.md#saasproductvisibilityfiltertypedef) 
4. See [:material-code-braces: SaaSProductLastModifiedDateFilterTypeDef](./type_defs.md#saasproductlastmodifieddatefiltertypedef) 
## EntityTypeFiltersTypeDef

```python
# EntityTypeFiltersTypeDef definition

class EntityTypeFiltersTypeDef(TypedDict):
    DataProductFilters: NotRequired[DataProductFiltersTypeDef],  # (1)
    SaaSProductFilters: NotRequired[SaaSProductFiltersTypeDef],  # (2)
    AmiProductFilters: NotRequired[AmiProductFiltersTypeDef],  # (3)
    OfferFilters: NotRequired[OfferFiltersTypeDef],  # (4)
    ContainerProductFilters: NotRequired[ContainerProductFiltersTypeDef],  # (5)
    ResaleAuthorizationFilters: NotRequired[ResaleAuthorizationFiltersTypeDef],  # (6)
```

1. See [:material-code-braces: DataProductFiltersTypeDef](./type_defs.md#dataproductfilterstypedef) 
2. See [:material-code-braces: SaaSProductFiltersTypeDef](./type_defs.md#saasproductfilterstypedef) 
3. See [:material-code-braces: AmiProductFiltersTypeDef](./type_defs.md#amiproductfilterstypedef) 
4. See [:material-code-braces: OfferFiltersTypeDef](./type_defs.md#offerfilterstypedef) 
5. See [:material-code-braces: ContainerProductFiltersTypeDef](./type_defs.md#containerproductfilterstypedef) 
6. See [:material-code-braces: ResaleAuthorizationFiltersTypeDef](./type_defs.md#resaleauthorizationfilterstypedef) 
## ListEntitiesRequestPaginateTypeDef

```python
# ListEntitiesRequestPaginateTypeDef definition

class ListEntitiesRequestPaginateTypeDef(TypedDict):
    Catalog: str,
    EntityType: str,
    FilterList: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Sort: NotRequired[SortTypeDef],  # (2)
    OwnershipType: NotRequired[OwnershipTypeType],  # (3)
    EntityTypeFilters: NotRequired[EntityTypeFiltersTypeDef],  # (4)
    EntityTypeSort: NotRequired[EntityTypeSortTypeDef],  # (5)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (6)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-brackets: OwnershipTypeType](./literals.md#ownershiptypetype) 
4. See [:material-code-braces: EntityTypeFiltersTypeDef](./type_defs.md#entitytypefilterstypedef) 
5. See [:material-code-braces: EntityTypeSortTypeDef](./type_defs.md#entitytypesorttypedef) 
6. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEntitiesRequestRequestTypeDef

```python
# ListEntitiesRequestRequestTypeDef definition

class ListEntitiesRequestRequestTypeDef(TypedDict):
    Catalog: str,
    EntityType: str,
    FilterList: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Sort: NotRequired[SortTypeDef],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    OwnershipType: NotRequired[OwnershipTypeType],  # (3)
    EntityTypeFilters: NotRequired[EntityTypeFiltersTypeDef],  # (4)
    EntityTypeSort: NotRequired[EntityTypeSortTypeDef],  # (5)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-brackets: OwnershipTypeType](./literals.md#ownershiptypetype) 
4. See [:material-code-braces: EntityTypeFiltersTypeDef](./type_defs.md#entitytypefilterstypedef) 
5. See [:material-code-braces: EntityTypeSortTypeDef](./type_defs.md#entitytypesorttypedef) 
