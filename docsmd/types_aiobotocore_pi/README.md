# PI module

> [Index](../README.md) > PI


!!! note ""

    Auto-generated documentation for [PI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
    type annotations stubs module [types-aiobotocore-pi](https://pypi.org/project/types-aiobotocore-pi/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `PI` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[pi]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[pi]'


# standalone installation
python -m pip install types-aiobotocore-pi
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-pi
```

## Usage

Code samples can be found in [Examples](./usage.md).

## PIClient

Type annotations and code completion for  `#!python session.create_client("pi")` as [PIClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client)

```python
# PIClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_pi.client import PIClient


session = get_session()
async with session.create_client("pi") as client:
    client: PIClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AcceptLanguageType usage example

from types_aiobotocore_pi.literals import AcceptLanguageType

def get_value() -> AcceptLanguageType:
    return "EN_US"
```

- [AcceptLanguageType](./literals.md#acceptlanguagetype)
- [AnalysisStatusType](./literals.md#analysisstatustype)
- [ContextTypeType](./literals.md#contexttypetype)
- [DetailStatusType](./literals.md#detailstatustype)
- [FeatureStatusType](./literals.md#featurestatustype)
- [FineGrainedActionType](./literals.md#finegrainedactiontype)
- [PeriodAlignmentType](./literals.md#periodalignmenttype)
- [ServiceTypeType](./literals.md#servicetypetype)
- [SeverityType](./literals.md#severitytype)
- [TextFormatType](./literals.md#textformattype)
- [PIServiceName](./literals.md#piservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [TagTypeDef](./type_defs.md#tagtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DataPointTypeDef](./type_defs.md#datapointtypedef)
- [PerformanceInsightsMetricTypeDef](./type_defs.md#performanceinsightsmetrictypedef)
- [DeletePerformanceAnalysisReportRequestRequestTypeDef](./type_defs.md#deleteperformanceanalysisreportrequestrequesttypedef)
- [DimensionGroupTypeDef](./type_defs.md#dimensiongrouptypedef)
- [DimensionKeyDescriptionTypeDef](./type_defs.md#dimensionkeydescriptiontypedef)
- [ResponsePartitionKeyTypeDef](./type_defs.md#responsepartitionkeytypedef)
- [DimensionDetailTypeDef](./type_defs.md#dimensiondetailtypedef)
- [DimensionKeyDetailTypeDef](./type_defs.md#dimensionkeydetailtypedef)
- [FeatureMetadataTypeDef](./type_defs.md#featuremetadatatypedef)
- [GetDimensionKeyDetailsRequestRequestTypeDef](./type_defs.md#getdimensionkeydetailsrequestrequesttypedef)
- [GetPerformanceAnalysisReportRequestRequestTypeDef](./type_defs.md#getperformanceanalysisreportrequestrequesttypedef)
- [GetResourceMetadataRequestRequestTypeDef](./type_defs.md#getresourcemetadatarequestrequesttypedef)
- [RecommendationTypeDef](./type_defs.md#recommendationtypedef)
- [ListAvailableResourceDimensionsRequestRequestTypeDef](./type_defs.md#listavailableresourcedimensionsrequestrequesttypedef)
- [ListAvailableResourceMetricsRequestRequestTypeDef](./type_defs.md#listavailableresourcemetricsrequestrequesttypedef)
- [ResponseResourceMetricTypeDef](./type_defs.md#responseresourcemetrictypedef)
- [ListPerformanceAnalysisReportsRequestRequestTypeDef](./type_defs.md#listperformanceanalysisreportsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ResponseResourceMetricKeyTypeDef](./type_defs.md#responseresourcemetrickeytypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [AnalysisReportSummaryTypeDef](./type_defs.md#analysisreportsummarytypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreatePerformanceAnalysisReportRequestRequestTypeDef](./type_defs.md#createperformanceanalysisreportrequestrequesttypedef)
- [CreatePerformanceAnalysisReportResponseTypeDef](./type_defs.md#createperformanceanalysisreportresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [DataTypeDef](./type_defs.md#datatypedef)
- [DescribeDimensionKeysRequestRequestTypeDef](./type_defs.md#describedimensionkeysrequestrequesttypedef)
- [MetricQueryTypeDef](./type_defs.md#metricquerytypedef)
- [DescribeDimensionKeysResponseTypeDef](./type_defs.md#describedimensionkeysresponsetypedef)
- [DimensionGroupDetailTypeDef](./type_defs.md#dimensiongroupdetailtypedef)
- [GetDimensionKeyDetailsResponseTypeDef](./type_defs.md#getdimensionkeydetailsresponsetypedef)
- [GetResourceMetadataResponseTypeDef](./type_defs.md#getresourcemetadataresponsetypedef)
- [ListAvailableResourceMetricsResponseTypeDef](./type_defs.md#listavailableresourcemetricsresponsetypedef)
- [MetricKeyDataPointsTypeDef](./type_defs.md#metrickeydatapointstypedef)
- [ListPerformanceAnalysisReportsResponseTypeDef](./type_defs.md#listperformanceanalysisreportsresponsetypedef)
- [InsightTypeDef](./type_defs.md#insighttypedef)
- [GetResourceMetricsRequestRequestTypeDef](./type_defs.md#getresourcemetricsrequestrequesttypedef)
- [MetricDimensionGroupsTypeDef](./type_defs.md#metricdimensiongroupstypedef)
- [GetResourceMetricsResponseTypeDef](./type_defs.md#getresourcemetricsresponsetypedef)
- [AnalysisReportTypeDef](./type_defs.md#analysisreporttypedef)
- [ListAvailableResourceDimensionsResponseTypeDef](./type_defs.md#listavailableresourcedimensionsresponsetypedef)
- [GetPerformanceAnalysisReportResponseTypeDef](./type_defs.md#getperformanceanalysisreportresponsetypedef)

