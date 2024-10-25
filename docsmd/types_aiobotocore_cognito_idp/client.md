# CognitoIdentityProviderClient

> [Index](../README.md) > [CognitoIdentityProvider](./README.md) > CognitoIdentityProviderClient

!!! note ""

    Auto-generated documentation for [CognitoIdentityProvider](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
    type annotations stubs module [types-aiobotocore-cognito-idp](https://pypi.org/project/types-aiobotocore-cognito-idp/).

## CognitoIdentityProviderClient

Type annotations and code completion for `#!python session.create_client("cognito-idp")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client)

```python
# CognitoIdentityProviderClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_cognito_idp.client import CognitoIdentityProviderClient

session = get_session()
async with session.create_client("cognito-idp") as client:
    client: CognitoIdentityProviderClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("cognito-idp").exceptions` structure.

```python
# CognitoIdentityProviderClient.exceptions usage example

async with session.create_client("cognito-idp") as client:
    try:
        do_something(client)
    except (
            client.AliasExistsException,
        client.ClientError,
        client.CodeDeliveryFailureException,
        client.CodeMismatchException,
        client.ConcurrentModificationException,
        client.DuplicateProviderException,
        client.EnableSoftwareTokenMFAException,
        client.ExpiredCodeException,
        client.ForbiddenException,
        client.GroupExistsException,
        client.InternalErrorException,
        client.InvalidEmailRoleAccessPolicyException,
        client.InvalidLambdaResponseException,
        client.InvalidOAuthFlowException,
        client.InvalidParameterException,
        client.InvalidPasswordException,
        client.InvalidSmsRoleAccessPolicyException,
        client.InvalidSmsRoleTrustRelationshipException,
        client.InvalidUserPoolConfigurationException,
        client.LimitExceededException,
        client.MFAMethodNotFoundException,
        client.NotAuthorizedException,
        client.PasswordHistoryPolicyViolationException,
        client.PasswordResetRequiredException,
        client.PreconditionNotMetException,
        client.ResourceNotFoundException,
        client.ScopeDoesNotExistException,
        client.SoftwareTokenMFANotFoundException,
        client.TooManyFailedAttemptsException,
        client.TooManyRequestsException,
        client.UnauthorizedException,
        client.UnexpectedLambdaException,
        client.UnsupportedIdentityProviderException,
        client.UnsupportedOperationException,
        client.UnsupportedTokenTypeException,
        client.UnsupportedUserStateException,
        client.UserImportInProgressException,
        client.UserLambdaValidationException,
        client.UserNotConfirmedException,
        client.UserNotFoundException,
        client.UserPoolAddOnNotEnabledException,
        client.UserPoolTaggingException,
        client.UsernameExistsException,
    ) as e:
        print(e)
```

```python
# CognitoIdentityProviderClient usage type checking example

from types_aiobotocore_cognito_idp.client import Exceptions

def handle_error(exc: Exceptions.AliasExistsException) -> None:
    ...
```


## Methods


### add\_custom\_attributes

Adds additional user attributes to the user pool schema.

Type annotations and code completion for `#!python session.create_client("cognito-idp").add_custom_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.add_custom_attributes)

```python
# add_custom_attributes method definition

await def add_custom_attributes(
    self,
    *,
    UserPoolId: str,
    CustomAttributes: Sequence[SchemaAttributeTypeTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: SchemaAttributeTypeTypeDef](./type_defs.md#schemaattributetypetypedef) 


```python
# add_custom_attributes method usage example with argument unpacking

kwargs: AddCustomAttributesRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "CustomAttributes": ...,
}

parent.add_custom_attributes(**kwargs)
```

1. See [:material-code-braces: AddCustomAttributesRequestRequestTypeDef](./type_defs.md#addcustomattributesrequestrequesttypedef) 

### admin\_add\_user\_to\_group

Adds a user to a group.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_add_user_to_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_add_user_to_group)

```python
# admin_add_user_to_group method definition

await def admin_add_user_to_group(
    self,
    *,
    UserPoolId: str,
    Username: str,
    GroupName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# admin_add_user_to_group method usage example with argument unpacking

kwargs: AdminAddUserToGroupRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Username": ...,
    "GroupName": ...,
}

parent.admin_add_user_to_group(**kwargs)
```

1. See [:material-code-braces: AdminAddUserToGroupRequestRequestTypeDef](./type_defs.md#adminaddusertogrouprequestrequesttypedef) 

### admin\_confirm\_sign\_up

This IAM-authenticated API operation confirms user sign-up as an administrator.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_confirm_sign_up` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_confirm_sign_up)

```python
# admin_confirm_sign_up method definition

await def admin_confirm_sign_up(
    self,
    *,
    UserPoolId: str,
    Username: str,
    ClientMetadata: Mapping[str, str] = ...,
) -> Dict[str, Any]:
    ...
```



```python
# admin_confirm_sign_up method usage example with argument unpacking

kwargs: AdminConfirmSignUpRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Username": ...,
}

parent.admin_confirm_sign_up(**kwargs)
```

1. See [:material-code-braces: AdminConfirmSignUpRequestRequestTypeDef](./type_defs.md#adminconfirmsignuprequestrequesttypedef) 

### admin\_create\_user

Creates a new user in the specified user pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_create_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_create_user)

```python
# admin_create_user method definition

await def admin_create_user(
    self,
    *,
    UserPoolId: str,
    Username: str,
    UserAttributes: Sequence[AttributeTypeTypeDef] = ...,  # (1)
    ValidationData: Sequence[AttributeTypeTypeDef] = ...,  # (1)
    TemporaryPassword: str = ...,
    ForceAliasCreation: bool = ...,
    MessageAction: MessageActionTypeType = ...,  # (3)
    DesiredDeliveryMediums: Sequence[DeliveryMediumTypeType] = ...,  # (4)
    ClientMetadata: Mapping[str, str] = ...,
) -> AdminCreateUserResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: AttributeTypeTypeDef](./type_defs.md#attributetypetypedef) 
2. See [:material-code-braces: AttributeTypeTypeDef](./type_defs.md#attributetypetypedef) 
3. See [:material-code-brackets: MessageActionTypeType](./literals.md#messageactiontypetype) 
4. See [:material-code-brackets: DeliveryMediumTypeType](./literals.md#deliverymediumtypetype) 
5. See [:material-code-braces: AdminCreateUserResponseTypeDef](./type_defs.md#admincreateuserresponsetypedef) 


```python
# admin_create_user method usage example with argument unpacking

kwargs: AdminCreateUserRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Username": ...,
}

parent.admin_create_user(**kwargs)
```

1. See [:material-code-braces: AdminCreateUserRequestRequestTypeDef](./type_defs.md#admincreateuserrequestrequesttypedef) 

### admin\_delete\_user

Deletes a user as an administrator.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_delete_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_delete_user)

```python
# admin_delete_user method definition

await def admin_delete_user(
    self,
    *,
    UserPoolId: str,
    Username: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# admin_delete_user method usage example with argument unpacking

kwargs: AdminDeleteUserRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Username": ...,
}

parent.admin_delete_user(**kwargs)
```

1. See [:material-code-braces: AdminDeleteUserRequestRequestTypeDef](./type_defs.md#admindeleteuserrequestrequesttypedef) 

### admin\_delete\_user\_attributes

Deletes the user attributes in a user pool as an administrator.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_delete_user_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_delete_user_attributes)

```python
# admin_delete_user_attributes method definition

await def admin_delete_user_attributes(
    self,
    *,
    UserPoolId: str,
    Username: str,
    UserAttributeNames: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# admin_delete_user_attributes method usage example with argument unpacking

kwargs: AdminDeleteUserAttributesRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Username": ...,
    "UserAttributeNames": ...,
}

parent.admin_delete_user_attributes(**kwargs)
```

1. See [:material-code-braces: AdminDeleteUserAttributesRequestRequestTypeDef](./type_defs.md#admindeleteuserattributesrequestrequesttypedef) 

### admin\_disable\_provider\_for\_user

Prevents the user from signing in with the specified external (SAML or social)
identity provider
(IdP).

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_disable_provider_for_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_disable_provider_for_user)

```python
# admin_disable_provider_for_user method definition

