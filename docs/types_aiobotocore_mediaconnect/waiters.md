<a id="waiters-for-aiobotocore-mediaconnect-module"></a>

# Waiters for aiobotocore MediaConnect module

> [Index](../README.md) > [MediaConnect](./README.md) > Waiters

Auto-generated documentation for
[MediaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
type annotations stubs module
[types-aiobotocore-mediaconnect](https://pypi.org/project/types-aiobotocore-mediaconnect/).

- [Waiters for aiobotocore MediaConnect module](#waiters-for-aiobotocore-mediaconnect-module)
  - [FlowActiveWaiter](#flowactivewaiter)
  - [FlowDeletedWaiter](#flowdeletedwaiter)
  - [FlowStandbyWaiter](#flowstandbywaiter)

<a id="flowactivewaiter"></a>

## FlowActiveWaiter

Type annotations for
`session.create_client("mediaconnect").get_waiter("flow_active")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_mediaconnect.waiter import FlowActiveWaiter

def get_flow_active_waiter() -> FlowActiveWaiter:
    return Session().client("mediaconnect").get_waiter("flow_active")
```

Boto3 documentation:
[MediaConnect.Waiter.flow_active](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Waiter.FlowActive)

Arguments for `FlowActiveWaiter.wait` method:

- `FlowArn`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="flowdeletedwaiter"></a>

## FlowDeletedWaiter

Type annotations for
`session.create_client("mediaconnect").get_waiter("flow_deleted")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_mediaconnect.waiter import FlowDeletedWaiter

def get_flow_deleted_waiter() -> FlowDeletedWaiter:
    return Session().client("mediaconnect").get_waiter("flow_deleted")
```

Boto3 documentation:
[MediaConnect.Waiter.flow_deleted](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Waiter.FlowDeleted)

Arguments for `FlowDeletedWaiter.wait` method:

- `FlowArn`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="flowstandbywaiter"></a>

## FlowStandbyWaiter

Type annotations for
`session.create_client("mediaconnect").get_waiter("flow_standby")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_mediaconnect.waiter import FlowStandbyWaiter

def get_flow_standby_waiter() -> FlowStandbyWaiter:
    return Session().client("mediaconnect").get_waiter("flow_standby")
```

Boto3 documentation:
[MediaConnect.Waiter.flow_standby](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Waiter.FlowStandby)

Arguments for `FlowStandbyWaiter.wait` method:

- `FlowArn`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
