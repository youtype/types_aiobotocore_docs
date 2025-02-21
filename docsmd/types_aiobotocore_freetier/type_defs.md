# Type definitions

> [Index](../README.md) > [FreeTier](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [FreeTier](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/freetier.html#freetier)
    type annotations stubs module [types-aiobotocore-freetier](https://pypi.org/project/types-aiobotocore-freetier/).



## DimensionValuesTypeDef

```python
# DimensionValuesTypeDef TypedDict usage example

from types_aiobotocore_freetier.type_defs import DimensionValuesTypeDef


def get_value() -> DimensionValuesTypeDef:
    return {
        "Key": ...,
    }


# DimensionValuesTypeDef definition

class DimensionValuesTypeDef(TypedDict):
    Key: DimensionType,  # (1)
    MatchOptions: Sequence[MatchOptionType],  # (2)
    Values: Sequence[str],
```

1. See [:material-code-brackets: DimensionType](./literals.md#dimensiontype) 
2. See [:material-code-brackets: MatchOptionType](./literals.md#matchoptiontype) 
## FreeTierUsageTypeDef

```python
# FreeTierUsageTypeDef TypedDict usage example

from types_aiobotocore_freetier.type_defs import FreeTierUsageTypeDef


def get_value() -> FreeTierUsageTypeDef:
    return {
        "actualUsageAmount": ...,
    }


# FreeTierUsageTypeDef definition

class FreeTierUsageTypeDef(TypedDict):
    actualUsageAmount: NotRequired[float],
    description: NotRequired[str],
    forecastedUsageAmount: NotRequired[float],
    freeTierType: NotRequired[str],
    limit: NotRequired[float],
    operation: NotRequired[str],
    region: NotRequired[str],
    service: NotRequired[str],
    unit: NotRequired[str],
    usageType: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_freetier.type_defs import PaginatorConfigTypeDef


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

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_freetier.type_defs import ResponseMetadataTypeDef


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

## ExpressionPaginatorTypeDef

```python
# ExpressionPaginatorTypeDef TypedDict usage example

from types_aiobotocore_freetier.type_defs import ExpressionPaginatorTypeDef


def get_value() -> ExpressionPaginatorTypeDef:
    return {
        "And": ...,
    }


# ExpressionPaginatorTypeDef definition

class ExpressionPaginatorTypeDef(TypedDict):
    And: NotRequired[Sequence[Mapping[str, Any]]],
    Dimensions: NotRequired[DimensionValuesTypeDef],  # (1)
    Not: NotRequired[Mapping[str, Any]],
    Or: NotRequired[Sequence[Mapping[str, Any]]],
```

1. See [:material-code-braces: DimensionValuesTypeDef](./type_defs.md#dimensionvaluestypedef) 
## ExpressionTypeDef

```python
# ExpressionTypeDef TypedDict usage example

from types_aiobotocore_freetier.type_defs import ExpressionTypeDef


def get_value() -> ExpressionTypeDef:
    return {
        "And": ...,
    }


# ExpressionTypeDef definition

class ExpressionTypeDef(TypedDict):
    And: NotRequired[Sequence[Mapping[str, Any]]],
    Dimensions: NotRequired[DimensionValuesTypeDef],  # (1)
    Not: NotRequired[Mapping[str, Any]],
    Or: NotRequired[Sequence[Mapping[str, Any]]],
```

1. See [:material-code-braces: DimensionValuesTypeDef](./type_defs.md#dimensionvaluestypedef) 
## GetFreeTierUsageResponseTypeDef

```python
# GetFreeTierUsageResponseTypeDef TypedDict usage example

from types_aiobotocore_freetier.type_defs import GetFreeTierUsageResponseTypeDef


def get_value() -> GetFreeTierUsageResponseTypeDef:
    return {
        "freeTierUsages": ...,
    }


# GetFreeTierUsageResponseTypeDef definition

class GetFreeTierUsageResponseTypeDef(TypedDict):
    freeTierUsages: List[FreeTierUsageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FreeTierUsageTypeDef](./type_defs.md#freetierusagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFreeTierUsageRequestPaginateTypeDef

```python
# GetFreeTierUsageRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_freetier.type_defs import GetFreeTierUsageRequestPaginateTypeDef


def get_value() -> GetFreeTierUsageRequestPaginateTypeDef:
    return {
        "filter": ...,
    }


# GetFreeTierUsageRequestPaginateTypeDef definition

class GetFreeTierUsageRequestPaginateTypeDef(TypedDict):
    filter: NotRequired[ExpressionPaginatorTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ExpressionPaginatorTypeDef](./type_defs.md#expressionpaginatortypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetFreeTierUsageRequestTypeDef

```python
# GetFreeTierUsageRequestTypeDef TypedDict usage example

from types_aiobotocore_freetier.type_defs import GetFreeTierUsageRequestTypeDef


def get_value() -> GetFreeTierUsageRequestTypeDef:
    return {
        "filter": ...,
    }


# GetFreeTierUsageRequestTypeDef definition

class GetFreeTierUsageRequestTypeDef(TypedDict):
    filter: NotRequired[ExpressionTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
