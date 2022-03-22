<a id="examples-for-aiobotocore-medialive-module"></a>

# Examples for aiobotocore MediaLive module

> [Index](../README.md) > [MediaLive](./README.md) > Examples

- [Examples for aiobotocore MediaLive module](#examples-for-aiobotocore-medialive-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[medialive]` package installed.

Write your `MediaLive` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type MediaLiveClient
# and provides type checking and code completion
async with session.create_client("medialive") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.accept_input_device_transfer()
    

    
    # paginator has type DescribeSchedulePaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_schedule")
    async for item in paginator.paginate(...):
        # item has type DescribeScheduleResponseTypeDef
        print(item)
    

    
    # waiter has type ChannelCreatedWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("channel_created")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[medialive]` or a standalone
`types_aiobotocore_medialive` package, you have to explicitly specify
`client: MediaLiveClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_medialive.client import MediaLiveClient
from types_aiobotocore_medialive.type_defs import Dict[str, Any]
from types_aiobotocore_medialive.paginator import DescribeSchedulePaginator
from types_aiobotocore_medialive.waiter import ChannelCreatedWaiter
from types_aiobotocore_medialive.literals import PaginatorName
from types_aiobotocore_medialive.literals import WaiterName


session = get_session()

async with session.create_client("medialive") as client:
    client: MediaLiveClient

    
    result: Dict[str, Any] = client.accept_input_device_transfer()
    

    
    paginator_name: PaginatorName = "describe_schedule"
    paginator: DescribeSchedulePaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeScheduleResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "channel_created"
    waiter: ChannelCreatedWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
