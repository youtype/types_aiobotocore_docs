# Type definitions

> [Index](../README.md) > [CognitoIdentity](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CognitoIdentity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#cognitoidentity)
    type annotations stubs module [types-aiobotocore-cognito-identity](https://pypi.org/project/types-aiobotocore-cognito-identity/).

## RulesConfigurationTypeUnionTypeDef

```python
# RulesConfigurationTypeUnionTypeDef definition

RulesConfigurationTypeUnionTypeDef = Union[
    RulesConfigurationTypeTypeDef,  # (1)
    RulesConfigurationTypeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RulesConfigurationTypeTypeDef](./type_defs.md#rulesconfigurationtypetypedef) 
2. See [:material-code-braces: RulesConfigurationTypeOutputTypeDef](./type_defs.md#rulesconfigurationtypeoutputtypedef) 

## RoleMappingUnionTypeDef

```python
# RoleMappingUnionTypeDef definition

RoleMappingUnionTypeDef = Union[
    RoleMappingTypeDef,  # (1)
    RoleMappingOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RoleMappingTypeDef](./type_defs.md#rolemappingtypedef) 
2. See [:material-code-braces: RoleMappingOutputTypeDef](./type_defs.md#rolemappingoutputtypedef) 



## CognitoIdentityProviderTypeDef

```python
# CognitoIdentityProviderTypeDef definition

class CognitoIdentityProviderTypeDef(TypedDict):
    ProviderName: NotRequired[str],
    ClientId: NotRequired[str],
    ServerSideTokenCheck: NotRequired[bool],
```

## CredentialsTypeDef

```python
# CredentialsTypeDef definition

class CredentialsTypeDef(TypedDict):
    AccessKeyId: NotRequired[str],
    SecretKey: NotRequired[str],
    SessionToken: NotRequired[str],
    Expiration: NotRequired[datetime],
```

## DeleteIdentitiesInputRequestTypeDef

```python
# DeleteIdentitiesInputRequestTypeDef definition

class DeleteIdentitiesInputRequestTypeDef(TypedDict):
    IdentityIdsToDelete: Sequence[str],
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

## UnprocessedIdentityIdTypeDef

```python
# UnprocessedIdentityIdTypeDef definition

class UnprocessedIdentityIdTypeDef(TypedDict):
    IdentityId: NotRequired[str],
    ErrorCode: NotRequired[ErrorCodeType],  # (1)
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## DeleteIdentityPoolInputRequestTypeDef

```python
# DeleteIdentityPoolInputRequestTypeDef definition

class DeleteIdentityPoolInputRequestTypeDef(TypedDict):
    IdentityPoolId: str,
```

## DescribeIdentityInputRequestTypeDef

```python
# DescribeIdentityInputRequestTypeDef definition

class DescribeIdentityInputRequestTypeDef(TypedDict):
    IdentityId: str,
```

## DescribeIdentityPoolInputRequestTypeDef

```python
# DescribeIdentityPoolInputRequestTypeDef definition

class DescribeIdentityPoolInputRequestTypeDef(TypedDict):
    IdentityPoolId: str,
```

## GetCredentialsForIdentityInputRequestTypeDef

```python
# GetCredentialsForIdentityInputRequestTypeDef definition

class GetCredentialsForIdentityInputRequestTypeDef(TypedDict):
    IdentityId: str,
    Logins: NotRequired[Mapping[str, str]],
    CustomRoleArn: NotRequired[str],
```

## GetIdInputRequestTypeDef

```python
# GetIdInputRequestTypeDef definition

class GetIdInputRequestTypeDef(TypedDict):
    IdentityPoolId: str,
    AccountId: NotRequired[str],
    Logins: NotRequired[Mapping[str, str]],
```

## GetIdentityPoolRolesInputRequestTypeDef

```python
# GetIdentityPoolRolesInputRequestTypeDef definition

class GetIdentityPoolRolesInputRequestTypeDef(TypedDict):
    IdentityPoolId: str,
```

## GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef

```python
# GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef definition

class GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef(TypedDict):
    IdentityPoolId: str,
    Logins: Mapping[str, str],
    IdentityId: NotRequired[str],
    PrincipalTags: NotRequired[Mapping[str, str]],
    TokenDuration: NotRequired[int],
```

## GetOpenIdTokenInputRequestTypeDef

```python
# GetOpenIdTokenInputRequestTypeDef definition

class GetOpenIdTokenInputRequestTypeDef(TypedDict):
    IdentityId: str,
    Logins: NotRequired[Mapping[str, str]],
```

## GetPrincipalTagAttributeMapInputRequestTypeDef

```python
# GetPrincipalTagAttributeMapInputRequestTypeDef definition

class GetPrincipalTagAttributeMapInputRequestTypeDef(TypedDict):
    IdentityPoolId: str,
    IdentityProviderName: str,
```

## IdentityDescriptionTypeDef

```python
# IdentityDescriptionTypeDef definition

class IdentityDescriptionTypeDef(TypedDict):
    IdentityId: NotRequired[str],
    Logins: NotRequired[List[str]],
    CreationDate: NotRequired[datetime],
    LastModifiedDate: NotRequired[datetime],
```

## IdentityPoolShortDescriptionTypeDef

```python
# IdentityPoolShortDescriptionTypeDef definition

class IdentityPoolShortDescriptionTypeDef(TypedDict):
    IdentityPoolId: NotRequired[str],
    IdentityPoolName: NotRequired[str],
```

## ListIdentitiesInputRequestTypeDef

```python
# ListIdentitiesInputRequestTypeDef definition

class ListIdentitiesInputRequestTypeDef(TypedDict):
    IdentityPoolId: str,
    MaxResults: int,
    NextToken: NotRequired[str],
    HideDisabled: NotRequired[bool],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListIdentityPoolsInputRequestTypeDef

```python
# ListIdentityPoolsInputRequestTypeDef definition

class ListIdentityPoolsInputRequestTypeDef(TypedDict):
    MaxResults: int,
    NextToken: NotRequired[str],
```

## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## LookupDeveloperIdentityInputRequestTypeDef

```python
# LookupDeveloperIdentityInputRequestTypeDef definition

class LookupDeveloperIdentityInputRequestTypeDef(TypedDict):
    IdentityPoolId: str,
    IdentityId: NotRequired[str],
    DeveloperUserIdentifier: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## MappingRuleTypeDef

```python
# MappingRuleTypeDef definition

class MappingRuleTypeDef(TypedDict):
    Claim: str,
    MatchType: MappingRuleMatchTypeType,  # (1)
    Value: str,
    RoleARN: str,
```

1. See [:material-code-brackets: MappingRuleMatchTypeType](./literals.md#mappingrulematchtypetype) 
## MergeDeveloperIdentitiesInputRequestTypeDef

```python
# MergeDeveloperIdentitiesInputRequestTypeDef definition

class MergeDeveloperIdentitiesInputRequestTypeDef(TypedDict):
    SourceUserIdentifier: str,
    DestinationUserIdentifier: str,
    DeveloperProviderName: str,
    IdentityPoolId: str,
```

## SetPrincipalTagAttributeMapInputRequestTypeDef

```python
# SetPrincipalTagAttributeMapInputRequestTypeDef definition

class SetPrincipalTagAttributeMapInputRequestTypeDef(TypedDict):
    IdentityPoolId: str,
    IdentityProviderName: str,
    UseDefaults: NotRequired[bool],
    PrincipalTags: NotRequired[Mapping[str, str]],
```

## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UnlinkDeveloperIdentityInputRequestTypeDef

```python
# UnlinkDeveloperIdentityInputRequestTypeDef definition

class UnlinkDeveloperIdentityInputRequestTypeDef(TypedDict):
    IdentityId: str,
    IdentityPoolId: str,
    DeveloperProviderName: str,
    DeveloperUserIdentifier: str,
```

## UnlinkIdentityInputRequestTypeDef

```python
# UnlinkIdentityInputRequestTypeDef definition

class UnlinkIdentityInputRequestTypeDef(TypedDict):
    IdentityId: str,
    Logins: Mapping[str, str],
    LoginsToRemove: Sequence[str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## CreateIdentityPoolInputRequestTypeDef

```python
# CreateIdentityPoolInputRequestTypeDef definition

class CreateIdentityPoolInputRequestTypeDef(TypedDict):
    IdentityPoolName: str,
    AllowUnauthenticatedIdentities: bool,
    AllowClassicFlow: NotRequired[bool],
    SupportedLoginProviders: NotRequired[Mapping[str, str]],
    DeveloperProviderName: NotRequired[str],
    OpenIdConnectProviderARNs: NotRequired[Sequence[str]],
    CognitoIdentityProviders: NotRequired[Sequence[CognitoIdentityProviderTypeDef]],  # (1)
    SamlProviderARNs: NotRequired[Sequence[str]],
    IdentityPoolTags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: CognitoIdentityProviderTypeDef](./type_defs.md#cognitoidentityprovidertypedef) 
## IdentityPoolRequestTypeDef

```python
# IdentityPoolRequestTypeDef definition

class IdentityPoolRequestTypeDef(TypedDict):
    IdentityPoolId: str,
    IdentityPoolName: str,
    AllowUnauthenticatedIdentities: bool,
    AllowClassicFlow: NotRequired[bool],
    SupportedLoginProviders: NotRequired[Mapping[str, str]],
    DeveloperProviderName: NotRequired[str],
    OpenIdConnectProviderARNs: NotRequired[Sequence[str]],
    CognitoIdentityProviders: NotRequired[Sequence[CognitoIdentityProviderTypeDef]],  # (1)
    SamlProviderARNs: NotRequired[Sequence[str]],
    IdentityPoolTags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: CognitoIdentityProviderTypeDef](./type_defs.md#cognitoidentityprovidertypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCredentialsForIdentityResponseTypeDef

```python
# GetCredentialsForIdentityResponseTypeDef definition

class GetCredentialsForIdentityResponseTypeDef(TypedDict):
    IdentityId: str,
    Credentials: CredentialsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CredentialsTypeDef](./type_defs.md#credentialstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIdResponseTypeDef

```python
# GetIdResponseTypeDef definition

class GetIdResponseTypeDef(TypedDict):
    IdentityId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOpenIdTokenForDeveloperIdentityResponseTypeDef

```python
# GetOpenIdTokenForDeveloperIdentityResponseTypeDef definition

class GetOpenIdTokenForDeveloperIdentityResponseTypeDef(TypedDict):
    IdentityId: str,
    Token: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOpenIdTokenResponseTypeDef

```python
# GetOpenIdTokenResponseTypeDef definition

class GetOpenIdTokenResponseTypeDef(TypedDict):
    IdentityId: str,
    Token: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPrincipalTagAttributeMapResponseTypeDef

```python
# GetPrincipalTagAttributeMapResponseTypeDef definition

class GetPrincipalTagAttributeMapResponseTypeDef(TypedDict):
    IdentityPoolId: str,
    IdentityProviderName: str,
    UseDefaults: bool,
    PrincipalTags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IdentityDescriptionResponseTypeDef

```python
# IdentityDescriptionResponseTypeDef definition

class IdentityDescriptionResponseTypeDef(TypedDict):
    IdentityId: str,
    Logins: List[str],
    CreationDate: datetime,
    LastModifiedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IdentityPoolTypeDef

```python
# IdentityPoolTypeDef definition

class IdentityPoolTypeDef(TypedDict):
    IdentityPoolId: str,
    IdentityPoolName: str,
    AllowUnauthenticatedIdentities: bool,
    AllowClassicFlow: bool,
    SupportedLoginProviders: Dict[str, str],
    DeveloperProviderName: str,
    OpenIdConnectProviderARNs: List[str],
    CognitoIdentityProviders: List[CognitoIdentityProviderTypeDef],  # (1)
    SamlProviderARNs: List[str],
    IdentityPoolTags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CognitoIdentityProviderTypeDef](./type_defs.md#cognitoidentityprovidertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LookupDeveloperIdentityResponseTypeDef

```python
# LookupDeveloperIdentityResponseTypeDef definition

class LookupDeveloperIdentityResponseTypeDef(TypedDict):
    IdentityId: str,
    DeveloperUserIdentifierList: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MergeDeveloperIdentitiesResponseTypeDef

```python
# MergeDeveloperIdentitiesResponseTypeDef definition

class MergeDeveloperIdentitiesResponseTypeDef(TypedDict):
    IdentityId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetPrincipalTagAttributeMapResponseTypeDef

```python
# SetPrincipalTagAttributeMapResponseTypeDef definition

class SetPrincipalTagAttributeMapResponseTypeDef(TypedDict):
    IdentityPoolId: str,
    IdentityProviderName: str,
    UseDefaults: bool,
    PrincipalTags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteIdentitiesResponseTypeDef

```python
# DeleteIdentitiesResponseTypeDef definition

class DeleteIdentitiesResponseTypeDef(TypedDict):
    UnprocessedIdentityIds: List[UnprocessedIdentityIdTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UnprocessedIdentityIdTypeDef](./type_defs.md#unprocessedidentityidtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIdentitiesResponseTypeDef

```python
# ListIdentitiesResponseTypeDef definition

class ListIdentitiesResponseTypeDef(TypedDict):
    IdentityPoolId: str,
    Identities: List[IdentityDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IdentityDescriptionTypeDef](./type_defs.md#identitydescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIdentityPoolsResponseTypeDef

```python
# ListIdentityPoolsResponseTypeDef definition

class ListIdentityPoolsResponseTypeDef(TypedDict):
    IdentityPools: List[IdentityPoolShortDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IdentityPoolShortDescriptionTypeDef](./type_defs.md#identitypoolshortdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIdentityPoolsInputPaginateTypeDef

```python
# ListIdentityPoolsInputPaginateTypeDef definition

class ListIdentityPoolsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## RulesConfigurationTypeOutputTypeDef

```python
# RulesConfigurationTypeOutputTypeDef definition

class RulesConfigurationTypeOutputTypeDef(TypedDict):
    Rules: List[MappingRuleTypeDef],  # (1)
```

1. See [:material-code-braces: MappingRuleTypeDef](./type_defs.md#mappingruletypedef) 
## RulesConfigurationTypeTypeDef

```python
# RulesConfigurationTypeTypeDef definition

class RulesConfigurationTypeTypeDef(TypedDict):
    Rules: Sequence[MappingRuleTypeDef],  # (1)
```

1. See [:material-code-braces: MappingRuleTypeDef](./type_defs.md#mappingruletypedef) 
## RoleMappingOutputTypeDef

```python
# RoleMappingOutputTypeDef definition

class RoleMappingOutputTypeDef(TypedDict):
    Type: RoleMappingTypeType,  # (1)
    AmbiguousRoleResolution: NotRequired[AmbiguousRoleResolutionTypeType],  # (2)
    RulesConfiguration: NotRequired[RulesConfigurationTypeOutputTypeDef],  # (3)
```

1. See [:material-code-brackets: RoleMappingTypeType](./literals.md#rolemappingtypetype) 
2. See [:material-code-brackets: AmbiguousRoleResolutionTypeType](./literals.md#ambiguousroleresolutiontypetype) 
3. See [:material-code-braces: RulesConfigurationTypeOutputTypeDef](./type_defs.md#rulesconfigurationtypeoutputtypedef) 
## GetIdentityPoolRolesResponseTypeDef

```python
# GetIdentityPoolRolesResponseTypeDef definition

class GetIdentityPoolRolesResponseTypeDef(TypedDict):
    IdentityPoolId: str,
    Roles: Dict[str, str],
    RoleMappings: Dict[str, RoleMappingOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoleMappingOutputTypeDef](./type_defs.md#rolemappingoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RoleMappingTypeDef

```python
# RoleMappingTypeDef definition

class RoleMappingTypeDef(TypedDict):
    Type: RoleMappingTypeType,  # (1)
    AmbiguousRoleResolution: NotRequired[AmbiguousRoleResolutionTypeType],  # (2)
    RulesConfiguration: NotRequired[RulesConfigurationTypeUnionTypeDef],  # (3)
```

1. See [:material-code-brackets: RoleMappingTypeType](./literals.md#rolemappingtypetype) 
2. See [:material-code-brackets: AmbiguousRoleResolutionTypeType](./literals.md#ambiguousroleresolutiontypetype) 
3. See [:material-code-braces: RulesConfigurationTypeTypeDef](./type_defs.md#rulesconfigurationtypetypedef) [:material-code-braces: RulesConfigurationTypeOutputTypeDef](./type_defs.md#rulesconfigurationtypeoutputtypedef) 
## SetIdentityPoolRolesInputRequestTypeDef

```python
# SetIdentityPoolRolesInputRequestTypeDef definition

class SetIdentityPoolRolesInputRequestTypeDef(TypedDict):
    IdentityPoolId: str,
    Roles: Mapping[str, str],
    RoleMappings: NotRequired[Mapping[str, RoleMappingUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: RoleMappingTypeDef](./type_defs.md#rolemappingtypedef) [:material-code-braces: RoleMappingOutputTypeDef](./type_defs.md#rolemappingoutputtypedef) 
