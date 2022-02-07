<a id="paginators-for-aiobotocore-chime-module"></a>

# Paginators for aiobotocore Chime module

> [Index](..) > [Chime](.) > Paginators

Auto-generated documentation for
[Chime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
type annotations stubs module
[types-aiobotocore-chime](https://pypi.org/project/types-aiobotocore-chime/).

- [Paginators for aiobotocore Chime module](#paginators-for-aiobotocore-chime-module)
  - [ListAccountsPaginator](#listaccountspaginator)
  - [ListUsersPaginator](#listuserspaginator)

<a id="listaccountspaginator"></a>

## ListAccountsPaginator

Type annotations for
`session.create_client("chime").get_paginator("list_accounts")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_chime.paginator import ListAccountsPaginator

session = get_session()
async with session.create_client("chime") as client:
    client: ChimeClient
    paginator: ListAccountsPaginator = client.get_paginator("list_accounts")
```

Boto3 documentation:
[Chime.Paginator.ListAccounts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Paginator.ListAccounts)

Arguments for `ListAccountsPaginator.paginate` method:

- `Name`: `str`
- `UserEmail`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAccountsPaginator.paginate` returns
`_PageIterator`\[[ListAccountsResponseTypeDef](./type_defs.md#listaccountsresponsetypedef)\].

<a id="listuserspaginator"></a>

## ListUsersPaginator

Type annotations for
`session.create_client("chime").get_paginator("list_users")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_chime.paginator import ListUsersPaginator

session = get_session()
async with session.create_client("chime") as client:
    client: ChimeClient
    paginator: ListUsersPaginator = client.get_paginator("list_users")
```

Boto3 documentation:
[Chime.Paginator.ListUsers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Paginator.ListUsers)

Arguments for `ListUsersPaginator.paginate` method:

- `AccountId`: `str` *(required)*
- `UserEmail`: `str`
- `UserType`: [UserTypeType](./literals.md#usertypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListUsersPaginator.paginate` returns
`_PageIterator`\[[ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef)\].
