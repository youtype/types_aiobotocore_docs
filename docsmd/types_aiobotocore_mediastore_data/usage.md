# Examples

> [Index](../README.md) > [MediaStoreData](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MediaStoreData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#mediastoredata)
    type annotations stubs module [types-aiobotocore-mediastore-data](https://pypi.org/project/types-aiobotocore-mediastore-data/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[mediastore-data]` package installed.

Write your `MediaStoreData` code as usual,
type checking and code completion should work out of the box.



```python
# MediaStoreDataClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("mediastore-data") as client:  # (1)
    result = await client.describe_object()  # (2)
```

1. client: [MediaStoreDataClient](./client.md)
2. result: [:material-code-braces: DescribeObjectResponseTypeDef](./type_defs.md#describeobjectresponsetypedef) 



```python
# ListItemsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("mediastore-data") as client:  # (1)
    paginator = client.get_paginator("list_items")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MediaStoreDataClient](./client.md)
2. paginator: [ListItemsPaginator](./paginators.md#listitemspaginator)
3. item: [:material-code-braces: ListItemsResponseTypeDef](./type_defs.md#listitemsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[mediastore-data]`
or a standalone `types_aiobotocore_mediastore_data` package, you have to explicitly specify
`client: MediaStoreDataClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# MediaStoreDataClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_mediastore_data.client import MediaStoreDataClient
from types_aiobotocore_mediastore_data.type_defs import DescribeObjectResponseTypeDef
from types_aiobotocore_mediastore_data.type_defs import DescribeObjectRequestTypeDef


session = get_session()

async with session.create_client("mediastore-data") as client:
    client: MediaStoreDataClient
    kwargs: DescribeObjectRequestTypeDef = {...}
    result: DescribeObjectResponseTypeDef = await client.describe_object(**kwargs)
```



```python
# ListItemsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_mediastore_data.client import MediaStoreDataClient
from types_aiobotocore_mediastore_data.paginator import ListItemsPaginator
from types_aiobotocore_mediastore_data.type_defs import ListItemsResponseTypeDef


session = get_session()

async with session.create_client("mediastore-data") as client:
    client: MediaStoreDataClient
    paginator: ListItemsPaginator = client.get_paginator("list_items")
    async for item in paginator.paginate(...):
        item: ListItemsResponseTypeDef
        print(item)
```


