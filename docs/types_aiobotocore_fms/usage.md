<a id="examples-for-aiobotocore-fms-module"></a>

# Examples for aiobotocore FMS module

> [Index](../README.md) > [FMS](./README.md) > Examples

- [Examples for aiobotocore FMS module](#examples-for-aiobotocore-fms-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[fms]` package installed.

Write your `FMS` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type FMSClient
# and provides type checking and code completion
async with session.create_client("fms") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_admin_account()
    

    
    # paginator has type ListAppsListsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_apps_lists")
    async for item in paginator.paginate(...):
        # item has type ListAppsListsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[fms]` or a standalone `types_aiobotocore_fms`
package, you have to explicitly specify `client: FMSClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_fms.client import FMSClient
from types_aiobotocore_fms.type_defs import None
from types_aiobotocore_fms.paginator import ListAppsListsPaginator

from types_aiobotocore_fms.literals import PaginatorName



session = get_session()

async with session.create_client("fms") as client:
    client: FMSClient

    
    result: None = client.associate_admin_account()
    

    
    paginator_name: PaginatorName = "list_apps_lists"
    paginator: ListAppsListsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAppsListsResponseTypeDef
        print(item)
    

    
```
