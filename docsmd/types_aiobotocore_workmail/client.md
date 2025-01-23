# WorkMailClient

> [Index](../README.md) > [WorkMail](./README.md) > WorkMailClient

!!! note ""

    Auto-generated documentation for [WorkMail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#workmail)
    type annotations stubs module [types-aiobotocore-workmail](https://pypi.org/project/types-aiobotocore-workmail/).

## WorkMailClient

Type annotations and code completion for `#!python session.create_client("workmail")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client)

```python
# WorkMailClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_workmail.client import WorkMailClient

session = get_session()
async with session.create_client("workmail") as client:
    client: WorkMailClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("workmail").exceptions` structure.

```python
# WorkMailClient.exceptions usage example

async with session.create_client("workmail") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.DirectoryInUseException,
        client.DirectoryServiceAuthenticationFailedException,
        client.DirectoryUnavailableException,
        client.EmailAddressInUseException,
        client.EntityAlreadyRegisteredException,
        client.EntityNotFoundException,
        client.EntityStateException,
        client.InvalidConfigurationException,
        client.InvalidCustomSesConfigurationException,
        client.InvalidParameterException,
        client.InvalidPasswordException,
        client.LimitExceededException,
        client.MailDomainInUseException,
        client.MailDomainNotFoundException,
        client.MailDomainStateException,
        client.NameAvailabilityException,
        client.OrganizationNotFoundException,
        client.OrganizationStateException,
        client.ReservedNameException,
        client.ResourceNotFoundException,
        client.TooManyTagsException,
        client.UnsupportedOperationException,
    ) as e:
        print(e)
```

```python
# WorkMailClient usage type checking example

from types_aiobotocore_workmail.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("workmail").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("workmail").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/generate_presigned_url.html)

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


### associate\_delegate\_to\_resource

Adds a member (user or group) to the resource's set of delegates.

Type annotations and code completion for `#!python session.create_client("workmail").associate_delegate_to_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/associate_delegate_to_resource.html)

```python
# associate_delegate_to_resource method definition

await def associate_delegate_to_resource(
    self,
    *,
    OrganizationId: str,
    ResourceId: str,
    EntityId: str,
) -> Dict[str, Any]:
    ...
```



```python
# associate_delegate_to_resource method usage example with argument unpacking

kwargs: AssociateDelegateToResourceRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "ResourceId": ...,
    "EntityId": ...,
}

parent.associate_delegate_to_resource(**kwargs)
```

1. See [:material-code-braces: AssociateDelegateToResourceRequestRequestTypeDef](./type_defs.md#associatedelegatetoresourcerequestrequesttypedef) 

### associate\_member\_to\_group

Adds a member (user or group) to the group's set.

Type annotations and code completion for `#!python session.create_client("workmail").associate_member_to_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/associate_member_to_group.html)

```python
# associate_member_to_group method definition

await def associate_member_to_group(
    self,
    *,
    OrganizationId: str,
    GroupId: str,
    MemberId: str,
) -> Dict[str, Any]:
    ...
```



```python
# associate_member_to_group method usage example with argument unpacking

kwargs: AssociateMemberToGroupRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "GroupId": ...,
    "MemberId": ...,
}

parent.associate_member_to_group(**kwargs)
```

