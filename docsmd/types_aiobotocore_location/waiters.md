# Waiters

> [Index](../README.md) > [LocationService](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [LocationService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#locationservice)
    type annotations stubs module [types-aiobotocore-location](https://pypi.org/project/types-aiobotocore-location/).

## JobCompletedWaiter

Type annotations and code completion for `#!python session.create_client("location").get_waiter("job_completed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location/waiter/JobCompleted.html#LocationService.Waiter.JobCompleted)

```python
# JobCompletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_location.waiter import JobCompletedWaiter

session = get_session()
async with session.create_client("location") as client:  # (1)
    waiter: JobCompletedWaiter = client.get_waiter("job_completed")  # (2)
    await waiter.wait(...)
```

1. client: [LocationServiceClient](./client.md)
2. waiter: [JobCompletedWaiter](./waiters.md#jobcompletedwaiter)


### wait

Type annotations and code completion for `#!python JobCompletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    JobId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)


```python
# wait method usage example with argument unpacking

kwargs: GetJobRequestWaitTypeDef = {  # (1)
    "JobId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetJobRequestWaitTypeDef](./type_defs.md#getjobrequestwaittypedef)
