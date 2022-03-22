<a id="examples-for-aiobotocore-cognitoidentity-module"></a>

# Examples for aiobotocore CognitoIdentity module

> [Index](../README.md) > [CognitoIdentity](./README.md) > Examples

- [Examples for aiobotocore CognitoIdentity module](#examples-for-aiobotocore-cognitoidentity-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[cognito-identity]` package installed.

Write your `CognitoIdentity` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CognitoIdentityClient
# and provides type checking and code completion
async with session.create_client("cognito-identity") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListIdentityPoolsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_identity_pools")
    async for item in paginator.paginate(...):
        # item has type ListIdentityPoolsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[cognito-identity]` or a standalone
`types_aiobotocore_cognito_identity` package, you have to explicitly specify
`client: CognitoIdentityClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_cognito_identity.client import CognitoIdentityClient
from types_aiobotocore_cognito_identity.type_defs import bool
from types_aiobotocore_cognito_identity.paginator import ListIdentityPoolsPaginator

from types_aiobotocore_cognito_identity.literals import PaginatorName



session = get_session()

async with session.create_client("cognito-identity") as client:
    client: CognitoIdentityClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_identity_pools"
    paginator: ListIdentityPoolsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListIdentityPoolsResponseTypeDef
        print(item)
    

    
```
