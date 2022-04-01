# Paginators

> [Index](../README.md) > [SSO](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SSO](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
    type annotations stubs module [types-aiobotocore-sso](https://pypi.org/project/types-aiobotocore-sso/).

## ListAccountRolesPaginator

Type annotations and code completion for `#!python session.create_client("sso").get_paginator("list_account_roles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccountRoles)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_sso.paginator import ListAccountRolesPaginator

session = get_session()
async with session.create_client("sso") as client:
    client: SSOClient
    paginator: ListAccountRolesPaginator = client.get_paginator("list_account_roles")
```


### paginate

Type annotations and code completion for `#!python ListAccountRolesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    accessToken: str,
    accountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAccountRolesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAccountRolesResponseTypeDef](./type_defs.md#listaccountrolesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAccountRolesRequestListAccountRolesPaginateTypeDef = {  # (1)
    "accessToken": ...,
    "accountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountRolesRequestListAccountRolesPaginateTypeDef](./type_defs.md#listaccountrolesrequestlistaccountrolespaginatetypedef) 
## ListAccountsPaginator

Type annotations and code completion for `#!python session.create_client("sso").get_paginator("list_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccounts)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_sso.paginator import ListAccountsPaginator

session = get_session()
async with session.create_client("sso") as client:
    client: SSOClient
    paginator: ListAccountsPaginator = client.get_paginator("list_accounts")
```


### paginate

Type annotations and code completion for `#!python ListAccountsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    accessToken: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAccountsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAccountsResponseTypeDef](./type_defs.md#listaccountsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAccountsRequestListAccountsPaginateTypeDef = {  # (1)
    "accessToken": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountsRequestListAccountsPaginateTypeDef](./type_defs.md#listaccountsrequestlistaccountspaginatetypedef) 
