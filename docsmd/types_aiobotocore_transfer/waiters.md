# Waiters

> [Index](../README.md) > [Transfer](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [Transfer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
    type annotations stubs module [types-aiobotocore-transfer](https://pypi.org/project/types-aiobotocore-transfer/).

## ServerOfflineWaiter

Type annotations and code completion for `#!python session.create_client("transfer").get_waiter("server_offline")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Waiter.ServerOffline)

```python title="Usage example"
from aiobotocore.session import Session

from types_aiobotocore_transfer.waiter import ServerOfflineWaiter

def get_server_offline_waiter() -> ServerOfflineWaiter:
    return Session().client("transfer").get_waiter("server_offline")
```


### wait

Type annotations and code completion for `#!python ServerOfflineWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    ServerId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeServerRequestServerOfflineWaitTypeDef = {  # (1)
    "ServerId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeServerRequestServerOfflineWaitTypeDef](./type_defs.md#describeserverrequestserverofflinewaittypedef) 
## ServerOnlineWaiter

Type annotations and code completion for `#!python session.create_client("transfer").get_waiter("server_online")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Waiter.ServerOnline)

```python title="Usage example"
from aiobotocore.session import Session

from types_aiobotocore_transfer.waiter import ServerOnlineWaiter

def get_server_online_waiter() -> ServerOnlineWaiter:
    return Session().client("transfer").get_waiter("server_online")
```


### wait

Type annotations and code completion for `#!python ServerOnlineWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    ServerId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeServerRequestServerOnlineWaitTypeDef = {  # (1)
    "ServerId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeServerRequestServerOnlineWaitTypeDef](./type_defs.md#describeserverrequestserveronlinewaittypedef) 
