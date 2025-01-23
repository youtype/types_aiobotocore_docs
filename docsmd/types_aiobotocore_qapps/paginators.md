# Paginators

> [Index](../README.md) > [QApps](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [QApps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#qapps)
    type annotations stubs module [types-aiobotocore-qapps](https://pypi.org/project/types-aiobotocore-qapps/).

## ListLibraryItemsPaginator

Type annotations and code completion for `#!python session.create_client("qapps").get_paginator("list_library_items")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/paginator/ListLibraryItems.html#QApps.Paginator.ListLibraryItems)

```python
# ListLibraryItemsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qapps.paginator import ListLibraryItemsPaginator

session = get_session()
async with session.create_client("qapps") as client:  # (1)
    paginator: ListLibraryItemsPaginator = client.get_paginator("list_library_items")  # (2)
    async for item in paginator.paginate(...):
        item: ListLibraryItemsOutputTypeDef
        print(item)  # (3)
```

1. client: [QAppsClient](./client.md)
2. paginator: [ListLibraryItemsPaginator](./paginators.md#listlibraryitemspaginator)
3. item: [:material-code-braces: ListLibraryItemsOutputTypeDef](./type_defs.md#listlibraryitemsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListLibraryItemsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    instanceId: str,
    categoryId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListLibraryItemsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListLibraryItemsOutputTypeDef](./type_defs.md#listlibraryitemsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListLibraryItemsInputPaginateTypeDef = {  # (1)
    "instanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLibraryItemsInputPaginateTypeDef](./type_defs.md#listlibraryitemsinputpaginatetypedef) 
## ListQAppsPaginator

Type annotations and code completion for `#!python session.create_client("qapps").get_paginator("list_q_apps")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/paginator/ListQApps.html#QApps.Paginator.ListQApps)

```python
# ListQAppsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qapps.paginator import ListQAppsPaginator

session = get_session()
async with session.create_client("qapps") as client:  # (1)
    paginator: ListQAppsPaginator = client.get_paginator("list_q_apps")  # (2)
    async for item in paginator.paginate(...):
        item: ListQAppsOutputTypeDef
        print(item)  # (3)
```

1. client: [QAppsClient](./client.md)
2. paginator: [ListQAppsPaginator](./paginators.md#listqappspaginator)
3. item: [:material-code-braces: ListQAppsOutputTypeDef](./type_defs.md#listqappsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListQAppsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    instanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListQAppsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListQAppsOutputTypeDef](./type_defs.md#listqappsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListQAppsInputPaginateTypeDef = {  # (1)
    "instanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListQAppsInputPaginateTypeDef](./type_defs.md#listqappsinputpaginatetypedef) 
