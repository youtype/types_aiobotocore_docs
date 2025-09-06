# Examples

> [Index](../README.md) > [DataZone](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DataZone](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#datazone)
    type annotations stubs module [types-aiobotocore-datazone](https://pypi.org/project/types-aiobotocore-datazone/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[datazone]` package installed.

Write your `DataZone` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# DataZoneClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("datazone") as client:  # (1)
    result = await client.accept_predictions()  # (2)
```

1. client: [DataZoneClient](./client.md)
2. result: [:material-code-braces: AcceptPredictionsOutputTypeDef](./type_defs.md#acceptpredictionsoutputtypedef)



#### Paginator usage example

```python
# ListAccountPoolsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("datazone") as client:  # (1)
    paginator = client.get_paginator("list_account_pools")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [ListAccountPoolsPaginator](./paginators.md#listaccountpoolspaginator)
3. item: [:material-code-braces: ListAccountPoolsOutputTypeDef](./type_defs.md#listaccountpoolsoutputtypedef)




### Explicit type annotations

With `types-aiobotocore-lite[datazone]`
or a standalone `types_aiobotocore_datazone` package, you have to explicitly specify
`client: DataZoneClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# DataZoneClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_datazone.client import DataZoneClient
from types_aiobotocore_datazone.type_defs import AcceptPredictionsOutputTypeDef
from types_aiobotocore_datazone.type_defs import AcceptPredictionsInputTypeDef


session = get_session()

async with session.create_client("datazone") as client:
    client: DataZoneClient
    kwargs: AcceptPredictionsInputTypeDef = {...}
    result: AcceptPredictionsOutputTypeDef = await client.accept_predictions(**kwargs)
```



#### Paginator usage example

```python
# ListAccountPoolsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_datazone.client import DataZoneClient
from types_aiobotocore_datazone.paginator import ListAccountPoolsPaginator
from types_aiobotocore_datazone.type_defs import ListAccountPoolsOutputTypeDef


session = get_session()

async with session.create_client("datazone") as client:
    client: DataZoneClient
    paginator: ListAccountPoolsPaginator = client.get_paginator("list_account_pools")
    async for item in paginator.paginate(...):
        item: ListAccountPoolsOutputTypeDef
        print(item)
```


