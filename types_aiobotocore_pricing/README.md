<a id="type-annotations-for-aiobotocore-pricing-module"></a>

# Type annotations for aiobotocore Pricing module

> [Index](..) > Pricing

Auto-generated documentation for
[Pricing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
type annotations stubs module
[types-aiobotocore-pricing](https://pypi.org/project/types-aiobotocore-pricing/).

```bash
# install with types-aiobotocore
pip install 'types-aiobotocore[pricing]'

# Lite version does not provide session.create_client overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[pricing]'

# standalone installation
pip install types-aiobotocore-pricing
```

- [Type annotations for aiobotocore Pricing module](#type-annotations-for-aiobotocore-pricing-module)
  - [PricingClient](#pricingclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Paginators](#paginators)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="pricingclient"></a>

## PricingClient

Type annotations for `session.create_client("pricing")` as
[PricingClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_pricing.client import PricingClient
```

<a id="methods"></a>

### Methods

- [__aenter__](./client.md#__aenter__)
- [__aexit__](./client.md#__aexit__)
- [can_paginate](./client.md#can_paginate)
- [describe_services](./client.md#describe_services)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [get_attribute_values](./client.md#get_attribute_values)
- [get_paginator](./client.md#get_paginator)
- [get_products](./client.md#get_products)

<a id="exceptions"></a>

### Exceptions

PricingClient [exceptions](./client.md#exceptions)

- ClientError
- ExpiredNextTokenException
- InternalErrorException
- InvalidNextTokenException
- InvalidParameterException
- NotFoundException

<a id="paginators"></a>

## Paginators

Type annotations for [paginators](./paginators.md) from
`boto3.client("pricing").get_paginator("...")`.

Can be used directly:

```python
from types_aiobotocore_pricing.paginator import DescribeServicesPaginator, ...
```

- [DescribeServicesPaginator](./paginators.md#describeservicespaginator)
- [GetAttributeValuesPaginator](./paginators.md#getattributevaluespaginator)
- [GetProductsPaginator](./paginators.md#getproductspaginator)

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_pricing.literals import DescribeServicesPaginatorName, ...
```

- [DescribeServicesPaginatorName](./literals.md#describeservicespaginatorname)
- [FilterTypeType](./literals.md#filtertypetype)
- [GetAttributeValuesPaginatorName](./literals.md#getattributevaluespaginatorname)
- [GetProductsPaginatorName](./literals.md#getproductspaginatorname)
- [ServiceName](./literals.md#servicename)
- [PaginatorName](./literals.md#paginatorname)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_pricing.type_defs import AttributeValueTypeDef, ...
```

- [AttributeValueTypeDef](./type_defs.md#attributevaluetypedef)
- [DescribeServicesRequestRequestTypeDef](./type_defs.md#describeservicesrequestrequesttypedef)
- [DescribeServicesResponseTypeDef](./type_defs.md#describeservicesresponsetypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [GetAttributeValuesRequestRequestTypeDef](./type_defs.md#getattributevaluesrequestrequesttypedef)
- [GetAttributeValuesResponseTypeDef](./type_defs.md#getattributevaluesresponsetypedef)
- [GetProductsRequestRequestTypeDef](./type_defs.md#getproductsrequestrequesttypedef)
- [GetProductsResponseTypeDef](./type_defs.md#getproductsresponsetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ServiceTypeDef](./type_defs.md#servicetypedef)
