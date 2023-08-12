# Type definitions

> [Index](../README.md) > [FIS](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [FIS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
    type annotations stubs module [types-aiobotocore-fis](https://pypi.org/project/types-aiobotocore-fis/).



## ActionParameterTypeDef

```python
# ActionParameterTypeDef definition

class ActionParameterTypeDef(TypedDict):
    description: NotRequired[str],
    required: NotRequired[bool],
```

## ActionTargetTypeDef

```python
# ActionTargetTypeDef definition

class ActionTargetTypeDef(TypedDict):
    resourceType: NotRequired[str],
```

## CreateExperimentTemplateActionInputTypeDef

```python
# CreateExperimentTemplateActionInputTypeDef definition

class CreateExperimentTemplateActionInputTypeDef(TypedDict):
    actionId: str,
    description: NotRequired[str],
    parameters: NotRequired[Mapping[str, str]],
    targets: NotRequired[Mapping[str, str]],
    startAfter: NotRequired[Sequence[str]],
```

## ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef

```python
# ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef definition

class ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef(TypedDict):
    logGroupArn: str,
```

## ExperimentTemplateS3LogConfigurationInputTypeDef

```python
# ExperimentTemplateS3LogConfigurationInputTypeDef definition

class ExperimentTemplateS3LogConfigurationInputTypeDef(TypedDict):
    bucketName: str,
    prefix: NotRequired[str],
```

## CreateExperimentTemplateStopConditionInputTypeDef

```python
# CreateExperimentTemplateStopConditionInputTypeDef definition

class CreateExperimentTemplateStopConditionInputTypeDef(TypedDict):
    source: str,
    value: NotRequired[str],
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

## ExperimentTemplateTargetInputFilterTypeDef

```python
# ExperimentTemplateTargetInputFilterTypeDef definition

class ExperimentTemplateTargetInputFilterTypeDef(TypedDict):
    path: str,
    values: Sequence[str],
```

## DeleteExperimentTemplateRequestRequestTypeDef

```python
# DeleteExperimentTemplateRequestRequestTypeDef definition

class DeleteExperimentTemplateRequestRequestTypeDef(TypedDict):
    id: str,
```

## ExperimentActionStateTypeDef

```python
# ExperimentActionStateTypeDef definition

class ExperimentActionStateTypeDef(TypedDict):
    status: NotRequired[ExperimentActionStatusType],  # (1)
    reason: NotRequired[str],
```

1. See [:material-code-brackets: ExperimentActionStatusType](./literals.md#experimentactionstatustype) 
## ExperimentCloudWatchLogsLogConfigurationTypeDef

```python
# ExperimentCloudWatchLogsLogConfigurationTypeDef definition

class ExperimentCloudWatchLogsLogConfigurationTypeDef(TypedDict):
    logGroupArn: NotRequired[str],
```

## ExperimentS3LogConfigurationTypeDef

```python
# ExperimentS3LogConfigurationTypeDef definition

class ExperimentS3LogConfigurationTypeDef(TypedDict):
    bucketName: NotRequired[str],
    prefix: NotRequired[str],
```

## ExperimentStateTypeDef

```python
# ExperimentStateTypeDef definition

class ExperimentStateTypeDef(TypedDict):
    status: NotRequired[ExperimentStatusType],  # (1)
    reason: NotRequired[str],
```

1. See [:material-code-brackets: ExperimentStatusType](./literals.md#experimentstatustype) 
## ExperimentStopConditionTypeDef

```python
# ExperimentStopConditionTypeDef definition

class ExperimentStopConditionTypeDef(TypedDict):
    source: NotRequired[str],
    value: NotRequired[str],
```

## ExperimentTargetFilterTypeDef

```python
# ExperimentTargetFilterTypeDef definition

class ExperimentTargetFilterTypeDef(TypedDict):
    path: NotRequired[str],
    values: NotRequired[List[str]],
```

## ExperimentTemplateActionTypeDef

```python
# ExperimentTemplateActionTypeDef definition

class ExperimentTemplateActionTypeDef(TypedDict):
    actionId: NotRequired[str],
    description: NotRequired[str],
    parameters: NotRequired[Dict[str, str]],
    targets: NotRequired[Dict[str, str]],
    startAfter: NotRequired[List[str]],
```

## ExperimentTemplateCloudWatchLogsLogConfigurationTypeDef

```python
# ExperimentTemplateCloudWatchLogsLogConfigurationTypeDef definition

class ExperimentTemplateCloudWatchLogsLogConfigurationTypeDef(TypedDict):
    logGroupArn: NotRequired[str],
```

## ExperimentTemplateS3LogConfigurationTypeDef

```python
# ExperimentTemplateS3LogConfigurationTypeDef definition

class ExperimentTemplateS3LogConfigurationTypeDef(TypedDict):
    bucketName: NotRequired[str],
    prefix: NotRequired[str],
```

## ExperimentTemplateStopConditionTypeDef

```python
# ExperimentTemplateStopConditionTypeDef definition

class ExperimentTemplateStopConditionTypeDef(TypedDict):
    source: NotRequired[str],
    value: NotRequired[str],
```

## ExperimentTemplateSummaryTypeDef

```python
# ExperimentTemplateSummaryTypeDef definition

class ExperimentTemplateSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    description: NotRequired[str],
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
```

## ExperimentTemplateTargetFilterTypeDef

```python
# ExperimentTemplateTargetFilterTypeDef definition

class ExperimentTemplateTargetFilterTypeDef(TypedDict):
    path: NotRequired[str],
    values: NotRequired[List[str]],
```

## GetActionRequestRequestTypeDef

```python
# GetActionRequestRequestTypeDef definition

class GetActionRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetExperimentRequestRequestTypeDef

```python
# GetExperimentRequestRequestTypeDef definition

class GetExperimentRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetExperimentTemplateRequestRequestTypeDef

```python
# GetExperimentTemplateRequestRequestTypeDef definition

class GetExperimentTemplateRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetTargetResourceTypeRequestRequestTypeDef

```python
# GetTargetResourceTypeRequestRequestTypeDef definition

class GetTargetResourceTypeRequestRequestTypeDef(TypedDict):
    resourceType: str,
```

## ListActionsRequestRequestTypeDef

```python
# ListActionsRequestRequestTypeDef definition

class ListActionsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListExperimentTemplatesRequestRequestTypeDef

```python
# ListExperimentTemplatesRequestRequestTypeDef definition

class ListExperimentTemplatesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListExperimentsRequestRequestTypeDef

```python
# ListExperimentsRequestRequestTypeDef definition

class ListExperimentsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListTargetResourceTypesRequestRequestTypeDef

```python
# ListTargetResourceTypesRequestRequestTypeDef definition

class ListTargetResourceTypesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## TargetResourceTypeSummaryTypeDef

```python
# TargetResourceTypeSummaryTypeDef definition

class TargetResourceTypeSummaryTypeDef(TypedDict):
    resourceType: NotRequired[str],
    description: NotRequired[str],
```

## StartExperimentRequestRequestTypeDef

```python
# StartExperimentRequestRequestTypeDef definition

class StartExperimentRequestRequestTypeDef(TypedDict):
    clientToken: str,
    experimentTemplateId: str,
    tags: NotRequired[Mapping[str, str]],
```

## StopExperimentRequestRequestTypeDef

```python
# StopExperimentRequestRequestTypeDef definition

class StopExperimentRequestRequestTypeDef(TypedDict):
    id: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## TargetResourceTypeParameterTypeDef

```python
# TargetResourceTypeParameterTypeDef definition

class TargetResourceTypeParameterTypeDef(TypedDict):
    description: NotRequired[str],
    required: NotRequired[bool],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: NotRequired[Sequence[str]],
```

## UpdateExperimentTemplateActionInputItemTypeDef

```python
# UpdateExperimentTemplateActionInputItemTypeDef definition

class UpdateExperimentTemplateActionInputItemTypeDef(TypedDict):
    actionId: NotRequired[str],
    description: NotRequired[str],
    parameters: NotRequired[Mapping[str, str]],
    targets: NotRequired[Mapping[str, str]],
    startAfter: NotRequired[Sequence[str]],
```

## UpdateExperimentTemplateStopConditionInputTypeDef

```python
# UpdateExperimentTemplateStopConditionInputTypeDef definition

class UpdateExperimentTemplateStopConditionInputTypeDef(TypedDict):
    source: str,
    value: NotRequired[str],
```

## ActionSummaryTypeDef

```python
# ActionSummaryTypeDef definition

class ActionSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    description: NotRequired[str],
    targets: NotRequired[Dict[str, ActionTargetTypeDef]],  # (1)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ActionTargetTypeDef](./type_defs.md#actiontargettypedef) 
## ActionTypeDef

```python
# ActionTypeDef definition

class ActionTypeDef(TypedDict):
    id: NotRequired[str],
    description: NotRequired[str],
    parameters: NotRequired[Dict[str, ActionParameterTypeDef]],  # (1)
    targets: NotRequired[Dict[str, ActionTargetTypeDef]],  # (2)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ActionParameterTypeDef](./type_defs.md#actionparametertypedef) 
2. See [:material-code-braces: ActionTargetTypeDef](./type_defs.md#actiontargettypedef) 
## CreateExperimentTemplateLogConfigurationInputTypeDef

```python
# CreateExperimentTemplateLogConfigurationInputTypeDef definition

class CreateExperimentTemplateLogConfigurationInputTypeDef(TypedDict):
    logSchemaVersion: int,
    cloudWatchLogsConfiguration: NotRequired[ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef],  # (1)
    s3Configuration: NotRequired[ExperimentTemplateS3LogConfigurationInputTypeDef],  # (2)
```

1. See [:material-code-braces: ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef](./type_defs.md#experimenttemplatecloudwatchlogslogconfigurationinputtypedef) 
2. See [:material-code-braces: ExperimentTemplateS3LogConfigurationInputTypeDef](./type_defs.md#experimenttemplates3logconfigurationinputtypedef) 
## UpdateExperimentTemplateLogConfigurationInputTypeDef

```python
# UpdateExperimentTemplateLogConfigurationInputTypeDef definition

class UpdateExperimentTemplateLogConfigurationInputTypeDef(TypedDict):
    cloudWatchLogsConfiguration: NotRequired[ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef],  # (1)
    s3Configuration: NotRequired[ExperimentTemplateS3LogConfigurationInputTypeDef],  # (2)
    logSchemaVersion: NotRequired[int],
```

1. See [:material-code-braces: ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef](./type_defs.md#experimenttemplatecloudwatchlogslogconfigurationinputtypedef) 
2. See [:material-code-braces: ExperimentTemplateS3LogConfigurationInputTypeDef](./type_defs.md#experimenttemplates3logconfigurationinputtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateExperimentTemplateTargetInputTypeDef

```python
# CreateExperimentTemplateTargetInputTypeDef definition

class CreateExperimentTemplateTargetInputTypeDef(TypedDict):
    resourceType: str,
    selectionMode: str,
    resourceArns: NotRequired[Sequence[str]],
    resourceTags: NotRequired[Mapping[str, str]],
    filters: NotRequired[Sequence[ExperimentTemplateTargetInputFilterTypeDef]],  # (1)
    parameters: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ExperimentTemplateTargetInputFilterTypeDef](./type_defs.md#experimenttemplatetargetinputfiltertypedef) 
## UpdateExperimentTemplateTargetInputTypeDef

```python
# UpdateExperimentTemplateTargetInputTypeDef definition

class UpdateExperimentTemplateTargetInputTypeDef(TypedDict):
    resourceType: str,
    selectionMode: str,
    resourceArns: NotRequired[Sequence[str]],
    resourceTags: NotRequired[Mapping[str, str]],
    filters: NotRequired[Sequence[ExperimentTemplateTargetInputFilterTypeDef]],  # (1)
    parameters: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ExperimentTemplateTargetInputFilterTypeDef](./type_defs.md#experimenttemplatetargetinputfiltertypedef) 
## ExperimentActionTypeDef

```python
# ExperimentActionTypeDef definition

class ExperimentActionTypeDef(TypedDict):
    actionId: NotRequired[str],
    description: NotRequired[str],
    parameters: NotRequired[Dict[str, str]],
    targets: NotRequired[Dict[str, str]],
    startAfter: NotRequired[List[str]],
    state: NotRequired[ExperimentActionStateTypeDef],  # (1)
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
```

1. See [:material-code-braces: ExperimentActionStateTypeDef](./type_defs.md#experimentactionstatetypedef) 
## ExperimentLogConfigurationTypeDef

```python
# ExperimentLogConfigurationTypeDef definition

class ExperimentLogConfigurationTypeDef(TypedDict):
    cloudWatchLogsConfiguration: NotRequired[ExperimentCloudWatchLogsLogConfigurationTypeDef],  # (1)
    s3Configuration: NotRequired[ExperimentS3LogConfigurationTypeDef],  # (2)
    logSchemaVersion: NotRequired[int],
```

1. See [:material-code-braces: ExperimentCloudWatchLogsLogConfigurationTypeDef](./type_defs.md#experimentcloudwatchlogslogconfigurationtypedef) 
2. See [:material-code-braces: ExperimentS3LogConfigurationTypeDef](./type_defs.md#experiments3logconfigurationtypedef) 
## ExperimentSummaryTypeDef

```python
# ExperimentSummaryTypeDef definition

class ExperimentSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    experimentTemplateId: NotRequired[str],
    state: NotRequired[ExperimentStateTypeDef],  # (1)
    creationTime: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ExperimentStateTypeDef](./type_defs.md#experimentstatetypedef) 
## ExperimentTargetTypeDef

```python
# ExperimentTargetTypeDef definition

class ExperimentTargetTypeDef(TypedDict):
    resourceType: NotRequired[str],
    resourceArns: NotRequired[List[str]],
    resourceTags: NotRequired[Dict[str, str]],
    filters: NotRequired[List[ExperimentTargetFilterTypeDef]],  # (1)
    selectionMode: NotRequired[str],
    parameters: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ExperimentTargetFilterTypeDef](./type_defs.md#experimenttargetfiltertypedef) 
## ExperimentTemplateLogConfigurationTypeDef

```python
# ExperimentTemplateLogConfigurationTypeDef definition

class ExperimentTemplateLogConfigurationTypeDef(TypedDict):
    cloudWatchLogsConfiguration: NotRequired[ExperimentTemplateCloudWatchLogsLogConfigurationTypeDef],  # (1)
    s3Configuration: NotRequired[ExperimentTemplateS3LogConfigurationTypeDef],  # (2)
    logSchemaVersion: NotRequired[int],
```

1. See [:material-code-braces: ExperimentTemplateCloudWatchLogsLogConfigurationTypeDef](./type_defs.md#experimenttemplatecloudwatchlogslogconfigurationtypedef) 
2. See [:material-code-braces: ExperimentTemplateS3LogConfigurationTypeDef](./type_defs.md#experimenttemplates3logconfigurationtypedef) 
## ListExperimentTemplatesResponseTypeDef

```python
# ListExperimentTemplatesResponseTypeDef definition

class ListExperimentTemplatesResponseTypeDef(TypedDict):
    experimentTemplates: List[ExperimentTemplateSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentTemplateSummaryTypeDef](./type_defs.md#experimenttemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExperimentTemplateTargetTypeDef

```python
# ExperimentTemplateTargetTypeDef definition

class ExperimentTemplateTargetTypeDef(TypedDict):
    resourceType: NotRequired[str],
    resourceArns: NotRequired[List[str]],
    resourceTags: NotRequired[Dict[str, str]],
    filters: NotRequired[List[ExperimentTemplateTargetFilterTypeDef]],  # (1)
    selectionMode: NotRequired[str],
    parameters: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ExperimentTemplateTargetFilterTypeDef](./type_defs.md#experimenttemplatetargetfiltertypedef) 
## ListTargetResourceTypesResponseTypeDef

```python
# ListTargetResourceTypesResponseTypeDef definition

class ListTargetResourceTypesResponseTypeDef(TypedDict):
    targetResourceTypes: List[TargetResourceTypeSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TargetResourceTypeSummaryTypeDef](./type_defs.md#targetresourcetypesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TargetResourceTypeTypeDef

```python
# TargetResourceTypeTypeDef definition

class TargetResourceTypeTypeDef(TypedDict):
    resourceType: NotRequired[str],
    description: NotRequired[str],
    parameters: NotRequired[Dict[str, TargetResourceTypeParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: TargetResourceTypeParameterTypeDef](./type_defs.md#targetresourcetypeparametertypedef) 
## ListActionsResponseTypeDef

```python
# ListActionsResponseTypeDef definition

class ListActionsResponseTypeDef(TypedDict):
    actions: List[ActionSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActionSummaryTypeDef](./type_defs.md#actionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetActionResponseTypeDef

```python
# GetActionResponseTypeDef definition

class GetActionResponseTypeDef(TypedDict):
    action: ActionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateExperimentTemplateRequestRequestTypeDef

```python
# CreateExperimentTemplateRequestRequestTypeDef definition

class CreateExperimentTemplateRequestRequestTypeDef(TypedDict):
    clientToken: str,
    description: str,
    stopConditions: Sequence[CreateExperimentTemplateStopConditionInputTypeDef],  # (1)
    actions: Mapping[str, CreateExperimentTemplateActionInputTypeDef],  # (2)
    roleArn: str,
    targets: NotRequired[Mapping[str, CreateExperimentTemplateTargetInputTypeDef]],  # (3)
    tags: NotRequired[Mapping[str, str]],
    logConfiguration: NotRequired[CreateExperimentTemplateLogConfigurationInputTypeDef],  # (4)
```

1. See [:material-code-braces: CreateExperimentTemplateStopConditionInputTypeDef](./type_defs.md#createexperimenttemplatestopconditioninputtypedef) 
2. See [:material-code-braces: CreateExperimentTemplateActionInputTypeDef](./type_defs.md#createexperimenttemplateactioninputtypedef) 
3. See [:material-code-braces: CreateExperimentTemplateTargetInputTypeDef](./type_defs.md#createexperimenttemplatetargetinputtypedef) 
4. See [:material-code-braces: CreateExperimentTemplateLogConfigurationInputTypeDef](./type_defs.md#createexperimenttemplatelogconfigurationinputtypedef) 
## UpdateExperimentTemplateRequestRequestTypeDef

```python
# UpdateExperimentTemplateRequestRequestTypeDef definition

class UpdateExperimentTemplateRequestRequestTypeDef(TypedDict):
    id: str,
    description: NotRequired[str],
    stopConditions: NotRequired[Sequence[UpdateExperimentTemplateStopConditionInputTypeDef]],  # (1)
    targets: NotRequired[Mapping[str, UpdateExperimentTemplateTargetInputTypeDef]],  # (2)
    actions: NotRequired[Mapping[str, UpdateExperimentTemplateActionInputItemTypeDef]],  # (3)
    roleArn: NotRequired[str],
    logConfiguration: NotRequired[UpdateExperimentTemplateLogConfigurationInputTypeDef],  # (4)
```

1. See [:material-code-braces: UpdateExperimentTemplateStopConditionInputTypeDef](./type_defs.md#updateexperimenttemplatestopconditioninputtypedef) 
2. See [:material-code-braces: UpdateExperimentTemplateTargetInputTypeDef](./type_defs.md#updateexperimenttemplatetargetinputtypedef) 
3. See [:material-code-braces: UpdateExperimentTemplateActionInputItemTypeDef](./type_defs.md#updateexperimenttemplateactioninputitemtypedef) 
4. See [:material-code-braces: UpdateExperimentTemplateLogConfigurationInputTypeDef](./type_defs.md#updateexperimenttemplatelogconfigurationinputtypedef) 
## ListExperimentsResponseTypeDef

```python
# ListExperimentsResponseTypeDef definition

class ListExperimentsResponseTypeDef(TypedDict):
    experiments: List[ExperimentSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentSummaryTypeDef](./type_defs.md#experimentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExperimentTypeDef

```python
# ExperimentTypeDef definition

class ExperimentTypeDef(TypedDict):
    id: NotRequired[str],
    experimentTemplateId: NotRequired[str],
    roleArn: NotRequired[str],
    state: NotRequired[ExperimentStateTypeDef],  # (1)
    targets: NotRequired[Dict[str, ExperimentTargetTypeDef]],  # (2)
    actions: NotRequired[Dict[str, ExperimentActionTypeDef]],  # (3)
    stopConditions: NotRequired[List[ExperimentStopConditionTypeDef]],  # (4)
    creationTime: NotRequired[datetime],
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
    logConfiguration: NotRequired[ExperimentLogConfigurationTypeDef],  # (5)
```

1. See [:material-code-braces: ExperimentStateTypeDef](./type_defs.md#experimentstatetypedef) 
2. See [:material-code-braces: ExperimentTargetTypeDef](./type_defs.md#experimenttargettypedef) 
3. See [:material-code-braces: ExperimentActionTypeDef](./type_defs.md#experimentactiontypedef) 
4. See [:material-code-braces: ExperimentStopConditionTypeDef](./type_defs.md#experimentstopconditiontypedef) 
5. See [:material-code-braces: ExperimentLogConfigurationTypeDef](./type_defs.md#experimentlogconfigurationtypedef) 
## ExperimentTemplateTypeDef

```python
# ExperimentTemplateTypeDef definition

class ExperimentTemplateTypeDef(TypedDict):
    id: NotRequired[str],
    description: NotRequired[str],
    targets: NotRequired[Dict[str, ExperimentTemplateTargetTypeDef]],  # (1)
    actions: NotRequired[Dict[str, ExperimentTemplateActionTypeDef]],  # (2)
    stopConditions: NotRequired[List[ExperimentTemplateStopConditionTypeDef]],  # (3)
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
    roleArn: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    logConfiguration: NotRequired[ExperimentTemplateLogConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: ExperimentTemplateTargetTypeDef](./type_defs.md#experimenttemplatetargettypedef) 
2. See [:material-code-braces: ExperimentTemplateActionTypeDef](./type_defs.md#experimenttemplateactiontypedef) 
3. See [:material-code-braces: ExperimentTemplateStopConditionTypeDef](./type_defs.md#experimenttemplatestopconditiontypedef) 
4. See [:material-code-braces: ExperimentTemplateLogConfigurationTypeDef](./type_defs.md#experimenttemplatelogconfigurationtypedef) 
## GetTargetResourceTypeResponseTypeDef

```python
# GetTargetResourceTypeResponseTypeDef definition

class GetTargetResourceTypeResponseTypeDef(TypedDict):
    targetResourceType: TargetResourceTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TargetResourceTypeTypeDef](./type_defs.md#targetresourcetypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetExperimentResponseTypeDef

```python
# GetExperimentResponseTypeDef definition

class GetExperimentResponseTypeDef(TypedDict):
    experiment: ExperimentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentTypeDef](./type_defs.md#experimenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartExperimentResponseTypeDef

```python
# StartExperimentResponseTypeDef definition

class StartExperimentResponseTypeDef(TypedDict):
    experiment: ExperimentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentTypeDef](./type_defs.md#experimenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopExperimentResponseTypeDef

```python
# StopExperimentResponseTypeDef definition

class StopExperimentResponseTypeDef(TypedDict):
    experiment: ExperimentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentTypeDef](./type_defs.md#experimenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateExperimentTemplateResponseTypeDef

```python
# CreateExperimentTemplateResponseTypeDef definition

class CreateExperimentTemplateResponseTypeDef(TypedDict):
    experimentTemplate: ExperimentTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentTemplateTypeDef](./type_defs.md#experimenttemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteExperimentTemplateResponseTypeDef

```python
# DeleteExperimentTemplateResponseTypeDef definition

class DeleteExperimentTemplateResponseTypeDef(TypedDict):
    experimentTemplate: ExperimentTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentTemplateTypeDef](./type_defs.md#experimenttemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetExperimentTemplateResponseTypeDef

```python
# GetExperimentTemplateResponseTypeDef definition

class GetExperimentTemplateResponseTypeDef(TypedDict):
    experimentTemplate: ExperimentTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentTemplateTypeDef](./type_defs.md#experimenttemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateExperimentTemplateResponseTypeDef

```python
# UpdateExperimentTemplateResponseTypeDef definition

class UpdateExperimentTemplateResponseTypeDef(TypedDict):
    experimentTemplate: ExperimentTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentTemplateTypeDef](./type_defs.md#experimenttemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
