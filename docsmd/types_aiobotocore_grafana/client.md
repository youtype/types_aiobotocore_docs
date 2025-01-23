# ManagedGrafanaClient

> [Index](../README.md) > [ManagedGrafana](./README.md) > ManagedGrafanaClient

!!! note ""

    Auto-generated documentation for [ManagedGrafana](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#managedgrafana)
    type annotations stubs module [types-aiobotocore-grafana](https://pypi.org/project/types-aiobotocore-grafana/).

## ManagedGrafanaClient

Type annotations and code completion for `#!python session.create_client("grafana")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client)

```python
# ManagedGrafanaClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_grafana.client import ManagedGrafanaClient

session = get_session()
async with session.create_client("grafana") as client:
    client: ManagedGrafanaClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("grafana").exceptions` structure.

```python
# ManagedGrafanaClient.exceptions usage example

async with session.create_client("grafana") as client:
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
# ManagedGrafanaClient usage type checking example

from types_aiobotocore_grafana.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("grafana").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("grafana").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/generate_presigned_url.html)

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


### associate\_license

Assigns a Grafana Enterprise license to a workspace.

Type annotations and code completion for `#!python session.create_client("grafana").associate_license` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/associate_license.html)

```python
# associate_license method definition

await def associate_license(
    self,
    *,
    licenseType: LicenseTypeType,  # (1)
    workspaceId: str,
    grafanaToken: str = ...,
) -> AssociateLicenseResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LicenseTypeType](./literals.md#licensetypetype) 
2. See [:material-code-braces: AssociateLicenseResponseTypeDef](./type_defs.md#associatelicenseresponsetypedef) 


```python
# associate_license method usage example with argument unpacking

kwargs: AssociateLicenseRequestRequestTypeDef = {  # (1)
    "licenseType": ...,
    "workspaceId": ...,
}

parent.associate_license(**kwargs)
```

1. See [:material-code-braces: AssociateLicenseRequestRequestTypeDef](./type_defs.md#associatelicenserequestrequesttypedef) 

### create\_workspace

Creates a <i>workspace</i>.

Type annotations and code completion for `#!python session.create_client("grafana").create_workspace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/create_workspace.html)

```python
# create_workspace method definition

await def create_workspace(
    self,
    *,
    accountAccessType: AccountAccessTypeType,  # (1)
    authenticationProviders: Sequence[AuthenticationProviderTypesType],  # (2)
    permissionType: PermissionTypeType,  # (3)
    clientToken: str = ...,
    configuration: str = ...,
    grafanaVersion: str = ...,
    networkAccessControl: NetworkAccessConfigurationTypeDef = ...,  # (4)
    organizationRoleName: str = ...,
    stackSetName: str = ...,
    tags: Mapping[str, str] = ...,
    vpcConfiguration: VpcConfigurationTypeDef = ...,  # (5)
    workspaceDataSources: Sequence[DataSourceTypeType] = ...,  # (6)
    workspaceDescription: str = ...,
    workspaceName: str = ...,
    workspaceNotificationDestinations: Sequence[NotificationDestinationTypeType] = ...,  # (7)
    workspaceOrganizationalUnits: Sequence[str] = ...,
    workspaceRoleArn: str = ...,
) -> CreateWorkspaceResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-brackets: AccountAccessTypeType](./literals.md#accountaccesstypetype) 
2. See [:material-code-brackets: AuthenticationProviderTypesType](./literals.md#authenticationprovidertypestype) 
3. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
4. See [:material-code-braces: NetworkAccessConfigurationTypeDef](./type_defs.md#networkaccessconfigurationtypedef) 
5. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
6. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
7. See [:material-code-brackets: NotificationDestinationTypeType](./literals.md#notificationdestinationtypetype) 
8. See [:material-code-braces: CreateWorkspaceResponseTypeDef](./type_defs.md#createworkspaceresponsetypedef) 


```python
# create_workspace method usage example with argument unpacking

kwargs: CreateWorkspaceRequestRequestTypeDef = {  # (1)
    "accountAccessType": ...,
    "authenticationProviders": ...,
    "permissionType": ...,
}

