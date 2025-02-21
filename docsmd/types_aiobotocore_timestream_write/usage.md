# Examples

> [Index](../README.md) > [TimestreamWrite](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [TimestreamWrite](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#timestreamwrite)
    type annotations stubs module [types-aiobotocore-timestream-write](https://pypi.org/project/types-aiobotocore-timestream-write/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[timestream-write]` package installed.

Write your `TimestreamWrite` code as usual,
type checking and code completion should work out of the box.



```python
# TimestreamWriteClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("timestream-write") as client:  # (1)
    result = await client.create_batch_load_task()  # (2)
```

1. client: [TimestreamWriteClient](./client.md)
2. result: [:material-code-braces: CreateBatchLoadTaskResponseTypeDef](./type_defs.md#createbatchloadtaskresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[timestream-write]`
or a standalone `types_aiobotocore_timestream_write` package, you have to explicitly specify
`client: TimestreamWriteClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# TimestreamWriteClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_timestream_write.client import TimestreamWriteClient
from types_aiobotocore_timestream_write.type_defs import CreateBatchLoadTaskResponseTypeDef
from types_aiobotocore_timestream_write.type_defs import CreateBatchLoadTaskRequestTypeDef


session = get_session()

async with session.create_client("timestream-write") as client:
    client: TimestreamWriteClient
    kwargs: CreateBatchLoadTaskRequestTypeDef = {...}
    result: CreateBatchLoadTaskResponseTypeDef = await client.create_batch_load_task(**kwargs)
```




