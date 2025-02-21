# Examples

> [Index](../README.md) > [DirectoryServiceData](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DirectoryServiceData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data.html#directoryservicedata)
    type annotations stubs module [types-aiobotocore-ds-data](https://pypi.org/project/types-aiobotocore-ds-data/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[ds-data]` package installed.

Write your `DirectoryServiceData` code as usual,
type checking and code completion should work out of the box.



```python
# DirectoryServiceDataClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ds-data") as client:  # (1)
    result = await client.create_group()  # (2)
```

1. client: [DirectoryServiceDataClient](./client.md)
2. result: [:material-code-braces: CreateGroupResultTypeDef](./type_defs.md#creategroupresulttypedef) 



```python
# ListGroupMembersPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ds-data") as client:  # (1)
    paginator = client.get_paginator("list_group_members")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DirectoryServiceDataClient](./client.md)
2. paginator: [ListGroupMembersPaginator](./paginators.md#listgroupmemberspaginator)
3. item: [:material-code-braces: ListGroupMembersResultTypeDef](./type_defs.md#listgroupmembersresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[ds-data]`
or a standalone `types_aiobotocore_ds_data` package, you have to explicitly specify
`client: DirectoryServiceDataClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# DirectoryServiceDataClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ds_data.client import DirectoryServiceDataClient
from types_aiobotocore_ds_data.type_defs import CreateGroupResultTypeDef
from types_aiobotocore_ds_data.type_defs import CreateGroupRequestTypeDef


session = get_session()

async with session.create_client("ds-data") as client:
    client: DirectoryServiceDataClient
    kwargs: CreateGroupRequestTypeDef = {...}
    result: CreateGroupResultTypeDef = await client.create_group(**kwargs)
```



```python
# ListGroupMembersPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ds_data.client import DirectoryServiceDataClient
from types_aiobotocore_ds_data.paginator import ListGroupMembersPaginator
from types_aiobotocore_ds_data.type_defs import ListGroupMembersResultTypeDef


session = get_session()

async with session.create_client("ds-data") as client:
    client: DirectoryServiceDataClient
    paginator: ListGroupMembersPaginator = client.get_paginator("list_group_members")
    async for item in paginator.paginate(...):
        item: ListGroupMembersResultTypeDef
        print(item)
```


