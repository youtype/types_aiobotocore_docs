# Paginators

> [Index](../README.md) > [CodeGuruProfiler](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CodeGuruProfiler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#codeguruprofiler)
    type annotations stubs module [types-aiobotocore-codeguruprofiler](https://pypi.org/project/types-aiobotocore-codeguruprofiler/).

## ListProfileTimesPaginator

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").get_paginator("list_profile_times")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler/paginator/ListProfileTimes.html#CodeGuruProfiler.Paginator.ListProfileTimes)

```python
# ListProfileTimesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codeguruprofiler.paginator import ListProfileTimesPaginator

session = get_session()
async with session.create_client("codeguruprofiler") as client:  # (1)
    paginator: ListProfileTimesPaginator = client.get_paginator("list_profile_times")  # (2)
    async for item in paginator.paginate(...):
        item: ListProfileTimesResponseTypeDef
        print(item)  # (3)
```

1. client: [CodeGuruProfilerClient](./client.md)
2. paginator: [ListProfileTimesPaginator](./paginators.md#listprofiletimespaginator)
3. item: [:material-code-braces: ListProfileTimesResponseTypeDef](./type_defs.md#listprofiletimesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListProfileTimesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    endTime: TimestampTypeDef,
    period: AggregationPeriodType,  # (1)
    profilingGroupName: str,
    startTime: TimestampTypeDef,
    orderBy: OrderByType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListProfileTimesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: AggregationPeriodType](./literals.md#aggregationperiodtype) 
2. See [:material-code-brackets: OrderByType](./literals.md#orderbytype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListProfileTimesResponseTypeDef](./type_defs.md#listprofiletimesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListProfileTimesRequestPaginateTypeDef = {  # (1)
    "endTime": ...,
    "period": ...,
    "profilingGroupName": ...,
    "startTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProfileTimesRequestPaginateTypeDef](./type_defs.md#listprofiletimesrequestpaginatetypedef) 
