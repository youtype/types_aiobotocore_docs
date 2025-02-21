# Examples

> [Index](../README.md) > [Glue](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Glue](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#glue)
    type annotations stubs module [types-aiobotocore-glue](https://pypi.org/project/types-aiobotocore-glue/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[glue]` package installed.

Write your `Glue` code as usual,
type checking and code completion should work out of the box.



```python
# GlueClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("glue") as client:  # (1)
    result = await client.batch_create_partition()  # (2)
```

1. client: [GlueClient](./client.md)
2. result: [:material-code-braces: BatchCreatePartitionResponseTypeDef](./type_defs.md#batchcreatepartitionresponsetypedef) 



```python
# DescribeEntityPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("glue") as client:  # (1)
    paginator = client.get_paginator("describe_entity")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [DescribeEntityPaginator](./paginators.md#describeentitypaginator)
3. item: [:material-code-braces: DescribeEntityResponseTypeDef](./type_defs.md#describeentityresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[glue]`
or a standalone `types_aiobotocore_glue` package, you have to explicitly specify
`client: GlueClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# GlueClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_glue.client import GlueClient
from types_aiobotocore_glue.type_defs import BatchCreatePartitionResponseTypeDef
from types_aiobotocore_glue.type_defs import BatchCreatePartitionRequestTypeDef


session = get_session()

async with session.create_client("glue") as client:
    client: GlueClient
    kwargs: BatchCreatePartitionRequestTypeDef = {...}
    result: BatchCreatePartitionResponseTypeDef = await client.batch_create_partition(**kwargs)
```



```python
# DescribeEntityPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_glue.client import GlueClient
from types_aiobotocore_glue.paginator import DescribeEntityPaginator
from types_aiobotocore_glue.type_defs import DescribeEntityResponseTypeDef


session = get_session()

async with session.create_client("glue") as client:
    client: GlueClient
    paginator: DescribeEntityPaginator = client.get_paginator("describe_entity")
    async for item in paginator.paginate(...):
        item: DescribeEntityResponseTypeDef
        print(item)
```


