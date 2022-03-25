<a id="examples-for-aiobotocore-chime-module"></a>

# Examples for aiobotocore Chime module

> [Index](../README.md) > [Chime](./README.md) > Examples

- [Examples for aiobotocore Chime module](#examples-for-aiobotocore-chime-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[chime]` package installed.

Write your `Chime` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ChimeClient
# and provides type checking and code completion
async with session.create_client("chime") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_phone_number_with_user()
    

    
    # paginator has type ListAccountsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_accounts")
    async for item in paginator.paginate(...):
        # item has type ListAccountsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[chime]` or a standalone `types_aiobotocore_chime`
package, you have to explicitly specify `client: ChimeClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_chime.client import ChimeClient
from types_aiobotocore_chime.type_defs import Dict[str, Any]
from types_aiobotocore_chime.paginator import ListAccountsPaginator

from types_aiobotocore_chime.literals import PaginatorName



session = get_session()

async with session.create_client("chime") as client:
    client: ChimeClient

    
    result: Dict[str, Any] = client.associate_phone_number_with_user()
    

    
    paginator_name: PaginatorName = "list_accounts"
    paginator: ListAccountsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAccountsResponseTypeDef
        print(item)
    

    
```