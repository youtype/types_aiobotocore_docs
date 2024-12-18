# Type definitions

> [Index](../README.md) > [ChimeSDKMeetings](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ChimeSDKMeetings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#chimesdkmeetings)
    type annotations stubs module [types-aiobotocore-chime-sdk-meetings](https://pypi.org/project/types-aiobotocore-chime-sdk-meetings/).



## AttendeeCapabilitiesTypeDef

```python
# AttendeeCapabilitiesTypeDef definition

class AttendeeCapabilitiesTypeDef(TypedDict):
    Audio: MediaCapabilitiesType,  # (1)
    Video: MediaCapabilitiesType,  # (1)
    Content: MediaCapabilitiesType,  # (1)
```

1. See [:material-code-brackets: MediaCapabilitiesType](./literals.md#mediacapabilitiestype) 
2. See [:material-code-brackets: MediaCapabilitiesType](./literals.md#mediacapabilitiestype) 
3. See [:material-code-brackets: MediaCapabilitiesType](./literals.md#mediacapabilitiestype) 
## AttendeeFeaturesTypeDef

```python
# AttendeeFeaturesTypeDef definition

class AttendeeFeaturesTypeDef(TypedDict):
    MaxCount: NotRequired[int],
```

## AttendeeIdItemTypeDef

```python
# AttendeeIdItemTypeDef definition

class AttendeeIdItemTypeDef(TypedDict):
    AttendeeId: str,
```

## AudioFeaturesTypeDef

```python
# AudioFeaturesTypeDef definition

class AudioFeaturesTypeDef(TypedDict):
    EchoReduction: NotRequired[MeetingFeatureStatusType],  # (1)
```

1. See [:material-code-brackets: MeetingFeatureStatusType](./literals.md#meetingfeaturestatustype) 
## CreateAttendeeErrorTypeDef

```python
# CreateAttendeeErrorTypeDef definition

class CreateAttendeeErrorTypeDef(TypedDict):
    ExternalUserId: NotRequired[str],
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
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

## ContentFeaturesTypeDef

```python
# ContentFeaturesTypeDef definition

class ContentFeaturesTypeDef(TypedDict):
    MaxResolution: NotRequired[ContentResolutionType],  # (1)
```

1. See [:material-code-brackets: ContentResolutionType](./literals.md#contentresolutiontype) 
## NotificationsConfigurationTypeDef

```python
# NotificationsConfigurationTypeDef definition

class NotificationsConfigurationTypeDef(TypedDict):
    LambdaFunctionArn: NotRequired[str],
    SnsTopicArn: NotRequired[str],
    SqsQueueArn: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## DeleteAttendeeRequestRequestTypeDef

```python
# DeleteAttendeeRequestRequestTypeDef definition

class DeleteAttendeeRequestRequestTypeDef(TypedDict):
    MeetingId: str,
    AttendeeId: str,
```

## DeleteMeetingRequestRequestTypeDef

```python
# DeleteMeetingRequestRequestTypeDef definition

class DeleteMeetingRequestRequestTypeDef(TypedDict):
    MeetingId: str,
```

## EngineTranscribeMedicalSettingsTypeDef

```python
# EngineTranscribeMedicalSettingsTypeDef definition

class EngineTranscribeMedicalSettingsTypeDef(TypedDict):
    LanguageCode: TranscribeMedicalLanguageCodeType,  # (1)
    Specialty: TranscribeMedicalSpecialtyType,  # (2)
    Type: TranscribeMedicalTypeType,  # (3)
    VocabularyName: NotRequired[str],
    Region: NotRequired[TranscribeMedicalRegionType],  # (4)
    ContentIdentificationType: NotRequired[TranscribeMedicalContentIdentificationTypeType],  # (5)
```

1. See [:material-code-brackets: TranscribeMedicalLanguageCodeType](./literals.md#transcribemedicallanguagecodetype) 
2. See [:material-code-brackets: TranscribeMedicalSpecialtyType](./literals.md#transcribemedicalspecialtytype) 
3. See [:material-code-brackets: TranscribeMedicalTypeType](./literals.md#transcribemedicaltypetype) 
4. See [:material-code-brackets: TranscribeMedicalRegionType](./literals.md#transcribemedicalregiontype) 
5. See [:material-code-brackets: TranscribeMedicalContentIdentificationTypeType](./literals.md#transcribemedicalcontentidentificationtypetype) 
## EngineTranscribeSettingsTypeDef

```python
# EngineTranscribeSettingsTypeDef definition

class EngineTranscribeSettingsTypeDef(TypedDict):
    LanguageCode: NotRequired[TranscribeLanguageCodeType],  # (1)
    VocabularyFilterMethod: NotRequired[TranscribeVocabularyFilterMethodType],  # (2)
    VocabularyFilterName: NotRequired[str],
    VocabularyName: NotRequired[str],
    Region: NotRequired[TranscribeRegionType],  # (3)
    EnablePartialResultsStabilization: NotRequired[bool],
    PartialResultsStability: NotRequired[TranscribePartialResultsStabilityType],  # (4)
    ContentIdentificationType: NotRequired[TranscribeContentIdentificationTypeType],  # (5)
    ContentRedactionType: NotRequired[TranscribeContentRedactionTypeType],  # (6)
    PiiEntityTypes: NotRequired[str],
    LanguageModelName: NotRequired[str],
    IdentifyLanguage: NotRequired[bool],
    LanguageOptions: NotRequired[str],
    PreferredLanguage: NotRequired[TranscribeLanguageCodeType],  # (1)
    VocabularyNames: NotRequired[str],
    VocabularyFilterNames: NotRequired[str],
```

1. See [:material-code-brackets: TranscribeLanguageCodeType](./literals.md#transcribelanguagecodetype) 
2. See [:material-code-brackets: TranscribeVocabularyFilterMethodType](./literals.md#transcribevocabularyfiltermethodtype) 
3. See [:material-code-brackets: TranscribeRegionType](./literals.md#transcriberegiontype) 
4. See [:material-code-brackets: TranscribePartialResultsStabilityType](./literals.md#transcribepartialresultsstabilitytype) 
5. See [:material-code-brackets: TranscribeContentIdentificationTypeType](./literals.md#transcribecontentidentificationtypetype) 
6. See [:material-code-brackets: TranscribeContentRedactionTypeType](./literals.md#transcribecontentredactiontypetype) 
7. See [:material-code-brackets: TranscribeLanguageCodeType](./literals.md#transcribelanguagecodetype) 
## GetAttendeeRequestRequestTypeDef

```python
# GetAttendeeRequestRequestTypeDef definition

class GetAttendeeRequestRequestTypeDef(TypedDict):
    MeetingId: str,
    AttendeeId: str,
```

## GetMeetingRequestRequestTypeDef

```python
# GetMeetingRequestRequestTypeDef definition

class GetMeetingRequestRequestTypeDef(TypedDict):
    MeetingId: str,
```

## ListAttendeesRequestRequestTypeDef

```python
# ListAttendeesRequestRequestTypeDef definition

class ListAttendeesRequestRequestTypeDef(TypedDict):
    MeetingId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## MediaPlacementTypeDef

```python
# MediaPlacementTypeDef definition

class MediaPlacementTypeDef(TypedDict):
    AudioHostUrl: NotRequired[str],
    AudioFallbackUrl: NotRequired[str],
    SignalingUrl: NotRequired[str],
    TurnControlUrl: NotRequired[str],
    ScreenDataUrl: NotRequired[str],
    ScreenViewingUrl: NotRequired[str],
    ScreenSharingUrl: NotRequired[str],
    EventIngestionUrl: NotRequired[str],
```

## VideoFeaturesTypeDef

```python
# VideoFeaturesTypeDef definition

class VideoFeaturesTypeDef(TypedDict):
    MaxResolution: NotRequired[VideoResolutionType],  # (1)
```

1. See [:material-code-brackets: VideoResolutionType](./literals.md#videoresolutiontype) 
## StopMeetingTranscriptionRequestRequestTypeDef

```python
# StopMeetingTranscriptionRequestRequestTypeDef definition

class StopMeetingTranscriptionRequestRequestTypeDef(TypedDict):
    MeetingId: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## AttendeeTypeDef

```python
# AttendeeTypeDef definition

class AttendeeTypeDef(TypedDict):
    ExternalUserId: NotRequired[str],
    AttendeeId: NotRequired[str],
    JoinToken: NotRequired[str],
    Capabilities: NotRequired[AttendeeCapabilitiesTypeDef],  # (1)
```

1. See [:material-code-braces: AttendeeCapabilitiesTypeDef](./type_defs.md#attendeecapabilitiestypedef) 
## CreateAttendeeRequestItemTypeDef

```python
# CreateAttendeeRequestItemTypeDef definition

class CreateAttendeeRequestItemTypeDef(TypedDict):
    ExternalUserId: str,
    Capabilities: NotRequired[AttendeeCapabilitiesTypeDef],  # (1)
```

1. See [:material-code-braces: AttendeeCapabilitiesTypeDef](./type_defs.md#attendeecapabilitiestypedef) 
## CreateAttendeeRequestRequestTypeDef

```python
# CreateAttendeeRequestRequestTypeDef definition

class CreateAttendeeRequestRequestTypeDef(TypedDict):
    MeetingId: str,
    ExternalUserId: str,
    Capabilities: NotRequired[AttendeeCapabilitiesTypeDef],  # (1)
```

1. See [:material-code-braces: AttendeeCapabilitiesTypeDef](./type_defs.md#attendeecapabilitiestypedef) 
## UpdateAttendeeCapabilitiesRequestRequestTypeDef

```python
# UpdateAttendeeCapabilitiesRequestRequestTypeDef definition

class UpdateAttendeeCapabilitiesRequestRequestTypeDef(TypedDict):
    MeetingId: str,
    AttendeeId: str,
    Capabilities: AttendeeCapabilitiesTypeDef,  # (1)
```

1. See [:material-code-braces: AttendeeCapabilitiesTypeDef](./type_defs.md#attendeecapabilitiestypedef) 
## BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef

```python
# BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef definition

class BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef(TypedDict):
    MeetingId: str,
    ExcludedAttendeeIds: Sequence[AttendeeIdItemTypeDef],  # (1)
    Capabilities: AttendeeCapabilitiesTypeDef,  # (2)
```

1. See [:material-code-braces: AttendeeIdItemTypeDef](./type_defs.md#attendeeiditemtypedef) 
2. See [:material-code-braces: AttendeeCapabilitiesTypeDef](./type_defs.md#attendeecapabilitiestypedef) 
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
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TranscriptionConfigurationTypeDef

```python
# TranscriptionConfigurationTypeDef definition

class TranscriptionConfigurationTypeDef(TypedDict):
    EngineTranscribeSettings: NotRequired[EngineTranscribeSettingsTypeDef],  # (1)
    EngineTranscribeMedicalSettings: NotRequired[EngineTranscribeMedicalSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: EngineTranscribeSettingsTypeDef](./type_defs.md#enginetranscribesettingstypedef) 
2. See [:material-code-braces: EngineTranscribeMedicalSettingsTypeDef](./type_defs.md#enginetranscribemedicalsettingstypedef) 
## MeetingFeaturesConfigurationTypeDef

```python
# MeetingFeaturesConfigurationTypeDef definition

class MeetingFeaturesConfigurationTypeDef(TypedDict):
    Audio: NotRequired[AudioFeaturesTypeDef],  # (1)
    Video: NotRequired[VideoFeaturesTypeDef],  # (2)
    Content: NotRequired[ContentFeaturesTypeDef],  # (3)
    Attendee: NotRequired[AttendeeFeaturesTypeDef],  # (4)
```

1. See [:material-code-braces: AudioFeaturesTypeDef](./type_defs.md#audiofeaturestypedef) 
2. See [:material-code-braces: VideoFeaturesTypeDef](./type_defs.md#videofeaturestypedef) 
3. See [:material-code-braces: ContentFeaturesTypeDef](./type_defs.md#contentfeaturestypedef) 
4. See [:material-code-braces: AttendeeFeaturesTypeDef](./type_defs.md#attendeefeaturestypedef) 
## BatchCreateAttendeeResponseTypeDef

```python
# BatchCreateAttendeeResponseTypeDef definition

class BatchCreateAttendeeResponseTypeDef(TypedDict):
    Attendees: List[AttendeeTypeDef],  # (1)
    Errors: List[CreateAttendeeErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AttendeeTypeDef](./type_defs.md#attendeetypedef) 
2. See [:material-code-braces: CreateAttendeeErrorTypeDef](./type_defs.md#createattendeeerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAttendeeResponseTypeDef

```python
# CreateAttendeeResponseTypeDef definition

class CreateAttendeeResponseTypeDef(TypedDict):
    Attendee: AttendeeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttendeeTypeDef](./type_defs.md#attendeetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAttendeeResponseTypeDef

```python
# GetAttendeeResponseTypeDef definition

class GetAttendeeResponseTypeDef(TypedDict):
    Attendee: AttendeeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttendeeTypeDef](./type_defs.md#attendeetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAttendeesResponseTypeDef

```python
# ListAttendeesResponseTypeDef definition

class ListAttendeesResponseTypeDef(TypedDict):
    Attendees: List[AttendeeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AttendeeTypeDef](./type_defs.md#attendeetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAttendeeCapabilitiesResponseTypeDef

```python
# UpdateAttendeeCapabilitiesResponseTypeDef definition

class UpdateAttendeeCapabilitiesResponseTypeDef(TypedDict):
    Attendee: AttendeeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttendeeTypeDef](./type_defs.md#attendeetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchCreateAttendeeRequestRequestTypeDef

```python
# BatchCreateAttendeeRequestRequestTypeDef definition

class BatchCreateAttendeeRequestRequestTypeDef(TypedDict):
    MeetingId: str,
    Attendees: Sequence[CreateAttendeeRequestItemTypeDef],  # (1)
```

1. See [:material-code-braces: CreateAttendeeRequestItemTypeDef](./type_defs.md#createattendeerequestitemtypedef) 
## StartMeetingTranscriptionRequestRequestTypeDef

```python
# StartMeetingTranscriptionRequestRequestTypeDef definition

class StartMeetingTranscriptionRequestRequestTypeDef(TypedDict):
    MeetingId: str,
    TranscriptionConfiguration: TranscriptionConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: TranscriptionConfigurationTypeDef](./type_defs.md#transcriptionconfigurationtypedef) 
## CreateMeetingRequestRequestTypeDef

```python
# CreateMeetingRequestRequestTypeDef definition

class CreateMeetingRequestRequestTypeDef(TypedDict):
    ClientRequestToken: str,
    MediaRegion: str,
    ExternalMeetingId: str,
    MeetingHostId: NotRequired[str],
    NotificationsConfiguration: NotRequired[NotificationsConfigurationTypeDef],  # (1)
    MeetingFeatures: NotRequired[MeetingFeaturesConfigurationTypeDef],  # (2)
    PrimaryMeetingId: NotRequired[str],
    TenantIds: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: NotificationsConfigurationTypeDef](./type_defs.md#notificationsconfigurationtypedef) 
2. See [:material-code-braces: MeetingFeaturesConfigurationTypeDef](./type_defs.md#meetingfeaturesconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateMeetingWithAttendeesRequestRequestTypeDef

```python
# CreateMeetingWithAttendeesRequestRequestTypeDef definition

class CreateMeetingWithAttendeesRequestRequestTypeDef(TypedDict):
    ClientRequestToken: str,
    MediaRegion: str,
    ExternalMeetingId: str,
    Attendees: Sequence[CreateAttendeeRequestItemTypeDef],  # (1)
    MeetingHostId: NotRequired[str],
    MeetingFeatures: NotRequired[MeetingFeaturesConfigurationTypeDef],  # (2)
    NotificationsConfiguration: NotRequired[NotificationsConfigurationTypeDef],  # (3)
    PrimaryMeetingId: NotRequired[str],
    TenantIds: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-braces: CreateAttendeeRequestItemTypeDef](./type_defs.md#createattendeerequestitemtypedef) 
2. See [:material-code-braces: MeetingFeaturesConfigurationTypeDef](./type_defs.md#meetingfeaturesconfigurationtypedef) 
3. See [:material-code-braces: NotificationsConfigurationTypeDef](./type_defs.md#notificationsconfigurationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## MeetingTypeDef

```python
# MeetingTypeDef definition

class MeetingTypeDef(TypedDict):
    MeetingId: NotRequired[str],
    MeetingHostId: NotRequired[str],
    ExternalMeetingId: NotRequired[str],
    MediaRegion: NotRequired[str],
    MediaPlacement: NotRequired[MediaPlacementTypeDef],  # (1)
    MeetingFeatures: NotRequired[MeetingFeaturesConfigurationTypeDef],  # (2)
    PrimaryMeetingId: NotRequired[str],
    TenantIds: NotRequired[List[str]],
    MeetingArn: NotRequired[str],
```

1. See [:material-code-braces: MediaPlacementTypeDef](./type_defs.md#mediaplacementtypedef) 
2. See [:material-code-braces: MeetingFeaturesConfigurationTypeDef](./type_defs.md#meetingfeaturesconfigurationtypedef) 
## CreateMeetingResponseTypeDef

```python
# CreateMeetingResponseTypeDef definition

class CreateMeetingResponseTypeDef(TypedDict):
    Meeting: MeetingTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MeetingTypeDef](./type_defs.md#meetingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMeetingWithAttendeesResponseTypeDef

```python
# CreateMeetingWithAttendeesResponseTypeDef definition

class CreateMeetingWithAttendeesResponseTypeDef(TypedDict):
    Meeting: MeetingTypeDef,  # (1)
    Attendees: List[AttendeeTypeDef],  # (2)
    Errors: List[CreateAttendeeErrorTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: MeetingTypeDef](./type_defs.md#meetingtypedef) 
2. See [:material-code-braces: AttendeeTypeDef](./type_defs.md#attendeetypedef) 
3. See [:material-code-braces: CreateAttendeeErrorTypeDef](./type_defs.md#createattendeeerrortypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMeetingResponseTypeDef

```python
# GetMeetingResponseTypeDef definition

class GetMeetingResponseTypeDef(TypedDict):
    Meeting: MeetingTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MeetingTypeDef](./type_defs.md#meetingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
