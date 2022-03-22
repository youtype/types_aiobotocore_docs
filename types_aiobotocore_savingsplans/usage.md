<a id="examples-for-aiobotocore-savingsplans-module"></a>

# Examples for aiobotocore SavingsPlans module

> [Index](../README.md) > [SavingsPlans](./README.md) > Examples

- [Examples for aiobotocore SavingsPlans module](#examples-for-aiobotocore-savingsplans-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[savingsplans]` package installed.

Write your `SavingsPlans` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SavingsPlansClient
# and provides type checking and code completion
async with session.create_client("savingsplans") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[savingsplans]` or a standalone
`types_aiobotocore_savingsplans` package, you have to explicitly specify
`client: SavingsPlansClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_savingsplans.client import SavingsPlansClient
from types_aiobotocore_savingsplans.type_defs import bool






session = get_session()

async with session.create_client("savingsplans") as client:
    client: SavingsPlansClient

    
    result: bool = client.can_paginate()
    

    

    
```
