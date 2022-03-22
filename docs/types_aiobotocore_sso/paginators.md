<a id="paginators-for-aiobotocore-sso-module"></a>

# Paginators for aiobotocore SSO module

> [Index](../README.md) > [SSO](./README.md) > Paginators

Auto-generated documentation for
[SSO](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
type annotations stubs module
[types-aiobotocore-sso](https://pypi.org/project/types-aiobotocore-sso/).

- [Paginators for aiobotocore SSO module](#paginators-for-aiobotocore-sso-module)
  - [ListAccountRolesPaginator](#listaccountrolespaginator)
  - [ListAccountsPaginator](#listaccountspaginator)

<a id="listaccountrolespaginator"></a>

## ListAccountRolesPaginator

Type annotations for
`session.create_client("sso").get_paginator("list_account_roles")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_sso.paginator import ListAccountRolesPaginator

session = get_session()
async with session.create_client("sso") as client:
    client: SSOClient
    paginator: ListAccountRolesPaginator = client.get_paginator("list_account_roles")
```

Boto3 documentation:
[SSO.Paginator.ListAccountRoles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccountRoles)

Arguments for `ListAccountRolesPaginator.paginate` method:

- `accessToken`: `str` *(required)*
- `accountId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAccountRolesPaginator.paginate` returns
`AsyncIterator`\[[ListAccountRolesResponseTypeDef](./type_defs.md#listaccountrolesresponsetypedef)\].

<a id="listaccountspaginator"></a>

## ListAccountsPaginator

Type annotations for
`session.create_client("sso").get_paginator("list_accounts")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_sso.paginator import ListAccountsPaginator

session = get_session()
async with session.create_client("sso") as client:
    client: SSOClient
    paginator: ListAccountsPaginator = client.get_paginator("list_accounts")
```

Boto3 documentation:
[SSO.Paginator.ListAccounts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccounts)

Arguments for `ListAccountsPaginator.paginate` method:

- `accessToken`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAccountsPaginator.paginate` returns
`AsyncIterator`\[[ListAccountsResponseTypeDef](./type_defs.md#listaccountsresponsetypedef)\].
