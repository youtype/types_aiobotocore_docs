# Examples

> [Index](../README.md) > [ResourceExplorer](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ResourceExplorer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#resourceexplorer)
    type annotations stubs module [types-aiobotocore-resource-explorer-2](https://pypi.org/project/types-aiobotocore-resource-explorer-2/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[resource-explorer-2]` package installed.

Write your `ResourceExplorer` code as usual,
type checking and code completion should work out of the box.



```python
# ResourceExplorerClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("resource-explorer-2") as client:  # (1)
    result = await client.associate_default_view()  # (2)
```

1. client: [ResourceExplorerClient](./client.md)
2. result: [:material-code-braces: AssociateDefaultViewOutputTypeDef](./type_defs.md#associatedefaultviewoutputtypedef) 



```python
# ListIndexesForMembersPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("resource-explorer-2") as client:  # (1)
    paginator = client.get_paginator("list_indexes_for_members")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [ListIndexesForMembersPaginator](./paginators.md#listindexesformemberspaginator)
3. item: [:material-code-braces: ListIndexesForMembersOutputTypeDef](./type_defs.md#listindexesformembersoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[resource-explorer-2]`
or a standalone `types_aiobotocore_resource_explorer_2` package, you have to explicitly specify
`client: ResourceExplorerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ResourceExplorerClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_resource_explorer_2.client import ResourceExplorerClient
from types_aiobotocore_resource_explorer_2.type_defs import AssociateDefaultViewOutputTypeDef
from types_aiobotocore_resource_explorer_2.type_defs import AssociateDefaultViewInputTypeDef


session = get_session()

async with session.create_client("resource-explorer-2") as client:
    client: ResourceExplorerClient
    kwargs: AssociateDefaultViewInputTypeDef = {...}
    result: AssociateDefaultViewOutputTypeDef = await client.associate_default_view(**kwargs)
```



```python
# ListIndexesForMembersPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_resource_explorer_2.client import ResourceExplorerClient
from types_aiobotocore_resource_explorer_2.paginator import ListIndexesForMembersPaginator
from types_aiobotocore_resource_explorer_2.type_defs import ListIndexesForMembersOutputTypeDef


session = get_session()

async with session.create_client("resource-explorer-2") as client:
    client: ResourceExplorerClient
    paginator: ListIndexesForMembersPaginator = client.get_paginator("list_indexes_for_members")
    async for item in paginator.paginate(...):
        item: ListIndexesForMembersOutputTypeDef
        print(item)
```


