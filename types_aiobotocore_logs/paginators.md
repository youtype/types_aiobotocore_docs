<a id="paginators-for-aiobotocore-cloudwatchlogs-module"></a>

# Paginators for aiobotocore CloudWatchLogs module

> [Index](..) > [CloudWatchLogs](.) > Paginators

Auto-generated documentation for
[CloudWatchLogs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
type annotations stubs module
[types-aiobotocore-logs](https://pypi.org/project/types-aiobotocore-logs/).

- [Paginators for aiobotocore CloudWatchLogs module](#paginators-for-aiobotocore-cloudwatchlogs-module)
  - [DescribeDestinationsPaginator](#describedestinationspaginator)
  - [DescribeExportTasksPaginator](#describeexporttaskspaginator)
  - [DescribeLogGroupsPaginator](#describeloggroupspaginator)
  - [DescribeLogStreamsPaginator](#describelogstreamspaginator)
  - [DescribeMetricFiltersPaginator](#describemetricfilterspaginator)
  - [DescribeQueriesPaginator](#describequeriespaginator)
  - [DescribeResourcePoliciesPaginator](#describeresourcepoliciespaginator)
  - [DescribeSubscriptionFiltersPaginator](#describesubscriptionfilterspaginator)
  - [FilterLogEventsPaginator](#filterlogeventspaginator)

<a id="describedestinationspaginator"></a>

## DescribeDestinationsPaginator

Type annotations for
`session.create_client("logs").get_paginator("describe_destinations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeDestinationsPaginator

session = get_session()
async with session.create_client("logs") as client:
    client: CloudWatchLogsClient
    paginator: DescribeDestinationsPaginator = client.get_paginator("describe_destinations")
```

Boto3 documentation:
[CloudWatchLogs.Paginator.DescribeDestinations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeDestinations)

Arguments for `DescribeDestinationsPaginator.paginate` method:

- `DestinationNamePrefix`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeDestinationsPaginator.paginate` returns
`_PageIterator`\[[DescribeDestinationsResponseTypeDef](./type_defs.md#describedestinationsresponsetypedef)\].

<a id="describeexporttaskspaginator"></a>

## DescribeExportTasksPaginator

Type annotations for
`session.create_client("logs").get_paginator("describe_export_tasks")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeExportTasksPaginator

session = get_session()
async with session.create_client("logs") as client:
    client: CloudWatchLogsClient
    paginator: DescribeExportTasksPaginator = client.get_paginator("describe_export_tasks")
```

Boto3 documentation:
[CloudWatchLogs.Paginator.DescribeExportTasks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeExportTasks)

Arguments for `DescribeExportTasksPaginator.paginate` method:

- `taskId`: `str`
- `statusCode`:
  [ExportTaskStatusCodeType](./literals.md#exporttaskstatuscodetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeExportTasksPaginator.paginate` returns
`_PageIterator`\[[DescribeExportTasksResponseTypeDef](./type_defs.md#describeexporttasksresponsetypedef)\].

<a id="describeloggroupspaginator"></a>

## DescribeLogGroupsPaginator

Type annotations for
`session.create_client("logs").get_paginator("describe_log_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeLogGroupsPaginator

session = get_session()
async with session.create_client("logs") as client:
    client: CloudWatchLogsClient
    paginator: DescribeLogGroupsPaginator = client.get_paginator("describe_log_groups")
```

Boto3 documentation:
[CloudWatchLogs.Paginator.DescribeLogGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogGroups)

Arguments for `DescribeLogGroupsPaginator.paginate` method:

- `logGroupNamePrefix`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeLogGroupsPaginator.paginate` returns
`_PageIterator`\[[DescribeLogGroupsResponseTypeDef](./type_defs.md#describeloggroupsresponsetypedef)\].

<a id="describelogstreamspaginator"></a>

## DescribeLogStreamsPaginator

Type annotations for
`session.create_client("logs").get_paginator("describe_log_streams")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeLogStreamsPaginator

session = get_session()
async with session.create_client("logs") as client:
    client: CloudWatchLogsClient
    paginator: DescribeLogStreamsPaginator = client.get_paginator("describe_log_streams")
```

Boto3 documentation:
[CloudWatchLogs.Paginator.DescribeLogStreams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogStreams)

Arguments for `DescribeLogStreamsPaginator.paginate` method:

- `logGroupName`: `str` *(required)*
- `logStreamNamePrefix`: `str`
- `orderBy`: [OrderByType](./literals.md#orderbytype)
- `descending`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeLogStreamsPaginator.paginate` returns
`_PageIterator`\[[DescribeLogStreamsResponseTypeDef](./type_defs.md#describelogstreamsresponsetypedef)\].

<a id="describemetricfilterspaginator"></a>

## DescribeMetricFiltersPaginator

Type annotations for
`session.create_client("logs").get_paginator("describe_metric_filters")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeMetricFiltersPaginator

session = get_session()
async with session.create_client("logs") as client:
    client: CloudWatchLogsClient
    paginator: DescribeMetricFiltersPaginator = client.get_paginator("describe_metric_filters")
```

Boto3 documentation:
[CloudWatchLogs.Paginator.DescribeMetricFilters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeMetricFilters)

Arguments for `DescribeMetricFiltersPaginator.paginate` method:

- `logGroupName`: `str`
- `filterNamePrefix`: `str`
- `metricName`: `str`
- `metricNamespace`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeMetricFiltersPaginator.paginate` returns
`_PageIterator`\[[DescribeMetricFiltersResponseTypeDef](./type_defs.md#describemetricfiltersresponsetypedef)\].

<a id="describequeriespaginator"></a>

## DescribeQueriesPaginator

Type annotations for
`session.create_client("logs").get_paginator("describe_queries")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeQueriesPaginator

session = get_session()
async with session.create_client("logs") as client:
    client: CloudWatchLogsClient
    paginator: DescribeQueriesPaginator = client.get_paginator("describe_queries")
```

Boto3 documentation:
[CloudWatchLogs.Paginator.DescribeQueries](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeQueries)

Arguments for `DescribeQueriesPaginator.paginate` method:

- `logGroupName`: `str`
- `status`: [QueryStatusType](./literals.md#querystatustype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeQueriesPaginator.paginate` returns
`_PageIterator`\[[DescribeQueriesResponseTypeDef](./type_defs.md#describequeriesresponsetypedef)\].

<a id="describeresourcepoliciespaginator"></a>

## DescribeResourcePoliciesPaginator

Type annotations for
`session.create_client("logs").get_paginator("describe_resource_policies")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeResourcePoliciesPaginator

session = get_session()
async with session.create_client("logs") as client:
    client: CloudWatchLogsClient
    paginator: DescribeResourcePoliciesPaginator = client.get_paginator("describe_resource_policies")
```

Boto3 documentation:
[CloudWatchLogs.Paginator.DescribeResourcePolicies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeResourcePolicies)

Arguments for `DescribeResourcePoliciesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeResourcePoliciesPaginator.paginate` returns
`_PageIterator`\[[DescribeResourcePoliciesResponseTypeDef](./type_defs.md#describeresourcepoliciesresponsetypedef)\].

<a id="describesubscriptionfilterspaginator"></a>

## DescribeSubscriptionFiltersPaginator

Type annotations for
`session.create_client("logs").get_paginator("describe_subscription_filters")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeSubscriptionFiltersPaginator

session = get_session()
async with session.create_client("logs") as client:
    client: CloudWatchLogsClient
    paginator: DescribeSubscriptionFiltersPaginator = client.get_paginator("describe_subscription_filters")
```

Boto3 documentation:
[CloudWatchLogs.Paginator.DescribeSubscriptionFilters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeSubscriptionFilters)

Arguments for `DescribeSubscriptionFiltersPaginator.paginate` method:

- `logGroupName`: `str` *(required)*
- `filterNamePrefix`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeSubscriptionFiltersPaginator.paginate` returns
`_PageIterator`\[[DescribeSubscriptionFiltersResponseTypeDef](./type_defs.md#describesubscriptionfiltersresponsetypedef)\].

<a id="filterlogeventspaginator"></a>

## FilterLogEventsPaginator

Type annotations for
`session.create_client("logs").get_paginator("filter_log_events")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import FilterLogEventsPaginator

session = get_session()
async with session.create_client("logs") as client:
    client: CloudWatchLogsClient
    paginator: FilterLogEventsPaginator = client.get_paginator("filter_log_events")
```

Boto3 documentation:
[CloudWatchLogs.Paginator.FilterLogEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.FilterLogEvents)

Arguments for `FilterLogEventsPaginator.paginate` method:

- `logGroupName`: `str` *(required)*
- `logStreamNames`: `Sequence`\[`str`\]
- `logStreamNamePrefix`: `str`
- `startTime`: `int`
- `endTime`: `int`
- `filterPattern`: `str`
- `interleaved`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`FilterLogEventsPaginator.paginate` returns
`_PageIterator`\[[FilterLogEventsResponseTypeDef](./type_defs.md#filterlogeventsresponsetypedef)\].
