<a id="examples-for-aiobotocore-wellarchitected-module"></a>

# Examples for aiobotocore WellArchitected module

> [Index](../README.md) > [WellArchitected](./README.md) > Examples

- [Examples for aiobotocore WellArchitected module](#examples-for-aiobotocore-wellarchitected-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[wellarchitected]` package installed.

Write your `WellArchitected` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type WellArchitectedClient
# and provides type checking and code completion
async with session.create_client("wellarchitected") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_lenses()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[wellarchitected]` or a standalone
`types_aiobotocore_wellarchitected` package, you have to explicitly specify
`client: WellArchitectedClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_wellarchitected.client import WellArchitectedClient
from types_aiobotocore_wellarchitected.type_defs import None






session = get_session()

async with session.create_client("wellarchitected") as client:
    client: WellArchitectedClient

    
    result: None = client.associate_lenses()
    

    

    
```
