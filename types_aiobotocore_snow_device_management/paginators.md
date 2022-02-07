<a id="paginators-for-aiobotocore-snowdevicemanagement-module"></a>

# Paginators for aiobotocore SnowDeviceManagement module

> [Index](..) > [SnowDeviceManagement](.) > Paginators

Auto-generated documentation for
[SnowDeviceManagement](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement)
type annotations stubs module
[types-aiobotocore-snow-device-management](https://pypi.org/project/types-aiobotocore-snow-device-management/).

- [Paginators for aiobotocore SnowDeviceManagement module](#paginators-for-aiobotocore-snowdevicemanagement-module)
  - [ListDeviceResourcesPaginator](#listdeviceresourcespaginator)
  - [ListDevicesPaginator](#listdevicespaginator)
  - [ListExecutionsPaginator](#listexecutionspaginator)
  - [ListTasksPaginator](#listtaskspaginator)

<a id="listdeviceresourcespaginator"></a>

## ListDeviceResourcesPaginator

Type annotations for
`session.create_client("snow-device-management").get_paginator("list_device_resources")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_snow_device_management.paginator import ListDeviceResourcesPaginator

session = get_session()
async with session.create_client("snow-device-management") as client:
    client: SnowDeviceManagementClient
    paginator: ListDeviceResourcesPaginator = client.get_paginator("list_device_resources")
```

Boto3 documentation:
[SnowDeviceManagement.Paginator.ListDeviceResources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListDeviceResources)

Arguments for `ListDeviceResourcesPaginator.paginate` method:

- `managedDeviceId`: `str` *(required)*
- `type`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDeviceResourcesPaginator.paginate` returns
`_PageIterator`\[[ListDeviceResourcesOutputTypeDef](./type_defs.md#listdeviceresourcesoutputtypedef)\].

<a id="listdevicespaginator"></a>

## ListDevicesPaginator

Type annotations for
`session.create_client("snow-device-management").get_paginator("list_devices")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_snow_device_management.paginator import ListDevicesPaginator

session = get_session()
async with session.create_client("snow-device-management") as client:
    client: SnowDeviceManagementClient
    paginator: ListDevicesPaginator = client.get_paginator("list_devices")
```

Boto3 documentation:
[SnowDeviceManagement.Paginator.ListDevices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListDevices)

Arguments for `ListDevicesPaginator.paginate` method:

- `jobId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDevicesPaginator.paginate` returns
`_PageIterator`\[[ListDevicesOutputTypeDef](./type_defs.md#listdevicesoutputtypedef)\].

<a id="listexecutionspaginator"></a>

## ListExecutionsPaginator

Type annotations for
`session.create_client("snow-device-management").get_paginator("list_executions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_snow_device_management.paginator import ListExecutionsPaginator

session = get_session()
async with session.create_client("snow-device-management") as client:
    client: SnowDeviceManagementClient
    paginator: ListExecutionsPaginator = client.get_paginator("list_executions")
```

Boto3 documentation:
[SnowDeviceManagement.Paginator.ListExecutions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListExecutions)

Arguments for `ListExecutionsPaginator.paginate` method:

- `taskId`: `str` *(required)*
- `state`: [ExecutionStateType](./literals.md#executionstatetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListExecutionsPaginator.paginate` returns
`_PageIterator`\[[ListExecutionsOutputTypeDef](./type_defs.md#listexecutionsoutputtypedef)\].

<a id="listtaskspaginator"></a>

## ListTasksPaginator

Type annotations for
`session.create_client("snow-device-management").get_paginator("list_tasks")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_snow_device_management.paginator import ListTasksPaginator

session = get_session()
async with session.create_client("snow-device-management") as client:
    client: SnowDeviceManagementClient
    paginator: ListTasksPaginator = client.get_paginator("list_tasks")
```

Boto3 documentation:
[SnowDeviceManagement.Paginator.ListTasks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListTasks)

Arguments for `ListTasksPaginator.paginate` method:

- `state`: [TaskStateType](./literals.md#taskstatetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTasksPaginator.paginate` returns
`_PageIterator`\[[ListTasksOutputTypeDef](./type_defs.md#listtasksoutputtypedef)\].
