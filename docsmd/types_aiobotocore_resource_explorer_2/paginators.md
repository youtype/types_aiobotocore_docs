# Paginators

> [Index](../README.md) > [ResourceExplorer](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ResourceExplorer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#resourceexplorer)
    type annotations stubs module [types-aiobotocore-resource-explorer-2](https://pypi.org/project/types-aiobotocore-resource-explorer-2/).

## ListIndexesForMembersPaginator

Type annotations and code completion for `#!python session.create_client("resource-explorer-2").get_paginator("list_indexes_for_members")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2/paginator/ListIndexesForMembers.html#ResourceExplorer.Paginator.ListIndexesForMembers)

```python
# ListIndexesForMembersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_explorer_2.paginator import ListIndexesForMembersPaginator

session = get_session()
async with session.create_client("resource-explorer-2") as client:  # (1)
    paginator: ListIndexesForMembersPaginator = client.get_paginator("list_indexes_for_members")  # (2)
    async for item in paginator.paginate(...):
        item: ListIndexesForMembersOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [ListIndexesForMembersPaginator](./paginators.md#listindexesformemberspaginator)
3. item: [:material-code-braces: ListIndexesForMembersOutputTypeDef](./type_defs.md#listindexesformembersoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListIndexesForMembersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccountIdList: Sequence[str],
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListIndexesForMembersOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListIndexesForMembersOutputTypeDef](./type_defs.md#listindexesformembersoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListIndexesForMembersInputPaginateTypeDef = {  # (1)
    "AccountIdList": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIndexesForMembersInputPaginateTypeDef](./type_defs.md#listindexesformembersinputpaginatetypedef) 
## ListIndexesPaginator

Type annotations and code completion for `#!python session.create_client("resource-explorer-2").get_paginator("list_indexes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2/paginator/ListIndexes.html#ResourceExplorer.Paginator.ListIndexes)

```python
# ListIndexesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_explorer_2.paginator import ListIndexesPaginator

session = get_session()
async with session.create_client("resource-explorer-2") as client:  # (1)
    paginator: ListIndexesPaginator = client.get_paginator("list_indexes")  # (2)
    async for item in paginator.paginate(...):
        item: ListIndexesOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [ListIndexesPaginator](./paginators.md#listindexespaginator)
3. item: [:material-code-braces: ListIndexesOutputTypeDef](./type_defs.md#listindexesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListIndexesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Regions: Sequence[str] = ...,
    Type: IndexTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListIndexesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: IndexTypeType](./literals.md#indextypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListIndexesOutputTypeDef](./type_defs.md#listindexesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListIndexesInputPaginateTypeDef = {  # (1)
    "Regions": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIndexesInputPaginateTypeDef](./type_defs.md#listindexesinputpaginatetypedef) 
## ListManagedViewsPaginator

Type annotations and code completion for `#!python session.create_client("resource-explorer-2").get_paginator("list_managed_views")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2/paginator/ListManagedViews.html#ResourceExplorer.Paginator.ListManagedViews)

```python
# ListManagedViewsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_explorer_2.paginator import ListManagedViewsPaginator

session = get_session()
async with session.create_client("resource-explorer-2") as client:  # (1)
    paginator: ListManagedViewsPaginator = client.get_paginator("list_managed_views")  # (2)
    async for item in paginator.paginate(...):
        item: ListManagedViewsOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [ListManagedViewsPaginator](./paginators.md#listmanagedviewspaginator)
3. item: [:material-code-braces: ListManagedViewsOutputTypeDef](./type_defs.md#listmanagedviewsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListManagedViewsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ServicePrincipal: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListManagedViewsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListManagedViewsOutputTypeDef](./type_defs.md#listmanagedviewsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListManagedViewsInputPaginateTypeDef = {  # (1)
    "ServicePrincipal": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListManagedViewsInputPaginateTypeDef](./type_defs.md#listmanagedviewsinputpaginatetypedef) 
## ListResourcesPaginator

Type annotations and code completion for `#!python session.create_client("resource-explorer-2").get_paginator("list_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2/paginator/ListResources.html#ResourceExplorer.Paginator.ListResources)

```python
# ListResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_explorer_2.paginator import ListResourcesPaginator

session = get_session()
async with session.create_client("resource-explorer-2") as client:  # (1)
    paginator: ListResourcesPaginator = client.get_paginator("list_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourcesOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [ListResourcesPaginator](./paginators.md#listresourcespaginator)
3. item: [:material-code-braces: ListResourcesOutputTypeDef](./type_defs.md#listresourcesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: SearchFilterTypeDef = ...,  # (1)
    ViewArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListResourcesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SearchFilterTypeDef](./type_defs.md#searchfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListResourcesOutputTypeDef](./type_defs.md#listresourcesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResourcesInputPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourcesInputPaginateTypeDef](./type_defs.md#listresourcesinputpaginatetypedef) 
## ListSupportedResourceTypesPaginator

Type annotations and code completion for `#!python session.create_client("resource-explorer-2").get_paginator("list_supported_resource_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2/paginator/ListSupportedResourceTypes.html#ResourceExplorer.Paginator.ListSupportedResourceTypes)

```python
# ListSupportedResourceTypesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_explorer_2.paginator import ListSupportedResourceTypesPaginator

session = get_session()
async with session.create_client("resource-explorer-2") as client:  # (1)
    paginator: ListSupportedResourceTypesPaginator = client.get_paginator("list_supported_resource_types")  # (2)
    async for item in paginator.paginate(...):
        item: ListSupportedResourceTypesOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [ListSupportedResourceTypesPaginator](./paginators.md#listsupportedresourcetypespaginator)
3. item: [:material-code-braces: ListSupportedResourceTypesOutputTypeDef](./type_defs.md#listsupportedresourcetypesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSupportedResourceTypesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSupportedResourceTypesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSupportedResourceTypesOutputTypeDef](./type_defs.md#listsupportedresourcetypesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSupportedResourceTypesInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSupportedResourceTypesInputPaginateTypeDef](./type_defs.md#listsupportedresourcetypesinputpaginatetypedef) 
## ListViewsPaginator

Type annotations and code completion for `#!python session.create_client("resource-explorer-2").get_paginator("list_views")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2/paginator/ListViews.html#ResourceExplorer.Paginator.ListViews)

```python
# ListViewsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_explorer_2.paginator import ListViewsPaginator

session = get_session()
async with session.create_client("resource-explorer-2") as client:  # (1)
    paginator: ListViewsPaginator = client.get_paginator("list_views")  # (2)
    async for item in paginator.paginate(...):
        item: ListViewsOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [ListViewsPaginator](./paginators.md#listviewspaginator)
3. item: [:material-code-braces: ListViewsOutputTypeDef](./type_defs.md#listviewsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListViewsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListViewsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListViewsOutputTypeDef](./type_defs.md#listviewsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListViewsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListViewsInputPaginateTypeDef](./type_defs.md#listviewsinputpaginatetypedef) 
## SearchPaginator

Type annotations and code completion for `#!python session.create_client("resource-explorer-2").get_paginator("search")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2/paginator/Search.html#ResourceExplorer.Paginator.Search)

```python
# SearchPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_explorer_2.paginator import SearchPaginator

session = get_session()
async with session.create_client("resource-explorer-2") as client:  # (1)
    paginator: SearchPaginator = client.get_paginator("search")  # (2)
    async for item in paginator.paginate(...):
        item: SearchOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [SearchPaginator](./paginators.md#searchpaginator)
3. item: [:material-code-braces: SearchOutputTypeDef](./type_defs.md#searchoutputtypedef) 


### paginate

Type annotations and code completion for `#!python SearchPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    QueryString: str,
    ViewArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[SearchOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: SearchOutputTypeDef](./type_defs.md#searchoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchInputPaginateTypeDef = {  # (1)
    "QueryString": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchInputPaginateTypeDef](./type_defs.md#searchinputpaginatetypedef) 
