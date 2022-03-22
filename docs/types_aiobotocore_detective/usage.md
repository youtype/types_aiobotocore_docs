<a id="examples-for-aiobotocore-detective-module"></a>

# Examples for aiobotocore Detective module

> [Index](../README.md) > [Detective](./README.md) > Examples

- [Examples for aiobotocore Detective module](#examples-for-aiobotocore-detective-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[detective]` package installed.

Write your `Detective` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type DetectiveClient
# and provides type checking and code completion
async with session.create_client("detective") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.accept_invitation()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[detective]` or a standalone
`types_aiobotocore_detective` package, you have to explicitly specify
`client: DetectiveClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_detective.client import DetectiveClient
from types_aiobotocore_detective.type_defs import None






session = get_session()

async with session.create_client("detective") as client:
    client: DetectiveClient

    
    result: None = client.accept_invitation()
    

    

    
```
