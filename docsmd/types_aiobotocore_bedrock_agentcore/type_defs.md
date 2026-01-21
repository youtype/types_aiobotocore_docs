# Type definitions

> [Index](../README.md) > [BedrockAgentCore](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [BedrockAgentCore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore.html#bedrockagentcore)
    type annotations stubs module [types-aiobotocore-bedrock-agentcore](https://pypi.org/project/types-aiobotocore-bedrock-agentcore/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_bedrock_agentcore.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    aiobotocore.response.StreamingBody,
]
```


## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_bedrock_agentcore.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime.datetime,
    str,
]
```


## PayloadTypeUnionTypeDef

```python
# PayloadTypeUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agentcore.type_defs import PayloadTypeUnionTypeDef


def get_value() -> PayloadTypeUnionTypeDef:
    return ...


# PayloadTypeUnionTypeDef definition

PayloadTypeUnionTypeDef = Union[
    PayloadTypeTypeDef,  # (1)
    PayloadTypeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PayloadTypeTypeDef](./type_defs.md#payloadtypetypedef)
2. See [:material-code-braces: PayloadTypeOutputTypeDef](./type_defs.md#payloadtypeoutputtypedef)



## AccessDeniedExceptionTypeDef

```python
# AccessDeniedExceptionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import AccessDeniedExceptionTypeDef


def get_value() -> AccessDeniedExceptionTypeDef:
    return {
        "message": ...,
    }


# AccessDeniedExceptionTypeDef definition

class AccessDeniedExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```


## ActorSummaryTypeDef

```python
# ActorSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ActorSummaryTypeDef


def get_value() -> ActorSummaryTypeDef:
    return {
        "actorId": ...,
    }


# ActorSummaryTypeDef definition

class ActorSummaryTypeDef(TypedDict):
    actorId: str,
```


## AutomationStreamTypeDef

```python
# AutomationStreamTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import AutomationStreamTypeDef


def get_value() -> AutomationStreamTypeDef:
    return {
        "streamEndpoint": ...,
    }


# AutomationStreamTypeDef definition

class AutomationStreamTypeDef(TypedDict):
    streamEndpoint: str,
    streamStatus: AutomationStreamStatusType,  # (1)
```

1. See [:material-code-brackets: AutomationStreamStatusType](./literals.md#automationstreamstatustype)

## AutomationStreamUpdateTypeDef

```python
# AutomationStreamUpdateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import AutomationStreamUpdateTypeDef


def get_value() -> AutomationStreamUpdateTypeDef:
    return {
        "streamStatus": ...,
    }


# AutomationStreamUpdateTypeDef definition

class AutomationStreamUpdateTypeDef(TypedDict):
    streamStatus: NotRequired[AutomationStreamStatusType],  # (1)
```

1. See [:material-code-brackets: AutomationStreamStatusType](./literals.md#automationstreamstatustype)

## MemoryRecordOutputTypeDef

```python
# MemoryRecordOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import MemoryRecordOutputTypeDef


def get_value() -> MemoryRecordOutputTypeDef:
    return {
        "memoryRecordId": ...,
    }


# MemoryRecordOutputTypeDef definition

class MemoryRecordOutputTypeDef(TypedDict):
    memoryRecordId: str,
    status: MemoryRecordStatusType,  # (1)
    requestIdentifier: NotRequired[str],
    errorCode: NotRequired[int],
    errorMessage: NotRequired[str],
```

1. See [:material-code-brackets: MemoryRecordStatusType](./literals.md#memoryrecordstatustype)

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```


## MemoryRecordDeleteInputTypeDef

```python
# MemoryRecordDeleteInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import MemoryRecordDeleteInputTypeDef


def get_value() -> MemoryRecordDeleteInputTypeDef:
    return {
        "memoryRecordId": ...,
    }


# MemoryRecordDeleteInputTypeDef definition

class MemoryRecordDeleteInputTypeDef(TypedDict):
    memoryRecordId: str,
```


## BranchFilterTypeDef

```python
# BranchFilterTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import BranchFilterTypeDef


def get_value() -> BranchFilterTypeDef:
    return {
        "name": ...,
    }


# BranchFilterTypeDef definition

class BranchFilterTypeDef(TypedDict):
    name: str,
    includeParentBranches: NotRequired[bool],
```


## BranchTypeDef

```python
# BranchTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import BranchTypeDef


def get_value() -> BranchTypeDef:
    return {
        "rootEventId": ...,
    }


# BranchTypeDef definition

class BranchTypeDef(TypedDict):
    name: str,
    rootEventId: NotRequired[str],
```


## LiveViewStreamTypeDef

```python
# LiveViewStreamTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import LiveViewStreamTypeDef


def get_value() -> LiveViewStreamTypeDef:
    return {
        "streamEndpoint": ...,
    }


# LiveViewStreamTypeDef definition

class LiveViewStreamTypeDef(TypedDict):
    streamEndpoint: NotRequired[str],
```


## BrowserSessionSummaryTypeDef

```python
# BrowserSessionSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import BrowserSessionSummaryTypeDef


def get_value() -> BrowserSessionSummaryTypeDef:
    return {
        "browserIdentifier": ...,
    }


# BrowserSessionSummaryTypeDef definition

class BrowserSessionSummaryTypeDef(TypedDict):
    browserIdentifier: str,
    sessionId: str,
    status: BrowserSessionStatusType,  # (1)
    createdAt: datetime.datetime,
    name: NotRequired[str],
    lastUpdatedAt: NotRequired[datetime.datetime],
```

1. See [:material-code-brackets: BrowserSessionStatusType](./literals.md#browsersessionstatustype)

## ToolResultStructuredContentTypeDef

```python
# ToolResultStructuredContentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ToolResultStructuredContentTypeDef


def get_value() -> ToolResultStructuredContentTypeDef:
    return {
        "taskId": ...,
    }


# ToolResultStructuredContentTypeDef definition

class ToolResultStructuredContentTypeDef(TypedDict):
    taskId: NotRequired[str],
    taskStatus: NotRequired[TaskStatusType],  # (1)
    stdout: NotRequired[str],
    stderr: NotRequired[str],
    exitCode: NotRequired[int],
    executionTime: NotRequired[float],
```

1. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype)

## CodeInterpreterSessionSummaryTypeDef

```python
# CodeInterpreterSessionSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import CodeInterpreterSessionSummaryTypeDef


def get_value() -> CodeInterpreterSessionSummaryTypeDef:
    return {
        "codeInterpreterIdentifier": ...,
    }


# CodeInterpreterSessionSummaryTypeDef definition

class CodeInterpreterSessionSummaryTypeDef(TypedDict):
    codeInterpreterIdentifier: str,
    sessionId: str,
    status: CodeInterpreterSessionStatusType,  # (1)
    createdAt: datetime.datetime,
    name: NotRequired[str],
    lastUpdatedAt: NotRequired[datetime.datetime],
```

1. See [:material-code-brackets: CodeInterpreterSessionStatusType](./literals.md#codeinterpretersessionstatustype)

## ConflictExceptionTypeDef

```python
# ConflictExceptionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ConflictExceptionTypeDef


def get_value() -> ConflictExceptionTypeDef:
    return {
        "message": ...,
    }


# ConflictExceptionTypeDef definition

class ConflictExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```


## InternalServerExceptionTypeDef

```python
# InternalServerExceptionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import InternalServerExceptionTypeDef


def get_value() -> InternalServerExceptionTypeDef:
    return {
        "message": ...,
    }


# InternalServerExceptionTypeDef definition

class InternalServerExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```


## ResourceNotFoundExceptionTypeDef

```python
# ResourceNotFoundExceptionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ResourceNotFoundExceptionTypeDef


def get_value() -> ResourceNotFoundExceptionTypeDef:
    return {
        "message": ...,
    }


# ResourceNotFoundExceptionTypeDef definition

class ResourceNotFoundExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```


## ServiceQuotaExceededExceptionTypeDef

```python
# ServiceQuotaExceededExceptionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ServiceQuotaExceededExceptionTypeDef


def get_value() -> ServiceQuotaExceededExceptionTypeDef:
    return {
        "message": ...,
    }


# ServiceQuotaExceededExceptionTypeDef definition

class ServiceQuotaExceededExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```


## ThrottlingExceptionTypeDef

```python
# ThrottlingExceptionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ThrottlingExceptionTypeDef


def get_value() -> ThrottlingExceptionTypeDef:
    return {
        "message": ...,
    }


# ThrottlingExceptionTypeDef definition

class ThrottlingExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```


## UserIdentifierTypeDef

```python
# UserIdentifierTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import UserIdentifierTypeDef


def get_value() -> UserIdentifierTypeDef:
    return {
        "userToken": ...,
    }


# UserIdentifierTypeDef definition

class UserIdentifierTypeDef(TypedDict):
    userToken: NotRequired[str],
    userId: NotRequired[str],
```


## ResourceContentTypeDef

```python
# ResourceContentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ResourceContentTypeDef


def get_value() -> ResourceContentTypeDef:
    return {
        "type": ...,
    }


# ResourceContentTypeDef definition

class ResourceContentTypeDef(TypedDict):
    type: ResourceContentTypeType,  # (1)
    uri: NotRequired[str],
    mimeType: NotRequired[str],
    text: NotRequired[str],
    blob: NotRequired[bytes],
```

1. See [:material-code-brackets: ResourceContentTypeType](./literals.md#resourcecontenttypetype)

## ContentTypeDef

```python
# ContentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ContentTypeDef


def get_value() -> ContentTypeDef:
    return {
        "text": ...,
    }


# ContentTypeDef definition

class ContentTypeDef(TypedDict):
    text: NotRequired[str],
```


## SpanContextTypeDef

```python
# SpanContextTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import SpanContextTypeDef


def get_value() -> SpanContextTypeDef:
    return {
        "sessionId": ...,
    }


# SpanContextTypeDef definition

class SpanContextTypeDef(TypedDict):
    sessionId: str,
    traceId: NotRequired[str],
    spanId: NotRequired[str],
```


## MetadataValueTypeDef

```python
# MetadataValueTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import MetadataValueTypeDef


def get_value() -> MetadataValueTypeDef:
    return {
        "stringValue": ...,
    }


# MetadataValueTypeDef definition

class MetadataValueTypeDef(TypedDict):
    stringValue: NotRequired[str],
```


## DeleteEventInputTypeDef

```python
# DeleteEventInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import DeleteEventInputTypeDef


def get_value() -> DeleteEventInputTypeDef:
    return {
        "memoryId": ...,
    }


# DeleteEventInputTypeDef definition

class DeleteEventInputTypeDef(TypedDict):
    memoryId: str,
    sessionId: str,
    eventId: str,
    actorId: str,
```


## DeleteMemoryRecordInputTypeDef

```python
# DeleteMemoryRecordInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import DeleteMemoryRecordInputTypeDef


def get_value() -> DeleteMemoryRecordInputTypeDef:
    return {
        "memoryId": ...,
    }


# DeleteMemoryRecordInputTypeDef definition

class DeleteMemoryRecordInputTypeDef(TypedDict):
    memoryId: str,
    memoryRecordId: str,
```


## EvaluationInputTypeDef

```python
# EvaluationInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import EvaluationInputTypeDef


def get_value() -> EvaluationInputTypeDef:
    return {
        "sessionSpans": ...,
    }


# EvaluationInputTypeDef definition

class EvaluationInputTypeDef(TypedDict):
    sessionSpans: NotRequired[Sequence[Mapping[str, Any]]],
```


## EvaluationTargetTypeDef

```python
# EvaluationTargetTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import EvaluationTargetTypeDef


def get_value() -> EvaluationTargetTypeDef:
    return {
        "spanIds": ...,
    }


# EvaluationTargetTypeDef definition

class EvaluationTargetTypeDef(TypedDict):
    spanIds: NotRequired[Sequence[str]],
    traceIds: NotRequired[Sequence[str]],
```


## TokenUsageTypeDef

```python
# TokenUsageTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import TokenUsageTypeDef


def get_value() -> TokenUsageTypeDef:
    return {
        "inputTokens": ...,
    }


# TokenUsageTypeDef definition

class TokenUsageTypeDef(TypedDict):
    inputTokens: NotRequired[int],
    outputTokens: NotRequired[int],
    totalTokens: NotRequired[int],
```


## LeftExpressionTypeDef

```python
# LeftExpressionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import LeftExpressionTypeDef


def get_value() -> LeftExpressionTypeDef:
    return {
        "metadataKey": ...,
    }


# LeftExpressionTypeDef definition

class LeftExpressionTypeDef(TypedDict):
    metadataKey: NotRequired[str],
```


## ExtractionJobFilterInputTypeDef

```python
# ExtractionJobFilterInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ExtractionJobFilterInputTypeDef


def get_value() -> ExtractionJobFilterInputTypeDef:
    return {
        "strategyId": ...,
    }


# ExtractionJobFilterInputTypeDef definition

class ExtractionJobFilterInputTypeDef(TypedDict):
    strategyId: NotRequired[str],
    sessionId: NotRequired[str],
    actorId: NotRequired[str],
    status: NotRequired[ExtractionJobStatusType],  # (1)
```

1. See [:material-code-brackets: ExtractionJobStatusType](./literals.md#extractionjobstatustype)

## MessageMetadataTypeDef

```python
# MessageMetadataTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import MessageMetadataTypeDef


def get_value() -> MessageMetadataTypeDef:
    return {
        "eventId": ...,
    }


# MessageMetadataTypeDef definition

class MessageMetadataTypeDef(TypedDict):
    eventId: str,
    messageIndex: int,
```


## ExtractionJobTypeDef

```python
# ExtractionJobTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ExtractionJobTypeDef


def get_value() -> ExtractionJobTypeDef:
    return {
        "jobId": ...,
    }


# ExtractionJobTypeDef definition

class ExtractionJobTypeDef(TypedDict):
    jobId: str,
```


## GetAgentCardRequestTypeDef

```python
# GetAgentCardRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import GetAgentCardRequestTypeDef


def get_value() -> GetAgentCardRequestTypeDef:
    return {
        "agentRuntimeArn": ...,
    }


# GetAgentCardRequestTypeDef definition

class GetAgentCardRequestTypeDef(TypedDict):
    agentRuntimeArn: str,
    runtimeSessionId: NotRequired[str],
    qualifier: NotRequired[str],
```


## GetBrowserSessionRequestTypeDef

```python
# GetBrowserSessionRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import GetBrowserSessionRequestTypeDef


def get_value() -> GetBrowserSessionRequestTypeDef:
    return {
        "browserIdentifier": ...,
    }


# GetBrowserSessionRequestTypeDef definition

class GetBrowserSessionRequestTypeDef(TypedDict):
    browserIdentifier: str,
    sessionId: str,
```


## ViewPortTypeDef

```python
# ViewPortTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ViewPortTypeDef


def get_value() -> ViewPortTypeDef:
    return {
        "width": ...,
    }


# ViewPortTypeDef definition

class ViewPortTypeDef(TypedDict):
    width: int,
    height: int,
```


## GetCodeInterpreterSessionRequestTypeDef

```python
# GetCodeInterpreterSessionRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import GetCodeInterpreterSessionRequestTypeDef


def get_value() -> GetCodeInterpreterSessionRequestTypeDef:
    return {
        "codeInterpreterIdentifier": ...,
    }


# GetCodeInterpreterSessionRequestTypeDef definition

class GetCodeInterpreterSessionRequestTypeDef(TypedDict):
    codeInterpreterIdentifier: str,
    sessionId: str,
```


## GetEventInputTypeDef

```python
# GetEventInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import GetEventInputTypeDef


def get_value() -> GetEventInputTypeDef:
    return {
        "memoryId": ...,
    }


# GetEventInputTypeDef definition

class GetEventInputTypeDef(TypedDict):
    memoryId: str,
    sessionId: str,
    actorId: str,
    eventId: str,
```


## GetMemoryRecordInputTypeDef

```python
# GetMemoryRecordInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import GetMemoryRecordInputTypeDef


def get_value() -> GetMemoryRecordInputTypeDef:
    return {
        "memoryId": ...,
    }


# GetMemoryRecordInputTypeDef definition

class GetMemoryRecordInputTypeDef(TypedDict):
    memoryId: str,
    memoryRecordId: str,
```


## GetResourceApiKeyRequestTypeDef

```python
# GetResourceApiKeyRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import GetResourceApiKeyRequestTypeDef


def get_value() -> GetResourceApiKeyRequestTypeDef:
    return {
        "workloadIdentityToken": ...,
    }


# GetResourceApiKeyRequestTypeDef definition

class GetResourceApiKeyRequestTypeDef(TypedDict):
    workloadIdentityToken: str,
    resourceCredentialProviderName: str,
```


## GetResourceOauth2TokenRequestTypeDef

```python
# GetResourceOauth2TokenRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import GetResourceOauth2TokenRequestTypeDef


def get_value() -> GetResourceOauth2TokenRequestTypeDef:
    return {
        "workloadIdentityToken": ...,
    }


# GetResourceOauth2TokenRequestTypeDef definition

class GetResourceOauth2TokenRequestTypeDef(TypedDict):
    workloadIdentityToken: str,
    resourceCredentialProviderName: str,
    scopes: Sequence[str],
    oauth2Flow: Oauth2FlowTypeType,  # (1)
    sessionUri: NotRequired[str],
    resourceOauth2ReturnUrl: NotRequired[str],
    forceAuthentication: NotRequired[bool],
    customParameters: NotRequired[Mapping[str, str]],
    customState: NotRequired[str],
```

1. See [:material-code-brackets: Oauth2FlowTypeType](./literals.md#oauth2flowtypetype)

## GetWorkloadAccessTokenForJWTRequestTypeDef

```python
# GetWorkloadAccessTokenForJWTRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import GetWorkloadAccessTokenForJWTRequestTypeDef


def get_value() -> GetWorkloadAccessTokenForJWTRequestTypeDef:
    return {
        "workloadName": ...,
    }


# GetWorkloadAccessTokenForJWTRequestTypeDef definition

class GetWorkloadAccessTokenForJWTRequestTypeDef(TypedDict):
    workloadName: str,
    userToken: str,
```


## GetWorkloadAccessTokenForUserIdRequestTypeDef

```python
# GetWorkloadAccessTokenForUserIdRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import GetWorkloadAccessTokenForUserIdRequestTypeDef


def get_value() -> GetWorkloadAccessTokenForUserIdRequestTypeDef:
    return {
        "workloadName": ...,
    }


# GetWorkloadAccessTokenForUserIdRequestTypeDef definition

class GetWorkloadAccessTokenForUserIdRequestTypeDef(TypedDict):
    workloadName: str,
    userId: str,
```


## GetWorkloadAccessTokenRequestTypeDef

```python
# GetWorkloadAccessTokenRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import GetWorkloadAccessTokenRequestTypeDef


def get_value() -> GetWorkloadAccessTokenRequestTypeDef:
    return {
        "workloadName": ...,
    }


# GetWorkloadAccessTokenRequestTypeDef definition

class GetWorkloadAccessTokenRequestTypeDef(TypedDict):
    workloadName: str,
```


## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import PaginatorConfigTypeDef


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


## ListActorsInputTypeDef

```python
# ListActorsInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ListActorsInputTypeDef


def get_value() -> ListActorsInputTypeDef:
    return {
        "memoryId": ...,
    }


# ListActorsInputTypeDef definition

class ListActorsInputTypeDef(TypedDict):
    memoryId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListBrowserSessionsRequestTypeDef

```python
# ListBrowserSessionsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ListBrowserSessionsRequestTypeDef


def get_value() -> ListBrowserSessionsRequestTypeDef:
    return {
        "browserIdentifier": ...,
    }


# ListBrowserSessionsRequestTypeDef definition

class ListBrowserSessionsRequestTypeDef(TypedDict):
    browserIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    status: NotRequired[BrowserSessionStatusType],  # (1)
```

1. See [:material-code-brackets: BrowserSessionStatusType](./literals.md#browsersessionstatustype)

## ListCodeInterpreterSessionsRequestTypeDef

```python
# ListCodeInterpreterSessionsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ListCodeInterpreterSessionsRequestTypeDef


def get_value() -> ListCodeInterpreterSessionsRequestTypeDef:
    return {
        "codeInterpreterIdentifier": ...,
    }


# ListCodeInterpreterSessionsRequestTypeDef definition

class ListCodeInterpreterSessionsRequestTypeDef(TypedDict):
    codeInterpreterIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    status: NotRequired[CodeInterpreterSessionStatusType],  # (1)
```

1. See [:material-code-brackets: CodeInterpreterSessionStatusType](./literals.md#codeinterpretersessionstatustype)

## ListMemoryRecordsInputTypeDef

```python
# ListMemoryRecordsInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ListMemoryRecordsInputTypeDef


def get_value() -> ListMemoryRecordsInputTypeDef:
    return {
        "memoryId": ...,
    }


# ListMemoryRecordsInputTypeDef definition

class ListMemoryRecordsInputTypeDef(TypedDict):
    memoryId: str,
    namespace: str,
    memoryStrategyId: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListSessionsInputTypeDef

```python
# ListSessionsInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ListSessionsInputTypeDef


def get_value() -> ListSessionsInputTypeDef:
    return {
        "memoryId": ...,
    }


# ListSessionsInputTypeDef definition

class ListSessionsInputTypeDef(TypedDict):
    memoryId: str,
    actorId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## SessionSummaryTypeDef

```python
# SessionSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import SessionSummaryTypeDef


def get_value() -> SessionSummaryTypeDef:
    return {
        "sessionId": ...,
    }


# SessionSummaryTypeDef definition

class SessionSummaryTypeDef(TypedDict):
    sessionId: str,
    actorId: str,
    createdAt: datetime.datetime,
```


## MemoryContentTypeDef

```python
# MemoryContentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import MemoryContentTypeDef


def get_value() -> MemoryContentTypeDef:
    return {
        "text": ...,
    }


# MemoryContentTypeDef definition

class MemoryContentTypeDef(TypedDict):
    text: NotRequired[str],
```


## StartCodeInterpreterSessionRequestTypeDef

```python
# StartCodeInterpreterSessionRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import StartCodeInterpreterSessionRequestTypeDef


def get_value() -> StartCodeInterpreterSessionRequestTypeDef:
    return {
        "codeInterpreterIdentifier": ...,
    }


# StartCodeInterpreterSessionRequestTypeDef definition

class StartCodeInterpreterSessionRequestTypeDef(TypedDict):
    codeInterpreterIdentifier: str,
    traceId: NotRequired[str],
    traceParent: NotRequired[str],
    name: NotRequired[str],
    sessionTimeoutSeconds: NotRequired[int],
    clientToken: NotRequired[str],
```


## StopBrowserSessionRequestTypeDef

```python
# StopBrowserSessionRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import StopBrowserSessionRequestTypeDef


def get_value() -> StopBrowserSessionRequestTypeDef:
    return {
        "browserIdentifier": ...,
    }


# StopBrowserSessionRequestTypeDef definition

class StopBrowserSessionRequestTypeDef(TypedDict):
    browserIdentifier: str,
    sessionId: str,
    traceId: NotRequired[str],
    traceParent: NotRequired[str],
    clientToken: NotRequired[str],
```


## StopCodeInterpreterSessionRequestTypeDef

```python
# StopCodeInterpreterSessionRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import StopCodeInterpreterSessionRequestTypeDef


def get_value() -> StopCodeInterpreterSessionRequestTypeDef:
    return {
        "codeInterpreterIdentifier": ...,
    }


# StopCodeInterpreterSessionRequestTypeDef definition

class StopCodeInterpreterSessionRequestTypeDef(TypedDict):
    codeInterpreterIdentifier: str,
    sessionId: str,
    traceId: NotRequired[str],
    traceParent: NotRequired[str],
    clientToken: NotRequired[str],
```


## StopRuntimeSessionRequestTypeDef

```python
# StopRuntimeSessionRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import StopRuntimeSessionRequestTypeDef


def get_value() -> StopRuntimeSessionRequestTypeDef:
    return {
        "runtimeSessionId": ...,
    }


# StopRuntimeSessionRequestTypeDef definition

class StopRuntimeSessionRequestTypeDef(TypedDict):
    runtimeSessionId: str,
    agentRuntimeArn: str,
    qualifier: NotRequired[str],
    clientToken: NotRequired[str],
```


## ValidationExceptionFieldTypeDef

```python
# ValidationExceptionFieldTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ValidationExceptionFieldTypeDef


def get_value() -> ValidationExceptionFieldTypeDef:
    return {
        "name": ...,
    }


# ValidationExceptionFieldTypeDef definition

class ValidationExceptionFieldTypeDef(TypedDict):
    name: str,
    message: str,
```


## StreamUpdateTypeDef

```python
# StreamUpdateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import StreamUpdateTypeDef


def get_value() -> StreamUpdateTypeDef:
    return {
        "automationStreamUpdate": ...,
    }


# StreamUpdateTypeDef definition

class StreamUpdateTypeDef(TypedDict):
    automationStreamUpdate: NotRequired[AutomationStreamUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: AutomationStreamUpdateTypeDef](./type_defs.md#automationstreamupdatetypedef)

## BatchCreateMemoryRecordsOutputTypeDef

```python
# BatchCreateMemoryRecordsOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import BatchCreateMemoryRecordsOutputTypeDef


def get_value() -> BatchCreateMemoryRecordsOutputTypeDef:
    return {
        "successfulRecords": ...,
    }


# BatchCreateMemoryRecordsOutputTypeDef definition

class BatchCreateMemoryRecordsOutputTypeDef(TypedDict):
    successfulRecords: list[MemoryRecordOutputTypeDef],  # (1)
    failedRecords: list[MemoryRecordOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See `list[MemoryRecordOutputTypeDef]`
2. See `list[MemoryRecordOutputTypeDef]`
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## BatchDeleteMemoryRecordsOutputTypeDef

```python
# BatchDeleteMemoryRecordsOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import BatchDeleteMemoryRecordsOutputTypeDef


def get_value() -> BatchDeleteMemoryRecordsOutputTypeDef:
    return {
        "successfulRecords": ...,
    }


# BatchDeleteMemoryRecordsOutputTypeDef definition

class BatchDeleteMemoryRecordsOutputTypeDef(TypedDict):
    successfulRecords: list[MemoryRecordOutputTypeDef],  # (1)
    failedRecords: list[MemoryRecordOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See `list[MemoryRecordOutputTypeDef]`
2. See `list[MemoryRecordOutputTypeDef]`
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## BatchUpdateMemoryRecordsOutputTypeDef

```python
# BatchUpdateMemoryRecordsOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import BatchUpdateMemoryRecordsOutputTypeDef


def get_value() -> BatchUpdateMemoryRecordsOutputTypeDef:
    return {
        "successfulRecords": ...,
    }


# BatchUpdateMemoryRecordsOutputTypeDef definition

class BatchUpdateMemoryRecordsOutputTypeDef(TypedDict):
    successfulRecords: list[MemoryRecordOutputTypeDef],  # (1)
    failedRecords: list[MemoryRecordOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See `list[MemoryRecordOutputTypeDef]`
2. See `list[MemoryRecordOutputTypeDef]`
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeleteEventOutputTypeDef

```python
# DeleteEventOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import DeleteEventOutputTypeDef


def get_value() -> DeleteEventOutputTypeDef:
    return {
        "eventId": ...,
    }


# DeleteEventOutputTypeDef definition

class DeleteEventOutputTypeDef(TypedDict):
    eventId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeleteMemoryRecordOutputTypeDef

```python
# DeleteMemoryRecordOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import DeleteMemoryRecordOutputTypeDef


def get_value() -> DeleteMemoryRecordOutputTypeDef:
    return {
        "memoryRecordId": ...,
    }


# DeleteMemoryRecordOutputTypeDef definition

class DeleteMemoryRecordOutputTypeDef(TypedDict):
    memoryRecordId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetAgentCardResponseTypeDef

```python
# GetAgentCardResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import GetAgentCardResponseTypeDef


def get_value() -> GetAgentCardResponseTypeDef:
    return {
        "runtimeSessionId": ...,
    }


# GetAgentCardResponseTypeDef definition

class GetAgentCardResponseTypeDef(TypedDict):
    runtimeSessionId: str,
    agentCard: dict[str, Any],
    statusCode: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetCodeInterpreterSessionResponseTypeDef

```python
# GetCodeInterpreterSessionResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import GetCodeInterpreterSessionResponseTypeDef


def get_value() -> GetCodeInterpreterSessionResponseTypeDef:
    return {
        "codeInterpreterIdentifier": ...,
    }


# GetCodeInterpreterSessionResponseTypeDef definition

class GetCodeInterpreterSessionResponseTypeDef(TypedDict):
    codeInterpreterIdentifier: str,
    sessionId: str,
    name: str,
    createdAt: datetime.datetime,
    sessionTimeoutSeconds: int,
    status: CodeInterpreterSessionStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: CodeInterpreterSessionStatusType](./literals.md#codeinterpretersessionstatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetResourceApiKeyResponseTypeDef

```python
# GetResourceApiKeyResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import GetResourceApiKeyResponseTypeDef


def get_value() -> GetResourceApiKeyResponseTypeDef:
    return {
        "apiKey": ...,
    }


# GetResourceApiKeyResponseTypeDef definition

class GetResourceApiKeyResponseTypeDef(TypedDict):
    apiKey: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetResourceOauth2TokenResponseTypeDef

```python
# GetResourceOauth2TokenResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import GetResourceOauth2TokenResponseTypeDef


def get_value() -> GetResourceOauth2TokenResponseTypeDef:
    return {
        "authorizationUrl": ...,
    }


# GetResourceOauth2TokenResponseTypeDef definition

class GetResourceOauth2TokenResponseTypeDef(TypedDict):
    authorizationUrl: str,
    accessToken: str,
    sessionUri: str,
    sessionStatus: SessionStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: SessionStatusType](./literals.md#sessionstatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetWorkloadAccessTokenForJWTResponseTypeDef

```python
# GetWorkloadAccessTokenForJWTResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import GetWorkloadAccessTokenForJWTResponseTypeDef


def get_value() -> GetWorkloadAccessTokenForJWTResponseTypeDef:
    return {
        "workloadAccessToken": ...,
    }


# GetWorkloadAccessTokenForJWTResponseTypeDef definition

class GetWorkloadAccessTokenForJWTResponseTypeDef(TypedDict):
    workloadAccessToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetWorkloadAccessTokenForUserIdResponseTypeDef

```python
# GetWorkloadAccessTokenForUserIdResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import GetWorkloadAccessTokenForUserIdResponseTypeDef


def get_value() -> GetWorkloadAccessTokenForUserIdResponseTypeDef:
    return {
        "workloadAccessToken": ...,
    }


# GetWorkloadAccessTokenForUserIdResponseTypeDef definition

class GetWorkloadAccessTokenForUserIdResponseTypeDef(TypedDict):
    workloadAccessToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetWorkloadAccessTokenResponseTypeDef

```python
# GetWorkloadAccessTokenResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import GetWorkloadAccessTokenResponseTypeDef


def get_value() -> GetWorkloadAccessTokenResponseTypeDef:
    return {
        "workloadAccessToken": ...,
    }


# GetWorkloadAccessTokenResponseTypeDef definition

class GetWorkloadAccessTokenResponseTypeDef(TypedDict):
    workloadAccessToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## InvokeAgentRuntimeResponseTypeDef

```python
# InvokeAgentRuntimeResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import InvokeAgentRuntimeResponseTypeDef


def get_value() -> InvokeAgentRuntimeResponseTypeDef:
    return {
        "runtimeSessionId": ...,
    }


# InvokeAgentRuntimeResponseTypeDef definition

class InvokeAgentRuntimeResponseTypeDef(TypedDict):
    runtimeSessionId: str,
    mcpSessionId: str,
    mcpProtocolVersion: str,
    traceId: str,
    traceParent: str,
    traceState: str,
    baggage: str,
    contentType: str,
    response: aiobotocore.response.StreamingBody,
    statusCode: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListActorsOutputTypeDef

```python
# ListActorsOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ListActorsOutputTypeDef


def get_value() -> ListActorsOutputTypeDef:
    return {
        "actorSummaries": ...,
    }


# ListActorsOutputTypeDef definition

class ListActorsOutputTypeDef(TypedDict):
    actorSummaries: list[ActorSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[ActorSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## StartCodeInterpreterSessionResponseTypeDef

```python
# StartCodeInterpreterSessionResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import StartCodeInterpreterSessionResponseTypeDef


def get_value() -> StartCodeInterpreterSessionResponseTypeDef:
    return {
        "codeInterpreterIdentifier": ...,
    }


# StartCodeInterpreterSessionResponseTypeDef definition

class StartCodeInterpreterSessionResponseTypeDef(TypedDict):
    codeInterpreterIdentifier: str,
    sessionId: str,
    createdAt: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## StartMemoryExtractionJobOutputTypeDef

```python
# StartMemoryExtractionJobOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import StartMemoryExtractionJobOutputTypeDef


def get_value() -> StartMemoryExtractionJobOutputTypeDef:
    return {
        "jobId": ...,
    }


# StartMemoryExtractionJobOutputTypeDef definition

class StartMemoryExtractionJobOutputTypeDef(TypedDict):
    jobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## StopBrowserSessionResponseTypeDef

```python
# StopBrowserSessionResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import StopBrowserSessionResponseTypeDef


def get_value() -> StopBrowserSessionResponseTypeDef:
    return {
        "browserIdentifier": ...,
    }


# StopBrowserSessionResponseTypeDef definition

class StopBrowserSessionResponseTypeDef(TypedDict):
    browserIdentifier: str,
    sessionId: str,
    lastUpdatedAt: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## StopCodeInterpreterSessionResponseTypeDef

```python
# StopCodeInterpreterSessionResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import StopCodeInterpreterSessionResponseTypeDef


def get_value() -> StopCodeInterpreterSessionResponseTypeDef:
    return {
        "codeInterpreterIdentifier": ...,
    }


# StopCodeInterpreterSessionResponseTypeDef definition

class StopCodeInterpreterSessionResponseTypeDef(TypedDict):
    codeInterpreterIdentifier: str,
    sessionId: str,
    lastUpdatedAt: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## StopRuntimeSessionResponseTypeDef

```python
# StopRuntimeSessionResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import StopRuntimeSessionResponseTypeDef


def get_value() -> StopRuntimeSessionResponseTypeDef:
    return {
        "runtimeSessionId": ...,
    }


# StopRuntimeSessionResponseTypeDef definition

class StopRuntimeSessionResponseTypeDef(TypedDict):
    runtimeSessionId: str,
    statusCode: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## BatchDeleteMemoryRecordsInputTypeDef

```python
# BatchDeleteMemoryRecordsInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import BatchDeleteMemoryRecordsInputTypeDef


def get_value() -> BatchDeleteMemoryRecordsInputTypeDef:
    return {
        "memoryId": ...,
    }


# BatchDeleteMemoryRecordsInputTypeDef definition

class BatchDeleteMemoryRecordsInputTypeDef(TypedDict):
    memoryId: str,
    records: Sequence[MemoryRecordDeleteInputTypeDef],  # (1)
```

1. See `Sequence[MemoryRecordDeleteInputTypeDef]`

## InputContentBlockTypeDef

```python
# InputContentBlockTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import InputContentBlockTypeDef


def get_value() -> InputContentBlockTypeDef:
    return {
        "path": ...,
    }


# InputContentBlockTypeDef definition

class InputContentBlockTypeDef(TypedDict):
    path: str,
    text: NotRequired[str],
    blob: NotRequired[BlobTypeDef],
```


## InvokeAgentRuntimeRequestTypeDef

```python
# InvokeAgentRuntimeRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import InvokeAgentRuntimeRequestTypeDef


def get_value() -> InvokeAgentRuntimeRequestTypeDef:
    return {
        "agentRuntimeArn": ...,
    }


# InvokeAgentRuntimeRequestTypeDef definition

class InvokeAgentRuntimeRequestTypeDef(TypedDict):
    agentRuntimeArn: str,
    payload: BlobTypeDef,
    contentType: NotRequired[str],
    accept: NotRequired[str],
    mcpSessionId: NotRequired[str],
    runtimeSessionId: NotRequired[str],
    mcpProtocolVersion: NotRequired[str],
    runtimeUserId: NotRequired[str],
    traceId: NotRequired[str],
    traceParent: NotRequired[str],
    traceState: NotRequired[str],
    baggage: NotRequired[str],
    qualifier: NotRequired[str],
    accountId: NotRequired[str],
```


## BrowserSessionStreamTypeDef

```python
# BrowserSessionStreamTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import BrowserSessionStreamTypeDef


def get_value() -> BrowserSessionStreamTypeDef:
    return {
        "automationStream": ...,
    }


# BrowserSessionStreamTypeDef definition

class BrowserSessionStreamTypeDef(TypedDict):
    automationStream: AutomationStreamTypeDef,  # (1)
    liveViewStream: NotRequired[LiveViewStreamTypeDef],  # (2)
```

1. See [:material-code-braces: AutomationStreamTypeDef](./type_defs.md#automationstreamtypedef)
2. See [:material-code-braces: LiveViewStreamTypeDef](./type_defs.md#liveviewstreamtypedef)

## ListBrowserSessionsResponseTypeDef

```python
# ListBrowserSessionsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ListBrowserSessionsResponseTypeDef


def get_value() -> ListBrowserSessionsResponseTypeDef:
    return {
        "items": ...,
    }


# ListBrowserSessionsResponseTypeDef definition

class ListBrowserSessionsResponseTypeDef(TypedDict):
    items: list[BrowserSessionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[BrowserSessionSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListCodeInterpreterSessionsResponseTypeDef

```python
# ListCodeInterpreterSessionsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ListCodeInterpreterSessionsResponseTypeDef


def get_value() -> ListCodeInterpreterSessionsResponseTypeDef:
    return {
        "items": ...,
    }


# ListCodeInterpreterSessionsResponseTypeDef definition

class ListCodeInterpreterSessionsResponseTypeDef(TypedDict):
    items: list[CodeInterpreterSessionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[CodeInterpreterSessionSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CompleteResourceTokenAuthRequestTypeDef

```python
# CompleteResourceTokenAuthRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import CompleteResourceTokenAuthRequestTypeDef


def get_value() -> CompleteResourceTokenAuthRequestTypeDef:
    return {
        "userIdentifier": ...,
    }


# CompleteResourceTokenAuthRequestTypeDef definition

class CompleteResourceTokenAuthRequestTypeDef(TypedDict):
    userIdentifier: UserIdentifierTypeDef,  # (1)
    sessionUri: str,
```

1. See [:material-code-braces: UserIdentifierTypeDef](./type_defs.md#useridentifiertypedef)

## ContentBlockTypeDef

```python
# ContentBlockTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ContentBlockTypeDef


def get_value() -> ContentBlockTypeDef:
    return {
        "type": ...,
    }


# ContentBlockTypeDef definition

class ContentBlockTypeDef(TypedDict):
    type: ContentBlockTypeType,  # (1)
    text: NotRequired[str],
    data: NotRequired[bytes],
    mimeType: NotRequired[str],
    uri: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    size: NotRequired[int],
    resource: NotRequired[ResourceContentTypeDef],  # (2)
```

1. See [:material-code-brackets: ContentBlockTypeType](./literals.md#contentblocktypetype)
2. See [:material-code-braces: ResourceContentTypeDef](./type_defs.md#resourcecontenttypedef)

## ConversationalTypeDef

```python
# ConversationalTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ConversationalTypeDef


def get_value() -> ConversationalTypeDef:
    return {
        "content": ...,
    }


# ConversationalTypeDef definition

class ConversationalTypeDef(TypedDict):
    content: ContentTypeDef,  # (1)
    role: RoleType,  # (2)
```

1. See [:material-code-braces: ContentTypeDef](./type_defs.md#contenttypedef)
2. See [:material-code-brackets: RoleType](./literals.md#roletype)

## ContextTypeDef

```python
# ContextTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ContextTypeDef


def get_value() -> ContextTypeDef:
    return {
        "spanContext": ...,
    }


# ContextTypeDef definition

class ContextTypeDef(TypedDict):
    spanContext: NotRequired[SpanContextTypeDef],  # (1)
```

1. See [:material-code-braces: SpanContextTypeDef](./type_defs.md#spancontexttypedef)

## RightExpressionTypeDef

```python
# RightExpressionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import RightExpressionTypeDef


def get_value() -> RightExpressionTypeDef:
    return {
        "metadataValue": ...,
    }


# RightExpressionTypeDef definition

class RightExpressionTypeDef(TypedDict):
    metadataValue: NotRequired[MetadataValueTypeDef],  # (1)
```

1. See [:material-code-braces: MetadataValueTypeDef](./type_defs.md#metadatavaluetypedef)

## EvaluateRequestTypeDef

```python
# EvaluateRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import EvaluateRequestTypeDef


def get_value() -> EvaluateRequestTypeDef:
    return {
        "evaluatorId": ...,
    }


# EvaluateRequestTypeDef definition

class EvaluateRequestTypeDef(TypedDict):
    evaluatorId: str,
    evaluationInput: EvaluationInputTypeDef,  # (1)
    evaluationTarget: NotRequired[EvaluationTargetTypeDef],  # (2)
```

1. See [:material-code-braces: EvaluationInputTypeDef](./type_defs.md#evaluationinputtypedef)
2. See [:material-code-braces: EvaluationTargetTypeDef](./type_defs.md#evaluationtargettypedef)

## ListMemoryExtractionJobsInputTypeDef

```python
# ListMemoryExtractionJobsInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ListMemoryExtractionJobsInputTypeDef


def get_value() -> ListMemoryExtractionJobsInputTypeDef:
    return {
        "memoryId": ...,
    }


# ListMemoryExtractionJobsInputTypeDef definition

class ListMemoryExtractionJobsInputTypeDef(TypedDict):
    memoryId: str,
    maxResults: NotRequired[int],
    filter: NotRequired[ExtractionJobFilterInputTypeDef],  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ExtractionJobFilterInputTypeDef](./type_defs.md#extractionjobfilterinputtypedef)

## ExtractionJobMessagesTypeDef

```python
# ExtractionJobMessagesTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ExtractionJobMessagesTypeDef


def get_value() -> ExtractionJobMessagesTypeDef:
    return {
        "messagesList": ...,
    }


# ExtractionJobMessagesTypeDef definition

class ExtractionJobMessagesTypeDef(TypedDict):
    messagesList: NotRequired[list[MessageMetadataTypeDef]],  # (1)
```

1. See `list[MessageMetadataTypeDef]`

## StartMemoryExtractionJobInputTypeDef

```python
# StartMemoryExtractionJobInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import StartMemoryExtractionJobInputTypeDef


def get_value() -> StartMemoryExtractionJobInputTypeDef:
    return {
        "memoryId": ...,
    }


# StartMemoryExtractionJobInputTypeDef definition

class StartMemoryExtractionJobInputTypeDef(TypedDict):
    memoryId: str,
    extractionJob: ExtractionJobTypeDef,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: ExtractionJobTypeDef](./type_defs.md#extractionjobtypedef)

## StartBrowserSessionRequestTypeDef

```python
# StartBrowserSessionRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import StartBrowserSessionRequestTypeDef


def get_value() -> StartBrowserSessionRequestTypeDef:
    return {
        "browserIdentifier": ...,
    }


# StartBrowserSessionRequestTypeDef definition

class StartBrowserSessionRequestTypeDef(TypedDict):
    browserIdentifier: str,
    traceId: NotRequired[str],
    traceParent: NotRequired[str],
    name: NotRequired[str],
    sessionTimeoutSeconds: NotRequired[int],
    viewPort: NotRequired[ViewPortTypeDef],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: ViewPortTypeDef](./type_defs.md#viewporttypedef)

## ListActorsInputPaginateTypeDef

```python
# ListActorsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ListActorsInputPaginateTypeDef


def get_value() -> ListActorsInputPaginateTypeDef:
    return {
        "memoryId": ...,
    }


# ListActorsInputPaginateTypeDef definition

class ListActorsInputPaginateTypeDef(TypedDict):
    memoryId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListMemoryExtractionJobsInputPaginateTypeDef

```python
# ListMemoryExtractionJobsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ListMemoryExtractionJobsInputPaginateTypeDef


def get_value() -> ListMemoryExtractionJobsInputPaginateTypeDef:
    return {
        "memoryId": ...,
    }


# ListMemoryExtractionJobsInputPaginateTypeDef definition

class ListMemoryExtractionJobsInputPaginateTypeDef(TypedDict):
    memoryId: str,
    filter: NotRequired[ExtractionJobFilterInputTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ExtractionJobFilterInputTypeDef](./type_defs.md#extractionjobfilterinputtypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListMemoryRecordsInputPaginateTypeDef

```python
# ListMemoryRecordsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ListMemoryRecordsInputPaginateTypeDef


def get_value() -> ListMemoryRecordsInputPaginateTypeDef:
    return {
        "memoryId": ...,
    }


# ListMemoryRecordsInputPaginateTypeDef definition

class ListMemoryRecordsInputPaginateTypeDef(TypedDict):
    memoryId: str,
    namespace: str,
    memoryStrategyId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListSessionsInputPaginateTypeDef

```python
# ListSessionsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ListSessionsInputPaginateTypeDef


def get_value() -> ListSessionsInputPaginateTypeDef:
    return {
        "memoryId": ...,
    }


# ListSessionsInputPaginateTypeDef definition

class ListSessionsInputPaginateTypeDef(TypedDict):
    memoryId: str,
    actorId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListSessionsOutputTypeDef

```python
# ListSessionsOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ListSessionsOutputTypeDef


def get_value() -> ListSessionsOutputTypeDef:
    return {
        "sessionSummaries": ...,
    }


# ListSessionsOutputTypeDef definition

class ListSessionsOutputTypeDef(TypedDict):
    sessionSummaries: list[SessionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[SessionSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## MemoryRecordCreateInputTypeDef

```python
# MemoryRecordCreateInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import MemoryRecordCreateInputTypeDef


def get_value() -> MemoryRecordCreateInputTypeDef:
    return {
        "requestIdentifier": ...,
    }


# MemoryRecordCreateInputTypeDef definition

class MemoryRecordCreateInputTypeDef(TypedDict):
    requestIdentifier: str,
    namespaces: Sequence[str],
    content: MemoryContentTypeDef,  # (1)
    timestamp: TimestampTypeDef,
    memoryStrategyId: NotRequired[str],
```

1. See [:material-code-braces: MemoryContentTypeDef](./type_defs.md#memorycontenttypedef)

## MemoryRecordSummaryTypeDef

```python
# MemoryRecordSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import MemoryRecordSummaryTypeDef


def get_value() -> MemoryRecordSummaryTypeDef:
    return {
        "memoryRecordId": ...,
    }


# MemoryRecordSummaryTypeDef definition

class MemoryRecordSummaryTypeDef(TypedDict):
    memoryRecordId: str,
    content: MemoryContentTypeDef,  # (1)
    memoryStrategyId: str,
    namespaces: list[str],
    createdAt: datetime.datetime,
    score: NotRequired[float],
    metadata: NotRequired[dict[str, MetadataValueTypeDef]],  # (2)
```

1. See [:material-code-braces: MemoryContentTypeDef](./type_defs.md#memorycontenttypedef)
2. See `dict[str, MetadataValueTypeDef]`

## MemoryRecordTypeDef

```python
# MemoryRecordTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import MemoryRecordTypeDef


def get_value() -> MemoryRecordTypeDef:
    return {
        "memoryRecordId": ...,
    }


# MemoryRecordTypeDef definition

class MemoryRecordTypeDef(TypedDict):
    memoryRecordId: str,
    content: MemoryContentTypeDef,  # (1)
    memoryStrategyId: str,
    namespaces: list[str],
    createdAt: datetime.datetime,
    metadata: NotRequired[dict[str, MetadataValueTypeDef]],  # (2)
```

1. See [:material-code-braces: MemoryContentTypeDef](./type_defs.md#memorycontenttypedef)
2. See `dict[str, MetadataValueTypeDef]`

## MemoryRecordUpdateInputTypeDef

```python
# MemoryRecordUpdateInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import MemoryRecordUpdateInputTypeDef


def get_value() -> MemoryRecordUpdateInputTypeDef:
    return {
        "memoryRecordId": ...,
    }


# MemoryRecordUpdateInputTypeDef definition

class MemoryRecordUpdateInputTypeDef(TypedDict):
    memoryRecordId: str,
    timestamp: TimestampTypeDef,
    content: NotRequired[MemoryContentTypeDef],  # (1)
    namespaces: NotRequired[Sequence[str]],
    memoryStrategyId: NotRequired[str],
```

1. See [:material-code-braces: MemoryContentTypeDef](./type_defs.md#memorycontenttypedef)

## ValidationExceptionTypeDef

```python
# ValidationExceptionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ValidationExceptionTypeDef


def get_value() -> ValidationExceptionTypeDef:
    return {
        "message": ...,
    }


# ValidationExceptionTypeDef definition

class ValidationExceptionTypeDef(TypedDict):
    message: str,
    reason: ValidationExceptionReasonType,  # (1)
    fieldList: NotRequired[list[ValidationExceptionFieldTypeDef]],  # (2)
```

1. See [:material-code-brackets: ValidationExceptionReasonType](./literals.md#validationexceptionreasontype)
2. See `list[ValidationExceptionFieldTypeDef]`

## UpdateBrowserStreamRequestTypeDef

```python
# UpdateBrowserStreamRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import UpdateBrowserStreamRequestTypeDef


def get_value() -> UpdateBrowserStreamRequestTypeDef:
    return {
        "browserIdentifier": ...,
    }


# UpdateBrowserStreamRequestTypeDef definition

class UpdateBrowserStreamRequestTypeDef(TypedDict):
    browserIdentifier: str,
    sessionId: str,
    streamUpdate: StreamUpdateTypeDef,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: StreamUpdateTypeDef](./type_defs.md#streamupdatetypedef)

## ToolArgumentsTypeDef

```python
# ToolArgumentsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ToolArgumentsTypeDef


def get_value() -> ToolArgumentsTypeDef:
    return {
        "code": ...,
    }


# ToolArgumentsTypeDef definition

class ToolArgumentsTypeDef(TypedDict):
    code: NotRequired[str],
    language: NotRequired[ProgrammingLanguageType],  # (1)
    clearContext: NotRequired[bool],
    command: NotRequired[str],
    path: NotRequired[str],
    paths: NotRequired[Sequence[str]],
    content: NotRequired[Sequence[InputContentBlockTypeDef]],  # (2)
    directoryPath: NotRequired[str],
    taskId: NotRequired[str],
```

1. See [:material-code-brackets: ProgrammingLanguageType](./literals.md#programminglanguagetype)
2. See `Sequence[InputContentBlockTypeDef]`

## GetBrowserSessionResponseTypeDef

```python
# GetBrowserSessionResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import GetBrowserSessionResponseTypeDef


def get_value() -> GetBrowserSessionResponseTypeDef:
    return {
        "browserIdentifier": ...,
    }


# GetBrowserSessionResponseTypeDef definition

class GetBrowserSessionResponseTypeDef(TypedDict):
    browserIdentifier: str,
    sessionId: str,
    name: str,
    createdAt: datetime.datetime,
    viewPort: ViewPortTypeDef,  # (1)
    sessionTimeoutSeconds: int,
    status: BrowserSessionStatusType,  # (2)
    streams: BrowserSessionStreamTypeDef,  # (3)
    sessionReplayArtifact: str,
    lastUpdatedAt: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ViewPortTypeDef](./type_defs.md#viewporttypedef)
2. See [:material-code-brackets: BrowserSessionStatusType](./literals.md#browsersessionstatustype)
3. See [:material-code-braces: BrowserSessionStreamTypeDef](./type_defs.md#browsersessionstreamtypedef)
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## StartBrowserSessionResponseTypeDef

```python
# StartBrowserSessionResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import StartBrowserSessionResponseTypeDef


def get_value() -> StartBrowserSessionResponseTypeDef:
    return {
        "browserIdentifier": ...,
    }


# StartBrowserSessionResponseTypeDef definition

class StartBrowserSessionResponseTypeDef(TypedDict):
    browserIdentifier: str,
    sessionId: str,
    createdAt: datetime.datetime,
    streams: BrowserSessionStreamTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BrowserSessionStreamTypeDef](./type_defs.md#browsersessionstreamtypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateBrowserStreamResponseTypeDef

```python
# UpdateBrowserStreamResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import UpdateBrowserStreamResponseTypeDef


def get_value() -> UpdateBrowserStreamResponseTypeDef:
    return {
        "browserIdentifier": ...,
    }


# UpdateBrowserStreamResponseTypeDef definition

class UpdateBrowserStreamResponseTypeDef(TypedDict):
    browserIdentifier: str,
    sessionId: str,
    streams: BrowserSessionStreamTypeDef,  # (1)
    updatedAt: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BrowserSessionStreamTypeDef](./type_defs.md#browsersessionstreamtypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CodeInterpreterResultTypeDef

```python
# CodeInterpreterResultTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import CodeInterpreterResultTypeDef


def get_value() -> CodeInterpreterResultTypeDef:
    return {
        "content": ...,
    }


# CodeInterpreterResultTypeDef definition

class CodeInterpreterResultTypeDef(TypedDict):
    content: list[ContentBlockTypeDef],  # (1)
    structuredContent: NotRequired[ToolResultStructuredContentTypeDef],  # (2)
    isError: NotRequired[bool],
```

1. See `list[ContentBlockTypeDef]`
2. See [:material-code-braces: ToolResultStructuredContentTypeDef](./type_defs.md#toolresultstructuredcontenttypedef)

## PayloadTypeOutputTypeDef

```python
# PayloadTypeOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import PayloadTypeOutputTypeDef


def get_value() -> PayloadTypeOutputTypeDef:
    return {
        "conversational": ...,
    }


# PayloadTypeOutputTypeDef definition

class PayloadTypeOutputTypeDef(TypedDict):
    conversational: NotRequired[ConversationalTypeDef],  # (1)
    blob: NotRequired[dict[str, Any]],
```

1. See [:material-code-braces: ConversationalTypeDef](./type_defs.md#conversationaltypedef)

## PayloadTypeTypeDef

```python
# PayloadTypeTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import PayloadTypeTypeDef


def get_value() -> PayloadTypeTypeDef:
    return {
        "conversational": ...,
    }


# PayloadTypeTypeDef definition

class PayloadTypeTypeDef(TypedDict):
    conversational: NotRequired[ConversationalTypeDef],  # (1)
    blob: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: ConversationalTypeDef](./type_defs.md#conversationaltypedef)

## EvaluationResultContentTypeDef

```python
# EvaluationResultContentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import EvaluationResultContentTypeDef


def get_value() -> EvaluationResultContentTypeDef:
    return {
        "evaluatorArn": ...,
    }


# EvaluationResultContentTypeDef definition

class EvaluationResultContentTypeDef(TypedDict):
    evaluatorArn: str,
    evaluatorId: str,
    evaluatorName: str,
    context: ContextTypeDef,  # (1)
    explanation: NotRequired[str],
    value: NotRequired[float],
    label: NotRequired[str],
    tokenUsage: NotRequired[TokenUsageTypeDef],  # (2)
    errorMessage: NotRequired[str],
    errorCode: NotRequired[str],
```

1. See [:material-code-braces: ContextTypeDef](./type_defs.md#contexttypedef)
2. See [:material-code-braces: TokenUsageTypeDef](./type_defs.md#tokenusagetypedef)

## EventMetadataFilterExpressionTypeDef

```python
# EventMetadataFilterExpressionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import EventMetadataFilterExpressionTypeDef


def get_value() -> EventMetadataFilterExpressionTypeDef:
    return {
        "left": ...,
    }


# EventMetadataFilterExpressionTypeDef definition

class EventMetadataFilterExpressionTypeDef(TypedDict):
    left: LeftExpressionTypeDef,  # (1)
    operator: OperatorTypeType,  # (2)
    right: NotRequired[RightExpressionTypeDef],  # (3)
```

1. See [:material-code-braces: LeftExpressionTypeDef](./type_defs.md#leftexpressiontypedef)
2. See [:material-code-brackets: OperatorTypeType](./literals.md#operatortypetype)
3. See [:material-code-braces: RightExpressionTypeDef](./type_defs.md#rightexpressiontypedef)

## MemoryMetadataFilterExpressionTypeDef

```python
# MemoryMetadataFilterExpressionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import MemoryMetadataFilterExpressionTypeDef


def get_value() -> MemoryMetadataFilterExpressionTypeDef:
    return {
        "left": ...,
    }


# MemoryMetadataFilterExpressionTypeDef definition

class MemoryMetadataFilterExpressionTypeDef(TypedDict):
    left: LeftExpressionTypeDef,  # (1)
    operator: OperatorTypeType,  # (2)
    right: NotRequired[RightExpressionTypeDef],  # (3)
```

1. See [:material-code-braces: LeftExpressionTypeDef](./type_defs.md#leftexpressiontypedef)
2. See [:material-code-brackets: OperatorTypeType](./literals.md#operatortypetype)
3. See [:material-code-braces: RightExpressionTypeDef](./type_defs.md#rightexpressiontypedef)

## ExtractionJobMetadataTypeDef

```python
# ExtractionJobMetadataTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ExtractionJobMetadataTypeDef


def get_value() -> ExtractionJobMetadataTypeDef:
    return {
        "jobID": ...,
    }


# ExtractionJobMetadataTypeDef definition

class ExtractionJobMetadataTypeDef(TypedDict):
    jobID: str,
    messages: ExtractionJobMessagesTypeDef,  # (1)
    status: NotRequired[ExtractionJobStatusType],  # (2)
    failureReason: NotRequired[str],
    strategyId: NotRequired[str],
    sessionId: NotRequired[str],
    actorId: NotRequired[str],
```

1. See [:material-code-braces: ExtractionJobMessagesTypeDef](./type_defs.md#extractionjobmessagestypedef)
2. See [:material-code-brackets: ExtractionJobStatusType](./literals.md#extractionjobstatustype)

## BatchCreateMemoryRecordsInputTypeDef

```python
# BatchCreateMemoryRecordsInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import BatchCreateMemoryRecordsInputTypeDef


def get_value() -> BatchCreateMemoryRecordsInputTypeDef:
    return {
        "memoryId": ...,
    }


# BatchCreateMemoryRecordsInputTypeDef definition

class BatchCreateMemoryRecordsInputTypeDef(TypedDict):
    memoryId: str,
    records: Sequence[MemoryRecordCreateInputTypeDef],  # (1)
    clientToken: NotRequired[str],
```

1. See `Sequence[MemoryRecordCreateInputTypeDef]`

## ListMemoryRecordsOutputTypeDef

```python
# ListMemoryRecordsOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ListMemoryRecordsOutputTypeDef


def get_value() -> ListMemoryRecordsOutputTypeDef:
    return {
        "memoryRecordSummaries": ...,
    }


# ListMemoryRecordsOutputTypeDef definition

class ListMemoryRecordsOutputTypeDef(TypedDict):
    memoryRecordSummaries: list[MemoryRecordSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[MemoryRecordSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## RetrieveMemoryRecordsOutputTypeDef

```python
# RetrieveMemoryRecordsOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import RetrieveMemoryRecordsOutputTypeDef


def get_value() -> RetrieveMemoryRecordsOutputTypeDef:
    return {
        "memoryRecordSummaries": ...,
    }


# RetrieveMemoryRecordsOutputTypeDef definition

class RetrieveMemoryRecordsOutputTypeDef(TypedDict):
    memoryRecordSummaries: list[MemoryRecordSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[MemoryRecordSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetMemoryRecordOutputTypeDef

```python
# GetMemoryRecordOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import GetMemoryRecordOutputTypeDef


def get_value() -> GetMemoryRecordOutputTypeDef:
    return {
        "memoryRecord": ...,
    }


# GetMemoryRecordOutputTypeDef definition

class GetMemoryRecordOutputTypeDef(TypedDict):
    memoryRecord: MemoryRecordTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MemoryRecordTypeDef](./type_defs.md#memoryrecordtypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## BatchUpdateMemoryRecordsInputTypeDef

```python
# BatchUpdateMemoryRecordsInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import BatchUpdateMemoryRecordsInputTypeDef


def get_value() -> BatchUpdateMemoryRecordsInputTypeDef:
    return {
        "memoryId": ...,
    }


# BatchUpdateMemoryRecordsInputTypeDef definition

class BatchUpdateMemoryRecordsInputTypeDef(TypedDict):
    memoryId: str,
    records: Sequence[MemoryRecordUpdateInputTypeDef],  # (1)
```

1. See `Sequence[MemoryRecordUpdateInputTypeDef]`

## InvokeCodeInterpreterRequestTypeDef

```python
# InvokeCodeInterpreterRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import InvokeCodeInterpreterRequestTypeDef


def get_value() -> InvokeCodeInterpreterRequestTypeDef:
    return {
        "codeInterpreterIdentifier": ...,
    }


# InvokeCodeInterpreterRequestTypeDef definition

class InvokeCodeInterpreterRequestTypeDef(TypedDict):
    codeInterpreterIdentifier: str,
    name: ToolNameType,  # (1)
    sessionId: NotRequired[str],
    traceId: NotRequired[str],
    traceParent: NotRequired[str],
    arguments: NotRequired[ToolArgumentsTypeDef],  # (2)
```

1. See [:material-code-brackets: ToolNameType](./literals.md#toolnametype)
2. See [:material-code-braces: ToolArgumentsTypeDef](./type_defs.md#toolargumentstypedef)

## CodeInterpreterStreamOutputTypeDef

```python
# CodeInterpreterStreamOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import CodeInterpreterStreamOutputTypeDef


def get_value() -> CodeInterpreterStreamOutputTypeDef:
    return {
        "result": ...,
    }


# CodeInterpreterStreamOutputTypeDef definition

class CodeInterpreterStreamOutputTypeDef(TypedDict):
    result: NotRequired[CodeInterpreterResultTypeDef],  # (1)
    accessDeniedException: NotRequired[AccessDeniedExceptionTypeDef],  # (2)
    conflictException: NotRequired[ConflictExceptionTypeDef],  # (3)
    internalServerException: NotRequired[InternalServerExceptionTypeDef],  # (4)
    resourceNotFoundException: NotRequired[ResourceNotFoundExceptionTypeDef],  # (5)
    serviceQuotaExceededException: NotRequired[ServiceQuotaExceededExceptionTypeDef],  # (6)
    throttlingException: NotRequired[ThrottlingExceptionTypeDef],  # (7)
    validationException: NotRequired[ValidationExceptionTypeDef],  # (8)
```

1. See [:material-code-braces: CodeInterpreterResultTypeDef](./type_defs.md#codeinterpreterresulttypedef)
2. See [:material-code-braces: AccessDeniedExceptionTypeDef](./type_defs.md#accessdeniedexceptiontypedef)
3. See [:material-code-braces: ConflictExceptionTypeDef](./type_defs.md#conflictexceptiontypedef)
4. See [:material-code-braces: InternalServerExceptionTypeDef](./type_defs.md#internalserverexceptiontypedef)
5. See [:material-code-braces: ResourceNotFoundExceptionTypeDef](./type_defs.md#resourcenotfoundexceptiontypedef)
6. See [:material-code-braces: ServiceQuotaExceededExceptionTypeDef](./type_defs.md#servicequotaexceededexceptiontypedef)
7. See [:material-code-braces: ThrottlingExceptionTypeDef](./type_defs.md#throttlingexceptiontypedef)
8. See [:material-code-braces: ValidationExceptionTypeDef](./type_defs.md#validationexceptiontypedef)

## EventTypeDef

```python
# EventTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import EventTypeDef


def get_value() -> EventTypeDef:
    return {
        "memoryId": ...,
    }


# EventTypeDef definition

class EventTypeDef(TypedDict):
    memoryId: str,
    actorId: str,
    sessionId: str,
    eventId: str,
    eventTimestamp: datetime.datetime,
    payload: list[PayloadTypeOutputTypeDef],  # (1)
    branch: NotRequired[BranchTypeDef],  # (2)
    metadata: NotRequired[dict[str, MetadataValueTypeDef]],  # (3)
```

1. See `list[PayloadTypeOutputTypeDef]`
2. See [:material-code-braces: BranchTypeDef](./type_defs.md#branchtypedef)
3. See `dict[str, MetadataValueTypeDef]`

## EvaluateResponseTypeDef

```python
# EvaluateResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import EvaluateResponseTypeDef


def get_value() -> EvaluateResponseTypeDef:
    return {
        "evaluationResults": ...,
    }


# EvaluateResponseTypeDef definition

class EvaluateResponseTypeDef(TypedDict):
    evaluationResults: list[EvaluationResultContentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `list[EvaluationResultContentTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## FilterInputTypeDef

```python
# FilterInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import FilterInputTypeDef


def get_value() -> FilterInputTypeDef:
    return {
        "branch": ...,
    }


# FilterInputTypeDef definition

class FilterInputTypeDef(TypedDict):
    branch: NotRequired[BranchFilterTypeDef],  # (1)
    eventMetadata: NotRequired[Sequence[EventMetadataFilterExpressionTypeDef]],  # (2)
```

1. See [:material-code-braces: BranchFilterTypeDef](./type_defs.md#branchfiltertypedef)
2. See `Sequence[EventMetadataFilterExpressionTypeDef]`

## SearchCriteriaTypeDef

```python
# SearchCriteriaTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import SearchCriteriaTypeDef


def get_value() -> SearchCriteriaTypeDef:
    return {
        "searchQuery": ...,
    }


# SearchCriteriaTypeDef definition

class SearchCriteriaTypeDef(TypedDict):
    searchQuery: str,
    memoryStrategyId: NotRequired[str],
    topK: NotRequired[int],
    metadataFilters: NotRequired[Sequence[MemoryMetadataFilterExpressionTypeDef]],  # (1)
```

1. See `Sequence[MemoryMetadataFilterExpressionTypeDef]`

## ListMemoryExtractionJobsOutputTypeDef

```python
# ListMemoryExtractionJobsOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ListMemoryExtractionJobsOutputTypeDef


def get_value() -> ListMemoryExtractionJobsOutputTypeDef:
    return {
        "jobs": ...,
    }


# ListMemoryExtractionJobsOutputTypeDef definition

class ListMemoryExtractionJobsOutputTypeDef(TypedDict):
    jobs: list[ExtractionJobMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[ExtractionJobMetadataTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## InvokeCodeInterpreterResponseTypeDef

```python
# InvokeCodeInterpreterResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import InvokeCodeInterpreterResponseTypeDef


def get_value() -> InvokeCodeInterpreterResponseTypeDef:
    return {
        "sessionId": ...,
    }


# InvokeCodeInterpreterResponseTypeDef definition

class InvokeCodeInterpreterResponseTypeDef(TypedDict):
    sessionId: str,
    stream: aiobotocore.eventstream.AioEventStream[CodeInterpreterStreamOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `AioEventStream[CodeInterpreterStreamOutputTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateEventOutputTypeDef

```python
# CreateEventOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import CreateEventOutputTypeDef


def get_value() -> CreateEventOutputTypeDef:
    return {
        "event": ...,
    }


# CreateEventOutputTypeDef definition

class CreateEventOutputTypeDef(TypedDict):
    event: EventTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetEventOutputTypeDef

```python
# GetEventOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import GetEventOutputTypeDef


def get_value() -> GetEventOutputTypeDef:
    return {
        "event": ...,
    }


# GetEventOutputTypeDef definition

class GetEventOutputTypeDef(TypedDict):
    event: EventTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListEventsOutputTypeDef

```python
# ListEventsOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ListEventsOutputTypeDef


def get_value() -> ListEventsOutputTypeDef:
    return {
        "events": ...,
    }


# ListEventsOutputTypeDef definition

class ListEventsOutputTypeDef(TypedDict):
    events: list[EventTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[EventTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateEventInputTypeDef

```python
# CreateEventInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import CreateEventInputTypeDef


def get_value() -> CreateEventInputTypeDef:
    return {
        "memoryId": ...,
    }


# CreateEventInputTypeDef definition

class CreateEventInputTypeDef(TypedDict):
    memoryId: str,
    actorId: str,
    eventTimestamp: TimestampTypeDef,
    payload: Sequence[PayloadTypeUnionTypeDef],  # (1)
    sessionId: NotRequired[str],
    branch: NotRequired[BranchTypeDef],  # (2)
    clientToken: NotRequired[str],
    metadata: NotRequired[Mapping[str, MetadataValueTypeDef]],  # (3)
```

1. See `Sequence[PayloadTypeUnionTypeDef]`
2. See [:material-code-braces: BranchTypeDef](./type_defs.md#branchtypedef)
3. See `Mapping[str, MetadataValueTypeDef]`

## ListEventsInputPaginateTypeDef

```python
# ListEventsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ListEventsInputPaginateTypeDef


def get_value() -> ListEventsInputPaginateTypeDef:
    return {
        "memoryId": ...,
    }


# ListEventsInputPaginateTypeDef definition

class ListEventsInputPaginateTypeDef(TypedDict):
    memoryId: str,
    sessionId: str,
    actorId: str,
    includePayloads: NotRequired[bool],
    filter: NotRequired[FilterInputTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterInputTypeDef](./type_defs.md#filterinputtypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListEventsInputTypeDef

```python
# ListEventsInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import ListEventsInputTypeDef


def get_value() -> ListEventsInputTypeDef:
    return {
        "memoryId": ...,
    }


# ListEventsInputTypeDef definition

class ListEventsInputTypeDef(TypedDict):
    memoryId: str,
    sessionId: str,
    actorId: str,
    includePayloads: NotRequired[bool],
    filter: NotRequired[FilterInputTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterInputTypeDef](./type_defs.md#filterinputtypedef)

## RetrieveMemoryRecordsInputPaginateTypeDef

```python
# RetrieveMemoryRecordsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import RetrieveMemoryRecordsInputPaginateTypeDef


def get_value() -> RetrieveMemoryRecordsInputPaginateTypeDef:
    return {
        "memoryId": ...,
    }


# RetrieveMemoryRecordsInputPaginateTypeDef definition

class RetrieveMemoryRecordsInputPaginateTypeDef(TypedDict):
    memoryId: str,
    namespace: str,
    searchCriteria: SearchCriteriaTypeDef,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SearchCriteriaTypeDef](./type_defs.md#searchcriteriatypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## RetrieveMemoryRecordsInputTypeDef

```python
# RetrieveMemoryRecordsInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agentcore.type_defs import RetrieveMemoryRecordsInputTypeDef


def get_value() -> RetrieveMemoryRecordsInputTypeDef:
    return {
        "memoryId": ...,
    }


# RetrieveMemoryRecordsInputTypeDef definition

class RetrieveMemoryRecordsInputTypeDef(TypedDict):
    memoryId: str,
    namespace: str,
    searchCriteria: SearchCriteriaTypeDef,  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: SearchCriteriaTypeDef](./type_defs.md#searchcriteriatypedef)

