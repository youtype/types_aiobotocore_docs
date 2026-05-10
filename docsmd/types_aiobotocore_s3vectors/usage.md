# Examples

> [Index](../README.md) > [S3Vectors](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [S3Vectors](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors.html#s3vectors)
    type annotations stubs module [types-aiobotocore-s3vectors](https://pypi.org/project/types-aiobotocore-s3vectors/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[s3vectors]` package installed.

Write your `S3Vectors` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# S3VectorsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("s3vectors") as client:  # (1)
    result = await client.create_index()  # (2)
```

1. client: [S3VectorsClient](./client.md)
2. result: [:material-code-braces: CreateIndexOutputTypeDef](./type_defs.md#createindexoutputtypedef)



#### Paginator usage example

```python
# ListIndexesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("s3vectors") as client:  # (1)
    paginator = client.get_paginator("list_indexes")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [S3VectorsClient](./client.md)
2. paginator: [ListIndexesPaginator](./paginators.md#listindexespaginator)
3. item: [:material-code-braces: ListIndexesOutputTypeDef](./type_defs.md#listindexesoutputtypedef)




### Explicit type annotations

With `types-aiobotocore-lite[s3vectors]`
or a standalone `types_aiobotocore_s3vectors` package, you have to explicitly specify
`client: S3VectorsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# S3VectorsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_s3vectors.client import S3VectorsClient
from types_aiobotocore_s3vectors.type_defs import CreateIndexOutputTypeDef
from types_aiobotocore_s3vectors.type_defs import CreateIndexInputTypeDef


session = get_session()

async with session.create_client("s3vectors") as client:
    client: S3VectorsClient
    kwargs: CreateIndexInputTypeDef = {...}
    result: CreateIndexOutputTypeDef = await client.create_index(**kwargs)
```



#### Paginator usage example

```python
# ListIndexesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_s3vectors.client import S3VectorsClient
from types_aiobotocore_s3vectors.paginator import ListIndexesPaginator
from types_aiobotocore_s3vectors.type_defs import ListIndexesOutputTypeDef


session = get_session()

async with session.create_client("s3vectors") as client:
    client: S3VectorsClient
    paginator: ListIndexesPaginator = client.get_paginator("list_indexes")
    async for item in paginator.paginate(...):
        item: ListIndexesOutputTypeDef
        print(item)
```


