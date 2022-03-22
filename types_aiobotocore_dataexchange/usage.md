<a id="examples-for-aiobotocore-dataexchange-module"></a>

# Examples for aiobotocore DataExchange module

> [Index](../README.md) > [DataExchange](./README.md) > Examples

- [Examples for aiobotocore DataExchange module](#examples-for-aiobotocore-dataexchange-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[dataexchange]` package installed.

Write your `DataExchange` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type DataExchangeClient
# and provides type checking and code completion
async with session.create_client("dataexchange") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListDataSetRevisionsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_data_set_revisions")
    async for item in paginator.paginate(...):
        # item has type ListDataSetRevisionsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[dataexchange]` or a standalone
`types_aiobotocore_dataexchange` package, you have to explicitly specify
`client: DataExchangeClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_dataexchange.client import DataExchangeClient
from types_aiobotocore_dataexchange.type_defs import bool
from types_aiobotocore_dataexchange.paginator import ListDataSetRevisionsPaginator

from types_aiobotocore_dataexchange.literals import PaginatorName



session = get_session()

async with session.create_client("dataexchange") as client:
    client: DataExchangeClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_data_set_revisions"
    paginator: ListDataSetRevisionsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListDataSetRevisionsResponseTypeDef
        print(item)
    

    
```
