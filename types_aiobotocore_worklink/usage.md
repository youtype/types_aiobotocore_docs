<a id="examples-for-aiobotocore-worklink-module"></a>

# Examples for aiobotocore WorkLink module

> [Index](../README.md) > [WorkLink](./README.md) > Examples

- [Examples for aiobotocore WorkLink module](#examples-for-aiobotocore-worklink-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[worklink]` package installed.

Write your `WorkLink` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type WorkLinkClient
# and provides type checking and code completion
async with session.create_client("worklink") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_domain()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[worklink]` or a standalone
`types_aiobotocore_worklink` package, you have to explicitly specify
`client: WorkLinkClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_worklink.client import WorkLinkClient
from types_aiobotocore_worklink.type_defs import Dict[str, Any]






session = get_session()

async with session.create_client("worklink") as client:
    client: WorkLinkClient

    
    result: Dict[str, Any] = client.associate_domain()
    

    

    
```
