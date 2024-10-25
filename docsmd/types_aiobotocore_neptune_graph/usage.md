# Examples

> [Index](../README.md) > [NeptuneGraph](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [NeptuneGraph](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph)
    type annotations stubs module [types-aiobotocore-neptune-graph](https://pypi.org/project/types-aiobotocore-neptune-graph/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[neptune-graph]` package installed.

Write your `NeptuneGraph` code as usual,
type checking and code completion should work out of the box.



```python
# NeptuneGraphClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("neptune-graph") as client:  # (1)
    result = await client.cancel_import_task()  # (2)
```

1. client: [NeptuneGraphClient](./client.md)
2. result: [:material-code-braces: CancelImportTaskOutputTypeDef](./type_defs.md#cancelimporttaskoutputtypedef) 



```python
# ListGraphSnapshotsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("neptune-graph") as client:  # (1)
    paginator = client.get_paginator("list_graph_snapshots")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [NeptuneGraphClient](./client.md)
2. paginator: [ListGraphSnapshotsPaginator](./paginators.md#listgraphsnapshotspaginator)
3. item: [:material-code-braces: ListGraphSnapshotsOutputTypeDef](./type_defs.md#listgraphsnapshotsoutputtypedef) 



```python
# GraphAvailableWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("neptune-graph") as client:  # (1)
    waiter = client.get_waiter("graph_available")  # (2)
    await waiter.wait()
```

1. client: [NeptuneGraphClient](./client.md)
2. waiter: [GraphAvailableWaiter](./waiters.md#graphavailablewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[neptune-graph]`
or a standalone `types_aiobotocore_neptune_graph` package, you have to explicitly specify
`client: NeptuneGraphClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# NeptuneGraphClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_neptune_graph.client import NeptuneGraphClient
from types_aiobotocore_neptune_graph.type_defs import CancelImportTaskOutputTypeDef
from types_aiobotocore_neptune_graph.type_defs import CancelImportTaskInputRequestTypeDef


session = get_session()

async with session.create_client("neptune-graph") as client:
    client: NeptuneGraphClient
    kwargs: CancelImportTaskInputRequestTypeDef = {...}
    result: CancelImportTaskOutputTypeDef = await client.cancel_import_task(**kwargs)
```



```python
# ListGraphSnapshotsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_neptune_graph.client import NeptuneGraphClient
from types_aiobotocore_neptune_graph.paginator import ListGraphSnapshotsPaginator
from types_aiobotocore_neptune_graph.type_defs import ListGraphSnapshotsOutputTypeDef


session = get_session()

async with session.create_client("neptune-graph") as client:
    client: NeptuneGraphClient
    paginator: ListGraphSnapshotsPaginator = client.get_paginator("list_graph_snapshots")
    async for item in paginator.paginate(...):
        item: ListGraphSnapshotsOutputTypeDef
        print(item)
```



```python
# GraphAvailableWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_neptune_graph.client import NeptuneGraphClient
from types_aiobotocore_neptune_graph.waiter import GraphAvailableWaiter


session = get_session()

async with session.create_client("neptune-graph") as client:
    client: NeptuneGraphClient
    waiter: GraphAvailableWaiter = client.get_waiter("graph_available")
    await waiter.wait()
```
