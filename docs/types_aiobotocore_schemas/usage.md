<a id="examples-for-aiobotocore-schemas-module"></a>

# Examples for aiobotocore Schemas module

> [Index](../README.md) > [Schemas](./README.md) > Examples

- [Examples for aiobotocore Schemas module](#examples-for-aiobotocore-schemas-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[schemas]` package installed.

Write your `Schemas` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SchemasClient
# and provides type checking and code completion
async with session.create_client("schemas") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListDiscoverersPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_discoverers")
    async for item in paginator.paginate(...):
        # item has type ListDiscoverersResponseTypeDef
        print(item)
    

    
    # waiter has type CodeBindingExistsWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("code_binding_exists")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[schemas]` or a standalone
`types_aiobotocore_schemas` package, you have to explicitly specify
`client: SchemasClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_schemas.client import SchemasClient
from types_aiobotocore_schemas.type_defs import bool
from types_aiobotocore_schemas.paginator import ListDiscoverersPaginator
from types_aiobotocore_schemas.waiter import CodeBindingExistsWaiter
from types_aiobotocore_schemas.literals import PaginatorName
from types_aiobotocore_schemas.literals import WaiterName


session = get_session()

async with session.create_client("schemas") as client:
    client: SchemasClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_discoverers"
    paginator: ListDiscoverersPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListDiscoverersResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "code_binding_exists"
    waiter: CodeBindingExistsWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
