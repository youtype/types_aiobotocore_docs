# Examples

> [Index](../README.md) > [ECS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ECS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ecs)
    type annotations stubs module [types-aiobotocore-ecs](https://pypi.org/project/types-aiobotocore-ecs/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[ecs]` package installed.

Write your `ECS` code as usual,
type checking and code completion should work out of the box.



```python
# ECSClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ecs") as client:  # (1)
    result = await client.create_capacity_provider()  # (2)
```

1. client: [ECSClient](./client.md)
2. result: [:material-code-braces: CreateCapacityProviderResponseTypeDef](./type_defs.md#createcapacityproviderresponsetypedef) 



```python
# ListAccountSettingsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ecs") as client:  # (1)
    paginator = client.get_paginator("list_account_settings")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ECSClient](./client.md)
2. paginator: [ListAccountSettingsPaginator](./paginators.md#listaccountsettingspaginator)
3. item: [:material-code-braces: ListAccountSettingsResponseTypeDef](./type_defs.md#listaccountsettingsresponsetypedef) 



```python
# ServicesInactiveWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ecs") as client:  # (1)
    waiter = client.get_waiter("services_inactive")  # (2)
    await waiter.wait()
```

1. client: [ECSClient](./client.md)
2. waiter: [ServicesInactiveWaiter](./waiters.md#servicesinactivewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[ecs]`
or a standalone `types_aiobotocore_ecs` package, you have to explicitly specify
`client: ECSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ECSClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ecs.client import ECSClient
from types_aiobotocore_ecs.type_defs import CreateCapacityProviderResponseTypeDef
from types_aiobotocore_ecs.type_defs import CreateCapacityProviderRequestTypeDef


session = get_session()

async with session.create_client("ecs") as client:
    client: ECSClient
    kwargs: CreateCapacityProviderRequestTypeDef = {...}
    result: CreateCapacityProviderResponseTypeDef = await client.create_capacity_provider(**kwargs)
```



```python
# ListAccountSettingsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ecs.client import ECSClient
from types_aiobotocore_ecs.paginator import ListAccountSettingsPaginator
from types_aiobotocore_ecs.type_defs import ListAccountSettingsResponseTypeDef


session = get_session()

async with session.create_client("ecs") as client:
    client: ECSClient
    paginator: ListAccountSettingsPaginator = client.get_paginator("list_account_settings")
    async for item in paginator.paginate(...):
        item: ListAccountSettingsResponseTypeDef
        print(item)
```



```python
# ServicesInactiveWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ecs.client import ECSClient
from types_aiobotocore_ecs.waiter import ServicesInactiveWaiter


session = get_session()

async with session.create_client("ecs") as client:
    client: ECSClient
    waiter: ServicesInactiveWaiter = client.get_waiter("services_inactive")
    await waiter.wait()
```
