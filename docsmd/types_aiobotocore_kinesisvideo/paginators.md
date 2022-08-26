# Paginators

> [Index](../README.md) > [KinesisVideo](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [KinesisVideo](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
    type annotations stubs module [types-aiobotocore-kinesisvideo](https://pypi.org/project/types-aiobotocore-kinesisvideo/).

## ListSignalingChannelsPaginator

Type annotations and code completion for `#!python session.create_client("kinesisvideo").get_paginator("list_signaling_channels")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListSignalingChannels)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_kinesisvideo.paginator import ListSignalingChannelsPaginator

session = get_session()
async with session.create_client("kinesisvideo") as client:  # (1)
    paginator: ListSignalingChannelsPaginator = client.get_paginator("list_signaling_channels")  # (2)
    async for item in paginator.paginate(...):
        item: ListSignalingChannelsOutputTypeDef
        print(item)  # (3)
```

1. client: [KinesisVideoClient](./client.md)
2. paginator: [ListSignalingChannelsPaginator](./paginators.md#listsignalingchannelspaginator)
3. item: [:material-code-braces: ListSignalingChannelsOutputTypeDef](./type_defs.md#listsignalingchannelsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSignalingChannelsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ChannelNameCondition: ChannelNameConditionTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListSignalingChannelsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ChannelNameConditionTypeDef](./type_defs.md#channelnameconditiontypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSignalingChannelsOutputTypeDef](./type_defs.md#listsignalingchannelsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = {  # (1)
    "ChannelNameCondition": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef](./type_defs.md#listsignalingchannelsinputlistsignalingchannelspaginatetypedef) 
## ListStreamsPaginator

Type annotations and code completion for `#!python session.create_client("kinesisvideo").get_paginator("list_streams")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListStreams)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_kinesisvideo.paginator import ListStreamsPaginator

session = get_session()
async with session.create_client("kinesisvideo") as client:  # (1)
    paginator: ListStreamsPaginator = client.get_paginator("list_streams")  # (2)
    async for item in paginator.paginate(...):
        item: ListStreamsOutputTypeDef
        print(item)  # (3)
```

1. client: [KinesisVideoClient](./client.md)
2. paginator: [ListStreamsPaginator](./paginators.md#liststreamspaginator)
3. item: [:material-code-braces: ListStreamsOutputTypeDef](./type_defs.md#liststreamsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListStreamsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    StreamNameCondition: StreamNameConditionTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListStreamsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: StreamNameConditionTypeDef](./type_defs.md#streamnameconditiontypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListStreamsOutputTypeDef](./type_defs.md#liststreamsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListStreamsInputListStreamsPaginateTypeDef = {  # (1)
    "StreamNameCondition": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStreamsInputListStreamsPaginateTypeDef](./type_defs.md#liststreamsinputliststreamspaginatetypedef) 
