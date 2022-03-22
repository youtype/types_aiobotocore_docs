<a id="waiters-for-aiobotocore-appstream-module"></a>

# Waiters for aiobotocore AppStream module

> [Index](../README.md) > [AppStream](./README.md) > Waiters

Auto-generated documentation for
[AppStream](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
type annotations stubs module
[types-aiobotocore-appstream](https://pypi.org/project/types-aiobotocore-appstream/).

- [Waiters for aiobotocore AppStream module](#waiters-for-aiobotocore-appstream-module)
  - [FleetStartedWaiter](#fleetstartedwaiter)
  - [FleetStoppedWaiter](#fleetstoppedwaiter)

<a id="fleetstartedwaiter"></a>

## FleetStartedWaiter

Type annotations for
`session.create_client("appstream").get_waiter("fleet_started")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_appstream.waiter import FleetStartedWaiter

def get_fleet_started_waiter() -> FleetStartedWaiter:
    return Session().client("appstream").get_waiter("fleet_started")
```

Boto3 documentation:
[AppStream.Waiter.fleet_started](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Waiter.FleetStarted)

Arguments for `FleetStartedWaiter.wait` method:

- `Names`: `Sequence`\[`str`\]
- `NextToken`: `str`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="fleetstoppedwaiter"></a>

## FleetStoppedWaiter

Type annotations for
`session.create_client("appstream").get_waiter("fleet_stopped")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_appstream.waiter import FleetStoppedWaiter

def get_fleet_stopped_waiter() -> FleetStoppedWaiter:
    return Session().client("appstream").get_waiter("fleet_stopped")
```

Boto3 documentation:
[AppStream.Waiter.fleet_stopped](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Waiter.FleetStopped)

Arguments for `FleetStoppedWaiter.wait` method:

- `Names`: `Sequence`\[`str`\]
- `NextToken`: `str`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
