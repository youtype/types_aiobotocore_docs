# ForecastService module

> [Index](../README.md) > ForecastService


!!! note ""

    Auto-generated documentation for [ForecastService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#forecastservice)
    type annotations stubs module [types-aiobotocore-forecast](https://pypi.org/project/types-aiobotocore-forecast/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ForecastService` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ForecastService` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[forecast]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[forecast]'

# standalone installation
python -m pip install types-aiobotocore-forecast
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-forecast
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ForecastServiceClient

Type annotations and code completion for  `#!python session.create_client("forecast")` as [ForecastServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client)

```python
# ForecastServiceClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_forecast.client import ForecastServiceClient


session = get_session()
async with session.create_client("forecast") as client:
    client: ForecastServiceClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("forecast").get_paginator("...")`.

```python
# ListDatasetGroupsPaginator usage example

from types_aiobotocore_forecast.paginator import ListDatasetGroupsPaginator

def get_list_dataset_groups_paginator() -> ListDatasetGroupsPaginator:
    return client.get_paginator("list_dataset_groups"))
```

- [ListDatasetGroupsPaginator](./paginators.md#listdatasetgroupspaginator)
- [ListDatasetImportJobsPaginator](./paginators.md#listdatasetimportjobspaginator)
- [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
- [ListExplainabilitiesPaginator](./paginators.md#listexplainabilitiespaginator)
- [ListExplainabilityExportsPaginator](./paginators.md#listexplainabilityexportspaginator)
- [ListForecastExportJobsPaginator](./paginators.md#listforecastexportjobspaginator)
- [ListForecastsPaginator](./paginators.md#listforecastspaginator)
- [ListMonitorEvaluationsPaginator](./paginators.md#listmonitorevaluationspaginator)
- [ListMonitorsPaginator](./paginators.md#listmonitorspaginator)
- [ListPredictorBacktestExportJobsPaginator](./paginators.md#listpredictorbacktestexportjobspaginator)
- [ListPredictorsPaginator](./paginators.md#listpredictorspaginator)
- [ListWhatIfAnalysesPaginator](./paginators.md#listwhatifanalysespaginator)
- [ListWhatIfForecastExportsPaginator](./paginators.md#listwhatifforecastexportspaginator)
- [ListWhatIfForecastsPaginator](./paginators.md#listwhatifforecastspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AttributeTypeType usage example

from types_aiobotocore_forecast.literals import AttributeTypeType

def get_value() -> AttributeTypeType:
    return "float"
```

- [AttributeTypeType](./literals.md#attributetypetype)
- [AutoMLOverrideStrategyType](./literals.md#automloverridestrategytype)
- [ConditionType](./literals.md#conditiontype)
- [DatasetTypeType](./literals.md#datasettypetype)
- [DayOfWeekType](./literals.md#dayofweektype)
- [DomainType](./literals.md#domaintype)
- [EvaluationTypeType](./literals.md#evaluationtypetype)
- [FeaturizationMethodNameType](./literals.md#featurizationmethodnametype)
- [FilterConditionStringType](./literals.md#filterconditionstringtype)
- [ImportModeType](./literals.md#importmodetype)
- [ListDatasetGroupsPaginatorName](./literals.md#listdatasetgroupspaginatorname)
- [ListDatasetImportJobsPaginatorName](./literals.md#listdatasetimportjobspaginatorname)
- [ListDatasetsPaginatorName](./literals.md#listdatasetspaginatorname)
- [ListExplainabilitiesPaginatorName](./literals.md#listexplainabilitiespaginatorname)
- [ListExplainabilityExportsPaginatorName](./literals.md#listexplainabilityexportspaginatorname)
- [ListForecastExportJobsPaginatorName](./literals.md#listforecastexportjobspaginatorname)
- [ListForecastsPaginatorName](./literals.md#listforecastspaginatorname)
- [ListMonitorEvaluationsPaginatorName](./literals.md#listmonitorevaluationspaginatorname)
- [ListMonitorsPaginatorName](./literals.md#listmonitorspaginatorname)
- [ListPredictorBacktestExportJobsPaginatorName](./literals.md#listpredictorbacktestexportjobspaginatorname)
- [ListPredictorsPaginatorName](./literals.md#listpredictorspaginatorname)
- [ListWhatIfAnalysesPaginatorName](./literals.md#listwhatifanalysespaginatorname)
- [ListWhatIfForecastExportsPaginatorName](./literals.md#listwhatifforecastexportspaginatorname)
- [ListWhatIfForecastsPaginatorName](./literals.md#listwhatifforecastspaginatorname)
- [MonthType](./literals.md#monthtype)
- [OperationType](./literals.md#operationtype)
- [OptimizationMetricType](./literals.md#optimizationmetrictype)
- [ScalingTypeType](./literals.md#scalingtypetype)
- [StateType](./literals.md#statetype)
- [TimePointGranularityType](./literals.md#timepointgranularitytype)
- [TimeSeriesGranularityType](./literals.md#timeseriesgranularitytype)
- [ForecastServiceServiceName](./literals.md#forecastserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ActionTypeDef](./type_defs.md#actiontypedef)
- [AdditionalDatasetOutputTypeDef](./type_defs.md#additionaldatasetoutputtypedef)
- [AdditionalDatasetTypeDef](./type_defs.md#additionaldatasettypedef)
- [AttributeConfigOutputTypeDef](./type_defs.md#attributeconfigoutputtypedef)
- [AttributeConfigTypeDef](./type_defs.md#attributeconfigtypedef)
- [BaselineMetricTypeDef](./type_defs.md#baselinemetrictypedef)
- [CategoricalParameterRangeOutputTypeDef](./type_defs.md#categoricalparameterrangeoutputtypedef)
- [CategoricalParameterRangeTypeDef](./type_defs.md#categoricalparameterrangetypedef)
- [ContinuousParameterRangeTypeDef](./type_defs.md#continuousparameterrangetypedef)
- [EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef)
- [MonitorConfigTypeDef](./type_defs.md#monitorconfigtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [TimeAlignmentBoundaryTypeDef](./type_defs.md#timealignmentboundarytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ExplainabilityConfigTypeDef](./type_defs.md#explainabilityconfigtypedef)
- [EvaluationParametersTypeDef](./type_defs.md#evaluationparameterstypedef)
- [S3ConfigTypeDef](./type_defs.md#s3configtypedef)
- [DatasetGroupSummaryTypeDef](./type_defs.md#datasetgroupsummarytypedef)
- [DatasetSummaryTypeDef](./type_defs.md#datasetsummarytypedef)
- [DeleteDatasetGroupRequestRequestTypeDef](./type_defs.md#deletedatasetgrouprequestrequesttypedef)
- [DeleteDatasetImportJobRequestRequestTypeDef](./type_defs.md#deletedatasetimportjobrequestrequesttypedef)
- [DeleteDatasetRequestRequestTypeDef](./type_defs.md#deletedatasetrequestrequesttypedef)
- [DeleteExplainabilityExportRequestRequestTypeDef](./type_defs.md#deleteexplainabilityexportrequestrequesttypedef)
- [DeleteExplainabilityRequestRequestTypeDef](./type_defs.md#deleteexplainabilityrequestrequesttypedef)
- [DeleteForecastExportJobRequestRequestTypeDef](./type_defs.md#deleteforecastexportjobrequestrequesttypedef)
- [DeleteForecastRequestRequestTypeDef](./type_defs.md#deleteforecastrequestrequesttypedef)
- [DeleteMonitorRequestRequestTypeDef](./type_defs.md#deletemonitorrequestrequesttypedef)
- [DeletePredictorBacktestExportJobRequestRequestTypeDef](./type_defs.md#deletepredictorbacktestexportjobrequestrequesttypedef)
- [DeletePredictorRequestRequestTypeDef](./type_defs.md#deletepredictorrequestrequesttypedef)
- [DeleteResourceTreeRequestRequestTypeDef](./type_defs.md#deleteresourcetreerequestrequesttypedef)
- [DeleteWhatIfAnalysisRequestRequestTypeDef](./type_defs.md#deletewhatifanalysisrequestrequesttypedef)
- [DeleteWhatIfForecastExportRequestRequestTypeDef](./type_defs.md#deletewhatifforecastexportrequestrequesttypedef)
- [DeleteWhatIfForecastRequestRequestTypeDef](./type_defs.md#deletewhatifforecastrequestrequesttypedef)
- [DescribeAutoPredictorRequestRequestTypeDef](./type_defs.md#describeautopredictorrequestrequesttypedef)
- [ExplainabilityInfoTypeDef](./type_defs.md#explainabilityinfotypedef)
- [MonitorInfoTypeDef](./type_defs.md#monitorinfotypedef)
- [ReferencePredictorSummaryTypeDef](./type_defs.md#referencepredictorsummarytypedef)
- [DescribeDatasetGroupRequestRequestTypeDef](./type_defs.md#describedatasetgrouprequestrequesttypedef)
- [DescribeDatasetImportJobRequestRequestTypeDef](./type_defs.md#describedatasetimportjobrequestrequesttypedef)
- [StatisticsTypeDef](./type_defs.md#statisticstypedef)
- [DescribeDatasetRequestRequestTypeDef](./type_defs.md#describedatasetrequestrequesttypedef)
- [DescribeExplainabilityExportRequestRequestTypeDef](./type_defs.md#describeexplainabilityexportrequestrequesttypedef)
- [DescribeExplainabilityRequestRequestTypeDef](./type_defs.md#describeexplainabilityrequestrequesttypedef)
- [DescribeForecastExportJobRequestRequestTypeDef](./type_defs.md#describeforecastexportjobrequestrequesttypedef)
- [DescribeForecastRequestRequestTypeDef](./type_defs.md#describeforecastrequestrequesttypedef)
- [DescribeMonitorRequestRequestTypeDef](./type_defs.md#describemonitorrequestrequesttypedef)
- [DescribePredictorBacktestExportJobRequestRequestTypeDef](./type_defs.md#describepredictorbacktestexportjobrequestrequesttypedef)
- [DescribePredictorRequestRequestTypeDef](./type_defs.md#describepredictorrequestrequesttypedef)
- [DescribeWhatIfAnalysisRequestRequestTypeDef](./type_defs.md#describewhatifanalysisrequestrequesttypedef)
- [DescribeWhatIfForecastExportRequestRequestTypeDef](./type_defs.md#describewhatifforecastexportrequestrequesttypedef)
- [DescribeWhatIfForecastRequestRequestTypeDef](./type_defs.md#describewhatifforecastrequestrequesttypedef)
- [ErrorMetricTypeDef](./type_defs.md#errormetrictypedef)
- [FeaturizationMethodOutputTypeDef](./type_defs.md#featurizationmethodoutputtypedef)
- [FeaturizationMethodTypeDef](./type_defs.md#featurizationmethodtypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [ForecastSummaryTypeDef](./type_defs.md#forecastsummarytypedef)
- [GetAccuracyMetricsRequestRequestTypeDef](./type_defs.md#getaccuracymetricsrequestrequesttypedef)
- [SupplementaryFeatureTypeDef](./type_defs.md#supplementaryfeaturetypedef)
- [IntegerParameterRangeTypeDef](./type_defs.md#integerparameterrangetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListDatasetGroupsRequestRequestTypeDef](./type_defs.md#listdatasetgroupsrequestrequesttypedef)
- [ListDatasetsRequestRequestTypeDef](./type_defs.md#listdatasetsrequestrequesttypedef)
- [MonitorSummaryTypeDef](./type_defs.md#monitorsummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [WhatIfAnalysisSummaryTypeDef](./type_defs.md#whatifanalysissummarytypedef)
- [WhatIfForecastSummaryTypeDef](./type_defs.md#whatifforecastsummarytypedef)
- [MetricResultTypeDef](./type_defs.md#metricresulttypedef)
- [WeightedQuantileLossTypeDef](./type_defs.md#weightedquantilelosstypedef)
- [MonitorDataSourceTypeDef](./type_defs.md#monitordatasourcetypedef)
- [PredictorEventTypeDef](./type_defs.md#predictoreventtypedef)
- [TestWindowSummaryTypeDef](./type_defs.md#testwindowsummarytypedef)
- [ResumeResourceRequestRequestTypeDef](./type_defs.md#resumeresourcerequestrequesttypedef)
- [SchemaAttributeTypeDef](./type_defs.md#schemaattributetypedef)
- [StopResourceRequestRequestTypeDef](./type_defs.md#stopresourcerequestrequesttypedef)
- [TimeSeriesConditionTypeDef](./type_defs.md#timeseriesconditiontypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateDatasetGroupRequestRequestTypeDef](./type_defs.md#updatedatasetgrouprequestrequesttypedef)
- [AdditionalDatasetUnionTypeDef](./type_defs.md#additionaldatasetuniontypedef)
- [DataConfigOutputTypeDef](./type_defs.md#dataconfigoutputtypedef)
- [AttributeConfigUnionTypeDef](./type_defs.md#attributeconfiguniontypedef)
- [PredictorBaselineTypeDef](./type_defs.md#predictorbaselinetypedef)
- [CategoricalParameterRangeUnionTypeDef](./type_defs.md#categoricalparameterrangeuniontypedef)
- [CreateDatasetGroupRequestRequestTypeDef](./type_defs.md#createdatasetgrouprequestrequesttypedef)
- [CreateMonitorRequestRequestTypeDef](./type_defs.md#createmonitorrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateAutoPredictorResponseTypeDef](./type_defs.md#createautopredictorresponsetypedef)
- [CreateDatasetGroupResponseTypeDef](./type_defs.md#createdatasetgroupresponsetypedef)
- [CreateDatasetImportJobResponseTypeDef](./type_defs.md#createdatasetimportjobresponsetypedef)
- [CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef)
- [CreateExplainabilityExportResponseTypeDef](./type_defs.md#createexplainabilityexportresponsetypedef)
- [CreateExplainabilityResponseTypeDef](./type_defs.md#createexplainabilityresponsetypedef)
- [CreateForecastExportJobResponseTypeDef](./type_defs.md#createforecastexportjobresponsetypedef)
- [CreateForecastResponseTypeDef](./type_defs.md#createforecastresponsetypedef)
- [CreateMonitorResponseTypeDef](./type_defs.md#createmonitorresponsetypedef)
- [CreatePredictorBacktestExportJobResponseTypeDef](./type_defs.md#createpredictorbacktestexportjobresponsetypedef)
- [CreatePredictorResponseTypeDef](./type_defs.md#createpredictorresponsetypedef)
- [CreateWhatIfAnalysisResponseTypeDef](./type_defs.md#createwhatifanalysisresponsetypedef)
- [CreateWhatIfForecastExportResponseTypeDef](./type_defs.md#createwhatifforecastexportresponsetypedef)
- [CreateWhatIfForecastResponseTypeDef](./type_defs.md#createwhatifforecastresponsetypedef)
- [DescribeDatasetGroupResponseTypeDef](./type_defs.md#describedatasetgroupresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ExplainabilitySummaryTypeDef](./type_defs.md#explainabilitysummarytypedef)
- [DataDestinationTypeDef](./type_defs.md#datadestinationtypedef)
- [DataSourceTypeDef](./type_defs.md#datasourcetypedef)
- [ListDatasetGroupsResponseTypeDef](./type_defs.md#listdatasetgroupsresponsetypedef)
- [ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef)
- [PredictorSummaryTypeDef](./type_defs.md#predictorsummarytypedef)
- [FeaturizationOutputTypeDef](./type_defs.md#featurizationoutputtypedef)
- [FeaturizationMethodUnionTypeDef](./type_defs.md#featurizationmethoduniontypedef)
- [ListDatasetImportJobsRequestRequestTypeDef](./type_defs.md#listdatasetimportjobsrequestrequesttypedef)
- [ListExplainabilitiesRequestRequestTypeDef](./type_defs.md#listexplainabilitiesrequestrequesttypedef)
- [ListExplainabilityExportsRequestRequestTypeDef](./type_defs.md#listexplainabilityexportsrequestrequesttypedef)
- [ListForecastExportJobsRequestRequestTypeDef](./type_defs.md#listforecastexportjobsrequestrequesttypedef)
- [ListForecastsRequestRequestTypeDef](./type_defs.md#listforecastsrequestrequesttypedef)
- [ListMonitorEvaluationsRequestRequestTypeDef](./type_defs.md#listmonitorevaluationsrequestrequesttypedef)
- [ListMonitorsRequestRequestTypeDef](./type_defs.md#listmonitorsrequestrequesttypedef)
- [ListPredictorBacktestExportJobsRequestRequestTypeDef](./type_defs.md#listpredictorbacktestexportjobsrequestrequesttypedef)
- [ListPredictorsRequestRequestTypeDef](./type_defs.md#listpredictorsrequestrequesttypedef)
- [ListWhatIfAnalysesRequestRequestTypeDef](./type_defs.md#listwhatifanalysesrequestrequesttypedef)
- [ListWhatIfForecastExportsRequestRequestTypeDef](./type_defs.md#listwhatifforecastexportsrequestrequesttypedef)
- [ListWhatIfForecastsRequestRequestTypeDef](./type_defs.md#listwhatifforecastsrequestrequesttypedef)
- [ListForecastsResponseTypeDef](./type_defs.md#listforecastsresponsetypedef)
- [InputDataConfigOutputTypeDef](./type_defs.md#inputdataconfigoutputtypedef)
- [InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef)
- [ParameterRangesOutputTypeDef](./type_defs.md#parameterrangesoutputtypedef)
- [ListDatasetGroupsRequestPaginateTypeDef](./type_defs.md#listdatasetgroupsrequestpaginatetypedef)
- [ListDatasetImportJobsRequestPaginateTypeDef](./type_defs.md#listdatasetimportjobsrequestpaginatetypedef)
- [ListDatasetsRequestPaginateTypeDef](./type_defs.md#listdatasetsrequestpaginatetypedef)
- [ListExplainabilitiesRequestPaginateTypeDef](./type_defs.md#listexplainabilitiesrequestpaginatetypedef)
- [ListExplainabilityExportsRequestPaginateTypeDef](./type_defs.md#listexplainabilityexportsrequestpaginatetypedef)
- [ListForecastExportJobsRequestPaginateTypeDef](./type_defs.md#listforecastexportjobsrequestpaginatetypedef)
- [ListForecastsRequestPaginateTypeDef](./type_defs.md#listforecastsrequestpaginatetypedef)
- [ListMonitorEvaluationsRequestPaginateTypeDef](./type_defs.md#listmonitorevaluationsrequestpaginatetypedef)
- [ListMonitorsRequestPaginateTypeDef](./type_defs.md#listmonitorsrequestpaginatetypedef)
- [ListPredictorBacktestExportJobsRequestPaginateTypeDef](./type_defs.md#listpredictorbacktestexportjobsrequestpaginatetypedef)
- [ListPredictorsRequestPaginateTypeDef](./type_defs.md#listpredictorsrequestpaginatetypedef)
- [ListWhatIfAnalysesRequestPaginateTypeDef](./type_defs.md#listwhatifanalysesrequestpaginatetypedef)
- [ListWhatIfForecastExportsRequestPaginateTypeDef](./type_defs.md#listwhatifforecastexportsrequestpaginatetypedef)
- [ListWhatIfForecastsRequestPaginateTypeDef](./type_defs.md#listwhatifforecastsrequestpaginatetypedef)
- [ListMonitorsResponseTypeDef](./type_defs.md#listmonitorsresponsetypedef)
- [ListWhatIfAnalysesResponseTypeDef](./type_defs.md#listwhatifanalysesresponsetypedef)
- [ListWhatIfForecastsResponseTypeDef](./type_defs.md#listwhatifforecastsresponsetypedef)
- [MetricsTypeDef](./type_defs.md#metricstypedef)
- [PredictorMonitorEvaluationTypeDef](./type_defs.md#predictormonitorevaluationtypedef)
- [PredictorExecutionTypeDef](./type_defs.md#predictorexecutiontypedef)
- [SchemaOutputTypeDef](./type_defs.md#schemaoutputtypedef)
- [SchemaTypeDef](./type_defs.md#schematypedef)
- [TimeSeriesTransformationOutputTypeDef](./type_defs.md#timeseriestransformationoutputtypedef)
- [TimeSeriesTransformationTypeDef](./type_defs.md#timeseriestransformationtypedef)
- [DescribeAutoPredictorResponseTypeDef](./type_defs.md#describeautopredictorresponsetypedef)
- [DataConfigTypeDef](./type_defs.md#dataconfigtypedef)
- [BaselineTypeDef](./type_defs.md#baselinetypedef)
- [ParameterRangesTypeDef](./type_defs.md#parameterrangestypedef)
- [ListExplainabilitiesResponseTypeDef](./type_defs.md#listexplainabilitiesresponsetypedef)
- [CreateExplainabilityExportRequestRequestTypeDef](./type_defs.md#createexplainabilityexportrequestrequesttypedef)
- [CreateForecastExportJobRequestRequestTypeDef](./type_defs.md#createforecastexportjobrequestrequesttypedef)
- [CreatePredictorBacktestExportJobRequestRequestTypeDef](./type_defs.md#createpredictorbacktestexportjobrequestrequesttypedef)
- [CreateWhatIfForecastExportRequestRequestTypeDef](./type_defs.md#createwhatifforecastexportrequestrequesttypedef)
- [DescribeExplainabilityExportResponseTypeDef](./type_defs.md#describeexplainabilityexportresponsetypedef)
- [DescribeForecastExportJobResponseTypeDef](./type_defs.md#describeforecastexportjobresponsetypedef)
- [DescribePredictorBacktestExportJobResponseTypeDef](./type_defs.md#describepredictorbacktestexportjobresponsetypedef)
- [DescribeWhatIfForecastExportResponseTypeDef](./type_defs.md#describewhatifforecastexportresponsetypedef)
- [ExplainabilityExportSummaryTypeDef](./type_defs.md#explainabilityexportsummarytypedef)
- [ForecastExportJobSummaryTypeDef](./type_defs.md#forecastexportjobsummarytypedef)
- [PredictorBacktestExportJobSummaryTypeDef](./type_defs.md#predictorbacktestexportjobsummarytypedef)
- [WhatIfForecastExportSummaryTypeDef](./type_defs.md#whatifforecastexportsummarytypedef)
- [CreateDatasetImportJobRequestRequestTypeDef](./type_defs.md#createdatasetimportjobrequestrequesttypedef)
- [DatasetImportJobSummaryTypeDef](./type_defs.md#datasetimportjobsummarytypedef)
- [DescribeDatasetImportJobResponseTypeDef](./type_defs.md#describedatasetimportjobresponsetypedef)
- [ListPredictorsResponseTypeDef](./type_defs.md#listpredictorsresponsetypedef)
- [FeaturizationConfigOutputTypeDef](./type_defs.md#featurizationconfigoutputtypedef)
- [FeaturizationTypeDef](./type_defs.md#featurizationtypedef)
- [HyperParameterTuningJobConfigOutputTypeDef](./type_defs.md#hyperparametertuningjobconfigoutputtypedef)
- [WindowSummaryTypeDef](./type_defs.md#windowsummarytypedef)
- [ListMonitorEvaluationsResponseTypeDef](./type_defs.md#listmonitorevaluationsresponsetypedef)
- [PredictorExecutionDetailsTypeDef](./type_defs.md#predictorexecutiondetailstypedef)
- [DescribeDatasetResponseTypeDef](./type_defs.md#describedatasetresponsetypedef)
- [DescribeExplainabilityResponseTypeDef](./type_defs.md#describeexplainabilityresponsetypedef)
- [TimeSeriesIdentifiersOutputTypeDef](./type_defs.md#timeseriesidentifiersoutputtypedef)
- [TimeSeriesReplacementsDataSourceOutputTypeDef](./type_defs.md#timeseriesreplacementsdatasourceoutputtypedef)
- [CreateDatasetRequestRequestTypeDef](./type_defs.md#createdatasetrequestrequesttypedef)
- [CreateExplainabilityRequestRequestTypeDef](./type_defs.md#createexplainabilityrequestrequesttypedef)
- [SchemaUnionTypeDef](./type_defs.md#schemauniontypedef)
- [TimeSeriesTransformationUnionTypeDef](./type_defs.md#timeseriestransformationuniontypedef)
- [CreateAutoPredictorRequestRequestTypeDef](./type_defs.md#createautopredictorrequestrequesttypedef)
- [DescribeMonitorResponseTypeDef](./type_defs.md#describemonitorresponsetypedef)
- [ParameterRangesUnionTypeDef](./type_defs.md#parameterrangesuniontypedef)
- [ListExplainabilityExportsResponseTypeDef](./type_defs.md#listexplainabilityexportsresponsetypedef)
- [ListForecastExportJobsResponseTypeDef](./type_defs.md#listforecastexportjobsresponsetypedef)
- [ListPredictorBacktestExportJobsResponseTypeDef](./type_defs.md#listpredictorbacktestexportjobsresponsetypedef)
- [ListWhatIfForecastExportsResponseTypeDef](./type_defs.md#listwhatifforecastexportsresponsetypedef)
- [ListDatasetImportJobsResponseTypeDef](./type_defs.md#listdatasetimportjobsresponsetypedef)
- [FeaturizationUnionTypeDef](./type_defs.md#featurizationuniontypedef)
- [EvaluationResultTypeDef](./type_defs.md#evaluationresulttypedef)
- [DescribePredictorResponseTypeDef](./type_defs.md#describepredictorresponsetypedef)
- [TimeSeriesSelectorOutputTypeDef](./type_defs.md#timeseriesselectoroutputtypedef)
- [DescribeWhatIfForecastResponseTypeDef](./type_defs.md#describewhatifforecastresponsetypedef)
- [TimeSeriesIdentifiersTypeDef](./type_defs.md#timeseriesidentifierstypedef)
- [TimeSeriesReplacementsDataSourceTypeDef](./type_defs.md#timeseriesreplacementsdatasourcetypedef)
- [HyperParameterTuningJobConfigTypeDef](./type_defs.md#hyperparametertuningjobconfigtypedef)
- [FeaturizationConfigTypeDef](./type_defs.md#featurizationconfigtypedef)
- [GetAccuracyMetricsResponseTypeDef](./type_defs.md#getaccuracymetricsresponsetypedef)
- [DescribeForecastResponseTypeDef](./type_defs.md#describeforecastresponsetypedef)
- [DescribeWhatIfAnalysisResponseTypeDef](./type_defs.md#describewhatifanalysisresponsetypedef)
- [TimeSeriesIdentifiersUnionTypeDef](./type_defs.md#timeseriesidentifiersuniontypedef)
- [CreateWhatIfForecastRequestRequestTypeDef](./type_defs.md#createwhatifforecastrequestrequesttypedef)
- [CreatePredictorRequestRequestTypeDef](./type_defs.md#createpredictorrequestrequesttypedef)
- [TimeSeriesSelectorTypeDef](./type_defs.md#timeseriesselectortypedef)
- [CreateForecastRequestRequestTypeDef](./type_defs.md#createforecastrequestrequesttypedef)
- [CreateWhatIfAnalysisRequestRequestTypeDef](./type_defs.md#createwhatifanalysisrequestrequesttypedef)

