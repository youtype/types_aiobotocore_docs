# Examples

> [Index](../README.md) > [EventBridgeScheduler](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EventBridgeScheduler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#eventbridgescheduler)
    type annotations stubs module [types-aiobotocore-scheduler](https://pypi.org/project/types-aiobotocore-scheduler/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[scheduler]` package installed.

Write your `EventBridgeScheduler` code as usual,
type checking and code completion should work out of the box.



```python
# EventBridgeSchedulerClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("scheduler") as client:  # (1)
    result = await client.create_schedule()  # (2)
```

1. client: [EventBridgeSchedulerClient](./client.md)
2. result: [:material-code-braces: CreateScheduleOutputTypeDef](./type_defs.md#createscheduleoutputtypedef) 



```python
# ListScheduleGroupsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("scheduler") as client:  # (1)
    paginator = client.get_paginator("list_schedule_groups")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [EventBridgeSchedulerClient](./client.md)
2. paginator: [ListScheduleGroupsPaginator](./paginators.md#listschedulegroupspaginator)
3. item: [:material-code-braces: ListScheduleGroupsOutputTypeDef](./type_defs.md#listschedulegroupsoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[scheduler]`
or a standalone `types_aiobotocore_scheduler` package, you have to explicitly specify
`client: EventBridgeSchedulerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# EventBridgeSchedulerClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_scheduler.client import EventBridgeSchedulerClient
from types_aiobotocore_scheduler.type_defs import CreateScheduleOutputTypeDef
from types_aiobotocore_scheduler.type_defs import CreateScheduleInputTypeDef


session = get_session()

async with session.create_client("scheduler") as client:
    client: EventBridgeSchedulerClient
    kwargs: CreateScheduleInputTypeDef = {...}
    result: CreateScheduleOutputTypeDef = await client.create_schedule(**kwargs)
```



```python
# ListScheduleGroupsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_scheduler.client import EventBridgeSchedulerClient
from types_aiobotocore_scheduler.paginator import ListScheduleGroupsPaginator
from types_aiobotocore_scheduler.type_defs import ListScheduleGroupsOutputTypeDef


session = get_session()

async with session.create_client("scheduler") as client:
    client: EventBridgeSchedulerClient
    paginator: ListScheduleGroupsPaginator = client.get_paginator("list_schedule_groups")
    async for item in paginator.paginate(...):
        item: ListScheduleGroupsOutputTypeDef
        print(item)
```


