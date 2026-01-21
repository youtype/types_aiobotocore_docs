# MarketplaceEntitlementService module

> [Index](../README.md) > MarketplaceEntitlementService


!!! note ""

    Auto-generated documentation for [MarketplaceEntitlementService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#marketplaceentitlementservice)
    type annotations stubs module [types-aiobotocore-marketplace-entitlement](https://pypi.org/project/types-aiobotocore-marketplace-entitlement/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `MarketplaceEntitlementService` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `MarketplaceEntitlementService` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[marketplace-entitlement]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[marketplace-entitlement]'

# standalone installation
python -m pip install types-aiobotocore-marketplace-entitlement
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-marketplace-entitlement
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MarketplaceEntitlementServiceClient

Type annotations and code completion for  `#!python session.create_client("marketplace-entitlement")` as [MarketplaceEntitlementServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client)

```python
# MarketplaceEntitlementServiceClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_marketplace_entitlement.client import MarketplaceEntitlementServiceClient


session = get_session()
async with session.create_client("marketplace-entitlement") as client:
    client: MarketplaceEntitlementServiceClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("marketplace-entitlement").get_paginator("...")`.

```python
# GetEntitlementsPaginator usage example

from types_aiobotocore_marketplace_entitlement.paginator import GetEntitlementsPaginator

def get_get_entitlements_paginator() -> GetEntitlementsPaginator:
    return client.get_paginator("get_entitlements"))
```

- [GetEntitlementsPaginator](./paginators.md#getentitlementspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# GetEntitlementFilterNameType usage example

from types_aiobotocore_marketplace_entitlement.literals import GetEntitlementFilterNameType

def get_value() -> GetEntitlementFilterNameType:
    return "CUSTOMER_AWS_ACCOUNT_ID"
```

- [GetEntitlementFilterNameType](./literals.md#getentitlementfilternametype)
- [GetEntitlementsPaginatorName](./literals.md#getentitlementspaginatorname)
- [MarketplaceEntitlementServiceServiceName](./literals.md#marketplaceentitlementserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [EntitlementValueTypeDef](./type_defs.md#entitlementvaluetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetEntitlementsRequestTypeDef](./type_defs.md#getentitlementsrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [EntitlementTypeDef](./type_defs.md#entitlementtypedef)
- [GetEntitlementsRequestPaginateTypeDef](./type_defs.md#getentitlementsrequestpaginatetypedef)
- [GetEntitlementsResultTypeDef](./type_defs.md#getentitlementsresulttypedef)

