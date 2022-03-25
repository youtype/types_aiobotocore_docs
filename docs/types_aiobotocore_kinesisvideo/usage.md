<a id="examples-for-aiobotocore-kinesisvideo-module"></a>

# Examples for aiobotocore KinesisVideo module

> [Index](../README.md) > [KinesisVideo](./README.md) > Examples

- [Examples for aiobotocore KinesisVideo module](#examples-for-aiobotocore-kinesisvideo-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[kinesisvideo]` package installed.

Write your `KinesisVideo` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type KinesisVideoClient
# and provides type checking and code completion
async with session.create_client("kinesisvideo") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListSignalingChannelsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_signaling_channels")
    async for item in paginator.paginate(...):
        # item has type ListSignalingChannelsOutputTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[kinesisvideo]` or a standalone
`types_aiobotocore_kinesisvideo` package, you have to explicitly specify
`client: KinesisVideoClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_kinesisvideo.client import KinesisVideoClient
from types_aiobotocore_kinesisvideo.type_defs import bool
from types_aiobotocore_kinesisvideo.paginator import ListSignalingChannelsPaginator

from types_aiobotocore_kinesisvideo.literals import PaginatorName



session = get_session()

async with session.create_client("kinesisvideo") as client:
    client: KinesisVideoClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_signaling_channels"
    paginator: ListSignalingChannelsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListSignalingChannelsOutputTypeDef
        print(item)
    

    
```