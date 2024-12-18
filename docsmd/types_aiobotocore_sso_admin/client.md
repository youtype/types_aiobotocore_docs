# SSOAdminClient

> [Index](../README.md) > [SSOAdmin](./README.md) > SSOAdminClient

!!! note ""

    Auto-generated documentation for [SSOAdmin](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#ssoadmin)
    type annotations stubs module [types-aiobotocore-sso-admin](https://pypi.org/project/types-aiobotocore-sso-admin/).

## SSOAdminClient

Type annotations and code completion for `#!python session.create_client("sso-admin")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client)

```python
# SSOAdminClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_sso_admin.client import SSOAdminClient

session = get_session()
async with session.create_client("sso-admin") as client:
    client: SSOAdminClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("sso-admin").exceptions` structure.

```python
# SSOAdminClient.exceptions usage example

async with session.create_client("sso-admin") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# SSOAdminClient usage type checking example

from types_aiobotocore_sso_admin.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("sso-admin").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("sso-admin").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/generate_presigned_url.html)

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



Type annotations and code completion for `#!python session.create_client("sso-admin").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### attach\_customer\_managed\_policy\_reference\_to\_permission\_set

Attaches the specified customer managed policy to the specified
<a>PermissionSet</a>.

Type annotations and code completion for `#!python session.create_client("sso-admin").attach_customer_managed_policy_reference_to_permission_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/attach_customer_managed_policy_reference_to_permission_set.html)

```python
# attach_customer_managed_policy_reference_to_permission_set method definition

await def attach_customer_managed_policy_reference_to_permission_set(
    self,
    *,
    CustomerManagedPolicyReference: CustomerManagedPolicyReferenceTypeDef,  # (1)
    InstanceArn: str,
    PermissionSetArn: str,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: CustomerManagedPolicyReferenceTypeDef](./type_defs.md#customermanagedpolicyreferencetypedef) 


```python
# attach_customer_managed_policy_reference_to_permission_set method usage example with argument unpacking

kwargs: AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef = {  # (1)
    "CustomerManagedPolicyReference": ...,
    "InstanceArn": ...,
    "PermissionSetArn": ...,
}

parent.attach_customer_managed_policy_reference_to_permission_set(**kwargs)
```

1. See [:material-code-braces: AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef](./type_defs.md#attachcustomermanagedpolicyreferencetopermissionsetrequestrequesttypedef) 

### attach\_managed\_policy\_to\_permission\_set

Attaches an Amazon Web Services managed policy ARN to a permission set.

Type annotations and code completion for `#!python session.create_client("sso-admin").attach_managed_policy_to_permission_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/attach_managed_policy_to_permission_set.html)

```python
# attach_managed_policy_to_permission_set method definition

await def attach_managed_policy_to_permission_set(
    self,
    *,
    InstanceArn: str,
    ManagedPolicyArn: str,
    PermissionSetArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# attach_managed_policy_to_permission_set method usage example with argument unpacking

kwargs: AttachManagedPolicyToPermissionSetRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
    "ManagedPolicyArn": ...,
    "PermissionSetArn": ...,
}

parent.attach_managed_policy_to_permission_set(**kwargs)
```

1. See [:material-code-braces: AttachManagedPolicyToPermissionSetRequestRequestTypeDef](./type_defs.md#attachmanagedpolicytopermissionsetrequestrequesttypedef) 

### create\_account\_assignment

Assigns access to a principal for a specified Amazon Web Services account using
a specified permission set.

Type annotations and code completion for `#!python session.create_client("sso-admin").create_account_assignment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/create_account_assignment.html)

```python
# create_account_assignment method definition

await def create_account_assignment(
    self,
    *,
    InstanceArn: str,
    PermissionSetArn: str,
    PrincipalId: str,
    PrincipalType: PrincipalTypeType,  # (1)
    TargetId: str,
    TargetType: TargetTypeType,  # (2)
) -> CreateAccountAssignmentResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
3. See [:material-code-braces: CreateAccountAssignmentResponseTypeDef](./type_defs.md#createaccountassignmentresponsetypedef) 


```python
# create_account_assignment method usage example with argument unpacking

kwargs: CreateAccountAssignmentRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
    "PermissionSetArn": ...,
    "PrincipalId": ...,
    "PrincipalType": ...,
    "TargetId": ...,
    "TargetType": ...,
}

parent.create_account_assignment(**kwargs)
```

1. See [:material-code-braces: CreateAccountAssignmentRequestRequestTypeDef](./type_defs.md#createaccountassignmentrequestrequesttypedef) 

### create\_application

Creates an application in IAM Identity Center for the given application
provider.

Type annotations and code completion for `#!python session.create_client("sso-admin").create_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/create_application.html)

```python
# create_application method definition

await def create_application(
    self,
    *,
    ApplicationProviderArn: str,
    InstanceArn: str,
    Name: str,
    ClientToken: str = ...,
    Description: str = ...,
    PortalOptions: PortalOptionsTypeDef = ...,  # (1)
    Status: ApplicationStatusType = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateApplicationResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: PortalOptionsTypeDef](./type_defs.md#portaloptionstypedef) 
2. See [:material-code-brackets: ApplicationStatusType](./literals.md#applicationstatustype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef) 


```python
# create_application method usage example with argument unpacking

kwargs: CreateApplicationRequestRequestTypeDef = {  # (1)
    "ApplicationProviderArn": ...,
    "InstanceArn": ...,
    "Name": ...,
}

parent.create_application(**kwargs)
```

1. See [:material-code-braces: CreateApplicationRequestRequestTypeDef](./type_defs.md#createapplicationrequestrequesttypedef) 

### create\_application\_assignment

Grant application access to a user or group.

Type annotations and code completion for `#!python session.create_client("sso-admin").create_application_assignment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/create_application_assignment.html)

```python
# create_application_assignment method definition

await def create_application_assignment(
    self,
    *,
    ApplicationArn: str,
    PrincipalId: str,
    PrincipalType: PrincipalTypeType,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 


```python
# create_application_assignment method usage example with argument unpacking

kwargs: CreateApplicationAssignmentRequestRequestTypeDef = {  # (1)
    "ApplicationArn": ...,
    "PrincipalId": ...,
    "PrincipalType": ...,
}

parent.create_application_assignment(**kwargs)
```

1. See [:material-code-braces: CreateApplicationAssignmentRequestRequestTypeDef](./type_defs.md#createapplicationassignmentrequestrequesttypedef) 

### create\_instance

Creates an instance of IAM Identity Center for a standalone Amazon Web Services
account that is not managed by Organizations or a member Amazon Web Services
account in an organization.

Type annotations and code completion for `#!python session.create_client("sso-admin").create_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/create_instance.html)

```python
# create_instance method definition

await def create_instance(
    self,
    *,
    ClientToken: str = ...,
    Name: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateInstanceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateInstanceResponseTypeDef](./type_defs.md#createinstanceresponsetypedef) 


```python
# create_instance method usage example with argument unpacking

kwargs: CreateInstanceRequestRequestTypeDef = {  # (1)
    "ClientToken": ...,
}

parent.create_instance(**kwargs)
```

1. See [:material-code-braces: CreateInstanceRequestRequestTypeDef](./type_defs.md#createinstancerequestrequesttypedef) 

### create\_instance\_access\_control\_attribute\_configuration

Enables the attributes-based access control (ABAC) feature for the specified
IAM Identity Center instance.

Type annotations and code completion for `#!python session.create_client("sso-admin").create_instance_access_control_attribute_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/create_instance_access_control_attribute_configuration.html)

```python
# create_instance_access_control_attribute_configuration method definition

await def create_instance_access_control_attribute_configuration(
    self,
    *,
    InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationTypeDef,  # (1)
    InstanceArn: str,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: InstanceAccessControlAttributeConfigurationTypeDef](./type_defs.md#instanceaccesscontrolattributeconfigurationtypedef) 


```python
# create_instance_access_control_attribute_configuration method usage example with argument unpacking

kwargs: CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef = {  # (1)
    "InstanceAccessControlAttributeConfiguration": ...,
    "InstanceArn": ...,
}

parent.create_instance_access_control_attribute_configuration(**kwargs)
```

1. See [:material-code-braces: CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef](./type_defs.md#createinstanceaccesscontrolattributeconfigurationrequestrequesttypedef) 

### create\_permission\_set

Creates a permission set within a specified IAM Identity Center instance.

Type annotations and code completion for `#!python session.create_client("sso-admin").create_permission_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/create_permission_set.html)

```python
# create_permission_set method definition

await def create_permission_set(
    self,
    *,
    InstanceArn: str,
    Name: str,
    Description: str = ...,
    RelayState: str = ...,
    SessionDuration: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreatePermissionSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreatePermissionSetResponseTypeDef](./type_defs.md#createpermissionsetresponsetypedef) 


```python
# create_permission_set method usage example with argument unpacking

kwargs: CreatePermissionSetRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
    "Name": ...,
}

parent.create_permission_set(**kwargs)
```

1. See [:material-code-braces: CreatePermissionSetRequestRequestTypeDef](./type_defs.md#createpermissionsetrequestrequesttypedef) 

### create\_trusted\_token\_issuer

Creates a connection to a trusted token issuer in an instance of IAM Identity
Center.

Type annotations and code completion for `#!python session.create_client("sso-admin").create_trusted_token_issuer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/create_trusted_token_issuer.html)

```python
# create_trusted_token_issuer method definition

await def create_trusted_token_issuer(
    self,
    *,
    InstanceArn: str,
    Name: str,
    TrustedTokenIssuerConfiguration: TrustedTokenIssuerConfigurationTypeDef,  # (1)
    TrustedTokenIssuerType: TrustedTokenIssuerTypeType,  # (2)
    ClientToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateTrustedTokenIssuerResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: TrustedTokenIssuerConfigurationTypeDef](./type_defs.md#trustedtokenissuerconfigurationtypedef) 
2. See [:material-code-brackets: TrustedTokenIssuerTypeType](./literals.md#trustedtokenissuertypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateTrustedTokenIssuerResponseTypeDef](./type_defs.md#createtrustedtokenissuerresponsetypedef) 


```python
# create_trusted_token_issuer method usage example with argument unpacking

kwargs: CreateTrustedTokenIssuerRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
    "Name": ...,
    "TrustedTokenIssuerConfiguration": ...,
    "TrustedTokenIssuerType": ...,
}

parent.create_trusted_token_issuer(**kwargs)
```

1. See [:material-code-braces: CreateTrustedTokenIssuerRequestRequestTypeDef](./type_defs.md#createtrustedtokenissuerrequestrequesttypedef) 

### delete\_account\_assignment

Deletes a principal's access from a specified Amazon Web Services account using
a specified permission set.

Type annotations and code completion for `#!python session.create_client("sso-admin").delete_account_assignment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/delete_account_assignment.html)

```python
# delete_account_assignment method definition

await def delete_account_assignment(
    self,
    *,
    InstanceArn: str,
    PermissionSetArn: str,
    PrincipalId: str,
    PrincipalType: PrincipalTypeType,  # (1)
    TargetId: str,
    TargetType: TargetTypeType,  # (2)
) -> DeleteAccountAssignmentResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
3. See [:material-code-braces: DeleteAccountAssignmentResponseTypeDef](./type_defs.md#deleteaccountassignmentresponsetypedef) 


```python
# delete_account_assignment method usage example with argument unpacking

kwargs: DeleteAccountAssignmentRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
    "PermissionSetArn": ...,
    "PrincipalId": ...,
    "PrincipalType": ...,
    "TargetId": ...,
    "TargetType": ...,
}

parent.delete_account_assignment(**kwargs)
```

1. See [:material-code-braces: DeleteAccountAssignmentRequestRequestTypeDef](./type_defs.md#deleteaccountassignmentrequestrequesttypedef) 

### delete\_application

Deletes the association with the application.

Type annotations and code completion for `#!python session.create_client("sso-admin").delete_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/delete_application.html)

```python
# delete_application method definition

await def delete_application(
    self,
    *,
    ApplicationArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_application method usage example with argument unpacking

kwargs: DeleteApplicationRequestRequestTypeDef = {  # (1)
    "ApplicationArn": ...,
}

parent.delete_application(**kwargs)
```

1. See [:material-code-braces: DeleteApplicationRequestRequestTypeDef](./type_defs.md#deleteapplicationrequestrequesttypedef) 

### delete\_application\_access\_scope

Deletes an IAM Identity Center access scope from an application.

Type annotations and code completion for `#!python session.create_client("sso-admin").delete_application_access_scope` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/delete_application_access_scope.html)

```python
# delete_application_access_scope method definition

await def delete_application_access_scope(
    self,
    *,
    ApplicationArn: str,
    Scope: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_application_access_scope method usage example with argument unpacking

kwargs: DeleteApplicationAccessScopeRequestRequestTypeDef = {  # (1)
    "ApplicationArn": ...,
    "Scope": ...,
}

parent.delete_application_access_scope(**kwargs)
```

1. See [:material-code-braces: DeleteApplicationAccessScopeRequestRequestTypeDef](./type_defs.md#deleteapplicationaccessscoperequestrequesttypedef) 

### delete\_application\_assignment

Revoke application access to an application by deleting application assignments
for a user or group.

Type annotations and code completion for `#!python session.create_client("sso-admin").delete_application_assignment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/delete_application_assignment.html)

```python
# delete_application_assignment method definition

await def delete_application_assignment(
    self,
    *,
    ApplicationArn: str,
    PrincipalId: str,
    PrincipalType: PrincipalTypeType,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 


```python
# delete_application_assignment method usage example with argument unpacking

kwargs: DeleteApplicationAssignmentRequestRequestTypeDef = {  # (1)
    "ApplicationArn": ...,
    "PrincipalId": ...,
    "PrincipalType": ...,
}

parent.delete_application_assignment(**kwargs)
```

1. See [:material-code-braces: DeleteApplicationAssignmentRequestRequestTypeDef](./type_defs.md#deleteapplicationassignmentrequestrequesttypedef) 

### delete\_application\_authentication\_method

Deletes an authentication method from an application.

Type annotations and code completion for `#!python session.create_client("sso-admin").delete_application_authentication_method` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/delete_application_authentication_method.html)

```python
# delete_application_authentication_method method definition

await def delete_application_authentication_method(
    self,
    *,
    ApplicationArn: str,
    AuthenticationMethodType: AuthenticationMethodTypeType,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AuthenticationMethodTypeType](./literals.md#authenticationmethodtypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_application_authentication_method method usage example with argument unpacking

kwargs: DeleteApplicationAuthenticationMethodRequestRequestTypeDef = {  # (1)
    "ApplicationArn": ...,
    "AuthenticationMethodType": ...,
}

parent.delete_application_authentication_method(**kwargs)
```

1. See [:material-code-braces: DeleteApplicationAuthenticationMethodRequestRequestTypeDef](./type_defs.md#deleteapplicationauthenticationmethodrequestrequesttypedef) 

### delete\_application\_grant

Deletes a grant from an application.

Type annotations and code completion for `#!python session.create_client("sso-admin").delete_application_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/delete_application_grant.html)

```python
# delete_application_grant method definition

await def delete_application_grant(
    self,
    *,
    ApplicationArn: str,
    GrantType: GrantTypeType,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: GrantTypeType](./literals.md#granttypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_application_grant method usage example with argument unpacking

kwargs: DeleteApplicationGrantRequestRequestTypeDef = {  # (1)
    "ApplicationArn": ...,
    "GrantType": ...,
}

parent.delete_application_grant(**kwargs)
```

1. See [:material-code-braces: DeleteApplicationGrantRequestRequestTypeDef](./type_defs.md#deleteapplicationgrantrequestrequesttypedef) 

### delete\_inline\_policy\_from\_permission\_set

Deletes the inline policy from a specified permission set.

Type annotations and code completion for `#!python session.create_client("sso-admin").delete_inline_policy_from_permission_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/delete_inline_policy_from_permission_set.html)

```python
# delete_inline_policy_from_permission_set method definition

await def delete_inline_policy_from_permission_set(
    self,
    *,
    InstanceArn: str,
    PermissionSetArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_inline_policy_from_permission_set method usage example with argument unpacking

kwargs: DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
    "PermissionSetArn": ...,
}

parent.delete_inline_policy_from_permission_set(**kwargs)
```

1. See [:material-code-braces: DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef](./type_defs.md#deleteinlinepolicyfrompermissionsetrequestrequesttypedef) 

### delete\_instance

Deletes the instance of IAM Identity Center.

Type annotations and code completion for `#!python session.create_client("sso-admin").delete_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/delete_instance.html)

```python
# delete_instance method definition

await def delete_instance(
    self,
    *,
    InstanceArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_instance method usage example with argument unpacking

kwargs: DeleteInstanceRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
}

parent.delete_instance(**kwargs)
```

1. See [:material-code-braces: DeleteInstanceRequestRequestTypeDef](./type_defs.md#deleteinstancerequestrequesttypedef) 

### delete\_instance\_access\_control\_attribute\_configuration

Disables the attributes-based access control (ABAC) feature for the specified
IAM Identity Center instance and deletes all of the attribute mappings that
have been configured.

Type annotations and code completion for `#!python session.create_client("sso-admin").delete_instance_access_control_attribute_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/delete_instance_access_control_attribute_configuration.html)

```python
# delete_instance_access_control_attribute_configuration method definition

await def delete_instance_access_control_attribute_configuration(
    self,
    *,
    InstanceArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_instance_access_control_attribute_configuration method usage example with argument unpacking

kwargs: DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
}

parent.delete_instance_access_control_attribute_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef](./type_defs.md#deleteinstanceaccesscontrolattributeconfigurationrequestrequesttypedef) 

### delete\_permission\_set

Deletes the specified permission set.

Type annotations and code completion for `#!python session.create_client("sso-admin").delete_permission_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/delete_permission_set.html)

```python
# delete_permission_set method definition

await def delete_permission_set(
    self,
    *,
    InstanceArn: str,
    PermissionSetArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_permission_set method usage example with argument unpacking

kwargs: DeletePermissionSetRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
    "PermissionSetArn": ...,
}

parent.delete_permission_set(**kwargs)
```

1. See [:material-code-braces: DeletePermissionSetRequestRequestTypeDef](./type_defs.md#deletepermissionsetrequestrequesttypedef) 

### delete\_permissions\_boundary\_from\_permission\_set

Deletes the permissions boundary from a specified <a>PermissionSet</a>.

Type annotations and code completion for `#!python session.create_client("sso-admin").delete_permissions_boundary_from_permission_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/delete_permissions_boundary_from_permission_set.html)

```python
# delete_permissions_boundary_from_permission_set method definition

await def delete_permissions_boundary_from_permission_set(
    self,
    *,
    InstanceArn: str,
    PermissionSetArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_permissions_boundary_from_permission_set method usage example with argument unpacking

kwargs: DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
    "PermissionSetArn": ...,
}

parent.delete_permissions_boundary_from_permission_set(**kwargs)
```

1. See [:material-code-braces: DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef](./type_defs.md#deletepermissionsboundaryfrompermissionsetrequestrequesttypedef) 

### delete\_trusted\_token\_issuer

Deletes a trusted token issuer configuration from an instance of IAM Identity
Center.

Type annotations and code completion for `#!python session.create_client("sso-admin").delete_trusted_token_issuer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/delete_trusted_token_issuer.html)

```python
# delete_trusted_token_issuer method definition

await def delete_trusted_token_issuer(
    self,
    *,
    TrustedTokenIssuerArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_trusted_token_issuer method usage example with argument unpacking

kwargs: DeleteTrustedTokenIssuerRequestRequestTypeDef = {  # (1)
    "TrustedTokenIssuerArn": ...,
}

parent.delete_trusted_token_issuer(**kwargs)
```

1. See [:material-code-braces: DeleteTrustedTokenIssuerRequestRequestTypeDef](./type_defs.md#deletetrustedtokenissuerrequestrequesttypedef) 

### describe\_account\_assignment\_creation\_status

Describes the status of the assignment creation request.

Type annotations and code completion for `#!python session.create_client("sso-admin").describe_account_assignment_creation_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/describe_account_assignment_creation_status.html)

```python
# describe_account_assignment_creation_status method definition

await def describe_account_assignment_creation_status(
    self,
    *,
    AccountAssignmentCreationRequestId: str,
    InstanceArn: str,
) -> DescribeAccountAssignmentCreationStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAccountAssignmentCreationStatusResponseTypeDef](./type_defs.md#describeaccountassignmentcreationstatusresponsetypedef) 


```python
# describe_account_assignment_creation_status method usage example with argument unpacking

kwargs: DescribeAccountAssignmentCreationStatusRequestRequestTypeDef = {  # (1)
    "AccountAssignmentCreationRequestId": ...,
    "InstanceArn": ...,
}

parent.describe_account_assignment_creation_status(**kwargs)
```

1. See [:material-code-braces: DescribeAccountAssignmentCreationStatusRequestRequestTypeDef](./type_defs.md#describeaccountassignmentcreationstatusrequestrequesttypedef) 

### describe\_account\_assignment\_deletion\_status

Describes the status of the assignment deletion request.

Type annotations and code completion for `#!python session.create_client("sso-admin").describe_account_assignment_deletion_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/describe_account_assignment_deletion_status.html)

```python
# describe_account_assignment_deletion_status method definition

await def describe_account_assignment_deletion_status(
    self,
    *,
    AccountAssignmentDeletionRequestId: str,
    InstanceArn: str,
) -> DescribeAccountAssignmentDeletionStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAccountAssignmentDeletionStatusResponseTypeDef](./type_defs.md#describeaccountassignmentdeletionstatusresponsetypedef) 


```python
# describe_account_assignment_deletion_status method usage example with argument unpacking

kwargs: DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef = {  # (1)
    "AccountAssignmentDeletionRequestId": ...,
    "InstanceArn": ...,
}

parent.describe_account_assignment_deletion_status(**kwargs)
```

1. See [:material-code-braces: DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef](./type_defs.md#describeaccountassignmentdeletionstatusrequestrequesttypedef) 

### describe\_application

Retrieves the details of an application associated with an instance of IAM
Identity Center.

Type annotations and code completion for `#!python session.create_client("sso-admin").describe_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/describe_application.html)

```python
# describe_application method definition

await def describe_application(
    self,
    *,
    ApplicationArn: str,
) -> DescribeApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeApplicationResponseTypeDef](./type_defs.md#describeapplicationresponsetypedef) 


```python
# describe_application method usage example with argument unpacking

kwargs: DescribeApplicationRequestRequestTypeDef = {  # (1)
    "ApplicationArn": ...,
}

parent.describe_application(**kwargs)
```

1. See [:material-code-braces: DescribeApplicationRequestRequestTypeDef](./type_defs.md#describeapplicationrequestrequesttypedef) 

### describe\_application\_assignment

Retrieves a direct assignment of a user or group to an application.

Type annotations and code completion for `#!python session.create_client("sso-admin").describe_application_assignment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/describe_application_assignment.html)

```python
# describe_application_assignment method definition

await def describe_application_assignment(
    self,
    *,
    ApplicationArn: str,
    PrincipalId: str,
    PrincipalType: PrincipalTypeType,  # (1)
) -> DescribeApplicationAssignmentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-braces: DescribeApplicationAssignmentResponseTypeDef](./type_defs.md#describeapplicationassignmentresponsetypedef) 


```python
# describe_application_assignment method usage example with argument unpacking

kwargs: DescribeApplicationAssignmentRequestRequestTypeDef = {  # (1)
    "ApplicationArn": ...,
    "PrincipalId": ...,
    "PrincipalType": ...,
}

parent.describe_application_assignment(**kwargs)
```

1. See [:material-code-braces: DescribeApplicationAssignmentRequestRequestTypeDef](./type_defs.md#describeapplicationassignmentrequestrequesttypedef) 

### describe\_application\_provider

Retrieves details about a provider that can be used to connect an Amazon Web
Services managed application or customer managed application to IAM Identity
Center.

Type annotations and code completion for `#!python session.create_client("sso-admin").describe_application_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/describe_application_provider.html)

```python
# describe_application_provider method definition

await def describe_application_provider(
    self,
    *,
    ApplicationProviderArn: str,
) -> DescribeApplicationProviderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeApplicationProviderResponseTypeDef](./type_defs.md#describeapplicationproviderresponsetypedef) 


```python
# describe_application_provider method usage example with argument unpacking

kwargs: DescribeApplicationProviderRequestRequestTypeDef = {  # (1)
    "ApplicationProviderArn": ...,
}

parent.describe_application_provider(**kwargs)
```

1. See [:material-code-braces: DescribeApplicationProviderRequestRequestTypeDef](./type_defs.md#describeapplicationproviderrequestrequesttypedef) 

### describe\_instance

Returns the details of an instance of IAM Identity Center.

Type annotations and code completion for `#!python session.create_client("sso-admin").describe_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/describe_instance.html)

```python
# describe_instance method definition

await def describe_instance(
    self,
    *,
    InstanceArn: str,
) -> DescribeInstanceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeInstanceResponseTypeDef](./type_defs.md#describeinstanceresponsetypedef) 


```python
# describe_instance method usage example with argument unpacking

kwargs: DescribeInstanceRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
}

parent.describe_instance(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceRequestRequestTypeDef](./type_defs.md#describeinstancerequestrequesttypedef) 

### describe\_instance\_access\_control\_attribute\_configuration

Returns the list of IAM Identity Center identity store attributes that have
been configured to work with attributes-based access control (ABAC) for the
specified IAM Identity Center instance.

Type annotations and code completion for `#!python session.create_client("sso-admin").describe_instance_access_control_attribute_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/describe_instance_access_control_attribute_configuration.html)

```python
# describe_instance_access_control_attribute_configuration method definition

await def describe_instance_access_control_attribute_configuration(
    self,
    *,
    InstanceArn: str,
) -> DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef](./type_defs.md#describeinstanceaccesscontrolattributeconfigurationresponsetypedef) 


```python
# describe_instance_access_control_attribute_configuration method usage example with argument unpacking

kwargs: DescribeInstanceAccessControlAttributeConfigurationRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
}

parent.describe_instance_access_control_attribute_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceAccessControlAttributeConfigurationRequestRequestTypeDef](./type_defs.md#describeinstanceaccesscontrolattributeconfigurationrequestrequesttypedef) 

### describe\_permission\_set

Gets the details of the permission set.

Type annotations and code completion for `#!python session.create_client("sso-admin").describe_permission_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/describe_permission_set.html)

```python
# describe_permission_set method definition

await def describe_permission_set(
    self,
    *,
    InstanceArn: str,
    PermissionSetArn: str,
) -> DescribePermissionSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePermissionSetResponseTypeDef](./type_defs.md#describepermissionsetresponsetypedef) 


```python
# describe_permission_set method usage example with argument unpacking

kwargs: DescribePermissionSetRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
    "PermissionSetArn": ...,
}

parent.describe_permission_set(**kwargs)
```

1. See [:material-code-braces: DescribePermissionSetRequestRequestTypeDef](./type_defs.md#describepermissionsetrequestrequesttypedef) 

### describe\_permission\_set\_provisioning\_status

Describes the status for the given permission set provisioning request.

Type annotations and code completion for `#!python session.create_client("sso-admin").describe_permission_set_provisioning_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/describe_permission_set_provisioning_status.html)

```python
# describe_permission_set_provisioning_status method definition

await def describe_permission_set_provisioning_status(
    self,
    *,
    InstanceArn: str,
    ProvisionPermissionSetRequestId: str,
) -> DescribePermissionSetProvisioningStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePermissionSetProvisioningStatusResponseTypeDef](./type_defs.md#describepermissionsetprovisioningstatusresponsetypedef) 


```python
# describe_permission_set_provisioning_status method usage example with argument unpacking

kwargs: DescribePermissionSetProvisioningStatusRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
    "ProvisionPermissionSetRequestId": ...,
}

parent.describe_permission_set_provisioning_status(**kwargs)
```

1. See [:material-code-braces: DescribePermissionSetProvisioningStatusRequestRequestTypeDef](./type_defs.md#describepermissionsetprovisioningstatusrequestrequesttypedef) 

### describe\_trusted\_token\_issuer

Retrieves details about a trusted token issuer configuration stored in an
instance of IAM Identity Center.

Type annotations and code completion for `#!python session.create_client("sso-admin").describe_trusted_token_issuer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/describe_trusted_token_issuer.html)

```python
# describe_trusted_token_issuer method definition

await def describe_trusted_token_issuer(
    self,
    *,
    TrustedTokenIssuerArn: str,
) -> DescribeTrustedTokenIssuerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTrustedTokenIssuerResponseTypeDef](./type_defs.md#describetrustedtokenissuerresponsetypedef) 


```python
# describe_trusted_token_issuer method usage example with argument unpacking

kwargs: DescribeTrustedTokenIssuerRequestRequestTypeDef = {  # (1)
    "TrustedTokenIssuerArn": ...,
}

parent.describe_trusted_token_issuer(**kwargs)
```

1. See [:material-code-braces: DescribeTrustedTokenIssuerRequestRequestTypeDef](./type_defs.md#describetrustedtokenissuerrequestrequesttypedef) 

### detach\_customer\_managed\_policy\_reference\_from\_permission\_set

Detaches the specified customer managed policy from the specified
<a>PermissionSet</a>.

Type annotations and code completion for `#!python session.create_client("sso-admin").detach_customer_managed_policy_reference_from_permission_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/detach_customer_managed_policy_reference_from_permission_set.html)

```python
# detach_customer_managed_policy_reference_from_permission_set method definition

await def detach_customer_managed_policy_reference_from_permission_set(
    self,
    *,
    CustomerManagedPolicyReference: CustomerManagedPolicyReferenceTypeDef,  # (1)
    InstanceArn: str,
    PermissionSetArn: str,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: CustomerManagedPolicyReferenceTypeDef](./type_defs.md#customermanagedpolicyreferencetypedef) 


```python
# detach_customer_managed_policy_reference_from_permission_set method usage example with argument unpacking

kwargs: DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef = {  # (1)
    "CustomerManagedPolicyReference": ...,
    "InstanceArn": ...,
    "PermissionSetArn": ...,
}

parent.detach_customer_managed_policy_reference_from_permission_set(**kwargs)
```

1. See [:material-code-braces: DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef](./type_defs.md#detachcustomermanagedpolicyreferencefrompermissionsetrequestrequesttypedef) 

### detach\_managed\_policy\_from\_permission\_set

Detaches the attached Amazon Web Services managed policy ARN from the specified
permission set.

Type annotations and code completion for `#!python session.create_client("sso-admin").detach_managed_policy_from_permission_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/detach_managed_policy_from_permission_set.html)

```python
# detach_managed_policy_from_permission_set method definition

await def detach_managed_policy_from_permission_set(
    self,
    *,
    InstanceArn: str,
    ManagedPolicyArn: str,
    PermissionSetArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# detach_managed_policy_from_permission_set method usage example with argument unpacking

kwargs: DetachManagedPolicyFromPermissionSetRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
    "ManagedPolicyArn": ...,
    "PermissionSetArn": ...,
}

parent.detach_managed_policy_from_permission_set(**kwargs)
```

1. See [:material-code-braces: DetachManagedPolicyFromPermissionSetRequestRequestTypeDef](./type_defs.md#detachmanagedpolicyfrompermissionsetrequestrequesttypedef) 

### get\_application\_access\_scope

Retrieves the authorized targets for an IAM Identity Center access scope for an
application.

Type annotations and code completion for `#!python session.create_client("sso-admin").get_application_access_scope` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/get_application_access_scope.html)

```python
# get_application_access_scope method definition

await def get_application_access_scope(
    self,
    *,
    ApplicationArn: str,
    Scope: str,
) -> GetApplicationAccessScopeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetApplicationAccessScopeResponseTypeDef](./type_defs.md#getapplicationaccessscoperesponsetypedef) 


```python
# get_application_access_scope method usage example with argument unpacking

kwargs: GetApplicationAccessScopeRequestRequestTypeDef = {  # (1)
    "ApplicationArn": ...,
    "Scope": ...,
}

parent.get_application_access_scope(**kwargs)
```

1. See [:material-code-braces: GetApplicationAccessScopeRequestRequestTypeDef](./type_defs.md#getapplicationaccessscoperequestrequesttypedef) 

### get\_application\_assignment\_configuration

Retrieves the configuration of <a>PutApplicationAssignmentConfiguration</a>.

Type annotations and code completion for `#!python session.create_client("sso-admin").get_application_assignment_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/get_application_assignment_configuration.html)

```python
# get_application_assignment_configuration method definition

await def get_application_assignment_configuration(
    self,
    *,
    ApplicationArn: str,
) -> GetApplicationAssignmentConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetApplicationAssignmentConfigurationResponseTypeDef](./type_defs.md#getapplicationassignmentconfigurationresponsetypedef) 


```python
# get_application_assignment_configuration method usage example with argument unpacking

kwargs: GetApplicationAssignmentConfigurationRequestRequestTypeDef = {  # (1)
    "ApplicationArn": ...,
}

parent.get_application_assignment_configuration(**kwargs)
```

1. See [:material-code-braces: GetApplicationAssignmentConfigurationRequestRequestTypeDef](./type_defs.md#getapplicationassignmentconfigurationrequestrequesttypedef) 

### get\_application\_authentication\_method

Retrieves details about an authentication method used by an application.

Type annotations and code completion for `#!python session.create_client("sso-admin").get_application_authentication_method` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/get_application_authentication_method.html)

```python
# get_application_authentication_method method definition

await def get_application_authentication_method(
    self,
    *,
    ApplicationArn: str,
    AuthenticationMethodType: AuthenticationMethodTypeType,  # (1)
) -> GetApplicationAuthenticationMethodResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AuthenticationMethodTypeType](./literals.md#authenticationmethodtypetype) 
2. See [:material-code-braces: GetApplicationAuthenticationMethodResponseTypeDef](./type_defs.md#getapplicationauthenticationmethodresponsetypedef) 


```python
# get_application_authentication_method method usage example with argument unpacking

kwargs: GetApplicationAuthenticationMethodRequestRequestTypeDef = {  # (1)
    "ApplicationArn": ...,
    "AuthenticationMethodType": ...,
}

parent.get_application_authentication_method(**kwargs)
```

1. See [:material-code-braces: GetApplicationAuthenticationMethodRequestRequestTypeDef](./type_defs.md#getapplicationauthenticationmethodrequestrequesttypedef) 

### get\_application\_grant

Retrieves details about an application grant.

Type annotations and code completion for `#!python session.create_client("sso-admin").get_application_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/get_application_grant.html)

```python
# get_application_grant method definition

await def get_application_grant(
    self,
    *,
    ApplicationArn: str,
    GrantType: GrantTypeType,  # (1)
) -> GetApplicationGrantResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: GrantTypeType](./literals.md#granttypetype) 
2. See [:material-code-braces: GetApplicationGrantResponseTypeDef](./type_defs.md#getapplicationgrantresponsetypedef) 


```python
# get_application_grant method usage example with argument unpacking

kwargs: GetApplicationGrantRequestRequestTypeDef = {  # (1)
    "ApplicationArn": ...,
    "GrantType": ...,
}

parent.get_application_grant(**kwargs)
```

1. See [:material-code-braces: GetApplicationGrantRequestRequestTypeDef](./type_defs.md#getapplicationgrantrequestrequesttypedef) 

### get\_inline\_policy\_for\_permission\_set

Obtains the inline policy assigned to the permission set.

Type annotations and code completion for `#!python session.create_client("sso-admin").get_inline_policy_for_permission_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/get_inline_policy_for_permission_set.html)

```python
# get_inline_policy_for_permission_set method definition

await def get_inline_policy_for_permission_set(
    self,
    *,
    InstanceArn: str,
    PermissionSetArn: str,
) -> GetInlinePolicyForPermissionSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInlinePolicyForPermissionSetResponseTypeDef](./type_defs.md#getinlinepolicyforpermissionsetresponsetypedef) 


```python
# get_inline_policy_for_permission_set method usage example with argument unpacking

kwargs: GetInlinePolicyForPermissionSetRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
    "PermissionSetArn": ...,
}

parent.get_inline_policy_for_permission_set(**kwargs)
```

1. See [:material-code-braces: GetInlinePolicyForPermissionSetRequestRequestTypeDef](./type_defs.md#getinlinepolicyforpermissionsetrequestrequesttypedef) 

### get\_permissions\_boundary\_for\_permission\_set

Obtains the permissions boundary for a specified <a>PermissionSet</a>.

Type annotations and code completion for `#!python session.create_client("sso-admin").get_permissions_boundary_for_permission_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/get_permissions_boundary_for_permission_set.html)

```python
# get_permissions_boundary_for_permission_set method definition

await def get_permissions_boundary_for_permission_set(
    self,
    *,
    InstanceArn: str,
    PermissionSetArn: str,
) -> GetPermissionsBoundaryForPermissionSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPermissionsBoundaryForPermissionSetResponseTypeDef](./type_defs.md#getpermissionsboundaryforpermissionsetresponsetypedef) 


```python
# get_permissions_boundary_for_permission_set method usage example with argument unpacking

kwargs: GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
    "PermissionSetArn": ...,
}

parent.get_permissions_boundary_for_permission_set(**kwargs)
```

1. See [:material-code-braces: GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef](./type_defs.md#getpermissionsboundaryforpermissionsetrequestrequesttypedef) 

### list\_account\_assignment\_creation\_status

Lists the status of the Amazon Web Services account assignment creation
requests for a specified IAM Identity Center instance.

Type annotations and code completion for `#!python session.create_client("sso-admin").list_account_assignment_creation_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/list_account_assignment_creation_status.html)

```python
# list_account_assignment_creation_status method definition

await def list_account_assignment_creation_status(
    self,
    *,
    InstanceArn: str,
    Filter: OperationStatusFilterTypeDef = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAccountAssignmentCreationStatusResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: OperationStatusFilterTypeDef](./type_defs.md#operationstatusfiltertypedef) 
2. See [:material-code-braces: ListAccountAssignmentCreationStatusResponseTypeDef](./type_defs.md#listaccountassignmentcreationstatusresponsetypedef) 


```python
# list_account_assignment_creation_status method usage example with argument unpacking

kwargs: ListAccountAssignmentCreationStatusRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
}

parent.list_account_assignment_creation_status(**kwargs)
```

1. See [:material-code-braces: ListAccountAssignmentCreationStatusRequestRequestTypeDef](./type_defs.md#listaccountassignmentcreationstatusrequestrequesttypedef) 

### list\_account\_assignment\_deletion\_status

Lists the status of the Amazon Web Services account assignment deletion
requests for a specified IAM Identity Center instance.

Type annotations and code completion for `#!python session.create_client("sso-admin").list_account_assignment_deletion_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/list_account_assignment_deletion_status.html)

```python
# list_account_assignment_deletion_status method definition

await def list_account_assignment_deletion_status(
    self,
    *,
    InstanceArn: str,
    Filter: OperationStatusFilterTypeDef = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAccountAssignmentDeletionStatusResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: OperationStatusFilterTypeDef](./type_defs.md#operationstatusfiltertypedef) 
2. See [:material-code-braces: ListAccountAssignmentDeletionStatusResponseTypeDef](./type_defs.md#listaccountassignmentdeletionstatusresponsetypedef) 


```python
# list_account_assignment_deletion_status method usage example with argument unpacking

kwargs: ListAccountAssignmentDeletionStatusRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
}

parent.list_account_assignment_deletion_status(**kwargs)
```

1. See [:material-code-braces: ListAccountAssignmentDeletionStatusRequestRequestTypeDef](./type_defs.md#listaccountassignmentdeletionstatusrequestrequesttypedef) 

### list\_account\_assignments

Lists the assignee of the specified Amazon Web Services account with the
specified permission set.

Type annotations and code completion for `#!python session.create_client("sso-admin").list_account_assignments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/list_account_assignments.html)

```python
# list_account_assignments method definition

await def list_account_assignments(
    self,
    *,
    AccountId: str,
    InstanceArn: str,
    PermissionSetArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAccountAssignmentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAccountAssignmentsResponseTypeDef](./type_defs.md#listaccountassignmentsresponsetypedef) 


```python
# list_account_assignments method usage example with argument unpacking

kwargs: ListAccountAssignmentsRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "InstanceArn": ...,
    "PermissionSetArn": ...,
}

parent.list_account_assignments(**kwargs)
```

1. See [:material-code-braces: ListAccountAssignmentsRequestRequestTypeDef](./type_defs.md#listaccountassignmentsrequestrequesttypedef) 

### list\_account\_assignments\_for\_principal

Retrieves a list of the IAM Identity Center associated Amazon Web Services
accounts that the principal has access to.

Type annotations and code completion for `#!python session.create_client("sso-admin").list_account_assignments_for_principal` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/list_account_assignments_for_principal.html)

```python
# list_account_assignments_for_principal method definition

await def list_account_assignments_for_principal(
    self,
    *,
    InstanceArn: str,
    PrincipalId: str,
    PrincipalType: PrincipalTypeType,  # (1)
    Filter: ListAccountAssignmentsFilterTypeDef = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAccountAssignmentsForPrincipalResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-braces: ListAccountAssignmentsFilterTypeDef](./type_defs.md#listaccountassignmentsfiltertypedef) 
3. See [:material-code-braces: ListAccountAssignmentsForPrincipalResponseTypeDef](./type_defs.md#listaccountassignmentsforprincipalresponsetypedef) 


```python
# list_account_assignments_for_principal method usage example with argument unpacking

kwargs: ListAccountAssignmentsForPrincipalRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
    "PrincipalId": ...,
    "PrincipalType": ...,
}

parent.list_account_assignments_for_principal(**kwargs)
```

1. See [:material-code-braces: ListAccountAssignmentsForPrincipalRequestRequestTypeDef](./type_defs.md#listaccountassignmentsforprincipalrequestrequesttypedef) 

### list\_accounts\_for\_provisioned\_permission\_set

Lists all the Amazon Web Services accounts where the specified permission set
is provisioned.

Type annotations and code completion for `#!python session.create_client("sso-admin").list_accounts_for_provisioned_permission_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/list_accounts_for_provisioned_permission_set.html)

```python
# list_accounts_for_provisioned_permission_set method definition

await def list_accounts_for_provisioned_permission_set(
    self,
    *,
    InstanceArn: str,
    PermissionSetArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    ProvisioningStatus: ProvisioningStatusType = ...,  # (1)
) -> ListAccountsForProvisionedPermissionSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ProvisioningStatusType](./literals.md#provisioningstatustype) 
2. See [:material-code-braces: ListAccountsForProvisionedPermissionSetResponseTypeDef](./type_defs.md#listaccountsforprovisionedpermissionsetresponsetypedef) 


```python
# list_accounts_for_provisioned_permission_set method usage example with argument unpacking

kwargs: ListAccountsForProvisionedPermissionSetRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
    "PermissionSetArn": ...,
}

parent.list_accounts_for_provisioned_permission_set(**kwargs)
```

1. See [:material-code-braces: ListAccountsForProvisionedPermissionSetRequestRequestTypeDef](./type_defs.md#listaccountsforprovisionedpermissionsetrequestrequesttypedef) 

### list\_application\_access\_scopes

Lists the access scopes and authorized targets associated with an application.

Type annotations and code completion for `#!python session.create_client("sso-admin").list_application_access_scopes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/list_application_access_scopes.html)

```python
# list_application_access_scopes method definition

await def list_application_access_scopes(
    self,
    *,
    ApplicationArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListApplicationAccessScopesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListApplicationAccessScopesResponseTypeDef](./type_defs.md#listapplicationaccessscopesresponsetypedef) 


```python
# list_application_access_scopes method usage example with argument unpacking

kwargs: ListApplicationAccessScopesRequestRequestTypeDef = {  # (1)
    "ApplicationArn": ...,
}

parent.list_application_access_scopes(**kwargs)
```

1. See [:material-code-braces: ListApplicationAccessScopesRequestRequestTypeDef](./type_defs.md#listapplicationaccessscopesrequestrequesttypedef) 

### list\_application\_assignments

Lists Amazon Web Services account users that are assigned to an application.

Type annotations and code completion for `#!python session.create_client("sso-admin").list_application_assignments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/list_application_assignments.html)

```python
# list_application_assignments method definition

await def list_application_assignments(
    self,
    *,
    ApplicationArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListApplicationAssignmentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListApplicationAssignmentsResponseTypeDef](./type_defs.md#listapplicationassignmentsresponsetypedef) 


```python
# list_application_assignments method usage example with argument unpacking

kwargs: ListApplicationAssignmentsRequestRequestTypeDef = {  # (1)
    "ApplicationArn": ...,
}

parent.list_application_assignments(**kwargs)
```

1. See [:material-code-braces: ListApplicationAssignmentsRequestRequestTypeDef](./type_defs.md#listapplicationassignmentsrequestrequesttypedef) 

### list\_application\_assignments\_for\_principal

Lists the applications to which a specified principal is assigned.

Type annotations and code completion for `#!python session.create_client("sso-admin").list_application_assignments_for_principal` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/list_application_assignments_for_principal.html)

```python
# list_application_assignments_for_principal method definition

await def list_application_assignments_for_principal(
    self,
    *,
    InstanceArn: str,
    PrincipalId: str,
    PrincipalType: PrincipalTypeType,  # (1)
    Filter: ListApplicationAssignmentsFilterTypeDef = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListApplicationAssignmentsForPrincipalResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-braces: ListApplicationAssignmentsFilterTypeDef](./type_defs.md#listapplicationassignmentsfiltertypedef) 
3. See [:material-code-braces: ListApplicationAssignmentsForPrincipalResponseTypeDef](./type_defs.md#listapplicationassignmentsforprincipalresponsetypedef) 


```python
# list_application_assignments_for_principal method usage example with argument unpacking

kwargs: ListApplicationAssignmentsForPrincipalRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
    "PrincipalId": ...,
    "PrincipalType": ...,
}

parent.list_application_assignments_for_principal(**kwargs)
```

1. See [:material-code-braces: ListApplicationAssignmentsForPrincipalRequestRequestTypeDef](./type_defs.md#listapplicationassignmentsforprincipalrequestrequesttypedef) 

### list\_application\_authentication\_methods

Lists all of the authentication methods supported by the specified application.

Type annotations and code completion for `#!python session.create_client("sso-admin").list_application_authentication_methods` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/list_application_authentication_methods.html)

```python
# list_application_authentication_methods method definition

await def list_application_authentication_methods(
    self,
    *,
    ApplicationArn: str,
    NextToken: str = ...,
) -> ListApplicationAuthenticationMethodsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListApplicationAuthenticationMethodsResponseTypeDef](./type_defs.md#listapplicationauthenticationmethodsresponsetypedef) 


```python
# list_application_authentication_methods method usage example with argument unpacking

kwargs: ListApplicationAuthenticationMethodsRequestRequestTypeDef = {  # (1)
    "ApplicationArn": ...,
}

parent.list_application_authentication_methods(**kwargs)
```

1. See [:material-code-braces: ListApplicationAuthenticationMethodsRequestRequestTypeDef](./type_defs.md#listapplicationauthenticationmethodsrequestrequesttypedef) 

### list\_application\_grants

List the grants associated with an application.

Type annotations and code completion for `#!python session.create_client("sso-admin").list_application_grants` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/list_application_grants.html)

```python
# list_application_grants method definition

await def list_application_grants(
    self,
    *,
    ApplicationArn: str,
    NextToken: str = ...,
) -> ListApplicationGrantsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListApplicationGrantsResponseTypeDef](./type_defs.md#listapplicationgrantsresponsetypedef) 


```python
# list_application_grants method usage example with argument unpacking

kwargs: ListApplicationGrantsRequestRequestTypeDef = {  # (1)
    "ApplicationArn": ...,
}

parent.list_application_grants(**kwargs)
```

1. See [:material-code-braces: ListApplicationGrantsRequestRequestTypeDef](./type_defs.md#listapplicationgrantsrequestrequesttypedef) 

### list\_application\_providers

Lists the application providers configured in the IAM Identity Center identity
store.

Type annotations and code completion for `#!python session.create_client("sso-admin").list_application_providers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/list_application_providers.html)

```python
# list_application_providers method definition

await def list_application_providers(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListApplicationProvidersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListApplicationProvidersResponseTypeDef](./type_defs.md#listapplicationprovidersresponsetypedef) 


```python
# list_application_providers method usage example with argument unpacking

kwargs: ListApplicationProvidersRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_application_providers(**kwargs)
```

1. See [:material-code-braces: ListApplicationProvidersRequestRequestTypeDef](./type_defs.md#listapplicationprovidersrequestrequesttypedef) 

### list\_applications

Lists all applications associated with the instance of IAM Identity Center.

Type annotations and code completion for `#!python session.create_client("sso-admin").list_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/list_applications.html)

```python
# list_applications method definition

await def list_applications(
    self,
    *,
    InstanceArn: str,
    Filter: ListApplicationsFilterTypeDef = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListApplicationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListApplicationsFilterTypeDef](./type_defs.md#listapplicationsfiltertypedef) 
2. See [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


```python
# list_applications method usage example with argument unpacking

kwargs: ListApplicationsRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
}

parent.list_applications(**kwargs)
```

1. See [:material-code-braces: ListApplicationsRequestRequestTypeDef](./type_defs.md#listapplicationsrequestrequesttypedef) 

### list\_customer\_managed\_policy\_references\_in\_permission\_set

Lists all customer managed policies attached to a specified
<a>PermissionSet</a>.

Type annotations and code completion for `#!python session.create_client("sso-admin").list_customer_managed_policy_references_in_permission_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/list_customer_managed_policy_references_in_permission_set.html)

```python
# list_customer_managed_policy_references_in_permission_set method definition

await def list_customer_managed_policy_references_in_permission_set(
    self,
    *,
    InstanceArn: str,
    PermissionSetArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef](./type_defs.md#listcustomermanagedpolicyreferencesinpermissionsetresponsetypedef) 


```python
# list_customer_managed_policy_references_in_permission_set method usage example with argument unpacking

kwargs: ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
    "PermissionSetArn": ...,
}

parent.list_customer_managed_policy_references_in_permission_set(**kwargs)
```

1. See [:material-code-braces: ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef](./type_defs.md#listcustomermanagedpolicyreferencesinpermissionsetrequestrequesttypedef) 

### list\_instances

Lists the details of the organization and account instances of IAM Identity
Center that were created in or visible to the account calling this API.

Type annotations and code completion for `#!python session.create_client("sso-admin").list_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/list_instances.html)

```python
# list_instances method definition

await def list_instances(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListInstancesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListInstancesResponseTypeDef](./type_defs.md#listinstancesresponsetypedef) 


```python
# list_instances method usage example with argument unpacking

kwargs: ListInstancesRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_instances(**kwargs)
```

1. See [:material-code-braces: ListInstancesRequestRequestTypeDef](./type_defs.md#listinstancesrequestrequesttypedef) 

### list\_managed\_policies\_in\_permission\_set

Lists the Amazon Web Services managed policy that is attached to a specified
permission set.

Type annotations and code completion for `#!python session.create_client("sso-admin").list_managed_policies_in_permission_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/list_managed_policies_in_permission_set.html)

```python
# list_managed_policies_in_permission_set method definition

await def list_managed_policies_in_permission_set(
    self,
    *,
    InstanceArn: str,
    PermissionSetArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListManagedPoliciesInPermissionSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListManagedPoliciesInPermissionSetResponseTypeDef](./type_defs.md#listmanagedpoliciesinpermissionsetresponsetypedef) 


```python
# list_managed_policies_in_permission_set method usage example with argument unpacking

kwargs: ListManagedPoliciesInPermissionSetRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
    "PermissionSetArn": ...,
}

parent.list_managed_policies_in_permission_set(**kwargs)
```

1. See [:material-code-braces: ListManagedPoliciesInPermissionSetRequestRequestTypeDef](./type_defs.md#listmanagedpoliciesinpermissionsetrequestrequesttypedef) 

### list\_permission\_set\_provisioning\_status

Lists the status of the permission set provisioning requests for a specified
IAM Identity Center instance.

Type annotations and code completion for `#!python session.create_client("sso-admin").list_permission_set_provisioning_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/list_permission_set_provisioning_status.html)

```python
# list_permission_set_provisioning_status method definition

await def list_permission_set_provisioning_status(
    self,
    *,
    InstanceArn: str,
    Filter: OperationStatusFilterTypeDef = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListPermissionSetProvisioningStatusResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: OperationStatusFilterTypeDef](./type_defs.md#operationstatusfiltertypedef) 
2. See [:material-code-braces: ListPermissionSetProvisioningStatusResponseTypeDef](./type_defs.md#listpermissionsetprovisioningstatusresponsetypedef) 


```python
# list_permission_set_provisioning_status method usage example with argument unpacking

kwargs: ListPermissionSetProvisioningStatusRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
}

parent.list_permission_set_provisioning_status(**kwargs)
```

1. See [:material-code-braces: ListPermissionSetProvisioningStatusRequestRequestTypeDef](./type_defs.md#listpermissionsetprovisioningstatusrequestrequesttypedef) 

### list\_permission\_sets

Lists the <a>PermissionSet</a>s in an IAM Identity Center instance.

Type annotations and code completion for `#!python session.create_client("sso-admin").list_permission_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/list_permission_sets.html)

```python
# list_permission_sets method definition

await def list_permission_sets(
    self,
    *,
    InstanceArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListPermissionSetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPermissionSetsResponseTypeDef](./type_defs.md#listpermissionsetsresponsetypedef) 


```python
# list_permission_sets method usage example with argument unpacking

kwargs: ListPermissionSetsRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
}

parent.list_permission_sets(**kwargs)
```

1. See [:material-code-braces: ListPermissionSetsRequestRequestTypeDef](./type_defs.md#listpermissionsetsrequestrequesttypedef) 

### list\_permission\_sets\_provisioned\_to\_account

Lists all the permission sets that are provisioned to a specified Amazon Web
Services account.

Type annotations and code completion for `#!python session.create_client("sso-admin").list_permission_sets_provisioned_to_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/list_permission_sets_provisioned_to_account.html)

```python
# list_permission_sets_provisioned_to_account method definition

await def list_permission_sets_provisioned_to_account(
    self,
    *,
    AccountId: str,
    InstanceArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    ProvisioningStatus: ProvisioningStatusType = ...,  # (1)
) -> ListPermissionSetsProvisionedToAccountResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ProvisioningStatusType](./literals.md#provisioningstatustype) 
2. See [:material-code-braces: ListPermissionSetsProvisionedToAccountResponseTypeDef](./type_defs.md#listpermissionsetsprovisionedtoaccountresponsetypedef) 


```python
# list_permission_sets_provisioned_to_account method usage example with argument unpacking

kwargs: ListPermissionSetsProvisionedToAccountRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "InstanceArn": ...,
}

parent.list_permission_sets_provisioned_to_account(**kwargs)
```

1. See [:material-code-braces: ListPermissionSetsProvisionedToAccountRequestRequestTypeDef](./type_defs.md#listpermissionsetsprovisionedtoaccountrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags that are attached to a specified resource.

Type annotations and code completion for `#!python session.create_client("sso-admin").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
    InstanceArn: str = ...,
    NextToken: str = ...,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_trusted\_token\_issuers

Lists all the trusted token issuers configured in an instance of IAM Identity
Center.

Type annotations and code completion for `#!python session.create_client("sso-admin").list_trusted_token_issuers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/list_trusted_token_issuers.html)

```python
# list_trusted_token_issuers method definition

await def list_trusted_token_issuers(
    self,
    *,
    InstanceArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTrustedTokenIssuersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTrustedTokenIssuersResponseTypeDef](./type_defs.md#listtrustedtokenissuersresponsetypedef) 


```python
# list_trusted_token_issuers method usage example with argument unpacking

kwargs: ListTrustedTokenIssuersRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
}

parent.list_trusted_token_issuers(**kwargs)
```

1. See [:material-code-braces: ListTrustedTokenIssuersRequestRequestTypeDef](./type_defs.md#listtrustedtokenissuersrequestrequesttypedef) 

### provision\_permission\_set

The process by which a specified permission set is provisioned to the specified
target.

Type annotations and code completion for `#!python session.create_client("sso-admin").provision_permission_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/provision_permission_set.html)

```python
# provision_permission_set method definition

await def provision_permission_set(
    self,
    *,
    InstanceArn: str,
    PermissionSetArn: str,
    TargetType: ProvisionTargetTypeType,  # (1)
    TargetId: str = ...,
) -> ProvisionPermissionSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ProvisionTargetTypeType](./literals.md#provisiontargettypetype) 
2. See [:material-code-braces: ProvisionPermissionSetResponseTypeDef](./type_defs.md#provisionpermissionsetresponsetypedef) 


```python
# provision_permission_set method usage example with argument unpacking

kwargs: ProvisionPermissionSetRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
    "PermissionSetArn": ...,
    "TargetType": ...,
}

parent.provision_permission_set(**kwargs)
```

1. See [:material-code-braces: ProvisionPermissionSetRequestRequestTypeDef](./type_defs.md#provisionpermissionsetrequestrequesttypedef) 

### put\_application\_access\_scope

Adds or updates the list of authorized targets for an IAM Identity Center
access scope for an application.

Type annotations and code completion for `#!python session.create_client("sso-admin").put_application_access_scope` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/put_application_access_scope.html)

```python
# put_application_access_scope method definition

await def put_application_access_scope(
    self,
    *,
    ApplicationArn: str,
    Scope: str,
    AuthorizedTargets: Sequence[str] = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_application_access_scope method usage example with argument unpacking

kwargs: PutApplicationAccessScopeRequestRequestTypeDef = {  # (1)
    "ApplicationArn": ...,
    "Scope": ...,
}

parent.put_application_access_scope(**kwargs)
```

1. See [:material-code-braces: PutApplicationAccessScopeRequestRequestTypeDef](./type_defs.md#putapplicationaccessscoperequestrequesttypedef) 

### put\_application\_assignment\_configuration

Configure how users gain access to an application.

Type annotations and code completion for `#!python session.create_client("sso-admin").put_application_assignment_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/put_application_assignment_configuration.html)

```python
# put_application_assignment_configuration method definition

await def put_application_assignment_configuration(
    self,
    *,
    ApplicationArn: str,
    AssignmentRequired: bool,
) -> Dict[str, Any]:
    ...
```



```python
# put_application_assignment_configuration method usage example with argument unpacking

kwargs: PutApplicationAssignmentConfigurationRequestRequestTypeDef = {  # (1)
    "ApplicationArn": ...,
    "AssignmentRequired": ...,
}

parent.put_application_assignment_configuration(**kwargs)
```

1. See [:material-code-braces: PutApplicationAssignmentConfigurationRequestRequestTypeDef](./type_defs.md#putapplicationassignmentconfigurationrequestrequesttypedef) 

### put\_application\_authentication\_method

Adds or updates an authentication method for an application.

Type annotations and code completion for `#!python session.create_client("sso-admin").put_application_authentication_method` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/put_application_authentication_method.html)

```python
# put_application_authentication_method method definition

await def put_application_authentication_method(
    self,
    *,
    ApplicationArn: str,
    AuthenticationMethod: AuthenticationMethodTypeDef,  # (1)
    AuthenticationMethodType: AuthenticationMethodTypeType,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AuthenticationMethodTypeDef](./type_defs.md#authenticationmethodtypedef) 
2. See [:material-code-brackets: AuthenticationMethodTypeType](./literals.md#authenticationmethodtypetype) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_application_authentication_method method usage example with argument unpacking

kwargs: PutApplicationAuthenticationMethodRequestRequestTypeDef = {  # (1)
    "ApplicationArn": ...,
    "AuthenticationMethod": ...,
    "AuthenticationMethodType": ...,
}

parent.put_application_authentication_method(**kwargs)
```

1. See [:material-code-braces: PutApplicationAuthenticationMethodRequestRequestTypeDef](./type_defs.md#putapplicationauthenticationmethodrequestrequesttypedef) 

### put\_application\_grant

Adds a grant to an application.

Type annotations and code completion for `#!python session.create_client("sso-admin").put_application_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/put_application_grant.html)

```python
# put_application_grant method definition

await def put_application_grant(
    self,
    *,
    ApplicationArn: str,
    Grant: GrantTypeDef,  # (1)
    GrantType: GrantTypeType,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: GrantTypeDef](./type_defs.md#granttypedef) 
2. See [:material-code-brackets: GrantTypeType](./literals.md#granttypetype) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_application_grant method usage example with argument unpacking

kwargs: PutApplicationGrantRequestRequestTypeDef = {  # (1)
    "ApplicationArn": ...,
    "Grant": ...,
    "GrantType": ...,
}

parent.put_application_grant(**kwargs)
```

1. See [:material-code-braces: PutApplicationGrantRequestRequestTypeDef](./type_defs.md#putapplicationgrantrequestrequesttypedef) 

### put\_inline\_policy\_to\_permission\_set

Attaches an inline policy to a permission set.

Type annotations and code completion for `#!python session.create_client("sso-admin").put_inline_policy_to_permission_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/put_inline_policy_to_permission_set.html)

```python
# put_inline_policy_to_permission_set method definition

await def put_inline_policy_to_permission_set(
    self,
    *,
    InlinePolicy: str,
    InstanceArn: str,
    PermissionSetArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# put_inline_policy_to_permission_set method usage example with argument unpacking

kwargs: PutInlinePolicyToPermissionSetRequestRequestTypeDef = {  # (1)
    "InlinePolicy": ...,
    "InstanceArn": ...,
    "PermissionSetArn": ...,
}

parent.put_inline_policy_to_permission_set(**kwargs)
```

1. See [:material-code-braces: PutInlinePolicyToPermissionSetRequestRequestTypeDef](./type_defs.md#putinlinepolicytopermissionsetrequestrequesttypedef) 

### put\_permissions\_boundary\_to\_permission\_set

Attaches an Amazon Web Services managed or customer managed policy to the
specified <a>PermissionSet</a> as a permissions boundary.

Type annotations and code completion for `#!python session.create_client("sso-admin").put_permissions_boundary_to_permission_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/put_permissions_boundary_to_permission_set.html)

```python
# put_permissions_boundary_to_permission_set method definition

await def put_permissions_boundary_to_permission_set(
    self,
    *,
    InstanceArn: str,
    PermissionSetArn: str,
    PermissionsBoundary: PermissionsBoundaryTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: PermissionsBoundaryTypeDef](./type_defs.md#permissionsboundarytypedef) 


```python
# put_permissions_boundary_to_permission_set method usage example with argument unpacking

kwargs: PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
    "PermissionSetArn": ...,
    "PermissionsBoundary": ...,
}

parent.put_permissions_boundary_to_permission_set(**kwargs)
```

1. See [:material-code-braces: PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef](./type_defs.md#putpermissionsboundarytopermissionsetrequestrequesttypedef) 

### tag\_resource

Associates a set of tags with a specified resource.

Type annotations and code completion for `#!python session.create_client("sso-admin").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
    InstanceArn: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Disassociates a set of tags from a specified resource.

Type annotations and code completion for `#!python session.create_client("sso-admin").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
    InstanceArn: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_application

Updates application properties.

Type annotations and code completion for `#!python session.create_client("sso-admin").update_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/update_application.html)

```python
# update_application method definition

await def update_application(
    self,
    *,
    ApplicationArn: str,
    Description: str = ...,
    Name: str = ...,
    PortalOptions: UpdateApplicationPortalOptionsTypeDef = ...,  # (1)
    Status: ApplicationStatusType = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: UpdateApplicationPortalOptionsTypeDef](./type_defs.md#updateapplicationportaloptionstypedef) 
2. See [:material-code-brackets: ApplicationStatusType](./literals.md#applicationstatustype) 


```python
# update_application method usage example with argument unpacking

kwargs: UpdateApplicationRequestRequestTypeDef = {  # (1)
    "ApplicationArn": ...,
}

parent.update_application(**kwargs)
```

1. See [:material-code-braces: UpdateApplicationRequestRequestTypeDef](./type_defs.md#updateapplicationrequestrequesttypedef) 

### update\_instance

Update the details for the instance of IAM Identity Center that is owned by the
Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("sso-admin").update_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/update_instance.html)

```python
# update_instance method definition

await def update_instance(
    self,
    *,
    InstanceArn: str,
    Name: str,
) -> Dict[str, Any]:
    ...
```



```python
# update_instance method usage example with argument unpacking

kwargs: UpdateInstanceRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
    "Name": ...,
}

parent.update_instance(**kwargs)
```

1. See [:material-code-braces: UpdateInstanceRequestRequestTypeDef](./type_defs.md#updateinstancerequestrequesttypedef) 

### update\_instance\_access\_control\_attribute\_configuration

Updates the IAM Identity Center identity store attributes that you can use with
the IAM Identity Center instance for attributes-based access control (ABAC).

Type annotations and code completion for `#!python session.create_client("sso-admin").update_instance_access_control_attribute_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/update_instance_access_control_attribute_configuration.html)

```python
# update_instance_access_control_attribute_configuration method definition

await def update_instance_access_control_attribute_configuration(
    self,
    *,
    InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationTypeDef,  # (1)
    InstanceArn: str,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: InstanceAccessControlAttributeConfigurationTypeDef](./type_defs.md#instanceaccesscontrolattributeconfigurationtypedef) 


```python
# update_instance_access_control_attribute_configuration method usage example with argument unpacking

kwargs: UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef = {  # (1)
    "InstanceAccessControlAttributeConfiguration": ...,
    "InstanceArn": ...,
}

parent.update_instance_access_control_attribute_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef](./type_defs.md#updateinstanceaccesscontrolattributeconfigurationrequestrequesttypedef) 

### update\_permission\_set

Updates an existing permission set.

Type annotations and code completion for `#!python session.create_client("sso-admin").update_permission_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/update_permission_set.html)

```python
# update_permission_set method definition

await def update_permission_set(
    self,
    *,
    InstanceArn: str,
    PermissionSetArn: str,
    Description: str = ...,
    RelayState: str = ...,
    SessionDuration: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_permission_set method usage example with argument unpacking

kwargs: UpdatePermissionSetRequestRequestTypeDef = {  # (1)
    "InstanceArn": ...,
    "PermissionSetArn": ...,
}

parent.update_permission_set(**kwargs)
```

1. See [:material-code-braces: UpdatePermissionSetRequestRequestTypeDef](./type_defs.md#updatepermissionsetrequestrequesttypedef) 

### update\_trusted\_token\_issuer

Updates the name of the trusted token issuer, or the path of a source attribute
or destination attribute for a trusted token issuer configuration.

Type annotations and code completion for `#!python session.create_client("sso-admin").update_trusted_token_issuer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/client/update_trusted_token_issuer.html)

```python
# update_trusted_token_issuer method definition

await def update_trusted_token_issuer(
    self,
    *,
    TrustedTokenIssuerArn: str,
    Name: str = ...,
    TrustedTokenIssuerConfiguration: TrustedTokenIssuerUpdateConfigurationTypeDef = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TrustedTokenIssuerUpdateConfigurationTypeDef](./type_defs.md#trustedtokenissuerupdateconfigurationtypedef) 


```python
# update_trusted_token_issuer method usage example with argument unpacking

kwargs: UpdateTrustedTokenIssuerRequestRequestTypeDef = {  # (1)
    "TrustedTokenIssuerArn": ...,
}

parent.update_trusted_token_issuer(**kwargs)
```

1. See [:material-code-braces: UpdateTrustedTokenIssuerRequestRequestTypeDef](./type_defs.md#updatetrustedtokenissuerrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("sso-admin").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "SSOAdminClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("sso-admin").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client)

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

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator` method with overloads.

- `client.get_paginator("list_account_assignment_creation_status")` -> [ListAccountAssignmentCreationStatusPaginator](./paginators.md#listaccountassignmentcreationstatuspaginator)
- `client.get_paginator("list_account_assignment_deletion_status")` -> [ListAccountAssignmentDeletionStatusPaginator](./paginators.md#listaccountassignmentdeletionstatuspaginator)
- `client.get_paginator("list_account_assignments_for_principal")` -> [ListAccountAssignmentsForPrincipalPaginator](./paginators.md#listaccountassignmentsforprincipalpaginator)
- `client.get_paginator("list_account_assignments")` -> [ListAccountAssignmentsPaginator](./paginators.md#listaccountassignmentspaginator)
- `client.get_paginator("list_accounts_for_provisioned_permission_set")` -> [ListAccountsForProvisionedPermissionSetPaginator](./paginators.md#listaccountsforprovisionedpermissionsetpaginator)
- `client.get_paginator("list_application_access_scopes")` -> [ListApplicationAccessScopesPaginator](./paginators.md#listapplicationaccessscopespaginator)
- `client.get_paginator("list_application_assignments_for_principal")` -> [ListApplicationAssignmentsForPrincipalPaginator](./paginators.md#listapplicationassignmentsforprincipalpaginator)
- `client.get_paginator("list_application_assignments")` -> [ListApplicationAssignmentsPaginator](./paginators.md#listapplicationassignmentspaginator)
- `client.get_paginator("list_application_authentication_methods")` -> [ListApplicationAuthenticationMethodsPaginator](./paginators.md#listapplicationauthenticationmethodspaginator)
- `client.get_paginator("list_application_grants")` -> [ListApplicationGrantsPaginator](./paginators.md#listapplicationgrantspaginator)
- `client.get_paginator("list_application_providers")` -> [ListApplicationProvidersPaginator](./paginators.md#listapplicationproviderspaginator)
- `client.get_paginator("list_applications")` -> [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
- `client.get_paginator("list_customer_managed_policy_references_in_permission_set")` -> [ListCustomerManagedPolicyReferencesInPermissionSetPaginator](./paginators.md#listcustomermanagedpolicyreferencesinpermissionsetpaginator)
- `client.get_paginator("list_instances")` -> [ListInstancesPaginator](./paginators.md#listinstancespaginator)
- `client.get_paginator("list_managed_policies_in_permission_set")` -> [ListManagedPoliciesInPermissionSetPaginator](./paginators.md#listmanagedpoliciesinpermissionsetpaginator)
- `client.get_paginator("list_permission_set_provisioning_status")` -> [ListPermissionSetProvisioningStatusPaginator](./paginators.md#listpermissionsetprovisioningstatuspaginator)
- `client.get_paginator("list_permission_sets")` -> [ListPermissionSetsPaginator](./paginators.md#listpermissionsetspaginator)
- `client.get_paginator("list_permission_sets_provisioned_to_account")` -> [ListPermissionSetsProvisionedToAccountPaginator](./paginators.md#listpermissionsetsprovisionedtoaccountpaginator)
- `client.get_paginator("list_tags_for_resource")` -> [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
- `client.get_paginator("list_trusted_token_issuers")` -> [ListTrustedTokenIssuersPaginator](./paginators.md#listtrustedtokenissuerspaginator)



