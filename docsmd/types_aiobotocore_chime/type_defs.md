# Type definitions

> [Index](../README.md) > [Chime](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Chime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
    type annotations stubs module [types-aiobotocore-chime](https://pypi.org/project/types-aiobotocore-chime/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## SelectedVideoStreamsUnionTypeDef

```python
# SelectedVideoStreamsUnionTypeDef definition

SelectedVideoStreamsUnionTypeDef = Union[
    SelectedVideoStreamsTypeDef,  # (1)
    SelectedVideoStreamsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SelectedVideoStreamsTypeDef](./type_defs.md#selectedvideostreamstypedef) 
2. See [:material-code-braces: SelectedVideoStreamsOutputTypeDef](./type_defs.md#selectedvideostreamsoutputtypedef) 

## SourceConfigurationUnionTypeDef

```python
# SourceConfigurationUnionTypeDef definition

SourceConfigurationUnionTypeDef = Union[
    SourceConfigurationTypeDef,  # (1)
    SourceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SourceConfigurationTypeDef](./type_defs.md#sourceconfigurationtypedef) 
2. See [:material-code-braces: SourceConfigurationOutputTypeDef](./type_defs.md#sourceconfigurationoutputtypedef) 



## AccountSettingsTypeDef

```python
# AccountSettingsTypeDef definition

class AccountSettingsTypeDef(TypedDict):
    DisableRemoteControl: NotRequired[bool],
    EnableDialOut: NotRequired[bool],
```

## SigninDelegateGroupTypeDef

```python
# SigninDelegateGroupTypeDef definition

class SigninDelegateGroupTypeDef(TypedDict):
    GroupName: NotRequired[str],
```

## AddressTypeDef

```python
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
# AlexaForBusinessMetadataTypeDef definition

class AlexaForBusinessMetadataTypeDef(TypedDict):
    IsAlexaForBusinessEnabled: NotRequired[bool],
    AlexaForBusinessRoomArn: NotRequired[str],
```

## IdentityTypeDef

```python
# IdentityTypeDef definition

class IdentityTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
```

## ChannelRetentionSettingsTypeDef

```python
# ChannelRetentionSettingsTypeDef definition

class ChannelRetentionSettingsTypeDef(TypedDict):
    RetentionDays: NotRequired[int],
```

## AppInstanceStreamingConfigurationTypeDef

```python
# AppInstanceStreamingConfigurationTypeDef definition

class AppInstanceStreamingConfigurationTypeDef(TypedDict):
    AppInstanceDataType: AppInstanceDataTypeType,  # (1)
    ResourceArn: str,
```

1. See [:material-code-brackets: AppInstanceDataTypeType](./literals.md#appinstancedatatypetype) 
## AppInstanceSummaryTypeDef

```python
# AppInstanceSummaryTypeDef definition

class AppInstanceSummaryTypeDef(TypedDict):
    AppInstanceArn: NotRequired[str],
    Name: NotRequired[str],
    Metadata: NotRequired[str],
```

## AppInstanceTypeDef

```python
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
# AppInstanceUserMembershipSummaryTypeDef definition

class AppInstanceUserMembershipSummaryTypeDef(TypedDict):
    Type: NotRequired[ChannelMembershipTypeType],  # (1)
    ReadMarkerTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: ChannelMembershipTypeType](./literals.md#channelmembershiptypetype) 
## AppInstanceUserSummaryTypeDef

```python
# AppInstanceUserSummaryTypeDef definition

class AppInstanceUserSummaryTypeDef(TypedDict):
    AppInstanceUserArn: NotRequired[str],
    Name: NotRequired[str],
    Metadata: NotRequired[str],
```

## AppInstanceUserTypeDef

```python
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
# AudioArtifactsConfigurationTypeDef definition

class AudioArtifactsConfigurationTypeDef(TypedDict):
    MuxType: AudioMuxTypeType,  # (1)
```

1. See [:material-code-brackets: AudioMuxTypeType](./literals.md#audiomuxtypetype) 
## ContentArtifactsConfigurationTypeDef

```python
# ContentArtifactsConfigurationTypeDef definition

class ContentArtifactsConfigurationTypeDef(TypedDict):
    State: ArtifactsStateType,  # (1)
    MuxType: NotRequired[ContentMuxTypeType],  # (2)
```

1. See [:material-code-brackets: ArtifactsStateType](./literals.md#artifactsstatetype) 
2. See [:material-code-brackets: ContentMuxTypeType](./literals.md#contentmuxtypetype) 
## VideoArtifactsConfigurationTypeDef

```python
# VideoArtifactsConfigurationTypeDef definition

class VideoArtifactsConfigurationTypeDef(TypedDict):
    State: ArtifactsStateType,  # (1)
    MuxType: NotRequired[VideoMuxTypeType],  # (2)
```

1. See [:material-code-brackets: ArtifactsStateType](./literals.md#artifactsstatetype) 
2. See [:material-code-brackets: VideoMuxTypeType](./literals.md#videomuxtypetype) 
## AssociatePhoneNumberWithUserRequestRequestTypeDef

```python
# AssociatePhoneNumberWithUserRequestRequestTypeDef definition

class AssociatePhoneNumberWithUserRequestRequestTypeDef(TypedDict):
    AccountId: str,
    UserId: str,
    E164PhoneNumber: str,
```

## AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef

```python
# AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef definition

class AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef(TypedDict):
    VoiceConnectorGroupId: str,
    E164PhoneNumbers: Sequence[str],
    ForceAssociate: NotRequired[bool],
```

## PhoneNumberErrorTypeDef

```python
# PhoneNumberErrorTypeDef definition

class PhoneNumberErrorTypeDef(TypedDict):
    PhoneNumberId: NotRequired[str],
    ErrorCode: NotRequired[ErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
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

## AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef

```python
# AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef definition

class AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    E164PhoneNumbers: Sequence[str],
    ForceAssociate: NotRequired[bool],
```

## AttendeeTypeDef

```python
# AttendeeTypeDef definition

class AttendeeTypeDef(TypedDict):
    ExternalUserId: NotRequired[str],
    AttendeeId: NotRequired[str],
    JoinToken: NotRequired[str],
```

## CreateAttendeeErrorTypeDef

```python
# CreateAttendeeErrorTypeDef definition

class CreateAttendeeErrorTypeDef(TypedDict):
    ExternalUserId: NotRequired[str],
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## BatchCreateChannelMembershipErrorTypeDef

```python
# BatchCreateChannelMembershipErrorTypeDef definition

class BatchCreateChannelMembershipErrorTypeDef(TypedDict):
    MemberArn: NotRequired[str],
    ErrorCode: NotRequired[ErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## BatchCreateChannelMembershipRequestRequestTypeDef

```python
# BatchCreateChannelMembershipRequestRequestTypeDef definition

class BatchCreateChannelMembershipRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MemberArns: Sequence[str],
    Type: NotRequired[ChannelMembershipTypeType],  # (1)
    ChimeBearer: NotRequired[str],
```

1. See [:material-code-brackets: ChannelMembershipTypeType](./literals.md#channelmembershiptypetype) 
## MembershipItemTypeDef

```python
# MembershipItemTypeDef definition

class MembershipItemTypeDef(TypedDict):
    MemberId: NotRequired[str],
    Role: NotRequired[RoomMembershipRoleType],  # (1)
```

1. See [:material-code-brackets: RoomMembershipRoleType](./literals.md#roommembershiproletype) 
## MemberErrorTypeDef

```python
# MemberErrorTypeDef definition

class MemberErrorTypeDef(TypedDict):
    MemberId: NotRequired[str],
    ErrorCode: NotRequired[ErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## BatchDeletePhoneNumberRequestRequestTypeDef

```python
# BatchDeletePhoneNumberRequestRequestTypeDef definition

class BatchDeletePhoneNumberRequestRequestTypeDef(TypedDict):
    PhoneNumberIds: Sequence[str],
```

## BatchSuspendUserRequestRequestTypeDef

```python
# BatchSuspendUserRequestRequestTypeDef definition

class BatchSuspendUserRequestRequestTypeDef(TypedDict):
    AccountId: str,
    UserIdList: Sequence[str],
```

## UserErrorTypeDef

```python
# UserErrorTypeDef definition

class UserErrorTypeDef(TypedDict):
    UserId: NotRequired[str],
    ErrorCode: NotRequired[ErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## BatchUnsuspendUserRequestRequestTypeDef

```python
# BatchUnsuspendUserRequestRequestTypeDef definition

class BatchUnsuspendUserRequestRequestTypeDef(TypedDict):
    AccountId: str,
    UserIdList: Sequence[str],
```

## UpdatePhoneNumberRequestItemTypeDef

```python
# UpdatePhoneNumberRequestItemTypeDef definition

class UpdatePhoneNumberRequestItemTypeDef(TypedDict):
    PhoneNumberId: str,
    ProductType: NotRequired[PhoneNumberProductTypeType],  # (1)
    CallingName: NotRequired[str],
```

1. See [:material-code-brackets: PhoneNumberProductTypeType](./literals.md#phonenumberproducttypetype) 
## BotTypeDef

```python
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
# BusinessCallingSettingsTypeDef definition

class BusinessCallingSettingsTypeDef(TypedDict):
    CdrBucket: NotRequired[str],
```

## CandidateAddressTypeDef

```python
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
# ConversationRetentionSettingsTypeDef definition

class ConversationRetentionSettingsTypeDef(TypedDict):
    RetentionDays: NotRequired[int],
```

## CreateAccountRequestRequestTypeDef

```python
# CreateAccountRequestRequestTypeDef definition

class CreateAccountRequestRequestTypeDef(TypedDict):
    Name: str,
```

## CreateAppInstanceAdminRequestRequestTypeDef

```python
# CreateAppInstanceAdminRequestRequestTypeDef definition

class CreateAppInstanceAdminRequestRequestTypeDef(TypedDict):
    AppInstanceAdminArn: str,
    AppInstanceArn: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## CreateBotRequestRequestTypeDef

```python
# CreateBotRequestRequestTypeDef definition

class CreateBotRequestRequestTypeDef(TypedDict):
    AccountId: str,
    DisplayName: str,
    Domain: NotRequired[str],
```

## CreateChannelBanRequestRequestTypeDef

```python
# CreateChannelBanRequestRequestTypeDef definition

class CreateChannelBanRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MemberArn: str,
    ChimeBearer: NotRequired[str],
```

## CreateChannelMembershipRequestRequestTypeDef

```python
# CreateChannelMembershipRequestRequestTypeDef definition

class CreateChannelMembershipRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MemberArn: str,
    Type: ChannelMembershipTypeType,  # (1)
    ChimeBearer: NotRequired[str],
```

1. See [:material-code-brackets: ChannelMembershipTypeType](./literals.md#channelmembershiptypetype) 
## CreateChannelModeratorRequestRequestTypeDef

```python
# CreateChannelModeratorRequestRequestTypeDef definition

class CreateChannelModeratorRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChannelModeratorArn: str,
    ChimeBearer: NotRequired[str],
```

## CreateMeetingDialOutRequestRequestTypeDef

```python
# CreateMeetingDialOutRequestRequestTypeDef definition

class CreateMeetingDialOutRequestRequestTypeDef(TypedDict):
    MeetingId: str,
    FromPhoneNumber: str,
    ToPhoneNumber: str,
    JoinToken: str,
```

## MeetingNotificationConfigurationTypeDef

```python
# MeetingNotificationConfigurationTypeDef definition

class MeetingNotificationConfigurationTypeDef(TypedDict):
    SnsTopicArn: NotRequired[str],
    SqsQueueArn: NotRequired[str],
```

## CreatePhoneNumberOrderRequestRequestTypeDef

```python
# CreatePhoneNumberOrderRequestRequestTypeDef definition

class CreatePhoneNumberOrderRequestRequestTypeDef(TypedDict):
    ProductType: PhoneNumberProductTypeType,  # (1)
    E164PhoneNumbers: Sequence[str],
```

1. See [:material-code-brackets: PhoneNumberProductTypeType](./literals.md#phonenumberproducttypetype) 
## GeoMatchParamsTypeDef

```python
# GeoMatchParamsTypeDef definition

class GeoMatchParamsTypeDef(TypedDict):
    Country: str,
    AreaCode: str,
```

## CreateRoomMembershipRequestRequestTypeDef

```python
# CreateRoomMembershipRequestRequestTypeDef definition

class CreateRoomMembershipRequestRequestTypeDef(TypedDict):
    AccountId: str,
    RoomId: str,
    MemberId: str,
    Role: NotRequired[RoomMembershipRoleType],  # (1)
```

1. See [:material-code-brackets: RoomMembershipRoleType](./literals.md#roommembershiproletype) 
## CreateRoomRequestRequestTypeDef

```python
# CreateRoomRequestRequestTypeDef definition

class CreateRoomRequestRequestTypeDef(TypedDict):
    AccountId: str,
    Name: str,
    ClientRequestToken: NotRequired[str],
```

## RoomTypeDef

```python
# RoomTypeDef definition

class RoomTypeDef(TypedDict):
    RoomId: NotRequired[str],
    Name: NotRequired[str],
    AccountId: NotRequired[str],
    CreatedBy: NotRequired[str],
    CreatedTimestamp: NotRequired[datetime],
    UpdatedTimestamp: NotRequired[datetime],
```

## CreateSipMediaApplicationCallRequestRequestTypeDef

```python
# CreateSipMediaApplicationCallRequestRequestTypeDef definition

class CreateSipMediaApplicationCallRequestRequestTypeDef(TypedDict):
    FromPhoneNumber: str,
    ToPhoneNumber: str,
    SipMediaApplicationId: str,
    SipHeaders: NotRequired[Mapping[str, str]],
```

## SipMediaApplicationCallTypeDef

```python
# SipMediaApplicationCallTypeDef definition

class SipMediaApplicationCallTypeDef(TypedDict):
    TransactionId: NotRequired[str],
```

## SipMediaApplicationEndpointTypeDef

```python
# SipMediaApplicationEndpointTypeDef definition

class SipMediaApplicationEndpointTypeDef(TypedDict):
    LambdaArn: NotRequired[str],
```

## SipRuleTargetApplicationTypeDef

```python
# SipRuleTargetApplicationTypeDef definition

class SipRuleTargetApplicationTypeDef(TypedDict):
    SipMediaApplicationId: NotRequired[str],
    Priority: NotRequired[int],
    AwsRegion: NotRequired[str],
```

## CreateUserRequestRequestTypeDef

```python
# CreateUserRequestRequestTypeDef definition

class CreateUserRequestRequestTypeDef(TypedDict):
    AccountId: str,
    Username: NotRequired[str],
    Email: NotRequired[str],
    UserType: NotRequired[UserTypeType],  # (1)
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
## VoiceConnectorItemTypeDef

```python
# VoiceConnectorItemTypeDef definition

class VoiceConnectorItemTypeDef(TypedDict):
    VoiceConnectorId: str,
    Priority: int,
```

## CreateVoiceConnectorRequestRequestTypeDef

```python
# CreateVoiceConnectorRequestRequestTypeDef definition

class CreateVoiceConnectorRequestRequestTypeDef(TypedDict):
    Name: str,
    RequireEncryption: bool,
    AwsRegion: NotRequired[VoiceConnectorAwsRegionType],  # (1)
```

1. See [:material-code-brackets: VoiceConnectorAwsRegionType](./literals.md#voiceconnectorawsregiontype) 
## VoiceConnectorTypeDef

```python
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
# CredentialTypeDef definition

class CredentialTypeDef(TypedDict):
    Username: NotRequired[str],
    Password: NotRequired[str],
```

## DNISEmergencyCallingConfigurationTypeDef

```python
# DNISEmergencyCallingConfigurationTypeDef definition

class DNISEmergencyCallingConfigurationTypeDef(TypedDict):
    EmergencyPhoneNumber: str,
    CallingCountry: str,
    TestPhoneNumber: NotRequired[str],
```

## DeleteAccountRequestRequestTypeDef

```python
# DeleteAccountRequestRequestTypeDef definition

class DeleteAccountRequestRequestTypeDef(TypedDict):
    AccountId: str,
```

## DeleteAppInstanceAdminRequestRequestTypeDef

```python
# DeleteAppInstanceAdminRequestRequestTypeDef definition

class DeleteAppInstanceAdminRequestRequestTypeDef(TypedDict):
    AppInstanceAdminArn: str,
    AppInstanceArn: str,
```

## DeleteAppInstanceRequestRequestTypeDef

```python
# DeleteAppInstanceRequestRequestTypeDef definition

class DeleteAppInstanceRequestRequestTypeDef(TypedDict):
    AppInstanceArn: str,
```

## DeleteAppInstanceStreamingConfigurationsRequestRequestTypeDef

```python
# DeleteAppInstanceStreamingConfigurationsRequestRequestTypeDef definition

class DeleteAppInstanceStreamingConfigurationsRequestRequestTypeDef(TypedDict):
    AppInstanceArn: str,
```

## DeleteAppInstanceUserRequestRequestTypeDef

```python
# DeleteAppInstanceUserRequestRequestTypeDef definition

class DeleteAppInstanceUserRequestRequestTypeDef(TypedDict):
    AppInstanceUserArn: str,
```

## DeleteAttendeeRequestRequestTypeDef

```python
# DeleteAttendeeRequestRequestTypeDef definition

class DeleteAttendeeRequestRequestTypeDef(TypedDict):
    MeetingId: str,
    AttendeeId: str,
```

## DeleteChannelBanRequestRequestTypeDef

```python
# DeleteChannelBanRequestRequestTypeDef definition

class DeleteChannelBanRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MemberArn: str,
    ChimeBearer: NotRequired[str],
```

## DeleteChannelMembershipRequestRequestTypeDef

```python
# DeleteChannelMembershipRequestRequestTypeDef definition

class DeleteChannelMembershipRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MemberArn: str,
    ChimeBearer: NotRequired[str],
```

## DeleteChannelMessageRequestRequestTypeDef

```python
# DeleteChannelMessageRequestRequestTypeDef definition

class DeleteChannelMessageRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MessageId: str,
    ChimeBearer: NotRequired[str],
```

## DeleteChannelModeratorRequestRequestTypeDef

```python
# DeleteChannelModeratorRequestRequestTypeDef definition

class DeleteChannelModeratorRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChannelModeratorArn: str,
    ChimeBearer: NotRequired[str],
```

## DeleteChannelRequestRequestTypeDef

```python
# DeleteChannelRequestRequestTypeDef definition

class DeleteChannelRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChimeBearer: NotRequired[str],
```

## DeleteEventsConfigurationRequestRequestTypeDef

```python
# DeleteEventsConfigurationRequestRequestTypeDef definition

class DeleteEventsConfigurationRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BotId: str,
```

## DeleteMediaCapturePipelineRequestRequestTypeDef

```python
# DeleteMediaCapturePipelineRequestRequestTypeDef definition

class DeleteMediaCapturePipelineRequestRequestTypeDef(TypedDict):
    MediaPipelineId: str,
```

## DeleteMeetingRequestRequestTypeDef

```python
# DeleteMeetingRequestRequestTypeDef definition

class DeleteMeetingRequestRequestTypeDef(TypedDict):
    MeetingId: str,
```

## DeletePhoneNumberRequestRequestTypeDef

```python
# DeletePhoneNumberRequestRequestTypeDef definition

class DeletePhoneNumberRequestRequestTypeDef(TypedDict):
    PhoneNumberId: str,
```

## DeleteProxySessionRequestRequestTypeDef

```python
# DeleteProxySessionRequestRequestTypeDef definition

class DeleteProxySessionRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    ProxySessionId: str,
```

## DeleteRoomMembershipRequestRequestTypeDef

```python
# DeleteRoomMembershipRequestRequestTypeDef definition

class DeleteRoomMembershipRequestRequestTypeDef(TypedDict):
    AccountId: str,
    RoomId: str,
    MemberId: str,
```

## DeleteRoomRequestRequestTypeDef

```python
# DeleteRoomRequestRequestTypeDef definition

class DeleteRoomRequestRequestTypeDef(TypedDict):
    AccountId: str,
    RoomId: str,
```

## DeleteSipMediaApplicationRequestRequestTypeDef

```python
# DeleteSipMediaApplicationRequestRequestTypeDef definition

class DeleteSipMediaApplicationRequestRequestTypeDef(TypedDict):
    SipMediaApplicationId: str,
```

## DeleteSipRuleRequestRequestTypeDef

```python
# DeleteSipRuleRequestRequestTypeDef definition

class DeleteSipRuleRequestRequestTypeDef(TypedDict):
    SipRuleId: str,
```

## DeleteVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef

```python
# DeleteVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef definition

class DeleteVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## DeleteVoiceConnectorGroupRequestRequestTypeDef

```python
# DeleteVoiceConnectorGroupRequestRequestTypeDef definition

class DeleteVoiceConnectorGroupRequestRequestTypeDef(TypedDict):
    VoiceConnectorGroupId: str,
```

## DeleteVoiceConnectorOriginationRequestRequestTypeDef

```python
# DeleteVoiceConnectorOriginationRequestRequestTypeDef definition

class DeleteVoiceConnectorOriginationRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## DeleteVoiceConnectorProxyRequestRequestTypeDef

```python
# DeleteVoiceConnectorProxyRequestRequestTypeDef definition

class DeleteVoiceConnectorProxyRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## DeleteVoiceConnectorRequestRequestTypeDef

```python
# DeleteVoiceConnectorRequestRequestTypeDef definition

class DeleteVoiceConnectorRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## DeleteVoiceConnectorStreamingConfigurationRequestRequestTypeDef

```python
# DeleteVoiceConnectorStreamingConfigurationRequestRequestTypeDef definition

class DeleteVoiceConnectorStreamingConfigurationRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef

```python
# DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef definition

class DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    Usernames: Sequence[str],
```

## DeleteVoiceConnectorTerminationRequestRequestTypeDef

```python
# DeleteVoiceConnectorTerminationRequestRequestTypeDef definition

class DeleteVoiceConnectorTerminationRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## DescribeAppInstanceAdminRequestRequestTypeDef

```python
# DescribeAppInstanceAdminRequestRequestTypeDef definition

class DescribeAppInstanceAdminRequestRequestTypeDef(TypedDict):
    AppInstanceAdminArn: str,
    AppInstanceArn: str,
```

## DescribeAppInstanceRequestRequestTypeDef

```python
# DescribeAppInstanceRequestRequestTypeDef definition

class DescribeAppInstanceRequestRequestTypeDef(TypedDict):
    AppInstanceArn: str,
```

## DescribeAppInstanceUserRequestRequestTypeDef

```python
# DescribeAppInstanceUserRequestRequestTypeDef definition

class DescribeAppInstanceUserRequestRequestTypeDef(TypedDict):
    AppInstanceUserArn: str,
```

## DescribeChannelBanRequestRequestTypeDef

```python
# DescribeChannelBanRequestRequestTypeDef definition

class DescribeChannelBanRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MemberArn: str,
    ChimeBearer: NotRequired[str],
```

## DescribeChannelMembershipForAppInstanceUserRequestRequestTypeDef

```python
# DescribeChannelMembershipForAppInstanceUserRequestRequestTypeDef definition

class DescribeChannelMembershipForAppInstanceUserRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    AppInstanceUserArn: str,
    ChimeBearer: NotRequired[str],
```

## DescribeChannelMembershipRequestRequestTypeDef

```python
# DescribeChannelMembershipRequestRequestTypeDef definition

class DescribeChannelMembershipRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MemberArn: str,
    ChimeBearer: NotRequired[str],
```

## DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef

```python
# DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef definition

class DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    AppInstanceUserArn: str,
    ChimeBearer: NotRequired[str],
```

## DescribeChannelModeratorRequestRequestTypeDef

```python
# DescribeChannelModeratorRequestRequestTypeDef definition

class DescribeChannelModeratorRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChannelModeratorArn: str,
    ChimeBearer: NotRequired[str],
```

## DescribeChannelRequestRequestTypeDef

```python
# DescribeChannelRequestRequestTypeDef definition

class DescribeChannelRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChimeBearer: NotRequired[str],
```

## DisassociatePhoneNumberFromUserRequestRequestTypeDef

```python
# DisassociatePhoneNumberFromUserRequestRequestTypeDef definition

class DisassociatePhoneNumberFromUserRequestRequestTypeDef(TypedDict):
    AccountId: str,
    UserId: str,
```

## DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef

```python
# DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef definition

class DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef(TypedDict):
    VoiceConnectorGroupId: str,
    E164PhoneNumbers: Sequence[str],
```

## DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef

```python
# DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef definition

class DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    E164PhoneNumbers: Sequence[str],
```

## DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef

```python
# DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef definition

class DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef(TypedDict):
    AccountId: str,
    GroupNames: Sequence[str],
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
## EventsConfigurationTypeDef

```python
# EventsConfigurationTypeDef definition

class EventsConfigurationTypeDef(TypedDict):
    BotId: NotRequired[str],
    OutboundEventsHTTPSEndpoint: NotRequired[str],
    LambdaFunctionArn: NotRequired[str],
```

## GetAccountRequestRequestTypeDef

```python
# GetAccountRequestRequestTypeDef definition

class GetAccountRequestRequestTypeDef(TypedDict):
    AccountId: str,
```

## GetAccountSettingsRequestRequestTypeDef

```python
# GetAccountSettingsRequestRequestTypeDef definition

class GetAccountSettingsRequestRequestTypeDef(TypedDict):
    AccountId: str,
```

## GetAppInstanceRetentionSettingsRequestRequestTypeDef

```python
# GetAppInstanceRetentionSettingsRequestRequestTypeDef definition

class GetAppInstanceRetentionSettingsRequestRequestTypeDef(TypedDict):
    AppInstanceArn: str,
```

## GetAppInstanceStreamingConfigurationsRequestRequestTypeDef

```python
# GetAppInstanceStreamingConfigurationsRequestRequestTypeDef definition

class GetAppInstanceStreamingConfigurationsRequestRequestTypeDef(TypedDict):
    AppInstanceArn: str,
```

## GetAttendeeRequestRequestTypeDef

```python
# GetAttendeeRequestRequestTypeDef definition

class GetAttendeeRequestRequestTypeDef(TypedDict):
    MeetingId: str,
    AttendeeId: str,
```

## GetBotRequestRequestTypeDef

```python
# GetBotRequestRequestTypeDef definition

class GetBotRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BotId: str,
```

## GetChannelMessageRequestRequestTypeDef

```python
# GetChannelMessageRequestRequestTypeDef definition

class GetChannelMessageRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MessageId: str,
    ChimeBearer: NotRequired[str],
```

## GetEventsConfigurationRequestRequestTypeDef

```python
# GetEventsConfigurationRequestRequestTypeDef definition

class GetEventsConfigurationRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BotId: str,
```

## VoiceConnectorSettingsTypeDef

```python
# VoiceConnectorSettingsTypeDef definition

class VoiceConnectorSettingsTypeDef(TypedDict):
    CdrBucket: NotRequired[str],
```

## GetMediaCapturePipelineRequestRequestTypeDef

```python
# GetMediaCapturePipelineRequestRequestTypeDef definition

class GetMediaCapturePipelineRequestRequestTypeDef(TypedDict):
    MediaPipelineId: str,
```

## GetMeetingRequestRequestTypeDef

```python
# GetMeetingRequestRequestTypeDef definition

class GetMeetingRequestRequestTypeDef(TypedDict):
    MeetingId: str,
```

## MessagingSessionEndpointTypeDef

```python
# MessagingSessionEndpointTypeDef definition

class MessagingSessionEndpointTypeDef(TypedDict):
    Url: NotRequired[str],
```

## GetPhoneNumberOrderRequestRequestTypeDef

```python
# GetPhoneNumberOrderRequestRequestTypeDef definition

class GetPhoneNumberOrderRequestRequestTypeDef(TypedDict):
    PhoneNumberOrderId: str,
```

## GetPhoneNumberRequestRequestTypeDef

```python
# GetPhoneNumberRequestRequestTypeDef definition

class GetPhoneNumberRequestRequestTypeDef(TypedDict):
    PhoneNumberId: str,
```

## GetProxySessionRequestRequestTypeDef

```python
# GetProxySessionRequestRequestTypeDef definition

class GetProxySessionRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    ProxySessionId: str,
```

## GetRetentionSettingsRequestRequestTypeDef

```python
# GetRetentionSettingsRequestRequestTypeDef definition

class GetRetentionSettingsRequestRequestTypeDef(TypedDict):
    AccountId: str,
```

## GetRoomRequestRequestTypeDef

```python
# GetRoomRequestRequestTypeDef definition

class GetRoomRequestRequestTypeDef(TypedDict):
    AccountId: str,
    RoomId: str,
```

## GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef

```python
# GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef definition

class GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef(TypedDict):
    SipMediaApplicationId: str,
```

## SipMediaApplicationLoggingConfigurationTypeDef

```python
# SipMediaApplicationLoggingConfigurationTypeDef definition

class SipMediaApplicationLoggingConfigurationTypeDef(TypedDict):
    EnableSipMediaApplicationMessageLogs: NotRequired[bool],
```

## GetSipMediaApplicationRequestRequestTypeDef

```python
# GetSipMediaApplicationRequestRequestTypeDef definition

class GetSipMediaApplicationRequestRequestTypeDef(TypedDict):
    SipMediaApplicationId: str,
```

## GetSipRuleRequestRequestTypeDef

```python
# GetSipRuleRequestRequestTypeDef definition

class GetSipRuleRequestRequestTypeDef(TypedDict):
    SipRuleId: str,
```

## GetUserRequestRequestTypeDef

```python
# GetUserRequestRequestTypeDef definition

class GetUserRequestRequestTypeDef(TypedDict):
    AccountId: str,
    UserId: str,
```

## GetUserSettingsRequestRequestTypeDef

```python
# GetUserSettingsRequestRequestTypeDef definition

class GetUserSettingsRequestRequestTypeDef(TypedDict):
    AccountId: str,
    UserId: str,
```

## GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef

```python
# GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef definition

class GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## GetVoiceConnectorGroupRequestRequestTypeDef

```python
# GetVoiceConnectorGroupRequestRequestTypeDef definition

class GetVoiceConnectorGroupRequestRequestTypeDef(TypedDict):
    VoiceConnectorGroupId: str,
```

## GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef

```python
# GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef definition

class GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## LoggingConfigurationTypeDef

```python
# LoggingConfigurationTypeDef definition

class LoggingConfigurationTypeDef(TypedDict):
    EnableSIPLogs: NotRequired[bool],
    EnableMediaMetricLogs: NotRequired[bool],
```

## GetVoiceConnectorOriginationRequestRequestTypeDef

```python
# GetVoiceConnectorOriginationRequestRequestTypeDef definition

class GetVoiceConnectorOriginationRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## GetVoiceConnectorProxyRequestRequestTypeDef

```python
# GetVoiceConnectorProxyRequestRequestTypeDef definition

class GetVoiceConnectorProxyRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## ProxyTypeDef

```python
# ProxyTypeDef definition

class ProxyTypeDef(TypedDict):
    DefaultSessionExpiryMinutes: NotRequired[int],
    Disabled: NotRequired[bool],
    FallBackPhoneNumber: NotRequired[str],
    PhoneNumberCountries: NotRequired[List[str]],
```

## GetVoiceConnectorRequestRequestTypeDef

```python
# GetVoiceConnectorRequestRequestTypeDef definition

class GetVoiceConnectorRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef

```python
# GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef definition

class GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## GetVoiceConnectorTerminationHealthRequestRequestTypeDef

```python
# GetVoiceConnectorTerminationHealthRequestRequestTypeDef definition

class GetVoiceConnectorTerminationHealthRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## TerminationHealthTypeDef

```python
# TerminationHealthTypeDef definition

class TerminationHealthTypeDef(TypedDict):
    Timestamp: NotRequired[datetime],
    Source: NotRequired[str],
```

## GetVoiceConnectorTerminationRequestRequestTypeDef

```python
# GetVoiceConnectorTerminationRequestRequestTypeDef definition

class GetVoiceConnectorTerminationRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## TerminationOutputTypeDef

```python
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
# InviteTypeDef definition

class InviteTypeDef(TypedDict):
    InviteId: NotRequired[str],
    Status: NotRequired[InviteStatusType],  # (1)
    EmailAddress: NotRequired[str],
    EmailStatus: NotRequired[EmailStatusType],  # (2)
```

1. See [:material-code-brackets: InviteStatusType](./literals.md#invitestatustype) 
2. See [:material-code-brackets: EmailStatusType](./literals.md#emailstatustype) 
## InviteUsersRequestRequestTypeDef

```python
# InviteUsersRequestRequestTypeDef definition

class InviteUsersRequestRequestTypeDef(TypedDict):
    AccountId: str,
    UserEmailList: Sequence[str],
    UserType: NotRequired[UserTypeType],  # (1)
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAccountsRequestRequestTypeDef

```python
# ListAccountsRequestRequestTypeDef definition

class ListAccountsRequestRequestTypeDef(TypedDict):
    Name: NotRequired[str],
    UserEmail: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListAppInstanceAdminsRequestRequestTypeDef

```python
# ListAppInstanceAdminsRequestRequestTypeDef definition

class ListAppInstanceAdminsRequestRequestTypeDef(TypedDict):
    AppInstanceArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListAppInstanceUsersRequestRequestTypeDef

```python
# ListAppInstanceUsersRequestRequestTypeDef definition

class ListAppInstanceUsersRequestRequestTypeDef(TypedDict):
    AppInstanceArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListAppInstancesRequestRequestTypeDef

```python
# ListAppInstancesRequestRequestTypeDef definition

class ListAppInstancesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListAttendeeTagsRequestRequestTypeDef

```python
# ListAttendeeTagsRequestRequestTypeDef definition

class ListAttendeeTagsRequestRequestTypeDef(TypedDict):
    MeetingId: str,
    AttendeeId: str,
```

## ListAttendeesRequestRequestTypeDef

```python
# ListAttendeesRequestRequestTypeDef definition

class ListAttendeesRequestRequestTypeDef(TypedDict):
    MeetingId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListBotsRequestRequestTypeDef

```python
# ListBotsRequestRequestTypeDef definition

class ListBotsRequestRequestTypeDef(TypedDict):
    AccountId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListChannelBansRequestRequestTypeDef

```python
# ListChannelBansRequestRequestTypeDef definition

class ListChannelBansRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ChimeBearer: NotRequired[str],
```

## ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef

```python
# ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef definition

class ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef(TypedDict):
    AppInstanceUserArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ChimeBearer: NotRequired[str],
```

## ListChannelMembershipsRequestRequestTypeDef

```python
# ListChannelMembershipsRequestRequestTypeDef definition

class ListChannelMembershipsRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    Type: NotRequired[ChannelMembershipTypeType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ChimeBearer: NotRequired[str],
```

1. See [:material-code-brackets: ChannelMembershipTypeType](./literals.md#channelmembershiptypetype) 
## ListChannelModeratorsRequestRequestTypeDef

```python
# ListChannelModeratorsRequestRequestTypeDef definition

class ListChannelModeratorsRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ChimeBearer: NotRequired[str],
```

## ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef

```python
# ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef definition

class ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef(TypedDict):
    AppInstanceUserArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ChimeBearer: NotRequired[str],
```

## ListChannelsRequestRequestTypeDef

```python
# ListChannelsRequestRequestTypeDef definition

class ListChannelsRequestRequestTypeDef(TypedDict):
    AppInstanceArn: str,
    Privacy: NotRequired[ChannelPrivacyType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ChimeBearer: NotRequired[str],
```

1. See [:material-code-brackets: ChannelPrivacyType](./literals.md#channelprivacytype) 
## ListMediaCapturePipelinesRequestRequestTypeDef

```python
# ListMediaCapturePipelinesRequestRequestTypeDef definition

class ListMediaCapturePipelinesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListMeetingTagsRequestRequestTypeDef

```python
# ListMeetingTagsRequestRequestTypeDef definition

class ListMeetingTagsRequestRequestTypeDef(TypedDict):
    MeetingId: str,
```

## ListMeetingsRequestRequestTypeDef

```python
# ListMeetingsRequestRequestTypeDef definition

class ListMeetingsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListPhoneNumberOrdersRequestRequestTypeDef

```python
# ListPhoneNumberOrdersRequestRequestTypeDef definition

class ListPhoneNumberOrdersRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListPhoneNumbersRequestRequestTypeDef

```python
# ListPhoneNumbersRequestRequestTypeDef definition

class ListPhoneNumbersRequestRequestTypeDef(TypedDict):
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
## ListProxySessionsRequestRequestTypeDef

```python
# ListProxySessionsRequestRequestTypeDef definition

class ListProxySessionsRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    Status: NotRequired[ProxySessionStatusType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: ProxySessionStatusType](./literals.md#proxysessionstatustype) 
## ListRoomMembershipsRequestRequestTypeDef

```python
# ListRoomMembershipsRequestRequestTypeDef definition

class ListRoomMembershipsRequestRequestTypeDef(TypedDict):
    AccountId: str,
    RoomId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListRoomsRequestRequestTypeDef

```python
# ListRoomsRequestRequestTypeDef definition

class ListRoomsRequestRequestTypeDef(TypedDict):
    AccountId: str,
    MemberId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListSipMediaApplicationsRequestRequestTypeDef

```python
# ListSipMediaApplicationsRequestRequestTypeDef definition

class ListSipMediaApplicationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListSipRulesRequestRequestTypeDef

```python
# ListSipRulesRequestRequestTypeDef definition

class ListSipRulesRequestRequestTypeDef(TypedDict):
    SipMediaApplicationId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListSupportedPhoneNumberCountriesRequestRequestTypeDef

```python
# ListSupportedPhoneNumberCountriesRequestRequestTypeDef definition

class ListSupportedPhoneNumberCountriesRequestRequestTypeDef(TypedDict):
    ProductType: PhoneNumberProductTypeType,  # (1)
```

1. See [:material-code-brackets: PhoneNumberProductTypeType](./literals.md#phonenumberproducttypetype) 
## PhoneNumberCountryTypeDef

```python
# PhoneNumberCountryTypeDef definition

class PhoneNumberCountryTypeDef(TypedDict):
    CountryCode: NotRequired[str],
    SupportedPhoneNumberTypes: NotRequired[List[PhoneNumberTypeType]],  # (1)
```

1. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## ListUsersRequestRequestTypeDef

```python
# ListUsersRequestRequestTypeDef definition

class ListUsersRequestRequestTypeDef(TypedDict):
    AccountId: str,
    UserEmail: NotRequired[str],
    UserType: NotRequired[UserTypeType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
## ListVoiceConnectorGroupsRequestRequestTypeDef

```python
# ListVoiceConnectorGroupsRequestRequestTypeDef definition

class ListVoiceConnectorGroupsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef

```python
# ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef definition

class ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
```

## ListVoiceConnectorsRequestRequestTypeDef

```python
# ListVoiceConnectorsRequestRequestTypeDef definition

class ListVoiceConnectorsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## LogoutUserRequestRequestTypeDef

```python
# LogoutUserRequestRequestTypeDef definition

class LogoutUserRequestRequestTypeDef(TypedDict):
    AccountId: str,
    UserId: str,
```

## MediaPlacementTypeDef

```python
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
# OrderedPhoneNumberTypeDef definition

class OrderedPhoneNumberTypeDef(TypedDict):
    E164PhoneNumber: NotRequired[str],
    Status: NotRequired[OrderedPhoneNumberStatusType],  # (1)
```

1. See [:material-code-brackets: OrderedPhoneNumberStatusType](./literals.md#orderedphonenumberstatustype) 
## OriginationRouteTypeDef

```python
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
# ParticipantTypeDef definition

class ParticipantTypeDef(TypedDict):
    PhoneNumber: NotRequired[str],
    ProxyPhoneNumber: NotRequired[str],
```

## PhoneNumberAssociationTypeDef

```python
# PhoneNumberAssociationTypeDef definition

class PhoneNumberAssociationTypeDef(TypedDict):
    Value: NotRequired[str],
    Name: NotRequired[PhoneNumberAssociationNameType],  # (1)
    AssociatedTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: PhoneNumberAssociationNameType](./literals.md#phonenumberassociationnametype) 
## PhoneNumberCapabilitiesTypeDef

```python
# PhoneNumberCapabilitiesTypeDef definition

class PhoneNumberCapabilitiesTypeDef(TypedDict):
    InboundCall: NotRequired[bool],
    OutboundCall: NotRequired[bool],
    InboundSMS: NotRequired[bool],
    OutboundSMS: NotRequired[bool],
    InboundMMS: NotRequired[bool],
    OutboundMMS: NotRequired[bool],
```

## PutEventsConfigurationRequestRequestTypeDef

```python
# PutEventsConfigurationRequestRequestTypeDef definition

class PutEventsConfigurationRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BotId: str,
    OutboundEventsHTTPSEndpoint: NotRequired[str],
    LambdaFunctionArn: NotRequired[str],
```

## PutVoiceConnectorProxyRequestRequestTypeDef

```python
# PutVoiceConnectorProxyRequestRequestTypeDef definition

class PutVoiceConnectorProxyRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    DefaultSessionExpiryMinutes: int,
    PhoneNumberPoolCountries: Sequence[str],
    FallBackPhoneNumber: NotRequired[str],
    Disabled: NotRequired[bool],
```

## TerminationTypeDef

```python
# TerminationTypeDef definition

class TerminationTypeDef(TypedDict):
    CpsLimit: NotRequired[int],
    DefaultPhoneNumber: NotRequired[str],
    CallingRegions: NotRequired[Sequence[str]],
    CidrAllowedList: NotRequired[Sequence[str]],
    Disabled: NotRequired[bool],
```

## RedactChannelMessageRequestRequestTypeDef

```python
# RedactChannelMessageRequestRequestTypeDef definition

class RedactChannelMessageRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MessageId: str,
    ChimeBearer: NotRequired[str],
```

## RedactConversationMessageRequestRequestTypeDef

```python
# RedactConversationMessageRequestRequestTypeDef definition

class RedactConversationMessageRequestRequestTypeDef(TypedDict):
    AccountId: str,
    ConversationId: str,
    MessageId: str,
```

## RedactRoomMessageRequestRequestTypeDef

```python
# RedactRoomMessageRequestRequestTypeDef definition

class RedactRoomMessageRequestRequestTypeDef(TypedDict):
    AccountId: str,
    RoomId: str,
    MessageId: str,
```

## RegenerateSecurityTokenRequestRequestTypeDef

```python
# RegenerateSecurityTokenRequestRequestTypeDef definition

class RegenerateSecurityTokenRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BotId: str,
```

## ResetPersonalPINRequestRequestTypeDef

```python
# ResetPersonalPINRequestRequestTypeDef definition

class ResetPersonalPINRequestRequestTypeDef(TypedDict):
    AccountId: str,
    UserId: str,
```

## RestorePhoneNumberRequestRequestTypeDef

```python
# RestorePhoneNumberRequestRequestTypeDef definition

class RestorePhoneNumberRequestRequestTypeDef(TypedDict):
    PhoneNumberId: str,
```

## RoomRetentionSettingsTypeDef

```python
# RoomRetentionSettingsTypeDef definition

class RoomRetentionSettingsTypeDef(TypedDict):
    RetentionDays: NotRequired[int],
```

## SearchAvailablePhoneNumbersRequestRequestTypeDef

```python
# SearchAvailablePhoneNumbersRequestRequestTypeDef definition

class SearchAvailablePhoneNumbersRequestRequestTypeDef(TypedDict):
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
# SelectedVideoStreamsOutputTypeDef definition

class SelectedVideoStreamsOutputTypeDef(TypedDict):
    AttendeeIds: NotRequired[List[str]],
    ExternalUserIds: NotRequired[List[str]],
```

## SelectedVideoStreamsTypeDef

```python
# SelectedVideoStreamsTypeDef definition

class SelectedVideoStreamsTypeDef(TypedDict):
    AttendeeIds: NotRequired[Sequence[str]],
    ExternalUserIds: NotRequired[Sequence[str]],
```

## SendChannelMessageRequestRequestTypeDef

```python
# SendChannelMessageRequestRequestTypeDef definition

class SendChannelMessageRequestRequestTypeDef(TypedDict):
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
## StopMeetingTranscriptionRequestRequestTypeDef

```python
# StopMeetingTranscriptionRequestRequestTypeDef definition

class StopMeetingTranscriptionRequestRequestTypeDef(TypedDict):
    MeetingId: str,
```

## StreamingNotificationTargetTypeDef

```python
# StreamingNotificationTargetTypeDef definition

class StreamingNotificationTargetTypeDef(TypedDict):
    NotificationTarget: NotificationTargetType,  # (1)
```

1. See [:material-code-brackets: NotificationTargetType](./literals.md#notificationtargettype) 
## TelephonySettingsTypeDef

```python
# TelephonySettingsTypeDef definition

class TelephonySettingsTypeDef(TypedDict):
    InboundCalling: bool,
    OutboundCalling: bool,
    SMS: bool,
```

## UntagAttendeeRequestRequestTypeDef

```python
# UntagAttendeeRequestRequestTypeDef definition

class UntagAttendeeRequestRequestTypeDef(TypedDict):
    MeetingId: str,
    AttendeeId: str,
    TagKeys: Sequence[str],
```

## UntagMeetingRequestRequestTypeDef

```python
# UntagMeetingRequestRequestTypeDef definition

class UntagMeetingRequestRequestTypeDef(TypedDict):
    MeetingId: str,
    TagKeys: Sequence[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateAccountRequestRequestTypeDef

```python
# UpdateAccountRequestRequestTypeDef definition

class UpdateAccountRequestRequestTypeDef(TypedDict):
    AccountId: str,
    Name: NotRequired[str],
    DefaultLicense: NotRequired[LicenseType],  # (1)
```

1. See [:material-code-brackets: LicenseType](./literals.md#licensetype) 
## UpdateAppInstanceRequestRequestTypeDef

```python
# UpdateAppInstanceRequestRequestTypeDef definition

class UpdateAppInstanceRequestRequestTypeDef(TypedDict):
    AppInstanceArn: str,
    Name: str,
    Metadata: NotRequired[str],
```

## UpdateAppInstanceUserRequestRequestTypeDef

```python
# UpdateAppInstanceUserRequestRequestTypeDef definition

class UpdateAppInstanceUserRequestRequestTypeDef(TypedDict):
    AppInstanceUserArn: str,
    Name: str,
    Metadata: NotRequired[str],
```

## UpdateBotRequestRequestTypeDef

```python
# UpdateBotRequestRequestTypeDef definition

class UpdateBotRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BotId: str,
    Disabled: NotRequired[bool],
```

## UpdateChannelMessageRequestRequestTypeDef

```python
# UpdateChannelMessageRequestRequestTypeDef definition

class UpdateChannelMessageRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MessageId: str,
    Content: NotRequired[str],
    Metadata: NotRequired[str],
    ChimeBearer: NotRequired[str],
```

## UpdateChannelReadMarkerRequestRequestTypeDef

```python
# UpdateChannelReadMarkerRequestRequestTypeDef definition

class UpdateChannelReadMarkerRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChimeBearer: NotRequired[str],
```

## UpdateChannelRequestRequestTypeDef

```python
# UpdateChannelRequestRequestTypeDef definition

class UpdateChannelRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    Name: str,
    Mode: ChannelModeType,  # (1)
    Metadata: NotRequired[str],
    ChimeBearer: NotRequired[str],
```

1. See [:material-code-brackets: ChannelModeType](./literals.md#channelmodetype) 
## UpdatePhoneNumberRequestRequestTypeDef

```python
# UpdatePhoneNumberRequestRequestTypeDef definition

class UpdatePhoneNumberRequestRequestTypeDef(TypedDict):
    PhoneNumberId: str,
    ProductType: NotRequired[PhoneNumberProductTypeType],  # (1)
    CallingName: NotRequired[str],
```

1. See [:material-code-brackets: PhoneNumberProductTypeType](./literals.md#phonenumberproducttypetype) 
## UpdatePhoneNumberSettingsRequestRequestTypeDef

```python
# UpdatePhoneNumberSettingsRequestRequestTypeDef definition

class UpdatePhoneNumberSettingsRequestRequestTypeDef(TypedDict):
    CallingName: str,
```

## UpdateProxySessionRequestRequestTypeDef

```python
# UpdateProxySessionRequestRequestTypeDef definition

class UpdateProxySessionRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    ProxySessionId: str,
    Capabilities: Sequence[CapabilityType],  # (1)
    ExpiryMinutes: NotRequired[int],
```

1. See [:material-code-brackets: CapabilityType](./literals.md#capabilitytype) 
## UpdateRoomMembershipRequestRequestTypeDef

```python
# UpdateRoomMembershipRequestRequestTypeDef definition

class UpdateRoomMembershipRequestRequestTypeDef(TypedDict):
    AccountId: str,
    RoomId: str,
    MemberId: str,
    Role: NotRequired[RoomMembershipRoleType],  # (1)
```

1. See [:material-code-brackets: RoomMembershipRoleType](./literals.md#roommembershiproletype) 
## UpdateRoomRequestRequestTypeDef

```python
# UpdateRoomRequestRequestTypeDef definition

class UpdateRoomRequestRequestTypeDef(TypedDict):
    AccountId: str,
    RoomId: str,
    Name: NotRequired[str],
```

## UpdateSipMediaApplicationCallRequestRequestTypeDef

```python
# UpdateSipMediaApplicationCallRequestRequestTypeDef definition

class UpdateSipMediaApplicationCallRequestRequestTypeDef(TypedDict):
    SipMediaApplicationId: str,
    TransactionId: str,
    Arguments: Mapping[str, str],
```

## UpdateVoiceConnectorRequestRequestTypeDef

```python
# UpdateVoiceConnectorRequestRequestTypeDef definition

class UpdateVoiceConnectorRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    Name: str,
    RequireEncryption: bool,
```

## ValidateE911AddressRequestRequestTypeDef

```python
# ValidateE911AddressRequestRequestTypeDef definition

class ValidateE911AddressRequestRequestTypeDef(TypedDict):
    AwsAccountId: str,
    StreetNumber: str,
    StreetInfo: str,
    City: str,
    State: str,
    Country: str,
    PostalCode: str,
```

## UpdateAccountSettingsRequestRequestTypeDef

```python
# UpdateAccountSettingsRequestRequestTypeDef definition

class UpdateAccountSettingsRequestRequestTypeDef(TypedDict):
    AccountId: str,
    AccountSettings: AccountSettingsTypeDef,  # (1)
```

1. See [:material-code-braces: AccountSettingsTypeDef](./type_defs.md#accountsettingstypedef) 
## AccountTypeDef

```python
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
## AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef

```python
# AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef definition

class AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef(TypedDict):
    AccountId: str,
    SigninDelegateGroups: Sequence[SigninDelegateGroupTypeDef],  # (1)
```

1. See [:material-code-braces: SigninDelegateGroupTypeDef](./type_defs.md#signindelegategrouptypedef) 
## UpdateUserRequestItemTypeDef

```python
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
## UpdateUserRequestRequestTypeDef

```python
# UpdateUserRequestRequestTypeDef definition

class UpdateUserRequestRequestTypeDef(TypedDict):
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
# AppInstanceAdminSummaryTypeDef definition

class AppInstanceAdminSummaryTypeDef(TypedDict):
    Admin: NotRequired[IdentityTypeDef],  # (1)
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
## AppInstanceAdminTypeDef

```python
# AppInstanceAdminTypeDef definition

class AppInstanceAdminTypeDef(TypedDict):
    Admin: NotRequired[IdentityTypeDef],  # (1)
    AppInstanceArn: NotRequired[str],
    CreatedTimestamp: NotRequired[datetime],
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
## BatchChannelMembershipsTypeDef

```python
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
# ChannelBanSummaryTypeDef definition

class ChannelBanSummaryTypeDef(TypedDict):
    Member: NotRequired[IdentityTypeDef],  # (1)
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
## ChannelBanTypeDef

```python
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
# ChannelMembershipSummaryTypeDef definition

class ChannelMembershipSummaryTypeDef(TypedDict):
    Member: NotRequired[IdentityTypeDef],  # (1)
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
## ChannelMembershipTypeDef

```python
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
# ChannelModeratorSummaryTypeDef definition

class ChannelModeratorSummaryTypeDef(TypedDict):
    Moderator: NotRequired[IdentityTypeDef],  # (1)
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
## ChannelModeratorTypeDef

```python
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
# AppInstanceRetentionSettingsTypeDef definition

class AppInstanceRetentionSettingsTypeDef(TypedDict):
    ChannelRetentionSettings: NotRequired[ChannelRetentionSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: ChannelRetentionSettingsTypeDef](./type_defs.md#channelretentionsettingstypedef) 
## PutAppInstanceStreamingConfigurationsRequestRequestTypeDef

```python
# PutAppInstanceStreamingConfigurationsRequestRequestTypeDef definition

class PutAppInstanceStreamingConfigurationsRequestRequestTypeDef(TypedDict):
    AppInstanceArn: str,
    AppInstanceStreamingConfigurations: Sequence[AppInstanceStreamingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: AppInstanceStreamingConfigurationTypeDef](./type_defs.md#appinstancestreamingconfigurationtypedef) 
## ArtifactsConfigurationTypeDef

```python
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
# AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef definition

class AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef(TypedDict):
    PhoneNumberErrors: List[PhoneNumberErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberErrorTypeDef](./type_defs.md#phonenumbererrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef

```python
# AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef definition

class AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef(TypedDict):
    PhoneNumberErrors: List[PhoneNumberErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberErrorTypeDef](./type_defs.md#phonenumbererrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeletePhoneNumberResponseTypeDef

```python
# BatchDeletePhoneNumberResponseTypeDef definition

class BatchDeletePhoneNumberResponseTypeDef(TypedDict):
    PhoneNumberErrors: List[PhoneNumberErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberErrorTypeDef](./type_defs.md#phonenumbererrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdatePhoneNumberResponseTypeDef

```python
# BatchUpdatePhoneNumberResponseTypeDef definition

class BatchUpdatePhoneNumberResponseTypeDef(TypedDict):
    PhoneNumberErrors: List[PhoneNumberErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberErrorTypeDef](./type_defs.md#phonenumbererrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAppInstanceAdminResponseTypeDef

```python
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
# CreateAppInstanceResponseTypeDef definition

class CreateAppInstanceResponseTypeDef(TypedDict):
    AppInstanceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAppInstanceUserResponseTypeDef

```python
# CreateAppInstanceUserResponseTypeDef definition

class CreateAppInstanceUserResponseTypeDef(TypedDict):
    AppInstanceUserArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateChannelBanResponseTypeDef

```python
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
# CreateChannelResponseTypeDef definition

class CreateChannelResponseTypeDef(TypedDict):
    ChannelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMeetingDialOutResponseTypeDef

```python
# CreateMeetingDialOutResponseTypeDef definition

class CreateMeetingDialOutResponseTypeDef(TypedDict):
    TransactionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAppInstanceResponseTypeDef

```python
# DescribeAppInstanceResponseTypeDef definition

class DescribeAppInstanceResponseTypeDef(TypedDict):
    AppInstance: AppInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppInstanceTypeDef](./type_defs.md#appinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAppInstanceUserResponseTypeDef

```python
# DescribeAppInstanceUserResponseTypeDef definition

class DescribeAppInstanceUserResponseTypeDef(TypedDict):
    AppInstanceUser: AppInstanceUserTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppInstanceUserTypeDef](./type_defs.md#appinstanceusertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef

```python
# DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef definition

class DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef(TypedDict):
    PhoneNumberErrors: List[PhoneNumberErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberErrorTypeDef](./type_defs.md#phonenumbererrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef

```python
# DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef definition

class DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef(TypedDict):
    PhoneNumberErrors: List[PhoneNumberErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberErrorTypeDef](./type_defs.md#phonenumbererrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccountSettingsResponseTypeDef

```python
# GetAccountSettingsResponseTypeDef definition

class GetAccountSettingsResponseTypeDef(TypedDict):
    AccountSettings: AccountSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountSettingsTypeDef](./type_defs.md#accountsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAppInstanceStreamingConfigurationsResponseTypeDef

```python
# GetAppInstanceStreamingConfigurationsResponseTypeDef definition

class GetAppInstanceStreamingConfigurationsResponseTypeDef(TypedDict):
    AppInstanceStreamingConfigurations: List[AppInstanceStreamingConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppInstanceStreamingConfigurationTypeDef](./type_defs.md#appinstancestreamingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPhoneNumberSettingsResponseTypeDef

```python
# GetPhoneNumberSettingsResponseTypeDef definition

class GetPhoneNumberSettingsResponseTypeDef(TypedDict):
    CallingName: str,
    CallingNameUpdatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAppInstanceUsersResponseTypeDef

```python
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
# ListVoiceConnectorTerminationCredentialsResponseTypeDef definition

class ListVoiceConnectorTerminationCredentialsResponseTypeDef(TypedDict):
    Usernames: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAppInstanceStreamingConfigurationsResponseTypeDef

```python
# PutAppInstanceStreamingConfigurationsResponseTypeDef definition

class PutAppInstanceStreamingConfigurationsResponseTypeDef(TypedDict):
    AppInstanceStreamingConfigurations: List[AppInstanceStreamingConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppInstanceStreamingConfigurationTypeDef](./type_defs.md#appinstancestreamingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RedactChannelMessageResponseTypeDef

```python
# RedactChannelMessageResponseTypeDef definition

class RedactChannelMessageResponseTypeDef(TypedDict):
    ChannelArn: str,
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchAvailablePhoneNumbersResponseTypeDef

```python
# SearchAvailablePhoneNumbersResponseTypeDef definition

class SearchAvailablePhoneNumbersResponseTypeDef(TypedDict):
    E164PhoneNumbers: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendChannelMessageResponseTypeDef

```python
# SendChannelMessageResponseTypeDef definition

class SendChannelMessageResponseTypeDef(TypedDict):
    ChannelArn: str,
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAppInstanceResponseTypeDef

```python
# UpdateAppInstanceResponseTypeDef definition

class UpdateAppInstanceResponseTypeDef(TypedDict):
    AppInstanceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAppInstanceUserResponseTypeDef

```python
# UpdateAppInstanceUserResponseTypeDef definition

class UpdateAppInstanceUserResponseTypeDef(TypedDict):
    AppInstanceUserArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateChannelMessageResponseTypeDef

```python
# UpdateChannelMessageResponseTypeDef definition

class UpdateChannelMessageResponseTypeDef(TypedDict):
    ChannelArn: str,
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateChannelReadMarkerResponseTypeDef

```python
# UpdateChannelReadMarkerResponseTypeDef definition

class UpdateChannelReadMarkerResponseTypeDef(TypedDict):
    ChannelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateChannelResponseTypeDef

```python
# UpdateChannelResponseTypeDef definition

class UpdateChannelResponseTypeDef(TypedDict):
    ChannelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## BatchCreateRoomMembershipRequestRequestTypeDef

```python
# BatchCreateRoomMembershipRequestRequestTypeDef definition

class BatchCreateRoomMembershipRequestRequestTypeDef(TypedDict):
    AccountId: str,
    RoomId: str,
    MembershipItemList: Sequence[MembershipItemTypeDef],  # (1)
```

1. See [:material-code-braces: MembershipItemTypeDef](./type_defs.md#membershipitemtypedef) 
## BatchCreateRoomMembershipResponseTypeDef

```python
# BatchCreateRoomMembershipResponseTypeDef definition

class BatchCreateRoomMembershipResponseTypeDef(TypedDict):
    Errors: List[MemberErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MemberErrorTypeDef](./type_defs.md#membererrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchSuspendUserResponseTypeDef

```python
# BatchSuspendUserResponseTypeDef definition

class BatchSuspendUserResponseTypeDef(TypedDict):
    UserErrors: List[UserErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserErrorTypeDef](./type_defs.md#usererrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUnsuspendUserResponseTypeDef

```python
# BatchUnsuspendUserResponseTypeDef definition

class BatchUnsuspendUserResponseTypeDef(TypedDict):
    UserErrors: List[UserErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserErrorTypeDef](./type_defs.md#usererrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateUserResponseTypeDef

```python
# BatchUpdateUserResponseTypeDef definition

class BatchUpdateUserResponseTypeDef(TypedDict):
    UserErrors: List[UserErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserErrorTypeDef](./type_defs.md#usererrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdatePhoneNumberRequestRequestTypeDef

```python
# BatchUpdatePhoneNumberRequestRequestTypeDef definition

class BatchUpdatePhoneNumberRequestRequestTypeDef(TypedDict):
    UpdatePhoneNumberRequestItems: Sequence[UpdatePhoneNumberRequestItemTypeDef],  # (1)
```

1. See [:material-code-braces: UpdatePhoneNumberRequestItemTypeDef](./type_defs.md#updatephonenumberrequestitemtypedef) 
## CreateBotResponseTypeDef

```python
# CreateBotResponseTypeDef definition

class CreateBotResponseTypeDef(TypedDict):
    Bot: BotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BotTypeDef](./type_defs.md#bottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBotResponseTypeDef

```python
# GetBotResponseTypeDef definition

class GetBotResponseTypeDef(TypedDict):
    Bot: BotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BotTypeDef](./type_defs.md#bottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBotsResponseTypeDef

```python
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
# RegenerateSecurityTokenResponseTypeDef definition

class RegenerateSecurityTokenResponseTypeDef(TypedDict):
    Bot: BotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BotTypeDef](./type_defs.md#bottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBotResponseTypeDef

```python
# UpdateBotResponseTypeDef definition

class UpdateBotResponseTypeDef(TypedDict):
    Bot: BotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BotTypeDef](./type_defs.md#bottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ValidateE911AddressResponseTypeDef

```python
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
# ChannelMembershipForAppInstanceUserSummaryTypeDef definition

class ChannelMembershipForAppInstanceUserSummaryTypeDef(TypedDict):
    ChannelSummary: NotRequired[ChannelSummaryTypeDef],  # (1)
    AppInstanceUserMembershipSummary: NotRequired[AppInstanceUserMembershipSummaryTypeDef],  # (2)
```

1. See [:material-code-braces: ChannelSummaryTypeDef](./type_defs.md#channelsummarytypedef) 
2. See [:material-code-braces: AppInstanceUserMembershipSummaryTypeDef](./type_defs.md#appinstanceusermembershipsummarytypedef) 
## ChannelModeratedByAppInstanceUserSummaryTypeDef

```python
# ChannelModeratedByAppInstanceUserSummaryTypeDef definition

class ChannelModeratedByAppInstanceUserSummaryTypeDef(TypedDict):
    ChannelSummary: NotRequired[ChannelSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: ChannelSummaryTypeDef](./type_defs.md#channelsummarytypedef) 
## ListChannelsResponseTypeDef

```python
# ListChannelsResponseTypeDef definition

class ListChannelsResponseTypeDef(TypedDict):
    Channels: List[ChannelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ChannelSummaryTypeDef](./type_defs.md#channelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAppInstanceRequestRequestTypeDef

```python
# CreateAppInstanceRequestRequestTypeDef definition

class CreateAppInstanceRequestRequestTypeDef(TypedDict):
    Name: str,
    ClientRequestToken: str,
    Metadata: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateAppInstanceUserRequestRequestTypeDef

```python
# CreateAppInstanceUserRequestRequestTypeDef definition

class CreateAppInstanceUserRequestRequestTypeDef(TypedDict):
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
# CreateAttendeeRequestItemTypeDef definition

class CreateAttendeeRequestItemTypeDef(TypedDict):
    ExternalUserId: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateAttendeeRequestRequestTypeDef

```python
# CreateAttendeeRequestRequestTypeDef definition

class CreateAttendeeRequestRequestTypeDef(TypedDict):
    MeetingId: str,
    ExternalUserId: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateChannelRequestRequestTypeDef

```python
# CreateChannelRequestRequestTypeDef definition

class CreateChannelRequestRequestTypeDef(TypedDict):
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
# ListAttendeeTagsResponseTypeDef definition

class ListAttendeeTagsResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMeetingTagsResponseTypeDef

```python
# ListMeetingTagsResponseTypeDef definition

class ListMeetingTagsResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagAttendeeRequestRequestTypeDef

```python
# TagAttendeeRequestRequestTypeDef definition

class TagAttendeeRequestRequestTypeDef(TypedDict):
    MeetingId: str,
    AttendeeId: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagMeetingRequestRequestTypeDef

```python
# TagMeetingRequestRequestTypeDef definition

class TagMeetingRequestRequestTypeDef(TypedDict):
    MeetingId: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateMeetingRequestRequestTypeDef

```python
# CreateMeetingRequestRequestTypeDef definition

class CreateMeetingRequestRequestTypeDef(TypedDict):
    ClientRequestToken: str,
    ExternalMeetingId: NotRequired[str],
    MeetingHostId: NotRequired[str],
    MediaRegion: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    NotificationsConfiguration: NotRequired[MeetingNotificationConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: MeetingNotificationConfigurationTypeDef](./type_defs.md#meetingnotificationconfigurationtypedef) 
## CreateProxySessionRequestRequestTypeDef

```python
# CreateProxySessionRequestRequestTypeDef definition

class CreateProxySessionRequestRequestTypeDef(TypedDict):
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
# CreateRoomResponseTypeDef definition

class CreateRoomResponseTypeDef(TypedDict):
    Room: RoomTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoomTypeDef](./type_defs.md#roomtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRoomResponseTypeDef

```python
# GetRoomResponseTypeDef definition

class GetRoomResponseTypeDef(TypedDict):
    Room: RoomTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoomTypeDef](./type_defs.md#roomtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRoomsResponseTypeDef

```python
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
# UpdateRoomResponseTypeDef definition

class UpdateRoomResponseTypeDef(TypedDict):
    Room: RoomTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoomTypeDef](./type_defs.md#roomtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSipMediaApplicationCallResponseTypeDef

```python
# CreateSipMediaApplicationCallResponseTypeDef definition

class CreateSipMediaApplicationCallResponseTypeDef(TypedDict):
    SipMediaApplicationCall: SipMediaApplicationCallTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SipMediaApplicationCallTypeDef](./type_defs.md#sipmediaapplicationcalltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSipMediaApplicationCallResponseTypeDef

```python
# UpdateSipMediaApplicationCallResponseTypeDef definition

class UpdateSipMediaApplicationCallResponseTypeDef(TypedDict):
    SipMediaApplicationCall: SipMediaApplicationCallTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SipMediaApplicationCallTypeDef](./type_defs.md#sipmediaapplicationcalltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSipMediaApplicationRequestRequestTypeDef

```python
# CreateSipMediaApplicationRequestRequestTypeDef definition

class CreateSipMediaApplicationRequestRequestTypeDef(TypedDict):
    AwsRegion: str,
    Name: str,
    Endpoints: Sequence[SipMediaApplicationEndpointTypeDef],  # (1)
```

1. See [:material-code-braces: SipMediaApplicationEndpointTypeDef](./type_defs.md#sipmediaapplicationendpointtypedef) 
## SipMediaApplicationTypeDef

```python
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
## UpdateSipMediaApplicationRequestRequestTypeDef

```python
# UpdateSipMediaApplicationRequestRequestTypeDef definition

class UpdateSipMediaApplicationRequestRequestTypeDef(TypedDict):
    SipMediaApplicationId: str,
    Name: NotRequired[str],
    Endpoints: NotRequired[Sequence[SipMediaApplicationEndpointTypeDef]],  # (1)
```

1. See [:material-code-braces: SipMediaApplicationEndpointTypeDef](./type_defs.md#sipmediaapplicationendpointtypedef) 
## CreateSipRuleRequestRequestTypeDef

```python
# CreateSipRuleRequestRequestTypeDef definition

class CreateSipRuleRequestRequestTypeDef(TypedDict):
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
## UpdateSipRuleRequestRequestTypeDef

```python
# UpdateSipRuleRequestRequestTypeDef definition

class UpdateSipRuleRequestRequestTypeDef(TypedDict):
    SipRuleId: str,
    Name: str,
    Disabled: NotRequired[bool],
    TargetApplications: NotRequired[Sequence[SipRuleTargetApplicationTypeDef]],  # (1)
```

1. See [:material-code-braces: SipRuleTargetApplicationTypeDef](./type_defs.md#sipruletargetapplicationtypedef) 
## CreateVoiceConnectorGroupRequestRequestTypeDef

```python
# CreateVoiceConnectorGroupRequestRequestTypeDef definition

class CreateVoiceConnectorGroupRequestRequestTypeDef(TypedDict):
    Name: str,
    VoiceConnectorItems: NotRequired[Sequence[VoiceConnectorItemTypeDef]],  # (1)
```

1. See [:material-code-braces: VoiceConnectorItemTypeDef](./type_defs.md#voiceconnectoritemtypedef) 
## UpdateVoiceConnectorGroupRequestRequestTypeDef

```python
# UpdateVoiceConnectorGroupRequestRequestTypeDef definition

class UpdateVoiceConnectorGroupRequestRequestTypeDef(TypedDict):
    VoiceConnectorGroupId: str,
    Name: str,
    VoiceConnectorItems: Sequence[VoiceConnectorItemTypeDef],  # (1)
```

1. See [:material-code-braces: VoiceConnectorItemTypeDef](./type_defs.md#voiceconnectoritemtypedef) 
## VoiceConnectorGroupTypeDef

```python
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
# CreateVoiceConnectorResponseTypeDef definition

class CreateVoiceConnectorResponseTypeDef(TypedDict):
    VoiceConnector: VoiceConnectorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VoiceConnectorTypeDef](./type_defs.md#voiceconnectortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVoiceConnectorResponseTypeDef

```python
# GetVoiceConnectorResponseTypeDef definition

class GetVoiceConnectorResponseTypeDef(TypedDict):
    VoiceConnector: VoiceConnectorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VoiceConnectorTypeDef](./type_defs.md#voiceconnectortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVoiceConnectorsResponseTypeDef

```python
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
# UpdateVoiceConnectorResponseTypeDef definition

class UpdateVoiceConnectorResponseTypeDef(TypedDict):
    VoiceConnector: VoiceConnectorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VoiceConnectorTypeDef](./type_defs.md#voiceconnectortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef

```python
# PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef definition

class PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    Credentials: NotRequired[Sequence[CredentialTypeDef]],  # (1)
```

1. See [:material-code-braces: CredentialTypeDef](./type_defs.md#credentialtypedef) 
## EmergencyCallingConfigurationOutputTypeDef

```python
# EmergencyCallingConfigurationOutputTypeDef definition

class EmergencyCallingConfigurationOutputTypeDef(TypedDict):
    DNIS: NotRequired[List[DNISEmergencyCallingConfigurationTypeDef]],  # (1)
```

1. See [:material-code-braces: DNISEmergencyCallingConfigurationTypeDef](./type_defs.md#dnisemergencycallingconfigurationtypedef) 
## EmergencyCallingConfigurationTypeDef

```python
# EmergencyCallingConfigurationTypeDef definition

class EmergencyCallingConfigurationTypeDef(TypedDict):
    DNIS: NotRequired[Sequence[DNISEmergencyCallingConfigurationTypeDef]],  # (1)
```

1. See [:material-code-braces: DNISEmergencyCallingConfigurationTypeDef](./type_defs.md#dnisemergencycallingconfigurationtypedef) 
## TranscriptionConfigurationTypeDef

```python
# TranscriptionConfigurationTypeDef definition

class TranscriptionConfigurationTypeDef(TypedDict):
    EngineTranscribeSettings: NotRequired[EngineTranscribeSettingsTypeDef],  # (1)
    EngineTranscribeMedicalSettings: NotRequired[EngineTranscribeMedicalSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: EngineTranscribeSettingsTypeDef](./type_defs.md#enginetranscribesettingstypedef) 
2. See [:material-code-braces: EngineTranscribeMedicalSettingsTypeDef](./type_defs.md#enginetranscribemedicalsettingstypedef) 
## GetEventsConfigurationResponseTypeDef

```python
# GetEventsConfigurationResponseTypeDef definition

class GetEventsConfigurationResponseTypeDef(TypedDict):
    EventsConfiguration: EventsConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventsConfigurationTypeDef](./type_defs.md#eventsconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutEventsConfigurationResponseTypeDef

```python
# PutEventsConfigurationResponseTypeDef definition

class PutEventsConfigurationResponseTypeDef(TypedDict):
    EventsConfiguration: EventsConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventsConfigurationTypeDef](./type_defs.md#eventsconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGlobalSettingsResponseTypeDef

```python
# GetGlobalSettingsResponseTypeDef definition

class GetGlobalSettingsResponseTypeDef(TypedDict):
    BusinessCalling: BusinessCallingSettingsTypeDef,  # (1)
    VoiceConnector: VoiceConnectorSettingsTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BusinessCallingSettingsTypeDef](./type_defs.md#businesscallingsettingstypedef) 
2. See [:material-code-braces: VoiceConnectorSettingsTypeDef](./type_defs.md#voiceconnectorsettingstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGlobalSettingsRequestRequestTypeDef

```python
# UpdateGlobalSettingsRequestRequestTypeDef definition

class UpdateGlobalSettingsRequestRequestTypeDef(TypedDict):
    BusinessCalling: NotRequired[BusinessCallingSettingsTypeDef],  # (1)
    VoiceConnector: NotRequired[VoiceConnectorSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: BusinessCallingSettingsTypeDef](./type_defs.md#businesscallingsettingstypedef) 
2. See [:material-code-braces: VoiceConnectorSettingsTypeDef](./type_defs.md#voiceconnectorsettingstypedef) 
## GetMessagingSessionEndpointResponseTypeDef

```python
# GetMessagingSessionEndpointResponseTypeDef definition

class GetMessagingSessionEndpointResponseTypeDef(TypedDict):
    Endpoint: MessagingSessionEndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessagingSessionEndpointTypeDef](./type_defs.md#messagingsessionendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSipMediaApplicationLoggingConfigurationResponseTypeDef

```python
# GetSipMediaApplicationLoggingConfigurationResponseTypeDef definition

class GetSipMediaApplicationLoggingConfigurationResponseTypeDef(TypedDict):
    SipMediaApplicationLoggingConfiguration: SipMediaApplicationLoggingConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SipMediaApplicationLoggingConfigurationTypeDef](./type_defs.md#sipmediaapplicationloggingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef

```python
# PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef definition

class PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef(TypedDict):
    SipMediaApplicationId: str,
    SipMediaApplicationLoggingConfiguration: NotRequired[SipMediaApplicationLoggingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: SipMediaApplicationLoggingConfigurationTypeDef](./type_defs.md#sipmediaapplicationloggingconfigurationtypedef) 
## PutSipMediaApplicationLoggingConfigurationResponseTypeDef

```python
# PutSipMediaApplicationLoggingConfigurationResponseTypeDef definition

class PutSipMediaApplicationLoggingConfigurationResponseTypeDef(TypedDict):
    SipMediaApplicationLoggingConfiguration: SipMediaApplicationLoggingConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SipMediaApplicationLoggingConfigurationTypeDef](./type_defs.md#sipmediaapplicationloggingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVoiceConnectorLoggingConfigurationResponseTypeDef

```python
# GetVoiceConnectorLoggingConfigurationResponseTypeDef definition

class GetVoiceConnectorLoggingConfigurationResponseTypeDef(TypedDict):
    LoggingConfiguration: LoggingConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef

```python
# PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef definition

class PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    LoggingConfiguration: LoggingConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
## PutVoiceConnectorLoggingConfigurationResponseTypeDef

```python
# PutVoiceConnectorLoggingConfigurationResponseTypeDef definition

class PutVoiceConnectorLoggingConfigurationResponseTypeDef(TypedDict):
    LoggingConfiguration: LoggingConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVoiceConnectorProxyResponseTypeDef

```python
# GetVoiceConnectorProxyResponseTypeDef definition

class GetVoiceConnectorProxyResponseTypeDef(TypedDict):
    Proxy: ProxyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProxyTypeDef](./type_defs.md#proxytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutVoiceConnectorProxyResponseTypeDef

```python
# PutVoiceConnectorProxyResponseTypeDef definition

class PutVoiceConnectorProxyResponseTypeDef(TypedDict):
    Proxy: ProxyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProxyTypeDef](./type_defs.md#proxytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVoiceConnectorTerminationHealthResponseTypeDef

```python
# GetVoiceConnectorTerminationHealthResponseTypeDef definition

class GetVoiceConnectorTerminationHealthResponseTypeDef(TypedDict):
    TerminationHealth: TerminationHealthTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TerminationHealthTypeDef](./type_defs.md#terminationhealthtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVoiceConnectorTerminationResponseTypeDef

```python
# GetVoiceConnectorTerminationResponseTypeDef definition

class GetVoiceConnectorTerminationResponseTypeDef(TypedDict):
    Termination: TerminationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TerminationOutputTypeDef](./type_defs.md#terminationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutVoiceConnectorTerminationResponseTypeDef

```python
# PutVoiceConnectorTerminationResponseTypeDef definition

class PutVoiceConnectorTerminationResponseTypeDef(TypedDict):
    Termination: TerminationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TerminationOutputTypeDef](./type_defs.md#terminationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InviteUsersResponseTypeDef

```python
# InviteUsersResponseTypeDef definition

class InviteUsersResponseTypeDef(TypedDict):
    Invites: List[InviteTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InviteTypeDef](./type_defs.md#invitetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountsRequestListAccountsPaginateTypeDef

```python
# ListAccountsRequestListAccountsPaginateTypeDef definition

class ListAccountsRequestListAccountsPaginateTypeDef(TypedDict):
    Name: NotRequired[str],
    UserEmail: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUsersRequestListUsersPaginateTypeDef

```python
# ListUsersRequestListUsersPaginateTypeDef definition

class ListUsersRequestListUsersPaginateTypeDef(TypedDict):
    AccountId: str,
    UserEmail: NotRequired[str],
    UserType: NotRequired[UserTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListChannelMessagesRequestRequestTypeDef

```python
# ListChannelMessagesRequestRequestTypeDef definition

class ListChannelMessagesRequestRequestTypeDef(TypedDict):
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
# ListSupportedPhoneNumberCountriesResponseTypeDef definition

class ListSupportedPhoneNumberCountriesResponseTypeDef(TypedDict):
    PhoneNumberCountries: List[PhoneNumberCountryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberCountryTypeDef](./type_defs.md#phonenumbercountrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MeetingTypeDef

```python
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
# OriginationOutputTypeDef definition

class OriginationOutputTypeDef(TypedDict):
    Routes: NotRequired[List[OriginationRouteTypeDef]],  # (1)
    Disabled: NotRequired[bool],
```

1. See [:material-code-braces: OriginationRouteTypeDef](./type_defs.md#originationroutetypedef) 
## OriginationTypeDef

```python
# OriginationTypeDef definition

class OriginationTypeDef(TypedDict):
    Routes: NotRequired[Sequence[OriginationRouteTypeDef]],  # (1)
    Disabled: NotRequired[bool],
```

1. See [:material-code-braces: OriginationRouteTypeDef](./type_defs.md#originationroutetypedef) 
## ProxySessionTypeDef

```python
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
## PutVoiceConnectorTerminationRequestRequestTypeDef

```python
# PutVoiceConnectorTerminationRequestRequestTypeDef definition

class PutVoiceConnectorTerminationRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    Termination: TerminationTypeDef,  # (1)
```

1. See [:material-code-braces: TerminationTypeDef](./type_defs.md#terminationtypedef) 
## RetentionSettingsTypeDef

```python
# RetentionSettingsTypeDef definition

class RetentionSettingsTypeDef(TypedDict):
    RoomRetentionSettings: NotRequired[RoomRetentionSettingsTypeDef],  # (1)
    ConversationRetentionSettings: NotRequired[ConversationRetentionSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: RoomRetentionSettingsTypeDef](./type_defs.md#roomretentionsettingstypedef) 
2. See [:material-code-braces: ConversationRetentionSettingsTypeDef](./type_defs.md#conversationretentionsettingstypedef) 
## SourceConfigurationOutputTypeDef

```python
# SourceConfigurationOutputTypeDef definition

class SourceConfigurationOutputTypeDef(TypedDict):
    SelectedVideoStreams: NotRequired[SelectedVideoStreamsOutputTypeDef],  # (1)
```

1. See [:material-code-braces: SelectedVideoStreamsOutputTypeDef](./type_defs.md#selectedvideostreamsoutputtypedef) 
## StreamingConfigurationOutputTypeDef

```python
# StreamingConfigurationOutputTypeDef definition

class StreamingConfigurationOutputTypeDef(TypedDict):
    DataRetentionInHours: int,
    Disabled: NotRequired[bool],
    StreamingNotificationTargets: NotRequired[List[StreamingNotificationTargetTypeDef]],  # (1)
```

1. See [:material-code-braces: StreamingNotificationTargetTypeDef](./type_defs.md#streamingnotificationtargettypedef) 
## StreamingConfigurationTypeDef

```python
# StreamingConfigurationTypeDef definition

class StreamingConfigurationTypeDef(TypedDict):
    DataRetentionInHours: int,
    Disabled: NotRequired[bool],
    StreamingNotificationTargets: NotRequired[Sequence[StreamingNotificationTargetTypeDef]],  # (1)
```

1. See [:material-code-braces: StreamingNotificationTargetTypeDef](./type_defs.md#streamingnotificationtargettypedef) 
## UserSettingsTypeDef

```python
# UserSettingsTypeDef definition

class UserSettingsTypeDef(TypedDict):
    Telephony: TelephonySettingsTypeDef,  # (1)
```

1. See [:material-code-braces: TelephonySettingsTypeDef](./type_defs.md#telephonysettingstypedef) 
## CreateAccountResponseTypeDef

```python
# CreateAccountResponseTypeDef definition

class CreateAccountResponseTypeDef(TypedDict):
    Account: AccountTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccountResponseTypeDef

```python
# GetAccountResponseTypeDef definition

class GetAccountResponseTypeDef(TypedDict):
    Account: AccountTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountsResponseTypeDef

```python
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
# UpdateAccountResponseTypeDef definition

class UpdateAccountResponseTypeDef(TypedDict):
    Account: AccountTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateUserRequestRequestTypeDef

```python
# BatchUpdateUserRequestRequestTypeDef definition

class BatchUpdateUserRequestRequestTypeDef(TypedDict):
    AccountId: str,
    UpdateUserRequestItems: Sequence[UpdateUserRequestItemTypeDef],  # (1)
```

1. See [:material-code-braces: UpdateUserRequestItemTypeDef](./type_defs.md#updateuserrequestitemtypedef) 
## CreateUserResponseTypeDef

```python
# CreateUserResponseTypeDef definition

class CreateUserResponseTypeDef(TypedDict):
    User: UserTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUserResponseTypeDef

```python
# GetUserResponseTypeDef definition

class GetUserResponseTypeDef(TypedDict):
    User: UserTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUsersResponseTypeDef

```python
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
# ResetPersonalPINResponseTypeDef definition

class ResetPersonalPINResponseTypeDef(TypedDict):
    User: UserTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserResponseTypeDef

```python
# UpdateUserResponseTypeDef definition

class UpdateUserResponseTypeDef(TypedDict):
    User: UserTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAppInstanceAdminsResponseTypeDef

```python
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
# DescribeAppInstanceAdminResponseTypeDef definition

class DescribeAppInstanceAdminResponseTypeDef(TypedDict):
    AppInstanceAdmin: AppInstanceAdminTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppInstanceAdminTypeDef](./type_defs.md#appinstanceadmintypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchCreateChannelMembershipResponseTypeDef

```python
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
# DescribeChannelBanResponseTypeDef definition

class DescribeChannelBanResponseTypeDef(TypedDict):
    ChannelBan: ChannelBanTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelBanTypeDef](./type_defs.md#channelbantypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChannelMembershipsResponseTypeDef

```python
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
# DescribeChannelMembershipResponseTypeDef definition

class DescribeChannelMembershipResponseTypeDef(TypedDict):
    ChannelMembership: ChannelMembershipTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelMembershipTypeDef](./type_defs.md#channelmembershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChannelMessagesResponseTypeDef

```python
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
# GetChannelMessageResponseTypeDef definition

class GetChannelMessageResponseTypeDef(TypedDict):
    ChannelMessage: ChannelMessageTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelMessageTypeDef](./type_defs.md#channelmessagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChannelModeratorsResponseTypeDef

```python
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
# DescribeChannelModeratorResponseTypeDef definition

class DescribeChannelModeratorResponseTypeDef(TypedDict):
    ChannelModerator: ChannelModeratorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelModeratorTypeDef](./type_defs.md#channelmoderatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeChannelResponseTypeDef

```python
# DescribeChannelResponseTypeDef definition

class DescribeChannelResponseTypeDef(TypedDict):
    Channel: ChannelTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAppInstanceRetentionSettingsResponseTypeDef

```python
# GetAppInstanceRetentionSettingsResponseTypeDef definition

class GetAppInstanceRetentionSettingsResponseTypeDef(TypedDict):
    AppInstanceRetentionSettings: AppInstanceRetentionSettingsTypeDef,  # (1)
    InitiateDeletionTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppInstanceRetentionSettingsTypeDef](./type_defs.md#appinstanceretentionsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAppInstanceRetentionSettingsRequestRequestTypeDef

```python
# PutAppInstanceRetentionSettingsRequestRequestTypeDef definition

class PutAppInstanceRetentionSettingsRequestRequestTypeDef(TypedDict):
    AppInstanceArn: str,
    AppInstanceRetentionSettings: AppInstanceRetentionSettingsTypeDef,  # (1)
```

1. See [:material-code-braces: AppInstanceRetentionSettingsTypeDef](./type_defs.md#appinstanceretentionsettingstypedef) 
## PutAppInstanceRetentionSettingsResponseTypeDef

```python
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
# DescribeChannelMembershipForAppInstanceUserResponseTypeDef definition

class DescribeChannelMembershipForAppInstanceUserResponseTypeDef(TypedDict):
    ChannelMembership: ChannelMembershipForAppInstanceUserSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelMembershipForAppInstanceUserSummaryTypeDef](./type_defs.md#channelmembershipforappinstanceusersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChannelMembershipsForAppInstanceUserResponseTypeDef

```python
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
# DescribeChannelModeratedByAppInstanceUserResponseTypeDef definition

class DescribeChannelModeratedByAppInstanceUserResponseTypeDef(TypedDict):
    Channel: ChannelModeratedByAppInstanceUserSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelModeratedByAppInstanceUserSummaryTypeDef](./type_defs.md#channelmoderatedbyappinstanceusersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChannelsModeratedByAppInstanceUserResponseTypeDef

```python
# ListChannelsModeratedByAppInstanceUserResponseTypeDef definition

class ListChannelsModeratedByAppInstanceUserResponseTypeDef(TypedDict):
    Channels: List[ChannelModeratedByAppInstanceUserSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ChannelModeratedByAppInstanceUserSummaryTypeDef](./type_defs.md#channelmoderatedbyappinstanceusersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchCreateAttendeeRequestRequestTypeDef

```python
# BatchCreateAttendeeRequestRequestTypeDef definition

class BatchCreateAttendeeRequestRequestTypeDef(TypedDict):
    MeetingId: str,
    Attendees: Sequence[CreateAttendeeRequestItemTypeDef],  # (1)
```

1. See [:material-code-braces: CreateAttendeeRequestItemTypeDef](./type_defs.md#createattendeerequestitemtypedef) 
## CreateMeetingWithAttendeesRequestRequestTypeDef

```python
# CreateMeetingWithAttendeesRequestRequestTypeDef definition

class CreateMeetingWithAttendeesRequestRequestTypeDef(TypedDict):
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
# CreateSipMediaApplicationResponseTypeDef definition

class CreateSipMediaApplicationResponseTypeDef(TypedDict):
    SipMediaApplication: SipMediaApplicationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SipMediaApplicationTypeDef](./type_defs.md#sipmediaapplicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSipMediaApplicationResponseTypeDef

```python
# GetSipMediaApplicationResponseTypeDef definition

class GetSipMediaApplicationResponseTypeDef(TypedDict):
    SipMediaApplication: SipMediaApplicationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SipMediaApplicationTypeDef](./type_defs.md#sipmediaapplicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSipMediaApplicationsResponseTypeDef

```python
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
# UpdateSipMediaApplicationResponseTypeDef definition

class UpdateSipMediaApplicationResponseTypeDef(TypedDict):
    SipMediaApplication: SipMediaApplicationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SipMediaApplicationTypeDef](./type_defs.md#sipmediaapplicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSipRuleResponseTypeDef

```python
# CreateSipRuleResponseTypeDef definition

class CreateSipRuleResponseTypeDef(TypedDict):
    SipRule: SipRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SipRuleTypeDef](./type_defs.md#sipruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSipRuleResponseTypeDef

```python
# GetSipRuleResponseTypeDef definition

class GetSipRuleResponseTypeDef(TypedDict):
    SipRule: SipRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SipRuleTypeDef](./type_defs.md#sipruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSipRulesResponseTypeDef

```python
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
# UpdateSipRuleResponseTypeDef definition

class UpdateSipRuleResponseTypeDef(TypedDict):
    SipRule: SipRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SipRuleTypeDef](./type_defs.md#sipruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVoiceConnectorGroupResponseTypeDef

```python
# CreateVoiceConnectorGroupResponseTypeDef definition

class CreateVoiceConnectorGroupResponseTypeDef(TypedDict):
    VoiceConnectorGroup: VoiceConnectorGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VoiceConnectorGroupTypeDef](./type_defs.md#voiceconnectorgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVoiceConnectorGroupResponseTypeDef

```python
# GetVoiceConnectorGroupResponseTypeDef definition

class GetVoiceConnectorGroupResponseTypeDef(TypedDict):
    VoiceConnectorGroup: VoiceConnectorGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VoiceConnectorGroupTypeDef](./type_defs.md#voiceconnectorgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVoiceConnectorGroupsResponseTypeDef

```python
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
# UpdateVoiceConnectorGroupResponseTypeDef definition

class UpdateVoiceConnectorGroupResponseTypeDef(TypedDict):
    VoiceConnectorGroup: VoiceConnectorGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VoiceConnectorGroupTypeDef](./type_defs.md#voiceconnectorgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef

```python
# GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef definition

class GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef(TypedDict):
    EmergencyCallingConfiguration: EmergencyCallingConfigurationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EmergencyCallingConfigurationOutputTypeDef](./type_defs.md#emergencycallingconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef

```python
# PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef definition

class PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef(TypedDict):
    EmergencyCallingConfiguration: EmergencyCallingConfigurationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EmergencyCallingConfigurationOutputTypeDef](./type_defs.md#emergencycallingconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef

```python
# PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef definition

class PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    EmergencyCallingConfiguration: EmergencyCallingConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: EmergencyCallingConfigurationTypeDef](./type_defs.md#emergencycallingconfigurationtypedef) 
## StartMeetingTranscriptionRequestRequestTypeDef

```python
# StartMeetingTranscriptionRequestRequestTypeDef definition

class StartMeetingTranscriptionRequestRequestTypeDef(TypedDict):
    MeetingId: str,
    TranscriptionConfiguration: TranscriptionConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: TranscriptionConfigurationTypeDef](./type_defs.md#transcriptionconfigurationtypedef) 
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
## ListMeetingsResponseTypeDef

```python
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
# CreateRoomMembershipResponseTypeDef definition

class CreateRoomMembershipResponseTypeDef(TypedDict):
    RoomMembership: RoomMembershipTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoomMembershipTypeDef](./type_defs.md#roommembershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRoomMembershipsResponseTypeDef

```python
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
# UpdateRoomMembershipResponseTypeDef definition

class UpdateRoomMembershipResponseTypeDef(TypedDict):
    RoomMembership: RoomMembershipTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoomMembershipTypeDef](./type_defs.md#roommembershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePhoneNumberOrderResponseTypeDef

```python
# CreatePhoneNumberOrderResponseTypeDef definition

class CreatePhoneNumberOrderResponseTypeDef(TypedDict):
    PhoneNumberOrder: PhoneNumberOrderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberOrderTypeDef](./type_defs.md#phonenumberordertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPhoneNumberOrderResponseTypeDef

```python
# GetPhoneNumberOrderResponseTypeDef definition

class GetPhoneNumberOrderResponseTypeDef(TypedDict):
    PhoneNumberOrder: PhoneNumberOrderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberOrderTypeDef](./type_defs.md#phonenumberordertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPhoneNumberOrdersResponseTypeDef

```python
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
# GetVoiceConnectorOriginationResponseTypeDef definition

class GetVoiceConnectorOriginationResponseTypeDef(TypedDict):
    Origination: OriginationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OriginationOutputTypeDef](./type_defs.md#originationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutVoiceConnectorOriginationResponseTypeDef

```python
# PutVoiceConnectorOriginationResponseTypeDef definition

class PutVoiceConnectorOriginationResponseTypeDef(TypedDict):
    Origination: OriginationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OriginationOutputTypeDef](./type_defs.md#originationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutVoiceConnectorOriginationRequestRequestTypeDef

```python
# PutVoiceConnectorOriginationRequestRequestTypeDef definition

class PutVoiceConnectorOriginationRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    Origination: OriginationTypeDef,  # (1)
```

1. See [:material-code-braces: OriginationTypeDef](./type_defs.md#originationtypedef) 
## CreateProxySessionResponseTypeDef

```python
# CreateProxySessionResponseTypeDef definition

class CreateProxySessionResponseTypeDef(TypedDict):
    ProxySession: ProxySessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProxySessionTypeDef](./type_defs.md#proxysessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProxySessionResponseTypeDef

```python
# GetProxySessionResponseTypeDef definition

class GetProxySessionResponseTypeDef(TypedDict):
    ProxySession: ProxySessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProxySessionTypeDef](./type_defs.md#proxysessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProxySessionsResponseTypeDef

```python
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
# UpdateProxySessionResponseTypeDef definition

class UpdateProxySessionResponseTypeDef(TypedDict):
    ProxySession: ProxySessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProxySessionTypeDef](./type_defs.md#proxysessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPhoneNumberResponseTypeDef

```python
# GetPhoneNumberResponseTypeDef definition

class GetPhoneNumberResponseTypeDef(TypedDict):
    PhoneNumber: PhoneNumberTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberTypeDef](./type_defs.md#phonenumbertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPhoneNumbersResponseTypeDef

```python
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
# RestorePhoneNumberResponseTypeDef definition

class RestorePhoneNumberResponseTypeDef(TypedDict):
    PhoneNumber: PhoneNumberTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberTypeDef](./type_defs.md#phonenumbertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePhoneNumberResponseTypeDef

```python
# UpdatePhoneNumberResponseTypeDef definition

class UpdatePhoneNumberResponseTypeDef(TypedDict):
    PhoneNumber: PhoneNumberTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberTypeDef](./type_defs.md#phonenumbertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRetentionSettingsResponseTypeDef

```python
# GetRetentionSettingsResponseTypeDef definition

class GetRetentionSettingsResponseTypeDef(TypedDict):
    RetentionSettings: RetentionSettingsTypeDef,  # (1)
    InitiateDeletionTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RetentionSettingsTypeDef](./type_defs.md#retentionsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRetentionSettingsRequestRequestTypeDef

```python
# PutRetentionSettingsRequestRequestTypeDef definition

class PutRetentionSettingsRequestRequestTypeDef(TypedDict):
    AccountId: str,
    RetentionSettings: RetentionSettingsTypeDef,  # (1)
```

1. See [:material-code-braces: RetentionSettingsTypeDef](./type_defs.md#retentionsettingstypedef) 
## PutRetentionSettingsResponseTypeDef

```python
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
# ChimeSdkMeetingConfigurationOutputTypeDef definition

class ChimeSdkMeetingConfigurationOutputTypeDef(TypedDict):
    SourceConfiguration: NotRequired[SourceConfigurationOutputTypeDef],  # (1)
    ArtifactsConfiguration: NotRequired[ArtifactsConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: SourceConfigurationOutputTypeDef](./type_defs.md#sourceconfigurationoutputtypedef) 
2. See [:material-code-braces: ArtifactsConfigurationTypeDef](./type_defs.md#artifactsconfigurationtypedef) 
## SourceConfigurationTypeDef

```python
# SourceConfigurationTypeDef definition

class SourceConfigurationTypeDef(TypedDict):
    SelectedVideoStreams: NotRequired[SelectedVideoStreamsUnionTypeDef],  # (1)
```

1. See [:material-code-braces: SelectedVideoStreamsTypeDef](./type_defs.md#selectedvideostreamstypedef) [:material-code-braces: SelectedVideoStreamsOutputTypeDef](./type_defs.md#selectedvideostreamsoutputtypedef) 
## GetVoiceConnectorStreamingConfigurationResponseTypeDef

```python
# GetVoiceConnectorStreamingConfigurationResponseTypeDef definition

class GetVoiceConnectorStreamingConfigurationResponseTypeDef(TypedDict):
    StreamingConfiguration: StreamingConfigurationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingConfigurationOutputTypeDef](./type_defs.md#streamingconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutVoiceConnectorStreamingConfigurationResponseTypeDef

```python
# PutVoiceConnectorStreamingConfigurationResponseTypeDef definition

class PutVoiceConnectorStreamingConfigurationResponseTypeDef(TypedDict):
    StreamingConfiguration: StreamingConfigurationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingConfigurationOutputTypeDef](./type_defs.md#streamingconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef

```python
# PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef definition

class PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef(TypedDict):
    VoiceConnectorId: str,
    StreamingConfiguration: StreamingConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: StreamingConfigurationTypeDef](./type_defs.md#streamingconfigurationtypedef) 
## GetUserSettingsResponseTypeDef

```python
# GetUserSettingsResponseTypeDef definition

class GetUserSettingsResponseTypeDef(TypedDict):
    UserSettings: UserSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserSettingsTypeDef](./type_defs.md#usersettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserSettingsRequestRequestTypeDef

```python
# UpdateUserSettingsRequestRequestTypeDef definition

class UpdateUserSettingsRequestRequestTypeDef(TypedDict):
    AccountId: str,
    UserId: str,
    UserSettings: UserSettingsTypeDef,  # (1)
```

1. See [:material-code-braces: UserSettingsTypeDef](./type_defs.md#usersettingstypedef) 
## MediaCapturePipelineTypeDef

```python
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
## CreateMediaCapturePipelineResponseTypeDef

```python
# CreateMediaCapturePipelineResponseTypeDef definition

class CreateMediaCapturePipelineResponseTypeDef(TypedDict):
    MediaCapturePipeline: MediaCapturePipelineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MediaCapturePipelineTypeDef](./type_defs.md#mediacapturepipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMediaCapturePipelineResponseTypeDef

```python
# GetMediaCapturePipelineResponseTypeDef definition

class GetMediaCapturePipelineResponseTypeDef(TypedDict):
    MediaCapturePipeline: MediaCapturePipelineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MediaCapturePipelineTypeDef](./type_defs.md#mediacapturepipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMediaCapturePipelinesResponseTypeDef

```python
# ListMediaCapturePipelinesResponseTypeDef definition

class ListMediaCapturePipelinesResponseTypeDef(TypedDict):
    MediaCapturePipelines: List[MediaCapturePipelineTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MediaCapturePipelineTypeDef](./type_defs.md#mediacapturepipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ChimeSdkMeetingConfigurationTypeDef

```python
# ChimeSdkMeetingConfigurationTypeDef definition

class ChimeSdkMeetingConfigurationTypeDef(TypedDict):
    SourceConfiguration: NotRequired[SourceConfigurationUnionTypeDef],  # (1)
    ArtifactsConfiguration: NotRequired[ArtifactsConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: SourceConfigurationTypeDef](./type_defs.md#sourceconfigurationtypedef) [:material-code-braces: SourceConfigurationOutputTypeDef](./type_defs.md#sourceconfigurationoutputtypedef) 
2. See [:material-code-braces: ArtifactsConfigurationTypeDef](./type_defs.md#artifactsconfigurationtypedef) 
## CreateMediaCapturePipelineRequestRequestTypeDef

```python
# CreateMediaCapturePipelineRequestRequestTypeDef definition

class CreateMediaCapturePipelineRequestRequestTypeDef(TypedDict):
    SourceType: MediaPipelineSourceTypeType,  # (1)
    SourceArn: str,
    SinkType: MediaPipelineSinkTypeType,  # (2)
    SinkArn: str,
    ClientRequestToken: NotRequired[str],
    ChimeSdkMeetingConfiguration: NotRequired[ChimeSdkMeetingConfigurationTypeDef],  # (3)
```

1. See [:material-code-brackets: MediaPipelineSourceTypeType](./literals.md#mediapipelinesourcetypetype) 
2. See [:material-code-brackets: MediaPipelineSinkTypeType](./literals.md#mediapipelinesinktypetype) 
3. See [:material-code-braces: ChimeSdkMeetingConfigurationTypeDef](./type_defs.md#chimesdkmeetingconfigurationtypedef) 