1. See [:material-code-braces: AssociateMemberToGroupRequestRequestTypeDef](./type_defs.md#associatemembertogrouprequestrequesttypedef) 

### assume\_impersonation\_role

Assumes an impersonation role for the given WorkMail organization.

Type annotations and code completion for `#!python session.create_client("workmail").assume_impersonation_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/assume_impersonation_role.html)

```python
# assume_impersonation_role method definition

await def assume_impersonation_role(
    self,
    *,
    OrganizationId: str,
    ImpersonationRoleId: str,
) -> AssumeImpersonationRoleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssumeImpersonationRoleResponseTypeDef](./type_defs.md#assumeimpersonationroleresponsetypedef) 


```python
# assume_impersonation_role method usage example with argument unpacking

kwargs: AssumeImpersonationRoleRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "ImpersonationRoleId": ...,
}

parent.assume_impersonation_role(**kwargs)
```

1. See [:material-code-braces: AssumeImpersonationRoleRequestRequestTypeDef](./type_defs.md#assumeimpersonationrolerequestrequesttypedef) 

### cancel\_mailbox\_export\_job

Cancels a mailbox export job.

Type annotations and code completion for `#!python session.create_client("workmail").cancel_mailbox_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/cancel_mailbox_export_job.html)

```python
# cancel_mailbox_export_job method definition

await def cancel_mailbox_export_job(
    self,
    *,
    ClientToken: str,
    JobId: str,
    OrganizationId: str,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_mailbox_export_job method usage example with argument unpacking

kwargs: CancelMailboxExportJobRequestRequestTypeDef = {  # (1)
    "ClientToken": ...,
    "JobId": ...,
    "OrganizationId": ...,
}

parent.cancel_mailbox_export_job(**kwargs)
```

1. See [:material-code-braces: CancelMailboxExportJobRequestRequestTypeDef](./type_defs.md#cancelmailboxexportjobrequestrequesttypedef) 

### create\_alias

Adds an alias to the set of a given member (user or group) of WorkMail.

Type annotations and code completion for `#!python session.create_client("workmail").create_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/create_alias.html)

```python
# create_alias method definition

await def create_alias(
    self,
    *,
    OrganizationId: str,
    EntityId: str,
    Alias: str,
) -> Dict[str, Any]:
    ...
```



```python
# create_alias method usage example with argument unpacking

kwargs: CreateAliasRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "EntityId": ...,
    "Alias": ...,
}

parent.create_alias(**kwargs)
```

1. See [:material-code-braces: CreateAliasRequestRequestTypeDef](./type_defs.md#createaliasrequestrequesttypedef) 

### create\_availability\_configuration

Creates an <code>AvailabilityConfiguration</code> for the given WorkMail
organization and domain.

Type annotations and code completion for `#!python session.create_client("workmail").create_availability_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/create_availability_configuration.html)

```python
# create_availability_configuration method definition

await def create_availability_configuration(
    self,
    *,
    OrganizationId: str,
    DomainName: str,
    ClientToken: str = ...,
    EwsProvider: EwsAvailabilityProviderTypeDef = ...,  # (1)
    LambdaProvider: LambdaAvailabilityProviderTypeDef = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: EwsAvailabilityProviderTypeDef](./type_defs.md#ewsavailabilityprovidertypedef) 
2. See [:material-code-braces: LambdaAvailabilityProviderTypeDef](./type_defs.md#lambdaavailabilityprovidertypedef) 


```python
# create_availability_configuration method usage example with argument unpacking

kwargs: CreateAvailabilityConfigurationRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "DomainName": ...,
}

parent.create_availability_configuration(**kwargs)
```

1. See [:material-code-braces: CreateAvailabilityConfigurationRequestRequestTypeDef](./type_defs.md#createavailabilityconfigurationrequestrequesttypedef) 

### create\_group

Creates a group that can be used in WorkMail by calling the
<a>RegisterToWorkMail</a> operation.

Type annotations and code completion for `#!python session.create_client("workmail").create_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/create_group.html)

```python
# create_group method definition

await def create_group(
    self,
    *,
    OrganizationId: str,
    Name: str,
    HiddenFromGlobalAddressList: bool = ...,
) -> CreateGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateGroupResponseTypeDef](./type_defs.md#creategroupresponsetypedef) 


```python
# create_group method usage example with argument unpacking

kwargs: CreateGroupRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "Name": ...,
}

parent.create_group(**kwargs)
```

1. See [:material-code-braces: CreateGroupRequestRequestTypeDef](./type_defs.md#creategrouprequestrequesttypedef) 

### create\_identity\_center\_application

Creates the WorkMail application in IAM Identity Center that can be used later
in the WorkMail - IdC integration.

Type annotations and code completion for `#!python session.create_client("workmail").create_identity_center_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/create_identity_center_application.html)

```python
# create_identity_center_application method definition

await def create_identity_center_application(
    self,
    *,
    Name: str,
    InstanceArn: str,
    ClientToken: str = ...,
) -> CreateIdentityCenterApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateIdentityCenterApplicationResponseTypeDef](./type_defs.md#createidentitycenterapplicationresponsetypedef) 


```python
# create_identity_center_application method usage example with argument unpacking

kwargs: CreateIdentityCenterApplicationRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "InstanceArn": ...,
}

parent.create_identity_center_application(**kwargs)
```

1. See [:material-code-braces: CreateIdentityCenterApplicationRequestRequestTypeDef](./type_defs.md#createidentitycenterapplicationrequestrequesttypedef) 

### create\_impersonation\_role

Creates an impersonation role for the given WorkMail organization.

Type annotations and code completion for `#!python session.create_client("workmail").create_impersonation_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/create_impersonation_role.html)

```python
# create_impersonation_role method definition

await def create_impersonation_role(
    self,
    *,
    OrganizationId: str,
    Name: str,
    Type: ImpersonationRoleTypeType,  # (1)
    Rules: Sequence[ImpersonationRuleUnionTypeDef],  # (2)
    ClientToken: str = ...,
    Description: str = ...,
) -> CreateImpersonationRoleResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ImpersonationRoleTypeType](./literals.md#impersonationroletypetype) 
2. See [:material-code-braces: ImpersonationRuleTypeDef](./type_defs.md#impersonationruletypedef) [:material-code-braces: ImpersonationRuleOutputTypeDef](./type_defs.md#impersonationruleoutputtypedef) 
3. See [:material-code-braces: CreateImpersonationRoleResponseTypeDef](./type_defs.md#createimpersonationroleresponsetypedef) 


```python
# create_impersonation_role method usage example with argument unpacking

kwargs: CreateImpersonationRoleRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "Name": ...,
    "Type": ...,
    "Rules": ...,
}

parent.create_impersonation_role(**kwargs)
```

1. See [:material-code-braces: CreateImpersonationRoleRequestRequestTypeDef](./type_defs.md#createimpersonationrolerequestrequesttypedef) 

### create\_mobile\_device\_access\_rule

Creates a new mobile device access rule for the specified WorkMail organization.

Type annotations and code completion for `#!python session.create_client("workmail").create_mobile_device_access_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/create_mobile_device_access_rule.html)

```python
# create_mobile_device_access_rule method definition

await def create_mobile_device_access_rule(
    self,
    *,
    OrganizationId: str,
    Name: str,
    Effect: MobileDeviceAccessRuleEffectType,  # (1)
    ClientToken: str = ...,
    Description: str = ...,
    DeviceTypes: Sequence[str] = ...,
    NotDeviceTypes: Sequence[str] = ...,
    DeviceModels: Sequence[str] = ...,
    NotDeviceModels: Sequence[str] = ...,
    DeviceOperatingSystems: Sequence[str] = ...,
    NotDeviceOperatingSystems: Sequence[str] = ...,
    DeviceUserAgents: Sequence[str] = ...,
    NotDeviceUserAgents: Sequence[str] = ...,
) -> CreateMobileDeviceAccessRuleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MobileDeviceAccessRuleEffectType](./literals.md#mobiledeviceaccessruleeffecttype) 
2. See [:material-code-braces: CreateMobileDeviceAccessRuleResponseTypeDef](./type_defs.md#createmobiledeviceaccessruleresponsetypedef) 


```python
# create_mobile_device_access_rule method usage example with argument unpacking

kwargs: CreateMobileDeviceAccessRuleRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "Name": ...,
    "Effect": ...,
}

parent.create_mobile_device_access_rule(**kwargs)
```

1. See [:material-code-braces: CreateMobileDeviceAccessRuleRequestRequestTypeDef](./type_defs.md#createmobiledeviceaccessrulerequestrequesttypedef) 

### create\_organization

Creates a new WorkMail organization.

Type annotations and code completion for `#!python session.create_client("workmail").create_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/create_organization.html)

```python
# create_organization method definition

await def create_organization(
    self,
    *,
    Alias: str,
    DirectoryId: str = ...,
    ClientToken: str = ...,
    Domains: Sequence[DomainTypeDef] = ...,  # (1)
    KmsKeyArn: str = ...,
    EnableInteroperability: bool = ...,
) -> CreateOrganizationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DomainTypeDef](./type_defs.md#domaintypedef) 
2. See [:material-code-braces: CreateOrganizationResponseTypeDef](./type_defs.md#createorganizationresponsetypedef) 


```python
# create_organization method usage example with argument unpacking

kwargs: CreateOrganizationRequestRequestTypeDef = {  # (1)
    "Alias": ...,
}

parent.create_organization(**kwargs)
```

1. See [:material-code-braces: CreateOrganizationRequestRequestTypeDef](./type_defs.md#createorganizationrequestrequesttypedef) 

### create\_resource

Creates a new WorkMail resource.

Type annotations and code completion for `#!python session.create_client("workmail").create_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/create_resource.html)

```python
# create_resource method definition

await def create_resource(
    self,
    *,
    OrganizationId: str,
    Name: str,
    Type: ResourceTypeType,  # (1)
    Description: str = ...,
    HiddenFromGlobalAddressList: bool = ...,
) -> CreateResourceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: CreateResourceResponseTypeDef](./type_defs.md#createresourceresponsetypedef) 


```python
# create_resource method usage example with argument unpacking

kwargs: CreateResourceRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "Name": ...,
    "Type": ...,
}

parent.create_resource(**kwargs)
```

1. See [:material-code-braces: CreateResourceRequestRequestTypeDef](./type_defs.md#createresourcerequestrequesttypedef) 

### create\_user

Creates a user who can be used in WorkMail by calling the
<a>RegisterToWorkMail</a> operation.

Type annotations and code completion for `#!python session.create_client("workmail").create_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/create_user.html)

```python
# create_user method definition

await def create_user(
    self,
    *,
    OrganizationId: str,
    Name: str,
    DisplayName: str,
    Password: str = ...,
    Role: UserRoleType = ...,  # (1)
    FirstName: str = ...,
    LastName: str = ...,
    HiddenFromGlobalAddressList: bool = ...,
    IdentityProviderUserId: str = ...,
) -> CreateUserResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: UserRoleType](./literals.md#userroletype) 
2. See [:material-code-braces: CreateUserResponseTypeDef](./type_defs.md#createuserresponsetypedef) 


```python
# create_user method usage example with argument unpacking

kwargs: CreateUserRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "Name": ...,
    "DisplayName": ...,
}

parent.create_user(**kwargs)
```

1. See [:material-code-braces: CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef) 

### delete\_access\_control\_rule

Deletes an access control rule for the specified WorkMail organization.

Type annotations and code completion for `#!python session.create_client("workmail").delete_access_control_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/delete_access_control_rule.html)

```python
# delete_access_control_rule method definition

await def delete_access_control_rule(
    self,
    *,
    OrganizationId: str,
    Name: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_access_control_rule method usage example with argument unpacking

kwargs: DeleteAccessControlRuleRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "Name": ...,
}

parent.delete_access_control_rule(**kwargs)
```

1. See [:material-code-braces: DeleteAccessControlRuleRequestRequestTypeDef](./type_defs.md#deleteaccesscontrolrulerequestrequesttypedef) 

### delete\_alias

Remove one or more specified aliases from a set of aliases for a given user.

Type annotations and code completion for `#!python session.create_client("workmail").delete_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/delete_alias.html)

```python
# delete_alias method definition

await def delete_alias(
    self,
    *,
    OrganizationId: str,
    EntityId: str,
    Alias: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_alias method usage example with argument unpacking

kwargs: DeleteAliasRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "EntityId": ...,
    "Alias": ...,
}

parent.delete_alias(**kwargs)
```

1. See [:material-code-braces: DeleteAliasRequestRequestTypeDef](./type_defs.md#deletealiasrequestrequesttypedef) 

### delete\_availability\_configuration

Deletes the <code>AvailabilityConfiguration</code> for the given WorkMail
organization and domain.

Type annotations and code completion for `#!python session.create_client("workmail").delete_availability_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/delete_availability_configuration.html)

```python
# delete_availability_configuration method definition

await def delete_availability_configuration(
    self,
    *,
    OrganizationId: str,
    DomainName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_availability_configuration method usage example with argument unpacking

kwargs: DeleteAvailabilityConfigurationRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "DomainName": ...,
}

parent.delete_availability_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteAvailabilityConfigurationRequestRequestTypeDef](./type_defs.md#deleteavailabilityconfigurationrequestrequesttypedef) 

### delete\_email\_monitoring\_configuration

Deletes the email monitoring configuration for a specified organization.

Type annotations and code completion for `#!python session.create_client("workmail").delete_email_monitoring_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/delete_email_monitoring_configuration.html)

```python
# delete_email_monitoring_configuration method definition

await def delete_email_monitoring_configuration(
    self,
    *,
    OrganizationId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_email_monitoring_configuration method usage example with argument unpacking

kwargs: DeleteEmailMonitoringConfigurationRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.delete_email_monitoring_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteEmailMonitoringConfigurationRequestRequestTypeDef](./type_defs.md#deleteemailmonitoringconfigurationrequestrequesttypedef) 

### delete\_group

Deletes a group from WorkMail.

Type annotations and code completion for `#!python session.create_client("workmail").delete_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/delete_group.html)

```python
# delete_group method definition

await def delete_group(
    self,
    *,
    OrganizationId: str,
    GroupId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_group method usage example with argument unpacking

kwargs: DeleteGroupRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "GroupId": ...,
}

parent.delete_group(**kwargs)
```

1. See [:material-code-braces: DeleteGroupRequestRequestTypeDef](./type_defs.md#deletegrouprequestrequesttypedef) 

### delete\_identity\_center\_application

Deletes the IAM Identity Center application from WorkMail.

Type annotations and code completion for `#!python session.create_client("workmail").delete_identity_center_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/delete_identity_center_application.html)

```python
# delete_identity_center_application method definition

await def delete_identity_center_application(
    self,
    *,
    ApplicationArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_identity_center_application method usage example with argument unpacking

kwargs: DeleteIdentityCenterApplicationRequestRequestTypeDef = {  # (1)
    "ApplicationArn": ...,
}

parent.delete_identity_center_application(**kwargs)
```

1. See [:material-code-braces: DeleteIdentityCenterApplicationRequestRequestTypeDef](./type_defs.md#deleteidentitycenterapplicationrequestrequesttypedef) 

### delete\_identity\_provider\_configuration

Disables the integration between IdC and WorkMail.

Type annotations and code completion for `#!python session.create_client("workmail").delete_identity_provider_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/delete_identity_provider_configuration.html)

```python
# delete_identity_provider_configuration method definition

await def delete_identity_provider_configuration(
    self,
    *,
    OrganizationId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_identity_provider_configuration method usage example with argument unpacking

kwargs: DeleteIdentityProviderConfigurationRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.delete_identity_provider_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteIdentityProviderConfigurationRequestRequestTypeDef](./type_defs.md#deleteidentityproviderconfigurationrequestrequesttypedef) 

### delete\_impersonation\_role

Deletes an impersonation role for the given WorkMail organization.

Type annotations and code completion for `#!python session.create_client("workmail").delete_impersonation_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/delete_impersonation_role.html)

```python
# delete_impersonation_role method definition

await def delete_impersonation_role(
    self,
    *,
    OrganizationId: str,
    ImpersonationRoleId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_impersonation_role method usage example with argument unpacking

kwargs: DeleteImpersonationRoleRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "ImpersonationRoleId": ...,
}

parent.delete_impersonation_role(**kwargs)
```

1. See [:material-code-braces: DeleteImpersonationRoleRequestRequestTypeDef](./type_defs.md#deleteimpersonationrolerequestrequesttypedef) 

### delete\_mailbox\_permissions

Deletes permissions granted to a member (user or group).

Type annotations and code completion for `#!python session.create_client("workmail").delete_mailbox_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/delete_mailbox_permissions.html)

```python
# delete_mailbox_permissions method definition

await def delete_mailbox_permissions(
    self,
    *,
    OrganizationId: str,
    EntityId: str,
    GranteeId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_mailbox_permissions method usage example with argument unpacking

kwargs: DeleteMailboxPermissionsRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "EntityId": ...,
    "GranteeId": ...,
}

parent.delete_mailbox_permissions(**kwargs)
```

1. See [:material-code-braces: DeleteMailboxPermissionsRequestRequestTypeDef](./type_defs.md#deletemailboxpermissionsrequestrequesttypedef) 

### delete\_mobile\_device\_access\_override

Deletes the mobile device access override for the given WorkMail organization,
user, and device.

Type annotations and code completion for `#!python session.create_client("workmail").delete_mobile_device_access_override` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/delete_mobile_device_access_override.html)

```python
# delete_mobile_device_access_override method definition

await def delete_mobile_device_access_override(
    self,
    *,
    OrganizationId: str,
    UserId: str,
    DeviceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_mobile_device_access_override method usage example with argument unpacking

kwargs: DeleteMobileDeviceAccessOverrideRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "UserId": ...,
    "DeviceId": ...,
}

parent.delete_mobile_device_access_override(**kwargs)
```

1. See [:material-code-braces: DeleteMobileDeviceAccessOverrideRequestRequestTypeDef](./type_defs.md#deletemobiledeviceaccessoverriderequestrequesttypedef) 

### delete\_mobile\_device\_access\_rule

Deletes a mobile device access rule for the specified WorkMail organization.

Type annotations and code completion for `#!python session.create_client("workmail").delete_mobile_device_access_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/delete_mobile_device_access_rule.html)

```python
# delete_mobile_device_access_rule method definition

await def delete_mobile_device_access_rule(
    self,
    *,
    OrganizationId: str,
    MobileDeviceAccessRuleId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_mobile_device_access_rule method usage example with argument unpacking

kwargs: DeleteMobileDeviceAccessRuleRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "MobileDeviceAccessRuleId": ...,
}

parent.delete_mobile_device_access_rule(**kwargs)
```

1. See [:material-code-braces: DeleteMobileDeviceAccessRuleRequestRequestTypeDef](./type_defs.md#deletemobiledeviceaccessrulerequestrequesttypedef) 

### delete\_organization

Deletes an WorkMail organization and all underlying AWS resources managed by
WorkMail as part of the organization.

Type annotations and code completion for `#!python session.create_client("workmail").delete_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/delete_organization.html)

```python
# delete_organization method definition

await def delete_organization(
    self,
    *,
    OrganizationId: str,
    DeleteDirectory: bool,
    ClientToken: str = ...,
    ForceDelete: bool = ...,
    DeleteIdentityCenterApplication: bool = ...,
) -> DeleteOrganizationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteOrganizationResponseTypeDef](./type_defs.md#deleteorganizationresponsetypedef) 


```python
# delete_organization method usage example with argument unpacking

kwargs: DeleteOrganizationRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "DeleteDirectory": ...,
}

parent.delete_organization(**kwargs)
```

1. See [:material-code-braces: DeleteOrganizationRequestRequestTypeDef](./type_defs.md#deleteorganizationrequestrequesttypedef) 

### delete\_personal\_access\_token

Deletes the Personal Access Token from the provided WorkMail Organization.

Type annotations and code completion for `#!python session.create_client("workmail").delete_personal_access_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/delete_personal_access_token.html)

```python
# delete_personal_access_token method definition

await def delete_personal_access_token(
    self,
    *,
    OrganizationId: str,
    PersonalAccessTokenId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_personal_access_token method usage example with argument unpacking

kwargs: DeletePersonalAccessTokenRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "PersonalAccessTokenId": ...,
}

parent.delete_personal_access_token(**kwargs)
```

1. See [:material-code-braces: DeletePersonalAccessTokenRequestRequestTypeDef](./type_defs.md#deletepersonalaccesstokenrequestrequesttypedef) 

### delete\_resource

Deletes the specified resource.

Type annotations and code completion for `#!python session.create_client("workmail").delete_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/delete_resource.html)

```python
# delete_resource method definition

await def delete_resource(
    self,
    *,
    OrganizationId: str,
    ResourceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_resource method usage example with argument unpacking

kwargs: DeleteResourceRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "ResourceId": ...,
}

parent.delete_resource(**kwargs)
```

1. See [:material-code-braces: DeleteResourceRequestRequestTypeDef](./type_defs.md#deleteresourcerequestrequesttypedef) 

### delete\_retention\_policy

Deletes the specified retention policy from the specified organization.

Type annotations and code completion for `#!python session.create_client("workmail").delete_retention_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/delete_retention_policy.html)

```python
# delete_retention_policy method definition

await def delete_retention_policy(
    self,
    *,
    OrganizationId: str,
    Id: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_retention_policy method usage example with argument unpacking

kwargs: DeleteRetentionPolicyRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "Id": ...,
}

parent.delete_retention_policy(**kwargs)
```

1. See [:material-code-braces: DeleteRetentionPolicyRequestRequestTypeDef](./type_defs.md#deleteretentionpolicyrequestrequesttypedef) 

### delete\_user

Deletes a user from WorkMail and all subsequent systems.

Type annotations and code completion for `#!python session.create_client("workmail").delete_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/delete_user.html)

```python
# delete_user method definition

await def delete_user(
    self,
    *,
    OrganizationId: str,
    UserId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_user method usage example with argument unpacking

kwargs: DeleteUserRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "UserId": ...,
}

parent.delete_user(**kwargs)
```

1. See [:material-code-braces: DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef) 

### deregister\_from\_work\_mail

Mark a user, group, or resource as no longer used in WorkMail.

Type annotations and code completion for `#!python session.create_client("workmail").deregister_from_work_mail` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/deregister_from_work_mail.html)

```python
# deregister_from_work_mail method definition

await def deregister_from_work_mail(
    self,
    *,
    OrganizationId: str,
    EntityId: str,
) -> Dict[str, Any]:
    ...
```



```python
# deregister_from_work_mail method usage example with argument unpacking

kwargs: DeregisterFromWorkMailRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "EntityId": ...,
}

parent.deregister_from_work_mail(**kwargs)
```

1. See [:material-code-braces: DeregisterFromWorkMailRequestRequestTypeDef](./type_defs.md#deregisterfromworkmailrequestrequesttypedef) 

### deregister\_mail\_domain

Removes a domain from WorkMail, stops email routing to WorkMail, and removes
the authorization allowing WorkMail use.

Type annotations and code completion for `#!python session.create_client("workmail").deregister_mail_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/deregister_mail_domain.html)

```python
# deregister_mail_domain method definition

await def deregister_mail_domain(
    self,
    *,
    OrganizationId: str,
    DomainName: str,
) -> Dict[str, Any]:
    ...
```



```python
# deregister_mail_domain method usage example with argument unpacking

kwargs: DeregisterMailDomainRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "DomainName": ...,
}

parent.deregister_mail_domain(**kwargs)
```

1. See [:material-code-braces: DeregisterMailDomainRequestRequestTypeDef](./type_defs.md#deregistermaildomainrequestrequesttypedef) 

### describe\_email\_monitoring\_configuration

Describes the current email monitoring configuration for a specified
organization.

Type annotations and code completion for `#!python session.create_client("workmail").describe_email_monitoring_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/describe_email_monitoring_configuration.html)

```python
# describe_email_monitoring_configuration method definition

await def describe_email_monitoring_configuration(
    self,
    *,
    OrganizationId: str,
) -> DescribeEmailMonitoringConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEmailMonitoringConfigurationResponseTypeDef](./type_defs.md#describeemailmonitoringconfigurationresponsetypedef) 


```python
# describe_email_monitoring_configuration method usage example with argument unpacking

kwargs: DescribeEmailMonitoringConfigurationRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.describe_email_monitoring_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeEmailMonitoringConfigurationRequestRequestTypeDef](./type_defs.md#describeemailmonitoringconfigurationrequestrequesttypedef) 

### describe\_entity

Returns basic details about an entity in WorkMail.

Type annotations and code completion for `#!python session.create_client("workmail").describe_entity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/describe_entity.html)

```python
# describe_entity method definition

await def describe_entity(
    self,
    *,
    OrganizationId: str,
    Email: str,
) -> DescribeEntityResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEntityResponseTypeDef](./type_defs.md#describeentityresponsetypedef) 


```python
# describe_entity method usage example with argument unpacking

kwargs: DescribeEntityRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "Email": ...,
}

parent.describe_entity(**kwargs)
```

1. See [:material-code-braces: DescribeEntityRequestRequestTypeDef](./type_defs.md#describeentityrequestrequesttypedef) 

### describe\_group

Returns the data available for the group.

Type annotations and code completion for `#!python session.create_client("workmail").describe_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/describe_group.html)

```python
# describe_group method definition

await def describe_group(
    self,
    *,
    OrganizationId: str,
    GroupId: str,
) -> DescribeGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeGroupResponseTypeDef](./type_defs.md#describegroupresponsetypedef) 


```python
# describe_group method usage example with argument unpacking

kwargs: DescribeGroupRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "GroupId": ...,
}

parent.describe_group(**kwargs)
```

1. See [:material-code-braces: DescribeGroupRequestRequestTypeDef](./type_defs.md#describegrouprequestrequesttypedef) 

### describe\_identity\_provider\_configuration

Returns detailed information on the current IdC setup for the WorkMail
organization.

Type annotations and code completion for `#!python session.create_client("workmail").describe_identity_provider_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/describe_identity_provider_configuration.html)

```python
# describe_identity_provider_configuration method definition

await def describe_identity_provider_configuration(
    self,
    *,
    OrganizationId: str,
) -> DescribeIdentityProviderConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeIdentityProviderConfigurationResponseTypeDef](./type_defs.md#describeidentityproviderconfigurationresponsetypedef) 


```python
# describe_identity_provider_configuration method usage example with argument unpacking

kwargs: DescribeIdentityProviderConfigurationRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.describe_identity_provider_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeIdentityProviderConfigurationRequestRequestTypeDef](./type_defs.md#describeidentityproviderconfigurationrequestrequesttypedef) 

### describe\_inbound\_dmarc\_settings

Lists the settings in a DMARC policy for a specified organization.

Type annotations and code completion for `#!python session.create_client("workmail").describe_inbound_dmarc_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/describe_inbound_dmarc_settings.html)

```python
# describe_inbound_dmarc_settings method definition

await def describe_inbound_dmarc_settings(
    self,
    *,
    OrganizationId: str,
) -> DescribeInboundDmarcSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeInboundDmarcSettingsResponseTypeDef](./type_defs.md#describeinbounddmarcsettingsresponsetypedef) 


```python
# describe_inbound_dmarc_settings method usage example with argument unpacking

kwargs: DescribeInboundDmarcSettingsRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.describe_inbound_dmarc_settings(**kwargs)
```

1. See [:material-code-braces: DescribeInboundDmarcSettingsRequestRequestTypeDef](./type_defs.md#describeinbounddmarcsettingsrequestrequesttypedef) 

### describe\_mailbox\_export\_job

Describes the current status of a mailbox export job.

Type annotations and code completion for `#!python session.create_client("workmail").describe_mailbox_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/describe_mailbox_export_job.html)

```python
# describe_mailbox_export_job method definition

await def describe_mailbox_export_job(
    self,
    *,
    JobId: str,
    OrganizationId: str,
) -> DescribeMailboxExportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeMailboxExportJobResponseTypeDef](./type_defs.md#describemailboxexportjobresponsetypedef) 


```python
# describe_mailbox_export_job method usage example with argument unpacking

kwargs: DescribeMailboxExportJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
    "OrganizationId": ...,
}

parent.describe_mailbox_export_job(**kwargs)
```

1. See [:material-code-braces: DescribeMailboxExportJobRequestRequestTypeDef](./type_defs.md#describemailboxexportjobrequestrequesttypedef) 

### describe\_organization

Provides more information regarding a given organization based on its
identifier.

Type annotations and code completion for `#!python session.create_client("workmail").describe_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/describe_organization.html)

```python
# describe_organization method definition

await def describe_organization(
    self,
    *,
    OrganizationId: str,
) -> DescribeOrganizationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeOrganizationResponseTypeDef](./type_defs.md#describeorganizationresponsetypedef) 


```python
# describe_organization method usage example with argument unpacking

kwargs: DescribeOrganizationRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.describe_organization(**kwargs)
```

1. See [:material-code-braces: DescribeOrganizationRequestRequestTypeDef](./type_defs.md#describeorganizationrequestrequesttypedef) 

### describe\_resource

Returns the data available for the resource.

Type annotations and code completion for `#!python session.create_client("workmail").describe_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/describe_resource.html)

```python
# describe_resource method definition

await def describe_resource(
    self,
    *,
    OrganizationId: str,
    ResourceId: str,
) -> DescribeResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeResourceResponseTypeDef](./type_defs.md#describeresourceresponsetypedef) 


```python
# describe_resource method usage example with argument unpacking

kwargs: DescribeResourceRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "ResourceId": ...,
}

parent.describe_resource(**kwargs)
```

1. See [:material-code-braces: DescribeResourceRequestRequestTypeDef](./type_defs.md#describeresourcerequestrequesttypedef) 

### describe\_user

Provides information regarding the user.

Type annotations and code completion for `#!python session.create_client("workmail").describe_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/describe_user.html)

```python
# describe_user method definition

await def describe_user(
    self,
    *,
    OrganizationId: str,
    UserId: str,
) -> DescribeUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeUserResponseTypeDef](./type_defs.md#describeuserresponsetypedef) 


```python
# describe_user method usage example with argument unpacking

kwargs: DescribeUserRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "UserId": ...,
}

parent.describe_user(**kwargs)
```

1. See [:material-code-braces: DescribeUserRequestRequestTypeDef](./type_defs.md#describeuserrequestrequesttypedef) 

### disassociate\_delegate\_from\_resource

Removes a member from the resource's set of delegates.

Type annotations and code completion for `#!python session.create_client("workmail").disassociate_delegate_from_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/disassociate_delegate_from_resource.html)

```python
# disassociate_delegate_from_resource method definition

await def disassociate_delegate_from_resource(
    self,
    *,
    OrganizationId: str,
    ResourceId: str,
    EntityId: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_delegate_from_resource method usage example with argument unpacking

kwargs: DisassociateDelegateFromResourceRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "ResourceId": ...,
    "EntityId": ...,
}

parent.disassociate_delegate_from_resource(**kwargs)
```

1. See [:material-code-braces: DisassociateDelegateFromResourceRequestRequestTypeDef](./type_defs.md#disassociatedelegatefromresourcerequestrequesttypedef) 

### disassociate\_member\_from\_group

Removes a member from a group.

Type annotations and code completion for `#!python session.create_client("workmail").disassociate_member_from_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/disassociate_member_from_group.html)

```python
# disassociate_member_from_group method definition

await def disassociate_member_from_group(
    self,
    *,
    OrganizationId: str,
    GroupId: str,
    MemberId: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_member_from_group method usage example with argument unpacking

kwargs: DisassociateMemberFromGroupRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "GroupId": ...,
    "MemberId": ...,
}

parent.disassociate_member_from_group(**kwargs)
```

1. See [:material-code-braces: DisassociateMemberFromGroupRequestRequestTypeDef](./type_defs.md#disassociatememberfromgrouprequestrequesttypedef) 

### get\_access\_control\_effect

Gets the effects of an organization's access control rules as they apply to a
specified IPv4 address, access protocol action, and user ID or impersonation
role ID.

Type annotations and code completion for `#!python session.create_client("workmail").get_access_control_effect` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/get_access_control_effect.html)

```python
# get_access_control_effect method definition

await def get_access_control_effect(
    self,
    *,
    OrganizationId: str,
    IpAddress: str,
    Action: str,
    UserId: str = ...,
    ImpersonationRoleId: str = ...,
) -> GetAccessControlEffectResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccessControlEffectResponseTypeDef](./type_defs.md#getaccesscontroleffectresponsetypedef) 


```python
# get_access_control_effect method usage example with argument unpacking

kwargs: GetAccessControlEffectRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "IpAddress": ...,
    "Action": ...,
}

parent.get_access_control_effect(**kwargs)
```

1. See [:material-code-braces: GetAccessControlEffectRequestRequestTypeDef](./type_defs.md#getaccesscontroleffectrequestrequesttypedef) 

### get\_default\_retention\_policy

Gets the default retention policy details for the specified organization.

Type annotations and code completion for `#!python session.create_client("workmail").get_default_retention_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/get_default_retention_policy.html)

```python
# get_default_retention_policy method definition

await def get_default_retention_policy(
    self,
    *,
    OrganizationId: str,
) -> GetDefaultRetentionPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDefaultRetentionPolicyResponseTypeDef](./type_defs.md#getdefaultretentionpolicyresponsetypedef) 


```python
# get_default_retention_policy method usage example with argument unpacking

kwargs: GetDefaultRetentionPolicyRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.get_default_retention_policy(**kwargs)
```

1. See [:material-code-braces: GetDefaultRetentionPolicyRequestRequestTypeDef](./type_defs.md#getdefaultretentionpolicyrequestrequesttypedef) 

### get\_impersonation\_role

Gets the impersonation role details for the given WorkMail organization.

Type annotations and code completion for `#!python session.create_client("workmail").get_impersonation_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/get_impersonation_role.html)

```python
# get_impersonation_role method definition

await def get_impersonation_role(
    self,
    *,
    OrganizationId: str,
    ImpersonationRoleId: str,
) -> GetImpersonationRoleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetImpersonationRoleResponseTypeDef](./type_defs.md#getimpersonationroleresponsetypedef) 


```python
# get_impersonation_role method usage example with argument unpacking

kwargs: GetImpersonationRoleRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "ImpersonationRoleId": ...,
}

parent.get_impersonation_role(**kwargs)
```

1. See [:material-code-braces: GetImpersonationRoleRequestRequestTypeDef](./type_defs.md#getimpersonationrolerequestrequesttypedef) 

### get\_impersonation\_role\_effect

Tests whether the given impersonation role can impersonate a target user.

Type annotations and code completion for `#!python session.create_client("workmail").get_impersonation_role_effect` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/get_impersonation_role_effect.html)

```python
# get_impersonation_role_effect method definition

await def get_impersonation_role_effect(
    self,
    *,
    OrganizationId: str,
    ImpersonationRoleId: str,
    TargetUser: str,
) -> GetImpersonationRoleEffectResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetImpersonationRoleEffectResponseTypeDef](./type_defs.md#getimpersonationroleeffectresponsetypedef) 


```python
# get_impersonation_role_effect method usage example with argument unpacking

kwargs: GetImpersonationRoleEffectRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "ImpersonationRoleId": ...,
    "TargetUser": ...,
}

parent.get_impersonation_role_effect(**kwargs)
```

1. See [:material-code-braces: GetImpersonationRoleEffectRequestRequestTypeDef](./type_defs.md#getimpersonationroleeffectrequestrequesttypedef) 

### get\_mail\_domain

Gets details for a mail domain, including domain records required to configure
your domain with recommended security.

Type annotations and code completion for `#!python session.create_client("workmail").get_mail_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/get_mail_domain.html)

```python
# get_mail_domain method definition

await def get_mail_domain(
    self,
    *,
    OrganizationId: str,
    DomainName: str,
) -> GetMailDomainResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMailDomainResponseTypeDef](./type_defs.md#getmaildomainresponsetypedef) 


```python
# get_mail_domain method usage example with argument unpacking

kwargs: GetMailDomainRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "DomainName": ...,
}

parent.get_mail_domain(**kwargs)
```

1. See [:material-code-braces: GetMailDomainRequestRequestTypeDef](./type_defs.md#getmaildomainrequestrequesttypedef) 

### get\_mailbox\_details

Requests a user's mailbox details for a specified organization and user.

Type annotations and code completion for `#!python session.create_client("workmail").get_mailbox_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/get_mailbox_details.html)

```python
# get_mailbox_details method definition

await def get_mailbox_details(
    self,
    *,
    OrganizationId: str,
    UserId: str,
) -> GetMailboxDetailsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMailboxDetailsResponseTypeDef](./type_defs.md#getmailboxdetailsresponsetypedef) 


```python
# get_mailbox_details method usage example with argument unpacking

kwargs: GetMailboxDetailsRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "UserId": ...,
}

parent.get_mailbox_details(**kwargs)
```

1. See [:material-code-braces: GetMailboxDetailsRequestRequestTypeDef](./type_defs.md#getmailboxdetailsrequestrequesttypedef) 

### get\_mobile\_device\_access\_effect

Simulates the effect of the mobile device access rules for the given attributes
of a sample access event.

Type annotations and code completion for `#!python session.create_client("workmail").get_mobile_device_access_effect` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/get_mobile_device_access_effect.html)

```python
# get_mobile_device_access_effect method definition

await def get_mobile_device_access_effect(
    self,
    *,
    OrganizationId: str,
    DeviceType: str = ...,
    DeviceModel: str = ...,
    DeviceOperatingSystem: str = ...,
    DeviceUserAgent: str = ...,
) -> GetMobileDeviceAccessEffectResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMobileDeviceAccessEffectResponseTypeDef](./type_defs.md#getmobiledeviceaccesseffectresponsetypedef) 


```python
# get_mobile_device_access_effect method usage example with argument unpacking

kwargs: GetMobileDeviceAccessEffectRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.get_mobile_device_access_effect(**kwargs)
```

1. See [:material-code-braces: GetMobileDeviceAccessEffectRequestRequestTypeDef](./type_defs.md#getmobiledeviceaccesseffectrequestrequesttypedef) 

### get\_mobile\_device\_access\_override

Gets the mobile device access override for the given WorkMail organization,
user, and device.

Type annotations and code completion for `#!python session.create_client("workmail").get_mobile_device_access_override` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/get_mobile_device_access_override.html)

```python
# get_mobile_device_access_override method definition

await def get_mobile_device_access_override(
    self,
    *,
    OrganizationId: str,
    UserId: str,
    DeviceId: str,
) -> GetMobileDeviceAccessOverrideResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMobileDeviceAccessOverrideResponseTypeDef](./type_defs.md#getmobiledeviceaccessoverrideresponsetypedef) 


```python
# get_mobile_device_access_override method usage example with argument unpacking

kwargs: GetMobileDeviceAccessOverrideRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "UserId": ...,
    "DeviceId": ...,
}

parent.get_mobile_device_access_override(**kwargs)
```

1. See [:material-code-braces: GetMobileDeviceAccessOverrideRequestRequestTypeDef](./type_defs.md#getmobiledeviceaccessoverriderequestrequesttypedef) 

### get\_personal\_access\_token\_metadata

Requests details of a specific Personal Access Token within the WorkMail
organization.

Type annotations and code completion for `#!python session.create_client("workmail").get_personal_access_token_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/get_personal_access_token_metadata.html)

```python
# get_personal_access_token_metadata method definition

await def get_personal_access_token_metadata(
    self,
    *,
    OrganizationId: str,
    PersonalAccessTokenId: str,
) -> GetPersonalAccessTokenMetadataResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPersonalAccessTokenMetadataResponseTypeDef](./type_defs.md#getpersonalaccesstokenmetadataresponsetypedef) 


```python
# get_personal_access_token_metadata method usage example with argument unpacking

kwargs: GetPersonalAccessTokenMetadataRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "PersonalAccessTokenId": ...,
}

parent.get_personal_access_token_metadata(**kwargs)
```

1. See [:material-code-braces: GetPersonalAccessTokenMetadataRequestRequestTypeDef](./type_defs.md#getpersonalaccesstokenmetadatarequestrequesttypedef) 

### list\_access\_control\_rules

Lists the access control rules for the specified organization.

Type annotations and code completion for `#!python session.create_client("workmail").list_access_control_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/list_access_control_rules.html)

```python
# list_access_control_rules method definition

await def list_access_control_rules(
    self,
    *,
    OrganizationId: str,
) -> ListAccessControlRulesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAccessControlRulesResponseTypeDef](./type_defs.md#listaccesscontrolrulesresponsetypedef) 


```python
# list_access_control_rules method usage example with argument unpacking

kwargs: ListAccessControlRulesRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.list_access_control_rules(**kwargs)
```

1. See [:material-code-braces: ListAccessControlRulesRequestRequestTypeDef](./type_defs.md#listaccesscontrolrulesrequestrequesttypedef) 

### list\_aliases

Creates a paginated call to list the aliases associated with a given entity.

Type annotations and code completion for `#!python session.create_client("workmail").list_aliases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/list_aliases.html)

```python
# list_aliases method definition

await def list_aliases(
    self,
    *,
    OrganizationId: str,
    EntityId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListAliasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef) 


```python
# list_aliases method usage example with argument unpacking

kwargs: ListAliasesRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "EntityId": ...,
}

parent.list_aliases(**kwargs)
```

1. See [:material-code-braces: ListAliasesRequestRequestTypeDef](./type_defs.md#listaliasesrequestrequesttypedef) 

### list\_availability\_configurations

List all the <code>AvailabilityConfiguration</code>'s for the given WorkMail
organization.

Type annotations and code completion for `#!python session.create_client("workmail").list_availability_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/list_availability_configurations.html)

```python
# list_availability_configurations method definition

await def list_availability_configurations(
    self,
    *,
    OrganizationId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAvailabilityConfigurationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAvailabilityConfigurationsResponseTypeDef](./type_defs.md#listavailabilityconfigurationsresponsetypedef) 


```python
# list_availability_configurations method usage example with argument unpacking

kwargs: ListAvailabilityConfigurationsRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.list_availability_configurations(**kwargs)
```

1. See [:material-code-braces: ListAvailabilityConfigurationsRequestRequestTypeDef](./type_defs.md#listavailabilityconfigurationsrequestrequesttypedef) 

### list\_group\_members

Returns an overview of the members of a group.

Type annotations and code completion for `#!python session.create_client("workmail").list_group_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/list_group_members.html)

```python
# list_group_members method definition

await def list_group_members(
    self,
    *,
    OrganizationId: str,
    GroupId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListGroupMembersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGroupMembersResponseTypeDef](./type_defs.md#listgroupmembersresponsetypedef) 


```python
# list_group_members method usage example with argument unpacking

kwargs: ListGroupMembersRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "GroupId": ...,
}

parent.list_group_members(**kwargs)
```

1. See [:material-code-braces: ListGroupMembersRequestRequestTypeDef](./type_defs.md#listgroupmembersrequestrequesttypedef) 

### list\_groups

Returns summaries of the organization's groups.

Type annotations and code completion for `#!python session.create_client("workmail").list_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/list_groups.html)

```python
# list_groups method definition

await def list_groups(
    self,
    *,
    OrganizationId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    Filters: ListGroupsFiltersTypeDef = ...,  # (1)
) -> ListGroupsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListGroupsFiltersTypeDef](./type_defs.md#listgroupsfilterstypedef) 
2. See [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


```python
# list_groups method usage example with argument unpacking

kwargs: ListGroupsRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.list_groups(**kwargs)
```

1. See [:material-code-braces: ListGroupsRequestRequestTypeDef](./type_defs.md#listgroupsrequestrequesttypedef) 

### list\_groups\_for\_entity

Returns all the groups to which an entity belongs.

Type annotations and code completion for `#!python session.create_client("workmail").list_groups_for_entity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/list_groups_for_entity.html)

```python
# list_groups_for_entity method definition

await def list_groups_for_entity(
    self,
    *,
    OrganizationId: str,
    EntityId: str,
    Filters: ListGroupsForEntityFiltersTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListGroupsForEntityResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListGroupsForEntityFiltersTypeDef](./type_defs.md#listgroupsforentityfilterstypedef) 
2. See [:material-code-braces: ListGroupsForEntityResponseTypeDef](./type_defs.md#listgroupsforentityresponsetypedef) 


```python
# list_groups_for_entity method usage example with argument unpacking

kwargs: ListGroupsForEntityRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "EntityId": ...,
}

parent.list_groups_for_entity(**kwargs)
```

1. See [:material-code-braces: ListGroupsForEntityRequestRequestTypeDef](./type_defs.md#listgroupsforentityrequestrequesttypedef) 

### list\_impersonation\_roles

Lists all the impersonation roles for the given WorkMail organization.

Type annotations and code completion for `#!python session.create_client("workmail").list_impersonation_roles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/list_impersonation_roles.html)

```python
# list_impersonation_roles method definition

await def list_impersonation_roles(
    self,
    *,
    OrganizationId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListImpersonationRolesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListImpersonationRolesResponseTypeDef](./type_defs.md#listimpersonationrolesresponsetypedef) 


```python
# list_impersonation_roles method usage example with argument unpacking

kwargs: ListImpersonationRolesRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.list_impersonation_roles(**kwargs)
```

1. See [:material-code-braces: ListImpersonationRolesRequestRequestTypeDef](./type_defs.md#listimpersonationrolesrequestrequesttypedef) 

### list\_mail\_domains

Lists the mail domains in a given WorkMail organization.

Type annotations and code completion for `#!python session.create_client("workmail").list_mail_domains` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/list_mail_domains.html)

```python
# list_mail_domains method definition

await def list_mail_domains(
    self,
    *,
    OrganizationId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListMailDomainsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMailDomainsResponseTypeDef](./type_defs.md#listmaildomainsresponsetypedef) 


```python
# list_mail_domains method usage example with argument unpacking

kwargs: ListMailDomainsRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.list_mail_domains(**kwargs)
```

1. See [:material-code-braces: ListMailDomainsRequestRequestTypeDef](./type_defs.md#listmaildomainsrequestrequesttypedef) 

### list\_mailbox\_export\_jobs

Lists the mailbox export jobs started for the specified organization within the
last seven days.

Type annotations and code completion for `#!python session.create_client("workmail").list_mailbox_export_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/list_mailbox_export_jobs.html)

```python
# list_mailbox_export_jobs method definition

await def list_mailbox_export_jobs(
    self,
    *,
    OrganizationId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListMailboxExportJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMailboxExportJobsResponseTypeDef](./type_defs.md#listmailboxexportjobsresponsetypedef) 


```python
# list_mailbox_export_jobs method usage example with argument unpacking

kwargs: ListMailboxExportJobsRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.list_mailbox_export_jobs(**kwargs)
```

1. See [:material-code-braces: ListMailboxExportJobsRequestRequestTypeDef](./type_defs.md#listmailboxexportjobsrequestrequesttypedef) 

### list\_mailbox\_permissions

Lists the mailbox permissions associated with a user, group, or resource
mailbox.

Type annotations and code completion for `#!python session.create_client("workmail").list_mailbox_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/list_mailbox_permissions.html)

```python
# list_mailbox_permissions method definition

await def list_mailbox_permissions(
    self,
    *,
    OrganizationId: str,
    EntityId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListMailboxPermissionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMailboxPermissionsResponseTypeDef](./type_defs.md#listmailboxpermissionsresponsetypedef) 


```python
# list_mailbox_permissions method usage example with argument unpacking

kwargs: ListMailboxPermissionsRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "EntityId": ...,
}

parent.list_mailbox_permissions(**kwargs)
```

1. See [:material-code-braces: ListMailboxPermissionsRequestRequestTypeDef](./type_defs.md#listmailboxpermissionsrequestrequesttypedef) 

### list\_mobile\_device\_access\_overrides

Lists all the mobile device access overrides for any given combination of
WorkMail organization, user, or device.

Type annotations and code completion for `#!python session.create_client("workmail").list_mobile_device_access_overrides` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/list_mobile_device_access_overrides.html)

```python
# list_mobile_device_access_overrides method definition

await def list_mobile_device_access_overrides(
    self,
    *,
    OrganizationId: str,
    UserId: str = ...,
    DeviceId: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListMobileDeviceAccessOverridesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMobileDeviceAccessOverridesResponseTypeDef](./type_defs.md#listmobiledeviceaccessoverridesresponsetypedef) 


```python
# list_mobile_device_access_overrides method usage example with argument unpacking

kwargs: ListMobileDeviceAccessOverridesRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.list_mobile_device_access_overrides(**kwargs)
```

1. See [:material-code-braces: ListMobileDeviceAccessOverridesRequestRequestTypeDef](./type_defs.md#listmobiledeviceaccessoverridesrequestrequesttypedef) 

### list\_mobile\_device\_access\_rules

Lists the mobile device access rules for the specified WorkMail organization.

Type annotations and code completion for `#!python session.create_client("workmail").list_mobile_device_access_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/list_mobile_device_access_rules.html)

```python
# list_mobile_device_access_rules method definition

await def list_mobile_device_access_rules(
    self,
    *,
    OrganizationId: str,
) -> ListMobileDeviceAccessRulesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMobileDeviceAccessRulesResponseTypeDef](./type_defs.md#listmobiledeviceaccessrulesresponsetypedef) 


```python
# list_mobile_device_access_rules method usage example with argument unpacking

kwargs: ListMobileDeviceAccessRulesRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.list_mobile_device_access_rules(**kwargs)
```

1. See [:material-code-braces: ListMobileDeviceAccessRulesRequestRequestTypeDef](./type_defs.md#listmobiledeviceaccessrulesrequestrequesttypedef) 

### list\_organizations

Returns summaries of the customer's organizations.

Type annotations and code completion for `#!python session.create_client("workmail").list_organizations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/list_organizations.html)

```python
# list_organizations method definition

await def list_organizations(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListOrganizationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOrganizationsResponseTypeDef](./type_defs.md#listorganizationsresponsetypedef) 


```python
# list_organizations method usage example with argument unpacking

kwargs: ListOrganizationsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_organizations(**kwargs)
```

1. See [:material-code-braces: ListOrganizationsRequestRequestTypeDef](./type_defs.md#listorganizationsrequestrequesttypedef) 

### list\_personal\_access\_tokens

Returns a summary of your Personal Access Tokens.

Type annotations and code completion for `#!python session.create_client("workmail").list_personal_access_tokens` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/list_personal_access_tokens.html)

```python
# list_personal_access_tokens method definition

await def list_personal_access_tokens(
    self,
    *,
    OrganizationId: str,
    UserId: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListPersonalAccessTokensResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPersonalAccessTokensResponseTypeDef](./type_defs.md#listpersonalaccesstokensresponsetypedef) 


```python
# list_personal_access_tokens method usage example with argument unpacking

kwargs: ListPersonalAccessTokensRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.list_personal_access_tokens(**kwargs)
```

1. See [:material-code-braces: ListPersonalAccessTokensRequestRequestTypeDef](./type_defs.md#listpersonalaccesstokensrequestrequesttypedef) 

### list\_resource\_delegates

Lists the delegates associated with a resource.

Type annotations and code completion for `#!python session.create_client("workmail").list_resource_delegates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/list_resource_delegates.html)

```python
# list_resource_delegates method definition

await def list_resource_delegates(
    self,
    *,
    OrganizationId: str,
    ResourceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListResourceDelegatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListResourceDelegatesResponseTypeDef](./type_defs.md#listresourcedelegatesresponsetypedef) 


```python
# list_resource_delegates method usage example with argument unpacking

kwargs: ListResourceDelegatesRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "ResourceId": ...,
}

parent.list_resource_delegates(**kwargs)
```

1. See [:material-code-braces: ListResourceDelegatesRequestRequestTypeDef](./type_defs.md#listresourcedelegatesrequestrequesttypedef) 

### list\_resources

Returns summaries of the organization's resources.

Type annotations and code completion for `#!python session.create_client("workmail").list_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/list_resources.html)

```python
# list_resources method definition

await def list_resources(
    self,
    *,
    OrganizationId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    Filters: ListResourcesFiltersTypeDef = ...,  # (1)
) -> ListResourcesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListResourcesFiltersTypeDef](./type_defs.md#listresourcesfilterstypedef) 
2. See [:material-code-braces: ListResourcesResponseTypeDef](./type_defs.md#listresourcesresponsetypedef) 


```python
# list_resources method usage example with argument unpacking

kwargs: ListResourcesRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.list_resources(**kwargs)
```

1. See [:material-code-braces: ListResourcesRequestRequestTypeDef](./type_defs.md#listresourcesrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags applied to an WorkMail organization resource.

Type annotations and code completion for `#!python session.create_client("workmail").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_users

Returns summaries of the organization's users.

Type annotations and code completion for `#!python session.create_client("workmail").list_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/list_users.html)

```python
# list_users method definition

await def list_users(
    self,
    *,
    OrganizationId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    Filters: ListUsersFiltersTypeDef = ...,  # (1)
) -> ListUsersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListUsersFiltersTypeDef](./type_defs.md#listusersfilterstypedef) 
2. See [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


```python
# list_users method usage example with argument unpacking

kwargs: ListUsersRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.list_users(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestRequestTypeDef](./type_defs.md#listusersrequestrequesttypedef) 

### put\_access\_control\_rule

Adds a new access control rule for the specified organization.

Type annotations and code completion for `#!python session.create_client("workmail").put_access_control_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/put_access_control_rule.html)

```python
# put_access_control_rule method definition

await def put_access_control_rule(
    self,
    *,
    Name: str,
    Effect: AccessControlRuleEffectType,  # (1)
    Description: str,
    OrganizationId: str,
    IpRanges: Sequence[str] = ...,
    NotIpRanges: Sequence[str] = ...,
    Actions: Sequence[str] = ...,
    NotActions: Sequence[str] = ...,
    UserIds: Sequence[str] = ...,
    NotUserIds: Sequence[str] = ...,
    ImpersonationRoleIds: Sequence[str] = ...,
    NotImpersonationRoleIds: Sequence[str] = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: AccessControlRuleEffectType](./literals.md#accesscontrolruleeffecttype) 


```python
# put_access_control_rule method usage example with argument unpacking

kwargs: PutAccessControlRuleRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Effect": ...,
    "Description": ...,
    "OrganizationId": ...,
}

parent.put_access_control_rule(**kwargs)
```

1. See [:material-code-braces: PutAccessControlRuleRequestRequestTypeDef](./type_defs.md#putaccesscontrolrulerequestrequesttypedef) 

### put\_email\_monitoring\_configuration

Creates or updates the email monitoring configuration for a specified
organization.

Type annotations and code completion for `#!python session.create_client("workmail").put_email_monitoring_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/put_email_monitoring_configuration.html)

```python
# put_email_monitoring_configuration method definition

await def put_email_monitoring_configuration(
    self,
    *,
    OrganizationId: str,
    RoleArn: str,
    LogGroupArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# put_email_monitoring_configuration method usage example with argument unpacking

kwargs: PutEmailMonitoringConfigurationRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "RoleArn": ...,
    "LogGroupArn": ...,
}

parent.put_email_monitoring_configuration(**kwargs)
```

1. See [:material-code-braces: PutEmailMonitoringConfigurationRequestRequestTypeDef](./type_defs.md#putemailmonitoringconfigurationrequestrequesttypedef) 

### put\_identity\_provider\_configuration

Enables integration between IAM Identity Center (IdC) and WorkMail to proxy
authentication requests for mailbox users.

Type annotations and code completion for `#!python session.create_client("workmail").put_identity_provider_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/put_identity_provider_configuration.html)

```python
# put_identity_provider_configuration method definition

await def put_identity_provider_configuration(
    self,
    *,
    OrganizationId: str,
    AuthenticationMode: IdentityProviderAuthenticationModeType,  # (1)
    IdentityCenterConfiguration: IdentityCenterConfigurationTypeDef,  # (2)
    PersonalAccessTokenConfiguration: PersonalAccessTokenConfigurationTypeDef,  # (3)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: IdentityProviderAuthenticationModeType](./literals.md#identityproviderauthenticationmodetype) 
2. See [:material-code-braces: IdentityCenterConfigurationTypeDef](./type_defs.md#identitycenterconfigurationtypedef) 
3. See [:material-code-braces: PersonalAccessTokenConfigurationTypeDef](./type_defs.md#personalaccesstokenconfigurationtypedef) 


```python
# put_identity_provider_configuration method usage example with argument unpacking

kwargs: PutIdentityProviderConfigurationRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "AuthenticationMode": ...,
    "IdentityCenterConfiguration": ...,
    "PersonalAccessTokenConfiguration": ...,
}

parent.put_identity_provider_configuration(**kwargs)
```

1. See [:material-code-braces: PutIdentityProviderConfigurationRequestRequestTypeDef](./type_defs.md#putidentityproviderconfigurationrequestrequesttypedef) 

### put\_inbound\_dmarc\_settings

Enables or disables a DMARC policy for a given organization.

Type annotations and code completion for `#!python session.create_client("workmail").put_inbound_dmarc_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/put_inbound_dmarc_settings.html)

```python
# put_inbound_dmarc_settings method definition

await def put_inbound_dmarc_settings(
    self,
    *,
    OrganizationId: str,
    Enforced: bool,
) -> Dict[str, Any]:
    ...
```



```python
# put_inbound_dmarc_settings method usage example with argument unpacking

kwargs: PutInboundDmarcSettingsRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "Enforced": ...,
}

parent.put_inbound_dmarc_settings(**kwargs)
```

1. See [:material-code-braces: PutInboundDmarcSettingsRequestRequestTypeDef](./type_defs.md#putinbounddmarcsettingsrequestrequesttypedef) 

### put\_mailbox\_permissions

Sets permissions for a user, group, or resource.

Type annotations and code completion for `#!python session.create_client("workmail").put_mailbox_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/put_mailbox_permissions.html)

```python
# put_mailbox_permissions method definition

await def put_mailbox_permissions(
    self,
    *,
    OrganizationId: str,
    EntityId: str,
    GranteeId: str,
    PermissionValues: Sequence[PermissionTypeType],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 


```python
# put_mailbox_permissions method usage example with argument unpacking

kwargs: PutMailboxPermissionsRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "EntityId": ...,
    "GranteeId": ...,
    "PermissionValues": ...,
}

parent.put_mailbox_permissions(**kwargs)
```

1. See [:material-code-braces: PutMailboxPermissionsRequestRequestTypeDef](./type_defs.md#putmailboxpermissionsrequestrequesttypedef) 

### put\_mobile\_device\_access\_override

Creates or updates a mobile device access override for the given WorkMail
organization, user, and device.

Type annotations and code completion for `#!python session.create_client("workmail").put_mobile_device_access_override` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/put_mobile_device_access_override.html)

```python
# put_mobile_device_access_override method definition

await def put_mobile_device_access_override(
    self,
    *,
    OrganizationId: str,
    UserId: str,
    DeviceId: str,
    Effect: MobileDeviceAccessRuleEffectType,  # (1)
    Description: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: MobileDeviceAccessRuleEffectType](./literals.md#mobiledeviceaccessruleeffecttype) 


```python
# put_mobile_device_access_override method usage example with argument unpacking

kwargs: PutMobileDeviceAccessOverrideRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "UserId": ...,
    "DeviceId": ...,
    "Effect": ...,
}

parent.put_mobile_device_access_override(**kwargs)
```

1. See [:material-code-braces: PutMobileDeviceAccessOverrideRequestRequestTypeDef](./type_defs.md#putmobiledeviceaccessoverriderequestrequesttypedef) 

### put\_retention\_policy

Puts a retention policy to the specified organization.

Type annotations and code completion for `#!python session.create_client("workmail").put_retention_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/put_retention_policy.html)

```python
# put_retention_policy method definition

await def put_retention_policy(
    self,
    *,
    OrganizationId: str,
    Name: str,
    FolderConfigurations: Sequence[FolderConfigurationTypeDef],  # (1)
    Id: str = ...,
    Description: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: FolderConfigurationTypeDef](./type_defs.md#folderconfigurationtypedef) 


```python
# put_retention_policy method usage example with argument unpacking

kwargs: PutRetentionPolicyRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "Name": ...,
    "FolderConfigurations": ...,
}

parent.put_retention_policy(**kwargs)
```

1. See [:material-code-braces: PutRetentionPolicyRequestRequestTypeDef](./type_defs.md#putretentionpolicyrequestrequesttypedef) 

### register\_mail\_domain

Registers a new domain in WorkMail and SES, and configures it for use by
WorkMail.

Type annotations and code completion for `#!python session.create_client("workmail").register_mail_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/register_mail_domain.html)

```python
# register_mail_domain method definition

await def register_mail_domain(
    self,
    *,
    OrganizationId: str,
    DomainName: str,
    ClientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# register_mail_domain method usage example with argument unpacking

kwargs: RegisterMailDomainRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "DomainName": ...,
}

parent.register_mail_domain(**kwargs)
```

1. See [:material-code-braces: RegisterMailDomainRequestRequestTypeDef](./type_defs.md#registermaildomainrequestrequesttypedef) 

### register\_to\_work\_mail

Registers an existing and disabled user, group, or resource for WorkMail use by
associating a mailbox and calendaring capabilities.

Type annotations and code completion for `#!python session.create_client("workmail").register_to_work_mail` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/register_to_work_mail.html)

```python
# register_to_work_mail method definition

await def register_to_work_mail(
    self,
    *,
    OrganizationId: str,
    EntityId: str,
    Email: str,
) -> Dict[str, Any]:
    ...
```



```python
# register_to_work_mail method usage example with argument unpacking

kwargs: RegisterToWorkMailRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "EntityId": ...,
    "Email": ...,
}

parent.register_to_work_mail(**kwargs)
```

1. See [:material-code-braces: RegisterToWorkMailRequestRequestTypeDef](./type_defs.md#registertoworkmailrequestrequesttypedef) 

### reset\_password

Allows the administrator to reset the password for a user.

Type annotations and code completion for `#!python session.create_client("workmail").reset_password` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/reset_password.html)

```python
# reset_password method definition

await def reset_password(
    self,
    *,
    OrganizationId: str,
    UserId: str,
    Password: str,
) -> Dict[str, Any]:
    ...
```



```python
# reset_password method usage example with argument unpacking

kwargs: ResetPasswordRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "UserId": ...,
    "Password": ...,
}

parent.reset_password(**kwargs)
```

1. See [:material-code-braces: ResetPasswordRequestRequestTypeDef](./type_defs.md#resetpasswordrequestrequesttypedef) 

### start\_mailbox\_export\_job

Starts a mailbox export job to export MIME-format email messages and calendar
items from the specified mailbox to the specified Amazon Simple Storage Service
(Amazon S3) bucket.

Type annotations and code completion for `#!python session.create_client("workmail").start_mailbox_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/start_mailbox_export_job.html)

```python
# start_mailbox_export_job method definition

await def start_mailbox_export_job(
    self,
    *,
    ClientToken: str,
    OrganizationId: str,
    EntityId: str,
    RoleArn: str,
    KmsKeyArn: str,
    S3BucketName: str,
    S3Prefix: str,
    Description: str = ...,
) -> StartMailboxExportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartMailboxExportJobResponseTypeDef](./type_defs.md#startmailboxexportjobresponsetypedef) 


```python
# start_mailbox_export_job method usage example with argument unpacking

kwargs: StartMailboxExportJobRequestRequestTypeDef = {  # (1)
    "ClientToken": ...,
    "OrganizationId": ...,
    "EntityId": ...,
    "RoleArn": ...,
    "KmsKeyArn": ...,
    "S3BucketName": ...,
    "S3Prefix": ...,
}

parent.start_mailbox_export_job(**kwargs)
```

1. See [:material-code-braces: StartMailboxExportJobRequestRequestTypeDef](./type_defs.md#startmailboxexportjobrequestrequesttypedef) 

### tag\_resource

Applies the specified tags to the specified WorkMailorganization resource.

Type annotations and code completion for `#!python session.create_client("workmail").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### test\_availability\_configuration

Performs a test on an availability provider to ensure that access is allowed.

Type annotations and code completion for `#!python session.create_client("workmail").test_availability_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/test_availability_configuration.html)

```python
# test_availability_configuration method definition

await def test_availability_configuration(
    self,
    *,
    OrganizationId: str,
    DomainName: str = ...,
    EwsProvider: EwsAvailabilityProviderTypeDef = ...,  # (1)
    LambdaProvider: LambdaAvailabilityProviderTypeDef = ...,  # (2)
) -> TestAvailabilityConfigurationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EwsAvailabilityProviderTypeDef](./type_defs.md#ewsavailabilityprovidertypedef) 
2. See [:material-code-braces: LambdaAvailabilityProviderTypeDef](./type_defs.md#lambdaavailabilityprovidertypedef) 
3. See [:material-code-braces: TestAvailabilityConfigurationResponseTypeDef](./type_defs.md#testavailabilityconfigurationresponsetypedef) 


```python
# test_availability_configuration method usage example with argument unpacking

kwargs: TestAvailabilityConfigurationRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.test_availability_configuration(**kwargs)
```

1. See [:material-code-braces: TestAvailabilityConfigurationRequestRequestTypeDef](./type_defs.md#testavailabilityconfigurationrequestrequesttypedef) 

### untag\_resource

Untags the specified tags from the specified WorkMail organization resource.

Type annotations and code completion for `#!python session.create_client("workmail").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceARN: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_availability\_configuration

Updates an existing <code>AvailabilityConfiguration</code> for the given
WorkMail organization and domain.

Type annotations and code completion for `#!python session.create_client("workmail").update_availability_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/update_availability_configuration.html)

```python
# update_availability_configuration method definition

await def update_availability_configuration(
    self,
    *,
    OrganizationId: str,
    DomainName: str,
    EwsProvider: EwsAvailabilityProviderTypeDef = ...,  # (1)
    LambdaProvider: LambdaAvailabilityProviderTypeDef = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: EwsAvailabilityProviderTypeDef](./type_defs.md#ewsavailabilityprovidertypedef) 
2. See [:material-code-braces: LambdaAvailabilityProviderTypeDef](./type_defs.md#lambdaavailabilityprovidertypedef) 


```python
# update_availability_configuration method usage example with argument unpacking

kwargs: UpdateAvailabilityConfigurationRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "DomainName": ...,
}

parent.update_availability_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateAvailabilityConfigurationRequestRequestTypeDef](./type_defs.md#updateavailabilityconfigurationrequestrequesttypedef) 

### update\_default\_mail\_domain

Updates the default mail domain for an organization.

Type annotations and code completion for `#!python session.create_client("workmail").update_default_mail_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/update_default_mail_domain.html)

```python
# update_default_mail_domain method definition

await def update_default_mail_domain(
    self,
    *,
    OrganizationId: str,
    DomainName: str,
) -> Dict[str, Any]:
    ...
```



```python
# update_default_mail_domain method usage example with argument unpacking

kwargs: UpdateDefaultMailDomainRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "DomainName": ...,
}

parent.update_default_mail_domain(**kwargs)
```

1. See [:material-code-braces: UpdateDefaultMailDomainRequestRequestTypeDef](./type_defs.md#updatedefaultmaildomainrequestrequesttypedef) 

### update\_group

Updates attributes in a group.

Type annotations and code completion for `#!python session.create_client("workmail").update_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/update_group.html)

```python
# update_group method definition

await def update_group(
    self,
    *,
    OrganizationId: str,
    GroupId: str,
    HiddenFromGlobalAddressList: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_group method usage example with argument unpacking

kwargs: UpdateGroupRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "GroupId": ...,
}

parent.update_group(**kwargs)
```

1. See [:material-code-braces: UpdateGroupRequestRequestTypeDef](./type_defs.md#updategrouprequestrequesttypedef) 

### update\_impersonation\_role

Updates an impersonation role for the given WorkMail organization.

Type annotations and code completion for `#!python session.create_client("workmail").update_impersonation_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/update_impersonation_role.html)

```python
# update_impersonation_role method definition

await def update_impersonation_role(
    self,
    *,
    OrganizationId: str,
    ImpersonationRoleId: str,
    Name: str,
    Type: ImpersonationRoleTypeType,  # (1)
    Rules: Sequence[ImpersonationRuleTypeDef],  # (2)
    Description: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ImpersonationRoleTypeType](./literals.md#impersonationroletypetype) 
2. See [:material-code-braces: ImpersonationRuleTypeDef](./type_defs.md#impersonationruletypedef) 


```python
# update_impersonation_role method usage example with argument unpacking

kwargs: UpdateImpersonationRoleRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "ImpersonationRoleId": ...,
    "Name": ...,
    "Type": ...,
    "Rules": ...,
}

parent.update_impersonation_role(**kwargs)
```

1. See [:material-code-braces: UpdateImpersonationRoleRequestRequestTypeDef](./type_defs.md#updateimpersonationrolerequestrequesttypedef) 

### update\_mailbox\_quota

Updates a user's current mailbox quota for a specified organization and user.

Type annotations and code completion for `#!python session.create_client("workmail").update_mailbox_quota` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/update_mailbox_quota.html)

```python
# update_mailbox_quota method definition

await def update_mailbox_quota(
    self,
    *,
    OrganizationId: str,
    UserId: str,
    MailboxQuota: int,
) -> Dict[str, Any]:
    ...
```



```python
# update_mailbox_quota method usage example with argument unpacking

kwargs: UpdateMailboxQuotaRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "UserId": ...,
    "MailboxQuota": ...,
}

parent.update_mailbox_quota(**kwargs)
```

1. See [:material-code-braces: UpdateMailboxQuotaRequestRequestTypeDef](./type_defs.md#updatemailboxquotarequestrequesttypedef) 

### update\_mobile\_device\_access\_rule

Updates a mobile device access rule for the specified WorkMail organization.

Type annotations and code completion for `#!python session.create_client("workmail").update_mobile_device_access_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/update_mobile_device_access_rule.html)

```python
# update_mobile_device_access_rule method definition

await def update_mobile_device_access_rule(
    self,
    *,
    OrganizationId: str,
    MobileDeviceAccessRuleId: str,
    Name: str,
    Effect: MobileDeviceAccessRuleEffectType,  # (1)
    Description: str = ...,
    DeviceTypes: Sequence[str] = ...,
    NotDeviceTypes: Sequence[str] = ...,
    DeviceModels: Sequence[str] = ...,
    NotDeviceModels: Sequence[str] = ...,
    DeviceOperatingSystems: Sequence[str] = ...,
    NotDeviceOperatingSystems: Sequence[str] = ...,
    DeviceUserAgents: Sequence[str] = ...,
    NotDeviceUserAgents: Sequence[str] = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: MobileDeviceAccessRuleEffectType](./literals.md#mobiledeviceaccessruleeffecttype) 


```python
# update_mobile_device_access_rule method usage example with argument unpacking

kwargs: UpdateMobileDeviceAccessRuleRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "MobileDeviceAccessRuleId": ...,
    "Name": ...,
    "Effect": ...,
}

parent.update_mobile_device_access_rule(**kwargs)
```

1. See [:material-code-braces: UpdateMobileDeviceAccessRuleRequestRequestTypeDef](./type_defs.md#updatemobiledeviceaccessrulerequestrequesttypedef) 

### update\_primary\_email\_address

Updates the primary email for a user, group, or resource.

Type annotations and code completion for `#!python session.create_client("workmail").update_primary_email_address` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/update_primary_email_address.html)

```python
# update_primary_email_address method definition

await def update_primary_email_address(
    self,
    *,
    OrganizationId: str,
    EntityId: str,
    Email: str,
) -> Dict[str, Any]:
    ...
```



```python
# update_primary_email_address method usage example with argument unpacking

kwargs: UpdatePrimaryEmailAddressRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "EntityId": ...,
    "Email": ...,
}

parent.update_primary_email_address(**kwargs)
```

1. See [:material-code-braces: UpdatePrimaryEmailAddressRequestRequestTypeDef](./type_defs.md#updateprimaryemailaddressrequestrequesttypedef) 

### update\_resource

Updates data for the resource.

Type annotations and code completion for `#!python session.create_client("workmail").update_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/update_resource.html)

```python
# update_resource method definition

await def update_resource(
    self,
    *,
    OrganizationId: str,
    ResourceId: str,
    Name: str = ...,
    BookingOptions: BookingOptionsTypeDef = ...,  # (1)
    Description: str = ...,
    Type: ResourceTypeType = ...,  # (2)
    HiddenFromGlobalAddressList: bool = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: BookingOptionsTypeDef](./type_defs.md#bookingoptionstypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 


```python
# update_resource method usage example with argument unpacking

kwargs: UpdateResourceRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "ResourceId": ...,
}

parent.update_resource(**kwargs)
```

1. See [:material-code-braces: UpdateResourceRequestRequestTypeDef](./type_defs.md#updateresourcerequestrequesttypedef) 

### update\_user

Updates data for the user.

Type annotations and code completion for `#!python session.create_client("workmail").update_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/client/update_user.html)

```python
# update_user method definition

await def update_user(
    self,
    *,
    OrganizationId: str,
    UserId: str,
    Role: UserRoleType = ...,  # (1)
    DisplayName: str = ...,
    FirstName: str = ...,
    LastName: str = ...,
    HiddenFromGlobalAddressList: bool = ...,
    Initials: str = ...,
    Telephone: str = ...,
    Street: str = ...,
    JobTitle: str = ...,
    City: str = ...,
    Company: str = ...,
    ZipCode: str = ...,
    Department: str = ...,
    Country: str = ...,
    Office: str = ...,
    IdentityProviderUserId: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: UserRoleType](./literals.md#userroletype) 


```python
# update_user method usage example with argument unpacking

kwargs: UpdateUserRequestRequestTypeDef = {  # (1)
    "OrganizationId": ...,
    "UserId": ...,
}

parent.update_user(**kwargs)
```

1. See [:material-code-braces: UpdateUserRequestRequestTypeDef](./type_defs.md#updateuserrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("workmail").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("workmail").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("workmail").get_paginator` method with overloads.

- `client.get_paginator("list_aliases")` -> [ListAliasesPaginator](./paginators.md#listaliasespaginator)
- `client.get_paginator("list_availability_configurations")` -> [ListAvailabilityConfigurationsPaginator](./paginators.md#listavailabilityconfigurationspaginator)
- `client.get_paginator("list_group_members")` -> [ListGroupMembersPaginator](./paginators.md#listgroupmemberspaginator)
- `client.get_paginator("list_groups")` -> [ListGroupsPaginator](./paginators.md#listgroupspaginator)
- `client.get_paginator("list_mailbox_permissions")` -> [ListMailboxPermissionsPaginator](./paginators.md#listmailboxpermissionspaginator)
- `client.get_paginator("list_organizations")` -> [ListOrganizationsPaginator](./paginators.md#listorganizationspaginator)
- `client.get_paginator("list_personal_access_tokens")` -> [ListPersonalAccessTokensPaginator](./paginators.md#listpersonalaccesstokenspaginator)
- `client.get_paginator("list_resource_delegates")` -> [ListResourceDelegatesPaginator](./paginators.md#listresourcedelegatespaginator)
- `client.get_paginator("list_resources")` -> [ListResourcesPaginator](./paginators.md#listresourcespaginator)
- `client.get_paginator("list_users")` -> [ListUsersPaginator](./paginators.md#listuserspaginator)



