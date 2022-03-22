<a id="waiters-for-aiobotocore-emr-module"></a>

# Waiters for aiobotocore EMR module

> [Index](../README.md) > [EMR](./README.md) > Waiters

Auto-generated documentation for
[EMR](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
type annotations stubs module
[types-aiobotocore-emr](https://pypi.org/project/types-aiobotocore-emr/).

- [Waiters for aiobotocore EMR module](#waiters-for-aiobotocore-emr-module)
  - [ClusterRunningWaiter](#clusterrunningwaiter)
  - [ClusterTerminatedWaiter](#clusterterminatedwaiter)
  - [StepCompleteWaiter](#stepcompletewaiter)

<a id="clusterrunningwaiter"></a>

## ClusterRunningWaiter

Type annotations for
`session.create_client("emr").get_waiter("cluster_running")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_emr.waiter import ClusterRunningWaiter

def get_cluster_running_waiter() -> ClusterRunningWaiter:
    return Session().client("emr").get_waiter("cluster_running")
```

Boto3 documentation:
[EMR.Waiter.cluster_running](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Waiter.ClusterRunning)

Arguments for `ClusterRunningWaiter.wait` method:

- `ClusterId`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="clusterterminatedwaiter"></a>

## ClusterTerminatedWaiter

Type annotations for
`session.create_client("emr").get_waiter("cluster_terminated")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_emr.waiter import ClusterTerminatedWaiter

def get_cluster_terminated_waiter() -> ClusterTerminatedWaiter:
    return Session().client("emr").get_waiter("cluster_terminated")
```

Boto3 documentation:
[EMR.Waiter.cluster_terminated](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Waiter.ClusterTerminated)

Arguments for `ClusterTerminatedWaiter.wait` method:

- `ClusterId`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="stepcompletewaiter"></a>

## StepCompleteWaiter

Type annotations for
`session.create_client("emr").get_waiter("step_complete")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_emr.waiter import StepCompleteWaiter

def get_step_complete_waiter() -> StepCompleteWaiter:
    return Session().client("emr").get_waiter("step_complete")
```

Boto3 documentation:
[EMR.Waiter.step_complete](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Waiter.StepComplete)

Arguments for `StepCompleteWaiter.wait` method:

- `ClusterId`: `str` *(required)*
- `StepId`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
