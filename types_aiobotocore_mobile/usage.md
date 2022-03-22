<a id="examples-for-aiobotocore-mobile-module"></a>

# Examples for aiobotocore Mobile module

> [Index](../README.md) > [Mobile](./README.md) > Examples

- [Examples for aiobotocore Mobile module](#examples-for-aiobotocore-mobile-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[mobile]` package installed.

Write your `Mobile` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type MobileClient
# and provides type checking and code completion
async with session.create_client("mobile") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListBundlesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_bundles")
    async for item in paginator.paginate(...):
        # item has type ListBundlesResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[mobile]` or a standalone
`types_aiobotocore_mobile` package, you have to explicitly specify
`client: MobileClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_mobile.client import MobileClient
from types_aiobotocore_mobile.type_defs import bool
from types_aiobotocore_mobile.paginator import ListBundlesPaginator

from types_aiobotocore_mobile.literals import PaginatorName



session = get_session()

async with session.create_client("mobile") as client:
    client: MobileClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_bundles"
    paginator: ListBundlesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListBundlesResultTypeDef
        print(item)
    

    
```
