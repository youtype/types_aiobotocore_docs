<a id="examples-for-aiobotocore-honeycode-module"></a>

# Examples for aiobotocore Honeycode module

> [Index](../README.md) > [Honeycode](./README.md) > Examples

- [Examples for aiobotocore Honeycode module](#examples-for-aiobotocore-honeycode-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[honeycode]` package installed.

Write your `Honeycode` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type HoneycodeClient
# and provides type checking and code completion
async with session.create_client("honeycode") as client:
    
    # result has type BatchCreateTableRowsResultTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_create_table_rows()
    

    
    # paginator has type ListTableColumnsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_table_columns")
    async for item in paginator.paginate(...):
        # item has type ListTableColumnsResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[honeycode]` or a standalone
`types_aiobotocore_honeycode` package, you have to explicitly specify
`client: HoneycodeClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_honeycode.client import HoneycodeClient
from types_aiobotocore_honeycode.type_defs import BatchCreateTableRowsResultTypeDef
from types_aiobotocore_honeycode.paginator import ListTableColumnsPaginator

from types_aiobotocore_honeycode.literals import PaginatorName



session = get_session()

async with session.create_client("honeycode") as client:
    client: HoneycodeClient

    
    result: BatchCreateTableRowsResultTypeDef = client.batch_create_table_rows()
    

    
    paginator_name: PaginatorName = "list_table_columns"
    paginator: ListTableColumnsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListTableColumnsResultTypeDef
        print(item)
    

    
```
