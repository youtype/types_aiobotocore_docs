# IAMServiceResource

> [Index](../README.md) > [IAM](./README.md) > IAMServiceResource

!!! note ""

    Auto-generated documentation for [IAM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
    type annotations stubs module [types-aiobotocore-iam](https://pypi.org/project/types-aiobotocore-iam/).

## IAMServiceResource

Type annotations and code completion for `#!python session.resource("iam")`, included resources and collections.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource)

```python
# IAMServiceResource usage example

from types_aiobotocore_iam.service_resource import IAMServiceResource

def get_iam_resource() -> IAMServiceResource:
    return session.resource("iam")
```


## Attributes


- `meta`: [IAMResourceMeta](#iamresourcemeta)

- `groups`: [ServiceResourceGroupsCollection](#serviceresourcegroupscollection)

- `instance_profiles`: [ServiceResourceInstanceProfilesCollection](#serviceresourceinstanceprofilescollection)

- `policies`: [ServiceResourcePoliciesCollection](#serviceresourcepoliciescollection)

- `roles`: [ServiceResourceRolesCollection](#serviceresourcerolescollection)

- `saml_providers`: [ServiceResourceSamlProvidersCollection](#serviceresourcesamlproviderscollection)

- `server_certificates`: [ServiceResourceServerCertificatesCollection](#serviceresourceservercertificatescollection)

- `users`: [ServiceResourceUsersCollection](#serviceresourceuserscollection)

- `virtual_mfa_devices`: [ServiceResourceVirtualMfaDevicesCollection](#serviceresourcevirtualmfadevicescollection)




## Collections

### ServiceResourceGroupsCollection

Provides access to [Group](#group) resource.

Type annotations and code completion for `#!python session.resource("iam").groups` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.groups)

```python
# ServiceResourceGroupsCollection usage example

from types_aiobotocore_iam.service_resource import ServiceResourceGroupsCollection

def get_collection() -> ServiceResourceGroupsCollection:
    return session.resource("iam").groups
```

### ServiceResourceInstanceProfilesCollection

Provides access to [InstanceProfile](#instanceprofile) resource.

Type annotations and code completion for `#!python session.resource("iam").instance_profiles` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.instance_profiles)

```python
# ServiceResourceInstanceProfilesCollection usage example

from types_aiobotocore_iam.service_resource import ServiceResourceInstanceProfilesCollection

def get_collection() -> ServiceResourceInstanceProfilesCollection:
    return session.resource("iam").instance_profiles
```

### ServiceResourcePoliciesCollection

Provides access to [Policy](#policy) resource.

Type annotations and code completion for `#!python session.resource("iam").policies` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.policies)

```python
# ServiceResourcePoliciesCollection usage example

from types_aiobotocore_iam.service_resource import ServiceResourcePoliciesCollection

def get_collection() -> ServiceResourcePoliciesCollection:
    return session.resource("iam").policies
```

### ServiceResourceRolesCollection

Provides access to [Role](#role) resource.

Type annotations and code completion for `#!python session.resource("iam").roles` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.roles)

```python
# ServiceResourceRolesCollection usage example

from types_aiobotocore_iam.service_resource import ServiceResourceRolesCollection

def get_collection() -> ServiceResourceRolesCollection:
    return session.resource("iam").roles
```

### ServiceResourceSamlProvidersCollection

Provides access to [SamlProvider](#samlprovider) resource.

Type annotations and code completion for `#!python session.resource("iam").saml_providers` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.saml_providers)

```python
# ServiceResourceSamlProvidersCollection usage example

from types_aiobotocore_iam.service_resource import ServiceResourceSamlProvidersCollection

def get_collection() -> ServiceResourceSamlProvidersCollection:
    return session.resource("iam").saml_providers
```

### ServiceResourceServerCertificatesCollection

Provides access to [ServerCertificate](#servercertificate) resource.

Type annotations and code completion for `#!python session.resource("iam").server_certificates` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.server_certificates)

```python
# ServiceResourceServerCertificatesCollection usage example

from types_aiobotocore_iam.service_resource import ServiceResourceServerCertificatesCollection

def get_collection() -> ServiceResourceServerCertificatesCollection:
    return session.resource("iam").server_certificates
```

### ServiceResourceUsersCollection

Provides access to [User](#user) resource.

Type annotations and code completion for `#!python session.resource("iam").users` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.users)

```python
# ServiceResourceUsersCollection usage example

from types_aiobotocore_iam.service_resource import ServiceResourceUsersCollection

def get_collection() -> ServiceResourceUsersCollection:
    return session.resource("iam").users
```

### ServiceResourceVirtualMfaDevicesCollection

Provides access to [VirtualMfaDevice](#virtualmfadevice) resource.

Type annotations and code completion for `#!python session.resource("iam").virtual_mfa_devices` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.virtual_mfa_devices)

```python
# ServiceResourceVirtualMfaDevicesCollection usage example

from types_aiobotocore_iam.service_resource import ServiceResourceVirtualMfaDevicesCollection

def get_collection() -> ServiceResourceVirtualMfaDevicesCollection:
    return session.resource("iam").virtual_mfa_devices
```



## Methods

### IAMServiceResource.AccessKey method

Creates a AccessKey resource.

Type annotations and code completion for `#!python session.resource("iam").AccessKey` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AccessKey)

```python
# AccessKey method definition

await def AccessKey(
    self,
    user_name: str,
    id: str,
) -> AccessKey:
    ...
```


### IAMServiceResource.AccessKeyPair method

Creates a AccessKeyPair resource.

Type annotations and code completion for `#!python session.resource("iam").AccessKeyPair` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AccessKeyPair)

```python
# AccessKeyPair method definition

await def AccessKeyPair(
    self,
    user_name: str,
    id: str,
    secret: str,
) -> AccessKeyPair:
    ...
```


### IAMServiceResource.AccountPasswordPolicy method

Creates a AccountPasswordPolicy resource.

Type annotations and code completion for `#!python session.resource("iam").AccountPasswordPolicy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AccountPasswordPolicy)

```python
# AccountPasswordPolicy method definition

await def AccountPasswordPolicy(
    self,
) -> AccountPasswordPolicy:
    ...
```


### IAMServiceResource.AccountSummary method

Creates a AccountSummary resource.

Type annotations and code completion for `#!python session.resource("iam").AccountSummary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AccountSummary)

```python
# AccountSummary method definition

await def AccountSummary(
    self,
) -> AccountSummary:
    ...
```


### IAMServiceResource.AssumeRolePolicy method

Creates a AssumeRolePolicy resource.

Type annotations and code completion for `#!python session.resource("iam").AssumeRolePolicy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AssumeRolePolicy)

```python
# AssumeRolePolicy method definition

await def AssumeRolePolicy(
    self,
    role_name: str,
) -> AssumeRolePolicy:
    ...
```


### IAMServiceResource.CurrentUser method

Creates a CurrentUser resource.

Type annotations and code completion for `#!python session.resource("iam").CurrentUser` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.CurrentUser)

```python
# CurrentUser method definition

await def CurrentUser(
    self,
) -> CurrentUser:
    ...
```


### IAMServiceResource.Group method

Creates a Group resource.

Type annotations and code completion for `#!python session.resource("iam").Group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.Group)

```python
# Group method definition

await def Group(
    self,
    name: str,
) -> Group:
    ...
```


### IAMServiceResource.GroupPolicy method

Creates a GroupPolicy resource.

Type annotations and code completion for `#!python session.resource("iam").GroupPolicy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.GroupPolicy)

```python
# GroupPolicy method definition

await def GroupPolicy(
    self,
    group_name: str,
    name: str,
) -> GroupPolicy:
    ...
```


### IAMServiceResource.InstanceProfile method

Creates a InstanceProfile resource.

Type annotations and code completion for `#!python session.resource("iam").InstanceProfile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.InstanceProfile)

```python
# InstanceProfile method definition

await def InstanceProfile(
    self,
    name: str,
) -> InstanceProfile:
    ...
```


### IAMServiceResource.LoginProfile method

Creates a LoginProfile resource.

Type annotations and code completion for `#!python session.resource("iam").LoginProfile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.LoginProfile)

```python
# LoginProfile method definition

await def LoginProfile(
    self,
    user_name: str,
) -> LoginProfile:
    ...
```


### IAMServiceResource.MfaDevice method

Creates a MfaDevice resource.

Type annotations and code completion for `#!python session.resource("iam").MfaDevice` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.MfaDevice)

```python
# MfaDevice method definition

await def MfaDevice(
    self,
    user_name: str,
    serial_number: str,
) -> MfaDevice:
    ...
```


### IAMServiceResource.Policy method

Creates a Policy resource.

Type annotations and code completion for `#!python session.resource("iam").Policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.Policy)

```python
# Policy method definition

await def Policy(
    self,
    arn: str,
) -> Policy:
    ...
```


### IAMServiceResource.PolicyVersion method

Creates a PolicyVersion resource.

Type annotations and code completion for `#!python session.resource("iam").PolicyVersion` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.PolicyVersion)

```python
# PolicyVersion method definition

await def PolicyVersion(
    self,
    arn: str,
    version_id: str,
) -> PolicyVersion:
    ...
```


### IAMServiceResource.Role method

Creates a Role resource.

Type annotations and code completion for `#!python session.resource("iam").Role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.Role)

```python
# Role method definition

await def Role(
    self,
    name: str,
) -> Role:
    ...
```


### IAMServiceResource.RolePolicy method

Creates a RolePolicy resource.

Type annotations and code completion for `#!python session.resource("iam").RolePolicy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.RolePolicy)

```python
# RolePolicy method definition

await def RolePolicy(
    self,
    role_name: str,
    name: str,
) -> RolePolicy:
    ...
```


### IAMServiceResource.SamlProvider method

Creates a SamlProvider resource.

Type annotations and code completion for `#!python session.resource("iam").SamlProvider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.SamlProvider)

```python
# SamlProvider method definition

await def SamlProvider(
    self,
    arn: str,
) -> SamlProvider:
    ...
```


### IAMServiceResource.ServerCertificate method

Creates a ServerCertificate resource.

Type annotations and code completion for `#!python session.resource("iam").ServerCertificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.ServerCertificate)

```python
# ServerCertificate method definition

await def ServerCertificate(
    self,
    name: str,
) -> ServerCertificate:
    ...
```


### IAMServiceResource.SigningCertificate method

Creates a SigningCertificate resource.

Type annotations and code completion for `#!python session.resource("iam").SigningCertificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.SigningCertificate)

```python
# SigningCertificate method definition

await def SigningCertificate(
    self,
    user_name: str,
    id: str,
) -> SigningCertificate:
    ...
```


### IAMServiceResource.User method

Creates a User resource.

Type annotations and code completion for `#!python session.resource("iam").User` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.User)

```python
# User method definition

await def User(
    self,
    name: str,
) -> User:
    ...
```


### IAMServiceResource.UserPolicy method

Creates a UserPolicy resource.

Type annotations and code completion for `#!python session.resource("iam").UserPolicy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.UserPolicy)

```python
# UserPolicy method definition

await def UserPolicy(
    self,
    user_name: str,
    name: str,
) -> UserPolicy:
    ...
```


### IAMServiceResource.VirtualMfaDevice method

Creates a VirtualMfaDevice resource.

Type annotations and code completion for `#!python session.resource("iam").VirtualMfaDevice` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.VirtualMfaDevice)

```python
# VirtualMfaDevice method definition

await def VirtualMfaDevice(
    self,
    serial_number: str,
) -> VirtualMfaDevice:
    ...
```


### IAMServiceResource.change\_password method

Changes the password of the IAM user who is calling this operation.

Type annotations and code completion for `#!python session.resource("iam").change_password` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.change_password)

```python
# change_password method definition

await def change_password(
    self,
    *,
    OldPassword: str,
    NewPassword: str,
) -> None:
    ...
```



```python
# change_password method usage example with argument unpacking

kwargs: ChangePasswordRequestServiceResourceChangePasswordTypeDef = {  # (1)
    "OldPassword": ...,
    "NewPassword": ...,
}

parent.change_password(**kwargs)
```

1. See [:material-code-braces: ChangePasswordRequestServiceResourceChangePasswordTypeDef](./type_defs.md#changepasswordrequestserviceresourcechangepasswordtypedef) 

### IAMServiceResource.create\_account\_alias method

Creates an alias for your Amazon Web Services account.

Type annotations and code completion for `#!python session.resource("iam").create_account_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_account_alias)

```python
# create_account_alias method definition

await def create_account_alias(
    self,
    *,
    AccountAlias: str,
) -> None:
    ...
```



```python
# create_account_alias method usage example with argument unpacking

kwargs: CreateAccountAliasRequestServiceResourceCreateAccountAliasTypeDef = {  # (1)
    "AccountAlias": ...,
}

parent.create_account_alias(**kwargs)
```

1. See [:material-code-braces: CreateAccountAliasRequestServiceResourceCreateAccountAliasTypeDef](./type_defs.md#createaccountaliasrequestserviceresourcecreateaccountaliastypedef) 

### IAMServiceResource.create\_account\_password\_policy method

Updates the password policy settings for the Amazon Web Services account.

Type annotations and code completion for `#!python session.resource("iam").create_account_password_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_account_password_policy)

```python
# create_account_password_policy method definition

await def create_account_password_policy(
    self,
    *,
    MinimumPasswordLength: int = ...,
    RequireSymbols: bool = ...,
    RequireNumbers: bool = ...,
    RequireUppercaseCharacters: bool = ...,
    RequireLowercaseCharacters: bool = ...,
    AllowUsersToChangePassword: bool = ...,
    MaxPasswordAge: int = ...,
    PasswordReusePrevention: int = ...,
    HardExpiry: bool = ...,
) -> AccountPasswordPolicy:
    ...
```



```python
# create_account_password_policy method usage example with argument unpacking

kwargs: UpdateAccountPasswordPolicyRequestServiceResourceCreateAccountPasswordPolicyTypeDef = {  # (1)
    "MinimumPasswordLength": ...,
}

parent.create_account_password_policy(**kwargs)
```

1. See [:material-code-braces: UpdateAccountPasswordPolicyRequestServiceResourceCreateAccountPasswordPolicyTypeDef](./type_defs.md#updateaccountpasswordpolicyrequestserviceresourcecreateaccountpasswordpolicytypedef) 

### IAMServiceResource.create\_group method

Creates a new group.

Type annotations and code completion for `#!python session.resource("iam").create_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_group)

```python
# create_group method definition

await def create_group(
    self,
    *,
    GroupName: str,
    Path: str = ...,
) -> Group:
    ...
```



```python
# create_group method usage example with argument unpacking

kwargs: CreateGroupRequestServiceResourceCreateGroupTypeDef = {  # (1)
    "GroupName": ...,
}

parent.create_group(**kwargs)
```

1. See [:material-code-braces: CreateGroupRequestServiceResourceCreateGroupTypeDef](./type_defs.md#creategrouprequestserviceresourcecreategrouptypedef) 

### IAMServiceResource.create\_instance\_profile method

Creates a new instance profile.

Type annotations and code completion for `#!python session.resource("iam").create_instance_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_instance_profile)

```python
# create_instance_profile method definition

await def create_instance_profile(
    self,
    *,
    InstanceProfileName: str,
    Path: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> InstanceProfile:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# create_instance_profile method usage example with argument unpacking

kwargs: CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef = {  # (1)
    "InstanceProfileName": ...,
}

parent.create_instance_profile(**kwargs)
```

1. See [:material-code-braces: CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef](./type_defs.md#createinstanceprofilerequestserviceresourcecreateinstanceprofiletypedef) 

### IAMServiceResource.create\_policy method

Creates a new managed policy for your Amazon Web Services account.

Type annotations and code completion for `#!python session.resource("iam").create_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_policy)

```python
# create_policy method definition

await def create_policy(
    self,
    *,
    PolicyName: str,
    PolicyDocument: str,
    Path: str = ...,
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> Policy:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# create_policy method usage example with argument unpacking

kwargs: CreatePolicyRequestServiceResourceCreatePolicyTypeDef = {  # (1)
    "PolicyName": ...,
    "PolicyDocument": ...,
}

parent.create_policy(**kwargs)
```

1. See [:material-code-braces: CreatePolicyRequestServiceResourceCreatePolicyTypeDef](./type_defs.md#createpolicyrequestserviceresourcecreatepolicytypedef) 

### IAMServiceResource.create\_role method

Creates a new role for your Amazon Web Services account.

Type annotations and code completion for `#!python session.resource("iam").create_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_role)

```python
# create_role method definition

await def create_role(
    self,
    *,
    RoleName: str,
    AssumeRolePolicyDocument: str,
    Path: str = ...,
    Description: str = ...,
    MaxSessionDuration: int = ...,
    PermissionsBoundary: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> Role:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# create_role method usage example with argument unpacking

kwargs: CreateRoleRequestServiceResourceCreateRoleTypeDef = {  # (1)
    "RoleName": ...,
    "AssumeRolePolicyDocument": ...,
}

parent.create_role(**kwargs)
```

1. See [:material-code-braces: CreateRoleRequestServiceResourceCreateRoleTypeDef](./type_defs.md#createrolerequestserviceresourcecreateroletypedef) 

### IAMServiceResource.create\_saml\_provider method

Creates an IAM resource that describes an identity provider (IdP) that supports
SAML 2.0.

Type annotations and code completion for `#!python session.resource("iam").create_saml_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_saml_provider)

```python
# create_saml_provider method definition

await def create_saml_provider(
    self,
    *,
    SAMLMetadataDocument: str,
    Name: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> SamlProvider:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# create_saml_provider method usage example with argument unpacking

kwargs: CreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef = {  # (1)
    "SAMLMetadataDocument": ...,
    "Name": ...,
}

parent.create_saml_provider(**kwargs)
```

1. See [:material-code-braces: CreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef](./type_defs.md#createsamlproviderrequestserviceresourcecreatesamlprovidertypedef) 

### IAMServiceResource.create\_server\_certificate method

Uploads a server certificate entity for the Amazon Web Services account.

Type annotations and code completion for `#!python session.resource("iam").create_server_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_server_certificate)

```python
# create_server_certificate method definition

await def create_server_certificate(
    self,
    *,
    ServerCertificateName: str,
    CertificateBody: str,
    PrivateKey: str,
    Path: str = ...,
    CertificateChain: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> ServerCertificate:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# create_server_certificate method usage example with argument unpacking

kwargs: UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef = {  # (1)
    "ServerCertificateName": ...,
    "CertificateBody": ...,
    "PrivateKey": ...,
}

parent.create_server_certificate(**kwargs)
```

1. See [:material-code-braces: UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef](./type_defs.md#uploadservercertificaterequestserviceresourcecreateservercertificatetypedef) 

### IAMServiceResource.create\_signing\_certificate method

Uploads an X.509 signing certificate and associates it with the specified IAM
user.

Type annotations and code completion for `#!python session.resource("iam").create_signing_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_signing_certificate)

```python
# create_signing_certificate method definition

await def create_signing_certificate(
    self,
    *,
    CertificateBody: str,
    UserName: str = ...,
) -> SigningCertificate:
    ...
```



```python
# create_signing_certificate method usage example with argument unpacking

kwargs: UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef = {  # (1)
    "CertificateBody": ...,
}

parent.create_signing_certificate(**kwargs)
```

1. See [:material-code-braces: UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef](./type_defs.md#uploadsigningcertificaterequestserviceresourcecreatesigningcertificatetypedef) 

### IAMServiceResource.create\_user method

Creates a new IAM user for your Amazon Web Services account.

Type annotations and code completion for `#!python session.resource("iam").create_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_user)

```python
# create_user method definition

await def create_user(
    self,
    *,
    UserName: str,
    Path: str = ...,
    PermissionsBoundary: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> User:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# create_user method usage example with argument unpacking

kwargs: CreateUserRequestServiceResourceCreateUserTypeDef = {  # (1)
    "UserName": ...,
}

parent.create_user(**kwargs)
```

1. See [:material-code-braces: CreateUserRequestServiceResourceCreateUserTypeDef](./type_defs.md#createuserrequestserviceresourcecreateusertypedef) 

### IAMServiceResource.create\_virtual\_mfa\_device method

Creates a new virtual MFA device for the Amazon Web Services account.

Type annotations and code completion for `#!python session.resource("iam").create_virtual_mfa_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_virtual_mfa_device)

```python
# create_virtual_mfa_device method definition

await def create_virtual_mfa_device(
    self,
    *,
    VirtualMFADeviceName: str,
    Path: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> VirtualMfaDevice:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# create_virtual_mfa_device method usage example with argument unpacking

kwargs: CreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef = {  # (1)
    "VirtualMFADeviceName": ...,
}

parent.create_virtual_mfa_device(**kwargs)
```

1. See [:material-code-braces: CreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef](./type_defs.md#createvirtualmfadevicerequestserviceresourcecreatevirtualmfadevicetypedef) 

### IAMServiceResource.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python session.resource("iam").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```




## AccessKey

Type annotations and code completion for `#!python session.resource("iam").AccessKey` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AccessKey)

```python
# AccessKey usage example

from types_aiobotocore_iam.service_resource import AccessKey

def get_resource() -> AccessKey:
    return session.resource("iam").AccessKey(...)
```


### AccessKey attributes


- `access_key_id`: `Awaitable`[`str`]
- `status`: `Awaitable`[[statusTypeType](./literals.md#statustypetype)]
- `create_date`: `Awaitable`[`datetime`]
- `user_name`: `str`
- `id`: `str`





### AccessKey methods


#### AccessKey.User method

Creates a User resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").User` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccessKey.User)

```python
# User method definition

await def User(
    self,
) -> User:
    ...
```


#### AccessKey.activate method

Changes the status of the specified access key from Active to Inactive, or vice
versa.

Type annotations and code completion for `#!python aiobotocore.resource("iam").activate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccessKey.activate)

```python
# activate method definition

await def activate(
    self,
    *,
    Status: statusTypeType = 'Active',  # (1)
) -> None:
    ...
```

1. See [:material-code-brackets: statusTypeType](./literals.md#statustypetype) 


```python
# activate method usage example with argument unpacking

kwargs: UpdateAccessKeyRequestAccessKeyActivateTypeDef = {  # (1)
    "Status": ...,
}

parent.activate(**kwargs)
```

1. See [:material-code-braces: UpdateAccessKeyRequestAccessKeyActivateTypeDef](./type_defs.md#updateaccesskeyrequestaccesskeyactivatetypedef) 

#### AccessKey.deactivate method

Changes the status of the specified access key from Active to Inactive, or vice
versa.

Type annotations and code completion for `#!python aiobotocore.resource("iam").deactivate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccessKey.deactivate)

```python
# deactivate method definition

await def deactivate(
    self,
    *,
    Status: statusTypeType = 'Inactive',  # (1)
) -> None:
    ...
```

1. See [:material-code-brackets: statusTypeType](./literals.md#statustypetype) 


```python
# deactivate method usage example with argument unpacking

kwargs: UpdateAccessKeyRequestAccessKeyDeactivateTypeDef = {  # (1)
    "Status": ...,
}

parent.deactivate(**kwargs)
```

1. See [:material-code-braces: UpdateAccessKeyRequestAccessKeyDeactivateTypeDef](./type_defs.md#updateaccesskeyrequestaccesskeydeactivatetypedef) 

#### AccessKey.delete method

Deletes the access key pair associated with the specified IAM user.

Type annotations and code completion for `#!python aiobotocore.resource("iam").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccessKey.delete)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### AccessKey.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccessKey.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```





## AccessKeyPair

Type annotations and code completion for `#!python session.resource("iam").AccessKeyPair` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AccessKeyPair)

```python
# AccessKeyPair usage example

from types_aiobotocore_iam.service_resource import AccessKeyPair

def get_resource() -> AccessKeyPair:
    return session.resource("iam").AccessKeyPair(...)
```


### AccessKeyPair attributes


- `access_key_id`: `Awaitable`[`str`]
- `status`: `Awaitable`[[statusTypeType](./literals.md#statustypetype)]
- `secret_access_key`: `Awaitable`[`str`]
- `create_date`: `Awaitable`[`datetime`]
- `user_name`: `str`
- `id`: `str`
- `secret`: `str`





### AccessKeyPair methods


#### AccessKeyPair.activate method

Changes the status of the specified access key from Active to Inactive, or vice
versa.

Type annotations and code completion for `#!python aiobotocore.resource("iam").activate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccessKeyPair.activate)

```python
# activate method definition

await def activate(
    self,
    *,
    Status: statusTypeType = 'Active',  # (1)
) -> None:
    ...
```

1. See [:material-code-brackets: statusTypeType](./literals.md#statustypetype) 


```python
# activate method usage example with argument unpacking

kwargs: UpdateAccessKeyRequestAccessKeyPairActivateTypeDef = {  # (1)
    "Status": ...,
}

parent.activate(**kwargs)
```

1. See [:material-code-braces: UpdateAccessKeyRequestAccessKeyPairActivateTypeDef](./type_defs.md#updateaccesskeyrequestaccesskeypairactivatetypedef) 

#### AccessKeyPair.deactivate method

Changes the status of the specified access key from Active to Inactive, or vice
versa.

Type annotations and code completion for `#!python aiobotocore.resource("iam").deactivate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccessKeyPair.deactivate)

```python
# deactivate method definition

await def deactivate(
    self,
    *,
    Status: statusTypeType = 'Inactive',  # (1)
) -> None:
    ...
```

1. See [:material-code-brackets: statusTypeType](./literals.md#statustypetype) 


```python
# deactivate method usage example with argument unpacking

kwargs: UpdateAccessKeyRequestAccessKeyPairDeactivateTypeDef = {  # (1)
    "Status": ...,
}

parent.deactivate(**kwargs)
```

1. See [:material-code-braces: UpdateAccessKeyRequestAccessKeyPairDeactivateTypeDef](./type_defs.md#updateaccesskeyrequestaccesskeypairdeactivatetypedef) 

#### AccessKeyPair.delete method

Deletes the access key pair associated with the specified IAM user.

Type annotations and code completion for `#!python aiobotocore.resource("iam").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccessKeyPair.delete)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### AccessKeyPair.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccessKeyPair.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```





## AccountPasswordPolicy

Type annotations and code completion for `#!python session.resource("iam").AccountPasswordPolicy` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AccountPasswordPolicy)

```python
# AccountPasswordPolicy usage example

from types_aiobotocore_iam.service_resource import AccountPasswordPolicy

def get_resource() -> AccountPasswordPolicy:
    return session.resource("iam").AccountPasswordPolicy(...)
```


### AccountPasswordPolicy attributes


- `minimum_password_length`: `Awaitable`[`int`]
- `require_symbols`: `Awaitable`[`bool`]
- `require_numbers`: `Awaitable`[`bool`]
- `require_uppercase_characters`: `Awaitable`[`bool`]
- `require_lowercase_characters`: `Awaitable`[`bool`]
- `allow_users_to_change_password`: `Awaitable`[`bool`]
- `expire_passwords`: `Awaitable`[`bool`]
- `max_password_age`: `Awaitable`[`int`]
- `password_reuse_prevention`: `Awaitable`[`int`]
- `hard_expiry`: `Awaitable`[`bool`]





### AccountPasswordPolicy methods


#### AccountPasswordPolicy.delete method

Deletes the password policy for the Amazon Web Services account.

Type annotations and code completion for `#!python aiobotocore.resource("iam").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccountPasswordPolicy.delete)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### AccountPasswordPolicy.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccountPasswordPolicy.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### AccountPasswordPolicy.load method

Calls :py:meth:`IAM.Client.get_account_password_policy` to update the attributes
of the AccountPasswordPolicy resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccountPasswordPolicy.load)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### AccountPasswordPolicy.reload method

Calls :py:meth:`IAM.Client.get_account_password_policy` to update the attributes
of the AccountPasswordPolicy resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccountPasswordPolicy.reload)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```


#### AccountPasswordPolicy.update method

Updates the password policy settings for the Amazon Web Services account.

Type annotations and code completion for `#!python aiobotocore.resource("iam").update` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccountPasswordPolicy.update)

```python
# update method definition

await def update(
    self,
    *,
    MinimumPasswordLength: int = ...,
    RequireSymbols: bool = ...,
    RequireNumbers: bool = ...,
    RequireUppercaseCharacters: bool = ...,
    RequireLowercaseCharacters: bool = ...,
    AllowUsersToChangePassword: bool = ...,
    MaxPasswordAge: int = ...,
    PasswordReusePrevention: int = ...,
    HardExpiry: bool = ...,
) -> None:
    ...
```



```python
# update method usage example with argument unpacking

kwargs: UpdateAccountPasswordPolicyRequestAccountPasswordPolicyUpdateTypeDef = {  # (1)
    "MinimumPasswordLength": ...,
}

parent.update(**kwargs)
```

1. See [:material-code-braces: UpdateAccountPasswordPolicyRequestAccountPasswordPolicyUpdateTypeDef](./type_defs.md#updateaccountpasswordpolicyrequestaccountpasswordpolicyupdatetypedef) 




## AccountSummary

Type annotations and code completion for `#!python session.resource("iam").AccountSummary` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AccountSummary)

```python
# AccountSummary usage example

from types_aiobotocore_iam.service_resource import AccountSummary

def get_resource() -> AccountSummary:
    return session.resource("iam").AccountSummary(...)
```


### AccountSummary attributes


- `summary_map`: `Awaitable`[`Dict`[[summaryKeyTypeType](./literals.md#summarykeytypetype), `int`]]





### AccountSummary methods


#### AccountSummary.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccountSummary.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### AccountSummary.load method

Calls :py:meth:`IAM.Client.get_account_summary` to update the attributes of the
AccountSummary resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccountSummary.load)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### AccountSummary.reload method

Calls :py:meth:`IAM.Client.get_account_summary` to update the attributes of the
AccountSummary resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccountSummary.reload)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## AssumeRolePolicy

Type annotations and code completion for `#!python session.resource("iam").AssumeRolePolicy` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AssumeRolePolicy)

```python
# AssumeRolePolicy usage example

from types_aiobotocore_iam.service_resource import AssumeRolePolicy

def get_resource() -> AssumeRolePolicy:
    return session.resource("iam").AssumeRolePolicy(...)
```


### AssumeRolePolicy attributes


- `role_name`: `str`





### AssumeRolePolicy methods


#### AssumeRolePolicy.Role method

Creates a Role resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").Role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AssumeRolePolicy.Role)

```python
# Role method definition

await def Role(
    self,
) -> Role:
    ...
```


#### AssumeRolePolicy.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AssumeRolePolicy.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### AssumeRolePolicy.update method

Updates the policy that grants an IAM entity permission to assume a role.

Type annotations and code completion for `#!python aiobotocore.resource("iam").update` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AssumeRolePolicy.update)

```python
# update method definition

await def update(
    self,
    *,
    PolicyDocument: str,
) -> None:
    ...
```



```python
# update method usage example with argument unpacking

kwargs: UpdateAssumeRolePolicyRequestAssumeRolePolicyUpdateTypeDef = {  # (1)
    "PolicyDocument": ...,
}

parent.update(**kwargs)
```

1. See [:material-code-braces: UpdateAssumeRolePolicyRequestAssumeRolePolicyUpdateTypeDef](./type_defs.md#updateassumerolepolicyrequestassumerolepolicyupdatetypedef) 




## CurrentUser

Type annotations and code completion for `#!python session.resource("iam").CurrentUser` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.CurrentUser)

```python
# CurrentUser usage example

from types_aiobotocore_iam.service_resource import CurrentUser

def get_resource() -> CurrentUser:
    return session.resource("iam").CurrentUser(...)
```


### CurrentUser attributes


- `path`: `Awaitable`[`str`]
- `user_name`: `Awaitable`[`str`]
- `user_id`: `Awaitable`[`str`]
- `arn`: `Awaitable`[`str`]
- `create_date`: `Awaitable`[`datetime`]
- `password_last_used`: `Awaitable`[`datetime`]
- `permissions_boundary`: `Awaitable`[[AttachedPermissionsBoundaryTypeDef](./type_defs.md#attachedpermissionsboundarytypedef)]
- `tags`: `Awaitable`[`List`[[TagTypeDef](./type_defs.md#tagtypedef)]]
- `user`: [User](#user)
- `access_keys`: [CurrentUserAccessKeysCollection](#currentuseraccesskeyscollection)
- `mfa_devices`: [CurrentUserMfaDevicesCollection](#currentusermfadevicescollection)
- `signing_certificates`: [CurrentUserSigningCertificatesCollection](#currentusersigningcertificatescollection)



### CurrentUser collections


#### CurrentUser.access_keys

Provides access to [AccessKey](#accesskey) resource.

Type annotations and code completion for `#!python session.resource("iam").CurrentUser(...).access_keys` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.CurrentUser.access_keys)

```python
# CurrentUserAccessKeysCollection usage example

from types_aiobotocore_iam.service_resource import CurrentUserAccessKeysCollection

def get_collection() -> CurrentUserAccessKeysCollection:
    resource = session.resource("iam").CurrentUser(...)
    return resource.access_keys
```

#### CurrentUser.mfa_devices

Provides access to [MfaDevice](#mfadevice) resource.

Type annotations and code completion for `#!python session.resource("iam").CurrentUser(...).mfa_devices` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.CurrentUser.mfa_devices)

```python
# CurrentUserMfaDevicesCollection usage example

from types_aiobotocore_iam.service_resource import CurrentUserMfaDevicesCollection

def get_collection() -> CurrentUserMfaDevicesCollection:
    resource = session.resource("iam").CurrentUser(...)
    return resource.mfa_devices
```

#### CurrentUser.signing_certificates

Provides access to [SigningCertificate](#signingcertificate) resource.

Type annotations and code completion for `#!python session.resource("iam").CurrentUser(...).signing_certificates` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.CurrentUser.signing_certificates)

```python
# CurrentUserSigningCertificatesCollection usage example

from types_aiobotocore_iam.service_resource import CurrentUserSigningCertificatesCollection

def get_collection() -> CurrentUserSigningCertificatesCollection:
    resource = session.resource("iam").CurrentUser(...)
    return resource.signing_certificates
```




### CurrentUser methods


#### CurrentUser.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.CurrentUser.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### CurrentUser.load method

Calls :py:meth:`IAM.Client.get_user` to update the attributes of the CurrentUser
resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.CurrentUser.load)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### CurrentUser.reload method

Calls :py:meth:`IAM.Client.get_user` to update the attributes of the CurrentUser
resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.CurrentUser.reload)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## Group

Type annotations and code completion for `#!python session.resource("iam").Group` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.Group)

```python
# Group usage example

from types_aiobotocore_iam.service_resource import Group

def get_resource() -> Group:
    return session.resource("iam").Group(...)
```


### Group attributes


- `path`: `Awaitable`[`str`]
- `group_name`: `Awaitable`[`str`]
- `group_id`: `Awaitable`[`str`]
- `arn`: `Awaitable`[`str`]
- `create_date`: `Awaitable`[`datetime`]
- `name`: `str`
- `attached_policies`: [GroupAttachedPoliciesCollection](#groupattachedpoliciescollection)
- `policies`: [GroupPoliciesCollection](#grouppoliciescollection)
- `users`: [GroupUsersCollection](#groupuserscollection)



### Group collections


#### Group.attached_policies

Provides access to [Policy](#policy) resource.

Type annotations and code completion for `#!python session.resource("iam").Group(...).attached_policies` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.attached_policies)

```python
# GroupAttachedPoliciesCollection usage example

from types_aiobotocore_iam.service_resource import GroupAttachedPoliciesCollection

def get_collection() -> GroupAttachedPoliciesCollection:
    resource = session.resource("iam").Group(...)
    return resource.attached_policies
```

#### Group.policies

Provides access to [GroupPolicy](#grouppolicy) resource.

Type annotations and code completion for `#!python session.resource("iam").Group(...).policies` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.policies)

```python
# GroupPoliciesCollection usage example

from types_aiobotocore_iam.service_resource import GroupPoliciesCollection

def get_collection() -> GroupPoliciesCollection:
    resource = session.resource("iam").Group(...)
    return resource.policies
```

#### Group.users

Provides access to [User](#user) resource.

Type annotations and code completion for `#!python session.resource("iam").Group(...).users` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.users)

```python
# GroupUsersCollection usage example

from types_aiobotocore_iam.service_resource import GroupUsersCollection

def get_collection() -> GroupUsersCollection:
    resource = session.resource("iam").Group(...)
    return resource.users
```




### Group methods


#### Group.Policy method

Creates a GroupPolicy resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").Policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.Policy)

```python
# Policy method definition

await def Policy(
    self,
    name: str,
) -> GroupPolicy:
    ...
```


#### Group.add\_user method

Adds the specified user to the specified group.

Type annotations and code completion for `#!python aiobotocore.resource("iam").add_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.add_user)

```python
# add_user method definition

await def add_user(
    self,
    *,
    UserName: str,
) -> None:
    ...
```



```python
# add_user method usage example with argument unpacking

kwargs: AddUserToGroupRequestGroupAddUserTypeDef = {  # (1)
    "UserName": ...,
}

parent.add_user(**kwargs)
```

1. See [:material-code-braces: AddUserToGroupRequestGroupAddUserTypeDef](./type_defs.md#addusertogrouprequestgroupaddusertypedef) 

#### Group.attach\_policy method

Attaches the specified managed policy to the specified IAM group.

Type annotations and code completion for `#!python aiobotocore.resource("iam").attach_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.attach_policy)

```python
# attach_policy method definition

await def attach_policy(
    self,
    *,
    PolicyArn: str,
) -> None:
    ...
```



```python
# attach_policy method usage example with argument unpacking

kwargs: AttachGroupPolicyRequestGroupAttachPolicyTypeDef = {  # (1)
    "PolicyArn": ...,
}

parent.attach_policy(**kwargs)
```

1. See [:material-code-braces: AttachGroupPolicyRequestGroupAttachPolicyTypeDef](./type_defs.md#attachgrouppolicyrequestgroupattachpolicytypedef) 

#### Group.create method

Creates a new group.

Type annotations and code completion for `#!python aiobotocore.resource("iam").create` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.create)

```python
# create method definition

await def create(
    self,
    *,
    Path: str = ...,
) -> Group:
    ...
```



```python
# create method usage example with argument unpacking

kwargs: CreateGroupRequestGroupCreateTypeDef = {  # (1)
    "Path": ...,
}

parent.create(**kwargs)
```

1. See [:material-code-braces: CreateGroupRequestGroupCreateTypeDef](./type_defs.md#creategrouprequestgroupcreatetypedef) 

#### Group.create\_policy method

Adds or updates an inline policy document that is embedded in the specified IAM
group.

Type annotations and code completion for `#!python aiobotocore.resource("iam").create_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.create_policy)

```python
# create_policy method definition

await def create_policy(
    self,
    *,
    PolicyName: str,
    PolicyDocument: str,
) -> GroupPolicy:
    ...
```



```python
# create_policy method usage example with argument unpacking

kwargs: PutGroupPolicyRequestGroupCreatePolicyTypeDef = {  # (1)
    "PolicyName": ...,
    "PolicyDocument": ...,
}

parent.create_policy(**kwargs)
```

1. See [:material-code-braces: PutGroupPolicyRequestGroupCreatePolicyTypeDef](./type_defs.md#putgrouppolicyrequestgroupcreatepolicytypedef) 

#### Group.delete method

Deletes the specified IAM group.

Type annotations and code completion for `#!python aiobotocore.resource("iam").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.delete)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### Group.detach\_policy method

Removes the specified managed policy from the specified IAM group.

Type annotations and code completion for `#!python aiobotocore.resource("iam").detach_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.detach_policy)

```python
# detach_policy method definition

await def detach_policy(
    self,
    *,
    PolicyArn: str,
) -> None:
    ...
```



```python
# detach_policy method usage example with argument unpacking

kwargs: DetachGroupPolicyRequestGroupDetachPolicyTypeDef = {  # (1)
    "PolicyArn": ...,
}

parent.detach_policy(**kwargs)
```

1. See [:material-code-braces: DetachGroupPolicyRequestGroupDetachPolicyTypeDef](./type_defs.md#detachgrouppolicyrequestgroupdetachpolicytypedef) 

#### Group.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### Group.load method

Calls :py:meth:`IAM.Client.get_group` to update the attributes of the Group
resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.load)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### Group.reload method

Calls :py:meth:`IAM.Client.get_group` to update the attributes of the Group
resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.reload)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```


#### Group.remove\_user method

Removes the specified user from the specified group.

Type annotations and code completion for `#!python aiobotocore.resource("iam").remove_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.remove_user)

```python
# remove_user method definition

await def remove_user(
    self,
    *,
    UserName: str,
) -> None:
    ...
```



```python
# remove_user method usage example with argument unpacking

kwargs: RemoveUserFromGroupRequestGroupRemoveUserTypeDef = {  # (1)
    "UserName": ...,
}

parent.remove_user(**kwargs)
```

1. See [:material-code-braces: RemoveUserFromGroupRequestGroupRemoveUserTypeDef](./type_defs.md#removeuserfromgrouprequestgroupremoveusertypedef) 

#### Group.update method

Updates the name and/or the path of the specified IAM group.

Type annotations and code completion for `#!python aiobotocore.resource("iam").update` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.update)

```python
# update method definition

await def update(
    self,
    *,
    NewPath: str = ...,
    NewGroupName: str = ...,
) -> Group:
    ...
```



```python
# update method usage example with argument unpacking

kwargs: UpdateGroupRequestGroupUpdateTypeDef = {  # (1)
    "NewPath": ...,
}

parent.update(**kwargs)
```

1. See [:material-code-braces: UpdateGroupRequestGroupUpdateTypeDef](./type_defs.md#updategrouprequestgroupupdatetypedef) 




## GroupPolicy

Type annotations and code completion for `#!python session.resource("iam").GroupPolicy` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.GroupPolicy)

```python
# GroupPolicy usage example

from types_aiobotocore_iam.service_resource import GroupPolicy

def get_resource() -> GroupPolicy:
    return session.resource("iam").GroupPolicy(...)
```


### GroupPolicy attributes


- `policy_name`: `Awaitable`[`str`]
- `policy_document`: `Awaitable`[`str`]
- `group_name`: `str`
- `name`: `str`





### GroupPolicy methods


#### GroupPolicy.Group method

Creates a Group resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").Group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.GroupPolicy.Group)

```python
# Group method definition

await def Group(
    self,
) -> Group:
    ...
```


#### GroupPolicy.delete method

Deletes the specified inline policy that is embedded in the specified IAM group.

Type annotations and code completion for `#!python aiobotocore.resource("iam").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.GroupPolicy.delete)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### GroupPolicy.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.GroupPolicy.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### GroupPolicy.load method

Calls :py:meth:`IAM.Client.get_group_policy` to update the attributes of the
GroupPolicy resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.GroupPolicy.load)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### GroupPolicy.put method

Adds or updates an inline policy document that is embedded in the specified IAM
group.

Type annotations and code completion for `#!python aiobotocore.resource("iam").put` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.GroupPolicy.put)

```python
# put method definition

await def put(
    self,
    *,
    PolicyDocument: str,
) -> None:
    ...
```



```python
# put method usage example with argument unpacking

kwargs: PutGroupPolicyRequestGroupPolicyPutTypeDef = {  # (1)
    "PolicyDocument": ...,
}

parent.put(**kwargs)
```

1. See [:material-code-braces: PutGroupPolicyRequestGroupPolicyPutTypeDef](./type_defs.md#putgrouppolicyrequestgrouppolicyputtypedef) 

#### GroupPolicy.reload method

Calls :py:meth:`IAM.Client.get_group_policy` to update the attributes of the
GroupPolicy resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.GroupPolicy.reload)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## InstanceProfile

Type annotations and code completion for `#!python session.resource("iam").InstanceProfile` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.InstanceProfile)

```python
# InstanceProfile usage example

from types_aiobotocore_iam.service_resource import InstanceProfile

def get_resource() -> InstanceProfile:
    return session.resource("iam").InstanceProfile(...)
```


### InstanceProfile attributes


- `path`: `Awaitable`[`str`]
- `instance_profile_name`: `Awaitable`[`str`]
- `instance_profile_id`: `Awaitable`[`str`]
- `arn`: `Awaitable`[`str`]
- `create_date`: `Awaitable`[`datetime`]
- `roles_attribute`: `Awaitable`[`List`[[RoleTypeDef](./type_defs.md#roletypedef)]]
- `tags`: `Awaitable`[`List`[[TagTypeDef](./type_defs.md#tagtypedef)]]
- `name`: `str`
- `roles`: `List`[[Role](#role)]





### InstanceProfile methods


#### InstanceProfile.add\_role method

Adds the specified IAM role to the specified instance profile.

Type annotations and code completion for `#!python aiobotocore.resource("iam").add_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.InstanceProfile.add_role)

```python
# add_role method definition

await def add_role(
    self,
    *,
    RoleName: str,
) -> None:
    ...
```



```python
# add_role method usage example with argument unpacking

kwargs: AddRoleToInstanceProfileRequestInstanceProfileAddRoleTypeDef = {  # (1)
    "RoleName": ...,
}

parent.add_role(**kwargs)
```

1. See [:material-code-braces: AddRoleToInstanceProfileRequestInstanceProfileAddRoleTypeDef](./type_defs.md#addroletoinstanceprofilerequestinstanceprofileaddroletypedef) 

#### InstanceProfile.delete method

Deletes the specified instance profile.

Type annotations and code completion for `#!python aiobotocore.resource("iam").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.InstanceProfile.delete)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### InstanceProfile.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.InstanceProfile.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### InstanceProfile.load method

Calls :py:meth:`IAM.Client.get_instance_profile` to update the attributes of the
InstanceProfile resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.InstanceProfile.load)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### InstanceProfile.reload method

Calls :py:meth:`IAM.Client.get_instance_profile` to update the attributes of the
InstanceProfile resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.InstanceProfile.reload)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```


#### InstanceProfile.remove\_role method

Removes the specified IAM role from the specified EC2 instance profile.

Type annotations and code completion for `#!python aiobotocore.resource("iam").remove_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.InstanceProfile.remove_role)

```python
# remove_role method definition

await def remove_role(
    self,
    *,
    RoleName: str,
) -> None:
    ...
```



```python
# remove_role method usage example with argument unpacking

kwargs: RemoveRoleFromInstanceProfileRequestInstanceProfileRemoveRoleTypeDef = {  # (1)
    "RoleName": ...,
}

parent.remove_role(**kwargs)
```

1. See [:material-code-braces: RemoveRoleFromInstanceProfileRequestInstanceProfileRemoveRoleTypeDef](./type_defs.md#removerolefrominstanceprofilerequestinstanceprofileremoveroletypedef) 




## LoginProfile

Type annotations and code completion for `#!python session.resource("iam").LoginProfile` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.LoginProfile)

```python
# LoginProfile usage example

from types_aiobotocore_iam.service_resource import LoginProfile

def get_resource() -> LoginProfile:
    return session.resource("iam").LoginProfile(...)
```


### LoginProfile attributes


- `create_date`: `Awaitable`[`datetime`]
- `password_reset_required`: `Awaitable`[`bool`]
- `user_name`: `str`





### LoginProfile methods


#### LoginProfile.User method

Creates a User resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").User` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.LoginProfile.User)

```python
# User method definition

await def User(
    self,
) -> User:
    ...
```


#### LoginProfile.create method

Creates a password for the specified IAM user.

Type annotations and code completion for `#!python aiobotocore.resource("iam").create` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.LoginProfile.create)

```python
# create method definition

await def create(
    self,
    *,
    Password: str,
    PasswordResetRequired: bool = ...,
) -> LoginProfile:
    ...
```



```python
# create method usage example with argument unpacking

kwargs: CreateLoginProfileRequestLoginProfileCreateTypeDef = {  # (1)
    "Password": ...,
}

parent.create(**kwargs)
```

1. See [:material-code-braces: CreateLoginProfileRequestLoginProfileCreateTypeDef](./type_defs.md#createloginprofilerequestloginprofilecreatetypedef) 

#### LoginProfile.delete method

Deletes the password for the specified IAM user, For more information, see
[Managing passwords for IAM
users](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_passwords_admin-
change-user.html)_.

Type annotations and code completion for `#!python aiobotocore.resource("iam").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.LoginProfile.delete)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### LoginProfile.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.LoginProfile.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### LoginProfile.load method

Calls :py:meth:`IAM.Client.get_login_profile` to update the attributes of the
LoginProfile resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.LoginProfile.load)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### LoginProfile.reload method

Calls :py:meth:`IAM.Client.get_login_profile` to update the attributes of the
LoginProfile resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.LoginProfile.reload)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```


#### LoginProfile.update method

Changes the password for the specified IAM user.

Type annotations and code completion for `#!python aiobotocore.resource("iam").update` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.LoginProfile.update)

```python
# update method definition

await def update(
    self,
    *,
    Password: str = ...,
    PasswordResetRequired: bool = ...,
) -> None:
    ...
```



```python
# update method usage example with argument unpacking

kwargs: UpdateLoginProfileRequestLoginProfileUpdateTypeDef = {  # (1)
    "Password": ...,
}

parent.update(**kwargs)
```

1. See [:material-code-braces: UpdateLoginProfileRequestLoginProfileUpdateTypeDef](./type_defs.md#updateloginprofilerequestloginprofileupdatetypedef) 




## MfaDevice

Type annotations and code completion for `#!python session.resource("iam").MfaDevice` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.MfaDevice)

```python
# MfaDevice usage example

from types_aiobotocore_iam.service_resource import MfaDevice

def get_resource() -> MfaDevice:
    return session.resource("iam").MfaDevice(...)
```


### MfaDevice attributes


- `enable_date`: `Awaitable`[`datetime`]
- `user_name`: `str`
- `serial_number`: `str`





### MfaDevice methods


#### MfaDevice.User method

Creates a User resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").User` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.MfaDevice.User)

```python
# User method definition

await def User(
    self,
) -> User:
    ...
```


#### MfaDevice.associate method

Enables the specified MFA device and associates it with the specified IAM user.

Type annotations and code completion for `#!python aiobotocore.resource("iam").associate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.MfaDevice.associate)

```python
# associate method definition

await def associate(
    self,
    *,
    AuthenticationCode1: str,
    AuthenticationCode2: str,
) -> None:
    ...
```



```python
# associate method usage example with argument unpacking

kwargs: EnableMFADeviceRequestMfaDeviceAssociateTypeDef = {  # (1)
    "AuthenticationCode1": ...,
    "AuthenticationCode2": ...,
}

parent.associate(**kwargs)
```

1. See [:material-code-braces: EnableMFADeviceRequestMfaDeviceAssociateTypeDef](./type_defs.md#enablemfadevicerequestmfadeviceassociatetypedef) 

#### MfaDevice.disassociate method

Deactivates the specified MFA device and removes it from association with the
user name for which it was originally enabled.

Type annotations and code completion for `#!python aiobotocore.resource("iam").disassociate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.MfaDevice.disassociate)

```python
# disassociate method definition

await def disassociate(
    self,
) -> None:
    ...
```


#### MfaDevice.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.MfaDevice.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### MfaDevice.resync method

Synchronizes the specified MFA device with its IAM resource object on the Amazon
Web Services servers.

Type annotations and code completion for `#!python aiobotocore.resource("iam").resync` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.MfaDevice.resync)

```python
# resync method definition

await def resync(
    self,
    *,
    AuthenticationCode1: str,
    AuthenticationCode2: str,
) -> None:
    ...
```



```python
# resync method usage example with argument unpacking

kwargs: ResyncMFADeviceRequestMfaDeviceResyncTypeDef = {  # (1)
    "AuthenticationCode1": ...,
    "AuthenticationCode2": ...,
}

parent.resync(**kwargs)
```

1. See [:material-code-braces: ResyncMFADeviceRequestMfaDeviceResyncTypeDef](./type_defs.md#resyncmfadevicerequestmfadeviceresynctypedef) 




## Policy

Type annotations and code completion for `#!python session.resource("iam").Policy` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.Policy)

```python
# Policy usage example

from types_aiobotocore_iam.service_resource import Policy

def get_resource() -> Policy:
    return session.resource("iam").Policy(...)
```


### Policy attributes


- `policy_name`: `Awaitable`[`str`]
- `policy_id`: `Awaitable`[`str`]
- `path`: `Awaitable`[`str`]
- `default_version_id`: `Awaitable`[`str`]
- `attachment_count`: `Awaitable`[`int`]
- `permissions_boundary_usage_count`: `Awaitable`[`int`]
- `is_attachable`: `Awaitable`[`bool`]
- `description`: `Awaitable`[`str`]
- `create_date`: `Awaitable`[`datetime`]
- `update_date`: `Awaitable`[`datetime`]
- `tags`: `Awaitable`[`List`[[TagTypeDef](./type_defs.md#tagtypedef)]]
- `arn`: `str`
- `default_version`: [PolicyVersion](#policyversion)
- `attached_groups`: [PolicyAttachedGroupsCollection](#policyattachedgroupscollection)
- `attached_roles`: [PolicyAttachedRolesCollection](#policyattachedrolescollection)
- `attached_users`: [PolicyAttachedUsersCollection](#policyattacheduserscollection)
- `versions`: [PolicyVersionsCollection](#policyversionscollection)



### Policy collections


#### Policy.attached_groups

Provides access to [Group](#group) resource.

Type annotations and code completion for `#!python session.resource("iam").Policy(...).attached_groups` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.attached_groups)

```python
# PolicyAttachedGroupsCollection usage example

from types_aiobotocore_iam.service_resource import PolicyAttachedGroupsCollection

def get_collection() -> PolicyAttachedGroupsCollection:
    resource = session.resource("iam").Policy(...)
    return resource.attached_groups
```

#### Policy.attached_roles

Provides access to [Role](#role) resource.

Type annotations and code completion for `#!python session.resource("iam").Policy(...).attached_roles` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.attached_roles)

```python
# PolicyAttachedRolesCollection usage example

from types_aiobotocore_iam.service_resource import PolicyAttachedRolesCollection

def get_collection() -> PolicyAttachedRolesCollection:
    resource = session.resource("iam").Policy(...)
    return resource.attached_roles
```

#### Policy.attached_users

Provides access to [User](#user) resource.

Type annotations and code completion for `#!python session.resource("iam").Policy(...).attached_users` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.attached_users)

```python
# PolicyAttachedUsersCollection usage example

from types_aiobotocore_iam.service_resource import PolicyAttachedUsersCollection

def get_collection() -> PolicyAttachedUsersCollection:
    resource = session.resource("iam").Policy(...)
    return resource.attached_users
```

#### Policy.versions

Provides access to [PolicyVersion](#policyversion) resource.

Type annotations and code completion for `#!python session.resource("iam").Policy(...).versions` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.versions)

```python
# PolicyVersionsCollection usage example

from types_aiobotocore_iam.service_resource import PolicyVersionsCollection

def get_collection() -> PolicyVersionsCollection:
    resource = session.resource("iam").Policy(...)
    return resource.versions
```




### Policy methods


#### Policy.attach\_group method

Attaches the specified managed policy to the specified IAM group.

Type annotations and code completion for `#!python aiobotocore.resource("iam").attach_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.attach_group)

```python
# attach_group method definition

await def attach_group(
    self,
    *,
    GroupName: str,
) -> None:
    ...
```



```python
# attach_group method usage example with argument unpacking

kwargs: AttachGroupPolicyRequestPolicyAttachGroupTypeDef = {  # (1)
    "GroupName": ...,
}

parent.attach_group(**kwargs)
```

1. See [:material-code-braces: AttachGroupPolicyRequestPolicyAttachGroupTypeDef](./type_defs.md#attachgrouppolicyrequestpolicyattachgrouptypedef) 

#### Policy.attach\_role method

Attaches the specified managed policy to the specified IAM role.

Type annotations and code completion for `#!python aiobotocore.resource("iam").attach_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.attach_role)

```python
# attach_role method definition

await def attach_role(
    self,
    *,
    RoleName: str,
) -> None:
    ...
```



```python
# attach_role method usage example with argument unpacking

kwargs: AttachRolePolicyRequestPolicyAttachRoleTypeDef = {  # (1)
    "RoleName": ...,
}

parent.attach_role(**kwargs)
```

1. See [:material-code-braces: AttachRolePolicyRequestPolicyAttachRoleTypeDef](./type_defs.md#attachrolepolicyrequestpolicyattachroletypedef) 

#### Policy.attach\_user method

Attaches the specified managed policy to the specified user.

Type annotations and code completion for `#!python aiobotocore.resource("iam").attach_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.attach_user)

```python
# attach_user method definition

await def attach_user(
    self,
    *,
    UserName: str,
) -> None:
    ...
```



```python
# attach_user method usage example with argument unpacking

kwargs: AttachUserPolicyRequestPolicyAttachUserTypeDef = {  # (1)
    "UserName": ...,
}

parent.attach_user(**kwargs)
```

1. See [:material-code-braces: AttachUserPolicyRequestPolicyAttachUserTypeDef](./type_defs.md#attachuserpolicyrequestpolicyattachusertypedef) 

#### Policy.create\_version method

Creates a new version of the specified managed policy.

Type annotations and code completion for `#!python aiobotocore.resource("iam").create_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.create_version)

```python
# create_version method definition

await def create_version(
    self,
    *,
    PolicyDocument: str,
    SetAsDefault: bool = ...,
) -> PolicyVersion:
    ...
```



```python
# create_version method usage example with argument unpacking

kwargs: CreatePolicyVersionRequestPolicyCreateVersionTypeDef = {  # (1)
    "PolicyDocument": ...,
}

parent.create_version(**kwargs)
```

1. See [:material-code-braces: CreatePolicyVersionRequestPolicyCreateVersionTypeDef](./type_defs.md#createpolicyversionrequestpolicycreateversiontypedef) 

#### Policy.delete method

Deletes the specified managed policy.

Type annotations and code completion for `#!python aiobotocore.resource("iam").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.delete)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### Policy.detach\_group method

Removes the specified managed policy from the specified IAM group.

Type annotations and code completion for `#!python aiobotocore.resource("iam").detach_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.detach_group)

```python
# detach_group method definition

await def detach_group(
    self,
    *,
    GroupName: str,
) -> None:
    ...
```



```python
# detach_group method usage example with argument unpacking

kwargs: DetachGroupPolicyRequestPolicyDetachGroupTypeDef = {  # (1)
    "GroupName": ...,
}

parent.detach_group(**kwargs)
```

1. See [:material-code-braces: DetachGroupPolicyRequestPolicyDetachGroupTypeDef](./type_defs.md#detachgrouppolicyrequestpolicydetachgrouptypedef) 

#### Policy.detach\_role method

Removes the specified managed policy from the specified role.

Type annotations and code completion for `#!python aiobotocore.resource("iam").detach_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.detach_role)

```python
# detach_role method definition

await def detach_role(
    self,
    *,
    RoleName: str,
) -> None:
    ...
```



```python
# detach_role method usage example with argument unpacking

kwargs: DetachRolePolicyRequestPolicyDetachRoleTypeDef = {  # (1)
    "RoleName": ...,
}

parent.detach_role(**kwargs)
```

1. See [:material-code-braces: DetachRolePolicyRequestPolicyDetachRoleTypeDef](./type_defs.md#detachrolepolicyrequestpolicydetachroletypedef) 

#### Policy.detach\_user method

Removes the specified managed policy from the specified user.

Type annotations and code completion for `#!python aiobotocore.resource("iam").detach_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.detach_user)

```python
# detach_user method definition

await def detach_user(
    self,
    *,
    UserName: str,
) -> None:
    ...
```



```python
# detach_user method usage example with argument unpacking

kwargs: DetachUserPolicyRequestPolicyDetachUserTypeDef = {  # (1)
    "UserName": ...,
}

parent.detach_user(**kwargs)
```

1. See [:material-code-braces: DetachUserPolicyRequestPolicyDetachUserTypeDef](./type_defs.md#detachuserpolicyrequestpolicydetachusertypedef) 

#### Policy.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### Policy.load method

Calls :py:meth:`IAM.Client.get_policy` to update the attributes of the Policy
resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.load)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### Policy.reload method

Calls :py:meth:`IAM.Client.get_policy` to update the attributes of the Policy
resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.reload)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## PolicyVersion

Type annotations and code completion for `#!python session.resource("iam").PolicyVersion` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.PolicyVersion)

```python
# PolicyVersion usage example

from types_aiobotocore_iam.service_resource import PolicyVersion

def get_resource() -> PolicyVersion:
    return session.resource("iam").PolicyVersion(...)
```


### PolicyVersion attributes


- `document`: `Awaitable`[`str`]
- `is_default_version`: `Awaitable`[`bool`]
- `create_date`: `Awaitable`[`datetime`]
- `arn`: `str`
- `version_id`: `str`





### PolicyVersion methods


#### PolicyVersion.delete method

Deletes the specified version from the specified managed policy.

Type annotations and code completion for `#!python aiobotocore.resource("iam").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.PolicyVersion.delete)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### PolicyVersion.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.PolicyVersion.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### PolicyVersion.load method

Calls :py:meth:`IAM.Client.get_policy_version` to update the attributes of the
PolicyVersion resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.PolicyVersion.load)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### PolicyVersion.reload method

Calls :py:meth:`IAM.Client.get_policy_version` to update the attributes of the
PolicyVersion resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.PolicyVersion.reload)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```


#### PolicyVersion.set\_as\_default method

Sets the specified version of the specified policy as the policy's default
(operative) version.

Type annotations and code completion for `#!python aiobotocore.resource("iam").set_as_default` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.PolicyVersion.set_as_default)

```python
# set_as_default method definition

await def set_as_default(
    self,
) -> None:
    ...
```





## Role

Type annotations and code completion for `#!python session.resource("iam").Role` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.Role)

```python
# Role usage example

from types_aiobotocore_iam.service_resource import Role

def get_resource() -> Role:
    return session.resource("iam").Role(...)
```


### Role attributes


- `path`: `Awaitable`[`str`]
- `role_name`: `Awaitable`[`str`]
- `role_id`: `Awaitable`[`str`]
- `arn`: `Awaitable`[`str`]
- `create_date`: `Awaitable`[`datetime`]
- `assume_role_policy_document`: `Awaitable`[`str`]
- `description`: `Awaitable`[`str`]
- `max_session_duration`: `Awaitable`[`int`]
- `permissions_boundary`: `Awaitable`[[AttachedPermissionsBoundaryTypeDef](./type_defs.md#attachedpermissionsboundarytypedef)]
- `tags`: `Awaitable`[`List`[[TagTypeDef](./type_defs.md#tagtypedef)]]
- `role_last_used`: `Awaitable`[[RoleLastUsedResponseTypeDef](./type_defs.md#rolelastusedresponsetypedef)]
- `name`: `str`
- `attached_policies`: [RoleAttachedPoliciesCollection](#roleattachedpoliciescollection)
- `instance_profiles`: [RoleInstanceProfilesCollection](#roleinstanceprofilescollection)
- `policies`: [RolePoliciesCollection](#rolepoliciescollection)



### Role collections


#### Role.attached_policies

Provides access to [Policy](#policy) resource.

Type annotations and code completion for `#!python session.resource("iam").Role(...).attached_policies` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Role.attached_policies)

```python
# RoleAttachedPoliciesCollection usage example

from types_aiobotocore_iam.service_resource import RoleAttachedPoliciesCollection

def get_collection() -> RoleAttachedPoliciesCollection:
    resource = session.resource("iam").Role(...)
    return resource.attached_policies
```

#### Role.instance_profiles

Provides access to [InstanceProfile](#instanceprofile) resource.

Type annotations and code completion for `#!python session.resource("iam").Role(...).instance_profiles` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Role.instance_profiles)

```python
# RoleInstanceProfilesCollection usage example

from types_aiobotocore_iam.service_resource import RoleInstanceProfilesCollection

def get_collection() -> RoleInstanceProfilesCollection:
    resource = session.resource("iam").Role(...)
    return resource.instance_profiles
```

#### Role.policies

Provides access to [RolePolicy](#rolepolicy) resource.

Type annotations and code completion for `#!python session.resource("iam").Role(...).policies` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Role.policies)

```python
# RolePoliciesCollection usage example

from types_aiobotocore_iam.service_resource import RolePoliciesCollection

def get_collection() -> RolePoliciesCollection:
    resource = session.resource("iam").Role(...)
    return resource.policies
```




### Role methods


#### Role.AssumeRolePolicy method

Creates a AssumeRolePolicy resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").AssumeRolePolicy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Role.AssumeRolePolicy)

```python
# AssumeRolePolicy method definition

await def AssumeRolePolicy(
    self,
) -> AssumeRolePolicy:
    ...
```


#### Role.Policy method

Creates a RolePolicy resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").Policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Role.Policy)

```python
# Policy method definition

await def Policy(
    self,
    name: str,
) -> RolePolicy:
    ...
```


#### Role.attach\_policy method

Attaches the specified managed policy to the specified IAM role.

Type annotations and code completion for `#!python aiobotocore.resource("iam").attach_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Role.attach_policy)

```python
# attach_policy method definition

await def attach_policy(
    self,
    *,
    PolicyArn: str,
) -> None:
    ...
```



```python
# attach_policy method usage example with argument unpacking

kwargs: AttachRolePolicyRequestRoleAttachPolicyTypeDef = {  # (1)
    "PolicyArn": ...,
}

parent.attach_policy(**kwargs)
```

1. See [:material-code-braces: AttachRolePolicyRequestRoleAttachPolicyTypeDef](./type_defs.md#attachrolepolicyrequestroleattachpolicytypedef) 

#### Role.delete method

Deletes the specified role.

Type annotations and code completion for `#!python aiobotocore.resource("iam").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Role.delete)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### Role.detach\_policy method

Removes the specified managed policy from the specified role.

Type annotations and code completion for `#!python aiobotocore.resource("iam").detach_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Role.detach_policy)

```python
# detach_policy method definition

await def detach_policy(
    self,
    *,
    PolicyArn: str,
) -> None:
    ...
```



```python
# detach_policy method usage example with argument unpacking

kwargs: DetachRolePolicyRequestRoleDetachPolicyTypeDef = {  # (1)
    "PolicyArn": ...,
}

parent.detach_policy(**kwargs)
```

1. See [:material-code-braces: DetachRolePolicyRequestRoleDetachPolicyTypeDef](./type_defs.md#detachrolepolicyrequestroledetachpolicytypedef) 

#### Role.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Role.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### Role.load method

Calls :py:meth:`IAM.Client.get_role` to update the attributes of the Role
resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Role.load)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### Role.reload method

Calls :py:meth:`IAM.Client.get_role` to update the attributes of the Role
resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Role.reload)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## RolePolicy

Type annotations and code completion for `#!python session.resource("iam").RolePolicy` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.RolePolicy)

```python
# RolePolicy usage example

from types_aiobotocore_iam.service_resource import RolePolicy

def get_resource() -> RolePolicy:
    return session.resource("iam").RolePolicy(...)
```


### RolePolicy attributes


- `policy_name`: `Awaitable`[`str`]
- `policy_document`: `Awaitable`[`str`]
- `role_name`: `str`
- `name`: `str`





### RolePolicy methods


#### RolePolicy.Role method

Creates a Role resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").Role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.RolePolicy.Role)

```python
# Role method definition

await def Role(
    self,
) -> Role:
    ...
```


#### RolePolicy.delete method

Deletes the specified inline policy that is embedded in the specified IAM role.

Type annotations and code completion for `#!python aiobotocore.resource("iam").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.RolePolicy.delete)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### RolePolicy.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.RolePolicy.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### RolePolicy.load method

Calls :py:meth:`IAM.Client.get_role_policy` to update the attributes of the
RolePolicy resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.RolePolicy.load)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### RolePolicy.put method

Adds or updates an inline policy document that is embedded in the specified IAM
role.

Type annotations and code completion for `#!python aiobotocore.resource("iam").put` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.RolePolicy.put)

```python
# put method definition

await def put(
    self,
    *,
    PolicyDocument: str,
) -> None:
    ...
```



```python
# put method usage example with argument unpacking

kwargs: PutRolePolicyRequestRolePolicyPutTypeDef = {  # (1)
    "PolicyDocument": ...,
}

parent.put(**kwargs)
```

1. See [:material-code-braces: PutRolePolicyRequestRolePolicyPutTypeDef](./type_defs.md#putrolepolicyrequestrolepolicyputtypedef) 

#### RolePolicy.reload method

Calls :py:meth:`IAM.Client.get_role_policy` to update the attributes of the
RolePolicy resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.RolePolicy.reload)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## SamlProvider

Type annotations and code completion for `#!python session.resource("iam").SamlProvider` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.SamlProvider)

```python
# SamlProvider usage example

from types_aiobotocore_iam.service_resource import SamlProvider

def get_resource() -> SamlProvider:
    return session.resource("iam").SamlProvider(...)
```


### SamlProvider attributes


- `saml_metadata_document`: `Awaitable`[`str`]
- `create_date`: `Awaitable`[`datetime`]
- `valid_until`: `Awaitable`[`datetime`]
- `tags`: `Awaitable`[`List`[[TagTypeDef](./type_defs.md#tagtypedef)]]
- `arn`: `str`





### SamlProvider methods


#### SamlProvider.delete method

Deletes a SAML provider resource in IAM.

Type annotations and code completion for `#!python aiobotocore.resource("iam").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SamlProvider.delete)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### SamlProvider.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SamlProvider.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### SamlProvider.load method

Calls :py:meth:`IAM.Client.get_saml_provider` to update the attributes of the
SamlProvider resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SamlProvider.load)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### SamlProvider.reload method

Calls :py:meth:`IAM.Client.get_saml_provider` to update the attributes of the
SamlProvider resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SamlProvider.reload)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```


#### SamlProvider.update method

Updates the metadata document for an existing SAML provider resource object.

Type annotations and code completion for `#!python aiobotocore.resource("iam").update` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SamlProvider.update)

```python
# update method definition

await def update(
    self,
    *,
    SAMLMetadataDocument: str,
) -> UpdateSAMLProviderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateSAMLProviderResponseTypeDef](./type_defs.md#updatesamlproviderresponsetypedef) 


```python
# update method usage example with argument unpacking

kwargs: UpdateSAMLProviderRequestSamlProviderUpdateTypeDef = {  # (1)
    "SAMLMetadataDocument": ...,
}

parent.update(**kwargs)
```

1. See [:material-code-braces: UpdateSAMLProviderRequestSamlProviderUpdateTypeDef](./type_defs.md#updatesamlproviderrequestsamlproviderupdatetypedef) 




## ServerCertificate

Type annotations and code completion for `#!python session.resource("iam").ServerCertificate` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.ServerCertificate)

```python
# ServerCertificate usage example

from types_aiobotocore_iam.service_resource import ServerCertificate

def get_resource() -> ServerCertificate:
    return session.resource("iam").ServerCertificate(...)
```


### ServerCertificate attributes


- `server_certificate_metadata`: `Awaitable`[[ServerCertificateMetadataResponseTypeDef](./type_defs.md#servercertificatemetadataresponsetypedef)]
- `certificate_body`: `Awaitable`[`str`]
- `certificate_chain`: `Awaitable`[`str`]
- `tags`: `Awaitable`[`List`[[TagTypeDef](./type_defs.md#tagtypedef)]]
- `name`: `str`





### ServerCertificate methods


#### ServerCertificate.delete method

Deletes the specified server certificate.

Type annotations and code completion for `#!python aiobotocore.resource("iam").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServerCertificate.delete)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### ServerCertificate.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServerCertificate.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### ServerCertificate.load method

Calls :py:meth:`IAM.Client.get_server_certificate` to update the attributes of
the ServerCertificate resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServerCertificate.load)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### ServerCertificate.reload method

Calls :py:meth:`IAM.Client.get_server_certificate` to update the attributes of
the ServerCertificate resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServerCertificate.reload)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```


#### ServerCertificate.update method

Updates the name and/or the path of the specified server certificate stored in
IAM.

Type annotations and code completion for `#!python aiobotocore.resource("iam").update` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServerCertificate.update)

```python
# update method definition

await def update(
    self,
    *,
    NewPath: str = ...,
    NewServerCertificateName: str = ...,
) -> ServerCertificate:
    ...
```



```python
# update method usage example with argument unpacking

kwargs: UpdateServerCertificateRequestServerCertificateUpdateTypeDef = {  # (1)
    "NewPath": ...,
}

parent.update(**kwargs)
```

1. See [:material-code-braces: UpdateServerCertificateRequestServerCertificateUpdateTypeDef](./type_defs.md#updateservercertificaterequestservercertificateupdatetypedef) 




## SigningCertificate

Type annotations and code completion for `#!python session.resource("iam").SigningCertificate` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.SigningCertificate)

```python
# SigningCertificate usage example

from types_aiobotocore_iam.service_resource import SigningCertificate

def get_resource() -> SigningCertificate:
    return session.resource("iam").SigningCertificate(...)
```


### SigningCertificate attributes


- `certificate_id`: `Awaitable`[`str`]
- `certificate_body`: `Awaitable`[`str`]
- `status`: `Awaitable`[[statusTypeType](./literals.md#statustypetype)]
- `upload_date`: `Awaitable`[`datetime`]
- `user_name`: `str`
- `id`: `str`





### SigningCertificate methods


#### SigningCertificate.User method

Creates a User resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").User` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SigningCertificate.User)

```python
# User method definition

await def User(
    self,
) -> User:
    ...
```


#### SigningCertificate.activate method

Changes the status of the specified user signing certificate from active to
disabled, or vice versa.

Type annotations and code completion for `#!python aiobotocore.resource("iam").activate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SigningCertificate.activate)

```python
# activate method definition

await def activate(
    self,
    *,
    Status: statusTypeType = 'Active',  # (1)
) -> None:
    ...
```

1. See [:material-code-brackets: statusTypeType](./literals.md#statustypetype) 


```python
# activate method usage example with argument unpacking

kwargs: UpdateSigningCertificateRequestSigningCertificateActivateTypeDef = {  # (1)
    "Status": ...,
}

parent.activate(**kwargs)
```

1. See [:material-code-braces: UpdateSigningCertificateRequestSigningCertificateActivateTypeDef](./type_defs.md#updatesigningcertificaterequestsigningcertificateactivatetypedef) 

#### SigningCertificate.deactivate method

Changes the status of the specified user signing certificate from active to
disabled, or vice versa.

Type annotations and code completion for `#!python aiobotocore.resource("iam").deactivate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SigningCertificate.deactivate)

```python
# deactivate method definition

await def deactivate(
    self,
    *,
    Status: statusTypeType = 'Inactive',  # (1)
) -> None:
    ...
```

1. See [:material-code-brackets: statusTypeType](./literals.md#statustypetype) 


```python
# deactivate method usage example with argument unpacking

kwargs: UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef = {  # (1)
    "Status": ...,
}

parent.deactivate(**kwargs)
```

1. See [:material-code-braces: UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef](./type_defs.md#updatesigningcertificaterequestsigningcertificatedeactivatetypedef) 

#### SigningCertificate.delete method

Deletes a signing certificate associated with the specified IAM user.

Type annotations and code completion for `#!python aiobotocore.resource("iam").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SigningCertificate.delete)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### SigningCertificate.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SigningCertificate.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```





## User

Type annotations and code completion for `#!python session.resource("iam").User` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.User)

```python
# User usage example

from types_aiobotocore_iam.service_resource import User

def get_resource() -> User:
    return session.resource("iam").User(...)
```


### User attributes


- `path`: `Awaitable`[`str`]
- `user_name`: `Awaitable`[`str`]
- `user_id`: `Awaitable`[`str`]
- `arn`: `Awaitable`[`str`]
- `create_date`: `Awaitable`[`datetime`]
- `password_last_used`: `Awaitable`[`datetime`]
- `permissions_boundary`: `Awaitable`[[AttachedPermissionsBoundaryResponseTypeDef](./type_defs.md#attachedpermissionsboundaryresponsetypedef)]
- `tags`: `Awaitable`[`List`[[TagTypeDef](./type_defs.md#tagtypedef)]]
- `name`: `str`
- `access_keys`: [UserAccessKeysCollection](#useraccesskeyscollection)
- `attached_policies`: [UserAttachedPoliciesCollection](#userattachedpoliciescollection)
- `groups`: [UserGroupsCollection](#usergroupscollection)
- `mfa_devices`: [UserMfaDevicesCollection](#usermfadevicescollection)
- `policies`: [UserPoliciesCollection](#userpoliciescollection)
- `signing_certificates`: [UserSigningCertificatesCollection](#usersigningcertificatescollection)



### User collections


#### User.access_keys

Provides access to [AccessKey](#accesskey) resource.

Type annotations and code completion for `#!python session.resource("iam").User(...).access_keys` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.access_keys)

```python
# UserAccessKeysCollection usage example

from types_aiobotocore_iam.service_resource import UserAccessKeysCollection

def get_collection() -> UserAccessKeysCollection:
    resource = session.resource("iam").User(...)
    return resource.access_keys
```

#### User.attached_policies

Provides access to [Policy](#policy) resource.

Type annotations and code completion for `#!python session.resource("iam").User(...).attached_policies` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.attached_policies)

```python
# UserAttachedPoliciesCollection usage example

from types_aiobotocore_iam.service_resource import UserAttachedPoliciesCollection

def get_collection() -> UserAttachedPoliciesCollection:
    resource = session.resource("iam").User(...)
    return resource.attached_policies
```

#### User.groups

Provides access to [Group](#group) resource.

Type annotations and code completion for `#!python session.resource("iam").User(...).groups` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.groups)

```python
# UserGroupsCollection usage example

from types_aiobotocore_iam.service_resource import UserGroupsCollection

def get_collection() -> UserGroupsCollection:
    resource = session.resource("iam").User(...)
    return resource.groups
```

#### User.mfa_devices

Provides access to [MfaDevice](#mfadevice) resource.

Type annotations and code completion for `#!python session.resource("iam").User(...).mfa_devices` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.mfa_devices)

```python
# UserMfaDevicesCollection usage example

from types_aiobotocore_iam.service_resource import UserMfaDevicesCollection

def get_collection() -> UserMfaDevicesCollection:
    resource = session.resource("iam").User(...)
    return resource.mfa_devices
```

#### User.policies

Provides access to [UserPolicy](#userpolicy) resource.

Type annotations and code completion for `#!python session.resource("iam").User(...).policies` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.policies)

```python
# UserPoliciesCollection usage example

from types_aiobotocore_iam.service_resource import UserPoliciesCollection

def get_collection() -> UserPoliciesCollection:
    resource = session.resource("iam").User(...)
    return resource.policies
```

#### User.signing_certificates

Provides access to [SigningCertificate](#signingcertificate) resource.

Type annotations and code completion for `#!python session.resource("iam").User(...).signing_certificates` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.signing_certificates)

```python
# UserSigningCertificatesCollection usage example

from types_aiobotocore_iam.service_resource import UserSigningCertificatesCollection

def get_collection() -> UserSigningCertificatesCollection:
    resource = session.resource("iam").User(...)
    return resource.signing_certificates
```




### User methods


#### User.AccessKey method

Creates a AccessKey resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").AccessKey` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.AccessKey)

```python
# AccessKey method definition

await def AccessKey(
    self,
    id: str,
) -> AccessKey:
    ...
```


#### User.LoginProfile method

Creates a LoginProfile resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").LoginProfile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.LoginProfile)

```python
# LoginProfile method definition

await def LoginProfile(
    self,
) -> LoginProfile:
    ...
```


#### User.MfaDevice method

Creates a MfaDevice resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").MfaDevice` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.MfaDevice)

```python
# MfaDevice method definition

await def MfaDevice(
    self,
    serial_number: str,
) -> MfaDevice:
    ...
```


#### User.Policy method

Creates a UserPolicy resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").Policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.Policy)

```python
# Policy method definition

await def Policy(
    self,
    name: str,
) -> UserPolicy:
    ...
```


#### User.SigningCertificate method

Creates a SigningCertificate resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").SigningCertificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.SigningCertificate)

```python
# SigningCertificate method definition

await def SigningCertificate(
    self,
    id: str,
) -> SigningCertificate:
    ...
```


#### User.add\_group method

Adds the specified user to the specified group.

Type annotations and code completion for `#!python aiobotocore.resource("iam").add_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.add_group)

```python
# add_group method definition

await def add_group(
    self,
    *,
    GroupName: str,
) -> None:
    ...
```



```python
# add_group method usage example with argument unpacking

kwargs: AddUserToGroupRequestUserAddGroupTypeDef = {  # (1)
    "GroupName": ...,
}

parent.add_group(**kwargs)
```

1. See [:material-code-braces: AddUserToGroupRequestUserAddGroupTypeDef](./type_defs.md#addusertogrouprequestuseraddgrouptypedef) 

#### User.attach\_policy method

Attaches the specified managed policy to the specified user.

Type annotations and code completion for `#!python aiobotocore.resource("iam").attach_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.attach_policy)

```python
# attach_policy method definition

await def attach_policy(
    self,
    *,
    PolicyArn: str,
) -> None:
    ...
```



```python
# attach_policy method usage example with argument unpacking

kwargs: AttachUserPolicyRequestUserAttachPolicyTypeDef = {  # (1)
    "PolicyArn": ...,
}

parent.attach_policy(**kwargs)
```

1. See [:material-code-braces: AttachUserPolicyRequestUserAttachPolicyTypeDef](./type_defs.md#attachuserpolicyrequestuserattachpolicytypedef) 

#### User.create method

Creates a new IAM user for your Amazon Web Services account.

Type annotations and code completion for `#!python aiobotocore.resource("iam").create` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.create)

```python
# create method definition

await def create(
    self,
    *,
    Path: str = ...,
    PermissionsBoundary: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> User:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# create method usage example with argument unpacking

kwargs: CreateUserRequestUserCreateTypeDef = {  # (1)
    "Path": ...,
}

parent.create(**kwargs)
```

1. See [:material-code-braces: CreateUserRequestUserCreateTypeDef](./type_defs.md#createuserrequestusercreatetypedef) 

#### User.create\_access\_key\_pair method

Creates a new Amazon Web Services secret access key and corresponding Amazon Web
Services access key ID for the specified user.

Type annotations and code completion for `#!python aiobotocore.resource("iam").create_access_key_pair` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.create_access_key_pair)

```python
# create_access_key_pair method definition

await def create_access_key_pair(
    self,
) -> AccessKeyPair:
    ...
```


#### User.create\_login\_profile method

Creates a password for the specified IAM user.

Type annotations and code completion for `#!python aiobotocore.resource("iam").create_login_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.create_login_profile)

```python
# create_login_profile method definition

await def create_login_profile(
    self,
    *,
    Password: str,
    PasswordResetRequired: bool = ...,
) -> LoginProfile:
    ...
```



```python
# create_login_profile method usage example with argument unpacking

kwargs: CreateLoginProfileRequestUserCreateLoginProfileTypeDef = {  # (1)
    "Password": ...,
}

parent.create_login_profile(**kwargs)
```

1. See [:material-code-braces: CreateLoginProfileRequestUserCreateLoginProfileTypeDef](./type_defs.md#createloginprofilerequestusercreateloginprofiletypedef) 

#### User.create\_policy method

Adds or updates an inline policy document that is embedded in the specified IAM
user.

Type annotations and code completion for `#!python aiobotocore.resource("iam").create_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.create_policy)

```python
# create_policy method definition

await def create_policy(
    self,
    *,
    PolicyName: str,
    PolicyDocument: str,
) -> UserPolicy:
    ...
```



```python
# create_policy method usage example with argument unpacking

kwargs: PutUserPolicyRequestUserCreatePolicyTypeDef = {  # (1)
    "PolicyName": ...,
    "PolicyDocument": ...,
}

parent.create_policy(**kwargs)
```

1. See [:material-code-braces: PutUserPolicyRequestUserCreatePolicyTypeDef](./type_defs.md#putuserpolicyrequestusercreatepolicytypedef) 

#### User.delete method

Deletes the specified IAM user.

Type annotations and code completion for `#!python aiobotocore.resource("iam").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.delete)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### User.detach\_policy method

Removes the specified managed policy from the specified user.

Type annotations and code completion for `#!python aiobotocore.resource("iam").detach_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.detach_policy)

```python
# detach_policy method definition

await def detach_policy(
    self,
    *,
    PolicyArn: str,
) -> None:
    ...
```



```python
# detach_policy method usage example with argument unpacking

kwargs: DetachUserPolicyRequestUserDetachPolicyTypeDef = {  # (1)
    "PolicyArn": ...,
}

parent.detach_policy(**kwargs)
```

1. See [:material-code-braces: DetachUserPolicyRequestUserDetachPolicyTypeDef](./type_defs.md#detachuserpolicyrequestuserdetachpolicytypedef) 

#### User.enable\_mfa method

Enables the specified MFA device and associates it with the specified IAM user.

Type annotations and code completion for `#!python aiobotocore.resource("iam").enable_mfa` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.enable_mfa)

```python
# enable_mfa method definition

await def enable_mfa(
    self,
    *,
    SerialNumber: str,
    AuthenticationCode1: str,
    AuthenticationCode2: str,
) -> MfaDevice:
    ...
```



```python
# enable_mfa method usage example with argument unpacking

kwargs: EnableMFADeviceRequestUserEnableMfaTypeDef = {  # (1)
    "SerialNumber": ...,
    "AuthenticationCode1": ...,
    "AuthenticationCode2": ...,
}

parent.enable_mfa(**kwargs)
```

1. See [:material-code-braces: EnableMFADeviceRequestUserEnableMfaTypeDef](./type_defs.md#enablemfadevicerequestuserenablemfatypedef) 

#### User.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### User.load method

Calls :py:meth:`IAM.Client.get_user` to update the attributes of the User
resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.load)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### User.reload method

Calls :py:meth:`IAM.Client.get_user` to update the attributes of the User
resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.reload)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```


#### User.remove\_group method

Removes the specified user from the specified group.

Type annotations and code completion for `#!python aiobotocore.resource("iam").remove_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.remove_group)

```python
# remove_group method definition

await def remove_group(
    self,
    *,
    GroupName: str,
) -> None:
    ...
```



```python
# remove_group method usage example with argument unpacking

kwargs: RemoveUserFromGroupRequestUserRemoveGroupTypeDef = {  # (1)
    "GroupName": ...,
}

parent.remove_group(**kwargs)
```

1. See [:material-code-braces: RemoveUserFromGroupRequestUserRemoveGroupTypeDef](./type_defs.md#removeuserfromgrouprequestuserremovegrouptypedef) 

#### User.update method

Updates the name and/or the path of the specified IAM user.

Type annotations and code completion for `#!python aiobotocore.resource("iam").update` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.update)

```python
# update method definition

await def update(
    self,
    *,
    NewPath: str = ...,
    NewUserName: str = ...,
) -> User:
    ...
```



```python
# update method usage example with argument unpacking

kwargs: UpdateUserRequestUserUpdateTypeDef = {  # (1)
    "NewPath": ...,
}

parent.update(**kwargs)
```

1. See [:material-code-braces: UpdateUserRequestUserUpdateTypeDef](./type_defs.md#updateuserrequestuserupdatetypedef) 




## UserPolicy

Type annotations and code completion for `#!python session.resource("iam").UserPolicy` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.UserPolicy)

```python
# UserPolicy usage example

from types_aiobotocore_iam.service_resource import UserPolicy

def get_resource() -> UserPolicy:
    return session.resource("iam").UserPolicy(...)
```


### UserPolicy attributes


- `policy_name`: `Awaitable`[`str`]
- `policy_document`: `Awaitable`[`str`]
- `user_name`: `str`
- `name`: `str`





### UserPolicy methods


#### UserPolicy.User method

Creates a User resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").User` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.UserPolicy.User)

```python
# User method definition

await def User(
    self,
) -> User:
    ...
```


#### UserPolicy.delete method

Deletes the specified inline policy that is embedded in the specified IAM user.

Type annotations and code completion for `#!python aiobotocore.resource("iam").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.UserPolicy.delete)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### UserPolicy.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.UserPolicy.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### UserPolicy.load method

Calls :py:meth:`IAM.Client.get_user_policy` to update the attributes of the
UserPolicy resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.UserPolicy.load)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### UserPolicy.put method

Adds or updates an inline policy document that is embedded in the specified IAM
user.

Type annotations and code completion for `#!python aiobotocore.resource("iam").put` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.UserPolicy.put)

```python
# put method definition

await def put(
    self,
    *,
    PolicyDocument: str,
) -> None:
    ...
```



```python
# put method usage example with argument unpacking

kwargs: PutUserPolicyRequestUserPolicyPutTypeDef = {  # (1)
    "PolicyDocument": ...,
}

parent.put(**kwargs)
```

1. See [:material-code-braces: PutUserPolicyRequestUserPolicyPutTypeDef](./type_defs.md#putuserpolicyrequestuserpolicyputtypedef) 

#### UserPolicy.reload method

Calls :py:meth:`IAM.Client.get_user_policy` to update the attributes of the
UserPolicy resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.UserPolicy.reload)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## VirtualMfaDevice

Type annotations and code completion for `#!python session.resource("iam").VirtualMfaDevice` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.VirtualMfaDevice)

```python
# VirtualMfaDevice usage example

from types_aiobotocore_iam.service_resource import VirtualMfaDevice

def get_resource() -> VirtualMfaDevice:
    return session.resource("iam").VirtualMfaDevice(...)
```


### VirtualMfaDevice attributes


- `base32_string_seed`: `Awaitable`[`bytes`]
- `qr_code_png`: `Awaitable`[`bytes`]
- `user_attribute`: `Awaitable`[[UserResponseTypeDef](./type_defs.md#userresponsetypedef)]
- `enable_date`: `Awaitable`[`datetime`]
- `tags`: `Awaitable`[`List`[[TagTypeDef](./type_defs.md#tagtypedef)]]
- `serial_number`: `str`
- `user`: [User](#user)





### VirtualMfaDevice methods


#### VirtualMfaDevice.delete method

Deletes a virtual MFA device.

Type annotations and code completion for `#!python aiobotocore.resource("iam").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.VirtualMfaDevice.delete)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### VirtualMfaDevice.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("iam").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.VirtualMfaDevice.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```




