# Type definitions

> [Index](../README.md) > [OpenSearchIngestion](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [OpenSearchIngestion](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#opensearchingestion)
    type annotations stubs module [types-aiobotocore-osis](https://pypi.org/project/types-aiobotocore-osis/).

## VpcOptionsUnionTypeDef

```python
# VpcOptionsUnionTypeDef Union usage example

from types_aiobotocore_osis.type_defs import VpcOptionsUnionTypeDef


def get_value() -> VpcOptionsUnionTypeDef:
    return ...


# VpcOptionsUnionTypeDef definition

VpcOptionsUnionTypeDef = Union[
    VpcOptionsTypeDef,  # (1)
    VpcOptionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: VpcOptionsTypeDef](./type_defs.md#vpcoptionstypedef) 
2. See [:material-code-braces: VpcOptionsOutputTypeDef](./type_defs.md#vpcoptionsoutputtypedef) 



## BufferOptionsTypeDef

```python
# BufferOptionsTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import BufferOptionsTypeDef


def get_value() -> BufferOptionsTypeDef:
    return {
        "PersistentBufferEnabled": ...,
    }


# BufferOptionsTypeDef definition

class BufferOptionsTypeDef(TypedDict):
    PersistentBufferEnabled: bool,
```

## ChangeProgressStageTypeDef

```python
# ChangeProgressStageTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import ChangeProgressStageTypeDef


def get_value() -> ChangeProgressStageTypeDef:
    return {
        "Name": ...,
    }


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
# CloudWatchLogDestinationTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import CloudWatchLogDestinationTypeDef


def get_value() -> CloudWatchLogDestinationTypeDef:
    return {
        "LogGroup": ...,
    }


# CloudWatchLogDestinationTypeDef definition

class CloudWatchLogDestinationTypeDef(TypedDict):
    LogGroup: str,
```

## EncryptionAtRestOptionsTypeDef

```python
# EncryptionAtRestOptionsTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import EncryptionAtRestOptionsTypeDef


def get_value() -> EncryptionAtRestOptionsTypeDef:
    return {
        "KmsKeyArn": ...,
    }


# EncryptionAtRestOptionsTypeDef definition

class EncryptionAtRestOptionsTypeDef(TypedDict):
    KmsKeyArn: str,
```

## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "Key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import ResponseMetadataTypeDef


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

## DeletePipelineRequestTypeDef

```python
# DeletePipelineRequestTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import DeletePipelineRequestTypeDef


def get_value() -> DeletePipelineRequestTypeDef:
    return {
        "PipelineName": ...,
    }


# DeletePipelineRequestTypeDef definition

class DeletePipelineRequestTypeDef(TypedDict):
    PipelineName: str,
```

## GetPipelineBlueprintRequestTypeDef

```python
# GetPipelineBlueprintRequestTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import GetPipelineBlueprintRequestTypeDef


def get_value() -> GetPipelineBlueprintRequestTypeDef:
    return {
        "BlueprintName": ...,
    }


# GetPipelineBlueprintRequestTypeDef definition

class GetPipelineBlueprintRequestTypeDef(TypedDict):
    BlueprintName: str,
    Format: NotRequired[str],
```

## PipelineBlueprintTypeDef

```python
# PipelineBlueprintTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import PipelineBlueprintTypeDef


def get_value() -> PipelineBlueprintTypeDef:
    return {
        "BlueprintName": ...,
    }


# PipelineBlueprintTypeDef definition

class PipelineBlueprintTypeDef(TypedDict):
    BlueprintName: NotRequired[str],
    PipelineConfigurationBody: NotRequired[str],
    DisplayName: NotRequired[str],
    DisplayDescription: NotRequired[str],
    Service: NotRequired[str],
    UseCase: NotRequired[str],
```

## GetPipelineChangeProgressRequestTypeDef

```python
# GetPipelineChangeProgressRequestTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import GetPipelineChangeProgressRequestTypeDef


def get_value() -> GetPipelineChangeProgressRequestTypeDef:
    return {
        "PipelineName": ...,
    }


# GetPipelineChangeProgressRequestTypeDef definition

class GetPipelineChangeProgressRequestTypeDef(TypedDict):
    PipelineName: str,
```

## GetPipelineRequestTypeDef

```python
# GetPipelineRequestTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import GetPipelineRequestTypeDef


def get_value() -> GetPipelineRequestTypeDef:
    return {
        "PipelineName": ...,
    }


# GetPipelineRequestTypeDef definition

class GetPipelineRequestTypeDef(TypedDict):
    PipelineName: str,
```

## PipelineBlueprintSummaryTypeDef

```python
# PipelineBlueprintSummaryTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import PipelineBlueprintSummaryTypeDef


def get_value() -> PipelineBlueprintSummaryTypeDef:
    return {
        "BlueprintName": ...,
    }


# PipelineBlueprintSummaryTypeDef definition

class PipelineBlueprintSummaryTypeDef(TypedDict):
    BlueprintName: NotRequired[str],
    DisplayName: NotRequired[str],
    DisplayDescription: NotRequired[str],
    Service: NotRequired[str],
    UseCase: NotRequired[str],
```

## ListPipelinesRequestTypeDef

```python
# ListPipelinesRequestTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import ListPipelinesRequestTypeDef


def get_value() -> ListPipelinesRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListPipelinesRequestTypeDef definition

class ListPipelinesRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "Arn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    Arn: str,
```

## PipelineDestinationTypeDef

```python
# PipelineDestinationTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import PipelineDestinationTypeDef


def get_value() -> PipelineDestinationTypeDef:
    return {
        "ServiceName": ...,
    }


# PipelineDestinationTypeDef definition

class PipelineDestinationTypeDef(TypedDict):
    ServiceName: NotRequired[str],
    Endpoint: NotRequired[str],
```

## PipelineStatusReasonTypeDef

```python
# PipelineStatusReasonTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import PipelineStatusReasonTypeDef


def get_value() -> PipelineStatusReasonTypeDef:
    return {
        "Description": ...,
    }


# PipelineStatusReasonTypeDef definition

class PipelineStatusReasonTypeDef(TypedDict):
    Description: NotRequired[str],
```

## ServiceVpcEndpointTypeDef

```python
# ServiceVpcEndpointTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import ServiceVpcEndpointTypeDef


def get_value() -> ServiceVpcEndpointTypeDef:
    return {
        "ServiceName": ...,
    }


# ServiceVpcEndpointTypeDef definition

class ServiceVpcEndpointTypeDef(TypedDict):
    ServiceName: NotRequired[VpcEndpointServiceNameType],  # (1)
    VpcEndpointId: NotRequired[str],
```

1. See [:material-code-brackets: VpcEndpointServiceNameType](./literals.md#vpcendpointservicenametype) 
## StartPipelineRequestTypeDef

```python
# StartPipelineRequestTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import StartPipelineRequestTypeDef


def get_value() -> StartPipelineRequestTypeDef:
    return {
        "PipelineName": ...,
    }


# StartPipelineRequestTypeDef definition

class StartPipelineRequestTypeDef(TypedDict):
    PipelineName: str,
```

## StopPipelineRequestTypeDef

```python
# StopPipelineRequestTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import StopPipelineRequestTypeDef


def get_value() -> StopPipelineRequestTypeDef:
    return {
        "PipelineName": ...,
    }


# StopPipelineRequestTypeDef definition

class StopPipelineRequestTypeDef(TypedDict):
    PipelineName: str,
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "Arn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    Arn: str,
    TagKeys: Sequence[str],
```

## ValidatePipelineRequestTypeDef

```python
# ValidatePipelineRequestTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import ValidatePipelineRequestTypeDef


def get_value() -> ValidatePipelineRequestTypeDef:
    return {
        "PipelineConfigurationBody": ...,
    }


# ValidatePipelineRequestTypeDef definition

class ValidatePipelineRequestTypeDef(TypedDict):
    PipelineConfigurationBody: str,
```

## ValidationMessageTypeDef

```python
# ValidationMessageTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import ValidationMessageTypeDef


def get_value() -> ValidationMessageTypeDef:
    return {
        "Message": ...,
    }


# ValidationMessageTypeDef definition

class ValidationMessageTypeDef(TypedDict):
    Message: NotRequired[str],
```

## VpcAttachmentOptionsTypeDef

```python
# VpcAttachmentOptionsTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import VpcAttachmentOptionsTypeDef


def get_value() -> VpcAttachmentOptionsTypeDef:
    return {
        "AttachToVpc": ...,
    }


# VpcAttachmentOptionsTypeDef definition

class VpcAttachmentOptionsTypeDef(TypedDict):
    AttachToVpc: bool,
    CidrBlock: NotRequired[str],
```

## ChangeProgressStatusTypeDef

```python
# ChangeProgressStatusTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import ChangeProgressStatusTypeDef


def get_value() -> ChangeProgressStatusTypeDef:
    return {
        "StartTime": ...,
    }


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
# LogPublishingOptionsTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import LogPublishingOptionsTypeDef


def get_value() -> LogPublishingOptionsTypeDef:
    return {
        "IsLoggingEnabled": ...,
    }


# LogPublishingOptionsTypeDef definition

class LogPublishingOptionsTypeDef(TypedDict):
    IsLoggingEnabled: NotRequired[bool],
    CloudWatchLogDestination: NotRequired[CloudWatchLogDestinationTypeDef],  # (1)
```

1. See [:material-code-braces: CloudWatchLogDestinationTypeDef](./type_defs.md#cloudwatchlogdestinationtypedef) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "Arn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    Arn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPipelineBlueprintResponseTypeDef

```python
# GetPipelineBlueprintResponseTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import GetPipelineBlueprintResponseTypeDef


def get_value() -> GetPipelineBlueprintResponseTypeDef:
    return {
        "Blueprint": ...,
    }


# GetPipelineBlueprintResponseTypeDef definition

class GetPipelineBlueprintResponseTypeDef(TypedDict):
    Blueprint: PipelineBlueprintTypeDef,  # (1)
    Format: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineBlueprintTypeDef](./type_defs.md#pipelineblueprinttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPipelineBlueprintsResponseTypeDef

```python
# ListPipelineBlueprintsResponseTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import ListPipelineBlueprintsResponseTypeDef


def get_value() -> ListPipelineBlueprintsResponseTypeDef:
    return {
        "Blueprints": ...,
    }


# ListPipelineBlueprintsResponseTypeDef definition

class ListPipelineBlueprintsResponseTypeDef(TypedDict):
    Blueprints: List[PipelineBlueprintSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineBlueprintSummaryTypeDef](./type_defs.md#pipelineblueprintsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PipelineSummaryTypeDef

```python
# PipelineSummaryTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import PipelineSummaryTypeDef


def get_value() -> PipelineSummaryTypeDef:
    return {
        "Status": ...,
    }


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
    Destinations: NotRequired[List[PipelineDestinationTypeDef]],  # (3)
    Tags: NotRequired[List[TagTypeDef]],  # (4)
```

1. See [:material-code-brackets: PipelineStatusType](./literals.md#pipelinestatustype) 
2. See [:material-code-braces: PipelineStatusReasonTypeDef](./type_defs.md#pipelinestatusreasontypedef) 
3. See [:material-code-braces: PipelineDestinationTypeDef](./type_defs.md#pipelinedestinationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ValidatePipelineResponseTypeDef

```python
# ValidatePipelineResponseTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import ValidatePipelineResponseTypeDef


def get_value() -> ValidatePipelineResponseTypeDef:
    return {
        "isValid": ...,
    }


# ValidatePipelineResponseTypeDef definition

class ValidatePipelineResponseTypeDef(TypedDict):
    isValid: bool,
    Errors: List[ValidationMessageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ValidationMessageTypeDef](./type_defs.md#validationmessagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VpcOptionsOutputTypeDef

```python
# VpcOptionsOutputTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import VpcOptionsOutputTypeDef


def get_value() -> VpcOptionsOutputTypeDef:
    return {
        "SubnetIds": ...,
    }


# VpcOptionsOutputTypeDef definition

class VpcOptionsOutputTypeDef(TypedDict):
    SubnetIds: List[str],
    SecurityGroupIds: NotRequired[List[str]],
    VpcAttachmentOptions: NotRequired[VpcAttachmentOptionsTypeDef],  # (1)
    VpcEndpointManagement: NotRequired[VpcEndpointManagementType],  # (2)
```

1. See [:material-code-braces: VpcAttachmentOptionsTypeDef](./type_defs.md#vpcattachmentoptionstypedef) 
2. See [:material-code-brackets: VpcEndpointManagementType](./literals.md#vpcendpointmanagementtype) 
## VpcOptionsTypeDef

```python
# VpcOptionsTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import VpcOptionsTypeDef


def get_value() -> VpcOptionsTypeDef:
    return {
        "SubnetIds": ...,
    }


# VpcOptionsTypeDef definition

class VpcOptionsTypeDef(TypedDict):
    SubnetIds: Sequence[str],
    SecurityGroupIds: NotRequired[Sequence[str]],
    VpcAttachmentOptions: NotRequired[VpcAttachmentOptionsTypeDef],  # (1)
    VpcEndpointManagement: NotRequired[VpcEndpointManagementType],  # (2)
```

1. See [:material-code-braces: VpcAttachmentOptionsTypeDef](./type_defs.md#vpcattachmentoptionstypedef) 
2. See [:material-code-brackets: VpcEndpointManagementType](./literals.md#vpcendpointmanagementtype) 
## GetPipelineChangeProgressResponseTypeDef

```python
# GetPipelineChangeProgressResponseTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import GetPipelineChangeProgressResponseTypeDef


def get_value() -> GetPipelineChangeProgressResponseTypeDef:
    return {
        "ChangeProgressStatuses": ...,
    }


# GetPipelineChangeProgressResponseTypeDef definition

class GetPipelineChangeProgressResponseTypeDef(TypedDict):
    ChangeProgressStatuses: List[ChangeProgressStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChangeProgressStatusTypeDef](./type_defs.md#changeprogressstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePipelineRequestTypeDef

```python
# UpdatePipelineRequestTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import UpdatePipelineRequestTypeDef


def get_value() -> UpdatePipelineRequestTypeDef:
    return {
        "PipelineName": ...,
    }


# UpdatePipelineRequestTypeDef definition

class UpdatePipelineRequestTypeDef(TypedDict):
    PipelineName: str,
    MinUnits: NotRequired[int],
    MaxUnits: NotRequired[int],
    PipelineConfigurationBody: NotRequired[str],
    LogPublishingOptions: NotRequired[LogPublishingOptionsTypeDef],  # (1)
    BufferOptions: NotRequired[BufferOptionsTypeDef],  # (2)
    EncryptionAtRestOptions: NotRequired[EncryptionAtRestOptionsTypeDef],  # (3)
```

1. See [:material-code-braces: LogPublishingOptionsTypeDef](./type_defs.md#logpublishingoptionstypedef) 
2. See [:material-code-braces: BufferOptionsTypeDef](./type_defs.md#bufferoptionstypedef) 
3. See [:material-code-braces: EncryptionAtRestOptionsTypeDef](./type_defs.md#encryptionatrestoptionstypedef) 
## ListPipelinesResponseTypeDef

```python
# ListPipelinesResponseTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import ListPipelinesResponseTypeDef


def get_value() -> ListPipelinesResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListPipelinesResponseTypeDef definition

class ListPipelinesResponseTypeDef(TypedDict):
    Pipelines: List[PipelineSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PipelineSummaryTypeDef](./type_defs.md#pipelinesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VpcEndpointTypeDef

```python
# VpcEndpointTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import VpcEndpointTypeDef


def get_value() -> VpcEndpointTypeDef:
    return {
        "VpcEndpointId": ...,
    }


# VpcEndpointTypeDef definition

class VpcEndpointTypeDef(TypedDict):
    VpcEndpointId: NotRequired[str],
    VpcId: NotRequired[str],
    VpcOptions: NotRequired[VpcOptionsOutputTypeDef],  # (1)
```

1. See [:material-code-braces: VpcOptionsOutputTypeDef](./type_defs.md#vpcoptionsoutputtypedef) 
## PipelineTypeDef

```python
# PipelineTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import PipelineTypeDef


def get_value() -> PipelineTypeDef:
    return {
        "PipelineName": ...,
    }


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
    BufferOptions: NotRequired[BufferOptionsTypeDef],  # (5)
    EncryptionAtRestOptions: NotRequired[EncryptionAtRestOptionsTypeDef],  # (6)
    VpcEndpointService: NotRequired[str],
    ServiceVpcEndpoints: NotRequired[List[ServiceVpcEndpointTypeDef]],  # (7)
    Destinations: NotRequired[List[PipelineDestinationTypeDef]],  # (8)
    Tags: NotRequired[List[TagTypeDef]],  # (9)
```

1. See [:material-code-brackets: PipelineStatusType](./literals.md#pipelinestatustype) 
2. See [:material-code-braces: PipelineStatusReasonTypeDef](./type_defs.md#pipelinestatusreasontypedef) 
3. See [:material-code-braces: LogPublishingOptionsTypeDef](./type_defs.md#logpublishingoptionstypedef) 
4. See [:material-code-braces: VpcEndpointTypeDef](./type_defs.md#vpcendpointtypedef) 
5. See [:material-code-braces: BufferOptionsTypeDef](./type_defs.md#bufferoptionstypedef) 
6. See [:material-code-braces: EncryptionAtRestOptionsTypeDef](./type_defs.md#encryptionatrestoptionstypedef) 
7. See [:material-code-braces: ServiceVpcEndpointTypeDef](./type_defs.md#servicevpcendpointtypedef) 
8. See [:material-code-braces: PipelineDestinationTypeDef](./type_defs.md#pipelinedestinationtypedef) 
9. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePipelineRequestTypeDef

```python
# CreatePipelineRequestTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import CreatePipelineRequestTypeDef


def get_value() -> CreatePipelineRequestTypeDef:
    return {
        "PipelineName": ...,
    }


# CreatePipelineRequestTypeDef definition

class CreatePipelineRequestTypeDef(TypedDict):
    PipelineName: str,
    MinUnits: int,
    MaxUnits: int,
    PipelineConfigurationBody: str,
    LogPublishingOptions: NotRequired[LogPublishingOptionsTypeDef],  # (1)
    VpcOptions: NotRequired[VpcOptionsUnionTypeDef],  # (2)
    BufferOptions: NotRequired[BufferOptionsTypeDef],  # (3)
    EncryptionAtRestOptions: NotRequired[EncryptionAtRestOptionsTypeDef],  # (4)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (5)
```

1. See [:material-code-braces: LogPublishingOptionsTypeDef](./type_defs.md#logpublishingoptionstypedef) 
2. See [:material-code-braces: VpcOptionsTypeDef](./type_defs.md#vpcoptionstypedef) [:material-code-braces: VpcOptionsOutputTypeDef](./type_defs.md#vpcoptionsoutputtypedef) 
3. See [:material-code-braces: BufferOptionsTypeDef](./type_defs.md#bufferoptionstypedef) 
4. See [:material-code-braces: EncryptionAtRestOptionsTypeDef](./type_defs.md#encryptionatrestoptionstypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePipelineResponseTypeDef

```python
# CreatePipelineResponseTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import CreatePipelineResponseTypeDef


def get_value() -> CreatePipelineResponseTypeDef:
    return {
        "Pipeline": ...,
    }


# CreatePipelineResponseTypeDef definition

class CreatePipelineResponseTypeDef(TypedDict):
    Pipeline: PipelineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineTypeDef](./type_defs.md#pipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPipelineResponseTypeDef

```python
# GetPipelineResponseTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import GetPipelineResponseTypeDef


def get_value() -> GetPipelineResponseTypeDef:
    return {
        "Pipeline": ...,
    }


# GetPipelineResponseTypeDef definition

class GetPipelineResponseTypeDef(TypedDict):
    Pipeline: PipelineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineTypeDef](./type_defs.md#pipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartPipelineResponseTypeDef

```python
# StartPipelineResponseTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import StartPipelineResponseTypeDef


def get_value() -> StartPipelineResponseTypeDef:
    return {
        "Pipeline": ...,
    }


# StartPipelineResponseTypeDef definition

class StartPipelineResponseTypeDef(TypedDict):
    Pipeline: PipelineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineTypeDef](./type_defs.md#pipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopPipelineResponseTypeDef

```python
# StopPipelineResponseTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import StopPipelineResponseTypeDef


def get_value() -> StopPipelineResponseTypeDef:
    return {
        "Pipeline": ...,
    }


# StopPipelineResponseTypeDef definition

class StopPipelineResponseTypeDef(TypedDict):
    Pipeline: PipelineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineTypeDef](./type_defs.md#pipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePipelineResponseTypeDef

```python
# UpdatePipelineResponseTypeDef TypedDict usage example

from types_aiobotocore_osis.type_defs import UpdatePipelineResponseTypeDef


def get_value() -> UpdatePipelineResponseTypeDef:
    return {
        "Pipeline": ...,
    }


# UpdatePipelineResponseTypeDef definition

class UpdatePipelineResponseTypeDef(TypedDict):
    Pipeline: PipelineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineTypeDef](./type_defs.md#pipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
