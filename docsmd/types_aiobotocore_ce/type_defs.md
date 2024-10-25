# Type definitions

> [Index](../README.md) > [CostExplorer](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CostExplorer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
    type annotations stubs module [types-aiobotocore-ce](https://pypi.org/project/types-aiobotocore-ce/).

## CostCategorySplitChargeRuleParameterUnionTypeDef

```python
# CostCategorySplitChargeRuleParameterUnionTypeDef definition

CostCategorySplitChargeRuleParameterUnionTypeDef = Union[
    CostCategorySplitChargeRuleParameterTypeDef,  # (1)
    CostCategorySplitChargeRuleParameterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CostCategorySplitChargeRuleParameterTypeDef](./type_defs.md#costcategorysplitchargeruleparametertypedef) 
2. See [:material-code-braces: CostCategorySplitChargeRuleParameterOutputTypeDef](./type_defs.md#costcategorysplitchargeruleparameteroutputtypedef) 

## CostCategoryValuesUnionTypeDef

```python
# CostCategoryValuesUnionTypeDef definition

CostCategoryValuesUnionTypeDef = Union[
    CostCategoryValuesTypeDef,  # (1)
    CostCategoryValuesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CostCategoryValuesTypeDef](./type_defs.md#costcategoryvaluestypedef) 
2. See [:material-code-braces: CostCategoryValuesOutputTypeDef](./type_defs.md#costcategoryvaluesoutputtypedef) 

## DimensionValuesUnionTypeDef

```python
# DimensionValuesUnionTypeDef definition

DimensionValuesUnionTypeDef = Union[
    DimensionValuesTypeDef,  # (1)
    DimensionValuesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DimensionValuesTypeDef](./type_defs.md#dimensionvaluestypedef) 
2. See [:material-code-braces: DimensionValuesOutputTypeDef](./type_defs.md#dimensionvaluesoutputtypedef) 

## TagValuesUnionTypeDef

```python
# TagValuesUnionTypeDef definition

TagValuesUnionTypeDef = Union[
    TagValuesTypeDef,  # (1)
    TagValuesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TagValuesTypeDef](./type_defs.md#tagvaluestypedef) 
2. See [:material-code-braces: TagValuesOutputTypeDef](./type_defs.md#tagvaluesoutputtypedef) 

## CostCategorySplitChargeRuleUnionTypeDef

```python
# CostCategorySplitChargeRuleUnionTypeDef definition

CostCategorySplitChargeRuleUnionTypeDef = Union[
    CostCategorySplitChargeRuleTypeDef,  # (1)
    CostCategorySplitChargeRuleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CostCategorySplitChargeRuleTypeDef](./type_defs.md#costcategorysplitchargeruletypedef) 
2. See [:material-code-braces: CostCategorySplitChargeRuleOutputTypeDef](./type_defs.md#costcategorysplitchargeruleoutputtypedef) 

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

## CostCategoryRuleUnionTypeDef

```python
# CostCategoryRuleUnionTypeDef definition

CostCategoryRuleUnionTypeDef = Union[
    CostCategoryRuleTypeDef,  # (1)
    CostCategoryRuleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CostCategoryRuleTypeDef](./type_defs.md#costcategoryruletypedef) 
2. See [:material-code-braces: CostCategoryRuleOutputTypeDef](./type_defs.md#costcategoryruleoutputtypedef) 



## AnomalyDateIntervalTypeDef

```python
# AnomalyDateIntervalTypeDef definition

class AnomalyDateIntervalTypeDef(TypedDict):
    StartDate: str,
    EndDate: NotRequired[str],
```

## AnomalyScoreTypeDef

```python
# AnomalyScoreTypeDef definition

class AnomalyScoreTypeDef(TypedDict):
    MaxScore: float,
    CurrentScore: float,
```

## SubscriberTypeDef

```python
# SubscriberTypeDef definition

class SubscriberTypeDef(TypedDict):
    Address: NotRequired[str],
    Type: NotRequired[SubscriberTypeType],  # (1)
    Status: NotRequired[SubscriberStatusType],  # (2)
```

1. See [:material-code-brackets: SubscriberTypeType](./literals.md#subscribertypetype) 
2. See [:material-code-brackets: SubscriberStatusType](./literals.md#subscriberstatustype) 
## ImpactTypeDef

```python
# ImpactTypeDef definition

class ImpactTypeDef(TypedDict):
    MaxImpact: float,
    TotalImpact: NotRequired[float],
    TotalActualSpend: NotRequired[float],
    TotalExpectedSpend: NotRequired[float],
    TotalImpactPercentage: NotRequired[float],
```

## RootCauseTypeDef

```python
# RootCauseTypeDef definition

class RootCauseTypeDef(TypedDict):
    Service: NotRequired[str],
    Region: NotRequired[str],
    LinkedAccount: NotRequired[str],
    UsageType: NotRequired[str],
    LinkedAccountName: NotRequired[str],
```

## CostAllocationTagBackfillRequestTypeDef

```python
# CostAllocationTagBackfillRequestTypeDef definition

class CostAllocationTagBackfillRequestTypeDef(TypedDict):
    BackfillFrom: NotRequired[str],
    RequestedAt: NotRequired[str],
    CompletedAt: NotRequired[str],
    BackfillStatus: NotRequired[CostAllocationTagBackfillStatusType],  # (1)
    LastUpdatedAt: NotRequired[str],
```

1. See [:material-code-brackets: CostAllocationTagBackfillStatusType](./literals.md#costallocationtagbackfillstatustype) 
## CostAllocationTagStatusEntryTypeDef

```python
# CostAllocationTagStatusEntryTypeDef definition

class CostAllocationTagStatusEntryTypeDef(TypedDict):
    TagKey: str,
    Status: CostAllocationTagStatusType,  # (1)
```

1. See [:material-code-brackets: CostAllocationTagStatusType](./literals.md#costallocationtagstatustype) 
## CostAllocationTagTypeDef

```python
# CostAllocationTagTypeDef definition

class CostAllocationTagTypeDef(TypedDict):
    TagKey: str,
    Type: CostAllocationTagTypeType,  # (1)
    Status: CostAllocationTagStatusType,  # (2)
    LastUpdatedDate: NotRequired[str],
    LastUsedDate: NotRequired[str],
```

1. See [:material-code-brackets: CostAllocationTagTypeType](./literals.md#costallocationtagtypetype) 
2. See [:material-code-brackets: CostAllocationTagStatusType](./literals.md#costallocationtagstatustype) 
## CostCategoryInheritedValueDimensionTypeDef

```python
# CostCategoryInheritedValueDimensionTypeDef definition

class CostCategoryInheritedValueDimensionTypeDef(TypedDict):
    DimensionName: NotRequired[CostCategoryInheritedValueDimensionNameType],  # (1)
    DimensionKey: NotRequired[str],
```

1. See [:material-code-brackets: CostCategoryInheritedValueDimensionNameType](./literals.md#costcategoryinheritedvaluedimensionnametype) 
## CostCategoryProcessingStatusTypeDef

```python
# CostCategoryProcessingStatusTypeDef definition

class CostCategoryProcessingStatusTypeDef(TypedDict):
    Component: NotRequired[CostCategoryStatusComponentType],  # (1)
    Status: NotRequired[CostCategoryStatusType],  # (2)
```

1. See [:material-code-brackets: CostCategoryStatusComponentType](./literals.md#costcategorystatuscomponenttype) 
2. See [:material-code-brackets: CostCategoryStatusType](./literals.md#costcategorystatustype) 
## CostCategorySplitChargeRuleParameterOutputTypeDef

```python
# CostCategorySplitChargeRuleParameterOutputTypeDef definition

class CostCategorySplitChargeRuleParameterOutputTypeDef(TypedDict):
    Type: CostCategorySplitChargeRuleParameterTypeType,  # (1)
    Values: List[str],
```

1. See [:material-code-brackets: CostCategorySplitChargeRuleParameterTypeType](./literals.md#costcategorysplitchargeruleparametertypetype) 
## CostCategorySplitChargeRuleParameterTypeDef

```python
# CostCategorySplitChargeRuleParameterTypeDef definition

class CostCategorySplitChargeRuleParameterTypeDef(TypedDict):
    Type: CostCategorySplitChargeRuleParameterTypeType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: CostCategorySplitChargeRuleParameterTypeType](./literals.md#costcategorysplitchargeruleparametertypetype) 
## CostCategoryValuesOutputTypeDef

```python
# CostCategoryValuesOutputTypeDef definition

class CostCategoryValuesOutputTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[List[str]],
    MatchOptions: NotRequired[List[MatchOptionType]],  # (1)
```

1. See [:material-code-brackets: MatchOptionType](./literals.md#matchoptiontype) 
## CostCategoryValuesTypeDef

```python
# CostCategoryValuesTypeDef definition

class CostCategoryValuesTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[Sequence[str]],
    MatchOptions: NotRequired[Sequence[MatchOptionType]],  # (1)
```

1. See [:material-code-brackets: MatchOptionType](./literals.md#matchoptiontype) 
## DateIntervalTypeDef

```python
# DateIntervalTypeDef definition

class DateIntervalTypeDef(TypedDict):
    Start: str,
    End: str,
```

## CoverageCostTypeDef

```python
# CoverageCostTypeDef definition

class CoverageCostTypeDef(TypedDict):
    OnDemandCost: NotRequired[str],
```

## CoverageHoursTypeDef

```python
# CoverageHoursTypeDef definition

class CoverageHoursTypeDef(TypedDict):
    OnDemandHours: NotRequired[str],
    ReservedHours: NotRequired[str],
    TotalRunningHours: NotRequired[str],
    CoverageHoursPercentage: NotRequired[str],
```

## CoverageNormalizedUnitsTypeDef

```python
# CoverageNormalizedUnitsTypeDef definition

class CoverageNormalizedUnitsTypeDef(TypedDict):
    OnDemandNormalizedUnits: NotRequired[str],
    ReservedNormalizedUnits: NotRequired[str],
    TotalRunningNormalizedUnits: NotRequired[str],
    CoverageNormalizedUnitsPercentage: NotRequired[str],
```

## ResourceTagTypeDef

```python
# ResourceTagTypeDef definition

class ResourceTagTypeDef(TypedDict):
    Key: str,
    Value: str,
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

## TagValuesOutputTypeDef

```python
# TagValuesOutputTypeDef definition

class TagValuesOutputTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[List[str]],
    MatchOptions: NotRequired[List[MatchOptionType]],  # (1)
```

1. See [:material-code-brackets: MatchOptionType](./literals.md#matchoptiontype) 
## DeleteAnomalyMonitorRequestRequestTypeDef

```python
# DeleteAnomalyMonitorRequestRequestTypeDef definition

class DeleteAnomalyMonitorRequestRequestTypeDef(TypedDict):
    MonitorArn: str,
```

## DeleteAnomalySubscriptionRequestRequestTypeDef

```python
# DeleteAnomalySubscriptionRequestRequestTypeDef definition

class DeleteAnomalySubscriptionRequestRequestTypeDef(TypedDict):
    SubscriptionArn: str,
```

## DeleteCostCategoryDefinitionRequestRequestTypeDef

```python
# DeleteCostCategoryDefinitionRequestRequestTypeDef definition

class DeleteCostCategoryDefinitionRequestRequestTypeDef(TypedDict):
    CostCategoryArn: str,
```

## DescribeCostCategoryDefinitionRequestRequestTypeDef

```python
# DescribeCostCategoryDefinitionRequestRequestTypeDef definition

class DescribeCostCategoryDefinitionRequestRequestTypeDef(TypedDict):
    CostCategoryArn: str,
    EffectiveOn: NotRequired[str],
```

## DimensionValuesOutputTypeDef

```python
# DimensionValuesOutputTypeDef definition

class DimensionValuesOutputTypeDef(TypedDict):
    Key: NotRequired[DimensionType],  # (1)
    Values: NotRequired[List[str]],
    MatchOptions: NotRequired[List[MatchOptionType]],  # (2)
```

1. See [:material-code-brackets: DimensionType](./literals.md#dimensiontype) 
2. See [:material-code-brackets: MatchOptionType](./literals.md#matchoptiontype) 
## DimensionValuesTypeDef

```python
# DimensionValuesTypeDef definition

class DimensionValuesTypeDef(TypedDict):
    Key: NotRequired[DimensionType],  # (1)
    Values: NotRequired[Sequence[str]],
    MatchOptions: NotRequired[Sequence[MatchOptionType]],  # (2)
```

1. See [:material-code-brackets: DimensionType](./literals.md#dimensiontype) 
2. See [:material-code-brackets: MatchOptionType](./literals.md#matchoptiontype) 
## DimensionValuesWithAttributesTypeDef

```python
# DimensionValuesWithAttributesTypeDef definition

class DimensionValuesWithAttributesTypeDef(TypedDict):
    Value: NotRequired[str],
    Attributes: NotRequired[Dict[str, str]],
```

## DiskResourceUtilizationTypeDef

```python
# DiskResourceUtilizationTypeDef definition

class DiskResourceUtilizationTypeDef(TypedDict):
    DiskReadOpsPerSecond: NotRequired[str],
    DiskWriteOpsPerSecond: NotRequired[str],
    DiskReadBytesPerSecond: NotRequired[str],
    DiskWriteBytesPerSecond: NotRequired[str],
```

## DynamoDBCapacityDetailsTypeDef

```python
# DynamoDBCapacityDetailsTypeDef definition

class DynamoDBCapacityDetailsTypeDef(TypedDict):
    CapacityUnits: NotRequired[str],
    Region: NotRequired[str],
```

## EBSResourceUtilizationTypeDef

```python
# EBSResourceUtilizationTypeDef definition

class EBSResourceUtilizationTypeDef(TypedDict):
    EbsReadOpsPerSecond: NotRequired[str],
    EbsWriteOpsPerSecond: NotRequired[str],
    EbsReadBytesPerSecond: NotRequired[str],
    EbsWriteBytesPerSecond: NotRequired[str],
```

## EC2InstanceDetailsTypeDef

```python
# EC2InstanceDetailsTypeDef definition

class EC2InstanceDetailsTypeDef(TypedDict):
    Family: NotRequired[str],
    InstanceType: NotRequired[str],
    Region: NotRequired[str],
    AvailabilityZone: NotRequired[str],
    Platform: NotRequired[str],
    Tenancy: NotRequired[str],
    CurrentGeneration: NotRequired[bool],
    SizeFlexEligible: NotRequired[bool],
```

## EC2ResourceDetailsTypeDef

```python
# EC2ResourceDetailsTypeDef definition

class EC2ResourceDetailsTypeDef(TypedDict):
    HourlyOnDemandRate: NotRequired[str],
    InstanceType: NotRequired[str],
    Platform: NotRequired[str],
    Region: NotRequired[str],
    Sku: NotRequired[str],
    Memory: NotRequired[str],
    NetworkPerformance: NotRequired[str],
    Storage: NotRequired[str],
    Vcpu: NotRequired[str],
```

## NetworkResourceUtilizationTypeDef

```python
# NetworkResourceUtilizationTypeDef definition

class NetworkResourceUtilizationTypeDef(TypedDict):
    NetworkInBytesPerSecond: NotRequired[str],
    NetworkOutBytesPerSecond: NotRequired[str],
    NetworkPacketsInPerSecond: NotRequired[str],
    NetworkPacketsOutPerSecond: NotRequired[str],
```

## EC2SpecificationTypeDef

```python
# EC2SpecificationTypeDef definition

class EC2SpecificationTypeDef(TypedDict):
    OfferingClass: NotRequired[OfferingClassType],  # (1)
```

1. See [:material-code-brackets: OfferingClassType](./literals.md#offeringclasstype) 
## ESInstanceDetailsTypeDef

```python
# ESInstanceDetailsTypeDef definition

class ESInstanceDetailsTypeDef(TypedDict):
    InstanceClass: NotRequired[str],
    InstanceSize: NotRequired[str],
    Region: NotRequired[str],
    CurrentGeneration: NotRequired[bool],
    SizeFlexEligible: NotRequired[bool],
```

## ElastiCacheInstanceDetailsTypeDef

```python
# ElastiCacheInstanceDetailsTypeDef definition

class ElastiCacheInstanceDetailsTypeDef(TypedDict):
    Family: NotRequired[str],
    NodeType: NotRequired[str],
    Region: NotRequired[str],
    ProductDescription: NotRequired[str],
    CurrentGeneration: NotRequired[bool],
    SizeFlexEligible: NotRequired[bool],
```

## GenerationSummaryTypeDef

```python
# GenerationSummaryTypeDef definition

class GenerationSummaryTypeDef(TypedDict):
    RecommendationId: NotRequired[str],
    GenerationStatus: NotRequired[GenerationStatusType],  # (1)
    GenerationStartedTime: NotRequired[str],
    GenerationCompletionTime: NotRequired[str],
    EstimatedCompletionTime: NotRequired[str],
```

1. See [:material-code-brackets: GenerationStatusType](./literals.md#generationstatustype) 
## TotalImpactFilterTypeDef

```python
# TotalImpactFilterTypeDef definition

class TotalImpactFilterTypeDef(TypedDict):
    NumericOperator: NumericOperatorType,  # (1)
    StartValue: float,
    EndValue: NotRequired[float],
```

1. See [:material-code-brackets: NumericOperatorType](./literals.md#numericoperatortype) 
## GetAnomalyMonitorsRequestRequestTypeDef

```python
# GetAnomalyMonitorsRequestRequestTypeDef definition

class GetAnomalyMonitorsRequestRequestTypeDef(TypedDict):
    MonitorArnList: NotRequired[Sequence[str]],
    NextPageToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetAnomalySubscriptionsRequestRequestTypeDef

```python
# GetAnomalySubscriptionsRequestRequestTypeDef definition

class GetAnomalySubscriptionsRequestRequestTypeDef(TypedDict):
    SubscriptionArnList: NotRequired[Sequence[str]],
    MonitorArn: NotRequired[str],
    NextPageToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetApproximateUsageRecordsRequestRequestTypeDef

```python
# GetApproximateUsageRecordsRequestRequestTypeDef definition

class GetApproximateUsageRecordsRequestRequestTypeDef(TypedDict):
    Granularity: GranularityType,  # (1)
    ApproximationDimension: ApproximationDimensionType,  # (2)
    Services: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
2. See [:material-code-brackets: ApproximationDimensionType](./literals.md#approximationdimensiontype) 
## GroupDefinitionTypeDef

```python
# GroupDefinitionTypeDef definition

class GroupDefinitionTypeDef(TypedDict):
    Type: NotRequired[GroupDefinitionTypeType],  # (1)
    Key: NotRequired[str],
```

1. See [:material-code-brackets: GroupDefinitionTypeType](./literals.md#groupdefinitiontypetype) 
## SortDefinitionTypeDef

```python
# SortDefinitionTypeDef definition

class SortDefinitionTypeDef(TypedDict):
    Key: str,
    SortOrder: NotRequired[SortOrderType],  # (1)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## MetricValueTypeDef

```python
# MetricValueTypeDef definition

class MetricValueTypeDef(TypedDict):
    Amount: NotRequired[str],
    Unit: NotRequired[str],
```

## ReservationPurchaseRecommendationMetadataTypeDef

```python
# ReservationPurchaseRecommendationMetadataTypeDef definition

class ReservationPurchaseRecommendationMetadataTypeDef(TypedDict):
    RecommendationId: NotRequired[str],
    GenerationTimestamp: NotRequired[str],
    AdditionalMetadata: NotRequired[str],
```

## ReservationAggregatesTypeDef

```python
# ReservationAggregatesTypeDef definition

class ReservationAggregatesTypeDef(TypedDict):
    UtilizationPercentage: NotRequired[str],
    UtilizationPercentageInUnits: NotRequired[str],
    PurchasedHours: NotRequired[str],
    PurchasedUnits: NotRequired[str],
    TotalActualHours: NotRequired[str],
    TotalActualUnits: NotRequired[str],
    UnusedHours: NotRequired[str],
    UnusedUnits: NotRequired[str],
    OnDemandCostOfRIHoursUsed: NotRequired[str],
    NetRISavings: NotRequired[str],
    TotalPotentialRISavings: NotRequired[str],
    AmortizedUpfrontFee: NotRequired[str],
    AmortizedRecurringFee: NotRequired[str],
    TotalAmortizedFee: NotRequired[str],
    RICostForUnusedHours: NotRequired[str],
    RealizedSavings: NotRequired[str],
    UnrealizedSavings: NotRequired[str],
```

## RightsizingRecommendationConfigurationTypeDef

```python
# RightsizingRecommendationConfigurationTypeDef definition

class RightsizingRecommendationConfigurationTypeDef(TypedDict):
    RecommendationTarget: RecommendationTargetType,  # (1)
    BenefitsConsidered: bool,
```

1. See [:material-code-brackets: RecommendationTargetType](./literals.md#recommendationtargettype) 
## RightsizingRecommendationMetadataTypeDef

```python
# RightsizingRecommendationMetadataTypeDef definition

class RightsizingRecommendationMetadataTypeDef(TypedDict):
    RecommendationId: NotRequired[str],
    GenerationTimestamp: NotRequired[str],
    LookbackPeriodInDays: NotRequired[LookbackPeriodInDaysType],  # (1)
    AdditionalMetadata: NotRequired[str],
```

1. See [:material-code-brackets: LookbackPeriodInDaysType](./literals.md#lookbackperiodindaystype) 
## RightsizingRecommendationSummaryTypeDef

```python
# RightsizingRecommendationSummaryTypeDef definition

class RightsizingRecommendationSummaryTypeDef(TypedDict):
    TotalRecommendationCount: NotRequired[str],
    EstimatedTotalMonthlySavingsAmount: NotRequired[str],
    SavingsCurrencyCode: NotRequired[str],
    SavingsPercentage: NotRequired[str],
```

## GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef

```python
# GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef definition

class GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef(TypedDict):
    RecommendationDetailId: str,
```

## SavingsPlansPurchaseRecommendationMetadataTypeDef

```python
# SavingsPlansPurchaseRecommendationMetadataTypeDef definition

class SavingsPlansPurchaseRecommendationMetadataTypeDef(TypedDict):
    RecommendationId: NotRequired[str],
    GenerationTimestamp: NotRequired[str],
    AdditionalMetadata: NotRequired[str],
```

## MemoryDBInstanceDetailsTypeDef

```python
# MemoryDBInstanceDetailsTypeDef definition

class MemoryDBInstanceDetailsTypeDef(TypedDict):
    Family: NotRequired[str],
    NodeType: NotRequired[str],
    Region: NotRequired[str],
    CurrentGeneration: NotRequired[bool],
    SizeFlexEligible: NotRequired[bool],
```

## RDSInstanceDetailsTypeDef

```python
# RDSInstanceDetailsTypeDef definition

class RDSInstanceDetailsTypeDef(TypedDict):
    Family: NotRequired[str],
    InstanceType: NotRequired[str],
    Region: NotRequired[str],
    DatabaseEngine: NotRequired[str],
    DatabaseEdition: NotRequired[str],
    DeploymentOption: NotRequired[str],
    LicenseModel: NotRequired[str],
    CurrentGeneration: NotRequired[bool],
    SizeFlexEligible: NotRequired[bool],
```

## RedshiftInstanceDetailsTypeDef

```python
# RedshiftInstanceDetailsTypeDef definition

class RedshiftInstanceDetailsTypeDef(TypedDict):
    Family: NotRequired[str],
    NodeType: NotRequired[str],
    Region: NotRequired[str],
    CurrentGeneration: NotRequired[bool],
    SizeFlexEligible: NotRequired[bool],
```

## ListCostAllocationTagBackfillHistoryRequestRequestTypeDef

```python
# ListCostAllocationTagBackfillHistoryRequestRequestTypeDef definition

class ListCostAllocationTagBackfillHistoryRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListCostAllocationTagsRequestRequestTypeDef

```python
# ListCostAllocationTagsRequestRequestTypeDef definition

class ListCostAllocationTagsRequestRequestTypeDef(TypedDict):
    Status: NotRequired[CostAllocationTagStatusType],  # (1)
    TagKeys: NotRequired[Sequence[str]],
    Type: NotRequired[CostAllocationTagTypeType],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: CostAllocationTagStatusType](./literals.md#costallocationtagstatustype) 
2. See [:material-code-brackets: CostAllocationTagTypeType](./literals.md#costallocationtagtypetype) 
## ListCostCategoryDefinitionsRequestRequestTypeDef

```python
# ListCostCategoryDefinitionsRequestRequestTypeDef definition

class ListCostCategoryDefinitionsRequestRequestTypeDef(TypedDict):
    EffectiveOn: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef

```python
# ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef definition

class ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef(TypedDict):
    GenerationStatus: NotRequired[GenerationStatusType],  # (1)
    RecommendationIds: NotRequired[Sequence[str]],
    PageSize: NotRequired[int],
    NextPageToken: NotRequired[str],
```

1. See [:material-code-brackets: GenerationStatusType](./literals.md#generationstatustype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ProvideAnomalyFeedbackRequestRequestTypeDef

```python
# ProvideAnomalyFeedbackRequestRequestTypeDef definition

class ProvideAnomalyFeedbackRequestRequestTypeDef(TypedDict):
    AnomalyId: str,
    Feedback: AnomalyFeedbackTypeType,  # (1)
```

1. See [:material-code-brackets: AnomalyFeedbackTypeType](./literals.md#anomalyfeedbacktypetype) 
## RecommendationDetailHourlyMetricsTypeDef

```python
# RecommendationDetailHourlyMetricsTypeDef definition

class RecommendationDetailHourlyMetricsTypeDef(TypedDict):
    StartTime: NotRequired[str],
    EstimatedOnDemandCost: NotRequired[str],
    CurrentCoverage: NotRequired[str],
    EstimatedCoverage: NotRequired[str],
    EstimatedNewCommitmentUtilization: NotRequired[str],
```

## ReservationPurchaseRecommendationSummaryTypeDef

```python
# ReservationPurchaseRecommendationSummaryTypeDef definition

class ReservationPurchaseRecommendationSummaryTypeDef(TypedDict):
    TotalEstimatedMonthlySavingsAmount: NotRequired[str],
    TotalEstimatedMonthlySavingsPercentage: NotRequired[str],
    CurrencyCode: NotRequired[str],
```

## TerminateRecommendationDetailTypeDef

```python
# TerminateRecommendationDetailTypeDef definition

class TerminateRecommendationDetailTypeDef(TypedDict):
    EstimatedMonthlySavings: NotRequired[str],
    CurrencyCode: NotRequired[str],
```

## SavingsPlansAmortizedCommitmentTypeDef

```python
# SavingsPlansAmortizedCommitmentTypeDef definition

class SavingsPlansAmortizedCommitmentTypeDef(TypedDict):
    AmortizedRecurringCommitment: NotRequired[str],
    AmortizedUpfrontCommitment: NotRequired[str],
    TotalAmortizedCommitment: NotRequired[str],
```

## SavingsPlansCoverageDataTypeDef

```python
# SavingsPlansCoverageDataTypeDef definition

class SavingsPlansCoverageDataTypeDef(TypedDict):
    SpendCoveredBySavingsPlans: NotRequired[str],
    OnDemandCost: NotRequired[str],
    TotalCost: NotRequired[str],
    CoveragePercentage: NotRequired[str],
```

## SavingsPlansDetailsTypeDef

```python
# SavingsPlansDetailsTypeDef definition

class SavingsPlansDetailsTypeDef(TypedDict):
    Region: NotRequired[str],
    InstanceFamily: NotRequired[str],
    OfferingId: NotRequired[str],
```

## SavingsPlansPurchaseRecommendationSummaryTypeDef

```python
# SavingsPlansPurchaseRecommendationSummaryTypeDef definition

class SavingsPlansPurchaseRecommendationSummaryTypeDef(TypedDict):
    EstimatedROI: NotRequired[str],
    CurrencyCode: NotRequired[str],
    EstimatedTotalCost: NotRequired[str],
    CurrentOnDemandSpend: NotRequired[str],
    EstimatedSavingsAmount: NotRequired[str],
    TotalRecommendationCount: NotRequired[str],
    DailyCommitmentToPurchase: NotRequired[str],
    HourlyCommitmentToPurchase: NotRequired[str],
    EstimatedSavingsPercentage: NotRequired[str],
    EstimatedMonthlySavingsAmount: NotRequired[str],
    EstimatedOnDemandCostWithCurrentCommitment: NotRequired[str],
```

## SavingsPlansSavingsTypeDef

```python
# SavingsPlansSavingsTypeDef definition

class SavingsPlansSavingsTypeDef(TypedDict):
    NetSavings: NotRequired[str],
    OnDemandCostEquivalent: NotRequired[str],
```

## SavingsPlansUtilizationTypeDef

```python
# SavingsPlansUtilizationTypeDef definition

class SavingsPlansUtilizationTypeDef(TypedDict):
    TotalCommitment: NotRequired[str],
    UsedCommitment: NotRequired[str],
    UnusedCommitment: NotRequired[str],
    UtilizationPercentage: NotRequired[str],
```

## StartCostAllocationTagBackfillRequestRequestTypeDef

```python
# StartCostAllocationTagBackfillRequestRequestTypeDef definition

class StartCostAllocationTagBackfillRequestRequestTypeDef(TypedDict):
    BackfillFrom: str,
```

## TagValuesTypeDef

```python
# TagValuesTypeDef definition

class TagValuesTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[Sequence[str]],
    MatchOptions: NotRequired[Sequence[MatchOptionType]],  # (1)
```

1. See [:material-code-brackets: MatchOptionType](./literals.md#matchoptiontype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    ResourceTagKeys: Sequence[str],
```

## UpdateAnomalyMonitorRequestRequestTypeDef

```python
# UpdateAnomalyMonitorRequestRequestTypeDef definition

class UpdateAnomalyMonitorRequestRequestTypeDef(TypedDict):
    MonitorArn: str,
    MonitorName: NotRequired[str],
```

## UpdateCostAllocationTagsStatusErrorTypeDef

```python
# UpdateCostAllocationTagsStatusErrorTypeDef definition

class UpdateCostAllocationTagsStatusErrorTypeDef(TypedDict):
    TagKey: NotRequired[str],
    Code: NotRequired[str],
    Message: NotRequired[str],
```

## AnomalyTypeDef

```python
# AnomalyTypeDef definition

class AnomalyTypeDef(TypedDict):
    AnomalyId: str,
    AnomalyScore: AnomalyScoreTypeDef,  # (2)
    Impact: ImpactTypeDef,  # (3)
    MonitorArn: str,
    AnomalyStartDate: NotRequired[str],
    AnomalyEndDate: NotRequired[str],
    DimensionValue: NotRequired[str],
    RootCauses: NotRequired[List[RootCauseTypeDef]],  # (1)
    Feedback: NotRequired[AnomalyFeedbackTypeType],  # (4)
```

1. See [:material-code-braces: RootCauseTypeDef](./type_defs.md#rootcausetypedef) 
2. See [:material-code-braces: AnomalyScoreTypeDef](./type_defs.md#anomalyscoretypedef) 
3. See [:material-code-braces: ImpactTypeDef](./type_defs.md#impacttypedef) 
4. See [:material-code-brackets: AnomalyFeedbackTypeType](./literals.md#anomalyfeedbacktypetype) 
## UpdateCostAllocationTagsStatusRequestRequestTypeDef

```python
# UpdateCostAllocationTagsStatusRequestRequestTypeDef definition

class UpdateCostAllocationTagsStatusRequestRequestTypeDef(TypedDict):
    CostAllocationTagsStatus: Sequence[CostAllocationTagStatusEntryTypeDef],  # (1)
```

1. See [:material-code-braces: CostAllocationTagStatusEntryTypeDef](./type_defs.md#costallocationtagstatusentrytypedef) 
## CostCategoryReferenceTypeDef

```python
# CostCategoryReferenceTypeDef definition

class CostCategoryReferenceTypeDef(TypedDict):
    CostCategoryArn: NotRequired[str],
    Name: NotRequired[str],
    EffectiveStart: NotRequired[str],
    EffectiveEnd: NotRequired[str],
    NumberOfRules: NotRequired[int],
    ProcessingStatus: NotRequired[List[CostCategoryProcessingStatusTypeDef]],  # (1)
    Values: NotRequired[List[str]],
    DefaultValue: NotRequired[str],
```

1. See [:material-code-braces: CostCategoryProcessingStatusTypeDef](./type_defs.md#costcategoryprocessingstatustypedef) 
## CostCategorySplitChargeRuleOutputTypeDef

```python
# CostCategorySplitChargeRuleOutputTypeDef definition

class CostCategorySplitChargeRuleOutputTypeDef(TypedDict):
    Source: str,
    Targets: List[str],
    Method: CostCategorySplitChargeMethodType,  # (1)
    Parameters: NotRequired[List[CostCategorySplitChargeRuleParameterOutputTypeDef]],  # (2)
```

1. See [:material-code-brackets: CostCategorySplitChargeMethodType](./literals.md#costcategorysplitchargemethodtype) 
2. See [:material-code-braces: CostCategorySplitChargeRuleParameterOutputTypeDef](./type_defs.md#costcategorysplitchargeruleparameteroutputtypedef) 
## ForecastResultTypeDef

```python
# ForecastResultTypeDef definition

class ForecastResultTypeDef(TypedDict):
    TimePeriod: NotRequired[DateIntervalTypeDef],  # (1)
    MeanValue: NotRequired[str],
    PredictionIntervalLowerBound: NotRequired[str],
    PredictionIntervalUpperBound: NotRequired[str],
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
## CoverageTypeDef

```python
# CoverageTypeDef definition

class CoverageTypeDef(TypedDict):
    CoverageHours: NotRequired[CoverageHoursTypeDef],  # (1)
    CoverageNormalizedUnits: NotRequired[CoverageNormalizedUnitsTypeDef],  # (2)
    CoverageCost: NotRequired[CoverageCostTypeDef],  # (3)
```

1. See [:material-code-braces: CoverageHoursTypeDef](./type_defs.md#coveragehourstypedef) 
2. See [:material-code-braces: CoverageNormalizedUnitsTypeDef](./type_defs.md#coveragenormalizedunitstypedef) 
3. See [:material-code-braces: CoverageCostTypeDef](./type_defs.md#coveragecosttypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    ResourceTags: Sequence[ResourceTagTypeDef],  # (1)
```

1. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
## CreateAnomalyMonitorResponseTypeDef

```python
# CreateAnomalyMonitorResponseTypeDef definition

class CreateAnomalyMonitorResponseTypeDef(TypedDict):
    MonitorArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAnomalySubscriptionResponseTypeDef

```python
# CreateAnomalySubscriptionResponseTypeDef definition

class CreateAnomalySubscriptionResponseTypeDef(TypedDict):
    SubscriptionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCostCategoryDefinitionResponseTypeDef

```python
# CreateCostCategoryDefinitionResponseTypeDef definition

class CreateCostCategoryDefinitionResponseTypeDef(TypedDict):
    CostCategoryArn: str,
    EffectiveStart: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteCostCategoryDefinitionResponseTypeDef

```python
# DeleteCostCategoryDefinitionResponseTypeDef definition

class DeleteCostCategoryDefinitionResponseTypeDef(TypedDict):
    CostCategoryArn: str,
    EffectiveEnd: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApproximateUsageRecordsResponseTypeDef

```python
# GetApproximateUsageRecordsResponseTypeDef definition

class GetApproximateUsageRecordsResponseTypeDef(TypedDict):
    Services: Dict[str, int],
    TotalRecords: int,
    LookbackPeriod: DateIntervalTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCostCategoriesResponseTypeDef

```python
# GetCostCategoriesResponseTypeDef definition

class GetCostCategoriesResponseTypeDef(TypedDict):
    NextPageToken: str,
    CostCategoryNames: List[str],
    CostCategoryValues: List[str],
    ReturnSize: int,
    TotalSize: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTagsResponseTypeDef

```python
# GetTagsResponseTypeDef definition

class GetTagsResponseTypeDef(TypedDict):
    NextPageToken: str,
    Tags: List[str],
    ReturnSize: int,
    TotalSize: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCostAllocationTagBackfillHistoryResponseTypeDef

```python
# ListCostAllocationTagBackfillHistoryResponseTypeDef definition

class ListCostAllocationTagBackfillHistoryResponseTypeDef(TypedDict):
    BackfillRequests: List[CostAllocationTagBackfillRequestTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CostAllocationTagBackfillRequestTypeDef](./type_defs.md#costallocationtagbackfillrequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCostAllocationTagsResponseTypeDef

```python
# ListCostAllocationTagsResponseTypeDef definition

class ListCostAllocationTagsResponseTypeDef(TypedDict):
    CostAllocationTags: List[CostAllocationTagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CostAllocationTagTypeDef](./type_defs.md#costallocationtagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    ResourceTags: List[ResourceTagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProvideAnomalyFeedbackResponseTypeDef

```python
# ProvideAnomalyFeedbackResponseTypeDef definition

class ProvideAnomalyFeedbackResponseTypeDef(TypedDict):
    AnomalyId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartCostAllocationTagBackfillResponseTypeDef

```python
# StartCostAllocationTagBackfillResponseTypeDef definition

class StartCostAllocationTagBackfillResponseTypeDef(TypedDict):
    BackfillRequest: CostAllocationTagBackfillRequestTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CostAllocationTagBackfillRequestTypeDef](./type_defs.md#costallocationtagbackfillrequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef

```python
# StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef definition

class StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef(TypedDict):
    RecommendationId: str,
    GenerationStartedTime: str,
    EstimatedCompletionTime: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAnomalyMonitorResponseTypeDef

```python
# UpdateAnomalyMonitorResponseTypeDef definition

class UpdateAnomalyMonitorResponseTypeDef(TypedDict):
    MonitorArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAnomalySubscriptionResponseTypeDef

```python
# UpdateAnomalySubscriptionResponseTypeDef definition

class UpdateAnomalySubscriptionResponseTypeDef(TypedDict):
    SubscriptionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCostCategoryDefinitionResponseTypeDef

```python
# UpdateCostCategoryDefinitionResponseTypeDef definition

class UpdateCostCategoryDefinitionResponseTypeDef(TypedDict):
    CostCategoryArn: str,
    EffectiveStart: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExpressionOutputTypeDef

```python
# ExpressionOutputTypeDef definition

class ExpressionOutputTypeDef(TypedDict):
    Or: NotRequired[List[Dict[str, Any]]],
    And: NotRequired[List[Dict[str, Any]]],
    Not: NotRequired[Dict[str, Any]],
    Dimensions: NotRequired[DimensionValuesOutputTypeDef],  # (1)
    Tags: NotRequired[TagValuesOutputTypeDef],  # (2)
    CostCategories: NotRequired[CostCategoryValuesOutputTypeDef],  # (3)
```

1. See [:material-code-braces: DimensionValuesOutputTypeDef](./type_defs.md#dimensionvaluesoutputtypedef) 
2. See [:material-code-braces: TagValuesOutputTypeDef](./type_defs.md#tagvaluesoutputtypedef) 
3. See [:material-code-braces: CostCategoryValuesOutputTypeDef](./type_defs.md#costcategoryvaluesoutputtypedef) 
## GetDimensionValuesResponseTypeDef

```python
# GetDimensionValuesResponseTypeDef definition

class GetDimensionValuesResponseTypeDef(TypedDict):
    DimensionValues: List[DimensionValuesWithAttributesTypeDef],  # (1)
    ReturnSize: int,
    TotalSize: int,
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DimensionValuesWithAttributesTypeDef](./type_defs.md#dimensionvalueswithattributestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReservedCapacityDetailsTypeDef

```python
# ReservedCapacityDetailsTypeDef definition

class ReservedCapacityDetailsTypeDef(TypedDict):
    DynamoDBCapacityDetails: NotRequired[DynamoDBCapacityDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: DynamoDBCapacityDetailsTypeDef](./type_defs.md#dynamodbcapacitydetailstypedef) 
## ResourceDetailsTypeDef

```python
# ResourceDetailsTypeDef definition

class ResourceDetailsTypeDef(TypedDict):
    EC2ResourceDetails: NotRequired[EC2ResourceDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: EC2ResourceDetailsTypeDef](./type_defs.md#ec2resourcedetailstypedef) 
## EC2ResourceUtilizationTypeDef

```python
# EC2ResourceUtilizationTypeDef definition

class EC2ResourceUtilizationTypeDef(TypedDict):
    MaxCpuUtilizationPercentage: NotRequired[str],
    MaxMemoryUtilizationPercentage: NotRequired[str],
    MaxStorageUtilizationPercentage: NotRequired[str],
    EBSResourceUtilization: NotRequired[EBSResourceUtilizationTypeDef],  # (1)
    DiskResourceUtilization: NotRequired[DiskResourceUtilizationTypeDef],  # (2)
    NetworkResourceUtilization: NotRequired[NetworkResourceUtilizationTypeDef],  # (3)
```

1. See [:material-code-braces: EBSResourceUtilizationTypeDef](./type_defs.md#ebsresourceutilizationtypedef) 
2. See [:material-code-braces: DiskResourceUtilizationTypeDef](./type_defs.md#diskresourceutilizationtypedef) 
3. See [:material-code-braces: NetworkResourceUtilizationTypeDef](./type_defs.md#networkresourceutilizationtypedef) 
## ServiceSpecificationTypeDef

```python
# ServiceSpecificationTypeDef definition

class ServiceSpecificationTypeDef(TypedDict):
    EC2Specification: NotRequired[EC2SpecificationTypeDef],  # (1)
```

1. See [:material-code-braces: EC2SpecificationTypeDef](./type_defs.md#ec2specificationtypedef) 
## ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef

```python
# ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef definition

class ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef(TypedDict):
    GenerationSummaryList: List[GenerationSummaryTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GenerationSummaryTypeDef](./type_defs.md#generationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAnomaliesRequestRequestTypeDef

```python
# GetAnomaliesRequestRequestTypeDef definition

class GetAnomaliesRequestRequestTypeDef(TypedDict):
    DateInterval: AnomalyDateIntervalTypeDef,  # (1)
    MonitorArn: NotRequired[str],
    Feedback: NotRequired[AnomalyFeedbackTypeType],  # (2)
    TotalImpact: NotRequired[TotalImpactFilterTypeDef],  # (3)
    NextPageToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: AnomalyDateIntervalTypeDef](./type_defs.md#anomalydateintervaltypedef) 
2. See [:material-code-brackets: AnomalyFeedbackTypeType](./literals.md#anomalyfeedbacktypetype) 
3. See [:material-code-braces: TotalImpactFilterTypeDef](./type_defs.md#totalimpactfiltertypedef) 
## GroupTypeDef

```python
# GroupTypeDef definition

class GroupTypeDef(TypedDict):
    Keys: NotRequired[List[str]],
    Metrics: NotRequired[Dict[str, MetricValueTypeDef]],  # (1)
```

1. See [:material-code-braces: MetricValueTypeDef](./type_defs.md#metricvaluetypedef) 
## ReservationUtilizationGroupTypeDef

```python
# ReservationUtilizationGroupTypeDef definition

class ReservationUtilizationGroupTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
    Attributes: NotRequired[Dict[str, str]],
    Utilization: NotRequired[ReservationAggregatesTypeDef],  # (1)
```

1. See [:material-code-braces: ReservationAggregatesTypeDef](./type_defs.md#reservationaggregatestypedef) 
## InstanceDetailsTypeDef

```python
# InstanceDetailsTypeDef definition

class InstanceDetailsTypeDef(TypedDict):
    EC2InstanceDetails: NotRequired[EC2InstanceDetailsTypeDef],  # (1)
    RDSInstanceDetails: NotRequired[RDSInstanceDetailsTypeDef],  # (2)
    RedshiftInstanceDetails: NotRequired[RedshiftInstanceDetailsTypeDef],  # (3)
    ElastiCacheInstanceDetails: NotRequired[ElastiCacheInstanceDetailsTypeDef],  # (4)
    ESInstanceDetails: NotRequired[ESInstanceDetailsTypeDef],  # (5)
    MemoryDBInstanceDetails: NotRequired[MemoryDBInstanceDetailsTypeDef],  # (6)
```

1. See [:material-code-braces: EC2InstanceDetailsTypeDef](./type_defs.md#ec2instancedetailstypedef) 
2. See [:material-code-braces: RDSInstanceDetailsTypeDef](./type_defs.md#rdsinstancedetailstypedef) 
3. See [:material-code-braces: RedshiftInstanceDetailsTypeDef](./type_defs.md#redshiftinstancedetailstypedef) 
4. See [:material-code-braces: ElastiCacheInstanceDetailsTypeDef](./type_defs.md#elasticacheinstancedetailstypedef) 
5. See [:material-code-braces: ESInstanceDetailsTypeDef](./type_defs.md#esinstancedetailstypedef) 
6. See [:material-code-braces: MemoryDBInstanceDetailsTypeDef](./type_defs.md#memorydbinstancedetailstypedef) 
## RecommendationDetailDataTypeDef

```python
# RecommendationDetailDataTypeDef definition

class RecommendationDetailDataTypeDef(TypedDict):
    AccountScope: NotRequired[AccountScopeType],  # (1)
    LookbackPeriodInDays: NotRequired[LookbackPeriodInDaysType],  # (2)
    SavingsPlansType: NotRequired[SupportedSavingsPlansTypeType],  # (3)
    TermInYears: NotRequired[TermInYearsType],  # (4)
    PaymentOption: NotRequired[PaymentOptionType],  # (5)
    AccountId: NotRequired[str],
    CurrencyCode: NotRequired[str],
    InstanceFamily: NotRequired[str],
    Region: NotRequired[str],
    OfferingId: NotRequired[str],
    GenerationTimestamp: NotRequired[str],
    LatestUsageTimestamp: NotRequired[str],
    CurrentAverageHourlyOnDemandSpend: NotRequired[str],
    CurrentMaximumHourlyOnDemandSpend: NotRequired[str],
    CurrentMinimumHourlyOnDemandSpend: NotRequired[str],
    EstimatedAverageUtilization: NotRequired[str],
    EstimatedMonthlySavingsAmount: NotRequired[str],
    EstimatedOnDemandCost: NotRequired[str],
    EstimatedOnDemandCostWithCurrentCommitment: NotRequired[str],
    EstimatedROI: NotRequired[str],
    EstimatedSPCost: NotRequired[str],
    EstimatedSavingsAmount: NotRequired[str],
    EstimatedSavingsPercentage: NotRequired[str],
    ExistingHourlyCommitment: NotRequired[str],
    HourlyCommitmentToPurchase: NotRequired[str],
    UpfrontCost: NotRequired[str],
    CurrentAverageCoverage: NotRequired[str],
    EstimatedAverageCoverage: NotRequired[str],
    MetricsOverLookbackPeriod: NotRequired[List[RecommendationDetailHourlyMetricsTypeDef]],  # (6)
```

1. See [:material-code-brackets: AccountScopeType](./literals.md#accountscopetype) 
2. See [:material-code-brackets: LookbackPeriodInDaysType](./literals.md#lookbackperiodindaystype) 
3. See [:material-code-brackets: SupportedSavingsPlansTypeType](./literals.md#supportedsavingsplanstypetype) 
4. See [:material-code-brackets: TermInYearsType](./literals.md#terminyearstype) 
5. See [:material-code-brackets: PaymentOptionType](./literals.md#paymentoptiontype) 
6. See [:material-code-braces: RecommendationDetailHourlyMetricsTypeDef](./type_defs.md#recommendationdetailhourlymetricstypedef) 
## SavingsPlansCoverageTypeDef

```python
# SavingsPlansCoverageTypeDef definition

class SavingsPlansCoverageTypeDef(TypedDict):
    Attributes: NotRequired[Dict[str, str]],
    Coverage: NotRequired[SavingsPlansCoverageDataTypeDef],  # (1)
    TimePeriod: NotRequired[DateIntervalTypeDef],  # (2)
```

1. See [:material-code-braces: SavingsPlansCoverageDataTypeDef](./type_defs.md#savingsplanscoveragedatatypedef) 
2. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
## SavingsPlansPurchaseRecommendationDetailTypeDef

```python
# SavingsPlansPurchaseRecommendationDetailTypeDef definition

class SavingsPlansPurchaseRecommendationDetailTypeDef(TypedDict):
    SavingsPlansDetails: NotRequired[SavingsPlansDetailsTypeDef],  # (1)
    AccountId: NotRequired[str],
    UpfrontCost: NotRequired[str],
    EstimatedROI: NotRequired[str],
    CurrencyCode: NotRequired[str],
    EstimatedSPCost: NotRequired[str],
    EstimatedOnDemandCost: NotRequired[str],
    EstimatedOnDemandCostWithCurrentCommitment: NotRequired[str],
    EstimatedSavingsAmount: NotRequired[str],
    EstimatedSavingsPercentage: NotRequired[str],
    HourlyCommitmentToPurchase: NotRequired[str],
    EstimatedAverageUtilization: NotRequired[str],
    EstimatedMonthlySavingsAmount: NotRequired[str],
    CurrentMinimumHourlyOnDemandSpend: NotRequired[str],
    CurrentMaximumHourlyOnDemandSpend: NotRequired[str],
    CurrentAverageHourlyOnDemandSpend: NotRequired[str],
    RecommendationDetailId: NotRequired[str],
```

1. See [:material-code-braces: SavingsPlansDetailsTypeDef](./type_defs.md#savingsplansdetailstypedef) 
## SavingsPlansUtilizationAggregatesTypeDef

```python
# SavingsPlansUtilizationAggregatesTypeDef definition

class SavingsPlansUtilizationAggregatesTypeDef(TypedDict):
    Utilization: SavingsPlansUtilizationTypeDef,  # (1)
    Savings: NotRequired[SavingsPlansSavingsTypeDef],  # (2)
    AmortizedCommitment: NotRequired[SavingsPlansAmortizedCommitmentTypeDef],  # (3)
```

1. See [:material-code-braces: SavingsPlansUtilizationTypeDef](./type_defs.md#savingsplansutilizationtypedef) 
2. See [:material-code-braces: SavingsPlansSavingsTypeDef](./type_defs.md#savingsplanssavingstypedef) 
3. See [:material-code-braces: SavingsPlansAmortizedCommitmentTypeDef](./type_defs.md#savingsplansamortizedcommitmenttypedef) 
## SavingsPlansUtilizationByTimeTypeDef

```python
# SavingsPlansUtilizationByTimeTypeDef definition

class SavingsPlansUtilizationByTimeTypeDef(TypedDict):
    TimePeriod: DateIntervalTypeDef,  # (1)
    Utilization: SavingsPlansUtilizationTypeDef,  # (2)
    Savings: NotRequired[SavingsPlansSavingsTypeDef],  # (3)
    AmortizedCommitment: NotRequired[SavingsPlansAmortizedCommitmentTypeDef],  # (4)
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: SavingsPlansUtilizationTypeDef](./type_defs.md#savingsplansutilizationtypedef) 
3. See [:material-code-braces: SavingsPlansSavingsTypeDef](./type_defs.md#savingsplanssavingstypedef) 
4. See [:material-code-braces: SavingsPlansAmortizedCommitmentTypeDef](./type_defs.md#savingsplansamortizedcommitmenttypedef) 
## SavingsPlansUtilizationDetailTypeDef

```python
# SavingsPlansUtilizationDetailTypeDef definition

class SavingsPlansUtilizationDetailTypeDef(TypedDict):
    SavingsPlanArn: NotRequired[str],
    Attributes: NotRequired[Dict[str, str]],
    Utilization: NotRequired[SavingsPlansUtilizationTypeDef],  # (1)
    Savings: NotRequired[SavingsPlansSavingsTypeDef],  # (2)
    AmortizedCommitment: NotRequired[SavingsPlansAmortizedCommitmentTypeDef],  # (3)
```

1. See [:material-code-braces: SavingsPlansUtilizationTypeDef](./type_defs.md#savingsplansutilizationtypedef) 
2. See [:material-code-braces: SavingsPlansSavingsTypeDef](./type_defs.md#savingsplanssavingstypedef) 
3. See [:material-code-braces: SavingsPlansAmortizedCommitmentTypeDef](./type_defs.md#savingsplansamortizedcommitmenttypedef) 
## UpdateCostAllocationTagsStatusResponseTypeDef

```python
# UpdateCostAllocationTagsStatusResponseTypeDef definition

class UpdateCostAllocationTagsStatusResponseTypeDef(TypedDict):
    Errors: List[UpdateCostAllocationTagsStatusErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateCostAllocationTagsStatusErrorTypeDef](./type_defs.md#updatecostallocationtagsstatuserrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAnomaliesResponseTypeDef

```python
# GetAnomaliesResponseTypeDef definition

class GetAnomaliesResponseTypeDef(TypedDict):
    Anomalies: List[AnomalyTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnomalyTypeDef](./type_defs.md#anomalytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCostCategoryDefinitionsResponseTypeDef

```python
# ListCostCategoryDefinitionsResponseTypeDef definition

class ListCostCategoryDefinitionsResponseTypeDef(TypedDict):
    CostCategoryReferences: List[CostCategoryReferenceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CostCategoryReferenceTypeDef](./type_defs.md#costcategoryreferencetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CostCategorySplitChargeRuleTypeDef

```python
# CostCategorySplitChargeRuleTypeDef definition

class CostCategorySplitChargeRuleTypeDef(TypedDict):
    Source: str,
    Targets: Sequence[str],
    Method: CostCategorySplitChargeMethodType,  # (1)
    Parameters: NotRequired[Sequence[CostCategorySplitChargeRuleParameterUnionTypeDef]],  # (2)
```

1. See [:material-code-brackets: CostCategorySplitChargeMethodType](./literals.md#costcategorysplitchargemethodtype) 
2. See [:material-code-braces: CostCategorySplitChargeRuleParameterTypeDef](./type_defs.md#costcategorysplitchargeruleparametertypedef) [:material-code-braces: CostCategorySplitChargeRuleParameterOutputTypeDef](./type_defs.md#costcategorysplitchargeruleparameteroutputtypedef) 
## GetCostForecastResponseTypeDef

```python
# GetCostForecastResponseTypeDef definition

class GetCostForecastResponseTypeDef(TypedDict):
    Total: MetricValueTypeDef,  # (1)
    ForecastResultsByTime: List[ForecastResultTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MetricValueTypeDef](./type_defs.md#metricvaluetypedef) 
2. See [:material-code-braces: ForecastResultTypeDef](./type_defs.md#forecastresulttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUsageForecastResponseTypeDef

```python
# GetUsageForecastResponseTypeDef definition

class GetUsageForecastResponseTypeDef(TypedDict):
    Total: MetricValueTypeDef,  # (1)
    ForecastResultsByTime: List[ForecastResultTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MetricValueTypeDef](./type_defs.md#metricvaluetypedef) 
2. See [:material-code-braces: ForecastResultTypeDef](./type_defs.md#forecastresulttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReservationCoverageGroupTypeDef

```python
# ReservationCoverageGroupTypeDef definition

class ReservationCoverageGroupTypeDef(TypedDict):
    Attributes: NotRequired[Dict[str, str]],
    Coverage: NotRequired[CoverageTypeDef],  # (1)
```

1. See [:material-code-braces: CoverageTypeDef](./type_defs.md#coveragetypedef) 
## AnomalyMonitorOutputTypeDef

```python
# AnomalyMonitorOutputTypeDef definition

class AnomalyMonitorOutputTypeDef(TypedDict):
    MonitorName: str,
    MonitorType: MonitorTypeType,  # (1)
    MonitorArn: NotRequired[str],
    CreationDate: NotRequired[str],
    LastUpdatedDate: NotRequired[str],
    LastEvaluatedDate: NotRequired[str],
    MonitorDimension: NotRequired[MonitorDimensionType],  # (2)
    MonitorSpecification: NotRequired[ExpressionOutputTypeDef],  # (3)
    DimensionalValueCount: NotRequired[int],
```

1. See [:material-code-brackets: MonitorTypeType](./literals.md#monitortypetype) 
2. See [:material-code-brackets: MonitorDimensionType](./literals.md#monitordimensiontype) 
3. See [:material-code-braces: ExpressionOutputTypeDef](./type_defs.md#expressionoutputtypedef) 
## AnomalySubscriptionOutputTypeDef

```python
# AnomalySubscriptionOutputTypeDef definition

class AnomalySubscriptionOutputTypeDef(TypedDict):
    MonitorArnList: List[str],
    Subscribers: List[SubscriberTypeDef],  # (1)
    Frequency: AnomalySubscriptionFrequencyType,  # (2)
    SubscriptionName: str,
    SubscriptionArn: NotRequired[str],
    AccountId: NotRequired[str],
    Threshold: NotRequired[float],
    ThresholdExpression: NotRequired[ExpressionOutputTypeDef],  # (3)
```

1. See [:material-code-braces: SubscriberTypeDef](./type_defs.md#subscribertypedef) 
2. See [:material-code-brackets: AnomalySubscriptionFrequencyType](./literals.md#anomalysubscriptionfrequencytype) 
3. See [:material-code-braces: ExpressionOutputTypeDef](./type_defs.md#expressionoutputtypedef) 
## CostCategoryRuleOutputTypeDef

```python
# CostCategoryRuleOutputTypeDef definition

class CostCategoryRuleOutputTypeDef(TypedDict):
    Value: NotRequired[str],
    Rule: NotRequired[ExpressionOutputTypeDef],  # (1)
    InheritedValue: NotRequired[CostCategoryInheritedValueDimensionTypeDef],  # (2)
    Type: NotRequired[CostCategoryRuleTypeType],  # (3)
```

1. See [:material-code-braces: ExpressionOutputTypeDef](./type_defs.md#expressionoutputtypedef) 
2. See [:material-code-braces: CostCategoryInheritedValueDimensionTypeDef](./type_defs.md#costcategoryinheritedvaluedimensiontypedef) 
3. See [:material-code-brackets: CostCategoryRuleTypeType](./literals.md#costcategoryruletypetype) 
## ResourceUtilizationTypeDef

```python
# ResourceUtilizationTypeDef definition

class ResourceUtilizationTypeDef(TypedDict):
    EC2ResourceUtilization: NotRequired[EC2ResourceUtilizationTypeDef],  # (1)
```

1. See [:material-code-braces: EC2ResourceUtilizationTypeDef](./type_defs.md#ec2resourceutilizationtypedef) 
## ResultByTimeTypeDef

```python
# ResultByTimeTypeDef definition

class ResultByTimeTypeDef(TypedDict):
    TimePeriod: NotRequired[DateIntervalTypeDef],  # (1)
    Total: NotRequired[Dict[str, MetricValueTypeDef]],  # (2)
    Groups: NotRequired[List[GroupTypeDef]],  # (3)
    Estimated: NotRequired[bool],
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: MetricValueTypeDef](./type_defs.md#metricvaluetypedef) 
3. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
## UtilizationByTimeTypeDef

```python
# UtilizationByTimeTypeDef definition

class UtilizationByTimeTypeDef(TypedDict):
    TimePeriod: NotRequired[DateIntervalTypeDef],  # (1)
    Groups: NotRequired[List[ReservationUtilizationGroupTypeDef]],  # (2)
    Total: NotRequired[ReservationAggregatesTypeDef],  # (3)
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: ReservationUtilizationGroupTypeDef](./type_defs.md#reservationutilizationgrouptypedef) 
3. See [:material-code-braces: ReservationAggregatesTypeDef](./type_defs.md#reservationaggregatestypedef) 
## ReservationPurchaseRecommendationDetailTypeDef

```python
# ReservationPurchaseRecommendationDetailTypeDef definition

class ReservationPurchaseRecommendationDetailTypeDef(TypedDict):
    AccountId: NotRequired[str],
    InstanceDetails: NotRequired[InstanceDetailsTypeDef],  # (1)
    RecommendedNumberOfInstancesToPurchase: NotRequired[str],
    RecommendedNormalizedUnitsToPurchase: NotRequired[str],
    MinimumNumberOfInstancesUsedPerHour: NotRequired[str],
    MinimumNormalizedUnitsUsedPerHour: NotRequired[str],
    MaximumNumberOfInstancesUsedPerHour: NotRequired[str],
    MaximumNormalizedUnitsUsedPerHour: NotRequired[str],
    AverageNumberOfInstancesUsedPerHour: NotRequired[str],
    AverageNormalizedUnitsUsedPerHour: NotRequired[str],
    AverageUtilization: NotRequired[str],
    EstimatedBreakEvenInMonths: NotRequired[str],
    CurrencyCode: NotRequired[str],
    EstimatedMonthlySavingsAmount: NotRequired[str],
    EstimatedMonthlySavingsPercentage: NotRequired[str],
    EstimatedMonthlyOnDemandCost: NotRequired[str],
    EstimatedReservationCostForLookbackPeriod: NotRequired[str],
    UpfrontCost: NotRequired[str],
    RecurringStandardMonthlyCost: NotRequired[str],
    ReservedCapacityDetails: NotRequired[ReservedCapacityDetailsTypeDef],  # (2)
    RecommendedNumberOfCapacityUnitsToPurchase: NotRequired[str],
    MinimumNumberOfCapacityUnitsUsedPerHour: NotRequired[str],
    MaximumNumberOfCapacityUnitsUsedPerHour: NotRequired[str],
    AverageNumberOfCapacityUnitsUsedPerHour: NotRequired[str],
```

1. See [:material-code-braces: InstanceDetailsTypeDef](./type_defs.md#instancedetailstypedef) 
2. See [:material-code-braces: ReservedCapacityDetailsTypeDef](./type_defs.md#reservedcapacitydetailstypedef) 
## GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef

```python
# GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef definition

class GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef(TypedDict):
    RecommendationDetailId: str,
    RecommendationDetailData: RecommendationDetailDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecommendationDetailDataTypeDef](./type_defs.md#recommendationdetaildatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSavingsPlansCoverageResponseTypeDef

```python
# GetSavingsPlansCoverageResponseTypeDef definition

class GetSavingsPlansCoverageResponseTypeDef(TypedDict):
    SavingsPlansCoverages: List[SavingsPlansCoverageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SavingsPlansCoverageTypeDef](./type_defs.md#savingsplanscoveragetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SavingsPlansPurchaseRecommendationTypeDef

```python
# SavingsPlansPurchaseRecommendationTypeDef definition

class SavingsPlansPurchaseRecommendationTypeDef(TypedDict):
    AccountScope: NotRequired[AccountScopeType],  # (1)
    SavingsPlansType: NotRequired[SupportedSavingsPlansTypeType],  # (2)
    TermInYears: NotRequired[TermInYearsType],  # (3)
    PaymentOption: NotRequired[PaymentOptionType],  # (4)
    LookbackPeriodInDays: NotRequired[LookbackPeriodInDaysType],  # (5)
    SavingsPlansPurchaseRecommendationDetails: NotRequired[List[SavingsPlansPurchaseRecommendationDetailTypeDef]],  # (6)
    SavingsPlansPurchaseRecommendationSummary: NotRequired[SavingsPlansPurchaseRecommendationSummaryTypeDef],  # (7)
```

1. See [:material-code-brackets: AccountScopeType](./literals.md#accountscopetype) 
2. See [:material-code-brackets: SupportedSavingsPlansTypeType](./literals.md#supportedsavingsplanstypetype) 
3. See [:material-code-brackets: TermInYearsType](./literals.md#terminyearstype) 
4. See [:material-code-brackets: PaymentOptionType](./literals.md#paymentoptiontype) 
5. See [:material-code-brackets: LookbackPeriodInDaysType](./literals.md#lookbackperiodindaystype) 
6. See [:material-code-braces: SavingsPlansPurchaseRecommendationDetailTypeDef](./type_defs.md#savingsplanspurchaserecommendationdetailtypedef) 
7. See [:material-code-braces: SavingsPlansPurchaseRecommendationSummaryTypeDef](./type_defs.md#savingsplanspurchaserecommendationsummarytypedef) 
## GetSavingsPlansUtilizationResponseTypeDef

```python
# GetSavingsPlansUtilizationResponseTypeDef definition

class GetSavingsPlansUtilizationResponseTypeDef(TypedDict):
    SavingsPlansUtilizationsByTime: List[SavingsPlansUtilizationByTimeTypeDef],  # (1)
    Total: SavingsPlansUtilizationAggregatesTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SavingsPlansUtilizationByTimeTypeDef](./type_defs.md#savingsplansutilizationbytimetypedef) 
2. See [:material-code-braces: SavingsPlansUtilizationAggregatesTypeDef](./type_defs.md#savingsplansutilizationaggregatestypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSavingsPlansUtilizationDetailsResponseTypeDef

```python
# GetSavingsPlansUtilizationDetailsResponseTypeDef definition

class GetSavingsPlansUtilizationDetailsResponseTypeDef(TypedDict):
    SavingsPlansUtilizationDetails: List[SavingsPlansUtilizationDetailTypeDef],  # (1)
    Total: SavingsPlansUtilizationAggregatesTypeDef,  # (2)
    TimePeriod: DateIntervalTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SavingsPlansUtilizationDetailTypeDef](./type_defs.md#savingsplansutilizationdetailtypedef) 
2. See [:material-code-braces: SavingsPlansUtilizationAggregatesTypeDef](./type_defs.md#savingsplansutilizationaggregatestypedef) 
3. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExpressionTypeDef

```python
# ExpressionTypeDef definition

class ExpressionTypeDef(TypedDict):
    Or: NotRequired[Sequence[Mapping[str, Any]]],
    And: NotRequired[Sequence[Mapping[str, Any]]],
    Not: NotRequired[Mapping[str, Any]],
    Dimensions: NotRequired[DimensionValuesUnionTypeDef],  # (1)
    Tags: NotRequired[TagValuesUnionTypeDef],  # (2)
    CostCategories: NotRequired[CostCategoryValuesUnionTypeDef],  # (3)
```

1. See [:material-code-braces: DimensionValuesTypeDef](./type_defs.md#dimensionvaluestypedef) [:material-code-braces: DimensionValuesOutputTypeDef](./type_defs.md#dimensionvaluesoutputtypedef) 
2. See [:material-code-braces: TagValuesTypeDef](./type_defs.md#tagvaluestypedef) [:material-code-braces: TagValuesOutputTypeDef](./type_defs.md#tagvaluesoutputtypedef) 
3. See [:material-code-braces: CostCategoryValuesTypeDef](./type_defs.md#costcategoryvaluestypedef) [:material-code-braces: CostCategoryValuesOutputTypeDef](./type_defs.md#costcategoryvaluesoutputtypedef) 
## CoverageByTimeTypeDef

```python
# CoverageByTimeTypeDef definition

class CoverageByTimeTypeDef(TypedDict):
    TimePeriod: NotRequired[DateIntervalTypeDef],  # (1)
    Groups: NotRequired[List[ReservationCoverageGroupTypeDef]],  # (2)
    Total: NotRequired[CoverageTypeDef],  # (3)
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: ReservationCoverageGroupTypeDef](./type_defs.md#reservationcoveragegrouptypedef) 
3. See [:material-code-braces: CoverageTypeDef](./type_defs.md#coveragetypedef) 
## GetAnomalyMonitorsResponseTypeDef

```python
# GetAnomalyMonitorsResponseTypeDef definition

class GetAnomalyMonitorsResponseTypeDef(TypedDict):
    AnomalyMonitors: List[AnomalyMonitorOutputTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnomalyMonitorOutputTypeDef](./type_defs.md#anomalymonitoroutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAnomalySubscriptionsResponseTypeDef

```python
# GetAnomalySubscriptionsResponseTypeDef definition

class GetAnomalySubscriptionsResponseTypeDef(TypedDict):
    AnomalySubscriptions: List[AnomalySubscriptionOutputTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnomalySubscriptionOutputTypeDef](./type_defs.md#anomalysubscriptionoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CostCategoryTypeDef

```python
# CostCategoryTypeDef definition

class CostCategoryTypeDef(TypedDict):
    CostCategoryArn: str,
    EffectiveStart: str,
    Name: str,
    RuleVersion: CostCategoryRuleVersionType,  # (1)
    Rules: List[CostCategoryRuleOutputTypeDef],  # (2)
    EffectiveEnd: NotRequired[str],
    SplitChargeRules: NotRequired[List[CostCategorySplitChargeRuleOutputTypeDef]],  # (3)
    ProcessingStatus: NotRequired[List[CostCategoryProcessingStatusTypeDef]],  # (4)
    DefaultValue: NotRequired[str],
```

1. See [:material-code-brackets: CostCategoryRuleVersionType](./literals.md#costcategoryruleversiontype) 
2. See [:material-code-braces: CostCategoryRuleOutputTypeDef](./type_defs.md#costcategoryruleoutputtypedef) 
3. See [:material-code-braces: CostCategorySplitChargeRuleOutputTypeDef](./type_defs.md#costcategorysplitchargeruleoutputtypedef) 
4. See [:material-code-braces: CostCategoryProcessingStatusTypeDef](./type_defs.md#costcategoryprocessingstatustypedef) 
## CurrentInstanceTypeDef

```python
# CurrentInstanceTypeDef definition

class CurrentInstanceTypeDef(TypedDict):
    ResourceId: NotRequired[str],
    InstanceName: NotRequired[str],
    Tags: NotRequired[List[TagValuesOutputTypeDef]],  # (1)
    ResourceDetails: NotRequired[ResourceDetailsTypeDef],  # (2)
    ResourceUtilization: NotRequired[ResourceUtilizationTypeDef],  # (3)
    ReservationCoveredHoursInLookbackPeriod: NotRequired[str],
    SavingsPlansCoveredHoursInLookbackPeriod: NotRequired[str],
    OnDemandHoursInLookbackPeriod: NotRequired[str],
    TotalRunningHoursInLookbackPeriod: NotRequired[str],
    MonthlyCost: NotRequired[str],
    CurrencyCode: NotRequired[str],
```

1. See [:material-code-braces: TagValuesOutputTypeDef](./type_defs.md#tagvaluesoutputtypedef) 
2. See [:material-code-braces: ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef) 
3. See [:material-code-braces: ResourceUtilizationTypeDef](./type_defs.md#resourceutilizationtypedef) 
## TargetInstanceTypeDef

```python
# TargetInstanceTypeDef definition

class TargetInstanceTypeDef(TypedDict):
    EstimatedMonthlyCost: NotRequired[str],
    EstimatedMonthlySavings: NotRequired[str],
    CurrencyCode: NotRequired[str],
    DefaultTargetInstance: NotRequired[bool],
    ResourceDetails: NotRequired[ResourceDetailsTypeDef],  # (1)
    ExpectedResourceUtilization: NotRequired[ResourceUtilizationTypeDef],  # (2)
    PlatformDifferences: NotRequired[List[PlatformDifferenceType]],  # (3)
```

1. See [:material-code-braces: ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef) 
2. See [:material-code-braces: ResourceUtilizationTypeDef](./type_defs.md#resourceutilizationtypedef) 
3. See [:material-code-brackets: PlatformDifferenceType](./literals.md#platformdifferencetype) 
## GetCostAndUsageResponseTypeDef

```python
# GetCostAndUsageResponseTypeDef definition

class GetCostAndUsageResponseTypeDef(TypedDict):
    NextPageToken: str,
    GroupDefinitions: List[GroupDefinitionTypeDef],  # (1)
    ResultsByTime: List[ResultByTimeTypeDef],  # (2)
    DimensionValueAttributes: List[DimensionValuesWithAttributesTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: GroupDefinitionTypeDef](./type_defs.md#groupdefinitiontypedef) 
2. See [:material-code-braces: ResultByTimeTypeDef](./type_defs.md#resultbytimetypedef) 
3. See [:material-code-braces: DimensionValuesWithAttributesTypeDef](./type_defs.md#dimensionvalueswithattributestypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCostAndUsageWithResourcesResponseTypeDef

```python
# GetCostAndUsageWithResourcesResponseTypeDef definition

class GetCostAndUsageWithResourcesResponseTypeDef(TypedDict):
    NextPageToken: str,
    GroupDefinitions: List[GroupDefinitionTypeDef],  # (1)
    ResultsByTime: List[ResultByTimeTypeDef],  # (2)
    DimensionValueAttributes: List[DimensionValuesWithAttributesTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: GroupDefinitionTypeDef](./type_defs.md#groupdefinitiontypedef) 
2. See [:material-code-braces: ResultByTimeTypeDef](./type_defs.md#resultbytimetypedef) 
3. See [:material-code-braces: DimensionValuesWithAttributesTypeDef](./type_defs.md#dimensionvalueswithattributestypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetReservationUtilizationResponseTypeDef

```python
# GetReservationUtilizationResponseTypeDef definition

class GetReservationUtilizationResponseTypeDef(TypedDict):
    UtilizationsByTime: List[UtilizationByTimeTypeDef],  # (1)
    Total: ReservationAggregatesTypeDef,  # (2)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: UtilizationByTimeTypeDef](./type_defs.md#utilizationbytimetypedef) 
2. See [:material-code-braces: ReservationAggregatesTypeDef](./type_defs.md#reservationaggregatestypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReservationPurchaseRecommendationTypeDef

```python
# ReservationPurchaseRecommendationTypeDef definition

class ReservationPurchaseRecommendationTypeDef(TypedDict):
    AccountScope: NotRequired[AccountScopeType],  # (1)
    LookbackPeriodInDays: NotRequired[LookbackPeriodInDaysType],  # (2)
    TermInYears: NotRequired[TermInYearsType],  # (3)
    PaymentOption: NotRequired[PaymentOptionType],  # (4)
    ServiceSpecification: NotRequired[ServiceSpecificationTypeDef],  # (5)
    RecommendationDetails: NotRequired[List[ReservationPurchaseRecommendationDetailTypeDef]],  # (6)
    RecommendationSummary: NotRequired[ReservationPurchaseRecommendationSummaryTypeDef],  # (7)
```

1. See [:material-code-brackets: AccountScopeType](./literals.md#accountscopetype) 
2. See [:material-code-brackets: LookbackPeriodInDaysType](./literals.md#lookbackperiodindaystype) 
3. See [:material-code-brackets: TermInYearsType](./literals.md#terminyearstype) 
4. See [:material-code-brackets: PaymentOptionType](./literals.md#paymentoptiontype) 
5. See [:material-code-braces: ServiceSpecificationTypeDef](./type_defs.md#servicespecificationtypedef) 
6. See [:material-code-braces: ReservationPurchaseRecommendationDetailTypeDef](./type_defs.md#reservationpurchaserecommendationdetailtypedef) 
7. See [:material-code-braces: ReservationPurchaseRecommendationSummaryTypeDef](./type_defs.md#reservationpurchaserecommendationsummarytypedef) 
## GetSavingsPlansPurchaseRecommendationResponseTypeDef

```python
# GetSavingsPlansPurchaseRecommendationResponseTypeDef definition

class GetSavingsPlansPurchaseRecommendationResponseTypeDef(TypedDict):
    Metadata: SavingsPlansPurchaseRecommendationMetadataTypeDef,  # (1)
    SavingsPlansPurchaseRecommendation: SavingsPlansPurchaseRecommendationTypeDef,  # (2)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SavingsPlansPurchaseRecommendationMetadataTypeDef](./type_defs.md#savingsplanspurchaserecommendationmetadatatypedef) 
2. See [:material-code-braces: SavingsPlansPurchaseRecommendationTypeDef](./type_defs.md#savingsplanspurchaserecommendationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCostAndUsageRequestRequestTypeDef

```python
# GetCostAndUsageRequestRequestTypeDef definition

class GetCostAndUsageRequestRequestTypeDef(TypedDict):
    TimePeriod: DateIntervalTypeDef,  # (1)
    Granularity: GranularityType,  # (2)
    Metrics: Sequence[str],
    Filter: NotRequired[ExpressionTypeDef],  # (3)
    GroupBy: NotRequired[Sequence[GroupDefinitionTypeDef]],  # (4)
    NextPageToken: NotRequired[str],
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
3. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
4. See [:material-code-braces: GroupDefinitionTypeDef](./type_defs.md#groupdefinitiontypedef) 
## GetCostAndUsageWithResourcesRequestRequestTypeDef

```python
# GetCostAndUsageWithResourcesRequestRequestTypeDef definition

class GetCostAndUsageWithResourcesRequestRequestTypeDef(TypedDict):
    TimePeriod: DateIntervalTypeDef,  # (1)
    Granularity: GranularityType,  # (2)
    Filter: ExpressionTypeDef,  # (3)
    Metrics: NotRequired[Sequence[str]],
    GroupBy: NotRequired[Sequence[GroupDefinitionTypeDef]],  # (4)
    NextPageToken: NotRequired[str],
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
3. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
4. See [:material-code-braces: GroupDefinitionTypeDef](./type_defs.md#groupdefinitiontypedef) 
## GetCostCategoriesRequestRequestTypeDef

```python
# GetCostCategoriesRequestRequestTypeDef definition

class GetCostCategoriesRequestRequestTypeDef(TypedDict):
    TimePeriod: DateIntervalTypeDef,  # (1)
    SearchString: NotRequired[str],
    CostCategoryName: NotRequired[str],
    Filter: NotRequired[ExpressionTypeDef],  # (2)
    SortBy: NotRequired[Sequence[SortDefinitionTypeDef]],  # (3)
    MaxResults: NotRequired[int],
    NextPageToken: NotRequired[str],
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
3. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
## GetCostForecastRequestRequestTypeDef

```python
# GetCostForecastRequestRequestTypeDef definition

class GetCostForecastRequestRequestTypeDef(TypedDict):
    TimePeriod: DateIntervalTypeDef,  # (1)
    Metric: MetricType,  # (2)
    Granularity: GranularityType,  # (3)
    Filter: NotRequired[ExpressionTypeDef],  # (4)
    PredictionIntervalLevel: NotRequired[int],
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-brackets: MetricType](./literals.md#metrictype) 
3. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
4. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
## GetDimensionValuesRequestRequestTypeDef

```python
# GetDimensionValuesRequestRequestTypeDef definition

class GetDimensionValuesRequestRequestTypeDef(TypedDict):
    TimePeriod: DateIntervalTypeDef,  # (1)
    Dimension: DimensionType,  # (2)
    SearchString: NotRequired[str],
    Context: NotRequired[ContextType],  # (3)
    Filter: NotRequired[ExpressionTypeDef],  # (4)
    SortBy: NotRequired[Sequence[SortDefinitionTypeDef]],  # (5)
    MaxResults: NotRequired[int],
    NextPageToken: NotRequired[str],
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-brackets: DimensionType](./literals.md#dimensiontype) 
3. See [:material-code-brackets: ContextType](./literals.md#contexttype) 
4. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
5. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
## GetReservationCoverageRequestRequestTypeDef

```python
# GetReservationCoverageRequestRequestTypeDef definition

class GetReservationCoverageRequestRequestTypeDef(TypedDict):
    TimePeriod: DateIntervalTypeDef,  # (1)
    GroupBy: NotRequired[Sequence[GroupDefinitionTypeDef]],  # (2)
    Granularity: NotRequired[GranularityType],  # (3)
    Filter: NotRequired[ExpressionTypeDef],  # (4)
    Metrics: NotRequired[Sequence[str]],
    NextPageToken: NotRequired[str],
    SortBy: NotRequired[SortDefinitionTypeDef],  # (5)
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: GroupDefinitionTypeDef](./type_defs.md#groupdefinitiontypedef) 
3. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
4. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
5. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
## GetReservationPurchaseRecommendationRequestRequestTypeDef

```python
# GetReservationPurchaseRecommendationRequestRequestTypeDef definition

class GetReservationPurchaseRecommendationRequestRequestTypeDef(TypedDict):
    Service: str,
    AccountId: NotRequired[str],
    Filter: NotRequired[ExpressionTypeDef],  # (1)
    AccountScope: NotRequired[AccountScopeType],  # (2)
    LookbackPeriodInDays: NotRequired[LookbackPeriodInDaysType],  # (3)
    TermInYears: NotRequired[TermInYearsType],  # (4)
    PaymentOption: NotRequired[PaymentOptionType],  # (5)
    ServiceSpecification: NotRequired[ServiceSpecificationTypeDef],  # (6)
    PageSize: NotRequired[int],
    NextPageToken: NotRequired[str],
```

1. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
2. See [:material-code-brackets: AccountScopeType](./literals.md#accountscopetype) 
3. See [:material-code-brackets: LookbackPeriodInDaysType](./literals.md#lookbackperiodindaystype) 
4. See [:material-code-brackets: TermInYearsType](./literals.md#terminyearstype) 
5. See [:material-code-brackets: PaymentOptionType](./literals.md#paymentoptiontype) 
6. See [:material-code-braces: ServiceSpecificationTypeDef](./type_defs.md#servicespecificationtypedef) 
## GetReservationUtilizationRequestRequestTypeDef

```python
# GetReservationUtilizationRequestRequestTypeDef definition

class GetReservationUtilizationRequestRequestTypeDef(TypedDict):
    TimePeriod: DateIntervalTypeDef,  # (1)
    GroupBy: NotRequired[Sequence[GroupDefinitionTypeDef]],  # (2)
    Granularity: NotRequired[GranularityType],  # (3)
    Filter: NotRequired[ExpressionTypeDef],  # (4)
    SortBy: NotRequired[SortDefinitionTypeDef],  # (5)
    NextPageToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: GroupDefinitionTypeDef](./type_defs.md#groupdefinitiontypedef) 
3. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
4. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
5. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
## GetRightsizingRecommendationRequestRequestTypeDef

```python
# GetRightsizingRecommendationRequestRequestTypeDef definition

class GetRightsizingRecommendationRequestRequestTypeDef(TypedDict):
    Service: str,
    Filter: NotRequired[ExpressionTypeDef],  # (1)
    Configuration: NotRequired[RightsizingRecommendationConfigurationTypeDef],  # (2)
    PageSize: NotRequired[int],
    NextPageToken: NotRequired[str],
```

1. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
2. See [:material-code-braces: RightsizingRecommendationConfigurationTypeDef](./type_defs.md#rightsizingrecommendationconfigurationtypedef) 
## GetSavingsPlansCoverageRequestRequestTypeDef

```python
# GetSavingsPlansCoverageRequestRequestTypeDef definition

class GetSavingsPlansCoverageRequestRequestTypeDef(TypedDict):
    TimePeriod: DateIntervalTypeDef,  # (1)
    GroupBy: NotRequired[Sequence[GroupDefinitionTypeDef]],  # (2)
    Granularity: NotRequired[GranularityType],  # (3)
    Filter: NotRequired[ExpressionTypeDef],  # (4)
    Metrics: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SortBy: NotRequired[SortDefinitionTypeDef],  # (5)
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: GroupDefinitionTypeDef](./type_defs.md#groupdefinitiontypedef) 
3. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
4. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
5. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
## GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef

```python
# GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef definition

class GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef(TypedDict):
    SavingsPlansType: SupportedSavingsPlansTypeType,  # (1)
    TermInYears: TermInYearsType,  # (2)
    PaymentOption: PaymentOptionType,  # (3)
    LookbackPeriodInDays: LookbackPeriodInDaysType,  # (4)
    AccountScope: NotRequired[AccountScopeType],  # (5)
    NextPageToken: NotRequired[str],
    PageSize: NotRequired[int],
    Filter: NotRequired[ExpressionTypeDef],  # (6)
```

1. See [:material-code-brackets: SupportedSavingsPlansTypeType](./literals.md#supportedsavingsplanstypetype) 
2. See [:material-code-brackets: TermInYearsType](./literals.md#terminyearstype) 
3. See [:material-code-brackets: PaymentOptionType](./literals.md#paymentoptiontype) 
4. See [:material-code-brackets: LookbackPeriodInDaysType](./literals.md#lookbackperiodindaystype) 
5. See [:material-code-brackets: AccountScopeType](./literals.md#accountscopetype) 
6. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
## GetSavingsPlansUtilizationDetailsRequestRequestTypeDef

```python
# GetSavingsPlansUtilizationDetailsRequestRequestTypeDef definition

class GetSavingsPlansUtilizationDetailsRequestRequestTypeDef(TypedDict):
    TimePeriod: DateIntervalTypeDef,  # (1)
    Filter: NotRequired[ExpressionTypeDef],  # (2)
    DataType: NotRequired[Sequence[SavingsPlansDataTypeType]],  # (3)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SortBy: NotRequired[SortDefinitionTypeDef],  # (4)
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
3. See [:material-code-brackets: SavingsPlansDataTypeType](./literals.md#savingsplansdatatypetype) 
4. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
## GetSavingsPlansUtilizationRequestRequestTypeDef

```python
# GetSavingsPlansUtilizationRequestRequestTypeDef definition

class GetSavingsPlansUtilizationRequestRequestTypeDef(TypedDict):
    TimePeriod: DateIntervalTypeDef,  # (1)
    Granularity: NotRequired[GranularityType],  # (2)
    Filter: NotRequired[ExpressionTypeDef],  # (3)
    SortBy: NotRequired[SortDefinitionTypeDef],  # (4)
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
3. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
4. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
## GetTagsRequestRequestTypeDef

```python
# GetTagsRequestRequestTypeDef definition

class GetTagsRequestRequestTypeDef(TypedDict):
    TimePeriod: DateIntervalTypeDef,  # (1)
    SearchString: NotRequired[str],
    TagKey: NotRequired[str],
    Filter: NotRequired[ExpressionTypeDef],  # (2)
    SortBy: NotRequired[Sequence[SortDefinitionTypeDef]],  # (3)
    MaxResults: NotRequired[int],
    NextPageToken: NotRequired[str],
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
3. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
## GetUsageForecastRequestRequestTypeDef

```python
# GetUsageForecastRequestRequestTypeDef definition

class GetUsageForecastRequestRequestTypeDef(TypedDict):
    TimePeriod: DateIntervalTypeDef,  # (1)
    Metric: MetricType,  # (2)
    Granularity: GranularityType,  # (3)
    Filter: NotRequired[ExpressionTypeDef],  # (4)
    PredictionIntervalLevel: NotRequired[int],
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-brackets: MetricType](./literals.md#metrictype) 
3. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
4. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
## UpdateAnomalySubscriptionRequestRequestTypeDef

```python
# UpdateAnomalySubscriptionRequestRequestTypeDef definition

class UpdateAnomalySubscriptionRequestRequestTypeDef(TypedDict):
    SubscriptionArn: str,
    Threshold: NotRequired[float],
    Frequency: NotRequired[AnomalySubscriptionFrequencyType],  # (1)
    MonitorArnList: NotRequired[Sequence[str]],
    Subscribers: NotRequired[Sequence[SubscriberTypeDef]],  # (2)
    SubscriptionName: NotRequired[str],
    ThresholdExpression: NotRequired[ExpressionTypeDef],  # (3)
```

1. See [:material-code-brackets: AnomalySubscriptionFrequencyType](./literals.md#anomalysubscriptionfrequencytype) 
2. See [:material-code-braces: SubscriberTypeDef](./type_defs.md#subscribertypedef) 
3. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
## GetReservationCoverageResponseTypeDef

```python
# GetReservationCoverageResponseTypeDef definition

class GetReservationCoverageResponseTypeDef(TypedDict):
    CoveragesByTime: List[CoverageByTimeTypeDef],  # (1)
    Total: CoverageTypeDef,  # (2)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CoverageByTimeTypeDef](./type_defs.md#coveragebytimetypedef) 
2. See [:material-code-braces: CoverageTypeDef](./type_defs.md#coveragetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCostCategoryDefinitionResponseTypeDef

```python
# DescribeCostCategoryDefinitionResponseTypeDef definition

class DescribeCostCategoryDefinitionResponseTypeDef(TypedDict):
    CostCategory: CostCategoryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CostCategoryTypeDef](./type_defs.md#costcategorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyRecommendationDetailTypeDef

```python
# ModifyRecommendationDetailTypeDef definition

class ModifyRecommendationDetailTypeDef(TypedDict):
    TargetInstances: NotRequired[List[TargetInstanceTypeDef]],  # (1)
```

1. See [:material-code-braces: TargetInstanceTypeDef](./type_defs.md#targetinstancetypedef) 
## GetReservationPurchaseRecommendationResponseTypeDef

```python
# GetReservationPurchaseRecommendationResponseTypeDef definition

class GetReservationPurchaseRecommendationResponseTypeDef(TypedDict):
    Metadata: ReservationPurchaseRecommendationMetadataTypeDef,  # (1)
    Recommendations: List[ReservationPurchaseRecommendationTypeDef],  # (2)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ReservationPurchaseRecommendationMetadataTypeDef](./type_defs.md#reservationpurchaserecommendationmetadatatypedef) 
2. See [:material-code-braces: ReservationPurchaseRecommendationTypeDef](./type_defs.md#reservationpurchaserecommendationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AnomalyMonitorTypeDef

```python
# AnomalyMonitorTypeDef definition

class AnomalyMonitorTypeDef(TypedDict):
    MonitorName: str,
    MonitorType: MonitorTypeType,  # (1)
    MonitorArn: NotRequired[str],
    CreationDate: NotRequired[str],
    LastUpdatedDate: NotRequired[str],
    LastEvaluatedDate: NotRequired[str],
    MonitorDimension: NotRequired[MonitorDimensionType],  # (2)
    MonitorSpecification: NotRequired[ExpressionUnionTypeDef],  # (3)
    DimensionalValueCount: NotRequired[int],
```

1. See [:material-code-brackets: MonitorTypeType](./literals.md#monitortypetype) 
2. See [:material-code-brackets: MonitorDimensionType](./literals.md#monitordimensiontype) 
3. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) [:material-code-braces: ExpressionOutputTypeDef](./type_defs.md#expressionoutputtypedef) 
## AnomalySubscriptionTypeDef

```python
# AnomalySubscriptionTypeDef definition

class AnomalySubscriptionTypeDef(TypedDict):
    MonitorArnList: Sequence[str],
    Subscribers: Sequence[SubscriberTypeDef],  # (1)
    Frequency: AnomalySubscriptionFrequencyType,  # (2)
    SubscriptionName: str,
    SubscriptionArn: NotRequired[str],
    AccountId: NotRequired[str],
    Threshold: NotRequired[float],
    ThresholdExpression: NotRequired[ExpressionUnionTypeDef],  # (3)
```

1. See [:material-code-braces: SubscriberTypeDef](./type_defs.md#subscribertypedef) 
2. See [:material-code-brackets: AnomalySubscriptionFrequencyType](./literals.md#anomalysubscriptionfrequencytype) 
3. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) [:material-code-braces: ExpressionOutputTypeDef](./type_defs.md#expressionoutputtypedef) 
## CostCategoryRuleTypeDef

```python
# CostCategoryRuleTypeDef definition

class CostCategoryRuleTypeDef(TypedDict):
    Value: NotRequired[str],
    Rule: NotRequired[ExpressionUnionTypeDef],  # (1)
    InheritedValue: NotRequired[CostCategoryInheritedValueDimensionTypeDef],  # (2)
    Type: NotRequired[CostCategoryRuleTypeType],  # (3)
```

1. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) [:material-code-braces: ExpressionOutputTypeDef](./type_defs.md#expressionoutputtypedef) 
2. See [:material-code-braces: CostCategoryInheritedValueDimensionTypeDef](./type_defs.md#costcategoryinheritedvaluedimensiontypedef) 
3. See [:material-code-brackets: CostCategoryRuleTypeType](./literals.md#costcategoryruletypetype) 
## RightsizingRecommendationTypeDef

```python
# RightsizingRecommendationTypeDef definition

class RightsizingRecommendationTypeDef(TypedDict):
    AccountId: NotRequired[str],
    CurrentInstance: NotRequired[CurrentInstanceTypeDef],  # (1)
    RightsizingType: NotRequired[RightsizingTypeType],  # (2)
    ModifyRecommendationDetail: NotRequired[ModifyRecommendationDetailTypeDef],  # (3)
    TerminateRecommendationDetail: NotRequired[TerminateRecommendationDetailTypeDef],  # (4)
    FindingReasonCodes: NotRequired[List[FindingReasonCodeType]],  # (5)
```

1. See [:material-code-braces: CurrentInstanceTypeDef](./type_defs.md#currentinstancetypedef) 
2. See [:material-code-brackets: RightsizingTypeType](./literals.md#rightsizingtypetype) 
3. See [:material-code-braces: ModifyRecommendationDetailTypeDef](./type_defs.md#modifyrecommendationdetailtypedef) 
4. See [:material-code-braces: TerminateRecommendationDetailTypeDef](./type_defs.md#terminaterecommendationdetailtypedef) 
5. See [:material-code-brackets: FindingReasonCodeType](./literals.md#findingreasoncodetype) 
## CreateAnomalyMonitorRequestRequestTypeDef

```python
# CreateAnomalyMonitorRequestRequestTypeDef definition

class CreateAnomalyMonitorRequestRequestTypeDef(TypedDict):
    AnomalyMonitor: AnomalyMonitorTypeDef,  # (1)
    ResourceTags: NotRequired[Sequence[ResourceTagTypeDef]],  # (2)
```

1. See [:material-code-braces: AnomalyMonitorTypeDef](./type_defs.md#anomalymonitortypedef) 
2. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
## CreateAnomalySubscriptionRequestRequestTypeDef

```python
# CreateAnomalySubscriptionRequestRequestTypeDef definition

class CreateAnomalySubscriptionRequestRequestTypeDef(TypedDict):
    AnomalySubscription: AnomalySubscriptionTypeDef,  # (1)
    ResourceTags: NotRequired[Sequence[ResourceTagTypeDef]],  # (2)
```

1. See [:material-code-braces: AnomalySubscriptionTypeDef](./type_defs.md#anomalysubscriptiontypedef) 
2. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
## UpdateCostCategoryDefinitionRequestRequestTypeDef

```python
# UpdateCostCategoryDefinitionRequestRequestTypeDef definition

class UpdateCostCategoryDefinitionRequestRequestTypeDef(TypedDict):
    CostCategoryArn: str,
    RuleVersion: CostCategoryRuleVersionType,  # (1)
    Rules: Sequence[CostCategoryRuleTypeDef],  # (2)
    EffectiveStart: NotRequired[str],
    DefaultValue: NotRequired[str],
    SplitChargeRules: NotRequired[Sequence[CostCategorySplitChargeRuleTypeDef]],  # (3)
```

1. See [:material-code-brackets: CostCategoryRuleVersionType](./literals.md#costcategoryruleversiontype) 
2. See [:material-code-braces: CostCategoryRuleTypeDef](./type_defs.md#costcategoryruletypedef) 
3. See [:material-code-braces: CostCategorySplitChargeRuleTypeDef](./type_defs.md#costcategorysplitchargeruletypedef) 
## GetRightsizingRecommendationResponseTypeDef

```python
# GetRightsizingRecommendationResponseTypeDef definition

class GetRightsizingRecommendationResponseTypeDef(TypedDict):
    Metadata: RightsizingRecommendationMetadataTypeDef,  # (1)
    Summary: RightsizingRecommendationSummaryTypeDef,  # (2)
    RightsizingRecommendations: List[RightsizingRecommendationTypeDef],  # (3)
    NextPageToken: str,
    Configuration: RightsizingRecommendationConfigurationTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: RightsizingRecommendationMetadataTypeDef](./type_defs.md#rightsizingrecommendationmetadatatypedef) 
2. See [:material-code-braces: RightsizingRecommendationSummaryTypeDef](./type_defs.md#rightsizingrecommendationsummarytypedef) 
3. See [:material-code-braces: RightsizingRecommendationTypeDef](./type_defs.md#rightsizingrecommendationtypedef) 
4. See [:material-code-braces: RightsizingRecommendationConfigurationTypeDef](./type_defs.md#rightsizingrecommendationconfigurationtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCostCategoryDefinitionRequestRequestTypeDef

```python
# CreateCostCategoryDefinitionRequestRequestTypeDef definition

class CreateCostCategoryDefinitionRequestRequestTypeDef(TypedDict):
    Name: str,
    RuleVersion: CostCategoryRuleVersionType,  # (1)
    Rules: Sequence[CostCategoryRuleUnionTypeDef],  # (2)
    EffectiveStart: NotRequired[str],
    DefaultValue: NotRequired[str],
    SplitChargeRules: NotRequired[Sequence[CostCategorySplitChargeRuleUnionTypeDef]],  # (3)
    ResourceTags: NotRequired[Sequence[ResourceTagTypeDef]],  # (4)
```

1. See [:material-code-brackets: CostCategoryRuleVersionType](./literals.md#costcategoryruleversiontype) 
2. See [:material-code-braces: CostCategoryRuleTypeDef](./type_defs.md#costcategoryruletypedef) [:material-code-braces: CostCategoryRuleOutputTypeDef](./type_defs.md#costcategoryruleoutputtypedef) 
3. See [:material-code-braces: CostCategorySplitChargeRuleTypeDef](./type_defs.md#costcategorysplitchargeruletypedef) [:material-code-braces: CostCategorySplitChargeRuleOutputTypeDef](./type_defs.md#costcategorysplitchargeruleoutputtypedef) 
4. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
