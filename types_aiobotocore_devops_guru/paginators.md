<a id="paginators-for-aiobotocore-devopsguru-module"></a>

# Paginators for aiobotocore DevOpsGuru module

> [Index](..) > [DevOpsGuru](.) > Paginators

Auto-generated documentation for
[DevOpsGuru](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
type annotations stubs module
[types-aiobotocore-devops-guru](https://pypi.org/project/types-aiobotocore-devops-guru/).

- [Paginators for aiobotocore DevOpsGuru module](#paginators-for-aiobotocore-devopsguru-module)
  - [DescribeOrganizationResourceCollectionHealthPaginator](#describeorganizationresourcecollectionhealthpaginator)
  - [DescribeResourceCollectionHealthPaginator](#describeresourcecollectionhealthpaginator)
  - [GetCostEstimationPaginator](#getcostestimationpaginator)
  - [GetResourceCollectionPaginator](#getresourcecollectionpaginator)
  - [ListAnomaliesForInsightPaginator](#listanomaliesforinsightpaginator)
  - [ListEventsPaginator](#listeventspaginator)
  - [ListInsightsPaginator](#listinsightspaginator)
  - [ListNotificationChannelsPaginator](#listnotificationchannelspaginator)
  - [ListOrganizationInsightsPaginator](#listorganizationinsightspaginator)
  - [ListRecommendationsPaginator](#listrecommendationspaginator)
  - [SearchInsightsPaginator](#searchinsightspaginator)
  - [SearchOrganizationInsightsPaginator](#searchorganizationinsightspaginator)

<a id="describeorganizationresourcecollectionhealthpaginator"></a>

## DescribeOrganizationResourceCollectionHealthPaginator

Type annotations for
`session.create_client("devops-guru").get_paginator("describe_organization_resource_collection_health")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import DescribeOrganizationResourceCollectionHealthPaginator

session = get_session()
async with session.create_client("devops-guru") as client:
    client: DevOpsGuruClient
    paginator: DescribeOrganizationResourceCollectionHealthPaginator = client.get_paginator("describe_organization_resource_collection_health")
```

Boto3 documentation:
[DevOpsGuru.Paginator.DescribeOrganizationResourceCollectionHealth](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeOrganizationResourceCollectionHealth)

Arguments for `DescribeOrganizationResourceCollectionHealthPaginator.paginate`
method:

- `OrganizationResourceCollectionType`:
  [OrganizationResourceCollectionTypeType](./literals.md#organizationresourcecollectiontypetype)
  *(required)*
- `AccountIds`: `Sequence`\[`str`\]
- `OrganizationalUnitIds`: `Sequence`\[`str`\]
- `MaxResults`: `int`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeOrganizationResourceCollectionHealthPaginator.paginate` returns
`AsyncIterable`\[[DescribeOrganizationResourceCollectionHealthResponseTypeDef](./type_defs.md#describeorganizationresourcecollectionhealthresponsetypedef)\].

<a id="describeresourcecollectionhealthpaginator"></a>

## DescribeResourceCollectionHealthPaginator

Type annotations for
`session.create_client("devops-guru").get_paginator("describe_resource_collection_health")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import DescribeResourceCollectionHealthPaginator

session = get_session()
async with session.create_client("devops-guru") as client:
    client: DevOpsGuruClient
    paginator: DescribeResourceCollectionHealthPaginator = client.get_paginator("describe_resource_collection_health")
```

Boto3 documentation:
[DevOpsGuru.Paginator.DescribeResourceCollectionHealth](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeResourceCollectionHealth)

Arguments for `DescribeResourceCollectionHealthPaginator.paginate` method:

- `ResourceCollectionType`:
  [ResourceCollectionTypeType](./literals.md#resourcecollectiontypetype)
  *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeResourceCollectionHealthPaginator.paginate` returns
`AsyncIterable`\[[DescribeResourceCollectionHealthResponseTypeDef](./type_defs.md#describeresourcecollectionhealthresponsetypedef)\].

<a id="getcostestimationpaginator"></a>

## GetCostEstimationPaginator

Type annotations for
`session.create_client("devops-guru").get_paginator("get_cost_estimation")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import GetCostEstimationPaginator

session = get_session()
async with session.create_client("devops-guru") as client:
    client: DevOpsGuruClient
    paginator: GetCostEstimationPaginator = client.get_paginator("get_cost_estimation")
```

Boto3 documentation:
[DevOpsGuru.Paginator.GetCostEstimation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetCostEstimation)

Arguments for `GetCostEstimationPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetCostEstimationPaginator.paginate` returns
`AsyncIterable`\[[GetCostEstimationResponseTypeDef](./type_defs.md#getcostestimationresponsetypedef)\].

<a id="getresourcecollectionpaginator"></a>

## GetResourceCollectionPaginator

Type annotations for
`session.create_client("devops-guru").get_paginator("get_resource_collection")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import GetResourceCollectionPaginator

session = get_session()
async with session.create_client("devops-guru") as client:
    client: DevOpsGuruClient
    paginator: GetResourceCollectionPaginator = client.get_paginator("get_resource_collection")
```

Boto3 documentation:
[DevOpsGuru.Paginator.GetResourceCollection](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetResourceCollection)

Arguments for `GetResourceCollectionPaginator.paginate` method:

- `ResourceCollectionType`:
  [ResourceCollectionTypeType](./literals.md#resourcecollectiontypetype)
  *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetResourceCollectionPaginator.paginate` returns
`AsyncIterable`\[[GetResourceCollectionResponseTypeDef](./type_defs.md#getresourcecollectionresponsetypedef)\].

<a id="listanomaliesforinsightpaginator"></a>

## ListAnomaliesForInsightPaginator

Type annotations for
`session.create_client("devops-guru").get_paginator("list_anomalies_for_insight")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import ListAnomaliesForInsightPaginator

session = get_session()
async with session.create_client("devops-guru") as client:
    client: DevOpsGuruClient
    paginator: ListAnomaliesForInsightPaginator = client.get_paginator("list_anomalies_for_insight")
```

Boto3 documentation:
[DevOpsGuru.Paginator.ListAnomaliesForInsight](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomaliesForInsight)

Arguments for `ListAnomaliesForInsightPaginator.paginate` method:

- `InsightId`: `str` *(required)*
- `StartTimeRange`:
  [StartTimeRangeTypeDef](./type_defs.md#starttimerangetypedef)
- `AccountId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAnomaliesForInsightPaginator.paginate` returns
`AsyncIterable`\[[ListAnomaliesForInsightResponseTypeDef](./type_defs.md#listanomaliesforinsightresponsetypedef)\].

<a id="listeventspaginator"></a>

## ListEventsPaginator

Type annotations for
`session.create_client("devops-guru").get_paginator("list_events")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import ListEventsPaginator

session = get_session()
async with session.create_client("devops-guru") as client:
    client: DevOpsGuruClient
    paginator: ListEventsPaginator = client.get_paginator("list_events")
```

Boto3 documentation:
[DevOpsGuru.Paginator.ListEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListEvents)

Arguments for `ListEventsPaginator.paginate` method:

- `Filters`:
  [ListEventsFiltersTypeDef](./type_defs.md#listeventsfilterstypedef)
  *(required)*
- `AccountId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListEventsPaginator.paginate` returns
`AsyncIterable`\[[ListEventsResponseTypeDef](./type_defs.md#listeventsresponsetypedef)\].

<a id="listinsightspaginator"></a>

## ListInsightsPaginator

Type annotations for
`session.create_client("devops-guru").get_paginator("list_insights")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import ListInsightsPaginator

session = get_session()
async with session.create_client("devops-guru") as client:
    client: DevOpsGuruClient
    paginator: ListInsightsPaginator = client.get_paginator("list_insights")
```

Boto3 documentation:
[DevOpsGuru.Paginator.ListInsights](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListInsights)

Arguments for `ListInsightsPaginator.paginate` method:

- `StatusFilter`:
  [ListInsightsStatusFilterTypeDef](./type_defs.md#listinsightsstatusfiltertypedef)
  *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListInsightsPaginator.paginate` returns
`AsyncIterable`\[[ListInsightsResponseTypeDef](./type_defs.md#listinsightsresponsetypedef)\].

<a id="listnotificationchannelspaginator"></a>

## ListNotificationChannelsPaginator

Type annotations for
`session.create_client("devops-guru").get_paginator("list_notification_channels")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import ListNotificationChannelsPaginator

session = get_session()
async with session.create_client("devops-guru") as client:
    client: DevOpsGuruClient
    paginator: ListNotificationChannelsPaginator = client.get_paginator("list_notification_channels")
```

Boto3 documentation:
[DevOpsGuru.Paginator.ListNotificationChannels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListNotificationChannels)

Arguments for `ListNotificationChannelsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListNotificationChannelsPaginator.paginate` returns
`AsyncIterable`\[[ListNotificationChannelsResponseTypeDef](./type_defs.md#listnotificationchannelsresponsetypedef)\].

<a id="listorganizationinsightspaginator"></a>

## ListOrganizationInsightsPaginator

Type annotations for
`session.create_client("devops-guru").get_paginator("list_organization_insights")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import ListOrganizationInsightsPaginator

session = get_session()
async with session.create_client("devops-guru") as client:
    client: DevOpsGuruClient
    paginator: ListOrganizationInsightsPaginator = client.get_paginator("list_organization_insights")
```

Boto3 documentation:
[DevOpsGuru.Paginator.ListOrganizationInsights](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListOrganizationInsights)

Arguments for `ListOrganizationInsightsPaginator.paginate` method:

- `StatusFilter`:
  [ListInsightsStatusFilterTypeDef](./type_defs.md#listinsightsstatusfiltertypedef)
  *(required)*
- `AccountIds`: `Sequence`\[`str`\]
- `OrganizationalUnitIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListOrganizationInsightsPaginator.paginate` returns
`AsyncIterable`\[[ListOrganizationInsightsResponseTypeDef](./type_defs.md#listorganizationinsightsresponsetypedef)\].

<a id="listrecommendationspaginator"></a>

## ListRecommendationsPaginator

Type annotations for
`session.create_client("devops-guru").get_paginator("list_recommendations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import ListRecommendationsPaginator

session = get_session()
async with session.create_client("devops-guru") as client:
    client: DevOpsGuruClient
    paginator: ListRecommendationsPaginator = client.get_paginator("list_recommendations")
```

Boto3 documentation:
[DevOpsGuru.Paginator.ListRecommendations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListRecommendations)

Arguments for `ListRecommendationsPaginator.paginate` method:

- `InsightId`: `str` *(required)*
- `Locale`: [LocaleType](./literals.md#localetype)
- `AccountId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRecommendationsPaginator.paginate` returns
`AsyncIterable`\[[ListRecommendationsResponseTypeDef](./type_defs.md#listrecommendationsresponsetypedef)\].

<a id="searchinsightspaginator"></a>

## SearchInsightsPaginator

Type annotations for
`session.create_client("devops-guru").get_paginator("search_insights")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import SearchInsightsPaginator

session = get_session()
async with session.create_client("devops-guru") as client:
    client: DevOpsGuruClient
    paginator: SearchInsightsPaginator = client.get_paginator("search_insights")
```

Boto3 documentation:
[DevOpsGuru.Paginator.SearchInsights](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchInsights)

Arguments for `SearchInsightsPaginator.paginate` method:

- `StartTimeRange`:
  [StartTimeRangeTypeDef](./type_defs.md#starttimerangetypedef) *(required)*
- `Type`: [InsightTypeType](./literals.md#insighttypetype) *(required)*
- `Filters`:
  [SearchInsightsFiltersTypeDef](./type_defs.md#searchinsightsfilterstypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`SearchInsightsPaginator.paginate` returns
`AsyncIterable`\[[SearchInsightsResponseTypeDef](./type_defs.md#searchinsightsresponsetypedef)\].

<a id="searchorganizationinsightspaginator"></a>

## SearchOrganizationInsightsPaginator

Type annotations for
`session.create_client("devops-guru").get_paginator("search_organization_insights")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import SearchOrganizationInsightsPaginator

session = get_session()
async with session.create_client("devops-guru") as client:
    client: DevOpsGuruClient
    paginator: SearchOrganizationInsightsPaginator = client.get_paginator("search_organization_insights")
```

Boto3 documentation:
[DevOpsGuru.Paginator.SearchOrganizationInsights](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchOrganizationInsights)

Arguments for `SearchOrganizationInsightsPaginator.paginate` method:

- `AccountIds`: `Sequence`\[`str`\] *(required)*
- `StartTimeRange`:
  [StartTimeRangeTypeDef](./type_defs.md#starttimerangetypedef) *(required)*
- `Type`: [InsightTypeType](./literals.md#insighttypetype) *(required)*
- `Filters`:
  [SearchOrganizationInsightsFiltersTypeDef](./type_defs.md#searchorganizationinsightsfilterstypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`SearchOrganizationInsightsPaginator.paginate` returns
`AsyncIterable`\[[SearchOrganizationInsightsResponseTypeDef](./type_defs.md#searchorganizationinsightsresponsetypedef)\].
