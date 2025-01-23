# Paginators

> [Index](../README.md) > [EventBridgeScheduler](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [EventBridgeScheduler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#eventbridgescheduler)
    type annotations stubs module [types-aiobotocore-scheduler](https://pypi.org/project/types-aiobotocore-scheduler/).

## ListScheduleGroupsPaginator

Type annotations and code completion for `#!python session.create_client("scheduler").get_paginator("list_schedule_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler/paginator/ListScheduleGroups.html#EventBridgeScheduler.Paginator.ListScheduleGroups)

```python
# ListScheduleGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_scheduler.paginator import ListScheduleGroupsPaginator

session = get_session()
async with session.create_client("scheduler") as client:  # (1)
    paginator: ListScheduleGroupsPaginator = client.get_paginator("list_schedule_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListScheduleGroupsOutputTypeDef
        print(item)  # (3)
```

1. client: [EventBridgeSchedulerClient](./client.md)
2. paginator: [ListScheduleGroupsPaginator](./paginators.md#listschedulegroupspaginator)
3. item: [:material-code-braces: ListScheduleGroupsOutputTypeDef](./type_defs.md#listschedulegroupsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListScheduleGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    NamePrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListScheduleGroupsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListScheduleGroupsOutputTypeDef](./type_defs.md#listschedulegroupsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListScheduleGroupsInputPaginateTypeDef = {  # (1)
    "NamePrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListScheduleGroupsInputPaginateTypeDef](./type_defs.md#listschedulegroupsinputpaginatetypedef) 
## ListSchedulesPaginator

Type annotations and code completion for `#!python session.create_client("scheduler").get_paginator("list_schedules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler/paginator/ListSchedules.html#EventBridgeScheduler.Paginator.ListSchedules)

```python
# ListSchedulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_scheduler.paginator import ListSchedulesPaginator

session = get_session()
async with session.create_client("scheduler") as client:  # (1)
    paginator: ListSchedulesPaginator = client.get_paginator("list_schedules")  # (2)
    async for item in paginator.paginate(...):
        item: ListSchedulesOutputTypeDef
        print(item)  # (3)
```

1. client: [EventBridgeSchedulerClient](./client.md)
2. paginator: [ListSchedulesPaginator](./paginators.md#listschedulespaginator)
3. item: [:material-code-braces: ListSchedulesOutputTypeDef](./type_defs.md#listschedulesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSchedulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GroupName: str = ...,
    NamePrefix: str = ...,
    State: ScheduleStateType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListSchedulesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ScheduleStateType](./literals.md#schedulestatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSchedulesOutputTypeDef](./type_defs.md#listschedulesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSchedulesInputPaginateTypeDef = {  # (1)
    "GroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchedulesInputPaginateTypeDef](./type_defs.md#listschedulesinputpaginatetypedef) 
