# Type definitions

> [Index](../README.md) > [ElasticTranscoder](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ElasticTranscoder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
    type annotations stubs module [types-aiobotocore-elastictranscoder](https://pypi.org/project/types-aiobotocore-elastictranscoder/).

## PermissionUnionTypeDef

```python
# PermissionUnionTypeDef definition

PermissionUnionTypeDef = Union[
    PermissionTypeDef,  # (1)
    PermissionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PermissionTypeDef](./type_defs.md#permissiontypedef) 
2. See [:material-code-braces: PermissionOutputTypeDef](./type_defs.md#permissionoutputtypedef) 

## JobAlbumArtUnionTypeDef

```python
# JobAlbumArtUnionTypeDef definition

JobAlbumArtUnionTypeDef = Union[
    JobAlbumArtTypeDef,  # (1)
    JobAlbumArtOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: JobAlbumArtTypeDef](./type_defs.md#jobalbumarttypedef) 
2. See [:material-code-braces: JobAlbumArtOutputTypeDef](./type_defs.md#jobalbumartoutputtypedef) 

## CaptionsUnionTypeDef

```python
# CaptionsUnionTypeDef definition

CaptionsUnionTypeDef = Union[
    CaptionsTypeDef,  # (1)
    CaptionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CaptionsTypeDef](./type_defs.md#captionstypedef) 
2. See [:material-code-braces: CaptionsOutputTypeDef](./type_defs.md#captionsoutputtypedef) 

## InputCaptionsUnionTypeDef

```python
# InputCaptionsUnionTypeDef definition

InputCaptionsUnionTypeDef = Union[
    InputCaptionsTypeDef,  # (1)
    InputCaptionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: InputCaptionsTypeDef](./type_defs.md#inputcaptionstypedef) 
2. See [:material-code-braces: InputCaptionsOutputTypeDef](./type_defs.md#inputcaptionsoutputtypedef) 

## JobInputUnionTypeDef

```python
# JobInputUnionTypeDef definition

JobInputUnionTypeDef = Union[
    JobInputTypeDef,  # (1)
    JobInputOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: JobInputTypeDef](./type_defs.md#jobinputtypedef) 
2. See [:material-code-braces: JobInputOutputTypeDef](./type_defs.md#jobinputoutputtypedef) 



## EncryptionTypeDef

```python
# EncryptionTypeDef definition

class EncryptionTypeDef(TypedDict):
    Mode: NotRequired[str],
    Key: NotRequired[str],
    KeyMd5: NotRequired[str],
    InitializationVector: NotRequired[str],
```

## AudioCodecOptionsTypeDef

```python
# AudioCodecOptionsTypeDef definition

class AudioCodecOptionsTypeDef(TypedDict):
    Profile: NotRequired[str],
    BitDepth: NotRequired[str],
    BitOrder: NotRequired[str],
    Signed: NotRequired[str],
```

## CancelJobRequestRequestTypeDef

```python
# CancelJobRequestRequestTypeDef definition

class CancelJobRequestRequestTypeDef(TypedDict):
    Id: str,
```

## TimeSpanTypeDef

```python
# TimeSpanTypeDef definition

class TimeSpanTypeDef(TypedDict):
    StartTime: NotRequired[str],
    Duration: NotRequired[str],
```

## HlsContentProtectionTypeDef

```python
# HlsContentProtectionTypeDef definition

class HlsContentProtectionTypeDef(TypedDict):
    Method: NotRequired[str],
    Key: NotRequired[str],
    KeyMd5: NotRequired[str],
    InitializationVector: NotRequired[str],
    LicenseAcquisitionUrl: NotRequired[str],
    KeyStoragePolicy: NotRequired[str],
```

## PlayReadyDrmTypeDef

```python
# PlayReadyDrmTypeDef definition

class PlayReadyDrmTypeDef(TypedDict):
    Format: NotRequired[str],
    Key: NotRequired[str],
    KeyMd5: NotRequired[str],
    KeyId: NotRequired[str],
    InitializationVector: NotRequired[str],
    LicenseAcquisitionUrl: NotRequired[str],
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

## NotificationsTypeDef

```python
# NotificationsTypeDef definition

class NotificationsTypeDef(TypedDict):
    Progressing: NotRequired[str],
    Completed: NotRequired[str],
    Warning: NotRequired[str],
    Error: NotRequired[str],
```

## WarningTypeDef

```python
# WarningTypeDef definition

class WarningTypeDef(TypedDict):
    Code: NotRequired[str],
    Message: NotRequired[str],
```

## ThumbnailsTypeDef

```python
# ThumbnailsTypeDef definition

class ThumbnailsTypeDef(TypedDict):
    Format: NotRequired[str],
    Interval: NotRequired[str],
    Resolution: NotRequired[str],
    AspectRatio: NotRequired[str],
    MaxWidth: NotRequired[str],
    MaxHeight: NotRequired[str],
    SizingPolicy: NotRequired[str],
    PaddingPolicy: NotRequired[str],
```

## DeletePipelineRequestRequestTypeDef

```python
# DeletePipelineRequestRequestTypeDef definition

class DeletePipelineRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DeletePresetRequestRequestTypeDef

```python
# DeletePresetRequestRequestTypeDef definition

class DeletePresetRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DetectedPropertiesTypeDef

```python
# DetectedPropertiesTypeDef definition

class DetectedPropertiesTypeDef(TypedDict):
    Width: NotRequired[int],
    Height: NotRequired[int],
    FrameRate: NotRequired[str],
    FileSize: NotRequired[int],
    DurationMillis: NotRequired[int],
```

## TimingTypeDef

```python
# TimingTypeDef definition

class TimingTypeDef(TypedDict):
    SubmitTimeMillis: NotRequired[int],
    StartTimeMillis: NotRequired[int],
    FinishTimeMillis: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListJobsByPipelineRequestRequestTypeDef

```python
# ListJobsByPipelineRequestRequestTypeDef definition

class ListJobsByPipelineRequestRequestTypeDef(TypedDict):
    PipelineId: str,
    Ascending: NotRequired[str],
    PageToken: NotRequired[str],
```

## ListJobsByStatusRequestRequestTypeDef

```python
# ListJobsByStatusRequestRequestTypeDef definition

class ListJobsByStatusRequestRequestTypeDef(TypedDict):
    Status: str,
    Ascending: NotRequired[str],
    PageToken: NotRequired[str],
```

## ListPipelinesRequestRequestTypeDef

```python
# ListPipelinesRequestRequestTypeDef definition

class ListPipelinesRequestRequestTypeDef(TypedDict):
    Ascending: NotRequired[str],
    PageToken: NotRequired[str],
```

## ListPresetsRequestRequestTypeDef

```python
# ListPresetsRequestRequestTypeDef definition

class ListPresetsRequestRequestTypeDef(TypedDict):
    Ascending: NotRequired[str],
    PageToken: NotRequired[str],
```

## PermissionOutputTypeDef

```python
# PermissionOutputTypeDef definition

class PermissionOutputTypeDef(TypedDict):
    GranteeType: NotRequired[str],
    Grantee: NotRequired[str],
    Access: NotRequired[List[str]],
```

## PermissionTypeDef

```python
# PermissionTypeDef definition

class PermissionTypeDef(TypedDict):
    GranteeType: NotRequired[str],
    Grantee: NotRequired[str],
    Access: NotRequired[Sequence[str]],
```

## PresetWatermarkTypeDef

```python
# PresetWatermarkTypeDef definition

class PresetWatermarkTypeDef(TypedDict):
    Id: NotRequired[str],
    MaxWidth: NotRequired[str],
    MaxHeight: NotRequired[str],
    SizingPolicy: NotRequired[str],
    HorizontalAlign: NotRequired[str],
    HorizontalOffset: NotRequired[str],
    VerticalAlign: NotRequired[str],
    VerticalOffset: NotRequired[str],
    Opacity: NotRequired[str],
    Target: NotRequired[str],
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## ReadJobRequestRequestTypeDef

```python
# ReadJobRequestRequestTypeDef definition

class ReadJobRequestRequestTypeDef(TypedDict):
    Id: str,
```

## ReadPipelineRequestRequestTypeDef

```python
# ReadPipelineRequestRequestTypeDef definition

class ReadPipelineRequestRequestTypeDef(TypedDict):
    Id: str,
```

## ReadPresetRequestRequestTypeDef

```python
# ReadPresetRequestRequestTypeDef definition

class ReadPresetRequestRequestTypeDef(TypedDict):
    Id: str,
```

## TestRoleRequestRequestTypeDef

```python
# TestRoleRequestRequestTypeDef definition

class TestRoleRequestRequestTypeDef(TypedDict):
    Role: str,
    InputBucket: str,
    OutputBucket: str,
    Topics: Sequence[str],
```

## UpdatePipelineStatusRequestRequestTypeDef

```python
# UpdatePipelineStatusRequestRequestTypeDef definition

class UpdatePipelineStatusRequestRequestTypeDef(TypedDict):
    Id: str,
    Status: str,
```

## ArtworkTypeDef

```python
# ArtworkTypeDef definition

class ArtworkTypeDef(TypedDict):
    InputKey: NotRequired[str],
    MaxWidth: NotRequired[str],
    MaxHeight: NotRequired[str],
    SizingPolicy: NotRequired[str],
    PaddingPolicy: NotRequired[str],
    AlbumArtFormat: NotRequired[str],
    Encryption: NotRequired[EncryptionTypeDef],  # (1)
```

1. See [:material-code-braces: EncryptionTypeDef](./type_defs.md#encryptiontypedef) 
## CaptionFormatTypeDef

```python
# CaptionFormatTypeDef definition

class CaptionFormatTypeDef(TypedDict):
    Format: NotRequired[str],
    Pattern: NotRequired[str],
    Encryption: NotRequired[EncryptionTypeDef],  # (1)
```

1. See [:material-code-braces: EncryptionTypeDef](./type_defs.md#encryptiontypedef) 
## CaptionSourceTypeDef

```python
# CaptionSourceTypeDef definition

class CaptionSourceTypeDef(TypedDict):
    Key: NotRequired[str],
    Language: NotRequired[str],
    TimeOffset: NotRequired[str],
    Label: NotRequired[str],
    Encryption: NotRequired[EncryptionTypeDef],  # (1)
```

1. See [:material-code-braces: EncryptionTypeDef](./type_defs.md#encryptiontypedef) 
## JobWatermarkTypeDef

```python
# JobWatermarkTypeDef definition

class JobWatermarkTypeDef(TypedDict):
    PresetWatermarkId: NotRequired[str],
    InputKey: NotRequired[str],
    Encryption: NotRequired[EncryptionTypeDef],  # (1)
```

1. See [:material-code-braces: EncryptionTypeDef](./type_defs.md#encryptiontypedef) 
## AudioParametersTypeDef

```python
# AudioParametersTypeDef definition

class AudioParametersTypeDef(TypedDict):
    Codec: NotRequired[str],
    SampleRate: NotRequired[str],
    BitRate: NotRequired[str],
    Channels: NotRequired[str],
    AudioPackingMode: NotRequired[str],
    CodecOptions: NotRequired[AudioCodecOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: AudioCodecOptionsTypeDef](./type_defs.md#audiocodecoptionstypedef) 
## ClipTypeDef

```python
# ClipTypeDef definition

class ClipTypeDef(TypedDict):
    TimeSpan: NotRequired[TimeSpanTypeDef],  # (1)
```

1. See [:material-code-braces: TimeSpanTypeDef](./type_defs.md#timespantypedef) 
## CreateJobPlaylistTypeDef

```python
# CreateJobPlaylistTypeDef definition

class CreateJobPlaylistTypeDef(TypedDict):
    Name: NotRequired[str],
    Format: NotRequired[str],
    OutputKeys: NotRequired[Sequence[str]],
    HlsContentProtection: NotRequired[HlsContentProtectionTypeDef],  # (1)
    PlayReadyDrm: NotRequired[PlayReadyDrmTypeDef],  # (2)
```

1. See [:material-code-braces: HlsContentProtectionTypeDef](./type_defs.md#hlscontentprotectiontypedef) 
2. See [:material-code-braces: PlayReadyDrmTypeDef](./type_defs.md#playreadydrmtypedef) 
## PlaylistTypeDef

```python
# PlaylistTypeDef definition

class PlaylistTypeDef(TypedDict):
    Name: NotRequired[str],
    Format: NotRequired[str],
    OutputKeys: NotRequired[List[str]],
    HlsContentProtection: NotRequired[HlsContentProtectionTypeDef],  # (1)
    PlayReadyDrm: NotRequired[PlayReadyDrmTypeDef],  # (2)
    Status: NotRequired[str],
    StatusDetail: NotRequired[str],
```

1. See [:material-code-braces: HlsContentProtectionTypeDef](./type_defs.md#hlscontentprotectiontypedef) 
2. See [:material-code-braces: PlayReadyDrmTypeDef](./type_defs.md#playreadydrmtypedef) 
## TestRoleResponseTypeDef

```python
# TestRoleResponseTypeDef definition

class TestRoleResponseTypeDef(TypedDict):
    Success: str,
    Messages: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePipelineNotificationsRequestRequestTypeDef

```python
# UpdatePipelineNotificationsRequestRequestTypeDef definition

class UpdatePipelineNotificationsRequestRequestTypeDef(TypedDict):
    Id: str,
    Notifications: NotificationsTypeDef,  # (1)
```

1. See [:material-code-braces: NotificationsTypeDef](./type_defs.md#notificationstypedef) 
## ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef

```python
# ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef definition

class ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef(TypedDict):
    PipelineId: str,
    Ascending: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobsByStatusRequestListJobsByStatusPaginateTypeDef

```python
# ListJobsByStatusRequestListJobsByStatusPaginateTypeDef definition

class ListJobsByStatusRequestListJobsByStatusPaginateTypeDef(TypedDict):
    Status: str,
    Ascending: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPipelinesRequestListPipelinesPaginateTypeDef

```python
# ListPipelinesRequestListPipelinesPaginateTypeDef definition

class ListPipelinesRequestListPipelinesPaginateTypeDef(TypedDict):
    Ascending: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPresetsRequestListPresetsPaginateTypeDef

```python
# ListPresetsRequestListPresetsPaginateTypeDef definition

class ListPresetsRequestListPresetsPaginateTypeDef(TypedDict):
    Ascending: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## PipelineOutputConfigOutputTypeDef

```python
# PipelineOutputConfigOutputTypeDef definition

class PipelineOutputConfigOutputTypeDef(TypedDict):
    Bucket: NotRequired[str],
    StorageClass: NotRequired[str],
    Permissions: NotRequired[List[PermissionOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: PermissionOutputTypeDef](./type_defs.md#permissionoutputtypedef) 
## VideoParametersOutputTypeDef

```python
# VideoParametersOutputTypeDef definition

class VideoParametersOutputTypeDef(TypedDict):
    Codec: NotRequired[str],
    CodecOptions: NotRequired[Dict[str, str]],
    KeyframesMaxDist: NotRequired[str],
    FixedGOP: NotRequired[str],
    BitRate: NotRequired[str],
    FrameRate: NotRequired[str],
    MaxFrameRate: NotRequired[str],
    Resolution: NotRequired[str],
    AspectRatio: NotRequired[str],
    MaxWidth: NotRequired[str],
    MaxHeight: NotRequired[str],
    DisplayAspectRatio: NotRequired[str],
    SizingPolicy: NotRequired[str],
    PaddingPolicy: NotRequired[str],
    Watermarks: NotRequired[List[PresetWatermarkTypeDef]],  # (1)
```

1. See [:material-code-braces: PresetWatermarkTypeDef](./type_defs.md#presetwatermarktypedef) 
## VideoParametersTypeDef

```python
# VideoParametersTypeDef definition

class VideoParametersTypeDef(TypedDict):
    Codec: NotRequired[str],
    CodecOptions: NotRequired[Mapping[str, str]],
    KeyframesMaxDist: NotRequired[str],
    FixedGOP: NotRequired[str],
    BitRate: NotRequired[str],
    FrameRate: NotRequired[str],
    MaxFrameRate: NotRequired[str],
    Resolution: NotRequired[str],
    AspectRatio: NotRequired[str],
    MaxWidth: NotRequired[str],
    MaxHeight: NotRequired[str],
    DisplayAspectRatio: NotRequired[str],
    SizingPolicy: NotRequired[str],
    PaddingPolicy: NotRequired[str],
    Watermarks: NotRequired[Sequence[PresetWatermarkTypeDef]],  # (1)
```

1. See [:material-code-braces: PresetWatermarkTypeDef](./type_defs.md#presetwatermarktypedef) 
## ReadJobRequestJobCompleteWaitTypeDef

```python
# ReadJobRequestJobCompleteWaitTypeDef definition

class ReadJobRequestJobCompleteWaitTypeDef(TypedDict):
    Id: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## JobAlbumArtOutputTypeDef

```python
# JobAlbumArtOutputTypeDef definition

class JobAlbumArtOutputTypeDef(TypedDict):
    MergePolicy: NotRequired[str],
    Artwork: NotRequired[List[ArtworkTypeDef]],  # (1)
```

1. See [:material-code-braces: ArtworkTypeDef](./type_defs.md#artworktypedef) 
## JobAlbumArtTypeDef

```python
# JobAlbumArtTypeDef definition

class JobAlbumArtTypeDef(TypedDict):
    MergePolicy: NotRequired[str],
    Artwork: NotRequired[Sequence[ArtworkTypeDef]],  # (1)
```

1. See [:material-code-braces: ArtworkTypeDef](./type_defs.md#artworktypedef) 
## CaptionsOutputTypeDef

```python
# CaptionsOutputTypeDef definition

class CaptionsOutputTypeDef(TypedDict):
    MergePolicy: NotRequired[str],
    CaptionSources: NotRequired[List[CaptionSourceTypeDef]],  # (1)
    CaptionFormats: NotRequired[List[CaptionFormatTypeDef]],  # (2)
```

1. See [:material-code-braces: CaptionSourceTypeDef](./type_defs.md#captionsourcetypedef) 
2. See [:material-code-braces: CaptionFormatTypeDef](./type_defs.md#captionformattypedef) 
## CaptionsTypeDef

```python
# CaptionsTypeDef definition

class CaptionsTypeDef(TypedDict):
    MergePolicy: NotRequired[str],
    CaptionSources: NotRequired[Sequence[CaptionSourceTypeDef]],  # (1)
    CaptionFormats: NotRequired[Sequence[CaptionFormatTypeDef]],  # (2)
```

1. See [:material-code-braces: CaptionSourceTypeDef](./type_defs.md#captionsourcetypedef) 
2. See [:material-code-braces: CaptionFormatTypeDef](./type_defs.md#captionformattypedef) 
## InputCaptionsOutputTypeDef

```python
# InputCaptionsOutputTypeDef definition

class InputCaptionsOutputTypeDef(TypedDict):
    MergePolicy: NotRequired[str],
    CaptionSources: NotRequired[List[CaptionSourceTypeDef]],  # (1)
```

1. See [:material-code-braces: CaptionSourceTypeDef](./type_defs.md#captionsourcetypedef) 
## InputCaptionsTypeDef

```python
# InputCaptionsTypeDef definition

class InputCaptionsTypeDef(TypedDict):
    MergePolicy: NotRequired[str],
    CaptionSources: NotRequired[Sequence[CaptionSourceTypeDef]],  # (1)
```

1. See [:material-code-braces: CaptionSourceTypeDef](./type_defs.md#captionsourcetypedef) 
## PipelineTypeDef

```python
# PipelineTypeDef definition

class PipelineTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[str],
    InputBucket: NotRequired[str],
    OutputBucket: NotRequired[str],
    Role: NotRequired[str],
    AwsKmsKeyArn: NotRequired[str],
    Notifications: NotRequired[NotificationsTypeDef],  # (1)
    ContentConfig: NotRequired[PipelineOutputConfigOutputTypeDef],  # (2)
    ThumbnailConfig: NotRequired[PipelineOutputConfigOutputTypeDef],  # (2)
```

1. See [:material-code-braces: NotificationsTypeDef](./type_defs.md#notificationstypedef) 
2. See [:material-code-braces: PipelineOutputConfigOutputTypeDef](./type_defs.md#pipelineoutputconfigoutputtypedef) 
3. See [:material-code-braces: PipelineOutputConfigOutputTypeDef](./type_defs.md#pipelineoutputconfigoutputtypedef) 
## PipelineOutputConfigTypeDef

```python
# PipelineOutputConfigTypeDef definition

class PipelineOutputConfigTypeDef(TypedDict):
    Bucket: NotRequired[str],
    StorageClass: NotRequired[str],
    Permissions: NotRequired[Sequence[PermissionUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: PermissionTypeDef](./type_defs.md#permissiontypedef) [:material-code-braces: PermissionOutputTypeDef](./type_defs.md#permissionoutputtypedef) 
## PresetTypeDef

```python
# PresetTypeDef definition

class PresetTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    Container: NotRequired[str],
    Audio: NotRequired[AudioParametersTypeDef],  # (1)
    Video: NotRequired[VideoParametersOutputTypeDef],  # (2)
    Thumbnails: NotRequired[ThumbnailsTypeDef],  # (3)
    Type: NotRequired[str],
```

1. See [:material-code-braces: AudioParametersTypeDef](./type_defs.md#audioparameterstypedef) 
2. See [:material-code-braces: VideoParametersOutputTypeDef](./type_defs.md#videoparametersoutputtypedef) 
3. See [:material-code-braces: ThumbnailsTypeDef](./type_defs.md#thumbnailstypedef) 
## CreatePresetRequestRequestTypeDef

```python
# CreatePresetRequestRequestTypeDef definition

class CreatePresetRequestRequestTypeDef(TypedDict):
    Name: str,
    Container: str,
    Description: NotRequired[str],
    Video: NotRequired[VideoParametersTypeDef],  # (1)
    Audio: NotRequired[AudioParametersTypeDef],  # (2)
    Thumbnails: NotRequired[ThumbnailsTypeDef],  # (3)
```

1. See [:material-code-braces: VideoParametersTypeDef](./type_defs.md#videoparameterstypedef) 
2. See [:material-code-braces: AudioParametersTypeDef](./type_defs.md#audioparameterstypedef) 
3. See [:material-code-braces: ThumbnailsTypeDef](./type_defs.md#thumbnailstypedef) 
## JobOutputTypeDef

```python
# JobOutputTypeDef definition

class JobOutputTypeDef(TypedDict):
    Id: NotRequired[str],
    Key: NotRequired[str],
    ThumbnailPattern: NotRequired[str],
    ThumbnailEncryption: NotRequired[EncryptionTypeDef],  # (1)
    Rotate: NotRequired[str],
    PresetId: NotRequired[str],
    SegmentDuration: NotRequired[str],
    Status: NotRequired[str],
    StatusDetail: NotRequired[str],
    Duration: NotRequired[int],
    Width: NotRequired[int],
    Height: NotRequired[int],
    FrameRate: NotRequired[str],
    FileSize: NotRequired[int],
    DurationMillis: NotRequired[int],
    Watermarks: NotRequired[List[JobWatermarkTypeDef]],  # (2)
    AlbumArt: NotRequired[JobAlbumArtOutputTypeDef],  # (3)
    Composition: NotRequired[List[ClipTypeDef]],  # (4)
    Captions: NotRequired[CaptionsOutputTypeDef],  # (5)
    Encryption: NotRequired[EncryptionTypeDef],  # (1)
    AppliedColorSpaceConversion: NotRequired[str],
```

1. See [:material-code-braces: EncryptionTypeDef](./type_defs.md#encryptiontypedef) 
2. See [:material-code-braces: JobWatermarkTypeDef](./type_defs.md#jobwatermarktypedef) 
3. See [:material-code-braces: JobAlbumArtOutputTypeDef](./type_defs.md#jobalbumartoutputtypedef) 
4. See [:material-code-braces: ClipTypeDef](./type_defs.md#cliptypedef) 
5. See [:material-code-braces: CaptionsOutputTypeDef](./type_defs.md#captionsoutputtypedef) 
6. See [:material-code-braces: EncryptionTypeDef](./type_defs.md#encryptiontypedef) 
## JobInputOutputTypeDef

```python
# JobInputOutputTypeDef definition

class JobInputOutputTypeDef(TypedDict):
    Key: NotRequired[str],
    FrameRate: NotRequired[str],
    Resolution: NotRequired[str],
    AspectRatio: NotRequired[str],
    Interlaced: NotRequired[str],
    Container: NotRequired[str],
    Encryption: NotRequired[EncryptionTypeDef],  # (1)
    TimeSpan: NotRequired[TimeSpanTypeDef],  # (2)
    InputCaptions: NotRequired[InputCaptionsOutputTypeDef],  # (3)
    DetectedProperties: NotRequired[DetectedPropertiesTypeDef],  # (4)
```

1. See [:material-code-braces: EncryptionTypeDef](./type_defs.md#encryptiontypedef) 
2. See [:material-code-braces: TimeSpanTypeDef](./type_defs.md#timespantypedef) 
3. See [:material-code-braces: InputCaptionsOutputTypeDef](./type_defs.md#inputcaptionsoutputtypedef) 
4. See [:material-code-braces: DetectedPropertiesTypeDef](./type_defs.md#detectedpropertiestypedef) 
## CreatePipelineResponseTypeDef

```python
# CreatePipelineResponseTypeDef definition

class CreatePipelineResponseTypeDef(TypedDict):
    Pipeline: PipelineTypeDef,  # (1)
    Warnings: List[WarningTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PipelineTypeDef](./type_defs.md#pipelinetypedef) 
2. See [:material-code-braces: WarningTypeDef](./type_defs.md#warningtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPipelinesResponseTypeDef

```python
# ListPipelinesResponseTypeDef definition

class ListPipelinesResponseTypeDef(TypedDict):
    Pipelines: List[PipelineTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineTypeDef](./type_defs.md#pipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReadPipelineResponseTypeDef

```python
# ReadPipelineResponseTypeDef definition

class ReadPipelineResponseTypeDef(TypedDict):
    Pipeline: PipelineTypeDef,  # (1)
    Warnings: List[WarningTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PipelineTypeDef](./type_defs.md#pipelinetypedef) 
2. See [:material-code-braces: WarningTypeDef](./type_defs.md#warningtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePipelineNotificationsResponseTypeDef

```python
# UpdatePipelineNotificationsResponseTypeDef definition

class UpdatePipelineNotificationsResponseTypeDef(TypedDict):
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
    Warnings: List[WarningTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PipelineTypeDef](./type_defs.md#pipelinetypedef) 
2. See [:material-code-braces: WarningTypeDef](./type_defs.md#warningtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePipelineStatusResponseTypeDef

```python
# UpdatePipelineStatusResponseTypeDef definition

class UpdatePipelineStatusResponseTypeDef(TypedDict):
    Pipeline: PipelineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineTypeDef](./type_defs.md#pipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePipelineRequestRequestTypeDef

```python
# CreatePipelineRequestRequestTypeDef definition

class CreatePipelineRequestRequestTypeDef(TypedDict):
    Name: str,
    InputBucket: str,
    Role: str,
    OutputBucket: NotRequired[str],
    AwsKmsKeyArn: NotRequired[str],
    Notifications: NotRequired[NotificationsTypeDef],  # (1)
    ContentConfig: NotRequired[PipelineOutputConfigTypeDef],  # (2)
    ThumbnailConfig: NotRequired[PipelineOutputConfigTypeDef],  # (2)
```

1. See [:material-code-braces: NotificationsTypeDef](./type_defs.md#notificationstypedef) 
2. See [:material-code-braces: PipelineOutputConfigTypeDef](./type_defs.md#pipelineoutputconfigtypedef) 
3. See [:material-code-braces: PipelineOutputConfigTypeDef](./type_defs.md#pipelineoutputconfigtypedef) 
## UpdatePipelineRequestRequestTypeDef

```python
# UpdatePipelineRequestRequestTypeDef definition

class UpdatePipelineRequestRequestTypeDef(TypedDict):
    Id: str,
    Name: NotRequired[str],
    InputBucket: NotRequired[str],
    Role: NotRequired[str],
    AwsKmsKeyArn: NotRequired[str],
    Notifications: NotRequired[NotificationsTypeDef],  # (1)
    ContentConfig: NotRequired[PipelineOutputConfigTypeDef],  # (2)
    ThumbnailConfig: NotRequired[PipelineOutputConfigTypeDef],  # (2)
```

1. See [:material-code-braces: NotificationsTypeDef](./type_defs.md#notificationstypedef) 
2. See [:material-code-braces: PipelineOutputConfigTypeDef](./type_defs.md#pipelineoutputconfigtypedef) 
3. See [:material-code-braces: PipelineOutputConfigTypeDef](./type_defs.md#pipelineoutputconfigtypedef) 
## CreatePresetResponseTypeDef

```python
# CreatePresetResponseTypeDef definition

class CreatePresetResponseTypeDef(TypedDict):
    Preset: PresetTypeDef,  # (1)
    Warning: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PresetTypeDef](./type_defs.md#presettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPresetsResponseTypeDef

```python
# ListPresetsResponseTypeDef definition

class ListPresetsResponseTypeDef(TypedDict):
    Presets: List[PresetTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PresetTypeDef](./type_defs.md#presettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReadPresetResponseTypeDef

```python
# ReadPresetResponseTypeDef definition

class ReadPresetResponseTypeDef(TypedDict):
    Preset: PresetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PresetTypeDef](./type_defs.md#presettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobOutputTypeDef

```python
# CreateJobOutputTypeDef definition

class CreateJobOutputTypeDef(TypedDict):
    Key: NotRequired[str],
    ThumbnailPattern: NotRequired[str],
    ThumbnailEncryption: NotRequired[EncryptionTypeDef],  # (1)
    Rotate: NotRequired[str],
    PresetId: NotRequired[str],
    SegmentDuration: NotRequired[str],
    Watermarks: NotRequired[Sequence[JobWatermarkTypeDef]],  # (2)
    AlbumArt: NotRequired[JobAlbumArtUnionTypeDef],  # (3)
    Composition: NotRequired[Sequence[ClipTypeDef]],  # (4)
    Captions: NotRequired[CaptionsUnionTypeDef],  # (5)
    Encryption: NotRequired[EncryptionTypeDef],  # (1)
```

1. See [:material-code-braces: EncryptionTypeDef](./type_defs.md#encryptiontypedef) 
2. See [:material-code-braces: JobWatermarkTypeDef](./type_defs.md#jobwatermarktypedef) 
3. See [:material-code-braces: JobAlbumArtTypeDef](./type_defs.md#jobalbumarttypedef) [:material-code-braces: JobAlbumArtOutputTypeDef](./type_defs.md#jobalbumartoutputtypedef) 
4. See [:material-code-braces: ClipTypeDef](./type_defs.md#cliptypedef) 
5. See [:material-code-braces: CaptionsTypeDef](./type_defs.md#captionstypedef) [:material-code-braces: CaptionsOutputTypeDef](./type_defs.md#captionsoutputtypedef) 
6. See [:material-code-braces: EncryptionTypeDef](./type_defs.md#encryptiontypedef) 
## JobTypeDef

```python
# JobTypeDef definition

class JobTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    PipelineId: NotRequired[str],
    Input: NotRequired[JobInputOutputTypeDef],  # (1)
    Inputs: NotRequired[List[JobInputOutputTypeDef]],  # (2)
    Output: NotRequired[JobOutputTypeDef],  # (3)
    Outputs: NotRequired[List[JobOutputTypeDef]],  # (4)
    OutputKeyPrefix: NotRequired[str],
    Playlists: NotRequired[List[PlaylistTypeDef]],  # (5)
    Status: NotRequired[str],
    UserMetadata: NotRequired[Dict[str, str]],
    Timing: NotRequired[TimingTypeDef],  # (6)
```

1. See [:material-code-braces: JobInputOutputTypeDef](./type_defs.md#jobinputoutputtypedef) 
2. See [:material-code-braces: JobInputOutputTypeDef](./type_defs.md#jobinputoutputtypedef) 
3. See [:material-code-braces: JobOutputTypeDef](./type_defs.md#joboutputtypedef) 
4. See [:material-code-braces: JobOutputTypeDef](./type_defs.md#joboutputtypedef) 
5. See [:material-code-braces: PlaylistTypeDef](./type_defs.md#playlisttypedef) 
6. See [:material-code-braces: TimingTypeDef](./type_defs.md#timingtypedef) 
## JobInputTypeDef

```python
# JobInputTypeDef definition

class JobInputTypeDef(TypedDict):
    Key: NotRequired[str],
    FrameRate: NotRequired[str],
    Resolution: NotRequired[str],
    AspectRatio: NotRequired[str],
    Interlaced: NotRequired[str],
    Container: NotRequired[str],
    Encryption: NotRequired[EncryptionTypeDef],  # (1)
    TimeSpan: NotRequired[TimeSpanTypeDef],  # (2)
    InputCaptions: NotRequired[InputCaptionsUnionTypeDef],  # (3)
    DetectedProperties: NotRequired[DetectedPropertiesTypeDef],  # (4)
```

1. See [:material-code-braces: EncryptionTypeDef](./type_defs.md#encryptiontypedef) 
2. See [:material-code-braces: TimeSpanTypeDef](./type_defs.md#timespantypedef) 
3. See [:material-code-braces: InputCaptionsTypeDef](./type_defs.md#inputcaptionstypedef) [:material-code-braces: InputCaptionsOutputTypeDef](./type_defs.md#inputcaptionsoutputtypedef) 
4. See [:material-code-braces: DetectedPropertiesTypeDef](./type_defs.md#detectedpropertiestypedef) 
## CreateJobResponseTypeDef

```python
# CreateJobResponseTypeDef definition

class CreateJobResponseTypeDef(TypedDict):
    Job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJobsByPipelineResponseTypeDef

```python
# ListJobsByPipelineResponseTypeDef definition

class ListJobsByPipelineResponseTypeDef(TypedDict):
    Jobs: List[JobTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJobsByStatusResponseTypeDef

```python
# ListJobsByStatusResponseTypeDef definition

class ListJobsByStatusResponseTypeDef(TypedDict):
    Jobs: List[JobTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReadJobResponseTypeDef

```python
# ReadJobResponseTypeDef definition

class ReadJobResponseTypeDef(TypedDict):
    Job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobRequestRequestTypeDef

```python
# CreateJobRequestRequestTypeDef definition

class CreateJobRequestRequestTypeDef(TypedDict):
    PipelineId: str,
    Input: NotRequired[JobInputTypeDef],  # (1)
    Inputs: NotRequired[Sequence[JobInputUnionTypeDef]],  # (2)
    Output: NotRequired[CreateJobOutputTypeDef],  # (3)
    Outputs: NotRequired[Sequence[CreateJobOutputTypeDef]],  # (4)
    OutputKeyPrefix: NotRequired[str],
    Playlists: NotRequired[Sequence[CreateJobPlaylistTypeDef]],  # (5)
    UserMetadata: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: JobInputTypeDef](./type_defs.md#jobinputtypedef) 
2. See [:material-code-braces: JobInputTypeDef](./type_defs.md#jobinputtypedef) [:material-code-braces: JobInputOutputTypeDef](./type_defs.md#jobinputoutputtypedef) 
3. See [:material-code-braces: CreateJobOutputTypeDef](./type_defs.md#createjoboutputtypedef) 
4. See [:material-code-braces: CreateJobOutputTypeDef](./type_defs.md#createjoboutputtypedef) 
5. See [:material-code-braces: CreateJobPlaylistTypeDef](./type_defs.md#createjobplaylisttypedef) 
