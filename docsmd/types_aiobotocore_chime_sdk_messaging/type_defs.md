# Type definitions

> [Index](../README.md) > [ChimeSDKMessaging](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ChimeSDKMessaging](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
    type annotations stubs module [types-aiobotocore-chime-sdk-messaging](https://pypi.org/project/types-aiobotocore-chime-sdk-messaging/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## MessageAttributeValueUnionTypeDef

```python
# MessageAttributeValueUnionTypeDef definition

MessageAttributeValueUnionTypeDef = Union[
    MessageAttributeValueTypeDef,  # (1)
    MessageAttributeValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MessageAttributeValueTypeDef](./type_defs.md#messageattributevaluetypedef) 
2. See [:material-code-braces: MessageAttributeValueOutputTypeDef](./type_defs.md#messageattributevalueoutputtypedef) 



## AppInstanceUserMembershipSummaryTypeDef

```python
# AppInstanceUserMembershipSummaryTypeDef definition

class AppInstanceUserMembershipSummaryTypeDef(TypedDict):
    Type: NotRequired[ChannelMembershipTypeType],  # (1)
    ReadMarkerTimestamp: NotRequired[datetime],
    SubChannelId: NotRequired[str],
```

1. See [:material-code-brackets: ChannelMembershipTypeType](./literals.md#channelmembershiptypetype) 
## AssociateChannelFlowRequestRequestTypeDef

```python
# AssociateChannelFlowRequestRequestTypeDef definition

class AssociateChannelFlowRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChannelFlowArn: str,
    ChimeBearer: str,
```

## IdentityTypeDef

```python
# IdentityTypeDef definition

class IdentityTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
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
    ChimeBearer: str,
    Type: NotRequired[ChannelMembershipTypeType],  # (1)
    SubChannelId: NotRequired[str],
```

1. See [:material-code-brackets: ChannelMembershipTypeType](./literals.md#channelmembershiptypetype) 
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

## ChannelAssociatedWithFlowSummaryTypeDef

```python
# ChannelAssociatedWithFlowSummaryTypeDef definition

class ChannelAssociatedWithFlowSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    ChannelArn: NotRequired[str],
    Mode: NotRequired[ChannelModeType],  # (1)
    Privacy: NotRequired[ChannelPrivacyType],  # (2)
    Metadata: NotRequired[str],
```

1. See [:material-code-brackets: ChannelModeType](./literals.md#channelmodetype) 
2. See [:material-code-brackets: ChannelPrivacyType](./literals.md#channelprivacytype) 
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
## PushNotificationPreferencesTypeDef

```python
# PushNotificationPreferencesTypeDef definition

class PushNotificationPreferencesTypeDef(TypedDict):
    AllowNotifications: AllowNotificationsType,  # (1)
    FilterRule: NotRequired[str],
```

1. See [:material-code-brackets: AllowNotificationsType](./literals.md#allownotificationstype) 
## PushNotificationConfigurationTypeDef

```python
# PushNotificationConfigurationTypeDef definition

class PushNotificationConfigurationTypeDef(TypedDict):
    Title: NotRequired[str],
    Body: NotRequired[str],
    Type: NotRequired[PushNotificationTypeType],  # (1)
```

1. See [:material-code-brackets: PushNotificationTypeType](./literals.md#pushnotificationtypetype) 
## ChannelMessageStatusStructureTypeDef

```python
# ChannelMessageStatusStructureTypeDef definition

class ChannelMessageStatusStructureTypeDef(TypedDict):
    Value: NotRequired[ChannelMessageStatusType],  # (1)
    Detail: NotRequired[str],
```

1. See [:material-code-brackets: ChannelMessageStatusType](./literals.md#channelmessagestatustype) 
## MessageAttributeValueOutputTypeDef

```python
# MessageAttributeValueOutputTypeDef definition

class MessageAttributeValueOutputTypeDef(TypedDict):
    StringValues: NotRequired[List[str]],
```

## TargetTypeDef

```python
# TargetTypeDef definition

class TargetTypeDef(TypedDict):
    MemberArn: NotRequired[str],
```

## ElasticChannelConfigurationTypeDef

```python
# ElasticChannelConfigurationTypeDef definition

class ElasticChannelConfigurationTypeDef(TypedDict):
    MaximumSubChannels: int,
    TargetMembershipsPerSubChannel: int,
    MinimumMembershipPercentage: int,
```

## ExpirationSettingsTypeDef

```python
# ExpirationSettingsTypeDef definition

class ExpirationSettingsTypeDef(TypedDict):
    ExpirationDays: int,
    ExpirationCriterion: ExpirationCriterionType,  # (1)
```

1. See [:material-code-brackets: ExpirationCriterionType](./literals.md#expirationcriteriontype) 
## CreateChannelBanRequestRequestTypeDef

```python
# CreateChannelBanRequestRequestTypeDef definition

class CreateChannelBanRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MemberArn: str,
    ChimeBearer: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## CreateChannelMembershipRequestRequestTypeDef

```python
# CreateChannelMembershipRequestRequestTypeDef definition

class CreateChannelMembershipRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MemberArn: str,
    Type: ChannelMembershipTypeType,  # (1)
    ChimeBearer: str,
    SubChannelId: NotRequired[str],
```

1. See [:material-code-brackets: ChannelMembershipTypeType](./literals.md#channelmembershiptypetype) 
## CreateChannelModeratorRequestRequestTypeDef

```python
# CreateChannelModeratorRequestRequestTypeDef definition

class CreateChannelModeratorRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChannelModeratorArn: str,
    ChimeBearer: str,
```

## DeleteChannelBanRequestRequestTypeDef

```python
# DeleteChannelBanRequestRequestTypeDef definition

class DeleteChannelBanRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MemberArn: str,
    ChimeBearer: str,
```

## DeleteChannelFlowRequestRequestTypeDef

```python
# DeleteChannelFlowRequestRequestTypeDef definition

class DeleteChannelFlowRequestRequestTypeDef(TypedDict):
    ChannelFlowArn: str,
```

## DeleteChannelMembershipRequestRequestTypeDef

```python
# DeleteChannelMembershipRequestRequestTypeDef definition

class DeleteChannelMembershipRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MemberArn: str,
    ChimeBearer: str,
    SubChannelId: NotRequired[str],
```

## DeleteChannelMessageRequestRequestTypeDef

```python
# DeleteChannelMessageRequestRequestTypeDef definition

class DeleteChannelMessageRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MessageId: str,
    ChimeBearer: str,
    SubChannelId: NotRequired[str],
```

## DeleteChannelModeratorRequestRequestTypeDef

```python
# DeleteChannelModeratorRequestRequestTypeDef definition

class DeleteChannelModeratorRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChannelModeratorArn: str,
    ChimeBearer: str,
```

## DeleteChannelRequestRequestTypeDef

```python
# DeleteChannelRequestRequestTypeDef definition

class DeleteChannelRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChimeBearer: str,
```

## DeleteMessagingStreamingConfigurationsRequestRequestTypeDef

```python
# DeleteMessagingStreamingConfigurationsRequestRequestTypeDef definition

class DeleteMessagingStreamingConfigurationsRequestRequestTypeDef(TypedDict):
    AppInstanceArn: str,
```

## DescribeChannelBanRequestRequestTypeDef

```python
# DescribeChannelBanRequestRequestTypeDef definition

class DescribeChannelBanRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MemberArn: str,
    ChimeBearer: str,
```

## DescribeChannelFlowRequestRequestTypeDef

```python
# DescribeChannelFlowRequestRequestTypeDef definition

class DescribeChannelFlowRequestRequestTypeDef(TypedDict):
    ChannelFlowArn: str,
```

## DescribeChannelMembershipForAppInstanceUserRequestRequestTypeDef

```python
# DescribeChannelMembershipForAppInstanceUserRequestRequestTypeDef definition

class DescribeChannelMembershipForAppInstanceUserRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    AppInstanceUserArn: str,
    ChimeBearer: str,
```

## DescribeChannelMembershipRequestRequestTypeDef

```python
# DescribeChannelMembershipRequestRequestTypeDef definition

class DescribeChannelMembershipRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MemberArn: str,
    ChimeBearer: str,
    SubChannelId: NotRequired[str],
```

## DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef

```python
# DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef definition

class DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    AppInstanceUserArn: str,
    ChimeBearer: str,
```

## DescribeChannelModeratorRequestRequestTypeDef

```python
# DescribeChannelModeratorRequestRequestTypeDef definition

class DescribeChannelModeratorRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChannelModeratorArn: str,
    ChimeBearer: str,
```

## DescribeChannelRequestRequestTypeDef

```python
# DescribeChannelRequestRequestTypeDef definition

class DescribeChannelRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChimeBearer: str,
```

## DisassociateChannelFlowRequestRequestTypeDef

```python
# DisassociateChannelFlowRequestRequestTypeDef definition

class DisassociateChannelFlowRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChannelFlowArn: str,
    ChimeBearer: str,
```

## GetChannelMembershipPreferencesRequestRequestTypeDef

```python
# GetChannelMembershipPreferencesRequestRequestTypeDef definition

class GetChannelMembershipPreferencesRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MemberArn: str,
    ChimeBearer: str,
```

## GetChannelMessageRequestRequestTypeDef

```python
# GetChannelMessageRequestRequestTypeDef definition

class GetChannelMessageRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MessageId: str,
    ChimeBearer: str,
    SubChannelId: NotRequired[str],
```

## GetChannelMessageStatusRequestRequestTypeDef

```python
# GetChannelMessageStatusRequestRequestTypeDef definition

class GetChannelMessageStatusRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MessageId: str,
    ChimeBearer: str,
    SubChannelId: NotRequired[str],
```

## MessagingSessionEndpointTypeDef

```python
# MessagingSessionEndpointTypeDef definition

class MessagingSessionEndpointTypeDef(TypedDict):
    Url: NotRequired[str],
```

## GetMessagingStreamingConfigurationsRequestRequestTypeDef

```python
# GetMessagingStreamingConfigurationsRequestRequestTypeDef definition

class GetMessagingStreamingConfigurationsRequestRequestTypeDef(TypedDict):
    AppInstanceArn: str,
```

## StreamingConfigurationTypeDef

```python
# StreamingConfigurationTypeDef definition

class StreamingConfigurationTypeDef(TypedDict):
    DataType: MessagingDataTypeType,  # (1)
    ResourceArn: str,
```

1. See [:material-code-brackets: MessagingDataTypeType](./literals.md#messagingdatatypetype) 
## LambdaConfigurationTypeDef

```python
# LambdaConfigurationTypeDef definition

class LambdaConfigurationTypeDef(TypedDict):
    ResourceArn: str,
    InvocationType: InvocationTypeType,  # (1)
```

1. See [:material-code-brackets: InvocationTypeType](./literals.md#invocationtypetype) 
## ListChannelBansRequestRequestTypeDef

```python
# ListChannelBansRequestRequestTypeDef definition

class ListChannelBansRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChimeBearer: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListChannelFlowsRequestRequestTypeDef

```python
# ListChannelFlowsRequestRequestTypeDef definition

class ListChannelFlowsRequestRequestTypeDef(TypedDict):
    AppInstanceArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef

```python
# ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef definition

class ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef(TypedDict):
    ChimeBearer: str,
    AppInstanceUserArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListChannelMembershipsRequestRequestTypeDef

```python
# ListChannelMembershipsRequestRequestTypeDef definition

class ListChannelMembershipsRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChimeBearer: str,
    Type: NotRequired[ChannelMembershipTypeType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    SubChannelId: NotRequired[str],
```

1. See [:material-code-brackets: ChannelMembershipTypeType](./literals.md#channelmembershiptypetype) 
## ListChannelModeratorsRequestRequestTypeDef

```python
# ListChannelModeratorsRequestRequestTypeDef definition

class ListChannelModeratorsRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChimeBearer: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef

```python
# ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef definition

class ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef(TypedDict):
    ChannelFlowArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef

```python
# ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef definition

class ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef(TypedDict):
    ChimeBearer: str,
    AppInstanceUserArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListChannelsRequestRequestTypeDef

```python
# ListChannelsRequestRequestTypeDef definition

class ListChannelsRequestRequestTypeDef(TypedDict):
    AppInstanceArn: str,
    ChimeBearer: str,
    Privacy: NotRequired[ChannelPrivacyType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ChannelPrivacyType](./literals.md#channelprivacytype) 
## ListSubChannelsRequestRequestTypeDef

```python
# ListSubChannelsRequestRequestTypeDef definition

class ListSubChannelsRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChimeBearer: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## SubChannelSummaryTypeDef

```python
# SubChannelSummaryTypeDef definition

class SubChannelSummaryTypeDef(TypedDict):
    SubChannelId: NotRequired[str],
    MembershipCount: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## MessageAttributeValueTypeDef

```python
# MessageAttributeValueTypeDef definition

class MessageAttributeValueTypeDef(TypedDict):
    StringValues: NotRequired[Sequence[str]],
```

## RedactChannelMessageRequestRequestTypeDef

```python
# RedactChannelMessageRequestRequestTypeDef definition

class RedactChannelMessageRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MessageId: str,
    ChimeBearer: str,
    SubChannelId: NotRequired[str],
```

## SearchFieldTypeDef

```python
# SearchFieldTypeDef definition

class SearchFieldTypeDef(TypedDict):
    Key: SearchFieldKeyType,  # (1)
    Values: Sequence[str],
    Operator: SearchFieldOperatorType,  # (2)
```

1. See [:material-code-brackets: SearchFieldKeyType](./literals.md#searchfieldkeytype) 
2. See [:material-code-brackets: SearchFieldOperatorType](./literals.md#searchfieldoperatortype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateChannelMessageRequestRequestTypeDef

```python
# UpdateChannelMessageRequestRequestTypeDef definition

class UpdateChannelMessageRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MessageId: str,
    Content: str,
    ChimeBearer: str,
    Metadata: NotRequired[str],
    SubChannelId: NotRequired[str],
    ContentType: NotRequired[str],
```

## UpdateChannelReadMarkerRequestRequestTypeDef

```python
# UpdateChannelReadMarkerRequestRequestTypeDef definition

class UpdateChannelReadMarkerRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChimeBearer: str,
```

## UpdateChannelRequestRequestTypeDef

```python
# UpdateChannelRequestRequestTypeDef definition

class UpdateChannelRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChimeBearer: str,
    Name: NotRequired[str],
    Mode: NotRequired[ChannelModeType],  # (1)
    Metadata: NotRequired[str],
```

1. See [:material-code-brackets: ChannelModeType](./literals.md#channelmodetype) 
## BatchChannelMembershipsTypeDef

```python
# BatchChannelMembershipsTypeDef definition

class BatchChannelMembershipsTypeDef(TypedDict):
    InvitedBy: NotRequired[IdentityTypeDef],  # (1)
    Type: NotRequired[ChannelMembershipTypeType],  # (2)
    Members: NotRequired[List[IdentityTypeDef]],  # (3)
    ChannelArn: NotRequired[str],
    SubChannelId: NotRequired[str],
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
    SubChannelId: NotRequired[str],
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
2. See [:material-code-brackets: ChannelMembershipTypeType](./literals.md#channelmembershiptypetype) 
3. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
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
## ChannelFlowCallbackResponseTypeDef

```python
# ChannelFlowCallbackResponseTypeDef definition

class ChannelFlowCallbackResponseTypeDef(TypedDict):
    ChannelArn: str,
    CallbackId: str,
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
## CreateChannelFlowResponseTypeDef

```python
# CreateChannelFlowResponseTypeDef definition

class CreateChannelFlowResponseTypeDef(TypedDict):
    ChannelFlowArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateChannelMembershipResponseTypeDef

```python
# CreateChannelMembershipResponseTypeDef definition

class CreateChannelMembershipResponseTypeDef(TypedDict):
    ChannelArn: str,
    Member: IdentityTypeDef,  # (1)
    SubChannelId: str,
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
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RedactChannelMessageResponseTypeDef

```python
# RedactChannelMessageResponseTypeDef definition

class RedactChannelMessageResponseTypeDef(TypedDict):
    ChannelArn: str,
    MessageId: str,
    SubChannelId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateChannelFlowResponseTypeDef

```python
# UpdateChannelFlowResponseTypeDef definition

class UpdateChannelFlowResponseTypeDef(TypedDict):
    ChannelFlowArn: str,
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
## ListChannelsAssociatedWithChannelFlowResponseTypeDef

```python
# ListChannelsAssociatedWithChannelFlowResponseTypeDef definition

class ListChannelsAssociatedWithChannelFlowResponseTypeDef(TypedDict):
    Channels: List[ChannelAssociatedWithFlowSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ChannelAssociatedWithFlowSummaryTypeDef](./type_defs.md#channelassociatedwithflowsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## SearchChannelsResponseTypeDef

```python
# SearchChannelsResponseTypeDef definition

class SearchChannelsResponseTypeDef(TypedDict):
    Channels: List[ChannelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ChannelSummaryTypeDef](./type_defs.md#channelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ChannelMembershipPreferencesTypeDef

```python
# ChannelMembershipPreferencesTypeDef definition

class ChannelMembershipPreferencesTypeDef(TypedDict):
    PushNotifications: NotRequired[PushNotificationPreferencesTypeDef],  # (1)
```

1. See [:material-code-braces: PushNotificationPreferencesTypeDef](./type_defs.md#pushnotificationpreferencestypedef) 
## GetChannelMessageStatusResponseTypeDef

```python
# GetChannelMessageStatusResponseTypeDef definition

class GetChannelMessageStatusResponseTypeDef(TypedDict):
    Status: ChannelMessageStatusStructureTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelMessageStatusStructureTypeDef](./type_defs.md#channelmessagestatusstructuretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendChannelMessageResponseTypeDef

```python
# SendChannelMessageResponseTypeDef definition

class SendChannelMessageResponseTypeDef(TypedDict):
    ChannelArn: str,
    MessageId: str,
    Status: ChannelMessageStatusStructureTypeDef,  # (1)
    SubChannelId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelMessageStatusStructureTypeDef](./type_defs.md#channelmessagestatusstructuretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateChannelMessageResponseTypeDef

```python
# UpdateChannelMessageResponseTypeDef definition

class UpdateChannelMessageResponseTypeDef(TypedDict):
    ChannelArn: str,
    MessageId: str,
    Status: ChannelMessageStatusStructureTypeDef,  # (1)
    SubChannelId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelMessageStatusStructureTypeDef](./type_defs.md#channelmessagestatusstructuretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    Status: NotRequired[ChannelMessageStatusStructureTypeDef],  # (3)
    MessageAttributes: NotRequired[Dict[str, MessageAttributeValueOutputTypeDef]],  # (4)
    ContentType: NotRequired[str],
    Target: NotRequired[List[TargetTypeDef]],  # (5)
```

1. See [:material-code-brackets: ChannelMessageTypeType](./literals.md#channelmessagetypetype) 
2. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
3. See [:material-code-braces: ChannelMessageStatusStructureTypeDef](./type_defs.md#channelmessagestatusstructuretypedef) 
4. See [:material-code-braces: MessageAttributeValueOutputTypeDef](./type_defs.md#messageattributevalueoutputtypedef) 
5. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
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
    Status: NotRequired[ChannelMessageStatusStructureTypeDef],  # (4)
    MessageAttributes: NotRequired[Dict[str, MessageAttributeValueOutputTypeDef]],  # (5)
    SubChannelId: NotRequired[str],
    ContentType: NotRequired[str],
    Target: NotRequired[List[TargetTypeDef]],  # (6)
```

1. See [:material-code-brackets: ChannelMessageTypeType](./literals.md#channelmessagetypetype) 
2. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
3. See [:material-code-brackets: ChannelMessagePersistenceTypeType](./literals.md#channelmessagepersistencetypetype) 
4. See [:material-code-braces: ChannelMessageStatusStructureTypeDef](./type_defs.md#channelmessagestatusstructuretypedef) 
5. See [:material-code-braces: MessageAttributeValueOutputTypeDef](./type_defs.md#messageattributevalueoutputtypedef) 
6. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
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
    ChannelFlowArn: NotRequired[str],
    ElasticChannelConfiguration: NotRequired[ElasticChannelConfigurationTypeDef],  # (4)
    ExpirationSettings: NotRequired[ExpirationSettingsTypeDef],  # (5)
```

1. See [:material-code-brackets: ChannelModeType](./literals.md#channelmodetype) 
2. See [:material-code-brackets: ChannelPrivacyType](./literals.md#channelprivacytype) 
3. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
4. See [:material-code-braces: ElasticChannelConfigurationTypeDef](./type_defs.md#elasticchannelconfigurationtypedef) 
5. See [:material-code-braces: ExpirationSettingsTypeDef](./type_defs.md#expirationsettingstypedef) 
## PutChannelExpirationSettingsRequestRequestTypeDef

```python
# PutChannelExpirationSettingsRequestRequestTypeDef definition

class PutChannelExpirationSettingsRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChimeBearer: NotRequired[str],
    ExpirationSettings: NotRequired[ExpirationSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: ExpirationSettingsTypeDef](./type_defs.md#expirationsettingstypedef) 
## PutChannelExpirationSettingsResponseTypeDef

```python
# PutChannelExpirationSettingsResponseTypeDef definition

class PutChannelExpirationSettingsResponseTypeDef(TypedDict):
    ChannelArn: str,
    ExpirationSettings: ExpirationSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExpirationSettingsTypeDef](./type_defs.md#expirationsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateChannelRequestRequestTypeDef

```python
# CreateChannelRequestRequestTypeDef definition

class CreateChannelRequestRequestTypeDef(TypedDict):
    AppInstanceArn: str,
    Name: str,
    ClientRequestToken: str,
    ChimeBearer: str,
    Mode: NotRequired[ChannelModeType],  # (1)
    Privacy: NotRequired[ChannelPrivacyType],  # (2)
    Metadata: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    ChannelId: NotRequired[str],
    MemberArns: NotRequired[Sequence[str]],
    ModeratorArns: NotRequired[Sequence[str]],
    ElasticChannelConfiguration: NotRequired[ElasticChannelConfigurationTypeDef],  # (4)
    ExpirationSettings: NotRequired[ExpirationSettingsTypeDef],  # (5)
```

1. See [:material-code-brackets: ChannelModeType](./literals.md#channelmodetype) 
2. See [:material-code-brackets: ChannelPrivacyType](./literals.md#channelprivacytype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: ElasticChannelConfigurationTypeDef](./type_defs.md#elasticchannelconfigurationtypedef) 
5. See [:material-code-braces: ExpirationSettingsTypeDef](./type_defs.md#expirationsettingstypedef) 
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
## GetMessagingSessionEndpointResponseTypeDef

```python
# GetMessagingSessionEndpointResponseTypeDef definition

class GetMessagingSessionEndpointResponseTypeDef(TypedDict):
    Endpoint: MessagingSessionEndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessagingSessionEndpointTypeDef](./type_defs.md#messagingsessionendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMessagingStreamingConfigurationsResponseTypeDef

```python
# GetMessagingStreamingConfigurationsResponseTypeDef definition

class GetMessagingStreamingConfigurationsResponseTypeDef(TypedDict):
    StreamingConfigurations: List[StreamingConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingConfigurationTypeDef](./type_defs.md#streamingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutMessagingStreamingConfigurationsRequestRequestTypeDef

```python
# PutMessagingStreamingConfigurationsRequestRequestTypeDef definition

class PutMessagingStreamingConfigurationsRequestRequestTypeDef(TypedDict):
    AppInstanceArn: str,
    StreamingConfigurations: Sequence[StreamingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: StreamingConfigurationTypeDef](./type_defs.md#streamingconfigurationtypedef) 
## PutMessagingStreamingConfigurationsResponseTypeDef

```python
# PutMessagingStreamingConfigurationsResponseTypeDef definition

class PutMessagingStreamingConfigurationsResponseTypeDef(TypedDict):
    StreamingConfigurations: List[StreamingConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingConfigurationTypeDef](./type_defs.md#streamingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProcessorConfigurationTypeDef

```python
# ProcessorConfigurationTypeDef definition

class ProcessorConfigurationTypeDef(TypedDict):
    Lambda: LambdaConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: LambdaConfigurationTypeDef](./type_defs.md#lambdaconfigurationtypedef) 
## ListChannelMessagesRequestRequestTypeDef

```python
# ListChannelMessagesRequestRequestTypeDef definition

class ListChannelMessagesRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    ChimeBearer: str,
    SortOrder: NotRequired[SortOrderType],  # (1)
    NotBefore: NotRequired[TimestampTypeDef],
    NotAfter: NotRequired[TimestampTypeDef],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    SubChannelId: NotRequired[str],
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListSubChannelsResponseTypeDef

```python
# ListSubChannelsResponseTypeDef definition

class ListSubChannelsResponseTypeDef(TypedDict):
    ChannelArn: str,
    SubChannels: List[SubChannelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SubChannelSummaryTypeDef](./type_defs.md#subchannelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchChannelsRequestRequestTypeDef

```python
# SearchChannelsRequestRequestTypeDef definition

class SearchChannelsRequestRequestTypeDef(TypedDict):
    Fields: Sequence[SearchFieldTypeDef],  # (1)
    ChimeBearer: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchFieldTypeDef](./type_defs.md#searchfieldtypedef) 
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
## GetChannelMembershipPreferencesResponseTypeDef

```python
# GetChannelMembershipPreferencesResponseTypeDef definition

class GetChannelMembershipPreferencesResponseTypeDef(TypedDict):
    ChannelArn: str,
    Member: IdentityTypeDef,  # (1)
    Preferences: ChannelMembershipPreferencesTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
2. See [:material-code-braces: ChannelMembershipPreferencesTypeDef](./type_defs.md#channelmembershippreferencestypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutChannelMembershipPreferencesRequestRequestTypeDef

```python
# PutChannelMembershipPreferencesRequestRequestTypeDef definition

class PutChannelMembershipPreferencesRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    MemberArn: str,
    ChimeBearer: str,
    Preferences: ChannelMembershipPreferencesTypeDef,  # (1)
```

1. See [:material-code-braces: ChannelMembershipPreferencesTypeDef](./type_defs.md#channelmembershippreferencestypedef) 
## PutChannelMembershipPreferencesResponseTypeDef

```python
# PutChannelMembershipPreferencesResponseTypeDef definition

class PutChannelMembershipPreferencesResponseTypeDef(TypedDict):
    ChannelArn: str,
    Member: IdentityTypeDef,  # (1)
    Preferences: ChannelMembershipPreferencesTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
2. See [:material-code-braces: ChannelMembershipPreferencesTypeDef](./type_defs.md#channelmembershippreferencestypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChannelMessagesResponseTypeDef

```python
# ListChannelMessagesResponseTypeDef definition

class ListChannelMessagesResponseTypeDef(TypedDict):
    ChannelArn: str,
    ChannelMessages: List[ChannelMessageSummaryTypeDef],  # (1)
    SubChannelId: str,
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
## DescribeChannelResponseTypeDef

```python
# DescribeChannelResponseTypeDef definition

class DescribeChannelResponseTypeDef(TypedDict):
    Channel: ChannelTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProcessorTypeDef

```python
# ProcessorTypeDef definition

class ProcessorTypeDef(TypedDict):
    Name: str,
    Configuration: ProcessorConfigurationTypeDef,  # (1)
    ExecutionOrder: int,
    FallbackAction: FallbackActionType,  # (2)
```

1. See [:material-code-braces: ProcessorConfigurationTypeDef](./type_defs.md#processorconfigurationtypedef) 
2. See [:material-code-brackets: FallbackActionType](./literals.md#fallbackactiontype) 
## ChannelMessageCallbackTypeDef

```python
# ChannelMessageCallbackTypeDef definition

class ChannelMessageCallbackTypeDef(TypedDict):
    MessageId: str,
    Content: NotRequired[str],
    Metadata: NotRequired[str],
    PushNotification: NotRequired[PushNotificationConfigurationTypeDef],  # (1)
    MessageAttributes: NotRequired[Mapping[str, MessageAttributeValueUnionTypeDef]],  # (2)
    SubChannelId: NotRequired[str],
    ContentType: NotRequired[str],
```

1. See [:material-code-braces: PushNotificationConfigurationTypeDef](./type_defs.md#pushnotificationconfigurationtypedef) 
2. See [:material-code-braces: MessageAttributeValueTypeDef](./type_defs.md#messageattributevaluetypedef) [:material-code-braces: MessageAttributeValueOutputTypeDef](./type_defs.md#messageattributevalueoutputtypedef) 
## SendChannelMessageRequestRequestTypeDef

```python
# SendChannelMessageRequestRequestTypeDef definition

class SendChannelMessageRequestRequestTypeDef(TypedDict):
    ChannelArn: str,
    Content: str,
    Type: ChannelMessageTypeType,  # (1)
    Persistence: ChannelMessagePersistenceTypeType,  # (2)
    ClientRequestToken: str,
    ChimeBearer: str,
    Metadata: NotRequired[str],
    PushNotification: NotRequired[PushNotificationConfigurationTypeDef],  # (3)
    MessageAttributes: NotRequired[Mapping[str, MessageAttributeValueUnionTypeDef]],  # (4)
    SubChannelId: NotRequired[str],
    ContentType: NotRequired[str],
    Target: NotRequired[Sequence[TargetTypeDef]],  # (5)
```

1. See [:material-code-brackets: ChannelMessageTypeType](./literals.md#channelmessagetypetype) 
2. See [:material-code-brackets: ChannelMessagePersistenceTypeType](./literals.md#channelmessagepersistencetypetype) 
3. See [:material-code-braces: PushNotificationConfigurationTypeDef](./type_defs.md#pushnotificationconfigurationtypedef) 
4. See [:material-code-braces: MessageAttributeValueTypeDef](./type_defs.md#messageattributevaluetypedef) [:material-code-braces: MessageAttributeValueOutputTypeDef](./type_defs.md#messageattributevalueoutputtypedef) 
5. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
## ChannelFlowSummaryTypeDef

```python
# ChannelFlowSummaryTypeDef definition

class ChannelFlowSummaryTypeDef(TypedDict):
    ChannelFlowArn: NotRequired[str],
    Name: NotRequired[str],
    Processors: NotRequired[List[ProcessorTypeDef]],  # (1)
```

1. See [:material-code-braces: ProcessorTypeDef](./type_defs.md#processortypedef) 
## ChannelFlowTypeDef

```python
# ChannelFlowTypeDef definition

class ChannelFlowTypeDef(TypedDict):
    ChannelFlowArn: NotRequired[str],
    Processors: NotRequired[List[ProcessorTypeDef]],  # (1)
    Name: NotRequired[str],
    CreatedTimestamp: NotRequired[datetime],
    LastUpdatedTimestamp: NotRequired[datetime],
```

1. See [:material-code-braces: ProcessorTypeDef](./type_defs.md#processortypedef) 
## CreateChannelFlowRequestRequestTypeDef

```python
# CreateChannelFlowRequestRequestTypeDef definition

class CreateChannelFlowRequestRequestTypeDef(TypedDict):
    AppInstanceArn: str,
    Processors: Sequence[ProcessorTypeDef],  # (1)
    Name: str,
    ClientRequestToken: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ProcessorTypeDef](./type_defs.md#processortypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateChannelFlowRequestRequestTypeDef

```python
# UpdateChannelFlowRequestRequestTypeDef definition

class UpdateChannelFlowRequestRequestTypeDef(TypedDict):
    ChannelFlowArn: str,
    Processors: Sequence[ProcessorTypeDef],  # (1)
    Name: str,
```

1. See [:material-code-braces: ProcessorTypeDef](./type_defs.md#processortypedef) 
## ChannelFlowCallbackRequestRequestTypeDef

```python
# ChannelFlowCallbackRequestRequestTypeDef definition

class ChannelFlowCallbackRequestRequestTypeDef(TypedDict):
    CallbackId: str,
    ChannelArn: str,
    ChannelMessage: ChannelMessageCallbackTypeDef,  # (1)
    DeleteResource: NotRequired[bool],
```

1. See [:material-code-braces: ChannelMessageCallbackTypeDef](./type_defs.md#channelmessagecallbacktypedef) 
## ListChannelFlowsResponseTypeDef

```python
# ListChannelFlowsResponseTypeDef definition

class ListChannelFlowsResponseTypeDef(TypedDict):
    ChannelFlows: List[ChannelFlowSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ChannelFlowSummaryTypeDef](./type_defs.md#channelflowsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeChannelFlowResponseTypeDef

```python
# DescribeChannelFlowResponseTypeDef definition

class DescribeChannelFlowResponseTypeDef(TypedDict):
    ChannelFlow: ChannelFlowTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelFlowTypeDef](./type_defs.md#channelflowtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
