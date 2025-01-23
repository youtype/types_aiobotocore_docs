# Paginators

> [Index](../README.md) > [CloudWatchInternetMonitor](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CloudWatchInternetMonitor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#cloudwatchinternetmonitor)
    type annotations stubs module [types-aiobotocore-internetmonitor](https://pypi.org/project/types-aiobotocore-internetmonitor/).

## ListHealthEventsPaginator

Type annotations and code completion for `#!python session.create_client("internetmonitor").get_paginator("list_health_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor/paginator/ListHealthEvents.html#CloudWatchInternetMonitor.Paginator.ListHealthEvents)

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
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    EventStatus: HealthEventStatusType = ...,  # (1)
    LinkedAccountId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListHealthEventsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: HealthEventStatusType](./literals.md#healtheventstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListHealthEventsOutputTypeDef](./type_defs.md#listhealtheventsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListHealthEventsInputPaginateTypeDef = {  # (1)
    "MonitorName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHealthEventsInputPaginateTypeDef](./type_defs.md#listhealtheventsinputpaginatetypedef) 
## ListInternetEventsPaginator

Type annotations and code completion for `#!python session.create_client("internetmonitor").get_paginator("list_internet_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor/paginator/ListInternetEvents.html#CloudWatchInternetMonitor.Paginator.ListInternetEvents)

```python
# ListInternetEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_internetmonitor.paginator import ListInternetEventsPaginator

session = get_session()
async with session.create_client("internetmonitor") as client:  # (1)
    paginator: ListInternetEventsPaginator = client.get_paginator("list_internet_events")  # (2)
    async for item in paginator.paginate(...):
        item: ListInternetEventsOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchInternetMonitorClient](./client.md)
2. paginator: [ListInternetEventsPaginator](./paginators.md#listinterneteventspaginator)
3. item: [:material-code-braces: ListInternetEventsOutputTypeDef](./type_defs.md#listinterneteventsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListInternetEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    EventStatus: str = ...,
    EventType: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListInternetEventsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInternetEventsOutputTypeDef](./type_defs.md#listinterneteventsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListInternetEventsInputPaginateTypeDef = {  # (1)
    "StartTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInternetEventsInputPaginateTypeDef](./type_defs.md#listinterneteventsinputpaginatetypedef) 
## ListMonitorsPaginator

Type annotations and code completion for `#!python session.create_client("internetmonitor").get_paginator("list_monitors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor/paginator/ListMonitors.html#CloudWatchInternetMonitor.Paginator.ListMonitors)

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
    IncludeLinkedAccounts: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListMonitorsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMonitorsOutputTypeDef](./type_defs.md#listmonitorsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMonitorsInputPaginateTypeDef = {  # (1)
    "MonitorStatus": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMonitorsInputPaginateTypeDef](./type_defs.md#listmonitorsinputpaginatetypedef) 
