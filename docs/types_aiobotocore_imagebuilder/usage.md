<a id="examples-for-aiobotocore-imagebuilder-module"></a>

# Examples for aiobotocore imagebuilder module

> [Index](../README.md) > [imagebuilder](./README.md) > Examples

- [Examples for aiobotocore imagebuilder module](#examples-for-aiobotocore-imagebuilder-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[imagebuilder]` package installed.

Write your `imagebuilder` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type imagebuilderClient
# and provides type checking and code completion
async with session.create_client("imagebuilder") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[imagebuilder]` or a standalone
`types_aiobotocore_imagebuilder` package, you have to explicitly specify
`client: imagebuilderClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_imagebuilder.client import imagebuilderClient
from types_aiobotocore_imagebuilder.type_defs import bool






session = get_session()

async with session.create_client("imagebuilder") as client:
    client: imagebuilderClient

    
    result: bool = client.can_paginate()
    

    

    
```
