# Paginators

> [Index](../README.md) > [UserNotifications](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [UserNotifications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications.html#usernotifications)
    type annotations stubs module [types-aiobotocore-notifications](https://pypi.org/project/types-aiobotocore-notifications/).

## ListChannelsPaginator

Type annotations and code completion for `#!python session.create_client("notifications").get_paginator("list_channels")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/paginator/ListChannels.html#UserNotifications.Paginator.ListChannels)

```python
# ListChannelsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_notifications.paginator import ListChannelsPaginator

session = get_session()
async with session.create_client("notifications") as client:  # (1)
    paginator: ListChannelsPaginator = client.get_paginator("list_channels")  # (2)
    async for item in paginator.paginate(...):
        item: ListChannelsResponseTypeDef
        print(item)  # (3)
```

1. client: [UserNotificationsClient](./client.md)
2. paginator: [ListChannelsPaginator](./paginators.md#listchannelspaginator)
3. item: [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListChannelsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    notificationConfigurationArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListChannelsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListChannelsRequestListChannelsPaginateTypeDef = {  # (1)
    "notificationConfigurationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListChannelsRequestListChannelsPaginateTypeDef](./type_defs.md#listchannelsrequestlistchannelspaginatetypedef) 
## ListEventRulesPaginator

Type annotations and code completion for `#!python session.create_client("notifications").get_paginator("list_event_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/paginator/ListEventRules.html#UserNotifications.Paginator.ListEventRules)

```python
# ListEventRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_notifications.paginator import ListEventRulesPaginator

session = get_session()
async with session.create_client("notifications") as client:  # (1)
    paginator: ListEventRulesPaginator = client.get_paginator("list_event_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListEventRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [UserNotificationsClient](./client.md)
2. paginator: [ListEventRulesPaginator](./paginators.md#listeventrulespaginator)
3. item: [:material-code-braces: ListEventRulesResponseTypeDef](./type_defs.md#listeventrulesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEventRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    notificationConfigurationArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEventRulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEventRulesResponseTypeDef](./type_defs.md#listeventrulesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEventRulesRequestListEventRulesPaginateTypeDef = {  # (1)
    "notificationConfigurationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventRulesRequestListEventRulesPaginateTypeDef](./type_defs.md#listeventrulesrequestlisteventrulespaginatetypedef) 
## ListNotificationConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("notifications").get_paginator("list_notification_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/paginator/ListNotificationConfigurations.html#UserNotifications.Paginator.ListNotificationConfigurations)

```python
# ListNotificationConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_notifications.paginator import ListNotificationConfigurationsPaginator

session = get_session()
async with session.create_client("notifications") as client:  # (1)
    paginator: ListNotificationConfigurationsPaginator = client.get_paginator("list_notification_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListNotificationConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [UserNotificationsClient](./client.md)
2. paginator: [ListNotificationConfigurationsPaginator](./paginators.md#listnotificationconfigurationspaginator)
3. item: [:material-code-braces: ListNotificationConfigurationsResponseTypeDef](./type_defs.md#listnotificationconfigurationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListNotificationConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    eventRuleSource: str = ...,
    channelArn: str = ...,
    status: NotificationConfigurationStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListNotificationConfigurationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: NotificationConfigurationStatusType](./literals.md#notificationconfigurationstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListNotificationConfigurationsResponseTypeDef](./type_defs.md#listnotificationconfigurationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListNotificationConfigurationsRequestListNotificationConfigurationsPaginateTypeDef = {  # (1)
    "eventRuleSource": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNotificationConfigurationsRequestListNotificationConfigurationsPaginateTypeDef](./type_defs.md#listnotificationconfigurationsrequestlistnotificationconfigurationspaginatetypedef) 
## ListNotificationEventsPaginator

Type annotations and code completion for `#!python session.create_client("notifications").get_paginator("list_notification_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/paginator/ListNotificationEvents.html#UserNotifications.Paginator.ListNotificationEvents)

```python
# ListNotificationEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_notifications.paginator import ListNotificationEventsPaginator

session = get_session()
async with session.create_client("notifications") as client:  # (1)
    paginator: ListNotificationEventsPaginator = client.get_paginator("list_notification_events")  # (2)
    async for item in paginator.paginate(...):
        item: ListNotificationEventsResponseTypeDef
        print(item)  # (3)
```

1. client: [UserNotificationsClient](./client.md)
2. paginator: [ListNotificationEventsPaginator](./paginators.md#listnotificationeventspaginator)
3. item: [:material-code-braces: ListNotificationEventsResponseTypeDef](./type_defs.md#listnotificationeventsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListNotificationEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    startTime: TimestampTypeDef = ...,
    endTime: TimestampTypeDef = ...,
    locale: LocaleCodeType = ...,  # (1)
    source: str = ...,
    includeChildEvents: bool = ...,
    aggregateNotificationEventArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListNotificationEventsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: LocaleCodeType](./literals.md#localecodetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListNotificationEventsResponseTypeDef](./type_defs.md#listnotificationeventsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListNotificationEventsRequestListNotificationEventsPaginateTypeDef = {  # (1)
    "startTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNotificationEventsRequestListNotificationEventsPaginateTypeDef](./type_defs.md#listnotificationeventsrequestlistnotificationeventspaginatetypedef) 
## ListNotificationHubsPaginator

Type annotations and code completion for `#!python session.create_client("notifications").get_paginator("list_notification_hubs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/paginator/ListNotificationHubs.html#UserNotifications.Paginator.ListNotificationHubs)

```python
# ListNotificationHubsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_notifications.paginator import ListNotificationHubsPaginator

session = get_session()
async with session.create_client("notifications") as client:  # (1)
    paginator: ListNotificationHubsPaginator = client.get_paginator("list_notification_hubs")  # (2)
    async for item in paginator.paginate(...):
        item: ListNotificationHubsResponseTypeDef
        print(item)  # (3)
```

1. client: [UserNotificationsClient](./client.md)
2. paginator: [ListNotificationHubsPaginator](./paginators.md#listnotificationhubspaginator)
3. item: [:material-code-braces: ListNotificationHubsResponseTypeDef](./type_defs.md#listnotificationhubsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListNotificationHubsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListNotificationHubsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListNotificationHubsResponseTypeDef](./type_defs.md#listnotificationhubsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListNotificationHubsRequestListNotificationHubsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNotificationHubsRequestListNotificationHubsPaginateTypeDef](./type_defs.md#listnotificationhubsrequestlistnotificationhubspaginatetypedef) 
