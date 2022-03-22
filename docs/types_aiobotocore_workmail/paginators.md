<a id="paginators-for-aiobotocore-workmail-module"></a>

# Paginators for aiobotocore WorkMail module

> [Index](../README.md) > [WorkMail](./README.md) > Paginators

Auto-generated documentation for
[WorkMail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
type annotations stubs module
[types-aiobotocore-workmail](https://pypi.org/project/types-aiobotocore-workmail/).

- [Paginators for aiobotocore WorkMail module](#paginators-for-aiobotocore-workmail-module)
  - [ListAliasesPaginator](#listaliasespaginator)
  - [ListGroupMembersPaginator](#listgroupmemberspaginator)
  - [ListGroupsPaginator](#listgroupspaginator)
  - [ListMailboxPermissionsPaginator](#listmailboxpermissionspaginator)
  - [ListOrganizationsPaginator](#listorganizationspaginator)
  - [ListResourceDelegatesPaginator](#listresourcedelegatespaginator)
  - [ListResourcesPaginator](#listresourcespaginator)
  - [ListUsersPaginator](#listuserspaginator)

<a id="listaliasespaginator"></a>

## ListAliasesPaginator

Type annotations for
`session.create_client("workmail").get_paginator("list_aliases")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListAliasesPaginator

session = get_session()
async with session.create_client("workmail") as client:
    client: WorkMailClient
    paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
```

Boto3 documentation:
[WorkMail.Paginator.ListAliases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListAliases)

Arguments for `ListAliasesPaginator.paginate` method:

- `OrganizationId`: `str` *(required)*
- `EntityId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAliasesPaginator.paginate` returns
`AsyncIterator`\[[ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef)\].

<a id="listgroupmemberspaginator"></a>

## ListGroupMembersPaginator

Type annotations for
`session.create_client("workmail").get_paginator("list_group_members")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListGroupMembersPaginator

session = get_session()
async with session.create_client("workmail") as client:
    client: WorkMailClient
    paginator: ListGroupMembersPaginator = client.get_paginator("list_group_members")
```

Boto3 documentation:
[WorkMail.Paginator.ListGroupMembers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListGroupMembers)

Arguments for `ListGroupMembersPaginator.paginate` method:

- `OrganizationId`: `str` *(required)*
- `GroupId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListGroupMembersPaginator.paginate` returns
`AsyncIterator`\[[ListGroupMembersResponseTypeDef](./type_defs.md#listgroupmembersresponsetypedef)\].

<a id="listgroupspaginator"></a>

## ListGroupsPaginator

Type annotations for
`session.create_client("workmail").get_paginator("list_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListGroupsPaginator

session = get_session()
async with session.create_client("workmail") as client:
    client: WorkMailClient
    paginator: ListGroupsPaginator = client.get_paginator("list_groups")
```

Boto3 documentation:
[WorkMail.Paginator.ListGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListGroups)

Arguments for `ListGroupsPaginator.paginate` method:

- `OrganizationId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListGroupsPaginator.paginate` returns
`AsyncIterator`\[[ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef)\].

<a id="listmailboxpermissionspaginator"></a>

## ListMailboxPermissionsPaginator

Type annotations for
`session.create_client("workmail").get_paginator("list_mailbox_permissions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListMailboxPermissionsPaginator

session = get_session()
async with session.create_client("workmail") as client:
    client: WorkMailClient
    paginator: ListMailboxPermissionsPaginator = client.get_paginator("list_mailbox_permissions")
```

Boto3 documentation:
[WorkMail.Paginator.ListMailboxPermissions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListMailboxPermissions)

Arguments for `ListMailboxPermissionsPaginator.paginate` method:

- `OrganizationId`: `str` *(required)*
- `EntityId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListMailboxPermissionsPaginator.paginate` returns
`AsyncIterator`\[[ListMailboxPermissionsResponseTypeDef](./type_defs.md#listmailboxpermissionsresponsetypedef)\].

<a id="listorganizationspaginator"></a>

## ListOrganizationsPaginator

Type annotations for
`session.create_client("workmail").get_paginator("list_organizations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListOrganizationsPaginator

session = get_session()
async with session.create_client("workmail") as client:
    client: WorkMailClient
    paginator: ListOrganizationsPaginator = client.get_paginator("list_organizations")
```

Boto3 documentation:
[WorkMail.Paginator.ListOrganizations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListOrganizations)

Arguments for `ListOrganizationsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListOrganizationsPaginator.paginate` returns
`AsyncIterator`\[[ListOrganizationsResponseTypeDef](./type_defs.md#listorganizationsresponsetypedef)\].

<a id="listresourcedelegatespaginator"></a>

## ListResourceDelegatesPaginator

Type annotations for
`session.create_client("workmail").get_paginator("list_resource_delegates")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListResourceDelegatesPaginator

session = get_session()
async with session.create_client("workmail") as client:
    client: WorkMailClient
    paginator: ListResourceDelegatesPaginator = client.get_paginator("list_resource_delegates")
```

Boto3 documentation:
[WorkMail.Paginator.ListResourceDelegates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListResourceDelegates)

Arguments for `ListResourceDelegatesPaginator.paginate` method:

- `OrganizationId`: `str` *(required)*
- `ResourceId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListResourceDelegatesPaginator.paginate` returns
`AsyncIterator`\[[ListResourceDelegatesResponseTypeDef](./type_defs.md#listresourcedelegatesresponsetypedef)\].

<a id="listresourcespaginator"></a>

## ListResourcesPaginator

Type annotations for
`session.create_client("workmail").get_paginator("list_resources")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListResourcesPaginator

session = get_session()
async with session.create_client("workmail") as client:
    client: WorkMailClient
    paginator: ListResourcesPaginator = client.get_paginator("list_resources")
```

Boto3 documentation:
[WorkMail.Paginator.ListResources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListResources)

Arguments for `ListResourcesPaginator.paginate` method:

- `OrganizationId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListResourcesPaginator.paginate` returns
`AsyncIterator`\[[ListResourcesResponseTypeDef](./type_defs.md#listresourcesresponsetypedef)\].

<a id="listuserspaginator"></a>

## ListUsersPaginator

Type annotations for
`session.create_client("workmail").get_paginator("list_users")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_workmail.paginator import ListUsersPaginator

session = get_session()
async with session.create_client("workmail") as client:
    client: WorkMailClient
    paginator: ListUsersPaginator = client.get_paginator("list_users")
```

Boto3 documentation:
[WorkMail.Paginator.ListUsers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListUsers)

Arguments for `ListUsersPaginator.paginate` method:

- `OrganizationId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListUsersPaginator.paginate` returns
`AsyncIterator`\[[ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef)\].
