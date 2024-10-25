# Type definitions

> [Index](../README.md) > [CostOptimizationHub](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CostOptimizationHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub)
    type annotations stubs module [types-aiobotocore-cost-optimization-hub](https://pypi.org/project/types-aiobotocore-cost-optimization-hub/).



## AccountEnrollmentStatusTypeDef

```python
# AccountEnrollmentStatusTypeDef definition

class AccountEnrollmentStatusTypeDef(TypedDict):
    accountId: NotRequired[str],
    status: NotRequired[EnrollmentStatusType],  # (1)
    lastUpdatedTimestamp: NotRequired[datetime],
    createdTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: EnrollmentStatusType](./literals.md#enrollmentstatustype) 
## BlockStoragePerformanceConfigurationTypeDef

```python
# BlockStoragePerformanceConfigurationTypeDef definition

class BlockStoragePerformanceConfigurationTypeDef(TypedDict):
    iops: NotRequired[float],
    throughput: NotRequired[float],
```

## ComputeConfigurationTypeDef

```python
# ComputeConfigurationTypeDef definition

class ComputeConfigurationTypeDef(TypedDict):
    vCpu: NotRequired[float],
    memorySizeInMB: NotRequired[int],
    architecture: NotRequired[str],
    platform: NotRequired[str],
```

## ComputeSavingsPlansConfigurationTypeDef

```python
# ComputeSavingsPlansConfigurationTypeDef definition

class ComputeSavingsPlansConfigurationTypeDef(TypedDict):
    accountScope: NotRequired[str],
    term: NotRequired[str],
    paymentOption: NotRequired[str],
    hourlyCommitment: NotRequired[str],
```

## DbInstanceConfigurationTypeDef

```python
# DbInstanceConfigurationTypeDef definition

class DbInstanceConfigurationTypeDef(TypedDict):
    dbInstanceClass: NotRequired[str],
```

## StorageConfigurationTypeDef

```python
# StorageConfigurationTypeDef definition

class StorageConfigurationTypeDef(TypedDict):
    type: NotRequired[str],
    sizeInGb: NotRequired[float],
```

## InstanceConfigurationTypeDef

```python
# InstanceConfigurationTypeDef definition

class InstanceConfigurationTypeDef(TypedDict):
    type: NotRequired[str],
```

## Ec2InstanceSavingsPlansConfigurationTypeDef

```python
# Ec2InstanceSavingsPlansConfigurationTypeDef definition

class Ec2InstanceSavingsPlansConfigurationTypeDef(TypedDict):
    accountScope: NotRequired[str],
    term: NotRequired[str],
    paymentOption: NotRequired[str],
    hourlyCommitment: NotRequired[str],
    instanceFamily: NotRequired[str],
    savingsPlansRegion: NotRequired[str],
```

## Ec2ReservedInstancesConfigurationTypeDef

```python
# Ec2ReservedInstancesConfigurationTypeDef definition

class Ec2ReservedInstancesConfigurationTypeDef(TypedDict):
    accountScope: NotRequired[str],
    service: NotRequired[str],
    normalizedUnitsToPurchase: NotRequired[str],
    term: NotRequired[str],
    paymentOption: NotRequired[str],
    numberOfInstancesToPurchase: NotRequired[str],
    offeringClass: NotRequired[str],
    instanceFamily: NotRequired[str],
    instanceType: NotRequired[str],
    reservedInstancesRegion: NotRequired[str],
    currentGeneration: NotRequired[str],
    platform: NotRequired[str],
    tenancy: NotRequired[str],
    sizeFlexEligible: NotRequired[bool],
    upfrontCost: NotRequired[str],
    monthlyRecurringCost: NotRequired[str],
```

## ElastiCacheReservedInstancesConfigurationTypeDef

```python
# ElastiCacheReservedInstancesConfigurationTypeDef definition

class ElastiCacheReservedInstancesConfigurationTypeDef(TypedDict):
    accountScope: NotRequired[str],
    service: NotRequired[str],
    normalizedUnitsToPurchase: NotRequired[str],
    term: NotRequired[str],
    paymentOption: NotRequired[str],
    numberOfInstancesToPurchase: NotRequired[str],
    instanceFamily: NotRequired[str],
    instanceType: NotRequired[str],
    reservedInstancesRegion: NotRequired[str],
    currentGeneration: NotRequired[str],
    sizeFlexEligible: NotRequired[bool],
    upfrontCost: NotRequired[str],
    monthlyRecurringCost: NotRequired[str],
```

## EstimatedDiscountsTypeDef

```python
# EstimatedDiscountsTypeDef definition

class EstimatedDiscountsTypeDef(TypedDict):
    savingsPlansDiscount: NotRequired[float],
    reservedInstancesDiscount: NotRequired[float],
    otherDiscount: NotRequired[float],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[str],
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

## GetRecommendationRequestRequestTypeDef

```python
# GetRecommendationRequestRequestTypeDef definition

class GetRecommendationRequestRequestTypeDef(TypedDict):
    recommendationId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListEnrollmentStatusesRequestRequestTypeDef

```python
# ListEnrollmentStatusesRequestRequestTypeDef definition

class ListEnrollmentStatusesRequestRequestTypeDef(TypedDict):
    includeOrganizationInfo: NotRequired[bool],
    accountId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## RecommendationSummaryTypeDef

```python
# RecommendationSummaryTypeDef definition

class RecommendationSummaryTypeDef(TypedDict):
    group: NotRequired[str],
    estimatedMonthlySavings: NotRequired[float],
    recommendationCount: NotRequired[int],
```

## SummaryMetricsResultTypeDef

```python
# SummaryMetricsResultTypeDef definition

class SummaryMetricsResultTypeDef(TypedDict):
    savingsPercentage: NotRequired[str],
```

## OrderByTypeDef

```python
# OrderByTypeDef definition

class OrderByTypeDef(TypedDict):
    dimension: NotRequired[str],
    order: NotRequired[OrderType],  # (1)
```

1. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
## OpenSearchReservedInstancesConfigurationTypeDef

```python
# OpenSearchReservedInstancesConfigurationTypeDef definition

class OpenSearchReservedInstancesConfigurationTypeDef(TypedDict):
    accountScope: NotRequired[str],
    service: NotRequired[str],
    normalizedUnitsToPurchase: NotRequired[str],
    term: NotRequired[str],
    paymentOption: NotRequired[str],
    numberOfInstancesToPurchase: NotRequired[str],
    instanceType: NotRequired[str],
    reservedInstancesRegion: NotRequired[str],
    currentGeneration: NotRequired[str],
    sizeFlexEligible: NotRequired[bool],
    upfrontCost: NotRequired[str],
    monthlyRecurringCost: NotRequired[str],
```

## RdsDbInstanceStorageConfigurationTypeDef

```python
# RdsDbInstanceStorageConfigurationTypeDef definition

class RdsDbInstanceStorageConfigurationTypeDef(TypedDict):
    storageType: NotRequired[str],
    allocatedStorageInGb: NotRequired[float],
    iops: NotRequired[float],
    storageThroughput: NotRequired[float],
```

## RdsReservedInstancesConfigurationTypeDef

```python
# RdsReservedInstancesConfigurationTypeDef definition

class RdsReservedInstancesConfigurationTypeDef(TypedDict):
    accountScope: NotRequired[str],
    service: NotRequired[str],
    normalizedUnitsToPurchase: NotRequired[str],
    term: NotRequired[str],
    paymentOption: NotRequired[str],
    numberOfInstancesToPurchase: NotRequired[str],
    instanceFamily: NotRequired[str],
    instanceType: NotRequired[str],
    reservedInstancesRegion: NotRequired[str],
    sizeFlexEligible: NotRequired[bool],
    currentGeneration: NotRequired[str],
    upfrontCost: NotRequired[str],
    monthlyRecurringCost: NotRequired[str],
    licenseModel: NotRequired[str],
    databaseEdition: NotRequired[str],
    databaseEngine: NotRequired[str],
    deploymentOption: NotRequired[str],
```

## RedshiftReservedInstancesConfigurationTypeDef

```python
# RedshiftReservedInstancesConfigurationTypeDef definition

class RedshiftReservedInstancesConfigurationTypeDef(TypedDict):
    accountScope: NotRequired[str],
    service: NotRequired[str],
    normalizedUnitsToPurchase: NotRequired[str],
    term: NotRequired[str],
    paymentOption: NotRequired[str],
    numberOfInstancesToPurchase: NotRequired[str],
    instanceFamily: NotRequired[str],
    instanceType: NotRequired[str],
    reservedInstancesRegion: NotRequired[str],
    sizeFlexEligible: NotRequired[bool],
    currentGeneration: NotRequired[str],
    upfrontCost: NotRequired[str],
    monthlyRecurringCost: NotRequired[str],
```

## ReservedInstancesPricingTypeDef

```python
# ReservedInstancesPricingTypeDef definition

class ReservedInstancesPricingTypeDef(TypedDict):
    estimatedOnDemandCost: NotRequired[float],
    monthlyReservationEligibleCost: NotRequired[float],
    savingsPercentage: NotRequired[float],
    estimatedMonthlyAmortizedReservationCost: NotRequired[float],
```

## UsageTypeDef

```python
# UsageTypeDef definition

class UsageTypeDef(TypedDict):
    usageType: NotRequired[str],
    usageAmount: NotRequired[float],
    operation: NotRequired[str],
    productCode: NotRequired[str],
    unit: NotRequired[str],
```

## SageMakerSavingsPlansConfigurationTypeDef

```python
# SageMakerSavingsPlansConfigurationTypeDef definition

class SageMakerSavingsPlansConfigurationTypeDef(TypedDict):
    accountScope: NotRequired[str],
    term: NotRequired[str],
    paymentOption: NotRequired[str],
    hourlyCommitment: NotRequired[str],
```

## SavingsPlansPricingTypeDef

```python
# SavingsPlansPricingTypeDef definition

class SavingsPlansPricingTypeDef(TypedDict):
    monthlySavingsPlansEligibleCost: NotRequired[float],
    estimatedMonthlyCommitment: NotRequired[float],
    savingsPercentage: NotRequired[float],
    estimatedOnDemandCost: NotRequired[float],
```

## UpdateEnrollmentStatusRequestRequestTypeDef

```python
# UpdateEnrollmentStatusRequestRequestTypeDef definition

class UpdateEnrollmentStatusRequestRequestTypeDef(TypedDict):
    status: EnrollmentStatusType,  # (1)
    includeMemberAccounts: NotRequired[bool],
```

1. See [:material-code-brackets: EnrollmentStatusType](./literals.md#enrollmentstatustype) 
## UpdatePreferencesRequestRequestTypeDef

```python
# UpdatePreferencesRequestRequestTypeDef definition

class UpdatePreferencesRequestRequestTypeDef(TypedDict):
    savingsEstimationMode: NotRequired[SavingsEstimationModeType],  # (1)
    memberAccountDiscountVisibility: NotRequired[MemberAccountDiscountVisibilityType],  # (2)
```

1. See [:material-code-brackets: SavingsEstimationModeType](./literals.md#savingsestimationmodetype) 
2. See [:material-code-brackets: MemberAccountDiscountVisibilityType](./literals.md#memberaccountdiscountvisibilitytype) 
## EcsServiceConfigurationTypeDef

```python
# EcsServiceConfigurationTypeDef definition

class EcsServiceConfigurationTypeDef(TypedDict):
    compute: NotRequired[ComputeConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ComputeConfigurationTypeDef](./type_defs.md#computeconfigurationtypedef) 
## LambdaFunctionConfigurationTypeDef

```python
# LambdaFunctionConfigurationTypeDef definition

class LambdaFunctionConfigurationTypeDef(TypedDict):
    compute: NotRequired[ComputeConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ComputeConfigurationTypeDef](./type_defs.md#computeconfigurationtypedef) 
## RdsDbInstanceConfigurationTypeDef

```python
# RdsDbInstanceConfigurationTypeDef definition

class RdsDbInstanceConfigurationTypeDef(TypedDict):
    instance: NotRequired[DbInstanceConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: DbInstanceConfigurationTypeDef](./type_defs.md#dbinstanceconfigurationtypedef) 
## EbsVolumeConfigurationTypeDef

```python
# EbsVolumeConfigurationTypeDef definition

class EbsVolumeConfigurationTypeDef(TypedDict):
    storage: NotRequired[StorageConfigurationTypeDef],  # (1)
    performance: NotRequired[BlockStoragePerformanceConfigurationTypeDef],  # (2)
    attachmentState: NotRequired[str],
```

1. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef) 
2. See [:material-code-braces: BlockStoragePerformanceConfigurationTypeDef](./type_defs.md#blockstorageperformanceconfigurationtypedef) 
## Ec2AutoScalingGroupConfigurationTypeDef

```python
# Ec2AutoScalingGroupConfigurationTypeDef definition

class Ec2AutoScalingGroupConfigurationTypeDef(TypedDict):
    instance: NotRequired[InstanceConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: InstanceConfigurationTypeDef](./type_defs.md#instanceconfigurationtypedef) 
## Ec2InstanceConfigurationTypeDef

```python
# Ec2InstanceConfigurationTypeDef definition

class Ec2InstanceConfigurationTypeDef(TypedDict):
    instance: NotRequired[InstanceConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: InstanceConfigurationTypeDef](./type_defs.md#instanceconfigurationtypedef) 
## ResourcePricingTypeDef

```python
# ResourcePricingTypeDef definition

class ResourcePricingTypeDef(TypedDict):
    estimatedCostBeforeDiscounts: NotRequired[float],
    estimatedNetUnusedAmortizedCommitments: NotRequired[float],
    estimatedDiscounts: NotRequired[EstimatedDiscountsTypeDef],  # (1)
    estimatedCostAfterDiscounts: NotRequired[float],
```

1. See [:material-code-braces: EstimatedDiscountsTypeDef](./type_defs.md#estimateddiscountstypedef) 
## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    restartNeeded: NotRequired[bool],
    rollbackPossible: NotRequired[bool],
    implementationEfforts: NotRequired[Sequence[ImplementationEffortType]],  # (1)
    accountIds: NotRequired[Sequence[str]],
    regions: NotRequired[Sequence[str]],
    resourceTypes: NotRequired[Sequence[ResourceTypeType]],  # (2)
    actionTypes: NotRequired[Sequence[ActionTypeType]],  # (3)
    tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    resourceIds: NotRequired[Sequence[str]],
    resourceArns: NotRequired[Sequence[str]],
    recommendationIds: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: ImplementationEffortType](./literals.md#implementationefforttype) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## RecommendationTypeDef

```python
# RecommendationTypeDef definition

class RecommendationTypeDef(TypedDict):
    recommendationId: NotRequired[str],
    accountId: NotRequired[str],
    region: NotRequired[str],
    resourceId: NotRequired[str],
    resourceArn: NotRequired[str],
    currentResourceType: NotRequired[str],
    recommendedResourceType: NotRequired[str],
    estimatedMonthlySavings: NotRequired[float],
    estimatedSavingsPercentage: NotRequired[float],
    estimatedMonthlyCost: NotRequired[float],
    currencyCode: NotRequired[str],
    implementationEffort: NotRequired[str],
    restartNeeded: NotRequired[bool],
    actionType: NotRequired[str],
    rollbackPossible: NotRequired[bool],
    currentResourceSummary: NotRequired[str],
    recommendedResourceSummary: NotRequired[str],
    lastRefreshTimestamp: NotRequired[datetime],
    recommendationLookbackPeriodInDays: NotRequired[int],
    source: NotRequired[SourceType],  # (1)
    tags: NotRequired[List[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: SourceType](./literals.md#sourcetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetPreferencesResponseTypeDef

```python
# GetPreferencesResponseTypeDef definition

class GetPreferencesResponseTypeDef(TypedDict):
    savingsEstimationMode: SavingsEstimationModeType,  # (1)
    memberAccountDiscountVisibility: MemberAccountDiscountVisibilityType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: SavingsEstimationModeType](./literals.md#savingsestimationmodetype) 
2. See [:material-code-brackets: MemberAccountDiscountVisibilityType](./literals.md#memberaccountdiscountvisibilitytype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnrollmentStatusesResponseTypeDef

```python
# ListEnrollmentStatusesResponseTypeDef definition

class ListEnrollmentStatusesResponseTypeDef(TypedDict):
    items: List[AccountEnrollmentStatusTypeDef],  # (1)
    includeMemberAccounts: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AccountEnrollmentStatusTypeDef](./type_defs.md#accountenrollmentstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEnrollmentStatusResponseTypeDef

```python
# UpdateEnrollmentStatusResponseTypeDef definition

class UpdateEnrollmentStatusResponseTypeDef(TypedDict):
    status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePreferencesResponseTypeDef

```python
# UpdatePreferencesResponseTypeDef definition

class UpdatePreferencesResponseTypeDef(TypedDict):
    savingsEstimationMode: SavingsEstimationModeType,  # (1)
    memberAccountDiscountVisibility: MemberAccountDiscountVisibilityType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: SavingsEstimationModeType](./literals.md#savingsestimationmodetype) 
2. See [:material-code-brackets: MemberAccountDiscountVisibilityType](./literals.md#memberaccountdiscountvisibilitytype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnrollmentStatusesRequestListEnrollmentStatusesPaginateTypeDef

```python
# ListEnrollmentStatusesRequestListEnrollmentStatusesPaginateTypeDef definition

class ListEnrollmentStatusesRequestListEnrollmentStatusesPaginateTypeDef(TypedDict):
    includeOrganizationInfo: NotRequired[bool],
    accountId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecommendationSummariesResponseTypeDef

```python
# ListRecommendationSummariesResponseTypeDef definition

class ListRecommendationSummariesResponseTypeDef(TypedDict):
    estimatedTotalDedupedSavings: float,
    items: List[RecommendationSummaryTypeDef],  # (1)
    groupBy: str,
    currencyCode: str,
    metrics: SummaryMetricsResultTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RecommendationSummaryTypeDef](./type_defs.md#recommendationsummarytypedef) 
2. See [:material-code-braces: SummaryMetricsResultTypeDef](./type_defs.md#summarymetricsresulttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReservedInstancesCostCalculationTypeDef

```python
# ReservedInstancesCostCalculationTypeDef definition

class ReservedInstancesCostCalculationTypeDef(TypedDict):
    pricing: NotRequired[ReservedInstancesPricingTypeDef],  # (1)
```

1. See [:material-code-braces: ReservedInstancesPricingTypeDef](./type_defs.md#reservedinstancespricingtypedef) 
## SavingsPlansCostCalculationTypeDef

```python
# SavingsPlansCostCalculationTypeDef definition

class SavingsPlansCostCalculationTypeDef(TypedDict):
    pricing: NotRequired[SavingsPlansPricingTypeDef],  # (1)
```

1. See [:material-code-braces: SavingsPlansPricingTypeDef](./type_defs.md#savingsplanspricingtypedef) 
## ResourceCostCalculationTypeDef

```python
# ResourceCostCalculationTypeDef definition

class ResourceCostCalculationTypeDef(TypedDict):
    usages: NotRequired[List[UsageTypeDef]],  # (1)
    pricing: NotRequired[ResourcePricingTypeDef],  # (2)
```

1. See [:material-code-braces: UsageTypeDef](./type_defs.md#usagetypedef) 
2. See [:material-code-braces: ResourcePricingTypeDef](./type_defs.md#resourcepricingtypedef) 
## ListRecommendationSummariesRequestListRecommendationSummariesPaginateTypeDef

```python
# ListRecommendationSummariesRequestListRecommendationSummariesPaginateTypeDef definition

class ListRecommendationSummariesRequestListRecommendationSummariesPaginateTypeDef(TypedDict):
    groupBy: str,
    filter: NotRequired[FilterTypeDef],  # (1)
    metrics: NotRequired[Sequence[SummaryMetricsType]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: SummaryMetricsType](./literals.md#summarymetricstype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecommendationSummariesRequestRequestTypeDef

```python
# ListRecommendationSummariesRequestRequestTypeDef definition

class ListRecommendationSummariesRequestRequestTypeDef(TypedDict):
    groupBy: str,
    filter: NotRequired[FilterTypeDef],  # (1)
    maxResults: NotRequired[int],
    metrics: NotRequired[Sequence[SummaryMetricsType]],  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: SummaryMetricsType](./literals.md#summarymetricstype) 
## ListRecommendationsRequestListRecommendationsPaginateTypeDef

```python
# ListRecommendationsRequestListRecommendationsPaginateTypeDef definition

class ListRecommendationsRequestListRecommendationsPaginateTypeDef(TypedDict):
    filter: NotRequired[FilterTypeDef],  # (1)
    orderBy: NotRequired[OrderByTypeDef],  # (2)
    includeAllRecommendations: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: OrderByTypeDef](./type_defs.md#orderbytypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecommendationsRequestRequestTypeDef

```python
# ListRecommendationsRequestRequestTypeDef definition

class ListRecommendationsRequestRequestTypeDef(TypedDict):
    filter: NotRequired[FilterTypeDef],  # (1)
    orderBy: NotRequired[OrderByTypeDef],  # (2)
    includeAllRecommendations: NotRequired[bool],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: OrderByTypeDef](./type_defs.md#orderbytypedef) 
## ListRecommendationsResponseTypeDef

```python
# ListRecommendationsResponseTypeDef definition

class ListRecommendationsResponseTypeDef(TypedDict):
    items: List[RecommendationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RecommendationTypeDef](./type_defs.md#recommendationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## Ec2ReservedInstancesTypeDef

```python
# Ec2ReservedInstancesTypeDef definition

class Ec2ReservedInstancesTypeDef(TypedDict):
    configuration: NotRequired[Ec2ReservedInstancesConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[ReservedInstancesCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: Ec2ReservedInstancesConfigurationTypeDef](./type_defs.md#ec2reservedinstancesconfigurationtypedef) 
2. See [:material-code-braces: ReservedInstancesCostCalculationTypeDef](./type_defs.md#reservedinstancescostcalculationtypedef) 
## ElastiCacheReservedInstancesTypeDef

```python
# ElastiCacheReservedInstancesTypeDef definition

class ElastiCacheReservedInstancesTypeDef(TypedDict):
    configuration: NotRequired[ElastiCacheReservedInstancesConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[ReservedInstancesCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: ElastiCacheReservedInstancesConfigurationTypeDef](./type_defs.md#elasticachereservedinstancesconfigurationtypedef) 
2. See [:material-code-braces: ReservedInstancesCostCalculationTypeDef](./type_defs.md#reservedinstancescostcalculationtypedef) 
## OpenSearchReservedInstancesTypeDef

```python
# OpenSearchReservedInstancesTypeDef definition

class OpenSearchReservedInstancesTypeDef(TypedDict):
    configuration: NotRequired[OpenSearchReservedInstancesConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[ReservedInstancesCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: OpenSearchReservedInstancesConfigurationTypeDef](./type_defs.md#opensearchreservedinstancesconfigurationtypedef) 
2. See [:material-code-braces: ReservedInstancesCostCalculationTypeDef](./type_defs.md#reservedinstancescostcalculationtypedef) 
## RdsReservedInstancesTypeDef

```python
# RdsReservedInstancesTypeDef definition

class RdsReservedInstancesTypeDef(TypedDict):
    configuration: NotRequired[RdsReservedInstancesConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[ReservedInstancesCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: RdsReservedInstancesConfigurationTypeDef](./type_defs.md#rdsreservedinstancesconfigurationtypedef) 
2. See [:material-code-braces: ReservedInstancesCostCalculationTypeDef](./type_defs.md#reservedinstancescostcalculationtypedef) 
## RedshiftReservedInstancesTypeDef

```python
# RedshiftReservedInstancesTypeDef definition

class RedshiftReservedInstancesTypeDef(TypedDict):
    configuration: NotRequired[RedshiftReservedInstancesConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[ReservedInstancesCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: RedshiftReservedInstancesConfigurationTypeDef](./type_defs.md#redshiftreservedinstancesconfigurationtypedef) 
2. See [:material-code-braces: ReservedInstancesCostCalculationTypeDef](./type_defs.md#reservedinstancescostcalculationtypedef) 
## ComputeSavingsPlansTypeDef

```python
# ComputeSavingsPlansTypeDef definition

class ComputeSavingsPlansTypeDef(TypedDict):
    configuration: NotRequired[ComputeSavingsPlansConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[SavingsPlansCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: ComputeSavingsPlansConfigurationTypeDef](./type_defs.md#computesavingsplansconfigurationtypedef) 
2. See [:material-code-braces: SavingsPlansCostCalculationTypeDef](./type_defs.md#savingsplanscostcalculationtypedef) 
## Ec2InstanceSavingsPlansTypeDef

```python
# Ec2InstanceSavingsPlansTypeDef definition

class Ec2InstanceSavingsPlansTypeDef(TypedDict):
    configuration: NotRequired[Ec2InstanceSavingsPlansConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[SavingsPlansCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: Ec2InstanceSavingsPlansConfigurationTypeDef](./type_defs.md#ec2instancesavingsplansconfigurationtypedef) 
2. See [:material-code-braces: SavingsPlansCostCalculationTypeDef](./type_defs.md#savingsplanscostcalculationtypedef) 
## SageMakerSavingsPlansTypeDef

```python
# SageMakerSavingsPlansTypeDef definition

class SageMakerSavingsPlansTypeDef(TypedDict):
    configuration: NotRequired[SageMakerSavingsPlansConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[SavingsPlansCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: SageMakerSavingsPlansConfigurationTypeDef](./type_defs.md#sagemakersavingsplansconfigurationtypedef) 
2. See [:material-code-braces: SavingsPlansCostCalculationTypeDef](./type_defs.md#savingsplanscostcalculationtypedef) 
## EbsVolumeTypeDef

```python
# EbsVolumeTypeDef definition

class EbsVolumeTypeDef(TypedDict):
    configuration: NotRequired[EbsVolumeConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[ResourceCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: EbsVolumeConfigurationTypeDef](./type_defs.md#ebsvolumeconfigurationtypedef) 
2. See [:material-code-braces: ResourceCostCalculationTypeDef](./type_defs.md#resourcecostcalculationtypedef) 
## Ec2AutoScalingGroupTypeDef

```python
# Ec2AutoScalingGroupTypeDef definition

class Ec2AutoScalingGroupTypeDef(TypedDict):
    configuration: NotRequired[Ec2AutoScalingGroupConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[ResourceCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: Ec2AutoScalingGroupConfigurationTypeDef](./type_defs.md#ec2autoscalinggroupconfigurationtypedef) 
2. See [:material-code-braces: ResourceCostCalculationTypeDef](./type_defs.md#resourcecostcalculationtypedef) 
## Ec2InstanceTypeDef

```python
# Ec2InstanceTypeDef definition

class Ec2InstanceTypeDef(TypedDict):
    configuration: NotRequired[Ec2InstanceConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[ResourceCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: Ec2InstanceConfigurationTypeDef](./type_defs.md#ec2instanceconfigurationtypedef) 
2. See [:material-code-braces: ResourceCostCalculationTypeDef](./type_defs.md#resourcecostcalculationtypedef) 
## EcsServiceTypeDef

```python
# EcsServiceTypeDef definition

class EcsServiceTypeDef(TypedDict):
    configuration: NotRequired[EcsServiceConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[ResourceCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: EcsServiceConfigurationTypeDef](./type_defs.md#ecsserviceconfigurationtypedef) 
2. See [:material-code-braces: ResourceCostCalculationTypeDef](./type_defs.md#resourcecostcalculationtypedef) 
## LambdaFunctionTypeDef

```python
# LambdaFunctionTypeDef definition

class LambdaFunctionTypeDef(TypedDict):
    configuration: NotRequired[LambdaFunctionConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[ResourceCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: LambdaFunctionConfigurationTypeDef](./type_defs.md#lambdafunctionconfigurationtypedef) 
2. See [:material-code-braces: ResourceCostCalculationTypeDef](./type_defs.md#resourcecostcalculationtypedef) 
## RdsDbInstanceStorageTypeDef

```python
# RdsDbInstanceStorageTypeDef definition

class RdsDbInstanceStorageTypeDef(TypedDict):
    configuration: NotRequired[RdsDbInstanceStorageConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[ResourceCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: RdsDbInstanceStorageConfigurationTypeDef](./type_defs.md#rdsdbinstancestorageconfigurationtypedef) 
2. See [:material-code-braces: ResourceCostCalculationTypeDef](./type_defs.md#resourcecostcalculationtypedef) 
## RdsDbInstanceTypeDef

```python
# RdsDbInstanceTypeDef definition

class RdsDbInstanceTypeDef(TypedDict):
    configuration: NotRequired[RdsDbInstanceConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[ResourceCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: RdsDbInstanceConfigurationTypeDef](./type_defs.md#rdsdbinstanceconfigurationtypedef) 
2. See [:material-code-braces: ResourceCostCalculationTypeDef](./type_defs.md#resourcecostcalculationtypedef) 
## ResourceDetailsTypeDef

```python
# ResourceDetailsTypeDef definition

class ResourceDetailsTypeDef(TypedDict):
    lambdaFunction: NotRequired[LambdaFunctionTypeDef],  # (1)
    ecsService: NotRequired[EcsServiceTypeDef],  # (2)
    ec2Instance: NotRequired[Ec2InstanceTypeDef],  # (3)
    ebsVolume: NotRequired[EbsVolumeTypeDef],  # (4)
    ec2AutoScalingGroup: NotRequired[Ec2AutoScalingGroupTypeDef],  # (5)
    ec2ReservedInstances: NotRequired[Ec2ReservedInstancesTypeDef],  # (6)
    rdsReservedInstances: NotRequired[RdsReservedInstancesTypeDef],  # (7)
    elastiCacheReservedInstances: NotRequired[ElastiCacheReservedInstancesTypeDef],  # (8)
    openSearchReservedInstances: NotRequired[OpenSearchReservedInstancesTypeDef],  # (9)
    redshiftReservedInstances: NotRequired[RedshiftReservedInstancesTypeDef],  # (10)
    ec2InstanceSavingsPlans: NotRequired[Ec2InstanceSavingsPlansTypeDef],  # (11)
    computeSavingsPlans: NotRequired[ComputeSavingsPlansTypeDef],  # (12)
    sageMakerSavingsPlans: NotRequired[SageMakerSavingsPlansTypeDef],  # (13)
    rdsDbInstance: NotRequired[RdsDbInstanceTypeDef],  # (14)
    rdsDbInstanceStorage: NotRequired[RdsDbInstanceStorageTypeDef],  # (15)
```

1. See [:material-code-braces: LambdaFunctionTypeDef](./type_defs.md#lambdafunctiontypedef) 
2. See [:material-code-braces: EcsServiceTypeDef](./type_defs.md#ecsservicetypedef) 
3. See [:material-code-braces: Ec2InstanceTypeDef](./type_defs.md#ec2instancetypedef) 
4. See [:material-code-braces: EbsVolumeTypeDef](./type_defs.md#ebsvolumetypedef) 
5. See [:material-code-braces: Ec2AutoScalingGroupTypeDef](./type_defs.md#ec2autoscalinggrouptypedef) 
6. See [:material-code-braces: Ec2ReservedInstancesTypeDef](./type_defs.md#ec2reservedinstancestypedef) 
7. See [:material-code-braces: RdsReservedInstancesTypeDef](./type_defs.md#rdsreservedinstancestypedef) 
8. See [:material-code-braces: ElastiCacheReservedInstancesTypeDef](./type_defs.md#elasticachereservedinstancestypedef) 
9. See [:material-code-braces: OpenSearchReservedInstancesTypeDef](./type_defs.md#opensearchreservedinstancestypedef) 
10. See [:material-code-braces: RedshiftReservedInstancesTypeDef](./type_defs.md#redshiftreservedinstancestypedef) 
11. See [:material-code-braces: Ec2InstanceSavingsPlansTypeDef](./type_defs.md#ec2instancesavingsplanstypedef) 
12. See [:material-code-braces: ComputeSavingsPlansTypeDef](./type_defs.md#computesavingsplanstypedef) 
13. See [:material-code-braces: SageMakerSavingsPlansTypeDef](./type_defs.md#sagemakersavingsplanstypedef) 
14. See [:material-code-braces: RdsDbInstanceTypeDef](./type_defs.md#rdsdbinstancetypedef) 
15. See [:material-code-braces: RdsDbInstanceStorageTypeDef](./type_defs.md#rdsdbinstancestoragetypedef) 
## GetRecommendationResponseTypeDef

```python
# GetRecommendationResponseTypeDef definition

class GetRecommendationResponseTypeDef(TypedDict):
    recommendationId: str,
    resourceId: str,
    resourceArn: str,
    accountId: str,
    currencyCode: str,
    recommendationLookbackPeriodInDays: int,
    costCalculationLookbackPeriodInDays: int,
    estimatedSavingsPercentage: float,
    estimatedSavingsOverCostCalculationLookbackPeriod: float,
    currentResourceType: ResourceTypeType,  # (1)
    recommendedResourceType: ResourceTypeType,  # (1)
    region: str,
    source: SourceType,  # (3)
    lastRefreshTimestamp: datetime,
    estimatedMonthlySavings: float,
    estimatedMonthlyCost: float,
    implementationEffort: ImplementationEffortType,  # (4)
    restartNeeded: bool,
    actionType: ActionTypeType,  # (5)
    rollbackPossible: bool,
    currentResourceDetails: ResourceDetailsTypeDef,  # (6)
    recommendedResourceDetails: ResourceDetailsTypeDef,  # (6)
    tags: List[TagTypeDef],  # (8)
    ResponseMetadata: ResponseMetadataTypeDef,  # (9)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-brackets: SourceType](./literals.md#sourcetype) 
4. See [:material-code-brackets: ImplementationEffortType](./literals.md#implementationefforttype) 
5. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
6. See [:material-code-braces: ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef) 
7. See [:material-code-braces: ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
9. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
