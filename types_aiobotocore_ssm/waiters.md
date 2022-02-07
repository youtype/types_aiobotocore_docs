<a id="waiters-for-aiobotocore-ssm-module"></a>

# Waiters for aiobotocore SSM module

> [Index](..) > [SSM](.) > Waiters

Auto-generated documentation for
[SSM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
type annotations stubs module
[types-aiobotocore-ssm](https://pypi.org/project/types-aiobotocore-ssm/).

- [Waiters for aiobotocore SSM module](#waiters-for-aiobotocore-ssm-module)
  - [CommandExecutedWaiter](#commandexecutedwaiter)

<a id="commandexecutedwaiter"></a>

## CommandExecutedWaiter

Type annotations for
`session.create_client("ssm").get_waiter("command_executed")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_ssm.waiter import CommandExecutedWaiter

def get_command_executed_waiter() -> CommandExecutedWaiter:
    return Session().client("ssm").get_waiter("command_executed")
```

Boto3 documentation:
[SSM.Waiter.command_executed](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Waiter.CommandExecuted)

Arguments for `CommandExecutedWaiter.wait` method:

- `CommandId`: `str` *(required)*
- `InstanceId`: `str` *(required)*
- `PluginName`: `str`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
