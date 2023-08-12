# Type definitions

> [Index](../README.md) > [OpenSearchIngestion](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [OpenSearchIngestion](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
    type annotations stubs module [types-aiobotocore-osis](https://pypi.org/project/types-aiobotocore-osis/).



## ChangeProgressStageTypeDef

```python
# ChangeProgressStageTypeDef definition

class ChangeProgressStageTypeDef(TypedDict):
    Name: NotRequired[str],
    Status: NotRequired[ChangeProgressStageStatusesType],  # (1)
    Description: NotRequired[str],
    LastUpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: ChangeProgressStageStatusesType](./literals.md#changeprogressstagestatusestype) 
## CloudWatchLogDestinationTypeDef

```python
# CloudWatchLogDestinationTypeDef definition

class CloudWatchLogDestinationTypeDef(TypedDict):
    LogGroup: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## VpcOptionsTypeDef

```python
# VpcOptionsTypeDef definition

class VpcOptionsTypeDef(TypedDict):
    SubnetIds: Sequence[str],
    SecurityGroupIds: NotRequired[Sequence[str]],
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

## DeletePipelineRequestRequestTypeDef

```python
# DeletePipelineRequestRequestTypeDef definition

class DeletePipelineRequestRequestTypeDef(TypedDict):
    PipelineName: str,
```

## GetPipelineBlueprintRequestRequestTypeDef

```python
# GetPipelineBlueprintRequestRequestTypeDef definition

class GetPipelineBlueprintRequestRequestTypeDef(TypedDict):
    BlueprintName: str,
```

## PipelineBlueprintTypeDef

```python
# PipelineBlueprintTypeDef definition

class PipelineBlueprintTypeDef(TypedDict):
    BlueprintName: NotRequired[str],
    PipelineConfigurationBody: NotRequired[str],
```

## GetPipelineChangeProgressRequestRequestTypeDef

```python
# GetPipelineChangeProgressRequestRequestTypeDef definition

class GetPipelineChangeProgressRequestRequestTypeDef(TypedDict):
    PipelineName: str,
```

## GetPipelineRequestRequestTypeDef

```python
# GetPipelineRequestRequestTypeDef definition

class GetPipelineRequestRequestTypeDef(TypedDict):
    PipelineName: str,
```

## PipelineBlueprintSummaryTypeDef

```python
# PipelineBlueprintSummaryTypeDef definition

class PipelineBlueprintSummaryTypeDef(TypedDict):
    BlueprintName: NotRequired[str],
```

## ListPipelinesRequestRequestTypeDef

```python
# ListPipelinesRequestRequestTypeDef definition

class ListPipelinesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    Arn: str,
```

## PipelineStatusReasonTypeDef

```python
# PipelineStatusReasonTypeDef definition

class PipelineStatusReasonTypeDef(TypedDict):
    Description: NotRequired[str],
```

## StartPipelineRequestRequestTypeDef

```python
# StartPipelineRequestRequestTypeDef definition

class StartPipelineRequestRequestTypeDef(TypedDict):
    PipelineName: str,
```

## StopPipelineRequestRequestTypeDef

```python
# StopPipelineRequestRequestTypeDef definition

class StopPipelineRequestRequestTypeDef(TypedDict):
    PipelineName: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    Arn: str,
    TagKeys: Sequence[str],
```

## ValidatePipelineRequestRequestTypeDef

```python
# ValidatePipelineRequestRequestTypeDef definition

class ValidatePipelineRequestRequestTypeDef(TypedDict):
    PipelineConfigurationBody: str,
```

## ValidationMessageTypeDef

```python
# ValidationMessageTypeDef definition

class ValidationMessageTypeDef(TypedDict):
    Message: NotRequired[str],
```

## ChangeProgressStatusTypeDef

```python
# ChangeProgressStatusTypeDef definition

class ChangeProgressStatusTypeDef(TypedDict):
    StartTime: NotRequired[datetime],
    Status: NotRequired[ChangeProgressStatusesType],  # (1)
    TotalNumberOfStages: NotRequired[int],
    ChangeProgressStages: NotRequired[List[ChangeProgressStageTypeDef]],  # (2)
```

1. See [:material-code-brackets: ChangeProgressStatusesType](./literals.md#changeprogressstatusestype) 
2. See [:material-code-braces: ChangeProgressStageTypeDef](./type_defs.md#changeprogressstagetypedef) 
## LogPublishingOptionsTypeDef

```python
# LogPublishingOptionsTypeDef definition

class LogPublishingOptionsTypeDef(TypedDict):
    IsLoggingEnabled: NotRequired[bool],
    CloudWatchLogDestination: NotRequired[CloudWatchLogDestinationTypeDef],  # (1)
```

1. See [:material-code-braces: CloudWatchLogDestinationTypeDef](./type_defs.md#cloudwatchlogdestinationtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    Arn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## VpcEndpointTypeDef

```python
# VpcEndpointTypeDef definition

class VpcEndpointTypeDef(TypedDict):
    VpcEndpointId: NotRequired[str],
    VpcId: NotRequired[str],
    VpcOptions: NotRequired[VpcOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: VpcOptionsTypeDef](./type_defs.md#vpcoptionstypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPipelineBlueprintResponseTypeDef

```python
# GetPipelineBlueprintResponseTypeDef definition

class GetPipelineBlueprintResponseTypeDef(TypedDict):
    Blueprint: PipelineBlueprintTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineBlueprintTypeDef](./type_defs.md#pipelineblueprinttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPipelineBlueprintsResponseTypeDef

```python
# ListPipelineBlueprintsResponseTypeDef definition

class ListPipelineBlueprintsResponseTypeDef(TypedDict):
    Blueprints: List[PipelineBlueprintSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineBlueprintSummaryTypeDef](./type_defs.md#pipelineblueprintsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PipelineSummaryTypeDef

```python
# PipelineSummaryTypeDef definition

class PipelineSummaryTypeDef(TypedDict):
    Status: NotRequired[PipelineStatusType],  # (1)
    StatusReason: NotRequired[PipelineStatusReasonTypeDef],  # (2)
    PipelineName: NotRequired[str],
    PipelineArn: NotRequired[str],
    MinUnits: NotRequired[int],
    MaxUnits: NotRequired[int],
    CreatedAt: NotRequired[datetime],
    LastUpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: PipelineStatusType](./literals.md#pipelinestatustype) 
2. See [:material-code-braces: PipelineStatusReasonTypeDef](./type_defs.md#pipelinestatusreasontypedef) 
## ValidatePipelineResponseTypeDef

```python
# ValidatePipelineResponseTypeDef definition

class ValidatePipelineResponseTypeDef(TypedDict):
    isValid: bool,
    Errors: List[ValidationMessageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ValidationMessageTypeDef](./type_defs.md#validationmessagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPipelineChangeProgressResponseTypeDef

```python
# GetPipelineChangeProgressResponseTypeDef definition

class GetPipelineChangeProgressResponseTypeDef(TypedDict):
    ChangeProgressStatuses: List[ChangeProgressStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChangeProgressStatusTypeDef](./type_defs.md#changeprogressstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePipelineRequestRequestTypeDef

```python
# CreatePipelineRequestRequestTypeDef definition

class CreatePipelineRequestRequestTypeDef(TypedDict):
    PipelineName: str,
    MinUnits: int,
    MaxUnits: int,
    PipelineConfigurationBody: str,
    LogPublishingOptions: NotRequired[LogPublishingOptionsTypeDef],  # (1)
    VpcOptions: NotRequired[VpcOptionsTypeDef],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: LogPublishingOptionsTypeDef](./type_defs.md#logpublishingoptionstypedef) 
2. See [:material-code-braces: VpcOptionsTypeDef](./type_defs.md#vpcoptionstypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdatePipelineRequestRequestTypeDef

```python
# UpdatePipelineRequestRequestTypeDef definition

class UpdatePipelineRequestRequestTypeDef(TypedDict):
    PipelineName: str,
    MinUnits: NotRequired[int],
    MaxUnits: NotRequired[int],
    PipelineConfigurationBody: NotRequired[str],
    LogPublishingOptions: NotRequired[LogPublishingOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: LogPublishingOptionsTypeDef](./type_defs.md#logpublishingoptionstypedef) 
## PipelineTypeDef

```python
# PipelineTypeDef definition

class PipelineTypeDef(TypedDict):
    PipelineName: NotRequired[str],
    PipelineArn: NotRequired[str],
    MinUnits: NotRequired[int],
    MaxUnits: NotRequired[int],
    Status: NotRequired[PipelineStatusType],  # (1)
    StatusReason: NotRequired[PipelineStatusReasonTypeDef],  # (2)
    PipelineConfigurationBody: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    LastUpdatedAt: NotRequired[datetime],
    IngestEndpointUrls: NotRequired[List[str]],
    LogPublishingOptions: NotRequired[LogPublishingOptionsTypeDef],  # (3)
    VpcEndpoints: NotRequired[List[VpcEndpointTypeDef]],  # (4)
```

1. See [:material-code-brackets: PipelineStatusType](./literals.md#pipelinestatustype) 
2. See [:material-code-braces: PipelineStatusReasonTypeDef](./type_defs.md#pipelinestatusreasontypedef) 
3. See [:material-code-braces: LogPublishingOptionsTypeDef](./type_defs.md#logpublishingoptionstypedef) 
4. See [:material-code-braces: VpcEndpointTypeDef](./type_defs.md#vpcendpointtypedef) 
## ListPipelinesResponseTypeDef

```python
# ListPipelinesResponseTypeDef definition

class ListPipelinesResponseTypeDef(TypedDict):
    NextToken: str,
    Pipelines: List[PipelineSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineSummaryTypeDef](./type_defs.md#pipelinesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePipelineResponseTypeDef

```python
# CreatePipelineResponseTypeDef definition

class CreatePipelineResponseTypeDef(TypedDict):
    Pipeline: PipelineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineTypeDef](./type_defs.md#pipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPipelineResponseTypeDef

```python
# GetPipelineResponseTypeDef definition

class GetPipelineResponseTypeDef(TypedDict):
    Pipeline: PipelineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineTypeDef](./type_defs.md#pipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartPipelineResponseTypeDef

```python
# StartPipelineResponseTypeDef definition

class StartPipelineResponseTypeDef(TypedDict):
    Pipeline: PipelineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineTypeDef](./type_defs.md#pipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopPipelineResponseTypeDef

```python
# StopPipelineResponseTypeDef definition

class StopPipelineResponseTypeDef(TypedDict):
    Pipeline: PipelineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineTypeDef](./type_defs.md#pipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePipelineResponseTypeDef

```python
# UpdatePipelineResponseTypeDef definition

class UpdatePipelineResponseTypeDef(TypedDict):
    Pipeline: PipelineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineTypeDef](./type_defs.md#pipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
