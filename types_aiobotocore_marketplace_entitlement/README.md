<a id="type-annotations-for-aiobotocore-marketplaceentitlementservice-module"></a>

# Type annotations for aiobotocore MarketplaceEntitlementService module

> [Index](..) > MarketplaceEntitlementService

Auto-generated documentation for
[MarketplaceEntitlementService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
type annotations stubs module
[types-aiobotocore-marketplace-entitlement](https://pypi.org/project/types-aiobotocore-marketplace-entitlement/).

```bash
# install with types-aiobotocore
pip install 'types-aiobotocore[marketplace-entitlement]'

# install as a standalone
pip install types-aiobotocore-marketplace-entitlement
```

- [Type annotations for aiobotocore MarketplaceEntitlementService module](#type-annotations-for-aiobotocore-marketplaceentitlementservice-module)
  - [MarketplaceEntitlementServiceClient](#marketplaceentitlementserviceclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Paginators](#paginators)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="marketplaceentitlementserviceclient"></a>

## MarketplaceEntitlementServiceClient

Type annotations for `aiobotocore.create_client("marketplace-entitlement")` as
[MarketplaceEntitlementServiceClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_marketplace_entitlement.client import MarketplaceEntitlementServiceClient
```

<a id="methods"></a>

### Methods

- [can_paginate](./client.md#can_paginate)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [get_entitlements](./client.md#get_entitlements)
- [get_paginator](./client.md#get_paginator)

<a id="exceptions"></a>

### Exceptions

MarketplaceEntitlementServiceClient [exceptions](./client.md#exceptions)

- ClientError
- InternalServiceErrorException
- InvalidParameterException
- ThrottlingException

<a id="paginators"></a>

## Paginators

Type annotations for [paginators](./paginators.md) from
`boto3.client("marketplace-entitlement").get_paginator("...")`.

Can be used directly:

```python
from types_aiobotocore_marketplace_entitlement.paginators import GetEntitlementsPaginator, ...
```

- [GetEntitlementsPaginator](./paginators.md#getentitlementspaginator)

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_marketplace_entitlement.literals import GetEntitlementFilterNameType, ...
```

- [GetEntitlementFilterNameType](./literals.md#getentitlementfilternametype)
- [GetEntitlementsPaginatorName](./literals.md#getentitlementspaginatorname)
- [ServiceName](./literals.md#servicename)
- [PaginatorName](./literals.md#paginatorname)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_marketplace_entitlement.type_defs import EntitlementTypeDef, ...
```

- [EntitlementTypeDef](./type_defs.md#entitlementtypedef)
- [EntitlementValueTypeDef](./type_defs.md#entitlementvaluetypedef)
- [GetEntitlementsRequestRequestTypeDef](./type_defs.md#getentitlementsrequestrequesttypedef)
- [GetEntitlementsResultTypeDef](./type_defs.md#getentitlementsresulttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
