# Type definitions

> [Index](../README.md) > [SSOAdmin](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SSOAdmin](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#ssoadmin)
    type annotations stubs module [types-aiobotocore-sso-admin](https://pypi.org/project/types-aiobotocore-sso-admin/).

## AccessControlAttributeValueUnionTypeDef

```python
# AccessControlAttributeValueUnionTypeDef definition

AccessControlAttributeValueUnionTypeDef = Union[
    AccessControlAttributeValueTypeDef,  # (1)
    AccessControlAttributeValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AccessControlAttributeValueTypeDef](./type_defs.md#accesscontrolattributevaluetypedef) 
2. See [:material-code-braces: AccessControlAttributeValueOutputTypeDef](./type_defs.md#accesscontrolattributevalueoutputtypedef) 

## AuthorizationCodeGrantUnionTypeDef

```python
# AuthorizationCodeGrantUnionTypeDef definition

AuthorizationCodeGrantUnionTypeDef = Union[
    AuthorizationCodeGrantTypeDef,  # (1)
    AuthorizationCodeGrantOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AuthorizationCodeGrantTypeDef](./type_defs.md#authorizationcodegranttypedef) 
2. See [:material-code-braces: AuthorizationCodeGrantOutputTypeDef](./type_defs.md#authorizationcodegrantoutputtypedef) 

## AuthorizedTokenIssuerUnionTypeDef

```python
# AuthorizedTokenIssuerUnionTypeDef definition

AuthorizedTokenIssuerUnionTypeDef = Union[
    AuthorizedTokenIssuerTypeDef,  # (1)
    AuthorizedTokenIssuerOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AuthorizedTokenIssuerTypeDef](./type_defs.md#authorizedtokenissuertypedef) 
2. See [:material-code-braces: AuthorizedTokenIssuerOutputTypeDef](./type_defs.md#authorizedtokenissueroutputtypedef) 

## IamAuthenticationMethodUnionTypeDef

```python
# IamAuthenticationMethodUnionTypeDef definition

IamAuthenticationMethodUnionTypeDef = Union[
    IamAuthenticationMethodTypeDef,  # (1)
    IamAuthenticationMethodOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IamAuthenticationMethodTypeDef](./type_defs.md#iamauthenticationmethodtypedef) 
2. See [:material-code-braces: IamAuthenticationMethodOutputTypeDef](./type_defs.md#iamauthenticationmethodoutputtypedef) 

## AccessControlAttributeUnionTypeDef

```python
# AccessControlAttributeUnionTypeDef definition

AccessControlAttributeUnionTypeDef = Union[
    AccessControlAttributeTypeDef,  # (1)
    AccessControlAttributeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AccessControlAttributeTypeDef](./type_defs.md#accesscontrolattributetypedef) 
2. See [:material-code-braces: AccessControlAttributeOutputTypeDef](./type_defs.md#accesscontrolattributeoutputtypedef) 

## JwtBearerGrantUnionTypeDef

```python
# JwtBearerGrantUnionTypeDef definition

JwtBearerGrantUnionTypeDef = Union[
    JwtBearerGrantTypeDef,  # (1)
    JwtBearerGrantOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: JwtBearerGrantTypeDef](./type_defs.md#jwtbearergranttypedef) 
2. See [:material-code-braces: JwtBearerGrantOutputTypeDef](./type_defs.md#jwtbearergrantoutputtypedef) 



## AccessControlAttributeValueOutputTypeDef

```python
# AccessControlAttributeValueOutputTypeDef definition

class AccessControlAttributeValueOutputTypeDef(TypedDict):
    Source: List[str],
```

## AccessControlAttributeValueTypeDef

```python
# AccessControlAttributeValueTypeDef definition

class AccessControlAttributeValueTypeDef(TypedDict):
    Source: Sequence[str],
```

## AccountAssignmentForPrincipalTypeDef

```python
# AccountAssignmentForPrincipalTypeDef definition

class AccountAssignmentForPrincipalTypeDef(TypedDict):
    AccountId: NotRequired[str],
    PermissionSetArn: NotRequired[str],
    PrincipalId: NotRequired[str],
    PrincipalType: NotRequired[PrincipalTypeType],  # (1)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
## AccountAssignmentOperationStatusMetadataTypeDef

```python
# AccountAssignmentOperationStatusMetadataTypeDef definition

class AccountAssignmentOperationStatusMetadataTypeDef(TypedDict):
    CreatedDate: NotRequired[datetime],
    RequestId: NotRequired[str],
    Status: NotRequired[StatusValuesType],  # (1)
```

1. See [:material-code-brackets: StatusValuesType](./literals.md#statusvaluestype) 
## AccountAssignmentOperationStatusTypeDef

```python
# AccountAssignmentOperationStatusTypeDef definition

class AccountAssignmentOperationStatusTypeDef(TypedDict):
    CreatedDate: NotRequired[datetime],
    FailureReason: NotRequired[str],
    PermissionSetArn: NotRequired[str],
    PrincipalId: NotRequired[str],
    PrincipalType: NotRequired[PrincipalTypeType],  # (1)
    RequestId: NotRequired[str],
    Status: NotRequired[StatusValuesType],  # (2)
    TargetId: NotRequired[str],
    TargetType: NotRequired[TargetTypeType],  # (3)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-brackets: StatusValuesType](./literals.md#statusvaluestype) 
3. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
## AccountAssignmentTypeDef

```python
# AccountAssignmentTypeDef definition

class AccountAssignmentTypeDef(TypedDict):
    AccountId: NotRequired[str],
    PermissionSetArn: NotRequired[str],
    PrincipalId: NotRequired[str],
    PrincipalType: NotRequired[PrincipalTypeType],  # (1)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
## ApplicationAssignmentForPrincipalTypeDef

```python
# ApplicationAssignmentForPrincipalTypeDef definition

class ApplicationAssignmentForPrincipalTypeDef(TypedDict):
    ApplicationArn: NotRequired[str],
    PrincipalId: NotRequired[str],
    PrincipalType: NotRequired[PrincipalTypeType],  # (1)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
## ApplicationAssignmentTypeDef

```python
# ApplicationAssignmentTypeDef definition

class ApplicationAssignmentTypeDef(TypedDict):
    ApplicationArn: str,
    PrincipalId: str,
    PrincipalType: PrincipalTypeType,  # (1)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
## DisplayDataTypeDef

```python
# DisplayDataTypeDef definition

class DisplayDataTypeDef(TypedDict):
    Description: NotRequired[str],
    DisplayName: NotRequired[str],
    IconUrl: NotRequired[str],
```

## CustomerManagedPolicyReferenceTypeDef

```python
# CustomerManagedPolicyReferenceTypeDef definition

class CustomerManagedPolicyReferenceTypeDef(TypedDict):
    Name: str,
    Path: NotRequired[str],
```

## AttachManagedPolicyToPermissionSetRequestRequestTypeDef

```python
# AttachManagedPolicyToPermissionSetRequestRequestTypeDef definition

class AttachManagedPolicyToPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    ManagedPolicyArn: str,
    PermissionSetArn: str,
```

## AttachedManagedPolicyTypeDef

```python
# AttachedManagedPolicyTypeDef definition

class AttachedManagedPolicyTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
```

## IamAuthenticationMethodOutputTypeDef

```python
# IamAuthenticationMethodOutputTypeDef definition

class IamAuthenticationMethodOutputTypeDef(TypedDict):
    ActorPolicy: Dict[str, Any],
```

## AuthorizationCodeGrantOutputTypeDef

```python
# AuthorizationCodeGrantOutputTypeDef definition

class AuthorizationCodeGrantOutputTypeDef(TypedDict):
    RedirectUris: NotRequired[List[str]],
```

## AuthorizationCodeGrantTypeDef

```python
# AuthorizationCodeGrantTypeDef definition

class AuthorizationCodeGrantTypeDef(TypedDict):
    RedirectUris: NotRequired[Sequence[str]],
```

## AuthorizedTokenIssuerOutputTypeDef

```python
# AuthorizedTokenIssuerOutputTypeDef definition

class AuthorizedTokenIssuerOutputTypeDef(TypedDict):
    AuthorizedAudiences: NotRequired[List[str]],
    TrustedTokenIssuerArn: NotRequired[str],
```

## AuthorizedTokenIssuerTypeDef

```python
# AuthorizedTokenIssuerTypeDef definition

class AuthorizedTokenIssuerTypeDef(TypedDict):
    AuthorizedAudiences: NotRequired[Sequence[str]],
    TrustedTokenIssuerArn: NotRequired[str],
```

## CreateAccountAssignmentRequestRequestTypeDef

```python
# CreateAccountAssignmentRequestRequestTypeDef definition

class CreateAccountAssignmentRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    PrincipalId: str,
    PrincipalType: PrincipalTypeType,  # (1)
    TargetId: str,
    TargetType: TargetTypeType,  # (2)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
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

## CreateApplicationAssignmentRequestRequestTypeDef

```python
# CreateApplicationAssignmentRequestRequestTypeDef definition

class CreateApplicationAssignmentRequestRequestTypeDef(TypedDict):
    ApplicationArn: str,
    PrincipalId: str,
    PrincipalType: PrincipalTypeType,  # (1)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## PermissionSetTypeDef

```python
# PermissionSetTypeDef definition

class PermissionSetTypeDef(TypedDict):
    CreatedDate: NotRequired[datetime],
    Description: NotRequired[str],
    Name: NotRequired[str],
    PermissionSetArn: NotRequired[str],
    RelayState: NotRequired[str],
    SessionDuration: NotRequired[str],
```

## DeleteAccountAssignmentRequestRequestTypeDef

```python
# DeleteAccountAssignmentRequestRequestTypeDef definition

class DeleteAccountAssignmentRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    PrincipalId: str,
    PrincipalType: PrincipalTypeType,  # (1)
    TargetId: str,
    TargetType: TargetTypeType,  # (2)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
## DeleteApplicationAccessScopeRequestRequestTypeDef

```python
# DeleteApplicationAccessScopeRequestRequestTypeDef definition

class DeleteApplicationAccessScopeRequestRequestTypeDef(TypedDict):
    ApplicationArn: str,
    Scope: str,
```

## DeleteApplicationAssignmentRequestRequestTypeDef

```python
# DeleteApplicationAssignmentRequestRequestTypeDef definition

class DeleteApplicationAssignmentRequestRequestTypeDef(TypedDict):
    ApplicationArn: str,
    PrincipalId: str,
    PrincipalType: PrincipalTypeType,  # (1)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
## DeleteApplicationAuthenticationMethodRequestRequestTypeDef

```python
# DeleteApplicationAuthenticationMethodRequestRequestTypeDef definition

class DeleteApplicationAuthenticationMethodRequestRequestTypeDef(TypedDict):
    ApplicationArn: str,
    AuthenticationMethodType: AuthenticationMethodTypeType,  # (1)
```

1. See [:material-code-brackets: AuthenticationMethodTypeType](./literals.md#authenticationmethodtypetype) 
## DeleteApplicationGrantRequestRequestTypeDef

```python
# DeleteApplicationGrantRequestRequestTypeDef definition

class DeleteApplicationGrantRequestRequestTypeDef(TypedDict):
    ApplicationArn: str,
    GrantType: GrantTypeType,  # (1)
```

1. See [:material-code-brackets: GrantTypeType](./literals.md#granttypetype) 
## DeleteApplicationRequestRequestTypeDef

```python
# DeleteApplicationRequestRequestTypeDef definition

class DeleteApplicationRequestRequestTypeDef(TypedDict):
    ApplicationArn: str,
```

## DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef

```python
# DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef definition

class DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
```

## DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef

```python
# DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef definition

class DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
```

## DeleteInstanceRequestRequestTypeDef

```python
# DeleteInstanceRequestRequestTypeDef definition

class DeleteInstanceRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
```

## DeletePermissionSetRequestRequestTypeDef

```python
# DeletePermissionSetRequestRequestTypeDef definition

class DeletePermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
```

## DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef

```python
# DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef definition

class DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
```

## DeleteTrustedTokenIssuerRequestRequestTypeDef

```python
# DeleteTrustedTokenIssuerRequestRequestTypeDef definition

class DeleteTrustedTokenIssuerRequestRequestTypeDef(TypedDict):
    TrustedTokenIssuerArn: str,
```

## DescribeAccountAssignmentCreationStatusRequestRequestTypeDef

```python
# DescribeAccountAssignmentCreationStatusRequestRequestTypeDef definition

class DescribeAccountAssignmentCreationStatusRequestRequestTypeDef(TypedDict):
    AccountAssignmentCreationRequestId: str,
    InstanceArn: str,
```

## DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef

```python
# DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef definition

class DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef(TypedDict):
    AccountAssignmentDeletionRequestId: str,
    InstanceArn: str,
```

## DescribeApplicationAssignmentRequestRequestTypeDef

```python
# DescribeApplicationAssignmentRequestRequestTypeDef definition

class DescribeApplicationAssignmentRequestRequestTypeDef(TypedDict):
    ApplicationArn: str,
    PrincipalId: str,
    PrincipalType: PrincipalTypeType,  # (1)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
## DescribeApplicationProviderRequestRequestTypeDef

```python
# DescribeApplicationProviderRequestRequestTypeDef definition

class DescribeApplicationProviderRequestRequestTypeDef(TypedDict):
    ApplicationProviderArn: str,
```

## DescribeApplicationRequestRequestTypeDef

```python
# DescribeApplicationRequestRequestTypeDef definition

class DescribeApplicationRequestRequestTypeDef(TypedDict):
    ApplicationArn: str,
```

## DescribeInstanceAccessControlAttributeConfigurationRequestRequestTypeDef

```python
# DescribeInstanceAccessControlAttributeConfigurationRequestRequestTypeDef definition

class DescribeInstanceAccessControlAttributeConfigurationRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
```

## DescribeInstanceRequestRequestTypeDef

```python
# DescribeInstanceRequestRequestTypeDef definition

class DescribeInstanceRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
```

## DescribePermissionSetProvisioningStatusRequestRequestTypeDef

```python
# DescribePermissionSetProvisioningStatusRequestRequestTypeDef definition

class DescribePermissionSetProvisioningStatusRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    ProvisionPermissionSetRequestId: str,
```

## PermissionSetProvisioningStatusTypeDef

```python
# PermissionSetProvisioningStatusTypeDef definition

class PermissionSetProvisioningStatusTypeDef(TypedDict):
    AccountId: NotRequired[str],
    CreatedDate: NotRequired[datetime],
    FailureReason: NotRequired[str],
    PermissionSetArn: NotRequired[str],
    RequestId: NotRequired[str],
    Status: NotRequired[StatusValuesType],  # (1)
```

1. See [:material-code-brackets: StatusValuesType](./literals.md#statusvaluestype) 
## DescribePermissionSetRequestRequestTypeDef

```python
# DescribePermissionSetRequestRequestTypeDef definition

class DescribePermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
```

## DescribeTrustedTokenIssuerRequestRequestTypeDef

```python
# DescribeTrustedTokenIssuerRequestRequestTypeDef definition

class DescribeTrustedTokenIssuerRequestRequestTypeDef(TypedDict):
    TrustedTokenIssuerArn: str,
```

## DetachManagedPolicyFromPermissionSetRequestRequestTypeDef

```python
# DetachManagedPolicyFromPermissionSetRequestRequestTypeDef definition

class DetachManagedPolicyFromPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    ManagedPolicyArn: str,
    PermissionSetArn: str,
```

## GetApplicationAccessScopeRequestRequestTypeDef

```python
# GetApplicationAccessScopeRequestRequestTypeDef definition

class GetApplicationAccessScopeRequestRequestTypeDef(TypedDict):
    ApplicationArn: str,
    Scope: str,
```

## GetApplicationAssignmentConfigurationRequestRequestTypeDef

```python
# GetApplicationAssignmentConfigurationRequestRequestTypeDef definition

class GetApplicationAssignmentConfigurationRequestRequestTypeDef(TypedDict):
    ApplicationArn: str,
```

## GetApplicationAuthenticationMethodRequestRequestTypeDef

```python
# GetApplicationAuthenticationMethodRequestRequestTypeDef definition

class GetApplicationAuthenticationMethodRequestRequestTypeDef(TypedDict):
    ApplicationArn: str,
    AuthenticationMethodType: AuthenticationMethodTypeType,  # (1)
```

1. See [:material-code-brackets: AuthenticationMethodTypeType](./literals.md#authenticationmethodtypetype) 
## GetApplicationGrantRequestRequestTypeDef

```python
# GetApplicationGrantRequestRequestTypeDef definition

class GetApplicationGrantRequestRequestTypeDef(TypedDict):
    ApplicationArn: str,
    GrantType: GrantTypeType,  # (1)
```

1. See [:material-code-brackets: GrantTypeType](./literals.md#granttypetype) 
## GetInlinePolicyForPermissionSetRequestRequestTypeDef

```python
# GetInlinePolicyForPermissionSetRequestRequestTypeDef definition

class GetInlinePolicyForPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
```

## GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef

```python
# GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef definition

class GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
```

## IamAuthenticationMethodTypeDef

```python
# IamAuthenticationMethodTypeDef definition

class IamAuthenticationMethodTypeDef(TypedDict):
    ActorPolicy: Mapping[str, Any],
```

## InstanceMetadataTypeDef

```python
# InstanceMetadataTypeDef definition

class InstanceMetadataTypeDef(TypedDict):
    CreatedDate: NotRequired[datetime],
    IdentityStoreId: NotRequired[str],
    InstanceArn: NotRequired[str],
    Name: NotRequired[str],
    OwnerAccountId: NotRequired[str],
    Status: NotRequired[InstanceStatusType],  # (1)
```

1. See [:material-code-brackets: InstanceStatusType](./literals.md#instancestatustype) 
## OperationStatusFilterTypeDef

```python
# OperationStatusFilterTypeDef definition

class OperationStatusFilterTypeDef(TypedDict):
    Status: NotRequired[StatusValuesType],  # (1)
```

1. See [:material-code-brackets: StatusValuesType](./literals.md#statusvaluestype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAccountAssignmentsFilterTypeDef

```python
# ListAccountAssignmentsFilterTypeDef definition

class ListAccountAssignmentsFilterTypeDef(TypedDict):
    AccountId: NotRequired[str],
```

## ListAccountAssignmentsRequestRequestTypeDef

```python
# ListAccountAssignmentsRequestRequestTypeDef definition

class ListAccountAssignmentsRequestRequestTypeDef(TypedDict):
    AccountId: str,
    InstanceArn: str,
    PermissionSetArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListAccountsForProvisionedPermissionSetRequestRequestTypeDef

```python
# ListAccountsForProvisionedPermissionSetRequestRequestTypeDef definition

class ListAccountsForProvisionedPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ProvisioningStatus: NotRequired[ProvisioningStatusType],  # (1)
```

1. See [:material-code-brackets: ProvisioningStatusType](./literals.md#provisioningstatustype) 
## ListApplicationAccessScopesRequestRequestTypeDef

```python
# ListApplicationAccessScopesRequestRequestTypeDef definition

class ListApplicationAccessScopesRequestRequestTypeDef(TypedDict):
    ApplicationArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ScopeDetailsTypeDef

```python
# ScopeDetailsTypeDef definition

class ScopeDetailsTypeDef(TypedDict):
    Scope: str,
    AuthorizedTargets: NotRequired[List[str]],
```

## ListApplicationAssignmentsFilterTypeDef

```python
# ListApplicationAssignmentsFilterTypeDef definition

class ListApplicationAssignmentsFilterTypeDef(TypedDict):
    ApplicationArn: NotRequired[str],
```

## ListApplicationAssignmentsRequestRequestTypeDef

```python
# ListApplicationAssignmentsRequestRequestTypeDef definition

class ListApplicationAssignmentsRequestRequestTypeDef(TypedDict):
    ApplicationArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListApplicationAuthenticationMethodsRequestRequestTypeDef

```python
# ListApplicationAuthenticationMethodsRequestRequestTypeDef definition

class ListApplicationAuthenticationMethodsRequestRequestTypeDef(TypedDict):
    ApplicationArn: str,
    NextToken: NotRequired[str],
```

## ListApplicationGrantsRequestRequestTypeDef

```python
# ListApplicationGrantsRequestRequestTypeDef definition

class ListApplicationGrantsRequestRequestTypeDef(TypedDict):
    ApplicationArn: str,
    NextToken: NotRequired[str],
```

## ListApplicationProvidersRequestRequestTypeDef

```python
# ListApplicationProvidersRequestRequestTypeDef definition

class ListApplicationProvidersRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListApplicationsFilterTypeDef

```python
# ListApplicationsFilterTypeDef definition

class ListApplicationsFilterTypeDef(TypedDict):
    ApplicationAccount: NotRequired[str],
    ApplicationProvider: NotRequired[str],
```

## ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef

```python
# ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef definition

class ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListInstancesRequestRequestTypeDef

```python
# ListInstancesRequestRequestTypeDef definition

class ListInstancesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListManagedPoliciesInPermissionSetRequestRequestTypeDef

```python
# ListManagedPoliciesInPermissionSetRequestRequestTypeDef definition

class ListManagedPoliciesInPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## PermissionSetProvisioningStatusMetadataTypeDef

```python
# PermissionSetProvisioningStatusMetadataTypeDef definition

class PermissionSetProvisioningStatusMetadataTypeDef(TypedDict):
    CreatedDate: NotRequired[datetime],
    RequestId: NotRequired[str],
    Status: NotRequired[StatusValuesType],  # (1)
```

1. See [:material-code-brackets: StatusValuesType](./literals.md#statusvaluestype) 
## ListPermissionSetsProvisionedToAccountRequestRequestTypeDef

```python
# ListPermissionSetsProvisionedToAccountRequestRequestTypeDef definition

class ListPermissionSetsProvisionedToAccountRequestRequestTypeDef(TypedDict):
    AccountId: str,
    InstanceArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ProvisioningStatus: NotRequired[ProvisioningStatusType],  # (1)
```

1. See [:material-code-brackets: ProvisioningStatusType](./literals.md#provisioningstatustype) 
## ListPermissionSetsRequestRequestTypeDef

```python
# ListPermissionSetsRequestRequestTypeDef definition

class ListPermissionSetsRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    InstanceArn: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListTrustedTokenIssuersRequestRequestTypeDef

```python
# ListTrustedTokenIssuersRequestRequestTypeDef definition

class ListTrustedTokenIssuersRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## TrustedTokenIssuerMetadataTypeDef

```python
# TrustedTokenIssuerMetadataTypeDef definition

class TrustedTokenIssuerMetadataTypeDef(TypedDict):
    Name: NotRequired[str],
    TrustedTokenIssuerArn: NotRequired[str],
    TrustedTokenIssuerType: NotRequired[TrustedTokenIssuerTypeType],  # (1)
```

1. See [:material-code-brackets: TrustedTokenIssuerTypeType](./literals.md#trustedtokenissuertypetype) 
## OidcJwtConfigurationTypeDef

```python
# OidcJwtConfigurationTypeDef definition

class OidcJwtConfigurationTypeDef(TypedDict):
    ClaimAttributePath: str,
    IdentityStoreAttributePath: str,
    IssuerUrl: str,
    JwksRetrievalOption: JwksRetrievalOptionType,  # (1)
```

1. See [:material-code-brackets: JwksRetrievalOptionType](./literals.md#jwksretrievaloptiontype) 
## OidcJwtUpdateConfigurationTypeDef

```python
# OidcJwtUpdateConfigurationTypeDef definition

class OidcJwtUpdateConfigurationTypeDef(TypedDict):
    ClaimAttributePath: NotRequired[str],
    IdentityStoreAttributePath: NotRequired[str],
    JwksRetrievalOption: NotRequired[JwksRetrievalOptionType],  # (1)
```

1. See [:material-code-brackets: JwksRetrievalOptionType](./literals.md#jwksretrievaloptiontype) 
## SignInOptionsTypeDef

```python
# SignInOptionsTypeDef definition

class SignInOptionsTypeDef(TypedDict):
    Origin: SignInOriginType,  # (1)
    ApplicationUrl: NotRequired[str],
```

1. See [:material-code-brackets: SignInOriginType](./literals.md#signinorigintype) 
## ProvisionPermissionSetRequestRequestTypeDef

```python
# ProvisionPermissionSetRequestRequestTypeDef definition

class ProvisionPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    TargetType: ProvisionTargetTypeType,  # (1)
    TargetId: NotRequired[str],
```

1. See [:material-code-brackets: ProvisionTargetTypeType](./literals.md#provisiontargettypetype) 
## PutApplicationAccessScopeRequestRequestTypeDef

```python
# PutApplicationAccessScopeRequestRequestTypeDef definition

class PutApplicationAccessScopeRequestRequestTypeDef(TypedDict):
    ApplicationArn: str,
    Scope: str,
    AuthorizedTargets: NotRequired[Sequence[str]],
```

## PutApplicationAssignmentConfigurationRequestRequestTypeDef

```python
# PutApplicationAssignmentConfigurationRequestRequestTypeDef definition

class PutApplicationAssignmentConfigurationRequestRequestTypeDef(TypedDict):
    ApplicationArn: str,
    AssignmentRequired: bool,
```

## PutInlinePolicyToPermissionSetRequestRequestTypeDef

```python
# PutInlinePolicyToPermissionSetRequestRequestTypeDef definition

class PutInlinePolicyToPermissionSetRequestRequestTypeDef(TypedDict):
    InlinePolicy: str,
    InstanceArn: str,
    PermissionSetArn: str,
```

## ResourceServerScopeDetailsTypeDef

```python
# ResourceServerScopeDetailsTypeDef definition

class ResourceServerScopeDetailsTypeDef(TypedDict):
    DetailedTitle: NotRequired[str],
    LongDescription: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
    InstanceArn: NotRequired[str],
```

## UpdateInstanceRequestRequestTypeDef

```python
# UpdateInstanceRequestRequestTypeDef definition

class UpdateInstanceRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    Name: str,
```

## UpdatePermissionSetRequestRequestTypeDef

```python
# UpdatePermissionSetRequestRequestTypeDef definition

class UpdatePermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    Description: NotRequired[str],
    RelayState: NotRequired[str],
    SessionDuration: NotRequired[str],
```

## AccessControlAttributeOutputTypeDef

```python
# AccessControlAttributeOutputTypeDef definition

class AccessControlAttributeOutputTypeDef(TypedDict):
    Key: str,
    Value: AccessControlAttributeValueOutputTypeDef,  # (1)
```

1. See [:material-code-braces: AccessControlAttributeValueOutputTypeDef](./type_defs.md#accesscontrolattributevalueoutputtypedef) 
## AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef

```python
# AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef definition

class AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef(TypedDict):
    CustomerManagedPolicyReference: CustomerManagedPolicyReferenceTypeDef,  # (1)
    InstanceArn: str,
    PermissionSetArn: str,
```

1. See [:material-code-braces: CustomerManagedPolicyReferenceTypeDef](./type_defs.md#customermanagedpolicyreferencetypedef) 
## DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef

```python
# DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef definition

class DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef(TypedDict):
    CustomerManagedPolicyReference: CustomerManagedPolicyReferenceTypeDef,  # (1)
    InstanceArn: str,
    PermissionSetArn: str,
```

1. See [:material-code-braces: CustomerManagedPolicyReferenceTypeDef](./type_defs.md#customermanagedpolicyreferencetypedef) 
## PermissionsBoundaryTypeDef

```python
# PermissionsBoundaryTypeDef definition

class PermissionsBoundaryTypeDef(TypedDict):
    CustomerManagedPolicyReference: NotRequired[CustomerManagedPolicyReferenceTypeDef],  # (1)
    ManagedPolicyArn: NotRequired[str],
```

1. See [:material-code-braces: CustomerManagedPolicyReferenceTypeDef](./type_defs.md#customermanagedpolicyreferencetypedef) 
## AuthenticationMethodOutputTypeDef

```python
# AuthenticationMethodOutputTypeDef definition

class AuthenticationMethodOutputTypeDef(TypedDict):
    Iam: NotRequired[IamAuthenticationMethodOutputTypeDef],  # (1)
```

1. See [:material-code-braces: IamAuthenticationMethodOutputTypeDef](./type_defs.md#iamauthenticationmethodoutputtypedef) 
## JwtBearerGrantOutputTypeDef

```python
# JwtBearerGrantOutputTypeDef definition

class JwtBearerGrantOutputTypeDef(TypedDict):
    AuthorizedTokenIssuers: NotRequired[List[AuthorizedTokenIssuerOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: AuthorizedTokenIssuerOutputTypeDef](./type_defs.md#authorizedtokenissueroutputtypedef) 
## CreateAccountAssignmentResponseTypeDef

```python
# CreateAccountAssignmentResponseTypeDef definition

class CreateAccountAssignmentResponseTypeDef(TypedDict):
    AccountAssignmentCreationStatus: AccountAssignmentOperationStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountAssignmentOperationStatusTypeDef](./type_defs.md#accountassignmentoperationstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateApplicationResponseTypeDef

```python
# CreateApplicationResponseTypeDef definition

class CreateApplicationResponseTypeDef(TypedDict):
    ApplicationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInstanceResponseTypeDef

```python
# CreateInstanceResponseTypeDef definition

class CreateInstanceResponseTypeDef(TypedDict):
    InstanceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrustedTokenIssuerResponseTypeDef

```python
# CreateTrustedTokenIssuerResponseTypeDef definition

class CreateTrustedTokenIssuerResponseTypeDef(TypedDict):
    TrustedTokenIssuerArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAccountAssignmentResponseTypeDef

```python
# DeleteAccountAssignmentResponseTypeDef definition

class DeleteAccountAssignmentResponseTypeDef(TypedDict):
    AccountAssignmentDeletionStatus: AccountAssignmentOperationStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountAssignmentOperationStatusTypeDef](./type_defs.md#accountassignmentoperationstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountAssignmentCreationStatusResponseTypeDef

```python
# DescribeAccountAssignmentCreationStatusResponseTypeDef definition

class DescribeAccountAssignmentCreationStatusResponseTypeDef(TypedDict):
    AccountAssignmentCreationStatus: AccountAssignmentOperationStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountAssignmentOperationStatusTypeDef](./type_defs.md#accountassignmentoperationstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountAssignmentDeletionStatusResponseTypeDef

```python
# DescribeAccountAssignmentDeletionStatusResponseTypeDef definition

class DescribeAccountAssignmentDeletionStatusResponseTypeDef(TypedDict):
    AccountAssignmentDeletionStatus: AccountAssignmentOperationStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountAssignmentOperationStatusTypeDef](./type_defs.md#accountassignmentoperationstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeApplicationAssignmentResponseTypeDef

```python
# DescribeApplicationAssignmentResponseTypeDef definition

class DescribeApplicationAssignmentResponseTypeDef(TypedDict):
    ApplicationArn: str,
    PrincipalId: str,
    PrincipalType: PrincipalTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInstanceResponseTypeDef

```python
# DescribeInstanceResponseTypeDef definition

class DescribeInstanceResponseTypeDef(TypedDict):
    CreatedDate: datetime,
    IdentityStoreId: str,
    InstanceArn: str,
    Name: str,
    OwnerAccountId: str,
    Status: InstanceStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: InstanceStatusType](./literals.md#instancestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApplicationAccessScopeResponseTypeDef

```python
# GetApplicationAccessScopeResponseTypeDef definition

class GetApplicationAccessScopeResponseTypeDef(TypedDict):
    AuthorizedTargets: List[str],
    Scope: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApplicationAssignmentConfigurationResponseTypeDef

```python
# GetApplicationAssignmentConfigurationResponseTypeDef definition

class GetApplicationAssignmentConfigurationResponseTypeDef(TypedDict):
    AssignmentRequired: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInlinePolicyForPermissionSetResponseTypeDef

```python
# GetInlinePolicyForPermissionSetResponseTypeDef definition

class GetInlinePolicyForPermissionSetResponseTypeDef(TypedDict):
    InlinePolicy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountAssignmentCreationStatusResponseTypeDef

```python
# ListAccountAssignmentCreationStatusResponseTypeDef definition

class ListAccountAssignmentCreationStatusResponseTypeDef(TypedDict):
    AccountAssignmentsCreationStatus: List[AccountAssignmentOperationStatusMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AccountAssignmentOperationStatusMetadataTypeDef](./type_defs.md#accountassignmentoperationstatusmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountAssignmentDeletionStatusResponseTypeDef

```python
# ListAccountAssignmentDeletionStatusResponseTypeDef definition

class ListAccountAssignmentDeletionStatusResponseTypeDef(TypedDict):
    AccountAssignmentsDeletionStatus: List[AccountAssignmentOperationStatusMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AccountAssignmentOperationStatusMetadataTypeDef](./type_defs.md#accountassignmentoperationstatusmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountAssignmentsForPrincipalResponseTypeDef

```python
# ListAccountAssignmentsForPrincipalResponseTypeDef definition

class ListAccountAssignmentsForPrincipalResponseTypeDef(TypedDict):
    AccountAssignments: List[AccountAssignmentForPrincipalTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AccountAssignmentForPrincipalTypeDef](./type_defs.md#accountassignmentforprincipaltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountAssignmentsResponseTypeDef

```python
# ListAccountAssignmentsResponseTypeDef definition

class ListAccountAssignmentsResponseTypeDef(TypedDict):
    AccountAssignments: List[AccountAssignmentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AccountAssignmentTypeDef](./type_defs.md#accountassignmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountsForProvisionedPermissionSetResponseTypeDef

```python
# ListAccountsForProvisionedPermissionSetResponseTypeDef definition

class ListAccountsForProvisionedPermissionSetResponseTypeDef(TypedDict):
    AccountIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationAssignmentsForPrincipalResponseTypeDef

```python
# ListApplicationAssignmentsForPrincipalResponseTypeDef definition

class ListApplicationAssignmentsForPrincipalResponseTypeDef(TypedDict):
    ApplicationAssignments: List[ApplicationAssignmentForPrincipalTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationAssignmentForPrincipalTypeDef](./type_defs.md#applicationassignmentforprincipaltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationAssignmentsResponseTypeDef

```python
# ListApplicationAssignmentsResponseTypeDef definition

class ListApplicationAssignmentsResponseTypeDef(TypedDict):
    ApplicationAssignments: List[ApplicationAssignmentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationAssignmentTypeDef](./type_defs.md#applicationassignmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef

```python
# ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef definition

class ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef(TypedDict):
    CustomerManagedPolicyReferences: List[CustomerManagedPolicyReferenceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CustomerManagedPolicyReferenceTypeDef](./type_defs.md#customermanagedpolicyreferencetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListManagedPoliciesInPermissionSetResponseTypeDef

```python
# ListManagedPoliciesInPermissionSetResponseTypeDef definition

class ListManagedPoliciesInPermissionSetResponseTypeDef(TypedDict):
    AttachedManagedPolicies: List[AttachedManagedPolicyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AttachedManagedPolicyTypeDef](./type_defs.md#attachedmanagedpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPermissionSetsProvisionedToAccountResponseTypeDef

```python
# ListPermissionSetsProvisionedToAccountResponseTypeDef definition

class ListPermissionSetsProvisionedToAccountResponseTypeDef(TypedDict):
    PermissionSets: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPermissionSetsResponseTypeDef

```python
# ListPermissionSetsResponseTypeDef definition

class ListPermissionSetsResponseTypeDef(TypedDict):
    PermissionSets: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInstanceRequestRequestTypeDef

```python
# CreateInstanceRequestRequestTypeDef definition

class CreateInstanceRequestRequestTypeDef(TypedDict):
    ClientToken: NotRequired[str],
    Name: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePermissionSetRequestRequestTypeDef

```python
# CreatePermissionSetRequestRequestTypeDef definition

class CreatePermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    Name: str,
    Description: NotRequired[str],
    RelayState: NotRequired[str],
    SessionDuration: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
    InstanceArn: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePermissionSetResponseTypeDef

```python
# CreatePermissionSetResponseTypeDef definition

class CreatePermissionSetResponseTypeDef(TypedDict):
    PermissionSet: PermissionSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PermissionSetTypeDef](./type_defs.md#permissionsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePermissionSetResponseTypeDef

```python
# DescribePermissionSetResponseTypeDef definition

class DescribePermissionSetResponseTypeDef(TypedDict):
    PermissionSet: PermissionSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PermissionSetTypeDef](./type_defs.md#permissionsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePermissionSetProvisioningStatusResponseTypeDef

```python
# DescribePermissionSetProvisioningStatusResponseTypeDef definition

class DescribePermissionSetProvisioningStatusResponseTypeDef(TypedDict):
    PermissionSetProvisioningStatus: PermissionSetProvisioningStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PermissionSetProvisioningStatusTypeDef](./type_defs.md#permissionsetprovisioningstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProvisionPermissionSetResponseTypeDef

```python
# ProvisionPermissionSetResponseTypeDef definition

class ProvisionPermissionSetResponseTypeDef(TypedDict):
    PermissionSetProvisioningStatus: PermissionSetProvisioningStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PermissionSetProvisioningStatusTypeDef](./type_defs.md#permissionsetprovisioningstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInstancesResponseTypeDef

```python
# ListInstancesResponseTypeDef definition

class ListInstancesResponseTypeDef(TypedDict):
    Instances: List[InstanceMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InstanceMetadataTypeDef](./type_defs.md#instancemetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountAssignmentCreationStatusRequestRequestTypeDef

```python
# ListAccountAssignmentCreationStatusRequestRequestTypeDef definition

class ListAccountAssignmentCreationStatusRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    Filter: NotRequired[OperationStatusFilterTypeDef],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OperationStatusFilterTypeDef](./type_defs.md#operationstatusfiltertypedef) 
## ListAccountAssignmentDeletionStatusRequestRequestTypeDef

```python
# ListAccountAssignmentDeletionStatusRequestRequestTypeDef definition

class ListAccountAssignmentDeletionStatusRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    Filter: NotRequired[OperationStatusFilterTypeDef],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OperationStatusFilterTypeDef](./type_defs.md#operationstatusfiltertypedef) 
## ListPermissionSetProvisioningStatusRequestRequestTypeDef

```python
# ListPermissionSetProvisioningStatusRequestRequestTypeDef definition

class ListPermissionSetProvisioningStatusRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    Filter: NotRequired[OperationStatusFilterTypeDef],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OperationStatusFilterTypeDef](./type_defs.md#operationstatusfiltertypedef) 
## ListAccountAssignmentCreationStatusRequestPaginateTypeDef

```python
# ListAccountAssignmentCreationStatusRequestPaginateTypeDef definition

class ListAccountAssignmentCreationStatusRequestPaginateTypeDef(TypedDict):
    InstanceArn: str,
    Filter: NotRequired[OperationStatusFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: OperationStatusFilterTypeDef](./type_defs.md#operationstatusfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAccountAssignmentDeletionStatusRequestPaginateTypeDef

```python
# ListAccountAssignmentDeletionStatusRequestPaginateTypeDef definition

class ListAccountAssignmentDeletionStatusRequestPaginateTypeDef(TypedDict):
    InstanceArn: str,
    Filter: NotRequired[OperationStatusFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: OperationStatusFilterTypeDef](./type_defs.md#operationstatusfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAccountAssignmentsRequestPaginateTypeDef

```python
# ListAccountAssignmentsRequestPaginateTypeDef definition

class ListAccountAssignmentsRequestPaginateTypeDef(TypedDict):
    AccountId: str,
    InstanceArn: str,
    PermissionSetArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAccountsForProvisionedPermissionSetRequestPaginateTypeDef

```python
# ListAccountsForProvisionedPermissionSetRequestPaginateTypeDef definition

class ListAccountsForProvisionedPermissionSetRequestPaginateTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    ProvisioningStatus: NotRequired[ProvisioningStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ProvisioningStatusType](./literals.md#provisioningstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListApplicationAccessScopesRequestPaginateTypeDef

```python
# ListApplicationAccessScopesRequestPaginateTypeDef definition

class ListApplicationAccessScopesRequestPaginateTypeDef(TypedDict):
    ApplicationArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListApplicationAssignmentsRequestPaginateTypeDef

```python
# ListApplicationAssignmentsRequestPaginateTypeDef definition

class ListApplicationAssignmentsRequestPaginateTypeDef(TypedDict):
    ApplicationArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListApplicationAuthenticationMethodsRequestPaginateTypeDef

```python
# ListApplicationAuthenticationMethodsRequestPaginateTypeDef definition

class ListApplicationAuthenticationMethodsRequestPaginateTypeDef(TypedDict):
    ApplicationArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListApplicationGrantsRequestPaginateTypeDef

```python
# ListApplicationGrantsRequestPaginateTypeDef definition

class ListApplicationGrantsRequestPaginateTypeDef(TypedDict):
    ApplicationArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListApplicationProvidersRequestPaginateTypeDef

```python
# ListApplicationProvidersRequestPaginateTypeDef definition

class ListApplicationProvidersRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCustomerManagedPolicyReferencesInPermissionSetRequestPaginateTypeDef

```python
# ListCustomerManagedPolicyReferencesInPermissionSetRequestPaginateTypeDef definition

class ListCustomerManagedPolicyReferencesInPermissionSetRequestPaginateTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstancesRequestPaginateTypeDef

```python
# ListInstancesRequestPaginateTypeDef definition

class ListInstancesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListManagedPoliciesInPermissionSetRequestPaginateTypeDef

```python
# ListManagedPoliciesInPermissionSetRequestPaginateTypeDef definition

class ListManagedPoliciesInPermissionSetRequestPaginateTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPermissionSetProvisioningStatusRequestPaginateTypeDef

```python
# ListPermissionSetProvisioningStatusRequestPaginateTypeDef definition

class ListPermissionSetProvisioningStatusRequestPaginateTypeDef(TypedDict):
    InstanceArn: str,
    Filter: NotRequired[OperationStatusFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: OperationStatusFilterTypeDef](./type_defs.md#operationstatusfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPermissionSetsProvisionedToAccountRequestPaginateTypeDef

```python
# ListPermissionSetsProvisionedToAccountRequestPaginateTypeDef definition

class ListPermissionSetsProvisionedToAccountRequestPaginateTypeDef(TypedDict):
    AccountId: str,
    InstanceArn: str,
    ProvisioningStatus: NotRequired[ProvisioningStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ProvisioningStatusType](./literals.md#provisioningstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPermissionSetsRequestPaginateTypeDef

```python
# ListPermissionSetsRequestPaginateTypeDef definition

class ListPermissionSetsRequestPaginateTypeDef(TypedDict):
    InstanceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceRequestPaginateTypeDef

```python
# ListTagsForResourceRequestPaginateTypeDef definition

class ListTagsForResourceRequestPaginateTypeDef(TypedDict):
    ResourceArn: str,
    InstanceArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTrustedTokenIssuersRequestPaginateTypeDef

```python
# ListTrustedTokenIssuersRequestPaginateTypeDef definition

class ListTrustedTokenIssuersRequestPaginateTypeDef(TypedDict):
    InstanceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAccountAssignmentsForPrincipalRequestPaginateTypeDef

```python
# ListAccountAssignmentsForPrincipalRequestPaginateTypeDef definition

class ListAccountAssignmentsForPrincipalRequestPaginateTypeDef(TypedDict):
    InstanceArn: str,
    PrincipalId: str,
    PrincipalType: PrincipalTypeType,  # (1)
    Filter: NotRequired[ListAccountAssignmentsFilterTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-braces: ListAccountAssignmentsFilterTypeDef](./type_defs.md#listaccountassignmentsfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAccountAssignmentsForPrincipalRequestRequestTypeDef

```python
# ListAccountAssignmentsForPrincipalRequestRequestTypeDef definition

class ListAccountAssignmentsForPrincipalRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PrincipalId: str,
    PrincipalType: PrincipalTypeType,  # (1)
    Filter: NotRequired[ListAccountAssignmentsFilterTypeDef],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-braces: ListAccountAssignmentsFilterTypeDef](./type_defs.md#listaccountassignmentsfiltertypedef) 
## ListApplicationAccessScopesResponseTypeDef

```python
# ListApplicationAccessScopesResponseTypeDef definition

class ListApplicationAccessScopesResponseTypeDef(TypedDict):
    Scopes: List[ScopeDetailsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ScopeDetailsTypeDef](./type_defs.md#scopedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationAssignmentsForPrincipalRequestPaginateTypeDef

```python
# ListApplicationAssignmentsForPrincipalRequestPaginateTypeDef definition

class ListApplicationAssignmentsForPrincipalRequestPaginateTypeDef(TypedDict):
    InstanceArn: str,
    PrincipalId: str,
    PrincipalType: PrincipalTypeType,  # (1)
    Filter: NotRequired[ListApplicationAssignmentsFilterTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-braces: ListApplicationAssignmentsFilterTypeDef](./type_defs.md#listapplicationassignmentsfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListApplicationAssignmentsForPrincipalRequestRequestTypeDef

```python
# ListApplicationAssignmentsForPrincipalRequestRequestTypeDef definition

class ListApplicationAssignmentsForPrincipalRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PrincipalId: str,
    PrincipalType: PrincipalTypeType,  # (1)
    Filter: NotRequired[ListApplicationAssignmentsFilterTypeDef],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-braces: ListApplicationAssignmentsFilterTypeDef](./type_defs.md#listapplicationassignmentsfiltertypedef) 
## ListApplicationsRequestPaginateTypeDef

```python
# ListApplicationsRequestPaginateTypeDef definition

class ListApplicationsRequestPaginateTypeDef(TypedDict):
    InstanceArn: str,
    Filter: NotRequired[ListApplicationsFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListApplicationsFilterTypeDef](./type_defs.md#listapplicationsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListApplicationsRequestRequestTypeDef

```python
# ListApplicationsRequestRequestTypeDef definition

class ListApplicationsRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    Filter: NotRequired[ListApplicationsFilterTypeDef],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListApplicationsFilterTypeDef](./type_defs.md#listapplicationsfiltertypedef) 
## ListPermissionSetProvisioningStatusResponseTypeDef

```python
# ListPermissionSetProvisioningStatusResponseTypeDef definition

class ListPermissionSetProvisioningStatusResponseTypeDef(TypedDict):
    PermissionSetsProvisioningStatus: List[PermissionSetProvisioningStatusMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PermissionSetProvisioningStatusMetadataTypeDef](./type_defs.md#permissionsetprovisioningstatusmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrustedTokenIssuersResponseTypeDef

```python
# ListTrustedTokenIssuersResponseTypeDef definition

class ListTrustedTokenIssuersResponseTypeDef(TypedDict):
    TrustedTokenIssuers: List[TrustedTokenIssuerMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TrustedTokenIssuerMetadataTypeDef](./type_defs.md#trustedtokenissuermetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TrustedTokenIssuerConfigurationTypeDef

```python
# TrustedTokenIssuerConfigurationTypeDef definition

class TrustedTokenIssuerConfigurationTypeDef(TypedDict):
    OidcJwtConfiguration: NotRequired[OidcJwtConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: OidcJwtConfigurationTypeDef](./type_defs.md#oidcjwtconfigurationtypedef) 
## TrustedTokenIssuerUpdateConfigurationTypeDef

```python
# TrustedTokenIssuerUpdateConfigurationTypeDef definition

class TrustedTokenIssuerUpdateConfigurationTypeDef(TypedDict):
    OidcJwtConfiguration: NotRequired[OidcJwtUpdateConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: OidcJwtUpdateConfigurationTypeDef](./type_defs.md#oidcjwtupdateconfigurationtypedef) 
## PortalOptionsTypeDef

```python
# PortalOptionsTypeDef definition

class PortalOptionsTypeDef(TypedDict):
    SignInOptions: NotRequired[SignInOptionsTypeDef],  # (1)
    Visibility: NotRequired[ApplicationVisibilityType],  # (2)
```

1. See [:material-code-braces: SignInOptionsTypeDef](./type_defs.md#signinoptionstypedef) 
2. See [:material-code-brackets: ApplicationVisibilityType](./literals.md#applicationvisibilitytype) 
## UpdateApplicationPortalOptionsTypeDef

```python
# UpdateApplicationPortalOptionsTypeDef definition

class UpdateApplicationPortalOptionsTypeDef(TypedDict):
    SignInOptions: NotRequired[SignInOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: SignInOptionsTypeDef](./type_defs.md#signinoptionstypedef) 
## ResourceServerConfigTypeDef

```python
# ResourceServerConfigTypeDef definition

class ResourceServerConfigTypeDef(TypedDict):
    Scopes: NotRequired[Dict[str, ResourceServerScopeDetailsTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourceServerScopeDetailsTypeDef](./type_defs.md#resourceserverscopedetailstypedef) 
## InstanceAccessControlAttributeConfigurationOutputTypeDef

```python
# InstanceAccessControlAttributeConfigurationOutputTypeDef definition

class InstanceAccessControlAttributeConfigurationOutputTypeDef(TypedDict):
    AccessControlAttributes: List[AccessControlAttributeOutputTypeDef],  # (1)
```

1. See [:material-code-braces: AccessControlAttributeOutputTypeDef](./type_defs.md#accesscontrolattributeoutputtypedef) 
## AccessControlAttributeTypeDef

```python
# AccessControlAttributeTypeDef definition

class AccessControlAttributeTypeDef(TypedDict):
    Key: str,
    Value: AccessControlAttributeValueUnionTypeDef,  # (1)
```

1. See [:material-code-braces: AccessControlAttributeValueTypeDef](./type_defs.md#accesscontrolattributevaluetypedef) [:material-code-braces: AccessControlAttributeValueOutputTypeDef](./type_defs.md#accesscontrolattributevalueoutputtypedef) 
## GetPermissionsBoundaryForPermissionSetResponseTypeDef

```python
# GetPermissionsBoundaryForPermissionSetResponseTypeDef definition

class GetPermissionsBoundaryForPermissionSetResponseTypeDef(TypedDict):
    PermissionsBoundary: PermissionsBoundaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PermissionsBoundaryTypeDef](./type_defs.md#permissionsboundarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef

```python
# PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef definition

class PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    PermissionsBoundary: PermissionsBoundaryTypeDef,  # (1)
```

1. See [:material-code-braces: PermissionsBoundaryTypeDef](./type_defs.md#permissionsboundarytypedef) 
## AuthenticationMethodItemTypeDef

```python
# AuthenticationMethodItemTypeDef definition

class AuthenticationMethodItemTypeDef(TypedDict):
    AuthenticationMethod: NotRequired[AuthenticationMethodOutputTypeDef],  # (1)
    AuthenticationMethodType: NotRequired[AuthenticationMethodTypeType],  # (2)
```

1. See [:material-code-braces: AuthenticationMethodOutputTypeDef](./type_defs.md#authenticationmethodoutputtypedef) 
2. See [:material-code-brackets: AuthenticationMethodTypeType](./literals.md#authenticationmethodtypetype) 
## GetApplicationAuthenticationMethodResponseTypeDef

```python
# GetApplicationAuthenticationMethodResponseTypeDef definition

class GetApplicationAuthenticationMethodResponseTypeDef(TypedDict):
    AuthenticationMethod: AuthenticationMethodOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AuthenticationMethodOutputTypeDef](./type_defs.md#authenticationmethodoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GrantOutputTypeDef

```python
# GrantOutputTypeDef definition

class GrantOutputTypeDef(TypedDict):
    AuthorizationCode: NotRequired[AuthorizationCodeGrantOutputTypeDef],  # (1)
    JwtBearer: NotRequired[JwtBearerGrantOutputTypeDef],  # (2)
    RefreshToken: NotRequired[Dict[str, Any]],
    TokenExchange: NotRequired[Dict[str, Any]],
```

1. See [:material-code-braces: AuthorizationCodeGrantOutputTypeDef](./type_defs.md#authorizationcodegrantoutputtypedef) 
2. See [:material-code-braces: JwtBearerGrantOutputTypeDef](./type_defs.md#jwtbearergrantoutputtypedef) 
## JwtBearerGrantTypeDef

```python
# JwtBearerGrantTypeDef definition

class JwtBearerGrantTypeDef(TypedDict):
    AuthorizedTokenIssuers: NotRequired[Sequence[AuthorizedTokenIssuerUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: AuthorizedTokenIssuerTypeDef](./type_defs.md#authorizedtokenissuertypedef) [:material-code-braces: AuthorizedTokenIssuerOutputTypeDef](./type_defs.md#authorizedtokenissueroutputtypedef) 
## AuthenticationMethodTypeDef

```python
# AuthenticationMethodTypeDef definition

class AuthenticationMethodTypeDef(TypedDict):
    Iam: NotRequired[IamAuthenticationMethodUnionTypeDef],  # (1)
```

1. See [:material-code-braces: IamAuthenticationMethodTypeDef](./type_defs.md#iamauthenticationmethodtypedef) [:material-code-braces: IamAuthenticationMethodOutputTypeDef](./type_defs.md#iamauthenticationmethodoutputtypedef) 
## CreateTrustedTokenIssuerRequestRequestTypeDef

```python
# CreateTrustedTokenIssuerRequestRequestTypeDef definition

class CreateTrustedTokenIssuerRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    Name: str,
    TrustedTokenIssuerConfiguration: TrustedTokenIssuerConfigurationTypeDef,  # (1)
    TrustedTokenIssuerType: TrustedTokenIssuerTypeType,  # (2)
    ClientToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: TrustedTokenIssuerConfigurationTypeDef](./type_defs.md#trustedtokenissuerconfigurationtypedef) 
2. See [:material-code-brackets: TrustedTokenIssuerTypeType](./literals.md#trustedtokenissuertypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeTrustedTokenIssuerResponseTypeDef

```python
# DescribeTrustedTokenIssuerResponseTypeDef definition

class DescribeTrustedTokenIssuerResponseTypeDef(TypedDict):
    Name: str,
    TrustedTokenIssuerArn: str,
    TrustedTokenIssuerConfiguration: TrustedTokenIssuerConfigurationTypeDef,  # (1)
    TrustedTokenIssuerType: TrustedTokenIssuerTypeType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: TrustedTokenIssuerConfigurationTypeDef](./type_defs.md#trustedtokenissuerconfigurationtypedef) 
2. See [:material-code-brackets: TrustedTokenIssuerTypeType](./literals.md#trustedtokenissuertypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTrustedTokenIssuerRequestRequestTypeDef

```python
# UpdateTrustedTokenIssuerRequestRequestTypeDef definition

class UpdateTrustedTokenIssuerRequestRequestTypeDef(TypedDict):
    TrustedTokenIssuerArn: str,
    Name: NotRequired[str],
    TrustedTokenIssuerConfiguration: NotRequired[TrustedTokenIssuerUpdateConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: TrustedTokenIssuerUpdateConfigurationTypeDef](./type_defs.md#trustedtokenissuerupdateconfigurationtypedef) 
## ApplicationTypeDef

```python
# ApplicationTypeDef definition

class ApplicationTypeDef(TypedDict):
    ApplicationAccount: NotRequired[str],
    ApplicationArn: NotRequired[str],
    ApplicationProviderArn: NotRequired[str],
    CreatedDate: NotRequired[datetime],
    Description: NotRequired[str],
    InstanceArn: NotRequired[str],
    Name: NotRequired[str],
    PortalOptions: NotRequired[PortalOptionsTypeDef],  # (1)
    Status: NotRequired[ApplicationStatusType],  # (2)
```

1. See [:material-code-braces: PortalOptionsTypeDef](./type_defs.md#portaloptionstypedef) 
2. See [:material-code-brackets: ApplicationStatusType](./literals.md#applicationstatustype) 
## CreateApplicationRequestRequestTypeDef

```python
# CreateApplicationRequestRequestTypeDef definition

class CreateApplicationRequestRequestTypeDef(TypedDict):
    ApplicationProviderArn: str,
    InstanceArn: str,
    Name: str,
    ClientToken: NotRequired[str],
    Description: NotRequired[str],
    PortalOptions: NotRequired[PortalOptionsTypeDef],  # (1)
    Status: NotRequired[ApplicationStatusType],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: PortalOptionsTypeDef](./type_defs.md#portaloptionstypedef) 
2. See [:material-code-brackets: ApplicationStatusType](./literals.md#applicationstatustype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeApplicationResponseTypeDef

```python
# DescribeApplicationResponseTypeDef definition

class DescribeApplicationResponseTypeDef(TypedDict):
    ApplicationAccount: str,
    ApplicationArn: str,
    ApplicationProviderArn: str,
    CreatedDate: datetime,
    Description: str,
    InstanceArn: str,
    Name: str,
    PortalOptions: PortalOptionsTypeDef,  # (1)
    Status: ApplicationStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PortalOptionsTypeDef](./type_defs.md#portaloptionstypedef) 
2. See [:material-code-brackets: ApplicationStatusType](./literals.md#applicationstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApplicationRequestRequestTypeDef

```python
# UpdateApplicationRequestRequestTypeDef definition

class UpdateApplicationRequestRequestTypeDef(TypedDict):
    ApplicationArn: str,
    Description: NotRequired[str],
    Name: NotRequired[str],
    PortalOptions: NotRequired[UpdateApplicationPortalOptionsTypeDef],  # (1)
    Status: NotRequired[ApplicationStatusType],  # (2)
```

1. See [:material-code-braces: UpdateApplicationPortalOptionsTypeDef](./type_defs.md#updateapplicationportaloptionstypedef) 
2. See [:material-code-brackets: ApplicationStatusType](./literals.md#applicationstatustype) 
## ApplicationProviderTypeDef

```python
# ApplicationProviderTypeDef definition

class ApplicationProviderTypeDef(TypedDict):
    ApplicationProviderArn: str,
    DisplayData: NotRequired[DisplayDataTypeDef],  # (1)
    FederationProtocol: NotRequired[FederationProtocolType],  # (2)
    ResourceServerConfig: NotRequired[ResourceServerConfigTypeDef],  # (3)
```

1. See [:material-code-braces: DisplayDataTypeDef](./type_defs.md#displaydatatypedef) 
2. See [:material-code-brackets: FederationProtocolType](./literals.md#federationprotocoltype) 
3. See [:material-code-braces: ResourceServerConfigTypeDef](./type_defs.md#resourceserverconfigtypedef) 
## DescribeApplicationProviderResponseTypeDef

```python
# DescribeApplicationProviderResponseTypeDef definition

class DescribeApplicationProviderResponseTypeDef(TypedDict):
    ApplicationProviderArn: str,
    DisplayData: DisplayDataTypeDef,  # (1)
    FederationProtocol: FederationProtocolType,  # (2)
    ResourceServerConfig: ResourceServerConfigTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: DisplayDataTypeDef](./type_defs.md#displaydatatypedef) 
2. See [:material-code-brackets: FederationProtocolType](./literals.md#federationprotocoltype) 
3. See [:material-code-braces: ResourceServerConfigTypeDef](./type_defs.md#resourceserverconfigtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef

```python
# DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef definition

class DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef(TypedDict):
    InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationOutputTypeDef,  # (1)
    Status: InstanceAccessControlAttributeConfigurationStatusType,  # (2)
    StatusReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: InstanceAccessControlAttributeConfigurationOutputTypeDef](./type_defs.md#instanceaccesscontrolattributeconfigurationoutputtypedef) 
2. See [:material-code-brackets: InstanceAccessControlAttributeConfigurationStatusType](./literals.md#instanceaccesscontrolattributeconfigurationstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationAuthenticationMethodsResponseTypeDef

```python
# ListApplicationAuthenticationMethodsResponseTypeDef definition

class ListApplicationAuthenticationMethodsResponseTypeDef(TypedDict):
    AuthenticationMethods: List[AuthenticationMethodItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AuthenticationMethodItemTypeDef](./type_defs.md#authenticationmethoditemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApplicationGrantResponseTypeDef

```python
# GetApplicationGrantResponseTypeDef definition

class GetApplicationGrantResponseTypeDef(TypedDict):
    Grant: GrantOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GrantOutputTypeDef](./type_defs.md#grantoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GrantItemTypeDef

```python
# GrantItemTypeDef definition

class GrantItemTypeDef(TypedDict):
    Grant: GrantOutputTypeDef,  # (1)
    GrantType: GrantTypeType,  # (2)
```

1. See [:material-code-braces: GrantOutputTypeDef](./type_defs.md#grantoutputtypedef) 
2. See [:material-code-brackets: GrantTypeType](./literals.md#granttypetype) 
## PutApplicationAuthenticationMethodRequestRequestTypeDef

```python
# PutApplicationAuthenticationMethodRequestRequestTypeDef definition

class PutApplicationAuthenticationMethodRequestRequestTypeDef(TypedDict):
    ApplicationArn: str,
    AuthenticationMethod: AuthenticationMethodTypeDef,  # (1)
    AuthenticationMethodType: AuthenticationMethodTypeType,  # (2)
```

1. See [:material-code-braces: AuthenticationMethodTypeDef](./type_defs.md#authenticationmethodtypedef) 
2. See [:material-code-brackets: AuthenticationMethodTypeType](./literals.md#authenticationmethodtypetype) 
## ListApplicationsResponseTypeDef

```python
# ListApplicationsResponseTypeDef definition

class ListApplicationsResponseTypeDef(TypedDict):
    Applications: List[ApplicationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationProvidersResponseTypeDef

```python
# ListApplicationProvidersResponseTypeDef definition

class ListApplicationProvidersResponseTypeDef(TypedDict):
    ApplicationProviders: List[ApplicationProviderTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationProviderTypeDef](./type_defs.md#applicationprovidertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstanceAccessControlAttributeConfigurationTypeDef

```python
# InstanceAccessControlAttributeConfigurationTypeDef definition

class InstanceAccessControlAttributeConfigurationTypeDef(TypedDict):
    AccessControlAttributes: Sequence[AccessControlAttributeUnionTypeDef],  # (1)
```

1. See [:material-code-braces: AccessControlAttributeTypeDef](./type_defs.md#accesscontrolattributetypedef) [:material-code-braces: AccessControlAttributeOutputTypeDef](./type_defs.md#accesscontrolattributeoutputtypedef) 
## ListApplicationGrantsResponseTypeDef

```python
# ListApplicationGrantsResponseTypeDef definition

class ListApplicationGrantsResponseTypeDef(TypedDict):
    Grants: List[GrantItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GrantItemTypeDef](./type_defs.md#grantitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GrantTypeDef

```python
# GrantTypeDef definition

class GrantTypeDef(TypedDict):
    AuthorizationCode: NotRequired[AuthorizationCodeGrantUnionTypeDef],  # (1)
    JwtBearer: NotRequired[JwtBearerGrantUnionTypeDef],  # (2)
    RefreshToken: NotRequired[Mapping[str, Any]],
    TokenExchange: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: AuthorizationCodeGrantTypeDef](./type_defs.md#authorizationcodegranttypedef) [:material-code-braces: AuthorizationCodeGrantOutputTypeDef](./type_defs.md#authorizationcodegrantoutputtypedef) 
2. See [:material-code-braces: JwtBearerGrantTypeDef](./type_defs.md#jwtbearergranttypedef) [:material-code-braces: JwtBearerGrantOutputTypeDef](./type_defs.md#jwtbearergrantoutputtypedef) 
## CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef

```python
# CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef definition

class CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef(TypedDict):
    InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationTypeDef,  # (1)
    InstanceArn: str,
```

1. See [:material-code-braces: InstanceAccessControlAttributeConfigurationTypeDef](./type_defs.md#instanceaccesscontrolattributeconfigurationtypedef) 
## UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef

```python
# UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef definition

class UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef(TypedDict):
    InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationTypeDef,  # (1)
    InstanceArn: str,
```

1. See [:material-code-braces: InstanceAccessControlAttributeConfigurationTypeDef](./type_defs.md#instanceaccesscontrolattributeconfigurationtypedef) 
## PutApplicationGrantRequestRequestTypeDef

```python
# PutApplicationGrantRequestRequestTypeDef definition

class PutApplicationGrantRequestRequestTypeDef(TypedDict):
    ApplicationArn: str,
    Grant: GrantTypeDef,  # (1)
    GrantType: GrantTypeType,  # (2)
```

1. See [:material-code-braces: GrantTypeDef](./type_defs.md#granttypedef) 
2. See [:material-code-brackets: GrantTypeType](./literals.md#granttypetype) 
