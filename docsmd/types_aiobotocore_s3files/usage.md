# Examples

> [Index](../README.md) > [S3Files](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [S3Files](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3files.html#s3files)
    type annotations stubs module [types-aiobotocore-s3files](https://pypi.org/project/types-aiobotocore-s3files/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[s3files]` package installed.

Write your `S3Files` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# S3FilesClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("s3files") as client:  # (1)
    result = await client.create_access_point()  # (2)
```

1. client: [S3FilesClient](./client.md)
2. result: [:material-code-braces: CreateAccessPointResponseTypeDef](./type_defs.md#createaccesspointresponsetypedef)



#### Paginator usage example

```python
# ListAccessPointsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("s3files") as client:  # (1)
    paginator = client.get_paginator("list_access_points")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [S3FilesClient](./client.md)
2. paginator: [ListAccessPointsPaginator](./paginators.md#listaccesspointspaginator)
3. item: [:material-code-braces: ListAccessPointsResponseTypeDef](./type_defs.md#listaccesspointsresponsetypedef)




### Explicit type annotations

With `types-aiobotocore-lite[s3files]`
or a standalone `types_aiobotocore_s3files` package, you have to explicitly specify
`client: S3FilesClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# S3FilesClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_s3files.client import S3FilesClient
from types_aiobotocore_s3files.type_defs import CreateAccessPointResponseTypeDef
from types_aiobotocore_s3files.type_defs import CreateAccessPointRequestTypeDef


session = get_session()

async with session.create_client("s3files") as client:
    client: S3FilesClient
    kwargs: CreateAccessPointRequestTypeDef = {...}
    result: CreateAccessPointResponseTypeDef = await client.create_access_point(**kwargs)
```



#### Paginator usage example

```python
# ListAccessPointsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_s3files.client import S3FilesClient
from types_aiobotocore_s3files.paginator import ListAccessPointsPaginator
from types_aiobotocore_s3files.type_defs import ListAccessPointsResponseTypeDef


session = get_session()

async with session.create_client("s3files") as client:
    client: S3FilesClient
    paginator: ListAccessPointsPaginator = client.get_paginator("list_access_points")
    async for item in paginator.paginate(...):
        item: ListAccessPointsResponseTypeDef
        print(item)
```


