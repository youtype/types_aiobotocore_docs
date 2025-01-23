# Type definitions

> [Index](../README.md) > [IAM](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IAM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#iam)
    type annotations stubs module [types-aiobotocore-iam](https://pypi.org/project/types-aiobotocore-iam/).

## PolicyDocumentTypeDef

```python
# PolicyDocumentTypeDef definition

PolicyDocumentTypeDef = Union[
    str,
    PolicyDocumentDictTypeDef,  # (1)
]
```

1. See [:material-code-braces: PolicyDocumentDictTypeDef](./type_defs.md#policydocumentdicttypedef) 



## AccessDetailTypeDef

```python
# AccessDetailTypeDef definition

class AccessDetailTypeDef(TypedDict):
    ServiceName: str,
    ServiceNamespace: str,
    Region: NotRequired[str],
    EntityPath: NotRequired[str],
    LastAuthenticatedTime: NotRequired[datetime],
    TotalAuthenticatedEntities: NotRequired[int],
```

## AccessKeyLastUsedTypeDef

```python
# AccessKeyLastUsedTypeDef definition

class AccessKeyLastUsedTypeDef(TypedDict):
    ServiceName: str,
    Region: str,
    LastUsedDate: NotRequired[datetime],
```

## AccessKeyMetadataTypeDef

```python
# AccessKeyMetadataTypeDef definition

class AccessKeyMetadataTypeDef(TypedDict):
    UserName: NotRequired[str],
    AccessKeyId: NotRequired[str],
    Status: NotRequired[StatusTypeType],  # (1)
    CreateDate: NotRequired[datetime],
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
## AccessKeyTypeDef

```python
# AccessKeyTypeDef definition

class AccessKeyTypeDef(TypedDict):
    UserName: str,
    AccessKeyId: str,
    Status: StatusTypeType,  # (1)
    SecretAccessKey: str,
    CreateDate: NotRequired[datetime],
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
## AddClientIDToOpenIDConnectProviderRequestRequestTypeDef

```python
# AddClientIDToOpenIDConnectProviderRequestRequestTypeDef definition

class AddClientIDToOpenIDConnectProviderRequestRequestTypeDef(TypedDict):
    OpenIDConnectProviderArn: str,
    ClientID: str,
```

## AddRoleToInstanceProfileRequestInstanceProfileAddRoleTypeDef

```python
# AddRoleToInstanceProfileRequestInstanceProfileAddRoleTypeDef definition

class AddRoleToInstanceProfileRequestInstanceProfileAddRoleTypeDef(TypedDict):
    RoleName: str,
```

## AddRoleToInstanceProfileRequestRequestTypeDef

```python
# AddRoleToInstanceProfileRequestRequestTypeDef definition

class AddRoleToInstanceProfileRequestRequestTypeDef(TypedDict):
    InstanceProfileName: str,
    RoleName: str,
```

## AddUserToGroupRequestGroupAddUserTypeDef

```python
# AddUserToGroupRequestGroupAddUserTypeDef definition

class AddUserToGroupRequestGroupAddUserTypeDef(TypedDict):
    UserName: str,
```

## AddUserToGroupRequestRequestTypeDef

```python
# AddUserToGroupRequestRequestTypeDef definition

class AddUserToGroupRequestRequestTypeDef(TypedDict):
    GroupName: str,
    UserName: str,
```

## AddUserToGroupRequestUserAddGroupTypeDef

```python
# AddUserToGroupRequestUserAddGroupTypeDef definition

class AddUserToGroupRequestUserAddGroupTypeDef(TypedDict):
    GroupName: str,
```

## AttachGroupPolicyRequestGroupAttachPolicyTypeDef

```python
# AttachGroupPolicyRequestGroupAttachPolicyTypeDef definition

class AttachGroupPolicyRequestGroupAttachPolicyTypeDef(TypedDict):
    PolicyArn: str,
```

## AttachGroupPolicyRequestPolicyAttachGroupTypeDef

```python
# AttachGroupPolicyRequestPolicyAttachGroupTypeDef definition

class AttachGroupPolicyRequestPolicyAttachGroupTypeDef(TypedDict):
    GroupName: str,
```

## AttachGroupPolicyRequestRequestTypeDef

```python
# AttachGroupPolicyRequestRequestTypeDef definition

class AttachGroupPolicyRequestRequestTypeDef(TypedDict):
    GroupName: str,
    PolicyArn: str,
```

## AttachRolePolicyRequestPolicyAttachRoleTypeDef

```python
# AttachRolePolicyRequestPolicyAttachRoleTypeDef definition

class AttachRolePolicyRequestPolicyAttachRoleTypeDef(TypedDict):
    RoleName: str,
```

## AttachRolePolicyRequestRequestTypeDef

```python
# AttachRolePolicyRequestRequestTypeDef definition

class AttachRolePolicyRequestRequestTypeDef(TypedDict):
    RoleName: str,
    PolicyArn: str,
```

## AttachRolePolicyRequestRoleAttachPolicyTypeDef

```python
# AttachRolePolicyRequestRoleAttachPolicyTypeDef definition

class AttachRolePolicyRequestRoleAttachPolicyTypeDef(TypedDict):
    PolicyArn: str,
```

## AttachUserPolicyRequestPolicyAttachUserTypeDef

```python
# AttachUserPolicyRequestPolicyAttachUserTypeDef definition

class AttachUserPolicyRequestPolicyAttachUserTypeDef(TypedDict):
    UserName: str,
```

## AttachUserPolicyRequestRequestTypeDef

```python
# AttachUserPolicyRequestRequestTypeDef definition

class AttachUserPolicyRequestRequestTypeDef(TypedDict):
    UserName: str,
    PolicyArn: str,
```

## AttachUserPolicyRequestUserAttachPolicyTypeDef

```python
# AttachUserPolicyRequestUserAttachPolicyTypeDef definition

class AttachUserPolicyRequestUserAttachPolicyTypeDef(TypedDict):
    PolicyArn: str,
```

## AttachedPermissionsBoundaryTypeDef

```python
# AttachedPermissionsBoundaryTypeDef definition

class AttachedPermissionsBoundaryTypeDef(TypedDict):
    PermissionsBoundaryType: NotRequired[PermissionsBoundaryAttachmentTypeType],  # (1)
    PermissionsBoundaryArn: NotRequired[str],
```

1. See [:material-code-brackets: PermissionsBoundaryAttachmentTypeType](./literals.md#permissionsboundaryattachmenttypetype) 
## AttachedPolicyTypeDef

```python
# AttachedPolicyTypeDef definition

class AttachedPolicyTypeDef(TypedDict):
    PolicyName: NotRequired[str],
    PolicyArn: NotRequired[str],
```

## ChangePasswordRequestRequestTypeDef

```python
# ChangePasswordRequestRequestTypeDef definition

class ChangePasswordRequestRequestTypeDef(TypedDict):
    OldPassword: str,
    NewPassword: str,
```

## ChangePasswordRequestServiceResourceChangePasswordTypeDef

```python
# ChangePasswordRequestServiceResourceChangePasswordTypeDef definition

class ChangePasswordRequestServiceResourceChangePasswordTypeDef(TypedDict):
    OldPassword: str,
    NewPassword: str,
```

## ContextEntryTypeDef

```python
# ContextEntryTypeDef definition

class ContextEntryTypeDef(TypedDict):
    ContextKeyName: NotRequired[str],
    ContextKeyValues: NotRequired[Sequence[str]],
    ContextKeyType: NotRequired[ContextKeyTypeEnumType],  # (1)
```

1. See [:material-code-brackets: ContextKeyTypeEnumType](./literals.md#contextkeytypeenumtype) 
## CreateAccessKeyRequestRequestTypeDef

```python
# CreateAccessKeyRequestRequestTypeDef definition

class CreateAccessKeyRequestRequestTypeDef(TypedDict):
    UserName: NotRequired[str],
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

## CreateAccountAliasRequestRequestTypeDef

```python
# CreateAccountAliasRequestRequestTypeDef definition

class CreateAccountAliasRequestRequestTypeDef(TypedDict):
    AccountAlias: str,
```

## CreateAccountAliasRequestServiceResourceCreateAccountAliasTypeDef

```python
# CreateAccountAliasRequestServiceResourceCreateAccountAliasTypeDef definition

class CreateAccountAliasRequestServiceResourceCreateAccountAliasTypeDef(TypedDict):
    AccountAlias: str,
```

## CreateGroupRequestGroupCreateTypeDef

```python
# CreateGroupRequestGroupCreateTypeDef definition

class CreateGroupRequestGroupCreateTypeDef(TypedDict):
    Path: NotRequired[str],
```

## CreateGroupRequestRequestTypeDef

```python
# CreateGroupRequestRequestTypeDef definition

class CreateGroupRequestRequestTypeDef(TypedDict):
    GroupName: str,
    Path: NotRequired[str],
```

## CreateGroupRequestServiceResourceCreateGroupTypeDef

```python
# CreateGroupRequestServiceResourceCreateGroupTypeDef definition

class CreateGroupRequestServiceResourceCreateGroupTypeDef(TypedDict):
    GroupName: str,
    Path: NotRequired[str],
```

## GroupTypeDef

```python
# GroupTypeDef definition

class GroupTypeDef(TypedDict):
    Path: str,
    GroupName: str,
    GroupId: str,
    Arn: str,
    CreateDate: datetime,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## CreateLoginProfileRequestLoginProfileCreateTypeDef

```python
# CreateLoginProfileRequestLoginProfileCreateTypeDef definition

class CreateLoginProfileRequestLoginProfileCreateTypeDef(TypedDict):
    Password: NotRequired[str],
    PasswordResetRequired: NotRequired[bool],
```

## CreateLoginProfileRequestRequestTypeDef

```python
# CreateLoginProfileRequestRequestTypeDef definition

class CreateLoginProfileRequestRequestTypeDef(TypedDict):
    UserName: NotRequired[str],
    Password: NotRequired[str],
    PasswordResetRequired: NotRequired[bool],
```

## CreateLoginProfileRequestUserCreateLoginProfileTypeDef

```python
# CreateLoginProfileRequestUserCreateLoginProfileTypeDef definition

class CreateLoginProfileRequestUserCreateLoginProfileTypeDef(TypedDict):
    Password: NotRequired[str],
    PasswordResetRequired: NotRequired[bool],
```

## LoginProfileTypeDef

```python
# LoginProfileTypeDef definition

class LoginProfileTypeDef(TypedDict):
    UserName: str,
    CreateDate: datetime,
    PasswordResetRequired: NotRequired[bool],
```

## CreatePolicyVersionRequestPolicyCreateVersionTypeDef

```python
# CreatePolicyVersionRequestPolicyCreateVersionTypeDef definition

class CreatePolicyVersionRequestPolicyCreateVersionTypeDef(TypedDict):
    PolicyDocument: str,
    SetAsDefault: NotRequired[bool],
```

## CreatePolicyVersionRequestRequestTypeDef

```python
# CreatePolicyVersionRequestRequestTypeDef definition

class CreatePolicyVersionRequestRequestTypeDef(TypedDict):
    PolicyArn: str,
    PolicyDocument: str,
    SetAsDefault: NotRequired[bool],
```

## CreateServiceLinkedRoleRequestRequestTypeDef

```python
# CreateServiceLinkedRoleRequestRequestTypeDef definition

class CreateServiceLinkedRoleRequestRequestTypeDef(TypedDict):
    AWSServiceName: str,
    Description: NotRequired[str],
    CustomSuffix: NotRequired[str],
```

## CreateServiceSpecificCredentialRequestRequestTypeDef

```python
# CreateServiceSpecificCredentialRequestRequestTypeDef definition

class CreateServiceSpecificCredentialRequestRequestTypeDef(TypedDict):
    UserName: str,
    ServiceName: str,
```

## ServiceSpecificCredentialTypeDef

```python
# ServiceSpecificCredentialTypeDef definition

class ServiceSpecificCredentialTypeDef(TypedDict):
    CreateDate: datetime,
    ServiceName: str,
    ServiceUserName: str,
    ServicePassword: str,
    ServiceSpecificCredentialId: str,
    UserName: str,
    Status: StatusTypeType,  # (1)
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
## DeactivateMFADeviceRequestRequestTypeDef

```python
# DeactivateMFADeviceRequestRequestTypeDef definition

class DeactivateMFADeviceRequestRequestTypeDef(TypedDict):
    SerialNumber: str,
    UserName: NotRequired[str],
```

## DeleteAccessKeyRequestRequestTypeDef

```python
# DeleteAccessKeyRequestRequestTypeDef definition

class DeleteAccessKeyRequestRequestTypeDef(TypedDict):
    AccessKeyId: str,
    UserName: NotRequired[str],
```

## DeleteAccountAliasRequestRequestTypeDef

```python
# DeleteAccountAliasRequestRequestTypeDef definition

class DeleteAccountAliasRequestRequestTypeDef(TypedDict):
    AccountAlias: str,
```

## DeleteGroupPolicyRequestRequestTypeDef

```python
# DeleteGroupPolicyRequestRequestTypeDef definition

class DeleteGroupPolicyRequestRequestTypeDef(TypedDict):
    GroupName: str,
    PolicyName: str,
```

## DeleteGroupRequestRequestTypeDef

```python
# DeleteGroupRequestRequestTypeDef definition

class DeleteGroupRequestRequestTypeDef(TypedDict):
    GroupName: str,
```

## DeleteInstanceProfileRequestRequestTypeDef

```python
# DeleteInstanceProfileRequestRequestTypeDef definition

class DeleteInstanceProfileRequestRequestTypeDef(TypedDict):
    InstanceProfileName: str,
```

## DeleteLoginProfileRequestRequestTypeDef

```python
# DeleteLoginProfileRequestRequestTypeDef definition

class DeleteLoginProfileRequestRequestTypeDef(TypedDict):
    UserName: NotRequired[str],
```

## DeleteOpenIDConnectProviderRequestRequestTypeDef

```python
# DeleteOpenIDConnectProviderRequestRequestTypeDef definition

class DeleteOpenIDConnectProviderRequestRequestTypeDef(TypedDict):
    OpenIDConnectProviderArn: str,
```

## DeletePolicyRequestRequestTypeDef

```python
# DeletePolicyRequestRequestTypeDef definition

class DeletePolicyRequestRequestTypeDef(TypedDict):
    PolicyArn: str,
```

## DeletePolicyVersionRequestRequestTypeDef

```python
# DeletePolicyVersionRequestRequestTypeDef definition

class DeletePolicyVersionRequestRequestTypeDef(TypedDict):
    PolicyArn: str,
    VersionId: str,
```

## DeleteRolePermissionsBoundaryRequestRequestTypeDef

```python
# DeleteRolePermissionsBoundaryRequestRequestTypeDef definition

class DeleteRolePermissionsBoundaryRequestRequestTypeDef(TypedDict):
    RoleName: str,
```

## DeleteRolePolicyRequestRequestTypeDef

```python
# DeleteRolePolicyRequestRequestTypeDef definition

class DeleteRolePolicyRequestRequestTypeDef(TypedDict):
    RoleName: str,
    PolicyName: str,
```

## DeleteRoleRequestRequestTypeDef

```python
# DeleteRoleRequestRequestTypeDef definition

class DeleteRoleRequestRequestTypeDef(TypedDict):
    RoleName: str,
```

## DeleteSAMLProviderRequestRequestTypeDef

```python
# DeleteSAMLProviderRequestRequestTypeDef definition

class DeleteSAMLProviderRequestRequestTypeDef(TypedDict):
    SAMLProviderArn: str,
```

## DeleteSSHPublicKeyRequestRequestTypeDef

```python
# DeleteSSHPublicKeyRequestRequestTypeDef definition

class DeleteSSHPublicKeyRequestRequestTypeDef(TypedDict):
    UserName: str,
    SSHPublicKeyId: str,
```

## DeleteServerCertificateRequestRequestTypeDef

```python
# DeleteServerCertificateRequestRequestTypeDef definition

class DeleteServerCertificateRequestRequestTypeDef(TypedDict):
    ServerCertificateName: str,
```

## DeleteServiceLinkedRoleRequestRequestTypeDef

```python
# DeleteServiceLinkedRoleRequestRequestTypeDef definition

class DeleteServiceLinkedRoleRequestRequestTypeDef(TypedDict):
    RoleName: str,
```

## DeleteServiceSpecificCredentialRequestRequestTypeDef

```python
# DeleteServiceSpecificCredentialRequestRequestTypeDef definition

class DeleteServiceSpecificCredentialRequestRequestTypeDef(TypedDict):
    ServiceSpecificCredentialId: str,
    UserName: NotRequired[str],
```

## DeleteSigningCertificateRequestRequestTypeDef

```python
# DeleteSigningCertificateRequestRequestTypeDef definition

class DeleteSigningCertificateRequestRequestTypeDef(TypedDict):
    CertificateId: str,
    UserName: NotRequired[str],
```

## DeleteUserPermissionsBoundaryRequestRequestTypeDef

```python
# DeleteUserPermissionsBoundaryRequestRequestTypeDef definition

class DeleteUserPermissionsBoundaryRequestRequestTypeDef(TypedDict):
    UserName: str,
```

## DeleteUserPolicyRequestRequestTypeDef

```python
# DeleteUserPolicyRequestRequestTypeDef definition

class DeleteUserPolicyRequestRequestTypeDef(TypedDict):
    UserName: str,
    PolicyName: str,
```

## DeleteUserRequestRequestTypeDef

```python
# DeleteUserRequestRequestTypeDef definition

class DeleteUserRequestRequestTypeDef(TypedDict):
    UserName: str,
```

## DeleteVirtualMFADeviceRequestRequestTypeDef

```python
# DeleteVirtualMFADeviceRequestRequestTypeDef definition

class DeleteVirtualMFADeviceRequestRequestTypeDef(TypedDict):
    SerialNumber: str,
```

## RoleUsageTypeTypeDef

```python
# RoleUsageTypeTypeDef definition

class RoleUsageTypeTypeDef(TypedDict):
    Region: NotRequired[str],
    Resources: NotRequired[List[str]],
```

## DetachGroupPolicyRequestGroupDetachPolicyTypeDef

```python
# DetachGroupPolicyRequestGroupDetachPolicyTypeDef definition

class DetachGroupPolicyRequestGroupDetachPolicyTypeDef(TypedDict):
    PolicyArn: str,
```

## DetachGroupPolicyRequestPolicyDetachGroupTypeDef

```python
# DetachGroupPolicyRequestPolicyDetachGroupTypeDef definition

class DetachGroupPolicyRequestPolicyDetachGroupTypeDef(TypedDict):
    GroupName: str,
```

## DetachGroupPolicyRequestRequestTypeDef

```python
# DetachGroupPolicyRequestRequestTypeDef definition

class DetachGroupPolicyRequestRequestTypeDef(TypedDict):
    GroupName: str,
    PolicyArn: str,
```

## DetachRolePolicyRequestPolicyDetachRoleTypeDef

```python
# DetachRolePolicyRequestPolicyDetachRoleTypeDef definition

class DetachRolePolicyRequestPolicyDetachRoleTypeDef(TypedDict):
    RoleName: str,
```

## DetachRolePolicyRequestRequestTypeDef

```python
# DetachRolePolicyRequestRequestTypeDef definition

class DetachRolePolicyRequestRequestTypeDef(TypedDict):
    RoleName: str,
    PolicyArn: str,
```

## DetachRolePolicyRequestRoleDetachPolicyTypeDef

```python
# DetachRolePolicyRequestRoleDetachPolicyTypeDef definition

class DetachRolePolicyRequestRoleDetachPolicyTypeDef(TypedDict):
    PolicyArn: str,
```

## DetachUserPolicyRequestPolicyDetachUserTypeDef

```python
# DetachUserPolicyRequestPolicyDetachUserTypeDef definition

class DetachUserPolicyRequestPolicyDetachUserTypeDef(TypedDict):
    UserName: str,
```

## DetachUserPolicyRequestRequestTypeDef

```python
# DetachUserPolicyRequestRequestTypeDef definition

class DetachUserPolicyRequestRequestTypeDef(TypedDict):
    UserName: str,
    PolicyArn: str,
```

## DetachUserPolicyRequestUserDetachPolicyTypeDef

```python
# DetachUserPolicyRequestUserDetachPolicyTypeDef definition

class DetachUserPolicyRequestUserDetachPolicyTypeDef(TypedDict):
    PolicyArn: str,
```

## EnableMFADeviceRequestMfaDeviceAssociateTypeDef

```python
# EnableMFADeviceRequestMfaDeviceAssociateTypeDef definition

class EnableMFADeviceRequestMfaDeviceAssociateTypeDef(TypedDict):
    AuthenticationCode1: str,
    AuthenticationCode2: str,
```

## EnableMFADeviceRequestRequestTypeDef

```python
# EnableMFADeviceRequestRequestTypeDef definition

class EnableMFADeviceRequestRequestTypeDef(TypedDict):
    UserName: str,
    SerialNumber: str,
    AuthenticationCode1: str,
    AuthenticationCode2: str,
```

## EnableMFADeviceRequestUserEnableMfaTypeDef

```python
# EnableMFADeviceRequestUserEnableMfaTypeDef definition

class EnableMFADeviceRequestUserEnableMfaTypeDef(TypedDict):
    SerialNumber: str,
    AuthenticationCode1: str,
    AuthenticationCode2: str,
```

## EntityInfoTypeDef

```python
# EntityInfoTypeDef definition

class EntityInfoTypeDef(TypedDict):
    Arn: str,
    Name: str,
    Type: PolicyOwnerEntityTypeType,  # (1)
    Id: str,
    Path: NotRequired[str],
```

1. See [:material-code-brackets: PolicyOwnerEntityTypeType](./literals.md#policyownerentitytypetype) 
## ErrorDetailsTypeDef

```python
# ErrorDetailsTypeDef definition

class ErrorDetailsTypeDef(TypedDict):
    Message: str,
    Code: str,
```

## OrganizationsDecisionDetailTypeDef

```python
# OrganizationsDecisionDetailTypeDef definition

class OrganizationsDecisionDetailTypeDef(TypedDict):
    AllowedByOrganizations: NotRequired[bool],
```

## PermissionsBoundaryDecisionDetailTypeDef

```python
# PermissionsBoundaryDecisionDetailTypeDef definition

class PermissionsBoundaryDecisionDetailTypeDef(TypedDict):
    AllowedByPermissionsBoundary: NotRequired[bool],
```

## GenerateOrganizationsAccessReportRequestRequestTypeDef

```python
# GenerateOrganizationsAccessReportRequestRequestTypeDef definition

class GenerateOrganizationsAccessReportRequestRequestTypeDef(TypedDict):
    EntityPath: str,
    OrganizationsPolicyId: NotRequired[str],
```

## GenerateServiceLastAccessedDetailsRequestRequestTypeDef

```python
# GenerateServiceLastAccessedDetailsRequestRequestTypeDef definition

class GenerateServiceLastAccessedDetailsRequestRequestTypeDef(TypedDict):
    Arn: str,
    Granularity: NotRequired[AccessAdvisorUsageGranularityTypeType],  # (1)
```

1. See [:material-code-brackets: AccessAdvisorUsageGranularityTypeType](./literals.md#accessadvisorusagegranularitytypetype) 
## GetAccessKeyLastUsedRequestRequestTypeDef

```python
# GetAccessKeyLastUsedRequestRequestTypeDef definition

class GetAccessKeyLastUsedRequestRequestTypeDef(TypedDict):
    AccessKeyId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetAccountAuthorizationDetailsRequestRequestTypeDef

```python
# GetAccountAuthorizationDetailsRequestRequestTypeDef definition

class GetAccountAuthorizationDetailsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[Sequence[EntityTypeType]],  # (1)
    MaxItems: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
## PasswordPolicyTypeDef

```python
# PasswordPolicyTypeDef definition

class PasswordPolicyTypeDef(TypedDict):
    MinimumPasswordLength: NotRequired[int],
    RequireSymbols: NotRequired[bool],
    RequireNumbers: NotRequired[bool],
    RequireUppercaseCharacters: NotRequired[bool],
    RequireLowercaseCharacters: NotRequired[bool],
    AllowUsersToChangePassword: NotRequired[bool],
    ExpirePasswords: NotRequired[bool],
    MaxPasswordAge: NotRequired[int],
    PasswordReusePrevention: NotRequired[int],
    HardExpiry: NotRequired[bool],
```

## GetContextKeysForCustomPolicyRequestRequestTypeDef

```python
# GetContextKeysForCustomPolicyRequestRequestTypeDef definition

class GetContextKeysForCustomPolicyRequestRequestTypeDef(TypedDict):
    PolicyInputList: Sequence[str],
```

## GetContextKeysForPrincipalPolicyRequestRequestTypeDef

```python
# GetContextKeysForPrincipalPolicyRequestRequestTypeDef definition

class GetContextKeysForPrincipalPolicyRequestRequestTypeDef(TypedDict):
    PolicySourceArn: str,
    PolicyInputList: NotRequired[Sequence[str]],
```

## GetGroupPolicyRequestRequestTypeDef

```python
# GetGroupPolicyRequestRequestTypeDef definition

class GetGroupPolicyRequestRequestTypeDef(TypedDict):
    GroupName: str,
    PolicyName: str,
```

## GetGroupRequestRequestTypeDef

```python
# GetGroupRequestRequestTypeDef definition

class GetGroupRequestRequestTypeDef(TypedDict):
    GroupName: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## GetInstanceProfileRequestRequestTypeDef

```python
# GetInstanceProfileRequestRequestTypeDef definition

class GetInstanceProfileRequestRequestTypeDef(TypedDict):
    InstanceProfileName: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## GetLoginProfileRequestRequestTypeDef

```python
# GetLoginProfileRequestRequestTypeDef definition

class GetLoginProfileRequestRequestTypeDef(TypedDict):
    UserName: NotRequired[str],
```

## GetMFADeviceRequestRequestTypeDef

```python
# GetMFADeviceRequestRequestTypeDef definition

class GetMFADeviceRequestRequestTypeDef(TypedDict):
    SerialNumber: str,
    UserName: NotRequired[str],
```

## GetOpenIDConnectProviderRequestRequestTypeDef

```python
# GetOpenIDConnectProviderRequestRequestTypeDef definition

class GetOpenIDConnectProviderRequestRequestTypeDef(TypedDict):
    OpenIDConnectProviderArn: str,
```

## GetOrganizationsAccessReportRequestRequestTypeDef

```python
# GetOrganizationsAccessReportRequestRequestTypeDef definition

class GetOrganizationsAccessReportRequestRequestTypeDef(TypedDict):
    JobId: str,
    MaxItems: NotRequired[int],
    Marker: NotRequired[str],
    SortKey: NotRequired[SortKeyTypeType],  # (1)
```

1. See [:material-code-brackets: SortKeyTypeType](./literals.md#sortkeytypetype) 
## GetPolicyRequestRequestTypeDef

```python
# GetPolicyRequestRequestTypeDef definition

class GetPolicyRequestRequestTypeDef(TypedDict):
    PolicyArn: str,
```

## GetPolicyVersionRequestRequestTypeDef

```python
# GetPolicyVersionRequestRequestTypeDef definition

class GetPolicyVersionRequestRequestTypeDef(TypedDict):
    PolicyArn: str,
    VersionId: str,
```

## GetRolePolicyRequestRequestTypeDef

```python
# GetRolePolicyRequestRequestTypeDef definition

class GetRolePolicyRequestRequestTypeDef(TypedDict):
    RoleName: str,
    PolicyName: str,
```

## GetRoleRequestRequestTypeDef

```python
# GetRoleRequestRequestTypeDef definition

class GetRoleRequestRequestTypeDef(TypedDict):
    RoleName: str,
```

## GetSAMLProviderRequestRequestTypeDef

```python
# GetSAMLProviderRequestRequestTypeDef definition

class GetSAMLProviderRequestRequestTypeDef(TypedDict):
    SAMLProviderArn: str,
```

## GetSSHPublicKeyRequestRequestTypeDef

```python
# GetSSHPublicKeyRequestRequestTypeDef definition

class GetSSHPublicKeyRequestRequestTypeDef(TypedDict):
    UserName: str,
    SSHPublicKeyId: str,
    Encoding: EncodingTypeType,  # (1)
```

1. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
## SSHPublicKeyTypeDef

```python
# SSHPublicKeyTypeDef definition

class SSHPublicKeyTypeDef(TypedDict):
    UserName: str,
    SSHPublicKeyId: str,
    Fingerprint: str,
    SSHPublicKeyBody: str,
    Status: StatusTypeType,  # (1)
    UploadDate: NotRequired[datetime],
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
## GetServerCertificateRequestRequestTypeDef

```python
# GetServerCertificateRequestRequestTypeDef definition

class GetServerCertificateRequestRequestTypeDef(TypedDict):
    ServerCertificateName: str,
```

## GetServiceLastAccessedDetailsRequestRequestTypeDef

```python
# GetServiceLastAccessedDetailsRequestRequestTypeDef definition

class GetServiceLastAccessedDetailsRequestRequestTypeDef(TypedDict):
    JobId: str,
    MaxItems: NotRequired[int],
    Marker: NotRequired[str],
```

## GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef

```python
# GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef definition

class GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef(TypedDict):
    JobId: str,
    ServiceNamespace: str,
    MaxItems: NotRequired[int],
    Marker: NotRequired[str],
```

## GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef

```python
# GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef definition

class GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef(TypedDict):
    DeletionTaskId: str,
```

## GetUserPolicyRequestRequestTypeDef

```python
# GetUserPolicyRequestRequestTypeDef definition

class GetUserPolicyRequestRequestTypeDef(TypedDict):
    UserName: str,
    PolicyName: str,
```

## GetUserRequestRequestTypeDef

```python
# GetUserRequestRequestTypeDef definition

class GetUserRequestRequestTypeDef(TypedDict):
    UserName: NotRequired[str],
```

## ListAccessKeysRequestRequestTypeDef

```python
# ListAccessKeysRequestRequestTypeDef definition

class ListAccessKeysRequestRequestTypeDef(TypedDict):
    UserName: NotRequired[str],
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListAccountAliasesRequestRequestTypeDef

```python
# ListAccountAliasesRequestRequestTypeDef definition

class ListAccountAliasesRequestRequestTypeDef(TypedDict):
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListAttachedGroupPoliciesRequestRequestTypeDef

```python
# ListAttachedGroupPoliciesRequestRequestTypeDef definition

class ListAttachedGroupPoliciesRequestRequestTypeDef(TypedDict):
    GroupName: str,
    PathPrefix: NotRequired[str],
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListAttachedRolePoliciesRequestRequestTypeDef

```python
# ListAttachedRolePoliciesRequestRequestTypeDef definition

class ListAttachedRolePoliciesRequestRequestTypeDef(TypedDict):
    RoleName: str,
    PathPrefix: NotRequired[str],
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListAttachedUserPoliciesRequestRequestTypeDef

```python
# ListAttachedUserPoliciesRequestRequestTypeDef definition

class ListAttachedUserPoliciesRequestRequestTypeDef(TypedDict):
    UserName: str,
    PathPrefix: NotRequired[str],
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListEntitiesForPolicyRequestRequestTypeDef

```python
# ListEntitiesForPolicyRequestRequestTypeDef definition

class ListEntitiesForPolicyRequestRequestTypeDef(TypedDict):
    PolicyArn: str,
    EntityFilter: NotRequired[EntityTypeType],  # (1)
    PathPrefix: NotRequired[str],
    PolicyUsageFilter: NotRequired[PolicyUsageTypeType],  # (2)
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
2. See [:material-code-brackets: PolicyUsageTypeType](./literals.md#policyusagetypetype) 
## PolicyGroupTypeDef

```python
# PolicyGroupTypeDef definition

class PolicyGroupTypeDef(TypedDict):
    GroupName: NotRequired[str],
    GroupId: NotRequired[str],
```

## PolicyRoleTypeDef

```python
# PolicyRoleTypeDef definition

class PolicyRoleTypeDef(TypedDict):
    RoleName: NotRequired[str],
    RoleId: NotRequired[str],
```

## PolicyUserTypeDef

```python
# PolicyUserTypeDef definition

class PolicyUserTypeDef(TypedDict):
    UserName: NotRequired[str],
    UserId: NotRequired[str],
```

## ListGroupPoliciesRequestRequestTypeDef

```python
# ListGroupPoliciesRequestRequestTypeDef definition

class ListGroupPoliciesRequestRequestTypeDef(TypedDict):
    GroupName: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListGroupsForUserRequestRequestTypeDef

```python
# ListGroupsForUserRequestRequestTypeDef definition

class ListGroupsForUserRequestRequestTypeDef(TypedDict):
    UserName: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListGroupsRequestRequestTypeDef

```python
# ListGroupsRequestRequestTypeDef definition

class ListGroupsRequestRequestTypeDef(TypedDict):
    PathPrefix: NotRequired[str],
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListInstanceProfileTagsRequestRequestTypeDef

```python
# ListInstanceProfileTagsRequestRequestTypeDef definition

class ListInstanceProfileTagsRequestRequestTypeDef(TypedDict):
    InstanceProfileName: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListInstanceProfilesForRoleRequestRequestTypeDef

```python
# ListInstanceProfilesForRoleRequestRequestTypeDef definition

class ListInstanceProfilesForRoleRequestRequestTypeDef(TypedDict):
    RoleName: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListInstanceProfilesRequestRequestTypeDef

```python
# ListInstanceProfilesRequestRequestTypeDef definition

class ListInstanceProfilesRequestRequestTypeDef(TypedDict):
    PathPrefix: NotRequired[str],
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListMFADeviceTagsRequestRequestTypeDef

```python
# ListMFADeviceTagsRequestRequestTypeDef definition

class ListMFADeviceTagsRequestRequestTypeDef(TypedDict):
    SerialNumber: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListMFADevicesRequestRequestTypeDef

```python
# ListMFADevicesRequestRequestTypeDef definition

class ListMFADevicesRequestRequestTypeDef(TypedDict):
    UserName: NotRequired[str],
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## MFADeviceTypeDef

```python
# MFADeviceTypeDef definition

class MFADeviceTypeDef(TypedDict):
    UserName: str,
    SerialNumber: str,
    EnableDate: datetime,
```

## ListOpenIDConnectProviderTagsRequestRequestTypeDef

```python
# ListOpenIDConnectProviderTagsRequestRequestTypeDef definition

class ListOpenIDConnectProviderTagsRequestRequestTypeDef(TypedDict):
    OpenIDConnectProviderArn: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## OpenIDConnectProviderListEntryTypeDef

```python
# OpenIDConnectProviderListEntryTypeDef definition

class OpenIDConnectProviderListEntryTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## PolicyGrantingServiceAccessTypeDef

```python
# PolicyGrantingServiceAccessTypeDef definition

class PolicyGrantingServiceAccessTypeDef(TypedDict):
    PolicyName: str,
    PolicyType: PolicyTypeType,  # (1)
    PolicyArn: NotRequired[str],
    EntityType: NotRequired[PolicyOwnerEntityTypeType],  # (2)
    EntityName: NotRequired[str],
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-brackets: PolicyOwnerEntityTypeType](./literals.md#policyownerentitytypetype) 
## ListPoliciesGrantingServiceAccessRequestRequestTypeDef

```python
# ListPoliciesGrantingServiceAccessRequestRequestTypeDef definition

class ListPoliciesGrantingServiceAccessRequestRequestTypeDef(TypedDict):
    Arn: str,
    ServiceNamespaces: Sequence[str],
    Marker: NotRequired[str],
```

## ListPoliciesRequestRequestTypeDef

```python
# ListPoliciesRequestRequestTypeDef definition

class ListPoliciesRequestRequestTypeDef(TypedDict):
    Scope: NotRequired[PolicyScopeTypeType],  # (1)
    OnlyAttached: NotRequired[bool],
    PathPrefix: NotRequired[str],
    PolicyUsageFilter: NotRequired[PolicyUsageTypeType],  # (2)
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

1. See [:material-code-brackets: PolicyScopeTypeType](./literals.md#policyscopetypetype) 
2. See [:material-code-brackets: PolicyUsageTypeType](./literals.md#policyusagetypetype) 
## ListPolicyTagsRequestRequestTypeDef

```python
# ListPolicyTagsRequestRequestTypeDef definition

class ListPolicyTagsRequestRequestTypeDef(TypedDict):
    PolicyArn: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListPolicyVersionsRequestRequestTypeDef

```python
# ListPolicyVersionsRequestRequestTypeDef definition

class ListPolicyVersionsRequestRequestTypeDef(TypedDict):
    PolicyArn: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListRolePoliciesRequestRequestTypeDef

```python
# ListRolePoliciesRequestRequestTypeDef definition

class ListRolePoliciesRequestRequestTypeDef(TypedDict):
    RoleName: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListRoleTagsRequestRequestTypeDef

```python
# ListRoleTagsRequestRequestTypeDef definition

class ListRoleTagsRequestRequestTypeDef(TypedDict):
    RoleName: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListRolesRequestRequestTypeDef

```python
# ListRolesRequestRequestTypeDef definition

class ListRolesRequestRequestTypeDef(TypedDict):
    PathPrefix: NotRequired[str],
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListSAMLProviderTagsRequestRequestTypeDef

```python
# ListSAMLProviderTagsRequestRequestTypeDef definition

class ListSAMLProviderTagsRequestRequestTypeDef(TypedDict):
    SAMLProviderArn: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## SAMLProviderListEntryTypeDef

```python
# SAMLProviderListEntryTypeDef definition

class SAMLProviderListEntryTypeDef(TypedDict):
    Arn: NotRequired[str],
    ValidUntil: NotRequired[datetime],
    CreateDate: NotRequired[datetime],
```

## ListSSHPublicKeysRequestRequestTypeDef

```python
# ListSSHPublicKeysRequestRequestTypeDef definition

class ListSSHPublicKeysRequestRequestTypeDef(TypedDict):
    UserName: NotRequired[str],
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## SSHPublicKeyMetadataTypeDef

```python
# SSHPublicKeyMetadataTypeDef definition

class SSHPublicKeyMetadataTypeDef(TypedDict):
    UserName: str,
    SSHPublicKeyId: str,
    Status: StatusTypeType,  # (1)
    UploadDate: datetime,
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
## ListServerCertificateTagsRequestRequestTypeDef

```python
# ListServerCertificateTagsRequestRequestTypeDef definition

class ListServerCertificateTagsRequestRequestTypeDef(TypedDict):
    ServerCertificateName: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListServerCertificatesRequestRequestTypeDef

```python
# ListServerCertificatesRequestRequestTypeDef definition

class ListServerCertificatesRequestRequestTypeDef(TypedDict):
    PathPrefix: NotRequired[str],
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ServerCertificateMetadataTypeDef

```python
# ServerCertificateMetadataTypeDef definition

class ServerCertificateMetadataTypeDef(TypedDict):
    Path: str,
    ServerCertificateName: str,
    ServerCertificateId: str,
    Arn: str,
    UploadDate: NotRequired[datetime],
    Expiration: NotRequired[datetime],
```

## ListServiceSpecificCredentialsRequestRequestTypeDef

```python
# ListServiceSpecificCredentialsRequestRequestTypeDef definition

class ListServiceSpecificCredentialsRequestRequestTypeDef(TypedDict):
    UserName: NotRequired[str],
    ServiceName: NotRequired[str],
```

## ServiceSpecificCredentialMetadataTypeDef

```python
# ServiceSpecificCredentialMetadataTypeDef definition

class ServiceSpecificCredentialMetadataTypeDef(TypedDict):
    UserName: str,
    Status: StatusTypeType,  # (1)
    ServiceUserName: str,
    CreateDate: datetime,
    ServiceSpecificCredentialId: str,
    ServiceName: str,
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
## ListSigningCertificatesRequestRequestTypeDef

```python
# ListSigningCertificatesRequestRequestTypeDef definition

class ListSigningCertificatesRequestRequestTypeDef(TypedDict):
    UserName: NotRequired[str],
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## SigningCertificateTypeDef

```python
# SigningCertificateTypeDef definition

class SigningCertificateTypeDef(TypedDict):
    UserName: str,
    CertificateId: str,
    CertificateBody: str,
    Status: StatusTypeType,  # (1)
    UploadDate: NotRequired[datetime],
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
## ListUserPoliciesRequestRequestTypeDef

```python
# ListUserPoliciesRequestRequestTypeDef definition

class ListUserPoliciesRequestRequestTypeDef(TypedDict):
    UserName: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListUserTagsRequestRequestTypeDef

```python
# ListUserTagsRequestRequestTypeDef definition

class ListUserTagsRequestRequestTypeDef(TypedDict):
    UserName: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListUsersRequestRequestTypeDef

```python
# ListUsersRequestRequestTypeDef definition

class ListUsersRequestRequestTypeDef(TypedDict):
    PathPrefix: NotRequired[str],
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListVirtualMFADevicesRequestRequestTypeDef

```python
# ListVirtualMFADevicesRequestRequestTypeDef definition

class ListVirtualMFADevicesRequestRequestTypeDef(TypedDict):
    AssignmentStatus: NotRequired[AssignmentStatusTypeType],  # (1)
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

1. See [:material-code-brackets: AssignmentStatusTypeType](./literals.md#assignmentstatustypetype) 
## PolicyDocumentStatementTypeDef

```python
# PolicyDocumentStatementTypeDef definition

class PolicyDocumentStatementTypeDef(TypedDict):
    Effect: str,
    Resource: Union[str, List[str]],
    Sid: str,
    Action: Union[str, List[str]],
```

## PositionTypeDef

```python
# PositionTypeDef definition

class PositionTypeDef(TypedDict):
    Line: NotRequired[int],
    Column: NotRequired[int],
```

## PutGroupPolicyRequestGroupCreatePolicyTypeDef

```python
# PutGroupPolicyRequestGroupCreatePolicyTypeDef definition

class PutGroupPolicyRequestGroupCreatePolicyTypeDef(TypedDict):
    PolicyName: str,
    PolicyDocument: str,
```

## PutGroupPolicyRequestGroupPolicyPutTypeDef

```python
# PutGroupPolicyRequestGroupPolicyPutTypeDef definition

class PutGroupPolicyRequestGroupPolicyPutTypeDef(TypedDict):
    PolicyDocument: str,
```

## PutGroupPolicyRequestRequestTypeDef

```python
# PutGroupPolicyRequestRequestTypeDef definition

class PutGroupPolicyRequestRequestTypeDef(TypedDict):
    GroupName: str,
    PolicyName: str,
    PolicyDocument: str,
```

## PutRolePermissionsBoundaryRequestRequestTypeDef

```python
# PutRolePermissionsBoundaryRequestRequestTypeDef definition

class PutRolePermissionsBoundaryRequestRequestTypeDef(TypedDict):
    RoleName: str,
    PermissionsBoundary: str,
```

## PutRolePolicyRequestRequestTypeDef

```python
# PutRolePolicyRequestRequestTypeDef definition

class PutRolePolicyRequestRequestTypeDef(TypedDict):
    RoleName: str,
    PolicyName: str,
    PolicyDocument: str,
```

## PutRolePolicyRequestRolePolicyPutTypeDef

```python
# PutRolePolicyRequestRolePolicyPutTypeDef definition

class PutRolePolicyRequestRolePolicyPutTypeDef(TypedDict):
    PolicyDocument: str,
```

## PutUserPermissionsBoundaryRequestRequestTypeDef

```python
# PutUserPermissionsBoundaryRequestRequestTypeDef definition

class PutUserPermissionsBoundaryRequestRequestTypeDef(TypedDict):
    UserName: str,
    PermissionsBoundary: str,
```

## PutUserPolicyRequestRequestTypeDef

```python
# PutUserPolicyRequestRequestTypeDef definition

class PutUserPolicyRequestRequestTypeDef(TypedDict):
    UserName: str,
    PolicyName: str,
    PolicyDocument: str,
```

## PutUserPolicyRequestUserCreatePolicyTypeDef

```python
# PutUserPolicyRequestUserCreatePolicyTypeDef definition

class PutUserPolicyRequestUserCreatePolicyTypeDef(TypedDict):
    PolicyName: str,
    PolicyDocument: str,
```

## PutUserPolicyRequestUserPolicyPutTypeDef

```python
# PutUserPolicyRequestUserPolicyPutTypeDef definition

class PutUserPolicyRequestUserPolicyPutTypeDef(TypedDict):
    PolicyDocument: str,
```

## RemoveClientIDFromOpenIDConnectProviderRequestRequestTypeDef

```python
# RemoveClientIDFromOpenIDConnectProviderRequestRequestTypeDef definition

class RemoveClientIDFromOpenIDConnectProviderRequestRequestTypeDef(TypedDict):
    OpenIDConnectProviderArn: str,
    ClientID: str,
```

## RemoveRoleFromInstanceProfileRequestInstanceProfileRemoveRoleTypeDef

```python
# RemoveRoleFromInstanceProfileRequestInstanceProfileRemoveRoleTypeDef definition

class RemoveRoleFromInstanceProfileRequestInstanceProfileRemoveRoleTypeDef(TypedDict):
    RoleName: str,
```

## RemoveRoleFromInstanceProfileRequestRequestTypeDef

```python
# RemoveRoleFromInstanceProfileRequestRequestTypeDef definition

class RemoveRoleFromInstanceProfileRequestRequestTypeDef(TypedDict):
    InstanceProfileName: str,
    RoleName: str,
```

## RemoveUserFromGroupRequestGroupRemoveUserTypeDef

```python
# RemoveUserFromGroupRequestGroupRemoveUserTypeDef definition

class RemoveUserFromGroupRequestGroupRemoveUserTypeDef(TypedDict):
    UserName: str,
```

## RemoveUserFromGroupRequestRequestTypeDef

```python
# RemoveUserFromGroupRequestRequestTypeDef definition

class RemoveUserFromGroupRequestRequestTypeDef(TypedDict):
    GroupName: str,
    UserName: str,
```

## RemoveUserFromGroupRequestUserRemoveGroupTypeDef

```python
# RemoveUserFromGroupRequestUserRemoveGroupTypeDef definition

class RemoveUserFromGroupRequestUserRemoveGroupTypeDef(TypedDict):
    GroupName: str,
```

## ResetServiceSpecificCredentialRequestRequestTypeDef

```python
# ResetServiceSpecificCredentialRequestRequestTypeDef definition

class ResetServiceSpecificCredentialRequestRequestTypeDef(TypedDict):
    ServiceSpecificCredentialId: str,
    UserName: NotRequired[str],
```

## ResyncMFADeviceRequestMfaDeviceResyncTypeDef

```python
# ResyncMFADeviceRequestMfaDeviceResyncTypeDef definition

class ResyncMFADeviceRequestMfaDeviceResyncTypeDef(TypedDict):
    AuthenticationCode1: str,
    AuthenticationCode2: str,
```

## ResyncMFADeviceRequestRequestTypeDef

```python
# ResyncMFADeviceRequestRequestTypeDef definition

class ResyncMFADeviceRequestRequestTypeDef(TypedDict):
    UserName: str,
    SerialNumber: str,
    AuthenticationCode1: str,
    AuthenticationCode2: str,
```

## RoleLastUsedTypeDef

```python
# RoleLastUsedTypeDef definition

class RoleLastUsedTypeDef(TypedDict):
    LastUsedDate: NotRequired[datetime],
    Region: NotRequired[str],
```

## TrackedActionLastAccessedTypeDef

```python
# TrackedActionLastAccessedTypeDef definition

class TrackedActionLastAccessedTypeDef(TypedDict):
    ActionName: NotRequired[str],
    LastAccessedEntity: NotRequired[str],
    LastAccessedTime: NotRequired[datetime],
    LastAccessedRegion: NotRequired[str],
```

## SetDefaultPolicyVersionRequestRequestTypeDef

```python
# SetDefaultPolicyVersionRequestRequestTypeDef definition

class SetDefaultPolicyVersionRequestRequestTypeDef(TypedDict):
    PolicyArn: str,
    VersionId: str,
```

## SetSecurityTokenServicePreferencesRequestRequestTypeDef

```python
# SetSecurityTokenServicePreferencesRequestRequestTypeDef definition

class SetSecurityTokenServicePreferencesRequestRequestTypeDef(TypedDict):
    GlobalEndpointTokenVersion: GlobalEndpointTokenVersionType,  # (1)
```

1. See [:material-code-brackets: GlobalEndpointTokenVersionType](./literals.md#globalendpointtokenversiontype) 
## UntagInstanceProfileRequestRequestTypeDef

```python
# UntagInstanceProfileRequestRequestTypeDef definition

class UntagInstanceProfileRequestRequestTypeDef(TypedDict):
    InstanceProfileName: str,
    TagKeys: Sequence[str],
```

## UntagMFADeviceRequestRequestTypeDef

```python
# UntagMFADeviceRequestRequestTypeDef definition

class UntagMFADeviceRequestRequestTypeDef(TypedDict):
    SerialNumber: str,
    TagKeys: Sequence[str],
```

## UntagOpenIDConnectProviderRequestRequestTypeDef

```python
# UntagOpenIDConnectProviderRequestRequestTypeDef definition

class UntagOpenIDConnectProviderRequestRequestTypeDef(TypedDict):
    OpenIDConnectProviderArn: str,
    TagKeys: Sequence[str],
```

## UntagPolicyRequestRequestTypeDef

```python
# UntagPolicyRequestRequestTypeDef definition

class UntagPolicyRequestRequestTypeDef(TypedDict):
    PolicyArn: str,
    TagKeys: Sequence[str],
```

## UntagRoleRequestRequestTypeDef

```python
# UntagRoleRequestRequestTypeDef definition

class UntagRoleRequestRequestTypeDef(TypedDict):
    RoleName: str,
    TagKeys: Sequence[str],
```

## UntagSAMLProviderRequestRequestTypeDef

```python
# UntagSAMLProviderRequestRequestTypeDef definition

class UntagSAMLProviderRequestRequestTypeDef(TypedDict):
    SAMLProviderArn: str,
    TagKeys: Sequence[str],
```

## UntagServerCertificateRequestRequestTypeDef

```python
# UntagServerCertificateRequestRequestTypeDef definition

class UntagServerCertificateRequestRequestTypeDef(TypedDict):
    ServerCertificateName: str,
    TagKeys: Sequence[str],
```

## UntagUserRequestRequestTypeDef

```python
# UntagUserRequestRequestTypeDef definition

class UntagUserRequestRequestTypeDef(TypedDict):
    UserName: str,
    TagKeys: Sequence[str],
```

## UpdateAccessKeyRequestAccessKeyActivateTypeDef

```python
# UpdateAccessKeyRequestAccessKeyActivateTypeDef definition

class UpdateAccessKeyRequestAccessKeyActivateTypeDef(TypedDict):
    Status: NotRequired[StatusTypeType],  # (1)
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
## UpdateAccessKeyRequestAccessKeyDeactivateTypeDef

```python
# UpdateAccessKeyRequestAccessKeyDeactivateTypeDef definition

class UpdateAccessKeyRequestAccessKeyDeactivateTypeDef(TypedDict):
    Status: NotRequired[StatusTypeType],  # (1)
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
## UpdateAccessKeyRequestAccessKeyPairActivateTypeDef

```python
# UpdateAccessKeyRequestAccessKeyPairActivateTypeDef definition

class UpdateAccessKeyRequestAccessKeyPairActivateTypeDef(TypedDict):
    Status: NotRequired[StatusTypeType],  # (1)
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
## UpdateAccessKeyRequestAccessKeyPairDeactivateTypeDef

```python
# UpdateAccessKeyRequestAccessKeyPairDeactivateTypeDef definition

class UpdateAccessKeyRequestAccessKeyPairDeactivateTypeDef(TypedDict):
    Status: NotRequired[StatusTypeType],  # (1)
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
## UpdateAccessKeyRequestRequestTypeDef

```python
# UpdateAccessKeyRequestRequestTypeDef definition

class UpdateAccessKeyRequestRequestTypeDef(TypedDict):
    AccessKeyId: str,
    Status: StatusTypeType,  # (1)
    UserName: NotRequired[str],
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
## UpdateAccountPasswordPolicyRequestAccountPasswordPolicyUpdateTypeDef

```python
# UpdateAccountPasswordPolicyRequestAccountPasswordPolicyUpdateTypeDef definition

class UpdateAccountPasswordPolicyRequestAccountPasswordPolicyUpdateTypeDef(TypedDict):
    MinimumPasswordLength: NotRequired[int],
    RequireSymbols: NotRequired[bool],
    RequireNumbers: NotRequired[bool],
    RequireUppercaseCharacters: NotRequired[bool],
    RequireLowercaseCharacters: NotRequired[bool],
    AllowUsersToChangePassword: NotRequired[bool],
    MaxPasswordAge: NotRequired[int],
    PasswordReusePrevention: NotRequired[int],
    HardExpiry: NotRequired[bool],
```

## UpdateAccountPasswordPolicyRequestRequestTypeDef

```python
# UpdateAccountPasswordPolicyRequestRequestTypeDef definition

class UpdateAccountPasswordPolicyRequestRequestTypeDef(TypedDict):
    MinimumPasswordLength: NotRequired[int],
    RequireSymbols: NotRequired[bool],
    RequireNumbers: NotRequired[bool],
    RequireUppercaseCharacters: NotRequired[bool],
    RequireLowercaseCharacters: NotRequired[bool],
    AllowUsersToChangePassword: NotRequired[bool],
    MaxPasswordAge: NotRequired[int],
    PasswordReusePrevention: NotRequired[int],
    HardExpiry: NotRequired[bool],
```

## UpdateAccountPasswordPolicyRequestServiceResourceCreateAccountPasswordPolicyTypeDef

```python
# UpdateAccountPasswordPolicyRequestServiceResourceCreateAccountPasswordPolicyTypeDef definition

class UpdateAccountPasswordPolicyRequestServiceResourceCreateAccountPasswordPolicyTypeDef(TypedDict):
    MinimumPasswordLength: NotRequired[int],
    RequireSymbols: NotRequired[bool],
    RequireNumbers: NotRequired[bool],
    RequireUppercaseCharacters: NotRequired[bool],
    RequireLowercaseCharacters: NotRequired[bool],
    AllowUsersToChangePassword: NotRequired[bool],
    MaxPasswordAge: NotRequired[int],
    PasswordReusePrevention: NotRequired[int],
    HardExpiry: NotRequired[bool],
```

## UpdateAssumeRolePolicyRequestAssumeRolePolicyUpdateTypeDef

```python
# UpdateAssumeRolePolicyRequestAssumeRolePolicyUpdateTypeDef definition

class UpdateAssumeRolePolicyRequestAssumeRolePolicyUpdateTypeDef(TypedDict):
    PolicyDocument: str,
```

## UpdateAssumeRolePolicyRequestRequestTypeDef

```python
# UpdateAssumeRolePolicyRequestRequestTypeDef definition

class UpdateAssumeRolePolicyRequestRequestTypeDef(TypedDict):
    RoleName: str,
    PolicyDocument: str,
```

## UpdateGroupRequestGroupUpdateTypeDef

```python
# UpdateGroupRequestGroupUpdateTypeDef definition

class UpdateGroupRequestGroupUpdateTypeDef(TypedDict):
    NewPath: NotRequired[str],
    NewGroupName: NotRequired[str],
```

## UpdateGroupRequestRequestTypeDef

```python
# UpdateGroupRequestRequestTypeDef definition

class UpdateGroupRequestRequestTypeDef(TypedDict):
    GroupName: str,
    NewPath: NotRequired[str],
    NewGroupName: NotRequired[str],
```

## UpdateLoginProfileRequestLoginProfileUpdateTypeDef

```python
# UpdateLoginProfileRequestLoginProfileUpdateTypeDef definition

class UpdateLoginProfileRequestLoginProfileUpdateTypeDef(TypedDict):
    Password: NotRequired[str],
    PasswordResetRequired: NotRequired[bool],
```

## UpdateLoginProfileRequestRequestTypeDef

```python
# UpdateLoginProfileRequestRequestTypeDef definition

class UpdateLoginProfileRequestRequestTypeDef(TypedDict):
    UserName: str,
    Password: NotRequired[str],
    PasswordResetRequired: NotRequired[bool],
```

## UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef

```python
# UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef definition

class UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef(TypedDict):
    OpenIDConnectProviderArn: str,
    ThumbprintList: Sequence[str],
```

## UpdateRoleDescriptionRequestRequestTypeDef

```python
# UpdateRoleDescriptionRequestRequestTypeDef definition

class UpdateRoleDescriptionRequestRequestTypeDef(TypedDict):
    RoleName: str,
    Description: str,
```

## UpdateRoleRequestRequestTypeDef

```python
# UpdateRoleRequestRequestTypeDef definition

class UpdateRoleRequestRequestTypeDef(TypedDict):
    RoleName: str,
    Description: NotRequired[str],
    MaxSessionDuration: NotRequired[int],
```

## UpdateSAMLProviderRequestRequestTypeDef

```python
# UpdateSAMLProviderRequestRequestTypeDef definition

class UpdateSAMLProviderRequestRequestTypeDef(TypedDict):
    SAMLMetadataDocument: str,
    SAMLProviderArn: str,
```

## UpdateSAMLProviderRequestSamlProviderUpdateTypeDef

```python
# UpdateSAMLProviderRequestSamlProviderUpdateTypeDef definition

class UpdateSAMLProviderRequestSamlProviderUpdateTypeDef(TypedDict):
    SAMLMetadataDocument: str,
```

## UpdateSSHPublicKeyRequestRequestTypeDef

```python
# UpdateSSHPublicKeyRequestRequestTypeDef definition

class UpdateSSHPublicKeyRequestRequestTypeDef(TypedDict):
    UserName: str,
    SSHPublicKeyId: str,
    Status: StatusTypeType,  # (1)
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
## UpdateServerCertificateRequestRequestTypeDef

```python
# UpdateServerCertificateRequestRequestTypeDef definition

class UpdateServerCertificateRequestRequestTypeDef(TypedDict):
    ServerCertificateName: str,
    NewPath: NotRequired[str],
    NewServerCertificateName: NotRequired[str],
```

## UpdateServerCertificateRequestServerCertificateUpdateTypeDef

```python
# UpdateServerCertificateRequestServerCertificateUpdateTypeDef definition

class UpdateServerCertificateRequestServerCertificateUpdateTypeDef(TypedDict):
    NewPath: NotRequired[str],
    NewServerCertificateName: NotRequired[str],
```

## UpdateServiceSpecificCredentialRequestRequestTypeDef

```python
# UpdateServiceSpecificCredentialRequestRequestTypeDef definition

class UpdateServiceSpecificCredentialRequestRequestTypeDef(TypedDict):
    ServiceSpecificCredentialId: str,
    Status: StatusTypeType,  # (1)
    UserName: NotRequired[str],
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
## UpdateSigningCertificateRequestRequestTypeDef

```python
# UpdateSigningCertificateRequestRequestTypeDef definition

class UpdateSigningCertificateRequestRequestTypeDef(TypedDict):
    CertificateId: str,
    Status: StatusTypeType,  # (1)
    UserName: NotRequired[str],
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
## UpdateSigningCertificateRequestSigningCertificateActivateTypeDef

```python
# UpdateSigningCertificateRequestSigningCertificateActivateTypeDef definition

class UpdateSigningCertificateRequestSigningCertificateActivateTypeDef(TypedDict):
    Status: NotRequired[StatusTypeType],  # (1)
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
## UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef

```python
# UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef definition

class UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef(TypedDict):
    Status: NotRequired[StatusTypeType],  # (1)
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
## UpdateUserRequestRequestTypeDef

```python
# UpdateUserRequestRequestTypeDef definition

class UpdateUserRequestRequestTypeDef(TypedDict):
    UserName: str,
    NewPath: NotRequired[str],
    NewUserName: NotRequired[str],
```

## UpdateUserRequestUserUpdateTypeDef

```python
# UpdateUserRequestUserUpdateTypeDef definition

class UpdateUserRequestUserUpdateTypeDef(TypedDict):
    NewPath: NotRequired[str],
    NewUserName: NotRequired[str],
```

## UploadSSHPublicKeyRequestRequestTypeDef

```python
# UploadSSHPublicKeyRequestRequestTypeDef definition

class UploadSSHPublicKeyRequestRequestTypeDef(TypedDict):
    UserName: str,
    SSHPublicKeyBody: str,
```

## UploadSigningCertificateRequestRequestTypeDef

```python
# UploadSigningCertificateRequestRequestTypeDef definition

class UploadSigningCertificateRequestRequestTypeDef(TypedDict):
    CertificateBody: str,
    UserName: NotRequired[str],
```

## UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef

```python
# UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef definition

class UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef(TypedDict):
    CertificateBody: str,
    UserName: NotRequired[str],
```

## SimulateCustomPolicyRequestRequestTypeDef

```python
# SimulateCustomPolicyRequestRequestTypeDef definition

class SimulateCustomPolicyRequestRequestTypeDef(TypedDict):
    PolicyInputList: Sequence[str],
    ActionNames: Sequence[str],
    PermissionsBoundaryPolicyInputList: NotRequired[Sequence[str]],
    ResourceArns: NotRequired[Sequence[str]],
    ResourcePolicy: NotRequired[str],
    ResourceOwner: NotRequired[str],
    CallerArn: NotRequired[str],
    ContextEntries: NotRequired[Sequence[ContextEntryTypeDef]],  # (1)
    ResourceHandlingOption: NotRequired[str],
    MaxItems: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: ContextEntryTypeDef](./type_defs.md#contextentrytypedef) 
## SimulatePrincipalPolicyRequestRequestTypeDef

```python
# SimulatePrincipalPolicyRequestRequestTypeDef definition

class SimulatePrincipalPolicyRequestRequestTypeDef(TypedDict):
    PolicySourceArn: str,
    ActionNames: Sequence[str],
    PolicyInputList: NotRequired[Sequence[str]],
    PermissionsBoundaryPolicyInputList: NotRequired[Sequence[str]],
    ResourceArns: NotRequired[Sequence[str]],
    ResourcePolicy: NotRequired[str],
    ResourceOwner: NotRequired[str],
    CallerArn: NotRequired[str],
    ContextEntries: NotRequired[Sequence[ContextEntryTypeDef]],  # (1)
    ResourceHandlingOption: NotRequired[str],
    MaxItems: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: ContextEntryTypeDef](./type_defs.md#contextentrytypedef) 
## CreateAccessKeyResponseTypeDef

```python
# CreateAccessKeyResponseTypeDef definition

class CreateAccessKeyResponseTypeDef(TypedDict):
    AccessKey: AccessKeyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccessKeyTypeDef](./type_defs.md#accesskeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteServiceLinkedRoleResponseTypeDef

```python
# DeleteServiceLinkedRoleResponseTypeDef definition

class DeleteServiceLinkedRoleResponseTypeDef(TypedDict):
    DeletionTaskId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisableOrganizationsRootCredentialsManagementResponseTypeDef

```python
# DisableOrganizationsRootCredentialsManagementResponseTypeDef definition

class DisableOrganizationsRootCredentialsManagementResponseTypeDef(TypedDict):
    OrganizationId: str,
    EnabledFeatures: List[FeatureTypeType],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisableOrganizationsRootSessionsResponseTypeDef

```python
# DisableOrganizationsRootSessionsResponseTypeDef definition

class DisableOrganizationsRootSessionsResponseTypeDef(TypedDict):
    OrganizationId: str,
    EnabledFeatures: List[FeatureTypeType],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableOrganizationsRootCredentialsManagementResponseTypeDef

```python
# EnableOrganizationsRootCredentialsManagementResponseTypeDef definition

class EnableOrganizationsRootCredentialsManagementResponseTypeDef(TypedDict):
    OrganizationId: str,
    EnabledFeatures: List[FeatureTypeType],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableOrganizationsRootSessionsResponseTypeDef

```python
# EnableOrganizationsRootSessionsResponseTypeDef definition

class EnableOrganizationsRootSessionsResponseTypeDef(TypedDict):
    OrganizationId: str,
    EnabledFeatures: List[FeatureTypeType],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GenerateCredentialReportResponseTypeDef

```python
# GenerateCredentialReportResponseTypeDef definition

class GenerateCredentialReportResponseTypeDef(TypedDict):
    State: ReportStateTypeType,  # (1)
    Description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ReportStateTypeType](./literals.md#reportstatetypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GenerateOrganizationsAccessReportResponseTypeDef

```python
# GenerateOrganizationsAccessReportResponseTypeDef definition

class GenerateOrganizationsAccessReportResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GenerateServiceLastAccessedDetailsResponseTypeDef

```python
# GenerateServiceLastAccessedDetailsResponseTypeDef definition

class GenerateServiceLastAccessedDetailsResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccessKeyLastUsedResponseTypeDef

```python
# GetAccessKeyLastUsedResponseTypeDef definition

class GetAccessKeyLastUsedResponseTypeDef(TypedDict):
    UserName: str,
    AccessKeyLastUsed: AccessKeyLastUsedTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccessKeyLastUsedTypeDef](./type_defs.md#accesskeylastusedtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccountSummaryResponseTypeDef

```python
# GetAccountSummaryResponseTypeDef definition

class GetAccountSummaryResponseTypeDef(TypedDict):
    SummaryMap: Dict[SummaryKeyTypeType, int],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: SummaryKeyTypeType](./literals.md#summarykeytypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetContextKeysForPolicyResponseTypeDef

```python
# GetContextKeysForPolicyResponseTypeDef definition

class GetContextKeysForPolicyResponseTypeDef(TypedDict):
    ContextKeyNames: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCredentialReportResponseTypeDef

```python
# GetCredentialReportResponseTypeDef definition

class GetCredentialReportResponseTypeDef(TypedDict):
    Content: bytes,
    ReportFormat: ReportFormatTypeType,  # (1)
    GeneratedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ReportFormatTypeType](./literals.md#reportformattypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMFADeviceResponseTypeDef

```python
# GetMFADeviceResponseTypeDef definition

class GetMFADeviceResponseTypeDef(TypedDict):
    UserName: str,
    SerialNumber: str,
    EnableDate: datetime,
    Certifications: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccessKeysResponseTypeDef

```python
# ListAccessKeysResponseTypeDef definition

class ListAccessKeysResponseTypeDef(TypedDict):
    AccessKeyMetadata: List[AccessKeyMetadataTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccessKeyMetadataTypeDef](./type_defs.md#accesskeymetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountAliasesResponseTypeDef

```python
# ListAccountAliasesResponseTypeDef definition

class ListAccountAliasesResponseTypeDef(TypedDict):
    AccountAliases: List[str],
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAttachedGroupPoliciesResponseTypeDef

```python
# ListAttachedGroupPoliciesResponseTypeDef definition

class ListAttachedGroupPoliciesResponseTypeDef(TypedDict):
    AttachedPolicies: List[AttachedPolicyTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttachedPolicyTypeDef](./type_defs.md#attachedpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAttachedRolePoliciesResponseTypeDef

```python
# ListAttachedRolePoliciesResponseTypeDef definition

class ListAttachedRolePoliciesResponseTypeDef(TypedDict):
    AttachedPolicies: List[AttachedPolicyTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttachedPolicyTypeDef](./type_defs.md#attachedpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAttachedUserPoliciesResponseTypeDef

```python
# ListAttachedUserPoliciesResponseTypeDef definition

class ListAttachedUserPoliciesResponseTypeDef(TypedDict):
    AttachedPolicies: List[AttachedPolicyTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttachedPolicyTypeDef](./type_defs.md#attachedpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGroupPoliciesResponseTypeDef

```python
# ListGroupPoliciesResponseTypeDef definition

class ListGroupPoliciesResponseTypeDef(TypedDict):
    PolicyNames: List[str],
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOrganizationsFeaturesResponseTypeDef

```python
# ListOrganizationsFeaturesResponseTypeDef definition

class ListOrganizationsFeaturesResponseTypeDef(TypedDict):
    OrganizationId: str,
    EnabledFeatures: List[FeatureTypeType],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRolePoliciesResponseTypeDef

```python
# ListRolePoliciesResponseTypeDef definition

class ListRolePoliciesResponseTypeDef(TypedDict):
    PolicyNames: List[str],
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUserPoliciesResponseTypeDef

```python
# ListUserPoliciesResponseTypeDef definition

class ListUserPoliciesResponseTypeDef(TypedDict):
    PolicyNames: List[str],
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSAMLProviderResponseTypeDef

```python
# UpdateSAMLProviderResponseTypeDef definition

class UpdateSAMLProviderResponseTypeDef(TypedDict):
    SAMLProviderArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGroupResponseTypeDef

```python
# CreateGroupResponseTypeDef definition

class CreateGroupResponseTypeDef(TypedDict):
    Group: GroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGroupsForUserResponseTypeDef

```python
# ListGroupsForUserResponseTypeDef definition

class ListGroupsForUserResponseTypeDef(TypedDict):
    Groups: List[GroupTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGroupsResponseTypeDef

```python
# ListGroupsResponseTypeDef definition

class ListGroupsResponseTypeDef(TypedDict):
    Groups: List[GroupTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInstanceProfileRequestRequestTypeDef

```python
# CreateInstanceProfileRequestRequestTypeDef definition

class CreateInstanceProfileRequestRequestTypeDef(TypedDict):
    InstanceProfileName: str,
    Path: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef

```python
# CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef definition

class CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef(TypedDict):
    InstanceProfileName: str,
    Path: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateOpenIDConnectProviderRequestRequestTypeDef

```python
# CreateOpenIDConnectProviderRequestRequestTypeDef definition

class CreateOpenIDConnectProviderRequestRequestTypeDef(TypedDict):
    Url: str,
    ClientIDList: NotRequired[Sequence[str]],
    ThumbprintList: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateOpenIDConnectProviderResponseTypeDef

```python
# CreateOpenIDConnectProviderResponseTypeDef definition

class CreateOpenIDConnectProviderResponseTypeDef(TypedDict):
    OpenIDConnectProviderArn: str,
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePolicyRequestRequestTypeDef

```python
# CreatePolicyRequestRequestTypeDef definition

class CreatePolicyRequestRequestTypeDef(TypedDict):
    PolicyName: str,
    PolicyDocument: str,
    Path: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePolicyRequestServiceResourceCreatePolicyTypeDef

```python
# CreatePolicyRequestServiceResourceCreatePolicyTypeDef definition

class CreatePolicyRequestServiceResourceCreatePolicyTypeDef(TypedDict):
    PolicyName: str,
    PolicyDocument: str,
    Path: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateRoleRequestRequestTypeDef

```python
# CreateRoleRequestRequestTypeDef definition

class CreateRoleRequestRequestTypeDef(TypedDict):
    RoleName: str,
    AssumeRolePolicyDocument: str,
    Path: NotRequired[str],
    Description: NotRequired[str],
    MaxSessionDuration: NotRequired[int],
    PermissionsBoundary: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateRoleRequestServiceResourceCreateRoleTypeDef

```python
# CreateRoleRequestServiceResourceCreateRoleTypeDef definition

class CreateRoleRequestServiceResourceCreateRoleTypeDef(TypedDict):
    RoleName: str,
    AssumeRolePolicyDocument: str,
    Path: NotRequired[str],
    Description: NotRequired[str],
    MaxSessionDuration: NotRequired[int],
    PermissionsBoundary: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateSAMLProviderRequestRequestTypeDef

```python
# CreateSAMLProviderRequestRequestTypeDef definition

class CreateSAMLProviderRequestRequestTypeDef(TypedDict):
    SAMLMetadataDocument: str,
    Name: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef

```python
# CreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef definition

class CreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef(TypedDict):
    SAMLMetadataDocument: str,
    Name: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateSAMLProviderResponseTypeDef

```python
# CreateSAMLProviderResponseTypeDef definition

class CreateSAMLProviderResponseTypeDef(TypedDict):
    SAMLProviderArn: str,
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserRequestRequestTypeDef

```python
# CreateUserRequestRequestTypeDef definition

class CreateUserRequestRequestTypeDef(TypedDict):
    UserName: str,
    Path: NotRequired[str],
    PermissionsBoundary: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateUserRequestServiceResourceCreateUserTypeDef

```python
# CreateUserRequestServiceResourceCreateUserTypeDef definition

class CreateUserRequestServiceResourceCreateUserTypeDef(TypedDict):
    UserName: str,
    Path: NotRequired[str],
    PermissionsBoundary: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateUserRequestUserCreateTypeDef

```python
# CreateUserRequestUserCreateTypeDef definition

class CreateUserRequestUserCreateTypeDef(TypedDict):
    Path: NotRequired[str],
    PermissionsBoundary: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateVirtualMFADeviceRequestRequestTypeDef

```python
# CreateVirtualMFADeviceRequestRequestTypeDef definition

class CreateVirtualMFADeviceRequestRequestTypeDef(TypedDict):
    VirtualMFADeviceName: str,
    Path: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef

```python
# CreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef definition

class CreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef(TypedDict):
    VirtualMFADeviceName: str,
    Path: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetOpenIDConnectProviderResponseTypeDef

```python
# GetOpenIDConnectProviderResponseTypeDef definition

class GetOpenIDConnectProviderResponseTypeDef(TypedDict):
    Url: str,
    ClientIDList: List[str],
    ThumbprintList: List[str],
    CreateDate: datetime,
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSAMLProviderResponseTypeDef

```python
# GetSAMLProviderResponseTypeDef definition

class GetSAMLProviderResponseTypeDef(TypedDict):
    SAMLMetadataDocument: str,
    CreateDate: datetime,
    ValidUntil: datetime,
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInstanceProfileTagsResponseTypeDef

```python
# ListInstanceProfileTagsResponseTypeDef definition

class ListInstanceProfileTagsResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMFADeviceTagsResponseTypeDef

```python
# ListMFADeviceTagsResponseTypeDef definition

class ListMFADeviceTagsResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOpenIDConnectProviderTagsResponseTypeDef

```python
# ListOpenIDConnectProviderTagsResponseTypeDef definition

class ListOpenIDConnectProviderTagsResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPolicyTagsResponseTypeDef

```python
# ListPolicyTagsResponseTypeDef definition

class ListPolicyTagsResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRoleTagsResponseTypeDef

```python
# ListRoleTagsResponseTypeDef definition

class ListRoleTagsResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSAMLProviderTagsResponseTypeDef

```python
# ListSAMLProviderTagsResponseTypeDef definition

class ListSAMLProviderTagsResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServerCertificateTagsResponseTypeDef

```python
# ListServerCertificateTagsResponseTypeDef definition

class ListServerCertificateTagsResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUserTagsResponseTypeDef

```python
# ListUserTagsResponseTypeDef definition

class ListUserTagsResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PolicyTypeDef

```python
# PolicyTypeDef definition

class PolicyTypeDef(TypedDict):
    PolicyName: NotRequired[str],
    PolicyId: NotRequired[str],
    Arn: NotRequired[str],
    Path: NotRequired[str],
    DefaultVersionId: NotRequired[str],
    AttachmentCount: NotRequired[int],
    PermissionsBoundaryUsageCount: NotRequired[int],
    IsAttachable: NotRequired[bool],
    Description: NotRequired[str],
    CreateDate: NotRequired[datetime],
    UpdateDate: NotRequired[datetime],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagInstanceProfileRequestRequestTypeDef

```python
# TagInstanceProfileRequestRequestTypeDef definition

class TagInstanceProfileRequestRequestTypeDef(TypedDict):
    InstanceProfileName: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagMFADeviceRequestRequestTypeDef

```python
# TagMFADeviceRequestRequestTypeDef definition

class TagMFADeviceRequestRequestTypeDef(TypedDict):
    SerialNumber: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagOpenIDConnectProviderRequestRequestTypeDef

```python
# TagOpenIDConnectProviderRequestRequestTypeDef definition

class TagOpenIDConnectProviderRequestRequestTypeDef(TypedDict):
    OpenIDConnectProviderArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagPolicyRequestRequestTypeDef

```python
# TagPolicyRequestRequestTypeDef definition

class TagPolicyRequestRequestTypeDef(TypedDict):
    PolicyArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagRoleRequestRequestTypeDef

```python
# TagRoleRequestRequestTypeDef definition

class TagRoleRequestRequestTypeDef(TypedDict):
    RoleName: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagSAMLProviderRequestRequestTypeDef

```python
# TagSAMLProviderRequestRequestTypeDef definition

class TagSAMLProviderRequestRequestTypeDef(TypedDict):
    SAMLProviderArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagServerCertificateRequestRequestTypeDef

```python
# TagServerCertificateRequestRequestTypeDef definition

class TagServerCertificateRequestRequestTypeDef(TypedDict):
    ServerCertificateName: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagUserRequestRequestTypeDef

```python
# TagUserRequestRequestTypeDef definition

class TagUserRequestRequestTypeDef(TypedDict):
    UserName: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UploadServerCertificateRequestRequestTypeDef

```python
# UploadServerCertificateRequestRequestTypeDef definition

class UploadServerCertificateRequestRequestTypeDef(TypedDict):
    ServerCertificateName: str,
    CertificateBody: str,
    PrivateKey: str,
    Path: NotRequired[str],
    CertificateChain: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef

```python
# UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef definition

class UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef(TypedDict):
    ServerCertificateName: str,
    CertificateBody: str,
    PrivateKey: str,
    Path: NotRequired[str],
    CertificateChain: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UserTypeDef

```python
# UserTypeDef definition

class UserTypeDef(TypedDict):
    Path: str,
    UserName: str,
    UserId: str,
    Arn: str,
    CreateDate: datetime,
    PasswordLastUsed: NotRequired[datetime],
    PermissionsBoundary: NotRequired[AttachedPermissionsBoundaryTypeDef],  # (1)
    Tags: NotRequired[List[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: AttachedPermissionsBoundaryTypeDef](./type_defs.md#attachedpermissionsboundarytypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateLoginProfileResponseTypeDef

```python
# CreateLoginProfileResponseTypeDef definition

class CreateLoginProfileResponseTypeDef(TypedDict):
    LoginProfile: LoginProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoginProfileTypeDef](./type_defs.md#loginprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLoginProfileResponseTypeDef

```python
# GetLoginProfileResponseTypeDef definition

class GetLoginProfileResponseTypeDef(TypedDict):
    LoginProfile: LoginProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoginProfileTypeDef](./type_defs.md#loginprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateServiceSpecificCredentialResponseTypeDef

```python
# CreateServiceSpecificCredentialResponseTypeDef definition

class CreateServiceSpecificCredentialResponseTypeDef(TypedDict):
    ServiceSpecificCredential: ServiceSpecificCredentialTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceSpecificCredentialTypeDef](./type_defs.md#servicespecificcredentialtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResetServiceSpecificCredentialResponseTypeDef

```python
# ResetServiceSpecificCredentialResponseTypeDef definition

class ResetServiceSpecificCredentialResponseTypeDef(TypedDict):
    ServiceSpecificCredential: ServiceSpecificCredentialTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceSpecificCredentialTypeDef](./type_defs.md#servicespecificcredentialtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletionTaskFailureReasonTypeTypeDef

```python
# DeletionTaskFailureReasonTypeTypeDef definition

class DeletionTaskFailureReasonTypeTypeDef(TypedDict):
    Reason: NotRequired[str],
    RoleUsageList: NotRequired[List[RoleUsageTypeTypeDef]],  # (1)
```

1. See [:material-code-braces: RoleUsageTypeTypeDef](./type_defs.md#roleusagetypetypedef) 
## EntityDetailsTypeDef

```python
# EntityDetailsTypeDef definition

class EntityDetailsTypeDef(TypedDict):
    EntityInfo: EntityInfoTypeDef,  # (1)
    LastAuthenticated: NotRequired[datetime],
```

1. See [:material-code-braces: EntityInfoTypeDef](./type_defs.md#entityinfotypedef) 
## GetOrganizationsAccessReportResponseTypeDef

```python
# GetOrganizationsAccessReportResponseTypeDef definition

class GetOrganizationsAccessReportResponseTypeDef(TypedDict):
    JobStatus: JobStatusTypeType,  # (1)
    JobCreationDate: datetime,
    JobCompletionDate: datetime,
    NumberOfServicesAccessible: int,
    NumberOfServicesNotAccessed: int,
    AccessDetails: List[AccessDetailTypeDef],  # (2)
    IsTruncated: bool,
    Marker: str,
    ErrorDetails: ErrorDetailsTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: JobStatusTypeType](./literals.md#jobstatustypetype) 
2. See [:material-code-braces: AccessDetailTypeDef](./type_defs.md#accessdetailtypedef) 
3. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccountAuthorizationDetailsRequestPaginateTypeDef

```python
# GetAccountAuthorizationDetailsRequestPaginateTypeDef definition

class GetAccountAuthorizationDetailsRequestPaginateTypeDef(TypedDict):
    Filter: NotRequired[Sequence[EntityTypeType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetGroupRequestPaginateTypeDef

```python
# GetGroupRequestPaginateTypeDef definition

class GetGroupRequestPaginateTypeDef(TypedDict):
    GroupName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAccessKeysRequestPaginateTypeDef

```python
# ListAccessKeysRequestPaginateTypeDef definition

class ListAccessKeysRequestPaginateTypeDef(TypedDict):
    UserName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAccountAliasesRequestPaginateTypeDef

```python
# ListAccountAliasesRequestPaginateTypeDef definition

class ListAccountAliasesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAttachedGroupPoliciesRequestPaginateTypeDef

```python
# ListAttachedGroupPoliciesRequestPaginateTypeDef definition

class ListAttachedGroupPoliciesRequestPaginateTypeDef(TypedDict):
    GroupName: str,
    PathPrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAttachedRolePoliciesRequestPaginateTypeDef

```python
# ListAttachedRolePoliciesRequestPaginateTypeDef definition

class ListAttachedRolePoliciesRequestPaginateTypeDef(TypedDict):
    RoleName: str,
    PathPrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAttachedUserPoliciesRequestPaginateTypeDef

```python
# ListAttachedUserPoliciesRequestPaginateTypeDef definition

class ListAttachedUserPoliciesRequestPaginateTypeDef(TypedDict):
    UserName: str,
    PathPrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEntitiesForPolicyRequestPaginateTypeDef

```python
# ListEntitiesForPolicyRequestPaginateTypeDef definition

class ListEntitiesForPolicyRequestPaginateTypeDef(TypedDict):
    PolicyArn: str,
    EntityFilter: NotRequired[EntityTypeType],  # (1)
    PathPrefix: NotRequired[str],
    PolicyUsageFilter: NotRequired[PolicyUsageTypeType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
2. See [:material-code-brackets: PolicyUsageTypeType](./literals.md#policyusagetypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupPoliciesRequestPaginateTypeDef

```python
# ListGroupPoliciesRequestPaginateTypeDef definition

class ListGroupPoliciesRequestPaginateTypeDef(TypedDict):
    GroupName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupsForUserRequestPaginateTypeDef

```python
# ListGroupsForUserRequestPaginateTypeDef definition

class ListGroupsForUserRequestPaginateTypeDef(TypedDict):
    UserName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupsRequestPaginateTypeDef

```python
# ListGroupsRequestPaginateTypeDef definition

class ListGroupsRequestPaginateTypeDef(TypedDict):
    PathPrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstanceProfileTagsRequestPaginateTypeDef

```python
# ListInstanceProfileTagsRequestPaginateTypeDef definition

class ListInstanceProfileTagsRequestPaginateTypeDef(TypedDict):
    InstanceProfileName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstanceProfilesForRoleRequestPaginateTypeDef

```python
# ListInstanceProfilesForRoleRequestPaginateTypeDef definition

class ListInstanceProfilesForRoleRequestPaginateTypeDef(TypedDict):
    RoleName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstanceProfilesRequestPaginateTypeDef

```python
# ListInstanceProfilesRequestPaginateTypeDef definition

class ListInstanceProfilesRequestPaginateTypeDef(TypedDict):
    PathPrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMFADeviceTagsRequestPaginateTypeDef

```python
# ListMFADeviceTagsRequestPaginateTypeDef definition

class ListMFADeviceTagsRequestPaginateTypeDef(TypedDict):
    SerialNumber: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMFADevicesRequestPaginateTypeDef

```python
# ListMFADevicesRequestPaginateTypeDef definition

class ListMFADevicesRequestPaginateTypeDef(TypedDict):
    UserName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOpenIDConnectProviderTagsRequestPaginateTypeDef

```python
# ListOpenIDConnectProviderTagsRequestPaginateTypeDef definition

class ListOpenIDConnectProviderTagsRequestPaginateTypeDef(TypedDict):
    OpenIDConnectProviderArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPoliciesRequestPaginateTypeDef

```python
# ListPoliciesRequestPaginateTypeDef definition

class ListPoliciesRequestPaginateTypeDef(TypedDict):
    Scope: NotRequired[PolicyScopeTypeType],  # (1)
    OnlyAttached: NotRequired[bool],
    PathPrefix: NotRequired[str],
    PolicyUsageFilter: NotRequired[PolicyUsageTypeType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: PolicyScopeTypeType](./literals.md#policyscopetypetype) 
2. See [:material-code-brackets: PolicyUsageTypeType](./literals.md#policyusagetypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPolicyTagsRequestPaginateTypeDef

```python
# ListPolicyTagsRequestPaginateTypeDef definition

class ListPolicyTagsRequestPaginateTypeDef(TypedDict):
    PolicyArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPolicyVersionsRequestPaginateTypeDef

```python
# ListPolicyVersionsRequestPaginateTypeDef definition

class ListPolicyVersionsRequestPaginateTypeDef(TypedDict):
    PolicyArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRolePoliciesRequestPaginateTypeDef

```python
# ListRolePoliciesRequestPaginateTypeDef definition

class ListRolePoliciesRequestPaginateTypeDef(TypedDict):
    RoleName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRoleTagsRequestPaginateTypeDef

```python
# ListRoleTagsRequestPaginateTypeDef definition

class ListRoleTagsRequestPaginateTypeDef(TypedDict):
    RoleName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRolesRequestPaginateTypeDef

```python
# ListRolesRequestPaginateTypeDef definition

class ListRolesRequestPaginateTypeDef(TypedDict):
    PathPrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSAMLProviderTagsRequestPaginateTypeDef

```python
# ListSAMLProviderTagsRequestPaginateTypeDef definition

class ListSAMLProviderTagsRequestPaginateTypeDef(TypedDict):
    SAMLProviderArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSSHPublicKeysRequestPaginateTypeDef

```python
# ListSSHPublicKeysRequestPaginateTypeDef definition

class ListSSHPublicKeysRequestPaginateTypeDef(TypedDict):
    UserName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServerCertificateTagsRequestPaginateTypeDef

```python
# ListServerCertificateTagsRequestPaginateTypeDef definition

class ListServerCertificateTagsRequestPaginateTypeDef(TypedDict):
    ServerCertificateName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServerCertificatesRequestPaginateTypeDef

```python
# ListServerCertificatesRequestPaginateTypeDef definition

class ListServerCertificatesRequestPaginateTypeDef(TypedDict):
    PathPrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSigningCertificatesRequestPaginateTypeDef

```python
# ListSigningCertificatesRequestPaginateTypeDef definition

class ListSigningCertificatesRequestPaginateTypeDef(TypedDict):
    UserName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUserPoliciesRequestPaginateTypeDef

```python
# ListUserPoliciesRequestPaginateTypeDef definition

class ListUserPoliciesRequestPaginateTypeDef(TypedDict):
    UserName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUserTagsRequestPaginateTypeDef

```python
# ListUserTagsRequestPaginateTypeDef definition

class ListUserTagsRequestPaginateTypeDef(TypedDict):
    UserName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUsersRequestPaginateTypeDef

```python
# ListUsersRequestPaginateTypeDef definition

class ListUsersRequestPaginateTypeDef(TypedDict):
    PathPrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVirtualMFADevicesRequestPaginateTypeDef

```python
# ListVirtualMFADevicesRequestPaginateTypeDef definition

class ListVirtualMFADevicesRequestPaginateTypeDef(TypedDict):
    AssignmentStatus: NotRequired[AssignmentStatusTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AssignmentStatusTypeType](./literals.md#assignmentstatustypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SimulateCustomPolicyRequestPaginateTypeDef

```python
# SimulateCustomPolicyRequestPaginateTypeDef definition

class SimulateCustomPolicyRequestPaginateTypeDef(TypedDict):
    PolicyInputList: Sequence[str],
    ActionNames: Sequence[str],
    PermissionsBoundaryPolicyInputList: NotRequired[Sequence[str]],
    ResourceArns: NotRequired[Sequence[str]],
    ResourcePolicy: NotRequired[str],
    ResourceOwner: NotRequired[str],
    CallerArn: NotRequired[str],
    ContextEntries: NotRequired[Sequence[ContextEntryTypeDef]],  # (1)
    ResourceHandlingOption: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ContextEntryTypeDef](./type_defs.md#contextentrytypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SimulatePrincipalPolicyRequestPaginateTypeDef

```python
# SimulatePrincipalPolicyRequestPaginateTypeDef definition

class SimulatePrincipalPolicyRequestPaginateTypeDef(TypedDict):
    PolicySourceArn: str,
    ActionNames: Sequence[str],
    PolicyInputList: NotRequired[Sequence[str]],
    PermissionsBoundaryPolicyInputList: NotRequired[Sequence[str]],
    ResourceArns: NotRequired[Sequence[str]],
    ResourcePolicy: NotRequired[str],
    ResourceOwner: NotRequired[str],
    CallerArn: NotRequired[str],
    ContextEntries: NotRequired[Sequence[ContextEntryTypeDef]],  # (1)
    ResourceHandlingOption: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ContextEntryTypeDef](./type_defs.md#contextentrytypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetAccountPasswordPolicyResponseTypeDef

```python
# GetAccountPasswordPolicyResponseTypeDef definition

class GetAccountPasswordPolicyResponseTypeDef(TypedDict):
    PasswordPolicy: PasswordPolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PasswordPolicyTypeDef](./type_defs.md#passwordpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInstanceProfileRequestWaitTypeDef

```python
# GetInstanceProfileRequestWaitTypeDef definition

class GetInstanceProfileRequestWaitTypeDef(TypedDict):
    InstanceProfileName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetPolicyRequestWaitTypeDef

```python
# GetPolicyRequestWaitTypeDef definition

class GetPolicyRequestWaitTypeDef(TypedDict):
    PolicyArn: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetRoleRequestWaitTypeDef

```python
# GetRoleRequestWaitTypeDef definition

class GetRoleRequestWaitTypeDef(TypedDict):
    RoleName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetUserRequestWaitTypeDef

```python
# GetUserRequestWaitTypeDef definition

class GetUserRequestWaitTypeDef(TypedDict):
    UserName: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetSSHPublicKeyResponseTypeDef

```python
# GetSSHPublicKeyResponseTypeDef definition

class GetSSHPublicKeyResponseTypeDef(TypedDict):
    SSHPublicKey: SSHPublicKeyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SSHPublicKeyTypeDef](./type_defs.md#sshpublickeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UploadSSHPublicKeyResponseTypeDef

```python
# UploadSSHPublicKeyResponseTypeDef definition

class UploadSSHPublicKeyResponseTypeDef(TypedDict):
    SSHPublicKey: SSHPublicKeyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SSHPublicKeyTypeDef](./type_defs.md#sshpublickeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEntitiesForPolicyResponseTypeDef

```python
# ListEntitiesForPolicyResponseTypeDef definition

class ListEntitiesForPolicyResponseTypeDef(TypedDict):
    PolicyGroups: List[PolicyGroupTypeDef],  # (1)
    PolicyUsers: List[PolicyUserTypeDef],  # (2)
    PolicyRoles: List[PolicyRoleTypeDef],  # (3)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: PolicyGroupTypeDef](./type_defs.md#policygrouptypedef) 
2. See [:material-code-braces: PolicyUserTypeDef](./type_defs.md#policyusertypedef) 
3. See [:material-code-braces: PolicyRoleTypeDef](./type_defs.md#policyroletypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMFADevicesResponseTypeDef

```python
# ListMFADevicesResponseTypeDef definition

class ListMFADevicesResponseTypeDef(TypedDict):
    MFADevices: List[MFADeviceTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MFADeviceTypeDef](./type_defs.md#mfadevicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOpenIDConnectProvidersResponseTypeDef

```python
# ListOpenIDConnectProvidersResponseTypeDef definition

class ListOpenIDConnectProvidersResponseTypeDef(TypedDict):
    OpenIDConnectProviderList: List[OpenIDConnectProviderListEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OpenIDConnectProviderListEntryTypeDef](./type_defs.md#openidconnectproviderlistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPoliciesGrantingServiceAccessEntryTypeDef

```python
# ListPoliciesGrantingServiceAccessEntryTypeDef definition

class ListPoliciesGrantingServiceAccessEntryTypeDef(TypedDict):
    ServiceNamespace: NotRequired[str],
    Policies: NotRequired[List[PolicyGrantingServiceAccessTypeDef]],  # (1)
```

1. See [:material-code-braces: PolicyGrantingServiceAccessTypeDef](./type_defs.md#policygrantingserviceaccesstypedef) 
## ListSAMLProvidersResponseTypeDef

```python
# ListSAMLProvidersResponseTypeDef definition

class ListSAMLProvidersResponseTypeDef(TypedDict):
    SAMLProviderList: List[SAMLProviderListEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SAMLProviderListEntryTypeDef](./type_defs.md#samlproviderlistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSSHPublicKeysResponseTypeDef

```python
# ListSSHPublicKeysResponseTypeDef definition

class ListSSHPublicKeysResponseTypeDef(TypedDict):
    SSHPublicKeys: List[SSHPublicKeyMetadataTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SSHPublicKeyMetadataTypeDef](./type_defs.md#sshpublickeymetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServerCertificatesResponseTypeDef

```python
# ListServerCertificatesResponseTypeDef definition

class ListServerCertificatesResponseTypeDef(TypedDict):
    ServerCertificateMetadataList: List[ServerCertificateMetadataTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerCertificateMetadataTypeDef](./type_defs.md#servercertificatemetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ServerCertificateTypeDef

```python
# ServerCertificateTypeDef definition

class ServerCertificateTypeDef(TypedDict):
    ServerCertificateMetadata: ServerCertificateMetadataTypeDef,  # (1)
    CertificateBody: str,
    CertificateChain: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ServerCertificateMetadataTypeDef](./type_defs.md#servercertificatemetadatatypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UploadServerCertificateResponseTypeDef

```python
# UploadServerCertificateResponseTypeDef definition

class UploadServerCertificateResponseTypeDef(TypedDict):
    ServerCertificateMetadata: ServerCertificateMetadataTypeDef,  # (1)
    Tags: List[TagTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ServerCertificateMetadataTypeDef](./type_defs.md#servercertificatemetadatatypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServiceSpecificCredentialsResponseTypeDef

```python
# ListServiceSpecificCredentialsResponseTypeDef definition

class ListServiceSpecificCredentialsResponseTypeDef(TypedDict):
    ServiceSpecificCredentials: List[ServiceSpecificCredentialMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceSpecificCredentialMetadataTypeDef](./type_defs.md#servicespecificcredentialmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSigningCertificatesResponseTypeDef

```python
# ListSigningCertificatesResponseTypeDef definition

class ListSigningCertificatesResponseTypeDef(TypedDict):
    Certificates: List[SigningCertificateTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SigningCertificateTypeDef](./type_defs.md#signingcertificatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UploadSigningCertificateResponseTypeDef

```python
# UploadSigningCertificateResponseTypeDef definition

class UploadSigningCertificateResponseTypeDef(TypedDict):
    Certificate: SigningCertificateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SigningCertificateTypeDef](./type_defs.md#signingcertificatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PolicyDocumentDictTypeDef

```python
# PolicyDocumentDictTypeDef definition

class PolicyDocumentDictTypeDef(TypedDict):
    Version: str,
    Statement: List[PolicyDocumentStatementTypeDef],  # (1)
```

1. See [:material-code-braces: PolicyDocumentStatementTypeDef](./type_defs.md#policydocumentstatementtypedef) 
## StatementTypeDef

```python
# StatementTypeDef definition

class StatementTypeDef(TypedDict):
    SourcePolicyId: NotRequired[str],
    SourcePolicyType: NotRequired[PolicySourceTypeType],  # (1)
    StartPosition: NotRequired[PositionTypeDef],  # (2)
    EndPosition: NotRequired[PositionTypeDef],  # (2)
```

1. See [:material-code-brackets: PolicySourceTypeType](./literals.md#policysourcetypetype) 
2. See [:material-code-braces: PositionTypeDef](./type_defs.md#positiontypedef) 
3. See [:material-code-braces: PositionTypeDef](./type_defs.md#positiontypedef) 
## ServiceLastAccessedTypeDef

```python
# ServiceLastAccessedTypeDef definition

class ServiceLastAccessedTypeDef(TypedDict):
    ServiceName: str,
    ServiceNamespace: str,
    LastAuthenticated: NotRequired[datetime],
    LastAuthenticatedEntity: NotRequired[str],
    LastAuthenticatedRegion: NotRequired[str],
    TotalAuthenticatedEntities: NotRequired[int],
    TrackedActionsLastAccessed: NotRequired[List[TrackedActionLastAccessedTypeDef]],  # (1)
```

1. See [:material-code-braces: TrackedActionLastAccessedTypeDef](./type_defs.md#trackedactionlastaccessedtypedef) 
## CreatePolicyResponseTypeDef

```python
# CreatePolicyResponseTypeDef definition

class CreatePolicyResponseTypeDef(TypedDict):
    Policy: PolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPolicyResponseTypeDef

```python
# GetPolicyResponseTypeDef definition

class GetPolicyResponseTypeDef(TypedDict):
    Policy: PolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPoliciesResponseTypeDef

```python
# ListPoliciesResponseTypeDef definition

class ListPoliciesResponseTypeDef(TypedDict):
    Policies: List[PolicyTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserResponseTypeDef

```python
# CreateUserResponseTypeDef definition

class CreateUserResponseTypeDef(TypedDict):
    User: UserTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGroupResponseTypeDef

```python
# GetGroupResponseTypeDef definition

class GetGroupResponseTypeDef(TypedDict):
    Group: GroupTypeDef,  # (1)
    Users: List[UserTypeDef],  # (2)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUserResponseTypeDef

```python
# GetUserResponseTypeDef definition

class GetUserResponseTypeDef(TypedDict):
    User: UserTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUsersResponseTypeDef

```python
# ListUsersResponseTypeDef definition

class ListUsersResponseTypeDef(TypedDict):
    Users: List[UserTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VirtualMFADeviceTypeDef

```python
# VirtualMFADeviceTypeDef definition

class VirtualMFADeviceTypeDef(TypedDict):
    SerialNumber: str,
    Base32StringSeed: NotRequired[bytes],
    QRCodePNG: NotRequired[bytes],
    User: NotRequired[UserTypeDef],  # (1)
    EnableDate: NotRequired[datetime],
    Tags: NotRequired[List[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetServiceLinkedRoleDeletionStatusResponseTypeDef

```python
# GetServiceLinkedRoleDeletionStatusResponseTypeDef definition

class GetServiceLinkedRoleDeletionStatusResponseTypeDef(TypedDict):
    Status: DeletionTaskStatusTypeType,  # (1)
    Reason: DeletionTaskFailureReasonTypeTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: DeletionTaskStatusTypeType](./literals.md#deletiontaskstatustypetype) 
2. See [:material-code-braces: DeletionTaskFailureReasonTypeTypeDef](./type_defs.md#deletiontaskfailurereasontypetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef

```python
# GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef definition

class GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef(TypedDict):
    JobStatus: JobStatusTypeType,  # (1)
    JobCreationDate: datetime,
    JobCompletionDate: datetime,
    EntityDetailsList: List[EntityDetailsTypeDef],  # (2)
    IsTruncated: bool,
    Marker: str,
    Error: ErrorDetailsTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: JobStatusTypeType](./literals.md#jobstatustypetype) 
2. See [:material-code-braces: EntityDetailsTypeDef](./type_defs.md#entitydetailstypedef) 
3. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPoliciesGrantingServiceAccessResponseTypeDef

```python
# ListPoliciesGrantingServiceAccessResponseTypeDef definition

class ListPoliciesGrantingServiceAccessResponseTypeDef(TypedDict):
    PoliciesGrantingServiceAccess: List[ListPoliciesGrantingServiceAccessEntryTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListPoliciesGrantingServiceAccessEntryTypeDef](./type_defs.md#listpoliciesgrantingserviceaccessentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServerCertificateResponseTypeDef

```python
# GetServerCertificateResponseTypeDef definition

class GetServerCertificateResponseTypeDef(TypedDict):
    ServerCertificate: ServerCertificateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerCertificateTypeDef](./type_defs.md#servercertificatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResourceSpecificResultTypeDef

```python
# ResourceSpecificResultTypeDef definition

class ResourceSpecificResultTypeDef(TypedDict):
    EvalResourceName: str,
    EvalResourceDecision: PolicyEvaluationDecisionTypeType,  # (1)
    MatchedStatements: NotRequired[List[StatementTypeDef]],  # (2)
    MissingContextValues: NotRequired[List[str]],
    EvalDecisionDetails: NotRequired[Dict[str, PolicyEvaluationDecisionTypeType]],  # (3)
    PermissionsBoundaryDecisionDetail: NotRequired[PermissionsBoundaryDecisionDetailTypeDef],  # (4)
```

1. See [:material-code-brackets: PolicyEvaluationDecisionTypeType](./literals.md#policyevaluationdecisiontypetype) 
2. See [:material-code-braces: StatementTypeDef](./type_defs.md#statementtypedef) 
3. See [:material-code-brackets: PolicyEvaluationDecisionTypeType](./literals.md#policyevaluationdecisiontypetype) 
4. See [:material-code-braces: PermissionsBoundaryDecisionDetailTypeDef](./type_defs.md#permissionsboundarydecisiondetailtypedef) 
## GetServiceLastAccessedDetailsResponseTypeDef

```python
# GetServiceLastAccessedDetailsResponseTypeDef definition

class GetServiceLastAccessedDetailsResponseTypeDef(TypedDict):
    JobStatus: JobStatusTypeType,  # (1)
    JobType: AccessAdvisorUsageGranularityTypeType,  # (2)
    JobCreationDate: datetime,
    ServicesLastAccessed: List[ServiceLastAccessedTypeDef],  # (3)
    JobCompletionDate: datetime,
    IsTruncated: bool,
    Marker: str,
    Error: ErrorDetailsTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: JobStatusTypeType](./literals.md#jobstatustypetype) 
2. See [:material-code-brackets: AccessAdvisorUsageGranularityTypeType](./literals.md#accessadvisorusagegranularitytypetype) 
3. See [:material-code-braces: ServiceLastAccessedTypeDef](./type_defs.md#servicelastaccessedtypedef) 
4. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVirtualMFADeviceResponseTypeDef

```python
# CreateVirtualMFADeviceResponseTypeDef definition

class CreateVirtualMFADeviceResponseTypeDef(TypedDict):
    VirtualMFADevice: VirtualMFADeviceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualMFADeviceTypeDef](./type_defs.md#virtualmfadevicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVirtualMFADevicesResponseTypeDef

```python
# ListVirtualMFADevicesResponseTypeDef definition

class ListVirtualMFADevicesResponseTypeDef(TypedDict):
    VirtualMFADevices: List[VirtualMFADeviceTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualMFADeviceTypeDef](./type_defs.md#virtualmfadevicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGroupPolicyResponseTypeDef

```python
# GetGroupPolicyResponseTypeDef definition

class GetGroupPolicyResponseTypeDef(TypedDict):
    GroupName: str,
    PolicyName: str,
    PolicyDocument: PolicyDocumentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyDocumentDictTypeDef](./type_defs.md#policydocumentdicttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRolePolicyResponseTypeDef

```python
# GetRolePolicyResponseTypeDef definition

class GetRolePolicyResponseTypeDef(TypedDict):
    RoleName: str,
    PolicyName: str,
    PolicyDocument: PolicyDocumentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyDocumentDictTypeDef](./type_defs.md#policydocumentdicttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUserPolicyResponseTypeDef

```python
# GetUserPolicyResponseTypeDef definition

class GetUserPolicyResponseTypeDef(TypedDict):
    UserName: str,
    PolicyName: str,
    PolicyDocument: PolicyDocumentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyDocumentDictTypeDef](./type_defs.md#policydocumentdicttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PolicyDetailTypeDef

```python
# PolicyDetailTypeDef definition

class PolicyDetailTypeDef(TypedDict):
    PolicyName: NotRequired[str],
    PolicyDocument: NotRequired[PolicyDocumentTypeDef],  # (1)
```

1. See [:material-code-braces: PolicyDocumentDictTypeDef](./type_defs.md#policydocumentdicttypedef) 
## PolicyVersionTypeDef

```python
# PolicyVersionTypeDef definition

class PolicyVersionTypeDef(TypedDict):
    Document: NotRequired[PolicyDocumentTypeDef],  # (1)
    VersionId: NotRequired[str],
    IsDefaultVersion: NotRequired[bool],
    CreateDate: NotRequired[datetime],
```

1. See [:material-code-braces: PolicyDocumentDictTypeDef](./type_defs.md#policydocumentdicttypedef) 
## RoleTypeDef

```python
# RoleTypeDef definition

class RoleTypeDef(TypedDict):
    Path: str,
    RoleName: str,
    RoleId: str,
    Arn: str,
    CreateDate: datetime,
    AssumeRolePolicyDocument: NotRequired[PolicyDocumentTypeDef],  # (1)
    Description: NotRequired[str],
    MaxSessionDuration: NotRequired[int],
    PermissionsBoundary: NotRequired[AttachedPermissionsBoundaryTypeDef],  # (2)
    Tags: NotRequired[List[TagTypeDef]],  # (3)
    RoleLastUsed: NotRequired[RoleLastUsedTypeDef],  # (4)
```

1. See [:material-code-braces: PolicyDocumentDictTypeDef](./type_defs.md#policydocumentdicttypedef) 
2. See [:material-code-braces: AttachedPermissionsBoundaryTypeDef](./type_defs.md#attachedpermissionsboundarytypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: RoleLastUsedTypeDef](./type_defs.md#rolelastusedtypedef) 
## EvaluationResultTypeDef

```python
# EvaluationResultTypeDef definition

class EvaluationResultTypeDef(TypedDict):
    EvalActionName: str,
    EvalDecision: PolicyEvaluationDecisionTypeType,  # (1)
    EvalResourceName: NotRequired[str],
    MatchedStatements: NotRequired[List[StatementTypeDef]],  # (2)
    MissingContextValues: NotRequired[List[str]],
    OrganizationsDecisionDetail: NotRequired[OrganizationsDecisionDetailTypeDef],  # (3)
    PermissionsBoundaryDecisionDetail: NotRequired[PermissionsBoundaryDecisionDetailTypeDef],  # (4)
    EvalDecisionDetails: NotRequired[Dict[str, PolicyEvaluationDecisionTypeType]],  # (5)
    ResourceSpecificResults: NotRequired[List[ResourceSpecificResultTypeDef]],  # (6)
```

1. See [:material-code-brackets: PolicyEvaluationDecisionTypeType](./literals.md#policyevaluationdecisiontypetype) 
2. See [:material-code-braces: StatementTypeDef](./type_defs.md#statementtypedef) 
3. See [:material-code-braces: OrganizationsDecisionDetailTypeDef](./type_defs.md#organizationsdecisiondetailtypedef) 
4. See [:material-code-braces: PermissionsBoundaryDecisionDetailTypeDef](./type_defs.md#permissionsboundarydecisiondetailtypedef) 
5. See [:material-code-brackets: PolicyEvaluationDecisionTypeType](./literals.md#policyevaluationdecisiontypetype) 
6. See [:material-code-braces: ResourceSpecificResultTypeDef](./type_defs.md#resourcespecificresulttypedef) 
## GroupDetailTypeDef

```python
# GroupDetailTypeDef definition

class GroupDetailTypeDef(TypedDict):
    Path: NotRequired[str],
    GroupName: NotRequired[str],
    GroupId: NotRequired[str],
    Arn: NotRequired[str],
    CreateDate: NotRequired[datetime],
    GroupPolicyList: NotRequired[List[PolicyDetailTypeDef]],  # (1)
    AttachedManagedPolicies: NotRequired[List[AttachedPolicyTypeDef]],  # (2)
```

1. See [:material-code-braces: PolicyDetailTypeDef](./type_defs.md#policydetailtypedef) 
2. See [:material-code-braces: AttachedPolicyTypeDef](./type_defs.md#attachedpolicytypedef) 
## UserDetailTypeDef

```python
# UserDetailTypeDef definition

class UserDetailTypeDef(TypedDict):
    Path: NotRequired[str],
    UserName: NotRequired[str],
    UserId: NotRequired[str],
    Arn: NotRequired[str],
    CreateDate: NotRequired[datetime],
    UserPolicyList: NotRequired[List[PolicyDetailTypeDef]],  # (1)
    GroupList: NotRequired[List[str]],
    AttachedManagedPolicies: NotRequired[List[AttachedPolicyTypeDef]],  # (2)
    PermissionsBoundary: NotRequired[AttachedPermissionsBoundaryTypeDef],  # (3)
    Tags: NotRequired[List[TagTypeDef]],  # (4)
```

1. See [:material-code-braces: PolicyDetailTypeDef](./type_defs.md#policydetailtypedef) 
2. See [:material-code-braces: AttachedPolicyTypeDef](./type_defs.md#attachedpolicytypedef) 
3. See [:material-code-braces: AttachedPermissionsBoundaryTypeDef](./type_defs.md#attachedpermissionsboundarytypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePolicyVersionResponseTypeDef

```python
# CreatePolicyVersionResponseTypeDef definition

class CreatePolicyVersionResponseTypeDef(TypedDict):
    PolicyVersion: PolicyVersionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyVersionTypeDef](./type_defs.md#policyversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPolicyVersionResponseTypeDef

```python
# GetPolicyVersionResponseTypeDef definition

class GetPolicyVersionResponseTypeDef(TypedDict):
    PolicyVersion: PolicyVersionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyVersionTypeDef](./type_defs.md#policyversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPolicyVersionsResponseTypeDef

```python
# ListPolicyVersionsResponseTypeDef definition

class ListPolicyVersionsResponseTypeDef(TypedDict):
    Versions: List[PolicyVersionTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyVersionTypeDef](./type_defs.md#policyversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ManagedPolicyDetailTypeDef

```python
# ManagedPolicyDetailTypeDef definition

class ManagedPolicyDetailTypeDef(TypedDict):
    PolicyName: NotRequired[str],
    PolicyId: NotRequired[str],
    Arn: NotRequired[str],
    Path: NotRequired[str],
    DefaultVersionId: NotRequired[str],
    AttachmentCount: NotRequired[int],
    PermissionsBoundaryUsageCount: NotRequired[int],
    IsAttachable: NotRequired[bool],
    Description: NotRequired[str],
    CreateDate: NotRequired[datetime],
    UpdateDate: NotRequired[datetime],
    PolicyVersionList: NotRequired[List[PolicyVersionTypeDef]],  # (1)
```

1. See [:material-code-braces: PolicyVersionTypeDef](./type_defs.md#policyversiontypedef) 
## CreateRoleResponseTypeDef

```python
# CreateRoleResponseTypeDef definition

class CreateRoleResponseTypeDef(TypedDict):
    Role: RoleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoleTypeDef](./type_defs.md#roletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateServiceLinkedRoleResponseTypeDef

```python
# CreateServiceLinkedRoleResponseTypeDef definition

class CreateServiceLinkedRoleResponseTypeDef(TypedDict):
    Role: RoleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoleTypeDef](./type_defs.md#roletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRoleResponseTypeDef

```python
# GetRoleResponseTypeDef definition

class GetRoleResponseTypeDef(TypedDict):
    Role: RoleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoleTypeDef](./type_defs.md#roletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstanceProfileTypeDef

```python
# InstanceProfileTypeDef definition

class InstanceProfileTypeDef(TypedDict):
    Path: str,
    InstanceProfileName: str,
    InstanceProfileId: str,
    Arn: str,
    CreateDate: datetime,
    Roles: List[RoleTypeDef],  # (1)
    Tags: NotRequired[List[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: RoleTypeDef](./type_defs.md#roletypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListRolesResponseTypeDef

```python
# ListRolesResponseTypeDef definition

class ListRolesResponseTypeDef(TypedDict):
    Roles: List[RoleTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoleTypeDef](./type_defs.md#roletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRoleDescriptionResponseTypeDef

```python
# UpdateRoleDescriptionResponseTypeDef definition

class UpdateRoleDescriptionResponseTypeDef(TypedDict):
    Role: RoleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoleTypeDef](./type_defs.md#roletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SimulatePolicyResponseTypeDef

```python
# SimulatePolicyResponseTypeDef definition

class SimulatePolicyResponseTypeDef(TypedDict):
    EvaluationResults: List[EvaluationResultTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EvaluationResultTypeDef](./type_defs.md#evaluationresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInstanceProfileResponseTypeDef

```python
# CreateInstanceProfileResponseTypeDef definition

class CreateInstanceProfileResponseTypeDef(TypedDict):
    InstanceProfile: InstanceProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceProfileTypeDef](./type_defs.md#instanceprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInstanceProfileResponseTypeDef

```python
# GetInstanceProfileResponseTypeDef definition

class GetInstanceProfileResponseTypeDef(TypedDict):
    InstanceProfile: InstanceProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceProfileTypeDef](./type_defs.md#instanceprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInstanceProfilesForRoleResponseTypeDef

```python
# ListInstanceProfilesForRoleResponseTypeDef definition

class ListInstanceProfilesForRoleResponseTypeDef(TypedDict):
    InstanceProfiles: List[InstanceProfileTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceProfileTypeDef](./type_defs.md#instanceprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInstanceProfilesResponseTypeDef

```python
# ListInstanceProfilesResponseTypeDef definition

class ListInstanceProfilesResponseTypeDef(TypedDict):
    InstanceProfiles: List[InstanceProfileTypeDef],  # (1)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceProfileTypeDef](./type_defs.md#instanceprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RoleDetailTypeDef

```python
# RoleDetailTypeDef definition

class RoleDetailTypeDef(TypedDict):
    Path: NotRequired[str],
    RoleName: NotRequired[str],
    RoleId: NotRequired[str],
    Arn: NotRequired[str],
    CreateDate: NotRequired[datetime],
    AssumeRolePolicyDocument: NotRequired[PolicyDocumentTypeDef],  # (1)
    InstanceProfileList: NotRequired[List[InstanceProfileTypeDef]],  # (2)
    RolePolicyList: NotRequired[List[PolicyDetailTypeDef]],  # (3)
    AttachedManagedPolicies: NotRequired[List[AttachedPolicyTypeDef]],  # (4)
    PermissionsBoundary: NotRequired[AttachedPermissionsBoundaryTypeDef],  # (5)
    Tags: NotRequired[List[TagTypeDef]],  # (6)
    RoleLastUsed: NotRequired[RoleLastUsedTypeDef],  # (7)
```

1. See [:material-code-braces: PolicyDocumentDictTypeDef](./type_defs.md#policydocumentdicttypedef) 
2. See [:material-code-braces: InstanceProfileTypeDef](./type_defs.md#instanceprofiletypedef) 
3. See [:material-code-braces: PolicyDetailTypeDef](./type_defs.md#policydetailtypedef) 
4. See [:material-code-braces: AttachedPolicyTypeDef](./type_defs.md#attachedpolicytypedef) 
5. See [:material-code-braces: AttachedPermissionsBoundaryTypeDef](./type_defs.md#attachedpermissionsboundarytypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-braces: RoleLastUsedTypeDef](./type_defs.md#rolelastusedtypedef) 
## GetAccountAuthorizationDetailsResponseTypeDef

```python
# GetAccountAuthorizationDetailsResponseTypeDef definition

class GetAccountAuthorizationDetailsResponseTypeDef(TypedDict):
    UserDetailList: List[UserDetailTypeDef],  # (1)
    GroupDetailList: List[GroupDetailTypeDef],  # (2)
    RoleDetailList: List[RoleDetailTypeDef],  # (3)
    Policies: List[ManagedPolicyDetailTypeDef],  # (4)
    IsTruncated: bool,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: UserDetailTypeDef](./type_defs.md#userdetailtypedef) 
2. See [:material-code-braces: GroupDetailTypeDef](./type_defs.md#groupdetailtypedef) 
3. See [:material-code-braces: RoleDetailTypeDef](./type_defs.md#roledetailtypedef) 
4. See [:material-code-braces: ManagedPolicyDetailTypeDef](./type_defs.md#managedpolicydetailtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
