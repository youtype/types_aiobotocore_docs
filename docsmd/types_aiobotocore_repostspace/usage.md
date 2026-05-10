# Examples

> [Index](../README.md) > [RePostPrivate](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [RePostPrivate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace.html#repostprivate)
    type annotations stubs module [types-aiobotocore-repostspace](https://pypi.org/project/types-aiobotocore-repostspace/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[repostspace]` package installed.

Write your `RePostPrivate` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# RePostPrivateClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("repostspace") as client:  # (1)
    result = await client.batch_add_channel_role_to_accessors()  # (2)
```

1. client: [RePostPrivateClient](./client.md)
2. result: [:material-code-braces: BatchAddChannelRoleToAccessorsOutputTypeDef](./type_defs.md#batchaddchannelroletoaccessorsoutputtypedef)



#### Paginator usage example

```python
# ListChannelsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("repostspace") as client:  # (1)
    paginator = client.get_paginator("list_channels")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [RePostPrivateClient](./client.md)
2. paginator: [ListChannelsPaginator](./paginators.md#listchannelspaginator)
3. item: [:material-code-braces: ListChannelsOutputTypeDef](./type_defs.md#listchannelsoutputtypedef)



#### Waiter usage example

```python
# ChannelCreatedWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("repostspace") as client:  # (1)
    waiter = client.get_waiter("channel_created")  # (2)
    await waiter.wait(...)
```

1. client: [RePostPrivateClient](./client.md)
2. waiter: [ChannelCreatedWaiter](./waiters.md#channelcreatedwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[repostspace]`
or a standalone `types_aiobotocore_repostspace` package, you have to explicitly specify
`client: RePostPrivateClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# RePostPrivateClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_repostspace.client import RePostPrivateClient
from types_aiobotocore_repostspace.type_defs import BatchAddChannelRoleToAccessorsOutputTypeDef
from types_aiobotocore_repostspace.type_defs import BatchAddChannelRoleToAccessorsInputTypeDef


session = get_session()

async with session.create_client("repostspace") as client:
    client: RePostPrivateClient
    kwargs: BatchAddChannelRoleToAccessorsInputTypeDef = {...}
    result: BatchAddChannelRoleToAccessorsOutputTypeDef = await client.batch_add_channel_role_to_accessors(**kwargs)
```



#### Paginator usage example

```python
# ListChannelsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_repostspace.client import RePostPrivateClient
from types_aiobotocore_repostspace.paginator import ListChannelsPaginator
from types_aiobotocore_repostspace.type_defs import ListChannelsOutputTypeDef


session = get_session()

async with session.create_client("repostspace") as client:
    client: RePostPrivateClient
    paginator: ListChannelsPaginator = client.get_paginator("list_channels")
    async for item in paginator.paginate(...):
        item: ListChannelsOutputTypeDef
        print(item)
```



#### Waiter usage example

```python
# ChannelCreatedWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_repostspace.client import RePostPrivateClient
from types_aiobotocore_repostspace.waiter import ChannelCreatedWaiter


session = get_session()

async with session.create_client("repostspace") as client:
    client: RePostPrivateClient
    waiter: ChannelCreatedWaiter = client.get_waiter("channel_created")
    await waiter.wait(...)
```
