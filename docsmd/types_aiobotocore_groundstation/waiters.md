# Waiters

> [Index](../README.md) > [GroundStation](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [GroundStation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#groundstation)
    type annotations stubs module [types-aiobotocore-groundstation](https://pypi.org/project/types-aiobotocore-groundstation/).

## ContactScheduledWaiter

Type annotations and code completion for `#!python session.create_client("groundstation").get_waiter("contact_scheduled")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation/waiter/ContactScheduled.html#GroundStation.Waiter.ContactScheduled)

```python
# ContactScheduledWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_groundstation.waiter import ContactScheduledWaiter

session = get_session()
async with session.create_client("groundstation") as client:  # (1)
    waiter: ContactScheduledWaiter = client.get_waiter("contact_scheduled")  # (2)
    await waiter.wait()
```

1. client: [GroundStationClient](./client.md)
2. waiter: [ContactScheduledWaiter](./waiters.md#contactscheduledwaiter)


### wait

Type annotations and code completion for `#!python ContactScheduledWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    contactId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeContactRequestWaitTypeDef = {  # (1)
    "contactId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeContactRequestWaitTypeDef](./type_defs.md#describecontactrequestwaittypedef) 
