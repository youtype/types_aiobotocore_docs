# Type definitions

> [Index](../README.md) > [SES](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SES](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#ses)
    type annotations stubs module [types-aiobotocore-ses](https://pypi.org/project/types-aiobotocore-ses/).

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


## CloudWatchDestinationUnionTypeDef

```python
# CloudWatchDestinationUnionTypeDef definition

CloudWatchDestinationUnionTypeDef = Union[
    CloudWatchDestinationTypeDef,  # (1)
    CloudWatchDestinationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CloudWatchDestinationTypeDef](./type_defs.md#cloudwatchdestinationtypedef) 
2. See [:material-code-braces: CloudWatchDestinationOutputTypeDef](./type_defs.md#cloudwatchdestinationoutputtypedef) 



## AddHeaderActionTypeDef

```python
# AddHeaderActionTypeDef definition

class AddHeaderActionTypeDef(TypedDict):
    HeaderName: str,
    HeaderValue: str,
```

## ContentTypeDef

```python
# ContentTypeDef definition

class ContentTypeDef(TypedDict):
    Data: str,
    Charset: NotRequired[str],
```

## BounceActionTypeDef

```python
# BounceActionTypeDef definition

class BounceActionTypeDef(TypedDict):
    SmtpReplyCode: str,
    Message: str,
    Sender: str,
    TopicArn: NotRequired[str],
    StatusCode: NotRequired[str],
```

## BulkEmailDestinationStatusTypeDef

```python
# BulkEmailDestinationStatusTypeDef definition

class BulkEmailDestinationStatusTypeDef(TypedDict):
    Status: NotRequired[BulkEmailStatusType],  # (1)
    Error: NotRequired[str],
    MessageId: NotRequired[str],
```

1. See [:material-code-brackets: BulkEmailStatusType](./literals.md#bulkemailstatustype) 
## DestinationTypeDef

```python
# DestinationTypeDef definition

class DestinationTypeDef(TypedDict):
    ToAddresses: NotRequired[Sequence[str]],
    CcAddresses: NotRequired[Sequence[str]],
    BccAddresses: NotRequired[Sequence[str]],
```

## MessageTagTypeDef

```python
# MessageTagTypeDef definition

class MessageTagTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## CloneReceiptRuleSetRequestRequestTypeDef

```python
# CloneReceiptRuleSetRequestRequestTypeDef definition

class CloneReceiptRuleSetRequestRequestTypeDef(TypedDict):
    RuleSetName: str,
    OriginalRuleSetName: str,
```

## CloudWatchDimensionConfigurationTypeDef

```python
# CloudWatchDimensionConfigurationTypeDef definition

class CloudWatchDimensionConfigurationTypeDef(TypedDict):
    DimensionName: str,
    DimensionValueSource: DimensionValueSourceType,  # (1)
    DefaultDimensionValue: str,
```

1. See [:material-code-brackets: DimensionValueSourceType](./literals.md#dimensionvaluesourcetype) 
## ConfigurationSetTypeDef

```python
# ConfigurationSetTypeDef definition

class ConfigurationSetTypeDef(TypedDict):
    Name: str,
```

## ConnectActionTypeDef

```python
# ConnectActionTypeDef definition

class ConnectActionTypeDef(TypedDict):
    InstanceARN: str,
    IAMRoleARN: str,
```

## TrackingOptionsTypeDef

```python
# TrackingOptionsTypeDef definition

class TrackingOptionsTypeDef(TypedDict):
    CustomRedirectDomain: NotRequired[str],
```

## CreateCustomVerificationEmailTemplateRequestRequestTypeDef

```python
# CreateCustomVerificationEmailTemplateRequestRequestTypeDef definition

class CreateCustomVerificationEmailTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
    FromEmailAddress: str,
    TemplateSubject: str,
    TemplateContent: str,
    SuccessRedirectionURL: str,
    FailureRedirectionURL: str,
```

## CreateReceiptRuleSetRequestRequestTypeDef

```python
# CreateReceiptRuleSetRequestRequestTypeDef definition

class CreateReceiptRuleSetRequestRequestTypeDef(TypedDict):
    RuleSetName: str,
```

## TemplateTypeDef

```python
# TemplateTypeDef definition

class TemplateTypeDef(TypedDict):
    TemplateName: str,
    SubjectPart: NotRequired[str],
    TextPart: NotRequired[str],
    HtmlPart: NotRequired[str],
```

## CustomVerificationEmailTemplateTypeDef

```python
# CustomVerificationEmailTemplateTypeDef definition

class CustomVerificationEmailTemplateTypeDef(TypedDict):
    TemplateName: NotRequired[str],
    FromEmailAddress: NotRequired[str],
    TemplateSubject: NotRequired[str],
    SuccessRedirectionURL: NotRequired[str],
    FailureRedirectionURL: NotRequired[str],
```

## DeleteConfigurationSetEventDestinationRequestRequestTypeDef

```python
# DeleteConfigurationSetEventDestinationRequestRequestTypeDef definition

class DeleteConfigurationSetEventDestinationRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    EventDestinationName: str,
```

## DeleteConfigurationSetRequestRequestTypeDef

```python
# DeleteConfigurationSetRequestRequestTypeDef definition

class DeleteConfigurationSetRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
```

## DeleteConfigurationSetTrackingOptionsRequestRequestTypeDef

```python
# DeleteConfigurationSetTrackingOptionsRequestRequestTypeDef definition

class DeleteConfigurationSetTrackingOptionsRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
```

## DeleteCustomVerificationEmailTemplateRequestRequestTypeDef

```python
# DeleteCustomVerificationEmailTemplateRequestRequestTypeDef definition

class DeleteCustomVerificationEmailTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
```

## DeleteIdentityPolicyRequestRequestTypeDef

```python
# DeleteIdentityPolicyRequestRequestTypeDef definition

class DeleteIdentityPolicyRequestRequestTypeDef(TypedDict):
    Identity: str,
    PolicyName: str,
```

## DeleteIdentityRequestRequestTypeDef

```python
# DeleteIdentityRequestRequestTypeDef definition

class DeleteIdentityRequestRequestTypeDef(TypedDict):
    Identity: str,
```

## DeleteReceiptFilterRequestRequestTypeDef

```python
# DeleteReceiptFilterRequestRequestTypeDef definition

class DeleteReceiptFilterRequestRequestTypeDef(TypedDict):
    FilterName: str,
```

## DeleteReceiptRuleRequestRequestTypeDef

```python
# DeleteReceiptRuleRequestRequestTypeDef definition

class DeleteReceiptRuleRequestRequestTypeDef(TypedDict):
    RuleSetName: str,
    RuleName: str,
```

## DeleteReceiptRuleSetRequestRequestTypeDef

```python
# DeleteReceiptRuleSetRequestRequestTypeDef definition

class DeleteReceiptRuleSetRequestRequestTypeDef(TypedDict):
    RuleSetName: str,
```

## DeleteTemplateRequestRequestTypeDef

```python
# DeleteTemplateRequestRequestTypeDef definition

class DeleteTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
```

## DeleteVerifiedEmailAddressRequestRequestTypeDef

```python
# DeleteVerifiedEmailAddressRequestRequestTypeDef definition

class DeleteVerifiedEmailAddressRequestRequestTypeDef(TypedDict):
    EmailAddress: str,
```

## DeliveryOptionsTypeDef

```python
# DeliveryOptionsTypeDef definition

class DeliveryOptionsTypeDef(TypedDict):
    TlsPolicy: NotRequired[TlsPolicyType],  # (1)
```

1. See [:material-code-brackets: TlsPolicyType](./literals.md#tlspolicytype) 
## ReceiptRuleSetMetadataTypeDef

```python
# ReceiptRuleSetMetadataTypeDef definition

class ReceiptRuleSetMetadataTypeDef(TypedDict):
    Name: NotRequired[str],
    CreatedTimestamp: NotRequired[datetime],
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

## DescribeConfigurationSetRequestRequestTypeDef

```python
# DescribeConfigurationSetRequestRequestTypeDef definition

class DescribeConfigurationSetRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    ConfigurationSetAttributeNames: NotRequired[Sequence[ConfigurationSetAttributeType]],  # (1)
```

1. See [:material-code-brackets: ConfigurationSetAttributeType](./literals.md#configurationsetattributetype) 
## ReputationOptionsTypeDef

```python
# ReputationOptionsTypeDef definition

class ReputationOptionsTypeDef(TypedDict):
    SendingEnabled: NotRequired[bool],
    ReputationMetricsEnabled: NotRequired[bool],
    LastFreshStart: NotRequired[datetime],
```

## DescribeReceiptRuleRequestRequestTypeDef

```python
# DescribeReceiptRuleRequestRequestTypeDef definition

class DescribeReceiptRuleRequestRequestTypeDef(TypedDict):
    RuleSetName: str,
    RuleName: str,
```

## DescribeReceiptRuleSetRequestRequestTypeDef

```python
# DescribeReceiptRuleSetRequestRequestTypeDef definition

class DescribeReceiptRuleSetRequestRequestTypeDef(TypedDict):
    RuleSetName: str,
```

## KinesisFirehoseDestinationTypeDef

```python
# KinesisFirehoseDestinationTypeDef definition

class KinesisFirehoseDestinationTypeDef(TypedDict):
    IAMRoleARN: str,
    DeliveryStreamARN: str,
```

## SNSDestinationTypeDef

```python
# SNSDestinationTypeDef definition

class SNSDestinationTypeDef(TypedDict):
    TopicARN: str,
```

## ExtensionFieldTypeDef

```python
# ExtensionFieldTypeDef definition

class ExtensionFieldTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## GetCustomVerificationEmailTemplateRequestRequestTypeDef

```python
# GetCustomVerificationEmailTemplateRequestRequestTypeDef definition

class GetCustomVerificationEmailTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
```

## GetIdentityDkimAttributesRequestRequestTypeDef

```python
# GetIdentityDkimAttributesRequestRequestTypeDef definition

class GetIdentityDkimAttributesRequestRequestTypeDef(TypedDict):
    Identities: Sequence[str],
```

## IdentityDkimAttributesTypeDef

```python
# IdentityDkimAttributesTypeDef definition

class IdentityDkimAttributesTypeDef(TypedDict):
    DkimEnabled: bool,
    DkimVerificationStatus: VerificationStatusType,  # (1)
    DkimTokens: NotRequired[List[str]],
```

1. See [:material-code-brackets: VerificationStatusType](./literals.md#verificationstatustype) 
## GetIdentityMailFromDomainAttributesRequestRequestTypeDef

```python
# GetIdentityMailFromDomainAttributesRequestRequestTypeDef definition

class GetIdentityMailFromDomainAttributesRequestRequestTypeDef(TypedDict):
    Identities: Sequence[str],
```

## IdentityMailFromDomainAttributesTypeDef

```python
# IdentityMailFromDomainAttributesTypeDef definition

class IdentityMailFromDomainAttributesTypeDef(TypedDict):
    MailFromDomain: str,
    MailFromDomainStatus: CustomMailFromStatusType,  # (1)
    BehaviorOnMXFailure: BehaviorOnMXFailureType,  # (2)
```

1. See [:material-code-brackets: CustomMailFromStatusType](./literals.md#custommailfromstatustype) 
2. See [:material-code-brackets: BehaviorOnMXFailureType](./literals.md#behavioronmxfailuretype) 
## GetIdentityNotificationAttributesRequestRequestTypeDef

```python
# GetIdentityNotificationAttributesRequestRequestTypeDef definition

class GetIdentityNotificationAttributesRequestRequestTypeDef(TypedDict):
    Identities: Sequence[str],
```

## IdentityNotificationAttributesTypeDef

```python
# IdentityNotificationAttributesTypeDef definition

class IdentityNotificationAttributesTypeDef(TypedDict):
    BounceTopic: str,
    ComplaintTopic: str,
    DeliveryTopic: str,
    ForwardingEnabled: bool,
    HeadersInBounceNotificationsEnabled: NotRequired[bool],
    HeadersInComplaintNotificationsEnabled: NotRequired[bool],
    HeadersInDeliveryNotificationsEnabled: NotRequired[bool],
```

## GetIdentityPoliciesRequestRequestTypeDef

```python
# GetIdentityPoliciesRequestRequestTypeDef definition

class GetIdentityPoliciesRequestRequestTypeDef(TypedDict):
    Identity: str,
    PolicyNames: Sequence[str],
```

## GetIdentityVerificationAttributesRequestRequestTypeDef

```python
# GetIdentityVerificationAttributesRequestRequestTypeDef definition

class GetIdentityVerificationAttributesRequestRequestTypeDef(TypedDict):
    Identities: Sequence[str],
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## IdentityVerificationAttributesTypeDef

```python
# IdentityVerificationAttributesTypeDef definition

class IdentityVerificationAttributesTypeDef(TypedDict):
    VerificationStatus: VerificationStatusType,  # (1)
    VerificationToken: NotRequired[str],
```

1. See [:material-code-brackets: VerificationStatusType](./literals.md#verificationstatustype) 
## SendDataPointTypeDef

```python
# SendDataPointTypeDef definition

class SendDataPointTypeDef(TypedDict):
    Timestamp: NotRequired[datetime],
    DeliveryAttempts: NotRequired[int],
    Bounces: NotRequired[int],
    Complaints: NotRequired[int],
    Rejects: NotRequired[int],
```

## GetTemplateRequestRequestTypeDef

```python
# GetTemplateRequestRequestTypeDef definition

class GetTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
```

## LambdaActionTypeDef

```python
# LambdaActionTypeDef definition

class LambdaActionTypeDef(TypedDict):
    FunctionArn: str,
    TopicArn: NotRequired[str],
    InvocationType: NotRequired[InvocationTypeType],  # (1)
```

1. See [:material-code-brackets: InvocationTypeType](./literals.md#invocationtypetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListConfigurationSetsRequestRequestTypeDef

```python
# ListConfigurationSetsRequestRequestTypeDef definition

class ListConfigurationSetsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListCustomVerificationEmailTemplatesRequestRequestTypeDef

```python
# ListCustomVerificationEmailTemplatesRequestRequestTypeDef definition

class ListCustomVerificationEmailTemplatesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListIdentitiesRequestRequestTypeDef

```python
# ListIdentitiesRequestRequestTypeDef definition

class ListIdentitiesRequestRequestTypeDef(TypedDict):
    IdentityType: NotRequired[IdentityTypeType],  # (1)
    NextToken: NotRequired[str],
    MaxItems: NotRequired[int],
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
## ListIdentityPoliciesRequestRequestTypeDef

```python
# ListIdentityPoliciesRequestRequestTypeDef definition

class ListIdentityPoliciesRequestRequestTypeDef(TypedDict):
    Identity: str,
```

## ListReceiptRuleSetsRequestRequestTypeDef

```python
# ListReceiptRuleSetsRequestRequestTypeDef definition

class ListReceiptRuleSetsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
```

## ListTemplatesRequestRequestTypeDef

```python
# ListTemplatesRequestRequestTypeDef definition

class ListTemplatesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxItems: NotRequired[int],
```

## TemplateMetadataTypeDef

```python
# TemplateMetadataTypeDef definition

class TemplateMetadataTypeDef(TypedDict):
    Name: NotRequired[str],
    CreatedTimestamp: NotRequired[datetime],
```

## PutIdentityPolicyRequestRequestTypeDef

```python
# PutIdentityPolicyRequestRequestTypeDef definition

class PutIdentityPolicyRequestRequestTypeDef(TypedDict):
    Identity: str,
    PolicyName: str,
    Policy: str,
```

## S3ActionTypeDef

```python
# S3ActionTypeDef definition

class S3ActionTypeDef(TypedDict):
    BucketName: str,
    TopicArn: NotRequired[str],
    ObjectKeyPrefix: NotRequired[str],
    KmsKeyArn: NotRequired[str],
    IamRoleArn: NotRequired[str],
```

## SNSActionTypeDef

```python
# SNSActionTypeDef definition

class SNSActionTypeDef(TypedDict):
    TopicArn: str,
    Encoding: NotRequired[SNSActionEncodingType],  # (1)
```

1. See [:material-code-brackets: SNSActionEncodingType](./literals.md#snsactionencodingtype) 
## StopActionTypeDef

```python
# StopActionTypeDef definition

class StopActionTypeDef(TypedDict):
    Scope: StopScopeType,  # (1)
    TopicArn: NotRequired[str],
```

1. See [:material-code-brackets: StopScopeType](./literals.md#stopscopetype) 
## WorkmailActionTypeDef

```python
# WorkmailActionTypeDef definition

class WorkmailActionTypeDef(TypedDict):
    OrganizationArn: str,
    TopicArn: NotRequired[str],
```

## ReceiptIpFilterTypeDef

```python
# ReceiptIpFilterTypeDef definition

class ReceiptIpFilterTypeDef(TypedDict):
    Policy: ReceiptFilterPolicyType,  # (1)
    Cidr: str,
```

1. See [:material-code-brackets: ReceiptFilterPolicyType](./literals.md#receiptfilterpolicytype) 
## ReorderReceiptRuleSetRequestRequestTypeDef

```python
# ReorderReceiptRuleSetRequestRequestTypeDef definition

class ReorderReceiptRuleSetRequestRequestTypeDef(TypedDict):
    RuleSetName: str,
    RuleNames: Sequence[str],
```

## SendCustomVerificationEmailRequestRequestTypeDef

```python
# SendCustomVerificationEmailRequestRequestTypeDef definition

class SendCustomVerificationEmailRequestRequestTypeDef(TypedDict):
    EmailAddress: str,
    TemplateName: str,
    ConfigurationSetName: NotRequired[str],
```

## SetActiveReceiptRuleSetRequestRequestTypeDef

```python
# SetActiveReceiptRuleSetRequestRequestTypeDef definition

class SetActiveReceiptRuleSetRequestRequestTypeDef(TypedDict):
    RuleSetName: NotRequired[str],
```

## SetIdentityDkimEnabledRequestRequestTypeDef

```python
# SetIdentityDkimEnabledRequestRequestTypeDef definition

class SetIdentityDkimEnabledRequestRequestTypeDef(TypedDict):
    Identity: str,
    DkimEnabled: bool,
```

## SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef

```python
# SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef definition

class SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef(TypedDict):
    Identity: str,
    ForwardingEnabled: bool,
```

## SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef

```python
# SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef definition

class SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef(TypedDict):
    Identity: str,
    NotificationType: NotificationTypeType,  # (1)
    Enabled: bool,
```

1. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
## SetIdentityMailFromDomainRequestRequestTypeDef

```python
# SetIdentityMailFromDomainRequestRequestTypeDef definition

class SetIdentityMailFromDomainRequestRequestTypeDef(TypedDict):
    Identity: str,
    MailFromDomain: NotRequired[str],
    BehaviorOnMXFailure: NotRequired[BehaviorOnMXFailureType],  # (1)
```

1. See [:material-code-brackets: BehaviorOnMXFailureType](./literals.md#behavioronmxfailuretype) 
## SetIdentityNotificationTopicRequestRequestTypeDef

```python
# SetIdentityNotificationTopicRequestRequestTypeDef definition

class SetIdentityNotificationTopicRequestRequestTypeDef(TypedDict):
    Identity: str,
    NotificationType: NotificationTypeType,  # (1)
    SnsTopic: NotRequired[str],
```

1. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
## SetReceiptRulePositionRequestRequestTypeDef

```python
# SetReceiptRulePositionRequestRequestTypeDef definition

class SetReceiptRulePositionRequestRequestTypeDef(TypedDict):
    RuleSetName: str,
    RuleName: str,
    After: NotRequired[str],
```

## TestRenderTemplateRequestRequestTypeDef

```python
# TestRenderTemplateRequestRequestTypeDef definition

class TestRenderTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
    TemplateData: str,
```

## UpdateAccountSendingEnabledRequestRequestTypeDef

```python
# UpdateAccountSendingEnabledRequestRequestTypeDef definition

class UpdateAccountSendingEnabledRequestRequestTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef

```python
# UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef definition

class UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    Enabled: bool,
```

## UpdateConfigurationSetSendingEnabledRequestRequestTypeDef

```python
# UpdateConfigurationSetSendingEnabledRequestRequestTypeDef definition

class UpdateConfigurationSetSendingEnabledRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    Enabled: bool,
```

## UpdateCustomVerificationEmailTemplateRequestRequestTypeDef

```python
# UpdateCustomVerificationEmailTemplateRequestRequestTypeDef definition

class UpdateCustomVerificationEmailTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
    FromEmailAddress: NotRequired[str],
    TemplateSubject: NotRequired[str],
    TemplateContent: NotRequired[str],
    SuccessRedirectionURL: NotRequired[str],
    FailureRedirectionURL: NotRequired[str],
```

## VerifyDomainDkimRequestRequestTypeDef

```python
# VerifyDomainDkimRequestRequestTypeDef definition

class VerifyDomainDkimRequestRequestTypeDef(TypedDict):
    Domain: str,
```

## VerifyDomainIdentityRequestRequestTypeDef

```python
# VerifyDomainIdentityRequestRequestTypeDef definition

class VerifyDomainIdentityRequestRequestTypeDef(TypedDict):
    Domain: str,
```

## VerifyEmailAddressRequestRequestTypeDef

```python
# VerifyEmailAddressRequestRequestTypeDef definition

class VerifyEmailAddressRequestRequestTypeDef(TypedDict):
    EmailAddress: str,
```

## VerifyEmailIdentityRequestRequestTypeDef

```python
# VerifyEmailIdentityRequestRequestTypeDef definition

class VerifyEmailIdentityRequestRequestTypeDef(TypedDict):
    EmailAddress: str,
```

## RawMessageTypeDef

```python
# RawMessageTypeDef definition

class RawMessageTypeDef(TypedDict):
    Data: BlobTypeDef,
```

## BodyTypeDef

```python
# BodyTypeDef definition

class BodyTypeDef(TypedDict):
    Text: NotRequired[ContentTypeDef],  # (1)
    Html: NotRequired[ContentTypeDef],  # (1)
```

1. See [:material-code-braces: ContentTypeDef](./type_defs.md#contenttypedef) 
2. See [:material-code-braces: ContentTypeDef](./type_defs.md#contenttypedef) 
## BulkEmailDestinationTypeDef

```python
# BulkEmailDestinationTypeDef definition

class BulkEmailDestinationTypeDef(TypedDict):
    Destination: DestinationTypeDef,  # (1)
    ReplacementTags: NotRequired[Sequence[MessageTagTypeDef]],  # (2)
    ReplacementTemplateData: NotRequired[str],
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: MessageTagTypeDef](./type_defs.md#messagetagtypedef) 
## SendTemplatedEmailRequestRequestTypeDef

```python
# SendTemplatedEmailRequestRequestTypeDef definition

class SendTemplatedEmailRequestRequestTypeDef(TypedDict):
    Source: str,
    Destination: DestinationTypeDef,  # (1)
    Template: str,
    TemplateData: str,
    ReplyToAddresses: NotRequired[Sequence[str]],
    ReturnPath: NotRequired[str],
    SourceArn: NotRequired[str],
    ReturnPathArn: NotRequired[str],
    Tags: NotRequired[Sequence[MessageTagTypeDef]],  # (2)
    ConfigurationSetName: NotRequired[str],
    TemplateArn: NotRequired[str],
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: MessageTagTypeDef](./type_defs.md#messagetagtypedef) 
## CloudWatchDestinationOutputTypeDef

```python
# CloudWatchDestinationOutputTypeDef definition

class CloudWatchDestinationOutputTypeDef(TypedDict):
    DimensionConfigurations: List[CloudWatchDimensionConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: CloudWatchDimensionConfigurationTypeDef](./type_defs.md#cloudwatchdimensionconfigurationtypedef) 
## CloudWatchDestinationTypeDef

```python
# CloudWatchDestinationTypeDef definition

class CloudWatchDestinationTypeDef(TypedDict):
    DimensionConfigurations: Sequence[CloudWatchDimensionConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: CloudWatchDimensionConfigurationTypeDef](./type_defs.md#cloudwatchdimensionconfigurationtypedef) 
## CreateConfigurationSetRequestRequestTypeDef

```python
# CreateConfigurationSetRequestRequestTypeDef definition

class CreateConfigurationSetRequestRequestTypeDef(TypedDict):
    ConfigurationSet: ConfigurationSetTypeDef,  # (1)
```

1. See [:material-code-braces: ConfigurationSetTypeDef](./type_defs.md#configurationsettypedef) 
## CreateConfigurationSetTrackingOptionsRequestRequestTypeDef

```python
# CreateConfigurationSetTrackingOptionsRequestRequestTypeDef definition

class CreateConfigurationSetTrackingOptionsRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    TrackingOptions: TrackingOptionsTypeDef,  # (1)
```

1. See [:material-code-braces: TrackingOptionsTypeDef](./type_defs.md#trackingoptionstypedef) 
## UpdateConfigurationSetTrackingOptionsRequestRequestTypeDef

```python
# UpdateConfigurationSetTrackingOptionsRequestRequestTypeDef definition

class UpdateConfigurationSetTrackingOptionsRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    TrackingOptions: TrackingOptionsTypeDef,  # (1)
```

1. See [:material-code-braces: TrackingOptionsTypeDef](./type_defs.md#trackingoptionstypedef) 
## CreateTemplateRequestRequestTypeDef

```python
# CreateTemplateRequestRequestTypeDef definition

class CreateTemplateRequestRequestTypeDef(TypedDict):
    Template: TemplateTypeDef,  # (1)
```

1. See [:material-code-braces: TemplateTypeDef](./type_defs.md#templatetypedef) 
## UpdateTemplateRequestRequestTypeDef

```python
# UpdateTemplateRequestRequestTypeDef definition

class UpdateTemplateRequestRequestTypeDef(TypedDict):
    Template: TemplateTypeDef,  # (1)
```

1. See [:material-code-braces: TemplateTypeDef](./type_defs.md#templatetypedef) 
## PutConfigurationSetDeliveryOptionsRequestRequestTypeDef

```python
# PutConfigurationSetDeliveryOptionsRequestRequestTypeDef definition

class PutConfigurationSetDeliveryOptionsRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    DeliveryOptions: NotRequired[DeliveryOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: DeliveryOptionsTypeDef](./type_defs.md#deliveryoptionstypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccountSendingEnabledResponseTypeDef

```python
# GetAccountSendingEnabledResponseTypeDef definition

class GetAccountSendingEnabledResponseTypeDef(TypedDict):
    Enabled: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCustomVerificationEmailTemplateResponseTypeDef

```python
# GetCustomVerificationEmailTemplateResponseTypeDef definition

class GetCustomVerificationEmailTemplateResponseTypeDef(TypedDict):
    TemplateName: str,
    FromEmailAddress: str,
    TemplateSubject: str,
    TemplateContent: str,
    SuccessRedirectionURL: str,
    FailureRedirectionURL: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIdentityPoliciesResponseTypeDef

```python
# GetIdentityPoliciesResponseTypeDef definition

class GetIdentityPoliciesResponseTypeDef(TypedDict):
    Policies: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSendQuotaResponseTypeDef

```python
# GetSendQuotaResponseTypeDef definition

class GetSendQuotaResponseTypeDef(TypedDict):
    Max24HourSend: float,
    MaxSendRate: float,
    SentLast24Hours: float,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTemplateResponseTypeDef

```python
# GetTemplateResponseTypeDef definition

class GetTemplateResponseTypeDef(TypedDict):
    Template: TemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TemplateTypeDef](./type_defs.md#templatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfigurationSetsResponseTypeDef

```python
# ListConfigurationSetsResponseTypeDef definition

class ListConfigurationSetsResponseTypeDef(TypedDict):
    ConfigurationSets: List[ConfigurationSetTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfigurationSetTypeDef](./type_defs.md#configurationsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCustomVerificationEmailTemplatesResponseTypeDef

```python
# ListCustomVerificationEmailTemplatesResponseTypeDef definition

class ListCustomVerificationEmailTemplatesResponseTypeDef(TypedDict):
    CustomVerificationEmailTemplates: List[CustomVerificationEmailTemplateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CustomVerificationEmailTemplateTypeDef](./type_defs.md#customverificationemailtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIdentitiesResponseTypeDef

```python
# ListIdentitiesResponseTypeDef definition

class ListIdentitiesResponseTypeDef(TypedDict):
    Identities: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIdentityPoliciesResponseTypeDef

```python
# ListIdentityPoliciesResponseTypeDef definition

class ListIdentityPoliciesResponseTypeDef(TypedDict):
    PolicyNames: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReceiptRuleSetsResponseTypeDef

```python
# ListReceiptRuleSetsResponseTypeDef definition

class ListReceiptRuleSetsResponseTypeDef(TypedDict):
    RuleSets: List[ReceiptRuleSetMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ReceiptRuleSetMetadataTypeDef](./type_defs.md#receiptrulesetmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVerifiedEmailAddressesResponseTypeDef

```python
# ListVerifiedEmailAddressesResponseTypeDef definition

class ListVerifiedEmailAddressesResponseTypeDef(TypedDict):
    VerifiedEmailAddresses: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendBounceResponseTypeDef

```python
# SendBounceResponseTypeDef definition

class SendBounceResponseTypeDef(TypedDict):
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendBulkTemplatedEmailResponseTypeDef

```python
# SendBulkTemplatedEmailResponseTypeDef definition

class SendBulkTemplatedEmailResponseTypeDef(TypedDict):
    Status: List[BulkEmailDestinationStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BulkEmailDestinationStatusTypeDef](./type_defs.md#bulkemaildestinationstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendCustomVerificationEmailResponseTypeDef

```python
# SendCustomVerificationEmailResponseTypeDef definition

class SendCustomVerificationEmailResponseTypeDef(TypedDict):
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendEmailResponseTypeDef

```python
# SendEmailResponseTypeDef definition

class SendEmailResponseTypeDef(TypedDict):
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendRawEmailResponseTypeDef

```python
# SendRawEmailResponseTypeDef definition

class SendRawEmailResponseTypeDef(TypedDict):
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendTemplatedEmailResponseTypeDef

```python
# SendTemplatedEmailResponseTypeDef definition

class SendTemplatedEmailResponseTypeDef(TypedDict):
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestRenderTemplateResponseTypeDef

```python
# TestRenderTemplateResponseTypeDef definition

class TestRenderTemplateResponseTypeDef(TypedDict):
    RenderedTemplate: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VerifyDomainDkimResponseTypeDef

```python
# VerifyDomainDkimResponseTypeDef definition

class VerifyDomainDkimResponseTypeDef(TypedDict):
    DkimTokens: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VerifyDomainIdentityResponseTypeDef

```python
# VerifyDomainIdentityResponseTypeDef definition

class VerifyDomainIdentityResponseTypeDef(TypedDict):
    VerificationToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIdentityDkimAttributesResponseTypeDef

```python
# GetIdentityDkimAttributesResponseTypeDef definition

class GetIdentityDkimAttributesResponseTypeDef(TypedDict):
    DkimAttributes: Dict[str, IdentityDkimAttributesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityDkimAttributesTypeDef](./type_defs.md#identitydkimattributestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIdentityMailFromDomainAttributesResponseTypeDef

```python
# GetIdentityMailFromDomainAttributesResponseTypeDef definition

class GetIdentityMailFromDomainAttributesResponseTypeDef(TypedDict):
    MailFromDomainAttributes: Dict[str, IdentityMailFromDomainAttributesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityMailFromDomainAttributesTypeDef](./type_defs.md#identitymailfromdomainattributestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIdentityNotificationAttributesResponseTypeDef

```python
# GetIdentityNotificationAttributesResponseTypeDef definition

class GetIdentityNotificationAttributesResponseTypeDef(TypedDict):
    NotificationAttributes: Dict[str, IdentityNotificationAttributesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityNotificationAttributesTypeDef](./type_defs.md#identitynotificationattributestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIdentityVerificationAttributesRequestWaitTypeDef

```python
# GetIdentityVerificationAttributesRequestWaitTypeDef definition

class GetIdentityVerificationAttributesRequestWaitTypeDef(TypedDict):
    Identities: Sequence[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetIdentityVerificationAttributesResponseTypeDef

```python
# GetIdentityVerificationAttributesResponseTypeDef definition

class GetIdentityVerificationAttributesResponseTypeDef(TypedDict):
    VerificationAttributes: Dict[str, IdentityVerificationAttributesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityVerificationAttributesTypeDef](./type_defs.md#identityverificationattributestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSendStatisticsResponseTypeDef

```python
# GetSendStatisticsResponseTypeDef definition

class GetSendStatisticsResponseTypeDef(TypedDict):
    SendDataPoints: List[SendDataPointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SendDataPointTypeDef](./type_defs.md#senddatapointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfigurationSetsRequestPaginateTypeDef

```python
# ListConfigurationSetsRequestPaginateTypeDef definition

class ListConfigurationSetsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCustomVerificationEmailTemplatesRequestPaginateTypeDef

```python
# ListCustomVerificationEmailTemplatesRequestPaginateTypeDef definition

class ListCustomVerificationEmailTemplatesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIdentitiesRequestPaginateTypeDef

```python
# ListIdentitiesRequestPaginateTypeDef definition

class ListIdentitiesRequestPaginateTypeDef(TypedDict):
    IdentityType: NotRequired[IdentityTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReceiptRuleSetsRequestPaginateTypeDef

```python
# ListReceiptRuleSetsRequestPaginateTypeDef definition

class ListReceiptRuleSetsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTemplatesRequestPaginateTypeDef

```python
# ListTemplatesRequestPaginateTypeDef definition

class ListTemplatesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTemplatesResponseTypeDef

```python
# ListTemplatesResponseTypeDef definition

class ListTemplatesResponseTypeDef(TypedDict):
    TemplatesMetadata: List[TemplateMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TemplateMetadataTypeDef](./type_defs.md#templatemetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MessageDsnTypeDef

```python
# MessageDsnTypeDef definition

class MessageDsnTypeDef(TypedDict):
    ReportingMta: str,
    ArrivalDate: NotRequired[TimestampTypeDef],
    ExtensionFields: NotRequired[Sequence[ExtensionFieldTypeDef]],  # (1)
```

1. See [:material-code-braces: ExtensionFieldTypeDef](./type_defs.md#extensionfieldtypedef) 
## RecipientDsnFieldsTypeDef

```python
# RecipientDsnFieldsTypeDef definition

class RecipientDsnFieldsTypeDef(TypedDict):
    Action: DsnActionType,  # (1)
    Status: str,
    FinalRecipient: NotRequired[str],
    RemoteMta: NotRequired[str],
    DiagnosticCode: NotRequired[str],
    LastAttemptDate: NotRequired[TimestampTypeDef],
    ExtensionFields: NotRequired[Sequence[ExtensionFieldTypeDef]],  # (2)
```

1. See [:material-code-brackets: DsnActionType](./literals.md#dsnactiontype) 
2. See [:material-code-braces: ExtensionFieldTypeDef](./type_defs.md#extensionfieldtypedef) 
## ReceiptActionTypeDef

```python
# ReceiptActionTypeDef definition

class ReceiptActionTypeDef(TypedDict):
    S3Action: NotRequired[S3ActionTypeDef],  # (1)
    BounceAction: NotRequired[BounceActionTypeDef],  # (2)
    WorkmailAction: NotRequired[WorkmailActionTypeDef],  # (3)
    LambdaAction: NotRequired[LambdaActionTypeDef],  # (4)
    StopAction: NotRequired[StopActionTypeDef],  # (5)
    AddHeaderAction: NotRequired[AddHeaderActionTypeDef],  # (6)
    SNSAction: NotRequired[SNSActionTypeDef],  # (7)
    ConnectAction: NotRequired[ConnectActionTypeDef],  # (8)
```

1. See [:material-code-braces: S3ActionTypeDef](./type_defs.md#s3actiontypedef) 
2. See [:material-code-braces: BounceActionTypeDef](./type_defs.md#bounceactiontypedef) 
3. See [:material-code-braces: WorkmailActionTypeDef](./type_defs.md#workmailactiontypedef) 
4. See [:material-code-braces: LambdaActionTypeDef](./type_defs.md#lambdaactiontypedef) 
5. See [:material-code-braces: StopActionTypeDef](./type_defs.md#stopactiontypedef) 
6. See [:material-code-braces: AddHeaderActionTypeDef](./type_defs.md#addheaderactiontypedef) 
7. See [:material-code-braces: SNSActionTypeDef](./type_defs.md#snsactiontypedef) 
8. See [:material-code-braces: ConnectActionTypeDef](./type_defs.md#connectactiontypedef) 
## ReceiptFilterTypeDef

```python
# ReceiptFilterTypeDef definition

class ReceiptFilterTypeDef(TypedDict):
    Name: str,
    IpFilter: ReceiptIpFilterTypeDef,  # (1)
```

1. See [:material-code-braces: ReceiptIpFilterTypeDef](./type_defs.md#receiptipfiltertypedef) 
## SendRawEmailRequestRequestTypeDef

```python
# SendRawEmailRequestRequestTypeDef definition

class SendRawEmailRequestRequestTypeDef(TypedDict):
    RawMessage: RawMessageTypeDef,  # (1)
    Source: NotRequired[str],
    Destinations: NotRequired[Sequence[str]],
    FromArn: NotRequired[str],
    SourceArn: NotRequired[str],
    ReturnPathArn: NotRequired[str],
    Tags: NotRequired[Sequence[MessageTagTypeDef]],  # (2)
    ConfigurationSetName: NotRequired[str],
```

1. See [:material-code-braces: RawMessageTypeDef](./type_defs.md#rawmessagetypedef) 
2. See [:material-code-braces: MessageTagTypeDef](./type_defs.md#messagetagtypedef) 
## MessageTypeDef

```python
# MessageTypeDef definition

class MessageTypeDef(TypedDict):
    Subject: ContentTypeDef,  # (1)
    Body: BodyTypeDef,  # (2)
```

1. See [:material-code-braces: ContentTypeDef](./type_defs.md#contenttypedef) 
2. See [:material-code-braces: BodyTypeDef](./type_defs.md#bodytypedef) 
## SendBulkTemplatedEmailRequestRequestTypeDef

```python
# SendBulkTemplatedEmailRequestRequestTypeDef definition

class SendBulkTemplatedEmailRequestRequestTypeDef(TypedDict):
    Source: str,
    Template: str,
    DefaultTemplateData: str,
    Destinations: Sequence[BulkEmailDestinationTypeDef],  # (1)
    SourceArn: NotRequired[str],
    ReplyToAddresses: NotRequired[Sequence[str]],
    ReturnPath: NotRequired[str],
    ReturnPathArn: NotRequired[str],
    ConfigurationSetName: NotRequired[str],
    DefaultTags: NotRequired[Sequence[MessageTagTypeDef]],  # (2)
    TemplateArn: NotRequired[str],
```

1. See [:material-code-braces: BulkEmailDestinationTypeDef](./type_defs.md#bulkemaildestinationtypedef) 
2. See [:material-code-braces: MessageTagTypeDef](./type_defs.md#messagetagtypedef) 
## EventDestinationOutputTypeDef

```python
# EventDestinationOutputTypeDef definition

class EventDestinationOutputTypeDef(TypedDict):
    Name: str,
    MatchingEventTypes: List[EventTypeType],  # (1)
    Enabled: NotRequired[bool],
    KinesisFirehoseDestination: NotRequired[KinesisFirehoseDestinationTypeDef],  # (2)
    CloudWatchDestination: NotRequired[CloudWatchDestinationOutputTypeDef],  # (3)
    SNSDestination: NotRequired[SNSDestinationTypeDef],  # (4)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
2. See [:material-code-braces: KinesisFirehoseDestinationTypeDef](./type_defs.md#kinesisfirehosedestinationtypedef) 
3. See [:material-code-braces: CloudWatchDestinationOutputTypeDef](./type_defs.md#cloudwatchdestinationoutputtypedef) 
4. See [:material-code-braces: SNSDestinationTypeDef](./type_defs.md#snsdestinationtypedef) 
## BouncedRecipientInfoTypeDef

```python
# BouncedRecipientInfoTypeDef definition

class BouncedRecipientInfoTypeDef(TypedDict):
    Recipient: str,
    RecipientArn: NotRequired[str],
    BounceType: NotRequired[BounceTypeType],  # (1)
    RecipientDsnFields: NotRequired[RecipientDsnFieldsTypeDef],  # (2)
```

1. See [:material-code-brackets: BounceTypeType](./literals.md#bouncetypetype) 
2. See [:material-code-braces: RecipientDsnFieldsTypeDef](./type_defs.md#recipientdsnfieldstypedef) 
## ReceiptRuleOutputTypeDef

```python
# ReceiptRuleOutputTypeDef definition

class ReceiptRuleOutputTypeDef(TypedDict):
    Name: str,
    Enabled: NotRequired[bool],
    TlsPolicy: NotRequired[TlsPolicyType],  # (1)
    Recipients: NotRequired[List[str]],
    Actions: NotRequired[List[ReceiptActionTypeDef]],  # (2)
    ScanEnabled: NotRequired[bool],
```

1. See [:material-code-brackets: TlsPolicyType](./literals.md#tlspolicytype) 
2. See [:material-code-braces: ReceiptActionTypeDef](./type_defs.md#receiptactiontypedef) 
## ReceiptRuleTypeDef

```python
# ReceiptRuleTypeDef definition

class ReceiptRuleTypeDef(TypedDict):
    Name: str,
    Enabled: NotRequired[bool],
    TlsPolicy: NotRequired[TlsPolicyType],  # (1)
    Recipients: NotRequired[Sequence[str]],
    Actions: NotRequired[Sequence[ReceiptActionTypeDef]],  # (2)
    ScanEnabled: NotRequired[bool],
```

1. See [:material-code-brackets: TlsPolicyType](./literals.md#tlspolicytype) 
2. See [:material-code-braces: ReceiptActionTypeDef](./type_defs.md#receiptactiontypedef) 
## CreateReceiptFilterRequestRequestTypeDef

```python
# CreateReceiptFilterRequestRequestTypeDef definition

class CreateReceiptFilterRequestRequestTypeDef(TypedDict):
    Filter: ReceiptFilterTypeDef,  # (1)
```

1. See [:material-code-braces: ReceiptFilterTypeDef](./type_defs.md#receiptfiltertypedef) 
## ListReceiptFiltersResponseTypeDef

```python
# ListReceiptFiltersResponseTypeDef definition

class ListReceiptFiltersResponseTypeDef(TypedDict):
    Filters: List[ReceiptFilterTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReceiptFilterTypeDef](./type_defs.md#receiptfiltertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendEmailRequestRequestTypeDef

```python
# SendEmailRequestRequestTypeDef definition

class SendEmailRequestRequestTypeDef(TypedDict):
    Source: str,
    Destination: DestinationTypeDef,  # (1)
    Message: MessageTypeDef,  # (2)
    ReplyToAddresses: NotRequired[Sequence[str]],
    ReturnPath: NotRequired[str],
    SourceArn: NotRequired[str],
    ReturnPathArn: NotRequired[str],
    Tags: NotRequired[Sequence[MessageTagTypeDef]],  # (3)
    ConfigurationSetName: NotRequired[str],
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
3. See [:material-code-braces: MessageTagTypeDef](./type_defs.md#messagetagtypedef) 
## DescribeConfigurationSetResponseTypeDef

```python
# DescribeConfigurationSetResponseTypeDef definition

class DescribeConfigurationSetResponseTypeDef(TypedDict):
    ConfigurationSet: ConfigurationSetTypeDef,  # (1)
    EventDestinations: List[EventDestinationOutputTypeDef],  # (2)
    TrackingOptions: TrackingOptionsTypeDef,  # (3)
    DeliveryOptions: DeliveryOptionsTypeDef,  # (4)
    ReputationOptions: ReputationOptionsTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: ConfigurationSetTypeDef](./type_defs.md#configurationsettypedef) 
2. See [:material-code-braces: EventDestinationOutputTypeDef](./type_defs.md#eventdestinationoutputtypedef) 
3. See [:material-code-braces: TrackingOptionsTypeDef](./type_defs.md#trackingoptionstypedef) 
4. See [:material-code-braces: DeliveryOptionsTypeDef](./type_defs.md#deliveryoptionstypedef) 
5. See [:material-code-braces: ReputationOptionsTypeDef](./type_defs.md#reputationoptionstypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EventDestinationTypeDef

```python
# EventDestinationTypeDef definition

class EventDestinationTypeDef(TypedDict):
    Name: str,
    MatchingEventTypes: Sequence[EventTypeType],  # (1)
    Enabled: NotRequired[bool],
    KinesisFirehoseDestination: NotRequired[KinesisFirehoseDestinationTypeDef],  # (2)
    CloudWatchDestination: NotRequired[CloudWatchDestinationUnionTypeDef],  # (3)
    SNSDestination: NotRequired[SNSDestinationTypeDef],  # (4)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
2. See [:material-code-braces: KinesisFirehoseDestinationTypeDef](./type_defs.md#kinesisfirehosedestinationtypedef) 
3. See [:material-code-braces: CloudWatchDestinationTypeDef](./type_defs.md#cloudwatchdestinationtypedef) [:material-code-braces: CloudWatchDestinationOutputTypeDef](./type_defs.md#cloudwatchdestinationoutputtypedef) 
4. See [:material-code-braces: SNSDestinationTypeDef](./type_defs.md#snsdestinationtypedef) 
## SendBounceRequestRequestTypeDef

```python
# SendBounceRequestRequestTypeDef definition

class SendBounceRequestRequestTypeDef(TypedDict):
    OriginalMessageId: str,
    BounceSender: str,
    BouncedRecipientInfoList: Sequence[BouncedRecipientInfoTypeDef],  # (1)
    Explanation: NotRequired[str],
    MessageDsn: NotRequired[MessageDsnTypeDef],  # (2)
    BounceSenderArn: NotRequired[str],
```

1. See [:material-code-braces: BouncedRecipientInfoTypeDef](./type_defs.md#bouncedrecipientinfotypedef) 
2. See [:material-code-braces: MessageDsnTypeDef](./type_defs.md#messagedsntypedef) 
## DescribeActiveReceiptRuleSetResponseTypeDef

```python
# DescribeActiveReceiptRuleSetResponseTypeDef definition

class DescribeActiveReceiptRuleSetResponseTypeDef(TypedDict):
    Metadata: ReceiptRuleSetMetadataTypeDef,  # (1)
    Rules: List[ReceiptRuleOutputTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ReceiptRuleSetMetadataTypeDef](./type_defs.md#receiptrulesetmetadatatypedef) 
2. See [:material-code-braces: ReceiptRuleOutputTypeDef](./type_defs.md#receiptruleoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeReceiptRuleResponseTypeDef

```python
# DescribeReceiptRuleResponseTypeDef definition

class DescribeReceiptRuleResponseTypeDef(TypedDict):
    Rule: ReceiptRuleOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReceiptRuleOutputTypeDef](./type_defs.md#receiptruleoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeReceiptRuleSetResponseTypeDef

```python
# DescribeReceiptRuleSetResponseTypeDef definition

class DescribeReceiptRuleSetResponseTypeDef(TypedDict):
    Metadata: ReceiptRuleSetMetadataTypeDef,  # (1)
    Rules: List[ReceiptRuleOutputTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ReceiptRuleSetMetadataTypeDef](./type_defs.md#receiptrulesetmetadatatypedef) 
2. See [:material-code-braces: ReceiptRuleOutputTypeDef](./type_defs.md#receiptruleoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateReceiptRuleRequestRequestTypeDef

```python
# CreateReceiptRuleRequestRequestTypeDef definition

class CreateReceiptRuleRequestRequestTypeDef(TypedDict):
    RuleSetName: str,
    Rule: ReceiptRuleTypeDef,  # (1)
    After: NotRequired[str],
```

1. See [:material-code-braces: ReceiptRuleTypeDef](./type_defs.md#receiptruletypedef) 
## UpdateReceiptRuleRequestRequestTypeDef

```python
# UpdateReceiptRuleRequestRequestTypeDef definition

class UpdateReceiptRuleRequestRequestTypeDef(TypedDict):
    RuleSetName: str,
    Rule: ReceiptRuleTypeDef,  # (1)
```

1. See [:material-code-braces: ReceiptRuleTypeDef](./type_defs.md#receiptruletypedef) 
## CreateConfigurationSetEventDestinationRequestRequestTypeDef

```python
# CreateConfigurationSetEventDestinationRequestRequestTypeDef definition

class CreateConfigurationSetEventDestinationRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    EventDestination: EventDestinationTypeDef,  # (1)
```

1. See [:material-code-braces: EventDestinationTypeDef](./type_defs.md#eventdestinationtypedef) 
## UpdateConfigurationSetEventDestinationRequestRequestTypeDef

```python
# UpdateConfigurationSetEventDestinationRequestRequestTypeDef definition

class UpdateConfigurationSetEventDestinationRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    EventDestination: EventDestinationTypeDef,  # (1)
```

1. See [:material-code-braces: EventDestinationTypeDef](./type_defs.md#eventdestinationtypedef) 
