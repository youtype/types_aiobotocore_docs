# Paginators

> [Index](../README.md) > [CodeGuruProfiler](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CodeGuruProfiler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
    type annotations stubs module [types-aiobotocore-codeguruprofiler](https://pypi.org/project/types-aiobotocore-codeguruprofiler/).

## ListProfileTimesPaginator

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").get_paginator("list_profile_times")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Paginator.ListProfileTimes)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codeguruprofiler.paginator import ListProfileTimesPaginator

session = get_session()
async with session.create_client("codeguruprofiler") as client:
    client: CodeGuruProfilerClient
    paginator: ListProfileTimesPaginator = client.get_paginator("list_profile_times")
```


### paginate

Type annotations and code completion for `#!python ListProfileTimesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    endTime: Union[datetime, str],
    period: AggregationPeriodType,  # (1)
    profilingGroupName: str,
    startTime: Union[datetime, str],
    orderBy: OrderByType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListProfileTimesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: AggregationPeriodType](./literals.md#aggregationperiodtype) 
2. See [:material-code-brackets: OrderByType](./literals.md#orderbytype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListProfileTimesResponseTypeDef](./type_defs.md#listprofiletimesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListProfileTimesRequestListProfileTimesPaginateTypeDef = {  # (1)
    "endTime": ...,
    "period": ...,
    "profilingGroupName": ...,
    "startTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProfileTimesRequestListProfileTimesPaginateTypeDef](./type_defs.md#listprofiletimesrequestlistprofiletimespaginatetypedef) 
