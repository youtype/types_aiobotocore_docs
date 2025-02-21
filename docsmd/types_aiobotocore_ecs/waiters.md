# Waiters

> [Index](../README.md) > [ECS](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [ECS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ecs)
    type annotations stubs module [types-aiobotocore-ecs](https://pypi.org/project/types-aiobotocore-ecs/).

## ServicesInactiveWaiter

Type annotations and code completion for `#!python session.create_client("ecs").get_waiter("services_inactive")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs/waiter/ServicesInactive.html#ECS.Waiter.ServicesInactive)

```python
# ServicesInactiveWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ecs.waiter import ServicesInactiveWaiter

session = get_session()
async with session.create_client("ecs") as client:  # (1)
    waiter: ServicesInactiveWaiter = client.get_waiter("services_inactive")  # (2)
    await waiter.wait()
```

1. client: [ECSClient](./client.md)
2. waiter: [ServicesInactiveWaiter](./waiters.md#servicesinactivewaiter)


### wait

Type annotations and code completion for `#!python ServicesInactiveWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    services: Sequence[str],
    cluster: str = ...,
    include: Sequence[ServiceFieldType] = ...,  # (1)
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-brackets: ServiceFieldType](./literals.md#servicefieldtype) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeServicesRequestWaitExtraTypeDef = {  # (1)
    "services": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeServicesRequestWaitExtraTypeDef](./type_defs.md#describeservicesrequestwaitextratypedef) 
## ServicesStableWaiter

Type annotations and code completion for `#!python session.create_client("ecs").get_waiter("services_stable")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs/waiter/ServicesStable.html#ECS.Waiter.ServicesStable)

```python
# ServicesStableWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ecs.waiter import ServicesStableWaiter

session = get_session()
async with session.create_client("ecs") as client:  # (1)
    waiter: ServicesStableWaiter = client.get_waiter("services_stable")  # (2)
    await waiter.wait()
```

1. client: [ECSClient](./client.md)
2. waiter: [ServicesStableWaiter](./waiters.md#servicesstablewaiter)


### wait

Type annotations and code completion for `#!python ServicesStableWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    services: Sequence[str],
    cluster: str = ...,
    include: Sequence[ServiceFieldType] = ...,  # (1)
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-brackets: ServiceFieldType](./literals.md#servicefieldtype) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeServicesRequestWaitTypeDef = {  # (1)
    "services": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeServicesRequestWaitTypeDef](./type_defs.md#describeservicesrequestwaittypedef) 
## TasksRunningWaiter

Type annotations and code completion for `#!python session.create_client("ecs").get_waiter("tasks_running")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs/waiter/TasksRunning.html#ECS.Waiter.TasksRunning)

```python
# TasksRunningWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ecs.waiter import TasksRunningWaiter

session = get_session()
async with session.create_client("ecs") as client:  # (1)
    waiter: TasksRunningWaiter = client.get_waiter("tasks_running")  # (2)
    await waiter.wait()
```

1. client: [ECSClient](./client.md)
2. waiter: [TasksRunningWaiter](./waiters.md#tasksrunningwaiter)


### wait

Type annotations and code completion for `#!python TasksRunningWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    tasks: Sequence[str],
    cluster: str = ...,
    include: Sequence[TaskFieldType] = ...,  # (1)
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-brackets: TaskFieldType](./literals.md#taskfieldtype) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeTasksRequestWaitTypeDef = {  # (1)
    "tasks": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeTasksRequestWaitTypeDef](./type_defs.md#describetasksrequestwaittypedef) 
## TasksStoppedWaiter

Type annotations and code completion for `#!python session.create_client("ecs").get_waiter("tasks_stopped")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs/waiter/TasksStopped.html#ECS.Waiter.TasksStopped)

```python
# TasksStoppedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ecs.waiter import TasksStoppedWaiter

session = get_session()
async with session.create_client("ecs") as client:  # (1)
    waiter: TasksStoppedWaiter = client.get_waiter("tasks_stopped")  # (2)
    await waiter.wait()
```

1. client: [ECSClient](./client.md)
2. waiter: [TasksStoppedWaiter](./waiters.md#tasksstoppedwaiter)


### wait

Type annotations and code completion for `#!python TasksStoppedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    tasks: Sequence[str],
    cluster: str = ...,
    include: Sequence[TaskFieldType] = ...,  # (1)
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-brackets: TaskFieldType](./literals.md#taskfieldtype) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeTasksRequestWaitExtraTypeDef = {  # (1)
    "tasks": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeTasksRequestWaitExtraTypeDef](./type_defs.md#describetasksrequestwaitextratypedef) 
