<a id="examples-for-aiobotocore-mediapackagevod-module"></a>

# Examples for aiobotocore MediaPackageVod module

> [Index](../README.md) > [MediaPackageVod](./README.md) > Examples

- [Examples for aiobotocore MediaPackageVod module](#examples-for-aiobotocore-mediapackagevod-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[mediapackage-vod]` package installed.

Write your `MediaPackageVod` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type MediaPackageVodClient
# and provides type checking and code completion
async with session.create_client("mediapackage-vod") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListAssetsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_assets")
    async for item in paginator.paginate(...):
        # item has type ListAssetsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[mediapackage-vod]` or a standalone
`types_aiobotocore_mediapackage_vod` package, you have to explicitly specify
`client: MediaPackageVodClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediapackage_vod.client import MediaPackageVodClient
from types_aiobotocore_mediapackage_vod.type_defs import bool
from types_aiobotocore_mediapackage_vod.paginator import ListAssetsPaginator

from types_aiobotocore_mediapackage_vod.literals import PaginatorName



session = get_session()

async with session.create_client("mediapackage-vod") as client:
    client: MediaPackageVodClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_assets"
    paginator: ListAssetsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAssetsResponseTypeDef
        print(item)
    

    
```
