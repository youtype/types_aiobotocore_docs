<a id="examples-for-aiobotocore-mediatailor-module"></a>

# Examples for aiobotocore MediaTailor module

> [Index](../README.md) > [MediaTailor](./README.md) > Examples

- [Examples for aiobotocore MediaTailor module](#examples-for-aiobotocore-mediatailor-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[mediatailor]` package installed.

Write your `MediaTailor` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type MediaTailorClient
# and provides type checking and code completion
async with session.create_client("mediatailor") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type GetChannelSchedulePaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_channel_schedule")
    async for item in paginator.paginate(...):
        # item has type GetChannelScheduleResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[mediatailor]` or a standalone
`types_aiobotocore_mediatailor` package, you have to explicitly specify
`client: MediaTailorClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediatailor.client import MediaTailorClient
from types_aiobotocore_mediatailor.type_defs import bool
from types_aiobotocore_mediatailor.paginator import GetChannelSchedulePaginator

from types_aiobotocore_mediatailor.literals import PaginatorName



session = get_session()

async with session.create_client("mediatailor") as client:
    client: MediaTailorClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "get_channel_schedule"
    paginator: GetChannelSchedulePaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetChannelScheduleResponseTypeDef
        print(item)
    

    
```
