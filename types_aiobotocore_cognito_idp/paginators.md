<a id="paginators-for-aiobotocore-cognitoidentityprovider-module"></a>

# Paginators for aiobotocore CognitoIdentityProvider module

> [Index](..) > [CognitoIdentityProvider](.) > Paginators

Auto-generated documentation for
[CognitoIdentityProvider](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
type annotations stubs module
[types-aiobotocore-cognito-idp](https://pypi.org/project/types-aiobotocore-cognito-idp/).

- [Paginators for aiobotocore CognitoIdentityProvider module](#paginators-for-aiobotocore-cognitoidentityprovider-module)
  - [AdminListGroupsForUserPaginator](#adminlistgroupsforuserpaginator)
  - [AdminListUserAuthEventsPaginator](#adminlistuserautheventspaginator)
  - [ListGroupsPaginator](#listgroupspaginator)
  - [ListIdentityProvidersPaginator](#listidentityproviderspaginator)
  - [ListResourceServersPaginator](#listresourceserverspaginator)
  - [ListUserPoolClientsPaginator](#listuserpoolclientspaginator)
  - [ListUserPoolsPaginator](#listuserpoolspaginator)
  - [ListUsersPaginator](#listuserspaginator)
  - [ListUsersInGroupPaginator](#listusersingrouppaginator)

<a id="adminlistgroupsforuserpaginator"></a>

## AdminListGroupsForUserPaginator

Type annotations for
`session.create_client("cognito-idp").get_paginator("admin_list_groups_for_user")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cognito_idp.paginator import AdminListGroupsForUserPaginator

session = get_session()
async with session.create_client("cognito-idp") as client:
    client: CognitoIdentityProviderClient
    paginator: AdminListGroupsForUserPaginator = client.get_paginator("admin_list_groups_for_user")
```

Boto3 documentation:
[CognitoIdentityProvider.Paginator.AdminListGroupsForUser](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser)

Arguments for `AdminListGroupsForUserPaginator.paginate` method:

- `Username`: `str` *(required)*
- `UserPoolId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`AdminListGroupsForUserPaginator.paginate` returns
`AsyncIterable`\[[AdminListGroupsForUserResponseTypeDef](./type_defs.md#adminlistgroupsforuserresponsetypedef)\].

<a id="adminlistuserautheventspaginator"></a>

## AdminListUserAuthEventsPaginator

Type annotations for
`session.create_client("cognito-idp").get_paginator("admin_list_user_auth_events")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cognito_idp.paginator import AdminListUserAuthEventsPaginator

session = get_session()
async with session.create_client("cognito-idp") as client:
    client: CognitoIdentityProviderClient
    paginator: AdminListUserAuthEventsPaginator = client.get_paginator("admin_list_user_auth_events")
```

Boto3 documentation:
[CognitoIdentityProvider.Paginator.AdminListUserAuthEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents)

Arguments for `AdminListUserAuthEventsPaginator.paginate` method:

- `UserPoolId`: `str` *(required)*
- `Username`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`AdminListUserAuthEventsPaginator.paginate` returns
`AsyncIterable`\[[AdminListUserAuthEventsResponseTypeDef](./type_defs.md#adminlistuserautheventsresponsetypedef)\].

<a id="listgroupspaginator"></a>

## ListGroupsPaginator

Type annotations for
`session.create_client("cognito-idp").get_paginator("list_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cognito_idp.paginator import ListGroupsPaginator

session = get_session()
async with session.create_client("cognito-idp") as client:
    client: CognitoIdentityProviderClient
    paginator: ListGroupsPaginator = client.get_paginator("list_groups")
```

Boto3 documentation:
[CognitoIdentityProvider.Paginator.ListGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListGroups)

Arguments for `ListGroupsPaginator.paginate` method:

- `UserPoolId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListGroupsPaginator.paginate` returns
`AsyncIterable`\[[ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef)\].

<a id="listidentityproviderspaginator"></a>

## ListIdentityProvidersPaginator

Type annotations for
`session.create_client("cognito-idp").get_paginator("list_identity_providers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cognito_idp.paginator import ListIdentityProvidersPaginator

session = get_session()
async with session.create_client("cognito-idp") as client:
    client: CognitoIdentityProviderClient
    paginator: ListIdentityProvidersPaginator = client.get_paginator("list_identity_providers")
```

Boto3 documentation:
[CognitoIdentityProvider.Paginator.ListIdentityProviders](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListIdentityProviders)

Arguments for `ListIdentityProvidersPaginator.paginate` method:

- `UserPoolId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListIdentityProvidersPaginator.paginate` returns
`AsyncIterable`\[[ListIdentityProvidersResponseTypeDef](./type_defs.md#listidentityprovidersresponsetypedef)\].

<a id="listresourceserverspaginator"></a>

## ListResourceServersPaginator

Type annotations for
`session.create_client("cognito-idp").get_paginator("list_resource_servers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cognito_idp.paginator import ListResourceServersPaginator

session = get_session()
async with session.create_client("cognito-idp") as client:
    client: CognitoIdentityProviderClient
    paginator: ListResourceServersPaginator = client.get_paginator("list_resource_servers")
```

Boto3 documentation:
[CognitoIdentityProvider.Paginator.ListResourceServers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListResourceServers)

Arguments for `ListResourceServersPaginator.paginate` method:

- `UserPoolId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListResourceServersPaginator.paginate` returns
`AsyncIterable`\[[ListResourceServersResponseTypeDef](./type_defs.md#listresourceserversresponsetypedef)\].

<a id="listuserpoolclientspaginator"></a>

## ListUserPoolClientsPaginator

Type annotations for
`session.create_client("cognito-idp").get_paginator("list_user_pool_clients")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cognito_idp.paginator import ListUserPoolClientsPaginator

session = get_session()
async with session.create_client("cognito-idp") as client:
    client: CognitoIdentityProviderClient
    paginator: ListUserPoolClientsPaginator = client.get_paginator("list_user_pool_clients")
```

Boto3 documentation:
[CognitoIdentityProvider.Paginator.ListUserPoolClients](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPoolClients)

Arguments for `ListUserPoolClientsPaginator.paginate` method:

- `UserPoolId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListUserPoolClientsPaginator.paginate` returns
`AsyncIterable`\[[ListUserPoolClientsResponseTypeDef](./type_defs.md#listuserpoolclientsresponsetypedef)\].

<a id="listuserpoolspaginator"></a>

## ListUserPoolsPaginator

Type annotations for
`session.create_client("cognito-idp").get_paginator("list_user_pools")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cognito_idp.paginator import ListUserPoolsPaginator

session = get_session()
async with session.create_client("cognito-idp") as client:
    client: CognitoIdentityProviderClient
    paginator: ListUserPoolsPaginator = client.get_paginator("list_user_pools")
```

Boto3 documentation:
[CognitoIdentityProvider.Paginator.ListUserPools](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPools)

Arguments for `ListUserPoolsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListUserPoolsPaginator.paginate` returns
`AsyncIterable`\[[ListUserPoolsResponseTypeDef](./type_defs.md#listuserpoolsresponsetypedef)\].

<a id="listuserspaginator"></a>

## ListUsersPaginator

Type annotations for
`session.create_client("cognito-idp").get_paginator("list_users")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cognito_idp.paginator import ListUsersPaginator

session = get_session()
async with session.create_client("cognito-idp") as client:
    client: CognitoIdentityProviderClient
    paginator: ListUsersPaginator = client.get_paginator("list_users")
```

Boto3 documentation:
[CognitoIdentityProvider.Paginator.ListUsers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsers)

Arguments for `ListUsersPaginator.paginate` method:

- `UserPoolId`: `str` *(required)*
- `AttributesToGet`: `Sequence`\[`str`\]
- `Filter`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListUsersPaginator.paginate` returns
`AsyncIterable`\[[ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef)\].

<a id="listusersingrouppaginator"></a>

## ListUsersInGroupPaginator

Type annotations for
`session.create_client("cognito-idp").get_paginator("list_users_in_group")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cognito_idp.paginator import ListUsersInGroupPaginator

session = get_session()
async with session.create_client("cognito-idp") as client:
    client: CognitoIdentityProviderClient
    paginator: ListUsersInGroupPaginator = client.get_paginator("list_users_in_group")
```

Boto3 documentation:
[CognitoIdentityProvider.Paginator.ListUsersInGroup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsersInGroup)

Arguments for `ListUsersInGroupPaginator.paginate` method:

- `UserPoolId`: `str` *(required)*
- `GroupName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListUsersInGroupPaginator.paginate` returns
`AsyncIterable`\[[ListUsersInGroupResponseTypeDef](./type_defs.md#listusersingroupresponsetypedef)\].
