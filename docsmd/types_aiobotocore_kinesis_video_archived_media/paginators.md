# Paginators

> [Index](../README.md) > [KinesisVideoArchivedMedia](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [KinesisVideoArchivedMedia](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#kinesisvideoarchivedmedia)
    type annotations stubs module [types-aiobotocore-kinesis-video-archived-media](https://pypi.org/project/types-aiobotocore-kinesis-video-archived-media/).

## GetImagesPaginator

Type annotations and code completion for `#!python session.create_client("kinesis-video-archived-media").get_paginator("get_images")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media/paginator/GetImages.html#KinesisVideoArchivedMedia.Paginator.GetImages)

```python
# GetImagesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kinesis_video_archived_media.paginator import GetImagesPaginator

session = get_session()
async with session.create_client("kinesis-video-archived-media") as client:  # (1)
    paginator: GetImagesPaginator = client.get_paginator("get_images")  # (2)
    async for item in paginator.paginate(...):
        item: GetImagesOutputTypeDef
        print(item)  # (3)
```

1. client: [KinesisVideoArchivedMediaClient](./client.md)
2. paginator: [GetImagesPaginator](./paginators.md#getimagespaginator)
3. item: [:material-code-braces: GetImagesOutputTypeDef](./type_defs.md#getimagesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python GetImagesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ImageSelectorType: ImageSelectorTypeType,  # (1)
    StartTimestamp: TimestampTypeDef,
    EndTimestamp: TimestampTypeDef,
    Format: FormatType,  # (2)
    StreamName: str = ...,
    StreamARN: str = ...,
    SamplingInterval: int = ...,
    FormatConfig: Mapping[FormatConfigKeyType, str] = ...,  # (3)
    WidthPixels: int = ...,
    HeightPixels: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[GetImagesOutputTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: ImageSelectorTypeType](./literals.md#imageselectortypetype) 
2. See [:material-code-brackets: FormatType](./literals.md#formattype) 
3. See [:material-code-brackets: FormatConfigKeyType](./literals.md#formatconfigkeytype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: GetImagesOutputTypeDef](./type_defs.md#getimagesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetImagesInputPaginateTypeDef = {  # (1)
    "ImageSelectorType": ...,
    "StartTimestamp": ...,
    "EndTimestamp": ...,
    "Format": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetImagesInputPaginateTypeDef](./type_defs.md#getimagesinputpaginatetypedef) 
## ListFragmentsPaginator

Type annotations and code completion for `#!python session.create_client("kinesis-video-archived-media").get_paginator("list_fragments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media/paginator/ListFragments.html#KinesisVideoArchivedMedia.Paginator.ListFragments)

```python
# ListFragmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kinesis_video_archived_media.paginator import ListFragmentsPaginator

session = get_session()
async with session.create_client("kinesis-video-archived-media") as client:  # (1)
    paginator: ListFragmentsPaginator = client.get_paginator("list_fragments")  # (2)
    async for item in paginator.paginate(...):
        item: ListFragmentsOutputTypeDef
        print(item)  # (3)
```

1. client: [KinesisVideoArchivedMediaClient](./client.md)
2. paginator: [ListFragmentsPaginator](./paginators.md#listfragmentspaginator)
3. item: [:material-code-braces: ListFragmentsOutputTypeDef](./type_defs.md#listfragmentsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListFragmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StreamName: str = ...,
    StreamARN: str = ...,
    FragmentSelector: FragmentSelectorTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListFragmentsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FragmentSelectorTypeDef](./type_defs.md#fragmentselectortypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListFragmentsOutputTypeDef](./type_defs.md#listfragmentsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFragmentsInputPaginateTypeDef = {  # (1)
    "StreamName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFragmentsInputPaginateTypeDef](./type_defs.md#listfragmentsinputpaginatetypedef) 
