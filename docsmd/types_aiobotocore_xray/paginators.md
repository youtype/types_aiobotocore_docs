# Paginators

> [Index](../README.md) > [XRay](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [XRay](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#xray)
    type annotations stubs module [types-aiobotocore-xray](https://pypi.org/project/types-aiobotocore-xray/).

## BatchGetTracesPaginator

Type annotations and code completion for `#!python session.create_client("xray").get_paginator("batch_get_traces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray/paginator/BatchGetTraces.html#XRay.Paginator.BatchGetTraces)

```python
# BatchGetTracesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_xray.paginator import BatchGetTracesPaginator

session = get_session()
async with session.create_client("xray") as client:  # (1)
    paginator: BatchGetTracesPaginator = client.get_paginator("batch_get_traces")  # (2)
    async for item in paginator.paginate(...):
        item: BatchGetTracesResultTypeDef
        print(item)  # (3)
```

1. client: [XRayClient](./client.md)
2. paginator: [BatchGetTracesPaginator](./paginators.md#batchgettracespaginator)
3. item: [:material-code-braces: BatchGetTracesResultTypeDef](./type_defs.md#batchgettracesresulttypedef) 


### paginate

Type annotations and code completion for `#!python BatchGetTracesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TraceIds: Sequence[str],
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[BatchGetTracesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: BatchGetTracesResultTypeDef](./type_defs.md#batchgettracesresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: BatchGetTracesRequestPaginateTypeDef = {  # (1)
    "TraceIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: BatchGetTracesRequestPaginateTypeDef](./type_defs.md#batchgettracesrequestpaginatetypedef) 
## GetGroupsPaginator

Type annotations and code completion for `#!python session.create_client("xray").get_paginator("get_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray/paginator/GetGroups.html#XRay.Paginator.GetGroups)

```python
# GetGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_xray.paginator import GetGroupsPaginator

session = get_session()
async with session.create_client("xray") as client:  # (1)
    paginator: GetGroupsPaginator = client.get_paginator("get_groups")  # (2)
    async for item in paginator.paginate(...):
        item: GetGroupsResultTypeDef
        print(item)  # (3)
```

1. client: [XRayClient](./client.md)
2. paginator: [GetGroupsPaginator](./paginators.md#getgroupspaginator)
3. item: [:material-code-braces: GetGroupsResultTypeDef](./type_defs.md#getgroupsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetGroupsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetGroupsResultTypeDef](./type_defs.md#getgroupsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetGroupsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetGroupsRequestPaginateTypeDef](./type_defs.md#getgroupsrequestpaginatetypedef) 
## GetSamplingRulesPaginator

Type annotations and code completion for `#!python session.create_client("xray").get_paginator("get_sampling_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray/paginator/GetSamplingRules.html#XRay.Paginator.GetSamplingRules)

```python
# GetSamplingRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_xray.paginator import GetSamplingRulesPaginator

session = get_session()
async with session.create_client("xray") as client:  # (1)
    paginator: GetSamplingRulesPaginator = client.get_paginator("get_sampling_rules")  # (2)
    async for item in paginator.paginate(...):
        item: GetSamplingRulesResultTypeDef
        print(item)  # (3)
```

1. client: [XRayClient](./client.md)
2. paginator: [GetSamplingRulesPaginator](./paginators.md#getsamplingrulespaginator)
3. item: [:material-code-braces: GetSamplingRulesResultTypeDef](./type_defs.md#getsamplingrulesresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetSamplingRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetSamplingRulesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetSamplingRulesResultTypeDef](./type_defs.md#getsamplingrulesresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetSamplingRulesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetSamplingRulesRequestPaginateTypeDef](./type_defs.md#getsamplingrulesrequestpaginatetypedef) 
## GetSamplingStatisticSummariesPaginator

Type annotations and code completion for `#!python session.create_client("xray").get_paginator("get_sampling_statistic_summaries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray/paginator/GetSamplingStatisticSummaries.html#XRay.Paginator.GetSamplingStatisticSummaries)

```python
# GetSamplingStatisticSummariesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_xray.paginator import GetSamplingStatisticSummariesPaginator

session = get_session()
async with session.create_client("xray") as client:  # (1)
    paginator: GetSamplingStatisticSummariesPaginator = client.get_paginator("get_sampling_statistic_summaries")  # (2)
    async for item in paginator.paginate(...):
        item: GetSamplingStatisticSummariesResultTypeDef
        print(item)  # (3)
```

1. client: [XRayClient](./client.md)
2. paginator: [GetSamplingStatisticSummariesPaginator](./paginators.md#getsamplingstatisticsummariespaginator)
3. item: [:material-code-braces: GetSamplingStatisticSummariesResultTypeDef](./type_defs.md#getsamplingstatisticsummariesresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetSamplingStatisticSummariesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetSamplingStatisticSummariesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetSamplingStatisticSummariesResultTypeDef](./type_defs.md#getsamplingstatisticsummariesresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetSamplingStatisticSummariesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetSamplingStatisticSummariesRequestPaginateTypeDef](./type_defs.md#getsamplingstatisticsummariesrequestpaginatetypedef) 
## GetServiceGraphPaginator

Type annotations and code completion for `#!python session.create_client("xray").get_paginator("get_service_graph")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray/paginator/GetServiceGraph.html#XRay.Paginator.GetServiceGraph)

```python
# GetServiceGraphPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_xray.paginator import GetServiceGraphPaginator

session = get_session()
async with session.create_client("xray") as client:  # (1)
    paginator: GetServiceGraphPaginator = client.get_paginator("get_service_graph")  # (2)
    async for item in paginator.paginate(...):
        item: GetServiceGraphResultTypeDef
        print(item)  # (3)
```

1. client: [XRayClient](./client.md)
2. paginator: [GetServiceGraphPaginator](./paginators.md#getservicegraphpaginator)
3. item: [:material-code-braces: GetServiceGraphResultTypeDef](./type_defs.md#getservicegraphresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetServiceGraphPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    GroupName: str = ...,
    GroupARN: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetServiceGraphResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetServiceGraphResultTypeDef](./type_defs.md#getservicegraphresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetServiceGraphRequestPaginateTypeDef = {  # (1)
    "StartTime": ...,
    "EndTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetServiceGraphRequestPaginateTypeDef](./type_defs.md#getservicegraphrequestpaginatetypedef) 
## GetTimeSeriesServiceStatisticsPaginator

Type annotations and code completion for `#!python session.create_client("xray").get_paginator("get_time_series_service_statistics")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray/paginator/GetTimeSeriesServiceStatistics.html#XRay.Paginator.GetTimeSeriesServiceStatistics)

```python
# GetTimeSeriesServiceStatisticsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_xray.paginator import GetTimeSeriesServiceStatisticsPaginator

session = get_session()
async with session.create_client("xray") as client:  # (1)
    paginator: GetTimeSeriesServiceStatisticsPaginator = client.get_paginator("get_time_series_service_statistics")  # (2)
    async for item in paginator.paginate(...):
        item: GetTimeSeriesServiceStatisticsResultTypeDef
        print(item)  # (3)
```

1. client: [XRayClient](./client.md)
2. paginator: [GetTimeSeriesServiceStatisticsPaginator](./paginators.md#gettimeseriesservicestatisticspaginator)
3. item: [:material-code-braces: GetTimeSeriesServiceStatisticsResultTypeDef](./type_defs.md#gettimeseriesservicestatisticsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetTimeSeriesServiceStatisticsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    GroupName: str = ...,
    GroupARN: str = ...,
    EntitySelectorExpression: str = ...,
    Period: int = ...,
    ForecastStatistics: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetTimeSeriesServiceStatisticsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetTimeSeriesServiceStatisticsResultTypeDef](./type_defs.md#gettimeseriesservicestatisticsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetTimeSeriesServiceStatisticsRequestPaginateTypeDef = {  # (1)
    "StartTime": ...,
    "EndTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTimeSeriesServiceStatisticsRequestPaginateTypeDef](./type_defs.md#gettimeseriesservicestatisticsrequestpaginatetypedef) 
## GetTraceGraphPaginator

Type annotations and code completion for `#!python session.create_client("xray").get_paginator("get_trace_graph")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray/paginator/GetTraceGraph.html#XRay.Paginator.GetTraceGraph)

```python
# GetTraceGraphPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_xray.paginator import GetTraceGraphPaginator

session = get_session()
async with session.create_client("xray") as client:  # (1)
    paginator: GetTraceGraphPaginator = client.get_paginator("get_trace_graph")  # (2)
    async for item in paginator.paginate(...):
        item: GetTraceGraphResultTypeDef
        print(item)  # (3)
```

1. client: [XRayClient](./client.md)
2. paginator: [GetTraceGraphPaginator](./paginators.md#gettracegraphpaginator)
3. item: [:material-code-braces: GetTraceGraphResultTypeDef](./type_defs.md#gettracegraphresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetTraceGraphPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TraceIds: Sequence[str],
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetTraceGraphResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetTraceGraphResultTypeDef](./type_defs.md#gettracegraphresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetTraceGraphRequestPaginateTypeDef = {  # (1)
    "TraceIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTraceGraphRequestPaginateTypeDef](./type_defs.md#gettracegraphrequestpaginatetypedef) 
## GetTraceSummariesPaginator

Type annotations and code completion for `#!python session.create_client("xray").get_paginator("get_trace_summaries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray/paginator/GetTraceSummaries.html#XRay.Paginator.GetTraceSummaries)

```python
# GetTraceSummariesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_xray.paginator import GetTraceSummariesPaginator

session = get_session()
async with session.create_client("xray") as client:  # (1)
    paginator: GetTraceSummariesPaginator = client.get_paginator("get_trace_summaries")  # (2)
    async for item in paginator.paginate(...):
        item: GetTraceSummariesResultTypeDef
        print(item)  # (3)
```

1. client: [XRayClient](./client.md)
2. paginator: [GetTraceSummariesPaginator](./paginators.md#gettracesummariespaginator)
3. item: [:material-code-braces: GetTraceSummariesResultTypeDef](./type_defs.md#gettracesummariesresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetTraceSummariesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    TimeRangeType: TimeRangeTypeType = ...,  # (1)
    Sampling: bool = ...,
    SamplingStrategy: SamplingStrategyTypeDef = ...,  # (2)
    FilterExpression: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[GetTraceSummariesResultTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: TimeRangeTypeType](./literals.md#timerangetypetype) 
2. See [:material-code-braces: SamplingStrategyTypeDef](./type_defs.md#samplingstrategytypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: GetTraceSummariesResultTypeDef](./type_defs.md#gettracesummariesresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetTraceSummariesRequestPaginateTypeDef = {  # (1)
    "StartTime": ...,
    "EndTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTraceSummariesRequestPaginateTypeDef](./type_defs.md#gettracesummariesrequestpaginatetypedef) 
## ListResourcePoliciesPaginator

Type annotations and code completion for `#!python session.create_client("xray").get_paginator("list_resource_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray/paginator/ListResourcePolicies.html#XRay.Paginator.ListResourcePolicies)

```python
# ListResourcePoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_xray.paginator import ListResourcePoliciesPaginator

session = get_session()
async with session.create_client("xray") as client:  # (1)
    paginator: ListResourcePoliciesPaginator = client.get_paginator("list_resource_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourcePoliciesResultTypeDef
        print(item)  # (3)
```

1. client: [XRayClient](./client.md)
2. paginator: [ListResourcePoliciesPaginator](./paginators.md#listresourcepoliciespaginator)
3. item: [:material-code-braces: ListResourcePoliciesResultTypeDef](./type_defs.md#listresourcepoliciesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListResourcePoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListResourcePoliciesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResourcePoliciesResultTypeDef](./type_defs.md#listresourcepoliciesresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResourcePoliciesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourcePoliciesRequestPaginateTypeDef](./type_defs.md#listresourcepoliciesrequestpaginatetypedef) 
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("xray").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray/paginator/ListTagsForResource.html#XRay.Paginator.ListTagsForResource)

```python
# ListTagsForResourcePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_xray.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("xray") as client:  # (1)
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsForResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [XRayClient](./client.md)
2. paginator: [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
3. item: [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceARN: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTagsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTagsForResourceRequestPaginateTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestPaginateTypeDef](./type_defs.md#listtagsforresourcerequestpaginatetypedef) 
