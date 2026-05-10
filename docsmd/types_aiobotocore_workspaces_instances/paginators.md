# Paginators

> [Index](../README.md) > [WorkspacesInstances](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [WorkspacesInstances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances.html#workspacesinstances)
    type annotations stubs module [types-aiobotocore-workspaces-instances](https://pypi.org/project/types-aiobotocore-workspaces-instances/).

## ListInstanceTypesPaginator

Type annotations and code completion for `#!python session.create_client("workspaces-instances").get_paginator("list_instance_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances/paginator/ListInstanceTypes.html#WorkspacesInstances.Paginator.ListInstanceTypes)

```python
# ListInstanceTypesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workspaces_instances.paginator import ListInstanceTypesPaginator

session = get_session()
async with session.create_client("workspaces-instances") as client:  # (1)
    paginator: ListInstanceTypesPaginator = client.get_paginator("list_instance_types")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstanceTypesResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkspacesInstancesClient](./client.md)
2. paginator: [ListInstanceTypesPaginator](./paginators.md#listinstancetypespaginator)
3. item: `AioPageIterator[ListInstanceTypesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListInstanceTypesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceConfigurationFilter: InstanceConfigurationFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListInstanceTypesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: InstanceConfigurationFilterTypeDef](./type_defs.md#instanceconfigurationfiltertypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListInstanceTypesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListInstanceTypesRequestPaginateTypeDef = {  # (1)
    "InstanceConfigurationFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstanceTypesRequestPaginateTypeDef](./type_defs.md#listinstancetypesrequestpaginatetypedef)
## ListRegionsPaginator

Type annotations and code completion for `#!python session.create_client("workspaces-instances").get_paginator("list_regions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances/paginator/ListRegions.html#WorkspacesInstances.Paginator.ListRegions)

```python
# ListRegionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workspaces_instances.paginator import ListRegionsPaginator

session = get_session()
async with session.create_client("workspaces-instances") as client:  # (1)
    paginator: ListRegionsPaginator = client.get_paginator("list_regions")  # (2)
    async for item in paginator.paginate(...):
        item: ListRegionsResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkspacesInstancesClient](./client.md)
2. paginator: [ListRegionsPaginator](./paginators.md#listregionspaginator)
3. item: `AioPageIterator[ListRegionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRegionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRegionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRegionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRegionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRegionsRequestPaginateTypeDef](./type_defs.md#listregionsrequestpaginatetypedef)
## ListWorkspaceInstancesPaginator

Type annotations and code completion for `#!python session.create_client("workspaces-instances").get_paginator("list_workspace_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances/paginator/ListWorkspaceInstances.html#WorkspacesInstances.Paginator.ListWorkspaceInstances)

```python
# ListWorkspaceInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workspaces_instances.paginator import ListWorkspaceInstancesPaginator

session = get_session()
async with session.create_client("workspaces-instances") as client:  # (1)
    paginator: ListWorkspaceInstancesPaginator = client.get_paginator("list_workspace_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkspaceInstancesResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkspacesInstancesClient](./client.md)
2. paginator: [ListWorkspaceInstancesPaginator](./paginators.md#listworkspaceinstancespaginator)
3. item: `AioPageIterator[ListWorkspaceInstancesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListWorkspaceInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ProvisionStates: Sequence[ProvisionStateEnumType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListWorkspaceInstancesResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[ProvisionStateEnumType]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListWorkspaceInstancesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkspaceInstancesRequestPaginateTypeDef = {  # (1)
    "ProvisionStates": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkspaceInstancesRequestPaginateTypeDef](./type_defs.md#listworkspaceinstancesrequestpaginatetypedef)
