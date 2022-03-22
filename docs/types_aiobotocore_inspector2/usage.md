<a id="examples-for-aiobotocore-inspector2-module"></a>

# Examples for aiobotocore Inspector2 module

> [Index](../README.md) > [Inspector2](./README.md) > Examples

- [Examples for aiobotocore Inspector2 module](#examples-for-aiobotocore-inspector2-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[inspector2]` package installed.

Write your `Inspector2` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type Inspector2Client
# and provides type checking and code completion
async with session.create_client("inspector2") as client:
    
    # result has type AssociateMemberResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_member()
    

    
    # paginator has type ListAccountPermissionsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_account_permissions")
    async for item in paginator.paginate(...):
        # item has type ListAccountPermissionsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[inspector2]` or a standalone
`types_aiobotocore_inspector2` package, you have to explicitly specify
`client: Inspector2Client` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_inspector2.client import Inspector2Client
from types_aiobotocore_inspector2.type_defs import AssociateMemberResponseTypeDef
from types_aiobotocore_inspector2.paginator import ListAccountPermissionsPaginator

from types_aiobotocore_inspector2.literals import PaginatorName



session = get_session()

async with session.create_client("inspector2") as client:
    client: Inspector2Client

    
    result: AssociateMemberResponseTypeDef = client.associate_member()
    

    
    paginator_name: PaginatorName = "list_account_permissions"
    paginator: ListAccountPermissionsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAccountPermissionsResponseTypeDef
        print(item)
    

    
```
