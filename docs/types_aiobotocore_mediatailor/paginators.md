<a id="paginators-for-aiobotocore-mediatailor-module"></a>

# Paginators for aiobotocore MediaTailor module

> [Index](../README.md) > [MediaTailor](./README.md) > Paginators

Auto-generated documentation for
[MediaTailor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
type annotations stubs module
[types-aiobotocore-mediatailor](https://pypi.org/project/types-aiobotocore-mediatailor/).

- [Paginators for aiobotocore MediaTailor module](#paginators-for-aiobotocore-mediatailor-module)
  - [GetChannelSchedulePaginator](#getchannelschedulepaginator)
  - [ListAlertsPaginator](#listalertspaginator)
  - [ListChannelsPaginator](#listchannelspaginator)
  - [ListPlaybackConfigurationsPaginator](#listplaybackconfigurationspaginator)
  - [ListPrefetchSchedulesPaginator](#listprefetchschedulespaginator)
  - [ListSourceLocationsPaginator](#listsourcelocationspaginator)
  - [ListVodSourcesPaginator](#listvodsourcespaginator)

<a id="getchannelschedulepaginator"></a>

## GetChannelSchedulePaginator

Type annotations for
`session.create_client("mediatailor").get_paginator("get_channel_schedule")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediatailor.paginator import GetChannelSchedulePaginator

session = get_session()
async with session.create_client("mediatailor") as client:
    client: MediaTailorClient
    paginator: GetChannelSchedulePaginator = client.get_paginator("get_channel_schedule")
```

Boto3 documentation:
[MediaTailor.Paginator.GetChannelSchedule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.GetChannelSchedule)

Arguments for `GetChannelSchedulePaginator.paginate` method:

- `ChannelName`: `str` *(required)*
- `DurationMinutes`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetChannelSchedulePaginator.paginate` returns
`AsyncIterator`\[[GetChannelScheduleResponseTypeDef](./type_defs.md#getchannelscheduleresponsetypedef)\].

<a id="listalertspaginator"></a>

## ListAlertsPaginator

Type annotations for
`session.create_client("mediatailor").get_paginator("list_alerts")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediatailor.paginator import ListAlertsPaginator

session = get_session()
async with session.create_client("mediatailor") as client:
    client: MediaTailorClient
    paginator: ListAlertsPaginator = client.get_paginator("list_alerts")
```

Boto3 documentation:
[MediaTailor.Paginator.ListAlerts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListAlerts)

Arguments for `ListAlertsPaginator.paginate` method:

- `ResourceArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAlertsPaginator.paginate` returns
`AsyncIterator`\[[ListAlertsResponseTypeDef](./type_defs.md#listalertsresponsetypedef)\].

<a id="listchannelspaginator"></a>

## ListChannelsPaginator

Type annotations for
`session.create_client("mediatailor").get_paginator("list_channels")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediatailor.paginator import ListChannelsPaginator

session = get_session()
async with session.create_client("mediatailor") as client:
    client: MediaTailorClient
    paginator: ListChannelsPaginator = client.get_paginator("list_channels")
```

Boto3 documentation:
[MediaTailor.Paginator.ListChannels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListChannels)

Arguments for `ListChannelsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListChannelsPaginator.paginate` returns
`AsyncIterator`\[[ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef)\].

<a id="listplaybackconfigurationspaginator"></a>

## ListPlaybackConfigurationsPaginator

Type annotations for
`session.create_client("mediatailor").get_paginator("list_playback_configurations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediatailor.paginator import ListPlaybackConfigurationsPaginator

session = get_session()
async with session.create_client("mediatailor") as client:
    client: MediaTailorClient
    paginator: ListPlaybackConfigurationsPaginator = client.get_paginator("list_playback_configurations")
```

Boto3 documentation:
[MediaTailor.Paginator.ListPlaybackConfigurations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPlaybackConfigurations)

Arguments for `ListPlaybackConfigurationsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPlaybackConfigurationsPaginator.paginate` returns
`AsyncIterator`\[[ListPlaybackConfigurationsResponseTypeDef](./type_defs.md#listplaybackconfigurationsresponsetypedef)\].

<a id="listprefetchschedulespaginator"></a>

## ListPrefetchSchedulesPaginator

Type annotations for
`session.create_client("mediatailor").get_paginator("list_prefetch_schedules")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediatailor.paginator import ListPrefetchSchedulesPaginator

session = get_session()
async with session.create_client("mediatailor") as client:
    client: MediaTailorClient
    paginator: ListPrefetchSchedulesPaginator = client.get_paginator("list_prefetch_schedules")
```

Boto3 documentation:
[MediaTailor.Paginator.ListPrefetchSchedules](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPrefetchSchedules)

Arguments for `ListPrefetchSchedulesPaginator.paginate` method:

- `PlaybackConfigurationName`: `str` *(required)*
- `StreamId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPrefetchSchedulesPaginator.paginate` returns
`AsyncIterator`\[[ListPrefetchSchedulesResponseTypeDef](./type_defs.md#listprefetchschedulesresponsetypedef)\].

<a id="listsourcelocationspaginator"></a>

## ListSourceLocationsPaginator

Type annotations for
`session.create_client("mediatailor").get_paginator("list_source_locations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediatailor.paginator import ListSourceLocationsPaginator

session = get_session()
async with session.create_client("mediatailor") as client:
    client: MediaTailorClient
    paginator: ListSourceLocationsPaginator = client.get_paginator("list_source_locations")
```

Boto3 documentation:
[MediaTailor.Paginator.ListSourceLocations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListSourceLocations)

Arguments for `ListSourceLocationsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSourceLocationsPaginator.paginate` returns
`AsyncIterator`\[[ListSourceLocationsResponseTypeDef](./type_defs.md#listsourcelocationsresponsetypedef)\].

<a id="listvodsourcespaginator"></a>

## ListVodSourcesPaginator

Type annotations for
`session.create_client("mediatailor").get_paginator("list_vod_sources")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediatailor.paginator import ListVodSourcesPaginator

session = get_session()
async with session.create_client("mediatailor") as client:
    client: MediaTailorClient
    paginator: ListVodSourcesPaginator = client.get_paginator("list_vod_sources")
```

Boto3 documentation:
[MediaTailor.Paginator.ListVodSources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListVodSources)

Arguments for `ListVodSourcesPaginator.paginate` method:

- `SourceLocationName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListVodSourcesPaginator.paginate` returns
`AsyncIterator`\[[ListVodSourcesResponseTypeDef](./type_defs.md#listvodsourcesresponsetypedef)\].
