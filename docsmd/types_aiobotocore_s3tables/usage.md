# Examples

> [Index](../README.md) > [S3Tables](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [S3Tables](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables.html#s3tables)
    type annotations stubs module [types-aiobotocore-s3tables](https://pypi.org/project/types-aiobotocore-s3tables/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[s3tables]` package installed.

Write your `S3Tables` code as usual,
type checking and code completion should work out of the box.



```python
# S3TablesClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("s3tables") as client:  # (1)
    result = await client.create_namespace()  # (2)
```

1. client: [S3TablesClient](./client.md)
2. result: [:material-code-braces: CreateNamespaceResponseTypeDef](./type_defs.md#createnamespaceresponsetypedef) 



```python
# ListNamespacesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("s3tables") as client:  # (1)
    paginator = client.get_paginator("list_namespaces")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [S3TablesClient](./client.md)
2. paginator: [ListNamespacesPaginator](./paginators.md#listnamespacespaginator)
3. item: [:material-code-braces: ListNamespacesResponseTypeDef](./type_defs.md#listnamespacesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[s3tables]`
or a standalone `types_aiobotocore_s3tables` package, you have to explicitly specify
`client: S3TablesClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# S3TablesClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_s3tables.client import S3TablesClient
from types_aiobotocore_s3tables.type_defs import CreateNamespaceResponseTypeDef
from types_aiobotocore_s3tables.type_defs import CreateNamespaceRequestTypeDef


session = get_session()

async with session.create_client("s3tables") as client:
    client: S3TablesClient
    kwargs: CreateNamespaceRequestTypeDef = {...}
    result: CreateNamespaceResponseTypeDef = await client.create_namespace(**kwargs)
```



```python
# ListNamespacesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_s3tables.client import S3TablesClient
from types_aiobotocore_s3tables.paginator import ListNamespacesPaginator
from types_aiobotocore_s3tables.type_defs import ListNamespacesResponseTypeDef


session = get_session()

async with session.create_client("s3tables") as client:
    client: S3TablesClient
    paginator: ListNamespacesPaginator = client.get_paginator("list_namespaces")
    async for item in paginator.paginate(...):
        item: ListNamespacesResponseTypeDef
        print(item)
```