await def admin_disable_provider_for_user(
    self,
    *,
    UserPoolId: str,
    User: ProviderUserIdentifierTypeTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ProviderUserIdentifierTypeTypeDef](./type_defs.md#provideruseridentifiertypetypedef) 


```python
# admin_disable_provider_for_user method usage example with argument unpacking

kwargs: AdminDisableProviderForUserRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "User": ...,
}

parent.admin_disable_provider_for_user(**kwargs)
```

1. See [:material-code-braces: AdminDisableProviderForUserRequestRequestTypeDef](./type_defs.md#admindisableproviderforuserrequestrequesttypedef) 

### admin\_disable\_user

Deactivates a user and revokes all access tokens for the user.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_disable_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_disable_user)

```python
# admin_disable_user method definition

await def admin_disable_user(
    self,
    *,
    UserPoolId: str,
    Username: str,
) -> Dict[str, Any]:
    ...
```



```python
# admin_disable_user method usage example with argument unpacking

kwargs: AdminDisableUserRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Username": ...,
}

parent.admin_disable_user(**kwargs)
```

1. See [:material-code-braces: AdminDisableUserRequestRequestTypeDef](./type_defs.md#admindisableuserrequestrequesttypedef) 

### admin\_enable\_user

Enables the specified user as an administrator.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_enable_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_enable_user)

```python
# admin_enable_user method definition

await def admin_enable_user(
    self,
    *,
    UserPoolId: str,
    Username: str,
) -> Dict[str, Any]:
    ...
```



```python
# admin_enable_user method usage example with argument unpacking

kwargs: AdminEnableUserRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Username": ...,
}

parent.admin_enable_user(**kwargs)
```

1. See [:material-code-braces: AdminEnableUserRequestRequestTypeDef](./type_defs.md#adminenableuserrequestrequesttypedef) 

### admin\_forget\_device

Forgets the device, as an administrator.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_forget_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_forget_device)

```python
# admin_forget_device method definition

await def admin_forget_device(
    self,
    *,
    UserPoolId: str,
    Username: str,
    DeviceKey: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# admin_forget_device method usage example with argument unpacking

kwargs: AdminForgetDeviceRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Username": ...,
    "DeviceKey": ...,
}

parent.admin_forget_device(**kwargs)
```

1. See [:material-code-braces: AdminForgetDeviceRequestRequestTypeDef](./type_defs.md#adminforgetdevicerequestrequesttypedef) 

### admin\_get\_device

Gets the device, as an administrator.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_get_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_get_device)

```python
# admin_get_device method definition

await def admin_get_device(
    self,
    *,
    DeviceKey: str,
    UserPoolId: str,
    Username: str,
) -> AdminGetDeviceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AdminGetDeviceResponseTypeDef](./type_defs.md#admingetdeviceresponsetypedef) 


```python
# admin_get_device method usage example with argument unpacking

kwargs: AdminGetDeviceRequestRequestTypeDef = {  # (1)
    "DeviceKey": ...,
    "UserPoolId": ...,
    "Username": ...,
}

parent.admin_get_device(**kwargs)
```

1. See [:material-code-braces: AdminGetDeviceRequestRequestTypeDef](./type_defs.md#admingetdevicerequestrequesttypedef) 

### admin\_get\_user

Gets the specified user by user name in a user pool as an administrator.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_get_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_get_user)

```python
# admin_get_user method definition

await def admin_get_user(
    self,
    *,
    UserPoolId: str,
    Username: str,
) -> AdminGetUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AdminGetUserResponseTypeDef](./type_defs.md#admingetuserresponsetypedef) 


```python
# admin_get_user method usage example with argument unpacking

kwargs: AdminGetUserRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Username": ...,
}

parent.admin_get_user(**kwargs)
```

1. See [:material-code-braces: AdminGetUserRequestRequestTypeDef](./type_defs.md#admingetuserrequestrequesttypedef) 

### admin\_initiate\_auth

Initiates the authentication flow, as an administrator.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_initiate_auth` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_initiate_auth)

```python
# admin_initiate_auth method definition

await def admin_initiate_auth(
    self,
    *,
    UserPoolId: str,
    ClientId: str,
    AuthFlow: AuthFlowTypeType,  # (1)
    AuthParameters: Mapping[str, str] = ...,
    ClientMetadata: Mapping[str, str] = ...,
    AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,  # (2)
    ContextData: ContextDataTypeTypeDef = ...,  # (3)
) -> AdminInitiateAuthResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: AuthFlowTypeType](./literals.md#authflowtypetype) 
2. See [:material-code-braces: AnalyticsMetadataTypeTypeDef](./type_defs.md#analyticsmetadatatypetypedef) 
3. See [:material-code-braces: ContextDataTypeTypeDef](./type_defs.md#contextdatatypetypedef) 
4. See [:material-code-braces: AdminInitiateAuthResponseTypeDef](./type_defs.md#admininitiateauthresponsetypedef) 


```python
# admin_initiate_auth method usage example with argument unpacking

kwargs: AdminInitiateAuthRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "ClientId": ...,
    "AuthFlow": ...,
}

parent.admin_initiate_auth(**kwargs)
```

1. See [:material-code-braces: AdminInitiateAuthRequestRequestTypeDef](./type_defs.md#admininitiateauthrequestrequesttypedef) 

### admin\_link\_provider\_for\_user

Links an existing user account in a user pool ( `DestinationUser`) to an
identity from an external IdP ( `SourceUser`) based on a specified attribute
name and value from the external
IdP.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_link_provider_for_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_link_provider_for_user)

```python
# admin_link_provider_for_user method definition

await def admin_link_provider_for_user(
    self,
    *,
    UserPoolId: str,
    DestinationUser: ProviderUserIdentifierTypeTypeDef,  # (1)
    SourceUser: ProviderUserIdentifierTypeTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ProviderUserIdentifierTypeTypeDef](./type_defs.md#provideruseridentifiertypetypedef) 
2. See [:material-code-braces: ProviderUserIdentifierTypeTypeDef](./type_defs.md#provideruseridentifiertypetypedef) 


```python
# admin_link_provider_for_user method usage example with argument unpacking

kwargs: AdminLinkProviderForUserRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "DestinationUser": ...,
    "SourceUser": ...,
}

parent.admin_link_provider_for_user(**kwargs)
```

1. See [:material-code-braces: AdminLinkProviderForUserRequestRequestTypeDef](./type_defs.md#adminlinkproviderforuserrequestrequesttypedef) 

### admin\_list\_devices

Lists devices, as an administrator.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_list_devices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_list_devices)

```python
# admin_list_devices method definition

await def admin_list_devices(
    self,
    *,
    UserPoolId: str,
    Username: str,
    Limit: int = ...,
    PaginationToken: str = ...,
) -> AdminListDevicesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AdminListDevicesResponseTypeDef](./type_defs.md#adminlistdevicesresponsetypedef) 


```python
# admin_list_devices method usage example with argument unpacking

kwargs: AdminListDevicesRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Username": ...,
}

parent.admin_list_devices(**kwargs)
```

1. See [:material-code-braces: AdminListDevicesRequestRequestTypeDef](./type_defs.md#adminlistdevicesrequestrequesttypedef) 

### admin\_list\_groups\_for\_user

Lists the groups that a user belongs to.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_list_groups_for_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_list_groups_for_user)

```python
# admin_list_groups_for_user method definition

await def admin_list_groups_for_user(
    self,
    *,
    Username: str,
    UserPoolId: str,
    Limit: int = ...,
    NextToken: str = ...,
) -> AdminListGroupsForUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AdminListGroupsForUserResponseTypeDef](./type_defs.md#adminlistgroupsforuserresponsetypedef) 


```python
# admin_list_groups_for_user method usage example with argument unpacking

kwargs: AdminListGroupsForUserRequestRequestTypeDef = {  # (1)
    "Username": ...,
    "UserPoolId": ...,
}

parent.admin_list_groups_for_user(**kwargs)
```

1. See [:material-code-braces: AdminListGroupsForUserRequestRequestTypeDef](./type_defs.md#adminlistgroupsforuserrequestrequesttypedef) 

### admin\_list\_user\_auth\_events

A history of user activity and any risks detected as part of Amazon Cognito
advanced
security.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_list_user_auth_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_list_user_auth_events)

```python
# admin_list_user_auth_events method definition

await def admin_list_user_auth_events(
    self,
    *,
    UserPoolId: str,
    Username: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> AdminListUserAuthEventsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AdminListUserAuthEventsResponseTypeDef](./type_defs.md#adminlistuserautheventsresponsetypedef) 


```python
# admin_list_user_auth_events method usage example with argument unpacking

kwargs: AdminListUserAuthEventsRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Username": ...,
}

parent.admin_list_user_auth_events(**kwargs)
```

1. See [:material-code-braces: AdminListUserAuthEventsRequestRequestTypeDef](./type_defs.md#adminlistuserautheventsrequestrequesttypedef) 

### admin\_remove\_user\_from\_group

Removes the specified user from the specified group.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_remove_user_from_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_remove_user_from_group)

```python
# admin_remove_user_from_group method definition

await def admin_remove_user_from_group(
    self,
    *,
    UserPoolId: str,
    Username: str,
    GroupName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# admin_remove_user_from_group method usage example with argument unpacking

kwargs: AdminRemoveUserFromGroupRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Username": ...,
    "GroupName": ...,
}

parent.admin_remove_user_from_group(**kwargs)
```

1. See [:material-code-braces: AdminRemoveUserFromGroupRequestRequestTypeDef](./type_defs.md#adminremoveuserfromgrouprequestrequesttypedef) 

### admin\_reset\_user\_password

Resets the specified user's password in a user pool as an administrator.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_reset_user_password` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_reset_user_password)

```python
# admin_reset_user_password method definition

await def admin_reset_user_password(
    self,
    *,
    UserPoolId: str,
    Username: str,
    ClientMetadata: Mapping[str, str] = ...,
) -> Dict[str, Any]:
    ...
```



```python
# admin_reset_user_password method usage example with argument unpacking

kwargs: AdminResetUserPasswordRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Username": ...,
}

parent.admin_reset_user_password(**kwargs)
```

1. See [:material-code-braces: AdminResetUserPasswordRequestRequestTypeDef](./type_defs.md#adminresetuserpasswordrequestrequesttypedef) 

### admin\_respond\_to\_auth\_challenge

Some API operations in a user pool generate a challenge, like a prompt for an
MFA code, for device authentication that bypasses MFA, or for a custom
authentication
challenge.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_respond_to_auth_challenge` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_respond_to_auth_challenge)

```python
# admin_respond_to_auth_challenge method definition

await def admin_respond_to_auth_challenge(
    self,
    *,
    UserPoolId: str,
    ClientId: str,
    ChallengeName: ChallengeNameTypeType,  # (1)
    ChallengeResponses: Mapping[str, str] = ...,
    Session: str = ...,
    AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,  # (2)
    ContextData: ContextDataTypeTypeDef = ...,  # (3)
    ClientMetadata: Mapping[str, str] = ...,
) -> AdminRespondToAuthChallengeResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ChallengeNameTypeType](./literals.md#challengenametypetype) 
2. See [:material-code-braces: AnalyticsMetadataTypeTypeDef](./type_defs.md#analyticsmetadatatypetypedef) 
3. See [:material-code-braces: ContextDataTypeTypeDef](./type_defs.md#contextdatatypetypedef) 
4. See [:material-code-braces: AdminRespondToAuthChallengeResponseTypeDef](./type_defs.md#adminrespondtoauthchallengeresponsetypedef) 


```python
# admin_respond_to_auth_challenge method usage example with argument unpacking

kwargs: AdminRespondToAuthChallengeRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "ClientId": ...,
    "ChallengeName": ...,
}

parent.admin_respond_to_auth_challenge(**kwargs)
```

1. See [:material-code-braces: AdminRespondToAuthChallengeRequestRequestTypeDef](./type_defs.md#adminrespondtoauthchallengerequestrequesttypedef) 

### admin\_set\_user\_mfa\_preference

Sets the user's multi-factor authentication (MFA) preference, including which
MFA options are activated, and if any are
preferred.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_set_user_mfa_preference` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_set_user_mfa_preference)

```python
# admin_set_user_mfa_preference method definition

await def admin_set_user_mfa_preference(
    self,
    *,
    Username: str,
    UserPoolId: str,
    SMSMfaSettings: SMSMfaSettingsTypeTypeDef = ...,  # (1)
    SoftwareTokenMfaSettings: SoftwareTokenMfaSettingsTypeTypeDef = ...,  # (2)
    EmailMfaSettings: EmailMfaSettingsTypeTypeDef = ...,  # (3)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: SMSMfaSettingsTypeTypeDef](./type_defs.md#smsmfasettingstypetypedef) 
2. See [:material-code-braces: SoftwareTokenMfaSettingsTypeTypeDef](./type_defs.md#softwaretokenmfasettingstypetypedef) 
3. See [:material-code-braces: EmailMfaSettingsTypeTypeDef](./type_defs.md#emailmfasettingstypetypedef) 


```python
# admin_set_user_mfa_preference method usage example with argument unpacking

kwargs: AdminSetUserMFAPreferenceRequestRequestTypeDef = {  # (1)
    "Username": ...,
    "UserPoolId": ...,
}

parent.admin_set_user_mfa_preference(**kwargs)
```

1. See [:material-code-braces: AdminSetUserMFAPreferenceRequestRequestTypeDef](./type_defs.md#adminsetusermfapreferencerequestrequesttypedef) 

### admin\_set\_user\_password

Sets the specified user's password in a user pool as an administrator.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_set_user_password` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_set_user_password)

```python
# admin_set_user_password method definition

await def admin_set_user_password(
    self,
    *,
    UserPoolId: str,
    Username: str,
    Password: str,
    Permanent: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# admin_set_user_password method usage example with argument unpacking

kwargs: AdminSetUserPasswordRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Username": ...,
    "Password": ...,
}

parent.admin_set_user_password(**kwargs)
```

1. See [:material-code-braces: AdminSetUserPasswordRequestRequestTypeDef](./type_defs.md#adminsetuserpasswordrequestrequesttypedef) 

### admin\_set\_user\_settings

*This action is no longer supported.* You can use it to configure only SMS MFA.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_set_user_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_set_user_settings)

```python
# admin_set_user_settings method definition

await def admin_set_user_settings(
    self,
    *,
    UserPoolId: str,
    Username: str,
    MFAOptions: Sequence[MFAOptionTypeTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: MFAOptionTypeTypeDef](./type_defs.md#mfaoptiontypetypedef) 


```python
# admin_set_user_settings method usage example with argument unpacking

kwargs: AdminSetUserSettingsRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Username": ...,
    "MFAOptions": ...,
}

parent.admin_set_user_settings(**kwargs)
```

1. See [:material-code-braces: AdminSetUserSettingsRequestRequestTypeDef](./type_defs.md#adminsetusersettingsrequestrequesttypedef) 

### admin\_update\_auth\_event\_feedback

Provides feedback for an authentication event indicating if it was from a valid
user.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_update_auth_event_feedback` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_update_auth_event_feedback)

```python
# admin_update_auth_event_feedback method definition

await def admin_update_auth_event_feedback(
    self,
    *,
    UserPoolId: str,
    Username: str,
    EventId: str,
    FeedbackValue: FeedbackValueTypeType,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: FeedbackValueTypeType](./literals.md#feedbackvaluetypetype) 


```python
# admin_update_auth_event_feedback method usage example with argument unpacking

kwargs: AdminUpdateAuthEventFeedbackRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Username": ...,
    "EventId": ...,
    "FeedbackValue": ...,
}

parent.admin_update_auth_event_feedback(**kwargs)
```

1. See [:material-code-braces: AdminUpdateAuthEventFeedbackRequestRequestTypeDef](./type_defs.md#adminupdateautheventfeedbackrequestrequesttypedef) 

### admin\_update\_device\_status

Updates the device status as an administrator.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_update_device_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_update_device_status)

```python
# admin_update_device_status method definition

await def admin_update_device_status(
    self,
    *,
    UserPoolId: str,
    Username: str,
    DeviceKey: str,
    DeviceRememberedStatus: DeviceRememberedStatusTypeType = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: DeviceRememberedStatusTypeType](./literals.md#devicerememberedstatustypetype) 


```python
# admin_update_device_status method usage example with argument unpacking

kwargs: AdminUpdateDeviceStatusRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Username": ...,
    "DeviceKey": ...,
}

parent.admin_update_device_status(**kwargs)
```

1. See [:material-code-braces: AdminUpdateDeviceStatusRequestRequestTypeDef](./type_defs.md#adminupdatedevicestatusrequestrequesttypedef) 

### admin\_update\_user\_attributes

.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_update_user_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_update_user_attributes)

```python
# admin_update_user_attributes method definition

await def admin_update_user_attributes(
    self,
    *,
    UserPoolId: str,
    Username: str,
    UserAttributes: Sequence[AttributeTypeTypeDef],  # (1)
    ClientMetadata: Mapping[str, str] = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: AttributeTypeTypeDef](./type_defs.md#attributetypetypedef) 


```python
# admin_update_user_attributes method usage example with argument unpacking

kwargs: AdminUpdateUserAttributesRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Username": ...,
    "UserAttributes": ...,
}

parent.admin_update_user_attributes(**kwargs)
```

1. See [:material-code-braces: AdminUpdateUserAttributesRequestRequestTypeDef](./type_defs.md#adminupdateuserattributesrequestrequesttypedef) 

### admin\_user\_global\_sign\_out

Invalidates the identity, access, and refresh tokens that Amazon Cognito issued
to a
user.

Type annotations and code completion for `#!python session.create_client("cognito-idp").admin_user_global_sign_out` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_user_global_sign_out)

```python
# admin_user_global_sign_out method definition

await def admin_user_global_sign_out(
    self,
    *,
    UserPoolId: str,
    Username: str,
) -> Dict[str, Any]:
    ...
```



```python
# admin_user_global_sign_out method usage example with argument unpacking

kwargs: AdminUserGlobalSignOutRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Username": ...,
}

parent.admin_user_global_sign_out(**kwargs)
```

1. See [:material-code-braces: AdminUserGlobalSignOutRequestRequestTypeDef](./type_defs.md#adminuserglobalsignoutrequestrequesttypedef) 

### associate\_software\_token

Begins setup of time-based one-time password (TOTP) multi-factor authentication
(MFA) for a user, with a unique private key that Amazon Cognito generates and
returns in the API
response.

Type annotations and code completion for `#!python session.create_client("cognito-idp").associate_software_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.associate_software_token)

```python
# associate_software_token method definition

await def associate_software_token(
    self,
    *,
    AccessToken: str = ...,
    Session: str = ...,
) -> AssociateSoftwareTokenResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateSoftwareTokenResponseTypeDef](./type_defs.md#associatesoftwaretokenresponsetypedef) 


```python
# associate_software_token method usage example with argument unpacking

kwargs: AssociateSoftwareTokenRequestRequestTypeDef = {  # (1)
    "AccessToken": ...,
}

parent.associate_software_token(**kwargs)
```

1. See [:material-code-braces: AssociateSoftwareTokenRequestRequestTypeDef](./type_defs.md#associatesoftwaretokenrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("cognito-idp").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### change\_password

Changes the password for a specified user in a user pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").change_password` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.change_password)

```python
# change_password method definition

await def change_password(
    self,
    *,
    PreviousPassword: str,
    ProposedPassword: str,
    AccessToken: str,
) -> Dict[str, Any]:
    ...
```



```python
# change_password method usage example with argument unpacking

kwargs: ChangePasswordRequestRequestTypeDef = {  # (1)
    "PreviousPassword": ...,
    "ProposedPassword": ...,
    "AccessToken": ...,
}

parent.change_password(**kwargs)
```

1. See [:material-code-braces: ChangePasswordRequestRequestTypeDef](./type_defs.md#changepasswordrequestrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("cognito-idp").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### confirm\_device

Confirms tracking of the device.

Type annotations and code completion for `#!python session.create_client("cognito-idp").confirm_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.confirm_device)

```python
# confirm_device method definition

await def confirm_device(
    self,
    *,
    AccessToken: str,
    DeviceKey: str,
    DeviceSecretVerifierConfig: DeviceSecretVerifierConfigTypeTypeDef = ...,  # (1)
    DeviceName: str = ...,
) -> ConfirmDeviceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DeviceSecretVerifierConfigTypeTypeDef](./type_defs.md#devicesecretverifierconfigtypetypedef) 
2. See [:material-code-braces: ConfirmDeviceResponseTypeDef](./type_defs.md#confirmdeviceresponsetypedef) 


```python
# confirm_device method usage example with argument unpacking

kwargs: ConfirmDeviceRequestRequestTypeDef = {  # (1)
    "AccessToken": ...,
    "DeviceKey": ...,
}

parent.confirm_device(**kwargs)
```

1. See [:material-code-braces: ConfirmDeviceRequestRequestTypeDef](./type_defs.md#confirmdevicerequestrequesttypedef) 

### confirm\_forgot\_password

Allows a user to enter a confirmation code to reset a forgotten password.

Type annotations and code completion for `#!python session.create_client("cognito-idp").confirm_forgot_password` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.confirm_forgot_password)

```python
# confirm_forgot_password method definition

await def confirm_forgot_password(
    self,
    *,
    ClientId: str,
    Username: str,
    ConfirmationCode: str,
    Password: str,
    SecretHash: str = ...,
    AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,  # (1)
    UserContextData: UserContextDataTypeTypeDef = ...,  # (2)
    ClientMetadata: Mapping[str, str] = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: AnalyticsMetadataTypeTypeDef](./type_defs.md#analyticsmetadatatypetypedef) 
2. See [:material-code-braces: UserContextDataTypeTypeDef](./type_defs.md#usercontextdatatypetypedef) 


```python
# confirm_forgot_password method usage example with argument unpacking

kwargs: ConfirmForgotPasswordRequestRequestTypeDef = {  # (1)
    "ClientId": ...,
    "Username": ...,
    "ConfirmationCode": ...,
    "Password": ...,
}

parent.confirm_forgot_password(**kwargs)
```

1. See [:material-code-braces: ConfirmForgotPasswordRequestRequestTypeDef](./type_defs.md#confirmforgotpasswordrequestrequesttypedef) 

### confirm\_sign\_up

This public API operation provides a code that Amazon Cognito sent to your user
when they signed up in your user pool via the
[SignUp](https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_SignUp.html)
API
operation.

Type annotations and code completion for `#!python session.create_client("cognito-idp").confirm_sign_up` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.confirm_sign_up)

```python
# confirm_sign_up method definition

await def confirm_sign_up(
    self,
    *,
    ClientId: str,
    Username: str,
    ConfirmationCode: str,
    SecretHash: str = ...,
    ForceAliasCreation: bool = ...,
    AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,  # (1)
    UserContextData: UserContextDataTypeTypeDef = ...,  # (2)
    ClientMetadata: Mapping[str, str] = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: AnalyticsMetadataTypeTypeDef](./type_defs.md#analyticsmetadatatypetypedef) 
2. See [:material-code-braces: UserContextDataTypeTypeDef](./type_defs.md#usercontextdatatypetypedef) 


```python
# confirm_sign_up method usage example with argument unpacking

kwargs: ConfirmSignUpRequestRequestTypeDef = {  # (1)
    "ClientId": ...,
    "Username": ...,
    "ConfirmationCode": ...,
}

parent.confirm_sign_up(**kwargs)
```

1. See [:material-code-braces: ConfirmSignUpRequestRequestTypeDef](./type_defs.md#confirmsignuprequestrequesttypedef) 

### create\_group

Creates a new group in the specified user pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").create_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_group)

```python
# create_group method definition

await def create_group(
    self,
    *,
    GroupName: str,
    UserPoolId: str,
    Description: str = ...,
    RoleArn: str = ...,
    Precedence: int = ...,
) -> CreateGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateGroupResponseTypeDef](./type_defs.md#creategroupresponsetypedef) 


```python
# create_group method usage example with argument unpacking

kwargs: CreateGroupRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
    "UserPoolId": ...,
}

parent.create_group(**kwargs)
```

1. See [:material-code-braces: CreateGroupRequestRequestTypeDef](./type_defs.md#creategrouprequestrequesttypedef) 

### create\_identity\_provider

Adds a configuration and trust relationship between a third-party identity
provider (IdP) and a user
pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").create_identity_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_identity_provider)

```python
# create_identity_provider method definition

await def create_identity_provider(
    self,
    *,
    UserPoolId: str,
    ProviderName: str,
    ProviderType: IdentityProviderTypeTypeType,  # (1)
    ProviderDetails: Mapping[str, str],
    AttributeMapping: Mapping[str, str] = ...,
    IdpIdentifiers: Sequence[str] = ...,
) -> CreateIdentityProviderResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: IdentityProviderTypeTypeType](./literals.md#identityprovidertypetypetype) 
2. See [:material-code-braces: CreateIdentityProviderResponseTypeDef](./type_defs.md#createidentityproviderresponsetypedef) 


```python
# create_identity_provider method usage example with argument unpacking

kwargs: CreateIdentityProviderRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "ProviderName": ...,
    "ProviderType": ...,
    "ProviderDetails": ...,
}

parent.create_identity_provider(**kwargs)
```

1. See [:material-code-braces: CreateIdentityProviderRequestRequestTypeDef](./type_defs.md#createidentityproviderrequestrequesttypedef) 

### create\_resource\_server

Creates a new OAuth2.0 resource server and defines custom scopes within it.

Type annotations and code completion for `#!python session.create_client("cognito-idp").create_resource_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_resource_server)

```python
# create_resource_server method definition

await def create_resource_server(
    self,
    *,
    UserPoolId: str,
    Identifier: str,
    Name: str,
    Scopes: Sequence[ResourceServerScopeTypeTypeDef] = ...,  # (1)
) -> CreateResourceServerResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ResourceServerScopeTypeTypeDef](./type_defs.md#resourceserverscopetypetypedef) 
2. See [:material-code-braces: CreateResourceServerResponseTypeDef](./type_defs.md#createresourceserverresponsetypedef) 


```python
# create_resource_server method usage example with argument unpacking

kwargs: CreateResourceServerRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Identifier": ...,
    "Name": ...,
}

parent.create_resource_server(**kwargs)
```

1. See [:material-code-braces: CreateResourceServerRequestRequestTypeDef](./type_defs.md#createresourceserverrequestrequesttypedef) 

### create\_user\_import\_job

Creates a user import job.

Type annotations and code completion for `#!python session.create_client("cognito-idp").create_user_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_import_job)

```python
# create_user_import_job method definition

await def create_user_import_job(
    self,
    *,
    JobName: str,
    UserPoolId: str,
    CloudWatchLogsRoleArn: str,
) -> CreateUserImportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateUserImportJobResponseTypeDef](./type_defs.md#createuserimportjobresponsetypedef) 


```python
# create_user_import_job method usage example with argument unpacking

kwargs: CreateUserImportJobRequestRequestTypeDef = {  # (1)
    "JobName": ...,
    "UserPoolId": ...,
    "CloudWatchLogsRoleArn": ...,
}

parent.create_user_import_job(**kwargs)
```

1. See [:material-code-braces: CreateUserImportJobRequestRequestTypeDef](./type_defs.md#createuserimportjobrequestrequesttypedef) 

### create\_user\_pool

.

Type annotations and code completion for `#!python session.create_client("cognito-idp").create_user_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool)

```python
# create_user_pool method definition

await def create_user_pool(
    self,
    *,
    PoolName: str,
    Policies: UserPoolPolicyTypeTypeDef = ...,  # (1)
    DeletionProtection: DeletionProtectionTypeType = ...,  # (2)
    LambdaConfig: LambdaConfigTypeTypeDef = ...,  # (3)
    AutoVerifiedAttributes: Sequence[VerifiedAttributeTypeType] = ...,  # (4)
    AliasAttributes: Sequence[AliasAttributeTypeType] = ...,  # (5)
    UsernameAttributes: Sequence[UsernameAttributeTypeType] = ...,  # (6)
    SmsVerificationMessage: str = ...,
    EmailVerificationMessage: str = ...,
    EmailVerificationSubject: str = ...,
    VerificationMessageTemplate: VerificationMessageTemplateTypeTypeDef = ...,  # (7)
    SmsAuthenticationMessage: str = ...,
    MfaConfiguration: UserPoolMfaTypeType = ...,  # (8)
    UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeTypeDef = ...,  # (9)
    DeviceConfiguration: DeviceConfigurationTypeTypeDef = ...,  # (10)
    EmailConfiguration: EmailConfigurationTypeTypeDef = ...,  # (11)
    SmsConfiguration: SmsConfigurationTypeTypeDef = ...,  # (12)
    UserPoolTags: Mapping[str, str] = ...,
    AdminCreateUserConfig: AdminCreateUserConfigTypeTypeDef = ...,  # (13)
    Schema: Sequence[SchemaAttributeTypeTypeDef] = ...,  # (14)
    UserPoolAddOns: UserPoolAddOnsTypeTypeDef = ...,  # (15)
    UsernameConfiguration: UsernameConfigurationTypeTypeDef = ...,  # (16)
    AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...,  # (17)
) -> CreateUserPoolResponseTypeDef:  # (18)
    ...
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
18. See [:material-code-braces: CreateUserPoolResponseTypeDef](./type_defs.md#createuserpoolresponsetypedef) 


```python
# create_user_pool method usage example with argument unpacking

kwargs: CreateUserPoolRequestRequestTypeDef = {  # (1)
    "PoolName": ...,
}

parent.create_user_pool(**kwargs)
```

1. See [:material-code-braces: CreateUserPoolRequestRequestTypeDef](./type_defs.md#createuserpoolrequestrequesttypedef) 

### create\_user\_pool\_client

Creates the user pool client.

Type annotations and code completion for `#!python session.create_client("cognito-idp").create_user_pool_client` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool_client)

```python
# create_user_pool_client method definition

await def create_user_pool_client(
    self,
    *,
    UserPoolId: str,
    ClientName: str,
    GenerateSecret: bool = ...,
    RefreshTokenValidity: int = ...,
    AccessTokenValidity: int = ...,
    IdTokenValidity: int = ...,
    TokenValidityUnits: TokenValidityUnitsTypeTypeDef = ...,  # (1)
    ReadAttributes: Sequence[str] = ...,
    WriteAttributes: Sequence[str] = ...,
    ExplicitAuthFlows: Sequence[ExplicitAuthFlowsTypeType] = ...,  # (2)
    SupportedIdentityProviders: Sequence[str] = ...,
    CallbackURLs: Sequence[str] = ...,
    LogoutURLs: Sequence[str] = ...,
    DefaultRedirectURI: str = ...,
    AllowedOAuthFlows: Sequence[OAuthFlowTypeType] = ...,  # (3)
    AllowedOAuthScopes: Sequence[str] = ...,
    AllowedOAuthFlowsUserPoolClient: bool = ...,
    AnalyticsConfiguration: AnalyticsConfigurationTypeTypeDef = ...,  # (4)
    PreventUserExistenceErrors: PreventUserExistenceErrorTypesType = ...,  # (5)
    EnableTokenRevocation: bool = ...,
    EnablePropagateAdditionalUserContextData: bool = ...,
    AuthSessionValidity: int = ...,
) -> CreateUserPoolClientResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: TokenValidityUnitsTypeTypeDef](./type_defs.md#tokenvalidityunitstypetypedef) 
2. See [:material-code-brackets: ExplicitAuthFlowsTypeType](./literals.md#explicitauthflowstypetype) 
3. See [:material-code-brackets: OAuthFlowTypeType](./literals.md#oauthflowtypetype) 
4. See [:material-code-braces: AnalyticsConfigurationTypeTypeDef](./type_defs.md#analyticsconfigurationtypetypedef) 
5. See [:material-code-brackets: PreventUserExistenceErrorTypesType](./literals.md#preventuserexistenceerrortypestype) 
6. See [:material-code-braces: CreateUserPoolClientResponseTypeDef](./type_defs.md#createuserpoolclientresponsetypedef) 


```python
# create_user_pool_client method usage example with argument unpacking

kwargs: CreateUserPoolClientRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "ClientName": ...,
}

parent.create_user_pool_client(**kwargs)
```

1. See [:material-code-braces: CreateUserPoolClientRequestRequestTypeDef](./type_defs.md#createuserpoolclientrequestrequesttypedef) 

### create\_user\_pool\_domain

Creates a new domain for a user pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").create_user_pool_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool_domain)

```python
# create_user_pool_domain method definition

await def create_user_pool_domain(
    self,
    *,
    Domain: str,
    UserPoolId: str,
    CustomDomainConfig: CustomDomainConfigTypeTypeDef = ...,  # (1)
) -> CreateUserPoolDomainResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CustomDomainConfigTypeTypeDef](./type_defs.md#customdomainconfigtypetypedef) 
2. See [:material-code-braces: CreateUserPoolDomainResponseTypeDef](./type_defs.md#createuserpooldomainresponsetypedef) 


```python
# create_user_pool_domain method usage example with argument unpacking

kwargs: CreateUserPoolDomainRequestRequestTypeDef = {  # (1)
    "Domain": ...,
    "UserPoolId": ...,
}

parent.create_user_pool_domain(**kwargs)
```

1. See [:material-code-braces: CreateUserPoolDomainRequestRequestTypeDef](./type_defs.md#createuserpooldomainrequestrequesttypedef) 

### delete\_group

Deletes a group.

Type annotations and code completion for `#!python session.create_client("cognito-idp").delete_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.delete_group)

```python
# delete_group method definition

await def delete_group(
    self,
    *,
    GroupName: str,
    UserPoolId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_group method usage example with argument unpacking

kwargs: DeleteGroupRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
    "UserPoolId": ...,
}

parent.delete_group(**kwargs)
```

1. See [:material-code-braces: DeleteGroupRequestRequestTypeDef](./type_defs.md#deletegrouprequestrequesttypedef) 

### delete\_identity\_provider

Deletes an IdP for a user pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").delete_identity_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.delete_identity_provider)

```python
# delete_identity_provider method definition

await def delete_identity_provider(
    self,
    *,
    UserPoolId: str,
    ProviderName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_identity_provider method usage example with argument unpacking

kwargs: DeleteIdentityProviderRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "ProviderName": ...,
}

parent.delete_identity_provider(**kwargs)
```

1. See [:material-code-braces: DeleteIdentityProviderRequestRequestTypeDef](./type_defs.md#deleteidentityproviderrequestrequesttypedef) 

### delete\_resource\_server

Deletes a resource server.

Type annotations and code completion for `#!python session.create_client("cognito-idp").delete_resource_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.delete_resource_server)

```python
# delete_resource_server method definition

await def delete_resource_server(
    self,
    *,
    UserPoolId: str,
    Identifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_resource_server method usage example with argument unpacking

kwargs: DeleteResourceServerRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Identifier": ...,
}

parent.delete_resource_server(**kwargs)
```

1. See [:material-code-braces: DeleteResourceServerRequestRequestTypeDef](./type_defs.md#deleteresourceserverrequestrequesttypedef) 

### delete\_user

Allows a user to delete their own user profile.

Type annotations and code completion for `#!python session.create_client("cognito-idp").delete_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.delete_user)

```python
# delete_user method definition

await def delete_user(
    self,
    *,
    AccessToken: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_user method usage example with argument unpacking

kwargs: DeleteUserRequestRequestTypeDef = {  # (1)
    "AccessToken": ...,
}

parent.delete_user(**kwargs)
```

1. See [:material-code-braces: DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef) 

### delete\_user\_attributes

Deletes the attributes for a user.

Type annotations and code completion for `#!python session.create_client("cognito-idp").delete_user_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.delete_user_attributes)

```python
# delete_user_attributes method definition

await def delete_user_attributes(
    self,
    *,
    UserAttributeNames: Sequence[str],
    AccessToken: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_user_attributes method usage example with argument unpacking

kwargs: DeleteUserAttributesRequestRequestTypeDef = {  # (1)
    "UserAttributeNames": ...,
    "AccessToken": ...,
}

parent.delete_user_attributes(**kwargs)
```

1. See [:material-code-braces: DeleteUserAttributesRequestRequestTypeDef](./type_defs.md#deleteuserattributesrequestrequesttypedef) 

### delete\_user\_pool

Deletes the specified Amazon Cognito user pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").delete_user_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.delete_user_pool)

```python
# delete_user_pool method definition

await def delete_user_pool(
    self,
    *,
    UserPoolId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_user_pool method usage example with argument unpacking

kwargs: DeleteUserPoolRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.delete_user_pool(**kwargs)
```

1. See [:material-code-braces: DeleteUserPoolRequestRequestTypeDef](./type_defs.md#deleteuserpoolrequestrequesttypedef) 

### delete\_user\_pool\_client

Allows the developer to delete the user pool client.

Type annotations and code completion for `#!python session.create_client("cognito-idp").delete_user_pool_client` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.delete_user_pool_client)

```python
# delete_user_pool_client method definition

await def delete_user_pool_client(
    self,
    *,
    UserPoolId: str,
    ClientId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_user_pool_client method usage example with argument unpacking

kwargs: DeleteUserPoolClientRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "ClientId": ...,
}

parent.delete_user_pool_client(**kwargs)
```

1. See [:material-code-braces: DeleteUserPoolClientRequestRequestTypeDef](./type_defs.md#deleteuserpoolclientrequestrequesttypedef) 

### delete\_user\_pool\_domain

Deletes a domain for a user pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").delete_user_pool_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.delete_user_pool_domain)

```python
# delete_user_pool_domain method definition

await def delete_user_pool_domain(
    self,
    *,
    Domain: str,
    UserPoolId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_user_pool_domain method usage example with argument unpacking

kwargs: DeleteUserPoolDomainRequestRequestTypeDef = {  # (1)
    "Domain": ...,
    "UserPoolId": ...,
}

parent.delete_user_pool_domain(**kwargs)
```

1. See [:material-code-braces: DeleteUserPoolDomainRequestRequestTypeDef](./type_defs.md#deleteuserpooldomainrequestrequesttypedef) 

### describe\_identity\_provider

Gets information about a specific IdP.

Type annotations and code completion for `#!python session.create_client("cognito-idp").describe_identity_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_identity_provider)

```python
# describe_identity_provider method definition

await def describe_identity_provider(
    self,
    *,
    UserPoolId: str,
    ProviderName: str,
) -> DescribeIdentityProviderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeIdentityProviderResponseTypeDef](./type_defs.md#describeidentityproviderresponsetypedef) 


```python
# describe_identity_provider method usage example with argument unpacking

kwargs: DescribeIdentityProviderRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "ProviderName": ...,
}

parent.describe_identity_provider(**kwargs)
```

1. See [:material-code-braces: DescribeIdentityProviderRequestRequestTypeDef](./type_defs.md#describeidentityproviderrequestrequesttypedef) 

### describe\_resource\_server

Describes a resource server.

Type annotations and code completion for `#!python session.create_client("cognito-idp").describe_resource_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_resource_server)

```python
# describe_resource_server method definition

await def describe_resource_server(
    self,
    *,
    UserPoolId: str,
    Identifier: str,
) -> DescribeResourceServerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeResourceServerResponseTypeDef](./type_defs.md#describeresourceserverresponsetypedef) 


```python
# describe_resource_server method usage example with argument unpacking

kwargs: DescribeResourceServerRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Identifier": ...,
}

parent.describe_resource_server(**kwargs)
```

1. See [:material-code-braces: DescribeResourceServerRequestRequestTypeDef](./type_defs.md#describeresourceserverrequestrequesttypedef) 

### describe\_risk\_configuration

Describes the risk configuration.

Type annotations and code completion for `#!python session.create_client("cognito-idp").describe_risk_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_risk_configuration)

```python
# describe_risk_configuration method definition

await def describe_risk_configuration(
    self,
    *,
    UserPoolId: str,
    ClientId: str = ...,
) -> DescribeRiskConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRiskConfigurationResponseTypeDef](./type_defs.md#describeriskconfigurationresponsetypedef) 


```python
# describe_risk_configuration method usage example with argument unpacking

kwargs: DescribeRiskConfigurationRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.describe_risk_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeRiskConfigurationRequestRequestTypeDef](./type_defs.md#describeriskconfigurationrequestrequesttypedef) 

### describe\_user\_import\_job

Describes the user import job.

Type annotations and code completion for `#!python session.create_client("cognito-idp").describe_user_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_user_import_job)

```python
# describe_user_import_job method definition

await def describe_user_import_job(
    self,
    *,
    UserPoolId: str,
    JobId: str,
) -> DescribeUserImportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeUserImportJobResponseTypeDef](./type_defs.md#describeuserimportjobresponsetypedef) 


```python
# describe_user_import_job method usage example with argument unpacking

kwargs: DescribeUserImportJobRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "JobId": ...,
}

parent.describe_user_import_job(**kwargs)
```

1. See [:material-code-braces: DescribeUserImportJobRequestRequestTypeDef](./type_defs.md#describeuserimportjobrequestrequesttypedef) 

### describe\_user\_pool

Returns the configuration information and metadata of the specified user pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").describe_user_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_user_pool)

```python
# describe_user_pool method definition

await def describe_user_pool(
    self,
    *,
    UserPoolId: str,
) -> DescribeUserPoolResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeUserPoolResponseTypeDef](./type_defs.md#describeuserpoolresponsetypedef) 


```python
# describe_user_pool method usage example with argument unpacking

kwargs: DescribeUserPoolRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.describe_user_pool(**kwargs)
```

1. See [:material-code-braces: DescribeUserPoolRequestRequestTypeDef](./type_defs.md#describeuserpoolrequestrequesttypedef) 

### describe\_user\_pool\_client

Client method for returning the configuration information and metadata of the
specified user pool app
client.

Type annotations and code completion for `#!python session.create_client("cognito-idp").describe_user_pool_client` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_user_pool_client)

```python
# describe_user_pool_client method definition

await def describe_user_pool_client(
    self,
    *,
    UserPoolId: str,
    ClientId: str,
) -> DescribeUserPoolClientResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeUserPoolClientResponseTypeDef](./type_defs.md#describeuserpoolclientresponsetypedef) 


```python
# describe_user_pool_client method usage example with argument unpacking

kwargs: DescribeUserPoolClientRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "ClientId": ...,
}

parent.describe_user_pool_client(**kwargs)
```

1. See [:material-code-braces: DescribeUserPoolClientRequestRequestTypeDef](./type_defs.md#describeuserpoolclientrequestrequesttypedef) 

### describe\_user\_pool\_domain

Gets information about a domain.

Type annotations and code completion for `#!python session.create_client("cognito-idp").describe_user_pool_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_user_pool_domain)

```python
# describe_user_pool_domain method definition

await def describe_user_pool_domain(
    self,
    *,
    Domain: str,
) -> DescribeUserPoolDomainResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeUserPoolDomainResponseTypeDef](./type_defs.md#describeuserpooldomainresponsetypedef) 


```python
# describe_user_pool_domain method usage example with argument unpacking

kwargs: DescribeUserPoolDomainRequestRequestTypeDef = {  # (1)
    "Domain": ...,
}

parent.describe_user_pool_domain(**kwargs)
```

1. See [:material-code-braces: DescribeUserPoolDomainRequestRequestTypeDef](./type_defs.md#describeuserpooldomainrequestrequesttypedef) 

### forget\_device

Forgets the specified device.

Type annotations and code completion for `#!python session.create_client("cognito-idp").forget_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.forget_device)

```python
# forget_device method definition

await def forget_device(
    self,
    *,
    DeviceKey: str,
    AccessToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# forget_device method usage example with argument unpacking

kwargs: ForgetDeviceRequestRequestTypeDef = {  # (1)
    "DeviceKey": ...,
}

parent.forget_device(**kwargs)
```

1. See [:material-code-braces: ForgetDeviceRequestRequestTypeDef](./type_defs.md#forgetdevicerequestrequesttypedef) 

### forgot\_password

Calling this API causes a message to be sent to the end user with a
confirmation code that is required to change the user's
password.

Type annotations and code completion for `#!python session.create_client("cognito-idp").forgot_password` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.forgot_password)

```python
# forgot_password method definition

await def forgot_password(
    self,
    *,
    ClientId: str,
    Username: str,
    SecretHash: str = ...,
    UserContextData: UserContextDataTypeTypeDef = ...,  # (1)
    AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,  # (2)
    ClientMetadata: Mapping[str, str] = ...,
) -> ForgotPasswordResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: UserContextDataTypeTypeDef](./type_defs.md#usercontextdatatypetypedef) 
2. See [:material-code-braces: AnalyticsMetadataTypeTypeDef](./type_defs.md#analyticsmetadatatypetypedef) 
3. See [:material-code-braces: ForgotPasswordResponseTypeDef](./type_defs.md#forgotpasswordresponsetypedef) 


```python
# forgot_password method usage example with argument unpacking

kwargs: ForgotPasswordRequestRequestTypeDef = {  # (1)
    "ClientId": ...,
    "Username": ...,
}

parent.forgot_password(**kwargs)
```

1. See [:material-code-braces: ForgotPasswordRequestRequestTypeDef](./type_defs.md#forgotpasswordrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("cognito-idp").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.generate_presigned_url)

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


### get\_csv\_header

Gets the header information for the comma-separated value (CSV) file to be used
as input for the user import
job.

Type annotations and code completion for `#!python session.create_client("cognito-idp").get_csv_header` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_csv_header)

```python
# get_csv_header method definition

await def get_csv_header(
    self,
    *,
    UserPoolId: str,
) -> GetCSVHeaderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCSVHeaderResponseTypeDef](./type_defs.md#getcsvheaderresponsetypedef) 


```python
# get_csv_header method usage example with argument unpacking

kwargs: GetCSVHeaderRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.get_csv_header(**kwargs)
```

1. See [:material-code-braces: GetCSVHeaderRequestRequestTypeDef](./type_defs.md#getcsvheaderrequestrequesttypedef) 

### get\_device

Gets the device.

Type annotations and code completion for `#!python session.create_client("cognito-idp").get_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_device)

```python
# get_device method definition

await def get_device(
    self,
    *,
    DeviceKey: str,
    AccessToken: str = ...,
) -> GetDeviceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeviceResponseTypeDef](./type_defs.md#getdeviceresponsetypedef) 


```python
# get_device method usage example with argument unpacking

kwargs: GetDeviceRequestRequestTypeDef = {  # (1)
    "DeviceKey": ...,
}

parent.get_device(**kwargs)
```

1. See [:material-code-braces: GetDeviceRequestRequestTypeDef](./type_defs.md#getdevicerequestrequesttypedef) 

### get\_group

Gets a group.

Type annotations and code completion for `#!python session.create_client("cognito-idp").get_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_group)

```python
# get_group method definition

await def get_group(
    self,
    *,
    GroupName: str,
    UserPoolId: str,
) -> GetGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGroupResponseTypeDef](./type_defs.md#getgroupresponsetypedef) 


```python
# get_group method usage example with argument unpacking

kwargs: GetGroupRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
    "UserPoolId": ...,
}

parent.get_group(**kwargs)
```

1. See [:material-code-braces: GetGroupRequestRequestTypeDef](./type_defs.md#getgrouprequestrequesttypedef) 

### get\_identity\_provider\_by\_identifier

Gets the specified IdP.

Type annotations and code completion for `#!python session.create_client("cognito-idp").get_identity_provider_by_identifier` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_identity_provider_by_identifier)

```python
# get_identity_provider_by_identifier method definition

await def get_identity_provider_by_identifier(
    self,
    *,
    UserPoolId: str,
    IdpIdentifier: str,
) -> GetIdentityProviderByIdentifierResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIdentityProviderByIdentifierResponseTypeDef](./type_defs.md#getidentityproviderbyidentifierresponsetypedef) 


```python
# get_identity_provider_by_identifier method usage example with argument unpacking

kwargs: GetIdentityProviderByIdentifierRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "IdpIdentifier": ...,
}

parent.get_identity_provider_by_identifier(**kwargs)
```

1. See [:material-code-braces: GetIdentityProviderByIdentifierRequestRequestTypeDef](./type_defs.md#getidentityproviderbyidentifierrequestrequesttypedef) 

### get\_log\_delivery\_configuration

Gets the logging configuration of a user pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").get_log_delivery_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_log_delivery_configuration)

```python
# get_log_delivery_configuration method definition

await def get_log_delivery_configuration(
    self,
    *,
    UserPoolId: str,
) -> GetLogDeliveryConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLogDeliveryConfigurationResponseTypeDef](./type_defs.md#getlogdeliveryconfigurationresponsetypedef) 


```python
# get_log_delivery_configuration method usage example with argument unpacking

kwargs: GetLogDeliveryConfigurationRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.get_log_delivery_configuration(**kwargs)
```

1. See [:material-code-braces: GetLogDeliveryConfigurationRequestRequestTypeDef](./type_defs.md#getlogdeliveryconfigurationrequestrequesttypedef) 

### get\_signing\_certificate

This method takes a user pool ID, and returns the signing certificate.

Type annotations and code completion for `#!python session.create_client("cognito-idp").get_signing_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_signing_certificate)

```python
# get_signing_certificate method definition

await def get_signing_certificate(
    self,
    *,
    UserPoolId: str,
) -> GetSigningCertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSigningCertificateResponseTypeDef](./type_defs.md#getsigningcertificateresponsetypedef) 


```python
# get_signing_certificate method usage example with argument unpacking

kwargs: GetSigningCertificateRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.get_signing_certificate(**kwargs)
```

1. See [:material-code-braces: GetSigningCertificateRequestRequestTypeDef](./type_defs.md#getsigningcertificaterequestrequesttypedef) 

### get\_ui\_customization

Gets the user interface (UI) Customization information for a particular app
client's app UI, if any such information exists for the
client.

Type annotations and code completion for `#!python session.create_client("cognito-idp").get_ui_customization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_ui_customization)

```python
# get_ui_customization method definition

await def get_ui_customization(
    self,
    *,
    UserPoolId: str,
    ClientId: str = ...,
) -> GetUICustomizationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetUICustomizationResponseTypeDef](./type_defs.md#getuicustomizationresponsetypedef) 


```python
# get_ui_customization method usage example with argument unpacking

kwargs: GetUICustomizationRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.get_ui_customization(**kwargs)
```

1. See [:material-code-braces: GetUICustomizationRequestRequestTypeDef](./type_defs.md#getuicustomizationrequestrequesttypedef) 

### get\_user

Gets the user attributes and metadata for a user.

Type annotations and code completion for `#!python session.create_client("cognito-idp").get_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_user)

```python
# get_user method definition

await def get_user(
    self,
    *,
    AccessToken: str,
) -> GetUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetUserResponseTypeDef](./type_defs.md#getuserresponsetypedef) 


```python
# get_user method usage example with argument unpacking

kwargs: GetUserRequestRequestTypeDef = {  # (1)
    "AccessToken": ...,
}

parent.get_user(**kwargs)
```

1. See [:material-code-braces: GetUserRequestRequestTypeDef](./type_defs.md#getuserrequestrequesttypedef) 

### get\_user\_attribute\_verification\_code

Generates a user attribute verification code for the specified attribute name.

Type annotations and code completion for `#!python session.create_client("cognito-idp").get_user_attribute_verification_code` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_user_attribute_verification_code)

```python
# get_user_attribute_verification_code method definition

await def get_user_attribute_verification_code(
    self,
    *,
    AccessToken: str,
    AttributeName: str,
    ClientMetadata: Mapping[str, str] = ...,
) -> GetUserAttributeVerificationCodeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetUserAttributeVerificationCodeResponseTypeDef](./type_defs.md#getuserattributeverificationcoderesponsetypedef) 


```python
# get_user_attribute_verification_code method usage example with argument unpacking

kwargs: GetUserAttributeVerificationCodeRequestRequestTypeDef = {  # (1)
    "AccessToken": ...,
    "AttributeName": ...,
}

parent.get_user_attribute_verification_code(**kwargs)
```

1. See [:material-code-braces: GetUserAttributeVerificationCodeRequestRequestTypeDef](./type_defs.md#getuserattributeverificationcoderequestrequesttypedef) 

### get\_user\_pool\_mfa\_config

Gets the user pool multi-factor authentication (MFA) configuration.

Type annotations and code completion for `#!python session.create_client("cognito-idp").get_user_pool_mfa_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_user_pool_mfa_config)

```python
# get_user_pool_mfa_config method definition

await def get_user_pool_mfa_config(
    self,
    *,
    UserPoolId: str,
) -> GetUserPoolMfaConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetUserPoolMfaConfigResponseTypeDef](./type_defs.md#getuserpoolmfaconfigresponsetypedef) 


```python
# get_user_pool_mfa_config method usage example with argument unpacking

kwargs: GetUserPoolMfaConfigRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.get_user_pool_mfa_config(**kwargs)
```

1. See [:material-code-braces: GetUserPoolMfaConfigRequestRequestTypeDef](./type_defs.md#getuserpoolmfaconfigrequestrequesttypedef) 

### global\_sign\_out

Invalidates the identity, access, and refresh tokens that Amazon Cognito issued
to a
user.

Type annotations and code completion for `#!python session.create_client("cognito-idp").global_sign_out` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.global_sign_out)

```python
# global_sign_out method definition

await def global_sign_out(
    self,
    *,
    AccessToken: str,
) -> Dict[str, Any]:
    ...
```



```python
# global_sign_out method usage example with argument unpacking

kwargs: GlobalSignOutRequestRequestTypeDef = {  # (1)
    "AccessToken": ...,
}

parent.global_sign_out(**kwargs)
```

1. See [:material-code-braces: GlobalSignOutRequestRequestTypeDef](./type_defs.md#globalsignoutrequestrequesttypedef) 

### initiate\_auth

Initiates sign-in for a user in the Amazon Cognito user directory.

Type annotations and code completion for `#!python session.create_client("cognito-idp").initiate_auth` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.initiate_auth)

```python
# initiate_auth method definition

await def initiate_auth(
    self,
    *,
    AuthFlow: AuthFlowTypeType,  # (1)
    ClientId: str,
    AuthParameters: Mapping[str, str] = ...,
    ClientMetadata: Mapping[str, str] = ...,
    AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,  # (2)
    UserContextData: UserContextDataTypeTypeDef = ...,  # (3)
) -> InitiateAuthResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: AuthFlowTypeType](./literals.md#authflowtypetype) 
2. See [:material-code-braces: AnalyticsMetadataTypeTypeDef](./type_defs.md#analyticsmetadatatypetypedef) 
3. See [:material-code-braces: UserContextDataTypeTypeDef](./type_defs.md#usercontextdatatypetypedef) 
4. See [:material-code-braces: InitiateAuthResponseTypeDef](./type_defs.md#initiateauthresponsetypedef) 


```python
# initiate_auth method usage example with argument unpacking

kwargs: InitiateAuthRequestRequestTypeDef = {  # (1)
    "AuthFlow": ...,
    "ClientId": ...,
}

parent.initiate_auth(**kwargs)
```

1. See [:material-code-braces: InitiateAuthRequestRequestTypeDef](./type_defs.md#initiateauthrequestrequesttypedef) 

### list\_devices

Lists the sign-in devices that Amazon Cognito has registered to the current
user.

Type annotations and code completion for `#!python session.create_client("cognito-idp").list_devices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_devices)

```python
# list_devices method definition

await def list_devices(
    self,
    *,
    AccessToken: str,
    Limit: int = ...,
    PaginationToken: str = ...,
) -> ListDevicesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDevicesResponseTypeDef](./type_defs.md#listdevicesresponsetypedef) 


```python
# list_devices method usage example with argument unpacking

kwargs: ListDevicesRequestRequestTypeDef = {  # (1)
    "AccessToken": ...,
}

parent.list_devices(**kwargs)
```

1. See [:material-code-braces: ListDevicesRequestRequestTypeDef](./type_defs.md#listdevicesrequestrequesttypedef) 

### list\_groups

Lists the groups associated with a user pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").list_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_groups)

```python
# list_groups method definition

await def list_groups(
    self,
    *,
    UserPoolId: str,
    Limit: int = ...,
    NextToken: str = ...,
) -> ListGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


```python
# list_groups method usage example with argument unpacking

kwargs: ListGroupsRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.list_groups(**kwargs)
```

1. See [:material-code-braces: ListGroupsRequestRequestTypeDef](./type_defs.md#listgroupsrequestrequesttypedef) 

### list\_identity\_providers

Lists information about all IdPs for a user pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").list_identity_providers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_identity_providers)

```python
# list_identity_providers method definition

await def list_identity_providers(
    self,
    *,
    UserPoolId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListIdentityProvidersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIdentityProvidersResponseTypeDef](./type_defs.md#listidentityprovidersresponsetypedef) 


```python
# list_identity_providers method usage example with argument unpacking

kwargs: ListIdentityProvidersRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.list_identity_providers(**kwargs)
```

1. See [:material-code-braces: ListIdentityProvidersRequestRequestTypeDef](./type_defs.md#listidentityprovidersrequestrequesttypedef) 

### list\_resource\_servers

Lists the resource servers for a user pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").list_resource_servers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_resource_servers)

```python
# list_resource_servers method definition

await def list_resource_servers(
    self,
    *,
    UserPoolId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListResourceServersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListResourceServersResponseTypeDef](./type_defs.md#listresourceserversresponsetypedef) 


```python
# list_resource_servers method usage example with argument unpacking

kwargs: ListResourceServersRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.list_resource_servers(**kwargs)
```

1. See [:material-code-braces: ListResourceServersRequestRequestTypeDef](./type_defs.md#listresourceserversrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags that are assigned to an Amazon Cognito user pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
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

### list\_user\_import\_jobs

Lists user import jobs for a user pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").list_user_import_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_user_import_jobs)

```python
# list_user_import_jobs method definition

await def list_user_import_jobs(
    self,
    *,
    UserPoolId: str,
    MaxResults: int,
    PaginationToken: str = ...,
) -> ListUserImportJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListUserImportJobsResponseTypeDef](./type_defs.md#listuserimportjobsresponsetypedef) 


```python
# list_user_import_jobs method usage example with argument unpacking

kwargs: ListUserImportJobsRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "MaxResults": ...,
}

parent.list_user_import_jobs(**kwargs)
```

1. See [:material-code-braces: ListUserImportJobsRequestRequestTypeDef](./type_defs.md#listuserimportjobsrequestrequesttypedef) 

### list\_user\_pool\_clients

Lists the clients that have been created for the specified user pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").list_user_pool_clients` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_user_pool_clients)

```python
# list_user_pool_clients method definition

await def list_user_pool_clients(
    self,
    *,
    UserPoolId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListUserPoolClientsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListUserPoolClientsResponseTypeDef](./type_defs.md#listuserpoolclientsresponsetypedef) 


```python
# list_user_pool_clients method usage example with argument unpacking

kwargs: ListUserPoolClientsRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.list_user_pool_clients(**kwargs)
```

1. See [:material-code-braces: ListUserPoolClientsRequestRequestTypeDef](./type_defs.md#listuserpoolclientsrequestrequesttypedef) 

### list\_user\_pools

Lists the user pools associated with an Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("cognito-idp").list_user_pools` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_user_pools)

```python
# list_user_pools method definition

await def list_user_pools(
    self,
    *,
    MaxResults: int,
    NextToken: str = ...,
) -> ListUserPoolsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListUserPoolsResponseTypeDef](./type_defs.md#listuserpoolsresponsetypedef) 


```python
# list_user_pools method usage example with argument unpacking

kwargs: ListUserPoolsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_user_pools(**kwargs)
```

1. See [:material-code-braces: ListUserPoolsRequestRequestTypeDef](./type_defs.md#listuserpoolsrequestrequesttypedef) 

### list\_users

Lists users and their basic details in a user pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").list_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_users)

```python
# list_users method definition

await def list_users(
    self,
    *,
    UserPoolId: str,
    AttributesToGet: Sequence[str] = ...,
    Limit: int = ...,
    PaginationToken: str = ...,
    Filter: str = ...,
) -> ListUsersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


```python
# list_users method usage example with argument unpacking

kwargs: ListUsersRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.list_users(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestRequestTypeDef](./type_defs.md#listusersrequestrequesttypedef) 

### list\_users\_in\_group

Lists the users in the specified group.

Type annotations and code completion for `#!python session.create_client("cognito-idp").list_users_in_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_users_in_group)

```python
# list_users_in_group method definition

await def list_users_in_group(
    self,
    *,
    UserPoolId: str,
    GroupName: str,
    Limit: int = ...,
    NextToken: str = ...,
) -> ListUsersInGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListUsersInGroupResponseTypeDef](./type_defs.md#listusersingroupresponsetypedef) 


```python
# list_users_in_group method usage example with argument unpacking

kwargs: ListUsersInGroupRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "GroupName": ...,
}

parent.list_users_in_group(**kwargs)
```

1. See [:material-code-braces: ListUsersInGroupRequestRequestTypeDef](./type_defs.md#listusersingrouprequestrequesttypedef) 

### resend\_confirmation\_code

Resends the confirmation (for confirmation of registration) to a specific user
in the user
pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").resend_confirmation_code` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.resend_confirmation_code)

```python
# resend_confirmation_code method definition

await def resend_confirmation_code(
    self,
    *,
    ClientId: str,
    Username: str,
    SecretHash: str = ...,
    UserContextData: UserContextDataTypeTypeDef = ...,  # (1)
    AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,  # (2)
    ClientMetadata: Mapping[str, str] = ...,
) -> ResendConfirmationCodeResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: UserContextDataTypeTypeDef](./type_defs.md#usercontextdatatypetypedef) 
2. See [:material-code-braces: AnalyticsMetadataTypeTypeDef](./type_defs.md#analyticsmetadatatypetypedef) 
3. See [:material-code-braces: ResendConfirmationCodeResponseTypeDef](./type_defs.md#resendconfirmationcoderesponsetypedef) 


```python
# resend_confirmation_code method usage example with argument unpacking

kwargs: ResendConfirmationCodeRequestRequestTypeDef = {  # (1)
    "ClientId": ...,
    "Username": ...,
}

parent.resend_confirmation_code(**kwargs)
```

1. See [:material-code-braces: ResendConfirmationCodeRequestRequestTypeDef](./type_defs.md#resendconfirmationcoderequestrequesttypedef) 

### respond\_to\_auth\_challenge

Some API operations in a user pool generate a challenge, like a prompt for an
MFA code, for device authentication that bypasses MFA, or for a custom
authentication
challenge.

Type annotations and code completion for `#!python session.create_client("cognito-idp").respond_to_auth_challenge` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.respond_to_auth_challenge)

```python
# respond_to_auth_challenge method definition

await def respond_to_auth_challenge(
    self,
    *,
    ClientId: str,
    ChallengeName: ChallengeNameTypeType,  # (1)
    Session: str = ...,
    ChallengeResponses: Mapping[str, str] = ...,
    AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,  # (2)
    UserContextData: UserContextDataTypeTypeDef = ...,  # (3)
    ClientMetadata: Mapping[str, str] = ...,
) -> RespondToAuthChallengeResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ChallengeNameTypeType](./literals.md#challengenametypetype) 
2. See [:material-code-braces: AnalyticsMetadataTypeTypeDef](./type_defs.md#analyticsmetadatatypetypedef) 
3. See [:material-code-braces: UserContextDataTypeTypeDef](./type_defs.md#usercontextdatatypetypedef) 
4. See [:material-code-braces: RespondToAuthChallengeResponseTypeDef](./type_defs.md#respondtoauthchallengeresponsetypedef) 


```python
# respond_to_auth_challenge method usage example with argument unpacking

kwargs: RespondToAuthChallengeRequestRequestTypeDef = {  # (1)
    "ClientId": ...,
    "ChallengeName": ...,
}

parent.respond_to_auth_challenge(**kwargs)
```

1. See [:material-code-braces: RespondToAuthChallengeRequestRequestTypeDef](./type_defs.md#respondtoauthchallengerequestrequesttypedef) 

### revoke\_token

Revokes all of the access tokens generated by, and at the same time as, the
specified refresh
token.

Type annotations and code completion for `#!python session.create_client("cognito-idp").revoke_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.revoke_token)

```python
# revoke_token method definition

await def revoke_token(
    self,
    *,
    Token: str,
    ClientId: str,
    ClientSecret: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# revoke_token method usage example with argument unpacking

kwargs: RevokeTokenRequestRequestTypeDef = {  # (1)
    "Token": ...,
    "ClientId": ...,
}

parent.revoke_token(**kwargs)
```

1. See [:material-code-braces: RevokeTokenRequestRequestTypeDef](./type_defs.md#revoketokenrequestrequesttypedef) 

### set\_log\_delivery\_configuration

Sets up or modifies the logging configuration of a user pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").set_log_delivery_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_log_delivery_configuration)

```python
# set_log_delivery_configuration method definition

await def set_log_delivery_configuration(
    self,
    *,
    UserPoolId: str,
    LogConfigurations: Sequence[LogConfigurationTypeTypeDef],  # (1)
) -> SetLogDeliveryConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LogConfigurationTypeTypeDef](./type_defs.md#logconfigurationtypetypedef) 
2. See [:material-code-braces: SetLogDeliveryConfigurationResponseTypeDef](./type_defs.md#setlogdeliveryconfigurationresponsetypedef) 


```python
# set_log_delivery_configuration method usage example with argument unpacking

kwargs: SetLogDeliveryConfigurationRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "LogConfigurations": ...,
}

parent.set_log_delivery_configuration(**kwargs)
```

1. See [:material-code-braces: SetLogDeliveryConfigurationRequestRequestTypeDef](./type_defs.md#setlogdeliveryconfigurationrequestrequesttypedef) 

### set\_risk\_configuration

Configures actions on detected risks.

Type annotations and code completion for `#!python session.create_client("cognito-idp").set_risk_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_risk_configuration)

```python
# set_risk_configuration method definition

await def set_risk_configuration(
    self,
    *,
    UserPoolId: str,
    ClientId: str = ...,
    CompromisedCredentialsRiskConfiguration: CompromisedCredentialsRiskConfigurationTypeTypeDef = ...,  # (1)
    AccountTakeoverRiskConfiguration: AccountTakeoverRiskConfigurationTypeTypeDef = ...,  # (2)
    RiskExceptionConfiguration: RiskExceptionConfigurationTypeTypeDef = ...,  # (3)
) -> SetRiskConfigurationResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: CompromisedCredentialsRiskConfigurationTypeTypeDef](./type_defs.md#compromisedcredentialsriskconfigurationtypetypedef) 
2. See [:material-code-braces: AccountTakeoverRiskConfigurationTypeTypeDef](./type_defs.md#accounttakeoverriskconfigurationtypetypedef) 
3. See [:material-code-braces: RiskExceptionConfigurationTypeTypeDef](./type_defs.md#riskexceptionconfigurationtypetypedef) 
4. See [:material-code-braces: SetRiskConfigurationResponseTypeDef](./type_defs.md#setriskconfigurationresponsetypedef) 


```python
# set_risk_configuration method usage example with argument unpacking

kwargs: SetRiskConfigurationRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.set_risk_configuration(**kwargs)
```

1. See [:material-code-braces: SetRiskConfigurationRequestRequestTypeDef](./type_defs.md#setriskconfigurationrequestrequesttypedef) 

### set\_ui\_customization

Sets the user interface (UI) customization information for a user pool's
built-in app
UI.

Type annotations and code completion for `#!python session.create_client("cognito-idp").set_ui_customization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_ui_customization)

```python
# set_ui_customization method definition

await def set_ui_customization(
    self,
    *,
    UserPoolId: str,
    ClientId: str = ...,
    CSS: str = ...,
    ImageFile: BlobTypeDef = ...,
) -> SetUICustomizationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SetUICustomizationResponseTypeDef](./type_defs.md#setuicustomizationresponsetypedef) 


```python
# set_ui_customization method usage example with argument unpacking

kwargs: SetUICustomizationRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.set_ui_customization(**kwargs)
```

1. See [:material-code-braces: SetUICustomizationRequestRequestTypeDef](./type_defs.md#setuicustomizationrequestrequesttypedef) 

### set\_user\_mfa\_preference

Set the user's multi-factor authentication (MFA) method preference, including
which MFA factors are activated and if any are
preferred.

Type annotations and code completion for `#!python session.create_client("cognito-idp").set_user_mfa_preference` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_user_mfa_preference)

```python
# set_user_mfa_preference method definition

await def set_user_mfa_preference(
    self,
    *,
    AccessToken: str,
    SMSMfaSettings: SMSMfaSettingsTypeTypeDef = ...,  # (1)
    SoftwareTokenMfaSettings: SoftwareTokenMfaSettingsTypeTypeDef = ...,  # (2)
    EmailMfaSettings: EmailMfaSettingsTypeTypeDef = ...,  # (3)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: SMSMfaSettingsTypeTypeDef](./type_defs.md#smsmfasettingstypetypedef) 
2. See [:material-code-braces: SoftwareTokenMfaSettingsTypeTypeDef](./type_defs.md#softwaretokenmfasettingstypetypedef) 
3. See [:material-code-braces: EmailMfaSettingsTypeTypeDef](./type_defs.md#emailmfasettingstypetypedef) 


```python
# set_user_mfa_preference method usage example with argument unpacking

kwargs: SetUserMFAPreferenceRequestRequestTypeDef = {  # (1)
    "AccessToken": ...,
}

parent.set_user_mfa_preference(**kwargs)
```

1. See [:material-code-braces: SetUserMFAPreferenceRequestRequestTypeDef](./type_defs.md#setusermfapreferencerequestrequesttypedef) 

### set\_user\_pool\_mfa\_config

Sets the user pool multi-factor authentication (MFA) configuration.

Type annotations and code completion for `#!python session.create_client("cognito-idp").set_user_pool_mfa_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_user_pool_mfa_config)

```python
# set_user_pool_mfa_config method definition

await def set_user_pool_mfa_config(
    self,
    *,
    UserPoolId: str,
    SmsMfaConfiguration: SmsMfaConfigTypeTypeDef = ...,  # (1)
    SoftwareTokenMfaConfiguration: SoftwareTokenMfaConfigTypeTypeDef = ...,  # (2)
    EmailMfaConfiguration: EmailMfaConfigTypeTypeDef = ...,  # (3)
    MfaConfiguration: UserPoolMfaTypeType = ...,  # (4)
) -> SetUserPoolMfaConfigResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: SmsMfaConfigTypeTypeDef](./type_defs.md#smsmfaconfigtypetypedef) 
2. See [:material-code-braces: SoftwareTokenMfaConfigTypeTypeDef](./type_defs.md#softwaretokenmfaconfigtypetypedef) 
3. See [:material-code-braces: EmailMfaConfigTypeTypeDef](./type_defs.md#emailmfaconfigtypetypedef) 
4. See [:material-code-brackets: UserPoolMfaTypeType](./literals.md#userpoolmfatypetype) 
5. See [:material-code-braces: SetUserPoolMfaConfigResponseTypeDef](./type_defs.md#setuserpoolmfaconfigresponsetypedef) 


```python
# set_user_pool_mfa_config method usage example with argument unpacking

kwargs: SetUserPoolMfaConfigRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.set_user_pool_mfa_config(**kwargs)
```

1. See [:material-code-braces: SetUserPoolMfaConfigRequestRequestTypeDef](./type_defs.md#setuserpoolmfaconfigrequestrequesttypedef) 

### set\_user\_settings

*This action is no longer supported.* You can use it to configure only SMS MFA.

Type annotations and code completion for `#!python session.create_client("cognito-idp").set_user_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_user_settings)

```python
# set_user_settings method definition

await def set_user_settings(
    self,
    *,
    AccessToken: str,
    MFAOptions: Sequence[MFAOptionTypeTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: MFAOptionTypeTypeDef](./type_defs.md#mfaoptiontypetypedef) 


```python
# set_user_settings method usage example with argument unpacking

kwargs: SetUserSettingsRequestRequestTypeDef = {  # (1)
    "AccessToken": ...,
    "MFAOptions": ...,
}

parent.set_user_settings(**kwargs)
```

1. See [:material-code-braces: SetUserSettingsRequestRequestTypeDef](./type_defs.md#setusersettingsrequestrequesttypedef) 

### sign\_up

Registers the user in the specified user pool and creates a user name,
password, and user
attributes.

Type annotations and code completion for `#!python session.create_client("cognito-idp").sign_up` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.sign_up)

```python
# sign_up method definition

await def sign_up(
    self,
    *,
    ClientId: str,
    Username: str,
    Password: str,
    SecretHash: str = ...,
    UserAttributes: Sequence[AttributeTypeTypeDef] = ...,  # (1)
    ValidationData: Sequence[AttributeTypeTypeDef] = ...,  # (1)
    AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,  # (3)
    UserContextData: UserContextDataTypeTypeDef = ...,  # (4)
    ClientMetadata: Mapping[str, str] = ...,
) -> SignUpResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: AttributeTypeTypeDef](./type_defs.md#attributetypetypedef) 
2. See [:material-code-braces: AttributeTypeTypeDef](./type_defs.md#attributetypetypedef) 
3. See [:material-code-braces: AnalyticsMetadataTypeTypeDef](./type_defs.md#analyticsmetadatatypetypedef) 
4. See [:material-code-braces: UserContextDataTypeTypeDef](./type_defs.md#usercontextdatatypetypedef) 
5. See [:material-code-braces: SignUpResponseTypeDef](./type_defs.md#signupresponsetypedef) 


```python
# sign_up method usage example with argument unpacking

kwargs: SignUpRequestRequestTypeDef = {  # (1)
    "ClientId": ...,
    "Username": ...,
    "Password": ...,
}

parent.sign_up(**kwargs)
```

1. See [:material-code-braces: SignUpRequestRequestTypeDef](./type_defs.md#signuprequestrequesttypedef) 

### start\_user\_import\_job

Starts the user import.

Type annotations and code completion for `#!python session.create_client("cognito-idp").start_user_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.start_user_import_job)

```python
# start_user_import_job method definition

await def start_user_import_job(
    self,
    *,
    UserPoolId: str,
    JobId: str,
) -> StartUserImportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartUserImportJobResponseTypeDef](./type_defs.md#startuserimportjobresponsetypedef) 


```python
# start_user_import_job method usage example with argument unpacking

kwargs: StartUserImportJobRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "JobId": ...,
}

parent.start_user_import_job(**kwargs)
```

1. See [:material-code-braces: StartUserImportJobRequestRequestTypeDef](./type_defs.md#startuserimportjobrequestrequesttypedef) 

### stop\_user\_import\_job

Stops the user import job.

Type annotations and code completion for `#!python session.create_client("cognito-idp").stop_user_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.stop_user_import_job)

```python
# stop_user_import_job method definition

await def stop_user_import_job(
    self,
    *,
    UserPoolId: str,
    JobId: str,
) -> StopUserImportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopUserImportJobResponseTypeDef](./type_defs.md#stopuserimportjobresponsetypedef) 


```python
# stop_user_import_job method usage example with argument unpacking

kwargs: StopUserImportJobRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "JobId": ...,
}

parent.stop_user_import_job(**kwargs)
```

1. See [:material-code-braces: StopUserImportJobRequestRequestTypeDef](./type_defs.md#stopuserimportjobrequestrequesttypedef) 

### tag\_resource

Assigns a set of tags to an Amazon Cognito user pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



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

Removes the specified tags from an Amazon Cognito user pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
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

### update\_auth\_event\_feedback

Provides the feedback for an authentication event, whether it was from a valid
user or
not.

Type annotations and code completion for `#!python session.create_client("cognito-idp").update_auth_event_feedback` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_auth_event_feedback)

```python
# update_auth_event_feedback method definition

await def update_auth_event_feedback(
    self,
    *,
    UserPoolId: str,
    Username: str,
    EventId: str,
    FeedbackToken: str,
    FeedbackValue: FeedbackValueTypeType,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: FeedbackValueTypeType](./literals.md#feedbackvaluetypetype) 


```python
# update_auth_event_feedback method usage example with argument unpacking

kwargs: UpdateAuthEventFeedbackRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Username": ...,
    "EventId": ...,
    "FeedbackToken": ...,
    "FeedbackValue": ...,
}

parent.update_auth_event_feedback(**kwargs)
```

1. See [:material-code-braces: UpdateAuthEventFeedbackRequestRequestTypeDef](./type_defs.md#updateautheventfeedbackrequestrequesttypedef) 

### update\_device\_status

Updates the device status.

Type annotations and code completion for `#!python session.create_client("cognito-idp").update_device_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_device_status)

```python
# update_device_status method definition

await def update_device_status(
    self,
    *,
    AccessToken: str,
    DeviceKey: str,
    DeviceRememberedStatus: DeviceRememberedStatusTypeType = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: DeviceRememberedStatusTypeType](./literals.md#devicerememberedstatustypetype) 


```python
# update_device_status method usage example with argument unpacking

kwargs: UpdateDeviceStatusRequestRequestTypeDef = {  # (1)
    "AccessToken": ...,
    "DeviceKey": ...,
}

parent.update_device_status(**kwargs)
```

1. See [:material-code-braces: UpdateDeviceStatusRequestRequestTypeDef](./type_defs.md#updatedevicestatusrequestrequesttypedef) 

### update\_group

Updates the specified group with the specified attributes.

Type annotations and code completion for `#!python session.create_client("cognito-idp").update_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_group)

```python
# update_group method definition

await def update_group(
    self,
    *,
    GroupName: str,
    UserPoolId: str,
    Description: str = ...,
    RoleArn: str = ...,
    Precedence: int = ...,
) -> UpdateGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateGroupResponseTypeDef](./type_defs.md#updategroupresponsetypedef) 


```python
# update_group method usage example with argument unpacking

kwargs: UpdateGroupRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
    "UserPoolId": ...,
}

parent.update_group(**kwargs)
```

1. See [:material-code-braces: UpdateGroupRequestRequestTypeDef](./type_defs.md#updategrouprequestrequesttypedef) 

### update\_identity\_provider

Updates IdP information for a user pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").update_identity_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_identity_provider)

```python
# update_identity_provider method definition

await def update_identity_provider(
    self,
    *,
    UserPoolId: str,
    ProviderName: str,
    ProviderDetails: Mapping[str, str] = ...,
    AttributeMapping: Mapping[str, str] = ...,
    IdpIdentifiers: Sequence[str] = ...,
) -> UpdateIdentityProviderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateIdentityProviderResponseTypeDef](./type_defs.md#updateidentityproviderresponsetypedef) 


```python
# update_identity_provider method usage example with argument unpacking

kwargs: UpdateIdentityProviderRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "ProviderName": ...,
}

parent.update_identity_provider(**kwargs)
```

1. See [:material-code-braces: UpdateIdentityProviderRequestRequestTypeDef](./type_defs.md#updateidentityproviderrequestrequesttypedef) 

### update\_resource\_server

Updates the name and scopes of resource server.

Type annotations and code completion for `#!python session.create_client("cognito-idp").update_resource_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_resource_server)

```python
# update_resource_server method definition

await def update_resource_server(
    self,
    *,
    UserPoolId: str,
    Identifier: str,
    Name: str,
    Scopes: Sequence[ResourceServerScopeTypeTypeDef] = ...,  # (1)
) -> UpdateResourceServerResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ResourceServerScopeTypeTypeDef](./type_defs.md#resourceserverscopetypetypedef) 
2. See [:material-code-braces: UpdateResourceServerResponseTypeDef](./type_defs.md#updateresourceserverresponsetypedef) 


```python
# update_resource_server method usage example with argument unpacking

kwargs: UpdateResourceServerRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "Identifier": ...,
    "Name": ...,
}

parent.update_resource_server(**kwargs)
```

1. See [:material-code-braces: UpdateResourceServerRequestRequestTypeDef](./type_defs.md#updateresourceserverrequestrequesttypedef) 

### update\_user\_attributes

With this operation, your users can update one or more of their attributes with
their own
credentials.

Type annotations and code completion for `#!python session.create_client("cognito-idp").update_user_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_attributes)

```python
# update_user_attributes method definition

await def update_user_attributes(
    self,
    *,
    UserAttributes: Sequence[AttributeTypeTypeDef],  # (1)
    AccessToken: str,
    ClientMetadata: Mapping[str, str] = ...,
) -> UpdateUserAttributesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AttributeTypeTypeDef](./type_defs.md#attributetypetypedef) 
2. See [:material-code-braces: UpdateUserAttributesResponseTypeDef](./type_defs.md#updateuserattributesresponsetypedef) 


```python
# update_user_attributes method usage example with argument unpacking

kwargs: UpdateUserAttributesRequestRequestTypeDef = {  # (1)
    "UserAttributes": ...,
    "AccessToken": ...,
}

parent.update_user_attributes(**kwargs)
```

1. See [:material-code-braces: UpdateUserAttributesRequestRequestTypeDef](./type_defs.md#updateuserattributesrequestrequesttypedef) 

### update\_user\_pool

.

Type annotations and code completion for `#!python session.create_client("cognito-idp").update_user_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_pool)

```python
# update_user_pool method definition

await def update_user_pool(
    self,
    *,
    UserPoolId: str,
    Policies: UserPoolPolicyTypeTypeDef = ...,  # (1)
    DeletionProtection: DeletionProtectionTypeType = ...,  # (2)
    LambdaConfig: LambdaConfigTypeTypeDef = ...,  # (3)
    AutoVerifiedAttributes: Sequence[VerifiedAttributeTypeType] = ...,  # (4)
    SmsVerificationMessage: str = ...,
    EmailVerificationMessage: str = ...,
    EmailVerificationSubject: str = ...,
    VerificationMessageTemplate: VerificationMessageTemplateTypeTypeDef = ...,  # (5)
    SmsAuthenticationMessage: str = ...,
    UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeTypeDef = ...,  # (6)
    MfaConfiguration: UserPoolMfaTypeType = ...,  # (7)
    DeviceConfiguration: DeviceConfigurationTypeTypeDef = ...,  # (8)
    EmailConfiguration: EmailConfigurationTypeTypeDef = ...,  # (9)
    SmsConfiguration: SmsConfigurationTypeTypeDef = ...,  # (10)
    UserPoolTags: Mapping[str, str] = ...,
    AdminCreateUserConfig: AdminCreateUserConfigTypeTypeDef = ...,  # (11)
    UserPoolAddOns: UserPoolAddOnsTypeTypeDef = ...,  # (12)
    AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...,  # (13)
) -> Dict[str, Any]:
    ...
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


```python
# update_user_pool method usage example with argument unpacking

kwargs: UpdateUserPoolRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.update_user_pool(**kwargs)
```

1. See [:material-code-braces: UpdateUserPoolRequestRequestTypeDef](./type_defs.md#updateuserpoolrequestrequesttypedef) 

### update\_user\_pool\_client

Updates the specified user pool app client with the specified attributes.

Type annotations and code completion for `#!python session.create_client("cognito-idp").update_user_pool_client` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_pool_client)

```python
# update_user_pool_client method definition

await def update_user_pool_client(
    self,
    *,
    UserPoolId: str,
    ClientId: str,
    ClientName: str = ...,
    RefreshTokenValidity: int = ...,
    AccessTokenValidity: int = ...,
    IdTokenValidity: int = ...,
    TokenValidityUnits: TokenValidityUnitsTypeTypeDef = ...,  # (1)
    ReadAttributes: Sequence[str] = ...,
    WriteAttributes: Sequence[str] = ...,
    ExplicitAuthFlows: Sequence[ExplicitAuthFlowsTypeType] = ...,  # (2)
    SupportedIdentityProviders: Sequence[str] = ...,
    CallbackURLs: Sequence[str] = ...,
    LogoutURLs: Sequence[str] = ...,
    DefaultRedirectURI: str = ...,
    AllowedOAuthFlows: Sequence[OAuthFlowTypeType] = ...,  # (3)
    AllowedOAuthScopes: Sequence[str] = ...,
    AllowedOAuthFlowsUserPoolClient: bool = ...,
    AnalyticsConfiguration: AnalyticsConfigurationTypeTypeDef = ...,  # (4)
    PreventUserExistenceErrors: PreventUserExistenceErrorTypesType = ...,  # (5)
    EnableTokenRevocation: bool = ...,
    EnablePropagateAdditionalUserContextData: bool = ...,
    AuthSessionValidity: int = ...,
) -> UpdateUserPoolClientResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: TokenValidityUnitsTypeTypeDef](./type_defs.md#tokenvalidityunitstypetypedef) 
2. See [:material-code-brackets: ExplicitAuthFlowsTypeType](./literals.md#explicitauthflowstypetype) 
3. See [:material-code-brackets: OAuthFlowTypeType](./literals.md#oauthflowtypetype) 
4. See [:material-code-braces: AnalyticsConfigurationTypeTypeDef](./type_defs.md#analyticsconfigurationtypetypedef) 
5. See [:material-code-brackets: PreventUserExistenceErrorTypesType](./literals.md#preventuserexistenceerrortypestype) 
6. See [:material-code-braces: UpdateUserPoolClientResponseTypeDef](./type_defs.md#updateuserpoolclientresponsetypedef) 


```python
# update_user_pool_client method usage example with argument unpacking

kwargs: UpdateUserPoolClientRequestRequestTypeDef = {  # (1)
    "UserPoolId": ...,
    "ClientId": ...,
}

parent.update_user_pool_client(**kwargs)
```

1. See [:material-code-braces: UpdateUserPoolClientRequestRequestTypeDef](./type_defs.md#updateuserpoolclientrequestrequesttypedef) 

### update\_user\_pool\_domain

Updates the Secure Sockets Layer (SSL) certificate for the custom domain for
your user
pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").update_user_pool_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_pool_domain)

```python
# update_user_pool_domain method definition

await def update_user_pool_domain(
    self,
    *,
    Domain: str,
    UserPoolId: str,
    CustomDomainConfig: CustomDomainConfigTypeTypeDef,  # (1)
) -> UpdateUserPoolDomainResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CustomDomainConfigTypeTypeDef](./type_defs.md#customdomainconfigtypetypedef) 
2. See [:material-code-braces: UpdateUserPoolDomainResponseTypeDef](./type_defs.md#updateuserpooldomainresponsetypedef) 


```python
# update_user_pool_domain method usage example with argument unpacking

kwargs: UpdateUserPoolDomainRequestRequestTypeDef = {  # (1)
    "Domain": ...,
    "UserPoolId": ...,
    "CustomDomainConfig": ...,
}

parent.update_user_pool_domain(**kwargs)
```

1. See [:material-code-braces: UpdateUserPoolDomainRequestRequestTypeDef](./type_defs.md#updateuserpooldomainrequestrequesttypedef) 

### verify\_software\_token

Use this API to register a user's entered time-based one-time password (TOTP)
code and mark the user's software token MFA status as "verified" if
successful.

Type annotations and code completion for `#!python session.create_client("cognito-idp").verify_software_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.verify_software_token)

```python
# verify_software_token method definition

await def verify_software_token(
    self,
    *,
    UserCode: str,
    AccessToken: str = ...,
    Session: str = ...,
    FriendlyDeviceName: str = ...,
) -> VerifySoftwareTokenResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: VerifySoftwareTokenResponseTypeDef](./type_defs.md#verifysoftwaretokenresponsetypedef) 


```python
# verify_software_token method usage example with argument unpacking

kwargs: VerifySoftwareTokenRequestRequestTypeDef = {  # (1)
    "UserCode": ...,
}

parent.verify_software_token(**kwargs)
```

1. See [:material-code-braces: VerifySoftwareTokenRequestRequestTypeDef](./type_defs.md#verifysoftwaretokenrequestrequesttypedef) 

### verify\_user\_attribute

Verifies the specified user attributes in the user pool.

Type annotations and code completion for `#!python session.create_client("cognito-idp").verify_user_attribute` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.verify_user_attribute)

```python
# verify_user_attribute method definition

await def verify_user_attribute(
    self,
    *,
    AccessToken: str,
    AttributeName: str,
    Code: str,
) -> Dict[str, Any]:
    ...
```



```python
# verify_user_attribute method usage example with argument unpacking

kwargs: VerifyUserAttributeRequestRequestTypeDef = {  # (1)
    "AccessToken": ...,
    "AttributeName": ...,
    "Code": ...,
}

parent.verify_user_attribute(**kwargs)
```

1. See [:material-code-braces: VerifyUserAttributeRequestRequestTypeDef](./type_defs.md#verifyuserattributerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("cognito-idp").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "CognitoIdentityProviderClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("cognito-idp").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("cognito-idp").get_paginator` method with overloads.

- `client.get_paginator("admin_list_groups_for_user")` -> [AdminListGroupsForUserPaginator](./paginators.md#adminlistgroupsforuserpaginator)
- `client.get_paginator("admin_list_user_auth_events")` -> [AdminListUserAuthEventsPaginator](./paginators.md#adminlistuserautheventspaginator)
- `client.get_paginator("list_groups")` -> [ListGroupsPaginator](./paginators.md#listgroupspaginator)
- `client.get_paginator("list_identity_providers")` -> [ListIdentityProvidersPaginator](./paginators.md#listidentityproviderspaginator)
- `client.get_paginator("list_resource_servers")` -> [ListResourceServersPaginator](./paginators.md#listresourceserverspaginator)
- `client.get_paginator("list_user_pool_clients")` -> [ListUserPoolClientsPaginator](./paginators.md#listuserpoolclientspaginator)
- `client.get_paginator("list_user_pools")` -> [ListUserPoolsPaginator](./paginators.md#listuserpoolspaginator)
- `client.get_paginator("list_users")` -> [ListUsersPaginator](./paginators.md#listuserspaginator)
- `client.get_paginator("list_users_in_group")` -> [ListUsersInGroupPaginator](./paginators.md#listusersingrouppaginator)



