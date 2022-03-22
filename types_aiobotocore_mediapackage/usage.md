<a id="examples-for-aiobotocore-mediapackage-module"></a>

# Examples for aiobotocore MediaPackage module

> [Index](../README.md) > [MediaPackage](./README.md) > Examples

- [Examples for aiobotocore MediaPackage module](#examples-for-aiobotocore-mediapackage-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[mediapackage]` package installed.

Write your `MediaPackage` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type MediaPackageClient
# and provides type checking and code completion
async with session.create_client("mediapackage") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListChannelsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_channels")
    async for item in paginator.paginate(...):
        # item has type ListChannelsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[mediapackage]` or a standalone
`types_aiobotocore_mediapackage` package, you have to explicitly specify
`client: MediaPackageClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediapackage.client import MediaPackageClient
from types_aiobotocore_mediapackage.type_defs import bool
from types_aiobotocore_mediapackage.paginator import ListChannelsPaginator

from types_aiobotocore_mediapackage.literals import PaginatorName



session = get_session()

async with session.create_client("mediapackage") as client:
    client: MediaPackageClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_channels"
    paginator: ListChannelsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListChannelsResponseTypeDef
        print(item)
    

    
```
