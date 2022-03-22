<a id="examples-for-aiobotocore-personalize-module"></a>

# Examples for aiobotocore Personalize module

> [Index](../README.md) > [Personalize](./README.md) > Examples

- [Examples for aiobotocore Personalize module](#examples-for-aiobotocore-personalize-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[personalize]` package installed.

Write your `Personalize` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type PersonalizeClient
# and provides type checking and code completion
async with session.create_client("personalize") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListBatchInferenceJobsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_batch_inference_jobs")
    async for item in paginator.paginate(...):
        # item has type ListBatchInferenceJobsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[personalize]` or a standalone
`types_aiobotocore_personalize` package, you have to explicitly specify
`client: PersonalizeClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_personalize.client import PersonalizeClient
from types_aiobotocore_personalize.type_defs import bool
from types_aiobotocore_personalize.paginator import ListBatchInferenceJobsPaginator

from types_aiobotocore_personalize.literals import PaginatorName



session = get_session()

async with session.create_client("personalize") as client:
    client: PersonalizeClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_batch_inference_jobs"
    paginator: ListBatchInferenceJobsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListBatchInferenceJobsResponseTypeDef
        print(item)
    

    
```
