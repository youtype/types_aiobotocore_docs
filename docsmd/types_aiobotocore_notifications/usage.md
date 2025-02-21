# Examples

> [Index](../README.md) > [UserNotifications](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [UserNotifications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications.html#usernotifications)
    type annotations stubs module [types-aiobotocore-notifications](https://pypi.org/project/types-aiobotocore-notifications/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[notifications]` package installed.

Write your `UserNotifications` code as usual,
type checking and code completion should work out of the box.



```python
# UserNotificationsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("notifications") as client:  # (1)
    result = await client.create_event_rule()  # (2)
```

1. client: [UserNotificationsClient](./client.md)
2. result: [:material-code-braces: CreateEventRuleResponseTypeDef](./type_defs.md#createeventruleresponsetypedef) 



```python
# ListChannelsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("notifications") as client:  # (1)
    paginator = client.get_paginator("list_channels")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [UserNotificationsClient](./client.md)
2. paginator: [ListChannelsPaginator](./paginators.md#listchannelspaginator)
3. item: [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[notifications]`
or a standalone `types_aiobotocore_notifications` package, you have to explicitly specify
`client: UserNotificationsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# UserNotificationsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_notifications.client import UserNotificationsClient
from types_aiobotocore_notifications.type_defs import CreateEventRuleResponseTypeDef
from types_aiobotocore_notifications.type_defs import CreateEventRuleRequestTypeDef


session = get_session()

async with session.create_client("notifications") as client:
    client: UserNotificationsClient
    kwargs: CreateEventRuleRequestTypeDef = {...}
    result: CreateEventRuleResponseTypeDef = await client.create_event_rule(**kwargs)
```



```python
# ListChannelsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_notifications.client import UserNotificationsClient
from types_aiobotocore_notifications.paginator import ListChannelsPaginator
from types_aiobotocore_notifications.type_defs import ListChannelsResponseTypeDef


session = get_session()

async with session.create_client("notifications") as client:
    client: UserNotificationsClient
    paginator: ListChannelsPaginator = client.get_paginator("list_channels")
    async for item in paginator.paginate(...):
        item: ListChannelsResponseTypeDef
        print(item)
```


