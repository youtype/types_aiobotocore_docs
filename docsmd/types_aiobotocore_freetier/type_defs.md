# Type definitions

> [Index](../README.md) > [FreeTier](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [FreeTier](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/freetier.html#freetier)
    type annotations stubs module [types-aiobotocore-freetier](https://pypi.org/project/types-aiobotocore-freetier/).



## DimensionValuesTypeDef

```python
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
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
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
# GetFreeTierUsageRequestPaginateTypeDef definition

class GetFreeTierUsageRequestPaginateTypeDef(TypedDict):
    filter: NotRequired[ExpressionPaginatorTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ExpressionPaginatorTypeDef](./type_defs.md#expressionpaginatortypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetFreeTierUsageRequestRequestTypeDef

```python
# GetFreeTierUsageRequestRequestTypeDef definition

class GetFreeTierUsageRequestRequestTypeDef(TypedDict):
    filter: NotRequired[ExpressionTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
