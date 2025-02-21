# Examples

> [Index](../README.md) > [SSOOIDC](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SSOOIDC](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#ssooidc)
    type annotations stubs module [types-aiobotocore-sso-oidc](https://pypi.org/project/types-aiobotocore-sso-oidc/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[sso-oidc]` package installed.

Write your `SSOOIDC` code as usual,
type checking and code completion should work out of the box.



```python
# SSOOIDCClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("sso-oidc") as client:  # (1)
    result = await client.create_token()  # (2)
```

1. client: [SSOOIDCClient](./client.md)
2. result: [:material-code-braces: CreateTokenResponseTypeDef](./type_defs.md#createtokenresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[sso-oidc]`
or a standalone `types_aiobotocore_sso_oidc` package, you have to explicitly specify
`client: SSOOIDCClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SSOOIDCClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_sso_oidc.client import SSOOIDCClient
from types_aiobotocore_sso_oidc.type_defs import CreateTokenResponseTypeDef
from types_aiobotocore_sso_oidc.type_defs import CreateTokenRequestTypeDef


session = get_session()

async with session.create_client("sso-oidc") as client:
    client: SSOOIDCClient
    kwargs: CreateTokenRequestTypeDef = {...}
    result: CreateTokenResponseTypeDef = await client.create_token(**kwargs)
```




