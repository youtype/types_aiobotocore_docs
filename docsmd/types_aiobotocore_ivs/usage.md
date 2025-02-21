# Examples

> [Index](../README.md) > [IVS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IVS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#ivs)
    type annotations stubs module [types-aiobotocore-ivs](https://pypi.org/project/types-aiobotocore-ivs/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[ivs]` package installed.

Write your `IVS` code as usual,
type checking and code completion should work out of the box.



```python
# IVSClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ivs") as client:  # (1)
    result = await client.batch_get_channel()  # (2)
```

1. client: [IVSClient](./client.md)
2. result: [:material-code-braces: BatchGetChannelResponseTypeDef](./type_defs.md#batchgetchannelresponsetypedef) 



```python
# ListChannelsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ivs") as client:  # (1)
    paginator = client.get_paginator("list_channels")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [IVSClient](./client.md)
2. paginator: [ListChannelsPaginator](./paginators.md#listchannelspaginator)
3. item: [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[ivs]`
or a standalone `types_aiobotocore_ivs` package, you have to explicitly specify
`client: IVSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# IVSClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ivs.client import IVSClient
from types_aiobotocore_ivs.type_defs import BatchGetChannelResponseTypeDef
from types_aiobotocore_ivs.type_defs import BatchGetChannelRequestTypeDef


session = get_session()

async with session.create_client("ivs") as client:
    client: IVSClient
    kwargs: BatchGetChannelRequestTypeDef = {...}
    result: BatchGetChannelResponseTypeDef = await client.batch_get_channel(**kwargs)
```



```python
# ListChannelsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ivs.client import IVSClient
from types_aiobotocore_ivs.paginator import ListChannelsPaginator
from types_aiobotocore_ivs.type_defs import ListChannelsResponseTypeDef


session = get_session()

async with session.create_client("ivs") as client:
    client: IVSClient
    paginator: ListChannelsPaginator = client.get_paginator("list_channels")
    async for item in paginator.paginate(...):
        item: ListChannelsResponseTypeDef
        print(item)
```


