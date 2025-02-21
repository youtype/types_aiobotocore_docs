# Examples

> [Index](../README.md) > [Mediapackagev2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Mediapackagev2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
    type annotations stubs module [types-aiobotocore-mediapackagev2](https://pypi.org/project/types-aiobotocore-mediapackagev2/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[mediapackagev2]` package installed.

Write your `Mediapackagev2` code as usual,
type checking and code completion should work out of the box.



```python
# Mediapackagev2Client usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("mediapackagev2") as client:  # (1)
    result = await client.create_channel()  # (2)
```

1. client: [Mediapackagev2Client](./client.md)
2. result: [:material-code-braces: CreateChannelResponseTypeDef](./type_defs.md#createchannelresponsetypedef) 



```python
# ListChannelGroupsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("mediapackagev2") as client:  # (1)
    paginator = client.get_paginator("list_channel_groups")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [Mediapackagev2Client](./client.md)
2. paginator: [ListChannelGroupsPaginator](./paginators.md#listchannelgroupspaginator)
3. item: [:material-code-braces: ListChannelGroupsResponseTypeDef](./type_defs.md#listchannelgroupsresponsetypedef) 



```python
# HarvestJobFinishedWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("mediapackagev2") as client:  # (1)
    waiter = client.get_waiter("harvest_job_finished")  # (2)
    await waiter.wait()
```

1. client: [Mediapackagev2Client](./client.md)
2. waiter: [HarvestJobFinishedWaiter](./waiters.md#harvestjobfinishedwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[mediapackagev2]`
or a standalone `types_aiobotocore_mediapackagev2` package, you have to explicitly specify
`client: Mediapackagev2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# Mediapackagev2Client usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_mediapackagev2.client import Mediapackagev2Client
from types_aiobotocore_mediapackagev2.type_defs import CreateChannelResponseTypeDef
from types_aiobotocore_mediapackagev2.type_defs import CreateChannelRequestTypeDef


session = get_session()

async with session.create_client("mediapackagev2") as client:
    client: Mediapackagev2Client
    kwargs: CreateChannelRequestTypeDef = {...}
    result: CreateChannelResponseTypeDef = await client.create_channel(**kwargs)
```



```python
# ListChannelGroupsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_mediapackagev2.client import Mediapackagev2Client
from types_aiobotocore_mediapackagev2.paginator import ListChannelGroupsPaginator
from types_aiobotocore_mediapackagev2.type_defs import ListChannelGroupsResponseTypeDef


session = get_session()

async with session.create_client("mediapackagev2") as client:
    client: Mediapackagev2Client
    paginator: ListChannelGroupsPaginator = client.get_paginator("list_channel_groups")
    async for item in paginator.paginate(...):
        item: ListChannelGroupsResponseTypeDef
        print(item)
```



```python
# HarvestJobFinishedWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_mediapackagev2.client import Mediapackagev2Client
from types_aiobotocore_mediapackagev2.waiter import HarvestJobFinishedWaiter


session = get_session()

async with session.create_client("mediapackagev2") as client:
    client: Mediapackagev2Client
    waiter: HarvestJobFinishedWaiter = client.get_waiter("harvest_job_finished")
    await waiter.wait()
```
