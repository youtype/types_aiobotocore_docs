# Paginators

> [Index](../README.md) > [BillingandCostManagementDashboards](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [BillingandCostManagementDashboards](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-dashboards.html#billingandcostmanagementdashboards)
    type annotations stubs module [types-aiobotocore-bcm-dashboards](https://pypi.org/project/types-aiobotocore-bcm-dashboards/).

## ListDashboardsPaginator

Type annotations and code completion for `#!python session.create_client("bcm-dashboards").get_paginator("list_dashboards")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-dashboards/paginator/ListDashboards.html#BillingandCostManagementDashboards.Paginator.ListDashboards)

```python
# ListDashboardsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bcm_dashboards.paginator import ListDashboardsPaginator

session = get_session()
async with session.create_client("bcm-dashboards") as client:  # (1)
    paginator: ListDashboardsPaginator = client.get_paginator("list_dashboards")  # (2)
    async for item in paginator.paginate(...):
        item: ListDashboardsResponseTypeDef
        print(item)  # (3)
```

1. client: [BillingandCostManagementDashboardsClient](./client.md)
2. paginator: [ListDashboardsPaginator](./paginators.md#listdashboardspaginator)
3. item: `AioPageIterator[ListDashboardsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDashboardsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDashboardsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDashboardsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDashboardsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDashboardsRequestPaginateTypeDef](./type_defs.md#listdashboardsrequestpaginatetypedef)
