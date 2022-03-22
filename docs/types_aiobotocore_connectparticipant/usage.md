<a id="examples-for-aiobotocore-connectparticipant-module"></a>

# Examples for aiobotocore ConnectParticipant module

> [Index](../README.md) > [ConnectParticipant](./README.md) > Examples

- [Examples for aiobotocore ConnectParticipant module](#examples-for-aiobotocore-connectparticipant-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[connectparticipant]` package installed.

Write your `ConnectParticipant` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ConnectParticipantClient
# and provides type checking and code completion
async with session.create_client("connectparticipant") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[connectparticipant]` or a standalone
`types_aiobotocore_connectparticipant` package, you have to explicitly specify
`client: ConnectParticipantClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_connectparticipant.client import ConnectParticipantClient
from types_aiobotocore_connectparticipant.type_defs import bool






session = get_session()

async with session.create_client("connectparticipant") as client:
    client: ConnectParticipantClient

    
    result: bool = client.can_paginate()
    

    

    
```
