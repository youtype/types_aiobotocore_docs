# Type definitions

> [Index](../README.md) > [ControlTower](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ControlTower](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
    type annotations stubs module [types-aiobotocore-controltower](https://pypi.org/project/types-aiobotocore-controltower/).



## ControlOperationTypeDef

```python
# ControlOperationTypeDef definition

class ControlOperationTypeDef(TypedDict):
    endTime: NotRequired[datetime],
    operationType: NotRequired[ControlOperationTypeType],  # (1)
    startTime: NotRequired[datetime],
    status: NotRequired[ControlOperationStatusType],  # (2)
    statusMessage: NotRequired[str],
```

1. See [:material-code-brackets: ControlOperationTypeType](./literals.md#controloperationtypetype) 
2. See [:material-code-brackets: ControlOperationStatusType](./literals.md#controloperationstatustype) 
## DisableControlInputRequestTypeDef

```python
# DisableControlInputRequestTypeDef definition

class DisableControlInputRequestTypeDef(TypedDict):
    controlIdentifier: str,
    targetIdentifier: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## EnableControlInputRequestTypeDef

```python
# EnableControlInputRequestTypeDef definition

class EnableControlInputRequestTypeDef(TypedDict):
    controlIdentifier: str,
    targetIdentifier: str,
```

## EnabledControlSummaryTypeDef

```python
# EnabledControlSummaryTypeDef definition

class EnabledControlSummaryTypeDef(TypedDict):
    controlIdentifier: NotRequired[str],
```

## GetControlOperationInputRequestTypeDef

```python
# GetControlOperationInputRequestTypeDef definition

class GetControlOperationInputRequestTypeDef(TypedDict):
    operationIdentifier: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListEnabledControlsInputRequestTypeDef

```python
# ListEnabledControlsInputRequestTypeDef definition

class ListEnabledControlsInputRequestTypeDef(TypedDict):
    targetIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## DisableControlOutputTypeDef

```python
# DisableControlOutputTypeDef definition

class DisableControlOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableControlOutputTypeDef

```python
# EnableControlOutputTypeDef definition

class EnableControlOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetControlOperationOutputTypeDef

```python
# GetControlOperationOutputTypeDef definition

class GetControlOperationOutputTypeDef(TypedDict):
    controlOperation: ControlOperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ControlOperationTypeDef](./type_defs.md#controloperationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnabledControlsOutputTypeDef

```python
# ListEnabledControlsOutputTypeDef definition

class ListEnabledControlsOutputTypeDef(TypedDict):
    enabledControls: List[EnabledControlSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnabledControlSummaryTypeDef](./type_defs.md#enabledcontrolsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnabledControlsInputListEnabledControlsPaginateTypeDef

```python
# ListEnabledControlsInputListEnabledControlsPaginateTypeDef definition

class ListEnabledControlsInputListEnabledControlsPaginateTypeDef(TypedDict):
    targetIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
