# Examples

> [Index](../README.md) > [Athena](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Athena](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#athena)
    type annotations stubs module [types-aiobotocore-athena](https://pypi.org/project/types-aiobotocore-athena/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[athena]` package installed.

Write your `Athena` code as usual,
type checking and code completion should work out of the box.



```python
# AthenaClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("athena") as client:  # (1)
    result = await client.batch_get_named_query()  # (2)
```

1. client: [AthenaClient](./client.md)
2. result: [:material-code-braces: BatchGetNamedQueryOutputTypeDef](./type_defs.md#batchgetnamedqueryoutputtypedef) 



```python
# GetQueryResultsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("athena") as client:  # (1)
    paginator = client.get_paginator("get_query_results")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AthenaClient](./client.md)
2. paginator: [GetQueryResultsPaginator](./paginators.md#getqueryresultspaginator)
3. item: [:material-code-braces: GetQueryResultsOutputTypeDef](./type_defs.md#getqueryresultsoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[athena]`
or a standalone `types_aiobotocore_athena` package, you have to explicitly specify
`client: AthenaClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# AthenaClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_athena.client import AthenaClient
from types_aiobotocore_athena.type_defs import BatchGetNamedQueryOutputTypeDef
from types_aiobotocore_athena.type_defs import BatchGetNamedQueryInputTypeDef


session = get_session()

async with session.create_client("athena") as client:
    client: AthenaClient
    kwargs: BatchGetNamedQueryInputTypeDef = {...}
    result: BatchGetNamedQueryOutputTypeDef = await client.batch_get_named_query(**kwargs)
```



```python
# GetQueryResultsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_athena.client import AthenaClient
from types_aiobotocore_athena.paginator import GetQueryResultsPaginator
from types_aiobotocore_athena.type_defs import GetQueryResultsOutputTypeDef


session = get_session()

async with session.create_client("athena") as client:
    client: AthenaClient
    paginator: GetQueryResultsPaginator = client.get_paginator("get_query_results")
    async for item in paginator.paginate(...):
        item: GetQueryResultsOutputTypeDef
        print(item)
```


