# Waiters

> [Index](../README.md) > [Neptune](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [Neptune](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
    type annotations stubs module [types-aiobotocore-neptune](https://pypi.org/project/types-aiobotocore-neptune/).

## DBInstanceAvailableWaiter

Type annotations and code completion for `#!python session.create_client("neptune").get_waiter("db_instance_available")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Waiter.DBInstanceAvailable)

```python title="Usage example"
from aiobotocore.session import Session

from types_aiobotocore_neptune.waiter import DBInstanceAvailableWaiter

session = get_session()
async with session.create_client("neptune") as client:  # (1)
    waiter: DBInstanceAvailableWaiter = client.get_waiter("db_instance_available")  # (2)
    await waiter.wait()
```

1. client: [NeptuneClient](./client.md)
2. waiter: [DBInstanceAvailableWaiter](./waiters.md#dbinstanceavailablewaiter)


### wait

Type annotations and code completion for `#!python DBInstanceAvailableWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    DBInstanceIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef = {  # (1)
    "DBInstanceIdentifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef](./type_defs.md#describedbinstancesmessagedbinstanceavailablewaittypedef) 
## DBInstanceDeletedWaiter

Type annotations and code completion for `#!python session.create_client("neptune").get_waiter("db_instance_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Waiter.DBInstanceDeleted)

```python title="Usage example"
from aiobotocore.session import Session

from types_aiobotocore_neptune.waiter import DBInstanceDeletedWaiter

session = get_session()
async with session.create_client("neptune") as client:  # (1)
    waiter: DBInstanceDeletedWaiter = client.get_waiter("db_instance_deleted")  # (2)
    await waiter.wait()
```

1. client: [NeptuneClient](./client.md)
2. waiter: [DBInstanceDeletedWaiter](./waiters.md#dbinstancedeletedwaiter)


### wait

Type annotations and code completion for `#!python DBInstanceDeletedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    DBInstanceIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef = {  # (1)
    "DBInstanceIdentifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef](./type_defs.md#describedbinstancesmessagedbinstancedeletedwaittypedef) 
