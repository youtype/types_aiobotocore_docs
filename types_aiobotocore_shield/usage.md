<a id="examples-for-aiobotocore-shield-module"></a>

# Examples for aiobotocore Shield module

> [Index](../README.md) > [Shield](./README.md) > Examples

- [Examples for aiobotocore Shield module](#examples-for-aiobotocore-shield-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[shield]` package installed.

Write your `Shield` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ShieldClient
# and provides type checking and code completion
async with session.create_client("shield") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_drt_log_bucket()
    

    
    # paginator has type ListAttacksPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_attacks")
    async for item in paginator.paginate(...):
        # item has type ListAttacksResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[shield]` or a standalone
`types_aiobotocore_shield` package, you have to explicitly specify
`client: ShieldClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_shield.client import ShieldClient
from types_aiobotocore_shield.type_defs import Dict[str, Any]
from types_aiobotocore_shield.paginator import ListAttacksPaginator

from types_aiobotocore_shield.literals import PaginatorName



session = get_session()

async with session.create_client("shield") as client:
    client: ShieldClient

    
    result: Dict[str, Any] = client.associate_drt_log_bucket()
    

    
    paginator_name: PaginatorName = "list_attacks"
    paginator: ListAttacksPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAttacksResponseTypeDef
        print(item)
    

    
```
