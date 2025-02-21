# Type definitions

> [Index](../README.md) > [Chime](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Chime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#chime)
    type annotations stubs module [types-aiobotocore-chime](https://pypi.org/project/types-aiobotocore-chime/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_chime.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## TerminationUnionTypeDef

```python
# TerminationUnionTypeDef Union usage example

from types_aiobotocore_chime.type_defs import TerminationUnionTypeDef


def get_value() -> TerminationUnionTypeDef:
    return ...


# TerminationUnionTypeDef definition

TerminationUnionTypeDef = Union[
    TerminationTypeDef,  # (1)
    TerminationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TerminationTypeDef](./type_defs.md#terminationtypedef) 
2. See [:material-code-braces: TerminationOutputTypeDef](./type_defs.md#terminationoutputtypedef) 

## EmergencyCallingConfigurationUnionTypeDef

```python
# EmergencyCallingConfigurationUnionTypeDef Union usage example

from types_aiobotocore_chime.type_defs import EmergencyCallingConfigurationUnionTypeDef


def get_value() -> EmergencyCallingConfigurationUnionTypeDef:
    return ...


# EmergencyCallingConfigurationUnionTypeDef definition

EmergencyCallingConfigurationUnionTypeDef = Union[
    EmergencyCallingConfigurationTypeDef,  # (1)
    EmergencyCallingConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EmergencyCallingConfigurationTypeDef](./type_defs.md#emergencycallingconfigurationtypedef) 
2. See [:material-code-braces: EmergencyCallingConfigurationOutputTypeDef](./type_defs.md#emergencycallingconfigurationoutputtypedef) 

## OriginationUnionTypeDef

```python
# OriginationUnionTypeDef Union usage example

from types_aiobotocore_chime.type_defs import OriginationUnionTypeDef


def get_value() -> OriginationUnionTypeDef:
    return ...


# OriginationUnionTypeDef definition

OriginationUnionTypeDef = Union[
    OriginationTypeDef,  # (1)
    OriginationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OriginationTypeDef](./type_defs.md#originationtypedef) 
2. See [:material-code-braces: OriginationOutputTypeDef](./type_defs.md#originationoutputtypedef) 

## StreamingConfigurationUnionTypeDef

```python
# StreamingConfigurationUnionTypeDef Union usage example

from types_aiobotocore_chime.type_defs import StreamingConfigurationUnionTypeDef


def get_value() -> StreamingConfigurationUnionTypeDef:
    return ...


# StreamingConfigurationUnionTypeDef definition

StreamingConfigurationUnionTypeDef = Union[
    StreamingConfigurationTypeDef,  # (1)
    StreamingConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: StreamingConfigurationTypeDef](./type_defs.md#streamingconfigurationtypedef) 
2. See [:material-code-braces: StreamingConfigurationOutputTypeDef](./type_defs.md#streamingconfigurationoutputtypedef) 

## ChimeSdkMeetingConfigurationUnionTypeDef

```python
# ChimeSdkMeetingConfigurationUnionTypeDef Union usage example

from types_aiobotocore_chime.type_defs import ChimeSdkMeetingConfigurationUnionTypeDef


def get_value() -> ChimeSdkMeetingConfigurationUnionTypeDef:
    return ...


# ChimeSdkMeetingConfigurationUnionTypeDef definition

ChimeSdkMeetingConfigurationUnionTypeDef = Union[
    ChimeSdkMeetingConfigurationTypeDef,  # (1)
    ChimeSdkMeetingConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ChimeSdkMeetingConfigurationTypeDef](./type_defs.md#chimesdkmeetingconfigurationtypedef) 
2. See [:material-code-braces: ChimeSdkMeetingConfigurationOutputTypeDef](./type_defs.md#chimesdkmeetingconfigurationoutputtypedef) 



## AccountSettingsTypeDef

```python
# AccountSettingsTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import AccountSettingsTypeDef


def get_value() -> AccountSettingsTypeDef:
    return {
        "DisableRemoteControl": ...,
    }


# AccountSettingsTypeDef definition

class AccountSettingsTypeDef(TypedDict):
    DisableRemoteControl: NotRequired[bool],
    EnableDialOut: NotRequired[bool],
```

## SigninDelegateGroupTypeDef

```python
# SigninDelegateGroupTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import SigninDelegateGroupTypeDef


def get_value() -> SigninDelegateGroupTypeDef:
    return {
        "GroupName": ...,
    }


# SigninDelegateGroupTypeDef definition

class SigninDelegateGroupTypeDef(TypedDict):
    GroupName: NotRequired[str],
```

## AddressTypeDef

```python
# AddressTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import AddressTypeDef


def get_value() -> AddressTypeDef:
    return {
        "streetName": ...,
    }


# AddressTypeDef definition

class AddressTypeDef(TypedDict):
    streetName: NotRequired[str],
    streetSuffix: NotRequired[str],
    postDirectional: NotRequired[str],
    preDirectional: NotRequired[str],
    streetNumber: NotRequired[str],
    city: NotRequired[str],
    state: NotRequired[str],
    postalCode: NotRequired[str],
    postalCodePlus4: NotRequired[str],
    country: NotRequired[str],
```

## AlexaForBusinessMetadataTypeDef

```python
# AlexaForBusinessMetadataTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import AlexaForBusinessMetadataTypeDef


def get_value() -> AlexaForBusinessMetadataTypeDef:
    return {
        "IsAlexaForBusinessEnabled": ...,
    }


# AlexaForBusinessMetadataTypeDef definition

class AlexaForBusinessMetadataTypeDef(TypedDict):
    IsAlexaForBusinessEnabled: NotRequired[bool],
    AlexaForBusinessRoomArn: NotRequired[str],
```

## IdentityTypeDef

```python
# IdentityTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import IdentityTypeDef


def get_value() -> IdentityTypeDef:
    return {
        "Arn": ...,
    }


# IdentityTypeDef definition

class IdentityTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
```

## ChannelRetentionSettingsTypeDef

```python
# ChannelRetentionSettingsTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ChannelRetentionSettingsTypeDef


def get_value() -> ChannelRetentionSettingsTypeDef:
    return {
        "RetentionDays": ...,
    }


# ChannelRetentionSettingsTypeDef definition

class ChannelRetentionSettingsTypeDef(TypedDict):
    RetentionDays: NotRequired[int],
```

## AppInstanceStreamingConfigurationTypeDef

```python
# AppInstanceStreamingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import AppInstanceStreamingConfigurationTypeDef


def get_value() -> AppInstanceStreamingConfigurationTypeDef:
    return {
        "AppInstanceDataType": ...,
    }


# AppInstanceStreamingConfigurationTypeDef definition

class AppInstanceStreamingConfigurationTypeDef(TypedDict):
    AppInstanceDataType: AppInstanceDataTypeType,  # (1)
    ResourceArn: str,
```

1. See [:material-code-brackets: AppInstanceDataTypeType](./literals.md#appinstancedatatypetype) 
## AppInstanceSummaryTypeDef

```python
# AppInstanceSummaryTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import AppInstanceSummaryTypeDef


def get_value() -> AppInstanceSummaryTypeDef:
    return {
        "AppInstanceArn": ...,
    }


# AppInstanceSummaryTypeDef definition

class AppInstanceSummaryTypeDef(TypedDict):
    AppInstanceArn: NotRequired[str],
    Name: NotRequired[str],
    Metadata: NotRequired[str],
```

## AppInstanceTypeDef

```python
# AppInstanceTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import AppInstanceTypeDef


def get_value() -> AppInstanceTypeDef:
    return {
        "AppInstanceArn": ...,
    }


# AppInstanceTypeDef definition

class AppInstanceTypeDef(TypedDict):
    AppInstanceArn: NotRequired[str],
    Name: NotRequired[str],
    Metadata: NotRequired[str],
    CreatedTimestamp: NotRequired[datetime],
    LastUpdatedTimestamp: NotRequired[datetime],
```

## AppInstanceUserMembershipSummaryTypeDef

```python
# AppInstanceUserMembershipSummaryTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import AppInstanceUserMembershipSummaryTypeDef


def get_value() -> AppInstanceUserMembershipSummaryTypeDef:
    return {
        "Type": ...,
    }


# AppInstanceUserMembershipSummaryTypeDef definition

class AppInstanceUserMembershipSummaryTypeDef(TypedDict):
    Type: NotRequired[ChannelMembershipTypeType],  # (1)
    ReadMarkerTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: ChannelMembershipTypeType](./literals.md#channelmembershiptypetype) 
## AppInstanceUserSummaryTypeDef

```python
# AppInstanceUserSummaryTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import AppInstanceUserSummaryTypeDef


def get_value() -> AppInstanceUserSummaryTypeDef:
    return {
        "AppInstanceUserArn": ...,
    }


# AppInstanceUserSummaryTypeDef definition

class AppInstanceUserSummaryTypeDef(TypedDict):
    AppInstanceUserArn: NotRequired[str],
    Name: NotRequired[str],
    Metadata: NotRequired[str],
```

## AppInstanceUserTypeDef

```python
# AppInstanceUserTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import AppInstanceUserTypeDef


def get_value() -> AppInstanceUserTypeDef:
    return {
        "AppInstanceUserArn": ...,
    }


# AppInstanceUserTypeDef definition

class AppInstanceUserTypeDef(TypedDict):
    AppInstanceUserArn: NotRequired[str],
    Name: NotRequired[str],
    CreatedTimestamp: NotRequired[datetime],
    Metadata: NotRequired[str],
    LastUpdatedTimestamp: NotRequired[datetime],
```

## AudioArtifactsConfigurationTypeDef

```python
# AudioArtifactsConfigurationTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import AudioArtifactsConfigurationTypeDef


def get_value() -> AudioArtifactsConfigurationTypeDef:
    return {
        "MuxType": ...,
    }


# AudioArtifactsConfigurationTypeDef definition

class AudioArtifactsConfigurationTypeDef(TypedDict):
    MuxType: AudioMuxTypeType,  # (1)
```

1. See [:material-code-brackets: AudioMuxTypeType](./literals.md#audiomuxtypetype) 
## ContentArtifactsConfigurationTypeDef

```python
# ContentArtifactsConfigurationTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ContentArtifactsConfigurationTypeDef


def get_value() -> ContentArtifactsConfigurationTypeDef:
    return {
        "State": ...,
    }


# ContentArtifactsConfigurationTypeDef definition

class ContentArtifactsConfigurationTypeDef(TypedDict):
    State: ArtifactsStateType,  # (1)
    MuxType: NotRequired[ContentMuxTypeType],  # (2)
```

1. See [:material-code-brackets: ArtifactsStateType](./literals.md#artifactsstatetype) 
2. See [:material-code-brackets: ContentMuxTypeType](./literals.md#contentmuxtypetype) 
## VideoArtifactsConfigurationTypeDef

```python
# VideoArtifactsConfigurationTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import VideoArtifactsConfigurationTypeDef


def get_value() -> VideoArtifactsConfigurationTypeDef:
    return {
        "State": ...,
    }


# VideoArtifactsConfigurationTypeDef definition

class VideoArtifactsConfigurationTypeDef(TypedDict):
    State: ArtifactsStateType,  # (1)
    MuxType: NotRequired[VideoMuxTypeType],  # (2)
```

1. See [:material-code-brackets: ArtifactsStateType](./literals.md#artifactsstatetype) 
2. See [:material-code-brackets: VideoMuxTypeType](./literals.md#videomuxtypetype) 
## AssociatePhoneNumberWithUserRequestTypeDef

```python
# AssociatePhoneNumberWithUserRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import AssociatePhoneNumberWithUserRequestTypeDef


def get_value() -> AssociatePhoneNumberWithUserRequestTypeDef:
    return {
        "AccountId": ...,
    }


# AssociatePhoneNumberWithUserRequestTypeDef definition

class AssociatePhoneNumberWithUserRequestTypeDef(TypedDict):
    AccountId: str,
    UserId: str,
    E164PhoneNumber: str,
```

## AssociatePhoneNumbersWithVoiceConnectorGroupRequestTypeDef

```python
# AssociatePhoneNumbersWithVoiceConnectorGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import AssociatePhoneNumbersWithVoiceConnectorGroupRequestTypeDef


def get_value() -> AssociatePhoneNumbersWithVoiceConnectorGroupRequestTypeDef:
    return {
        "VoiceConnectorGroupId": ...,
    }


# AssociatePhoneNumbersWithVoiceConnectorGroupRequestTypeDef definition

class AssociatePhoneNumbersWithVoiceConnectorGroupRequestTypeDef(TypedDict):
    VoiceConnectorGroupId: str,
    E164PhoneNumbers: Sequence[str],
    ForceAssociate: NotRequired[bool],
```

## PhoneNumberErrorTypeDef

```python
# PhoneNumberErrorTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PhoneNumberErrorTypeDef


def get_value() -> PhoneNumberErrorTypeDef:
    return {
        "PhoneNumberId": ...,
    }


# PhoneNumberErrorTypeDef definition

class PhoneNumberErrorTypeDef(TypedDict):
    PhoneNumberId: NotRequired[str],
    ErrorCode: NotRequired[ErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ResponseMetadataTypeDef


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

## AssociatePhoneNumbersWithVoiceConnectorRequestTypeDef

```python
# AssociatePhoneNumbersWithVoiceConnectorRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import AssociatePhoneNumbersWithVoiceConnectorRequestTypeDef


def get_value() -> AssociatePhoneNumbersWithVoiceConnectorRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# AssociatePhoneNumbersWithVoiceConnectorRequestTypeDef definition

class AssociatePhoneNumbersWithVoiceConnectorRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    E164PhoneNumbers: Sequence[str],
    ForceAssociate: NotRequired[bool],
```

## AttendeeTypeDef

```python
# AttendeeTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import AttendeeTypeDef


def get_value() -> AttendeeTypeDef:
    return {
        "ExternalUserId": ...,
    }


# AttendeeTypeDef definition

class AttendeeTypeDef(TypedDict):
    ExternalUserId: NotRequired[str],
    AttendeeId: NotRequired[str],
    JoinToken: NotRequired[str],
```

## CreateAttendeeErrorTypeDef

```python
# CreateAttendeeErrorTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateAttendeeErrorTypeDef


def get_value() -> CreateAttendeeErrorTypeDef:
    return {
        "ExternalUserId": ...,
    }


# CreateAttendeeErrorTypeDef definition

class CreateAttendeeErrorTypeDef(TypedDict):
    ExternalUserId: NotRequired[str],
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## BatchCreateChannelMembershipErrorTypeDef

```python
# BatchCreateChannelMembershipErrorTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import BatchCreateChannelMembershipErrorTypeDef


def get_value() -> BatchCreateChannelMembershipErrorTypeDef:
    return {
        "MemberArn": ...,
    }


# BatchCreateChannelMembershipErrorTypeDef definition

class BatchCreateChannelMembershipErrorTypeDef(TypedDict):
    MemberArn: NotRequired[str],
    ErrorCode: NotRequired[ErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## BatchCreateChannelMembershipRequestTypeDef

```python
# BatchCreateChannelMembershipRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import BatchCreateChannelMembershipRequestTypeDef


def get_value() -> BatchCreateChannelMembershipRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# BatchCreateChannelMembershipRequestTypeDef definition

class BatchCreateChannelMembershipRequestTypeDef(TypedDict):
    ChannelArn: str,
    MemberArns: Sequence[str],
    Type: NotRequired[ChannelMembershipTypeType],  # (1)
    ChimeBearer: NotRequired[str],
```

1. See [:material-code-brackets: ChannelMembershipTypeType](./literals.md#channelmembershiptypetype) 
## MembershipItemTypeDef

```python
# MembershipItemTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import MembershipItemTypeDef


def get_value() -> MembershipItemTypeDef:
    return {
        "MemberId": ...,
    }


# MembershipItemTypeDef definition

class MembershipItemTypeDef(TypedDict):
    MemberId: NotRequired[str],
    Role: NotRequired[RoomMembershipRoleType],  # (1)
```

1. See [:material-code-brackets: RoomMembershipRoleType](./literals.md#roommembershiproletype) 
## MemberErrorTypeDef

```python
# MemberErrorTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import MemberErrorTypeDef


def get_value() -> MemberErrorTypeDef:
    return {
        "MemberId": ...,
    }


# MemberErrorTypeDef definition

class MemberErrorTypeDef(TypedDict):
    MemberId: NotRequired[str],
    ErrorCode: NotRequired[ErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## BatchDeletePhoneNumberRequestTypeDef

```python
# BatchDeletePhoneNumberRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import BatchDeletePhoneNumberRequestTypeDef


def get_value() -> BatchDeletePhoneNumberRequestTypeDef:
    return {
        "PhoneNumberIds": ...,
    }


# BatchDeletePhoneNumberRequestTypeDef definition

class BatchDeletePhoneNumberRequestTypeDef(TypedDict):
    PhoneNumberIds: Sequence[str],
```

## BatchSuspendUserRequestTypeDef

```python
# BatchSuspendUserRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import BatchSuspendUserRequestTypeDef


def get_value() -> BatchSuspendUserRequestTypeDef:
    return {
        "AccountId": ...,
    }


# BatchSuspendUserRequestTypeDef definition

class BatchSuspendUserRequestTypeDef(TypedDict):
    AccountId: str,
    UserIdList: Sequence[str],
```

## UserErrorTypeDef

```python
# UserErrorTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UserErrorTypeDef


def get_value() -> UserErrorTypeDef:
    return {
        "UserId": ...,
    }


# UserErrorTypeDef definition

class UserErrorTypeDef(TypedDict):
    UserId: NotRequired[str],
    ErrorCode: NotRequired[ErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## BatchUnsuspendUserRequestTypeDef

```python
# BatchUnsuspendUserRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import BatchUnsuspendUserRequestTypeDef


def get_value() -> BatchUnsuspendUserRequestTypeDef:
    return {
        "AccountId": ...,
    }


# BatchUnsuspendUserRequestTypeDef definition

class BatchUnsuspendUserRequestTypeDef(TypedDict):
    AccountId: str,
    UserIdList: Sequence[str],
```

## UpdatePhoneNumberRequestItemTypeDef

```python
# UpdatePhoneNumberRequestItemTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdatePhoneNumberRequestItemTypeDef


def get_value() -> UpdatePhoneNumberRequestItemTypeDef:
    return {
        "PhoneNumberId": ...,
    }


# UpdatePhoneNumberRequestItemTypeDef definition

class UpdatePhoneNumberRequestItemTypeDef(TypedDict):
    PhoneNumberId: str,
    ProductType: NotRequired[PhoneNumberProductTypeType],  # (1)
    CallingName: NotRequired[str],
```

1. See [:material-code-brackets: PhoneNumberProductTypeType](./literals.md#phonenumberproducttypetype) 
## BotTypeDef

```python
# BotTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import BotTypeDef


def get_value() -> BotTypeDef:
    return {
        "BotId": ...,
    }


# BotTypeDef definition

class BotTypeDef(TypedDict):
    BotId: NotRequired[str],
    UserId: NotRequired[str],
    DisplayName: NotRequired[str],
    BotType: NotRequired[BotTypeType],  # (1)
    Disabled: NotRequired[bool],
    CreatedTimestamp: NotRequired[datetime],
    UpdatedTimestamp: NotRequired[datetime],
    BotEmail: NotRequired[str],
    SecurityToken: NotRequired[str],
```

1. See [:material-code-brackets: BotTypeType](./literals.md#bottypetype) 
## BusinessCallingSettingsTypeDef

```python
# BusinessCallingSettingsTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import BusinessCallingSettingsTypeDef


def get_value() -> BusinessCallingSettingsTypeDef:
    return {
        "CdrBucket": ...,
    }


# BusinessCallingSettingsTypeDef definition

class BusinessCallingSettingsTypeDef(TypedDict):
    CdrBucket: NotRequired[str],
```

## CandidateAddressTypeDef

```python
# CandidateAddressTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CandidateAddressTypeDef


def get_value() -> CandidateAddressTypeDef:
    return {
        "streetInfo": ...,
    }


# CandidateAddressTypeDef definition

class CandidateAddressTypeDef(TypedDict):
    streetInfo: NotRequired[str],
    streetNumber: NotRequired[str],
    city: NotRequired[str],
    state: NotRequired[str],
    postalCode: NotRequired[str],
    postalCodePlus4: NotRequired[str],
    country: NotRequired[str],
```

## ChannelSummaryTypeDef

```python
# ChannelSummaryTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ChannelSummaryTypeDef


def get_value() -> ChannelSummaryTypeDef:
    return {
        "Name": ...,
    }


# ChannelSummaryTypeDef definition

class ChannelSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    ChannelArn: NotRequired[str],
    Mode: NotRequired[ChannelModeType],  # (1)
    Privacy: NotRequired[ChannelPrivacyType],  # (2)
    Metadata: NotRequired[str],
    LastMessageTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: ChannelModeType](./literals.md#channelmodetype) 
2. See [:material-code-brackets: ChannelPrivacyType](./literals.md#channelprivacytype) 
## ConversationRetentionSettingsTypeDef

```python
# ConversationRetentionSettingsTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ConversationRetentionSettingsTypeDef


def get_value() -> ConversationRetentionSettingsTypeDef:
    return {
        "RetentionDays": ...,
    }


# ConversationRetentionSettingsTypeDef definition

class ConversationRetentionSettingsTypeDef(TypedDict):
    RetentionDays: NotRequired[int],
```

## CreateAccountRequestTypeDef

```python
# CreateAccountRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateAccountRequestTypeDef


def get_value() -> CreateAccountRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateAccountRequestTypeDef definition

class CreateAccountRequestTypeDef(TypedDict):
    Name: str,
```

## CreateAppInstanceAdminRequestTypeDef

```python
# CreateAppInstanceAdminRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateAppInstanceAdminRequestTypeDef


def get_value() -> CreateAppInstanceAdminRequestTypeDef:
    return {
        "AppInstanceAdminArn": ...,
    }


# CreateAppInstanceAdminRequestTypeDef definition

class CreateAppInstanceAdminRequestTypeDef(TypedDict):
    AppInstanceAdminArn: str,
    AppInstanceArn: str,
```

## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "Key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## CreateBotRequestTypeDef

```python
# CreateBotRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateBotRequestTypeDef


def get_value() -> CreateBotRequestTypeDef:
    return {
        "AccountId": ...,
    }


# CreateBotRequestTypeDef definition

class CreateBotRequestTypeDef(TypedDict):
    AccountId: str,
    DisplayName: str,
    Domain: NotRequired[str],
```

## CreateChannelBanRequestTypeDef

```python
# CreateChannelBanRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateChannelBanRequestTypeDef


def get_value() -> CreateChannelBanRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# CreateChannelBanRequestTypeDef definition

class CreateChannelBanRequestTypeDef(TypedDict):
    ChannelArn: str,
    MemberArn: str,
    ChimeBearer: NotRequired[str],
```

## CreateChannelMembershipRequestTypeDef

```python
# CreateChannelMembershipRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateChannelMembershipRequestTypeDef


def get_value() -> CreateChannelMembershipRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# CreateChannelMembershipRequestTypeDef definition

class CreateChannelMembershipRequestTypeDef(TypedDict):
    ChannelArn: str,
    MemberArn: str,
    Type: ChannelMembershipTypeType,  # (1)
    ChimeBearer: NotRequired[str],
```

1. See [:material-code-brackets: ChannelMembershipTypeType](./literals.md#channelmembershiptypetype) 
## CreateChannelModeratorRequestTypeDef

```python
# CreateChannelModeratorRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateChannelModeratorRequestTypeDef


def get_value() -> CreateChannelModeratorRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# CreateChannelModeratorRequestTypeDef definition

class CreateChannelModeratorRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChannelModeratorArn: str,
    ChimeBearer: NotRequired[str],
```

## CreateMeetingDialOutRequestTypeDef

```python
# CreateMeetingDialOutRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateMeetingDialOutRequestTypeDef


def get_value() -> CreateMeetingDialOutRequestTypeDef:
    return {
        "MeetingId": ...,
    }


# CreateMeetingDialOutRequestTypeDef definition

class CreateMeetingDialOutRequestTypeDef(TypedDict):
    MeetingId: str,
    FromPhoneNumber: str,
    ToPhoneNumber: str,
    JoinToken: str,
```

## MeetingNotificationConfigurationTypeDef

```python
# MeetingNotificationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import MeetingNotificationConfigurationTypeDef


def get_value() -> MeetingNotificationConfigurationTypeDef:
    return {
        "SnsTopicArn": ...,
    }


# MeetingNotificationConfigurationTypeDef definition

class MeetingNotificationConfigurationTypeDef(TypedDict):
    SnsTopicArn: NotRequired[str],
    SqsQueueArn: NotRequired[str],
```

## CreatePhoneNumberOrderRequestTypeDef

```python
# CreatePhoneNumberOrderRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreatePhoneNumberOrderRequestTypeDef


def get_value() -> CreatePhoneNumberOrderRequestTypeDef:
    return {
        "ProductType": ...,
    }


# CreatePhoneNumberOrderRequestTypeDef definition

class CreatePhoneNumberOrderRequestTypeDef(TypedDict):
    ProductType: PhoneNumberProductTypeType,  # (1)
    E164PhoneNumbers: Sequence[str],
```

1. See [:material-code-brackets: PhoneNumberProductTypeType](./literals.md#phonenumberproducttypetype) 
## GeoMatchParamsTypeDef

```python
# GeoMatchParamsTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GeoMatchParamsTypeDef


def get_value() -> GeoMatchParamsTypeDef:
    return {
        "Country": ...,
    }


# GeoMatchParamsTypeDef definition

class GeoMatchParamsTypeDef(TypedDict):
    Country: str,
    AreaCode: str,
```

## CreateRoomMembershipRequestTypeDef

```python
# CreateRoomMembershipRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateRoomMembershipRequestTypeDef


def get_value() -> CreateRoomMembershipRequestTypeDef:
    return {
        "AccountId": ...,
    }


# CreateRoomMembershipRequestTypeDef definition

class CreateRoomMembershipRequestTypeDef(TypedDict):
    AccountId: str,
    RoomId: str,
    MemberId: str,
    Role: NotRequired[RoomMembershipRoleType],  # (1)
```

1. See [:material-code-brackets: RoomMembershipRoleType](./literals.md#roommembershiproletype) 
## CreateRoomRequestTypeDef

```python
# CreateRoomRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateRoomRequestTypeDef


def get_value() -> CreateRoomRequestTypeDef:
    return {
        "AccountId": ...,
    }


# CreateRoomRequestTypeDef definition

class CreateRoomRequestTypeDef(TypedDict):
    AccountId: str,
    Name: str,
    ClientRequestToken: NotRequired[str],
```

## RoomTypeDef

```python
# RoomTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import RoomTypeDef


def get_value() -> RoomTypeDef:
    return {
        "RoomId": ...,
    }


# RoomTypeDef definition

class RoomTypeDef(TypedDict):
    RoomId: NotRequired[str],
    Name: NotRequired[str],
    AccountId: NotRequired[str],
    CreatedBy: NotRequired[str],
    CreatedTimestamp: NotRequired[datetime],
    UpdatedTimestamp: NotRequired[datetime],
```

## CreateSipMediaApplicationCallRequestTypeDef

```python
# CreateSipMediaApplicationCallRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateSipMediaApplicationCallRequestTypeDef


def get_value() -> CreateSipMediaApplicationCallRequestTypeDef:
    return {
        "FromPhoneNumber": ...,
    }


# CreateSipMediaApplicationCallRequestTypeDef definition

class CreateSipMediaApplicationCallRequestTypeDef(TypedDict):
    FromPhoneNumber: str,
    ToPhoneNumber: str,
    SipMediaApplicationId: str,
    SipHeaders: NotRequired[Mapping[str, str]],
```

## SipMediaApplicationCallTypeDef

```python
# SipMediaApplicationCallTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import SipMediaApplicationCallTypeDef


def get_value() -> SipMediaApplicationCallTypeDef:
    return {
        "TransactionId": ...,
    }


# SipMediaApplicationCallTypeDef definition

class SipMediaApplicationCallTypeDef(TypedDict):
    TransactionId: NotRequired[str],
```

## SipMediaApplicationEndpointTypeDef

```python
# SipMediaApplicationEndpointTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import SipMediaApplicationEndpointTypeDef


def get_value() -> SipMediaApplicationEndpointTypeDef:
    return {
        "LambdaArn": ...,
    }


# SipMediaApplicationEndpointTypeDef definition

class SipMediaApplicationEndpointTypeDef(TypedDict):
    LambdaArn: NotRequired[str],
```

## SipRuleTargetApplicationTypeDef

```python
# SipRuleTargetApplicationTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import SipRuleTargetApplicationTypeDef


def get_value() -> SipRuleTargetApplicationTypeDef:
    return {
        "SipMediaApplicationId": ...,
    }


# SipRuleTargetApplicationTypeDef definition

class SipRuleTargetApplicationTypeDef(TypedDict):
    SipMediaApplicationId: NotRequired[str],
    Priority: NotRequired[int],
    AwsRegion: NotRequired[str],
```

## CreateUserRequestTypeDef

```python
# CreateUserRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateUserRequestTypeDef


def get_value() -> CreateUserRequestTypeDef:
    return {
        "AccountId": ...,
    }


# CreateUserRequestTypeDef definition

class CreateUserRequestTypeDef(TypedDict):
    AccountId: str,
    Username: NotRequired[str],
    Email: NotRequired[str],
    UserType: NotRequired[UserTypeType],  # (1)
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
## VoiceConnectorItemTypeDef

```python
# VoiceConnectorItemTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import VoiceConnectorItemTypeDef


def get_value() -> VoiceConnectorItemTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# VoiceConnectorItemTypeDef definition

class VoiceConnectorItemTypeDef(TypedDict):
    VoiceConnectorId: str,
    Priority: int,
```

## CreateVoiceConnectorRequestTypeDef

```python
# CreateVoiceConnectorRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateVoiceConnectorRequestTypeDef


def get_value() -> CreateVoiceConnectorRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateVoiceConnectorRequestTypeDef definition

class CreateVoiceConnectorRequestTypeDef(TypedDict):
    Name: str,
    RequireEncryption: bool,
    AwsRegion: NotRequired[VoiceConnectorAwsRegionType],  # (1)
```

1. See [:material-code-brackets: VoiceConnectorAwsRegionType](./literals.md#voiceconnectorawsregiontype) 
## VoiceConnectorTypeDef

```python
# VoiceConnectorTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import VoiceConnectorTypeDef


def get_value() -> VoiceConnectorTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# VoiceConnectorTypeDef definition

class VoiceConnectorTypeDef(TypedDict):
    VoiceConnectorId: NotRequired[str],
    AwsRegion: NotRequired[VoiceConnectorAwsRegionType],  # (1)
    Name: NotRequired[str],
    OutboundHostName: NotRequired[str],
    RequireEncryption: NotRequired[bool],
    CreatedTimestamp: NotRequired[datetime],
    UpdatedTimestamp: NotRequired[datetime],
    VoiceConnectorArn: NotRequired[str],
```

1. See [:material-code-brackets: VoiceConnectorAwsRegionType](./literals.md#voiceconnectorawsregiontype) 
## CredentialTypeDef

```python
# CredentialTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CredentialTypeDef


def get_value() -> CredentialTypeDef:
    return {
        "Username": ...,
    }


# CredentialTypeDef definition

class CredentialTypeDef(TypedDict):
    Username: NotRequired[str],
    Password: NotRequired[str],
```

## DNISEmergencyCallingConfigurationTypeDef

```python
# DNISEmergencyCallingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DNISEmergencyCallingConfigurationTypeDef


def get_value() -> DNISEmergencyCallingConfigurationTypeDef:
    return {
        "EmergencyPhoneNumber": ...,
    }


# DNISEmergencyCallingConfigurationTypeDef definition

class DNISEmergencyCallingConfigurationTypeDef(TypedDict):
    EmergencyPhoneNumber: str,
    CallingCountry: str,
    TestPhoneNumber: NotRequired[str],
```

## DeleteAccountRequestTypeDef

```python
# DeleteAccountRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteAccountRequestTypeDef


def get_value() -> DeleteAccountRequestTypeDef:
    return {
        "AccountId": ...,
    }


# DeleteAccountRequestTypeDef definition

class DeleteAccountRequestTypeDef(TypedDict):
    AccountId: str,
```

## DeleteAppInstanceAdminRequestTypeDef

```python
# DeleteAppInstanceAdminRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteAppInstanceAdminRequestTypeDef


def get_value() -> DeleteAppInstanceAdminRequestTypeDef:
    return {
        "AppInstanceAdminArn": ...,
    }


# DeleteAppInstanceAdminRequestTypeDef definition

class DeleteAppInstanceAdminRequestTypeDef(TypedDict):
    AppInstanceAdminArn: str,
    AppInstanceArn: str,
```

## DeleteAppInstanceRequestTypeDef

```python
# DeleteAppInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteAppInstanceRequestTypeDef


def get_value() -> DeleteAppInstanceRequestTypeDef:
    return {
        "AppInstanceArn": ...,
    }


# DeleteAppInstanceRequestTypeDef definition

class DeleteAppInstanceRequestTypeDef(TypedDict):
    AppInstanceArn: str,
```

## DeleteAppInstanceStreamingConfigurationsRequestTypeDef

```python
# DeleteAppInstanceStreamingConfigurationsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteAppInstanceStreamingConfigurationsRequestTypeDef


def get_value() -> DeleteAppInstanceStreamingConfigurationsRequestTypeDef:
    return {
        "AppInstanceArn": ...,
    }


# DeleteAppInstanceStreamingConfigurationsRequestTypeDef definition

class DeleteAppInstanceStreamingConfigurationsRequestTypeDef(TypedDict):
    AppInstanceArn: str,
```

## DeleteAppInstanceUserRequestTypeDef

```python
# DeleteAppInstanceUserRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteAppInstanceUserRequestTypeDef


def get_value() -> DeleteAppInstanceUserRequestTypeDef:
    return {
        "AppInstanceUserArn": ...,
    }


# DeleteAppInstanceUserRequestTypeDef definition

class DeleteAppInstanceUserRequestTypeDef(TypedDict):
    AppInstanceUserArn: str,
```

## DeleteAttendeeRequestTypeDef

```python
# DeleteAttendeeRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteAttendeeRequestTypeDef


def get_value() -> DeleteAttendeeRequestTypeDef:
    return {
        "MeetingId": ...,
    }


# DeleteAttendeeRequestTypeDef definition

class DeleteAttendeeRequestTypeDef(TypedDict):
    MeetingId: str,
    AttendeeId: str,
```

## DeleteChannelBanRequestTypeDef

```python
# DeleteChannelBanRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteChannelBanRequestTypeDef


def get_value() -> DeleteChannelBanRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# DeleteChannelBanRequestTypeDef definition

class DeleteChannelBanRequestTypeDef(TypedDict):
    ChannelArn: str,
    MemberArn: str,
    ChimeBearer: NotRequired[str],
```

## DeleteChannelMembershipRequestTypeDef

```python
# DeleteChannelMembershipRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteChannelMembershipRequestTypeDef


def get_value() -> DeleteChannelMembershipRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# DeleteChannelMembershipRequestTypeDef definition

class DeleteChannelMembershipRequestTypeDef(TypedDict):
    ChannelArn: str,
    MemberArn: str,
    ChimeBearer: NotRequired[str],
```

## DeleteChannelMessageRequestTypeDef

```python
# DeleteChannelMessageRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteChannelMessageRequestTypeDef


def get_value() -> DeleteChannelMessageRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# DeleteChannelMessageRequestTypeDef definition

class DeleteChannelMessageRequestTypeDef(TypedDict):
    ChannelArn: str,
    MessageId: str,
    ChimeBearer: NotRequired[str],
```

## DeleteChannelModeratorRequestTypeDef

```python
# DeleteChannelModeratorRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteChannelModeratorRequestTypeDef


def get_value() -> DeleteChannelModeratorRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# DeleteChannelModeratorRequestTypeDef definition

class DeleteChannelModeratorRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChannelModeratorArn: str,
    ChimeBearer: NotRequired[str],
```

## DeleteChannelRequestTypeDef

```python
# DeleteChannelRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteChannelRequestTypeDef


def get_value() -> DeleteChannelRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# DeleteChannelRequestTypeDef definition

class DeleteChannelRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChimeBearer: NotRequired[str],
```

## DeleteEventsConfigurationRequestTypeDef

```python
# DeleteEventsConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteEventsConfigurationRequestTypeDef


def get_value() -> DeleteEventsConfigurationRequestTypeDef:
    return {
        "AccountId": ...,
    }


# DeleteEventsConfigurationRequestTypeDef definition

class DeleteEventsConfigurationRequestTypeDef(TypedDict):
    AccountId: str,
    BotId: str,
```

## DeleteMediaCapturePipelineRequestTypeDef

```python
# DeleteMediaCapturePipelineRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteMediaCapturePipelineRequestTypeDef


def get_value() -> DeleteMediaCapturePipelineRequestTypeDef:
    return {
        "MediaPipelineId": ...,
    }


# DeleteMediaCapturePipelineRequestTypeDef definition

class DeleteMediaCapturePipelineRequestTypeDef(TypedDict):
    MediaPipelineId: str,
```

## DeleteMeetingRequestTypeDef

```python
# DeleteMeetingRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteMeetingRequestTypeDef


def get_value() -> DeleteMeetingRequestTypeDef:
    return {
        "MeetingId": ...,
    }


# DeleteMeetingRequestTypeDef definition

class DeleteMeetingRequestTypeDef(TypedDict):
    MeetingId: str,
```

## DeletePhoneNumberRequestTypeDef

```python
# DeletePhoneNumberRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeletePhoneNumberRequestTypeDef


def get_value() -> DeletePhoneNumberRequestTypeDef:
    return {
        "PhoneNumberId": ...,
    }


# DeletePhoneNumberRequestTypeDef definition

class DeletePhoneNumberRequestTypeDef(TypedDict):
    PhoneNumberId: str,
```

## DeleteProxySessionRequestTypeDef

```python
# DeleteProxySessionRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteProxySessionRequestTypeDef


def get_value() -> DeleteProxySessionRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# DeleteProxySessionRequestTypeDef definition

class DeleteProxySessionRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    ProxySessionId: str,
```

## DeleteRoomMembershipRequestTypeDef

```python
# DeleteRoomMembershipRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteRoomMembershipRequestTypeDef


def get_value() -> DeleteRoomMembershipRequestTypeDef:
    return {
        "AccountId": ...,
    }


# DeleteRoomMembershipRequestTypeDef definition

class DeleteRoomMembershipRequestTypeDef(TypedDict):
    AccountId: str,
    RoomId: str,
    MemberId: str,
```

## DeleteRoomRequestTypeDef

```python
# DeleteRoomRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteRoomRequestTypeDef


def get_value() -> DeleteRoomRequestTypeDef:
    return {
        "AccountId": ...,
    }


# DeleteRoomRequestTypeDef definition

class DeleteRoomRequestTypeDef(TypedDict):
    AccountId: str,
    RoomId: str,
```

## DeleteSipMediaApplicationRequestTypeDef

```python
# DeleteSipMediaApplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteSipMediaApplicationRequestTypeDef


def get_value() -> DeleteSipMediaApplicationRequestTypeDef:
    return {
        "SipMediaApplicationId": ...,
    }


# DeleteSipMediaApplicationRequestTypeDef definition

class DeleteSipMediaApplicationRequestTypeDef(TypedDict):
    SipMediaApplicationId: str,
```

## DeleteSipRuleRequestTypeDef

```python
# DeleteSipRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteSipRuleRequestTypeDef


def get_value() -> DeleteSipRuleRequestTypeDef:
    return {
        "SipRuleId": ...,
    }


# DeleteSipRuleRequestTypeDef definition

class DeleteSipRuleRequestTypeDef(TypedDict):
    SipRuleId: str,
```

## DeleteVoiceConnectorEmergencyCallingConfigurationRequestTypeDef

```python
# DeleteVoiceConnectorEmergencyCallingConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteVoiceConnectorEmergencyCallingConfigurationRequestTypeDef


def get_value() -> DeleteVoiceConnectorEmergencyCallingConfigurationRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# DeleteVoiceConnectorEmergencyCallingConfigurationRequestTypeDef definition

class DeleteVoiceConnectorEmergencyCallingConfigurationRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## DeleteVoiceConnectorGroupRequestTypeDef

```python
# DeleteVoiceConnectorGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteVoiceConnectorGroupRequestTypeDef


def get_value() -> DeleteVoiceConnectorGroupRequestTypeDef:
    return {
        "VoiceConnectorGroupId": ...,
    }


# DeleteVoiceConnectorGroupRequestTypeDef definition

class DeleteVoiceConnectorGroupRequestTypeDef(TypedDict):
    VoiceConnectorGroupId: str,
```

## DeleteVoiceConnectorOriginationRequestTypeDef

```python
# DeleteVoiceConnectorOriginationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteVoiceConnectorOriginationRequestTypeDef


def get_value() -> DeleteVoiceConnectorOriginationRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# DeleteVoiceConnectorOriginationRequestTypeDef definition

class DeleteVoiceConnectorOriginationRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## DeleteVoiceConnectorProxyRequestTypeDef

```python
# DeleteVoiceConnectorProxyRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteVoiceConnectorProxyRequestTypeDef


def get_value() -> DeleteVoiceConnectorProxyRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# DeleteVoiceConnectorProxyRequestTypeDef definition

class DeleteVoiceConnectorProxyRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## DeleteVoiceConnectorRequestTypeDef

```python
# DeleteVoiceConnectorRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteVoiceConnectorRequestTypeDef


def get_value() -> DeleteVoiceConnectorRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# DeleteVoiceConnectorRequestTypeDef definition

class DeleteVoiceConnectorRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## DeleteVoiceConnectorStreamingConfigurationRequestTypeDef

```python
# DeleteVoiceConnectorStreamingConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteVoiceConnectorStreamingConfigurationRequestTypeDef


def get_value() -> DeleteVoiceConnectorStreamingConfigurationRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# DeleteVoiceConnectorStreamingConfigurationRequestTypeDef definition

class DeleteVoiceConnectorStreamingConfigurationRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## DeleteVoiceConnectorTerminationCredentialsRequestTypeDef

```python
# DeleteVoiceConnectorTerminationCredentialsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteVoiceConnectorTerminationCredentialsRequestTypeDef


def get_value() -> DeleteVoiceConnectorTerminationCredentialsRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# DeleteVoiceConnectorTerminationCredentialsRequestTypeDef definition

class DeleteVoiceConnectorTerminationCredentialsRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    Usernames: Sequence[str],
```

## DeleteVoiceConnectorTerminationRequestTypeDef

```python
# DeleteVoiceConnectorTerminationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DeleteVoiceConnectorTerminationRequestTypeDef


def get_value() -> DeleteVoiceConnectorTerminationRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# DeleteVoiceConnectorTerminationRequestTypeDef definition

class DeleteVoiceConnectorTerminationRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## DescribeAppInstanceAdminRequestTypeDef

```python
# DescribeAppInstanceAdminRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DescribeAppInstanceAdminRequestTypeDef


def get_value() -> DescribeAppInstanceAdminRequestTypeDef:
    return {
        "AppInstanceAdminArn": ...,
    }


# DescribeAppInstanceAdminRequestTypeDef definition

class DescribeAppInstanceAdminRequestTypeDef(TypedDict):
    AppInstanceAdminArn: str,
    AppInstanceArn: str,
```

## DescribeAppInstanceRequestTypeDef

```python
# DescribeAppInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DescribeAppInstanceRequestTypeDef


def get_value() -> DescribeAppInstanceRequestTypeDef:
    return {
        "AppInstanceArn": ...,
    }


# DescribeAppInstanceRequestTypeDef definition

class DescribeAppInstanceRequestTypeDef(TypedDict):
    AppInstanceArn: str,
```

## DescribeAppInstanceUserRequestTypeDef

```python
# DescribeAppInstanceUserRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DescribeAppInstanceUserRequestTypeDef


def get_value() -> DescribeAppInstanceUserRequestTypeDef:
    return {
        "AppInstanceUserArn": ...,
    }


# DescribeAppInstanceUserRequestTypeDef definition

class DescribeAppInstanceUserRequestTypeDef(TypedDict):
    AppInstanceUserArn: str,
```

## DescribeChannelBanRequestTypeDef

```python
# DescribeChannelBanRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DescribeChannelBanRequestTypeDef


def get_value() -> DescribeChannelBanRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# DescribeChannelBanRequestTypeDef definition

class DescribeChannelBanRequestTypeDef(TypedDict):
    ChannelArn: str,
    MemberArn: str,
    ChimeBearer: NotRequired[str],
```

## DescribeChannelMembershipForAppInstanceUserRequestTypeDef

```python
# DescribeChannelMembershipForAppInstanceUserRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DescribeChannelMembershipForAppInstanceUserRequestTypeDef


def get_value() -> DescribeChannelMembershipForAppInstanceUserRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# DescribeChannelMembershipForAppInstanceUserRequestTypeDef definition

class DescribeChannelMembershipForAppInstanceUserRequestTypeDef(TypedDict):
    ChannelArn: str,
    AppInstanceUserArn: str,
    ChimeBearer: NotRequired[str],
```

## DescribeChannelMembershipRequestTypeDef

```python
# DescribeChannelMembershipRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DescribeChannelMembershipRequestTypeDef


def get_value() -> DescribeChannelMembershipRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# DescribeChannelMembershipRequestTypeDef definition

class DescribeChannelMembershipRequestTypeDef(TypedDict):
    ChannelArn: str,
    MemberArn: str,
    ChimeBearer: NotRequired[str],
```

## DescribeChannelModeratedByAppInstanceUserRequestTypeDef

```python
# DescribeChannelModeratedByAppInstanceUserRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DescribeChannelModeratedByAppInstanceUserRequestTypeDef


def get_value() -> DescribeChannelModeratedByAppInstanceUserRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# DescribeChannelModeratedByAppInstanceUserRequestTypeDef definition

class DescribeChannelModeratedByAppInstanceUserRequestTypeDef(TypedDict):
    ChannelArn: str,
    AppInstanceUserArn: str,
    ChimeBearer: NotRequired[str],
```

## DescribeChannelModeratorRequestTypeDef

```python
# DescribeChannelModeratorRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DescribeChannelModeratorRequestTypeDef


def get_value() -> DescribeChannelModeratorRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# DescribeChannelModeratorRequestTypeDef definition

class DescribeChannelModeratorRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChannelModeratorArn: str,
    ChimeBearer: NotRequired[str],
```

## DescribeChannelRequestTypeDef

```python
# DescribeChannelRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DescribeChannelRequestTypeDef


def get_value() -> DescribeChannelRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# DescribeChannelRequestTypeDef definition

class DescribeChannelRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChimeBearer: NotRequired[str],
```

## DisassociatePhoneNumberFromUserRequestTypeDef

```python
# DisassociatePhoneNumberFromUserRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DisassociatePhoneNumberFromUserRequestTypeDef


def get_value() -> DisassociatePhoneNumberFromUserRequestTypeDef:
    return {
        "AccountId": ...,
    }


# DisassociatePhoneNumberFromUserRequestTypeDef definition

class DisassociatePhoneNumberFromUserRequestTypeDef(TypedDict):
    AccountId: str,
    UserId: str,
```

## DisassociatePhoneNumbersFromVoiceConnectorGroupRequestTypeDef

```python
# DisassociatePhoneNumbersFromVoiceConnectorGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DisassociatePhoneNumbersFromVoiceConnectorGroupRequestTypeDef


def get_value() -> DisassociatePhoneNumbersFromVoiceConnectorGroupRequestTypeDef:
    return {
        "VoiceConnectorGroupId": ...,
    }


# DisassociatePhoneNumbersFromVoiceConnectorGroupRequestTypeDef definition

class DisassociatePhoneNumbersFromVoiceConnectorGroupRequestTypeDef(TypedDict):
    VoiceConnectorGroupId: str,
    E164PhoneNumbers: Sequence[str],
```

## DisassociatePhoneNumbersFromVoiceConnectorRequestTypeDef

```python
# DisassociatePhoneNumbersFromVoiceConnectorRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DisassociatePhoneNumbersFromVoiceConnectorRequestTypeDef


def get_value() -> DisassociatePhoneNumbersFromVoiceConnectorRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# DisassociatePhoneNumbersFromVoiceConnectorRequestTypeDef definition

class DisassociatePhoneNumbersFromVoiceConnectorRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    E164PhoneNumbers: Sequence[str],
```

## DisassociateSigninDelegateGroupsFromAccountRequestTypeDef

```python
# DisassociateSigninDelegateGroupsFromAccountRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DisassociateSigninDelegateGroupsFromAccountRequestTypeDef


def get_value() -> DisassociateSigninDelegateGroupsFromAccountRequestTypeDef:
    return {
        "AccountId": ...,
    }


# DisassociateSigninDelegateGroupsFromAccountRequestTypeDef definition

class DisassociateSigninDelegateGroupsFromAccountRequestTypeDef(TypedDict):
    AccountId: str,
    GroupNames: Sequence[str],
```

## EngineTranscribeMedicalSettingsTypeDef

```python
# EngineTranscribeMedicalSettingsTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import EngineTranscribeMedicalSettingsTypeDef


def get_value() -> EngineTranscribeMedicalSettingsTypeDef:
    return {
        "LanguageCode": ...,
    }


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
# EngineTranscribeSettingsTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import EngineTranscribeSettingsTypeDef


def get_value() -> EngineTranscribeSettingsTypeDef:
    return {
        "LanguageCode": ...,
    }


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
## EventsConfigurationTypeDef

```python
# EventsConfigurationTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import EventsConfigurationTypeDef


def get_value() -> EventsConfigurationTypeDef:
    return {
        "BotId": ...,
    }


# EventsConfigurationTypeDef definition

class EventsConfigurationTypeDef(TypedDict):
    BotId: NotRequired[str],
    OutboundEventsHTTPSEndpoint: NotRequired[str],
    LambdaFunctionArn: NotRequired[str],
```

## GetAccountRequestTypeDef

```python
# GetAccountRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetAccountRequestTypeDef


def get_value() -> GetAccountRequestTypeDef:
    return {
        "AccountId": ...,
    }


# GetAccountRequestTypeDef definition

class GetAccountRequestTypeDef(TypedDict):
    AccountId: str,
```

## GetAccountSettingsRequestTypeDef

```python
# GetAccountSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetAccountSettingsRequestTypeDef


def get_value() -> GetAccountSettingsRequestTypeDef:
    return {
        "AccountId": ...,
    }


# GetAccountSettingsRequestTypeDef definition

class GetAccountSettingsRequestTypeDef(TypedDict):
    AccountId: str,
```

## GetAppInstanceRetentionSettingsRequestTypeDef

```python
# GetAppInstanceRetentionSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetAppInstanceRetentionSettingsRequestTypeDef


def get_value() -> GetAppInstanceRetentionSettingsRequestTypeDef:
    return {
        "AppInstanceArn": ...,
    }


# GetAppInstanceRetentionSettingsRequestTypeDef definition

class GetAppInstanceRetentionSettingsRequestTypeDef(TypedDict):
    AppInstanceArn: str,
```

## GetAppInstanceStreamingConfigurationsRequestTypeDef

```python
# GetAppInstanceStreamingConfigurationsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetAppInstanceStreamingConfigurationsRequestTypeDef


def get_value() -> GetAppInstanceStreamingConfigurationsRequestTypeDef:
    return {
        "AppInstanceArn": ...,
    }


# GetAppInstanceStreamingConfigurationsRequestTypeDef definition

class GetAppInstanceStreamingConfigurationsRequestTypeDef(TypedDict):
    AppInstanceArn: str,
```

## GetAttendeeRequestTypeDef

```python
# GetAttendeeRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetAttendeeRequestTypeDef


def get_value() -> GetAttendeeRequestTypeDef:
    return {
        "MeetingId": ...,
    }


# GetAttendeeRequestTypeDef definition

class GetAttendeeRequestTypeDef(TypedDict):
    MeetingId: str,
    AttendeeId: str,
```

## GetBotRequestTypeDef

```python
# GetBotRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetBotRequestTypeDef


def get_value() -> GetBotRequestTypeDef:
    return {
        "AccountId": ...,
    }


# GetBotRequestTypeDef definition

class GetBotRequestTypeDef(TypedDict):
    AccountId: str,
    BotId: str,
```

## GetChannelMessageRequestTypeDef

```python
# GetChannelMessageRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetChannelMessageRequestTypeDef


def get_value() -> GetChannelMessageRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# GetChannelMessageRequestTypeDef definition

class GetChannelMessageRequestTypeDef(TypedDict):
    ChannelArn: str,
    MessageId: str,
    ChimeBearer: NotRequired[str],
```

## GetEventsConfigurationRequestTypeDef

```python
# GetEventsConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetEventsConfigurationRequestTypeDef


def get_value() -> GetEventsConfigurationRequestTypeDef:
    return {
        "AccountId": ...,
    }


# GetEventsConfigurationRequestTypeDef definition

class GetEventsConfigurationRequestTypeDef(TypedDict):
    AccountId: str,
    BotId: str,
```

## VoiceConnectorSettingsTypeDef

```python
# VoiceConnectorSettingsTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import VoiceConnectorSettingsTypeDef


def get_value() -> VoiceConnectorSettingsTypeDef:
    return {
        "CdrBucket": ...,
    }


# VoiceConnectorSettingsTypeDef definition

class VoiceConnectorSettingsTypeDef(TypedDict):
    CdrBucket: NotRequired[str],
```

## GetMediaCapturePipelineRequestTypeDef

```python
# GetMediaCapturePipelineRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetMediaCapturePipelineRequestTypeDef


def get_value() -> GetMediaCapturePipelineRequestTypeDef:
    return {
        "MediaPipelineId": ...,
    }


# GetMediaCapturePipelineRequestTypeDef definition

class GetMediaCapturePipelineRequestTypeDef(TypedDict):
    MediaPipelineId: str,
```

## GetMeetingRequestTypeDef

```python
# GetMeetingRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetMeetingRequestTypeDef


def get_value() -> GetMeetingRequestTypeDef:
    return {
        "MeetingId": ...,
    }


# GetMeetingRequestTypeDef definition

class GetMeetingRequestTypeDef(TypedDict):
    MeetingId: str,
```

## MessagingSessionEndpointTypeDef

```python
# MessagingSessionEndpointTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import MessagingSessionEndpointTypeDef


def get_value() -> MessagingSessionEndpointTypeDef:
    return {
        "Url": ...,
    }


# MessagingSessionEndpointTypeDef definition

class MessagingSessionEndpointTypeDef(TypedDict):
    Url: NotRequired[str],
```

## GetPhoneNumberOrderRequestTypeDef

```python
# GetPhoneNumberOrderRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetPhoneNumberOrderRequestTypeDef


def get_value() -> GetPhoneNumberOrderRequestTypeDef:
    return {
        "PhoneNumberOrderId": ...,
    }


# GetPhoneNumberOrderRequestTypeDef definition

class GetPhoneNumberOrderRequestTypeDef(TypedDict):
    PhoneNumberOrderId: str,
```

## GetPhoneNumberRequestTypeDef

```python
# GetPhoneNumberRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetPhoneNumberRequestTypeDef


def get_value() -> GetPhoneNumberRequestTypeDef:
    return {
        "PhoneNumberId": ...,
    }


# GetPhoneNumberRequestTypeDef definition

class GetPhoneNumberRequestTypeDef(TypedDict):
    PhoneNumberId: str,
```

## GetProxySessionRequestTypeDef

```python
# GetProxySessionRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetProxySessionRequestTypeDef


def get_value() -> GetProxySessionRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# GetProxySessionRequestTypeDef definition

class GetProxySessionRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    ProxySessionId: str,
```

## GetRetentionSettingsRequestTypeDef

```python
# GetRetentionSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetRetentionSettingsRequestTypeDef


def get_value() -> GetRetentionSettingsRequestTypeDef:
    return {
        "AccountId": ...,
    }


# GetRetentionSettingsRequestTypeDef definition

class GetRetentionSettingsRequestTypeDef(TypedDict):
    AccountId: str,
```

## GetRoomRequestTypeDef

```python
# GetRoomRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetRoomRequestTypeDef


def get_value() -> GetRoomRequestTypeDef:
    return {
        "AccountId": ...,
    }


# GetRoomRequestTypeDef definition

class GetRoomRequestTypeDef(TypedDict):
    AccountId: str,
    RoomId: str,
```

## GetSipMediaApplicationLoggingConfigurationRequestTypeDef

```python
# GetSipMediaApplicationLoggingConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetSipMediaApplicationLoggingConfigurationRequestTypeDef


def get_value() -> GetSipMediaApplicationLoggingConfigurationRequestTypeDef:
    return {
        "SipMediaApplicationId": ...,
    }


# GetSipMediaApplicationLoggingConfigurationRequestTypeDef definition

class GetSipMediaApplicationLoggingConfigurationRequestTypeDef(TypedDict):
    SipMediaApplicationId: str,
```

## SipMediaApplicationLoggingConfigurationTypeDef

```python
# SipMediaApplicationLoggingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import SipMediaApplicationLoggingConfigurationTypeDef


def get_value() -> SipMediaApplicationLoggingConfigurationTypeDef:
    return {
        "EnableSipMediaApplicationMessageLogs": ...,
    }


# SipMediaApplicationLoggingConfigurationTypeDef definition

class SipMediaApplicationLoggingConfigurationTypeDef(TypedDict):
    EnableSipMediaApplicationMessageLogs: NotRequired[bool],
```

## GetSipMediaApplicationRequestTypeDef

```python
# GetSipMediaApplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetSipMediaApplicationRequestTypeDef


def get_value() -> GetSipMediaApplicationRequestTypeDef:
    return {
        "SipMediaApplicationId": ...,
    }


# GetSipMediaApplicationRequestTypeDef definition

class GetSipMediaApplicationRequestTypeDef(TypedDict):
    SipMediaApplicationId: str,
```

## GetSipRuleRequestTypeDef

```python
# GetSipRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetSipRuleRequestTypeDef


def get_value() -> GetSipRuleRequestTypeDef:
    return {
        "SipRuleId": ...,
    }


# GetSipRuleRequestTypeDef definition

class GetSipRuleRequestTypeDef(TypedDict):
    SipRuleId: str,
```

## GetUserRequestTypeDef

```python
# GetUserRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetUserRequestTypeDef


def get_value() -> GetUserRequestTypeDef:
    return {
        "AccountId": ...,
    }


# GetUserRequestTypeDef definition

class GetUserRequestTypeDef(TypedDict):
    AccountId: str,
    UserId: str,
```

## GetUserSettingsRequestTypeDef

```python
# GetUserSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetUserSettingsRequestTypeDef


def get_value() -> GetUserSettingsRequestTypeDef:
    return {
        "AccountId": ...,
    }


# GetUserSettingsRequestTypeDef definition

class GetUserSettingsRequestTypeDef(TypedDict):
    AccountId: str,
    UserId: str,
```

## GetVoiceConnectorEmergencyCallingConfigurationRequestTypeDef

```python
# GetVoiceConnectorEmergencyCallingConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetVoiceConnectorEmergencyCallingConfigurationRequestTypeDef


def get_value() -> GetVoiceConnectorEmergencyCallingConfigurationRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# GetVoiceConnectorEmergencyCallingConfigurationRequestTypeDef definition

class GetVoiceConnectorEmergencyCallingConfigurationRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## GetVoiceConnectorGroupRequestTypeDef

```python
# GetVoiceConnectorGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetVoiceConnectorGroupRequestTypeDef


def get_value() -> GetVoiceConnectorGroupRequestTypeDef:
    return {
        "VoiceConnectorGroupId": ...,
    }


# GetVoiceConnectorGroupRequestTypeDef definition

class GetVoiceConnectorGroupRequestTypeDef(TypedDict):
    VoiceConnectorGroupId: str,
```

## GetVoiceConnectorLoggingConfigurationRequestTypeDef

```python
# GetVoiceConnectorLoggingConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetVoiceConnectorLoggingConfigurationRequestTypeDef


def get_value() -> GetVoiceConnectorLoggingConfigurationRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# GetVoiceConnectorLoggingConfigurationRequestTypeDef definition

class GetVoiceConnectorLoggingConfigurationRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## LoggingConfigurationTypeDef

```python
# LoggingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import LoggingConfigurationTypeDef


def get_value() -> LoggingConfigurationTypeDef:
    return {
        "EnableSIPLogs": ...,
    }


# LoggingConfigurationTypeDef definition

class LoggingConfigurationTypeDef(TypedDict):
    EnableSIPLogs: NotRequired[bool],
    EnableMediaMetricLogs: NotRequired[bool],
```

## GetVoiceConnectorOriginationRequestTypeDef

```python
# GetVoiceConnectorOriginationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetVoiceConnectorOriginationRequestTypeDef


def get_value() -> GetVoiceConnectorOriginationRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# GetVoiceConnectorOriginationRequestTypeDef definition

class GetVoiceConnectorOriginationRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## GetVoiceConnectorProxyRequestTypeDef

```python
# GetVoiceConnectorProxyRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetVoiceConnectorProxyRequestTypeDef


def get_value() -> GetVoiceConnectorProxyRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# GetVoiceConnectorProxyRequestTypeDef definition

class GetVoiceConnectorProxyRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## ProxyTypeDef

```python
# ProxyTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ProxyTypeDef


def get_value() -> ProxyTypeDef:
    return {
        "DefaultSessionExpiryMinutes": ...,
    }


# ProxyTypeDef definition

class ProxyTypeDef(TypedDict):
    DefaultSessionExpiryMinutes: NotRequired[int],
    Disabled: NotRequired[bool],
    FallBackPhoneNumber: NotRequired[str],
    PhoneNumberCountries: NotRequired[List[str]],
```

## GetVoiceConnectorRequestTypeDef

```python
# GetVoiceConnectorRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetVoiceConnectorRequestTypeDef


def get_value() -> GetVoiceConnectorRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# GetVoiceConnectorRequestTypeDef definition

class GetVoiceConnectorRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## GetVoiceConnectorStreamingConfigurationRequestTypeDef

```python
# GetVoiceConnectorStreamingConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetVoiceConnectorStreamingConfigurationRequestTypeDef


def get_value() -> GetVoiceConnectorStreamingConfigurationRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# GetVoiceConnectorStreamingConfigurationRequestTypeDef definition

class GetVoiceConnectorStreamingConfigurationRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## GetVoiceConnectorTerminationHealthRequestTypeDef

```python
# GetVoiceConnectorTerminationHealthRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetVoiceConnectorTerminationHealthRequestTypeDef


def get_value() -> GetVoiceConnectorTerminationHealthRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# GetVoiceConnectorTerminationHealthRequestTypeDef definition

class GetVoiceConnectorTerminationHealthRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## TerminationHealthTypeDef

```python
# TerminationHealthTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import TerminationHealthTypeDef


def get_value() -> TerminationHealthTypeDef:
    return {
        "Timestamp": ...,
    }


# TerminationHealthTypeDef definition

class TerminationHealthTypeDef(TypedDict):
    Timestamp: NotRequired[datetime],
    Source: NotRequired[str],
```

## GetVoiceConnectorTerminationRequestTypeDef

```python
# GetVoiceConnectorTerminationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetVoiceConnectorTerminationRequestTypeDef


def get_value() -> GetVoiceConnectorTerminationRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# GetVoiceConnectorTerminationRequestTypeDef definition

class GetVoiceConnectorTerminationRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## TerminationOutputTypeDef

```python
# TerminationOutputTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import TerminationOutputTypeDef


def get_value() -> TerminationOutputTypeDef:
    return {
        "CpsLimit": ...,
    }


# TerminationOutputTypeDef definition

class TerminationOutputTypeDef(TypedDict):
    CpsLimit: NotRequired[int],
    DefaultPhoneNumber: NotRequired[str],
    CallingRegions: NotRequired[List[str]],
    CidrAllowedList: NotRequired[List[str]],
    Disabled: NotRequired[bool],
```

## InviteTypeDef

```python
# InviteTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import InviteTypeDef


def get_value() -> InviteTypeDef:
    return {
        "InviteId": ...,
    }


# InviteTypeDef definition

class InviteTypeDef(TypedDict):
    InviteId: NotRequired[str],
    Status: NotRequired[InviteStatusType],  # (1)
    EmailAddress: NotRequired[str],
    EmailStatus: NotRequired[EmailStatusType],  # (2)
```

1. See [:material-code-brackets: InviteStatusType](./literals.md#invitestatustype) 
2. See [:material-code-brackets: EmailStatusType](./literals.md#emailstatustype) 
## InviteUsersRequestTypeDef

```python
# InviteUsersRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import InviteUsersRequestTypeDef


def get_value() -> InviteUsersRequestTypeDef:
    return {
        "AccountId": ...,
    }


# InviteUsersRequestTypeDef definition

class InviteUsersRequestTypeDef(TypedDict):
    AccountId: str,
    UserEmailList: Sequence[str],
    UserType: NotRequired[UserTypeType],  # (1)
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PaginatorConfigTypeDef


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

## ListAccountsRequestTypeDef

```python
# ListAccountsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListAccountsRequestTypeDef


def get_value() -> ListAccountsRequestTypeDef:
    return {
        "Name": ...,
    }


# ListAccountsRequestTypeDef definition

class ListAccountsRequestTypeDef(TypedDict):
    Name: NotRequired[str],
    UserEmail: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListAppInstanceAdminsRequestTypeDef

```python
# ListAppInstanceAdminsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListAppInstanceAdminsRequestTypeDef


def get_value() -> ListAppInstanceAdminsRequestTypeDef:
    return {
        "AppInstanceArn": ...,
    }


# ListAppInstanceAdminsRequestTypeDef definition

class ListAppInstanceAdminsRequestTypeDef(TypedDict):
    AppInstanceArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListAppInstanceUsersRequestTypeDef

```python
# ListAppInstanceUsersRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListAppInstanceUsersRequestTypeDef


def get_value() -> ListAppInstanceUsersRequestTypeDef:
    return {
        "AppInstanceArn": ...,
    }


# ListAppInstanceUsersRequestTypeDef definition

class ListAppInstanceUsersRequestTypeDef(TypedDict):
    AppInstanceArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListAppInstancesRequestTypeDef

```python
# ListAppInstancesRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListAppInstancesRequestTypeDef


def get_value() -> ListAppInstancesRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListAppInstancesRequestTypeDef definition

class ListAppInstancesRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListAttendeeTagsRequestTypeDef

```python
# ListAttendeeTagsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListAttendeeTagsRequestTypeDef


def get_value() -> ListAttendeeTagsRequestTypeDef:
    return {
        "MeetingId": ...,
    }


# ListAttendeeTagsRequestTypeDef definition

class ListAttendeeTagsRequestTypeDef(TypedDict):
    MeetingId: str,
    AttendeeId: str,
```

## ListAttendeesRequestTypeDef

```python
# ListAttendeesRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListAttendeesRequestTypeDef


def get_value() -> ListAttendeesRequestTypeDef:
    return {
        "MeetingId": ...,
    }


# ListAttendeesRequestTypeDef definition

class ListAttendeesRequestTypeDef(TypedDict):
    MeetingId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListBotsRequestTypeDef

```python
# ListBotsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListBotsRequestTypeDef


def get_value() -> ListBotsRequestTypeDef:
    return {
        "AccountId": ...,
    }


# ListBotsRequestTypeDef definition

class ListBotsRequestTypeDef(TypedDict):
    AccountId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListChannelBansRequestTypeDef

```python
# ListChannelBansRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListChannelBansRequestTypeDef


def get_value() -> ListChannelBansRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# ListChannelBansRequestTypeDef definition

class ListChannelBansRequestTypeDef(TypedDict):
    ChannelArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ChimeBearer: NotRequired[str],
```

## ListChannelMembershipsForAppInstanceUserRequestTypeDef

```python
# ListChannelMembershipsForAppInstanceUserRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListChannelMembershipsForAppInstanceUserRequestTypeDef


def get_value() -> ListChannelMembershipsForAppInstanceUserRequestTypeDef:
    return {
        "AppInstanceUserArn": ...,
    }


# ListChannelMembershipsForAppInstanceUserRequestTypeDef definition

class ListChannelMembershipsForAppInstanceUserRequestTypeDef(TypedDict):
    AppInstanceUserArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ChimeBearer: NotRequired[str],
```

## ListChannelMembershipsRequestTypeDef

```python
# ListChannelMembershipsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListChannelMembershipsRequestTypeDef


def get_value() -> ListChannelMembershipsRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# ListChannelMembershipsRequestTypeDef definition

class ListChannelMembershipsRequestTypeDef(TypedDict):
    ChannelArn: str,
    Type: NotRequired[ChannelMembershipTypeType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ChimeBearer: NotRequired[str],
```

1. See [:material-code-brackets: ChannelMembershipTypeType](./literals.md#channelmembershiptypetype) 
## ListChannelModeratorsRequestTypeDef

```python
# ListChannelModeratorsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListChannelModeratorsRequestTypeDef


def get_value() -> ListChannelModeratorsRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# ListChannelModeratorsRequestTypeDef definition

class ListChannelModeratorsRequestTypeDef(TypedDict):
    ChannelArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ChimeBearer: NotRequired[str],
```

## ListChannelsModeratedByAppInstanceUserRequestTypeDef

```python
# ListChannelsModeratedByAppInstanceUserRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListChannelsModeratedByAppInstanceUserRequestTypeDef


def get_value() -> ListChannelsModeratedByAppInstanceUserRequestTypeDef:
    return {
        "AppInstanceUserArn": ...,
    }


# ListChannelsModeratedByAppInstanceUserRequestTypeDef definition

class ListChannelsModeratedByAppInstanceUserRequestTypeDef(TypedDict):
    AppInstanceUserArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ChimeBearer: NotRequired[str],
```

## ListChannelsRequestTypeDef

```python
# ListChannelsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListChannelsRequestTypeDef


def get_value() -> ListChannelsRequestTypeDef:
    return {
        "AppInstanceArn": ...,
    }


# ListChannelsRequestTypeDef definition

class ListChannelsRequestTypeDef(TypedDict):
    AppInstanceArn: str,
    Privacy: NotRequired[ChannelPrivacyType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ChimeBearer: NotRequired[str],
```

1. See [:material-code-brackets: ChannelPrivacyType](./literals.md#channelprivacytype) 
## ListMediaCapturePipelinesRequestTypeDef

```python
# ListMediaCapturePipelinesRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListMediaCapturePipelinesRequestTypeDef


def get_value() -> ListMediaCapturePipelinesRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListMediaCapturePipelinesRequestTypeDef definition

class ListMediaCapturePipelinesRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListMeetingTagsRequestTypeDef

```python
# ListMeetingTagsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListMeetingTagsRequestTypeDef


def get_value() -> ListMeetingTagsRequestTypeDef:
    return {
        "MeetingId": ...,
    }


# ListMeetingTagsRequestTypeDef definition

class ListMeetingTagsRequestTypeDef(TypedDict):
    MeetingId: str,
```

## ListMeetingsRequestTypeDef

```python
# ListMeetingsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListMeetingsRequestTypeDef


def get_value() -> ListMeetingsRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListMeetingsRequestTypeDef definition

class ListMeetingsRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListPhoneNumberOrdersRequestTypeDef

```python
# ListPhoneNumberOrdersRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListPhoneNumberOrdersRequestTypeDef


def get_value() -> ListPhoneNumberOrdersRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListPhoneNumberOrdersRequestTypeDef definition

class ListPhoneNumberOrdersRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListPhoneNumbersRequestTypeDef

```python
# ListPhoneNumbersRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListPhoneNumbersRequestTypeDef


def get_value() -> ListPhoneNumbersRequestTypeDef:
    return {
        "Status": ...,
    }


# ListPhoneNumbersRequestTypeDef definition

class ListPhoneNumbersRequestTypeDef(TypedDict):
    Status: NotRequired[PhoneNumberStatusType],  # (1)
    ProductType: NotRequired[PhoneNumberProductTypeType],  # (2)
    FilterName: NotRequired[PhoneNumberAssociationNameType],  # (3)
    FilterValue: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: PhoneNumberStatusType](./literals.md#phonenumberstatustype) 
2. See [:material-code-brackets: PhoneNumberProductTypeType](./literals.md#phonenumberproducttypetype) 
3. See [:material-code-brackets: PhoneNumberAssociationNameType](./literals.md#phonenumberassociationnametype) 
## ListProxySessionsRequestTypeDef

```python
# ListProxySessionsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListProxySessionsRequestTypeDef


def get_value() -> ListProxySessionsRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# ListProxySessionsRequestTypeDef definition

class ListProxySessionsRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    Status: NotRequired[ProxySessionStatusType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: ProxySessionStatusType](./literals.md#proxysessionstatustype) 
## ListRoomMembershipsRequestTypeDef

```python
# ListRoomMembershipsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListRoomMembershipsRequestTypeDef


def get_value() -> ListRoomMembershipsRequestTypeDef:
    return {
        "AccountId": ...,
    }


# ListRoomMembershipsRequestTypeDef definition

class ListRoomMembershipsRequestTypeDef(TypedDict):
    AccountId: str,
    RoomId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListRoomsRequestTypeDef

```python
# ListRoomsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListRoomsRequestTypeDef


def get_value() -> ListRoomsRequestTypeDef:
    return {
        "AccountId": ...,
    }


# ListRoomsRequestTypeDef definition

class ListRoomsRequestTypeDef(TypedDict):
    AccountId: str,
    MemberId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListSipMediaApplicationsRequestTypeDef

```python
# ListSipMediaApplicationsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListSipMediaApplicationsRequestTypeDef


def get_value() -> ListSipMediaApplicationsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListSipMediaApplicationsRequestTypeDef definition

class ListSipMediaApplicationsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListSipRulesRequestTypeDef

```python
# ListSipRulesRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListSipRulesRequestTypeDef


def get_value() -> ListSipRulesRequestTypeDef:
    return {
        "SipMediaApplicationId": ...,
    }


# ListSipRulesRequestTypeDef definition

class ListSipRulesRequestTypeDef(TypedDict):
    SipMediaApplicationId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListSupportedPhoneNumberCountriesRequestTypeDef

```python
# ListSupportedPhoneNumberCountriesRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListSupportedPhoneNumberCountriesRequestTypeDef


def get_value() -> ListSupportedPhoneNumberCountriesRequestTypeDef:
    return {
        "ProductType": ...,
    }


# ListSupportedPhoneNumberCountriesRequestTypeDef definition

class ListSupportedPhoneNumberCountriesRequestTypeDef(TypedDict):
    ProductType: PhoneNumberProductTypeType,  # (1)
```

1. See [:material-code-brackets: PhoneNumberProductTypeType](./literals.md#phonenumberproducttypetype) 
## PhoneNumberCountryTypeDef

```python
# PhoneNumberCountryTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PhoneNumberCountryTypeDef


def get_value() -> PhoneNumberCountryTypeDef:
    return {
        "CountryCode": ...,
    }


# PhoneNumberCountryTypeDef definition

class PhoneNumberCountryTypeDef(TypedDict):
    CountryCode: NotRequired[str],
    SupportedPhoneNumberTypes: NotRequired[List[PhoneNumberTypeType]],  # (1)
```

1. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "ResourceARN": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## ListUsersRequestTypeDef

```python
# ListUsersRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListUsersRequestTypeDef


def get_value() -> ListUsersRequestTypeDef:
    return {
        "AccountId": ...,
    }


# ListUsersRequestTypeDef definition

class ListUsersRequestTypeDef(TypedDict):
    AccountId: str,
    UserEmail: NotRequired[str],
    UserType: NotRequired[UserTypeType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
## ListVoiceConnectorGroupsRequestTypeDef

```python
# ListVoiceConnectorGroupsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListVoiceConnectorGroupsRequestTypeDef


def get_value() -> ListVoiceConnectorGroupsRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListVoiceConnectorGroupsRequestTypeDef definition

class ListVoiceConnectorGroupsRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListVoiceConnectorTerminationCredentialsRequestTypeDef

```python
# ListVoiceConnectorTerminationCredentialsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListVoiceConnectorTerminationCredentialsRequestTypeDef


def get_value() -> ListVoiceConnectorTerminationCredentialsRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# ListVoiceConnectorTerminationCredentialsRequestTypeDef definition

class ListVoiceConnectorTerminationCredentialsRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## ListVoiceConnectorsRequestTypeDef

```python
# ListVoiceConnectorsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListVoiceConnectorsRequestTypeDef


def get_value() -> ListVoiceConnectorsRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListVoiceConnectorsRequestTypeDef definition

class ListVoiceConnectorsRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## LogoutUserRequestTypeDef

```python
# LogoutUserRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import LogoutUserRequestTypeDef


def get_value() -> LogoutUserRequestTypeDef:
    return {
        "AccountId": ...,
    }


# LogoutUserRequestTypeDef definition

class LogoutUserRequestTypeDef(TypedDict):
    AccountId: str,
    UserId: str,
```

## MediaPlacementTypeDef

```python
# MediaPlacementTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import MediaPlacementTypeDef


def get_value() -> MediaPlacementTypeDef:
    return {
        "AudioHostUrl": ...,
    }


# MediaPlacementTypeDef definition

class MediaPlacementTypeDef(TypedDict):
    AudioHostUrl: NotRequired[str],
    AudioFallbackUrl: NotRequired[str],
    ScreenDataUrl: NotRequired[str],
    ScreenSharingUrl: NotRequired[str],
    ScreenViewingUrl: NotRequired[str],
    SignalingUrl: NotRequired[str],
    TurnControlUrl: NotRequired[str],
    EventIngestionUrl: NotRequired[str],
```

## MemberTypeDef

```python
# MemberTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import MemberTypeDef


def get_value() -> MemberTypeDef:
    return {
        "MemberId": ...,
    }


# MemberTypeDef definition

class MemberTypeDef(TypedDict):
    MemberId: NotRequired[str],
    MemberType: NotRequired[MemberTypeType],  # (1)
    Email: NotRequired[str],
    FullName: NotRequired[str],
    AccountId: NotRequired[str],
```

1. See [:material-code-brackets: MemberTypeType](./literals.md#membertypetype) 
## OrderedPhoneNumberTypeDef

```python
# OrderedPhoneNumberTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import OrderedPhoneNumberTypeDef


def get_value() -> OrderedPhoneNumberTypeDef:
    return {
        "E164PhoneNumber": ...,
    }


# OrderedPhoneNumberTypeDef definition

class OrderedPhoneNumberTypeDef(TypedDict):
    E164PhoneNumber: NotRequired[str],
    Status: NotRequired[OrderedPhoneNumberStatusType],  # (1)
```

1. See [:material-code-brackets: OrderedPhoneNumberStatusType](./literals.md#orderedphonenumberstatustype) 
## OriginationRouteTypeDef

```python
# OriginationRouteTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import OriginationRouteTypeDef


def get_value() -> OriginationRouteTypeDef:
    return {
        "Host": ...,
    }


# OriginationRouteTypeDef definition

class OriginationRouteTypeDef(TypedDict):
    Host: NotRequired[str],
    Port: NotRequired[int],
    Protocol: NotRequired[OriginationRouteProtocolType],  # (1)
    Priority: NotRequired[int],
    Weight: NotRequired[int],
```

1. See [:material-code-brackets: OriginationRouteProtocolType](./literals.md#originationrouteprotocoltype) 
## ParticipantTypeDef

```python
# ParticipantTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ParticipantTypeDef


def get_value() -> ParticipantTypeDef:
    return {
        "PhoneNumber": ...,
    }


# ParticipantTypeDef definition

class ParticipantTypeDef(TypedDict):
    PhoneNumber: NotRequired[str],
    ProxyPhoneNumber: NotRequired[str],
```

## PhoneNumberAssociationTypeDef

```python
# PhoneNumberAssociationTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PhoneNumberAssociationTypeDef


def get_value() -> PhoneNumberAssociationTypeDef:
    return {
        "Value": ...,
    }


# PhoneNumberAssociationTypeDef definition

class PhoneNumberAssociationTypeDef(TypedDict):
    Value: NotRequired[str],
    Name: NotRequired[PhoneNumberAssociationNameType],  # (1)
    AssociatedTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: PhoneNumberAssociationNameType](./literals.md#phonenumberassociationnametype) 
## PhoneNumberCapabilitiesTypeDef

```python
# PhoneNumberCapabilitiesTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PhoneNumberCapabilitiesTypeDef


def get_value() -> PhoneNumberCapabilitiesTypeDef:
    return {
        "InboundCall": ...,
    }


# PhoneNumberCapabilitiesTypeDef definition

class PhoneNumberCapabilitiesTypeDef(TypedDict):
    InboundCall: NotRequired[bool],
    OutboundCall: NotRequired[bool],
    InboundSMS: NotRequired[bool],
    OutboundSMS: NotRequired[bool],
    InboundMMS: NotRequired[bool],
    OutboundMMS: NotRequired[bool],
```

## PutEventsConfigurationRequestTypeDef

```python
# PutEventsConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutEventsConfigurationRequestTypeDef


def get_value() -> PutEventsConfigurationRequestTypeDef:
    return {
        "AccountId": ...,
    }


# PutEventsConfigurationRequestTypeDef definition

class PutEventsConfigurationRequestTypeDef(TypedDict):
    AccountId: str,
    BotId: str,
    OutboundEventsHTTPSEndpoint: NotRequired[str],
    LambdaFunctionArn: NotRequired[str],
```

## PutVoiceConnectorProxyRequestTypeDef

```python
# PutVoiceConnectorProxyRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutVoiceConnectorProxyRequestTypeDef


def get_value() -> PutVoiceConnectorProxyRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# PutVoiceConnectorProxyRequestTypeDef definition

class PutVoiceConnectorProxyRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    DefaultSessionExpiryMinutes: int,
    PhoneNumberPoolCountries: Sequence[str],
    FallBackPhoneNumber: NotRequired[str],
    Disabled: NotRequired[bool],
```

## RedactChannelMessageRequestTypeDef

```python
# RedactChannelMessageRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import RedactChannelMessageRequestTypeDef


def get_value() -> RedactChannelMessageRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# RedactChannelMessageRequestTypeDef definition

class RedactChannelMessageRequestTypeDef(TypedDict):
    ChannelArn: str,
    MessageId: str,
    ChimeBearer: NotRequired[str],
```

## RedactConversationMessageRequestTypeDef

```python
# RedactConversationMessageRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import RedactConversationMessageRequestTypeDef


def get_value() -> RedactConversationMessageRequestTypeDef:
    return {
        "AccountId": ...,
    }


# RedactConversationMessageRequestTypeDef definition

class RedactConversationMessageRequestTypeDef(TypedDict):
    AccountId: str,
    ConversationId: str,
    MessageId: str,
```

## RedactRoomMessageRequestTypeDef

```python
# RedactRoomMessageRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import RedactRoomMessageRequestTypeDef


def get_value() -> RedactRoomMessageRequestTypeDef:
    return {
        "AccountId": ...,
    }


# RedactRoomMessageRequestTypeDef definition

class RedactRoomMessageRequestTypeDef(TypedDict):
    AccountId: str,
    RoomId: str,
    MessageId: str,
```

## RegenerateSecurityTokenRequestTypeDef

```python
# RegenerateSecurityTokenRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import RegenerateSecurityTokenRequestTypeDef


def get_value() -> RegenerateSecurityTokenRequestTypeDef:
    return {
        "AccountId": ...,
    }


# RegenerateSecurityTokenRequestTypeDef definition

class RegenerateSecurityTokenRequestTypeDef(TypedDict):
    AccountId: str,
    BotId: str,
```

## ResetPersonalPINRequestTypeDef

```python
# ResetPersonalPINRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ResetPersonalPINRequestTypeDef


def get_value() -> ResetPersonalPINRequestTypeDef:
    return {
        "AccountId": ...,
    }


# ResetPersonalPINRequestTypeDef definition

class ResetPersonalPINRequestTypeDef(TypedDict):
    AccountId: str,
    UserId: str,
```

## RestorePhoneNumberRequestTypeDef

```python
# RestorePhoneNumberRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import RestorePhoneNumberRequestTypeDef


def get_value() -> RestorePhoneNumberRequestTypeDef:
    return {
        "PhoneNumberId": ...,
    }


# RestorePhoneNumberRequestTypeDef definition

class RestorePhoneNumberRequestTypeDef(TypedDict):
    PhoneNumberId: str,
```

## RoomRetentionSettingsTypeDef

```python
# RoomRetentionSettingsTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import RoomRetentionSettingsTypeDef


def get_value() -> RoomRetentionSettingsTypeDef:
    return {
        "RetentionDays": ...,
    }


# RoomRetentionSettingsTypeDef definition

class RoomRetentionSettingsTypeDef(TypedDict):
    RetentionDays: NotRequired[int],
```

## SearchAvailablePhoneNumbersRequestTypeDef

```python
# SearchAvailablePhoneNumbersRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import SearchAvailablePhoneNumbersRequestTypeDef


def get_value() -> SearchAvailablePhoneNumbersRequestTypeDef:
    return {
        "AreaCode": ...,
    }


# SearchAvailablePhoneNumbersRequestTypeDef definition

class SearchAvailablePhoneNumbersRequestTypeDef(TypedDict):
    AreaCode: NotRequired[str],
    City: NotRequired[str],
    Country: NotRequired[str],
    State: NotRequired[str],
    TollFreePrefix: NotRequired[str],
    PhoneNumberType: NotRequired[PhoneNumberTypeType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
## SelectedVideoStreamsOutputTypeDef

```python
# SelectedVideoStreamsOutputTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import SelectedVideoStreamsOutputTypeDef


def get_value() -> SelectedVideoStreamsOutputTypeDef:
    return {
        "AttendeeIds": ...,
    }


# SelectedVideoStreamsOutputTypeDef definition

class SelectedVideoStreamsOutputTypeDef(TypedDict):
    AttendeeIds: NotRequired[List[str]],
    ExternalUserIds: NotRequired[List[str]],
```

## SelectedVideoStreamsTypeDef

```python
# SelectedVideoStreamsTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import SelectedVideoStreamsTypeDef


def get_value() -> SelectedVideoStreamsTypeDef:
    return {
        "AttendeeIds": ...,
    }


# SelectedVideoStreamsTypeDef definition

class SelectedVideoStreamsTypeDef(TypedDict):
    AttendeeIds: NotRequired[Sequence[str]],
    ExternalUserIds: NotRequired[Sequence[str]],
```

## SendChannelMessageRequestTypeDef

```python
# SendChannelMessageRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import SendChannelMessageRequestTypeDef


def get_value() -> SendChannelMessageRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# SendChannelMessageRequestTypeDef definition

class SendChannelMessageRequestTypeDef(TypedDict):
    ChannelArn: str,
    Content: str,
    Type: ChannelMessageTypeType,  # (1)
    Persistence: ChannelMessagePersistenceTypeType,  # (2)
    ClientRequestToken: str,
    Metadata: NotRequired[str],
    ChimeBearer: NotRequired[str],
```

1. See [:material-code-brackets: ChannelMessageTypeType](./literals.md#channelmessagetypetype) 
2. See [:material-code-brackets: ChannelMessagePersistenceTypeType](./literals.md#channelmessagepersistencetypetype) 
## StopMeetingTranscriptionRequestTypeDef

```python
# StopMeetingTranscriptionRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import StopMeetingTranscriptionRequestTypeDef


def get_value() -> StopMeetingTranscriptionRequestTypeDef:
    return {
        "MeetingId": ...,
    }


# StopMeetingTranscriptionRequestTypeDef definition

class StopMeetingTranscriptionRequestTypeDef(TypedDict):
    MeetingId: str,
```

## StreamingNotificationTargetTypeDef

```python
# StreamingNotificationTargetTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import StreamingNotificationTargetTypeDef


def get_value() -> StreamingNotificationTargetTypeDef:
    return {
        "NotificationTarget": ...,
    }


# StreamingNotificationTargetTypeDef definition

class StreamingNotificationTargetTypeDef(TypedDict):
    NotificationTarget: NotificationTargetType,  # (1)
```

1. See [:material-code-brackets: NotificationTargetType](./literals.md#notificationtargettype) 
## TelephonySettingsTypeDef

```python
# TelephonySettingsTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import TelephonySettingsTypeDef


def get_value() -> TelephonySettingsTypeDef:
    return {
        "InboundCalling": ...,
    }


# TelephonySettingsTypeDef definition

class TelephonySettingsTypeDef(TypedDict):
    InboundCalling: bool,
    OutboundCalling: bool,
    SMS: bool,
```

## TerminationTypeDef

```python
# TerminationTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import TerminationTypeDef


def get_value() -> TerminationTypeDef:
    return {
        "CpsLimit": ...,
    }


# TerminationTypeDef definition

class TerminationTypeDef(TypedDict):
    CpsLimit: NotRequired[int],
    DefaultPhoneNumber: NotRequired[str],
    CallingRegions: NotRequired[Sequence[str]],
    CidrAllowedList: NotRequired[Sequence[str]],
    Disabled: NotRequired[bool],
```

## UntagAttendeeRequestTypeDef

```python
# UntagAttendeeRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UntagAttendeeRequestTypeDef


def get_value() -> UntagAttendeeRequestTypeDef:
    return {
        "MeetingId": ...,
    }


# UntagAttendeeRequestTypeDef definition

class UntagAttendeeRequestTypeDef(TypedDict):
    MeetingId: str,
    AttendeeId: str,
    TagKeys: Sequence[str],
```

## UntagMeetingRequestTypeDef

```python
# UntagMeetingRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UntagMeetingRequestTypeDef


def get_value() -> UntagMeetingRequestTypeDef:
    return {
        "MeetingId": ...,
    }


# UntagMeetingRequestTypeDef definition

class UntagMeetingRequestTypeDef(TypedDict):
    MeetingId: str,
    TagKeys: Sequence[str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ResourceARN": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateAccountRequestTypeDef

```python
# UpdateAccountRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateAccountRequestTypeDef


def get_value() -> UpdateAccountRequestTypeDef:
    return {
        "AccountId": ...,
    }


# UpdateAccountRequestTypeDef definition

class UpdateAccountRequestTypeDef(TypedDict):
    AccountId: str,
    Name: NotRequired[str],
    DefaultLicense: NotRequired[LicenseType],  # (1)
```

1. See [:material-code-brackets: LicenseType](./literals.md#licensetype) 
## UpdateAppInstanceRequestTypeDef

```python
# UpdateAppInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateAppInstanceRequestTypeDef


def get_value() -> UpdateAppInstanceRequestTypeDef:
    return {
        "AppInstanceArn": ...,
    }


# UpdateAppInstanceRequestTypeDef definition

class UpdateAppInstanceRequestTypeDef(TypedDict):
    AppInstanceArn: str,
    Name: str,
    Metadata: NotRequired[str],
```

## UpdateAppInstanceUserRequestTypeDef

```python
# UpdateAppInstanceUserRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateAppInstanceUserRequestTypeDef


def get_value() -> UpdateAppInstanceUserRequestTypeDef:
    return {
        "AppInstanceUserArn": ...,
    }


# UpdateAppInstanceUserRequestTypeDef definition

class UpdateAppInstanceUserRequestTypeDef(TypedDict):
    AppInstanceUserArn: str,
    Name: str,
    Metadata: NotRequired[str],
```

## UpdateBotRequestTypeDef

```python
# UpdateBotRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateBotRequestTypeDef


def get_value() -> UpdateBotRequestTypeDef:
    return {
        "AccountId": ...,
    }


# UpdateBotRequestTypeDef definition

class UpdateBotRequestTypeDef(TypedDict):
    AccountId: str,
    BotId: str,
    Disabled: NotRequired[bool],
```

## UpdateChannelMessageRequestTypeDef

```python
# UpdateChannelMessageRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateChannelMessageRequestTypeDef


def get_value() -> UpdateChannelMessageRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# UpdateChannelMessageRequestTypeDef definition

class UpdateChannelMessageRequestTypeDef(TypedDict):
    ChannelArn: str,
    MessageId: str,
    Content: NotRequired[str],
    Metadata: NotRequired[str],
    ChimeBearer: NotRequired[str],
```

## UpdateChannelReadMarkerRequestTypeDef

```python
# UpdateChannelReadMarkerRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateChannelReadMarkerRequestTypeDef


def get_value() -> UpdateChannelReadMarkerRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# UpdateChannelReadMarkerRequestTypeDef definition

class UpdateChannelReadMarkerRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChimeBearer: NotRequired[str],
```

## UpdateChannelRequestTypeDef

```python
# UpdateChannelRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateChannelRequestTypeDef


def get_value() -> UpdateChannelRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# UpdateChannelRequestTypeDef definition

class UpdateChannelRequestTypeDef(TypedDict):
    ChannelArn: str,
    Name: str,
    Mode: ChannelModeType,  # (1)
    Metadata: NotRequired[str],
    ChimeBearer: NotRequired[str],
```

1. See [:material-code-brackets: ChannelModeType](./literals.md#channelmodetype) 
## UpdatePhoneNumberRequestTypeDef

```python
# UpdatePhoneNumberRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdatePhoneNumberRequestTypeDef


def get_value() -> UpdatePhoneNumberRequestTypeDef:
    return {
        "PhoneNumberId": ...,
    }


# UpdatePhoneNumberRequestTypeDef definition

class UpdatePhoneNumberRequestTypeDef(TypedDict):
    PhoneNumberId: str,
    ProductType: NotRequired[PhoneNumberProductTypeType],  # (1)
    CallingName: NotRequired[str],
```

1. See [:material-code-brackets: PhoneNumberProductTypeType](./literals.md#phonenumberproducttypetype) 
## UpdatePhoneNumberSettingsRequestTypeDef

```python
# UpdatePhoneNumberSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdatePhoneNumberSettingsRequestTypeDef


def get_value() -> UpdatePhoneNumberSettingsRequestTypeDef:
    return {
        "CallingName": ...,
    }


# UpdatePhoneNumberSettingsRequestTypeDef definition

class UpdatePhoneNumberSettingsRequestTypeDef(TypedDict):
    CallingName: str,
```

## UpdateProxySessionRequestTypeDef

```python
# UpdateProxySessionRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateProxySessionRequestTypeDef


def get_value() -> UpdateProxySessionRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# UpdateProxySessionRequestTypeDef definition

class UpdateProxySessionRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    ProxySessionId: str,
    Capabilities: Sequence[CapabilityType],  # (1)
    ExpiryMinutes: NotRequired[int],
```

1. See [:material-code-brackets: CapabilityType](./literals.md#capabilitytype) 
## UpdateRoomMembershipRequestTypeDef

```python
# UpdateRoomMembershipRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateRoomMembershipRequestTypeDef


def get_value() -> UpdateRoomMembershipRequestTypeDef:
    return {
        "AccountId": ...,
    }


# UpdateRoomMembershipRequestTypeDef definition

class UpdateRoomMembershipRequestTypeDef(TypedDict):
    AccountId: str,
    RoomId: str,
    MemberId: str,
    Role: NotRequired[RoomMembershipRoleType],  # (1)
```

1. See [:material-code-brackets: RoomMembershipRoleType](./literals.md#roommembershiproletype) 
## UpdateRoomRequestTypeDef

```python
# UpdateRoomRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateRoomRequestTypeDef


def get_value() -> UpdateRoomRequestTypeDef:
    return {
        "AccountId": ...,
    }


# UpdateRoomRequestTypeDef definition

class UpdateRoomRequestTypeDef(TypedDict):
    AccountId: str,
    RoomId: str,
    Name: NotRequired[str],
```

## UpdateSipMediaApplicationCallRequestTypeDef

```python
# UpdateSipMediaApplicationCallRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateSipMediaApplicationCallRequestTypeDef


def get_value() -> UpdateSipMediaApplicationCallRequestTypeDef:
    return {
        "SipMediaApplicationId": ...,
    }


# UpdateSipMediaApplicationCallRequestTypeDef definition

class UpdateSipMediaApplicationCallRequestTypeDef(TypedDict):
    SipMediaApplicationId: str,
    TransactionId: str,
    Arguments: Mapping[str, str],
```

## UpdateVoiceConnectorRequestTypeDef

```python
# UpdateVoiceConnectorRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateVoiceConnectorRequestTypeDef


def get_value() -> UpdateVoiceConnectorRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# UpdateVoiceConnectorRequestTypeDef definition

class UpdateVoiceConnectorRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    Name: str,
    RequireEncryption: bool,
```

## ValidateE911AddressRequestTypeDef

```python
# ValidateE911AddressRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ValidateE911AddressRequestTypeDef


def get_value() -> ValidateE911AddressRequestTypeDef:
    return {
        "AwsAccountId": ...,
    }


# ValidateE911AddressRequestTypeDef definition

class ValidateE911AddressRequestTypeDef(TypedDict):
    AwsAccountId: str,
    StreetNumber: str,
    StreetInfo: str,
    City: str,
    State: str,
    Country: str,
    PostalCode: str,
```

## UpdateAccountSettingsRequestTypeDef

```python
# UpdateAccountSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateAccountSettingsRequestTypeDef


def get_value() -> UpdateAccountSettingsRequestTypeDef:
    return {
        "AccountId": ...,
    }


# UpdateAccountSettingsRequestTypeDef definition

class UpdateAccountSettingsRequestTypeDef(TypedDict):
    AccountId: str,
    AccountSettings: AccountSettingsTypeDef,  # (1)
```

1. See [:material-code-braces: AccountSettingsTypeDef](./type_defs.md#accountsettingstypedef) 
## AccountTypeDef

```python
# AccountTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import AccountTypeDef


def get_value() -> AccountTypeDef:
    return {
        "AwsAccountId": ...,
    }


# AccountTypeDef definition

class AccountTypeDef(TypedDict):
    AwsAccountId: str,
    AccountId: str,
    Name: str,
    AccountType: NotRequired[AccountTypeType],  # (1)
    CreatedTimestamp: NotRequired[datetime],
    DefaultLicense: NotRequired[LicenseType],  # (2)
    SupportedLicenses: NotRequired[List[LicenseType]],  # (3)
    AccountStatus: NotRequired[AccountStatusType],  # (4)
    SigninDelegateGroups: NotRequired[List[SigninDelegateGroupTypeDef]],  # (5)
```

1. See [:material-code-brackets: AccountTypeType](./literals.md#accounttypetype) 
2. See [:material-code-brackets: LicenseType](./literals.md#licensetype) 
3. See [:material-code-brackets: LicenseType](./literals.md#licensetype) 
4. See [:material-code-brackets: AccountStatusType](./literals.md#accountstatustype) 
5. See [:material-code-braces: SigninDelegateGroupTypeDef](./type_defs.md#signindelegategrouptypedef) 
## AssociateSigninDelegateGroupsWithAccountRequestTypeDef

```python
# AssociateSigninDelegateGroupsWithAccountRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import AssociateSigninDelegateGroupsWithAccountRequestTypeDef


def get_value() -> AssociateSigninDelegateGroupsWithAccountRequestTypeDef:
    return {
        "AccountId": ...,
    }


# AssociateSigninDelegateGroupsWithAccountRequestTypeDef definition

class AssociateSigninDelegateGroupsWithAccountRequestTypeDef(TypedDict):
    AccountId: str,
    SigninDelegateGroups: Sequence[SigninDelegateGroupTypeDef],  # (1)
```

1. See [:material-code-braces: SigninDelegateGroupTypeDef](./type_defs.md#signindelegategrouptypedef) 
## UpdateUserRequestItemTypeDef

```python
# UpdateUserRequestItemTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateUserRequestItemTypeDef


def get_value() -> UpdateUserRequestItemTypeDef:
    return {
        "UserId": ...,
    }


# UpdateUserRequestItemTypeDef definition

class UpdateUserRequestItemTypeDef(TypedDict):
    UserId: str,
    LicenseType: NotRequired[LicenseType],  # (1)
    UserType: NotRequired[UserTypeType],  # (2)
    AlexaForBusinessMetadata: NotRequired[AlexaForBusinessMetadataTypeDef],  # (3)
```

1. See [:material-code-brackets: LicenseType](./literals.md#licensetype) 
2. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
3. See [:material-code-braces: AlexaForBusinessMetadataTypeDef](./type_defs.md#alexaforbusinessmetadatatypedef) 
## UpdateUserRequestTypeDef

```python
# UpdateUserRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateUserRequestTypeDef


def get_value() -> UpdateUserRequestTypeDef:
    return {
        "AccountId": ...,
    }


# UpdateUserRequestTypeDef definition

class UpdateUserRequestTypeDef(TypedDict):
    AccountId: str,
    UserId: str,
    LicenseType: NotRequired[LicenseType],  # (1)
    UserType: NotRequired[UserTypeType],  # (2)
    AlexaForBusinessMetadata: NotRequired[AlexaForBusinessMetadataTypeDef],  # (3)
```

1. See [:material-code-brackets: LicenseType](./literals.md#licensetype) 
2. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
3. See [:material-code-braces: AlexaForBusinessMetadataTypeDef](./type_defs.md#alexaforbusinessmetadatatypedef) 
## UserTypeDef

```python
# UserTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UserTypeDef


def get_value() -> UserTypeDef:
    return {
        "UserId": ...,
    }


# UserTypeDef definition

class UserTypeDef(TypedDict):
    UserId: str,
    AccountId: NotRequired[str],
    PrimaryEmail: NotRequired[str],
    PrimaryProvisionedNumber: NotRequired[str],
    DisplayName: NotRequired[str],
    LicenseType: NotRequired[LicenseType],  # (1)
    UserType: NotRequired[UserTypeType],  # (2)
    UserRegistrationStatus: NotRequired[RegistrationStatusType],  # (3)
    UserInvitationStatus: NotRequired[InviteStatusType],  # (4)
    RegisteredOn: NotRequired[datetime],
    InvitedOn: NotRequired[datetime],
    AlexaForBusinessMetadata: NotRequired[AlexaForBusinessMetadataTypeDef],  # (5)
    PersonalPIN: NotRequired[str],
```

1. See [:material-code-brackets: LicenseType](./literals.md#licensetype) 
2. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
3. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
4. See [:material-code-brackets: InviteStatusType](./literals.md#invitestatustype) 
5. See [:material-code-braces: AlexaForBusinessMetadataTypeDef](./type_defs.md#alexaforbusinessmetadatatypedef) 
## AppInstanceAdminSummaryTypeDef

```python
# AppInstanceAdminSummaryTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import AppInstanceAdminSummaryTypeDef


def get_value() -> AppInstanceAdminSummaryTypeDef:
    return {
        "Admin": ...,
    }


# AppInstanceAdminSummaryTypeDef definition

class AppInstanceAdminSummaryTypeDef(TypedDict):
    Admin: NotRequired[IdentityTypeDef],  # (1)
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
## AppInstanceAdminTypeDef

```python
# AppInstanceAdminTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import AppInstanceAdminTypeDef


def get_value() -> AppInstanceAdminTypeDef:
    return {
        "Admin": ...,
    }


# AppInstanceAdminTypeDef definition

class AppInstanceAdminTypeDef(TypedDict):
    Admin: NotRequired[IdentityTypeDef],  # (1)
    AppInstanceArn: NotRequired[str],
    CreatedTimestamp: NotRequired[datetime],
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
## BatchChannelMembershipsTypeDef

```python
# BatchChannelMembershipsTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import BatchChannelMembershipsTypeDef


def get_value() -> BatchChannelMembershipsTypeDef:
    return {
        "InvitedBy": ...,
    }


# BatchChannelMembershipsTypeDef definition

class BatchChannelMembershipsTypeDef(TypedDict):
    InvitedBy: NotRequired[IdentityTypeDef],  # (1)
    Type: NotRequired[ChannelMembershipTypeType],  # (2)
    Members: NotRequired[List[IdentityTypeDef]],  # (3)
    ChannelArn: NotRequired[str],
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
2. See [:material-code-brackets: ChannelMembershipTypeType](./literals.md#channelmembershiptypetype) 
3. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
## ChannelBanSummaryTypeDef

```python
# ChannelBanSummaryTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ChannelBanSummaryTypeDef


def get_value() -> ChannelBanSummaryTypeDef:
    return {
        "Member": ...,
    }


# ChannelBanSummaryTypeDef definition

class ChannelBanSummaryTypeDef(TypedDict):
    Member: NotRequired[IdentityTypeDef],  # (1)
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
## ChannelBanTypeDef

```python
# ChannelBanTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ChannelBanTypeDef


def get_value() -> ChannelBanTypeDef:
    return {
        "Member": ...,
    }


# ChannelBanTypeDef definition

class ChannelBanTypeDef(TypedDict):
    Member: NotRequired[IdentityTypeDef],  # (1)
    ChannelArn: NotRequired[str],
    CreatedTimestamp: NotRequired[datetime],
    CreatedBy: NotRequired[IdentityTypeDef],  # (1)
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
2. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
## ChannelMembershipSummaryTypeDef

```python
# ChannelMembershipSummaryTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ChannelMembershipSummaryTypeDef


def get_value() -> ChannelMembershipSummaryTypeDef:
    return {
        "Member": ...,
    }


# ChannelMembershipSummaryTypeDef definition

class ChannelMembershipSummaryTypeDef(TypedDict):
    Member: NotRequired[IdentityTypeDef],  # (1)
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
## ChannelMembershipTypeDef

```python
# ChannelMembershipTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ChannelMembershipTypeDef


def get_value() -> ChannelMembershipTypeDef:
    return {
        "InvitedBy": ...,
    }


# ChannelMembershipTypeDef definition

class ChannelMembershipTypeDef(TypedDict):
    InvitedBy: NotRequired[IdentityTypeDef],  # (1)
    Type: NotRequired[ChannelMembershipTypeType],  # (2)
    Member: NotRequired[IdentityTypeDef],  # (1)
    ChannelArn: NotRequired[str],
    CreatedTimestamp: NotRequired[datetime],
    LastUpdatedTimestamp: NotRequired[datetime],
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
2. See [:material-code-brackets: ChannelMembershipTypeType](./literals.md#channelmembershiptypetype) 
3. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
## ChannelMessageSummaryTypeDef

```python
# ChannelMessageSummaryTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ChannelMessageSummaryTypeDef


def get_value() -> ChannelMessageSummaryTypeDef:
    return {
        "MessageId": ...,
    }


# ChannelMessageSummaryTypeDef definition

class ChannelMessageSummaryTypeDef(TypedDict):
    MessageId: NotRequired[str],
    Content: NotRequired[str],
    Metadata: NotRequired[str],
    Type: NotRequired[ChannelMessageTypeType],  # (1)
    CreatedTimestamp: NotRequired[datetime],
    LastUpdatedTimestamp: NotRequired[datetime],
    LastEditedTimestamp: NotRequired[datetime],
    Sender: NotRequired[IdentityTypeDef],  # (2)
    Redacted: NotRequired[bool],
```

1. See [:material-code-brackets: ChannelMessageTypeType](./literals.md#channelmessagetypetype) 
2. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
## ChannelMessageTypeDef

```python
# ChannelMessageTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ChannelMessageTypeDef


def get_value() -> ChannelMessageTypeDef:
    return {
        "ChannelArn": ...,
    }


# ChannelMessageTypeDef definition

class ChannelMessageTypeDef(TypedDict):
    ChannelArn: NotRequired[str],
    MessageId: NotRequired[str],
    Content: NotRequired[str],
    Metadata: NotRequired[str],
    Type: NotRequired[ChannelMessageTypeType],  # (1)
    CreatedTimestamp: NotRequired[datetime],
    LastEditedTimestamp: NotRequired[datetime],
    LastUpdatedTimestamp: NotRequired[datetime],
    Sender: NotRequired[IdentityTypeDef],  # (2)
    Redacted: NotRequired[bool],
    Persistence: NotRequired[ChannelMessagePersistenceTypeType],  # (3)
```

1. See [:material-code-brackets: ChannelMessageTypeType](./literals.md#channelmessagetypetype) 
2. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
3. See [:material-code-brackets: ChannelMessagePersistenceTypeType](./literals.md#channelmessagepersistencetypetype) 
## ChannelModeratorSummaryTypeDef

```python
# ChannelModeratorSummaryTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ChannelModeratorSummaryTypeDef


def get_value() -> ChannelModeratorSummaryTypeDef:
    return {
        "Moderator": ...,
    }


# ChannelModeratorSummaryTypeDef definition

class ChannelModeratorSummaryTypeDef(TypedDict):
    Moderator: NotRequired[IdentityTypeDef],  # (1)
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
## ChannelModeratorTypeDef

```python
# ChannelModeratorTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ChannelModeratorTypeDef


def get_value() -> ChannelModeratorTypeDef:
    return {
        "Moderator": ...,
    }


# ChannelModeratorTypeDef definition

class ChannelModeratorTypeDef(TypedDict):
    Moderator: NotRequired[IdentityTypeDef],  # (1)
    ChannelArn: NotRequired[str],
    CreatedTimestamp: NotRequired[datetime],
    CreatedBy: NotRequired[IdentityTypeDef],  # (1)
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
2. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
## ChannelTypeDef

```python
# ChannelTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ChannelTypeDef


def get_value() -> ChannelTypeDef:
    return {
        "Name": ...,
    }


# ChannelTypeDef definition

class ChannelTypeDef(TypedDict):
    Name: NotRequired[str],
    ChannelArn: NotRequired[str],
    Mode: NotRequired[ChannelModeType],  # (1)
    Privacy: NotRequired[ChannelPrivacyType],  # (2)
    Metadata: NotRequired[str],
    CreatedBy: NotRequired[IdentityTypeDef],  # (3)
    CreatedTimestamp: NotRequired[datetime],
    LastMessageTimestamp: NotRequired[datetime],
    LastUpdatedTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: ChannelModeType](./literals.md#channelmodetype) 
2. See [:material-code-brackets: ChannelPrivacyType](./literals.md#channelprivacytype) 
3. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
## AppInstanceRetentionSettingsTypeDef

```python
# AppInstanceRetentionSettingsTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import AppInstanceRetentionSettingsTypeDef


def get_value() -> AppInstanceRetentionSettingsTypeDef:
    return {
        "ChannelRetentionSettings": ...,
    }


# AppInstanceRetentionSettingsTypeDef definition

class AppInstanceRetentionSettingsTypeDef(TypedDict):
    ChannelRetentionSettings: NotRequired[ChannelRetentionSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: ChannelRetentionSettingsTypeDef](./type_defs.md#channelretentionsettingstypedef) 
## PutAppInstanceStreamingConfigurationsRequestTypeDef

```python
# PutAppInstanceStreamingConfigurationsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutAppInstanceStreamingConfigurationsRequestTypeDef


def get_value() -> PutAppInstanceStreamingConfigurationsRequestTypeDef:
    return {
        "AppInstanceArn": ...,
    }


# PutAppInstanceStreamingConfigurationsRequestTypeDef definition

class PutAppInstanceStreamingConfigurationsRequestTypeDef(TypedDict):
    AppInstanceArn: str,
    AppInstanceStreamingConfigurations: Sequence[AppInstanceStreamingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: AppInstanceStreamingConfigurationTypeDef](./type_defs.md#appinstancestreamingconfigurationtypedef) 
## ArtifactsConfigurationTypeDef

```python
# ArtifactsConfigurationTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ArtifactsConfigurationTypeDef


def get_value() -> ArtifactsConfigurationTypeDef:
    return {
        "Audio": ...,
    }


# ArtifactsConfigurationTypeDef definition

class ArtifactsConfigurationTypeDef(TypedDict):
    Audio: AudioArtifactsConfigurationTypeDef,  # (1)
    Video: VideoArtifactsConfigurationTypeDef,  # (2)
    Content: ContentArtifactsConfigurationTypeDef,  # (3)
```

1. See [:material-code-braces: AudioArtifactsConfigurationTypeDef](./type_defs.md#audioartifactsconfigurationtypedef) 
2. See [:material-code-braces: VideoArtifactsConfigurationTypeDef](./type_defs.md#videoartifactsconfigurationtypedef) 
3. See [:material-code-braces: ContentArtifactsConfigurationTypeDef](./type_defs.md#contentartifactsconfigurationtypedef) 
## AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef

```python
# AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef


def get_value() -> AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef:
    return {
        "PhoneNumberErrors": ...,
    }


# AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef definition

class AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef(TypedDict):
    PhoneNumberErrors: List[PhoneNumberErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberErrorTypeDef](./type_defs.md#phonenumbererrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef

```python
# AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef


def get_value() -> AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef:
    return {
        "PhoneNumberErrors": ...,
    }


# AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef definition

class AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef(TypedDict):
    PhoneNumberErrors: List[PhoneNumberErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberErrorTypeDef](./type_defs.md#phonenumbererrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeletePhoneNumberResponseTypeDef

```python
# BatchDeletePhoneNumberResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import BatchDeletePhoneNumberResponseTypeDef


def get_value() -> BatchDeletePhoneNumberResponseTypeDef:
    return {
        "PhoneNumberErrors": ...,
    }


# BatchDeletePhoneNumberResponseTypeDef definition

class BatchDeletePhoneNumberResponseTypeDef(TypedDict):
    PhoneNumberErrors: List[PhoneNumberErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberErrorTypeDef](./type_defs.md#phonenumbererrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdatePhoneNumberResponseTypeDef

```python
# BatchUpdatePhoneNumberResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import BatchUpdatePhoneNumberResponseTypeDef


def get_value() -> BatchUpdatePhoneNumberResponseTypeDef:
    return {
        "PhoneNumberErrors": ...,
    }


# BatchUpdatePhoneNumberResponseTypeDef definition

class BatchUpdatePhoneNumberResponseTypeDef(TypedDict):
    PhoneNumberErrors: List[PhoneNumberErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberErrorTypeDef](./type_defs.md#phonenumbererrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAppInstanceAdminResponseTypeDef

```python
# CreateAppInstanceAdminResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateAppInstanceAdminResponseTypeDef


def get_value() -> CreateAppInstanceAdminResponseTypeDef:
    return {
        "AppInstanceAdmin": ...,
    }


# CreateAppInstanceAdminResponseTypeDef definition

class CreateAppInstanceAdminResponseTypeDef(TypedDict):
    AppInstanceAdmin: IdentityTypeDef,  # (1)
    AppInstanceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAppInstanceResponseTypeDef

```python
# CreateAppInstanceResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateAppInstanceResponseTypeDef


def get_value() -> CreateAppInstanceResponseTypeDef:
    return {
        "AppInstanceArn": ...,
    }


# CreateAppInstanceResponseTypeDef definition

class CreateAppInstanceResponseTypeDef(TypedDict):
    AppInstanceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAppInstanceUserResponseTypeDef

```python
# CreateAppInstanceUserResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateAppInstanceUserResponseTypeDef


def get_value() -> CreateAppInstanceUserResponseTypeDef:
    return {
        "AppInstanceUserArn": ...,
    }


# CreateAppInstanceUserResponseTypeDef definition

class CreateAppInstanceUserResponseTypeDef(TypedDict):
    AppInstanceUserArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateChannelBanResponseTypeDef

```python
# CreateChannelBanResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateChannelBanResponseTypeDef


def get_value() -> CreateChannelBanResponseTypeDef:
    return {
        "ChannelArn": ...,
    }


# CreateChannelBanResponseTypeDef definition

class CreateChannelBanResponseTypeDef(TypedDict):
    ChannelArn: str,
    Member: IdentityTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateChannelMembershipResponseTypeDef

```python
# CreateChannelMembershipResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateChannelMembershipResponseTypeDef


def get_value() -> CreateChannelMembershipResponseTypeDef:
    return {
        "ChannelArn": ...,
    }


# CreateChannelMembershipResponseTypeDef definition

class CreateChannelMembershipResponseTypeDef(TypedDict):
    ChannelArn: str,
    Member: IdentityTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateChannelModeratorResponseTypeDef

```python
# CreateChannelModeratorResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateChannelModeratorResponseTypeDef


def get_value() -> CreateChannelModeratorResponseTypeDef:
    return {
        "ChannelArn": ...,
    }


# CreateChannelModeratorResponseTypeDef definition

class CreateChannelModeratorResponseTypeDef(TypedDict):
    ChannelArn: str,
    ChannelModerator: IdentityTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateChannelResponseTypeDef

```python
# CreateChannelResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateChannelResponseTypeDef


def get_value() -> CreateChannelResponseTypeDef:
    return {
        "ChannelArn": ...,
    }


# CreateChannelResponseTypeDef definition

class CreateChannelResponseTypeDef(TypedDict):
    ChannelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMeetingDialOutResponseTypeDef

```python
# CreateMeetingDialOutResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateMeetingDialOutResponseTypeDef


def get_value() -> CreateMeetingDialOutResponseTypeDef:
    return {
        "TransactionId": ...,
    }


# CreateMeetingDialOutResponseTypeDef definition

class CreateMeetingDialOutResponseTypeDef(TypedDict):
    TransactionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAppInstanceResponseTypeDef

```python
# DescribeAppInstanceResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DescribeAppInstanceResponseTypeDef


def get_value() -> DescribeAppInstanceResponseTypeDef:
    return {
        "AppInstance": ...,
    }


# DescribeAppInstanceResponseTypeDef definition

class DescribeAppInstanceResponseTypeDef(TypedDict):
    AppInstance: AppInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppInstanceTypeDef](./type_defs.md#appinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAppInstanceUserResponseTypeDef

```python
# DescribeAppInstanceUserResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DescribeAppInstanceUserResponseTypeDef


def get_value() -> DescribeAppInstanceUserResponseTypeDef:
    return {
        "AppInstanceUser": ...,
    }


# DescribeAppInstanceUserResponseTypeDef definition

class DescribeAppInstanceUserResponseTypeDef(TypedDict):
    AppInstanceUser: AppInstanceUserTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppInstanceUserTypeDef](./type_defs.md#appinstanceusertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef

```python
# DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef


def get_value() -> DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef:
    return {
        "PhoneNumberErrors": ...,
    }


# DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef definition

class DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef(TypedDict):
    PhoneNumberErrors: List[PhoneNumberErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberErrorTypeDef](./type_defs.md#phonenumbererrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef

```python
# DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef


def get_value() -> DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef:
    return {
        "PhoneNumberErrors": ...,
    }


# DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef definition

class DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef(TypedDict):
    PhoneNumberErrors: List[PhoneNumberErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberErrorTypeDef](./type_defs.md#phonenumbererrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccountSettingsResponseTypeDef

```python
# GetAccountSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetAccountSettingsResponseTypeDef


def get_value() -> GetAccountSettingsResponseTypeDef:
    return {
        "AccountSettings": ...,
    }


# GetAccountSettingsResponseTypeDef definition

class GetAccountSettingsResponseTypeDef(TypedDict):
    AccountSettings: AccountSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountSettingsTypeDef](./type_defs.md#accountsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAppInstanceStreamingConfigurationsResponseTypeDef

```python
# GetAppInstanceStreamingConfigurationsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetAppInstanceStreamingConfigurationsResponseTypeDef


def get_value() -> GetAppInstanceStreamingConfigurationsResponseTypeDef:
    return {
        "AppInstanceStreamingConfigurations": ...,
    }


# GetAppInstanceStreamingConfigurationsResponseTypeDef definition

class GetAppInstanceStreamingConfigurationsResponseTypeDef(TypedDict):
    AppInstanceStreamingConfigurations: List[AppInstanceStreamingConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppInstanceStreamingConfigurationTypeDef](./type_defs.md#appinstancestreamingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPhoneNumberSettingsResponseTypeDef

```python
# GetPhoneNumberSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetPhoneNumberSettingsResponseTypeDef


def get_value() -> GetPhoneNumberSettingsResponseTypeDef:
    return {
        "CallingName": ...,
    }


# GetPhoneNumberSettingsResponseTypeDef definition

class GetPhoneNumberSettingsResponseTypeDef(TypedDict):
    CallingName: str,
    CallingNameUpdatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAppInstanceUsersResponseTypeDef

```python
# ListAppInstanceUsersResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListAppInstanceUsersResponseTypeDef


def get_value() -> ListAppInstanceUsersResponseTypeDef:
    return {
        "AppInstanceArn": ...,
    }


# ListAppInstanceUsersResponseTypeDef definition

class ListAppInstanceUsersResponseTypeDef(TypedDict):
    AppInstanceArn: str,
    AppInstanceUsers: List[AppInstanceUserSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AppInstanceUserSummaryTypeDef](./type_defs.md#appinstanceusersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAppInstancesResponseTypeDef

```python
# ListAppInstancesResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListAppInstancesResponseTypeDef


def get_value() -> ListAppInstancesResponseTypeDef:
    return {
        "AppInstances": ...,
    }


# ListAppInstancesResponseTypeDef definition

class ListAppInstancesResponseTypeDef(TypedDict):
    AppInstances: List[AppInstanceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AppInstanceSummaryTypeDef](./type_defs.md#appinstancesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVoiceConnectorTerminationCredentialsResponseTypeDef

```python
# ListVoiceConnectorTerminationCredentialsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListVoiceConnectorTerminationCredentialsResponseTypeDef


def get_value() -> ListVoiceConnectorTerminationCredentialsResponseTypeDef:
    return {
        "Usernames": ...,
    }


# ListVoiceConnectorTerminationCredentialsResponseTypeDef definition

class ListVoiceConnectorTerminationCredentialsResponseTypeDef(TypedDict):
    Usernames: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAppInstanceStreamingConfigurationsResponseTypeDef

```python
# PutAppInstanceStreamingConfigurationsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutAppInstanceStreamingConfigurationsResponseTypeDef


def get_value() -> PutAppInstanceStreamingConfigurationsResponseTypeDef:
    return {
        "AppInstanceStreamingConfigurations": ...,
    }


# PutAppInstanceStreamingConfigurationsResponseTypeDef definition

class PutAppInstanceStreamingConfigurationsResponseTypeDef(TypedDict):
    AppInstanceStreamingConfigurations: List[AppInstanceStreamingConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppInstanceStreamingConfigurationTypeDef](./type_defs.md#appinstancestreamingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RedactChannelMessageResponseTypeDef

```python
# RedactChannelMessageResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import RedactChannelMessageResponseTypeDef


def get_value() -> RedactChannelMessageResponseTypeDef:
    return {
        "ChannelArn": ...,
    }


# RedactChannelMessageResponseTypeDef definition

class RedactChannelMessageResponseTypeDef(TypedDict):
    ChannelArn: str,
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchAvailablePhoneNumbersResponseTypeDef

```python
# SearchAvailablePhoneNumbersResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import SearchAvailablePhoneNumbersResponseTypeDef


def get_value() -> SearchAvailablePhoneNumbersResponseTypeDef:
    return {
        "E164PhoneNumbers": ...,
    }


# SearchAvailablePhoneNumbersResponseTypeDef definition

class SearchAvailablePhoneNumbersResponseTypeDef(TypedDict):
    E164PhoneNumbers: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendChannelMessageResponseTypeDef

```python
# SendChannelMessageResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import SendChannelMessageResponseTypeDef


def get_value() -> SendChannelMessageResponseTypeDef:
    return {
        "ChannelArn": ...,
    }


# SendChannelMessageResponseTypeDef definition

class SendChannelMessageResponseTypeDef(TypedDict):
    ChannelArn: str,
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAppInstanceResponseTypeDef

```python
# UpdateAppInstanceResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateAppInstanceResponseTypeDef


def get_value() -> UpdateAppInstanceResponseTypeDef:
    return {
        "AppInstanceArn": ...,
    }


# UpdateAppInstanceResponseTypeDef definition

class UpdateAppInstanceResponseTypeDef(TypedDict):
    AppInstanceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAppInstanceUserResponseTypeDef

```python
# UpdateAppInstanceUserResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateAppInstanceUserResponseTypeDef


def get_value() -> UpdateAppInstanceUserResponseTypeDef:
    return {
        "AppInstanceUserArn": ...,
    }


# UpdateAppInstanceUserResponseTypeDef definition

class UpdateAppInstanceUserResponseTypeDef(TypedDict):
    AppInstanceUserArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateChannelMessageResponseTypeDef

```python
# UpdateChannelMessageResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateChannelMessageResponseTypeDef


def get_value() -> UpdateChannelMessageResponseTypeDef:
    return {
        "ChannelArn": ...,
    }


# UpdateChannelMessageResponseTypeDef definition

class UpdateChannelMessageResponseTypeDef(TypedDict):
    ChannelArn: str,
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateChannelReadMarkerResponseTypeDef

```python
# UpdateChannelReadMarkerResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateChannelReadMarkerResponseTypeDef


def get_value() -> UpdateChannelReadMarkerResponseTypeDef:
    return {
        "ChannelArn": ...,
    }


# UpdateChannelReadMarkerResponseTypeDef definition

class UpdateChannelReadMarkerResponseTypeDef(TypedDict):
    ChannelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateChannelResponseTypeDef

```python
# UpdateChannelResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateChannelResponseTypeDef


def get_value() -> UpdateChannelResponseTypeDef:
    return {
        "ChannelArn": ...,
    }


# UpdateChannelResponseTypeDef definition

class UpdateChannelResponseTypeDef(TypedDict):
    ChannelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAttendeeResponseTypeDef

```python
# CreateAttendeeResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateAttendeeResponseTypeDef


def get_value() -> CreateAttendeeResponseTypeDef:
    return {
        "Attendee": ...,
    }


# CreateAttendeeResponseTypeDef definition

class CreateAttendeeResponseTypeDef(TypedDict):
    Attendee: AttendeeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttendeeTypeDef](./type_defs.md#attendeetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAttendeeResponseTypeDef

```python
# GetAttendeeResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetAttendeeResponseTypeDef


def get_value() -> GetAttendeeResponseTypeDef:
    return {
        "Attendee": ...,
    }


# GetAttendeeResponseTypeDef definition

class GetAttendeeResponseTypeDef(TypedDict):
    Attendee: AttendeeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttendeeTypeDef](./type_defs.md#attendeetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAttendeesResponseTypeDef

```python
# ListAttendeesResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListAttendeesResponseTypeDef


def get_value() -> ListAttendeesResponseTypeDef:
    return {
        "Attendees": ...,
    }


# ListAttendeesResponseTypeDef definition

class ListAttendeesResponseTypeDef(TypedDict):
    Attendees: List[AttendeeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AttendeeTypeDef](./type_defs.md#attendeetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchCreateAttendeeResponseTypeDef

```python
# BatchCreateAttendeeResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import BatchCreateAttendeeResponseTypeDef


def get_value() -> BatchCreateAttendeeResponseTypeDef:
    return {
        "Attendees": ...,
    }


# BatchCreateAttendeeResponseTypeDef definition

class BatchCreateAttendeeResponseTypeDef(TypedDict):
    Attendees: List[AttendeeTypeDef],  # (1)
    Errors: List[CreateAttendeeErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AttendeeTypeDef](./type_defs.md#attendeetypedef) 
2. See [:material-code-braces: CreateAttendeeErrorTypeDef](./type_defs.md#createattendeeerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchCreateRoomMembershipRequestTypeDef

```python
# BatchCreateRoomMembershipRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import BatchCreateRoomMembershipRequestTypeDef


def get_value() -> BatchCreateRoomMembershipRequestTypeDef:
    return {
        "AccountId": ...,
    }


# BatchCreateRoomMembershipRequestTypeDef definition

class BatchCreateRoomMembershipRequestTypeDef(TypedDict):
    AccountId: str,
    RoomId: str,
    MembershipItemList: Sequence[MembershipItemTypeDef],  # (1)
```

1. See [:material-code-braces: MembershipItemTypeDef](./type_defs.md#membershipitemtypedef) 
## BatchCreateRoomMembershipResponseTypeDef

```python
# BatchCreateRoomMembershipResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import BatchCreateRoomMembershipResponseTypeDef


def get_value() -> BatchCreateRoomMembershipResponseTypeDef:
    return {
        "Errors": ...,
    }


# BatchCreateRoomMembershipResponseTypeDef definition

class BatchCreateRoomMembershipResponseTypeDef(TypedDict):
    Errors: List[MemberErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MemberErrorTypeDef](./type_defs.md#membererrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchSuspendUserResponseTypeDef

```python
# BatchSuspendUserResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import BatchSuspendUserResponseTypeDef


def get_value() -> BatchSuspendUserResponseTypeDef:
    return {
        "UserErrors": ...,
    }


# BatchSuspendUserResponseTypeDef definition

class BatchSuspendUserResponseTypeDef(TypedDict):
    UserErrors: List[UserErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserErrorTypeDef](./type_defs.md#usererrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUnsuspendUserResponseTypeDef

```python
# BatchUnsuspendUserResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import BatchUnsuspendUserResponseTypeDef


def get_value() -> BatchUnsuspendUserResponseTypeDef:
    return {
        "UserErrors": ...,
    }


# BatchUnsuspendUserResponseTypeDef definition

class BatchUnsuspendUserResponseTypeDef(TypedDict):
    UserErrors: List[UserErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserErrorTypeDef](./type_defs.md#usererrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateUserResponseTypeDef

```python
# BatchUpdateUserResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import BatchUpdateUserResponseTypeDef


def get_value() -> BatchUpdateUserResponseTypeDef:
    return {
        "UserErrors": ...,
    }


# BatchUpdateUserResponseTypeDef definition

class BatchUpdateUserResponseTypeDef(TypedDict):
    UserErrors: List[UserErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserErrorTypeDef](./type_defs.md#usererrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdatePhoneNumberRequestTypeDef

```python
# BatchUpdatePhoneNumberRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import BatchUpdatePhoneNumberRequestTypeDef


def get_value() -> BatchUpdatePhoneNumberRequestTypeDef:
    return {
        "UpdatePhoneNumberRequestItems": ...,
    }


# BatchUpdatePhoneNumberRequestTypeDef definition

class BatchUpdatePhoneNumberRequestTypeDef(TypedDict):
    UpdatePhoneNumberRequestItems: Sequence[UpdatePhoneNumberRequestItemTypeDef],  # (1)
```

1. See [:material-code-braces: UpdatePhoneNumberRequestItemTypeDef](./type_defs.md#updatephonenumberrequestitemtypedef) 
## CreateBotResponseTypeDef

```python
# CreateBotResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateBotResponseTypeDef


def get_value() -> CreateBotResponseTypeDef:
    return {
        "Bot": ...,
    }


# CreateBotResponseTypeDef definition

class CreateBotResponseTypeDef(TypedDict):
    Bot: BotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BotTypeDef](./type_defs.md#bottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBotResponseTypeDef

```python
# GetBotResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetBotResponseTypeDef


def get_value() -> GetBotResponseTypeDef:
    return {
        "Bot": ...,
    }


# GetBotResponseTypeDef definition

class GetBotResponseTypeDef(TypedDict):
    Bot: BotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BotTypeDef](./type_defs.md#bottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBotsResponseTypeDef

```python
# ListBotsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListBotsResponseTypeDef


def get_value() -> ListBotsResponseTypeDef:
    return {
        "Bots": ...,
    }


# ListBotsResponseTypeDef definition

class ListBotsResponseTypeDef(TypedDict):
    Bots: List[BotTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BotTypeDef](./type_defs.md#bottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegenerateSecurityTokenResponseTypeDef

```python
# RegenerateSecurityTokenResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import RegenerateSecurityTokenResponseTypeDef


def get_value() -> RegenerateSecurityTokenResponseTypeDef:
    return {
        "Bot": ...,
    }


# RegenerateSecurityTokenResponseTypeDef definition

class RegenerateSecurityTokenResponseTypeDef(TypedDict):
    Bot: BotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BotTypeDef](./type_defs.md#bottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBotResponseTypeDef

```python
# UpdateBotResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateBotResponseTypeDef


def get_value() -> UpdateBotResponseTypeDef:
    return {
        "Bot": ...,
    }


# UpdateBotResponseTypeDef definition

class UpdateBotResponseTypeDef(TypedDict):
    Bot: BotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BotTypeDef](./type_defs.md#bottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ValidateE911AddressResponseTypeDef

```python
# ValidateE911AddressResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ValidateE911AddressResponseTypeDef


def get_value() -> ValidateE911AddressResponseTypeDef:
    return {
        "ValidationResult": ...,
    }


# ValidateE911AddressResponseTypeDef definition

class ValidateE911AddressResponseTypeDef(TypedDict):
    ValidationResult: int,
    AddressExternalId: str,
    Address: AddressTypeDef,  # (1)
    CandidateAddressList: List[CandidateAddressTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
2. See [:material-code-braces: CandidateAddressTypeDef](./type_defs.md#candidateaddresstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ChannelMembershipForAppInstanceUserSummaryTypeDef

```python
# ChannelMembershipForAppInstanceUserSummaryTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ChannelMembershipForAppInstanceUserSummaryTypeDef


def get_value() -> ChannelMembershipForAppInstanceUserSummaryTypeDef:
    return {
        "ChannelSummary": ...,
    }


# ChannelMembershipForAppInstanceUserSummaryTypeDef definition

class ChannelMembershipForAppInstanceUserSummaryTypeDef(TypedDict):
    ChannelSummary: NotRequired[ChannelSummaryTypeDef],  # (1)
    AppInstanceUserMembershipSummary: NotRequired[AppInstanceUserMembershipSummaryTypeDef],  # (2)
```

1. See [:material-code-braces: ChannelSummaryTypeDef](./type_defs.md#channelsummarytypedef) 
2. See [:material-code-braces: AppInstanceUserMembershipSummaryTypeDef](./type_defs.md#appinstanceusermembershipsummarytypedef) 
## ChannelModeratedByAppInstanceUserSummaryTypeDef

```python
# ChannelModeratedByAppInstanceUserSummaryTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ChannelModeratedByAppInstanceUserSummaryTypeDef


def get_value() -> ChannelModeratedByAppInstanceUserSummaryTypeDef:
    return {
        "ChannelSummary": ...,
    }


# ChannelModeratedByAppInstanceUserSummaryTypeDef definition

class ChannelModeratedByAppInstanceUserSummaryTypeDef(TypedDict):
    ChannelSummary: NotRequired[ChannelSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: ChannelSummaryTypeDef](./type_defs.md#channelsummarytypedef) 
## ListChannelsResponseTypeDef

```python
# ListChannelsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListChannelsResponseTypeDef


def get_value() -> ListChannelsResponseTypeDef:
    return {
        "Channels": ...,
    }


# ListChannelsResponseTypeDef definition

class ListChannelsResponseTypeDef(TypedDict):
    Channels: List[ChannelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ChannelSummaryTypeDef](./type_defs.md#channelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAppInstanceRequestTypeDef

```python
# CreateAppInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateAppInstanceRequestTypeDef


def get_value() -> CreateAppInstanceRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateAppInstanceRequestTypeDef definition

class CreateAppInstanceRequestTypeDef(TypedDict):
    Name: str,
    ClientRequestToken: str,
    Metadata: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateAppInstanceUserRequestTypeDef

```python
# CreateAppInstanceUserRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateAppInstanceUserRequestTypeDef


def get_value() -> CreateAppInstanceUserRequestTypeDef:
    return {
        "AppInstanceArn": ...,
    }


# CreateAppInstanceUserRequestTypeDef definition

class CreateAppInstanceUserRequestTypeDef(TypedDict):
    AppInstanceArn: str,
    AppInstanceUserId: str,
    Name: str,
    ClientRequestToken: str,
    Metadata: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateAttendeeRequestItemTypeDef

```python
# CreateAttendeeRequestItemTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateAttendeeRequestItemTypeDef


def get_value() -> CreateAttendeeRequestItemTypeDef:
    return {
        "ExternalUserId": ...,
    }


# CreateAttendeeRequestItemTypeDef definition

class CreateAttendeeRequestItemTypeDef(TypedDict):
    ExternalUserId: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateAttendeeRequestTypeDef

```python
# CreateAttendeeRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateAttendeeRequestTypeDef


def get_value() -> CreateAttendeeRequestTypeDef:
    return {
        "MeetingId": ...,
    }


# CreateAttendeeRequestTypeDef definition

class CreateAttendeeRequestTypeDef(TypedDict):
    MeetingId: str,
    ExternalUserId: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateChannelRequestTypeDef

```python
# CreateChannelRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateChannelRequestTypeDef


def get_value() -> CreateChannelRequestTypeDef:
    return {
        "AppInstanceArn": ...,
    }


# CreateChannelRequestTypeDef definition

class CreateChannelRequestTypeDef(TypedDict):
    AppInstanceArn: str,
    Name: str,
    ClientRequestToken: str,
    Mode: NotRequired[ChannelModeType],  # (1)
    Privacy: NotRequired[ChannelPrivacyType],  # (2)
    Metadata: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    ChimeBearer: NotRequired[str],
```

1. See [:material-code-brackets: ChannelModeType](./literals.md#channelmodetype) 
2. See [:material-code-brackets: ChannelPrivacyType](./literals.md#channelprivacytype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListAttendeeTagsResponseTypeDef

```python
# ListAttendeeTagsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListAttendeeTagsResponseTypeDef


def get_value() -> ListAttendeeTagsResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListAttendeeTagsResponseTypeDef definition

class ListAttendeeTagsResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMeetingTagsResponseTypeDef

```python
# ListMeetingTagsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListMeetingTagsResponseTypeDef


def get_value() -> ListMeetingTagsResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListMeetingTagsResponseTypeDef definition

class ListMeetingTagsResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagAttendeeRequestTypeDef

```python
# TagAttendeeRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import TagAttendeeRequestTypeDef


def get_value() -> TagAttendeeRequestTypeDef:
    return {
        "MeetingId": ...,
    }


# TagAttendeeRequestTypeDef definition

class TagAttendeeRequestTypeDef(TypedDict):
    MeetingId: str,
    AttendeeId: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagMeetingRequestTypeDef

```python
# TagMeetingRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import TagMeetingRequestTypeDef


def get_value() -> TagMeetingRequestTypeDef:
    return {
        "MeetingId": ...,
    }


# TagMeetingRequestTypeDef definition

class TagMeetingRequestTypeDef(TypedDict):
    MeetingId: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "ResourceARN": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateMeetingRequestTypeDef

```python
# CreateMeetingRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateMeetingRequestTypeDef


def get_value() -> CreateMeetingRequestTypeDef:
    return {
        "ClientRequestToken": ...,
    }


# CreateMeetingRequestTypeDef definition

class CreateMeetingRequestTypeDef(TypedDict):
    ClientRequestToken: str,
    ExternalMeetingId: NotRequired[str],
    MeetingHostId: NotRequired[str],
    MediaRegion: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    NotificationsConfiguration: NotRequired[MeetingNotificationConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: MeetingNotificationConfigurationTypeDef](./type_defs.md#meetingnotificationconfigurationtypedef) 
## CreateProxySessionRequestTypeDef

```python
# CreateProxySessionRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateProxySessionRequestTypeDef


def get_value() -> CreateProxySessionRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# CreateProxySessionRequestTypeDef definition

class CreateProxySessionRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    ParticipantPhoneNumbers: Sequence[str],
    Capabilities: Sequence[CapabilityType],  # (1)
    Name: NotRequired[str],
    ExpiryMinutes: NotRequired[int],
    NumberSelectionBehavior: NotRequired[NumberSelectionBehaviorType],  # (2)
    GeoMatchLevel: NotRequired[GeoMatchLevelType],  # (3)
    GeoMatchParams: NotRequired[GeoMatchParamsTypeDef],  # (4)
```

1. See [:material-code-brackets: CapabilityType](./literals.md#capabilitytype) 
2. See [:material-code-brackets: NumberSelectionBehaviorType](./literals.md#numberselectionbehaviortype) 
3. See [:material-code-brackets: GeoMatchLevelType](./literals.md#geomatchleveltype) 
4. See [:material-code-braces: GeoMatchParamsTypeDef](./type_defs.md#geomatchparamstypedef) 
## CreateRoomResponseTypeDef

```python
# CreateRoomResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateRoomResponseTypeDef


def get_value() -> CreateRoomResponseTypeDef:
    return {
        "Room": ...,
    }


# CreateRoomResponseTypeDef definition

class CreateRoomResponseTypeDef(TypedDict):
    Room: RoomTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoomTypeDef](./type_defs.md#roomtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRoomResponseTypeDef

```python
# GetRoomResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetRoomResponseTypeDef


def get_value() -> GetRoomResponseTypeDef:
    return {
        "Room": ...,
    }


# GetRoomResponseTypeDef definition

class GetRoomResponseTypeDef(TypedDict):
    Room: RoomTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoomTypeDef](./type_defs.md#roomtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRoomsResponseTypeDef

```python
# ListRoomsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListRoomsResponseTypeDef


def get_value() -> ListRoomsResponseTypeDef:
    return {
        "Rooms": ...,
    }


# ListRoomsResponseTypeDef definition

class ListRoomsResponseTypeDef(TypedDict):
    Rooms: List[RoomTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RoomTypeDef](./type_defs.md#roomtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRoomResponseTypeDef

```python
# UpdateRoomResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateRoomResponseTypeDef


def get_value() -> UpdateRoomResponseTypeDef:
    return {
        "Room": ...,
    }


# UpdateRoomResponseTypeDef definition

class UpdateRoomResponseTypeDef(TypedDict):
    Room: RoomTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoomTypeDef](./type_defs.md#roomtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSipMediaApplicationCallResponseTypeDef

```python
# CreateSipMediaApplicationCallResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateSipMediaApplicationCallResponseTypeDef


def get_value() -> CreateSipMediaApplicationCallResponseTypeDef:
    return {
        "SipMediaApplicationCall": ...,
    }


# CreateSipMediaApplicationCallResponseTypeDef definition

class CreateSipMediaApplicationCallResponseTypeDef(TypedDict):
    SipMediaApplicationCall: SipMediaApplicationCallTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SipMediaApplicationCallTypeDef](./type_defs.md#sipmediaapplicationcalltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSipMediaApplicationCallResponseTypeDef

```python
# UpdateSipMediaApplicationCallResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateSipMediaApplicationCallResponseTypeDef


def get_value() -> UpdateSipMediaApplicationCallResponseTypeDef:
    return {
        "SipMediaApplicationCall": ...,
    }


# UpdateSipMediaApplicationCallResponseTypeDef definition

class UpdateSipMediaApplicationCallResponseTypeDef(TypedDict):
    SipMediaApplicationCall: SipMediaApplicationCallTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SipMediaApplicationCallTypeDef](./type_defs.md#sipmediaapplicationcalltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSipMediaApplicationRequestTypeDef

```python
# CreateSipMediaApplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateSipMediaApplicationRequestTypeDef


def get_value() -> CreateSipMediaApplicationRequestTypeDef:
    return {
        "AwsRegion": ...,
    }


# CreateSipMediaApplicationRequestTypeDef definition

class CreateSipMediaApplicationRequestTypeDef(TypedDict):
    AwsRegion: str,
    Name: str,
    Endpoints: Sequence[SipMediaApplicationEndpointTypeDef],  # (1)
```

1. See [:material-code-braces: SipMediaApplicationEndpointTypeDef](./type_defs.md#sipmediaapplicationendpointtypedef) 
## SipMediaApplicationTypeDef

```python
# SipMediaApplicationTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import SipMediaApplicationTypeDef


def get_value() -> SipMediaApplicationTypeDef:
    return {
        "SipMediaApplicationId": ...,
    }


# SipMediaApplicationTypeDef definition

class SipMediaApplicationTypeDef(TypedDict):
    SipMediaApplicationId: NotRequired[str],
    AwsRegion: NotRequired[str],
    Name: NotRequired[str],
    Endpoints: NotRequired[List[SipMediaApplicationEndpointTypeDef]],  # (1)
    CreatedTimestamp: NotRequired[datetime],
    UpdatedTimestamp: NotRequired[datetime],
```

1. See [:material-code-braces: SipMediaApplicationEndpointTypeDef](./type_defs.md#sipmediaapplicationendpointtypedef) 
## UpdateSipMediaApplicationRequestTypeDef

```python
# UpdateSipMediaApplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateSipMediaApplicationRequestTypeDef


def get_value() -> UpdateSipMediaApplicationRequestTypeDef:
    return {
        "SipMediaApplicationId": ...,
    }


# UpdateSipMediaApplicationRequestTypeDef definition

class UpdateSipMediaApplicationRequestTypeDef(TypedDict):
    SipMediaApplicationId: str,
    Name: NotRequired[str],
    Endpoints: NotRequired[Sequence[SipMediaApplicationEndpointTypeDef]],  # (1)
```

1. See [:material-code-braces: SipMediaApplicationEndpointTypeDef](./type_defs.md#sipmediaapplicationendpointtypedef) 
## CreateSipRuleRequestTypeDef

```python
# CreateSipRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateSipRuleRequestTypeDef


def get_value() -> CreateSipRuleRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateSipRuleRequestTypeDef definition

class CreateSipRuleRequestTypeDef(TypedDict):
    Name: str,
    TriggerType: SipRuleTriggerTypeType,  # (1)
    TriggerValue: str,
    TargetApplications: Sequence[SipRuleTargetApplicationTypeDef],  # (2)
    Disabled: NotRequired[bool],
```

1. See [:material-code-brackets: SipRuleTriggerTypeType](./literals.md#sipruletriggertypetype) 
2. See [:material-code-braces: SipRuleTargetApplicationTypeDef](./type_defs.md#sipruletargetapplicationtypedef) 
## SipRuleTypeDef

```python
# SipRuleTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import SipRuleTypeDef


def get_value() -> SipRuleTypeDef:
    return {
        "SipRuleId": ...,
    }


# SipRuleTypeDef definition

class SipRuleTypeDef(TypedDict):
    SipRuleId: NotRequired[str],
    Name: NotRequired[str],
    Disabled: NotRequired[bool],
    TriggerType: NotRequired[SipRuleTriggerTypeType],  # (1)
    TriggerValue: NotRequired[str],
    TargetApplications: NotRequired[List[SipRuleTargetApplicationTypeDef]],  # (2)
    CreatedTimestamp: NotRequired[datetime],
    UpdatedTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: SipRuleTriggerTypeType](./literals.md#sipruletriggertypetype) 
2. See [:material-code-braces: SipRuleTargetApplicationTypeDef](./type_defs.md#sipruletargetapplicationtypedef) 
## UpdateSipRuleRequestTypeDef

```python
# UpdateSipRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateSipRuleRequestTypeDef


def get_value() -> UpdateSipRuleRequestTypeDef:
    return {
        "SipRuleId": ...,
    }


# UpdateSipRuleRequestTypeDef definition

class UpdateSipRuleRequestTypeDef(TypedDict):
    SipRuleId: str,
    Name: str,
    Disabled: NotRequired[bool],
    TargetApplications: NotRequired[Sequence[SipRuleTargetApplicationTypeDef]],  # (1)
```

1. See [:material-code-braces: SipRuleTargetApplicationTypeDef](./type_defs.md#sipruletargetapplicationtypedef) 
## CreateVoiceConnectorGroupRequestTypeDef

```python
# CreateVoiceConnectorGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateVoiceConnectorGroupRequestTypeDef


def get_value() -> CreateVoiceConnectorGroupRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateVoiceConnectorGroupRequestTypeDef definition

class CreateVoiceConnectorGroupRequestTypeDef(TypedDict):
    Name: str,
    VoiceConnectorItems: NotRequired[Sequence[VoiceConnectorItemTypeDef]],  # (1)
```

1. See [:material-code-braces: VoiceConnectorItemTypeDef](./type_defs.md#voiceconnectoritemtypedef) 
## UpdateVoiceConnectorGroupRequestTypeDef

```python
# UpdateVoiceConnectorGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateVoiceConnectorGroupRequestTypeDef


def get_value() -> UpdateVoiceConnectorGroupRequestTypeDef:
    return {
        "VoiceConnectorGroupId": ...,
    }


# UpdateVoiceConnectorGroupRequestTypeDef definition

class UpdateVoiceConnectorGroupRequestTypeDef(TypedDict):
    VoiceConnectorGroupId: str,
    Name: str,
    VoiceConnectorItems: Sequence[VoiceConnectorItemTypeDef],  # (1)
```

1. See [:material-code-braces: VoiceConnectorItemTypeDef](./type_defs.md#voiceconnectoritemtypedef) 
## VoiceConnectorGroupTypeDef

```python
# VoiceConnectorGroupTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import VoiceConnectorGroupTypeDef


def get_value() -> VoiceConnectorGroupTypeDef:
    return {
        "VoiceConnectorGroupId": ...,
    }


# VoiceConnectorGroupTypeDef definition

class VoiceConnectorGroupTypeDef(TypedDict):
    VoiceConnectorGroupId: NotRequired[str],
    Name: NotRequired[str],
    VoiceConnectorItems: NotRequired[List[VoiceConnectorItemTypeDef]],  # (1)
    CreatedTimestamp: NotRequired[datetime],
    UpdatedTimestamp: NotRequired[datetime],
    VoiceConnectorGroupArn: NotRequired[str],
```

1. See [:material-code-braces: VoiceConnectorItemTypeDef](./type_defs.md#voiceconnectoritemtypedef) 
## CreateVoiceConnectorResponseTypeDef

```python
# CreateVoiceConnectorResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateVoiceConnectorResponseTypeDef


def get_value() -> CreateVoiceConnectorResponseTypeDef:
    return {
        "VoiceConnector": ...,
    }


# CreateVoiceConnectorResponseTypeDef definition

class CreateVoiceConnectorResponseTypeDef(TypedDict):
    VoiceConnector: VoiceConnectorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VoiceConnectorTypeDef](./type_defs.md#voiceconnectortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVoiceConnectorResponseTypeDef

```python
# GetVoiceConnectorResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetVoiceConnectorResponseTypeDef


def get_value() -> GetVoiceConnectorResponseTypeDef:
    return {
        "VoiceConnector": ...,
    }


# GetVoiceConnectorResponseTypeDef definition

class GetVoiceConnectorResponseTypeDef(TypedDict):
    VoiceConnector: VoiceConnectorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VoiceConnectorTypeDef](./type_defs.md#voiceconnectortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVoiceConnectorsResponseTypeDef

```python
# ListVoiceConnectorsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListVoiceConnectorsResponseTypeDef


def get_value() -> ListVoiceConnectorsResponseTypeDef:
    return {
        "VoiceConnectors": ...,
    }


# ListVoiceConnectorsResponseTypeDef definition

class ListVoiceConnectorsResponseTypeDef(TypedDict):
    VoiceConnectors: List[VoiceConnectorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: VoiceConnectorTypeDef](./type_defs.md#voiceconnectortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateVoiceConnectorResponseTypeDef

```python
# UpdateVoiceConnectorResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateVoiceConnectorResponseTypeDef


def get_value() -> UpdateVoiceConnectorResponseTypeDef:
    return {
        "VoiceConnector": ...,
    }


# UpdateVoiceConnectorResponseTypeDef definition

class UpdateVoiceConnectorResponseTypeDef(TypedDict):
    VoiceConnector: VoiceConnectorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VoiceConnectorTypeDef](./type_defs.md#voiceconnectortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutVoiceConnectorTerminationCredentialsRequestTypeDef

```python
# PutVoiceConnectorTerminationCredentialsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutVoiceConnectorTerminationCredentialsRequestTypeDef


def get_value() -> PutVoiceConnectorTerminationCredentialsRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# PutVoiceConnectorTerminationCredentialsRequestTypeDef definition

class PutVoiceConnectorTerminationCredentialsRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    Credentials: NotRequired[Sequence[CredentialTypeDef]],  # (1)
```

1. See [:material-code-braces: CredentialTypeDef](./type_defs.md#credentialtypedef) 
## EmergencyCallingConfigurationOutputTypeDef

```python
# EmergencyCallingConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import EmergencyCallingConfigurationOutputTypeDef


def get_value() -> EmergencyCallingConfigurationOutputTypeDef:
    return {
        "DNIS": ...,
    }


# EmergencyCallingConfigurationOutputTypeDef definition

class EmergencyCallingConfigurationOutputTypeDef(TypedDict):
    DNIS: NotRequired[List[DNISEmergencyCallingConfigurationTypeDef]],  # (1)
```

1. See [:material-code-braces: DNISEmergencyCallingConfigurationTypeDef](./type_defs.md#dnisemergencycallingconfigurationtypedef) 
## EmergencyCallingConfigurationTypeDef

```python
# EmergencyCallingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import EmergencyCallingConfigurationTypeDef


def get_value() -> EmergencyCallingConfigurationTypeDef:
    return {
        "DNIS": ...,
    }


# EmergencyCallingConfigurationTypeDef definition

class EmergencyCallingConfigurationTypeDef(TypedDict):
    DNIS: NotRequired[Sequence[DNISEmergencyCallingConfigurationTypeDef]],  # (1)
```

1. See [:material-code-braces: DNISEmergencyCallingConfigurationTypeDef](./type_defs.md#dnisemergencycallingconfigurationtypedef) 
## TranscriptionConfigurationTypeDef

```python
# TranscriptionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import TranscriptionConfigurationTypeDef


def get_value() -> TranscriptionConfigurationTypeDef:
    return {
        "EngineTranscribeSettings": ...,
    }


# TranscriptionConfigurationTypeDef definition

class TranscriptionConfigurationTypeDef(TypedDict):
    EngineTranscribeSettings: NotRequired[EngineTranscribeSettingsTypeDef],  # (1)
    EngineTranscribeMedicalSettings: NotRequired[EngineTranscribeMedicalSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: EngineTranscribeSettingsTypeDef](./type_defs.md#enginetranscribesettingstypedef) 
2. See [:material-code-braces: EngineTranscribeMedicalSettingsTypeDef](./type_defs.md#enginetranscribemedicalsettingstypedef) 
## GetEventsConfigurationResponseTypeDef

```python
# GetEventsConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetEventsConfigurationResponseTypeDef


def get_value() -> GetEventsConfigurationResponseTypeDef:
    return {
        "EventsConfiguration": ...,
    }


# GetEventsConfigurationResponseTypeDef definition

class GetEventsConfigurationResponseTypeDef(TypedDict):
    EventsConfiguration: EventsConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventsConfigurationTypeDef](./type_defs.md#eventsconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutEventsConfigurationResponseTypeDef

```python
# PutEventsConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutEventsConfigurationResponseTypeDef


def get_value() -> PutEventsConfigurationResponseTypeDef:
    return {
        "EventsConfiguration": ...,
    }


# PutEventsConfigurationResponseTypeDef definition

class PutEventsConfigurationResponseTypeDef(TypedDict):
    EventsConfiguration: EventsConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventsConfigurationTypeDef](./type_defs.md#eventsconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGlobalSettingsResponseTypeDef

```python
# GetGlobalSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetGlobalSettingsResponseTypeDef


def get_value() -> GetGlobalSettingsResponseTypeDef:
    return {
        "BusinessCalling": ...,
    }


# GetGlobalSettingsResponseTypeDef definition

class GetGlobalSettingsResponseTypeDef(TypedDict):
    BusinessCalling: BusinessCallingSettingsTypeDef,  # (1)
    VoiceConnector: VoiceConnectorSettingsTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BusinessCallingSettingsTypeDef](./type_defs.md#businesscallingsettingstypedef) 
2. See [:material-code-braces: VoiceConnectorSettingsTypeDef](./type_defs.md#voiceconnectorsettingstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGlobalSettingsRequestTypeDef

```python
# UpdateGlobalSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateGlobalSettingsRequestTypeDef


def get_value() -> UpdateGlobalSettingsRequestTypeDef:
    return {
        "BusinessCalling": ...,
    }


# UpdateGlobalSettingsRequestTypeDef definition

class UpdateGlobalSettingsRequestTypeDef(TypedDict):
    BusinessCalling: NotRequired[BusinessCallingSettingsTypeDef],  # (1)
    VoiceConnector: NotRequired[VoiceConnectorSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: BusinessCallingSettingsTypeDef](./type_defs.md#businesscallingsettingstypedef) 
2. See [:material-code-braces: VoiceConnectorSettingsTypeDef](./type_defs.md#voiceconnectorsettingstypedef) 
## GetMessagingSessionEndpointResponseTypeDef

```python
# GetMessagingSessionEndpointResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetMessagingSessionEndpointResponseTypeDef


def get_value() -> GetMessagingSessionEndpointResponseTypeDef:
    return {
        "Endpoint": ...,
    }


# GetMessagingSessionEndpointResponseTypeDef definition

class GetMessagingSessionEndpointResponseTypeDef(TypedDict):
    Endpoint: MessagingSessionEndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessagingSessionEndpointTypeDef](./type_defs.md#messagingsessionendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSipMediaApplicationLoggingConfigurationResponseTypeDef

```python
# GetSipMediaApplicationLoggingConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetSipMediaApplicationLoggingConfigurationResponseTypeDef


def get_value() -> GetSipMediaApplicationLoggingConfigurationResponseTypeDef:
    return {
        "SipMediaApplicationLoggingConfiguration": ...,
    }


# GetSipMediaApplicationLoggingConfigurationResponseTypeDef definition

class GetSipMediaApplicationLoggingConfigurationResponseTypeDef(TypedDict):
    SipMediaApplicationLoggingConfiguration: SipMediaApplicationLoggingConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SipMediaApplicationLoggingConfigurationTypeDef](./type_defs.md#sipmediaapplicationloggingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutSipMediaApplicationLoggingConfigurationRequestTypeDef

```python
# PutSipMediaApplicationLoggingConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutSipMediaApplicationLoggingConfigurationRequestTypeDef


def get_value() -> PutSipMediaApplicationLoggingConfigurationRequestTypeDef:
    return {
        "SipMediaApplicationId": ...,
    }


# PutSipMediaApplicationLoggingConfigurationRequestTypeDef definition

class PutSipMediaApplicationLoggingConfigurationRequestTypeDef(TypedDict):
    SipMediaApplicationId: str,
    SipMediaApplicationLoggingConfiguration: NotRequired[SipMediaApplicationLoggingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: SipMediaApplicationLoggingConfigurationTypeDef](./type_defs.md#sipmediaapplicationloggingconfigurationtypedef) 
## PutSipMediaApplicationLoggingConfigurationResponseTypeDef

```python
# PutSipMediaApplicationLoggingConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutSipMediaApplicationLoggingConfigurationResponseTypeDef


def get_value() -> PutSipMediaApplicationLoggingConfigurationResponseTypeDef:
    return {
        "SipMediaApplicationLoggingConfiguration": ...,
    }


# PutSipMediaApplicationLoggingConfigurationResponseTypeDef definition

class PutSipMediaApplicationLoggingConfigurationResponseTypeDef(TypedDict):
    SipMediaApplicationLoggingConfiguration: SipMediaApplicationLoggingConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SipMediaApplicationLoggingConfigurationTypeDef](./type_defs.md#sipmediaapplicationloggingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVoiceConnectorLoggingConfigurationResponseTypeDef

```python
# GetVoiceConnectorLoggingConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetVoiceConnectorLoggingConfigurationResponseTypeDef


def get_value() -> GetVoiceConnectorLoggingConfigurationResponseTypeDef:
    return {
        "LoggingConfiguration": ...,
    }


# GetVoiceConnectorLoggingConfigurationResponseTypeDef definition

class GetVoiceConnectorLoggingConfigurationResponseTypeDef(TypedDict):
    LoggingConfiguration: LoggingConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutVoiceConnectorLoggingConfigurationRequestTypeDef

```python
# PutVoiceConnectorLoggingConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutVoiceConnectorLoggingConfigurationRequestTypeDef


def get_value() -> PutVoiceConnectorLoggingConfigurationRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# PutVoiceConnectorLoggingConfigurationRequestTypeDef definition

class PutVoiceConnectorLoggingConfigurationRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    LoggingConfiguration: LoggingConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
## PutVoiceConnectorLoggingConfigurationResponseTypeDef

```python
# PutVoiceConnectorLoggingConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutVoiceConnectorLoggingConfigurationResponseTypeDef


def get_value() -> PutVoiceConnectorLoggingConfigurationResponseTypeDef:
    return {
        "LoggingConfiguration": ...,
    }


# PutVoiceConnectorLoggingConfigurationResponseTypeDef definition

class PutVoiceConnectorLoggingConfigurationResponseTypeDef(TypedDict):
    LoggingConfiguration: LoggingConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVoiceConnectorProxyResponseTypeDef

```python
# GetVoiceConnectorProxyResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetVoiceConnectorProxyResponseTypeDef


def get_value() -> GetVoiceConnectorProxyResponseTypeDef:
    return {
        "Proxy": ...,
    }


# GetVoiceConnectorProxyResponseTypeDef definition

class GetVoiceConnectorProxyResponseTypeDef(TypedDict):
    Proxy: ProxyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProxyTypeDef](./type_defs.md#proxytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutVoiceConnectorProxyResponseTypeDef

```python
# PutVoiceConnectorProxyResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutVoiceConnectorProxyResponseTypeDef


def get_value() -> PutVoiceConnectorProxyResponseTypeDef:
    return {
        "Proxy": ...,
    }


# PutVoiceConnectorProxyResponseTypeDef definition

class PutVoiceConnectorProxyResponseTypeDef(TypedDict):
    Proxy: ProxyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProxyTypeDef](./type_defs.md#proxytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVoiceConnectorTerminationHealthResponseTypeDef

```python
# GetVoiceConnectorTerminationHealthResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetVoiceConnectorTerminationHealthResponseTypeDef


def get_value() -> GetVoiceConnectorTerminationHealthResponseTypeDef:
    return {
        "TerminationHealth": ...,
    }


# GetVoiceConnectorTerminationHealthResponseTypeDef definition

class GetVoiceConnectorTerminationHealthResponseTypeDef(TypedDict):
    TerminationHealth: TerminationHealthTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TerminationHealthTypeDef](./type_defs.md#terminationhealthtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVoiceConnectorTerminationResponseTypeDef

```python
# GetVoiceConnectorTerminationResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetVoiceConnectorTerminationResponseTypeDef


def get_value() -> GetVoiceConnectorTerminationResponseTypeDef:
    return {
        "Termination": ...,
    }


# GetVoiceConnectorTerminationResponseTypeDef definition

class GetVoiceConnectorTerminationResponseTypeDef(TypedDict):
    Termination: TerminationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TerminationOutputTypeDef](./type_defs.md#terminationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutVoiceConnectorTerminationResponseTypeDef

```python
# PutVoiceConnectorTerminationResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutVoiceConnectorTerminationResponseTypeDef


def get_value() -> PutVoiceConnectorTerminationResponseTypeDef:
    return {
        "Termination": ...,
    }


# PutVoiceConnectorTerminationResponseTypeDef definition

class PutVoiceConnectorTerminationResponseTypeDef(TypedDict):
    Termination: TerminationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TerminationOutputTypeDef](./type_defs.md#terminationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InviteUsersResponseTypeDef

```python
# InviteUsersResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import InviteUsersResponseTypeDef


def get_value() -> InviteUsersResponseTypeDef:
    return {
        "Invites": ...,
    }


# InviteUsersResponseTypeDef definition

class InviteUsersResponseTypeDef(TypedDict):
    Invites: List[InviteTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InviteTypeDef](./type_defs.md#invitetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountsRequestPaginateTypeDef

```python
# ListAccountsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListAccountsRequestPaginateTypeDef


def get_value() -> ListAccountsRequestPaginateTypeDef:
    return {
        "Name": ...,
    }


# ListAccountsRequestPaginateTypeDef definition

class ListAccountsRequestPaginateTypeDef(TypedDict):
    Name: NotRequired[str],
    UserEmail: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUsersRequestPaginateTypeDef

```python
# ListUsersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListUsersRequestPaginateTypeDef


def get_value() -> ListUsersRequestPaginateTypeDef:
    return {
        "AccountId": ...,
    }


# ListUsersRequestPaginateTypeDef definition

class ListUsersRequestPaginateTypeDef(TypedDict):
    AccountId: str,
    UserEmail: NotRequired[str],
    UserType: NotRequired[UserTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListChannelMessagesRequestTypeDef

```python
# ListChannelMessagesRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListChannelMessagesRequestTypeDef


def get_value() -> ListChannelMessagesRequestTypeDef:
    return {
        "ChannelArn": ...,
    }


# ListChannelMessagesRequestTypeDef definition

class ListChannelMessagesRequestTypeDef(TypedDict):
    ChannelArn: str,
    SortOrder: NotRequired[SortOrderType],  # (1)
    NotBefore: NotRequired[TimestampTypeDef],
    NotAfter: NotRequired[TimestampTypeDef],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ChimeBearer: NotRequired[str],
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListSupportedPhoneNumberCountriesResponseTypeDef

```python
# ListSupportedPhoneNumberCountriesResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListSupportedPhoneNumberCountriesResponseTypeDef


def get_value() -> ListSupportedPhoneNumberCountriesResponseTypeDef:
    return {
        "PhoneNumberCountries": ...,
    }


# ListSupportedPhoneNumberCountriesResponseTypeDef definition

class ListSupportedPhoneNumberCountriesResponseTypeDef(TypedDict):
    PhoneNumberCountries: List[PhoneNumberCountryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberCountryTypeDef](./type_defs.md#phonenumbercountrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MeetingTypeDef

```python
# MeetingTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import MeetingTypeDef


def get_value() -> MeetingTypeDef:
    return {
        "MeetingId": ...,
    }


# MeetingTypeDef definition

class MeetingTypeDef(TypedDict):
    MeetingId: NotRequired[str],
    ExternalMeetingId: NotRequired[str],
    MediaPlacement: NotRequired[MediaPlacementTypeDef],  # (1)
    MediaRegion: NotRequired[str],
```

1. See [:material-code-braces: MediaPlacementTypeDef](./type_defs.md#mediaplacementtypedef) 
## RoomMembershipTypeDef

```python
# RoomMembershipTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import RoomMembershipTypeDef


def get_value() -> RoomMembershipTypeDef:
    return {
        "RoomId": ...,
    }


# RoomMembershipTypeDef definition

class RoomMembershipTypeDef(TypedDict):
    RoomId: NotRequired[str],
    Member: NotRequired[MemberTypeDef],  # (1)
    Role: NotRequired[RoomMembershipRoleType],  # (2)
    InvitedBy: NotRequired[str],
    UpdatedTimestamp: NotRequired[datetime],
```

1. See [:material-code-braces: MemberTypeDef](./type_defs.md#membertypedef) 
2. See [:material-code-brackets: RoomMembershipRoleType](./literals.md#roommembershiproletype) 
## PhoneNumberOrderTypeDef

```python
# PhoneNumberOrderTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PhoneNumberOrderTypeDef


def get_value() -> PhoneNumberOrderTypeDef:
    return {
        "PhoneNumberOrderId": ...,
    }


# PhoneNumberOrderTypeDef definition

class PhoneNumberOrderTypeDef(TypedDict):
    PhoneNumberOrderId: NotRequired[str],
    ProductType: NotRequired[PhoneNumberProductTypeType],  # (1)
    Status: NotRequired[PhoneNumberOrderStatusType],  # (2)
    OrderedPhoneNumbers: NotRequired[List[OrderedPhoneNumberTypeDef]],  # (3)
    CreatedTimestamp: NotRequired[datetime],
    UpdatedTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: PhoneNumberProductTypeType](./literals.md#phonenumberproducttypetype) 
2. See [:material-code-brackets: PhoneNumberOrderStatusType](./literals.md#phonenumberorderstatustype) 
3. See [:material-code-braces: OrderedPhoneNumberTypeDef](./type_defs.md#orderedphonenumbertypedef) 
## OriginationOutputTypeDef

```python
# OriginationOutputTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import OriginationOutputTypeDef


def get_value() -> OriginationOutputTypeDef:
    return {
        "Routes": ...,
    }


# OriginationOutputTypeDef definition

class OriginationOutputTypeDef(TypedDict):
    Routes: NotRequired[List[OriginationRouteTypeDef]],  # (1)
    Disabled: NotRequired[bool],
```

1. See [:material-code-braces: OriginationRouteTypeDef](./type_defs.md#originationroutetypedef) 
## OriginationTypeDef

```python
# OriginationTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import OriginationTypeDef


def get_value() -> OriginationTypeDef:
    return {
        "Routes": ...,
    }


# OriginationTypeDef definition

class OriginationTypeDef(TypedDict):
    Routes: NotRequired[Sequence[OriginationRouteTypeDef]],  # (1)
    Disabled: NotRequired[bool],
```

1. See [:material-code-braces: OriginationRouteTypeDef](./type_defs.md#originationroutetypedef) 
## ProxySessionTypeDef

```python
# ProxySessionTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ProxySessionTypeDef


def get_value() -> ProxySessionTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# ProxySessionTypeDef definition

class ProxySessionTypeDef(TypedDict):
    VoiceConnectorId: NotRequired[str],
    ProxySessionId: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[ProxySessionStatusType],  # (1)
    ExpiryMinutes: NotRequired[int],
    Capabilities: NotRequired[List[CapabilityType]],  # (2)
    CreatedTimestamp: NotRequired[datetime],
    UpdatedTimestamp: NotRequired[datetime],
    EndedTimestamp: NotRequired[datetime],
    Participants: NotRequired[List[ParticipantTypeDef]],  # (3)
    NumberSelectionBehavior: NotRequired[NumberSelectionBehaviorType],  # (4)
    GeoMatchLevel: NotRequired[GeoMatchLevelType],  # (5)
    GeoMatchParams: NotRequired[GeoMatchParamsTypeDef],  # (6)
```

1. See [:material-code-brackets: ProxySessionStatusType](./literals.md#proxysessionstatustype) 
2. See [:material-code-brackets: CapabilityType](./literals.md#capabilitytype) 
3. See [:material-code-braces: ParticipantTypeDef](./type_defs.md#participanttypedef) 
4. See [:material-code-brackets: NumberSelectionBehaviorType](./literals.md#numberselectionbehaviortype) 
5. See [:material-code-brackets: GeoMatchLevelType](./literals.md#geomatchleveltype) 
6. See [:material-code-braces: GeoMatchParamsTypeDef](./type_defs.md#geomatchparamstypedef) 
## PhoneNumberTypeDef

```python
# PhoneNumberTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PhoneNumberTypeDef


def get_value() -> PhoneNumberTypeDef:
    return {
        "PhoneNumberId": ...,
    }


# PhoneNumberTypeDef definition

class PhoneNumberTypeDef(TypedDict):
    PhoneNumberId: NotRequired[str],
    E164PhoneNumber: NotRequired[str],
    Country: NotRequired[str],
    Type: NotRequired[PhoneNumberTypeType],  # (1)
    ProductType: NotRequired[PhoneNumberProductTypeType],  # (2)
    Status: NotRequired[PhoneNumberStatusType],  # (3)
    Capabilities: NotRequired[PhoneNumberCapabilitiesTypeDef],  # (4)
    Associations: NotRequired[List[PhoneNumberAssociationTypeDef]],  # (5)
    CallingName: NotRequired[str],
    CallingNameStatus: NotRequired[CallingNameStatusType],  # (6)
    CreatedTimestamp: NotRequired[datetime],
    UpdatedTimestamp: NotRequired[datetime],
    DeletionTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
2. See [:material-code-brackets: PhoneNumberProductTypeType](./literals.md#phonenumberproducttypetype) 
3. See [:material-code-brackets: PhoneNumberStatusType](./literals.md#phonenumberstatustype) 
4. See [:material-code-braces: PhoneNumberCapabilitiesTypeDef](./type_defs.md#phonenumbercapabilitiestypedef) 
5. See [:material-code-braces: PhoneNumberAssociationTypeDef](./type_defs.md#phonenumberassociationtypedef) 
6. See [:material-code-brackets: CallingNameStatusType](./literals.md#callingnamestatustype) 
## RetentionSettingsTypeDef

```python
# RetentionSettingsTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import RetentionSettingsTypeDef


def get_value() -> RetentionSettingsTypeDef:
    return {
        "RoomRetentionSettings": ...,
    }


# RetentionSettingsTypeDef definition

class RetentionSettingsTypeDef(TypedDict):
    RoomRetentionSettings: NotRequired[RoomRetentionSettingsTypeDef],  # (1)
    ConversationRetentionSettings: NotRequired[ConversationRetentionSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: RoomRetentionSettingsTypeDef](./type_defs.md#roomretentionsettingstypedef) 
2. See [:material-code-braces: ConversationRetentionSettingsTypeDef](./type_defs.md#conversationretentionsettingstypedef) 
## SourceConfigurationOutputTypeDef

```python
# SourceConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import SourceConfigurationOutputTypeDef


def get_value() -> SourceConfigurationOutputTypeDef:
    return {
        "SelectedVideoStreams": ...,
    }


# SourceConfigurationOutputTypeDef definition

class SourceConfigurationOutputTypeDef(TypedDict):
    SelectedVideoStreams: NotRequired[SelectedVideoStreamsOutputTypeDef],  # (1)
```

1. See [:material-code-braces: SelectedVideoStreamsOutputTypeDef](./type_defs.md#selectedvideostreamsoutputtypedef) 
## SourceConfigurationTypeDef

```python
# SourceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import SourceConfigurationTypeDef


def get_value() -> SourceConfigurationTypeDef:
    return {
        "SelectedVideoStreams": ...,
    }


# SourceConfigurationTypeDef definition

class SourceConfigurationTypeDef(TypedDict):
    SelectedVideoStreams: NotRequired[SelectedVideoStreamsTypeDef],  # (1)
```

1. See [:material-code-braces: SelectedVideoStreamsTypeDef](./type_defs.md#selectedvideostreamstypedef) 
## StreamingConfigurationOutputTypeDef

```python
# StreamingConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import StreamingConfigurationOutputTypeDef


def get_value() -> StreamingConfigurationOutputTypeDef:
    return {
        "DataRetentionInHours": ...,
    }


# StreamingConfigurationOutputTypeDef definition

class StreamingConfigurationOutputTypeDef(TypedDict):
    DataRetentionInHours: int,
    Disabled: NotRequired[bool],
    StreamingNotificationTargets: NotRequired[List[StreamingNotificationTargetTypeDef]],  # (1)
```

1. See [:material-code-braces: StreamingNotificationTargetTypeDef](./type_defs.md#streamingnotificationtargettypedef) 
## StreamingConfigurationTypeDef

```python
# StreamingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import StreamingConfigurationTypeDef


def get_value() -> StreamingConfigurationTypeDef:
    return {
        "DataRetentionInHours": ...,
    }


# StreamingConfigurationTypeDef definition

class StreamingConfigurationTypeDef(TypedDict):
    DataRetentionInHours: int,
    Disabled: NotRequired[bool],
    StreamingNotificationTargets: NotRequired[Sequence[StreamingNotificationTargetTypeDef]],  # (1)
```

1. See [:material-code-braces: StreamingNotificationTargetTypeDef](./type_defs.md#streamingnotificationtargettypedef) 
## UserSettingsTypeDef

```python
# UserSettingsTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UserSettingsTypeDef


def get_value() -> UserSettingsTypeDef:
    return {
        "Telephony": ...,
    }


# UserSettingsTypeDef definition

class UserSettingsTypeDef(TypedDict):
    Telephony: TelephonySettingsTypeDef,  # (1)
```

1. See [:material-code-braces: TelephonySettingsTypeDef](./type_defs.md#telephonysettingstypedef) 
## CreateAccountResponseTypeDef

```python
# CreateAccountResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateAccountResponseTypeDef


def get_value() -> CreateAccountResponseTypeDef:
    return {
        "Account": ...,
    }


# CreateAccountResponseTypeDef definition

class CreateAccountResponseTypeDef(TypedDict):
    Account: AccountTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccountResponseTypeDef

```python
# GetAccountResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetAccountResponseTypeDef


def get_value() -> GetAccountResponseTypeDef:
    return {
        "Account": ...,
    }


# GetAccountResponseTypeDef definition

class GetAccountResponseTypeDef(TypedDict):
    Account: AccountTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountsResponseTypeDef

```python
# ListAccountsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListAccountsResponseTypeDef


def get_value() -> ListAccountsResponseTypeDef:
    return {
        "Accounts": ...,
    }


# ListAccountsResponseTypeDef definition

class ListAccountsResponseTypeDef(TypedDict):
    Accounts: List[AccountTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAccountResponseTypeDef

```python
# UpdateAccountResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateAccountResponseTypeDef


def get_value() -> UpdateAccountResponseTypeDef:
    return {
        "Account": ...,
    }


# UpdateAccountResponseTypeDef definition

class UpdateAccountResponseTypeDef(TypedDict):
    Account: AccountTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateUserRequestTypeDef

```python
# BatchUpdateUserRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import BatchUpdateUserRequestTypeDef


def get_value() -> BatchUpdateUserRequestTypeDef:
    return {
        "AccountId": ...,
    }


# BatchUpdateUserRequestTypeDef definition

class BatchUpdateUserRequestTypeDef(TypedDict):
    AccountId: str,
    UpdateUserRequestItems: Sequence[UpdateUserRequestItemTypeDef],  # (1)
```

1. See [:material-code-braces: UpdateUserRequestItemTypeDef](./type_defs.md#updateuserrequestitemtypedef) 
## CreateUserResponseTypeDef

```python
# CreateUserResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateUserResponseTypeDef


def get_value() -> CreateUserResponseTypeDef:
    return {
        "User": ...,
    }


# CreateUserResponseTypeDef definition

class CreateUserResponseTypeDef(TypedDict):
    User: UserTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUserResponseTypeDef

```python
# GetUserResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetUserResponseTypeDef


def get_value() -> GetUserResponseTypeDef:
    return {
        "User": ...,
    }


# GetUserResponseTypeDef definition

class GetUserResponseTypeDef(TypedDict):
    User: UserTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUsersResponseTypeDef

```python
# ListUsersResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListUsersResponseTypeDef


def get_value() -> ListUsersResponseTypeDef:
    return {
        "Users": ...,
    }


# ListUsersResponseTypeDef definition

class ListUsersResponseTypeDef(TypedDict):
    Users: List[UserTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResetPersonalPINResponseTypeDef

```python
# ResetPersonalPINResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ResetPersonalPINResponseTypeDef


def get_value() -> ResetPersonalPINResponseTypeDef:
    return {
        "User": ...,
    }


# ResetPersonalPINResponseTypeDef definition

class ResetPersonalPINResponseTypeDef(TypedDict):
    User: UserTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserResponseTypeDef

```python
# UpdateUserResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateUserResponseTypeDef


def get_value() -> UpdateUserResponseTypeDef:
    return {
        "User": ...,
    }


# UpdateUserResponseTypeDef definition

class UpdateUserResponseTypeDef(TypedDict):
    User: UserTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAppInstanceAdminsResponseTypeDef

```python
# ListAppInstanceAdminsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListAppInstanceAdminsResponseTypeDef


def get_value() -> ListAppInstanceAdminsResponseTypeDef:
    return {
        "AppInstanceArn": ...,
    }


# ListAppInstanceAdminsResponseTypeDef definition

class ListAppInstanceAdminsResponseTypeDef(TypedDict):
    AppInstanceArn: str,
    AppInstanceAdmins: List[AppInstanceAdminSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AppInstanceAdminSummaryTypeDef](./type_defs.md#appinstanceadminsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAppInstanceAdminResponseTypeDef

```python
# DescribeAppInstanceAdminResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DescribeAppInstanceAdminResponseTypeDef


def get_value() -> DescribeAppInstanceAdminResponseTypeDef:
    return {
        "AppInstanceAdmin": ...,
    }


# DescribeAppInstanceAdminResponseTypeDef definition

class DescribeAppInstanceAdminResponseTypeDef(TypedDict):
    AppInstanceAdmin: AppInstanceAdminTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppInstanceAdminTypeDef](./type_defs.md#appinstanceadmintypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchCreateChannelMembershipResponseTypeDef

```python
# BatchCreateChannelMembershipResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import BatchCreateChannelMembershipResponseTypeDef


def get_value() -> BatchCreateChannelMembershipResponseTypeDef:
    return {
        "BatchChannelMemberships": ...,
    }


# BatchCreateChannelMembershipResponseTypeDef definition

class BatchCreateChannelMembershipResponseTypeDef(TypedDict):
    BatchChannelMemberships: BatchChannelMembershipsTypeDef,  # (1)
    Errors: List[BatchCreateChannelMembershipErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchChannelMembershipsTypeDef](./type_defs.md#batchchannelmembershipstypedef) 
2. See [:material-code-braces: BatchCreateChannelMembershipErrorTypeDef](./type_defs.md#batchcreatechannelmembershiperrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChannelBansResponseTypeDef

```python
# ListChannelBansResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListChannelBansResponseTypeDef


def get_value() -> ListChannelBansResponseTypeDef:
    return {
        "ChannelArn": ...,
    }


# ListChannelBansResponseTypeDef definition

class ListChannelBansResponseTypeDef(TypedDict):
    ChannelArn: str,
    ChannelBans: List[ChannelBanSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ChannelBanSummaryTypeDef](./type_defs.md#channelbansummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeChannelBanResponseTypeDef

```python
# DescribeChannelBanResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DescribeChannelBanResponseTypeDef


def get_value() -> DescribeChannelBanResponseTypeDef:
    return {
        "ChannelBan": ...,
    }


# DescribeChannelBanResponseTypeDef definition

class DescribeChannelBanResponseTypeDef(TypedDict):
    ChannelBan: ChannelBanTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelBanTypeDef](./type_defs.md#channelbantypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChannelMembershipsResponseTypeDef

```python
# ListChannelMembershipsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListChannelMembershipsResponseTypeDef


def get_value() -> ListChannelMembershipsResponseTypeDef:
    return {
        "ChannelArn": ...,
    }


# ListChannelMembershipsResponseTypeDef definition

class ListChannelMembershipsResponseTypeDef(TypedDict):
    ChannelArn: str,
    ChannelMemberships: List[ChannelMembershipSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ChannelMembershipSummaryTypeDef](./type_defs.md#channelmembershipsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeChannelMembershipResponseTypeDef

```python
# DescribeChannelMembershipResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DescribeChannelMembershipResponseTypeDef


def get_value() -> DescribeChannelMembershipResponseTypeDef:
    return {
        "ChannelMembership": ...,
    }


# DescribeChannelMembershipResponseTypeDef definition

class DescribeChannelMembershipResponseTypeDef(TypedDict):
    ChannelMembership: ChannelMembershipTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelMembershipTypeDef](./type_defs.md#channelmembershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChannelMessagesResponseTypeDef

```python
# ListChannelMessagesResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListChannelMessagesResponseTypeDef


def get_value() -> ListChannelMessagesResponseTypeDef:
    return {
        "ChannelArn": ...,
    }


# ListChannelMessagesResponseTypeDef definition

class ListChannelMessagesResponseTypeDef(TypedDict):
    ChannelArn: str,
    ChannelMessages: List[ChannelMessageSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ChannelMessageSummaryTypeDef](./type_defs.md#channelmessagesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetChannelMessageResponseTypeDef

```python
# GetChannelMessageResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetChannelMessageResponseTypeDef


def get_value() -> GetChannelMessageResponseTypeDef:
    return {
        "ChannelMessage": ...,
    }


# GetChannelMessageResponseTypeDef definition

class GetChannelMessageResponseTypeDef(TypedDict):
    ChannelMessage: ChannelMessageTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelMessageTypeDef](./type_defs.md#channelmessagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChannelModeratorsResponseTypeDef

```python
# ListChannelModeratorsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListChannelModeratorsResponseTypeDef


def get_value() -> ListChannelModeratorsResponseTypeDef:
    return {
        "ChannelArn": ...,
    }


# ListChannelModeratorsResponseTypeDef definition

class ListChannelModeratorsResponseTypeDef(TypedDict):
    ChannelArn: str,
    ChannelModerators: List[ChannelModeratorSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ChannelModeratorSummaryTypeDef](./type_defs.md#channelmoderatorsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeChannelModeratorResponseTypeDef

```python
# DescribeChannelModeratorResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DescribeChannelModeratorResponseTypeDef


def get_value() -> DescribeChannelModeratorResponseTypeDef:
    return {
        "ChannelModerator": ...,
    }


# DescribeChannelModeratorResponseTypeDef definition

class DescribeChannelModeratorResponseTypeDef(TypedDict):
    ChannelModerator: ChannelModeratorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelModeratorTypeDef](./type_defs.md#channelmoderatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeChannelResponseTypeDef

```python
# DescribeChannelResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DescribeChannelResponseTypeDef


def get_value() -> DescribeChannelResponseTypeDef:
    return {
        "Channel": ...,
    }


# DescribeChannelResponseTypeDef definition

class DescribeChannelResponseTypeDef(TypedDict):
    Channel: ChannelTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAppInstanceRetentionSettingsResponseTypeDef

```python
# GetAppInstanceRetentionSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetAppInstanceRetentionSettingsResponseTypeDef


def get_value() -> GetAppInstanceRetentionSettingsResponseTypeDef:
    return {
        "AppInstanceRetentionSettings": ...,
    }


# GetAppInstanceRetentionSettingsResponseTypeDef definition

class GetAppInstanceRetentionSettingsResponseTypeDef(TypedDict):
    AppInstanceRetentionSettings: AppInstanceRetentionSettingsTypeDef,  # (1)
    InitiateDeletionTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppInstanceRetentionSettingsTypeDef](./type_defs.md#appinstanceretentionsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAppInstanceRetentionSettingsRequestTypeDef

```python
# PutAppInstanceRetentionSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutAppInstanceRetentionSettingsRequestTypeDef


def get_value() -> PutAppInstanceRetentionSettingsRequestTypeDef:
    return {
        "AppInstanceArn": ...,
    }


# PutAppInstanceRetentionSettingsRequestTypeDef definition

class PutAppInstanceRetentionSettingsRequestTypeDef(TypedDict):
    AppInstanceArn: str,
    AppInstanceRetentionSettings: AppInstanceRetentionSettingsTypeDef,  # (1)
```

1. See [:material-code-braces: AppInstanceRetentionSettingsTypeDef](./type_defs.md#appinstanceretentionsettingstypedef) 
## PutAppInstanceRetentionSettingsResponseTypeDef

```python
# PutAppInstanceRetentionSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutAppInstanceRetentionSettingsResponseTypeDef


def get_value() -> PutAppInstanceRetentionSettingsResponseTypeDef:
    return {
        "AppInstanceRetentionSettings": ...,
    }


# PutAppInstanceRetentionSettingsResponseTypeDef definition

class PutAppInstanceRetentionSettingsResponseTypeDef(TypedDict):
    AppInstanceRetentionSettings: AppInstanceRetentionSettingsTypeDef,  # (1)
    InitiateDeletionTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppInstanceRetentionSettingsTypeDef](./type_defs.md#appinstanceretentionsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeChannelMembershipForAppInstanceUserResponseTypeDef

```python
# DescribeChannelMembershipForAppInstanceUserResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DescribeChannelMembershipForAppInstanceUserResponseTypeDef


def get_value() -> DescribeChannelMembershipForAppInstanceUserResponseTypeDef:
    return {
        "ChannelMembership": ...,
    }


# DescribeChannelMembershipForAppInstanceUserResponseTypeDef definition

class DescribeChannelMembershipForAppInstanceUserResponseTypeDef(TypedDict):
    ChannelMembership: ChannelMembershipForAppInstanceUserSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelMembershipForAppInstanceUserSummaryTypeDef](./type_defs.md#channelmembershipforappinstanceusersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChannelMembershipsForAppInstanceUserResponseTypeDef

```python
# ListChannelMembershipsForAppInstanceUserResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListChannelMembershipsForAppInstanceUserResponseTypeDef


def get_value() -> ListChannelMembershipsForAppInstanceUserResponseTypeDef:
    return {
        "ChannelMemberships": ...,
    }


# ListChannelMembershipsForAppInstanceUserResponseTypeDef definition

class ListChannelMembershipsForAppInstanceUserResponseTypeDef(TypedDict):
    ChannelMemberships: List[ChannelMembershipForAppInstanceUserSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ChannelMembershipForAppInstanceUserSummaryTypeDef](./type_defs.md#channelmembershipforappinstanceusersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeChannelModeratedByAppInstanceUserResponseTypeDef

```python
# DescribeChannelModeratedByAppInstanceUserResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import DescribeChannelModeratedByAppInstanceUserResponseTypeDef


def get_value() -> DescribeChannelModeratedByAppInstanceUserResponseTypeDef:
    return {
        "Channel": ...,
    }


# DescribeChannelModeratedByAppInstanceUserResponseTypeDef definition

class DescribeChannelModeratedByAppInstanceUserResponseTypeDef(TypedDict):
    Channel: ChannelModeratedByAppInstanceUserSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelModeratedByAppInstanceUserSummaryTypeDef](./type_defs.md#channelmoderatedbyappinstanceusersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChannelsModeratedByAppInstanceUserResponseTypeDef

```python
# ListChannelsModeratedByAppInstanceUserResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListChannelsModeratedByAppInstanceUserResponseTypeDef


def get_value() -> ListChannelsModeratedByAppInstanceUserResponseTypeDef:
    return {
        "Channels": ...,
    }


# ListChannelsModeratedByAppInstanceUserResponseTypeDef definition

class ListChannelsModeratedByAppInstanceUserResponseTypeDef(TypedDict):
    Channels: List[ChannelModeratedByAppInstanceUserSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ChannelModeratedByAppInstanceUserSummaryTypeDef](./type_defs.md#channelmoderatedbyappinstanceusersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchCreateAttendeeRequestTypeDef

```python
# BatchCreateAttendeeRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import BatchCreateAttendeeRequestTypeDef


def get_value() -> BatchCreateAttendeeRequestTypeDef:
    return {
        "MeetingId": ...,
    }


# BatchCreateAttendeeRequestTypeDef definition

class BatchCreateAttendeeRequestTypeDef(TypedDict):
    MeetingId: str,
    Attendees: Sequence[CreateAttendeeRequestItemTypeDef],  # (1)
```

1. See [:material-code-braces: CreateAttendeeRequestItemTypeDef](./type_defs.md#createattendeerequestitemtypedef) 
## CreateMeetingWithAttendeesRequestTypeDef

```python
# CreateMeetingWithAttendeesRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateMeetingWithAttendeesRequestTypeDef


def get_value() -> CreateMeetingWithAttendeesRequestTypeDef:
    return {
        "ClientRequestToken": ...,
    }


# CreateMeetingWithAttendeesRequestTypeDef definition

class CreateMeetingWithAttendeesRequestTypeDef(TypedDict):
    ClientRequestToken: str,
    ExternalMeetingId: NotRequired[str],
    MeetingHostId: NotRequired[str],
    MediaRegion: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    NotificationsConfiguration: NotRequired[MeetingNotificationConfigurationTypeDef],  # (2)
    Attendees: NotRequired[Sequence[CreateAttendeeRequestItemTypeDef]],  # (3)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: MeetingNotificationConfigurationTypeDef](./type_defs.md#meetingnotificationconfigurationtypedef) 
3. See [:material-code-braces: CreateAttendeeRequestItemTypeDef](./type_defs.md#createattendeerequestitemtypedef) 
## CreateSipMediaApplicationResponseTypeDef

```python
# CreateSipMediaApplicationResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateSipMediaApplicationResponseTypeDef


def get_value() -> CreateSipMediaApplicationResponseTypeDef:
    return {
        "SipMediaApplication": ...,
    }


# CreateSipMediaApplicationResponseTypeDef definition

class CreateSipMediaApplicationResponseTypeDef(TypedDict):
    SipMediaApplication: SipMediaApplicationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SipMediaApplicationTypeDef](./type_defs.md#sipmediaapplicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSipMediaApplicationResponseTypeDef

```python
# GetSipMediaApplicationResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetSipMediaApplicationResponseTypeDef


def get_value() -> GetSipMediaApplicationResponseTypeDef:
    return {
        "SipMediaApplication": ...,
    }


# GetSipMediaApplicationResponseTypeDef definition

class GetSipMediaApplicationResponseTypeDef(TypedDict):
    SipMediaApplication: SipMediaApplicationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SipMediaApplicationTypeDef](./type_defs.md#sipmediaapplicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSipMediaApplicationsResponseTypeDef

```python
# ListSipMediaApplicationsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListSipMediaApplicationsResponseTypeDef


def get_value() -> ListSipMediaApplicationsResponseTypeDef:
    return {
        "SipMediaApplications": ...,
    }


# ListSipMediaApplicationsResponseTypeDef definition

class ListSipMediaApplicationsResponseTypeDef(TypedDict):
    SipMediaApplications: List[SipMediaApplicationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SipMediaApplicationTypeDef](./type_defs.md#sipmediaapplicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSipMediaApplicationResponseTypeDef

```python
# UpdateSipMediaApplicationResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateSipMediaApplicationResponseTypeDef


def get_value() -> UpdateSipMediaApplicationResponseTypeDef:
    return {
        "SipMediaApplication": ...,
    }


# UpdateSipMediaApplicationResponseTypeDef definition

class UpdateSipMediaApplicationResponseTypeDef(TypedDict):
    SipMediaApplication: SipMediaApplicationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SipMediaApplicationTypeDef](./type_defs.md#sipmediaapplicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSipRuleResponseTypeDef

```python
# CreateSipRuleResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateSipRuleResponseTypeDef


def get_value() -> CreateSipRuleResponseTypeDef:
    return {
        "SipRule": ...,
    }


# CreateSipRuleResponseTypeDef definition

class CreateSipRuleResponseTypeDef(TypedDict):
    SipRule: SipRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SipRuleTypeDef](./type_defs.md#sipruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSipRuleResponseTypeDef

```python
# GetSipRuleResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetSipRuleResponseTypeDef


def get_value() -> GetSipRuleResponseTypeDef:
    return {
        "SipRule": ...,
    }


# GetSipRuleResponseTypeDef definition

class GetSipRuleResponseTypeDef(TypedDict):
    SipRule: SipRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SipRuleTypeDef](./type_defs.md#sipruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSipRulesResponseTypeDef

```python
# ListSipRulesResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListSipRulesResponseTypeDef


def get_value() -> ListSipRulesResponseTypeDef:
    return {
        "SipRules": ...,
    }


# ListSipRulesResponseTypeDef definition

class ListSipRulesResponseTypeDef(TypedDict):
    SipRules: List[SipRuleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SipRuleTypeDef](./type_defs.md#sipruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSipRuleResponseTypeDef

```python
# UpdateSipRuleResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateSipRuleResponseTypeDef


def get_value() -> UpdateSipRuleResponseTypeDef:
    return {
        "SipRule": ...,
    }


# UpdateSipRuleResponseTypeDef definition

class UpdateSipRuleResponseTypeDef(TypedDict):
    SipRule: SipRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SipRuleTypeDef](./type_defs.md#sipruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVoiceConnectorGroupResponseTypeDef

```python
# CreateVoiceConnectorGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateVoiceConnectorGroupResponseTypeDef


def get_value() -> CreateVoiceConnectorGroupResponseTypeDef:
    return {
        "VoiceConnectorGroup": ...,
    }


# CreateVoiceConnectorGroupResponseTypeDef definition

class CreateVoiceConnectorGroupResponseTypeDef(TypedDict):
    VoiceConnectorGroup: VoiceConnectorGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VoiceConnectorGroupTypeDef](./type_defs.md#voiceconnectorgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVoiceConnectorGroupResponseTypeDef

```python
# GetVoiceConnectorGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetVoiceConnectorGroupResponseTypeDef


def get_value() -> GetVoiceConnectorGroupResponseTypeDef:
    return {
        "VoiceConnectorGroup": ...,
    }


# GetVoiceConnectorGroupResponseTypeDef definition

class GetVoiceConnectorGroupResponseTypeDef(TypedDict):
    VoiceConnectorGroup: VoiceConnectorGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VoiceConnectorGroupTypeDef](./type_defs.md#voiceconnectorgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVoiceConnectorGroupsResponseTypeDef

```python
# ListVoiceConnectorGroupsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListVoiceConnectorGroupsResponseTypeDef


def get_value() -> ListVoiceConnectorGroupsResponseTypeDef:
    return {
        "VoiceConnectorGroups": ...,
    }


# ListVoiceConnectorGroupsResponseTypeDef definition

class ListVoiceConnectorGroupsResponseTypeDef(TypedDict):
    VoiceConnectorGroups: List[VoiceConnectorGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: VoiceConnectorGroupTypeDef](./type_defs.md#voiceconnectorgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateVoiceConnectorGroupResponseTypeDef

```python
# UpdateVoiceConnectorGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateVoiceConnectorGroupResponseTypeDef


def get_value() -> UpdateVoiceConnectorGroupResponseTypeDef:
    return {
        "VoiceConnectorGroup": ...,
    }


# UpdateVoiceConnectorGroupResponseTypeDef definition

class UpdateVoiceConnectorGroupResponseTypeDef(TypedDict):
    VoiceConnectorGroup: VoiceConnectorGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VoiceConnectorGroupTypeDef](./type_defs.md#voiceconnectorgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef

```python
# GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef


def get_value() -> GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef:
    return {
        "EmergencyCallingConfiguration": ...,
    }


# GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef definition

class GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef(TypedDict):
    EmergencyCallingConfiguration: EmergencyCallingConfigurationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EmergencyCallingConfigurationOutputTypeDef](./type_defs.md#emergencycallingconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef

```python
# PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef


def get_value() -> PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef:
    return {
        "EmergencyCallingConfiguration": ...,
    }


# PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef definition

class PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef(TypedDict):
    EmergencyCallingConfiguration: EmergencyCallingConfigurationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EmergencyCallingConfigurationOutputTypeDef](./type_defs.md#emergencycallingconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMeetingTranscriptionRequestTypeDef

```python
# StartMeetingTranscriptionRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import StartMeetingTranscriptionRequestTypeDef


def get_value() -> StartMeetingTranscriptionRequestTypeDef:
    return {
        "MeetingId": ...,
    }


# StartMeetingTranscriptionRequestTypeDef definition

class StartMeetingTranscriptionRequestTypeDef(TypedDict):
    MeetingId: str,
    TranscriptionConfiguration: TranscriptionConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: TranscriptionConfigurationTypeDef](./type_defs.md#transcriptionconfigurationtypedef) 
## CreateMeetingResponseTypeDef

```python
# CreateMeetingResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateMeetingResponseTypeDef


def get_value() -> CreateMeetingResponseTypeDef:
    return {
        "Meeting": ...,
    }


# CreateMeetingResponseTypeDef definition

class CreateMeetingResponseTypeDef(TypedDict):
    Meeting: MeetingTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MeetingTypeDef](./type_defs.md#meetingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMeetingWithAttendeesResponseTypeDef

```python
# CreateMeetingWithAttendeesResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateMeetingWithAttendeesResponseTypeDef


def get_value() -> CreateMeetingWithAttendeesResponseTypeDef:
    return {
        "Meeting": ...,
    }


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
# GetMeetingResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetMeetingResponseTypeDef


def get_value() -> GetMeetingResponseTypeDef:
    return {
        "Meeting": ...,
    }


# GetMeetingResponseTypeDef definition

class GetMeetingResponseTypeDef(TypedDict):
    Meeting: MeetingTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MeetingTypeDef](./type_defs.md#meetingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMeetingsResponseTypeDef

```python
# ListMeetingsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListMeetingsResponseTypeDef


def get_value() -> ListMeetingsResponseTypeDef:
    return {
        "Meetings": ...,
    }


# ListMeetingsResponseTypeDef definition

class ListMeetingsResponseTypeDef(TypedDict):
    Meetings: List[MeetingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MeetingTypeDef](./type_defs.md#meetingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRoomMembershipResponseTypeDef

```python
# CreateRoomMembershipResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateRoomMembershipResponseTypeDef


def get_value() -> CreateRoomMembershipResponseTypeDef:
    return {
        "RoomMembership": ...,
    }


# CreateRoomMembershipResponseTypeDef definition

class CreateRoomMembershipResponseTypeDef(TypedDict):
    RoomMembership: RoomMembershipTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoomMembershipTypeDef](./type_defs.md#roommembershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRoomMembershipsResponseTypeDef

```python
# ListRoomMembershipsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListRoomMembershipsResponseTypeDef


def get_value() -> ListRoomMembershipsResponseTypeDef:
    return {
        "RoomMemberships": ...,
    }


# ListRoomMembershipsResponseTypeDef definition

class ListRoomMembershipsResponseTypeDef(TypedDict):
    RoomMemberships: List[RoomMembershipTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RoomMembershipTypeDef](./type_defs.md#roommembershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRoomMembershipResponseTypeDef

```python
# UpdateRoomMembershipResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateRoomMembershipResponseTypeDef


def get_value() -> UpdateRoomMembershipResponseTypeDef:
    return {
        "RoomMembership": ...,
    }


# UpdateRoomMembershipResponseTypeDef definition

class UpdateRoomMembershipResponseTypeDef(TypedDict):
    RoomMembership: RoomMembershipTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoomMembershipTypeDef](./type_defs.md#roommembershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePhoneNumberOrderResponseTypeDef

```python
# CreatePhoneNumberOrderResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreatePhoneNumberOrderResponseTypeDef


def get_value() -> CreatePhoneNumberOrderResponseTypeDef:
    return {
        "PhoneNumberOrder": ...,
    }


# CreatePhoneNumberOrderResponseTypeDef definition

class CreatePhoneNumberOrderResponseTypeDef(TypedDict):
    PhoneNumberOrder: PhoneNumberOrderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberOrderTypeDef](./type_defs.md#phonenumberordertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPhoneNumberOrderResponseTypeDef

```python
# GetPhoneNumberOrderResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetPhoneNumberOrderResponseTypeDef


def get_value() -> GetPhoneNumberOrderResponseTypeDef:
    return {
        "PhoneNumberOrder": ...,
    }


# GetPhoneNumberOrderResponseTypeDef definition

class GetPhoneNumberOrderResponseTypeDef(TypedDict):
    PhoneNumberOrder: PhoneNumberOrderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberOrderTypeDef](./type_defs.md#phonenumberordertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPhoneNumberOrdersResponseTypeDef

```python
# ListPhoneNumberOrdersResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListPhoneNumberOrdersResponseTypeDef


def get_value() -> ListPhoneNumberOrdersResponseTypeDef:
    return {
        "PhoneNumberOrders": ...,
    }


# ListPhoneNumberOrdersResponseTypeDef definition

class ListPhoneNumberOrdersResponseTypeDef(TypedDict):
    PhoneNumberOrders: List[PhoneNumberOrderTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PhoneNumberOrderTypeDef](./type_defs.md#phonenumberordertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVoiceConnectorOriginationResponseTypeDef

```python
# GetVoiceConnectorOriginationResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetVoiceConnectorOriginationResponseTypeDef


def get_value() -> GetVoiceConnectorOriginationResponseTypeDef:
    return {
        "Origination": ...,
    }


# GetVoiceConnectorOriginationResponseTypeDef definition

class GetVoiceConnectorOriginationResponseTypeDef(TypedDict):
    Origination: OriginationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OriginationOutputTypeDef](./type_defs.md#originationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutVoiceConnectorOriginationResponseTypeDef

```python
# PutVoiceConnectorOriginationResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutVoiceConnectorOriginationResponseTypeDef


def get_value() -> PutVoiceConnectorOriginationResponseTypeDef:
    return {
        "Origination": ...,
    }


# PutVoiceConnectorOriginationResponseTypeDef definition

class PutVoiceConnectorOriginationResponseTypeDef(TypedDict):
    Origination: OriginationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OriginationOutputTypeDef](./type_defs.md#originationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProxySessionResponseTypeDef

```python
# CreateProxySessionResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateProxySessionResponseTypeDef


def get_value() -> CreateProxySessionResponseTypeDef:
    return {
        "ProxySession": ...,
    }


# CreateProxySessionResponseTypeDef definition

class CreateProxySessionResponseTypeDef(TypedDict):
    ProxySession: ProxySessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProxySessionTypeDef](./type_defs.md#proxysessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProxySessionResponseTypeDef

```python
# GetProxySessionResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetProxySessionResponseTypeDef


def get_value() -> GetProxySessionResponseTypeDef:
    return {
        "ProxySession": ...,
    }


# GetProxySessionResponseTypeDef definition

class GetProxySessionResponseTypeDef(TypedDict):
    ProxySession: ProxySessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProxySessionTypeDef](./type_defs.md#proxysessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProxySessionsResponseTypeDef

```python
# ListProxySessionsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListProxySessionsResponseTypeDef


def get_value() -> ListProxySessionsResponseTypeDef:
    return {
        "ProxySessions": ...,
    }


# ListProxySessionsResponseTypeDef definition

class ListProxySessionsResponseTypeDef(TypedDict):
    ProxySessions: List[ProxySessionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProxySessionTypeDef](./type_defs.md#proxysessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProxySessionResponseTypeDef

```python
# UpdateProxySessionResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateProxySessionResponseTypeDef


def get_value() -> UpdateProxySessionResponseTypeDef:
    return {
        "ProxySession": ...,
    }


# UpdateProxySessionResponseTypeDef definition

class UpdateProxySessionResponseTypeDef(TypedDict):
    ProxySession: ProxySessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProxySessionTypeDef](./type_defs.md#proxysessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPhoneNumberResponseTypeDef

```python
# GetPhoneNumberResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetPhoneNumberResponseTypeDef


def get_value() -> GetPhoneNumberResponseTypeDef:
    return {
        "PhoneNumber": ...,
    }


# GetPhoneNumberResponseTypeDef definition

class GetPhoneNumberResponseTypeDef(TypedDict):
    PhoneNumber: PhoneNumberTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberTypeDef](./type_defs.md#phonenumbertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPhoneNumbersResponseTypeDef

```python
# ListPhoneNumbersResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListPhoneNumbersResponseTypeDef


def get_value() -> ListPhoneNumbersResponseTypeDef:
    return {
        "PhoneNumbers": ...,
    }


# ListPhoneNumbersResponseTypeDef definition

class ListPhoneNumbersResponseTypeDef(TypedDict):
    PhoneNumbers: List[PhoneNumberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PhoneNumberTypeDef](./type_defs.md#phonenumbertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestorePhoneNumberResponseTypeDef

```python
# RestorePhoneNumberResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import RestorePhoneNumberResponseTypeDef


def get_value() -> RestorePhoneNumberResponseTypeDef:
    return {
        "PhoneNumber": ...,
    }


# RestorePhoneNumberResponseTypeDef definition

class RestorePhoneNumberResponseTypeDef(TypedDict):
    PhoneNumber: PhoneNumberTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberTypeDef](./type_defs.md#phonenumbertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePhoneNumberResponseTypeDef

```python
# UpdatePhoneNumberResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdatePhoneNumberResponseTypeDef


def get_value() -> UpdatePhoneNumberResponseTypeDef:
    return {
        "PhoneNumber": ...,
    }


# UpdatePhoneNumberResponseTypeDef definition

class UpdatePhoneNumberResponseTypeDef(TypedDict):
    PhoneNumber: PhoneNumberTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberTypeDef](./type_defs.md#phonenumbertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRetentionSettingsResponseTypeDef

```python
# GetRetentionSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetRetentionSettingsResponseTypeDef


def get_value() -> GetRetentionSettingsResponseTypeDef:
    return {
        "RetentionSettings": ...,
    }


# GetRetentionSettingsResponseTypeDef definition

class GetRetentionSettingsResponseTypeDef(TypedDict):
    RetentionSettings: RetentionSettingsTypeDef,  # (1)
    InitiateDeletionTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RetentionSettingsTypeDef](./type_defs.md#retentionsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRetentionSettingsRequestTypeDef

```python
# PutRetentionSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutRetentionSettingsRequestTypeDef


def get_value() -> PutRetentionSettingsRequestTypeDef:
    return {
        "AccountId": ...,
    }


# PutRetentionSettingsRequestTypeDef definition

class PutRetentionSettingsRequestTypeDef(TypedDict):
    AccountId: str,
    RetentionSettings: RetentionSettingsTypeDef,  # (1)
```

1. See [:material-code-braces: RetentionSettingsTypeDef](./type_defs.md#retentionsettingstypedef) 
## PutRetentionSettingsResponseTypeDef

```python
# PutRetentionSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutRetentionSettingsResponseTypeDef


def get_value() -> PutRetentionSettingsResponseTypeDef:
    return {
        "RetentionSettings": ...,
    }


# PutRetentionSettingsResponseTypeDef definition

class PutRetentionSettingsResponseTypeDef(TypedDict):
    RetentionSettings: RetentionSettingsTypeDef,  # (1)
    InitiateDeletionTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RetentionSettingsTypeDef](./type_defs.md#retentionsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ChimeSdkMeetingConfigurationOutputTypeDef

```python
# ChimeSdkMeetingConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ChimeSdkMeetingConfigurationOutputTypeDef


def get_value() -> ChimeSdkMeetingConfigurationOutputTypeDef:
    return {
        "SourceConfiguration": ...,
    }


# ChimeSdkMeetingConfigurationOutputTypeDef definition

class ChimeSdkMeetingConfigurationOutputTypeDef(TypedDict):
    SourceConfiguration: NotRequired[SourceConfigurationOutputTypeDef],  # (1)
    ArtifactsConfiguration: NotRequired[ArtifactsConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: SourceConfigurationOutputTypeDef](./type_defs.md#sourceconfigurationoutputtypedef) 
2. See [:material-code-braces: ArtifactsConfigurationTypeDef](./type_defs.md#artifactsconfigurationtypedef) 
## ChimeSdkMeetingConfigurationTypeDef

```python
# ChimeSdkMeetingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ChimeSdkMeetingConfigurationTypeDef


def get_value() -> ChimeSdkMeetingConfigurationTypeDef:
    return {
        "SourceConfiguration": ...,
    }


# ChimeSdkMeetingConfigurationTypeDef definition

class ChimeSdkMeetingConfigurationTypeDef(TypedDict):
    SourceConfiguration: NotRequired[SourceConfigurationTypeDef],  # (1)
    ArtifactsConfiguration: NotRequired[ArtifactsConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: SourceConfigurationTypeDef](./type_defs.md#sourceconfigurationtypedef) 
2. See [:material-code-braces: ArtifactsConfigurationTypeDef](./type_defs.md#artifactsconfigurationtypedef) 
## GetVoiceConnectorStreamingConfigurationResponseTypeDef

```python
# GetVoiceConnectorStreamingConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetVoiceConnectorStreamingConfigurationResponseTypeDef


def get_value() -> GetVoiceConnectorStreamingConfigurationResponseTypeDef:
    return {
        "StreamingConfiguration": ...,
    }


# GetVoiceConnectorStreamingConfigurationResponseTypeDef definition

class GetVoiceConnectorStreamingConfigurationResponseTypeDef(TypedDict):
    StreamingConfiguration: StreamingConfigurationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingConfigurationOutputTypeDef](./type_defs.md#streamingconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutVoiceConnectorStreamingConfigurationResponseTypeDef

```python
# PutVoiceConnectorStreamingConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutVoiceConnectorStreamingConfigurationResponseTypeDef


def get_value() -> PutVoiceConnectorStreamingConfigurationResponseTypeDef:
    return {
        "StreamingConfiguration": ...,
    }


# PutVoiceConnectorStreamingConfigurationResponseTypeDef definition

class PutVoiceConnectorStreamingConfigurationResponseTypeDef(TypedDict):
    StreamingConfiguration: StreamingConfigurationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingConfigurationOutputTypeDef](./type_defs.md#streamingconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUserSettingsResponseTypeDef

```python
# GetUserSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetUserSettingsResponseTypeDef


def get_value() -> GetUserSettingsResponseTypeDef:
    return {
        "UserSettings": ...,
    }


# GetUserSettingsResponseTypeDef definition

class GetUserSettingsResponseTypeDef(TypedDict):
    UserSettings: UserSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserSettingsTypeDef](./type_defs.md#usersettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserSettingsRequestTypeDef

```python
# UpdateUserSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import UpdateUserSettingsRequestTypeDef


def get_value() -> UpdateUserSettingsRequestTypeDef:
    return {
        "AccountId": ...,
    }


# UpdateUserSettingsRequestTypeDef definition

class UpdateUserSettingsRequestTypeDef(TypedDict):
    AccountId: str,
    UserId: str,
    UserSettings: UserSettingsTypeDef,  # (1)
```

1. See [:material-code-braces: UserSettingsTypeDef](./type_defs.md#usersettingstypedef) 
## PutVoiceConnectorTerminationRequestTypeDef

```python
# PutVoiceConnectorTerminationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutVoiceConnectorTerminationRequestTypeDef


def get_value() -> PutVoiceConnectorTerminationRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# PutVoiceConnectorTerminationRequestTypeDef definition

class PutVoiceConnectorTerminationRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    Termination: TerminationUnionTypeDef,  # (1)
```

1. See [:material-code-braces: TerminationTypeDef](./type_defs.md#terminationtypedef) [:material-code-braces: TerminationOutputTypeDef](./type_defs.md#terminationoutputtypedef) 
## PutVoiceConnectorEmergencyCallingConfigurationRequestTypeDef

```python
# PutVoiceConnectorEmergencyCallingConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutVoiceConnectorEmergencyCallingConfigurationRequestTypeDef


def get_value() -> PutVoiceConnectorEmergencyCallingConfigurationRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# PutVoiceConnectorEmergencyCallingConfigurationRequestTypeDef definition

class PutVoiceConnectorEmergencyCallingConfigurationRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    EmergencyCallingConfiguration: EmergencyCallingConfigurationUnionTypeDef,  # (1)
```

1. See [:material-code-braces: EmergencyCallingConfigurationTypeDef](./type_defs.md#emergencycallingconfigurationtypedef) [:material-code-braces: EmergencyCallingConfigurationOutputTypeDef](./type_defs.md#emergencycallingconfigurationoutputtypedef) 
## PutVoiceConnectorOriginationRequestTypeDef

```python
# PutVoiceConnectorOriginationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutVoiceConnectorOriginationRequestTypeDef


def get_value() -> PutVoiceConnectorOriginationRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# PutVoiceConnectorOriginationRequestTypeDef definition

class PutVoiceConnectorOriginationRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    Origination: OriginationUnionTypeDef,  # (1)
```

1. See [:material-code-braces: OriginationTypeDef](./type_defs.md#originationtypedef) [:material-code-braces: OriginationOutputTypeDef](./type_defs.md#originationoutputtypedef) 
## MediaCapturePipelineTypeDef

```python
# MediaCapturePipelineTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import MediaCapturePipelineTypeDef


def get_value() -> MediaCapturePipelineTypeDef:
    return {
        "MediaPipelineId": ...,
    }


# MediaCapturePipelineTypeDef definition

class MediaCapturePipelineTypeDef(TypedDict):
    MediaPipelineId: NotRequired[str],
    SourceType: NotRequired[MediaPipelineSourceTypeType],  # (1)
    SourceArn: NotRequired[str],
    Status: NotRequired[MediaPipelineStatusType],  # (2)
    SinkType: NotRequired[MediaPipelineSinkTypeType],  # (3)
    SinkArn: NotRequired[str],
    CreatedTimestamp: NotRequired[datetime],
    UpdatedTimestamp: NotRequired[datetime],
    ChimeSdkMeetingConfiguration: NotRequired[ChimeSdkMeetingConfigurationOutputTypeDef],  # (4)
```

1. See [:material-code-brackets: MediaPipelineSourceTypeType](./literals.md#mediapipelinesourcetypetype) 
2. See [:material-code-brackets: MediaPipelineStatusType](./literals.md#mediapipelinestatustype) 
3. See [:material-code-brackets: MediaPipelineSinkTypeType](./literals.md#mediapipelinesinktypetype) 
4. See [:material-code-braces: ChimeSdkMeetingConfigurationOutputTypeDef](./type_defs.md#chimesdkmeetingconfigurationoutputtypedef) 
## PutVoiceConnectorStreamingConfigurationRequestTypeDef

```python
# PutVoiceConnectorStreamingConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import PutVoiceConnectorStreamingConfigurationRequestTypeDef


def get_value() -> PutVoiceConnectorStreamingConfigurationRequestTypeDef:
    return {
        "VoiceConnectorId": ...,
    }


# PutVoiceConnectorStreamingConfigurationRequestTypeDef definition

class PutVoiceConnectorStreamingConfigurationRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    StreamingConfiguration: StreamingConfigurationUnionTypeDef,  # (1)
```

1. See [:material-code-braces: StreamingConfigurationTypeDef](./type_defs.md#streamingconfigurationtypedef) [:material-code-braces: StreamingConfigurationOutputTypeDef](./type_defs.md#streamingconfigurationoutputtypedef) 
## CreateMediaCapturePipelineResponseTypeDef

```python
# CreateMediaCapturePipelineResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateMediaCapturePipelineResponseTypeDef


def get_value() -> CreateMediaCapturePipelineResponseTypeDef:
    return {
        "MediaCapturePipeline": ...,
    }


# CreateMediaCapturePipelineResponseTypeDef definition

class CreateMediaCapturePipelineResponseTypeDef(TypedDict):
    MediaCapturePipeline: MediaCapturePipelineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MediaCapturePipelineTypeDef](./type_defs.md#mediacapturepipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMediaCapturePipelineResponseTypeDef

```python
# GetMediaCapturePipelineResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import GetMediaCapturePipelineResponseTypeDef


def get_value() -> GetMediaCapturePipelineResponseTypeDef:
    return {
        "MediaCapturePipeline": ...,
    }


# GetMediaCapturePipelineResponseTypeDef definition

class GetMediaCapturePipelineResponseTypeDef(TypedDict):
    MediaCapturePipeline: MediaCapturePipelineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MediaCapturePipelineTypeDef](./type_defs.md#mediacapturepipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMediaCapturePipelinesResponseTypeDef

```python
# ListMediaCapturePipelinesResponseTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import ListMediaCapturePipelinesResponseTypeDef


def get_value() -> ListMediaCapturePipelinesResponseTypeDef:
    return {
        "MediaCapturePipelines": ...,
    }


# ListMediaCapturePipelinesResponseTypeDef definition

class ListMediaCapturePipelinesResponseTypeDef(TypedDict):
    MediaCapturePipelines: List[MediaCapturePipelineTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MediaCapturePipelineTypeDef](./type_defs.md#mediacapturepipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMediaCapturePipelineRequestTypeDef

```python
# CreateMediaCapturePipelineRequestTypeDef TypedDict usage example

from types_aiobotocore_chime.type_defs import CreateMediaCapturePipelineRequestTypeDef


def get_value() -> CreateMediaCapturePipelineRequestTypeDef:
    return {
        "SourceType": ...,
    }


# CreateMediaCapturePipelineRequestTypeDef definition

class CreateMediaCapturePipelineRequestTypeDef(TypedDict):
    SourceType: MediaPipelineSourceTypeType,  # (1)
    SourceArn: str,
    SinkType: MediaPipelineSinkTypeType,  # (2)
    SinkArn: str,
    ClientRequestToken: NotRequired[str],
    ChimeSdkMeetingConfiguration: NotRequired[ChimeSdkMeetingConfigurationUnionTypeDef],  # (3)
```

1. See [:material-code-brackets: MediaPipelineSourceTypeType](./literals.md#mediapipelinesourcetypetype) 
2. See [:material-code-brackets: MediaPipelineSinkTypeType](./literals.md#mediapipelinesinktypetype) 
3. See [:material-code-braces: ChimeSdkMeetingConfigurationTypeDef](./type_defs.md#chimesdkmeetingconfigurationtypedef) [:material-code-braces: ChimeSdkMeetingConfigurationOutputTypeDef](./type_defs.md#chimesdkmeetingconfigurationoutputtypedef) 
