# Paginators

> [Index](../README.md) > [MediaTailor](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MediaTailor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
    type annotations stubs module [types-aiobotocore-mediatailor](https://pypi.org/project/types-aiobotocore-mediatailor/).

## GetChannelSchedulePaginator

Type annotations and code completion for `#!python session.create_client("mediatailor").get_paginator("get_channel_schedule")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.GetChannelSchedule)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mediatailor.paginator import GetChannelSchedulePaginator

session = get_session()
async with session.create_client("mediatailor") as client:
    client: MediaTailorClient
    paginator: GetChannelSchedulePaginator = client.get_paginator("get_channel_schedule")
```


### paginate

Type annotations and code completion for `#!python GetChannelSchedulePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ChannelName: str,
    DurationMinutes: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetChannelScheduleResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetChannelScheduleResponseTypeDef](./type_defs.md#getchannelscheduleresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef = {  # (1)
    "ChannelName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef](./type_defs.md#getchannelschedulerequestgetchannelschedulepaginatetypedef) 
## ListAlertsPaginator

Type annotations and code completion for `#!python session.create_client("mediatailor").get_paginator("list_alerts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListAlerts)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mediatailor.paginator import ListAlertsPaginator

session = get_session()
async with session.create_client("mediatailor") as client:
    client: MediaTailorClient
    paginator: ListAlertsPaginator = client.get_paginator("list_alerts")
```


### paginate

Type annotations and code completion for `#!python ListAlertsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAlertsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAlertsResponseTypeDef](./type_defs.md#listalertsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAlertsRequestListAlertsPaginateTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAlertsRequestListAlertsPaginateTypeDef](./type_defs.md#listalertsrequestlistalertspaginatetypedef) 
## ListChannelsPaginator

Type annotations and code completion for `#!python session.create_client("mediatailor").get_paginator("list_channels")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListChannels)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mediatailor.paginator import ListChannelsPaginator

session = get_session()
async with session.create_client("mediatailor") as client:
    client: MediaTailorClient
    paginator: ListChannelsPaginator = client.get_paginator("list_channels")
```


### paginate

Type annotations and code completion for `#!python ListChannelsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListChannelsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListChannelsRequestListChannelsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListChannelsRequestListChannelsPaginateTypeDef](./type_defs.md#listchannelsrequestlistchannelspaginatetypedef) 
## ListPlaybackConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("mediatailor").get_paginator("list_playback_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPlaybackConfigurations)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mediatailor.paginator import ListPlaybackConfigurationsPaginator

session = get_session()
async with session.create_client("mediatailor") as client:
    client: MediaTailorClient
    paginator: ListPlaybackConfigurationsPaginator = client.get_paginator("list_playback_configurations")
```


### paginate

Type annotations and code completion for `#!python ListPlaybackConfigurationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPlaybackConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPlaybackConfigurationsResponseTypeDef](./type_defs.md#listplaybackconfigurationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef](./type_defs.md#listplaybackconfigurationsrequestlistplaybackconfigurationspaginatetypedef) 
## ListPrefetchSchedulesPaginator

Type annotations and code completion for `#!python session.create_client("mediatailor").get_paginator("list_prefetch_schedules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPrefetchSchedules)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mediatailor.paginator import ListPrefetchSchedulesPaginator

session = get_session()
async with session.create_client("mediatailor") as client:
    client: MediaTailorClient
    paginator: ListPrefetchSchedulesPaginator = client.get_paginator("list_prefetch_schedules")
```


### paginate

Type annotations and code completion for `#!python ListPrefetchSchedulesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PlaybackConfigurationName: str,
    StreamId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPrefetchSchedulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPrefetchSchedulesResponseTypeDef](./type_defs.md#listprefetchschedulesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef = {  # (1)
    "PlaybackConfigurationName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef](./type_defs.md#listprefetchschedulesrequestlistprefetchschedulespaginatetypedef) 
## ListSourceLocationsPaginator

Type annotations and code completion for `#!python session.create_client("mediatailor").get_paginator("list_source_locations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListSourceLocations)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mediatailor.paginator import ListSourceLocationsPaginator

session = get_session()
async with session.create_client("mediatailor") as client:
    client: MediaTailorClient
    paginator: ListSourceLocationsPaginator = client.get_paginator("list_source_locations")
```


### paginate

Type annotations and code completion for `#!python ListSourceLocationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSourceLocationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSourceLocationsResponseTypeDef](./type_defs.md#listsourcelocationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSourceLocationsRequestListSourceLocationsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSourceLocationsRequestListSourceLocationsPaginateTypeDef](./type_defs.md#listsourcelocationsrequestlistsourcelocationspaginatetypedef) 
## ListVodSourcesPaginator

Type annotations and code completion for `#!python session.create_client("mediatailor").get_paginator("list_vod_sources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListVodSources)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mediatailor.paginator import ListVodSourcesPaginator

session = get_session()
async with session.create_client("mediatailor") as client:
    client: MediaTailorClient
    paginator: ListVodSourcesPaginator = client.get_paginator("list_vod_sources")
```


### paginate

Type annotations and code completion for `#!python ListVodSourcesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    SourceLocationName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListVodSourcesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListVodSourcesResponseTypeDef](./type_defs.md#listvodsourcesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListVodSourcesRequestListVodSourcesPaginateTypeDef = {  # (1)
    "SourceLocationName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVodSourcesRequestListVodSourcesPaginateTypeDef](./type_defs.md#listvodsourcesrequestlistvodsourcespaginatetypedef) 
