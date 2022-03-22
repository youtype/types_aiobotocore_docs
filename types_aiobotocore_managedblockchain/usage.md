<a id="examples-for-aiobotocore-managedblockchain-module"></a>

# Examples for aiobotocore ManagedBlockchain module

> [Index](../README.md) > [ManagedBlockchain](./README.md) > Examples

- [Examples for aiobotocore ManagedBlockchain module](#examples-for-aiobotocore-managedblockchain-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[managedblockchain]` package installed.

Write your `ManagedBlockchain` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ManagedBlockchainClient
# and provides type checking and code completion
async with session.create_client("managedblockchain") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[managedblockchain]` or a standalone
`types_aiobotocore_managedblockchain` package, you have to explicitly specify
`client: ManagedBlockchainClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_managedblockchain.client import ManagedBlockchainClient
from types_aiobotocore_managedblockchain.type_defs import bool






session = get_session()

async with session.create_client("managedblockchain") as client:
    client: ManagedBlockchainClient

    
    result: bool = client.can_paginate()
    

    

    
```
