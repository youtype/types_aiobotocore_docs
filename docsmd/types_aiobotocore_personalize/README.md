# Personalize module

> [Index](../README.md) > Personalize


!!! note ""

    Auto-generated documentation for [Personalize](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#personalize)
    type annotations stubs module [types-aiobotocore-personalize](https://pypi.org/project/types-aiobotocore-personalize/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Personalize` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Personalize` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[personalize]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[personalize]'

# standalone installation
python -m pip install types-aiobotocore-personalize
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-personalize
```

## Usage

Code samples can be found in [Examples](./usage.md).

## PersonalizeClient

Type annotations and code completion for  `#!python session.create_client("personalize")` as [PersonalizeClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client)

```python
# PersonalizeClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_personalize.client import PersonalizeClient


session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("personalize").get_paginator("...")`.

```python
# ListBatchInferenceJobsPaginator usage example

from types_aiobotocore_personalize.paginator import ListBatchInferenceJobsPaginator

def get_list_batch_inference_jobs_paginator() -> ListBatchInferenceJobsPaginator:
    return client.get_paginator("list_batch_inference_jobs"))
```

- [ListBatchInferenceJobsPaginator](./paginators.md#listbatchinferencejobspaginator)
- [ListBatchSegmentJobsPaginator](./paginators.md#listbatchsegmentjobspaginator)
- [ListCampaignsPaginator](./paginators.md#listcampaignspaginator)
- [ListDatasetExportJobsPaginator](./paginators.md#listdatasetexportjobspaginator)
- [ListDatasetGroupsPaginator](./paginators.md#listdatasetgroupspaginator)
- [ListDatasetImportJobsPaginator](./paginators.md#listdatasetimportjobspaginator)
- [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
- [ListEventTrackersPaginator](./paginators.md#listeventtrackerspaginator)
- [ListFiltersPaginator](./paginators.md#listfilterspaginator)
- [ListMetricAttributionMetricsPaginator](./paginators.md#listmetricattributionmetricspaginator)
- [ListMetricAttributionsPaginator](./paginators.md#listmetricattributionspaginator)
- [ListRecipesPaginator](./paginators.md#listrecipespaginator)
- [ListRecommendersPaginator](./paginators.md#listrecommenderspaginator)
- [ListSchemasPaginator](./paginators.md#listschemaspaginator)
- [ListSolutionVersionsPaginator](./paginators.md#listsolutionversionspaginator)
- [ListSolutionsPaginator](./paginators.md#listsolutionspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# BatchInferenceJobModeType usage example

from types_aiobotocore_personalize.literals import BatchInferenceJobModeType

def get_value() -> BatchInferenceJobModeType:
    return "BATCH_INFERENCE"
```

- [BatchInferenceJobModeType](./literals.md#batchinferencejobmodetype)
- [DomainType](./literals.md#domaintype)
- [ImportModeType](./literals.md#importmodetype)
- [IngestionModeType](./literals.md#ingestionmodetype)
- [ListBatchInferenceJobsPaginatorName](./literals.md#listbatchinferencejobspaginatorname)
- [ListBatchSegmentJobsPaginatorName](./literals.md#listbatchsegmentjobspaginatorname)
- [ListCampaignsPaginatorName](./literals.md#listcampaignspaginatorname)
- [ListDatasetExportJobsPaginatorName](./literals.md#listdatasetexportjobspaginatorname)
- [ListDatasetGroupsPaginatorName](./literals.md#listdatasetgroupspaginatorname)
- [ListDatasetImportJobsPaginatorName](./literals.md#listdatasetimportjobspaginatorname)
- [ListDatasetsPaginatorName](./literals.md#listdatasetspaginatorname)
- [ListEventTrackersPaginatorName](./literals.md#listeventtrackerspaginatorname)
- [ListFiltersPaginatorName](./literals.md#listfilterspaginatorname)
- [ListMetricAttributionMetricsPaginatorName](./literals.md#listmetricattributionmetricspaginatorname)
- [ListMetricAttributionsPaginatorName](./literals.md#listmetricattributionspaginatorname)
- [ListRecipesPaginatorName](./literals.md#listrecipespaginatorname)
- [ListRecommendersPaginatorName](./literals.md#listrecommenderspaginatorname)
- [ListSchemasPaginatorName](./literals.md#listschemaspaginatorname)
- [ListSolutionVersionsPaginatorName](./literals.md#listsolutionversionspaginatorname)
- [ListSolutionsPaginatorName](./literals.md#listsolutionspaginatorname)
- [ObjectiveSensitivityType](./literals.md#objectivesensitivitytype)
- [RecipeProviderType](./literals.md#recipeprovidertype)
- [TrainingModeType](./literals.md#trainingmodetype)
- [TrainingTypeType](./literals.md#trainingtypetype)
- [PersonalizeServiceName](./literals.md#personalizeservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AlgorithmImageTypeDef](./type_defs.md#algorithmimagetypedef)
- [AutoMLConfigOutputTypeDef](./type_defs.md#automlconfigoutputtypedef)
- [AutoMLConfigTypeDef](./type_defs.md#automlconfigtypedef)
- [AutoMLResultTypeDef](./type_defs.md#automlresulttypedef)
- [AutoTrainingConfigTypeDef](./type_defs.md#autotrainingconfigtypedef)
- [BatchInferenceJobConfigOutputTypeDef](./type_defs.md#batchinferencejobconfigoutputtypedef)
- [BatchInferenceJobConfigTypeDef](./type_defs.md#batchinferencejobconfigtypedef)
- [S3DataConfigTypeDef](./type_defs.md#s3dataconfigtypedef)
- [BatchInferenceJobSummaryTypeDef](./type_defs.md#batchinferencejobsummarytypedef)
- [BatchSegmentJobSummaryTypeDef](./type_defs.md#batchsegmentjobsummarytypedef)
- [CampaignConfigOutputTypeDef](./type_defs.md#campaignconfigoutputtypedef)
- [CampaignConfigTypeDef](./type_defs.md#campaignconfigtypedef)
- [CampaignSummaryTypeDef](./type_defs.md#campaignsummarytypedef)
- [CategoricalHyperParameterRangeOutputTypeDef](./type_defs.md#categoricalhyperparameterrangeoutputtypedef)
- [CategoricalHyperParameterRangeTypeDef](./type_defs.md#categoricalhyperparameterrangetypedef)
- [ContinuousHyperParameterRangeTypeDef](./type_defs.md#continuoushyperparameterrangetypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DataSourceTypeDef](./type_defs.md#datasourcetypedef)
- [MetricAttributeTypeDef](./type_defs.md#metricattributetypedef)
- [CreateSchemaRequestRequestTypeDef](./type_defs.md#createschemarequestrequesttypedef)
- [DataDeletionJobSummaryTypeDef](./type_defs.md#datadeletionjobsummarytypedef)
- [DatasetExportJobSummaryTypeDef](./type_defs.md#datasetexportjobsummarytypedef)
- [DatasetGroupSummaryTypeDef](./type_defs.md#datasetgroupsummarytypedef)
- [DatasetGroupTypeDef](./type_defs.md#datasetgrouptypedef)
- [DatasetImportJobSummaryTypeDef](./type_defs.md#datasetimportjobsummarytypedef)
- [DatasetSchemaSummaryTypeDef](./type_defs.md#datasetschemasummarytypedef)
- [DatasetSchemaTypeDef](./type_defs.md#datasetschematypedef)
- [DatasetSummaryTypeDef](./type_defs.md#datasetsummarytypedef)
- [DatasetUpdateSummaryTypeDef](./type_defs.md#datasetupdatesummarytypedef)
- [DefaultCategoricalHyperParameterRangeTypeDef](./type_defs.md#defaultcategoricalhyperparameterrangetypedef)
- [DefaultContinuousHyperParameterRangeTypeDef](./type_defs.md#defaultcontinuoushyperparameterrangetypedef)
- [DefaultIntegerHyperParameterRangeTypeDef](./type_defs.md#defaultintegerhyperparameterrangetypedef)
- [DeleteCampaignRequestRequestTypeDef](./type_defs.md#deletecampaignrequestrequesttypedef)
- [DeleteDatasetGroupRequestRequestTypeDef](./type_defs.md#deletedatasetgrouprequestrequesttypedef)
- [DeleteDatasetRequestRequestTypeDef](./type_defs.md#deletedatasetrequestrequesttypedef)
- [DeleteEventTrackerRequestRequestTypeDef](./type_defs.md#deleteeventtrackerrequestrequesttypedef)
- [DeleteFilterRequestRequestTypeDef](./type_defs.md#deletefilterrequestrequesttypedef)
- [DeleteMetricAttributionRequestRequestTypeDef](./type_defs.md#deletemetricattributionrequestrequesttypedef)
- [DeleteRecommenderRequestRequestTypeDef](./type_defs.md#deleterecommenderrequestrequesttypedef)
- [DeleteSchemaRequestRequestTypeDef](./type_defs.md#deleteschemarequestrequesttypedef)
- [DeleteSolutionRequestRequestTypeDef](./type_defs.md#deletesolutionrequestrequesttypedef)
- [DescribeAlgorithmRequestRequestTypeDef](./type_defs.md#describealgorithmrequestrequesttypedef)
- [DescribeBatchInferenceJobRequestRequestTypeDef](./type_defs.md#describebatchinferencejobrequestrequesttypedef)
- [DescribeBatchSegmentJobRequestRequestTypeDef](./type_defs.md#describebatchsegmentjobrequestrequesttypedef)
- [DescribeCampaignRequestRequestTypeDef](./type_defs.md#describecampaignrequestrequesttypedef)
- [DescribeDataDeletionJobRequestRequestTypeDef](./type_defs.md#describedatadeletionjobrequestrequesttypedef)
- [DescribeDatasetExportJobRequestRequestTypeDef](./type_defs.md#describedatasetexportjobrequestrequesttypedef)
- [DescribeDatasetGroupRequestRequestTypeDef](./type_defs.md#describedatasetgrouprequestrequesttypedef)
- [DescribeDatasetImportJobRequestRequestTypeDef](./type_defs.md#describedatasetimportjobrequestrequesttypedef)
- [DescribeDatasetRequestRequestTypeDef](./type_defs.md#describedatasetrequestrequesttypedef)
- [DescribeEventTrackerRequestRequestTypeDef](./type_defs.md#describeeventtrackerrequestrequesttypedef)
- [EventTrackerTypeDef](./type_defs.md#eventtrackertypedef)
- [DescribeFeatureTransformationRequestRequestTypeDef](./type_defs.md#describefeaturetransformationrequestrequesttypedef)
- [FeatureTransformationTypeDef](./type_defs.md#featuretransformationtypedef)
- [DescribeFilterRequestRequestTypeDef](./type_defs.md#describefilterrequestrequesttypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [DescribeMetricAttributionRequestRequestTypeDef](./type_defs.md#describemetricattributionrequestrequesttypedef)
- [DescribeRecipeRequestRequestTypeDef](./type_defs.md#describereciperequestrequesttypedef)
- [RecipeTypeDef](./type_defs.md#recipetypedef)
- [DescribeRecommenderRequestRequestTypeDef](./type_defs.md#describerecommenderrequestrequesttypedef)
- [DescribeSchemaRequestRequestTypeDef](./type_defs.md#describeschemarequestrequesttypedef)
- [DescribeSolutionRequestRequestTypeDef](./type_defs.md#describesolutionrequestrequesttypedef)
- [DescribeSolutionVersionRequestRequestTypeDef](./type_defs.md#describesolutionversionrequestrequesttypedef)
- [EventTrackerSummaryTypeDef](./type_defs.md#eventtrackersummarytypedef)
- [FieldsForThemeGenerationTypeDef](./type_defs.md#fieldsforthemegenerationtypedef)
- [FilterSummaryTypeDef](./type_defs.md#filtersummarytypedef)
- [GetSolutionMetricsRequestRequestTypeDef](./type_defs.md#getsolutionmetricsrequestrequesttypedef)
- [HPOObjectiveTypeDef](./type_defs.md#hpoobjectivetypedef)
- [HPOResourceConfigTypeDef](./type_defs.md#hporesourceconfigtypedef)
- [IntegerHyperParameterRangeTypeDef](./type_defs.md#integerhyperparameterrangetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListBatchInferenceJobsRequestRequestTypeDef](./type_defs.md#listbatchinferencejobsrequestrequesttypedef)
- [ListBatchSegmentJobsRequestRequestTypeDef](./type_defs.md#listbatchsegmentjobsrequestrequesttypedef)
- [ListCampaignsRequestRequestTypeDef](./type_defs.md#listcampaignsrequestrequesttypedef)
- [ListDataDeletionJobsRequestRequestTypeDef](./type_defs.md#listdatadeletionjobsrequestrequesttypedef)
- [ListDatasetExportJobsRequestRequestTypeDef](./type_defs.md#listdatasetexportjobsrequestrequesttypedef)
- [ListDatasetGroupsRequestRequestTypeDef](./type_defs.md#listdatasetgroupsrequestrequesttypedef)
- [ListDatasetImportJobsRequestRequestTypeDef](./type_defs.md#listdatasetimportjobsrequestrequesttypedef)
- [ListDatasetsRequestRequestTypeDef](./type_defs.md#listdatasetsrequestrequesttypedef)
- [ListEventTrackersRequestRequestTypeDef](./type_defs.md#listeventtrackersrequestrequesttypedef)
- [ListFiltersRequestRequestTypeDef](./type_defs.md#listfiltersrequestrequesttypedef)
- [ListMetricAttributionMetricsRequestRequestTypeDef](./type_defs.md#listmetricattributionmetricsrequestrequesttypedef)
- [ListMetricAttributionsRequestRequestTypeDef](./type_defs.md#listmetricattributionsrequestrequesttypedef)
- [MetricAttributionSummaryTypeDef](./type_defs.md#metricattributionsummarytypedef)
- [ListRecipesRequestRequestTypeDef](./type_defs.md#listrecipesrequestrequesttypedef)
- [RecipeSummaryTypeDef](./type_defs.md#recipesummarytypedef)
- [ListRecommendersRequestRequestTypeDef](./type_defs.md#listrecommendersrequestrequesttypedef)
- [ListSchemasRequestRequestTypeDef](./type_defs.md#listschemasrequestrequesttypedef)
- [ListSolutionVersionsRequestRequestTypeDef](./type_defs.md#listsolutionversionsrequestrequesttypedef)
- [SolutionVersionSummaryTypeDef](./type_defs.md#solutionversionsummarytypedef)
- [ListSolutionsRequestRequestTypeDef](./type_defs.md#listsolutionsrequestrequesttypedef)
- [SolutionSummaryTypeDef](./type_defs.md#solutionsummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [OptimizationObjectiveTypeDef](./type_defs.md#optimizationobjectivetypedef)
- [TrainingDataConfigOutputTypeDef](./type_defs.md#trainingdataconfigoutputtypedef)
- [TunedHPOParamsTypeDef](./type_defs.md#tunedhpoparamstypedef)
- [StartRecommenderRequestRequestTypeDef](./type_defs.md#startrecommenderrequestrequesttypedef)
- [StopRecommenderRequestRequestTypeDef](./type_defs.md#stoprecommenderrequestrequesttypedef)
- [StopSolutionVersionCreationRequestRequestTypeDef](./type_defs.md#stopsolutionversioncreationrequestrequesttypedef)
- [TrainingDataConfigTypeDef](./type_defs.md#trainingdataconfigtypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateDatasetRequestRequestTypeDef](./type_defs.md#updatedatasetrequestrequesttypedef)
- [AutoMLConfigUnionTypeDef](./type_defs.md#automlconfiguniontypedef)
- [SolutionUpdateConfigTypeDef](./type_defs.md#solutionupdateconfigtypedef)
- [BatchInferenceJobInputTypeDef](./type_defs.md#batchinferencejobinputtypedef)
- [BatchInferenceJobOutputTypeDef](./type_defs.md#batchinferencejoboutputtypedef)
- [BatchSegmentJobInputTypeDef](./type_defs.md#batchsegmentjobinputtypedef)
- [BatchSegmentJobOutputTypeDef](./type_defs.md#batchsegmentjoboutputtypedef)
- [DatasetExportJobOutputTypeDef](./type_defs.md#datasetexportjoboutputtypedef)
- [MetricAttributionOutputTypeDef](./type_defs.md#metricattributionoutputtypedef)
- [CampaignUpdateSummaryTypeDef](./type_defs.md#campaignupdatesummarytypedef)
- [UpdateCampaignRequestRequestTypeDef](./type_defs.md#updatecampaignrequestrequesttypedef)
- [CategoricalHyperParameterRangeUnionTypeDef](./type_defs.md#categoricalhyperparameterrangeuniontypedef)
- [CreateCampaignRequestRequestTypeDef](./type_defs.md#createcampaignrequestrequesttypedef)
- [CreateDatasetGroupRequestRequestTypeDef](./type_defs.md#createdatasetgrouprequestrequesttypedef)
- [CreateDatasetRequestRequestTypeDef](./type_defs.md#createdatasetrequestrequesttypedef)
- [CreateEventTrackerRequestRequestTypeDef](./type_defs.md#createeventtrackerrequestrequesttypedef)
- [CreateFilterRequestRequestTypeDef](./type_defs.md#createfilterrequestrequesttypedef)
- [CreateSolutionVersionRequestRequestTypeDef](./type_defs.md#createsolutionversionrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateBatchInferenceJobResponseTypeDef](./type_defs.md#createbatchinferencejobresponsetypedef)
- [CreateBatchSegmentJobResponseTypeDef](./type_defs.md#createbatchsegmentjobresponsetypedef)
- [CreateCampaignResponseTypeDef](./type_defs.md#createcampaignresponsetypedef)
- [CreateDataDeletionJobResponseTypeDef](./type_defs.md#createdatadeletionjobresponsetypedef)
- [CreateDatasetExportJobResponseTypeDef](./type_defs.md#createdatasetexportjobresponsetypedef)
- [CreateDatasetGroupResponseTypeDef](./type_defs.md#createdatasetgroupresponsetypedef)
- [CreateDatasetImportJobResponseTypeDef](./type_defs.md#createdatasetimportjobresponsetypedef)
- [CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef)
- [CreateEventTrackerResponseTypeDef](./type_defs.md#createeventtrackerresponsetypedef)
- [CreateFilterResponseTypeDef](./type_defs.md#createfilterresponsetypedef)
- [CreateMetricAttributionResponseTypeDef](./type_defs.md#createmetricattributionresponsetypedef)
- [CreateRecommenderResponseTypeDef](./type_defs.md#createrecommenderresponsetypedef)
- [CreateSchemaResponseTypeDef](./type_defs.md#createschemaresponsetypedef)
- [CreateSolutionResponseTypeDef](./type_defs.md#createsolutionresponsetypedef)
- [CreateSolutionVersionResponseTypeDef](./type_defs.md#createsolutionversionresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetSolutionMetricsResponseTypeDef](./type_defs.md#getsolutionmetricsresponsetypedef)
- [ListBatchInferenceJobsResponseTypeDef](./type_defs.md#listbatchinferencejobsresponsetypedef)
- [ListBatchSegmentJobsResponseTypeDef](./type_defs.md#listbatchsegmentjobsresponsetypedef)
- [ListCampaignsResponseTypeDef](./type_defs.md#listcampaignsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartRecommenderResponseTypeDef](./type_defs.md#startrecommenderresponsetypedef)
- [StopRecommenderResponseTypeDef](./type_defs.md#stoprecommenderresponsetypedef)
- [UpdateCampaignResponseTypeDef](./type_defs.md#updatecampaignresponsetypedef)
- [UpdateDatasetResponseTypeDef](./type_defs.md#updatedatasetresponsetypedef)
- [UpdateMetricAttributionResponseTypeDef](./type_defs.md#updatemetricattributionresponsetypedef)
- [UpdateRecommenderResponseTypeDef](./type_defs.md#updaterecommenderresponsetypedef)
- [UpdateSolutionResponseTypeDef](./type_defs.md#updatesolutionresponsetypedef)
- [CreateDataDeletionJobRequestRequestTypeDef](./type_defs.md#createdatadeletionjobrequestrequesttypedef)
- [CreateDatasetImportJobRequestRequestTypeDef](./type_defs.md#createdatasetimportjobrequestrequesttypedef)
- [DataDeletionJobTypeDef](./type_defs.md#datadeletionjobtypedef)
- [DatasetImportJobTypeDef](./type_defs.md#datasetimportjobtypedef)
- [ListMetricAttributionMetricsResponseTypeDef](./type_defs.md#listmetricattributionmetricsresponsetypedef)
- [ListDataDeletionJobsResponseTypeDef](./type_defs.md#listdatadeletionjobsresponsetypedef)
- [ListDatasetExportJobsResponseTypeDef](./type_defs.md#listdatasetexportjobsresponsetypedef)
- [ListDatasetGroupsResponseTypeDef](./type_defs.md#listdatasetgroupsresponsetypedef)
- [DescribeDatasetGroupResponseTypeDef](./type_defs.md#describedatasetgroupresponsetypedef)
- [ListDatasetImportJobsResponseTypeDef](./type_defs.md#listdatasetimportjobsresponsetypedef)
- [ListSchemasResponseTypeDef](./type_defs.md#listschemasresponsetypedef)
- [DescribeSchemaResponseTypeDef](./type_defs.md#describeschemaresponsetypedef)
- [ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef)
- [DatasetTypeDef](./type_defs.md#datasettypedef)
- [DefaultHyperParameterRangesTypeDef](./type_defs.md#defaulthyperparameterrangestypedef)
- [DescribeEventTrackerResponseTypeDef](./type_defs.md#describeeventtrackerresponsetypedef)
- [DescribeFeatureTransformationResponseTypeDef](./type_defs.md#describefeaturetransformationresponsetypedef)
- [DescribeFilterResponseTypeDef](./type_defs.md#describefilterresponsetypedef)
- [DescribeRecipeResponseTypeDef](./type_defs.md#describereciperesponsetypedef)
- [ListEventTrackersResponseTypeDef](./type_defs.md#listeventtrackersresponsetypedef)
- [ThemeGenerationConfigTypeDef](./type_defs.md#themegenerationconfigtypedef)
- [ListFiltersResponseTypeDef](./type_defs.md#listfiltersresponsetypedef)
- [HyperParameterRangesOutputTypeDef](./type_defs.md#hyperparameterrangesoutputtypedef)
- [ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef](./type_defs.md#listbatchinferencejobsrequestlistbatchinferencejobspaginatetypedef)
- [ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef](./type_defs.md#listbatchsegmentjobsrequestlistbatchsegmentjobspaginatetypedef)
- [ListCampaignsRequestListCampaignsPaginateTypeDef](./type_defs.md#listcampaignsrequestlistcampaignspaginatetypedef)
- [ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef](./type_defs.md#listdatasetexportjobsrequestlistdatasetexportjobspaginatetypedef)
- [ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef](./type_defs.md#listdatasetgroupsrequestlistdatasetgroupspaginatetypedef)
- [ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef](./type_defs.md#listdatasetimportjobsrequestlistdatasetimportjobspaginatetypedef)
- [ListDatasetsRequestListDatasetsPaginateTypeDef](./type_defs.md#listdatasetsrequestlistdatasetspaginatetypedef)
- [ListEventTrackersRequestListEventTrackersPaginateTypeDef](./type_defs.md#listeventtrackersrequestlisteventtrackerspaginatetypedef)
- [ListFiltersRequestListFiltersPaginateTypeDef](./type_defs.md#listfiltersrequestlistfilterspaginatetypedef)
- [ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef](./type_defs.md#listmetricattributionmetricsrequestlistmetricattributionmetricspaginatetypedef)
- [ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef](./type_defs.md#listmetricattributionsrequestlistmetricattributionspaginatetypedef)
- [ListRecipesRequestListRecipesPaginateTypeDef](./type_defs.md#listrecipesrequestlistrecipespaginatetypedef)
- [ListRecommendersRequestListRecommendersPaginateTypeDef](./type_defs.md#listrecommendersrequestlistrecommenderspaginatetypedef)
- [ListSchemasRequestListSchemasPaginateTypeDef](./type_defs.md#listschemasrequestlistschemaspaginatetypedef)
- [ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef](./type_defs.md#listsolutionversionsrequestlistsolutionversionspaginatetypedef)
- [ListSolutionsRequestListSolutionsPaginateTypeDef](./type_defs.md#listsolutionsrequestlistsolutionspaginatetypedef)
- [ListMetricAttributionsResponseTypeDef](./type_defs.md#listmetricattributionsresponsetypedef)
- [ListRecipesResponseTypeDef](./type_defs.md#listrecipesresponsetypedef)
- [ListSolutionVersionsResponseTypeDef](./type_defs.md#listsolutionversionsresponsetypedef)
- [ListSolutionsResponseTypeDef](./type_defs.md#listsolutionsresponsetypedef)
- [RecommenderConfigOutputTypeDef](./type_defs.md#recommenderconfigoutputtypedef)
- [TrainingDataConfigUnionTypeDef](./type_defs.md#trainingdataconfiguniontypedef)
- [SolutionUpdateSummaryTypeDef](./type_defs.md#solutionupdatesummarytypedef)
- [UpdateSolutionRequestRequestTypeDef](./type_defs.md#updatesolutionrequestrequesttypedef)
- [BatchSegmentJobTypeDef](./type_defs.md#batchsegmentjobtypedef)
- [CreateBatchSegmentJobRequestRequestTypeDef](./type_defs.md#createbatchsegmentjobrequestrequesttypedef)
- [CreateDatasetExportJobRequestRequestTypeDef](./type_defs.md#createdatasetexportjobrequestrequesttypedef)
- [DatasetExportJobTypeDef](./type_defs.md#datasetexportjobtypedef)
- [CreateMetricAttributionRequestRequestTypeDef](./type_defs.md#createmetricattributionrequestrequesttypedef)
- [MetricAttributionTypeDef](./type_defs.md#metricattributiontypedef)
- [UpdateMetricAttributionRequestRequestTypeDef](./type_defs.md#updatemetricattributionrequestrequesttypedef)
- [CampaignTypeDef](./type_defs.md#campaigntypedef)
- [HyperParameterRangesTypeDef](./type_defs.md#hyperparameterrangestypedef)
- [DescribeDataDeletionJobResponseTypeDef](./type_defs.md#describedatadeletionjobresponsetypedef)
- [DescribeDatasetImportJobResponseTypeDef](./type_defs.md#describedatasetimportjobresponsetypedef)
- [DescribeDatasetResponseTypeDef](./type_defs.md#describedatasetresponsetypedef)
- [AlgorithmTypeDef](./type_defs.md#algorithmtypedef)
- [BatchInferenceJobTypeDef](./type_defs.md#batchinferencejobtypedef)
- [CreateBatchInferenceJobRequestRequestTypeDef](./type_defs.md#createbatchinferencejobrequestrequesttypedef)
- [HPOConfigOutputTypeDef](./type_defs.md#hpoconfigoutputtypedef)
- [RecommenderSummaryTypeDef](./type_defs.md#recommendersummarytypedef)
- [RecommenderUpdateSummaryTypeDef](./type_defs.md#recommenderupdatesummarytypedef)
- [RecommenderConfigTypeDef](./type_defs.md#recommenderconfigtypedef)
- [DescribeBatchSegmentJobResponseTypeDef](./type_defs.md#describebatchsegmentjobresponsetypedef)
- [DescribeDatasetExportJobResponseTypeDef](./type_defs.md#describedatasetexportjobresponsetypedef)
- [DescribeMetricAttributionResponseTypeDef](./type_defs.md#describemetricattributionresponsetypedef)
- [DescribeCampaignResponseTypeDef](./type_defs.md#describecampaignresponsetypedef)
- [HyperParameterRangesUnionTypeDef](./type_defs.md#hyperparameterrangesuniontypedef)
- [DescribeAlgorithmResponseTypeDef](./type_defs.md#describealgorithmresponsetypedef)
- [DescribeBatchInferenceJobResponseTypeDef](./type_defs.md#describebatchinferencejobresponsetypedef)
- [SolutionConfigOutputTypeDef](./type_defs.md#solutionconfigoutputtypedef)
- [ListRecommendersResponseTypeDef](./type_defs.md#listrecommendersresponsetypedef)
- [RecommenderTypeDef](./type_defs.md#recommendertypedef)
- [CreateRecommenderRequestRequestTypeDef](./type_defs.md#createrecommenderrequestrequesttypedef)
- [UpdateRecommenderRequestRequestTypeDef](./type_defs.md#updaterecommenderrequestrequesttypedef)
- [HPOConfigTypeDef](./type_defs.md#hpoconfigtypedef)
- [SolutionTypeDef](./type_defs.md#solutiontypedef)
- [SolutionVersionTypeDef](./type_defs.md#solutionversiontypedef)
- [DescribeRecommenderResponseTypeDef](./type_defs.md#describerecommenderresponsetypedef)
- [HPOConfigUnionTypeDef](./type_defs.md#hpoconfiguniontypedef)
- [DescribeSolutionResponseTypeDef](./type_defs.md#describesolutionresponsetypedef)
- [DescribeSolutionVersionResponseTypeDef](./type_defs.md#describesolutionversionresponsetypedef)
- [SolutionConfigTypeDef](./type_defs.md#solutionconfigtypedef)
- [CreateSolutionRequestRequestTypeDef](./type_defs.md#createsolutionrequestrequesttypedef)

