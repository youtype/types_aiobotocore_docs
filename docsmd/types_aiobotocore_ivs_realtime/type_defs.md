# Type definitions

> [Index](../README.md) > [Ivsrealtime](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Ivsrealtime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
    type annotations stubs module [types-aiobotocore-ivs-realtime](https://pypi.org/project/types-aiobotocore-ivs-realtime/).

## CompositionThumbnailConfigurationUnionTypeDef

```python
# CompositionThumbnailConfigurationUnionTypeDef Union usage example

from types_aiobotocore_ivs_realtime.type_defs import CompositionThumbnailConfigurationUnionTypeDef


def get_value() -> CompositionThumbnailConfigurationUnionTypeDef:
    return ...


# CompositionThumbnailConfigurationUnionTypeDef definition

CompositionThumbnailConfigurationUnionTypeDef = Union[
    CompositionThumbnailConfigurationTypeDef,  # (1)
    CompositionThumbnailConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CompositionThumbnailConfigurationTypeDef](./type_defs.md#compositionthumbnailconfigurationtypedef) 
2. See [:material-code-braces: CompositionThumbnailConfigurationOutputTypeDef](./type_defs.md#compositionthumbnailconfigurationoutputtypedef) 

## AutoParticipantRecordingConfigurationUnionTypeDef

```python
# AutoParticipantRecordingConfigurationUnionTypeDef Union usage example

from types_aiobotocore_ivs_realtime.type_defs import AutoParticipantRecordingConfigurationUnionTypeDef


def get_value() -> AutoParticipantRecordingConfigurationUnionTypeDef:
    return ...


# AutoParticipantRecordingConfigurationUnionTypeDef definition

AutoParticipantRecordingConfigurationUnionTypeDef = Union[
    AutoParticipantRecordingConfigurationTypeDef,  # (1)
    AutoParticipantRecordingConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AutoParticipantRecordingConfigurationTypeDef](./type_defs.md#autoparticipantrecordingconfigurationtypedef) 
2. See [:material-code-braces: AutoParticipantRecordingConfigurationOutputTypeDef](./type_defs.md#autoparticipantrecordingconfigurationoutputtypedef) 

## S3DestinationConfigurationUnionTypeDef

```python
# S3DestinationConfigurationUnionTypeDef Union usage example

from types_aiobotocore_ivs_realtime.type_defs import S3DestinationConfigurationUnionTypeDef


def get_value() -> S3DestinationConfigurationUnionTypeDef:
    return ...


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
# DestinationConfigurationUnionTypeDef Union usage example

from types_aiobotocore_ivs_realtime.type_defs import DestinationConfigurationUnionTypeDef


def get_value() -> DestinationConfigurationUnionTypeDef:
    return ...


# DestinationConfigurationUnionTypeDef definition

DestinationConfigurationUnionTypeDef = Union[
    DestinationConfigurationTypeDef,  # (1)
    DestinationConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
2. See [:material-code-braces: DestinationConfigurationOutputTypeDef](./type_defs.md#destinationconfigurationoutputtypedef) 



## ParticipantThumbnailConfigurationOutputTypeDef

```python
# ParticipantThumbnailConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ParticipantThumbnailConfigurationOutputTypeDef


def get_value() -> ParticipantThumbnailConfigurationOutputTypeDef:
    return {
        "targetIntervalSeconds": ...,
    }


# ParticipantThumbnailConfigurationOutputTypeDef definition

class ParticipantThumbnailConfigurationOutputTypeDef(TypedDict):
    targetIntervalSeconds: NotRequired[int],
    storage: NotRequired[List[ThumbnailStorageTypeType]],  # (1)
    recordingMode: NotRequired[ThumbnailRecordingModeType],  # (2)
```

1. See [:material-code-brackets: ThumbnailStorageTypeType](./literals.md#thumbnailstoragetypetype) 
2. See [:material-code-brackets: ThumbnailRecordingModeType](./literals.md#thumbnailrecordingmodetype) 
## ParticipantThumbnailConfigurationTypeDef

```python
# ParticipantThumbnailConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ParticipantThumbnailConfigurationTypeDef


def get_value() -> ParticipantThumbnailConfigurationTypeDef:
    return {
        "targetIntervalSeconds": ...,
    }


# ParticipantThumbnailConfigurationTypeDef definition

class ParticipantThumbnailConfigurationTypeDef(TypedDict):
    targetIntervalSeconds: NotRequired[int],
    storage: NotRequired[Sequence[ThumbnailStorageTypeType]],  # (1)
    recordingMode: NotRequired[ThumbnailRecordingModeType],  # (2)
```

1. See [:material-code-brackets: ThumbnailStorageTypeType](./literals.md#thumbnailstoragetypetype) 
2. See [:material-code-brackets: ThumbnailRecordingModeType](./literals.md#thumbnailrecordingmodetype) 
## ChannelDestinationConfigurationTypeDef

```python
# ChannelDestinationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ChannelDestinationConfigurationTypeDef


def get_value() -> ChannelDestinationConfigurationTypeDef:
    return {
        "channelArn": ...,
    }


# ChannelDestinationConfigurationTypeDef definition

class ChannelDestinationConfigurationTypeDef(TypedDict):
    channelArn: str,
    encoderConfigurationArn: NotRequired[str],
```

## DestinationSummaryTypeDef

```python
# DestinationSummaryTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import DestinationSummaryTypeDef


def get_value() -> DestinationSummaryTypeDef:
    return {
        "id": ...,
    }


# DestinationSummaryTypeDef definition

class DestinationSummaryTypeDef(TypedDict):
    id: str,
    state: DestinationStateType,  # (1)
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
```

1. See [:material-code-brackets: DestinationStateType](./literals.md#destinationstatetype) 
## CompositionThumbnailConfigurationOutputTypeDef

```python
# CompositionThumbnailConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import CompositionThumbnailConfigurationOutputTypeDef


def get_value() -> CompositionThumbnailConfigurationOutputTypeDef:
    return {
        "targetIntervalSeconds": ...,
    }


# CompositionThumbnailConfigurationOutputTypeDef definition

class CompositionThumbnailConfigurationOutputTypeDef(TypedDict):
    targetIntervalSeconds: NotRequired[int],
    storage: NotRequired[List[ThumbnailStorageTypeType]],  # (1)
```

1. See [:material-code-brackets: ThumbnailStorageTypeType](./literals.md#thumbnailstoragetypetype) 
## CompositionThumbnailConfigurationTypeDef

```python
# CompositionThumbnailConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import CompositionThumbnailConfigurationTypeDef


def get_value() -> CompositionThumbnailConfigurationTypeDef:
    return {
        "targetIntervalSeconds": ...,
    }


# CompositionThumbnailConfigurationTypeDef definition

class CompositionThumbnailConfigurationTypeDef(TypedDict):
    targetIntervalSeconds: NotRequired[int],
    storage: NotRequired[Sequence[ThumbnailStorageTypeType]],  # (1)
```

1. See [:material-code-brackets: ThumbnailStorageTypeType](./literals.md#thumbnailstoragetypetype) 
## VideoTypeDef

```python
# VideoTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import VideoTypeDef


def get_value() -> VideoTypeDef:
    return {
        "width": ...,
    }


# VideoTypeDef definition

class VideoTypeDef(TypedDict):
    width: NotRequired[int],
    height: NotRequired[int],
    framerate: NotRequired[float],
    bitrate: NotRequired[int],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ResponseMetadataTypeDef


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

## CreateIngestConfigurationRequestTypeDef

```python
# CreateIngestConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import CreateIngestConfigurationRequestTypeDef


def get_value() -> CreateIngestConfigurationRequestTypeDef:
    return {
        "ingestProtocol": ...,
    }


# CreateIngestConfigurationRequestTypeDef definition

class CreateIngestConfigurationRequestTypeDef(TypedDict):
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
# IngestConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import IngestConfigurationTypeDef


def get_value() -> IngestConfigurationTypeDef:
    return {
        "name": ...,
    }


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
## CreateParticipantTokenRequestTypeDef

```python
# CreateParticipantTokenRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import CreateParticipantTokenRequestTypeDef


def get_value() -> CreateParticipantTokenRequestTypeDef:
    return {
        "stageArn": ...,
    }


# CreateParticipantTokenRequestTypeDef definition

class CreateParticipantTokenRequestTypeDef(TypedDict):
    stageArn: str,
    duration: NotRequired[int],
    userId: NotRequired[str],
    attributes: NotRequired[Mapping[str, str]],
    capabilities: NotRequired[Sequence[ParticipantTokenCapabilityType]],  # (1)
```

1. See [:material-code-brackets: ParticipantTokenCapabilityType](./literals.md#participanttokencapabilitytype) 
## ParticipantTokenTypeDef

```python
# ParticipantTokenTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ParticipantTokenTypeDef


def get_value() -> ParticipantTokenTypeDef:
    return {
        "participantId": ...,
    }


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
# ParticipantTokenConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ParticipantTokenConfigurationTypeDef


def get_value() -> ParticipantTokenConfigurationTypeDef:
    return {
        "duration": ...,
    }


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
# S3StorageConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import S3StorageConfigurationTypeDef


def get_value() -> S3StorageConfigurationTypeDef:
    return {
        "bucketName": ...,
    }


# S3StorageConfigurationTypeDef definition

class S3StorageConfigurationTypeDef(TypedDict):
    bucketName: str,
```

## DeleteEncoderConfigurationRequestTypeDef

```python
# DeleteEncoderConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import DeleteEncoderConfigurationRequestTypeDef


def get_value() -> DeleteEncoderConfigurationRequestTypeDef:
    return {
        "arn": ...,
    }


# DeleteEncoderConfigurationRequestTypeDef definition

class DeleteEncoderConfigurationRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteIngestConfigurationRequestTypeDef

```python
# DeleteIngestConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import DeleteIngestConfigurationRequestTypeDef


def get_value() -> DeleteIngestConfigurationRequestTypeDef:
    return {
        "arn": ...,
    }


# DeleteIngestConfigurationRequestTypeDef definition

class DeleteIngestConfigurationRequestTypeDef(TypedDict):
    arn: str,
    force: NotRequired[bool],
```

## DeletePublicKeyRequestTypeDef

```python
# DeletePublicKeyRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import DeletePublicKeyRequestTypeDef


def get_value() -> DeletePublicKeyRequestTypeDef:
    return {
        "arn": ...,
    }


# DeletePublicKeyRequestTypeDef definition

class DeletePublicKeyRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteStageRequestTypeDef

```python
# DeleteStageRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import DeleteStageRequestTypeDef


def get_value() -> DeleteStageRequestTypeDef:
    return {
        "arn": ...,
    }


# DeleteStageRequestTypeDef definition

class DeleteStageRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteStorageConfigurationRequestTypeDef

```python
# DeleteStorageConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import DeleteStorageConfigurationRequestTypeDef


def get_value() -> DeleteStorageConfigurationRequestTypeDef:
    return {
        "arn": ...,
    }


# DeleteStorageConfigurationRequestTypeDef definition

class DeleteStorageConfigurationRequestTypeDef(TypedDict):
    arn: str,
```

## S3DetailTypeDef

```python
# S3DetailTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import S3DetailTypeDef


def get_value() -> S3DetailTypeDef:
    return {
        "recordingPrefix": ...,
    }


# S3DetailTypeDef definition

class S3DetailTypeDef(TypedDict):
    recordingPrefix: str,
```

## DisconnectParticipantRequestTypeDef

```python
# DisconnectParticipantRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import DisconnectParticipantRequestTypeDef


def get_value() -> DisconnectParticipantRequestTypeDef:
    return {
        "stageArn": ...,
    }


# DisconnectParticipantRequestTypeDef definition

class DisconnectParticipantRequestTypeDef(TypedDict):
    stageArn: str,
    participantId: str,
    reason: NotRequired[str],
```

## EncoderConfigurationSummaryTypeDef

```python
# EncoderConfigurationSummaryTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import EncoderConfigurationSummaryTypeDef


def get_value() -> EncoderConfigurationSummaryTypeDef:
    return {
        "arn": ...,
    }


# EncoderConfigurationSummaryTypeDef definition

class EncoderConfigurationSummaryTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## EventTypeDef

```python
# EventTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import EventTypeDef


def get_value() -> EventTypeDef:
    return {
        "name": ...,
    }


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
## GetCompositionRequestTypeDef

```python
# GetCompositionRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import GetCompositionRequestTypeDef


def get_value() -> GetCompositionRequestTypeDef:
    return {
        "arn": ...,
    }


# GetCompositionRequestTypeDef definition

class GetCompositionRequestTypeDef(TypedDict):
    arn: str,
```

## GetEncoderConfigurationRequestTypeDef

```python
# GetEncoderConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import GetEncoderConfigurationRequestTypeDef


def get_value() -> GetEncoderConfigurationRequestTypeDef:
    return {
        "arn": ...,
    }


# GetEncoderConfigurationRequestTypeDef definition

class GetEncoderConfigurationRequestTypeDef(TypedDict):
    arn: str,
```

## GetIngestConfigurationRequestTypeDef

```python
# GetIngestConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import GetIngestConfigurationRequestTypeDef


def get_value() -> GetIngestConfigurationRequestTypeDef:
    return {
        "arn": ...,
    }


# GetIngestConfigurationRequestTypeDef definition

class GetIngestConfigurationRequestTypeDef(TypedDict):
    arn: str,
```

## GetParticipantRequestTypeDef

```python
# GetParticipantRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import GetParticipantRequestTypeDef


def get_value() -> GetParticipantRequestTypeDef:
    return {
        "stageArn": ...,
    }


# GetParticipantRequestTypeDef definition

class GetParticipantRequestTypeDef(TypedDict):
    stageArn: str,
    sessionId: str,
    participantId: str,
```

## ParticipantTypeDef

```python
# ParticipantTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ParticipantTypeDef


def get_value() -> ParticipantTypeDef:
    return {
        "participantId": ...,
    }


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
## GetPublicKeyRequestTypeDef

```python
# GetPublicKeyRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import GetPublicKeyRequestTypeDef


def get_value() -> GetPublicKeyRequestTypeDef:
    return {
        "arn": ...,
    }


# GetPublicKeyRequestTypeDef definition

class GetPublicKeyRequestTypeDef(TypedDict):
    arn: str,
```

## PublicKeyTypeDef

```python
# PublicKeyTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import PublicKeyTypeDef


def get_value() -> PublicKeyTypeDef:
    return {
        "arn": ...,
    }


# PublicKeyTypeDef definition

class PublicKeyTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    publicKeyMaterial: NotRequired[str],
    fingerprint: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## GetStageRequestTypeDef

```python
# GetStageRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import GetStageRequestTypeDef


def get_value() -> GetStageRequestTypeDef:
    return {
        "arn": ...,
    }


# GetStageRequestTypeDef definition

class GetStageRequestTypeDef(TypedDict):
    arn: str,
```

## GetStageSessionRequestTypeDef

```python
# GetStageSessionRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import GetStageSessionRequestTypeDef


def get_value() -> GetStageSessionRequestTypeDef:
    return {
        "stageArn": ...,
    }


# GetStageSessionRequestTypeDef definition

class GetStageSessionRequestTypeDef(TypedDict):
    stageArn: str,
    sessionId: str,
```

## StageSessionTypeDef

```python
# StageSessionTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import StageSessionTypeDef


def get_value() -> StageSessionTypeDef:
    return {
        "sessionId": ...,
    }


# StageSessionTypeDef definition

class StageSessionTypeDef(TypedDict):
    sessionId: NotRequired[str],
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
```

## GetStorageConfigurationRequestTypeDef

```python
# GetStorageConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import GetStorageConfigurationRequestTypeDef


def get_value() -> GetStorageConfigurationRequestTypeDef:
    return {
        "arn": ...,
    }


# GetStorageConfigurationRequestTypeDef definition

class GetStorageConfigurationRequestTypeDef(TypedDict):
    arn: str,
```

## GridConfigurationTypeDef

```python
# GridConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import GridConfigurationTypeDef


def get_value() -> GridConfigurationTypeDef:
    return {
        "featuredParticipantAttribute": ...,
    }


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
## ImportPublicKeyRequestTypeDef

```python
# ImportPublicKeyRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ImportPublicKeyRequestTypeDef


def get_value() -> ImportPublicKeyRequestTypeDef:
    return {
        "publicKeyMaterial": ...,
    }


# ImportPublicKeyRequestTypeDef definition

class ImportPublicKeyRequestTypeDef(TypedDict):
    publicKeyMaterial: str,
    name: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## IngestConfigurationSummaryTypeDef

```python
# IngestConfigurationSummaryTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import IngestConfigurationSummaryTypeDef


def get_value() -> IngestConfigurationSummaryTypeDef:
    return {
        "name": ...,
    }


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
# PipConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import PipConfigurationTypeDef


def get_value() -> PipConfigurationTypeDef:
    return {
        "featuredParticipantAttribute": ...,
    }


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
## ListCompositionsRequestTypeDef

```python
# ListCompositionsRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ListCompositionsRequestTypeDef


def get_value() -> ListCompositionsRequestTypeDef:
    return {
        "filterByStageArn": ...,
    }


# ListCompositionsRequestTypeDef definition

class ListCompositionsRequestTypeDef(TypedDict):
    filterByStageArn: NotRequired[str],
    filterByEncoderConfigurationArn: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListEncoderConfigurationsRequestTypeDef

```python
# ListEncoderConfigurationsRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ListEncoderConfigurationsRequestTypeDef


def get_value() -> ListEncoderConfigurationsRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListEncoderConfigurationsRequestTypeDef definition

class ListEncoderConfigurationsRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import PaginatorConfigTypeDef


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

## ListIngestConfigurationsRequestTypeDef

```python
# ListIngestConfigurationsRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ListIngestConfigurationsRequestTypeDef


def get_value() -> ListIngestConfigurationsRequestTypeDef:
    return {
        "filterByStageArn": ...,
    }


# ListIngestConfigurationsRequestTypeDef definition

class ListIngestConfigurationsRequestTypeDef(TypedDict):
    filterByStageArn: NotRequired[str],
    filterByState: NotRequired[IngestConfigurationStateType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: IngestConfigurationStateType](./literals.md#ingestconfigurationstatetype) 
## ListParticipantEventsRequestTypeDef

```python
# ListParticipantEventsRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ListParticipantEventsRequestTypeDef


def get_value() -> ListParticipantEventsRequestTypeDef:
    return {
        "stageArn": ...,
    }


# ListParticipantEventsRequestTypeDef definition

class ListParticipantEventsRequestTypeDef(TypedDict):
    stageArn: str,
    sessionId: str,
    participantId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListParticipantsRequestTypeDef

```python
# ListParticipantsRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ListParticipantsRequestTypeDef


def get_value() -> ListParticipantsRequestTypeDef:
    return {
        "stageArn": ...,
    }


# ListParticipantsRequestTypeDef definition

class ListParticipantsRequestTypeDef(TypedDict):
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
# ParticipantSummaryTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ParticipantSummaryTypeDef


def get_value() -> ParticipantSummaryTypeDef:
    return {
        "participantId": ...,
    }


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
## ListPublicKeysRequestTypeDef

```python
# ListPublicKeysRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ListPublicKeysRequestTypeDef


def get_value() -> ListPublicKeysRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListPublicKeysRequestTypeDef definition

class ListPublicKeysRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## PublicKeySummaryTypeDef

```python
# PublicKeySummaryTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import PublicKeySummaryTypeDef


def get_value() -> PublicKeySummaryTypeDef:
    return {
        "arn": ...,
    }


# PublicKeySummaryTypeDef definition

class PublicKeySummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## ListStageSessionsRequestTypeDef

```python
# ListStageSessionsRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ListStageSessionsRequestTypeDef


def get_value() -> ListStageSessionsRequestTypeDef:
    return {
        "stageArn": ...,
    }


# ListStageSessionsRequestTypeDef definition

class ListStageSessionsRequestTypeDef(TypedDict):
    stageArn: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## StageSessionSummaryTypeDef

```python
# StageSessionSummaryTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import StageSessionSummaryTypeDef


def get_value() -> StageSessionSummaryTypeDef:
    return {
        "sessionId": ...,
    }


# StageSessionSummaryTypeDef definition

class StageSessionSummaryTypeDef(TypedDict):
    sessionId: NotRequired[str],
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
```

## ListStagesRequestTypeDef

```python
# ListStagesRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ListStagesRequestTypeDef


def get_value() -> ListStagesRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListStagesRequestTypeDef definition

class ListStagesRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## StageSummaryTypeDef

```python
# StageSummaryTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import StageSummaryTypeDef


def get_value() -> StageSummaryTypeDef:
    return {
        "arn": ...,
    }


# StageSummaryTypeDef definition

class StageSummaryTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    activeSessionId: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## ListStorageConfigurationsRequestTypeDef

```python
# ListStorageConfigurationsRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ListStorageConfigurationsRequestTypeDef


def get_value() -> ListStorageConfigurationsRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListStorageConfigurationsRequestTypeDef definition

class ListStorageConfigurationsRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## RecordingConfigurationTypeDef

```python
# RecordingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import RecordingConfigurationTypeDef


def get_value() -> RecordingConfigurationTypeDef:
    return {
        "format": ...,
    }


# RecordingConfigurationTypeDef definition

class RecordingConfigurationTypeDef(TypedDict):
    format: NotRequired[RecordingConfigurationFormatType],  # (1)
```

1. See [:material-code-brackets: RecordingConfigurationFormatType](./literals.md#recordingconfigurationformattype) 
## StageEndpointsTypeDef

```python
# StageEndpointsTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import StageEndpointsTypeDef


def get_value() -> StageEndpointsTypeDef:
    return {
        "events": ...,
    }


# StageEndpointsTypeDef definition

class StageEndpointsTypeDef(TypedDict):
    events: NotRequired[str],
    whip: NotRequired[str],
    rtmp: NotRequired[str],
    rtmps: NotRequired[str],
```

## StopCompositionRequestTypeDef

```python
# StopCompositionRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import StopCompositionRequestTypeDef


def get_value() -> StopCompositionRequestTypeDef:
    return {
        "arn": ...,
    }


# StopCompositionRequestTypeDef definition

class StopCompositionRequestTypeDef(TypedDict):
    arn: str,
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateIngestConfigurationRequestTypeDef

```python
# UpdateIngestConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import UpdateIngestConfigurationRequestTypeDef


def get_value() -> UpdateIngestConfigurationRequestTypeDef:
    return {
        "arn": ...,
    }


# UpdateIngestConfigurationRequestTypeDef definition

class UpdateIngestConfigurationRequestTypeDef(TypedDict):
    arn: str,
    stageArn: NotRequired[str],
```

## AutoParticipantRecordingConfigurationOutputTypeDef

```python
# AutoParticipantRecordingConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import AutoParticipantRecordingConfigurationOutputTypeDef


def get_value() -> AutoParticipantRecordingConfigurationOutputTypeDef:
    return {
        "storageConfigurationArn": ...,
    }


# AutoParticipantRecordingConfigurationOutputTypeDef definition

class AutoParticipantRecordingConfigurationOutputTypeDef(TypedDict):
    storageConfigurationArn: str,
    mediaTypes: NotRequired[List[ParticipantRecordingMediaTypeType]],  # (1)
    thumbnailConfiguration: NotRequired[ParticipantThumbnailConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: ParticipantRecordingMediaTypeType](./literals.md#participantrecordingmediatypetype) 
2. See [:material-code-braces: ParticipantThumbnailConfigurationOutputTypeDef](./type_defs.md#participantthumbnailconfigurationoutputtypedef) 
## AutoParticipantRecordingConfigurationTypeDef

```python
# AutoParticipantRecordingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import AutoParticipantRecordingConfigurationTypeDef


def get_value() -> AutoParticipantRecordingConfigurationTypeDef:
    return {
        "storageConfigurationArn": ...,
    }


# AutoParticipantRecordingConfigurationTypeDef definition

class AutoParticipantRecordingConfigurationTypeDef(TypedDict):
    storageConfigurationArn: str,
    mediaTypes: NotRequired[Sequence[ParticipantRecordingMediaTypeType]],  # (1)
    thumbnailConfiguration: NotRequired[ParticipantThumbnailConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: ParticipantRecordingMediaTypeType](./literals.md#participantrecordingmediatypetype) 
2. See [:material-code-braces: ParticipantThumbnailConfigurationTypeDef](./type_defs.md#participantthumbnailconfigurationtypedef) 
## CompositionSummaryTypeDef

```python
# CompositionSummaryTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import CompositionSummaryTypeDef


def get_value() -> CompositionSummaryTypeDef:
    return {
        "arn": ...,
    }


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
## CreateEncoderConfigurationRequestTypeDef

```python
# CreateEncoderConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import CreateEncoderConfigurationRequestTypeDef


def get_value() -> CreateEncoderConfigurationRequestTypeDef:
    return {
        "name": ...,
    }


# CreateEncoderConfigurationRequestTypeDef definition

class CreateEncoderConfigurationRequestTypeDef(TypedDict):
    name: NotRequired[str],
    video: NotRequired[VideoTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: VideoTypeDef](./type_defs.md#videotypedef) 
## EncoderConfigurationTypeDef

```python
# EncoderConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import EncoderConfigurationTypeDef


def get_value() -> EncoderConfigurationTypeDef:
    return {
        "arn": ...,
    }


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
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIngestConfigurationResponseTypeDef

```python
# CreateIngestConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import CreateIngestConfigurationResponseTypeDef


def get_value() -> CreateIngestConfigurationResponseTypeDef:
    return {
        "ingestConfiguration": ...,
    }


# CreateIngestConfigurationResponseTypeDef definition

class CreateIngestConfigurationResponseTypeDef(TypedDict):
    ingestConfiguration: IngestConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestConfigurationTypeDef](./type_defs.md#ingestconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIngestConfigurationResponseTypeDef

```python
# GetIngestConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import GetIngestConfigurationResponseTypeDef


def get_value() -> GetIngestConfigurationResponseTypeDef:
    return {
        "ingestConfiguration": ...,
    }


# GetIngestConfigurationResponseTypeDef definition

class GetIngestConfigurationResponseTypeDef(TypedDict):
    ingestConfiguration: IngestConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestConfigurationTypeDef](./type_defs.md#ingestconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIngestConfigurationResponseTypeDef

```python
# UpdateIngestConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import UpdateIngestConfigurationResponseTypeDef


def get_value() -> UpdateIngestConfigurationResponseTypeDef:
    return {
        "ingestConfiguration": ...,
    }


# UpdateIngestConfigurationResponseTypeDef definition

class UpdateIngestConfigurationResponseTypeDef(TypedDict):
    ingestConfiguration: IngestConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestConfigurationTypeDef](./type_defs.md#ingestconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateParticipantTokenResponseTypeDef

```python
# CreateParticipantTokenResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import CreateParticipantTokenResponseTypeDef


def get_value() -> CreateParticipantTokenResponseTypeDef:
    return {
        "participantToken": ...,
    }


# CreateParticipantTokenResponseTypeDef definition

class CreateParticipantTokenResponseTypeDef(TypedDict):
    participantToken: ParticipantTokenTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParticipantTokenTypeDef](./type_defs.md#participanttokentypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStorageConfigurationRequestTypeDef

```python
# CreateStorageConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import CreateStorageConfigurationRequestTypeDef


def get_value() -> CreateStorageConfigurationRequestTypeDef:
    return {
        "s3": ...,
    }


# CreateStorageConfigurationRequestTypeDef definition

class CreateStorageConfigurationRequestTypeDef(TypedDict):
    s3: S3StorageConfigurationTypeDef,  # (1)
    name: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: S3StorageConfigurationTypeDef](./type_defs.md#s3storageconfigurationtypedef) 
## StorageConfigurationSummaryTypeDef

```python
# StorageConfigurationSummaryTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import StorageConfigurationSummaryTypeDef


def get_value() -> StorageConfigurationSummaryTypeDef:
    return {
        "arn": ...,
    }


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
# StorageConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import StorageConfigurationTypeDef


def get_value() -> StorageConfigurationTypeDef:
    return {
        "arn": ...,
    }


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
# DestinationDetailTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import DestinationDetailTypeDef


def get_value() -> DestinationDetailTypeDef:
    return {
        "s3": ...,
    }


# DestinationDetailTypeDef definition

class DestinationDetailTypeDef(TypedDict):
    s3: NotRequired[S3DetailTypeDef],  # (1)
```

1. See [:material-code-braces: S3DetailTypeDef](./type_defs.md#s3detailtypedef) 
## ListEncoderConfigurationsResponseTypeDef

```python
# ListEncoderConfigurationsResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ListEncoderConfigurationsResponseTypeDef


def get_value() -> ListEncoderConfigurationsResponseTypeDef:
    return {
        "encoderConfigurations": ...,
    }


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
# ListParticipantEventsResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ListParticipantEventsResponseTypeDef


def get_value() -> ListParticipantEventsResponseTypeDef:
    return {
        "events": ...,
    }


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
# GetParticipantResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import GetParticipantResponseTypeDef


def get_value() -> GetParticipantResponseTypeDef:
    return {
        "participant": ...,
    }


# GetParticipantResponseTypeDef definition

class GetParticipantResponseTypeDef(TypedDict):
    participant: ParticipantTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParticipantTypeDef](./type_defs.md#participanttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPublicKeyResponseTypeDef

```python
# GetPublicKeyResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import GetPublicKeyResponseTypeDef


def get_value() -> GetPublicKeyResponseTypeDef:
    return {
        "publicKey": ...,
    }


# GetPublicKeyResponseTypeDef definition

class GetPublicKeyResponseTypeDef(TypedDict):
    publicKey: PublicKeyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PublicKeyTypeDef](./type_defs.md#publickeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportPublicKeyResponseTypeDef

```python
# ImportPublicKeyResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ImportPublicKeyResponseTypeDef


def get_value() -> ImportPublicKeyResponseTypeDef:
    return {
        "publicKey": ...,
    }


# ImportPublicKeyResponseTypeDef definition

class ImportPublicKeyResponseTypeDef(TypedDict):
    publicKey: PublicKeyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PublicKeyTypeDef](./type_defs.md#publickeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStageSessionResponseTypeDef

```python
# GetStageSessionResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import GetStageSessionResponseTypeDef


def get_value() -> GetStageSessionResponseTypeDef:
    return {
        "stageSession": ...,
    }


# GetStageSessionResponseTypeDef definition

class GetStageSessionResponseTypeDef(TypedDict):
    stageSession: StageSessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StageSessionTypeDef](./type_defs.md#stagesessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIngestConfigurationsResponseTypeDef

```python
# ListIngestConfigurationsResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ListIngestConfigurationsResponseTypeDef


def get_value() -> ListIngestConfigurationsResponseTypeDef:
    return {
        "ingestConfigurations": ...,
    }


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
# LayoutConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import LayoutConfigurationTypeDef


def get_value() -> LayoutConfigurationTypeDef:
    return {
        "grid": ...,
    }


# LayoutConfigurationTypeDef definition

class LayoutConfigurationTypeDef(TypedDict):
    grid: NotRequired[GridConfigurationTypeDef],  # (1)
    pip: NotRequired[PipConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: GridConfigurationTypeDef](./type_defs.md#gridconfigurationtypedef) 
2. See [:material-code-braces: PipConfigurationTypeDef](./type_defs.md#pipconfigurationtypedef) 
## ListIngestConfigurationsRequestPaginateTypeDef

```python
# ListIngestConfigurationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ListIngestConfigurationsRequestPaginateTypeDef


def get_value() -> ListIngestConfigurationsRequestPaginateTypeDef:
    return {
        "filterByStageArn": ...,
    }


# ListIngestConfigurationsRequestPaginateTypeDef definition

class ListIngestConfigurationsRequestPaginateTypeDef(TypedDict):
    filterByStageArn: NotRequired[str],
    filterByState: NotRequired[IngestConfigurationStateType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: IngestConfigurationStateType](./literals.md#ingestconfigurationstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPublicKeysRequestPaginateTypeDef

```python
# ListPublicKeysRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ListPublicKeysRequestPaginateTypeDef


def get_value() -> ListPublicKeysRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListPublicKeysRequestPaginateTypeDef definition

class ListPublicKeysRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListParticipantsResponseTypeDef

```python
# ListParticipantsResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ListParticipantsResponseTypeDef


def get_value() -> ListParticipantsResponseTypeDef:
    return {
        "participants": ...,
    }


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
# ListPublicKeysResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ListPublicKeysResponseTypeDef


def get_value() -> ListPublicKeysResponseTypeDef:
    return {
        "publicKeys": ...,
    }


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
# ListStageSessionsResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ListStageSessionsResponseTypeDef


def get_value() -> ListStageSessionsResponseTypeDef:
    return {
        "stageSessions": ...,
    }


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
# ListStagesResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ListStagesResponseTypeDef


def get_value() -> ListStagesResponseTypeDef:
    return {
        "stages": ...,
    }


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
# S3DestinationConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import S3DestinationConfigurationOutputTypeDef


def get_value() -> S3DestinationConfigurationOutputTypeDef:
    return {
        "storageConfigurationArn": ...,
    }


# S3DestinationConfigurationOutputTypeDef definition

class S3DestinationConfigurationOutputTypeDef(TypedDict):
    storageConfigurationArn: str,
    encoderConfigurationArns: List[str],
    recordingConfiguration: NotRequired[RecordingConfigurationTypeDef],  # (1)
    thumbnailConfigurations: NotRequired[List[CompositionThumbnailConfigurationOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: RecordingConfigurationTypeDef](./type_defs.md#recordingconfigurationtypedef) 
2. See [:material-code-braces: CompositionThumbnailConfigurationOutputTypeDef](./type_defs.md#compositionthumbnailconfigurationoutputtypedef) 
## StageTypeDef

```python
# StageTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import StageTypeDef


def get_value() -> StageTypeDef:
    return {
        "arn": ...,
    }


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
# ListCompositionsResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ListCompositionsResponseTypeDef


def get_value() -> ListCompositionsResponseTypeDef:
    return {
        "compositions": ...,
    }


# ListCompositionsResponseTypeDef definition

class ListCompositionsResponseTypeDef(TypedDict):
    compositions: List[CompositionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CompositionSummaryTypeDef](./type_defs.md#compositionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## S3DestinationConfigurationTypeDef

```python
# S3DestinationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import S3DestinationConfigurationTypeDef


def get_value() -> S3DestinationConfigurationTypeDef:
    return {
        "storageConfigurationArn": ...,
    }


# S3DestinationConfigurationTypeDef definition

class S3DestinationConfigurationTypeDef(TypedDict):
    storageConfigurationArn: str,
    encoderConfigurationArns: Sequence[str],
    recordingConfiguration: NotRequired[RecordingConfigurationTypeDef],  # (1)
    thumbnailConfigurations: NotRequired[Sequence[CompositionThumbnailConfigurationUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: RecordingConfigurationTypeDef](./type_defs.md#recordingconfigurationtypedef) 
2. See [:material-code-braces: CompositionThumbnailConfigurationTypeDef](./type_defs.md#compositionthumbnailconfigurationtypedef) [:material-code-braces: CompositionThumbnailConfigurationOutputTypeDef](./type_defs.md#compositionthumbnailconfigurationoutputtypedef) 
## CreateEncoderConfigurationResponseTypeDef

```python
# CreateEncoderConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import CreateEncoderConfigurationResponseTypeDef


def get_value() -> CreateEncoderConfigurationResponseTypeDef:
    return {
        "encoderConfiguration": ...,
    }


# CreateEncoderConfigurationResponseTypeDef definition

class CreateEncoderConfigurationResponseTypeDef(TypedDict):
    encoderConfiguration: EncoderConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EncoderConfigurationTypeDef](./type_defs.md#encoderconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEncoderConfigurationResponseTypeDef

```python
# GetEncoderConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import GetEncoderConfigurationResponseTypeDef


def get_value() -> GetEncoderConfigurationResponseTypeDef:
    return {
        "encoderConfiguration": ...,
    }


# GetEncoderConfigurationResponseTypeDef definition

class GetEncoderConfigurationResponseTypeDef(TypedDict):
    encoderConfiguration: EncoderConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EncoderConfigurationTypeDef](./type_defs.md#encoderconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStorageConfigurationsResponseTypeDef

```python
# ListStorageConfigurationsResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import ListStorageConfigurationsResponseTypeDef


def get_value() -> ListStorageConfigurationsResponseTypeDef:
    return {
        "storageConfigurations": ...,
    }


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
# CreateStorageConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import CreateStorageConfigurationResponseTypeDef


def get_value() -> CreateStorageConfigurationResponseTypeDef:
    return {
        "storageConfiguration": ...,
    }


# CreateStorageConfigurationResponseTypeDef definition

class CreateStorageConfigurationResponseTypeDef(TypedDict):
    storageConfiguration: StorageConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStorageConfigurationResponseTypeDef

```python
# GetStorageConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import GetStorageConfigurationResponseTypeDef


def get_value() -> GetStorageConfigurationResponseTypeDef:
    return {
        "storageConfiguration": ...,
    }


# GetStorageConfigurationResponseTypeDef definition

class GetStorageConfigurationResponseTypeDef(TypedDict):
    storageConfiguration: StorageConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DestinationConfigurationOutputTypeDef

```python
# DestinationConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import DestinationConfigurationOutputTypeDef


def get_value() -> DestinationConfigurationOutputTypeDef:
    return {
        "name": ...,
    }


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
# CreateStageResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import CreateStageResponseTypeDef


def get_value() -> CreateStageResponseTypeDef:
    return {
        "stage": ...,
    }


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
# GetStageResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import GetStageResponseTypeDef


def get_value() -> GetStageResponseTypeDef:
    return {
        "stage": ...,
    }


# GetStageResponseTypeDef definition

class GetStageResponseTypeDef(TypedDict):
    stage: StageTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StageTypeDef](./type_defs.md#stagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateStageResponseTypeDef

```python
# UpdateStageResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import UpdateStageResponseTypeDef


def get_value() -> UpdateStageResponseTypeDef:
    return {
        "stage": ...,
    }


# UpdateStageResponseTypeDef definition

class UpdateStageResponseTypeDef(TypedDict):
    stage: StageTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StageTypeDef](./type_defs.md#stagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStageRequestTypeDef

```python
# CreateStageRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import CreateStageRequestTypeDef


def get_value() -> CreateStageRequestTypeDef:
    return {
        "name": ...,
    }


# CreateStageRequestTypeDef definition

class CreateStageRequestTypeDef(TypedDict):
    name: NotRequired[str],
    participantTokenConfigurations: NotRequired[Sequence[ParticipantTokenConfigurationTypeDef]],  # (1)
    tags: NotRequired[Mapping[str, str]],
    autoParticipantRecordingConfiguration: NotRequired[AutoParticipantRecordingConfigurationUnionTypeDef],  # (2)
```

1. See [:material-code-braces: ParticipantTokenConfigurationTypeDef](./type_defs.md#participanttokenconfigurationtypedef) 
2. See [:material-code-braces: AutoParticipantRecordingConfigurationTypeDef](./type_defs.md#autoparticipantrecordingconfigurationtypedef) [:material-code-braces: AutoParticipantRecordingConfigurationOutputTypeDef](./type_defs.md#autoparticipantrecordingconfigurationoutputtypedef) 
## UpdateStageRequestTypeDef

```python
# UpdateStageRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import UpdateStageRequestTypeDef


def get_value() -> UpdateStageRequestTypeDef:
    return {
        "arn": ...,
    }


# UpdateStageRequestTypeDef definition

class UpdateStageRequestTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    autoParticipantRecordingConfiguration: NotRequired[AutoParticipantRecordingConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: AutoParticipantRecordingConfigurationTypeDef](./type_defs.md#autoparticipantrecordingconfigurationtypedef) [:material-code-braces: AutoParticipantRecordingConfigurationOutputTypeDef](./type_defs.md#autoparticipantrecordingconfigurationoutputtypedef) 
## DestinationTypeDef

```python
# DestinationTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import DestinationTypeDef


def get_value() -> DestinationTypeDef:
    return {
        "id": ...,
    }


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
# DestinationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import DestinationConfigurationTypeDef


def get_value() -> DestinationConfigurationTypeDef:
    return {
        "name": ...,
    }


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
# CompositionTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import CompositionTypeDef


def get_value() -> CompositionTypeDef:
    return {
        "arn": ...,
    }


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
# GetCompositionResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import GetCompositionResponseTypeDef


def get_value() -> GetCompositionResponseTypeDef:
    return {
        "composition": ...,
    }


# GetCompositionResponseTypeDef definition

class GetCompositionResponseTypeDef(TypedDict):
    composition: CompositionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CompositionTypeDef](./type_defs.md#compositiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartCompositionResponseTypeDef

```python
# StartCompositionResponseTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import StartCompositionResponseTypeDef


def get_value() -> StartCompositionResponseTypeDef:
    return {
        "composition": ...,
    }


# StartCompositionResponseTypeDef definition

class StartCompositionResponseTypeDef(TypedDict):
    composition: CompositionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CompositionTypeDef](./type_defs.md#compositiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartCompositionRequestTypeDef

```python
# StartCompositionRequestTypeDef TypedDict usage example

from types_aiobotocore_ivs_realtime.type_defs import StartCompositionRequestTypeDef


def get_value() -> StartCompositionRequestTypeDef:
    return {
        "stageArn": ...,
    }


# StartCompositionRequestTypeDef definition

class StartCompositionRequestTypeDef(TypedDict):
    stageArn: str,
    destinations: Sequence[DestinationConfigurationUnionTypeDef],  # (1)
    idempotencyToken: NotRequired[str],
    layout: NotRequired[LayoutConfigurationTypeDef],  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) [:material-code-braces: DestinationConfigurationOutputTypeDef](./type_defs.md#destinationconfigurationoutputtypedef) 
2. See [:material-code-braces: LayoutConfigurationTypeDef](./type_defs.md#layoutconfigurationtypedef) 
