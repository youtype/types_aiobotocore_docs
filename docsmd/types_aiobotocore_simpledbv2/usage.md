# Examples

> [Index](../README.md) > [SimpleDBv2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SimpleDBv2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simpledbv2.html#simpledbv2)
    type annotations stubs module [types-aiobotocore-simpledbv2](https://pypi.org/project/types-aiobotocore-simpledbv2/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[simpledbv2]` package installed.

Write your `SimpleDBv2` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SimpleDBv2Client usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("simpledbv2") as client:  # (1)
    result = await client.get_export()  # (2)
```

1. client: [SimpleDBv2Client](./client.md)
2. result: [:material-code-braces: GetExportResponseTypeDef](./type_defs.md#getexportresponsetypedef)



#### Paginator usage example

```python
# ListExportsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("simpledbv2") as client:  # (1)
    paginator = client.get_paginator("list_exports")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SimpleDBv2Client](./client.md)
2. paginator: [ListExportsPaginator](./paginators.md#listexportspaginator)
3. item: [:material-code-braces: ListExportsResponseTypeDef](./type_defs.md#listexportsresponsetypedef)



#### Waiter usage example

```python
# ExportSucceededWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("simpledbv2") as client:  # (1)
    waiter = client.get_waiter("export_succeeded")  # (2)
    await waiter.wait(...)
```

1. client: [SimpleDBv2Client](./client.md)
2. waiter: [ExportSucceededWaiter](./waiters.md#exportsucceededwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[simpledbv2]`
or a standalone `types_aiobotocore_simpledbv2` package, you have to explicitly specify
`client: SimpleDBv2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SimpleDBv2Client usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_simpledbv2.client import SimpleDBv2Client
from types_aiobotocore_simpledbv2.type_defs import GetExportResponseTypeDef
from types_aiobotocore_simpledbv2.type_defs import GetExportRequestTypeDef


session = get_session()

async with session.create_client("simpledbv2") as client:
    client: SimpleDBv2Client
    kwargs: GetExportRequestTypeDef = {...}
    result: GetExportResponseTypeDef = await client.get_export(**kwargs)
```



#### Paginator usage example

```python
# ListExportsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_simpledbv2.client import SimpleDBv2Client
from types_aiobotocore_simpledbv2.paginator import ListExportsPaginator
from types_aiobotocore_simpledbv2.type_defs import ListExportsResponseTypeDef


session = get_session()

async with session.create_client("simpledbv2") as client:
    client: SimpleDBv2Client
    paginator: ListExportsPaginator = client.get_paginator("list_exports")
    async for item in paginator.paginate(...):
        item: ListExportsResponseTypeDef
        print(item)
```



#### Waiter usage example

```python
# ExportSucceededWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_simpledbv2.client import SimpleDBv2Client
from types_aiobotocore_simpledbv2.waiter import ExportSucceededWaiter


session = get_session()

async with session.create_client("simpledbv2") as client:
    client: SimpleDBv2Client
    waiter: ExportSucceededWaiter = client.get_waiter("export_succeeded")
    await waiter.wait(...)
```
