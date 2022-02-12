<a id="paginators-for-aiobotocore-pricing-module"></a>

# Paginators for aiobotocore Pricing module

> [Index](..) > [Pricing](.) > Paginators

Auto-generated documentation for
[Pricing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
type annotations stubs module
[types-aiobotocore-pricing](https://pypi.org/project/types-aiobotocore-pricing/).

- [Paginators for aiobotocore Pricing module](#paginators-for-aiobotocore-pricing-module)
  - [DescribeServicesPaginator](#describeservicespaginator)
  - [GetAttributeValuesPaginator](#getattributevaluespaginator)
  - [GetProductsPaginator](#getproductspaginator)

<a id="describeservicespaginator"></a>

## DescribeServicesPaginator

Type annotations for
`session.create_client("pricing").get_paginator("describe_services")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_pricing.paginator import DescribeServicesPaginator

session = get_session()
async with session.create_client("pricing") as client:
    client: PricingClient
    paginator: DescribeServicesPaginator = client.get_paginator("describe_services")
```

Boto3 documentation:
[Pricing.Paginator.DescribeServices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.DescribeServices)

Arguments for `DescribeServicesPaginator.paginate` method:

- `ServiceCode`: `str`
- `FormatVersion`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeServicesPaginator.paginate` returns
`AsyncIterable`\[[DescribeServicesResponseTypeDef](./type_defs.md#describeservicesresponsetypedef)\].

<a id="getattributevaluespaginator"></a>

## GetAttributeValuesPaginator

Type annotations for
`session.create_client("pricing").get_paginator("get_attribute_values")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_pricing.paginator import GetAttributeValuesPaginator

session = get_session()
async with session.create_client("pricing") as client:
    client: PricingClient
    paginator: GetAttributeValuesPaginator = client.get_paginator("get_attribute_values")
```

Boto3 documentation:
[Pricing.Paginator.GetAttributeValues](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.GetAttributeValues)

Arguments for `GetAttributeValuesPaginator.paginate` method:

- `ServiceCode`: `str` *(required)*
- `AttributeName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetAttributeValuesPaginator.paginate` returns
`AsyncIterable`\[[GetAttributeValuesResponseTypeDef](./type_defs.md#getattributevaluesresponsetypedef)\].

<a id="getproductspaginator"></a>

## GetProductsPaginator

Type annotations for
`session.create_client("pricing").get_paginator("get_products")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_pricing.paginator import GetProductsPaginator

session = get_session()
async with session.create_client("pricing") as client:
    client: PricingClient
    paginator: GetProductsPaginator = client.get_paginator("get_products")
```

Boto3 documentation:
[Pricing.Paginator.GetProducts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.GetProducts)

Arguments for `GetProductsPaginator.paginate` method:

- `ServiceCode`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `FormatVersion`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetProductsPaginator.paginate` returns
`AsyncIterable`\[[GetProductsResponseTypeDef](./type_defs.md#getproductsresponsetypedef)\].
