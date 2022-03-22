<a id="typed-dictionaries-for-aiobotocore-marketplaceentitlementservice-module"></a>

# Typed dictionaries for aiobotocore MarketplaceEntitlementService module

> [Index](../README.md) > [MarketplaceEntitlementService](./README.md) > Typed
> dictionaries

Auto-generated documentation for
[MarketplaceEntitlementService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
type annotations stubs module
[types-aiobotocore-marketplace-entitlement](https://pypi.org/project/types-aiobotocore-marketplace-entitlement/).

- [Typed dictionaries for aiobotocore MarketplaceEntitlementService module](#typed-dictionaries-for-aiobotocore-marketplaceentitlementservice-module)
  - [EntitlementTypeDef](#entitlementtypedef)
  - [EntitlementValueTypeDef](#entitlementvaluetypedef)
  - [GetEntitlementsRequestRequestTypeDef](#getentitlementsrequestrequesttypedef)
  - [GetEntitlementsResultTypeDef](#getentitlementsresulttypedef)
  - [PaginatorConfigTypeDef](#paginatorconfigtypedef)
  - [ResponseMetadataTypeDef](#responsemetadatatypedef)

<a id="entitlementtypedef"></a>

## EntitlementTypeDef

```python
from types_aiobotocore_marketplace_entitlement.type_defs import EntitlementTypeDef
```

Optional fields:

- `ProductCode`: `str`
- `Dimension`: `str`
- `CustomerIdentifier`: `str`
- `Value`: [EntitlementValueTypeDef](./type_defs.md#entitlementvaluetypedef)
- `ExpirationDate`: `datetime`

<a id="entitlementvaluetypedef"></a>

## EntitlementValueTypeDef

```python
from types_aiobotocore_marketplace_entitlement.type_defs import EntitlementValueTypeDef
```

Optional fields:

- `IntegerValue`: `int`
- `DoubleValue`: `float`
- `BooleanValue`: `bool`
- `StringValue`: `str`

<a id="getentitlementsrequestrequesttypedef"></a>

## GetEntitlementsRequestRequestTypeDef

```python
from types_aiobotocore_marketplace_entitlement.type_defs import GetEntitlementsRequestRequestTypeDef
```

Required fields:

- `ProductCode`: `str`

Optional fields:

- `Filter`:
  `Mapping`\[[GetEntitlementFilterNameType](./literals.md#getentitlementfilternametype),
  `Sequence`\[`str`\]\]
- `NextToken`: `str`
- `MaxResults`: `int`

<a id="getentitlementsresulttypedef"></a>

## GetEntitlementsResultTypeDef

```python
from types_aiobotocore_marketplace_entitlement.type_defs import GetEntitlementsResultTypeDef
```

Required fields:

- `Entitlements`:
  `List`\[[EntitlementTypeDef](./type_defs.md#entitlementtypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="paginatorconfigtypedef"></a>

## PaginatorConfigTypeDef

```python
from types_aiobotocore_marketplace_entitlement.type_defs import PaginatorConfigTypeDef
```

Optional fields:

- `MaxItems`: `int`
- `PageSize`: `int`
- `StartingToken`: `str`

<a id="responsemetadatatypedef"></a>

## ResponseMetadataTypeDef

```python
from types_aiobotocore_marketplace_entitlement.type_defs import ResponseMetadataTypeDef
```

Required fields:

- `RequestId`: `str`
- `HostId`: `str`
- `HTTPStatusCode`: `int`
- `HTTPHeaders`: `Dict`\[`str`, `str`\]
- `RetryAttempts`: `int`
