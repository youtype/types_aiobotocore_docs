# Waiters

> [Index](../README.md) > [Mediapackagev2](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [Mediapackagev2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
    type annotations stubs module [types-aiobotocore-mediapackagev2](https://pypi.org/project/types-aiobotocore-mediapackagev2/).

## HarvestJobFinishedWaiter

Type annotations and code completion for `#!python session.create_client("mediapackagev2").get_waiter("harvest_job_finished")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/waiter/HarvestJobFinished.html#Mediapackagev2.Waiter.HarvestJobFinished)

```python
# HarvestJobFinishedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_mediapackagev2.waiter import HarvestJobFinishedWaiter

session = get_session()
async with session.create_client("mediapackagev2") as client:  # (1)
    waiter: HarvestJobFinishedWaiter = client.get_waiter("harvest_job_finished")  # (2)
    await waiter.wait()
```

1. client: [Mediapackagev2Client](./client.md)
2. waiter: [HarvestJobFinishedWaiter](./waiters.md#harvestjobfinishedwaiter)


### wait

Type annotations and code completion for `#!python HarvestJobFinishedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
    HarvestJobName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetHarvestJobRequestWaitTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
    "OriginEndpointName": ...,
    "HarvestJobName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetHarvestJobRequestWaitTypeDef](./type_defs.md#getharvestjobrequestwaittypedef) 