parent.create_workspace(**kwargs)
```

1. See [:material-code-braces: CreateWorkspaceRequestRequestTypeDef](./type_defs.md#createworkspacerequestrequesttypedef) 

### create\_workspace\_api\_key

Creates a Grafana API key for the workspace.

Type annotations and code completion for `#!python session.create_client("grafana").create_workspace_api_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/create_workspace_api_key.html)

```python
# create_workspace_api_key method definition

await def create_workspace_api_key(
    self,
    *,
    keyName: str,
    keyRole: str,
    secondsToLive: int,
    workspaceId: str,
) -> CreateWorkspaceApiKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateWorkspaceApiKeyResponseTypeDef](./type_defs.md#createworkspaceapikeyresponsetypedef) 


```python
# create_workspace_api_key method usage example with argument unpacking

kwargs: CreateWorkspaceApiKeyRequestRequestTypeDef = {  # (1)
    "keyName": ...,
    "keyRole": ...,
    "secondsToLive": ...,
    "workspaceId": ...,
}

parent.create_workspace_api_key(**kwargs)
```

1. See [:material-code-braces: CreateWorkspaceApiKeyRequestRequestTypeDef](./type_defs.md#createworkspaceapikeyrequestrequesttypedef) 

### create\_workspace\_service\_account

Creates a service account for the workspace.

Type annotations and code completion for `#!python session.create_client("grafana").create_workspace_service_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/create_workspace_service_account.html)

```python
# create_workspace_service_account method definition

await def create_workspace_service_account(
    self,
    *,
    grafanaRole: RoleType,  # (1)
    name: str,
    workspaceId: str,
) -> CreateWorkspaceServiceAccountResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype) 
2. See [:material-code-braces: CreateWorkspaceServiceAccountResponseTypeDef](./type_defs.md#createworkspaceserviceaccountresponsetypedef) 


```python
# create_workspace_service_account method usage example with argument unpacking

kwargs: CreateWorkspaceServiceAccountRequestRequestTypeDef = {  # (1)
    "grafanaRole": ...,
    "name": ...,
    "workspaceId": ...,
}

parent.create_workspace_service_account(**kwargs)
```

1. See [:material-code-braces: CreateWorkspaceServiceAccountRequestRequestTypeDef](./type_defs.md#createworkspaceserviceaccountrequestrequesttypedef) 

### create\_workspace\_service\_account\_token

Creates a token that can be used to authenticate and authorize Grafana HTTP API
operations for the given <a
href="https://docs.aws.amazon.com/grafana/latest/userguide/service-accounts.html">workspace
service account</a>.

Type annotations and code completion for `#!python session.create_client("grafana").create_workspace_service_account_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/create_workspace_service_account_token.html)

```python
# create_workspace_service_account_token method definition

await def create_workspace_service_account_token(
    self,
    *,
    name: str,
    secondsToLive: int,
    serviceAccountId: str,
    workspaceId: str,
) -> CreateWorkspaceServiceAccountTokenResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateWorkspaceServiceAccountTokenResponseTypeDef](./type_defs.md#createworkspaceserviceaccounttokenresponsetypedef) 


```python
# create_workspace_service_account_token method usage example with argument unpacking

kwargs: CreateWorkspaceServiceAccountTokenRequestRequestTypeDef = {  # (1)
    "name": ...,
    "secondsToLive": ...,
    "serviceAccountId": ...,
    "workspaceId": ...,
}

parent.create_workspace_service_account_token(**kwargs)
```

1. See [:material-code-braces: CreateWorkspaceServiceAccountTokenRequestRequestTypeDef](./type_defs.md#createworkspaceserviceaccounttokenrequestrequesttypedef) 

### delete\_workspace

Deletes an Amazon Managed Grafana workspace.

Type annotations and code completion for `#!python session.create_client("grafana").delete_workspace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/delete_workspace.html)

```python
# delete_workspace method definition

await def delete_workspace(
    self,
    *,
    workspaceId: str,
) -> DeleteWorkspaceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteWorkspaceResponseTypeDef](./type_defs.md#deleteworkspaceresponsetypedef) 


```python
# delete_workspace method usage example with argument unpacking

kwargs: DeleteWorkspaceRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.delete_workspace(**kwargs)
```

1. See [:material-code-braces: DeleteWorkspaceRequestRequestTypeDef](./type_defs.md#deleteworkspacerequestrequesttypedef) 

### delete\_workspace\_api\_key

Deletes a Grafana API key for the workspace.

Type annotations and code completion for `#!python session.create_client("grafana").delete_workspace_api_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/delete_workspace_api_key.html)

