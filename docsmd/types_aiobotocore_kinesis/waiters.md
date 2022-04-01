# Waiters

> [Index](../README.md) > [Kinesis](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [Kinesis](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
    type annotations stubs module [types-aiobotocore-kinesis](https://pypi.org/project/types-aiobotocore-kinesis/).

## StreamExistsWaiter

Type annotations and code completion for `#!python session.create_client("kinesis").get_waiter("stream_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Waiter.StreamExists)

```python title="Usage example"
from aiobotocore.session import Session

from types_aiobotocore_kinesis.waiter import StreamExistsWaiter

def get_stream_exists_waiter() -> StreamExistsWaiter:
    return Session().client("kinesis").get_waiter("stream_exists")
```


### wait

Type annotations and code completion for `#!python StreamExistsWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    StreamName: str,
    Limit: int = ...,
    ExclusiveStartShardId: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeStreamInputStreamExistsWaitTypeDef = {  # (1)
    "StreamName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeStreamInputStreamExistsWaitTypeDef](./type_defs.md#describestreaminputstreamexistswaittypedef) 
## StreamNotExistsWaiter

Type annotations and code completion for `#!python session.create_client("kinesis").get_waiter("stream_not_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Waiter.StreamNotExists)

```python title="Usage example"
from aiobotocore.session import Session

from types_aiobotocore_kinesis.waiter import StreamNotExistsWaiter

def get_stream_not_exists_waiter() -> StreamNotExistsWaiter:
    return Session().client("kinesis").get_waiter("stream_not_exists")
```


### wait

Type annotations and code completion for `#!python StreamNotExistsWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    StreamName: str,
    Limit: int = ...,
    ExclusiveStartShardId: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeStreamInputStreamNotExistsWaitTypeDef = {  # (1)
    "StreamName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeStreamInputStreamNotExistsWaitTypeDef](./type_defs.md#describestreaminputstreamnotexistswaittypedef) 
