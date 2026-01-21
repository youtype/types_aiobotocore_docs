# PI module

> [Index](../README.md) > PI


!!! note ""

    Auto-generated documentation for [PI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#pi)
    type annotations stubs module [types-aiobotocore-pi](https://pypi.org/project/types-aiobotocore-pi/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `PI` service.
1. Use provided commands to install generated packages.



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
- [DeletePerformanceAnalysisReportRequestTypeDef](./type_defs.md#deleteperformanceanalysisreportrequesttypedef)
- [DimensionGroupTypeDef](./type_defs.md#dimensiongrouptypedef)
- [DimensionKeyDescriptionTypeDef](./type_defs.md#dimensionkeydescriptiontypedef)
- [ResponsePartitionKeyTypeDef](./type_defs.md#responsepartitionkeytypedef)
- [DimensionDetailTypeDef](./type_defs.md#dimensiondetailtypedef)
- [DimensionKeyDetailTypeDef](./type_defs.md#dimensionkeydetailtypedef)
- [FeatureMetadataTypeDef](./type_defs.md#featuremetadatatypedef)
- [GetDimensionKeyDetailsRequestTypeDef](./type_defs.md#getdimensionkeydetailsrequesttypedef)
- [GetPerformanceAnalysisReportRequestTypeDef](./type_defs.md#getperformanceanalysisreportrequesttypedef)
- [GetResourceMetadataRequestTypeDef](./type_defs.md#getresourcemetadatarequesttypedef)
- [RecommendationTypeDef](./type_defs.md#recommendationtypedef)
- [ListAvailableResourceDimensionsRequestTypeDef](./type_defs.md#listavailableresourcedimensionsrequesttypedef)
- [ListAvailableResourceMetricsRequestTypeDef](./type_defs.md#listavailableresourcemetricsrequesttypedef)
- [ResponseResourceMetricTypeDef](./type_defs.md#responseresourcemetrictypedef)
- [ListPerformanceAnalysisReportsRequestTypeDef](./type_defs.md#listperformanceanalysisreportsrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [ResponseResourceMetricKeyTypeDef](./type_defs.md#responseresourcemetrickeytypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [AnalysisReportSummaryTypeDef](./type_defs.md#analysisreportsummarytypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [CreatePerformanceAnalysisReportRequestTypeDef](./type_defs.md#createperformanceanalysisreportrequesttypedef)
- [CreatePerformanceAnalysisReportResponseTypeDef](./type_defs.md#createperformanceanalysisreportresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [DataTypeDef](./type_defs.md#datatypedef)
- [DescribeDimensionKeysRequestTypeDef](./type_defs.md#describedimensionkeysrequesttypedef)
- [MetricQueryTypeDef](./type_defs.md#metricquerytypedef)
- [DescribeDimensionKeysResponseTypeDef](./type_defs.md#describedimensionkeysresponsetypedef)
- [DimensionGroupDetailTypeDef](./type_defs.md#dimensiongroupdetailtypedef)
- [GetDimensionKeyDetailsResponseTypeDef](./type_defs.md#getdimensionkeydetailsresponsetypedef)
- [GetResourceMetadataResponseTypeDef](./type_defs.md#getresourcemetadataresponsetypedef)
- [ListAvailableResourceMetricsResponseTypeDef](./type_defs.md#listavailableresourcemetricsresponsetypedef)
- [MetricKeyDataPointsTypeDef](./type_defs.md#metrickeydatapointstypedef)
- [ListPerformanceAnalysisReportsResponseTypeDef](./type_defs.md#listperformanceanalysisreportsresponsetypedef)
- [InsightTypeDef](./type_defs.md#insighttypedef)
- [GetResourceMetricsRequestTypeDef](./type_defs.md#getresourcemetricsrequesttypedef)
- [MetricDimensionGroupsTypeDef](./type_defs.md#metricdimensiongroupstypedef)
- [GetResourceMetricsResponseTypeDef](./type_defs.md#getresourcemetricsresponsetypedef)
- [AnalysisReportTypeDef](./type_defs.md#analysisreporttypedef)
- [ListAvailableResourceDimensionsResponseTypeDef](./type_defs.md#listavailableresourcedimensionsresponsetypedef)
- [GetPerformanceAnalysisReportResponseTypeDef](./type_defs.md#getperformanceanalysisreportresponsetypedef)

