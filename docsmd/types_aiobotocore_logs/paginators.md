# Paginators

> [Index](../README.md) > [CloudWatchLogs](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CloudWatchLogs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
    type annotations stubs module [types-aiobotocore-logs](https://pypi.org/project/types-aiobotocore-logs/).

## DescribeDestinationsPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("describe_destinations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeDestinations)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeDestinationsPaginator

session = get_session()
async with session.create_client("logs") as client:
    client: CloudWatchLogsClient
    paginator: DescribeDestinationsPaginator = client.get_paginator("describe_destinations")
```


### paginate

Type annotations and code completion for `#!python DescribeDestinationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DestinationNamePrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeDestinationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeDestinationsResponseTypeDef](./type_defs.md#describedestinationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef = {  # (1)
    "DestinationNamePrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef](./type_defs.md#describedestinationsrequestdescribedestinationspaginatetypedef) 
## DescribeExportTasksPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("describe_export_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeExportTasks)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeExportTasksPaginator

session = get_session()
async with session.create_client("logs") as client:
    client: CloudWatchLogsClient
    paginator: DescribeExportTasksPaginator = client.get_paginator("describe_export_tasks")
```


### paginate

Type annotations and code completion for `#!python DescribeExportTasksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    taskId: str = ...,
    statusCode: ExportTaskStatusCodeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeExportTasksResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ExportTaskStatusCodeType](./literals.md#exporttaskstatuscodetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeExportTasksResponseTypeDef](./type_defs.md#describeexporttasksresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef = {  # (1)
    "taskId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef](./type_defs.md#describeexporttasksrequestdescribeexporttaskspaginatetypedef) 
## DescribeLogGroupsPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("describe_log_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogGroups)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeLogGroupsPaginator

session = get_session()
async with session.create_client("logs") as client:
    client: CloudWatchLogsClient
    paginator: DescribeLogGroupsPaginator = client.get_paginator("describe_log_groups")
```


### paginate

Type annotations and code completion for `#!python DescribeLogGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    logGroupNamePrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeLogGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeLogGroupsResponseTypeDef](./type_defs.md#describeloggroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef = {  # (1)
    "logGroupNamePrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef](./type_defs.md#describeloggroupsrequestdescribeloggroupspaginatetypedef) 
## DescribeLogStreamsPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("describe_log_streams")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogStreams)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeLogStreamsPaginator

session = get_session()
async with session.create_client("logs") as client:
    client: CloudWatchLogsClient
    paginator: DescribeLogStreamsPaginator = client.get_paginator("describe_log_streams")
```


### paginate

Type annotations and code completion for `#!python DescribeLogStreamsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    logGroupName: str,
    logStreamNamePrefix: str = ...,
    orderBy: OrderByType = ...,  # (1)
    descending: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeLogStreamsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: OrderByType](./literals.md#orderbytype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeLogStreamsResponseTypeDef](./type_defs.md#describelogstreamsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef = {  # (1)
    "logGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef](./type_defs.md#describelogstreamsrequestdescribelogstreamspaginatetypedef) 
## DescribeMetricFiltersPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("describe_metric_filters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeMetricFilters)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeMetricFiltersPaginator

session = get_session()
async with session.create_client("logs") as client:
    client: CloudWatchLogsClient
    paginator: DescribeMetricFiltersPaginator = client.get_paginator("describe_metric_filters")
```


### paginate

Type annotations and code completion for `#!python DescribeMetricFiltersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    logGroupName: str = ...,
    filterNamePrefix: str = ...,
    metricName: str = ...,
    metricNamespace: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeMetricFiltersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeMetricFiltersResponseTypeDef](./type_defs.md#describemetricfiltersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef = {  # (1)
    "logGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef](./type_defs.md#describemetricfiltersrequestdescribemetricfilterspaginatetypedef) 
## DescribeQueriesPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("describe_queries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeQueries)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeQueriesPaginator

session = get_session()
async with session.create_client("logs") as client:
    client: CloudWatchLogsClient
    paginator: DescribeQueriesPaginator = client.get_paginator("describe_queries")
```


### paginate

Type annotations and code completion for `#!python DescribeQueriesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    logGroupName: str = ...,
    status: QueryStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeQueriesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: QueryStatusType](./literals.md#querystatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeQueriesResponseTypeDef](./type_defs.md#describequeriesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeQueriesRequestDescribeQueriesPaginateTypeDef = {  # (1)
    "logGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeQueriesRequestDescribeQueriesPaginateTypeDef](./type_defs.md#describequeriesrequestdescribequeriespaginatetypedef) 
## DescribeResourcePoliciesPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("describe_resource_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeResourcePolicies)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeResourcePoliciesPaginator

session = get_session()
async with session.create_client("logs") as client:
    client: CloudWatchLogsClient
    paginator: DescribeResourcePoliciesPaginator = client.get_paginator("describe_resource_policies")
```


### paginate

Type annotations and code completion for `#!python DescribeResourcePoliciesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeResourcePoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeResourcePoliciesResponseTypeDef](./type_defs.md#describeresourcepoliciesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef](./type_defs.md#describeresourcepoliciesrequestdescriberesourcepoliciespaginatetypedef) 
## DescribeSubscriptionFiltersPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("describe_subscription_filters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeSubscriptionFilters)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeSubscriptionFiltersPaginator

session = get_session()
async with session.create_client("logs") as client:
    client: CloudWatchLogsClient
    paginator: DescribeSubscriptionFiltersPaginator = client.get_paginator("describe_subscription_filters")
```


### paginate

Type annotations and code completion for `#!python DescribeSubscriptionFiltersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    logGroupName: str,
    filterNamePrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeSubscriptionFiltersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeSubscriptionFiltersResponseTypeDef](./type_defs.md#describesubscriptionfiltersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef = {  # (1)
    "logGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef](./type_defs.md#describesubscriptionfiltersrequestdescribesubscriptionfilterspaginatetypedef) 
## FilterLogEventsPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("filter_log_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.FilterLogEvents)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import FilterLogEventsPaginator

session = get_session()
async with session.create_client("logs") as client:
    client: CloudWatchLogsClient
    paginator: FilterLogEventsPaginator = client.get_paginator("filter_log_events")
```


### paginate

Type annotations and code completion for `#!python FilterLogEventsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    logGroupName: str,
    logStreamNames: Sequence[str] = ...,
    logStreamNamePrefix: str = ...,
    startTime: int = ...,
    endTime: int = ...,
    filterPattern: str = ...,
    interleaved: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[FilterLogEventsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: FilterLogEventsResponseTypeDef](./type_defs.md#filterlogeventsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: FilterLogEventsRequestFilterLogEventsPaginateTypeDef = {  # (1)
    "logGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: FilterLogEventsRequestFilterLogEventsPaginateTypeDef](./type_defs.md#filterlogeventsrequestfilterlogeventspaginatetypedef) 
