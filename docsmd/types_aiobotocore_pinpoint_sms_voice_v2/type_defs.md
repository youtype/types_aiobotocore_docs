# Type definitions

> [Index](../README.md) > [PinpointSMSVoiceV2](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [PinpointSMSVoiceV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
    type annotations stubs module [types-aiobotocore-pinpoint-sms-voice-v2](https://pypi.org/project/types-aiobotocore-pinpoint-sms-voice-v2/).



## AccountAttributeTypeDef

```python
# AccountAttributeTypeDef definition

class AccountAttributeTypeDef(TypedDict):
    Name: AccountAttributeNameType,  # (1)
    Value: str,
```

1. See [:material-code-brackets: AccountAttributeNameType](./literals.md#accountattributenametype) 
## AccountLimitTypeDef

```python
# AccountLimitTypeDef definition

class AccountLimitTypeDef(TypedDict):
    Name: AccountLimitNameType,  # (1)
    Used: int,
    Max: int,
```

1. See [:material-code-brackets: AccountLimitNameType](./literals.md#accountlimitnametype) 
## AssociateOriginationIdentityRequestRequestTypeDef

```python
# AssociateOriginationIdentityRequestRequestTypeDef definition

class AssociateOriginationIdentityRequestRequestTypeDef(TypedDict):
    PoolId: str,
    OriginationIdentity: str,
    IsoCountryCode: str,
    ClientToken: NotRequired[str],
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

## CloudWatchLogsDestinationTypeDef

```python
# CloudWatchLogsDestinationTypeDef definition

class CloudWatchLogsDestinationTypeDef(TypedDict):
    IamRoleArn: str,
    LogGroupArn: str,
```

## ConfigurationSetFilterTypeDef

```python
# ConfigurationSetFilterTypeDef definition

class ConfigurationSetFilterTypeDef(TypedDict):
    Name: ConfigurationSetFilterNameType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: ConfigurationSetFilterNameType](./literals.md#configurationsetfilternametype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## KinesisFirehoseDestinationTypeDef

```python
# KinesisFirehoseDestinationTypeDef definition

class KinesisFirehoseDestinationTypeDef(TypedDict):
    IamRoleArn: str,
    DeliveryStreamArn: str,
```

## SnsDestinationTypeDef

```python
# SnsDestinationTypeDef definition

class SnsDestinationTypeDef(TypedDict):
    TopicArn: str,
```

## DeleteConfigurationSetRequestRequestTypeDef

```python
# DeleteConfigurationSetRequestRequestTypeDef definition

class DeleteConfigurationSetRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
```

## DeleteDefaultMessageTypeRequestRequestTypeDef

```python
# DeleteDefaultMessageTypeRequestRequestTypeDef definition

class DeleteDefaultMessageTypeRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
```

## DeleteDefaultSenderIdRequestRequestTypeDef

```python
# DeleteDefaultSenderIdRequestRequestTypeDef definition

class DeleteDefaultSenderIdRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
```

## DeleteEventDestinationRequestRequestTypeDef

```python
# DeleteEventDestinationRequestRequestTypeDef definition

class DeleteEventDestinationRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    EventDestinationName: str,
```

## DeleteKeywordRequestRequestTypeDef

```python
# DeleteKeywordRequestRequestTypeDef definition

class DeleteKeywordRequestRequestTypeDef(TypedDict):
    OriginationIdentity: str,
    Keyword: str,
```

## DeleteOptOutListRequestRequestTypeDef

```python
# DeleteOptOutListRequestRequestTypeDef definition

class DeleteOptOutListRequestRequestTypeDef(TypedDict):
    OptOutListName: str,
```

## DeleteOptedOutNumberRequestRequestTypeDef

```python
# DeleteOptedOutNumberRequestRequestTypeDef definition

class DeleteOptedOutNumberRequestRequestTypeDef(TypedDict):
    OptOutListName: str,
    OptedOutNumber: str,
```

## DeletePoolRequestRequestTypeDef

```python
# DeletePoolRequestRequestTypeDef definition

class DeletePoolRequestRequestTypeDef(TypedDict):
    PoolId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeAccountAttributesRequestRequestTypeDef

```python
# DescribeAccountAttributesRequestRequestTypeDef definition

class DescribeAccountAttributesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## DescribeAccountLimitsRequestRequestTypeDef

```python
# DescribeAccountLimitsRequestRequestTypeDef definition

class DescribeAccountLimitsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## KeywordFilterTypeDef

```python
# KeywordFilterTypeDef definition

class KeywordFilterTypeDef(TypedDict):
    Name: KeywordFilterNameType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: KeywordFilterNameType](./literals.md#keywordfilternametype) 
## KeywordInformationTypeDef

```python
# KeywordInformationTypeDef definition

class KeywordInformationTypeDef(TypedDict):
    Keyword: str,
    KeywordMessage: str,
    KeywordAction: KeywordActionType,  # (1)
```

1. See [:material-code-brackets: KeywordActionType](./literals.md#keywordactiontype) 
## DescribeOptOutListsRequestRequestTypeDef

```python
# DescribeOptOutListsRequestRequestTypeDef definition

class DescribeOptOutListsRequestRequestTypeDef(TypedDict):
    OptOutListNames: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## OptOutListInformationTypeDef

```python
# OptOutListInformationTypeDef definition

class OptOutListInformationTypeDef(TypedDict):
    OptOutListArn: str,
    OptOutListName: str,
    CreatedTimestamp: datetime,
```

## OptedOutFilterTypeDef

```python
# OptedOutFilterTypeDef definition

class OptedOutFilterTypeDef(TypedDict):
    Name: OptedOutFilterNameType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: OptedOutFilterNameType](./literals.md#optedoutfilternametype) 
## OptedOutNumberInformationTypeDef

```python
# OptedOutNumberInformationTypeDef definition

class OptedOutNumberInformationTypeDef(TypedDict):
    OptedOutNumber: str,
    OptedOutTimestamp: datetime,
    EndUserOptedOut: bool,
```

## PhoneNumberFilterTypeDef

```python
# PhoneNumberFilterTypeDef definition

class PhoneNumberFilterTypeDef(TypedDict):
    Name: PhoneNumberFilterNameType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: PhoneNumberFilterNameType](./literals.md#phonenumberfilternametype) 
## PhoneNumberInformationTypeDef

```python
# PhoneNumberInformationTypeDef definition

class PhoneNumberInformationTypeDef(TypedDict):
    PhoneNumberArn: str,
    PhoneNumber: str,
    Status: NumberStatusType,  # (1)
    IsoCountryCode: str,
    MessageType: MessageTypeType,  # (2)
    NumberCapabilities: List[NumberCapabilityType],  # (3)
    NumberType: NumberTypeType,  # (4)
    MonthlyLeasingPrice: str,
    TwoWayEnabled: bool,
    SelfManagedOptOutsEnabled: bool,
    OptOutListName: str,
    DeletionProtectionEnabled: bool,
    CreatedTimestamp: datetime,
    PhoneNumberId: NotRequired[str],
    TwoWayChannelArn: NotRequired[str],
    PoolId: NotRequired[str],
```

1. See [:material-code-brackets: NumberStatusType](./literals.md#numberstatustype) 
2. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
3. See [:material-code-brackets: NumberCapabilityType](./literals.md#numbercapabilitytype) 
4. See [:material-code-brackets: NumberTypeType](./literals.md#numbertypetype) 
## PoolFilterTypeDef

```python
# PoolFilterTypeDef definition

class PoolFilterTypeDef(TypedDict):
    Name: PoolFilterNameType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: PoolFilterNameType](./literals.md#poolfilternametype) 
## PoolInformationTypeDef

```python
# PoolInformationTypeDef definition

class PoolInformationTypeDef(TypedDict):
    PoolArn: str,
    PoolId: str,
    Status: PoolStatusType,  # (1)
    MessageType: MessageTypeType,  # (2)
    TwoWayEnabled: bool,
    SelfManagedOptOutsEnabled: bool,
    OptOutListName: str,
    SharedRoutesEnabled: bool,
    DeletionProtectionEnabled: bool,
    CreatedTimestamp: datetime,
    TwoWayChannelArn: NotRequired[str],
```

1. See [:material-code-brackets: PoolStatusType](./literals.md#poolstatustype) 
2. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
## SenderIdAndCountryTypeDef

```python
# SenderIdAndCountryTypeDef definition

class SenderIdAndCountryTypeDef(TypedDict):
    SenderId: str,
    IsoCountryCode: str,
```

## SenderIdFilterTypeDef

```python
# SenderIdFilterTypeDef definition

class SenderIdFilterTypeDef(TypedDict):
    Name: SenderIdFilterNameType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: SenderIdFilterNameType](./literals.md#senderidfilternametype) 
## SenderIdInformationTypeDef

```python
# SenderIdInformationTypeDef definition

class SenderIdInformationTypeDef(TypedDict):
    SenderIdArn: str,
    SenderId: str,
    IsoCountryCode: str,
    MessageTypes: List[MessageTypeType],  # (1)
    MonthlyLeasingPrice: str,
```

1. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
## DescribeSpendLimitsRequestRequestTypeDef

```python
# DescribeSpendLimitsRequestRequestTypeDef definition

class DescribeSpendLimitsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## SpendLimitTypeDef

```python
# SpendLimitTypeDef definition

class SpendLimitTypeDef(TypedDict):
    Name: SpendLimitNameType,  # (1)
    EnforcedLimit: int,
    MaxLimit: int,
    Overridden: bool,
```

1. See [:material-code-brackets: SpendLimitNameType](./literals.md#spendlimitnametype) 
## DisassociateOriginationIdentityRequestRequestTypeDef

```python
# DisassociateOriginationIdentityRequestRequestTypeDef definition

class DisassociateOriginationIdentityRequestRequestTypeDef(TypedDict):
    PoolId: str,
    OriginationIdentity: str,
    IsoCountryCode: str,
    ClientToken: NotRequired[str],
```

## PoolOriginationIdentitiesFilterTypeDef

```python
# PoolOriginationIdentitiesFilterTypeDef definition

class PoolOriginationIdentitiesFilterTypeDef(TypedDict):
    Name: PoolOriginationIdentitiesFilterNameType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: PoolOriginationIdentitiesFilterNameType](./literals.md#pooloriginationidentitiesfilternametype) 
## OriginationIdentityMetadataTypeDef

```python
# OriginationIdentityMetadataTypeDef definition

class OriginationIdentityMetadataTypeDef(TypedDict):
    OriginationIdentityArn: str,
    OriginationIdentity: str,
    IsoCountryCode: str,
    NumberCapabilities: List[NumberCapabilityType],  # (1)
```

1. See [:material-code-brackets: NumberCapabilityType](./literals.md#numbercapabilitytype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## PutKeywordRequestRequestTypeDef

```python
# PutKeywordRequestRequestTypeDef definition

class PutKeywordRequestRequestTypeDef(TypedDict):
    OriginationIdentity: str,
    Keyword: str,
    KeywordMessage: str,
    KeywordAction: NotRequired[KeywordActionType],  # (1)
```

1. See [:material-code-brackets: KeywordActionType](./literals.md#keywordactiontype) 
## PutOptedOutNumberRequestRequestTypeDef

```python
# PutOptedOutNumberRequestRequestTypeDef definition

class PutOptedOutNumberRequestRequestTypeDef(TypedDict):
    OptOutListName: str,
    OptedOutNumber: str,
```

## ReleasePhoneNumberRequestRequestTypeDef

```python
# ReleasePhoneNumberRequestRequestTypeDef definition

class ReleasePhoneNumberRequestRequestTypeDef(TypedDict):
    PhoneNumberId: str,
```

## SendTextMessageRequestRequestTypeDef

```python
# SendTextMessageRequestRequestTypeDef definition

class SendTextMessageRequestRequestTypeDef(TypedDict):
    DestinationPhoneNumber: str,
    OriginationIdentity: NotRequired[str],
    MessageBody: NotRequired[str],
    MessageType: NotRequired[MessageTypeType],  # (1)
    Keyword: NotRequired[str],
    ConfigurationSetName: NotRequired[str],
    MaxPrice: NotRequired[str],
    TimeToLive: NotRequired[int],
    Context: NotRequired[Mapping[str, str]],
    DestinationCountryParameters: NotRequired[Mapping[DestinationCountryParameterKeyType, str]],  # (2)
    DryRun: NotRequired[bool],
```

1. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
2. See [:material-code-brackets: DestinationCountryParameterKeyType](./literals.md#destinationcountryparameterkeytype) 
## SendVoiceMessageRequestRequestTypeDef

```python
# SendVoiceMessageRequestRequestTypeDef definition

class SendVoiceMessageRequestRequestTypeDef(TypedDict):
    DestinationPhoneNumber: str,
    OriginationIdentity: str,
    MessageBody: NotRequired[str],
    MessageBodyTextType: NotRequired[VoiceMessageBodyTextTypeType],  # (1)
    VoiceId: NotRequired[VoiceIdType],  # (2)
    ConfigurationSetName: NotRequired[str],
    MaxPricePerMinute: NotRequired[str],
    TimeToLive: NotRequired[int],
    Context: NotRequired[Mapping[str, str]],
    DryRun: NotRequired[bool],
```

1. See [:material-code-brackets: VoiceMessageBodyTextTypeType](./literals.md#voicemessagebodytexttypetype) 
2. See [:material-code-brackets: VoiceIdType](./literals.md#voiceidtype) 
## SetDefaultMessageTypeRequestRequestTypeDef

```python
# SetDefaultMessageTypeRequestRequestTypeDef definition

class SetDefaultMessageTypeRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    MessageType: MessageTypeType,  # (1)
```

1. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
## SetDefaultSenderIdRequestRequestTypeDef

```python
# SetDefaultSenderIdRequestRequestTypeDef definition

class SetDefaultSenderIdRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    SenderId: str,
```

## SetTextMessageSpendLimitOverrideRequestRequestTypeDef

```python
# SetTextMessageSpendLimitOverrideRequestRequestTypeDef definition

class SetTextMessageSpendLimitOverrideRequestRequestTypeDef(TypedDict):
    MonthlyLimit: int,
```

## SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef

```python
# SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef definition

class SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef(TypedDict):
    MonthlyLimit: int,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdatePhoneNumberRequestRequestTypeDef

```python
# UpdatePhoneNumberRequestRequestTypeDef definition

class UpdatePhoneNumberRequestRequestTypeDef(TypedDict):
    PhoneNumberId: str,
    TwoWayEnabled: NotRequired[bool],
    TwoWayChannelArn: NotRequired[str],
    SelfManagedOptOutsEnabled: NotRequired[bool],
    OptOutListName: NotRequired[str],
    DeletionProtectionEnabled: NotRequired[bool],
```

## UpdatePoolRequestRequestTypeDef

```python
# UpdatePoolRequestRequestTypeDef definition

class UpdatePoolRequestRequestTypeDef(TypedDict):
    PoolId: str,
    TwoWayEnabled: NotRequired[bool],
    TwoWayChannelArn: NotRequired[str],
    SelfManagedOptOutsEnabled: NotRequired[bool],
    OptOutListName: NotRequired[str],
    SharedRoutesEnabled: NotRequired[bool],
    DeletionProtectionEnabled: NotRequired[bool],
```

## AssociateOriginationIdentityResultTypeDef

```python
# AssociateOriginationIdentityResultTypeDef definition

class AssociateOriginationIdentityResultTypeDef(TypedDict):
    PoolArn: str,
    PoolId: str,
    OriginationIdentityArn: str,
    OriginationIdentity: str,
    IsoCountryCode: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDefaultMessageTypeResultTypeDef

```python
# DeleteDefaultMessageTypeResultTypeDef definition

class DeleteDefaultMessageTypeResultTypeDef(TypedDict):
    ConfigurationSetArn: str,
    ConfigurationSetName: str,
    MessageType: MessageTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDefaultSenderIdResultTypeDef

```python
# DeleteDefaultSenderIdResultTypeDef definition

class DeleteDefaultSenderIdResultTypeDef(TypedDict):
    ConfigurationSetArn: str,
    ConfigurationSetName: str,
    SenderId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteKeywordResultTypeDef

```python
# DeleteKeywordResultTypeDef definition

class DeleteKeywordResultTypeDef(TypedDict):
    OriginationIdentityArn: str,
    OriginationIdentity: str,
    Keyword: str,
    KeywordMessage: str,
    KeywordAction: KeywordActionType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: KeywordActionType](./literals.md#keywordactiontype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteOptOutListResultTypeDef

```python
# DeleteOptOutListResultTypeDef definition

class DeleteOptOutListResultTypeDef(TypedDict):
    OptOutListArn: str,
    OptOutListName: str,
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteOptedOutNumberResultTypeDef

```python
# DeleteOptedOutNumberResultTypeDef definition

class DeleteOptedOutNumberResultTypeDef(TypedDict):
    OptOutListArn: str,
    OptOutListName: str,
    OptedOutNumber: str,
    OptedOutTimestamp: datetime,
    EndUserOptedOut: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePoolResultTypeDef

```python
# DeletePoolResultTypeDef definition

class DeletePoolResultTypeDef(TypedDict):
    PoolArn: str,
    PoolId: str,
    Status: PoolStatusType,  # (1)
    MessageType: MessageTypeType,  # (2)
    TwoWayEnabled: bool,
    TwoWayChannelArn: str,
    SelfManagedOptOutsEnabled: bool,
    OptOutListName: str,
    SharedRoutesEnabled: bool,
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: PoolStatusType](./literals.md#poolstatustype) 
2. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTextMessageSpendLimitOverrideResultTypeDef

```python
# DeleteTextMessageSpendLimitOverrideResultTypeDef definition

class DeleteTextMessageSpendLimitOverrideResultTypeDef(TypedDict):
    MonthlyLimit: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteVoiceMessageSpendLimitOverrideResultTypeDef

```python
# DeleteVoiceMessageSpendLimitOverrideResultTypeDef definition

class DeleteVoiceMessageSpendLimitOverrideResultTypeDef(TypedDict):
    MonthlyLimit: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountAttributesResultTypeDef

```python
# DescribeAccountAttributesResultTypeDef definition

class DescribeAccountAttributesResultTypeDef(TypedDict):
    AccountAttributes: List[AccountAttributeTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountAttributeTypeDef](./type_defs.md#accountattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountLimitsResultTypeDef

```python
# DescribeAccountLimitsResultTypeDef definition

class DescribeAccountLimitsResultTypeDef(TypedDict):
    AccountLimits: List[AccountLimitTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountLimitTypeDef](./type_defs.md#accountlimittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateOriginationIdentityResultTypeDef

```python
# DisassociateOriginationIdentityResultTypeDef definition

class DisassociateOriginationIdentityResultTypeDef(TypedDict):
    PoolArn: str,
    PoolId: str,
    OriginationIdentityArn: str,
    OriginationIdentity: str,
    IsoCountryCode: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutKeywordResultTypeDef

```python
# PutKeywordResultTypeDef definition

class PutKeywordResultTypeDef(TypedDict):
    OriginationIdentityArn: str,
    OriginationIdentity: str,
    Keyword: str,
    KeywordMessage: str,
    KeywordAction: KeywordActionType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: KeywordActionType](./literals.md#keywordactiontype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutOptedOutNumberResultTypeDef

```python
# PutOptedOutNumberResultTypeDef definition

class PutOptedOutNumberResultTypeDef(TypedDict):
    OptOutListArn: str,
    OptOutListName: str,
    OptedOutNumber: str,
    OptedOutTimestamp: datetime,
    EndUserOptedOut: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReleasePhoneNumberResultTypeDef

```python
# ReleasePhoneNumberResultTypeDef definition

class ReleasePhoneNumberResultTypeDef(TypedDict):
    PhoneNumberArn: str,
    PhoneNumberId: str,
    PhoneNumber: str,
    Status: NumberStatusType,  # (1)
    IsoCountryCode: str,
    MessageType: MessageTypeType,  # (2)
    NumberCapabilities: List[NumberCapabilityType],  # (3)
    NumberType: NumberTypeType,  # (4)
    MonthlyLeasingPrice: str,
    TwoWayEnabled: bool,
    TwoWayChannelArn: str,
    SelfManagedOptOutsEnabled: bool,
    OptOutListName: str,
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: NumberStatusType](./literals.md#numberstatustype) 
2. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
3. See [:material-code-brackets: NumberCapabilityType](./literals.md#numbercapabilitytype) 
4. See [:material-code-brackets: NumberTypeType](./literals.md#numbertypetype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendTextMessageResultTypeDef

```python
# SendTextMessageResultTypeDef definition

class SendTextMessageResultTypeDef(TypedDict):
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendVoiceMessageResultTypeDef

```python
# SendVoiceMessageResultTypeDef definition

class SendVoiceMessageResultTypeDef(TypedDict):
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetDefaultMessageTypeResultTypeDef

```python
# SetDefaultMessageTypeResultTypeDef definition

class SetDefaultMessageTypeResultTypeDef(TypedDict):
    ConfigurationSetArn: str,
    ConfigurationSetName: str,
    MessageType: MessageTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetDefaultSenderIdResultTypeDef

```python
# SetDefaultSenderIdResultTypeDef definition

class SetDefaultSenderIdResultTypeDef(TypedDict):
    ConfigurationSetArn: str,
    ConfigurationSetName: str,
    SenderId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetTextMessageSpendLimitOverrideResultTypeDef

```python
# SetTextMessageSpendLimitOverrideResultTypeDef definition

class SetTextMessageSpendLimitOverrideResultTypeDef(TypedDict):
    MonthlyLimit: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetVoiceMessageSpendLimitOverrideResultTypeDef

```python
# SetVoiceMessageSpendLimitOverrideResultTypeDef definition

class SetVoiceMessageSpendLimitOverrideResultTypeDef(TypedDict):
    MonthlyLimit: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePhoneNumberResultTypeDef

```python
# UpdatePhoneNumberResultTypeDef definition

class UpdatePhoneNumberResultTypeDef(TypedDict):
    PhoneNumberArn: str,
    PhoneNumberId: str,
    PhoneNumber: str,
    Status: NumberStatusType,  # (1)
    IsoCountryCode: str,
    MessageType: MessageTypeType,  # (2)
    NumberCapabilities: List[NumberCapabilityType],  # (3)
    NumberType: NumberTypeType,  # (4)
    MonthlyLeasingPrice: str,
    TwoWayEnabled: bool,
    TwoWayChannelArn: str,
    SelfManagedOptOutsEnabled: bool,
    OptOutListName: str,
    DeletionProtectionEnabled: bool,
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: NumberStatusType](./literals.md#numberstatustype) 
2. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
3. See [:material-code-brackets: NumberCapabilityType](./literals.md#numbercapabilitytype) 
4. See [:material-code-brackets: NumberTypeType](./literals.md#numbertypetype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePoolResultTypeDef

```python
# UpdatePoolResultTypeDef definition

class UpdatePoolResultTypeDef(TypedDict):
    PoolArn: str,
    PoolId: str,
    Status: PoolStatusType,  # (1)
    MessageType: MessageTypeType,  # (2)
    TwoWayEnabled: bool,
    TwoWayChannelArn: str,
    SelfManagedOptOutsEnabled: bool,
    OptOutListName: str,
    SharedRoutesEnabled: bool,
    DeletionProtectionEnabled: bool,
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: PoolStatusType](./literals.md#poolstatustype) 
2. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeConfigurationSetsRequestRequestTypeDef

```python
# DescribeConfigurationSetsRequestRequestTypeDef definition

class DescribeConfigurationSetsRequestRequestTypeDef(TypedDict):
    ConfigurationSetNames: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[ConfigurationSetFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ConfigurationSetFilterTypeDef](./type_defs.md#configurationsetfiltertypedef) 
## CreateConfigurationSetRequestRequestTypeDef

```python
# CreateConfigurationSetRequestRequestTypeDef definition

class CreateConfigurationSetRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateConfigurationSetResultTypeDef

```python
# CreateConfigurationSetResultTypeDef definition

class CreateConfigurationSetResultTypeDef(TypedDict):
    ConfigurationSetArn: str,
    ConfigurationSetName: str,
    Tags: List[TagTypeDef],  # (1)
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateOptOutListRequestRequestTypeDef

```python
# CreateOptOutListRequestRequestTypeDef definition

class CreateOptOutListRequestRequestTypeDef(TypedDict):
    OptOutListName: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateOptOutListResultTypeDef

```python
# CreateOptOutListResultTypeDef definition

class CreateOptOutListResultTypeDef(TypedDict):
    OptOutListArn: str,
    OptOutListName: str,
    Tags: List[TagTypeDef],  # (1)
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePoolRequestRequestTypeDef

```python
# CreatePoolRequestRequestTypeDef definition

class CreatePoolRequestRequestTypeDef(TypedDict):
    OriginationIdentity: str,
    IsoCountryCode: str,
    MessageType: MessageTypeType,  # (1)
    DeletionProtectionEnabled: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    ClientToken: NotRequired[str],
```

1. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePoolResultTypeDef

```python
# CreatePoolResultTypeDef definition

class CreatePoolResultTypeDef(TypedDict):
    PoolArn: str,
    PoolId: str,
    Status: PoolStatusType,  # (1)
    MessageType: MessageTypeType,  # (2)
    TwoWayEnabled: bool,
    TwoWayChannelArn: str,
    SelfManagedOptOutsEnabled: bool,
    OptOutListName: str,
    SharedRoutesEnabled: bool,
    DeletionProtectionEnabled: bool,
    Tags: List[TagTypeDef],  # (3)
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: PoolStatusType](./literals.md#poolstatustype) 
2. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResultTypeDef

```python
# ListTagsForResourceResultTypeDef definition

class ListTagsForResourceResultTypeDef(TypedDict):
    ResourceArn: str,
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RequestPhoneNumberRequestRequestTypeDef

```python
# RequestPhoneNumberRequestRequestTypeDef definition

class RequestPhoneNumberRequestRequestTypeDef(TypedDict):
    IsoCountryCode: str,
    MessageType: MessageTypeType,  # (1)
    NumberCapabilities: Sequence[NumberCapabilityType],  # (2)
    NumberType: RequestableNumberTypeType,  # (3)
    OptOutListName: NotRequired[str],
    PoolId: NotRequired[str],
    RegistrationId: NotRequired[str],
    DeletionProtectionEnabled: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    ClientToken: NotRequired[str],
```

1. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
2. See [:material-code-brackets: NumberCapabilityType](./literals.md#numbercapabilitytype) 
3. See [:material-code-brackets: RequestableNumberTypeType](./literals.md#requestablenumbertypetype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## RequestPhoneNumberResultTypeDef

```python
# RequestPhoneNumberResultTypeDef definition

class RequestPhoneNumberResultTypeDef(TypedDict):
    PhoneNumberArn: str,
    PhoneNumberId: str,
    PhoneNumber: str,
    Status: NumberStatusType,  # (1)
    IsoCountryCode: str,
    MessageType: MessageTypeType,  # (2)
    NumberCapabilities: List[NumberCapabilityType],  # (3)
    NumberType: RequestableNumberTypeType,  # (4)
    MonthlyLeasingPrice: str,
    TwoWayEnabled: bool,
    TwoWayChannelArn: str,
    SelfManagedOptOutsEnabled: bool,
    OptOutListName: str,
    DeletionProtectionEnabled: bool,
    PoolId: str,
    Tags: List[TagTypeDef],  # (5)
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: NumberStatusType](./literals.md#numberstatustype) 
2. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
3. See [:material-code-brackets: NumberCapabilityType](./literals.md#numbercapabilitytype) 
4. See [:material-code-brackets: RequestableNumberTypeType](./literals.md#requestablenumbertypetype) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateEventDestinationRequestRequestTypeDef

```python
# CreateEventDestinationRequestRequestTypeDef definition

class CreateEventDestinationRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    EventDestinationName: str,
    MatchingEventTypes: Sequence[EventTypeType],  # (1)
    CloudWatchLogsDestination: NotRequired[CloudWatchLogsDestinationTypeDef],  # (2)
    KinesisFirehoseDestination: NotRequired[KinesisFirehoseDestinationTypeDef],  # (3)
    SnsDestination: NotRequired[SnsDestinationTypeDef],  # (4)
    ClientToken: NotRequired[str],
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
2. See [:material-code-braces: CloudWatchLogsDestinationTypeDef](./type_defs.md#cloudwatchlogsdestinationtypedef) 
3. See [:material-code-braces: KinesisFirehoseDestinationTypeDef](./type_defs.md#kinesisfirehosedestinationtypedef) 
4. See [:material-code-braces: SnsDestinationTypeDef](./type_defs.md#snsdestinationtypedef) 
## EventDestinationTypeDef

```python
# EventDestinationTypeDef definition

class EventDestinationTypeDef(TypedDict):
    EventDestinationName: str,
    Enabled: bool,
    MatchingEventTypes: List[EventTypeType],  # (1)
    CloudWatchLogsDestination: NotRequired[CloudWatchLogsDestinationTypeDef],  # (2)
    KinesisFirehoseDestination: NotRequired[KinesisFirehoseDestinationTypeDef],  # (3)
    SnsDestination: NotRequired[SnsDestinationTypeDef],  # (4)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
2. See [:material-code-braces: CloudWatchLogsDestinationTypeDef](./type_defs.md#cloudwatchlogsdestinationtypedef) 
3. See [:material-code-braces: KinesisFirehoseDestinationTypeDef](./type_defs.md#kinesisfirehosedestinationtypedef) 
4. See [:material-code-braces: SnsDestinationTypeDef](./type_defs.md#snsdestinationtypedef) 
## UpdateEventDestinationRequestRequestTypeDef

```python
# UpdateEventDestinationRequestRequestTypeDef definition

class UpdateEventDestinationRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    EventDestinationName: str,
    Enabled: NotRequired[bool],
    MatchingEventTypes: NotRequired[Sequence[EventTypeType]],  # (1)
    CloudWatchLogsDestination: NotRequired[CloudWatchLogsDestinationTypeDef],  # (2)
    KinesisFirehoseDestination: NotRequired[KinesisFirehoseDestinationTypeDef],  # (3)
    SnsDestination: NotRequired[SnsDestinationTypeDef],  # (4)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
2. See [:material-code-braces: CloudWatchLogsDestinationTypeDef](./type_defs.md#cloudwatchlogsdestinationtypedef) 
3. See [:material-code-braces: KinesisFirehoseDestinationTypeDef](./type_defs.md#kinesisfirehosedestinationtypedef) 
4. See [:material-code-braces: SnsDestinationTypeDef](./type_defs.md#snsdestinationtypedef) 
## DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef

```python
# DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef definition

class DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef

```python
# DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef definition

class DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef

```python
# DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef definition

class DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef(TypedDict):
    ConfigurationSetNames: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[ConfigurationSetFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ConfigurationSetFilterTypeDef](./type_defs.md#configurationsetfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef

```python
# DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef definition

class DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef(TypedDict):
    OptOutListNames: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef

```python
# DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef definition

class DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef

```python
# DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef definition

class DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef(TypedDict):
    OriginationIdentity: str,
    Keywords: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[KeywordFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: KeywordFilterTypeDef](./type_defs.md#keywordfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeKeywordsRequestRequestTypeDef

```python
# DescribeKeywordsRequestRequestTypeDef definition

class DescribeKeywordsRequestRequestTypeDef(TypedDict):
    OriginationIdentity: str,
    Keywords: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[KeywordFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: KeywordFilterTypeDef](./type_defs.md#keywordfiltertypedef) 
## DescribeKeywordsResultTypeDef

```python
# DescribeKeywordsResultTypeDef definition

class DescribeKeywordsResultTypeDef(TypedDict):
    OriginationIdentityArn: str,
    OriginationIdentity: str,
    Keywords: List[KeywordInformationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KeywordInformationTypeDef](./type_defs.md#keywordinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOptOutListsResultTypeDef

```python
# DescribeOptOutListsResultTypeDef definition

class DescribeOptOutListsResultTypeDef(TypedDict):
    OptOutLists: List[OptOutListInformationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OptOutListInformationTypeDef](./type_defs.md#optoutlistinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef

```python
# DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef definition

class DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef(TypedDict):
    OptOutListName: str,
    OptedOutNumbers: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[OptedOutFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: OptedOutFilterTypeDef](./type_defs.md#optedoutfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeOptedOutNumbersRequestRequestTypeDef

```python
# DescribeOptedOutNumbersRequestRequestTypeDef definition

class DescribeOptedOutNumbersRequestRequestTypeDef(TypedDict):
    OptOutListName: str,
    OptedOutNumbers: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[OptedOutFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: OptedOutFilterTypeDef](./type_defs.md#optedoutfiltertypedef) 
## DescribeOptedOutNumbersResultTypeDef

```python
# DescribeOptedOutNumbersResultTypeDef definition

class DescribeOptedOutNumbersResultTypeDef(TypedDict):
    OptOutListArn: str,
    OptOutListName: str,
    OptedOutNumbers: List[OptedOutNumberInformationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OptedOutNumberInformationTypeDef](./type_defs.md#optedoutnumberinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePhoneNumbersRequestDescribePhoneNumbersPaginateTypeDef

```python
# DescribePhoneNumbersRequestDescribePhoneNumbersPaginateTypeDef definition

class DescribePhoneNumbersRequestDescribePhoneNumbersPaginateTypeDef(TypedDict):
    PhoneNumberIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[PhoneNumberFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: PhoneNumberFilterTypeDef](./type_defs.md#phonenumberfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribePhoneNumbersRequestRequestTypeDef

```python
# DescribePhoneNumbersRequestRequestTypeDef definition

class DescribePhoneNumbersRequestRequestTypeDef(TypedDict):
    PhoneNumberIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[PhoneNumberFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: PhoneNumberFilterTypeDef](./type_defs.md#phonenumberfiltertypedef) 
## DescribePhoneNumbersResultTypeDef

```python
# DescribePhoneNumbersResultTypeDef definition

class DescribePhoneNumbersResultTypeDef(TypedDict):
    PhoneNumbers: List[PhoneNumberInformationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberInformationTypeDef](./type_defs.md#phonenumberinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePoolsRequestDescribePoolsPaginateTypeDef

```python
# DescribePoolsRequestDescribePoolsPaginateTypeDef definition

class DescribePoolsRequestDescribePoolsPaginateTypeDef(TypedDict):
    PoolIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[PoolFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: PoolFilterTypeDef](./type_defs.md#poolfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribePoolsRequestRequestTypeDef

```python
# DescribePoolsRequestRequestTypeDef definition

class DescribePoolsRequestRequestTypeDef(TypedDict):
    PoolIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[PoolFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: PoolFilterTypeDef](./type_defs.md#poolfiltertypedef) 
## DescribePoolsResultTypeDef

```python
# DescribePoolsResultTypeDef definition

class DescribePoolsResultTypeDef(TypedDict):
    Pools: List[PoolInformationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PoolInformationTypeDef](./type_defs.md#poolinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef

```python
# DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef definition

class DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef(TypedDict):
    SenderIds: NotRequired[Sequence[SenderIdAndCountryTypeDef]],  # (1)
    Filters: NotRequired[Sequence[SenderIdFilterTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: SenderIdAndCountryTypeDef](./type_defs.md#senderidandcountrytypedef) 
2. See [:material-code-braces: SenderIdFilterTypeDef](./type_defs.md#senderidfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSenderIdsRequestRequestTypeDef

```python
# DescribeSenderIdsRequestRequestTypeDef definition

class DescribeSenderIdsRequestRequestTypeDef(TypedDict):
    SenderIds: NotRequired[Sequence[SenderIdAndCountryTypeDef]],  # (1)
    Filters: NotRequired[Sequence[SenderIdFilterTypeDef]],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: SenderIdAndCountryTypeDef](./type_defs.md#senderidandcountrytypedef) 
2. See [:material-code-braces: SenderIdFilterTypeDef](./type_defs.md#senderidfiltertypedef) 
## DescribeSenderIdsResultTypeDef

```python
# DescribeSenderIdsResultTypeDef definition

class DescribeSenderIdsResultTypeDef(TypedDict):
    SenderIds: List[SenderIdInformationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SenderIdInformationTypeDef](./type_defs.md#senderidinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSpendLimitsResultTypeDef

```python
# DescribeSpendLimitsResultTypeDef definition

class DescribeSpendLimitsResultTypeDef(TypedDict):
    SpendLimits: List[SpendLimitTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SpendLimitTypeDef](./type_defs.md#spendlimittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef

```python
# ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef definition

class ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef(TypedDict):
    PoolId: str,
    Filters: NotRequired[Sequence[PoolOriginationIdentitiesFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: PoolOriginationIdentitiesFilterTypeDef](./type_defs.md#pooloriginationidentitiesfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPoolOriginationIdentitiesRequestRequestTypeDef

```python
# ListPoolOriginationIdentitiesRequestRequestTypeDef definition

class ListPoolOriginationIdentitiesRequestRequestTypeDef(TypedDict):
    PoolId: str,
    Filters: NotRequired[Sequence[PoolOriginationIdentitiesFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: PoolOriginationIdentitiesFilterTypeDef](./type_defs.md#pooloriginationidentitiesfiltertypedef) 
## ListPoolOriginationIdentitiesResultTypeDef

```python
# ListPoolOriginationIdentitiesResultTypeDef definition

class ListPoolOriginationIdentitiesResultTypeDef(TypedDict):
    PoolArn: str,
    PoolId: str,
    OriginationIdentities: List[OriginationIdentityMetadataTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OriginationIdentityMetadataTypeDef](./type_defs.md#originationidentitymetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfigurationSetInformationTypeDef

```python
# ConfigurationSetInformationTypeDef definition

class ConfigurationSetInformationTypeDef(TypedDict):
    ConfigurationSetArn: str,
    ConfigurationSetName: str,
    EventDestinations: List[EventDestinationTypeDef],  # (1)
    CreatedTimestamp: datetime,
    DefaultMessageType: NotRequired[MessageTypeType],  # (2)
    DefaultSenderId: NotRequired[str],
```

1. See [:material-code-braces: EventDestinationTypeDef](./type_defs.md#eventdestinationtypedef) 
2. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
## CreateEventDestinationResultTypeDef

```python
# CreateEventDestinationResultTypeDef definition

class CreateEventDestinationResultTypeDef(TypedDict):
    ConfigurationSetArn: str,
    ConfigurationSetName: str,
    EventDestination: EventDestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventDestinationTypeDef](./type_defs.md#eventdestinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteConfigurationSetResultTypeDef

```python
# DeleteConfigurationSetResultTypeDef definition

class DeleteConfigurationSetResultTypeDef(TypedDict):
    ConfigurationSetArn: str,
    ConfigurationSetName: str,
    EventDestinations: List[EventDestinationTypeDef],  # (1)
    DefaultMessageType: MessageTypeType,  # (2)
    DefaultSenderId: str,
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: EventDestinationTypeDef](./type_defs.md#eventdestinationtypedef) 
2. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteEventDestinationResultTypeDef

```python
# DeleteEventDestinationResultTypeDef definition

class DeleteEventDestinationResultTypeDef(TypedDict):
    ConfigurationSetArn: str,
    ConfigurationSetName: str,
    EventDestination: EventDestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventDestinationTypeDef](./type_defs.md#eventdestinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEventDestinationResultTypeDef

```python
# UpdateEventDestinationResultTypeDef definition

class UpdateEventDestinationResultTypeDef(TypedDict):
    ConfigurationSetArn: str,
    ConfigurationSetName: str,
    EventDestination: EventDestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventDestinationTypeDef](./type_defs.md#eventdestinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeConfigurationSetsResultTypeDef

```python
# DescribeConfigurationSetsResultTypeDef definition

class DescribeConfigurationSetsResultTypeDef(TypedDict):
    ConfigurationSets: List[ConfigurationSetInformationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfigurationSetInformationTypeDef](./type_defs.md#configurationsetinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
