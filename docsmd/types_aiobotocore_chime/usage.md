# Examples

> [Index](../README.md) > [Chime](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Chime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#chime)
    type annotations stubs module [types-aiobotocore-chime](https://pypi.org/project/types-aiobotocore-chime/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[chime]` package installed.

Write your `Chime` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ChimeClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("chime") as client:  # (1)
    result = await client.batch_create_room_membership()  # (2)
```

1. client: [ChimeClient](./client.md)
2. result: [:material-code-braces: BatchCreateRoomMembershipResponseTypeDef](./type_defs.md#batchcreateroommembershipresponsetypedef)



#### Paginator usage example

```python
# ListAccountsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("chime") as client:  # (1)
    paginator = client.get_paginator("list_accounts")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ChimeClient](./client.md)
2. paginator: [ListAccountsPaginator](./paginators.md#listaccountspaginator)
3. item: [:material-code-braces: ListAccountsResponseTypeDef](./type_defs.md#listaccountsresponsetypedef)




### Explicit type annotations

With `types-aiobotocore-lite[chime]`
or a standalone `types_aiobotocore_chime` package, you have to explicitly specify
`client: ChimeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ChimeClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_chime.client import ChimeClient
from types_aiobotocore_chime.type_defs import BatchCreateRoomMembershipResponseTypeDef
from types_aiobotocore_chime.type_defs import BatchCreateRoomMembershipRequestTypeDef


session = get_session()

async with session.create_client("chime") as client:
    client: ChimeClient
    kwargs: BatchCreateRoomMembershipRequestTypeDef = {...}
    result: BatchCreateRoomMembershipResponseTypeDef = await client.batch_create_room_membership(**kwargs)
```



#### Paginator usage example

```python
# ListAccountsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_chime.client import ChimeClient
from types_aiobotocore_chime.paginator import ListAccountsPaginator
from types_aiobotocore_chime.type_defs import ListAccountsResponseTypeDef


session = get_session()

async with session.create_client("chime") as client:
    client: ChimeClient
    paginator: ListAccountsPaginator = client.get_paginator("list_accounts")
    async for item in paginator.paginate(...):
        item: ListAccountsResponseTypeDef
        print(item)
```


