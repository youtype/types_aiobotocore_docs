# Paginators

> [Index](../README.md) > [Pricing](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Pricing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#pricing)
    type annotations stubs module [types-aiobotocore-pricing](https://pypi.org/project/types-aiobotocore-pricing/).

## DescribeServicesPaginator

Type annotations and code completion for `#!python session.create_client("pricing").get_paginator("describe_services")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing/paginator/DescribeServices.html#Pricing.Paginator.DescribeServices)

```python
# DescribeServicesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pricing.paginator import DescribeServicesPaginator

session = get_session()
async with session.create_client("pricing") as client:  # (1)
    paginator: DescribeServicesPaginator = client.get_paginator("describe_services")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeServicesResponseTypeDef
        print(item)  # (3)
```

1. client: [PricingClient](./client.md)
2. paginator: [DescribeServicesPaginator](./paginators.md#describeservicespaginator)
3. item: [:material-code-braces: DescribeServicesResponseTypeDef](./type_defs.md#describeservicesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeServicesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ServiceCode: str = ...,
    FormatVersion: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeServicesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeServicesResponseTypeDef](./type_defs.md#describeservicesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeServicesRequestPaginateTypeDef = {  # (1)
    "ServiceCode": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeServicesRequestPaginateTypeDef](./type_defs.md#describeservicesrequestpaginatetypedef) 
## GetAttributeValuesPaginator

Type annotations and code completion for `#!python session.create_client("pricing").get_paginator("get_attribute_values")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing/paginator/GetAttributeValues.html#Pricing.Paginator.GetAttributeValues)

```python
# GetAttributeValuesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pricing.paginator import GetAttributeValuesPaginator

session = get_session()
async with session.create_client("pricing") as client:  # (1)
    paginator: GetAttributeValuesPaginator = client.get_paginator("get_attribute_values")  # (2)
    async for item in paginator.paginate(...):
        item: GetAttributeValuesResponseTypeDef
        print(item)  # (3)
```

1. client: [PricingClient](./client.md)
2. paginator: [GetAttributeValuesPaginator](./paginators.md#getattributevaluespaginator)
3. item: [:material-code-braces: GetAttributeValuesResponseTypeDef](./type_defs.md#getattributevaluesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetAttributeValuesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ServiceCode: str,
    AttributeName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetAttributeValuesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetAttributeValuesResponseTypeDef](./type_defs.md#getattributevaluesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetAttributeValuesRequestPaginateTypeDef = {  # (1)
    "ServiceCode": ...,
    "AttributeName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetAttributeValuesRequestPaginateTypeDef](./type_defs.md#getattributevaluesrequestpaginatetypedef) 
## GetProductsPaginator

Type annotations and code completion for `#!python session.create_client("pricing").get_paginator("get_products")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing/paginator/GetProducts.html#Pricing.Paginator.GetProducts)

```python
# GetProductsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pricing.paginator import GetProductsPaginator

session = get_session()
async with session.create_client("pricing") as client:  # (1)
    paginator: GetProductsPaginator = client.get_paginator("get_products")  # (2)
    async for item in paginator.paginate(...):
        item: GetProductsResponseTypeDef
        print(item)  # (3)
```

1. client: [PricingClient](./client.md)
2. paginator: [GetProductsPaginator](./paginators.md#getproductspaginator)
3. item: [:material-code-braces: GetProductsResponseTypeDef](./type_defs.md#getproductsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetProductsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ServiceCode: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    FormatVersion: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[GetProductsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetProductsResponseTypeDef](./type_defs.md#getproductsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetProductsRequestPaginateTypeDef = {  # (1)
    "ServiceCode": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetProductsRequestPaginateTypeDef](./type_defs.md#getproductsrequestpaginatetypedef) 
## ListPriceListsPaginator

Type annotations and code completion for `#!python session.create_client("pricing").get_paginator("list_price_lists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing/paginator/ListPriceLists.html#Pricing.Paginator.ListPriceLists)

```python
# ListPriceListsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pricing.paginator import ListPriceListsPaginator

session = get_session()
async with session.create_client("pricing") as client:  # (1)
    paginator: ListPriceListsPaginator = client.get_paginator("list_price_lists")  # (2)
    async for item in paginator.paginate(...):
        item: ListPriceListsResponseTypeDef
        print(item)  # (3)
```

1. client: [PricingClient](./client.md)
2. paginator: [ListPriceListsPaginator](./paginators.md#listpricelistspaginator)
3. item: [:material-code-braces: ListPriceListsResponseTypeDef](./type_defs.md#listpricelistsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPriceListsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ServiceCode: str,
    EffectiveDate: TimestampTypeDef,
    CurrencyCode: str,
    RegionCode: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPriceListsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPriceListsResponseTypeDef](./type_defs.md#listpricelistsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPriceListsRequestPaginateTypeDef = {  # (1)
    "ServiceCode": ...,
    "EffectiveDate": ...,
    "CurrencyCode": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPriceListsRequestPaginateTypeDef](./type_defs.md#listpricelistsrequestpaginatetypedef) 
