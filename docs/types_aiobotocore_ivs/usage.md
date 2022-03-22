<a id="examples-for-aiobotocore-ivs-module"></a>

# Examples for aiobotocore IVS module

> [Index](../README.md) > [IVS](./README.md) > Examples

- [Examples for aiobotocore IVS module](#examples-for-aiobotocore-ivs-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[ivs]` package installed.

Write your `IVS` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type IVSClient
# and provides type checking and code completion
async with session.create_client("ivs") as client:
    
    # result has type BatchGetChannelResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_get_channel()
    

    
    # paginator has type ListChannelsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_channels")
    async for item in paginator.paginate(...):
        # item has type ListChannelsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[ivs]` or a standalone `types_aiobotocore_ivs`
package, you have to explicitly specify `client: IVSClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_ivs.client import IVSClient
from types_aiobotocore_ivs.type_defs import BatchGetChannelResponseTypeDef
from types_aiobotocore_ivs.paginator import ListChannelsPaginator

from types_aiobotocore_ivs.literals import PaginatorName



session = get_session()

async with session.create_client("ivs") as client:
    client: IVSClient

    
    result: BatchGetChannelResponseTypeDef = client.batch_get_channel()
    

    
    paginator_name: PaginatorName = "list_channels"
    paginator: ListChannelsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListChannelsResponseTypeDef
        print(item)
    

    
```
