# Type definitions

> [Index](../README.md) > [CognitoIdentityProvider](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CognitoIdentityProvider](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#cognitoidentityprovider)
    type annotations stubs module [types-aiobotocore-cognito-idp](https://pypi.org/project/types-aiobotocore-cognito-idp/).

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


## SignInPolicyTypeUnionTypeDef

```python
# SignInPolicyTypeUnionTypeDef definition

SignInPolicyTypeUnionTypeDef = Union[
    SignInPolicyTypeTypeDef,  # (1)
    SignInPolicyTypeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SignInPolicyTypeTypeDef](./type_defs.md#signinpolicytypetypedef) 
2. See [:material-code-braces: SignInPolicyTypeOutputTypeDef](./type_defs.md#signinpolicytypeoutputtypedef) 

## AssetTypeUnionTypeDef

```python
# AssetTypeUnionTypeDef definition

AssetTypeUnionTypeDef = Union[
    AssetTypeTypeDef,  # (1)
    AssetTypeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AssetTypeTypeDef](./type_defs.md#assettypetypedef) 
2. See [:material-code-braces: AssetTypeOutputTypeDef](./type_defs.md#assettypeoutputtypedef) 



## RecoveryOptionTypeTypeDef

```python
# RecoveryOptionTypeTypeDef definition

class RecoveryOptionTypeTypeDef(TypedDict):
    Priority: int,
    Name: RecoveryOptionNameTypeType,  # (1)
```

1. See [:material-code-brackets: RecoveryOptionNameTypeType](./literals.md#recoveryoptionnametypetype) 
## AccountTakeoverActionTypeTypeDef

```python
# AccountTakeoverActionTypeTypeDef definition

class AccountTakeoverActionTypeTypeDef(TypedDict):
    Notify: bool,
    EventAction: AccountTakeoverEventActionTypeType,  # (1)
```

1. See [:material-code-brackets: AccountTakeoverEventActionTypeType](./literals.md#accounttakeovereventactiontypetype) 
## AdminAddUserToGroupRequestRequestTypeDef

```python
# AdminAddUserToGroupRequestRequestTypeDef definition

class AdminAddUserToGroupRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Username: str,
    GroupName: str,
```

## AdminConfirmSignUpRequestRequestTypeDef

```python
# AdminConfirmSignUpRequestRequestTypeDef definition

class AdminConfirmSignUpRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Username: str,
    ClientMetadata: NotRequired[Mapping[str, str]],
```

## MessageTemplateTypeTypeDef

```python
# MessageTemplateTypeTypeDef definition

class MessageTemplateTypeTypeDef(TypedDict):
    SMSMessage: NotRequired[str],
    EmailMessage: NotRequired[str],
    EmailSubject: NotRequired[str],
```

## AttributeTypeTypeDef

```python
# AttributeTypeTypeDef definition

class AttributeTypeTypeDef(TypedDict):
    Name: str,
    Value: NotRequired[str],
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

## AdminDeleteUserAttributesRequestRequestTypeDef

```python
# AdminDeleteUserAttributesRequestRequestTypeDef definition

class AdminDeleteUserAttributesRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Username: str,
    UserAttributeNames: Sequence[str],
```

## AdminDeleteUserRequestRequestTypeDef

```python
# AdminDeleteUserRequestRequestTypeDef definition

class AdminDeleteUserRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Username: str,
```

## ProviderUserIdentifierTypeTypeDef

```python
# ProviderUserIdentifierTypeTypeDef definition

class ProviderUserIdentifierTypeTypeDef(TypedDict):
    ProviderName: NotRequired[str],
    ProviderAttributeName: NotRequired[str],
    ProviderAttributeValue: NotRequired[str],
```

## AdminDisableUserRequestRequestTypeDef

```python
# AdminDisableUserRequestRequestTypeDef definition

class AdminDisableUserRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Username: str,
```

## AdminEnableUserRequestRequestTypeDef

```python
# AdminEnableUserRequestRequestTypeDef definition

class AdminEnableUserRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Username: str,
```

## AdminForgetDeviceRequestRequestTypeDef

```python
# AdminForgetDeviceRequestRequestTypeDef definition

class AdminForgetDeviceRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Username: str,
    DeviceKey: str,
```

## AdminGetDeviceRequestRequestTypeDef

```python
# AdminGetDeviceRequestRequestTypeDef definition

class AdminGetDeviceRequestRequestTypeDef(TypedDict):
    DeviceKey: str,
    UserPoolId: str,
    Username: str,
```

## AdminGetUserRequestRequestTypeDef

```python
# AdminGetUserRequestRequestTypeDef definition

class AdminGetUserRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Username: str,
```

## MFAOptionTypeTypeDef

```python
# MFAOptionTypeTypeDef definition

class MFAOptionTypeTypeDef(TypedDict):
    DeliveryMedium: NotRequired[DeliveryMediumTypeType],  # (1)
    AttributeName: NotRequired[str],
```

1. See [:material-code-brackets: DeliveryMediumTypeType](./literals.md#deliverymediumtypetype) 
## AnalyticsMetadataTypeTypeDef

```python
# AnalyticsMetadataTypeTypeDef definition

class AnalyticsMetadataTypeTypeDef(TypedDict):
    AnalyticsEndpointId: NotRequired[str],
```

## AdminListDevicesRequestRequestTypeDef

```python
# AdminListDevicesRequestRequestTypeDef definition

class AdminListDevicesRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Username: str,
    Limit: NotRequired[int],
    PaginationToken: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## AdminListGroupsForUserRequestRequestTypeDef

```python
# AdminListGroupsForUserRequestRequestTypeDef definition

class AdminListGroupsForUserRequestRequestTypeDef(TypedDict):
    Username: str,
    UserPoolId: str,
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## GroupTypeTypeDef

```python
# GroupTypeTypeDef definition

class GroupTypeTypeDef(TypedDict):
    GroupName: NotRequired[str],
    UserPoolId: NotRequired[str],
    Description: NotRequired[str],
    RoleArn: NotRequired[str],
    Precedence: NotRequired[int],
    LastModifiedDate: NotRequired[datetime],
    CreationDate: NotRequired[datetime],
```

## AdminListUserAuthEventsRequestRequestTypeDef

```python
# AdminListUserAuthEventsRequestRequestTypeDef definition

class AdminListUserAuthEventsRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Username: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## AdminRemoveUserFromGroupRequestRequestTypeDef

```python
# AdminRemoveUserFromGroupRequestRequestTypeDef definition

class AdminRemoveUserFromGroupRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Username: str,
    GroupName: str,
```

## AdminResetUserPasswordRequestRequestTypeDef

```python
# AdminResetUserPasswordRequestRequestTypeDef definition

class AdminResetUserPasswordRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Username: str,
    ClientMetadata: NotRequired[Mapping[str, str]],
```

## EmailMfaSettingsTypeTypeDef

```python
# EmailMfaSettingsTypeTypeDef definition

class EmailMfaSettingsTypeTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    PreferredMfa: NotRequired[bool],
```

## SMSMfaSettingsTypeTypeDef

```python
# SMSMfaSettingsTypeTypeDef definition

class SMSMfaSettingsTypeTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    PreferredMfa: NotRequired[bool],
```

## SoftwareTokenMfaSettingsTypeTypeDef

```python
# SoftwareTokenMfaSettingsTypeTypeDef definition

class SoftwareTokenMfaSettingsTypeTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    PreferredMfa: NotRequired[bool],
```

## AdminSetUserPasswordRequestRequestTypeDef

```python
# AdminSetUserPasswordRequestRequestTypeDef definition

class AdminSetUserPasswordRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Username: str,
    Password: str,
    Permanent: NotRequired[bool],
```

## AdminUpdateAuthEventFeedbackRequestRequestTypeDef

```python
# AdminUpdateAuthEventFeedbackRequestRequestTypeDef definition

class AdminUpdateAuthEventFeedbackRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Username: str,
    EventId: str,
    FeedbackValue: FeedbackValueTypeType,  # (1)
```

1. See [:material-code-brackets: FeedbackValueTypeType](./literals.md#feedbackvaluetypetype) 
## AdminUpdateDeviceStatusRequestRequestTypeDef

```python
# AdminUpdateDeviceStatusRequestRequestTypeDef definition

class AdminUpdateDeviceStatusRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Username: str,
    DeviceKey: str,
    DeviceRememberedStatus: NotRequired[DeviceRememberedStatusTypeType],  # (1)
```

1. See [:material-code-brackets: DeviceRememberedStatusTypeType](./literals.md#devicerememberedstatustypetype) 
## AdminUserGlobalSignOutRequestRequestTypeDef

```python
# AdminUserGlobalSignOutRequestRequestTypeDef definition

class AdminUserGlobalSignOutRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Username: str,
```

## AdvancedSecurityAdditionalFlowsTypeTypeDef

```python
# AdvancedSecurityAdditionalFlowsTypeTypeDef definition

class AdvancedSecurityAdditionalFlowsTypeTypeDef(TypedDict):
    CustomAuthMode: NotRequired[AdvancedSecurityEnabledModeTypeType],  # (1)
```

1. See [:material-code-brackets: AdvancedSecurityEnabledModeTypeType](./literals.md#advancedsecurityenabledmodetypetype) 
## AnalyticsConfigurationTypeTypeDef

```python
# AnalyticsConfigurationTypeTypeDef definition

class AnalyticsConfigurationTypeTypeDef(TypedDict):
    ApplicationId: NotRequired[str],
    ApplicationArn: NotRequired[str],
    RoleArn: NotRequired[str],
    ExternalId: NotRequired[str],
    UserDataShared: NotRequired[bool],
```

## AssetTypeOutputTypeDef

```python
# AssetTypeOutputTypeDef definition

class AssetTypeOutputTypeDef(TypedDict):
    Category: AssetCategoryTypeType,  # (1)
    ColorMode: ColorSchemeModeTypeType,  # (2)
    Extension: AssetExtensionTypeType,  # (3)
    Bytes: NotRequired[bytes],
    ResourceId: NotRequired[str],
```

1. See [:material-code-brackets: AssetCategoryTypeType](./literals.md#assetcategorytypetype) 
2. See [:material-code-brackets: ColorSchemeModeTypeType](./literals.md#colorschememodetypetype) 
3. See [:material-code-brackets: AssetExtensionTypeType](./literals.md#assetextensiontypetype) 
## AssociateSoftwareTokenRequestRequestTypeDef

```python
# AssociateSoftwareTokenRequestRequestTypeDef definition

class AssociateSoftwareTokenRequestRequestTypeDef(TypedDict):
    AccessToken: NotRequired[str],
    Session: NotRequired[str],
```

## ChallengeResponseTypeTypeDef

```python
# ChallengeResponseTypeTypeDef definition

class ChallengeResponseTypeTypeDef(TypedDict):
    ChallengeName: NotRequired[ChallengeNameType],  # (1)
    ChallengeResponse: NotRequired[ChallengeResponseType],  # (2)
```

1. See [:material-code-brackets: ChallengeNameType](./literals.md#challengenametype) 
2. See [:material-code-brackets: ChallengeResponseType](./literals.md#challengeresponsetype) 
## EventContextDataTypeTypeDef

```python
# EventContextDataTypeTypeDef definition

class EventContextDataTypeTypeDef(TypedDict):
    IpAddress: NotRequired[str],
    DeviceName: NotRequired[str],
    Timezone: NotRequired[str],
    City: NotRequired[str],
    Country: NotRequired[str],
```

## EventFeedbackTypeTypeDef

```python
# EventFeedbackTypeTypeDef definition

class EventFeedbackTypeTypeDef(TypedDict):
    FeedbackValue: FeedbackValueTypeType,  # (1)
    Provider: str,
    FeedbackDate: NotRequired[datetime],
```

1. See [:material-code-brackets: FeedbackValueTypeType](./literals.md#feedbackvaluetypetype) 
## EventRiskTypeTypeDef

```python
# EventRiskTypeTypeDef definition

class EventRiskTypeTypeDef(TypedDict):
    RiskDecision: NotRequired[RiskDecisionTypeType],  # (1)
    RiskLevel: NotRequired[RiskLevelTypeType],  # (2)
    CompromisedCredentialsDetected: NotRequired[bool],
```

1. See [:material-code-brackets: RiskDecisionTypeType](./literals.md#riskdecisiontypetype) 
2. See [:material-code-brackets: RiskLevelTypeType](./literals.md#riskleveltypetype) 
## NewDeviceMetadataTypeTypeDef

```python
# NewDeviceMetadataTypeTypeDef definition

class NewDeviceMetadataTypeTypeDef(TypedDict):
    DeviceKey: NotRequired[str],
    DeviceGroupKey: NotRequired[str],
```

## ChangePasswordRequestRequestTypeDef

```python
# ChangePasswordRequestRequestTypeDef definition

class ChangePasswordRequestRequestTypeDef(TypedDict):
    ProposedPassword: str,
    AccessToken: str,
    PreviousPassword: NotRequired[str],
```

## CloudWatchLogsConfigurationTypeTypeDef

```python
# CloudWatchLogsConfigurationTypeTypeDef definition

class CloudWatchLogsConfigurationTypeTypeDef(TypedDict):
    LogGroupArn: NotRequired[str],
```

## CodeDeliveryDetailsTypeTypeDef

```python
# CodeDeliveryDetailsTypeTypeDef definition

class CodeDeliveryDetailsTypeTypeDef(TypedDict):
    Destination: NotRequired[str],
    DeliveryMedium: NotRequired[DeliveryMediumTypeType],  # (1)
    AttributeName: NotRequired[str],
```

1. See [:material-code-brackets: DeliveryMediumTypeType](./literals.md#deliverymediumtypetype) 
## CompleteWebAuthnRegistrationRequestRequestTypeDef

```python
# CompleteWebAuthnRegistrationRequestRequestTypeDef definition

class CompleteWebAuthnRegistrationRequestRequestTypeDef(TypedDict):
    AccessToken: str,
    Credential: Mapping[str, Any],
```

## CompromisedCredentialsActionsTypeTypeDef

```python
# CompromisedCredentialsActionsTypeTypeDef definition

class CompromisedCredentialsActionsTypeTypeDef(TypedDict):
    EventAction: CompromisedCredentialsEventActionTypeType,  # (1)
```

1. See [:material-code-brackets: CompromisedCredentialsEventActionTypeType](./literals.md#compromisedcredentialseventactiontypetype) 
## DeviceSecretVerifierConfigTypeTypeDef

```python
# DeviceSecretVerifierConfigTypeTypeDef definition

class DeviceSecretVerifierConfigTypeTypeDef(TypedDict):
    PasswordVerifier: NotRequired[str],
    Salt: NotRequired[str],
```

## UserContextDataTypeTypeDef

```python
# UserContextDataTypeTypeDef definition

class UserContextDataTypeTypeDef(TypedDict):
    IpAddress: NotRequired[str],
    EncodedData: NotRequired[str],
```

## HttpHeaderTypeDef

```python
# HttpHeaderTypeDef definition

class HttpHeaderTypeDef(TypedDict):
    headerName: NotRequired[str],
    headerValue: NotRequired[str],
```

## CreateGroupRequestRequestTypeDef

```python
# CreateGroupRequestRequestTypeDef definition

class CreateGroupRequestRequestTypeDef(TypedDict):
    GroupName: str,
    UserPoolId: str,
    Description: NotRequired[str],
    RoleArn: NotRequired[str],
    Precedence: NotRequired[int],
```

## CreateIdentityProviderRequestRequestTypeDef

```python
# CreateIdentityProviderRequestRequestTypeDef definition

class CreateIdentityProviderRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    ProviderName: str,
    ProviderType: IdentityProviderTypeTypeType,  # (1)
    ProviderDetails: Mapping[str, str],
    AttributeMapping: NotRequired[Mapping[str, str]],
    IdpIdentifiers: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: IdentityProviderTypeTypeType](./literals.md#identityprovidertypetypetype) 
## IdentityProviderTypeTypeDef

```python
# IdentityProviderTypeTypeDef definition

class IdentityProviderTypeTypeDef(TypedDict):
    UserPoolId: NotRequired[str],
    ProviderName: NotRequired[str],
    ProviderType: NotRequired[IdentityProviderTypeTypeType],  # (1)
    ProviderDetails: NotRequired[Dict[str, str]],
    AttributeMapping: NotRequired[Dict[str, str]],
    IdpIdentifiers: NotRequired[List[str]],
    LastModifiedDate: NotRequired[datetime],
    CreationDate: NotRequired[datetime],
```

1. See [:material-code-brackets: IdentityProviderTypeTypeType](./literals.md#identityprovidertypetypetype) 
## ResourceServerScopeTypeTypeDef

```python
# ResourceServerScopeTypeTypeDef definition

class ResourceServerScopeTypeTypeDef(TypedDict):
    ScopeName: str,
    ScopeDescription: str,
```

## CreateUserImportJobRequestRequestTypeDef

```python
# CreateUserImportJobRequestRequestTypeDef definition

class CreateUserImportJobRequestRequestTypeDef(TypedDict):
    JobName: str,
    UserPoolId: str,
    CloudWatchLogsRoleArn: str,
```

## UserImportJobTypeTypeDef

```python
# UserImportJobTypeTypeDef definition

class UserImportJobTypeTypeDef(TypedDict):
    JobName: NotRequired[str],
    JobId: NotRequired[str],
    UserPoolId: NotRequired[str],
    PreSignedUrl: NotRequired[str],
    CreationDate: NotRequired[datetime],
    StartDate: NotRequired[datetime],
    CompletionDate: NotRequired[datetime],
    Status: NotRequired[UserImportJobStatusTypeType],  # (1)
    CloudWatchLogsRoleArn: NotRequired[str],
    ImportedUsers: NotRequired[int],
    SkippedUsers: NotRequired[int],
    FailedUsers: NotRequired[int],
    CompletionMessage: NotRequired[str],
```

1. See [:material-code-brackets: UserImportJobStatusTypeType](./literals.md#userimportjobstatustypetype) 
## TokenValidityUnitsTypeTypeDef

```python
# TokenValidityUnitsTypeTypeDef definition

class TokenValidityUnitsTypeTypeDef(TypedDict):
    AccessToken: NotRequired[TimeUnitsTypeType],  # (1)
    IdToken: NotRequired[TimeUnitsTypeType],  # (1)
    RefreshToken: NotRequired[TimeUnitsTypeType],  # (1)
```

1. See [:material-code-brackets: TimeUnitsTypeType](./literals.md#timeunitstypetype) 
2. See [:material-code-brackets: TimeUnitsTypeType](./literals.md#timeunitstypetype) 
3. See [:material-code-brackets: TimeUnitsTypeType](./literals.md#timeunitstypetype) 
## CustomDomainConfigTypeTypeDef

```python
# CustomDomainConfigTypeTypeDef definition

class CustomDomainConfigTypeTypeDef(TypedDict):
    CertificateArn: str,
```

## DeviceConfigurationTypeTypeDef

```python
# DeviceConfigurationTypeTypeDef definition

class DeviceConfigurationTypeTypeDef(TypedDict):
    ChallengeRequiredOnNewDevice: NotRequired[bool],
    DeviceOnlyRememberedOnUserPrompt: NotRequired[bool],
```

## EmailConfigurationTypeTypeDef

```python
# EmailConfigurationTypeTypeDef definition

class EmailConfigurationTypeTypeDef(TypedDict):
    SourceArn: NotRequired[str],
    ReplyToEmailAddress: NotRequired[str],
    EmailSendingAccount: NotRequired[EmailSendingAccountTypeType],  # (1)
    From: NotRequired[str],
    ConfigurationSet: NotRequired[str],
```

1. See [:material-code-brackets: EmailSendingAccountTypeType](./literals.md#emailsendingaccounttypetype) 
## SmsConfigurationTypeTypeDef

```python
# SmsConfigurationTypeTypeDef definition

class SmsConfigurationTypeTypeDef(TypedDict):
    SnsCallerArn: str,
    ExternalId: NotRequired[str],
    SnsRegion: NotRequired[str],
```

## UserAttributeUpdateSettingsTypeTypeDef

```python
# UserAttributeUpdateSettingsTypeTypeDef definition

class UserAttributeUpdateSettingsTypeTypeDef(TypedDict):
    AttributesRequireVerificationBeforeUpdate: NotRequired[Sequence[VerifiedAttributeTypeType]],  # (1)
```

1. See [:material-code-brackets: VerifiedAttributeTypeType](./literals.md#verifiedattributetypetype) 
## UsernameConfigurationTypeTypeDef

```python
# UsernameConfigurationTypeTypeDef definition

class UsernameConfigurationTypeTypeDef(TypedDict):
    CaseSensitive: bool,
```

## VerificationMessageTemplateTypeTypeDef

```python
# VerificationMessageTemplateTypeTypeDef definition

class VerificationMessageTemplateTypeTypeDef(TypedDict):
    SmsMessage: NotRequired[str],
    EmailMessage: NotRequired[str],
    EmailSubject: NotRequired[str],
    EmailMessageByLink: NotRequired[str],
    EmailSubjectByLink: NotRequired[str],
    DefaultEmailOption: NotRequired[DefaultEmailOptionTypeType],  # (1)
```

1. See [:material-code-brackets: DefaultEmailOptionTypeType](./literals.md#defaultemailoptiontypetype) 
## CustomEmailLambdaVersionConfigTypeTypeDef

```python
# CustomEmailLambdaVersionConfigTypeTypeDef definition

class CustomEmailLambdaVersionConfigTypeTypeDef(TypedDict):
    LambdaVersion: CustomEmailSenderLambdaVersionTypeType,  # (1)
    LambdaArn: str,
```

1. See [:material-code-brackets: CustomEmailSenderLambdaVersionTypeType](./literals.md#customemailsenderlambdaversiontypetype) 
## CustomSMSLambdaVersionConfigTypeTypeDef

```python
# CustomSMSLambdaVersionConfigTypeTypeDef definition

class CustomSMSLambdaVersionConfigTypeTypeDef(TypedDict):
    LambdaVersion: CustomSMSSenderLambdaVersionTypeType,  # (1)
    LambdaArn: str,
```

1. See [:material-code-brackets: CustomSMSSenderLambdaVersionTypeType](./literals.md#customsmssenderlambdaversiontypetype) 
## DeleteGroupRequestRequestTypeDef

```python
# DeleteGroupRequestRequestTypeDef definition

class DeleteGroupRequestRequestTypeDef(TypedDict):
    GroupName: str,
    UserPoolId: str,
```

## DeleteIdentityProviderRequestRequestTypeDef

```python
# DeleteIdentityProviderRequestRequestTypeDef definition

class DeleteIdentityProviderRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    ProviderName: str,
```

## DeleteManagedLoginBrandingRequestRequestTypeDef

```python
# DeleteManagedLoginBrandingRequestRequestTypeDef definition

class DeleteManagedLoginBrandingRequestRequestTypeDef(TypedDict):
    ManagedLoginBrandingId: str,
    UserPoolId: str,
```

## DeleteResourceServerRequestRequestTypeDef

```python
# DeleteResourceServerRequestRequestTypeDef definition

class DeleteResourceServerRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Identifier: str,
```

## DeleteUserAttributesRequestRequestTypeDef

```python
# DeleteUserAttributesRequestRequestTypeDef definition

class DeleteUserAttributesRequestRequestTypeDef(TypedDict):
    UserAttributeNames: Sequence[str],
    AccessToken: str,
```

## DeleteUserPoolClientRequestRequestTypeDef

```python
# DeleteUserPoolClientRequestRequestTypeDef definition

class DeleteUserPoolClientRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    ClientId: str,
```

## DeleteUserPoolDomainRequestRequestTypeDef

```python
# DeleteUserPoolDomainRequestRequestTypeDef definition

class DeleteUserPoolDomainRequestRequestTypeDef(TypedDict):
    Domain: str,
    UserPoolId: str,
```

## DeleteUserPoolRequestRequestTypeDef

```python
# DeleteUserPoolRequestRequestTypeDef definition

class DeleteUserPoolRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
```

## DeleteUserRequestRequestTypeDef

```python
# DeleteUserRequestRequestTypeDef definition

class DeleteUserRequestRequestTypeDef(TypedDict):
    AccessToken: str,
```

## DeleteWebAuthnCredentialRequestRequestTypeDef

```python
# DeleteWebAuthnCredentialRequestRequestTypeDef definition

class DeleteWebAuthnCredentialRequestRequestTypeDef(TypedDict):
    AccessToken: str,
    CredentialId: str,
```

## DescribeIdentityProviderRequestRequestTypeDef

```python
# DescribeIdentityProviderRequestRequestTypeDef definition

class DescribeIdentityProviderRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    ProviderName: str,
```

## DescribeManagedLoginBrandingByClientRequestRequestTypeDef

```python
# DescribeManagedLoginBrandingByClientRequestRequestTypeDef definition

class DescribeManagedLoginBrandingByClientRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    ClientId: str,
    ReturnMergedResources: NotRequired[bool],
```

## DescribeManagedLoginBrandingRequestRequestTypeDef

```python
# DescribeManagedLoginBrandingRequestRequestTypeDef definition

class DescribeManagedLoginBrandingRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    ManagedLoginBrandingId: str,
    ReturnMergedResources: NotRequired[bool],
```

## DescribeResourceServerRequestRequestTypeDef

```python
# DescribeResourceServerRequestRequestTypeDef definition

class DescribeResourceServerRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Identifier: str,
```

## DescribeRiskConfigurationRequestRequestTypeDef

```python
# DescribeRiskConfigurationRequestRequestTypeDef definition

class DescribeRiskConfigurationRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    ClientId: NotRequired[str],
```

## DescribeUserImportJobRequestRequestTypeDef

```python
# DescribeUserImportJobRequestRequestTypeDef definition

class DescribeUserImportJobRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    JobId: str,
```

## DescribeUserPoolClientRequestRequestTypeDef

```python
# DescribeUserPoolClientRequestRequestTypeDef definition

class DescribeUserPoolClientRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    ClientId: str,
```

## DescribeUserPoolDomainRequestRequestTypeDef

```python
# DescribeUserPoolDomainRequestRequestTypeDef definition

class DescribeUserPoolDomainRequestRequestTypeDef(TypedDict):
    Domain: str,
```

## DescribeUserPoolRequestRequestTypeDef

```python
# DescribeUserPoolRequestRequestTypeDef definition

class DescribeUserPoolRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
```

## EmailMfaConfigTypeTypeDef

```python
# EmailMfaConfigTypeTypeDef definition

class EmailMfaConfigTypeTypeDef(TypedDict):
    Message: NotRequired[str],
    Subject: NotRequired[str],
```

## FirehoseConfigurationTypeTypeDef

```python
# FirehoseConfigurationTypeTypeDef definition

class FirehoseConfigurationTypeTypeDef(TypedDict):
    StreamArn: NotRequired[str],
```

## ForgetDeviceRequestRequestTypeDef

```python
# ForgetDeviceRequestRequestTypeDef definition

class ForgetDeviceRequestRequestTypeDef(TypedDict):
    DeviceKey: str,
    AccessToken: NotRequired[str],
```

## GetCSVHeaderRequestRequestTypeDef

```python
# GetCSVHeaderRequestRequestTypeDef definition

class GetCSVHeaderRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
```

## GetDeviceRequestRequestTypeDef

```python
# GetDeviceRequestRequestTypeDef definition

class GetDeviceRequestRequestTypeDef(TypedDict):
    DeviceKey: str,
    AccessToken: NotRequired[str],
```

## GetGroupRequestRequestTypeDef

```python
# GetGroupRequestRequestTypeDef definition

class GetGroupRequestRequestTypeDef(TypedDict):
    GroupName: str,
    UserPoolId: str,
```

## GetIdentityProviderByIdentifierRequestRequestTypeDef

```python
# GetIdentityProviderByIdentifierRequestRequestTypeDef definition

class GetIdentityProviderByIdentifierRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    IdpIdentifier: str,
```

## GetLogDeliveryConfigurationRequestRequestTypeDef

```python
# GetLogDeliveryConfigurationRequestRequestTypeDef definition

class GetLogDeliveryConfigurationRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
```

## GetSigningCertificateRequestRequestTypeDef

```python
# GetSigningCertificateRequestRequestTypeDef definition

class GetSigningCertificateRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
```

## GetUICustomizationRequestRequestTypeDef

```python
# GetUICustomizationRequestRequestTypeDef definition

class GetUICustomizationRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    ClientId: NotRequired[str],
```

## UICustomizationTypeTypeDef

```python
# UICustomizationTypeTypeDef definition

class UICustomizationTypeTypeDef(TypedDict):
    UserPoolId: NotRequired[str],
    ClientId: NotRequired[str],
    ImageUrl: NotRequired[str],
    CSS: NotRequired[str],
    CSSVersion: NotRequired[str],
    LastModifiedDate: NotRequired[datetime],
    CreationDate: NotRequired[datetime],
```

## GetUserAttributeVerificationCodeRequestRequestTypeDef

```python
# GetUserAttributeVerificationCodeRequestRequestTypeDef definition

class GetUserAttributeVerificationCodeRequestRequestTypeDef(TypedDict):
    AccessToken: str,
    AttributeName: str,
    ClientMetadata: NotRequired[Mapping[str, str]],
```

## GetUserAuthFactorsRequestRequestTypeDef

```python
# GetUserAuthFactorsRequestRequestTypeDef definition

class GetUserAuthFactorsRequestRequestTypeDef(TypedDict):
    AccessToken: str,
```

## GetUserPoolMfaConfigRequestRequestTypeDef

```python
# GetUserPoolMfaConfigRequestRequestTypeDef definition

class GetUserPoolMfaConfigRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
```

## SoftwareTokenMfaConfigTypeTypeDef

```python
# SoftwareTokenMfaConfigTypeTypeDef definition

class SoftwareTokenMfaConfigTypeTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## WebAuthnConfigurationTypeTypeDef

```python
# WebAuthnConfigurationTypeTypeDef definition

class WebAuthnConfigurationTypeTypeDef(TypedDict):
    RelyingPartyId: NotRequired[str],
    UserVerification: NotRequired[UserVerificationTypeType],  # (1)
```

1. See [:material-code-brackets: UserVerificationTypeType](./literals.md#userverificationtypetype) 
## GetUserRequestRequestTypeDef

```python
# GetUserRequestRequestTypeDef definition

class GetUserRequestRequestTypeDef(TypedDict):
    AccessToken: str,
```

## GlobalSignOutRequestRequestTypeDef

```python
# GlobalSignOutRequestRequestTypeDef definition

class GlobalSignOutRequestRequestTypeDef(TypedDict):
    AccessToken: str,
```

## PreTokenGenerationVersionConfigTypeTypeDef

```python
# PreTokenGenerationVersionConfigTypeTypeDef definition

class PreTokenGenerationVersionConfigTypeTypeDef(TypedDict):
    LambdaVersion: PreTokenGenerationLambdaVersionTypeType,  # (1)
    LambdaArn: str,
```

1. See [:material-code-brackets: PreTokenGenerationLambdaVersionTypeType](./literals.md#pretokengenerationlambdaversiontypetype) 
## ListDevicesRequestRequestTypeDef

```python
# ListDevicesRequestRequestTypeDef definition

class ListDevicesRequestRequestTypeDef(TypedDict):
    AccessToken: str,
    Limit: NotRequired[int],
    PaginationToken: NotRequired[str],
```

## ListGroupsRequestRequestTypeDef

```python
# ListGroupsRequestRequestTypeDef definition

class ListGroupsRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListIdentityProvidersRequestRequestTypeDef

```python
# ListIdentityProvidersRequestRequestTypeDef definition

class ListIdentityProvidersRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ProviderDescriptionTypeDef

```python
# ProviderDescriptionTypeDef definition

class ProviderDescriptionTypeDef(TypedDict):
    ProviderName: NotRequired[str],
    ProviderType: NotRequired[IdentityProviderTypeTypeType],  # (1)
    LastModifiedDate: NotRequired[datetime],
    CreationDate: NotRequired[datetime],
```

1. See [:material-code-brackets: IdentityProviderTypeTypeType](./literals.md#identityprovidertypetypetype) 
## ListResourceServersRequestRequestTypeDef

```python
# ListResourceServersRequestRequestTypeDef definition

class ListResourceServersRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ListUserImportJobsRequestRequestTypeDef

```python
# ListUserImportJobsRequestRequestTypeDef definition

class ListUserImportJobsRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    MaxResults: int,
    PaginationToken: NotRequired[str],
```

## ListUserPoolClientsRequestRequestTypeDef

```python
# ListUserPoolClientsRequestRequestTypeDef definition

class ListUserPoolClientsRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## UserPoolClientDescriptionTypeDef

```python
# UserPoolClientDescriptionTypeDef definition

class UserPoolClientDescriptionTypeDef(TypedDict):
    ClientId: NotRequired[str],
    UserPoolId: NotRequired[str],
    ClientName: NotRequired[str],
```

## ListUserPoolsRequestRequestTypeDef

```python
# ListUserPoolsRequestRequestTypeDef definition

class ListUserPoolsRequestRequestTypeDef(TypedDict):
    MaxResults: int,
    NextToken: NotRequired[str],
```

## ListUsersInGroupRequestRequestTypeDef

```python
# ListUsersInGroupRequestRequestTypeDef definition

class ListUsersInGroupRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    GroupName: str,
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListUsersRequestRequestTypeDef

```python
# ListUsersRequestRequestTypeDef definition

class ListUsersRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    AttributesToGet: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    PaginationToken: NotRequired[str],
    Filter: NotRequired[str],
```

## ListWebAuthnCredentialsRequestRequestTypeDef

```python
# ListWebAuthnCredentialsRequestRequestTypeDef definition

class ListWebAuthnCredentialsRequestRequestTypeDef(TypedDict):
    AccessToken: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## WebAuthnCredentialDescriptionTypeDef

```python
# WebAuthnCredentialDescriptionTypeDef definition

class WebAuthnCredentialDescriptionTypeDef(TypedDict):
    CredentialId: str,
    FriendlyCredentialName: str,
    RelyingPartyId: str,
    AuthenticatorTransports: List[str],
    CreatedAt: datetime,
    AuthenticatorAttachment: NotRequired[str],
```

## S3ConfigurationTypeTypeDef

```python
# S3ConfigurationTypeTypeDef definition

class S3ConfigurationTypeTypeDef(TypedDict):
    BucketArn: NotRequired[str],
```

## NotifyEmailTypeTypeDef

```python
# NotifyEmailTypeTypeDef definition

class NotifyEmailTypeTypeDef(TypedDict):
    Subject: str,
    HtmlBody: NotRequired[str],
    TextBody: NotRequired[str],
```

## NumberAttributeConstraintsTypeTypeDef

```python
# NumberAttributeConstraintsTypeTypeDef definition

class NumberAttributeConstraintsTypeTypeDef(TypedDict):
    MinValue: NotRequired[str],
    MaxValue: NotRequired[str],
```

## PasswordPolicyTypeTypeDef

```python
# PasswordPolicyTypeTypeDef definition

class PasswordPolicyTypeTypeDef(TypedDict):
    MinimumLength: NotRequired[int],
    RequireUppercase: NotRequired[bool],
    RequireLowercase: NotRequired[bool],
    RequireNumbers: NotRequired[bool],
    RequireSymbols: NotRequired[bool],
    PasswordHistorySize: NotRequired[int],
    TemporaryPasswordValidityDays: NotRequired[int],
```

## RevokeTokenRequestRequestTypeDef

```python
# RevokeTokenRequestRequestTypeDef definition

class RevokeTokenRequestRequestTypeDef(TypedDict):
    Token: str,
    ClientId: str,
    ClientSecret: NotRequired[str],
```

## RiskExceptionConfigurationTypeOutputTypeDef

```python
# RiskExceptionConfigurationTypeOutputTypeDef definition

class RiskExceptionConfigurationTypeOutputTypeDef(TypedDict):
    BlockedIPRangeList: NotRequired[List[str]],
    SkippedIPRangeList: NotRequired[List[str]],
```

## RiskExceptionConfigurationTypeTypeDef

```python
# RiskExceptionConfigurationTypeTypeDef definition

class RiskExceptionConfigurationTypeTypeDef(TypedDict):
    BlockedIPRangeList: NotRequired[Sequence[str]],
    SkippedIPRangeList: NotRequired[Sequence[str]],
```

## StringAttributeConstraintsTypeTypeDef

```python
# StringAttributeConstraintsTypeTypeDef definition

class StringAttributeConstraintsTypeTypeDef(TypedDict):
    MinLength: NotRequired[str],
    MaxLength: NotRequired[str],
```

## SignInPolicyTypeOutputTypeDef

```python
# SignInPolicyTypeOutputTypeDef definition

class SignInPolicyTypeOutputTypeDef(TypedDict):
    AllowedFirstAuthFactors: NotRequired[List[AuthFactorTypeType]],  # (1)
```

1. See [:material-code-brackets: AuthFactorTypeType](./literals.md#authfactortypetype) 
## SignInPolicyTypeTypeDef

```python
# SignInPolicyTypeTypeDef definition

class SignInPolicyTypeTypeDef(TypedDict):
    AllowedFirstAuthFactors: NotRequired[Sequence[AuthFactorTypeType]],  # (1)
```

1. See [:material-code-brackets: AuthFactorTypeType](./literals.md#authfactortypetype) 
## StartUserImportJobRequestRequestTypeDef

```python
# StartUserImportJobRequestRequestTypeDef definition

class StartUserImportJobRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    JobId: str,
```

## StartWebAuthnRegistrationRequestRequestTypeDef

```python
# StartWebAuthnRegistrationRequestRequestTypeDef definition

class StartWebAuthnRegistrationRequestRequestTypeDef(TypedDict):
    AccessToken: str,
```

## StopUserImportJobRequestRequestTypeDef

```python
# StopUserImportJobRequestRequestTypeDef definition

class StopUserImportJobRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    JobId: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateAuthEventFeedbackRequestRequestTypeDef

```python
# UpdateAuthEventFeedbackRequestRequestTypeDef definition

class UpdateAuthEventFeedbackRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Username: str,
    EventId: str,
    FeedbackToken: str,
    FeedbackValue: FeedbackValueTypeType,  # (1)
```

1. See [:material-code-brackets: FeedbackValueTypeType](./literals.md#feedbackvaluetypetype) 
## UpdateDeviceStatusRequestRequestTypeDef

```python
# UpdateDeviceStatusRequestRequestTypeDef definition

class UpdateDeviceStatusRequestRequestTypeDef(TypedDict):
    AccessToken: str,
    DeviceKey: str,
    DeviceRememberedStatus: NotRequired[DeviceRememberedStatusTypeType],  # (1)
```

1. See [:material-code-brackets: DeviceRememberedStatusTypeType](./literals.md#devicerememberedstatustypetype) 
## UpdateGroupRequestRequestTypeDef

```python
# UpdateGroupRequestRequestTypeDef definition

class UpdateGroupRequestRequestTypeDef(TypedDict):
    GroupName: str,
    UserPoolId: str,
    Description: NotRequired[str],
    RoleArn: NotRequired[str],
    Precedence: NotRequired[int],
```

## UpdateIdentityProviderRequestRequestTypeDef

```python
# UpdateIdentityProviderRequestRequestTypeDef definition

class UpdateIdentityProviderRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    ProviderName: str,
    ProviderDetails: NotRequired[Mapping[str, str]],
    AttributeMapping: NotRequired[Mapping[str, str]],
    IdpIdentifiers: NotRequired[Sequence[str]],
```

## UserAttributeUpdateSettingsTypeOutputTypeDef

```python
# UserAttributeUpdateSettingsTypeOutputTypeDef definition

class UserAttributeUpdateSettingsTypeOutputTypeDef(TypedDict):
    AttributesRequireVerificationBeforeUpdate: NotRequired[List[VerifiedAttributeTypeType]],  # (1)
```

1. See [:material-code-brackets: VerifiedAttributeTypeType](./literals.md#verifiedattributetypetype) 
## VerifySoftwareTokenRequestRequestTypeDef

```python
# VerifySoftwareTokenRequestRequestTypeDef definition

class VerifySoftwareTokenRequestRequestTypeDef(TypedDict):
    UserCode: str,
    AccessToken: NotRequired[str],
    Session: NotRequired[str],
    FriendlyDeviceName: NotRequired[str],
```

## VerifyUserAttributeRequestRequestTypeDef

```python
# VerifyUserAttributeRequestRequestTypeDef definition

class VerifyUserAttributeRequestRequestTypeDef(TypedDict):
    AccessToken: str,
    AttributeName: str,
    Code: str,
```

## AccountRecoverySettingTypeOutputTypeDef

```python
# AccountRecoverySettingTypeOutputTypeDef definition

class AccountRecoverySettingTypeOutputTypeDef(TypedDict):
    RecoveryMechanisms: NotRequired[List[RecoveryOptionTypeTypeDef]],  # (1)
```

1. See [:material-code-braces: RecoveryOptionTypeTypeDef](./type_defs.md#recoveryoptiontypetypedef) 
## AccountRecoverySettingTypeTypeDef

```python
# AccountRecoverySettingTypeTypeDef definition

class AccountRecoverySettingTypeTypeDef(TypedDict):
    RecoveryMechanisms: NotRequired[Sequence[RecoveryOptionTypeTypeDef]],  # (1)
```

1. See [:material-code-braces: RecoveryOptionTypeTypeDef](./type_defs.md#recoveryoptiontypetypedef) 
## AccountTakeoverActionsTypeTypeDef

```python
# AccountTakeoverActionsTypeTypeDef definition

class AccountTakeoverActionsTypeTypeDef(TypedDict):
    LowAction: NotRequired[AccountTakeoverActionTypeTypeDef],  # (1)
    MediumAction: NotRequired[AccountTakeoverActionTypeTypeDef],  # (1)
    HighAction: NotRequired[AccountTakeoverActionTypeTypeDef],  # (1)
```

1. See [:material-code-braces: AccountTakeoverActionTypeTypeDef](./type_defs.md#accounttakeoveractiontypetypedef) 
2. See [:material-code-braces: AccountTakeoverActionTypeTypeDef](./type_defs.md#accounttakeoveractiontypetypedef) 
3. See [:material-code-braces: AccountTakeoverActionTypeTypeDef](./type_defs.md#accounttakeoveractiontypetypedef) 
## AdminCreateUserConfigTypeTypeDef

```python
# AdminCreateUserConfigTypeTypeDef definition

class AdminCreateUserConfigTypeTypeDef(TypedDict):
    AllowAdminCreateUserOnly: NotRequired[bool],
    UnusedAccountValidityDays: NotRequired[int],
    InviteMessageTemplate: NotRequired[MessageTemplateTypeTypeDef],  # (1)
```

1. See [:material-code-braces: MessageTemplateTypeTypeDef](./type_defs.md#messagetemplatetypetypedef) 
## AdminCreateUserRequestRequestTypeDef

```python
# AdminCreateUserRequestRequestTypeDef definition

class AdminCreateUserRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Username: str,
    UserAttributes: NotRequired[Sequence[AttributeTypeTypeDef]],  # (1)
    ValidationData: NotRequired[Sequence[AttributeTypeTypeDef]],  # (1)
    TemporaryPassword: NotRequired[str],
    ForceAliasCreation: NotRequired[bool],
    MessageAction: NotRequired[MessageActionTypeType],  # (3)
    DesiredDeliveryMediums: NotRequired[Sequence[DeliveryMediumTypeType]],  # (4)
    ClientMetadata: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AttributeTypeTypeDef](./type_defs.md#attributetypetypedef) 
2. See [:material-code-braces: AttributeTypeTypeDef](./type_defs.md#attributetypetypedef) 
3. See [:material-code-brackets: MessageActionTypeType](./literals.md#messageactiontypetype) 
4. See [:material-code-brackets: DeliveryMediumTypeType](./literals.md#deliverymediumtypetype) 
## AdminUpdateUserAttributesRequestRequestTypeDef

```python
# AdminUpdateUserAttributesRequestRequestTypeDef definition

class AdminUpdateUserAttributesRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Username: str,
    UserAttributes: Sequence[AttributeTypeTypeDef],  # (1)
    ClientMetadata: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AttributeTypeTypeDef](./type_defs.md#attributetypetypedef) 
## DeviceTypeTypeDef

```python
# DeviceTypeTypeDef definition

class DeviceTypeTypeDef(TypedDict):
    DeviceKey: NotRequired[str],
    DeviceAttributes: NotRequired[List[AttributeTypeTypeDef]],  # (1)
    DeviceCreateDate: NotRequired[datetime],
    DeviceLastModifiedDate: NotRequired[datetime],
    DeviceLastAuthenticatedDate: NotRequired[datetime],
```

1. See [:material-code-braces: AttributeTypeTypeDef](./type_defs.md#attributetypetypedef) 
## UpdateUserAttributesRequestRequestTypeDef

```python
# UpdateUserAttributesRequestRequestTypeDef definition

class UpdateUserAttributesRequestRequestTypeDef(TypedDict):
    UserAttributes: Sequence[AttributeTypeTypeDef],  # (1)
    AccessToken: str,
    ClientMetadata: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AttributeTypeTypeDef](./type_defs.md#attributetypetypedef) 
## AssociateSoftwareTokenResponseTypeDef

```python
# AssociateSoftwareTokenResponseTypeDef definition

class AssociateSoftwareTokenResponseTypeDef(TypedDict):
    SecretCode: str,
    Session: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfirmDeviceResponseTypeDef

```python
# ConfirmDeviceResponseTypeDef definition

class ConfirmDeviceResponseTypeDef(TypedDict):
    UserConfirmationNecessary: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfirmSignUpResponseTypeDef

```python
# ConfirmSignUpResponseTypeDef definition

class ConfirmSignUpResponseTypeDef(TypedDict):
    Session: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserPoolDomainResponseTypeDef

```python
# CreateUserPoolDomainResponseTypeDef definition

class CreateUserPoolDomainResponseTypeDef(TypedDict):
    ManagedLoginVersion: int,
    CloudFrontDomain: str,
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
## GetCSVHeaderResponseTypeDef

```python
# GetCSVHeaderResponseTypeDef definition

class GetCSVHeaderResponseTypeDef(TypedDict):
    UserPoolId: str,
    CSVHeader: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSigningCertificateResponseTypeDef

```python
# GetSigningCertificateResponseTypeDef definition

class GetSigningCertificateResponseTypeDef(TypedDict):
    Certificate: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUserAuthFactorsResponseTypeDef

```python
# GetUserAuthFactorsResponseTypeDef definition

class GetUserAuthFactorsResponseTypeDef(TypedDict):
    Username: str,
    PreferredMfaSetting: str,
    UserMFASettingList: List[str],
    ConfiguredUserAuthFactors: List[AuthFactorTypeType],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AuthFactorTypeType](./literals.md#authfactortypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartWebAuthnRegistrationResponseTypeDef

```python
# StartWebAuthnRegistrationResponseTypeDef definition

class StartWebAuthnRegistrationResponseTypeDef(TypedDict):
    CredentialCreationOptions: Dict[str, Any],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserPoolDomainResponseTypeDef

```python
# UpdateUserPoolDomainResponseTypeDef definition

class UpdateUserPoolDomainResponseTypeDef(TypedDict):
    ManagedLoginVersion: int,
    CloudFrontDomain: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VerifySoftwareTokenResponseTypeDef

```python
# VerifySoftwareTokenResponseTypeDef definition

class VerifySoftwareTokenResponseTypeDef(TypedDict):
    Status: VerifySoftwareTokenResponseTypeType,  # (1)
    Session: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: VerifySoftwareTokenResponseTypeType](./literals.md#verifysoftwaretokenresponsetypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AdminDisableProviderForUserRequestRequestTypeDef

```python
# AdminDisableProviderForUserRequestRequestTypeDef definition

class AdminDisableProviderForUserRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    User: ProviderUserIdentifierTypeTypeDef,  # (1)
```

1. See [:material-code-braces: ProviderUserIdentifierTypeTypeDef](./type_defs.md#provideruseridentifiertypetypedef) 
## AdminLinkProviderForUserRequestRequestTypeDef

```python
# AdminLinkProviderForUserRequestRequestTypeDef definition

class AdminLinkProviderForUserRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    DestinationUser: ProviderUserIdentifierTypeTypeDef,  # (1)
    SourceUser: ProviderUserIdentifierTypeTypeDef,  # (1)
```

1. See [:material-code-braces: ProviderUserIdentifierTypeTypeDef](./type_defs.md#provideruseridentifiertypetypedef) 
2. See [:material-code-braces: ProviderUserIdentifierTypeTypeDef](./type_defs.md#provideruseridentifiertypetypedef) 
## AdminGetUserResponseTypeDef

```python
# AdminGetUserResponseTypeDef definition

class AdminGetUserResponseTypeDef(TypedDict):
    Username: str,
    UserAttributes: List[AttributeTypeTypeDef],  # (1)
    UserCreateDate: datetime,
    UserLastModifiedDate: datetime,
    Enabled: bool,
    UserStatus: UserStatusTypeType,  # (2)
    MFAOptions: List[MFAOptionTypeTypeDef],  # (3)
    PreferredMfaSetting: str,
    UserMFASettingList: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AttributeTypeTypeDef](./type_defs.md#attributetypetypedef) 
2. See [:material-code-brackets: UserStatusTypeType](./literals.md#userstatustypetype) 
3. See [:material-code-braces: MFAOptionTypeTypeDef](./type_defs.md#mfaoptiontypetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AdminSetUserSettingsRequestRequestTypeDef

```python
# AdminSetUserSettingsRequestRequestTypeDef definition

class AdminSetUserSettingsRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Username: str,
    MFAOptions: Sequence[MFAOptionTypeTypeDef],  # (1)
```

1. See [:material-code-braces: MFAOptionTypeTypeDef](./type_defs.md#mfaoptiontypetypedef) 
## GetUserResponseTypeDef

```python
# GetUserResponseTypeDef definition

class GetUserResponseTypeDef(TypedDict):
    Username: str,
    UserAttributes: List[AttributeTypeTypeDef],  # (1)
    MFAOptions: List[MFAOptionTypeTypeDef],  # (2)
    PreferredMfaSetting: str,
    UserMFASettingList: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AttributeTypeTypeDef](./type_defs.md#attributetypetypedef) 
2. See [:material-code-braces: MFAOptionTypeTypeDef](./type_defs.md#mfaoptiontypetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetUserSettingsRequestRequestTypeDef

```python
# SetUserSettingsRequestRequestTypeDef definition

class SetUserSettingsRequestRequestTypeDef(TypedDict):
    AccessToken: str,
    MFAOptions: Sequence[MFAOptionTypeTypeDef],  # (1)
```

1. See [:material-code-braces: MFAOptionTypeTypeDef](./type_defs.md#mfaoptiontypetypedef) 
## UserTypeTypeDef

```python
# UserTypeTypeDef definition

class UserTypeTypeDef(TypedDict):
    Username: NotRequired[str],
    Attributes: NotRequired[List[AttributeTypeTypeDef]],  # (1)
    UserCreateDate: NotRequired[datetime],
    UserLastModifiedDate: NotRequired[datetime],
    Enabled: NotRequired[bool],
    UserStatus: NotRequired[UserStatusTypeType],  # (2)
    MFAOptions: NotRequired[List[MFAOptionTypeTypeDef]],  # (3)
```

1. See [:material-code-braces: AttributeTypeTypeDef](./type_defs.md#attributetypetypedef) 
2. See [:material-code-brackets: UserStatusTypeType](./literals.md#userstatustypetype) 
3. See [:material-code-braces: MFAOptionTypeTypeDef](./type_defs.md#mfaoptiontypetypedef) 
## AdminListGroupsForUserRequestPaginateTypeDef

```python
# AdminListGroupsForUserRequestPaginateTypeDef definition

class AdminListGroupsForUserRequestPaginateTypeDef(TypedDict):
    Username: str,
    UserPoolId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## AdminListUserAuthEventsRequestPaginateTypeDef

```python
# AdminListUserAuthEventsRequestPaginateTypeDef definition

class AdminListUserAuthEventsRequestPaginateTypeDef(TypedDict):
    UserPoolId: str,
    Username: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupsRequestPaginateTypeDef

```python
# ListGroupsRequestPaginateTypeDef definition

class ListGroupsRequestPaginateTypeDef(TypedDict):
    UserPoolId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIdentityProvidersRequestPaginateTypeDef

```python
# ListIdentityProvidersRequestPaginateTypeDef definition

class ListIdentityProvidersRequestPaginateTypeDef(TypedDict):
    UserPoolId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceServersRequestPaginateTypeDef

```python
# ListResourceServersRequestPaginateTypeDef definition

class ListResourceServersRequestPaginateTypeDef(TypedDict):
    UserPoolId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUserPoolClientsRequestPaginateTypeDef

```python
# ListUserPoolClientsRequestPaginateTypeDef definition

class ListUserPoolClientsRequestPaginateTypeDef(TypedDict):
    UserPoolId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUserPoolsRequestPaginateTypeDef

```python
# ListUserPoolsRequestPaginateTypeDef definition

class ListUserPoolsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUsersInGroupRequestPaginateTypeDef

```python
# ListUsersInGroupRequestPaginateTypeDef definition

class ListUsersInGroupRequestPaginateTypeDef(TypedDict):
    UserPoolId: str,
    GroupName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUsersRequestPaginateTypeDef

```python
# ListUsersRequestPaginateTypeDef definition

class ListUsersRequestPaginateTypeDef(TypedDict):
    UserPoolId: str,
    AttributesToGet: NotRequired[Sequence[str]],
    Filter: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## AdminListGroupsForUserResponseTypeDef

```python
# AdminListGroupsForUserResponseTypeDef definition

class AdminListGroupsForUserResponseTypeDef(TypedDict):
    Groups: List[GroupTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GroupTypeTypeDef](./type_defs.md#grouptypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGroupResponseTypeDef

```python
# CreateGroupResponseTypeDef definition

class CreateGroupResponseTypeDef(TypedDict):
    Group: GroupTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupTypeTypeDef](./type_defs.md#grouptypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGroupResponseTypeDef

```python
# GetGroupResponseTypeDef definition

class GetGroupResponseTypeDef(TypedDict):
    Group: GroupTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupTypeTypeDef](./type_defs.md#grouptypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGroupsResponseTypeDef

```python
# ListGroupsResponseTypeDef definition

class ListGroupsResponseTypeDef(TypedDict):
    Groups: List[GroupTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GroupTypeTypeDef](./type_defs.md#grouptypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGroupResponseTypeDef

```python
# UpdateGroupResponseTypeDef definition

class UpdateGroupResponseTypeDef(TypedDict):
    Group: GroupTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupTypeTypeDef](./type_defs.md#grouptypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AdminSetUserMFAPreferenceRequestRequestTypeDef

```python
# AdminSetUserMFAPreferenceRequestRequestTypeDef definition

class AdminSetUserMFAPreferenceRequestRequestTypeDef(TypedDict):
    Username: str,
    UserPoolId: str,
    SMSMfaSettings: NotRequired[SMSMfaSettingsTypeTypeDef],  # (1)
    SoftwareTokenMfaSettings: NotRequired[SoftwareTokenMfaSettingsTypeTypeDef],  # (2)
    EmailMfaSettings: NotRequired[EmailMfaSettingsTypeTypeDef],  # (3)
```

1. See [:material-code-braces: SMSMfaSettingsTypeTypeDef](./type_defs.md#smsmfasettingstypetypedef) 
2. See [:material-code-braces: SoftwareTokenMfaSettingsTypeTypeDef](./type_defs.md#softwaretokenmfasettingstypetypedef) 
3. See [:material-code-braces: EmailMfaSettingsTypeTypeDef](./type_defs.md#emailmfasettingstypetypedef) 
## SetUserMFAPreferenceRequestRequestTypeDef

```python
# SetUserMFAPreferenceRequestRequestTypeDef definition

class SetUserMFAPreferenceRequestRequestTypeDef(TypedDict):
    AccessToken: str,
    SMSMfaSettings: NotRequired[SMSMfaSettingsTypeTypeDef],  # (1)
    SoftwareTokenMfaSettings: NotRequired[SoftwareTokenMfaSettingsTypeTypeDef],  # (2)
    EmailMfaSettings: NotRequired[EmailMfaSettingsTypeTypeDef],  # (3)
```

1. See [:material-code-braces: SMSMfaSettingsTypeTypeDef](./type_defs.md#smsmfasettingstypetypedef) 
2. See [:material-code-braces: SoftwareTokenMfaSettingsTypeTypeDef](./type_defs.md#softwaretokenmfasettingstypetypedef) 
3. See [:material-code-braces: EmailMfaSettingsTypeTypeDef](./type_defs.md#emailmfasettingstypetypedef) 
## UserPoolAddOnsTypeTypeDef

```python
# UserPoolAddOnsTypeTypeDef definition

class UserPoolAddOnsTypeTypeDef(TypedDict):
    AdvancedSecurityMode: AdvancedSecurityModeTypeType,  # (1)
    AdvancedSecurityAdditionalFlows: NotRequired[AdvancedSecurityAdditionalFlowsTypeTypeDef],  # (2)
```

1. See [:material-code-brackets: AdvancedSecurityModeTypeType](./literals.md#advancedsecuritymodetypetype) 
2. See [:material-code-braces: AdvancedSecurityAdditionalFlowsTypeTypeDef](./type_defs.md#advancedsecurityadditionalflowstypetypedef) 
## ManagedLoginBrandingTypeTypeDef

```python
# ManagedLoginBrandingTypeTypeDef definition

class ManagedLoginBrandingTypeTypeDef(TypedDict):
    ManagedLoginBrandingId: NotRequired[str],
    UserPoolId: NotRequired[str],
    UseCognitoProvidedValues: NotRequired[bool],
    Settings: NotRequired[Dict[str, Any]],
    Assets: NotRequired[List[AssetTypeOutputTypeDef]],  # (1)
    CreationDate: NotRequired[datetime],
    LastModifiedDate: NotRequired[datetime],
```

1. See [:material-code-braces: AssetTypeOutputTypeDef](./type_defs.md#assettypeoutputtypedef) 
## AssetTypeTypeDef

```python
# AssetTypeTypeDef definition

class AssetTypeTypeDef(TypedDict):
    Category: AssetCategoryTypeType,  # (1)
    ColorMode: ColorSchemeModeTypeType,  # (2)
    Extension: AssetExtensionTypeType,  # (3)
    Bytes: NotRequired[BlobTypeDef],
    ResourceId: NotRequired[str],
```

1. See [:material-code-brackets: AssetCategoryTypeType](./literals.md#assetcategorytypetype) 
2. See [:material-code-brackets: ColorSchemeModeTypeType](./literals.md#colorschememodetypetype) 
3. See [:material-code-brackets: AssetExtensionTypeType](./literals.md#assetextensiontypetype) 
## SetUICustomizationRequestRequestTypeDef

```python
# SetUICustomizationRequestRequestTypeDef definition

class SetUICustomizationRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    ClientId: NotRequired[str],
    CSS: NotRequired[str],
    ImageFile: NotRequired[BlobTypeDef],
```

## AuthEventTypeTypeDef

```python
# AuthEventTypeTypeDef definition

class AuthEventTypeTypeDef(TypedDict):
    EventId: NotRequired[str],
    EventType: NotRequired[EventTypeType],  # (1)
    CreationDate: NotRequired[datetime],
    EventResponse: NotRequired[EventResponseTypeType],  # (2)
    EventRisk: NotRequired[EventRiskTypeTypeDef],  # (3)
    ChallengeResponses: NotRequired[List[ChallengeResponseTypeTypeDef]],  # (4)
    EventContextData: NotRequired[EventContextDataTypeTypeDef],  # (5)
    EventFeedback: NotRequired[EventFeedbackTypeTypeDef],  # (6)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
2. See [:material-code-brackets: EventResponseTypeType](./literals.md#eventresponsetypetype) 
3. See [:material-code-braces: EventRiskTypeTypeDef](./type_defs.md#eventrisktypetypedef) 
4. See [:material-code-braces: ChallengeResponseTypeTypeDef](./type_defs.md#challengeresponsetypetypedef) 
5. See [:material-code-braces: EventContextDataTypeTypeDef](./type_defs.md#eventcontextdatatypetypedef) 
6. See [:material-code-braces: EventFeedbackTypeTypeDef](./type_defs.md#eventfeedbacktypetypedef) 
## AuthenticationResultTypeTypeDef

```python
# AuthenticationResultTypeTypeDef definition

class AuthenticationResultTypeTypeDef(TypedDict):
    AccessToken: NotRequired[str],
    ExpiresIn: NotRequired[int],
    TokenType: NotRequired[str],
    RefreshToken: NotRequired[str],
    IdToken: NotRequired[str],
    NewDeviceMetadata: NotRequired[NewDeviceMetadataTypeTypeDef],  # (1)
```

1. See [:material-code-braces: NewDeviceMetadataTypeTypeDef](./type_defs.md#newdevicemetadatatypetypedef) 
## ForgotPasswordResponseTypeDef

```python
# ForgotPasswordResponseTypeDef definition

class ForgotPasswordResponseTypeDef(TypedDict):
    CodeDeliveryDetails: CodeDeliveryDetailsTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CodeDeliveryDetailsTypeTypeDef](./type_defs.md#codedeliverydetailstypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUserAttributeVerificationCodeResponseTypeDef

```python
# GetUserAttributeVerificationCodeResponseTypeDef definition

class GetUserAttributeVerificationCodeResponseTypeDef(TypedDict):
    CodeDeliveryDetails: CodeDeliveryDetailsTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CodeDeliveryDetailsTypeTypeDef](./type_defs.md#codedeliverydetailstypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResendConfirmationCodeResponseTypeDef

```python
# ResendConfirmationCodeResponseTypeDef definition

class ResendConfirmationCodeResponseTypeDef(TypedDict):
    CodeDeliveryDetails: CodeDeliveryDetailsTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CodeDeliveryDetailsTypeTypeDef](./type_defs.md#codedeliverydetailstypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SignUpResponseTypeDef

```python
# SignUpResponseTypeDef definition

class SignUpResponseTypeDef(TypedDict):
    UserConfirmed: bool,
    CodeDeliveryDetails: CodeDeliveryDetailsTypeTypeDef,  # (1)
    UserSub: str,
    Session: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CodeDeliveryDetailsTypeTypeDef](./type_defs.md#codedeliverydetailstypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserAttributesResponseTypeDef

```python
# UpdateUserAttributesResponseTypeDef definition

class UpdateUserAttributesResponseTypeDef(TypedDict):
    CodeDeliveryDetailsList: List[CodeDeliveryDetailsTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CodeDeliveryDetailsTypeTypeDef](./type_defs.md#codedeliverydetailstypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CompromisedCredentialsRiskConfigurationTypeOutputTypeDef

```python
# CompromisedCredentialsRiskConfigurationTypeOutputTypeDef definition

class CompromisedCredentialsRiskConfigurationTypeOutputTypeDef(TypedDict):
    Actions: CompromisedCredentialsActionsTypeTypeDef,  # (2)
    EventFilter: NotRequired[List[EventFilterTypeType]],  # (1)
```

1. See [:material-code-brackets: EventFilterTypeType](./literals.md#eventfiltertypetype) 
2. See [:material-code-braces: CompromisedCredentialsActionsTypeTypeDef](./type_defs.md#compromisedcredentialsactionstypetypedef) 
## CompromisedCredentialsRiskConfigurationTypeTypeDef

```python
# CompromisedCredentialsRiskConfigurationTypeTypeDef definition

class CompromisedCredentialsRiskConfigurationTypeTypeDef(TypedDict):
    Actions: CompromisedCredentialsActionsTypeTypeDef,  # (2)
    EventFilter: NotRequired[Sequence[EventFilterTypeType]],  # (1)
```

1. See [:material-code-brackets: EventFilterTypeType](./literals.md#eventfiltertypetype) 
2. See [:material-code-braces: CompromisedCredentialsActionsTypeTypeDef](./type_defs.md#compromisedcredentialsactionstypetypedef) 
## ConfirmDeviceRequestRequestTypeDef

```python
# ConfirmDeviceRequestRequestTypeDef definition

class ConfirmDeviceRequestRequestTypeDef(TypedDict):
    AccessToken: str,
    DeviceKey: str,
    DeviceSecretVerifierConfig: NotRequired[DeviceSecretVerifierConfigTypeTypeDef],  # (1)
    DeviceName: NotRequired[str],
```

1. See [:material-code-braces: DeviceSecretVerifierConfigTypeTypeDef](./type_defs.md#devicesecretverifierconfigtypetypedef) 
## ConfirmForgotPasswordRequestRequestTypeDef

```python
# ConfirmForgotPasswordRequestRequestTypeDef definition

class ConfirmForgotPasswordRequestRequestTypeDef(TypedDict):
    ClientId: str,
    Username: str,
    ConfirmationCode: str,
    Password: str,
    SecretHash: NotRequired[str],
    AnalyticsMetadata: NotRequired[AnalyticsMetadataTypeTypeDef],  # (1)
    UserContextData: NotRequired[UserContextDataTypeTypeDef],  # (2)
    ClientMetadata: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AnalyticsMetadataTypeTypeDef](./type_defs.md#analyticsmetadatatypetypedef) 
2. See [:material-code-braces: UserContextDataTypeTypeDef](./type_defs.md#usercontextdatatypetypedef) 
## ConfirmSignUpRequestRequestTypeDef

```python
# ConfirmSignUpRequestRequestTypeDef definition

class ConfirmSignUpRequestRequestTypeDef(TypedDict):
    ClientId: str,
    Username: str,
    ConfirmationCode: str,
    SecretHash: NotRequired[str],
    ForceAliasCreation: NotRequired[bool],
    AnalyticsMetadata: NotRequired[AnalyticsMetadataTypeTypeDef],  # (1)
    UserContextData: NotRequired[UserContextDataTypeTypeDef],  # (2)
    ClientMetadata: NotRequired[Mapping[str, str]],
    Session: NotRequired[str],
```

1. See [:material-code-braces: AnalyticsMetadataTypeTypeDef](./type_defs.md#analyticsmetadatatypetypedef) 
2. See [:material-code-braces: UserContextDataTypeTypeDef](./type_defs.md#usercontextdatatypetypedef) 
## ForgotPasswordRequestRequestTypeDef

```python
# ForgotPasswordRequestRequestTypeDef definition

class ForgotPasswordRequestRequestTypeDef(TypedDict):
    ClientId: str,
    Username: str,
    SecretHash: NotRequired[str],
    UserContextData: NotRequired[UserContextDataTypeTypeDef],  # (1)
    AnalyticsMetadata: NotRequired[AnalyticsMetadataTypeTypeDef],  # (2)
    ClientMetadata: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: UserContextDataTypeTypeDef](./type_defs.md#usercontextdatatypetypedef) 
2. See [:material-code-braces: AnalyticsMetadataTypeTypeDef](./type_defs.md#analyticsmetadatatypetypedef) 
## InitiateAuthRequestRequestTypeDef

```python
# InitiateAuthRequestRequestTypeDef definition

class InitiateAuthRequestRequestTypeDef(TypedDict):
    AuthFlow: AuthFlowTypeType,  # (1)
    ClientId: str,
    AuthParameters: NotRequired[Mapping[str, str]],
    ClientMetadata: NotRequired[Mapping[str, str]],
    AnalyticsMetadata: NotRequired[AnalyticsMetadataTypeTypeDef],  # (2)
    UserContextData: NotRequired[UserContextDataTypeTypeDef],  # (3)
    Session: NotRequired[str],
```

1. See [:material-code-brackets: AuthFlowTypeType](./literals.md#authflowtypetype) 
2. See [:material-code-braces: AnalyticsMetadataTypeTypeDef](./type_defs.md#analyticsmetadatatypetypedef) 
3. See [:material-code-braces: UserContextDataTypeTypeDef](./type_defs.md#usercontextdatatypetypedef) 
## ResendConfirmationCodeRequestRequestTypeDef

```python
# ResendConfirmationCodeRequestRequestTypeDef definition

class ResendConfirmationCodeRequestRequestTypeDef(TypedDict):
    ClientId: str,
    Username: str,
    SecretHash: NotRequired[str],
    UserContextData: NotRequired[UserContextDataTypeTypeDef],  # (1)
    AnalyticsMetadata: NotRequired[AnalyticsMetadataTypeTypeDef],  # (2)
    ClientMetadata: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: UserContextDataTypeTypeDef](./type_defs.md#usercontextdatatypetypedef) 
2. See [:material-code-braces: AnalyticsMetadataTypeTypeDef](./type_defs.md#analyticsmetadatatypetypedef) 
## RespondToAuthChallengeRequestRequestTypeDef

```python
# RespondToAuthChallengeRequestRequestTypeDef definition

class RespondToAuthChallengeRequestRequestTypeDef(TypedDict):
    ClientId: str,
    ChallengeName: ChallengeNameTypeType,  # (1)
    Session: NotRequired[str],
    ChallengeResponses: NotRequired[Mapping[str, str]],
    AnalyticsMetadata: NotRequired[AnalyticsMetadataTypeTypeDef],  # (2)
    UserContextData: NotRequired[UserContextDataTypeTypeDef],  # (3)
    ClientMetadata: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ChallengeNameTypeType](./literals.md#challengenametypetype) 
2. See [:material-code-braces: AnalyticsMetadataTypeTypeDef](./type_defs.md#analyticsmetadatatypetypedef) 
3. See [:material-code-braces: UserContextDataTypeTypeDef](./type_defs.md#usercontextdatatypetypedef) 
## SignUpRequestRequestTypeDef

```python
# SignUpRequestRequestTypeDef definition

class SignUpRequestRequestTypeDef(TypedDict):
    ClientId: str,
    Username: str,
    SecretHash: NotRequired[str],
    Password: NotRequired[str],
    UserAttributes: NotRequired[Sequence[AttributeTypeTypeDef]],  # (1)
    ValidationData: NotRequired[Sequence[AttributeTypeTypeDef]],  # (1)
    AnalyticsMetadata: NotRequired[AnalyticsMetadataTypeTypeDef],  # (3)
    UserContextData: NotRequired[UserContextDataTypeTypeDef],  # (4)
    ClientMetadata: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AttributeTypeTypeDef](./type_defs.md#attributetypetypedef) 
2. See [:material-code-braces: AttributeTypeTypeDef](./type_defs.md#attributetypetypedef) 
3. See [:material-code-braces: AnalyticsMetadataTypeTypeDef](./type_defs.md#analyticsmetadatatypetypedef) 
4. See [:material-code-braces: UserContextDataTypeTypeDef](./type_defs.md#usercontextdatatypetypedef) 
## ContextDataTypeTypeDef

```python
# ContextDataTypeTypeDef definition

class ContextDataTypeTypeDef(TypedDict):
    IpAddress: str,
    ServerName: str,
    ServerPath: str,
    HttpHeaders: Sequence[HttpHeaderTypeDef],  # (1)
    EncodedData: NotRequired[str],
```

1. See [:material-code-braces: HttpHeaderTypeDef](./type_defs.md#httpheadertypedef) 
## CreateIdentityProviderResponseTypeDef

```python
# CreateIdentityProviderResponseTypeDef definition

class CreateIdentityProviderResponseTypeDef(TypedDict):
    IdentityProvider: IdentityProviderTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityProviderTypeTypeDef](./type_defs.md#identityprovidertypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeIdentityProviderResponseTypeDef

```python
# DescribeIdentityProviderResponseTypeDef definition

class DescribeIdentityProviderResponseTypeDef(TypedDict):
    IdentityProvider: IdentityProviderTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityProviderTypeTypeDef](./type_defs.md#identityprovidertypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIdentityProviderByIdentifierResponseTypeDef

```python
# GetIdentityProviderByIdentifierResponseTypeDef definition

class GetIdentityProviderByIdentifierResponseTypeDef(TypedDict):
    IdentityProvider: IdentityProviderTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityProviderTypeTypeDef](./type_defs.md#identityprovidertypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIdentityProviderResponseTypeDef

```python
# UpdateIdentityProviderResponseTypeDef definition

class UpdateIdentityProviderResponseTypeDef(TypedDict):
    IdentityProvider: IdentityProviderTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityProviderTypeTypeDef](./type_defs.md#identityprovidertypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateResourceServerRequestRequestTypeDef

```python
# CreateResourceServerRequestRequestTypeDef definition

class CreateResourceServerRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Identifier: str,
    Name: str,
    Scopes: NotRequired[Sequence[ResourceServerScopeTypeTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourceServerScopeTypeTypeDef](./type_defs.md#resourceserverscopetypetypedef) 
## ResourceServerTypeTypeDef

```python
# ResourceServerTypeTypeDef definition

class ResourceServerTypeTypeDef(TypedDict):
    UserPoolId: NotRequired[str],
    Identifier: NotRequired[str],
    Name: NotRequired[str],
    Scopes: NotRequired[List[ResourceServerScopeTypeTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourceServerScopeTypeTypeDef](./type_defs.md#resourceserverscopetypetypedef) 
## UpdateResourceServerRequestRequestTypeDef

```python
# UpdateResourceServerRequestRequestTypeDef definition

class UpdateResourceServerRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Identifier: str,
    Name: str,
    Scopes: NotRequired[Sequence[ResourceServerScopeTypeTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourceServerScopeTypeTypeDef](./type_defs.md#resourceserverscopetypetypedef) 
## CreateUserImportJobResponseTypeDef

```python
# CreateUserImportJobResponseTypeDef definition

class CreateUserImportJobResponseTypeDef(TypedDict):
    UserImportJob: UserImportJobTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserImportJobTypeTypeDef](./type_defs.md#userimportjobtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeUserImportJobResponseTypeDef

```python
# DescribeUserImportJobResponseTypeDef definition

class DescribeUserImportJobResponseTypeDef(TypedDict):
    UserImportJob: UserImportJobTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserImportJobTypeTypeDef](./type_defs.md#userimportjobtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUserImportJobsResponseTypeDef

```python
# ListUserImportJobsResponseTypeDef definition

class ListUserImportJobsResponseTypeDef(TypedDict):
    UserImportJobs: List[UserImportJobTypeTypeDef],  # (1)
    PaginationToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserImportJobTypeTypeDef](./type_defs.md#userimportjobtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartUserImportJobResponseTypeDef

```python
# StartUserImportJobResponseTypeDef definition

class StartUserImportJobResponseTypeDef(TypedDict):
    UserImportJob: UserImportJobTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserImportJobTypeTypeDef](./type_defs.md#userimportjobtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopUserImportJobResponseTypeDef

```python
# StopUserImportJobResponseTypeDef definition

class StopUserImportJobResponseTypeDef(TypedDict):
    UserImportJob: UserImportJobTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserImportJobTypeTypeDef](./type_defs.md#userimportjobtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserPoolClientRequestRequestTypeDef

```python
# CreateUserPoolClientRequestRequestTypeDef definition

class CreateUserPoolClientRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    ClientName: str,
    GenerateSecret: NotRequired[bool],
    RefreshTokenValidity: NotRequired[int],
    AccessTokenValidity: NotRequired[int],
    IdTokenValidity: NotRequired[int],
    TokenValidityUnits: NotRequired[TokenValidityUnitsTypeTypeDef],  # (1)
    ReadAttributes: NotRequired[Sequence[str]],
    WriteAttributes: NotRequired[Sequence[str]],
    ExplicitAuthFlows: NotRequired[Sequence[ExplicitAuthFlowsTypeType]],  # (2)
    SupportedIdentityProviders: NotRequired[Sequence[str]],
    CallbackURLs: NotRequired[Sequence[str]],
    LogoutURLs: NotRequired[Sequence[str]],
    DefaultRedirectURI: NotRequired[str],
    AllowedOAuthFlows: NotRequired[Sequence[OAuthFlowTypeType]],  # (3)
    AllowedOAuthScopes: NotRequired[Sequence[str]],
    AllowedOAuthFlowsUserPoolClient: NotRequired[bool],
    AnalyticsConfiguration: NotRequired[AnalyticsConfigurationTypeTypeDef],  # (4)
    PreventUserExistenceErrors: NotRequired[PreventUserExistenceErrorTypesType],  # (5)
    EnableTokenRevocation: NotRequired[bool],
    EnablePropagateAdditionalUserContextData: NotRequired[bool],
    AuthSessionValidity: NotRequired[int],
```

1. See [:material-code-braces: TokenValidityUnitsTypeTypeDef](./type_defs.md#tokenvalidityunitstypetypedef) 
2. See [:material-code-brackets: ExplicitAuthFlowsTypeType](./literals.md#explicitauthflowstypetype) 
3. See [:material-code-brackets: OAuthFlowTypeType](./literals.md#oauthflowtypetype) 
4. See [:material-code-braces: AnalyticsConfigurationTypeTypeDef](./type_defs.md#analyticsconfigurationtypetypedef) 
5. See [:material-code-brackets: PreventUserExistenceErrorTypesType](./literals.md#preventuserexistenceerrortypestype) 
## UpdateUserPoolClientRequestRequestTypeDef

```python
# UpdateUserPoolClientRequestRequestTypeDef definition

class UpdateUserPoolClientRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    ClientId: str,
    ClientName: NotRequired[str],
    RefreshTokenValidity: NotRequired[int],
    AccessTokenValidity: NotRequired[int],
    IdTokenValidity: NotRequired[int],
    TokenValidityUnits: NotRequired[TokenValidityUnitsTypeTypeDef],  # (1)
    ReadAttributes: NotRequired[Sequence[str]],
    WriteAttributes: NotRequired[Sequence[str]],
    ExplicitAuthFlows: NotRequired[Sequence[ExplicitAuthFlowsTypeType]],  # (2)
    SupportedIdentityProviders: NotRequired[Sequence[str]],
    CallbackURLs: NotRequired[Sequence[str]],
    LogoutURLs: NotRequired[Sequence[str]],
    DefaultRedirectURI: NotRequired[str],
    AllowedOAuthFlows: NotRequired[Sequence[OAuthFlowTypeType]],  # (3)
    AllowedOAuthScopes: NotRequired[Sequence[str]],
    AllowedOAuthFlowsUserPoolClient: NotRequired[bool],
    AnalyticsConfiguration: NotRequired[AnalyticsConfigurationTypeTypeDef],  # (4)
    PreventUserExistenceErrors: NotRequired[PreventUserExistenceErrorTypesType],  # (5)
    EnableTokenRevocation: NotRequired[bool],
    EnablePropagateAdditionalUserContextData: NotRequired[bool],
    AuthSessionValidity: NotRequired[int],
```

1. See [:material-code-braces: TokenValidityUnitsTypeTypeDef](./type_defs.md#tokenvalidityunitstypetypedef) 
2. See [:material-code-brackets: ExplicitAuthFlowsTypeType](./literals.md#explicitauthflowstypetype) 
3. See [:material-code-brackets: OAuthFlowTypeType](./literals.md#oauthflowtypetype) 
4. See [:material-code-braces: AnalyticsConfigurationTypeTypeDef](./type_defs.md#analyticsconfigurationtypetypedef) 
5. See [:material-code-brackets: PreventUserExistenceErrorTypesType](./literals.md#preventuserexistenceerrortypestype) 
## UserPoolClientTypeTypeDef

```python
# UserPoolClientTypeTypeDef definition

class UserPoolClientTypeTypeDef(TypedDict):
    UserPoolId: NotRequired[str],
    ClientName: NotRequired[str],
    ClientId: NotRequired[str],
    ClientSecret: NotRequired[str],
    LastModifiedDate: NotRequired[datetime],
    CreationDate: NotRequired[datetime],
    RefreshTokenValidity: NotRequired[int],
    AccessTokenValidity: NotRequired[int],
    IdTokenValidity: NotRequired[int],
    TokenValidityUnits: NotRequired[TokenValidityUnitsTypeTypeDef],  # (1)
    ReadAttributes: NotRequired[List[str]],
    WriteAttributes: NotRequired[List[str]],
    ExplicitAuthFlows: NotRequired[List[ExplicitAuthFlowsTypeType]],  # (2)
    SupportedIdentityProviders: NotRequired[List[str]],
    CallbackURLs: NotRequired[List[str]],
    LogoutURLs: NotRequired[List[str]],
    DefaultRedirectURI: NotRequired[str],
    AllowedOAuthFlows: NotRequired[List[OAuthFlowTypeType]],  # (3)
    AllowedOAuthScopes: NotRequired[List[str]],
    AllowedOAuthFlowsUserPoolClient: NotRequired[bool],
    AnalyticsConfiguration: NotRequired[AnalyticsConfigurationTypeTypeDef],  # (4)
    PreventUserExistenceErrors: NotRequired[PreventUserExistenceErrorTypesType],  # (5)
    EnableTokenRevocation: NotRequired[bool],
    EnablePropagateAdditionalUserContextData: NotRequired[bool],
    AuthSessionValidity: NotRequired[int],
```

1. See [:material-code-braces: TokenValidityUnitsTypeTypeDef](./type_defs.md#tokenvalidityunitstypetypedef) 
2. See [:material-code-brackets: ExplicitAuthFlowsTypeType](./literals.md#explicitauthflowstypetype) 
3. See [:material-code-brackets: OAuthFlowTypeType](./literals.md#oauthflowtypetype) 
4. See [:material-code-braces: AnalyticsConfigurationTypeTypeDef](./type_defs.md#analyticsconfigurationtypetypedef) 
5. See [:material-code-brackets: PreventUserExistenceErrorTypesType](./literals.md#preventuserexistenceerrortypestype) 
## CreateUserPoolDomainRequestRequestTypeDef

```python
# CreateUserPoolDomainRequestRequestTypeDef definition

class CreateUserPoolDomainRequestRequestTypeDef(TypedDict):
    Domain: str,
    UserPoolId: str,
    ManagedLoginVersion: NotRequired[int],
    CustomDomainConfig: NotRequired[CustomDomainConfigTypeTypeDef],  # (1)
```

1. See [:material-code-braces: CustomDomainConfigTypeTypeDef](./type_defs.md#customdomainconfigtypetypedef) 
## DomainDescriptionTypeTypeDef

```python
# DomainDescriptionTypeTypeDef definition

class DomainDescriptionTypeTypeDef(TypedDict):
    UserPoolId: NotRequired[str],
    AWSAccountId: NotRequired[str],
    Domain: NotRequired[str],
    S3Bucket: NotRequired[str],
    CloudFrontDistribution: NotRequired[str],
    Version: NotRequired[str],
    Status: NotRequired[DomainStatusTypeType],  # (1)
    CustomDomainConfig: NotRequired[CustomDomainConfigTypeTypeDef],  # (2)
    ManagedLoginVersion: NotRequired[int],
```

1. See [:material-code-brackets: DomainStatusTypeType](./literals.md#domainstatustypetype) 
2. See [:material-code-braces: CustomDomainConfigTypeTypeDef](./type_defs.md#customdomainconfigtypetypedef) 
## UpdateUserPoolDomainRequestRequestTypeDef

```python
# UpdateUserPoolDomainRequestRequestTypeDef definition

class UpdateUserPoolDomainRequestRequestTypeDef(TypedDict):
    Domain: str,
    UserPoolId: str,
    ManagedLoginVersion: NotRequired[int],
    CustomDomainConfig: NotRequired[CustomDomainConfigTypeTypeDef],  # (1)
```

1. See [:material-code-braces: CustomDomainConfigTypeTypeDef](./type_defs.md#customdomainconfigtypetypedef) 
## SmsMfaConfigTypeTypeDef

```python
# SmsMfaConfigTypeTypeDef definition

class SmsMfaConfigTypeTypeDef(TypedDict):
    SmsAuthenticationMessage: NotRequired[str],
    SmsConfiguration: NotRequired[SmsConfigurationTypeTypeDef],  # (1)
```

1. See [:material-code-braces: SmsConfigurationTypeTypeDef](./type_defs.md#smsconfigurationtypetypedef) 
## GetUICustomizationResponseTypeDef

```python
# GetUICustomizationResponseTypeDef definition

class GetUICustomizationResponseTypeDef(TypedDict):
    UICustomization: UICustomizationTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UICustomizationTypeTypeDef](./type_defs.md#uicustomizationtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetUICustomizationResponseTypeDef

```python
# SetUICustomizationResponseTypeDef definition

class SetUICustomizationResponseTypeDef(TypedDict):
    UICustomization: UICustomizationTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UICustomizationTypeTypeDef](./type_defs.md#uicustomizationtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LambdaConfigTypeTypeDef

```python
# LambdaConfigTypeTypeDef definition

class LambdaConfigTypeTypeDef(TypedDict):
    PreSignUp: NotRequired[str],
    CustomMessage: NotRequired[str],
    PostConfirmation: NotRequired[str],
    PreAuthentication: NotRequired[str],
    PostAuthentication: NotRequired[str],
    DefineAuthChallenge: NotRequired[str],
    CreateAuthChallenge: NotRequired[str],
    VerifyAuthChallengeResponse: NotRequired[str],
    PreTokenGeneration: NotRequired[str],
    UserMigration: NotRequired[str],
    PreTokenGenerationConfig: NotRequired[PreTokenGenerationVersionConfigTypeTypeDef],  # (1)
    CustomSMSSender: NotRequired[CustomSMSLambdaVersionConfigTypeTypeDef],  # (2)
    CustomEmailSender: NotRequired[CustomEmailLambdaVersionConfigTypeTypeDef],  # (3)
    KMSKeyID: NotRequired[str],
```

1. See [:material-code-braces: PreTokenGenerationVersionConfigTypeTypeDef](./type_defs.md#pretokengenerationversionconfigtypetypedef) 
2. See [:material-code-braces: CustomSMSLambdaVersionConfigTypeTypeDef](./type_defs.md#customsmslambdaversionconfigtypetypedef) 
3. See [:material-code-braces: CustomEmailLambdaVersionConfigTypeTypeDef](./type_defs.md#customemaillambdaversionconfigtypetypedef) 
## ListIdentityProvidersResponseTypeDef

```python
# ListIdentityProvidersResponseTypeDef definition

class ListIdentityProvidersResponseTypeDef(TypedDict):
    Providers: List[ProviderDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProviderDescriptionTypeDef](./type_defs.md#providerdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUserPoolClientsResponseTypeDef

```python
# ListUserPoolClientsResponseTypeDef definition

class ListUserPoolClientsResponseTypeDef(TypedDict):
    UserPoolClients: List[UserPoolClientDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UserPoolClientDescriptionTypeDef](./type_defs.md#userpoolclientdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWebAuthnCredentialsResponseTypeDef

```python
# ListWebAuthnCredentialsResponseTypeDef definition

class ListWebAuthnCredentialsResponseTypeDef(TypedDict):
    Credentials: List[WebAuthnCredentialDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: WebAuthnCredentialDescriptionTypeDef](./type_defs.md#webauthncredentialdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LogConfigurationTypeTypeDef

```python
# LogConfigurationTypeTypeDef definition

class LogConfigurationTypeTypeDef(TypedDict):
    LogLevel: LogLevelType,  # (1)
    EventSource: EventSourceNameType,  # (2)
    CloudWatchLogsConfiguration: NotRequired[CloudWatchLogsConfigurationTypeTypeDef],  # (3)
    S3Configuration: NotRequired[S3ConfigurationTypeTypeDef],  # (4)
    FirehoseConfiguration: NotRequired[FirehoseConfigurationTypeTypeDef],  # (5)
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
2. See [:material-code-brackets: EventSourceNameType](./literals.md#eventsourcenametype) 
3. See [:material-code-braces: CloudWatchLogsConfigurationTypeTypeDef](./type_defs.md#cloudwatchlogsconfigurationtypetypedef) 
4. See [:material-code-braces: S3ConfigurationTypeTypeDef](./type_defs.md#s3configurationtypetypedef) 
5. See [:material-code-braces: FirehoseConfigurationTypeTypeDef](./type_defs.md#firehoseconfigurationtypetypedef) 
## NotifyConfigurationTypeTypeDef

```python
# NotifyConfigurationTypeTypeDef definition

class NotifyConfigurationTypeTypeDef(TypedDict):
    SourceArn: str,
    From: NotRequired[str],
    ReplyTo: NotRequired[str],
    BlockEmail: NotRequired[NotifyEmailTypeTypeDef],  # (1)
    NoActionEmail: NotRequired[NotifyEmailTypeTypeDef],  # (1)
    MfaEmail: NotRequired[NotifyEmailTypeTypeDef],  # (1)
```

1. See [:material-code-braces: NotifyEmailTypeTypeDef](./type_defs.md#notifyemailtypetypedef) 
2. See [:material-code-braces: NotifyEmailTypeTypeDef](./type_defs.md#notifyemailtypetypedef) 
3. See [:material-code-braces: NotifyEmailTypeTypeDef](./type_defs.md#notifyemailtypetypedef) 
## SchemaAttributeTypeTypeDef

```python
# SchemaAttributeTypeTypeDef definition

class SchemaAttributeTypeTypeDef(TypedDict):
    Name: NotRequired[str],
    AttributeDataType: NotRequired[AttributeDataTypeType],  # (1)
    DeveloperOnlyAttribute: NotRequired[bool],
    Mutable: NotRequired[bool],
    Required: NotRequired[bool],
    NumberAttributeConstraints: NotRequired[NumberAttributeConstraintsTypeTypeDef],  # (2)
    StringAttributeConstraints: NotRequired[StringAttributeConstraintsTypeTypeDef],  # (3)
```

1. See [:material-code-brackets: AttributeDataTypeType](./literals.md#attributedatatypetype) 
2. See [:material-code-braces: NumberAttributeConstraintsTypeTypeDef](./type_defs.md#numberattributeconstraintstypetypedef) 
3. See [:material-code-braces: StringAttributeConstraintsTypeTypeDef](./type_defs.md#stringattributeconstraintstypetypedef) 
## UserPoolPolicyTypeOutputTypeDef

```python
# UserPoolPolicyTypeOutputTypeDef definition

class UserPoolPolicyTypeOutputTypeDef(TypedDict):
    PasswordPolicy: NotRequired[PasswordPolicyTypeTypeDef],  # (1)
    SignInPolicy: NotRequired[SignInPolicyTypeOutputTypeDef],  # (2)
```

1. See [:material-code-braces: PasswordPolicyTypeTypeDef](./type_defs.md#passwordpolicytypetypedef) 
2. See [:material-code-braces: SignInPolicyTypeOutputTypeDef](./type_defs.md#signinpolicytypeoutputtypedef) 
## AdminGetDeviceResponseTypeDef

```python
# AdminGetDeviceResponseTypeDef definition

class AdminGetDeviceResponseTypeDef(TypedDict):
    Device: DeviceTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeviceTypeTypeDef](./type_defs.md#devicetypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AdminListDevicesResponseTypeDef

```python
# AdminListDevicesResponseTypeDef definition

class AdminListDevicesResponseTypeDef(TypedDict):
    Devices: List[DeviceTypeTypeDef],  # (1)
    PaginationToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeviceTypeTypeDef](./type_defs.md#devicetypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeviceResponseTypeDef

```python
# GetDeviceResponseTypeDef definition

class GetDeviceResponseTypeDef(TypedDict):
    Device: DeviceTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeviceTypeTypeDef](./type_defs.md#devicetypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDevicesResponseTypeDef

```python
# ListDevicesResponseTypeDef definition

class ListDevicesResponseTypeDef(TypedDict):
    Devices: List[DeviceTypeTypeDef],  # (1)
    PaginationToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeviceTypeTypeDef](./type_defs.md#devicetypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AdminCreateUserResponseTypeDef

```python
# AdminCreateUserResponseTypeDef definition

class AdminCreateUserResponseTypeDef(TypedDict):
    User: UserTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeTypeDef](./type_defs.md#usertypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUsersInGroupResponseTypeDef

```python
# ListUsersInGroupResponseTypeDef definition

class ListUsersInGroupResponseTypeDef(TypedDict):
    Users: List[UserTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UserTypeTypeDef](./type_defs.md#usertypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUsersResponseTypeDef

```python
# ListUsersResponseTypeDef definition

class ListUsersResponseTypeDef(TypedDict):
    Users: List[UserTypeTypeDef],  # (1)
    PaginationToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeTypeDef](./type_defs.md#usertypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateManagedLoginBrandingResponseTypeDef

```python
# CreateManagedLoginBrandingResponseTypeDef definition

class CreateManagedLoginBrandingResponseTypeDef(TypedDict):
    ManagedLoginBranding: ManagedLoginBrandingTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ManagedLoginBrandingTypeTypeDef](./type_defs.md#managedloginbrandingtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeManagedLoginBrandingByClientResponseTypeDef

```python
# DescribeManagedLoginBrandingByClientResponseTypeDef definition

class DescribeManagedLoginBrandingByClientResponseTypeDef(TypedDict):
    ManagedLoginBranding: ManagedLoginBrandingTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ManagedLoginBrandingTypeTypeDef](./type_defs.md#managedloginbrandingtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeManagedLoginBrandingResponseTypeDef

```python
# DescribeManagedLoginBrandingResponseTypeDef definition

class DescribeManagedLoginBrandingResponseTypeDef(TypedDict):
    ManagedLoginBranding: ManagedLoginBrandingTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ManagedLoginBrandingTypeTypeDef](./type_defs.md#managedloginbrandingtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateManagedLoginBrandingResponseTypeDef

```python
# UpdateManagedLoginBrandingResponseTypeDef definition

class UpdateManagedLoginBrandingResponseTypeDef(TypedDict):
    ManagedLoginBranding: ManagedLoginBrandingTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ManagedLoginBrandingTypeTypeDef](./type_defs.md#managedloginbrandingtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateManagedLoginBrandingRequestRequestTypeDef

```python
# UpdateManagedLoginBrandingRequestRequestTypeDef definition

class UpdateManagedLoginBrandingRequestRequestTypeDef(TypedDict):
    UserPoolId: NotRequired[str],
    ManagedLoginBrandingId: NotRequired[str],
    UseCognitoProvidedValues: NotRequired[bool],
    Settings: NotRequired[Mapping[str, Any]],
    Assets: NotRequired[Sequence[AssetTypeTypeDef]],  # (1)
```

1. See [:material-code-braces: AssetTypeTypeDef](./type_defs.md#assettypetypedef) 
## AdminListUserAuthEventsResponseTypeDef

```python
# AdminListUserAuthEventsResponseTypeDef definition

class AdminListUserAuthEventsResponseTypeDef(TypedDict):
    AuthEvents: List[AuthEventTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AuthEventTypeTypeDef](./type_defs.md#autheventtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AdminInitiateAuthResponseTypeDef

```python
# AdminInitiateAuthResponseTypeDef definition

class AdminInitiateAuthResponseTypeDef(TypedDict):
    ChallengeName: ChallengeNameTypeType,  # (1)
    Session: str,
    ChallengeParameters: Dict[str, str],
    AuthenticationResult: AuthenticationResultTypeTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ChallengeNameTypeType](./literals.md#challengenametypetype) 
2. See [:material-code-braces: AuthenticationResultTypeTypeDef](./type_defs.md#authenticationresulttypetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AdminRespondToAuthChallengeResponseTypeDef

```python
# AdminRespondToAuthChallengeResponseTypeDef definition

class AdminRespondToAuthChallengeResponseTypeDef(TypedDict):
    ChallengeName: ChallengeNameTypeType,  # (1)
    Session: str,
    ChallengeParameters: Dict[str, str],
    AuthenticationResult: AuthenticationResultTypeTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ChallengeNameTypeType](./literals.md#challengenametypetype) 
2. See [:material-code-braces: AuthenticationResultTypeTypeDef](./type_defs.md#authenticationresulttypetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InitiateAuthResponseTypeDef

```python
# InitiateAuthResponseTypeDef definition

class InitiateAuthResponseTypeDef(TypedDict):
    ChallengeName: ChallengeNameTypeType,  # (1)
    Session: str,
    ChallengeParameters: Dict[str, str],
    AuthenticationResult: AuthenticationResultTypeTypeDef,  # (2)
    AvailableChallenges: List[ChallengeNameTypeType],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ChallengeNameTypeType](./literals.md#challengenametypetype) 
2. See [:material-code-braces: AuthenticationResultTypeTypeDef](./type_defs.md#authenticationresulttypetypedef) 
3. See [:material-code-brackets: ChallengeNameTypeType](./literals.md#challengenametypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RespondToAuthChallengeResponseTypeDef

```python
# RespondToAuthChallengeResponseTypeDef definition

class RespondToAuthChallengeResponseTypeDef(TypedDict):
    ChallengeName: ChallengeNameTypeType,  # (1)
    Session: str,
    ChallengeParameters: Dict[str, str],
    AuthenticationResult: AuthenticationResultTypeTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ChallengeNameTypeType](./literals.md#challengenametypetype) 
2. See [:material-code-braces: AuthenticationResultTypeTypeDef](./type_defs.md#authenticationresulttypetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AdminInitiateAuthRequestRequestTypeDef

```python
# AdminInitiateAuthRequestRequestTypeDef definition

class AdminInitiateAuthRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    ClientId: str,
    AuthFlow: AuthFlowTypeType,  # (1)
    AuthParameters: NotRequired[Mapping[str, str]],
    ClientMetadata: NotRequired[Mapping[str, str]],
    AnalyticsMetadata: NotRequired[AnalyticsMetadataTypeTypeDef],  # (2)
    ContextData: NotRequired[ContextDataTypeTypeDef],  # (3)
    Session: NotRequired[str],
```

1. See [:material-code-brackets: AuthFlowTypeType](./literals.md#authflowtypetype) 
2. See [:material-code-braces: AnalyticsMetadataTypeTypeDef](./type_defs.md#analyticsmetadatatypetypedef) 
3. See [:material-code-braces: ContextDataTypeTypeDef](./type_defs.md#contextdatatypetypedef) 
## AdminRespondToAuthChallengeRequestRequestTypeDef

```python
# AdminRespondToAuthChallengeRequestRequestTypeDef definition

class AdminRespondToAuthChallengeRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    ClientId: str,
    ChallengeName: ChallengeNameTypeType,  # (1)
    ChallengeResponses: NotRequired[Mapping[str, str]],
    Session: NotRequired[str],
    AnalyticsMetadata: NotRequired[AnalyticsMetadataTypeTypeDef],  # (2)
    ContextData: NotRequired[ContextDataTypeTypeDef],  # (3)
    ClientMetadata: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ChallengeNameTypeType](./literals.md#challengenametypetype) 
2. See [:material-code-braces: AnalyticsMetadataTypeTypeDef](./type_defs.md#analyticsmetadatatypetypedef) 
3. See [:material-code-braces: ContextDataTypeTypeDef](./type_defs.md#contextdatatypetypedef) 
## CreateResourceServerResponseTypeDef

```python
# CreateResourceServerResponseTypeDef definition

class CreateResourceServerResponseTypeDef(TypedDict):
    ResourceServer: ResourceServerTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceServerTypeTypeDef](./type_defs.md#resourceservertypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeResourceServerResponseTypeDef

```python
# DescribeResourceServerResponseTypeDef definition

class DescribeResourceServerResponseTypeDef(TypedDict):
    ResourceServer: ResourceServerTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceServerTypeTypeDef](./type_defs.md#resourceservertypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourceServersResponseTypeDef

```python
# ListResourceServersResponseTypeDef definition

class ListResourceServersResponseTypeDef(TypedDict):
    ResourceServers: List[ResourceServerTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceServerTypeTypeDef](./type_defs.md#resourceservertypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateResourceServerResponseTypeDef

```python
# UpdateResourceServerResponseTypeDef definition

class UpdateResourceServerResponseTypeDef(TypedDict):
    ResourceServer: ResourceServerTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceServerTypeTypeDef](./type_defs.md#resourceservertypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserPoolClientResponseTypeDef

```python
# CreateUserPoolClientResponseTypeDef definition

class CreateUserPoolClientResponseTypeDef(TypedDict):
    UserPoolClient: UserPoolClientTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserPoolClientTypeTypeDef](./type_defs.md#userpoolclienttypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeUserPoolClientResponseTypeDef

```python
# DescribeUserPoolClientResponseTypeDef definition

class DescribeUserPoolClientResponseTypeDef(TypedDict):
    UserPoolClient: UserPoolClientTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserPoolClientTypeTypeDef](./type_defs.md#userpoolclienttypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserPoolClientResponseTypeDef

```python
# UpdateUserPoolClientResponseTypeDef definition

class UpdateUserPoolClientResponseTypeDef(TypedDict):
    UserPoolClient: UserPoolClientTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserPoolClientTypeTypeDef](./type_defs.md#userpoolclienttypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeUserPoolDomainResponseTypeDef

```python
# DescribeUserPoolDomainResponseTypeDef definition

class DescribeUserPoolDomainResponseTypeDef(TypedDict):
    DomainDescription: DomainDescriptionTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainDescriptionTypeTypeDef](./type_defs.md#domaindescriptiontypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUserPoolMfaConfigResponseTypeDef

```python
# GetUserPoolMfaConfigResponseTypeDef definition

class GetUserPoolMfaConfigResponseTypeDef(TypedDict):
    SmsMfaConfiguration: SmsMfaConfigTypeTypeDef,  # (1)
    SoftwareTokenMfaConfiguration: SoftwareTokenMfaConfigTypeTypeDef,  # (2)
    EmailMfaConfiguration: EmailMfaConfigTypeTypeDef,  # (3)
    MfaConfiguration: UserPoolMfaTypeType,  # (4)
    WebAuthnConfiguration: WebAuthnConfigurationTypeTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: SmsMfaConfigTypeTypeDef](./type_defs.md#smsmfaconfigtypetypedef) 
2. See [:material-code-braces: SoftwareTokenMfaConfigTypeTypeDef](./type_defs.md#softwaretokenmfaconfigtypetypedef) 
3. See [:material-code-braces: EmailMfaConfigTypeTypeDef](./type_defs.md#emailmfaconfigtypetypedef) 
4. See [:material-code-brackets: UserPoolMfaTypeType](./literals.md#userpoolmfatypetype) 
5. See [:material-code-braces: WebAuthnConfigurationTypeTypeDef](./type_defs.md#webauthnconfigurationtypetypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetUserPoolMfaConfigRequestRequestTypeDef

```python
# SetUserPoolMfaConfigRequestRequestTypeDef definition

class SetUserPoolMfaConfigRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    SmsMfaConfiguration: NotRequired[SmsMfaConfigTypeTypeDef],  # (1)
    SoftwareTokenMfaConfiguration: NotRequired[SoftwareTokenMfaConfigTypeTypeDef],  # (2)
    EmailMfaConfiguration: NotRequired[EmailMfaConfigTypeTypeDef],  # (3)
    MfaConfiguration: NotRequired[UserPoolMfaTypeType],  # (4)
    WebAuthnConfiguration: NotRequired[WebAuthnConfigurationTypeTypeDef],  # (5)
```

1. See [:material-code-braces: SmsMfaConfigTypeTypeDef](./type_defs.md#smsmfaconfigtypetypedef) 
2. See [:material-code-braces: SoftwareTokenMfaConfigTypeTypeDef](./type_defs.md#softwaretokenmfaconfigtypetypedef) 
3. See [:material-code-braces: EmailMfaConfigTypeTypeDef](./type_defs.md#emailmfaconfigtypetypedef) 
4. See [:material-code-brackets: UserPoolMfaTypeType](./literals.md#userpoolmfatypetype) 
5. See [:material-code-braces: WebAuthnConfigurationTypeTypeDef](./type_defs.md#webauthnconfigurationtypetypedef) 
## SetUserPoolMfaConfigResponseTypeDef

```python
# SetUserPoolMfaConfigResponseTypeDef definition

class SetUserPoolMfaConfigResponseTypeDef(TypedDict):
    SmsMfaConfiguration: SmsMfaConfigTypeTypeDef,  # (1)
    SoftwareTokenMfaConfiguration: SoftwareTokenMfaConfigTypeTypeDef,  # (2)
    EmailMfaConfiguration: EmailMfaConfigTypeTypeDef,  # (3)
    MfaConfiguration: UserPoolMfaTypeType,  # (4)
    WebAuthnConfiguration: WebAuthnConfigurationTypeTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: SmsMfaConfigTypeTypeDef](./type_defs.md#smsmfaconfigtypetypedef) 
2. See [:material-code-braces: SoftwareTokenMfaConfigTypeTypeDef](./type_defs.md#softwaretokenmfaconfigtypetypedef) 
3. See [:material-code-braces: EmailMfaConfigTypeTypeDef](./type_defs.md#emailmfaconfigtypetypedef) 
4. See [:material-code-brackets: UserPoolMfaTypeType](./literals.md#userpoolmfatypetype) 
5. See [:material-code-braces: WebAuthnConfigurationTypeTypeDef](./type_defs.md#webauthnconfigurationtypetypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UserPoolDescriptionTypeTypeDef

```python
# UserPoolDescriptionTypeTypeDef definition

class UserPoolDescriptionTypeTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    LambdaConfig: NotRequired[LambdaConfigTypeTypeDef],  # (1)
    Status: NotRequired[StatusTypeType],  # (2)
    LastModifiedDate: NotRequired[datetime],
    CreationDate: NotRequired[datetime],
```

1. See [:material-code-braces: LambdaConfigTypeTypeDef](./type_defs.md#lambdaconfigtypetypedef) 
2. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
## LogDeliveryConfigurationTypeTypeDef

```python
# LogDeliveryConfigurationTypeTypeDef definition

class LogDeliveryConfigurationTypeTypeDef(TypedDict):
    UserPoolId: str,
    LogConfigurations: List[LogConfigurationTypeTypeDef],  # (1)
```

1. See [:material-code-braces: LogConfigurationTypeTypeDef](./type_defs.md#logconfigurationtypetypedef) 
## SetLogDeliveryConfigurationRequestRequestTypeDef

```python
# SetLogDeliveryConfigurationRequestRequestTypeDef definition

class SetLogDeliveryConfigurationRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    LogConfigurations: Sequence[LogConfigurationTypeTypeDef],  # (1)
```

1. See [:material-code-braces: LogConfigurationTypeTypeDef](./type_defs.md#logconfigurationtypetypedef) 
## AccountTakeoverRiskConfigurationTypeTypeDef

```python
# AccountTakeoverRiskConfigurationTypeTypeDef definition

class AccountTakeoverRiskConfigurationTypeTypeDef(TypedDict):
    Actions: AccountTakeoverActionsTypeTypeDef,  # (2)
    NotifyConfiguration: NotRequired[NotifyConfigurationTypeTypeDef],  # (1)
```

1. See [:material-code-braces: NotifyConfigurationTypeTypeDef](./type_defs.md#notifyconfigurationtypetypedef) 
2. See [:material-code-braces: AccountTakeoverActionsTypeTypeDef](./type_defs.md#accounttakeoveractionstypetypedef) 
## AddCustomAttributesRequestRequestTypeDef

```python
# AddCustomAttributesRequestRequestTypeDef definition

class AddCustomAttributesRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    CustomAttributes: Sequence[SchemaAttributeTypeTypeDef],  # (1)
```

1. See [:material-code-braces: SchemaAttributeTypeTypeDef](./type_defs.md#schemaattributetypetypedef) 
## UserPoolTypeTypeDef

```python
# UserPoolTypeTypeDef definition

class UserPoolTypeTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Policies: NotRequired[UserPoolPolicyTypeOutputTypeDef],  # (1)
    DeletionProtection: NotRequired[DeletionProtectionTypeType],  # (2)
    LambdaConfig: NotRequired[LambdaConfigTypeTypeDef],  # (3)
    Status: NotRequired[StatusTypeType],  # (4)
    LastModifiedDate: NotRequired[datetime],
    CreationDate: NotRequired[datetime],
    SchemaAttributes: NotRequired[List[SchemaAttributeTypeTypeDef]],  # (5)
    AutoVerifiedAttributes: NotRequired[List[VerifiedAttributeTypeType]],  # (6)
    AliasAttributes: NotRequired[List[AliasAttributeTypeType]],  # (7)
    UsernameAttributes: NotRequired[List[UsernameAttributeTypeType]],  # (8)
    SmsVerificationMessage: NotRequired[str],
    EmailVerificationMessage: NotRequired[str],
    EmailVerificationSubject: NotRequired[str],
    VerificationMessageTemplate: NotRequired[VerificationMessageTemplateTypeTypeDef],  # (9)
    SmsAuthenticationMessage: NotRequired[str],
    UserAttributeUpdateSettings: NotRequired[UserAttributeUpdateSettingsTypeOutputTypeDef],  # (10)
    MfaConfiguration: NotRequired[UserPoolMfaTypeType],  # (11)
    DeviceConfiguration: NotRequired[DeviceConfigurationTypeTypeDef],  # (12)
    EstimatedNumberOfUsers: NotRequired[int],
    EmailConfiguration: NotRequired[EmailConfigurationTypeTypeDef],  # (13)
    SmsConfiguration: NotRequired[SmsConfigurationTypeTypeDef],  # (14)
    UserPoolTags: NotRequired[Dict[str, str]],
    SmsConfigurationFailure: NotRequired[str],
    EmailConfigurationFailure: NotRequired[str],
    Domain: NotRequired[str],
    CustomDomain: NotRequired[str],
    AdminCreateUserConfig: NotRequired[AdminCreateUserConfigTypeTypeDef],  # (15)
    UserPoolAddOns: NotRequired[UserPoolAddOnsTypeTypeDef],  # (16)
    UsernameConfiguration: NotRequired[UsernameConfigurationTypeTypeDef],  # (17)
    Arn: NotRequired[str],
    AccountRecoverySetting: NotRequired[AccountRecoverySettingTypeOutputTypeDef],  # (18)
    UserPoolTier: NotRequired[UserPoolTierTypeType],  # (19)
```

1. See [:material-code-braces: UserPoolPolicyTypeOutputTypeDef](./type_defs.md#userpoolpolicytypeoutputtypedef) 
2. See [:material-code-brackets: DeletionProtectionTypeType](./literals.md#deletionprotectiontypetype) 
3. See [:material-code-braces: LambdaConfigTypeTypeDef](./type_defs.md#lambdaconfigtypetypedef) 
4. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
5. See [:material-code-braces: SchemaAttributeTypeTypeDef](./type_defs.md#schemaattributetypetypedef) 
6. See [:material-code-brackets: VerifiedAttributeTypeType](./literals.md#verifiedattributetypetype) 
7. See [:material-code-brackets: AliasAttributeTypeType](./literals.md#aliasattributetypetype) 
8. See [:material-code-brackets: UsernameAttributeTypeType](./literals.md#usernameattributetypetype) 
9. See [:material-code-braces: VerificationMessageTemplateTypeTypeDef](./type_defs.md#verificationmessagetemplatetypetypedef) 
10. See [:material-code-braces: UserAttributeUpdateSettingsTypeOutputTypeDef](./type_defs.md#userattributeupdatesettingstypeoutputtypedef) 
11. See [:material-code-brackets: UserPoolMfaTypeType](./literals.md#userpoolmfatypetype) 
12. See [:material-code-braces: DeviceConfigurationTypeTypeDef](./type_defs.md#deviceconfigurationtypetypedef) 
13. See [:material-code-braces: EmailConfigurationTypeTypeDef](./type_defs.md#emailconfigurationtypetypedef) 
14. See [:material-code-braces: SmsConfigurationTypeTypeDef](./type_defs.md#smsconfigurationtypetypedef) 
15. See [:material-code-braces: AdminCreateUserConfigTypeTypeDef](./type_defs.md#admincreateuserconfigtypetypedef) 
16. See [:material-code-braces: UserPoolAddOnsTypeTypeDef](./type_defs.md#userpooladdonstypetypedef) 
17. See [:material-code-braces: UsernameConfigurationTypeTypeDef](./type_defs.md#usernameconfigurationtypetypedef) 
18. See [:material-code-braces: AccountRecoverySettingTypeOutputTypeDef](./type_defs.md#accountrecoverysettingtypeoutputtypedef) 
19. See [:material-code-brackets: UserPoolTierTypeType](./literals.md#userpooltiertypetype) 
## UserPoolPolicyTypeTypeDef

```python
# UserPoolPolicyTypeTypeDef definition

class UserPoolPolicyTypeTypeDef(TypedDict):
    PasswordPolicy: NotRequired[PasswordPolicyTypeTypeDef],  # (1)
    SignInPolicy: NotRequired[SignInPolicyTypeUnionTypeDef],  # (2)
```

1. See [:material-code-braces: PasswordPolicyTypeTypeDef](./type_defs.md#passwordpolicytypetypedef) 
2. See [:material-code-braces: SignInPolicyTypeTypeDef](./type_defs.md#signinpolicytypetypedef) [:material-code-braces: SignInPolicyTypeOutputTypeDef](./type_defs.md#signinpolicytypeoutputtypedef) 
## CreateManagedLoginBrandingRequestRequestTypeDef

```python
# CreateManagedLoginBrandingRequestRequestTypeDef definition

class CreateManagedLoginBrandingRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    ClientId: str,
    UseCognitoProvidedValues: NotRequired[bool],
    Settings: NotRequired[Mapping[str, Any]],
    Assets: NotRequired[Sequence[AssetTypeUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: AssetTypeTypeDef](./type_defs.md#assettypetypedef) [:material-code-braces: AssetTypeOutputTypeDef](./type_defs.md#assettypeoutputtypedef) 
## ListUserPoolsResponseTypeDef

```python
# ListUserPoolsResponseTypeDef definition

class ListUserPoolsResponseTypeDef(TypedDict):
    UserPools: List[UserPoolDescriptionTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UserPoolDescriptionTypeTypeDef](./type_defs.md#userpooldescriptiontypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLogDeliveryConfigurationResponseTypeDef

```python
# GetLogDeliveryConfigurationResponseTypeDef definition

class GetLogDeliveryConfigurationResponseTypeDef(TypedDict):
    LogDeliveryConfiguration: LogDeliveryConfigurationTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LogDeliveryConfigurationTypeTypeDef](./type_defs.md#logdeliveryconfigurationtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetLogDeliveryConfigurationResponseTypeDef

```python
# SetLogDeliveryConfigurationResponseTypeDef definition

class SetLogDeliveryConfigurationResponseTypeDef(TypedDict):
    LogDeliveryConfiguration: LogDeliveryConfigurationTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LogDeliveryConfigurationTypeTypeDef](./type_defs.md#logdeliveryconfigurationtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RiskConfigurationTypeTypeDef

```python
# RiskConfigurationTypeTypeDef definition

class RiskConfigurationTypeTypeDef(TypedDict):
    UserPoolId: NotRequired[str],
    ClientId: NotRequired[str],
    CompromisedCredentialsRiskConfiguration: NotRequired[CompromisedCredentialsRiskConfigurationTypeOutputTypeDef],  # (1)
    AccountTakeoverRiskConfiguration: NotRequired[AccountTakeoverRiskConfigurationTypeTypeDef],  # (2)
    RiskExceptionConfiguration: NotRequired[RiskExceptionConfigurationTypeOutputTypeDef],  # (3)
    LastModifiedDate: NotRequired[datetime],
```

1. See [:material-code-braces: CompromisedCredentialsRiskConfigurationTypeOutputTypeDef](./type_defs.md#compromisedcredentialsriskconfigurationtypeoutputtypedef) 
2. See [:material-code-braces: AccountTakeoverRiskConfigurationTypeTypeDef](./type_defs.md#accounttakeoverriskconfigurationtypetypedef) 
3. See [:material-code-braces: RiskExceptionConfigurationTypeOutputTypeDef](./type_defs.md#riskexceptionconfigurationtypeoutputtypedef) 
## SetRiskConfigurationRequestRequestTypeDef

```python
# SetRiskConfigurationRequestRequestTypeDef definition

class SetRiskConfigurationRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    ClientId: NotRequired[str],
    CompromisedCredentialsRiskConfiguration: NotRequired[CompromisedCredentialsRiskConfigurationTypeTypeDef],  # (1)
    AccountTakeoverRiskConfiguration: NotRequired[AccountTakeoverRiskConfigurationTypeTypeDef],  # (2)
    RiskExceptionConfiguration: NotRequired[RiskExceptionConfigurationTypeTypeDef],  # (3)
```

1. See [:material-code-braces: CompromisedCredentialsRiskConfigurationTypeTypeDef](./type_defs.md#compromisedcredentialsriskconfigurationtypetypedef) 
2. See [:material-code-braces: AccountTakeoverRiskConfigurationTypeTypeDef](./type_defs.md#accounttakeoverriskconfigurationtypetypedef) 
3. See [:material-code-braces: RiskExceptionConfigurationTypeTypeDef](./type_defs.md#riskexceptionconfigurationtypetypedef) 
## CreateUserPoolResponseTypeDef

```python
# CreateUserPoolResponseTypeDef definition

class CreateUserPoolResponseTypeDef(TypedDict):
    UserPool: UserPoolTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserPoolTypeTypeDef](./type_defs.md#userpooltypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeUserPoolResponseTypeDef

```python
# DescribeUserPoolResponseTypeDef definition

class DescribeUserPoolResponseTypeDef(TypedDict):
    UserPool: UserPoolTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserPoolTypeTypeDef](./type_defs.md#userpooltypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserPoolRequestRequestTypeDef

```python
# CreateUserPoolRequestRequestTypeDef definition

class CreateUserPoolRequestRequestTypeDef(TypedDict):
    PoolName: str,
    Policies: NotRequired[UserPoolPolicyTypeTypeDef],  # (1)
    DeletionProtection: NotRequired[DeletionProtectionTypeType],  # (2)
    LambdaConfig: NotRequired[LambdaConfigTypeTypeDef],  # (3)
    AutoVerifiedAttributes: NotRequired[Sequence[VerifiedAttributeTypeType]],  # (4)
    AliasAttributes: NotRequired[Sequence[AliasAttributeTypeType]],  # (5)
    UsernameAttributes: NotRequired[Sequence[UsernameAttributeTypeType]],  # (6)
    SmsVerificationMessage: NotRequired[str],
    EmailVerificationMessage: NotRequired[str],
    EmailVerificationSubject: NotRequired[str],
    VerificationMessageTemplate: NotRequired[VerificationMessageTemplateTypeTypeDef],  # (7)
    SmsAuthenticationMessage: NotRequired[str],
    MfaConfiguration: NotRequired[UserPoolMfaTypeType],  # (8)
    UserAttributeUpdateSettings: NotRequired[UserAttributeUpdateSettingsTypeTypeDef],  # (9)
    DeviceConfiguration: NotRequired[DeviceConfigurationTypeTypeDef],  # (10)
    EmailConfiguration: NotRequired[EmailConfigurationTypeTypeDef],  # (11)
    SmsConfiguration: NotRequired[SmsConfigurationTypeTypeDef],  # (12)
    UserPoolTags: NotRequired[Mapping[str, str]],
    AdminCreateUserConfig: NotRequired[AdminCreateUserConfigTypeTypeDef],  # (13)
    Schema: NotRequired[Sequence[SchemaAttributeTypeTypeDef]],  # (14)
    UserPoolAddOns: NotRequired[UserPoolAddOnsTypeTypeDef],  # (15)
    UsernameConfiguration: NotRequired[UsernameConfigurationTypeTypeDef],  # (16)
    AccountRecoverySetting: NotRequired[AccountRecoverySettingTypeTypeDef],  # (17)
    UserPoolTier: NotRequired[UserPoolTierTypeType],  # (18)
```

1. See [:material-code-braces: UserPoolPolicyTypeTypeDef](./type_defs.md#userpoolpolicytypetypedef) 
2. See [:material-code-brackets: DeletionProtectionTypeType](./literals.md#deletionprotectiontypetype) 
3. See [:material-code-braces: LambdaConfigTypeTypeDef](./type_defs.md#lambdaconfigtypetypedef) 
4. See [:material-code-brackets: VerifiedAttributeTypeType](./literals.md#verifiedattributetypetype) 
5. See [:material-code-brackets: AliasAttributeTypeType](./literals.md#aliasattributetypetype) 
6. See [:material-code-brackets: UsernameAttributeTypeType](./literals.md#usernameattributetypetype) 
7. See [:material-code-braces: VerificationMessageTemplateTypeTypeDef](./type_defs.md#verificationmessagetemplatetypetypedef) 
8. See [:material-code-brackets: UserPoolMfaTypeType](./literals.md#userpoolmfatypetype) 
9. See [:material-code-braces: UserAttributeUpdateSettingsTypeTypeDef](./type_defs.md#userattributeupdatesettingstypetypedef) 
10. See [:material-code-braces: DeviceConfigurationTypeTypeDef](./type_defs.md#deviceconfigurationtypetypedef) 
11. See [:material-code-braces: EmailConfigurationTypeTypeDef](./type_defs.md#emailconfigurationtypetypedef) 
12. See [:material-code-braces: SmsConfigurationTypeTypeDef](./type_defs.md#smsconfigurationtypetypedef) 
13. See [:material-code-braces: AdminCreateUserConfigTypeTypeDef](./type_defs.md#admincreateuserconfigtypetypedef) 
14. See [:material-code-braces: SchemaAttributeTypeTypeDef](./type_defs.md#schemaattributetypetypedef) 
15. See [:material-code-braces: UserPoolAddOnsTypeTypeDef](./type_defs.md#userpooladdonstypetypedef) 
16. See [:material-code-braces: UsernameConfigurationTypeTypeDef](./type_defs.md#usernameconfigurationtypetypedef) 
17. See [:material-code-braces: AccountRecoverySettingTypeTypeDef](./type_defs.md#accountrecoverysettingtypetypedef) 
18. See [:material-code-brackets: UserPoolTierTypeType](./literals.md#userpooltiertypetype) 
## UpdateUserPoolRequestRequestTypeDef

```python
# UpdateUserPoolRequestRequestTypeDef definition

class UpdateUserPoolRequestRequestTypeDef(TypedDict):
    UserPoolId: str,
    Policies: NotRequired[UserPoolPolicyTypeTypeDef],  # (1)
    DeletionProtection: NotRequired[DeletionProtectionTypeType],  # (2)
    LambdaConfig: NotRequired[LambdaConfigTypeTypeDef],  # (3)
    AutoVerifiedAttributes: NotRequired[Sequence[VerifiedAttributeTypeType]],  # (4)
    SmsVerificationMessage: NotRequired[str],
    EmailVerificationMessage: NotRequired[str],
    EmailVerificationSubject: NotRequired[str],
    VerificationMessageTemplate: NotRequired[VerificationMessageTemplateTypeTypeDef],  # (5)
    SmsAuthenticationMessage: NotRequired[str],
    UserAttributeUpdateSettings: NotRequired[UserAttributeUpdateSettingsTypeTypeDef],  # (6)
    MfaConfiguration: NotRequired[UserPoolMfaTypeType],  # (7)
    DeviceConfiguration: NotRequired[DeviceConfigurationTypeTypeDef],  # (8)
    EmailConfiguration: NotRequired[EmailConfigurationTypeTypeDef],  # (9)
    SmsConfiguration: NotRequired[SmsConfigurationTypeTypeDef],  # (10)
    UserPoolTags: NotRequired[Mapping[str, str]],
    AdminCreateUserConfig: NotRequired[AdminCreateUserConfigTypeTypeDef],  # (11)
    UserPoolAddOns: NotRequired[UserPoolAddOnsTypeTypeDef],  # (12)
    AccountRecoverySetting: NotRequired[AccountRecoverySettingTypeTypeDef],  # (13)
    PoolName: NotRequired[str],
    UserPoolTier: NotRequired[UserPoolTierTypeType],  # (14)
```

1. See [:material-code-braces: UserPoolPolicyTypeTypeDef](./type_defs.md#userpoolpolicytypetypedef) 
2. See [:material-code-brackets: DeletionProtectionTypeType](./literals.md#deletionprotectiontypetype) 
3. See [:material-code-braces: LambdaConfigTypeTypeDef](./type_defs.md#lambdaconfigtypetypedef) 
4. See [:material-code-brackets: VerifiedAttributeTypeType](./literals.md#verifiedattributetypetype) 
5. See [:material-code-braces: VerificationMessageTemplateTypeTypeDef](./type_defs.md#verificationmessagetemplatetypetypedef) 
6. See [:material-code-braces: UserAttributeUpdateSettingsTypeTypeDef](./type_defs.md#userattributeupdatesettingstypetypedef) 
7. See [:material-code-brackets: UserPoolMfaTypeType](./literals.md#userpoolmfatypetype) 
8. See [:material-code-braces: DeviceConfigurationTypeTypeDef](./type_defs.md#deviceconfigurationtypetypedef) 
9. See [:material-code-braces: EmailConfigurationTypeTypeDef](./type_defs.md#emailconfigurationtypetypedef) 
10. See [:material-code-braces: SmsConfigurationTypeTypeDef](./type_defs.md#smsconfigurationtypetypedef) 
11. See [:material-code-braces: AdminCreateUserConfigTypeTypeDef](./type_defs.md#admincreateuserconfigtypetypedef) 
12. See [:material-code-braces: UserPoolAddOnsTypeTypeDef](./type_defs.md#userpooladdonstypetypedef) 
13. See [:material-code-braces: AccountRecoverySettingTypeTypeDef](./type_defs.md#accountrecoverysettingtypetypedef) 
14. See [:material-code-brackets: UserPoolTierTypeType](./literals.md#userpooltiertypetype) 
## DescribeRiskConfigurationResponseTypeDef

```python
# DescribeRiskConfigurationResponseTypeDef definition

class DescribeRiskConfigurationResponseTypeDef(TypedDict):
    RiskConfiguration: RiskConfigurationTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RiskConfigurationTypeTypeDef](./type_defs.md#riskconfigurationtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetRiskConfigurationResponseTypeDef

```python
# SetRiskConfigurationResponseTypeDef definition

class SetRiskConfigurationResponseTypeDef(TypedDict):
    RiskConfiguration: RiskConfigurationTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RiskConfigurationTypeTypeDef](./type_defs.md#riskconfigurationtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
