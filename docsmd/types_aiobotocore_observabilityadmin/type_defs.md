# Type definitions

> [Index](../README.md) > [CloudWatchObservabilityAdminService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CloudWatchObservabilityAdminService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin.html#cloudwatchobservabilityadminservice)
    type annotations stubs module [types-aiobotocore-observabilityadmin](https://pypi.org/project/types-aiobotocore-observabilityadmin/).



## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import ResponseMetadataTypeDef


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

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import PaginatorConfigTypeDef


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

## ListResourceTelemetryForOrganizationInputTypeDef

```python
# ListResourceTelemetryForOrganizationInputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import ListResourceTelemetryForOrganizationInputTypeDef


def get_value() -> ListResourceTelemetryForOrganizationInputTypeDef:
    return {
        "AccountIdentifiers": ...,
    }


# ListResourceTelemetryForOrganizationInputTypeDef definition

class ListResourceTelemetryForOrganizationInputTypeDef(TypedDict):
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
# TelemetryConfigurationTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import TelemetryConfigurationTypeDef


def get_value() -> TelemetryConfigurationTypeDef:
    return {
        "AccountIdentifier": ...,
    }


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
## ListResourceTelemetryInputTypeDef

```python
# ListResourceTelemetryInputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import ListResourceTelemetryInputTypeDef


def get_value() -> ListResourceTelemetryInputTypeDef:
    return {
        "ResourceIdentifierPrefix": ...,
    }


# ListResourceTelemetryInputTypeDef definition

class ListResourceTelemetryInputTypeDef(TypedDict):
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
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTelemetryEvaluationStatusForOrganizationOutputTypeDef

```python
# GetTelemetryEvaluationStatusForOrganizationOutputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import GetTelemetryEvaluationStatusForOrganizationOutputTypeDef


def get_value() -> GetTelemetryEvaluationStatusForOrganizationOutputTypeDef:
    return {
        "Status": ...,
    }


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
# GetTelemetryEvaluationStatusOutputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import GetTelemetryEvaluationStatusOutputTypeDef


def get_value() -> GetTelemetryEvaluationStatusOutputTypeDef:
    return {
        "Status": ...,
    }


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
# ListResourceTelemetryForOrganizationInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import ListResourceTelemetryForOrganizationInputPaginateTypeDef


def get_value() -> ListResourceTelemetryForOrganizationInputPaginateTypeDef:
    return {
        "AccountIdentifiers": ...,
    }


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
# ListResourceTelemetryInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import ListResourceTelemetryInputPaginateTypeDef


def get_value() -> ListResourceTelemetryInputPaginateTypeDef:
    return {
        "ResourceIdentifierPrefix": ...,
    }


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
# ListResourceTelemetryForOrganizationOutputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import ListResourceTelemetryForOrganizationOutputTypeDef


def get_value() -> ListResourceTelemetryForOrganizationOutputTypeDef:
    return {
        "TelemetryConfigurations": ...,
    }


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
# ListResourceTelemetryOutputTypeDef TypedDict usage example

from types_aiobotocore_observabilityadmin.type_defs import ListResourceTelemetryOutputTypeDef


def get_value() -> ListResourceTelemetryOutputTypeDef:
    return {
        "TelemetryConfigurations": ...,
    }


# ListResourceTelemetryOutputTypeDef definition

class ListResourceTelemetryOutputTypeDef(TypedDict):
    TelemetryConfigurations: List[TelemetryConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TelemetryConfigurationTypeDef](./type_defs.md#telemetryconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
