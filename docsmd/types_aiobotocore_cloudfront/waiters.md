# Waiters

> [Index](../README.md) > [CloudFront](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [CloudFront](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#cloudfront)
    type annotations stubs module [types-aiobotocore-cloudfront](https://pypi.org/project/types-aiobotocore-cloudfront/).

## DistributionDeployedWaiter

Type annotations and code completion for `#!python session.create_client("cloudfront").get_waiter("distribution_deployed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront/waiter/DistributionDeployed.html#CloudFront.Waiter.DistributionDeployed)

```python
# DistributionDeployedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_cloudfront.waiter import DistributionDeployedWaiter

session = get_session()
async with session.create_client("cloudfront") as client:  # (1)
    waiter: DistributionDeployedWaiter = client.get_waiter("distribution_deployed")  # (2)
    await waiter.wait()
```

1. client: [CloudFrontClient](./client.md)
2. waiter: [DistributionDeployedWaiter](./waiters.md#distributiondeployedwaiter)


### wait

Type annotations and code completion for `#!python DistributionDeployedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Id: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetDistributionRequestWaitTypeDef = {  # (1)
    "Id": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetDistributionRequestWaitTypeDef](./type_defs.md#getdistributionrequestwaittypedef) 
## InvalidationCompletedWaiter

Type annotations and code completion for `#!python session.create_client("cloudfront").get_waiter("invalidation_completed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront/waiter/InvalidationCompleted.html#CloudFront.Waiter.InvalidationCompleted)

```python
# InvalidationCompletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_cloudfront.waiter import InvalidationCompletedWaiter

session = get_session()
async with session.create_client("cloudfront") as client:  # (1)
    waiter: InvalidationCompletedWaiter = client.get_waiter("invalidation_completed")  # (2)
    await waiter.wait()
```

1. client: [CloudFrontClient](./client.md)
2. waiter: [InvalidationCompletedWaiter](./waiters.md#invalidationcompletedwaiter)


### wait

Type annotations and code completion for `#!python InvalidationCompletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    DistributionId: str,
    Id: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetInvalidationRequestWaitTypeDef = {  # (1)
    "DistributionId": ...,
    "Id": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetInvalidationRequestWaitTypeDef](./type_defs.md#getinvalidationrequestwaittypedef) 
## StreamingDistributionDeployedWaiter

Type annotations and code completion for `#!python session.create_client("cloudfront").get_waiter("streaming_distribution_deployed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront/waiter/StreamingDistributionDeployed.html#CloudFront.Waiter.StreamingDistributionDeployed)

```python
# StreamingDistributionDeployedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_cloudfront.waiter import StreamingDistributionDeployedWaiter

session = get_session()
async with session.create_client("cloudfront") as client:  # (1)
    waiter: StreamingDistributionDeployedWaiter = client.get_waiter("streaming_distribution_deployed")  # (2)
    await waiter.wait()
```

1. client: [CloudFrontClient](./client.md)
2. waiter: [StreamingDistributionDeployedWaiter](./waiters.md#streamingdistributiondeployedwaiter)


### wait

Type annotations and code completion for `#!python StreamingDistributionDeployedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Id: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetStreamingDistributionRequestWaitTypeDef = {  # (1)
    "Id": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetStreamingDistributionRequestWaitTypeDef](./type_defs.md#getstreamingdistributionrequestwaittypedef) 
