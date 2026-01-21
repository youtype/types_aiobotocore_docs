# SignInServiceClient

> [Index](../README.md) > [SignInService](./README.md) > SignInServiceClient

!!! note ""

    Auto-generated documentation for [SignInService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signin.html#signinservice)
    type annotations stubs module [types-aiobotocore-signin](https://pypi.org/project/types-aiobotocore-signin/).

## SignInServiceClient

Type annotations and code completion for `#!python session.create_client("signin")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signin.html#SignInService.Client)

```python
# SignInServiceClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_signin.client import SignInServiceClient

session = get_session()
async with session.create_client("signin") as client:
    client: SignInServiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("signin").exceptions` structure.

```python
# SignInServiceClient.exceptions usage example

async with session.create_client("signin") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.InternalServerException,
        client.TooManyRequestsError,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# SignInServiceClient usage type checking example

from types_aiobotocore_signin.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("signin").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signin/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("signin").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signin/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### create\_o\_auth2\_token

CreateOAuth2Token API.

Type annotations and code completion for `#!python session.create_client("signin").create_o_auth2_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signin/client/create_o_auth2_token.html)

```python
# create_o_auth2_token method definition

await def create_o_auth2_token(
    self,
    *,
    tokenInput: CreateOAuth2TokenRequestBodyTypeDef,  # (1)
) -> CreateOAuth2TokenResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CreateOAuth2TokenRequestBodyTypeDef](./type_defs.md#createoauth2tokenrequestbodytypedef)
2. See [:material-code-braces: CreateOAuth2TokenResponseTypeDef](./type_defs.md#createoauth2tokenresponsetypedef)


```python
# create_o_auth2_token method usage example with argument unpacking

kwargs: CreateOAuth2TokenRequestTypeDef = {  # (1)
    "tokenInput": ...,
}

parent.create_o_auth2_token(**kwargs)
```

1. See [:material-code-braces: CreateOAuth2TokenRequestTypeDef](./type_defs.md#createoauth2tokenrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("signin").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signin.html#SignInService.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("signin").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signin.html#SignInService.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```





