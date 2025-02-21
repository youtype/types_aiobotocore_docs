# Examples

> [Index](../README.md) > [UserNotificationsContacts](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [UserNotificationsContacts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notificationscontacts.html#usernotificationscontacts)
    type annotations stubs module [types-aiobotocore-notificationscontacts](https://pypi.org/project/types-aiobotocore-notificationscontacts/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[notificationscontacts]` package installed.

Write your `UserNotificationsContacts` code as usual,
type checking and code completion should work out of the box.



```python
# UserNotificationsContactsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("notificationscontacts") as client:  # (1)
    result = await client.create_email_contact()  # (2)
```

1. client: [UserNotificationsContactsClient](./client.md)
2. result: [:material-code-braces: CreateEmailContactResponseTypeDef](./type_defs.md#createemailcontactresponsetypedef) 



```python
# ListEmailContactsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("notificationscontacts") as client:  # (1)
    paginator = client.get_paginator("list_email_contacts")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [UserNotificationsContactsClient](./client.md)
2. paginator: [ListEmailContactsPaginator](./paginators.md#listemailcontactspaginator)
3. item: [:material-code-braces: ListEmailContactsResponseTypeDef](./type_defs.md#listemailcontactsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[notificationscontacts]`
or a standalone `types_aiobotocore_notificationscontacts` package, you have to explicitly specify
`client: UserNotificationsContactsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# UserNotificationsContactsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_notificationscontacts.client import UserNotificationsContactsClient
from types_aiobotocore_notificationscontacts.type_defs import CreateEmailContactResponseTypeDef
from types_aiobotocore_notificationscontacts.type_defs import CreateEmailContactRequestTypeDef


session = get_session()

async with session.create_client("notificationscontacts") as client:
    client: UserNotificationsContactsClient
    kwargs: CreateEmailContactRequestTypeDef = {...}
    result: CreateEmailContactResponseTypeDef = await client.create_email_contact(**kwargs)
```



```python
# ListEmailContactsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_notificationscontacts.client import UserNotificationsContactsClient
from types_aiobotocore_notificationscontacts.paginator import ListEmailContactsPaginator
from types_aiobotocore_notificationscontacts.type_defs import ListEmailContactsResponseTypeDef


session = get_session()

async with session.create_client("notificationscontacts") as client:
    client: UserNotificationsContactsClient
    paginator: ListEmailContactsPaginator = client.get_paginator("list_email_contacts")
    async for item in paginator.paginate(...):
        item: ListEmailContactsResponseTypeDef
        print(item)
```


