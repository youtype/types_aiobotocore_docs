# Examples

> [Index](../README.md) > [KinesisVideoArchivedMedia](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [KinesisVideoArchivedMedia](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#kinesisvideoarchivedmedia)
    type annotations stubs module [types-aiobotocore-kinesis-video-archived-media](https://pypi.org/project/types-aiobotocore-kinesis-video-archived-media/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[kinesis-video-archived-media]` package installed.

Write your `KinesisVideoArchivedMedia` code as usual,
type checking and code completion should work out of the box.



```python
# KinesisVideoArchivedMediaClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("kinesis-video-archived-media") as client:  # (1)
    result = await client.get_clip()  # (2)
```

1. client: [KinesisVideoArchivedMediaClient](./client.md)
2. result: [:material-code-braces: GetClipOutputTypeDef](./type_defs.md#getclipoutputtypedef) 



```python
# GetImagesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("kinesis-video-archived-media") as client:  # (1)
    paginator = client.get_paginator("get_images")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [KinesisVideoArchivedMediaClient](./client.md)
2. paginator: [GetImagesPaginator](./paginators.md#getimagespaginator)
3. item: [:material-code-braces: GetImagesOutputTypeDef](./type_defs.md#getimagesoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[kinesis-video-archived-media]`
or a standalone `types_aiobotocore_kinesis_video_archived_media` package, you have to explicitly specify
`client: KinesisVideoArchivedMediaClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# KinesisVideoArchivedMediaClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_kinesis_video_archived_media.client import KinesisVideoArchivedMediaClient
from types_aiobotocore_kinesis_video_archived_media.type_defs import GetClipOutputTypeDef
from types_aiobotocore_kinesis_video_archived_media.type_defs import GetClipInputTypeDef


session = get_session()

async with session.create_client("kinesis-video-archived-media") as client:
    client: KinesisVideoArchivedMediaClient
    kwargs: GetClipInputTypeDef = {...}
    result: GetClipOutputTypeDef = await client.get_clip(**kwargs)
```



```python
# GetImagesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_kinesis_video_archived_media.client import KinesisVideoArchivedMediaClient
from types_aiobotocore_kinesis_video_archived_media.paginator import GetImagesPaginator
from types_aiobotocore_kinesis_video_archived_media.type_defs import GetImagesOutputTypeDef


session = get_session()

async with session.create_client("kinesis-video-archived-media") as client:
    client: KinesisVideoArchivedMediaClient
    paginator: GetImagesPaginator = client.get_paginator("get_images")
    async for item in paginator.paginate(...):
        item: GetImagesOutputTypeDef
        print(item)
```


