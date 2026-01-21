# Paginators

> [Index](../README.md) > [CostOptimizationHub](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CostOptimizationHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#costoptimizationhub)
    type annotations stubs module [types-aiobotocore-cost-optimization-hub](https://pypi.org/project/types-aiobotocore-cost-optimization-hub/).

## ListEfficiencyMetricsPaginator

Type annotations and code completion for `#!python session.create_client("cost-optimization-hub").get_paginator("list_efficiency_metrics")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub/paginator/ListEfficiencyMetrics.html#CostOptimizationHub.Paginator.ListEfficiencyMetrics)

```python
# ListEfficiencyMetricsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cost_optimization_hub.paginator import ListEfficiencyMetricsPaginator

session = get_session()
async with session.create_client("cost-optimization-hub") as client:  # (1)
    paginator: ListEfficiencyMetricsPaginator = client.get_paginator("list_efficiency_metrics")  # (2)
    async for item in paginator.paginate(...):
        item: ListEfficiencyMetricsResponseTypeDef
        print(item)  # (3)
```

1. client: [CostOptimizationHubClient](./client.md)
2. paginator: [ListEfficiencyMetricsPaginator](./paginators.md#listefficiencymetricspaginator)
3. item: `AioPageIterator[ListEfficiencyMetricsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListEfficiencyMetricsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    granularity: GranularityTypeType,  # (1)
    timePeriod: TimePeriodTypeDef,  # (2)
    groupBy: str = ...,
    orderBy: OrderByTypeDef = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[ListEfficiencyMetricsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: GranularityTypeType](./literals.md#granularitytypetype)
2. See [:material-code-braces: TimePeriodTypeDef](./type_defs.md#timeperiodtypedef)
3. See [:material-code-braces: OrderByTypeDef](./type_defs.md#orderbytypedef)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[ListEfficiencyMetricsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListEfficiencyMetricsRequestPaginateTypeDef = {  # (1)
    "granularity": ...,
    "timePeriod": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEfficiencyMetricsRequestPaginateTypeDef](./type_defs.md#listefficiencymetricsrequestpaginatetypedef)
## ListEnrollmentStatusesPaginator

Type annotations and code completion for `#!python session.create_client("cost-optimization-hub").get_paginator("list_enrollment_statuses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub/paginator/ListEnrollmentStatuses.html#CostOptimizationHub.Paginator.ListEnrollmentStatuses)

```python
# ListEnrollmentStatusesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cost_optimization_hub.paginator import ListEnrollmentStatusesPaginator

session = get_session()
async with session.create_client("cost-optimization-hub") as client:  # (1)
    paginator: ListEnrollmentStatusesPaginator = client.get_paginator("list_enrollment_statuses")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnrollmentStatusesResponseTypeDef
        print(item)  # (3)
```

1. client: [CostOptimizationHubClient](./client.md)
2. paginator: [ListEnrollmentStatusesPaginator](./paginators.md#listenrollmentstatusespaginator)
3. item: `AioPageIterator[ListEnrollmentStatusesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListEnrollmentStatusesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    includeOrganizationInfo: bool = ...,
    accountId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListEnrollmentStatusesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListEnrollmentStatusesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListEnrollmentStatusesRequestPaginateTypeDef = {  # (1)
    "includeOrganizationInfo": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnrollmentStatusesRequestPaginateTypeDef](./type_defs.md#listenrollmentstatusesrequestpaginatetypedef)
## ListRecommendationSummariesPaginator

Type annotations and code completion for `#!python session.create_client("cost-optimization-hub").get_paginator("list_recommendation_summaries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub/paginator/ListRecommendationSummaries.html#CostOptimizationHub.Paginator.ListRecommendationSummaries)

```python
# ListRecommendationSummariesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cost_optimization_hub.paginator import ListRecommendationSummariesPaginator

session = get_session()
async with session.create_client("cost-optimization-hub") as client:  # (1)
    paginator: ListRecommendationSummariesPaginator = client.get_paginator("list_recommendation_summaries")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecommendationSummariesResponseTypeDef
        print(item)  # (3)
```

1. client: [CostOptimizationHubClient](./client.md)
2. paginator: [ListRecommendationSummariesPaginator](./paginators.md#listrecommendationsummariespaginator)
3. item: `AioPageIterator[ListRecommendationSummariesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRecommendationSummariesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    groupBy: str,
    filter: FilterTypeDef = ...,  # (1)
    metrics: Sequence[SummaryMetricsType] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListRecommendationSummariesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef)
2. See `Sequence[Literal['SavingsPercentage']]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListRecommendationSummariesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRecommendationSummariesRequestPaginateTypeDef = {  # (1)
    "groupBy": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecommendationSummariesRequestPaginateTypeDef](./type_defs.md#listrecommendationsummariesrequestpaginatetypedef)
## ListRecommendationsPaginator

Type annotations and code completion for `#!python session.create_client("cost-optimization-hub").get_paginator("list_recommendations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub/paginator/ListRecommendations.html#CostOptimizationHub.Paginator.ListRecommendations)

```python
# ListRecommendationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cost_optimization_hub.paginator import ListRecommendationsPaginator

session = get_session()
async with session.create_client("cost-optimization-hub") as client:  # (1)
    paginator: ListRecommendationsPaginator = client.get_paginator("list_recommendations")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecommendationsResponseTypeDef
        print(item)  # (3)
```

1. client: [CostOptimizationHubClient](./client.md)
2. paginator: [ListRecommendationsPaginator](./paginators.md#listrecommendationspaginator)
3. item: `AioPageIterator[ListRecommendationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRecommendationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filter: FilterTypeDef = ...,  # (1)
    orderBy: OrderByTypeDef = ...,  # (2)
    includeAllRecommendations: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListRecommendationsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef)
2. See [:material-code-braces: OrderByTypeDef](./type_defs.md#orderbytypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListRecommendationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRecommendationsRequestPaginateTypeDef = {  # (1)
    "filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecommendationsRequestPaginateTypeDef](./type_defs.md#listrecommendationsrequestpaginatetypedef)
