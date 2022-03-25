<a id="paginators-for-aiobotocore-codeguruprofiler-module"></a>

# Paginators for aiobotocore CodeGuruProfiler module

> [Index](../README.md) > [CodeGuruProfiler](./README.md) > Paginators

Auto-generated documentation for
[CodeGuruProfiler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
type annotations stubs module
[types-aiobotocore-codeguruprofiler](https://pypi.org/project/types-aiobotocore-codeguruprofiler/).

- [Paginators for aiobotocore CodeGuruProfiler module](#paginators-for-aiobotocore-codeguruprofiler-module)
  - [ListProfileTimesPaginator](#listprofiletimespaginator)

<a id="listprofiletimespaginator"></a>

## ListProfileTimesPaginator

Type annotations for
`session.create_client("codeguruprofiler").get_paginator("list_profile_times")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codeguruprofiler.paginator import ListProfileTimesPaginator

session = get_session()
async with session.create_client("codeguruprofiler") as client:
    client: CodeGuruProfilerClient
    paginator: ListProfileTimesPaginator = client.get_paginator("list_profile_times")
```

Boto3 documentation:
[CodeGuruProfiler.Paginator.ListProfileTimes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Paginator.ListProfileTimes)

Arguments for `ListProfileTimesPaginator.paginate` method:

- `endTime`: `Union`\[`datetime`, `str`\] *(required)*
- `period`: [AggregationPeriodType](./literals.md#aggregationperiodtype)
  *(required)*
- `profilingGroupName`: `str` *(required)*
- `startTime`: `Union`\[`datetime`, `str`\] *(required)*
- `orderBy`: [OrderByType](./literals.md#orderbytype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListProfileTimesPaginator.paginate` returns
`AsyncIterator`\[[ListProfileTimesResponseTypeDef](./type_defs.md#listprofiletimesresponsetypedef)\].