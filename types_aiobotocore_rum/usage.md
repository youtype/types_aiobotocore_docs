<a id="examples-for-aiobotocore-cloudwatchrum-module"></a>

# Examples for aiobotocore CloudWatchRUM module

> [Index](../README.md) > [CloudWatchRUM](./README.md) > Examples

- [Examples for aiobotocore CloudWatchRUM module](#examples-for-aiobotocore-cloudwatchrum-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[rum]` package installed.

Write your `CloudWatchRUM` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CloudWatchRUMClient
# and provides type checking and code completion
async with session.create_client("rum") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type GetAppMonitorDataPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_app_monitor_data")
    async for item in paginator.paginate(...):
        # item has type GetAppMonitorDataResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[rum]` or a standalone `types_aiobotocore_rum`
package, you have to explicitly specify `client: CloudWatchRUMClient` type
annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_rum.client import CloudWatchRUMClient
from types_aiobotocore_rum.type_defs import bool
from types_aiobotocore_rum.paginator import GetAppMonitorDataPaginator

from types_aiobotocore_rum.literals import PaginatorName



session = get_session()

async with session.create_client("rum") as client:
    client: CloudWatchRUMClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "get_app_monitor_data"
    paginator: GetAppMonitorDataPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetAppMonitorDataResponseTypeDef
        print(item)
    

    
```
