# Paginators

> [Index](../README.md) > [WorkMail](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [WorkMail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#workmail)
    type annotations stubs module [types-aiobotocore-workmail](https://pypi.org/project/types-aiobotocore-workmail/).

## ListAliasesPaginator

Type annotations and code completion for `#!python session.create_client("workmail").get_paginator("list_aliases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/paginator/ListAliases.html#WorkMail.Paginator.ListAliases)

```python
# ListAliasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListAliasesPaginator

session = get_session()
async with session.create_client("workmail") as client:  # (1)
    paginator: ListAliasesPaginator = client.get_paginator("list_aliases")  # (2)
    async for item in paginator.paginate(...):
        item: ListAliasesResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkMailClient](./client.md)
2. paginator: [ListAliasesPaginator](./paginators.md#listaliasespaginator)
3. item: [:material-code-braces: ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAliasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OrganizationId: str,
    EntityId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAliasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAliasesRequestPaginateTypeDef = {  # (1)
    "OrganizationId": ...,
    "EntityId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAliasesRequestPaginateTypeDef](./type_defs.md#listaliasesrequestpaginatetypedef) 
## ListAvailabilityConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("workmail").get_paginator("list_availability_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/paginator/ListAvailabilityConfigurations.html#WorkMail.Paginator.ListAvailabilityConfigurations)

```python
# ListAvailabilityConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListAvailabilityConfigurationsPaginator

session = get_session()
async with session.create_client("workmail") as client:  # (1)
    paginator: ListAvailabilityConfigurationsPaginator = client.get_paginator("list_availability_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListAvailabilityConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkMailClient](./client.md)
2. paginator: [ListAvailabilityConfigurationsPaginator](./paginators.md#listavailabilityconfigurationspaginator)
3. item: [:material-code-braces: ListAvailabilityConfigurationsResponseTypeDef](./type_defs.md#listavailabilityconfigurationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAvailabilityConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OrganizationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAvailabilityConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAvailabilityConfigurationsResponseTypeDef](./type_defs.md#listavailabilityconfigurationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAvailabilityConfigurationsRequestPaginateTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAvailabilityConfigurationsRequestPaginateTypeDef](./type_defs.md#listavailabilityconfigurationsrequestpaginatetypedef) 
## ListGroupMembersPaginator

Type annotations and code completion for `#!python session.create_client("workmail").get_paginator("list_group_members")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/paginator/ListGroupMembers.html#WorkMail.Paginator.ListGroupMembers)

```python
# ListGroupMembersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListGroupMembersPaginator

session = get_session()
async with session.create_client("workmail") as client:  # (1)
    paginator: ListGroupMembersPaginator = client.get_paginator("list_group_members")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupMembersResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkMailClient](./client.md)
2. paginator: [ListGroupMembersPaginator](./paginators.md#listgroupmemberspaginator)
3. item: [:material-code-braces: ListGroupMembersResponseTypeDef](./type_defs.md#listgroupmembersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupMembersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OrganizationId: str,
    GroupId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListGroupMembersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGroupMembersResponseTypeDef](./type_defs.md#listgroupmembersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGroupMembersRequestPaginateTypeDef = {  # (1)
    "OrganizationId": ...,
    "GroupId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupMembersRequestPaginateTypeDef](./type_defs.md#listgroupmembersrequestpaginatetypedef) 
## ListGroupsPaginator

Type annotations and code completion for `#!python session.create_client("workmail").get_paginator("list_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/paginator/ListGroups.html#WorkMail.Paginator.ListGroups)

```python
# ListGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListGroupsPaginator

session = get_session()
async with session.create_client("workmail") as client:  # (1)
    paginator: ListGroupsPaginator = client.get_paginator("list_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkMailClient](./client.md)
2. paginator: [ListGroupsPaginator](./paginators.md#listgroupspaginator)
3. item: [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OrganizationId: str,
    Filters: ListGroupsFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListGroupsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ListGroupsFiltersTypeDef](./type_defs.md#listgroupsfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGroupsRequestPaginateTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupsRequestPaginateTypeDef](./type_defs.md#listgroupsrequestpaginatetypedef) 
## ListMailboxPermissionsPaginator

Type annotations and code completion for `#!python session.create_client("workmail").get_paginator("list_mailbox_permissions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/paginator/ListMailboxPermissions.html#WorkMail.Paginator.ListMailboxPermissions)

```python
# ListMailboxPermissionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListMailboxPermissionsPaginator

session = get_session()
async with session.create_client("workmail") as client:  # (1)
    paginator: ListMailboxPermissionsPaginator = client.get_paginator("list_mailbox_permissions")  # (2)
    async for item in paginator.paginate(...):
        item: ListMailboxPermissionsResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkMailClient](./client.md)
2. paginator: [ListMailboxPermissionsPaginator](./paginators.md#listmailboxpermissionspaginator)
3. item: [:material-code-braces: ListMailboxPermissionsResponseTypeDef](./type_defs.md#listmailboxpermissionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMailboxPermissionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OrganizationId: str,
    EntityId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListMailboxPermissionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMailboxPermissionsResponseTypeDef](./type_defs.md#listmailboxpermissionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMailboxPermissionsRequestPaginateTypeDef = {  # (1)
    "OrganizationId": ...,
    "EntityId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMailboxPermissionsRequestPaginateTypeDef](./type_defs.md#listmailboxpermissionsrequestpaginatetypedef) 
## ListOrganizationsPaginator

Type annotations and code completion for `#!python session.create_client("workmail").get_paginator("list_organizations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/paginator/ListOrganizations.html#WorkMail.Paginator.ListOrganizations)

```python
# ListOrganizationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListOrganizationsPaginator

session = get_session()
async with session.create_client("workmail") as client:  # (1)
    paginator: ListOrganizationsPaginator = client.get_paginator("list_organizations")  # (2)
    async for item in paginator.paginate(...):
        item: ListOrganizationsResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkMailClient](./client.md)
2. paginator: [ListOrganizationsPaginator](./paginators.md#listorganizationspaginator)
3. item: [:material-code-braces: ListOrganizationsResponseTypeDef](./type_defs.md#listorganizationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListOrganizationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListOrganizationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOrganizationsResponseTypeDef](./type_defs.md#listorganizationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListOrganizationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOrganizationsRequestPaginateTypeDef](./type_defs.md#listorganizationsrequestpaginatetypedef) 
## ListPersonalAccessTokensPaginator

Type annotations and code completion for `#!python session.create_client("workmail").get_paginator("list_personal_access_tokens")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/paginator/ListPersonalAccessTokens.html#WorkMail.Paginator.ListPersonalAccessTokens)

```python
# ListPersonalAccessTokensPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListPersonalAccessTokensPaginator

session = get_session()
async with session.create_client("workmail") as client:  # (1)
    paginator: ListPersonalAccessTokensPaginator = client.get_paginator("list_personal_access_tokens")  # (2)
    async for item in paginator.paginate(...):
        item: ListPersonalAccessTokensResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkMailClient](./client.md)
2. paginator: [ListPersonalAccessTokensPaginator](./paginators.md#listpersonalaccesstokenspaginator)
3. item: [:material-code-braces: ListPersonalAccessTokensResponseTypeDef](./type_defs.md#listpersonalaccesstokensresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPersonalAccessTokensPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OrganizationId: str,
    UserId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPersonalAccessTokensResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPersonalAccessTokensResponseTypeDef](./type_defs.md#listpersonalaccesstokensresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPersonalAccessTokensRequestPaginateTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPersonalAccessTokensRequestPaginateTypeDef](./type_defs.md#listpersonalaccesstokensrequestpaginatetypedef) 
## ListResourceDelegatesPaginator

Type annotations and code completion for `#!python session.create_client("workmail").get_paginator("list_resource_delegates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/paginator/ListResourceDelegates.html#WorkMail.Paginator.ListResourceDelegates)

```python
# ListResourceDelegatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListResourceDelegatesPaginator

session = get_session()
async with session.create_client("workmail") as client:  # (1)
    paginator: ListResourceDelegatesPaginator = client.get_paginator("list_resource_delegates")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceDelegatesResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkMailClient](./client.md)
2. paginator: [ListResourceDelegatesPaginator](./paginators.md#listresourcedelegatespaginator)
3. item: [:material-code-braces: ListResourceDelegatesResponseTypeDef](./type_defs.md#listresourcedelegatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResourceDelegatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OrganizationId: str,
    ResourceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListResourceDelegatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResourceDelegatesResponseTypeDef](./type_defs.md#listresourcedelegatesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResourceDelegatesRequestPaginateTypeDef = {  # (1)
    "OrganizationId": ...,
    "ResourceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceDelegatesRequestPaginateTypeDef](./type_defs.md#listresourcedelegatesrequestpaginatetypedef) 
## ListResourcesPaginator

Type annotations and code completion for `#!python session.create_client("workmail").get_paginator("list_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/paginator/ListResources.html#WorkMail.Paginator.ListResources)

```python
# ListResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListResourcesPaginator

session = get_session()
async with session.create_client("workmail") as client:  # (1)
    paginator: ListResourcesPaginator = client.get_paginator("list_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkMailClient](./client.md)
2. paginator: [ListResourcesPaginator](./paginators.md#listresourcespaginator)
3. item: [:material-code-braces: ListResourcesResponseTypeDef](./type_defs.md#listresourcesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OrganizationId: str,
    Filters: ListResourcesFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListResourcesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ListResourcesFiltersTypeDef](./type_defs.md#listresourcesfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListResourcesResponseTypeDef](./type_defs.md#listresourcesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResourcesRequestPaginateTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourcesRequestPaginateTypeDef](./type_defs.md#listresourcesrequestpaginatetypedef) 
## ListUsersPaginator

Type annotations and code completion for `#!python session.create_client("workmail").get_paginator("list_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail/paginator/ListUsers.html#WorkMail.Paginator.ListUsers)

```python
# ListUsersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListUsersPaginator

session = get_session()
async with session.create_client("workmail") as client:  # (1)
    paginator: ListUsersPaginator = client.get_paginator("list_users")  # (2)
    async for item in paginator.paginate(...):
        item: ListUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkMailClient](./client.md)
2. paginator: [ListUsersPaginator](./paginators.md#listuserspaginator)
3. item: [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUsersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OrganizationId: str,
    Filters: ListUsersFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListUsersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ListUsersFiltersTypeDef](./type_defs.md#listusersfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListUsersRequestPaginateTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestPaginateTypeDef](./type_defs.md#listusersrequestpaginatetypedef) 
