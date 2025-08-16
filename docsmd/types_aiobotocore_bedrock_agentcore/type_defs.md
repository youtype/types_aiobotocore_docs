# Type definitions

> [Index](../README.md) > [BedrockAgentCoreDataPlaneFrontingLayer](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [BedrockAgentCoreDataPlaneFrontingLayer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore.html#bedrockagentcoredataplanefrontinglayer)
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
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
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
    resourceOauth2ReturnUrl: NotRequired[str],
    forceAuthentication: NotRequired[bool],
    customParameters: NotRequired[Mapping[str, str]],
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
```


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
```

1. See [:material-code-braces: BranchFilterTypeDef](./type_defs.md#branchfiltertypedef)

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
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

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
    actorSummaries: List[ActorSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `List[ActorSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

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
    items: List[BrowserSessionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `List[BrowserSessionSummaryTypeDef]`
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
    items: List[CodeInterpreterSessionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `List[CodeInterpreterSessionSummaryTypeDef]`
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
    sessionSummaries: List[SessionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `List[SessionSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

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
    namespaces: List[str],
    createdAt: datetime.datetime,
    score: NotRequired[float],
```

1. See [:material-code-braces: MemoryContentTypeDef](./type_defs.md#memorycontenttypedef)

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
    namespaces: List[str],
    createdAt: datetime.datetime,
```

1. See [:material-code-braces: MemoryContentTypeDef](./type_defs.md#memorycontenttypedef)

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
    fieldList: NotRequired[List[ValidationExceptionFieldTypeDef]],  # (2)
```

1. See [:material-code-brackets: ValidationExceptionReasonType](./literals.md#validationexceptionreasontype)
2. See `List[ValidationExceptionFieldTypeDef]`

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
    content: List[ContentBlockTypeDef],  # (1)
    structuredContent: NotRequired[ToolResultStructuredContentTypeDef],  # (2)
    isError: NotRequired[bool],
```

1. See `List[ContentBlockTypeDef]`
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
    blob: NotRequired[Dict[str, Any]],
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
    memoryRecordSummaries: List[MemoryRecordSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `List[MemoryRecordSummaryTypeDef]`
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
    memoryRecordSummaries: List[MemoryRecordSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `List[MemoryRecordSummaryTypeDef]`
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
    payload: List[PayloadTypeOutputTypeDef],  # (1)
    branch: NotRequired[BranchTypeDef],  # (2)
```

1. See `List[PayloadTypeOutputTypeDef]`
2. See [:material-code-braces: BranchTypeDef](./type_defs.md#branchtypedef)

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
    events: List[EventTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `List[EventTypeDef]`
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
```

1. See `Sequence[PayloadTypeUnionTypeDef]`
2. See [:material-code-braces: BranchTypeDef](./type_defs.md#branchtypedef)

