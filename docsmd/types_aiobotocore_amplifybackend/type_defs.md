# Type definitions

> [Index](../README.md) > [AmplifyBackend](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AmplifyBackend](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
    type annotations stubs module [types-aiobotocore-amplifybackend](https://pypi.org/project/types-aiobotocore-amplifybackend/).



## BackendAPIAppSyncAuthSettingsTypeDef

```python
# BackendAPIAppSyncAuthSettingsTypeDef definition

class BackendAPIAppSyncAuthSettingsTypeDef(TypedDict):
    CognitoUserPoolId: NotRequired[str],
    Description: NotRequired[str],
    ExpirationTime: NotRequired[float],
    OpenIDAuthTTL: NotRequired[str],
    OpenIDClientId: NotRequired[str],
    OpenIDIatTTL: NotRequired[str],
    OpenIDIssueURL: NotRequired[str],
    OpenIDProviderName: NotRequired[str],
```

## BackendAPIConflictResolutionTypeDef

```python
# BackendAPIConflictResolutionTypeDef definition

class BackendAPIConflictResolutionTypeDef(TypedDict):
    ResolutionStrategy: NotRequired[ResolutionStrategyType],  # (1)
```

1. See [:material-code-brackets: ResolutionStrategyType](./literals.md#resolutionstrategytype) 
## BackendAuthAppleProviderConfigTypeDef

```python
# BackendAuthAppleProviderConfigTypeDef definition

class BackendAuthAppleProviderConfigTypeDef(TypedDict):
    ClientId: NotRequired[str],
    KeyId: NotRequired[str],
    PrivateKey: NotRequired[str],
    TeamId: NotRequired[str],
```

## BackendAuthSocialProviderConfigTypeDef

```python
# BackendAuthSocialProviderConfigTypeDef definition

class BackendAuthSocialProviderConfigTypeDef(TypedDict):
    ClientId: NotRequired[str],
    ClientSecret: NotRequired[str],
```

## BackendJobRespObjTypeDef

```python
# BackendJobRespObjTypeDef definition

class BackendJobRespObjTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    CreateTime: NotRequired[str],
    Error: NotRequired[str],
    JobId: NotRequired[str],
    Operation: NotRequired[str],
    Status: NotRequired[str],
    UpdateTime: NotRequired[str],
```

## BackendStoragePermissionsTypeDef

```python
# BackendStoragePermissionsTypeDef definition

class BackendStoragePermissionsTypeDef(TypedDict):
    Authenticated: Sequence[AuthenticatedElementType],  # (1)
    UnAuthenticated: NotRequired[Sequence[UnAuthenticatedElementType]],  # (2)
```

1. See [:material-code-brackets: AuthenticatedElementType](./literals.md#authenticatedelementtype) 
2. See [:material-code-brackets: UnAuthenticatedElementType](./literals.md#unauthenticatedelementtype) 
## CloneBackendRequestRequestTypeDef

```python
# CloneBackendRequestRequestTypeDef definition

class CloneBackendRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    TargetEnvironmentName: str,
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

## EmailSettingsTypeDef

```python
# EmailSettingsTypeDef definition

class EmailSettingsTypeDef(TypedDict):
    EmailMessage: NotRequired[str],
    EmailSubject: NotRequired[str],
```

## SmsSettingsTypeDef

```python
# SmsSettingsTypeDef definition

class SmsSettingsTypeDef(TypedDict):
    SmsMessage: NotRequired[str],
```

## CreateBackendAuthIdentityPoolConfigTypeDef

```python
# CreateBackendAuthIdentityPoolConfigTypeDef definition

class CreateBackendAuthIdentityPoolConfigTypeDef(TypedDict):
    IdentityPoolName: str,
    UnauthenticatedLogin: bool,
```

## SettingsTypeDef

```python
# SettingsTypeDef definition

class SettingsTypeDef(TypedDict):
    MfaTypes: NotRequired[Sequence[MfaTypesElementType]],  # (1)
    SmsMessage: NotRequired[str],
```

1. See [:material-code-brackets: MfaTypesElementType](./literals.md#mfatypeselementtype) 
## CreateBackendAuthPasswordPolicyConfigTypeDef

```python
# CreateBackendAuthPasswordPolicyConfigTypeDef definition

class CreateBackendAuthPasswordPolicyConfigTypeDef(TypedDict):
    MinimumLength: float,
    AdditionalConstraints: NotRequired[Sequence[AdditionalConstraintsElementType]],  # (1)
```

1. See [:material-code-brackets: AdditionalConstraintsElementType](./literals.md#additionalconstraintselementtype) 
## CreateBackendConfigRequestRequestTypeDef

```python
# CreateBackendConfigRequestRequestTypeDef definition

class CreateBackendConfigRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendManagerAppId: NotRequired[str],
```

## CreateBackendRequestRequestTypeDef

```python
# CreateBackendRequestRequestTypeDef definition

class CreateBackendRequestRequestTypeDef(TypedDict):
    AppId: str,
    AppName: str,
    BackendEnvironmentName: str,
    ResourceConfig: NotRequired[Mapping[str, Any]],
    ResourceName: NotRequired[str],
```

## CreateTokenRequestRequestTypeDef

```python
# CreateTokenRequestRequestTypeDef definition

class CreateTokenRequestRequestTypeDef(TypedDict):
    AppId: str,
```

## DeleteBackendAuthRequestRequestTypeDef

```python
# DeleteBackendAuthRequestRequestTypeDef definition

class DeleteBackendAuthRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    ResourceName: str,
```

## DeleteBackendRequestRequestTypeDef

```python
# DeleteBackendRequestRequestTypeDef definition

class DeleteBackendRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
```

## DeleteBackendStorageRequestRequestTypeDef

```python
# DeleteBackendStorageRequestRequestTypeDef definition

class DeleteBackendStorageRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    ResourceName: str,
    ServiceName: ServiceNameType,  # (1)
```

1. See [:material-code-brackets: ServiceNameType](./literals.md#servicenametype) 
## DeleteTokenRequestRequestTypeDef

```python
# DeleteTokenRequestRequestTypeDef definition

class DeleteTokenRequestRequestTypeDef(TypedDict):
    AppId: str,
    SessionId: str,
```

## GenerateBackendAPIModelsRequestRequestTypeDef

```python
# GenerateBackendAPIModelsRequestRequestTypeDef definition

class GenerateBackendAPIModelsRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    ResourceName: str,
```

## GetBackendAPIModelsRequestRequestTypeDef

```python
# GetBackendAPIModelsRequestRequestTypeDef definition

class GetBackendAPIModelsRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    ResourceName: str,
```

## GetBackendAuthRequestRequestTypeDef

```python
# GetBackendAuthRequestRequestTypeDef definition

class GetBackendAuthRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    ResourceName: str,
```

## GetBackendJobRequestRequestTypeDef

```python
# GetBackendJobRequestRequestTypeDef definition

class GetBackendJobRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    JobId: str,
```

## GetBackendRequestRequestTypeDef

```python
# GetBackendRequestRequestTypeDef definition

class GetBackendRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: NotRequired[str],
```

## GetBackendStorageRequestRequestTypeDef

```python
# GetBackendStorageRequestRequestTypeDef definition

class GetBackendStorageRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    ResourceName: str,
```

## GetTokenRequestRequestTypeDef

```python
# GetTokenRequestRequestTypeDef definition

class GetTokenRequestRequestTypeDef(TypedDict):
    AppId: str,
    SessionId: str,
```

## ImportBackendAuthRequestRequestTypeDef

```python
# ImportBackendAuthRequestRequestTypeDef definition

class ImportBackendAuthRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    NativeClientId: str,
    UserPoolId: str,
    WebClientId: str,
    IdentityPoolId: NotRequired[str],
```

## ImportBackendStorageRequestRequestTypeDef

```python
# ImportBackendStorageRequestRequestTypeDef definition

class ImportBackendStorageRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    ServiceName: ServiceNameType,  # (1)
    BucketName: NotRequired[str],
```

1. See [:material-code-brackets: ServiceNameType](./literals.md#servicenametype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListBackendJobsRequestRequestTypeDef

```python
# ListBackendJobsRequestRequestTypeDef definition

class ListBackendJobsRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    JobId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Operation: NotRequired[str],
    Status: NotRequired[str],
```

## ListS3BucketsRequestRequestTypeDef

```python
# ListS3BucketsRequestRequestTypeDef definition

class ListS3BucketsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
```

## S3BucketInfoTypeDef

```python
# S3BucketInfoTypeDef definition

class S3BucketInfoTypeDef(TypedDict):
    CreationDate: NotRequired[str],
    Name: NotRequired[str],
```

## LoginAuthConfigReqObjTypeDef

```python
# LoginAuthConfigReqObjTypeDef definition

class LoginAuthConfigReqObjTypeDef(TypedDict):
    AwsCognitoIdentityPoolId: NotRequired[str],
    AwsCognitoRegion: NotRequired[str],
    AwsUserPoolsId: NotRequired[str],
    AwsUserPoolsWebClientId: NotRequired[str],
```

## RemoveAllBackendsRequestRequestTypeDef

```python
# RemoveAllBackendsRequestRequestTypeDef definition

class RemoveAllBackendsRequestRequestTypeDef(TypedDict):
    AppId: str,
    CleanAmplifyApp: NotRequired[bool],
```

## RemoveBackendConfigRequestRequestTypeDef

```python
# RemoveBackendConfigRequestRequestTypeDef definition

class RemoveBackendConfigRequestRequestTypeDef(TypedDict):
    AppId: str,
```

## UpdateBackendAuthIdentityPoolConfigTypeDef

```python
# UpdateBackendAuthIdentityPoolConfigTypeDef definition

class UpdateBackendAuthIdentityPoolConfigTypeDef(TypedDict):
    UnauthenticatedLogin: NotRequired[bool],
```

## UpdateBackendAuthPasswordPolicyConfigTypeDef

```python
# UpdateBackendAuthPasswordPolicyConfigTypeDef definition

class UpdateBackendAuthPasswordPolicyConfigTypeDef(TypedDict):
    AdditionalConstraints: NotRequired[Sequence[AdditionalConstraintsElementType]],  # (1)
    MinimumLength: NotRequired[float],
```

1. See [:material-code-brackets: AdditionalConstraintsElementType](./literals.md#additionalconstraintselementtype) 
## UpdateBackendJobRequestRequestTypeDef

```python
# UpdateBackendJobRequestRequestTypeDef definition

class UpdateBackendJobRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    JobId: str,
    Operation: NotRequired[str],
    Status: NotRequired[str],
```

## BackendAPIAuthTypeTypeDef

```python
# BackendAPIAuthTypeTypeDef definition

class BackendAPIAuthTypeTypeDef(TypedDict):
    Mode: NotRequired[ModeType],  # (1)
    Settings: NotRequired[BackendAPIAppSyncAuthSettingsTypeDef],  # (2)
```

1. See [:material-code-brackets: ModeType](./literals.md#modetype) 
2. See [:material-code-braces: BackendAPIAppSyncAuthSettingsTypeDef](./type_defs.md#backendapiappsyncauthsettingstypedef) 
## SocialProviderSettingsTypeDef

```python
# SocialProviderSettingsTypeDef definition

class SocialProviderSettingsTypeDef(TypedDict):
    Facebook: NotRequired[BackendAuthSocialProviderConfigTypeDef],  # (1)
    Google: NotRequired[BackendAuthSocialProviderConfigTypeDef],  # (1)
    LoginWithAmazon: NotRequired[BackendAuthSocialProviderConfigTypeDef],  # (1)
    SignInWithApple: NotRequired[BackendAuthAppleProviderConfigTypeDef],  # (4)
```

1. See [:material-code-braces: BackendAuthSocialProviderConfigTypeDef](./type_defs.md#backendauthsocialproviderconfigtypedef) 
2. See [:material-code-braces: BackendAuthSocialProviderConfigTypeDef](./type_defs.md#backendauthsocialproviderconfigtypedef) 
3. See [:material-code-braces: BackendAuthSocialProviderConfigTypeDef](./type_defs.md#backendauthsocialproviderconfigtypedef) 
4. See [:material-code-braces: BackendAuthAppleProviderConfigTypeDef](./type_defs.md#backendauthappleproviderconfigtypedef) 
## CreateBackendStorageResourceConfigTypeDef

```python
# CreateBackendStorageResourceConfigTypeDef definition

class CreateBackendStorageResourceConfigTypeDef(TypedDict):
    Permissions: BackendStoragePermissionsTypeDef,  # (1)
    ServiceName: ServiceNameType,  # (2)
    BucketName: NotRequired[str],
```

1. See [:material-code-braces: BackendStoragePermissionsTypeDef](./type_defs.md#backendstoragepermissionstypedef) 
2. See [:material-code-brackets: ServiceNameType](./literals.md#servicenametype) 
## GetBackendStorageResourceConfigTypeDef

```python
# GetBackendStorageResourceConfigTypeDef definition

class GetBackendStorageResourceConfigTypeDef(TypedDict):
    Imported: bool,
    ServiceName: ServiceNameType,  # (2)
    BucketName: NotRequired[str],
    Permissions: NotRequired[BackendStoragePermissionsTypeDef],  # (1)
```

1. See [:material-code-braces: BackendStoragePermissionsTypeDef](./type_defs.md#backendstoragepermissionstypedef) 
2. See [:material-code-brackets: ServiceNameType](./literals.md#servicenametype) 
## UpdateBackendStorageResourceConfigTypeDef

```python
# UpdateBackendStorageResourceConfigTypeDef definition

class UpdateBackendStorageResourceConfigTypeDef(TypedDict):
    Permissions: BackendStoragePermissionsTypeDef,  # (1)
    ServiceName: ServiceNameType,  # (2)
```

1. See [:material-code-braces: BackendStoragePermissionsTypeDef](./type_defs.md#backendstoragepermissionstypedef) 
2. See [:material-code-brackets: ServiceNameType](./literals.md#servicenametype) 
## CloneBackendResponseTypeDef

```python
# CloneBackendResponseTypeDef definition

class CloneBackendResponseTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    Error: str,
    JobId: str,
    Operation: str,
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBackendAPIResponseTypeDef

```python
# CreateBackendAPIResponseTypeDef definition

class CreateBackendAPIResponseTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    Error: str,
    JobId: str,
    Operation: str,
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBackendAuthResponseTypeDef

```python
# CreateBackendAuthResponseTypeDef definition

class CreateBackendAuthResponseTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    Error: str,
    JobId: str,
    Operation: str,
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBackendConfigResponseTypeDef

```python
# CreateBackendConfigResponseTypeDef definition

class CreateBackendConfigResponseTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    JobId: str,
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBackendResponseTypeDef

```python
# CreateBackendResponseTypeDef definition

class CreateBackendResponseTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    Error: str,
    JobId: str,
    Operation: str,
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBackendStorageResponseTypeDef

```python
# CreateBackendStorageResponseTypeDef definition

class CreateBackendStorageResponseTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    JobId: str,
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTokenResponseTypeDef

```python
# CreateTokenResponseTypeDef definition

class CreateTokenResponseTypeDef(TypedDict):
    AppId: str,
    ChallengeCode: str,
    SessionId: str,
    Ttl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBackendAPIResponseTypeDef

```python
# DeleteBackendAPIResponseTypeDef definition

class DeleteBackendAPIResponseTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    Error: str,
    JobId: str,
    Operation: str,
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBackendAuthResponseTypeDef

```python
# DeleteBackendAuthResponseTypeDef definition

class DeleteBackendAuthResponseTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    Error: str,
    JobId: str,
    Operation: str,
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBackendResponseTypeDef

```python
# DeleteBackendResponseTypeDef definition

class DeleteBackendResponseTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    Error: str,
    JobId: str,
    Operation: str,
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBackendStorageResponseTypeDef

```python
# DeleteBackendStorageResponseTypeDef definition

class DeleteBackendStorageResponseTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    JobId: str,
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTokenResponseTypeDef

```python
# DeleteTokenResponseTypeDef definition

class DeleteTokenResponseTypeDef(TypedDict):
    IsSuccess: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GenerateBackendAPIModelsResponseTypeDef

```python
# GenerateBackendAPIModelsResponseTypeDef definition

class GenerateBackendAPIModelsResponseTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    Error: str,
    JobId: str,
    Operation: str,
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBackendAPIModelsResponseTypeDef

```python
# GetBackendAPIModelsResponseTypeDef definition

class GetBackendAPIModelsResponseTypeDef(TypedDict):
    Models: str,
    Status: StatusType,  # (1)
    ModelIntrospectionSchema: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBackendJobResponseTypeDef

```python
# GetBackendJobResponseTypeDef definition

class GetBackendJobResponseTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    CreateTime: str,
    Error: str,
    JobId: str,
    Operation: str,
    Status: str,
    UpdateTime: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBackendResponseTypeDef

```python
# GetBackendResponseTypeDef definition

class GetBackendResponseTypeDef(TypedDict):
    AmplifyFeatureFlags: str,
    AmplifyMetaConfig: str,
    AppId: str,
    AppName: str,
    BackendEnvironmentList: List[str],
    BackendEnvironmentName: str,
    Error: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTokenResponseTypeDef

```python
# GetTokenResponseTypeDef definition

class GetTokenResponseTypeDef(TypedDict):
    AppId: str,
    ChallengeCode: str,
    SessionId: str,
    Ttl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportBackendAuthResponseTypeDef

```python
# ImportBackendAuthResponseTypeDef definition

class ImportBackendAuthResponseTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    Error: str,
    JobId: str,
    Operation: str,
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportBackendStorageResponseTypeDef

```python
# ImportBackendStorageResponseTypeDef definition

class ImportBackendStorageResponseTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    JobId: str,
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBackendJobsResponseTypeDef

```python
# ListBackendJobsResponseTypeDef definition

class ListBackendJobsResponseTypeDef(TypedDict):
    Jobs: List[BackendJobRespObjTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackendJobRespObjTypeDef](./type_defs.md#backendjobrespobjtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveAllBackendsResponseTypeDef

```python
# RemoveAllBackendsResponseTypeDef definition

class RemoveAllBackendsResponseTypeDef(TypedDict):
    AppId: str,
    Error: str,
    JobId: str,
    Operation: str,
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveBackendConfigResponseTypeDef

```python
# RemoveBackendConfigResponseTypeDef definition

class RemoveBackendConfigResponseTypeDef(TypedDict):
    Error: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBackendAPIResponseTypeDef

```python
# UpdateBackendAPIResponseTypeDef definition

class UpdateBackendAPIResponseTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    Error: str,
    JobId: str,
    Operation: str,
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBackendAuthResponseTypeDef

```python
# UpdateBackendAuthResponseTypeDef definition

class UpdateBackendAuthResponseTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    Error: str,
    JobId: str,
    Operation: str,
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBackendJobResponseTypeDef

```python
# UpdateBackendJobResponseTypeDef definition

class UpdateBackendJobResponseTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    CreateTime: str,
    Error: str,
    JobId: str,
    Operation: str,
    Status: str,
    UpdateTime: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBackendStorageResponseTypeDef

```python
# UpdateBackendStorageResponseTypeDef definition

class UpdateBackendStorageResponseTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    JobId: str,
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBackendAuthForgotPasswordConfigTypeDef

```python
# CreateBackendAuthForgotPasswordConfigTypeDef definition

class CreateBackendAuthForgotPasswordConfigTypeDef(TypedDict):
    DeliveryMethod: DeliveryMethodType,  # (1)
    EmailSettings: NotRequired[EmailSettingsTypeDef],  # (2)
    SmsSettings: NotRequired[SmsSettingsTypeDef],  # (3)
```

1. See [:material-code-brackets: DeliveryMethodType](./literals.md#deliverymethodtype) 
2. See [:material-code-braces: EmailSettingsTypeDef](./type_defs.md#emailsettingstypedef) 
3. See [:material-code-braces: SmsSettingsTypeDef](./type_defs.md#smssettingstypedef) 
## CreateBackendAuthVerificationMessageConfigTypeDef

```python
# CreateBackendAuthVerificationMessageConfigTypeDef definition

class CreateBackendAuthVerificationMessageConfigTypeDef(TypedDict):
    DeliveryMethod: DeliveryMethodType,  # (1)
    EmailSettings: NotRequired[EmailSettingsTypeDef],  # (2)
    SmsSettings: NotRequired[SmsSettingsTypeDef],  # (3)
```

1. See [:material-code-brackets: DeliveryMethodType](./literals.md#deliverymethodtype) 
2. See [:material-code-braces: EmailSettingsTypeDef](./type_defs.md#emailsettingstypedef) 
3. See [:material-code-braces: SmsSettingsTypeDef](./type_defs.md#smssettingstypedef) 
## UpdateBackendAuthForgotPasswordConfigTypeDef

```python
# UpdateBackendAuthForgotPasswordConfigTypeDef definition

class UpdateBackendAuthForgotPasswordConfigTypeDef(TypedDict):
    DeliveryMethod: NotRequired[DeliveryMethodType],  # (1)
    EmailSettings: NotRequired[EmailSettingsTypeDef],  # (2)
    SmsSettings: NotRequired[SmsSettingsTypeDef],  # (3)
```

1. See [:material-code-brackets: DeliveryMethodType](./literals.md#deliverymethodtype) 
2. See [:material-code-braces: EmailSettingsTypeDef](./type_defs.md#emailsettingstypedef) 
3. See [:material-code-braces: SmsSettingsTypeDef](./type_defs.md#smssettingstypedef) 
## UpdateBackendAuthVerificationMessageConfigTypeDef

```python
# UpdateBackendAuthVerificationMessageConfigTypeDef definition

class UpdateBackendAuthVerificationMessageConfigTypeDef(TypedDict):
    DeliveryMethod: DeliveryMethodType,  # (1)
    EmailSettings: NotRequired[EmailSettingsTypeDef],  # (2)
    SmsSettings: NotRequired[SmsSettingsTypeDef],  # (3)
```

1. See [:material-code-brackets: DeliveryMethodType](./literals.md#deliverymethodtype) 
2. See [:material-code-braces: EmailSettingsTypeDef](./type_defs.md#emailsettingstypedef) 
3. See [:material-code-braces: SmsSettingsTypeDef](./type_defs.md#smssettingstypedef) 
## CreateBackendAuthMFAConfigTypeDef

```python
# CreateBackendAuthMFAConfigTypeDef definition

class CreateBackendAuthMFAConfigTypeDef(TypedDict):
    MFAMode: MFAModeType,  # (1)
    Settings: NotRequired[SettingsTypeDef],  # (2)
```

1. See [:material-code-brackets: MFAModeType](./literals.md#mfamodetype) 
2. See [:material-code-braces: SettingsTypeDef](./type_defs.md#settingstypedef) 
## UpdateBackendAuthMFAConfigTypeDef

```python
# UpdateBackendAuthMFAConfigTypeDef definition

class UpdateBackendAuthMFAConfigTypeDef(TypedDict):
    MFAMode: NotRequired[MFAModeType],  # (1)
    Settings: NotRequired[SettingsTypeDef],  # (2)
```

1. See [:material-code-brackets: MFAModeType](./literals.md#mfamodetype) 
2. See [:material-code-braces: SettingsTypeDef](./type_defs.md#settingstypedef) 
## ListBackendJobsRequestListBackendJobsPaginateTypeDef

```python
# ListBackendJobsRequestListBackendJobsPaginateTypeDef definition

class ListBackendJobsRequestListBackendJobsPaginateTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    JobId: NotRequired[str],
    Operation: NotRequired[str],
    Status: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListS3BucketsResponseTypeDef

```python
# ListS3BucketsResponseTypeDef definition

class ListS3BucketsResponseTypeDef(TypedDict):
    Buckets: List[S3BucketInfoTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: S3BucketInfoTypeDef](./type_defs.md#s3bucketinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBackendConfigRequestRequestTypeDef

```python
# UpdateBackendConfigRequestRequestTypeDef definition

class UpdateBackendConfigRequestRequestTypeDef(TypedDict):
    AppId: str,
    LoginAuthConfig: NotRequired[LoginAuthConfigReqObjTypeDef],  # (1)
```

1. See [:material-code-braces: LoginAuthConfigReqObjTypeDef](./type_defs.md#loginauthconfigreqobjtypedef) 
## UpdateBackendConfigResponseTypeDef

```python
# UpdateBackendConfigResponseTypeDef definition

class UpdateBackendConfigResponseTypeDef(TypedDict):
    AppId: str,
    BackendManagerAppId: str,
    Error: str,
    LoginAuthConfig: LoginAuthConfigReqObjTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoginAuthConfigReqObjTypeDef](./type_defs.md#loginauthconfigreqobjtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BackendAPIResourceConfigTypeDef

```python
# BackendAPIResourceConfigTypeDef definition

class BackendAPIResourceConfigTypeDef(TypedDict):
    AdditionalAuthTypes: NotRequired[Sequence[BackendAPIAuthTypeTypeDef]],  # (1)
    ApiName: NotRequired[str],
    ConflictResolution: NotRequired[BackendAPIConflictResolutionTypeDef],  # (2)
    DefaultAuthType: NotRequired[BackendAPIAuthTypeTypeDef],  # (3)
    Service: NotRequired[str],
    TransformSchema: NotRequired[str],
```

1. See [:material-code-braces: BackendAPIAuthTypeTypeDef](./type_defs.md#backendapiauthtypetypedef) 
2. See [:material-code-braces: BackendAPIConflictResolutionTypeDef](./type_defs.md#backendapiconflictresolutiontypedef) 
3. See [:material-code-braces: BackendAPIAuthTypeTypeDef](./type_defs.md#backendapiauthtypetypedef) 
## CreateBackendAuthOAuthConfigTypeDef

```python
# CreateBackendAuthOAuthConfigTypeDef definition

class CreateBackendAuthOAuthConfigTypeDef(TypedDict):
    OAuthGrantType: OAuthGrantTypeType,  # (1)
    OAuthScopes: Sequence[OAuthScopesElementType],  # (2)
    RedirectSignInURIs: Sequence[str],
    RedirectSignOutURIs: Sequence[str],
    DomainPrefix: NotRequired[str],
    SocialProviderSettings: NotRequired[SocialProviderSettingsTypeDef],  # (3)
```

1. See [:material-code-brackets: OAuthGrantTypeType](./literals.md#oauthgranttypetype) 
2. See [:material-code-brackets: OAuthScopesElementType](./literals.md#oauthscopeselementtype) 
3. See [:material-code-braces: SocialProviderSettingsTypeDef](./type_defs.md#socialprovidersettingstypedef) 
## UpdateBackendAuthOAuthConfigTypeDef

```python
# UpdateBackendAuthOAuthConfigTypeDef definition

class UpdateBackendAuthOAuthConfigTypeDef(TypedDict):
    DomainPrefix: NotRequired[str],
    OAuthGrantType: NotRequired[OAuthGrantTypeType],  # (1)
    OAuthScopes: NotRequired[Sequence[OAuthScopesElementType]],  # (2)
    RedirectSignInURIs: NotRequired[Sequence[str]],
    RedirectSignOutURIs: NotRequired[Sequence[str]],
    SocialProviderSettings: NotRequired[SocialProviderSettingsTypeDef],  # (3)
```

1. See [:material-code-brackets: OAuthGrantTypeType](./literals.md#oauthgranttypetype) 
2. See [:material-code-brackets: OAuthScopesElementType](./literals.md#oauthscopeselementtype) 
3. See [:material-code-braces: SocialProviderSettingsTypeDef](./type_defs.md#socialprovidersettingstypedef) 
## CreateBackendStorageRequestRequestTypeDef

```python
# CreateBackendStorageRequestRequestTypeDef definition

class CreateBackendStorageRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    ResourceConfig: CreateBackendStorageResourceConfigTypeDef,  # (1)
    ResourceName: str,
```

1. See [:material-code-braces: CreateBackendStorageResourceConfigTypeDef](./type_defs.md#createbackendstorageresourceconfigtypedef) 
## GetBackendStorageResponseTypeDef

```python
# GetBackendStorageResponseTypeDef definition

class GetBackendStorageResponseTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    ResourceConfig: GetBackendStorageResourceConfigTypeDef,  # (1)
    ResourceName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GetBackendStorageResourceConfigTypeDef](./type_defs.md#getbackendstorageresourceconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBackendStorageRequestRequestTypeDef

```python
# UpdateBackendStorageRequestRequestTypeDef definition

class UpdateBackendStorageRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    ResourceConfig: UpdateBackendStorageResourceConfigTypeDef,  # (1)
    ResourceName: str,
```

1. See [:material-code-braces: UpdateBackendStorageResourceConfigTypeDef](./type_defs.md#updatebackendstorageresourceconfigtypedef) 
## CreateBackendAPIRequestRequestTypeDef

```python
# CreateBackendAPIRequestRequestTypeDef definition

class CreateBackendAPIRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    ResourceConfig: BackendAPIResourceConfigTypeDef,  # (1)
    ResourceName: str,
```

1. See [:material-code-braces: BackendAPIResourceConfigTypeDef](./type_defs.md#backendapiresourceconfigtypedef) 
## DeleteBackendAPIRequestRequestTypeDef

```python
# DeleteBackendAPIRequestRequestTypeDef definition

class DeleteBackendAPIRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    ResourceName: str,
    ResourceConfig: NotRequired[BackendAPIResourceConfigTypeDef],  # (1)
```

1. See [:material-code-braces: BackendAPIResourceConfigTypeDef](./type_defs.md#backendapiresourceconfigtypedef) 
## GetBackendAPIRequestRequestTypeDef

```python
# GetBackendAPIRequestRequestTypeDef definition

class GetBackendAPIRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    ResourceName: str,
    ResourceConfig: NotRequired[BackendAPIResourceConfigTypeDef],  # (1)
```

1. See [:material-code-braces: BackendAPIResourceConfigTypeDef](./type_defs.md#backendapiresourceconfigtypedef) 
## GetBackendAPIResponseTypeDef

```python
# GetBackendAPIResponseTypeDef definition

class GetBackendAPIResponseTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    Error: str,
    ResourceConfig: BackendAPIResourceConfigTypeDef,  # (1)
    ResourceName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackendAPIResourceConfigTypeDef](./type_defs.md#backendapiresourceconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBackendAPIRequestRequestTypeDef

```python
# UpdateBackendAPIRequestRequestTypeDef definition

class UpdateBackendAPIRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    ResourceName: str,
    ResourceConfig: NotRequired[BackendAPIResourceConfigTypeDef],  # (1)
```

1. See [:material-code-braces: BackendAPIResourceConfigTypeDef](./type_defs.md#backendapiresourceconfigtypedef) 
## CreateBackendAuthUserPoolConfigTypeDef

```python
# CreateBackendAuthUserPoolConfigTypeDef definition

class CreateBackendAuthUserPoolConfigTypeDef(TypedDict):
    RequiredSignUpAttributes: Sequence[RequiredSignUpAttributesElementType],  # (5)
    SignInMethod: SignInMethodType,  # (6)
    UserPoolName: str,
    ForgotPassword: NotRequired[CreateBackendAuthForgotPasswordConfigTypeDef],  # (1)
    Mfa: NotRequired[CreateBackendAuthMFAConfigTypeDef],  # (2)
    OAuth: NotRequired[CreateBackendAuthOAuthConfigTypeDef],  # (3)
    PasswordPolicy: NotRequired[CreateBackendAuthPasswordPolicyConfigTypeDef],  # (4)
    VerificationMessage: NotRequired[CreateBackendAuthVerificationMessageConfigTypeDef],  # (7)
```

1. See [:material-code-braces: CreateBackendAuthForgotPasswordConfigTypeDef](./type_defs.md#createbackendauthforgotpasswordconfigtypedef) 
2. See [:material-code-braces: CreateBackendAuthMFAConfigTypeDef](./type_defs.md#createbackendauthmfaconfigtypedef) 
3. See [:material-code-braces: CreateBackendAuthOAuthConfigTypeDef](./type_defs.md#createbackendauthoauthconfigtypedef) 
4. See [:material-code-braces: CreateBackendAuthPasswordPolicyConfigTypeDef](./type_defs.md#createbackendauthpasswordpolicyconfigtypedef) 
5. See [:material-code-brackets: RequiredSignUpAttributesElementType](./literals.md#requiredsignupattributeselementtype) 
6. See [:material-code-brackets: SignInMethodType](./literals.md#signinmethodtype) 
7. See [:material-code-braces: CreateBackendAuthVerificationMessageConfigTypeDef](./type_defs.md#createbackendauthverificationmessageconfigtypedef) 
## UpdateBackendAuthUserPoolConfigTypeDef

```python
# UpdateBackendAuthUserPoolConfigTypeDef definition

class UpdateBackendAuthUserPoolConfigTypeDef(TypedDict):
    ForgotPassword: NotRequired[UpdateBackendAuthForgotPasswordConfigTypeDef],  # (1)
    Mfa: NotRequired[UpdateBackendAuthMFAConfigTypeDef],  # (2)
    OAuth: NotRequired[UpdateBackendAuthOAuthConfigTypeDef],  # (3)
    PasswordPolicy: NotRequired[UpdateBackendAuthPasswordPolicyConfigTypeDef],  # (4)
    VerificationMessage: NotRequired[UpdateBackendAuthVerificationMessageConfigTypeDef],  # (5)
```

1. See [:material-code-braces: UpdateBackendAuthForgotPasswordConfigTypeDef](./type_defs.md#updatebackendauthforgotpasswordconfigtypedef) 
2. See [:material-code-braces: UpdateBackendAuthMFAConfigTypeDef](./type_defs.md#updatebackendauthmfaconfigtypedef) 
3. See [:material-code-braces: UpdateBackendAuthOAuthConfigTypeDef](./type_defs.md#updatebackendauthoauthconfigtypedef) 
4. See [:material-code-braces: UpdateBackendAuthPasswordPolicyConfigTypeDef](./type_defs.md#updatebackendauthpasswordpolicyconfigtypedef) 
5. See [:material-code-braces: UpdateBackendAuthVerificationMessageConfigTypeDef](./type_defs.md#updatebackendauthverificationmessageconfigtypedef) 
## CreateBackendAuthResourceConfigTypeDef

```python
# CreateBackendAuthResourceConfigTypeDef definition

class CreateBackendAuthResourceConfigTypeDef(TypedDict):
    AuthResources: AuthResourcesType,  # (1)
    Service: ServiceType,  # (3)
    UserPoolConfigs: CreateBackendAuthUserPoolConfigTypeDef,  # (4)
    IdentityPoolConfigs: NotRequired[CreateBackendAuthIdentityPoolConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AuthResourcesType](./literals.md#authresourcestype) 
2. See [:material-code-braces: CreateBackendAuthIdentityPoolConfigTypeDef](./type_defs.md#createbackendauthidentitypoolconfigtypedef) 
3. See [:material-code-brackets: ServiceType](./literals.md#servicetype) 
4. See [:material-code-braces: CreateBackendAuthUserPoolConfigTypeDef](./type_defs.md#createbackendauthuserpoolconfigtypedef) 
## UpdateBackendAuthResourceConfigTypeDef

```python
# UpdateBackendAuthResourceConfigTypeDef definition

class UpdateBackendAuthResourceConfigTypeDef(TypedDict):
    AuthResources: AuthResourcesType,  # (1)
    Service: ServiceType,  # (3)
    UserPoolConfigs: UpdateBackendAuthUserPoolConfigTypeDef,  # (4)
    IdentityPoolConfigs: NotRequired[UpdateBackendAuthIdentityPoolConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AuthResourcesType](./literals.md#authresourcestype) 
2. See [:material-code-braces: UpdateBackendAuthIdentityPoolConfigTypeDef](./type_defs.md#updatebackendauthidentitypoolconfigtypedef) 
3. See [:material-code-brackets: ServiceType](./literals.md#servicetype) 
4. See [:material-code-braces: UpdateBackendAuthUserPoolConfigTypeDef](./type_defs.md#updatebackendauthuserpoolconfigtypedef) 
## CreateBackendAuthRequestRequestTypeDef

```python
# CreateBackendAuthRequestRequestTypeDef definition

class CreateBackendAuthRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    ResourceConfig: CreateBackendAuthResourceConfigTypeDef,  # (1)
    ResourceName: str,
```

1. See [:material-code-braces: CreateBackendAuthResourceConfigTypeDef](./type_defs.md#createbackendauthresourceconfigtypedef) 
## GetBackendAuthResponseTypeDef

```python
# GetBackendAuthResponseTypeDef definition

class GetBackendAuthResponseTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    Error: str,
    ResourceConfig: CreateBackendAuthResourceConfigTypeDef,  # (1)
    ResourceName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CreateBackendAuthResourceConfigTypeDef](./type_defs.md#createbackendauthresourceconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBackendAuthRequestRequestTypeDef

```python
# UpdateBackendAuthRequestRequestTypeDef definition

class UpdateBackendAuthRequestRequestTypeDef(TypedDict):
    AppId: str,
    BackendEnvironmentName: str,
    ResourceConfig: UpdateBackendAuthResourceConfigTypeDef,  # (1)
    ResourceName: str,
```

1. See [:material-code-braces: UpdateBackendAuthResourceConfigTypeDef](./type_defs.md#updatebackendauthresourceconfigtypedef) 
