# Examples

> [Index](../README.md) > [DataExchange](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DataExchange](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#dataexchange)
    type annotations stubs module [types-aiobotocore-dataexchange](https://pypi.org/project/types-aiobotocore-dataexchange/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[dataexchange]` package installed.

Write your `DataExchange` code as usual,
type checking and code completion should work out of the box.



```python
# DataExchangeClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("dataexchange") as client:  # (1)
    result = await client.accept_data_grant()  # (2)
```

1. client: [DataExchangeClient](./client.md)
2. result: [:material-code-braces: AcceptDataGrantResponseTypeDef](./type_defs.md#acceptdatagrantresponsetypedef) 



```python
# ListDataGrantsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("dataexchange") as client:  # (1)
    paginator = client.get_paginator("list_data_grants")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DataExchangeClient](./client.md)
2. paginator: [ListDataGrantsPaginator](./paginators.md#listdatagrantspaginator)
3. item: [:material-code-braces: ListDataGrantsResponseTypeDef](./type_defs.md#listdatagrantsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[dataexchange]`
or a standalone `types_aiobotocore_dataexchange` package, you have to explicitly specify
`client: DataExchangeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# DataExchangeClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_dataexchange.client import DataExchangeClient
from types_aiobotocore_dataexchange.type_defs import AcceptDataGrantResponseTypeDef
from types_aiobotocore_dataexchange.type_defs import AcceptDataGrantRequestTypeDef


session = get_session()

async with session.create_client("dataexchange") as client:
    client: DataExchangeClient
    kwargs: AcceptDataGrantRequestTypeDef = {...}
    result: AcceptDataGrantResponseTypeDef = await client.accept_data_grant(**kwargs)
```



```python
# ListDataGrantsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_dataexchange.client import DataExchangeClient
from types_aiobotocore_dataexchange.paginator import ListDataGrantsPaginator
from types_aiobotocore_dataexchange.type_defs import ListDataGrantsResponseTypeDef


session = get_session()

async with session.create_client("dataexchange") as client:
    client: DataExchangeClient
    paginator: ListDataGrantsPaginator = client.get_paginator("list_data_grants")
    async for item in paginator.paginate(...):
        item: ListDataGrantsResponseTypeDef
        print(item)
```


