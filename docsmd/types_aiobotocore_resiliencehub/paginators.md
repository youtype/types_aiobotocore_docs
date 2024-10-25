# Paginators

> [Index](../README.md) > [ResilienceHub](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ResilienceHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
    type annotations stubs module [types-aiobotocore-resiliencehub](https://pypi.org/project/types-aiobotocore-resiliencehub/).

## ListAppAssessmentResourceDriftsPaginator

Type annotations and code completion for `#!python session.create_client("resiliencehub").get_paginator("list_app_assessment_resource_drifts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Paginator.ListAppAssessmentResourceDrifts)

```python
# ListAppAssessmentResourceDriftsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resiliencehub.paginator import ListAppAssessmentResourceDriftsPaginator

session = get_session()
async with session.create_client("resiliencehub") as client:  # (1)
    paginator: ListAppAssessmentResourceDriftsPaginator = client.get_paginator("list_app_assessment_resource_drifts")  # (2)
    async for item in paginator.paginate(...):
        item: ListAppAssessmentResourceDriftsResponseTypeDef
        print(item)  # (3)
```

1. client: [ResilienceHubClient](./client.md)
2. paginator: [ListAppAssessmentResourceDriftsPaginator](./paginators.md#listappassessmentresourcedriftspaginator)
3. item: [:material-code-braces: ListAppAssessmentResourceDriftsResponseTypeDef](./type_defs.md#listappassessmentresourcedriftsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAppAssessmentResourceDriftsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assessmentArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAppAssessmentResourceDriftsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAppAssessmentResourceDriftsResponseTypeDef](./type_defs.md#listappassessmentresourcedriftsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAppAssessmentResourceDriftsRequestListAppAssessmentResourceDriftsPaginateTypeDef = {  # (1)
    "assessmentArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAppAssessmentResourceDriftsRequestListAppAssessmentResourceDriftsPaginateTypeDef](./type_defs.md#listappassessmentresourcedriftsrequestlistappassessmentresourcedriftspaginatetypedef) 
## ListResourceGroupingRecommendationsPaginator

Type annotations and code completion for `#!python session.create_client("resiliencehub").get_paginator("list_resource_grouping_recommendations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Paginator.ListResourceGroupingRecommendations)

```python
# ListResourceGroupingRecommendationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resiliencehub.paginator import ListResourceGroupingRecommendationsPaginator

session = get_session()
async with session.create_client("resiliencehub") as client:  # (1)
    paginator: ListResourceGroupingRecommendationsPaginator = client.get_paginator("list_resource_grouping_recommendations")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceGroupingRecommendationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ResilienceHubClient](./client.md)
2. paginator: [ListResourceGroupingRecommendationsPaginator](./paginators.md#listresourcegroupingrecommendationspaginator)
3. item: [:material-code-braces: ListResourceGroupingRecommendationsResponseTypeDef](./type_defs.md#listresourcegroupingrecommendationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResourceGroupingRecommendationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    appArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListResourceGroupingRecommendationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResourceGroupingRecommendationsResponseTypeDef](./type_defs.md#listresourcegroupingrecommendationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResourceGroupingRecommendationsRequestListResourceGroupingRecommendationsPaginateTypeDef = {  # (1)
    "appArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceGroupingRecommendationsRequestListResourceGroupingRecommendationsPaginateTypeDef](./type_defs.md#listresourcegroupingrecommendationsrequestlistresourcegroupingrecommendationspaginatetypedef) 
