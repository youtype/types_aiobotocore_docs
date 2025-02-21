# Examples

> [Index](../README.md) > [MediaLive](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MediaLive](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#medialive)
    type annotations stubs module [types-aiobotocore-medialive](https://pypi.org/project/types-aiobotocore-medialive/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[medialive]` package installed.

Write your `MediaLive` code as usual,
type checking and code completion should work out of the box.



```python
# MediaLiveClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("medialive") as client:  # (1)
    result = await client.batch_delete()  # (2)
```

1. client: [MediaLiveClient](./client.md)
2. result: [:material-code-braces: BatchDeleteResponseTypeDef](./type_defs.md#batchdeleteresponsetypedef) 



```python
# DescribeSchedulePaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("medialive") as client:  # (1)
    paginator = client.get_paginator("describe_schedule")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. paginator: [DescribeSchedulePaginator](./paginators.md#describeschedulepaginator)
3. item: [:material-code-braces: DescribeScheduleResponseTypeDef](./type_defs.md#describescheduleresponsetypedef) 



```python
# ChannelCreatedWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("medialive") as client:  # (1)
    waiter = client.get_waiter("channel_created")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [ChannelCreatedWaiter](./waiters.md#channelcreatedwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[medialive]`
or a standalone `types_aiobotocore_medialive` package, you have to explicitly specify
`client: MediaLiveClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# MediaLiveClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_medialive.client import MediaLiveClient
from types_aiobotocore_medialive.type_defs import BatchDeleteResponseTypeDef
from types_aiobotocore_medialive.type_defs import BatchDeleteRequestTypeDef


session = get_session()

async with session.create_client("medialive") as client:
    client: MediaLiveClient
    kwargs: BatchDeleteRequestTypeDef = {...}
    result: BatchDeleteResponseTypeDef = await client.batch_delete(**kwargs)
```



```python
# DescribeSchedulePaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_medialive.client import MediaLiveClient
from types_aiobotocore_medialive.paginator import DescribeSchedulePaginator
from types_aiobotocore_medialive.type_defs import DescribeScheduleResponseTypeDef


session = get_session()

async with session.create_client("medialive") as client:
    client: MediaLiveClient
    paginator: DescribeSchedulePaginator = client.get_paginator("describe_schedule")
    async for item in paginator.paginate(...):
        item: DescribeScheduleResponseTypeDef
        print(item)
```



```python
# ChannelCreatedWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_medialive.client import MediaLiveClient
from types_aiobotocore_medialive.waiter import ChannelCreatedWaiter


session = get_session()

async with session.create_client("medialive") as client:
    client: MediaLiveClient
    waiter: ChannelCreatedWaiter = client.get_waiter("channel_created")
    await waiter.wait()
```
