# Examples

> [Index](../README.md) > [SSO](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SSO](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#sso)
    type annotations stubs module [types-aiobotocore-sso](https://pypi.org/project/types-aiobotocore-sso/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[sso]` package installed.

Write your `SSO` code as usual,
type checking and code completion should work out of the box.



```python
# SSOClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("sso") as client:  # (1)
    result = await client.get_role_credentials()  # (2)
```

1. client: [SSOClient](./client.md)
2. result: [:material-code-braces: GetRoleCredentialsResponseTypeDef](./type_defs.md#getrolecredentialsresponsetypedef) 



```python
# ListAccountRolesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("sso") as client:  # (1)
    paginator = client.get_paginator("list_account_roles")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SSOClient](./client.md)
2. paginator: [ListAccountRolesPaginator](./paginators.md#listaccountrolespaginator)
3. item: [:material-code-braces: ListAccountRolesResponseTypeDef](./type_defs.md#listaccountrolesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[sso]`
or a standalone `types_aiobotocore_sso` package, you have to explicitly specify
`client: SSOClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SSOClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_sso.client import SSOClient
from types_aiobotocore_sso.type_defs import GetRoleCredentialsResponseTypeDef
from types_aiobotocore_sso.type_defs import GetRoleCredentialsRequestTypeDef


session = get_session()

async with session.create_client("sso") as client:
    client: SSOClient
    kwargs: GetRoleCredentialsRequestTypeDef = {...}
    result: GetRoleCredentialsResponseTypeDef = await client.get_role_credentials(**kwargs)
```



```python
# ListAccountRolesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_sso.client import SSOClient
from types_aiobotocore_sso.paginator import ListAccountRolesPaginator
from types_aiobotocore_sso.type_defs import ListAccountRolesResponseTypeDef


session = get_session()

async with session.create_client("sso") as client:
    client: SSOClient
    paginator: ListAccountRolesPaginator = client.get_paginator("list_account_roles")
    async for item in paginator.paginate(...):
        item: ListAccountRolesResponseTypeDef
        print(item)
```


