<a id="paginators-for-aiobotocore-kinesisvideo-module"></a>

# Paginators for aiobotocore KinesisVideo module

> [Index](..) > [KinesisVideo](.) > Paginators

Auto-generated documentation for
[KinesisVideo](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
type annotations stubs module
[types-aiobotocore-kinesisvideo](https://pypi.org/project/types-aiobotocore-kinesisvideo/).

- [Paginators for aiobotocore KinesisVideo module](#paginators-for-aiobotocore-kinesisvideo-module)
  - [ListSignalingChannelsPaginator](#listsignalingchannelspaginator)
  - [ListStreamsPaginator](#liststreamspaginator)

<a id="listsignalingchannelspaginator"></a>

## ListSignalingChannelsPaginator

Type annotations for
`aiobotocore.create_client("kinesisvideo").get_paginator("list_signaling_channels")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_kinesisvideo.paginator import ListSignalingChannelsPaginator

def get_list_signaling_channels_paginator() -> ListSignalingChannelsPaginator:
    return Session().create_client("kinesisvideo").get_paginator("list_signaling_channels")
```

Boto3 documentation:
[KinesisVideo.Paginator.ListSignalingChannels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListSignalingChannels)

Arguments for `ListSignalingChannelsPaginator.paginate` method:

- `ChannelNameCondition`:
  [ChannelNameConditionTypeDef](./type_defs.md#channelnameconditiontypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSignalingChannelsPaginator.paginate` returns
`_PageIterator`\[[ListSignalingChannelsOutputTypeDef](./type_defs.md#listsignalingchannelsoutputtypedef)\].

<a id="liststreamspaginator"></a>

## ListStreamsPaginator

Type annotations for
`aiobotocore.create_client("kinesisvideo").get_paginator("list_streams")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_kinesisvideo.paginator import ListStreamsPaginator

def get_list_streams_paginator() -> ListStreamsPaginator:
    return Session().create_client("kinesisvideo").get_paginator("list_streams")
```

Boto3 documentation:
[KinesisVideo.Paginator.ListStreams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListStreams)

Arguments for `ListStreamsPaginator.paginate` method:

- `StreamNameCondition`:
  [StreamNameConditionTypeDef](./type_defs.md#streamnameconditiontypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListStreamsPaginator.paginate` returns
`_PageIterator`\[[ListStreamsOutputTypeDef](./type_defs.md#liststreamsoutputtypedef)\].
