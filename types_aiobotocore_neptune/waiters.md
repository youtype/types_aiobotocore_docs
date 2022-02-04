<a id="waiters-for-aiobotocore-neptune-module"></a>

# Waiters for aiobotocore Neptune module

> [Index](..) > [Neptune](.) > Waiters

Auto-generated documentation for
[Neptune](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
type annotations stubs module
[types-aiobotocore-neptune](https://pypi.org/project/types-aiobotocore-neptune/).

- [Waiters for aiobotocore Neptune module](#waiters-for-aiobotocore-neptune-module)
  - [DBInstanceAvailableWaiter](#dbinstanceavailablewaiter)
  - [DBInstanceDeletedWaiter](#dbinstancedeletedwaiter)

<a id="dbinstanceavailablewaiter"></a>

## DBInstanceAvailableWaiter

Type annotations for
`aiobotocore.create_client("neptune").get_waiter("db_instance_available")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_neptune.waiter import DBInstanceAvailableWaiter

def get_db_instance_available_waiter() -> DBInstanceAvailableWaiter:
    return Session().create_client("neptune").get_waiter("db_instance_available")
```

Boto3 documentation:
[Neptune.Waiter.db_instance_available](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Waiter.DBInstanceAvailable)

Arguments for `DBInstanceAvailableWaiter.wait` method:

- `DBInstanceIdentifier`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `MaxRecords`: `int`
- `Marker`: `str`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="dbinstancedeletedwaiter"></a>

## DBInstanceDeletedWaiter

Type annotations for
`aiobotocore.create_client("neptune").get_waiter("db_instance_deleted")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_neptune.waiter import DBInstanceDeletedWaiter

def get_db_instance_deleted_waiter() -> DBInstanceDeletedWaiter:
    return Session().create_client("neptune").get_waiter("db_instance_deleted")
```

Boto3 documentation:
[Neptune.Waiter.db_instance_deleted](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Waiter.DBInstanceDeleted)

Arguments for `DBInstanceDeletedWaiter.wait` method:

- `DBInstanceIdentifier`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `MaxRecords`: `int`
- `Marker`: `str`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
