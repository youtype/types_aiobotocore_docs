# Waiters

> [Index](../README.md) > [Kinesis](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [Kinesis](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#kinesis)
    type annotations stubs module [types-aiobotocore-kinesis](https://pypi.org/project/types-aiobotocore-kinesis/).

## StreamExistsWaiter

Type annotations and code completion for `#!python session.create_client("kinesis").get_waiter("stream_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/waiter/StreamExists.html#Kinesis.Waiter.StreamExists)

```python
# StreamExistsWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_kinesis.waiter import StreamExistsWaiter

session = get_session()
async with session.create_client("kinesis") as client:  # (1)
    waiter: StreamExistsWaiter = client.get_waiter("stream_exists")  # (2)
    await waiter.wait()
```

1. client: [KinesisClient](./client.md)
2. waiter: [StreamExistsWaiter](./waiters.md#streamexistswaiter)


### wait

Type annotations and code completion for `#!python StreamExistsWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    StreamName: str = ...,
    Limit: int = ...,
    ExclusiveStartShardId: str = ...,
    StreamARN: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeStreamInputWaitTypeDef = {  # (1)
    "StreamName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeStreamInputWaitTypeDef](./type_defs.md#describestreaminputwaittypedef) 
## StreamNotExistsWaiter

Type annotations and code completion for `#!python session.create_client("kinesis").get_waiter("stream_not_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/waiter/StreamNotExists.html#Kinesis.Waiter.StreamNotExists)

```python
# StreamNotExistsWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_kinesis.waiter import StreamNotExistsWaiter

session = get_session()
async with session.create_client("kinesis") as client:  # (1)
    waiter: StreamNotExistsWaiter = client.get_waiter("stream_not_exists")  # (2)
    await waiter.wait()
```

1. client: [KinesisClient](./client.md)
2. waiter: [StreamNotExistsWaiter](./waiters.md#streamnotexistswaiter)


### wait

Type annotations and code completion for `#!python StreamNotExistsWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    StreamName: str = ...,
    Limit: int = ...,
    ExclusiveStartShardId: str = ...,
    StreamARN: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeStreamInputWaitExtraTypeDef = {  # (1)
    "StreamName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeStreamInputWaitExtraTypeDef](./type_defs.md#describestreaminputwaitextratypedef) 
