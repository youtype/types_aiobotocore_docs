# Examples

> [Index](../README.md) > [BillingandCostManagementDashboards](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [BillingandCostManagementDashboards](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-dashboards.html#billingandcostmanagementdashboards)
    type annotations stubs module [types-aiobotocore-bcm-dashboards](https://pypi.org/project/types-aiobotocore-bcm-dashboards/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[bcm-dashboards]` package installed.

Write your `BillingandCostManagementDashboards` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# BillingandCostManagementDashboardsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("bcm-dashboards") as client:  # (1)
    result = await client.create_dashboard()  # (2)
```

1. client: [BillingandCostManagementDashboardsClient](./client.md)
2. result: [:material-code-braces: CreateDashboardResponseTypeDef](./type_defs.md#createdashboardresponsetypedef)



#### Paginator usage example

```python
# ListDashboardsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("bcm-dashboards") as client:  # (1)
    paginator = client.get_paginator("list_dashboards")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [BillingandCostManagementDashboardsClient](./client.md)
2. paginator: [ListDashboardsPaginator](./paginators.md#listdashboardspaginator)
3. item: [:material-code-braces: ListDashboardsResponseTypeDef](./type_defs.md#listdashboardsresponsetypedef)




### Explicit type annotations

With `types-aiobotocore-lite[bcm-dashboards]`
or a standalone `types_aiobotocore_bcm_dashboards` package, you have to explicitly specify
`client: BillingandCostManagementDashboardsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# BillingandCostManagementDashboardsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_bcm_dashboards.client import BillingandCostManagementDashboardsClient
from types_aiobotocore_bcm_dashboards.type_defs import CreateDashboardResponseTypeDef
from types_aiobotocore_bcm_dashboards.type_defs import CreateDashboardRequestTypeDef


session = get_session()

async with session.create_client("bcm-dashboards") as client:
    client: BillingandCostManagementDashboardsClient
    kwargs: CreateDashboardRequestTypeDef = {...}
    result: CreateDashboardResponseTypeDef = await client.create_dashboard(**kwargs)
```



#### Paginator usage example

```python
# ListDashboardsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_bcm_dashboards.client import BillingandCostManagementDashboardsClient
from types_aiobotocore_bcm_dashboards.paginator import ListDashboardsPaginator
from types_aiobotocore_bcm_dashboards.type_defs import ListDashboardsResponseTypeDef


session = get_session()

async with session.create_client("bcm-dashboards") as client:
    client: BillingandCostManagementDashboardsClient
    paginator: ListDashboardsPaginator = client.get_paginator("list_dashboards")
    async for item in paginator.paginate(...):
        item: ListDashboardsResponseTypeDef
        print(item)
```


