<a id="examples-for-aiobotocore-mediaconnect-module"></a>

# Examples for aiobotocore MediaConnect module

> [Index](../README.md) > [MediaConnect](./README.md) > Examples

- [Examples for aiobotocore MediaConnect module](#examples-for-aiobotocore-mediaconnect-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[mediaconnect]` package installed.

Write your `MediaConnect` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type MediaConnectClient
# and provides type checking and code completion
async with session.create_client("mediaconnect") as client:
    
    # result has type AddFlowMediaStreamsResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_flow_media_streams()
    

    
    # paginator has type ListEntitlementsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_entitlements")
    async for item in paginator.paginate(...):
        # item has type ListEntitlementsResponseTypeDef
        print(item)
    

    
    # waiter has type FlowActiveWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("flow_active")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[mediaconnect]` or a standalone
`types_aiobotocore_mediaconnect` package, you have to explicitly specify
`client: MediaConnectClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.client import MediaConnectClient
from types_aiobotocore_mediaconnect.type_defs import AddFlowMediaStreamsResponseTypeDef
from types_aiobotocore_mediaconnect.paginator import ListEntitlementsPaginator
from types_aiobotocore_mediaconnect.waiter import FlowActiveWaiter
from types_aiobotocore_mediaconnect.literals import PaginatorName
from types_aiobotocore_mediaconnect.literals import WaiterName


session = get_session()

async with session.create_client("mediaconnect") as client:
    client: MediaConnectClient

    
    result: AddFlowMediaStreamsResponseTypeDef = client.add_flow_media_streams()
    

    
    paginator_name: PaginatorName = "list_entitlements"
    paginator: ListEntitlementsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListEntitlementsResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "flow_active"
    waiter: FlowActiveWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
