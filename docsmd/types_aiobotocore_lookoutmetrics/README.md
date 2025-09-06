# LookoutMetrics module

> [Index](../README.md) > LookoutMetrics


!!! note ""

    Auto-generated documentation for [LookoutMetrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#lookoutmetrics)
    type annotations stubs module [types-aiobotocore-lookoutmetrics](https://pypi.org/project/types-aiobotocore-lookoutmetrics/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.24.2' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `LookoutMetrics` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `LookoutMetrics` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[lookoutmetrics]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[lookoutmetrics]'

# standalone installation
python -m pip install types-aiobotocore-lookoutmetrics
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-lookoutmetrics
```

## Usage

Code samples can be found in [Examples](./usage.md).

## LookoutMetricsClient

Type annotations and code completion for  `#!python session.create_client("lookoutmetrics")` as [LookoutMetricsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client)

```python
# LookoutMetricsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_lookoutmetrics.client import LookoutMetricsClient


session = get_session()
async with session.create_client("lookoutmetrics") as client:
    client: LookoutMetricsClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AggregationFunctionType usage example

from types_aiobotocore_lookoutmetrics.literals import AggregationFunctionType

def get_value() -> AggregationFunctionType:
    return "AVG"
```

- [AggregationFunctionType](./literals.md#aggregationfunctiontype)
- [AlertStatusType](./literals.md#alertstatustype)
- [AlertTypeType](./literals.md#alerttypetype)
- [AnomalyDetectionTaskStatusType](./literals.md#anomalydetectiontaskstatustype)
- [AnomalyDetectorFailureTypeType](./literals.md#anomalydetectorfailuretypetype)
- [AnomalyDetectorStatusType](./literals.md#anomalydetectorstatustype)
- [CSVFileCompressionType](./literals.md#csvfilecompressiontype)
- [ConfidenceType](./literals.md#confidencetype)
- [DataQualityMetricTypeType](./literals.md#dataqualitymetrictypetype)
- [FilterOperationType](./literals.md#filteroperationtype)
- [FrequencyType](./literals.md#frequencytype)
- [JsonFileCompressionType](./literals.md#jsonfilecompressiontype)
- [RelationshipTypeType](./literals.md#relationshiptypetype)
- [SnsFormatType](./literals.md#snsformattype)
- [LookoutMetricsServiceName](./literals.md#lookoutmetricsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [LambdaConfigurationTypeDef](./type_defs.md#lambdaconfigurationtypedef)
- [SNSConfigurationTypeDef](./type_defs.md#snsconfigurationtypedef)
- [ActivateAnomalyDetectorRequestTypeDef](./type_defs.md#activateanomalydetectorrequesttypedef)
- [DimensionFilterOutputTypeDef](./type_defs.md#dimensionfilteroutputtypedef)
- [DimensionFilterTypeDef](./type_defs.md#dimensionfiltertypedef)
- [AlertSummaryTypeDef](./type_defs.md#alertsummarytypedef)
- [AnomalyDetectorConfigSummaryTypeDef](./type_defs.md#anomalydetectorconfigsummarytypedef)
- [AnomalyDetectorConfigTypeDef](./type_defs.md#anomalydetectorconfigtypedef)
- [AnomalyDetectorSummaryTypeDef](./type_defs.md#anomalydetectorsummarytypedef)
- [ItemizedMetricStatsTypeDef](./type_defs.md#itemizedmetricstatstypedef)
- [AnomalyGroupSummaryTypeDef](./type_defs.md#anomalygroupsummarytypedef)
- [AnomalyGroupTimeSeriesFeedbackTypeDef](./type_defs.md#anomalygrouptimeseriesfeedbacktypedef)
- [AnomalyGroupTimeSeriesTypeDef](./type_defs.md#anomalygrouptimeseriestypedef)
- [AppFlowConfigTypeDef](./type_defs.md#appflowconfigtypedef)
- [BackTestConfigurationTypeDef](./type_defs.md#backtestconfigurationtypedef)
- [AttributeValueTypeDef](./type_defs.md#attributevaluetypedef)
- [AutoDetectionS3SourceConfigTypeDef](./type_defs.md#autodetections3sourceconfigtypedef)
- [BackTestAnomalyDetectorRequestTypeDef](./type_defs.md#backtestanomalydetectorrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [MetricTypeDef](./type_defs.md#metrictypedef)
- [TimestampColumnTypeDef](./type_defs.md#timestampcolumntypedef)
- [CsvFormatDescriptorOutputTypeDef](./type_defs.md#csvformatdescriptoroutputtypedef)
- [CsvFormatDescriptorTypeDef](./type_defs.md#csvformatdescriptortypedef)
- [DataQualityMetricTypeDef](./type_defs.md#dataqualitymetrictypedef)
- [DeactivateAnomalyDetectorRequestTypeDef](./type_defs.md#deactivateanomalydetectorrequesttypedef)
- [DeleteAlertRequestTypeDef](./type_defs.md#deletealertrequesttypedef)
- [DeleteAnomalyDetectorRequestTypeDef](./type_defs.md#deleteanomalydetectorrequesttypedef)
- [DescribeAlertRequestTypeDef](./type_defs.md#describealertrequesttypedef)
- [DescribeAnomalyDetectionExecutionsRequestTypeDef](./type_defs.md#describeanomalydetectionexecutionsrequesttypedef)
- [ExecutionStatusTypeDef](./type_defs.md#executionstatustypedef)
- [DescribeAnomalyDetectorRequestTypeDef](./type_defs.md#describeanomalydetectorrequesttypedef)
- [DescribeMetricSetRequestTypeDef](./type_defs.md#describemetricsetrequesttypedef)
- [DimensionValueContributionTypeDef](./type_defs.md#dimensionvaluecontributiontypedef)
- [DimensionNameValueTypeDef](./type_defs.md#dimensionnamevaluetypedef)
- [JsonFormatDescriptorTypeDef](./type_defs.md#jsonformatdescriptortypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [GetAnomalyGroupRequestTypeDef](./type_defs.md#getanomalygrouprequesttypedef)
- [GetDataQualityMetricsRequestTypeDef](./type_defs.md#getdataqualitymetricsrequesttypedef)
- [TimeSeriesFeedbackTypeDef](./type_defs.md#timeseriesfeedbacktypedef)
- [InterMetricImpactDetailsTypeDef](./type_defs.md#intermetricimpactdetailstypedef)
- [ListAlertsRequestTypeDef](./type_defs.md#listalertsrequesttypedef)
- [ListAnomalyDetectorsRequestTypeDef](./type_defs.md#listanomalydetectorsrequesttypedef)
- [ListAnomalyGroupRelatedMetricsRequestTypeDef](./type_defs.md#listanomalygrouprelatedmetricsrequesttypedef)
- [ListAnomalyGroupSummariesRequestTypeDef](./type_defs.md#listanomalygroupsummariesrequesttypedef)
- [ListAnomalyGroupTimeSeriesRequestTypeDef](./type_defs.md#listanomalygrouptimeseriesrequesttypedef)
- [ListMetricSetsRequestTypeDef](./type_defs.md#listmetricsetsrequesttypedef)
- [MetricSetSummaryTypeDef](./type_defs.md#metricsetsummarytypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [VpcConfigurationOutputTypeDef](./type_defs.md#vpcconfigurationoutputtypedef)
- [VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [ActionTypeDef](./type_defs.md#actiontypedef)
- [AlertFiltersOutputTypeDef](./type_defs.md#alertfiltersoutputtypedef)
- [AlertFiltersTypeDef](./type_defs.md#alertfilterstypedef)
- [CreateAnomalyDetectorRequestTypeDef](./type_defs.md#createanomalydetectorrequesttypedef)
- [UpdateAnomalyDetectorRequestTypeDef](./type_defs.md#updateanomalydetectorrequesttypedef)
- [AnomalyGroupStatisticsTypeDef](./type_defs.md#anomalygroupstatisticstypedef)
- [PutFeedbackRequestTypeDef](./type_defs.md#putfeedbackrequesttypedef)
- [GetFeedbackRequestTypeDef](./type_defs.md#getfeedbackrequesttypedef)
- [AthenaSourceConfigTypeDef](./type_defs.md#athenasourceconfigtypedef)
- [CloudWatchConfigTypeDef](./type_defs.md#cloudwatchconfigtypedef)
- [DetectedFieldTypeDef](./type_defs.md#detectedfieldtypedef)
- [AutoDetectionMetricSourceTypeDef](./type_defs.md#autodetectionmetricsourcetypedef)
- [CreateAlertResponseTypeDef](./type_defs.md#createalertresponsetypedef)
- [CreateAnomalyDetectorResponseTypeDef](./type_defs.md#createanomalydetectorresponsetypedef)
- [CreateMetricSetResponseTypeDef](./type_defs.md#createmetricsetresponsetypedef)
- [DescribeAnomalyDetectorResponseTypeDef](./type_defs.md#describeanomalydetectorresponsetypedef)
- [GetSampleDataResponseTypeDef](./type_defs.md#getsampledataresponsetypedef)
- [ListAlertsResponseTypeDef](./type_defs.md#listalertsresponsetypedef)
- [ListAnomalyDetectorsResponseTypeDef](./type_defs.md#listanomalydetectorsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdateAlertResponseTypeDef](./type_defs.md#updatealertresponsetypedef)
- [UpdateAnomalyDetectorResponseTypeDef](./type_defs.md#updateanomalydetectorresponsetypedef)
- [UpdateMetricSetResponseTypeDef](./type_defs.md#updatemetricsetresponsetypedef)
- [CsvFormatDescriptorUnionTypeDef](./type_defs.md#csvformatdescriptoruniontypedef)
- [MetricSetDataQualityMetricTypeDef](./type_defs.md#metricsetdataqualitymetrictypedef)
- [DescribeAnomalyDetectionExecutionsResponseTypeDef](./type_defs.md#describeanomalydetectionexecutionsresponsetypedef)
- [DimensionContributionTypeDef](./type_defs.md#dimensioncontributiontypedef)
- [TimeSeriesTypeDef](./type_defs.md#timeseriestypedef)
- [FileFormatDescriptorOutputTypeDef](./type_defs.md#fileformatdescriptoroutputtypedef)
- [MetricSetDimensionFilterOutputTypeDef](./type_defs.md#metricsetdimensionfilteroutputtypedef)
- [MetricSetDimensionFilterTypeDef](./type_defs.md#metricsetdimensionfiltertypedef)
- [GetFeedbackResponseTypeDef](./type_defs.md#getfeedbackresponsetypedef)
- [ListAnomalyGroupRelatedMetricsResponseTypeDef](./type_defs.md#listanomalygrouprelatedmetricsresponsetypedef)
- [ListMetricSetsResponseTypeDef](./type_defs.md#listmetricsetsresponsetypedef)
- [RDSSourceConfigOutputTypeDef](./type_defs.md#rdssourceconfigoutputtypedef)
- [RedshiftSourceConfigOutputTypeDef](./type_defs.md#redshiftsourceconfigoutputtypedef)
- [RDSSourceConfigTypeDef](./type_defs.md#rdssourceconfigtypedef)
- [RedshiftSourceConfigTypeDef](./type_defs.md#redshiftsourceconfigtypedef)
- [AlertTypeDef](./type_defs.md#alerttypedef)
- [AlertFiltersUnionTypeDef](./type_defs.md#alertfiltersuniontypedef)
- [ListAnomalyGroupSummariesResponseTypeDef](./type_defs.md#listanomalygroupsummariesresponsetypedef)
- [DetectedCsvFormatDescriptorTypeDef](./type_defs.md#detectedcsvformatdescriptortypedef)
- [DetectedJsonFormatDescriptorTypeDef](./type_defs.md#detectedjsonformatdescriptortypedef)
- [DetectMetricSetConfigRequestTypeDef](./type_defs.md#detectmetricsetconfigrequesttypedef)
- [FileFormatDescriptorTypeDef](./type_defs.md#fileformatdescriptortypedef)
- [AnomalyDetectorDataQualityMetricTypeDef](./type_defs.md#anomalydetectordataqualitymetrictypedef)
- [ContributionMatrixTypeDef](./type_defs.md#contributionmatrixtypedef)
- [ListAnomalyGroupTimeSeriesResponseTypeDef](./type_defs.md#listanomalygrouptimeseriesresponsetypedef)
- [S3SourceConfigOutputTypeDef](./type_defs.md#s3sourceconfigoutputtypedef)
- [MetricSetDimensionFilterUnionTypeDef](./type_defs.md#metricsetdimensionfilteruniontypedef)
- [DescribeAlertResponseTypeDef](./type_defs.md#describealertresponsetypedef)
- [CreateAlertRequestTypeDef](./type_defs.md#createalertrequesttypedef)
- [UpdateAlertRequestTypeDef](./type_defs.md#updatealertrequesttypedef)
- [DetectedFileFormatDescriptorTypeDef](./type_defs.md#detectedfileformatdescriptortypedef)
- [FileFormatDescriptorUnionTypeDef](./type_defs.md#fileformatdescriptoruniontypedef)
- [S3SourceConfigTypeDef](./type_defs.md#s3sourceconfigtypedef)
- [GetDataQualityMetricsResponseTypeDef](./type_defs.md#getdataqualitymetricsresponsetypedef)
- [MetricLevelImpactTypeDef](./type_defs.md#metriclevelimpacttypedef)
- [MetricSourceOutputTypeDef](./type_defs.md#metricsourceoutputtypedef)
- [DetectedS3SourceConfigTypeDef](./type_defs.md#detecteds3sourceconfigtypedef)
- [SampleDataS3SourceConfigTypeDef](./type_defs.md#sampledatas3sourceconfigtypedef)
- [MetricSourceTypeDef](./type_defs.md#metricsourcetypedef)
- [AnomalyGroupTypeDef](./type_defs.md#anomalygrouptypedef)
- [DescribeMetricSetResponseTypeDef](./type_defs.md#describemetricsetresponsetypedef)
- [DetectedMetricSourceTypeDef](./type_defs.md#detectedmetricsourcetypedef)
- [GetSampleDataRequestTypeDef](./type_defs.md#getsampledatarequesttypedef)
- [MetricSourceUnionTypeDef](./type_defs.md#metricsourceuniontypedef)
- [GetAnomalyGroupResponseTypeDef](./type_defs.md#getanomalygroupresponsetypedef)
- [DetectedMetricSetConfigTypeDef](./type_defs.md#detectedmetricsetconfigtypedef)
- [CreateMetricSetRequestTypeDef](./type_defs.md#createmetricsetrequesttypedef)
- [UpdateMetricSetRequestTypeDef](./type_defs.md#updatemetricsetrequesttypedef)
- [DetectMetricSetConfigResponseTypeDef](./type_defs.md#detectmetricsetconfigresponsetypedef)

