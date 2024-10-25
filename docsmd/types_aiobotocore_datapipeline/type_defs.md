# Type definitions

> [Index](../README.md) > [DataPipeline](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [DataPipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
    type annotations stubs module [types-aiobotocore-datapipeline](https://pypi.org/project/types-aiobotocore-datapipeline/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## PipelineObjectUnionTypeDef

```python
# PipelineObjectUnionTypeDef definition

PipelineObjectUnionTypeDef = Union[
    PipelineObjectTypeDef,  # (1)
    PipelineObjectOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PipelineObjectTypeDef](./type_defs.md#pipelineobjecttypedef) 
2. See [:material-code-braces: PipelineObjectOutputTypeDef](./type_defs.md#pipelineobjectoutputtypedef) 

## ParameterObjectUnionTypeDef

```python
# ParameterObjectUnionTypeDef definition

ParameterObjectUnionTypeDef = Union[
    ParameterObjectTypeDef,  # (1)
    ParameterObjectOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ParameterObjectTypeDef](./type_defs.md#parameterobjecttypedef) 
2. See [:material-code-braces: ParameterObjectOutputTypeDef](./type_defs.md#parameterobjectoutputtypedef) 



## ParameterValueTypeDef

```python
# ParameterValueTypeDef definition

class ParameterValueTypeDef(TypedDict):
    id: str,
    stringValue: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
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

## DeactivatePipelineInputRequestTypeDef

```python
# DeactivatePipelineInputRequestTypeDef definition

class DeactivatePipelineInputRequestTypeDef(TypedDict):
    pipelineId: str,
    cancelActive: NotRequired[bool],
```

## DeletePipelineInputRequestTypeDef

```python
# DeletePipelineInputRequestTypeDef definition

class DeletePipelineInputRequestTypeDef(TypedDict):
    pipelineId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeObjectsInputRequestTypeDef

```python
# DescribeObjectsInputRequestTypeDef definition

class DescribeObjectsInputRequestTypeDef(TypedDict):
    pipelineId: str,
    objectIds: Sequence[str],
    evaluateExpressions: NotRequired[bool],
    marker: NotRequired[str],
```

## DescribePipelinesInputRequestTypeDef

```python
# DescribePipelinesInputRequestTypeDef definition

class DescribePipelinesInputRequestTypeDef(TypedDict):
    pipelineIds: Sequence[str],
```

## EvaluateExpressionInputRequestTypeDef

```python
# EvaluateExpressionInputRequestTypeDef definition

class EvaluateExpressionInputRequestTypeDef(TypedDict):
    pipelineId: str,
    objectId: str,
    expression: str,
```

## FieldTypeDef

```python
# FieldTypeDef definition

class FieldTypeDef(TypedDict):
    key: str,
    stringValue: NotRequired[str],
    refValue: NotRequired[str],
```

## GetPipelineDefinitionInputRequestTypeDef

```python
# GetPipelineDefinitionInputRequestTypeDef definition

class GetPipelineDefinitionInputRequestTypeDef(TypedDict):
    pipelineId: str,
    version: NotRequired[str],
```

## InstanceIdentityTypeDef

```python
# InstanceIdentityTypeDef definition

class InstanceIdentityTypeDef(TypedDict):
    document: NotRequired[str],
    signature: NotRequired[str],
```

## ListPipelinesInputRequestTypeDef

```python
# ListPipelinesInputRequestTypeDef definition

class ListPipelinesInputRequestTypeDef(TypedDict):
    marker: NotRequired[str],
```

## PipelineIdNameTypeDef

```python
# PipelineIdNameTypeDef definition

class PipelineIdNameTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
```

## OperatorTypeDef

```python
# OperatorTypeDef definition

class OperatorTypeDef(TypedDict):
    type: NotRequired[OperatorTypeType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: OperatorTypeType](./literals.md#operatortypetype) 
## ParameterAttributeTypeDef

```python
# ParameterAttributeTypeDef definition

class ParameterAttributeTypeDef(TypedDict):
    key: str,
    stringValue: str,
```

## ValidationErrorTypeDef

```python
# ValidationErrorTypeDef definition

class ValidationErrorTypeDef(TypedDict):
    id: NotRequired[str],
    errors: NotRequired[List[str]],
```

## ValidationWarningTypeDef

```python
# ValidationWarningTypeDef definition

class ValidationWarningTypeDef(TypedDict):
    id: NotRequired[str],
    warnings: NotRequired[List[str]],
```

## RemoveTagsInputRequestTypeDef

```python
# RemoveTagsInputRequestTypeDef definition

class RemoveTagsInputRequestTypeDef(TypedDict):
    pipelineId: str,
    tagKeys: Sequence[str],
```

## ReportTaskRunnerHeartbeatInputRequestTypeDef

```python
# ReportTaskRunnerHeartbeatInputRequestTypeDef definition

class ReportTaskRunnerHeartbeatInputRequestTypeDef(TypedDict):
    taskrunnerId: str,
    workerGroup: NotRequired[str],
    hostname: NotRequired[str],
```

## SetStatusInputRequestTypeDef

```python
# SetStatusInputRequestTypeDef definition

class SetStatusInputRequestTypeDef(TypedDict):
    pipelineId: str,
    objectIds: Sequence[str],
    status: str,
```

## SetTaskStatusInputRequestTypeDef

```python
# SetTaskStatusInputRequestTypeDef definition

class SetTaskStatusInputRequestTypeDef(TypedDict):
    taskId: str,
    taskStatus: TaskStatusType,  # (1)
    errorId: NotRequired[str],
    errorMessage: NotRequired[str],
    errorStackTrace: NotRequired[str],
```

1. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
## ActivatePipelineInputRequestTypeDef

```python
# ActivatePipelineInputRequestTypeDef definition

class ActivatePipelineInputRequestTypeDef(TypedDict):
    pipelineId: str,
    parameterValues: NotRequired[Sequence[ParameterValueTypeDef]],  # (1)
    startTimestamp: NotRequired[TimestampTypeDef],
```

1. See [:material-code-braces: ParameterValueTypeDef](./type_defs.md#parametervaluetypedef) 
## AddTagsInputRequestTypeDef

```python
# AddTagsInputRequestTypeDef definition

class AddTagsInputRequestTypeDef(TypedDict):
    pipelineId: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePipelineInputRequestTypeDef

```python
# CreatePipelineInputRequestTypeDef definition

class CreatePipelineInputRequestTypeDef(TypedDict):
    name: str,
    uniqueId: str,
    description: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePipelineOutputTypeDef

```python
# CreatePipelineOutputTypeDef definition

class CreatePipelineOutputTypeDef(TypedDict):
    pipelineId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EvaluateExpressionOutputTypeDef

```python
# EvaluateExpressionOutputTypeDef definition

class EvaluateExpressionOutputTypeDef(TypedDict):
    evaluatedExpression: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## QueryObjectsOutputTypeDef

```python
# QueryObjectsOutputTypeDef definition

class QueryObjectsOutputTypeDef(TypedDict):
    ids: List[str],
    marker: str,
    hasMoreResults: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReportTaskProgressOutputTypeDef

```python
# ReportTaskProgressOutputTypeDef definition

class ReportTaskProgressOutputTypeDef(TypedDict):
    canceled: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReportTaskRunnerHeartbeatOutputTypeDef

```python
# ReportTaskRunnerHeartbeatOutputTypeDef definition

class ReportTaskRunnerHeartbeatOutputTypeDef(TypedDict):
    terminate: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeObjectsInputDescribeObjectsPaginateTypeDef

```python
# DescribeObjectsInputDescribeObjectsPaginateTypeDef definition

class DescribeObjectsInputDescribeObjectsPaginateTypeDef(TypedDict):
    pipelineId: str,
    objectIds: Sequence[str],
    evaluateExpressions: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPipelinesInputListPipelinesPaginateTypeDef

```python
# ListPipelinesInputListPipelinesPaginateTypeDef definition

class ListPipelinesInputListPipelinesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## PipelineDescriptionTypeDef

```python
# PipelineDescriptionTypeDef definition

class PipelineDescriptionTypeDef(TypedDict):
    pipelineId: str,
    name: str,
    fields: List[FieldTypeDef],  # (1)
    description: NotRequired[str],
    tags: NotRequired[List[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: FieldTypeDef](./type_defs.md#fieldtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PipelineObjectOutputTypeDef

```python
# PipelineObjectOutputTypeDef definition

class PipelineObjectOutputTypeDef(TypedDict):
    id: str,
    name: str,
    fields: List[FieldTypeDef],  # (1)
```

1. See [:material-code-braces: FieldTypeDef](./type_defs.md#fieldtypedef) 
## PipelineObjectTypeDef

```python
# PipelineObjectTypeDef definition

class PipelineObjectTypeDef(TypedDict):
    id: str,
    name: str,
    fields: Sequence[FieldTypeDef],  # (1)
```

1. See [:material-code-braces: FieldTypeDef](./type_defs.md#fieldtypedef) 
## ReportTaskProgressInputRequestTypeDef

```python
# ReportTaskProgressInputRequestTypeDef definition

class ReportTaskProgressInputRequestTypeDef(TypedDict):
    taskId: str,
    fields: NotRequired[Sequence[FieldTypeDef]],  # (1)
```

1. See [:material-code-braces: FieldTypeDef](./type_defs.md#fieldtypedef) 
## PollForTaskInputRequestTypeDef

```python
# PollForTaskInputRequestTypeDef definition

class PollForTaskInputRequestTypeDef(TypedDict):
    workerGroup: str,
    hostname: NotRequired[str],
    instanceIdentity: NotRequired[InstanceIdentityTypeDef],  # (1)
```

1. See [:material-code-braces: InstanceIdentityTypeDef](./type_defs.md#instanceidentitytypedef) 
## ListPipelinesOutputTypeDef

```python
# ListPipelinesOutputTypeDef definition

class ListPipelinesOutputTypeDef(TypedDict):
    pipelineIdList: List[PipelineIdNameTypeDef],  # (1)
    marker: str,
    hasMoreResults: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineIdNameTypeDef](./type_defs.md#pipelineidnametypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SelectorTypeDef

```python
# SelectorTypeDef definition

class SelectorTypeDef(TypedDict):
    fieldName: NotRequired[str],
    operator: NotRequired[OperatorTypeDef],  # (1)
```

1. See [:material-code-braces: OperatorTypeDef](./type_defs.md#operatortypedef) 
## ParameterObjectOutputTypeDef

```python
# ParameterObjectOutputTypeDef definition

class ParameterObjectOutputTypeDef(TypedDict):
    id: str,
    attributes: List[ParameterAttributeTypeDef],  # (1)
```

1. See [:material-code-braces: ParameterAttributeTypeDef](./type_defs.md#parameterattributetypedef) 
## ParameterObjectTypeDef

```python
# ParameterObjectTypeDef definition

class ParameterObjectTypeDef(TypedDict):
    id: str,
    attributes: Sequence[ParameterAttributeTypeDef],  # (1)
```

1. See [:material-code-braces: ParameterAttributeTypeDef](./type_defs.md#parameterattributetypedef) 
## PutPipelineDefinitionOutputTypeDef

```python
# PutPipelineDefinitionOutputTypeDef definition

class PutPipelineDefinitionOutputTypeDef(TypedDict):
    validationErrors: List[ValidationErrorTypeDef],  # (1)
    validationWarnings: List[ValidationWarningTypeDef],  # (2)
    errored: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ValidationErrorTypeDef](./type_defs.md#validationerrortypedef) 
2. See [:material-code-braces: ValidationWarningTypeDef](./type_defs.md#validationwarningtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ValidatePipelineDefinitionOutputTypeDef

```python
# ValidatePipelineDefinitionOutputTypeDef definition

class ValidatePipelineDefinitionOutputTypeDef(TypedDict):
    validationErrors: List[ValidationErrorTypeDef],  # (1)
    validationWarnings: List[ValidationWarningTypeDef],  # (2)
    errored: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ValidationErrorTypeDef](./type_defs.md#validationerrortypedef) 
2. See [:material-code-braces: ValidationWarningTypeDef](./type_defs.md#validationwarningtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePipelinesOutputTypeDef

```python
# DescribePipelinesOutputTypeDef definition

class DescribePipelinesOutputTypeDef(TypedDict):
    pipelineDescriptionList: List[PipelineDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineDescriptionTypeDef](./type_defs.md#pipelinedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeObjectsOutputTypeDef

```python
# DescribeObjectsOutputTypeDef definition

class DescribeObjectsOutputTypeDef(TypedDict):
    pipelineObjects: List[PipelineObjectOutputTypeDef],  # (1)
    marker: str,
    hasMoreResults: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineObjectOutputTypeDef](./type_defs.md#pipelineobjectoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TaskObjectTypeDef

```python
# TaskObjectTypeDef definition

class TaskObjectTypeDef(TypedDict):
    taskId: NotRequired[str],
    pipelineId: NotRequired[str],
    attemptId: NotRequired[str],
    objects: NotRequired[Dict[str, PipelineObjectOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: PipelineObjectOutputTypeDef](./type_defs.md#pipelineobjectoutputtypedef) 
## QueryTypeDef

```python
# QueryTypeDef definition

class QueryTypeDef(TypedDict):
    selectors: NotRequired[Sequence[SelectorTypeDef]],  # (1)
```

1. See [:material-code-braces: SelectorTypeDef](./type_defs.md#selectortypedef) 
## GetPipelineDefinitionOutputTypeDef

```python
# GetPipelineDefinitionOutputTypeDef definition

class GetPipelineDefinitionOutputTypeDef(TypedDict):
    pipelineObjects: List[PipelineObjectOutputTypeDef],  # (1)
    parameterObjects: List[ParameterObjectOutputTypeDef],  # (2)
    parameterValues: List[ParameterValueTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: PipelineObjectOutputTypeDef](./type_defs.md#pipelineobjectoutputtypedef) 
2. See [:material-code-braces: ParameterObjectOutputTypeDef](./type_defs.md#parameterobjectoutputtypedef) 
3. See [:material-code-braces: ParameterValueTypeDef](./type_defs.md#parametervaluetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ValidatePipelineDefinitionInputRequestTypeDef

```python
# ValidatePipelineDefinitionInputRequestTypeDef definition

class ValidatePipelineDefinitionInputRequestTypeDef(TypedDict):
    pipelineId: str,
    pipelineObjects: Sequence[PipelineObjectTypeDef],  # (1)
    parameterObjects: NotRequired[Sequence[ParameterObjectTypeDef]],  # (2)
    parameterValues: NotRequired[Sequence[ParameterValueTypeDef]],  # (3)
```

1. See [:material-code-braces: PipelineObjectTypeDef](./type_defs.md#pipelineobjecttypedef) 
2. See [:material-code-braces: ParameterObjectTypeDef](./type_defs.md#parameterobjecttypedef) 
3. See [:material-code-braces: ParameterValueTypeDef](./type_defs.md#parametervaluetypedef) 
## PollForTaskOutputTypeDef

```python
# PollForTaskOutputTypeDef definition

class PollForTaskOutputTypeDef(TypedDict):
    taskObject: TaskObjectTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TaskObjectTypeDef](./type_defs.md#taskobjecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## QueryObjectsInputQueryObjectsPaginateTypeDef

```python
# QueryObjectsInputQueryObjectsPaginateTypeDef definition

class QueryObjectsInputQueryObjectsPaginateTypeDef(TypedDict):
    pipelineId: str,
    sphere: str,
    query: NotRequired[QueryTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: QueryTypeDef](./type_defs.md#querytypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## QueryObjectsInputRequestTypeDef

```python
# QueryObjectsInputRequestTypeDef definition

class QueryObjectsInputRequestTypeDef(TypedDict):
    pipelineId: str,
    sphere: str,
    query: NotRequired[QueryTypeDef],  # (1)
    marker: NotRequired[str],
    limit: NotRequired[int],
```

1. See [:material-code-braces: QueryTypeDef](./type_defs.md#querytypedef) 
## PutPipelineDefinitionInputRequestTypeDef

```python
# PutPipelineDefinitionInputRequestTypeDef definition

class PutPipelineDefinitionInputRequestTypeDef(TypedDict):
    pipelineId: str,
    pipelineObjects: Sequence[PipelineObjectUnionTypeDef],  # (1)
    parameterObjects: NotRequired[Sequence[ParameterObjectUnionTypeDef]],  # (2)
    parameterValues: NotRequired[Sequence[ParameterValueTypeDef]],  # (3)
```

1. See [:material-code-braces: PipelineObjectTypeDef](./type_defs.md#pipelineobjecttypedef) [:material-code-braces: PipelineObjectOutputTypeDef](./type_defs.md#pipelineobjectoutputtypedef) 
2. See [:material-code-braces: ParameterObjectTypeDef](./type_defs.md#parameterobjecttypedef) [:material-code-braces: ParameterObjectOutputTypeDef](./type_defs.md#parameterobjectoutputtypedef) 
3. See [:material-code-braces: ParameterValueTypeDef](./type_defs.md#parametervaluetypedef) 
