# Examples

> [Index](../README.md) > [SignInService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SignInService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signin.html#signinservice)
    type annotations stubs module [types-aiobotocore-signin](https://pypi.org/project/types-aiobotocore-signin/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[signin]` package installed.

Write your `SignInService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SignInServiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("signin") as client:  # (1)
    result = await client.create_o_auth2_token()  # (2)
```

1. client: [SignInServiceClient](./client.md)
2. result: [:material-code-braces: CreateOAuth2TokenResponseTypeDef](./type_defs.md#createoauth2tokenresponsetypedef)






### Explicit type annotations

With `types-aiobotocore-lite[signin]`
or a standalone `types_aiobotocore_signin` package, you have to explicitly specify
`client: SignInServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SignInServiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_signin.client import SignInServiceClient
from types_aiobotocore_signin.type_defs import CreateOAuth2TokenResponseTypeDef
from types_aiobotocore_signin.type_defs import CreateOAuth2TokenRequestTypeDef


session = get_session()

async with session.create_client("signin") as client:
    client: SignInServiceClient
    kwargs: CreateOAuth2TokenRequestTypeDef = {...}
    result: CreateOAuth2TokenResponseTypeDef = await client.create_o_auth2_token(**kwargs)
```




