# Pricing module

> [Index](../README.md) > Pricing


!!! note ""

    Auto-generated documentation for [Pricing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
    type annotations stubs module [types-aiobotocore-pricing](https://pypi.org/project/types-aiobotocore-pricing/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `Pricing`.

### From PyPI with pip

Install `types-aiobotocore` for `Pricing` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[pricing]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[pricing]'


# standalone installation
python -m pip install types-aiobotocore-pricing
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-pricing
```

## Usage

Code samples can be found in [Examples](./usage.md).

## PricingClient

Type annotations and code completion for  `#!python session.create_client("pricing")` as [PricingClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_pricing.client import PricingClient


session = get_session()
async with session.create_client("pricing") as client:
    client: PricingClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("pricing").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_pricing.paginator import DescribeServicesPaginator

def get_describe_services_paginator() -> DescribeServicesPaginator:
    return client.get_paginator("describe_services"))
```

- [DescribeServicesPaginator](./paginators.md#describeservicespaginator)
- [GetAttributeValuesPaginator](./paginators.md#getattributevaluespaginator)
- [GetProductsPaginator](./paginators.md#getproductspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_pricing.literals import DescribeServicesPaginatorName

def get_value() -> DescribeServicesPaginatorName:
    return "describe_services"
```

- [DescribeServicesPaginatorName](./literals.md#describeservicespaginatorname)
- [FilterTypeType](./literals.md#filtertypetype)
- [GetAttributeValuesPaginatorName](./literals.md#getattributevaluespaginatorname)
- [GetProductsPaginatorName](./literals.md#getproductspaginatorname)
- [PricingServiceName](./literals.md#pricingservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_pricing.type_defs import AttributeValueTypeDef

def get_value() -> AttributeValueTypeDef:
    return {
        "Value": ...,
    }
```

- [AttributeValueTypeDef](./type_defs.md#attributevaluetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeServicesRequestRequestTypeDef](./type_defs.md#describeservicesrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ServiceTypeDef](./type_defs.md#servicetypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [GetAttributeValuesRequestRequestTypeDef](./type_defs.md#getattributevaluesrequestrequesttypedef)
- [DescribeServicesRequestDescribeServicesPaginateTypeDef](./type_defs.md#describeservicesrequestdescribeservicespaginatetypedef)
- [GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef](./type_defs.md#getattributevaluesrequestgetattributevaluespaginatetypedef)
- [GetAttributeValuesResponseTypeDef](./type_defs.md#getattributevaluesresponsetypedef)
- [GetProductsResponseTypeDef](./type_defs.md#getproductsresponsetypedef)
- [DescribeServicesResponseTypeDef](./type_defs.md#describeservicesresponsetypedef)
- [GetProductsRequestGetProductsPaginateTypeDef](./type_defs.md#getproductsrequestgetproductspaginatetypedef)
- [GetProductsRequestRequestTypeDef](./type_defs.md#getproductsrequestrequesttypedef)

