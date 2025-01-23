# Paginators

> [Index](../README.md) > [SnowDeviceManagement](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SnowDeviceManagement](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#snowdevicemanagement)
    type annotations stubs module [types-aiobotocore-snow-device-management](https://pypi.org/project/types-aiobotocore-snow-device-management/).

## ListDeviceResourcesPaginator

Type annotations and code completion for `#!python session.create_client("snow-device-management").get_paginator("list_device_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management/paginator/ListDeviceResources.html#SnowDeviceManagement.Paginator.ListDeviceResources)

```python
# ListDeviceResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_snow_device_management.paginator import ListDeviceResourcesPaginator

session = get_session()
async with session.create_client("snow-device-management") as client:  # (1)
    paginator: ListDeviceResourcesPaginator = client.get_paginator("list_device_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeviceResourcesOutputTypeDef
        print(item)  # (3)
```

1. client: [SnowDeviceManagementClient](./client.md)
2. paginator: [ListDeviceResourcesPaginator](./paginators.md#listdeviceresourcespaginator)
3. item: [:material-code-braces: ListDeviceResourcesOutputTypeDef](./type_defs.md#listdeviceresourcesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListDeviceResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    managedDeviceId: str,
    type: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDeviceResourcesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDeviceResourcesOutputTypeDef](./type_defs.md#listdeviceresourcesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDeviceResourcesInputPaginateTypeDef = {  # (1)
    "managedDeviceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeviceResourcesInputPaginateTypeDef](./type_defs.md#listdeviceresourcesinputpaginatetypedef) 
## ListDevicesPaginator

Type annotations and code completion for `#!python session.create_client("snow-device-management").get_paginator("list_devices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management/paginator/ListDevices.html#SnowDeviceManagement.Paginator.ListDevices)

```python
# ListDevicesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_snow_device_management.paginator import ListDevicesPaginator

session = get_session()
async with session.create_client("snow-device-management") as client:  # (1)
    paginator: ListDevicesPaginator = client.get_paginator("list_devices")  # (2)
    async for item in paginator.paginate(...):
        item: ListDevicesOutputTypeDef
        print(item)  # (3)
```

1. client: [SnowDeviceManagementClient](./client.md)
2. paginator: [ListDevicesPaginator](./paginators.md#listdevicespaginator)
3. item: [:material-code-braces: ListDevicesOutputTypeDef](./type_defs.md#listdevicesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListDevicesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    jobId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDevicesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDevicesOutputTypeDef](./type_defs.md#listdevicesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDevicesInputPaginateTypeDef = {  # (1)
    "jobId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDevicesInputPaginateTypeDef](./type_defs.md#listdevicesinputpaginatetypedef) 
## ListExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("snow-device-management").get_paginator("list_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management/paginator/ListExecutions.html#SnowDeviceManagement.Paginator.ListExecutions)

```python
# ListExecutionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_snow_device_management.paginator import ListExecutionsPaginator

session = get_session()
async with session.create_client("snow-device-management") as client:  # (1)
    paginator: ListExecutionsPaginator = client.get_paginator("list_executions")  # (2)
    async for item in paginator.paginate(...):
        item: ListExecutionsOutputTypeDef
        print(item)  # (3)
```

1. client: [SnowDeviceManagementClient](./client.md)
2. paginator: [ListExecutionsPaginator](./paginators.md#listexecutionspaginator)
3. item: [:material-code-braces: ListExecutionsOutputTypeDef](./type_defs.md#listexecutionsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListExecutionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    taskId: str,
    state: ExecutionStateType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListExecutionsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ExecutionStateType](./literals.md#executionstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListExecutionsOutputTypeDef](./type_defs.md#listexecutionsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListExecutionsInputPaginateTypeDef = {  # (1)
    "taskId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListExecutionsInputPaginateTypeDef](./type_defs.md#listexecutionsinputpaginatetypedef) 
## ListTasksPaginator

Type annotations and code completion for `#!python session.create_client("snow-device-management").get_paginator("list_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management/paginator/ListTasks.html#SnowDeviceManagement.Paginator.ListTasks)

```python
# ListTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_snow_device_management.paginator import ListTasksPaginator

session = get_session()
async with session.create_client("snow-device-management") as client:  # (1)
    paginator: ListTasksPaginator = client.get_paginator("list_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: ListTasksOutputTypeDef
        print(item)  # (3)
```

1. client: [SnowDeviceManagementClient](./client.md)
2. paginator: [ListTasksPaginator](./paginators.md#listtaskspaginator)
3. item: [:material-code-braces: ListTasksOutputTypeDef](./type_defs.md#listtasksoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    state: TaskStateType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListTasksOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: TaskStateType](./literals.md#taskstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListTasksOutputTypeDef](./type_defs.md#listtasksoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTasksInputPaginateTypeDef = {  # (1)
    "state": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTasksInputPaginateTypeDef](./type_defs.md#listtasksinputpaginatetypedef) 
