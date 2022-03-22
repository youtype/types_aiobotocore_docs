<a id="pricingclient-for-aiobotocore-pricing-module"></a>

# PricingClient for aiobotocore Pricing module

> [Index](../README.md) > [Pricing](./README.md) > PricingClient

Auto-generated documentation for
[Pricing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
type annotations stubs module
[types-aiobotocore-pricing](https://pypi.org/project/types-aiobotocore-pricing/).

- [PricingClient for aiobotocore Pricing module](#pricingclient-for-aiobotocore-pricing-module)
  - [PricingClient](#pricingclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [describe_services](#describe_services)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_attribute_values](#get_attribute_values)
    - [get_products](#get_products)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="pricingclient"></a>

## PricingClient

Type annotations for `session.create_client("pricing")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_pricing.client import PricingClient

session = get_session()
async with session.create_client("pricing") as client:
    client: PricingClient
```

Boto3 documentation:
[Pricing.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_pricing.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ExpiredNextTokenException`
- `Exceptions.InternalErrorException`
- `Exceptions.InvalidNextTokenException`
- `Exceptions.InvalidParameterException`
- `Exceptions.NotFoundException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

PricingClient exceptions.

Type annotations for `session.create_client("pricing").exceptions` method.

Boto3 documentation:
[Pricing.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("pricing").can_paginate` method.

Boto3 documentation:
[Pricing.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="describe\_services"></a>

### describe_services

Returns the metadata for one service or a list of the metadata for all
services.

Type annotations for `session.create_client("pricing").describe_services`
method.

Boto3 documentation:
[Pricing.Client.describe_services](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client.describe_services)

Asynchronous method. Use `await describe_services(...)` for a synchronous call.

Arguments mapping described in
[DescribeServicesRequestRequestTypeDef](./type_defs.md#describeservicesrequestrequesttypedef).

Keyword-only arguments:

- `ServiceCode`: `str`
- `FormatVersion`: `str`
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[DescribeServicesResponseTypeDef](./type_defs.md#describeservicesresponsetypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("pricing").generate_presigned_url`
method.

Boto3 documentation:
[Pricing.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_attribute\_values"></a>

### get_attribute_values

Returns a list of attribute values.

Type annotations for `session.create_client("pricing").get_attribute_values`
method.

Boto3 documentation:
[Pricing.Client.get_attribute_values](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client.get_attribute_values)

Asynchronous method. Use `await get_attribute_values(...)` for a synchronous
call.

Arguments mapping described in
[GetAttributeValuesRequestRequestTypeDef](./type_defs.md#getattributevaluesrequestrequesttypedef).

Keyword-only arguments:

- `ServiceCode`: `str` *(required)*
- `AttributeName`: `str` *(required)*
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[GetAttributeValuesResponseTypeDef](./type_defs.md#getattributevaluesresponsetypedef).

<a id="get\_products"></a>

### get_products

Returns a list of all products that match the filter criteria.

Type annotations for `session.create_client("pricing").get_products` method.

Boto3 documentation:
[Pricing.Client.get_products](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client.get_products)

Asynchronous method. Use `await get_products(...)` for a synchronous call.

Arguments mapping described in
[GetProductsRequestRequestTypeDef](./type_defs.md#getproductsrequestrequesttypedef).

Keyword-only arguments:

- `ServiceCode`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `FormatVersion`: `str`
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[GetProductsResponseTypeDef](./type_defs.md#getproductsresponsetypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("pricing").__aenter__` method.

Boto3 documentation:
[Pricing.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [PricingClient](#pricingclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("pricing").__aexit__` method.

Boto3 documentation:
[Pricing.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("pricing").get_paginator` method
with overloads.

- `client.get_paginator("describe_services")` ->
  [DescribeServicesPaginator](./paginators.md#describeservicespaginator)
- `client.get_paginator("get_attribute_values")` ->
  [GetAttributeValuesPaginator](./paginators.md#getattributevaluespaginator)
- `client.get_paginator("get_products")` ->
  [GetProductsPaginator](./paginators.md#getproductspaginator)
