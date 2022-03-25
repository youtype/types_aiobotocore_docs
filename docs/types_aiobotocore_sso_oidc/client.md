<a id="ssooidcclient-for-aiobotocore-ssooidc-module"></a>

# SSOOIDCClient for aiobotocore SSOOIDC module

> [Index](../README.md) > [SSOOIDC](./README.md) > SSOOIDCClient

Auto-generated documentation for
[SSOOIDC](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
type annotations stubs module
[types-aiobotocore-sso-oidc](https://pypi.org/project/types-aiobotocore-sso-oidc/).

- [SSOOIDCClient for aiobotocore SSOOIDC module](#ssooidcclient-for-aiobotocore-ssooidc-module)
  - [SSOOIDCClient](#ssooidcclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_token](#create_token)
    - [generate_presigned_url](#generate_presigned_url)
    - [register_client](#register_client)
    - [start_device_authorization](#start_device_authorization)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)

<a id="ssooidcclient"></a>

## SSOOIDCClient

Type annotations for `session.create_client("sso-oidc")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_sso_oidc.client import SSOOIDCClient

session = get_session()
async with session.create_client("sso-oidc") as client:
    client: SSOOIDCClient
```

Boto3 documentation:
[SSOOIDC.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_sso_oidc.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.AuthorizationPendingException`
- `Exceptions.ClientError`
- `Exceptions.ExpiredTokenException`
- `Exceptions.InternalServerException`
- `Exceptions.InvalidClientException`
- `Exceptions.InvalidClientMetadataException`
- `Exceptions.InvalidGrantException`
- `Exceptions.InvalidRequestException`
- `Exceptions.InvalidScopeException`
- `Exceptions.SlowDownException`
- `Exceptions.UnauthorizedClientException`
- `Exceptions.UnsupportedGrantTypeException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

SSOOIDCClient exceptions.

Type annotations for `session.create_client("sso-oidc").exceptions` method.

Boto3 documentation:
[SSOOIDC.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("sso-oidc").can_paginate` method.

Boto3 documentation:
[SSOOIDC.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create\_token"></a>

### create_token

Creates and returns an access token for the authorized client.

Type annotations for `session.create_client("sso-oidc").create_token` method.

Boto3 documentation:
[SSOOIDC.Client.create_token](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC.Client.create_token)

Asynchronous method. Use `await create_token(...)` for a synchronous call.

Arguments mapping described in
[CreateTokenRequestRequestTypeDef](./type_defs.md#createtokenrequestrequesttypedef).

Keyword-only arguments:

- `clientId`: `str` *(required)*
- `clientSecret`: `str` *(required)*
- `grantType`: `str` *(required)*
- `deviceCode`: `str` *(required)*
- `code`: `str`
- `refreshToken`: `str`
- `scope`: `Sequence`\[`str`\]
- `redirectUri`: `str`

Returns a `Coroutine` for
[CreateTokenResponseTypeDef](./type_defs.md#createtokenresponsetypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("sso-oidc").generate_presigned_url`
method.

Boto3 documentation:
[SSOOIDC.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="register\_client"></a>

### register_client

Registers a client with AWS SSO.

Type annotations for `session.create_client("sso-oidc").register_client`
method.

Boto3 documentation:
[SSOOIDC.Client.register_client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC.Client.register_client)

Asynchronous method. Use `await register_client(...)` for a synchronous call.

Arguments mapping described in
[RegisterClientRequestRequestTypeDef](./type_defs.md#registerclientrequestrequesttypedef).

Keyword-only arguments:

- `clientName`: `str` *(required)*
- `clientType`: `str` *(required)*
- `scopes`: `Sequence`\[`str`\]

Returns a `Coroutine` for
[RegisterClientResponseTypeDef](./type_defs.md#registerclientresponsetypedef).

<a id="start\_device\_authorization"></a>

### start_device_authorization

Initiates device authorization by requesting a pair of verification codes from
the authorization service.

Type annotations for
`session.create_client("sso-oidc").start_device_authorization` method.

Boto3 documentation:
[SSOOIDC.Client.start_device_authorization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC.Client.start_device_authorization)

Asynchronous method. Use `await start_device_authorization(...)` for a
synchronous call.

Arguments mapping described in
[StartDeviceAuthorizationRequestRequestTypeDef](./type_defs.md#startdeviceauthorizationrequestrequesttypedef).

Keyword-only arguments:

- `clientId`: `str` *(required)*
- `clientSecret`: `str` *(required)*
- `startUrl`: `str` *(required)*

Returns a `Coroutine` for
[StartDeviceAuthorizationResponseTypeDef](./type_defs.md#startdeviceauthorizationresponsetypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("sso-oidc").__aenter__` method.

Boto3 documentation:
[SSOOIDC.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [SSOOIDCClient](#ssooidcclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("sso-oidc").__aexit__` method.

Boto3 documentation:
[SSOOIDC.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.