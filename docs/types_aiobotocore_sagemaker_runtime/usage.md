<a id="examples-for-aiobotocore-sagemakerruntime-module"></a>

# Examples for aiobotocore SageMakerRuntime module

> [Index](../README.md) > [SageMakerRuntime](./README.md) > Examples

- [Examples for aiobotocore SageMakerRuntime module](#examples-for-aiobotocore-sagemakerruntime-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[sagemaker-runtime]` package installed.

Write your `SageMakerRuntime` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SageMakerRuntimeClient
# and provides type checking and code completion
async with session.create_client("sagemaker-runtime") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[sagemaker-runtime]` or a standalone
`types_aiobotocore_sagemaker_runtime` package, you have to explicitly specify
`client: SageMakerRuntimeClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_sagemaker_runtime.client import SageMakerRuntimeClient
from types_aiobotocore_sagemaker_runtime.type_defs import bool






session = get_session()

async with session.create_client("sagemaker-runtime") as client:
    client: SageMakerRuntimeClient

    
    result: bool = client.can_paginate()
    

    

    
```