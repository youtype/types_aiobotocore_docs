# Type definitions

> [Index](../README.md) > [ForecastQueryService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ForecastQueryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService)
    type annotations stubs module [types-aiobotocore-forecastquery](https://pypi.org/project/types-aiobotocore-forecastquery/).



## DataPointTypeDef

```python
# DataPointTypeDef definition

class DataPointTypeDef(TypedDict):
    Timestamp: NotRequired[str],
    Value: NotRequired[float],
```

## QueryForecastRequestRequestTypeDef

```python
# QueryForecastRequestRequestTypeDef definition

class QueryForecastRequestRequestTypeDef(TypedDict):
    ForecastArn: str,
    Filters: Mapping[str, str],
    StartDate: NotRequired[str],
    EndDate: NotRequired[str],
    NextToken: NotRequired[str],
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

## QueryWhatIfForecastRequestRequestTypeDef

```python
# QueryWhatIfForecastRequestRequestTypeDef definition

class QueryWhatIfForecastRequestRequestTypeDef(TypedDict):
    WhatIfForecastArn: str,
    Filters: Mapping[str, str],
    StartDate: NotRequired[str],
    EndDate: NotRequired[str],
    NextToken: NotRequired[str],
```

## ForecastTypeDef

```python
# ForecastTypeDef definition

class ForecastTypeDef(TypedDict):
    Predictions: NotRequired[Dict[str, List[DataPointTypeDef]]],  # (1)
```

1. See [:material-code-braces: DataPointTypeDef](./type_defs.md#datapointtypedef) 
## QueryForecastResponseTypeDef

```python
# QueryForecastResponseTypeDef definition

class QueryForecastResponseTypeDef(TypedDict):
    Forecast: ForecastTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ForecastTypeDef](./type_defs.md#forecasttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## QueryWhatIfForecastResponseTypeDef

```python
# QueryWhatIfForecastResponseTypeDef definition

class QueryWhatIfForecastResponseTypeDef(TypedDict):
    Forecast: ForecastTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ForecastTypeDef](./type_defs.md#forecasttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
