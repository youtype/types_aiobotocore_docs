# Examples

> [Index](../README.md) > [ChimeSDKIdentity](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ChimeSDKIdentity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#chimesdkidentity)
    type annotations stubs module [types-aiobotocore-chime-sdk-identity](https://pypi.org/project/types-aiobotocore-chime-sdk-identity/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[chime-sdk-identity]` package installed.

Write your `ChimeSDKIdentity` code as usual,
type checking and code completion should work out of the box.



```python
# ChimeSDKIdentityClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("chime-sdk-identity") as client:  # (1)
    result = await client.create_app_instance()  # (2)
```

1. client: [ChimeSDKIdentityClient](./client.md)
2. result: [:material-code-braces: CreateAppInstanceResponseTypeDef](./type_defs.md#createappinstanceresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[chime-sdk-identity]`
or a standalone `types_aiobotocore_chime_sdk_identity` package, you have to explicitly specify
`client: ChimeSDKIdentityClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ChimeSDKIdentityClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_chime_sdk_identity.client import ChimeSDKIdentityClient
from types_aiobotocore_chime_sdk_identity.type_defs import CreateAppInstanceResponseTypeDef
from types_aiobotocore_chime_sdk_identity.type_defs import CreateAppInstanceRequestTypeDef


session = get_session()

async with session.create_client("chime-sdk-identity") as client:
    client: ChimeSDKIdentityClient
    kwargs: CreateAppInstanceRequestTypeDef = {...}
    result: CreateAppInstanceResponseTypeDef = await client.create_app_instance(**kwargs)
```




