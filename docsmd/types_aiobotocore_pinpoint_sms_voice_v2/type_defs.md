# Type definitions

> [Index](../README.md) > [PinpointSMSVoiceV2](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [PinpointSMSVoiceV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#pinpointsmsvoicev2)
    type annotations stubs module [types-aiobotocore-pinpoint-sms-voice-v2](https://pypi.org/project/types-aiobotocore-pinpoint-sms-voice-v2/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




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
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## AssociateProtectConfigurationRequestRequestTypeDef

```python
# AssociateProtectConfigurationRequestRequestTypeDef definition

class AssociateProtectConfigurationRequestRequestTypeDef(TypedDict):
    ProtectConfigurationId: str,
    ConfigurationSetName: str,
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

## CreateRegistrationAssociationRequestRequestTypeDef

```python
# CreateRegistrationAssociationRequestRequestTypeDef definition

class CreateRegistrationAssociationRequestRequestTypeDef(TypedDict):
    RegistrationId: str,
    ResourceId: str,
```

## CreateRegistrationVersionRequestRequestTypeDef

```python
# CreateRegistrationVersionRequestRequestTypeDef definition

class CreateRegistrationVersionRequestRequestTypeDef(TypedDict):
    RegistrationId: str,
```

## RegistrationVersionStatusHistoryTypeDef

```python
# RegistrationVersionStatusHistoryTypeDef definition

class RegistrationVersionStatusHistoryTypeDef(TypedDict):
    DraftTimestamp: datetime,
    SubmittedTimestamp: NotRequired[datetime],
    ReviewingTimestamp: NotRequired[datetime],
    RequiresAuthenticationTimestamp: NotRequired[datetime],
    ApprovedTimestamp: NotRequired[datetime],
    DiscardedTimestamp: NotRequired[datetime],
    DeniedTimestamp: NotRequired[datetime],
    RevokedTimestamp: NotRequired[datetime],
    ArchivedTimestamp: NotRequired[datetime],
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

## DeleteProtectConfigurationRequestRequestTypeDef

```python
# DeleteProtectConfigurationRequestRequestTypeDef definition

class DeleteProtectConfigurationRequestRequestTypeDef(TypedDict):
    ProtectConfigurationId: str,
```

## DeleteProtectConfigurationRuleSetNumberOverrideRequestRequestTypeDef

```python
# DeleteProtectConfigurationRuleSetNumberOverrideRequestRequestTypeDef definition

class DeleteProtectConfigurationRuleSetNumberOverrideRequestRequestTypeDef(TypedDict):
    ProtectConfigurationId: str,
    DestinationPhoneNumber: str,
```

## DeleteRegistrationAttachmentRequestRequestTypeDef

```python
# DeleteRegistrationAttachmentRequestRequestTypeDef definition

class DeleteRegistrationAttachmentRequestRequestTypeDef(TypedDict):
    RegistrationAttachmentId: str,
```

## DeleteRegistrationFieldValueRequestRequestTypeDef

```python
# DeleteRegistrationFieldValueRequestRequestTypeDef definition

class DeleteRegistrationFieldValueRequestRequestTypeDef(TypedDict):
    RegistrationId: str,
    FieldPath: str,
```

## DeleteRegistrationRequestRequestTypeDef

```python
# DeleteRegistrationRequestRequestTypeDef definition

class DeleteRegistrationRequestRequestTypeDef(TypedDict):
    RegistrationId: str,
```

## DeleteResourcePolicyRequestRequestTypeDef

```python
# DeleteResourcePolicyRequestRequestTypeDef definition

class DeleteResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## DeleteVerifiedDestinationNumberRequestRequestTypeDef

```python
# DeleteVerifiedDestinationNumberRequestRequestTypeDef definition

class DeleteVerifiedDestinationNumberRequestRequestTypeDef(TypedDict):
    VerifiedDestinationNumberId: str,
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
    Owner: NotRequired[OwnerType],  # (1)
```

1. See [:material-code-brackets: OwnerType](./literals.md#ownertype) 
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
    TwoWayChannelRole: NotRequired[str],
    PoolId: NotRequired[str],
    RegistrationId: NotRequired[str],
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
    TwoWayChannelRole: NotRequired[str],
```

1. See [:material-code-brackets: PoolStatusType](./literals.md#poolstatustype) 
2. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
## ProtectConfigurationFilterTypeDef

```python
# ProtectConfigurationFilterTypeDef definition

class ProtectConfigurationFilterTypeDef(TypedDict):
    Name: ProtectConfigurationFilterNameType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: ProtectConfigurationFilterNameType](./literals.md#protectconfigurationfilternametype) 
## ProtectConfigurationInformationTypeDef

```python
# ProtectConfigurationInformationTypeDef definition

class ProtectConfigurationInformationTypeDef(TypedDict):
    ProtectConfigurationArn: str,
    ProtectConfigurationId: str,
    CreatedTimestamp: datetime,
    AccountDefault: bool,
    DeletionProtectionEnabled: bool,
```

## RegistrationAttachmentFilterTypeDef

```python
# RegistrationAttachmentFilterTypeDef definition

class RegistrationAttachmentFilterTypeDef(TypedDict):
    Name: RegistrationAttachmentFilterNameType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: RegistrationAttachmentFilterNameType](./literals.md#registrationattachmentfilternametype) 
## RegistrationAttachmentsInformationTypeDef

```python
# RegistrationAttachmentsInformationTypeDef definition

class RegistrationAttachmentsInformationTypeDef(TypedDict):
    RegistrationAttachmentArn: str,
    RegistrationAttachmentId: str,
    AttachmentStatus: AttachmentStatusType,  # (1)
    CreatedTimestamp: datetime,
    AttachmentUploadErrorReason: NotRequired[AttachmentUploadErrorReasonType],  # (2)
```

1. See [:material-code-brackets: AttachmentStatusType](./literals.md#attachmentstatustype) 
2. See [:material-code-brackets: AttachmentUploadErrorReasonType](./literals.md#attachmentuploaderrorreasontype) 
## DescribeRegistrationFieldDefinitionsRequestRequestTypeDef

```python
# DescribeRegistrationFieldDefinitionsRequestRequestTypeDef definition

class DescribeRegistrationFieldDefinitionsRequestRequestTypeDef(TypedDict):
    RegistrationType: str,
    SectionPath: NotRequired[str],
    FieldPaths: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## DescribeRegistrationFieldValuesRequestRequestTypeDef

```python
# DescribeRegistrationFieldValuesRequestRequestTypeDef definition

class DescribeRegistrationFieldValuesRequestRequestTypeDef(TypedDict):
    RegistrationId: str,
    VersionNumber: NotRequired[int],
    SectionPath: NotRequired[str],
    FieldPaths: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## RegistrationFieldValueInformationTypeDef

```python
# RegistrationFieldValueInformationTypeDef definition

class RegistrationFieldValueInformationTypeDef(TypedDict):
    FieldPath: str,
    SelectChoices: NotRequired[List[str]],
    TextValue: NotRequired[str],
    RegistrationAttachmentId: NotRequired[str],
    DeniedReason: NotRequired[str],
```

## DescribeRegistrationSectionDefinitionsRequestRequestTypeDef

```python
# DescribeRegistrationSectionDefinitionsRequestRequestTypeDef definition

class DescribeRegistrationSectionDefinitionsRequestRequestTypeDef(TypedDict):
    RegistrationType: str,
    SectionPaths: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## RegistrationTypeFilterTypeDef

```python
# RegistrationTypeFilterTypeDef definition

class RegistrationTypeFilterTypeDef(TypedDict):
    Name: RegistrationTypeFilterNameType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: RegistrationTypeFilterNameType](./literals.md#registrationtypefilternametype) 
## RegistrationVersionFilterTypeDef

```python
# RegistrationVersionFilterTypeDef definition

class RegistrationVersionFilterTypeDef(TypedDict):
    Name: RegistrationVersionFilterNameType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: RegistrationVersionFilterNameType](./literals.md#registrationversionfilternametype) 
## RegistrationFilterTypeDef

```python
# RegistrationFilterTypeDef definition

class RegistrationFilterTypeDef(TypedDict):
    Name: RegistrationFilterNameType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: RegistrationFilterNameType](./literals.md#registrationfilternametype) 
## RegistrationInformationTypeDef

```python
# RegistrationInformationTypeDef definition

class RegistrationInformationTypeDef(TypedDict):
    RegistrationArn: str,
    RegistrationId: str,
    RegistrationType: str,
    RegistrationStatus: RegistrationStatusType,  # (1)
    CurrentVersionNumber: int,
    CreatedTimestamp: datetime,
    ApprovedVersionNumber: NotRequired[int],
    LatestDeniedVersionNumber: NotRequired[int],
    AdditionalAttributes: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
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
    DeletionProtectionEnabled: bool,
    Registered: bool,
    RegistrationId: NotRequired[str],
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
## VerifiedDestinationNumberFilterTypeDef

```python
# VerifiedDestinationNumberFilterTypeDef definition

class VerifiedDestinationNumberFilterTypeDef(TypedDict):
    Name: VerifiedDestinationNumberFilterNameType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: VerifiedDestinationNumberFilterNameType](./literals.md#verifieddestinationnumberfilternametype) 
## VerifiedDestinationNumberInformationTypeDef

```python
# VerifiedDestinationNumberInformationTypeDef definition

class VerifiedDestinationNumberInformationTypeDef(TypedDict):
    VerifiedDestinationNumberArn: str,
    VerifiedDestinationNumberId: str,
    DestinationPhoneNumber: str,
    Status: VerificationStatusType,  # (1)
    CreatedTimestamp: datetime,
```

1. See [:material-code-brackets: VerificationStatusType](./literals.md#verificationstatustype) 
## DisassociateOriginationIdentityRequestRequestTypeDef

```python
# DisassociateOriginationIdentityRequestRequestTypeDef definition

class DisassociateOriginationIdentityRequestRequestTypeDef(TypedDict):
    PoolId: str,
    OriginationIdentity: str,
    IsoCountryCode: str,
    ClientToken: NotRequired[str],
```

## DisassociateProtectConfigurationRequestRequestTypeDef

```python
# DisassociateProtectConfigurationRequestRequestTypeDef definition

class DisassociateProtectConfigurationRequestRequestTypeDef(TypedDict):
    ProtectConfigurationId: str,
    ConfigurationSetName: str,
```

## DiscardRegistrationVersionRequestRequestTypeDef

```python
# DiscardRegistrationVersionRequestRequestTypeDef definition

class DiscardRegistrationVersionRequestRequestTypeDef(TypedDict):
    RegistrationId: str,
```

## GetProtectConfigurationCountryRuleSetRequestRequestTypeDef

```python
# GetProtectConfigurationCountryRuleSetRequestRequestTypeDef definition

class GetProtectConfigurationCountryRuleSetRequestRequestTypeDef(TypedDict):
    ProtectConfigurationId: str,
    NumberCapability: NumberCapabilityType,  # (1)
```

1. See [:material-code-brackets: NumberCapabilityType](./literals.md#numbercapabilitytype) 
## ProtectConfigurationCountryRuleSetInformationTypeDef

```python
# ProtectConfigurationCountryRuleSetInformationTypeDef definition

class ProtectConfigurationCountryRuleSetInformationTypeDef(TypedDict):
    ProtectStatus: ProtectStatusType,  # (1)
```

1. See [:material-code-brackets: ProtectStatusType](./literals.md#protectstatustype) 
## GetResourcePolicyRequestRequestTypeDef

```python
# GetResourcePolicyRequestRequestTypeDef definition

class GetResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
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
    PhoneNumber: NotRequired[str],
```

1. See [:material-code-brackets: NumberCapabilityType](./literals.md#numbercapabilitytype) 
## ProtectConfigurationRuleSetNumberOverrideFilterItemTypeDef

```python
# ProtectConfigurationRuleSetNumberOverrideFilterItemTypeDef definition

class ProtectConfigurationRuleSetNumberOverrideFilterItemTypeDef(TypedDict):
    Name: ProtectConfigurationRuleSetNumberOverrideFilterNameType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: ProtectConfigurationRuleSetNumberOverrideFilterNameType](./literals.md#protectconfigurationrulesetnumberoverridefilternametype) 
## ProtectConfigurationRuleSetNumberOverrideTypeDef

```python
# ProtectConfigurationRuleSetNumberOverrideTypeDef definition

class ProtectConfigurationRuleSetNumberOverrideTypeDef(TypedDict):
    DestinationPhoneNumber: str,
    CreatedTimestamp: datetime,
    Action: ProtectConfigurationRuleOverrideActionType,  # (1)
    IsoCountryCode: NotRequired[str],
    ExpirationTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: ProtectConfigurationRuleOverrideActionType](./literals.md#protectconfigurationruleoverrideactiontype) 
## RegistrationAssociationFilterTypeDef

```python
# RegistrationAssociationFilterTypeDef definition

class RegistrationAssociationFilterTypeDef(TypedDict):
    Name: RegistrationAssociationFilterNameType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: RegistrationAssociationFilterNameType](./literals.md#registrationassociationfilternametype) 
## RegistrationAssociationMetadataTypeDef

```python
# RegistrationAssociationMetadataTypeDef definition

class RegistrationAssociationMetadataTypeDef(TypedDict):
    ResourceArn: str,
    ResourceId: str,
    ResourceType: str,
    IsoCountryCode: NotRequired[str],
    PhoneNumber: NotRequired[str],
```

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
## PutMessageFeedbackRequestRequestTypeDef

```python
# PutMessageFeedbackRequestRequestTypeDef definition

class PutMessageFeedbackRequestRequestTypeDef(TypedDict):
    MessageId: str,
    MessageFeedbackStatus: MessageFeedbackStatusType,  # (1)
```

1. See [:material-code-brackets: MessageFeedbackStatusType](./literals.md#messagefeedbackstatustype) 
## PutOptedOutNumberRequestRequestTypeDef

```python
# PutOptedOutNumberRequestRequestTypeDef definition

class PutOptedOutNumberRequestRequestTypeDef(TypedDict):
    OptOutListName: str,
    OptedOutNumber: str,
```

## PutRegistrationFieldValueRequestRequestTypeDef

```python
# PutRegistrationFieldValueRequestRequestTypeDef definition

class PutRegistrationFieldValueRequestRequestTypeDef(TypedDict):
    RegistrationId: str,
    FieldPath: str,
    SelectChoices: NotRequired[Sequence[str]],
    TextValue: NotRequired[str],
    RegistrationAttachmentId: NotRequired[str],
```

## PutResourcePolicyRequestRequestTypeDef

```python
# PutResourcePolicyRequestRequestTypeDef definition

class PutResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Policy: str,
```

## RegistrationDeniedReasonInformationTypeDef

```python
# RegistrationDeniedReasonInformationTypeDef definition

class RegistrationDeniedReasonInformationTypeDef(TypedDict):
    Reason: str,
    ShortDescription: str,
    LongDescription: NotRequired[str],
    DocumentationTitle: NotRequired[str],
    DocumentationLink: NotRequired[str],
```

## SelectValidationTypeDef

```python
# SelectValidationTypeDef definition

class SelectValidationTypeDef(TypedDict):
    MinChoices: int,
    MaxChoices: int,
    Options: List[str],
```

## TextValidationTypeDef

```python
# TextValidationTypeDef definition

class TextValidationTypeDef(TypedDict):
    MinLength: int,
    MaxLength: int,
    Pattern: str,
```

## SelectOptionDescriptionTypeDef

```python
# SelectOptionDescriptionTypeDef definition

class SelectOptionDescriptionTypeDef(TypedDict):
    Option: str,
    Title: NotRequired[str],
    Description: NotRequired[str],
```

## RegistrationSectionDisplayHintsTypeDef

```python
# RegistrationSectionDisplayHintsTypeDef definition

class RegistrationSectionDisplayHintsTypeDef(TypedDict):
    Title: str,
    ShortDescription: str,
    LongDescription: NotRequired[str],
    DocumentationTitle: NotRequired[str],
    DocumentationLink: NotRequired[str],
```

## RegistrationTypeDisplayHintsTypeDef

```python
# RegistrationTypeDisplayHintsTypeDef definition

class RegistrationTypeDisplayHintsTypeDef(TypedDict):
    Title: str,
    ShortDescription: NotRequired[str],
    LongDescription: NotRequired[str],
    DocumentationTitle: NotRequired[str],
    DocumentationLink: NotRequired[str],
```

## SupportedAssociationTypeDef

```python
# SupportedAssociationTypeDef definition

class SupportedAssociationTypeDef(TypedDict):
    ResourceType: str,
    AssociationBehavior: RegistrationAssociationBehaviorType,  # (1)
    DisassociationBehavior: RegistrationDisassociationBehaviorType,  # (2)
    IsoCountryCode: NotRequired[str],
```

1. See [:material-code-brackets: RegistrationAssociationBehaviorType](./literals.md#registrationassociationbehaviortype) 
2. See [:material-code-brackets: RegistrationDisassociationBehaviorType](./literals.md#registrationdisassociationbehaviortype) 
## ReleasePhoneNumberRequestRequestTypeDef

```python
# ReleasePhoneNumberRequestRequestTypeDef definition

class ReleasePhoneNumberRequestRequestTypeDef(TypedDict):
    PhoneNumberId: str,
```

## ReleaseSenderIdRequestRequestTypeDef

```python
# ReleaseSenderIdRequestRequestTypeDef definition

class ReleaseSenderIdRequestRequestTypeDef(TypedDict):
    SenderId: str,
    IsoCountryCode: str,
```

## SendDestinationNumberVerificationCodeRequestRequestTypeDef

```python
# SendDestinationNumberVerificationCodeRequestRequestTypeDef definition

class SendDestinationNumberVerificationCodeRequestRequestTypeDef(TypedDict):
    VerifiedDestinationNumberId: str,
    VerificationChannel: VerificationChannelType,  # (1)
    LanguageCode: NotRequired[LanguageCodeType],  # (2)
    OriginationIdentity: NotRequired[str],
    ConfigurationSetName: NotRequired[str],
    Context: NotRequired[Mapping[str, str]],
    DestinationCountryParameters: NotRequired[Mapping[DestinationCountryParameterKeyType, str]],  # (3)
```

1. See [:material-code-brackets: VerificationChannelType](./literals.md#verificationchanneltype) 
2. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
3. See [:material-code-brackets: DestinationCountryParameterKeyType](./literals.md#destinationcountryparameterkeytype) 
## SendMediaMessageRequestRequestTypeDef

```python
# SendMediaMessageRequestRequestTypeDef definition

class SendMediaMessageRequestRequestTypeDef(TypedDict):
    DestinationPhoneNumber: str,
    OriginationIdentity: str,
    MessageBody: NotRequired[str],
    MediaUrls: NotRequired[Sequence[str]],
    ConfigurationSetName: NotRequired[str],
    MaxPrice: NotRequired[str],
    TimeToLive: NotRequired[int],
    Context: NotRequired[Mapping[str, str]],
    DryRun: NotRequired[bool],
    ProtectConfigurationId: NotRequired[str],
    MessageFeedbackEnabled: NotRequired[bool],
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
    ProtectConfigurationId: NotRequired[str],
    MessageFeedbackEnabled: NotRequired[bool],
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
    ProtectConfigurationId: NotRequired[str],
    MessageFeedbackEnabled: NotRequired[bool],
```

1. See [:material-code-brackets: VoiceMessageBodyTextTypeType](./literals.md#voicemessagebodytexttypetype) 
2. See [:material-code-brackets: VoiceIdType](./literals.md#voiceidtype) 
## SetAccountDefaultProtectConfigurationRequestRequestTypeDef

```python
# SetAccountDefaultProtectConfigurationRequestRequestTypeDef definition

class SetAccountDefaultProtectConfigurationRequestRequestTypeDef(TypedDict):
    ProtectConfigurationId: str,
```

## SetDefaultMessageFeedbackEnabledRequestRequestTypeDef

```python
# SetDefaultMessageFeedbackEnabledRequestRequestTypeDef definition

class SetDefaultMessageFeedbackEnabledRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    MessageFeedbackEnabled: bool,
```

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

## SetMediaMessageSpendLimitOverrideRequestRequestTypeDef

```python
# SetMediaMessageSpendLimitOverrideRequestRequestTypeDef definition

class SetMediaMessageSpendLimitOverrideRequestRequestTypeDef(TypedDict):
    MonthlyLimit: int,
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

## SubmitRegistrationVersionRequestRequestTypeDef

```python
# SubmitRegistrationVersionRequestRequestTypeDef definition

class SubmitRegistrationVersionRequestRequestTypeDef(TypedDict):
    RegistrationId: str,
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
    TwoWayChannelRole: NotRequired[str],
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
    TwoWayChannelRole: NotRequired[str],
    SelfManagedOptOutsEnabled: NotRequired[bool],
    OptOutListName: NotRequired[str],
    SharedRoutesEnabled: NotRequired[bool],
    DeletionProtectionEnabled: NotRequired[bool],
```

## UpdateProtectConfigurationRequestRequestTypeDef

```python
# UpdateProtectConfigurationRequestRequestTypeDef definition

class UpdateProtectConfigurationRequestRequestTypeDef(TypedDict):
    ProtectConfigurationId: str,
    DeletionProtectionEnabled: NotRequired[bool],
```

## UpdateSenderIdRequestRequestTypeDef

```python
# UpdateSenderIdRequestRequestTypeDef definition

class UpdateSenderIdRequestRequestTypeDef(TypedDict):
    SenderId: str,
    IsoCountryCode: str,
    DeletionProtectionEnabled: NotRequired[bool],
```

## VerifyDestinationNumberRequestRequestTypeDef

```python
# VerifyDestinationNumberRequestRequestTypeDef definition

class VerifyDestinationNumberRequestRequestTypeDef(TypedDict):
    VerifiedDestinationNumberId: str,
    VerificationCode: str,
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
## AssociateProtectConfigurationResultTypeDef

```python
# AssociateProtectConfigurationResultTypeDef definition

class AssociateProtectConfigurationResultTypeDef(TypedDict):
    ConfigurationSetArn: str,
    ConfigurationSetName: str,
    ProtectConfigurationArn: str,
    ProtectConfigurationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRegistrationAssociationResultTypeDef

```python
# CreateRegistrationAssociationResultTypeDef definition

class CreateRegistrationAssociationResultTypeDef(TypedDict):
    RegistrationArn: str,
    RegistrationId: str,
    RegistrationType: str,
    ResourceArn: str,
    ResourceId: str,
    ResourceType: str,
    IsoCountryCode: str,
    PhoneNumber: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAccountDefaultProtectConfigurationResultTypeDef

```python
# DeleteAccountDefaultProtectConfigurationResultTypeDef definition

class DeleteAccountDefaultProtectConfigurationResultTypeDef(TypedDict):
    DefaultProtectConfigurationArn: str,
    DefaultProtectConfigurationId: str,
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
## DeleteMediaMessageSpendLimitOverrideResultTypeDef

```python
# DeleteMediaMessageSpendLimitOverrideResultTypeDef definition

class DeleteMediaMessageSpendLimitOverrideResultTypeDef(TypedDict):
    MonthlyLimit: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    TwoWayChannelRole: str,
    SelfManagedOptOutsEnabled: bool,
    OptOutListName: str,
    SharedRoutesEnabled: bool,
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: PoolStatusType](./literals.md#poolstatustype) 
2. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteProtectConfigurationResultTypeDef

```python
# DeleteProtectConfigurationResultTypeDef definition

class DeleteProtectConfigurationResultTypeDef(TypedDict):
    ProtectConfigurationArn: str,
    ProtectConfigurationId: str,
    CreatedTimestamp: datetime,
    AccountDefault: bool,
    DeletionProtectionEnabled: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteProtectConfigurationRuleSetNumberOverrideResultTypeDef

```python
# DeleteProtectConfigurationRuleSetNumberOverrideResultTypeDef definition

class DeleteProtectConfigurationRuleSetNumberOverrideResultTypeDef(TypedDict):
    ProtectConfigurationArn: str,
    ProtectConfigurationId: str,
    DestinationPhoneNumber: str,
    CreatedTimestamp: datetime,
    Action: ProtectConfigurationRuleOverrideActionType,  # (1)
    IsoCountryCode: str,
    ExpirationTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ProtectConfigurationRuleOverrideActionType](./literals.md#protectconfigurationruleoverrideactiontype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRegistrationAttachmentResultTypeDef

```python
# DeleteRegistrationAttachmentResultTypeDef definition

class DeleteRegistrationAttachmentResultTypeDef(TypedDict):
    RegistrationAttachmentArn: str,
    RegistrationAttachmentId: str,
    AttachmentStatus: AttachmentStatusType,  # (1)
    AttachmentUploadErrorReason: AttachmentUploadErrorReasonType,  # (2)
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AttachmentStatusType](./literals.md#attachmentstatustype) 
2. See [:material-code-brackets: AttachmentUploadErrorReasonType](./literals.md#attachmentuploaderrorreasontype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRegistrationFieldValueResultTypeDef

```python
# DeleteRegistrationFieldValueResultTypeDef definition

class DeleteRegistrationFieldValueResultTypeDef(TypedDict):
    RegistrationArn: str,
    RegistrationId: str,
    VersionNumber: int,
    FieldPath: str,
    SelectChoices: List[str],
    TextValue: str,
    RegistrationAttachmentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRegistrationResultTypeDef

```python
# DeleteRegistrationResultTypeDef definition

class DeleteRegistrationResultTypeDef(TypedDict):
    RegistrationArn: str,
    RegistrationId: str,
    RegistrationType: str,
    RegistrationStatus: RegistrationStatusType,  # (1)
    CurrentVersionNumber: int,
    ApprovedVersionNumber: int,
    LatestDeniedVersionNumber: int,
    AdditionalAttributes: Dict[str, str],
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteResourcePolicyResultTypeDef

```python
# DeleteResourcePolicyResultTypeDef definition

class DeleteResourcePolicyResultTypeDef(TypedDict):
    ResourceArn: str,
    Policy: str,
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTextMessageSpendLimitOverrideResultTypeDef

```python
# DeleteTextMessageSpendLimitOverrideResultTypeDef definition

class DeleteTextMessageSpendLimitOverrideResultTypeDef(TypedDict):
    MonthlyLimit: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteVerifiedDestinationNumberResultTypeDef

```python
# DeleteVerifiedDestinationNumberResultTypeDef definition

class DeleteVerifiedDestinationNumberResultTypeDef(TypedDict):
    VerifiedDestinationNumberArn: str,
    VerifiedDestinationNumberId: str,
    DestinationPhoneNumber: str,
    CreatedTimestamp: datetime,
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
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AccountAttributeTypeDef](./type_defs.md#accountattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountLimitsResultTypeDef

```python
# DescribeAccountLimitsResultTypeDef definition

class DescribeAccountLimitsResultTypeDef(TypedDict):
    AccountLimits: List[AccountLimitTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
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
## DisassociateProtectConfigurationResultTypeDef

```python
# DisassociateProtectConfigurationResultTypeDef definition

class DisassociateProtectConfigurationResultTypeDef(TypedDict):
    ConfigurationSetArn: str,
    ConfigurationSetName: str,
    ProtectConfigurationArn: str,
    ProtectConfigurationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePolicyResultTypeDef

```python
# GetResourcePolicyResultTypeDef definition

class GetResourcePolicyResultTypeDef(TypedDict):
    ResourceArn: str,
    Policy: str,
    CreatedTimestamp: datetime,
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
## PutMessageFeedbackResultTypeDef

```python
# PutMessageFeedbackResultTypeDef definition

class PutMessageFeedbackResultTypeDef(TypedDict):
    MessageId: str,
    MessageFeedbackStatus: MessageFeedbackStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: MessageFeedbackStatusType](./literals.md#messagefeedbackstatustype) 
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
## PutProtectConfigurationRuleSetNumberOverrideResultTypeDef

```python
# PutProtectConfigurationRuleSetNumberOverrideResultTypeDef definition

class PutProtectConfigurationRuleSetNumberOverrideResultTypeDef(TypedDict):
    ProtectConfigurationArn: str,
    ProtectConfigurationId: str,
    DestinationPhoneNumber: str,
    CreatedTimestamp: datetime,
    Action: ProtectConfigurationRuleOverrideActionType,  # (1)
    IsoCountryCode: str,
    ExpirationTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ProtectConfigurationRuleOverrideActionType](./literals.md#protectconfigurationruleoverrideactiontype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRegistrationFieldValueResultTypeDef

```python
# PutRegistrationFieldValueResultTypeDef definition

class PutRegistrationFieldValueResultTypeDef(TypedDict):
    RegistrationArn: str,
    RegistrationId: str,
    VersionNumber: int,
    FieldPath: str,
    SelectChoices: List[str],
    TextValue: str,
    RegistrationAttachmentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResourcePolicyResultTypeDef

```python
# PutResourcePolicyResultTypeDef definition

class PutResourcePolicyResultTypeDef(TypedDict):
    ResourceArn: str,
    Policy: str,
    CreatedTimestamp: datetime,
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
    TwoWayChannelRole: str,
    SelfManagedOptOutsEnabled: bool,
    OptOutListName: str,
    RegistrationId: str,
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: NumberStatusType](./literals.md#numberstatustype) 
2. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
3. See [:material-code-brackets: NumberCapabilityType](./literals.md#numbercapabilitytype) 
4. See [:material-code-brackets: NumberTypeType](./literals.md#numbertypetype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReleaseSenderIdResultTypeDef

```python
# ReleaseSenderIdResultTypeDef definition

class ReleaseSenderIdResultTypeDef(TypedDict):
    SenderIdArn: str,
    SenderId: str,
    IsoCountryCode: str,
    MessageTypes: List[MessageTypeType],  # (1)
    MonthlyLeasingPrice: str,
    Registered: bool,
    RegistrationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendDestinationNumberVerificationCodeResultTypeDef

```python
# SendDestinationNumberVerificationCodeResultTypeDef definition

class SendDestinationNumberVerificationCodeResultTypeDef(TypedDict):
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendMediaMessageResultTypeDef

```python
# SendMediaMessageResultTypeDef definition

class SendMediaMessageResultTypeDef(TypedDict):
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## SetAccountDefaultProtectConfigurationResultTypeDef

```python
# SetAccountDefaultProtectConfigurationResultTypeDef definition

class SetAccountDefaultProtectConfigurationResultTypeDef(TypedDict):
    DefaultProtectConfigurationArn: str,
    DefaultProtectConfigurationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetDefaultMessageFeedbackEnabledResultTypeDef

```python
# SetDefaultMessageFeedbackEnabledResultTypeDef definition

class SetDefaultMessageFeedbackEnabledResultTypeDef(TypedDict):
    ConfigurationSetArn: str,
    ConfigurationSetName: str,
    MessageFeedbackEnabled: bool,
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
## SetMediaMessageSpendLimitOverrideResultTypeDef

```python
# SetMediaMessageSpendLimitOverrideResultTypeDef definition

class SetMediaMessageSpendLimitOverrideResultTypeDef(TypedDict):
    MonthlyLimit: int,
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
    TwoWayChannelRole: str,
    SelfManagedOptOutsEnabled: bool,
    OptOutListName: str,
    DeletionProtectionEnabled: bool,
    RegistrationId: str,
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
    TwoWayChannelRole: str,
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
## UpdateProtectConfigurationResultTypeDef

```python
# UpdateProtectConfigurationResultTypeDef definition

class UpdateProtectConfigurationResultTypeDef(TypedDict):
    ProtectConfigurationArn: str,
    ProtectConfigurationId: str,
    CreatedTimestamp: datetime,
    AccountDefault: bool,
    DeletionProtectionEnabled: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSenderIdResultTypeDef

```python
# UpdateSenderIdResultTypeDef definition

class UpdateSenderIdResultTypeDef(TypedDict):
    SenderIdArn: str,
    SenderId: str,
    IsoCountryCode: str,
    MessageTypes: List[MessageTypeType],  # (1)
    MonthlyLeasingPrice: str,
    DeletionProtectionEnabled: bool,
    Registered: bool,
    RegistrationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VerifyDestinationNumberResultTypeDef

```python
# VerifyDestinationNumberResultTypeDef definition

class VerifyDestinationNumberResultTypeDef(TypedDict):
    VerifiedDestinationNumberArn: str,
    VerifiedDestinationNumberId: str,
    DestinationPhoneNumber: str,
    Status: VerificationStatusType,  # (1)
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: VerificationStatusType](./literals.md#verificationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    TwoWayChannelRole: str,
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
## CreateProtectConfigurationRequestRequestTypeDef

```python
# CreateProtectConfigurationRequestRequestTypeDef definition

class CreateProtectConfigurationRequestRequestTypeDef(TypedDict):
    ClientToken: NotRequired[str],
    DeletionProtectionEnabled: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateProtectConfigurationResultTypeDef

```python
# CreateProtectConfigurationResultTypeDef definition

class CreateProtectConfigurationResultTypeDef(TypedDict):
    ProtectConfigurationArn: str,
    ProtectConfigurationId: str,
    CreatedTimestamp: datetime,
    AccountDefault: bool,
    DeletionProtectionEnabled: bool,
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRegistrationAttachmentRequestRequestTypeDef

```python
# CreateRegistrationAttachmentRequestRequestTypeDef definition

class CreateRegistrationAttachmentRequestRequestTypeDef(TypedDict):
    AttachmentBody: NotRequired[BlobTypeDef],
    AttachmentUrl: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateRegistrationAttachmentResultTypeDef

```python
# CreateRegistrationAttachmentResultTypeDef definition

class CreateRegistrationAttachmentResultTypeDef(TypedDict):
    RegistrationAttachmentArn: str,
    RegistrationAttachmentId: str,
    AttachmentStatus: AttachmentStatusType,  # (1)
    Tags: List[TagTypeDef],  # (2)
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AttachmentStatusType](./literals.md#attachmentstatustype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRegistrationRequestRequestTypeDef

```python
# CreateRegistrationRequestRequestTypeDef definition

class CreateRegistrationRequestRequestTypeDef(TypedDict):
    RegistrationType: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateRegistrationResultTypeDef

```python
# CreateRegistrationResultTypeDef definition

class CreateRegistrationResultTypeDef(TypedDict):
    RegistrationArn: str,
    RegistrationId: str,
    RegistrationType: str,
    RegistrationStatus: RegistrationStatusType,  # (1)
    CurrentVersionNumber: int,
    AdditionalAttributes: Dict[str, str],
    Tags: List[TagTypeDef],  # (2)
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVerifiedDestinationNumberRequestRequestTypeDef

```python
# CreateVerifiedDestinationNumberRequestRequestTypeDef definition

class CreateVerifiedDestinationNumberRequestRequestTypeDef(TypedDict):
    DestinationPhoneNumber: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateVerifiedDestinationNumberResultTypeDef

```python
# CreateVerifiedDestinationNumberResultTypeDef definition

class CreateVerifiedDestinationNumberResultTypeDef(TypedDict):
    VerifiedDestinationNumberArn: str,
    VerifiedDestinationNumberId: str,
    DestinationPhoneNumber: str,
    Status: VerificationStatusType,  # (1)
    Tags: List[TagTypeDef],  # (2)
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: VerificationStatusType](./literals.md#verificationstatustype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    TwoWayChannelRole: str,
    SelfManagedOptOutsEnabled: bool,
    OptOutListName: str,
    DeletionProtectionEnabled: bool,
    PoolId: str,
    RegistrationId: str,
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
## RequestSenderIdRequestRequestTypeDef

```python
# RequestSenderIdRequestRequestTypeDef definition

class RequestSenderIdRequestRequestTypeDef(TypedDict):
    SenderId: str,
    IsoCountryCode: str,
    MessageTypes: NotRequired[Sequence[MessageTypeType]],  # (1)
    DeletionProtectionEnabled: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    ClientToken: NotRequired[str],
```

1. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## RequestSenderIdResultTypeDef

```python
# RequestSenderIdResultTypeDef definition

class RequestSenderIdResultTypeDef(TypedDict):
    SenderIdArn: str,
    SenderId: str,
    IsoCountryCode: str,
    MessageTypes: List[MessageTypeType],  # (1)
    MonthlyLeasingPrice: str,
    DeletionProtectionEnabled: bool,
    Registered: bool,
    Tags: List[TagTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## CreateRegistrationVersionResultTypeDef

```python
# CreateRegistrationVersionResultTypeDef definition

class CreateRegistrationVersionResultTypeDef(TypedDict):
    RegistrationArn: str,
    RegistrationId: str,
    VersionNumber: int,
    RegistrationVersionStatus: RegistrationVersionStatusType,  # (1)
    RegistrationVersionStatusHistory: RegistrationVersionStatusHistoryTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: RegistrationVersionStatusType](./literals.md#registrationversionstatustype) 
2. See [:material-code-braces: RegistrationVersionStatusHistoryTypeDef](./type_defs.md#registrationversionstatushistorytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DiscardRegistrationVersionResultTypeDef

```python
# DiscardRegistrationVersionResultTypeDef definition

class DiscardRegistrationVersionResultTypeDef(TypedDict):
    RegistrationArn: str,
    RegistrationId: str,
    VersionNumber: int,
    RegistrationVersionStatus: RegistrationVersionStatusType,  # (1)
    RegistrationVersionStatusHistory: RegistrationVersionStatusHistoryTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: RegistrationVersionStatusType](./literals.md#registrationversionstatustype) 
2. See [:material-code-braces: RegistrationVersionStatusHistoryTypeDef](./type_defs.md#registrationversionstatushistorytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubmitRegistrationVersionResultTypeDef

```python
# SubmitRegistrationVersionResultTypeDef definition

class SubmitRegistrationVersionResultTypeDef(TypedDict):
    RegistrationArn: str,
    RegistrationId: str,
    VersionNumber: int,
    RegistrationVersionStatus: RegistrationVersionStatusType,  # (1)
    RegistrationVersionStatusHistory: RegistrationVersionStatusHistoryTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: RegistrationVersionStatusType](./literals.md#registrationversionstatustype) 
2. See [:material-code-braces: RegistrationVersionStatusHistoryTypeDef](./type_defs.md#registrationversionstatushistorytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountAttributesRequestPaginateTypeDef

```python
# DescribeAccountAttributesRequestPaginateTypeDef definition

class DescribeAccountAttributesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAccountLimitsRequestPaginateTypeDef

```python
# DescribeAccountLimitsRequestPaginateTypeDef definition

class DescribeAccountLimitsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeConfigurationSetsRequestPaginateTypeDef

```python
# DescribeConfigurationSetsRequestPaginateTypeDef definition

class DescribeConfigurationSetsRequestPaginateTypeDef(TypedDict):
    ConfigurationSetNames: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[ConfigurationSetFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ConfigurationSetFilterTypeDef](./type_defs.md#configurationsetfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeOptOutListsRequestPaginateTypeDef

```python
# DescribeOptOutListsRequestPaginateTypeDef definition

class DescribeOptOutListsRequestPaginateTypeDef(TypedDict):
    OptOutListNames: NotRequired[Sequence[str]],
    Owner: NotRequired[OwnerType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: OwnerType](./literals.md#ownertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeRegistrationFieldDefinitionsRequestPaginateTypeDef

```python
# DescribeRegistrationFieldDefinitionsRequestPaginateTypeDef definition

class DescribeRegistrationFieldDefinitionsRequestPaginateTypeDef(TypedDict):
    RegistrationType: str,
    SectionPath: NotRequired[str],
    FieldPaths: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeRegistrationFieldValuesRequestPaginateTypeDef

```python
# DescribeRegistrationFieldValuesRequestPaginateTypeDef definition

class DescribeRegistrationFieldValuesRequestPaginateTypeDef(TypedDict):
    RegistrationId: str,
    VersionNumber: NotRequired[int],
    SectionPath: NotRequired[str],
    FieldPaths: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeRegistrationSectionDefinitionsRequestPaginateTypeDef

```python
# DescribeRegistrationSectionDefinitionsRequestPaginateTypeDef definition

class DescribeRegistrationSectionDefinitionsRequestPaginateTypeDef(TypedDict):
    RegistrationType: str,
    SectionPaths: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSpendLimitsRequestPaginateTypeDef

```python
# DescribeSpendLimitsRequestPaginateTypeDef definition

class DescribeSpendLimitsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeKeywordsRequestPaginateTypeDef

```python
# DescribeKeywordsRequestPaginateTypeDef definition

class DescribeKeywordsRequestPaginateTypeDef(TypedDict):
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
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: KeywordInformationTypeDef](./type_defs.md#keywordinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOptOutListsResultTypeDef

```python
# DescribeOptOutListsResultTypeDef definition

class DescribeOptOutListsResultTypeDef(TypedDict):
    OptOutLists: List[OptOutListInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OptOutListInformationTypeDef](./type_defs.md#optoutlistinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOptedOutNumbersRequestPaginateTypeDef

```python
# DescribeOptedOutNumbersRequestPaginateTypeDef definition

class DescribeOptedOutNumbersRequestPaginateTypeDef(TypedDict):
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
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OptedOutNumberInformationTypeDef](./type_defs.md#optedoutnumberinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePhoneNumbersRequestPaginateTypeDef

```python
# DescribePhoneNumbersRequestPaginateTypeDef definition

class DescribePhoneNumbersRequestPaginateTypeDef(TypedDict):
    PhoneNumberIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[PhoneNumberFilterTypeDef]],  # (1)
    Owner: NotRequired[OwnerType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: PhoneNumberFilterTypeDef](./type_defs.md#phonenumberfiltertypedef) 
2. See [:material-code-brackets: OwnerType](./literals.md#ownertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribePhoneNumbersRequestRequestTypeDef

```python
# DescribePhoneNumbersRequestRequestTypeDef definition

class DescribePhoneNumbersRequestRequestTypeDef(TypedDict):
    PhoneNumberIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[PhoneNumberFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Owner: NotRequired[OwnerType],  # (2)
```

1. See [:material-code-braces: PhoneNumberFilterTypeDef](./type_defs.md#phonenumberfiltertypedef) 
2. See [:material-code-brackets: OwnerType](./literals.md#ownertype) 
## DescribePhoneNumbersResultTypeDef

```python
# DescribePhoneNumbersResultTypeDef definition

class DescribePhoneNumbersResultTypeDef(TypedDict):
    PhoneNumbers: List[PhoneNumberInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PhoneNumberInformationTypeDef](./type_defs.md#phonenumberinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePoolsRequestPaginateTypeDef

```python
# DescribePoolsRequestPaginateTypeDef definition

class DescribePoolsRequestPaginateTypeDef(TypedDict):
    PoolIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[PoolFilterTypeDef]],  # (1)
    Owner: NotRequired[OwnerType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: PoolFilterTypeDef](./type_defs.md#poolfiltertypedef) 
2. See [:material-code-brackets: OwnerType](./literals.md#ownertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribePoolsRequestRequestTypeDef

```python
# DescribePoolsRequestRequestTypeDef definition

class DescribePoolsRequestRequestTypeDef(TypedDict):
    PoolIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[PoolFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Owner: NotRequired[OwnerType],  # (2)
```

1. See [:material-code-braces: PoolFilterTypeDef](./type_defs.md#poolfiltertypedef) 
2. See [:material-code-brackets: OwnerType](./literals.md#ownertype) 
## DescribePoolsResultTypeDef

```python
# DescribePoolsResultTypeDef definition

class DescribePoolsResultTypeDef(TypedDict):
    Pools: List[PoolInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PoolInformationTypeDef](./type_defs.md#poolinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeProtectConfigurationsRequestPaginateTypeDef

```python
# DescribeProtectConfigurationsRequestPaginateTypeDef definition

class DescribeProtectConfigurationsRequestPaginateTypeDef(TypedDict):
    ProtectConfigurationIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[ProtectConfigurationFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ProtectConfigurationFilterTypeDef](./type_defs.md#protectconfigurationfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeProtectConfigurationsRequestRequestTypeDef

```python
# DescribeProtectConfigurationsRequestRequestTypeDef definition

class DescribeProtectConfigurationsRequestRequestTypeDef(TypedDict):
    ProtectConfigurationIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[ProtectConfigurationFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ProtectConfigurationFilterTypeDef](./type_defs.md#protectconfigurationfiltertypedef) 
## DescribeProtectConfigurationsResultTypeDef

```python
# DescribeProtectConfigurationsResultTypeDef definition

class DescribeProtectConfigurationsResultTypeDef(TypedDict):
    ProtectConfigurations: List[ProtectConfigurationInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProtectConfigurationInformationTypeDef](./type_defs.md#protectconfigurationinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRegistrationAttachmentsRequestPaginateTypeDef

```python
# DescribeRegistrationAttachmentsRequestPaginateTypeDef definition

class DescribeRegistrationAttachmentsRequestPaginateTypeDef(TypedDict):
    RegistrationAttachmentIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[RegistrationAttachmentFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: RegistrationAttachmentFilterTypeDef](./type_defs.md#registrationattachmentfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeRegistrationAttachmentsRequestRequestTypeDef

```python
# DescribeRegistrationAttachmentsRequestRequestTypeDef definition

class DescribeRegistrationAttachmentsRequestRequestTypeDef(TypedDict):
    RegistrationAttachmentIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[RegistrationAttachmentFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: RegistrationAttachmentFilterTypeDef](./type_defs.md#registrationattachmentfiltertypedef) 
## DescribeRegistrationAttachmentsResultTypeDef

```python
# DescribeRegistrationAttachmentsResultTypeDef definition

class DescribeRegistrationAttachmentsResultTypeDef(TypedDict):
    RegistrationAttachments: List[RegistrationAttachmentsInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RegistrationAttachmentsInformationTypeDef](./type_defs.md#registrationattachmentsinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRegistrationFieldValuesResultTypeDef

```python
# DescribeRegistrationFieldValuesResultTypeDef definition

class DescribeRegistrationFieldValuesResultTypeDef(TypedDict):
    RegistrationArn: str,
    RegistrationId: str,
    VersionNumber: int,
    RegistrationFieldValues: List[RegistrationFieldValueInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RegistrationFieldValueInformationTypeDef](./type_defs.md#registrationfieldvalueinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRegistrationTypeDefinitionsRequestPaginateTypeDef

```python
# DescribeRegistrationTypeDefinitionsRequestPaginateTypeDef definition

class DescribeRegistrationTypeDefinitionsRequestPaginateTypeDef(TypedDict):
    RegistrationTypes: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[RegistrationTypeFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: RegistrationTypeFilterTypeDef](./type_defs.md#registrationtypefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeRegistrationTypeDefinitionsRequestRequestTypeDef

```python
# DescribeRegistrationTypeDefinitionsRequestRequestTypeDef definition

class DescribeRegistrationTypeDefinitionsRequestRequestTypeDef(TypedDict):
    RegistrationTypes: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[RegistrationTypeFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: RegistrationTypeFilterTypeDef](./type_defs.md#registrationtypefiltertypedef) 
## DescribeRegistrationVersionsRequestPaginateTypeDef

```python
# DescribeRegistrationVersionsRequestPaginateTypeDef definition

class DescribeRegistrationVersionsRequestPaginateTypeDef(TypedDict):
    RegistrationId: str,
    VersionNumbers: NotRequired[Sequence[int]],
    Filters: NotRequired[Sequence[RegistrationVersionFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: RegistrationVersionFilterTypeDef](./type_defs.md#registrationversionfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeRegistrationVersionsRequestRequestTypeDef

```python
# DescribeRegistrationVersionsRequestRequestTypeDef definition

class DescribeRegistrationVersionsRequestRequestTypeDef(TypedDict):
    RegistrationId: str,
    VersionNumbers: NotRequired[Sequence[int]],
    Filters: NotRequired[Sequence[RegistrationVersionFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: RegistrationVersionFilterTypeDef](./type_defs.md#registrationversionfiltertypedef) 
## DescribeRegistrationsRequestPaginateTypeDef

```python
# DescribeRegistrationsRequestPaginateTypeDef definition

class DescribeRegistrationsRequestPaginateTypeDef(TypedDict):
    RegistrationIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[RegistrationFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: RegistrationFilterTypeDef](./type_defs.md#registrationfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeRegistrationsRequestRequestTypeDef

```python
# DescribeRegistrationsRequestRequestTypeDef definition

class DescribeRegistrationsRequestRequestTypeDef(TypedDict):
    RegistrationIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[RegistrationFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: RegistrationFilterTypeDef](./type_defs.md#registrationfiltertypedef) 
## DescribeRegistrationsResultTypeDef

```python
# DescribeRegistrationsResultTypeDef definition

class DescribeRegistrationsResultTypeDef(TypedDict):
    Registrations: List[RegistrationInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RegistrationInformationTypeDef](./type_defs.md#registrationinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSenderIdsRequestPaginateTypeDef

```python
# DescribeSenderIdsRequestPaginateTypeDef definition

class DescribeSenderIdsRequestPaginateTypeDef(TypedDict):
    SenderIds: NotRequired[Sequence[SenderIdAndCountryTypeDef]],  # (1)
    Filters: NotRequired[Sequence[SenderIdFilterTypeDef]],  # (2)
    Owner: NotRequired[OwnerType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: SenderIdAndCountryTypeDef](./type_defs.md#senderidandcountrytypedef) 
2. See [:material-code-braces: SenderIdFilterTypeDef](./type_defs.md#senderidfiltertypedef) 
3. See [:material-code-brackets: OwnerType](./literals.md#ownertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSenderIdsRequestRequestTypeDef

```python
# DescribeSenderIdsRequestRequestTypeDef definition

class DescribeSenderIdsRequestRequestTypeDef(TypedDict):
    SenderIds: NotRequired[Sequence[SenderIdAndCountryTypeDef]],  # (1)
    Filters: NotRequired[Sequence[SenderIdFilterTypeDef]],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Owner: NotRequired[OwnerType],  # (3)
```

1. See [:material-code-braces: SenderIdAndCountryTypeDef](./type_defs.md#senderidandcountrytypedef) 
2. See [:material-code-braces: SenderIdFilterTypeDef](./type_defs.md#senderidfiltertypedef) 
3. See [:material-code-brackets: OwnerType](./literals.md#ownertype) 
## DescribeSenderIdsResultTypeDef

```python
# DescribeSenderIdsResultTypeDef definition

class DescribeSenderIdsResultTypeDef(TypedDict):
    SenderIds: List[SenderIdInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SenderIdInformationTypeDef](./type_defs.md#senderidinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSpendLimitsResultTypeDef

```python
# DescribeSpendLimitsResultTypeDef definition

class DescribeSpendLimitsResultTypeDef(TypedDict):
    SpendLimits: List[SpendLimitTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SpendLimitTypeDef](./type_defs.md#spendlimittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeVerifiedDestinationNumbersRequestPaginateTypeDef

```python
# DescribeVerifiedDestinationNumbersRequestPaginateTypeDef definition

class DescribeVerifiedDestinationNumbersRequestPaginateTypeDef(TypedDict):
    VerifiedDestinationNumberIds: NotRequired[Sequence[str]],
    DestinationPhoneNumbers: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[VerifiedDestinationNumberFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: VerifiedDestinationNumberFilterTypeDef](./type_defs.md#verifieddestinationnumberfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeVerifiedDestinationNumbersRequestRequestTypeDef

```python
# DescribeVerifiedDestinationNumbersRequestRequestTypeDef definition

class DescribeVerifiedDestinationNumbersRequestRequestTypeDef(TypedDict):
    VerifiedDestinationNumberIds: NotRequired[Sequence[str]],
    DestinationPhoneNumbers: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[VerifiedDestinationNumberFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: VerifiedDestinationNumberFilterTypeDef](./type_defs.md#verifieddestinationnumberfiltertypedef) 
## DescribeVerifiedDestinationNumbersResultTypeDef

```python
# DescribeVerifiedDestinationNumbersResultTypeDef definition

class DescribeVerifiedDestinationNumbersResultTypeDef(TypedDict):
    VerifiedDestinationNumbers: List[VerifiedDestinationNumberInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: VerifiedDestinationNumberInformationTypeDef](./type_defs.md#verifieddestinationnumberinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProtectConfigurationCountryRuleSetResultTypeDef

```python
# GetProtectConfigurationCountryRuleSetResultTypeDef definition

class GetProtectConfigurationCountryRuleSetResultTypeDef(TypedDict):
    ProtectConfigurationArn: str,
    ProtectConfigurationId: str,
    NumberCapability: NumberCapabilityType,  # (1)
    CountryRuleSet: Dict[str, ProtectConfigurationCountryRuleSetInformationTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: NumberCapabilityType](./literals.md#numbercapabilitytype) 
2. See [:material-code-braces: ProtectConfigurationCountryRuleSetInformationTypeDef](./type_defs.md#protectconfigurationcountryrulesetinformationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProtectConfigurationCountryRuleSetRequestRequestTypeDef

```python
# UpdateProtectConfigurationCountryRuleSetRequestRequestTypeDef definition

class UpdateProtectConfigurationCountryRuleSetRequestRequestTypeDef(TypedDict):
    ProtectConfigurationId: str,
    NumberCapability: NumberCapabilityType,  # (1)
    CountryRuleSetUpdates: Mapping[str, ProtectConfigurationCountryRuleSetInformationTypeDef],  # (2)
```

1. See [:material-code-brackets: NumberCapabilityType](./literals.md#numbercapabilitytype) 
2. See [:material-code-braces: ProtectConfigurationCountryRuleSetInformationTypeDef](./type_defs.md#protectconfigurationcountryrulesetinformationtypedef) 
## UpdateProtectConfigurationCountryRuleSetResultTypeDef

```python
# UpdateProtectConfigurationCountryRuleSetResultTypeDef definition

class UpdateProtectConfigurationCountryRuleSetResultTypeDef(TypedDict):
    ProtectConfigurationArn: str,
    ProtectConfigurationId: str,
    NumberCapability: NumberCapabilityType,  # (1)
    CountryRuleSet: Dict[str, ProtectConfigurationCountryRuleSetInformationTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: NumberCapabilityType](./literals.md#numbercapabilitytype) 
2. See [:material-code-braces: ProtectConfigurationCountryRuleSetInformationTypeDef](./type_defs.md#protectconfigurationcountryrulesetinformationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPoolOriginationIdentitiesRequestPaginateTypeDef

```python
# ListPoolOriginationIdentitiesRequestPaginateTypeDef definition

class ListPoolOriginationIdentitiesRequestPaginateTypeDef(TypedDict):
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
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OriginationIdentityMetadataTypeDef](./type_defs.md#originationidentitymetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProtectConfigurationRuleSetNumberOverridesRequestPaginateTypeDef

```python
# ListProtectConfigurationRuleSetNumberOverridesRequestPaginateTypeDef definition

class ListProtectConfigurationRuleSetNumberOverridesRequestPaginateTypeDef(TypedDict):
    ProtectConfigurationId: str,
    Filters: NotRequired[Sequence[ProtectConfigurationRuleSetNumberOverrideFilterItemTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ProtectConfigurationRuleSetNumberOverrideFilterItemTypeDef](./type_defs.md#protectconfigurationrulesetnumberoverridefilteritemtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProtectConfigurationRuleSetNumberOverridesRequestRequestTypeDef

```python
# ListProtectConfigurationRuleSetNumberOverridesRequestRequestTypeDef definition

class ListProtectConfigurationRuleSetNumberOverridesRequestRequestTypeDef(TypedDict):
    ProtectConfigurationId: str,
    Filters: NotRequired[Sequence[ProtectConfigurationRuleSetNumberOverrideFilterItemTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ProtectConfigurationRuleSetNumberOverrideFilterItemTypeDef](./type_defs.md#protectconfigurationrulesetnumberoverridefilteritemtypedef) 
## ListProtectConfigurationRuleSetNumberOverridesResultTypeDef

```python
# ListProtectConfigurationRuleSetNumberOverridesResultTypeDef definition

class ListProtectConfigurationRuleSetNumberOverridesResultTypeDef(TypedDict):
    ProtectConfigurationArn: str,
    ProtectConfigurationId: str,
    RuleSetNumberOverrides: List[ProtectConfigurationRuleSetNumberOverrideTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProtectConfigurationRuleSetNumberOverrideTypeDef](./type_defs.md#protectconfigurationrulesetnumberoverridetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRegistrationAssociationsRequestPaginateTypeDef

```python
# ListRegistrationAssociationsRequestPaginateTypeDef definition

class ListRegistrationAssociationsRequestPaginateTypeDef(TypedDict):
    RegistrationId: str,
    Filters: NotRequired[Sequence[RegistrationAssociationFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: RegistrationAssociationFilterTypeDef](./type_defs.md#registrationassociationfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRegistrationAssociationsRequestRequestTypeDef

```python
# ListRegistrationAssociationsRequestRequestTypeDef definition

class ListRegistrationAssociationsRequestRequestTypeDef(TypedDict):
    RegistrationId: str,
    Filters: NotRequired[Sequence[RegistrationAssociationFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: RegistrationAssociationFilterTypeDef](./type_defs.md#registrationassociationfiltertypedef) 
## ListRegistrationAssociationsResultTypeDef

```python
# ListRegistrationAssociationsResultTypeDef definition

class ListRegistrationAssociationsResultTypeDef(TypedDict):
    RegistrationArn: str,
    RegistrationId: str,
    RegistrationType: str,
    RegistrationAssociations: List[RegistrationAssociationMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RegistrationAssociationMetadataTypeDef](./type_defs.md#registrationassociationmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutProtectConfigurationRuleSetNumberOverrideRequestRequestTypeDef

```python
# PutProtectConfigurationRuleSetNumberOverrideRequestRequestTypeDef definition

class PutProtectConfigurationRuleSetNumberOverrideRequestRequestTypeDef(TypedDict):
    ProtectConfigurationId: str,
    DestinationPhoneNumber: str,
    Action: ProtectConfigurationRuleOverrideActionType,  # (1)
    ClientToken: NotRequired[str],
    ExpirationTimestamp: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: ProtectConfigurationRuleOverrideActionType](./literals.md#protectconfigurationruleoverrideactiontype) 
## RegistrationVersionInformationTypeDef

```python
# RegistrationVersionInformationTypeDef definition

class RegistrationVersionInformationTypeDef(TypedDict):
    VersionNumber: int,
    RegistrationVersionStatus: RegistrationVersionStatusType,  # (1)
    RegistrationVersionStatusHistory: RegistrationVersionStatusHistoryTypeDef,  # (2)
    DeniedReasons: NotRequired[List[RegistrationDeniedReasonInformationTypeDef]],  # (3)
```

1. See [:material-code-brackets: RegistrationVersionStatusType](./literals.md#registrationversionstatustype) 
2. See [:material-code-braces: RegistrationVersionStatusHistoryTypeDef](./type_defs.md#registrationversionstatushistorytypedef) 
3. See [:material-code-braces: RegistrationDeniedReasonInformationTypeDef](./type_defs.md#registrationdeniedreasoninformationtypedef) 
## RegistrationFieldDisplayHintsTypeDef

```python
# RegistrationFieldDisplayHintsTypeDef definition

class RegistrationFieldDisplayHintsTypeDef(TypedDict):
    Title: str,
    ShortDescription: str,
    LongDescription: NotRequired[str],
    DocumentationTitle: NotRequired[str],
    DocumentationLink: NotRequired[str],
    SelectOptionDescriptions: NotRequired[List[SelectOptionDescriptionTypeDef]],  # (1)
    TextValidationDescription: NotRequired[str],
    ExampleTextValue: NotRequired[str],
```

1. See [:material-code-braces: SelectOptionDescriptionTypeDef](./type_defs.md#selectoptiondescriptiontypedef) 
## RegistrationSectionDefinitionTypeDef

```python
# RegistrationSectionDefinitionTypeDef definition

class RegistrationSectionDefinitionTypeDef(TypedDict):
    SectionPath: str,
    DisplayHints: RegistrationSectionDisplayHintsTypeDef,  # (1)
```

1. See [:material-code-braces: RegistrationSectionDisplayHintsTypeDef](./type_defs.md#registrationsectiondisplayhintstypedef) 
## RegistrationTypeDefinitionTypeDef

```python
# RegistrationTypeDefinitionTypeDef definition

class RegistrationTypeDefinitionTypeDef(TypedDict):
    RegistrationType: str,
    DisplayHints: RegistrationTypeDisplayHintsTypeDef,  # (2)
    SupportedAssociations: NotRequired[List[SupportedAssociationTypeDef]],  # (1)
```

1. See [:material-code-braces: SupportedAssociationTypeDef](./type_defs.md#supportedassociationtypedef) 
2. See [:material-code-braces: RegistrationTypeDisplayHintsTypeDef](./type_defs.md#registrationtypedisplayhintstypedef) 
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
    DefaultMessageFeedbackEnabled: NotRequired[bool],
    ProtectConfigurationId: NotRequired[str],
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
    DefaultMessageFeedbackEnabled: bool,
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
## DescribeRegistrationVersionsResultTypeDef

```python
# DescribeRegistrationVersionsResultTypeDef definition

class DescribeRegistrationVersionsResultTypeDef(TypedDict):
    RegistrationArn: str,
    RegistrationId: str,
    RegistrationVersions: List[RegistrationVersionInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RegistrationVersionInformationTypeDef](./type_defs.md#registrationversioninformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegistrationFieldDefinitionTypeDef

```python
# RegistrationFieldDefinitionTypeDef definition

class RegistrationFieldDefinitionTypeDef(TypedDict):
    SectionPath: str,
    FieldPath: str,
    FieldType: FieldTypeType,  # (1)
    FieldRequirement: FieldRequirementType,  # (2)
    DisplayHints: RegistrationFieldDisplayHintsTypeDef,  # (5)
    SelectValidation: NotRequired[SelectValidationTypeDef],  # (3)
    TextValidation: NotRequired[TextValidationTypeDef],  # (4)
```

1. See [:material-code-brackets: FieldTypeType](./literals.md#fieldtypetype) 
2. See [:material-code-brackets: FieldRequirementType](./literals.md#fieldrequirementtype) 
3. See [:material-code-braces: SelectValidationTypeDef](./type_defs.md#selectvalidationtypedef) 
4. See [:material-code-braces: TextValidationTypeDef](./type_defs.md#textvalidationtypedef) 
5. See [:material-code-braces: RegistrationFieldDisplayHintsTypeDef](./type_defs.md#registrationfielddisplayhintstypedef) 
## DescribeRegistrationSectionDefinitionsResultTypeDef

```python
# DescribeRegistrationSectionDefinitionsResultTypeDef definition

class DescribeRegistrationSectionDefinitionsResultTypeDef(TypedDict):
    RegistrationType: str,
    RegistrationSectionDefinitions: List[RegistrationSectionDefinitionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RegistrationSectionDefinitionTypeDef](./type_defs.md#registrationsectiondefinitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRegistrationTypeDefinitionsResultTypeDef

```python
# DescribeRegistrationTypeDefinitionsResultTypeDef definition

class DescribeRegistrationTypeDefinitionsResultTypeDef(TypedDict):
    RegistrationTypeDefinitions: List[RegistrationTypeDefinitionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RegistrationTypeDefinitionTypeDef](./type_defs.md#registrationtypedefinitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeConfigurationSetsResultTypeDef

```python
# DescribeConfigurationSetsResultTypeDef definition

class DescribeConfigurationSetsResultTypeDef(TypedDict):
    ConfigurationSets: List[ConfigurationSetInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfigurationSetInformationTypeDef](./type_defs.md#configurationsetinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRegistrationFieldDefinitionsResultTypeDef

```python
# DescribeRegistrationFieldDefinitionsResultTypeDef definition

class DescribeRegistrationFieldDefinitionsResultTypeDef(TypedDict):
    RegistrationType: str,
    RegistrationFieldDefinitions: List[RegistrationFieldDefinitionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RegistrationFieldDefinitionTypeDef](./type_defs.md#registrationfielddefinitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
