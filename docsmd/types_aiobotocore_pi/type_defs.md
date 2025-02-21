# Type definitions

> [Index](../README.md) > [PI](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [PI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#pi)
    type annotations stubs module [types-aiobotocore-pi](https://pypi.org/project/types-aiobotocore-pi/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_pi.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "Key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## DataPointTypeDef

```python
# DataPointTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import DataPointTypeDef


def get_value() -> DataPointTypeDef:
    return {
        "Timestamp": ...,
    }


# DataPointTypeDef definition

class DataPointTypeDef(TypedDict):
    Timestamp: datetime,
    Value: float,
```

## PerformanceInsightsMetricTypeDef

```python
# PerformanceInsightsMetricTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import PerformanceInsightsMetricTypeDef


def get_value() -> PerformanceInsightsMetricTypeDef:
    return {
        "Metric": ...,
    }


# PerformanceInsightsMetricTypeDef definition

class PerformanceInsightsMetricTypeDef(TypedDict):
    Metric: NotRequired[str],
    DisplayName: NotRequired[str],
    Dimensions: NotRequired[Dict[str, str]],
    Filter: NotRequired[Dict[str, str]],
    Value: NotRequired[float],
```

## DeletePerformanceAnalysisReportRequestTypeDef

```python
# DeletePerformanceAnalysisReportRequestTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import DeletePerformanceAnalysisReportRequestTypeDef


def get_value() -> DeletePerformanceAnalysisReportRequestTypeDef:
    return {
        "ServiceType": ...,
    }


# DeletePerformanceAnalysisReportRequestTypeDef definition

class DeletePerformanceAnalysisReportRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    AnalysisReportId: str,
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
## DimensionGroupTypeDef

```python
# DimensionGroupTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import DimensionGroupTypeDef


def get_value() -> DimensionGroupTypeDef:
    return {
        "Group": ...,
    }


# DimensionGroupTypeDef definition

class DimensionGroupTypeDef(TypedDict):
    Group: str,
    Dimensions: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
```

## DimensionKeyDescriptionTypeDef

```python
# DimensionKeyDescriptionTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import DimensionKeyDescriptionTypeDef


def get_value() -> DimensionKeyDescriptionTypeDef:
    return {
        "Dimensions": ...,
    }


# DimensionKeyDescriptionTypeDef definition

class DimensionKeyDescriptionTypeDef(TypedDict):
    Dimensions: NotRequired[Dict[str, str]],
    Total: NotRequired[float],
    AdditionalMetrics: NotRequired[Dict[str, float]],
    Partitions: NotRequired[List[float]],
```

## ResponsePartitionKeyTypeDef

```python
# ResponsePartitionKeyTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import ResponsePartitionKeyTypeDef


def get_value() -> ResponsePartitionKeyTypeDef:
    return {
        "Dimensions": ...,
    }


# ResponsePartitionKeyTypeDef definition

class ResponsePartitionKeyTypeDef(TypedDict):
    Dimensions: Dict[str, str],
```

## DimensionDetailTypeDef

```python
# DimensionDetailTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import DimensionDetailTypeDef


def get_value() -> DimensionDetailTypeDef:
    return {
        "Identifier": ...,
    }


# DimensionDetailTypeDef definition

class DimensionDetailTypeDef(TypedDict):
    Identifier: NotRequired[str],
```

## DimensionKeyDetailTypeDef

```python
# DimensionKeyDetailTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import DimensionKeyDetailTypeDef


def get_value() -> DimensionKeyDetailTypeDef:
    return {
        "Value": ...,
    }


# DimensionKeyDetailTypeDef definition

class DimensionKeyDetailTypeDef(TypedDict):
    Value: NotRequired[str],
    Dimension: NotRequired[str],
    Status: NotRequired[DetailStatusType],  # (1)
```

1. See [:material-code-brackets: DetailStatusType](./literals.md#detailstatustype) 
## FeatureMetadataTypeDef

```python
# FeatureMetadataTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import FeatureMetadataTypeDef


def get_value() -> FeatureMetadataTypeDef:
    return {
        "Status": ...,
    }


# FeatureMetadataTypeDef definition

class FeatureMetadataTypeDef(TypedDict):
    Status: NotRequired[FeatureStatusType],  # (1)
```

1. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
## GetDimensionKeyDetailsRequestTypeDef

```python
# GetDimensionKeyDetailsRequestTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import GetDimensionKeyDetailsRequestTypeDef


def get_value() -> GetDimensionKeyDetailsRequestTypeDef:
    return {
        "ServiceType": ...,
    }


# GetDimensionKeyDetailsRequestTypeDef definition

class GetDimensionKeyDetailsRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    Group: str,
    GroupIdentifier: str,
    RequestedDimensions: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
## GetPerformanceAnalysisReportRequestTypeDef

```python
# GetPerformanceAnalysisReportRequestTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import GetPerformanceAnalysisReportRequestTypeDef


def get_value() -> GetPerformanceAnalysisReportRequestTypeDef:
    return {
        "ServiceType": ...,
    }


# GetPerformanceAnalysisReportRequestTypeDef definition

class GetPerformanceAnalysisReportRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    AnalysisReportId: str,
    TextFormat: NotRequired[TextFormatType],  # (2)
    AcceptLanguage: NotRequired[AcceptLanguageType],  # (3)
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-brackets: TextFormatType](./literals.md#textformattype) 
3. See [:material-code-brackets: AcceptLanguageType](./literals.md#acceptlanguagetype) 
## GetResourceMetadataRequestTypeDef

```python
# GetResourceMetadataRequestTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import GetResourceMetadataRequestTypeDef


def get_value() -> GetResourceMetadataRequestTypeDef:
    return {
        "ServiceType": ...,
    }


# GetResourceMetadataRequestTypeDef definition

class GetResourceMetadataRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
## RecommendationTypeDef

```python
# RecommendationTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import RecommendationTypeDef


def get_value() -> RecommendationTypeDef:
    return {
        "RecommendationId": ...,
    }


# RecommendationTypeDef definition

class RecommendationTypeDef(TypedDict):
    RecommendationId: NotRequired[str],
    RecommendationDescription: NotRequired[str],
```

## ListAvailableResourceDimensionsRequestTypeDef

```python
# ListAvailableResourceDimensionsRequestTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import ListAvailableResourceDimensionsRequestTypeDef


def get_value() -> ListAvailableResourceDimensionsRequestTypeDef:
    return {
        "ServiceType": ...,
    }


# ListAvailableResourceDimensionsRequestTypeDef definition

class ListAvailableResourceDimensionsRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    Metrics: Sequence[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    AuthorizedActions: NotRequired[Sequence[FineGrainedActionType]],  # (2)
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-brackets: FineGrainedActionType](./literals.md#finegrainedactiontype) 
## ListAvailableResourceMetricsRequestTypeDef

```python
# ListAvailableResourceMetricsRequestTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import ListAvailableResourceMetricsRequestTypeDef


def get_value() -> ListAvailableResourceMetricsRequestTypeDef:
    return {
        "ServiceType": ...,
    }


# ListAvailableResourceMetricsRequestTypeDef definition

class ListAvailableResourceMetricsRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    MetricTypes: Sequence[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
## ResponseResourceMetricTypeDef

```python
# ResponseResourceMetricTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import ResponseResourceMetricTypeDef


def get_value() -> ResponseResourceMetricTypeDef:
    return {
        "Metric": ...,
    }


# ResponseResourceMetricTypeDef definition

class ResponseResourceMetricTypeDef(TypedDict):
    Metric: NotRequired[str],
    Description: NotRequired[str],
    Unit: NotRequired[str],
```

## ListPerformanceAnalysisReportsRequestTypeDef

```python
# ListPerformanceAnalysisReportsRequestTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import ListPerformanceAnalysisReportsRequestTypeDef


def get_value() -> ListPerformanceAnalysisReportsRequestTypeDef:
    return {
        "ServiceType": ...,
    }


# ListPerformanceAnalysisReportsRequestTypeDef definition

class ListPerformanceAnalysisReportsRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ListTags: NotRequired[bool],
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "ServiceType": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    ResourceARN: str,
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
## ResponseResourceMetricKeyTypeDef

```python
# ResponseResourceMetricKeyTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import ResponseResourceMetricKeyTypeDef


def get_value() -> ResponseResourceMetricKeyTypeDef:
    return {
        "Metric": ...,
    }


# ResponseResourceMetricKeyTypeDef definition

class ResponseResourceMetricKeyTypeDef(TypedDict):
    Metric: str,
    Dimensions: NotRequired[Dict[str, str]],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ServiceType": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    ResourceARN: str,
    TagKeys: Sequence[str],
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
## AnalysisReportSummaryTypeDef

```python
# AnalysisReportSummaryTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import AnalysisReportSummaryTypeDef


def get_value() -> AnalysisReportSummaryTypeDef:
    return {
        "AnalysisReportId": ...,
    }


# AnalysisReportSummaryTypeDef definition

class AnalysisReportSummaryTypeDef(TypedDict):
    AnalysisReportId: NotRequired[str],
    CreateTime: NotRequired[datetime],
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    Status: NotRequired[AnalysisStatusType],  # (1)
    Tags: NotRequired[List[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: AnalysisStatusType](./literals.md#analysisstatustype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "ServiceType": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (2)
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePerformanceAnalysisReportRequestTypeDef

```python
# CreatePerformanceAnalysisReportRequestTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import CreatePerformanceAnalysisReportRequestTypeDef


def get_value() -> CreatePerformanceAnalysisReportRequestTypeDef:
    return {
        "ServiceType": ...,
    }


# CreatePerformanceAnalysisReportRequestTypeDef definition

class CreatePerformanceAnalysisReportRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePerformanceAnalysisReportResponseTypeDef

```python
# CreatePerformanceAnalysisReportResponseTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import CreatePerformanceAnalysisReportResponseTypeDef


def get_value() -> CreatePerformanceAnalysisReportResponseTypeDef:
    return {
        "AnalysisReportId": ...,
    }


# CreatePerformanceAnalysisReportResponseTypeDef definition

class CreatePerformanceAnalysisReportResponseTypeDef(TypedDict):
    AnalysisReportId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataTypeDef

```python
# DataTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import DataTypeDef


def get_value() -> DataTypeDef:
    return {
        "PerformanceInsightsMetric": ...,
    }


# DataTypeDef definition

class DataTypeDef(TypedDict):
    PerformanceInsightsMetric: NotRequired[PerformanceInsightsMetricTypeDef],  # (1)
```

1. See [:material-code-braces: PerformanceInsightsMetricTypeDef](./type_defs.md#performanceinsightsmetrictypedef) 
## DescribeDimensionKeysRequestTypeDef

```python
# DescribeDimensionKeysRequestTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import DescribeDimensionKeysRequestTypeDef


def get_value() -> DescribeDimensionKeysRequestTypeDef:
    return {
        "ServiceType": ...,
    }


# DescribeDimensionKeysRequestTypeDef definition

class DescribeDimensionKeysRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    Metric: str,
    GroupBy: DimensionGroupTypeDef,  # (2)
    PeriodInSeconds: NotRequired[int],
    AdditionalMetrics: NotRequired[Sequence[str]],
    PartitionBy: NotRequired[DimensionGroupTypeDef],  # (2)
    Filter: NotRequired[Mapping[str, str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-braces: DimensionGroupTypeDef](./type_defs.md#dimensiongrouptypedef) 
3. See [:material-code-braces: DimensionGroupTypeDef](./type_defs.md#dimensiongrouptypedef) 
## MetricQueryTypeDef

```python
# MetricQueryTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import MetricQueryTypeDef


def get_value() -> MetricQueryTypeDef:
    return {
        "Metric": ...,
    }


# MetricQueryTypeDef definition

class MetricQueryTypeDef(TypedDict):
    Metric: str,
    GroupBy: NotRequired[DimensionGroupTypeDef],  # (1)
    Filter: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DimensionGroupTypeDef](./type_defs.md#dimensiongrouptypedef) 
## DescribeDimensionKeysResponseTypeDef

```python
# DescribeDimensionKeysResponseTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import DescribeDimensionKeysResponseTypeDef


def get_value() -> DescribeDimensionKeysResponseTypeDef:
    return {
        "AlignedStartTime": ...,
    }


# DescribeDimensionKeysResponseTypeDef definition

class DescribeDimensionKeysResponseTypeDef(TypedDict):
    AlignedStartTime: datetime,
    AlignedEndTime: datetime,
    PartitionKeys: List[ResponsePartitionKeyTypeDef],  # (1)
    Keys: List[DimensionKeyDescriptionTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponsePartitionKeyTypeDef](./type_defs.md#responsepartitionkeytypedef) 
2. See [:material-code-braces: DimensionKeyDescriptionTypeDef](./type_defs.md#dimensionkeydescriptiontypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DimensionGroupDetailTypeDef

```python
# DimensionGroupDetailTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import DimensionGroupDetailTypeDef


def get_value() -> DimensionGroupDetailTypeDef:
    return {
        "Group": ...,
    }


# DimensionGroupDetailTypeDef definition

class DimensionGroupDetailTypeDef(TypedDict):
    Group: NotRequired[str],
    Dimensions: NotRequired[List[DimensionDetailTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionDetailTypeDef](./type_defs.md#dimensiondetailtypedef) 
## GetDimensionKeyDetailsResponseTypeDef

```python
# GetDimensionKeyDetailsResponseTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import GetDimensionKeyDetailsResponseTypeDef


def get_value() -> GetDimensionKeyDetailsResponseTypeDef:
    return {
        "Dimensions": ...,
    }


# GetDimensionKeyDetailsResponseTypeDef definition

class GetDimensionKeyDetailsResponseTypeDef(TypedDict):
    Dimensions: List[DimensionKeyDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DimensionKeyDetailTypeDef](./type_defs.md#dimensionkeydetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourceMetadataResponseTypeDef

```python
# GetResourceMetadataResponseTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import GetResourceMetadataResponseTypeDef


def get_value() -> GetResourceMetadataResponseTypeDef:
    return {
        "Identifier": ...,
    }


# GetResourceMetadataResponseTypeDef definition

class GetResourceMetadataResponseTypeDef(TypedDict):
    Identifier: str,
    Features: Dict[str, FeatureMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FeatureMetadataTypeDef](./type_defs.md#featuremetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAvailableResourceMetricsResponseTypeDef

```python
# ListAvailableResourceMetricsResponseTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import ListAvailableResourceMetricsResponseTypeDef


def get_value() -> ListAvailableResourceMetricsResponseTypeDef:
    return {
        "Metrics": ...,
    }


# ListAvailableResourceMetricsResponseTypeDef definition

class ListAvailableResourceMetricsResponseTypeDef(TypedDict):
    Metrics: List[ResponseResourceMetricTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseResourceMetricTypeDef](./type_defs.md#responseresourcemetrictypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricKeyDataPointsTypeDef

```python
# MetricKeyDataPointsTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import MetricKeyDataPointsTypeDef


def get_value() -> MetricKeyDataPointsTypeDef:
    return {
        "Key": ...,
    }


# MetricKeyDataPointsTypeDef definition

class MetricKeyDataPointsTypeDef(TypedDict):
    Key: NotRequired[ResponseResourceMetricKeyTypeDef],  # (1)
    DataPoints: NotRequired[List[DataPointTypeDef]],  # (2)
```

1. See [:material-code-braces: ResponseResourceMetricKeyTypeDef](./type_defs.md#responseresourcemetrickeytypedef) 
2. See [:material-code-braces: DataPointTypeDef](./type_defs.md#datapointtypedef) 
## ListPerformanceAnalysisReportsResponseTypeDef

```python
# ListPerformanceAnalysisReportsResponseTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import ListPerformanceAnalysisReportsResponseTypeDef


def get_value() -> ListPerformanceAnalysisReportsResponseTypeDef:
    return {
        "AnalysisReports": ...,
    }


# ListPerformanceAnalysisReportsResponseTypeDef definition

class ListPerformanceAnalysisReportsResponseTypeDef(TypedDict):
    AnalysisReports: List[AnalysisReportSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AnalysisReportSummaryTypeDef](./type_defs.md#analysisreportsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InsightTypeDef

```python
# InsightTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import InsightTypeDef


def get_value() -> InsightTypeDef:
    return {
        "InsightId": ...,
    }


# InsightTypeDef definition

class InsightTypeDef(TypedDict):
    InsightId: str,
    InsightType: NotRequired[str],
    Context: NotRequired[ContextTypeType],  # (1)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    Severity: NotRequired[SeverityType],  # (2)
    SupportingInsights: NotRequired[List[Dict[str, Any]]],
    Description: NotRequired[str],
    Recommendations: NotRequired[List[RecommendationTypeDef]],  # (3)
    InsightData: NotRequired[List[DataTypeDef]],  # (4)
    BaselineData: NotRequired[List[DataTypeDef]],  # (4)
```

1. See [:material-code-brackets: ContextTypeType](./literals.md#contexttypetype) 
2. See [:material-code-brackets: SeverityType](./literals.md#severitytype) 
3. See [:material-code-braces: RecommendationTypeDef](./type_defs.md#recommendationtypedef) 
4. See [:material-code-braces: DataTypeDef](./type_defs.md#datatypedef) 
5. See [:material-code-braces: DataTypeDef](./type_defs.md#datatypedef) 
## GetResourceMetricsRequestTypeDef

```python
# GetResourceMetricsRequestTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import GetResourceMetricsRequestTypeDef


def get_value() -> GetResourceMetricsRequestTypeDef:
    return {
        "ServiceType": ...,
    }


# GetResourceMetricsRequestTypeDef definition

class GetResourceMetricsRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    MetricQueries: Sequence[MetricQueryTypeDef],  # (2)
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    PeriodInSeconds: NotRequired[int],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    PeriodAlignment: NotRequired[PeriodAlignmentType],  # (3)
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-braces: MetricQueryTypeDef](./type_defs.md#metricquerytypedef) 
3. See [:material-code-brackets: PeriodAlignmentType](./literals.md#periodalignmenttype) 
## MetricDimensionGroupsTypeDef

```python
# MetricDimensionGroupsTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import MetricDimensionGroupsTypeDef


def get_value() -> MetricDimensionGroupsTypeDef:
    return {
        "Metric": ...,
    }


# MetricDimensionGroupsTypeDef definition

class MetricDimensionGroupsTypeDef(TypedDict):
    Metric: NotRequired[str],
    Groups: NotRequired[List[DimensionGroupDetailTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionGroupDetailTypeDef](./type_defs.md#dimensiongroupdetailtypedef) 
## GetResourceMetricsResponseTypeDef

```python
# GetResourceMetricsResponseTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import GetResourceMetricsResponseTypeDef


def get_value() -> GetResourceMetricsResponseTypeDef:
    return {
        "AlignedStartTime": ...,
    }


# GetResourceMetricsResponseTypeDef definition

class GetResourceMetricsResponseTypeDef(TypedDict):
    AlignedStartTime: datetime,
    AlignedEndTime: datetime,
    Identifier: str,
    MetricList: List[MetricKeyDataPointsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MetricKeyDataPointsTypeDef](./type_defs.md#metrickeydatapointstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AnalysisReportTypeDef

```python
# AnalysisReportTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import AnalysisReportTypeDef


def get_value() -> AnalysisReportTypeDef:
    return {
        "AnalysisReportId": ...,
    }


# AnalysisReportTypeDef definition

class AnalysisReportTypeDef(TypedDict):
    AnalysisReportId: str,
    Identifier: NotRequired[str],
    ServiceType: NotRequired[ServiceTypeType],  # (1)
    CreateTime: NotRequired[datetime],
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    Status: NotRequired[AnalysisStatusType],  # (2)
    Insights: NotRequired[List[InsightTypeDef]],  # (3)
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-brackets: AnalysisStatusType](./literals.md#analysisstatustype) 
3. See [:material-code-braces: InsightTypeDef](./type_defs.md#insighttypedef) 
## ListAvailableResourceDimensionsResponseTypeDef

```python
# ListAvailableResourceDimensionsResponseTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import ListAvailableResourceDimensionsResponseTypeDef


def get_value() -> ListAvailableResourceDimensionsResponseTypeDef:
    return {
        "MetricDimensions": ...,
    }


# ListAvailableResourceDimensionsResponseTypeDef definition

class ListAvailableResourceDimensionsResponseTypeDef(TypedDict):
    MetricDimensions: List[MetricDimensionGroupsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MetricDimensionGroupsTypeDef](./type_defs.md#metricdimensiongroupstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPerformanceAnalysisReportResponseTypeDef

```python
# GetPerformanceAnalysisReportResponseTypeDef TypedDict usage example

from types_aiobotocore_pi.type_defs import GetPerformanceAnalysisReportResponseTypeDef


def get_value() -> GetPerformanceAnalysisReportResponseTypeDef:
    return {
        "AnalysisReport": ...,
    }


# GetPerformanceAnalysisReportResponseTypeDef definition

class GetPerformanceAnalysisReportResponseTypeDef(TypedDict):
    AnalysisReport: AnalysisReportTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalysisReportTypeDef](./type_defs.md#analysisreporttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
