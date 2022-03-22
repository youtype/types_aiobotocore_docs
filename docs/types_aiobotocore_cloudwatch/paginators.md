<a id="paginators-for-aiobotocore-cloudwatch-module"></a>

# Paginators for aiobotocore CloudWatch module

> [Index](../README.md) > [CloudWatch](./README.md) > Paginators

Auto-generated documentation for
[CloudWatch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
type annotations stubs module
[types-aiobotocore-cloudwatch](https://pypi.org/project/types-aiobotocore-cloudwatch/).

- [Paginators for aiobotocore CloudWatch module](#paginators-for-aiobotocore-cloudwatch-module)
  - [DescribeAlarmHistoryPaginator](#describealarmhistorypaginator)
  - [DescribeAlarmsPaginator](#describealarmspaginator)
  - [GetMetricDataPaginator](#getmetricdatapaginator)
  - [ListDashboardsPaginator](#listdashboardspaginator)
  - [ListMetricsPaginator](#listmetricspaginator)

<a id="describealarmhistorypaginator"></a>

## DescribeAlarmHistoryPaginator

Type annotations for
`session.create_client("cloudwatch").get_paginator("describe_alarm_history")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudwatch.paginator import DescribeAlarmHistoryPaginator

session = get_session()
async with session.create_client("cloudwatch") as client:
    client: CloudWatchClient
    paginator: DescribeAlarmHistoryPaginator = client.get_paginator("describe_alarm_history")
```

Boto3 documentation:
[CloudWatch.Paginator.DescribeAlarmHistory](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAlarmHistory)

Arguments for `DescribeAlarmHistoryPaginator.paginate` method:

- `AlarmName`: `str`
- `AlarmTypes`: `Sequence`\[[AlarmTypeType](./literals.md#alarmtypetype)\]
- `HistoryItemType`: [HistoryItemTypeType](./literals.md#historyitemtypetype)
- `StartDate`: `Union`\[`datetime`, `str`\]
- `EndDate`: `Union`\[`datetime`, `str`\]
- `ScanBy`: [ScanByType](./literals.md#scanbytype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeAlarmHistoryPaginator.paginate` returns
`AsyncIterator`\[[DescribeAlarmHistoryOutputTypeDef](./type_defs.md#describealarmhistoryoutputtypedef)\].

<a id="describealarmspaginator"></a>

## DescribeAlarmsPaginator

Type annotations for
`session.create_client("cloudwatch").get_paginator("describe_alarms")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudwatch.paginator import DescribeAlarmsPaginator

session = get_session()
async with session.create_client("cloudwatch") as client:
    client: CloudWatchClient
    paginator: DescribeAlarmsPaginator = client.get_paginator("describe_alarms")
```

Boto3 documentation:
[CloudWatch.Paginator.DescribeAlarms](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAlarms)

Arguments for `DescribeAlarmsPaginator.paginate` method:

- `AlarmNames`: `Sequence`\[`str`\]
- `AlarmNamePrefix`: `str`
- `AlarmTypes`: `Sequence`\[[AlarmTypeType](./literals.md#alarmtypetype)\]
- `ChildrenOfAlarmName`: `str`
- `ParentsOfAlarmName`: `str`
- `StateValue`: [StateValueType](./literals.md#statevaluetype)
- `ActionPrefix`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeAlarmsPaginator.paginate` returns
`AsyncIterator`\[[DescribeAlarmsOutputTypeDef](./type_defs.md#describealarmsoutputtypedef)\].

<a id="getmetricdatapaginator"></a>

## GetMetricDataPaginator

Type annotations for
`session.create_client("cloudwatch").get_paginator("get_metric_data")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudwatch.paginator import GetMetricDataPaginator

session = get_session()
async with session.create_client("cloudwatch") as client:
    client: CloudWatchClient
    paginator: GetMetricDataPaginator = client.get_paginator("get_metric_data")
```

Boto3 documentation:
[CloudWatch.Paginator.GetMetricData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.GetMetricData)

Arguments for `GetMetricDataPaginator.paginate` method:

- `MetricDataQueries`:
  `Sequence`\[[MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef)\]
  *(required)*
- `StartTime`: `Union`\[`datetime`, `str`\] *(required)*
- `EndTime`: `Union`\[`datetime`, `str`\] *(required)*
- `ScanBy`: [ScanByType](./literals.md#scanbytype)
- `LabelOptions`: [LabelOptionsTypeDef](./type_defs.md#labeloptionstypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetMetricDataPaginator.paginate` returns
`AsyncIterator`\[[GetMetricDataOutputTypeDef](./type_defs.md#getmetricdataoutputtypedef)\].

<a id="listdashboardspaginator"></a>

## ListDashboardsPaginator

Type annotations for
`session.create_client("cloudwatch").get_paginator("list_dashboards")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudwatch.paginator import ListDashboardsPaginator

session = get_session()
async with session.create_client("cloudwatch") as client:
    client: CloudWatchClient
    paginator: ListDashboardsPaginator = client.get_paginator("list_dashboards")
```

Boto3 documentation:
[CloudWatch.Paginator.ListDashboards](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.ListDashboards)

Arguments for `ListDashboardsPaginator.paginate` method:

- `DashboardNamePrefix`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDashboardsPaginator.paginate` returns
`AsyncIterator`\[[ListDashboardsOutputTypeDef](./type_defs.md#listdashboardsoutputtypedef)\].

<a id="listmetricspaginator"></a>

## ListMetricsPaginator

Type annotations for
`session.create_client("cloudwatch").get_paginator("list_metrics")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudwatch.paginator import ListMetricsPaginator

session = get_session()
async with session.create_client("cloudwatch") as client:
    client: CloudWatchClient
    paginator: ListMetricsPaginator = client.get_paginator("list_metrics")
```

Boto3 documentation:
[CloudWatch.Paginator.ListMetrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.ListMetrics)

Arguments for `ListMetricsPaginator.paginate` method:

- `Namespace`: `str`
- `MetricName`: `str`
- `Dimensions`:
  `Sequence`\[[DimensionFilterTypeDef](./type_defs.md#dimensionfiltertypedef)\]
- `RecentlyActive`: `Literal['PT3H']` (see
  [RecentlyActiveType](./literals.md#recentlyactivetype))
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListMetricsPaginator.paginate` returns
`AsyncIterator`\[[ListMetricsOutputTypeDef](./type_defs.md#listmetricsoutputtypedef)\].
