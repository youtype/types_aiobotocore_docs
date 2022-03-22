<a id="examples-for-aiobotocore-workmail-module"></a>

# Examples for aiobotocore WorkMail module

> [Index](../README.md) > [WorkMail](./README.md) > Examples

- [Examples for aiobotocore WorkMail module](#examples-for-aiobotocore-workmail-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[workmail]` package installed.

Write your `WorkMail` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type WorkMailClient
# and provides type checking and code completion
async with session.create_client("workmail") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_delegate_to_resource()
    

    
    # paginator has type ListAliasesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_aliases")
    async for item in paginator.paginate(...):
        # item has type ListAliasesResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[workmail]` or a standalone
`types_aiobotocore_workmail` package, you have to explicitly specify
`client: WorkMailClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_workmail.client import WorkMailClient
from types_aiobotocore_workmail.type_defs import Dict[str, Any]
from types_aiobotocore_workmail.paginator import ListAliasesPaginator

from types_aiobotocore_workmail.literals import PaginatorName



session = get_session()

async with session.create_client("workmail") as client:
    client: WorkMailClient

    
    result: Dict[str, Any] = client.associate_delegate_to_resource()
    

    
    paginator_name: PaginatorName = "list_aliases"
    paginator: ListAliasesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAliasesResponseTypeDef
        print(item)
    

    
```
