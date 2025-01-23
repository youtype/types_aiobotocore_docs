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
    activeTimeRange: ActiveTimeRangeTypeDef = ...,  # (1)
    arns: Sequence[str] = ...,
    billingViewTypes: Sequence[BillingViewTypeType] = ...,  # (2)
    ownerAccountId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListBillingViewsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: ActiveTimeRangeTypeDef](./type_defs.md#activetimerangetypedef) 
2. See [:material-code-brackets: BillingViewTypeType](./literals.md#billingviewtypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListBillingViewsResponseTypeDef](./type_defs.md#listbillingviewsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListBillingViewsRequestPaginateTypeDef = {  # (1)
    "activeTimeRange": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBillingViewsRequestPaginateTypeDef](./type_defs.md#listbillingviewsrequestpaginatetypedef) 
## ListSourceViewsForBillingViewPaginator

Type annotations and code completion for `#!python session.create_client("billing").get_paginator("list_source_views_for_billing_view")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing/paginator/ListSourceViewsForBillingView.html#Billing.Paginator.ListSourceViewsForBillingView)

```python
# ListSourceViewsForBillingViewPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_billing.paginator import ListSourceViewsForBillingViewPaginator

session = get_session()
async with session.create_client("billing") as client:  # (1)
    paginator: ListSourceViewsForBillingViewPaginator = client.get_paginator("list_source_views_for_billing_view")  # (2)
    async for item in paginator.paginate(...):
        item: ListSourceViewsForBillingViewResponseTypeDef
        print(item)  # (3)
```

1. client: [BillingClient](./client.md)
2. paginator: [ListSourceViewsForBillingViewPaginator](./paginators.md#listsourceviewsforbillingviewpaginator)
3. item: [:material-code-braces: ListSourceViewsForBillingViewResponseTypeDef](./type_defs.md#listsourceviewsforbillingviewresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSourceViewsForBillingViewPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    arn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSourceViewsForBillingViewResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSourceViewsForBillingViewResponseTypeDef](./type_defs.md#listsourceviewsforbillingviewresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSourceViewsForBillingViewRequestPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSourceViewsForBillingViewRequestPaginateTypeDef](./type_defs.md#listsourceviewsforbillingviewrequestpaginatetypedef) 
