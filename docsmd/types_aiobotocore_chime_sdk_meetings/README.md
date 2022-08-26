# ChimeSDKMeetings module

> [Index](../README.md) > ChimeSDKMeetings


!!! note ""

    Auto-generated documentation for [ChimeSDKMeetings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
    type annotations stubs module [types-aiobotocore-chime-sdk-meetings](https://pypi.org/project/types-aiobotocore-chime-sdk-meetings/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `ChimeSDKMeetings` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[chime-sdk-meetings]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[chime-sdk-meetings]'


# standalone installation
python -m pip install types-aiobotocore-chime-sdk-meetings
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-chime-sdk-meetings
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ChimeSDKMeetingsClient

Type annotations and code completion for  `#!python session.create_client("chime-sdk-meetings")` as [ChimeSDKMeetingsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_chime_sdk_meetings.client import ChimeSDKMeetingsClient


session = get_session()
async with session.create_client("chime-sdk-meetings") as client:
    client: ChimeSDKMeetingsClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_chime_sdk_meetings.literals import MediaCapabilitiesType

def get_value() -> MediaCapabilitiesType:
    return "None"
```

- [MediaCapabilitiesType](./literals.md#mediacapabilitiestype)
- [MeetingFeatureStatusType](./literals.md#meetingfeaturestatustype)
- [TranscribeContentIdentificationTypeType](./literals.md#transcribecontentidentificationtypetype)
- [TranscribeContentRedactionTypeType](./literals.md#transcribecontentredactiontypetype)
- [TranscribeLanguageCodeType](./literals.md#transcribelanguagecodetype)
- [TranscribeMedicalContentIdentificationTypeType](./literals.md#transcribemedicalcontentidentificationtypetype)
- [TranscribeMedicalLanguageCodeType](./literals.md#transcribemedicallanguagecodetype)
- [TranscribeMedicalRegionType](./literals.md#transcribemedicalregiontype)
- [TranscribeMedicalSpecialtyType](./literals.md#transcribemedicalspecialtytype)
- [TranscribeMedicalTypeType](./literals.md#transcribemedicaltypetype)
- [TranscribePartialResultsStabilityType](./literals.md#transcribepartialresultsstabilitytype)
- [TranscribeRegionType](./literals.md#transcriberegiontype)
- [TranscribeVocabularyFilterMethodType](./literals.md#transcribevocabularyfiltermethodtype)
- [ChimeSDKMeetingsServiceName](./literals.md#chimesdkmeetingsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_chime_sdk_meetings.type_defs import AttendeeCapabilitiesTypeDef

def get_value() -> AttendeeCapabilitiesTypeDef:
    return {
        "Audio": ...,
        "Video": ...,
        "Content": ...,
    }
```

- [AttendeeCapabilitiesTypeDef](./type_defs.md#attendeecapabilitiestypedef)
- [AttendeeIdItemTypeDef](./type_defs.md#attendeeiditemtypedef)
- [AudioFeaturesTypeDef](./type_defs.md#audiofeaturestypedef)
- [CreateAttendeeErrorTypeDef](./type_defs.md#createattendeeerrortypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [NotificationsConfigurationTypeDef](./type_defs.md#notificationsconfigurationtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [DeleteAttendeeRequestRequestTypeDef](./type_defs.md#deleteattendeerequestrequesttypedef)
- [DeleteMeetingRequestRequestTypeDef](./type_defs.md#deletemeetingrequestrequesttypedef)
- [EngineTranscribeMedicalSettingsTypeDef](./type_defs.md#enginetranscribemedicalsettingstypedef)
- [EngineTranscribeSettingsTypeDef](./type_defs.md#enginetranscribesettingstypedef)
- [GetAttendeeRequestRequestTypeDef](./type_defs.md#getattendeerequestrequesttypedef)
- [GetMeetingRequestRequestTypeDef](./type_defs.md#getmeetingrequestrequesttypedef)
- [ListAttendeesRequestRequestTypeDef](./type_defs.md#listattendeesrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [MediaPlacementTypeDef](./type_defs.md#mediaplacementtypedef)
- [StopMeetingTranscriptionRequestRequestTypeDef](./type_defs.md#stopmeetingtranscriptionrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [AttendeeTypeDef](./type_defs.md#attendeetypedef)
- [CreateAttendeeRequestItemTypeDef](./type_defs.md#createattendeerequestitemtypedef)
- [CreateAttendeeRequestRequestTypeDef](./type_defs.md#createattendeerequestrequesttypedef)
- [UpdateAttendeeCapabilitiesRequestRequestTypeDef](./type_defs.md#updateattendeecapabilitiesrequestrequesttypedef)
- [BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef](./type_defs.md#batchupdateattendeecapabilitiesexceptrequestrequesttypedef)
- [MeetingFeaturesConfigurationTypeDef](./type_defs.md#meetingfeaturesconfigurationtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [TranscriptionConfigurationTypeDef](./type_defs.md#transcriptionconfigurationtypedef)
- [BatchCreateAttendeeResponseTypeDef](./type_defs.md#batchcreateattendeeresponsetypedef)
- [CreateAttendeeResponseTypeDef](./type_defs.md#createattendeeresponsetypedef)
- [GetAttendeeResponseTypeDef](./type_defs.md#getattendeeresponsetypedef)
- [ListAttendeesResponseTypeDef](./type_defs.md#listattendeesresponsetypedef)
- [UpdateAttendeeCapabilitiesResponseTypeDef](./type_defs.md#updateattendeecapabilitiesresponsetypedef)
- [BatchCreateAttendeeRequestRequestTypeDef](./type_defs.md#batchcreateattendeerequestrequesttypedef)
- [CreateMeetingRequestRequestTypeDef](./type_defs.md#createmeetingrequestrequesttypedef)
- [CreateMeetingWithAttendeesRequestRequestTypeDef](./type_defs.md#createmeetingwithattendeesrequestrequesttypedef)
- [MeetingTypeDef](./type_defs.md#meetingtypedef)
- [StartMeetingTranscriptionRequestRequestTypeDef](./type_defs.md#startmeetingtranscriptionrequestrequesttypedef)
- [CreateMeetingResponseTypeDef](./type_defs.md#createmeetingresponsetypedef)
- [CreateMeetingWithAttendeesResponseTypeDef](./type_defs.md#createmeetingwithattendeesresponsetypedef)
- [GetMeetingResponseTypeDef](./type_defs.md#getmeetingresponsetypedef)

