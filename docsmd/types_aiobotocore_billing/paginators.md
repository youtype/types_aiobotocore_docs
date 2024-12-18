# Paginators

> [Index](../README.md) > [Billing](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Billing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing.html#billing)
    type annotations stubs module [types-aiobotocore-billing](https://pypi.org/project/types-aiobotocore-billing/).

## ListBillingViewsPaginator

Type annotations and code completion for `#!python session.create_client("billing").get_paginator("list_billing_views")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing/paginator/ListBillingViews.html#Billing.Paginator.ListBillingViews)

```python
# ListBillingViewsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_billing.paginator import ListBillingViewsPaginator

session = get_session()
async with session.create_client("billing") as client:  # (1)
    paginator: ListBillingViewsPaginator = client.get_paginator("list_billing_views")  # (2)
    async for item in paginator.paginate(...):
        item: ListBillingViewsResponseTypeDef
        print(item)  # (3)
```

1. client: [BillingClient](./client.md)
2. paginator: [ListBillingViewsPaginator](./paginators.md#listbillingviewspaginator)
3. item: [:material-code-braces: ListBillingViewsResponseTypeDef](./type_defs.md#listbillingviewsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListBillingViewsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    activeTimeRange: ActiveTimeRangeTypeDef,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListBillingViewsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ActiveTimeRangeTypeDef](./type_defs.md#activetimerangetypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListBillingViewsResponseTypeDef](./type_defs.md#listbillingviewsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListBillingViewsRequestListBillingViewsPaginateTypeDef = {  # (1)
    "activeTimeRange": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBillingViewsRequestListBillingViewsPaginateTypeDef](./type_defs.md#listbillingviewsrequestlistbillingviewspaginatetypedef) 
