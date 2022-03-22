<a id="examples-for-aiobotocore-timestreamquery-module"></a>

# Examples for aiobotocore TimestreamQuery module

> [Index](../README.md) > [TimestreamQuery](./README.md) > Examples

- [Examples for aiobotocore TimestreamQuery module](#examples-for-aiobotocore-timestreamquery-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[timestream-query]` package installed.

Write your `TimestreamQuery` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type TimestreamQueryClient
# and provides type checking and code completion
async with session.create_client("timestream-query") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListScheduledQueriesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_scheduled_queries")
    async for item in paginator.paginate(...):
        # item has type ListScheduledQueriesResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[timestream-query]` or a standalone
`types_aiobotocore_timestream_query` package, you have to explicitly specify
`client: TimestreamQueryClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_timestream_query.client import TimestreamQueryClient
from types_aiobotocore_timestream_query.type_defs import bool
from types_aiobotocore_timestream_query.paginator import ListScheduledQueriesPaginator

from types_aiobotocore_timestream_query.literals import PaginatorName



session = get_session()

async with session.create_client("timestream-query") as client:
    client: TimestreamQueryClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_scheduled_queries"
    paginator: ListScheduledQueriesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListScheduledQueriesResponseTypeDef
        print(item)
    

    
```
