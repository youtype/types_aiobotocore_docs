<a id="examples-for-aiobotocore-keyspaces-module"></a>

# Examples for aiobotocore Keyspaces module

> [Index](../README.md) > [Keyspaces](./README.md) > Examples

- [Examples for aiobotocore Keyspaces module](#examples-for-aiobotocore-keyspaces-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[keyspaces]` package installed.

Write your `Keyspaces` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type KeyspacesClient
# and provides type checking and code completion
async with session.create_client("keyspaces") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListKeyspacesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_keyspaces")
    async for item in paginator.paginate(...):
        # item has type ListKeyspacesResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[keyspaces]` or a standalone
`types_aiobotocore_keyspaces` package, you have to explicitly specify
`client: KeyspacesClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_keyspaces.client import KeyspacesClient
from types_aiobotocore_keyspaces.type_defs import bool
from types_aiobotocore_keyspaces.paginator import ListKeyspacesPaginator

from types_aiobotocore_keyspaces.literals import PaginatorName



session = get_session()

async with session.create_client("keyspaces") as client:
    client: KeyspacesClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_keyspaces"
    paginator: ListKeyspacesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListKeyspacesResponseTypeDef
        print(item)
    

    
```
