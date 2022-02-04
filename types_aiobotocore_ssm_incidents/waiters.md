<a id="waiters-for-aiobotocore-ssmincidents-module"></a>

# Waiters for aiobotocore SSMIncidents module

> [Index](..) > [SSMIncidents](.) > Waiters

Auto-generated documentation for
[SSMIncidents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
type annotations stubs module
[types-aiobotocore-ssm-incidents](https://pypi.org/project/types-aiobotocore-ssm-incidents/).

- [Waiters for aiobotocore SSMIncidents module](#waiters-for-aiobotocore-ssmincidents-module)
  - [WaitForReplicationSetActiveWaiter](#waitforreplicationsetactivewaiter)
  - [WaitForReplicationSetDeletedWaiter](#waitforreplicationsetdeletedwaiter)

<a id="waitforreplicationsetactivewaiter"></a>

## WaitForReplicationSetActiveWaiter

Type annotations for
`aiobotocore.create_client("ssm-incidents").get_waiter("wait_for_replication_set_active")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_ssm_incidents.waiter import WaitForReplicationSetActiveWaiter

def get_wait_for_replication_set_active_waiter() -> WaitForReplicationSetActiveWaiter:
    return Session().create_client("ssm-incidents").get_waiter("wait_for_replication_set_active")
```

Boto3 documentation:
[SSMIncidents.Waiter.wait_for_replication_set_active](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Waiter.WaitForReplicationSetActive)

Arguments for `WaitForReplicationSetActiveWaiter.wait` method:

- `arn`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="waitforreplicationsetdeletedwaiter"></a>

## WaitForReplicationSetDeletedWaiter

Type annotations for
`aiobotocore.create_client("ssm-incidents").get_waiter("wait_for_replication_set_deleted")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_ssm_incidents.waiter import WaitForReplicationSetDeletedWaiter

def get_wait_for_replication_set_deleted_waiter() -> WaitForReplicationSetDeletedWaiter:
    return Session().create_client("ssm-incidents").get_waiter("wait_for_replication_set_deleted")
```

Boto3 documentation:
[SSMIncidents.Waiter.wait_for_replication_set_deleted](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Waiter.WaitForReplicationSetDeleted)

Arguments for `WaitForReplicationSetDeletedWaiter.wait` method:

- `arn`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
