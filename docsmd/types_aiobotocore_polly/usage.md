# Examples

> [Index](../README.md) > [Polly](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Polly](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#polly)
    type annotations stubs module [types-aiobotocore-polly](https://pypi.org/project/types-aiobotocore-polly/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[polly]` package installed.

Write your `Polly` code as usual,
type checking and code completion should work out of the box.



```python
# PollyClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("polly") as client:  # (1)
    result = await client.describe_voices()  # (2)
```

1. client: [PollyClient](./client.md)
2. result: [:material-code-braces: DescribeVoicesOutputTypeDef](./type_defs.md#describevoicesoutputtypedef) 



```python
# DescribeVoicesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("polly") as client:  # (1)
    paginator = client.get_paginator("describe_voices")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [PollyClient](./client.md)
2. paginator: [DescribeVoicesPaginator](./paginators.md#describevoicespaginator)
3. item: [:material-code-braces: DescribeVoicesOutputTypeDef](./type_defs.md#describevoicesoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[polly]`
or a standalone `types_aiobotocore_polly` package, you have to explicitly specify
`client: PollyClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# PollyClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_polly.client import PollyClient
from types_aiobotocore_polly.type_defs import DescribeVoicesOutputTypeDef
from types_aiobotocore_polly.type_defs import DescribeVoicesInputTypeDef


session = get_session()

async with session.create_client("polly") as client:
    client: PollyClient
    kwargs: DescribeVoicesInputTypeDef = {...}
    result: DescribeVoicesOutputTypeDef = await client.describe_voices(**kwargs)
```



```python
# DescribeVoicesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_polly.client import PollyClient
from types_aiobotocore_polly.paginator import DescribeVoicesPaginator
from types_aiobotocore_polly.type_defs import DescribeVoicesOutputTypeDef


session = get_session()

async with session.create_client("polly") as client:
    client: PollyClient
    paginator: DescribeVoicesPaginator = client.get_paginator("describe_voices")
    async for item in paginator.paginate(...):
        item: DescribeVoicesOutputTypeDef
        print(item)
```


