# ChimeSDKMessaging module

> [Index](../README.md) > ChimeSDKMessaging


!!! note ""

    Auto-generated documentation for [ChimeSDKMessaging](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#chimesdkmessaging)
    type annotations stubs module [types-aiobotocore-chime-sdk-messaging](https://pypi.org/project/types-aiobotocore-chime-sdk-messaging/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ChimeSDKMessaging` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ChimeSDKMessaging` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[chime-sdk-messaging]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[chime-sdk-messaging]'

# standalone installation
python -m pip install types-aiobotocore-chime-sdk-messaging
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-chime-sdk-messaging
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ChimeSDKMessagingClient

Type annotations and code completion for  `#!python session.create_client("chime-sdk-messaging")` as [ChimeSDKMessagingClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client)

```python
# ChimeSDKMessagingClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_chime_sdk_messaging.client import ChimeSDKMessagingClient


session = get_session()
async with session.create_client("chime-sdk-messaging") as client:
    client: ChimeSDKMessagingClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AllowNotificationsType usage example

from types_aiobotocore_chime_sdk_messaging.literals import AllowNotificationsType

def get_value() -> AllowNotificationsType:
    return "ALL"
```

- [AllowNotificationsType](./literals.md#allownotificationstype)
- [ChannelMembershipTypeType](./literals.md#channelmembershiptypetype)
- [ChannelMessagePersistenceTypeType](./literals.md#channelmessagepersistencetypetype)
- [ChannelMessageStatusType](./literals.md#channelmessagestatustype)
- [ChannelMessageTypeType](./literals.md#channelmessagetypetype)
- [ChannelModeType](./literals.md#channelmodetype)
- [ChannelPrivacyType](./literals.md#channelprivacytype)
- [ErrorCodeType](./literals.md#errorcodetype)
- [ExpirationCriterionType](./literals.md#expirationcriteriontype)
- [FallbackActionType](./literals.md#fallbackactiontype)
- [InvocationTypeType](./literals.md#invocationtypetype)
- [MessagingDataTypeType](./literals.md#messagingdatatypetype)
- [PushNotificationTypeType](./literals.md#pushnotificationtypetype)
- [SearchFieldKeyType](./literals.md#searchfieldkeytype)
- [SearchFieldOperatorType](./literals.md#searchfieldoperatortype)
- [SortOrderType](./literals.md#sortordertype)
- [ChimeSDKMessagingServiceName](./literals.md#chimesdkmessagingservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AppInstanceUserMembershipSummaryTypeDef](./type_defs.md#appinstanceusermembershipsummarytypedef)
- [AssociateChannelFlowRequestRequestTypeDef](./type_defs.md#associatechannelflowrequestrequesttypedef)
- [IdentityTypeDef](./type_defs.md#identitytypedef)
- [BatchCreateChannelMembershipErrorTypeDef](./type_defs.md#batchcreatechannelmembershiperrortypedef)
- [BatchCreateChannelMembershipRequestRequestTypeDef](./type_defs.md#batchcreatechannelmembershiprequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ChannelAssociatedWithFlowSummaryTypeDef](./type_defs.md#channelassociatedwithflowsummarytypedef)
- [ChannelSummaryTypeDef](./type_defs.md#channelsummarytypedef)
- [PushNotificationPreferencesTypeDef](./type_defs.md#pushnotificationpreferencestypedef)
- [PushNotificationConfigurationTypeDef](./type_defs.md#pushnotificationconfigurationtypedef)
- [ChannelMessageStatusStructureTypeDef](./type_defs.md#channelmessagestatusstructuretypedef)
- [MessageAttributeValueOutputTypeDef](./type_defs.md#messageattributevalueoutputtypedef)
- [TargetTypeDef](./type_defs.md#targettypedef)
- [ElasticChannelConfigurationTypeDef](./type_defs.md#elasticchannelconfigurationtypedef)
- [ExpirationSettingsTypeDef](./type_defs.md#expirationsettingstypedef)
- [CreateChannelBanRequestRequestTypeDef](./type_defs.md#createchannelbanrequestrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [CreateChannelMembershipRequestRequestTypeDef](./type_defs.md#createchannelmembershiprequestrequesttypedef)
- [CreateChannelModeratorRequestRequestTypeDef](./type_defs.md#createchannelmoderatorrequestrequesttypedef)
- [DeleteChannelBanRequestRequestTypeDef](./type_defs.md#deletechannelbanrequestrequesttypedef)
- [DeleteChannelFlowRequestRequestTypeDef](./type_defs.md#deletechannelflowrequestrequesttypedef)
- [DeleteChannelMembershipRequestRequestTypeDef](./type_defs.md#deletechannelmembershiprequestrequesttypedef)
- [DeleteChannelMessageRequestRequestTypeDef](./type_defs.md#deletechannelmessagerequestrequesttypedef)
- [DeleteChannelModeratorRequestRequestTypeDef](./type_defs.md#deletechannelmoderatorrequestrequesttypedef)
- [DeleteChannelRequestRequestTypeDef](./type_defs.md#deletechannelrequestrequesttypedef)
- [DeleteMessagingStreamingConfigurationsRequestRequestTypeDef](./type_defs.md#deletemessagingstreamingconfigurationsrequestrequesttypedef)
- [DescribeChannelBanRequestRequestTypeDef](./type_defs.md#describechannelbanrequestrequesttypedef)
- [DescribeChannelFlowRequestRequestTypeDef](./type_defs.md#describechannelflowrequestrequesttypedef)
- [DescribeChannelMembershipForAppInstanceUserRequestRequestTypeDef](./type_defs.md#describechannelmembershipforappinstanceuserrequestrequesttypedef)
- [DescribeChannelMembershipRequestRequestTypeDef](./type_defs.md#describechannelmembershiprequestrequesttypedef)
- [DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef](./type_defs.md#describechannelmoderatedbyappinstanceuserrequestrequesttypedef)
- [DescribeChannelModeratorRequestRequestTypeDef](./type_defs.md#describechannelmoderatorrequestrequesttypedef)
- [DescribeChannelRequestRequestTypeDef](./type_defs.md#describechannelrequestrequesttypedef)
- [DisassociateChannelFlowRequestRequestTypeDef](./type_defs.md#disassociatechannelflowrequestrequesttypedef)
- [GetChannelMembershipPreferencesRequestRequestTypeDef](./type_defs.md#getchannelmembershippreferencesrequestrequesttypedef)
- [GetChannelMessageRequestRequestTypeDef](./type_defs.md#getchannelmessagerequestrequesttypedef)
- [GetChannelMessageStatusRequestRequestTypeDef](./type_defs.md#getchannelmessagestatusrequestrequesttypedef)
- [MessagingSessionEndpointTypeDef](./type_defs.md#messagingsessionendpointtypedef)
- [GetMessagingStreamingConfigurationsRequestRequestTypeDef](./type_defs.md#getmessagingstreamingconfigurationsrequestrequesttypedef)
- [StreamingConfigurationTypeDef](./type_defs.md#streamingconfigurationtypedef)
- [LambdaConfigurationTypeDef](./type_defs.md#lambdaconfigurationtypedef)
- [ListChannelBansRequestRequestTypeDef](./type_defs.md#listchannelbansrequestrequesttypedef)
- [ListChannelFlowsRequestRequestTypeDef](./type_defs.md#listchannelflowsrequestrequesttypedef)
- [ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef](./type_defs.md#listchannelmembershipsforappinstanceuserrequestrequesttypedef)
- [ListChannelMembershipsRequestRequestTypeDef](./type_defs.md#listchannelmembershipsrequestrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ListChannelModeratorsRequestRequestTypeDef](./type_defs.md#listchannelmoderatorsrequestrequesttypedef)
- [ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef](./type_defs.md#listchannelsassociatedwithchannelflowrequestrequesttypedef)
- [ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef](./type_defs.md#listchannelsmoderatedbyappinstanceuserrequestrequesttypedef)
- [ListChannelsRequestRequestTypeDef](./type_defs.md#listchannelsrequestrequesttypedef)
- [ListSubChannelsRequestRequestTypeDef](./type_defs.md#listsubchannelsrequestrequesttypedef)
- [SubChannelSummaryTypeDef](./type_defs.md#subchannelsummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [MessageAttributeValueTypeDef](./type_defs.md#messageattributevaluetypedef)
- [RedactChannelMessageRequestRequestTypeDef](./type_defs.md#redactchannelmessagerequestrequesttypedef)
- [SearchFieldTypeDef](./type_defs.md#searchfieldtypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateChannelMessageRequestRequestTypeDef](./type_defs.md#updatechannelmessagerequestrequesttypedef)
- [UpdateChannelReadMarkerRequestRequestTypeDef](./type_defs.md#updatechannelreadmarkerrequestrequesttypedef)
- [UpdateChannelRequestRequestTypeDef](./type_defs.md#updatechannelrequestrequesttypedef)
- [BatchChannelMembershipsTypeDef](./type_defs.md#batchchannelmembershipstypedef)
- [ChannelBanSummaryTypeDef](./type_defs.md#channelbansummarytypedef)
- [ChannelBanTypeDef](./type_defs.md#channelbantypedef)
- [ChannelMembershipSummaryTypeDef](./type_defs.md#channelmembershipsummarytypedef)
- [ChannelMembershipTypeDef](./type_defs.md#channelmembershiptypedef)
- [ChannelModeratorSummaryTypeDef](./type_defs.md#channelmoderatorsummarytypedef)
- [ChannelModeratorTypeDef](./type_defs.md#channelmoderatortypedef)
- [ChannelFlowCallbackResponseTypeDef](./type_defs.md#channelflowcallbackresponsetypedef)
- [CreateChannelBanResponseTypeDef](./type_defs.md#createchannelbanresponsetypedef)
- [CreateChannelFlowResponseTypeDef](./type_defs.md#createchannelflowresponsetypedef)
- [CreateChannelMembershipResponseTypeDef](./type_defs.md#createchannelmembershipresponsetypedef)
- [CreateChannelModeratorResponseTypeDef](./type_defs.md#createchannelmoderatorresponsetypedef)
- [CreateChannelResponseTypeDef](./type_defs.md#createchannelresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [RedactChannelMessageResponseTypeDef](./type_defs.md#redactchannelmessageresponsetypedef)
- [UpdateChannelFlowResponseTypeDef](./type_defs.md#updatechannelflowresponsetypedef)
- [UpdateChannelReadMarkerResponseTypeDef](./type_defs.md#updatechannelreadmarkerresponsetypedef)
- [UpdateChannelResponseTypeDef](./type_defs.md#updatechannelresponsetypedef)
- [ListChannelsAssociatedWithChannelFlowResponseTypeDef](./type_defs.md#listchannelsassociatedwithchannelflowresponsetypedef)
- [ChannelMembershipForAppInstanceUserSummaryTypeDef](./type_defs.md#channelmembershipforappinstanceusersummarytypedef)
- [ChannelModeratedByAppInstanceUserSummaryTypeDef](./type_defs.md#channelmoderatedbyappinstanceusersummarytypedef)
- [ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef)
- [SearchChannelsResponseTypeDef](./type_defs.md#searchchannelsresponsetypedef)
- [ChannelMembershipPreferencesTypeDef](./type_defs.md#channelmembershippreferencestypedef)
- [GetChannelMessageStatusResponseTypeDef](./type_defs.md#getchannelmessagestatusresponsetypedef)
- [SendChannelMessageResponseTypeDef](./type_defs.md#sendchannelmessageresponsetypedef)
- [UpdateChannelMessageResponseTypeDef](./type_defs.md#updatechannelmessageresponsetypedef)
- [ChannelMessageSummaryTypeDef](./type_defs.md#channelmessagesummarytypedef)
- [ChannelMessageTypeDef](./type_defs.md#channelmessagetypedef)
- [ChannelTypeDef](./type_defs.md#channeltypedef)
- [PutChannelExpirationSettingsRequestRequestTypeDef](./type_defs.md#putchannelexpirationsettingsrequestrequesttypedef)
- [PutChannelExpirationSettingsResponseTypeDef](./type_defs.md#putchannelexpirationsettingsresponsetypedef)
- [CreateChannelRequestRequestTypeDef](./type_defs.md#createchannelrequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [GetMessagingSessionEndpointResponseTypeDef](./type_defs.md#getmessagingsessionendpointresponsetypedef)
- [GetMessagingStreamingConfigurationsResponseTypeDef](./type_defs.md#getmessagingstreamingconfigurationsresponsetypedef)
- [PutMessagingStreamingConfigurationsRequestRequestTypeDef](./type_defs.md#putmessagingstreamingconfigurationsrequestrequesttypedef)
- [PutMessagingStreamingConfigurationsResponseTypeDef](./type_defs.md#putmessagingstreamingconfigurationsresponsetypedef)
- [ProcessorConfigurationTypeDef](./type_defs.md#processorconfigurationtypedef)
- [ListChannelMessagesRequestRequestTypeDef](./type_defs.md#listchannelmessagesrequestrequesttypedef)
- [ListSubChannelsResponseTypeDef](./type_defs.md#listsubchannelsresponsetypedef)
- [MessageAttributeValueUnionTypeDef](./type_defs.md#messageattributevalueuniontypedef)
- [SearchChannelsRequestRequestTypeDef](./type_defs.md#searchchannelsrequestrequesttypedef)
- [BatchCreateChannelMembershipResponseTypeDef](./type_defs.md#batchcreatechannelmembershipresponsetypedef)
- [ListChannelBansResponseTypeDef](./type_defs.md#listchannelbansresponsetypedef)
- [DescribeChannelBanResponseTypeDef](./type_defs.md#describechannelbanresponsetypedef)
- [ListChannelMembershipsResponseTypeDef](./type_defs.md#listchannelmembershipsresponsetypedef)
- [DescribeChannelMembershipResponseTypeDef](./type_defs.md#describechannelmembershipresponsetypedef)
- [ListChannelModeratorsResponseTypeDef](./type_defs.md#listchannelmoderatorsresponsetypedef)
- [DescribeChannelModeratorResponseTypeDef](./type_defs.md#describechannelmoderatorresponsetypedef)
- [DescribeChannelMembershipForAppInstanceUserResponseTypeDef](./type_defs.md#describechannelmembershipforappinstanceuserresponsetypedef)
- [ListChannelMembershipsForAppInstanceUserResponseTypeDef](./type_defs.md#listchannelmembershipsforappinstanceuserresponsetypedef)
- [DescribeChannelModeratedByAppInstanceUserResponseTypeDef](./type_defs.md#describechannelmoderatedbyappinstanceuserresponsetypedef)
- [ListChannelsModeratedByAppInstanceUserResponseTypeDef](./type_defs.md#listchannelsmoderatedbyappinstanceuserresponsetypedef)
- [GetChannelMembershipPreferencesResponseTypeDef](./type_defs.md#getchannelmembershippreferencesresponsetypedef)
- [PutChannelMembershipPreferencesRequestRequestTypeDef](./type_defs.md#putchannelmembershippreferencesrequestrequesttypedef)
- [PutChannelMembershipPreferencesResponseTypeDef](./type_defs.md#putchannelmembershippreferencesresponsetypedef)
- [ListChannelMessagesResponseTypeDef](./type_defs.md#listchannelmessagesresponsetypedef)
- [GetChannelMessageResponseTypeDef](./type_defs.md#getchannelmessageresponsetypedef)
- [DescribeChannelResponseTypeDef](./type_defs.md#describechannelresponsetypedef)
- [ProcessorTypeDef](./type_defs.md#processortypedef)
- [ChannelMessageCallbackTypeDef](./type_defs.md#channelmessagecallbacktypedef)
- [SendChannelMessageRequestRequestTypeDef](./type_defs.md#sendchannelmessagerequestrequesttypedef)
- [ChannelFlowSummaryTypeDef](./type_defs.md#channelflowsummarytypedef)
- [ChannelFlowTypeDef](./type_defs.md#channelflowtypedef)
- [CreateChannelFlowRequestRequestTypeDef](./type_defs.md#createchannelflowrequestrequesttypedef)
- [UpdateChannelFlowRequestRequestTypeDef](./type_defs.md#updatechannelflowrequestrequesttypedef)
- [ChannelFlowCallbackRequestRequestTypeDef](./type_defs.md#channelflowcallbackrequestrequesttypedef)
- [ListChannelFlowsResponseTypeDef](./type_defs.md#listchannelflowsresponsetypedef)
- [DescribeChannelFlowResponseTypeDef](./type_defs.md#describechannelflowresponsetypedef)

