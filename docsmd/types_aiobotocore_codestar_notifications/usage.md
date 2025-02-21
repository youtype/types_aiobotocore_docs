# Examples

> [Index](../README.md) > [CodeStarNotifications](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CodeStarNotifications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#codestarnotifications)
    type annotations stubs module [types-aiobotocore-codestar-notifications](https://pypi.org/project/types-aiobotocore-codestar-notifications/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[codestar-notifications]` package installed.

Write your `CodeStarNotifications` code as usual,
type checking and code completion should work out of the box.



```python
# CodeStarNotificationsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("codestar-notifications") as client:  # (1)
    result = await client.create_notification_rule()  # (2)
```

1. client: [CodeStarNotificationsClient](./client.md)
2. result: [:material-code-braces: CreateNotificationRuleResultTypeDef](./type_defs.md#createnotificationruleresulttypedef) 



```python
# ListEventTypesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("codestar-notifications") as client:  # (1)
    paginator = client.get_paginator("list_event_types")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CodeStarNotificationsClient](./client.md)
2. paginator: [ListEventTypesPaginator](./paginators.md#listeventtypespaginator)
3. item: [:material-code-braces: ListEventTypesResultTypeDef](./type_defs.md#listeventtypesresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[codestar-notifications]`
or a standalone `types_aiobotocore_codestar_notifications` package, you have to explicitly specify
`client: CodeStarNotificationsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CodeStarNotificationsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_codestar_notifications.client import CodeStarNotificationsClient
from types_aiobotocore_codestar_notifications.type_defs import CreateNotificationRuleResultTypeDef
from types_aiobotocore_codestar_notifications.type_defs import CreateNotificationRuleRequestTypeDef


session = get_session()

async with session.create_client("codestar-notifications") as client:
    client: CodeStarNotificationsClient
    kwargs: CreateNotificationRuleRequestTypeDef = {...}
    result: CreateNotificationRuleResultTypeDef = await client.create_notification_rule(**kwargs)
```



```python
# ListEventTypesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_codestar_notifications.client import CodeStarNotificationsClient
from types_aiobotocore_codestar_notifications.paginator import ListEventTypesPaginator
from types_aiobotocore_codestar_notifications.type_defs import ListEventTypesResultTypeDef


session = get_session()

async with session.create_client("codestar-notifications") as client:
    client: CodeStarNotificationsClient
    paginator: ListEventTypesPaginator = client.get_paginator("list_event_types")
    async for item in paginator.paginate(...):
        item: ListEventTypesResultTypeDef
        print(item)
```


