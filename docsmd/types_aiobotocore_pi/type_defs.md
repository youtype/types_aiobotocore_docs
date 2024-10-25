# Type definitions

> [Index](../README.md) > [PI](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [PI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
    type annotations stubs module [types-aiobotocore-pi](https://pypi.org/project/types-aiobotocore-pi/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## ResponseMetadataTypeDef

```python
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
# DataPointTypeDef definition

class DataPointTypeDef(TypedDict):
    Timestamp: datetime,
    Value: float,
```

## PerformanceInsightsMetricTypeDef

```python
# PerformanceInsightsMetricTypeDef definition

class PerformanceInsightsMetricTypeDef(TypedDict):
    Metric: NotRequired[str],
    DisplayName: NotRequired[str],
    Dimensions: NotRequired[Dict[str, str]],
    Value: NotRequired[float],
```

## DeletePerformanceAnalysisReportRequestRequestTypeDef

```python
# DeletePerformanceAnalysisReportRequestRequestTypeDef definition

class DeletePerformanceAnalysisReportRequestRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    AnalysisReportId: str,
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
## DimensionGroupTypeDef

```python
# DimensionGroupTypeDef definition

class DimensionGroupTypeDef(TypedDict):
    Group: str,
    Dimensions: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
```

## DimensionKeyDescriptionTypeDef

```python
# DimensionKeyDescriptionTypeDef definition

class DimensionKeyDescriptionTypeDef(TypedDict):
    Dimensions: NotRequired[Dict[str, str]],
    Total: NotRequired[float],
    AdditionalMetrics: NotRequired[Dict[str, float]],
    Partitions: NotRequired[List[float]],
```

## ResponsePartitionKeyTypeDef

```python
# ResponsePartitionKeyTypeDef definition

class ResponsePartitionKeyTypeDef(TypedDict):
    Dimensions: Dict[str, str],
```

## DimensionDetailTypeDef

```python
# DimensionDetailTypeDef definition

class DimensionDetailTypeDef(TypedDict):
    Identifier: NotRequired[str],
```

## DimensionKeyDetailTypeDef

```python
# DimensionKeyDetailTypeDef definition

class DimensionKeyDetailTypeDef(TypedDict):
    Value: NotRequired[str],
    Dimension: NotRequired[str],
    Status: NotRequired[DetailStatusType],  # (1)
```

1. See [:material-code-brackets: DetailStatusType](./literals.md#detailstatustype) 
## FeatureMetadataTypeDef

```python
# FeatureMetadataTypeDef definition

class FeatureMetadataTypeDef(TypedDict):
    Status: NotRequired[FeatureStatusType],  # (1)
```

1. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
## GetDimensionKeyDetailsRequestRequestTypeDef

```python
# GetDimensionKeyDetailsRequestRequestTypeDef definition

class GetDimensionKeyDetailsRequestRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    Group: str,
    GroupIdentifier: str,
    RequestedDimensions: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
## GetPerformanceAnalysisReportRequestRequestTypeDef

```python
# GetPerformanceAnalysisReportRequestRequestTypeDef definition

class GetPerformanceAnalysisReportRequestRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    AnalysisReportId: str,
    TextFormat: NotRequired[TextFormatType],  # (2)
    AcceptLanguage: NotRequired[AcceptLanguageType],  # (3)
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-brackets: TextFormatType](./literals.md#textformattype) 
3. See [:material-code-brackets: AcceptLanguageType](./literals.md#acceptlanguagetype) 
## GetResourceMetadataRequestRequestTypeDef

```python
# GetResourceMetadataRequestRequestTypeDef definition

class GetResourceMetadataRequestRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
## RecommendationTypeDef

```python
# RecommendationTypeDef definition

class RecommendationTypeDef(TypedDict):
    RecommendationId: NotRequired[str],
    RecommendationDescription: NotRequired[str],
```

## ListAvailableResourceDimensionsRequestRequestTypeDef

```python
# ListAvailableResourceDimensionsRequestRequestTypeDef definition

class ListAvailableResourceDimensionsRequestRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    Metrics: Sequence[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    AuthorizedActions: NotRequired[Sequence[FineGrainedActionType]],  # (2)
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-brackets: FineGrainedActionType](./literals.md#finegrainedactiontype) 
## ListAvailableResourceMetricsRequestRequestTypeDef

```python
# ListAvailableResourceMetricsRequestRequestTypeDef definition

class ListAvailableResourceMetricsRequestRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    MetricTypes: Sequence[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
## ResponseResourceMetricTypeDef

```python
# ResponseResourceMetricTypeDef definition

class ResponseResourceMetricTypeDef(TypedDict):
    Metric: NotRequired[str],
    Description: NotRequired[str],
    Unit: NotRequired[str],
```

## ListPerformanceAnalysisReportsRequestRequestTypeDef

```python
# ListPerformanceAnalysisReportsRequestRequestTypeDef definition

class ListPerformanceAnalysisReportsRequestRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ListTags: NotRequired[bool],
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    ResourceARN: str,
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
## ResponseResourceMetricKeyTypeDef

```python
# ResponseResourceMetricKeyTypeDef definition

class ResponseResourceMetricKeyTypeDef(TypedDict):
    Metric: str,
    Dimensions: NotRequired[Dict[str, str]],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    ResourceARN: str,
    TagKeys: Sequence[str],
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
## AnalysisReportSummaryTypeDef

```python
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
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (2)
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePerformanceAnalysisReportRequestRequestTypeDef

```python
# CreatePerformanceAnalysisReportRequestRequestTypeDef definition

class CreatePerformanceAnalysisReportRequestRequestTypeDef(TypedDict):
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
# CreatePerformanceAnalysisReportResponseTypeDef definition

class CreatePerformanceAnalysisReportResponseTypeDef(TypedDict):
    AnalysisReportId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataTypeDef

```python
# DataTypeDef definition

class DataTypeDef(TypedDict):
    PerformanceInsightsMetric: NotRequired[PerformanceInsightsMetricTypeDef],  # (1)
```

1. See [:material-code-braces: PerformanceInsightsMetricTypeDef](./type_defs.md#performanceinsightsmetrictypedef) 
## DescribeDimensionKeysRequestRequestTypeDef

```python
# DescribeDimensionKeysRequestRequestTypeDef definition

class DescribeDimensionKeysRequestRequestTypeDef(TypedDict):
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
# MetricQueryTypeDef definition

class MetricQueryTypeDef(TypedDict):
    Metric: str,
    GroupBy: NotRequired[DimensionGroupTypeDef],  # (1)
    Filter: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DimensionGroupTypeDef](./type_defs.md#dimensiongrouptypedef) 
## DescribeDimensionKeysResponseTypeDef

```python
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
# DimensionGroupDetailTypeDef definition

class DimensionGroupDetailTypeDef(TypedDict):
    Group: NotRequired[str],
    Dimensions: NotRequired[List[DimensionDetailTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionDetailTypeDef](./type_defs.md#dimensiondetailtypedef) 
## GetDimensionKeyDetailsResponseTypeDef

```python
# GetDimensionKeyDetailsResponseTypeDef definition

class GetDimensionKeyDetailsResponseTypeDef(TypedDict):
    Dimensions: List[DimensionKeyDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DimensionKeyDetailTypeDef](./type_defs.md#dimensionkeydetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourceMetadataResponseTypeDef

```python
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
# MetricKeyDataPointsTypeDef definition

class MetricKeyDataPointsTypeDef(TypedDict):
    Key: NotRequired[ResponseResourceMetricKeyTypeDef],  # (1)
    DataPoints: NotRequired[List[DataPointTypeDef]],  # (2)
```

1. See [:material-code-braces: ResponseResourceMetricKeyTypeDef](./type_defs.md#responseresourcemetrickeytypedef) 
2. See [:material-code-braces: DataPointTypeDef](./type_defs.md#datapointtypedef) 
## ListPerformanceAnalysisReportsResponseTypeDef

```python
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
## GetResourceMetricsRequestRequestTypeDef

```python
# GetResourceMetricsRequestRequestTypeDef definition

class GetResourceMetricsRequestRequestTypeDef(TypedDict):
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
# MetricDimensionGroupsTypeDef definition

class MetricDimensionGroupsTypeDef(TypedDict):
    Metric: NotRequired[str],
    Groups: NotRequired[List[DimensionGroupDetailTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionGroupDetailTypeDef](./type_defs.md#dimensiongroupdetailtypedef) 
## GetResourceMetricsResponseTypeDef

```python
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
# GetPerformanceAnalysisReportResponseTypeDef definition

class GetPerformanceAnalysisReportResponseTypeDef(TypedDict):
    AnalysisReport: AnalysisReportTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalysisReportTypeDef](./type_defs.md#analysisreporttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
