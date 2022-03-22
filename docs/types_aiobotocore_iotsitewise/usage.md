<a id="examples-for-aiobotocore-iotsitewise-module"></a>

# Examples for aiobotocore IoTSiteWise module

> [Index](../README.md) > [IoTSiteWise](./README.md) > Examples

- [Examples for aiobotocore IoTSiteWise module](#examples-for-aiobotocore-iotsitewise-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[iotsitewise]` package installed.

Write your `IoTSiteWise` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type IoTSiteWiseClient
# and provides type checking and code completion
async with session.create_client("iotsitewise") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_assets()
    

    
    # paginator has type GetAssetPropertyAggregatesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_asset_property_aggregates")
    async for item in paginator.paginate(...):
        # item has type GetAssetPropertyAggregatesResponseTypeDef
        print(item)
    

    
    # waiter has type AssetActiveWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("asset_active")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[iotsitewise]` or a standalone
`types_aiobotocore_iotsitewise` package, you have to explicitly specify
`client: IoTSiteWiseClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.client import IoTSiteWiseClient
from types_aiobotocore_iotsitewise.type_defs import None
from types_aiobotocore_iotsitewise.paginator import GetAssetPropertyAggregatesPaginator
from types_aiobotocore_iotsitewise.waiter import AssetActiveWaiter
from types_aiobotocore_iotsitewise.literals import PaginatorName
from types_aiobotocore_iotsitewise.literals import WaiterName


session = get_session()

async with session.create_client("iotsitewise") as client:
    client: IoTSiteWiseClient

    
    result: None = client.associate_assets()
    

    
    paginator_name: PaginatorName = "get_asset_property_aggregates"
    paginator: GetAssetPropertyAggregatesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetAssetPropertyAggregatesResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "asset_active"
    waiter: AssetActiveWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
