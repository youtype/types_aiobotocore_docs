<a id="examples-for-aiobotocore-identitystore-module"></a>

# Examples for aiobotocore IdentityStore module

> [Index](../README.md) > [IdentityStore](./README.md) > Examples

- [Examples for aiobotocore IdentityStore module](#examples-for-aiobotocore-identitystore-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[identitystore]` package installed.

Write your `IdentityStore` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type IdentityStoreClient
# and provides type checking and code completion
async with session.create_client("identitystore") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[identitystore]` or a standalone
`types_aiobotocore_identitystore` package, you have to explicitly specify
`client: IdentityStoreClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_identitystore.client import IdentityStoreClient
from types_aiobotocore_identitystore.type_defs import bool






session = get_session()

async with session.create_client("identitystore") as client:
    client: IdentityStoreClient

    
    result: bool = client.can_paginate()
    

    

    
```
