# Examples

> [Index](../README.md) > [FinSpaceData](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [FinSpaceData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#finspacedata)
    type annotations stubs module [types-aiobotocore-finspace-data](https://pypi.org/project/types-aiobotocore-finspace-data/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[finspace-data]` package installed.

Write your `FinSpaceData` code as usual,
type checking and code completion should work out of the box.



```python
# FinSpaceDataClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("finspace-data") as client:  # (1)
    result = await client.associate_user_to_permission_group()  # (2)
```

1. client: [FinSpaceDataClient](./client.md)
2. result: [:material-code-braces: AssociateUserToPermissionGroupResponseTypeDef](./type_defs.md#associateusertopermissiongroupresponsetypedef) 



```python
# ListChangesetsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("finspace-data") as client:  # (1)
    paginator = client.get_paginator("list_changesets")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [FinSpaceDataClient](./client.md)
2. paginator: [ListChangesetsPaginator](./paginators.md#listchangesetspaginator)
3. item: [:material-code-braces: ListChangesetsResponseTypeDef](./type_defs.md#listchangesetsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[finspace-data]`
or a standalone `types_aiobotocore_finspace_data` package, you have to explicitly specify
`client: FinSpaceDataClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# FinSpaceDataClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_finspace_data.client import FinSpaceDataClient
from types_aiobotocore_finspace_data.type_defs import AssociateUserToPermissionGroupResponseTypeDef
from types_aiobotocore_finspace_data.type_defs import AssociateUserToPermissionGroupRequestTypeDef


session = get_session()

async with session.create_client("finspace-data") as client:
    client: FinSpaceDataClient
    kwargs: AssociateUserToPermissionGroupRequestTypeDef = {...}
    result: AssociateUserToPermissionGroupResponseTypeDef = await client.associate_user_to_permission_group(**kwargs)
```



```python
# ListChangesetsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_finspace_data.client import FinSpaceDataClient
from types_aiobotocore_finspace_data.paginator import ListChangesetsPaginator
from types_aiobotocore_finspace_data.type_defs import ListChangesetsResponseTypeDef


session = get_session()

async with session.create_client("finspace-data") as client:
    client: FinSpaceDataClient
    paginator: ListChangesetsPaginator = client.get_paginator("list_changesets")
    async for item in paginator.paginate(...):
        item: ListChangesetsResponseTypeDef
        print(item)
```


