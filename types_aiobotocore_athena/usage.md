<a id="examples-for-aiobotocore-athena-module"></a>

# Examples for aiobotocore Athena module

> [Index](../README.md) > [Athena](./README.md) > Examples

- [Examples for aiobotocore Athena module](#examples-for-aiobotocore-athena-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[athena]` package installed.

Write your `Athena` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type AthenaClient
# and provides type checking and code completion
async with session.create_client("athena") as client:
    
    # result has type BatchGetNamedQueryOutputTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_get_named_query()
    

    
    # paginator has type GetQueryResultsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_query_results")
    async for item in paginator.paginate(...):
        # item has type GetQueryResultsOutputTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[athena]` or a standalone
`types_aiobotocore_athena` package, you have to explicitly specify
`client: AthenaClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_athena.client import AthenaClient
from types_aiobotocore_athena.type_defs import BatchGetNamedQueryOutputTypeDef
from types_aiobotocore_athena.paginator import GetQueryResultsPaginator

from types_aiobotocore_athena.literals import PaginatorName



session = get_session()

async with session.create_client("athena") as client:
    client: AthenaClient

    
    result: BatchGetNamedQueryOutputTypeDef = client.batch_get_named_query()
    

    
    paginator_name: PaginatorName = "get_query_results"
    paginator: GetQueryResultsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetQueryResultsOutputTypeDef
        print(item)
    

    
```
