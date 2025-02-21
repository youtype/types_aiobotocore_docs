# Type definitions

> [Index](../README.md) > [ElasticTranscoder](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ElasticTranscoder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#elastictranscoder)
    type annotations stubs module [types-aiobotocore-elastictranscoder](https://pypi.org/project/types-aiobotocore-elastictranscoder/).

## PipelineOutputConfigUnionTypeDef

```python
# PipelineOutputConfigUnionTypeDef Union usage example

from types_aiobotocore_elastictranscoder.type_defs import PipelineOutputConfigUnionTypeDef


def get_value() -> PipelineOutputConfigUnionTypeDef:
    return ...


# PipelineOutputConfigUnionTypeDef definition

PipelineOutputConfigUnionTypeDef = Union[
    PipelineOutputConfigTypeDef,  # (1)
    PipelineOutputConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PipelineOutputConfigTypeDef](./type_defs.md#pipelineoutputconfigtypedef) 
2. See [:material-code-braces: PipelineOutputConfigOutputTypeDef](./type_defs.md#pipelineoutputconfigoutputtypedef) 

## VideoParametersUnionTypeDef

```python
# VideoParametersUnionTypeDef Union usage example

from types_aiobotocore_elastictranscoder.type_defs import VideoParametersUnionTypeDef


def get_value() -> VideoParametersUnionTypeDef:
    return ...


# VideoParametersUnionTypeDef definition

VideoParametersUnionTypeDef = Union[
    VideoParametersTypeDef,  # (1)
    VideoParametersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: VideoParametersTypeDef](./type_defs.md#videoparameterstypedef) 
2. See [:material-code-braces: VideoParametersOutputTypeDef](./type_defs.md#videoparametersoutputtypedef) 

## JobAlbumArtUnionTypeDef

```python
# JobAlbumArtUnionTypeDef Union usage example

from types_aiobotocore_elastictranscoder.type_defs import JobAlbumArtUnionTypeDef


def get_value() -> JobAlbumArtUnionTypeDef:
    return ...


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
# CaptionsUnionTypeDef Union usage example

from types_aiobotocore_elastictranscoder.type_defs import CaptionsUnionTypeDef


def get_value() -> CaptionsUnionTypeDef:
    return ...


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
# InputCaptionsUnionTypeDef Union usage example

from types_aiobotocore_elastictranscoder.type_defs import InputCaptionsUnionTypeDef


def get_value() -> InputCaptionsUnionTypeDef:
    return ...


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
# JobInputUnionTypeDef Union usage example

from types_aiobotocore_elastictranscoder.type_defs import JobInputUnionTypeDef


def get_value() -> JobInputUnionTypeDef:
    return ...


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
# EncryptionTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import EncryptionTypeDef


def get_value() -> EncryptionTypeDef:
    return {
        "Mode": ...,
    }


# EncryptionTypeDef definition

class EncryptionTypeDef(TypedDict):
    Mode: NotRequired[str],
    Key: NotRequired[str],
    KeyMd5: NotRequired[str],
    InitializationVector: NotRequired[str],
```

## AudioCodecOptionsTypeDef

```python
# AudioCodecOptionsTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import AudioCodecOptionsTypeDef


def get_value() -> AudioCodecOptionsTypeDef:
    return {
        "Profile": ...,
    }


# AudioCodecOptionsTypeDef definition

class AudioCodecOptionsTypeDef(TypedDict):
    Profile: NotRequired[str],
    BitDepth: NotRequired[str],
    BitOrder: NotRequired[str],
    Signed: NotRequired[str],
```

## CancelJobRequestTypeDef

```python
# CancelJobRequestTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import CancelJobRequestTypeDef


def get_value() -> CancelJobRequestTypeDef:
    return {
        "Id": ...,
    }


# CancelJobRequestTypeDef definition

class CancelJobRequestTypeDef(TypedDict):
    Id: str,
```

## TimeSpanTypeDef

```python
# TimeSpanTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import TimeSpanTypeDef


def get_value() -> TimeSpanTypeDef:
    return {
        "StartTime": ...,
    }


# TimeSpanTypeDef definition

class TimeSpanTypeDef(TypedDict):
    StartTime: NotRequired[str],
    Duration: NotRequired[str],
```

## HlsContentProtectionTypeDef

```python
# HlsContentProtectionTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import HlsContentProtectionTypeDef


def get_value() -> HlsContentProtectionTypeDef:
    return {
        "Method": ...,
    }


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
# PlayReadyDrmTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import PlayReadyDrmTypeDef


def get_value() -> PlayReadyDrmTypeDef:
    return {
        "Format": ...,
    }


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
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ResponseMetadataTypeDef


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

## NotificationsTypeDef

```python
# NotificationsTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import NotificationsTypeDef


def get_value() -> NotificationsTypeDef:
    return {
        "Progressing": ...,
    }


# NotificationsTypeDef definition

class NotificationsTypeDef(TypedDict):
    Progressing: NotRequired[str],
    Completed: NotRequired[str],
    Warning: NotRequired[str],
    Error: NotRequired[str],
```

## WarningTypeDef

```python
# WarningTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import WarningTypeDef


def get_value() -> WarningTypeDef:
    return {
        "Code": ...,
    }


# WarningTypeDef definition

class WarningTypeDef(TypedDict):
    Code: NotRequired[str],
    Message: NotRequired[str],
```

## ThumbnailsTypeDef

```python
# ThumbnailsTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ThumbnailsTypeDef


def get_value() -> ThumbnailsTypeDef:
    return {
        "Format": ...,
    }


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

## DeletePipelineRequestTypeDef

```python
# DeletePipelineRequestTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import DeletePipelineRequestTypeDef


def get_value() -> DeletePipelineRequestTypeDef:
    return {
        "Id": ...,
    }


# DeletePipelineRequestTypeDef definition

class DeletePipelineRequestTypeDef(TypedDict):
    Id: str,
```

## DeletePresetRequestTypeDef

```python
# DeletePresetRequestTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import DeletePresetRequestTypeDef


def get_value() -> DeletePresetRequestTypeDef:
    return {
        "Id": ...,
    }


# DeletePresetRequestTypeDef definition

class DeletePresetRequestTypeDef(TypedDict):
    Id: str,
```

## DetectedPropertiesTypeDef

```python
# DetectedPropertiesTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import DetectedPropertiesTypeDef


def get_value() -> DetectedPropertiesTypeDef:
    return {
        "Width": ...,
    }


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
# TimingTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import TimingTypeDef


def get_value() -> TimingTypeDef:
    return {
        "SubmitTimeMillis": ...,
    }


# TimingTypeDef definition

class TimingTypeDef(TypedDict):
    SubmitTimeMillis: NotRequired[int],
    StartTimeMillis: NotRequired[int],
    FinishTimeMillis: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import PaginatorConfigTypeDef


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

## ListJobsByPipelineRequestTypeDef

```python
# ListJobsByPipelineRequestTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ListJobsByPipelineRequestTypeDef


def get_value() -> ListJobsByPipelineRequestTypeDef:
    return {
        "PipelineId": ...,
    }


# ListJobsByPipelineRequestTypeDef definition

class ListJobsByPipelineRequestTypeDef(TypedDict):
    PipelineId: str,
    Ascending: NotRequired[str],
    PageToken: NotRequired[str],
```

## ListJobsByStatusRequestTypeDef

```python
# ListJobsByStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ListJobsByStatusRequestTypeDef


def get_value() -> ListJobsByStatusRequestTypeDef:
    return {
        "Status": ...,
    }


# ListJobsByStatusRequestTypeDef definition

class ListJobsByStatusRequestTypeDef(TypedDict):
    Status: str,
    Ascending: NotRequired[str],
    PageToken: NotRequired[str],
```

## ListPipelinesRequestTypeDef

```python
# ListPipelinesRequestTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ListPipelinesRequestTypeDef


def get_value() -> ListPipelinesRequestTypeDef:
    return {
        "Ascending": ...,
    }


# ListPipelinesRequestTypeDef definition

class ListPipelinesRequestTypeDef(TypedDict):
    Ascending: NotRequired[str],
    PageToken: NotRequired[str],
```

## ListPresetsRequestTypeDef

```python
# ListPresetsRequestTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ListPresetsRequestTypeDef


def get_value() -> ListPresetsRequestTypeDef:
    return {
        "Ascending": ...,
    }


# ListPresetsRequestTypeDef definition

class ListPresetsRequestTypeDef(TypedDict):
    Ascending: NotRequired[str],
    PageToken: NotRequired[str],
```

## PermissionOutputTypeDef

```python
# PermissionOutputTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import PermissionOutputTypeDef


def get_value() -> PermissionOutputTypeDef:
    return {
        "GranteeType": ...,
    }


# PermissionOutputTypeDef definition

class PermissionOutputTypeDef(TypedDict):
    GranteeType: NotRequired[str],
    Grantee: NotRequired[str],
    Access: NotRequired[List[str]],
```

## PermissionTypeDef

```python
# PermissionTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import PermissionTypeDef


def get_value() -> PermissionTypeDef:
    return {
        "GranteeType": ...,
    }


# PermissionTypeDef definition

class PermissionTypeDef(TypedDict):
    GranteeType: NotRequired[str],
    Grantee: NotRequired[str],
    Access: NotRequired[Sequence[str]],
```

## PresetWatermarkTypeDef

```python
# PresetWatermarkTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import PresetWatermarkTypeDef


def get_value() -> PresetWatermarkTypeDef:
    return {
        "Id": ...,
    }


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

## ReadJobRequestTypeDef

```python
# ReadJobRequestTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ReadJobRequestTypeDef


def get_value() -> ReadJobRequestTypeDef:
    return {
        "Id": ...,
    }


# ReadJobRequestTypeDef definition

class ReadJobRequestTypeDef(TypedDict):
    Id: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import WaiterConfigTypeDef


def get_value() -> WaiterConfigTypeDef:
    return {
        "Delay": ...,
    }


# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## ReadPipelineRequestTypeDef

```python
# ReadPipelineRequestTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ReadPipelineRequestTypeDef


def get_value() -> ReadPipelineRequestTypeDef:
    return {
        "Id": ...,
    }


# ReadPipelineRequestTypeDef definition

class ReadPipelineRequestTypeDef(TypedDict):
    Id: str,
```

## ReadPresetRequestTypeDef

```python
# ReadPresetRequestTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ReadPresetRequestTypeDef


def get_value() -> ReadPresetRequestTypeDef:
    return {
        "Id": ...,
    }


# ReadPresetRequestTypeDef definition

class ReadPresetRequestTypeDef(TypedDict):
    Id: str,
```

## TestRoleRequestTypeDef

```python
# TestRoleRequestTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import TestRoleRequestTypeDef


def get_value() -> TestRoleRequestTypeDef:
    return {
        "Role": ...,
    }


# TestRoleRequestTypeDef definition

class TestRoleRequestTypeDef(TypedDict):
    Role: str,
    InputBucket: str,
    OutputBucket: str,
    Topics: Sequence[str],
```

## UpdatePipelineStatusRequestTypeDef

```python
# UpdatePipelineStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import UpdatePipelineStatusRequestTypeDef


def get_value() -> UpdatePipelineStatusRequestTypeDef:
    return {
        "Id": ...,
    }


# UpdatePipelineStatusRequestTypeDef definition

class UpdatePipelineStatusRequestTypeDef(TypedDict):
    Id: str,
    Status: str,
```

## ArtworkTypeDef

```python
# ArtworkTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ArtworkTypeDef


def get_value() -> ArtworkTypeDef:
    return {
        "InputKey": ...,
    }


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
# CaptionFormatTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import CaptionFormatTypeDef


def get_value() -> CaptionFormatTypeDef:
    return {
        "Format": ...,
    }


# CaptionFormatTypeDef definition

class CaptionFormatTypeDef(TypedDict):
    Format: NotRequired[str],
    Pattern: NotRequired[str],
    Encryption: NotRequired[EncryptionTypeDef],  # (1)
```

1. See [:material-code-braces: EncryptionTypeDef](./type_defs.md#encryptiontypedef) 
## CaptionSourceTypeDef

```python
# CaptionSourceTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import CaptionSourceTypeDef


def get_value() -> CaptionSourceTypeDef:
    return {
        "Key": ...,
    }


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
# JobWatermarkTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import JobWatermarkTypeDef


def get_value() -> JobWatermarkTypeDef:
    return {
        "PresetWatermarkId": ...,
    }


# JobWatermarkTypeDef definition

class JobWatermarkTypeDef(TypedDict):
    PresetWatermarkId: NotRequired[str],
    InputKey: NotRequired[str],
    Encryption: NotRequired[EncryptionTypeDef],  # (1)
```

1. See [:material-code-braces: EncryptionTypeDef](./type_defs.md#encryptiontypedef) 
## AudioParametersTypeDef

```python
# AudioParametersTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import AudioParametersTypeDef


def get_value() -> AudioParametersTypeDef:
    return {
        "Codec": ...,
    }


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
# ClipTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ClipTypeDef


def get_value() -> ClipTypeDef:
    return {
        "TimeSpan": ...,
    }


# ClipTypeDef definition

class ClipTypeDef(TypedDict):
    TimeSpan: NotRequired[TimeSpanTypeDef],  # (1)
```

1. See [:material-code-braces: TimeSpanTypeDef](./type_defs.md#timespantypedef) 
## CreateJobPlaylistTypeDef

```python
# CreateJobPlaylistTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import CreateJobPlaylistTypeDef


def get_value() -> CreateJobPlaylistTypeDef:
    return {
        "Name": ...,
    }


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
# PlaylistTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import PlaylistTypeDef


def get_value() -> PlaylistTypeDef:
    return {
        "Name": ...,
    }


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
# TestRoleResponseTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import TestRoleResponseTypeDef


def get_value() -> TestRoleResponseTypeDef:
    return {
        "Success": ...,
    }


# TestRoleResponseTypeDef definition

class TestRoleResponseTypeDef(TypedDict):
    Success: str,
    Messages: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePipelineNotificationsRequestTypeDef

```python
# UpdatePipelineNotificationsRequestTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import UpdatePipelineNotificationsRequestTypeDef


def get_value() -> UpdatePipelineNotificationsRequestTypeDef:
    return {
        "Id": ...,
    }


# UpdatePipelineNotificationsRequestTypeDef definition

class UpdatePipelineNotificationsRequestTypeDef(TypedDict):
    Id: str,
    Notifications: NotificationsTypeDef,  # (1)
```

1. See [:material-code-braces: NotificationsTypeDef](./type_defs.md#notificationstypedef) 
## ListJobsByPipelineRequestPaginateTypeDef

```python
# ListJobsByPipelineRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ListJobsByPipelineRequestPaginateTypeDef


def get_value() -> ListJobsByPipelineRequestPaginateTypeDef:
    return {
        "PipelineId": ...,
    }


# ListJobsByPipelineRequestPaginateTypeDef definition

class ListJobsByPipelineRequestPaginateTypeDef(TypedDict):
    PipelineId: str,
    Ascending: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobsByStatusRequestPaginateTypeDef

```python
# ListJobsByStatusRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ListJobsByStatusRequestPaginateTypeDef


def get_value() -> ListJobsByStatusRequestPaginateTypeDef:
    return {
        "Status": ...,
    }


# ListJobsByStatusRequestPaginateTypeDef definition

class ListJobsByStatusRequestPaginateTypeDef(TypedDict):
    Status: str,
    Ascending: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPipelinesRequestPaginateTypeDef

```python
# ListPipelinesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ListPipelinesRequestPaginateTypeDef


def get_value() -> ListPipelinesRequestPaginateTypeDef:
    return {
        "Ascending": ...,
    }


# ListPipelinesRequestPaginateTypeDef definition

class ListPipelinesRequestPaginateTypeDef(TypedDict):
    Ascending: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPresetsRequestPaginateTypeDef

```python
# ListPresetsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ListPresetsRequestPaginateTypeDef


def get_value() -> ListPresetsRequestPaginateTypeDef:
    return {
        "Ascending": ...,
    }


# ListPresetsRequestPaginateTypeDef definition

class ListPresetsRequestPaginateTypeDef(TypedDict):
    Ascending: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## PipelineOutputConfigOutputTypeDef

```python
# PipelineOutputConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import PipelineOutputConfigOutputTypeDef


def get_value() -> PipelineOutputConfigOutputTypeDef:
    return {
        "Bucket": ...,
    }


# PipelineOutputConfigOutputTypeDef definition

class PipelineOutputConfigOutputTypeDef(TypedDict):
    Bucket: NotRequired[str],
    StorageClass: NotRequired[str],
    Permissions: NotRequired[List[PermissionOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: PermissionOutputTypeDef](./type_defs.md#permissionoutputtypedef) 
## PipelineOutputConfigTypeDef

```python
# PipelineOutputConfigTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import PipelineOutputConfigTypeDef


def get_value() -> PipelineOutputConfigTypeDef:
    return {
        "Bucket": ...,
    }


# PipelineOutputConfigTypeDef definition

class PipelineOutputConfigTypeDef(TypedDict):
    Bucket: NotRequired[str],
    StorageClass: NotRequired[str],
    Permissions: NotRequired[Sequence[PermissionTypeDef]],  # (1)
```

1. See [:material-code-braces: PermissionTypeDef](./type_defs.md#permissiontypedef) 
## VideoParametersOutputTypeDef

```python
# VideoParametersOutputTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import VideoParametersOutputTypeDef


def get_value() -> VideoParametersOutputTypeDef:
    return {
        "Codec": ...,
    }


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
# VideoParametersTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import VideoParametersTypeDef


def get_value() -> VideoParametersTypeDef:
    return {
        "Codec": ...,
    }


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
## ReadJobRequestWaitTypeDef

```python
# ReadJobRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ReadJobRequestWaitTypeDef


def get_value() -> ReadJobRequestWaitTypeDef:
    return {
        "Id": ...,
    }


# ReadJobRequestWaitTypeDef definition

class ReadJobRequestWaitTypeDef(TypedDict):
    Id: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## JobAlbumArtOutputTypeDef

```python
# JobAlbumArtOutputTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import JobAlbumArtOutputTypeDef


def get_value() -> JobAlbumArtOutputTypeDef:
    return {
        "MergePolicy": ...,
    }


# JobAlbumArtOutputTypeDef definition

class JobAlbumArtOutputTypeDef(TypedDict):
    MergePolicy: NotRequired[str],
    Artwork: NotRequired[List[ArtworkTypeDef]],  # (1)
```

1. See [:material-code-braces: ArtworkTypeDef](./type_defs.md#artworktypedef) 
## JobAlbumArtTypeDef

```python
# JobAlbumArtTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import JobAlbumArtTypeDef


def get_value() -> JobAlbumArtTypeDef:
    return {
        "MergePolicy": ...,
    }


# JobAlbumArtTypeDef definition

class JobAlbumArtTypeDef(TypedDict):
    MergePolicy: NotRequired[str],
    Artwork: NotRequired[Sequence[ArtworkTypeDef]],  # (1)
```

1. See [:material-code-braces: ArtworkTypeDef](./type_defs.md#artworktypedef) 
## CaptionsOutputTypeDef

```python
# CaptionsOutputTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import CaptionsOutputTypeDef


def get_value() -> CaptionsOutputTypeDef:
    return {
        "MergePolicy": ...,
    }


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
# CaptionsTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import CaptionsTypeDef


def get_value() -> CaptionsTypeDef:
    return {
        "MergePolicy": ...,
    }


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
# InputCaptionsOutputTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import InputCaptionsOutputTypeDef


def get_value() -> InputCaptionsOutputTypeDef:
    return {
        "MergePolicy": ...,
    }


# InputCaptionsOutputTypeDef definition

class InputCaptionsOutputTypeDef(TypedDict):
    MergePolicy: NotRequired[str],
    CaptionSources: NotRequired[List[CaptionSourceTypeDef]],  # (1)
```

1. See [:material-code-braces: CaptionSourceTypeDef](./type_defs.md#captionsourcetypedef) 
## InputCaptionsTypeDef

```python
# InputCaptionsTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import InputCaptionsTypeDef


def get_value() -> InputCaptionsTypeDef:
    return {
        "MergePolicy": ...,
    }


# InputCaptionsTypeDef definition

class InputCaptionsTypeDef(TypedDict):
    MergePolicy: NotRequired[str],
    CaptionSources: NotRequired[Sequence[CaptionSourceTypeDef]],  # (1)
```

1. See [:material-code-braces: CaptionSourceTypeDef](./type_defs.md#captionsourcetypedef) 
## PipelineTypeDef

```python
# PipelineTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import PipelineTypeDef


def get_value() -> PipelineTypeDef:
    return {
        "Id": ...,
    }


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
## PresetTypeDef

```python
# PresetTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import PresetTypeDef


def get_value() -> PresetTypeDef:
    return {
        "Id": ...,
    }


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
## JobOutputTypeDef

```python
# JobOutputTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import JobOutputTypeDef


def get_value() -> JobOutputTypeDef:
    return {
        "Id": ...,
    }


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
# JobInputOutputTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import JobInputOutputTypeDef


def get_value() -> JobInputOutputTypeDef:
    return {
        "Key": ...,
    }


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
# CreatePipelineResponseTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import CreatePipelineResponseTypeDef


def get_value() -> CreatePipelineResponseTypeDef:
    return {
        "Pipeline": ...,
    }


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
# ListPipelinesResponseTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ListPipelinesResponseTypeDef


def get_value() -> ListPipelinesResponseTypeDef:
    return {
        "Pipelines": ...,
    }


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
# ReadPipelineResponseTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ReadPipelineResponseTypeDef


def get_value() -> ReadPipelineResponseTypeDef:
    return {
        "Pipeline": ...,
    }


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
# UpdatePipelineNotificationsResponseTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import UpdatePipelineNotificationsResponseTypeDef


def get_value() -> UpdatePipelineNotificationsResponseTypeDef:
    return {
        "Pipeline": ...,
    }


# UpdatePipelineNotificationsResponseTypeDef definition

class UpdatePipelineNotificationsResponseTypeDef(TypedDict):
    Pipeline: PipelineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineTypeDef](./type_defs.md#pipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePipelineResponseTypeDef

```python
# UpdatePipelineResponseTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import UpdatePipelineResponseTypeDef


def get_value() -> UpdatePipelineResponseTypeDef:
    return {
        "Pipeline": ...,
    }


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
# UpdatePipelineStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import UpdatePipelineStatusResponseTypeDef


def get_value() -> UpdatePipelineStatusResponseTypeDef:
    return {
        "Pipeline": ...,
    }


# UpdatePipelineStatusResponseTypeDef definition

class UpdatePipelineStatusResponseTypeDef(TypedDict):
    Pipeline: PipelineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineTypeDef](./type_defs.md#pipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePipelineRequestTypeDef

```python
# CreatePipelineRequestTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import CreatePipelineRequestTypeDef


def get_value() -> CreatePipelineRequestTypeDef:
    return {
        "Name": ...,
    }


# CreatePipelineRequestTypeDef definition

class CreatePipelineRequestTypeDef(TypedDict):
    Name: str,
    InputBucket: str,
    Role: str,
    OutputBucket: NotRequired[str],
    AwsKmsKeyArn: NotRequired[str],
    Notifications: NotRequired[NotificationsTypeDef],  # (1)
    ContentConfig: NotRequired[PipelineOutputConfigUnionTypeDef],  # (2)
    ThumbnailConfig: NotRequired[PipelineOutputConfigUnionTypeDef],  # (2)
```

1. See [:material-code-braces: NotificationsTypeDef](./type_defs.md#notificationstypedef) 
2. See [:material-code-braces: PipelineOutputConfigTypeDef](./type_defs.md#pipelineoutputconfigtypedef) [:material-code-braces: PipelineOutputConfigOutputTypeDef](./type_defs.md#pipelineoutputconfigoutputtypedef) 
3. See [:material-code-braces: PipelineOutputConfigTypeDef](./type_defs.md#pipelineoutputconfigtypedef) [:material-code-braces: PipelineOutputConfigOutputTypeDef](./type_defs.md#pipelineoutputconfigoutputtypedef) 
## UpdatePipelineRequestTypeDef

```python
# UpdatePipelineRequestTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import UpdatePipelineRequestTypeDef


def get_value() -> UpdatePipelineRequestTypeDef:
    return {
        "Id": ...,
    }


# UpdatePipelineRequestTypeDef definition

class UpdatePipelineRequestTypeDef(TypedDict):
    Id: str,
    Name: NotRequired[str],
    InputBucket: NotRequired[str],
    Role: NotRequired[str],
    AwsKmsKeyArn: NotRequired[str],
    Notifications: NotRequired[NotificationsTypeDef],  # (1)
    ContentConfig: NotRequired[PipelineOutputConfigUnionTypeDef],  # (2)
    ThumbnailConfig: NotRequired[PipelineOutputConfigUnionTypeDef],  # (2)
```

1. See [:material-code-braces: NotificationsTypeDef](./type_defs.md#notificationstypedef) 
2. See [:material-code-braces: PipelineOutputConfigTypeDef](./type_defs.md#pipelineoutputconfigtypedef) [:material-code-braces: PipelineOutputConfigOutputTypeDef](./type_defs.md#pipelineoutputconfigoutputtypedef) 
3. See [:material-code-braces: PipelineOutputConfigTypeDef](./type_defs.md#pipelineoutputconfigtypedef) [:material-code-braces: PipelineOutputConfigOutputTypeDef](./type_defs.md#pipelineoutputconfigoutputtypedef) 
## CreatePresetResponseTypeDef

```python
# CreatePresetResponseTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import CreatePresetResponseTypeDef


def get_value() -> CreatePresetResponseTypeDef:
    return {
        "Preset": ...,
    }


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
# ListPresetsResponseTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ListPresetsResponseTypeDef


def get_value() -> ListPresetsResponseTypeDef:
    return {
        "Presets": ...,
    }


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
# ReadPresetResponseTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ReadPresetResponseTypeDef


def get_value() -> ReadPresetResponseTypeDef:
    return {
        "Preset": ...,
    }


# ReadPresetResponseTypeDef definition

class ReadPresetResponseTypeDef(TypedDict):
    Preset: PresetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PresetTypeDef](./type_defs.md#presettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePresetRequestTypeDef

```python
# CreatePresetRequestTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import CreatePresetRequestTypeDef


def get_value() -> CreatePresetRequestTypeDef:
    return {
        "Name": ...,
    }


# CreatePresetRequestTypeDef definition

class CreatePresetRequestTypeDef(TypedDict):
    Name: str,
    Container: str,
    Description: NotRequired[str],
    Video: NotRequired[VideoParametersUnionTypeDef],  # (1)
    Audio: NotRequired[AudioParametersTypeDef],  # (2)
    Thumbnails: NotRequired[ThumbnailsTypeDef],  # (3)
```

1. See [:material-code-braces: VideoParametersTypeDef](./type_defs.md#videoparameterstypedef) [:material-code-braces: VideoParametersOutputTypeDef](./type_defs.md#videoparametersoutputtypedef) 
2. See [:material-code-braces: AudioParametersTypeDef](./type_defs.md#audioparameterstypedef) 
3. See [:material-code-braces: ThumbnailsTypeDef](./type_defs.md#thumbnailstypedef) 
## CreateJobOutputTypeDef

```python
# CreateJobOutputTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import CreateJobOutputTypeDef


def get_value() -> CreateJobOutputTypeDef:
    return {
        "Key": ...,
    }


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
# JobTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import JobTypeDef


def get_value() -> JobTypeDef:
    return {
        "Id": ...,
    }


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
# JobInputTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import JobInputTypeDef


def get_value() -> JobInputTypeDef:
    return {
        "Key": ...,
    }


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
# CreateJobResponseTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import CreateJobResponseTypeDef


def get_value() -> CreateJobResponseTypeDef:
    return {
        "Job": ...,
    }


# CreateJobResponseTypeDef definition

class CreateJobResponseTypeDef(TypedDict):
    Job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJobsByPipelineResponseTypeDef

```python
# ListJobsByPipelineResponseTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ListJobsByPipelineResponseTypeDef


def get_value() -> ListJobsByPipelineResponseTypeDef:
    return {
        "Jobs": ...,
    }


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
# ListJobsByStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ListJobsByStatusResponseTypeDef


def get_value() -> ListJobsByStatusResponseTypeDef:
    return {
        "Jobs": ...,
    }


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
# ReadJobResponseTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import ReadJobResponseTypeDef


def get_value() -> ReadJobResponseTypeDef:
    return {
        "Job": ...,
    }


# ReadJobResponseTypeDef definition

class ReadJobResponseTypeDef(TypedDict):
    Job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobRequestTypeDef

```python
# CreateJobRequestTypeDef TypedDict usage example

from types_aiobotocore_elastictranscoder.type_defs import CreateJobRequestTypeDef


def get_value() -> CreateJobRequestTypeDef:
    return {
        "PipelineId": ...,
    }


# CreateJobRequestTypeDef definition

class CreateJobRequestTypeDef(TypedDict):
    PipelineId: str,
    Input: NotRequired[JobInputUnionTypeDef],  # (1)
    Inputs: NotRequired[Sequence[JobInputUnionTypeDef]],  # (2)
    Output: NotRequired[CreateJobOutputTypeDef],  # (3)
    Outputs: NotRequired[Sequence[CreateJobOutputTypeDef]],  # (4)
    OutputKeyPrefix: NotRequired[str],
    Playlists: NotRequired[Sequence[CreateJobPlaylistTypeDef]],  # (5)
    UserMetadata: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: JobInputTypeDef](./type_defs.md#jobinputtypedef) [:material-code-braces: JobInputOutputTypeDef](./type_defs.md#jobinputoutputtypedef) 
2. See [:material-code-braces: JobInputTypeDef](./type_defs.md#jobinputtypedef) [:material-code-braces: JobInputOutputTypeDef](./type_defs.md#jobinputoutputtypedef) 
3. See [:material-code-braces: CreateJobOutputTypeDef](./type_defs.md#createjoboutputtypedef) 
4. See [:material-code-braces: CreateJobOutputTypeDef](./type_defs.md#createjoboutputtypedef) 
5. See [:material-code-braces: CreateJobPlaylistTypeDef](./type_defs.md#createjobplaylisttypedef) 
