<a id="examples-for-aiobotocore-recyclebin-module"></a>

# Examples for aiobotocore RecycleBin module

> [Index](../README.md) > [RecycleBin](./README.md) > Examples

- [Examples for aiobotocore RecycleBin module](#examples-for-aiobotocore-recyclebin-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[rbin]` package installed.

Write your `RecycleBin` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type RecycleBinClient
# and provides type checking and code completion
async with session.create_client("rbin") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListRulesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_rules")
    async for item in paginator.paginate(...):
        # item has type ListRulesResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[rbin]` or a standalone `types_aiobotocore_rbin`
package, you have to explicitly specify `client: RecycleBinClient` type
annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_rbin.client import RecycleBinClient
from types_aiobotocore_rbin.type_defs import bool
from types_aiobotocore_rbin.paginator import ListRulesPaginator

from types_aiobotocore_rbin.literals import PaginatorName



session = get_session()

async with session.create_client("rbin") as client:
    client: RecycleBinClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_rules"
    paginator: ListRulesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListRulesResponseTypeDef
        print(item)
    

    
```
