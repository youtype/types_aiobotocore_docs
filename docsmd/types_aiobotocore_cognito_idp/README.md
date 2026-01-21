# CognitoIdentityProvider module

> [Index](../README.md) > CognitoIdentityProvider


!!! note ""

    Auto-generated documentation for [CognitoIdentityProvider](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#cognitoidentityprovider)
    type annotations stubs module [types-aiobotocore-cognito-idp](https://pypi.org/project/types-aiobotocore-cognito-idp/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `CognitoIdentityProvider` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `CognitoIdentityProvider` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[cognito-idp]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[cognito-idp]'

# standalone installation
python -m pip install types-aiobotocore-cognito-idp
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-cognito-idp
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CognitoIdentityProviderClient

Type annotations and code completion for  `#!python session.create_client("cognito-idp")` as [CognitoIdentityProviderClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client)

```python
# CognitoIdentityProviderClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_cognito_idp.client import CognitoIdentityProviderClient


session = get_session()
async with session.create_client("cognito-idp") as client:
    client: CognitoIdentityProviderClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("cognito-idp").get_paginator("...")`.

```python
# AdminListGroupsForUserPaginator usage example

from types_aiobotocore_cognito_idp.paginator import AdminListGroupsForUserPaginator

def get_admin_list_groups_for_user_paginator() -> AdminListGroupsForUserPaginator:
    return client.get_paginator("admin_list_groups_for_user"))
```

- [AdminListGroupsForUserPaginator](./paginators.md#adminlistgroupsforuserpaginator)
- [AdminListUserAuthEventsPaginator](./paginators.md#adminlistuserautheventspaginator)
- [ListGroupsPaginator](./paginators.md#listgroupspaginator)
- [ListIdentityProvidersPaginator](./paginators.md#listidentityproviderspaginator)
- [ListResourceServersPaginator](./paginators.md#listresourceserverspaginator)
- [ListUserPoolClientsPaginator](./paginators.md#listuserpoolclientspaginator)
- [ListUserPoolsPaginator](./paginators.md#listuserpoolspaginator)
- [ListUsersInGroupPaginator](./paginators.md#listusersingrouppaginator)
- [ListUsersPaginator](./paginators.md#listuserspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccountTakeoverEventActionTypeType usage example

from types_aiobotocore_cognito_idp.literals import AccountTakeoverEventActionTypeType

def get_value() -> AccountTakeoverEventActionTypeType:
    return "BLOCK"
```

- [AccountTakeoverEventActionTypeType](./literals.md#accounttakeovereventactiontypetype)
- [AdminListGroupsForUserPaginatorName](./literals.md#adminlistgroupsforuserpaginatorname)
- [AdminListUserAuthEventsPaginatorName](./literals.md#adminlistuserautheventspaginatorname)
- [AdvancedSecurityEnabledModeTypeType](./literals.md#advancedsecurityenabledmodetypetype)
- [AdvancedSecurityModeTypeType](./literals.md#advancedsecuritymodetypetype)
- [AliasAttributeTypeType](./literals.md#aliasattributetypetype)
- [AssetCategoryTypeType](./literals.md#assetcategorytypetype)
- [AssetExtensionTypeType](./literals.md#assetextensiontypetype)
- [AttributeDataTypeType](./literals.md#attributedatatypetype)
- [AuthFactorTypeType](./literals.md#authfactortypetype)
- [AuthFlowTypeType](./literals.md#authflowtypetype)
- [ChallengeNameType](./literals.md#challengenametype)
- [ChallengeNameTypeType](./literals.md#challengenametypetype)
- [ChallengeResponseType](./literals.md#challengeresponsetype)
- [ColorSchemeModeTypeType](./literals.md#colorschememodetypetype)
- [CompromisedCredentialsEventActionTypeType](./literals.md#compromisedcredentialseventactiontypetype)
- [CustomEmailSenderLambdaVersionTypeType](./literals.md#customemailsenderlambdaversiontypetype)
- [CustomSMSSenderLambdaVersionTypeType](./literals.md#customsmssenderlambdaversiontypetype)
- [DefaultEmailOptionTypeType](./literals.md#defaultemailoptiontypetype)
- [DeletionProtectionTypeType](./literals.md#deletionprotectiontypetype)
- [DeliveryMediumTypeType](./literals.md#deliverymediumtypetype)
- [DeviceRememberedStatusTypeType](./literals.md#devicerememberedstatustypetype)
- [DomainStatusTypeType](./literals.md#domainstatustypetype)
- [EmailSendingAccountTypeType](./literals.md#emailsendingaccounttypetype)
- [EventFilterTypeType](./literals.md#eventfiltertypetype)
- [EventResponseTypeType](./literals.md#eventresponsetypetype)
- [EventSourceNameType](./literals.md#eventsourcenametype)
- [EventTypeType](./literals.md#eventtypetype)
- [ExplicitAuthFlowsTypeType](./literals.md#explicitauthflowstypetype)
- [FeatureTypeType](./literals.md#featuretypetype)
- [FeedbackValueTypeType](./literals.md#feedbackvaluetypetype)
- [IdentityProviderTypeTypeType](./literals.md#identityprovidertypetypetype)
- [ListGroupsPaginatorName](./literals.md#listgroupspaginatorname)
- [ListIdentityProvidersPaginatorName](./literals.md#listidentityproviderspaginatorname)
- [ListResourceServersPaginatorName](./literals.md#listresourceserverspaginatorname)
- [ListUserPoolClientsPaginatorName](./literals.md#listuserpoolclientspaginatorname)
- [ListUserPoolsPaginatorName](./literals.md#listuserpoolspaginatorname)
- [ListUsersInGroupPaginatorName](./literals.md#listusersingrouppaginatorname)
- [ListUsersPaginatorName](./literals.md#listuserspaginatorname)
- [LogLevelType](./literals.md#logleveltype)
- [MessageActionTypeType](./literals.md#messageactiontypetype)
- [OAuthFlowTypeType](./literals.md#oauthflowtypetype)
- [PreTokenGenerationLambdaVersionTypeType](./literals.md#pretokengenerationlambdaversiontypetype)
- [PreventUserExistenceErrorTypesType](./literals.md#preventuserexistenceerrortypestype)
- [RecoveryOptionNameTypeType](./literals.md#recoveryoptionnametypetype)
- [RiskDecisionTypeType](./literals.md#riskdecisiontypetype)
- [RiskLevelTypeType](./literals.md#riskleveltypetype)
- [StatusTypeType](./literals.md#statustypetype)
- [TermsEnforcementTypeType](./literals.md#termsenforcementtypetype)
- [TermsSourceTypeType](./literals.md#termssourcetypetype)
- [TimeUnitsTypeType](./literals.md#timeunitstypetype)
- [UserImportJobStatusTypeType](./literals.md#userimportjobstatustypetype)
- [UserPoolMfaTypeType](./literals.md#userpoolmfatypetype)
- [UserPoolTierTypeType](./literals.md#userpooltiertypetype)
- [UserStatusTypeType](./literals.md#userstatustypetype)
- [UserVerificationTypeType](./literals.md#userverificationtypetype)
- [UsernameAttributeTypeType](./literals.md#usernameattributetypetype)
- [VerifiedAttributeTypeType](./literals.md#verifiedattributetypetype)
- [VerifySoftwareTokenResponseTypeType](./literals.md#verifysoftwaretokenresponsetypetype)
- [CognitoIdentityProviderServiceName](./literals.md#cognitoidentityproviderservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [RecoveryOptionTypeTypeDef](./type_defs.md#recoveryoptiontypetypedef)
- [AccountTakeoverActionTypeTypeDef](./type_defs.md#accounttakeoveractiontypetypedef)
- [AdminAddUserToGroupRequestTypeDef](./type_defs.md#adminaddusertogrouprequesttypedef)
- [AdminConfirmSignUpRequestTypeDef](./type_defs.md#adminconfirmsignuprequesttypedef)
- [MessageTemplateTypeTypeDef](./type_defs.md#messagetemplatetypetypedef)
- [AttributeTypeTypeDef](./type_defs.md#attributetypetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AdminDeleteUserAttributesRequestTypeDef](./type_defs.md#admindeleteuserattributesrequesttypedef)
- [AdminDeleteUserRequestTypeDef](./type_defs.md#admindeleteuserrequesttypedef)
- [ProviderUserIdentifierTypeTypeDef](./type_defs.md#provideruseridentifiertypetypedef)
- [AdminDisableUserRequestTypeDef](./type_defs.md#admindisableuserrequesttypedef)
- [AdminEnableUserRequestTypeDef](./type_defs.md#adminenableuserrequesttypedef)
- [AdminForgetDeviceRequestTypeDef](./type_defs.md#adminforgetdevicerequesttypedef)
- [AdminGetDeviceRequestTypeDef](./type_defs.md#admingetdevicerequesttypedef)
- [AdminGetUserRequestTypeDef](./type_defs.md#admingetuserrequesttypedef)
- [MFAOptionTypeTypeDef](./type_defs.md#mfaoptiontypetypedef)
- [AnalyticsMetadataTypeTypeDef](./type_defs.md#analyticsmetadatatypetypedef)
- [AdminListDevicesRequestTypeDef](./type_defs.md#adminlistdevicesrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [AdminListGroupsForUserRequestTypeDef](./type_defs.md#adminlistgroupsforuserrequesttypedef)
- [GroupTypeTypeDef](./type_defs.md#grouptypetypedef)
- [AdminListUserAuthEventsRequestTypeDef](./type_defs.md#adminlistuserautheventsrequesttypedef)
- [AdminRemoveUserFromGroupRequestTypeDef](./type_defs.md#adminremoveuserfromgrouprequesttypedef)
- [AdminResetUserPasswordRequestTypeDef](./type_defs.md#adminresetuserpasswordrequesttypedef)
- [EmailMfaSettingsTypeTypeDef](./type_defs.md#emailmfasettingstypetypedef)
- [SMSMfaSettingsTypeTypeDef](./type_defs.md#smsmfasettingstypetypedef)
- [SoftwareTokenMfaSettingsTypeTypeDef](./type_defs.md#softwaretokenmfasettingstypetypedef)
- [AdminSetUserPasswordRequestTypeDef](./type_defs.md#adminsetuserpasswordrequesttypedef)
- [AdminUpdateAuthEventFeedbackRequestTypeDef](./type_defs.md#adminupdateautheventfeedbackrequesttypedef)
- [AdminUpdateDeviceStatusRequestTypeDef](./type_defs.md#adminupdatedevicestatusrequesttypedef)
- [AdminUserGlobalSignOutRequestTypeDef](./type_defs.md#adminuserglobalsignoutrequesttypedef)
- [AdvancedSecurityAdditionalFlowsTypeTypeDef](./type_defs.md#advancedsecurityadditionalflowstypetypedef)
- [AnalyticsConfigurationTypeTypeDef](./type_defs.md#analyticsconfigurationtypetypedef)
- [AssetTypeOutputTypeDef](./type_defs.md#assettypeoutputtypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [AssociateSoftwareTokenRequestTypeDef](./type_defs.md#associatesoftwaretokenrequesttypedef)
- [ChallengeResponseTypeTypeDef](./type_defs.md#challengeresponsetypetypedef)
- [EventContextDataTypeTypeDef](./type_defs.md#eventcontextdatatypetypedef)
- [EventFeedbackTypeTypeDef](./type_defs.md#eventfeedbacktypetypedef)
- [EventRiskTypeTypeDef](./type_defs.md#eventrisktypetypedef)
- [NewDeviceMetadataTypeTypeDef](./type_defs.md#newdevicemetadatatypetypedef)
- [ChangePasswordRequestTypeDef](./type_defs.md#changepasswordrequesttypedef)
- [CloudWatchLogsConfigurationTypeTypeDef](./type_defs.md#cloudwatchlogsconfigurationtypetypedef)
- [CodeDeliveryDetailsTypeTypeDef](./type_defs.md#codedeliverydetailstypetypedef)
- [CompleteWebAuthnRegistrationRequestTypeDef](./type_defs.md#completewebauthnregistrationrequesttypedef)
- [CompromisedCredentialsActionsTypeTypeDef](./type_defs.md#compromisedcredentialsactionstypetypedef)
- [DeviceSecretVerifierConfigTypeTypeDef](./type_defs.md#devicesecretverifierconfigtypetypedef)
- [UserContextDataTypeTypeDef](./type_defs.md#usercontextdatatypetypedef)
- [HttpHeaderTypeDef](./type_defs.md#httpheadertypedef)
- [CreateGroupRequestTypeDef](./type_defs.md#creategrouprequesttypedef)
- [CreateIdentityProviderRequestTypeDef](./type_defs.md#createidentityproviderrequesttypedef)
- [IdentityProviderTypeTypeDef](./type_defs.md#identityprovidertypetypedef)
- [ResourceServerScopeTypeTypeDef](./type_defs.md#resourceserverscopetypetypedef)
- [CreateTermsRequestTypeDef](./type_defs.md#createtermsrequesttypedef)
- [TermsTypeTypeDef](./type_defs.md#termstypetypedef)
- [CreateUserImportJobRequestTypeDef](./type_defs.md#createuserimportjobrequesttypedef)
- [UserImportJobTypeTypeDef](./type_defs.md#userimportjobtypetypedef)
- [RefreshTokenRotationTypeTypeDef](./type_defs.md#refreshtokenrotationtypetypedef)
- [TokenValidityUnitsTypeTypeDef](./type_defs.md#tokenvalidityunitstypetypedef)
- [CustomDomainConfigTypeTypeDef](./type_defs.md#customdomainconfigtypetypedef)
- [DeviceConfigurationTypeTypeDef](./type_defs.md#deviceconfigurationtypetypedef)
- [EmailConfigurationTypeTypeDef](./type_defs.md#emailconfigurationtypetypedef)
- [SmsConfigurationTypeTypeDef](./type_defs.md#smsconfigurationtypetypedef)
- [UsernameConfigurationTypeTypeDef](./type_defs.md#usernameconfigurationtypetypedef)
- [VerificationMessageTemplateTypeTypeDef](./type_defs.md#verificationmessagetemplatetypetypedef)
- [CustomEmailLambdaVersionConfigTypeTypeDef](./type_defs.md#customemaillambdaversionconfigtypetypedef)
- [CustomSMSLambdaVersionConfigTypeTypeDef](./type_defs.md#customsmslambdaversionconfigtypetypedef)
- [DeleteGroupRequestTypeDef](./type_defs.md#deletegrouprequesttypedef)
- [DeleteIdentityProviderRequestTypeDef](./type_defs.md#deleteidentityproviderrequesttypedef)
- [DeleteManagedLoginBrandingRequestTypeDef](./type_defs.md#deletemanagedloginbrandingrequesttypedef)
- [DeleteResourceServerRequestTypeDef](./type_defs.md#deleteresourceserverrequesttypedef)
- [DeleteTermsRequestTypeDef](./type_defs.md#deletetermsrequesttypedef)
- [DeleteUserAttributesRequestTypeDef](./type_defs.md#deleteuserattributesrequesttypedef)
- [DeleteUserPoolClientRequestTypeDef](./type_defs.md#deleteuserpoolclientrequesttypedef)
- [DeleteUserPoolDomainRequestTypeDef](./type_defs.md#deleteuserpooldomainrequesttypedef)
- [DeleteUserPoolRequestTypeDef](./type_defs.md#deleteuserpoolrequesttypedef)
- [DeleteUserRequestTypeDef](./type_defs.md#deleteuserrequesttypedef)
- [DeleteWebAuthnCredentialRequestTypeDef](./type_defs.md#deletewebauthncredentialrequesttypedef)
- [DescribeIdentityProviderRequestTypeDef](./type_defs.md#describeidentityproviderrequesttypedef)
- [DescribeManagedLoginBrandingByClientRequestTypeDef](./type_defs.md#describemanagedloginbrandingbyclientrequesttypedef)
- [DescribeManagedLoginBrandingRequestTypeDef](./type_defs.md#describemanagedloginbrandingrequesttypedef)
- [DescribeResourceServerRequestTypeDef](./type_defs.md#describeresourceserverrequesttypedef)
- [DescribeRiskConfigurationRequestTypeDef](./type_defs.md#describeriskconfigurationrequesttypedef)
- [DescribeTermsRequestTypeDef](./type_defs.md#describetermsrequesttypedef)
- [DescribeUserImportJobRequestTypeDef](./type_defs.md#describeuserimportjobrequesttypedef)
- [DescribeUserPoolClientRequestTypeDef](./type_defs.md#describeuserpoolclientrequesttypedef)
- [DescribeUserPoolDomainRequestTypeDef](./type_defs.md#describeuserpooldomainrequesttypedef)
- [DescribeUserPoolRequestTypeDef](./type_defs.md#describeuserpoolrequesttypedef)
- [EmailMfaConfigTypeTypeDef](./type_defs.md#emailmfaconfigtypetypedef)
- [FirehoseConfigurationTypeTypeDef](./type_defs.md#firehoseconfigurationtypetypedef)
- [ForgetDeviceRequestTypeDef](./type_defs.md#forgetdevicerequesttypedef)
- [GetCSVHeaderRequestTypeDef](./type_defs.md#getcsvheaderrequesttypedef)
- [GetDeviceRequestTypeDef](./type_defs.md#getdevicerequesttypedef)
- [GetGroupRequestTypeDef](./type_defs.md#getgrouprequesttypedef)
- [GetIdentityProviderByIdentifierRequestTypeDef](./type_defs.md#getidentityproviderbyidentifierrequesttypedef)
- [GetLogDeliveryConfigurationRequestTypeDef](./type_defs.md#getlogdeliveryconfigurationrequesttypedef)
- [GetSigningCertificateRequestTypeDef](./type_defs.md#getsigningcertificaterequesttypedef)
- [GetTokensFromRefreshTokenRequestTypeDef](./type_defs.md#gettokensfromrefreshtokenrequesttypedef)
- [GetUICustomizationRequestTypeDef](./type_defs.md#getuicustomizationrequesttypedef)
- [UICustomizationTypeTypeDef](./type_defs.md#uicustomizationtypetypedef)
- [GetUserAttributeVerificationCodeRequestTypeDef](./type_defs.md#getuserattributeverificationcoderequesttypedef)
- [GetUserAuthFactorsRequestTypeDef](./type_defs.md#getuserauthfactorsrequesttypedef)
- [GetUserPoolMfaConfigRequestTypeDef](./type_defs.md#getuserpoolmfaconfigrequesttypedef)
- [SoftwareTokenMfaConfigTypeTypeDef](./type_defs.md#softwaretokenmfaconfigtypetypedef)
- [WebAuthnConfigurationTypeTypeDef](./type_defs.md#webauthnconfigurationtypetypedef)
- [GetUserRequestTypeDef](./type_defs.md#getuserrequesttypedef)
- [GlobalSignOutRequestTypeDef](./type_defs.md#globalsignoutrequesttypedef)
- [PreTokenGenerationVersionConfigTypeTypeDef](./type_defs.md#pretokengenerationversionconfigtypetypedef)
- [ListDevicesRequestTypeDef](./type_defs.md#listdevicesrequesttypedef)
- [ListGroupsRequestTypeDef](./type_defs.md#listgroupsrequesttypedef)
- [ListIdentityProvidersRequestTypeDef](./type_defs.md#listidentityprovidersrequesttypedef)
- [ProviderDescriptionTypeDef](./type_defs.md#providerdescriptiontypedef)
- [ListResourceServersRequestTypeDef](./type_defs.md#listresourceserversrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [ListTermsRequestTypeDef](./type_defs.md#listtermsrequesttypedef)
- [TermsDescriptionTypeTypeDef](./type_defs.md#termsdescriptiontypetypedef)
- [ListUserImportJobsRequestTypeDef](./type_defs.md#listuserimportjobsrequesttypedef)
- [ListUserPoolClientsRequestTypeDef](./type_defs.md#listuserpoolclientsrequesttypedef)
- [UserPoolClientDescriptionTypeDef](./type_defs.md#userpoolclientdescriptiontypedef)
- [ListUserPoolsRequestTypeDef](./type_defs.md#listuserpoolsrequesttypedef)
- [ListUsersInGroupRequestTypeDef](./type_defs.md#listusersingrouprequesttypedef)
- [ListUsersRequestTypeDef](./type_defs.md#listusersrequesttypedef)
- [ListWebAuthnCredentialsRequestTypeDef](./type_defs.md#listwebauthncredentialsrequesttypedef)
- [WebAuthnCredentialDescriptionTypeDef](./type_defs.md#webauthncredentialdescriptiontypedef)
- [S3ConfigurationTypeTypeDef](./type_defs.md#s3configurationtypetypedef)
- [NotifyEmailTypeTypeDef](./type_defs.md#notifyemailtypetypedef)
- [NumberAttributeConstraintsTypeTypeDef](./type_defs.md#numberattributeconstraintstypetypedef)
- [PasswordPolicyTypeTypeDef](./type_defs.md#passwordpolicytypetypedef)
- [RevokeTokenRequestTypeDef](./type_defs.md#revoketokenrequesttypedef)
- [RiskExceptionConfigurationTypeOutputTypeDef](./type_defs.md#riskexceptionconfigurationtypeoutputtypedef)
- [RiskExceptionConfigurationTypeTypeDef](./type_defs.md#riskexceptionconfigurationtypetypedef)
- [StringAttributeConstraintsTypeTypeDef](./type_defs.md#stringattributeconstraintstypetypedef)
- [SignInPolicyTypeOutputTypeDef](./type_defs.md#signinpolicytypeoutputtypedef)
- [SignInPolicyTypeTypeDef](./type_defs.md#signinpolicytypetypedef)
- [StartUserImportJobRequestTypeDef](./type_defs.md#startuserimportjobrequesttypedef)
- [StartWebAuthnRegistrationRequestTypeDef](./type_defs.md#startwebauthnregistrationrequesttypedef)
- [StopUserImportJobRequestTypeDef](./type_defs.md#stopuserimportjobrequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateAuthEventFeedbackRequestTypeDef](./type_defs.md#updateautheventfeedbackrequesttypedef)
- [UpdateDeviceStatusRequestTypeDef](./type_defs.md#updatedevicestatusrequesttypedef)
- [UpdateGroupRequestTypeDef](./type_defs.md#updategrouprequesttypedef)
- [UpdateIdentityProviderRequestTypeDef](./type_defs.md#updateidentityproviderrequesttypedef)
- [UpdateTermsRequestTypeDef](./type_defs.md#updatetermsrequesttypedef)
- [UserAttributeUpdateSettingsTypeOutputTypeDef](./type_defs.md#userattributeupdatesettingstypeoutputtypedef)
- [UserAttributeUpdateSettingsTypeTypeDef](./type_defs.md#userattributeupdatesettingstypetypedef)
- [VerifySoftwareTokenRequestTypeDef](./type_defs.md#verifysoftwaretokenrequesttypedef)
- [VerifyUserAttributeRequestTypeDef](./type_defs.md#verifyuserattributerequesttypedef)
- [AccountRecoverySettingTypeOutputTypeDef](./type_defs.md#accountrecoverysettingtypeoutputtypedef)
- [AccountRecoverySettingTypeTypeDef](./type_defs.md#accountrecoverysettingtypetypedef)
- [AccountTakeoverActionsTypeTypeDef](./type_defs.md#accounttakeoveractionstypetypedef)
- [AdminCreateUserConfigTypeTypeDef](./type_defs.md#admincreateuserconfigtypetypedef)
- [AdminCreateUserRequestTypeDef](./type_defs.md#admincreateuserrequesttypedef)
- [AdminUpdateUserAttributesRequestTypeDef](./type_defs.md#adminupdateuserattributesrequesttypedef)
- [DeviceTypeTypeDef](./type_defs.md#devicetypetypedef)
- [UpdateUserAttributesRequestTypeDef](./type_defs.md#updateuserattributesrequesttypedef)
- [AssociateSoftwareTokenResponseTypeDef](./type_defs.md#associatesoftwaretokenresponsetypedef)
- [ConfirmDeviceResponseTypeDef](./type_defs.md#confirmdeviceresponsetypedef)
- [ConfirmSignUpResponseTypeDef](./type_defs.md#confirmsignupresponsetypedef)
- [CreateUserPoolDomainResponseTypeDef](./type_defs.md#createuserpooldomainresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetCSVHeaderResponseTypeDef](./type_defs.md#getcsvheaderresponsetypedef)
- [GetSigningCertificateResponseTypeDef](./type_defs.md#getsigningcertificateresponsetypedef)
- [GetUserAuthFactorsResponseTypeDef](./type_defs.md#getuserauthfactorsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartWebAuthnRegistrationResponseTypeDef](./type_defs.md#startwebauthnregistrationresponsetypedef)
- [UpdateUserPoolDomainResponseTypeDef](./type_defs.md#updateuserpooldomainresponsetypedef)
- [VerifySoftwareTokenResponseTypeDef](./type_defs.md#verifysoftwaretokenresponsetypedef)
- [AdminDisableProviderForUserRequestTypeDef](./type_defs.md#admindisableproviderforuserrequesttypedef)
- [AdminLinkProviderForUserRequestTypeDef](./type_defs.md#adminlinkproviderforuserrequesttypedef)
- [AdminGetUserResponseTypeDef](./type_defs.md#admingetuserresponsetypedef)
- [AdminSetUserSettingsRequestTypeDef](./type_defs.md#adminsetusersettingsrequesttypedef)
- [GetUserResponseTypeDef](./type_defs.md#getuserresponsetypedef)
- [SetUserSettingsRequestTypeDef](./type_defs.md#setusersettingsrequesttypedef)
- [UserTypeTypeDef](./type_defs.md#usertypetypedef)
- [AdminListGroupsForUserRequestPaginateTypeDef](./type_defs.md#adminlistgroupsforuserrequestpaginatetypedef)
- [AdminListUserAuthEventsRequestPaginateTypeDef](./type_defs.md#adminlistuserautheventsrequestpaginatetypedef)
- [ListGroupsRequestPaginateTypeDef](./type_defs.md#listgroupsrequestpaginatetypedef)
- [ListIdentityProvidersRequestPaginateTypeDef](./type_defs.md#listidentityprovidersrequestpaginatetypedef)
- [ListResourceServersRequestPaginateTypeDef](./type_defs.md#listresourceserversrequestpaginatetypedef)
- [ListUserPoolClientsRequestPaginateTypeDef](./type_defs.md#listuserpoolclientsrequestpaginatetypedef)
- [ListUserPoolsRequestPaginateTypeDef](./type_defs.md#listuserpoolsrequestpaginatetypedef)
- [ListUsersInGroupRequestPaginateTypeDef](./type_defs.md#listusersingrouprequestpaginatetypedef)
- [ListUsersRequestPaginateTypeDef](./type_defs.md#listusersrequestpaginatetypedef)
- [AdminListGroupsForUserResponseTypeDef](./type_defs.md#adminlistgroupsforuserresponsetypedef)
- [CreateGroupResponseTypeDef](./type_defs.md#creategroupresponsetypedef)
- [GetGroupResponseTypeDef](./type_defs.md#getgroupresponsetypedef)
- [ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef)
- [UpdateGroupResponseTypeDef](./type_defs.md#updategroupresponsetypedef)
- [AdminSetUserMFAPreferenceRequestTypeDef](./type_defs.md#adminsetusermfapreferencerequesttypedef)
- [SetUserMFAPreferenceRequestTypeDef](./type_defs.md#setusermfapreferencerequesttypedef)
- [UserPoolAddOnsTypeTypeDef](./type_defs.md#userpooladdonstypetypedef)
- [ManagedLoginBrandingTypeTypeDef](./type_defs.md#managedloginbrandingtypetypedef)
- [AssetTypeTypeDef](./type_defs.md#assettypetypedef)
- [SetUICustomizationRequestTypeDef](./type_defs.md#setuicustomizationrequesttypedef)
- [AuthEventTypeTypeDef](./type_defs.md#autheventtypetypedef)
- [AuthenticationResultTypeTypeDef](./type_defs.md#authenticationresulttypetypedef)
- [ForgotPasswordResponseTypeDef](./type_defs.md#forgotpasswordresponsetypedef)
- [GetUserAttributeVerificationCodeResponseTypeDef](./type_defs.md#getuserattributeverificationcoderesponsetypedef)
- [ResendConfirmationCodeResponseTypeDef](./type_defs.md#resendconfirmationcoderesponsetypedef)
- [SignUpResponseTypeDef](./type_defs.md#signupresponsetypedef)
- [UpdateUserAttributesResponseTypeDef](./type_defs.md#updateuserattributesresponsetypedef)
- [CompromisedCredentialsRiskConfigurationTypeOutputTypeDef](./type_defs.md#compromisedcredentialsriskconfigurationtypeoutputtypedef)
- [CompromisedCredentialsRiskConfigurationTypeTypeDef](./type_defs.md#compromisedcredentialsriskconfigurationtypetypedef)
- [ConfirmDeviceRequestTypeDef](./type_defs.md#confirmdevicerequesttypedef)
- [ConfirmForgotPasswordRequestTypeDef](./type_defs.md#confirmforgotpasswordrequesttypedef)
- [ConfirmSignUpRequestTypeDef](./type_defs.md#confirmsignuprequesttypedef)
- [ForgotPasswordRequestTypeDef](./type_defs.md#forgotpasswordrequesttypedef)
- [InitiateAuthRequestTypeDef](./type_defs.md#initiateauthrequesttypedef)
- [ResendConfirmationCodeRequestTypeDef](./type_defs.md#resendconfirmationcoderequesttypedef)
- [RespondToAuthChallengeRequestTypeDef](./type_defs.md#respondtoauthchallengerequesttypedef)
- [SignUpRequestTypeDef](./type_defs.md#signuprequesttypedef)
- [ContextDataTypeTypeDef](./type_defs.md#contextdatatypetypedef)
- [CreateIdentityProviderResponseTypeDef](./type_defs.md#createidentityproviderresponsetypedef)
- [DescribeIdentityProviderResponseTypeDef](./type_defs.md#describeidentityproviderresponsetypedef)
- [GetIdentityProviderByIdentifierResponseTypeDef](./type_defs.md#getidentityproviderbyidentifierresponsetypedef)
- [UpdateIdentityProviderResponseTypeDef](./type_defs.md#updateidentityproviderresponsetypedef)
- [CreateResourceServerRequestTypeDef](./type_defs.md#createresourceserverrequesttypedef)
- [ResourceServerTypeTypeDef](./type_defs.md#resourceservertypetypedef)
- [UpdateResourceServerRequestTypeDef](./type_defs.md#updateresourceserverrequesttypedef)
- [CreateTermsResponseTypeDef](./type_defs.md#createtermsresponsetypedef)
- [DescribeTermsResponseTypeDef](./type_defs.md#describetermsresponsetypedef)
- [UpdateTermsResponseTypeDef](./type_defs.md#updatetermsresponsetypedef)
- [CreateUserImportJobResponseTypeDef](./type_defs.md#createuserimportjobresponsetypedef)
- [DescribeUserImportJobResponseTypeDef](./type_defs.md#describeuserimportjobresponsetypedef)
- [ListUserImportJobsResponseTypeDef](./type_defs.md#listuserimportjobsresponsetypedef)
- [StartUserImportJobResponseTypeDef](./type_defs.md#startuserimportjobresponsetypedef)
- [StopUserImportJobResponseTypeDef](./type_defs.md#stopuserimportjobresponsetypedef)
- [CreateUserPoolClientRequestTypeDef](./type_defs.md#createuserpoolclientrequesttypedef)
- [UpdateUserPoolClientRequestTypeDef](./type_defs.md#updateuserpoolclientrequesttypedef)
- [UserPoolClientTypeTypeDef](./type_defs.md#userpoolclienttypetypedef)
- [CreateUserPoolDomainRequestTypeDef](./type_defs.md#createuserpooldomainrequesttypedef)
- [DomainDescriptionTypeTypeDef](./type_defs.md#domaindescriptiontypetypedef)
- [UpdateUserPoolDomainRequestTypeDef](./type_defs.md#updateuserpooldomainrequesttypedef)
- [SmsMfaConfigTypeTypeDef](./type_defs.md#smsmfaconfigtypetypedef)
- [GetUICustomizationResponseTypeDef](./type_defs.md#getuicustomizationresponsetypedef)
- [SetUICustomizationResponseTypeDef](./type_defs.md#setuicustomizationresponsetypedef)
- [LambdaConfigTypeTypeDef](./type_defs.md#lambdaconfigtypetypedef)
- [ListIdentityProvidersResponseTypeDef](./type_defs.md#listidentityprovidersresponsetypedef)
- [ListTermsResponseTypeDef](./type_defs.md#listtermsresponsetypedef)
- [ListUserPoolClientsResponseTypeDef](./type_defs.md#listuserpoolclientsresponsetypedef)
- [ListWebAuthnCredentialsResponseTypeDef](./type_defs.md#listwebauthncredentialsresponsetypedef)
- [LogConfigurationTypeTypeDef](./type_defs.md#logconfigurationtypetypedef)
- [NotifyConfigurationTypeTypeDef](./type_defs.md#notifyconfigurationtypetypedef)
- [RiskExceptionConfigurationTypeUnionTypeDef](./type_defs.md#riskexceptionconfigurationtypeuniontypedef)
- [SchemaAttributeTypeTypeDef](./type_defs.md#schemaattributetypetypedef)
- [UserPoolPolicyTypeOutputTypeDef](./type_defs.md#userpoolpolicytypeoutputtypedef)
- [UserPoolPolicyTypeTypeDef](./type_defs.md#userpoolpolicytypetypedef)
- [UserAttributeUpdateSettingsTypeUnionTypeDef](./type_defs.md#userattributeupdatesettingstypeuniontypedef)
- [AccountRecoverySettingTypeUnionTypeDef](./type_defs.md#accountrecoverysettingtypeuniontypedef)
- [AdminGetDeviceResponseTypeDef](./type_defs.md#admingetdeviceresponsetypedef)
- [AdminListDevicesResponseTypeDef](./type_defs.md#adminlistdevicesresponsetypedef)
- [GetDeviceResponseTypeDef](./type_defs.md#getdeviceresponsetypedef)
- [ListDevicesResponseTypeDef](./type_defs.md#listdevicesresponsetypedef)
- [AdminCreateUserResponseTypeDef](./type_defs.md#admincreateuserresponsetypedef)
- [ListUsersInGroupResponseTypeDef](./type_defs.md#listusersingroupresponsetypedef)
- [ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef)
- [CreateManagedLoginBrandingResponseTypeDef](./type_defs.md#createmanagedloginbrandingresponsetypedef)
- [DescribeManagedLoginBrandingByClientResponseTypeDef](./type_defs.md#describemanagedloginbrandingbyclientresponsetypedef)
- [DescribeManagedLoginBrandingResponseTypeDef](./type_defs.md#describemanagedloginbrandingresponsetypedef)
- [UpdateManagedLoginBrandingResponseTypeDef](./type_defs.md#updatemanagedloginbrandingresponsetypedef)
- [AssetTypeUnionTypeDef](./type_defs.md#assettypeuniontypedef)
- [AdminListUserAuthEventsResponseTypeDef](./type_defs.md#adminlistuserautheventsresponsetypedef)
- [AdminInitiateAuthResponseTypeDef](./type_defs.md#admininitiateauthresponsetypedef)
- [AdminRespondToAuthChallengeResponseTypeDef](./type_defs.md#adminrespondtoauthchallengeresponsetypedef)
- [GetTokensFromRefreshTokenResponseTypeDef](./type_defs.md#gettokensfromrefreshtokenresponsetypedef)
- [InitiateAuthResponseTypeDef](./type_defs.md#initiateauthresponsetypedef)
- [RespondToAuthChallengeResponseTypeDef](./type_defs.md#respondtoauthchallengeresponsetypedef)
- [CompromisedCredentialsRiskConfigurationTypeUnionTypeDef](./type_defs.md#compromisedcredentialsriskconfigurationtypeuniontypedef)
- [AdminInitiateAuthRequestTypeDef](./type_defs.md#admininitiateauthrequesttypedef)
- [AdminRespondToAuthChallengeRequestTypeDef](./type_defs.md#adminrespondtoauthchallengerequesttypedef)
- [CreateResourceServerResponseTypeDef](./type_defs.md#createresourceserverresponsetypedef)
- [DescribeResourceServerResponseTypeDef](./type_defs.md#describeresourceserverresponsetypedef)
- [ListResourceServersResponseTypeDef](./type_defs.md#listresourceserversresponsetypedef)
- [UpdateResourceServerResponseTypeDef](./type_defs.md#updateresourceserverresponsetypedef)
- [CreateUserPoolClientResponseTypeDef](./type_defs.md#createuserpoolclientresponsetypedef)
- [DescribeUserPoolClientResponseTypeDef](./type_defs.md#describeuserpoolclientresponsetypedef)
- [UpdateUserPoolClientResponseTypeDef](./type_defs.md#updateuserpoolclientresponsetypedef)
- [DescribeUserPoolDomainResponseTypeDef](./type_defs.md#describeuserpooldomainresponsetypedef)
- [GetUserPoolMfaConfigResponseTypeDef](./type_defs.md#getuserpoolmfaconfigresponsetypedef)
- [SetUserPoolMfaConfigRequestTypeDef](./type_defs.md#setuserpoolmfaconfigrequesttypedef)
- [SetUserPoolMfaConfigResponseTypeDef](./type_defs.md#setuserpoolmfaconfigresponsetypedef)
- [UserPoolDescriptionTypeTypeDef](./type_defs.md#userpooldescriptiontypetypedef)
- [LogDeliveryConfigurationTypeTypeDef](./type_defs.md#logdeliveryconfigurationtypetypedef)
- [SetLogDeliveryConfigurationRequestTypeDef](./type_defs.md#setlogdeliveryconfigurationrequesttypedef)
- [AccountTakeoverRiskConfigurationTypeTypeDef](./type_defs.md#accounttakeoverriskconfigurationtypetypedef)
- [AddCustomAttributesRequestTypeDef](./type_defs.md#addcustomattributesrequesttypedef)
- [UserPoolTypeTypeDef](./type_defs.md#userpooltypetypedef)
- [UserPoolPolicyTypeUnionTypeDef](./type_defs.md#userpoolpolicytypeuniontypedef)
- [CreateManagedLoginBrandingRequestTypeDef](./type_defs.md#createmanagedloginbrandingrequesttypedef)
- [UpdateManagedLoginBrandingRequestTypeDef](./type_defs.md#updatemanagedloginbrandingrequesttypedef)
- [ListUserPoolsResponseTypeDef](./type_defs.md#listuserpoolsresponsetypedef)
- [GetLogDeliveryConfigurationResponseTypeDef](./type_defs.md#getlogdeliveryconfigurationresponsetypedef)
- [SetLogDeliveryConfigurationResponseTypeDef](./type_defs.md#setlogdeliveryconfigurationresponsetypedef)
- [RiskConfigurationTypeTypeDef](./type_defs.md#riskconfigurationtypetypedef)
- [SetRiskConfigurationRequestTypeDef](./type_defs.md#setriskconfigurationrequesttypedef)
- [CreateUserPoolResponseTypeDef](./type_defs.md#createuserpoolresponsetypedef)
- [DescribeUserPoolResponseTypeDef](./type_defs.md#describeuserpoolresponsetypedef)
- [CreateUserPoolRequestTypeDef](./type_defs.md#createuserpoolrequesttypedef)
- [UpdateUserPoolRequestTypeDef](./type_defs.md#updateuserpoolrequesttypedef)
- [DescribeRiskConfigurationResponseTypeDef](./type_defs.md#describeriskconfigurationresponsetypedef)
- [SetRiskConfigurationResponseTypeDef](./type_defs.md#setriskconfigurationresponsetypedef)

