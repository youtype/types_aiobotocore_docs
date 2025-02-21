# Examples

> [Index](../README.md) > [Keyspaces](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Keyspaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#keyspaces)
    type annotations stubs module [types-aiobotocore-keyspaces](https://pypi.org/project/types-aiobotocore-keyspaces/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[keyspaces]` package installed.

Write your `Keyspaces` code as usual,
type checking and code completion should work out of the box.



```python
# KeyspacesClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("keyspaces") as client:  # (1)
    result = await client.create_keyspace()  # (2)
```

1. client: [KeyspacesClient](./client.md)
2. result: [:material-code-braces: CreateKeyspaceResponseTypeDef](./type_defs.md#createkeyspaceresponsetypedef) 



```python
# ListKeyspacesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("keyspaces") as client:  # (1)
    paginator = client.get_paginator("list_keyspaces")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [KeyspacesClient](./client.md)
2. paginator: [ListKeyspacesPaginator](./paginators.md#listkeyspacespaginator)
3. item: [:material-code-braces: ListKeyspacesResponseTypeDef](./type_defs.md#listkeyspacesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[keyspaces]`
or a standalone `types_aiobotocore_keyspaces` package, you have to explicitly specify
`client: KeyspacesClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# KeyspacesClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_keyspaces.client import KeyspacesClient
from types_aiobotocore_keyspaces.type_defs import CreateKeyspaceResponseTypeDef
from types_aiobotocore_keyspaces.type_defs import CreateKeyspaceRequestTypeDef


session = get_session()

async with session.create_client("keyspaces") as client:
    client: KeyspacesClient
    kwargs: CreateKeyspaceRequestTypeDef = {...}
    result: CreateKeyspaceResponseTypeDef = await client.create_keyspace(**kwargs)
```



```python
# ListKeyspacesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_keyspaces.client import KeyspacesClient
from types_aiobotocore_keyspaces.paginator import ListKeyspacesPaginator
from types_aiobotocore_keyspaces.type_defs import ListKeyspacesResponseTypeDef


session = get_session()

async with session.create_client("keyspaces") as client:
    client: KeyspacesClient
    paginator: ListKeyspacesPaginator = client.get_paginator("list_keyspaces")
    async for item in paginator.paginate(...):
        item: ListKeyspacesResponseTypeDef
        print(item)
```


