# Examples

> [Index](../README.md) > [DynamoDBStreams](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DynamoDBStreams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#dynamodbstreams)
    type annotations stubs module [types-aiobotocore-dynamodbstreams](https://pypi.org/project/types-aiobotocore-dynamodbstreams/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[dynamodbstreams]` package installed.

Write your `DynamoDBStreams` code as usual,
type checking and code completion should work out of the box.



```python
# DynamoDBStreamsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("dynamodbstreams") as client:  # (1)
    result = await client.describe_stream()  # (2)
```

1. client: [DynamoDBStreamsClient](./client.md)
2. result: [:material-code-braces: DescribeStreamOutputTypeDef](./type_defs.md#describestreamoutputtypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[dynamodbstreams]`
or a standalone `types_aiobotocore_dynamodbstreams` package, you have to explicitly specify
`client: DynamoDBStreamsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# DynamoDBStreamsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_dynamodbstreams.client import DynamoDBStreamsClient
from types_aiobotocore_dynamodbstreams.type_defs import DescribeStreamOutputTypeDef
from types_aiobotocore_dynamodbstreams.type_defs import DescribeStreamInputTypeDef


session = get_session()

async with session.create_client("dynamodbstreams") as client:
    client: DynamoDBStreamsClient
    kwargs: DescribeStreamInputTypeDef = {...}
    result: DescribeStreamOutputTypeDef = await client.describe_stream(**kwargs)
```




