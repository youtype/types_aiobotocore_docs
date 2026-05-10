# Paginators

> [Index](../README.md) > [ConnectHealth](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ConnectHealth](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connecthealth.html#connecthealth)
    type annotations stubs module [types-aiobotocore-connecthealth](https://pypi.org/project/types-aiobotocore-connecthealth/).

## ListDomainsPaginator

Type annotations and code completion for `#!python session.create_client("connecthealth").get_paginator("list_domains")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connecthealth/paginator/ListDomains.html#ConnectHealth.Paginator.ListDomains)

```python
# ListDomainsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connecthealth.paginator import ListDomainsPaginator

session = get_session()
async with session.create_client("connecthealth") as client:  # (1)
    paginator: ListDomainsPaginator = client.get_paginator("list_domains")  # (2)
    async for item in paginator.paginate(...):
        item: ListDomainsOutputTypeDef
        print(item)  # (3)
```

1. client: [ConnectHealthClient](./client.md)
2. paginator: [ListDomainsPaginator](./paginators.md#listdomainspaginator)
3. item: `AioPageIterator[ListDomainsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDomainsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    status: DomainStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListDomainsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListDomainsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDomainsInputPaginateTypeDef = {  # (1)
    "status": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDomainsInputPaginateTypeDef](./type_defs.md#listdomainsinputpaginatetypedef)
## ListSubscriptionsPaginator

Type annotations and code completion for `#!python session.create_client("connecthealth").get_paginator("list_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connecthealth/paginator/ListSubscriptions.html#ConnectHealth.Paginator.ListSubscriptions)

```python
# ListSubscriptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connecthealth.paginator import ListSubscriptionsPaginator

session = get_session()
async with session.create_client("connecthealth") as client:  # (1)
    paginator: ListSubscriptionsPaginator = client.get_paginator("list_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSubscriptionsOutputTypeDef
        print(item)  # (3)
```

1. client: [ConnectHealthClient](./client.md)
2. paginator: [ListSubscriptionsPaginator](./paginators.md#listsubscriptionspaginator)
3. item: `AioPageIterator[ListSubscriptionsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSubscriptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSubscriptionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSubscriptionsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSubscriptionsInputPaginateTypeDef = {  # (1)
    "domainId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSubscriptionsInputPaginateTypeDef](./type_defs.md#listsubscriptionsinputpaginatetypedef)
