# Examples

> [Index](../README.md) > [GameLiftStreams](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [GameLiftStreams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams.html#gameliftstreams)
    type annotations stubs module [types-aiobotocore-gameliftstreams](https://pypi.org/project/types-aiobotocore-gameliftstreams/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[gameliftstreams]` package installed.

Write your `GameLiftStreams` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# GameLiftStreamsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("gameliftstreams") as client:  # (1)
    result = await client.add_stream_group_locations()  # (2)
```

1. client: [GameLiftStreamsClient](./client.md)
2. result: [:material-code-braces: AddStreamGroupLocationsOutputTypeDef](./type_defs.md#addstreamgrouplocationsoutputtypedef)



#### Paginator usage example

```python
# ListApplicationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("gameliftstreams") as client:  # (1)
    paginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [GameLiftStreamsClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ListApplicationsOutputTypeDef](./type_defs.md#listapplicationsoutputtypedef)



#### Waiter usage example

```python
# ApplicationDeletedWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("gameliftstreams") as client:  # (1)
    waiter = client.get_waiter("application_deleted")  # (2)
    await waiter.wait(...)
```

1. client: [GameLiftStreamsClient](./client.md)
2. waiter: [ApplicationDeletedWaiter](./waiters.md#applicationdeletedwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[gameliftstreams]`
or a standalone `types_aiobotocore_gameliftstreams` package, you have to explicitly specify
`client: GameLiftStreamsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# GameLiftStreamsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_gameliftstreams.client import GameLiftStreamsClient
from types_aiobotocore_gameliftstreams.type_defs import AddStreamGroupLocationsOutputTypeDef
from types_aiobotocore_gameliftstreams.type_defs import AddStreamGroupLocationsInputTypeDef


session = get_session()

async with session.create_client("gameliftstreams") as client:
    client: GameLiftStreamsClient
    kwargs: AddStreamGroupLocationsInputTypeDef = {...}
    result: AddStreamGroupLocationsOutputTypeDef = await client.add_stream_group_locations(**kwargs)
```



#### Paginator usage example

```python
# ListApplicationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_gameliftstreams.client import GameLiftStreamsClient
from types_aiobotocore_gameliftstreams.paginator import ListApplicationsPaginator
from types_aiobotocore_gameliftstreams.type_defs import ListApplicationsOutputTypeDef


session = get_session()

async with session.create_client("gameliftstreams") as client:
    client: GameLiftStreamsClient
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
    async for item in paginator.paginate(...):
        item: ListApplicationsOutputTypeDef
        print(item)
```



#### Waiter usage example

```python
# ApplicationDeletedWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_gameliftstreams.client import GameLiftStreamsClient
from types_aiobotocore_gameliftstreams.waiter import ApplicationDeletedWaiter


session = get_session()

async with session.create_client("gameliftstreams") as client:
    client: GameLiftStreamsClient
    waiter: ApplicationDeletedWaiter = client.get_waiter("application_deleted")
    await waiter.wait(...)
```
