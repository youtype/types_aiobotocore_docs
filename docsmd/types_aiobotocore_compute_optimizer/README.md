# ComputeOptimizer module

> [Index](../README.md) > ComputeOptimizer


!!! note ""

    Auto-generated documentation for [ComputeOptimizer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
    type annotations stubs module [types-aiobotocore-compute-optimizer](https://pypi.org/project/types-aiobotocore-compute-optimizer/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `ComputeOptimizer` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[compute-optimizer]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[compute-optimizer]'


# standalone installation
python -m pip install types-aiobotocore-compute-optimizer
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-compute-optimizer
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ComputeOptimizerClient

Type annotations and code completion for  `#!python session.create_client("compute-optimizer")` as [ComputeOptimizerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_compute_optimizer.client import ComputeOptimizerClient


session = get_session()
async with session.create_client("compute-optimizer") as client:
    client: ComputeOptimizerClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_compute_optimizer.literals import CpuVendorArchitectureType

def get_value() -> CpuVendorArchitectureType:
    return "AWS_ARM64"
```

- [CpuVendorArchitectureType](./literals.md#cpuvendorarchitecturetype)
- [CurrencyType](./literals.md#currencytype)
- [CurrentPerformanceRiskType](./literals.md#currentperformancerisktype)
- [EBSFilterNameType](./literals.md#ebsfilternametype)
- [EBSFindingType](./literals.md#ebsfindingtype)
- [EBSMetricNameType](./literals.md#ebsmetricnametype)
- [EnhancedInfrastructureMetricsType](./literals.md#enhancedinfrastructuremetricstype)
- [EnrollmentFilterNameType](./literals.md#enrollmentfilternametype)
- [ExportableAutoScalingGroupFieldType](./literals.md#exportableautoscalinggroupfieldtype)
- [ExportableInstanceFieldType](./literals.md#exportableinstancefieldtype)
- [ExportableLambdaFunctionFieldType](./literals.md#exportablelambdafunctionfieldtype)
- [ExportableVolumeFieldType](./literals.md#exportablevolumefieldtype)
- [FileFormatType](./literals.md#fileformattype)
- [FilterNameType](./literals.md#filternametype)
- [FindingReasonCodeType](./literals.md#findingreasoncodetype)
- [FindingType](./literals.md#findingtype)
- [InferredWorkloadTypeType](./literals.md#inferredworkloadtypetype)
- [InferredWorkloadTypesPreferenceType](./literals.md#inferredworkloadtypespreferencetype)
- [InstanceRecommendationFindingReasonCodeType](./literals.md#instancerecommendationfindingreasoncodetype)
- [JobFilterNameType](./literals.md#jobfilternametype)
- [JobStatusType](./literals.md#jobstatustype)
- [LambdaFunctionMemoryMetricNameType](./literals.md#lambdafunctionmemorymetricnametype)
- [LambdaFunctionMemoryMetricStatisticType](./literals.md#lambdafunctionmemorymetricstatistictype)
- [LambdaFunctionMetricNameType](./literals.md#lambdafunctionmetricnametype)
- [LambdaFunctionMetricStatisticType](./literals.md#lambdafunctionmetricstatistictype)
- [LambdaFunctionRecommendationFilterNameType](./literals.md#lambdafunctionrecommendationfilternametype)
- [LambdaFunctionRecommendationFindingReasonCodeType](./literals.md#lambdafunctionrecommendationfindingreasoncodetype)
- [LambdaFunctionRecommendationFindingType](./literals.md#lambdafunctionrecommendationfindingtype)
- [MetricNameType](./literals.md#metricnametype)
- [MetricStatisticType](./literals.md#metricstatistictype)
- [MigrationEffortType](./literals.md#migrationefforttype)
- [PlatformDifferenceType](./literals.md#platformdifferencetype)
- [RecommendationPreferenceNameType](./literals.md#recommendationpreferencenametype)
- [RecommendationSourceTypeType](./literals.md#recommendationsourcetypetype)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [ScopeNameType](./literals.md#scopenametype)
- [StatusType](./literals.md#statustype)
- [ComputeOptimizerServiceName](./literals.md#computeoptimizerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_compute_optimizer.type_defs import AccountEnrollmentStatusTypeDef

def get_value() -> AccountEnrollmentStatusTypeDef:
    return {
        "accountId": ...,
    }
```

- [AccountEnrollmentStatusTypeDef](./type_defs.md#accountenrollmentstatustypedef)
- [AutoScalingGroupConfigurationTypeDef](./type_defs.md#autoscalinggroupconfigurationtypedef)
- [UtilizationMetricTypeDef](./type_defs.md#utilizationmetrictypedef)
- [EffectiveRecommendationPreferencesTypeDef](./type_defs.md#effectiverecommendationpreferencestypedef)
- [CurrentPerformanceRiskRatingsTypeDef](./type_defs.md#currentperformanceriskratingstypedef)
- [ScopeTypeDef](./type_defs.md#scopetypedef)
- [JobFilterTypeDef](./type_defs.md#jobfiltertypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [EBSFilterTypeDef](./type_defs.md#ebsfiltertypedef)
- [EBSUtilizationMetricTypeDef](./type_defs.md#ebsutilizationmetrictypedef)
- [EnrollmentFilterTypeDef](./type_defs.md#enrollmentfiltertypedef)
- [EstimatedMonthlySavingsTypeDef](./type_defs.md#estimatedmonthlysavingstypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef)
- [S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef)
- [S3DestinationTypeDef](./type_defs.md#s3destinationtypedef)
- [LambdaFunctionRecommendationFilterTypeDef](./type_defs.md#lambdafunctionrecommendationfiltertypedef)
- [GetRecommendationErrorTypeDef](./type_defs.md#getrecommendationerrortypedef)
- [GetEffectiveRecommendationPreferencesRequestRequestTypeDef](./type_defs.md#geteffectiverecommendationpreferencesrequestrequesttypedef)
- [GetRecommendationSummariesRequestRequestTypeDef](./type_defs.md#getrecommendationsummariesrequestrequesttypedef)
- [RecommendationSourceTypeDef](./type_defs.md#recommendationsourcetypedef)
- [LambdaFunctionMemoryProjectedMetricTypeDef](./type_defs.md#lambdafunctionmemoryprojectedmetrictypedef)
- [LambdaFunctionUtilizationMetricTypeDef](./type_defs.md#lambdafunctionutilizationmetrictypedef)
- [ProjectedMetricTypeDef](./type_defs.md#projectedmetrictypedef)
- [ReasonCodeSummaryTypeDef](./type_defs.md#reasoncodesummarytypedef)
- [UpdateEnrollmentStatusRequestRequestTypeDef](./type_defs.md#updateenrollmentstatusrequestrequesttypedef)
- [VolumeConfigurationTypeDef](./type_defs.md#volumeconfigurationtypedef)
- [DeleteRecommendationPreferencesRequestRequestTypeDef](./type_defs.md#deleterecommendationpreferencesrequestrequesttypedef)
- [GetRecommendationPreferencesRequestRequestTypeDef](./type_defs.md#getrecommendationpreferencesrequestrequesttypedef)
- [PutRecommendationPreferencesRequestRequestTypeDef](./type_defs.md#putrecommendationpreferencesrequestrequesttypedef)
- [RecommendationPreferencesDetailTypeDef](./type_defs.md#recommendationpreferencesdetailtypedef)
- [DescribeRecommendationExportJobsRequestRequestTypeDef](./type_defs.md#describerecommendationexportjobsrequestrequesttypedef)
- [GetEffectiveRecommendationPreferencesResponseTypeDef](./type_defs.md#geteffectiverecommendationpreferencesresponsetypedef)
- [GetEnrollmentStatusResponseTypeDef](./type_defs.md#getenrollmentstatusresponsetypedef)
- [GetEnrollmentStatusesForOrganizationResponseTypeDef](./type_defs.md#getenrollmentstatusesfororganizationresponsetypedef)
- [UpdateEnrollmentStatusResponseTypeDef](./type_defs.md#updateenrollmentstatusresponsetypedef)
- [GetEBSVolumeRecommendationsRequestRequestTypeDef](./type_defs.md#getebsvolumerecommendationsrequestrequesttypedef)
- [GetEnrollmentStatusesForOrganizationRequestRequestTypeDef](./type_defs.md#getenrollmentstatusesfororganizationrequestrequesttypedef)
- [SavingsOpportunityTypeDef](./type_defs.md#savingsopportunitytypedef)
- [GetAutoScalingGroupRecommendationsRequestRequestTypeDef](./type_defs.md#getautoscalinggrouprecommendationsrequestrequesttypedef)
- [GetEC2InstanceRecommendationsRequestRequestTypeDef](./type_defs.md#getec2instancerecommendationsrequestrequesttypedef)
- [GetEC2RecommendationProjectedMetricsRequestRequestTypeDef](./type_defs.md#getec2recommendationprojectedmetricsrequestrequesttypedef)
- [ExportAutoScalingGroupRecommendationsRequestRequestTypeDef](./type_defs.md#exportautoscalinggrouprecommendationsrequestrequesttypedef)
- [ExportEBSVolumeRecommendationsRequestRequestTypeDef](./type_defs.md#exportebsvolumerecommendationsrequestrequesttypedef)
- [ExportEC2InstanceRecommendationsRequestRequestTypeDef](./type_defs.md#exportec2instancerecommendationsrequestrequesttypedef)
- [ExportAutoScalingGroupRecommendationsResponseTypeDef](./type_defs.md#exportautoscalinggrouprecommendationsresponsetypedef)
- [ExportDestinationTypeDef](./type_defs.md#exportdestinationtypedef)
- [ExportEBSVolumeRecommendationsResponseTypeDef](./type_defs.md#exportebsvolumerecommendationsresponsetypedef)
- [ExportEC2InstanceRecommendationsResponseTypeDef](./type_defs.md#exportec2instancerecommendationsresponsetypedef)
- [ExportLambdaFunctionRecommendationsResponseTypeDef](./type_defs.md#exportlambdafunctionrecommendationsresponsetypedef)
- [ExportLambdaFunctionRecommendationsRequestRequestTypeDef](./type_defs.md#exportlambdafunctionrecommendationsrequestrequesttypedef)
- [GetLambdaFunctionRecommendationsRequestRequestTypeDef](./type_defs.md#getlambdafunctionrecommendationsrequestrequesttypedef)
- [RecommendedOptionProjectedMetricTypeDef](./type_defs.md#recommendedoptionprojectedmetrictypedef)
- [SummaryTypeDef](./type_defs.md#summarytypedef)
- [GetRecommendationPreferencesResponseTypeDef](./type_defs.md#getrecommendationpreferencesresponsetypedef)
- [AutoScalingGroupRecommendationOptionTypeDef](./type_defs.md#autoscalinggrouprecommendationoptiontypedef)
- [InstanceRecommendationOptionTypeDef](./type_defs.md#instancerecommendationoptiontypedef)
- [LambdaFunctionMemoryRecommendationOptionTypeDef](./type_defs.md#lambdafunctionmemoryrecommendationoptiontypedef)
- [VolumeRecommendationOptionTypeDef](./type_defs.md#volumerecommendationoptiontypedef)
- [RecommendationExportJobTypeDef](./type_defs.md#recommendationexportjobtypedef)
- [GetEC2RecommendationProjectedMetricsResponseTypeDef](./type_defs.md#getec2recommendationprojectedmetricsresponsetypedef)
- [RecommendationSummaryTypeDef](./type_defs.md#recommendationsummarytypedef)
- [AutoScalingGroupRecommendationTypeDef](./type_defs.md#autoscalinggrouprecommendationtypedef)
- [InstanceRecommendationTypeDef](./type_defs.md#instancerecommendationtypedef)
- [LambdaFunctionRecommendationTypeDef](./type_defs.md#lambdafunctionrecommendationtypedef)
- [VolumeRecommendationTypeDef](./type_defs.md#volumerecommendationtypedef)
- [DescribeRecommendationExportJobsResponseTypeDef](./type_defs.md#describerecommendationexportjobsresponsetypedef)
- [GetRecommendationSummariesResponseTypeDef](./type_defs.md#getrecommendationsummariesresponsetypedef)
- [GetAutoScalingGroupRecommendationsResponseTypeDef](./type_defs.md#getautoscalinggrouprecommendationsresponsetypedef)
- [GetEC2InstanceRecommendationsResponseTypeDef](./type_defs.md#getec2instancerecommendationsresponsetypedef)
- [GetLambdaFunctionRecommendationsResponseTypeDef](./type_defs.md#getlambdafunctionrecommendationsresponsetypedef)
- [GetEBSVolumeRecommendationsResponseTypeDef](./type_defs.md#getebsvolumerecommendationsresponsetypedef)

