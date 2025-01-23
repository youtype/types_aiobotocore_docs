# Type definitions

> [Index](../README.md) > [CloudWatchObservabilityAdminService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CloudWatchObservabilityAdminService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin.html#cloudwatchobservabilityadminservice)
    type annotations stubs module [types-aiobotocore-observabilityadmin](https://pypi.org/project/types-aiobotocore-observabilityadmin/).



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

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListResourceTelemetryForOrganizationInputRequestTypeDef

```python
# ListResourceTelemetryForOrganizationInputRequestTypeDef definition

class ListResourceTelemetryForOrganizationInputRequestTypeDef(TypedDict):
    AccountIdentifiers: NotRequired[Sequence[str]],
    ResourceIdentifierPrefix: NotRequired[str],
    ResourceTypes: NotRequired[Sequence[ResourceTypeType]],  # (1)
    TelemetryConfigurationState: NotRequired[Mapping[TelemetryTypeType, TelemetryStateType]],  # (2)
    ResourceTags: NotRequired[Mapping[str, str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: TelemetryTypeType](./literals.md#telemetrytypetype) [:material-code-brackets: TelemetryStateType](./literals.md#telemetrystatetype) 
## TelemetryConfigurationTypeDef

```python
# TelemetryConfigurationTypeDef definition

class TelemetryConfigurationTypeDef(TypedDict):
    AccountIdentifier: NotRequired[str],
    TelemetryConfigurationState: NotRequired[Dict[TelemetryTypeType, TelemetryStateType]],  # (1)
    ResourceType: NotRequired[ResourceTypeType],  # (2)
    ResourceIdentifier: NotRequired[str],
    ResourceTags: NotRequired[Dict[str, str]],
    LastUpdateTimeStamp: NotRequired[int],
```

1. See [:material-code-brackets: TelemetryTypeType](./literals.md#telemetrytypetype) [:material-code-brackets: TelemetryStateType](./literals.md#telemetrystatetype) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## ListResourceTelemetryInputRequestTypeDef

```python
# ListResourceTelemetryInputRequestTypeDef definition

class ListResourceTelemetryInputRequestTypeDef(TypedDict):
    ResourceIdentifierPrefix: NotRequired[str],
    ResourceTypes: NotRequired[Sequence[ResourceTypeType]],  # (1)
    TelemetryConfigurationState: NotRequired[Mapping[TelemetryTypeType, TelemetryStateType]],  # (2)
    ResourceTags: NotRequired[Mapping[str, str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: TelemetryTypeType](./literals.md#telemetrytypetype) [:material-code-brackets: TelemetryStateType](./literals.md#telemetrystatetype) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTelemetryEvaluationStatusForOrganizationOutputTypeDef

```python
# GetTelemetryEvaluationStatusForOrganizationOutputTypeDef definition

class GetTelemetryEvaluationStatusForOrganizationOutputTypeDef(TypedDict):
    Status: StatusType,  # (1)
    FailureReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTelemetryEvaluationStatusOutputTypeDef

```python
# GetTelemetryEvaluationStatusOutputTypeDef definition

class GetTelemetryEvaluationStatusOutputTypeDef(TypedDict):
    Status: StatusType,  # (1)
    FailureReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourceTelemetryForOrganizationInputPaginateTypeDef

```python
# ListResourceTelemetryForOrganizationInputPaginateTypeDef definition

class ListResourceTelemetryForOrganizationInputPaginateTypeDef(TypedDict):
    AccountIdentifiers: NotRequired[Sequence[str]],
    ResourceIdentifierPrefix: NotRequired[str],
    ResourceTypes: NotRequired[Sequence[ResourceTypeType]],  # (1)
    TelemetryConfigurationState: NotRequired[Mapping[TelemetryTypeType, TelemetryStateType]],  # (2)
    ResourceTags: NotRequired[Mapping[str, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: TelemetryTypeType](./literals.md#telemetrytypetype) [:material-code-brackets: TelemetryStateType](./literals.md#telemetrystatetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceTelemetryInputPaginateTypeDef

```python
# ListResourceTelemetryInputPaginateTypeDef definition

class ListResourceTelemetryInputPaginateTypeDef(TypedDict):
    ResourceIdentifierPrefix: NotRequired[str],
    ResourceTypes: NotRequired[Sequence[ResourceTypeType]],  # (1)
    TelemetryConfigurationState: NotRequired[Mapping[TelemetryTypeType, TelemetryStateType]],  # (2)
    ResourceTags: NotRequired[Mapping[str, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: TelemetryTypeType](./literals.md#telemetrytypetype) [:material-code-brackets: TelemetryStateType](./literals.md#telemetrystatetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceTelemetryForOrganizationOutputTypeDef

```python
# ListResourceTelemetryForOrganizationOutputTypeDef definition

class ListResourceTelemetryForOrganizationOutputTypeDef(TypedDict):
    TelemetryConfigurations: List[TelemetryConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TelemetryConfigurationTypeDef](./type_defs.md#telemetryconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourceTelemetryOutputTypeDef

```python
# ListResourceTelemetryOutputTypeDef definition

class ListResourceTelemetryOutputTypeDef(TypedDict):
    TelemetryConfigurations: List[TelemetryConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TelemetryConfigurationTypeDef](./type_defs.md#telemetryconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
