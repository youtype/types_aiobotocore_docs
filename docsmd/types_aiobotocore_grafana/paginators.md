# Paginators

> [Index](../README.md) > [ManagedGrafana](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ManagedGrafana](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#managedgrafana)
    type annotations stubs module [types-aiobotocore-grafana](https://pypi.org/project/types-aiobotocore-grafana/).

## ListPermissionsPaginator

Type annotations and code completion for `#!python session.create_client("grafana").get_paginator("list_permissions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/paginator/ListPermissions.html#ManagedGrafana.Paginator.ListPermissions)

```python
# ListPermissionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_grafana.paginator import ListPermissionsPaginator

session = get_session()
async with session.create_client("grafana") as client:  # (1)
    paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")  # (2)
    async for item in paginator.paginate(...):
        item: ListPermissionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ManagedGrafanaClient](./client.md)
2. paginator: [ListPermissionsPaginator](./paginators.md#listpermissionspaginator)
3. item: `AioPageIterator[ListPermissionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPermissionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    workspaceId: str,
    groupId: str = ...,
    userId: str = ...,
    userType: UserTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListPermissionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListPermissionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPermissionsRequestPaginateTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPermissionsRequestPaginateTypeDef](./type_defs.md#listpermissionsrequestpaginatetypedef)
## ListVersionsPaginator

Type annotations and code completion for `#!python session.create_client("grafana").get_paginator("list_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/paginator/ListVersions.html#ManagedGrafana.Paginator.ListVersions)

```python
# ListVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_grafana.paginator import ListVersionsPaginator

session = get_session()
async with session.create_client("grafana") as client:  # (1)
    paginator: ListVersionsPaginator = client.get_paginator("list_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ManagedGrafanaClient](./client.md)
2. paginator: [ListVersionsPaginator](./paginators.md#listversionspaginator)
3. item: `AioPageIterator[ListVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    workspaceId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListVersionsRequestPaginateTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVersionsRequestPaginateTypeDef](./type_defs.md#listversionsrequestpaginatetypedef)
## ListWorkspaceServiceAccountTokensPaginator

Type annotations and code completion for `#!python session.create_client("grafana").get_paginator("list_workspace_service_account_tokens")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/paginator/ListWorkspaceServiceAccountTokens.html#ManagedGrafana.Paginator.ListWorkspaceServiceAccountTokens)

```python
# ListWorkspaceServiceAccountTokensPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_grafana.paginator import ListWorkspaceServiceAccountTokensPaginator

session = get_session()
async with session.create_client("grafana") as client:  # (1)
    paginator: ListWorkspaceServiceAccountTokensPaginator = client.get_paginator("list_workspace_service_account_tokens")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkspaceServiceAccountTokensResponseTypeDef
        print(item)  # (3)
```

1. client: [ManagedGrafanaClient](./client.md)
2. paginator: [ListWorkspaceServiceAccountTokensPaginator](./paginators.md#listworkspaceserviceaccounttokenspaginator)
3. item: `AioPageIterator[ListWorkspaceServiceAccountTokensResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListWorkspaceServiceAccountTokensPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    serviceAccountId: str,
    workspaceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListWorkspaceServiceAccountTokensResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListWorkspaceServiceAccountTokensResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkspaceServiceAccountTokensRequestPaginateTypeDef = {  # (1)
    "serviceAccountId": ...,
    "workspaceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkspaceServiceAccountTokensRequestPaginateTypeDef](./type_defs.md#listworkspaceserviceaccounttokensrequestpaginatetypedef)
## ListWorkspaceServiceAccountsPaginator

Type annotations and code completion for `#!python session.create_client("grafana").get_paginator("list_workspace_service_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/paginator/ListWorkspaceServiceAccounts.html#ManagedGrafana.Paginator.ListWorkspaceServiceAccounts)

```python
# ListWorkspaceServiceAccountsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_grafana.paginator import ListWorkspaceServiceAccountsPaginator

session = get_session()
async with session.create_client("grafana") as client:  # (1)
    paginator: ListWorkspaceServiceAccountsPaginator = client.get_paginator("list_workspace_service_accounts")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkspaceServiceAccountsResponseTypeDef
        print(item)  # (3)
```

1. client: [ManagedGrafanaClient](./client.md)
2. paginator: [ListWorkspaceServiceAccountsPaginator](./paginators.md#listworkspaceserviceaccountspaginator)
3. item: `AioPageIterator[ListWorkspaceServiceAccountsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListWorkspaceServiceAccountsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    workspaceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListWorkspaceServiceAccountsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListWorkspaceServiceAccountsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkspaceServiceAccountsRequestPaginateTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkspaceServiceAccountsRequestPaginateTypeDef](./type_defs.md#listworkspaceserviceaccountsrequestpaginatetypedef)
## ListWorkspacesPaginator

Type annotations and code completion for `#!python session.create_client("grafana").get_paginator("list_workspaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana/paginator/ListWorkspaces.html#ManagedGrafana.Paginator.ListWorkspaces)

```python
# ListWorkspacesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_grafana.paginator import ListWorkspacesPaginator

session = get_session()
async with session.create_client("grafana") as client:  # (1)
    paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkspacesResponseTypeDef
        print(item)  # (3)
```

1. client: [ManagedGrafanaClient](./client.md)
2. paginator: [ListWorkspacesPaginator](./paginators.md#listworkspacespaginator)
3. item: `AioPageIterator[ListWorkspacesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListWorkspacesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListWorkspacesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListWorkspacesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkspacesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkspacesRequestPaginateTypeDef](./type_defs.md#listworkspacesrequestpaginatetypedef)
