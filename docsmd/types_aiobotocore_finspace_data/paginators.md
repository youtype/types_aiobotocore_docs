# Paginators

> [Index](../README.md) > [FinSpaceData](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [FinSpaceData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#finspacedata)
    type annotations stubs module [types-aiobotocore-finspace-data](https://pypi.org/project/types-aiobotocore-finspace-data/).

## ListChangesetsPaginator

Type annotations and code completion for `#!python session.create_client("finspace-data").get_paginator("list_changesets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data/paginator/ListChangesets.html#FinSpaceData.Paginator.ListChangesets)

```python
# ListChangesetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_finspace_data.paginator import ListChangesetsPaginator

session = get_session()
async with session.create_client("finspace-data") as client:  # (1)
    paginator: ListChangesetsPaginator = client.get_paginator("list_changesets")  # (2)
    async for item in paginator.paginate(...):
        item: ListChangesetsResponseTypeDef
        print(item)  # (3)
```

1. client: [FinSpaceDataClient](./client.md)
2. paginator: [ListChangesetsPaginator](./paginators.md#listchangesetspaginator)
3. item: [:material-code-braces: ListChangesetsResponseTypeDef](./type_defs.md#listchangesetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListChangesetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    datasetId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListChangesetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListChangesetsResponseTypeDef](./type_defs.md#listchangesetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListChangesetsRequestPaginateTypeDef = {  # (1)
    "datasetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListChangesetsRequestPaginateTypeDef](./type_defs.md#listchangesetsrequestpaginatetypedef) 
## ListDataViewsPaginator

Type annotations and code completion for `#!python session.create_client("finspace-data").get_paginator("list_data_views")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data/paginator/ListDataViews.html#FinSpaceData.Paginator.ListDataViews)

```python
# ListDataViewsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_finspace_data.paginator import ListDataViewsPaginator

session = get_session()
async with session.create_client("finspace-data") as client:  # (1)
    paginator: ListDataViewsPaginator = client.get_paginator("list_data_views")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataViewsResponseTypeDef
        print(item)  # (3)
```

1. client: [FinSpaceDataClient](./client.md)
2. paginator: [ListDataViewsPaginator](./paginators.md#listdataviewspaginator)
3. item: [:material-code-braces: ListDataViewsResponseTypeDef](./type_defs.md#listdataviewsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDataViewsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    datasetId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDataViewsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDataViewsResponseTypeDef](./type_defs.md#listdataviewsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDataViewsRequestPaginateTypeDef = {  # (1)
    "datasetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataViewsRequestPaginateTypeDef](./type_defs.md#listdataviewsrequestpaginatetypedef) 
## ListDatasetsPaginator

Type annotations and code completion for `#!python session.create_client("finspace-data").get_paginator("list_datasets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data/paginator/ListDatasets.html#FinSpaceData.Paginator.ListDatasets)

```python
# ListDatasetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_finspace_data.paginator import ListDatasetsPaginator

session = get_session()
async with session.create_client("finspace-data") as client:  # (1)
    paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatasetsResponseTypeDef
        print(item)  # (3)
```

1. client: [FinSpaceDataClient](./client.md)
2. paginator: [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
3. item: [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDatasetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDatasetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDatasetsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetsRequestPaginateTypeDef](./type_defs.md#listdatasetsrequestpaginatetypedef) 
## ListPermissionGroupsPaginator

Type annotations and code completion for `#!python session.create_client("finspace-data").get_paginator("list_permission_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data/paginator/ListPermissionGroups.html#FinSpaceData.Paginator.ListPermissionGroups)

```python
# ListPermissionGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_finspace_data.paginator import ListPermissionGroupsPaginator

session = get_session()
async with session.create_client("finspace-data") as client:  # (1)
    paginator: ListPermissionGroupsPaginator = client.get_paginator("list_permission_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListPermissionGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [FinSpaceDataClient](./client.md)
2. paginator: [ListPermissionGroupsPaginator](./paginators.md#listpermissiongroupspaginator)
3. item: [:material-code-braces: ListPermissionGroupsResponseTypeDef](./type_defs.md#listpermissiongroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPermissionGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPermissionGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPermissionGroupsResponseTypeDef](./type_defs.md#listpermissiongroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPermissionGroupsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPermissionGroupsRequestPaginateTypeDef](./type_defs.md#listpermissiongroupsrequestpaginatetypedef) 
## ListUsersPaginator

Type annotations and code completion for `#!python session.create_client("finspace-data").get_paginator("list_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data/paginator/ListUsers.html#FinSpaceData.Paginator.ListUsers)

```python
# ListUsersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_finspace_data.paginator import ListUsersPaginator

session = get_session()
async with session.create_client("finspace-data") as client:  # (1)
    paginator: ListUsersPaginator = client.get_paginator("list_users")  # (2)
    async for item in paginator.paginate(...):
        item: ListUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [FinSpaceDataClient](./client.md)
2. paginator: [ListUsersPaginator](./paginators.md#listuserspaginator)
3. item: [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUsersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListUsersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListUsersRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestPaginateTypeDef](./type_defs.md#listusersrequestpaginatetypedef) 
