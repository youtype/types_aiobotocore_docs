<a id="waiters-for-aiobotocore-docdb-module"></a>

# Waiters for aiobotocore DocDB module

> [Index](../README.md) > [DocDB](./README.md) > Waiters

Auto-generated documentation for
[DocDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
type annotations stubs module
[types-aiobotocore-docdb](https://pypi.org/project/types-aiobotocore-docdb/).

- [Waiters for aiobotocore DocDB module](#waiters-for-aiobotocore-docdb-module)
  - [DBInstanceAvailableWaiter](#dbinstanceavailablewaiter)
  - [DBInstanceDeletedWaiter](#dbinstancedeletedwaiter)

<a id="dbinstanceavailablewaiter"></a>

## DBInstanceAvailableWaiter

Type annotations for
`session.create_client("docdb").get_waiter("db_instance_available")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_docdb.waiter import DBInstanceAvailableWaiter

def get_db_instance_available_waiter() -> DBInstanceAvailableWaiter:
    return Session().client("docdb").get_waiter("db_instance_available")
```

Boto3 documentation:
[DocDB.Waiter.db_instance_available](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Waiter.DBInstanceAvailable)

Arguments for `DBInstanceAvailableWaiter.wait` method:

- `DBInstanceIdentifier`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `MaxRecords`: `int`
- `Marker`: `str`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="dbinstancedeletedwaiter"></a>

## DBInstanceDeletedWaiter

Type annotations for
`session.create_client("docdb").get_waiter("db_instance_deleted")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_docdb.waiter import DBInstanceDeletedWaiter

def get_db_instance_deleted_waiter() -> DBInstanceDeletedWaiter:
    return Session().client("docdb").get_waiter("db_instance_deleted")
```

Boto3 documentation:
[DocDB.Waiter.db_instance_deleted](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Waiter.DBInstanceDeleted)

Arguments for `DBInstanceDeletedWaiter.wait` method:

- `DBInstanceIdentifier`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `MaxRecords`: `int`
- `Marker`: `str`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
