<a id="examples-for-aiobotocore-lookoutforvision-module"></a>

# Examples for aiobotocore LookoutforVision module

> [Index](../README.md) > [LookoutforVision](./README.md) > Examples

- [Examples for aiobotocore LookoutforVision module](#examples-for-aiobotocore-lookoutforvision-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[lookoutvision]` package installed.

Write your `LookoutforVision` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type LookoutforVisionClient
# and provides type checking and code completion
async with session.create_client("lookoutvision") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListDatasetEntriesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_dataset_entries")
    async for item in paginator.paginate(...):
        # item has type ListDatasetEntriesResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[lookoutvision]` or a standalone
`types_aiobotocore_lookoutvision` package, you have to explicitly specify
`client: LookoutforVisionClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_lookoutvision.client import LookoutforVisionClient
from types_aiobotocore_lookoutvision.type_defs import bool
from types_aiobotocore_lookoutvision.paginator import ListDatasetEntriesPaginator

from types_aiobotocore_lookoutvision.literals import PaginatorName



session = get_session()

async with session.create_client("lookoutvision") as client:
    client: LookoutforVisionClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_dataset_entries"
    paginator: ListDatasetEntriesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListDatasetEntriesResponseTypeDef
        print(item)
    

    
```
