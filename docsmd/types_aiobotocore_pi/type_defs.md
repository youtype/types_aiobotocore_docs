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




## DataPointTypeDef

```python
# DataPointTypeDef definition

class DataPointTypeDef(TypedDict):
    Timestamp: datetime,
    Value: float,
```

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

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
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
## GetResourceMetadataRequestRequestTypeDef

```python
# GetResourceMetadataRequestRequestTypeDef definition

class GetResourceMetadataRequestRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
## ListAvailableResourceDimensionsRequestRequestTypeDef

```python
# ListAvailableResourceDimensionsRequestRequestTypeDef definition

class ListAvailableResourceDimensionsRequestRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    Metrics: Sequence[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
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

## ResponseResourceMetricKeyTypeDef

```python
# ResponseResourceMetricKeyTypeDef definition

class ResponseResourceMetricKeyTypeDef(TypedDict):
    Metric: str,
    Dimensions: NotRequired[Dict[str, str]],
```

## MetricQueryTypeDef

```python
# MetricQueryTypeDef definition

class MetricQueryTypeDef(TypedDict):
    Metric: str,
    GroupBy: NotRequired[DimensionGroupTypeDef],  # (1)
    Filter: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DimensionGroupTypeDef](./type_defs.md#dimensiongrouptypedef) 
## DescribeDimensionKeysRequestRequestTypeDef

```python
# DescribeDimensionKeysRequestRequestTypeDef definition

class DescribeDimensionKeysRequestRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    StartTime: Union[datetime, str],
    EndTime: Union[datetime, str],
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
## DescribeDimensionKeysResponseTypeDef

```python
# DescribeDimensionKeysResponseTypeDef definition

class DescribeDimensionKeysResponseTypeDef(TypedDict):
    AlignedStartTime: datetime,
    AlignedEndTime: datetime,
    PartitionKeys: List[ResponsePartitionKeyTypeDef],  # (1)
    Keys: List[DimensionKeyDescriptionTypeDef],  # (2)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
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
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
## GetResourceMetricsRequestRequestTypeDef

```python
# GetResourceMetricsRequestRequestTypeDef definition

class GetResourceMetricsRequestRequestTypeDef(TypedDict):
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    MetricQueries: Sequence[MetricQueryTypeDef],  # (2)
    StartTime: Union[datetime, str],
    EndTime: Union[datetime, str],
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
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MetricKeyDataPointsTypeDef](./type_defs.md#metrickeydatapointstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAvailableResourceDimensionsResponseTypeDef

```python
# ListAvailableResourceDimensionsResponseTypeDef definition

class ListAvailableResourceDimensionsResponseTypeDef(TypedDict):
    MetricDimensions: List[MetricDimensionGroupsTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MetricDimensionGroupsTypeDef](./type_defs.md#metricdimensiongroupstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
