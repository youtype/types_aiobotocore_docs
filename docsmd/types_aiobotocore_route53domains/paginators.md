# Paginators

> [Index](../README.md) > [Route53Domains](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Route53Domains](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#route53domains)
    type annotations stubs module [types-aiobotocore-route53domains](https://pypi.org/project/types-aiobotocore-route53domains/).

## ListDomainsPaginator

Type annotations and code completion for `#!python session.create_client("route53domains").get_paginator("list_domains")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains/paginator/ListDomains.html#Route53Domains.Paginator.ListDomains)

```python
# ListDomainsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53domains.paginator import ListDomainsPaginator

session = get_session()
async with session.create_client("route53domains") as client:  # (1)
    paginator: ListDomainsPaginator = client.get_paginator("list_domains")  # (2)
    async for item in paginator.paginate(...):
        item: ListDomainsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53DomainsClient](./client.md)
2. paginator: [ListDomainsPaginator](./paginators.md#listdomainspaginator)
3. item: [:material-code-braces: ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDomainsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FilterConditions: Sequence[FilterConditionTypeDef] = ...,  # (1)
    SortCondition: SortConditionTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListDomainsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FilterConditionTypeDef](./type_defs.md#filterconditiontypedef) 
2. See [:material-code-braces: SortConditionTypeDef](./type_defs.md#sortconditiontypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDomainsRequestPaginateTypeDef = {  # (1)
    "FilterConditions": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDomainsRequestPaginateTypeDef](./type_defs.md#listdomainsrequestpaginatetypedef) 
## ListOperationsPaginator

Type annotations and code completion for `#!python session.create_client("route53domains").get_paginator("list_operations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains/paginator/ListOperations.html#Route53Domains.Paginator.ListOperations)

```python
# ListOperationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53domains.paginator import ListOperationsPaginator

session = get_session()
async with session.create_client("route53domains") as client:  # (1)
    paginator: ListOperationsPaginator = client.get_paginator("list_operations")  # (2)
    async for item in paginator.paginate(...):
        item: ListOperationsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53DomainsClient](./client.md)
2. paginator: [ListOperationsPaginator](./paginators.md#listoperationspaginator)
3. item: [:material-code-braces: ListOperationsResponseTypeDef](./type_defs.md#listoperationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListOperationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SubmittedSince: TimestampTypeDef = ...,
    Status: Sequence[OperationStatusType] = ...,  # (1)
    Type: Sequence[OperationTypeType] = ...,  # (2)
    SortBy: ListOperationsSortAttributeNameType = ...,  # (3)
    SortOrder: SortOrderType = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> AioPageIterator[ListOperationsResponseTypeDef]:  # (6)
    ...
```

1. See [:material-code-brackets: OperationStatusType](./literals.md#operationstatustype) 
2. See [:material-code-brackets: OperationTypeType](./literals.md#operationtypetype) 
3. See [:material-code-brackets: ListOperationsSortAttributeNameType](./literals.md#listoperationssortattributenametype) 
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
6. See [:material-code-braces: ListOperationsResponseTypeDef](./type_defs.md#listoperationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListOperationsRequestPaginateTypeDef = {  # (1)
    "SubmittedSince": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOperationsRequestPaginateTypeDef](./type_defs.md#listoperationsrequestpaginatetypedef) 
## ListPricesPaginator

Type annotations and code completion for `#!python session.create_client("route53domains").get_paginator("list_prices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains/paginator/ListPrices.html#Route53Domains.Paginator.ListPrices)

```python
# ListPricesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53domains.paginator import ListPricesPaginator

session = get_session()
async with session.create_client("route53domains") as client:  # (1)
    paginator: ListPricesPaginator = client.get_paginator("list_prices")  # (2)
    async for item in paginator.paginate(...):
        item: ListPricesResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53DomainsClient](./client.md)
2. paginator: [ListPricesPaginator](./paginators.md#listpricespaginator)
3. item: [:material-code-braces: ListPricesResponseTypeDef](./type_defs.md#listpricesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPricesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Tld: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPricesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPricesResponseTypeDef](./type_defs.md#listpricesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPricesRequestPaginateTypeDef = {  # (1)
    "Tld": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPricesRequestPaginateTypeDef](./type_defs.md#listpricesrequestpaginatetypedef) 
## ViewBillingPaginator

Type annotations and code completion for `#!python session.create_client("route53domains").get_paginator("view_billing")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains/paginator/ViewBilling.html#Route53Domains.Paginator.ViewBilling)

```python
# ViewBillingPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53domains.paginator import ViewBillingPaginator

session = get_session()
async with session.create_client("route53domains") as client:  # (1)
    paginator: ViewBillingPaginator = client.get_paginator("view_billing")  # (2)
    async for item in paginator.paginate(...):
        item: ViewBillingResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53DomainsClient](./client.md)
2. paginator: [ViewBillingPaginator](./paginators.md#viewbillingpaginator)
3. item: [:material-code-braces: ViewBillingResponseTypeDef](./type_defs.md#viewbillingresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ViewBillingPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Start: TimestampTypeDef = ...,
    End: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ViewBillingResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ViewBillingResponseTypeDef](./type_defs.md#viewbillingresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ViewBillingRequestPaginateTypeDef = {  # (1)
    "Start": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ViewBillingRequestPaginateTypeDef](./type_defs.md#viewbillingrequestpaginatetypedef) 
