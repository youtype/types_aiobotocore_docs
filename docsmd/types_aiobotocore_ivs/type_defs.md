# Type definitions

> [Index](../README.md) > [IVS](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IVS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#ivs)
    type annotations stubs module [types-aiobotocore-ivs](https://pypi.org/project/types-aiobotocore-ivs/).



## AudioConfigurationTypeDef

```python
# AudioConfigurationTypeDef definition

class AudioConfigurationTypeDef(TypedDict):
    channels: NotRequired[int],
    codec: NotRequired[str],
    sampleRate: NotRequired[int],
    targetBitrate: NotRequired[int],
    track: NotRequired[str],
```

## BatchErrorTypeDef

```python
# BatchErrorTypeDef definition

class BatchErrorTypeDef(TypedDict):
    arn: NotRequired[str],
    code: NotRequired[str],
    message: NotRequired[str],
```

## BatchGetChannelRequestRequestTypeDef

```python
# BatchGetChannelRequestRequestTypeDef definition

class BatchGetChannelRequestRequestTypeDef(TypedDict):
    arns: Sequence[str],
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

## BatchGetStreamKeyRequestRequestTypeDef

```python
# BatchGetStreamKeyRequestRequestTypeDef definition

class BatchGetStreamKeyRequestRequestTypeDef(TypedDict):
    arns: Sequence[str],
```

## StreamKeyTypeDef

```python
# StreamKeyTypeDef definition

class StreamKeyTypeDef(TypedDict):
    arn: NotRequired[str],
    channelArn: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    value: NotRequired[str],
```

## BatchStartViewerSessionRevocationErrorTypeDef

```python
# BatchStartViewerSessionRevocationErrorTypeDef definition

class BatchStartViewerSessionRevocationErrorTypeDef(TypedDict):
    channelArn: str,
    viewerId: str,
    code: NotRequired[str],
    message: NotRequired[str],
```

## BatchStartViewerSessionRevocationViewerSessionTypeDef

```python
# BatchStartViewerSessionRevocationViewerSessionTypeDef definition

class BatchStartViewerSessionRevocationViewerSessionTypeDef(TypedDict):
    channelArn: str,
    viewerId: str,
    viewerSessionVersionsLessThanOrEqualTo: NotRequired[int],
```

## ChannelSummaryTypeDef

```python
# ChannelSummaryTypeDef definition

class ChannelSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    authorized: NotRequired[bool],
    insecureIngest: NotRequired[bool],
    latencyMode: NotRequired[ChannelLatencyModeType],  # (1)
    name: NotRequired[str],
    playbackRestrictionPolicyArn: NotRequired[str],
    preset: NotRequired[TranscodePresetType],  # (2)
    recordingConfigurationArn: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    type: NotRequired[ChannelTypeType],  # (3)
```

1. See [:material-code-brackets: ChannelLatencyModeType](./literals.md#channellatencymodetype) 
2. See [:material-code-brackets: TranscodePresetType](./literals.md#transcodepresettype) 
3. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
## MultitrackInputConfigurationTypeDef

```python
# MultitrackInputConfigurationTypeDef definition

class MultitrackInputConfigurationTypeDef(TypedDict):
    enabled: NotRequired[bool],
    maximumResolution: NotRequired[MultitrackMaximumResolutionType],  # (1)
    policy: NotRequired[MultitrackPolicyType],  # (2)
```

1. See [:material-code-brackets: MultitrackMaximumResolutionType](./literals.md#multitrackmaximumresolutiontype) 
2. See [:material-code-brackets: MultitrackPolicyType](./literals.md#multitrackpolicytype) 
## SrtTypeDef

```python
# SrtTypeDef definition

class SrtTypeDef(TypedDict):
    endpoint: NotRequired[str],
    passphrase: NotRequired[str],
```

## CreatePlaybackRestrictionPolicyRequestRequestTypeDef

```python
# CreatePlaybackRestrictionPolicyRequestRequestTypeDef definition

class CreatePlaybackRestrictionPolicyRequestRequestTypeDef(TypedDict):
    allowedCountries: NotRequired[Sequence[str]],
    allowedOrigins: NotRequired[Sequence[str]],
    enableStrictOriginEnforcement: NotRequired[bool],
    name: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## PlaybackRestrictionPolicyTypeDef

```python
# PlaybackRestrictionPolicyTypeDef definition

class PlaybackRestrictionPolicyTypeDef(TypedDict):
    allowedCountries: List[str],
    allowedOrigins: List[str],
    arn: str,
    enableStrictOriginEnforcement: NotRequired[bool],
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## RenditionConfigurationTypeDef

```python
# RenditionConfigurationTypeDef definition

class RenditionConfigurationTypeDef(TypedDict):
    renditionSelection: NotRequired[RenditionConfigurationRenditionSelectionType],  # (1)
    renditions: NotRequired[Sequence[RenditionConfigurationRenditionType]],  # (2)
```

1. See [:material-code-brackets: RenditionConfigurationRenditionSelectionType](./literals.md#renditionconfigurationrenditionselectiontype) 
2. See [:material-code-brackets: RenditionConfigurationRenditionType](./literals.md#renditionconfigurationrenditiontype) 
## ThumbnailConfigurationTypeDef

```python
# ThumbnailConfigurationTypeDef definition

class ThumbnailConfigurationTypeDef(TypedDict):
    recordingMode: NotRequired[RecordingModeType],  # (1)
    resolution: NotRequired[ThumbnailConfigurationResolutionType],  # (2)
    storage: NotRequired[Sequence[ThumbnailConfigurationStorageType]],  # (3)
    targetIntervalSeconds: NotRequired[int],
```

1. See [:material-code-brackets: RecordingModeType](./literals.md#recordingmodetype) 
2. See [:material-code-brackets: ThumbnailConfigurationResolutionType](./literals.md#thumbnailconfigurationresolutiontype) 
3. See [:material-code-brackets: ThumbnailConfigurationStorageType](./literals.md#thumbnailconfigurationstoragetype) 
## CreateStreamKeyRequestRequestTypeDef

```python
# CreateStreamKeyRequestRequestTypeDef definition

class CreateStreamKeyRequestRequestTypeDef(TypedDict):
    channelArn: str,
    tags: NotRequired[Mapping[str, str]],
```

## DeleteChannelRequestRequestTypeDef

```python
# DeleteChannelRequestRequestTypeDef definition

class DeleteChannelRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeletePlaybackKeyPairRequestRequestTypeDef

```python
# DeletePlaybackKeyPairRequestRequestTypeDef definition

class DeletePlaybackKeyPairRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeletePlaybackRestrictionPolicyRequestRequestTypeDef

```python
# DeletePlaybackRestrictionPolicyRequestRequestTypeDef definition

class DeletePlaybackRestrictionPolicyRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteRecordingConfigurationRequestRequestTypeDef

```python
# DeleteRecordingConfigurationRequestRequestTypeDef definition

class DeleteRecordingConfigurationRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteStreamKeyRequestRequestTypeDef

```python
# DeleteStreamKeyRequestRequestTypeDef definition

class DeleteStreamKeyRequestRequestTypeDef(TypedDict):
    arn: str,
```

## S3DestinationConfigurationTypeDef

```python
# S3DestinationConfigurationTypeDef definition

class S3DestinationConfigurationTypeDef(TypedDict):
    bucketName: str,
```

## GetChannelRequestRequestTypeDef

```python
# GetChannelRequestRequestTypeDef definition

class GetChannelRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetPlaybackKeyPairRequestRequestTypeDef

```python
# GetPlaybackKeyPairRequestRequestTypeDef definition

class GetPlaybackKeyPairRequestRequestTypeDef(TypedDict):
    arn: str,
```

## PlaybackKeyPairTypeDef

```python
# PlaybackKeyPairTypeDef definition

class PlaybackKeyPairTypeDef(TypedDict):
    arn: NotRequired[str],
    fingerprint: NotRequired[str],
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## GetPlaybackRestrictionPolicyRequestRequestTypeDef

```python
# GetPlaybackRestrictionPolicyRequestRequestTypeDef definition

class GetPlaybackRestrictionPolicyRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetRecordingConfigurationRequestRequestTypeDef

```python
# GetRecordingConfigurationRequestRequestTypeDef definition

class GetRecordingConfigurationRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetStreamKeyRequestRequestTypeDef

```python
# GetStreamKeyRequestRequestTypeDef definition

class GetStreamKeyRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetStreamRequestRequestTypeDef

```python
# GetStreamRequestRequestTypeDef definition

class GetStreamRequestRequestTypeDef(TypedDict):
    channelArn: str,
```

## StreamTypeDef

```python
# StreamTypeDef definition

class StreamTypeDef(TypedDict):
    channelArn: NotRequired[str],
    health: NotRequired[StreamHealthType],  # (1)
    playbackUrl: NotRequired[str],
    startTime: NotRequired[datetime],
    state: NotRequired[StreamStateType],  # (2)
    streamId: NotRequired[str],
    viewerCount: NotRequired[int],
```

1. See [:material-code-brackets: StreamHealthType](./literals.md#streamhealthtype) 
2. See [:material-code-brackets: StreamStateType](./literals.md#streamstatetype) 
## GetStreamSessionRequestRequestTypeDef

```python
# GetStreamSessionRequestRequestTypeDef definition

class GetStreamSessionRequestRequestTypeDef(TypedDict):
    channelArn: str,
    streamId: NotRequired[str],
```

## ImportPlaybackKeyPairRequestRequestTypeDef

```python
# ImportPlaybackKeyPairRequestRequestTypeDef definition

class ImportPlaybackKeyPairRequestRequestTypeDef(TypedDict):
    publicKeyMaterial: str,
    name: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## VideoConfigurationTypeDef

```python
# VideoConfigurationTypeDef definition

class VideoConfigurationTypeDef(TypedDict):
    avcLevel: NotRequired[str],
    avcProfile: NotRequired[str],
    codec: NotRequired[str],
    encoder: NotRequired[str],
    level: NotRequired[str],
    profile: NotRequired[str],
    targetBitrate: NotRequired[int],
    targetFramerate: NotRequired[int],
    track: NotRequired[str],
    videoHeight: NotRequired[int],
    videoWidth: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListChannelsRequestRequestTypeDef

```python
# ListChannelsRequestRequestTypeDef definition

class ListChannelsRequestRequestTypeDef(TypedDict):
    filterByName: NotRequired[str],
    filterByPlaybackRestrictionPolicyArn: NotRequired[str],
    filterByRecordingConfigurationArn: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListPlaybackKeyPairsRequestRequestTypeDef

```python
# ListPlaybackKeyPairsRequestRequestTypeDef definition

class ListPlaybackKeyPairsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## PlaybackKeyPairSummaryTypeDef

```python
# PlaybackKeyPairSummaryTypeDef definition

class PlaybackKeyPairSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## ListPlaybackRestrictionPoliciesRequestRequestTypeDef

```python
# ListPlaybackRestrictionPoliciesRequestRequestTypeDef definition

class ListPlaybackRestrictionPoliciesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## PlaybackRestrictionPolicySummaryTypeDef

```python
# PlaybackRestrictionPolicySummaryTypeDef definition

class PlaybackRestrictionPolicySummaryTypeDef(TypedDict):
    allowedCountries: List[str],
    allowedOrigins: List[str],
    arn: str,
    enableStrictOriginEnforcement: NotRequired[bool],
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## ListRecordingConfigurationsRequestRequestTypeDef

```python
# ListRecordingConfigurationsRequestRequestTypeDef definition

class ListRecordingConfigurationsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListStreamKeysRequestRequestTypeDef

```python
# ListStreamKeysRequestRequestTypeDef definition

class ListStreamKeysRequestRequestTypeDef(TypedDict):
    channelArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## StreamKeySummaryTypeDef

```python
# StreamKeySummaryTypeDef definition

class StreamKeySummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    channelArn: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## ListStreamSessionsRequestRequestTypeDef

```python
# ListStreamSessionsRequestRequestTypeDef definition

class ListStreamSessionsRequestRequestTypeDef(TypedDict):
    channelArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## StreamSessionSummaryTypeDef

```python
# StreamSessionSummaryTypeDef definition

class StreamSessionSummaryTypeDef(TypedDict):
    endTime: NotRequired[datetime],
    hasErrorEvent: NotRequired[bool],
    startTime: NotRequired[datetime],
    streamId: NotRequired[str],
```

## StreamFiltersTypeDef

```python
# StreamFiltersTypeDef definition

class StreamFiltersTypeDef(TypedDict):
    health: NotRequired[StreamHealthType],  # (1)
```

1. See [:material-code-brackets: StreamHealthType](./literals.md#streamhealthtype) 
## StreamSummaryTypeDef

```python
# StreamSummaryTypeDef definition

class StreamSummaryTypeDef(TypedDict):
    channelArn: NotRequired[str],
    health: NotRequired[StreamHealthType],  # (1)
    startTime: NotRequired[datetime],
    state: NotRequired[StreamStateType],  # (2)
    streamId: NotRequired[str],
    viewerCount: NotRequired[int],
```

1. See [:material-code-brackets: StreamHealthType](./literals.md#streamhealthtype) 
2. See [:material-code-brackets: StreamStateType](./literals.md#streamstatetype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## PutMetadataRequestRequestTypeDef

```python
# PutMetadataRequestRequestTypeDef definition

class PutMetadataRequestRequestTypeDef(TypedDict):
    channelArn: str,
    metadata: str,
```

## RenditionConfigurationOutputTypeDef

```python
# RenditionConfigurationOutputTypeDef definition

class RenditionConfigurationOutputTypeDef(TypedDict):
    renditionSelection: NotRequired[RenditionConfigurationRenditionSelectionType],  # (1)
    renditions: NotRequired[List[RenditionConfigurationRenditionType]],  # (2)
```

1. See [:material-code-brackets: RenditionConfigurationRenditionSelectionType](./literals.md#renditionconfigurationrenditionselectiontype) 
2. See [:material-code-brackets: RenditionConfigurationRenditionType](./literals.md#renditionconfigurationrenditiontype) 
## ThumbnailConfigurationOutputTypeDef

```python
# ThumbnailConfigurationOutputTypeDef definition

class ThumbnailConfigurationOutputTypeDef(TypedDict):
    recordingMode: NotRequired[RecordingModeType],  # (1)
    resolution: NotRequired[ThumbnailConfigurationResolutionType],  # (2)
    storage: NotRequired[List[ThumbnailConfigurationStorageType]],  # (3)
    targetIntervalSeconds: NotRequired[int],
```

1. See [:material-code-brackets: RecordingModeType](./literals.md#recordingmodetype) 
2. See [:material-code-brackets: ThumbnailConfigurationResolutionType](./literals.md#thumbnailconfigurationresolutiontype) 
3. See [:material-code-brackets: ThumbnailConfigurationStorageType](./literals.md#thumbnailconfigurationstoragetype) 
## StartViewerSessionRevocationRequestRequestTypeDef

```python
# StartViewerSessionRevocationRequestRequestTypeDef definition

class StartViewerSessionRevocationRequestRequestTypeDef(TypedDict):
    channelArn: str,
    viewerId: str,
    viewerSessionVersionsLessThanOrEqualTo: NotRequired[int],
```

## StopStreamRequestRequestTypeDef

```python
# StopStreamRequestRequestTypeDef definition

class StopStreamRequestRequestTypeDef(TypedDict):
    channelArn: str,
```

## StreamEventTypeDef

```python
# StreamEventTypeDef definition

class StreamEventTypeDef(TypedDict):
    code: NotRequired[str],
    eventTime: NotRequired[datetime],
    name: NotRequired[str],
    type: NotRequired[str],
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

## UpdatePlaybackRestrictionPolicyRequestRequestTypeDef

```python
# UpdatePlaybackRestrictionPolicyRequestRequestTypeDef definition

class UpdatePlaybackRestrictionPolicyRequestRequestTypeDef(TypedDict):
    arn: str,
    allowedCountries: NotRequired[Sequence[str]],
    allowedOrigins: NotRequired[Sequence[str]],
    enableStrictOriginEnforcement: NotRequired[bool],
    name: NotRequired[str],
```

## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetStreamKeyResponseTypeDef

```python
# BatchGetStreamKeyResponseTypeDef definition

class BatchGetStreamKeyResponseTypeDef(TypedDict):
    errors: List[BatchErrorTypeDef],  # (1)
    streamKeys: List[StreamKeyTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchErrorTypeDef](./type_defs.md#batcherrortypedef) 
2. See [:material-code-braces: StreamKeyTypeDef](./type_defs.md#streamkeytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStreamKeyResponseTypeDef

```python
# CreateStreamKeyResponseTypeDef definition

class CreateStreamKeyResponseTypeDef(TypedDict):
    streamKey: StreamKeyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamKeyTypeDef](./type_defs.md#streamkeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStreamKeyResponseTypeDef

```python
# GetStreamKeyResponseTypeDef definition

class GetStreamKeyResponseTypeDef(TypedDict):
    streamKey: StreamKeyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamKeyTypeDef](./type_defs.md#streamkeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchStartViewerSessionRevocationResponseTypeDef

```python
# BatchStartViewerSessionRevocationResponseTypeDef definition

class BatchStartViewerSessionRevocationResponseTypeDef(TypedDict):
    errors: List[BatchStartViewerSessionRevocationErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchStartViewerSessionRevocationErrorTypeDef](./type_defs.md#batchstartviewersessionrevocationerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchStartViewerSessionRevocationRequestRequestTypeDef

```python
# BatchStartViewerSessionRevocationRequestRequestTypeDef definition

class BatchStartViewerSessionRevocationRequestRequestTypeDef(TypedDict):
    viewerSessions: Sequence[BatchStartViewerSessionRevocationViewerSessionTypeDef],  # (1)
```

1. See [:material-code-braces: BatchStartViewerSessionRevocationViewerSessionTypeDef](./type_defs.md#batchstartviewersessionrevocationviewersessiontypedef) 
## ListChannelsResponseTypeDef

```python
# ListChannelsResponseTypeDef definition

class ListChannelsResponseTypeDef(TypedDict):
    channels: List[ChannelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ChannelSummaryTypeDef](./type_defs.md#channelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateChannelRequestRequestTypeDef

```python
# CreateChannelRequestRequestTypeDef definition

class CreateChannelRequestRequestTypeDef(TypedDict):
    authorized: NotRequired[bool],
    containerFormat: NotRequired[ContainerFormatType],  # (1)
    insecureIngest: NotRequired[bool],
    latencyMode: NotRequired[ChannelLatencyModeType],  # (2)
    multitrackInputConfiguration: NotRequired[MultitrackInputConfigurationTypeDef],  # (3)
    name: NotRequired[str],
    playbackRestrictionPolicyArn: NotRequired[str],
    preset: NotRequired[TranscodePresetType],  # (4)
    recordingConfigurationArn: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    type: NotRequired[ChannelTypeType],  # (5)
```

1. See [:material-code-brackets: ContainerFormatType](./literals.md#containerformattype) 
2. See [:material-code-brackets: ChannelLatencyModeType](./literals.md#channellatencymodetype) 
3. See [:material-code-braces: MultitrackInputConfigurationTypeDef](./type_defs.md#multitrackinputconfigurationtypedef) 
4. See [:material-code-brackets: TranscodePresetType](./literals.md#transcodepresettype) 
5. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
## UpdateChannelRequestRequestTypeDef

```python
# UpdateChannelRequestRequestTypeDef definition

class UpdateChannelRequestRequestTypeDef(TypedDict):
    arn: str,
    authorized: NotRequired[bool],
    containerFormat: NotRequired[ContainerFormatType],  # (1)
    insecureIngest: NotRequired[bool],
    latencyMode: NotRequired[ChannelLatencyModeType],  # (2)
    multitrackInputConfiguration: NotRequired[MultitrackInputConfigurationTypeDef],  # (3)
    name: NotRequired[str],
    playbackRestrictionPolicyArn: NotRequired[str],
    preset: NotRequired[TranscodePresetType],  # (4)
    recordingConfigurationArn: NotRequired[str],
    type: NotRequired[ChannelTypeType],  # (5)
```

1. See [:material-code-brackets: ContainerFormatType](./literals.md#containerformattype) 
2. See [:material-code-brackets: ChannelLatencyModeType](./literals.md#channellatencymodetype) 
3. See [:material-code-braces: MultitrackInputConfigurationTypeDef](./type_defs.md#multitrackinputconfigurationtypedef) 
4. See [:material-code-brackets: TranscodePresetType](./literals.md#transcodepresettype) 
5. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
## ChannelTypeDef

```python
# ChannelTypeDef definition

class ChannelTypeDef(TypedDict):
    arn: NotRequired[str],
    authorized: NotRequired[bool],
    containerFormat: NotRequired[ContainerFormatType],  # (1)
    ingestEndpoint: NotRequired[str],
    insecureIngest: NotRequired[bool],
    latencyMode: NotRequired[ChannelLatencyModeType],  # (2)
    multitrackInputConfiguration: NotRequired[MultitrackInputConfigurationTypeDef],  # (3)
    name: NotRequired[str],
    playbackRestrictionPolicyArn: NotRequired[str],
    playbackUrl: NotRequired[str],
    preset: NotRequired[TranscodePresetType],  # (4)
    recordingConfigurationArn: NotRequired[str],
    srt: NotRequired[SrtTypeDef],  # (5)
    tags: NotRequired[Dict[str, str]],
    type: NotRequired[ChannelTypeType],  # (6)
```

1. See [:material-code-brackets: ContainerFormatType](./literals.md#containerformattype) 
2. See [:material-code-brackets: ChannelLatencyModeType](./literals.md#channellatencymodetype) 
3. See [:material-code-braces: MultitrackInputConfigurationTypeDef](./type_defs.md#multitrackinputconfigurationtypedef) 
4. See [:material-code-brackets: TranscodePresetType](./literals.md#transcodepresettype) 
5. See [:material-code-braces: SrtTypeDef](./type_defs.md#srttypedef) 
6. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
## CreatePlaybackRestrictionPolicyResponseTypeDef

```python
# CreatePlaybackRestrictionPolicyResponseTypeDef definition

class CreatePlaybackRestrictionPolicyResponseTypeDef(TypedDict):
    playbackRestrictionPolicy: PlaybackRestrictionPolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PlaybackRestrictionPolicyTypeDef](./type_defs.md#playbackrestrictionpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPlaybackRestrictionPolicyResponseTypeDef

```python
# GetPlaybackRestrictionPolicyResponseTypeDef definition

class GetPlaybackRestrictionPolicyResponseTypeDef(TypedDict):
    playbackRestrictionPolicy: PlaybackRestrictionPolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PlaybackRestrictionPolicyTypeDef](./type_defs.md#playbackrestrictionpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePlaybackRestrictionPolicyResponseTypeDef

```python
# UpdatePlaybackRestrictionPolicyResponseTypeDef definition

class UpdatePlaybackRestrictionPolicyResponseTypeDef(TypedDict):
    playbackRestrictionPolicy: PlaybackRestrictionPolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PlaybackRestrictionPolicyTypeDef](./type_defs.md#playbackrestrictionpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DestinationConfigurationTypeDef

```python
# DestinationConfigurationTypeDef definition

class DestinationConfigurationTypeDef(TypedDict):
    s3: NotRequired[S3DestinationConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) 
## GetPlaybackKeyPairResponseTypeDef

```python
# GetPlaybackKeyPairResponseTypeDef definition

class GetPlaybackKeyPairResponseTypeDef(TypedDict):
    keyPair: PlaybackKeyPairTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PlaybackKeyPairTypeDef](./type_defs.md#playbackkeypairtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportPlaybackKeyPairResponseTypeDef

```python
# ImportPlaybackKeyPairResponseTypeDef definition

class ImportPlaybackKeyPairResponseTypeDef(TypedDict):
    keyPair: PlaybackKeyPairTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PlaybackKeyPairTypeDef](./type_defs.md#playbackkeypairtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStreamResponseTypeDef

```python
# GetStreamResponseTypeDef definition

class GetStreamResponseTypeDef(TypedDict):
    stream: StreamTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamTypeDef](./type_defs.md#streamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IngestConfigurationTypeDef

```python
# IngestConfigurationTypeDef definition

class IngestConfigurationTypeDef(TypedDict):
    audio: NotRequired[AudioConfigurationTypeDef],  # (1)
    video: NotRequired[VideoConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: AudioConfigurationTypeDef](./type_defs.md#audioconfigurationtypedef) 
2. See [:material-code-braces: VideoConfigurationTypeDef](./type_defs.md#videoconfigurationtypedef) 
## IngestConfigurationsTypeDef

```python
# IngestConfigurationsTypeDef definition

class IngestConfigurationsTypeDef(TypedDict):
    audioConfigurations: List[AudioConfigurationTypeDef],  # (1)
    videoConfigurations: List[VideoConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: AudioConfigurationTypeDef](./type_defs.md#audioconfigurationtypedef) 
2. See [:material-code-braces: VideoConfigurationTypeDef](./type_defs.md#videoconfigurationtypedef) 
## ListChannelsRequestPaginateTypeDef

```python
# ListChannelsRequestPaginateTypeDef definition

class ListChannelsRequestPaginateTypeDef(TypedDict):
    filterByName: NotRequired[str],
    filterByPlaybackRestrictionPolicyArn: NotRequired[str],
    filterByRecordingConfigurationArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPlaybackKeyPairsRequestPaginateTypeDef

```python
# ListPlaybackKeyPairsRequestPaginateTypeDef definition

class ListPlaybackKeyPairsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecordingConfigurationsRequestPaginateTypeDef

```python
# ListRecordingConfigurationsRequestPaginateTypeDef definition

class ListRecordingConfigurationsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStreamKeysRequestPaginateTypeDef

```python
# ListStreamKeysRequestPaginateTypeDef definition

class ListStreamKeysRequestPaginateTypeDef(TypedDict):
    channelArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPlaybackKeyPairsResponseTypeDef

```python
# ListPlaybackKeyPairsResponseTypeDef definition

class ListPlaybackKeyPairsResponseTypeDef(TypedDict):
    keyPairs: List[PlaybackKeyPairSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PlaybackKeyPairSummaryTypeDef](./type_defs.md#playbackkeypairsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPlaybackRestrictionPoliciesResponseTypeDef

```python
# ListPlaybackRestrictionPoliciesResponseTypeDef definition

class ListPlaybackRestrictionPoliciesResponseTypeDef(TypedDict):
    playbackRestrictionPolicies: List[PlaybackRestrictionPolicySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PlaybackRestrictionPolicySummaryTypeDef](./type_defs.md#playbackrestrictionpolicysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStreamKeysResponseTypeDef

```python
# ListStreamKeysResponseTypeDef definition

class ListStreamKeysResponseTypeDef(TypedDict):
    streamKeys: List[StreamKeySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: StreamKeySummaryTypeDef](./type_defs.md#streamkeysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStreamSessionsResponseTypeDef

```python
# ListStreamSessionsResponseTypeDef definition

class ListStreamSessionsResponseTypeDef(TypedDict):
    streamSessions: List[StreamSessionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: StreamSessionSummaryTypeDef](./type_defs.md#streamsessionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStreamsRequestPaginateTypeDef

```python
# ListStreamsRequestPaginateTypeDef definition

class ListStreamsRequestPaginateTypeDef(TypedDict):
    filterBy: NotRequired[StreamFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: StreamFiltersTypeDef](./type_defs.md#streamfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStreamsRequestRequestTypeDef

```python
# ListStreamsRequestRequestTypeDef definition

class ListStreamsRequestRequestTypeDef(TypedDict):
    filterBy: NotRequired[StreamFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: StreamFiltersTypeDef](./type_defs.md#streamfilterstypedef) 
## ListStreamsResponseTypeDef

```python
# ListStreamsResponseTypeDef definition

class ListStreamsResponseTypeDef(TypedDict):
    streams: List[StreamSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: StreamSummaryTypeDef](./type_defs.md#streamsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetChannelResponseTypeDef

```python
# BatchGetChannelResponseTypeDef definition

class BatchGetChannelResponseTypeDef(TypedDict):
    channels: List[ChannelTypeDef],  # (1)
    errors: List[BatchErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
2. See [:material-code-braces: BatchErrorTypeDef](./type_defs.md#batcherrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateChannelResponseTypeDef

```python
# CreateChannelResponseTypeDef definition

class CreateChannelResponseTypeDef(TypedDict):
    channel: ChannelTypeDef,  # (1)
    streamKey: StreamKeyTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
2. See [:material-code-braces: StreamKeyTypeDef](./type_defs.md#streamkeytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetChannelResponseTypeDef

```python
# GetChannelResponseTypeDef definition

class GetChannelResponseTypeDef(TypedDict):
    channel: ChannelTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateChannelResponseTypeDef

```python
# UpdateChannelResponseTypeDef definition

class UpdateChannelResponseTypeDef(TypedDict):
    channel: ChannelTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRecordingConfigurationRequestRequestTypeDef

```python
# CreateRecordingConfigurationRequestRequestTypeDef definition

class CreateRecordingConfigurationRequestRequestTypeDef(TypedDict):
    destinationConfiguration: DestinationConfigurationTypeDef,  # (1)
    name: NotRequired[str],
    recordingReconnectWindowSeconds: NotRequired[int],
    renditionConfiguration: NotRequired[RenditionConfigurationTypeDef],  # (2)
    tags: NotRequired[Mapping[str, str]],
    thumbnailConfiguration: NotRequired[ThumbnailConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
2. See [:material-code-braces: RenditionConfigurationTypeDef](./type_defs.md#renditionconfigurationtypedef) 
3. See [:material-code-braces: ThumbnailConfigurationTypeDef](./type_defs.md#thumbnailconfigurationtypedef) 
## RecordingConfigurationSummaryTypeDef

```python
# RecordingConfigurationSummaryTypeDef definition

class RecordingConfigurationSummaryTypeDef(TypedDict):
    arn: str,
    destinationConfiguration: DestinationConfigurationTypeDef,  # (1)
    state: RecordingConfigurationStateType,  # (2)
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
2. See [:material-code-brackets: RecordingConfigurationStateType](./literals.md#recordingconfigurationstatetype) 
## RecordingConfigurationTypeDef

```python
# RecordingConfigurationTypeDef definition

class RecordingConfigurationTypeDef(TypedDict):
    arn: str,
    destinationConfiguration: DestinationConfigurationTypeDef,  # (1)
    state: RecordingConfigurationStateType,  # (3)
    name: NotRequired[str],
    recordingReconnectWindowSeconds: NotRequired[int],
    renditionConfiguration: NotRequired[RenditionConfigurationOutputTypeDef],  # (2)
    tags: NotRequired[Dict[str, str]],
    thumbnailConfiguration: NotRequired[ThumbnailConfigurationOutputTypeDef],  # (4)
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
2. See [:material-code-braces: RenditionConfigurationOutputTypeDef](./type_defs.md#renditionconfigurationoutputtypedef) 
3. See [:material-code-brackets: RecordingConfigurationStateType](./literals.md#recordingconfigurationstatetype) 
4. See [:material-code-braces: ThumbnailConfigurationOutputTypeDef](./type_defs.md#thumbnailconfigurationoutputtypedef) 
## ListRecordingConfigurationsResponseTypeDef

```python
# ListRecordingConfigurationsResponseTypeDef definition

class ListRecordingConfigurationsResponseTypeDef(TypedDict):
    recordingConfigurations: List[RecordingConfigurationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RecordingConfigurationSummaryTypeDef](./type_defs.md#recordingconfigurationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRecordingConfigurationResponseTypeDef

```python
# CreateRecordingConfigurationResponseTypeDef definition

class CreateRecordingConfigurationResponseTypeDef(TypedDict):
    recordingConfiguration: RecordingConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecordingConfigurationTypeDef](./type_defs.md#recordingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRecordingConfigurationResponseTypeDef

```python
# GetRecordingConfigurationResponseTypeDef definition

class GetRecordingConfigurationResponseTypeDef(TypedDict):
    recordingConfiguration: RecordingConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecordingConfigurationTypeDef](./type_defs.md#recordingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StreamSessionTypeDef

```python
# StreamSessionTypeDef definition

class StreamSessionTypeDef(TypedDict):
    channel: NotRequired[ChannelTypeDef],  # (1)
    endTime: NotRequired[datetime],
    ingestConfiguration: NotRequired[IngestConfigurationTypeDef],  # (2)
    ingestConfigurations: NotRequired[IngestConfigurationsTypeDef],  # (3)
    recordingConfiguration: NotRequired[RecordingConfigurationTypeDef],  # (4)
    startTime: NotRequired[datetime],
    streamId: NotRequired[str],
    truncatedEvents: NotRequired[List[StreamEventTypeDef]],  # (5)
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
2. See [:material-code-braces: IngestConfigurationTypeDef](./type_defs.md#ingestconfigurationtypedef) 
3. See [:material-code-braces: IngestConfigurationsTypeDef](./type_defs.md#ingestconfigurationstypedef) 
4. See [:material-code-braces: RecordingConfigurationTypeDef](./type_defs.md#recordingconfigurationtypedef) 
5. See [:material-code-braces: StreamEventTypeDef](./type_defs.md#streameventtypedef) 
## GetStreamSessionResponseTypeDef

```python
# GetStreamSessionResponseTypeDef definition

class GetStreamSessionResponseTypeDef(TypedDict):
    streamSession: StreamSessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamSessionTypeDef](./type_defs.md#streamsessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
