<a id="examples-for-aiobotocore-connect-module"></a>

# Examples for aiobotocore Connect module

> [Index](../README.md) > [Connect](./README.md) > Examples

- [Examples for aiobotocore Connect module](#examples-for-aiobotocore-connect-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[connect]` package installed.

Write your `Connect` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ConnectClient
# and provides type checking and code completion
async with session.create_client("connect") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_approved_origin()
    

    
    # paginator has type GetMetricDataPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_metric_data")
    async for item in paginator.paginate(...):
        # item has type GetMetricDataResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[connect]` or a standalone
`types_aiobotocore_connect` package, you have to explicitly specify
`client: ConnectClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.client import ConnectClient
from types_aiobotocore_connect.type_defs import None
from types_aiobotocore_connect.paginator import GetMetricDataPaginator

from types_aiobotocore_connect.literals import PaginatorName



session = get_session()

async with session.create_client("connect") as client:
    client: ConnectClient

    
    result: None = client.associate_approved_origin()
    

    
    paginator_name: PaginatorName = "get_metric_data"
    paginator: GetMetricDataPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetMetricDataResponseTypeDef
        print(item)
    

    
```
