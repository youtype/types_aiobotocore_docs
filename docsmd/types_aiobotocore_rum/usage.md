# Examples

> [Index](../README.md) > [CloudWatchRUM](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudWatchRUM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#cloudwatchrum)
    type annotations stubs module [types-aiobotocore-rum](https://pypi.org/project/types-aiobotocore-rum/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[rum]` package installed.

Write your `CloudWatchRUM` code as usual,
type checking and code completion should work out of the box.



```python
# CloudWatchRUMClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("rum") as client:  # (1)
    result = await client.batch_create_rum_metric_definitions()  # (2)
```

1. client: [CloudWatchRUMClient](./client.md)
2. result: [:material-code-braces: BatchCreateRumMetricDefinitionsResponseTypeDef](./type_defs.md#batchcreaterummetricdefinitionsresponsetypedef) 



```python
# BatchGetRumMetricDefinitionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("rum") as client:  # (1)
    paginator = client.get_paginator("batch_get_rum_metric_definitions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CloudWatchRUMClient](./client.md)
2. paginator: [BatchGetRumMetricDefinitionsPaginator](./paginators.md#batchgetrummetricdefinitionspaginator)
3. item: [:material-code-braces: BatchGetRumMetricDefinitionsResponseTypeDef](./type_defs.md#batchgetrummetricdefinitionsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[rum]`
or a standalone `types_aiobotocore_rum` package, you have to explicitly specify
`client: CloudWatchRUMClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CloudWatchRUMClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_rum.client import CloudWatchRUMClient
from types_aiobotocore_rum.type_defs import BatchCreateRumMetricDefinitionsResponseTypeDef
from types_aiobotocore_rum.type_defs import BatchCreateRumMetricDefinitionsRequestTypeDef


session = get_session()

async with session.create_client("rum") as client:
    client: CloudWatchRUMClient
    kwargs: BatchCreateRumMetricDefinitionsRequestTypeDef = {...}
    result: BatchCreateRumMetricDefinitionsResponseTypeDef = await client.batch_create_rum_metric_definitions(**kwargs)
```



```python
# BatchGetRumMetricDefinitionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_rum.client import CloudWatchRUMClient
from types_aiobotocore_rum.paginator import BatchGetRumMetricDefinitionsPaginator
from types_aiobotocore_rum.type_defs import BatchGetRumMetricDefinitionsResponseTypeDef


session = get_session()

async with session.create_client("rum") as client:
    client: CloudWatchRUMClient
    paginator: BatchGetRumMetricDefinitionsPaginator = client.get_paginator("batch_get_rum_metric_definitions")
    async for item in paginator.paginate(...):
        item: BatchGetRumMetricDefinitionsResponseTypeDef
        print(item)
```


