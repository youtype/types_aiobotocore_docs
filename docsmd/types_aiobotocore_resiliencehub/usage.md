# Examples

> [Index](../README.md) > [ResilienceHub](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ResilienceHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#resiliencehub)
    type annotations stubs module [types-aiobotocore-resiliencehub](https://pypi.org/project/types-aiobotocore-resiliencehub/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[resiliencehub]` package installed.

Write your `ResilienceHub` code as usual,
type checking and code completion should work out of the box.



```python
# ResilienceHubClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("resiliencehub") as client:  # (1)
    result = await client.accept_resource_grouping_recommendations()  # (2)
```

1. client: [ResilienceHubClient](./client.md)
2. result: [:material-code-braces: AcceptResourceGroupingRecommendationsResponseTypeDef](./type_defs.md#acceptresourcegroupingrecommendationsresponsetypedef) 



```python
# ListAppAssessmentResourceDriftsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("resiliencehub") as client:  # (1)
    paginator = client.get_paginator("list_app_assessment_resource_drifts")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ResilienceHubClient](./client.md)
2. paginator: [ListAppAssessmentResourceDriftsPaginator](./paginators.md#listappassessmentresourcedriftspaginator)
3. item: [:material-code-braces: ListAppAssessmentResourceDriftsResponseTypeDef](./type_defs.md#listappassessmentresourcedriftsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[resiliencehub]`
or a standalone `types_aiobotocore_resiliencehub` package, you have to explicitly specify
`client: ResilienceHubClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ResilienceHubClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_resiliencehub.client import ResilienceHubClient
from types_aiobotocore_resiliencehub.type_defs import AcceptResourceGroupingRecommendationsResponseTypeDef
from types_aiobotocore_resiliencehub.type_defs import AcceptResourceGroupingRecommendationsRequestTypeDef


session = get_session()

async with session.create_client("resiliencehub") as client:
    client: ResilienceHubClient
    kwargs: AcceptResourceGroupingRecommendationsRequestTypeDef = {...}
    result: AcceptResourceGroupingRecommendationsResponseTypeDef = await client.accept_resource_grouping_recommendations(**kwargs)
```



```python
# ListAppAssessmentResourceDriftsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_resiliencehub.client import ResilienceHubClient
from types_aiobotocore_resiliencehub.paginator import ListAppAssessmentResourceDriftsPaginator
from types_aiobotocore_resiliencehub.type_defs import ListAppAssessmentResourceDriftsResponseTypeDef


session = get_session()

async with session.create_client("resiliencehub") as client:
    client: ResilienceHubClient
    paginator: ListAppAssessmentResourceDriftsPaginator = client.get_paginator("list_app_assessment_resource_drifts")
    async for item in paginator.paginate(...):
        item: ListAppAssessmentResourceDriftsResponseTypeDef
        print(item)
```


