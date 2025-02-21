# Paginators

> [Index](../README.md) > [CloudWatchRUM](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CloudWatchRUM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#cloudwatchrum)
    type annotations stubs module [types-aiobotocore-rum](https://pypi.org/project/types-aiobotocore-rum/).

## BatchGetRumMetricDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("rum").get_paginator("batch_get_rum_metric_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum/paginator/BatchGetRumMetricDefinitions.html#CloudWatchRUM.Paginator.BatchGetRumMetricDefinitions)

```python
# BatchGetRumMetricDefinitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rum.paginator import BatchGetRumMetricDefinitionsPaginator

session = get_session()
async with session.create_client("rum") as client:  # (1)
    paginator: BatchGetRumMetricDefinitionsPaginator = client.get_paginator("batch_get_rum_metric_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: BatchGetRumMetricDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchRUMClient](./client.md)
2. paginator: [BatchGetRumMetricDefinitionsPaginator](./paginators.md#batchgetrummetricdefinitionspaginator)
3. item: [:material-code-braces: BatchGetRumMetricDefinitionsResponseTypeDef](./type_defs.md#batchgetrummetricdefinitionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python BatchGetRumMetricDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AppMonitorName: str,
    Destination: MetricDestinationType,  # (1)
    DestinationArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[BatchGetRumMetricDefinitionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: MetricDestinationType](./literals.md#metricdestinationtype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: BatchGetRumMetricDefinitionsResponseTypeDef](./type_defs.md#batchgetrummetricdefinitionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: BatchGetRumMetricDefinitionsRequestPaginateTypeDef = {  # (1)
    "AppMonitorName": ...,
    "Destination": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: BatchGetRumMetricDefinitionsRequestPaginateTypeDef](./type_defs.md#batchgetrummetricdefinitionsrequestpaginatetypedef) 
## GetAppMonitorDataPaginator

Type annotations and code completion for `#!python session.create_client("rum").get_paginator("get_app_monitor_data")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum/paginator/GetAppMonitorData.html#CloudWatchRUM.Paginator.GetAppMonitorData)

```python
# GetAppMonitorDataPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rum.paginator import GetAppMonitorDataPaginator

session = get_session()
async with session.create_client("rum") as client:  # (1)
    paginator: GetAppMonitorDataPaginator = client.get_paginator("get_app_monitor_data")  # (2)
    async for item in paginator.paginate(...):
        item: GetAppMonitorDataResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchRUMClient](./client.md)
2. paginator: [GetAppMonitorDataPaginator](./paginators.md#getappmonitordatapaginator)
3. item: [:material-code-braces: GetAppMonitorDataResponseTypeDef](./type_defs.md#getappmonitordataresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetAppMonitorDataPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Name: str,
    TimeRange: TimeRangeTypeDef,  # (1)
    Filters: Sequence[QueryFilterTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[GetAppMonitorDataResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
2. See [:material-code-braces: QueryFilterTypeDef](./type_defs.md#queryfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: GetAppMonitorDataResponseTypeDef](./type_defs.md#getappmonitordataresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetAppMonitorDataRequestPaginateTypeDef = {  # (1)
    "Name": ...,
    "TimeRange": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetAppMonitorDataRequestPaginateTypeDef](./type_defs.md#getappmonitordatarequestpaginatetypedef) 
## ListAppMonitorsPaginator

Type annotations and code completion for `#!python session.create_client("rum").get_paginator("list_app_monitors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum/paginator/ListAppMonitors.html#CloudWatchRUM.Paginator.ListAppMonitors)

```python
# ListAppMonitorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rum.paginator import ListAppMonitorsPaginator

session = get_session()
async with session.create_client("rum") as client:  # (1)
    paginator: ListAppMonitorsPaginator = client.get_paginator("list_app_monitors")  # (2)
    async for item in paginator.paginate(...):
        item: ListAppMonitorsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchRUMClient](./client.md)
2. paginator: [ListAppMonitorsPaginator](./paginators.md#listappmonitorspaginator)
3. item: [:material-code-braces: ListAppMonitorsResponseTypeDef](./type_defs.md#listappmonitorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAppMonitorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAppMonitorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAppMonitorsResponseTypeDef](./type_defs.md#listappmonitorsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAppMonitorsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAppMonitorsRequestPaginateTypeDef](./type_defs.md#listappmonitorsrequestpaginatetypedef) 
## ListRumMetricsDestinationsPaginator

Type annotations and code completion for `#!python session.create_client("rum").get_paginator("list_rum_metrics_destinations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum/paginator/ListRumMetricsDestinations.html#CloudWatchRUM.Paginator.ListRumMetricsDestinations)

```python
# ListRumMetricsDestinationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rum.paginator import ListRumMetricsDestinationsPaginator

session = get_session()
async with session.create_client("rum") as client:  # (1)
    paginator: ListRumMetricsDestinationsPaginator = client.get_paginator("list_rum_metrics_destinations")  # (2)
    async for item in paginator.paginate(...):
        item: ListRumMetricsDestinationsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchRUMClient](./client.md)
2. paginator: [ListRumMetricsDestinationsPaginator](./paginators.md#listrummetricsdestinationspaginator)
3. item: [:material-code-braces: ListRumMetricsDestinationsResponseTypeDef](./type_defs.md#listrummetricsdestinationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRumMetricsDestinationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AppMonitorName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListRumMetricsDestinationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRumMetricsDestinationsResponseTypeDef](./type_defs.md#listrummetricsdestinationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRumMetricsDestinationsRequestPaginateTypeDef = {  # (1)
    "AppMonitorName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRumMetricsDestinationsRequestPaginateTypeDef](./type_defs.md#listrummetricsdestinationsrequestpaginatetypedef) 
