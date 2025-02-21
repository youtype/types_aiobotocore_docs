# Examples

> [Index](../README.md) > [Kinesis](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Kinesis](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#kinesis)
    type annotations stubs module [types-aiobotocore-kinesis](https://pypi.org/project/types-aiobotocore-kinesis/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[kinesis]` package installed.

Write your `Kinesis` code as usual,
type checking and code completion should work out of the box.



```python
# KinesisClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("kinesis") as client:  # (1)
    result = await client.add_tags_to_stream()  # (2)
```

1. client: [KinesisClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# DescribeStreamPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("kinesis") as client:  # (1)
    paginator = client.get_paginator("describe_stream")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [KinesisClient](./client.md)
2. paginator: [DescribeStreamPaginator](./paginators.md#describestreampaginator)
3. item: [:material-code-braces: DescribeStreamOutputTypeDef](./type_defs.md#describestreamoutputtypedef) 



```python
# StreamExistsWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("kinesis") as client:  # (1)
    waiter = client.get_waiter("stream_exists")  # (2)
    await waiter.wait()
```

1. client: [KinesisClient](./client.md)
2. waiter: [StreamExistsWaiter](./waiters.md#streamexistswaiter)


### Explicit type annotations

With `types-aiobotocore-lite[kinesis]`
or a standalone `types_aiobotocore_kinesis` package, you have to explicitly specify
`client: KinesisClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# KinesisClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_kinesis.client import KinesisClient
from types_aiobotocore_kinesis.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_kinesis.type_defs import AddTagsToStreamInputTypeDef


session = get_session()

async with session.create_client("kinesis") as client:
    client: KinesisClient
    kwargs: AddTagsToStreamInputTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.add_tags_to_stream(**kwargs)
```



```python
# DescribeStreamPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_kinesis.client import KinesisClient
from types_aiobotocore_kinesis.paginator import DescribeStreamPaginator
from types_aiobotocore_kinesis.type_defs import DescribeStreamOutputTypeDef


session = get_session()

async with session.create_client("kinesis") as client:
    client: KinesisClient
    paginator: DescribeStreamPaginator = client.get_paginator("describe_stream")
    async for item in paginator.paginate(...):
        item: DescribeStreamOutputTypeDef
        print(item)
```



```python
# StreamExistsWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_kinesis.client import KinesisClient
from types_aiobotocore_kinesis.waiter import StreamExistsWaiter


session = get_session()

async with session.create_client("kinesis") as client:
    client: KinesisClient
    waiter: StreamExistsWaiter = client.get_waiter("stream_exists")
    await waiter.wait()
```
