<a id="paginators-for-aiobotocore-kinesisvideoarchivedmedia-module"></a>

# Paginators for aiobotocore KinesisVideoArchivedMedia module

> [Index](../README.md) > [KinesisVideoArchivedMedia](./README.md) > Paginators

Auto-generated documentation for
[KinesisVideoArchivedMedia](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
type annotations stubs module
[types-aiobotocore-kinesis-video-archived-media](https://pypi.org/project/types-aiobotocore-kinesis-video-archived-media/).

- [Paginators for aiobotocore KinesisVideoArchivedMedia module](#paginators-for-aiobotocore-kinesisvideoarchivedmedia-module)
  - [ListFragmentsPaginator](#listfragmentspaginator)

<a id="listfragmentspaginator"></a>

## ListFragmentsPaginator

Type annotations for
`session.create_client("kinesis-video-archived-media").get_paginator("list_fragments")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_kinesis_video_archived_media.paginator import ListFragmentsPaginator

session = get_session()
async with session.create_client("kinesis-video-archived-media") as client:
    client: KinesisVideoArchivedMediaClient
    paginator: ListFragmentsPaginator = client.get_paginator("list_fragments")
```

Boto3 documentation:
[KinesisVideoArchivedMedia.Paginator.ListFragments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.ListFragments)

Arguments for `ListFragmentsPaginator.paginate` method:

- `StreamName`: `str`
- `StreamARN`: `str`
- `FragmentSelector`:
  [FragmentSelectorTypeDef](./type_defs.md#fragmentselectortypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFragmentsPaginator.paginate` returns
`AsyncIterator`\[[ListFragmentsOutputTypeDef](./type_defs.md#listfragmentsoutputtypedef)\].