<a id="examples-for-aiobotocore-mediastoredata-module"></a>

# Examples for aiobotocore MediaStoreData module

> [Index](../README.md) > [MediaStoreData](./README.md) > Examples

- [Examples for aiobotocore MediaStoreData module](#examples-for-aiobotocore-mediastoredata-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[mediastore-data]` package installed.

Write your `MediaStoreData` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type MediaStoreDataClient
# and provides type checking and code completion
async with session.create_client("mediastore-data") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListItemsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_items")
    async for item in paginator.paginate(...):
        # item has type ListItemsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[mediastore-data]` or a standalone
`types_aiobotocore_mediastore_data` package, you have to explicitly specify
`client: MediaStoreDataClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediastore_data.client import MediaStoreDataClient
from types_aiobotocore_mediastore_data.type_defs import bool
from types_aiobotocore_mediastore_data.paginator import ListItemsPaginator

from types_aiobotocore_mediastore_data.literals import PaginatorName



session = get_session()

async with session.create_client("mediastore-data") as client:
    client: MediaStoreDataClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_items"
    paginator: ListItemsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListItemsResponseTypeDef
        print(item)
    

    
```
