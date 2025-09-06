# Paginators

> [Index](../README.md) > [CostExplorer](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CostExplorer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#costexplorer)
    type annotations stubs module [types-aiobotocore-ce](https://pypi.org/project/types-aiobotocore-ce/).

## GetAnomaliesPaginator

Type annotations and code completion for `#!python session.create_client("ce").get_paginator("get_anomalies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/paginator/GetAnomalies.html#CostExplorer.Paginator.GetAnomalies)

```python
# GetAnomaliesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ce.paginator import GetAnomaliesPaginator

session = get_session()
async with session.create_client("ce") as client:  # (1)
    paginator: GetAnomaliesPaginator = client.get_paginator("get_anomalies")  # (2)
    async for item in paginator.paginate(...):
        item: GetAnomaliesResponseTypeDef
        print(item)  # (3)
```

1. client: [CostExplorerClient](./client.md)
2. paginator: [GetAnomaliesPaginator](./paginators.md#getanomaliespaginator)
3. item: `AioPageIterator[GetAnomaliesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetAnomaliesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DateInterval: AnomalyDateIntervalTypeDef,  # (1)
    MonitorArn: str = ...,
    Feedback: AnomalyFeedbackTypeType = ...,  # (2)
    TotalImpact: TotalImpactFilterTypeDef = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[GetAnomaliesResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: AnomalyDateIntervalTypeDef](./type_defs.md#anomalydateintervaltypedef)
2. See [:material-code-brackets: AnomalyFeedbackTypeType](./literals.md#anomalyfeedbacktypetype)
3. See [:material-code-braces: TotalImpactFilterTypeDef](./type_defs.md#totalimpactfiltertypedef)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[GetAnomaliesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetAnomaliesRequestPaginateTypeDef = {  # (1)
    "DateInterval": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetAnomaliesRequestPaginateTypeDef](./type_defs.md#getanomaliesrequestpaginatetypedef)
## GetAnomalyMonitorsPaginator

Type annotations and code completion for `#!python session.create_client("ce").get_paginator("get_anomaly_monitors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/paginator/GetAnomalyMonitors.html#CostExplorer.Paginator.GetAnomalyMonitors)

```python
# GetAnomalyMonitorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ce.paginator import GetAnomalyMonitorsPaginator

session = get_session()
async with session.create_client("ce") as client:  # (1)
    paginator: GetAnomalyMonitorsPaginator = client.get_paginator("get_anomaly_monitors")  # (2)
    async for item in paginator.paginate(...):
        item: GetAnomalyMonitorsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [CostExplorerClient](./client.md)
2. paginator: [GetAnomalyMonitorsPaginator](./paginators.md#getanomalymonitorspaginator)
3. item: `AioPageIterator[GetAnomalyMonitorsResponsePaginatorTypeDef]`


### paginate

Type annotations and code completion for `#!python GetAnomalyMonitorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    MonitorArnList: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetAnomalyMonitorsResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetAnomalyMonitorsResponsePaginatorTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetAnomalyMonitorsRequestPaginateTypeDef = {  # (1)
    "MonitorArnList": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetAnomalyMonitorsRequestPaginateTypeDef](./type_defs.md#getanomalymonitorsrequestpaginatetypedef)
## GetAnomalySubscriptionsPaginator

Type annotations and code completion for `#!python session.create_client("ce").get_paginator("get_anomaly_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/paginator/GetAnomalySubscriptions.html#CostExplorer.Paginator.GetAnomalySubscriptions)

```python
# GetAnomalySubscriptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ce.paginator import GetAnomalySubscriptionsPaginator

session = get_session()
async with session.create_client("ce") as client:  # (1)
    paginator: GetAnomalySubscriptionsPaginator = client.get_paginator("get_anomaly_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        item: GetAnomalySubscriptionsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [CostExplorerClient](./client.md)
2. paginator: [GetAnomalySubscriptionsPaginator](./paginators.md#getanomalysubscriptionspaginator)
3. item: `AioPageIterator[GetAnomalySubscriptionsResponsePaginatorTypeDef]`


### paginate

Type annotations and code completion for `#!python GetAnomalySubscriptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SubscriptionArnList: Sequence[str] = ...,
    MonitorArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetAnomalySubscriptionsResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetAnomalySubscriptionsResponsePaginatorTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetAnomalySubscriptionsRequestPaginateTypeDef = {  # (1)
    "SubscriptionArnList": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetAnomalySubscriptionsRequestPaginateTypeDef](./type_defs.md#getanomalysubscriptionsrequestpaginatetypedef)
## GetCostAndUsageComparisonsPaginator

Type annotations and code completion for `#!python session.create_client("ce").get_paginator("get_cost_and_usage_comparisons")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/paginator/GetCostAndUsageComparisons.html#CostExplorer.Paginator.GetCostAndUsageComparisons)

```python
# GetCostAndUsageComparisonsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ce.paginator import GetCostAndUsageComparisonsPaginator

session = get_session()
async with session.create_client("ce") as client:  # (1)
    paginator: GetCostAndUsageComparisonsPaginator = client.get_paginator("get_cost_and_usage_comparisons")  # (2)
    async for item in paginator.paginate(...):
        item: GetCostAndUsageComparisonsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [CostExplorerClient](./client.md)
2. paginator: [GetCostAndUsageComparisonsPaginator](./paginators.md#getcostandusagecomparisonspaginator)
3. item: `AioPageIterator[GetCostAndUsageComparisonsResponsePaginatorTypeDef]`


### paginate

Type annotations and code completion for `#!python GetCostAndUsageComparisonsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    BaselineTimePeriod: DateIntervalTypeDef,  # (1)
    ComparisonTimePeriod: DateIntervalTypeDef,  # (1)
    MetricForComparison: str,
    BillingViewArn: str = ...,
    Filter: ExpressionPaginatorUnionTypeDef = ...,  # (3)
    GroupBy: Sequence[GroupDefinitionTypeDef] = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> aiobotocore.paginate.AioPageIterator[GetCostAndUsageComparisonsResponsePaginatorTypeDef]:  # (6)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef)
2. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef)
3. See [:material-code-braces: ExpressionPaginatorUnionTypeDef](#expressionpaginatoruniontypedef)
4. See `Sequence[GroupDefinitionTypeDef]`
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
6. See `AioPageIterator[GetCostAndUsageComparisonsResponsePaginatorTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetCostAndUsageComparisonsRequestPaginateTypeDef = {  # (1)
    "BaselineTimePeriod": ...,
    "ComparisonTimePeriod": ...,
    "MetricForComparison": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetCostAndUsageComparisonsRequestPaginateTypeDef](./type_defs.md#getcostandusagecomparisonsrequestpaginatetypedef)
## GetCostComparisonDriversPaginator

Type annotations and code completion for `#!python session.create_client("ce").get_paginator("get_cost_comparison_drivers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/paginator/GetCostComparisonDrivers.html#CostExplorer.Paginator.GetCostComparisonDrivers)

```python
# GetCostComparisonDriversPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ce.paginator import GetCostComparisonDriversPaginator

session = get_session()
async with session.create_client("ce") as client:  # (1)
    paginator: GetCostComparisonDriversPaginator = client.get_paginator("get_cost_comparison_drivers")  # (2)
    async for item in paginator.paginate(...):
        item: GetCostComparisonDriversResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [CostExplorerClient](./client.md)
2. paginator: [GetCostComparisonDriversPaginator](./paginators.md#getcostcomparisondriverspaginator)
3. item: `AioPageIterator[GetCostComparisonDriversResponsePaginatorTypeDef]`


### paginate

Type annotations and code completion for `#!python GetCostComparisonDriversPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    BaselineTimePeriod: DateIntervalTypeDef,  # (1)
    ComparisonTimePeriod: DateIntervalTypeDef,  # (1)
    MetricForComparison: str,
    BillingViewArn: str = ...,
    Filter: ExpressionPaginatorUnionTypeDef = ...,  # (3)
    GroupBy: Sequence[GroupDefinitionTypeDef] = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> aiobotocore.paginate.AioPageIterator[GetCostComparisonDriversResponsePaginatorTypeDef]:  # (6)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef)
2. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef)
3. See [:material-code-braces: ExpressionPaginatorUnionTypeDef](#expressionpaginatoruniontypedef)
4. See `Sequence[GroupDefinitionTypeDef]`
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
6. See `AioPageIterator[GetCostComparisonDriversResponsePaginatorTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetCostComparisonDriversRequestPaginateTypeDef = {  # (1)
    "BaselineTimePeriod": ...,
    "ComparisonTimePeriod": ...,
    "MetricForComparison": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetCostComparisonDriversRequestPaginateTypeDef](./type_defs.md#getcostcomparisondriversrequestpaginatetypedef)
