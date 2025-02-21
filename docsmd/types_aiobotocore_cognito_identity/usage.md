# Examples

> [Index](../README.md) > [CognitoIdentity](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CognitoIdentity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#cognitoidentity)
    type annotations stubs module [types-aiobotocore-cognito-identity](https://pypi.org/project/types-aiobotocore-cognito-identity/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[cognito-identity]` package installed.

Write your `CognitoIdentity` code as usual,
type checking and code completion should work out of the box.



```python
# CognitoIdentityClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cognito-identity") as client:  # (1)
    result = await client.create_identity_pool()  # (2)
```

1. client: [CognitoIdentityClient](./client.md)
2. result: [:material-code-braces: IdentityPoolTypeDef](./type_defs.md#identitypooltypedef) 



```python
# ListIdentityPoolsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cognito-identity") as client:  # (1)
    paginator = client.get_paginator("list_identity_pools")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CognitoIdentityClient](./client.md)
2. paginator: [ListIdentityPoolsPaginator](./paginators.md#listidentitypoolspaginator)
3. item: [:material-code-braces: ListIdentityPoolsResponseTypeDef](./type_defs.md#listidentitypoolsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[cognito-identity]`
or a standalone `types_aiobotocore_cognito_identity` package, you have to explicitly specify
`client: CognitoIdentityClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CognitoIdentityClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cognito_identity.client import CognitoIdentityClient
from types_aiobotocore_cognito_identity.type_defs import IdentityPoolTypeDef
from types_aiobotocore_cognito_identity.type_defs import CreateIdentityPoolInputTypeDef


session = get_session()

async with session.create_client("cognito-identity") as client:
    client: CognitoIdentityClient
    kwargs: CreateIdentityPoolInputTypeDef = {...}
    result: IdentityPoolTypeDef = await client.create_identity_pool(**kwargs)
```



```python
# ListIdentityPoolsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cognito_identity.client import CognitoIdentityClient
from types_aiobotocore_cognito_identity.paginator import ListIdentityPoolsPaginator
from types_aiobotocore_cognito_identity.type_defs import ListIdentityPoolsResponseTypeDef


session = get_session()

async with session.create_client("cognito-identity") as client:
    client: CognitoIdentityClient
    paginator: ListIdentityPoolsPaginator = client.get_paginator("list_identity_pools")
    async for item in paginator.paginate(...):
        item: ListIdentityPoolsResponseTypeDef
        print(item)
```


