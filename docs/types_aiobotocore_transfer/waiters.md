<a id="waiters-for-aiobotocore-transfer-module"></a>

# Waiters for aiobotocore Transfer module

> [Index](../README.md) > [Transfer](./README.md) > Waiters

Auto-generated documentation for
[Transfer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
type annotations stubs module
[types-aiobotocore-transfer](https://pypi.org/project/types-aiobotocore-transfer/).

- [Waiters for aiobotocore Transfer module](#waiters-for-aiobotocore-transfer-module)
  - [ServerOfflineWaiter](#serverofflinewaiter)
  - [ServerOnlineWaiter](#serveronlinewaiter)

<a id="serverofflinewaiter"></a>

## ServerOfflineWaiter

Type annotations for
`session.create_client("transfer").get_waiter("server_offline")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_transfer.waiter import ServerOfflineWaiter

def get_server_offline_waiter() -> ServerOfflineWaiter:
    return Session().client("transfer").get_waiter("server_offline")
```

Boto3 documentation:
[Transfer.Waiter.server_offline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Waiter.ServerOffline)

Arguments for `ServerOfflineWaiter.wait` method:

- `ServerId`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="serveronlinewaiter"></a>

## ServerOnlineWaiter

Type annotations for
`session.create_client("transfer").get_waiter("server_online")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_transfer.waiter import ServerOnlineWaiter

def get_server_online_waiter() -> ServerOnlineWaiter:
    return Session().client("transfer").get_waiter("server_online")
```

Boto3 documentation:
[Transfer.Waiter.server_online](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Waiter.ServerOnline)

Arguments for `ServerOnlineWaiter.wait` method:

- `ServerId`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
