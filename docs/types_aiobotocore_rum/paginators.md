<a id="paginators-for-aiobotocore-cloudwatchrum-module"></a>

# Paginators for aiobotocore CloudWatchRUM module

> [Index](../README.md) > [CloudWatchRUM](./README.md) > Paginators

Auto-generated documentation for
[CloudWatchRUM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
type annotations stubs module
[types-aiobotocore-rum](https://pypi.org/project/types-aiobotocore-rum/).

- [Paginators for aiobotocore CloudWatchRUM module](#paginators-for-aiobotocore-cloudwatchrum-module)
  - [GetAppMonitorDataPaginator](#getappmonitordatapaginator)
  - [ListAppMonitorsPaginator](#listappmonitorspaginator)

<a id="getappmonitordatapaginator"></a>

## GetAppMonitorDataPaginator

Type annotations for
`session.create_client("rum").get_paginator("get_app_monitor_data")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_rum.paginator import GetAppMonitorDataPaginator

session = get_session()
async with session.create_client("rum") as client:
    client: CloudWatchRUMClient
    paginator: GetAppMonitorDataPaginator = client.get_paginator("get_app_monitor_data")
```

Boto3 documentation:
[CloudWatchRUM.Paginator.GetAppMonitorData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.GetAppMonitorData)

Arguments for `GetAppMonitorDataPaginator.paginate` method:

- `Name`: `str` *(required)*
- `TimeRange`: [TimeRangeTypeDef](./type_defs.md#timerangetypedef) *(required)*
- `Filters`:
  `Sequence`\[[QueryFilterTypeDef](./type_defs.md#queryfiltertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetAppMonitorDataPaginator.paginate` returns
`AsyncIterator`\[[GetAppMonitorDataResponseTypeDef](./type_defs.md#getappmonitordataresponsetypedef)\].

<a id="listappmonitorspaginator"></a>

## ListAppMonitorsPaginator

Type annotations for
`session.create_client("rum").get_paginator("list_app_monitors")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_rum.paginator import ListAppMonitorsPaginator

session = get_session()
async with session.create_client("rum") as client:
    client: CloudWatchRUMClient
    paginator: ListAppMonitorsPaginator = client.get_paginator("list_app_monitors")
```

Boto3 documentation:
[CloudWatchRUM.Paginator.ListAppMonitors](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.ListAppMonitors)

Arguments for `ListAppMonitorsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAppMonitorsPaginator.paginate` returns
`AsyncIterator`\[[ListAppMonitorsResponseTypeDef](./type_defs.md#listappmonitorsresponsetypedef)\].
