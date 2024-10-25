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

```python
# ComputeOptimizerClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_compute_optimizer.client import ComputeOptimizerClient


session = get_session()
async with session.create_client("compute-optimizer") as client:
    client: ComputeOptimizerClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("compute-optimizer").get_paginator("...")`.

```python
# DescribeRecommendationExportJobsPaginator usage example

from types_aiobotocore_compute_optimizer.paginator import DescribeRecommendationExportJobsPaginator

def get_describe_recommendation_export_jobs_paginator() -> DescribeRecommendationExportJobsPaginator:
    return client.get_paginator("describe_recommendation_export_jobs"))
```

- [DescribeRecommendationExportJobsPaginator](./paginators.md#describerecommendationexportjobspaginator)
- [GetEnrollmentStatusesForOrganizationPaginator](./paginators.md#getenrollmentstatusesfororganizationpaginator)
- [GetLambdaFunctionRecommendationsPaginator](./paginators.md#getlambdafunctionrecommendationspaginator)
- [GetRecommendationPreferencesPaginator](./paginators.md#getrecommendationpreferencespaginator)
- [GetRecommendationSummariesPaginator](./paginators.md#getrecommendationsummariespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AutoScalingConfigurationType usage example

from types_aiobotocore_compute_optimizer.literals import AutoScalingConfigurationType

def get_value() -> AutoScalingConfigurationType:
    return "TargetTrackingScalingCpu"
```

- [AutoScalingConfigurationType](./literals.md#autoscalingconfigurationtype)
- [CpuVendorArchitectureType](./literals.md#cpuvendorarchitecturetype)
- [CurrencyType](./literals.md#currencytype)
- [CurrentPerformanceRiskType](./literals.md#currentperformancerisktype)
- [CustomizableMetricHeadroomType](./literals.md#customizablemetricheadroomtype)
- [CustomizableMetricNameType](./literals.md#customizablemetricnametype)
- [CustomizableMetricThresholdType](./literals.md#customizablemetricthresholdtype)
- [DescribeRecommendationExportJobsPaginatorName](./literals.md#describerecommendationexportjobspaginatorname)
- [EBSFilterNameType](./literals.md#ebsfilternametype)
- [EBSFindingType](./literals.md#ebsfindingtype)
- [EBSMetricNameType](./literals.md#ebsmetricnametype)
- [EBSSavingsEstimationModeSourceType](./literals.md#ebssavingsestimationmodesourcetype)
- [ECSSavingsEstimationModeSourceType](./literals.md#ecssavingsestimationmodesourcetype)
- [ECSServiceLaunchTypeType](./literals.md#ecsservicelaunchtypetype)
- [ECSServiceMetricNameType](./literals.md#ecsservicemetricnametype)
- [ECSServiceMetricStatisticType](./literals.md#ecsservicemetricstatistictype)
- [ECSServiceRecommendationFilterNameType](./literals.md#ecsservicerecommendationfilternametype)
- [ECSServiceRecommendationFindingReasonCodeType](./literals.md#ecsservicerecommendationfindingreasoncodetype)
- [ECSServiceRecommendationFindingType](./literals.md#ecsservicerecommendationfindingtype)
- [EnhancedInfrastructureMetricsType](./literals.md#enhancedinfrastructuremetricstype)
- [EnrollmentFilterNameType](./literals.md#enrollmentfilternametype)
- [ExportableAutoScalingGroupFieldType](./literals.md#exportableautoscalinggroupfieldtype)
- [ExportableECSServiceFieldType](./literals.md#exportableecsservicefieldtype)
- [ExportableInstanceFieldType](./literals.md#exportableinstancefieldtype)
- [ExportableLambdaFunctionFieldType](./literals.md#exportablelambdafunctionfieldtype)
- [ExportableLicenseFieldType](./literals.md#exportablelicensefieldtype)
- [ExportableRDSDBFieldType](./literals.md#exportablerdsdbfieldtype)
- [ExportableVolumeFieldType](./literals.md#exportablevolumefieldtype)
- [ExternalMetricStatusCodeType](./literals.md#externalmetricstatuscodetype)
- [ExternalMetricsSourceType](./literals.md#externalmetricssourcetype)
- [FileFormatType](./literals.md#fileformattype)
- [FilterNameType](./literals.md#filternametype)
- [FindingReasonCodeType](./literals.md#findingreasoncodetype)
- [FindingType](./literals.md#findingtype)
- [GetEnrollmentStatusesForOrganizationPaginatorName](./literals.md#getenrollmentstatusesfororganizationpaginatorname)
- [GetLambdaFunctionRecommendationsPaginatorName](./literals.md#getlambdafunctionrecommendationspaginatorname)
- [GetRecommendationPreferencesPaginatorName](./literals.md#getrecommendationpreferencespaginatorname)
- [GetRecommendationSummariesPaginatorName](./literals.md#getrecommendationsummariespaginatorname)
- [IdleType](./literals.md#idletype)
- [InferredWorkloadTypeType](./literals.md#inferredworkloadtypetype)
- [InferredWorkloadTypesPreferenceType](./literals.md#inferredworkloadtypespreferencetype)
- [InstanceIdleType](./literals.md#instanceidletype)
- [InstanceRecommendationFindingReasonCodeType](./literals.md#instancerecommendationfindingreasoncodetype)
- [InstanceSavingsEstimationModeSourceType](./literals.md#instancesavingsestimationmodesourcetype)
- [InstanceStateType](./literals.md#instancestatetype)
- [JobFilterNameType](./literals.md#jobfilternametype)
- [JobStatusType](./literals.md#jobstatustype)
- [LambdaFunctionMemoryMetricNameType](./literals.md#lambdafunctionmemorymetricnametype)
- [LambdaFunctionMemoryMetricStatisticType](./literals.md#lambdafunctionmemorymetricstatistictype)
- [LambdaFunctionMetricNameType](./literals.md#lambdafunctionmetricnametype)
- [LambdaFunctionMetricStatisticType](./literals.md#lambdafunctionmetricstatistictype)
- [LambdaFunctionRecommendationFilterNameType](./literals.md#lambdafunctionrecommendationfilternametype)
- [LambdaFunctionRecommendationFindingReasonCodeType](./literals.md#lambdafunctionrecommendationfindingreasoncodetype)
- [LambdaFunctionRecommendationFindingType](./literals.md#lambdafunctionrecommendationfindingtype)
- [LambdaSavingsEstimationModeSourceType](./literals.md#lambdasavingsestimationmodesourcetype)
- [LicenseEditionType](./literals.md#licenseeditiontype)
- [LicenseFindingReasonCodeType](./literals.md#licensefindingreasoncodetype)
- [LicenseFindingType](./literals.md#licensefindingtype)
- [LicenseModelType](./literals.md#licensemodeltype)
- [LicenseNameType](./literals.md#licensenametype)
- [LicenseRecommendationFilterNameType](./literals.md#licenserecommendationfilternametype)
- [LookBackPeriodPreferenceType](./literals.md#lookbackperiodpreferencetype)
- [MetricNameType](./literals.md#metricnametype)
- [MetricSourceProviderType](./literals.md#metricsourceprovidertype)
- [MetricStatisticType](./literals.md#metricstatistictype)
- [MigrationEffortType](./literals.md#migrationefforttype)
- [PlatformDifferenceType](./literals.md#platformdifferencetype)
- [PreferredResourceNameType](./literals.md#preferredresourcenametype)
- [RDSDBMetricNameType](./literals.md#rdsdbmetricnametype)
- [RDSDBMetricStatisticType](./literals.md#rdsdbmetricstatistictype)
- [RDSDBRecommendationFilterNameType](./literals.md#rdsdbrecommendationfilternametype)
- [RDSInstanceFindingReasonCodeType](./literals.md#rdsinstancefindingreasoncodetype)
- [RDSInstanceFindingType](./literals.md#rdsinstancefindingtype)
- [RDSSavingsEstimationModeSourceType](./literals.md#rdssavingsestimationmodesourcetype)
- [RDSStorageFindingReasonCodeType](./literals.md#rdsstoragefindingreasoncodetype)
- [RDSStorageFindingType](./literals.md#rdsstoragefindingtype)
- [RecommendationPreferenceNameType](./literals.md#recommendationpreferencenametype)
- [RecommendationSourceTypeType](./literals.md#recommendationsourcetypetype)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [SavingsEstimationModeType](./literals.md#savingsestimationmodetype)
- [ScopeNameType](./literals.md#scopenametype)
- [StatusType](./literals.md#statustype)
- [ComputeOptimizerServiceName](./literals.md#computeoptimizerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccountEnrollmentStatusTypeDef](./type_defs.md#accountenrollmentstatustypedef)
- [AutoScalingGroupConfigurationTypeDef](./type_defs.md#autoscalinggroupconfigurationtypedef)
- [AutoScalingGroupEstimatedMonthlySavingsTypeDef](./type_defs.md#autoscalinggroupestimatedmonthlysavingstypedef)
- [UtilizationMetricTypeDef](./type_defs.md#utilizationmetrictypedef)
- [MemorySizeConfigurationTypeDef](./type_defs.md#memorysizeconfigurationtypedef)
- [CurrentPerformanceRiskRatingsTypeDef](./type_defs.md#currentperformanceriskratingstypedef)
- [CustomizableMetricParametersTypeDef](./type_defs.md#customizablemetricparameterstypedef)
- [DBStorageConfigurationTypeDef](./type_defs.md#dbstorageconfigurationtypedef)
- [ScopeTypeDef](./type_defs.md#scopetypedef)
- [JobFilterTypeDef](./type_defs.md#jobfiltertypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [EBSSavingsEstimationModeTypeDef](./type_defs.md#ebssavingsestimationmodetypedef)
- [EBSEstimatedMonthlySavingsTypeDef](./type_defs.md#ebsestimatedmonthlysavingstypedef)
- [EBSFilterTypeDef](./type_defs.md#ebsfiltertypedef)
- [EBSUtilizationMetricTypeDef](./type_defs.md#ebsutilizationmetrictypedef)
- [ECSSavingsEstimationModeTypeDef](./type_defs.md#ecssavingsestimationmodetypedef)
- [ECSEstimatedMonthlySavingsTypeDef](./type_defs.md#ecsestimatedmonthlysavingstypedef)
- [ECSServiceProjectedMetricTypeDef](./type_defs.md#ecsserviceprojectedmetrictypedef)
- [ECSServiceProjectedUtilizationMetricTypeDef](./type_defs.md#ecsserviceprojectedutilizationmetrictypedef)
- [ECSServiceRecommendationFilterTypeDef](./type_defs.md#ecsservicerecommendationfiltertypedef)
- [ECSServiceUtilizationMetricTypeDef](./type_defs.md#ecsserviceutilizationmetrictypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [EffectivePreferredResourceTypeDef](./type_defs.md#effectivepreferredresourcetypedef)
- [ExternalMetricsPreferenceTypeDef](./type_defs.md#externalmetricspreferencetypedef)
- [InstanceSavingsEstimationModeTypeDef](./type_defs.md#instancesavingsestimationmodetypedef)
- [EnrollmentFilterTypeDef](./type_defs.md#enrollmentfiltertypedef)
- [EstimatedMonthlySavingsTypeDef](./type_defs.md#estimatedmonthlysavingstypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef)
- [S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef)
- [S3DestinationTypeDef](./type_defs.md#s3destinationtypedef)
- [LambdaFunctionRecommendationFilterTypeDef](./type_defs.md#lambdafunctionrecommendationfiltertypedef)
- [LicenseRecommendationFilterTypeDef](./type_defs.md#licenserecommendationfiltertypedef)
- [RDSDBRecommendationFilterTypeDef](./type_defs.md#rdsdbrecommendationfiltertypedef)
- [ExternalMetricStatusTypeDef](./type_defs.md#externalmetricstatustypedef)
- [GetRecommendationErrorTypeDef](./type_defs.md#getrecommendationerrortypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [GetEffectiveRecommendationPreferencesRequestRequestTypeDef](./type_defs.md#geteffectiverecommendationpreferencesrequestrequesttypedef)
- [GetRecommendationSummariesRequestRequestTypeDef](./type_defs.md#getrecommendationsummariesrequestrequesttypedef)
- [GpuTypeDef](./type_defs.md#gputypedef)
- [InstanceEstimatedMonthlySavingsTypeDef](./type_defs.md#instanceestimatedmonthlysavingstypedef)
- [RecommendationSourceTypeDef](./type_defs.md#recommendationsourcetypedef)
- [LambdaSavingsEstimationModeTypeDef](./type_defs.md#lambdasavingsestimationmodetypedef)
- [LambdaEstimatedMonthlySavingsTypeDef](./type_defs.md#lambdaestimatedmonthlysavingstypedef)
- [LambdaFunctionMemoryProjectedMetricTypeDef](./type_defs.md#lambdafunctionmemoryprojectedmetrictypedef)
- [LambdaFunctionUtilizationMetricTypeDef](./type_defs.md#lambdafunctionutilizationmetrictypedef)
- [MetricSourceTypeDef](./type_defs.md#metricsourcetypedef)
- [PreferredResourceTypeDef](./type_defs.md#preferredresourcetypedef)
- [ProjectedMetricTypeDef](./type_defs.md#projectedmetrictypedef)
- [RDSDBUtilizationMetricTypeDef](./type_defs.md#rdsdbutilizationmetrictypedef)
- [RDSDatabaseProjectedMetricTypeDef](./type_defs.md#rdsdatabaseprojectedmetrictypedef)
- [RDSSavingsEstimationModeTypeDef](./type_defs.md#rdssavingsestimationmodetypedef)
- [RDSInstanceEstimatedMonthlySavingsTypeDef](./type_defs.md#rdsinstanceestimatedmonthlysavingstypedef)
- [RDSStorageEstimatedMonthlySavingsTypeDef](./type_defs.md#rdsstorageestimatedmonthlysavingstypedef)
- [ReasonCodeSummaryTypeDef](./type_defs.md#reasoncodesummarytypedef)
- [UpdateEnrollmentStatusRequestRequestTypeDef](./type_defs.md#updateenrollmentstatusrequestrequesttypedef)
- [VolumeConfigurationTypeDef](./type_defs.md#volumeconfigurationtypedef)
- [AutoScalingGroupSavingsOpportunityAfterDiscountsTypeDef](./type_defs.md#autoscalinggroupsavingsopportunityafterdiscountstypedef)
- [ContainerConfigurationTypeDef](./type_defs.md#containerconfigurationtypedef)
- [ContainerRecommendationTypeDef](./type_defs.md#containerrecommendationtypedef)
- [UtilizationPreferenceTypeDef](./type_defs.md#utilizationpreferencetypedef)
- [DeleteRecommendationPreferencesRequestRequestTypeDef](./type_defs.md#deleterecommendationpreferencesrequestrequesttypedef)
- [GetRecommendationPreferencesRequestRequestTypeDef](./type_defs.md#getrecommendationpreferencesrequestrequesttypedef)
- [DescribeRecommendationExportJobsRequestRequestTypeDef](./type_defs.md#describerecommendationexportjobsrequestrequesttypedef)
- [DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef](./type_defs.md#describerecommendationexportjobsrequestdescriberecommendationexportjobspaginatetypedef)
- [GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef](./type_defs.md#getrecommendationpreferencesrequestgetrecommendationpreferencespaginatetypedef)
- [GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef](./type_defs.md#getrecommendationsummariesrequestgetrecommendationsummariespaginatetypedef)
- [GetEnrollmentStatusResponseTypeDef](./type_defs.md#getenrollmentstatusresponsetypedef)
- [GetEnrollmentStatusesForOrganizationResponseTypeDef](./type_defs.md#getenrollmentstatusesfororganizationresponsetypedef)
- [UpdateEnrollmentStatusResponseTypeDef](./type_defs.md#updateenrollmentstatusresponsetypedef)
- [EBSEffectiveRecommendationPreferencesTypeDef](./type_defs.md#ebseffectiverecommendationpreferencestypedef)
- [EBSSavingsOpportunityAfterDiscountsTypeDef](./type_defs.md#ebssavingsopportunityafterdiscountstypedef)
- [GetEBSVolumeRecommendationsRequestRequestTypeDef](./type_defs.md#getebsvolumerecommendationsrequestrequesttypedef)
- [ECSEffectiveRecommendationPreferencesTypeDef](./type_defs.md#ecseffectiverecommendationpreferencestypedef)
- [ECSSavingsOpportunityAfterDiscountsTypeDef](./type_defs.md#ecssavingsopportunityafterdiscountstypedef)
- [ECSServiceRecommendedOptionProjectedMetricTypeDef](./type_defs.md#ecsservicerecommendedoptionprojectedmetrictypedef)
- [GetECSServiceRecommendationsRequestRequestTypeDef](./type_defs.md#getecsservicerecommendationsrequestrequesttypedef)
- [GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef](./type_defs.md#getenrollmentstatusesfororganizationrequestgetenrollmentstatusesfororganizationpaginatetypedef)
- [GetEnrollmentStatusesForOrganizationRequestRequestTypeDef](./type_defs.md#getenrollmentstatusesfororganizationrequestrequesttypedef)
- [InferredWorkloadSavingTypeDef](./type_defs.md#inferredworkloadsavingtypedef)
- [SavingsOpportunityTypeDef](./type_defs.md#savingsopportunitytypedef)
- [GetAutoScalingGroupRecommendationsRequestRequestTypeDef](./type_defs.md#getautoscalinggrouprecommendationsrequestrequesttypedef)
- [GetEC2InstanceRecommendationsRequestRequestTypeDef](./type_defs.md#getec2instancerecommendationsrequestrequesttypedef)
- [ExportAutoScalingGroupRecommendationsRequestRequestTypeDef](./type_defs.md#exportautoscalinggrouprecommendationsrequestrequesttypedef)
- [ExportEBSVolumeRecommendationsRequestRequestTypeDef](./type_defs.md#exportebsvolumerecommendationsrequestrequesttypedef)
- [ExportEC2InstanceRecommendationsRequestRequestTypeDef](./type_defs.md#exportec2instancerecommendationsrequestrequesttypedef)
- [ExportECSServiceRecommendationsRequestRequestTypeDef](./type_defs.md#exportecsservicerecommendationsrequestrequesttypedef)
- [ExportAutoScalingGroupRecommendationsResponseTypeDef](./type_defs.md#exportautoscalinggrouprecommendationsresponsetypedef)
- [ExportDestinationTypeDef](./type_defs.md#exportdestinationtypedef)
- [ExportEBSVolumeRecommendationsResponseTypeDef](./type_defs.md#exportebsvolumerecommendationsresponsetypedef)
- [ExportEC2InstanceRecommendationsResponseTypeDef](./type_defs.md#exportec2instancerecommendationsresponsetypedef)
- [ExportECSServiceRecommendationsResponseTypeDef](./type_defs.md#exportecsservicerecommendationsresponsetypedef)
- [ExportLambdaFunctionRecommendationsResponseTypeDef](./type_defs.md#exportlambdafunctionrecommendationsresponsetypedef)
- [ExportLicenseRecommendationsResponseTypeDef](./type_defs.md#exportlicenserecommendationsresponsetypedef)
- [ExportRDSDatabaseRecommendationsResponseTypeDef](./type_defs.md#exportrdsdatabaserecommendationsresponsetypedef)
- [ExportLambdaFunctionRecommendationsRequestRequestTypeDef](./type_defs.md#exportlambdafunctionrecommendationsrequestrequesttypedef)
- [GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef](./type_defs.md#getlambdafunctionrecommendationsrequestgetlambdafunctionrecommendationspaginatetypedef)
- [GetLambdaFunctionRecommendationsRequestRequestTypeDef](./type_defs.md#getlambdafunctionrecommendationsrequestrequesttypedef)
- [ExportLicenseRecommendationsRequestRequestTypeDef](./type_defs.md#exportlicenserecommendationsrequestrequesttypedef)
- [GetLicenseRecommendationsRequestRequestTypeDef](./type_defs.md#getlicenserecommendationsrequestrequesttypedef)
- [ExportRDSDatabaseRecommendationsRequestRequestTypeDef](./type_defs.md#exportrdsdatabaserecommendationsrequestrequesttypedef)
- [GetRDSDatabaseRecommendationsRequestRequestTypeDef](./type_defs.md#getrdsdatabaserecommendationsrequestrequesttypedef)
- [GetEC2RecommendationProjectedMetricsRequestRequestTypeDef](./type_defs.md#getec2recommendationprojectedmetricsrequestrequesttypedef)
- [GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef](./type_defs.md#getecsservicerecommendationprojectedmetricsrequestrequesttypedef)
- [GetRDSDatabaseRecommendationProjectedMetricsRequestRequestTypeDef](./type_defs.md#getrdsdatabaserecommendationprojectedmetricsrequestrequesttypedef)
- [GpuInfoTypeDef](./type_defs.md#gpuinfotypedef)
- [InstanceSavingsOpportunityAfterDiscountsTypeDef](./type_defs.md#instancesavingsopportunityafterdiscountstypedef)
- [LambdaEffectiveRecommendationPreferencesTypeDef](./type_defs.md#lambdaeffectiverecommendationpreferencestypedef)
- [LambdaSavingsOpportunityAfterDiscountsTypeDef](./type_defs.md#lambdasavingsopportunityafterdiscountstypedef)
- [LicenseConfigurationTypeDef](./type_defs.md#licenseconfigurationtypedef)
- [RecommendedOptionProjectedMetricTypeDef](./type_defs.md#recommendedoptionprojectedmetrictypedef)
- [RDSDatabaseRecommendedOptionProjectedMetricTypeDef](./type_defs.md#rdsdatabaserecommendedoptionprojectedmetrictypedef)
- [RDSEffectiveRecommendationPreferencesTypeDef](./type_defs.md#rdseffectiverecommendationpreferencestypedef)
- [RDSInstanceSavingsOpportunityAfterDiscountsTypeDef](./type_defs.md#rdsinstancesavingsopportunityafterdiscountstypedef)
- [RDSStorageSavingsOpportunityAfterDiscountsTypeDef](./type_defs.md#rdsstoragesavingsopportunityafterdiscountstypedef)
- [SummaryTypeDef](./type_defs.md#summarytypedef)
- [ServiceConfigurationTypeDef](./type_defs.md#serviceconfigurationtypedef)
- [EffectiveRecommendationPreferencesTypeDef](./type_defs.md#effectiverecommendationpreferencestypedef)
- [GetEffectiveRecommendationPreferencesResponseTypeDef](./type_defs.md#geteffectiverecommendationpreferencesresponsetypedef)
- [PutRecommendationPreferencesRequestRequestTypeDef](./type_defs.md#putrecommendationpreferencesrequestrequesttypedef)
- [RecommendationPreferencesDetailTypeDef](./type_defs.md#recommendationpreferencesdetailtypedef)
- [GetECSServiceRecommendationProjectedMetricsResponseTypeDef](./type_defs.md#getecsservicerecommendationprojectedmetricsresponsetypedef)
- [ECSServiceRecommendationOptionTypeDef](./type_defs.md#ecsservicerecommendationoptiontypedef)
- [LicenseRecommendationOptionTypeDef](./type_defs.md#licenserecommendationoptiontypedef)
- [VolumeRecommendationOptionTypeDef](./type_defs.md#volumerecommendationoptiontypedef)
- [RecommendationExportJobTypeDef](./type_defs.md#recommendationexportjobtypedef)
- [AutoScalingGroupRecommendationOptionTypeDef](./type_defs.md#autoscalinggrouprecommendationoptiontypedef)
- [InstanceRecommendationOptionTypeDef](./type_defs.md#instancerecommendationoptiontypedef)
- [LambdaFunctionMemoryRecommendationOptionTypeDef](./type_defs.md#lambdafunctionmemoryrecommendationoptiontypedef)
- [GetEC2RecommendationProjectedMetricsResponseTypeDef](./type_defs.md#getec2recommendationprojectedmetricsresponsetypedef)
- [GetRDSDatabaseRecommendationProjectedMetricsResponseTypeDef](./type_defs.md#getrdsdatabaserecommendationprojectedmetricsresponsetypedef)
- [RDSDBInstanceRecommendationOptionTypeDef](./type_defs.md#rdsdbinstancerecommendationoptiontypedef)
- [RDSDBStorageRecommendationOptionTypeDef](./type_defs.md#rdsdbstoragerecommendationoptiontypedef)
- [RecommendationSummaryTypeDef](./type_defs.md#recommendationsummarytypedef)
- [GetRecommendationPreferencesResponseTypeDef](./type_defs.md#getrecommendationpreferencesresponsetypedef)
- [ECSServiceRecommendationTypeDef](./type_defs.md#ecsservicerecommendationtypedef)
- [LicenseRecommendationTypeDef](./type_defs.md#licenserecommendationtypedef)
- [VolumeRecommendationTypeDef](./type_defs.md#volumerecommendationtypedef)
- [DescribeRecommendationExportJobsResponseTypeDef](./type_defs.md#describerecommendationexportjobsresponsetypedef)
- [AutoScalingGroupRecommendationTypeDef](./type_defs.md#autoscalinggrouprecommendationtypedef)
- [InstanceRecommendationTypeDef](./type_defs.md#instancerecommendationtypedef)
- [LambdaFunctionRecommendationTypeDef](./type_defs.md#lambdafunctionrecommendationtypedef)
- [RDSDBRecommendationTypeDef](./type_defs.md#rdsdbrecommendationtypedef)
- [GetRecommendationSummariesResponseTypeDef](./type_defs.md#getrecommendationsummariesresponsetypedef)
- [GetECSServiceRecommendationsResponseTypeDef](./type_defs.md#getecsservicerecommendationsresponsetypedef)
- [GetLicenseRecommendationsResponseTypeDef](./type_defs.md#getlicenserecommendationsresponsetypedef)
- [GetEBSVolumeRecommendationsResponseTypeDef](./type_defs.md#getebsvolumerecommendationsresponsetypedef)
- [GetAutoScalingGroupRecommendationsResponseTypeDef](./type_defs.md#getautoscalinggrouprecommendationsresponsetypedef)
- [GetEC2InstanceRecommendationsResponseTypeDef](./type_defs.md#getec2instancerecommendationsresponsetypedef)
- [GetLambdaFunctionRecommendationsResponseTypeDef](./type_defs.md#getlambdafunctionrecommendationsresponsetypedef)
- [GetRDSDatabaseRecommendationsResponseTypeDef](./type_defs.md#getrdsdatabaserecommendationsresponsetypedef)

