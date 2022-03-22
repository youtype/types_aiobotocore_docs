<a id="examples-for-aiobotocore-finspacedata-module"></a>

# Examples for aiobotocore FinSpaceData module

> [Index](../README.md) > [FinSpaceData](./README.md) > Examples

- [Examples for aiobotocore FinSpaceData module](#examples-for-aiobotocore-finspacedata-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[finspace-data]` package installed.

Write your `FinSpaceData` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type FinSpaceDataClient
# and provides type checking and code completion
async with session.create_client("finspace-data") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListChangesetsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_changesets")
    async for item in paginator.paginate(...):
        # item has type ListChangesetsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[finspace-data]` or a standalone
`types_aiobotocore_finspace_data` package, you have to explicitly specify
`client: FinSpaceDataClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_finspace_data.client import FinSpaceDataClient
from types_aiobotocore_finspace_data.type_defs import bool
from types_aiobotocore_finspace_data.paginator import ListChangesetsPaginator

from types_aiobotocore_finspace_data.literals import PaginatorName



session = get_session()

async with session.create_client("finspace-data") as client:
    client: FinSpaceDataClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_changesets"
    paginator: ListChangesetsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListChangesetsResponseTypeDef
        print(item)
    

    
```
