<a id="paginators-for-aiobotocore-mediastoredata-module"></a>

# Paginators for aiobotocore MediaStoreData module

> [Index](..) > [MediaStoreData](.) > Paginators

Auto-generated documentation for
[MediaStoreData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
type annotations stubs module
[types-aiobotocore-mediastore-data](https://pypi.org/project/types-aiobotocore-mediastore-data/).

- [Paginators for aiobotocore MediaStoreData module](#paginators-for-aiobotocore-mediastoredata-module)
  - [ListItemsPaginator](#listitemspaginator)

<a id="listitemspaginator"></a>

## ListItemsPaginator

Type annotations for
`session.create_client("mediastore-data").get_paginator("list_items")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediastore_data.paginator import ListItemsPaginator

session = get_session()
async with session.create_client("mediastore-data") as client:
    client: MediaStoreDataClient
    paginator: ListItemsPaginator = client.get_paginator("list_items")
```

Boto3 documentation:
[MediaStoreData.Paginator.ListItems](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData.Paginator.ListItems)

Arguments for `ListItemsPaginator.paginate` method:

- `Path`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListItemsPaginator.paginate` returns
`AsyncIterable`\[[ListItemsResponseTypeDef](./type_defs.md#listitemsresponsetypedef)\].
