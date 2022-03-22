<a id="examples-for-aiobotocore-computeoptimizer-module"></a>

# Examples for aiobotocore ComputeOptimizer module

> [Index](../README.md) > [ComputeOptimizer](./README.md) > Examples

- [Examples for aiobotocore ComputeOptimizer module](#examples-for-aiobotocore-computeoptimizer-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[compute-optimizer]` package installed.

Write your `ComputeOptimizer` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ComputeOptimizerClient
# and provides type checking and code completion
async with session.create_client("compute-optimizer") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[compute-optimizer]` or a standalone
`types_aiobotocore_compute_optimizer` package, you have to explicitly specify
`client: ComputeOptimizerClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_compute_optimizer.client import ComputeOptimizerClient
from types_aiobotocore_compute_optimizer.type_defs import bool






session = get_session()

async with session.create_client("compute-optimizer") as client:
    client: ComputeOptimizerClient

    
    result: bool = client.can_paginate()
    

    

    
```
