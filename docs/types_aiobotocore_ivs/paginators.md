<a id="paginators-for-aiobotocore-ivs-module"></a>

# Paginators for aiobotocore IVS module

> [Index](../README.md) > [IVS](./README.md) > Paginators

Auto-generated documentation for
[IVS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
type annotations stubs module
[types-aiobotocore-ivs](https://pypi.org/project/types-aiobotocore-ivs/).

- [Paginators for aiobotocore IVS module](#paginators-for-aiobotocore-ivs-module)
  - [ListChannelsPaginator](#listchannelspaginator)
  - [ListPlaybackKeyPairsPaginator](#listplaybackkeypairspaginator)
  - [ListRecordingConfigurationsPaginator](#listrecordingconfigurationspaginator)
  - [ListStreamKeysPaginator](#liststreamkeyspaginator)
  - [ListStreamsPaginator](#liststreamspaginator)

<a id="listchannelspaginator"></a>

## ListChannelsPaginator

Type annotations for
`session.create_client("ivs").get_paginator("list_channels")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ivs.paginator import ListChannelsPaginator

session = get_session()
async with session.create_client("ivs") as client:
    client: IVSClient
    paginator: ListChannelsPaginator = client.get_paginator("list_channels")
```

Boto3 documentation:
[IVS.Paginator.ListChannels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListChannels)

Arguments for `ListChannelsPaginator.paginate` method:

- `filterByName`: `str`
- `filterByRecordingConfigurationArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListChannelsPaginator.paginate` returns
`AsyncIterator`\[[ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef)\].

<a id="listplaybackkeypairspaginator"></a>

## ListPlaybackKeyPairsPaginator

Type annotations for
`session.create_client("ivs").get_paginator("list_playback_key_pairs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ivs.paginator import ListPlaybackKeyPairsPaginator

session = get_session()
async with session.create_client("ivs") as client:
    client: IVSClient
    paginator: ListPlaybackKeyPairsPaginator = client.get_paginator("list_playback_key_pairs")
```

Boto3 documentation:
[IVS.Paginator.ListPlaybackKeyPairs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListPlaybackKeyPairs)

Arguments for `ListPlaybackKeyPairsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPlaybackKeyPairsPaginator.paginate` returns
`AsyncIterator`\[[ListPlaybackKeyPairsResponseTypeDef](./type_defs.md#listplaybackkeypairsresponsetypedef)\].

<a id="listrecordingconfigurationspaginator"></a>

## ListRecordingConfigurationsPaginator

Type annotations for
`session.create_client("ivs").get_paginator("list_recording_configurations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ivs.paginator import ListRecordingConfigurationsPaginator

session = get_session()
async with session.create_client("ivs") as client:
    client: IVSClient
    paginator: ListRecordingConfigurationsPaginator = client.get_paginator("list_recording_configurations")
```

Boto3 documentation:
[IVS.Paginator.ListRecordingConfigurations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListRecordingConfigurations)

Arguments for `ListRecordingConfigurationsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRecordingConfigurationsPaginator.paginate` returns
`AsyncIterator`\[[ListRecordingConfigurationsResponseTypeDef](./type_defs.md#listrecordingconfigurationsresponsetypedef)\].

<a id="liststreamkeyspaginator"></a>

## ListStreamKeysPaginator

Type annotations for
`session.create_client("ivs").get_paginator("list_stream_keys")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ivs.paginator import ListStreamKeysPaginator

session = get_session()
async with session.create_client("ivs") as client:
    client: IVSClient
    paginator: ListStreamKeysPaginator = client.get_paginator("list_stream_keys")
```

Boto3 documentation:
[IVS.Paginator.ListStreamKeys](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreamKeys)

Arguments for `ListStreamKeysPaginator.paginate` method:

- `channelArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListStreamKeysPaginator.paginate` returns
`AsyncIterator`\[[ListStreamKeysResponseTypeDef](./type_defs.md#liststreamkeysresponsetypedef)\].

<a id="liststreamspaginator"></a>

## ListStreamsPaginator

Type annotations for
`session.create_client("ivs").get_paginator("list_streams")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ivs.paginator import ListStreamsPaginator

session = get_session()
async with session.create_client("ivs") as client:
    client: IVSClient
    paginator: ListStreamsPaginator = client.get_paginator("list_streams")
```

Boto3 documentation:
[IVS.Paginator.ListStreams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreams)

Arguments for `ListStreamsPaginator.paginate` method:

- `filterBy`: [StreamFiltersTypeDef](./type_defs.md#streamfilterstypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListStreamsPaginator.paginate` returns
`AsyncIterator`\[[ListStreamsResponseTypeDef](./type_defs.md#liststreamsresponsetypedef)\].