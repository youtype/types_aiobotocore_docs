# Type definitions

> [Index](../README.md) > [MigrationHubOrchestrator](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MigrationHubOrchestrator](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#migrationhuborchestrator)
    type annotations stubs module [types-aiobotocore-migrationhuborchestrator](https://pypi.org/project/types-aiobotocore-migrationhuborchestrator/).

## StepInputUnionTypeDef

```python
# StepInputUnionTypeDef definition

StepInputUnionTypeDef = Union[
    StepInputTypeDef,  # (1)
    StepInputOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: StepInputTypeDef](./type_defs.md#stepinputtypedef) 
2. See [:material-code-braces: StepInputOutputTypeDef](./type_defs.md#stepinputoutputtypedef) 

## WorkflowStepOutputUnionUnionTypeDef

```python
# WorkflowStepOutputUnionUnionTypeDef definition

WorkflowStepOutputUnionUnionTypeDef = Union[
    WorkflowStepOutputUnionTypeDef,  # (1)
    WorkflowStepOutputUnionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: WorkflowStepOutputUnionTypeDef](./type_defs.md#workflowstepoutputuniontypedef) 
2. See [:material-code-braces: WorkflowStepOutputUnionOutputTypeDef](./type_defs.md#workflowstepoutputunionoutputtypedef) 

## WorkflowStepUnionTypeDef

```python
# WorkflowStepUnionTypeDef definition

WorkflowStepUnionTypeDef = Union[
    WorkflowStepOutputTypeDef,  # (1)
    WorkflowStepExtraOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: WorkflowStepOutputTypeDef](./type_defs.md#workflowstepoutputtypedef) 
2. See [:material-code-braces: WorkflowStepExtraOutputTypeDef](./type_defs.md#workflowstepextraoutputtypedef) 



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

## StepInputOutputTypeDef

```python
# StepInputOutputTypeDef definition

class StepInputOutputTypeDef(TypedDict):
    integerValue: NotRequired[int],
    stringValue: NotRequired[str],
    listOfStringsValue: NotRequired[List[str]],
    mapOfStringValue: NotRequired[Dict[str, str]],
```

## TemplateSourceTypeDef

```python
# TemplateSourceTypeDef definition

class TemplateSourceTypeDef(TypedDict):
    workflowId: NotRequired[str],
```

## CreateWorkflowStepGroupRequestRequestTypeDef

```python
# CreateWorkflowStepGroupRequestRequestTypeDef definition

class CreateWorkflowStepGroupRequestRequestTypeDef(TypedDict):
    workflowId: str,
    name: str,
    description: NotRequired[str],
    next: NotRequired[Sequence[str]],
    previous: NotRequired[Sequence[str]],
```

## ToolTypeDef

```python
# ToolTypeDef definition

class ToolTypeDef(TypedDict):
    name: NotRequired[str],
    url: NotRequired[str],
```

## DeleteMigrationWorkflowRequestRequestTypeDef

```python
# DeleteMigrationWorkflowRequestRequestTypeDef definition

class DeleteMigrationWorkflowRequestRequestTypeDef(TypedDict):
    id: str,
```

## DeleteTemplateRequestRequestTypeDef

```python
# DeleteTemplateRequestRequestTypeDef definition

class DeleteTemplateRequestRequestTypeDef(TypedDict):
    id: str,
```

## DeleteWorkflowStepGroupRequestRequestTypeDef

```python
# DeleteWorkflowStepGroupRequestRequestTypeDef definition

class DeleteWorkflowStepGroupRequestRequestTypeDef(TypedDict):
    workflowId: str,
    id: str,
```

## DeleteWorkflowStepRequestRequestTypeDef

```python
# DeleteWorkflowStepRequestRequestTypeDef definition

class DeleteWorkflowStepRequestRequestTypeDef(TypedDict):
    id: str,
    stepGroupId: str,
    workflowId: str,
```

## GetMigrationWorkflowRequestRequestTypeDef

```python
# GetMigrationWorkflowRequestRequestTypeDef definition

class GetMigrationWorkflowRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetMigrationWorkflowTemplateRequestRequestTypeDef

```python
# GetMigrationWorkflowTemplateRequestRequestTypeDef definition

class GetMigrationWorkflowTemplateRequestRequestTypeDef(TypedDict):
    id: str,
```

## TemplateInputTypeDef

```python
# TemplateInputTypeDef definition

class TemplateInputTypeDef(TypedDict):
    inputName: NotRequired[str],
    dataType: NotRequired[DataTypeType],  # (1)
    required: NotRequired[bool],
```

1. See [:material-code-brackets: DataTypeType](./literals.md#datatypetype) 
## GetTemplateStepGroupRequestRequestTypeDef

```python
# GetTemplateStepGroupRequestRequestTypeDef definition

class GetTemplateStepGroupRequestRequestTypeDef(TypedDict):
    templateId: str,
    id: str,
```

## GetTemplateStepRequestRequestTypeDef

```python
# GetTemplateStepRequestRequestTypeDef definition

class GetTemplateStepRequestRequestTypeDef(TypedDict):
    id: str,
    templateId: str,
    stepGroupId: str,
```

## StepOutputTypeDef

```python
# StepOutputTypeDef definition

class StepOutputTypeDef(TypedDict):
    name: NotRequired[str],
    dataType: NotRequired[DataTypeType],  # (1)
    required: NotRequired[bool],
```

1. See [:material-code-brackets: DataTypeType](./literals.md#datatypetype) 
## GetWorkflowStepGroupRequestRequestTypeDef

```python
# GetWorkflowStepGroupRequestRequestTypeDef definition

class GetWorkflowStepGroupRequestRequestTypeDef(TypedDict):
    id: str,
    workflowId: str,
```

## GetWorkflowStepRequestRequestTypeDef

```python
# GetWorkflowStepRequestRequestTypeDef definition

class GetWorkflowStepRequestRequestTypeDef(TypedDict):
    workflowId: str,
    stepGroupId: str,
    id: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListMigrationWorkflowTemplatesRequestRequestTypeDef

```python
# ListMigrationWorkflowTemplatesRequestRequestTypeDef definition

class ListMigrationWorkflowTemplatesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    name: NotRequired[str],
```

## TemplateSummaryTypeDef

```python
# TemplateSummaryTypeDef definition

class TemplateSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    arn: NotRequired[str],
    description: NotRequired[str],
```

## ListMigrationWorkflowsRequestRequestTypeDef

```python
# ListMigrationWorkflowsRequestRequestTypeDef definition

class ListMigrationWorkflowsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    templateId: NotRequired[str],
    adsApplicationConfigurationName: NotRequired[str],
    status: NotRequired[MigrationWorkflowStatusEnumType],  # (1)
    name: NotRequired[str],
```

1. See [:material-code-brackets: MigrationWorkflowStatusEnumType](./literals.md#migrationworkflowstatusenumtype) 
## MigrationWorkflowSummaryTypeDef

```python
# MigrationWorkflowSummaryTypeDef definition

class MigrationWorkflowSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    templateId: NotRequired[str],
    adsApplicationConfigurationName: NotRequired[str],
    status: NotRequired[MigrationWorkflowStatusEnumType],  # (1)
    creationTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
    statusMessage: NotRequired[str],
    completedSteps: NotRequired[int],
    totalSteps: NotRequired[int],
```

1. See [:material-code-brackets: MigrationWorkflowStatusEnumType](./literals.md#migrationworkflowstatusenumtype) 
## ListPluginsRequestRequestTypeDef

```python
# ListPluginsRequestRequestTypeDef definition

class ListPluginsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## PluginSummaryTypeDef

```python
# PluginSummaryTypeDef definition

class PluginSummaryTypeDef(TypedDict):
    pluginId: NotRequired[str],
    hostname: NotRequired[str],
    status: NotRequired[PluginHealthType],  # (1)
    ipAddress: NotRequired[str],
    version: NotRequired[str],
    registeredTime: NotRequired[str],
```

1. See [:material-code-brackets: PluginHealthType](./literals.md#pluginhealthtype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListTemplateStepGroupsRequestRequestTypeDef

```python
# ListTemplateStepGroupsRequestRequestTypeDef definition

class ListTemplateStepGroupsRequestRequestTypeDef(TypedDict):
    templateId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## TemplateStepGroupSummaryTypeDef

```python
# TemplateStepGroupSummaryTypeDef definition

class TemplateStepGroupSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    previous: NotRequired[List[str]],
    next: NotRequired[List[str]],
```

## ListTemplateStepsRequestRequestTypeDef

```python
# ListTemplateStepsRequestRequestTypeDef definition

class ListTemplateStepsRequestRequestTypeDef(TypedDict):
    templateId: str,
    stepGroupId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## TemplateStepSummaryTypeDef

```python
# TemplateStepSummaryTypeDef definition

class TemplateStepSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    stepGroupId: NotRequired[str],
    templateId: NotRequired[str],
    name: NotRequired[str],
    stepActionType: NotRequired[StepActionTypeType],  # (1)
    targetType: NotRequired[TargetTypeType],  # (2)
    owner: NotRequired[OwnerType],  # (3)
    previous: NotRequired[List[str]],
    next: NotRequired[List[str]],
```

1. See [:material-code-brackets: StepActionTypeType](./literals.md#stepactiontypetype) 
2. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
3. See [:material-code-brackets: OwnerType](./literals.md#ownertype) 
## ListWorkflowStepGroupsRequestRequestTypeDef

```python
# ListWorkflowStepGroupsRequestRequestTypeDef definition

class ListWorkflowStepGroupsRequestRequestTypeDef(TypedDict):
    workflowId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## WorkflowStepGroupSummaryTypeDef

```python
# WorkflowStepGroupSummaryTypeDef definition

class WorkflowStepGroupSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    owner: NotRequired[OwnerType],  # (1)
    status: NotRequired[StepGroupStatusType],  # (2)
    previous: NotRequired[List[str]],
    next: NotRequired[List[str]],
```

1. See [:material-code-brackets: OwnerType](./literals.md#ownertype) 
2. See [:material-code-brackets: StepGroupStatusType](./literals.md#stepgroupstatustype) 
## ListWorkflowStepsRequestRequestTypeDef

```python
# ListWorkflowStepsRequestRequestTypeDef definition

class ListWorkflowStepsRequestRequestTypeDef(TypedDict):
    workflowId: str,
    stepGroupId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## WorkflowStepSummaryTypeDef

```python
# WorkflowStepSummaryTypeDef definition

class WorkflowStepSummaryTypeDef(TypedDict):
    stepId: NotRequired[str],
    name: NotRequired[str],
    stepActionType: NotRequired[StepActionTypeType],  # (1)
    owner: NotRequired[OwnerType],  # (2)
    previous: NotRequired[List[str]],
    next: NotRequired[List[str]],
    status: NotRequired[StepStatusType],  # (3)
    statusMessage: NotRequired[str],
    noOfSrvCompleted: NotRequired[int],
    noOfSrvFailed: NotRequired[int],
    totalNoOfSrv: NotRequired[int],
    description: NotRequired[str],
    scriptLocation: NotRequired[str],
```

1. See [:material-code-brackets: StepActionTypeType](./literals.md#stepactiontypetype) 
2. See [:material-code-brackets: OwnerType](./literals.md#ownertype) 
3. See [:material-code-brackets: StepStatusType](./literals.md#stepstatustype) 
## PlatformCommandTypeDef

```python
# PlatformCommandTypeDef definition

class PlatformCommandTypeDef(TypedDict):
    linux: NotRequired[str],
    windows: NotRequired[str],
```

## PlatformScriptKeyTypeDef

```python
# PlatformScriptKeyTypeDef definition

class PlatformScriptKeyTypeDef(TypedDict):
    linux: NotRequired[str],
    windows: NotRequired[str],
```

## RetryWorkflowStepRequestRequestTypeDef

```python
# RetryWorkflowStepRequestRequestTypeDef definition

class RetryWorkflowStepRequestRequestTypeDef(TypedDict):
    workflowId: str,
    stepGroupId: str,
    id: str,
```

## StartMigrationWorkflowRequestRequestTypeDef

```python
# StartMigrationWorkflowRequestRequestTypeDef definition

class StartMigrationWorkflowRequestRequestTypeDef(TypedDict):
    id: str,
```

## StepInputTypeDef

```python
# StepInputTypeDef definition

class StepInputTypeDef(TypedDict):
    integerValue: NotRequired[int],
    stringValue: NotRequired[str],
    listOfStringsValue: NotRequired[Sequence[str]],
    mapOfStringValue: NotRequired[Mapping[str, str]],
```

## StopMigrationWorkflowRequestRequestTypeDef

```python
# StopMigrationWorkflowRequestRequestTypeDef definition

class StopMigrationWorkflowRequestRequestTypeDef(TypedDict):
    id: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateTemplateRequestRequestTypeDef

```python
# UpdateTemplateRequestRequestTypeDef definition

class UpdateTemplateRequestRequestTypeDef(TypedDict):
    id: str,
    templateName: NotRequired[str],
    templateDescription: NotRequired[str],
    clientToken: NotRequired[str],
```

## UpdateWorkflowStepGroupRequestRequestTypeDef

```python
# UpdateWorkflowStepGroupRequestRequestTypeDef definition

class UpdateWorkflowStepGroupRequestRequestTypeDef(TypedDict):
    workflowId: str,
    id: str,
    name: NotRequired[str],
    description: NotRequired[str],
    next: NotRequired[Sequence[str]],
    previous: NotRequired[Sequence[str]],
```

## WorkflowStepOutputUnionOutputTypeDef

```python
# WorkflowStepOutputUnionOutputTypeDef definition

class WorkflowStepOutputUnionOutputTypeDef(TypedDict):
    integerValue: NotRequired[int],
    stringValue: NotRequired[str],
    listOfStringValue: NotRequired[List[str]],
```

## WorkflowStepOutputUnionTypeDef

```python
# WorkflowStepOutputUnionTypeDef definition

class WorkflowStepOutputUnionTypeDef(TypedDict):
    integerValue: NotRequired[int],
    stringValue: NotRequired[str],
    listOfStringValue: NotRequired[Sequence[str]],
```

## CreateTemplateResponseTypeDef

```python
# CreateTemplateResponseTypeDef definition

class CreateTemplateResponseTypeDef(TypedDict):
    templateId: str,
    templateArn: str,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkflowStepResponseTypeDef

```python
# CreateWorkflowStepResponseTypeDef definition

class CreateWorkflowStepResponseTypeDef(TypedDict):
    id: str,
    stepGroupId: str,
    workflowId: str,
    name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteMigrationWorkflowResponseTypeDef

```python
# DeleteMigrationWorkflowResponseTypeDef definition

class DeleteMigrationWorkflowResponseTypeDef(TypedDict):
    id: str,
    arn: str,
    status: MigrationWorkflowStatusEnumType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: MigrationWorkflowStatusEnumType](./literals.md#migrationworkflowstatusenumtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RetryWorkflowStepResponseTypeDef

```python
# RetryWorkflowStepResponseTypeDef definition

class RetryWorkflowStepResponseTypeDef(TypedDict):
    stepGroupId: str,
    workflowId: str,
    id: str,
    status: StepStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StepStatusType](./literals.md#stepstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMigrationWorkflowResponseTypeDef

```python
# StartMigrationWorkflowResponseTypeDef definition

class StartMigrationWorkflowResponseTypeDef(TypedDict):
    id: str,
    arn: str,
    status: MigrationWorkflowStatusEnumType,  # (1)
    statusMessage: str,
    lastStartTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: MigrationWorkflowStatusEnumType](./literals.md#migrationworkflowstatusenumtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopMigrationWorkflowResponseTypeDef

```python
# StopMigrationWorkflowResponseTypeDef definition

class StopMigrationWorkflowResponseTypeDef(TypedDict):
    id: str,
    arn: str,
    status: MigrationWorkflowStatusEnumType,  # (1)
    statusMessage: str,
    lastStopTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: MigrationWorkflowStatusEnumType](./literals.md#migrationworkflowstatusenumtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTemplateResponseTypeDef

```python
# UpdateTemplateResponseTypeDef definition

class UpdateTemplateResponseTypeDef(TypedDict):
    templateId: str,
    templateArn: str,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorkflowStepResponseTypeDef

```python
# UpdateWorkflowStepResponseTypeDef definition

class UpdateWorkflowStepResponseTypeDef(TypedDict):
    id: str,
    stepGroupId: str,
    workflowId: str,
    name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMigrationWorkflowResponseTypeDef

```python
# CreateMigrationWorkflowResponseTypeDef definition

class CreateMigrationWorkflowResponseTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    description: str,
    templateId: str,
    adsApplicationConfigurationId: str,
    workflowInputs: Dict[str, StepInputOutputTypeDef],  # (1)
    stepTargets: List[str],
    status: MigrationWorkflowStatusEnumType,  # (2)
    creationTime: datetime,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: StepInputOutputTypeDef](./type_defs.md#stepinputoutputtypedef) 
2. See [:material-code-brackets: MigrationWorkflowStatusEnumType](./literals.md#migrationworkflowstatusenumtype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMigrationWorkflowResponseTypeDef

```python
# UpdateMigrationWorkflowResponseTypeDef definition

class UpdateMigrationWorkflowResponseTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    description: str,
    templateId: str,
    adsApplicationConfigurationId: str,
    workflowInputs: Dict[str, StepInputOutputTypeDef],  # (1)
    stepTargets: List[str],
    status: MigrationWorkflowStatusEnumType,  # (2)
    creationTime: datetime,
    lastModifiedTime: datetime,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: StepInputOutputTypeDef](./type_defs.md#stepinputoutputtypedef) 
2. See [:material-code-brackets: MigrationWorkflowStatusEnumType](./literals.md#migrationworkflowstatusenumtype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTemplateRequestRequestTypeDef

```python
# CreateTemplateRequestRequestTypeDef definition

class CreateTemplateRequestRequestTypeDef(TypedDict):
    templateName: str,
    templateSource: TemplateSourceTypeDef,  # (1)
    templateDescription: NotRequired[str],
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: TemplateSourceTypeDef](./type_defs.md#templatesourcetypedef) 
## CreateWorkflowStepGroupResponseTypeDef

```python
# CreateWorkflowStepGroupResponseTypeDef definition

class CreateWorkflowStepGroupResponseTypeDef(TypedDict):
    workflowId: str,
    name: str,
    id: str,
    description: str,
    tools: List[ToolTypeDef],  # (1)
    next: List[str],
    previous: List[str],
    creationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ToolTypeDef](./type_defs.md#tooltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMigrationWorkflowResponseTypeDef

```python
# GetMigrationWorkflowResponseTypeDef definition

class GetMigrationWorkflowResponseTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    description: str,
    templateId: str,
    adsApplicationConfigurationId: str,
    adsApplicationName: str,
    status: MigrationWorkflowStatusEnumType,  # (1)
    statusMessage: str,
    creationTime: datetime,
    lastStartTime: datetime,
    lastStopTime: datetime,
    lastModifiedTime: datetime,
    endTime: datetime,
    tools: List[ToolTypeDef],  # (2)
    totalSteps: int,
    completedSteps: int,
    workflowInputs: Dict[str, StepInputOutputTypeDef],  # (3)
    tags: Dict[str, str],
    workflowBucket: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: MigrationWorkflowStatusEnumType](./literals.md#migrationworkflowstatusenumtype) 
2. See [:material-code-braces: ToolTypeDef](./type_defs.md#tooltypedef) 
3. See [:material-code-braces: StepInputOutputTypeDef](./type_defs.md#stepinputoutputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTemplateStepGroupResponseTypeDef

```python
# GetTemplateStepGroupResponseTypeDef definition

class GetTemplateStepGroupResponseTypeDef(TypedDict):
    templateId: str,
    id: str,
    name: str,
    description: str,
    status: StepGroupStatusType,  # (1)
    creationTime: datetime,
    lastModifiedTime: datetime,
    tools: List[ToolTypeDef],  # (2)
    previous: List[str],
    next: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: StepGroupStatusType](./literals.md#stepgroupstatustype) 
2. See [:material-code-braces: ToolTypeDef](./type_defs.md#tooltypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWorkflowStepGroupResponseTypeDef

```python
# GetWorkflowStepGroupResponseTypeDef definition

class GetWorkflowStepGroupResponseTypeDef(TypedDict):
    id: str,
    workflowId: str,
    name: str,
    description: str,
    status: StepGroupStatusType,  # (1)
    owner: OwnerType,  # (2)
    creationTime: datetime,
    lastModifiedTime: datetime,
    endTime: datetime,
    tools: List[ToolTypeDef],  # (3)
    previous: List[str],
    next: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: StepGroupStatusType](./literals.md#stepgroupstatustype) 
2. See [:material-code-brackets: OwnerType](./literals.md#ownertype) 
3. See [:material-code-braces: ToolTypeDef](./type_defs.md#tooltypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorkflowStepGroupResponseTypeDef

```python
# UpdateWorkflowStepGroupResponseTypeDef definition

class UpdateWorkflowStepGroupResponseTypeDef(TypedDict):
    workflowId: str,
    name: str,
    id: str,
    description: str,
    tools: List[ToolTypeDef],  # (1)
    next: List[str],
    previous: List[str],
    lastModifiedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ToolTypeDef](./type_defs.md#tooltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMigrationWorkflowTemplateResponseTypeDef

```python
# GetMigrationWorkflowTemplateResponseTypeDef definition

class GetMigrationWorkflowTemplateResponseTypeDef(TypedDict):
    id: str,
    templateArn: str,
    name: str,
    description: str,
    inputs: List[TemplateInputTypeDef],  # (1)
    tools: List[ToolTypeDef],  # (2)
    creationTime: datetime,
    owner: str,
    status: TemplateStatusType,  # (3)
    statusMessage: str,
    templateClass: str,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: TemplateInputTypeDef](./type_defs.md#templateinputtypedef) 
2. See [:material-code-braces: ToolTypeDef](./type_defs.md#tooltypedef) 
3. See [:material-code-brackets: TemplateStatusType](./literals.md#templatestatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMigrationWorkflowTemplatesRequestPaginateTypeDef

```python
# ListMigrationWorkflowTemplatesRequestPaginateTypeDef definition

class ListMigrationWorkflowTemplatesRequestPaginateTypeDef(TypedDict):
    name: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMigrationWorkflowsRequestPaginateTypeDef

```python
# ListMigrationWorkflowsRequestPaginateTypeDef definition

class ListMigrationWorkflowsRequestPaginateTypeDef(TypedDict):
    templateId: NotRequired[str],
    adsApplicationConfigurationName: NotRequired[str],
    status: NotRequired[MigrationWorkflowStatusEnumType],  # (1)
    name: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: MigrationWorkflowStatusEnumType](./literals.md#migrationworkflowstatusenumtype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPluginsRequestPaginateTypeDef

```python
# ListPluginsRequestPaginateTypeDef definition

class ListPluginsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTemplateStepGroupsRequestPaginateTypeDef

```python
# ListTemplateStepGroupsRequestPaginateTypeDef definition

class ListTemplateStepGroupsRequestPaginateTypeDef(TypedDict):
    templateId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTemplateStepsRequestPaginateTypeDef

```python
# ListTemplateStepsRequestPaginateTypeDef definition

class ListTemplateStepsRequestPaginateTypeDef(TypedDict):
    templateId: str,
    stepGroupId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkflowStepGroupsRequestPaginateTypeDef

```python
# ListWorkflowStepGroupsRequestPaginateTypeDef definition

class ListWorkflowStepGroupsRequestPaginateTypeDef(TypedDict):
    workflowId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkflowStepsRequestPaginateTypeDef

```python
# ListWorkflowStepsRequestPaginateTypeDef definition

class ListWorkflowStepsRequestPaginateTypeDef(TypedDict):
    workflowId: str,
    stepGroupId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMigrationWorkflowTemplatesResponseTypeDef

```python
# ListMigrationWorkflowTemplatesResponseTypeDef definition

class ListMigrationWorkflowTemplatesResponseTypeDef(TypedDict):
    templateSummary: List[TemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TemplateSummaryTypeDef](./type_defs.md#templatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMigrationWorkflowsResponseTypeDef

```python
# ListMigrationWorkflowsResponseTypeDef definition

class ListMigrationWorkflowsResponseTypeDef(TypedDict):
    migrationWorkflowSummary: List[MigrationWorkflowSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MigrationWorkflowSummaryTypeDef](./type_defs.md#migrationworkflowsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPluginsResponseTypeDef

```python
# ListPluginsResponseTypeDef definition

class ListPluginsResponseTypeDef(TypedDict):
    plugins: List[PluginSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PluginSummaryTypeDef](./type_defs.md#pluginsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTemplateStepGroupsResponseTypeDef

```python
# ListTemplateStepGroupsResponseTypeDef definition

class ListTemplateStepGroupsResponseTypeDef(TypedDict):
    templateStepGroupSummary: List[TemplateStepGroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TemplateStepGroupSummaryTypeDef](./type_defs.md#templatestepgroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTemplateStepsResponseTypeDef

```python
# ListTemplateStepsResponseTypeDef definition

class ListTemplateStepsResponseTypeDef(TypedDict):
    templateStepSummaryList: List[TemplateStepSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TemplateStepSummaryTypeDef](./type_defs.md#templatestepsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkflowStepGroupsResponseTypeDef

```python
# ListWorkflowStepGroupsResponseTypeDef definition

class ListWorkflowStepGroupsResponseTypeDef(TypedDict):
    workflowStepGroupsSummary: List[WorkflowStepGroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkflowStepGroupSummaryTypeDef](./type_defs.md#workflowstepgroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkflowStepsResponseTypeDef

```python
# ListWorkflowStepsResponseTypeDef definition

class ListWorkflowStepsResponseTypeDef(TypedDict):
    workflowStepsSummary: List[WorkflowStepSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkflowStepSummaryTypeDef](./type_defs.md#workflowstepsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StepAutomationConfigurationTypeDef

```python
# StepAutomationConfigurationTypeDef definition

class StepAutomationConfigurationTypeDef(TypedDict):
    scriptLocationS3Bucket: NotRequired[str],
    scriptLocationS3Key: NotRequired[PlatformScriptKeyTypeDef],  # (1)
    command: NotRequired[PlatformCommandTypeDef],  # (2)
    runEnvironment: NotRequired[RunEnvironmentType],  # (3)
    targetType: NotRequired[TargetTypeType],  # (4)
```

1. See [:material-code-braces: PlatformScriptKeyTypeDef](./type_defs.md#platformscriptkeytypedef) 
2. See [:material-code-braces: PlatformCommandTypeDef](./type_defs.md#platformcommandtypedef) 
3. See [:material-code-brackets: RunEnvironmentType](./literals.md#runenvironmenttype) 
4. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
## WorkflowStepAutomationConfigurationTypeDef

```python
# WorkflowStepAutomationConfigurationTypeDef definition

class WorkflowStepAutomationConfigurationTypeDef(TypedDict):
    scriptLocationS3Bucket: NotRequired[str],
    scriptLocationS3Key: NotRequired[PlatformScriptKeyTypeDef],  # (1)
    command: NotRequired[PlatformCommandTypeDef],  # (2)
    runEnvironment: NotRequired[RunEnvironmentType],  # (3)
    targetType: NotRequired[TargetTypeType],  # (4)
```

1. See [:material-code-braces: PlatformScriptKeyTypeDef](./type_defs.md#platformscriptkeytypedef) 
2. See [:material-code-braces: PlatformCommandTypeDef](./type_defs.md#platformcommandtypedef) 
3. See [:material-code-brackets: RunEnvironmentType](./literals.md#runenvironmenttype) 
4. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
## UpdateMigrationWorkflowRequestRequestTypeDef

```python
# UpdateMigrationWorkflowRequestRequestTypeDef definition

class UpdateMigrationWorkflowRequestRequestTypeDef(TypedDict):
    id: str,
    name: NotRequired[str],
    description: NotRequired[str],
    inputParameters: NotRequired[Mapping[str, StepInputTypeDef]],  # (1)
    stepTargets: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: StepInputTypeDef](./type_defs.md#stepinputtypedef) 
## WorkflowStepExtraOutputTypeDef

```python
# WorkflowStepExtraOutputTypeDef definition

class WorkflowStepExtraOutputTypeDef(TypedDict):
    name: NotRequired[str],
    dataType: NotRequired[DataTypeType],  # (1)
    required: NotRequired[bool],
    value: NotRequired[WorkflowStepOutputUnionOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: DataTypeType](./literals.md#datatypetype) 
2. See [:material-code-braces: WorkflowStepOutputUnionOutputTypeDef](./type_defs.md#workflowstepoutputunionoutputtypedef) 
## GetTemplateStepResponseTypeDef

```python
# GetTemplateStepResponseTypeDef definition

class GetTemplateStepResponseTypeDef(TypedDict):
    id: str,
    stepGroupId: str,
    templateId: str,
    name: str,
    description: str,
    stepActionType: StepActionTypeType,  # (1)
    creationTime: str,
    previous: List[str],
    next: List[str],
    outputs: List[StepOutputTypeDef],  # (2)
    stepAutomationConfiguration: StepAutomationConfigurationTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: StepActionTypeType](./literals.md#stepactiontypetype) 
2. See [:material-code-braces: StepOutputTypeDef](./type_defs.md#stepoutputtypedef) 
3. See [:material-code-braces: StepAutomationConfigurationTypeDef](./type_defs.md#stepautomationconfigurationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMigrationWorkflowRequestRequestTypeDef

```python
# CreateMigrationWorkflowRequestRequestTypeDef definition

class CreateMigrationWorkflowRequestRequestTypeDef(TypedDict):
    name: str,
    templateId: str,
    inputParameters: Mapping[str, StepInputUnionTypeDef],  # (1)
    description: NotRequired[str],
    applicationConfigurationId: NotRequired[str],
    stepTargets: NotRequired[Sequence[str]],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: StepInputTypeDef](./type_defs.md#stepinputtypedef) [:material-code-braces: StepInputOutputTypeDef](./type_defs.md#stepinputoutputtypedef) 
## GetWorkflowStepResponseTypeDef

```python
# GetWorkflowStepResponseTypeDef definition

class GetWorkflowStepResponseTypeDef(TypedDict):
    name: str,
    stepGroupId: str,
    workflowId: str,
    stepId: str,
    description: str,
    stepActionType: StepActionTypeType,  # (1)
    owner: OwnerType,  # (2)
    workflowStepAutomationConfiguration: WorkflowStepAutomationConfigurationTypeDef,  # (3)
    stepTarget: List[str],
    outputs: List[WorkflowStepExtraOutputTypeDef],  # (4)
    previous: List[str],
    next: List[str],
    status: StepStatusType,  # (5)
    statusMessage: str,
    scriptOutputLocation: str,
    creationTime: datetime,
    lastStartTime: datetime,
    endTime: datetime,
    noOfSrvCompleted: int,
    noOfSrvFailed: int,
    totalNoOfSrv: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: StepActionTypeType](./literals.md#stepactiontypetype) 
2. See [:material-code-brackets: OwnerType](./literals.md#ownertype) 
3. See [:material-code-braces: WorkflowStepAutomationConfigurationTypeDef](./type_defs.md#workflowstepautomationconfigurationtypedef) 
4. See [:material-code-braces: WorkflowStepExtraOutputTypeDef](./type_defs.md#workflowstepextraoutputtypedef) 
5. See [:material-code-brackets: StepStatusType](./literals.md#stepstatustype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkflowStepOutputTypeDef

```python
# WorkflowStepOutputTypeDef definition

class WorkflowStepOutputTypeDef(TypedDict):
    name: NotRequired[str],
    dataType: NotRequired[DataTypeType],  # (1)
    required: NotRequired[bool],
    value: NotRequired[WorkflowStepOutputUnionUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: DataTypeType](./literals.md#datatypetype) 
2. See [:material-code-braces: WorkflowStepOutputUnionTypeDef](./type_defs.md#workflowstepoutputuniontypedef) [:material-code-braces: WorkflowStepOutputUnionOutputTypeDef](./type_defs.md#workflowstepoutputunionoutputtypedef) 
## UpdateWorkflowStepRequestRequestTypeDef

```python
# UpdateWorkflowStepRequestRequestTypeDef definition

class UpdateWorkflowStepRequestRequestTypeDef(TypedDict):
    id: str,
    stepGroupId: str,
    workflowId: str,
    name: NotRequired[str],
    description: NotRequired[str],
    stepActionType: NotRequired[StepActionTypeType],  # (1)
    workflowStepAutomationConfiguration: NotRequired[WorkflowStepAutomationConfigurationTypeDef],  # (2)
    stepTarget: NotRequired[Sequence[str]],
    outputs: NotRequired[Sequence[WorkflowStepOutputTypeDef]],  # (3)
    previous: NotRequired[Sequence[str]],
    next: NotRequired[Sequence[str]],
    status: NotRequired[StepStatusType],  # (4)
```

1. See [:material-code-brackets: StepActionTypeType](./literals.md#stepactiontypetype) 
2. See [:material-code-braces: WorkflowStepAutomationConfigurationTypeDef](./type_defs.md#workflowstepautomationconfigurationtypedef) 
3. See [:material-code-braces: WorkflowStepOutputTypeDef](./type_defs.md#workflowstepoutputtypedef) 
4. See [:material-code-brackets: StepStatusType](./literals.md#stepstatustype) 
## CreateWorkflowStepRequestRequestTypeDef

```python
# CreateWorkflowStepRequestRequestTypeDef definition

class CreateWorkflowStepRequestRequestTypeDef(TypedDict):
    name: str,
    stepGroupId: str,
    workflowId: str,
    stepActionType: StepActionTypeType,  # (1)
    description: NotRequired[str],
    workflowStepAutomationConfiguration: NotRequired[WorkflowStepAutomationConfigurationTypeDef],  # (2)
    stepTarget: NotRequired[Sequence[str]],
    outputs: NotRequired[Sequence[WorkflowStepUnionTypeDef]],  # (3)
    previous: NotRequired[Sequence[str]],
    next: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: StepActionTypeType](./literals.md#stepactiontypetype) 
2. See [:material-code-braces: WorkflowStepAutomationConfigurationTypeDef](./type_defs.md#workflowstepautomationconfigurationtypedef) 
3. See [:material-code-braces: WorkflowStepOutputTypeDef](./type_defs.md#workflowstepoutputtypedef) [:material-code-braces: WorkflowStepExtraOutputTypeDef](./type_defs.md#workflowstepextraoutputtypedef) 
