<a id="examples-for-aiobotocore-pinpoint-module"></a>

# Examples for aiobotocore Pinpoint module

> [Index](../README.md) > [Pinpoint](./README.md) > Examples

- [Examples for aiobotocore Pinpoint module](#examples-for-aiobotocore-pinpoint-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[pinpoint]` package installed.

Write your `Pinpoint` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type PinpointClient
# and provides type checking and code completion
async with session.create_client("pinpoint") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[pinpoint]` or a standalone
`types_aiobotocore_pinpoint` package, you have to explicitly specify
`client: PinpointClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_pinpoint.client import PinpointClient
from types_aiobotocore_pinpoint.type_defs import bool






session = get_session()

async with session.create_client("pinpoint") as client:
    client: PinpointClient

    
    result: bool = client.can_paginate()
    

    

    
```
