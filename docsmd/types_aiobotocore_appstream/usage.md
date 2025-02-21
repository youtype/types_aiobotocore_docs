# Examples

> [Index](../README.md) > [AppStream](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AppStream](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#appstream)
    type annotations stubs module [types-aiobotocore-appstream](https://pypi.org/project/types-aiobotocore-appstream/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[appstream]` package installed.

Write your `AppStream` code as usual,
type checking and code completion should work out of the box.



```python
# AppStreamClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("appstream") as client:  # (1)
    result = await client.associate_app_block_builder_app_block()  # (2)
```

1. client: [AppStreamClient](./client.md)
2. result: [:material-code-braces: AssociateAppBlockBuilderAppBlockResultTypeDef](./type_defs.md#associateappblockbuilderappblockresulttypedef) 



```python
# DescribeDirectoryConfigsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("appstream") as client:  # (1)
    paginator = client.get_paginator("describe_directory_configs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [DescribeDirectoryConfigsPaginator](./paginators.md#describedirectoryconfigspaginator)
3. item: [:material-code-braces: DescribeDirectoryConfigsResultTypeDef](./type_defs.md#describedirectoryconfigsresulttypedef) 



```python
# FleetStartedWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("appstream") as client:  # (1)
    waiter = client.get_waiter("fleet_started")  # (2)
    await waiter.wait()
```

1. client: [AppStreamClient](./client.md)
2. waiter: [FleetStartedWaiter](./waiters.md#fleetstartedwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[appstream]`
or a standalone `types_aiobotocore_appstream` package, you have to explicitly specify
`client: AppStreamClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# AppStreamClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_appstream.client import AppStreamClient
from types_aiobotocore_appstream.type_defs import AssociateAppBlockBuilderAppBlockResultTypeDef
from types_aiobotocore_appstream.type_defs import AssociateAppBlockBuilderAppBlockRequestTypeDef


session = get_session()

async with session.create_client("appstream") as client:
    client: AppStreamClient
    kwargs: AssociateAppBlockBuilderAppBlockRequestTypeDef = {...}
    result: AssociateAppBlockBuilderAppBlockResultTypeDef = await client.associate_app_block_builder_app_block(**kwargs)
```



```python
# DescribeDirectoryConfigsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_appstream.client import AppStreamClient
from types_aiobotocore_appstream.paginator import DescribeDirectoryConfigsPaginator
from types_aiobotocore_appstream.type_defs import DescribeDirectoryConfigsResultTypeDef


session = get_session()

async with session.create_client("appstream") as client:
    client: AppStreamClient
    paginator: DescribeDirectoryConfigsPaginator = client.get_paginator("describe_directory_configs")
    async for item in paginator.paginate(...):
        item: DescribeDirectoryConfigsResultTypeDef
        print(item)
```



```python
# FleetStartedWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_appstream.client import AppStreamClient
from types_aiobotocore_appstream.waiter import FleetStartedWaiter


session = get_session()

async with session.create_client("appstream") as client:
    client: AppStreamClient
    waiter: FleetStartedWaiter = client.get_waiter("fleet_started")
    await waiter.wait()
```
