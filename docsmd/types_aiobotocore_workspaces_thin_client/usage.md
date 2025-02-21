# Examples

> [Index](../README.md) > [WorkSpacesThinClient](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WorkSpacesThinClient](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#workspacesthinclient)
    type annotations stubs module [types-aiobotocore-workspaces-thin-client](https://pypi.org/project/types-aiobotocore-workspaces-thin-client/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[workspaces-thin-client]` package installed.

Write your `WorkSpacesThinClient` code as usual,
type checking and code completion should work out of the box.



```python
# WorkSpacesThinClientClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("workspaces-thin-client") as client:  # (1)
    result = await client.create_environment()  # (2)
```

1. client: [WorkSpacesThinClientClient](./client.md)
2. result: [:material-code-braces: CreateEnvironmentResponseTypeDef](./type_defs.md#createenvironmentresponsetypedef) 



```python
# ListDevicesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("workspaces-thin-client") as client:  # (1)
    paginator = client.get_paginator("list_devices")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [WorkSpacesThinClientClient](./client.md)
2. paginator: [ListDevicesPaginator](./paginators.md#listdevicespaginator)
3. item: [:material-code-braces: ListDevicesResponseTypeDef](./type_defs.md#listdevicesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[workspaces-thin-client]`
or a standalone `types_aiobotocore_workspaces_thin_client` package, you have to explicitly specify
`client: WorkSpacesThinClientClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# WorkSpacesThinClientClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_workspaces_thin_client.client import WorkSpacesThinClientClient
from types_aiobotocore_workspaces_thin_client.type_defs import CreateEnvironmentResponseTypeDef
from types_aiobotocore_workspaces_thin_client.type_defs import CreateEnvironmentRequestTypeDef


session = get_session()

async with session.create_client("workspaces-thin-client") as client:
    client: WorkSpacesThinClientClient
    kwargs: CreateEnvironmentRequestTypeDef = {...}
    result: CreateEnvironmentResponseTypeDef = await client.create_environment(**kwargs)
```



```python
# ListDevicesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_workspaces_thin_client.client import WorkSpacesThinClientClient
from types_aiobotocore_workspaces_thin_client.paginator import ListDevicesPaginator
from types_aiobotocore_workspaces_thin_client.type_defs import ListDevicesResponseTypeDef


session = get_session()

async with session.create_client("workspaces-thin-client") as client:
    client: WorkSpacesThinClientClient
    paginator: ListDevicesPaginator = client.get_paginator("list_devices")
    async for item in paginator.paginate(...):
        item: ListDevicesResponseTypeDef
        print(item)
```


