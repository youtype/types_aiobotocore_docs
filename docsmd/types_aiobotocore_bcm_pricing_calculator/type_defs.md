# Type definitions

> [Index](../README.md) > [BillingandCostManagementPricingCalculator](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [BillingandCostManagementPricingCalculator](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-pricing-calculator.html#billingandcostmanagementpricingcalculator)
    type annotations stubs module [types-aiobotocore-bcm-pricing-calculator](https://pypi.org/project/types-aiobotocore-bcm-pricing-calculator/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## ExpressionFilterUnionTypeDef

```python
# ExpressionFilterUnionTypeDef definition

ExpressionFilterUnionTypeDef = Union[
    ExpressionFilterTypeDef,  # (1)
    ExpressionFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ExpressionFilterTypeDef](./type_defs.md#expressionfiltertypedef) 
2. See [:material-code-braces: ExpressionFilterOutputTypeDef](./type_defs.md#expressionfilteroutputtypedef) 

## BillIntervalUnionTypeDef

```python
# BillIntervalUnionTypeDef definition

BillIntervalUnionTypeDef = Union[
    BillIntervalTypeDef,  # (1)
    BillIntervalOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: BillIntervalTypeDef](./type_defs.md#billintervaltypedef) 
2. See [:material-code-braces: BillIntervalOutputTypeDef](./type_defs.md#billintervaloutputtypedef) 

## ExpressionUnionTypeDef

```python
# ExpressionUnionTypeDef definition

ExpressionUnionTypeDef = Union[
    ExpressionTypeDef,  # (1)
    ExpressionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
2. See [:material-code-braces: ExpressionOutputTypeDef](./type_defs.md#expressionoutputtypedef) 

## HistoricalUsageEntityUnionTypeDef

```python
# HistoricalUsageEntityUnionTypeDef definition

HistoricalUsageEntityUnionTypeDef = Union[
    HistoricalUsageEntityTypeDef,  # (1)
    HistoricalUsageEntityOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HistoricalUsageEntityTypeDef](./type_defs.md#historicalusageentitytypedef) 
2. See [:material-code-braces: HistoricalUsageEntityOutputTypeDef](./type_defs.md#historicalusageentityoutputtypedef) 



## AddReservedInstanceActionTypeDef

```python
# AddReservedInstanceActionTypeDef definition

class AddReservedInstanceActionTypeDef(TypedDict):
    reservedInstancesOfferingId: NotRequired[str],
    instanceCount: NotRequired[int],
```

## AddSavingsPlanActionTypeDef

```python
# AddSavingsPlanActionTypeDef definition

class AddSavingsPlanActionTypeDef(TypedDict):
    savingsPlanOfferingId: NotRequired[str],
    commitment: NotRequired[float],
```

## BatchCreateBillScenarioCommitmentModificationErrorTypeDef

```python
# BatchCreateBillScenarioCommitmentModificationErrorTypeDef definition

class BatchCreateBillScenarioCommitmentModificationErrorTypeDef(TypedDict):
    key: NotRequired[str],
    errorMessage: NotRequired[str],
    errorCode: NotRequired[BatchCreateBillScenarioCommitmentModificationErrorCodeType],  # (1)
```

1. See [:material-code-brackets: BatchCreateBillScenarioCommitmentModificationErrorCodeType](./literals.md#batchcreatebillscenariocommitmentmodificationerrorcodetype) 
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

## BatchCreateBillScenarioUsageModificationErrorTypeDef

```python
# BatchCreateBillScenarioUsageModificationErrorTypeDef definition

class BatchCreateBillScenarioUsageModificationErrorTypeDef(TypedDict):
    key: NotRequired[str],
    errorMessage: NotRequired[str],
    errorCode: NotRequired[BatchCreateBillScenarioUsageModificationErrorCodeType],  # (1)
```

1. See [:material-code-brackets: BatchCreateBillScenarioUsageModificationErrorCodeType](./literals.md#batchcreatebillscenariousagemodificationerrorcodetype) 
## UsageQuantityTypeDef

```python
# UsageQuantityTypeDef definition

class UsageQuantityTypeDef(TypedDict):
    startHour: NotRequired[datetime],
    unit: NotRequired[str],
    amount: NotRequired[float],
```

## BatchCreateWorkloadEstimateUsageErrorTypeDef

```python
# BatchCreateWorkloadEstimateUsageErrorTypeDef definition

class BatchCreateWorkloadEstimateUsageErrorTypeDef(TypedDict):
    key: NotRequired[str],
    errorCode: NotRequired[BatchCreateWorkloadEstimateUsageCodeType],  # (1)
    errorMessage: NotRequired[str],
```

1. See [:material-code-brackets: BatchCreateWorkloadEstimateUsageCodeType](./literals.md#batchcreateworkloadestimateusagecodetype) 
## WorkloadEstimateUsageQuantityTypeDef

```python
# WorkloadEstimateUsageQuantityTypeDef definition

class WorkloadEstimateUsageQuantityTypeDef(TypedDict):
    unit: NotRequired[str],
    amount: NotRequired[float],
```

## BatchDeleteBillScenarioCommitmentModificationErrorTypeDef

```python
# BatchDeleteBillScenarioCommitmentModificationErrorTypeDef definition

class BatchDeleteBillScenarioCommitmentModificationErrorTypeDef(TypedDict):
    id: NotRequired[str],
    errorCode: NotRequired[BatchDeleteBillScenarioCommitmentModificationErrorCodeType],  # (1)
    errorMessage: NotRequired[str],
```

1. See [:material-code-brackets: BatchDeleteBillScenarioCommitmentModificationErrorCodeType](./literals.md#batchdeletebillscenariocommitmentmodificationerrorcodetype) 
## BatchDeleteBillScenarioCommitmentModificationRequestRequestTypeDef

```python
# BatchDeleteBillScenarioCommitmentModificationRequestRequestTypeDef definition

class BatchDeleteBillScenarioCommitmentModificationRequestRequestTypeDef(TypedDict):
    billScenarioId: str,
    ids: Sequence[str],
```

## BatchDeleteBillScenarioUsageModificationErrorTypeDef

```python
# BatchDeleteBillScenarioUsageModificationErrorTypeDef definition

class BatchDeleteBillScenarioUsageModificationErrorTypeDef(TypedDict):
    id: NotRequired[str],
    errorMessage: NotRequired[str],
    errorCode: NotRequired[BatchDeleteBillScenarioUsageModificationErrorCodeType],  # (1)
```

1. See [:material-code-brackets: BatchDeleteBillScenarioUsageModificationErrorCodeType](./literals.md#batchdeletebillscenariousagemodificationerrorcodetype) 
## BatchDeleteBillScenarioUsageModificationRequestRequestTypeDef

```python
# BatchDeleteBillScenarioUsageModificationRequestRequestTypeDef definition

class BatchDeleteBillScenarioUsageModificationRequestRequestTypeDef(TypedDict):
    billScenarioId: str,
    ids: Sequence[str],
```

## BatchDeleteWorkloadEstimateUsageErrorTypeDef

```python
# BatchDeleteWorkloadEstimateUsageErrorTypeDef definition

class BatchDeleteWorkloadEstimateUsageErrorTypeDef(TypedDict):
    id: NotRequired[str],
    errorMessage: NotRequired[str],
    errorCode: NotRequired[WorkloadEstimateUpdateUsageErrorCodeType],  # (1)
```

1. See [:material-code-brackets: WorkloadEstimateUpdateUsageErrorCodeType](./literals.md#workloadestimateupdateusageerrorcodetype) 
## BatchDeleteWorkloadEstimateUsageRequestRequestTypeDef

```python
# BatchDeleteWorkloadEstimateUsageRequestRequestTypeDef definition

class BatchDeleteWorkloadEstimateUsageRequestRequestTypeDef(TypedDict):
    workloadEstimateId: str,
    ids: Sequence[str],
```

## BatchUpdateBillScenarioCommitmentModificationEntryTypeDef

```python
# BatchUpdateBillScenarioCommitmentModificationEntryTypeDef definition

class BatchUpdateBillScenarioCommitmentModificationEntryTypeDef(TypedDict):
    id: str,
    group: NotRequired[str],
```

## BatchUpdateBillScenarioCommitmentModificationErrorTypeDef

```python
# BatchUpdateBillScenarioCommitmentModificationErrorTypeDef definition

class BatchUpdateBillScenarioCommitmentModificationErrorTypeDef(TypedDict):
    id: NotRequired[str],
    errorCode: NotRequired[BatchUpdateBillScenarioCommitmentModificationErrorCodeType],  # (1)
    errorMessage: NotRequired[str],
```

1. See [:material-code-brackets: BatchUpdateBillScenarioCommitmentModificationErrorCodeType](./literals.md#batchupdatebillscenariocommitmentmodificationerrorcodetype) 
## BatchUpdateBillScenarioUsageModificationErrorTypeDef

```python
# BatchUpdateBillScenarioUsageModificationErrorTypeDef definition

class BatchUpdateBillScenarioUsageModificationErrorTypeDef(TypedDict):
    id: NotRequired[str],
    errorMessage: NotRequired[str],
    errorCode: NotRequired[BatchUpdateBillScenarioUsageModificationErrorCodeType],  # (1)
```

1. See [:material-code-brackets: BatchUpdateBillScenarioUsageModificationErrorCodeType](./literals.md#batchupdatebillscenariousagemodificationerrorcodetype) 
## BatchUpdateWorkloadEstimateUsageEntryTypeDef

```python
# BatchUpdateWorkloadEstimateUsageEntryTypeDef definition

class BatchUpdateWorkloadEstimateUsageEntryTypeDef(TypedDict):
    id: str,
    group: NotRequired[str],
    amount: NotRequired[float],
```

## BatchUpdateWorkloadEstimateUsageErrorTypeDef

```python
# BatchUpdateWorkloadEstimateUsageErrorTypeDef definition

class BatchUpdateWorkloadEstimateUsageErrorTypeDef(TypedDict):
    id: NotRequired[str],
    errorMessage: NotRequired[str],
    errorCode: NotRequired[WorkloadEstimateUpdateUsageErrorCodeType],  # (1)
```

1. See [:material-code-brackets: WorkloadEstimateUpdateUsageErrorCodeType](./literals.md#workloadestimateupdateusageerrorcodetype) 
## CostAmountTypeDef

```python
# CostAmountTypeDef definition

class CostAmountTypeDef(TypedDict):
    amount: NotRequired[float],
    currency: NotRequired[CurrencyCodeType],  # (1)
```

1. See [:material-code-brackets: CurrencyCodeType](./literals.md#currencycodetype) 
## UsageQuantityResultTypeDef

```python
# UsageQuantityResultTypeDef definition

class UsageQuantityResultTypeDef(TypedDict):
    amount: NotRequired[float],
    unit: NotRequired[str],
```

## BillIntervalOutputTypeDef

```python
# BillIntervalOutputTypeDef definition

class BillIntervalOutputTypeDef(TypedDict):
    start: NotRequired[datetime],
    end: NotRequired[datetime],
```

## NegateReservedInstanceActionTypeDef

```python
# NegateReservedInstanceActionTypeDef definition

class NegateReservedInstanceActionTypeDef(TypedDict):
    reservedInstancesId: NotRequired[str],
```

## NegateSavingsPlanActionTypeDef

```python
# NegateSavingsPlanActionTypeDef definition

class NegateSavingsPlanActionTypeDef(TypedDict):
    savingsPlanId: NotRequired[str],
```

## CreateBillEstimateRequestRequestTypeDef

```python
# CreateBillEstimateRequestRequestTypeDef definition

class CreateBillEstimateRequestRequestTypeDef(TypedDict):
    billScenarioId: str,
    name: str,
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## CreateBillScenarioRequestRequestTypeDef

```python
# CreateBillScenarioRequestRequestTypeDef definition

class CreateBillScenarioRequestRequestTypeDef(TypedDict):
    name: str,
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## CreateWorkloadEstimateRequestRequestTypeDef

```python
# CreateWorkloadEstimateRequestRequestTypeDef definition

class CreateWorkloadEstimateRequestRequestTypeDef(TypedDict):
    name: str,
    clientToken: NotRequired[str],
    rateType: NotRequired[WorkloadEstimateRateTypeType],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: WorkloadEstimateRateTypeType](./literals.md#workloadestimateratetypetype) 
## DeleteBillEstimateRequestRequestTypeDef

```python
# DeleteBillEstimateRequestRequestTypeDef definition

class DeleteBillEstimateRequestRequestTypeDef(TypedDict):
    identifier: str,
```

## DeleteBillScenarioRequestRequestTypeDef

```python
# DeleteBillScenarioRequestRequestTypeDef definition

class DeleteBillScenarioRequestRequestTypeDef(TypedDict):
    identifier: str,
```

## DeleteWorkloadEstimateRequestRequestTypeDef

```python
# DeleteWorkloadEstimateRequestRequestTypeDef definition

class DeleteWorkloadEstimateRequestRequestTypeDef(TypedDict):
    identifier: str,
```

## ExpressionFilterOutputTypeDef

```python
# ExpressionFilterOutputTypeDef definition

class ExpressionFilterOutputTypeDef(TypedDict):
    key: NotRequired[str],
    matchOptions: NotRequired[List[str]],
    values: NotRequired[List[str]],
```

## ExpressionFilterTypeDef

```python
# ExpressionFilterTypeDef definition

class ExpressionFilterTypeDef(TypedDict):
    key: NotRequired[str],
    matchOptions: NotRequired[Sequence[str]],
    values: NotRequired[Sequence[str]],
```

## GetBillEstimateRequestRequestTypeDef

```python
# GetBillEstimateRequestRequestTypeDef definition

class GetBillEstimateRequestRequestTypeDef(TypedDict):
    identifier: str,
```

## GetBillScenarioRequestRequestTypeDef

```python
# GetBillScenarioRequestRequestTypeDef definition

class GetBillScenarioRequestRequestTypeDef(TypedDict):
    identifier: str,
```

## GetWorkloadEstimateRequestRequestTypeDef

```python
# GetWorkloadEstimateRequestRequestTypeDef definition

class GetWorkloadEstimateRequestRequestTypeDef(TypedDict):
    identifier: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListBillEstimateCommitmentsRequestRequestTypeDef

```python
# ListBillEstimateCommitmentsRequestRequestTypeDef definition

class ListBillEstimateCommitmentsRequestRequestTypeDef(TypedDict):
    billEstimateId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListBillEstimateInputCommitmentModificationsRequestRequestTypeDef

```python
# ListBillEstimateInputCommitmentModificationsRequestRequestTypeDef definition

class ListBillEstimateInputCommitmentModificationsRequestRequestTypeDef(TypedDict):
    billEstimateId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListUsageFilterTypeDef

```python
# ListUsageFilterTypeDef definition

class ListUsageFilterTypeDef(TypedDict):
    name: ListUsageFilterNameType,  # (1)
    values: Sequence[str],
    matchOption: NotRequired[MatchOptionType],  # (2)
```

1. See [:material-code-brackets: ListUsageFilterNameType](./literals.md#listusagefilternametype) 
2. See [:material-code-brackets: MatchOptionType](./literals.md#matchoptiontype) 
## ListBillEstimateLineItemsFilterTypeDef

```python
# ListBillEstimateLineItemsFilterTypeDef definition

class ListBillEstimateLineItemsFilterTypeDef(TypedDict):
    name: ListBillEstimateLineItemsFilterNameType,  # (1)
    values: Sequence[str],
    matchOption: NotRequired[MatchOptionType],  # (2)
```

1. See [:material-code-brackets: ListBillEstimateLineItemsFilterNameType](./literals.md#listbillestimatelineitemsfilternametype) 
2. See [:material-code-brackets: MatchOptionType](./literals.md#matchoptiontype) 
## ListBillEstimatesFilterTypeDef

```python
# ListBillEstimatesFilterTypeDef definition

class ListBillEstimatesFilterTypeDef(TypedDict):
    name: ListBillEstimatesFilterNameType,  # (1)
    values: Sequence[str],
    matchOption: NotRequired[MatchOptionType],  # (2)
```

1. See [:material-code-brackets: ListBillEstimatesFilterNameType](./literals.md#listbillestimatesfilternametype) 
2. See [:material-code-brackets: MatchOptionType](./literals.md#matchoptiontype) 
## ListBillScenarioCommitmentModificationsRequestRequestTypeDef

```python
# ListBillScenarioCommitmentModificationsRequestRequestTypeDef definition

class ListBillScenarioCommitmentModificationsRequestRequestTypeDef(TypedDict):
    billScenarioId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListBillScenariosFilterTypeDef

```python
# ListBillScenariosFilterTypeDef definition

class ListBillScenariosFilterTypeDef(TypedDict):
    name: ListBillScenariosFilterNameType,  # (1)
    values: Sequence[str],
    matchOption: NotRequired[MatchOptionType],  # (2)
```

1. See [:material-code-brackets: ListBillScenariosFilterNameType](./literals.md#listbillscenariosfilternametype) 
2. See [:material-code-brackets: MatchOptionType](./literals.md#matchoptiontype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    arn: str,
```

## ListWorkloadEstimatesFilterTypeDef

```python
# ListWorkloadEstimatesFilterTypeDef definition

class ListWorkloadEstimatesFilterTypeDef(TypedDict):
    name: ListWorkloadEstimatesFilterNameType,  # (1)
    values: Sequence[str],
    matchOption: NotRequired[MatchOptionType],  # (2)
```

1. See [:material-code-brackets: ListWorkloadEstimatesFilterNameType](./literals.md#listworkloadestimatesfilternametype) 
2. See [:material-code-brackets: MatchOptionType](./literals.md#matchoptiontype) 
## WorkloadEstimateSummaryTypeDef

```python
# WorkloadEstimateSummaryTypeDef definition

class WorkloadEstimateSummaryTypeDef(TypedDict):
    id: str,
    name: NotRequired[str],
    createdAt: NotRequired[datetime],
    expiresAt: NotRequired[datetime],
    rateType: NotRequired[WorkloadEstimateRateTypeType],  # (1)
    rateTimestamp: NotRequired[datetime],
    status: NotRequired[WorkloadEstimateStatusType],  # (2)
    totalCost: NotRequired[float],
    costCurrency: NotRequired[CurrencyCodeType],  # (3)
    failureMessage: NotRequired[str],
```

1. See [:material-code-brackets: WorkloadEstimateRateTypeType](./literals.md#workloadestimateratetypetype) 
2. See [:material-code-brackets: WorkloadEstimateStatusType](./literals.md#workloadestimatestatustype) 
3. See [:material-code-brackets: CurrencyCodeType](./literals.md#currencycodetype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    arn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    arn: str,
    tagKeys: Sequence[str],
```

## UpdatePreferencesRequestRequestTypeDef

```python
# UpdatePreferencesRequestRequestTypeDef definition

class UpdatePreferencesRequestRequestTypeDef(TypedDict):
    managementAccountRateTypeSelections: NotRequired[Sequence[RateTypeType]],  # (1)
    memberAccountRateTypeSelections: NotRequired[Sequence[RateTypeType]],  # (1)
```

1. See [:material-code-brackets: RateTypeType](./literals.md#ratetypetype) 
2. See [:material-code-brackets: RateTypeType](./literals.md#ratetypetype) 
## CreateWorkloadEstimateResponseTypeDef

```python
# CreateWorkloadEstimateResponseTypeDef definition

class CreateWorkloadEstimateResponseTypeDef(TypedDict):
    id: str,
    name: str,
    createdAt: datetime,
    expiresAt: datetime,
    rateType: WorkloadEstimateRateTypeType,  # (1)
    rateTimestamp: datetime,
    status: WorkloadEstimateStatusType,  # (2)
    totalCost: float,
    costCurrency: CurrencyCodeType,  # (3)
    failureMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: WorkloadEstimateRateTypeType](./literals.md#workloadestimateratetypetype) 
2. See [:material-code-brackets: WorkloadEstimateStatusType](./literals.md#workloadestimatestatustype) 
3. See [:material-code-brackets: CurrencyCodeType](./literals.md#currencycodetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPreferencesResponseTypeDef

```python
# GetPreferencesResponseTypeDef definition

class GetPreferencesResponseTypeDef(TypedDict):
    managementAccountRateTypeSelections: List[RateTypeType],  # (1)
    memberAccountRateTypeSelections: List[RateTypeType],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: RateTypeType](./literals.md#ratetypetype) 
2. See [:material-code-brackets: RateTypeType](./literals.md#ratetypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWorkloadEstimateResponseTypeDef

```python
# GetWorkloadEstimateResponseTypeDef definition

class GetWorkloadEstimateResponseTypeDef(TypedDict):
    id: str,
    name: str,
    createdAt: datetime,
    expiresAt: datetime,
    rateType: WorkloadEstimateRateTypeType,  # (1)
    rateTimestamp: datetime,
    status: WorkloadEstimateStatusType,  # (2)
    totalCost: float,
    costCurrency: CurrencyCodeType,  # (3)
    failureMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: WorkloadEstimateRateTypeType](./literals.md#workloadestimateratetypetype) 
2. See [:material-code-brackets: WorkloadEstimateStatusType](./literals.md#workloadestimatestatustype) 
3. See [:material-code-brackets: CurrencyCodeType](./literals.md#currencycodetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePreferencesResponseTypeDef

```python
# UpdatePreferencesResponseTypeDef definition

class UpdatePreferencesResponseTypeDef(TypedDict):
    managementAccountRateTypeSelections: List[RateTypeType],  # (1)
    memberAccountRateTypeSelections: List[RateTypeType],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: RateTypeType](./literals.md#ratetypetype) 
2. See [:material-code-brackets: RateTypeType](./literals.md#ratetypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorkloadEstimateResponseTypeDef

```python
# UpdateWorkloadEstimateResponseTypeDef definition

class UpdateWorkloadEstimateResponseTypeDef(TypedDict):
    id: str,
    name: str,
    createdAt: datetime,
    expiresAt: datetime,
    rateType: WorkloadEstimateRateTypeType,  # (1)
    rateTimestamp: datetime,
    status: WorkloadEstimateStatusType,  # (2)
    totalCost: float,
    costCurrency: CurrencyCodeType,  # (3)
    failureMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: WorkloadEstimateRateTypeType](./literals.md#workloadestimateratetypetype) 
2. See [:material-code-brackets: WorkloadEstimateStatusType](./literals.md#workloadestimatestatustype) 
3. See [:material-code-brackets: CurrencyCodeType](./literals.md#currencycodetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteBillScenarioCommitmentModificationResponseTypeDef

```python
# BatchDeleteBillScenarioCommitmentModificationResponseTypeDef definition

class BatchDeleteBillScenarioCommitmentModificationResponseTypeDef(TypedDict):
    errors: List[BatchDeleteBillScenarioCommitmentModificationErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchDeleteBillScenarioCommitmentModificationErrorTypeDef](./type_defs.md#batchdeletebillscenariocommitmentmodificationerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteBillScenarioUsageModificationResponseTypeDef

```python
# BatchDeleteBillScenarioUsageModificationResponseTypeDef definition

class BatchDeleteBillScenarioUsageModificationResponseTypeDef(TypedDict):
    errors: List[BatchDeleteBillScenarioUsageModificationErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchDeleteBillScenarioUsageModificationErrorTypeDef](./type_defs.md#batchdeletebillscenariousagemodificationerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteWorkloadEstimateUsageResponseTypeDef

```python
# BatchDeleteWorkloadEstimateUsageResponseTypeDef definition

class BatchDeleteWorkloadEstimateUsageResponseTypeDef(TypedDict):
    errors: List[BatchDeleteWorkloadEstimateUsageErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchDeleteWorkloadEstimateUsageErrorTypeDef](./type_defs.md#batchdeleteworkloadestimateusageerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateBillScenarioCommitmentModificationRequestRequestTypeDef

```python
# BatchUpdateBillScenarioCommitmentModificationRequestRequestTypeDef definition

class BatchUpdateBillScenarioCommitmentModificationRequestRequestTypeDef(TypedDict):
    billScenarioId: str,
    commitmentModifications: Sequence[BatchUpdateBillScenarioCommitmentModificationEntryTypeDef],  # (1)
```

1. See [:material-code-braces: BatchUpdateBillScenarioCommitmentModificationEntryTypeDef](./type_defs.md#batchupdatebillscenariocommitmentmodificationentrytypedef) 
## BatchUpdateWorkloadEstimateUsageRequestRequestTypeDef

```python
# BatchUpdateWorkloadEstimateUsageRequestRequestTypeDef definition

class BatchUpdateWorkloadEstimateUsageRequestRequestTypeDef(TypedDict):
    workloadEstimateId: str,
    usage: Sequence[BatchUpdateWorkloadEstimateUsageEntryTypeDef],  # (1)
```

1. See [:material-code-braces: BatchUpdateWorkloadEstimateUsageEntryTypeDef](./type_defs.md#batchupdateworkloadestimateusageentrytypedef) 
## BillEstimateCommitmentSummaryTypeDef

```python
# BillEstimateCommitmentSummaryTypeDef definition

class BillEstimateCommitmentSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    purchaseAgreementType: NotRequired[PurchaseAgreementTypeType],  # (1)
    offeringId: NotRequired[str],
    usageAccountId: NotRequired[str],
    region: NotRequired[str],
    termLength: NotRequired[str],
    paymentOption: NotRequired[str],
    upfrontPayment: NotRequired[CostAmountTypeDef],  # (2)
    monthlyPayment: NotRequired[CostAmountTypeDef],  # (2)
```

1. See [:material-code-brackets: PurchaseAgreementTypeType](./literals.md#purchaseagreementtypetype) 
2. See [:material-code-braces: CostAmountTypeDef](./type_defs.md#costamounttypedef) 
3. See [:material-code-braces: CostAmountTypeDef](./type_defs.md#costamounttypedef) 
## CostDifferenceTypeDef

```python
# CostDifferenceTypeDef definition

class CostDifferenceTypeDef(TypedDict):
    historicalCost: NotRequired[CostAmountTypeDef],  # (1)
    estimatedCost: NotRequired[CostAmountTypeDef],  # (1)
```

1. See [:material-code-braces: CostAmountTypeDef](./type_defs.md#costamounttypedef) 
2. See [:material-code-braces: CostAmountTypeDef](./type_defs.md#costamounttypedef) 
## BillEstimateLineItemSummaryTypeDef

```python
# BillEstimateLineItemSummaryTypeDef definition

class BillEstimateLineItemSummaryTypeDef(TypedDict):
    serviceCode: str,
    usageType: str,
    operation: str,
    location: NotRequired[str],
    availabilityZone: NotRequired[str],
    id: NotRequired[str],
    lineItemId: NotRequired[str],
    lineItemType: NotRequired[str],
    payerAccountId: NotRequired[str],
    usageAccountId: NotRequired[str],
    estimatedUsageQuantity: NotRequired[UsageQuantityResultTypeDef],  # (1)
    estimatedCost: NotRequired[CostAmountTypeDef],  # (2)
    historicalUsageQuantity: NotRequired[UsageQuantityResultTypeDef],  # (1)
    historicalCost: NotRequired[CostAmountTypeDef],  # (2)
    savingsPlanArns: NotRequired[List[str]],
```

1. See [:material-code-braces: UsageQuantityResultTypeDef](./type_defs.md#usagequantityresulttypedef) 
2. See [:material-code-braces: CostAmountTypeDef](./type_defs.md#costamounttypedef) 
3. See [:material-code-braces: UsageQuantityResultTypeDef](./type_defs.md#usagequantityresulttypedef) 
4. See [:material-code-braces: CostAmountTypeDef](./type_defs.md#costamounttypedef) 
## BillEstimateSummaryTypeDef

```python
# BillEstimateSummaryTypeDef definition

class BillEstimateSummaryTypeDef(TypedDict):
    id: str,
    name: NotRequired[str],
    status: NotRequired[BillEstimateStatusType],  # (1)
    billInterval: NotRequired[BillIntervalOutputTypeDef],  # (2)
    createdAt: NotRequired[datetime],
    expiresAt: NotRequired[datetime],
```

1. See [:material-code-brackets: BillEstimateStatusType](./literals.md#billestimatestatustype) 
2. See [:material-code-braces: BillIntervalOutputTypeDef](./type_defs.md#billintervaloutputtypedef) 
## BillScenarioSummaryTypeDef

```python
# BillScenarioSummaryTypeDef definition

class BillScenarioSummaryTypeDef(TypedDict):
    id: str,
    name: NotRequired[str],
    billInterval: NotRequired[BillIntervalOutputTypeDef],  # (1)
    status: NotRequired[BillScenarioStatusType],  # (2)
    createdAt: NotRequired[datetime],
    expiresAt: NotRequired[datetime],
    failureMessage: NotRequired[str],
```

1. See [:material-code-braces: BillIntervalOutputTypeDef](./type_defs.md#billintervaloutputtypedef) 
2. See [:material-code-brackets: BillScenarioStatusType](./literals.md#billscenariostatustype) 
## CreateBillScenarioResponseTypeDef

```python
# CreateBillScenarioResponseTypeDef definition

class CreateBillScenarioResponseTypeDef(TypedDict):
    id: str,
    name: str,
    billInterval: BillIntervalOutputTypeDef,  # (1)
    status: BillScenarioStatusType,  # (2)
    createdAt: datetime,
    expiresAt: datetime,
    failureMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BillIntervalOutputTypeDef](./type_defs.md#billintervaloutputtypedef) 
2. See [:material-code-brackets: BillScenarioStatusType](./literals.md#billscenariostatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBillScenarioResponseTypeDef

```python
# GetBillScenarioResponseTypeDef definition

class GetBillScenarioResponseTypeDef(TypedDict):
    id: str,
    name: str,
    billInterval: BillIntervalOutputTypeDef,  # (1)
    status: BillScenarioStatusType,  # (2)
    createdAt: datetime,
    expiresAt: datetime,
    failureMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BillIntervalOutputTypeDef](./type_defs.md#billintervaloutputtypedef) 
2. See [:material-code-brackets: BillScenarioStatusType](./literals.md#billscenariostatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBillScenarioResponseTypeDef

```python
# UpdateBillScenarioResponseTypeDef definition

class UpdateBillScenarioResponseTypeDef(TypedDict):
    id: str,
    name: str,
    billInterval: BillIntervalOutputTypeDef,  # (1)
    status: BillScenarioStatusType,  # (2)
    createdAt: datetime,
    expiresAt: datetime,
    failureMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BillIntervalOutputTypeDef](./type_defs.md#billintervaloutputtypedef) 
2. See [:material-code-brackets: BillScenarioStatusType](./literals.md#billscenariostatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BillIntervalTypeDef

```python
# BillIntervalTypeDef definition

class BillIntervalTypeDef(TypedDict):
    start: NotRequired[TimestampTypeDef],
    end: NotRequired[TimestampTypeDef],
```

## FilterTimestampTypeDef

```python
# FilterTimestampTypeDef definition

class FilterTimestampTypeDef(TypedDict):
    afterTimestamp: NotRequired[TimestampTypeDef],
    beforeTimestamp: NotRequired[TimestampTypeDef],
```

## UpdateBillEstimateRequestRequestTypeDef

```python
# UpdateBillEstimateRequestRequestTypeDef definition

class UpdateBillEstimateRequestRequestTypeDef(TypedDict):
    identifier: str,
    name: NotRequired[str],
    expiresAt: NotRequired[TimestampTypeDef],
```

## UpdateBillScenarioRequestRequestTypeDef

```python
# UpdateBillScenarioRequestRequestTypeDef definition

class UpdateBillScenarioRequestRequestTypeDef(TypedDict):
    identifier: str,
    name: NotRequired[str],
    expiresAt: NotRequired[TimestampTypeDef],
```

## UpdateWorkloadEstimateRequestRequestTypeDef

```python
# UpdateWorkloadEstimateRequestRequestTypeDef definition

class UpdateWorkloadEstimateRequestRequestTypeDef(TypedDict):
    identifier: str,
    name: NotRequired[str],
    expiresAt: NotRequired[TimestampTypeDef],
```

## UsageAmountTypeDef

```python
# UsageAmountTypeDef definition

class UsageAmountTypeDef(TypedDict):
    startHour: TimestampTypeDef,
    amount: float,
```

## BillScenarioCommitmentModificationActionTypeDef

```python
# BillScenarioCommitmentModificationActionTypeDef definition

class BillScenarioCommitmentModificationActionTypeDef(TypedDict):
    addReservedInstanceAction: NotRequired[AddReservedInstanceActionTypeDef],  # (1)
    addSavingsPlanAction: NotRequired[AddSavingsPlanActionTypeDef],  # (2)
    negateReservedInstanceAction: NotRequired[NegateReservedInstanceActionTypeDef],  # (3)
    negateSavingsPlanAction: NotRequired[NegateSavingsPlanActionTypeDef],  # (4)
```

1. See [:material-code-braces: AddReservedInstanceActionTypeDef](./type_defs.md#addreservedinstanceactiontypedef) 
2. See [:material-code-braces: AddSavingsPlanActionTypeDef](./type_defs.md#addsavingsplanactiontypedef) 
3. See [:material-code-braces: NegateReservedInstanceActionTypeDef](./type_defs.md#negatereservedinstanceactiontypedef) 
4. See [:material-code-braces: NegateSavingsPlanActionTypeDef](./type_defs.md#negatesavingsplanactiontypedef) 
## ExpressionOutputTypeDef

```python
# ExpressionOutputTypeDef definition

class ExpressionOutputTypeDef(TypedDict):
    and: NotRequired[List[Dict[str, Any]]],
    or: NotRequired[List[Dict[str, Any]]],
    not: NotRequired[Dict[str, Any]],
    costCategories: NotRequired[ExpressionFilterOutputTypeDef],  # (1)
    dimensions: NotRequired[ExpressionFilterOutputTypeDef],  # (1)
    tags: NotRequired[ExpressionFilterOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ExpressionFilterOutputTypeDef](./type_defs.md#expressionfilteroutputtypedef) 
2. See [:material-code-braces: ExpressionFilterOutputTypeDef](./type_defs.md#expressionfilteroutputtypedef) 
3. See [:material-code-braces: ExpressionFilterOutputTypeDef](./type_defs.md#expressionfilteroutputtypedef) 
## ExpressionPaginatorTypeDef

```python
# ExpressionPaginatorTypeDef definition

class ExpressionPaginatorTypeDef(TypedDict):
    and: NotRequired[List[Dict[str, Any]]],
    or: NotRequired[List[Dict[str, Any]]],
    not: NotRequired[Dict[str, Any]],
    costCategories: NotRequired[ExpressionFilterOutputTypeDef],  # (1)
    dimensions: NotRequired[ExpressionFilterOutputTypeDef],  # (1)
    tags: NotRequired[ExpressionFilterOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ExpressionFilterOutputTypeDef](./type_defs.md#expressionfilteroutputtypedef) 
2. See [:material-code-braces: ExpressionFilterOutputTypeDef](./type_defs.md#expressionfilteroutputtypedef) 
3. See [:material-code-braces: ExpressionFilterOutputTypeDef](./type_defs.md#expressionfilteroutputtypedef) 
## ListBillEstimateCommitmentsRequestPaginateTypeDef

```python
# ListBillEstimateCommitmentsRequestPaginateTypeDef definition

class ListBillEstimateCommitmentsRequestPaginateTypeDef(TypedDict):
    billEstimateId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBillEstimateInputCommitmentModificationsRequestPaginateTypeDef

```python
# ListBillEstimateInputCommitmentModificationsRequestPaginateTypeDef definition

class ListBillEstimateInputCommitmentModificationsRequestPaginateTypeDef(TypedDict):
    billEstimateId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBillScenarioCommitmentModificationsRequestPaginateTypeDef

```python
# ListBillScenarioCommitmentModificationsRequestPaginateTypeDef definition

class ListBillScenarioCommitmentModificationsRequestPaginateTypeDef(TypedDict):
    billScenarioId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBillEstimateInputUsageModificationsRequestPaginateTypeDef

```python
# ListBillEstimateInputUsageModificationsRequestPaginateTypeDef definition

class ListBillEstimateInputUsageModificationsRequestPaginateTypeDef(TypedDict):
    billEstimateId: str,
    filters: NotRequired[Sequence[ListUsageFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListUsageFilterTypeDef](./type_defs.md#listusagefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBillEstimateInputUsageModificationsRequestRequestTypeDef

```python
# ListBillEstimateInputUsageModificationsRequestRequestTypeDef definition

class ListBillEstimateInputUsageModificationsRequestRequestTypeDef(TypedDict):
    billEstimateId: str,
    filters: NotRequired[Sequence[ListUsageFilterTypeDef]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: ListUsageFilterTypeDef](./type_defs.md#listusagefiltertypedef) 
## ListBillScenarioUsageModificationsRequestPaginateTypeDef

```python
# ListBillScenarioUsageModificationsRequestPaginateTypeDef definition

class ListBillScenarioUsageModificationsRequestPaginateTypeDef(TypedDict):
    billScenarioId: str,
    filters: NotRequired[Sequence[ListUsageFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListUsageFilterTypeDef](./type_defs.md#listusagefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBillScenarioUsageModificationsRequestRequestTypeDef

```python
# ListBillScenarioUsageModificationsRequestRequestTypeDef definition

class ListBillScenarioUsageModificationsRequestRequestTypeDef(TypedDict):
    billScenarioId: str,
    filters: NotRequired[Sequence[ListUsageFilterTypeDef]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: ListUsageFilterTypeDef](./type_defs.md#listusagefiltertypedef) 
## ListWorkloadEstimateUsageRequestPaginateTypeDef

```python
# ListWorkloadEstimateUsageRequestPaginateTypeDef definition

class ListWorkloadEstimateUsageRequestPaginateTypeDef(TypedDict):
    workloadEstimateId: str,
    filters: NotRequired[Sequence[ListUsageFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListUsageFilterTypeDef](./type_defs.md#listusagefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkloadEstimateUsageRequestRequestTypeDef

```python
# ListWorkloadEstimateUsageRequestRequestTypeDef definition

class ListWorkloadEstimateUsageRequestRequestTypeDef(TypedDict):
    workloadEstimateId: str,
    filters: NotRequired[Sequence[ListUsageFilterTypeDef]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: ListUsageFilterTypeDef](./type_defs.md#listusagefiltertypedef) 
## ListBillEstimateLineItemsRequestPaginateTypeDef

```python
# ListBillEstimateLineItemsRequestPaginateTypeDef definition

class ListBillEstimateLineItemsRequestPaginateTypeDef(TypedDict):
    billEstimateId: str,
    filters: NotRequired[Sequence[ListBillEstimateLineItemsFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListBillEstimateLineItemsFilterTypeDef](./type_defs.md#listbillestimatelineitemsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBillEstimateLineItemsRequestRequestTypeDef

```python
# ListBillEstimateLineItemsRequestRequestTypeDef definition

class ListBillEstimateLineItemsRequestRequestTypeDef(TypedDict):
    billEstimateId: str,
    filters: NotRequired[Sequence[ListBillEstimateLineItemsFilterTypeDef]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: ListBillEstimateLineItemsFilterTypeDef](./type_defs.md#listbillestimatelineitemsfiltertypedef) 
## ListWorkloadEstimatesResponseTypeDef

```python
# ListWorkloadEstimatesResponseTypeDef definition

class ListWorkloadEstimatesResponseTypeDef(TypedDict):
    items: List[WorkloadEstimateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkloadEstimateSummaryTypeDef](./type_defs.md#workloadestimatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBillEstimateCommitmentsResponseTypeDef

```python
# ListBillEstimateCommitmentsResponseTypeDef definition

class ListBillEstimateCommitmentsResponseTypeDef(TypedDict):
    items: List[BillEstimateCommitmentSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BillEstimateCommitmentSummaryTypeDef](./type_defs.md#billestimatecommitmentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BillEstimateCostSummaryTypeDef

```python
# BillEstimateCostSummaryTypeDef definition

class BillEstimateCostSummaryTypeDef(TypedDict):
    totalCostDifference: NotRequired[CostDifferenceTypeDef],  # (1)
    serviceCostDifferences: NotRequired[Dict[str, CostDifferenceTypeDef]],  # (2)
```

1. See [:material-code-braces: CostDifferenceTypeDef](./type_defs.md#costdifferencetypedef) 
2. See [:material-code-braces: CostDifferenceTypeDef](./type_defs.md#costdifferencetypedef) 
## ListBillEstimateLineItemsResponseTypeDef

```python
# ListBillEstimateLineItemsResponseTypeDef definition

class ListBillEstimateLineItemsResponseTypeDef(TypedDict):
    items: List[BillEstimateLineItemSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BillEstimateLineItemSummaryTypeDef](./type_defs.md#billestimatelineitemsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBillEstimatesResponseTypeDef

```python
# ListBillEstimatesResponseTypeDef definition

class ListBillEstimatesResponseTypeDef(TypedDict):
    items: List[BillEstimateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BillEstimateSummaryTypeDef](./type_defs.md#billestimatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBillScenariosResponseTypeDef

```python
# ListBillScenariosResponseTypeDef definition

class ListBillScenariosResponseTypeDef(TypedDict):
    items: List[BillScenarioSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BillScenarioSummaryTypeDef](./type_defs.md#billscenariosummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBillEstimatesRequestPaginateTypeDef

```python
# ListBillEstimatesRequestPaginateTypeDef definition

class ListBillEstimatesRequestPaginateTypeDef(TypedDict):
    filters: NotRequired[Sequence[ListBillEstimatesFilterTypeDef]],  # (1)
    createdAtFilter: NotRequired[FilterTimestampTypeDef],  # (2)
    expiresAtFilter: NotRequired[FilterTimestampTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: ListBillEstimatesFilterTypeDef](./type_defs.md#listbillestimatesfiltertypedef) 
2. See [:material-code-braces: FilterTimestampTypeDef](./type_defs.md#filtertimestamptypedef) 
3. See [:material-code-braces: FilterTimestampTypeDef](./type_defs.md#filtertimestamptypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBillEstimatesRequestRequestTypeDef

```python
# ListBillEstimatesRequestRequestTypeDef definition

class ListBillEstimatesRequestRequestTypeDef(TypedDict):
    filters: NotRequired[Sequence[ListBillEstimatesFilterTypeDef]],  # (1)
    createdAtFilter: NotRequired[FilterTimestampTypeDef],  # (2)
    expiresAtFilter: NotRequired[FilterTimestampTypeDef],  # (2)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: ListBillEstimatesFilterTypeDef](./type_defs.md#listbillestimatesfiltertypedef) 
2. See [:material-code-braces: FilterTimestampTypeDef](./type_defs.md#filtertimestamptypedef) 
3. See [:material-code-braces: FilterTimestampTypeDef](./type_defs.md#filtertimestamptypedef) 
## ListBillScenariosRequestPaginateTypeDef

```python
# ListBillScenariosRequestPaginateTypeDef definition

class ListBillScenariosRequestPaginateTypeDef(TypedDict):
    filters: NotRequired[Sequence[ListBillScenariosFilterTypeDef]],  # (1)
    createdAtFilter: NotRequired[FilterTimestampTypeDef],  # (2)
    expiresAtFilter: NotRequired[FilterTimestampTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: ListBillScenariosFilterTypeDef](./type_defs.md#listbillscenariosfiltertypedef) 
2. See [:material-code-braces: FilterTimestampTypeDef](./type_defs.md#filtertimestamptypedef) 
3. See [:material-code-braces: FilterTimestampTypeDef](./type_defs.md#filtertimestamptypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBillScenariosRequestRequestTypeDef

```python
# ListBillScenariosRequestRequestTypeDef definition

class ListBillScenariosRequestRequestTypeDef(TypedDict):
    filters: NotRequired[Sequence[ListBillScenariosFilterTypeDef]],  # (1)
    createdAtFilter: NotRequired[FilterTimestampTypeDef],  # (2)
    expiresAtFilter: NotRequired[FilterTimestampTypeDef],  # (2)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: ListBillScenariosFilterTypeDef](./type_defs.md#listbillscenariosfiltertypedef) 
2. See [:material-code-braces: FilterTimestampTypeDef](./type_defs.md#filtertimestamptypedef) 
3. See [:material-code-braces: FilterTimestampTypeDef](./type_defs.md#filtertimestamptypedef) 
## ListWorkloadEstimatesRequestPaginateTypeDef

```python
# ListWorkloadEstimatesRequestPaginateTypeDef definition

class ListWorkloadEstimatesRequestPaginateTypeDef(TypedDict):
    createdAtFilter: NotRequired[FilterTimestampTypeDef],  # (1)
    expiresAtFilter: NotRequired[FilterTimestampTypeDef],  # (1)
    filters: NotRequired[Sequence[ListWorkloadEstimatesFilterTypeDef]],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: FilterTimestampTypeDef](./type_defs.md#filtertimestamptypedef) 
2. See [:material-code-braces: FilterTimestampTypeDef](./type_defs.md#filtertimestamptypedef) 
3. See [:material-code-braces: ListWorkloadEstimatesFilterTypeDef](./type_defs.md#listworkloadestimatesfiltertypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkloadEstimatesRequestRequestTypeDef

```python
# ListWorkloadEstimatesRequestRequestTypeDef definition

class ListWorkloadEstimatesRequestRequestTypeDef(TypedDict):
    createdAtFilter: NotRequired[FilterTimestampTypeDef],  # (1)
    expiresAtFilter: NotRequired[FilterTimestampTypeDef],  # (1)
    filters: NotRequired[Sequence[ListWorkloadEstimatesFilterTypeDef]],  # (3)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: FilterTimestampTypeDef](./type_defs.md#filtertimestamptypedef) 
2. See [:material-code-braces: FilterTimestampTypeDef](./type_defs.md#filtertimestamptypedef) 
3. See [:material-code-braces: ListWorkloadEstimatesFilterTypeDef](./type_defs.md#listworkloadestimatesfiltertypedef) 
## BatchUpdateBillScenarioUsageModificationEntryTypeDef

```python
# BatchUpdateBillScenarioUsageModificationEntryTypeDef definition

class BatchUpdateBillScenarioUsageModificationEntryTypeDef(TypedDict):
    id: str,
    group: NotRequired[str],
    amounts: NotRequired[Sequence[UsageAmountTypeDef]],  # (1)
```

1. See [:material-code-braces: UsageAmountTypeDef](./type_defs.md#usageamounttypedef) 
## BatchCreateBillScenarioCommitmentModificationEntryTypeDef

```python
# BatchCreateBillScenarioCommitmentModificationEntryTypeDef definition

class BatchCreateBillScenarioCommitmentModificationEntryTypeDef(TypedDict):
    key: str,
    usageAccountId: str,
    commitmentAction: BillScenarioCommitmentModificationActionTypeDef,  # (1)
    group: NotRequired[str],
```

1. See [:material-code-braces: BillScenarioCommitmentModificationActionTypeDef](./type_defs.md#billscenariocommitmentmodificationactiontypedef) 
## BatchCreateBillScenarioCommitmentModificationItemTypeDef

```python
# BatchCreateBillScenarioCommitmentModificationItemTypeDef definition

class BatchCreateBillScenarioCommitmentModificationItemTypeDef(TypedDict):
    key: NotRequired[str],
    id: NotRequired[str],
    group: NotRequired[str],
    usageAccountId: NotRequired[str],
    commitmentAction: NotRequired[BillScenarioCommitmentModificationActionTypeDef],  # (1)
```

1. See [:material-code-braces: BillScenarioCommitmentModificationActionTypeDef](./type_defs.md#billscenariocommitmentmodificationactiontypedef) 
## BillEstimateInputCommitmentModificationSummaryTypeDef

```python
# BillEstimateInputCommitmentModificationSummaryTypeDef definition

class BillEstimateInputCommitmentModificationSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    group: NotRequired[str],
    usageAccountId: NotRequired[str],
    commitmentAction: NotRequired[BillScenarioCommitmentModificationActionTypeDef],  # (1)
```

1. See [:material-code-braces: BillScenarioCommitmentModificationActionTypeDef](./type_defs.md#billscenariocommitmentmodificationactiontypedef) 
## BillScenarioCommitmentModificationItemTypeDef

```python
# BillScenarioCommitmentModificationItemTypeDef definition

class BillScenarioCommitmentModificationItemTypeDef(TypedDict):
    id: NotRequired[str],
    usageAccountId: NotRequired[str],
    group: NotRequired[str],
    commitmentAction: NotRequired[BillScenarioCommitmentModificationActionTypeDef],  # (1)
```

1. See [:material-code-braces: BillScenarioCommitmentModificationActionTypeDef](./type_defs.md#billscenariocommitmentmodificationactiontypedef) 
## HistoricalUsageEntityOutputTypeDef

```python
# HistoricalUsageEntityOutputTypeDef definition

class HistoricalUsageEntityOutputTypeDef(TypedDict):
    serviceCode: str,
    usageType: str,
    operation: str,
    usageAccountId: str,
    billInterval: BillIntervalOutputTypeDef,  # (1)
    filterExpression: ExpressionOutputTypeDef,  # (2)
    location: NotRequired[str],
```

1. See [:material-code-braces: BillIntervalOutputTypeDef](./type_defs.md#billintervaloutputtypedef) 
2. See [:material-code-braces: ExpressionOutputTypeDef](./type_defs.md#expressionoutputtypedef) 
## HistoricalUsageEntityPaginatorTypeDef

```python
# HistoricalUsageEntityPaginatorTypeDef definition

class HistoricalUsageEntityPaginatorTypeDef(TypedDict):
    serviceCode: str,
    usageType: str,
    operation: str,
    usageAccountId: str,
    billInterval: BillIntervalOutputTypeDef,  # (1)
    filterExpression: ExpressionPaginatorTypeDef,  # (2)
    location: NotRequired[str],
```

1. See [:material-code-braces: BillIntervalOutputTypeDef](./type_defs.md#billintervaloutputtypedef) 
2. See [:material-code-braces: ExpressionPaginatorTypeDef](./type_defs.md#expressionpaginatortypedef) 
## ExpressionTypeDef

```python
# ExpressionTypeDef definition

class ExpressionTypeDef(TypedDict):
    and: NotRequired[Sequence[Mapping[str, Any]]],
    or: NotRequired[Sequence[Mapping[str, Any]]],
    not: NotRequired[Mapping[str, Any]],
    costCategories: NotRequired[ExpressionFilterUnionTypeDef],  # (1)
    dimensions: NotRequired[ExpressionFilterUnionTypeDef],  # (1)
    tags: NotRequired[ExpressionFilterUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ExpressionFilterTypeDef](./type_defs.md#expressionfiltertypedef) [:material-code-braces: ExpressionFilterOutputTypeDef](./type_defs.md#expressionfilteroutputtypedef) 
2. See [:material-code-braces: ExpressionFilterTypeDef](./type_defs.md#expressionfiltertypedef) [:material-code-braces: ExpressionFilterOutputTypeDef](./type_defs.md#expressionfilteroutputtypedef) 
3. See [:material-code-braces: ExpressionFilterTypeDef](./type_defs.md#expressionfiltertypedef) [:material-code-braces: ExpressionFilterOutputTypeDef](./type_defs.md#expressionfilteroutputtypedef) 
## CreateBillEstimateResponseTypeDef

```python
# CreateBillEstimateResponseTypeDef definition

class CreateBillEstimateResponseTypeDef(TypedDict):
    id: str,
    name: str,
    status: BillEstimateStatusType,  # (1)
    failureMessage: str,
    billInterval: BillIntervalOutputTypeDef,  # (2)
    costSummary: BillEstimateCostSummaryTypeDef,  # (3)
    createdAt: datetime,
    expiresAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: BillEstimateStatusType](./literals.md#billestimatestatustype) 
2. See [:material-code-braces: BillIntervalOutputTypeDef](./type_defs.md#billintervaloutputtypedef) 
3. See [:material-code-braces: BillEstimateCostSummaryTypeDef](./type_defs.md#billestimatecostsummarytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBillEstimateResponseTypeDef

```python
# GetBillEstimateResponseTypeDef definition

class GetBillEstimateResponseTypeDef(TypedDict):
    id: str,
    name: str,
    status: BillEstimateStatusType,  # (1)
    failureMessage: str,
    billInterval: BillIntervalOutputTypeDef,  # (2)
    costSummary: BillEstimateCostSummaryTypeDef,  # (3)
    createdAt: datetime,
    expiresAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: BillEstimateStatusType](./literals.md#billestimatestatustype) 
2. See [:material-code-braces: BillIntervalOutputTypeDef](./type_defs.md#billintervaloutputtypedef) 
3. See [:material-code-braces: BillEstimateCostSummaryTypeDef](./type_defs.md#billestimatecostsummarytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBillEstimateResponseTypeDef

```python
# UpdateBillEstimateResponseTypeDef definition

class UpdateBillEstimateResponseTypeDef(TypedDict):
    id: str,
    name: str,
    status: BillEstimateStatusType,  # (1)
    failureMessage: str,
    billInterval: BillIntervalOutputTypeDef,  # (2)
    costSummary: BillEstimateCostSummaryTypeDef,  # (3)
    createdAt: datetime,
    expiresAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: BillEstimateStatusType](./literals.md#billestimatestatustype) 
2. See [:material-code-braces: BillIntervalOutputTypeDef](./type_defs.md#billintervaloutputtypedef) 
3. See [:material-code-braces: BillEstimateCostSummaryTypeDef](./type_defs.md#billestimatecostsummarytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateBillScenarioUsageModificationRequestRequestTypeDef

```python
# BatchUpdateBillScenarioUsageModificationRequestRequestTypeDef definition

class BatchUpdateBillScenarioUsageModificationRequestRequestTypeDef(TypedDict):
    billScenarioId: str,
    usageModifications: Sequence[BatchUpdateBillScenarioUsageModificationEntryTypeDef],  # (1)
```

1. See [:material-code-braces: BatchUpdateBillScenarioUsageModificationEntryTypeDef](./type_defs.md#batchupdatebillscenariousagemodificationentrytypedef) 
## BatchCreateBillScenarioCommitmentModificationRequestRequestTypeDef

```python
# BatchCreateBillScenarioCommitmentModificationRequestRequestTypeDef definition

class BatchCreateBillScenarioCommitmentModificationRequestRequestTypeDef(TypedDict):
    billScenarioId: str,
    commitmentModifications: Sequence[BatchCreateBillScenarioCommitmentModificationEntryTypeDef],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: BatchCreateBillScenarioCommitmentModificationEntryTypeDef](./type_defs.md#batchcreatebillscenariocommitmentmodificationentrytypedef) 
## BatchCreateBillScenarioCommitmentModificationResponseTypeDef

```python
# BatchCreateBillScenarioCommitmentModificationResponseTypeDef definition

class BatchCreateBillScenarioCommitmentModificationResponseTypeDef(TypedDict):
    items: List[BatchCreateBillScenarioCommitmentModificationItemTypeDef],  # (1)
    errors: List[BatchCreateBillScenarioCommitmentModificationErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchCreateBillScenarioCommitmentModificationItemTypeDef](./type_defs.md#batchcreatebillscenariocommitmentmodificationitemtypedef) 
2. See [:material-code-braces: BatchCreateBillScenarioCommitmentModificationErrorTypeDef](./type_defs.md#batchcreatebillscenariocommitmentmodificationerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBillEstimateInputCommitmentModificationsResponseTypeDef

```python
# ListBillEstimateInputCommitmentModificationsResponseTypeDef definition

class ListBillEstimateInputCommitmentModificationsResponseTypeDef(TypedDict):
    items: List[BillEstimateInputCommitmentModificationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BillEstimateInputCommitmentModificationSummaryTypeDef](./type_defs.md#billestimateinputcommitmentmodificationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateBillScenarioCommitmentModificationResponseTypeDef

```python
# BatchUpdateBillScenarioCommitmentModificationResponseTypeDef definition

class BatchUpdateBillScenarioCommitmentModificationResponseTypeDef(TypedDict):
    items: List[BillScenarioCommitmentModificationItemTypeDef],  # (1)
    errors: List[BatchUpdateBillScenarioCommitmentModificationErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BillScenarioCommitmentModificationItemTypeDef](./type_defs.md#billscenariocommitmentmodificationitemtypedef) 
2. See [:material-code-braces: BatchUpdateBillScenarioCommitmentModificationErrorTypeDef](./type_defs.md#batchupdatebillscenariocommitmentmodificationerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBillScenarioCommitmentModificationsResponseTypeDef

```python
# ListBillScenarioCommitmentModificationsResponseTypeDef definition

class ListBillScenarioCommitmentModificationsResponseTypeDef(TypedDict):
    items: List[BillScenarioCommitmentModificationItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BillScenarioCommitmentModificationItemTypeDef](./type_defs.md#billscenariocommitmentmodificationitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchCreateBillScenarioUsageModificationItemTypeDef

```python
# BatchCreateBillScenarioUsageModificationItemTypeDef definition

class BatchCreateBillScenarioUsageModificationItemTypeDef(TypedDict):
    serviceCode: str,
    usageType: str,
    operation: str,
    location: NotRequired[str],
    availabilityZone: NotRequired[str],
    id: NotRequired[str],
    group: NotRequired[str],
    usageAccountId: NotRequired[str],
    quantities: NotRequired[List[UsageQuantityTypeDef]],  # (1)
    historicalUsage: NotRequired[HistoricalUsageEntityOutputTypeDef],  # (2)
    key: NotRequired[str],
```

1. See [:material-code-braces: UsageQuantityTypeDef](./type_defs.md#usagequantitytypedef) 
2. See [:material-code-braces: HistoricalUsageEntityOutputTypeDef](./type_defs.md#historicalusageentityoutputtypedef) 
## BatchCreateWorkloadEstimateUsageItemTypeDef

```python
# BatchCreateWorkloadEstimateUsageItemTypeDef definition

class BatchCreateWorkloadEstimateUsageItemTypeDef(TypedDict):
    serviceCode: str,
    usageType: str,
    operation: str,
    location: NotRequired[str],
    id: NotRequired[str],
    usageAccountId: NotRequired[str],
    group: NotRequired[str],
    quantity: NotRequired[WorkloadEstimateUsageQuantityTypeDef],  # (1)
    cost: NotRequired[float],
    currency: NotRequired[CurrencyCodeType],  # (2)
    status: NotRequired[WorkloadEstimateCostStatusType],  # (3)
    historicalUsage: NotRequired[HistoricalUsageEntityOutputTypeDef],  # (4)
    key: NotRequired[str],
```

1. See [:material-code-braces: WorkloadEstimateUsageQuantityTypeDef](./type_defs.md#workloadestimateusagequantitytypedef) 
2. See [:material-code-brackets: CurrencyCodeType](./literals.md#currencycodetype) 
3. See [:material-code-brackets: WorkloadEstimateCostStatusType](./literals.md#workloadestimatecoststatustype) 
4. See [:material-code-braces: HistoricalUsageEntityOutputTypeDef](./type_defs.md#historicalusageentityoutputtypedef) 
## BillEstimateInputUsageModificationSummaryTypeDef

```python
# BillEstimateInputUsageModificationSummaryTypeDef definition

class BillEstimateInputUsageModificationSummaryTypeDef(TypedDict):
    serviceCode: str,
    usageType: str,
    operation: str,
    location: NotRequired[str],
    availabilityZone: NotRequired[str],
    id: NotRequired[str],
    group: NotRequired[str],
    usageAccountId: NotRequired[str],
    quantities: NotRequired[List[UsageQuantityTypeDef]],  # (1)
    historicalUsage: NotRequired[HistoricalUsageEntityOutputTypeDef],  # (2)
```

1. See [:material-code-braces: UsageQuantityTypeDef](./type_defs.md#usagequantitytypedef) 
2. See [:material-code-braces: HistoricalUsageEntityOutputTypeDef](./type_defs.md#historicalusageentityoutputtypedef) 
## BillScenarioUsageModificationItemTypeDef

```python
# BillScenarioUsageModificationItemTypeDef definition

class BillScenarioUsageModificationItemTypeDef(TypedDict):
    serviceCode: str,
    usageType: str,
    operation: str,
    location: NotRequired[str],
    availabilityZone: NotRequired[str],
    id: NotRequired[str],
    group: NotRequired[str],
    usageAccountId: NotRequired[str],
    quantities: NotRequired[List[UsageQuantityTypeDef]],  # (1)
    historicalUsage: NotRequired[HistoricalUsageEntityOutputTypeDef],  # (2)
```

1. See [:material-code-braces: UsageQuantityTypeDef](./type_defs.md#usagequantitytypedef) 
2. See [:material-code-braces: HistoricalUsageEntityOutputTypeDef](./type_defs.md#historicalusageentityoutputtypedef) 
## WorkloadEstimateUsageItemTypeDef

```python
# WorkloadEstimateUsageItemTypeDef definition

class WorkloadEstimateUsageItemTypeDef(TypedDict):
    serviceCode: str,
    usageType: str,
    operation: str,
    location: NotRequired[str],
    id: NotRequired[str],
    usageAccountId: NotRequired[str],
    group: NotRequired[str],
    quantity: NotRequired[WorkloadEstimateUsageQuantityTypeDef],  # (1)
    cost: NotRequired[float],
    currency: NotRequired[CurrencyCodeType],  # (2)
    status: NotRequired[WorkloadEstimateCostStatusType],  # (3)
    historicalUsage: NotRequired[HistoricalUsageEntityOutputTypeDef],  # (4)
```

1. See [:material-code-braces: WorkloadEstimateUsageQuantityTypeDef](./type_defs.md#workloadestimateusagequantitytypedef) 
2. See [:material-code-brackets: CurrencyCodeType](./literals.md#currencycodetype) 
3. See [:material-code-brackets: WorkloadEstimateCostStatusType](./literals.md#workloadestimatecoststatustype) 
4. See [:material-code-braces: HistoricalUsageEntityOutputTypeDef](./type_defs.md#historicalusageentityoutputtypedef) 
## BillEstimateInputUsageModificationSummaryPaginatorTypeDef

```python
# BillEstimateInputUsageModificationSummaryPaginatorTypeDef definition

class BillEstimateInputUsageModificationSummaryPaginatorTypeDef(TypedDict):
    serviceCode: str,
    usageType: str,
    operation: str,
    location: NotRequired[str],
    availabilityZone: NotRequired[str],
    id: NotRequired[str],
    group: NotRequired[str],
    usageAccountId: NotRequired[str],
    quantities: NotRequired[List[UsageQuantityTypeDef]],  # (1)
    historicalUsage: NotRequired[HistoricalUsageEntityPaginatorTypeDef],  # (2)
```

1. See [:material-code-braces: UsageQuantityTypeDef](./type_defs.md#usagequantitytypedef) 
2. See [:material-code-braces: HistoricalUsageEntityPaginatorTypeDef](./type_defs.md#historicalusageentitypaginatortypedef) 
## BillScenarioUsageModificationItemPaginatorTypeDef

```python
# BillScenarioUsageModificationItemPaginatorTypeDef definition

class BillScenarioUsageModificationItemPaginatorTypeDef(TypedDict):
    serviceCode: str,
    usageType: str,
    operation: str,
    location: NotRequired[str],
    availabilityZone: NotRequired[str],
    id: NotRequired[str],
    group: NotRequired[str],
    usageAccountId: NotRequired[str],
    quantities: NotRequired[List[UsageQuantityTypeDef]],  # (1)
    historicalUsage: NotRequired[HistoricalUsageEntityPaginatorTypeDef],  # (2)
```

1. See [:material-code-braces: UsageQuantityTypeDef](./type_defs.md#usagequantitytypedef) 
2. See [:material-code-braces: HistoricalUsageEntityPaginatorTypeDef](./type_defs.md#historicalusageentitypaginatortypedef) 
## WorkloadEstimateUsageItemPaginatorTypeDef

```python
# WorkloadEstimateUsageItemPaginatorTypeDef definition

class WorkloadEstimateUsageItemPaginatorTypeDef(TypedDict):
    serviceCode: str,
    usageType: str,
    operation: str,
    location: NotRequired[str],
    id: NotRequired[str],
    usageAccountId: NotRequired[str],
    group: NotRequired[str],
    quantity: NotRequired[WorkloadEstimateUsageQuantityTypeDef],  # (1)
    cost: NotRequired[float],
    currency: NotRequired[CurrencyCodeType],  # (2)
    status: NotRequired[WorkloadEstimateCostStatusType],  # (3)
    historicalUsage: NotRequired[HistoricalUsageEntityPaginatorTypeDef],  # (4)
```

1. See [:material-code-braces: WorkloadEstimateUsageQuantityTypeDef](./type_defs.md#workloadestimateusagequantitytypedef) 
2. See [:material-code-brackets: CurrencyCodeType](./literals.md#currencycodetype) 
3. See [:material-code-brackets: WorkloadEstimateCostStatusType](./literals.md#workloadestimatecoststatustype) 
4. See [:material-code-braces: HistoricalUsageEntityPaginatorTypeDef](./type_defs.md#historicalusageentitypaginatortypedef) 
## BatchCreateBillScenarioUsageModificationResponseTypeDef

```python
# BatchCreateBillScenarioUsageModificationResponseTypeDef definition

class BatchCreateBillScenarioUsageModificationResponseTypeDef(TypedDict):
    items: List[BatchCreateBillScenarioUsageModificationItemTypeDef],  # (1)
    errors: List[BatchCreateBillScenarioUsageModificationErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchCreateBillScenarioUsageModificationItemTypeDef](./type_defs.md#batchcreatebillscenariousagemodificationitemtypedef) 
2. See [:material-code-braces: BatchCreateBillScenarioUsageModificationErrorTypeDef](./type_defs.md#batchcreatebillscenariousagemodificationerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchCreateWorkloadEstimateUsageResponseTypeDef

```python
# BatchCreateWorkloadEstimateUsageResponseTypeDef definition

class BatchCreateWorkloadEstimateUsageResponseTypeDef(TypedDict):
    items: List[BatchCreateWorkloadEstimateUsageItemTypeDef],  # (1)
    errors: List[BatchCreateWorkloadEstimateUsageErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchCreateWorkloadEstimateUsageItemTypeDef](./type_defs.md#batchcreateworkloadestimateusageitemtypedef) 
2. See [:material-code-braces: BatchCreateWorkloadEstimateUsageErrorTypeDef](./type_defs.md#batchcreateworkloadestimateusageerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBillEstimateInputUsageModificationsResponseTypeDef

```python
# ListBillEstimateInputUsageModificationsResponseTypeDef definition

class ListBillEstimateInputUsageModificationsResponseTypeDef(TypedDict):
    items: List[BillEstimateInputUsageModificationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BillEstimateInputUsageModificationSummaryTypeDef](./type_defs.md#billestimateinputusagemodificationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateBillScenarioUsageModificationResponseTypeDef

```python
# BatchUpdateBillScenarioUsageModificationResponseTypeDef definition

class BatchUpdateBillScenarioUsageModificationResponseTypeDef(TypedDict):
    items: List[BillScenarioUsageModificationItemTypeDef],  # (1)
    errors: List[BatchUpdateBillScenarioUsageModificationErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BillScenarioUsageModificationItemTypeDef](./type_defs.md#billscenariousagemodificationitemtypedef) 
2. See [:material-code-braces: BatchUpdateBillScenarioUsageModificationErrorTypeDef](./type_defs.md#batchupdatebillscenariousagemodificationerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBillScenarioUsageModificationsResponseTypeDef

```python
# ListBillScenarioUsageModificationsResponseTypeDef definition

class ListBillScenarioUsageModificationsResponseTypeDef(TypedDict):
    items: List[BillScenarioUsageModificationItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BillScenarioUsageModificationItemTypeDef](./type_defs.md#billscenariousagemodificationitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateWorkloadEstimateUsageResponseTypeDef

```python
# BatchUpdateWorkloadEstimateUsageResponseTypeDef definition

class BatchUpdateWorkloadEstimateUsageResponseTypeDef(TypedDict):
    items: List[WorkloadEstimateUsageItemTypeDef],  # (1)
    errors: List[BatchUpdateWorkloadEstimateUsageErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: WorkloadEstimateUsageItemTypeDef](./type_defs.md#workloadestimateusageitemtypedef) 
2. See [:material-code-braces: BatchUpdateWorkloadEstimateUsageErrorTypeDef](./type_defs.md#batchupdateworkloadestimateusageerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkloadEstimateUsageResponseTypeDef

```python
# ListWorkloadEstimateUsageResponseTypeDef definition

class ListWorkloadEstimateUsageResponseTypeDef(TypedDict):
    items: List[WorkloadEstimateUsageItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkloadEstimateUsageItemTypeDef](./type_defs.md#workloadestimateusageitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBillEstimateInputUsageModificationsResponsePaginatorTypeDef

```python
# ListBillEstimateInputUsageModificationsResponsePaginatorTypeDef definition

class ListBillEstimateInputUsageModificationsResponsePaginatorTypeDef(TypedDict):
    items: List[BillEstimateInputUsageModificationSummaryPaginatorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BillEstimateInputUsageModificationSummaryPaginatorTypeDef](./type_defs.md#billestimateinputusagemodificationsummarypaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBillScenarioUsageModificationsResponsePaginatorTypeDef

```python
# ListBillScenarioUsageModificationsResponsePaginatorTypeDef definition

class ListBillScenarioUsageModificationsResponsePaginatorTypeDef(TypedDict):
    items: List[BillScenarioUsageModificationItemPaginatorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BillScenarioUsageModificationItemPaginatorTypeDef](./type_defs.md#billscenariousagemodificationitempaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkloadEstimateUsageResponsePaginatorTypeDef

```python
# ListWorkloadEstimateUsageResponsePaginatorTypeDef definition

class ListWorkloadEstimateUsageResponsePaginatorTypeDef(TypedDict):
    items: List[WorkloadEstimateUsageItemPaginatorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkloadEstimateUsageItemPaginatorTypeDef](./type_defs.md#workloadestimateusageitempaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HistoricalUsageEntityTypeDef

```python
# HistoricalUsageEntityTypeDef definition

class HistoricalUsageEntityTypeDef(TypedDict):
    serviceCode: str,
    usageType: str,
    operation: str,
    usageAccountId: str,
    billInterval: BillIntervalUnionTypeDef,  # (1)
    filterExpression: ExpressionUnionTypeDef,  # (2)
    location: NotRequired[str],
```

1. See [:material-code-braces: BillIntervalTypeDef](./type_defs.md#billintervaltypedef) [:material-code-braces: BillIntervalOutputTypeDef](./type_defs.md#billintervaloutputtypedef) 
2. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) [:material-code-braces: ExpressionOutputTypeDef](./type_defs.md#expressionoutputtypedef) 
## BatchCreateBillScenarioUsageModificationEntryTypeDef

```python
# BatchCreateBillScenarioUsageModificationEntryTypeDef definition

class BatchCreateBillScenarioUsageModificationEntryTypeDef(TypedDict):
    serviceCode: str,
    usageType: str,
    operation: str,
    key: str,
    usageAccountId: str,
    availabilityZone: NotRequired[str],
    group: NotRequired[str],
    amounts: NotRequired[Sequence[UsageAmountTypeDef]],  # (1)
    historicalUsage: NotRequired[HistoricalUsageEntityUnionTypeDef],  # (2)
```

1. See [:material-code-braces: UsageAmountTypeDef](./type_defs.md#usageamounttypedef) 
2. See [:material-code-braces: HistoricalUsageEntityTypeDef](./type_defs.md#historicalusageentitytypedef) [:material-code-braces: HistoricalUsageEntityOutputTypeDef](./type_defs.md#historicalusageentityoutputtypedef) 
## BatchCreateWorkloadEstimateUsageEntryTypeDef

```python
# BatchCreateWorkloadEstimateUsageEntryTypeDef definition

class BatchCreateWorkloadEstimateUsageEntryTypeDef(TypedDict):
    serviceCode: str,
    usageType: str,
    operation: str,
    key: str,
    usageAccountId: str,
    amount: float,
    group: NotRequired[str],
    historicalUsage: NotRequired[HistoricalUsageEntityUnionTypeDef],  # (1)
```

1. See [:material-code-braces: HistoricalUsageEntityTypeDef](./type_defs.md#historicalusageentitytypedef) [:material-code-braces: HistoricalUsageEntityOutputTypeDef](./type_defs.md#historicalusageentityoutputtypedef) 
## BatchCreateBillScenarioUsageModificationRequestRequestTypeDef

```python
# BatchCreateBillScenarioUsageModificationRequestRequestTypeDef definition

class BatchCreateBillScenarioUsageModificationRequestRequestTypeDef(TypedDict):
    billScenarioId: str,
    usageModifications: Sequence[BatchCreateBillScenarioUsageModificationEntryTypeDef],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: BatchCreateBillScenarioUsageModificationEntryTypeDef](./type_defs.md#batchcreatebillscenariousagemodificationentrytypedef) 
## BatchCreateWorkloadEstimateUsageRequestRequestTypeDef

```python
# BatchCreateWorkloadEstimateUsageRequestRequestTypeDef definition

class BatchCreateWorkloadEstimateUsageRequestRequestTypeDef(TypedDict):
    workloadEstimateId: str,
    usage: Sequence[BatchCreateWorkloadEstimateUsageEntryTypeDef],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: BatchCreateWorkloadEstimateUsageEntryTypeDef](./type_defs.md#batchcreateworkloadestimateusageentrytypedef) 
