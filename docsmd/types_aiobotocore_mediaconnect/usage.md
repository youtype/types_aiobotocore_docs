# Examples

> [Index](../README.md) > [MediaConnect](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MediaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#mediaconnect)
    type annotations stubs module [types-aiobotocore-mediaconnect](https://pypi.org/project/types-aiobotocore-mediaconnect/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[mediaconnect]` package installed.

Write your `MediaConnect` code as usual,
type checking and code completion should work out of the box.



```python
# MediaConnectClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("mediaconnect") as client:  # (1)
    result = await client.add_bridge_outputs()  # (2)
```

1. client: [MediaConnectClient](./client.md)
2. result: [:material-code-braces: AddBridgeOutputsResponseTypeDef](./type_defs.md#addbridgeoutputsresponsetypedef) 



```python
# ListBridgesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("mediaconnect") as client:  # (1)
    paginator = client.get_paginator("list_bridges")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MediaConnectClient](./client.md)
2. paginator: [ListBridgesPaginator](./paginators.md#listbridgespaginator)
3. item: [:material-code-braces: ListBridgesResponseTypeDef](./type_defs.md#listbridgesresponsetypedef) 



```python
# FlowActiveWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("mediaconnect") as client:  # (1)
    waiter = client.get_waiter("flow_active")  # (2)
    await waiter.wait()
```

1. client: [MediaConnectClient](./client.md)
2. waiter: [FlowActiveWaiter](./waiters.md#flowactivewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[mediaconnect]`
or a standalone `types_aiobotocore_mediaconnect` package, you have to explicitly specify
`client: MediaConnectClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# MediaConnectClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.client import MediaConnectClient
from types_aiobotocore_mediaconnect.type_defs import AddBridgeOutputsResponseTypeDef
from types_aiobotocore_mediaconnect.type_defs import AddBridgeOutputsRequestTypeDef


session = get_session()

async with session.create_client("mediaconnect") as client:
    client: MediaConnectClient
    kwargs: AddBridgeOutputsRequestTypeDef = {...}
    result: AddBridgeOutputsResponseTypeDef = await client.add_bridge_outputs(**kwargs)
```



```python
# ListBridgesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.client import MediaConnectClient
from types_aiobotocore_mediaconnect.paginator import ListBridgesPaginator
from types_aiobotocore_mediaconnect.type_defs import ListBridgesResponseTypeDef


session = get_session()

async with session.create_client("mediaconnect") as client:
    client: MediaConnectClient
    paginator: ListBridgesPaginator = client.get_paginator("list_bridges")
    async for item in paginator.paginate(...):
        item: ListBridgesResponseTypeDef
        print(item)
```



```python
# FlowActiveWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.client import MediaConnectClient
from types_aiobotocore_mediaconnect.waiter import FlowActiveWaiter


session = get_session()

async with session.create_client("mediaconnect") as client:
    client: MediaConnectClient
    waiter: FlowActiveWaiter = client.get_waiter("flow_active")
    await waiter.wait()
```
