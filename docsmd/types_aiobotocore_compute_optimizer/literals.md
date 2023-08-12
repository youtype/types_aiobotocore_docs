# Literals

> [Index](../README.md) > [ComputeOptimizer](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [ComputeOptimizer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
    type annotations stubs module [types-aiobotocore-compute-optimizer](https://pypi.org/project/types-aiobotocore-compute-optimizer/).

## AutoScalingConfigurationType

```python
# AutoScalingConfigurationType usage example

from types_aiobotocore_compute_optimizer.literals import AutoScalingConfigurationType

def get_value() -> AutoScalingConfigurationType:
    return "TargetTrackingScalingCpu"
```

```python
# AutoScalingConfigurationType definition

AutoScalingConfigurationType = Literal[
    "TargetTrackingScalingCpu",
    "TargetTrackingScalingMemory",
]
```
## CpuVendorArchitectureType

```python
# CpuVendorArchitectureType usage example

from types_aiobotocore_compute_optimizer.literals import CpuVendorArchitectureType

def get_value() -> CpuVendorArchitectureType:
    return "AWS_ARM64"
```

```python
# CpuVendorArchitectureType definition

CpuVendorArchitectureType = Literal[
    "AWS_ARM64",
    "CURRENT",
]
```
## CurrencyType

```python
# CurrencyType usage example

from types_aiobotocore_compute_optimizer.literals import CurrencyType

def get_value() -> CurrencyType:
    return "CNY"
```

```python
# CurrencyType definition

CurrencyType = Literal[
    "CNY",
    "USD",
]
```
## CurrentPerformanceRiskType

```python
# CurrentPerformanceRiskType usage example

from types_aiobotocore_compute_optimizer.literals import CurrentPerformanceRiskType

def get_value() -> CurrentPerformanceRiskType:
    return "High"
```

```python
# CurrentPerformanceRiskType definition

CurrentPerformanceRiskType = Literal[
    "High",
    "Low",
    "Medium",
    "VeryLow",
]
```
## DescribeRecommendationExportJobsPaginatorName

```python
# DescribeRecommendationExportJobsPaginatorName usage example

from types_aiobotocore_compute_optimizer.literals import DescribeRecommendationExportJobsPaginatorName

def get_value() -> DescribeRecommendationExportJobsPaginatorName:
    return "describe_recommendation_export_jobs"
```

```python
# DescribeRecommendationExportJobsPaginatorName definition

DescribeRecommendationExportJobsPaginatorName = Literal[
    "describe_recommendation_export_jobs",
]
```
## EBSFilterNameType

```python
# EBSFilterNameType usage example

from types_aiobotocore_compute_optimizer.literals import EBSFilterNameType

def get_value() -> EBSFilterNameType:
    return "Finding"
```

```python
# EBSFilterNameType definition

EBSFilterNameType = Literal[
    "Finding",
]
```
## EBSFindingType

```python
# EBSFindingType usage example

from types_aiobotocore_compute_optimizer.literals import EBSFindingType

def get_value() -> EBSFindingType:
    return "NotOptimized"
```

```python
# EBSFindingType definition

EBSFindingType = Literal[
    "NotOptimized",
    "Optimized",
]
```
## EBSMetricNameType

```python
# EBSMetricNameType usage example

from types_aiobotocore_compute_optimizer.literals import EBSMetricNameType

def get_value() -> EBSMetricNameType:
    return "VolumeReadBytesPerSecond"
```

```python
# EBSMetricNameType definition

EBSMetricNameType = Literal[
    "VolumeReadBytesPerSecond",
    "VolumeReadOpsPerSecond",
    "VolumeWriteBytesPerSecond",
    "VolumeWriteOpsPerSecond",
]
```
## ECSServiceLaunchTypeType

```python
# ECSServiceLaunchTypeType usage example

from types_aiobotocore_compute_optimizer.literals import ECSServiceLaunchTypeType

def get_value() -> ECSServiceLaunchTypeType:
    return "EC2"
```

```python
# ECSServiceLaunchTypeType definition

ECSServiceLaunchTypeType = Literal[
    "EC2",
    "Fargate",
]
```
## ECSServiceMetricNameType

```python
# ECSServiceMetricNameType usage example

from types_aiobotocore_compute_optimizer.literals import ECSServiceMetricNameType

def get_value() -> ECSServiceMetricNameType:
    return "Cpu"
```

```python
# ECSServiceMetricNameType definition

ECSServiceMetricNameType = Literal[
    "Cpu",
    "Memory",
]
```
## ECSServiceMetricStatisticType

```python
# ECSServiceMetricStatisticType usage example

from types_aiobotocore_compute_optimizer.literals import ECSServiceMetricStatisticType

def get_value() -> ECSServiceMetricStatisticType:
    return "Average"
```

```python
# ECSServiceMetricStatisticType definition

ECSServiceMetricStatisticType = Literal[
    "Average",
    "Maximum",
]
```
## ECSServiceRecommendationFilterNameType

```python
# ECSServiceRecommendationFilterNameType usage example

from types_aiobotocore_compute_optimizer.literals import ECSServiceRecommendationFilterNameType

def get_value() -> ECSServiceRecommendationFilterNameType:
    return "Finding"
```

```python
# ECSServiceRecommendationFilterNameType definition

ECSServiceRecommendationFilterNameType = Literal[
    "Finding",
    "FindingReasonCode",
]
```
## ECSServiceRecommendationFindingReasonCodeType

```python
# ECSServiceRecommendationFindingReasonCodeType usage example

from types_aiobotocore_compute_optimizer.literals import ECSServiceRecommendationFindingReasonCodeType

def get_value() -> ECSServiceRecommendationFindingReasonCodeType:
    return "CPUOverprovisioned"
```

```python
# ECSServiceRecommendationFindingReasonCodeType definition

ECSServiceRecommendationFindingReasonCodeType = Literal[
    "CPUOverprovisioned",
    "CPUUnderprovisioned",
    "MemoryOverprovisioned",
    "MemoryUnderprovisioned",
]
```
## ECSServiceRecommendationFindingType

```python
# ECSServiceRecommendationFindingType usage example

from types_aiobotocore_compute_optimizer.literals import ECSServiceRecommendationFindingType

def get_value() -> ECSServiceRecommendationFindingType:
    return "Optimized"
```

```python
# ECSServiceRecommendationFindingType definition

ECSServiceRecommendationFindingType = Literal[
    "Optimized",
    "Overprovisioned",
    "Underprovisioned",
]
```
## EnhancedInfrastructureMetricsType

```python
# EnhancedInfrastructureMetricsType usage example

from types_aiobotocore_compute_optimizer.literals import EnhancedInfrastructureMetricsType

def get_value() -> EnhancedInfrastructureMetricsType:
    return "Active"
```

```python
# EnhancedInfrastructureMetricsType definition

EnhancedInfrastructureMetricsType = Literal[
    "Active",
    "Inactive",
]
```
## EnrollmentFilterNameType

```python
# EnrollmentFilterNameType usage example

from types_aiobotocore_compute_optimizer.literals import EnrollmentFilterNameType

def get_value() -> EnrollmentFilterNameType:
    return "Status"
```

```python
# EnrollmentFilterNameType definition

EnrollmentFilterNameType = Literal[
    "Status",
]
```
## ExportableAutoScalingGroupFieldType

```python
# ExportableAutoScalingGroupFieldType usage example

from types_aiobotocore_compute_optimizer.literals import ExportableAutoScalingGroupFieldType

def get_value() -> ExportableAutoScalingGroupFieldType:
    return "AccountId"
```

```python
# ExportableAutoScalingGroupFieldType definition

ExportableAutoScalingGroupFieldType = Literal[
    "AccountId",
    "AutoScalingGroupArn",
    "AutoScalingGroupName",
    "CurrentConfigurationDesiredCapacity",
    "CurrentConfigurationInstanceType",
    "CurrentConfigurationMaxSize",
    "CurrentConfigurationMinSize",
    "CurrentMemory",
    "CurrentNetwork",
    "CurrentOnDemandPrice",
    "CurrentPerformanceRisk",
    "CurrentStandardOneYearNoUpfrontReservedPrice",
    "CurrentStandardThreeYearNoUpfrontReservedPrice",
    "CurrentStorage",
    "CurrentVCpus",
    "EffectiveRecommendationPreferencesCpuVendorArchitectures",
    "EffectiveRecommendationPreferencesEnhancedInfrastructureMetrics",
    "EffectiveRecommendationPreferencesInferredWorkloadTypes",
    "Finding",
    "InferredWorkloadTypes",
    "LastRefreshTimestamp",
    "LookbackPeriodInDays",
    "RecommendationOptionsConfigurationDesiredCapacity",
    "RecommendationOptionsConfigurationInstanceType",
    "RecommendationOptionsConfigurationMaxSize",
    "RecommendationOptionsConfigurationMinSize",
    "RecommendationOptionsEstimatedMonthlySavingsCurrency",
    "RecommendationOptionsEstimatedMonthlySavingsValue",
    "RecommendationOptionsMemory",
    "RecommendationOptionsMigrationEffort",
    "RecommendationOptionsNetwork",
    "RecommendationOptionsOnDemandPrice",
    "RecommendationOptionsPerformanceRisk",
    "RecommendationOptionsProjectedUtilizationMetricsCpuMaximum",
    "RecommendationOptionsProjectedUtilizationMetricsMemoryMaximum",
    "RecommendationOptionsSavingsOpportunityPercentage",
    "RecommendationOptionsStandardOneYearNoUpfrontReservedPrice",
    "RecommendationOptionsStandardThreeYearNoUpfrontReservedPrice",
    "RecommendationOptionsStorage",
    "RecommendationOptionsVcpus",
    "UtilizationMetricsCpuMaximum",
    "UtilizationMetricsDiskReadBytesPerSecondMaximum",
    "UtilizationMetricsDiskReadOpsPerSecondMaximum",
    "UtilizationMetricsDiskWriteBytesPerSecondMaximum",
    "UtilizationMetricsDiskWriteOpsPerSecondMaximum",
    "UtilizationMetricsEbsReadBytesPerSecondMaximum",
    "UtilizationMetricsEbsReadOpsPerSecondMaximum",
    "UtilizationMetricsEbsWriteBytesPerSecondMaximum",
    "UtilizationMetricsEbsWriteOpsPerSecondMaximum",
    "UtilizationMetricsMemoryMaximum",
    "UtilizationMetricsNetworkInBytesPerSecondMaximum",
    "UtilizationMetricsNetworkOutBytesPerSecondMaximum",
    "UtilizationMetricsNetworkPacketsInPerSecondMaximum",
    "UtilizationMetricsNetworkPacketsOutPerSecondMaximum",
]
```
## ExportableECSServiceFieldType

```python
# ExportableECSServiceFieldType usage example

from types_aiobotocore_compute_optimizer.literals import ExportableECSServiceFieldType

def get_value() -> ExportableECSServiceFieldType:
    return "AccountId"
```

```python
# ExportableECSServiceFieldType definition

ExportableECSServiceFieldType = Literal[
    "AccountId",
    "CurrentPerformanceRisk",
    "CurrentServiceConfigurationAutoScalingConfiguration",
    "CurrentServiceConfigurationCpu",
    "CurrentServiceConfigurationMemory",
    "CurrentServiceConfigurationTaskDefinitionArn",
    "CurrentServiceContainerConfigurations",
    "Finding",
    "FindingReasonCodes",
    "LastRefreshTimestamp",
    "LaunchType",
    "LookbackPeriodInDays",
    "RecommendationOptionsContainerRecommendations",
    "RecommendationOptionsCpu",
    "RecommendationOptionsEstimatedMonthlySavingsCurrency",
    "RecommendationOptionsEstimatedMonthlySavingsValue",
    "RecommendationOptionsMemory",
    "RecommendationOptionsProjectedUtilizationMetricsCpuMaximum",
    "RecommendationOptionsProjectedUtilizationMetricsMemoryMaximum",
    "RecommendationOptionsSavingsOpportunityPercentage",
    "ServiceArn",
    "Tags",
    "UtilizationMetricsCpuMaximum",
    "UtilizationMetricsMemoryMaximum",
]
```
## ExportableInstanceFieldType

```python
# ExportableInstanceFieldType usage example

from types_aiobotocore_compute_optimizer.literals import ExportableInstanceFieldType

def get_value() -> ExportableInstanceFieldType:
    return "AccountId"
```

```python
# ExportableInstanceFieldType definition

ExportableInstanceFieldType = Literal[
    "AccountId",
    "CurrentInstanceType",
    "CurrentMemory",
    "CurrentNetwork",
    "CurrentOnDemandPrice",
    "CurrentPerformanceRisk",
    "CurrentStandardOneYearNoUpfrontReservedPrice",
    "CurrentStandardThreeYearNoUpfrontReservedPrice",
    "CurrentStorage",
    "CurrentVCpus",
    "EffectiveRecommendationPreferencesCpuVendorArchitectures",
    "EffectiveRecommendationPreferencesEnhancedInfrastructureMetrics",
    "EffectiveRecommendationPreferencesExternalMetricsSource",
    "EffectiveRecommendationPreferencesInferredWorkloadTypes",
    "ExternalMetricStatusCode",
    "ExternalMetricStatusReason",
    "Finding",
    "FindingReasonCodes",
    "InferredWorkloadTypes",
    "InstanceArn",
    "InstanceName",
    "InstanceState",
    "LastRefreshTimestamp",
    "LookbackPeriodInDays",
    "RecommendationOptionsEstimatedMonthlySavingsCurrency",
    "RecommendationOptionsEstimatedMonthlySavingsValue",
    "RecommendationOptionsInstanceType",
    "RecommendationOptionsMemory",
    "RecommendationOptionsMigrationEffort",
    "RecommendationOptionsNetwork",
    "RecommendationOptionsOnDemandPrice",
    "RecommendationOptionsPerformanceRisk",
    "RecommendationOptionsPlatformDifferences",
    "RecommendationOptionsProjectedUtilizationMetricsCpuMaximum",
    "RecommendationOptionsProjectedUtilizationMetricsMemoryMaximum",
    "RecommendationOptionsSavingsOpportunityPercentage",
    "RecommendationOptionsStandardOneYearNoUpfrontReservedPrice",
    "RecommendationOptionsStandardThreeYearNoUpfrontReservedPrice",
    "RecommendationOptionsStorage",
    "RecommendationOptionsVcpus",
    "RecommendationsSourcesRecommendationSourceArn",
    "RecommendationsSourcesRecommendationSourceType",
    "Tags",
    "UtilizationMetricsCpuMaximum",
    "UtilizationMetricsDiskReadBytesPerSecondMaximum",
    "UtilizationMetricsDiskReadOpsPerSecondMaximum",
    "UtilizationMetricsDiskWriteBytesPerSecondMaximum",
    "UtilizationMetricsDiskWriteOpsPerSecondMaximum",
    "UtilizationMetricsEbsReadBytesPerSecondMaximum",
    "UtilizationMetricsEbsReadOpsPerSecondMaximum",
    "UtilizationMetricsEbsWriteBytesPerSecondMaximum",
    "UtilizationMetricsEbsWriteOpsPerSecondMaximum",
    "UtilizationMetricsMemoryMaximum",
    "UtilizationMetricsNetworkInBytesPerSecondMaximum",
    "UtilizationMetricsNetworkOutBytesPerSecondMaximum",
    "UtilizationMetricsNetworkPacketsInPerSecondMaximum",
    "UtilizationMetricsNetworkPacketsOutPerSecondMaximum",
]
```
## ExportableLambdaFunctionFieldType

```python
# ExportableLambdaFunctionFieldType usage example

from types_aiobotocore_compute_optimizer.literals import ExportableLambdaFunctionFieldType

def get_value() -> ExportableLambdaFunctionFieldType:
    return "AccountId"
```

```python
# ExportableLambdaFunctionFieldType definition

ExportableLambdaFunctionFieldType = Literal[
    "AccountId",
    "CurrentConfigurationMemorySize",
    "CurrentConfigurationTimeout",
    "CurrentCostAverage",
    "CurrentCostTotal",
    "CurrentPerformanceRisk",
    "Finding",
    "FindingReasonCodes",
    "FunctionArn",
    "FunctionVersion",
    "LastRefreshTimestamp",
    "LookbackPeriodInDays",
    "NumberOfInvocations",
    "RecommendationOptionsConfigurationMemorySize",
    "RecommendationOptionsCostHigh",
    "RecommendationOptionsCostLow",
    "RecommendationOptionsEstimatedMonthlySavingsCurrency",
    "RecommendationOptionsEstimatedMonthlySavingsValue",
    "RecommendationOptionsProjectedUtilizationMetricsDurationExpected",
    "RecommendationOptionsProjectedUtilizationMetricsDurationLowerBound",
    "RecommendationOptionsProjectedUtilizationMetricsDurationUpperBound",
    "RecommendationOptionsSavingsOpportunityPercentage",
    "Tags",
    "UtilizationMetricsDurationAverage",
    "UtilizationMetricsDurationMaximum",
    "UtilizationMetricsMemoryAverage",
    "UtilizationMetricsMemoryMaximum",
]
```
## ExportableVolumeFieldType

```python
# ExportableVolumeFieldType usage example

from types_aiobotocore_compute_optimizer.literals import ExportableVolumeFieldType

def get_value() -> ExportableVolumeFieldType:
    return "AccountId"
```

```python
# ExportableVolumeFieldType definition

ExportableVolumeFieldType = Literal[
    "AccountId",
    "CurrentConfigurationVolumeBaselineIOPS",
    "CurrentConfigurationVolumeBaselineThroughput",
    "CurrentConfigurationVolumeBurstIOPS",
    "CurrentConfigurationVolumeBurstThroughput",
    "CurrentConfigurationVolumeSize",
    "CurrentConfigurationVolumeType",
    "CurrentMonthlyPrice",
    "CurrentPerformanceRisk",
    "Finding",
    "LastRefreshTimestamp",
    "LookbackPeriodInDays",
    "RecommendationOptionsConfigurationVolumeBaselineIOPS",
    "RecommendationOptionsConfigurationVolumeBaselineThroughput",
    "RecommendationOptionsConfigurationVolumeBurstIOPS",
    "RecommendationOptionsConfigurationVolumeBurstThroughput",
    "RecommendationOptionsConfigurationVolumeSize",
    "RecommendationOptionsConfigurationVolumeType",
    "RecommendationOptionsEstimatedMonthlySavingsCurrency",
    "RecommendationOptionsEstimatedMonthlySavingsValue",
    "RecommendationOptionsMonthlyPrice",
    "RecommendationOptionsPerformanceRisk",
    "RecommendationOptionsSavingsOpportunityPercentage",
    "RootVolume",
    "Tags",
    "UtilizationMetricsVolumeReadBytesPerSecondMaximum",
    "UtilizationMetricsVolumeReadOpsPerSecondMaximum",
    "UtilizationMetricsVolumeWriteBytesPerSecondMaximum",
    "UtilizationMetricsVolumeWriteOpsPerSecondMaximum",
    "VolumeArn",
]
```
## ExternalMetricStatusCodeType

```python
# ExternalMetricStatusCodeType usage example

from types_aiobotocore_compute_optimizer.literals import ExternalMetricStatusCodeType

def get_value() -> ExternalMetricStatusCodeType:
    return "DATADOG_INTEGRATION_ERROR"
```

```python
# ExternalMetricStatusCodeType definition

ExternalMetricStatusCodeType = Literal[
    "DATADOG_INTEGRATION_ERROR",
    "DYNATRACE_INTEGRATION_ERROR",
    "INSTANA_INTEGRATION_ERROR",
    "INSUFFICIENT_DATADOG_METRICS",
    "INSUFFICIENT_DYNATRACE_METRICS",
    "INSUFFICIENT_INSTANA_METRICS",
    "INSUFFICIENT_NEWRELIC_METRICS",
    "INTEGRATION_SUCCESS",
    "NEWRELIC_INTEGRATION_ERROR",
    "NO_EXTERNAL_METRIC_SET",
]
```
## ExternalMetricsSourceType

```python
# ExternalMetricsSourceType usage example

from types_aiobotocore_compute_optimizer.literals import ExternalMetricsSourceType

def get_value() -> ExternalMetricsSourceType:
    return "Datadog"
```

```python
# ExternalMetricsSourceType definition

ExternalMetricsSourceType = Literal[
    "Datadog",
    "Dynatrace",
    "Instana",
    "NewRelic",
]
```
## FileFormatType

```python
# FileFormatType usage example

from types_aiobotocore_compute_optimizer.literals import FileFormatType

def get_value() -> FileFormatType:
    return "Csv"
```

```python
# FileFormatType definition

FileFormatType = Literal[
    "Csv",
]
```
## FilterNameType

```python
# FilterNameType usage example

from types_aiobotocore_compute_optimizer.literals import FilterNameType

def get_value() -> FilterNameType:
    return "Finding"
```

```python
# FilterNameType definition

FilterNameType = Literal[
    "Finding",
    "FindingReasonCodes",
    "InferredWorkloadTypes",
    "RecommendationSourceType",
]
```
## FindingReasonCodeType

```python
# FindingReasonCodeType usage example

from types_aiobotocore_compute_optimizer.literals import FindingReasonCodeType

def get_value() -> FindingReasonCodeType:
    return "MemoryOverprovisioned"
```

```python
# FindingReasonCodeType definition

FindingReasonCodeType = Literal[
    "MemoryOverprovisioned",
    "MemoryUnderprovisioned",
]
```
## FindingType

```python
# FindingType usage example

from types_aiobotocore_compute_optimizer.literals import FindingType

def get_value() -> FindingType:
    return "NotOptimized"
```

```python
# FindingType definition

FindingType = Literal[
    "NotOptimized",
    "Optimized",
    "Overprovisioned",
    "Underprovisioned",
]
```
## GetEnrollmentStatusesForOrganizationPaginatorName

```python
# GetEnrollmentStatusesForOrganizationPaginatorName usage example

from types_aiobotocore_compute_optimizer.literals import GetEnrollmentStatusesForOrganizationPaginatorName

def get_value() -> GetEnrollmentStatusesForOrganizationPaginatorName:
    return "get_enrollment_statuses_for_organization"
```

```python
# GetEnrollmentStatusesForOrganizationPaginatorName definition

GetEnrollmentStatusesForOrganizationPaginatorName = Literal[
    "get_enrollment_statuses_for_organization",
]
```
## GetLambdaFunctionRecommendationsPaginatorName

```python
# GetLambdaFunctionRecommendationsPaginatorName usage example

from types_aiobotocore_compute_optimizer.literals import GetLambdaFunctionRecommendationsPaginatorName

def get_value() -> GetLambdaFunctionRecommendationsPaginatorName:
    return "get_lambda_function_recommendations"
```

```python
# GetLambdaFunctionRecommendationsPaginatorName definition

GetLambdaFunctionRecommendationsPaginatorName = Literal[
    "get_lambda_function_recommendations",
]
```
## GetRecommendationPreferencesPaginatorName

```python
# GetRecommendationPreferencesPaginatorName usage example

from types_aiobotocore_compute_optimizer.literals import GetRecommendationPreferencesPaginatorName

def get_value() -> GetRecommendationPreferencesPaginatorName:
    return "get_recommendation_preferences"
```

```python
# GetRecommendationPreferencesPaginatorName definition

GetRecommendationPreferencesPaginatorName = Literal[
    "get_recommendation_preferences",
]
```
## GetRecommendationSummariesPaginatorName

```python
# GetRecommendationSummariesPaginatorName usage example

from types_aiobotocore_compute_optimizer.literals import GetRecommendationSummariesPaginatorName

def get_value() -> GetRecommendationSummariesPaginatorName:
    return "get_recommendation_summaries"
```

```python
# GetRecommendationSummariesPaginatorName definition

GetRecommendationSummariesPaginatorName = Literal[
    "get_recommendation_summaries",
]
```
## InferredWorkloadTypeType

```python
# InferredWorkloadTypeType usage example

from types_aiobotocore_compute_optimizer.literals import InferredWorkloadTypeType

def get_value() -> InferredWorkloadTypeType:
    return "AmazonEmr"
```

```python
# InferredWorkloadTypeType definition

InferredWorkloadTypeType = Literal[
    "AmazonEmr",
    "ApacheCassandra",
    "ApacheHadoop",
    "Kafka",
    "Memcached",
    "Nginx",
    "PostgreSql",
    "Redis",
    "SQLServer",
]
```
## InferredWorkloadTypesPreferenceType

```python
# InferredWorkloadTypesPreferenceType usage example

from types_aiobotocore_compute_optimizer.literals import InferredWorkloadTypesPreferenceType

def get_value() -> InferredWorkloadTypesPreferenceType:
    return "Active"
```

```python
# InferredWorkloadTypesPreferenceType definition

InferredWorkloadTypesPreferenceType = Literal[
    "Active",
    "Inactive",
]
```
## InstanceRecommendationFindingReasonCodeType

```python
# InstanceRecommendationFindingReasonCodeType usage example

from types_aiobotocore_compute_optimizer.literals import InstanceRecommendationFindingReasonCodeType

def get_value() -> InstanceRecommendationFindingReasonCodeType:
    return "CPUOverprovisioned"
```

```python
# InstanceRecommendationFindingReasonCodeType definition

InstanceRecommendationFindingReasonCodeType = Literal[
    "CPUOverprovisioned",
    "CPUUnderprovisioned",
    "DiskIOPSOverprovisioned",
    "DiskIOPSUnderprovisioned",
    "DiskThroughputOverprovisioned",
    "DiskThroughputUnderprovisioned",
    "EBSIOPSOverprovisioned",
    "EBSIOPSUnderprovisioned",
    "EBSThroughputOverprovisioned",
    "EBSThroughputUnderprovisioned",
    "MemoryOverprovisioned",
    "MemoryUnderprovisioned",
    "NetworkBandwidthOverprovisioned",
    "NetworkBandwidthUnderprovisioned",
    "NetworkPPSOverprovisioned",
    "NetworkPPSUnderprovisioned",
]
```
## InstanceStateType

```python
# InstanceStateType usage example

from types_aiobotocore_compute_optimizer.literals import InstanceStateType

def get_value() -> InstanceStateType:
    return "pending"
```

```python
# InstanceStateType definition

InstanceStateType = Literal[
    "pending",
    "running",
    "shutting-down",
    "stopped",
    "stopping",
    "terminated",
]
```
## JobFilterNameType

```python
# JobFilterNameType usage example

from types_aiobotocore_compute_optimizer.literals import JobFilterNameType

def get_value() -> JobFilterNameType:
    return "JobStatus"
```

```python
# JobFilterNameType definition

JobFilterNameType = Literal[
    "JobStatus",
    "ResourceType",
]
```
## JobStatusType

```python
# JobStatusType usage example

from types_aiobotocore_compute_optimizer.literals import JobStatusType

def get_value() -> JobStatusType:
    return "Complete"
```

```python
# JobStatusType definition

JobStatusType = Literal[
    "Complete",
    "Failed",
    "InProgress",
    "Queued",
]
```
## LambdaFunctionMemoryMetricNameType

```python
# LambdaFunctionMemoryMetricNameType usage example

from types_aiobotocore_compute_optimizer.literals import LambdaFunctionMemoryMetricNameType

def get_value() -> LambdaFunctionMemoryMetricNameType:
    return "Duration"
```

```python
# LambdaFunctionMemoryMetricNameType definition

LambdaFunctionMemoryMetricNameType = Literal[
    "Duration",
]
```
## LambdaFunctionMemoryMetricStatisticType

```python
# LambdaFunctionMemoryMetricStatisticType usage example

from types_aiobotocore_compute_optimizer.literals import LambdaFunctionMemoryMetricStatisticType

def get_value() -> LambdaFunctionMemoryMetricStatisticType:
    return "Expected"
```

```python
# LambdaFunctionMemoryMetricStatisticType definition

LambdaFunctionMemoryMetricStatisticType = Literal[
    "Expected",
    "LowerBound",
    "UpperBound",
]
```
## LambdaFunctionMetricNameType

```python
# LambdaFunctionMetricNameType usage example

from types_aiobotocore_compute_optimizer.literals import LambdaFunctionMetricNameType

def get_value() -> LambdaFunctionMetricNameType:
    return "Duration"
```

```python
# LambdaFunctionMetricNameType definition

LambdaFunctionMetricNameType = Literal[
    "Duration",
    "Memory",
]
```
## LambdaFunctionMetricStatisticType

```python
# LambdaFunctionMetricStatisticType usage example

from types_aiobotocore_compute_optimizer.literals import LambdaFunctionMetricStatisticType

def get_value() -> LambdaFunctionMetricStatisticType:
    return "Average"
```

```python
# LambdaFunctionMetricStatisticType definition

LambdaFunctionMetricStatisticType = Literal[
    "Average",
    "Maximum",
]
```
## LambdaFunctionRecommendationFilterNameType

```python
# LambdaFunctionRecommendationFilterNameType usage example

from types_aiobotocore_compute_optimizer.literals import LambdaFunctionRecommendationFilterNameType

def get_value() -> LambdaFunctionRecommendationFilterNameType:
    return "Finding"
```

```python
# LambdaFunctionRecommendationFilterNameType definition

LambdaFunctionRecommendationFilterNameType = Literal[
    "Finding",
    "FindingReasonCode",
]
```
## LambdaFunctionRecommendationFindingReasonCodeType

```python
# LambdaFunctionRecommendationFindingReasonCodeType usage example

from types_aiobotocore_compute_optimizer.literals import LambdaFunctionRecommendationFindingReasonCodeType

def get_value() -> LambdaFunctionRecommendationFindingReasonCodeType:
    return "Inconclusive"
```

```python
# LambdaFunctionRecommendationFindingReasonCodeType definition

LambdaFunctionRecommendationFindingReasonCodeType = Literal[
    "Inconclusive",
    "InsufficientData",
    "MemoryOverprovisioned",
    "MemoryUnderprovisioned",
]
```
## LambdaFunctionRecommendationFindingType

```python
# LambdaFunctionRecommendationFindingType usage example

from types_aiobotocore_compute_optimizer.literals import LambdaFunctionRecommendationFindingType

def get_value() -> LambdaFunctionRecommendationFindingType:
    return "NotOptimized"
```

```python
# LambdaFunctionRecommendationFindingType definition

LambdaFunctionRecommendationFindingType = Literal[
    "NotOptimized",
    "Optimized",
    "Unavailable",
]
```
## MetricNameType

```python
# MetricNameType usage example

from types_aiobotocore_compute_optimizer.literals import MetricNameType

def get_value() -> MetricNameType:
    return "Cpu"
```

```python
# MetricNameType definition

MetricNameType = Literal[
    "Cpu",
    "DISK_READ_BYTES_PER_SECOND",
    "DISK_READ_OPS_PER_SECOND",
    "DISK_WRITE_BYTES_PER_SECOND",
    "DISK_WRITE_OPS_PER_SECOND",
    "EBS_READ_BYTES_PER_SECOND",
    "EBS_READ_OPS_PER_SECOND",
    "EBS_WRITE_BYTES_PER_SECOND",
    "EBS_WRITE_OPS_PER_SECOND",
    "Memory",
    "NETWORK_IN_BYTES_PER_SECOND",
    "NETWORK_OUT_BYTES_PER_SECOND",
    "NETWORK_PACKETS_IN_PER_SECOND",
    "NETWORK_PACKETS_OUT_PER_SECOND",
]
```
## MetricStatisticType

```python
# MetricStatisticType usage example

from types_aiobotocore_compute_optimizer.literals import MetricStatisticType

def get_value() -> MetricStatisticType:
    return "Average"
```

```python
# MetricStatisticType definition

MetricStatisticType = Literal[
    "Average",
    "Maximum",
]
```
## MigrationEffortType

```python
# MigrationEffortType usage example

from types_aiobotocore_compute_optimizer.literals import MigrationEffortType

def get_value() -> MigrationEffortType:
    return "High"
```

```python
# MigrationEffortType definition

MigrationEffortType = Literal[
    "High",
    "Low",
    "Medium",
    "VeryLow",
]
```
## PlatformDifferenceType

```python
# PlatformDifferenceType usage example

from types_aiobotocore_compute_optimizer.literals import PlatformDifferenceType

def get_value() -> PlatformDifferenceType:
    return "Architecture"
```

```python
# PlatformDifferenceType definition

PlatformDifferenceType = Literal[
    "Architecture",
    "Hypervisor",
    "InstanceStoreAvailability",
    "NetworkInterface",
    "StorageInterface",
    "VirtualizationType",
]
```
## RecommendationPreferenceNameType

```python
# RecommendationPreferenceNameType usage example

from types_aiobotocore_compute_optimizer.literals import RecommendationPreferenceNameType

def get_value() -> RecommendationPreferenceNameType:
    return "EnhancedInfrastructureMetrics"
```

```python
# RecommendationPreferenceNameType definition

RecommendationPreferenceNameType = Literal[
    "EnhancedInfrastructureMetrics",
    "ExternalMetricsPreference",
    "InferredWorkloadTypes",
]
```
## RecommendationSourceTypeType

```python
# RecommendationSourceTypeType usage example

from types_aiobotocore_compute_optimizer.literals import RecommendationSourceTypeType

def get_value() -> RecommendationSourceTypeType:
    return "AutoScalingGroup"
```

```python
# RecommendationSourceTypeType definition

RecommendationSourceTypeType = Literal[
    "AutoScalingGroup",
    "EbsVolume",
    "Ec2Instance",
    "EcsService",
    "LambdaFunction",
]
```
## ResourceTypeType

```python
# ResourceTypeType usage example

from types_aiobotocore_compute_optimizer.literals import ResourceTypeType

def get_value() -> ResourceTypeType:
    return "AutoScalingGroup"
```

```python
# ResourceTypeType definition

ResourceTypeType = Literal[
    "AutoScalingGroup",
    "EbsVolume",
    "Ec2Instance",
    "EcsService",
    "LambdaFunction",
    "NotApplicable",
]
```
## ScopeNameType

```python
# ScopeNameType usage example

from types_aiobotocore_compute_optimizer.literals import ScopeNameType

def get_value() -> ScopeNameType:
    return "AccountId"
```

```python
# ScopeNameType definition

ScopeNameType = Literal[
    "AccountId",
    "Organization",
    "ResourceArn",
]
```
## StatusType

```python
# StatusType usage example

from types_aiobotocore_compute_optimizer.literals import StatusType

def get_value() -> StatusType:
    return "Active"
```

```python
# StatusType definition

StatusType = Literal[
    "Active",
    "Failed",
    "Inactive",
    "Pending",
]
```
## ComputeOptimizerServiceName

```python
# ComputeOptimizerServiceName usage example

from types_aiobotocore_compute_optimizer.literals import ComputeOptimizerServiceName

def get_value() -> ComputeOptimizerServiceName:
    return "compute-optimizer"
```

```python
# ComputeOptimizerServiceName definition

ComputeOptimizerServiceName = Literal[
    "compute-optimizer",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_compute_optimizer.literals import ServiceName

def get_value() -> ServiceName:
    return "accessanalyzer"
```

```python
# ServiceName definition

ServiceName = Literal[
    "accessanalyzer",
    "account",
    "acm",
    "acm-pca",
    "alexaforbusiness",
    "amp",
    "amplify",
    "amplifybackend",
    "amplifyuibuilder",
    "apigateway",
    "apigatewaymanagementapi",
    "apigatewayv2",
    "appconfig",
    "appconfigdata",
    "appfabric",
    "appflow",
    "appintegrations",
    "application-autoscaling",
    "application-insights",
    "applicationcostprofiler",
    "appmesh",
    "apprunner",
    "appstream",
    "appsync",
    "arc-zonal-shift",
    "athena",
    "auditmanager",
    "autoscaling",
    "autoscaling-plans",
    "backup",
    "backup-gateway",
    "backupstorage",
    "batch",
    "billingconductor",
    "braket",
    "budgets",
    "ce",
    "chime",
    "chime-sdk-identity",
    "chime-sdk-media-pipelines",
    "chime-sdk-meetings",
    "chime-sdk-messaging",
    "chime-sdk-voice",
    "cleanrooms",
    "cloud9",
    "cloudcontrol",
    "clouddirectory",
    "cloudformation",
    "cloudfront",
    "cloudhsm",
    "cloudhsmv2",
    "cloudsearch",
    "cloudsearchdomain",
    "cloudtrail",
    "cloudtrail-data",
    "cloudwatch",
    "codeartifact",
    "codebuild",
    "codecatalyst",
    "codecommit",
    "codedeploy",
    "codeguru-reviewer",
    "codeguru-security",
    "codeguruprofiler",
    "codepipeline",
    "codestar",
    "codestar-connections",
    "codestar-notifications",
    "cognito-identity",
    "cognito-idp",
    "cognito-sync",
    "comprehend",
    "comprehendmedical",
    "compute-optimizer",
    "config",
    "connect",
    "connect-contact-lens",
    "connectcampaigns",
    "connectcases",
    "connectparticipant",
    "controltower",
    "cur",
    "customer-profiles",
    "databrew",
    "dataexchange",
    "datapipeline",
    "datasync",
    "dax",
    "detective",
    "devicefarm",
    "devops-guru",
    "directconnect",
    "discovery",
    "dlm",
    "dms",
    "docdb",
    "docdb-elastic",
    "drs",
    "ds",
    "dynamodb",
    "dynamodbstreams",
    "ebs",
    "ec2",
    "ec2-instance-connect",
    "ecr",
    "ecr-public",
    "ecs",
    "efs",
    "eks",
    "elastic-inference",
    "elasticache",
    "elasticbeanstalk",
    "elastictranscoder",
    "elb",
    "elbv2",
    "emr",
    "emr-containers",
    "emr-serverless",
    "entityresolution",
    "es",
    "events",
    "evidently",
    "finspace",
    "finspace-data",
    "firehose",
    "fis",
    "fms",
    "forecast",
    "forecastquery",
    "frauddetector",
    "fsx",
    "gamelift",
    "gamesparks",
    "glacier",
    "globalaccelerator",
    "glue",
    "grafana",
    "greengrass",
    "greengrassv2",
    "groundstation",
    "guardduty",
    "health",
    "healthlake",
    "honeycode",
    "iam",
    "identitystore",
    "imagebuilder",
    "importexport",
    "inspector",
    "inspector2",
    "internetmonitor",
    "iot",
    "iot-data",
    "iot-jobs-data",
    "iot-roborunner",
    "iot1click-devices",
    "iot1click-projects",
    "iotanalytics",
    "iotdeviceadvisor",
    "iotevents",
    "iotevents-data",
    "iotfleethub",
    "iotfleetwise",
    "iotsecuretunneling",
    "iotsitewise",
    "iotthingsgraph",
    "iottwinmaker",
    "iotwireless",
    "ivs",
    "ivs-realtime",
    "ivschat",
    "kafka",
    "kafkaconnect",
    "kendra",
    "kendra-ranking",
    "keyspaces",
    "kinesis",
    "kinesis-video-archived-media",
    "kinesis-video-media",
    "kinesis-video-signaling",
    "kinesis-video-webrtc-storage",
    "kinesisanalytics",
    "kinesisanalyticsv2",
    "kinesisvideo",
    "kms",
    "lakeformation",
    "lambda",
    "lex-models",
    "lex-runtime",
    "lexv2-models",
    "lexv2-runtime",
    "license-manager",
    "license-manager-linux-subscriptions",
    "license-manager-user-subscriptions",
    "lightsail",
    "location",
    "logs",
    "lookoutequipment",
    "lookoutmetrics",
    "lookoutvision",
    "m2",
    "machinelearning",
    "macie",
    "macie2",
    "managedblockchain",
    "managedblockchain-query",
    "marketplace-catalog",
    "marketplace-entitlement",
    "marketplacecommerceanalytics",
    "mediaconnect",
    "mediaconvert",
    "medialive",
    "mediapackage",
    "mediapackage-vod",
    "mediapackagev2",
    "mediastore",
    "mediastore-data",
    "mediatailor",
    "medical-imaging",
    "memorydb",
    "meteringmarketplace",
    "mgh",
    "mgn",
    "migration-hub-refactor-spaces",
    "migrationhub-config",
    "migrationhuborchestrator",
    "migrationhubstrategy",
    "mobile",
    "mq",
    "mturk",
    "mwaa",
    "neptune",
    "network-firewall",
    "networkmanager",
    "nimble",
    "oam",
    "omics",
    "opensearch",
    "opensearchserverless",
    "opsworks",
    "opsworkscm",
    "organizations",
    "osis",
    "outposts",
    "panorama",
    "payment-cryptography",
    "payment-cryptography-data",
    "personalize",
    "personalize-events",
    "personalize-runtime",
    "pi",
    "pinpoint",
    "pinpoint-email",
    "pinpoint-sms-voice",
    "pinpoint-sms-voice-v2",
    "pipes",
    "polly",
    "pricing",
    "privatenetworks",
    "proton",
    "qldb",
    "qldb-session",
    "quicksight",
    "ram",
    "rbin",
    "rds",
    "rds-data",
    "redshift",
    "redshift-data",
    "redshift-serverless",
    "rekognition",
    "resiliencehub",
    "resource-explorer-2",
    "resource-groups",
    "resourcegroupstaggingapi",
    "robomaker",
    "rolesanywhere",
    "route53",
    "route53-recovery-cluster",
    "route53-recovery-control-config",
    "route53-recovery-readiness",
    "route53domains",
    "route53resolver",
    "rum",
    "s3",
    "s3control",
    "s3outposts",
    "sagemaker",
    "sagemaker-a2i-runtime",
    "sagemaker-edge",
    "sagemaker-featurestore-runtime",
    "sagemaker-geospatial",
    "sagemaker-metrics",
    "sagemaker-runtime",
    "savingsplans",
    "scheduler",
    "schemas",
    "sdb",
    "secretsmanager",
    "securityhub",
    "securitylake",
    "serverlessrepo",
    "service-quotas",
    "servicecatalog",
    "servicecatalog-appregistry",
    "servicediscovery",
    "ses",
    "sesv2",
    "shield",
    "signer",
    "simspaceweaver",
    "sms",
    "sms-voice",
    "snow-device-management",
    "snowball",
    "sns",
    "sqs",
    "ssm",
    "ssm-contacts",
    "ssm-incidents",
    "ssm-sap",
    "sso",
    "sso-admin",
    "sso-oidc",
    "stepfunctions",
    "storagegateway",
    "sts",
    "support",
    "support-app",
    "swf",
    "synthetics",
    "textract",
    "timestream-query",
    "timestream-write",
    "tnb",
    "transcribe",
    "transfer",
    "translate",
    "verifiedpermissions",
    "voice-id",
    "vpc-lattice",
    "waf",
    "waf-regional",
    "wafv2",
    "wellarchitected",
    "wisdom",
    "workdocs",
    "worklink",
    "workmail",
    "workmailmessageflow",
    "workspaces",
    "workspaces-web",
    "xray",
]
```
## ResourceServiceName

```python
# ResourceServiceName usage example

from types_aiobotocore_compute_optimizer.literals import ResourceServiceName

def get_value() -> ResourceServiceName:
    return "cloudformation"
```

```python
# ResourceServiceName definition

ResourceServiceName = Literal[
    "cloudformation",
    "cloudwatch",
    "dynamodb",
    "ec2",
    "glacier",
    "iam",
    "opsworks",
    "s3",
    "sns",
    "sqs",
]
```
## PaginatorName

```python
# PaginatorName usage example

from types_aiobotocore_compute_optimizer.literals import PaginatorName

def get_value() -> PaginatorName:
    return "describe_recommendation_export_jobs"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "describe_recommendation_export_jobs",
    "get_enrollment_statuses_for_organization",
    "get_lambda_function_recommendations",
    "get_recommendation_preferences",
    "get_recommendation_summaries",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_compute_optimizer.literals import RegionName

def get_value() -> RegionName:
    return "af-south-1"
```

```python
# RegionName definition

RegionName = Literal[
    "af-south-1",
    "ap-east-1",
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-northeast-3",
    "ap-south-1",
    "ap-southeast-1",
    "ap-southeast-2",
    "ca-central-1",
    "eu-central-1",
    "eu-north-1",
    "eu-south-1",
    "eu-west-1",
    "eu-west-2",
    "eu-west-3",
    "me-south-1",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
