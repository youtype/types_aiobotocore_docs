# Type definitions

> [Index](../README.md) > [Ivsrealtime](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Ivsrealtime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime)
    type annotations stubs module [types-aiobotocore-ivs-realtime](https://pypi.org/project/types-aiobotocore-ivs-realtime/).

## S3DestinationConfigurationUnionTypeDef

```python
# S3DestinationConfigurationUnionTypeDef definition

S3DestinationConfigurationUnionTypeDef = Union[
    S3DestinationConfigurationTypeDef,  # (1)
    S3DestinationConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) 
2. See [:material-code-braces: S3DestinationConfigurationOutputTypeDef](./type_defs.md#s3destinationconfigurationoutputtypedef) 

## DestinationConfigurationUnionTypeDef

```python
# DestinationConfigurationUnionTypeDef definition

DestinationConfigurationUnionTypeDef = Union[
    DestinationConfigurationTypeDef,  # (1)
    DestinationConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
2. See [:material-code-braces: DestinationConfigurationOutputTypeDef](./type_defs.md#destinationconfigurationoutputtypedef) 



## AutoParticipantRecordingConfigurationOutputTypeDef

```python
# AutoParticipantRecordingConfigurationOutputTypeDef definition

class AutoParticipantRecordingConfigurationOutputTypeDef(TypedDict):
    storageConfigurationArn: str,
    mediaTypes: NotRequired[List[ParticipantRecordingMediaTypeType]],  # (1)
```

1. See [:material-code-brackets: ParticipantRecordingMediaTypeType](./literals.md#participantrecordingmediatypetype) 
## AutoParticipantRecordingConfigurationTypeDef

```python
# AutoParticipantRecordingConfigurationTypeDef definition

class AutoParticipantRecordingConfigurationTypeDef(TypedDict):
    storageConfigurationArn: str,
    mediaTypes: NotRequired[Sequence[ParticipantRecordingMediaTypeType]],  # (1)
```

1. See [:material-code-brackets: ParticipantRecordingMediaTypeType](./literals.md#participantrecordingmediatypetype) 
## ChannelDestinationConfigurationTypeDef

```python
# ChannelDestinationConfigurationTypeDef definition

class ChannelDestinationConfigurationTypeDef(TypedDict):
    channelArn: str,
    encoderConfigurationArn: NotRequired[str],
```

## DestinationSummaryTypeDef

```python
# DestinationSummaryTypeDef definition

class DestinationSummaryTypeDef(TypedDict):
    id: str,
    state: DestinationStateType,  # (1)
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
```

1. See [:material-code-brackets: DestinationStateType](./literals.md#destinationstatetype) 
## VideoTypeDef

```python
# VideoTypeDef definition

class VideoTypeDef(TypedDict):
    width: NotRequired[int],
    height: NotRequired[int],
    framerate: NotRequired[float],
    bitrate: NotRequired[int],
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

## CreateIngestConfigurationRequestRequestTypeDef

```python
# CreateIngestConfigurationRequestRequestTypeDef definition

class CreateIngestConfigurationRequestRequestTypeDef(TypedDict):
    ingestProtocol: IngestProtocolType,  # (1)
    name: NotRequired[str],
    stageArn: NotRequired[str],
    userId: NotRequired[str],
    attributes: NotRequired[Mapping[str, str]],
    insecureIngest: NotRequired[bool],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: IngestProtocolType](./literals.md#ingestprotocoltype) 
## IngestConfigurationTypeDef

```python
# IngestConfigurationTypeDef definition

class IngestConfigurationTypeDef(TypedDict):
    arn: str,
    ingestProtocol: IngestProtocolType,  # (1)
    streamKey: str,
    stageArn: str,
    participantId: str,
    state: IngestConfigurationStateType,  # (2)
    name: NotRequired[str],
    userId: NotRequired[str],
    attributes: NotRequired[Dict[str, str]],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: IngestProtocolType](./literals.md#ingestprotocoltype) 
2. See [:material-code-brackets: IngestConfigurationStateType](./literals.md#ingestconfigurationstatetype) 
## CreateParticipantTokenRequestRequestTypeDef

```python
# CreateParticipantTokenRequestRequestTypeDef definition

class CreateParticipantTokenRequestRequestTypeDef(TypedDict):
    stageArn: str,
    duration: NotRequired[int],
    userId: NotRequired[str],
    attributes: NotRequired[Mapping[str, str]],
    capabilities: NotRequired[Sequence[ParticipantTokenCapabilityType]],  # (1)
```

1. See [:material-code-brackets: ParticipantTokenCapabilityType](./literals.md#participanttokencapabilitytype) 
## ParticipantTokenTypeDef

```python
# ParticipantTokenTypeDef definition

class ParticipantTokenTypeDef(TypedDict):
    participantId: NotRequired[str],
    token: NotRequired[str],
    userId: NotRequired[str],
    attributes: NotRequired[Dict[str, str]],
    duration: NotRequired[int],
    capabilities: NotRequired[List[ParticipantTokenCapabilityType]],  # (1)
    expirationTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ParticipantTokenCapabilityType](./literals.md#participanttokencapabilitytype) 
## ParticipantTokenConfigurationTypeDef

```python
# ParticipantTokenConfigurationTypeDef definition

class ParticipantTokenConfigurationTypeDef(TypedDict):
    duration: NotRequired[int],
    userId: NotRequired[str],
    attributes: NotRequired[Mapping[str, str]],
    capabilities: NotRequired[Sequence[ParticipantTokenCapabilityType]],  # (1)
```

1. See [:material-code-brackets: ParticipantTokenCapabilityType](./literals.md#participanttokencapabilitytype) 
## S3StorageConfigurationTypeDef

```python
# S3StorageConfigurationTypeDef definition

class S3StorageConfigurationTypeDef(TypedDict):
    bucketName: str,
```

## DeleteEncoderConfigurationRequestRequestTypeDef

```python
# DeleteEncoderConfigurationRequestRequestTypeDef definition

class DeleteEncoderConfigurationRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteIngestConfigurationRequestRequestTypeDef

```python
# DeleteIngestConfigurationRequestRequestTypeDef definition

class DeleteIngestConfigurationRequestRequestTypeDef(TypedDict):
    arn: str,
    force: NotRequired[bool],
```

## DeletePublicKeyRequestRequestTypeDef

```python
# DeletePublicKeyRequestRequestTypeDef definition

class DeletePublicKeyRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteStageRequestRequestTypeDef

```python
# DeleteStageRequestRequestTypeDef definition

class DeleteStageRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteStorageConfigurationRequestRequestTypeDef

```python
# DeleteStorageConfigurationRequestRequestTypeDef definition

class DeleteStorageConfigurationRequestRequestTypeDef(TypedDict):
    arn: str,
```

## S3DetailTypeDef

```python
# S3DetailTypeDef definition

class S3DetailTypeDef(TypedDict):
    recordingPrefix: str,
```

## DisconnectParticipantRequestRequestTypeDef

```python
# DisconnectParticipantRequestRequestTypeDef definition

class DisconnectParticipantRequestRequestTypeDef(TypedDict):
    stageArn: str,
    participantId: str,
    reason: NotRequired[str],
```

## EncoderConfigurationSummaryTypeDef

```python
# EncoderConfigurationSummaryTypeDef definition

class EncoderConfigurationSummaryTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## EventTypeDef

```python
# EventTypeDef definition

class EventTypeDef(TypedDict):
    name: NotRequired[EventNameType],  # (1)
    participantId: NotRequired[str],
    eventTime: NotRequired[datetime],
    remoteParticipantId: NotRequired[str],
    errorCode: NotRequired[EventErrorCodeType],  # (2)
```

1. See [:material-code-brackets: EventNameType](./literals.md#eventnametype) 
2. See [:material-code-brackets: EventErrorCodeType](./literals.md#eventerrorcodetype) 
## GetCompositionRequestRequestTypeDef

```python
# GetCompositionRequestRequestTypeDef definition

class GetCompositionRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetEncoderConfigurationRequestRequestTypeDef

```python
# GetEncoderConfigurationRequestRequestTypeDef definition

class GetEncoderConfigurationRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetIngestConfigurationRequestRequestTypeDef

```python
# GetIngestConfigurationRequestRequestTypeDef definition

class GetIngestConfigurationRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetParticipantRequestRequestTypeDef

```python
# GetParticipantRequestRequestTypeDef definition

class GetParticipantRequestRequestTypeDef(TypedDict):
    stageArn: str,
    sessionId: str,
    participantId: str,
```

## ParticipantTypeDef

```python
# ParticipantTypeDef definition

class ParticipantTypeDef(TypedDict):
    participantId: NotRequired[str],
    userId: NotRequired[str],
    state: NotRequired[ParticipantStateType],  # (1)
    firstJoinTime: NotRequired[datetime],
    attributes: NotRequired[Dict[str, str]],
    published: NotRequired[bool],
    ispName: NotRequired[str],
    osName: NotRequired[str],
    osVersion: NotRequired[str],
    browserName: NotRequired[str],
    browserVersion: NotRequired[str],
    sdkVersion: NotRequired[str],
    recordingS3BucketName: NotRequired[str],
    recordingS3Prefix: NotRequired[str],
    recordingState: NotRequired[ParticipantRecordingStateType],  # (2)
    protocol: NotRequired[ParticipantProtocolType],  # (3)
```

1. See [:material-code-brackets: ParticipantStateType](./literals.md#participantstatetype) 
2. See [:material-code-brackets: ParticipantRecordingStateType](./literals.md#participantrecordingstatetype) 
3. See [:material-code-brackets: ParticipantProtocolType](./literals.md#participantprotocoltype) 
## GetPublicKeyRequestRequestTypeDef

```python
# GetPublicKeyRequestRequestTypeDef definition

class GetPublicKeyRequestRequestTypeDef(TypedDict):
    arn: str,
```

## PublicKeyTypeDef

```python
# PublicKeyTypeDef definition

class PublicKeyTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    publicKeyMaterial: NotRequired[str],
    fingerprint: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

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
    stageArn: str,
    sessionId: str,
```

## StageSessionTypeDef

```python
# StageSessionTypeDef definition

class StageSessionTypeDef(TypedDict):
    sessionId: NotRequired[str],
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
```

## GetStorageConfigurationRequestRequestTypeDef

```python
# GetStorageConfigurationRequestRequestTypeDef definition

class GetStorageConfigurationRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GridConfigurationTypeDef

```python
# GridConfigurationTypeDef definition

class GridConfigurationTypeDef(TypedDict):
    featuredParticipantAttribute: NotRequired[str],
    omitStoppedVideo: NotRequired[bool],
    videoAspectRatio: NotRequired[VideoAspectRatioType],  # (1)
    videoFillMode: NotRequired[VideoFillModeType],  # (2)
    gridGap: NotRequired[int],
```

1. See [:material-code-brackets: VideoAspectRatioType](./literals.md#videoaspectratiotype) 
2. See [:material-code-brackets: VideoFillModeType](./literals.md#videofillmodetype) 
## ImportPublicKeyRequestRequestTypeDef

```python
# ImportPublicKeyRequestRequestTypeDef definition

class ImportPublicKeyRequestRequestTypeDef(TypedDict):
    publicKeyMaterial: str,
    name: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## IngestConfigurationSummaryTypeDef

```python
# IngestConfigurationSummaryTypeDef definition

class IngestConfigurationSummaryTypeDef(TypedDict):
    arn: str,
    ingestProtocol: IngestProtocolType,  # (1)
    stageArn: str,
    participantId: str,
    state: IngestConfigurationStateType,  # (2)
    name: NotRequired[str],
    userId: NotRequired[str],
```

1. See [:material-code-brackets: IngestProtocolType](./literals.md#ingestprotocoltype) 
2. See [:material-code-brackets: IngestConfigurationStateType](./literals.md#ingestconfigurationstatetype) 
## PipConfigurationTypeDef

```python
# PipConfigurationTypeDef definition

class PipConfigurationTypeDef(TypedDict):
    featuredParticipantAttribute: NotRequired[str],
    omitStoppedVideo: NotRequired[bool],
    videoFillMode: NotRequired[VideoFillModeType],  # (1)
    gridGap: NotRequired[int],
    pipParticipantAttribute: NotRequired[str],
    pipBehavior: NotRequired[PipBehaviorType],  # (2)
    pipOffset: NotRequired[int],
    pipPosition: NotRequired[PipPositionType],  # (3)
    pipWidth: NotRequired[int],
    pipHeight: NotRequired[int],
```

1. See [:material-code-brackets: VideoFillModeType](./literals.md#videofillmodetype) 
2. See [:material-code-brackets: PipBehaviorType](./literals.md#pipbehaviortype) 
3. See [:material-code-brackets: PipPositionType](./literals.md#pippositiontype) 
## ListCompositionsRequestRequestTypeDef

```python
# ListCompositionsRequestRequestTypeDef definition

class ListCompositionsRequestRequestTypeDef(TypedDict):
    filterByStageArn: NotRequired[str],
    filterByEncoderConfigurationArn: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListEncoderConfigurationsRequestRequestTypeDef

```python
# ListEncoderConfigurationsRequestRequestTypeDef definition

class ListEncoderConfigurationsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListIngestConfigurationsRequestRequestTypeDef

```python
# ListIngestConfigurationsRequestRequestTypeDef definition

class ListIngestConfigurationsRequestRequestTypeDef(TypedDict):
    filterByStageArn: NotRequired[str],
    filterByState: NotRequired[IngestConfigurationStateType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: IngestConfigurationStateType](./literals.md#ingestconfigurationstatetype) 
## ListParticipantEventsRequestRequestTypeDef

```python
# ListParticipantEventsRequestRequestTypeDef definition

class ListParticipantEventsRequestRequestTypeDef(TypedDict):
    stageArn: str,
    sessionId: str,
    participantId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListParticipantsRequestRequestTypeDef

```python
# ListParticipantsRequestRequestTypeDef definition

class ListParticipantsRequestRequestTypeDef(TypedDict):
    stageArn: str,
    sessionId: str,
    filterByUserId: NotRequired[str],
    filterByPublished: NotRequired[bool],
    filterByState: NotRequired[ParticipantStateType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filterByRecordingState: NotRequired[ParticipantRecordingFilterByRecordingStateType],  # (2)
```

1. See [:material-code-brackets: ParticipantStateType](./literals.md#participantstatetype) 
2. See [:material-code-brackets: ParticipantRecordingFilterByRecordingStateType](./literals.md#participantrecordingfilterbyrecordingstatetype) 
## ParticipantSummaryTypeDef

```python
# ParticipantSummaryTypeDef definition

class ParticipantSummaryTypeDef(TypedDict):
    participantId: NotRequired[str],
    userId: NotRequired[str],
    state: NotRequired[ParticipantStateType],  # (1)
    firstJoinTime: NotRequired[datetime],
    published: NotRequired[bool],
    recordingState: NotRequired[ParticipantRecordingStateType],  # (2)
```

1. See [:material-code-brackets: ParticipantStateType](./literals.md#participantstatetype) 
2. See [:material-code-brackets: ParticipantRecordingStateType](./literals.md#participantrecordingstatetype) 
## ListPublicKeysRequestRequestTypeDef

```python
# ListPublicKeysRequestRequestTypeDef definition

class ListPublicKeysRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## PublicKeySummaryTypeDef

```python
# PublicKeySummaryTypeDef definition

class PublicKeySummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## ListStageSessionsRequestRequestTypeDef

```python
# ListStageSessionsRequestRequestTypeDef definition

class ListStageSessionsRequestRequestTypeDef(TypedDict):
    stageArn: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## StageSessionSummaryTypeDef

```python
# StageSessionSummaryTypeDef definition

class StageSessionSummaryTypeDef(TypedDict):
    sessionId: NotRequired[str],
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
```

## ListStagesRequestRequestTypeDef

```python
# ListStagesRequestRequestTypeDef definition

class ListStagesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## StageSummaryTypeDef

```python
# StageSummaryTypeDef definition

class StageSummaryTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    activeSessionId: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## ListStorageConfigurationsRequestRequestTypeDef

```python
# ListStorageConfigurationsRequestRequestTypeDef definition

class ListStorageConfigurationsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## RecordingConfigurationTypeDef

```python
# RecordingConfigurationTypeDef definition

class RecordingConfigurationTypeDef(TypedDict):
    format: NotRequired[RecordingConfigurationFormatType],  # (1)
```

1. See [:material-code-brackets: RecordingConfigurationFormatType](./literals.md#recordingconfigurationformattype) 
## StageEndpointsTypeDef

```python
# StageEndpointsTypeDef definition

class StageEndpointsTypeDef(TypedDict):
    events: NotRequired[str],
    whip: NotRequired[str],
    rtmp: NotRequired[str],
    rtmps: NotRequired[str],
```

## StopCompositionRequestRequestTypeDef

```python
# StopCompositionRequestRequestTypeDef definition

class StopCompositionRequestRequestTypeDef(TypedDict):
    arn: str,
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

## UpdateIngestConfigurationRequestRequestTypeDef

```python
# UpdateIngestConfigurationRequestRequestTypeDef definition

class UpdateIngestConfigurationRequestRequestTypeDef(TypedDict):
    arn: str,
    stageArn: NotRequired[str],
```

## UpdateStageRequestRequestTypeDef

```python
# UpdateStageRequestRequestTypeDef definition

class UpdateStageRequestRequestTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    autoParticipantRecordingConfiguration: NotRequired[AutoParticipantRecordingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: AutoParticipantRecordingConfigurationTypeDef](./type_defs.md#autoparticipantrecordingconfigurationtypedef) 
## CompositionSummaryTypeDef

```python
# CompositionSummaryTypeDef definition

class CompositionSummaryTypeDef(TypedDict):
    arn: str,
    stageArn: str,
    destinations: List[DestinationSummaryTypeDef],  # (1)
    state: CompositionStateType,  # (2)
    tags: NotRequired[Dict[str, str]],
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
```

1. See [:material-code-braces: DestinationSummaryTypeDef](./type_defs.md#destinationsummarytypedef) 
2. See [:material-code-brackets: CompositionStateType](./literals.md#compositionstatetype) 
## CreateEncoderConfigurationRequestRequestTypeDef

```python
# CreateEncoderConfigurationRequestRequestTypeDef definition

class CreateEncoderConfigurationRequestRequestTypeDef(TypedDict):
    name: NotRequired[str],
    video: NotRequired[VideoTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: VideoTypeDef](./type_defs.md#videotypedef) 
## EncoderConfigurationTypeDef

```python
# EncoderConfigurationTypeDef definition

class EncoderConfigurationTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    video: NotRequired[VideoTypeDef],  # (1)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: VideoTypeDef](./type_defs.md#videotypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIngestConfigurationResponseTypeDef

```python
# CreateIngestConfigurationResponseTypeDef definition

class CreateIngestConfigurationResponseTypeDef(TypedDict):
    ingestConfiguration: IngestConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestConfigurationTypeDef](./type_defs.md#ingestconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIngestConfigurationResponseTypeDef

```python
# GetIngestConfigurationResponseTypeDef definition

class GetIngestConfigurationResponseTypeDef(TypedDict):
    ingestConfiguration: IngestConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestConfigurationTypeDef](./type_defs.md#ingestconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIngestConfigurationResponseTypeDef

```python
# UpdateIngestConfigurationResponseTypeDef definition

class UpdateIngestConfigurationResponseTypeDef(TypedDict):
    ingestConfiguration: IngestConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestConfigurationTypeDef](./type_defs.md#ingestconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateParticipantTokenResponseTypeDef

```python
# CreateParticipantTokenResponseTypeDef definition

class CreateParticipantTokenResponseTypeDef(TypedDict):
    participantToken: ParticipantTokenTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParticipantTokenTypeDef](./type_defs.md#participanttokentypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStageRequestRequestTypeDef

```python
# CreateStageRequestRequestTypeDef definition

class CreateStageRequestRequestTypeDef(TypedDict):
    name: NotRequired[str],
    participantTokenConfigurations: NotRequired[Sequence[ParticipantTokenConfigurationTypeDef]],  # (1)
    tags: NotRequired[Mapping[str, str]],
    autoParticipantRecordingConfiguration: NotRequired[AutoParticipantRecordingConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ParticipantTokenConfigurationTypeDef](./type_defs.md#participanttokenconfigurationtypedef) 
2. See [:material-code-braces: AutoParticipantRecordingConfigurationTypeDef](./type_defs.md#autoparticipantrecordingconfigurationtypedef) 
## CreateStorageConfigurationRequestRequestTypeDef

```python
# CreateStorageConfigurationRequestRequestTypeDef definition

class CreateStorageConfigurationRequestRequestTypeDef(TypedDict):
    s3: S3StorageConfigurationTypeDef,  # (1)
    name: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: S3StorageConfigurationTypeDef](./type_defs.md#s3storageconfigurationtypedef) 
## StorageConfigurationSummaryTypeDef

```python
# StorageConfigurationSummaryTypeDef definition

class StorageConfigurationSummaryTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    s3: NotRequired[S3StorageConfigurationTypeDef],  # (1)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: S3StorageConfigurationTypeDef](./type_defs.md#s3storageconfigurationtypedef) 
## StorageConfigurationTypeDef

```python
# StorageConfigurationTypeDef definition

class StorageConfigurationTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    s3: NotRequired[S3StorageConfigurationTypeDef],  # (1)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: S3StorageConfigurationTypeDef](./type_defs.md#s3storageconfigurationtypedef) 
## DestinationDetailTypeDef

```python
# DestinationDetailTypeDef definition

class DestinationDetailTypeDef(TypedDict):
    s3: NotRequired[S3DetailTypeDef],  # (1)
```

1. See [:material-code-braces: S3DetailTypeDef](./type_defs.md#s3detailtypedef) 
## ListEncoderConfigurationsResponseTypeDef

```python
# ListEncoderConfigurationsResponseTypeDef definition

class ListEncoderConfigurationsResponseTypeDef(TypedDict):
    encoderConfigurations: List[EncoderConfigurationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EncoderConfigurationSummaryTypeDef](./type_defs.md#encoderconfigurationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListParticipantEventsResponseTypeDef

```python
# ListParticipantEventsResponseTypeDef definition

class ListParticipantEventsResponseTypeDef(TypedDict):
    events: List[EventTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
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
## GetPublicKeyResponseTypeDef

```python
# GetPublicKeyResponseTypeDef definition

class GetPublicKeyResponseTypeDef(TypedDict):
    publicKey: PublicKeyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PublicKeyTypeDef](./type_defs.md#publickeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportPublicKeyResponseTypeDef

```python
# ImportPublicKeyResponseTypeDef definition

class ImportPublicKeyResponseTypeDef(TypedDict):
    publicKey: PublicKeyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PublicKeyTypeDef](./type_defs.md#publickeytypedef) 
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
## ListIngestConfigurationsResponseTypeDef

```python
# ListIngestConfigurationsResponseTypeDef definition

class ListIngestConfigurationsResponseTypeDef(TypedDict):
    ingestConfigurations: List[IngestConfigurationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: IngestConfigurationSummaryTypeDef](./type_defs.md#ingestconfigurationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LayoutConfigurationTypeDef

```python
# LayoutConfigurationTypeDef definition

class LayoutConfigurationTypeDef(TypedDict):
    grid: NotRequired[GridConfigurationTypeDef],  # (1)
    pip: NotRequired[PipConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: GridConfigurationTypeDef](./type_defs.md#gridconfigurationtypedef) 
2. See [:material-code-braces: PipConfigurationTypeDef](./type_defs.md#pipconfigurationtypedef) 
## ListIngestConfigurationsRequestListIngestConfigurationsPaginateTypeDef

```python
# ListIngestConfigurationsRequestListIngestConfigurationsPaginateTypeDef definition

class ListIngestConfigurationsRequestListIngestConfigurationsPaginateTypeDef(TypedDict):
    filterByStageArn: NotRequired[str],
    filterByState: NotRequired[IngestConfigurationStateType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: IngestConfigurationStateType](./literals.md#ingestconfigurationstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPublicKeysRequestListPublicKeysPaginateTypeDef

```python
# ListPublicKeysRequestListPublicKeysPaginateTypeDef definition

class ListPublicKeysRequestListPublicKeysPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListParticipantsResponseTypeDef

```python
# ListParticipantsResponseTypeDef definition

class ListParticipantsResponseTypeDef(TypedDict):
    participants: List[ParticipantSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ParticipantSummaryTypeDef](./type_defs.md#participantsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPublicKeysResponseTypeDef

```python
# ListPublicKeysResponseTypeDef definition

class ListPublicKeysResponseTypeDef(TypedDict):
    publicKeys: List[PublicKeySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PublicKeySummaryTypeDef](./type_defs.md#publickeysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStageSessionsResponseTypeDef

```python
# ListStageSessionsResponseTypeDef definition

class ListStageSessionsResponseTypeDef(TypedDict):
    stageSessions: List[StageSessionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: StageSessionSummaryTypeDef](./type_defs.md#stagesessionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStagesResponseTypeDef

```python
# ListStagesResponseTypeDef definition

class ListStagesResponseTypeDef(TypedDict):
    stages: List[StageSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: StageSummaryTypeDef](./type_defs.md#stagesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## S3DestinationConfigurationOutputTypeDef

```python
# S3DestinationConfigurationOutputTypeDef definition

class S3DestinationConfigurationOutputTypeDef(TypedDict):
    storageConfigurationArn: str,
    encoderConfigurationArns: List[str],
    recordingConfiguration: NotRequired[RecordingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: RecordingConfigurationTypeDef](./type_defs.md#recordingconfigurationtypedef) 
## S3DestinationConfigurationTypeDef

```python
# S3DestinationConfigurationTypeDef definition

class S3DestinationConfigurationTypeDef(TypedDict):
    storageConfigurationArn: str,
    encoderConfigurationArns: Sequence[str],
    recordingConfiguration: NotRequired[RecordingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: RecordingConfigurationTypeDef](./type_defs.md#recordingconfigurationtypedef) 
## StageTypeDef

```python
# StageTypeDef definition

class StageTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    activeSessionId: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    autoParticipantRecordingConfiguration: NotRequired[AutoParticipantRecordingConfigurationOutputTypeDef],  # (1)
    endpoints: NotRequired[StageEndpointsTypeDef],  # (2)
```

1. See [:material-code-braces: AutoParticipantRecordingConfigurationOutputTypeDef](./type_defs.md#autoparticipantrecordingconfigurationoutputtypedef) 
2. See [:material-code-braces: StageEndpointsTypeDef](./type_defs.md#stageendpointstypedef) 
## ListCompositionsResponseTypeDef

```python
# ListCompositionsResponseTypeDef definition

class ListCompositionsResponseTypeDef(TypedDict):
    compositions: List[CompositionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CompositionSummaryTypeDef](./type_defs.md#compositionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEncoderConfigurationResponseTypeDef

```python
# CreateEncoderConfigurationResponseTypeDef definition

class CreateEncoderConfigurationResponseTypeDef(TypedDict):
    encoderConfiguration: EncoderConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EncoderConfigurationTypeDef](./type_defs.md#encoderconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEncoderConfigurationResponseTypeDef

```python
# GetEncoderConfigurationResponseTypeDef definition

class GetEncoderConfigurationResponseTypeDef(TypedDict):
    encoderConfiguration: EncoderConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EncoderConfigurationTypeDef](./type_defs.md#encoderconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStorageConfigurationsResponseTypeDef

```python
# ListStorageConfigurationsResponseTypeDef definition

class ListStorageConfigurationsResponseTypeDef(TypedDict):
    storageConfigurations: List[StorageConfigurationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: StorageConfigurationSummaryTypeDef](./type_defs.md#storageconfigurationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStorageConfigurationResponseTypeDef

```python
# CreateStorageConfigurationResponseTypeDef definition

class CreateStorageConfigurationResponseTypeDef(TypedDict):
    storageConfiguration: StorageConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStorageConfigurationResponseTypeDef

```python
# GetStorageConfigurationResponseTypeDef definition

class GetStorageConfigurationResponseTypeDef(TypedDict):
    storageConfiguration: StorageConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DestinationConfigurationOutputTypeDef

```python
# DestinationConfigurationOutputTypeDef definition

class DestinationConfigurationOutputTypeDef(TypedDict):
    name: NotRequired[str],
    channel: NotRequired[ChannelDestinationConfigurationTypeDef],  # (1)
    s3: NotRequired[S3DestinationConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ChannelDestinationConfigurationTypeDef](./type_defs.md#channeldestinationconfigurationtypedef) 
2. See [:material-code-braces: S3DestinationConfigurationOutputTypeDef](./type_defs.md#s3destinationconfigurationoutputtypedef) 
## CreateStageResponseTypeDef

```python
# CreateStageResponseTypeDef definition

class CreateStageResponseTypeDef(TypedDict):
    stage: StageTypeDef,  # (1)
    participantTokens: List[ParticipantTokenTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: StageTypeDef](./type_defs.md#stagetypedef) 
2. See [:material-code-braces: ParticipantTokenTypeDef](./type_defs.md#participanttokentypedef) 
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
## DestinationTypeDef

```python
# DestinationTypeDef definition

class DestinationTypeDef(TypedDict):
    id: str,
    state: DestinationStateType,  # (1)
    configuration: DestinationConfigurationOutputTypeDef,  # (2)
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
    detail: NotRequired[DestinationDetailTypeDef],  # (3)
```

1. See [:material-code-brackets: DestinationStateType](./literals.md#destinationstatetype) 
2. See [:material-code-braces: DestinationConfigurationOutputTypeDef](./type_defs.md#destinationconfigurationoutputtypedef) 
3. See [:material-code-braces: DestinationDetailTypeDef](./type_defs.md#destinationdetailtypedef) 
## DestinationConfigurationTypeDef

```python
# DestinationConfigurationTypeDef definition

class DestinationConfigurationTypeDef(TypedDict):
    name: NotRequired[str],
    channel: NotRequired[ChannelDestinationConfigurationTypeDef],  # (1)
    s3: NotRequired[S3DestinationConfigurationUnionTypeDef],  # (2)
```

1. See [:material-code-braces: ChannelDestinationConfigurationTypeDef](./type_defs.md#channeldestinationconfigurationtypedef) 
2. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) [:material-code-braces: S3DestinationConfigurationOutputTypeDef](./type_defs.md#s3destinationconfigurationoutputtypedef) 
## CompositionTypeDef

```python
# CompositionTypeDef definition

class CompositionTypeDef(TypedDict):
    arn: str,
    stageArn: str,
    state: CompositionStateType,  # (1)
    layout: LayoutConfigurationTypeDef,  # (2)
    destinations: List[DestinationTypeDef],  # (3)
    tags: NotRequired[Dict[str, str]],
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
```

1. See [:material-code-brackets: CompositionStateType](./literals.md#compositionstatetype) 
2. See [:material-code-braces: LayoutConfigurationTypeDef](./type_defs.md#layoutconfigurationtypedef) 
3. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
## GetCompositionResponseTypeDef

```python
# GetCompositionResponseTypeDef definition

class GetCompositionResponseTypeDef(TypedDict):
    composition: CompositionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CompositionTypeDef](./type_defs.md#compositiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartCompositionResponseTypeDef

```python
# StartCompositionResponseTypeDef definition

class StartCompositionResponseTypeDef(TypedDict):
    composition: CompositionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CompositionTypeDef](./type_defs.md#compositiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartCompositionRequestRequestTypeDef

```python
# StartCompositionRequestRequestTypeDef definition

class StartCompositionRequestRequestTypeDef(TypedDict):
    stageArn: str,
    destinations: Sequence[DestinationConfigurationUnionTypeDef],  # (1)
    idempotencyToken: NotRequired[str],
    layout: NotRequired[LayoutConfigurationTypeDef],  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) [:material-code-braces: DestinationConfigurationOutputTypeDef](./type_defs.md#destinationconfigurationoutputtypedef) 
2. See [:material-code-braces: LayoutConfigurationTypeDef](./type_defs.md#layoutconfigurationtypedef) 
