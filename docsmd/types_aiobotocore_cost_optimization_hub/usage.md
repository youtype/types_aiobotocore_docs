# Examples

> [Index](../README.md) > [CostOptimizationHub](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CostOptimizationHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#costoptimizationhub)
    type annotations stubs module [types-aiobotocore-cost-optimization-hub](https://pypi.org/project/types-aiobotocore-cost-optimization-hub/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[cost-optimization-hub]` package installed.

Write your `CostOptimizationHub` code as usual,
type checking and code completion should work out of the box.



```python
# CostOptimizationHubClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cost-optimization-hub") as client:  # (1)
    result = await client.get_recommendation()  # (2)
```

1. client: [CostOptimizationHubClient](./client.md)
2. result: [:material-code-braces: GetRecommendationResponseTypeDef](./type_defs.md#getrecommendationresponsetypedef) 



```python
# ListEnrollmentStatusesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cost-optimization-hub") as client:  # (1)
    paginator = client.get_paginator("list_enrollment_statuses")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CostOptimizationHubClient](./client.md)
2. paginator: [ListEnrollmentStatusesPaginator](./paginators.md#listenrollmentstatusespaginator)
3. item: [:material-code-braces: ListEnrollmentStatusesResponseTypeDef](./type_defs.md#listenrollmentstatusesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[cost-optimization-hub]`
or a standalone `types_aiobotocore_cost_optimization_hub` package, you have to explicitly specify
`client: CostOptimizationHubClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CostOptimizationHubClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cost_optimization_hub.client import CostOptimizationHubClient
from types_aiobotocore_cost_optimization_hub.type_defs import GetRecommendationResponseTypeDef
from types_aiobotocore_cost_optimization_hub.type_defs import GetRecommendationRequestTypeDef


session = get_session()

async with session.create_client("cost-optimization-hub") as client:
    client: CostOptimizationHubClient
    kwargs: GetRecommendationRequestTypeDef = {...}
    result: GetRecommendationResponseTypeDef = await client.get_recommendation(**kwargs)
```



```python
# ListEnrollmentStatusesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cost_optimization_hub.client import CostOptimizationHubClient
from types_aiobotocore_cost_optimization_hub.paginator import ListEnrollmentStatusesPaginator
from types_aiobotocore_cost_optimization_hub.type_defs import ListEnrollmentStatusesResponseTypeDef


session = get_session()

async with session.create_client("cost-optimization-hub") as client:
    client: CostOptimizationHubClient
    paginator: ListEnrollmentStatusesPaginator = client.get_paginator("list_enrollment_statuses")
    async for item in paginator.paginate(...):
        item: ListEnrollmentStatusesResponseTypeDef
        print(item)
```


