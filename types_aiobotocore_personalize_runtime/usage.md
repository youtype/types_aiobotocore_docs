<a id="examples-for-aiobotocore-personalizeruntime-module"></a>

# Examples for aiobotocore PersonalizeRuntime module

> [Index](../README.md) > [PersonalizeRuntime](./README.md) > Examples

- [Examples for aiobotocore PersonalizeRuntime module](#examples-for-aiobotocore-personalizeruntime-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[personalize-runtime]` package installed.

Write your `PersonalizeRuntime` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type PersonalizeRuntimeClient
# and provides type checking and code completion
async with session.create_client("personalize-runtime") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[personalize-runtime]` or a standalone
`types_aiobotocore_personalize_runtime` package, you have to explicitly specify
`client: PersonalizeRuntimeClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_personalize_runtime.client import PersonalizeRuntimeClient
from types_aiobotocore_personalize_runtime.type_defs import bool






session = get_session()

async with session.create_client("personalize-runtime") as client:
    client: PersonalizeRuntimeClient

    
    result: bool = client.can_paginate()
    

    

    
```
