# Examples

> [Index](../README.md) > [IdentityStore](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IdentityStore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#identitystore)
    type annotations stubs module [types-aiobotocore-identitystore](https://pypi.org/project/types-aiobotocore-identitystore/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[identitystore]` package installed.

Write your `IdentityStore` code as usual,
type checking and code completion should work out of the box.



```python
# IdentityStoreClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("identitystore") as client:  # (1)
    result = await client.create_group()  # (2)
```

1. client: [IdentityStoreClient](./client.md)
2. result: [:material-code-braces: CreateGroupResponseTypeDef](./type_defs.md#creategroupresponsetypedef) 



```python
# ListGroupMembershipsForMemberPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("identitystore") as client:  # (1)
    paginator = client.get_paginator("list_group_memberships_for_member")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [IdentityStoreClient](./client.md)
2. paginator: [ListGroupMembershipsForMemberPaginator](./paginators.md#listgroupmembershipsformemberpaginator)
3. item: [:material-code-braces: ListGroupMembershipsForMemberResponseTypeDef](./type_defs.md#listgroupmembershipsformemberresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[identitystore]`
or a standalone `types_aiobotocore_identitystore` package, you have to explicitly specify
`client: IdentityStoreClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# IdentityStoreClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_identitystore.client import IdentityStoreClient
from types_aiobotocore_identitystore.type_defs import CreateGroupResponseTypeDef
from types_aiobotocore_identitystore.type_defs import CreateGroupRequestTypeDef


session = get_session()

async with session.create_client("identitystore") as client:
    client: IdentityStoreClient
    kwargs: CreateGroupRequestTypeDef = {...}
    result: CreateGroupResponseTypeDef = await client.create_group(**kwargs)
```



```python
# ListGroupMembershipsForMemberPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_identitystore.client import IdentityStoreClient
from types_aiobotocore_identitystore.paginator import ListGroupMembershipsForMemberPaginator
from types_aiobotocore_identitystore.type_defs import ListGroupMembershipsForMemberResponseTypeDef


session = get_session()

async with session.create_client("identitystore") as client:
    client: IdentityStoreClient
    paginator: ListGroupMembershipsForMemberPaginator = client.get_paginator("list_group_memberships_for_member")
    async for item in paginator.paginate(...):
        item: ListGroupMembershipsForMemberResponseTypeDef
        print(item)
```