```python
# delete_workspace_api_key method definition

await def delete_workspace_api_key(
    self,
    *,
    keyName: str,
    workspaceId: str,
) -> DeleteWorkspaceApiKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteWorkspaceApiKeyResponseTypeDef](./type_defs.md#deleteworkspaceapikeyresponsetypedef) 


```python
# delete_workspace_api_key method usage example with argument unpacking

kwargs: DeleteWorkspaceApiKeyRequestRequestTypeDef = {  # (1)
    "keyName": ...,
    "workspaceId": ...,
}

parent.delete_workspace_api_key(**kwargs)
```

1. See [:material-code-braces: DeleteWorkspaceApiKeyRequestRequestTypeDef](./type_defs.md#deleteworkspaceapikeyrequestrequesttypedef) 

### delete\_workspace\_service\_account

Deletes a workspace service account from the workspace.

Type annotations and code completion for `#!python session.create_client("grafana").delete_workspace_service_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/delete_workspace_service_account.html)

```python
# delete_workspace_service_account method definition

await def delete_workspace_service_account(
    self,
    *,
    serviceAccountId: str,
    workspaceId: str,
) -> DeleteWorkspaceServiceAccountResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteWorkspaceServiceAccountResponseTypeDef](./type_defs.md#deleteworkspaceserviceaccountresponsetypedef) 


```python
# delete_workspace_service_account method usage example with argument unpacking

kwargs: DeleteWorkspaceServiceAccountRequestRequestTypeDef = {  # (1)
    "serviceAccountId": ...,
    "workspaceId": ...,
}

parent.delete_workspace_service_account(**kwargs)
```

1. See [:material-code-braces: DeleteWorkspaceServiceAccountRequestRequestTypeDef](./type_defs.md#deleteworkspaceserviceaccountrequestrequesttypedef) 

### delete\_workspace\_service\_account\_token

Deletes a token for the workspace service account.

Type annotations and code completion for `#!python session.create_client("grafana").delete_workspace_service_account_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/delete_workspace_service_account_token.html)

```python
# delete_workspace_service_account_token method definition

await def delete_workspace_service_account_token(
    self,
    *,
    serviceAccountId: str,
    tokenId: str,
    workspaceId: str,
) -> DeleteWorkspaceServiceAccountTokenResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteWorkspaceServiceAccountTokenResponseTypeDef](./type_defs.md#deleteworkspaceserviceaccounttokenresponsetypedef) 


```python
# delete_workspace_service_account_token method usage example with argument unpacking

kwargs: DeleteWorkspaceServiceAccountTokenRequestRequestTypeDef = {  # (1)
    "serviceAccountId": ...,
    "tokenId": ...,
    "workspaceId": ...,
}

parent.delete_workspace_service_account_token(**kwargs)
```

1. See [:material-code-braces: DeleteWorkspaceServiceAccountTokenRequestRequestTypeDef](./type_defs.md#deleteworkspaceserviceaccounttokenrequestrequesttypedef) 

### describe\_workspace

Displays information about one Amazon Managed Grafana workspace.

Type annotations and code completion for `#!python session.create_client("grafana").describe_workspace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/describe_workspace.html)

```python
# describe_workspace method definition

await def describe_workspace(
    self,
    *,
    workspaceId: str,
) -> DescribeWorkspaceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeWorkspaceResponseTypeDef](./type_defs.md#describeworkspaceresponsetypedef) 


```python
# describe_workspace method usage example with argument unpacking

kwargs: DescribeWorkspaceRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.describe_workspace(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspaceRequestRequestTypeDef](./type_defs.md#describeworkspacerequestrequesttypedef) 

### describe\_workspace\_authentication

Displays information about the authentication methods used in one Amazon
Managed Grafana workspace.

Type annotations and code completion for `#!python session.create_client("grafana").describe_workspace_authentication` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/describe_workspace_authentication.html)

```python
# describe_workspace_authentication method definition

await def describe_workspace_authentication(
    self,
    *,
    workspaceId: str,
) -> DescribeWorkspaceAuthenticationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeWorkspaceAuthenticationResponseTypeDef](./type_defs.md#describeworkspaceauthenticationresponsetypedef) 


```python
# describe_workspace_authentication method usage example with argument unpacking

