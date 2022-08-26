# Waiters

> [Index](../README.md) > [AppStream](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [AppStream](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
    type annotations stubs module [types-aiobotocore-appstream](https://pypi.org/project/types-aiobotocore-appstream/).

## FleetStartedWaiter

Type annotations and code completion for `#!python session.create_client("appstream").get_waiter("fleet_started")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Waiter.FleetStarted)

```python title="Usage example"
from aiobotocore.session import Session

from types_aiobotocore_appstream.waiter import FleetStartedWaiter

session = get_session()
async with session.create_client("appstream") as client:  # (1)
    waiter: FleetStartedWaiter = client.get_waiter("fleet_started")  # (2)
    await waiter.wait()
```

1. client: [AppStreamClient](./client.md)
2. waiter: [FleetStartedWaiter](./waiters.md#fleetstartedwaiter)


### wait

Type annotations and code completion for `#!python FleetStartedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    Names: Sequence[str] = ...,
    NextToken: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeFleetsRequestFleetStartedWaitTypeDef = {  # (1)
    "Names": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeFleetsRequestFleetStartedWaitTypeDef](./type_defs.md#describefleetsrequestfleetstartedwaittypedef) 
## FleetStoppedWaiter

Type annotations and code completion for `#!python session.create_client("appstream").get_waiter("fleet_stopped")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Waiter.FleetStopped)

```python title="Usage example"
from aiobotocore.session import Session

from types_aiobotocore_appstream.waiter import FleetStoppedWaiter

session = get_session()
async with session.create_client("appstream") as client:  # (1)
    waiter: FleetStoppedWaiter = client.get_waiter("fleet_stopped")  # (2)
    await waiter.wait()
```

1. client: [AppStreamClient](./client.md)
2. waiter: [FleetStoppedWaiter](./waiters.md#fleetstoppedwaiter)


### wait

Type annotations and code completion for `#!python FleetStoppedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    Names: Sequence[str] = ...,
    NextToken: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeFleetsRequestFleetStoppedWaitTypeDef = {  # (1)
    "Names": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeFleetsRequestFleetStoppedWaitTypeDef](./type_defs.md#describefleetsrequestfleetstoppedwaittypedef) 
