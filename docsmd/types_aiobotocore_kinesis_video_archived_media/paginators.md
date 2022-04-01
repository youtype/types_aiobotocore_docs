# Paginators

> [Index](../README.md) > [KinesisVideoArchivedMedia](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [KinesisVideoArchivedMedia](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
    type annotations stubs module [types-aiobotocore-kinesis-video-archived-media](https://pypi.org/project/types-aiobotocore-kinesis-video-archived-media/).

## ListFragmentsPaginator

Type annotations and code completion for `#!python session.create_client("kinesis-video-archived-media").get_paginator("list_fragments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.ListFragments)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_kinesis_video_archived_media.paginator import ListFragmentsPaginator

session = get_session()
async with session.create_client("kinesis-video-archived-media") as client:
    client: KinesisVideoArchivedMediaClient
    paginator: ListFragmentsPaginator = client.get_paginator("list_fragments")
```


### paginate

Type annotations and code completion for `#!python ListFragmentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    StreamName: str = ...,
    StreamARN: str = ...,
    FragmentSelector: FragmentSelectorTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListFragmentsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FragmentSelectorTypeDef](./type_defs.md#fragmentselectortypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListFragmentsOutputTypeDef](./type_defs.md#listfragmentsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListFragmentsInputListFragmentsPaginateTypeDef = {  # (1)
    "StreamName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFragmentsInputListFragmentsPaginateTypeDef](./type_defs.md#listfragmentsinputlistfragmentspaginatetypedef) 
