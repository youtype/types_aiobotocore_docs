# Waiters

> [Index](../README.md) > [DatabaseMigrationService](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [DatabaseMigrationService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#databasemigrationservice)
    type annotations stubs module [types-aiobotocore-dms](https://pypi.org/project/types-aiobotocore-dms/).

## EndpointDeletedWaiter

Type annotations and code completion for `#!python session.create_client("dms").get_waiter("endpoint_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/waiter/EndpointDeleted.html#DatabaseMigrationService.Waiter.EndpointDeleted)

```python
# EndpointDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_dms.waiter import EndpointDeletedWaiter

session = get_session()
async with session.create_client("dms") as client:  # (1)
    waiter: EndpointDeletedWaiter = client.get_waiter("endpoint_deleted")  # (2)
    await waiter.wait()
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. waiter: [EndpointDeletedWaiter](./waiters.md#endpointdeletedwaiter)


### wait

Type annotations and code completion for `#!python EndpointDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeEndpointsMessageWaitTypeDef = {  # (1)
    "Filters": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeEndpointsMessageWaitTypeDef](./type_defs.md#describeendpointsmessagewaittypedef) 
## ReplicationInstanceAvailableWaiter

Type annotations and code completion for `#!python session.create_client("dms").get_waiter("replication_instance_available")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/waiter/ReplicationInstanceAvailable.html#DatabaseMigrationService.Waiter.ReplicationInstanceAvailable)

```python
# ReplicationInstanceAvailableWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_dms.waiter import ReplicationInstanceAvailableWaiter

session = get_session()
async with session.create_client("dms") as client:  # (1)
    waiter: ReplicationInstanceAvailableWaiter = client.get_waiter("replication_instance_available")  # (2)
    await waiter.wait()
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. waiter: [ReplicationInstanceAvailableWaiter](./waiters.md#replicationinstanceavailablewaiter)


### wait

Type annotations and code completion for `#!python ReplicationInstanceAvailableWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeReplicationInstancesMessageWaitTypeDef = {  # (1)
    "Filters": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationInstancesMessageWaitTypeDef](./type_defs.md#describereplicationinstancesmessagewaittypedef) 
## ReplicationInstanceDeletedWaiter

Type annotations and code completion for `#!python session.create_client("dms").get_waiter("replication_instance_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/waiter/ReplicationInstanceDeleted.html#DatabaseMigrationService.Waiter.ReplicationInstanceDeleted)

```python
# ReplicationInstanceDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_dms.waiter import ReplicationInstanceDeletedWaiter

session = get_session()
async with session.create_client("dms") as client:  # (1)
    waiter: ReplicationInstanceDeletedWaiter = client.get_waiter("replication_instance_deleted")  # (2)
    await waiter.wait()
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. waiter: [ReplicationInstanceDeletedWaiter](./waiters.md#replicationinstancedeletedwaiter)


### wait

Type annotations and code completion for `#!python ReplicationInstanceDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeReplicationInstancesMessageWaitExtraTypeDef = {  # (1)
    "Filters": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationInstancesMessageWaitExtraTypeDef](./type_defs.md#describereplicationinstancesmessagewaitextratypedef) 
## ReplicationTaskDeletedWaiter

Type annotations and code completion for `#!python session.create_client("dms").get_waiter("replication_task_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/waiter/ReplicationTaskDeleted.html#DatabaseMigrationService.Waiter.ReplicationTaskDeleted)

```python
# ReplicationTaskDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_dms.waiter import ReplicationTaskDeletedWaiter

session = get_session()
async with session.create_client("dms") as client:  # (1)
    waiter: ReplicationTaskDeletedWaiter = client.get_waiter("replication_task_deleted")  # (2)
    await waiter.wait()
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. waiter: [ReplicationTaskDeletedWaiter](./waiters.md#replicationtaskdeletedwaiter)


### wait

Type annotations and code completion for `#!python ReplicationTaskDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
    WithoutSettings: bool = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeReplicationTasksMessageWaitExtraExtraExtraTypeDef = {  # (1)
    "Filters": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationTasksMessageWaitExtraExtraExtraTypeDef](./type_defs.md#describereplicationtasksmessagewaitextraextraextratypedef) 
## ReplicationTaskReadyWaiter

Type annotations and code completion for `#!python session.create_client("dms").get_waiter("replication_task_ready")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/waiter/ReplicationTaskReady.html#DatabaseMigrationService.Waiter.ReplicationTaskReady)

```python
# ReplicationTaskReadyWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_dms.waiter import ReplicationTaskReadyWaiter

session = get_session()
async with session.create_client("dms") as client:  # (1)
    waiter: ReplicationTaskReadyWaiter = client.get_waiter("replication_task_ready")  # (2)
    await waiter.wait()
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. waiter: [ReplicationTaskReadyWaiter](./waiters.md#replicationtaskreadywaiter)


### wait

Type annotations and code completion for `#!python ReplicationTaskReadyWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
    WithoutSettings: bool = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeReplicationTasksMessageWaitTypeDef = {  # (1)
    "Filters": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationTasksMessageWaitTypeDef](./type_defs.md#describereplicationtasksmessagewaittypedef) 
## ReplicationTaskRunningWaiter

Type annotations and code completion for `#!python session.create_client("dms").get_waiter("replication_task_running")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/waiter/ReplicationTaskRunning.html#DatabaseMigrationService.Waiter.ReplicationTaskRunning)

```python
# ReplicationTaskRunningWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_dms.waiter import ReplicationTaskRunningWaiter

session = get_session()
async with session.create_client("dms") as client:  # (1)
    waiter: ReplicationTaskRunningWaiter = client.get_waiter("replication_task_running")  # (2)
    await waiter.wait()
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. waiter: [ReplicationTaskRunningWaiter](./waiters.md#replicationtaskrunningwaiter)


### wait

Type annotations and code completion for `#!python ReplicationTaskRunningWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
    WithoutSettings: bool = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeReplicationTasksMessageWaitExtraExtraTypeDef = {  # (1)
    "Filters": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationTasksMessageWaitExtraExtraTypeDef](./type_defs.md#describereplicationtasksmessagewaitextraextratypedef) 
## ReplicationTaskStoppedWaiter

Type annotations and code completion for `#!python session.create_client("dms").get_waiter("replication_task_stopped")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/waiter/ReplicationTaskStopped.html#DatabaseMigrationService.Waiter.ReplicationTaskStopped)

```python
# ReplicationTaskStoppedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_dms.waiter import ReplicationTaskStoppedWaiter

session = get_session()
async with session.create_client("dms") as client:  # (1)
    waiter: ReplicationTaskStoppedWaiter = client.get_waiter("replication_task_stopped")  # (2)
    await waiter.wait()
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. waiter: [ReplicationTaskStoppedWaiter](./waiters.md#replicationtaskstoppedwaiter)


### wait

Type annotations and code completion for `#!python ReplicationTaskStoppedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
    WithoutSettings: bool = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeReplicationTasksMessageWaitExtraTypeDef = {  # (1)
    "Filters": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationTasksMessageWaitExtraTypeDef](./type_defs.md#describereplicationtasksmessagewaitextratypedef) 
## TestConnectionSucceedsWaiter

Type annotations and code completion for `#!python session.create_client("dms").get_waiter("test_connection_succeeds")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/waiter/TestConnectionSucceeds.html#DatabaseMigrationService.Waiter.TestConnectionSucceeds)

```python
# TestConnectionSucceedsWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_dms.waiter import TestConnectionSucceedsWaiter

session = get_session()
async with session.create_client("dms") as client:  # (1)
    waiter: TestConnectionSucceedsWaiter = client.get_waiter("test_connection_succeeds")  # (2)
    await waiter.wait()
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. waiter: [TestConnectionSucceedsWaiter](./waiters.md#testconnectionsucceedswaiter)


### wait

Type annotations and code completion for `#!python TestConnectionSucceedsWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeConnectionsMessageWaitTypeDef = {  # (1)
    "Filters": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeConnectionsMessageWaitTypeDef](./type_defs.md#describeconnectionsmessagewaittypedef) 
