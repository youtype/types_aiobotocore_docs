# Type definitions

> [Index](../README.md) > [ivsrealtime](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ivsrealtime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
    type annotations stubs module [types-aiobotocore-ivs-realtime](https://pypi.org/project/types-aiobotocore-ivs-realtime/).



## CreateParticipantTokenRequestRequestTypeDef

```python
# CreateParticipantTokenRequestRequestTypeDef definition

class CreateParticipantTokenRequestRequestTypeDef(TypedDict):
    stageArn: str,
    attributes: NotRequired[Mapping[str, str]],
    capabilities: NotRequired[Sequence[ParticipantTokenCapabilityType]],  # (1)
    duration: NotRequired[int],
    userId: NotRequired[str],
```

1. See [:material-code-brackets: ParticipantTokenCapabilityType](./literals.md#participanttokencapabilitytype) 
## ParticipantTokenTypeDef

```python
# ParticipantTokenTypeDef definition

class ParticipantTokenTypeDef(TypedDict):
    attributes: NotRequired[Dict[str, str]],
    capabilities: NotRequired[List[ParticipantTokenCapabilityType]],  # (1)
    duration: NotRequired[int],
    expirationTime: NotRequired[datetime],
    participantId: NotRequired[str],
    token: NotRequired[str],
    userId: NotRequired[str],
```

1. See [:material-code-brackets: ParticipantTokenCapabilityType](./literals.md#participanttokencapabilitytype) 
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

## ParticipantTokenConfigurationTypeDef

```python
# ParticipantTokenConfigurationTypeDef definition

class ParticipantTokenConfigurationTypeDef(TypedDict):
    attributes: NotRequired[Mapping[str, str]],
    capabilities: NotRequired[Sequence[ParticipantTokenCapabilityType]],  # (1)
    duration: NotRequired[int],
    userId: NotRequired[str],
```

1. See [:material-code-brackets: ParticipantTokenCapabilityType](./literals.md#participanttokencapabilitytype) 
## StageTypeDef

```python
# StageTypeDef definition

class StageTypeDef(TypedDict):
    arn: str,
    activeSessionId: NotRequired[str],
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## DeleteStageRequestRequestTypeDef

```python
# DeleteStageRequestRequestTypeDef definition

class DeleteStageRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DisconnectParticipantRequestRequestTypeDef

```python
# DisconnectParticipantRequestRequestTypeDef definition

class DisconnectParticipantRequestRequestTypeDef(TypedDict):
    participantId: str,
    stageArn: str,
    reason: NotRequired[str],
```

## EventTypeDef

```python
# EventTypeDef definition

class EventTypeDef(TypedDict):
    errorCode: NotRequired[EventErrorCodeType],  # (1)
    eventTime: NotRequired[datetime],
    name: NotRequired[EventNameType],  # (2)
    participantId: NotRequired[str],
    remoteParticipantId: NotRequired[str],
```

1. See [:material-code-brackets: EventErrorCodeType](./literals.md#eventerrorcodetype) 
2. See [:material-code-brackets: EventNameType](./literals.md#eventnametype) 
## GetParticipantRequestRequestTypeDef

```python
# GetParticipantRequestRequestTypeDef definition

class GetParticipantRequestRequestTypeDef(TypedDict):
    participantId: str,
    sessionId: str,
    stageArn: str,
```

## ParticipantTypeDef

```python
# ParticipantTypeDef definition

class ParticipantTypeDef(TypedDict):
    attributes: NotRequired[Dict[str, str]],
    firstJoinTime: NotRequired[datetime],
    participantId: NotRequired[str],
    published: NotRequired[bool],
    state: NotRequired[ParticipantStateType],  # (1)
    userId: NotRequired[str],
```

1. See [:material-code-brackets: ParticipantStateType](./literals.md#participantstatetype) 
## GetStageRequestRequestTypeDef

```python
# GetStageRequestRequestTypeDef definition

class GetStageRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetStageSessionRequestRequestTypeDef

```python
# GetStageSessionRequestRequestTypeDef definition

class GetStageSessionRequestRequestTypeDef(TypedDict):
    sessionId: str,
    stageArn: str,
```

## StageSessionTypeDef

```python
# StageSessionTypeDef definition

class StageSessionTypeDef(TypedDict):
    endTime: NotRequired[datetime],
    sessionId: NotRequired[str],
    startTime: NotRequired[datetime],
```

## ListParticipantEventsRequestRequestTypeDef

```python
# ListParticipantEventsRequestRequestTypeDef definition

class ListParticipantEventsRequestRequestTypeDef(TypedDict):
    participantId: str,
    sessionId: str,
    stageArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListParticipantsRequestRequestTypeDef

```python
# ListParticipantsRequestRequestTypeDef definition

class ListParticipantsRequestRequestTypeDef(TypedDict):
    sessionId: str,
    stageArn: str,
    filterByPublished: NotRequired[bool],
    filterByState: NotRequired[ParticipantStateType],  # (1)
    filterByUserId: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: ParticipantStateType](./literals.md#participantstatetype) 
## ParticipantSummaryTypeDef

```python
# ParticipantSummaryTypeDef definition

class ParticipantSummaryTypeDef(TypedDict):
    firstJoinTime: NotRequired[datetime],
    participantId: NotRequired[str],
    published: NotRequired[bool],
    state: NotRequired[ParticipantStateType],  # (1)
    userId: NotRequired[str],
```

1. See [:material-code-brackets: ParticipantStateType](./literals.md#participantstatetype) 
## ListStageSessionsRequestRequestTypeDef

```python
# ListStageSessionsRequestRequestTypeDef definition

class ListStageSessionsRequestRequestTypeDef(TypedDict):
    stageArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## StageSessionSummaryTypeDef

```python
# StageSessionSummaryTypeDef definition

class StageSessionSummaryTypeDef(TypedDict):
    endTime: NotRequired[datetime],
    sessionId: NotRequired[str],
    startTime: NotRequired[datetime],
```

## ListStagesRequestRequestTypeDef

```python
# ListStagesRequestRequestTypeDef definition

class ListStagesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## StageSummaryTypeDef

```python
# StageSummaryTypeDef definition

class StageSummaryTypeDef(TypedDict):
    arn: str,
    activeSessionId: NotRequired[str],
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
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

## UpdateStageRequestRequestTypeDef

```python
# UpdateStageRequestRequestTypeDef definition

class UpdateStageRequestRequestTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
```

## CreateParticipantTokenResponseTypeDef

```python
# CreateParticipantTokenResponseTypeDef definition

class CreateParticipantTokenResponseTypeDef(TypedDict):
    participantToken: ParticipantTokenTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParticipantTokenTypeDef](./type_defs.md#participanttokentypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStageRequestRequestTypeDef

```python
# CreateStageRequestRequestTypeDef definition

class CreateStageRequestRequestTypeDef(TypedDict):
    name: NotRequired[str],
    participantTokenConfigurations: NotRequired[Sequence[ParticipantTokenConfigurationTypeDef]],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ParticipantTokenConfigurationTypeDef](./type_defs.md#participanttokenconfigurationtypedef) 
## CreateStageResponseTypeDef

```python
# CreateStageResponseTypeDef definition

class CreateStageResponseTypeDef(TypedDict):
    participantTokens: List[ParticipantTokenTypeDef],  # (1)
    stage: StageTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ParticipantTokenTypeDef](./type_defs.md#participanttokentypedef) 
2. See [:material-code-braces: StageTypeDef](./type_defs.md#stagetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStageResponseTypeDef

```python
# GetStageResponseTypeDef definition

class GetStageResponseTypeDef(TypedDict):
    stage: StageTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StageTypeDef](./type_defs.md#stagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateStageResponseTypeDef

```python
# UpdateStageResponseTypeDef definition

class UpdateStageResponseTypeDef(TypedDict):
    stage: StageTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StageTypeDef](./type_defs.md#stagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListParticipantEventsResponseTypeDef

```python
# ListParticipantEventsResponseTypeDef definition

class ListParticipantEventsResponseTypeDef(TypedDict):
    events: List[EventTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetParticipantResponseTypeDef

```python
# GetParticipantResponseTypeDef definition

class GetParticipantResponseTypeDef(TypedDict):
    participant: ParticipantTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParticipantTypeDef](./type_defs.md#participanttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStageSessionResponseTypeDef

```python
# GetStageSessionResponseTypeDef definition

class GetStageSessionResponseTypeDef(TypedDict):
    stageSession: StageSessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StageSessionTypeDef](./type_defs.md#stagesessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListParticipantsResponseTypeDef

```python
# ListParticipantsResponseTypeDef definition

class ListParticipantsResponseTypeDef(TypedDict):
    nextToken: str,
    participants: List[ParticipantSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParticipantSummaryTypeDef](./type_defs.md#participantsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStageSessionsResponseTypeDef

```python
# ListStageSessionsResponseTypeDef definition

class ListStageSessionsResponseTypeDef(TypedDict):
    nextToken: str,
    stageSessions: List[StageSessionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StageSessionSummaryTypeDef](./type_defs.md#stagesessionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStagesResponseTypeDef

```python
# ListStagesResponseTypeDef definition

class ListStagesResponseTypeDef(TypedDict):
    nextToken: str,
    stages: List[StageSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StageSummaryTypeDef](./type_defs.md#stagesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
