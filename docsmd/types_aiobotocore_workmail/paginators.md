# Paginators

> [Index](../README.md) > [WorkMail](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [WorkMail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
    type annotations stubs module [types-aiobotocore-workmail](https://pypi.org/project/types-aiobotocore-workmail/).

## ListAliasesPaginator

Type annotations and code completion for `#!python session.create_client("workmail").get_paginator("list_aliases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListAliases)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListAliasesPaginator

session = get_session()
async with session.create_client("workmail") as client:
    client: WorkMailClient
    paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
```


### paginate

Type annotations and code completion for `#!python ListAliasesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    OrganizationId: str,
    EntityId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAliasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAliasesRequestListAliasesPaginateTypeDef = {  # (1)
    "OrganizationId": ...,
    "EntityId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAliasesRequestListAliasesPaginateTypeDef](./type_defs.md#listaliasesrequestlistaliasespaginatetypedef) 
## ListGroupMembersPaginator

Type annotations and code completion for `#!python session.create_client("workmail").get_paginator("list_group_members")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListGroupMembers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListGroupMembersPaginator

session = get_session()
async with session.create_client("workmail") as client:
    client: WorkMailClient
    paginator: ListGroupMembersPaginator = client.get_paginator("list_group_members")
```


### paginate

Type annotations and code completion for `#!python ListGroupMembersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    OrganizationId: str,
    GroupId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGroupMembersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGroupMembersResponseTypeDef](./type_defs.md#listgroupmembersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListGroupMembersRequestListGroupMembersPaginateTypeDef = {  # (1)
    "OrganizationId": ...,
    "GroupId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupMembersRequestListGroupMembersPaginateTypeDef](./type_defs.md#listgroupmembersrequestlistgroupmemberspaginatetypedef) 
## ListGroupsPaginator

Type annotations and code completion for `#!python session.create_client("workmail").get_paginator("list_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListGroups)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListGroupsPaginator

session = get_session()
async with session.create_client("workmail") as client:
    client: WorkMailClient
    paginator: ListGroupsPaginator = client.get_paginator("list_groups")
```


### paginate

Type annotations and code completion for `#!python ListGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    OrganizationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListGroupsRequestListGroupsPaginateTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupsRequestListGroupsPaginateTypeDef](./type_defs.md#listgroupsrequestlistgroupspaginatetypedef) 
## ListMailboxPermissionsPaginator

Type annotations and code completion for `#!python session.create_client("workmail").get_paginator("list_mailbox_permissions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListMailboxPermissions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListMailboxPermissionsPaginator

session = get_session()
async with session.create_client("workmail") as client:
    client: WorkMailClient
    paginator: ListMailboxPermissionsPaginator = client.get_paginator("list_mailbox_permissions")
```


### paginate

Type annotations and code completion for `#!python ListMailboxPermissionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    OrganizationId: str,
    EntityId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMailboxPermissionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMailboxPermissionsResponseTypeDef](./type_defs.md#listmailboxpermissionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef = {  # (1)
    "OrganizationId": ...,
    "EntityId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef](./type_defs.md#listmailboxpermissionsrequestlistmailboxpermissionspaginatetypedef) 
## ListOrganizationsPaginator

Type annotations and code completion for `#!python session.create_client("workmail").get_paginator("list_organizations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListOrganizations)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListOrganizationsPaginator

session = get_session()
async with session.create_client("workmail") as client:
    client: WorkMailClient
    paginator: ListOrganizationsPaginator = client.get_paginator("list_organizations")
```


### paginate

Type annotations and code completion for `#!python ListOrganizationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListOrganizationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOrganizationsResponseTypeDef](./type_defs.md#listorganizationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListOrganizationsRequestListOrganizationsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOrganizationsRequestListOrganizationsPaginateTypeDef](./type_defs.md#listorganizationsrequestlistorganizationspaginatetypedef) 
## ListResourceDelegatesPaginator

Type annotations and code completion for `#!python session.create_client("workmail").get_paginator("list_resource_delegates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListResourceDelegates)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListResourceDelegatesPaginator

session = get_session()
async with session.create_client("workmail") as client:
    client: WorkMailClient
    paginator: ListResourceDelegatesPaginator = client.get_paginator("list_resource_delegates")
```


### paginate

Type annotations and code completion for `#!python ListResourceDelegatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    OrganizationId: str,
    ResourceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListResourceDelegatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResourceDelegatesResponseTypeDef](./type_defs.md#listresourcedelegatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef = {  # (1)
    "OrganizationId": ...,
    "ResourceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef](./type_defs.md#listresourcedelegatesrequestlistresourcedelegatespaginatetypedef) 
## ListResourcesPaginator

Type annotations and code completion for `#!python session.create_client("workmail").get_paginator("list_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListResources)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListResourcesPaginator

session = get_session()
async with session.create_client("workmail") as client:
    client: WorkMailClient
    paginator: ListResourcesPaginator = client.get_paginator("list_resources")
```


### paginate

Type annotations and code completion for `#!python ListResourcesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    OrganizationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListResourcesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResourcesResponseTypeDef](./type_defs.md#listresourcesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListResourcesRequestListResourcesPaginateTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourcesRequestListResourcesPaginateTypeDef](./type_defs.md#listresourcesrequestlistresourcespaginatetypedef) 
## ListUsersPaginator

Type annotations and code completion for `#!python session.create_client("workmail").get_paginator("list_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListUsers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListUsersPaginator

session = get_session()
async with session.create_client("workmail") as client:
    client: WorkMailClient
    paginator: ListUsersPaginator = client.get_paginator("list_users")
```


### paginate

Type annotations and code completion for `#!python ListUsersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    OrganizationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListUsersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListUsersRequestListUsersPaginateTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestListUsersPaginateTypeDef](./type_defs.md#listusersrequestlistuserspaginatetypedef) 
