<a id="examples-for-aiobotocore-augmentedairuntime-module"></a>

# Examples for aiobotocore AugmentedAIRuntime module

> [Index](../README.md) > [AugmentedAIRuntime](./README.md) > Examples

- [Examples for aiobotocore AugmentedAIRuntime module](#examples-for-aiobotocore-augmentedairuntime-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[sagemaker-a2i-runtime]` package installed.

Write your `AugmentedAIRuntime` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type AugmentedAIRuntimeClient
# and provides type checking and code completion
async with session.create_client("sagemaker-a2i-runtime") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListHumanLoopsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_human_loops")
    async for item in paginator.paginate(...):
        # item has type ListHumanLoopsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[sagemaker-a2i-runtime]` or a standalone
`types_aiobotocore_sagemaker_a2i_runtime` package, you have to explicitly
specify `client: AugmentedAIRuntimeClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_sagemaker_a2i_runtime.client import AugmentedAIRuntimeClient
from types_aiobotocore_sagemaker_a2i_runtime.type_defs import bool
from types_aiobotocore_sagemaker_a2i_runtime.paginator import ListHumanLoopsPaginator

from types_aiobotocore_sagemaker_a2i_runtime.literals import PaginatorName



session = get_session()

async with session.create_client("sagemaker-a2i-runtime") as client:
    client: AugmentedAIRuntimeClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_human_loops"
    paginator: ListHumanLoopsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListHumanLoopsResponseTypeDef
        print(item)
    

    
```
