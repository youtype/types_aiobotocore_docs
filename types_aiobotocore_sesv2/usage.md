<a id="examples-for-aiobotocore-sesv2-module"></a>

# Examples for aiobotocore SESV2 module

> [Index](../README.md) > [SESV2](./README.md) > Examples

- [Examples for aiobotocore SESV2 module](#examples-for-aiobotocore-sesv2-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[sesv2]` package installed.

Write your `SESV2` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SESV2Client
# and provides type checking and code completion
async with session.create_client("sesv2") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[sesv2]` or a standalone `types_aiobotocore_sesv2`
package, you have to explicitly specify `client: SESV2Client` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_sesv2.client import SESV2Client
from types_aiobotocore_sesv2.type_defs import bool






session = get_session()

async with session.create_client("sesv2") as client:
    client: SESV2Client

    
    result: bool = client.can_paginate()
    

    

    
```
