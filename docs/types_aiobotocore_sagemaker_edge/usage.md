<a id="examples-for-aiobotocore-sagemakeredgemanager-module"></a>

# Examples for aiobotocore SagemakerEdgeManager module

> [Index](../README.md) > [SagemakerEdgeManager](./README.md) > Examples

- [Examples for aiobotocore SagemakerEdgeManager module](#examples-for-aiobotocore-sagemakeredgemanager-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[sagemaker-edge]` package installed.

Write your `SagemakerEdgeManager` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SagemakerEdgeManagerClient
# and provides type checking and code completion
async with session.create_client("sagemaker-edge") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[sagemaker-edge]` or a standalone
`types_aiobotocore_sagemaker_edge` package, you have to explicitly specify
`client: SagemakerEdgeManagerClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_sagemaker_edge.client import SagemakerEdgeManagerClient
from types_aiobotocore_sagemaker_edge.type_defs import bool






session = get_session()

async with session.create_client("sagemaker-edge") as client:
    client: SagemakerEdgeManagerClient

    
    result: bool = client.can_paginate()
    

    

    
```
