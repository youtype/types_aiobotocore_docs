# ResilienceHub module

> [Index](../README.md) > ResilienceHub


!!! note ""

    Auto-generated documentation for [ResilienceHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#resiliencehub)
    type annotations stubs module [types-aiobotocore-resiliencehub](https://pypi.org/project/types-aiobotocore-resiliencehub/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ResilienceHub` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ResilienceHub` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[resiliencehub]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[resiliencehub]'

# standalone installation
python -m pip install types-aiobotocore-resiliencehub
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-resiliencehub
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ResilienceHubClient

Type annotations and code completion for  `#!python session.create_client("resiliencehub")` as [ResilienceHubClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client)

```python
# ResilienceHubClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_resiliencehub.client import ResilienceHubClient


session = get_session()
async with session.create_client("resiliencehub") as client:
    client: ResilienceHubClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("resiliencehub").get_paginator("...")`.

```python
# ListAppAssessmentResourceDriftsPaginator usage example

from types_aiobotocore_resiliencehub.paginator import ListAppAssessmentResourceDriftsPaginator

def get_list_app_assessment_resource_drifts_paginator() -> ListAppAssessmentResourceDriftsPaginator:
    return client.get_paginator("list_app_assessment_resource_drifts"))
```

- [ListAppAssessmentResourceDriftsPaginator](./paginators.md#listappassessmentresourcedriftspaginator)
- [ListMetricsPaginator](./paginators.md#listmetricspaginator)
- [ListResourceGroupingRecommendationsPaginator](./paginators.md#listresourcegroupingrecommendationspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AlarmTypeType usage example

from types_aiobotocore_resiliencehub.literals import AlarmTypeType

def get_value() -> AlarmTypeType:
    return "Canary"
```

- [AlarmTypeType](./literals.md#alarmtypetype)
- [AppAssessmentScheduleTypeType](./literals.md#appassessmentscheduletypetype)
- [AppComplianceStatusTypeType](./literals.md#appcompliancestatustypetype)
- [AppDriftStatusTypeType](./literals.md#appdriftstatustypetype)
- [AppStatusTypeType](./literals.md#appstatustypetype)
- [AssessmentInvokerType](./literals.md#assessmentinvokertype)
- [AssessmentStatusType](./literals.md#assessmentstatustype)
- [ComplianceStatusType](./literals.md#compliancestatustype)
- [ConditionOperatorTypeType](./literals.md#conditionoperatortypetype)
- [ConfigRecommendationOptimizationTypeType](./literals.md#configrecommendationoptimizationtypetype)
- [CostFrequencyType](./literals.md#costfrequencytype)
- [DataLocationConstraintType](./literals.md#datalocationconstrainttype)
- [DifferenceTypeType](./literals.md#differencetypetype)
- [DisruptionTypeType](./literals.md#disruptiontypetype)
- [DriftStatusType](./literals.md#driftstatustype)
- [DriftTypeType](./literals.md#drifttypetype)
- [EstimatedCostTierType](./literals.md#estimatedcosttiertype)
- [EventTypeType](./literals.md#eventtypetype)
- [ExcludeRecommendationReasonType](./literals.md#excluderecommendationreasontype)
- [FieldAggregationTypeType](./literals.md#fieldaggregationtypetype)
- [GroupingRecommendationConfidenceLevelType](./literals.md#groupingrecommendationconfidenceleveltype)
- [GroupingRecommendationRejectionReasonType](./literals.md#groupingrecommendationrejectionreasontype)
- [GroupingRecommendationStatusTypeType](./literals.md#groupingrecommendationstatustypetype)
- [HaArchitectureType](./literals.md#haarchitecturetype)
- [ListAppAssessmentResourceDriftsPaginatorName](./literals.md#listappassessmentresourcedriftspaginatorname)
- [ListMetricsPaginatorName](./literals.md#listmetricspaginatorname)
- [ListResourceGroupingRecommendationsPaginatorName](./literals.md#listresourcegroupingrecommendationspaginatorname)
- [MetricsExportStatusTypeType](./literals.md#metricsexportstatustypetype)
- [PermissionModelTypeType](./literals.md#permissionmodeltypetype)
- [PhysicalIdentifierTypeType](./literals.md#physicalidentifiertypetype)
- [RecommendationComplianceStatusType](./literals.md#recommendationcompliancestatustype)
- [RecommendationStatusType](./literals.md#recommendationstatustype)
- [RecommendationTemplateStatusType](./literals.md#recommendationtemplatestatustype)
- [RenderRecommendationTypeType](./literals.md#renderrecommendationtypetype)
- [ResiliencyPolicyTierType](./literals.md#resiliencypolicytiertype)
- [ResiliencyScoreTypeType](./literals.md#resiliencyscoretypetype)
- [ResourceImportStatusTypeType](./literals.md#resourceimportstatustypetype)
- [ResourceImportStrategyTypeType](./literals.md#resourceimportstrategytypetype)
- [ResourceMappingTypeType](./literals.md#resourcemappingtypetype)
- [ResourceResolutionStatusTypeType](./literals.md#resourceresolutionstatustypetype)
- [ResourceSourceTypeType](./literals.md#resourcesourcetypetype)
- [ResourcesGroupingRecGenStatusTypeType](./literals.md#resourcesgroupingrecgenstatustypetype)
- [SopServiceTypeType](./literals.md#sopservicetypetype)
- [TemplateFormatType](./literals.md#templateformattype)
- [TestRiskType](./literals.md#testrisktype)
- [TestTypeType](./literals.md#testtypetype)
- [ResilienceHubServiceName](./literals.md#resiliencehubservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AcceptGroupingRecommendationEntryTypeDef](./type_defs.md#acceptgroupingrecommendationentrytypedef)
- [FailedGroupingRecommendationEntryTypeDef](./type_defs.md#failedgroupingrecommendationentrytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AlarmTypeDef](./type_defs.md#alarmtypedef)
- [CostTypeDef](./type_defs.md#costtypedef)
- [DisruptionComplianceTypeDef](./type_defs.md#disruptioncompliancetypedef)
- [AppComponentTypeDef](./type_defs.md#appcomponenttypedef)
- [EksSourceClusterNamespaceTypeDef](./type_defs.md#ekssourceclusternamespacetypedef)
- [TerraformSourceTypeDef](./type_defs.md#terraformsourcetypedef)
- [AppSummaryTypeDef](./type_defs.md#appsummarytypedef)
- [EventSubscriptionTypeDef](./type_defs.md#eventsubscriptiontypedef)
- [PermissionModelOutputTypeDef](./type_defs.md#permissionmodeloutputtypedef)
- [AppVersionSummaryTypeDef](./type_defs.md#appversionsummarytypedef)
- [AssessmentRiskRecommendationTypeDef](./type_defs.md#assessmentriskrecommendationtypedef)
- [BatchUpdateRecommendationStatusFailedEntryTypeDef](./type_defs.md#batchupdaterecommendationstatusfailedentrytypedef)
- [UpdateRecommendationStatusItemTypeDef](./type_defs.md#updaterecommendationstatusitemtypedef)
- [ConditionTypeDef](./type_defs.md#conditiontypedef)
- [RecommendationDisruptionComplianceTypeDef](./type_defs.md#recommendationdisruptioncompliancetypedef)
- [PermissionModelTypeDef](./type_defs.md#permissionmodeltypedef)
- [CreateAppVersionAppComponentRequestRequestTypeDef](./type_defs.md#createappversionappcomponentrequestrequesttypedef)
- [LogicalResourceIdTypeDef](./type_defs.md#logicalresourceidtypedef)
- [CreateRecommendationTemplateRequestRequestTypeDef](./type_defs.md#createrecommendationtemplaterequestrequesttypedef)
- [FailurePolicyTypeDef](./type_defs.md#failurepolicytypedef)
- [DeleteAppAssessmentRequestRequestTypeDef](./type_defs.md#deleteappassessmentrequestrequesttypedef)
- [DeleteAppRequestRequestTypeDef](./type_defs.md#deleteapprequestrequesttypedef)
- [DeleteAppVersionAppComponentRequestRequestTypeDef](./type_defs.md#deleteappversionappcomponentrequestrequesttypedef)
- [DeleteRecommendationTemplateRequestRequestTypeDef](./type_defs.md#deleterecommendationtemplaterequestrequesttypedef)
- [DeleteResiliencyPolicyRequestRequestTypeDef](./type_defs.md#deleteresiliencypolicyrequestrequesttypedef)
- [DescribeAppAssessmentRequestRequestTypeDef](./type_defs.md#describeappassessmentrequestrequesttypedef)
- [DescribeAppRequestRequestTypeDef](./type_defs.md#describeapprequestrequesttypedef)
- [DescribeAppVersionAppComponentRequestRequestTypeDef](./type_defs.md#describeappversionappcomponentrequestrequesttypedef)
- [DescribeAppVersionRequestRequestTypeDef](./type_defs.md#describeappversionrequestrequesttypedef)
- [DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef](./type_defs.md#describeappversionresourcesresolutionstatusrequestrequesttypedef)
- [DescribeAppVersionTemplateRequestRequestTypeDef](./type_defs.md#describeappversiontemplaterequestrequesttypedef)
- [DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef](./type_defs.md#describedraftappversionresourcesimportstatusrequestrequesttypedef)
- [ErrorDetailTypeDef](./type_defs.md#errordetailtypedef)
- [DescribeMetricsExportRequestRequestTypeDef](./type_defs.md#describemetricsexportrequestrequesttypedef)
- [S3LocationTypeDef](./type_defs.md#s3locationtypedef)
- [DescribeResiliencyPolicyRequestRequestTypeDef](./type_defs.md#describeresiliencypolicyrequestrequesttypedef)
- [DescribeResourceGroupingRecommendationTaskRequestRequestTypeDef](./type_defs.md#describeresourcegroupingrecommendationtaskrequestrequesttypedef)
- [EksSourceOutputTypeDef](./type_defs.md#ekssourceoutputtypedef)
- [EksSourceTypeDef](./type_defs.md#ekssourcetypedef)
- [ExperimentTypeDef](./type_defs.md#experimenttypedef)
- [FieldTypeDef](./type_defs.md#fieldtypedef)
- [GroupingAppComponentTypeDef](./type_defs.md#groupingappcomponenttypedef)
- [PhysicalResourceIdTypeDef](./type_defs.md#physicalresourceidtypedef)
- [ListAlarmRecommendationsRequestRequestTypeDef](./type_defs.md#listalarmrecommendationsrequestrequesttypedef)
- [ListAppAssessmentComplianceDriftsRequestRequestTypeDef](./type_defs.md#listappassessmentcompliancedriftsrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAppAssessmentResourceDriftsRequestRequestTypeDef](./type_defs.md#listappassessmentresourcedriftsrequestrequesttypedef)
- [ListAppAssessmentsRequestRequestTypeDef](./type_defs.md#listappassessmentsrequestrequesttypedef)
- [ListAppComponentCompliancesRequestRequestTypeDef](./type_defs.md#listappcomponentcompliancesrequestrequesttypedef)
- [ListAppComponentRecommendationsRequestRequestTypeDef](./type_defs.md#listappcomponentrecommendationsrequestrequesttypedef)
- [ListAppInputSourcesRequestRequestTypeDef](./type_defs.md#listappinputsourcesrequestrequesttypedef)
- [ListAppVersionAppComponentsRequestRequestTypeDef](./type_defs.md#listappversionappcomponentsrequestrequesttypedef)
- [ListAppVersionResourceMappingsRequestRequestTypeDef](./type_defs.md#listappversionresourcemappingsrequestrequesttypedef)
- [ListAppVersionResourcesRequestRequestTypeDef](./type_defs.md#listappversionresourcesrequestrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [SortTypeDef](./type_defs.md#sorttypedef)
- [ListRecommendationTemplatesRequestRequestTypeDef](./type_defs.md#listrecommendationtemplatesrequestrequesttypedef)
- [ListResiliencyPoliciesRequestRequestTypeDef](./type_defs.md#listresiliencypoliciesrequestrequesttypedef)
- [ListResourceGroupingRecommendationsRequestRequestTypeDef](./type_defs.md#listresourcegroupingrecommendationsrequestrequesttypedef)
- [ListSopRecommendationsRequestRequestTypeDef](./type_defs.md#listsoprecommendationsrequestrequesttypedef)
- [ListSuggestedResiliencyPoliciesRequestRequestTypeDef](./type_defs.md#listsuggestedresiliencypoliciesrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTestRecommendationsRequestRequestTypeDef](./type_defs.md#listtestrecommendationsrequestrequesttypedef)
- [ListUnsupportedAppVersionResourcesRequestRequestTypeDef](./type_defs.md#listunsupportedappversionresourcesrequestrequesttypedef)
- [PublishAppVersionRequestRequestTypeDef](./type_defs.md#publishappversionrequestrequesttypedef)
- [PutDraftAppVersionTemplateRequestRequestTypeDef](./type_defs.md#putdraftappversiontemplaterequestrequesttypedef)
- [RejectGroupingRecommendationEntryTypeDef](./type_defs.md#rejectgroupingrecommendationentrytypedef)
- [RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef](./type_defs.md#removedraftappversionresourcemappingsrequestrequesttypedef)
- [ScoringComponentResiliencyScoreTypeDef](./type_defs.md#scoringcomponentresiliencyscoretypedef)
- [ResolveAppVersionResourcesRequestRequestTypeDef](./type_defs.md#resolveappversionresourcesrequestrequesttypedef)
- [ResourceErrorTypeDef](./type_defs.md#resourceerrortypedef)
- [StartAppAssessmentRequestRequestTypeDef](./type_defs.md#startappassessmentrequestrequesttypedef)
- [StartMetricsExportRequestRequestTypeDef](./type_defs.md#startmetricsexportrequestrequesttypedef)
- [StartResourceGroupingRecommendationTaskRequestRequestTypeDef](./type_defs.md#startresourcegroupingrecommendationtaskrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateAppVersionAppComponentRequestRequestTypeDef](./type_defs.md#updateappversionappcomponentrequestrequesttypedef)
- [UpdateAppVersionRequestRequestTypeDef](./type_defs.md#updateappversionrequestrequesttypedef)
- [AcceptResourceGroupingRecommendationsRequestRequestTypeDef](./type_defs.md#acceptresourcegroupingrecommendationsrequestrequesttypedef)
- [AcceptResourceGroupingRecommendationsResponseTypeDef](./type_defs.md#acceptresourcegroupingrecommendationsresponsetypedef)
- [DeleteAppAssessmentResponseTypeDef](./type_defs.md#deleteappassessmentresponsetypedef)
- [DeleteAppResponseTypeDef](./type_defs.md#deleteappresponsetypedef)
- [DeleteRecommendationTemplateResponseTypeDef](./type_defs.md#deleterecommendationtemplateresponsetypedef)
- [DeleteResiliencyPolicyResponseTypeDef](./type_defs.md#deleteresiliencypolicyresponsetypedef)
- [DescribeAppVersionResourcesResolutionStatusResponseTypeDef](./type_defs.md#describeappversionresourcesresolutionstatusresponsetypedef)
- [DescribeAppVersionResponseTypeDef](./type_defs.md#describeappversionresponsetypedef)
- [DescribeAppVersionTemplateResponseTypeDef](./type_defs.md#describeappversiontemplateresponsetypedef)
- [DescribeResourceGroupingRecommendationTaskResponseTypeDef](./type_defs.md#describeresourcegroupingrecommendationtaskresponsetypedef)
- [ListMetricsResponseTypeDef](./type_defs.md#listmetricsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PublishAppVersionResponseTypeDef](./type_defs.md#publishappversionresponsetypedef)
- [PutDraftAppVersionTemplateResponseTypeDef](./type_defs.md#putdraftappversiontemplateresponsetypedef)
- [RejectResourceGroupingRecommendationsResponseTypeDef](./type_defs.md#rejectresourcegroupingrecommendationsresponsetypedef)
- [RemoveDraftAppVersionResourceMappingsResponseTypeDef](./type_defs.md#removedraftappversionresourcemappingsresponsetypedef)
- [ResolveAppVersionResourcesResponseTypeDef](./type_defs.md#resolveappversionresourcesresponsetypedef)
- [StartMetricsExportResponseTypeDef](./type_defs.md#startmetricsexportresponsetypedef)
- [StartResourceGroupingRecommendationTaskResponseTypeDef](./type_defs.md#startresourcegroupingrecommendationtaskresponsetypedef)
- [UpdateAppVersionResponseTypeDef](./type_defs.md#updateappversionresponsetypedef)
- [AppAssessmentSummaryTypeDef](./type_defs.md#appassessmentsummarytypedef)
- [ComplianceDriftTypeDef](./type_defs.md#compliancedrifttypedef)
- [CreateAppVersionAppComponentResponseTypeDef](./type_defs.md#createappversionappcomponentresponsetypedef)
- [DeleteAppVersionAppComponentResponseTypeDef](./type_defs.md#deleteappversionappcomponentresponsetypedef)
- [DescribeAppVersionAppComponentResponseTypeDef](./type_defs.md#describeappversionappcomponentresponsetypedef)
- [ListAppVersionAppComponentsResponseTypeDef](./type_defs.md#listappversionappcomponentsresponsetypedef)
- [UpdateAppVersionAppComponentResponseTypeDef](./type_defs.md#updateappversionappcomponentresponsetypedef)
- [AppInputSourceTypeDef](./type_defs.md#appinputsourcetypedef)
- [DeleteAppInputSourceRequestRequestTypeDef](./type_defs.md#deleteappinputsourcerequestrequesttypedef)
- [ListAppsResponseTypeDef](./type_defs.md#listappsresponsetypedef)
- [AppTypeDef](./type_defs.md#apptypedef)
- [ListAppVersionsResponseTypeDef](./type_defs.md#listappversionsresponsetypedef)
- [AssessmentSummaryTypeDef](./type_defs.md#assessmentsummarytypedef)
- [BatchUpdateRecommendationStatusSuccessfulEntryTypeDef](./type_defs.md#batchupdaterecommendationstatussuccessfulentrytypedef)
- [UpdateRecommendationStatusRequestEntryTypeDef](./type_defs.md#updaterecommendationstatusrequestentrytypedef)
- [ConfigRecommendationTypeDef](./type_defs.md#configrecommendationtypedef)
- [CreateAppRequestRequestTypeDef](./type_defs.md#createapprequestrequesttypedef)
- [UpdateAppRequestRequestTypeDef](./type_defs.md#updateapprequestrequesttypedef)
- [CreateAppVersionResourceRequestRequestTypeDef](./type_defs.md#createappversionresourcerequestrequesttypedef)
- [DeleteAppVersionResourceRequestRequestTypeDef](./type_defs.md#deleteappversionresourcerequestrequesttypedef)
- [DescribeAppVersionResourceRequestRequestTypeDef](./type_defs.md#describeappversionresourcerequestrequesttypedef)
- [ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef)
- [UpdateAppVersionResourceRequestRequestTypeDef](./type_defs.md#updateappversionresourcerequestrequesttypedef)
- [CreateResiliencyPolicyRequestRequestTypeDef](./type_defs.md#createresiliencypolicyrequestrequesttypedef)
- [ResiliencyPolicyTypeDef](./type_defs.md#resiliencypolicytypedef)
- [UpdateResiliencyPolicyRequestRequestTypeDef](./type_defs.md#updateresiliencypolicyrequestrequesttypedef)
- [DescribeDraftAppVersionResourcesImportStatusResponseTypeDef](./type_defs.md#describedraftappversionresourcesimportstatusresponsetypedef)
- [DescribeMetricsExportResponseTypeDef](./type_defs.md#describemetricsexportresponsetypedef)
- [RecommendationTemplateTypeDef](./type_defs.md#recommendationtemplatetypedef)
- [ImportResourcesToDraftAppVersionResponseTypeDef](./type_defs.md#importresourcestodraftappversionresponsetypedef)
- [EksSourceUnionTypeDef](./type_defs.md#ekssourceuniontypedef)
- [RecommendationItemTypeDef](./type_defs.md#recommendationitemtypedef)
- [GroupingResourceTypeDef](./type_defs.md#groupingresourcetypedef)
- [PhysicalResourceTypeDef](./type_defs.md#physicalresourcetypedef)
- [ResourceMappingTypeDef](./type_defs.md#resourcemappingtypedef)
- [UnsupportedResourceTypeDef](./type_defs.md#unsupportedresourcetypedef)
- [ListAppAssessmentResourceDriftsRequestPaginateTypeDef](./type_defs.md#listappassessmentresourcedriftsrequestpaginatetypedef)
- [ListResourceGroupingRecommendationsRequestPaginateTypeDef](./type_defs.md#listresourcegroupingrecommendationsrequestpaginatetypedef)
- [ListAppVersionsRequestRequestTypeDef](./type_defs.md#listappversionsrequestrequesttypedef)
- [ListAppsRequestRequestTypeDef](./type_defs.md#listappsrequestrequesttypedef)
- [ListMetricsRequestPaginateTypeDef](./type_defs.md#listmetricsrequestpaginatetypedef)
- [ListMetricsRequestRequestTypeDef](./type_defs.md#listmetricsrequestrequesttypedef)
- [RejectResourceGroupingRecommendationsRequestRequestTypeDef](./type_defs.md#rejectresourcegroupingrecommendationsrequestrequesttypedef)
- [ResiliencyScoreTypeDef](./type_defs.md#resiliencyscoretypedef)
- [ResourceErrorsDetailsTypeDef](./type_defs.md#resourceerrorsdetailstypedef)
- [ListAppAssessmentsResponseTypeDef](./type_defs.md#listappassessmentsresponsetypedef)
- [ListAppAssessmentComplianceDriftsResponseTypeDef](./type_defs.md#listappassessmentcompliancedriftsresponsetypedef)
- [DeleteAppInputSourceResponseTypeDef](./type_defs.md#deleteappinputsourceresponsetypedef)
- [ListAppInputSourcesResponseTypeDef](./type_defs.md#listappinputsourcesresponsetypedef)
- [CreateAppResponseTypeDef](./type_defs.md#createappresponsetypedef)
- [DescribeAppResponseTypeDef](./type_defs.md#describeappresponsetypedef)
- [UpdateAppResponseTypeDef](./type_defs.md#updateappresponsetypedef)
- [BatchUpdateRecommendationStatusResponseTypeDef](./type_defs.md#batchupdaterecommendationstatusresponsetypedef)
- [BatchUpdateRecommendationStatusRequestRequestTypeDef](./type_defs.md#batchupdaterecommendationstatusrequestrequesttypedef)
- [ComponentRecommendationTypeDef](./type_defs.md#componentrecommendationtypedef)
- [ResourceDriftTypeDef](./type_defs.md#resourcedrifttypedef)
- [CreateResiliencyPolicyResponseTypeDef](./type_defs.md#createresiliencypolicyresponsetypedef)
- [DescribeResiliencyPolicyResponseTypeDef](./type_defs.md#describeresiliencypolicyresponsetypedef)
- [ListResiliencyPoliciesResponseTypeDef](./type_defs.md#listresiliencypoliciesresponsetypedef)
- [ListSuggestedResiliencyPoliciesResponseTypeDef](./type_defs.md#listsuggestedresiliencypoliciesresponsetypedef)
- [UpdateResiliencyPolicyResponseTypeDef](./type_defs.md#updateresiliencypolicyresponsetypedef)
- [CreateRecommendationTemplateResponseTypeDef](./type_defs.md#createrecommendationtemplateresponsetypedef)
- [ListRecommendationTemplatesResponseTypeDef](./type_defs.md#listrecommendationtemplatesresponsetypedef)
- [ImportResourcesToDraftAppVersionRequestRequestTypeDef](./type_defs.md#importresourcestodraftappversionrequestrequesttypedef)
- [AlarmRecommendationTypeDef](./type_defs.md#alarmrecommendationtypedef)
- [SopRecommendationTypeDef](./type_defs.md#soprecommendationtypedef)
- [TestRecommendationTypeDef](./type_defs.md#testrecommendationtypedef)
- [GroupingRecommendationTypeDef](./type_defs.md#groupingrecommendationtypedef)
- [CreateAppVersionResourceResponseTypeDef](./type_defs.md#createappversionresourceresponsetypedef)
- [DeleteAppVersionResourceResponseTypeDef](./type_defs.md#deleteappversionresourceresponsetypedef)
- [DescribeAppVersionResourceResponseTypeDef](./type_defs.md#describeappversionresourceresponsetypedef)
- [ListAppVersionResourcesResponseTypeDef](./type_defs.md#listappversionresourcesresponsetypedef)
- [UpdateAppVersionResourceResponseTypeDef](./type_defs.md#updateappversionresourceresponsetypedef)
- [AddDraftAppVersionResourceMappingsRequestRequestTypeDef](./type_defs.md#adddraftappversionresourcemappingsrequestrequesttypedef)
- [AddDraftAppVersionResourceMappingsResponseTypeDef](./type_defs.md#adddraftappversionresourcemappingsresponsetypedef)
- [ListAppVersionResourceMappingsResponseTypeDef](./type_defs.md#listappversionresourcemappingsresponsetypedef)
- [ListUnsupportedAppVersionResourcesResponseTypeDef](./type_defs.md#listunsupportedappversionresourcesresponsetypedef)
- [AppComponentComplianceTypeDef](./type_defs.md#appcomponentcompliancetypedef)
- [AppAssessmentTypeDef](./type_defs.md#appassessmenttypedef)
- [ListAppComponentRecommendationsResponseTypeDef](./type_defs.md#listappcomponentrecommendationsresponsetypedef)
- [ListAppAssessmentResourceDriftsResponseTypeDef](./type_defs.md#listappassessmentresourcedriftsresponsetypedef)
- [ListAlarmRecommendationsResponseTypeDef](./type_defs.md#listalarmrecommendationsresponsetypedef)
- [ListSopRecommendationsResponseTypeDef](./type_defs.md#listsoprecommendationsresponsetypedef)
- [ListTestRecommendationsResponseTypeDef](./type_defs.md#listtestrecommendationsresponsetypedef)
- [ListResourceGroupingRecommendationsResponseTypeDef](./type_defs.md#listresourcegroupingrecommendationsresponsetypedef)
- [ListAppComponentCompliancesResponseTypeDef](./type_defs.md#listappcomponentcompliancesresponsetypedef)
- [DescribeAppAssessmentResponseTypeDef](./type_defs.md#describeappassessmentresponsetypedef)
- [StartAppAssessmentResponseTypeDef](./type_defs.md#startappassessmentresponsetypedef)

