# Examples

> [Index](../README.md) > [XRay](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [XRay](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#xray)
    type annotations stubs module [types-aiobotocore-xray](https://pypi.org/project/types-aiobotocore-xray/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[xray]` package installed.

Write your `XRay` code as usual,
type checking and code completion should work out of the box.



```python
# XRayClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("xray") as client:  # (1)
    result = await client.batch_get_traces()  # (2)
```

1. client: [XRayClient](./client.md)
2. result: [:material-code-braces: BatchGetTracesResultTypeDef](./type_defs.md#batchgettracesresulttypedef) 



```python
# BatchGetTracesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("xray") as client:  # (1)
    paginator = client.get_paginator("batch_get_traces")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [XRayClient](./client.md)
2. paginator: [BatchGetTracesPaginator](./paginators.md#batchgettracespaginator)
3. item: [:material-code-braces: BatchGetTracesResultTypeDef](./type_defs.md#batchgettracesresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[xray]`
or a standalone `types_aiobotocore_xray` package, you have to explicitly specify
`client: XRayClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# XRayClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_xray.client import XRayClient
from types_aiobotocore_xray.type_defs import BatchGetTracesResultTypeDef
from types_aiobotocore_xray.type_defs import BatchGetTracesRequestTypeDef


session = get_session()

async with session.create_client("xray") as client:
    client: XRayClient
    kwargs: BatchGetTracesRequestTypeDef = {...}
    result: BatchGetTracesResultTypeDef = await client.batch_get_traces(**kwargs)
```



```python
# BatchGetTracesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_xray.client import XRayClient
from types_aiobotocore_xray.paginator import BatchGetTracesPaginator
from types_aiobotocore_xray.type_defs import BatchGetTracesResultTypeDef


session = get_session()

async with session.create_client("xray") as client:
    client: XRayClient
    paginator: BatchGetTracesPaginator = client.get_paginator("batch_get_traces")
    async for item in paginator.paginate(...):
        item: BatchGetTracesResultTypeDef
        print(item)
```


