<a id="examples-for-aiobotocore-lexruntimev2-module"></a>

# Examples for aiobotocore LexRuntimeV2 module

> [Index](../README.md) > [LexRuntimeV2](./README.md) > Examples

- [Examples for aiobotocore LexRuntimeV2 module](#examples-for-aiobotocore-lexruntimev2-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[lexv2-runtime]` package installed.

Write your `LexRuntimeV2` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type LexRuntimeV2Client
# and provides type checking and code completion
async with session.create_client("lexv2-runtime") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[lexv2-runtime]` or a standalone
`types_aiobotocore_lexv2_runtime` package, you have to explicitly specify
`client: LexRuntimeV2Client` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_lexv2_runtime.client import LexRuntimeV2Client
from types_aiobotocore_lexv2_runtime.type_defs import bool






session = get_session()

async with session.create_client("lexv2-runtime") as client:
    client: LexRuntimeV2Client

    
    result: bool = client.can_paginate()
    

    

    
```
