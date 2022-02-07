<a id="paginators-for-aiobotocore-managedgrafana-module"></a>

# Paginators for aiobotocore ManagedGrafana module

> [Index](..) > [ManagedGrafana](.) > Paginators

Auto-generated documentation for
[ManagedGrafana](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
type annotations stubs module
[types-aiobotocore-grafana](https://pypi.org/project/types-aiobotocore-grafana/).

- [Paginators for aiobotocore ManagedGrafana module](#paginators-for-aiobotocore-managedgrafana-module)
  - [ListPermissionsPaginator](#listpermissionspaginator)
  - [ListWorkspacesPaginator](#listworkspacespaginator)

<a id="listpermissionspaginator"></a>

## ListPermissionsPaginator

Type annotations for
`session.create_client("grafana").get_paginator("list_permissions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_grafana.paginator import ListPermissionsPaginator

session = get_session()
async with session.create_client("grafana") as client:
    client: ManagedGrafanaClient
    paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")
```

Boto3 documentation:
[ManagedGrafana.Paginator.ListPermissions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListPermissions)

Arguments for `ListPermissionsPaginator.paginate` method:

- `workspaceId`: `str` *(required)*
- `groupId`: `str`
- `userId`: `str`
- `userType`: [UserTypeType](./literals.md#usertypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPermissionsPaginator.paginate` returns
`_PageIterator`\[[ListPermissionsResponseTypeDef](./type_defs.md#listpermissionsresponsetypedef)\].

<a id="listworkspacespaginator"></a>

## ListWorkspacesPaginator

Type annotations for
`session.create_client("grafana").get_paginator("list_workspaces")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_grafana.paginator import ListWorkspacesPaginator

session = get_session()
async with session.create_client("grafana") as client:
    client: ManagedGrafanaClient
    paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")
```

Boto3 documentation:
[ManagedGrafana.Paginator.ListWorkspaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListWorkspaces)

Arguments for `ListWorkspacesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListWorkspacesPaginator.paginate` returns
`_PageIterator`\[[ListWorkspacesResponseTypeDef](./type_defs.md#listworkspacesresponsetypedef)\].
