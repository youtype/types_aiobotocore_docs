# Examples

> [Index](../README.md) > [Schemas](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Schemas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#schemas)
    type annotations stubs module [types-aiobotocore-schemas](https://pypi.org/project/types-aiobotocore-schemas/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[schemas]` package installed.

Write your `Schemas` code as usual,
type checking and code completion should work out of the box.



```python
# SchemasClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("schemas") as client:  # (1)
    result = await client.create_discoverer()  # (2)
```

1. client: [SchemasClient](./client.md)
2. result: [:material-code-braces: CreateDiscovererResponseTypeDef](./type_defs.md#creatediscovererresponsetypedef) 



```python
# ListDiscoverersPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("schemas") as client:  # (1)
    paginator = client.get_paginator("list_discoverers")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SchemasClient](./client.md)
2. paginator: [ListDiscoverersPaginator](./paginators.md#listdiscovererspaginator)
3. item: [:material-code-braces: ListDiscoverersResponseTypeDef](./type_defs.md#listdiscoverersresponsetypedef) 



```python
# CodeBindingExistsWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("schemas") as client:  # (1)
    waiter = client.get_waiter("code_binding_exists")  # (2)
    await waiter.wait()
```

1. client: [SchemasClient](./client.md)
2. waiter: [CodeBindingExistsWaiter](./waiters.md#codebindingexistswaiter)


### Explicit type annotations

With `types-aiobotocore-lite[schemas]`
or a standalone `types_aiobotocore_schemas` package, you have to explicitly specify
`client: SchemasClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SchemasClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_schemas.client import SchemasClient
from types_aiobotocore_schemas.type_defs import CreateDiscovererResponseTypeDef
from types_aiobotocore_schemas.type_defs import CreateDiscovererRequestTypeDef


session = get_session()

async with session.create_client("schemas") as client:
    client: SchemasClient
    kwargs: CreateDiscovererRequestTypeDef = {...}
    result: CreateDiscovererResponseTypeDef = await client.create_discoverer(**kwargs)
```



```python
# ListDiscoverersPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_schemas.client import SchemasClient
from types_aiobotocore_schemas.paginator import ListDiscoverersPaginator
from types_aiobotocore_schemas.type_defs import ListDiscoverersResponseTypeDef


session = get_session()

async with session.create_client("schemas") as client:
    client: SchemasClient
    paginator: ListDiscoverersPaginator = client.get_paginator("list_discoverers")
    async for item in paginator.paginate(...):
        item: ListDiscoverersResponseTypeDef
        print(item)
```



```python
# CodeBindingExistsWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_schemas.client import SchemasClient
from types_aiobotocore_schemas.waiter import CodeBindingExistsWaiter


session = get_session()

async with session.create_client("schemas") as client:
    client: SchemasClient
    waiter: CodeBindingExistsWaiter = client.get_waiter("code_binding_exists")
    await waiter.wait()
```
