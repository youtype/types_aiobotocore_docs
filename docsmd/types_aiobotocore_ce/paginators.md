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
## GetReservationPurchaseRecommendationPaginator

Type annotations and code completion for `#!python session.create_client("ce").get_paginator("get_reservation_purchase_recommendation")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/paginator/GetReservationPurchaseRecommendation.html#CostExplorer.Paginator.GetReservationPurchaseRecommendation)

```python
# GetReservationPurchaseRecommendationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ce.paginator import GetReservationPurchaseRecommendationPaginator

session = get_session()
async with session.create_client("ce") as client:  # (1)
    paginator: GetReservationPurchaseRecommendationPaginator = client.get_paginator("get_reservation_purchase_recommendation")  # (2)
    async for item in paginator.paginate(...):
        item: GetReservationPurchaseRecommendationResponseTypeDef
        print(item)  # (3)
```

1. client: [CostExplorerClient](./client.md)
2. paginator: [GetReservationPurchaseRecommendationPaginator](./paginators.md#getreservationpurchaserecommendationpaginator)
3. item: `AioPageIterator[GetReservationPurchaseRecommendationResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetReservationPurchaseRecommendationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Service: str,
    AccountId: str = ...,
    Filter: ExpressionPaginatorUnionTypeDef = ...,  # (1)
    AccountScope: AccountScopeType = ...,  # (2)
    LookbackPeriodInDays: LookbackPeriodInDaysType = ...,  # (3)
    TermInYears: TermInYearsType = ...,  # (4)
    PaymentOption: PaymentOptionType = ...,  # (5)
    ServiceSpecification: ServiceSpecificationTypeDef = ...,  # (6)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (7)
) -> aiobotocore.paginate.AioPageIterator[GetReservationPurchaseRecommendationResponseTypeDef]:  # (8)
    ...
