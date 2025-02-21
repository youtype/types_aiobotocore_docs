# Type definitions

> [Index](../README.md) > [ComputeOptimizer](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ComputeOptimizer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#computeoptimizer)
    type annotations stubs module [types-aiobotocore-compute-optimizer](https://pypi.org/project/types-aiobotocore-compute-optimizer/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_compute_optimizer.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AccountEnrollmentStatusTypeDef

```python
# AccountEnrollmentStatusTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import AccountEnrollmentStatusTypeDef


def get_value() -> AccountEnrollmentStatusTypeDef:
    return {
        "accountId": ...,
    }


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
# AutoScalingGroupConfigurationTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import AutoScalingGroupConfigurationTypeDef


def get_value() -> AutoScalingGroupConfigurationTypeDef:
    return {
        "desiredCapacity": ...,
    }


# AutoScalingGroupConfigurationTypeDef definition

class AutoScalingGroupConfigurationTypeDef(TypedDict):
    desiredCapacity: NotRequired[int],
    minSize: NotRequired[int],
    maxSize: NotRequired[int],
    instanceType: NotRequired[str],
    allocationStrategy: NotRequired[AllocationStrategyType],  # (1)
    estimatedInstanceHourReductionPercentage: NotRequired[float],
    type: NotRequired[AsgTypeType],  # (2)
    mixedInstanceTypes: NotRequired[List[str]],
```

1. See [:material-code-brackets: AllocationStrategyType](./literals.md#allocationstrategytype) 
2. See [:material-code-brackets: AsgTypeType](./literals.md#asgtypetype) 
## AutoScalingGroupEstimatedMonthlySavingsTypeDef

```python
# AutoScalingGroupEstimatedMonthlySavingsTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import AutoScalingGroupEstimatedMonthlySavingsTypeDef


def get_value() -> AutoScalingGroupEstimatedMonthlySavingsTypeDef:
    return {
        "currency": ...,
    }


# AutoScalingGroupEstimatedMonthlySavingsTypeDef definition

class AutoScalingGroupEstimatedMonthlySavingsTypeDef(TypedDict):
    currency: NotRequired[CurrencyType],  # (1)
    value: NotRequired[float],
```

1. See [:material-code-brackets: CurrencyType](./literals.md#currencytype) 
## UtilizationMetricTypeDef

```python
# UtilizationMetricTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import UtilizationMetricTypeDef


def get_value() -> UtilizationMetricTypeDef:
    return {
        "name": ...,
    }


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
# MemorySizeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import MemorySizeConfigurationTypeDef


def get_value() -> MemorySizeConfigurationTypeDef:
    return {
        "memory": ...,
    }


# MemorySizeConfigurationTypeDef definition

class MemorySizeConfigurationTypeDef(TypedDict):
    memory: NotRequired[int],
    memoryReservation: NotRequired[int],
```

## CurrentPerformanceRiskRatingsTypeDef

```python
# CurrentPerformanceRiskRatingsTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import CurrentPerformanceRiskRatingsTypeDef


def get_value() -> CurrentPerformanceRiskRatingsTypeDef:
    return {
        "high": ...,
    }


# CurrentPerformanceRiskRatingsTypeDef definition

class CurrentPerformanceRiskRatingsTypeDef(TypedDict):
    high: NotRequired[int],
    medium: NotRequired[int],
    low: NotRequired[int],
    veryLow: NotRequired[int],
```

## CustomizableMetricParametersTypeDef

```python
# CustomizableMetricParametersTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import CustomizableMetricParametersTypeDef


def get_value() -> CustomizableMetricParametersTypeDef:
    return {
        "threshold": ...,
    }


# CustomizableMetricParametersTypeDef definition

class CustomizableMetricParametersTypeDef(TypedDict):
    threshold: NotRequired[CustomizableMetricThresholdType],  # (1)
    headroom: NotRequired[CustomizableMetricHeadroomType],  # (2)
```

1. See [:material-code-brackets: CustomizableMetricThresholdType](./literals.md#customizablemetricthresholdtype) 
2. See [:material-code-brackets: CustomizableMetricHeadroomType](./literals.md#customizablemetricheadroomtype) 
## DBStorageConfigurationTypeDef

```python
# DBStorageConfigurationTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import DBStorageConfigurationTypeDef


def get_value() -> DBStorageConfigurationTypeDef:
    return {
        "storageType": ...,
    }


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
# ScopeTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ScopeTypeDef


def get_value() -> ScopeTypeDef:
    return {
        "name": ...,
    }


# ScopeTypeDef definition

class ScopeTypeDef(TypedDict):
    name: NotRequired[ScopeNameType],  # (1)
    value: NotRequired[str],
```

1. See [:material-code-brackets: ScopeNameType](./literals.md#scopenametype) 
## JobFilterTypeDef

```python
# JobFilterTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import JobFilterTypeDef


def get_value() -> JobFilterTypeDef:
    return {
        "name": ...,
    }


# JobFilterTypeDef definition

class JobFilterTypeDef(TypedDict):
    name: NotRequired[JobFilterNameType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: JobFilterNameType](./literals.md#jobfilternametype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import PaginatorConfigTypeDef


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

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ResponseMetadataTypeDef


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

## EBSSavingsEstimationModeTypeDef

```python
# EBSSavingsEstimationModeTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import EBSSavingsEstimationModeTypeDef


def get_value() -> EBSSavingsEstimationModeTypeDef:
    return {
        "source": ...,
    }


# EBSSavingsEstimationModeTypeDef definition

class EBSSavingsEstimationModeTypeDef(TypedDict):
    source: NotRequired[EBSSavingsEstimationModeSourceType],  # (1)
```

1. See [:material-code-brackets: EBSSavingsEstimationModeSourceType](./literals.md#ebssavingsestimationmodesourcetype) 
## EBSEstimatedMonthlySavingsTypeDef

```python
# EBSEstimatedMonthlySavingsTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import EBSEstimatedMonthlySavingsTypeDef


def get_value() -> EBSEstimatedMonthlySavingsTypeDef:
    return {
        "currency": ...,
    }


# EBSEstimatedMonthlySavingsTypeDef definition

class EBSEstimatedMonthlySavingsTypeDef(TypedDict):
    currency: NotRequired[CurrencyType],  # (1)
    value: NotRequired[float],
```

1. See [:material-code-brackets: CurrencyType](./literals.md#currencytype) 
## EBSFilterTypeDef

```python
# EBSFilterTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import EBSFilterTypeDef


def get_value() -> EBSFilterTypeDef:
    return {
        "name": ...,
    }


# EBSFilterTypeDef definition

class EBSFilterTypeDef(TypedDict):
    name: NotRequired[EBSFilterNameType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: EBSFilterNameType](./literals.md#ebsfilternametype) 
## EBSUtilizationMetricTypeDef

```python
# EBSUtilizationMetricTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import EBSUtilizationMetricTypeDef


def get_value() -> EBSUtilizationMetricTypeDef:
    return {
        "name": ...,
    }


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
# ECSSavingsEstimationModeTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ECSSavingsEstimationModeTypeDef


def get_value() -> ECSSavingsEstimationModeTypeDef:
    return {
        "source": ...,
    }


# ECSSavingsEstimationModeTypeDef definition

class ECSSavingsEstimationModeTypeDef(TypedDict):
    source: NotRequired[ECSSavingsEstimationModeSourceType],  # (1)
```

1. See [:material-code-brackets: ECSSavingsEstimationModeSourceType](./literals.md#ecssavingsestimationmodesourcetype) 
## ECSEstimatedMonthlySavingsTypeDef

```python
# ECSEstimatedMonthlySavingsTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ECSEstimatedMonthlySavingsTypeDef


def get_value() -> ECSEstimatedMonthlySavingsTypeDef:
    return {
        "currency": ...,
    }


# ECSEstimatedMonthlySavingsTypeDef definition

class ECSEstimatedMonthlySavingsTypeDef(TypedDict):
    currency: NotRequired[CurrencyType],  # (1)
    value: NotRequired[float],
```

1. See [:material-code-brackets: CurrencyType](./literals.md#currencytype) 
## ECSServiceProjectedMetricTypeDef

```python
# ECSServiceProjectedMetricTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ECSServiceProjectedMetricTypeDef


def get_value() -> ECSServiceProjectedMetricTypeDef:
    return {
        "name": ...,
    }


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
# ECSServiceProjectedUtilizationMetricTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ECSServiceProjectedUtilizationMetricTypeDef


def get_value() -> ECSServiceProjectedUtilizationMetricTypeDef:
    return {
        "name": ...,
    }


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
# ECSServiceRecommendationFilterTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ECSServiceRecommendationFilterTypeDef


def get_value() -> ECSServiceRecommendationFilterTypeDef:
    return {
        "name": ...,
    }


# ECSServiceRecommendationFilterTypeDef definition

class ECSServiceRecommendationFilterTypeDef(TypedDict):
    name: NotRequired[ECSServiceRecommendationFilterNameType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: ECSServiceRecommendationFilterNameType](./literals.md#ecsservicerecommendationfilternametype) 
## ECSServiceUtilizationMetricTypeDef

```python
# ECSServiceUtilizationMetricTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ECSServiceUtilizationMetricTypeDef


def get_value() -> ECSServiceUtilizationMetricTypeDef:
    return {
        "name": ...,
    }


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
# TagTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[str],
```

## EffectivePreferredResourceTypeDef

```python
# EffectivePreferredResourceTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import EffectivePreferredResourceTypeDef


def get_value() -> EffectivePreferredResourceTypeDef:
    return {
        "name": ...,
    }


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
# ExternalMetricsPreferenceTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ExternalMetricsPreferenceTypeDef


def get_value() -> ExternalMetricsPreferenceTypeDef:
    return {
        "source": ...,
    }


# ExternalMetricsPreferenceTypeDef definition

class ExternalMetricsPreferenceTypeDef(TypedDict):
    source: NotRequired[ExternalMetricsSourceType],  # (1)
```

1. See [:material-code-brackets: ExternalMetricsSourceType](./literals.md#externalmetricssourcetype) 
## InstanceSavingsEstimationModeTypeDef

```python
# InstanceSavingsEstimationModeTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import InstanceSavingsEstimationModeTypeDef


def get_value() -> InstanceSavingsEstimationModeTypeDef:
    return {
        "source": ...,
    }


# InstanceSavingsEstimationModeTypeDef definition

class InstanceSavingsEstimationModeTypeDef(TypedDict):
    source: NotRequired[InstanceSavingsEstimationModeSourceType],  # (1)
```

1. See [:material-code-brackets: InstanceSavingsEstimationModeSourceType](./literals.md#instancesavingsestimationmodesourcetype) 
## EnrollmentFilterTypeDef

```python
# EnrollmentFilterTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import EnrollmentFilterTypeDef


def get_value() -> EnrollmentFilterTypeDef:
    return {
        "name": ...,
    }


# EnrollmentFilterTypeDef definition

class EnrollmentFilterTypeDef(TypedDict):
    name: NotRequired[EnrollmentFilterNameType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: EnrollmentFilterNameType](./literals.md#enrollmentfilternametype) 
## EstimatedMonthlySavingsTypeDef

```python
# EstimatedMonthlySavingsTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import EstimatedMonthlySavingsTypeDef


def get_value() -> EstimatedMonthlySavingsTypeDef:
    return {
        "currency": ...,
    }


# EstimatedMonthlySavingsTypeDef definition

class EstimatedMonthlySavingsTypeDef(TypedDict):
    currency: NotRequired[CurrencyType],  # (1)
    value: NotRequired[float],
```

1. See [:material-code-brackets: CurrencyType](./literals.md#currencytype) 
## FilterTypeDef

```python
# FilterTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import FilterTypeDef


def get_value() -> FilterTypeDef:
    return {
        "name": ...,
    }


# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    name: NotRequired[FilterNameType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: FilterNameType](./literals.md#filternametype) 
## RecommendationPreferencesTypeDef

```python
# RecommendationPreferencesTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import RecommendationPreferencesTypeDef


def get_value() -> RecommendationPreferencesTypeDef:
    return {
        "cpuVendorArchitectures": ...,
    }


# RecommendationPreferencesTypeDef definition

class RecommendationPreferencesTypeDef(TypedDict):
    cpuVendorArchitectures: NotRequired[Sequence[CpuVendorArchitectureType]],  # (1)
```

1. See [:material-code-brackets: CpuVendorArchitectureType](./literals.md#cpuvendorarchitecturetype) 
## S3DestinationConfigTypeDef

```python
# S3DestinationConfigTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import S3DestinationConfigTypeDef


def get_value() -> S3DestinationConfigTypeDef:
    return {
        "bucket": ...,
    }


# S3DestinationConfigTypeDef definition

class S3DestinationConfigTypeDef(TypedDict):
    bucket: NotRequired[str],
    keyPrefix: NotRequired[str],
```

## S3DestinationTypeDef

```python
# S3DestinationTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import S3DestinationTypeDef


def get_value() -> S3DestinationTypeDef:
    return {
        "bucket": ...,
    }


# S3DestinationTypeDef definition

class S3DestinationTypeDef(TypedDict):
    bucket: NotRequired[str],
    key: NotRequired[str],
    metadataKey: NotRequired[str],
```

## IdleRecommendationFilterTypeDef

```python
# IdleRecommendationFilterTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import IdleRecommendationFilterTypeDef


def get_value() -> IdleRecommendationFilterTypeDef:
    return {
        "name": ...,
    }


# IdleRecommendationFilterTypeDef definition

class IdleRecommendationFilterTypeDef(TypedDict):
    name: NotRequired[IdleRecommendationFilterNameType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: IdleRecommendationFilterNameType](./literals.md#idlerecommendationfilternametype) 
## LambdaFunctionRecommendationFilterTypeDef

```python
# LambdaFunctionRecommendationFilterTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import LambdaFunctionRecommendationFilterTypeDef


def get_value() -> LambdaFunctionRecommendationFilterTypeDef:
    return {
        "name": ...,
    }


# LambdaFunctionRecommendationFilterTypeDef definition

class LambdaFunctionRecommendationFilterTypeDef(TypedDict):
    name: NotRequired[LambdaFunctionRecommendationFilterNameType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: LambdaFunctionRecommendationFilterNameType](./literals.md#lambdafunctionrecommendationfilternametype) 
## LicenseRecommendationFilterTypeDef

```python
# LicenseRecommendationFilterTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import LicenseRecommendationFilterTypeDef


def get_value() -> LicenseRecommendationFilterTypeDef:
    return {
        "name": ...,
    }


# LicenseRecommendationFilterTypeDef definition

class LicenseRecommendationFilterTypeDef(TypedDict):
    name: NotRequired[LicenseRecommendationFilterNameType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: LicenseRecommendationFilterNameType](./literals.md#licenserecommendationfilternametype) 
## RDSDBRecommendationFilterTypeDef

```python
# RDSDBRecommendationFilterTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import RDSDBRecommendationFilterTypeDef


def get_value() -> RDSDBRecommendationFilterTypeDef:
    return {
        "name": ...,
    }


# RDSDBRecommendationFilterTypeDef definition

class RDSDBRecommendationFilterTypeDef(TypedDict):
    name: NotRequired[RDSDBRecommendationFilterNameType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: RDSDBRecommendationFilterNameType](./literals.md#rdsdbrecommendationfilternametype) 
## ExternalMetricStatusTypeDef

```python
# ExternalMetricStatusTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ExternalMetricStatusTypeDef


def get_value() -> ExternalMetricStatusTypeDef:
    return {
        "statusCode": ...,
    }


# ExternalMetricStatusTypeDef definition

class ExternalMetricStatusTypeDef(TypedDict):
    statusCode: NotRequired[ExternalMetricStatusCodeType],  # (1)
    statusReason: NotRequired[str],
```

1. See [:material-code-brackets: ExternalMetricStatusCodeType](./literals.md#externalmetricstatuscodetype) 
## GetRecommendationErrorTypeDef

```python
# GetRecommendationErrorTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetRecommendationErrorTypeDef


def get_value() -> GetRecommendationErrorTypeDef:
    return {
        "identifier": ...,
    }


# GetRecommendationErrorTypeDef definition

class GetRecommendationErrorTypeDef(TypedDict):
    identifier: NotRequired[str],
    code: NotRequired[str],
    message: NotRequired[str],
```

## GetEffectiveRecommendationPreferencesRequestTypeDef

```python
# GetEffectiveRecommendationPreferencesRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetEffectiveRecommendationPreferencesRequestTypeDef


def get_value() -> GetEffectiveRecommendationPreferencesRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# GetEffectiveRecommendationPreferencesRequestTypeDef definition

class GetEffectiveRecommendationPreferencesRequestTypeDef(TypedDict):
    resourceArn: str,
```

## OrderByTypeDef

```python
# OrderByTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import OrderByTypeDef


def get_value() -> OrderByTypeDef:
    return {
        "dimension": ...,
    }


# OrderByTypeDef definition

class OrderByTypeDef(TypedDict):
    dimension: NotRequired[DimensionType],  # (1)
    order: NotRequired[OrderType],  # (2)
```

1. See [:material-code-brackets: DimensionType](./literals.md#dimensiontype) 
2. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
## IdleRecommendationErrorTypeDef

```python
# IdleRecommendationErrorTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import IdleRecommendationErrorTypeDef


def get_value() -> IdleRecommendationErrorTypeDef:
    return {
        "identifier": ...,
    }


# IdleRecommendationErrorTypeDef definition

class IdleRecommendationErrorTypeDef(TypedDict):
    identifier: NotRequired[str],
    code: NotRequired[str],
    message: NotRequired[str],
    resourceType: NotRequired[IdleRecommendationResourceTypeType],  # (1)
```

1. See [:material-code-brackets: IdleRecommendationResourceTypeType](./literals.md#idlerecommendationresourcetypetype) 
## GetRecommendationSummariesRequestTypeDef

```python
# GetRecommendationSummariesRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetRecommendationSummariesRequestTypeDef


def get_value() -> GetRecommendationSummariesRequestTypeDef:
    return {
        "accountIds": ...,
    }


# GetRecommendationSummariesRequestTypeDef definition

class GetRecommendationSummariesRequestTypeDef(TypedDict):
    accountIds: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GpuTypeDef

```python
# GpuTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GpuTypeDef


def get_value() -> GpuTypeDef:
    return {
        "gpuCount": ...,
    }


# GpuTypeDef definition

class GpuTypeDef(TypedDict):
    gpuCount: NotRequired[int],
    gpuMemorySizeInMiB: NotRequired[int],
```

## IdleEstimatedMonthlySavingsTypeDef

```python
# IdleEstimatedMonthlySavingsTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import IdleEstimatedMonthlySavingsTypeDef


def get_value() -> IdleEstimatedMonthlySavingsTypeDef:
    return {
        "currency": ...,
    }


# IdleEstimatedMonthlySavingsTypeDef definition

class IdleEstimatedMonthlySavingsTypeDef(TypedDict):
    currency: NotRequired[CurrencyType],  # (1)
    value: NotRequired[float],
```

1. See [:material-code-brackets: CurrencyType](./literals.md#currencytype) 
## IdleUtilizationMetricTypeDef

```python
# IdleUtilizationMetricTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import IdleUtilizationMetricTypeDef


def get_value() -> IdleUtilizationMetricTypeDef:
    return {
        "name": ...,
    }


# IdleUtilizationMetricTypeDef definition

class IdleUtilizationMetricTypeDef(TypedDict):
    name: NotRequired[IdleMetricNameType],  # (1)
    statistic: NotRequired[MetricStatisticType],  # (2)
    value: NotRequired[float],
```

1. See [:material-code-brackets: IdleMetricNameType](./literals.md#idlemetricnametype) 
2. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
## IdleSummaryTypeDef

```python
# IdleSummaryTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import IdleSummaryTypeDef


def get_value() -> IdleSummaryTypeDef:
    return {
        "name": ...,
    }


# IdleSummaryTypeDef definition

class IdleSummaryTypeDef(TypedDict):
    name: NotRequired[IdleFindingType],  # (1)
    value: NotRequired[float],
```

1. See [:material-code-brackets: IdleFindingType](./literals.md#idlefindingtype) 
## InstanceEstimatedMonthlySavingsTypeDef

```python
# InstanceEstimatedMonthlySavingsTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import InstanceEstimatedMonthlySavingsTypeDef


def get_value() -> InstanceEstimatedMonthlySavingsTypeDef:
    return {
        "currency": ...,
    }


# InstanceEstimatedMonthlySavingsTypeDef definition

class InstanceEstimatedMonthlySavingsTypeDef(TypedDict):
    currency: NotRequired[CurrencyType],  # (1)
    value: NotRequired[float],
```

1. See [:material-code-brackets: CurrencyType](./literals.md#currencytype) 
## RecommendationSourceTypeDef

```python
# RecommendationSourceTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import RecommendationSourceTypeDef


def get_value() -> RecommendationSourceTypeDef:
    return {
        "recommendationSourceArn": ...,
    }


# RecommendationSourceTypeDef definition

class RecommendationSourceTypeDef(TypedDict):
    recommendationSourceArn: NotRequired[str],
    recommendationSourceType: NotRequired[RecommendationSourceTypeType],  # (1)
```

1. See [:material-code-brackets: RecommendationSourceTypeType](./literals.md#recommendationsourcetypetype) 
## LambdaSavingsEstimationModeTypeDef

```python
# LambdaSavingsEstimationModeTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import LambdaSavingsEstimationModeTypeDef


def get_value() -> LambdaSavingsEstimationModeTypeDef:
    return {
        "source": ...,
    }


# LambdaSavingsEstimationModeTypeDef definition

class LambdaSavingsEstimationModeTypeDef(TypedDict):
    source: NotRequired[LambdaSavingsEstimationModeSourceType],  # (1)
```

1. See [:material-code-brackets: LambdaSavingsEstimationModeSourceType](./literals.md#lambdasavingsestimationmodesourcetype) 
## LambdaEstimatedMonthlySavingsTypeDef

```python
# LambdaEstimatedMonthlySavingsTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import LambdaEstimatedMonthlySavingsTypeDef


def get_value() -> LambdaEstimatedMonthlySavingsTypeDef:
    return {
        "currency": ...,
    }


# LambdaEstimatedMonthlySavingsTypeDef definition

class LambdaEstimatedMonthlySavingsTypeDef(TypedDict):
    currency: NotRequired[CurrencyType],  # (1)
    value: NotRequired[float],
```

1. See [:material-code-brackets: CurrencyType](./literals.md#currencytype) 
## LambdaFunctionMemoryProjectedMetricTypeDef

```python
# LambdaFunctionMemoryProjectedMetricTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import LambdaFunctionMemoryProjectedMetricTypeDef


def get_value() -> LambdaFunctionMemoryProjectedMetricTypeDef:
    return {
        "name": ...,
    }


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
# LambdaFunctionUtilizationMetricTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import LambdaFunctionUtilizationMetricTypeDef


def get_value() -> LambdaFunctionUtilizationMetricTypeDef:
    return {
        "name": ...,
    }


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
# MetricSourceTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import MetricSourceTypeDef


def get_value() -> MetricSourceTypeDef:
    return {
        "provider": ...,
    }


# MetricSourceTypeDef definition

class MetricSourceTypeDef(TypedDict):
    provider: NotRequired[MetricSourceProviderType],  # (1)
    providerArn: NotRequired[str],
```

1. See [:material-code-brackets: MetricSourceProviderType](./literals.md#metricsourceprovidertype) 
## PreferredResourceTypeDef

```python
# PreferredResourceTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import PreferredResourceTypeDef


def get_value() -> PreferredResourceTypeDef:
    return {
        "name": ...,
    }


# PreferredResourceTypeDef definition

class PreferredResourceTypeDef(TypedDict):
    name: NotRequired[PreferredResourceNameType],  # (1)
    includeList: NotRequired[Sequence[str]],
    excludeList: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: PreferredResourceNameType](./literals.md#preferredresourcenametype) 
## ProjectedMetricTypeDef

```python
# ProjectedMetricTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ProjectedMetricTypeDef


def get_value() -> ProjectedMetricTypeDef:
    return {
        "name": ...,
    }


# ProjectedMetricTypeDef definition

class ProjectedMetricTypeDef(TypedDict):
    name: NotRequired[MetricNameType],  # (1)
    timestamps: NotRequired[List[datetime]],
    values: NotRequired[List[float]],
```

1. See [:material-code-brackets: MetricNameType](./literals.md#metricnametype) 
## RDSDBUtilizationMetricTypeDef

```python
# RDSDBUtilizationMetricTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import RDSDBUtilizationMetricTypeDef


def get_value() -> RDSDBUtilizationMetricTypeDef:
    return {
        "name": ...,
    }


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
# RDSDatabaseProjectedMetricTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import RDSDatabaseProjectedMetricTypeDef


def get_value() -> RDSDatabaseProjectedMetricTypeDef:
    return {
        "name": ...,
    }


# RDSDatabaseProjectedMetricTypeDef definition

class RDSDatabaseProjectedMetricTypeDef(TypedDict):
    name: NotRequired[RDSDBMetricNameType],  # (1)
    timestamps: NotRequired[List[datetime]],
    values: NotRequired[List[float]],
```

1. See [:material-code-brackets: RDSDBMetricNameType](./literals.md#rdsdbmetricnametype) 
## RDSSavingsEstimationModeTypeDef

```python
# RDSSavingsEstimationModeTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import RDSSavingsEstimationModeTypeDef


def get_value() -> RDSSavingsEstimationModeTypeDef:
    return {
        "source": ...,
    }


# RDSSavingsEstimationModeTypeDef definition

class RDSSavingsEstimationModeTypeDef(TypedDict):
    source: NotRequired[RDSSavingsEstimationModeSourceType],  # (1)
```

1. See [:material-code-brackets: RDSSavingsEstimationModeSourceType](./literals.md#rdssavingsestimationmodesourcetype) 
## RDSInstanceEstimatedMonthlySavingsTypeDef

```python
# RDSInstanceEstimatedMonthlySavingsTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import RDSInstanceEstimatedMonthlySavingsTypeDef


def get_value() -> RDSInstanceEstimatedMonthlySavingsTypeDef:
    return {
        "currency": ...,
    }


# RDSInstanceEstimatedMonthlySavingsTypeDef definition

class RDSInstanceEstimatedMonthlySavingsTypeDef(TypedDict):
    currency: NotRequired[CurrencyType],  # (1)
    value: NotRequired[float],
```

1. See [:material-code-brackets: CurrencyType](./literals.md#currencytype) 
## RDSStorageEstimatedMonthlySavingsTypeDef

```python
# RDSStorageEstimatedMonthlySavingsTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import RDSStorageEstimatedMonthlySavingsTypeDef


def get_value() -> RDSStorageEstimatedMonthlySavingsTypeDef:
    return {
        "currency": ...,
    }


# RDSStorageEstimatedMonthlySavingsTypeDef definition

class RDSStorageEstimatedMonthlySavingsTypeDef(TypedDict):
    currency: NotRequired[CurrencyType],  # (1)
    value: NotRequired[float],
```

1. See [:material-code-brackets: CurrencyType](./literals.md#currencytype) 
## ReasonCodeSummaryTypeDef

```python
# ReasonCodeSummaryTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ReasonCodeSummaryTypeDef


def get_value() -> ReasonCodeSummaryTypeDef:
    return {
        "name": ...,
    }


# ReasonCodeSummaryTypeDef definition

class ReasonCodeSummaryTypeDef(TypedDict):
    name: NotRequired[FindingReasonCodeType],  # (1)
    value: NotRequired[float],
```

1. See [:material-code-brackets: FindingReasonCodeType](./literals.md#findingreasoncodetype) 
## UpdateEnrollmentStatusRequestTypeDef

```python
# UpdateEnrollmentStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import UpdateEnrollmentStatusRequestTypeDef


def get_value() -> UpdateEnrollmentStatusRequestTypeDef:
    return {
        "status": ...,
    }


# UpdateEnrollmentStatusRequestTypeDef definition

class UpdateEnrollmentStatusRequestTypeDef(TypedDict):
    status: StatusType,  # (1)
    includeMemberAccounts: NotRequired[bool],
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## VolumeConfigurationTypeDef

```python
# VolumeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import VolumeConfigurationTypeDef


def get_value() -> VolumeConfigurationTypeDef:
    return {
        "volumeType": ...,
    }


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
# AutoScalingGroupSavingsOpportunityAfterDiscountsTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import AutoScalingGroupSavingsOpportunityAfterDiscountsTypeDef


def get_value() -> AutoScalingGroupSavingsOpportunityAfterDiscountsTypeDef:
    return {
        "savingsOpportunityPercentage": ...,
    }


# AutoScalingGroupSavingsOpportunityAfterDiscountsTypeDef definition

class AutoScalingGroupSavingsOpportunityAfterDiscountsTypeDef(TypedDict):
    savingsOpportunityPercentage: NotRequired[float],
    estimatedMonthlySavings: NotRequired[AutoScalingGroupEstimatedMonthlySavingsTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingGroupEstimatedMonthlySavingsTypeDef](./type_defs.md#autoscalinggroupestimatedmonthlysavingstypedef) 
## ContainerConfigurationTypeDef

```python
# ContainerConfigurationTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ContainerConfigurationTypeDef


def get_value() -> ContainerConfigurationTypeDef:
    return {
        "containerName": ...,
    }


# ContainerConfigurationTypeDef definition

class ContainerConfigurationTypeDef(TypedDict):
    containerName: NotRequired[str],
    memorySizeConfiguration: NotRequired[MemorySizeConfigurationTypeDef],  # (1)
    cpu: NotRequired[int],
```

1. See [:material-code-braces: MemorySizeConfigurationTypeDef](./type_defs.md#memorysizeconfigurationtypedef) 
## ContainerRecommendationTypeDef

```python
# ContainerRecommendationTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ContainerRecommendationTypeDef


def get_value() -> ContainerRecommendationTypeDef:
    return {
        "containerName": ...,
    }


# ContainerRecommendationTypeDef definition

class ContainerRecommendationTypeDef(TypedDict):
    containerName: NotRequired[str],
    memorySizeConfiguration: NotRequired[MemorySizeConfigurationTypeDef],  # (1)
    cpu: NotRequired[int],
```

1. See [:material-code-braces: MemorySizeConfigurationTypeDef](./type_defs.md#memorysizeconfigurationtypedef) 
## UtilizationPreferenceTypeDef

```python
# UtilizationPreferenceTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import UtilizationPreferenceTypeDef


def get_value() -> UtilizationPreferenceTypeDef:
    return {
        "metricName": ...,
    }


# UtilizationPreferenceTypeDef definition

class UtilizationPreferenceTypeDef(TypedDict):
    metricName: NotRequired[CustomizableMetricNameType],  # (1)
    metricParameters: NotRequired[CustomizableMetricParametersTypeDef],  # (2)
```

1. See [:material-code-brackets: CustomizableMetricNameType](./literals.md#customizablemetricnametype) 
2. See [:material-code-braces: CustomizableMetricParametersTypeDef](./type_defs.md#customizablemetricparameterstypedef) 
## DeleteRecommendationPreferencesRequestTypeDef

```python
# DeleteRecommendationPreferencesRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import DeleteRecommendationPreferencesRequestTypeDef


def get_value() -> DeleteRecommendationPreferencesRequestTypeDef:
    return {
        "resourceType": ...,
    }


# DeleteRecommendationPreferencesRequestTypeDef definition

class DeleteRecommendationPreferencesRequestTypeDef(TypedDict):
    resourceType: ResourceTypeType,  # (1)
    recommendationPreferenceNames: Sequence[RecommendationPreferenceNameType],  # (2)
    scope: NotRequired[ScopeTypeDef],  # (3)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: RecommendationPreferenceNameType](./literals.md#recommendationpreferencenametype) 
3. See [:material-code-braces: ScopeTypeDef](./type_defs.md#scopetypedef) 
## GetRecommendationPreferencesRequestTypeDef

```python
# GetRecommendationPreferencesRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetRecommendationPreferencesRequestTypeDef


def get_value() -> GetRecommendationPreferencesRequestTypeDef:
    return {
        "resourceType": ...,
    }


# GetRecommendationPreferencesRequestTypeDef definition

class GetRecommendationPreferencesRequestTypeDef(TypedDict):
    resourceType: ResourceTypeType,  # (1)
    scope: NotRequired[ScopeTypeDef],  # (2)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ScopeTypeDef](./type_defs.md#scopetypedef) 
## DescribeRecommendationExportJobsRequestTypeDef

```python
# DescribeRecommendationExportJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import DescribeRecommendationExportJobsRequestTypeDef


def get_value() -> DescribeRecommendationExportJobsRequestTypeDef:
    return {
        "jobIds": ...,
    }


# DescribeRecommendationExportJobsRequestTypeDef definition

class DescribeRecommendationExportJobsRequestTypeDef(TypedDict):
    jobIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[JobFilterTypeDef]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: JobFilterTypeDef](./type_defs.md#jobfiltertypedef) 
## DescribeRecommendationExportJobsRequestPaginateTypeDef

```python
# DescribeRecommendationExportJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import DescribeRecommendationExportJobsRequestPaginateTypeDef


def get_value() -> DescribeRecommendationExportJobsRequestPaginateTypeDef:
    return {
        "jobIds": ...,
    }


# DescribeRecommendationExportJobsRequestPaginateTypeDef definition

class DescribeRecommendationExportJobsRequestPaginateTypeDef(TypedDict):
    jobIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[JobFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: JobFilterTypeDef](./type_defs.md#jobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetRecommendationPreferencesRequestPaginateTypeDef

```python
# GetRecommendationPreferencesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetRecommendationPreferencesRequestPaginateTypeDef


def get_value() -> GetRecommendationPreferencesRequestPaginateTypeDef:
    return {
        "resourceType": ...,
    }


# GetRecommendationPreferencesRequestPaginateTypeDef definition

class GetRecommendationPreferencesRequestPaginateTypeDef(TypedDict):
    resourceType: ResourceTypeType,  # (1)
    scope: NotRequired[ScopeTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ScopeTypeDef](./type_defs.md#scopetypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetRecommendationSummariesRequestPaginateTypeDef

```python
# GetRecommendationSummariesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetRecommendationSummariesRequestPaginateTypeDef


def get_value() -> GetRecommendationSummariesRequestPaginateTypeDef:
    return {
        "accountIds": ...,
    }


# GetRecommendationSummariesRequestPaginateTypeDef definition

class GetRecommendationSummariesRequestPaginateTypeDef(TypedDict):
    accountIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetEnrollmentStatusResponseTypeDef

```python
# GetEnrollmentStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetEnrollmentStatusResponseTypeDef


def get_value() -> GetEnrollmentStatusResponseTypeDef:
    return {
        "status": ...,
    }


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
# GetEnrollmentStatusesForOrganizationResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetEnrollmentStatusesForOrganizationResponseTypeDef


def get_value() -> GetEnrollmentStatusesForOrganizationResponseTypeDef:
    return {
        "accountEnrollmentStatuses": ...,
    }


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
# UpdateEnrollmentStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import UpdateEnrollmentStatusResponseTypeDef


def get_value() -> UpdateEnrollmentStatusResponseTypeDef:
    return {
        "status": ...,
    }


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
# EBSEffectiveRecommendationPreferencesTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import EBSEffectiveRecommendationPreferencesTypeDef


def get_value() -> EBSEffectiveRecommendationPreferencesTypeDef:
    return {
        "savingsEstimationMode": ...,
    }


# EBSEffectiveRecommendationPreferencesTypeDef definition

class EBSEffectiveRecommendationPreferencesTypeDef(TypedDict):
    savingsEstimationMode: NotRequired[EBSSavingsEstimationModeTypeDef],  # (1)
```

1. See [:material-code-braces: EBSSavingsEstimationModeTypeDef](./type_defs.md#ebssavingsestimationmodetypedef) 
## EBSSavingsOpportunityAfterDiscountsTypeDef

```python
# EBSSavingsOpportunityAfterDiscountsTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import EBSSavingsOpportunityAfterDiscountsTypeDef


def get_value() -> EBSSavingsOpportunityAfterDiscountsTypeDef:
    return {
        "savingsOpportunityPercentage": ...,
    }


# EBSSavingsOpportunityAfterDiscountsTypeDef definition

class EBSSavingsOpportunityAfterDiscountsTypeDef(TypedDict):
    savingsOpportunityPercentage: NotRequired[float],
    estimatedMonthlySavings: NotRequired[EBSEstimatedMonthlySavingsTypeDef],  # (1)
```

1. See [:material-code-braces: EBSEstimatedMonthlySavingsTypeDef](./type_defs.md#ebsestimatedmonthlysavingstypedef) 
## GetEBSVolumeRecommendationsRequestTypeDef

```python
# GetEBSVolumeRecommendationsRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetEBSVolumeRecommendationsRequestTypeDef


def get_value() -> GetEBSVolumeRecommendationsRequestTypeDef:
    return {
        "volumeArns": ...,
    }


# GetEBSVolumeRecommendationsRequestTypeDef definition

class GetEBSVolumeRecommendationsRequestTypeDef(TypedDict):
    volumeArns: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[EBSFilterTypeDef]],  # (1)
    accountIds: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: EBSFilterTypeDef](./type_defs.md#ebsfiltertypedef) 
## ECSEffectiveRecommendationPreferencesTypeDef

```python
# ECSEffectiveRecommendationPreferencesTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ECSEffectiveRecommendationPreferencesTypeDef


def get_value() -> ECSEffectiveRecommendationPreferencesTypeDef:
    return {
        "savingsEstimationMode": ...,
    }


# ECSEffectiveRecommendationPreferencesTypeDef definition

class ECSEffectiveRecommendationPreferencesTypeDef(TypedDict):
    savingsEstimationMode: NotRequired[ECSSavingsEstimationModeTypeDef],  # (1)
```

1. See [:material-code-braces: ECSSavingsEstimationModeTypeDef](./type_defs.md#ecssavingsestimationmodetypedef) 
## ECSSavingsOpportunityAfterDiscountsTypeDef

```python
# ECSSavingsOpportunityAfterDiscountsTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ECSSavingsOpportunityAfterDiscountsTypeDef


def get_value() -> ECSSavingsOpportunityAfterDiscountsTypeDef:
    return {
        "savingsOpportunityPercentage": ...,
    }


# ECSSavingsOpportunityAfterDiscountsTypeDef definition

class ECSSavingsOpportunityAfterDiscountsTypeDef(TypedDict):
    savingsOpportunityPercentage: NotRequired[float],
    estimatedMonthlySavings: NotRequired[ECSEstimatedMonthlySavingsTypeDef],  # (1)
```

1. See [:material-code-braces: ECSEstimatedMonthlySavingsTypeDef](./type_defs.md#ecsestimatedmonthlysavingstypedef) 
## ECSServiceRecommendedOptionProjectedMetricTypeDef

```python
# ECSServiceRecommendedOptionProjectedMetricTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ECSServiceRecommendedOptionProjectedMetricTypeDef


def get_value() -> ECSServiceRecommendedOptionProjectedMetricTypeDef:
    return {
        "recommendedCpuUnits": ...,
    }


# ECSServiceRecommendedOptionProjectedMetricTypeDef definition

class ECSServiceRecommendedOptionProjectedMetricTypeDef(TypedDict):
    recommendedCpuUnits: NotRequired[int],
    recommendedMemorySize: NotRequired[int],
    projectedMetrics: NotRequired[List[ECSServiceProjectedMetricTypeDef]],  # (1)
```

1. See [:material-code-braces: ECSServiceProjectedMetricTypeDef](./type_defs.md#ecsserviceprojectedmetrictypedef) 
## GetECSServiceRecommendationsRequestTypeDef

```python
# GetECSServiceRecommendationsRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetECSServiceRecommendationsRequestTypeDef


def get_value() -> GetECSServiceRecommendationsRequestTypeDef:
    return {
        "serviceArns": ...,
    }


# GetECSServiceRecommendationsRequestTypeDef definition

class GetECSServiceRecommendationsRequestTypeDef(TypedDict):
    serviceArns: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[ECSServiceRecommendationFilterTypeDef]],  # (1)
    accountIds: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: ECSServiceRecommendationFilterTypeDef](./type_defs.md#ecsservicerecommendationfiltertypedef) 
## GetEnrollmentStatusesForOrganizationRequestPaginateTypeDef

```python
# GetEnrollmentStatusesForOrganizationRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetEnrollmentStatusesForOrganizationRequestPaginateTypeDef


def get_value() -> GetEnrollmentStatusesForOrganizationRequestPaginateTypeDef:
    return {
        "filters": ...,
    }


# GetEnrollmentStatusesForOrganizationRequestPaginateTypeDef definition

class GetEnrollmentStatusesForOrganizationRequestPaginateTypeDef(TypedDict):
    filters: NotRequired[Sequence[EnrollmentFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: EnrollmentFilterTypeDef](./type_defs.md#enrollmentfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetEnrollmentStatusesForOrganizationRequestTypeDef

```python
# GetEnrollmentStatusesForOrganizationRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetEnrollmentStatusesForOrganizationRequestTypeDef


def get_value() -> GetEnrollmentStatusesForOrganizationRequestTypeDef:
    return {
        "filters": ...,
    }


# GetEnrollmentStatusesForOrganizationRequestTypeDef definition

class GetEnrollmentStatusesForOrganizationRequestTypeDef(TypedDict):
    filters: NotRequired[Sequence[EnrollmentFilterTypeDef]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: EnrollmentFilterTypeDef](./type_defs.md#enrollmentfiltertypedef) 
## InferredWorkloadSavingTypeDef

```python
# InferredWorkloadSavingTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import InferredWorkloadSavingTypeDef


def get_value() -> InferredWorkloadSavingTypeDef:
    return {
        "inferredWorkloadTypes": ...,
    }


# InferredWorkloadSavingTypeDef definition

class InferredWorkloadSavingTypeDef(TypedDict):
    inferredWorkloadTypes: NotRequired[List[InferredWorkloadTypeType]],  # (1)
    estimatedMonthlySavings: NotRequired[EstimatedMonthlySavingsTypeDef],  # (2)
```

1. See [:material-code-brackets: InferredWorkloadTypeType](./literals.md#inferredworkloadtypetype) 
2. See [:material-code-braces: EstimatedMonthlySavingsTypeDef](./type_defs.md#estimatedmonthlysavingstypedef) 
## SavingsOpportunityTypeDef

```python
# SavingsOpportunityTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import SavingsOpportunityTypeDef


def get_value() -> SavingsOpportunityTypeDef:
    return {
        "savingsOpportunityPercentage": ...,
    }


# SavingsOpportunityTypeDef definition

class SavingsOpportunityTypeDef(TypedDict):
    savingsOpportunityPercentage: NotRequired[float],
    estimatedMonthlySavings: NotRequired[EstimatedMonthlySavingsTypeDef],  # (1)
```

1. See [:material-code-braces: EstimatedMonthlySavingsTypeDef](./type_defs.md#estimatedmonthlysavingstypedef) 
## GetAutoScalingGroupRecommendationsRequestTypeDef

```python
# GetAutoScalingGroupRecommendationsRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetAutoScalingGroupRecommendationsRequestTypeDef


def get_value() -> GetAutoScalingGroupRecommendationsRequestTypeDef:
    return {
        "accountIds": ...,
    }


# GetAutoScalingGroupRecommendationsRequestTypeDef definition

class GetAutoScalingGroupRecommendationsRequestTypeDef(TypedDict):
    accountIds: NotRequired[Sequence[str]],
    autoScalingGroupArns: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    recommendationPreferences: NotRequired[RecommendationPreferencesTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef) 
## GetEC2InstanceRecommendationsRequestTypeDef

```python
# GetEC2InstanceRecommendationsRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetEC2InstanceRecommendationsRequestTypeDef


def get_value() -> GetEC2InstanceRecommendationsRequestTypeDef:
    return {
        "instanceArns": ...,
    }


# GetEC2InstanceRecommendationsRequestTypeDef definition

class GetEC2InstanceRecommendationsRequestTypeDef(TypedDict):
    instanceArns: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    accountIds: NotRequired[Sequence[str]],
    recommendationPreferences: NotRequired[RecommendationPreferencesTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef) 
## ExportAutoScalingGroupRecommendationsRequestTypeDef

```python
# ExportAutoScalingGroupRecommendationsRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ExportAutoScalingGroupRecommendationsRequestTypeDef


def get_value() -> ExportAutoScalingGroupRecommendationsRequestTypeDef:
    return {
        "s3DestinationConfig": ...,
    }


# ExportAutoScalingGroupRecommendationsRequestTypeDef definition

class ExportAutoScalingGroupRecommendationsRequestTypeDef(TypedDict):
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
## ExportEBSVolumeRecommendationsRequestTypeDef

```python
# ExportEBSVolumeRecommendationsRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ExportEBSVolumeRecommendationsRequestTypeDef


def get_value() -> ExportEBSVolumeRecommendationsRequestTypeDef:
    return {
        "s3DestinationConfig": ...,
    }


# ExportEBSVolumeRecommendationsRequestTypeDef definition

class ExportEBSVolumeRecommendationsRequestTypeDef(TypedDict):
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
## ExportEC2InstanceRecommendationsRequestTypeDef

```python
# ExportEC2InstanceRecommendationsRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ExportEC2InstanceRecommendationsRequestTypeDef


def get_value() -> ExportEC2InstanceRecommendationsRequestTypeDef:
    return {
        "s3DestinationConfig": ...,
    }


# ExportEC2InstanceRecommendationsRequestTypeDef definition

class ExportEC2InstanceRecommendationsRequestTypeDef(TypedDict):
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
## ExportECSServiceRecommendationsRequestTypeDef

```python
# ExportECSServiceRecommendationsRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ExportECSServiceRecommendationsRequestTypeDef


def get_value() -> ExportECSServiceRecommendationsRequestTypeDef:
    return {
        "s3DestinationConfig": ...,
    }


# ExportECSServiceRecommendationsRequestTypeDef definition

class ExportECSServiceRecommendationsRequestTypeDef(TypedDict):
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
# ExportAutoScalingGroupRecommendationsResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ExportAutoScalingGroupRecommendationsResponseTypeDef


def get_value() -> ExportAutoScalingGroupRecommendationsResponseTypeDef:
    return {
        "jobId": ...,
    }


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
# ExportDestinationTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ExportDestinationTypeDef


def get_value() -> ExportDestinationTypeDef:
    return {
        "s3": ...,
    }


# ExportDestinationTypeDef definition

class ExportDestinationTypeDef(TypedDict):
    s3: NotRequired[S3DestinationTypeDef],  # (1)
```

1. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
## ExportEBSVolumeRecommendationsResponseTypeDef

```python
# ExportEBSVolumeRecommendationsResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ExportEBSVolumeRecommendationsResponseTypeDef


def get_value() -> ExportEBSVolumeRecommendationsResponseTypeDef:
    return {
        "jobId": ...,
    }


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
# ExportEC2InstanceRecommendationsResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ExportEC2InstanceRecommendationsResponseTypeDef


def get_value() -> ExportEC2InstanceRecommendationsResponseTypeDef:
    return {
        "jobId": ...,
    }


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
# ExportECSServiceRecommendationsResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ExportECSServiceRecommendationsResponseTypeDef


def get_value() -> ExportECSServiceRecommendationsResponseTypeDef:
    return {
        "jobId": ...,
    }


# ExportECSServiceRecommendationsResponseTypeDef definition

class ExportECSServiceRecommendationsResponseTypeDef(TypedDict):
    jobId: str,
    s3Destination: S3DestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportIdleRecommendationsResponseTypeDef

```python
# ExportIdleRecommendationsResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ExportIdleRecommendationsResponseTypeDef


def get_value() -> ExportIdleRecommendationsResponseTypeDef:
    return {
        "jobId": ...,
    }


# ExportIdleRecommendationsResponseTypeDef definition

class ExportIdleRecommendationsResponseTypeDef(TypedDict):
    jobId: str,
    s3Destination: S3DestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportLambdaFunctionRecommendationsResponseTypeDef

```python
# ExportLambdaFunctionRecommendationsResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ExportLambdaFunctionRecommendationsResponseTypeDef


def get_value() -> ExportLambdaFunctionRecommendationsResponseTypeDef:
    return {
        "jobId": ...,
    }


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
# ExportLicenseRecommendationsResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ExportLicenseRecommendationsResponseTypeDef


def get_value() -> ExportLicenseRecommendationsResponseTypeDef:
    return {
        "jobId": ...,
    }


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
# ExportRDSDatabaseRecommendationsResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ExportRDSDatabaseRecommendationsResponseTypeDef


def get_value() -> ExportRDSDatabaseRecommendationsResponseTypeDef:
    return {
        "jobId": ...,
    }


# ExportRDSDatabaseRecommendationsResponseTypeDef definition

class ExportRDSDatabaseRecommendationsResponseTypeDef(TypedDict):
    jobId: str,
    s3Destination: S3DestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportIdleRecommendationsRequestTypeDef

```python
# ExportIdleRecommendationsRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ExportIdleRecommendationsRequestTypeDef


def get_value() -> ExportIdleRecommendationsRequestTypeDef:
    return {
        "s3DestinationConfig": ...,
    }


# ExportIdleRecommendationsRequestTypeDef definition

class ExportIdleRecommendationsRequestTypeDef(TypedDict):
    s3DestinationConfig: S3DestinationConfigTypeDef,  # (1)
    accountIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[IdleRecommendationFilterTypeDef]],  # (2)
    fieldsToExport: NotRequired[Sequence[ExportableIdleFieldType]],  # (3)
    fileFormat: NotRequired[FileFormatType],  # (4)
    includeMemberAccounts: NotRequired[bool],
```

1. See [:material-code-braces: S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef) 
2. See [:material-code-braces: IdleRecommendationFilterTypeDef](./type_defs.md#idlerecommendationfiltertypedef) 
3. See [:material-code-brackets: ExportableIdleFieldType](./literals.md#exportableidlefieldtype) 
4. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
## ExportLambdaFunctionRecommendationsRequestTypeDef

```python
# ExportLambdaFunctionRecommendationsRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ExportLambdaFunctionRecommendationsRequestTypeDef


def get_value() -> ExportLambdaFunctionRecommendationsRequestTypeDef:
    return {
        "s3DestinationConfig": ...,
    }


# ExportLambdaFunctionRecommendationsRequestTypeDef definition

class ExportLambdaFunctionRecommendationsRequestTypeDef(TypedDict):
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
## GetLambdaFunctionRecommendationsRequestPaginateTypeDef

```python
# GetLambdaFunctionRecommendationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetLambdaFunctionRecommendationsRequestPaginateTypeDef


def get_value() -> GetLambdaFunctionRecommendationsRequestPaginateTypeDef:
    return {
        "functionArns": ...,
    }


# GetLambdaFunctionRecommendationsRequestPaginateTypeDef definition

class GetLambdaFunctionRecommendationsRequestPaginateTypeDef(TypedDict):
    functionArns: NotRequired[Sequence[str]],
    accountIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[LambdaFunctionRecommendationFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: LambdaFunctionRecommendationFilterTypeDef](./type_defs.md#lambdafunctionrecommendationfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetLambdaFunctionRecommendationsRequestTypeDef

```python
# GetLambdaFunctionRecommendationsRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetLambdaFunctionRecommendationsRequestTypeDef


def get_value() -> GetLambdaFunctionRecommendationsRequestTypeDef:
    return {
        "functionArns": ...,
    }


# GetLambdaFunctionRecommendationsRequestTypeDef definition

class GetLambdaFunctionRecommendationsRequestTypeDef(TypedDict):
    functionArns: NotRequired[Sequence[str]],
    accountIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[LambdaFunctionRecommendationFilterTypeDef]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: LambdaFunctionRecommendationFilterTypeDef](./type_defs.md#lambdafunctionrecommendationfiltertypedef) 
## ExportLicenseRecommendationsRequestTypeDef

```python
# ExportLicenseRecommendationsRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ExportLicenseRecommendationsRequestTypeDef


def get_value() -> ExportLicenseRecommendationsRequestTypeDef:
    return {
        "s3DestinationConfig": ...,
    }


# ExportLicenseRecommendationsRequestTypeDef definition

class ExportLicenseRecommendationsRequestTypeDef(TypedDict):
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
## GetLicenseRecommendationsRequestTypeDef

```python
# GetLicenseRecommendationsRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetLicenseRecommendationsRequestTypeDef


def get_value() -> GetLicenseRecommendationsRequestTypeDef:
    return {
        "resourceArns": ...,
    }


# GetLicenseRecommendationsRequestTypeDef definition

class GetLicenseRecommendationsRequestTypeDef(TypedDict):
    resourceArns: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[LicenseRecommendationFilterTypeDef]],  # (1)
    accountIds: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: LicenseRecommendationFilterTypeDef](./type_defs.md#licenserecommendationfiltertypedef) 
## ExportRDSDatabaseRecommendationsRequestTypeDef

```python
# ExportRDSDatabaseRecommendationsRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ExportRDSDatabaseRecommendationsRequestTypeDef


def get_value() -> ExportRDSDatabaseRecommendationsRequestTypeDef:
    return {
        "s3DestinationConfig": ...,
    }


# ExportRDSDatabaseRecommendationsRequestTypeDef definition

class ExportRDSDatabaseRecommendationsRequestTypeDef(TypedDict):
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
## GetRDSDatabaseRecommendationsRequestTypeDef

```python
# GetRDSDatabaseRecommendationsRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetRDSDatabaseRecommendationsRequestTypeDef


def get_value() -> GetRDSDatabaseRecommendationsRequestTypeDef:
    return {
        "resourceArns": ...,
    }


# GetRDSDatabaseRecommendationsRequestTypeDef definition

class GetRDSDatabaseRecommendationsRequestTypeDef(TypedDict):
    resourceArns: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[RDSDBRecommendationFilterTypeDef]],  # (1)
    accountIds: NotRequired[Sequence[str]],
    recommendationPreferences: NotRequired[RecommendationPreferencesTypeDef],  # (2)
```

1. See [:material-code-braces: RDSDBRecommendationFilterTypeDef](./type_defs.md#rdsdbrecommendationfiltertypedef) 
2. See [:material-code-braces: RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef) 
## GetEC2RecommendationProjectedMetricsRequestTypeDef

```python
# GetEC2RecommendationProjectedMetricsRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetEC2RecommendationProjectedMetricsRequestTypeDef


def get_value() -> GetEC2RecommendationProjectedMetricsRequestTypeDef:
    return {
        "instanceArn": ...,
    }


# GetEC2RecommendationProjectedMetricsRequestTypeDef definition

class GetEC2RecommendationProjectedMetricsRequestTypeDef(TypedDict):
    instanceArn: str,
    stat: MetricStatisticType,  # (1)
    period: int,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    recommendationPreferences: NotRequired[RecommendationPreferencesTypeDef],  # (2)
```

1. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
2. See [:material-code-braces: RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef) 
## GetECSServiceRecommendationProjectedMetricsRequestTypeDef

```python
# GetECSServiceRecommendationProjectedMetricsRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetECSServiceRecommendationProjectedMetricsRequestTypeDef


def get_value() -> GetECSServiceRecommendationProjectedMetricsRequestTypeDef:
    return {
        "serviceArn": ...,
    }


# GetECSServiceRecommendationProjectedMetricsRequestTypeDef definition

class GetECSServiceRecommendationProjectedMetricsRequestTypeDef(TypedDict):
    serviceArn: str,
    stat: MetricStatisticType,  # (1)
    period: int,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
```

1. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
## GetRDSDatabaseRecommendationProjectedMetricsRequestTypeDef

```python
# GetRDSDatabaseRecommendationProjectedMetricsRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetRDSDatabaseRecommendationProjectedMetricsRequestTypeDef


def get_value() -> GetRDSDatabaseRecommendationProjectedMetricsRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# GetRDSDatabaseRecommendationProjectedMetricsRequestTypeDef definition

class GetRDSDatabaseRecommendationProjectedMetricsRequestTypeDef(TypedDict):
    resourceArn: str,
    stat: MetricStatisticType,  # (1)
    period: int,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    recommendationPreferences: NotRequired[RecommendationPreferencesTypeDef],  # (2)
```

1. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
2. See [:material-code-braces: RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef) 
## GetIdleRecommendationsRequestTypeDef

```python
# GetIdleRecommendationsRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetIdleRecommendationsRequestTypeDef


def get_value() -> GetIdleRecommendationsRequestTypeDef:
    return {
        "resourceArns": ...,
    }


# GetIdleRecommendationsRequestTypeDef definition

class GetIdleRecommendationsRequestTypeDef(TypedDict):
    resourceArns: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[IdleRecommendationFilterTypeDef]],  # (1)
    accountIds: NotRequired[Sequence[str]],
    orderBy: NotRequired[OrderByTypeDef],  # (2)
```

1. See [:material-code-braces: IdleRecommendationFilterTypeDef](./type_defs.md#idlerecommendationfiltertypedef) 
2. See [:material-code-braces: OrderByTypeDef](./type_defs.md#orderbytypedef) 
## GpuInfoTypeDef

```python
# GpuInfoTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GpuInfoTypeDef


def get_value() -> GpuInfoTypeDef:
    return {
        "gpus": ...,
    }


# GpuInfoTypeDef definition

class GpuInfoTypeDef(TypedDict):
    gpus: NotRequired[List[GpuTypeDef]],  # (1)
```

1. See [:material-code-braces: GpuTypeDef](./type_defs.md#gputypedef) 
## IdleSavingsOpportunityAfterDiscountsTypeDef

```python
# IdleSavingsOpportunityAfterDiscountsTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import IdleSavingsOpportunityAfterDiscountsTypeDef


def get_value() -> IdleSavingsOpportunityAfterDiscountsTypeDef:
    return {
        "savingsOpportunityPercentage": ...,
    }


# IdleSavingsOpportunityAfterDiscountsTypeDef definition

class IdleSavingsOpportunityAfterDiscountsTypeDef(TypedDict):
    savingsOpportunityPercentage: NotRequired[float],
    estimatedMonthlySavings: NotRequired[IdleEstimatedMonthlySavingsTypeDef],  # (1)
```

1. See [:material-code-braces: IdleEstimatedMonthlySavingsTypeDef](./type_defs.md#idleestimatedmonthlysavingstypedef) 
## IdleSavingsOpportunityTypeDef

```python
# IdleSavingsOpportunityTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import IdleSavingsOpportunityTypeDef


def get_value() -> IdleSavingsOpportunityTypeDef:
    return {
        "savingsOpportunityPercentage": ...,
    }


# IdleSavingsOpportunityTypeDef definition

class IdleSavingsOpportunityTypeDef(TypedDict):
    savingsOpportunityPercentage: NotRequired[float],
    estimatedMonthlySavings: NotRequired[IdleEstimatedMonthlySavingsTypeDef],  # (1)
```

1. See [:material-code-braces: IdleEstimatedMonthlySavingsTypeDef](./type_defs.md#idleestimatedmonthlysavingstypedef) 
## InstanceSavingsOpportunityAfterDiscountsTypeDef

```python
# InstanceSavingsOpportunityAfterDiscountsTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import InstanceSavingsOpportunityAfterDiscountsTypeDef


def get_value() -> InstanceSavingsOpportunityAfterDiscountsTypeDef:
    return {
        "savingsOpportunityPercentage": ...,
    }


# InstanceSavingsOpportunityAfterDiscountsTypeDef definition

class InstanceSavingsOpportunityAfterDiscountsTypeDef(TypedDict):
    savingsOpportunityPercentage: NotRequired[float],
    estimatedMonthlySavings: NotRequired[InstanceEstimatedMonthlySavingsTypeDef],  # (1)
```

1. See [:material-code-braces: InstanceEstimatedMonthlySavingsTypeDef](./type_defs.md#instanceestimatedmonthlysavingstypedef) 
## LambdaEffectiveRecommendationPreferencesTypeDef

```python
# LambdaEffectiveRecommendationPreferencesTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import LambdaEffectiveRecommendationPreferencesTypeDef


def get_value() -> LambdaEffectiveRecommendationPreferencesTypeDef:
    return {
        "savingsEstimationMode": ...,
    }


# LambdaEffectiveRecommendationPreferencesTypeDef definition

class LambdaEffectiveRecommendationPreferencesTypeDef(TypedDict):
    savingsEstimationMode: NotRequired[LambdaSavingsEstimationModeTypeDef],  # (1)
```

1. See [:material-code-braces: LambdaSavingsEstimationModeTypeDef](./type_defs.md#lambdasavingsestimationmodetypedef) 
## LambdaSavingsOpportunityAfterDiscountsTypeDef

```python
# LambdaSavingsOpportunityAfterDiscountsTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import LambdaSavingsOpportunityAfterDiscountsTypeDef


def get_value() -> LambdaSavingsOpportunityAfterDiscountsTypeDef:
    return {
        "savingsOpportunityPercentage": ...,
    }


# LambdaSavingsOpportunityAfterDiscountsTypeDef definition

class LambdaSavingsOpportunityAfterDiscountsTypeDef(TypedDict):
    savingsOpportunityPercentage: NotRequired[float],
    estimatedMonthlySavings: NotRequired[LambdaEstimatedMonthlySavingsTypeDef],  # (1)
```

1. See [:material-code-braces: LambdaEstimatedMonthlySavingsTypeDef](./type_defs.md#lambdaestimatedmonthlysavingstypedef) 
## LicenseConfigurationTypeDef

```python
# LicenseConfigurationTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import LicenseConfigurationTypeDef


def get_value() -> LicenseConfigurationTypeDef:
    return {
        "numberOfCores": ...,
    }


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
# RecommendedOptionProjectedMetricTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import RecommendedOptionProjectedMetricTypeDef


def get_value() -> RecommendedOptionProjectedMetricTypeDef:
    return {
        "recommendedInstanceType": ...,
    }


# RecommendedOptionProjectedMetricTypeDef definition

class RecommendedOptionProjectedMetricTypeDef(TypedDict):
    recommendedInstanceType: NotRequired[str],
    rank: NotRequired[int],
    projectedMetrics: NotRequired[List[ProjectedMetricTypeDef]],  # (1)
```

1. See [:material-code-braces: ProjectedMetricTypeDef](./type_defs.md#projectedmetrictypedef) 
## RDSDatabaseRecommendedOptionProjectedMetricTypeDef

```python
# RDSDatabaseRecommendedOptionProjectedMetricTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import RDSDatabaseRecommendedOptionProjectedMetricTypeDef


def get_value() -> RDSDatabaseRecommendedOptionProjectedMetricTypeDef:
    return {
        "recommendedDBInstanceClass": ...,
    }


# RDSDatabaseRecommendedOptionProjectedMetricTypeDef definition

class RDSDatabaseRecommendedOptionProjectedMetricTypeDef(TypedDict):
    recommendedDBInstanceClass: NotRequired[str],
    rank: NotRequired[int],
    projectedMetrics: NotRequired[List[RDSDatabaseProjectedMetricTypeDef]],  # (1)
```

1. See [:material-code-braces: RDSDatabaseProjectedMetricTypeDef](./type_defs.md#rdsdatabaseprojectedmetrictypedef) 
## RDSEffectiveRecommendationPreferencesTypeDef

```python
# RDSEffectiveRecommendationPreferencesTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import RDSEffectiveRecommendationPreferencesTypeDef


def get_value() -> RDSEffectiveRecommendationPreferencesTypeDef:
    return {
        "cpuVendorArchitectures": ...,
    }


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
# RDSInstanceSavingsOpportunityAfterDiscountsTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import RDSInstanceSavingsOpportunityAfterDiscountsTypeDef


def get_value() -> RDSInstanceSavingsOpportunityAfterDiscountsTypeDef:
    return {
        "savingsOpportunityPercentage": ...,
    }


# RDSInstanceSavingsOpportunityAfterDiscountsTypeDef definition

class RDSInstanceSavingsOpportunityAfterDiscountsTypeDef(TypedDict):
    savingsOpportunityPercentage: NotRequired[float],
    estimatedMonthlySavings: NotRequired[RDSInstanceEstimatedMonthlySavingsTypeDef],  # (1)
```

1. See [:material-code-braces: RDSInstanceEstimatedMonthlySavingsTypeDef](./type_defs.md#rdsinstanceestimatedmonthlysavingstypedef) 
## RDSStorageSavingsOpportunityAfterDiscountsTypeDef

```python
# RDSStorageSavingsOpportunityAfterDiscountsTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import RDSStorageSavingsOpportunityAfterDiscountsTypeDef


def get_value() -> RDSStorageSavingsOpportunityAfterDiscountsTypeDef:
    return {
        "savingsOpportunityPercentage": ...,
    }


# RDSStorageSavingsOpportunityAfterDiscountsTypeDef definition

class RDSStorageSavingsOpportunityAfterDiscountsTypeDef(TypedDict):
    savingsOpportunityPercentage: NotRequired[float],
    estimatedMonthlySavings: NotRequired[RDSStorageEstimatedMonthlySavingsTypeDef],  # (1)
```

1. See [:material-code-braces: RDSStorageEstimatedMonthlySavingsTypeDef](./type_defs.md#rdsstorageestimatedmonthlysavingstypedef) 
## SummaryTypeDef

```python
# SummaryTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import SummaryTypeDef


def get_value() -> SummaryTypeDef:
    return {
        "name": ...,
    }


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
# ServiceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ServiceConfigurationTypeDef


def get_value() -> ServiceConfigurationTypeDef:
    return {
        "memory": ...,
    }


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
# EffectiveRecommendationPreferencesTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import EffectiveRecommendationPreferencesTypeDef


def get_value() -> EffectiveRecommendationPreferencesTypeDef:
    return {
        "cpuVendorArchitectures": ...,
    }


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
# GetEffectiveRecommendationPreferencesResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetEffectiveRecommendationPreferencesResponseTypeDef


def get_value() -> GetEffectiveRecommendationPreferencesResponseTypeDef:
    return {
        "enhancedInfrastructureMetrics": ...,
    }


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
## PutRecommendationPreferencesRequestTypeDef

```python
# PutRecommendationPreferencesRequestTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import PutRecommendationPreferencesRequestTypeDef


def get_value() -> PutRecommendationPreferencesRequestTypeDef:
    return {
        "resourceType": ...,
    }


# PutRecommendationPreferencesRequestTypeDef definition

class PutRecommendationPreferencesRequestTypeDef(TypedDict):
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
# RecommendationPreferencesDetailTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import RecommendationPreferencesDetailTypeDef


def get_value() -> RecommendationPreferencesDetailTypeDef:
    return {
        "scope": ...,
    }


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
# GetECSServiceRecommendationProjectedMetricsResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetECSServiceRecommendationProjectedMetricsResponseTypeDef


def get_value() -> GetECSServiceRecommendationProjectedMetricsResponseTypeDef:
    return {
        "recommendedOptionProjectedMetrics": ...,
    }


# GetECSServiceRecommendationProjectedMetricsResponseTypeDef definition

class GetECSServiceRecommendationProjectedMetricsResponseTypeDef(TypedDict):
    recommendedOptionProjectedMetrics: List[ECSServiceRecommendedOptionProjectedMetricTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ECSServiceRecommendedOptionProjectedMetricTypeDef](./type_defs.md#ecsservicerecommendedoptionprojectedmetrictypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ECSServiceRecommendationOptionTypeDef

```python
# ECSServiceRecommendationOptionTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ECSServiceRecommendationOptionTypeDef


def get_value() -> ECSServiceRecommendationOptionTypeDef:
    return {
        "memory": ...,
    }


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
# LicenseRecommendationOptionTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import LicenseRecommendationOptionTypeDef


def get_value() -> LicenseRecommendationOptionTypeDef:
    return {
        "rank": ...,
    }


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
# VolumeRecommendationOptionTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import VolumeRecommendationOptionTypeDef


def get_value() -> VolumeRecommendationOptionTypeDef:
    return {
        "configuration": ...,
    }


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
# RecommendationExportJobTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import RecommendationExportJobTypeDef


def get_value() -> RecommendationExportJobTypeDef:
    return {
        "jobId": ...,
    }


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
# AutoScalingGroupRecommendationOptionTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import AutoScalingGroupRecommendationOptionTypeDef


def get_value() -> AutoScalingGroupRecommendationOptionTypeDef:
    return {
        "configuration": ...,
    }


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
## IdleRecommendationTypeDef

```python
# IdleRecommendationTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import IdleRecommendationTypeDef


def get_value() -> IdleRecommendationTypeDef:
    return {
        "resourceArn": ...,
    }


# IdleRecommendationTypeDef definition

class IdleRecommendationTypeDef(TypedDict):
    resourceArn: NotRequired[str],
    resourceId: NotRequired[str],
    resourceType: NotRequired[IdleRecommendationResourceTypeType],  # (1)
    accountId: NotRequired[str],
    finding: NotRequired[IdleFindingType],  # (2)
    findingDescription: NotRequired[str],
    savingsOpportunity: NotRequired[IdleSavingsOpportunityTypeDef],  # (3)
    savingsOpportunityAfterDiscounts: NotRequired[IdleSavingsOpportunityAfterDiscountsTypeDef],  # (4)
    utilizationMetrics: NotRequired[List[IdleUtilizationMetricTypeDef]],  # (5)
    lookBackPeriodInDays: NotRequired[float],
    lastRefreshTimestamp: NotRequired[datetime],
    tags: NotRequired[List[TagTypeDef]],  # (6)
```

1. See [:material-code-brackets: IdleRecommendationResourceTypeType](./literals.md#idlerecommendationresourcetypetype) 
2. See [:material-code-brackets: IdleFindingType](./literals.md#idlefindingtype) 
3. See [:material-code-braces: IdleSavingsOpportunityTypeDef](./type_defs.md#idlesavingsopportunitytypedef) 
4. See [:material-code-braces: IdleSavingsOpportunityAfterDiscountsTypeDef](./type_defs.md#idlesavingsopportunityafterdiscountstypedef) 
5. See [:material-code-braces: IdleUtilizationMetricTypeDef](./type_defs.md#idleutilizationmetrictypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## InstanceRecommendationOptionTypeDef

```python
# InstanceRecommendationOptionTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import InstanceRecommendationOptionTypeDef


def get_value() -> InstanceRecommendationOptionTypeDef:
    return {
        "instanceType": ...,
    }


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
# LambdaFunctionMemoryRecommendationOptionTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import LambdaFunctionMemoryRecommendationOptionTypeDef


def get_value() -> LambdaFunctionMemoryRecommendationOptionTypeDef:
    return {
        "rank": ...,
    }


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
# GetEC2RecommendationProjectedMetricsResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetEC2RecommendationProjectedMetricsResponseTypeDef


def get_value() -> GetEC2RecommendationProjectedMetricsResponseTypeDef:
    return {
        "recommendedOptionProjectedMetrics": ...,
    }


# GetEC2RecommendationProjectedMetricsResponseTypeDef definition

class GetEC2RecommendationProjectedMetricsResponseTypeDef(TypedDict):
    recommendedOptionProjectedMetrics: List[RecommendedOptionProjectedMetricTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecommendedOptionProjectedMetricTypeDef](./type_defs.md#recommendedoptionprojectedmetrictypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRDSDatabaseRecommendationProjectedMetricsResponseTypeDef

```python
# GetRDSDatabaseRecommendationProjectedMetricsResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetRDSDatabaseRecommendationProjectedMetricsResponseTypeDef


def get_value() -> GetRDSDatabaseRecommendationProjectedMetricsResponseTypeDef:
    return {
        "recommendedOptionProjectedMetrics": ...,
    }


# GetRDSDatabaseRecommendationProjectedMetricsResponseTypeDef definition

class GetRDSDatabaseRecommendationProjectedMetricsResponseTypeDef(TypedDict):
    recommendedOptionProjectedMetrics: List[RDSDatabaseRecommendedOptionProjectedMetricTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RDSDatabaseRecommendedOptionProjectedMetricTypeDef](./type_defs.md#rdsdatabaserecommendedoptionprojectedmetrictypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RDSDBInstanceRecommendationOptionTypeDef

```python
# RDSDBInstanceRecommendationOptionTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import RDSDBInstanceRecommendationOptionTypeDef


def get_value() -> RDSDBInstanceRecommendationOptionTypeDef:
    return {
        "dbInstanceClass": ...,
    }


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
# RDSDBStorageRecommendationOptionTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import RDSDBStorageRecommendationOptionTypeDef


def get_value() -> RDSDBStorageRecommendationOptionTypeDef:
    return {
        "storageConfiguration": ...,
    }


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
# RecommendationSummaryTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import RecommendationSummaryTypeDef


def get_value() -> RecommendationSummaryTypeDef:
    return {
        "summaries": ...,
    }


# RecommendationSummaryTypeDef definition

class RecommendationSummaryTypeDef(TypedDict):
    summaries: NotRequired[List[SummaryTypeDef]],  # (1)
    idleSummaries: NotRequired[List[IdleSummaryTypeDef]],  # (2)
    recommendationResourceType: NotRequired[RecommendationSourceTypeType],  # (3)
    accountId: NotRequired[str],
    savingsOpportunity: NotRequired[SavingsOpportunityTypeDef],  # (4)
    idleSavingsOpportunity: NotRequired[SavingsOpportunityTypeDef],  # (4)
    aggregatedSavingsOpportunity: NotRequired[SavingsOpportunityTypeDef],  # (4)
    currentPerformanceRiskRatings: NotRequired[CurrentPerformanceRiskRatingsTypeDef],  # (7)
    inferredWorkloadSavings: NotRequired[List[InferredWorkloadSavingTypeDef]],  # (8)
```

1. See [:material-code-braces: SummaryTypeDef](./type_defs.md#summarytypedef) 
2. See [:material-code-braces: IdleSummaryTypeDef](./type_defs.md#idlesummarytypedef) 
3. See [:material-code-brackets: RecommendationSourceTypeType](./literals.md#recommendationsourcetypetype) 
4. See [:material-code-braces: SavingsOpportunityTypeDef](./type_defs.md#savingsopportunitytypedef) 
5. See [:material-code-braces: SavingsOpportunityTypeDef](./type_defs.md#savingsopportunitytypedef) 
6. See [:material-code-braces: SavingsOpportunityTypeDef](./type_defs.md#savingsopportunitytypedef) 
7. See [:material-code-braces: CurrentPerformanceRiskRatingsTypeDef](./type_defs.md#currentperformanceriskratingstypedef) 
8. See [:material-code-braces: InferredWorkloadSavingTypeDef](./type_defs.md#inferredworkloadsavingtypedef) 
## GetRecommendationPreferencesResponseTypeDef

```python
# GetRecommendationPreferencesResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetRecommendationPreferencesResponseTypeDef


def get_value() -> GetRecommendationPreferencesResponseTypeDef:
    return {
        "nextToken": ...,
    }


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
# ECSServiceRecommendationTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import ECSServiceRecommendationTypeDef


def get_value() -> ECSServiceRecommendationTypeDef:
    return {
        "serviceArn": ...,
    }


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
# LicenseRecommendationTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import LicenseRecommendationTypeDef


def get_value() -> LicenseRecommendationTypeDef:
    return {
        "resourceArn": ...,
    }


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
# VolumeRecommendationTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import VolumeRecommendationTypeDef


def get_value() -> VolumeRecommendationTypeDef:
    return {
        "volumeArn": ...,
    }


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
# DescribeRecommendationExportJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import DescribeRecommendationExportJobsResponseTypeDef


def get_value() -> DescribeRecommendationExportJobsResponseTypeDef:
    return {
        "recommendationExportJobs": ...,
    }


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
# AutoScalingGroupRecommendationTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import AutoScalingGroupRecommendationTypeDef


def get_value() -> AutoScalingGroupRecommendationTypeDef:
    return {
        "accountId": ...,
    }


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
## GetIdleRecommendationsResponseTypeDef

```python
# GetIdleRecommendationsResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetIdleRecommendationsResponseTypeDef


def get_value() -> GetIdleRecommendationsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# GetIdleRecommendationsResponseTypeDef definition

class GetIdleRecommendationsResponseTypeDef(TypedDict):
    idleRecommendations: List[IdleRecommendationTypeDef],  # (1)
    errors: List[IdleRecommendationErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: IdleRecommendationTypeDef](./type_defs.md#idlerecommendationtypedef) 
2. See [:material-code-braces: IdleRecommendationErrorTypeDef](./type_defs.md#idlerecommendationerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstanceRecommendationTypeDef

```python
# InstanceRecommendationTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import InstanceRecommendationTypeDef


def get_value() -> InstanceRecommendationTypeDef:
    return {
        "instanceArn": ...,
    }


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
# LambdaFunctionRecommendationTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import LambdaFunctionRecommendationTypeDef


def get_value() -> LambdaFunctionRecommendationTypeDef:
    return {
        "functionArn": ...,
    }


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
# RDSDBRecommendationTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import RDSDBRecommendationTypeDef


def get_value() -> RDSDBRecommendationTypeDef:
    return {
        "resourceArn": ...,
    }


# RDSDBRecommendationTypeDef definition

class RDSDBRecommendationTypeDef(TypedDict):
    resourceArn: NotRequired[str],
    accountId: NotRequired[str],
    engine: NotRequired[str],
    engineVersion: NotRequired[str],
    promotionTier: NotRequired[int],
    currentDBInstanceClass: NotRequired[str],
    currentStorageConfiguration: NotRequired[DBStorageConfigurationTypeDef],  # (1)
    dbClusterIdentifier: NotRequired[str],
    idle: NotRequired[IdleType],  # (2)
    instanceFinding: NotRequired[RDSInstanceFindingType],  # (3)
    storageFinding: NotRequired[RDSStorageFindingType],  # (4)
    instanceFindingReasonCodes: NotRequired[List[RDSInstanceFindingReasonCodeType]],  # (5)
    currentInstancePerformanceRisk: NotRequired[RDSCurrentInstancePerformanceRiskType],  # (6)
    storageFindingReasonCodes: NotRequired[List[RDSStorageFindingReasonCodeType]],  # (7)
    instanceRecommendationOptions: NotRequired[List[RDSDBInstanceRecommendationOptionTypeDef]],  # (8)
    storageRecommendationOptions: NotRequired[List[RDSDBStorageRecommendationOptionTypeDef]],  # (9)
    utilizationMetrics: NotRequired[List[RDSDBUtilizationMetricTypeDef]],  # (10)
    effectiveRecommendationPreferences: NotRequired[RDSEffectiveRecommendationPreferencesTypeDef],  # (11)
    lookbackPeriodInDays: NotRequired[float],
    lastRefreshTimestamp: NotRequired[datetime],
    tags: NotRequired[List[TagTypeDef]],  # (12)
```

1. See [:material-code-braces: DBStorageConfigurationTypeDef](./type_defs.md#dbstorageconfigurationtypedef) 
2. See [:material-code-brackets: IdleType](./literals.md#idletype) 
3. See [:material-code-brackets: RDSInstanceFindingType](./literals.md#rdsinstancefindingtype) 
4. See [:material-code-brackets: RDSStorageFindingType](./literals.md#rdsstoragefindingtype) 
5. See [:material-code-brackets: RDSInstanceFindingReasonCodeType](./literals.md#rdsinstancefindingreasoncodetype) 
6. See [:material-code-brackets: RDSCurrentInstancePerformanceRiskType](./literals.md#rdscurrentinstanceperformancerisktype) 
7. See [:material-code-brackets: RDSStorageFindingReasonCodeType](./literals.md#rdsstoragefindingreasoncodetype) 
8. See [:material-code-braces: RDSDBInstanceRecommendationOptionTypeDef](./type_defs.md#rdsdbinstancerecommendationoptiontypedef) 
9. See [:material-code-braces: RDSDBStorageRecommendationOptionTypeDef](./type_defs.md#rdsdbstoragerecommendationoptiontypedef) 
10. See [:material-code-braces: RDSDBUtilizationMetricTypeDef](./type_defs.md#rdsdbutilizationmetrictypedef) 
11. See [:material-code-braces: RDSEffectiveRecommendationPreferencesTypeDef](./type_defs.md#rdseffectiverecommendationpreferencestypedef) 
12. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetRecommendationSummariesResponseTypeDef

```python
# GetRecommendationSummariesResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetRecommendationSummariesResponseTypeDef


def get_value() -> GetRecommendationSummariesResponseTypeDef:
    return {
        "nextToken": ...,
    }


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
# GetECSServiceRecommendationsResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetECSServiceRecommendationsResponseTypeDef


def get_value() -> GetECSServiceRecommendationsResponseTypeDef:
    return {
        "nextToken": ...,
    }


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
# GetLicenseRecommendationsResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetLicenseRecommendationsResponseTypeDef


def get_value() -> GetLicenseRecommendationsResponseTypeDef:
    return {
        "nextToken": ...,
    }


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
# GetEBSVolumeRecommendationsResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetEBSVolumeRecommendationsResponseTypeDef


def get_value() -> GetEBSVolumeRecommendationsResponseTypeDef:
    return {
        "nextToken": ...,
    }


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
# GetAutoScalingGroupRecommendationsResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetAutoScalingGroupRecommendationsResponseTypeDef


def get_value() -> GetAutoScalingGroupRecommendationsResponseTypeDef:
    return {
        "nextToken": ...,
    }


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
# GetEC2InstanceRecommendationsResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetEC2InstanceRecommendationsResponseTypeDef


def get_value() -> GetEC2InstanceRecommendationsResponseTypeDef:
    return {
        "nextToken": ...,
    }


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
# GetLambdaFunctionRecommendationsResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetLambdaFunctionRecommendationsResponseTypeDef


def get_value() -> GetLambdaFunctionRecommendationsResponseTypeDef:
    return {
        "nextToken": ...,
    }


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
# GetRDSDatabaseRecommendationsResponseTypeDef TypedDict usage example

from types_aiobotocore_compute_optimizer.type_defs import GetRDSDatabaseRecommendationsResponseTypeDef


def get_value() -> GetRDSDatabaseRecommendationsResponseTypeDef:
    return {
        "nextToken": ...,
    }


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
