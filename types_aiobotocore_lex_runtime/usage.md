<a id="examples-for-aiobotocore-lexruntimeservice-module"></a>

# Examples for aiobotocore LexRuntimeService module

> [Index](../README.md) > [LexRuntimeService](./README.md) > Examples

- [Examples for aiobotocore LexRuntimeService module](#examples-for-aiobotocore-lexruntimeservice-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[lex-runtime]` package installed.

Write your `LexRuntimeService` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type LexRuntimeServiceClient
# and provides type checking and code completion
async with session.create_client("lex-runtime") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[lex-runtime]` or a standalone
`types_aiobotocore_lex_runtime` package, you have to explicitly specify
`client: LexRuntimeServiceClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_lex_runtime.client import LexRuntimeServiceClient
from types_aiobotocore_lex_runtime.type_defs import bool






session = get_session()

async with session.create_client("lex-runtime") as client:
    client: LexRuntimeServiceClient

    
    result: bool = client.can_paginate()
    

    

    
```
