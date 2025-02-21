# Paginators

> [Index](../README.md) > [SSO](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SSO](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#sso)
    type annotations stubs module [types-aiobotocore-sso](https://pypi.org/project/types-aiobotocore-sso/).

## ListAccountRolesPaginator

Type annotations and code completion for `#!python session.create_client("sso").get_paginator("list_account_roles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso/paginator/ListAccountRoles.html#SSO.Paginator.ListAccountRoles)

```python
# ListAccountRolesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso.paginator import ListAccountRolesPaginator

session = get_session()
async with session.create_client("sso") as client:  # (1)
    paginator: ListAccountRolesPaginator = client.get_paginator("list_account_roles")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccountRolesResponseTypeDef
        print(item)  # (3)
```

1. client: [SSOClient](./client.md)
2. paginator: [ListAccountRolesPaginator](./paginators.md#listaccountrolespaginator)
3. item: [:material-code-braces: ListAccountRolesResponseTypeDef](./type_defs.md#listaccountrolesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAccountRolesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    accessToken: str,
    accountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAccountRolesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAccountRolesResponseTypeDef](./type_defs.md#listaccountrolesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAccountRolesRequestPaginateTypeDef = {  # (1)
    "accessToken": ...,
    "accountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountRolesRequestPaginateTypeDef](./type_defs.md#listaccountrolesrequestpaginatetypedef) 
## ListAccountsPaginator

Type annotations and code completion for `#!python session.create_client("sso").get_paginator("list_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso/paginator/ListAccounts.html#SSO.Paginator.ListAccounts)

```python
# ListAccountsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso.paginator import ListAccountsPaginator

session = get_session()
async with session.create_client("sso") as client:  # (1)
    paginator: ListAccountsPaginator = client.get_paginator("list_accounts")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccountsResponseTypeDef
        print(item)  # (3)
```

1. client: [SSOClient](./client.md)
2. paginator: [ListAccountsPaginator](./paginators.md#listaccountspaginator)
3. item: [:material-code-braces: ListAccountsResponseTypeDef](./type_defs.md#listaccountsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAccountsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    accessToken: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAccountsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAccountsResponseTypeDef](./type_defs.md#listaccountsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAccountsRequestPaginateTypeDef = {  # (1)
    "accessToken": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountsRequestPaginateTypeDef](./type_defs.md#listaccountsrequestpaginatetypedef) 
