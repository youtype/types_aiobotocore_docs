# Paginators

> [Index](../README.md) > [ResourceExplorer](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ResourceExplorer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
    type annotations stubs module [types-aiobotocore-resource-explorer-2](https://pypi.org/project/types-aiobotocore-resource-explorer-2/).

## ListIndexesPaginator

Type annotations and code completion for `#!python session.create_client("resource-explorer-2").get_paginator("list_indexes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListIndexes)

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
) -> AsyncIterator[ListIndexesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: IndexTypeType](./literals.md#indextypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListIndexesOutputTypeDef](./type_defs.md#listindexesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListIndexesInputListIndexesPaginateTypeDef = {  # (1)
    "Regions": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIndexesInputListIndexesPaginateTypeDef](./type_defs.md#listindexesinputlistindexespaginatetypedef) 
## ListSupportedResourceTypesPaginator

Type annotations and code completion for `#!python session.create_client("resource-explorer-2").get_paginator("list_supported_resource_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListSupportedResourceTypes)

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
) -> AsyncIterator[ListSupportedResourceTypesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSupportedResourceTypesOutputTypeDef](./type_defs.md#listsupportedresourcetypesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef](./type_defs.md#listsupportedresourcetypesinputlistsupportedresourcetypespaginatetypedef) 
## ListViewsPaginator

Type annotations and code completion for `#!python session.create_client("resource-explorer-2").get_paginator("list_views")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListViews)

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
) -> AsyncIterator[ListViewsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListViewsOutputTypeDef](./type_defs.md#listviewsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListViewsInputListViewsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListViewsInputListViewsPaginateTypeDef](./type_defs.md#listviewsinputlistviewspaginatetypedef) 
## SearchPaginator

Type annotations and code completion for `#!python session.create_client("resource-explorer-2").get_paginator("search")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.Search)

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
) -> AsyncIterator[SearchOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: SearchOutputTypeDef](./type_defs.md#searchoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchInputSearchPaginateTypeDef = {  # (1)
    "QueryString": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchInputSearchPaginateTypeDef](./type_defs.md#searchinputsearchpaginatetypedef) 