kwargs: DescribeWorkspaceAuthenticationRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.describe_workspace_authentication(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspaceAuthenticationRequestRequestTypeDef](./type_defs.md#describeworkspaceauthenticationrequestrequesttypedef) 

### describe\_workspace\_configuration

Gets the current configuration string for the given workspace.

Type annotations and code completion for `#!python session.create_client("grafana").describe_workspace_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/describe_workspace_configuration.html)

```python
# describe_workspace_configuration method definition

await def describe_workspace_configuration(
    self,
    *,
    workspaceId: str,
) -> DescribeWorkspaceConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeWorkspaceConfigurationResponseTypeDef](./type_defs.md#describeworkspaceconfigurationresponsetypedef) 


```python
# describe_workspace_configuration method usage example with argument unpacking

kwargs: DescribeWorkspaceConfigurationRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.describe_workspace_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspaceConfigurationRequestRequestTypeDef](./type_defs.md#describeworkspaceconfigurationrequestrequesttypedef) 

### disassociate\_license

Removes the Grafana Enterprise license from a workspace.

Type annotations and code completion for `#!python session.create_client("grafana").disassociate_license` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/disassociate_license.html)

```python
# disassociate_license method definition

await def disassociate_license(
    self,
    *,
    licenseType: LicenseTypeType,  # (1)
    workspaceId: str,
) -> DisassociateLicenseResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LicenseTypeType](./literals.md#licensetypetype) 
2. See [:material-code-braces: DisassociateLicenseResponseTypeDef](./type_defs.md#disassociatelicenseresponsetypedef) 


```python
# disassociate_license method usage example with argument unpacking

kwargs: DisassociateLicenseRequestRequestTypeDef = {  # (1)
    "licenseType": ...,
    "workspaceId": ...,
}

parent.disassociate_license(**kwargs)
```

1. See [:material-code-braces: DisassociateLicenseRequestRequestTypeDef](./type_defs.md#disassociatelicenserequestrequesttypedef) 

### list\_permissions

Lists the users and groups who have the Grafana <code>Admin</code> and
<code>Editor</code> roles in this workspace.

Type annotations and code completion for `#!python session.create_client("grafana").list_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/list_permissions.html)

```python
# list_permissions method definition

await def list_permissions(
    self,
    *,
    workspaceId: str,
    groupId: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    userId: str = ...,
    userType: UserTypeType = ...,  # (1)
) -> ListPermissionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
2. See [:material-code-braces: ListPermissionsResponseTypeDef](./type_defs.md#listpermissionsresponsetypedef) 


```python
# list_permissions method usage example with argument unpacking

kwargs: ListPermissionsRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.list_permissions(**kwargs)
```

1. See [:material-code-braces: ListPermissionsRequestRequestTypeDef](./type_defs.md#listpermissionsrequestrequesttypedef) 

### list\_tags\_for\_resource

The <code>ListTagsForResource</code> operation returns the tags that are
associated with the Amazon Managed Service for Grafana resource specified by
the <code>resourceArn</code>.

Type annotations and code completion for `#!python session.create_client("grafana").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_versions

Lists available versions of Grafana.

Type annotations and code completion for `#!python session.create_client("grafana").list_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/list_versions.html)

```python
# list_versions method definition

await def list_versions(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    workspaceId: str = ...,
) -> ListVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVersionsResponseTypeDef](./type_defs.md#listversionsresponsetypedef) 


```python
# list_versions method usage example with argument unpacking

kwargs: ListVersionsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_versions(**kwargs)
```

1. See [:material-code-braces: ListVersionsRequestRequestTypeDef](./type_defs.md#listversionsrequestrequesttypedef) 

### list\_workspace\_service\_account\_tokens

Returns a list of tokens for a workspace service account.

Type annotations and code completion for `#!python session.create_client("grafana").list_workspace_service_account_tokens` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/list_workspace_service_account_tokens.html)

```python
# list_workspace_service_account_tokens method definition

await def list_workspace_service_account_tokens(
    self,
    *,
    serviceAccountId: str,
    workspaceId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListWorkspaceServiceAccountTokensResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkspaceServiceAccountTokensResponseTypeDef](./type_defs.md#listworkspaceserviceaccounttokensresponsetypedef) 


```python
# list_workspace_service_account_tokens method usage example with argument unpacking

kwargs: ListWorkspaceServiceAccountTokensRequestRequestTypeDef = {  # (1)
    "serviceAccountId": ...,
    "workspaceId": ...,
}

parent.list_workspace_service_account_tokens(**kwargs)
```

1. See [:material-code-braces: ListWorkspaceServiceAccountTokensRequestRequestTypeDef](./type_defs.md#listworkspaceserviceaccounttokensrequestrequesttypedef) 

### list\_workspace\_service\_accounts

Returns a list of service accounts for a workspace.

Type annotations and code completion for `#!python session.create_client("grafana").list_workspace_service_accounts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/list_workspace_service_accounts.html)

```python
# list_workspace_service_accounts method definition

await def list_workspace_service_accounts(
    self,
    *,
    workspaceId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListWorkspaceServiceAccountsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkspaceServiceAccountsResponseTypeDef](./type_defs.md#listworkspaceserviceaccountsresponsetypedef) 


```python
# list_workspace_service_accounts method usage example with argument unpacking

kwargs: ListWorkspaceServiceAccountsRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.list_workspace_service_accounts(**kwargs)
```

1. See [:material-code-braces: ListWorkspaceServiceAccountsRequestRequestTypeDef](./type_defs.md#listworkspaceserviceaccountsrequestrequesttypedef) 

### list\_workspaces

Returns a list of Amazon Managed Grafana workspaces in the account, with some
information about each workspace.

Type annotations and code completion for `#!python session.create_client("grafana").list_workspaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/list_workspaces.html)

```python
# list_workspaces method definition

await def list_workspaces(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListWorkspacesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkspacesResponseTypeDef](./type_defs.md#listworkspacesresponsetypedef) 


```python
# list_workspaces method usage example with argument unpacking

kwargs: ListWorkspacesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_workspaces(**kwargs)
```

1. See [:material-code-braces: ListWorkspacesRequestRequestTypeDef](./type_defs.md#listworkspacesrequestrequesttypedef) 

### tag\_resource

The <code>TagResource</code> operation associates tags with an Amazon Managed
Grafana resource.

Type annotations and code completion for `#!python session.create_client("grafana").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

The <code>UntagResource</code> operation removes the association of the tag
with the Amazon Managed Grafana resource.

Type annotations and code completion for `#!python session.create_client("grafana").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_permissions

Updates which users in a workspace have the Grafana <code>Admin</code> or
<code>Editor</code> roles.

Type annotations and code completion for `#!python session.create_client("grafana").update_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/update_permissions.html)

```python
# update_permissions method definition

await def update_permissions(
    self,
    *,
    updateInstructionBatch: Sequence[UpdateInstructionUnionTypeDef],  # (1)
    workspaceId: str,
) -> UpdatePermissionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UpdateInstructionTypeDef](./type_defs.md#updateinstructiontypedef) [:material-code-braces: UpdateInstructionOutputTypeDef](./type_defs.md#updateinstructionoutputtypedef) 
2. See [:material-code-braces: UpdatePermissionsResponseTypeDef](./type_defs.md#updatepermissionsresponsetypedef) 


```python
# update_permissions method usage example with argument unpacking

kwargs: UpdatePermissionsRequestRequestTypeDef = {  # (1)
    "updateInstructionBatch": ...,
    "workspaceId": ...,
}

parent.update_permissions(**kwargs)
```

1. See [:material-code-braces: UpdatePermissionsRequestRequestTypeDef](./type_defs.md#updatepermissionsrequestrequesttypedef) 

### update\_workspace

Modifies an existing Amazon Managed Grafana workspace.

Type annotations and code completion for `#!python session.create_client("grafana").update_workspace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/update_workspace.html)

```python
# update_workspace method definition

await def update_workspace(
    self,
    *,
    workspaceId: str,
    accountAccessType: AccountAccessTypeType = ...,  # (1)
    networkAccessControl: NetworkAccessConfigurationTypeDef = ...,  # (2)
    organizationRoleName: str = ...,
    permissionType: PermissionTypeType = ...,  # (3)
    removeNetworkAccessConfiguration: bool = ...,
    removeVpcConfiguration: bool = ...,
    stackSetName: str = ...,
    vpcConfiguration: VpcConfigurationTypeDef = ...,  # (4)
    workspaceDataSources: Sequence[DataSourceTypeType] = ...,  # (5)
    workspaceDescription: str = ...,
    workspaceName: str = ...,
    workspaceNotificationDestinations: Sequence[NotificationDestinationTypeType] = ...,  # (6)
    workspaceOrganizationalUnits: Sequence[str] = ...,
    workspaceRoleArn: str = ...,
) -> UpdateWorkspaceResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-brackets: AccountAccessTypeType](./literals.md#accountaccesstypetype) 
2. See [:material-code-braces: NetworkAccessConfigurationTypeDef](./type_defs.md#networkaccessconfigurationtypedef) 
3. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
4. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
5. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
6. See [:material-code-brackets: NotificationDestinationTypeType](./literals.md#notificationdestinationtypetype) 
7. See [:material-code-braces: UpdateWorkspaceResponseTypeDef](./type_defs.md#updateworkspaceresponsetypedef) 


```python
# update_workspace method usage example with argument unpacking

kwargs: UpdateWorkspaceRequestRequestTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.update_workspace(**kwargs)
```

1. See [:material-code-braces: UpdateWorkspaceRequestRequestTypeDef](./type_defs.md#updateworkspacerequestrequesttypedef) 

### update\_workspace\_authentication

Use this operation to define the identity provider (IdP) that this workspace
authenticates users from, using SAML.

Type annotations and code completion for `#!python session.create_client("grafana").update_workspace_authentication` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/update_workspace_authentication.html)

```python
# update_workspace_authentication method definition

await def update_workspace_authentication(
    self,
    *,
    authenticationProviders: Sequence[AuthenticationProviderTypesType],  # (1)
    workspaceId: str,
    samlConfiguration: SamlConfigurationTypeDef = ...,  # (2)
) -> UpdateWorkspaceAuthenticationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AuthenticationProviderTypesType](./literals.md#authenticationprovidertypestype) 
2. See [:material-code-braces: SamlConfigurationTypeDef](./type_defs.md#samlconfigurationtypedef) 
3. See [:material-code-braces: UpdateWorkspaceAuthenticationResponseTypeDef](./type_defs.md#updateworkspaceauthenticationresponsetypedef) 


```python
# update_workspace_authentication method usage example with argument unpacking

kwargs: UpdateWorkspaceAuthenticationRequestRequestTypeDef = {  # (1)
    "authenticationProviders": ...,
    "workspaceId": ...,
}

parent.update_workspace_authentication(**kwargs)
```

1. See [:material-code-braces: UpdateWorkspaceAuthenticationRequestRequestTypeDef](./type_defs.md#updateworkspaceauthenticationrequestrequesttypedef) 

### update\_workspace\_configuration

Updates the configuration string for the given workspace.

Type annotations and code completion for `#!python session.create_client("grafana").update_workspace_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/client/update_workspace_configuration.html)

```python
# update_workspace_configuration method definition

await def update_workspace_configuration(
    self,
    *,
    configuration: str,
    workspaceId: str,
    grafanaVersion: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_workspace_configuration method usage example with argument unpacking

kwargs: UpdateWorkspaceConfigurationRequestRequestTypeDef = {  # (1)
    "configuration": ...,
    "workspaceId": ...,
}

parent.update_workspace_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateWorkspaceConfigurationRequestRequestTypeDef](./type_defs.md#updateworkspaceconfigurationrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("grafana").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("grafana").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client)

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

Type annotations and code completion for `#!python session.create_client("grafana").get_paginator` method with overloads.

- `client.get_paginator("list_permissions")` -> [ListPermissionsPaginator](./paginators.md#listpermissionspaginator)
- `client.get_paginator("list_versions")` -> [ListVersionsPaginator](./paginators.md#listversionspaginator)
- `client.get_paginator("list_workspace_service_account_tokens")` -> [ListWorkspaceServiceAccountTokensPaginator](./paginators.md#listworkspaceserviceaccounttokenspaginator)
- `client.get_paginator("list_workspace_service_accounts")` -> [ListWorkspaceServiceAccountsPaginator](./paginators.md#listworkspaceserviceaccountspaginator)
- `client.get_paginator("list_workspaces")` -> [ListWorkspacesPaginator](./paginators.md#listworkspacespaginator)



