# Examples

> [Index](../README.md) > [WickrAdminAPI](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WickrAdminAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wickr.html#wickradminapi)
    type annotations stubs module [types-aiobotocore-wickr](https://pypi.org/project/types-aiobotocore-wickr/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[wickr]` package installed.

Write your `WickrAdminAPI` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# WickrAdminAPIClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("wickr") as client:  # (1)
    result = await client.batch_create_user()  # (2)
```

1. client: [WickrAdminAPIClient](./client.md)
2. result: [:material-code-braces: BatchCreateUserResponseTypeDef](./type_defs.md#batchcreateuserresponsetypedef)



#### Paginator usage example

```python
# ListBlockedGuestUsersPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("wickr") as client:  # (1)
    paginator = client.get_paginator("list_blocked_guest_users")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [WickrAdminAPIClient](./client.md)
2. paginator: [ListBlockedGuestUsersPaginator](./paginators.md#listblockedguestuserspaginator)
3. item: [:material-code-braces: ListBlockedGuestUsersResponseTypeDef](./type_defs.md#listblockedguestusersresponsetypedef)




### Explicit type annotations

With `types-aiobotocore-lite[wickr]`
or a standalone `types_aiobotocore_wickr` package, you have to explicitly specify
`client: WickrAdminAPIClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# WickrAdminAPIClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_wickr.client import WickrAdminAPIClient
from types_aiobotocore_wickr.type_defs import BatchCreateUserResponseTypeDef
from types_aiobotocore_wickr.type_defs import BatchCreateUserRequestTypeDef


session = get_session()

async with session.create_client("wickr") as client:
    client: WickrAdminAPIClient
    kwargs: BatchCreateUserRequestTypeDef = {...}
    result: BatchCreateUserResponseTypeDef = await client.batch_create_user(**kwargs)
```



#### Paginator usage example

```python
# ListBlockedGuestUsersPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_wickr.client import WickrAdminAPIClient
from types_aiobotocore_wickr.paginator import ListBlockedGuestUsersPaginator
from types_aiobotocore_wickr.type_defs import ListBlockedGuestUsersResponseTypeDef


session = get_session()

async with session.create_client("wickr") as client:
    client: WickrAdminAPIClient
    paginator: ListBlockedGuestUsersPaginator = client.get_paginator("list_blocked_guest_users")
    async for item in paginator.paginate(...):
        item: ListBlockedGuestUsersResponseTypeDef
        print(item)
```


