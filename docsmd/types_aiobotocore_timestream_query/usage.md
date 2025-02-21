# Examples

> [Index](../README.md) > [TimestreamQuery](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [TimestreamQuery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#timestreamquery)
    type annotations stubs module [types-aiobotocore-timestream-query](https://pypi.org/project/types-aiobotocore-timestream-query/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[timestream-query]` package installed.

Write your `TimestreamQuery` code as usual,
type checking and code completion should work out of the box.



```python
# TimestreamQueryClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("timestream-query") as client:  # (1)
    result = await client.cancel_query()  # (2)
```

1. client: [TimestreamQueryClient](./client.md)
2. result: [:material-code-braces: CancelQueryResponseTypeDef](./type_defs.md#cancelqueryresponsetypedef) 



```python
# ListScheduledQueriesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("timestream-query") as client:  # (1)
    paginator = client.get_paginator("list_scheduled_queries")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [TimestreamQueryClient](./client.md)
2. paginator: [ListScheduledQueriesPaginator](./paginators.md#listscheduledqueriespaginator)
3. item: [:material-code-braces: ListScheduledQueriesResponseTypeDef](./type_defs.md#listscheduledqueriesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[timestream-query]`
or a standalone `types_aiobotocore_timestream_query` package, you have to explicitly specify
`client: TimestreamQueryClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# TimestreamQueryClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_timestream_query.client import TimestreamQueryClient
from types_aiobotocore_timestream_query.type_defs import CancelQueryResponseTypeDef
from types_aiobotocore_timestream_query.type_defs import CancelQueryRequestTypeDef


session = get_session()

async with session.create_client("timestream-query") as client:
    client: TimestreamQueryClient
    kwargs: CancelQueryRequestTypeDef = {...}
    result: CancelQueryResponseTypeDef = await client.cancel_query(**kwargs)
```



```python
# ListScheduledQueriesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_timestream_query.client import TimestreamQueryClient
from types_aiobotocore_timestream_query.paginator import ListScheduledQueriesPaginator
from types_aiobotocore_timestream_query.type_defs import ListScheduledQueriesResponseTypeDef


session = get_session()

async with session.create_client("timestream-query") as client:
    client: TimestreamQueryClient
    paginator: ListScheduledQueriesPaginator = client.get_paginator("list_scheduled_queries")
    async for item in paginator.paginate(...):
        item: ListScheduledQueriesResponseTypeDef
        print(item)
```


