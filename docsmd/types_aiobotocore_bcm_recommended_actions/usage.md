# Examples

> [Index](../README.md) > [BillingandCostManagementRecommendedActions](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [BillingandCostManagementRecommendedActions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-recommended-actions.html#billingandcostmanagementrecommendedactions)
    type annotations stubs module [types-aiobotocore-bcm-recommended-actions](https://pypi.org/project/types-aiobotocore-bcm-recommended-actions/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[bcm-recommended-actions]` package installed.

Write your `BillingandCostManagementRecommendedActions` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# BillingandCostManagementRecommendedActionsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("bcm-recommended-actions") as client:  # (1)
    result = await client.list_recommended_actions()  # (2)
```

1. client: [BillingandCostManagementRecommendedActionsClient](./client.md)
2. result: [:material-code-braces: ListRecommendedActionsResponseTypeDef](./type_defs.md#listrecommendedactionsresponsetypedef)



#### Paginator usage example

```python
# ListRecommendedActionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("bcm-recommended-actions") as client:  # (1)
    paginator = client.get_paginator("list_recommended_actions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [BillingandCostManagementRecommendedActionsClient](./client.md)
2. paginator: [ListRecommendedActionsPaginator](./paginators.md#listrecommendedactionspaginator)
3. item: [:material-code-braces: ListRecommendedActionsResponseTypeDef](./type_defs.md#listrecommendedactionsresponsetypedef)




### Explicit type annotations

With `types-aiobotocore-lite[bcm-recommended-actions]`
or a standalone `types_aiobotocore_bcm_recommended_actions` package, you have to explicitly specify
`client: BillingandCostManagementRecommendedActionsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# BillingandCostManagementRecommendedActionsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_bcm_recommended_actions.client import BillingandCostManagementRecommendedActionsClient
from types_aiobotocore_bcm_recommended_actions.type_defs import ListRecommendedActionsResponseTypeDef
from types_aiobotocore_bcm_recommended_actions.type_defs import ListRecommendedActionsRequestTypeDef


session = get_session()

async with session.create_client("bcm-recommended-actions") as client:
    client: BillingandCostManagementRecommendedActionsClient
    kwargs: ListRecommendedActionsRequestTypeDef = {...}
    result: ListRecommendedActionsResponseTypeDef = await client.list_recommended_actions(**kwargs)
```



#### Paginator usage example

```python
# ListRecommendedActionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_bcm_recommended_actions.client import BillingandCostManagementRecommendedActionsClient
from types_aiobotocore_bcm_recommended_actions.paginator import ListRecommendedActionsPaginator
from types_aiobotocore_bcm_recommended_actions.type_defs import ListRecommendedActionsResponseTypeDef


session = get_session()

async with session.create_client("bcm-recommended-actions") as client:
    client: BillingandCostManagementRecommendedActionsClient
    paginator: ListRecommendedActionsPaginator = client.get_paginator("list_recommended_actions")
    async for item in paginator.paginate(...):
        item: ListRecommendedActionsResponseTypeDef
        print(item)
```


