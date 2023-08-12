# Type definitions

> [Index](../README.md) > [CodePipeline](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CodePipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
    type annotations stubs module [types-aiobotocore-codepipeline](https://pypi.org/project/types-aiobotocore-codepipeline/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AWSSessionCredentialsTypeDef

```python
# AWSSessionCredentialsTypeDef definition

class AWSSessionCredentialsTypeDef(TypedDict):
    accessKeyId: str,
    secretAccessKey: str,
    sessionToken: str,
```

## AcknowledgeJobInputRequestTypeDef

```python
# AcknowledgeJobInputRequestTypeDef definition

class AcknowledgeJobInputRequestTypeDef(TypedDict):
    jobId: str,
    nonce: str,
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

## AcknowledgeThirdPartyJobInputRequestTypeDef

```python
# AcknowledgeThirdPartyJobInputRequestTypeDef definition

class AcknowledgeThirdPartyJobInputRequestTypeDef(TypedDict):
    jobId: str,
    nonce: str,
    clientToken: str,
```

## ActionConfigurationPropertyTypeDef

```python
# ActionConfigurationPropertyTypeDef definition

class ActionConfigurationPropertyTypeDef(TypedDict):
    name: str,
    required: bool,
    key: bool,
    secret: bool,
    queryable: NotRequired[bool],
    description: NotRequired[str],
    type: NotRequired[ActionConfigurationPropertyTypeType],  # (1)
```

1. See [:material-code-brackets: ActionConfigurationPropertyTypeType](./literals.md#actionconfigurationpropertytypetype) 
## ActionConfigurationTypeDef

```python
# ActionConfigurationTypeDef definition

class ActionConfigurationTypeDef(TypedDict):
    configuration: NotRequired[Dict[str, str]],
```

## ActionContextTypeDef

```python
# ActionContextTypeDef definition

class ActionContextTypeDef(TypedDict):
    name: NotRequired[str],
    actionExecutionId: NotRequired[str],
```

## ActionTypeIdTypeDef

```python
# ActionTypeIdTypeDef definition

class ActionTypeIdTypeDef(TypedDict):
    category: ActionCategoryType,  # (1)
    owner: ActionOwnerType,  # (2)
    provider: str,
    version: str,
```

1. See [:material-code-brackets: ActionCategoryType](./literals.md#actioncategorytype) 
2. See [:material-code-brackets: ActionOwnerType](./literals.md#actionownertype) 
## InputArtifactTypeDef

```python
# InputArtifactTypeDef definition

class InputArtifactTypeDef(TypedDict):
    name: str,
```

## OutputArtifactTypeDef

```python
# OutputArtifactTypeDef definition

class OutputArtifactTypeDef(TypedDict):
    name: str,
```

## ActionExecutionFilterTypeDef

```python
# ActionExecutionFilterTypeDef definition

class ActionExecutionFilterTypeDef(TypedDict):
    pipelineExecutionId: NotRequired[str],
```

## ActionExecutionResultTypeDef

```python
# ActionExecutionResultTypeDef definition

class ActionExecutionResultTypeDef(TypedDict):
    externalExecutionId: NotRequired[str],
    externalExecutionSummary: NotRequired[str],
    externalExecutionUrl: NotRequired[str],
```

## ErrorDetailsTypeDef

```python
# ErrorDetailsTypeDef definition

class ErrorDetailsTypeDef(TypedDict):
    code: NotRequired[str],
    message: NotRequired[str],
```

## ActionRevisionTypeDef

```python
# ActionRevisionTypeDef definition

class ActionRevisionTypeDef(TypedDict):
    revisionId: str,
    revisionChangeId: str,
    created: datetime,
```

## ActionTypeArtifactDetailsTypeDef

```python
# ActionTypeArtifactDetailsTypeDef definition

class ActionTypeArtifactDetailsTypeDef(TypedDict):
    minimumCount: int,
    maximumCount: int,
```

## ActionTypeIdentifierTypeDef

```python
# ActionTypeIdentifierTypeDef definition

class ActionTypeIdentifierTypeDef(TypedDict):
    category: ActionCategoryType,  # (1)
    owner: str,
    provider: str,
    version: str,
```

1. See [:material-code-brackets: ActionCategoryType](./literals.md#actioncategorytype) 
## ActionTypePermissionsTypeDef

```python
# ActionTypePermissionsTypeDef definition

class ActionTypePermissionsTypeDef(TypedDict):
    allowedAccounts: List[str],
```

## ActionTypePropertyTypeDef

```python
# ActionTypePropertyTypeDef definition

class ActionTypePropertyTypeDef(TypedDict):
    name: str,
    optional: bool,
    key: bool,
    noEcho: bool,
    queryable: NotRequired[bool],
    description: NotRequired[str],
```

## ActionTypeUrlsTypeDef

```python
# ActionTypeUrlsTypeDef definition

class ActionTypeUrlsTypeDef(TypedDict):
    configurationUrl: NotRequired[str],
    entityUrlTemplate: NotRequired[str],
    executionUrlTemplate: NotRequired[str],
    revisionUrlTemplate: NotRequired[str],
```

## ActionTypeSettingsTypeDef

```python
# ActionTypeSettingsTypeDef definition

class ActionTypeSettingsTypeDef(TypedDict):
    thirdPartyConfigurationUrl: NotRequired[str],
    entityUrlTemplate: NotRequired[str],
    executionUrlTemplate: NotRequired[str],
    revisionUrlTemplate: NotRequired[str],
```

## ArtifactDetailsTypeDef

```python
# ArtifactDetailsTypeDef definition

class ArtifactDetailsTypeDef(TypedDict):
    minimumCount: int,
    maximumCount: int,
```

## ApprovalResultTypeDef

```python
# ApprovalResultTypeDef definition

class ApprovalResultTypeDef(TypedDict):
    summary: str,
    status: ApprovalStatusType,  # (1)
```

1. See [:material-code-brackets: ApprovalStatusType](./literals.md#approvalstatustype) 
## S3LocationTypeDef

```python
# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    bucket: NotRequired[str],
    key: NotRequired[str],
```

## S3ArtifactLocationTypeDef

```python
# S3ArtifactLocationTypeDef definition

class S3ArtifactLocationTypeDef(TypedDict):
    bucketName: str,
    objectKey: str,
```

## ArtifactRevisionTypeDef

```python
# ArtifactRevisionTypeDef definition

class ArtifactRevisionTypeDef(TypedDict):
    name: NotRequired[str],
    revisionId: NotRequired[str],
    revisionChangeIdentifier: NotRequired[str],
    revisionSummary: NotRequired[str],
    created: NotRequired[datetime],
    revisionUrl: NotRequired[str],
```

## EncryptionKeyTypeDef

```python
# EncryptionKeyTypeDef definition

class EncryptionKeyTypeDef(TypedDict):
    id: str,
    type: EncryptionKeyTypeType,  # (1)
```

1. See [:material-code-brackets: EncryptionKeyTypeType](./literals.md#encryptionkeytypetype) 
## BlockerDeclarationTypeDef

```python
# BlockerDeclarationTypeDef definition

class BlockerDeclarationTypeDef(TypedDict):
    name: str,
    type: BlockerTypeType,  # (1)
```

1. See [:material-code-brackets: BlockerTypeType](./literals.md#blockertypetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
```

## DeleteCustomActionTypeInputRequestTypeDef

```python
# DeleteCustomActionTypeInputRequestTypeDef definition

class DeleteCustomActionTypeInputRequestTypeDef(TypedDict):
    category: ActionCategoryType,  # (1)
    provider: str,
    version: str,
```

1. See [:material-code-brackets: ActionCategoryType](./literals.md#actioncategorytype) 
## DeletePipelineInputRequestTypeDef

```python
# DeletePipelineInputRequestTypeDef definition

class DeletePipelineInputRequestTypeDef(TypedDict):
    name: str,
```

## DeleteWebhookInputRequestTypeDef

```python
# DeleteWebhookInputRequestTypeDef definition

class DeleteWebhookInputRequestTypeDef(TypedDict):
    name: str,
```

## DeregisterWebhookWithThirdPartyInputRequestTypeDef

```python
# DeregisterWebhookWithThirdPartyInputRequestTypeDef definition

class DeregisterWebhookWithThirdPartyInputRequestTypeDef(TypedDict):
    webhookName: NotRequired[str],
```

## DisableStageTransitionInputRequestTypeDef

```python
# DisableStageTransitionInputRequestTypeDef definition

class DisableStageTransitionInputRequestTypeDef(TypedDict):
    pipelineName: str,
    stageName: str,
    transitionType: StageTransitionTypeType,  # (1)
    reason: str,
```

1. See [:material-code-brackets: StageTransitionTypeType](./literals.md#stagetransitiontypetype) 
## EnableStageTransitionInputRequestTypeDef

```python
# EnableStageTransitionInputRequestTypeDef definition

class EnableStageTransitionInputRequestTypeDef(TypedDict):
    pipelineName: str,
    stageName: str,
    transitionType: StageTransitionTypeType,  # (1)
```

1. See [:material-code-brackets: StageTransitionTypeType](./literals.md#stagetransitiontypetype) 
## ExecutionDetailsTypeDef

```python
# ExecutionDetailsTypeDef definition

class ExecutionDetailsTypeDef(TypedDict):
    summary: NotRequired[str],
    externalExecutionId: NotRequired[str],
    percentComplete: NotRequired[int],
```

## ExecutionTriggerTypeDef

```python
# ExecutionTriggerTypeDef definition

class ExecutionTriggerTypeDef(TypedDict):
    triggerType: NotRequired[TriggerTypeType],  # (1)
    triggerDetail: NotRequired[str],
```

1. See [:material-code-brackets: TriggerTypeType](./literals.md#triggertypetype) 
## JobWorkerExecutorConfigurationTypeDef

```python
# JobWorkerExecutorConfigurationTypeDef definition

class JobWorkerExecutorConfigurationTypeDef(TypedDict):
    pollingAccounts: NotRequired[List[str]],
    pollingServicePrincipals: NotRequired[List[str]],
```

## LambdaExecutorConfigurationTypeDef

```python
# LambdaExecutorConfigurationTypeDef definition

class LambdaExecutorConfigurationTypeDef(TypedDict):
    lambdaFunctionArn: str,
```

## FailureDetailsTypeDef

```python
# FailureDetailsTypeDef definition

class FailureDetailsTypeDef(TypedDict):
    type: FailureTypeType,  # (1)
    message: str,
    externalExecutionId: NotRequired[str],
```

1. See [:material-code-brackets: FailureTypeType](./literals.md#failuretypetype) 
## GetActionTypeInputRequestTypeDef

```python
# GetActionTypeInputRequestTypeDef definition

class GetActionTypeInputRequestTypeDef(TypedDict):
    category: ActionCategoryType,  # (1)
    owner: str,
    provider: str,
    version: str,
```

1. See [:material-code-brackets: ActionCategoryType](./literals.md#actioncategorytype) 
## GetJobDetailsInputRequestTypeDef

```python
# GetJobDetailsInputRequestTypeDef definition

class GetJobDetailsInputRequestTypeDef(TypedDict):
    jobId: str,
```

## GetPipelineExecutionInputRequestTypeDef

```python
# GetPipelineExecutionInputRequestTypeDef definition

class GetPipelineExecutionInputRequestTypeDef(TypedDict):
    pipelineName: str,
    pipelineExecutionId: str,
```

## GetPipelineInputRequestTypeDef

```python
# GetPipelineInputRequestTypeDef definition

class GetPipelineInputRequestTypeDef(TypedDict):
    name: str,
    version: NotRequired[int],
```

## PipelineMetadataTypeDef

```python
# PipelineMetadataTypeDef definition

class PipelineMetadataTypeDef(TypedDict):
    pipelineArn: NotRequired[str],
    created: NotRequired[datetime],
    updated: NotRequired[datetime],
    pollingDisabledAt: NotRequired[datetime],
```

## GetPipelineStateInputRequestTypeDef

```python
# GetPipelineStateInputRequestTypeDef definition

class GetPipelineStateInputRequestTypeDef(TypedDict):
    name: str,
```

## GetThirdPartyJobDetailsInputRequestTypeDef

```python
# GetThirdPartyJobDetailsInputRequestTypeDef definition

class GetThirdPartyJobDetailsInputRequestTypeDef(TypedDict):
    jobId: str,
    clientToken: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListActionTypesInputRequestTypeDef

```python
# ListActionTypesInputRequestTypeDef definition

class ListActionTypesInputRequestTypeDef(TypedDict):
    actionOwnerFilter: NotRequired[ActionOwnerType],  # (1)
    nextToken: NotRequired[str],
    regionFilter: NotRequired[str],
```

1. See [:material-code-brackets: ActionOwnerType](./literals.md#actionownertype) 
## ListPipelineExecutionsInputRequestTypeDef

```python
# ListPipelineExecutionsInputRequestTypeDef definition

class ListPipelineExecutionsInputRequestTypeDef(TypedDict):
    pipelineName: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListPipelinesInputRequestTypeDef

```python
# ListPipelinesInputRequestTypeDef definition

class ListPipelinesInputRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## PipelineSummaryTypeDef

```python
# PipelineSummaryTypeDef definition

class PipelineSummaryTypeDef(TypedDict):
    name: NotRequired[str],
    version: NotRequired[int],
    created: NotRequired[datetime],
    updated: NotRequired[datetime],
```

## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListWebhooksInputRequestTypeDef

```python
# ListWebhooksInputRequestTypeDef definition

class ListWebhooksInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## StageContextTypeDef

```python
# StageContextTypeDef definition

class StageContextTypeDef(TypedDict):
    name: NotRequired[str],
```

## SourceRevisionTypeDef

```python
# SourceRevisionTypeDef definition

class SourceRevisionTypeDef(TypedDict):
    actionName: str,
    revisionId: NotRequired[str],
    revisionSummary: NotRequired[str],
    revisionUrl: NotRequired[str],
```

## StopExecutionTriggerTypeDef

```python
# StopExecutionTriggerTypeDef definition

class StopExecutionTriggerTypeDef(TypedDict):
    reason: NotRequired[str],
```

## ThirdPartyJobTypeDef

```python
# ThirdPartyJobTypeDef definition

class ThirdPartyJobTypeDef(TypedDict):
    clientId: NotRequired[str],
    jobId: NotRequired[str],
```

## RegisterWebhookWithThirdPartyInputRequestTypeDef

```python
# RegisterWebhookWithThirdPartyInputRequestTypeDef definition

class RegisterWebhookWithThirdPartyInputRequestTypeDef(TypedDict):
    webhookName: NotRequired[str],
```

## RetryStageExecutionInputRequestTypeDef

```python
# RetryStageExecutionInputRequestTypeDef definition

class RetryStageExecutionInputRequestTypeDef(TypedDict):
    pipelineName: str,
    stageName: str,
    pipelineExecutionId: str,
    retryMode: StageRetryModeType,  # (1)
```

1. See [:material-code-brackets: StageRetryModeType](./literals.md#stageretrymodetype) 
## StageExecutionTypeDef

```python
# StageExecutionTypeDef definition

class StageExecutionTypeDef(TypedDict):
    pipelineExecutionId: str,
    status: StageExecutionStatusType,  # (1)
```

1. See [:material-code-brackets: StageExecutionStatusType](./literals.md#stageexecutionstatustype) 
## TransitionStateTypeDef

```python
# TransitionStateTypeDef definition

class TransitionStateTypeDef(TypedDict):
    enabled: NotRequired[bool],
    lastChangedBy: NotRequired[str],
    lastChangedAt: NotRequired[datetime],
    disabledReason: NotRequired[str],
```

## StartPipelineExecutionInputRequestTypeDef

```python
# StartPipelineExecutionInputRequestTypeDef definition

class StartPipelineExecutionInputRequestTypeDef(TypedDict):
    name: str,
    clientRequestToken: NotRequired[str],
```

## StopPipelineExecutionInputRequestTypeDef

```python
# StopPipelineExecutionInputRequestTypeDef definition

class StopPipelineExecutionInputRequestTypeDef(TypedDict):
    pipelineName: str,
    pipelineExecutionId: str,
    abandon: NotRequired[bool],
    reason: NotRequired[str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## WebhookAuthConfigurationTypeDef

```python
# WebhookAuthConfigurationTypeDef definition

class WebhookAuthConfigurationTypeDef(TypedDict):
    AllowedIPRange: NotRequired[str],
    SecretToken: NotRequired[str],
```

## WebhookFilterRuleTypeDef

```python
# WebhookFilterRuleTypeDef definition

class WebhookFilterRuleTypeDef(TypedDict):
    jsonPath: str,
    matchEquals: NotRequired[str],
```

## AcknowledgeJobOutputTypeDef

```python
# AcknowledgeJobOutputTypeDef definition

class AcknowledgeJobOutputTypeDef(TypedDict):
    status: JobStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AcknowledgeThirdPartyJobOutputTypeDef

```python
# AcknowledgeThirdPartyJobOutputTypeDef definition

class AcknowledgeThirdPartyJobOutputTypeDef(TypedDict):
    status: JobStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutActionRevisionOutputTypeDef

```python
# PutActionRevisionOutputTypeDef definition

class PutActionRevisionOutputTypeDef(TypedDict):
    newRevision: bool,
    pipelineExecutionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutApprovalResultOutputTypeDef

```python
# PutApprovalResultOutputTypeDef definition

class PutApprovalResultOutputTypeDef(TypedDict):
    approvedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RetryStageExecutionOutputTypeDef

```python
# RetryStageExecutionOutputTypeDef definition

class RetryStageExecutionOutputTypeDef(TypedDict):
    pipelineExecutionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartPipelineExecutionOutputTypeDef

```python
# StartPipelineExecutionOutputTypeDef definition

class StartPipelineExecutionOutputTypeDef(TypedDict):
    pipelineExecutionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopPipelineExecutionOutputTypeDef

```python
# StopPipelineExecutionOutputTypeDef definition

class StopPipelineExecutionOutputTypeDef(TypedDict):
    pipelineExecutionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PollForJobsInputRequestTypeDef

```python
# PollForJobsInputRequestTypeDef definition

class PollForJobsInputRequestTypeDef(TypedDict):
    actionTypeId: ActionTypeIdTypeDef,  # (1)
    maxBatchSize: NotRequired[int],
    queryParam: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ActionTypeIdTypeDef](./type_defs.md#actiontypeidtypedef) 
## PollForThirdPartyJobsInputRequestTypeDef

```python
# PollForThirdPartyJobsInputRequestTypeDef definition

class PollForThirdPartyJobsInputRequestTypeDef(TypedDict):
    actionTypeId: ActionTypeIdTypeDef,  # (1)
    maxBatchSize: NotRequired[int],
```

1. See [:material-code-braces: ActionTypeIdTypeDef](./type_defs.md#actiontypeidtypedef) 
## ActionDeclarationTypeDef

```python
# ActionDeclarationTypeDef definition

class ActionDeclarationTypeDef(TypedDict):
    name: str,
    actionTypeId: ActionTypeIdTypeDef,  # (1)
    runOrder: NotRequired[int],
    configuration: NotRequired[Mapping[str, str]],
    outputArtifacts: NotRequired[Sequence[OutputArtifactTypeDef]],  # (2)
    inputArtifacts: NotRequired[Sequence[InputArtifactTypeDef]],  # (3)
    roleArn: NotRequired[str],
    region: NotRequired[str],
    namespace: NotRequired[str],
```

1. See [:material-code-braces: ActionTypeIdTypeDef](./type_defs.md#actiontypeidtypedef) 
2. See [:material-code-braces: OutputArtifactTypeDef](./type_defs.md#outputartifacttypedef) 
3. See [:material-code-braces: InputArtifactTypeDef](./type_defs.md#inputartifacttypedef) 
## ListActionExecutionsInputRequestTypeDef

```python
# ListActionExecutionsInputRequestTypeDef definition

class ListActionExecutionsInputRequestTypeDef(TypedDict):
    pipelineName: str,
    filter: NotRequired[ActionExecutionFilterTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ActionExecutionFilterTypeDef](./type_defs.md#actionexecutionfiltertypedef) 
## ActionExecutionTypeDef

```python
# ActionExecutionTypeDef definition

class ActionExecutionTypeDef(TypedDict):
    actionExecutionId: NotRequired[str],
    status: NotRequired[ActionExecutionStatusType],  # (1)
    summary: NotRequired[str],
    lastStatusChange: NotRequired[datetime],
    token: NotRequired[str],
    lastUpdatedBy: NotRequired[str],
    externalExecutionId: NotRequired[str],
    externalExecutionUrl: NotRequired[str],
    percentComplete: NotRequired[int],
    errorDetails: NotRequired[ErrorDetailsTypeDef],  # (2)
```

1. See [:material-code-brackets: ActionExecutionStatusType](./literals.md#actionexecutionstatustype) 
2. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
## PutActionRevisionInputRequestTypeDef

```python
# PutActionRevisionInputRequestTypeDef definition

class PutActionRevisionInputRequestTypeDef(TypedDict):
    pipelineName: str,
    stageName: str,
    actionName: str,
    actionRevision: ActionRevisionTypeDef,  # (1)
```

1. See [:material-code-braces: ActionRevisionTypeDef](./type_defs.md#actionrevisiontypedef) 
## ActionTypeTypeDef

```python
# ActionTypeTypeDef definition

class ActionTypeTypeDef(TypedDict):
    id: ActionTypeIdTypeDef,  # (1)
    inputArtifactDetails: ArtifactDetailsTypeDef,  # (4)
    outputArtifactDetails: ArtifactDetailsTypeDef,  # (4)
    settings: NotRequired[ActionTypeSettingsTypeDef],  # (2)
    actionConfigurationProperties: NotRequired[List[ActionConfigurationPropertyTypeDef]],  # (3)
```

1. See [:material-code-braces: ActionTypeIdTypeDef](./type_defs.md#actiontypeidtypedef) 
2. See [:material-code-braces: ActionTypeSettingsTypeDef](./type_defs.md#actiontypesettingstypedef) 
3. See [:material-code-braces: ActionConfigurationPropertyTypeDef](./type_defs.md#actionconfigurationpropertytypedef) 
4. See [:material-code-braces: ArtifactDetailsTypeDef](./type_defs.md#artifactdetailstypedef) 
5. See [:material-code-braces: ArtifactDetailsTypeDef](./type_defs.md#artifactdetailstypedef) 
## PutApprovalResultInputRequestTypeDef

```python
# PutApprovalResultInputRequestTypeDef definition

class PutApprovalResultInputRequestTypeDef(TypedDict):
    pipelineName: str,
    stageName: str,
    actionName: str,
    result: ApprovalResultTypeDef,  # (1)
    token: str,
```

1. See [:material-code-braces: ApprovalResultTypeDef](./type_defs.md#approvalresulttypedef) 
## ArtifactDetailTypeDef

```python
# ArtifactDetailTypeDef definition

class ArtifactDetailTypeDef(TypedDict):
    name: NotRequired[str],
    s3location: NotRequired[S3LocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## ArtifactLocationTypeDef

```python
# ArtifactLocationTypeDef definition

class ArtifactLocationTypeDef(TypedDict):
    type: NotRequired[ArtifactLocationTypeType],  # (1)
    s3Location: NotRequired[S3ArtifactLocationTypeDef],  # (2)
```

1. See [:material-code-brackets: ArtifactLocationTypeType](./literals.md#artifactlocationtypetype) 
2. See [:material-code-braces: S3ArtifactLocationTypeDef](./type_defs.md#s3artifactlocationtypedef) 
## PipelineExecutionTypeDef

```python
# PipelineExecutionTypeDef definition

class PipelineExecutionTypeDef(TypedDict):
    pipelineName: NotRequired[str],
    pipelineVersion: NotRequired[int],
    pipelineExecutionId: NotRequired[str],
    status: NotRequired[PipelineExecutionStatusType],  # (1)
    statusSummary: NotRequired[str],
    artifactRevisions: NotRequired[List[ArtifactRevisionTypeDef]],  # (2)
```

1. See [:material-code-brackets: PipelineExecutionStatusType](./literals.md#pipelineexecutionstatustype) 
2. See [:material-code-braces: ArtifactRevisionTypeDef](./type_defs.md#artifactrevisiontypedef) 
## ArtifactStoreTypeDef

```python
# ArtifactStoreTypeDef definition

class ArtifactStoreTypeDef(TypedDict):
    type: ArtifactStoreTypeType,  # (1)
    location: str,
    encryptionKey: NotRequired[EncryptionKeyTypeDef],  # (2)
```

1. See [:material-code-brackets: ArtifactStoreTypeType](./literals.md#artifactstoretypetype) 
2. See [:material-code-braces: EncryptionKeyTypeDef](./type_defs.md#encryptionkeytypedef) 
## CreateCustomActionTypeInputRequestTypeDef

```python
# CreateCustomActionTypeInputRequestTypeDef definition

class CreateCustomActionTypeInputRequestTypeDef(TypedDict):
    category: ActionCategoryType,  # (1)
    provider: str,
    version: str,
    inputArtifactDetails: ArtifactDetailsTypeDef,  # (2)
    outputArtifactDetails: ArtifactDetailsTypeDef,  # (2)
    settings: NotRequired[ActionTypeSettingsTypeDef],  # (4)
    configurationProperties: NotRequired[Sequence[ActionConfigurationPropertyTypeDef]],  # (5)
    tags: NotRequired[Sequence[TagTypeDef]],  # (6)
```

1. See [:material-code-brackets: ActionCategoryType](./literals.md#actioncategorytype) 
2. See [:material-code-braces: ArtifactDetailsTypeDef](./type_defs.md#artifactdetailstypedef) 
3. See [:material-code-braces: ArtifactDetailsTypeDef](./type_defs.md#artifactdetailstypedef) 
4. See [:material-code-braces: ActionTypeSettingsTypeDef](./type_defs.md#actiontypesettingstypedef) 
5. See [:material-code-braces: ActionConfigurationPropertyTypeDef](./type_defs.md#actionconfigurationpropertytypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CurrentRevisionTypeDef

```python
# CurrentRevisionTypeDef definition

class CurrentRevisionTypeDef(TypedDict):
    revision: str,
    changeIdentifier: str,
    created: NotRequired[Union[datetime, str]],
    revisionSummary: NotRequired[str],
```

## ExecutorConfigurationTypeDef

```python
# ExecutorConfigurationTypeDef definition

class ExecutorConfigurationTypeDef(TypedDict):
    lambdaExecutorConfiguration: NotRequired[LambdaExecutorConfigurationTypeDef],  # (1)
    jobWorkerExecutorConfiguration: NotRequired[JobWorkerExecutorConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: LambdaExecutorConfigurationTypeDef](./type_defs.md#lambdaexecutorconfigurationtypedef) 
2. See [:material-code-braces: JobWorkerExecutorConfigurationTypeDef](./type_defs.md#jobworkerexecutorconfigurationtypedef) 
## PutJobFailureResultInputRequestTypeDef

```python
# PutJobFailureResultInputRequestTypeDef definition

class PutJobFailureResultInputRequestTypeDef(TypedDict):
    jobId: str,
    failureDetails: FailureDetailsTypeDef,  # (1)
```

1. See [:material-code-braces: FailureDetailsTypeDef](./type_defs.md#failuredetailstypedef) 
## PutThirdPartyJobFailureResultInputRequestTypeDef

```python
# PutThirdPartyJobFailureResultInputRequestTypeDef definition

class PutThirdPartyJobFailureResultInputRequestTypeDef(TypedDict):
    jobId: str,
    clientToken: str,
    failureDetails: FailureDetailsTypeDef,  # (1)
```

1. See [:material-code-braces: FailureDetailsTypeDef](./type_defs.md#failuredetailstypedef) 
## ListActionExecutionsInputListActionExecutionsPaginateTypeDef

```python
# ListActionExecutionsInputListActionExecutionsPaginateTypeDef definition

class ListActionExecutionsInputListActionExecutionsPaginateTypeDef(TypedDict):
    pipelineName: str,
    filter: NotRequired[ActionExecutionFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ActionExecutionFilterTypeDef](./type_defs.md#actionexecutionfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListActionTypesInputListActionTypesPaginateTypeDef

```python
# ListActionTypesInputListActionTypesPaginateTypeDef definition

class ListActionTypesInputListActionTypesPaginateTypeDef(TypedDict):
    actionOwnerFilter: NotRequired[ActionOwnerType],  # (1)
    regionFilter: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ActionOwnerType](./literals.md#actionownertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef

```python
# ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef definition

class ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef(TypedDict):
    pipelineName: str,
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
## ListTagsForResourceInputListTagsForResourcePaginateTypeDef

```python
# ListTagsForResourceInputListTagsForResourcePaginateTypeDef definition

class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(TypedDict):
    resourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWebhooksInputListWebhooksPaginateTypeDef

```python
# ListWebhooksInputListWebhooksPaginateTypeDef definition

class ListWebhooksInputListWebhooksPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPipelinesOutputTypeDef

```python
# ListPipelinesOutputTypeDef definition

class ListPipelinesOutputTypeDef(TypedDict):
    pipelines: List[PipelineSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineSummaryTypeDef](./type_defs.md#pipelinesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PipelineContextTypeDef

```python
# PipelineContextTypeDef definition

class PipelineContextTypeDef(TypedDict):
    pipelineName: NotRequired[str],
    stage: NotRequired[StageContextTypeDef],  # (1)
    action: NotRequired[ActionContextTypeDef],  # (2)
    pipelineArn: NotRequired[str],
    pipelineExecutionId: NotRequired[str],
```

1. See [:material-code-braces: StageContextTypeDef](./type_defs.md#stagecontexttypedef) 
2. See [:material-code-braces: ActionContextTypeDef](./type_defs.md#actioncontexttypedef) 
## PipelineExecutionSummaryTypeDef

```python
# PipelineExecutionSummaryTypeDef definition

class PipelineExecutionSummaryTypeDef(TypedDict):
    pipelineExecutionId: NotRequired[str],
    status: NotRequired[PipelineExecutionStatusType],  # (1)
    startTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
    sourceRevisions: NotRequired[List[SourceRevisionTypeDef]],  # (2)
    trigger: NotRequired[ExecutionTriggerTypeDef],  # (3)
    stopTrigger: NotRequired[StopExecutionTriggerTypeDef],  # (4)
```

1. See [:material-code-brackets: PipelineExecutionStatusType](./literals.md#pipelineexecutionstatustype) 
2. See [:material-code-braces: SourceRevisionTypeDef](./type_defs.md#sourcerevisiontypedef) 
3. See [:material-code-braces: ExecutionTriggerTypeDef](./type_defs.md#executiontriggertypedef) 
4. See [:material-code-braces: StopExecutionTriggerTypeDef](./type_defs.md#stopexecutiontriggertypedef) 
## PollForThirdPartyJobsOutputTypeDef

```python
# PollForThirdPartyJobsOutputTypeDef definition

class PollForThirdPartyJobsOutputTypeDef(TypedDict):
    jobs: List[ThirdPartyJobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThirdPartyJobTypeDef](./type_defs.md#thirdpartyjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WebhookDefinitionTypeDef

```python
# WebhookDefinitionTypeDef definition

class WebhookDefinitionTypeDef(TypedDict):
    name: str,
    targetPipeline: str,
    targetAction: str,
    filters: List[WebhookFilterRuleTypeDef],  # (1)
    authentication: WebhookAuthenticationTypeType,  # (2)
    authenticationConfiguration: WebhookAuthConfigurationTypeDef,  # (3)
```

1. See [:material-code-braces: WebhookFilterRuleTypeDef](./type_defs.md#webhookfilterruletypedef) 
2. See [:material-code-brackets: WebhookAuthenticationTypeType](./literals.md#webhookauthenticationtypetype) 
3. See [:material-code-braces: WebhookAuthConfigurationTypeDef](./type_defs.md#webhookauthconfigurationtypedef) 
## StageDeclarationTypeDef

```python
# StageDeclarationTypeDef definition

class StageDeclarationTypeDef(TypedDict):
    name: str,
    actions: Sequence[ActionDeclarationTypeDef],  # (2)
    blockers: NotRequired[Sequence[BlockerDeclarationTypeDef]],  # (1)
```

1. See [:material-code-braces: BlockerDeclarationTypeDef](./type_defs.md#blockerdeclarationtypedef) 
2. See [:material-code-braces: ActionDeclarationTypeDef](./type_defs.md#actiondeclarationtypedef) 
## ActionStateTypeDef

```python
# ActionStateTypeDef definition

class ActionStateTypeDef(TypedDict):
    actionName: NotRequired[str],
    currentRevision: NotRequired[ActionRevisionTypeDef],  # (1)
    latestExecution: NotRequired[ActionExecutionTypeDef],  # (2)
    entityUrl: NotRequired[str],
    revisionUrl: NotRequired[str],
```

1. See [:material-code-braces: ActionRevisionTypeDef](./type_defs.md#actionrevisiontypedef) 
2. See [:material-code-braces: ActionExecutionTypeDef](./type_defs.md#actionexecutiontypedef) 
## CreateCustomActionTypeOutputTypeDef

```python
# CreateCustomActionTypeOutputTypeDef definition

class CreateCustomActionTypeOutputTypeDef(TypedDict):
    actionType: ActionTypeTypeDef,  # (1)
    tags: List[TagTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ActionTypeTypeDef](./type_defs.md#actiontypetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListActionTypesOutputTypeDef

```python
# ListActionTypesOutputTypeDef definition

class ListActionTypesOutputTypeDef(TypedDict):
    actionTypes: List[ActionTypeTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActionTypeTypeDef](./type_defs.md#actiontypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ActionExecutionInputTypeDef

```python
# ActionExecutionInputTypeDef definition

class ActionExecutionInputTypeDef(TypedDict):
    actionTypeId: NotRequired[ActionTypeIdTypeDef],  # (1)
    configuration: NotRequired[Dict[str, str]],
    resolvedConfiguration: NotRequired[Dict[str, str]],
    roleArn: NotRequired[str],
    region: NotRequired[str],
    inputArtifacts: NotRequired[List[ArtifactDetailTypeDef]],  # (2)
    namespace: NotRequired[str],
```

1. See [:material-code-braces: ActionTypeIdTypeDef](./type_defs.md#actiontypeidtypedef) 
2. See [:material-code-braces: ArtifactDetailTypeDef](./type_defs.md#artifactdetailtypedef) 
## ActionExecutionOutputTypeDef

```python
# ActionExecutionOutputTypeDef definition

class ActionExecutionOutputTypeDef(TypedDict):
    outputArtifacts: NotRequired[List[ArtifactDetailTypeDef]],  # (1)
    executionResult: NotRequired[ActionExecutionResultTypeDef],  # (2)
    outputVariables: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ArtifactDetailTypeDef](./type_defs.md#artifactdetailtypedef) 
2. See [:material-code-braces: ActionExecutionResultTypeDef](./type_defs.md#actionexecutionresulttypedef) 
## ArtifactTypeDef

```python
# ArtifactTypeDef definition

class ArtifactTypeDef(TypedDict):
    name: NotRequired[str],
    revision: NotRequired[str],
    location: NotRequired[ArtifactLocationTypeDef],  # (1)
```

1. See [:material-code-braces: ArtifactLocationTypeDef](./type_defs.md#artifactlocationtypedef) 
## GetPipelineExecutionOutputTypeDef

```python
# GetPipelineExecutionOutputTypeDef definition

class GetPipelineExecutionOutputTypeDef(TypedDict):
    pipelineExecution: PipelineExecutionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineExecutionTypeDef](./type_defs.md#pipelineexecutiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutJobSuccessResultInputRequestTypeDef

```python
# PutJobSuccessResultInputRequestTypeDef definition

class PutJobSuccessResultInputRequestTypeDef(TypedDict):
    jobId: str,
    currentRevision: NotRequired[CurrentRevisionTypeDef],  # (1)
    continuationToken: NotRequired[str],
    executionDetails: NotRequired[ExecutionDetailsTypeDef],  # (2)
    outputVariables: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: CurrentRevisionTypeDef](./type_defs.md#currentrevisiontypedef) 
2. See [:material-code-braces: ExecutionDetailsTypeDef](./type_defs.md#executiondetailstypedef) 
## PutThirdPartyJobSuccessResultInputRequestTypeDef

```python
# PutThirdPartyJobSuccessResultInputRequestTypeDef definition

class PutThirdPartyJobSuccessResultInputRequestTypeDef(TypedDict):
    jobId: str,
    clientToken: str,
    currentRevision: NotRequired[CurrentRevisionTypeDef],  # (1)
    continuationToken: NotRequired[str],
    executionDetails: NotRequired[ExecutionDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: CurrentRevisionTypeDef](./type_defs.md#currentrevisiontypedef) 
2. See [:material-code-braces: ExecutionDetailsTypeDef](./type_defs.md#executiondetailstypedef) 
## ActionTypeExecutorTypeDef

```python
# ActionTypeExecutorTypeDef definition

class ActionTypeExecutorTypeDef(TypedDict):
    configuration: ExecutorConfigurationTypeDef,  # (1)
    type: ExecutorTypeType,  # (2)
    policyStatementsTemplate: NotRequired[str],
    jobTimeout: NotRequired[int],
```

1. See [:material-code-braces: ExecutorConfigurationTypeDef](./type_defs.md#executorconfigurationtypedef) 
2. See [:material-code-brackets: ExecutorTypeType](./literals.md#executortypetype) 
## ListPipelineExecutionsOutputTypeDef

```python
# ListPipelineExecutionsOutputTypeDef definition

class ListPipelineExecutionsOutputTypeDef(TypedDict):
    pipelineExecutionSummaries: List[PipelineExecutionSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineExecutionSummaryTypeDef](./type_defs.md#pipelineexecutionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWebhookItemTypeDef

```python
# ListWebhookItemTypeDef definition

class ListWebhookItemTypeDef(TypedDict):
    definition: WebhookDefinitionTypeDef,  # (1)
    url: str,
    errorMessage: NotRequired[str],
    errorCode: NotRequired[str],
    lastTriggered: NotRequired[datetime],
    arn: NotRequired[str],
    tags: NotRequired[List[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: WebhookDefinitionTypeDef](./type_defs.md#webhookdefinitiontypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PutWebhookInputRequestTypeDef

```python
# PutWebhookInputRequestTypeDef definition

class PutWebhookInputRequestTypeDef(TypedDict):
    webhook: WebhookDefinitionTypeDef,  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: WebhookDefinitionTypeDef](./type_defs.md#webhookdefinitiontypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PipelineDeclarationTypeDef

```python
# PipelineDeclarationTypeDef definition

class PipelineDeclarationTypeDef(TypedDict):
    name: str,
    roleArn: str,
    stages: Sequence[StageDeclarationTypeDef],  # (3)
    artifactStore: NotRequired[ArtifactStoreTypeDef],  # (1)
    artifactStores: NotRequired[Mapping[str, ArtifactStoreTypeDef]],  # (2)
    version: NotRequired[int],
```

1. See [:material-code-braces: ArtifactStoreTypeDef](./type_defs.md#artifactstoretypedef) 
2. See [:material-code-braces: ArtifactStoreTypeDef](./type_defs.md#artifactstoretypedef) 
3. See [:material-code-braces: StageDeclarationTypeDef](./type_defs.md#stagedeclarationtypedef) 
## StageStateTypeDef

```python
# StageStateTypeDef definition

class StageStateTypeDef(TypedDict):
    stageName: NotRequired[str],
    inboundExecution: NotRequired[StageExecutionTypeDef],  # (1)
    inboundTransitionState: NotRequired[TransitionStateTypeDef],  # (2)
    actionStates: NotRequired[List[ActionStateTypeDef]],  # (3)
    latestExecution: NotRequired[StageExecutionTypeDef],  # (1)
```

1. See [:material-code-braces: StageExecutionTypeDef](./type_defs.md#stageexecutiontypedef) 
2. See [:material-code-braces: TransitionStateTypeDef](./type_defs.md#transitionstatetypedef) 
3. See [:material-code-braces: ActionStateTypeDef](./type_defs.md#actionstatetypedef) 
4. See [:material-code-braces: StageExecutionTypeDef](./type_defs.md#stageexecutiontypedef) 
## ActionExecutionDetailTypeDef

```python
# ActionExecutionDetailTypeDef definition

class ActionExecutionDetailTypeDef(TypedDict):
    pipelineExecutionId: NotRequired[str],
    actionExecutionId: NotRequired[str],
    pipelineVersion: NotRequired[int],
    stageName: NotRequired[str],
    actionName: NotRequired[str],
    startTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
    status: NotRequired[ActionExecutionStatusType],  # (1)
    input: NotRequired[ActionExecutionInputTypeDef],  # (2)
    output: NotRequired[ActionExecutionOutputTypeDef],  # (3)
```

1. See [:material-code-brackets: ActionExecutionStatusType](./literals.md#actionexecutionstatustype) 
2. See [:material-code-braces: ActionExecutionInputTypeDef](./type_defs.md#actionexecutioninputtypedef) 
3. See [:material-code-braces: ActionExecutionOutputTypeDef](./type_defs.md#actionexecutionoutputtypedef) 
## JobDataTypeDef

```python
# JobDataTypeDef definition

class JobDataTypeDef(TypedDict):
    actionTypeId: NotRequired[ActionTypeIdTypeDef],  # (1)
    actionConfiguration: NotRequired[ActionConfigurationTypeDef],  # (2)
    pipelineContext: NotRequired[PipelineContextTypeDef],  # (3)
    inputArtifacts: NotRequired[List[ArtifactTypeDef]],  # (4)
    outputArtifacts: NotRequired[List[ArtifactTypeDef]],  # (4)
    artifactCredentials: NotRequired[AWSSessionCredentialsTypeDef],  # (6)
    continuationToken: NotRequired[str],
    encryptionKey: NotRequired[EncryptionKeyTypeDef],  # (7)
```

1. See [:material-code-braces: ActionTypeIdTypeDef](./type_defs.md#actiontypeidtypedef) 
2. See [:material-code-braces: ActionConfigurationTypeDef](./type_defs.md#actionconfigurationtypedef) 
3. See [:material-code-braces: PipelineContextTypeDef](./type_defs.md#pipelinecontexttypedef) 
4. See [:material-code-braces: ArtifactTypeDef](./type_defs.md#artifacttypedef) 
5. See [:material-code-braces: ArtifactTypeDef](./type_defs.md#artifacttypedef) 
6. See [:material-code-braces: AWSSessionCredentialsTypeDef](./type_defs.md#awssessioncredentialstypedef) 
7. See [:material-code-braces: EncryptionKeyTypeDef](./type_defs.md#encryptionkeytypedef) 
## ThirdPartyJobDataTypeDef

```python
# ThirdPartyJobDataTypeDef definition

class ThirdPartyJobDataTypeDef(TypedDict):
    actionTypeId: NotRequired[ActionTypeIdTypeDef],  # (1)
    actionConfiguration: NotRequired[ActionConfigurationTypeDef],  # (2)
    pipelineContext: NotRequired[PipelineContextTypeDef],  # (3)
    inputArtifacts: NotRequired[List[ArtifactTypeDef]],  # (4)
    outputArtifacts: NotRequired[List[ArtifactTypeDef]],  # (4)
    artifactCredentials: NotRequired[AWSSessionCredentialsTypeDef],  # (6)
    continuationToken: NotRequired[str],
    encryptionKey: NotRequired[EncryptionKeyTypeDef],  # (7)
```

1. See [:material-code-braces: ActionTypeIdTypeDef](./type_defs.md#actiontypeidtypedef) 
2. See [:material-code-braces: ActionConfigurationTypeDef](./type_defs.md#actionconfigurationtypedef) 
3. See [:material-code-braces: PipelineContextTypeDef](./type_defs.md#pipelinecontexttypedef) 
4. See [:material-code-braces: ArtifactTypeDef](./type_defs.md#artifacttypedef) 
5. See [:material-code-braces: ArtifactTypeDef](./type_defs.md#artifacttypedef) 
6. See [:material-code-braces: AWSSessionCredentialsTypeDef](./type_defs.md#awssessioncredentialstypedef) 
7. See [:material-code-braces: EncryptionKeyTypeDef](./type_defs.md#encryptionkeytypedef) 
## ActionTypeDeclarationTypeDef

```python
# ActionTypeDeclarationTypeDef definition

class ActionTypeDeclarationTypeDef(TypedDict):
    executor: ActionTypeExecutorTypeDef,  # (1)
    id: ActionTypeIdentifierTypeDef,  # (2)
    inputArtifactDetails: ActionTypeArtifactDetailsTypeDef,  # (3)
    outputArtifactDetails: ActionTypeArtifactDetailsTypeDef,  # (3)
    description: NotRequired[str],
    permissions: NotRequired[ActionTypePermissionsTypeDef],  # (5)
    properties: NotRequired[List[ActionTypePropertyTypeDef]],  # (6)
    urls: NotRequired[ActionTypeUrlsTypeDef],  # (7)
```

1. See [:material-code-braces: ActionTypeExecutorTypeDef](./type_defs.md#actiontypeexecutortypedef) 
2. See [:material-code-braces: ActionTypeIdentifierTypeDef](./type_defs.md#actiontypeidentifiertypedef) 
3. See [:material-code-braces: ActionTypeArtifactDetailsTypeDef](./type_defs.md#actiontypeartifactdetailstypedef) 
4. See [:material-code-braces: ActionTypeArtifactDetailsTypeDef](./type_defs.md#actiontypeartifactdetailstypedef) 
5. See [:material-code-braces: ActionTypePermissionsTypeDef](./type_defs.md#actiontypepermissionstypedef) 
6. See [:material-code-braces: ActionTypePropertyTypeDef](./type_defs.md#actiontypepropertytypedef) 
7. See [:material-code-braces: ActionTypeUrlsTypeDef](./type_defs.md#actiontypeurlstypedef) 
## ListWebhooksOutputTypeDef

```python
# ListWebhooksOutputTypeDef definition

class ListWebhooksOutputTypeDef(TypedDict):
    webhooks: List[ListWebhookItemTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListWebhookItemTypeDef](./type_defs.md#listwebhookitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutWebhookOutputTypeDef

```python
# PutWebhookOutputTypeDef definition

class PutWebhookOutputTypeDef(TypedDict):
    webhook: ListWebhookItemTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListWebhookItemTypeDef](./type_defs.md#listwebhookitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePipelineInputRequestTypeDef

```python
# CreatePipelineInputRequestTypeDef definition

class CreatePipelineInputRequestTypeDef(TypedDict):
    pipeline: PipelineDeclarationTypeDef,  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: PipelineDeclarationTypeDef](./type_defs.md#pipelinedeclarationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePipelineOutputTypeDef

```python
# CreatePipelineOutputTypeDef definition

class CreatePipelineOutputTypeDef(TypedDict):
    pipeline: PipelineDeclarationTypeDef,  # (1)
    tags: List[TagTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PipelineDeclarationTypeDef](./type_defs.md#pipelinedeclarationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPipelineOutputTypeDef

```python
# GetPipelineOutputTypeDef definition

class GetPipelineOutputTypeDef(TypedDict):
    pipeline: PipelineDeclarationTypeDef,  # (1)
    metadata: PipelineMetadataTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PipelineDeclarationTypeDef](./type_defs.md#pipelinedeclarationtypedef) 
2. See [:material-code-braces: PipelineMetadataTypeDef](./type_defs.md#pipelinemetadatatypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePipelineInputRequestTypeDef

```python
# UpdatePipelineInputRequestTypeDef definition

class UpdatePipelineInputRequestTypeDef(TypedDict):
    pipeline: PipelineDeclarationTypeDef,  # (1)
```

1. See [:material-code-braces: PipelineDeclarationTypeDef](./type_defs.md#pipelinedeclarationtypedef) 
## UpdatePipelineOutputTypeDef

```python
# UpdatePipelineOutputTypeDef definition

class UpdatePipelineOutputTypeDef(TypedDict):
    pipeline: PipelineDeclarationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineDeclarationTypeDef](./type_defs.md#pipelinedeclarationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPipelineStateOutputTypeDef

```python
# GetPipelineStateOutputTypeDef definition

class GetPipelineStateOutputTypeDef(TypedDict):
    pipelineName: str,
    pipelineVersion: int,
    stageStates: List[StageStateTypeDef],  # (1)
    created: datetime,
    updated: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StageStateTypeDef](./type_defs.md#stagestatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListActionExecutionsOutputTypeDef

```python
# ListActionExecutionsOutputTypeDef definition

class ListActionExecutionsOutputTypeDef(TypedDict):
    actionExecutionDetails: List[ActionExecutionDetailTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActionExecutionDetailTypeDef](./type_defs.md#actionexecutiondetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JobDetailsTypeDef

```python
# JobDetailsTypeDef definition

class JobDetailsTypeDef(TypedDict):
    id: NotRequired[str],
    data: NotRequired[JobDataTypeDef],  # (1)
    accountId: NotRequired[str],
```

1. See [:material-code-braces: JobDataTypeDef](./type_defs.md#jobdatatypedef) 
## JobTypeDef

```python
# JobTypeDef definition

class JobTypeDef(TypedDict):
    id: NotRequired[str],
    data: NotRequired[JobDataTypeDef],  # (1)
    nonce: NotRequired[str],
    accountId: NotRequired[str],
```

1. See [:material-code-braces: JobDataTypeDef](./type_defs.md#jobdatatypedef) 
## ThirdPartyJobDetailsTypeDef

```python
# ThirdPartyJobDetailsTypeDef definition

class ThirdPartyJobDetailsTypeDef(TypedDict):
    id: NotRequired[str],
    data: NotRequired[ThirdPartyJobDataTypeDef],  # (1)
    nonce: NotRequired[str],
```

1. See [:material-code-braces: ThirdPartyJobDataTypeDef](./type_defs.md#thirdpartyjobdatatypedef) 
## GetActionTypeOutputTypeDef

```python
# GetActionTypeOutputTypeDef definition

class GetActionTypeOutputTypeDef(TypedDict):
    actionType: ActionTypeDeclarationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActionTypeDeclarationTypeDef](./type_defs.md#actiontypedeclarationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateActionTypeInputRequestTypeDef

```python
# UpdateActionTypeInputRequestTypeDef definition

class UpdateActionTypeInputRequestTypeDef(TypedDict):
    actionType: ActionTypeDeclarationTypeDef,  # (1)
```

1. See [:material-code-braces: ActionTypeDeclarationTypeDef](./type_defs.md#actiontypedeclarationtypedef) 
## GetJobDetailsOutputTypeDef

```python
# GetJobDetailsOutputTypeDef definition

class GetJobDetailsOutputTypeDef(TypedDict):
    jobDetails: JobDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobDetailsTypeDef](./type_defs.md#jobdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PollForJobsOutputTypeDef

```python
# PollForJobsOutputTypeDef definition

class PollForJobsOutputTypeDef(TypedDict):
    jobs: List[JobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetThirdPartyJobDetailsOutputTypeDef

```python
# GetThirdPartyJobDetailsOutputTypeDef definition

class GetThirdPartyJobDetailsOutputTypeDef(TypedDict):
    jobDetails: ThirdPartyJobDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThirdPartyJobDetailsTypeDef](./type_defs.md#thirdpartyjobdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
