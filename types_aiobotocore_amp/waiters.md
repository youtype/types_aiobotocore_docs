<a id="waiters-for-aiobotocore-prometheusservice-module"></a>

# Waiters for aiobotocore PrometheusService module

> [Index](..) > [PrometheusService](.) > Waiters

Auto-generated documentation for
[PrometheusService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
type annotations stubs module
[types-aiobotocore-amp](https://pypi.org/project/types-aiobotocore-amp/).

- [Waiters for aiobotocore PrometheusService module](#waiters-for-aiobotocore-prometheusservice-module)
  - [WorkspaceActiveWaiter](#workspaceactivewaiter)
  - [WorkspaceDeletedWaiter](#workspacedeletedwaiter)

<a id="workspaceactivewaiter"></a>

## WorkspaceActiveWaiter

Type annotations for
`session.create_client("amp").get_waiter("workspace_active")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_amp.waiter import WorkspaceActiveWaiter

def get_workspace_active_waiter() -> WorkspaceActiveWaiter:
    return Session().client("amp").get_waiter("workspace_active")
```

Boto3 documentation:
[PrometheusService.Waiter.workspace_active](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Waiter.WorkspaceActive)

Arguments for `WorkspaceActiveWaiter.wait` method:

- `workspaceId`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="workspacedeletedwaiter"></a>

## WorkspaceDeletedWaiter

Type annotations for
`session.create_client("amp").get_waiter("workspace_deleted")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_amp.waiter import WorkspaceDeletedWaiter

def get_workspace_deleted_waiter() -> WorkspaceDeletedWaiter:
    return Session().client("amp").get_waiter("workspace_deleted")
```

Boto3 documentation:
[PrometheusService.Waiter.workspace_deleted](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Waiter.WorkspaceDeleted)

Arguments for `WorkspaceDeletedWaiter.wait` method:

- `workspaceId`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
