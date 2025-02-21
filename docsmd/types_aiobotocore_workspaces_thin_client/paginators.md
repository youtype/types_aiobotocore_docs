# Paginators

> [Index](../README.md) > [WorkSpacesThinClient](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [WorkSpacesThinClient](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#workspacesthinclient)
    type annotations stubs module [types-aiobotocore-workspaces-thin-client](https://pypi.org/project/types-aiobotocore-workspaces-thin-client/).

## ListDevicesPaginator

Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").get_paginator("list_devices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client/paginator/ListDevices.html#WorkSpacesThinClient.Paginator.ListDevices)

```python
# ListDevicesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workspaces_thin_client.paginator import ListDevicesPaginator

session = get_session()
async with session.create_client("workspaces-thin-client") as client:  # (1)
    paginator: ListDevicesPaginator = client.get_paginator("list_devices")  # (2)
    async for item in paginator.paginate(...):
        item: ListDevicesResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkSpacesThinClientClient](./client.md)
2. paginator: [ListDevicesPaginator](./paginators.md#listdevicespaginator)
3. item: [:material-code-braces: ListDevicesResponseTypeDef](./type_defs.md#listdevicesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDevicesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDevicesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDevicesResponseTypeDef](./type_defs.md#listdevicesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDevicesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDevicesRequestPaginateTypeDef](./type_defs.md#listdevicesrequestpaginatetypedef) 
## ListEnvironmentsPaginator

Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").get_paginator("list_environments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client/paginator/ListEnvironments.html#WorkSpacesThinClient.Paginator.ListEnvironments)

```python
# ListEnvironmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workspaces_thin_client.paginator import ListEnvironmentsPaginator

session = get_session()
async with session.create_client("workspaces-thin-client") as client:  # (1)
    paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnvironmentsResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkSpacesThinClientClient](./client.md)
2. paginator: [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
3. item: [:material-code-braces: ListEnvironmentsResponseTypeDef](./type_defs.md#listenvironmentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEnvironmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEnvironmentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEnvironmentsResponseTypeDef](./type_defs.md#listenvironmentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEnvironmentsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentsRequestPaginateTypeDef](./type_defs.md#listenvironmentsrequestpaginatetypedef) 
## ListSoftwareSetsPaginator

Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").get_paginator("list_software_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client/paginator/ListSoftwareSets.html#WorkSpacesThinClient.Paginator.ListSoftwareSets)

```python
# ListSoftwareSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workspaces_thin_client.paginator import ListSoftwareSetsPaginator

session = get_session()
async with session.create_client("workspaces-thin-client") as client:  # (1)
    paginator: ListSoftwareSetsPaginator = client.get_paginator("list_software_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListSoftwareSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkSpacesThinClientClient](./client.md)
2. paginator: [ListSoftwareSetsPaginator](./paginators.md#listsoftwaresetspaginator)
3. item: [:material-code-braces: ListSoftwareSetsResponseTypeDef](./type_defs.md#listsoftwaresetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSoftwareSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSoftwareSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSoftwareSetsResponseTypeDef](./type_defs.md#listsoftwaresetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSoftwareSetsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSoftwareSetsRequestPaginateTypeDef](./type_defs.md#listsoftwaresetsrequestpaginatetypedef) 
