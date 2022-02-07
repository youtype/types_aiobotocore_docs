<a id="waiters-for-aiobotocore-kinesis-module"></a>

# Waiters for aiobotocore Kinesis module

> [Index](..) > [Kinesis](.) > Waiters

Auto-generated documentation for
[Kinesis](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
type annotations stubs module
[types-aiobotocore-kinesis](https://pypi.org/project/types-aiobotocore-kinesis/).

- [Waiters for aiobotocore Kinesis module](#waiters-for-aiobotocore-kinesis-module)
  - [StreamExistsWaiter](#streamexistswaiter)
  - [StreamNotExistsWaiter](#streamnotexistswaiter)

<a id="streamexistswaiter"></a>

## StreamExistsWaiter

Type annotations for
`session.create_client("kinesis").get_waiter("stream_exists")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_kinesis.waiter import StreamExistsWaiter

def get_stream_exists_waiter() -> StreamExistsWaiter:
    return Session().client("kinesis").get_waiter("stream_exists")
```

Boto3 documentation:
[Kinesis.Waiter.stream_exists](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Waiter.StreamExists)

Arguments for `StreamExistsWaiter.wait` method:

- `StreamName`: `str` *(required)*
- `Limit`: `int`
- `ExclusiveStartShardId`: `str`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="streamnotexistswaiter"></a>

## StreamNotExistsWaiter

Type annotations for
`session.create_client("kinesis").get_waiter("stream_not_exists")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_kinesis.waiter import StreamNotExistsWaiter

def get_stream_not_exists_waiter() -> StreamNotExistsWaiter:
    return Session().client("kinesis").get_waiter("stream_not_exists")
```

Boto3 documentation:
[Kinesis.Waiter.stream_not_exists](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Waiter.StreamNotExists)

Arguments for `StreamNotExistsWaiter.wait` method:

- `StreamName`: `str` *(required)*
- `Limit`: `int`
- `ExclusiveStartShardId`: `str`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
