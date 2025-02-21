# Examples

> [Index](../README.md) > [Batch](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Batch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#batch)
    type annotations stubs module [types-aiobotocore-batch](https://pypi.org/project/types-aiobotocore-batch/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[batch]` package installed.

Write your `Batch` code as usual,
type checking and code completion should work out of the box.



```python
# BatchClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("batch") as client:  # (1)
    result = await client.create_compute_environment()  # (2)
```

1. client: [BatchClient](./client.md)
2. result: [:material-code-braces: CreateComputeEnvironmentResponseTypeDef](./type_defs.md#createcomputeenvironmentresponsetypedef) 



```python
# DescribeComputeEnvironmentsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("batch") as client:  # (1)
    paginator = client.get_paginator("describe_compute_environments")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [BatchClient](./client.md)
2. paginator: [DescribeComputeEnvironmentsPaginator](./paginators.md#describecomputeenvironmentspaginator)
3. item: [:material-code-braces: DescribeComputeEnvironmentsResponseTypeDef](./type_defs.md#describecomputeenvironmentsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[batch]`
or a standalone `types_aiobotocore_batch` package, you have to explicitly specify
`client: BatchClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# BatchClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_batch.client import BatchClient
from types_aiobotocore_batch.type_defs import CreateComputeEnvironmentResponseTypeDef
from types_aiobotocore_batch.type_defs import CreateComputeEnvironmentRequestTypeDef


session = get_session()

async with session.create_client("batch") as client:
    client: BatchClient
    kwargs: CreateComputeEnvironmentRequestTypeDef = {...}
    result: CreateComputeEnvironmentResponseTypeDef = await client.create_compute_environment(**kwargs)
```



```python
# DescribeComputeEnvironmentsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_batch.client import BatchClient
from types_aiobotocore_batch.paginator import DescribeComputeEnvironmentsPaginator
from types_aiobotocore_batch.type_defs import DescribeComputeEnvironmentsResponseTypeDef


session = get_session()

async with session.create_client("batch") as client:
    client: BatchClient
    paginator: DescribeComputeEnvironmentsPaginator = client.get_paginator("describe_compute_environments")
    async for item in paginator.paginate(...):
        item: DescribeComputeEnvironmentsResponseTypeDef
        print(item)
```


