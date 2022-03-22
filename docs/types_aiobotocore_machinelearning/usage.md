<a id="examples-for-aiobotocore-machinelearning-module"></a>

# Examples for aiobotocore MachineLearning module

> [Index](../README.md) > [MachineLearning](./README.md) > Examples

- [Examples for aiobotocore MachineLearning module](#examples-for-aiobotocore-machinelearning-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[machinelearning]` package installed.

Write your `MachineLearning` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type MachineLearningClient
# and provides type checking and code completion
async with session.create_client("machinelearning") as client:
    
    # result has type AddTagsOutputTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_tags()
    

    
    # paginator has type DescribeBatchPredictionsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_batch_predictions")
    async for item in paginator.paginate(...):
        # item has type DescribeBatchPredictionsOutputTypeDef
        print(item)
    

    
    # waiter has type BatchPredictionAvailableWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("batch_prediction_available")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[machinelearning]` or a standalone
`types_aiobotocore_machinelearning` package, you have to explicitly specify
`client: MachineLearningClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_machinelearning.client import MachineLearningClient
from types_aiobotocore_machinelearning.type_defs import AddTagsOutputTypeDef
from types_aiobotocore_machinelearning.paginator import DescribeBatchPredictionsPaginator
from types_aiobotocore_machinelearning.waiter import BatchPredictionAvailableWaiter
from types_aiobotocore_machinelearning.literals import PaginatorName
from types_aiobotocore_machinelearning.literals import WaiterName


session = get_session()

async with session.create_client("machinelearning") as client:
    client: MachineLearningClient

    
    result: AddTagsOutputTypeDef = client.add_tags()
    

    
    paginator_name: PaginatorName = "describe_batch_predictions"
    paginator: DescribeBatchPredictionsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeBatchPredictionsOutputTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "batch_prediction_available"
    waiter: BatchPredictionAvailableWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
