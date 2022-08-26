# Paginators

> [Index](../README.md) > [MediaStoreData](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MediaStoreData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
    type annotations stubs module [types-aiobotocore-mediastore-data](https://pypi.org/project/types-aiobotocore-mediastore-data/).

## ListItemsPaginator

Type annotations and code completion for `#!python session.create_client("mediastore-data").get_paginator("list_items")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData.Paginator.ListItems)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mediastore_data.paginator import ListItemsPaginator

session = get_session()
async with session.create_client("mediastore-data") as client:  # (1)
    paginator: ListItemsPaginator = client.get_paginator("list_items")  # (2)
    async for item in paginator.paginate(...):
        item: ListItemsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaStoreDataClient](./client.md)
2. paginator: [ListItemsPaginator](./paginators.md#listitemspaginator)
3. item: [:material-code-braces: ListItemsResponseTypeDef](./type_defs.md#listitemsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListItemsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Path: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListItemsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListItemsResponseTypeDef](./type_defs.md#listitemsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListItemsRequestListItemsPaginateTypeDef = {  # (1)
    "Path": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListItemsRequestListItemsPaginateTypeDef](./type_defs.md#listitemsrequestlistitemspaginatetypedef) 
