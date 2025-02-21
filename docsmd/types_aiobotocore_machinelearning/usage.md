# Examples

> [Index](../README.md) > [MachineLearning](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MachineLearning](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#machinelearning)
    type annotations stubs module [types-aiobotocore-machinelearning](https://pypi.org/project/types-aiobotocore-machinelearning/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[machinelearning]` package installed.

Write your `MachineLearning` code as usual,
type checking and code completion should work out of the box.



```python
# MachineLearningClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("machinelearning") as client:  # (1)
    result = await client.add_tags()  # (2)
```

1. client: [MachineLearningClient](./client.md)
2. result: [:material-code-braces: AddTagsOutputTypeDef](./type_defs.md#addtagsoutputtypedef) 



```python
# DescribeBatchPredictionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("machinelearning") as client:  # (1)
    paginator = client.get_paginator("describe_batch_predictions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MachineLearningClient](./client.md)
2. paginator: [DescribeBatchPredictionsPaginator](./paginators.md#describebatchpredictionspaginator)
3. item: [:material-code-braces: DescribeBatchPredictionsOutputTypeDef](./type_defs.md#describebatchpredictionsoutputtypedef) 



```python
# BatchPredictionAvailableWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("machinelearning") as client:  # (1)
    waiter = client.get_waiter("batch_prediction_available")  # (2)
    await waiter.wait()
```

1. client: [MachineLearningClient](./client.md)
2. waiter: [BatchPredictionAvailableWaiter](./waiters.md#batchpredictionavailablewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[machinelearning]`
or a standalone `types_aiobotocore_machinelearning` package, you have to explicitly specify
`client: MachineLearningClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# MachineLearningClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_machinelearning.client import MachineLearningClient
from types_aiobotocore_machinelearning.type_defs import AddTagsOutputTypeDef
from types_aiobotocore_machinelearning.type_defs import AddTagsInputTypeDef


session = get_session()

async with session.create_client("machinelearning") as client:
    client: MachineLearningClient
    kwargs: AddTagsInputTypeDef = {...}
    result: AddTagsOutputTypeDef = await client.add_tags(**kwargs)
```



```python
# DescribeBatchPredictionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_machinelearning.client import MachineLearningClient
from types_aiobotocore_machinelearning.paginator import DescribeBatchPredictionsPaginator
from types_aiobotocore_machinelearning.type_defs import DescribeBatchPredictionsOutputTypeDef


session = get_session()

async with session.create_client("machinelearning") as client:
    client: MachineLearningClient
    paginator: DescribeBatchPredictionsPaginator = client.get_paginator("describe_batch_predictions")
    async for item in paginator.paginate(...):
        item: DescribeBatchPredictionsOutputTypeDef
        print(item)
```



```python
# BatchPredictionAvailableWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_machinelearning.client import MachineLearningClient
from types_aiobotocore_machinelearning.waiter import BatchPredictionAvailableWaiter


session = get_session()

async with session.create_client("machinelearning") as client:
    client: MachineLearningClient
    waiter: BatchPredictionAvailableWaiter = client.get_waiter("batch_prediction_available")
    await waiter.wait()
```
