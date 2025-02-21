# Examples

> [Index](../README.md) > [MediaPackageVod](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MediaPackageVod](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#mediapackagevod)
    type annotations stubs module [types-aiobotocore-mediapackage-vod](https://pypi.org/project/types-aiobotocore-mediapackage-vod/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[mediapackage-vod]` package installed.

Write your `MediaPackageVod` code as usual,
type checking and code completion should work out of the box.



```python
# MediaPackageVodClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("mediapackage-vod") as client:  # (1)
    result = await client.configure_logs()  # (2)
```

1. client: [MediaPackageVodClient](./client.md)
2. result: [:material-code-braces: ConfigureLogsResponseTypeDef](./type_defs.md#configurelogsresponsetypedef) 



```python
# ListAssetsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("mediapackage-vod") as client:  # (1)
    paginator = client.get_paginator("list_assets")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MediaPackageVodClient](./client.md)
2. paginator: [ListAssetsPaginator](./paginators.md#listassetspaginator)
3. item: [:material-code-braces: ListAssetsResponseTypeDef](./type_defs.md#listassetsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[mediapackage-vod]`
or a standalone `types_aiobotocore_mediapackage_vod` package, you have to explicitly specify
`client: MediaPackageVodClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# MediaPackageVodClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_mediapackage_vod.client import MediaPackageVodClient
from types_aiobotocore_mediapackage_vod.type_defs import ConfigureLogsResponseTypeDef
from types_aiobotocore_mediapackage_vod.type_defs import ConfigureLogsRequestTypeDef


session = get_session()

async with session.create_client("mediapackage-vod") as client:
    client: MediaPackageVodClient
    kwargs: ConfigureLogsRequestTypeDef = {...}
    result: ConfigureLogsResponseTypeDef = await client.configure_logs(**kwargs)
```



```python
# ListAssetsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_mediapackage_vod.client import MediaPackageVodClient
from types_aiobotocore_mediapackage_vod.paginator import ListAssetsPaginator
from types_aiobotocore_mediapackage_vod.type_defs import ListAssetsResponseTypeDef


session = get_session()

async with session.create_client("mediapackage-vod") as client:
    client: MediaPackageVodClient
    paginator: ListAssetsPaginator = client.get_paginator("list_assets")
    async for item in paginator.paginate(...):
        item: ListAssetsResponseTypeDef
        print(item)
```


