<a id="examples-for-aiobotocore-kinesis-module"></a>

# Examples for aiobotocore Kinesis module

> [Index](../README.md) > [Kinesis](./README.md) > Examples

- [Examples for aiobotocore Kinesis module](#examples-for-aiobotocore-kinesis-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[kinesis]` package installed.

Write your `Kinesis` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type KinesisClient
# and provides type checking and code completion
async with session.create_client("kinesis") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_tags_to_stream()
    

    
    # paginator has type DescribeStreamPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_stream")
    async for item in paginator.paginate(...):
        # item has type DescribeStreamOutputTypeDef
        print(item)
    

    
    # waiter has type StreamExistsWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("stream_exists")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[kinesis]` or a standalone
`types_aiobotocore_kinesis` package, you have to explicitly specify
`client: KinesisClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_kinesis.client import KinesisClient
from types_aiobotocore_kinesis.type_defs import None
from types_aiobotocore_kinesis.paginator import DescribeStreamPaginator
from types_aiobotocore_kinesis.waiter import StreamExistsWaiter
from types_aiobotocore_kinesis.literals import PaginatorName
from types_aiobotocore_kinesis.literals import WaiterName


session = get_session()

async with session.create_client("kinesis") as client:
    client: KinesisClient

    
    result: None = client.add_tags_to_stream()
    

    
    paginator_name: PaginatorName = "describe_stream"
    paginator: DescribeStreamPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeStreamOutputTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "stream_exists"
    waiter: StreamExistsWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
