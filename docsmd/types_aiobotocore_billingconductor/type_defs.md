# Type definitions

> [Index](../README.md) > [BillingConductor](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [BillingConductor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#billingconductor)
    type annotations stubs module [types-aiobotocore-billingconductor](https://pypi.org/project/types-aiobotocore-billingconductor/).

## LineItemFilterUnionTypeDef

```python
# LineItemFilterUnionTypeDef definition

LineItemFilterUnionTypeDef = Union[
    LineItemFilterTypeDef,  # (1)
    LineItemFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: LineItemFilterTypeDef](./type_defs.md#lineitemfiltertypedef) 
2. See [:material-code-braces: LineItemFilterOutputTypeDef](./type_defs.md#lineitemfilteroutputtypedef) 



## AccountAssociationsListElementTypeDef

```python
# AccountAssociationsListElementTypeDef definition

class AccountAssociationsListElementTypeDef(TypedDict):
    AccountId: NotRequired[str],
    BillingGroupArn: NotRequired[str],
    AccountName: NotRequired[str],
    AccountEmail: NotRequired[str],
```

## AccountGroupingTypeDef

```python
# AccountGroupingTypeDef definition

class AccountGroupingTypeDef(TypedDict):
    LinkedAccountIds: Sequence[str],
    AutoAssociate: NotRequired[bool],
```

## AssociateAccountsInputRequestTypeDef

```python
# AssociateAccountsInputRequestTypeDef definition

class AssociateAccountsInputRequestTypeDef(TypedDict):
    Arn: str,
    AccountIds: Sequence[str],
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

## AssociatePricingRulesInputRequestTypeDef

```python
# AssociatePricingRulesInputRequestTypeDef definition

class AssociatePricingRulesInputRequestTypeDef(TypedDict):
    Arn: str,
    PricingRuleArns: Sequence[str],
```

## AssociateResourceErrorTypeDef

```python
# AssociateResourceErrorTypeDef definition

class AssociateResourceErrorTypeDef(TypedDict):
    Message: NotRequired[str],
    Reason: NotRequired[AssociateResourceErrorReasonType],  # (1)
```

1. See [:material-code-brackets: AssociateResourceErrorReasonType](./literals.md#associateresourceerrorreasontype) 
## AttributeTypeDef

```python
# AttributeTypeDef definition

class AttributeTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## CustomLineItemBillingPeriodRangeTypeDef

```python
# CustomLineItemBillingPeriodRangeTypeDef definition

class CustomLineItemBillingPeriodRangeTypeDef(TypedDict):
    InclusiveStartBillingPeriod: str,
    ExclusiveEndBillingPeriod: NotRequired[str],
```

## BillingGroupCostReportElementTypeDef

```python
# BillingGroupCostReportElementTypeDef definition

class BillingGroupCostReportElementTypeDef(TypedDict):
    Arn: NotRequired[str],
    AWSCost: NotRequired[str],
    ProformaCost: NotRequired[str],
    Margin: NotRequired[str],
    MarginPercentage: NotRequired[str],
    Currency: NotRequired[str],
```

## ComputationPreferenceTypeDef

```python
# ComputationPreferenceTypeDef definition

class ComputationPreferenceTypeDef(TypedDict):
    PricingPlanArn: str,
```

## ListBillingGroupAccountGroupingTypeDef

```python
# ListBillingGroupAccountGroupingTypeDef definition

class ListBillingGroupAccountGroupingTypeDef(TypedDict):
    AutoAssociate: NotRequired[bool],
```

## BillingPeriodRangeTypeDef

```python
# BillingPeriodRangeTypeDef definition

class BillingPeriodRangeTypeDef(TypedDict):
    InclusiveStartBillingPeriod: str,
    ExclusiveEndBillingPeriod: str,
```

## CreateFreeTierConfigTypeDef

```python
# CreateFreeTierConfigTypeDef definition

class CreateFreeTierConfigTypeDef(TypedDict):
    Activated: bool,
```

## CreatePricingPlanInputRequestTypeDef

```python
# CreatePricingPlanInputRequestTypeDef definition

class CreatePricingPlanInputRequestTypeDef(TypedDict):
    Name: str,
    ClientToken: NotRequired[str],
    Description: NotRequired[str],
    PricingRuleArns: NotRequired[Sequence[str]],
    Tags: NotRequired[Mapping[str, str]],
```

## CustomLineItemFlatChargeDetailsTypeDef

```python
# CustomLineItemFlatChargeDetailsTypeDef definition

class CustomLineItemFlatChargeDetailsTypeDef(TypedDict):
    ChargeValue: float,
```

## CustomLineItemPercentageChargeDetailsTypeDef

```python
# CustomLineItemPercentageChargeDetailsTypeDef definition

class CustomLineItemPercentageChargeDetailsTypeDef(TypedDict):
    PercentageValue: float,
    AssociatedValues: NotRequired[Sequence[str]],
```

## DeleteBillingGroupInputRequestTypeDef

```python
# DeleteBillingGroupInputRequestTypeDef definition

class DeleteBillingGroupInputRequestTypeDef(TypedDict):
    Arn: str,
```

## DeletePricingPlanInputRequestTypeDef

```python
# DeletePricingPlanInputRequestTypeDef definition

class DeletePricingPlanInputRequestTypeDef(TypedDict):
    Arn: str,
```

## DeletePricingRuleInputRequestTypeDef

```python
# DeletePricingRuleInputRequestTypeDef definition

class DeletePricingRuleInputRequestTypeDef(TypedDict):
    Arn: str,
```

## DisassociateAccountsInputRequestTypeDef

```python
# DisassociateAccountsInputRequestTypeDef definition

class DisassociateAccountsInputRequestTypeDef(TypedDict):
    Arn: str,
    AccountIds: Sequence[str],
```

## DisassociatePricingRulesInputRequestTypeDef

```python
# DisassociatePricingRulesInputRequestTypeDef definition

class DisassociatePricingRulesInputRequestTypeDef(TypedDict):
    Arn: str,
    PricingRuleArns: Sequence[str],
```

## FreeTierConfigTypeDef

```python
# FreeTierConfigTypeDef definition

class FreeTierConfigTypeDef(TypedDict):
    Activated: bool,
```

## LineItemFilterOutputTypeDef

```python
# LineItemFilterOutputTypeDef definition

class LineItemFilterOutputTypeDef(TypedDict):
    Attribute: LineItemFilterAttributeNameType,  # (1)
    MatchOption: MatchOptionType,  # (2)
    Values: List[LineItemFilterValueType],  # (3)
```

1. See [:material-code-brackets: LineItemFilterAttributeNameType](./literals.md#lineitemfilterattributenametype) 
2. See [:material-code-brackets: MatchOptionType](./literals.md#matchoptiontype) 
3. See [:material-code-brackets: LineItemFilterValueType](./literals.md#lineitemfiltervaluetype) 
## LineItemFilterTypeDef

```python
# LineItemFilterTypeDef definition

class LineItemFilterTypeDef(TypedDict):
    Attribute: LineItemFilterAttributeNameType,  # (1)
    MatchOption: MatchOptionType,  # (2)
    Values: Sequence[LineItemFilterValueType],  # (3)
```

1. See [:material-code-brackets: LineItemFilterAttributeNameType](./literals.md#lineitemfilterattributenametype) 
2. See [:material-code-brackets: MatchOptionType](./literals.md#matchoptiontype) 
3. See [:material-code-brackets: LineItemFilterValueType](./literals.md#lineitemfiltervaluetype) 
## ListAccountAssociationsFilterTypeDef

```python
# ListAccountAssociationsFilterTypeDef definition

class ListAccountAssociationsFilterTypeDef(TypedDict):
    Association: NotRequired[str],
    AccountId: NotRequired[str],
    AccountIds: NotRequired[Sequence[str]],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListBillingGroupCostReportsFilterTypeDef

```python
# ListBillingGroupCostReportsFilterTypeDef definition

class ListBillingGroupCostReportsFilterTypeDef(TypedDict):
    BillingGroupArns: NotRequired[Sequence[str]],
```

## ListBillingGroupsFilterTypeDef

```python
# ListBillingGroupsFilterTypeDef definition

class ListBillingGroupsFilterTypeDef(TypedDict):
    Arns: NotRequired[Sequence[str]],
    PricingPlan: NotRequired[str],
    Statuses: NotRequired[Sequence[BillingGroupStatusType]],  # (1)
    AutoAssociate: NotRequired[bool],
```

1. See [:material-code-brackets: BillingGroupStatusType](./literals.md#billinggroupstatustype) 
## ListCustomLineItemFlatChargeDetailsTypeDef

```python
# ListCustomLineItemFlatChargeDetailsTypeDef definition

class ListCustomLineItemFlatChargeDetailsTypeDef(TypedDict):
    ChargeValue: float,
```

## ListCustomLineItemPercentageChargeDetailsTypeDef

```python
# ListCustomLineItemPercentageChargeDetailsTypeDef definition

class ListCustomLineItemPercentageChargeDetailsTypeDef(TypedDict):
    PercentageValue: float,
```

## ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef

```python
# ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef definition

class ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef(TypedDict):
    StartBillingPeriod: NotRequired[str],
    EndBillingPeriod: NotRequired[str],
```

## ListCustomLineItemsFilterTypeDef

```python
# ListCustomLineItemsFilterTypeDef definition

class ListCustomLineItemsFilterTypeDef(TypedDict):
    Names: NotRequired[Sequence[str]],
    BillingGroups: NotRequired[Sequence[str]],
    Arns: NotRequired[Sequence[str]],
    AccountIds: NotRequired[Sequence[str]],
```

## ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef

```python
# ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef definition

class ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef(TypedDict):
    PricingRuleArn: str,
    BillingPeriod: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListPricingPlansFilterTypeDef

```python
# ListPricingPlansFilterTypeDef definition

class ListPricingPlansFilterTypeDef(TypedDict):
    Arns: NotRequired[Sequence[str]],
```

## PricingPlanListElementTypeDef

```python
# PricingPlanListElementTypeDef definition

class PricingPlanListElementTypeDef(TypedDict):
    Name: NotRequired[str],
    Arn: NotRequired[str],
    Description: NotRequired[str],
    Size: NotRequired[int],
    CreationTime: NotRequired[int],
    LastModifiedTime: NotRequired[int],
```

## ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef

```python
# ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef definition

class ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef(TypedDict):
    PricingPlanArn: str,
    BillingPeriod: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListPricingRulesFilterTypeDef

```python
# ListPricingRulesFilterTypeDef definition

class ListPricingRulesFilterTypeDef(TypedDict):
    Arns: NotRequired[Sequence[str]],
```

## ListResourcesAssociatedToCustomLineItemFilterTypeDef

```python
# ListResourcesAssociatedToCustomLineItemFilterTypeDef definition

class ListResourcesAssociatedToCustomLineItemFilterTypeDef(TypedDict):
    Relationship: NotRequired[CustomLineItemRelationshipType],  # (1)
```

1. See [:material-code-brackets: CustomLineItemRelationshipType](./literals.md#customlineitemrelationshiptype) 
## ListResourcesAssociatedToCustomLineItemResponseElementTypeDef

```python
# ListResourcesAssociatedToCustomLineItemResponseElementTypeDef definition

class ListResourcesAssociatedToCustomLineItemResponseElementTypeDef(TypedDict):
    Arn: NotRequired[str],
    Relationship: NotRequired[CustomLineItemRelationshipType],  # (1)
    EndBillingPeriod: NotRequired[str],
```

1. See [:material-code-brackets: CustomLineItemRelationshipType](./literals.md#customlineitemrelationshiptype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateBillingGroupAccountGroupingTypeDef

```python
# UpdateBillingGroupAccountGroupingTypeDef definition

class UpdateBillingGroupAccountGroupingTypeDef(TypedDict):
    AutoAssociate: NotRequired[bool],
```

## UpdateCustomLineItemFlatChargeDetailsTypeDef

```python
# UpdateCustomLineItemFlatChargeDetailsTypeDef definition

class UpdateCustomLineItemFlatChargeDetailsTypeDef(TypedDict):
    ChargeValue: float,
```

## UpdateCustomLineItemPercentageChargeDetailsTypeDef

```python
# UpdateCustomLineItemPercentageChargeDetailsTypeDef definition

class UpdateCustomLineItemPercentageChargeDetailsTypeDef(TypedDict):
    PercentageValue: float,
```

## UpdateFreeTierConfigTypeDef

```python
# UpdateFreeTierConfigTypeDef definition

class UpdateFreeTierConfigTypeDef(TypedDict):
    Activated: bool,
```

## UpdatePricingPlanInputRequestTypeDef

```python
# UpdatePricingPlanInputRequestTypeDef definition

class UpdatePricingPlanInputRequestTypeDef(TypedDict):
    Arn: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## AssociateAccountsOutputTypeDef

```python
# AssociateAccountsOutputTypeDef definition

class AssociateAccountsOutputTypeDef(TypedDict):
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociatePricingRulesOutputTypeDef

```python
# AssociatePricingRulesOutputTypeDef definition

class AssociatePricingRulesOutputTypeDef(TypedDict):
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBillingGroupOutputTypeDef

```python
# CreateBillingGroupOutputTypeDef definition

class CreateBillingGroupOutputTypeDef(TypedDict):
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCustomLineItemOutputTypeDef

```python
# CreateCustomLineItemOutputTypeDef definition

class CreateCustomLineItemOutputTypeDef(TypedDict):
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePricingPlanOutputTypeDef

```python
# CreatePricingPlanOutputTypeDef definition

class CreatePricingPlanOutputTypeDef(TypedDict):
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePricingRuleOutputTypeDef

```python
# CreatePricingRuleOutputTypeDef definition

class CreatePricingRuleOutputTypeDef(TypedDict):
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBillingGroupOutputTypeDef

```python
# DeleteBillingGroupOutputTypeDef definition

class DeleteBillingGroupOutputTypeDef(TypedDict):
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteCustomLineItemOutputTypeDef

```python
# DeleteCustomLineItemOutputTypeDef definition

class DeleteCustomLineItemOutputTypeDef(TypedDict):
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePricingPlanOutputTypeDef

```python
# DeletePricingPlanOutputTypeDef definition

class DeletePricingPlanOutputTypeDef(TypedDict):
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePricingRuleOutputTypeDef

```python
# DeletePricingRuleOutputTypeDef definition

class DeletePricingRuleOutputTypeDef(TypedDict):
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateAccountsOutputTypeDef

```python
# DisassociateAccountsOutputTypeDef definition

class DisassociateAccountsOutputTypeDef(TypedDict):
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociatePricingRulesOutputTypeDef

```python
# DisassociatePricingRulesOutputTypeDef definition

class DisassociatePricingRulesOutputTypeDef(TypedDict):
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountAssociationsOutputTypeDef

```python
# ListAccountAssociationsOutputTypeDef definition

class ListAccountAssociationsOutputTypeDef(TypedDict):
    LinkedAccounts: List[AccountAssociationsListElementTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AccountAssociationsListElementTypeDef](./type_defs.md#accountassociationslistelementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPricingPlansAssociatedWithPricingRuleOutputTypeDef

```python
# ListPricingPlansAssociatedWithPricingRuleOutputTypeDef definition

class ListPricingPlansAssociatedWithPricingRuleOutputTypeDef(TypedDict):
    BillingPeriod: str,
    PricingRuleArn: str,
    PricingPlanArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPricingRulesAssociatedToPricingPlanOutputTypeDef

```python
# ListPricingRulesAssociatedToPricingPlanOutputTypeDef definition

class ListPricingRulesAssociatedToPricingPlanOutputTypeDef(TypedDict):
    BillingPeriod: str,
    PricingPlanArn: str,
    PricingRuleArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePricingPlanOutputTypeDef

```python
# UpdatePricingPlanOutputTypeDef definition

class UpdatePricingPlanOutputTypeDef(TypedDict):
    Arn: str,
    Name: str,
    Description: str,
    Size: int,
    LastModifiedTime: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateResourceResponseElementTypeDef

```python
# AssociateResourceResponseElementTypeDef definition

class AssociateResourceResponseElementTypeDef(TypedDict):
    Arn: NotRequired[str],
    Error: NotRequired[AssociateResourceErrorTypeDef],  # (1)
```

1. See [:material-code-braces: AssociateResourceErrorTypeDef](./type_defs.md#associateresourceerrortypedef) 
## DisassociateResourceResponseElementTypeDef

```python
# DisassociateResourceResponseElementTypeDef definition

class DisassociateResourceResponseElementTypeDef(TypedDict):
    Arn: NotRequired[str],
    Error: NotRequired[AssociateResourceErrorTypeDef],  # (1)
```

1. See [:material-code-braces: AssociateResourceErrorTypeDef](./type_defs.md#associateresourceerrortypedef) 
## BillingGroupCostReportResultElementTypeDef

```python
# BillingGroupCostReportResultElementTypeDef definition

class BillingGroupCostReportResultElementTypeDef(TypedDict):
    Arn: NotRequired[str],
    AWSCost: NotRequired[str],
    ProformaCost: NotRequired[str],
    Margin: NotRequired[str],
    MarginPercentage: NotRequired[str],
    Currency: NotRequired[str],
    Attributes: NotRequired[List[AttributeTypeDef]],  # (1)
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
## BatchAssociateResourcesToCustomLineItemInputRequestTypeDef

```python
# BatchAssociateResourcesToCustomLineItemInputRequestTypeDef definition

class BatchAssociateResourcesToCustomLineItemInputRequestTypeDef(TypedDict):
    TargetArn: str,
    ResourceArns: Sequence[str],
    BillingPeriodRange: NotRequired[CustomLineItemBillingPeriodRangeTypeDef],  # (1)
```

1. See [:material-code-braces: CustomLineItemBillingPeriodRangeTypeDef](./type_defs.md#customlineitembillingperiodrangetypedef) 
## BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef

```python
# BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef definition

class BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef(TypedDict):
    TargetArn: str,
    ResourceArns: Sequence[str],
    BillingPeriodRange: NotRequired[CustomLineItemBillingPeriodRangeTypeDef],  # (1)
```

1. See [:material-code-braces: CustomLineItemBillingPeriodRangeTypeDef](./type_defs.md#customlineitembillingperiodrangetypedef) 
## DeleteCustomLineItemInputRequestTypeDef

```python
# DeleteCustomLineItemInputRequestTypeDef definition

class DeleteCustomLineItemInputRequestTypeDef(TypedDict):
    Arn: str,
    BillingPeriodRange: NotRequired[CustomLineItemBillingPeriodRangeTypeDef],  # (1)
```

1. See [:material-code-braces: CustomLineItemBillingPeriodRangeTypeDef](./type_defs.md#customlineitembillingperiodrangetypedef) 
## ListBillingGroupCostReportsOutputTypeDef

```python
# ListBillingGroupCostReportsOutputTypeDef definition

class ListBillingGroupCostReportsOutputTypeDef(TypedDict):
    BillingGroupCostReports: List[BillingGroupCostReportElementTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BillingGroupCostReportElementTypeDef](./type_defs.md#billinggroupcostreportelementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBillingGroupInputRequestTypeDef

```python
# CreateBillingGroupInputRequestTypeDef definition

class CreateBillingGroupInputRequestTypeDef(TypedDict):
    Name: str,
    AccountGrouping: AccountGroupingTypeDef,  # (1)
    ComputationPreference: ComputationPreferenceTypeDef,  # (2)
    ClientToken: NotRequired[str],
    PrimaryAccountId: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AccountGroupingTypeDef](./type_defs.md#accountgroupingtypedef) 
2. See [:material-code-braces: ComputationPreferenceTypeDef](./type_defs.md#computationpreferencetypedef) 
## BillingGroupListElementTypeDef

```python
# BillingGroupListElementTypeDef definition

class BillingGroupListElementTypeDef(TypedDict):
    Name: NotRequired[str],
    Arn: NotRequired[str],
    Description: NotRequired[str],
    PrimaryAccountId: NotRequired[str],
    ComputationPreference: NotRequired[ComputationPreferenceTypeDef],  # (1)
    Size: NotRequired[int],
    CreationTime: NotRequired[int],
    LastModifiedTime: NotRequired[int],
    Status: NotRequired[BillingGroupStatusType],  # (2)
    StatusReason: NotRequired[str],
    AccountGrouping: NotRequired[ListBillingGroupAccountGroupingTypeDef],  # (3)
```

1. See [:material-code-braces: ComputationPreferenceTypeDef](./type_defs.md#computationpreferencetypedef) 
2. See [:material-code-brackets: BillingGroupStatusType](./literals.md#billinggroupstatustype) 
3. See [:material-code-braces: ListBillingGroupAccountGroupingTypeDef](./type_defs.md#listbillinggroupaccountgroupingtypedef) 
## GetBillingGroupCostReportInputRequestTypeDef

```python
# GetBillingGroupCostReportInputRequestTypeDef definition

class GetBillingGroupCostReportInputRequestTypeDef(TypedDict):
    Arn: str,
    BillingPeriodRange: NotRequired[BillingPeriodRangeTypeDef],  # (1)
    GroupBy: NotRequired[Sequence[GroupByAttributeNameType]],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BillingPeriodRangeTypeDef](./type_defs.md#billingperiodrangetypedef) 
2. See [:material-code-brackets: GroupByAttributeNameType](./literals.md#groupbyattributenametype) 
## CreateTieringInputTypeDef

```python
# CreateTieringInputTypeDef definition

class CreateTieringInputTypeDef(TypedDict):
    FreeTier: CreateFreeTierConfigTypeDef,  # (1)
```

1. See [:material-code-braces: CreateFreeTierConfigTypeDef](./type_defs.md#createfreetierconfigtypedef) 
## TieringTypeDef

```python
# TieringTypeDef definition

class TieringTypeDef(TypedDict):
    FreeTier: FreeTierConfigTypeDef,  # (1)
```

1. See [:material-code-braces: FreeTierConfigTypeDef](./type_defs.md#freetierconfigtypedef) 
## ListAccountAssociationsInputRequestTypeDef

```python
# ListAccountAssociationsInputRequestTypeDef definition

class ListAccountAssociationsInputRequestTypeDef(TypedDict):
    BillingPeriod: NotRequired[str],
    Filters: NotRequired[ListAccountAssociationsFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListAccountAssociationsFilterTypeDef](./type_defs.md#listaccountassociationsfiltertypedef) 
## ListAccountAssociationsInputPaginateTypeDef

```python
# ListAccountAssociationsInputPaginateTypeDef definition

class ListAccountAssociationsInputPaginateTypeDef(TypedDict):
    BillingPeriod: NotRequired[str],
    Filters: NotRequired[ListAccountAssociationsFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListAccountAssociationsFilterTypeDef](./type_defs.md#listaccountassociationsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPricingPlansAssociatedWithPricingRuleInputPaginateTypeDef

```python
# ListPricingPlansAssociatedWithPricingRuleInputPaginateTypeDef definition

class ListPricingPlansAssociatedWithPricingRuleInputPaginateTypeDef(TypedDict):
    PricingRuleArn: str,
    BillingPeriod: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPricingRulesAssociatedToPricingPlanInputPaginateTypeDef

```python
# ListPricingRulesAssociatedToPricingPlanInputPaginateTypeDef definition

class ListPricingRulesAssociatedToPricingPlanInputPaginateTypeDef(TypedDict):
    PricingPlanArn: str,
    BillingPeriod: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBillingGroupCostReportsInputPaginateTypeDef

```python
# ListBillingGroupCostReportsInputPaginateTypeDef definition

class ListBillingGroupCostReportsInputPaginateTypeDef(TypedDict):
    BillingPeriod: NotRequired[str],
    Filters: NotRequired[ListBillingGroupCostReportsFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListBillingGroupCostReportsFilterTypeDef](./type_defs.md#listbillinggroupcostreportsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBillingGroupCostReportsInputRequestTypeDef

```python
# ListBillingGroupCostReportsInputRequestTypeDef definition

class ListBillingGroupCostReportsInputRequestTypeDef(TypedDict):
    BillingPeriod: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[ListBillingGroupCostReportsFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ListBillingGroupCostReportsFilterTypeDef](./type_defs.md#listbillinggroupcostreportsfiltertypedef) 
## ListBillingGroupsInputPaginateTypeDef

```python
# ListBillingGroupsInputPaginateTypeDef definition

class ListBillingGroupsInputPaginateTypeDef(TypedDict):
    BillingPeriod: NotRequired[str],
    Filters: NotRequired[ListBillingGroupsFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListBillingGroupsFilterTypeDef](./type_defs.md#listbillinggroupsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBillingGroupsInputRequestTypeDef

```python
# ListBillingGroupsInputRequestTypeDef definition

class ListBillingGroupsInputRequestTypeDef(TypedDict):
    BillingPeriod: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[ListBillingGroupsFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ListBillingGroupsFilterTypeDef](./type_defs.md#listbillinggroupsfiltertypedef) 
## ListCustomLineItemChargeDetailsTypeDef

```python
# ListCustomLineItemChargeDetailsTypeDef definition

class ListCustomLineItemChargeDetailsTypeDef(TypedDict):
    Type: CustomLineItemTypeType,  # (3)
    Flat: NotRequired[ListCustomLineItemFlatChargeDetailsTypeDef],  # (1)
    Percentage: NotRequired[ListCustomLineItemPercentageChargeDetailsTypeDef],  # (2)
    LineItemFilters: NotRequired[List[LineItemFilterOutputTypeDef]],  # (4)
```

1. See [:material-code-braces: ListCustomLineItemFlatChargeDetailsTypeDef](./type_defs.md#listcustomlineitemflatchargedetailstypedef) 
2. See [:material-code-braces: ListCustomLineItemPercentageChargeDetailsTypeDef](./type_defs.md#listcustomlineitempercentagechargedetailstypedef) 
3. See [:material-code-brackets: CustomLineItemTypeType](./literals.md#customlineitemtypetype) 
4. See [:material-code-braces: LineItemFilterOutputTypeDef](./type_defs.md#lineitemfilteroutputtypedef) 
## ListCustomLineItemVersionsFilterTypeDef

```python
# ListCustomLineItemVersionsFilterTypeDef definition

class ListCustomLineItemVersionsFilterTypeDef(TypedDict):
    BillingPeriodRange: NotRequired[ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef](./type_defs.md#listcustomlineitemversionsbillingperiodrangefiltertypedef) 
## ListCustomLineItemsInputPaginateTypeDef

```python
# ListCustomLineItemsInputPaginateTypeDef definition

class ListCustomLineItemsInputPaginateTypeDef(TypedDict):
    BillingPeriod: NotRequired[str],
    Filters: NotRequired[ListCustomLineItemsFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListCustomLineItemsFilterTypeDef](./type_defs.md#listcustomlineitemsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCustomLineItemsInputRequestTypeDef

```python
# ListCustomLineItemsInputRequestTypeDef definition

class ListCustomLineItemsInputRequestTypeDef(TypedDict):
    BillingPeriod: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[ListCustomLineItemsFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ListCustomLineItemsFilterTypeDef](./type_defs.md#listcustomlineitemsfiltertypedef) 
## ListPricingPlansInputPaginateTypeDef

```python
# ListPricingPlansInputPaginateTypeDef definition

class ListPricingPlansInputPaginateTypeDef(TypedDict):
    BillingPeriod: NotRequired[str],
    Filters: NotRequired[ListPricingPlansFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListPricingPlansFilterTypeDef](./type_defs.md#listpricingplansfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPricingPlansInputRequestTypeDef

```python
# ListPricingPlansInputRequestTypeDef definition

class ListPricingPlansInputRequestTypeDef(TypedDict):
    BillingPeriod: NotRequired[str],
    Filters: NotRequired[ListPricingPlansFilterTypeDef],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListPricingPlansFilterTypeDef](./type_defs.md#listpricingplansfiltertypedef) 
## ListPricingPlansOutputTypeDef

```python
# ListPricingPlansOutputTypeDef definition

class ListPricingPlansOutputTypeDef(TypedDict):
    BillingPeriod: str,
    PricingPlans: List[PricingPlanListElementTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PricingPlanListElementTypeDef](./type_defs.md#pricingplanlistelementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPricingRulesInputPaginateTypeDef

```python
# ListPricingRulesInputPaginateTypeDef definition

class ListPricingRulesInputPaginateTypeDef(TypedDict):
    BillingPeriod: NotRequired[str],
    Filters: NotRequired[ListPricingRulesFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListPricingRulesFilterTypeDef](./type_defs.md#listpricingrulesfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPricingRulesInputRequestTypeDef

```python
# ListPricingRulesInputRequestTypeDef definition

class ListPricingRulesInputRequestTypeDef(TypedDict):
    BillingPeriod: NotRequired[str],
    Filters: NotRequired[ListPricingRulesFilterTypeDef],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListPricingRulesFilterTypeDef](./type_defs.md#listpricingrulesfiltertypedef) 
## ListResourcesAssociatedToCustomLineItemInputPaginateTypeDef

```python
# ListResourcesAssociatedToCustomLineItemInputPaginateTypeDef definition

class ListResourcesAssociatedToCustomLineItemInputPaginateTypeDef(TypedDict):
    Arn: str,
    BillingPeriod: NotRequired[str],
    Filters: NotRequired[ListResourcesAssociatedToCustomLineItemFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListResourcesAssociatedToCustomLineItemFilterTypeDef](./type_defs.md#listresourcesassociatedtocustomlineitemfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourcesAssociatedToCustomLineItemInputRequestTypeDef

```python
# ListResourcesAssociatedToCustomLineItemInputRequestTypeDef definition

class ListResourcesAssociatedToCustomLineItemInputRequestTypeDef(TypedDict):
    Arn: str,
    BillingPeriod: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[ListResourcesAssociatedToCustomLineItemFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ListResourcesAssociatedToCustomLineItemFilterTypeDef](./type_defs.md#listresourcesassociatedtocustomlineitemfiltertypedef) 
## ListResourcesAssociatedToCustomLineItemOutputTypeDef

```python
# ListResourcesAssociatedToCustomLineItemOutputTypeDef definition

class ListResourcesAssociatedToCustomLineItemOutputTypeDef(TypedDict):
    Arn: str,
    AssociatedResources: List[ListResourcesAssociatedToCustomLineItemResponseElementTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListResourcesAssociatedToCustomLineItemResponseElementTypeDef](./type_defs.md#listresourcesassociatedtocustomlineitemresponseelementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBillingGroupInputRequestTypeDef

```python
# UpdateBillingGroupInputRequestTypeDef definition

class UpdateBillingGroupInputRequestTypeDef(TypedDict):
    Arn: str,
    Name: NotRequired[str],
    Status: NotRequired[BillingGroupStatusType],  # (1)
    ComputationPreference: NotRequired[ComputationPreferenceTypeDef],  # (2)
    Description: NotRequired[str],
    AccountGrouping: NotRequired[UpdateBillingGroupAccountGroupingTypeDef],  # (3)
```

1. See [:material-code-brackets: BillingGroupStatusType](./literals.md#billinggroupstatustype) 
2. See [:material-code-braces: ComputationPreferenceTypeDef](./type_defs.md#computationpreferencetypedef) 
3. See [:material-code-braces: UpdateBillingGroupAccountGroupingTypeDef](./type_defs.md#updatebillinggroupaccountgroupingtypedef) 
## UpdateBillingGroupOutputTypeDef

```python
# UpdateBillingGroupOutputTypeDef definition

class UpdateBillingGroupOutputTypeDef(TypedDict):
    Arn: str,
    Name: str,
    Description: str,
    PrimaryAccountId: str,
    PricingPlanArn: str,
    Size: int,
    LastModifiedTime: int,
    Status: BillingGroupStatusType,  # (1)
    StatusReason: str,
    AccountGrouping: UpdateBillingGroupAccountGroupingTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: BillingGroupStatusType](./literals.md#billinggroupstatustype) 
2. See [:material-code-braces: UpdateBillingGroupAccountGroupingTypeDef](./type_defs.md#updatebillinggroupaccountgroupingtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTieringInputTypeDef

```python
# UpdateTieringInputTypeDef definition

class UpdateTieringInputTypeDef(TypedDict):
    FreeTier: UpdateFreeTierConfigTypeDef,  # (1)
```

1. See [:material-code-braces: UpdateFreeTierConfigTypeDef](./type_defs.md#updatefreetierconfigtypedef) 
## BatchAssociateResourcesToCustomLineItemOutputTypeDef

```python
# BatchAssociateResourcesToCustomLineItemOutputTypeDef definition

class BatchAssociateResourcesToCustomLineItemOutputTypeDef(TypedDict):
    SuccessfullyAssociatedResources: List[AssociateResourceResponseElementTypeDef],  # (1)
    FailedAssociatedResources: List[AssociateResourceResponseElementTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AssociateResourceResponseElementTypeDef](./type_defs.md#associateresourceresponseelementtypedef) 
2. See [:material-code-braces: AssociateResourceResponseElementTypeDef](./type_defs.md#associateresourceresponseelementtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDisassociateResourcesFromCustomLineItemOutputTypeDef

```python
# BatchDisassociateResourcesFromCustomLineItemOutputTypeDef definition

class BatchDisassociateResourcesFromCustomLineItemOutputTypeDef(TypedDict):
    SuccessfullyDisassociatedResources: List[DisassociateResourceResponseElementTypeDef],  # (1)
    FailedDisassociatedResources: List[DisassociateResourceResponseElementTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DisassociateResourceResponseElementTypeDef](./type_defs.md#disassociateresourceresponseelementtypedef) 
2. See [:material-code-braces: DisassociateResourceResponseElementTypeDef](./type_defs.md#disassociateresourceresponseelementtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBillingGroupCostReportOutputTypeDef

```python
# GetBillingGroupCostReportOutputTypeDef definition

class GetBillingGroupCostReportOutputTypeDef(TypedDict):
    BillingGroupCostReportResults: List[BillingGroupCostReportResultElementTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BillingGroupCostReportResultElementTypeDef](./type_defs.md#billinggroupcostreportresultelementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBillingGroupsOutputTypeDef

```python
# ListBillingGroupsOutputTypeDef definition

class ListBillingGroupsOutputTypeDef(TypedDict):
    BillingGroups: List[BillingGroupListElementTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BillingGroupListElementTypeDef](./type_defs.md#billinggrouplistelementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePricingRuleInputRequestTypeDef

```python
# CreatePricingRuleInputRequestTypeDef definition

class CreatePricingRuleInputRequestTypeDef(TypedDict):
    Name: str,
    Scope: PricingRuleScopeType,  # (1)
    Type: PricingRuleTypeType,  # (2)
    ClientToken: NotRequired[str],
    Description: NotRequired[str],
    ModifierPercentage: NotRequired[float],
    Service: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    BillingEntity: NotRequired[str],
    Tiering: NotRequired[CreateTieringInputTypeDef],  # (3)
    UsageType: NotRequired[str],
    Operation: NotRequired[str],
```

1. See [:material-code-brackets: PricingRuleScopeType](./literals.md#pricingrulescopetype) 
2. See [:material-code-brackets: PricingRuleTypeType](./literals.md#pricingruletypetype) 
3. See [:material-code-braces: CreateTieringInputTypeDef](./type_defs.md#createtieringinputtypedef) 
## PricingRuleListElementTypeDef

```python
# PricingRuleListElementTypeDef definition

class PricingRuleListElementTypeDef(TypedDict):
    Name: NotRequired[str],
    Arn: NotRequired[str],
    Description: NotRequired[str],
    Scope: NotRequired[PricingRuleScopeType],  # (1)
    Type: NotRequired[PricingRuleTypeType],  # (2)
    ModifierPercentage: NotRequired[float],
    Service: NotRequired[str],
    AssociatedPricingPlanCount: NotRequired[int],
    CreationTime: NotRequired[int],
    LastModifiedTime: NotRequired[int],
    BillingEntity: NotRequired[str],
    Tiering: NotRequired[TieringTypeDef],  # (3)
    UsageType: NotRequired[str],
    Operation: NotRequired[str],
```

1. See [:material-code-brackets: PricingRuleScopeType](./literals.md#pricingrulescopetype) 
2. See [:material-code-brackets: PricingRuleTypeType](./literals.md#pricingruletypetype) 
3. See [:material-code-braces: TieringTypeDef](./type_defs.md#tieringtypedef) 
## CustomLineItemChargeDetailsTypeDef

```python
# CustomLineItemChargeDetailsTypeDef definition

class CustomLineItemChargeDetailsTypeDef(TypedDict):
    Type: CustomLineItemTypeType,  # (3)
    Flat: NotRequired[CustomLineItemFlatChargeDetailsTypeDef],  # (1)
    Percentage: NotRequired[CustomLineItemPercentageChargeDetailsTypeDef],  # (2)
    LineItemFilters: NotRequired[Sequence[LineItemFilterUnionTypeDef]],  # (4)
```

1. See [:material-code-braces: CustomLineItemFlatChargeDetailsTypeDef](./type_defs.md#customlineitemflatchargedetailstypedef) 
2. See [:material-code-braces: CustomLineItemPercentageChargeDetailsTypeDef](./type_defs.md#customlineitempercentagechargedetailstypedef) 
3. See [:material-code-brackets: CustomLineItemTypeType](./literals.md#customlineitemtypetype) 
4. See [:material-code-braces: LineItemFilterTypeDef](./type_defs.md#lineitemfiltertypedef) [:material-code-braces: LineItemFilterOutputTypeDef](./type_defs.md#lineitemfilteroutputtypedef) 
## UpdateCustomLineItemChargeDetailsTypeDef

```python
# UpdateCustomLineItemChargeDetailsTypeDef definition

class UpdateCustomLineItemChargeDetailsTypeDef(TypedDict):
    Flat: NotRequired[UpdateCustomLineItemFlatChargeDetailsTypeDef],  # (1)
    Percentage: NotRequired[UpdateCustomLineItemPercentageChargeDetailsTypeDef],  # (2)
    LineItemFilters: NotRequired[Sequence[LineItemFilterUnionTypeDef]],  # (3)
```

1. See [:material-code-braces: UpdateCustomLineItemFlatChargeDetailsTypeDef](./type_defs.md#updatecustomlineitemflatchargedetailstypedef) 
2. See [:material-code-braces: UpdateCustomLineItemPercentageChargeDetailsTypeDef](./type_defs.md#updatecustomlineitempercentagechargedetailstypedef) 
3. See [:material-code-braces: LineItemFilterTypeDef](./type_defs.md#lineitemfiltertypedef) [:material-code-braces: LineItemFilterOutputTypeDef](./type_defs.md#lineitemfilteroutputtypedef) 
## CustomLineItemListElementTypeDef

```python
# CustomLineItemListElementTypeDef definition

class CustomLineItemListElementTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
    ChargeDetails: NotRequired[ListCustomLineItemChargeDetailsTypeDef],  # (1)
    CurrencyCode: NotRequired[CurrencyCodeType],  # (2)
    Description: NotRequired[str],
    ProductCode: NotRequired[str],
    BillingGroupArn: NotRequired[str],
    CreationTime: NotRequired[int],
    LastModifiedTime: NotRequired[int],
    AssociationSize: NotRequired[int],
    AccountId: NotRequired[str],
```

1. See [:material-code-braces: ListCustomLineItemChargeDetailsTypeDef](./type_defs.md#listcustomlineitemchargedetailstypedef) 
2. See [:material-code-brackets: CurrencyCodeType](./literals.md#currencycodetype) 
## CustomLineItemVersionListElementTypeDef

```python
# CustomLineItemVersionListElementTypeDef definition

class CustomLineItemVersionListElementTypeDef(TypedDict):
    Name: NotRequired[str],
    ChargeDetails: NotRequired[ListCustomLineItemChargeDetailsTypeDef],  # (1)
    CurrencyCode: NotRequired[CurrencyCodeType],  # (2)
    Description: NotRequired[str],
    ProductCode: NotRequired[str],
    BillingGroupArn: NotRequired[str],
    CreationTime: NotRequired[int],
    LastModifiedTime: NotRequired[int],
    AssociationSize: NotRequired[int],
    StartBillingPeriod: NotRequired[str],
    EndBillingPeriod: NotRequired[str],
    Arn: NotRequired[str],
    StartTime: NotRequired[int],
    AccountId: NotRequired[str],
```

1. See [:material-code-braces: ListCustomLineItemChargeDetailsTypeDef](./type_defs.md#listcustomlineitemchargedetailstypedef) 
2. See [:material-code-brackets: CurrencyCodeType](./literals.md#currencycodetype) 
## UpdateCustomLineItemOutputTypeDef

```python
# UpdateCustomLineItemOutputTypeDef definition

class UpdateCustomLineItemOutputTypeDef(TypedDict):
    Arn: str,
    BillingGroupArn: str,
    Name: str,
    Description: str,
    ChargeDetails: ListCustomLineItemChargeDetailsTypeDef,  # (1)
    LastModifiedTime: int,
    AssociationSize: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListCustomLineItemChargeDetailsTypeDef](./type_defs.md#listcustomlineitemchargedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCustomLineItemVersionsInputPaginateTypeDef

```python
# ListCustomLineItemVersionsInputPaginateTypeDef definition

class ListCustomLineItemVersionsInputPaginateTypeDef(TypedDict):
    Arn: str,
    Filters: NotRequired[ListCustomLineItemVersionsFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListCustomLineItemVersionsFilterTypeDef](./type_defs.md#listcustomlineitemversionsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCustomLineItemVersionsInputRequestTypeDef

```python
# ListCustomLineItemVersionsInputRequestTypeDef definition

class ListCustomLineItemVersionsInputRequestTypeDef(TypedDict):
    Arn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[ListCustomLineItemVersionsFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ListCustomLineItemVersionsFilterTypeDef](./type_defs.md#listcustomlineitemversionsfiltertypedef) 
## UpdatePricingRuleInputRequestTypeDef

```python
# UpdatePricingRuleInputRequestTypeDef definition

class UpdatePricingRuleInputRequestTypeDef(TypedDict):
    Arn: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    Type: NotRequired[PricingRuleTypeType],  # (1)
    ModifierPercentage: NotRequired[float],
    Tiering: NotRequired[UpdateTieringInputTypeDef],  # (2)
```

1. See [:material-code-brackets: PricingRuleTypeType](./literals.md#pricingruletypetype) 
2. See [:material-code-braces: UpdateTieringInputTypeDef](./type_defs.md#updatetieringinputtypedef) 
## UpdatePricingRuleOutputTypeDef

```python
# UpdatePricingRuleOutputTypeDef definition

class UpdatePricingRuleOutputTypeDef(TypedDict):
    Arn: str,
    Name: str,
    Description: str,
    Scope: PricingRuleScopeType,  # (1)
    Type: PricingRuleTypeType,  # (2)
    ModifierPercentage: float,
    Service: str,
    AssociatedPricingPlanCount: int,
    LastModifiedTime: int,
    BillingEntity: str,
    Tiering: UpdateTieringInputTypeDef,  # (3)
    UsageType: str,
    Operation: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: PricingRuleScopeType](./literals.md#pricingrulescopetype) 
2. See [:material-code-brackets: PricingRuleTypeType](./literals.md#pricingruletypetype) 
3. See [:material-code-braces: UpdateTieringInputTypeDef](./type_defs.md#updatetieringinputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPricingRulesOutputTypeDef

```python
# ListPricingRulesOutputTypeDef definition

class ListPricingRulesOutputTypeDef(TypedDict):
    BillingPeriod: str,
    PricingRules: List[PricingRuleListElementTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PricingRuleListElementTypeDef](./type_defs.md#pricingrulelistelementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCustomLineItemInputRequestTypeDef

```python
# CreateCustomLineItemInputRequestTypeDef definition

class CreateCustomLineItemInputRequestTypeDef(TypedDict):
    Name: str,
    Description: str,
    BillingGroupArn: str,
    ChargeDetails: CustomLineItemChargeDetailsTypeDef,  # (1)
    ClientToken: NotRequired[str],
    BillingPeriodRange: NotRequired[CustomLineItemBillingPeriodRangeTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
    AccountId: NotRequired[str],
```

1. See [:material-code-braces: CustomLineItemChargeDetailsTypeDef](./type_defs.md#customlineitemchargedetailstypedef) 
2. See [:material-code-braces: CustomLineItemBillingPeriodRangeTypeDef](./type_defs.md#customlineitembillingperiodrangetypedef) 
## UpdateCustomLineItemInputRequestTypeDef

```python
# UpdateCustomLineItemInputRequestTypeDef definition

class UpdateCustomLineItemInputRequestTypeDef(TypedDict):
    Arn: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    ChargeDetails: NotRequired[UpdateCustomLineItemChargeDetailsTypeDef],  # (1)
    BillingPeriodRange: NotRequired[CustomLineItemBillingPeriodRangeTypeDef],  # (2)
```

1. See [:material-code-braces: UpdateCustomLineItemChargeDetailsTypeDef](./type_defs.md#updatecustomlineitemchargedetailstypedef) 
2. See [:material-code-braces: CustomLineItemBillingPeriodRangeTypeDef](./type_defs.md#customlineitembillingperiodrangetypedef) 
## ListCustomLineItemsOutputTypeDef

```python
# ListCustomLineItemsOutputTypeDef definition

class ListCustomLineItemsOutputTypeDef(TypedDict):
    CustomLineItems: List[CustomLineItemListElementTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CustomLineItemListElementTypeDef](./type_defs.md#customlineitemlistelementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCustomLineItemVersionsOutputTypeDef

```python
# ListCustomLineItemVersionsOutputTypeDef definition

class ListCustomLineItemVersionsOutputTypeDef(TypedDict):
    CustomLineItemVersions: List[CustomLineItemVersionListElementTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CustomLineItemVersionListElementTypeDef](./type_defs.md#customlineitemversionlistelementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
