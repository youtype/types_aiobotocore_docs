# Examples

> [Index](../README.md) > [QApps](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [QApps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#qapps)
    type annotations stubs module [types-aiobotocore-qapps](https://pypi.org/project/types-aiobotocore-qapps/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[qapps]` package installed.

Write your `QApps` code as usual,
type checking and code completion should work out of the box.



```python
# QAppsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("qapps") as client:  # (1)
    result = await client.associate_library_item_review()  # (2)
```

1. client: [QAppsClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# ListLibraryItemsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("qapps") as client:  # (1)
    paginator = client.get_paginator("list_library_items")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [QAppsClient](./client.md)
2. paginator: [ListLibraryItemsPaginator](./paginators.md#listlibraryitemspaginator)
3. item: [:material-code-braces: ListLibraryItemsOutputTypeDef](./type_defs.md#listlibraryitemsoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[qapps]`
or a standalone `types_aiobotocore_qapps` package, you have to explicitly specify
`client: QAppsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# QAppsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_qapps.client import QAppsClient
from types_aiobotocore_qapps.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_qapps.type_defs import AssociateLibraryItemReviewInputTypeDef


session = get_session()

async with session.create_client("qapps") as client:
    client: QAppsClient
    kwargs: AssociateLibraryItemReviewInputTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.associate_library_item_review(**kwargs)
```



```python
# ListLibraryItemsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_qapps.client import QAppsClient
from types_aiobotocore_qapps.paginator import ListLibraryItemsPaginator
from types_aiobotocore_qapps.type_defs import ListLibraryItemsOutputTypeDef


session = get_session()

async with session.create_client("qapps") as client:
    client: QAppsClient
    paginator: ListLibraryItemsPaginator = client.get_paginator("list_library_items")
    async for item in paginator.paginate(...):
        item: ListLibraryItemsOutputTypeDef
        print(item)
```


