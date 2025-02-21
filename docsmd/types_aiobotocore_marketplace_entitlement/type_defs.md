# Type definitions

> [Index](../README.md) > [MarketplaceEntitlementService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MarketplaceEntitlementService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#marketplaceentitlementservice)
    type annotations stubs module [types-aiobotocore-marketplace-entitlement](https://pypi.org/project/types-aiobotocore-marketplace-entitlement/).



## EntitlementValueTypeDef

```python
# EntitlementValueTypeDef TypedDict usage example

from types_aiobotocore_marketplace_entitlement.type_defs import EntitlementValueTypeDef


def get_value() -> EntitlementValueTypeDef:
    return {
        "IntegerValue": ...,
    }


# EntitlementValueTypeDef definition

class EntitlementValueTypeDef(TypedDict):
    IntegerValue: NotRequired[int],
    DoubleValue: NotRequired[float],
    BooleanValue: NotRequired[bool],
    StringValue: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_marketplace_entitlement.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetEntitlementsRequestTypeDef

```python
# GetEntitlementsRequestTypeDef TypedDict usage example

from types_aiobotocore_marketplace_entitlement.type_defs import GetEntitlementsRequestTypeDef


def get_value() -> GetEntitlementsRequestTypeDef:
    return {
        "ProductCode": ...,
    }


# GetEntitlementsRequestTypeDef definition

class GetEntitlementsRequestTypeDef(TypedDict):
    ProductCode: str,
    Filter: NotRequired[Mapping[GetEntitlementFilterNameType, Sequence[str]]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: GetEntitlementFilterNameType](./literals.md#getentitlementfilternametype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_marketplace_entitlement.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## EntitlementTypeDef

```python
# EntitlementTypeDef TypedDict usage example

from types_aiobotocore_marketplace_entitlement.type_defs import EntitlementTypeDef


def get_value() -> EntitlementTypeDef:
    return {
        "ProductCode": ...,
    }


# EntitlementTypeDef definition

class EntitlementTypeDef(TypedDict):
    ProductCode: NotRequired[str],
    Dimension: NotRequired[str],
    CustomerIdentifier: NotRequired[str],
    Value: NotRequired[EntitlementValueTypeDef],  # (1)
    ExpirationDate: NotRequired[datetime],
```

1. See [:material-code-braces: EntitlementValueTypeDef](./type_defs.md#entitlementvaluetypedef) 
## GetEntitlementsRequestPaginateTypeDef

```python
# GetEntitlementsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_marketplace_entitlement.type_defs import GetEntitlementsRequestPaginateTypeDef


def get_value() -> GetEntitlementsRequestPaginateTypeDef:
    return {
        "ProductCode": ...,
    }


# GetEntitlementsRequestPaginateTypeDef definition

class GetEntitlementsRequestPaginateTypeDef(TypedDict):
    ProductCode: str,
    Filter: NotRequired[Mapping[GetEntitlementFilterNameType, Sequence[str]]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: GetEntitlementFilterNameType](./literals.md#getentitlementfilternametype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetEntitlementsResultTypeDef

```python
# GetEntitlementsResultTypeDef TypedDict usage example

from types_aiobotocore_marketplace_entitlement.type_defs import GetEntitlementsResultTypeDef


def get_value() -> GetEntitlementsResultTypeDef:
    return {
        "Entitlements": ...,
    }


# GetEntitlementsResultTypeDef definition

class GetEntitlementsResultTypeDef(TypedDict):
    Entitlements: List[EntitlementTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EntitlementTypeDef](./type_defs.md#entitlementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
