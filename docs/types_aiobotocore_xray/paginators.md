<a id="paginators-for-aiobotocore-xray-module"></a>

# Paginators for aiobotocore XRay module

> [Index](../README.md) > [XRay](./README.md) > Paginators

Auto-generated documentation for
[XRay](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
type annotations stubs module
[types-aiobotocore-xray](https://pypi.org/project/types-aiobotocore-xray/).

- [Paginators for aiobotocore XRay module](#paginators-for-aiobotocore-xray-module)
  - [BatchGetTracesPaginator](#batchgettracespaginator)
  - [GetGroupsPaginator](#getgroupspaginator)
  - [GetSamplingRulesPaginator](#getsamplingrulespaginator)
  - [GetSamplingStatisticSummariesPaginator](#getsamplingstatisticsummariespaginator)
  - [GetServiceGraphPaginator](#getservicegraphpaginator)
  - [GetTimeSeriesServiceStatisticsPaginator](#gettimeseriesservicestatisticspaginator)
  - [GetTraceGraphPaginator](#gettracegraphpaginator)
  - [GetTraceSummariesPaginator](#gettracesummariespaginator)

<a id="batchgettracespaginator"></a>

## BatchGetTracesPaginator

Type annotations for
`session.create_client("xray").get_paginator("batch_get_traces")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_xray.paginator import BatchGetTracesPaginator

session = get_session()
async with session.create_client("xray") as client:
    client: XRayClient
    paginator: BatchGetTracesPaginator = client.get_paginator("batch_get_traces")
```

Boto3 documentation:
[XRay.Paginator.BatchGetTraces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.BatchGetTraces)

Arguments for `BatchGetTracesPaginator.paginate` method:

- `TraceIds`: `Sequence`\[`str`\] *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`BatchGetTracesPaginator.paginate` returns
`AsyncIterator`\[[BatchGetTracesResultTypeDef](./type_defs.md#batchgettracesresulttypedef)\].

<a id="getgroupspaginator"></a>

## GetGroupsPaginator

Type annotations for
`session.create_client("xray").get_paginator("get_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_xray.paginator import GetGroupsPaginator

session = get_session()
async with session.create_client("xray") as client:
    client: XRayClient
    paginator: GetGroupsPaginator = client.get_paginator("get_groups")
```

Boto3 documentation:
[XRay.Paginator.GetGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetGroups)

Arguments for `GetGroupsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetGroupsPaginator.paginate` returns
`AsyncIterator`\[[GetGroupsResultTypeDef](./type_defs.md#getgroupsresulttypedef)\].

<a id="getsamplingrulespaginator"></a>

## GetSamplingRulesPaginator

Type annotations for
`session.create_client("xray").get_paginator("get_sampling_rules")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_xray.paginator import GetSamplingRulesPaginator

session = get_session()
async with session.create_client("xray") as client:
    client: XRayClient
    paginator: GetSamplingRulesPaginator = client.get_paginator("get_sampling_rules")
```

Boto3 documentation:
[XRay.Paginator.GetSamplingRules](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingRules)

Arguments for `GetSamplingRulesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetSamplingRulesPaginator.paginate` returns
`AsyncIterator`\[[GetSamplingRulesResultTypeDef](./type_defs.md#getsamplingrulesresulttypedef)\].

<a id="getsamplingstatisticsummariespaginator"></a>

## GetSamplingStatisticSummariesPaginator

Type annotations for
`session.create_client("xray").get_paginator("get_sampling_statistic_summaries")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_xray.paginator import GetSamplingStatisticSummariesPaginator

session = get_session()
async with session.create_client("xray") as client:
    client: XRayClient
    paginator: GetSamplingStatisticSummariesPaginator = client.get_paginator("get_sampling_statistic_summaries")
```

Boto3 documentation:
[XRay.Paginator.GetSamplingStatisticSummaries](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingStatisticSummaries)

Arguments for `GetSamplingStatisticSummariesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetSamplingStatisticSummariesPaginator.paginate` returns
`AsyncIterator`\[[GetSamplingStatisticSummariesResultTypeDef](./type_defs.md#getsamplingstatisticsummariesresulttypedef)\].

<a id="getservicegraphpaginator"></a>

## GetServiceGraphPaginator

Type annotations for
`session.create_client("xray").get_paginator("get_service_graph")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_xray.paginator import GetServiceGraphPaginator

session = get_session()
async with session.create_client("xray") as client:
    client: XRayClient
    paginator: GetServiceGraphPaginator = client.get_paginator("get_service_graph")
```

Boto3 documentation:
[XRay.Paginator.GetServiceGraph](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetServiceGraph)

Arguments for `GetServiceGraphPaginator.paginate` method:

- `StartTime`: `Union`\[`datetime`, `str`\] *(required)*
- `EndTime`: `Union`\[`datetime`, `str`\] *(required)*
- `GroupName`: `str`
- `GroupARN`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetServiceGraphPaginator.paginate` returns
`AsyncIterator`\[[GetServiceGraphResultTypeDef](./type_defs.md#getservicegraphresulttypedef)\].

<a id="gettimeseriesservicestatisticspaginator"></a>

## GetTimeSeriesServiceStatisticsPaginator

Type annotations for
`session.create_client("xray").get_paginator("get_time_series_service_statistics")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_xray.paginator import GetTimeSeriesServiceStatisticsPaginator

session = get_session()
async with session.create_client("xray") as client:
    client: XRayClient
    paginator: GetTimeSeriesServiceStatisticsPaginator = client.get_paginator("get_time_series_service_statistics")
```

Boto3 documentation:
[XRay.Paginator.GetTimeSeriesServiceStatistics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTimeSeriesServiceStatistics)

Arguments for `GetTimeSeriesServiceStatisticsPaginator.paginate` method:

- `StartTime`: `Union`\[`datetime`, `str`\] *(required)*
- `EndTime`: `Union`\[`datetime`, `str`\] *(required)*
- `GroupName`: `str`
- `GroupARN`: `str`
- `EntitySelectorExpression`: `str`
- `Period`: `int`
- `ForecastStatistics`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetTimeSeriesServiceStatisticsPaginator.paginate` returns
`AsyncIterator`\[[GetTimeSeriesServiceStatisticsResultTypeDef](./type_defs.md#gettimeseriesservicestatisticsresulttypedef)\].

<a id="gettracegraphpaginator"></a>

## GetTraceGraphPaginator

Type annotations for
`session.create_client("xray").get_paginator("get_trace_graph")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_xray.paginator import GetTraceGraphPaginator

session = get_session()
async with session.create_client("xray") as client:
    client: XRayClient
    paginator: GetTraceGraphPaginator = client.get_paginator("get_trace_graph")
```

Boto3 documentation:
[XRay.Paginator.GetTraceGraph](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceGraph)

Arguments for `GetTraceGraphPaginator.paginate` method:

- `TraceIds`: `Sequence`\[`str`\] *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetTraceGraphPaginator.paginate` returns
`AsyncIterator`\[[GetTraceGraphResultTypeDef](./type_defs.md#gettracegraphresulttypedef)\].

<a id="gettracesummariespaginator"></a>

## GetTraceSummariesPaginator

Type annotations for
`session.create_client("xray").get_paginator("get_trace_summaries")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_xray.paginator import GetTraceSummariesPaginator

session = get_session()
async with session.create_client("xray") as client:
    client: XRayClient
    paginator: GetTraceSummariesPaginator = client.get_paginator("get_trace_summaries")
```

Boto3 documentation:
[XRay.Paginator.GetTraceSummaries](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceSummaries)

Arguments for `GetTraceSummariesPaginator.paginate` method:

- `StartTime`: `Union`\[`datetime`, `str`\] *(required)*
- `EndTime`: `Union`\[`datetime`, `str`\] *(required)*
- `TimeRangeType`: [TimeRangeTypeType](./literals.md#timerangetypetype)
- `Sampling`: `bool`
- `SamplingStrategy`:
  [SamplingStrategyTypeDef](./type_defs.md#samplingstrategytypedef)
- `FilterExpression`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetTraceSummariesPaginator.paginate` returns
`AsyncIterator`\[[GetTraceSummariesResultTypeDef](./type_defs.md#gettracesummariesresulttypedef)\].
