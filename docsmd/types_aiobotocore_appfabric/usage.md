# Examples

> [Index](../README.md) > [AppFabric](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AppFabric](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#appfabric)
    type annotations stubs module [types-aiobotocore-appfabric](https://pypi.org/project/types-aiobotocore-appfabric/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[appfabric]` package installed.

Write your `AppFabric` code as usual,
type checking and code completion should work out of the box.



```python
# AppFabricClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("appfabric") as client:  # (1)
    result = await client.batch_get_user_access_tasks()  # (2)
```

1. client: [AppFabricClient](./client.md)
2. result: [:material-code-braces: BatchGetUserAccessTasksResponseTypeDef](./type_defs.md#batchgetuseraccesstasksresponsetypedef) 



```python
# ListAppAuthorizationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("appfabric") as client:  # (1)
    paginator = client.get_paginator("list_app_authorizations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AppFabricClient](./client.md)
2. paginator: [ListAppAuthorizationsPaginator](./paginators.md#listappauthorizationspaginator)
3. item: [:material-code-braces: ListAppAuthorizationsResponseTypeDef](./type_defs.md#listappauthorizationsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[appfabric]`
or a standalone `types_aiobotocore_appfabric` package, you have to explicitly specify
`client: AppFabricClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# AppFabricClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_appfabric.client import AppFabricClient
from types_aiobotocore_appfabric.type_defs import BatchGetUserAccessTasksResponseTypeDef
from types_aiobotocore_appfabric.type_defs import BatchGetUserAccessTasksRequestTypeDef


session = get_session()

async with session.create_client("appfabric") as client:
    client: AppFabricClient
    kwargs: BatchGetUserAccessTasksRequestTypeDef = {...}
    result: BatchGetUserAccessTasksResponseTypeDef = await client.batch_get_user_access_tasks(**kwargs)
```



```python
# ListAppAuthorizationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_appfabric.client import AppFabricClient
from types_aiobotocore_appfabric.paginator import ListAppAuthorizationsPaginator
from types_aiobotocore_appfabric.type_defs import ListAppAuthorizationsResponseTypeDef


session = get_session()

async with session.create_client("appfabric") as client:
    client: AppFabricClient
    paginator: ListAppAuthorizationsPaginator = client.get_paginator("list_app_authorizations")
    async for item in paginator.paginate(...):
        item: ListAppAuthorizationsResponseTypeDef
        print(item)
```


