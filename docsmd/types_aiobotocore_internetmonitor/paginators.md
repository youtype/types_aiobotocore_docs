# Paginators

> [Index](../README.md) > [CloudWatchInternetMonitor](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CloudWatchInternetMonitor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
    type annotations stubs module [types-aiobotocore-internetmonitor](https://pypi.org/project/types-aiobotocore-internetmonitor/).

## ListHealthEventsPaginator

Type annotations and code completion for `#!python session.create_client("internetmonitor").get_paginator("list_health_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Paginator.ListHealthEvents)

```python
# ListHealthEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_internetmonitor.paginator import ListHealthEventsPaginator

session = get_session()
async with session.create_client("internetmonitor") as client:  # (1)
    paginator: ListHealthEventsPaginator = client.get_paginator("list_health_events")  # (2)
    async for item in paginator.paginate(...):
        item: ListHealthEventsOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchInternetMonitorClient](./client.md)
2. paginator: [ListHealthEventsPaginator](./paginators.md#listhealtheventspaginator)
3. item: [:material-code-braces: ListHealthEventsOutputTypeDef](./type_defs.md#listhealtheventsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListHealthEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    MonitorName: str,
    StartTime: Union[datetime, str] = ...,
    EndTime: Union[datetime, str] = ...,
    EventStatus: HealthEventStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListHealthEventsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: HealthEventStatusType](./literals.md#healtheventstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListHealthEventsOutputTypeDef](./type_defs.md#listhealtheventsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListHealthEventsInputListHealthEventsPaginateTypeDef = {  # (1)
    "MonitorName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHealthEventsInputListHealthEventsPaginateTypeDef](./type_defs.md#listhealtheventsinputlisthealtheventspaginatetypedef) 
## ListMonitorsPaginator

Type annotations and code completion for `#!python session.create_client("internetmonitor").get_paginator("list_monitors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Paginator.ListMonitors)

```python
# ListMonitorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_internetmonitor.paginator import ListMonitorsPaginator

session = get_session()
async with session.create_client("internetmonitor") as client:  # (1)
    paginator: ListMonitorsPaginator = client.get_paginator("list_monitors")  # (2)
    async for item in paginator.paginate(...):
        item: ListMonitorsOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchInternetMonitorClient](./client.md)
2. paginator: [ListMonitorsPaginator](./paginators.md#listmonitorspaginator)
3. item: [:material-code-braces: ListMonitorsOutputTypeDef](./type_defs.md#listmonitorsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListMonitorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    MonitorStatus: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMonitorsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMonitorsOutputTypeDef](./type_defs.md#listmonitorsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMonitorsInputListMonitorsPaginateTypeDef = {  # (1)
    "MonitorStatus": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMonitorsInputListMonitorsPaginateTypeDef](./type_defs.md#listmonitorsinputlistmonitorspaginatetypedef) 
