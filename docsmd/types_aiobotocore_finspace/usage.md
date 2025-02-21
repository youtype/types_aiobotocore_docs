# Examples

> [Index](../README.md) > [Finspace](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Finspace](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
    type annotations stubs module [types-aiobotocore-finspace](https://pypi.org/project/types-aiobotocore-finspace/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[finspace]` package installed.

Write your `Finspace` code as usual,
type checking and code completion should work out of the box.



```python
# FinspaceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("finspace") as client:  # (1)
    result = await client.create_environment()  # (2)
```

1. client: [FinspaceClient](./client.md)
2. result: [:material-code-braces: CreateEnvironmentResponseTypeDef](./type_defs.md#createenvironmentresponsetypedef) 



```python
# ListKxEnvironmentsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("finspace") as client:  # (1)
    paginator = client.get_paginator("list_kx_environments")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [FinspaceClient](./client.md)
2. paginator: [ListKxEnvironmentsPaginator](./paginators.md#listkxenvironmentspaginator)
3. item: [:material-code-braces: ListKxEnvironmentsResponseTypeDef](./type_defs.md#listkxenvironmentsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[finspace]`
or a standalone `types_aiobotocore_finspace` package, you have to explicitly specify
`client: FinspaceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# FinspaceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_finspace.client import FinspaceClient
from types_aiobotocore_finspace.type_defs import CreateEnvironmentResponseTypeDef
from types_aiobotocore_finspace.type_defs import CreateEnvironmentRequestTypeDef


session = get_session()

async with session.create_client("finspace") as client:
    client: FinspaceClient
    kwargs: CreateEnvironmentRequestTypeDef = {...}
    result: CreateEnvironmentResponseTypeDef = await client.create_environment(**kwargs)
```



```python
# ListKxEnvironmentsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_finspace.client import FinspaceClient
from types_aiobotocore_finspace.paginator import ListKxEnvironmentsPaginator
from types_aiobotocore_finspace.type_defs import ListKxEnvironmentsResponseTypeDef


session = get_session()

async with session.create_client("finspace") as client:
    client: FinspaceClient
    paginator: ListKxEnvironmentsPaginator = client.get_paginator("list_kx_environments")
    async for item in paginator.paginate(...):
        item: ListKxEnvironmentsResponseTypeDef
        print(item)
```


