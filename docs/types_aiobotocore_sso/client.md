<a id="ssoclient-for-aiobotocore-sso-module"></a>

# SSOClient for aiobotocore SSO module

> [Index](../README.md) > [SSO](./README.md) > SSOClient

Auto-generated documentation for
[SSO](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
type annotations stubs module
[types-aiobotocore-sso](https://pypi.org/project/types-aiobotocore-sso/).

- [SSOClient for aiobotocore SSO module](#ssoclient-for-aiobotocore-sso-module)
  - [SSOClient](#ssoclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_role_credentials](#get_role_credentials)
    - [list_account_roles](#list_account_roles)
    - [list_accounts](#list_accounts)
    - [logout](#logout)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="ssoclient"></a>

## SSOClient

Type annotations for `session.create_client("sso")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_sso.client import SSOClient

session = get_session()
async with session.create_client("sso") as client:
    client: SSOClient
```

Boto3 documentation:
[SSO.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_sso.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.InvalidRequestException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.TooManyRequestsException`
- `Exceptions.UnauthorizedException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

SSOClient exceptions.

Type annotations for `session.create_client("sso").exceptions` method.

Boto3 documentation:
[SSO.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("sso").can_paginate` method.

Boto3 documentation:
[SSO.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("sso").generate_presigned_url`
method.

Boto3 documentation:
[SSO.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_role\_credentials"></a>

### get_role_credentials

Returns the STS short-term credentials for a given role name that is assigned
to the user.

Type annotations for `session.create_client("sso").get_role_credentials`
method.

Boto3 documentation:
[SSO.Client.get_role_credentials](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Client.get_role_credentials)

Asynchronous method. Use `await get_role_credentials(...)` for a synchronous
call.

Arguments mapping described in
[GetRoleCredentialsRequestRequestTypeDef](./type_defs.md#getrolecredentialsrequestrequesttypedef).

Keyword-only arguments:

- `roleName`: `str` *(required)*
- `accountId`: `str` *(required)*
- `accessToken`: `str` *(required)*

Returns a `Coroutine` for
[GetRoleCredentialsResponseTypeDef](./type_defs.md#getrolecredentialsresponsetypedef).

<a id="list\_account\_roles"></a>

### list_account_roles

Lists all roles that are assigned to the user for a given AWS account.

Type annotations for `session.create_client("sso").list_account_roles` method.

Boto3 documentation:
[SSO.Client.list_account_roles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Client.list_account_roles)

Asynchronous method. Use `await list_account_roles(...)` for a synchronous
call.

Arguments mapping described in
[ListAccountRolesRequestRequestTypeDef](./type_defs.md#listaccountrolesrequestrequesttypedef).

Keyword-only arguments:

- `accessToken`: `str` *(required)*
- `accountId`: `str` *(required)*
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListAccountRolesResponseTypeDef](./type_defs.md#listaccountrolesresponsetypedef).

<a id="list\_accounts"></a>

### list_accounts

Lists all AWS accounts assigned to the user.

Type annotations for `session.create_client("sso").list_accounts` method.

Boto3 documentation:
[SSO.Client.list_accounts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Client.list_accounts)

Asynchronous method. Use `await list_accounts(...)` for a synchronous call.

Arguments mapping described in
[ListAccountsRequestRequestTypeDef](./type_defs.md#listaccountsrequestrequesttypedef).

Keyword-only arguments:

- `accessToken`: `str` *(required)*
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListAccountsResponseTypeDef](./type_defs.md#listaccountsresponsetypedef).

<a id="logout"></a>

### logout

Removes the client- and server-side session that is associated with the user.

Type annotations for `session.create_client("sso").logout` method.

Boto3 documentation:
[SSO.Client.logout](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Client.logout)

Asynchronous method. Use `await logout(...)` for a synchronous call.

Arguments mapping described in
[LogoutRequestRequestTypeDef](./type_defs.md#logoutrequestrequesttypedef).

Keyword-only arguments:

- `accessToken`: `str` *(required)*

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("sso").__aenter__` method.

Boto3 documentation:
[SSO.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [SSOClient](#ssoclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("sso").__aexit__` method.

Boto3 documentation:
[SSO.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("sso").get_paginator` method with
overloads.

- `client.get_paginator("list_account_roles")` ->
  [ListAccountRolesPaginator](./paginators.md#listaccountrolespaginator)
- `client.get_paginator("list_accounts")` ->
  [ListAccountsPaginator](./paginators.md#listaccountspaginator)
