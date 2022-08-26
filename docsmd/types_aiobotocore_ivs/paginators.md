# Paginators

> [Index](../README.md) > [IVS](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IVS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
    type annotations stubs module [types-aiobotocore-ivs](https://pypi.org/project/types-aiobotocore-ivs/).

## ListChannelsPaginator

Type annotations and code completion for `#!python session.create_client("ivs").get_paginator("list_channels")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListChannels)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ivs.paginator import ListChannelsPaginator

session = get_session()
async with session.create_client("ivs") as client:  # (1)
    paginator: ListChannelsPaginator = client.get_paginator("list_channels")  # (2)
    async for item in paginator.paginate(...):
        item: ListChannelsResponseTypeDef
        print(item)  # (3)
```

1. client: [IVSClient](./client.md)
2. paginator: [ListChannelsPaginator](./paginators.md#listchannelspaginator)
3. item: [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListChannelsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filterByName: str = ...,
    filterByRecordingConfigurationArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListChannelsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListChannelsRequestListChannelsPaginateTypeDef = {  # (1)
    "filterByName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListChannelsRequestListChannelsPaginateTypeDef](./type_defs.md#listchannelsrequestlistchannelspaginatetypedef) 
## ListPlaybackKeyPairsPaginator

Type annotations and code completion for `#!python session.create_client("ivs").get_paginator("list_playback_key_pairs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListPlaybackKeyPairs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ivs.paginator import ListPlaybackKeyPairsPaginator

session = get_session()
async with session.create_client("ivs") as client:  # (1)
    paginator: ListPlaybackKeyPairsPaginator = client.get_paginator("list_playback_key_pairs")  # (2)
    async for item in paginator.paginate(...):
        item: ListPlaybackKeyPairsResponseTypeDef
        print(item)  # (3)
```

1. client: [IVSClient](./client.md)
2. paginator: [ListPlaybackKeyPairsPaginator](./paginators.md#listplaybackkeypairspaginator)
3. item: [:material-code-braces: ListPlaybackKeyPairsResponseTypeDef](./type_defs.md#listplaybackkeypairsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPlaybackKeyPairsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPlaybackKeyPairsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPlaybackKeyPairsResponseTypeDef](./type_defs.md#listplaybackkeypairsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef](./type_defs.md#listplaybackkeypairsrequestlistplaybackkeypairspaginatetypedef) 
## ListRecordingConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("ivs").get_paginator("list_recording_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListRecordingConfigurations)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ivs.paginator import ListRecordingConfigurationsPaginator

session = get_session()
async with session.create_client("ivs") as client:  # (1)
    paginator: ListRecordingConfigurationsPaginator = client.get_paginator("list_recording_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecordingConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [IVSClient](./client.md)
2. paginator: [ListRecordingConfigurationsPaginator](./paginators.md#listrecordingconfigurationspaginator)
3. item: [:material-code-braces: ListRecordingConfigurationsResponseTypeDef](./type_defs.md#listrecordingconfigurationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRecordingConfigurationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRecordingConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRecordingConfigurationsResponseTypeDef](./type_defs.md#listrecordingconfigurationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef](./type_defs.md#listrecordingconfigurationsrequestlistrecordingconfigurationspaginatetypedef) 
## ListStreamKeysPaginator

Type annotations and code completion for `#!python session.create_client("ivs").get_paginator("list_stream_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreamKeys)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ivs.paginator import ListStreamKeysPaginator

session = get_session()
async with session.create_client("ivs") as client:  # (1)
    paginator: ListStreamKeysPaginator = client.get_paginator("list_stream_keys")  # (2)
    async for item in paginator.paginate(...):
        item: ListStreamKeysResponseTypeDef
        print(item)  # (3)
```

1. client: [IVSClient](./client.md)
2. paginator: [ListStreamKeysPaginator](./paginators.md#liststreamkeyspaginator)
3. item: [:material-code-braces: ListStreamKeysResponseTypeDef](./type_defs.md#liststreamkeysresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListStreamKeysPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    channelArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListStreamKeysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListStreamKeysResponseTypeDef](./type_defs.md#liststreamkeysresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListStreamKeysRequestListStreamKeysPaginateTypeDef = {  # (1)
    "channelArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStreamKeysRequestListStreamKeysPaginateTypeDef](./type_defs.md#liststreamkeysrequestliststreamkeyspaginatetypedef) 
## ListStreamsPaginator

Type annotations and code completion for `#!python session.create_client("ivs").get_paginator("list_streams")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreams)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ivs.paginator import ListStreamsPaginator

session = get_session()
async with session.create_client("ivs") as client:  # (1)
    paginator: ListStreamsPaginator = client.get_paginator("list_streams")  # (2)
    async for item in paginator.paginate(...):
        item: ListStreamsResponseTypeDef
        print(item)  # (3)
```

1. client: [IVSClient](./client.md)
2. paginator: [ListStreamsPaginator](./paginators.md#liststreamspaginator)
3. item: [:material-code-braces: ListStreamsResponseTypeDef](./type_defs.md#liststreamsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListStreamsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filterBy: StreamFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListStreamsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: StreamFiltersTypeDef](./type_defs.md#streamfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListStreamsResponseTypeDef](./type_defs.md#liststreamsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListStreamsRequestListStreamsPaginateTypeDef = {  # (1)
    "filterBy": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStreamsRequestListStreamsPaginateTypeDef](./type_defs.md#liststreamsrequestliststreamspaginatetypedef) 
