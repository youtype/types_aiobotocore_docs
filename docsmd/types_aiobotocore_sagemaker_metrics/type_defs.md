# Type definitions

> [Index](../README.md) > [SageMakerMetrics](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SageMakerMetrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
    type annotations stubs module [types-aiobotocore-sagemaker-metrics](https://pypi.org/project/types-aiobotocore-sagemaker-metrics/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## BatchPutMetricsErrorTypeDef

```python
# BatchPutMetricsErrorTypeDef definition

class BatchPutMetricsErrorTypeDef(TypedDict):
    Code: NotRequired[PutMetricsErrorCodeType],  # (1)
    MetricIndex: NotRequired[int],
```

1. See [:material-code-brackets: PutMetricsErrorCodeType](./literals.md#putmetricserrorcodetype) 
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
    Timestamp: Union[datetime, str],
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
