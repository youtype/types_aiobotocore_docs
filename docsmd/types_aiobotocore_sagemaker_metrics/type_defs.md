# Type definitions

> [Index](../README.md) > [SageMakerMetrics](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SageMakerMetrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#sagemakermetrics)
    type annotations stubs module [types-aiobotocore-sagemaker-metrics](https://pypi.org/project/types-aiobotocore-sagemaker-metrics/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## MetricQueryTypeDef

```python
# MetricQueryTypeDef definition

class MetricQueryTypeDef(TypedDict):
    MetricName: str,
    ResourceArn: str,
    MetricStat: MetricStatisticType,  # (1)
    Period: PeriodType,  # (2)
    XAxisType: XAxisTypeType,  # (3)
    Start: NotRequired[int],
    End: NotRequired[int],
```

1. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
2. See [:material-code-brackets: PeriodType](./literals.md#periodtype) 
3. See [:material-code-brackets: XAxisTypeType](./literals.md#xaxistypetype) 
## MetricQueryResultTypeDef

```python
# MetricQueryResultTypeDef definition

class MetricQueryResultTypeDef(TypedDict):
    Status: MetricQueryResultStatusType,  # (1)
    XAxisValues: List[int],
    MetricValues: List[float],
    Message: NotRequired[str],
```

1. See [:material-code-brackets: MetricQueryResultStatusType](./literals.md#metricqueryresultstatustype) 
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

## BatchPutMetricsErrorTypeDef

```python
# BatchPutMetricsErrorTypeDef definition

class BatchPutMetricsErrorTypeDef(TypedDict):
    Code: NotRequired[PutMetricsErrorCodeType],  # (1)
    MetricIndex: NotRequired[int],
```

1. See [:material-code-brackets: PutMetricsErrorCodeType](./literals.md#putmetricserrorcodetype) 
## BatchGetMetricsRequestRequestTypeDef

```python
# BatchGetMetricsRequestRequestTypeDef definition

class BatchGetMetricsRequestRequestTypeDef(TypedDict):
    MetricQueries: Sequence[MetricQueryTypeDef],  # (1)
```

1. See [:material-code-braces: MetricQueryTypeDef](./type_defs.md#metricquerytypedef) 
## BatchGetMetricsResponseTypeDef

```python
# BatchGetMetricsResponseTypeDef definition

class BatchGetMetricsResponseTypeDef(TypedDict):
    MetricQueryResults: List[MetricQueryResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MetricQueryResultTypeDef](./type_defs.md#metricqueryresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchPutMetricsResponseTypeDef

```python
# BatchPutMetricsResponseTypeDef definition

class BatchPutMetricsResponseTypeDef(TypedDict):
    Errors: List[BatchPutMetricsErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchPutMetricsErrorTypeDef](./type_defs.md#batchputmetricserrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RawMetricDataTypeDef

```python
# RawMetricDataTypeDef definition

class RawMetricDataTypeDef(TypedDict):
    MetricName: str,
    Timestamp: TimestampTypeDef,
    Value: float,
    Step: NotRequired[int],
```

## BatchPutMetricsRequestRequestTypeDef

```python
# BatchPutMetricsRequestRequestTypeDef definition

class BatchPutMetricsRequestRequestTypeDef(TypedDict):
    TrialComponentName: str,
    MetricData: Sequence[RawMetricDataTypeDef],  # (1)
```

1. See [:material-code-braces: RawMetricDataTypeDef](./type_defs.md#rawmetricdatatypedef) 
