# Examples

> [Index](../README.md) > [RePostPrivate](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [RePostPrivate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace.html#repostprivate)
    type annotations stubs module [types-aiobotocore-repostspace](https://pypi.org/project/types-aiobotocore-repostspace/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[repostspace]` package installed.

Write your `RePostPrivate` code as usual,
type checking and code completion should work out of the box.



```python
# RePostPrivateClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("repostspace") as client:  # (1)
    result = await client.batch_add_role()  # (2)
```

1. client: [RePostPrivateClient](./client.md)
2. result: [:material-code-braces: BatchAddRoleOutputTypeDef](./type_defs.md#batchaddroleoutputtypedef) 



```python
# ListSpacesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("repostspace") as client:  # (1)
    paginator = client.get_paginator("list_spaces")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [RePostPrivateClient](./client.md)
2. paginator: [ListSpacesPaginator](./paginators.md#listspacespaginator)
3. item: [:material-code-braces: ListSpacesOutputTypeDef](./type_defs.md#listspacesoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[repostspace]`
or a standalone `types_aiobotocore_repostspace` package, you have to explicitly specify
`client: RePostPrivateClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# RePostPrivateClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_repostspace.client import RePostPrivateClient
from types_aiobotocore_repostspace.type_defs import BatchAddRoleOutputTypeDef
from types_aiobotocore_repostspace.type_defs import BatchAddRoleInputTypeDef


session = get_session()

async with session.create_client("repostspace") as client:
    client: RePostPrivateClient
    kwargs: BatchAddRoleInputTypeDef = {...}
    result: BatchAddRoleOutputTypeDef = await client.batch_add_role(**kwargs)
```



```python
# ListSpacesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_repostspace.client import RePostPrivateClient
from types_aiobotocore_repostspace.paginator import ListSpacesPaginator
from types_aiobotocore_repostspace.type_defs import ListSpacesOutputTypeDef


session = get_session()

async with session.create_client("repostspace") as client:
    client: RePostPrivateClient
    paginator: ListSpacesPaginator = client.get_paginator("list_spaces")
    async for item in paginator.paginate(...):
        item: ListSpacesOutputTypeDef
        print(item)
```


