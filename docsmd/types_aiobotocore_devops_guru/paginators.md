# Paginators

> [Index](../README.md) > [DevOpsGuru](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [DevOpsGuru](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
    type annotations stubs module [types-aiobotocore-devops-guru](https://pypi.org/project/types-aiobotocore-devops-guru/).

## DescribeOrganizationResourceCollectionHealthPaginator

Type annotations and code completion for `#!python session.create_client("devops-guru").get_paginator("describe_organization_resource_collection_health")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeOrganizationResourceCollectionHealth)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import DescribeOrganizationResourceCollectionHealthPaginator

session = get_session()
async with session.create_client("devops-guru") as client:  # (1)
    paginator: DescribeOrganizationResourceCollectionHealthPaginator = client.get_paginator("describe_organization_resource_collection_health")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeOrganizationResourceCollectionHealthResponseTypeDef
        print(item)  # (3)
```

1. client: [DevOpsGuruClient](./client.md)
2. paginator: [DescribeOrganizationResourceCollectionHealthPaginator](./paginators.md#describeorganizationresourcecollectionhealthpaginator)
3. item: [:material-code-braces: DescribeOrganizationResourceCollectionHealthResponseTypeDef](./type_defs.md#describeorganizationresourcecollectionhealthresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeOrganizationResourceCollectionHealthPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    OrganizationResourceCollectionType: OrganizationResourceCollectionTypeType,  # (1)
    AccountIds: Sequence[str] = ...,
    OrganizationalUnitIds: Sequence[str] = ...,
    MaxResults: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeOrganizationResourceCollectionHealthResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: OrganizationResourceCollectionTypeType](./literals.md#organizationresourcecollectiontypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeOrganizationResourceCollectionHealthResponseTypeDef](./type_defs.md#describeorganizationresourcecollectionhealthresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = {  # (1)
    "OrganizationResourceCollectionType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef](./type_defs.md#describeorganizationresourcecollectionhealthrequestdescribeorganizationresourcecollectionhealthpaginatetypedef) 
## DescribeResourceCollectionHealthPaginator

Type annotations and code completion for `#!python session.create_client("devops-guru").get_paginator("describe_resource_collection_health")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeResourceCollectionHealth)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import DescribeResourceCollectionHealthPaginator

session = get_session()
async with session.create_client("devops-guru") as client:  # (1)
    paginator: DescribeResourceCollectionHealthPaginator = client.get_paginator("describe_resource_collection_health")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeResourceCollectionHealthResponseTypeDef
        print(item)  # (3)
```

1. client: [DevOpsGuruClient](./client.md)
2. paginator: [DescribeResourceCollectionHealthPaginator](./paginators.md#describeresourcecollectionhealthpaginator)
3. item: [:material-code-braces: DescribeResourceCollectionHealthResponseTypeDef](./type_defs.md#describeresourcecollectionhealthresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeResourceCollectionHealthPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceCollectionType: ResourceCollectionTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeResourceCollectionHealthResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceCollectionTypeType](./literals.md#resourcecollectiontypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeResourceCollectionHealthResponseTypeDef](./type_defs.md#describeresourcecollectionhealthresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = {  # (1)
    "ResourceCollectionType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef](./type_defs.md#describeresourcecollectionhealthrequestdescriberesourcecollectionhealthpaginatetypedef) 
## GetCostEstimationPaginator

Type annotations and code completion for `#!python session.create_client("devops-guru").get_paginator("get_cost_estimation")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetCostEstimation)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import GetCostEstimationPaginator

session = get_session()
async with session.create_client("devops-guru") as client:  # (1)
    paginator: GetCostEstimationPaginator = client.get_paginator("get_cost_estimation")  # (2)
    async for item in paginator.paginate(...):
        item: GetCostEstimationResponseTypeDef
        print(item)  # (3)
```

1. client: [DevOpsGuruClient](./client.md)
2. paginator: [GetCostEstimationPaginator](./paginators.md#getcostestimationpaginator)
3. item: [:material-code-braces: GetCostEstimationResponseTypeDef](./type_defs.md#getcostestimationresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetCostEstimationPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetCostEstimationResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetCostEstimationResponseTypeDef](./type_defs.md#getcostestimationresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetCostEstimationRequestGetCostEstimationPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetCostEstimationRequestGetCostEstimationPaginateTypeDef](./type_defs.md#getcostestimationrequestgetcostestimationpaginatetypedef) 
## GetResourceCollectionPaginator

Type annotations and code completion for `#!python session.create_client("devops-guru").get_paginator("get_resource_collection")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetResourceCollection)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import GetResourceCollectionPaginator

session = get_session()
async with session.create_client("devops-guru") as client:  # (1)
    paginator: GetResourceCollectionPaginator = client.get_paginator("get_resource_collection")  # (2)
    async for item in paginator.paginate(...):
        item: GetResourceCollectionResponseTypeDef
        print(item)  # (3)
```

1. client: [DevOpsGuruClient](./client.md)
2. paginator: [GetResourceCollectionPaginator](./paginators.md#getresourcecollectionpaginator)
3. item: [:material-code-braces: GetResourceCollectionResponseTypeDef](./type_defs.md#getresourcecollectionresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetResourceCollectionPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceCollectionType: ResourceCollectionTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetResourceCollectionResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceCollectionTypeType](./literals.md#resourcecollectiontypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetResourceCollectionResponseTypeDef](./type_defs.md#getresourcecollectionresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = {  # (1)
    "ResourceCollectionType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef](./type_defs.md#getresourcecollectionrequestgetresourcecollectionpaginatetypedef) 
## ListAnomaliesForInsightPaginator

Type annotations and code completion for `#!python session.create_client("devops-guru").get_paginator("list_anomalies_for_insight")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomaliesForInsight)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import ListAnomaliesForInsightPaginator

session = get_session()
async with session.create_client("devops-guru") as client:  # (1)
    paginator: ListAnomaliesForInsightPaginator = client.get_paginator("list_anomalies_for_insight")  # (2)
    async for item in paginator.paginate(...):
        item: ListAnomaliesForInsightResponseTypeDef
        print(item)  # (3)
```

1. client: [DevOpsGuruClient](./client.md)
2. paginator: [ListAnomaliesForInsightPaginator](./paginators.md#listanomaliesforinsightpaginator)
3. item: [:material-code-braces: ListAnomaliesForInsightResponseTypeDef](./type_defs.md#listanomaliesforinsightresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAnomaliesForInsightPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InsightId: str,
    StartTimeRange: StartTimeRangeTypeDef = ...,  # (1)
    AccountId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAnomaliesForInsightResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: StartTimeRangeTypeDef](./type_defs.md#starttimerangetypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAnomaliesForInsightResponseTypeDef](./type_defs.md#listanomaliesforinsightresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef = {  # (1)
    "InsightId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef](./type_defs.md#listanomaliesforinsightrequestlistanomaliesforinsightpaginatetypedef) 
## ListAnomalousLogGroupsPaginator

Type annotations and code completion for `#!python session.create_client("devops-guru").get_paginator("list_anomalous_log_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomalousLogGroups)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import ListAnomalousLogGroupsPaginator

session = get_session()
async with session.create_client("devops-guru") as client:  # (1)
    paginator: ListAnomalousLogGroupsPaginator = client.get_paginator("list_anomalous_log_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListAnomalousLogGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [DevOpsGuruClient](./client.md)
2. paginator: [ListAnomalousLogGroupsPaginator](./paginators.md#listanomalousloggroupspaginator)
3. item: [:material-code-braces: ListAnomalousLogGroupsResponseTypeDef](./type_defs.md#listanomalousloggroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAnomalousLogGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InsightId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAnomalousLogGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAnomalousLogGroupsResponseTypeDef](./type_defs.md#listanomalousloggroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = {  # (1)
    "InsightId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef](./type_defs.md#listanomalousloggroupsrequestlistanomalousloggroupspaginatetypedef) 
## ListEventsPaginator

Type annotations and code completion for `#!python session.create_client("devops-guru").get_paginator("list_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListEvents)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import ListEventsPaginator

session = get_session()
async with session.create_client("devops-guru") as client:  # (1)
    paginator: ListEventsPaginator = client.get_paginator("list_events")  # (2)
    async for item in paginator.paginate(...):
        item: ListEventsResponseTypeDef
        print(item)  # (3)
```

1. client: [DevOpsGuruClient](./client.md)
2. paginator: [ListEventsPaginator](./paginators.md#listeventspaginator)
3. item: [:material-code-braces: ListEventsResponseTypeDef](./type_defs.md#listeventsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEventsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: ListEventsFiltersTypeDef,  # (1)
    AccountId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListEventsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ListEventsFiltersTypeDef](./type_defs.md#listeventsfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListEventsResponseTypeDef](./type_defs.md#listeventsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListEventsRequestListEventsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventsRequestListEventsPaginateTypeDef](./type_defs.md#listeventsrequestlisteventspaginatetypedef) 
## ListInsightsPaginator

Type annotations and code completion for `#!python session.create_client("devops-guru").get_paginator("list_insights")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListInsights)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import ListInsightsPaginator

session = get_session()
async with session.create_client("devops-guru") as client:  # (1)
    paginator: ListInsightsPaginator = client.get_paginator("list_insights")  # (2)
    async for item in paginator.paginate(...):
        item: ListInsightsResponseTypeDef
        print(item)  # (3)
```

1. client: [DevOpsGuruClient](./client.md)
2. paginator: [ListInsightsPaginator](./paginators.md#listinsightspaginator)
3. item: [:material-code-braces: ListInsightsResponseTypeDef](./type_defs.md#listinsightsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInsightsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    StatusFilter: ListInsightsStatusFilterTypeDef,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListInsightsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ListInsightsStatusFilterTypeDef](./type_defs.md#listinsightsstatusfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListInsightsResponseTypeDef](./type_defs.md#listinsightsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListInsightsRequestListInsightsPaginateTypeDef = {  # (1)
    "StatusFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInsightsRequestListInsightsPaginateTypeDef](./type_defs.md#listinsightsrequestlistinsightspaginatetypedef) 
## ListMonitoredResourcesPaginator

Type annotations and code completion for `#!python session.create_client("devops-guru").get_paginator("list_monitored_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListMonitoredResources)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import ListMonitoredResourcesPaginator

session = get_session()
async with session.create_client("devops-guru") as client:  # (1)
    paginator: ListMonitoredResourcesPaginator = client.get_paginator("list_monitored_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListMonitoredResourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [DevOpsGuruClient](./client.md)
2. paginator: [ListMonitoredResourcesPaginator](./paginators.md#listmonitoredresourcespaginator)
3. item: [:material-code-braces: ListMonitoredResourcesResponseTypeDef](./type_defs.md#listmonitoredresourcesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMonitoredResourcesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: ListMonitoredResourcesFiltersTypeDef,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListMonitoredResourcesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ListMonitoredResourcesFiltersTypeDef](./type_defs.md#listmonitoredresourcesfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListMonitoredResourcesResponseTypeDef](./type_defs.md#listmonitoredresourcesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef](./type_defs.md#listmonitoredresourcesrequestlistmonitoredresourcespaginatetypedef) 
## ListNotificationChannelsPaginator

Type annotations and code completion for `#!python session.create_client("devops-guru").get_paginator("list_notification_channels")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListNotificationChannels)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import ListNotificationChannelsPaginator

session = get_session()
async with session.create_client("devops-guru") as client:  # (1)
    paginator: ListNotificationChannelsPaginator = client.get_paginator("list_notification_channels")  # (2)
    async for item in paginator.paginate(...):
        item: ListNotificationChannelsResponseTypeDef
        print(item)  # (3)
```

1. client: [DevOpsGuruClient](./client.md)
2. paginator: [ListNotificationChannelsPaginator](./paginators.md#listnotificationchannelspaginator)
3. item: [:material-code-braces: ListNotificationChannelsResponseTypeDef](./type_defs.md#listnotificationchannelsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListNotificationChannelsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListNotificationChannelsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListNotificationChannelsResponseTypeDef](./type_defs.md#listnotificationchannelsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef](./type_defs.md#listnotificationchannelsrequestlistnotificationchannelspaginatetypedef) 
## ListOrganizationInsightsPaginator

Type annotations and code completion for `#!python session.create_client("devops-guru").get_paginator("list_organization_insights")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListOrganizationInsights)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import ListOrganizationInsightsPaginator

session = get_session()
async with session.create_client("devops-guru") as client:  # (1)
    paginator: ListOrganizationInsightsPaginator = client.get_paginator("list_organization_insights")  # (2)
    async for item in paginator.paginate(...):
        item: ListOrganizationInsightsResponseTypeDef
        print(item)  # (3)
```

1. client: [DevOpsGuruClient](./client.md)
2. paginator: [ListOrganizationInsightsPaginator](./paginators.md#listorganizationinsightspaginator)
3. item: [:material-code-braces: ListOrganizationInsightsResponseTypeDef](./type_defs.md#listorganizationinsightsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListOrganizationInsightsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    StatusFilter: ListInsightsStatusFilterTypeDef,  # (1)
    AccountIds: Sequence[str] = ...,
    OrganizationalUnitIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListOrganizationInsightsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ListInsightsStatusFilterTypeDef](./type_defs.md#listinsightsstatusfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListOrganizationInsightsResponseTypeDef](./type_defs.md#listorganizationinsightsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = {  # (1)
    "StatusFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef](./type_defs.md#listorganizationinsightsrequestlistorganizationinsightspaginatetypedef) 
## ListRecommendationsPaginator

Type annotations and code completion for `#!python session.create_client("devops-guru").get_paginator("list_recommendations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListRecommendations)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import ListRecommendationsPaginator

session = get_session()
async with session.create_client("devops-guru") as client:  # (1)
    paginator: ListRecommendationsPaginator = client.get_paginator("list_recommendations")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecommendationsResponseTypeDef
        print(item)  # (3)
```

1. client: [DevOpsGuruClient](./client.md)
2. paginator: [ListRecommendationsPaginator](./paginators.md#listrecommendationspaginator)
3. item: [:material-code-braces: ListRecommendationsResponseTypeDef](./type_defs.md#listrecommendationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRecommendationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InsightId: str,
    Locale: LocaleType = ...,  # (1)
    AccountId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListRecommendationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListRecommendationsResponseTypeDef](./type_defs.md#listrecommendationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRecommendationsRequestListRecommendationsPaginateTypeDef = {  # (1)
    "InsightId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecommendationsRequestListRecommendationsPaginateTypeDef](./type_defs.md#listrecommendationsrequestlistrecommendationspaginatetypedef) 
## SearchInsightsPaginator

Type annotations and code completion for `#!python session.create_client("devops-guru").get_paginator("search_insights")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchInsights)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import SearchInsightsPaginator

session = get_session()
async with session.create_client("devops-guru") as client:  # (1)
    paginator: SearchInsightsPaginator = client.get_paginator("search_insights")  # (2)
    async for item in paginator.paginate(...):
        item: SearchInsightsResponseTypeDef
        print(item)  # (3)
```

1. client: [DevOpsGuruClient](./client.md)
2. paginator: [SearchInsightsPaginator](./paginators.md#searchinsightspaginator)
3. item: [:material-code-braces: SearchInsightsResponseTypeDef](./type_defs.md#searchinsightsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchInsightsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    StartTimeRange: StartTimeRangeTypeDef,  # (1)
    Type: InsightTypeType,  # (2)
    Filters: SearchInsightsFiltersTypeDef = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AsyncIterator[SearchInsightsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: StartTimeRangeTypeDef](./type_defs.md#starttimerangetypedef) 
2. See [:material-code-brackets: InsightTypeType](./literals.md#insighttypetype) 
3. See [:material-code-braces: SearchInsightsFiltersTypeDef](./type_defs.md#searchinsightsfilterstypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: SearchInsightsResponseTypeDef](./type_defs.md#searchinsightsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SearchInsightsRequestSearchInsightsPaginateTypeDef = {  # (1)
    "StartTimeRange": ...,
    "Type": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchInsightsRequestSearchInsightsPaginateTypeDef](./type_defs.md#searchinsightsrequestsearchinsightspaginatetypedef) 
## SearchOrganizationInsightsPaginator

Type annotations and code completion for `#!python session.create_client("devops-guru").get_paginator("search_organization_insights")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchOrganizationInsights)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.paginator import SearchOrganizationInsightsPaginator

session = get_session()
async with session.create_client("devops-guru") as client:  # (1)
    paginator: SearchOrganizationInsightsPaginator = client.get_paginator("search_organization_insights")  # (2)
    async for item in paginator.paginate(...):
        item: SearchOrganizationInsightsResponseTypeDef
        print(item)  # (3)
```

1. client: [DevOpsGuruClient](./client.md)
2. paginator: [SearchOrganizationInsightsPaginator](./paginators.md#searchorganizationinsightspaginator)
3. item: [:material-code-braces: SearchOrganizationInsightsResponseTypeDef](./type_defs.md#searchorganizationinsightsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchOrganizationInsightsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AccountIds: Sequence[str],
    StartTimeRange: StartTimeRangeTypeDef,  # (1)
    Type: InsightTypeType,  # (2)
    Filters: SearchOrganizationInsightsFiltersTypeDef = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AsyncIterator[SearchOrganizationInsightsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: StartTimeRangeTypeDef](./type_defs.md#starttimerangetypedef) 
2. See [:material-code-brackets: InsightTypeType](./literals.md#insighttypetype) 
3. See [:material-code-braces: SearchOrganizationInsightsFiltersTypeDef](./type_defs.md#searchorganizationinsightsfilterstypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: SearchOrganizationInsightsResponseTypeDef](./type_defs.md#searchorganizationinsightsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef = {  # (1)
    "AccountIds": ...,
    "StartTimeRange": ...,
    "Type": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef](./type_defs.md#searchorganizationinsightsrequestsearchorganizationinsightspaginatetypedef) 
