# Type definitions

> [Index](../README.md) > [ComputeOptimizer](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ComputeOptimizer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
    type annotations stubs module [types-aiobotocore-compute-optimizer](https://pypi.org/project/types-aiobotocore-compute-optimizer/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AccountEnrollmentStatusTypeDef

```python
# AccountEnrollmentStatusTypeDef definition

class AccountEnrollmentStatusTypeDef(TypedDict):
    accountId: NotRequired[str],
    status: NotRequired[StatusType],  # (1)
    statusReason: NotRequired[str],
    lastUpdatedTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## AutoScalingGroupConfigurationTypeDef

```python
# AutoScalingGroupConfigurationTypeDef definition

class AutoScalingGroupConfigurationTypeDef(TypedDict):
    desiredCapacity: NotRequired[int],
    minSize: NotRequired[int],
    maxSize: NotRequired[int],
    instanceType: NotRequired[str],
```

## AutoScalingGroupEstimatedMonthlySavingsTypeDef

```python
# AutoScalingGroupEstimatedMonthlySavingsTypeDef definition

class AutoScalingGroupEstimatedMonthlySavingsTypeDef(TypedDict):
    currency: NotRequired[CurrencyType],  # (1)
    value: NotRequired[float],
```

1. See [:material-code-brackets: CurrencyType](./literals.md#currencytype) 
## UtilizationMetricTypeDef

```python
# UtilizationMetricTypeDef definition

class UtilizationMetricTypeDef(TypedDict):
    name: NotRequired[MetricNameType],  # (1)
    statistic: NotRequired[MetricStatisticType],  # (2)
    value: NotRequired[float],
```

1. See [:material-code-brackets: MetricNameType](./literals.md#metricnametype) 
2. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
## MemorySizeConfigurationTypeDef

```python
# MemorySizeConfigurationTypeDef definition

class MemorySizeConfigurationTypeDef(TypedDict):
    memory: NotRequired[int],
    memoryReservation: NotRequired[int],
```

## CurrentPerformanceRiskRatingsTypeDef

```python
# CurrentPerformanceRiskRatingsTypeDef definition

class CurrentPerformanceRiskRatingsTypeDef(TypedDict):
    high: NotRequired[int],
    medium: NotRequired[int],
    low: NotRequired[int],
    veryLow: NotRequired[int],
```

## CustomizableMetricParametersTypeDef

```python
# CustomizableMetricParametersTypeDef definition

class CustomizableMetricParametersTypeDef(TypedDict):
    threshold: NotRequired[CustomizableMetricThresholdType],  # (1)
    headroom: NotRequired[CustomizableMetricHeadroomType],  # (2)
```

1. See [:material-code-brackets: CustomizableMetricThresholdType](./literals.md#customizablemetricthresholdtype) 
2. See [:material-code-brackets: CustomizableMetricHeadroomType](./literals.md#customizablemetricheadroomtype) 
## DBStorageConfigurationTypeDef

```python
# DBStorageConfigurationTypeDef definition

class DBStorageConfigurationTypeDef(TypedDict):
    storageType: NotRequired[str],
    allocatedStorage: NotRequired[int],
    iops: NotRequired[int],
    maxAllocatedStorage: NotRequired[int],
    storageThroughput: NotRequired[int],
```

## ScopeTypeDef

```python
# ScopeTypeDef definition

class ScopeTypeDef(TypedDict):
    name: NotRequired[ScopeNameType],  # (1)
    value: NotRequired[str],
```

1. See [:material-code-brackets: ScopeNameType](./literals.md#scopenametype) 
## JobFilterTypeDef

```python
# JobFilterTypeDef definition

class JobFilterTypeDef(TypedDict):
    name: NotRequired[JobFilterNameType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: JobFilterNameType](./literals.md#jobfilternametype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
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

## EBSSavingsEstimationModeTypeDef

```python
# EBSSavingsEstimationModeTypeDef definition

class EBSSavingsEstimationModeTypeDef(TypedDict):
    source: NotRequired[EBSSavingsEstimationModeSourceType],  # (1)
```

1. See [:material-code-brackets: EBSSavingsEstimationModeSourceType](./literals.md#ebssavingsestimationmodesourcetype) 
## EBSEstimatedMonthlySavingsTypeDef

```python
# EBSEstimatedMonthlySavingsTypeDef definition

class EBSEstimatedMonthlySavingsTypeDef(TypedDict):
    currency: NotRequired[CurrencyType],  # (1)
    value: NotRequired[float],
```

1. See [:material-code-brackets: CurrencyType](./literals.md#currencytype) 
## EBSFilterTypeDef

```python
# EBSFilterTypeDef definition

class EBSFilterTypeDef(TypedDict):
    name: NotRequired[EBSFilterNameType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: EBSFilterNameType](./literals.md#ebsfilternametype) 
## EBSUtilizationMetricTypeDef

```python
# EBSUtilizationMetricTypeDef definition

class EBSUtilizationMetricTypeDef(TypedDict):
    name: NotRequired[EBSMetricNameType],  # (1)
    statistic: NotRequired[MetricStatisticType],  # (2)
    value: NotRequired[float],
```

1. See [:material-code-brackets: EBSMetricNameType](./literals.md#ebsmetricnametype) 
2. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
## ECSSavingsEstimationModeTypeDef

```python
# ECSSavingsEstimationModeTypeDef definition

class ECSSavingsEstimationModeTypeDef(TypedDict):
    source: NotRequired[ECSSavingsEstimationModeSourceType],  # (1)
```

1. See [:material-code-brackets: ECSSavingsEstimationModeSourceType](./literals.md#ecssavingsestimationmodesourcetype) 
## ECSEstimatedMonthlySavingsTypeDef

```python
# ECSEstimatedMonthlySavingsTypeDef definition

class ECSEstimatedMonthlySavingsTypeDef(TypedDict):
    currency: NotRequired[CurrencyType],  # (1)
    value: NotRequired[float],
```

1. See [:material-code-brackets: CurrencyType](./literals.md#currencytype) 
## ECSServiceProjectedMetricTypeDef

```python
# ECSServiceProjectedMetricTypeDef definition

class ECSServiceProjectedMetricTypeDef(TypedDict):
    name: NotRequired[ECSServiceMetricNameType],  # (1)
    timestamps: NotRequired[List[datetime]],
    upperBoundValues: NotRequired[List[float]],
    lowerBoundValues: NotRequired[List[float]],
```

1. See [:material-code-brackets: ECSServiceMetricNameType](./literals.md#ecsservicemetricnametype) 
## ECSServiceProjectedUtilizationMetricTypeDef

```python
# ECSServiceProjectedUtilizationMetricTypeDef definition

class ECSServiceProjectedUtilizationMetricTypeDef(TypedDict):
    name: NotRequired[ECSServiceMetricNameType],  # (1)
    statistic: NotRequired[ECSServiceMetricStatisticType],  # (2)
    lowerBoundValue: NotRequired[float],
    upperBoundValue: NotRequired[float],
```

1. See [:material-code-brackets: ECSServiceMetricNameType](./literals.md#ecsservicemetricnametype) 
2. See [:material-code-brackets: ECSServiceMetricStatisticType](./literals.md#ecsservicemetricstatistictype) 
## ECSServiceRecommendationFilterTypeDef

```python
# ECSServiceRecommendationFilterTypeDef definition

class ECSServiceRecommendationFilterTypeDef(TypedDict):
    name: NotRequired[ECSServiceRecommendationFilterNameType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: ECSServiceRecommendationFilterNameType](./literals.md#ecsservicerecommendationfilternametype) 
## ECSServiceUtilizationMetricTypeDef

```python
# ECSServiceUtilizationMetricTypeDef definition

class ECSServiceUtilizationMetricTypeDef(TypedDict):
    name: NotRequired[ECSServiceMetricNameType],  # (1)
    statistic: NotRequired[ECSServiceMetricStatisticType],  # (2)
    value: NotRequired[float],
```

1. See [:material-code-brackets: ECSServiceMetricNameType](./literals.md#ecsservicemetricnametype) 
2. See [:material-code-brackets: ECSServiceMetricStatisticType](./literals.md#ecsservicemetricstatistictype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[str],
```

## EffectivePreferredResourceTypeDef

```python
# EffectivePreferredResourceTypeDef definition

class EffectivePreferredResourceTypeDef(TypedDict):
    name: NotRequired[PreferredResourceNameType],  # (1)
    includeList: NotRequired[List[str]],
    effectiveIncludeList: NotRequired[List[str]],
    excludeList: NotRequired[List[str]],
```

1. See [:material-code-brackets: PreferredResourceNameType](./literals.md#preferredresourcenametype) 
## ExternalMetricsPreferenceTypeDef

```python
# ExternalMetricsPreferenceTypeDef definition

class ExternalMetricsPreferenceTypeDef(TypedDict):
    source: NotRequired[ExternalMetricsSourceType],  # (1)
```

1. See [:material-code-brackets: ExternalMetricsSourceType](./literals.md#externalmetricssourcetype) 
## InstanceSavingsEstimationModeTypeDef

```python
# InstanceSavingsEstimationModeTypeDef definition

class InstanceSavingsEstimationModeTypeDef(TypedDict):
    source: NotRequired[InstanceSavingsEstimationModeSourceType],  # (1)
```

1. See [:material-code-brackets: InstanceSavingsEstimationModeSourceType](./literals.md#instancesavingsestimationmodesourcetype) 
## EnrollmentFilterTypeDef

```python
# EnrollmentFilterTypeDef definition

class EnrollmentFilterTypeDef(TypedDict):
    name: NotRequired[EnrollmentFilterNameType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: EnrollmentFilterNameType](./literals.md#enrollmentfilternametype) 
## EstimatedMonthlySavingsTypeDef

```python
# EstimatedMonthlySavingsTypeDef definition

class EstimatedMonthlySavingsTypeDef(TypedDict):
    currency: NotRequired[CurrencyType],  # (1)
    value: NotRequired[float],
```

1. See [:material-code-brackets: CurrencyType](./literals.md#currencytype) 
## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    name: NotRequired[FilterNameType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: FilterNameType](./literals.md#filternametype) 
## RecommendationPreferencesTypeDef

```python
# RecommendationPreferencesTypeDef definition

class RecommendationPreferencesTypeDef(TypedDict):
    cpuVendorArchitectures: NotRequired[Sequence[CpuVendorArchitectureType]],  # (1)
```

1. See [:material-code-brackets: CpuVendorArchitectureType](./literals.md#cpuvendorarchitecturetype) 
## S3DestinationConfigTypeDef

```python
# S3DestinationConfigTypeDef definition

class S3DestinationConfigTypeDef(TypedDict):
    bucket: NotRequired[str],
    keyPrefix: NotRequired[str],
```

## S3DestinationTypeDef

```python
# S3DestinationTypeDef definition

class S3DestinationTypeDef(TypedDict):
    bucket: NotRequired[str],
    key: NotRequired[str],
    metadataKey: NotRequired[str],
```

## LambdaFunctionRecommendationFilterTypeDef

```python
# LambdaFunctionRecommendationFilterTypeDef definition

class LambdaFunctionRecommendationFilterTypeDef(TypedDict):
    name: NotRequired[LambdaFunctionRecommendationFilterNameType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: LambdaFunctionRecommendationFilterNameType](./literals.md#lambdafunctionrecommendationfilternametype) 
## LicenseRecommendationFilterTypeDef

```python
# LicenseRecommendationFilterTypeDef definition

class LicenseRecommendationFilterTypeDef(TypedDict):
    name: NotRequired[LicenseRecommendationFilterNameType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: LicenseRecommendationFilterNameType](./literals.md#licenserecommendationfilternametype) 
## RDSDBRecommendationFilterTypeDef

```python
# RDSDBRecommendationFilterTypeDef definition

class RDSDBRecommendationFilterTypeDef(TypedDict):
    name: NotRequired[RDSDBRecommendationFilterNameType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: RDSDBRecommendationFilterNameType](./literals.md#rdsdbrecommendationfilternametype) 
## ExternalMetricStatusTypeDef

```python
# ExternalMetricStatusTypeDef definition

class ExternalMetricStatusTypeDef(TypedDict):
    statusCode: NotRequired[ExternalMetricStatusCodeType],  # (1)
    statusReason: NotRequired[str],
```

1. See [:material-code-brackets: ExternalMetricStatusCodeType](./literals.md#externalmetricstatuscodetype) 
## GetRecommendationErrorTypeDef

```python
# GetRecommendationErrorTypeDef definition

class GetRecommendationErrorTypeDef(TypedDict):
    identifier: NotRequired[str],
    code: NotRequired[str],
    message: NotRequired[str],
```

## GetEffectiveRecommendationPreferencesRequestRequestTypeDef

```python
# GetEffectiveRecommendationPreferencesRequestRequestTypeDef definition

class GetEffectiveRecommendationPreferencesRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## GetRecommendationSummariesRequestRequestTypeDef

```python
# GetRecommendationSummariesRequestRequestTypeDef definition

class GetRecommendationSummariesRequestRequestTypeDef(TypedDict):
    accountIds: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GpuTypeDef

```python
# GpuTypeDef definition

class GpuTypeDef(TypedDict):
    gpuCount: NotRequired[int],
    gpuMemorySizeInMiB: NotRequired[int],
```

## InstanceEstimatedMonthlySavingsTypeDef

```python
# InstanceEstimatedMonthlySavingsTypeDef definition

class InstanceEstimatedMonthlySavingsTypeDef(TypedDict):
    currency: NotRequired[CurrencyType],  # (1)
    value: NotRequired[float],
```

1. See [:material-code-brackets: CurrencyType](./literals.md#currencytype) 
## RecommendationSourceTypeDef

```python
# RecommendationSourceTypeDef definition

class RecommendationSourceTypeDef(TypedDict):
    recommendationSourceArn: NotRequired[str],
    recommendationSourceType: NotRequired[RecommendationSourceTypeType],  # (1)
```

1. See [:material-code-brackets: RecommendationSourceTypeType](./literals.md#recommendationsourcetypetype) 
## LambdaSavingsEstimationModeTypeDef

```python
# LambdaSavingsEstimationModeTypeDef definition

class LambdaSavingsEstimationModeTypeDef(TypedDict):
    source: NotRequired[LambdaSavingsEstimationModeSourceType],  # (1)
```

1. See [:material-code-brackets: LambdaSavingsEstimationModeSourceType](./literals.md#lambdasavingsestimationmodesourcetype) 
## LambdaEstimatedMonthlySavingsTypeDef

```python
# LambdaEstimatedMonthlySavingsTypeDef definition

class LambdaEstimatedMonthlySavingsTypeDef(TypedDict):
    currency: NotRequired[CurrencyType],  # (1)
    value: NotRequired[float],
```

1. See [:material-code-brackets: CurrencyType](./literals.md#currencytype) 
## LambdaFunctionMemoryProjectedMetricTypeDef

```python
# LambdaFunctionMemoryProjectedMetricTypeDef definition

class LambdaFunctionMemoryProjectedMetricTypeDef(TypedDict):
    name: NotRequired[LambdaFunctionMemoryMetricNameType],  # (1)
    statistic: NotRequired[LambdaFunctionMemoryMetricStatisticType],  # (2)
    value: NotRequired[float],
```

1. See [:material-code-brackets: LambdaFunctionMemoryMetricNameType](./literals.md#lambdafunctionmemorymetricnametype) 
2. See [:material-code-brackets: LambdaFunctionMemoryMetricStatisticType](./literals.md#lambdafunctionmemorymetricstatistictype) 
## LambdaFunctionUtilizationMetricTypeDef

```python
# LambdaFunctionUtilizationMetricTypeDef definition

class LambdaFunctionUtilizationMetricTypeDef(TypedDict):
    name: NotRequired[LambdaFunctionMetricNameType],  # (1)
    statistic: NotRequired[LambdaFunctionMetricStatisticType],  # (2)
    value: NotRequired[float],
```

1. See [:material-code-brackets: LambdaFunctionMetricNameType](./literals.md#lambdafunctionmetricnametype) 
2. See [:material-code-brackets: LambdaFunctionMetricStatisticType](./literals.md#lambdafunctionmetricstatistictype) 
## MetricSourceTypeDef

```python
# MetricSourceTypeDef definition

class MetricSourceTypeDef(TypedDict):
    provider: NotRequired[MetricSourceProviderType],  # (1)
    providerArn: NotRequired[str],
```

1. See [:material-code-brackets: MetricSourceProviderType](./literals.md#metricsourceprovidertype) 
## PreferredResourceTypeDef

```python
# PreferredResourceTypeDef definition

class PreferredResourceTypeDef(TypedDict):
    name: NotRequired[PreferredResourceNameType],  # (1)
    includeList: NotRequired[Sequence[str]],
    excludeList: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: PreferredResourceNameType](./literals.md#preferredresourcenametype) 
## ProjectedMetricTypeDef

```python
# ProjectedMetricTypeDef definition

class ProjectedMetricTypeDef(TypedDict):
    name: NotRequired[MetricNameType],  # (1)
    timestamps: NotRequired[List[datetime]],
    values: NotRequired[List[float]],
```

1. See [:material-code-brackets: MetricNameType](./literals.md#metricnametype) 
## RDSDBUtilizationMetricTypeDef

```python
# RDSDBUtilizationMetricTypeDef definition

class RDSDBUtilizationMetricTypeDef(TypedDict):
    name: NotRequired[RDSDBMetricNameType],  # (1)
    statistic: NotRequired[RDSDBMetricStatisticType],  # (2)
    value: NotRequired[float],
```

1. See [:material-code-brackets: RDSDBMetricNameType](./literals.md#rdsdbmetricnametype) 
2. See [:material-code-brackets: RDSDBMetricStatisticType](./literals.md#rdsdbmetricstatistictype) 
## RDSDatabaseProjectedMetricTypeDef

```python
# RDSDatabaseProjectedMetricTypeDef definition

class RDSDatabaseProjectedMetricTypeDef(TypedDict):
    name: NotRequired[RDSDBMetricNameType],  # (1)
    timestamps: NotRequired[List[datetime]],
    values: NotRequired[List[float]],
```

1. See [:material-code-brackets: RDSDBMetricNameType](./literals.md#rdsdbmetricnametype) 
## RDSSavingsEstimationModeTypeDef

```python
# RDSSavingsEstimationModeTypeDef definition

class RDSSavingsEstimationModeTypeDef(TypedDict):
    source: NotRequired[RDSSavingsEstimationModeSourceType],  # (1)
```

1. See [:material-code-brackets: RDSSavingsEstimationModeSourceType](./literals.md#rdssavingsestimationmodesourcetype) 
## RDSInstanceEstimatedMonthlySavingsTypeDef

```python
# RDSInstanceEstimatedMonthlySavingsTypeDef definition

class RDSInstanceEstimatedMonthlySavingsTypeDef(TypedDict):
    currency: NotRequired[CurrencyType],  # (1)
    value: NotRequired[float],
```

1. See [:material-code-brackets: CurrencyType](./literals.md#currencytype) 
## RDSStorageEstimatedMonthlySavingsTypeDef

```python
# RDSStorageEstimatedMonthlySavingsTypeDef definition

class RDSStorageEstimatedMonthlySavingsTypeDef(TypedDict):
    currency: NotRequired[CurrencyType],  # (1)
    value: NotRequired[float],
```

1. See [:material-code-brackets: CurrencyType](./literals.md#currencytype) 
## ReasonCodeSummaryTypeDef

```python
# ReasonCodeSummaryTypeDef definition

class ReasonCodeSummaryTypeDef(TypedDict):
    name: NotRequired[FindingReasonCodeType],  # (1)
    value: NotRequired[float],
```

1. See [:material-code-brackets: FindingReasonCodeType](./literals.md#findingreasoncodetype) 
## UpdateEnrollmentStatusRequestRequestTypeDef

```python
# UpdateEnrollmentStatusRequestRequestTypeDef definition

class UpdateEnrollmentStatusRequestRequestTypeDef(TypedDict):
    status: StatusType,  # (1)
    includeMemberAccounts: NotRequired[bool],
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## VolumeConfigurationTypeDef

```python
# VolumeConfigurationTypeDef definition

class VolumeConfigurationTypeDef(TypedDict):
    volumeType: NotRequired[str],
    volumeSize: NotRequired[int],
    volumeBaselineIOPS: NotRequired[int],
    volumeBurstIOPS: NotRequired[int],
    volumeBaselineThroughput: NotRequired[int],
    volumeBurstThroughput: NotRequired[int],
    rootVolume: NotRequired[bool],
```

## AutoScalingGroupSavingsOpportunityAfterDiscountsTypeDef

```python
# AutoScalingGroupSavingsOpportunityAfterDiscountsTypeDef definition

class AutoScalingGroupSavingsOpportunityAfterDiscountsTypeDef(TypedDict):
    savingsOpportunityPercentage: NotRequired[float],
    estimatedMonthlySavings: NotRequired[AutoScalingGroupEstimatedMonthlySavingsTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingGroupEstimatedMonthlySavingsTypeDef](./type_defs.md#autoscalinggroupestimatedmonthlysavingstypedef) 
## ContainerConfigurationTypeDef

```python
# ContainerConfigurationTypeDef definition

class ContainerConfigurationTypeDef(TypedDict):
    containerName: NotRequired[str],
    memorySizeConfiguration: NotRequired[MemorySizeConfigurationTypeDef],  # (1)
    cpu: NotRequired[int],
```

1. See [:material-code-braces: MemorySizeConfigurationTypeDef](./type_defs.md#memorysizeconfigurationtypedef) 
## ContainerRecommendationTypeDef

```python
# ContainerRecommendationTypeDef definition

class ContainerRecommendationTypeDef(TypedDict):
    containerName: NotRequired[str],
    memorySizeConfiguration: NotRequired[MemorySizeConfigurationTypeDef],  # (1)
    cpu: NotRequired[int],
```

1. See [:material-code-braces: MemorySizeConfigurationTypeDef](./type_defs.md#memorysizeconfigurationtypedef) 
## UtilizationPreferenceTypeDef

```python
# UtilizationPreferenceTypeDef definition

class UtilizationPreferenceTypeDef(TypedDict):
    metricName: NotRequired[CustomizableMetricNameType],  # (1)
    metricParameters: NotRequired[CustomizableMetricParametersTypeDef],  # (2)
```

1. See [:material-code-brackets: CustomizableMetricNameType](./literals.md#customizablemetricnametype) 
2. See [:material-code-braces: CustomizableMetricParametersTypeDef](./type_defs.md#customizablemetricparameterstypedef) 
## DeleteRecommendationPreferencesRequestRequestTypeDef

```python
# DeleteRecommendationPreferencesRequestRequestTypeDef definition

class DeleteRecommendationPreferencesRequestRequestTypeDef(TypedDict):
    resourceType: ResourceTypeType,  # (1)
    recommendationPreferenceNames: Sequence[RecommendationPreferenceNameType],  # (2)
    scope: NotRequired[ScopeTypeDef],  # (3)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: RecommendationPreferenceNameType](./literals.md#recommendationpreferencenametype) 
3. See [:material-code-braces: ScopeTypeDef](./type_defs.md#scopetypedef) 
## GetRecommendationPreferencesRequestRequestTypeDef

```python
# GetRecommendationPreferencesRequestRequestTypeDef definition

class GetRecommendationPreferencesRequestRequestTypeDef(TypedDict):
    resourceType: ResourceTypeType,  # (1)
    scope: NotRequired[ScopeTypeDef],  # (2)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ScopeTypeDef](./type_defs.md#scopetypedef) 
## DescribeRecommendationExportJobsRequestRequestTypeDef

```python
# DescribeRecommendationExportJobsRequestRequestTypeDef definition

class DescribeRecommendationExportJobsRequestRequestTypeDef(TypedDict):
    jobIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[JobFilterTypeDef]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: JobFilterTypeDef](./type_defs.md#jobfiltertypedef) 
## DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef

```python
# DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef definition

class DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef(TypedDict):
    jobIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[JobFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: JobFilterTypeDef](./type_defs.md#jobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef

```python
# GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef definition

class GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef(TypedDict):
    resourceType: ResourceTypeType,  # (1)
    scope: NotRequired[ScopeTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ScopeTypeDef](./type_defs.md#scopetypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef

```python
# GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef definition

class GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef(TypedDict):
    accountIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetEnrollmentStatusResponseTypeDef

```python
# GetEnrollmentStatusResponseTypeDef definition

class GetEnrollmentStatusResponseTypeDef(TypedDict):
    status: StatusType,  # (1)
    statusReason: str,
    memberAccountsEnrolled: bool,
    lastUpdatedTimestamp: datetime,
    numberOfMemberAccountsOptedIn: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEnrollmentStatusesForOrganizationResponseTypeDef

```python
# GetEnrollmentStatusesForOrganizationResponseTypeDef definition

class GetEnrollmentStatusesForOrganizationResponseTypeDef(TypedDict):
    accountEnrollmentStatuses: List[AccountEnrollmentStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AccountEnrollmentStatusTypeDef](./type_defs.md#accountenrollmentstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEnrollmentStatusResponseTypeDef

```python
# UpdateEnrollmentStatusResponseTypeDef definition

class UpdateEnrollmentStatusResponseTypeDef(TypedDict):
    status: StatusType,  # (1)
    statusReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EBSEffectiveRecommendationPreferencesTypeDef

```python
# EBSEffectiveRecommendationPreferencesTypeDef definition

class EBSEffectiveRecommendationPreferencesTypeDef(TypedDict):
    savingsEstimationMode: NotRequired[EBSSavingsEstimationModeTypeDef],  # (1)
```

1. See [:material-code-braces: EBSSavingsEstimationModeTypeDef](./type_defs.md#ebssavingsestimationmodetypedef) 
## EBSSavingsOpportunityAfterDiscountsTypeDef

```python
# EBSSavingsOpportunityAfterDiscountsTypeDef definition

class EBSSavingsOpportunityAfterDiscountsTypeDef(TypedDict):
    savingsOpportunityPercentage: NotRequired[float],
    estimatedMonthlySavings: NotRequired[EBSEstimatedMonthlySavingsTypeDef],  # (1)
```

1. See [:material-code-braces: EBSEstimatedMonthlySavingsTypeDef](./type_defs.md#ebsestimatedmonthlysavingstypedef) 
## GetEBSVolumeRecommendationsRequestRequestTypeDef

```python
# GetEBSVolumeRecommendationsRequestRequestTypeDef definition

class GetEBSVolumeRecommendationsRequestRequestTypeDef(TypedDict):
    volumeArns: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[EBSFilterTypeDef]],  # (1)
    accountIds: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: EBSFilterTypeDef](./type_defs.md#ebsfiltertypedef) 
## ECSEffectiveRecommendationPreferencesTypeDef

```python
# ECSEffectiveRecommendationPreferencesTypeDef definition

class ECSEffectiveRecommendationPreferencesTypeDef(TypedDict):
    savingsEstimationMode: NotRequired[ECSSavingsEstimationModeTypeDef],  # (1)
```

1. See [:material-code-braces: ECSSavingsEstimationModeTypeDef](./type_defs.md#ecssavingsestimationmodetypedef) 
## ECSSavingsOpportunityAfterDiscountsTypeDef

```python
# ECSSavingsOpportunityAfterDiscountsTypeDef definition

class ECSSavingsOpportunityAfterDiscountsTypeDef(TypedDict):
    savingsOpportunityPercentage: NotRequired[float],
    estimatedMonthlySavings: NotRequired[ECSEstimatedMonthlySavingsTypeDef],  # (1)
```

1. See [:material-code-braces: ECSEstimatedMonthlySavingsTypeDef](./type_defs.md#ecsestimatedmonthlysavingstypedef) 
## ECSServiceRecommendedOptionProjectedMetricTypeDef

```python
# ECSServiceRecommendedOptionProjectedMetricTypeDef definition

class ECSServiceRecommendedOptionProjectedMetricTypeDef(TypedDict):
    recommendedCpuUnits: NotRequired[int],
    recommendedMemorySize: NotRequired[int],
    projectedMetrics: NotRequired[List[ECSServiceProjectedMetricTypeDef]],  # (1)
```

1. See [:material-code-braces: ECSServiceProjectedMetricTypeDef](./type_defs.md#ecsserviceprojectedmetrictypedef) 
## GetECSServiceRecommendationsRequestRequestTypeDef

```python
# GetECSServiceRecommendationsRequestRequestTypeDef definition

class GetECSServiceRecommendationsRequestRequestTypeDef(TypedDict):
    serviceArns: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[ECSServiceRecommendationFilterTypeDef]],  # (1)
    accountIds: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: ECSServiceRecommendationFilterTypeDef](./type_defs.md#ecsservicerecommendationfiltertypedef) 
## GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef

```python
# GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef definition

class GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef(TypedDict):
    filters: NotRequired[Sequence[EnrollmentFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: EnrollmentFilterTypeDef](./type_defs.md#enrollmentfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetEnrollmentStatusesForOrganizationRequestRequestTypeDef

```python
# GetEnrollmentStatusesForOrganizationRequestRequestTypeDef definition

class GetEnrollmentStatusesForOrganizationRequestRequestTypeDef(TypedDict):
    filters: NotRequired[Sequence[EnrollmentFilterTypeDef]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: EnrollmentFilterTypeDef](./type_defs.md#enrollmentfiltertypedef) 
## InferredWorkloadSavingTypeDef

```python
# InferredWorkloadSavingTypeDef definition

class InferredWorkloadSavingTypeDef(TypedDict):
    inferredWorkloadTypes: NotRequired[List[InferredWorkloadTypeType]],  # (1)
    estimatedMonthlySavings: NotRequired[EstimatedMonthlySavingsTypeDef],  # (2)
```

1. See [:material-code-brackets: InferredWorkloadTypeType](./literals.md#inferredworkloadtypetype) 
2. See [:material-code-braces: EstimatedMonthlySavingsTypeDef](./type_defs.md#estimatedmonthlysavingstypedef) 
## SavingsOpportunityTypeDef

```python
# SavingsOpportunityTypeDef definition

class SavingsOpportunityTypeDef(TypedDict):
    savingsOpportunityPercentage: NotRequired[float],
    estimatedMonthlySavings: NotRequired[EstimatedMonthlySavingsTypeDef],  # (1)
```

1. See [:material-code-braces: EstimatedMonthlySavingsTypeDef](./type_defs.md#estimatedmonthlysavingstypedef) 
## GetAutoScalingGroupRecommendationsRequestRequestTypeDef

```python
# GetAutoScalingGroupRecommendationsRequestRequestTypeDef definition

class GetAutoScalingGroupRecommendationsRequestRequestTypeDef(TypedDict):
    accountIds: NotRequired[Sequence[str]],
    autoScalingGroupArns: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    recommendationPreferences: NotRequired[RecommendationPreferencesTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef) 
## GetEC2InstanceRecommendationsRequestRequestTypeDef

```python
# GetEC2InstanceRecommendationsRequestRequestTypeDef definition

class GetEC2InstanceRecommendationsRequestRequestTypeDef(TypedDict):
    instanceArns: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    accountIds: NotRequired[Sequence[str]],
    recommendationPreferences: NotRequired[RecommendationPreferencesTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef) 
## ExportAutoScalingGroupRecommendationsRequestRequestTypeDef

```python
# ExportAutoScalingGroupRecommendationsRequestRequestTypeDef definition

class ExportAutoScalingGroupRecommendationsRequestRequestTypeDef(TypedDict):
    s3DestinationConfig: S3DestinationConfigTypeDef,  # (1)
    accountIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (2)
    fieldsToExport: NotRequired[Sequence[ExportableAutoScalingGroupFieldType]],  # (3)
    fileFormat: NotRequired[FileFormatType],  # (4)
    includeMemberAccounts: NotRequired[bool],
    recommendationPreferences: NotRequired[RecommendationPreferencesTypeDef],  # (5)
```

1. See [:material-code-braces: S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-brackets: ExportableAutoScalingGroupFieldType](./literals.md#exportableautoscalinggroupfieldtype) 
4. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
5. See [:material-code-braces: RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef) 
## ExportEBSVolumeRecommendationsRequestRequestTypeDef

```python
# ExportEBSVolumeRecommendationsRequestRequestTypeDef definition

class ExportEBSVolumeRecommendationsRequestRequestTypeDef(TypedDict):
    s3DestinationConfig: S3DestinationConfigTypeDef,  # (1)
    accountIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[EBSFilterTypeDef]],  # (2)
    fieldsToExport: NotRequired[Sequence[ExportableVolumeFieldType]],  # (3)
    fileFormat: NotRequired[FileFormatType],  # (4)
    includeMemberAccounts: NotRequired[bool],
```

1. See [:material-code-braces: S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef) 
2. See [:material-code-braces: EBSFilterTypeDef](./type_defs.md#ebsfiltertypedef) 
3. See [:material-code-brackets: ExportableVolumeFieldType](./literals.md#exportablevolumefieldtype) 
4. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
## ExportEC2InstanceRecommendationsRequestRequestTypeDef

```python
# ExportEC2InstanceRecommendationsRequestRequestTypeDef definition

class ExportEC2InstanceRecommendationsRequestRequestTypeDef(TypedDict):
    s3DestinationConfig: S3DestinationConfigTypeDef,  # (1)
    accountIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (2)
    fieldsToExport: NotRequired[Sequence[ExportableInstanceFieldType]],  # (3)
    fileFormat: NotRequired[FileFormatType],  # (4)
    includeMemberAccounts: NotRequired[bool],
    recommendationPreferences: NotRequired[RecommendationPreferencesTypeDef],  # (5)
```

1. See [:material-code-braces: S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-brackets: ExportableInstanceFieldType](./literals.md#exportableinstancefieldtype) 
4. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
5. See [:material-code-braces: RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef) 
## ExportECSServiceRecommendationsRequestRequestTypeDef

```python
# ExportECSServiceRecommendationsRequestRequestTypeDef definition

class ExportECSServiceRecommendationsRequestRequestTypeDef(TypedDict):
    s3DestinationConfig: S3DestinationConfigTypeDef,  # (1)
    accountIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[ECSServiceRecommendationFilterTypeDef]],  # (2)
    fieldsToExport: NotRequired[Sequence[ExportableECSServiceFieldType]],  # (3)
    fileFormat: NotRequired[FileFormatType],  # (4)
    includeMemberAccounts: NotRequired[bool],
```

1. See [:material-code-braces: S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef) 
2. See [:material-code-braces: ECSServiceRecommendationFilterTypeDef](./type_defs.md#ecsservicerecommendationfiltertypedef) 
3. See [:material-code-brackets: ExportableECSServiceFieldType](./literals.md#exportableecsservicefieldtype) 
4. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
## ExportAutoScalingGroupRecommendationsResponseTypeDef

```python
# ExportAutoScalingGroupRecommendationsResponseTypeDef definition

class ExportAutoScalingGroupRecommendationsResponseTypeDef(TypedDict):
    jobId: str,
    s3Destination: S3DestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportDestinationTypeDef

```python
# ExportDestinationTypeDef definition

class ExportDestinationTypeDef(TypedDict):
    s3: NotRequired[S3DestinationTypeDef],  # (1)
```

1. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
## ExportEBSVolumeRecommendationsResponseTypeDef

```python
# ExportEBSVolumeRecommendationsResponseTypeDef definition

class ExportEBSVolumeRecommendationsResponseTypeDef(TypedDict):
    jobId: str,
    s3Destination: S3DestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportEC2InstanceRecommendationsResponseTypeDef

```python
# ExportEC2InstanceRecommendationsResponseTypeDef definition

class ExportEC2InstanceRecommendationsResponseTypeDef(TypedDict):
    jobId: str,
    s3Destination: S3DestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportECSServiceRecommendationsResponseTypeDef

```python
# ExportECSServiceRecommendationsResponseTypeDef definition

class ExportECSServiceRecommendationsResponseTypeDef(TypedDict):
    jobId: str,
    s3Destination: S3DestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportLambdaFunctionRecommendationsResponseTypeDef

```python
# ExportLambdaFunctionRecommendationsResponseTypeDef definition

class ExportLambdaFunctionRecommendationsResponseTypeDef(TypedDict):
    jobId: str,
    s3Destination: S3DestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportLicenseRecommendationsResponseTypeDef

```python
# ExportLicenseRecommendationsResponseTypeDef definition

class ExportLicenseRecommendationsResponseTypeDef(TypedDict):
    jobId: str,
    s3Destination: S3DestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportRDSDatabaseRecommendationsResponseTypeDef

```python
# ExportRDSDatabaseRecommendationsResponseTypeDef definition

class ExportRDSDatabaseRecommendationsResponseTypeDef(TypedDict):
    jobId: str,
    s3Destination: S3DestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportLambdaFunctionRecommendationsRequestRequestTypeDef

```python
# ExportLambdaFunctionRecommendationsRequestRequestTypeDef definition

class ExportLambdaFunctionRecommendationsRequestRequestTypeDef(TypedDict):
    s3DestinationConfig: S3DestinationConfigTypeDef,  # (1)
    accountIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[LambdaFunctionRecommendationFilterTypeDef]],  # (2)
    fieldsToExport: NotRequired[Sequence[ExportableLambdaFunctionFieldType]],  # (3)
    fileFormat: NotRequired[FileFormatType],  # (4)
    includeMemberAccounts: NotRequired[bool],
```

1. See [:material-code-braces: S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef) 
2. See [:material-code-braces: LambdaFunctionRecommendationFilterTypeDef](./type_defs.md#lambdafunctionrecommendationfiltertypedef) 
3. See [:material-code-brackets: ExportableLambdaFunctionFieldType](./literals.md#exportablelambdafunctionfieldtype) 
4. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
## GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef

```python
# GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef definition

class GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef(TypedDict):
    functionArns: NotRequired[Sequence[str]],
    accountIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[LambdaFunctionRecommendationFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: LambdaFunctionRecommendationFilterTypeDef](./type_defs.md#lambdafunctionrecommendationfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetLambdaFunctionRecommendationsRequestRequestTypeDef

```python
# GetLambdaFunctionRecommendationsRequestRequestTypeDef definition

class GetLambdaFunctionRecommendationsRequestRequestTypeDef(TypedDict):
    functionArns: NotRequired[Sequence[str]],
    accountIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[LambdaFunctionRecommendationFilterTypeDef]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: LambdaFunctionRecommendationFilterTypeDef](./type_defs.md#lambdafunctionrecommendationfiltertypedef) 
## ExportLicenseRecommendationsRequestRequestTypeDef

```python
# ExportLicenseRecommendationsRequestRequestTypeDef definition

class ExportLicenseRecommendationsRequestRequestTypeDef(TypedDict):
    s3DestinationConfig: S3DestinationConfigTypeDef,  # (1)
    accountIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[LicenseRecommendationFilterTypeDef]],  # (2)
    fieldsToExport: NotRequired[Sequence[ExportableLicenseFieldType]],  # (3)
    fileFormat: NotRequired[FileFormatType],  # (4)
    includeMemberAccounts: NotRequired[bool],
```

1. See [:material-code-braces: S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef) 
2. See [:material-code-braces: LicenseRecommendationFilterTypeDef](./type_defs.md#licenserecommendationfiltertypedef) 
3. See [:material-code-brackets: ExportableLicenseFieldType](./literals.md#exportablelicensefieldtype) 
4. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
## GetLicenseRecommendationsRequestRequestTypeDef

```python
# GetLicenseRecommendationsRequestRequestTypeDef definition

class GetLicenseRecommendationsRequestRequestTypeDef(TypedDict):
    resourceArns: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[LicenseRecommendationFilterTypeDef]],  # (1)
    accountIds: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: LicenseRecommendationFilterTypeDef](./type_defs.md#licenserecommendationfiltertypedef) 
## ExportRDSDatabaseRecommendationsRequestRequestTypeDef

```python
# ExportRDSDatabaseRecommendationsRequestRequestTypeDef definition

class ExportRDSDatabaseRecommendationsRequestRequestTypeDef(TypedDict):
    s3DestinationConfig: S3DestinationConfigTypeDef,  # (1)
    accountIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[RDSDBRecommendationFilterTypeDef]],  # (2)
    fieldsToExport: NotRequired[Sequence[ExportableRDSDBFieldType]],  # (3)
    fileFormat: NotRequired[FileFormatType],  # (4)
    includeMemberAccounts: NotRequired[bool],
    recommendationPreferences: NotRequired[RecommendationPreferencesTypeDef],  # (5)
```

1. See [:material-code-braces: S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef) 
2. See [:material-code-braces: RDSDBRecommendationFilterTypeDef](./type_defs.md#rdsdbrecommendationfiltertypedef) 
3. See [:material-code-brackets: ExportableRDSDBFieldType](./literals.md#exportablerdsdbfieldtype) 
4. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
5. See [:material-code-braces: RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef) 
## GetRDSDatabaseRecommendationsRequestRequestTypeDef

```python
# GetRDSDatabaseRecommendationsRequestRequestTypeDef definition

class GetRDSDatabaseRecommendationsRequestRequestTypeDef(TypedDict):
    resourceArns: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[RDSDBRecommendationFilterTypeDef]],  # (1)
    accountIds: NotRequired[Sequence[str]],
    recommendationPreferences: NotRequired[RecommendationPreferencesTypeDef],  # (2)
```

1. See [:material-code-braces: RDSDBRecommendationFilterTypeDef](./type_defs.md#rdsdbrecommendationfiltertypedef) 
2. See [:material-code-braces: RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef) 
## GetEC2RecommendationProjectedMetricsRequestRequestTypeDef

```python
# GetEC2RecommendationProjectedMetricsRequestRequestTypeDef definition

class GetEC2RecommendationProjectedMetricsRequestRequestTypeDef(TypedDict):
    instanceArn: str,
    stat: MetricStatisticType,  # (1)
    period: int,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    recommendationPreferences: NotRequired[RecommendationPreferencesTypeDef],  # (2)
```

1. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
2. See [:material-code-braces: RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef) 
## GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef

```python
# GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef definition

class GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef(TypedDict):
    serviceArn: str,
    stat: MetricStatisticType,  # (1)
    period: int,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
```

1. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
## GetRDSDatabaseRecommendationProjectedMetricsRequestRequestTypeDef

```python
# GetRDSDatabaseRecommendationProjectedMetricsRequestRequestTypeDef definition

class GetRDSDatabaseRecommendationProjectedMetricsRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    stat: MetricStatisticType,  # (1)
    period: int,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    recommendationPreferences: NotRequired[RecommendationPreferencesTypeDef],  # (2)
```

1. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
2. See [:material-code-braces: RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef) 
## GpuInfoTypeDef

```python
# GpuInfoTypeDef definition

class GpuInfoTypeDef(TypedDict):
    gpus: NotRequired[List[GpuTypeDef]],  # (1)
```

1. See [:material-code-braces: GpuTypeDef](./type_defs.md#gputypedef) 
## InstanceSavingsOpportunityAfterDiscountsTypeDef

```python
# InstanceSavingsOpportunityAfterDiscountsTypeDef definition

class InstanceSavingsOpportunityAfterDiscountsTypeDef(TypedDict):
    savingsOpportunityPercentage: NotRequired[float],
    estimatedMonthlySavings: NotRequired[InstanceEstimatedMonthlySavingsTypeDef],  # (1)
```

1. See [:material-code-braces: InstanceEstimatedMonthlySavingsTypeDef](./type_defs.md#instanceestimatedmonthlysavingstypedef) 
## LambdaEffectiveRecommendationPreferencesTypeDef

```python
# LambdaEffectiveRecommendationPreferencesTypeDef definition

class LambdaEffectiveRecommendationPreferencesTypeDef(TypedDict):
    savingsEstimationMode: NotRequired[LambdaSavingsEstimationModeTypeDef],  # (1)
```

1. See [:material-code-braces: LambdaSavingsEstimationModeTypeDef](./type_defs.md#lambdasavingsestimationmodetypedef) 
## LambdaSavingsOpportunityAfterDiscountsTypeDef

```python
# LambdaSavingsOpportunityAfterDiscountsTypeDef definition

class LambdaSavingsOpportunityAfterDiscountsTypeDef(TypedDict):
    savingsOpportunityPercentage: NotRequired[float],
    estimatedMonthlySavings: NotRequired[LambdaEstimatedMonthlySavingsTypeDef],  # (1)
```

1. See [:material-code-braces: LambdaEstimatedMonthlySavingsTypeDef](./type_defs.md#lambdaestimatedmonthlysavingstypedef) 
## LicenseConfigurationTypeDef

```python
# LicenseConfigurationTypeDef definition

class LicenseConfigurationTypeDef(TypedDict):
    numberOfCores: NotRequired[int],
    instanceType: NotRequired[str],
    operatingSystem: NotRequired[str],
    licenseEdition: NotRequired[LicenseEditionType],  # (1)
    licenseName: NotRequired[LicenseNameType],  # (2)
    licenseModel: NotRequired[LicenseModelType],  # (3)
    licenseVersion: NotRequired[str],
    metricsSource: NotRequired[List[MetricSourceTypeDef]],  # (4)
```

1. See [:material-code-brackets: LicenseEditionType](./literals.md#licenseeditiontype) 
2. See [:material-code-brackets: LicenseNameType](./literals.md#licensenametype) 
3. See [:material-code-brackets: LicenseModelType](./literals.md#licensemodeltype) 
4. See [:material-code-braces: MetricSourceTypeDef](./type_defs.md#metricsourcetypedef) 
## RecommendedOptionProjectedMetricTypeDef

```python
# RecommendedOptionProjectedMetricTypeDef definition

class RecommendedOptionProjectedMetricTypeDef(TypedDict):
    recommendedInstanceType: NotRequired[str],
    rank: NotRequired[int],
    projectedMetrics: NotRequired[List[ProjectedMetricTypeDef]],  # (1)
```

1. See [:material-code-braces: ProjectedMetricTypeDef](./type_defs.md#projectedmetrictypedef) 
## RDSDatabaseRecommendedOptionProjectedMetricTypeDef

```python
# RDSDatabaseRecommendedOptionProjectedMetricTypeDef definition

class RDSDatabaseRecommendedOptionProjectedMetricTypeDef(TypedDict):
    recommendedDBInstanceClass: NotRequired[str],
    rank: NotRequired[int],
    projectedMetrics: NotRequired[List[RDSDatabaseProjectedMetricTypeDef]],  # (1)
```

1. See [:material-code-braces: RDSDatabaseProjectedMetricTypeDef](./type_defs.md#rdsdatabaseprojectedmetrictypedef) 
## RDSEffectiveRecommendationPreferencesTypeDef

```python
# RDSEffectiveRecommendationPreferencesTypeDef definition

class RDSEffectiveRecommendationPreferencesTypeDef(TypedDict):
    cpuVendorArchitectures: NotRequired[List[CpuVendorArchitectureType]],  # (1)
    enhancedInfrastructureMetrics: NotRequired[EnhancedInfrastructureMetricsType],  # (2)
    lookBackPeriod: NotRequired[LookBackPeriodPreferenceType],  # (3)
    savingsEstimationMode: NotRequired[RDSSavingsEstimationModeTypeDef],  # (4)
```

1. See [:material-code-brackets: CpuVendorArchitectureType](./literals.md#cpuvendorarchitecturetype) 
2. See [:material-code-brackets: EnhancedInfrastructureMetricsType](./literals.md#enhancedinfrastructuremetricstype) 
3. See [:material-code-brackets: LookBackPeriodPreferenceType](./literals.md#lookbackperiodpreferencetype) 
4. See [:material-code-braces: RDSSavingsEstimationModeTypeDef](./type_defs.md#rdssavingsestimationmodetypedef) 
## RDSInstanceSavingsOpportunityAfterDiscountsTypeDef

```python
# RDSInstanceSavingsOpportunityAfterDiscountsTypeDef definition

class RDSInstanceSavingsOpportunityAfterDiscountsTypeDef(TypedDict):
    savingsOpportunityPercentage: NotRequired[float],
    estimatedMonthlySavings: NotRequired[RDSInstanceEstimatedMonthlySavingsTypeDef],  # (1)
```

1. See [:material-code-braces: RDSInstanceEstimatedMonthlySavingsTypeDef](./type_defs.md#rdsinstanceestimatedmonthlysavingstypedef) 
## RDSStorageSavingsOpportunityAfterDiscountsTypeDef

```python
# RDSStorageSavingsOpportunityAfterDiscountsTypeDef definition

class RDSStorageSavingsOpportunityAfterDiscountsTypeDef(TypedDict):
    savingsOpportunityPercentage: NotRequired[float],
    estimatedMonthlySavings: NotRequired[RDSStorageEstimatedMonthlySavingsTypeDef],  # (1)
```

1. See [:material-code-braces: RDSStorageEstimatedMonthlySavingsTypeDef](./type_defs.md#rdsstorageestimatedmonthlysavingstypedef) 
## SummaryTypeDef

```python
# SummaryTypeDef definition

class SummaryTypeDef(TypedDict):
    name: NotRequired[FindingType],  # (1)
    value: NotRequired[float],
    reasonCodeSummaries: NotRequired[List[ReasonCodeSummaryTypeDef]],  # (2)
```

1. See [:material-code-brackets: FindingType](./literals.md#findingtype) 
2. See [:material-code-braces: ReasonCodeSummaryTypeDef](./type_defs.md#reasoncodesummarytypedef) 
## ServiceConfigurationTypeDef

```python
# ServiceConfigurationTypeDef definition

class ServiceConfigurationTypeDef(TypedDict):
    memory: NotRequired[int],
    cpu: NotRequired[int],
    containerConfigurations: NotRequired[List[ContainerConfigurationTypeDef]],  # (1)
    autoScalingConfiguration: NotRequired[AutoScalingConfigurationType],  # (2)
    taskDefinitionArn: NotRequired[str],
```

1. See [:material-code-braces: ContainerConfigurationTypeDef](./type_defs.md#containerconfigurationtypedef) 
2. See [:material-code-brackets: AutoScalingConfigurationType](./literals.md#autoscalingconfigurationtype) 
## EffectiveRecommendationPreferencesTypeDef

```python
# EffectiveRecommendationPreferencesTypeDef definition

class EffectiveRecommendationPreferencesTypeDef(TypedDict):
    cpuVendorArchitectures: NotRequired[List[CpuVendorArchitectureType]],  # (1)
    enhancedInfrastructureMetrics: NotRequired[EnhancedInfrastructureMetricsType],  # (2)
    inferredWorkloadTypes: NotRequired[InferredWorkloadTypesPreferenceType],  # (3)
    externalMetricsPreference: NotRequired[ExternalMetricsPreferenceTypeDef],  # (4)
    lookBackPeriod: NotRequired[LookBackPeriodPreferenceType],  # (5)
    utilizationPreferences: NotRequired[List[UtilizationPreferenceTypeDef]],  # (6)
    preferredResources: NotRequired[List[EffectivePreferredResourceTypeDef]],  # (7)
    savingsEstimationMode: NotRequired[InstanceSavingsEstimationModeTypeDef],  # (8)
```

1. See [:material-code-brackets: CpuVendorArchitectureType](./literals.md#cpuvendorarchitecturetype) 
2. See [:material-code-brackets: EnhancedInfrastructureMetricsType](./literals.md#enhancedinfrastructuremetricstype) 
3. See [:material-code-brackets: InferredWorkloadTypesPreferenceType](./literals.md#inferredworkloadtypespreferencetype) 
4. See [:material-code-braces: ExternalMetricsPreferenceTypeDef](./type_defs.md#externalmetricspreferencetypedef) 
5. See [:material-code-brackets: LookBackPeriodPreferenceType](./literals.md#lookbackperiodpreferencetype) 
6. See [:material-code-braces: UtilizationPreferenceTypeDef](./type_defs.md#utilizationpreferencetypedef) 
7. See [:material-code-braces: EffectivePreferredResourceTypeDef](./type_defs.md#effectivepreferredresourcetypedef) 
8. See [:material-code-braces: InstanceSavingsEstimationModeTypeDef](./type_defs.md#instancesavingsestimationmodetypedef) 
## GetEffectiveRecommendationPreferencesResponseTypeDef

```python
# GetEffectiveRecommendationPreferencesResponseTypeDef definition

class GetEffectiveRecommendationPreferencesResponseTypeDef(TypedDict):
    enhancedInfrastructureMetrics: EnhancedInfrastructureMetricsType,  # (1)
    externalMetricsPreference: ExternalMetricsPreferenceTypeDef,  # (2)
    lookBackPeriod: LookBackPeriodPreferenceType,  # (3)
    utilizationPreferences: List[UtilizationPreferenceTypeDef],  # (4)
    preferredResources: List[EffectivePreferredResourceTypeDef],  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: EnhancedInfrastructureMetricsType](./literals.md#enhancedinfrastructuremetricstype) 
2. See [:material-code-braces: ExternalMetricsPreferenceTypeDef](./type_defs.md#externalmetricspreferencetypedef) 
3. See [:material-code-brackets: LookBackPeriodPreferenceType](./literals.md#lookbackperiodpreferencetype) 
4. See [:material-code-braces: UtilizationPreferenceTypeDef](./type_defs.md#utilizationpreferencetypedef) 
5. See [:material-code-braces: EffectivePreferredResourceTypeDef](./type_defs.md#effectivepreferredresourcetypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRecommendationPreferencesRequestRequestTypeDef

```python
# PutRecommendationPreferencesRequestRequestTypeDef definition

class PutRecommendationPreferencesRequestRequestTypeDef(TypedDict):
    resourceType: ResourceTypeType,  # (1)
    scope: NotRequired[ScopeTypeDef],  # (2)
    enhancedInfrastructureMetrics: NotRequired[EnhancedInfrastructureMetricsType],  # (3)
    inferredWorkloadTypes: NotRequired[InferredWorkloadTypesPreferenceType],  # (4)
    externalMetricsPreference: NotRequired[ExternalMetricsPreferenceTypeDef],  # (5)
    lookBackPeriod: NotRequired[LookBackPeriodPreferenceType],  # (6)
    utilizationPreferences: NotRequired[Sequence[UtilizationPreferenceTypeDef]],  # (7)
    preferredResources: NotRequired[Sequence[PreferredResourceTypeDef]],  # (8)
    savingsEstimationMode: NotRequired[SavingsEstimationModeType],  # (9)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ScopeTypeDef](./type_defs.md#scopetypedef) 
3. See [:material-code-brackets: EnhancedInfrastructureMetricsType](./literals.md#enhancedinfrastructuremetricstype) 
4. See [:material-code-brackets: InferredWorkloadTypesPreferenceType](./literals.md#inferredworkloadtypespreferencetype) 
5. See [:material-code-braces: ExternalMetricsPreferenceTypeDef](./type_defs.md#externalmetricspreferencetypedef) 
6. See [:material-code-brackets: LookBackPeriodPreferenceType](./literals.md#lookbackperiodpreferencetype) 
7. See [:material-code-braces: UtilizationPreferenceTypeDef](./type_defs.md#utilizationpreferencetypedef) 
8. See [:material-code-braces: PreferredResourceTypeDef](./type_defs.md#preferredresourcetypedef) 
9. See [:material-code-brackets: SavingsEstimationModeType](./literals.md#savingsestimationmodetype) 
## RecommendationPreferencesDetailTypeDef

```python
# RecommendationPreferencesDetailTypeDef definition

class RecommendationPreferencesDetailTypeDef(TypedDict):
    scope: NotRequired[ScopeTypeDef],  # (1)
    resourceType: NotRequired[ResourceTypeType],  # (2)
    enhancedInfrastructureMetrics: NotRequired[EnhancedInfrastructureMetricsType],  # (3)
    inferredWorkloadTypes: NotRequired[InferredWorkloadTypesPreferenceType],  # (4)
    externalMetricsPreference: NotRequired[ExternalMetricsPreferenceTypeDef],  # (5)
    lookBackPeriod: NotRequired[LookBackPeriodPreferenceType],  # (6)
    utilizationPreferences: NotRequired[List[UtilizationPreferenceTypeDef]],  # (7)
    preferredResources: NotRequired[List[EffectivePreferredResourceTypeDef]],  # (8)
    savingsEstimationMode: NotRequired[SavingsEstimationModeType],  # (9)
```

1. See [:material-code-braces: ScopeTypeDef](./type_defs.md#scopetypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-brackets: EnhancedInfrastructureMetricsType](./literals.md#enhancedinfrastructuremetricstype) 
4. See [:material-code-brackets: InferredWorkloadTypesPreferenceType](./literals.md#inferredworkloadtypespreferencetype) 
5. See [:material-code-braces: ExternalMetricsPreferenceTypeDef](./type_defs.md#externalmetricspreferencetypedef) 
6. See [:material-code-brackets: LookBackPeriodPreferenceType](./literals.md#lookbackperiodpreferencetype) 
7. See [:material-code-braces: UtilizationPreferenceTypeDef](./type_defs.md#utilizationpreferencetypedef) 
8. See [:material-code-braces: EffectivePreferredResourceTypeDef](./type_defs.md#effectivepreferredresourcetypedef) 
9. See [:material-code-brackets: SavingsEstimationModeType](./literals.md#savingsestimationmodetype) 
## GetECSServiceRecommendationProjectedMetricsResponseTypeDef

```python
# GetECSServiceRecommendationProjectedMetricsResponseTypeDef definition

class GetECSServiceRecommendationProjectedMetricsResponseTypeDef(TypedDict):
    recommendedOptionProjectedMetrics: List[ECSServiceRecommendedOptionProjectedMetricTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ECSServiceRecommendedOptionProjectedMetricTypeDef](./type_defs.md#ecsservicerecommendedoptionprojectedmetrictypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ECSServiceRecommendationOptionTypeDef

```python
# ECSServiceRecommendationOptionTypeDef definition

class ECSServiceRecommendationOptionTypeDef(TypedDict):
    memory: NotRequired[int],
    cpu: NotRequired[int],
    savingsOpportunity: NotRequired[SavingsOpportunityTypeDef],  # (1)
    savingsOpportunityAfterDiscounts: NotRequired[ECSSavingsOpportunityAfterDiscountsTypeDef],  # (2)
    projectedUtilizationMetrics: NotRequired[List[ECSServiceProjectedUtilizationMetricTypeDef]],  # (3)
    containerRecommendations: NotRequired[List[ContainerRecommendationTypeDef]],  # (4)
```

1. See [:material-code-braces: SavingsOpportunityTypeDef](./type_defs.md#savingsopportunitytypedef) 
2. See [:material-code-braces: ECSSavingsOpportunityAfterDiscountsTypeDef](./type_defs.md#ecssavingsopportunityafterdiscountstypedef) 
3. See [:material-code-braces: ECSServiceProjectedUtilizationMetricTypeDef](./type_defs.md#ecsserviceprojectedutilizationmetrictypedef) 
4. See [:material-code-braces: ContainerRecommendationTypeDef](./type_defs.md#containerrecommendationtypedef) 
## LicenseRecommendationOptionTypeDef

```python
# LicenseRecommendationOptionTypeDef definition

class LicenseRecommendationOptionTypeDef(TypedDict):
    rank: NotRequired[int],
    operatingSystem: NotRequired[str],
    licenseEdition: NotRequired[LicenseEditionType],  # (1)
    licenseModel: NotRequired[LicenseModelType],  # (2)
    savingsOpportunity: NotRequired[SavingsOpportunityTypeDef],  # (3)
```

1. See [:material-code-brackets: LicenseEditionType](./literals.md#licenseeditiontype) 
2. See [:material-code-brackets: LicenseModelType](./literals.md#licensemodeltype) 
3. See [:material-code-braces: SavingsOpportunityTypeDef](./type_defs.md#savingsopportunitytypedef) 
## VolumeRecommendationOptionTypeDef

```python
# VolumeRecommendationOptionTypeDef definition

class VolumeRecommendationOptionTypeDef(TypedDict):
    configuration: NotRequired[VolumeConfigurationTypeDef],  # (1)
    performanceRisk: NotRequired[float],
    rank: NotRequired[int],
    savingsOpportunity: NotRequired[SavingsOpportunityTypeDef],  # (2)
    savingsOpportunityAfterDiscounts: NotRequired[EBSSavingsOpportunityAfterDiscountsTypeDef],  # (3)
```

1. See [:material-code-braces: VolumeConfigurationTypeDef](./type_defs.md#volumeconfigurationtypedef) 
2. See [:material-code-braces: SavingsOpportunityTypeDef](./type_defs.md#savingsopportunitytypedef) 
3. See [:material-code-braces: EBSSavingsOpportunityAfterDiscountsTypeDef](./type_defs.md#ebssavingsopportunityafterdiscountstypedef) 
## RecommendationExportJobTypeDef

```python
# RecommendationExportJobTypeDef definition

class RecommendationExportJobTypeDef(TypedDict):
    jobId: NotRequired[str],
    destination: NotRequired[ExportDestinationTypeDef],  # (1)
    resourceType: NotRequired[ResourceTypeType],  # (2)
    status: NotRequired[JobStatusType],  # (3)
    creationTimestamp: NotRequired[datetime],
    lastUpdatedTimestamp: NotRequired[datetime],
    failureReason: NotRequired[str],
```

1. See [:material-code-braces: ExportDestinationTypeDef](./type_defs.md#exportdestinationtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## AutoScalingGroupRecommendationOptionTypeDef

```python
# AutoScalingGroupRecommendationOptionTypeDef definition

class AutoScalingGroupRecommendationOptionTypeDef(TypedDict):
    configuration: NotRequired[AutoScalingGroupConfigurationTypeDef],  # (1)
    instanceGpuInfo: NotRequired[GpuInfoTypeDef],  # (2)
    projectedUtilizationMetrics: NotRequired[List[UtilizationMetricTypeDef]],  # (3)
    performanceRisk: NotRequired[float],
    rank: NotRequired[int],
    savingsOpportunity: NotRequired[SavingsOpportunityTypeDef],  # (4)
    savingsOpportunityAfterDiscounts: NotRequired[AutoScalingGroupSavingsOpportunityAfterDiscountsTypeDef],  # (5)
    migrationEffort: NotRequired[MigrationEffortType],  # (6)
```

1. See [:material-code-braces: AutoScalingGroupConfigurationTypeDef](./type_defs.md#autoscalinggroupconfigurationtypedef) 
2. See [:material-code-braces: GpuInfoTypeDef](./type_defs.md#gpuinfotypedef) 
3. See [:material-code-braces: UtilizationMetricTypeDef](./type_defs.md#utilizationmetrictypedef) 
4. See [:material-code-braces: SavingsOpportunityTypeDef](./type_defs.md#savingsopportunitytypedef) 
5. See [:material-code-braces: AutoScalingGroupSavingsOpportunityAfterDiscountsTypeDef](./type_defs.md#autoscalinggroupsavingsopportunityafterdiscountstypedef) 
6. See [:material-code-brackets: MigrationEffortType](./literals.md#migrationefforttype) 
## InstanceRecommendationOptionTypeDef

```python
# InstanceRecommendationOptionTypeDef definition

class InstanceRecommendationOptionTypeDef(TypedDict):
    instanceType: NotRequired[str],
    instanceGpuInfo: NotRequired[GpuInfoTypeDef],  # (1)
    projectedUtilizationMetrics: NotRequired[List[UtilizationMetricTypeDef]],  # (2)
    platformDifferences: NotRequired[List[PlatformDifferenceType]],  # (3)
    performanceRisk: NotRequired[float],
    rank: NotRequired[int],
    savingsOpportunity: NotRequired[SavingsOpportunityTypeDef],  # (4)
    savingsOpportunityAfterDiscounts: NotRequired[InstanceSavingsOpportunityAfterDiscountsTypeDef],  # (5)
    migrationEffort: NotRequired[MigrationEffortType],  # (6)
```

1. See [:material-code-braces: GpuInfoTypeDef](./type_defs.md#gpuinfotypedef) 
2. See [:material-code-braces: UtilizationMetricTypeDef](./type_defs.md#utilizationmetrictypedef) 
3. See [:material-code-brackets: PlatformDifferenceType](./literals.md#platformdifferencetype) 
4. See [:material-code-braces: SavingsOpportunityTypeDef](./type_defs.md#savingsopportunitytypedef) 
5. See [:material-code-braces: InstanceSavingsOpportunityAfterDiscountsTypeDef](./type_defs.md#instancesavingsopportunityafterdiscountstypedef) 
6. See [:material-code-brackets: MigrationEffortType](./literals.md#migrationefforttype) 
## LambdaFunctionMemoryRecommendationOptionTypeDef

```python
# LambdaFunctionMemoryRecommendationOptionTypeDef definition

class LambdaFunctionMemoryRecommendationOptionTypeDef(TypedDict):
    rank: NotRequired[int],
    memorySize: NotRequired[int],
    projectedUtilizationMetrics: NotRequired[List[LambdaFunctionMemoryProjectedMetricTypeDef]],  # (1)
    savingsOpportunity: NotRequired[SavingsOpportunityTypeDef],  # (2)
    savingsOpportunityAfterDiscounts: NotRequired[LambdaSavingsOpportunityAfterDiscountsTypeDef],  # (3)
```

1. See [:material-code-braces: LambdaFunctionMemoryProjectedMetricTypeDef](./type_defs.md#lambdafunctionmemoryprojectedmetrictypedef) 
2. See [:material-code-braces: SavingsOpportunityTypeDef](./type_defs.md#savingsopportunitytypedef) 
3. See [:material-code-braces: LambdaSavingsOpportunityAfterDiscountsTypeDef](./type_defs.md#lambdasavingsopportunityafterdiscountstypedef) 
## GetEC2RecommendationProjectedMetricsResponseTypeDef

```python
# GetEC2RecommendationProjectedMetricsResponseTypeDef definition

class GetEC2RecommendationProjectedMetricsResponseTypeDef(TypedDict):
    recommendedOptionProjectedMetrics: List[RecommendedOptionProjectedMetricTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecommendedOptionProjectedMetricTypeDef](./type_defs.md#recommendedoptionprojectedmetrictypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRDSDatabaseRecommendationProjectedMetricsResponseTypeDef

```python
# GetRDSDatabaseRecommendationProjectedMetricsResponseTypeDef definition

class GetRDSDatabaseRecommendationProjectedMetricsResponseTypeDef(TypedDict):
    recommendedOptionProjectedMetrics: List[RDSDatabaseRecommendedOptionProjectedMetricTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RDSDatabaseRecommendedOptionProjectedMetricTypeDef](./type_defs.md#rdsdatabaserecommendedoptionprojectedmetrictypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RDSDBInstanceRecommendationOptionTypeDef

```python
# RDSDBInstanceRecommendationOptionTypeDef definition

class RDSDBInstanceRecommendationOptionTypeDef(TypedDict):
    dbInstanceClass: NotRequired[str],
    projectedUtilizationMetrics: NotRequired[List[RDSDBUtilizationMetricTypeDef]],  # (1)
    performanceRisk: NotRequired[float],
    rank: NotRequired[int],
    savingsOpportunity: NotRequired[SavingsOpportunityTypeDef],  # (2)
    savingsOpportunityAfterDiscounts: NotRequired[RDSInstanceSavingsOpportunityAfterDiscountsTypeDef],  # (3)
```

1. See [:material-code-braces: RDSDBUtilizationMetricTypeDef](./type_defs.md#rdsdbutilizationmetrictypedef) 
2. See [:material-code-braces: SavingsOpportunityTypeDef](./type_defs.md#savingsopportunitytypedef) 
3. See [:material-code-braces: RDSInstanceSavingsOpportunityAfterDiscountsTypeDef](./type_defs.md#rdsinstancesavingsopportunityafterdiscountstypedef) 
## RDSDBStorageRecommendationOptionTypeDef

```python
# RDSDBStorageRecommendationOptionTypeDef definition

class RDSDBStorageRecommendationOptionTypeDef(TypedDict):
    storageConfiguration: NotRequired[DBStorageConfigurationTypeDef],  # (1)
    rank: NotRequired[int],
    savingsOpportunity: NotRequired[SavingsOpportunityTypeDef],  # (2)
    savingsOpportunityAfterDiscounts: NotRequired[RDSStorageSavingsOpportunityAfterDiscountsTypeDef],  # (3)
```

1. See [:material-code-braces: DBStorageConfigurationTypeDef](./type_defs.md#dbstorageconfigurationtypedef) 
2. See [:material-code-braces: SavingsOpportunityTypeDef](./type_defs.md#savingsopportunitytypedef) 
3. See [:material-code-braces: RDSStorageSavingsOpportunityAfterDiscountsTypeDef](./type_defs.md#rdsstoragesavingsopportunityafterdiscountstypedef) 
## RecommendationSummaryTypeDef

```python
# RecommendationSummaryTypeDef definition

class RecommendationSummaryTypeDef(TypedDict):
    summaries: NotRequired[List[SummaryTypeDef]],  # (1)
    recommendationResourceType: NotRequired[RecommendationSourceTypeType],  # (2)
    accountId: NotRequired[str],
    savingsOpportunity: NotRequired[SavingsOpportunityTypeDef],  # (3)
    currentPerformanceRiskRatings: NotRequired[CurrentPerformanceRiskRatingsTypeDef],  # (4)
    inferredWorkloadSavings: NotRequired[List[InferredWorkloadSavingTypeDef]],  # (5)
```

1. See [:material-code-braces: SummaryTypeDef](./type_defs.md#summarytypedef) 
2. See [:material-code-brackets: RecommendationSourceTypeType](./literals.md#recommendationsourcetypetype) 
3. See [:material-code-braces: SavingsOpportunityTypeDef](./type_defs.md#savingsopportunitytypedef) 
4. See [:material-code-braces: CurrentPerformanceRiskRatingsTypeDef](./type_defs.md#currentperformanceriskratingstypedef) 
5. See [:material-code-braces: InferredWorkloadSavingTypeDef](./type_defs.md#inferredworkloadsavingtypedef) 
## GetRecommendationPreferencesResponseTypeDef

```python
# GetRecommendationPreferencesResponseTypeDef definition

class GetRecommendationPreferencesResponseTypeDef(TypedDict):
    recommendationPreferencesDetails: List[RecommendationPreferencesDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RecommendationPreferencesDetailTypeDef](./type_defs.md#recommendationpreferencesdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ECSServiceRecommendationTypeDef

```python
# ECSServiceRecommendationTypeDef definition

class ECSServiceRecommendationTypeDef(TypedDict):
    serviceArn: NotRequired[str],
    accountId: NotRequired[str],
    currentServiceConfiguration: NotRequired[ServiceConfigurationTypeDef],  # (1)
    utilizationMetrics: NotRequired[List[ECSServiceUtilizationMetricTypeDef]],  # (2)
    lookbackPeriodInDays: NotRequired[float],
    launchType: NotRequired[ECSServiceLaunchTypeType],  # (3)
    lastRefreshTimestamp: NotRequired[datetime],
    finding: NotRequired[ECSServiceRecommendationFindingType],  # (4)
    findingReasonCodes: NotRequired[List[ECSServiceRecommendationFindingReasonCodeType]],  # (5)
    serviceRecommendationOptions: NotRequired[List[ECSServiceRecommendationOptionTypeDef]],  # (6)
    currentPerformanceRisk: NotRequired[CurrentPerformanceRiskType],  # (7)
    effectiveRecommendationPreferences: NotRequired[ECSEffectiveRecommendationPreferencesTypeDef],  # (8)
    tags: NotRequired[List[TagTypeDef]],  # (9)
```

1. See [:material-code-braces: ServiceConfigurationTypeDef](./type_defs.md#serviceconfigurationtypedef) 
2. See [:material-code-braces: ECSServiceUtilizationMetricTypeDef](./type_defs.md#ecsserviceutilizationmetrictypedef) 
3. See [:material-code-brackets: ECSServiceLaunchTypeType](./literals.md#ecsservicelaunchtypetype) 
4. See [:material-code-brackets: ECSServiceRecommendationFindingType](./literals.md#ecsservicerecommendationfindingtype) 
5. See [:material-code-brackets: ECSServiceRecommendationFindingReasonCodeType](./literals.md#ecsservicerecommendationfindingreasoncodetype) 
6. See [:material-code-braces: ECSServiceRecommendationOptionTypeDef](./type_defs.md#ecsservicerecommendationoptiontypedef) 
7. See [:material-code-brackets: CurrentPerformanceRiskType](./literals.md#currentperformancerisktype) 
8. See [:material-code-braces: ECSEffectiveRecommendationPreferencesTypeDef](./type_defs.md#ecseffectiverecommendationpreferencestypedef) 
9. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## LicenseRecommendationTypeDef

```python
# LicenseRecommendationTypeDef definition

class LicenseRecommendationTypeDef(TypedDict):
    resourceArn: NotRequired[str],
    accountId: NotRequired[str],
    currentLicenseConfiguration: NotRequired[LicenseConfigurationTypeDef],  # (1)
    lookbackPeriodInDays: NotRequired[float],
    lastRefreshTimestamp: NotRequired[datetime],
    finding: NotRequired[LicenseFindingType],  # (2)
    findingReasonCodes: NotRequired[List[LicenseFindingReasonCodeType]],  # (3)
    licenseRecommendationOptions: NotRequired[List[LicenseRecommendationOptionTypeDef]],  # (4)
    tags: NotRequired[List[TagTypeDef]],  # (5)
```

1. See [:material-code-braces: LicenseConfigurationTypeDef](./type_defs.md#licenseconfigurationtypedef) 
2. See [:material-code-brackets: LicenseFindingType](./literals.md#licensefindingtype) 
3. See [:material-code-brackets: LicenseFindingReasonCodeType](./literals.md#licensefindingreasoncodetype) 
4. See [:material-code-braces: LicenseRecommendationOptionTypeDef](./type_defs.md#licenserecommendationoptiontypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## VolumeRecommendationTypeDef

```python
# VolumeRecommendationTypeDef definition

class VolumeRecommendationTypeDef(TypedDict):
    volumeArn: NotRequired[str],
    accountId: NotRequired[str],
    currentConfiguration: NotRequired[VolumeConfigurationTypeDef],  # (1)
    finding: NotRequired[EBSFindingType],  # (2)
    utilizationMetrics: NotRequired[List[EBSUtilizationMetricTypeDef]],  # (3)
    lookBackPeriodInDays: NotRequired[float],
    volumeRecommendationOptions: NotRequired[List[VolumeRecommendationOptionTypeDef]],  # (4)
    lastRefreshTimestamp: NotRequired[datetime],
    currentPerformanceRisk: NotRequired[CurrentPerformanceRiskType],  # (5)
    effectiveRecommendationPreferences: NotRequired[EBSEffectiveRecommendationPreferencesTypeDef],  # (6)
    tags: NotRequired[List[TagTypeDef]],  # (7)
```

1. See [:material-code-braces: VolumeConfigurationTypeDef](./type_defs.md#volumeconfigurationtypedef) 
2. See [:material-code-brackets: EBSFindingType](./literals.md#ebsfindingtype) 
3. See [:material-code-braces: EBSUtilizationMetricTypeDef](./type_defs.md#ebsutilizationmetrictypedef) 
4. See [:material-code-braces: VolumeRecommendationOptionTypeDef](./type_defs.md#volumerecommendationoptiontypedef) 
5. See [:material-code-brackets: CurrentPerformanceRiskType](./literals.md#currentperformancerisktype) 
6. See [:material-code-braces: EBSEffectiveRecommendationPreferencesTypeDef](./type_defs.md#ebseffectiverecommendationpreferencestypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeRecommendationExportJobsResponseTypeDef

```python
# DescribeRecommendationExportJobsResponseTypeDef definition

class DescribeRecommendationExportJobsResponseTypeDef(TypedDict):
    recommendationExportJobs: List[RecommendationExportJobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RecommendationExportJobTypeDef](./type_defs.md#recommendationexportjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AutoScalingGroupRecommendationTypeDef

```python
# AutoScalingGroupRecommendationTypeDef definition

class AutoScalingGroupRecommendationTypeDef(TypedDict):
    accountId: NotRequired[str],
    autoScalingGroupArn: NotRequired[str],
    autoScalingGroupName: NotRequired[str],
    finding: NotRequired[FindingType],  # (1)
    utilizationMetrics: NotRequired[List[UtilizationMetricTypeDef]],  # (2)
    lookBackPeriodInDays: NotRequired[float],
    currentConfiguration: NotRequired[AutoScalingGroupConfigurationTypeDef],  # (3)
    currentInstanceGpuInfo: NotRequired[GpuInfoTypeDef],  # (4)
    recommendationOptions: NotRequired[List[AutoScalingGroupRecommendationOptionTypeDef]],  # (5)
    lastRefreshTimestamp: NotRequired[datetime],
    currentPerformanceRisk: NotRequired[CurrentPerformanceRiskType],  # (6)
    effectiveRecommendationPreferences: NotRequired[EffectiveRecommendationPreferencesTypeDef],  # (7)
    inferredWorkloadTypes: NotRequired[List[InferredWorkloadTypeType]],  # (8)
```

1. See [:material-code-brackets: FindingType](./literals.md#findingtype) 
2. See [:material-code-braces: UtilizationMetricTypeDef](./type_defs.md#utilizationmetrictypedef) 
3. See [:material-code-braces: AutoScalingGroupConfigurationTypeDef](./type_defs.md#autoscalinggroupconfigurationtypedef) 
4. See [:material-code-braces: GpuInfoTypeDef](./type_defs.md#gpuinfotypedef) 
5. See [:material-code-braces: AutoScalingGroupRecommendationOptionTypeDef](./type_defs.md#autoscalinggrouprecommendationoptiontypedef) 
6. See [:material-code-brackets: CurrentPerformanceRiskType](./literals.md#currentperformancerisktype) 
7. See [:material-code-braces: EffectiveRecommendationPreferencesTypeDef](./type_defs.md#effectiverecommendationpreferencestypedef) 
8. See [:material-code-brackets: InferredWorkloadTypeType](./literals.md#inferredworkloadtypetype) 
## InstanceRecommendationTypeDef

```python
# InstanceRecommendationTypeDef definition

class InstanceRecommendationTypeDef(TypedDict):
    instanceArn: NotRequired[str],
    accountId: NotRequired[str],
    instanceName: NotRequired[str],
    currentInstanceType: NotRequired[str],
    finding: NotRequired[FindingType],  # (1)
    findingReasonCodes: NotRequired[List[InstanceRecommendationFindingReasonCodeType]],  # (2)
    utilizationMetrics: NotRequired[List[UtilizationMetricTypeDef]],  # (3)
    lookBackPeriodInDays: NotRequired[float],
    recommendationOptions: NotRequired[List[InstanceRecommendationOptionTypeDef]],  # (4)
    recommendationSources: NotRequired[List[RecommendationSourceTypeDef]],  # (5)
    lastRefreshTimestamp: NotRequired[datetime],
    currentPerformanceRisk: NotRequired[CurrentPerformanceRiskType],  # (6)
    effectiveRecommendationPreferences: NotRequired[EffectiveRecommendationPreferencesTypeDef],  # (7)
    inferredWorkloadTypes: NotRequired[List[InferredWorkloadTypeType]],  # (8)
    instanceState: NotRequired[InstanceStateType],  # (9)
    tags: NotRequired[List[TagTypeDef]],  # (10)
    externalMetricStatus: NotRequired[ExternalMetricStatusTypeDef],  # (11)
    currentInstanceGpuInfo: NotRequired[GpuInfoTypeDef],  # (12)
    idle: NotRequired[InstanceIdleType],  # (13)
```

1. See [:material-code-brackets: FindingType](./literals.md#findingtype) 
2. See [:material-code-brackets: InstanceRecommendationFindingReasonCodeType](./literals.md#instancerecommendationfindingreasoncodetype) 
3. See [:material-code-braces: UtilizationMetricTypeDef](./type_defs.md#utilizationmetrictypedef) 
4. See [:material-code-braces: InstanceRecommendationOptionTypeDef](./type_defs.md#instancerecommendationoptiontypedef) 
5. See [:material-code-braces: RecommendationSourceTypeDef](./type_defs.md#recommendationsourcetypedef) 
6. See [:material-code-brackets: CurrentPerformanceRiskType](./literals.md#currentperformancerisktype) 
7. See [:material-code-braces: EffectiveRecommendationPreferencesTypeDef](./type_defs.md#effectiverecommendationpreferencestypedef) 
8. See [:material-code-brackets: InferredWorkloadTypeType](./literals.md#inferredworkloadtypetype) 
9. See [:material-code-brackets: InstanceStateType](./literals.md#instancestatetype) 
10. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
11. See [:material-code-braces: ExternalMetricStatusTypeDef](./type_defs.md#externalmetricstatustypedef) 
12. See [:material-code-braces: GpuInfoTypeDef](./type_defs.md#gpuinfotypedef) 
13. See [:material-code-brackets: InstanceIdleType](./literals.md#instanceidletype) 
## LambdaFunctionRecommendationTypeDef

```python
# LambdaFunctionRecommendationTypeDef definition

class LambdaFunctionRecommendationTypeDef(TypedDict):
    functionArn: NotRequired[str],
    functionVersion: NotRequired[str],
    accountId: NotRequired[str],
    currentMemorySize: NotRequired[int],
    numberOfInvocations: NotRequired[int],
    utilizationMetrics: NotRequired[List[LambdaFunctionUtilizationMetricTypeDef]],  # (1)
    lookbackPeriodInDays: NotRequired[float],
    lastRefreshTimestamp: NotRequired[datetime],
    finding: NotRequired[LambdaFunctionRecommendationFindingType],  # (2)
    findingReasonCodes: NotRequired[List[LambdaFunctionRecommendationFindingReasonCodeType]],  # (3)
    memorySizeRecommendationOptions: NotRequired[List[LambdaFunctionMemoryRecommendationOptionTypeDef]],  # (4)
    currentPerformanceRisk: NotRequired[CurrentPerformanceRiskType],  # (5)
    effectiveRecommendationPreferences: NotRequired[LambdaEffectiveRecommendationPreferencesTypeDef],  # (6)
    tags: NotRequired[List[TagTypeDef]],  # (7)
```

1. See [:material-code-braces: LambdaFunctionUtilizationMetricTypeDef](./type_defs.md#lambdafunctionutilizationmetrictypedef) 
2. See [:material-code-brackets: LambdaFunctionRecommendationFindingType](./literals.md#lambdafunctionrecommendationfindingtype) 
3. See [:material-code-brackets: LambdaFunctionRecommendationFindingReasonCodeType](./literals.md#lambdafunctionrecommendationfindingreasoncodetype) 
4. See [:material-code-braces: LambdaFunctionMemoryRecommendationOptionTypeDef](./type_defs.md#lambdafunctionmemoryrecommendationoptiontypedef) 
5. See [:material-code-brackets: CurrentPerformanceRiskType](./literals.md#currentperformancerisktype) 
6. See [:material-code-braces: LambdaEffectiveRecommendationPreferencesTypeDef](./type_defs.md#lambdaeffectiverecommendationpreferencestypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## RDSDBRecommendationTypeDef

```python
# RDSDBRecommendationTypeDef definition

class RDSDBRecommendationTypeDef(TypedDict):
    resourceArn: NotRequired[str],
    accountId: NotRequired[str],
    engine: NotRequired[str],
    engineVersion: NotRequired[str],
    currentDBInstanceClass: NotRequired[str],
    currentStorageConfiguration: NotRequired[DBStorageConfigurationTypeDef],  # (1)
    idle: NotRequired[IdleType],  # (2)
    instanceFinding: NotRequired[RDSInstanceFindingType],  # (3)
    storageFinding: NotRequired[RDSStorageFindingType],  # (4)
    instanceFindingReasonCodes: NotRequired[List[RDSInstanceFindingReasonCodeType]],  # (5)
    storageFindingReasonCodes: NotRequired[List[RDSStorageFindingReasonCodeType]],  # (6)
    instanceRecommendationOptions: NotRequired[List[RDSDBInstanceRecommendationOptionTypeDef]],  # (7)
    storageRecommendationOptions: NotRequired[List[RDSDBStorageRecommendationOptionTypeDef]],  # (8)
    utilizationMetrics: NotRequired[List[RDSDBUtilizationMetricTypeDef]],  # (9)
    effectiveRecommendationPreferences: NotRequired[RDSEffectiveRecommendationPreferencesTypeDef],  # (10)
    lookbackPeriodInDays: NotRequired[float],
    lastRefreshTimestamp: NotRequired[datetime],
    tags: NotRequired[List[TagTypeDef]],  # (11)
```

1. See [:material-code-braces: DBStorageConfigurationTypeDef](./type_defs.md#dbstorageconfigurationtypedef) 
2. See [:material-code-brackets: IdleType](./literals.md#idletype) 
3. See [:material-code-brackets: RDSInstanceFindingType](./literals.md#rdsinstancefindingtype) 
4. See [:material-code-brackets: RDSStorageFindingType](./literals.md#rdsstoragefindingtype) 
5. See [:material-code-brackets: RDSInstanceFindingReasonCodeType](./literals.md#rdsinstancefindingreasoncodetype) 
6. See [:material-code-brackets: RDSStorageFindingReasonCodeType](./literals.md#rdsstoragefindingreasoncodetype) 
7. See [:material-code-braces: RDSDBInstanceRecommendationOptionTypeDef](./type_defs.md#rdsdbinstancerecommendationoptiontypedef) 
8. See [:material-code-braces: RDSDBStorageRecommendationOptionTypeDef](./type_defs.md#rdsdbstoragerecommendationoptiontypedef) 
9. See [:material-code-braces: RDSDBUtilizationMetricTypeDef](./type_defs.md#rdsdbutilizationmetrictypedef) 
10. See [:material-code-braces: RDSEffectiveRecommendationPreferencesTypeDef](./type_defs.md#rdseffectiverecommendationpreferencestypedef) 
11. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetRecommendationSummariesResponseTypeDef

```python
# GetRecommendationSummariesResponseTypeDef definition

class GetRecommendationSummariesResponseTypeDef(TypedDict):
    recommendationSummaries: List[RecommendationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RecommendationSummaryTypeDef](./type_defs.md#recommendationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetECSServiceRecommendationsResponseTypeDef

```python
# GetECSServiceRecommendationsResponseTypeDef definition

class GetECSServiceRecommendationsResponseTypeDef(TypedDict):
    ecsServiceRecommendations: List[ECSServiceRecommendationTypeDef],  # (1)
    errors: List[GetRecommendationErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ECSServiceRecommendationTypeDef](./type_defs.md#ecsservicerecommendationtypedef) 
2. See [:material-code-braces: GetRecommendationErrorTypeDef](./type_defs.md#getrecommendationerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLicenseRecommendationsResponseTypeDef

```python
# GetLicenseRecommendationsResponseTypeDef definition

class GetLicenseRecommendationsResponseTypeDef(TypedDict):
    licenseRecommendations: List[LicenseRecommendationTypeDef],  # (1)
    errors: List[GetRecommendationErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LicenseRecommendationTypeDef](./type_defs.md#licenserecommendationtypedef) 
2. See [:material-code-braces: GetRecommendationErrorTypeDef](./type_defs.md#getrecommendationerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEBSVolumeRecommendationsResponseTypeDef

```python
# GetEBSVolumeRecommendationsResponseTypeDef definition

class GetEBSVolumeRecommendationsResponseTypeDef(TypedDict):
    volumeRecommendations: List[VolumeRecommendationTypeDef],  # (1)
    errors: List[GetRecommendationErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: VolumeRecommendationTypeDef](./type_defs.md#volumerecommendationtypedef) 
2. See [:material-code-braces: GetRecommendationErrorTypeDef](./type_defs.md#getrecommendationerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAutoScalingGroupRecommendationsResponseTypeDef

```python
# GetAutoScalingGroupRecommendationsResponseTypeDef definition

class GetAutoScalingGroupRecommendationsResponseTypeDef(TypedDict):
    autoScalingGroupRecommendations: List[AutoScalingGroupRecommendationTypeDef],  # (1)
    errors: List[GetRecommendationErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AutoScalingGroupRecommendationTypeDef](./type_defs.md#autoscalinggrouprecommendationtypedef) 
2. See [:material-code-braces: GetRecommendationErrorTypeDef](./type_defs.md#getrecommendationerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEC2InstanceRecommendationsResponseTypeDef

```python
# GetEC2InstanceRecommendationsResponseTypeDef definition

class GetEC2InstanceRecommendationsResponseTypeDef(TypedDict):
    instanceRecommendations: List[InstanceRecommendationTypeDef],  # (1)
    errors: List[GetRecommendationErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: InstanceRecommendationTypeDef](./type_defs.md#instancerecommendationtypedef) 
2. See [:material-code-braces: GetRecommendationErrorTypeDef](./type_defs.md#getrecommendationerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLambdaFunctionRecommendationsResponseTypeDef

```python
# GetLambdaFunctionRecommendationsResponseTypeDef definition

class GetLambdaFunctionRecommendationsResponseTypeDef(TypedDict):
    lambdaFunctionRecommendations: List[LambdaFunctionRecommendationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LambdaFunctionRecommendationTypeDef](./type_defs.md#lambdafunctionrecommendationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRDSDatabaseRecommendationsResponseTypeDef

```python
# GetRDSDatabaseRecommendationsResponseTypeDef definition

class GetRDSDatabaseRecommendationsResponseTypeDef(TypedDict):
    rdsDBRecommendations: List[RDSDBRecommendationTypeDef],  # (1)
    errors: List[GetRecommendationErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RDSDBRecommendationTypeDef](./type_defs.md#rdsdbrecommendationtypedef) 
2. See [:material-code-braces: GetRecommendationErrorTypeDef](./type_defs.md#getrecommendationerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
