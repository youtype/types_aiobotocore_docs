# Examples

> [Index](../README.md) > [SageMakerMetrics](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SageMakerMetrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#sagemakermetrics)
    type annotations stubs module [types-aiobotocore-sagemaker-metrics](https://pypi.org/project/types-aiobotocore-sagemaker-metrics/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[sagemaker-metrics]` package installed.

Write your `SageMakerMetrics` code as usual,
type checking and code completion should work out of the box.



```python
# SageMakerMetricsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("sagemaker-metrics") as client:  # (1)
    result = await client.batch_get_metrics()  # (2)
```

1. client: [SageMakerMetricsClient](./client.md)
2. result: [:material-code-braces: BatchGetMetricsResponseTypeDef](./type_defs.md#batchgetmetricsresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[sagemaker-metrics]`
or a standalone `types_aiobotocore_sagemaker_metrics` package, you have to explicitly specify
`client: SageMakerMetricsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SageMakerMetricsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_sagemaker_metrics.client import SageMakerMetricsClient
from types_aiobotocore_sagemaker_metrics.type_defs import BatchGetMetricsResponseTypeDef
from types_aiobotocore_sagemaker_metrics.type_defs import BatchGetMetricsRequestTypeDef


session = get_session()

async with session.create_client("sagemaker-metrics") as client:
    client: SageMakerMetricsClient
    kwargs: BatchGetMetricsRequestTypeDef = {...}
    result: BatchGetMetricsResponseTypeDef = await client.batch_get_metrics(**kwargs)
```




