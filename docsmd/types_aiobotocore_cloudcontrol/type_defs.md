# Type definitions

> [Index](../README.md) > [CloudControlApi](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CloudControlApi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#cloudcontrolapi)
    type annotations stubs module [types-aiobotocore-cloudcontrol](https://pypi.org/project/types-aiobotocore-cloudcontrol/).



## CancelResourceRequestInputRequestTypeDef

```python
# CancelResourceRequestInputRequestTypeDef definition

class CancelResourceRequestInputRequestTypeDef(TypedDict):
    RequestToken: str,
```

## ProgressEventTypeDef

```python
# ProgressEventTypeDef definition

class ProgressEventTypeDef(TypedDict):
    TypeName: NotRequired[str],
    Identifier: NotRequired[str],
    RequestToken: NotRequired[str],
    HooksRequestToken: NotRequired[str],
    Operation: NotRequired[OperationType],  # (1)
    OperationStatus: NotRequired[OperationStatusType],  # (2)
    EventTime: NotRequired[datetime],
    ResourceModel: NotRequired[str],
    StatusMessage: NotRequired[str],
    ErrorCode: NotRequired[HandlerErrorCodeType],  # (3)
    RetryAfter: NotRequired[datetime],
```

1. See [:material-code-brackets: OperationType](./literals.md#operationtype) 
2. See [:material-code-brackets: OperationStatusType](./literals.md#operationstatustype) 
3. See [:material-code-brackets: HandlerErrorCodeType](./literals.md#handlererrorcodetype) 
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

## CreateResourceInputRequestTypeDef

```python
# CreateResourceInputRequestTypeDef definition

class CreateResourceInputRequestTypeDef(TypedDict):
    TypeName: str,
    DesiredState: str,
    TypeVersionId: NotRequired[str],
    RoleArn: NotRequired[str],
    ClientToken: NotRequired[str],
```

## DeleteResourceInputRequestTypeDef

```python
# DeleteResourceInputRequestTypeDef definition

class DeleteResourceInputRequestTypeDef(TypedDict):
    TypeName: str,
    Identifier: str,
    TypeVersionId: NotRequired[str],
    RoleArn: NotRequired[str],
    ClientToken: NotRequired[str],
```

## GetResourceInputRequestTypeDef

```python
# GetResourceInputRequestTypeDef definition

class GetResourceInputRequestTypeDef(TypedDict):
    TypeName: str,
    Identifier: str,
    TypeVersionId: NotRequired[str],
    RoleArn: NotRequired[str],
```

## ResourceDescriptionTypeDef

```python
# ResourceDescriptionTypeDef definition

class ResourceDescriptionTypeDef(TypedDict):
    Identifier: NotRequired[str],
    Properties: NotRequired[str],
```

## GetResourceRequestStatusInputRequestTypeDef

```python
# GetResourceRequestStatusInputRequestTypeDef definition

class GetResourceRequestStatusInputRequestTypeDef(TypedDict):
    RequestToken: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## HookProgressEventTypeDef

```python
# HookProgressEventTypeDef definition

class HookProgressEventTypeDef(TypedDict):
    HookTypeName: NotRequired[str],
    HookTypeVersionId: NotRequired[str],
    HookTypeArn: NotRequired[str],
    InvocationPoint: NotRequired[str],
    HookStatus: NotRequired[str],
    HookEventTime: NotRequired[datetime],
    HookStatusMessage: NotRequired[str],
    FailureMode: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ResourceRequestStatusFilterTypeDef

```python
# ResourceRequestStatusFilterTypeDef definition

class ResourceRequestStatusFilterTypeDef(TypedDict):
    Operations: NotRequired[Sequence[OperationType]],  # (1)
    OperationStatuses: NotRequired[Sequence[OperationStatusType]],  # (2)
```

1. See [:material-code-brackets: OperationType](./literals.md#operationtype) 
2. See [:material-code-brackets: OperationStatusType](./literals.md#operationstatustype) 
## ListResourcesInputRequestTypeDef

```python
# ListResourcesInputRequestTypeDef definition

class ListResourcesInputRequestTypeDef(TypedDict):
    TypeName: str,
    TypeVersionId: NotRequired[str],
    RoleArn: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ResourceModel: NotRequired[str],
```

## UpdateResourceInputRequestTypeDef

```python
# UpdateResourceInputRequestTypeDef definition

class UpdateResourceInputRequestTypeDef(TypedDict):
    TypeName: str,
    Identifier: str,
    PatchDocument: str,
    TypeVersionId: NotRequired[str],
    RoleArn: NotRequired[str],
    ClientToken: NotRequired[str],
```

## CancelResourceRequestOutputTypeDef

```python
# CancelResourceRequestOutputTypeDef definition

class CancelResourceRequestOutputTypeDef(TypedDict):
    ProgressEvent: ProgressEventTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProgressEventTypeDef](./type_defs.md#progresseventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateResourceOutputTypeDef

```python
# CreateResourceOutputTypeDef definition

class CreateResourceOutputTypeDef(TypedDict):
    ProgressEvent: ProgressEventTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProgressEventTypeDef](./type_defs.md#progresseventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteResourceOutputTypeDef

```python
# DeleteResourceOutputTypeDef definition

class DeleteResourceOutputTypeDef(TypedDict):
    ProgressEvent: ProgressEventTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProgressEventTypeDef](./type_defs.md#progresseventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourceRequestsOutputTypeDef

```python
# ListResourceRequestsOutputTypeDef definition

class ListResourceRequestsOutputTypeDef(TypedDict):
    ResourceRequestStatusSummaries: List[ProgressEventTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProgressEventTypeDef](./type_defs.md#progresseventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateResourceOutputTypeDef

```python
# UpdateResourceOutputTypeDef definition

class UpdateResourceOutputTypeDef(TypedDict):
    ProgressEvent: ProgressEventTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProgressEventTypeDef](./type_defs.md#progresseventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourceOutputTypeDef

```python
# GetResourceOutputTypeDef definition

class GetResourceOutputTypeDef(TypedDict):
    TypeName: str,
    ResourceDescription: ResourceDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceDescriptionTypeDef](./type_defs.md#resourcedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourcesOutputTypeDef

```python
# ListResourcesOutputTypeDef definition

class ListResourcesOutputTypeDef(TypedDict):
    TypeName: str,
    ResourceDescriptions: List[ResourceDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceDescriptionTypeDef](./type_defs.md#resourcedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourceRequestStatusInputWaitTypeDef

```python
# GetResourceRequestStatusInputWaitTypeDef definition

class GetResourceRequestStatusInputWaitTypeDef(TypedDict):
    RequestToken: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetResourceRequestStatusOutputTypeDef

```python
# GetResourceRequestStatusOutputTypeDef definition

class GetResourceRequestStatusOutputTypeDef(TypedDict):
    ProgressEvent: ProgressEventTypeDef,  # (1)
    HooksProgressEvent: List[HookProgressEventTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ProgressEventTypeDef](./type_defs.md#progresseventtypedef) 
2. See [:material-code-braces: HookProgressEventTypeDef](./type_defs.md#hookprogresseventtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourcesInputPaginateTypeDef

```python
# ListResourcesInputPaginateTypeDef definition

class ListResourcesInputPaginateTypeDef(TypedDict):
    TypeName: str,
    TypeVersionId: NotRequired[str],
    RoleArn: NotRequired[str],
    ResourceModel: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceRequestsInputPaginateTypeDef

```python
# ListResourceRequestsInputPaginateTypeDef definition

class ListResourceRequestsInputPaginateTypeDef(TypedDict):
    ResourceRequestStatusFilter: NotRequired[ResourceRequestStatusFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ResourceRequestStatusFilterTypeDef](./type_defs.md#resourcerequeststatusfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceRequestsInputRequestTypeDef

```python
# ListResourceRequestsInputRequestTypeDef definition

class ListResourceRequestsInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ResourceRequestStatusFilter: NotRequired[ResourceRequestStatusFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ResourceRequestStatusFilterTypeDef](./type_defs.md#resourcerequeststatusfiltertypedef) 