```

1. See [:material-code-braces: ExpressionPaginatorUnionTypeDef](#expressionpaginatoruniontypedef)
2. See [:material-code-brackets: AccountScopeType](./literals.md#accountscopetype)
3. See [:material-code-brackets: LookbackPeriodInDaysType](./literals.md#lookbackperiodindaystype)
4. See [:material-code-brackets: TermInYearsType](./literals.md#terminyearstype)
5. See [:material-code-brackets: PaymentOptionType](./literals.md#paymentoptiontype)
6. See [:material-code-braces: ServiceSpecificationTypeDef](./type_defs.md#servicespecificationtypedef)
7. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
8. See `AioPageIterator[GetReservationPurchaseRecommendationResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetReservationPurchaseRecommendationRequestPaginateTypeDef = {  # (1)
    "Service": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetReservationPurchaseRecommendationRequestPaginateTypeDef](./type_defs.md#getreservationpurchaserecommendationrequestpaginatetypedef)
## GetRightsizingRecommendationPaginator

Type annotations and code completion for `#!python session.create_client("ce").get_paginator("get_rightsizing_recommendation")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/paginator/GetRightsizingRecommendation.html#CostExplorer.Paginator.GetRightsizingRecommendation)

```python
# GetRightsizingRecommendationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ce.paginator import GetRightsizingRecommendationPaginator

session = get_session()
async with session.create_client("ce") as client:  # (1)
    paginator: GetRightsizingRecommendationPaginator = client.get_paginator("get_rightsizing_recommendation")  # (2)
    async for item in paginator.paginate(...):
        item: GetRightsizingRecommendationResponseTypeDef
        print(item)  # (3)
```

1. client: [CostExplorerClient](./client.md)
2. paginator: [GetRightsizingRecommendationPaginator](./paginators.md#getrightsizingrecommendationpaginator)
3. item: `AioPageIterator[GetRightsizingRecommendationResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetRightsizingRecommendationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Service: str,
    Filter: ExpressionPaginatorUnionTypeDef = ...,  # (1)
    Configuration: RightsizingRecommendationConfigurationTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[GetRightsizingRecommendationResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: ExpressionPaginatorUnionTypeDef](#expressionpaginatoruniontypedef)
2. See [:material-code-braces: RightsizingRecommendationConfigurationTypeDef](./type_defs.md#rightsizingrecommendationconfigurationtypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[GetRightsizingRecommendationResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetRightsizingRecommendationRequestPaginateTypeDef = {  # (1)
    "Service": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRightsizingRecommendationRequestPaginateTypeDef](./type_defs.md#getrightsizingrecommendationrequestpaginatetypedef)
## ListCommitmentPurchaseAnalysesPaginator

Type annotations and code completion for `#!python session.create_client("ce").get_paginator("list_commitment_purchase_analyses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/paginator/ListCommitmentPurchaseAnalyses.html#CostExplorer.Paginator.ListCommitmentPurchaseAnalyses)

```python
# ListCommitmentPurchaseAnalysesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ce.paginator import ListCommitmentPurchaseAnalysesPaginator

session = get_session()
async with session.create_client("ce") as client:  # (1)
    paginator: ListCommitmentPurchaseAnalysesPaginator = client.get_paginator("list_commitment_purchase_analyses")  # (2)
    async for item in paginator.paginate(...):
        item: ListCommitmentPurchaseAnalysesResponseTypeDef
        print(item)  # (3)
```

1. client: [CostExplorerClient](./client.md)
2. paginator: [ListCommitmentPurchaseAnalysesPaginator](./paginators.md#listcommitmentpurchaseanalysespaginator)
3. item: `AioPageIterator[ListCommitmentPurchaseAnalysesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCommitmentPurchaseAnalysesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AnalysisStatus: AnalysisStatusType = ...,  # (1)
    AnalysisIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListCommitmentPurchaseAnalysesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AnalysisStatusType](./literals.md#analysisstatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListCommitmentPurchaseAnalysesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCommitmentPurchaseAnalysesRequestPaginateTypeDef = {  # (1)
    "AnalysisStatus": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCommitmentPurchaseAnalysesRequestPaginateTypeDef](./type_defs.md#listcommitmentpurchaseanalysesrequestpaginatetypedef)
## ListCostAllocationTagBackfillHistoryPaginator

Type annotations and code completion for `#!python session.create_client("ce").get_paginator("list_cost_allocation_tag_backfill_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/paginator/ListCostAllocationTagBackfillHistory.html#CostExplorer.Paginator.ListCostAllocationTagBackfillHistory)

```python
# ListCostAllocationTagBackfillHistoryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ce.paginator import ListCostAllocationTagBackfillHistoryPaginator

session = get_session()
async with session.create_client("ce") as client:  # (1)
    paginator: ListCostAllocationTagBackfillHistoryPaginator = client.get_paginator("list_cost_allocation_tag_backfill_history")  # (2)
    async for item in paginator.paginate(...):
        item: ListCostAllocationTagBackfillHistoryResponseTypeDef
        print(item)  # (3)
```

1. client: [CostExplorerClient](./client.md)
2. paginator: [ListCostAllocationTagBackfillHistoryPaginator](./paginators.md#listcostallocationtagbackfillhistorypaginator)
3. item: `AioPageIterator[ListCostAllocationTagBackfillHistoryResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCostAllocationTagBackfillHistoryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCostAllocationTagBackfillHistoryResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCostAllocationTagBackfillHistoryResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCostAllocationTagBackfillHistoryRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCostAllocationTagBackfillHistoryRequestPaginateTypeDef](./type_defs.md#listcostallocationtagbackfillhistoryrequestpaginatetypedef)
## ListCostAllocationTagsPaginator

Type annotations and code completion for `#!python session.create_client("ce").get_paginator("list_cost_allocation_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/paginator/ListCostAllocationTags.html#CostExplorer.Paginator.ListCostAllocationTags)

```python
# ListCostAllocationTagsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ce.paginator import ListCostAllocationTagsPaginator

session = get_session()
async with session.create_client("ce") as client:  # (1)
    paginator: ListCostAllocationTagsPaginator = client.get_paginator("list_cost_allocation_tags")  # (2)
    async for item in paginator.paginate(...):
        item: ListCostAllocationTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [CostExplorerClient](./client.md)
2. paginator: [ListCostAllocationTagsPaginator](./paginators.md#listcostallocationtagspaginator)
3. item: `AioPageIterator[ListCostAllocationTagsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCostAllocationTagsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Status: CostAllocationTagStatusType = ...,  # (1)
    TagKeys: Sequence[str] = ...,
    Type: CostAllocationTagTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListCostAllocationTagsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: CostAllocationTagStatusType](./literals.md#costallocationtagstatustype)
2. See [:material-code-brackets: CostAllocationTagTypeType](./literals.md#costallocationtagtypetype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListCostAllocationTagsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCostAllocationTagsRequestPaginateTypeDef = {  # (1)
    "Status": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCostAllocationTagsRequestPaginateTypeDef](./type_defs.md#listcostallocationtagsrequestpaginatetypedef)
## ListCostCategoryDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("ce").get_paginator("list_cost_category_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/paginator/ListCostCategoryDefinitions.html#CostExplorer.Paginator.ListCostCategoryDefinitions)

```python
# ListCostCategoryDefinitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ce.paginator import ListCostCategoryDefinitionsPaginator

session = get_session()
async with session.create_client("ce") as client:  # (1)
    paginator: ListCostCategoryDefinitionsPaginator = client.get_paginator("list_cost_category_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListCostCategoryDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [CostExplorerClient](./client.md)
2. paginator: [ListCostCategoryDefinitionsPaginator](./paginators.md#listcostcategorydefinitionspaginator)
3. item: `AioPageIterator[ListCostCategoryDefinitionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCostCategoryDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    EffectiveOn: str = ...,
    SupportedResourceTypes: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCostCategoryDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCostCategoryDefinitionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCostCategoryDefinitionsRequestPaginateTypeDef = {  # (1)
    "EffectiveOn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCostCategoryDefinitionsRequestPaginateTypeDef](./type_defs.md#listcostcategorydefinitionsrequestpaginatetypedef)
## ListCostCategoryResourceAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("ce").get_paginator("list_cost_category_resource_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/paginator/ListCostCategoryResourceAssociations.html#CostExplorer.Paginator.ListCostCategoryResourceAssociations)

```python
# ListCostCategoryResourceAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ce.paginator import ListCostCategoryResourceAssociationsPaginator

session = get_session()
async with session.create_client("ce") as client:  # (1)
    paginator: ListCostCategoryResourceAssociationsPaginator = client.get_paginator("list_cost_category_resource_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListCostCategoryResourceAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [CostExplorerClient](./client.md)
2. paginator: [ListCostCategoryResourceAssociationsPaginator](./paginators.md#listcostcategoryresourceassociationspaginator)
3. item: `AioPageIterator[ListCostCategoryResourceAssociationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCostCategoryResourceAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CostCategoryArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCostCategoryResourceAssociationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCostCategoryResourceAssociationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCostCategoryResourceAssociationsRequestPaginateTypeDef = {  # (1)
    "CostCategoryArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCostCategoryResourceAssociationsRequestPaginateTypeDef](./type_defs.md#listcostcategoryresourceassociationsrequestpaginatetypedef)
## ListSavingsPlansPurchaseRecommendationGenerationPaginator

Type annotations and code completion for `#!python session.create_client("ce").get_paginator("list_savings_plans_purchase_recommendation_generation")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/paginator/ListSavingsPlansPurchaseRecommendationGeneration.html#CostExplorer.Paginator.ListSavingsPlansPurchaseRecommendationGeneration)

```python
# ListSavingsPlansPurchaseRecommendationGenerationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ce.paginator import ListSavingsPlansPurchaseRecommendationGenerationPaginator

session = get_session()
async with session.create_client("ce") as client:  # (1)
    paginator: ListSavingsPlansPurchaseRecommendationGenerationPaginator = client.get_paginator("list_savings_plans_purchase_recommendation_generation")  # (2)
    async for item in paginator.paginate(...):
        item: ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef
        print(item)  # (3)
```

1. client: [CostExplorerClient](./client.md)
2. paginator: [ListSavingsPlansPurchaseRecommendationGenerationPaginator](./paginators.md#listsavingsplanspurchaserecommendationgenerationpaginator)
3. item: `AioPageIterator[ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSavingsPlansPurchaseRecommendationGenerationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GenerationStatus: GenerationStatusType = ...,  # (1)
    RecommendationIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: GenerationStatusType](./literals.md#generationstatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSavingsPlansPurchaseRecommendationGenerationRequestPaginateTypeDef = {  # (1)
    "GenerationStatus": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSavingsPlansPurchaseRecommendationGenerationRequestPaginateTypeDef](./type_defs.md#listsavingsplanspurchaserecommendationgenerationrequestpaginatetypedef)
