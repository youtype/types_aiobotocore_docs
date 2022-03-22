<a id="examples-for-aiobotocore-mediastore-module"></a>

# Examples for aiobotocore MediaStore module

> [Index](../README.md) > [MediaStore](./README.md) > Examples

- [Examples for aiobotocore MediaStore module](#examples-for-aiobotocore-mediastore-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[mediastore]` package installed.

Write your `MediaStore` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type MediaStoreClient
# and provides type checking and code completion
async with session.create_client("mediastore") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListContainersPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_containers")
    async for item in paginator.paginate(...):
        # item has type ListContainersOutputTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[mediastore]` or a standalone
`types_aiobotocore_mediastore` package, you have to explicitly specify
`client: MediaStoreClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediastore.client import MediaStoreClient
from types_aiobotocore_mediastore.type_defs import bool
from types_aiobotocore_mediastore.paginator import ListContainersPaginator

from types_aiobotocore_mediastore.literals import PaginatorName



session = get_session()

async with session.create_client("mediastore") as client:
    client: MediaStoreClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_containers"
    paginator: ListContainersPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListContainersOutputTypeDef
        print(item)
    

    
```
