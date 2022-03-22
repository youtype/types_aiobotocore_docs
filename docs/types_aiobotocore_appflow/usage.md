<a id="examples-for-aiobotocore-appflow-module"></a>

# Examples for aiobotocore Appflow module

> [Index](../README.md) > [Appflow](./README.md) > Examples

- [Examples for aiobotocore Appflow module](#examples-for-aiobotocore-appflow-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[appflow]` package installed.

Write your `Appflow` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type AppflowClient
# and provides type checking and code completion
async with session.create_client("appflow") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[appflow]` or a standalone
`types_aiobotocore_appflow` package, you have to explicitly specify
`client: AppflowClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_appflow.client import AppflowClient
from types_aiobotocore_appflow.type_defs import bool






session = get_session()

async with session.create_client("appflow") as client:
    client: AppflowClient

    
    result: bool = client.can_paginate()
    

    

    
```
