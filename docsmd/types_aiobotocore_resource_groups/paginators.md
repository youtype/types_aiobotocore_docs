# Paginators

> [Index](../README.md) > [ResourceGroups](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ResourceGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#resourcegroups)
    type annotations stubs module [types-aiobotocore-resource-groups](https://pypi.org/project/types-aiobotocore-resource-groups/).

## ListGroupResourcesPaginator

Type annotations and code completion for `#!python session.create_client("resource-groups").get_paginator("list_group_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups/paginator/ListGroupResources.html#ResourceGroups.Paginator.ListGroupResources)

```python
# ListGroupResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_groups.paginator import ListGroupResourcesPaginator

session = get_session()
async with session.create_client("resource-groups") as client:  # (1)
    paginator: ListGroupResourcesPaginator = client.get_paginator("list_group_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupResourcesOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceGroupsClient](./client.md)
2. paginator: [ListGroupResourcesPaginator](./paginators.md#listgroupresourcespaginator)
3. item: [:material-code-braces: ListGroupResourcesOutputTypeDef](./type_defs.md#listgroupresourcesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GroupName: str = ...,
    Group: str = ...,
    Filters: Sequence[ResourceFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListGroupResourcesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ResourceFilterTypeDef](./type_defs.md#resourcefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListGroupResourcesOutputTypeDef](./type_defs.md#listgroupresourcesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGroupResourcesInputPaginateTypeDef = {  # (1)
    "GroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupResourcesInputPaginateTypeDef](./type_defs.md#listgroupresourcesinputpaginatetypedef) 
## ListGroupingStatusesPaginator

Type annotations and code completion for `#!python session.create_client("resource-groups").get_paginator("list_grouping_statuses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups/paginator/ListGroupingStatuses.html#ResourceGroups.Paginator.ListGroupingStatuses)

```python
# ListGroupingStatusesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_groups.paginator import ListGroupingStatusesPaginator

session = get_session()
async with session.create_client("resource-groups") as client:  # (1)
    paginator: ListGroupingStatusesPaginator = client.get_paginator("list_grouping_statuses")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupingStatusesOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceGroupsClient](./client.md)
2. paginator: [ListGroupingStatusesPaginator](./paginators.md#listgroupingstatusespaginator)
3. item: [:material-code-braces: ListGroupingStatusesOutputTypeDef](./type_defs.md#listgroupingstatusesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupingStatusesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Group: str,
    Filters: Sequence[ListGroupingStatusesFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListGroupingStatusesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ListGroupingStatusesFilterTypeDef](./type_defs.md#listgroupingstatusesfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListGroupingStatusesOutputTypeDef](./type_defs.md#listgroupingstatusesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGroupingStatusesInputPaginateTypeDef = {  # (1)
    "Group": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupingStatusesInputPaginateTypeDef](./type_defs.md#listgroupingstatusesinputpaginatetypedef) 
## ListGroupsPaginator

Type annotations and code completion for `#!python session.create_client("resource-groups").get_paginator("list_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups/paginator/ListGroups.html#ResourceGroups.Paginator.ListGroups)

```python
# ListGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_groups.paginator import ListGroupsPaginator

session = get_session()
async with session.create_client("resource-groups") as client:  # (1)
    paginator: ListGroupsPaginator = client.get_paginator("list_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupsOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceGroupsClient](./client.md)
2. paginator: [ListGroupsPaginator](./paginators.md#listgroupspaginator)
3. item: [:material-code-braces: ListGroupsOutputTypeDef](./type_defs.md#listgroupsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[GroupFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListGroupsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: GroupFilterTypeDef](./type_defs.md#groupfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListGroupsOutputTypeDef](./type_defs.md#listgroupsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGroupsInputPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupsInputPaginateTypeDef](./type_defs.md#listgroupsinputpaginatetypedef) 
## ListTagSyncTasksPaginator

Type annotations and code completion for `#!python session.create_client("resource-groups").get_paginator("list_tag_sync_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups/paginator/ListTagSyncTasks.html#ResourceGroups.Paginator.ListTagSyncTasks)

```python
# ListTagSyncTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_groups.paginator import ListTagSyncTasksPaginator

session = get_session()
async with session.create_client("resource-groups") as client:  # (1)
    paginator: ListTagSyncTasksPaginator = client.get_paginator("list_tag_sync_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagSyncTasksOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceGroupsClient](./client.md)
2. paginator: [ListTagSyncTasksPaginator](./paginators.md#listtagsynctaskspaginator)
3. item: [:material-code-braces: ListTagSyncTasksOutputTypeDef](./type_defs.md#listtagsynctasksoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListTagSyncTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[ListTagSyncTasksFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListTagSyncTasksOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ListTagSyncTasksFilterTypeDef](./type_defs.md#listtagsynctasksfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListTagSyncTasksOutputTypeDef](./type_defs.md#listtagsynctasksoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTagSyncTasksInputPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagSyncTasksInputPaginateTypeDef](./type_defs.md#listtagsynctasksinputpaginatetypedef) 
## SearchResourcesPaginator

Type annotations and code completion for `#!python session.create_client("resource-groups").get_paginator("search_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups/paginator/SearchResources.html#ResourceGroups.Paginator.SearchResources)

```python
# SearchResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_groups.paginator import SearchResourcesPaginator

session = get_session()
async with session.create_client("resource-groups") as client:  # (1)
    paginator: SearchResourcesPaginator = client.get_paginator("search_resources")  # (2)
    async for item in paginator.paginate(...):
        item: SearchResourcesOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceGroupsClient](./client.md)
2. paginator: [SearchResourcesPaginator](./paginators.md#searchresourcespaginator)
3. item: [:material-code-braces: SearchResourcesOutputTypeDef](./type_defs.md#searchresourcesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python SearchResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceQuery: ResourceQueryTypeDef,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[SearchResourcesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ResourceQueryTypeDef](./type_defs.md#resourcequerytypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SearchResourcesOutputTypeDef](./type_defs.md#searchresourcesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchResourcesInputPaginateTypeDef = {  # (1)
    "ResourceQuery": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchResourcesInputPaginateTypeDef](./type_defs.md#searchresourcesinputpaginatetypedef) 
