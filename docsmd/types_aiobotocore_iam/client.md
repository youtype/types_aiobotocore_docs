# IAMClient

> [Index](../README.md) > [IAM](./README.md) > IAMClient

!!! note ""

    Auto-generated documentation for [IAM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#iam)
    type annotations stubs module [types-aiobotocore-iam](https://pypi.org/project/types-aiobotocore-iam/).

## IAMClient

Type annotations and code completion for `#!python session.create_client("iam")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client)

```python
# IAMClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_iam.client import IAMClient

session = get_session()
async with session.create_client("iam") as client:
    client: IAMClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("iam").exceptions` structure.

```python
# IAMClient.exceptions usage example

async with session.create_client("iam") as client:
    try:
        do_something(client)
    except (
            client.AccountNotManagementOrDelegatedAdministratorException,
        client.CallerIsNotManagementAccountException,
        client.ClientError,
        client.ConcurrentModificationException,
        client.CredentialReportExpiredException,
        client.CredentialReportNotPresentException,
        client.CredentialReportNotReadyException,
        client.DeleteConflictException,
        client.DuplicateCertificateException,
        client.DuplicateSSHPublicKeyException,
        client.EntityAlreadyExistsException,
        client.EntityTemporarilyUnmodifiableException,
        client.InvalidAuthenticationCodeException,
        client.InvalidCertificateException,
        client.InvalidInputException,
        client.InvalidPublicKeyException,
        client.InvalidUserTypeException,
        client.KeyPairMismatchException,
        client.LimitExceededException,
        client.MalformedCertificateException,
        client.MalformedPolicyDocumentException,
        client.NoSuchEntityException,
        client.OpenIdIdpCommunicationErrorException,
        client.OrganizationNotFoundException,
        client.OrganizationNotInAllFeaturesModeException,
        client.PasswordPolicyViolationException,
        client.PolicyEvaluationException,
        client.PolicyNotAttachableException,
        client.ReportGenerationLimitExceededException,
        client.ServiceAccessNotEnabledException,
        client.ServiceFailureException,
        client.ServiceNotSupportedException,
        client.UnmodifiableEntityException,
        client.UnrecognizedPublicKeyEncodingException,
    ) as e:
        print(e)
```

```python
# IAMClient usage type checking example

from types_aiobotocore_iam.client import Exceptions

def handle_error(exc: Exceptions.AccountNotManagementOrDelegatedAdministratorException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("iam").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("iam").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### close



Type annotations and code completion for `#!python session.create_client("iam").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### add\_client\_id\_to\_open\_id\_connect\_provider

Adds a new client ID (also known as audience) to the list of client IDs already
registered for the specified IAM OpenID Connect (OIDC) provider resource.

Type annotations and code completion for `#!python session.create_client("iam").add_client_id_to_open_id_connect_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/add_client_id_to_open_id_connect_provider.html)

```python
# add_client_id_to_open_id_connect_provider method definition

await def add_client_id_to_open_id_connect_provider(
    self,
    *,
    OpenIDConnectProviderArn: str,
    ClientID: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# add_client_id_to_open_id_connect_provider method usage example with argument unpacking

kwargs: AddClientIDToOpenIDConnectProviderRequestRequestTypeDef = {  # (1)
    "OpenIDConnectProviderArn": ...,
    "ClientID": ...,
}

parent.add_client_id_to_open_id_connect_provider(**kwargs)
```

1. See [:material-code-braces: AddClientIDToOpenIDConnectProviderRequestRequestTypeDef](./type_defs.md#addclientidtoopenidconnectproviderrequestrequesttypedef) 

### add\_role\_to\_instance\_profile

Adds the specified IAM role to the specified instance profile.

Type annotations and code completion for `#!python session.create_client("iam").add_role_to_instance_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/add_role_to_instance_profile.html)

```python
# add_role_to_instance_profile method definition

await def add_role_to_instance_profile(
    self,
    *,
    InstanceProfileName: str,
    RoleName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# add_role_to_instance_profile method usage example with argument unpacking

kwargs: AddRoleToInstanceProfileRequestRequestTypeDef = {  # (1)
    "InstanceProfileName": ...,
    "RoleName": ...,
}

parent.add_role_to_instance_profile(**kwargs)
```

1. See [:material-code-braces: AddRoleToInstanceProfileRequestRequestTypeDef](./type_defs.md#addroletoinstanceprofilerequestrequesttypedef) 

### add\_user\_to\_group

Adds the specified user to the specified group.

Type annotations and code completion for `#!python session.create_client("iam").add_user_to_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/add_user_to_group.html)

```python
# add_user_to_group method definition

await def add_user_to_group(
    self,
    *,
    GroupName: str,
    UserName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# add_user_to_group method usage example with argument unpacking

kwargs: AddUserToGroupRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
    "UserName": ...,
}

parent.add_user_to_group(**kwargs)
```

1. See [:material-code-braces: AddUserToGroupRequestRequestTypeDef](./type_defs.md#addusertogrouprequestrequesttypedef) 

### attach\_group\_policy

Attaches the specified managed policy to the specified IAM group.

Type annotations and code completion for `#!python session.create_client("iam").attach_group_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/attach_group_policy.html)

```python
# attach_group_policy method definition

await def attach_group_policy(
    self,
    *,
    GroupName: str,
    PolicyArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# attach_group_policy method usage example with argument unpacking

kwargs: AttachGroupPolicyRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
    "PolicyArn": ...,
}

parent.attach_group_policy(**kwargs)
```

1. See [:material-code-braces: AttachGroupPolicyRequestRequestTypeDef](./type_defs.md#attachgrouppolicyrequestrequesttypedef) 

### attach\_role\_policy

Attaches the specified managed policy to the specified IAM role.

Type annotations and code completion for `#!python session.create_client("iam").attach_role_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/attach_role_policy.html)

```python
# attach_role_policy method definition

await def attach_role_policy(
    self,
    *,
    RoleName: str,
    PolicyArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# attach_role_policy method usage example with argument unpacking

kwargs: AttachRolePolicyRequestRequestTypeDef = {  # (1)
    "RoleName": ...,
    "PolicyArn": ...,
}

parent.attach_role_policy(**kwargs)
```

1. See [:material-code-braces: AttachRolePolicyRequestRequestTypeDef](./type_defs.md#attachrolepolicyrequestrequesttypedef) 

### attach\_user\_policy

Attaches the specified managed policy to the specified user.

Type annotations and code completion for `#!python session.create_client("iam").attach_user_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/attach_user_policy.html)

```python
# attach_user_policy method definition

await def attach_user_policy(
    self,
    *,
    UserName: str,
    PolicyArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# attach_user_policy method usage example with argument unpacking

kwargs: AttachUserPolicyRequestRequestTypeDef = {  # (1)
    "UserName": ...,
    "PolicyArn": ...,
}

parent.attach_user_policy(**kwargs)
```

1. See [:material-code-braces: AttachUserPolicyRequestRequestTypeDef](./type_defs.md#attachuserpolicyrequestrequesttypedef) 

### change\_password

Changes the password of the IAM user who is calling this operation.

Type annotations and code completion for `#!python session.create_client("iam").change_password` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/change_password.html)

```python
# change_password method definition

await def change_password(
    self,
    *,
    OldPassword: str,
    NewPassword: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# change_password method usage example with argument unpacking

kwargs: ChangePasswordRequestRequestTypeDef = {  # (1)
    "OldPassword": ...,
    "NewPassword": ...,
}

parent.change_password(**kwargs)
```

1. See [:material-code-braces: ChangePasswordRequestRequestTypeDef](./type_defs.md#changepasswordrequestrequesttypedef) 

### create\_access\_key

Creates a new Amazon Web Services secret access key and corresponding Amazon
Web Services access key ID for the specified user.

Type annotations and code completion for `#!python session.create_client("iam").create_access_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/create_access_key.html)

```python
# create_access_key method definition

await def create_access_key(
    self,
    *,
    UserName: str = ...,
) -> CreateAccessKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateAccessKeyResponseTypeDef](./type_defs.md#createaccesskeyresponsetypedef) 


```python
# create_access_key method usage example with argument unpacking

kwargs: CreateAccessKeyRequestRequestTypeDef = {  # (1)
    "UserName": ...,
}

parent.create_access_key(**kwargs)
```

1. See [:material-code-braces: CreateAccessKeyRequestRequestTypeDef](./type_defs.md#createaccesskeyrequestrequesttypedef) 

### create\_account\_alias

Creates an alias for your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("iam").create_account_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/create_account_alias.html)

```python
# create_account_alias method definition

await def create_account_alias(
    self,
    *,
    AccountAlias: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# create_account_alias method usage example with argument unpacking

kwargs: CreateAccountAliasRequestRequestTypeDef = {  # (1)
    "AccountAlias": ...,
}

parent.create_account_alias(**kwargs)
```

1. See [:material-code-braces: CreateAccountAliasRequestRequestTypeDef](./type_defs.md#createaccountaliasrequestrequesttypedef) 

### create\_group

Creates a new group.

Type annotations and code completion for `#!python session.create_client("iam").create_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/create_group.html)

```python
# create_group method definition

await def create_group(
    self,
    *,
    GroupName: str,
    Path: str = ...,
) -> CreateGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateGroupResponseTypeDef](./type_defs.md#creategroupresponsetypedef) 


```python
# create_group method usage example with argument unpacking

kwargs: CreateGroupRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
}

parent.create_group(**kwargs)
```

1. See [:material-code-braces: CreateGroupRequestRequestTypeDef](./type_defs.md#creategrouprequestrequesttypedef) 

### create\_instance\_profile

Creates a new instance profile.

Type annotations and code completion for `#!python session.create_client("iam").create_instance_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/create_instance_profile.html)

```python
# create_instance_profile method definition

await def create_instance_profile(
    self,
    *,
    InstanceProfileName: str,
    Path: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateInstanceProfileResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateInstanceProfileResponseTypeDef](./type_defs.md#createinstanceprofileresponsetypedef) 


```python
# create_instance_profile method usage example with argument unpacking

kwargs: CreateInstanceProfileRequestRequestTypeDef = {  # (1)
    "InstanceProfileName": ...,
}

parent.create_instance_profile(**kwargs)
```

1. See [:material-code-braces: CreateInstanceProfileRequestRequestTypeDef](./type_defs.md#createinstanceprofilerequestrequesttypedef) 

### create\_login\_profile

Creates a password for the specified IAM user.

Type annotations and code completion for `#!python session.create_client("iam").create_login_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/create_login_profile.html)

```python
# create_login_profile method definition

await def create_login_profile(
    self,
    *,
    UserName: str = ...,
    Password: str = ...,
    PasswordResetRequired: bool = ...,
) -> CreateLoginProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateLoginProfileResponseTypeDef](./type_defs.md#createloginprofileresponsetypedef) 


```python
# create_login_profile method usage example with argument unpacking

kwargs: CreateLoginProfileRequestRequestTypeDef = {  # (1)
    "UserName": ...,
}

parent.create_login_profile(**kwargs)
```

1. See [:material-code-braces: CreateLoginProfileRequestRequestTypeDef](./type_defs.md#createloginprofilerequestrequesttypedef) 

### create\_open\_id\_connect\_provider

Creates an IAM entity to describe an identity provider (IdP) that supports <a
href="http://openid.net/connect/">OpenID Connect (OIDC)</a>.

Type annotations and code completion for `#!python session.create_client("iam").create_open_id_connect_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/create_open_id_connect_provider.html)

```python
# create_open_id_connect_provider method definition

await def create_open_id_connect_provider(
    self,
    *,
    Url: str,
    ClientIDList: Sequence[str] = ...,
    ThumbprintList: Sequence[str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateOpenIDConnectProviderResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateOpenIDConnectProviderResponseTypeDef](./type_defs.md#createopenidconnectproviderresponsetypedef) 


```python
# create_open_id_connect_provider method usage example with argument unpacking

kwargs: CreateOpenIDConnectProviderRequestRequestTypeDef = {  # (1)
    "Url": ...,
}

parent.create_open_id_connect_provider(**kwargs)
```

1. See [:material-code-braces: CreateOpenIDConnectProviderRequestRequestTypeDef](./type_defs.md#createopenidconnectproviderrequestrequesttypedef) 

### create\_policy

Creates a new managed policy for your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("iam").create_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/create_policy.html)

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
) -> CreatePolicyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreatePolicyResponseTypeDef](./type_defs.md#createpolicyresponsetypedef) 


```python
# create_policy method usage example with argument unpacking

kwargs: CreatePolicyRequestRequestTypeDef = {  # (1)
    "PolicyName": ...,
    "PolicyDocument": ...,
}

parent.create_policy(**kwargs)
```

1. See [:material-code-braces: CreatePolicyRequestRequestTypeDef](./type_defs.md#createpolicyrequestrequesttypedef) 

### create\_policy\_version

Creates a new version of the specified managed policy.

Type annotations and code completion for `#!python session.create_client("iam").create_policy_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/create_policy_version.html)

```python
# create_policy_version method definition

await def create_policy_version(
    self,
    *,
    PolicyArn: str,
    PolicyDocument: str,
    SetAsDefault: bool = ...,
) -> CreatePolicyVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreatePolicyVersionResponseTypeDef](./type_defs.md#createpolicyversionresponsetypedef) 


```python
# create_policy_version method usage example with argument unpacking

kwargs: CreatePolicyVersionRequestRequestTypeDef = {  # (1)
    "PolicyArn": ...,
    "PolicyDocument": ...,
}

parent.create_policy_version(**kwargs)
```

1. See [:material-code-braces: CreatePolicyVersionRequestRequestTypeDef](./type_defs.md#createpolicyversionrequestrequesttypedef) 

### create\_role

Creates a new role for your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("iam").create_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/create_role.html)

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
) -> CreateRoleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateRoleResponseTypeDef](./type_defs.md#createroleresponsetypedef) 


```python
# create_role method usage example with argument unpacking

kwargs: CreateRoleRequestRequestTypeDef = {  # (1)
    "RoleName": ...,
    "AssumeRolePolicyDocument": ...,
}

parent.create_role(**kwargs)
```

1. See [:material-code-braces: CreateRoleRequestRequestTypeDef](./type_defs.md#createrolerequestrequesttypedef) 

### create\_saml\_provider

Creates an IAM resource that describes an identity provider (IdP) that supports
SAML 2.0.

Type annotations and code completion for `#!python session.create_client("iam").create_saml_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/create_saml_provider.html)

```python
# create_saml_provider method definition

await def create_saml_provider(
    self,
    *,
    SAMLMetadataDocument: str,
    Name: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateSAMLProviderResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateSAMLProviderResponseTypeDef](./type_defs.md#createsamlproviderresponsetypedef) 


```python
# create_saml_provider method usage example with argument unpacking

kwargs: CreateSAMLProviderRequestRequestTypeDef = {  # (1)
    "SAMLMetadataDocument": ...,
    "Name": ...,
}

parent.create_saml_provider(**kwargs)
```

1. See [:material-code-braces: CreateSAMLProviderRequestRequestTypeDef](./type_defs.md#createsamlproviderrequestrequesttypedef) 

### create\_service\_linked\_role

Creates an IAM role that is linked to a specific Amazon Web Services service.

Type annotations and code completion for `#!python session.create_client("iam").create_service_linked_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/create_service_linked_role.html)

```python
# create_service_linked_role method definition

await def create_service_linked_role(
    self,
    *,
    AWSServiceName: str,
    Description: str = ...,
    CustomSuffix: str = ...,
) -> CreateServiceLinkedRoleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateServiceLinkedRoleResponseTypeDef](./type_defs.md#createservicelinkedroleresponsetypedef) 


```python
# create_service_linked_role method usage example with argument unpacking

kwargs: CreateServiceLinkedRoleRequestRequestTypeDef = {  # (1)
    "AWSServiceName": ...,
}

parent.create_service_linked_role(**kwargs)
```

1. See [:material-code-braces: CreateServiceLinkedRoleRequestRequestTypeDef](./type_defs.md#createservicelinkedrolerequestrequesttypedef) 

### create\_service\_specific\_credential

Generates a set of credentials consisting of a user name and password that can
be used to access the service specified in the request.

Type annotations and code completion for `#!python session.create_client("iam").create_service_specific_credential` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/create_service_specific_credential.html)

```python
# create_service_specific_credential method definition

await def create_service_specific_credential(
    self,
    *,
    UserName: str,
    ServiceName: str,
) -> CreateServiceSpecificCredentialResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateServiceSpecificCredentialResponseTypeDef](./type_defs.md#createservicespecificcredentialresponsetypedef) 


```python
# create_service_specific_credential method usage example with argument unpacking

kwargs: CreateServiceSpecificCredentialRequestRequestTypeDef = {  # (1)
    "UserName": ...,
    "ServiceName": ...,
}

parent.create_service_specific_credential(**kwargs)
```

1. See [:material-code-braces: CreateServiceSpecificCredentialRequestRequestTypeDef](./type_defs.md#createservicespecificcredentialrequestrequesttypedef) 

### create\_user

Creates a new IAM user for your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("iam").create_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/create_user.html)

```python
# create_user method definition

await def create_user(
    self,
    *,
    UserName: str,
    Path: str = ...,
    PermissionsBoundary: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateUserResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateUserResponseTypeDef](./type_defs.md#createuserresponsetypedef) 


```python
# create_user method usage example with argument unpacking

kwargs: CreateUserRequestRequestTypeDef = {  # (1)
    "UserName": ...,
}

parent.create_user(**kwargs)
```

1. See [:material-code-braces: CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef) 

### create\_virtual\_mfa\_device

Creates a new virtual MFA device for the Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("iam").create_virtual_mfa_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/create_virtual_mfa_device.html)

```python
# create_virtual_mfa_device method definition

await def create_virtual_mfa_device(
    self,
    *,
    VirtualMFADeviceName: str,
    Path: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateVirtualMFADeviceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateVirtualMFADeviceResponseTypeDef](./type_defs.md#createvirtualmfadeviceresponsetypedef) 


```python
# create_virtual_mfa_device method usage example with argument unpacking

kwargs: CreateVirtualMFADeviceRequestRequestTypeDef = {  # (1)
    "VirtualMFADeviceName": ...,
}

parent.create_virtual_mfa_device(**kwargs)
```

1. See [:material-code-braces: CreateVirtualMFADeviceRequestRequestTypeDef](./type_defs.md#createvirtualmfadevicerequestrequesttypedef) 

### deactivate\_mfa\_device

Deactivates the specified MFA device and removes it from association with the
user name for which it was originally enabled.

Type annotations and code completion for `#!python session.create_client("iam").deactivate_mfa_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/deactivate_mfa_device.html)

```python
# deactivate_mfa_device method definition

await def deactivate_mfa_device(
    self,
    *,
    SerialNumber: str,
    UserName: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# deactivate_mfa_device method usage example with argument unpacking

kwargs: DeactivateMFADeviceRequestRequestTypeDef = {  # (1)
    "SerialNumber": ...,
}

parent.deactivate_mfa_device(**kwargs)
```

1. See [:material-code-braces: DeactivateMFADeviceRequestRequestTypeDef](./type_defs.md#deactivatemfadevicerequestrequesttypedef) 

### delete\_access\_key

Deletes the access key pair associated with the specified IAM user.

Type annotations and code completion for `#!python session.create_client("iam").delete_access_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_access_key.html)

```python
# delete_access_key method definition

await def delete_access_key(
    self,
    *,
    AccessKeyId: str,
    UserName: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_access_key method usage example with argument unpacking

kwargs: DeleteAccessKeyRequestRequestTypeDef = {  # (1)
    "AccessKeyId": ...,
}

parent.delete_access_key(**kwargs)
```

1. See [:material-code-braces: DeleteAccessKeyRequestRequestTypeDef](./type_defs.md#deleteaccesskeyrequestrequesttypedef) 

### delete\_account\_alias

Deletes the specified Amazon Web Services account alias.

Type annotations and code completion for `#!python session.create_client("iam").delete_account_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_account_alias.html)

```python
# delete_account_alias method definition

await def delete_account_alias(
    self,
    *,
    AccountAlias: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_account_alias method usage example with argument unpacking

kwargs: DeleteAccountAliasRequestRequestTypeDef = {  # (1)
    "AccountAlias": ...,
}

parent.delete_account_alias(**kwargs)
```

1. See [:material-code-braces: DeleteAccountAliasRequestRequestTypeDef](./type_defs.md#deleteaccountaliasrequestrequesttypedef) 

### delete\_account\_password\_policy

Deletes the password policy for the Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("iam").delete_account_password_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_account_password_policy.html)

```python
# delete_account_password_policy method definition

await def delete_account_password_policy(
    self,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 

### delete\_group

Deletes the specified IAM group.

Type annotations and code completion for `#!python session.create_client("iam").delete_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_group.html)

```python
# delete_group method definition

await def delete_group(
    self,
    *,
    GroupName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_group method usage example with argument unpacking

kwargs: DeleteGroupRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
}

parent.delete_group(**kwargs)
```

1. See [:material-code-braces: DeleteGroupRequestRequestTypeDef](./type_defs.md#deletegrouprequestrequesttypedef) 

### delete\_group\_policy

Deletes the specified inline policy that is embedded in the specified IAM group.

Type annotations and code completion for `#!python session.create_client("iam").delete_group_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_group_policy.html)

```python
# delete_group_policy method definition

await def delete_group_policy(
    self,
    *,
    GroupName: str,
    PolicyName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_group_policy method usage example with argument unpacking

kwargs: DeleteGroupPolicyRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
    "PolicyName": ...,
}

parent.delete_group_policy(**kwargs)
```

1. See [:material-code-braces: DeleteGroupPolicyRequestRequestTypeDef](./type_defs.md#deletegrouppolicyrequestrequesttypedef) 

### delete\_instance\_profile

Deletes the specified instance profile.

Type annotations and code completion for `#!python session.create_client("iam").delete_instance_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_instance_profile.html)

```python
# delete_instance_profile method definition

await def delete_instance_profile(
    self,
    *,
    InstanceProfileName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_instance_profile method usage example with argument unpacking

kwargs: DeleteInstanceProfileRequestRequestTypeDef = {  # (1)
    "InstanceProfileName": ...,
}

parent.delete_instance_profile(**kwargs)
```

1. See [:material-code-braces: DeleteInstanceProfileRequestRequestTypeDef](./type_defs.md#deleteinstanceprofilerequestrequesttypedef) 

### delete\_login\_profile

Deletes the password for the specified IAM user, For more information, see <a
href="https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_passwords_admin-change-user.html">Managing
passwords for IAM users</a>.

Type annotations and code completion for `#!python session.create_client("iam").delete_login_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_login_profile.html)

```python
# delete_login_profile method definition

await def delete_login_profile(
    self,
    *,
    UserName: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_login_profile method usage example with argument unpacking

kwargs: DeleteLoginProfileRequestRequestTypeDef = {  # (1)
    "UserName": ...,
}

parent.delete_login_profile(**kwargs)
```

1. See [:material-code-braces: DeleteLoginProfileRequestRequestTypeDef](./type_defs.md#deleteloginprofilerequestrequesttypedef) 

### delete\_open\_id\_connect\_provider

Deletes an OpenID Connect identity provider (IdP) resource object in IAM.

Type annotations and code completion for `#!python session.create_client("iam").delete_open_id_connect_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_open_id_connect_provider.html)

```python
# delete_open_id_connect_provider method definition

await def delete_open_id_connect_provider(
    self,
    *,
    OpenIDConnectProviderArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_open_id_connect_provider method usage example with argument unpacking

kwargs: DeleteOpenIDConnectProviderRequestRequestTypeDef = {  # (1)
    "OpenIDConnectProviderArn": ...,
}

parent.delete_open_id_connect_provider(**kwargs)
```

1. See [:material-code-braces: DeleteOpenIDConnectProviderRequestRequestTypeDef](./type_defs.md#deleteopenidconnectproviderrequestrequesttypedef) 

### delete\_policy

Deletes the specified managed policy.

Type annotations and code completion for `#!python session.create_client("iam").delete_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_policy.html)

```python
# delete_policy method definition

await def delete_policy(
    self,
    *,
    PolicyArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_policy method usage example with argument unpacking

kwargs: DeletePolicyRequestRequestTypeDef = {  # (1)
    "PolicyArn": ...,
}

parent.delete_policy(**kwargs)
```

1. See [:material-code-braces: DeletePolicyRequestRequestTypeDef](./type_defs.md#deletepolicyrequestrequesttypedef) 

### delete\_policy\_version

Deletes the specified version from the specified managed policy.

Type annotations and code completion for `#!python session.create_client("iam").delete_policy_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_policy_version.html)

```python
# delete_policy_version method definition

await def delete_policy_version(
    self,
    *,
    PolicyArn: str,
    VersionId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_policy_version method usage example with argument unpacking

kwargs: DeletePolicyVersionRequestRequestTypeDef = {  # (1)
    "PolicyArn": ...,
    "VersionId": ...,
}

parent.delete_policy_version(**kwargs)
```

1. See [:material-code-braces: DeletePolicyVersionRequestRequestTypeDef](./type_defs.md#deletepolicyversionrequestrequesttypedef) 

### delete\_role

Deletes the specified role.

Type annotations and code completion for `#!python session.create_client("iam").delete_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_role.html)

```python
# delete_role method definition

await def delete_role(
    self,
    *,
    RoleName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_role method usage example with argument unpacking

kwargs: DeleteRoleRequestRequestTypeDef = {  # (1)
    "RoleName": ...,
}

parent.delete_role(**kwargs)
```

1. See [:material-code-braces: DeleteRoleRequestRequestTypeDef](./type_defs.md#deleterolerequestrequesttypedef) 

### delete\_role\_permissions\_boundary

Deletes the permissions boundary for the specified IAM role.

Type annotations and code completion for `#!python session.create_client("iam").delete_role_permissions_boundary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_role_permissions_boundary.html)

```python
# delete_role_permissions_boundary method definition

await def delete_role_permissions_boundary(
    self,
    *,
    RoleName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_role_permissions_boundary method usage example with argument unpacking

kwargs: DeleteRolePermissionsBoundaryRequestRequestTypeDef = {  # (1)
    "RoleName": ...,
}

parent.delete_role_permissions_boundary(**kwargs)
```

1. See [:material-code-braces: DeleteRolePermissionsBoundaryRequestRequestTypeDef](./type_defs.md#deleterolepermissionsboundaryrequestrequesttypedef) 

### delete\_role\_policy

Deletes the specified inline policy that is embedded in the specified IAM role.

Type annotations and code completion for `#!python session.create_client("iam").delete_role_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_role_policy.html)

```python
# delete_role_policy method definition

await def delete_role_policy(
    self,
    *,
    RoleName: str,
    PolicyName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_role_policy method usage example with argument unpacking

kwargs: DeleteRolePolicyRequestRequestTypeDef = {  # (1)
    "RoleName": ...,
    "PolicyName": ...,
}

parent.delete_role_policy(**kwargs)
```

1. See [:material-code-braces: DeleteRolePolicyRequestRequestTypeDef](./type_defs.md#deleterolepolicyrequestrequesttypedef) 

### delete\_saml\_provider

Deletes a SAML provider resource in IAM.

Type annotations and code completion for `#!python session.create_client("iam").delete_saml_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_saml_provider.html)

```python
# delete_saml_provider method definition

await def delete_saml_provider(
    self,
    *,
    SAMLProviderArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_saml_provider method usage example with argument unpacking

kwargs: DeleteSAMLProviderRequestRequestTypeDef = {  # (1)
    "SAMLProviderArn": ...,
}

parent.delete_saml_provider(**kwargs)
```

1. See [:material-code-braces: DeleteSAMLProviderRequestRequestTypeDef](./type_defs.md#deletesamlproviderrequestrequesttypedef) 

### delete\_ssh\_public\_key

Deletes the specified SSH public key.

Type annotations and code completion for `#!python session.create_client("iam").delete_ssh_public_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_ssh_public_key.html)

```python
# delete_ssh_public_key method definition

await def delete_ssh_public_key(
    self,
    *,
    UserName: str,
    SSHPublicKeyId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_ssh_public_key method usage example with argument unpacking

kwargs: DeleteSSHPublicKeyRequestRequestTypeDef = {  # (1)
    "UserName": ...,
    "SSHPublicKeyId": ...,
}

parent.delete_ssh_public_key(**kwargs)
```

1. See [:material-code-braces: DeleteSSHPublicKeyRequestRequestTypeDef](./type_defs.md#deletesshpublickeyrequestrequesttypedef) 

### delete\_server\_certificate

Deletes the specified server certificate.

Type annotations and code completion for `#!python session.create_client("iam").delete_server_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_server_certificate.html)

```python
# delete_server_certificate method definition

await def delete_server_certificate(
    self,
    *,
    ServerCertificateName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_server_certificate method usage example with argument unpacking

kwargs: DeleteServerCertificateRequestRequestTypeDef = {  # (1)
    "ServerCertificateName": ...,
}

parent.delete_server_certificate(**kwargs)
```

1. See [:material-code-braces: DeleteServerCertificateRequestRequestTypeDef](./type_defs.md#deleteservercertificaterequestrequesttypedef) 

### delete\_service\_linked\_role

Submits a service-linked role deletion request and returns a
<code>DeletionTaskId</code>, which you can use to check the status of the
deletion.

Type annotations and code completion for `#!python session.create_client("iam").delete_service_linked_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_service_linked_role.html)

```python
# delete_service_linked_role method definition

await def delete_service_linked_role(
    self,
    *,
    RoleName: str,
) -> DeleteServiceLinkedRoleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteServiceLinkedRoleResponseTypeDef](./type_defs.md#deleteservicelinkedroleresponsetypedef) 


```python
# delete_service_linked_role method usage example with argument unpacking

kwargs: DeleteServiceLinkedRoleRequestRequestTypeDef = {  # (1)
    "RoleName": ...,
}

parent.delete_service_linked_role(**kwargs)
```

1. See [:material-code-braces: DeleteServiceLinkedRoleRequestRequestTypeDef](./type_defs.md#deleteservicelinkedrolerequestrequesttypedef) 

### delete\_service\_specific\_credential

Deletes the specified service-specific credential.

Type annotations and code completion for `#!python session.create_client("iam").delete_service_specific_credential` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_service_specific_credential.html)

```python
# delete_service_specific_credential method definition

await def delete_service_specific_credential(
    self,
    *,
    ServiceSpecificCredentialId: str,
    UserName: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_service_specific_credential method usage example with argument unpacking

kwargs: DeleteServiceSpecificCredentialRequestRequestTypeDef = {  # (1)
    "ServiceSpecificCredentialId": ...,
}

parent.delete_service_specific_credential(**kwargs)
```

1. See [:material-code-braces: DeleteServiceSpecificCredentialRequestRequestTypeDef](./type_defs.md#deleteservicespecificcredentialrequestrequesttypedef) 

### delete\_signing\_certificate

Deletes a signing certificate associated with the specified IAM user.

Type annotations and code completion for `#!python session.create_client("iam").delete_signing_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_signing_certificate.html)

```python
# delete_signing_certificate method definition

await def delete_signing_certificate(
    self,
    *,
    CertificateId: str,
    UserName: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_signing_certificate method usage example with argument unpacking

kwargs: DeleteSigningCertificateRequestRequestTypeDef = {  # (1)
    "CertificateId": ...,
}

parent.delete_signing_certificate(**kwargs)
```

1. See [:material-code-braces: DeleteSigningCertificateRequestRequestTypeDef](./type_defs.md#deletesigningcertificaterequestrequesttypedef) 

### delete\_user

Deletes the specified IAM user.

Type annotations and code completion for `#!python session.create_client("iam").delete_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_user.html)

```python
# delete_user method definition

await def delete_user(
    self,
    *,
    UserName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_user method usage example with argument unpacking

kwargs: DeleteUserRequestRequestTypeDef = {  # (1)
    "UserName": ...,
}

parent.delete_user(**kwargs)
```

1. See [:material-code-braces: DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef) 

### delete\_user\_permissions\_boundary

Deletes the permissions boundary for the specified IAM user.

Type annotations and code completion for `#!python session.create_client("iam").delete_user_permissions_boundary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_user_permissions_boundary.html)

```python
# delete_user_permissions_boundary method definition

await def delete_user_permissions_boundary(
    self,
    *,
    UserName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_user_permissions_boundary method usage example with argument unpacking

kwargs: DeleteUserPermissionsBoundaryRequestRequestTypeDef = {  # (1)
    "UserName": ...,
}

parent.delete_user_permissions_boundary(**kwargs)
```

1. See [:material-code-braces: DeleteUserPermissionsBoundaryRequestRequestTypeDef](./type_defs.md#deleteuserpermissionsboundaryrequestrequesttypedef) 

### delete\_user\_policy

Deletes the specified inline policy that is embedded in the specified IAM user.

Type annotations and code completion for `#!python session.create_client("iam").delete_user_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_user_policy.html)

```python
# delete_user_policy method definition

await def delete_user_policy(
    self,
    *,
    UserName: str,
    PolicyName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_user_policy method usage example with argument unpacking

kwargs: DeleteUserPolicyRequestRequestTypeDef = {  # (1)
    "UserName": ...,
    "PolicyName": ...,
}

parent.delete_user_policy(**kwargs)
```

1. See [:material-code-braces: DeleteUserPolicyRequestRequestTypeDef](./type_defs.md#deleteuserpolicyrequestrequesttypedef) 

### delete\_virtual\_mfa\_device

Deletes a virtual MFA device.

Type annotations and code completion for `#!python session.create_client("iam").delete_virtual_mfa_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/delete_virtual_mfa_device.html)

```python
# delete_virtual_mfa_device method definition

await def delete_virtual_mfa_device(
    self,
    *,
    SerialNumber: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_virtual_mfa_device method usage example with argument unpacking

kwargs: DeleteVirtualMFADeviceRequestRequestTypeDef = {  # (1)
    "SerialNumber": ...,
}

parent.delete_virtual_mfa_device(**kwargs)
```

1. See [:material-code-braces: DeleteVirtualMFADeviceRequestRequestTypeDef](./type_defs.md#deletevirtualmfadevicerequestrequesttypedef) 

### detach\_group\_policy

Removes the specified managed policy from the specified IAM group.

Type annotations and code completion for `#!python session.create_client("iam").detach_group_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/detach_group_policy.html)

```python
# detach_group_policy method definition

await def detach_group_policy(
    self,
    *,
    GroupName: str,
    PolicyArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# detach_group_policy method usage example with argument unpacking

kwargs: DetachGroupPolicyRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
    "PolicyArn": ...,
}

parent.detach_group_policy(**kwargs)
```

1. See [:material-code-braces: DetachGroupPolicyRequestRequestTypeDef](./type_defs.md#detachgrouppolicyrequestrequesttypedef) 

### detach\_role\_policy

Removes the specified managed policy from the specified role.

Type annotations and code completion for `#!python session.create_client("iam").detach_role_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/detach_role_policy.html)

```python
# detach_role_policy method definition

await def detach_role_policy(
    self,
    *,
    RoleName: str,
    PolicyArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# detach_role_policy method usage example with argument unpacking

kwargs: DetachRolePolicyRequestRequestTypeDef = {  # (1)
    "RoleName": ...,
    "PolicyArn": ...,
}

parent.detach_role_policy(**kwargs)
```

1. See [:material-code-braces: DetachRolePolicyRequestRequestTypeDef](./type_defs.md#detachrolepolicyrequestrequesttypedef) 

### detach\_user\_policy

Removes the specified managed policy from the specified user.

Type annotations and code completion for `#!python session.create_client("iam").detach_user_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/detach_user_policy.html)

```python
# detach_user_policy method definition

await def detach_user_policy(
    self,
    *,
    UserName: str,
    PolicyArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# detach_user_policy method usage example with argument unpacking

kwargs: DetachUserPolicyRequestRequestTypeDef = {  # (1)
    "UserName": ...,
    "PolicyArn": ...,
}

parent.detach_user_policy(**kwargs)
```

1. See [:material-code-braces: DetachUserPolicyRequestRequestTypeDef](./type_defs.md#detachuserpolicyrequestrequesttypedef) 

### disable\_organizations\_root\_credentials\_management

Disables the management of privileged root user credentials across member
accounts in your organization.

Type annotations and code completion for `#!python session.create_client("iam").disable_organizations_root_credentials_management` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/disable_organizations_root_credentials_management.html)

```python
# disable_organizations_root_credentials_management method definition

await def disable_organizations_root_credentials_management(
    self,
) -> DisableOrganizationsRootCredentialsManagementResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisableOrganizationsRootCredentialsManagementResponseTypeDef](./type_defs.md#disableorganizationsrootcredentialsmanagementresponsetypedef) 

### disable\_organizations\_root\_sessions

Disables root user sessions for privileged tasks across member accounts in your
organization.

Type annotations and code completion for `#!python session.create_client("iam").disable_organizations_root_sessions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/disable_organizations_root_sessions.html)

```python
# disable_organizations_root_sessions method definition

await def disable_organizations_root_sessions(
    self,
) -> DisableOrganizationsRootSessionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisableOrganizationsRootSessionsResponseTypeDef](./type_defs.md#disableorganizationsrootsessionsresponsetypedef) 

### enable\_mfa\_device

Enables the specified MFA device and associates it with the specified IAM user.

Type annotations and code completion for `#!python session.create_client("iam").enable_mfa_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/enable_mfa_device.html)

```python
# enable_mfa_device method definition

await def enable_mfa_device(
    self,
    *,
    UserName: str,
    SerialNumber: str,
    AuthenticationCode1: str,
    AuthenticationCode2: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# enable_mfa_device method usage example with argument unpacking

kwargs: EnableMFADeviceRequestRequestTypeDef = {  # (1)
    "UserName": ...,
    "SerialNumber": ...,
    "AuthenticationCode1": ...,
    "AuthenticationCode2": ...,
}

parent.enable_mfa_device(**kwargs)
```

1. See [:material-code-braces: EnableMFADeviceRequestRequestTypeDef](./type_defs.md#enablemfadevicerequestrequesttypedef) 

### enable\_organizations\_root\_credentials\_management

Enables the management of privileged root user credentials across member
accounts in your organization.

Type annotations and code completion for `#!python session.create_client("iam").enable_organizations_root_credentials_management` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/enable_organizations_root_credentials_management.html)

```python
# enable_organizations_root_credentials_management method definition

await def enable_organizations_root_credentials_management(
    self,
) -> EnableOrganizationsRootCredentialsManagementResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EnableOrganizationsRootCredentialsManagementResponseTypeDef](./type_defs.md#enableorganizationsrootcredentialsmanagementresponsetypedef) 

### enable\_organizations\_root\_sessions

Allows the management account or delegated administrator to perform privileged
tasks on member accounts in your organization.

Type annotations and code completion for `#!python session.create_client("iam").enable_organizations_root_sessions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/enable_organizations_root_sessions.html)

```python
# enable_organizations_root_sessions method definition

await def enable_organizations_root_sessions(
    self,
) -> EnableOrganizationsRootSessionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EnableOrganizationsRootSessionsResponseTypeDef](./type_defs.md#enableorganizationsrootsessionsresponsetypedef) 

### generate\_credential\_report

Generates a credential report for the Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("iam").generate_credential_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/generate_credential_report.html)

```python
# generate_credential_report method definition

await def generate_credential_report(
    self,
) -> GenerateCredentialReportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GenerateCredentialReportResponseTypeDef](./type_defs.md#generatecredentialreportresponsetypedef) 

### generate\_organizations\_access\_report

Generates a report for service last accessed data for Organizations.

Type annotations and code completion for `#!python session.create_client("iam").generate_organizations_access_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/generate_organizations_access_report.html)

```python
# generate_organizations_access_report method definition

await def generate_organizations_access_report(
    self,
    *,
    EntityPath: str,
    OrganizationsPolicyId: str = ...,
) -> GenerateOrganizationsAccessReportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GenerateOrganizationsAccessReportResponseTypeDef](./type_defs.md#generateorganizationsaccessreportresponsetypedef) 


```python
# generate_organizations_access_report method usage example with argument unpacking

kwargs: GenerateOrganizationsAccessReportRequestRequestTypeDef = {  # (1)
    "EntityPath": ...,
}

parent.generate_organizations_access_report(**kwargs)
```

1. See [:material-code-braces: GenerateOrganizationsAccessReportRequestRequestTypeDef](./type_defs.md#generateorganizationsaccessreportrequestrequesttypedef) 

### generate\_service\_last\_accessed\_details

Generates a report that includes details about when an IAM resource (user,
group, role, or policy) was last used in an attempt to access Amazon Web
Services services.

Type annotations and code completion for `#!python session.create_client("iam").generate_service_last_accessed_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/generate_service_last_accessed_details.html)

```python
# generate_service_last_accessed_details method definition

await def generate_service_last_accessed_details(
    self,
    *,
    Arn: str,
    Granularity: AccessAdvisorUsageGranularityTypeType = ...,  # (1)
) -> GenerateServiceLastAccessedDetailsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AccessAdvisorUsageGranularityTypeType](./literals.md#accessadvisorusagegranularitytypetype) 
2. See [:material-code-braces: GenerateServiceLastAccessedDetailsResponseTypeDef](./type_defs.md#generateservicelastaccesseddetailsresponsetypedef) 


```python
# generate_service_last_accessed_details method usage example with argument unpacking

kwargs: GenerateServiceLastAccessedDetailsRequestRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.generate_service_last_accessed_details(**kwargs)
```

1. See [:material-code-braces: GenerateServiceLastAccessedDetailsRequestRequestTypeDef](./type_defs.md#generateservicelastaccesseddetailsrequestrequesttypedef) 

### get\_access\_key\_last\_used

Retrieves information about when the specified access key was last used.

Type annotations and code completion for `#!python session.create_client("iam").get_access_key_last_used` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_access_key_last_used.html)

```python
# get_access_key_last_used method definition

await def get_access_key_last_used(
    self,
    *,
    AccessKeyId: str,
) -> GetAccessKeyLastUsedResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccessKeyLastUsedResponseTypeDef](./type_defs.md#getaccesskeylastusedresponsetypedef) 


```python
# get_access_key_last_used method usage example with argument unpacking

kwargs: GetAccessKeyLastUsedRequestRequestTypeDef = {  # (1)
    "AccessKeyId": ...,
}

parent.get_access_key_last_used(**kwargs)
```

1. See [:material-code-braces: GetAccessKeyLastUsedRequestRequestTypeDef](./type_defs.md#getaccesskeylastusedrequestrequesttypedef) 

### get\_account\_authorization\_details

Retrieves information about all IAM users, groups, roles, and policies in your
Amazon Web Services account, including their relationships to one another.

Type annotations and code completion for `#!python session.create_client("iam").get_account_authorization_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_account_authorization_details.html)

```python
# get_account_authorization_details method definition

await def get_account_authorization_details(
    self,
    *,
    Filter: Sequence[EntityTypeType] = ...,  # (1)
    MaxItems: int = ...,
    Marker: str = ...,
) -> GetAccountAuthorizationDetailsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
2. See [:material-code-braces: GetAccountAuthorizationDetailsResponseTypeDef](./type_defs.md#getaccountauthorizationdetailsresponsetypedef) 


```python
# get_account_authorization_details method usage example with argument unpacking

kwargs: GetAccountAuthorizationDetailsRequestRequestTypeDef = {  # (1)
    "Filter": ...,
}

parent.get_account_authorization_details(**kwargs)
```

1. See [:material-code-braces: GetAccountAuthorizationDetailsRequestRequestTypeDef](./type_defs.md#getaccountauthorizationdetailsrequestrequesttypedef) 

### get\_account\_password\_policy

Retrieves the password policy for the Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("iam").get_account_password_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_account_password_policy.html)

```python
# get_account_password_policy method definition

await def get_account_password_policy(
    self,
) -> GetAccountPasswordPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccountPasswordPolicyResponseTypeDef](./type_defs.md#getaccountpasswordpolicyresponsetypedef) 

### get\_account\_summary

Retrieves information about IAM entity usage and IAM quotas in the Amazon Web
Services account.

Type annotations and code completion for `#!python session.create_client("iam").get_account_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_account_summary.html)

```python
# get_account_summary method definition

await def get_account_summary(
    self,
) -> GetAccountSummaryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccountSummaryResponseTypeDef](./type_defs.md#getaccountsummaryresponsetypedef) 

### get\_context\_keys\_for\_custom\_policy

Gets a list of all of the context keys referenced in the input policies.

Type annotations and code completion for `#!python session.create_client("iam").get_context_keys_for_custom_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_context_keys_for_custom_policy.html)

```python
# get_context_keys_for_custom_policy method definition

await def get_context_keys_for_custom_policy(
    self,
    *,
    PolicyInputList: Sequence[str],
) -> GetContextKeysForPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetContextKeysForPolicyResponseTypeDef](./type_defs.md#getcontextkeysforpolicyresponsetypedef) 


```python
# get_context_keys_for_custom_policy method usage example with argument unpacking

kwargs: GetContextKeysForCustomPolicyRequestRequestTypeDef = {  # (1)
    "PolicyInputList": ...,
}

parent.get_context_keys_for_custom_policy(**kwargs)
```

1. See [:material-code-braces: GetContextKeysForCustomPolicyRequestRequestTypeDef](./type_defs.md#getcontextkeysforcustompolicyrequestrequesttypedef) 

### get\_context\_keys\_for\_principal\_policy

Gets a list of all of the context keys referenced in all the IAM policies that
are attached to the specified IAM entity.

Type annotations and code completion for `#!python session.create_client("iam").get_context_keys_for_principal_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_context_keys_for_principal_policy.html)

```python
# get_context_keys_for_principal_policy method definition

await def get_context_keys_for_principal_policy(
    self,
    *,
    PolicySourceArn: str,
    PolicyInputList: Sequence[str] = ...,
) -> GetContextKeysForPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetContextKeysForPolicyResponseTypeDef](./type_defs.md#getcontextkeysforpolicyresponsetypedef) 


```python
# get_context_keys_for_principal_policy method usage example with argument unpacking

kwargs: GetContextKeysForPrincipalPolicyRequestRequestTypeDef = {  # (1)
    "PolicySourceArn": ...,
}

parent.get_context_keys_for_principal_policy(**kwargs)
```

1. See [:material-code-braces: GetContextKeysForPrincipalPolicyRequestRequestTypeDef](./type_defs.md#getcontextkeysforprincipalpolicyrequestrequesttypedef) 

### get\_credential\_report

Retrieves a credential report for the Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("iam").get_credential_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_credential_report.html)

```python
# get_credential_report method definition

await def get_credential_report(
    self,
) -> GetCredentialReportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCredentialReportResponseTypeDef](./type_defs.md#getcredentialreportresponsetypedef) 

### get\_group

Returns a list of IAM users that are in the specified IAM group.

Type annotations and code completion for `#!python session.create_client("iam").get_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_group.html)

```python
# get_group method definition

await def get_group(
    self,
    *,
    GroupName: str,
    Marker: str = ...,
    MaxItems: int = ...,
) -> GetGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGroupResponseTypeDef](./type_defs.md#getgroupresponsetypedef) 


```python
# get_group method usage example with argument unpacking

kwargs: GetGroupRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
}

parent.get_group(**kwargs)
```

1. See [:material-code-braces: GetGroupRequestRequestTypeDef](./type_defs.md#getgrouprequestrequesttypedef) 

### get\_group\_policy

Retrieves the specified inline policy document that is embedded in the
specified IAM group.

Type annotations and code completion for `#!python session.create_client("iam").get_group_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_group_policy.html)

```python
# get_group_policy method definition

await def get_group_policy(
    self,
    *,
    GroupName: str,
    PolicyName: str,
) -> GetGroupPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGroupPolicyResponseTypeDef](./type_defs.md#getgrouppolicyresponsetypedef) 


```python
# get_group_policy method usage example with argument unpacking

kwargs: GetGroupPolicyRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
    "PolicyName": ...,
}

parent.get_group_policy(**kwargs)
```

1. See [:material-code-braces: GetGroupPolicyRequestRequestTypeDef](./type_defs.md#getgrouppolicyrequestrequesttypedef) 

### get\_instance\_profile

Retrieves information about the specified instance profile, including the
instance profile's path, GUID, ARN, and role.

Type annotations and code completion for `#!python session.create_client("iam").get_instance_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_instance_profile.html)

```python
# get_instance_profile method definition

await def get_instance_profile(
    self,
    *,
    InstanceProfileName: str,
) -> GetInstanceProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInstanceProfileResponseTypeDef](./type_defs.md#getinstanceprofileresponsetypedef) 


```python
# get_instance_profile method usage example with argument unpacking

kwargs: GetInstanceProfileRequestRequestTypeDef = {  # (1)
    "InstanceProfileName": ...,
}

parent.get_instance_profile(**kwargs)
```

1. See [:material-code-braces: GetInstanceProfileRequestRequestTypeDef](./type_defs.md#getinstanceprofilerequestrequesttypedef) 

### get\_login\_profile

Retrieves the user name for the specified IAM user.

Type annotations and code completion for `#!python session.create_client("iam").get_login_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_login_profile.html)

```python
# get_login_profile method definition

await def get_login_profile(
    self,
    *,
    UserName: str = ...,
) -> GetLoginProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLoginProfileResponseTypeDef](./type_defs.md#getloginprofileresponsetypedef) 


```python
# get_login_profile method usage example with argument unpacking

kwargs: GetLoginProfileRequestRequestTypeDef = {  # (1)
    "UserName": ...,
}

parent.get_login_profile(**kwargs)
```

1. See [:material-code-braces: GetLoginProfileRequestRequestTypeDef](./type_defs.md#getloginprofilerequestrequesttypedef) 

### get\_mfa\_device

Retrieves information about an MFA device for a specified user.

Type annotations and code completion for `#!python session.create_client("iam").get_mfa_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_mfa_device.html)

```python
# get_mfa_device method definition

await def get_mfa_device(
    self,
    *,
    SerialNumber: str,
    UserName: str = ...,
) -> GetMFADeviceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMFADeviceResponseTypeDef](./type_defs.md#getmfadeviceresponsetypedef) 


```python
# get_mfa_device method usage example with argument unpacking

kwargs: GetMFADeviceRequestRequestTypeDef = {  # (1)
    "SerialNumber": ...,
}

parent.get_mfa_device(**kwargs)
```

1. See [:material-code-braces: GetMFADeviceRequestRequestTypeDef](./type_defs.md#getmfadevicerequestrequesttypedef) 

### get\_open\_id\_connect\_provider

Returns information about the specified OpenID Connect (OIDC) provider resource
object in IAM.

Type annotations and code completion for `#!python session.create_client("iam").get_open_id_connect_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_open_id_connect_provider.html)

```python
# get_open_id_connect_provider method definition

await def get_open_id_connect_provider(
    self,
    *,
    OpenIDConnectProviderArn: str,
) -> GetOpenIDConnectProviderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOpenIDConnectProviderResponseTypeDef](./type_defs.md#getopenidconnectproviderresponsetypedef) 


```python
# get_open_id_connect_provider method usage example with argument unpacking

kwargs: GetOpenIDConnectProviderRequestRequestTypeDef = {  # (1)
    "OpenIDConnectProviderArn": ...,
}

parent.get_open_id_connect_provider(**kwargs)
```

1. See [:material-code-braces: GetOpenIDConnectProviderRequestRequestTypeDef](./type_defs.md#getopenidconnectproviderrequestrequesttypedef) 

### get\_organizations\_access\_report

Retrieves the service last accessed data report for Organizations that was
previously generated using the <code> <a>GenerateOrganizationsAccessReport</a>
</code> operation.

Type annotations and code completion for `#!python session.create_client("iam").get_organizations_access_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_organizations_access_report.html)

```python
# get_organizations_access_report method definition

await def get_organizations_access_report(
    self,
    *,
    JobId: str,
    MaxItems: int = ...,
    Marker: str = ...,
    SortKey: SortKeyTypeType = ...,  # (1)
) -> GetOrganizationsAccessReportResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SortKeyTypeType](./literals.md#sortkeytypetype) 
2. See [:material-code-braces: GetOrganizationsAccessReportResponseTypeDef](./type_defs.md#getorganizationsaccessreportresponsetypedef) 


```python
# get_organizations_access_report method usage example with argument unpacking

kwargs: GetOrganizationsAccessReportRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.get_organizations_access_report(**kwargs)
```

1. See [:material-code-braces: GetOrganizationsAccessReportRequestRequestTypeDef](./type_defs.md#getorganizationsaccessreportrequestrequesttypedef) 

### get\_policy

Retrieves information about the specified managed policy, including the
policy's default version and the total number of IAM users, groups, and roles
to which the policy is attached.

Type annotations and code completion for `#!python session.create_client("iam").get_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_policy.html)

```python
# get_policy method definition

await def get_policy(
    self,
    *,
    PolicyArn: str,
) -> GetPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPolicyResponseTypeDef](./type_defs.md#getpolicyresponsetypedef) 


```python
# get_policy method usage example with argument unpacking

kwargs: GetPolicyRequestRequestTypeDef = {  # (1)
    "PolicyArn": ...,
}

parent.get_policy(**kwargs)
```

1. See [:material-code-braces: GetPolicyRequestRequestTypeDef](./type_defs.md#getpolicyrequestrequesttypedef) 

### get\_policy\_version

Retrieves information about the specified version of the specified managed
policy, including the policy document.

Type annotations and code completion for `#!python session.create_client("iam").get_policy_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_policy_version.html)

```python
# get_policy_version method definition

await def get_policy_version(
    self,
    *,
    PolicyArn: str,
    VersionId: str,
) -> GetPolicyVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPolicyVersionResponseTypeDef](./type_defs.md#getpolicyversionresponsetypedef) 


```python
# get_policy_version method usage example with argument unpacking

kwargs: GetPolicyVersionRequestRequestTypeDef = {  # (1)
    "PolicyArn": ...,
    "VersionId": ...,
}

parent.get_policy_version(**kwargs)
```

1. See [:material-code-braces: GetPolicyVersionRequestRequestTypeDef](./type_defs.md#getpolicyversionrequestrequesttypedef) 

### get\_role

Retrieves information about the specified role, including the role's path,
GUID, ARN, and the role's trust policy that grants permission to assume the
role.

Type annotations and code completion for `#!python session.create_client("iam").get_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_role.html)

```python
# get_role method definition

await def get_role(
    self,
    *,
    RoleName: str,
) -> GetRoleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRoleResponseTypeDef](./type_defs.md#getroleresponsetypedef) 


```python
# get_role method usage example with argument unpacking

kwargs: GetRoleRequestRequestTypeDef = {  # (1)
    "RoleName": ...,
}

parent.get_role(**kwargs)
```

1. See [:material-code-braces: GetRoleRequestRequestTypeDef](./type_defs.md#getrolerequestrequesttypedef) 

### get\_role\_policy

Retrieves the specified inline policy document that is embedded with the
specified IAM role.

Type annotations and code completion for `#!python session.create_client("iam").get_role_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_role_policy.html)

```python
# get_role_policy method definition

await def get_role_policy(
    self,
    *,
    RoleName: str,
    PolicyName: str,
) -> GetRolePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRolePolicyResponseTypeDef](./type_defs.md#getrolepolicyresponsetypedef) 


```python
# get_role_policy method usage example with argument unpacking

kwargs: GetRolePolicyRequestRequestTypeDef = {  # (1)
    "RoleName": ...,
    "PolicyName": ...,
}

parent.get_role_policy(**kwargs)
```

1. See [:material-code-braces: GetRolePolicyRequestRequestTypeDef](./type_defs.md#getrolepolicyrequestrequesttypedef) 

### get\_saml\_provider

Returns the SAML provider metadocument that was uploaded when the IAM SAML
provider resource object was created or updated.

Type annotations and code completion for `#!python session.create_client("iam").get_saml_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_saml_provider.html)

```python
# get_saml_provider method definition

await def get_saml_provider(
    self,
    *,
    SAMLProviderArn: str,
) -> GetSAMLProviderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSAMLProviderResponseTypeDef](./type_defs.md#getsamlproviderresponsetypedef) 


```python
# get_saml_provider method usage example with argument unpacking

kwargs: GetSAMLProviderRequestRequestTypeDef = {  # (1)
    "SAMLProviderArn": ...,
}

parent.get_saml_provider(**kwargs)
```

1. See [:material-code-braces: GetSAMLProviderRequestRequestTypeDef](./type_defs.md#getsamlproviderrequestrequesttypedef) 

### get\_ssh\_public\_key

Retrieves the specified SSH public key, including metadata about the key.

Type annotations and code completion for `#!python session.create_client("iam").get_ssh_public_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_ssh_public_key.html)

```python
# get_ssh_public_key method definition

await def get_ssh_public_key(
    self,
    *,
    UserName: str,
    SSHPublicKeyId: str,
    Encoding: EncodingTypeType,  # (1)
) -> GetSSHPublicKeyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
2. See [:material-code-braces: GetSSHPublicKeyResponseTypeDef](./type_defs.md#getsshpublickeyresponsetypedef) 


```python
# get_ssh_public_key method usage example with argument unpacking

kwargs: GetSSHPublicKeyRequestRequestTypeDef = {  # (1)
    "UserName": ...,
    "SSHPublicKeyId": ...,
    "Encoding": ...,
}

parent.get_ssh_public_key(**kwargs)
```

1. See [:material-code-braces: GetSSHPublicKeyRequestRequestTypeDef](./type_defs.md#getsshpublickeyrequestrequesttypedef) 

### get\_server\_certificate

Retrieves information about the specified server certificate stored in IAM.

Type annotations and code completion for `#!python session.create_client("iam").get_server_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_server_certificate.html)

```python
# get_server_certificate method definition

await def get_server_certificate(
    self,
    *,
    ServerCertificateName: str,
) -> GetServerCertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServerCertificateResponseTypeDef](./type_defs.md#getservercertificateresponsetypedef) 


```python
# get_server_certificate method usage example with argument unpacking

kwargs: GetServerCertificateRequestRequestTypeDef = {  # (1)
    "ServerCertificateName": ...,
}

parent.get_server_certificate(**kwargs)
```

1. See [:material-code-braces: GetServerCertificateRequestRequestTypeDef](./type_defs.md#getservercertificaterequestrequesttypedef) 

### get\_service\_last\_accessed\_details

Retrieves a service last accessed report that was created using the
<code>GenerateServiceLastAccessedDetails</code> operation.

Type annotations and code completion for `#!python session.create_client("iam").get_service_last_accessed_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_service_last_accessed_details.html)

```python
# get_service_last_accessed_details method definition

await def get_service_last_accessed_details(
    self,
    *,
    JobId: str,
    MaxItems: int = ...,
    Marker: str = ...,
) -> GetServiceLastAccessedDetailsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceLastAccessedDetailsResponseTypeDef](./type_defs.md#getservicelastaccesseddetailsresponsetypedef) 


```python
# get_service_last_accessed_details method usage example with argument unpacking

kwargs: GetServiceLastAccessedDetailsRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.get_service_last_accessed_details(**kwargs)
```

1. See [:material-code-braces: GetServiceLastAccessedDetailsRequestRequestTypeDef](./type_defs.md#getservicelastaccesseddetailsrequestrequesttypedef) 

### get\_service\_last\_accessed\_details\_with\_entities

After you generate a group or policy report using the
<code>GenerateServiceLastAccessedDetails</code> operation, you can use the
<code>JobId</code> parameter in
<code>GetServiceLastAccessedDetailsWithEntities</code>.

Type annotations and code completion for `#!python session.create_client("iam").get_service_last_accessed_details_with_entities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_service_last_accessed_details_with_entities.html)

```python
# get_service_last_accessed_details_with_entities method definition

await def get_service_last_accessed_details_with_entities(
    self,
    *,
    JobId: str,
    ServiceNamespace: str,
    MaxItems: int = ...,
    Marker: str = ...,
) -> GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef](./type_defs.md#getservicelastaccesseddetailswithentitiesresponsetypedef) 


```python
# get_service_last_accessed_details_with_entities method usage example with argument unpacking

kwargs: GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef = {  # (1)
    "JobId": ...,
    "ServiceNamespace": ...,
}

parent.get_service_last_accessed_details_with_entities(**kwargs)
```

1. See [:material-code-braces: GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef](./type_defs.md#getservicelastaccesseddetailswithentitiesrequestrequesttypedef) 

### get\_service\_linked\_role\_deletion\_status

Retrieves the status of your service-linked role deletion.

Type annotations and code completion for `#!python session.create_client("iam").get_service_linked_role_deletion_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_service_linked_role_deletion_status.html)

```python
# get_service_linked_role_deletion_status method definition

await def get_service_linked_role_deletion_status(
    self,
    *,
    DeletionTaskId: str,
) -> GetServiceLinkedRoleDeletionStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceLinkedRoleDeletionStatusResponseTypeDef](./type_defs.md#getservicelinkedroledeletionstatusresponsetypedef) 


```python
# get_service_linked_role_deletion_status method usage example with argument unpacking

kwargs: GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef = {  # (1)
    "DeletionTaskId": ...,
}

parent.get_service_linked_role_deletion_status(**kwargs)
```

1. See [:material-code-braces: GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef](./type_defs.md#getservicelinkedroledeletionstatusrequestrequesttypedef) 

### get\_user

Retrieves information about the specified IAM user, including the user's
creation date, path, unique ID, and ARN.

Type annotations and code completion for `#!python session.create_client("iam").get_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_user.html)

```python
# get_user method definition

await def get_user(
    self,
    *,
    UserName: str = ...,
) -> GetUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetUserResponseTypeDef](./type_defs.md#getuserresponsetypedef) 


```python
# get_user method usage example with argument unpacking

kwargs: GetUserRequestRequestTypeDef = {  # (1)
    "UserName": ...,
}

parent.get_user(**kwargs)
```

1. See [:material-code-braces: GetUserRequestRequestTypeDef](./type_defs.md#getuserrequestrequesttypedef) 

### get\_user\_policy

Retrieves the specified inline policy document that is embedded in the
specified IAM user.

Type annotations and code completion for `#!python session.create_client("iam").get_user_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/get_user_policy.html)

```python
# get_user_policy method definition

await def get_user_policy(
    self,
    *,
    UserName: str,
    PolicyName: str,
) -> GetUserPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetUserPolicyResponseTypeDef](./type_defs.md#getuserpolicyresponsetypedef) 


```python
# get_user_policy method usage example with argument unpacking

kwargs: GetUserPolicyRequestRequestTypeDef = {  # (1)
    "UserName": ...,
    "PolicyName": ...,
}

parent.get_user_policy(**kwargs)
```

1. See [:material-code-braces: GetUserPolicyRequestRequestTypeDef](./type_defs.md#getuserpolicyrequestrequesttypedef) 

### list\_access\_keys

Returns information about the access key IDs associated with the specified IAM
user.

Type annotations and code completion for `#!python session.create_client("iam").list_access_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_access_keys.html)

```python
# list_access_keys method definition

await def list_access_keys(
    self,
    *,
    UserName: str = ...,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListAccessKeysResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAccessKeysResponseTypeDef](./type_defs.md#listaccesskeysresponsetypedef) 


```python
# list_access_keys method usage example with argument unpacking

kwargs: ListAccessKeysRequestRequestTypeDef = {  # (1)
    "UserName": ...,
}

parent.list_access_keys(**kwargs)
```

1. See [:material-code-braces: ListAccessKeysRequestRequestTypeDef](./type_defs.md#listaccesskeysrequestrequesttypedef) 

### list\_account\_aliases

Lists the account alias associated with the Amazon Web Services account (Note:
you can have only one).

Type annotations and code completion for `#!python session.create_client("iam").list_account_aliases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_account_aliases.html)

```python
# list_account_aliases method definition

await def list_account_aliases(
    self,
    *,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListAccountAliasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAccountAliasesResponseTypeDef](./type_defs.md#listaccountaliasesresponsetypedef) 


```python
# list_account_aliases method usage example with argument unpacking

kwargs: ListAccountAliasesRequestRequestTypeDef = {  # (1)
    "Marker": ...,
}

parent.list_account_aliases(**kwargs)
```

1. See [:material-code-braces: ListAccountAliasesRequestRequestTypeDef](./type_defs.md#listaccountaliasesrequestrequesttypedef) 

### list\_attached\_group\_policies

Lists all managed policies that are attached to the specified IAM group.

Type annotations and code completion for `#!python session.create_client("iam").list_attached_group_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_attached_group_policies.html)

```python
# list_attached_group_policies method definition

await def list_attached_group_policies(
    self,
    *,
    GroupName: str,
    PathPrefix: str = ...,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListAttachedGroupPoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAttachedGroupPoliciesResponseTypeDef](./type_defs.md#listattachedgrouppoliciesresponsetypedef) 


```python
# list_attached_group_policies method usage example with argument unpacking

kwargs: ListAttachedGroupPoliciesRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
}

parent.list_attached_group_policies(**kwargs)
```

1. See [:material-code-braces: ListAttachedGroupPoliciesRequestRequestTypeDef](./type_defs.md#listattachedgrouppoliciesrequestrequesttypedef) 

### list\_attached\_role\_policies

Lists all managed policies that are attached to the specified IAM role.

Type annotations and code completion for `#!python session.create_client("iam").list_attached_role_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_attached_role_policies.html)

```python
# list_attached_role_policies method definition

await def list_attached_role_policies(
    self,
    *,
    RoleName: str,
    PathPrefix: str = ...,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListAttachedRolePoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAttachedRolePoliciesResponseTypeDef](./type_defs.md#listattachedrolepoliciesresponsetypedef) 


```python
# list_attached_role_policies method usage example with argument unpacking

kwargs: ListAttachedRolePoliciesRequestRequestTypeDef = {  # (1)
    "RoleName": ...,
}

parent.list_attached_role_policies(**kwargs)
```

1. See [:material-code-braces: ListAttachedRolePoliciesRequestRequestTypeDef](./type_defs.md#listattachedrolepoliciesrequestrequesttypedef) 

### list\_attached\_user\_policies

Lists all managed policies that are attached to the specified IAM user.

Type annotations and code completion for `#!python session.create_client("iam").list_attached_user_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_attached_user_policies.html)

```python
# list_attached_user_policies method definition

await def list_attached_user_policies(
    self,
    *,
    UserName: str,
    PathPrefix: str = ...,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListAttachedUserPoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAttachedUserPoliciesResponseTypeDef](./type_defs.md#listattacheduserpoliciesresponsetypedef) 


```python
# list_attached_user_policies method usage example with argument unpacking

kwargs: ListAttachedUserPoliciesRequestRequestTypeDef = {  # (1)
    "UserName": ...,
}

parent.list_attached_user_policies(**kwargs)
```

1. See [:material-code-braces: ListAttachedUserPoliciesRequestRequestTypeDef](./type_defs.md#listattacheduserpoliciesrequestrequesttypedef) 

### list\_entities\_for\_policy

Lists all IAM users, groups, and roles that the specified managed policy is
attached to.

Type annotations and code completion for `#!python session.create_client("iam").list_entities_for_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_entities_for_policy.html)

```python
# list_entities_for_policy method definition

await def list_entities_for_policy(
    self,
    *,
    PolicyArn: str,
    EntityFilter: EntityTypeType = ...,  # (1)
    PathPrefix: str = ...,
    PolicyUsageFilter: PolicyUsageTypeType = ...,  # (2)
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListEntitiesForPolicyResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
2. See [:material-code-brackets: PolicyUsageTypeType](./literals.md#policyusagetypetype) 
3. See [:material-code-braces: ListEntitiesForPolicyResponseTypeDef](./type_defs.md#listentitiesforpolicyresponsetypedef) 


```python
# list_entities_for_policy method usage example with argument unpacking

kwargs: ListEntitiesForPolicyRequestRequestTypeDef = {  # (1)
    "PolicyArn": ...,
}

parent.list_entities_for_policy(**kwargs)
```

1. See [:material-code-braces: ListEntitiesForPolicyRequestRequestTypeDef](./type_defs.md#listentitiesforpolicyrequestrequesttypedef) 

### list\_group\_policies

Lists the names of the inline policies that are embedded in the specified IAM
group.

Type annotations and code completion for `#!python session.create_client("iam").list_group_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_group_policies.html)

```python
# list_group_policies method definition

await def list_group_policies(
    self,
    *,
    GroupName: str,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListGroupPoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGroupPoliciesResponseTypeDef](./type_defs.md#listgrouppoliciesresponsetypedef) 


```python
# list_group_policies method usage example with argument unpacking

kwargs: ListGroupPoliciesRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
}

parent.list_group_policies(**kwargs)
```

1. See [:material-code-braces: ListGroupPoliciesRequestRequestTypeDef](./type_defs.md#listgrouppoliciesrequestrequesttypedef) 

### list\_groups

Lists the IAM groups that have the specified path prefix.

Type annotations and code completion for `#!python session.create_client("iam").list_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_groups.html)

```python
# list_groups method definition

await def list_groups(
    self,
    *,
    PathPrefix: str = ...,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


```python
# list_groups method usage example with argument unpacking

kwargs: ListGroupsRequestRequestTypeDef = {  # (1)
    "PathPrefix": ...,
}

parent.list_groups(**kwargs)
```

1. See [:material-code-braces: ListGroupsRequestRequestTypeDef](./type_defs.md#listgroupsrequestrequesttypedef) 

### list\_groups\_for\_user

Lists the IAM groups that the specified IAM user belongs to.

Type annotations and code completion for `#!python session.create_client("iam").list_groups_for_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_groups_for_user.html)

```python
# list_groups_for_user method definition

await def list_groups_for_user(
    self,
    *,
    UserName: str,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListGroupsForUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGroupsForUserResponseTypeDef](./type_defs.md#listgroupsforuserresponsetypedef) 


```python
# list_groups_for_user method usage example with argument unpacking

kwargs: ListGroupsForUserRequestRequestTypeDef = {  # (1)
    "UserName": ...,
}

parent.list_groups_for_user(**kwargs)
```

1. See [:material-code-braces: ListGroupsForUserRequestRequestTypeDef](./type_defs.md#listgroupsforuserrequestrequesttypedef) 

### list\_instance\_profile\_tags

Lists the tags that are attached to the specified IAM instance profile.

Type annotations and code completion for `#!python session.create_client("iam").list_instance_profile_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_instance_profile_tags.html)

```python
# list_instance_profile_tags method definition

await def list_instance_profile_tags(
    self,
    *,
    InstanceProfileName: str,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListInstanceProfileTagsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListInstanceProfileTagsResponseTypeDef](./type_defs.md#listinstanceprofiletagsresponsetypedef) 


```python
# list_instance_profile_tags method usage example with argument unpacking

kwargs: ListInstanceProfileTagsRequestRequestTypeDef = {  # (1)
    "InstanceProfileName": ...,
}

parent.list_instance_profile_tags(**kwargs)
```

1. See [:material-code-braces: ListInstanceProfileTagsRequestRequestTypeDef](./type_defs.md#listinstanceprofiletagsrequestrequesttypedef) 

### list\_instance\_profiles

Lists the instance profiles that have the specified path prefix.

Type annotations and code completion for `#!python session.create_client("iam").list_instance_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_instance_profiles.html)

```python
# list_instance_profiles method definition

await def list_instance_profiles(
    self,
    *,
    PathPrefix: str = ...,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListInstanceProfilesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListInstanceProfilesResponseTypeDef](./type_defs.md#listinstanceprofilesresponsetypedef) 


```python
# list_instance_profiles method usage example with argument unpacking

kwargs: ListInstanceProfilesRequestRequestTypeDef = {  # (1)
    "PathPrefix": ...,
}

parent.list_instance_profiles(**kwargs)
```

1. See [:material-code-braces: ListInstanceProfilesRequestRequestTypeDef](./type_defs.md#listinstanceprofilesrequestrequesttypedef) 

### list\_instance\_profiles\_for\_role

Lists the instance profiles that have the specified associated IAM role.

Type annotations and code completion for `#!python session.create_client("iam").list_instance_profiles_for_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_instance_profiles_for_role.html)

```python
# list_instance_profiles_for_role method definition

await def list_instance_profiles_for_role(
    self,
    *,
    RoleName: str,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListInstanceProfilesForRoleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListInstanceProfilesForRoleResponseTypeDef](./type_defs.md#listinstanceprofilesforroleresponsetypedef) 


```python
# list_instance_profiles_for_role method usage example with argument unpacking

kwargs: ListInstanceProfilesForRoleRequestRequestTypeDef = {  # (1)
    "RoleName": ...,
}

parent.list_instance_profiles_for_role(**kwargs)
```

1. See [:material-code-braces: ListInstanceProfilesForRoleRequestRequestTypeDef](./type_defs.md#listinstanceprofilesforrolerequestrequesttypedef) 

### list\_mfa\_device\_tags

Lists the tags that are attached to the specified IAM virtual multi-factor
authentication (MFA) device.

Type annotations and code completion for `#!python session.create_client("iam").list_mfa_device_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_mfa_device_tags.html)

```python
# list_mfa_device_tags method definition

await def list_mfa_device_tags(
    self,
    *,
    SerialNumber: str,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListMFADeviceTagsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMFADeviceTagsResponseTypeDef](./type_defs.md#listmfadevicetagsresponsetypedef) 


```python
# list_mfa_device_tags method usage example with argument unpacking

kwargs: ListMFADeviceTagsRequestRequestTypeDef = {  # (1)
    "SerialNumber": ...,
}

parent.list_mfa_device_tags(**kwargs)
```

1. See [:material-code-braces: ListMFADeviceTagsRequestRequestTypeDef](./type_defs.md#listmfadevicetagsrequestrequesttypedef) 

### list\_mfa\_devices

Lists the MFA devices for an IAM user.

Type annotations and code completion for `#!python session.create_client("iam").list_mfa_devices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_mfa_devices.html)

```python
# list_mfa_devices method definition

await def list_mfa_devices(
    self,
    *,
    UserName: str = ...,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListMFADevicesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMFADevicesResponseTypeDef](./type_defs.md#listmfadevicesresponsetypedef) 


```python
# list_mfa_devices method usage example with argument unpacking

kwargs: ListMFADevicesRequestRequestTypeDef = {  # (1)
    "UserName": ...,
}

parent.list_mfa_devices(**kwargs)
```

1. See [:material-code-braces: ListMFADevicesRequestRequestTypeDef](./type_defs.md#listmfadevicesrequestrequesttypedef) 

### list\_open\_id\_connect\_provider\_tags

Lists the tags that are attached to the specified OpenID Connect
(OIDC)-compatible identity provider.

Type annotations and code completion for `#!python session.create_client("iam").list_open_id_connect_provider_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_open_id_connect_provider_tags.html)

```python
# list_open_id_connect_provider_tags method definition

await def list_open_id_connect_provider_tags(
    self,
    *,
    OpenIDConnectProviderArn: str,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListOpenIDConnectProviderTagsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOpenIDConnectProviderTagsResponseTypeDef](./type_defs.md#listopenidconnectprovidertagsresponsetypedef) 


```python
# list_open_id_connect_provider_tags method usage example with argument unpacking

kwargs: ListOpenIDConnectProviderTagsRequestRequestTypeDef = {  # (1)
    "OpenIDConnectProviderArn": ...,
}

parent.list_open_id_connect_provider_tags(**kwargs)
```

1. See [:material-code-braces: ListOpenIDConnectProviderTagsRequestRequestTypeDef](./type_defs.md#listopenidconnectprovidertagsrequestrequesttypedef) 

### list\_open\_id\_connect\_providers

Lists information about the IAM OpenID Connect (OIDC) provider resource objects
defined in the Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("iam").list_open_id_connect_providers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_open_id_connect_providers.html)

```python
# list_open_id_connect_providers method definition

await def list_open_id_connect_providers(
    self,
) -> ListOpenIDConnectProvidersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOpenIDConnectProvidersResponseTypeDef](./type_defs.md#listopenidconnectprovidersresponsetypedef) 

### list\_organizations\_features

Lists the centralized root access features enabled for your organization.

Type annotations and code completion for `#!python session.create_client("iam").list_organizations_features` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_organizations_features.html)

```python
# list_organizations_features method definition

await def list_organizations_features(
    self,
) -> ListOrganizationsFeaturesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOrganizationsFeaturesResponseTypeDef](./type_defs.md#listorganizationsfeaturesresponsetypedef) 

### list\_policies

Lists all the managed policies that are available in your Amazon Web Services
account, including your own customer-defined managed policies and all Amazon
Web Services managed policies.

Type annotations and code completion for `#!python session.create_client("iam").list_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_policies.html)

```python
# list_policies method definition

await def list_policies(
    self,
    *,
    Scope: PolicyScopeTypeType = ...,  # (1)
    OnlyAttached: bool = ...,
    PathPrefix: str = ...,
    PolicyUsageFilter: PolicyUsageTypeType = ...,  # (2)
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListPoliciesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: PolicyScopeTypeType](./literals.md#policyscopetypetype) 
2. See [:material-code-brackets: PolicyUsageTypeType](./literals.md#policyusagetypetype) 
3. See [:material-code-braces: ListPoliciesResponseTypeDef](./type_defs.md#listpoliciesresponsetypedef) 


```python
# list_policies method usage example with argument unpacking

kwargs: ListPoliciesRequestRequestTypeDef = {  # (1)
    "Scope": ...,
}

parent.list_policies(**kwargs)
```

1. See [:material-code-braces: ListPoliciesRequestRequestTypeDef](./type_defs.md#listpoliciesrequestrequesttypedef) 

### list\_policies\_granting\_service\_access

Retrieves a list of policies that the IAM identity (user, group, or role) can
use to access each specified service.

Type annotations and code completion for `#!python session.create_client("iam").list_policies_granting_service_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_policies_granting_service_access.html)

```python
# list_policies_granting_service_access method definition

await def list_policies_granting_service_access(
    self,
    *,
    Arn: str,
    ServiceNamespaces: Sequence[str],
    Marker: str = ...,
) -> ListPoliciesGrantingServiceAccessResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPoliciesGrantingServiceAccessResponseTypeDef](./type_defs.md#listpoliciesgrantingserviceaccessresponsetypedef) 


```python
# list_policies_granting_service_access method usage example with argument unpacking

kwargs: ListPoliciesGrantingServiceAccessRequestRequestTypeDef = {  # (1)
    "Arn": ...,
    "ServiceNamespaces": ...,
}

parent.list_policies_granting_service_access(**kwargs)
```

1. See [:material-code-braces: ListPoliciesGrantingServiceAccessRequestRequestTypeDef](./type_defs.md#listpoliciesgrantingserviceaccessrequestrequesttypedef) 

### list\_policy\_tags

Lists the tags that are attached to the specified IAM customer managed policy.

Type annotations and code completion for `#!python session.create_client("iam").list_policy_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_policy_tags.html)

```python
# list_policy_tags method definition

await def list_policy_tags(
    self,
    *,
    PolicyArn: str,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListPolicyTagsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPolicyTagsResponseTypeDef](./type_defs.md#listpolicytagsresponsetypedef) 


```python
# list_policy_tags method usage example with argument unpacking

kwargs: ListPolicyTagsRequestRequestTypeDef = {  # (1)
    "PolicyArn": ...,
}

parent.list_policy_tags(**kwargs)
```

1. See [:material-code-braces: ListPolicyTagsRequestRequestTypeDef](./type_defs.md#listpolicytagsrequestrequesttypedef) 

### list\_policy\_versions

Lists information about the versions of the specified managed policy, including
the version that is currently set as the policy's default version.

Type annotations and code completion for `#!python session.create_client("iam").list_policy_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_policy_versions.html)

```python
# list_policy_versions method definition

await def list_policy_versions(
    self,
    *,
    PolicyArn: str,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListPolicyVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPolicyVersionsResponseTypeDef](./type_defs.md#listpolicyversionsresponsetypedef) 


```python
# list_policy_versions method usage example with argument unpacking

kwargs: ListPolicyVersionsRequestRequestTypeDef = {  # (1)
    "PolicyArn": ...,
}

parent.list_policy_versions(**kwargs)
```

1. See [:material-code-braces: ListPolicyVersionsRequestRequestTypeDef](./type_defs.md#listpolicyversionsrequestrequesttypedef) 

### list\_role\_policies

Lists the names of the inline policies that are embedded in the specified IAM
role.

Type annotations and code completion for `#!python session.create_client("iam").list_role_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_role_policies.html)

```python
# list_role_policies method definition

await def list_role_policies(
    self,
    *,
    RoleName: str,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListRolePoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRolePoliciesResponseTypeDef](./type_defs.md#listrolepoliciesresponsetypedef) 


```python
# list_role_policies method usage example with argument unpacking

kwargs: ListRolePoliciesRequestRequestTypeDef = {  # (1)
    "RoleName": ...,
}

parent.list_role_policies(**kwargs)
```

1. See [:material-code-braces: ListRolePoliciesRequestRequestTypeDef](./type_defs.md#listrolepoliciesrequestrequesttypedef) 

### list\_role\_tags

Lists the tags that are attached to the specified role.

Type annotations and code completion for `#!python session.create_client("iam").list_role_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_role_tags.html)

```python
# list_role_tags method definition

await def list_role_tags(
    self,
    *,
    RoleName: str,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListRoleTagsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRoleTagsResponseTypeDef](./type_defs.md#listroletagsresponsetypedef) 


```python
# list_role_tags method usage example with argument unpacking

kwargs: ListRoleTagsRequestRequestTypeDef = {  # (1)
    "RoleName": ...,
}

parent.list_role_tags(**kwargs)
```

1. See [:material-code-braces: ListRoleTagsRequestRequestTypeDef](./type_defs.md#listroletagsrequestrequesttypedef) 

### list\_roles

Lists the IAM roles that have the specified path prefix.

Type annotations and code completion for `#!python session.create_client("iam").list_roles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_roles.html)

```python
# list_roles method definition

await def list_roles(
    self,
    *,
    PathPrefix: str = ...,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListRolesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRolesResponseTypeDef](./type_defs.md#listrolesresponsetypedef) 


```python
# list_roles method usage example with argument unpacking

kwargs: ListRolesRequestRequestTypeDef = {  # (1)
    "PathPrefix": ...,
}

parent.list_roles(**kwargs)
```

1. See [:material-code-braces: ListRolesRequestRequestTypeDef](./type_defs.md#listrolesrequestrequesttypedef) 

### list\_saml\_provider\_tags

Lists the tags that are attached to the specified Security Assertion Markup
Language (SAML) identity provider.

Type annotations and code completion for `#!python session.create_client("iam").list_saml_provider_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_saml_provider_tags.html)

```python
# list_saml_provider_tags method definition

await def list_saml_provider_tags(
    self,
    *,
    SAMLProviderArn: str,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListSAMLProviderTagsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSAMLProviderTagsResponseTypeDef](./type_defs.md#listsamlprovidertagsresponsetypedef) 


```python
# list_saml_provider_tags method usage example with argument unpacking

kwargs: ListSAMLProviderTagsRequestRequestTypeDef = {  # (1)
    "SAMLProviderArn": ...,
}

parent.list_saml_provider_tags(**kwargs)
```

1. See [:material-code-braces: ListSAMLProviderTagsRequestRequestTypeDef](./type_defs.md#listsamlprovidertagsrequestrequesttypedef) 

### list\_saml\_providers

Lists the SAML provider resource objects defined in IAM in the account.

Type annotations and code completion for `#!python session.create_client("iam").list_saml_providers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_saml_providers.html)

```python
# list_saml_providers method definition

await def list_saml_providers(
    self,
) -> ListSAMLProvidersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSAMLProvidersResponseTypeDef](./type_defs.md#listsamlprovidersresponsetypedef) 

### list\_ssh\_public\_keys

Returns information about the SSH public keys associated with the specified IAM
user.

Type annotations and code completion for `#!python session.create_client("iam").list_ssh_public_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_ssh_public_keys.html)

```python
# list_ssh_public_keys method definition

await def list_ssh_public_keys(
    self,
    *,
    UserName: str = ...,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListSSHPublicKeysResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSSHPublicKeysResponseTypeDef](./type_defs.md#listsshpublickeysresponsetypedef) 


```python
# list_ssh_public_keys method usage example with argument unpacking

kwargs: ListSSHPublicKeysRequestRequestTypeDef = {  # (1)
    "UserName": ...,
}

parent.list_ssh_public_keys(**kwargs)
```

1. See [:material-code-braces: ListSSHPublicKeysRequestRequestTypeDef](./type_defs.md#listsshpublickeysrequestrequesttypedef) 

### list\_server\_certificate\_tags

Lists the tags that are attached to the specified IAM server certificate.

Type annotations and code completion for `#!python session.create_client("iam").list_server_certificate_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_server_certificate_tags.html)

```python
# list_server_certificate_tags method definition

await def list_server_certificate_tags(
    self,
    *,
    ServerCertificateName: str,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListServerCertificateTagsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListServerCertificateTagsResponseTypeDef](./type_defs.md#listservercertificatetagsresponsetypedef) 


```python
# list_server_certificate_tags method usage example with argument unpacking

kwargs: ListServerCertificateTagsRequestRequestTypeDef = {  # (1)
    "ServerCertificateName": ...,
}

parent.list_server_certificate_tags(**kwargs)
```

1. See [:material-code-braces: ListServerCertificateTagsRequestRequestTypeDef](./type_defs.md#listservercertificatetagsrequestrequesttypedef) 

### list\_server\_certificates

Lists the server certificates stored in IAM that have the specified path prefix.

Type annotations and code completion for `#!python session.create_client("iam").list_server_certificates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_server_certificates.html)

```python
# list_server_certificates method definition

await def list_server_certificates(
    self,
    *,
    PathPrefix: str = ...,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListServerCertificatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListServerCertificatesResponseTypeDef](./type_defs.md#listservercertificatesresponsetypedef) 


```python
# list_server_certificates method usage example with argument unpacking

kwargs: ListServerCertificatesRequestRequestTypeDef = {  # (1)
    "PathPrefix": ...,
}

parent.list_server_certificates(**kwargs)
```

1. See [:material-code-braces: ListServerCertificatesRequestRequestTypeDef](./type_defs.md#listservercertificatesrequestrequesttypedef) 

### list\_service\_specific\_credentials

Returns information about the service-specific credentials associated with the
specified IAM user.

Type annotations and code completion for `#!python session.create_client("iam").list_service_specific_credentials` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_service_specific_credentials.html)

```python
# list_service_specific_credentials method definition

await def list_service_specific_credentials(
    self,
    *,
    UserName: str = ...,
    ServiceName: str = ...,
) -> ListServiceSpecificCredentialsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListServiceSpecificCredentialsResponseTypeDef](./type_defs.md#listservicespecificcredentialsresponsetypedef) 


```python
# list_service_specific_credentials method usage example with argument unpacking

kwargs: ListServiceSpecificCredentialsRequestRequestTypeDef = {  # (1)
    "UserName": ...,
}

parent.list_service_specific_credentials(**kwargs)
```

1. See [:material-code-braces: ListServiceSpecificCredentialsRequestRequestTypeDef](./type_defs.md#listservicespecificcredentialsrequestrequesttypedef) 

### list\_signing\_certificates

Returns information about the signing certificates associated with the
specified IAM user.

Type annotations and code completion for `#!python session.create_client("iam").list_signing_certificates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_signing_certificates.html)

```python
# list_signing_certificates method definition

await def list_signing_certificates(
    self,
    *,
    UserName: str = ...,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListSigningCertificatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSigningCertificatesResponseTypeDef](./type_defs.md#listsigningcertificatesresponsetypedef) 


```python
# list_signing_certificates method usage example with argument unpacking

kwargs: ListSigningCertificatesRequestRequestTypeDef = {  # (1)
    "UserName": ...,
}

parent.list_signing_certificates(**kwargs)
```

1. See [:material-code-braces: ListSigningCertificatesRequestRequestTypeDef](./type_defs.md#listsigningcertificatesrequestrequesttypedef) 

### list\_user\_policies

Lists the names of the inline policies embedded in the specified IAM user.

Type annotations and code completion for `#!python session.create_client("iam").list_user_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_user_policies.html)

```python
# list_user_policies method definition

await def list_user_policies(
    self,
    *,
    UserName: str,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListUserPoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListUserPoliciesResponseTypeDef](./type_defs.md#listuserpoliciesresponsetypedef) 


```python
# list_user_policies method usage example with argument unpacking

kwargs: ListUserPoliciesRequestRequestTypeDef = {  # (1)
    "UserName": ...,
}

parent.list_user_policies(**kwargs)
```

1. See [:material-code-braces: ListUserPoliciesRequestRequestTypeDef](./type_defs.md#listuserpoliciesrequestrequesttypedef) 

### list\_user\_tags

Lists the tags that are attached to the specified IAM user.

Type annotations and code completion for `#!python session.create_client("iam").list_user_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_user_tags.html)

```python
# list_user_tags method definition

await def list_user_tags(
    self,
    *,
    UserName: str,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListUserTagsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListUserTagsResponseTypeDef](./type_defs.md#listusertagsresponsetypedef) 


```python
# list_user_tags method usage example with argument unpacking

kwargs: ListUserTagsRequestRequestTypeDef = {  # (1)
    "UserName": ...,
}

parent.list_user_tags(**kwargs)
```

1. See [:material-code-braces: ListUserTagsRequestRequestTypeDef](./type_defs.md#listusertagsrequestrequesttypedef) 

### list\_users

Lists the IAM users that have the specified path prefix.

Type annotations and code completion for `#!python session.create_client("iam").list_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_users.html)

```python
# list_users method definition

await def list_users(
    self,
    *,
    PathPrefix: str = ...,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListUsersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


```python
# list_users method usage example with argument unpacking

kwargs: ListUsersRequestRequestTypeDef = {  # (1)
    "PathPrefix": ...,
}

parent.list_users(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestRequestTypeDef](./type_defs.md#listusersrequestrequesttypedef) 

### list\_virtual\_mfa\_devices

Lists the virtual MFA devices defined in the Amazon Web Services account by
assignment status.

Type annotations and code completion for `#!python session.create_client("iam").list_virtual_mfa_devices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/list_virtual_mfa_devices.html)

```python
# list_virtual_mfa_devices method definition

await def list_virtual_mfa_devices(
    self,
    *,
    AssignmentStatus: AssignmentStatusTypeType = ...,  # (1)
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListVirtualMFADevicesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AssignmentStatusTypeType](./literals.md#assignmentstatustypetype) 
2. See [:material-code-braces: ListVirtualMFADevicesResponseTypeDef](./type_defs.md#listvirtualmfadevicesresponsetypedef) 


```python
# list_virtual_mfa_devices method usage example with argument unpacking

kwargs: ListVirtualMFADevicesRequestRequestTypeDef = {  # (1)
    "AssignmentStatus": ...,
}

parent.list_virtual_mfa_devices(**kwargs)
```

1. See [:material-code-braces: ListVirtualMFADevicesRequestRequestTypeDef](./type_defs.md#listvirtualmfadevicesrequestrequesttypedef) 

### put\_group\_policy

Adds or updates an inline policy document that is embedded in the specified IAM
group.

Type annotations and code completion for `#!python session.create_client("iam").put_group_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/put_group_policy.html)

```python
# put_group_policy method definition

await def put_group_policy(
    self,
    *,
    GroupName: str,
    PolicyName: str,
    PolicyDocument: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_group_policy method usage example with argument unpacking

kwargs: PutGroupPolicyRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
    "PolicyName": ...,
    "PolicyDocument": ...,
}

parent.put_group_policy(**kwargs)
```

1. See [:material-code-braces: PutGroupPolicyRequestRequestTypeDef](./type_defs.md#putgrouppolicyrequestrequesttypedef) 

### put\_role\_permissions\_boundary

Adds or updates the policy that is specified as the IAM role's permissions
boundary.

Type annotations and code completion for `#!python session.create_client("iam").put_role_permissions_boundary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/put_role_permissions_boundary.html)

```python
# put_role_permissions_boundary method definition

await def put_role_permissions_boundary(
    self,
    *,
    RoleName: str,
    PermissionsBoundary: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_role_permissions_boundary method usage example with argument unpacking

kwargs: PutRolePermissionsBoundaryRequestRequestTypeDef = {  # (1)
    "RoleName": ...,
    "PermissionsBoundary": ...,
}

parent.put_role_permissions_boundary(**kwargs)
```

1. See [:material-code-braces: PutRolePermissionsBoundaryRequestRequestTypeDef](./type_defs.md#putrolepermissionsboundaryrequestrequesttypedef) 

### put\_role\_policy

Adds or updates an inline policy document that is embedded in the specified IAM
role.

Type annotations and code completion for `#!python session.create_client("iam").put_role_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/put_role_policy.html)

```python
# put_role_policy method definition

await def put_role_policy(
    self,
    *,
    RoleName: str,
    PolicyName: str,
    PolicyDocument: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_role_policy method usage example with argument unpacking

kwargs: PutRolePolicyRequestRequestTypeDef = {  # (1)
    "RoleName": ...,
    "PolicyName": ...,
    "PolicyDocument": ...,
}

parent.put_role_policy(**kwargs)
```

1. See [:material-code-braces: PutRolePolicyRequestRequestTypeDef](./type_defs.md#putrolepolicyrequestrequesttypedef) 

### put\_user\_permissions\_boundary

Adds or updates the policy that is specified as the IAM user's permissions
boundary.

Type annotations and code completion for `#!python session.create_client("iam").put_user_permissions_boundary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/put_user_permissions_boundary.html)

```python
# put_user_permissions_boundary method definition

await def put_user_permissions_boundary(
    self,
    *,
    UserName: str,
    PermissionsBoundary: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_user_permissions_boundary method usage example with argument unpacking

kwargs: PutUserPermissionsBoundaryRequestRequestTypeDef = {  # (1)
    "UserName": ...,
    "PermissionsBoundary": ...,
}

parent.put_user_permissions_boundary(**kwargs)
```

1. See [:material-code-braces: PutUserPermissionsBoundaryRequestRequestTypeDef](./type_defs.md#putuserpermissionsboundaryrequestrequesttypedef) 

### put\_user\_policy

Adds or updates an inline policy document that is embedded in the specified IAM
user.

Type annotations and code completion for `#!python session.create_client("iam").put_user_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/put_user_policy.html)

```python
# put_user_policy method definition

await def put_user_policy(
    self,
    *,
    UserName: str,
    PolicyName: str,
    PolicyDocument: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_user_policy method usage example with argument unpacking

kwargs: PutUserPolicyRequestRequestTypeDef = {  # (1)
    "UserName": ...,
    "PolicyName": ...,
    "PolicyDocument": ...,
}

parent.put_user_policy(**kwargs)
```

1. See [:material-code-braces: PutUserPolicyRequestRequestTypeDef](./type_defs.md#putuserpolicyrequestrequesttypedef) 

### remove\_client\_id\_from\_open\_id\_connect\_provider

Removes the specified client ID (also known as audience) from the list of
client IDs registered for the specified IAM OpenID Connect (OIDC) provider
resource object.

Type annotations and code completion for `#!python session.create_client("iam").remove_client_id_from_open_id_connect_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/remove_client_id_from_open_id_connect_provider.html)

```python
# remove_client_id_from_open_id_connect_provider method definition

await def remove_client_id_from_open_id_connect_provider(
    self,
    *,
    OpenIDConnectProviderArn: str,
    ClientID: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# remove_client_id_from_open_id_connect_provider method usage example with argument unpacking

kwargs: RemoveClientIDFromOpenIDConnectProviderRequestRequestTypeDef = {  # (1)
    "OpenIDConnectProviderArn": ...,
    "ClientID": ...,
}

parent.remove_client_id_from_open_id_connect_provider(**kwargs)
```

1. See [:material-code-braces: RemoveClientIDFromOpenIDConnectProviderRequestRequestTypeDef](./type_defs.md#removeclientidfromopenidconnectproviderrequestrequesttypedef) 

### remove\_role\_from\_instance\_profile

Removes the specified IAM role from the specified Amazon EC2 instance profile.

Type annotations and code completion for `#!python session.create_client("iam").remove_role_from_instance_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/remove_role_from_instance_profile.html)

```python
# remove_role_from_instance_profile method definition

await def remove_role_from_instance_profile(
    self,
    *,
    InstanceProfileName: str,
    RoleName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# remove_role_from_instance_profile method usage example with argument unpacking

kwargs: RemoveRoleFromInstanceProfileRequestRequestTypeDef = {  # (1)
    "InstanceProfileName": ...,
    "RoleName": ...,
}

parent.remove_role_from_instance_profile(**kwargs)
```

1. See [:material-code-braces: RemoveRoleFromInstanceProfileRequestRequestTypeDef](./type_defs.md#removerolefrominstanceprofilerequestrequesttypedef) 

### remove\_user\_from\_group

Removes the specified user from the specified group.

Type annotations and code completion for `#!python session.create_client("iam").remove_user_from_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/remove_user_from_group.html)

```python
# remove_user_from_group method definition

await def remove_user_from_group(
    self,
    *,
    GroupName: str,
    UserName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# remove_user_from_group method usage example with argument unpacking

kwargs: RemoveUserFromGroupRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
    "UserName": ...,
}

parent.remove_user_from_group(**kwargs)
```

1. See [:material-code-braces: RemoveUserFromGroupRequestRequestTypeDef](./type_defs.md#removeuserfromgrouprequestrequesttypedef) 

### reset\_service\_specific\_credential

Resets the password for a service-specific credential.

Type annotations and code completion for `#!python session.create_client("iam").reset_service_specific_credential` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/reset_service_specific_credential.html)

```python
# reset_service_specific_credential method definition

await def reset_service_specific_credential(
    self,
    *,
    ServiceSpecificCredentialId: str,
    UserName: str = ...,
) -> ResetServiceSpecificCredentialResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResetServiceSpecificCredentialResponseTypeDef](./type_defs.md#resetservicespecificcredentialresponsetypedef) 


```python
# reset_service_specific_credential method usage example with argument unpacking

kwargs: ResetServiceSpecificCredentialRequestRequestTypeDef = {  # (1)
    "ServiceSpecificCredentialId": ...,
}

parent.reset_service_specific_credential(**kwargs)
```

1. See [:material-code-braces: ResetServiceSpecificCredentialRequestRequestTypeDef](./type_defs.md#resetservicespecificcredentialrequestrequesttypedef) 

### resync\_mfa\_device

Synchronizes the specified MFA device with its IAM resource object on the
Amazon Web Services servers.

Type annotations and code completion for `#!python session.create_client("iam").resync_mfa_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/resync_mfa_device.html)

```python
# resync_mfa_device method definition

await def resync_mfa_device(
    self,
    *,
    UserName: str,
    SerialNumber: str,
    AuthenticationCode1: str,
    AuthenticationCode2: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# resync_mfa_device method usage example with argument unpacking

kwargs: ResyncMFADeviceRequestRequestTypeDef = {  # (1)
    "UserName": ...,
    "SerialNumber": ...,
    "AuthenticationCode1": ...,
    "AuthenticationCode2": ...,
}

parent.resync_mfa_device(**kwargs)
```

1. See [:material-code-braces: ResyncMFADeviceRequestRequestTypeDef](./type_defs.md#resyncmfadevicerequestrequesttypedef) 

### set\_default\_policy\_version

Sets the specified version of the specified policy as the policy's default
(operative) version.

Type annotations and code completion for `#!python session.create_client("iam").set_default_policy_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/set_default_policy_version.html)

```python
# set_default_policy_version method definition

await def set_default_policy_version(
    self,
    *,
    PolicyArn: str,
    VersionId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# set_default_policy_version method usage example with argument unpacking

kwargs: SetDefaultPolicyVersionRequestRequestTypeDef = {  # (1)
    "PolicyArn": ...,
    "VersionId": ...,
}

parent.set_default_policy_version(**kwargs)
```

1. See [:material-code-braces: SetDefaultPolicyVersionRequestRequestTypeDef](./type_defs.md#setdefaultpolicyversionrequestrequesttypedef) 

### set\_security\_token\_service\_preferences

Sets the specified version of the global endpoint token as the token version
used for the Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("iam").set_security_token_service_preferences` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/set_security_token_service_preferences.html)

```python
# set_security_token_service_preferences method definition

await def set_security_token_service_preferences(
    self,
    *,
    GlobalEndpointTokenVersion: GlobalEndpointTokenVersionType,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: GlobalEndpointTokenVersionType](./literals.md#globalendpointtokenversiontype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# set_security_token_service_preferences method usage example with argument unpacking

kwargs: SetSecurityTokenServicePreferencesRequestRequestTypeDef = {  # (1)
    "GlobalEndpointTokenVersion": ...,
}

parent.set_security_token_service_preferences(**kwargs)
```

1. See [:material-code-braces: SetSecurityTokenServicePreferencesRequestRequestTypeDef](./type_defs.md#setsecuritytokenservicepreferencesrequestrequesttypedef) 

### simulate\_custom\_policy

Simulate how a set of IAM policies and optionally a resource-based policy works
with a list of API operations and Amazon Web Services resources to determine
the policies' effective permissions.

Type annotations and code completion for `#!python session.create_client("iam").simulate_custom_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/simulate_custom_policy.html)

```python
# simulate_custom_policy method definition

await def simulate_custom_policy(
    self,
    *,
    PolicyInputList: Sequence[str],
    ActionNames: Sequence[str],
    PermissionsBoundaryPolicyInputList: Sequence[str] = ...,
    ResourceArns: Sequence[str] = ...,
    ResourcePolicy: str = ...,
    ResourceOwner: str = ...,
    CallerArn: str = ...,
    ContextEntries: Sequence[ContextEntryTypeDef] = ...,  # (1)
    ResourceHandlingOption: str = ...,
    MaxItems: int = ...,
    Marker: str = ...,
) -> SimulatePolicyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ContextEntryTypeDef](./type_defs.md#contextentrytypedef) 
2. See [:material-code-braces: SimulatePolicyResponseTypeDef](./type_defs.md#simulatepolicyresponsetypedef) 


```python
# simulate_custom_policy method usage example with argument unpacking

kwargs: SimulateCustomPolicyRequestRequestTypeDef = {  # (1)
    "PolicyInputList": ...,
    "ActionNames": ...,
}

parent.simulate_custom_policy(**kwargs)
```

1. See [:material-code-braces: SimulateCustomPolicyRequestRequestTypeDef](./type_defs.md#simulatecustompolicyrequestrequesttypedef) 

### simulate\_principal\_policy

Simulate how a set of IAM policies attached to an IAM entity works with a list
of API operations and Amazon Web Services resources to determine the policies'
effective permissions.

Type annotations and code completion for `#!python session.create_client("iam").simulate_principal_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/simulate_principal_policy.html)

```python
# simulate_principal_policy method definition

await def simulate_principal_policy(
    self,
    *,
    PolicySourceArn: str,
    ActionNames: Sequence[str],
    PolicyInputList: Sequence[str] = ...,
    PermissionsBoundaryPolicyInputList: Sequence[str] = ...,
    ResourceArns: Sequence[str] = ...,
    ResourcePolicy: str = ...,
    ResourceOwner: str = ...,
    CallerArn: str = ...,
    ContextEntries: Sequence[ContextEntryTypeDef] = ...,  # (1)
    ResourceHandlingOption: str = ...,
    MaxItems: int = ...,
    Marker: str = ...,
) -> SimulatePolicyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ContextEntryTypeDef](./type_defs.md#contextentrytypedef) 
2. See [:material-code-braces: SimulatePolicyResponseTypeDef](./type_defs.md#simulatepolicyresponsetypedef) 


```python
# simulate_principal_policy method usage example with argument unpacking

kwargs: SimulatePrincipalPolicyRequestRequestTypeDef = {  # (1)
    "PolicySourceArn": ...,
    "ActionNames": ...,
}

parent.simulate_principal_policy(**kwargs)
```

1. See [:material-code-braces: SimulatePrincipalPolicyRequestRequestTypeDef](./type_defs.md#simulateprincipalpolicyrequestrequesttypedef) 

### tag\_instance\_profile

Adds one or more tags to an IAM instance profile.

Type annotations and code completion for `#!python session.create_client("iam").tag_instance_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/tag_instance_profile.html)

```python
# tag_instance_profile method definition

await def tag_instance_profile(
    self,
    *,
    InstanceProfileName: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_instance_profile method usage example with argument unpacking

kwargs: TagInstanceProfileRequestRequestTypeDef = {  # (1)
    "InstanceProfileName": ...,
    "Tags": ...,
}

parent.tag_instance_profile(**kwargs)
```

1. See [:material-code-braces: TagInstanceProfileRequestRequestTypeDef](./type_defs.md#taginstanceprofilerequestrequesttypedef) 

### tag\_mfa\_device

Adds one or more tags to an IAM virtual multi-factor authentication (MFA)
device.

Type annotations and code completion for `#!python session.create_client("iam").tag_mfa_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/tag_mfa_device.html)

```python
# tag_mfa_device method definition

await def tag_mfa_device(
    self,
    *,
    SerialNumber: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_mfa_device method usage example with argument unpacking

kwargs: TagMFADeviceRequestRequestTypeDef = {  # (1)
    "SerialNumber": ...,
    "Tags": ...,
}

parent.tag_mfa_device(**kwargs)
```

1. See [:material-code-braces: TagMFADeviceRequestRequestTypeDef](./type_defs.md#tagmfadevicerequestrequesttypedef) 

### tag\_open\_id\_connect\_provider

Adds one or more tags to an OpenID Connect (OIDC)-compatible identity provider.

Type annotations and code completion for `#!python session.create_client("iam").tag_open_id_connect_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/tag_open_id_connect_provider.html)

```python
# tag_open_id_connect_provider method definition

await def tag_open_id_connect_provider(
    self,
    *,
    OpenIDConnectProviderArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_open_id_connect_provider method usage example with argument unpacking

kwargs: TagOpenIDConnectProviderRequestRequestTypeDef = {  # (1)
    "OpenIDConnectProviderArn": ...,
    "Tags": ...,
}

parent.tag_open_id_connect_provider(**kwargs)
```

1. See [:material-code-braces: TagOpenIDConnectProviderRequestRequestTypeDef](./type_defs.md#tagopenidconnectproviderrequestrequesttypedef) 

### tag\_policy

Adds one or more tags to an IAM customer managed policy.

Type annotations and code completion for `#!python session.create_client("iam").tag_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/tag_policy.html)

```python
# tag_policy method definition

await def tag_policy(
    self,
    *,
    PolicyArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_policy method usage example with argument unpacking

kwargs: TagPolicyRequestRequestTypeDef = {  # (1)
    "PolicyArn": ...,
    "Tags": ...,
}

parent.tag_policy(**kwargs)
```

1. See [:material-code-braces: TagPolicyRequestRequestTypeDef](./type_defs.md#tagpolicyrequestrequesttypedef) 

### tag\_role

Adds one or more tags to an IAM role.

Type annotations and code completion for `#!python session.create_client("iam").tag_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/tag_role.html)

```python
# tag_role method definition

await def tag_role(
    self,
    *,
    RoleName: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_role method usage example with argument unpacking

kwargs: TagRoleRequestRequestTypeDef = {  # (1)
    "RoleName": ...,
    "Tags": ...,
}

parent.tag_role(**kwargs)
```

1. See [:material-code-braces: TagRoleRequestRequestTypeDef](./type_defs.md#tagrolerequestrequesttypedef) 

### tag\_saml\_provider

Adds one or more tags to a Security Assertion Markup Language (SAML) identity
provider.

Type annotations and code completion for `#!python session.create_client("iam").tag_saml_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/tag_saml_provider.html)

```python
# tag_saml_provider method definition

await def tag_saml_provider(
    self,
    *,
    SAMLProviderArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_saml_provider method usage example with argument unpacking

kwargs: TagSAMLProviderRequestRequestTypeDef = {  # (1)
    "SAMLProviderArn": ...,
    "Tags": ...,
}

parent.tag_saml_provider(**kwargs)
```

1. See [:material-code-braces: TagSAMLProviderRequestRequestTypeDef](./type_defs.md#tagsamlproviderrequestrequesttypedef) 

### tag\_server\_certificate

Adds one or more tags to an IAM server certificate.

Type annotations and code completion for `#!python session.create_client("iam").tag_server_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/tag_server_certificate.html)

```python
# tag_server_certificate method definition

await def tag_server_certificate(
    self,
    *,
    ServerCertificateName: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_server_certificate method usage example with argument unpacking

kwargs: TagServerCertificateRequestRequestTypeDef = {  # (1)
    "ServerCertificateName": ...,
    "Tags": ...,
}

parent.tag_server_certificate(**kwargs)
```

1. See [:material-code-braces: TagServerCertificateRequestRequestTypeDef](./type_defs.md#tagservercertificaterequestrequesttypedef) 

### tag\_user

Adds one or more tags to an IAM user.

Type annotations and code completion for `#!python session.create_client("iam").tag_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/tag_user.html)

```python
# tag_user method definition

await def tag_user(
    self,
    *,
    UserName: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_user method usage example with argument unpacking

kwargs: TagUserRequestRequestTypeDef = {  # (1)
    "UserName": ...,
    "Tags": ...,
}

parent.tag_user(**kwargs)
```

1. See [:material-code-braces: TagUserRequestRequestTypeDef](./type_defs.md#taguserrequestrequesttypedef) 

### untag\_instance\_profile

Removes the specified tags from the IAM instance profile.

Type annotations and code completion for `#!python session.create_client("iam").untag_instance_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/untag_instance_profile.html)

```python
# untag_instance_profile method definition

await def untag_instance_profile(
    self,
    *,
    InstanceProfileName: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_instance_profile method usage example with argument unpacking

kwargs: UntagInstanceProfileRequestRequestTypeDef = {  # (1)
    "InstanceProfileName": ...,
    "TagKeys": ...,
}

parent.untag_instance_profile(**kwargs)
```

1. See [:material-code-braces: UntagInstanceProfileRequestRequestTypeDef](./type_defs.md#untaginstanceprofilerequestrequesttypedef) 

### untag\_mfa\_device

Removes the specified tags from the IAM virtual multi-factor authentication
(MFA) device.

Type annotations and code completion for `#!python session.create_client("iam").untag_mfa_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/untag_mfa_device.html)

```python
# untag_mfa_device method definition

await def untag_mfa_device(
    self,
    *,
    SerialNumber: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_mfa_device method usage example with argument unpacking

kwargs: UntagMFADeviceRequestRequestTypeDef = {  # (1)
    "SerialNumber": ...,
    "TagKeys": ...,
}

parent.untag_mfa_device(**kwargs)
```

1. See [:material-code-braces: UntagMFADeviceRequestRequestTypeDef](./type_defs.md#untagmfadevicerequestrequesttypedef) 

### untag\_open\_id\_connect\_provider

Removes the specified tags from the specified OpenID Connect (OIDC)-compatible
identity provider in IAM.

Type annotations and code completion for `#!python session.create_client("iam").untag_open_id_connect_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/untag_open_id_connect_provider.html)

```python
# untag_open_id_connect_provider method definition

await def untag_open_id_connect_provider(
    self,
    *,
    OpenIDConnectProviderArn: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_open_id_connect_provider method usage example with argument unpacking

kwargs: UntagOpenIDConnectProviderRequestRequestTypeDef = {  # (1)
    "OpenIDConnectProviderArn": ...,
    "TagKeys": ...,
}

parent.untag_open_id_connect_provider(**kwargs)
```

1. See [:material-code-braces: UntagOpenIDConnectProviderRequestRequestTypeDef](./type_defs.md#untagopenidconnectproviderrequestrequesttypedef) 

### untag\_policy

Removes the specified tags from the customer managed policy.

Type annotations and code completion for `#!python session.create_client("iam").untag_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/untag_policy.html)

```python
# untag_policy method definition

await def untag_policy(
    self,
    *,
    PolicyArn: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_policy method usage example with argument unpacking

kwargs: UntagPolicyRequestRequestTypeDef = {  # (1)
    "PolicyArn": ...,
    "TagKeys": ...,
}

parent.untag_policy(**kwargs)
```

1. See [:material-code-braces: UntagPolicyRequestRequestTypeDef](./type_defs.md#untagpolicyrequestrequesttypedef) 

### untag\_role

Removes the specified tags from the role.

Type annotations and code completion for `#!python session.create_client("iam").untag_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/untag_role.html)

```python
# untag_role method definition

await def untag_role(
    self,
    *,
    RoleName: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_role method usage example with argument unpacking

kwargs: UntagRoleRequestRequestTypeDef = {  # (1)
    "RoleName": ...,
    "TagKeys": ...,
}

parent.untag_role(**kwargs)
```

1. See [:material-code-braces: UntagRoleRequestRequestTypeDef](./type_defs.md#untagrolerequestrequesttypedef) 

### untag\_saml\_provider

Removes the specified tags from the specified Security Assertion Markup
Language (SAML) identity provider in IAM.

Type annotations and code completion for `#!python session.create_client("iam").untag_saml_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/untag_saml_provider.html)

```python
# untag_saml_provider method definition

await def untag_saml_provider(
    self,
    *,
    SAMLProviderArn: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_saml_provider method usage example with argument unpacking

kwargs: UntagSAMLProviderRequestRequestTypeDef = {  # (1)
    "SAMLProviderArn": ...,
    "TagKeys": ...,
}

parent.untag_saml_provider(**kwargs)
```

1. See [:material-code-braces: UntagSAMLProviderRequestRequestTypeDef](./type_defs.md#untagsamlproviderrequestrequesttypedef) 

### untag\_server\_certificate

Removes the specified tags from the IAM server certificate.

Type annotations and code completion for `#!python session.create_client("iam").untag_server_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/untag_server_certificate.html)

```python
# untag_server_certificate method definition

await def untag_server_certificate(
    self,
    *,
    ServerCertificateName: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_server_certificate method usage example with argument unpacking

kwargs: UntagServerCertificateRequestRequestTypeDef = {  # (1)
    "ServerCertificateName": ...,
    "TagKeys": ...,
}

parent.untag_server_certificate(**kwargs)
```

1. See [:material-code-braces: UntagServerCertificateRequestRequestTypeDef](./type_defs.md#untagservercertificaterequestrequesttypedef) 

### untag\_user

Removes the specified tags from the user.

Type annotations and code completion for `#!python session.create_client("iam").untag_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/untag_user.html)

```python
# untag_user method definition

await def untag_user(
    self,
    *,
    UserName: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_user method usage example with argument unpacking

kwargs: UntagUserRequestRequestTypeDef = {  # (1)
    "UserName": ...,
    "TagKeys": ...,
}

parent.untag_user(**kwargs)
```

1. See [:material-code-braces: UntagUserRequestRequestTypeDef](./type_defs.md#untaguserrequestrequesttypedef) 

### update\_access\_key

Changes the status of the specified access key from Active to Inactive, or vice
versa.

Type annotations and code completion for `#!python session.create_client("iam").update_access_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/update_access_key.html)

```python
# update_access_key method definition

await def update_access_key(
    self,
    *,
    AccessKeyId: str,
    Status: StatusTypeType,  # (1)
    UserName: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_access_key method usage example with argument unpacking

kwargs: UpdateAccessKeyRequestRequestTypeDef = {  # (1)
    "AccessKeyId": ...,
    "Status": ...,
}

parent.update_access_key(**kwargs)
```

1. See [:material-code-braces: UpdateAccessKeyRequestRequestTypeDef](./type_defs.md#updateaccesskeyrequestrequesttypedef) 

### update\_account\_password\_policy

Updates the password policy settings for the Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("iam").update_account_password_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/update_account_password_policy.html)

```python
# update_account_password_policy method definition

await def update_account_password_policy(
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
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_account_password_policy method usage example with argument unpacking

kwargs: UpdateAccountPasswordPolicyRequestRequestTypeDef = {  # (1)
    "MinimumPasswordLength": ...,
}

parent.update_account_password_policy(**kwargs)
```

1. See [:material-code-braces: UpdateAccountPasswordPolicyRequestRequestTypeDef](./type_defs.md#updateaccountpasswordpolicyrequestrequesttypedef) 

### update\_assume\_role\_policy

Updates the policy that grants an IAM entity permission to assume a role.

Type annotations and code completion for `#!python session.create_client("iam").update_assume_role_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/update_assume_role_policy.html)

```python
# update_assume_role_policy method definition

await def update_assume_role_policy(
    self,
    *,
    RoleName: str,
    PolicyDocument: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_assume_role_policy method usage example with argument unpacking

kwargs: UpdateAssumeRolePolicyRequestRequestTypeDef = {  # (1)
    "RoleName": ...,
    "PolicyDocument": ...,
}

parent.update_assume_role_policy(**kwargs)
```

1. See [:material-code-braces: UpdateAssumeRolePolicyRequestRequestTypeDef](./type_defs.md#updateassumerolepolicyrequestrequesttypedef) 

### update\_group

Updates the name and/or the path of the specified IAM group.

Type annotations and code completion for `#!python session.create_client("iam").update_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/update_group.html)

```python
# update_group method definition

await def update_group(
    self,
    *,
    GroupName: str,
    NewPath: str = ...,
    NewGroupName: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_group method usage example with argument unpacking

kwargs: UpdateGroupRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
}

parent.update_group(**kwargs)
```

1. See [:material-code-braces: UpdateGroupRequestRequestTypeDef](./type_defs.md#updategrouprequestrequesttypedef) 

### update\_login\_profile

Changes the password for the specified IAM user.

Type annotations and code completion for `#!python session.create_client("iam").update_login_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/update_login_profile.html)

```python
# update_login_profile method definition

await def update_login_profile(
    self,
    *,
    UserName: str,
    Password: str = ...,
    PasswordResetRequired: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_login_profile method usage example with argument unpacking

kwargs: UpdateLoginProfileRequestRequestTypeDef = {  # (1)
    "UserName": ...,
}

parent.update_login_profile(**kwargs)
```

1. See [:material-code-braces: UpdateLoginProfileRequestRequestTypeDef](./type_defs.md#updateloginprofilerequestrequesttypedef) 

### update\_open\_id\_connect\_provider\_thumbprint

Replaces the existing list of server certificate thumbprints associated with an
OpenID Connect (OIDC) provider resource object with a new list of thumbprints.

Type annotations and code completion for `#!python session.create_client("iam").update_open_id_connect_provider_thumbprint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/update_open_id_connect_provider_thumbprint.html)

```python
# update_open_id_connect_provider_thumbprint method definition

await def update_open_id_connect_provider_thumbprint(
    self,
    *,
    OpenIDConnectProviderArn: str,
    ThumbprintList: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_open_id_connect_provider_thumbprint method usage example with argument unpacking

kwargs: UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef = {  # (1)
    "OpenIDConnectProviderArn": ...,
    "ThumbprintList": ...,
}

parent.update_open_id_connect_provider_thumbprint(**kwargs)
```

1. See [:material-code-braces: UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef](./type_defs.md#updateopenidconnectproviderthumbprintrequestrequesttypedef) 

### update\_role

Updates the description or maximum session duration setting of a role.

Type annotations and code completion for `#!python session.create_client("iam").update_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/update_role.html)

```python
# update_role method definition

await def update_role(
    self,
    *,
    RoleName: str,
    Description: str = ...,
    MaxSessionDuration: int = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_role method usage example with argument unpacking

kwargs: UpdateRoleRequestRequestTypeDef = {  # (1)
    "RoleName": ...,
}

parent.update_role(**kwargs)
```

1. See [:material-code-braces: UpdateRoleRequestRequestTypeDef](./type_defs.md#updaterolerequestrequesttypedef) 

### update\_role\_description

Use <a>UpdateRole</a> instead.

Type annotations and code completion for `#!python session.create_client("iam").update_role_description` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/update_role_description.html)

```python
# update_role_description method definition

await def update_role_description(
    self,
    *,
    RoleName: str,
    Description: str,
) -> UpdateRoleDescriptionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateRoleDescriptionResponseTypeDef](./type_defs.md#updateroledescriptionresponsetypedef) 


```python
# update_role_description method usage example with argument unpacking

kwargs: UpdateRoleDescriptionRequestRequestTypeDef = {  # (1)
    "RoleName": ...,
    "Description": ...,
}

parent.update_role_description(**kwargs)
```

1. See [:material-code-braces: UpdateRoleDescriptionRequestRequestTypeDef](./type_defs.md#updateroledescriptionrequestrequesttypedef) 

### update\_saml\_provider

Updates the metadata document for an existing SAML provider resource object.

Type annotations and code completion for `#!python session.create_client("iam").update_saml_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/update_saml_provider.html)

```python
# update_saml_provider method definition

await def update_saml_provider(
    self,
    *,
    SAMLMetadataDocument: str,
    SAMLProviderArn: str,
) -> UpdateSAMLProviderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateSAMLProviderResponseTypeDef](./type_defs.md#updatesamlproviderresponsetypedef) 


```python
# update_saml_provider method usage example with argument unpacking

kwargs: UpdateSAMLProviderRequestRequestTypeDef = {  # (1)
    "SAMLMetadataDocument": ...,
    "SAMLProviderArn": ...,
}

parent.update_saml_provider(**kwargs)
```

1. See [:material-code-braces: UpdateSAMLProviderRequestRequestTypeDef](./type_defs.md#updatesamlproviderrequestrequesttypedef) 

### update\_ssh\_public\_key

Sets the status of an IAM user's SSH public key to active or inactive.

Type annotations and code completion for `#!python session.create_client("iam").update_ssh_public_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/update_ssh_public_key.html)

```python
# update_ssh_public_key method definition

await def update_ssh_public_key(
    self,
    *,
    UserName: str,
    SSHPublicKeyId: str,
    Status: StatusTypeType,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_ssh_public_key method usage example with argument unpacking

kwargs: UpdateSSHPublicKeyRequestRequestTypeDef = {  # (1)
    "UserName": ...,
    "SSHPublicKeyId": ...,
    "Status": ...,
}

parent.update_ssh_public_key(**kwargs)
```

1. See [:material-code-braces: UpdateSSHPublicKeyRequestRequestTypeDef](./type_defs.md#updatesshpublickeyrequestrequesttypedef) 

### update\_server\_certificate

Updates the name and/or the path of the specified server certificate stored in
IAM.

Type annotations and code completion for `#!python session.create_client("iam").update_server_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/update_server_certificate.html)

```python
# update_server_certificate method definition

await def update_server_certificate(
    self,
    *,
    ServerCertificateName: str,
    NewPath: str = ...,
    NewServerCertificateName: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_server_certificate method usage example with argument unpacking

kwargs: UpdateServerCertificateRequestRequestTypeDef = {  # (1)
    "ServerCertificateName": ...,
}

parent.update_server_certificate(**kwargs)
```

1. See [:material-code-braces: UpdateServerCertificateRequestRequestTypeDef](./type_defs.md#updateservercertificaterequestrequesttypedef) 

### update\_service\_specific\_credential

Sets the status of a service-specific credential to <code>Active</code> or
<code>Inactive</code>.

Type annotations and code completion for `#!python session.create_client("iam").update_service_specific_credential` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/update_service_specific_credential.html)

```python
# update_service_specific_credential method definition

await def update_service_specific_credential(
    self,
    *,
    ServiceSpecificCredentialId: str,
    Status: StatusTypeType,  # (1)
    UserName: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_service_specific_credential method usage example with argument unpacking

kwargs: UpdateServiceSpecificCredentialRequestRequestTypeDef = {  # (1)
    "ServiceSpecificCredentialId": ...,
    "Status": ...,
}

parent.update_service_specific_credential(**kwargs)
```

1. See [:material-code-braces: UpdateServiceSpecificCredentialRequestRequestTypeDef](./type_defs.md#updateservicespecificcredentialrequestrequesttypedef) 

### update\_signing\_certificate

Changes the status of the specified user signing certificate from active to
disabled, or vice versa.

Type annotations and code completion for `#!python session.create_client("iam").update_signing_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/update_signing_certificate.html)

```python
# update_signing_certificate method definition

await def update_signing_certificate(
    self,
    *,
    CertificateId: str,
    Status: StatusTypeType,  # (1)
    UserName: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_signing_certificate method usage example with argument unpacking

kwargs: UpdateSigningCertificateRequestRequestTypeDef = {  # (1)
    "CertificateId": ...,
    "Status": ...,
}

parent.update_signing_certificate(**kwargs)
```

1. See [:material-code-braces: UpdateSigningCertificateRequestRequestTypeDef](./type_defs.md#updatesigningcertificaterequestrequesttypedef) 

### update\_user

Updates the name and/or the path of the specified IAM user.

Type annotations and code completion for `#!python session.create_client("iam").update_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/update_user.html)

```python
# update_user method definition

await def update_user(
    self,
    *,
    UserName: str,
    NewPath: str = ...,
    NewUserName: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_user method usage example with argument unpacking

kwargs: UpdateUserRequestRequestTypeDef = {  # (1)
    "UserName": ...,
}

parent.update_user(**kwargs)
```

1. See [:material-code-braces: UpdateUserRequestRequestTypeDef](./type_defs.md#updateuserrequestrequesttypedef) 

### upload\_ssh\_public\_key

Uploads an SSH public key and associates it with the specified IAM user.

Type annotations and code completion for `#!python session.create_client("iam").upload_ssh_public_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/upload_ssh_public_key.html)

```python
# upload_ssh_public_key method definition

await def upload_ssh_public_key(
    self,
    *,
    UserName: str,
    SSHPublicKeyBody: str,
) -> UploadSSHPublicKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UploadSSHPublicKeyResponseTypeDef](./type_defs.md#uploadsshpublickeyresponsetypedef) 


```python
# upload_ssh_public_key method usage example with argument unpacking

kwargs: UploadSSHPublicKeyRequestRequestTypeDef = {  # (1)
    "UserName": ...,
    "SSHPublicKeyBody": ...,
}

parent.upload_ssh_public_key(**kwargs)
```

1. See [:material-code-braces: UploadSSHPublicKeyRequestRequestTypeDef](./type_defs.md#uploadsshpublickeyrequestrequesttypedef) 

### upload\_server\_certificate

Uploads a server certificate entity for the Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("iam").upload_server_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/upload_server_certificate.html)

```python
# upload_server_certificate method definition

await def upload_server_certificate(
    self,
    *,
    ServerCertificateName: str,
    CertificateBody: str,
    PrivateKey: str,
    Path: str = ...,
    CertificateChain: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> UploadServerCertificateResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: UploadServerCertificateResponseTypeDef](./type_defs.md#uploadservercertificateresponsetypedef) 


```python
# upload_server_certificate method usage example with argument unpacking

kwargs: UploadServerCertificateRequestRequestTypeDef = {  # (1)
    "ServerCertificateName": ...,
    "CertificateBody": ...,
    "PrivateKey": ...,
}

parent.upload_server_certificate(**kwargs)
```

1. See [:material-code-braces: UploadServerCertificateRequestRequestTypeDef](./type_defs.md#uploadservercertificaterequestrequesttypedef) 

### upload\_signing\_certificate

Uploads an X.509 signing certificate and associates it with the specified IAM
user.

Type annotations and code completion for `#!python session.create_client("iam").upload_signing_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/client/upload_signing_certificate.html)

```python
# upload_signing_certificate method definition

await def upload_signing_certificate(
    self,
    *,
    CertificateBody: str,
    UserName: str = ...,
) -> UploadSigningCertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UploadSigningCertificateResponseTypeDef](./type_defs.md#uploadsigningcertificateresponsetypedef) 


```python
# upload_signing_certificate method usage example with argument unpacking

kwargs: UploadSigningCertificateRequestRequestTypeDef = {  # (1)
    "CertificateBody": ...,
}

parent.upload_signing_certificate(**kwargs)
```

1. See [:material-code-braces: UploadSigningCertificateRequestRequestTypeDef](./type_defs.md#uploadsigningcertificaterequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("iam").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "IAMClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("iam").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("iam").get_paginator` method with overloads.

- `client.get_paginator("get_account_authorization_details")` -> [GetAccountAuthorizationDetailsPaginator](./paginators.md#getaccountauthorizationdetailspaginator)
- `client.get_paginator("get_group")` -> [GetGroupPaginator](./paginators.md#getgrouppaginator)
- `client.get_paginator("list_access_keys")` -> [ListAccessKeysPaginator](./paginators.md#listaccesskeyspaginator)
- `client.get_paginator("list_account_aliases")` -> [ListAccountAliasesPaginator](./paginators.md#listaccountaliasespaginator)
- `client.get_paginator("list_attached_group_policies")` -> [ListAttachedGroupPoliciesPaginator](./paginators.md#listattachedgrouppoliciespaginator)
- `client.get_paginator("list_attached_role_policies")` -> [ListAttachedRolePoliciesPaginator](./paginators.md#listattachedrolepoliciespaginator)
- `client.get_paginator("list_attached_user_policies")` -> [ListAttachedUserPoliciesPaginator](./paginators.md#listattacheduserpoliciespaginator)
- `client.get_paginator("list_entities_for_policy")` -> [ListEntitiesForPolicyPaginator](./paginators.md#listentitiesforpolicypaginator)
- `client.get_paginator("list_group_policies")` -> [ListGroupPoliciesPaginator](./paginators.md#listgrouppoliciespaginator)
- `client.get_paginator("list_groups_for_user")` -> [ListGroupsForUserPaginator](./paginators.md#listgroupsforuserpaginator)
- `client.get_paginator("list_groups")` -> [ListGroupsPaginator](./paginators.md#listgroupspaginator)
- `client.get_paginator("list_instance_profile_tags")` -> [ListInstanceProfileTagsPaginator](./paginators.md#listinstanceprofiletagspaginator)
- `client.get_paginator("list_instance_profiles_for_role")` -> [ListInstanceProfilesForRolePaginator](./paginators.md#listinstanceprofilesforrolepaginator)
- `client.get_paginator("list_instance_profiles")` -> [ListInstanceProfilesPaginator](./paginators.md#listinstanceprofilespaginator)
- `client.get_paginator("list_mfa_device_tags")` -> [ListMFADeviceTagsPaginator](./paginators.md#listmfadevicetagspaginator)
- `client.get_paginator("list_mfa_devices")` -> [ListMFADevicesPaginator](./paginators.md#listmfadevicespaginator)
- `client.get_paginator("list_open_id_connect_provider_tags")` -> [ListOpenIDConnectProviderTagsPaginator](./paginators.md#listopenidconnectprovidertagspaginator)
- `client.get_paginator("list_policies")` -> [ListPoliciesPaginator](./paginators.md#listpoliciespaginator)
- `client.get_paginator("list_policy_tags")` -> [ListPolicyTagsPaginator](./paginators.md#listpolicytagspaginator)
- `client.get_paginator("list_policy_versions")` -> [ListPolicyVersionsPaginator](./paginators.md#listpolicyversionspaginator)
- `client.get_paginator("list_role_policies")` -> [ListRolePoliciesPaginator](./paginators.md#listrolepoliciespaginator)
- `client.get_paginator("list_role_tags")` -> [ListRoleTagsPaginator](./paginators.md#listroletagspaginator)
- `client.get_paginator("list_roles")` -> [ListRolesPaginator](./paginators.md#listrolespaginator)
- `client.get_paginator("list_saml_provider_tags")` -> [ListSAMLProviderTagsPaginator](./paginators.md#listsamlprovidertagspaginator)
- `client.get_paginator("list_ssh_public_keys")` -> [ListSSHPublicKeysPaginator](./paginators.md#listsshpublickeyspaginator)
- `client.get_paginator("list_server_certificate_tags")` -> [ListServerCertificateTagsPaginator](./paginators.md#listservercertificatetagspaginator)
- `client.get_paginator("list_server_certificates")` -> [ListServerCertificatesPaginator](./paginators.md#listservercertificatespaginator)
- `client.get_paginator("list_signing_certificates")` -> [ListSigningCertificatesPaginator](./paginators.md#listsigningcertificatespaginator)
- `client.get_paginator("list_user_policies")` -> [ListUserPoliciesPaginator](./paginators.md#listuserpoliciespaginator)
- `client.get_paginator("list_user_tags")` -> [ListUserTagsPaginator](./paginators.md#listusertagspaginator)
- `client.get_paginator("list_users")` -> [ListUsersPaginator](./paginators.md#listuserspaginator)
- `client.get_paginator("list_virtual_mfa_devices")` -> [ListVirtualMFADevicesPaginator](./paginators.md#listvirtualmfadevicespaginator)
- `client.get_paginator("simulate_custom_policy")` -> [SimulateCustomPolicyPaginator](./paginators.md#simulatecustompolicypaginator)
- `client.get_paginator("simulate_principal_policy")` -> [SimulatePrincipalPolicyPaginator](./paginators.md#simulateprincipalpolicypaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("iam").get_waiter` method with overloads.

- `client.get_waiter("instance_profile_exists")` -> [InstanceProfileExistsWaiter](./waiters.md#instanceprofileexistswaiter)
- `client.get_waiter("policy_exists")` -> [PolicyExistsWaiter](./waiters.md#policyexistswaiter)
- `client.get_waiter("role_exists")` -> [RoleExistsWaiter](./waiters.md#roleexistswaiter)
- `client.get_waiter("user_exists")` -> [UserExistsWaiter](./waiters.md#userexistswaiter)

