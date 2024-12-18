# Paginators

> [Index](../README.md) > [SSOAdmin](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SSOAdmin](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#ssoadmin)
    type annotations stubs module [types-aiobotocore-sso-admin](https://pypi.org/project/types-aiobotocore-sso-admin/).

## ListAccountAssignmentCreationStatusPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_account_assignment_creation_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/paginator/ListAccountAssignmentCreationStatus.html#SSOAdmin.Paginator.ListAccountAssignmentCreationStatus)

```python
# ListAccountAssignmentCreationStatusPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListAccountAssignmentCreationStatusPaginator

session = get_session()
async with session.create_client("sso-admin") as client:  # (1)
    paginator: ListAccountAssignmentCreationStatusPaginator = client.get_paginator("list_account_assignment_creation_status")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccountAssignmentCreationStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [SSOAdminClient](./client.md)
2. paginator: [ListAccountAssignmentCreationStatusPaginator](./paginators.md#listaccountassignmentcreationstatuspaginator)
3. item: [:material-code-braces: ListAccountAssignmentCreationStatusResponseTypeDef](./type_defs.md#listaccountassignmentcreationstatusresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAccountAssignmentCreationStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceArn: str,
    Filter: OperationStatusFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAccountAssignmentCreationStatusResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: OperationStatusFilterTypeDef](./type_defs.md#operationstatusfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAccountAssignmentCreationStatusResponseTypeDef](./type_defs.md#listaccountassignmentcreationstatusresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef = {  # (1)
    "InstanceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef](./type_defs.md#listaccountassignmentcreationstatusrequestlistaccountassignmentcreationstatuspaginatetypedef) 
## ListAccountAssignmentDeletionStatusPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_account_assignment_deletion_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/paginator/ListAccountAssignmentDeletionStatus.html#SSOAdmin.Paginator.ListAccountAssignmentDeletionStatus)

```python
# ListAccountAssignmentDeletionStatusPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListAccountAssignmentDeletionStatusPaginator

session = get_session()
async with session.create_client("sso-admin") as client:  # (1)
    paginator: ListAccountAssignmentDeletionStatusPaginator = client.get_paginator("list_account_assignment_deletion_status")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccountAssignmentDeletionStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [SSOAdminClient](./client.md)
2. paginator: [ListAccountAssignmentDeletionStatusPaginator](./paginators.md#listaccountassignmentdeletionstatuspaginator)
3. item: [:material-code-braces: ListAccountAssignmentDeletionStatusResponseTypeDef](./type_defs.md#listaccountassignmentdeletionstatusresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAccountAssignmentDeletionStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceArn: str,
    Filter: OperationStatusFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAccountAssignmentDeletionStatusResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: OperationStatusFilterTypeDef](./type_defs.md#operationstatusfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAccountAssignmentDeletionStatusResponseTypeDef](./type_defs.md#listaccountassignmentdeletionstatusresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef = {  # (1)
    "InstanceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef](./type_defs.md#listaccountassignmentdeletionstatusrequestlistaccountassignmentdeletionstatuspaginatetypedef) 
## ListAccountAssignmentsForPrincipalPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_account_assignments_for_principal")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/paginator/ListAccountAssignmentsForPrincipal.html#SSOAdmin.Paginator.ListAccountAssignmentsForPrincipal)

```python
# ListAccountAssignmentsForPrincipalPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListAccountAssignmentsForPrincipalPaginator

session = get_session()
async with session.create_client("sso-admin") as client:  # (1)
    paginator: ListAccountAssignmentsForPrincipalPaginator = client.get_paginator("list_account_assignments_for_principal")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccountAssignmentsForPrincipalResponseTypeDef
        print(item)  # (3)
```

1. client: [SSOAdminClient](./client.md)
2. paginator: [ListAccountAssignmentsForPrincipalPaginator](./paginators.md#listaccountassignmentsforprincipalpaginator)
3. item: [:material-code-braces: ListAccountAssignmentsForPrincipalResponseTypeDef](./type_defs.md#listaccountassignmentsforprincipalresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAccountAssignmentsForPrincipalPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceArn: str,
    PrincipalId: str,
    PrincipalType: PrincipalTypeType,  # (1)
    Filter: ListAccountAssignmentsFilterTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListAccountAssignmentsForPrincipalResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-braces: ListAccountAssignmentsFilterTypeDef](./type_defs.md#listaccountassignmentsfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListAccountAssignmentsForPrincipalResponseTypeDef](./type_defs.md#listaccountassignmentsforprincipalresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAccountAssignmentsForPrincipalRequestListAccountAssignmentsForPrincipalPaginateTypeDef = {  # (1)
    "InstanceArn": ...,
    "PrincipalId": ...,
    "PrincipalType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountAssignmentsForPrincipalRequestListAccountAssignmentsForPrincipalPaginateTypeDef](./type_defs.md#listaccountassignmentsforprincipalrequestlistaccountassignmentsforprincipalpaginatetypedef) 
## ListAccountAssignmentsPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_account_assignments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/paginator/ListAccountAssignments.html#SSOAdmin.Paginator.ListAccountAssignments)

```python
# ListAccountAssignmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListAccountAssignmentsPaginator

session = get_session()
async with session.create_client("sso-admin") as client:  # (1)
    paginator: ListAccountAssignmentsPaginator = client.get_paginator("list_account_assignments")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccountAssignmentsResponseTypeDef
        print(item)  # (3)
```

1. client: [SSOAdminClient](./client.md)
2. paginator: [ListAccountAssignmentsPaginator](./paginators.md#listaccountassignmentspaginator)
3. item: [:material-code-braces: ListAccountAssignmentsResponseTypeDef](./type_defs.md#listaccountassignmentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAccountAssignmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccountId: str,
    InstanceArn: str,
    PermissionSetArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAccountAssignmentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAccountAssignmentsResponseTypeDef](./type_defs.md#listaccountassignmentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef = {  # (1)
    "AccountId": ...,
    "InstanceArn": ...,
    "PermissionSetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef](./type_defs.md#listaccountassignmentsrequestlistaccountassignmentspaginatetypedef) 
## ListAccountsForProvisionedPermissionSetPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_accounts_for_provisioned_permission_set")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/paginator/ListAccountsForProvisionedPermissionSet.html#SSOAdmin.Paginator.ListAccountsForProvisionedPermissionSet)

```python
# ListAccountsForProvisionedPermissionSetPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListAccountsForProvisionedPermissionSetPaginator

session = get_session()
async with session.create_client("sso-admin") as client:  # (1)
    paginator: ListAccountsForProvisionedPermissionSetPaginator = client.get_paginator("list_accounts_for_provisioned_permission_set")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccountsForProvisionedPermissionSetResponseTypeDef
        print(item)  # (3)
```

1. client: [SSOAdminClient](./client.md)
2. paginator: [ListAccountsForProvisionedPermissionSetPaginator](./paginators.md#listaccountsforprovisionedpermissionsetpaginator)
3. item: [:material-code-braces: ListAccountsForProvisionedPermissionSetResponseTypeDef](./type_defs.md#listaccountsforprovisionedpermissionsetresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAccountsForProvisionedPermissionSetPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceArn: str,
    PermissionSetArn: str,
    ProvisioningStatus: ProvisioningStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAccountsForProvisionedPermissionSetResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ProvisioningStatusType](./literals.md#provisioningstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAccountsForProvisionedPermissionSetResponseTypeDef](./type_defs.md#listaccountsforprovisionedpermissionsetresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef = {  # (1)
    "InstanceArn": ...,
    "PermissionSetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef](./type_defs.md#listaccountsforprovisionedpermissionsetrequestlistaccountsforprovisionedpermissionsetpaginatetypedef) 
## ListApplicationAccessScopesPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_application_access_scopes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/paginator/ListApplicationAccessScopes.html#SSOAdmin.Paginator.ListApplicationAccessScopes)

```python
# ListApplicationAccessScopesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListApplicationAccessScopesPaginator

session = get_session()
async with session.create_client("sso-admin") as client:  # (1)
    paginator: ListApplicationAccessScopesPaginator = client.get_paginator("list_application_access_scopes")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationAccessScopesResponseTypeDef
        print(item)  # (3)
```

1. client: [SSOAdminClient](./client.md)
2. paginator: [ListApplicationAccessScopesPaginator](./paginators.md#listapplicationaccessscopespaginator)
3. item: [:material-code-braces: ListApplicationAccessScopesResponseTypeDef](./type_defs.md#listapplicationaccessscopesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListApplicationAccessScopesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ApplicationArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListApplicationAccessScopesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListApplicationAccessScopesResponseTypeDef](./type_defs.md#listapplicationaccessscopesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListApplicationAccessScopesRequestListApplicationAccessScopesPaginateTypeDef = {  # (1)
    "ApplicationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationAccessScopesRequestListApplicationAccessScopesPaginateTypeDef](./type_defs.md#listapplicationaccessscopesrequestlistapplicationaccessscopespaginatetypedef) 
## ListApplicationAssignmentsForPrincipalPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_application_assignments_for_principal")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/paginator/ListApplicationAssignmentsForPrincipal.html#SSOAdmin.Paginator.ListApplicationAssignmentsForPrincipal)

```python
# ListApplicationAssignmentsForPrincipalPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListApplicationAssignmentsForPrincipalPaginator

session = get_session()
async with session.create_client("sso-admin") as client:  # (1)
    paginator: ListApplicationAssignmentsForPrincipalPaginator = client.get_paginator("list_application_assignments_for_principal")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationAssignmentsForPrincipalResponseTypeDef
        print(item)  # (3)
```

1. client: [SSOAdminClient](./client.md)
2. paginator: [ListApplicationAssignmentsForPrincipalPaginator](./paginators.md#listapplicationassignmentsforprincipalpaginator)
3. item: [:material-code-braces: ListApplicationAssignmentsForPrincipalResponseTypeDef](./type_defs.md#listapplicationassignmentsforprincipalresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListApplicationAssignmentsForPrincipalPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceArn: str,
    PrincipalId: str,
    PrincipalType: PrincipalTypeType,  # (1)
    Filter: ListApplicationAssignmentsFilterTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListApplicationAssignmentsForPrincipalResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-braces: ListApplicationAssignmentsFilterTypeDef](./type_defs.md#listapplicationassignmentsfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListApplicationAssignmentsForPrincipalResponseTypeDef](./type_defs.md#listapplicationassignmentsforprincipalresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListApplicationAssignmentsForPrincipalRequestListApplicationAssignmentsForPrincipalPaginateTypeDef = {  # (1)
    "InstanceArn": ...,
    "PrincipalId": ...,
    "PrincipalType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationAssignmentsForPrincipalRequestListApplicationAssignmentsForPrincipalPaginateTypeDef](./type_defs.md#listapplicationassignmentsforprincipalrequestlistapplicationassignmentsforprincipalpaginatetypedef) 
## ListApplicationAssignmentsPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_application_assignments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/paginator/ListApplicationAssignments.html#SSOAdmin.Paginator.ListApplicationAssignments)

```python
# ListApplicationAssignmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListApplicationAssignmentsPaginator

session = get_session()
async with session.create_client("sso-admin") as client:  # (1)
    paginator: ListApplicationAssignmentsPaginator = client.get_paginator("list_application_assignments")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationAssignmentsResponseTypeDef
        print(item)  # (3)
```

1. client: [SSOAdminClient](./client.md)
2. paginator: [ListApplicationAssignmentsPaginator](./paginators.md#listapplicationassignmentspaginator)
3. item: [:material-code-braces: ListApplicationAssignmentsResponseTypeDef](./type_defs.md#listapplicationassignmentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListApplicationAssignmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ApplicationArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListApplicationAssignmentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListApplicationAssignmentsResponseTypeDef](./type_defs.md#listapplicationassignmentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListApplicationAssignmentsRequestListApplicationAssignmentsPaginateTypeDef = {  # (1)
    "ApplicationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationAssignmentsRequestListApplicationAssignmentsPaginateTypeDef](./type_defs.md#listapplicationassignmentsrequestlistapplicationassignmentspaginatetypedef) 
## ListApplicationAuthenticationMethodsPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_application_authentication_methods")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/paginator/ListApplicationAuthenticationMethods.html#SSOAdmin.Paginator.ListApplicationAuthenticationMethods)

```python
# ListApplicationAuthenticationMethodsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListApplicationAuthenticationMethodsPaginator

session = get_session()
async with session.create_client("sso-admin") as client:  # (1)
    paginator: ListApplicationAuthenticationMethodsPaginator = client.get_paginator("list_application_authentication_methods")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationAuthenticationMethodsResponseTypeDef
        print(item)  # (3)
```

1. client: [SSOAdminClient](./client.md)
2. paginator: [ListApplicationAuthenticationMethodsPaginator](./paginators.md#listapplicationauthenticationmethodspaginator)
3. item: [:material-code-braces: ListApplicationAuthenticationMethodsResponseTypeDef](./type_defs.md#listapplicationauthenticationmethodsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListApplicationAuthenticationMethodsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ApplicationArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListApplicationAuthenticationMethodsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListApplicationAuthenticationMethodsResponseTypeDef](./type_defs.md#listapplicationauthenticationmethodsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListApplicationAuthenticationMethodsRequestListApplicationAuthenticationMethodsPaginateTypeDef = {  # (1)
    "ApplicationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationAuthenticationMethodsRequestListApplicationAuthenticationMethodsPaginateTypeDef](./type_defs.md#listapplicationauthenticationmethodsrequestlistapplicationauthenticationmethodspaginatetypedef) 
## ListApplicationGrantsPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_application_grants")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/paginator/ListApplicationGrants.html#SSOAdmin.Paginator.ListApplicationGrants)

```python
# ListApplicationGrantsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListApplicationGrantsPaginator

session = get_session()
async with session.create_client("sso-admin") as client:  # (1)
    paginator: ListApplicationGrantsPaginator = client.get_paginator("list_application_grants")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationGrantsResponseTypeDef
        print(item)  # (3)
```

1. client: [SSOAdminClient](./client.md)
2. paginator: [ListApplicationGrantsPaginator](./paginators.md#listapplicationgrantspaginator)
3. item: [:material-code-braces: ListApplicationGrantsResponseTypeDef](./type_defs.md#listapplicationgrantsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListApplicationGrantsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ApplicationArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListApplicationGrantsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListApplicationGrantsResponseTypeDef](./type_defs.md#listapplicationgrantsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListApplicationGrantsRequestListApplicationGrantsPaginateTypeDef = {  # (1)
    "ApplicationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationGrantsRequestListApplicationGrantsPaginateTypeDef](./type_defs.md#listapplicationgrantsrequestlistapplicationgrantspaginatetypedef) 
## ListApplicationProvidersPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_application_providers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/paginator/ListApplicationProviders.html#SSOAdmin.Paginator.ListApplicationProviders)

```python
# ListApplicationProvidersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListApplicationProvidersPaginator

session = get_session()
async with session.create_client("sso-admin") as client:  # (1)
    paginator: ListApplicationProvidersPaginator = client.get_paginator("list_application_providers")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationProvidersResponseTypeDef
        print(item)  # (3)
```

1. client: [SSOAdminClient](./client.md)
2. paginator: [ListApplicationProvidersPaginator](./paginators.md#listapplicationproviderspaginator)
3. item: [:material-code-braces: ListApplicationProvidersResponseTypeDef](./type_defs.md#listapplicationprovidersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListApplicationProvidersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListApplicationProvidersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListApplicationProvidersResponseTypeDef](./type_defs.md#listapplicationprovidersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListApplicationProvidersRequestListApplicationProvidersPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationProvidersRequestListApplicationProvidersPaginateTypeDef](./type_defs.md#listapplicationprovidersrequestlistapplicationproviderspaginatetypedef) 
## ListApplicationsPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/paginator/ListApplications.html#SSOAdmin.Paginator.ListApplications)

```python
# ListApplicationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListApplicationsPaginator

session = get_session()
async with session.create_client("sso-admin") as client:  # (1)
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationsResponseTypeDef
        print(item)  # (3)
```

1. client: [SSOAdminClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListApplicationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceArn: str,
    Filter: ListApplicationsFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListApplicationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ListApplicationsFilterTypeDef](./type_defs.md#listapplicationsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListApplicationsRequestListApplicationsPaginateTypeDef = {  # (1)
    "InstanceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationsRequestListApplicationsPaginateTypeDef](./type_defs.md#listapplicationsrequestlistapplicationspaginatetypedef) 
## ListCustomerManagedPolicyReferencesInPermissionSetPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_customer_managed_policy_references_in_permission_set")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/paginator/ListCustomerManagedPolicyReferencesInPermissionSet.html#SSOAdmin.Paginator.ListCustomerManagedPolicyReferencesInPermissionSet)

```python
# ListCustomerManagedPolicyReferencesInPermissionSetPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListCustomerManagedPolicyReferencesInPermissionSetPaginator

session = get_session()
async with session.create_client("sso-admin") as client:  # (1)
    paginator: ListCustomerManagedPolicyReferencesInPermissionSetPaginator = client.get_paginator("list_customer_managed_policy_references_in_permission_set")  # (2)
    async for item in paginator.paginate(...):
        item: ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef
        print(item)  # (3)
```

1. client: [SSOAdminClient](./client.md)
2. paginator: [ListCustomerManagedPolicyReferencesInPermissionSetPaginator](./paginators.md#listcustomermanagedpolicyreferencesinpermissionsetpaginator)
3. item: [:material-code-braces: ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef](./type_defs.md#listcustomermanagedpolicyreferencesinpermissionsetresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCustomerManagedPolicyReferencesInPermissionSetPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceArn: str,
    PermissionSetArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef](./type_defs.md#listcustomermanagedpolicyreferencesinpermissionsetresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef = {  # (1)
    "InstanceArn": ...,
    "PermissionSetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef](./type_defs.md#listcustomermanagedpolicyreferencesinpermissionsetrequestlistcustomermanagedpolicyreferencesinpermissionsetpaginatetypedef) 
## ListInstancesPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/paginator/ListInstances.html#SSOAdmin.Paginator.ListInstances)

```python
# ListInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListInstancesPaginator

session = get_session()
async with session.create_client("sso-admin") as client:  # (1)
    paginator: ListInstancesPaginator = client.get_paginator("list_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstancesResponseTypeDef
        print(item)  # (3)
```

1. client: [SSOAdminClient](./client.md)
2. paginator: [ListInstancesPaginator](./paginators.md#listinstancespaginator)
3. item: [:material-code-braces: ListInstancesResponseTypeDef](./type_defs.md#listinstancesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListInstancesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInstancesResponseTypeDef](./type_defs.md#listinstancesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListInstancesRequestListInstancesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstancesRequestListInstancesPaginateTypeDef](./type_defs.md#listinstancesrequestlistinstancespaginatetypedef) 
## ListManagedPoliciesInPermissionSetPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_managed_policies_in_permission_set")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/paginator/ListManagedPoliciesInPermissionSet.html#SSOAdmin.Paginator.ListManagedPoliciesInPermissionSet)

```python
# ListManagedPoliciesInPermissionSetPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListManagedPoliciesInPermissionSetPaginator

session = get_session()
async with session.create_client("sso-admin") as client:  # (1)
    paginator: ListManagedPoliciesInPermissionSetPaginator = client.get_paginator("list_managed_policies_in_permission_set")  # (2)
    async for item in paginator.paginate(...):
        item: ListManagedPoliciesInPermissionSetResponseTypeDef
        print(item)  # (3)
```

1. client: [SSOAdminClient](./client.md)
2. paginator: [ListManagedPoliciesInPermissionSetPaginator](./paginators.md#listmanagedpoliciesinpermissionsetpaginator)
3. item: [:material-code-braces: ListManagedPoliciesInPermissionSetResponseTypeDef](./type_defs.md#listmanagedpoliciesinpermissionsetresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListManagedPoliciesInPermissionSetPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceArn: str,
    PermissionSetArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListManagedPoliciesInPermissionSetResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListManagedPoliciesInPermissionSetResponseTypeDef](./type_defs.md#listmanagedpoliciesinpermissionsetresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef = {  # (1)
    "InstanceArn": ...,
    "PermissionSetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef](./type_defs.md#listmanagedpoliciesinpermissionsetrequestlistmanagedpoliciesinpermissionsetpaginatetypedef) 
## ListPermissionSetProvisioningStatusPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_permission_set_provisioning_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/paginator/ListPermissionSetProvisioningStatus.html#SSOAdmin.Paginator.ListPermissionSetProvisioningStatus)

```python
# ListPermissionSetProvisioningStatusPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListPermissionSetProvisioningStatusPaginator

session = get_session()
async with session.create_client("sso-admin") as client:  # (1)
    paginator: ListPermissionSetProvisioningStatusPaginator = client.get_paginator("list_permission_set_provisioning_status")  # (2)
    async for item in paginator.paginate(...):
        item: ListPermissionSetProvisioningStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [SSOAdminClient](./client.md)
2. paginator: [ListPermissionSetProvisioningStatusPaginator](./paginators.md#listpermissionsetprovisioningstatuspaginator)
3. item: [:material-code-braces: ListPermissionSetProvisioningStatusResponseTypeDef](./type_defs.md#listpermissionsetprovisioningstatusresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPermissionSetProvisioningStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceArn: str,
    Filter: OperationStatusFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListPermissionSetProvisioningStatusResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: OperationStatusFilterTypeDef](./type_defs.md#operationstatusfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPermissionSetProvisioningStatusResponseTypeDef](./type_defs.md#listpermissionsetprovisioningstatusresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef = {  # (1)
    "InstanceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef](./type_defs.md#listpermissionsetprovisioningstatusrequestlistpermissionsetprovisioningstatuspaginatetypedef) 
## ListPermissionSetsPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_permission_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/paginator/ListPermissionSets.html#SSOAdmin.Paginator.ListPermissionSets)

```python
# ListPermissionSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListPermissionSetsPaginator

session = get_session()
async with session.create_client("sso-admin") as client:  # (1)
    paginator: ListPermissionSetsPaginator = client.get_paginator("list_permission_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListPermissionSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [SSOAdminClient](./client.md)
2. paginator: [ListPermissionSetsPaginator](./paginators.md#listpermissionsetspaginator)
3. item: [:material-code-braces: ListPermissionSetsResponseTypeDef](./type_defs.md#listpermissionsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPermissionSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPermissionSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPermissionSetsResponseTypeDef](./type_defs.md#listpermissionsetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPermissionSetsRequestListPermissionSetsPaginateTypeDef = {  # (1)
    "InstanceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPermissionSetsRequestListPermissionSetsPaginateTypeDef](./type_defs.md#listpermissionsetsrequestlistpermissionsetspaginatetypedef) 
## ListPermissionSetsProvisionedToAccountPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_permission_sets_provisioned_to_account")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/paginator/ListPermissionSetsProvisionedToAccount.html#SSOAdmin.Paginator.ListPermissionSetsProvisionedToAccount)

```python
# ListPermissionSetsProvisionedToAccountPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListPermissionSetsProvisionedToAccountPaginator

session = get_session()
async with session.create_client("sso-admin") as client:  # (1)
    paginator: ListPermissionSetsProvisionedToAccountPaginator = client.get_paginator("list_permission_sets_provisioned_to_account")  # (2)
    async for item in paginator.paginate(...):
        item: ListPermissionSetsProvisionedToAccountResponseTypeDef
        print(item)  # (3)
```

1. client: [SSOAdminClient](./client.md)
2. paginator: [ListPermissionSetsProvisionedToAccountPaginator](./paginators.md#listpermissionsetsprovisionedtoaccountpaginator)
3. item: [:material-code-braces: ListPermissionSetsProvisionedToAccountResponseTypeDef](./type_defs.md#listpermissionsetsprovisionedtoaccountresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPermissionSetsProvisionedToAccountPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccountId: str,
    InstanceArn: str,
    ProvisioningStatus: ProvisioningStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListPermissionSetsProvisionedToAccountResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ProvisioningStatusType](./literals.md#provisioningstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPermissionSetsProvisionedToAccountResponseTypeDef](./type_defs.md#listpermissionsetsprovisionedtoaccountresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef = {  # (1)
    "AccountId": ...,
    "InstanceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef](./type_defs.md#listpermissionsetsprovisionedtoaccountrequestlistpermissionsetsprovisionedtoaccountpaginatetypedef) 
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/paginator/ListTagsForResource.html#SSOAdmin.Paginator.ListTagsForResource)

```python
# ListTagsForResourcePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("sso-admin") as client:  # (1)
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsForResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [SSOAdminClient](./client.md)
2. paginator: [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
3. item: [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceArn: str,
    InstanceArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTagsForResourceRequestListTagsForResourcePaginateTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestListTagsForResourcePaginateTypeDef](./type_defs.md#listtagsforresourcerequestlisttagsforresourcepaginatetypedef) 
## ListTrustedTokenIssuersPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_trusted_token_issuers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin/paginator/ListTrustedTokenIssuers.html#SSOAdmin.Paginator.ListTrustedTokenIssuers)

```python
# ListTrustedTokenIssuersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListTrustedTokenIssuersPaginator

session = get_session()
async with session.create_client("sso-admin") as client:  # (1)
    paginator: ListTrustedTokenIssuersPaginator = client.get_paginator("list_trusted_token_issuers")  # (2)
    async for item in paginator.paginate(...):
        item: ListTrustedTokenIssuersResponseTypeDef
        print(item)  # (3)
```

1. client: [SSOAdminClient](./client.md)
2. paginator: [ListTrustedTokenIssuersPaginator](./paginators.md#listtrustedtokenissuerspaginator)
3. item: [:material-code-braces: ListTrustedTokenIssuersResponseTypeDef](./type_defs.md#listtrustedtokenissuersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTrustedTokenIssuersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTrustedTokenIssuersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTrustedTokenIssuersResponseTypeDef](./type_defs.md#listtrustedtokenissuersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTrustedTokenIssuersRequestListTrustedTokenIssuersPaginateTypeDef = {  # (1)
    "InstanceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTrustedTokenIssuersRequestListTrustedTokenIssuersPaginateTypeDef](./type_defs.md#listtrustedtokenissuersrequestlisttrustedtokenissuerspaginatetypedef) 
