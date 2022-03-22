<a id="examples-for-aiobotocore-appstream-module"></a>

# Examples for aiobotocore AppStream module

> [Index](../README.md) > [AppStream](./README.md) > Examples

- [Examples for aiobotocore AppStream module](#examples-for-aiobotocore-appstream-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[appstream]` package installed.

Write your `AppStream` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type AppStreamClient
# and provides type checking and code completion
async with session.create_client("appstream") as client:
    
    # result has type AssociateApplicationFleetResultTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_application_fleet()
    

    
    # paginator has type DescribeDirectoryConfigsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_directory_configs")
    async for item in paginator.paginate(...):
        # item has type DescribeDirectoryConfigsResultTypeDef
        print(item)
    

    
    # waiter has type FleetStartedWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("fleet_started")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[appstream]` or a standalone
`types_aiobotocore_appstream` package, you have to explicitly specify
`client: AppStreamClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_appstream.client import AppStreamClient
from types_aiobotocore_appstream.type_defs import AssociateApplicationFleetResultTypeDef
from types_aiobotocore_appstream.paginator import DescribeDirectoryConfigsPaginator
from types_aiobotocore_appstream.waiter import FleetStartedWaiter
from types_aiobotocore_appstream.literals import PaginatorName
from types_aiobotocore_appstream.literals import WaiterName


session = get_session()

async with session.create_client("appstream") as client:
    client: AppStreamClient

    
    result: AssociateApplicationFleetResultTypeDef = client.associate_application_fleet()
    

    
    paginator_name: PaginatorName = "describe_directory_configs"
    paginator: DescribeDirectoryConfigsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeDirectoryConfigsResultTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "fleet_started"
    waiter: FleetStartedWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
