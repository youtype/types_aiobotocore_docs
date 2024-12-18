# CostOptimizationHub module

> [Index](../README.md) > CostOptimizationHub


!!! note ""

    Auto-generated documentation for [CostOptimizationHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#costoptimizationhub)
    type annotations stubs module [types-aiobotocore-cost-optimization-hub](https://pypi.org/project/types-aiobotocore-cost-optimization-hub/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `CostOptimizationHub` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `CostOptimizationHub` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[cost-optimization-hub]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[cost-optimization-hub]'

# standalone installation
python -m pip install types-aiobotocore-cost-optimization-hub
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-cost-optimization-hub
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CostOptimizationHubClient

Type annotations and code completion for  `#!python session.create_client("cost-optimization-hub")` as [CostOptimizationHubClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client)

```python
# CostOptimizationHubClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_cost_optimization_hub.client import CostOptimizationHubClient


session = get_session()
async with session.create_client("cost-optimization-hub") as client:
    client: CostOptimizationHubClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("cost-optimization-hub").get_paginator("...")`.

```python
# ListEnrollmentStatusesPaginator usage example

from types_aiobotocore_cost_optimization_hub.paginator import ListEnrollmentStatusesPaginator

def get_list_enrollment_statuses_paginator() -> ListEnrollmentStatusesPaginator:
    return client.get_paginator("list_enrollment_statuses"))
```

- [ListEnrollmentStatusesPaginator](./paginators.md#listenrollmentstatusespaginator)
- [ListRecommendationSummariesPaginator](./paginators.md#listrecommendationsummariespaginator)
- [ListRecommendationsPaginator](./paginators.md#listrecommendationspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActionTypeType usage example

from types_aiobotocore_cost_optimization_hub.literals import ActionTypeType

def get_value() -> ActionTypeType:
    return "Delete"
```

- [ActionTypeType](./literals.md#actiontypetype)
- [EnrollmentStatusType](./literals.md#enrollmentstatustype)
- [ImplementationEffortType](./literals.md#implementationefforttype)
- [ListEnrollmentStatusesPaginatorName](./literals.md#listenrollmentstatusespaginatorname)
- [ListRecommendationSummariesPaginatorName](./literals.md#listrecommendationsummariespaginatorname)
- [ListRecommendationsPaginatorName](./literals.md#listrecommendationspaginatorname)
- [MemberAccountDiscountVisibilityType](./literals.md#memberaccountdiscountvisibilitytype)
- [OrderType](./literals.md#ordertype)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [SavingsEstimationModeType](./literals.md#savingsestimationmodetype)
- [SourceType](./literals.md#sourcetype)
- [SummaryMetricsType](./literals.md#summarymetricstype)
- [CostOptimizationHubServiceName](./literals.md#costoptimizationhubservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccountEnrollmentStatusTypeDef](./type_defs.md#accountenrollmentstatustypedef)
- [BlockStoragePerformanceConfigurationTypeDef](./type_defs.md#blockstorageperformanceconfigurationtypedef)
- [ComputeConfigurationTypeDef](./type_defs.md#computeconfigurationtypedef)
- [ComputeSavingsPlansConfigurationTypeDef](./type_defs.md#computesavingsplansconfigurationtypedef)
- [DbInstanceConfigurationTypeDef](./type_defs.md#dbinstanceconfigurationtypedef)
- [StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef)
- [InstanceConfigurationTypeDef](./type_defs.md#instanceconfigurationtypedef)
- [Ec2InstanceSavingsPlansConfigurationTypeDef](./type_defs.md#ec2instancesavingsplansconfigurationtypedef)
- [Ec2ReservedInstancesConfigurationTypeDef](./type_defs.md#ec2reservedinstancesconfigurationtypedef)
- [ElastiCacheReservedInstancesConfigurationTypeDef](./type_defs.md#elasticachereservedinstancesconfigurationtypedef)
- [EstimatedDiscountsTypeDef](./type_defs.md#estimateddiscountstypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetRecommendationRequestRequestTypeDef](./type_defs.md#getrecommendationrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListEnrollmentStatusesRequestRequestTypeDef](./type_defs.md#listenrollmentstatusesrequestrequesttypedef)
- [RecommendationSummaryTypeDef](./type_defs.md#recommendationsummarytypedef)
- [SummaryMetricsResultTypeDef](./type_defs.md#summarymetricsresulttypedef)
- [OrderByTypeDef](./type_defs.md#orderbytypedef)
- [OpenSearchReservedInstancesConfigurationTypeDef](./type_defs.md#opensearchreservedinstancesconfigurationtypedef)
- [RdsDbInstanceStorageConfigurationTypeDef](./type_defs.md#rdsdbinstancestorageconfigurationtypedef)
- [RdsReservedInstancesConfigurationTypeDef](./type_defs.md#rdsreservedinstancesconfigurationtypedef)
- [RedshiftReservedInstancesConfigurationTypeDef](./type_defs.md#redshiftreservedinstancesconfigurationtypedef)
- [ReservedInstancesPricingTypeDef](./type_defs.md#reservedinstancespricingtypedef)
- [UsageTypeDef](./type_defs.md#usagetypedef)
- [SageMakerSavingsPlansConfigurationTypeDef](./type_defs.md#sagemakersavingsplansconfigurationtypedef)
- [SavingsPlansPricingTypeDef](./type_defs.md#savingsplanspricingtypedef)
- [UpdateEnrollmentStatusRequestRequestTypeDef](./type_defs.md#updateenrollmentstatusrequestrequesttypedef)
- [UpdatePreferencesRequestRequestTypeDef](./type_defs.md#updatepreferencesrequestrequesttypedef)
- [EcsServiceConfigurationTypeDef](./type_defs.md#ecsserviceconfigurationtypedef)
- [LambdaFunctionConfigurationTypeDef](./type_defs.md#lambdafunctionconfigurationtypedef)
- [RdsDbInstanceConfigurationTypeDef](./type_defs.md#rdsdbinstanceconfigurationtypedef)
- [EbsVolumeConfigurationTypeDef](./type_defs.md#ebsvolumeconfigurationtypedef)
- [Ec2AutoScalingGroupConfigurationTypeDef](./type_defs.md#ec2autoscalinggroupconfigurationtypedef)
- [Ec2InstanceConfigurationTypeDef](./type_defs.md#ec2instanceconfigurationtypedef)
- [ResourcePricingTypeDef](./type_defs.md#resourcepricingtypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [RecommendationTypeDef](./type_defs.md#recommendationtypedef)
- [GetPreferencesResponseTypeDef](./type_defs.md#getpreferencesresponsetypedef)
- [ListEnrollmentStatusesResponseTypeDef](./type_defs.md#listenrollmentstatusesresponsetypedef)
- [UpdateEnrollmentStatusResponseTypeDef](./type_defs.md#updateenrollmentstatusresponsetypedef)
- [UpdatePreferencesResponseTypeDef](./type_defs.md#updatepreferencesresponsetypedef)
- [ListEnrollmentStatusesRequestListEnrollmentStatusesPaginateTypeDef](./type_defs.md#listenrollmentstatusesrequestlistenrollmentstatusespaginatetypedef)
- [ListRecommendationSummariesResponseTypeDef](./type_defs.md#listrecommendationsummariesresponsetypedef)
- [ReservedInstancesCostCalculationTypeDef](./type_defs.md#reservedinstancescostcalculationtypedef)
- [SavingsPlansCostCalculationTypeDef](./type_defs.md#savingsplanscostcalculationtypedef)
- [ResourceCostCalculationTypeDef](./type_defs.md#resourcecostcalculationtypedef)
- [ListRecommendationSummariesRequestListRecommendationSummariesPaginateTypeDef](./type_defs.md#listrecommendationsummariesrequestlistrecommendationsummariespaginatetypedef)
- [ListRecommendationSummariesRequestRequestTypeDef](./type_defs.md#listrecommendationsummariesrequestrequesttypedef)
- [ListRecommendationsRequestListRecommendationsPaginateTypeDef](./type_defs.md#listrecommendationsrequestlistrecommendationspaginatetypedef)
- [ListRecommendationsRequestRequestTypeDef](./type_defs.md#listrecommendationsrequestrequesttypedef)
- [ListRecommendationsResponseTypeDef](./type_defs.md#listrecommendationsresponsetypedef)
- [Ec2ReservedInstancesTypeDef](./type_defs.md#ec2reservedinstancestypedef)
- [ElastiCacheReservedInstancesTypeDef](./type_defs.md#elasticachereservedinstancestypedef)
- [OpenSearchReservedInstancesTypeDef](./type_defs.md#opensearchreservedinstancestypedef)
- [RdsReservedInstancesTypeDef](./type_defs.md#rdsreservedinstancestypedef)
- [RedshiftReservedInstancesTypeDef](./type_defs.md#redshiftreservedinstancestypedef)
- [ComputeSavingsPlansTypeDef](./type_defs.md#computesavingsplanstypedef)
- [Ec2InstanceSavingsPlansTypeDef](./type_defs.md#ec2instancesavingsplanstypedef)
- [SageMakerSavingsPlansTypeDef](./type_defs.md#sagemakersavingsplanstypedef)
- [EbsVolumeTypeDef](./type_defs.md#ebsvolumetypedef)
- [Ec2AutoScalingGroupTypeDef](./type_defs.md#ec2autoscalinggrouptypedef)
- [Ec2InstanceTypeDef](./type_defs.md#ec2instancetypedef)
- [EcsServiceTypeDef](./type_defs.md#ecsservicetypedef)
- [LambdaFunctionTypeDef](./type_defs.md#lambdafunctiontypedef)
- [RdsDbInstanceStorageTypeDef](./type_defs.md#rdsdbinstancestoragetypedef)
- [RdsDbInstanceTypeDef](./type_defs.md#rdsdbinstancetypedef)
- [ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef)
- [GetRecommendationResponseTypeDef](./type_defs.md#getrecommendationresponsetypedef)

