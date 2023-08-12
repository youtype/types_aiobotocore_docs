# Type definitions

> [Index](../README.md) > [AlexaForBusiness](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AlexaForBusiness](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
    type annotations stubs module [types-aiobotocore-alexaforbusiness](https://pypi.org/project/types-aiobotocore-alexaforbusiness/).



## AddressBookDataTypeDef

```python
# AddressBookDataTypeDef definition

class AddressBookDataTypeDef(TypedDict):
    AddressBookArn: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## AddressBookTypeDef

```python
# AddressBookTypeDef definition

class AddressBookTypeDef(TypedDict):
    AddressBookArn: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## ApproveSkillRequestRequestTypeDef

```python
# ApproveSkillRequestRequestTypeDef definition

class ApproveSkillRequestRequestTypeDef(TypedDict):
    SkillId: str,
```

## AssociateContactWithAddressBookRequestRequestTypeDef

```python
# AssociateContactWithAddressBookRequestRequestTypeDef definition

class AssociateContactWithAddressBookRequestRequestTypeDef(TypedDict):
    ContactArn: str,
    AddressBookArn: str,
```

## AssociateDeviceWithNetworkProfileRequestRequestTypeDef

```python
# AssociateDeviceWithNetworkProfileRequestRequestTypeDef definition

class AssociateDeviceWithNetworkProfileRequestRequestTypeDef(TypedDict):
    DeviceArn: str,
    NetworkProfileArn: str,
```

## AssociateDeviceWithRoomRequestRequestTypeDef

```python
# AssociateDeviceWithRoomRequestRequestTypeDef definition

class AssociateDeviceWithRoomRequestRequestTypeDef(TypedDict):
    DeviceArn: NotRequired[str],
    RoomArn: NotRequired[str],
```

## AssociateSkillGroupWithRoomRequestRequestTypeDef

```python
# AssociateSkillGroupWithRoomRequestRequestTypeDef definition

class AssociateSkillGroupWithRoomRequestRequestTypeDef(TypedDict):
    SkillGroupArn: NotRequired[str],
    RoomArn: NotRequired[str],
```

## AssociateSkillWithSkillGroupRequestRequestTypeDef

```python
# AssociateSkillWithSkillGroupRequestRequestTypeDef definition

class AssociateSkillWithSkillGroupRequestRequestTypeDef(TypedDict):
    SkillId: str,
    SkillGroupArn: NotRequired[str],
```

## AssociateSkillWithUsersRequestRequestTypeDef

```python
# AssociateSkillWithUsersRequestRequestTypeDef definition

class AssociateSkillWithUsersRequestRequestTypeDef(TypedDict):
    SkillId: str,
```

## AudioTypeDef

```python
# AudioTypeDef definition

class AudioTypeDef(TypedDict):
    Locale: LocaleType,  # (1)
    Location: str,
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
## BusinessReportContentRangeTypeDef

```python
# BusinessReportContentRangeTypeDef definition

class BusinessReportContentRangeTypeDef(TypedDict):
    Interval: BusinessReportIntervalType,  # (1)
```

1. See [:material-code-brackets: BusinessReportIntervalType](./literals.md#businessreportintervaltype) 
## BusinessReportRecurrenceTypeDef

```python
# BusinessReportRecurrenceTypeDef definition

class BusinessReportRecurrenceTypeDef(TypedDict):
    StartDate: NotRequired[str],
```

## BusinessReportS3LocationTypeDef

```python
# BusinessReportS3LocationTypeDef definition

class BusinessReportS3LocationTypeDef(TypedDict):
    Path: NotRequired[str],
    BucketName: NotRequired[str],
```

## CategoryTypeDef

```python
# CategoryTypeDef definition

class CategoryTypeDef(TypedDict):
    CategoryId: NotRequired[int],
    CategoryName: NotRequired[str],
```

## ConferencePreferenceTypeDef

```python
# ConferencePreferenceTypeDef definition

class ConferencePreferenceTypeDef(TypedDict):
    DefaultConferenceProviderArn: NotRequired[str],
```

## IPDialInTypeDef

```python
# IPDialInTypeDef definition

class IPDialInTypeDef(TypedDict):
    Endpoint: str,
    CommsProtocol: CommsProtocolType,  # (1)
```

1. See [:material-code-brackets: CommsProtocolType](./literals.md#commsprotocoltype) 
## MeetingSettingTypeDef

```python
# MeetingSettingTypeDef definition

class MeetingSettingTypeDef(TypedDict):
    RequirePin: RequirePinType,  # (1)
```

1. See [:material-code-brackets: RequirePinType](./literals.md#requirepintype) 
## PSTNDialInTypeDef

```python
# PSTNDialInTypeDef definition

class PSTNDialInTypeDef(TypedDict):
    CountryCode: str,
    PhoneNumber: str,
    OneClickIdDelay: str,
    OneClickPinDelay: str,
```

## PhoneNumberTypeDef

```python
# PhoneNumberTypeDef definition

class PhoneNumberTypeDef(TypedDict):
    Number: str,
    Type: PhoneNumberTypeType,  # (1)
```

1. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
## SipAddressTypeDef

```python
# SipAddressTypeDef definition

class SipAddressTypeDef(TypedDict):
    Uri: str,
    Type: SipTypeType,  # (1)
```

1. See [:material-code-brackets: SipTypeType](./literals.md#siptypetype) 
## SsmlTypeDef

```python
# SsmlTypeDef definition

class SsmlTypeDef(TypedDict):
    Locale: LocaleType,  # (1)
    Value: str,
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
## TextTypeDef

```python
# TextTypeDef definition

class TextTypeDef(TypedDict):
    Locale: LocaleType,  # (1)
    Value: str,
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

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

## CreateEndOfMeetingReminderTypeDef

```python
# CreateEndOfMeetingReminderTypeDef definition

class CreateEndOfMeetingReminderTypeDef(TypedDict):
    ReminderAtMinutes: Sequence[int],
    ReminderType: EndOfMeetingReminderTypeType,  # (1)
    Enabled: bool,
```

1. See [:material-code-brackets: EndOfMeetingReminderTypeType](./literals.md#endofmeetingremindertypetype) 
## CreateInstantBookingTypeDef

```python
# CreateInstantBookingTypeDef definition

class CreateInstantBookingTypeDef(TypedDict):
    DurationInMinutes: int,
    Enabled: bool,
```

## CreateProactiveJoinTypeDef

```python
# CreateProactiveJoinTypeDef definition

class CreateProactiveJoinTypeDef(TypedDict):
    EnabledByMotion: bool,
```

## CreateRequireCheckInTypeDef

```python
# CreateRequireCheckInTypeDef definition

class CreateRequireCheckInTypeDef(TypedDict):
    ReleaseAfterMinutes: int,
    Enabled: bool,
```

## DeleteAddressBookRequestRequestTypeDef

```python
# DeleteAddressBookRequestRequestTypeDef definition

class DeleteAddressBookRequestRequestTypeDef(TypedDict):
    AddressBookArn: str,
```

## DeleteBusinessReportScheduleRequestRequestTypeDef

```python
# DeleteBusinessReportScheduleRequestRequestTypeDef definition

class DeleteBusinessReportScheduleRequestRequestTypeDef(TypedDict):
    ScheduleArn: str,
```

## DeleteConferenceProviderRequestRequestTypeDef

```python
# DeleteConferenceProviderRequestRequestTypeDef definition

class DeleteConferenceProviderRequestRequestTypeDef(TypedDict):
    ConferenceProviderArn: str,
```

## DeleteContactRequestRequestTypeDef

```python
# DeleteContactRequestRequestTypeDef definition

class DeleteContactRequestRequestTypeDef(TypedDict):
    ContactArn: str,
```

## DeleteDeviceRequestRequestTypeDef

```python
# DeleteDeviceRequestRequestTypeDef definition

class DeleteDeviceRequestRequestTypeDef(TypedDict):
    DeviceArn: str,
```

## DeleteDeviceUsageDataRequestRequestTypeDef

```python
# DeleteDeviceUsageDataRequestRequestTypeDef definition

class DeleteDeviceUsageDataRequestRequestTypeDef(TypedDict):
    DeviceArn: str,
    DeviceUsageType: DeviceUsageTypeType,  # (1)
```

1. See [:material-code-brackets: DeviceUsageTypeType](./literals.md#deviceusagetypetype) 
## DeleteGatewayGroupRequestRequestTypeDef

```python
# DeleteGatewayGroupRequestRequestTypeDef definition

class DeleteGatewayGroupRequestRequestTypeDef(TypedDict):
    GatewayGroupArn: str,
```

## DeleteNetworkProfileRequestRequestTypeDef

```python
# DeleteNetworkProfileRequestRequestTypeDef definition

class DeleteNetworkProfileRequestRequestTypeDef(TypedDict):
    NetworkProfileArn: str,
```

## DeleteProfileRequestRequestTypeDef

```python
# DeleteProfileRequestRequestTypeDef definition

class DeleteProfileRequestRequestTypeDef(TypedDict):
    ProfileArn: NotRequired[str],
```

## DeleteRoomRequestRequestTypeDef

```python
# DeleteRoomRequestRequestTypeDef definition

class DeleteRoomRequestRequestTypeDef(TypedDict):
    RoomArn: NotRequired[str],
```

## DeleteRoomSkillParameterRequestRequestTypeDef

```python
# DeleteRoomSkillParameterRequestRequestTypeDef definition

class DeleteRoomSkillParameterRequestRequestTypeDef(TypedDict):
    SkillId: str,
    ParameterKey: str,
    RoomArn: NotRequired[str],
```

## DeleteSkillAuthorizationRequestRequestTypeDef

```python
# DeleteSkillAuthorizationRequestRequestTypeDef definition

class DeleteSkillAuthorizationRequestRequestTypeDef(TypedDict):
    SkillId: str,
    RoomArn: NotRequired[str],
```

## DeleteSkillGroupRequestRequestTypeDef

```python
# DeleteSkillGroupRequestRequestTypeDef definition

class DeleteSkillGroupRequestRequestTypeDef(TypedDict):
    SkillGroupArn: NotRequired[str],
```

## DeleteUserRequestRequestTypeDef

```python
# DeleteUserRequestRequestTypeDef definition

class DeleteUserRequestRequestTypeDef(TypedDict):
    EnrollmentId: str,
    UserArn: NotRequired[str],
```

## DeveloperInfoTypeDef

```python
# DeveloperInfoTypeDef definition

class DeveloperInfoTypeDef(TypedDict):
    DeveloperName: NotRequired[str],
    PrivacyPolicy: NotRequired[str],
    Email: NotRequired[str],
    Url: NotRequired[str],
```

## DeviceEventTypeDef

```python
# DeviceEventTypeDef definition

class DeviceEventTypeDef(TypedDict):
    Type: NotRequired[DeviceEventTypeType],  # (1)
    Value: NotRequired[str],
    Timestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: DeviceEventTypeType](./literals.md#deviceeventtypetype) 
## DeviceNetworkProfileInfoTypeDef

```python
# DeviceNetworkProfileInfoTypeDef definition

class DeviceNetworkProfileInfoTypeDef(TypedDict):
    NetworkProfileArn: NotRequired[str],
    CertificateArn: NotRequired[str],
    CertificateExpirationTime: NotRequired[datetime],
```

## DeviceStatusDetailTypeDef

```python
# DeviceStatusDetailTypeDef definition

class DeviceStatusDetailTypeDef(TypedDict):
    Feature: NotRequired[FeatureType],  # (1)
    Code: NotRequired[DeviceStatusDetailCodeType],  # (2)
```

1. See [:material-code-brackets: FeatureType](./literals.md#featuretype) 
2. See [:material-code-brackets: DeviceStatusDetailCodeType](./literals.md#devicestatusdetailcodetype) 
## DisassociateContactFromAddressBookRequestRequestTypeDef

```python
# DisassociateContactFromAddressBookRequestRequestTypeDef definition

class DisassociateContactFromAddressBookRequestRequestTypeDef(TypedDict):
    ContactArn: str,
    AddressBookArn: str,
```

## DisassociateDeviceFromRoomRequestRequestTypeDef

```python
# DisassociateDeviceFromRoomRequestRequestTypeDef definition

class DisassociateDeviceFromRoomRequestRequestTypeDef(TypedDict):
    DeviceArn: NotRequired[str],
```

## DisassociateSkillFromSkillGroupRequestRequestTypeDef

```python
# DisassociateSkillFromSkillGroupRequestRequestTypeDef definition

class DisassociateSkillFromSkillGroupRequestRequestTypeDef(TypedDict):
    SkillId: str,
    SkillGroupArn: NotRequired[str],
```

## DisassociateSkillFromUsersRequestRequestTypeDef

```python
# DisassociateSkillFromUsersRequestRequestTypeDef definition

class DisassociateSkillFromUsersRequestRequestTypeDef(TypedDict):
    SkillId: str,
```

## DisassociateSkillGroupFromRoomRequestRequestTypeDef

```python
# DisassociateSkillGroupFromRoomRequestRequestTypeDef definition

class DisassociateSkillGroupFromRoomRequestRequestTypeDef(TypedDict):
    SkillGroupArn: NotRequired[str],
    RoomArn: NotRequired[str],
```

## EndOfMeetingReminderTypeDef

```python
# EndOfMeetingReminderTypeDef definition

class EndOfMeetingReminderTypeDef(TypedDict):
    ReminderAtMinutes: NotRequired[List[int]],
    ReminderType: NotRequired[EndOfMeetingReminderTypeType],  # (1)
    Enabled: NotRequired[bool],
```

1. See [:material-code-brackets: EndOfMeetingReminderTypeType](./literals.md#endofmeetingremindertypetype) 
## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Key: str,
    Values: Sequence[str],
```

## ForgetSmartHomeAppliancesRequestRequestTypeDef

```python
# ForgetSmartHomeAppliancesRequestRequestTypeDef definition

class ForgetSmartHomeAppliancesRequestRequestTypeDef(TypedDict):
    RoomArn: str,
```

## GatewayGroupSummaryTypeDef

```python
# GatewayGroupSummaryTypeDef definition

class GatewayGroupSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## GatewayGroupTypeDef

```python
# GatewayGroupTypeDef definition

class GatewayGroupTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## GatewaySummaryTypeDef

```python
# GatewaySummaryTypeDef definition

class GatewaySummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    GatewayGroupArn: NotRequired[str],
    SoftwareVersion: NotRequired[str],
```

## GatewayTypeDef

```python
# GatewayTypeDef definition

class GatewayTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    GatewayGroupArn: NotRequired[str],
    SoftwareVersion: NotRequired[str],
```

## GetAddressBookRequestRequestTypeDef

```python
# GetAddressBookRequestRequestTypeDef definition

class GetAddressBookRequestRequestTypeDef(TypedDict):
    AddressBookArn: str,
```

## GetConferenceProviderRequestRequestTypeDef

```python
# GetConferenceProviderRequestRequestTypeDef definition

class GetConferenceProviderRequestRequestTypeDef(TypedDict):
    ConferenceProviderArn: str,
```

## GetContactRequestRequestTypeDef

```python
# GetContactRequestRequestTypeDef definition

class GetContactRequestRequestTypeDef(TypedDict):
    ContactArn: str,
```

## GetDeviceRequestRequestTypeDef

```python
# GetDeviceRequestRequestTypeDef definition

class GetDeviceRequestRequestTypeDef(TypedDict):
    DeviceArn: NotRequired[str],
```

## GetGatewayGroupRequestRequestTypeDef

```python
# GetGatewayGroupRequestRequestTypeDef definition

class GetGatewayGroupRequestRequestTypeDef(TypedDict):
    GatewayGroupArn: str,
```

## GetGatewayRequestRequestTypeDef

```python
# GetGatewayRequestRequestTypeDef definition

class GetGatewayRequestRequestTypeDef(TypedDict):
    GatewayArn: str,
```

## GetNetworkProfileRequestRequestTypeDef

```python
# GetNetworkProfileRequestRequestTypeDef definition

class GetNetworkProfileRequestRequestTypeDef(TypedDict):
    NetworkProfileArn: str,
```

## NetworkProfileTypeDef

```python
# NetworkProfileTypeDef definition

class NetworkProfileTypeDef(TypedDict):
    NetworkProfileArn: NotRequired[str],
    NetworkProfileName: NotRequired[str],
    Description: NotRequired[str],
    Ssid: NotRequired[str],
    SecurityType: NotRequired[NetworkSecurityTypeType],  # (1)
    EapMethod: NotRequired[NetworkEapMethodType],  # (2)
    CurrentPassword: NotRequired[str],
    NextPassword: NotRequired[str],
    CertificateAuthorityArn: NotRequired[str],
    TrustAnchors: NotRequired[List[str]],
```

1. See [:material-code-brackets: NetworkSecurityTypeType](./literals.md#networksecuritytypetype) 
2. See [:material-code-brackets: NetworkEapMethodType](./literals.md#networkeapmethodtype) 
## GetProfileRequestRequestTypeDef

```python
# GetProfileRequestRequestTypeDef definition

class GetProfileRequestRequestTypeDef(TypedDict):
    ProfileArn: NotRequired[str],
```

## GetRoomRequestRequestTypeDef

```python
# GetRoomRequestRequestTypeDef definition

class GetRoomRequestRequestTypeDef(TypedDict):
    RoomArn: NotRequired[str],
```

## RoomTypeDef

```python
# RoomTypeDef definition

class RoomTypeDef(TypedDict):
    RoomArn: NotRequired[str],
    RoomName: NotRequired[str],
    Description: NotRequired[str],
    ProviderCalendarId: NotRequired[str],
    ProfileArn: NotRequired[str],
```

## GetRoomSkillParameterRequestRequestTypeDef

```python
# GetRoomSkillParameterRequestRequestTypeDef definition

class GetRoomSkillParameterRequestRequestTypeDef(TypedDict):
    SkillId: str,
    ParameterKey: str,
    RoomArn: NotRequired[str],
```

## RoomSkillParameterTypeDef

```python
# RoomSkillParameterTypeDef definition

class RoomSkillParameterTypeDef(TypedDict):
    ParameterKey: str,
    ParameterValue: str,
```

## GetSkillGroupRequestRequestTypeDef

```python
# GetSkillGroupRequestRequestTypeDef definition

class GetSkillGroupRequestRequestTypeDef(TypedDict):
    SkillGroupArn: NotRequired[str],
```

## SkillGroupTypeDef

```python
# SkillGroupTypeDef definition

class SkillGroupTypeDef(TypedDict):
    SkillGroupArn: NotRequired[str],
    SkillGroupName: NotRequired[str],
    Description: NotRequired[str],
```

## InstantBookingTypeDef

```python
# InstantBookingTypeDef definition

class InstantBookingTypeDef(TypedDict):
    DurationInMinutes: NotRequired[int],
    Enabled: NotRequired[bool],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListBusinessReportSchedulesRequestRequestTypeDef

```python
# ListBusinessReportSchedulesRequestRequestTypeDef definition

class ListBusinessReportSchedulesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListConferenceProvidersRequestRequestTypeDef

```python
# ListConferenceProvidersRequestRequestTypeDef definition

class ListConferenceProvidersRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListDeviceEventsRequestRequestTypeDef

```python
# ListDeviceEventsRequestRequestTypeDef definition

class ListDeviceEventsRequestRequestTypeDef(TypedDict):
    DeviceArn: str,
    EventType: NotRequired[DeviceEventTypeType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: DeviceEventTypeType](./literals.md#deviceeventtypetype) 
## ListGatewayGroupsRequestRequestTypeDef

```python
# ListGatewayGroupsRequestRequestTypeDef definition

class ListGatewayGroupsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListGatewaysRequestRequestTypeDef

```python
# ListGatewaysRequestRequestTypeDef definition

class ListGatewaysRequestRequestTypeDef(TypedDict):
    GatewayGroupArn: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListSkillsRequestRequestTypeDef

```python
# ListSkillsRequestRequestTypeDef definition

class ListSkillsRequestRequestTypeDef(TypedDict):
    SkillGroupArn: NotRequired[str],
    EnablementType: NotRequired[EnablementTypeFilterType],  # (1)
    SkillType: NotRequired[SkillTypeFilterType],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: EnablementTypeFilterType](./literals.md#enablementtypefiltertype) 
2. See [:material-code-brackets: SkillTypeFilterType](./literals.md#skilltypefiltertype) 
## SkillSummaryTypeDef

```python
# SkillSummaryTypeDef definition

class SkillSummaryTypeDef(TypedDict):
    SkillId: NotRequired[str],
    SkillName: NotRequired[str],
    SupportsLinking: NotRequired[bool],
    EnablementType: NotRequired[EnablementTypeType],  # (1)
    SkillType: NotRequired[SkillTypeType],  # (2)
```

1. See [:material-code-brackets: EnablementTypeType](./literals.md#enablementtypetype) 
2. See [:material-code-brackets: SkillTypeType](./literals.md#skilltypetype) 
## ListSkillsStoreCategoriesRequestRequestTypeDef

```python
# ListSkillsStoreCategoriesRequestRequestTypeDef definition

class ListSkillsStoreCategoriesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListSkillsStoreSkillsByCategoryRequestRequestTypeDef

```python
# ListSkillsStoreSkillsByCategoryRequestRequestTypeDef definition

class ListSkillsStoreSkillsByCategoryRequestRequestTypeDef(TypedDict):
    CategoryId: int,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListSmartHomeAppliancesRequestRequestTypeDef

```python
# ListSmartHomeAppliancesRequestRequestTypeDef definition

class ListSmartHomeAppliancesRequestRequestTypeDef(TypedDict):
    RoomArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## SmartHomeApplianceTypeDef

```python
# SmartHomeApplianceTypeDef definition

class SmartHomeApplianceTypeDef(TypedDict):
    FriendlyName: NotRequired[str],
    Description: NotRequired[str],
    ManufacturerName: NotRequired[str],
```

## ListTagsRequestRequestTypeDef

```python
# ListTagsRequestRequestTypeDef definition

class ListTagsRequestRequestTypeDef(TypedDict):
    Arn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ProactiveJoinTypeDef

```python
# ProactiveJoinTypeDef definition

class ProactiveJoinTypeDef(TypedDict):
    EnabledByMotion: NotRequired[bool],
```

## RequireCheckInTypeDef

```python
# RequireCheckInTypeDef definition

class RequireCheckInTypeDef(TypedDict):
    ReleaseAfterMinutes: NotRequired[int],
    Enabled: NotRequired[bool],
```

## NetworkProfileDataTypeDef

```python
# NetworkProfileDataTypeDef definition

class NetworkProfileDataTypeDef(TypedDict):
    NetworkProfileArn: NotRequired[str],
    NetworkProfileName: NotRequired[str],
    Description: NotRequired[str],
    Ssid: NotRequired[str],
    SecurityType: NotRequired[NetworkSecurityTypeType],  # (1)
    EapMethod: NotRequired[NetworkEapMethodType],  # (2)
    CertificateAuthorityArn: NotRequired[str],
```

1. See [:material-code-brackets: NetworkSecurityTypeType](./literals.md#networksecuritytypetype) 
2. See [:material-code-brackets: NetworkEapMethodType](./literals.md#networkeapmethodtype) 
## ProfileDataTypeDef

```python
# ProfileDataTypeDef definition

class ProfileDataTypeDef(TypedDict):
    ProfileArn: NotRequired[str],
    ProfileName: NotRequired[str],
    IsDefault: NotRequired[bool],
    Address: NotRequired[str],
    Timezone: NotRequired[str],
    DistanceUnit: NotRequired[DistanceUnitType],  # (1)
    TemperatureUnit: NotRequired[TemperatureUnitType],  # (2)
    WakeWord: NotRequired[WakeWordType],  # (3)
    Locale: NotRequired[str],
```

1. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
2. See [:material-code-brackets: TemperatureUnitType](./literals.md#temperatureunittype) 
3. See [:material-code-brackets: WakeWordType](./literals.md#wakewordtype) 
## PutInvitationConfigurationRequestRequestTypeDef

```python
# PutInvitationConfigurationRequestRequestTypeDef definition

class PutInvitationConfigurationRequestRequestTypeDef(TypedDict):
    OrganizationName: str,
    ContactEmail: NotRequired[str],
    PrivateSkillIds: NotRequired[Sequence[str]],
```

## PutSkillAuthorizationRequestRequestTypeDef

```python
# PutSkillAuthorizationRequestRequestTypeDef definition

class PutSkillAuthorizationRequestRequestTypeDef(TypedDict):
    AuthorizationResult: Mapping[str, str],
    SkillId: str,
    RoomArn: NotRequired[str],
```

## RejectSkillRequestRequestTypeDef

```python
# RejectSkillRequestRequestTypeDef definition

class RejectSkillRequestRequestTypeDef(TypedDict):
    SkillId: str,
```

## ResolveRoomRequestRequestTypeDef

```python
# ResolveRoomRequestRequestTypeDef definition

class ResolveRoomRequestRequestTypeDef(TypedDict):
    UserId: str,
    SkillId: str,
```

## RevokeInvitationRequestRequestTypeDef

```python
# RevokeInvitationRequestRequestTypeDef definition

class RevokeInvitationRequestRequestTypeDef(TypedDict):
    UserArn: NotRequired[str],
    EnrollmentId: NotRequired[str],
```

## RoomDataTypeDef

```python
# RoomDataTypeDef definition

class RoomDataTypeDef(TypedDict):
    RoomArn: NotRequired[str],
    RoomName: NotRequired[str],
    Description: NotRequired[str],
    ProviderCalendarId: NotRequired[str],
    ProfileArn: NotRequired[str],
    ProfileName: NotRequired[str],
```

## SortTypeDef

```python
# SortTypeDef definition

class SortTypeDef(TypedDict):
    Key: str,
    Value: SortValueType,  # (1)
```

1. See [:material-code-brackets: SortValueType](./literals.md#sortvaluetype) 
## SkillGroupDataTypeDef

```python
# SkillGroupDataTypeDef definition

class SkillGroupDataTypeDef(TypedDict):
    SkillGroupArn: NotRequired[str],
    SkillGroupName: NotRequired[str],
    Description: NotRequired[str],
```

## UserDataTypeDef

```python
# UserDataTypeDef definition

class UserDataTypeDef(TypedDict):
    UserArn: NotRequired[str],
    FirstName: NotRequired[str],
    LastName: NotRequired[str],
    Email: NotRequired[str],
    EnrollmentStatus: NotRequired[EnrollmentStatusType],  # (1)
    EnrollmentId: NotRequired[str],
```

1. See [:material-code-brackets: EnrollmentStatusType](./literals.md#enrollmentstatustype) 
## SendInvitationRequestRequestTypeDef

```python
# SendInvitationRequestRequestTypeDef definition

class SendInvitationRequestRequestTypeDef(TypedDict):
    UserArn: NotRequired[str],
```

## StartDeviceSyncRequestRequestTypeDef

```python
# StartDeviceSyncRequestRequestTypeDef definition

class StartDeviceSyncRequestRequestTypeDef(TypedDict):
    Features: Sequence[FeatureType],  # (1)
    RoomArn: NotRequired[str],
    DeviceArn: NotRequired[str],
```

1. See [:material-code-brackets: FeatureType](./literals.md#featuretype) 
## StartSmartHomeApplianceDiscoveryRequestRequestTypeDef

```python
# StartSmartHomeApplianceDiscoveryRequestRequestTypeDef definition

class StartSmartHomeApplianceDiscoveryRequestRequestTypeDef(TypedDict):
    RoomArn: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    Arn: str,
    TagKeys: Sequence[str],
```

## UpdateAddressBookRequestRequestTypeDef

```python
# UpdateAddressBookRequestRequestTypeDef definition

class UpdateAddressBookRequestRequestTypeDef(TypedDict):
    AddressBookArn: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## UpdateDeviceRequestRequestTypeDef

```python
# UpdateDeviceRequestRequestTypeDef definition

class UpdateDeviceRequestRequestTypeDef(TypedDict):
    DeviceArn: NotRequired[str],
    DeviceName: NotRequired[str],
```

## UpdateEndOfMeetingReminderTypeDef

```python
# UpdateEndOfMeetingReminderTypeDef definition

class UpdateEndOfMeetingReminderTypeDef(TypedDict):
    ReminderAtMinutes: NotRequired[Sequence[int]],
    ReminderType: NotRequired[EndOfMeetingReminderTypeType],  # (1)
    Enabled: NotRequired[bool],
```

1. See [:material-code-brackets: EndOfMeetingReminderTypeType](./literals.md#endofmeetingremindertypetype) 
## UpdateGatewayGroupRequestRequestTypeDef

```python
# UpdateGatewayGroupRequestRequestTypeDef definition

class UpdateGatewayGroupRequestRequestTypeDef(TypedDict):
    GatewayGroupArn: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## UpdateGatewayRequestRequestTypeDef

```python
# UpdateGatewayRequestRequestTypeDef definition

class UpdateGatewayRequestRequestTypeDef(TypedDict):
    GatewayArn: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    SoftwareVersion: NotRequired[str],
```

## UpdateInstantBookingTypeDef

```python
# UpdateInstantBookingTypeDef definition

class UpdateInstantBookingTypeDef(TypedDict):
    DurationInMinutes: NotRequired[int],
    Enabled: NotRequired[bool],
```

## UpdateProactiveJoinTypeDef

```python
# UpdateProactiveJoinTypeDef definition

class UpdateProactiveJoinTypeDef(TypedDict):
    EnabledByMotion: bool,
```

## UpdateRequireCheckInTypeDef

```python
# UpdateRequireCheckInTypeDef definition

class UpdateRequireCheckInTypeDef(TypedDict):
    ReleaseAfterMinutes: NotRequired[int],
    Enabled: NotRequired[bool],
```

## UpdateNetworkProfileRequestRequestTypeDef

```python
# UpdateNetworkProfileRequestRequestTypeDef definition

class UpdateNetworkProfileRequestRequestTypeDef(TypedDict):
    NetworkProfileArn: str,
    NetworkProfileName: NotRequired[str],
    Description: NotRequired[str],
    CurrentPassword: NotRequired[str],
    NextPassword: NotRequired[str],
    CertificateAuthorityArn: NotRequired[str],
    TrustAnchors: NotRequired[Sequence[str]],
```

## UpdateRoomRequestRequestTypeDef

```python
# UpdateRoomRequestRequestTypeDef definition

class UpdateRoomRequestRequestTypeDef(TypedDict):
    RoomArn: NotRequired[str],
    RoomName: NotRequired[str],
    Description: NotRequired[str],
    ProviderCalendarId: NotRequired[str],
    ProfileArn: NotRequired[str],
```

## UpdateSkillGroupRequestRequestTypeDef

```python
# UpdateSkillGroupRequestRequestTypeDef definition

class UpdateSkillGroupRequestRequestTypeDef(TypedDict):
    SkillGroupArn: NotRequired[str],
    SkillGroupName: NotRequired[str],
    Description: NotRequired[str],
```

## UpdateBusinessReportScheduleRequestRequestTypeDef

```python
# UpdateBusinessReportScheduleRequestRequestTypeDef definition

class UpdateBusinessReportScheduleRequestRequestTypeDef(TypedDict):
    ScheduleArn: str,
    S3BucketName: NotRequired[str],
    S3KeyPrefix: NotRequired[str],
    Format: NotRequired[BusinessReportFormatType],  # (1)
    ScheduleName: NotRequired[str],
    Recurrence: NotRequired[BusinessReportRecurrenceTypeDef],  # (2)
```

1. See [:material-code-brackets: BusinessReportFormatType](./literals.md#businessreportformattype) 
2. See [:material-code-braces: BusinessReportRecurrenceTypeDef](./type_defs.md#businessreportrecurrencetypedef) 
## BusinessReportTypeDef

```python
# BusinessReportTypeDef definition

class BusinessReportTypeDef(TypedDict):
    Status: NotRequired[BusinessReportStatusType],  # (1)
    FailureCode: NotRequired[BusinessReportFailureCodeType],  # (2)
    S3Location: NotRequired[BusinessReportS3LocationTypeDef],  # (3)
    DeliveryTime: NotRequired[datetime],
    DownloadUrl: NotRequired[str],
```

1. See [:material-code-brackets: BusinessReportStatusType](./literals.md#businessreportstatustype) 
2. See [:material-code-brackets: BusinessReportFailureCodeType](./literals.md#businessreportfailurecodetype) 
3. See [:material-code-braces: BusinessReportS3LocationTypeDef](./type_defs.md#businessreports3locationtypedef) 
## PutConferencePreferenceRequestRequestTypeDef

```python
# PutConferencePreferenceRequestRequestTypeDef definition

class PutConferencePreferenceRequestRequestTypeDef(TypedDict):
    ConferencePreference: ConferencePreferenceTypeDef,  # (1)
```

1. See [:material-code-braces: ConferencePreferenceTypeDef](./type_defs.md#conferencepreferencetypedef) 
## ConferenceProviderTypeDef

```python
# ConferenceProviderTypeDef definition

class ConferenceProviderTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Type: NotRequired[ConferenceProviderTypeType],  # (1)
    IPDialIn: NotRequired[IPDialInTypeDef],  # (2)
    PSTNDialIn: NotRequired[PSTNDialInTypeDef],  # (3)
    MeetingSetting: NotRequired[MeetingSettingTypeDef],  # (4)
```

1. See [:material-code-brackets: ConferenceProviderTypeType](./literals.md#conferenceprovidertypetype) 
2. See [:material-code-braces: IPDialInTypeDef](./type_defs.md#ipdialintypedef) 
3. See [:material-code-braces: PSTNDialInTypeDef](./type_defs.md#pstndialintypedef) 
4. See [:material-code-braces: MeetingSettingTypeDef](./type_defs.md#meetingsettingtypedef) 
## UpdateConferenceProviderRequestRequestTypeDef

```python
# UpdateConferenceProviderRequestRequestTypeDef definition

class UpdateConferenceProviderRequestRequestTypeDef(TypedDict):
    ConferenceProviderArn: str,
    ConferenceProviderType: ConferenceProviderTypeType,  # (1)
    MeetingSetting: MeetingSettingTypeDef,  # (2)
    IPDialIn: NotRequired[IPDialInTypeDef],  # (3)
    PSTNDialIn: NotRequired[PSTNDialInTypeDef],  # (4)
```

1. See [:material-code-brackets: ConferenceProviderTypeType](./literals.md#conferenceprovidertypetype) 
2. See [:material-code-braces: MeetingSettingTypeDef](./type_defs.md#meetingsettingtypedef) 
3. See [:material-code-braces: IPDialInTypeDef](./type_defs.md#ipdialintypedef) 
4. See [:material-code-braces: PSTNDialInTypeDef](./type_defs.md#pstndialintypedef) 
## ContactDataTypeDef

```python
# ContactDataTypeDef definition

class ContactDataTypeDef(TypedDict):
    ContactArn: NotRequired[str],
    DisplayName: NotRequired[str],
    FirstName: NotRequired[str],
    LastName: NotRequired[str],
    PhoneNumber: NotRequired[str],
    PhoneNumbers: NotRequired[List[PhoneNumberTypeDef]],  # (1)
    SipAddresses: NotRequired[List[SipAddressTypeDef]],  # (2)
```

1. See [:material-code-braces: PhoneNumberTypeDef](./type_defs.md#phonenumbertypedef) 
2. See [:material-code-braces: SipAddressTypeDef](./type_defs.md#sipaddresstypedef) 
## ContactTypeDef

```python
# ContactTypeDef definition

class ContactTypeDef(TypedDict):
    ContactArn: NotRequired[str],
    DisplayName: NotRequired[str],
    FirstName: NotRequired[str],
    LastName: NotRequired[str],
    PhoneNumber: NotRequired[str],
    PhoneNumbers: NotRequired[List[PhoneNumberTypeDef]],  # (1)
    SipAddresses: NotRequired[List[SipAddressTypeDef]],  # (2)
```

1. See [:material-code-braces: PhoneNumberTypeDef](./type_defs.md#phonenumbertypedef) 
2. See [:material-code-braces: SipAddressTypeDef](./type_defs.md#sipaddresstypedef) 
## UpdateContactRequestRequestTypeDef

```python
# UpdateContactRequestRequestTypeDef definition

class UpdateContactRequestRequestTypeDef(TypedDict):
    ContactArn: str,
    DisplayName: NotRequired[str],
    FirstName: NotRequired[str],
    LastName: NotRequired[str],
    PhoneNumber: NotRequired[str],
    PhoneNumbers: NotRequired[Sequence[PhoneNumberTypeDef]],  # (1)
    SipAddresses: NotRequired[Sequence[SipAddressTypeDef]],  # (2)
```

1. See [:material-code-braces: PhoneNumberTypeDef](./type_defs.md#phonenumbertypedef) 
2. See [:material-code-braces: SipAddressTypeDef](./type_defs.md#sipaddresstypedef) 
## ContentTypeDef

```python
# ContentTypeDef definition

class ContentTypeDef(TypedDict):
    TextList: NotRequired[Sequence[TextTypeDef]],  # (1)
    SsmlList: NotRequired[Sequence[SsmlTypeDef]],  # (2)
    AudioList: NotRequired[Sequence[AudioTypeDef]],  # (3)
```

1. See [:material-code-braces: TextTypeDef](./type_defs.md#texttypedef) 
2. See [:material-code-braces: SsmlTypeDef](./type_defs.md#ssmltypedef) 
3. See [:material-code-braces: AudioTypeDef](./type_defs.md#audiotypedef) 
## CreateAddressBookRequestRequestTypeDef

```python
# CreateAddressBookRequestRequestTypeDef definition

class CreateAddressBookRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateBusinessReportScheduleRequestRequestTypeDef

```python
# CreateBusinessReportScheduleRequestRequestTypeDef definition

class CreateBusinessReportScheduleRequestRequestTypeDef(TypedDict):
    Format: BusinessReportFormatType,  # (1)
    ContentRange: BusinessReportContentRangeTypeDef,  # (2)
    ScheduleName: NotRequired[str],
    S3BucketName: NotRequired[str],
    S3KeyPrefix: NotRequired[str],
    Recurrence: NotRequired[BusinessReportRecurrenceTypeDef],  # (3)
    ClientRequestToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-brackets: BusinessReportFormatType](./literals.md#businessreportformattype) 
2. See [:material-code-braces: BusinessReportContentRangeTypeDef](./type_defs.md#businessreportcontentrangetypedef) 
3. See [:material-code-braces: BusinessReportRecurrenceTypeDef](./type_defs.md#businessreportrecurrencetypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateConferenceProviderRequestRequestTypeDef

```python
# CreateConferenceProviderRequestRequestTypeDef definition

class CreateConferenceProviderRequestRequestTypeDef(TypedDict):
    ConferenceProviderName: str,
    ConferenceProviderType: ConferenceProviderTypeType,  # (1)
    MeetingSetting: MeetingSettingTypeDef,  # (2)
    IPDialIn: NotRequired[IPDialInTypeDef],  # (3)
    PSTNDialIn: NotRequired[PSTNDialInTypeDef],  # (4)
    ClientRequestToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (5)
```

1. See [:material-code-brackets: ConferenceProviderTypeType](./literals.md#conferenceprovidertypetype) 
2. See [:material-code-braces: MeetingSettingTypeDef](./type_defs.md#meetingsettingtypedef) 
3. See [:material-code-braces: IPDialInTypeDef](./type_defs.md#ipdialintypedef) 
4. See [:material-code-braces: PSTNDialInTypeDef](./type_defs.md#pstndialintypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateContactRequestRequestTypeDef

```python
# CreateContactRequestRequestTypeDef definition

class CreateContactRequestRequestTypeDef(TypedDict):
    FirstName: str,
    DisplayName: NotRequired[str],
    LastName: NotRequired[str],
    PhoneNumber: NotRequired[str],
    PhoneNumbers: NotRequired[Sequence[PhoneNumberTypeDef]],  # (1)
    SipAddresses: NotRequired[Sequence[SipAddressTypeDef]],  # (2)
    ClientRequestToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: PhoneNumberTypeDef](./type_defs.md#phonenumbertypedef) 
2. See [:material-code-braces: SipAddressTypeDef](./type_defs.md#sipaddresstypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateGatewayGroupRequestRequestTypeDef

```python
# CreateGatewayGroupRequestRequestTypeDef definition

class CreateGatewayGroupRequestRequestTypeDef(TypedDict):
    Name: str,
    ClientRequestToken: str,
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateNetworkProfileRequestRequestTypeDef

```python
# CreateNetworkProfileRequestRequestTypeDef definition

class CreateNetworkProfileRequestRequestTypeDef(TypedDict):
    NetworkProfileName: str,
    Ssid: str,
    SecurityType: NetworkSecurityTypeType,  # (1)
    ClientRequestToken: str,
    Description: NotRequired[str],
    EapMethod: NotRequired[NetworkEapMethodType],  # (2)
    CurrentPassword: NotRequired[str],
    NextPassword: NotRequired[str],
    CertificateAuthorityArn: NotRequired[str],
    TrustAnchors: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: NetworkSecurityTypeType](./literals.md#networksecuritytypetype) 
2. See [:material-code-brackets: NetworkEapMethodType](./literals.md#networkeapmethodtype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateRoomRequestRequestTypeDef

```python
# CreateRoomRequestRequestTypeDef definition

class CreateRoomRequestRequestTypeDef(TypedDict):
    RoomName: str,
    Description: NotRequired[str],
    ProfileArn: NotRequired[str],
    ProviderCalendarId: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateSkillGroupRequestRequestTypeDef

```python
# CreateSkillGroupRequestRequestTypeDef definition

class CreateSkillGroupRequestRequestTypeDef(TypedDict):
    SkillGroupName: str,
    Description: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateUserRequestRequestTypeDef

```python
# CreateUserRequestRequestTypeDef definition

class CreateUserRequestRequestTypeDef(TypedDict):
    UserId: str,
    FirstName: NotRequired[str],
    LastName: NotRequired[str],
    Email: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## RegisterAVSDeviceRequestRequestTypeDef

```python
# RegisterAVSDeviceRequestRequestTypeDef definition

class RegisterAVSDeviceRequestRequestTypeDef(TypedDict):
    ClientId: str,
    UserCode: str,
    ProductId: str,
    AmazonId: str,
    DeviceSerialNumber: NotRequired[str],
    RoomArn: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    Arn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateAddressBookResponseTypeDef

```python
# CreateAddressBookResponseTypeDef definition

class CreateAddressBookResponseTypeDef(TypedDict):
    AddressBookArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBusinessReportScheduleResponseTypeDef

```python
# CreateBusinessReportScheduleResponseTypeDef definition

class CreateBusinessReportScheduleResponseTypeDef(TypedDict):
    ScheduleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConferenceProviderResponseTypeDef

```python
# CreateConferenceProviderResponseTypeDef definition

class CreateConferenceProviderResponseTypeDef(TypedDict):
    ConferenceProviderArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateContactResponseTypeDef

```python
# CreateContactResponseTypeDef definition

class CreateContactResponseTypeDef(TypedDict):
    ContactArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGatewayGroupResponseTypeDef

```python
# CreateGatewayGroupResponseTypeDef definition

class CreateGatewayGroupResponseTypeDef(TypedDict):
    GatewayGroupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateNetworkProfileResponseTypeDef

```python
# CreateNetworkProfileResponseTypeDef definition

class CreateNetworkProfileResponseTypeDef(TypedDict):
    NetworkProfileArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProfileResponseTypeDef

```python
# CreateProfileResponseTypeDef definition

class CreateProfileResponseTypeDef(TypedDict):
    ProfileArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRoomResponseTypeDef

```python
# CreateRoomResponseTypeDef definition

class CreateRoomResponseTypeDef(TypedDict):
    RoomArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSkillGroupResponseTypeDef

```python
# CreateSkillGroupResponseTypeDef definition

class CreateSkillGroupResponseTypeDef(TypedDict):
    SkillGroupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserResponseTypeDef

```python
# CreateUserResponseTypeDef definition

class CreateUserResponseTypeDef(TypedDict):
    UserArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAddressBookResponseTypeDef

```python
# GetAddressBookResponseTypeDef definition

class GetAddressBookResponseTypeDef(TypedDict):
    AddressBook: AddressBookTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AddressBookTypeDef](./type_defs.md#addressbooktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConferencePreferenceResponseTypeDef

```python
# GetConferencePreferenceResponseTypeDef definition

class GetConferencePreferenceResponseTypeDef(TypedDict):
    Preference: ConferencePreferenceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConferencePreferenceTypeDef](./type_defs.md#conferencepreferencetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInvitationConfigurationResponseTypeDef

```python
# GetInvitationConfigurationResponseTypeDef definition

class GetInvitationConfigurationResponseTypeDef(TypedDict):
    OrganizationName: str,
    ContactEmail: str,
    PrivateSkillIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSkillsStoreCategoriesResponseTypeDef

```python
# ListSkillsStoreCategoriesResponseTypeDef definition

class ListSkillsStoreCategoriesResponseTypeDef(TypedDict):
    CategoryList: List[CategoryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CategoryTypeDef](./type_defs.md#categorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsResponseTypeDef

```python
# ListTagsResponseTypeDef definition

class ListTagsResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterAVSDeviceResponseTypeDef

```python
# RegisterAVSDeviceResponseTypeDef definition

class RegisterAVSDeviceResponseTypeDef(TypedDict):
    DeviceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchAddressBooksResponseTypeDef

```python
# SearchAddressBooksResponseTypeDef definition

class SearchAddressBooksResponseTypeDef(TypedDict):
    AddressBooks: List[AddressBookDataTypeDef],  # (1)
    NextToken: str,
    TotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AddressBookDataTypeDef](./type_defs.md#addressbookdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendAnnouncementResponseTypeDef

```python
# SendAnnouncementResponseTypeDef definition

class SendAnnouncementResponseTypeDef(TypedDict):
    AnnouncementArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMeetingRoomConfigurationTypeDef

```python
# CreateMeetingRoomConfigurationTypeDef definition

class CreateMeetingRoomConfigurationTypeDef(TypedDict):
    RoomUtilizationMetricsEnabled: NotRequired[bool],
    EndOfMeetingReminder: NotRequired[CreateEndOfMeetingReminderTypeDef],  # (1)
    InstantBooking: NotRequired[CreateInstantBookingTypeDef],  # (2)
    RequireCheckIn: NotRequired[CreateRequireCheckInTypeDef],  # (3)
    ProactiveJoin: NotRequired[CreateProactiveJoinTypeDef],  # (4)
```

1. See [:material-code-braces: CreateEndOfMeetingReminderTypeDef](./type_defs.md#createendofmeetingremindertypedef) 
2. See [:material-code-braces: CreateInstantBookingTypeDef](./type_defs.md#createinstantbookingtypedef) 
3. See [:material-code-braces: CreateRequireCheckInTypeDef](./type_defs.md#createrequirecheckintypedef) 
4. See [:material-code-braces: CreateProactiveJoinTypeDef](./type_defs.md#createproactivejointypedef) 
## SkillDetailsTypeDef

```python
# SkillDetailsTypeDef definition

class SkillDetailsTypeDef(TypedDict):
    ProductDescription: NotRequired[str],
    InvocationPhrase: NotRequired[str],
    ReleaseDate: NotRequired[str],
    EndUserLicenseAgreement: NotRequired[str],
    GenericKeywords: NotRequired[List[str]],
    BulletPoints: NotRequired[List[str]],
    NewInThisVersionBulletPoints: NotRequired[List[str]],
    SkillTypes: NotRequired[List[str]],
    Reviews: NotRequired[Dict[str, str]],
    DeveloperInfo: NotRequired[DeveloperInfoTypeDef],  # (1)
```

1. See [:material-code-braces: DeveloperInfoTypeDef](./type_defs.md#developerinfotypedef) 
## ListDeviceEventsResponseTypeDef

```python
# ListDeviceEventsResponseTypeDef definition

class ListDeviceEventsResponseTypeDef(TypedDict):
    DeviceEvents: List[DeviceEventTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeviceEventTypeDef](./type_defs.md#deviceeventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeviceStatusInfoTypeDef

```python
# DeviceStatusInfoTypeDef definition

class DeviceStatusInfoTypeDef(TypedDict):
    DeviceStatusDetails: NotRequired[List[DeviceStatusDetailTypeDef]],  # (1)
    ConnectionStatus: NotRequired[ConnectionStatusType],  # (2)
    ConnectionStatusUpdatedTime: NotRequired[datetime],
```

1. See [:material-code-braces: DeviceStatusDetailTypeDef](./type_defs.md#devicestatusdetailtypedef) 
2. See [:material-code-brackets: ConnectionStatusType](./literals.md#connectionstatustype) 
## ListGatewayGroupsResponseTypeDef

```python
# ListGatewayGroupsResponseTypeDef definition

class ListGatewayGroupsResponseTypeDef(TypedDict):
    GatewayGroups: List[GatewayGroupSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GatewayGroupSummaryTypeDef](./type_defs.md#gatewaygroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGatewayGroupResponseTypeDef

```python
# GetGatewayGroupResponseTypeDef definition

class GetGatewayGroupResponseTypeDef(TypedDict):
    GatewayGroup: GatewayGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GatewayGroupTypeDef](./type_defs.md#gatewaygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGatewaysResponseTypeDef

```python
# ListGatewaysResponseTypeDef definition

class ListGatewaysResponseTypeDef(TypedDict):
    Gateways: List[GatewaySummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GatewaySummaryTypeDef](./type_defs.md#gatewaysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGatewayResponseTypeDef

```python
# GetGatewayResponseTypeDef definition

class GetGatewayResponseTypeDef(TypedDict):
    Gateway: GatewayTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GatewayTypeDef](./type_defs.md#gatewaytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetNetworkProfileResponseTypeDef

```python
# GetNetworkProfileResponseTypeDef definition

class GetNetworkProfileResponseTypeDef(TypedDict):
    NetworkProfile: NetworkProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkProfileTypeDef](./type_defs.md#networkprofiletypedef) 
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
## GetRoomSkillParameterResponseTypeDef

```python
# GetRoomSkillParameterResponseTypeDef definition

class GetRoomSkillParameterResponseTypeDef(TypedDict):
    RoomSkillParameter: RoomSkillParameterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoomSkillParameterTypeDef](./type_defs.md#roomskillparametertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRoomSkillParameterRequestRequestTypeDef

```python
# PutRoomSkillParameterRequestRequestTypeDef definition

class PutRoomSkillParameterRequestRequestTypeDef(TypedDict):
    SkillId: str,
    RoomSkillParameter: RoomSkillParameterTypeDef,  # (1)
    RoomArn: NotRequired[str],
```

1. See [:material-code-braces: RoomSkillParameterTypeDef](./type_defs.md#roomskillparametertypedef) 
## ResolveRoomResponseTypeDef

```python
# ResolveRoomResponseTypeDef definition

class ResolveRoomResponseTypeDef(TypedDict):
    RoomArn: str,
    RoomName: str,
    RoomSkillParameters: List[RoomSkillParameterTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoomSkillParameterTypeDef](./type_defs.md#roomskillparametertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSkillGroupResponseTypeDef

```python
# GetSkillGroupResponseTypeDef definition

class GetSkillGroupResponseTypeDef(TypedDict):
    SkillGroup: SkillGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SkillGroupTypeDef](./type_defs.md#skillgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBusinessReportSchedulesRequestListBusinessReportSchedulesPaginateTypeDef

```python
# ListBusinessReportSchedulesRequestListBusinessReportSchedulesPaginateTypeDef definition

class ListBusinessReportSchedulesRequestListBusinessReportSchedulesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConferenceProvidersRequestListConferenceProvidersPaginateTypeDef

```python
# ListConferenceProvidersRequestListConferenceProvidersPaginateTypeDef definition

class ListConferenceProvidersRequestListConferenceProvidersPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDeviceEventsRequestListDeviceEventsPaginateTypeDef

```python
# ListDeviceEventsRequestListDeviceEventsPaginateTypeDef definition

class ListDeviceEventsRequestListDeviceEventsPaginateTypeDef(TypedDict):
    DeviceArn: str,
    EventType: NotRequired[DeviceEventTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DeviceEventTypeType](./literals.md#deviceeventtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSkillsRequestListSkillsPaginateTypeDef

```python
# ListSkillsRequestListSkillsPaginateTypeDef definition

class ListSkillsRequestListSkillsPaginateTypeDef(TypedDict):
    SkillGroupArn: NotRequired[str],
    EnablementType: NotRequired[EnablementTypeFilterType],  # (1)
    SkillType: NotRequired[SkillTypeFilterType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: EnablementTypeFilterType](./literals.md#enablementtypefiltertype) 
2. See [:material-code-brackets: SkillTypeFilterType](./literals.md#skilltypefiltertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSkillsStoreCategoriesRequestListSkillsStoreCategoriesPaginateTypeDef

```python
# ListSkillsStoreCategoriesRequestListSkillsStoreCategoriesPaginateTypeDef definition

class ListSkillsStoreCategoriesRequestListSkillsStoreCategoriesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSkillsStoreSkillsByCategoryRequestListSkillsStoreSkillsByCategoryPaginateTypeDef

```python
# ListSkillsStoreSkillsByCategoryRequestListSkillsStoreSkillsByCategoryPaginateTypeDef definition

class ListSkillsStoreSkillsByCategoryRequestListSkillsStoreSkillsByCategoryPaginateTypeDef(TypedDict):
    CategoryId: int,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSmartHomeAppliancesRequestListSmartHomeAppliancesPaginateTypeDef

```python
# ListSmartHomeAppliancesRequestListSmartHomeAppliancesPaginateTypeDef definition

class ListSmartHomeAppliancesRequestListSmartHomeAppliancesPaginateTypeDef(TypedDict):
    RoomArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsRequestListTagsPaginateTypeDef

```python
# ListTagsRequestListTagsPaginateTypeDef definition

class ListTagsRequestListTagsPaginateTypeDef(TypedDict):
    Arn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSkillsResponseTypeDef

```python
# ListSkillsResponseTypeDef definition

class ListSkillsResponseTypeDef(TypedDict):
    SkillSummaries: List[SkillSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SkillSummaryTypeDef](./type_defs.md#skillsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSmartHomeAppliancesResponseTypeDef

```python
# ListSmartHomeAppliancesResponseTypeDef definition

class ListSmartHomeAppliancesResponseTypeDef(TypedDict):
    SmartHomeAppliances: List[SmartHomeApplianceTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SmartHomeApplianceTypeDef](./type_defs.md#smarthomeappliancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MeetingRoomConfigurationTypeDef

```python
# MeetingRoomConfigurationTypeDef definition

class MeetingRoomConfigurationTypeDef(TypedDict):
    RoomUtilizationMetricsEnabled: NotRequired[bool],
    EndOfMeetingReminder: NotRequired[EndOfMeetingReminderTypeDef],  # (1)
    InstantBooking: NotRequired[InstantBookingTypeDef],  # (2)
    RequireCheckIn: NotRequired[RequireCheckInTypeDef],  # (3)
    ProactiveJoin: NotRequired[ProactiveJoinTypeDef],  # (4)
```

1. See [:material-code-braces: EndOfMeetingReminderTypeDef](./type_defs.md#endofmeetingremindertypedef) 
2. See [:material-code-braces: InstantBookingTypeDef](./type_defs.md#instantbookingtypedef) 
3. See [:material-code-braces: RequireCheckInTypeDef](./type_defs.md#requirecheckintypedef) 
4. See [:material-code-braces: ProactiveJoinTypeDef](./type_defs.md#proactivejointypedef) 
## SearchNetworkProfilesResponseTypeDef

```python
# SearchNetworkProfilesResponseTypeDef definition

class SearchNetworkProfilesResponseTypeDef(TypedDict):
    NetworkProfiles: List[NetworkProfileDataTypeDef],  # (1)
    NextToken: str,
    TotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkProfileDataTypeDef](./type_defs.md#networkprofiledatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchProfilesResponseTypeDef

```python
# SearchProfilesResponseTypeDef definition

class SearchProfilesResponseTypeDef(TypedDict):
    Profiles: List[ProfileDataTypeDef],  # (1)
    NextToken: str,
    TotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfileDataTypeDef](./type_defs.md#profiledatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchRoomsResponseTypeDef

```python
# SearchRoomsResponseTypeDef definition

class SearchRoomsResponseTypeDef(TypedDict):
    Rooms: List[RoomDataTypeDef],  # (1)
    NextToken: str,
    TotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoomDataTypeDef](./type_defs.md#roomdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchAddressBooksRequestRequestTypeDef

```python
# SearchAddressBooksRequestRequestTypeDef definition

class SearchAddressBooksRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    SortCriteria: NotRequired[Sequence[SortTypeDef]],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
## SearchContactsRequestRequestTypeDef

```python
# SearchContactsRequestRequestTypeDef definition

class SearchContactsRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    SortCriteria: NotRequired[Sequence[SortTypeDef]],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
## SearchDevicesRequestRequestTypeDef

```python
# SearchDevicesRequestRequestTypeDef definition

class SearchDevicesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    SortCriteria: NotRequired[Sequence[SortTypeDef]],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
## SearchDevicesRequestSearchDevicesPaginateTypeDef

```python
# SearchDevicesRequestSearchDevicesPaginateTypeDef definition

class SearchDevicesRequestSearchDevicesPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    SortCriteria: NotRequired[Sequence[SortTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchNetworkProfilesRequestRequestTypeDef

```python
# SearchNetworkProfilesRequestRequestTypeDef definition

class SearchNetworkProfilesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    SortCriteria: NotRequired[Sequence[SortTypeDef]],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
## SearchProfilesRequestRequestTypeDef

```python
# SearchProfilesRequestRequestTypeDef definition

class SearchProfilesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    SortCriteria: NotRequired[Sequence[SortTypeDef]],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
## SearchProfilesRequestSearchProfilesPaginateTypeDef

```python
# SearchProfilesRequestSearchProfilesPaginateTypeDef definition

class SearchProfilesRequestSearchProfilesPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    SortCriteria: NotRequired[Sequence[SortTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchRoomsRequestRequestTypeDef

```python
# SearchRoomsRequestRequestTypeDef definition

class SearchRoomsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    SortCriteria: NotRequired[Sequence[SortTypeDef]],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
## SearchRoomsRequestSearchRoomsPaginateTypeDef

```python
# SearchRoomsRequestSearchRoomsPaginateTypeDef definition

class SearchRoomsRequestSearchRoomsPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    SortCriteria: NotRequired[Sequence[SortTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchSkillGroupsRequestRequestTypeDef

```python
# SearchSkillGroupsRequestRequestTypeDef definition

class SearchSkillGroupsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    SortCriteria: NotRequired[Sequence[SortTypeDef]],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
## SearchSkillGroupsRequestSearchSkillGroupsPaginateTypeDef

```python
# SearchSkillGroupsRequestSearchSkillGroupsPaginateTypeDef definition

class SearchSkillGroupsRequestSearchSkillGroupsPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    SortCriteria: NotRequired[Sequence[SortTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchUsersRequestRequestTypeDef

```python
# SearchUsersRequestRequestTypeDef definition

class SearchUsersRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    SortCriteria: NotRequired[Sequence[SortTypeDef]],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
## SearchUsersRequestSearchUsersPaginateTypeDef

```python
# SearchUsersRequestSearchUsersPaginateTypeDef definition

class SearchUsersRequestSearchUsersPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    SortCriteria: NotRequired[Sequence[SortTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchSkillGroupsResponseTypeDef

```python
# SearchSkillGroupsResponseTypeDef definition

class SearchSkillGroupsResponseTypeDef(TypedDict):
    SkillGroups: List[SkillGroupDataTypeDef],  # (1)
    NextToken: str,
    TotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SkillGroupDataTypeDef](./type_defs.md#skillgroupdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchUsersResponseTypeDef

```python
# SearchUsersResponseTypeDef definition

class SearchUsersResponseTypeDef(TypedDict):
    Users: List[UserDataTypeDef],  # (1)
    NextToken: str,
    TotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserDataTypeDef](./type_defs.md#userdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMeetingRoomConfigurationTypeDef

```python
# UpdateMeetingRoomConfigurationTypeDef definition

class UpdateMeetingRoomConfigurationTypeDef(TypedDict):
    RoomUtilizationMetricsEnabled: NotRequired[bool],
    EndOfMeetingReminder: NotRequired[UpdateEndOfMeetingReminderTypeDef],  # (1)
    InstantBooking: NotRequired[UpdateInstantBookingTypeDef],  # (2)
    RequireCheckIn: NotRequired[UpdateRequireCheckInTypeDef],  # (3)
    ProactiveJoin: NotRequired[UpdateProactiveJoinTypeDef],  # (4)
```

1. See [:material-code-braces: UpdateEndOfMeetingReminderTypeDef](./type_defs.md#updateendofmeetingremindertypedef) 
2. See [:material-code-braces: UpdateInstantBookingTypeDef](./type_defs.md#updateinstantbookingtypedef) 
3. See [:material-code-braces: UpdateRequireCheckInTypeDef](./type_defs.md#updaterequirecheckintypedef) 
4. See [:material-code-braces: UpdateProactiveJoinTypeDef](./type_defs.md#updateproactivejointypedef) 
## BusinessReportScheduleTypeDef

```python
# BusinessReportScheduleTypeDef definition

class BusinessReportScheduleTypeDef(TypedDict):
    ScheduleArn: NotRequired[str],
    ScheduleName: NotRequired[str],
    S3BucketName: NotRequired[str],
    S3KeyPrefix: NotRequired[str],
    Format: NotRequired[BusinessReportFormatType],  # (1)
    ContentRange: NotRequired[BusinessReportContentRangeTypeDef],  # (2)
    Recurrence: NotRequired[BusinessReportRecurrenceTypeDef],  # (3)
    LastBusinessReport: NotRequired[BusinessReportTypeDef],  # (4)
```

1. See [:material-code-brackets: BusinessReportFormatType](./literals.md#businessreportformattype) 
2. See [:material-code-braces: BusinessReportContentRangeTypeDef](./type_defs.md#businessreportcontentrangetypedef) 
3. See [:material-code-braces: BusinessReportRecurrenceTypeDef](./type_defs.md#businessreportrecurrencetypedef) 
4. See [:material-code-braces: BusinessReportTypeDef](./type_defs.md#businessreporttypedef) 
## GetConferenceProviderResponseTypeDef

```python
# GetConferenceProviderResponseTypeDef definition

class GetConferenceProviderResponseTypeDef(TypedDict):
    ConferenceProvider: ConferenceProviderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConferenceProviderTypeDef](./type_defs.md#conferenceprovidertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConferenceProvidersResponseTypeDef

```python
# ListConferenceProvidersResponseTypeDef definition

class ListConferenceProvidersResponseTypeDef(TypedDict):
    ConferenceProviders: List[ConferenceProviderTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConferenceProviderTypeDef](./type_defs.md#conferenceprovidertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchContactsResponseTypeDef

```python
# SearchContactsResponseTypeDef definition

class SearchContactsResponseTypeDef(TypedDict):
    Contacts: List[ContactDataTypeDef],  # (1)
    NextToken: str,
    TotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContactDataTypeDef](./type_defs.md#contactdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetContactResponseTypeDef

```python
# GetContactResponseTypeDef definition

class GetContactResponseTypeDef(TypedDict):
    Contact: ContactTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContactTypeDef](./type_defs.md#contacttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendAnnouncementRequestRequestTypeDef

```python
# SendAnnouncementRequestRequestTypeDef definition

class SendAnnouncementRequestRequestTypeDef(TypedDict):
    RoomFilters: Sequence[FilterTypeDef],  # (1)
    Content: ContentTypeDef,  # (2)
    ClientRequestToken: str,
    TimeToLiveInSeconds: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ContentTypeDef](./type_defs.md#contenttypedef) 
## CreateProfileRequestRequestTypeDef

```python
# CreateProfileRequestRequestTypeDef definition

class CreateProfileRequestRequestTypeDef(TypedDict):
    ProfileName: str,
    Timezone: str,
    Address: str,
    DistanceUnit: DistanceUnitType,  # (1)
    TemperatureUnit: TemperatureUnitType,  # (2)
    WakeWord: WakeWordType,  # (3)
    Locale: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    SetupModeDisabled: NotRequired[bool],
    MaxVolumeLimit: NotRequired[int],
    PSTNEnabled: NotRequired[bool],
    DataRetentionOptIn: NotRequired[bool],
    MeetingRoomConfiguration: NotRequired[CreateMeetingRoomConfigurationTypeDef],  # (4)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (5)
```

1. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
2. See [:material-code-brackets: TemperatureUnitType](./literals.md#temperatureunittype) 
3. See [:material-code-brackets: WakeWordType](./literals.md#wakewordtype) 
4. See [:material-code-braces: CreateMeetingRoomConfigurationTypeDef](./type_defs.md#createmeetingroomconfigurationtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## SkillsStoreSkillTypeDef

```python
# SkillsStoreSkillTypeDef definition

class SkillsStoreSkillTypeDef(TypedDict):
    SkillId: NotRequired[str],
    SkillName: NotRequired[str],
    ShortDescription: NotRequired[str],
    IconUrl: NotRequired[str],
    SampleUtterances: NotRequired[List[str]],
    SkillDetails: NotRequired[SkillDetailsTypeDef],  # (1)
    SupportsLinking: NotRequired[bool],
```

1. See [:material-code-braces: SkillDetailsTypeDef](./type_defs.md#skilldetailstypedef) 
## DeviceDataTypeDef

```python
# DeviceDataTypeDef definition

class DeviceDataTypeDef(TypedDict):
    DeviceArn: NotRequired[str],
    DeviceSerialNumber: NotRequired[str],
    DeviceType: NotRequired[str],
    DeviceName: NotRequired[str],
    SoftwareVersion: NotRequired[str],
    MacAddress: NotRequired[str],
    DeviceStatus: NotRequired[DeviceStatusType],  # (1)
    NetworkProfileArn: NotRequired[str],
    NetworkProfileName: NotRequired[str],
    RoomArn: NotRequired[str],
    RoomName: NotRequired[str],
    DeviceStatusInfo: NotRequired[DeviceStatusInfoTypeDef],  # (2)
    CreatedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: DeviceStatusType](./literals.md#devicestatustype) 
2. See [:material-code-braces: DeviceStatusInfoTypeDef](./type_defs.md#devicestatusinfotypedef) 
## DeviceTypeDef

```python
# DeviceTypeDef definition

class DeviceTypeDef(TypedDict):
    DeviceArn: NotRequired[str],
    DeviceSerialNumber: NotRequired[str],
    DeviceType: NotRequired[str],
    DeviceName: NotRequired[str],
    SoftwareVersion: NotRequired[str],
    MacAddress: NotRequired[str],
    RoomArn: NotRequired[str],
    DeviceStatus: NotRequired[DeviceStatusType],  # (1)
    DeviceStatusInfo: NotRequired[DeviceStatusInfoTypeDef],  # (2)
    NetworkProfileInfo: NotRequired[DeviceNetworkProfileInfoTypeDef],  # (3)
```

1. See [:material-code-brackets: DeviceStatusType](./literals.md#devicestatustype) 
2. See [:material-code-braces: DeviceStatusInfoTypeDef](./type_defs.md#devicestatusinfotypedef) 
3. See [:material-code-braces: DeviceNetworkProfileInfoTypeDef](./type_defs.md#devicenetworkprofileinfotypedef) 
## ProfileTypeDef

```python
# ProfileTypeDef definition

class ProfileTypeDef(TypedDict):
    ProfileArn: NotRequired[str],
    ProfileName: NotRequired[str],
    IsDefault: NotRequired[bool],
    Address: NotRequired[str],
    Timezone: NotRequired[str],
    DistanceUnit: NotRequired[DistanceUnitType],  # (1)
    TemperatureUnit: NotRequired[TemperatureUnitType],  # (2)
    WakeWord: NotRequired[WakeWordType],  # (3)
    Locale: NotRequired[str],
    SetupModeDisabled: NotRequired[bool],
    MaxVolumeLimit: NotRequired[int],
    PSTNEnabled: NotRequired[bool],
    DataRetentionOptIn: NotRequired[bool],
    AddressBookArn: NotRequired[str],
    MeetingRoomConfiguration: NotRequired[MeetingRoomConfigurationTypeDef],  # (4)
```

1. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
2. See [:material-code-brackets: TemperatureUnitType](./literals.md#temperatureunittype) 
3. See [:material-code-brackets: WakeWordType](./literals.md#wakewordtype) 
4. See [:material-code-braces: MeetingRoomConfigurationTypeDef](./type_defs.md#meetingroomconfigurationtypedef) 
## UpdateProfileRequestRequestTypeDef

```python
# UpdateProfileRequestRequestTypeDef definition

class UpdateProfileRequestRequestTypeDef(TypedDict):
    ProfileArn: NotRequired[str],
    ProfileName: NotRequired[str],
    IsDefault: NotRequired[bool],
    Timezone: NotRequired[str],
    Address: NotRequired[str],
    DistanceUnit: NotRequired[DistanceUnitType],  # (1)
    TemperatureUnit: NotRequired[TemperatureUnitType],  # (2)
    WakeWord: NotRequired[WakeWordType],  # (3)
    Locale: NotRequired[str],
    SetupModeDisabled: NotRequired[bool],
    MaxVolumeLimit: NotRequired[int],
    PSTNEnabled: NotRequired[bool],
    DataRetentionOptIn: NotRequired[bool],
    MeetingRoomConfiguration: NotRequired[UpdateMeetingRoomConfigurationTypeDef],  # (4)
```

1. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
2. See [:material-code-brackets: TemperatureUnitType](./literals.md#temperatureunittype) 
3. See [:material-code-brackets: WakeWordType](./literals.md#wakewordtype) 
4. See [:material-code-braces: UpdateMeetingRoomConfigurationTypeDef](./type_defs.md#updatemeetingroomconfigurationtypedef) 
## ListBusinessReportSchedulesResponseTypeDef

```python
# ListBusinessReportSchedulesResponseTypeDef definition

class ListBusinessReportSchedulesResponseTypeDef(TypedDict):
    BusinessReportSchedules: List[BusinessReportScheduleTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BusinessReportScheduleTypeDef](./type_defs.md#businessreportscheduletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSkillsStoreSkillsByCategoryResponseTypeDef

```python
# ListSkillsStoreSkillsByCategoryResponseTypeDef definition

class ListSkillsStoreSkillsByCategoryResponseTypeDef(TypedDict):
    SkillsStoreSkills: List[SkillsStoreSkillTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SkillsStoreSkillTypeDef](./type_defs.md#skillsstoreskilltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchDevicesResponseTypeDef

```python
# SearchDevicesResponseTypeDef definition

class SearchDevicesResponseTypeDef(TypedDict):
    Devices: List[DeviceDataTypeDef],  # (1)
    NextToken: str,
    TotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeviceDataTypeDef](./type_defs.md#devicedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeviceResponseTypeDef

```python
# GetDeviceResponseTypeDef definition

class GetDeviceResponseTypeDef(TypedDict):
    Device: DeviceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeviceTypeDef](./type_defs.md#devicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProfileResponseTypeDef

```python
# GetProfileResponseTypeDef definition

class GetProfileResponseTypeDef(TypedDict):
    Profile: ProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfileTypeDef](./type_defs.md#profiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
