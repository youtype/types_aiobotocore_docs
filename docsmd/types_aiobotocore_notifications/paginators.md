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
3. item: `AioPageIterator[ListChannelsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListChannelsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    notificationConfigurationArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListChannelsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListChannelsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListChannelsRequestPaginateTypeDef = {  # (1)
    "notificationConfigurationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListChannelsRequestPaginateTypeDef](./type_defs.md#listchannelsrequestpaginatetypedef)
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
3. item: `AioPageIterator[ListEventRulesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListEventRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    notificationConfigurationArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListEventRulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListEventRulesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListEventRulesRequestPaginateTypeDef = {  # (1)
    "notificationConfigurationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventRulesRequestPaginateTypeDef](./type_defs.md#listeventrulesrequestpaginatetypedef)
## ListManagedNotificationChannelAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("notifications").get_paginator("list_managed_notification_channel_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/paginator/ListManagedNotificationChannelAssociations.html#UserNotifications.Paginator.ListManagedNotificationChannelAssociations)

```python
# ListManagedNotificationChannelAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_notifications.paginator import ListManagedNotificationChannelAssociationsPaginator

session = get_session()
async with session.create_client("notifications") as client:  # (1)
    paginator: ListManagedNotificationChannelAssociationsPaginator = client.get_paginator("list_managed_notification_channel_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListManagedNotificationChannelAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [UserNotificationsClient](./client.md)
2. paginator: [ListManagedNotificationChannelAssociationsPaginator](./paginators.md#listmanagednotificationchannelassociationspaginator)
3. item: `AioPageIterator[ListManagedNotificationChannelAssociationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListManagedNotificationChannelAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    managedNotificationConfigurationArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListManagedNotificationChannelAssociationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListManagedNotificationChannelAssociationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListManagedNotificationChannelAssociationsRequestPaginateTypeDef = {  # (1)
    "managedNotificationConfigurationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListManagedNotificationChannelAssociationsRequestPaginateTypeDef](./type_defs.md#listmanagednotificationchannelassociationsrequestpaginatetypedef)
## ListManagedNotificationChildEventsPaginator

Type annotations and code completion for `#!python session.create_client("notifications").get_paginator("list_managed_notification_child_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/paginator/ListManagedNotificationChildEvents.html#UserNotifications.Paginator.ListManagedNotificationChildEvents)

```python
# ListManagedNotificationChildEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_notifications.paginator import ListManagedNotificationChildEventsPaginator

session = get_session()
async with session.create_client("notifications") as client:  # (1)
    paginator: ListManagedNotificationChildEventsPaginator = client.get_paginator("list_managed_notification_child_events")  # (2)
    async for item in paginator.paginate(...):
        item: ListManagedNotificationChildEventsResponseTypeDef
        print(item)  # (3)
```

1. client: [UserNotificationsClient](./client.md)
2. paginator: [ListManagedNotificationChildEventsPaginator](./paginators.md#listmanagednotificationchildeventspaginator)
3. item: `AioPageIterator[ListManagedNotificationChildEventsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListManagedNotificationChildEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    aggregateManagedNotificationEventArn: str,
    startTime: TimestampTypeDef = ...,
    endTime: TimestampTypeDef = ...,
    locale: LocaleCodeType = ...,  # (1)
    relatedAccount: str = ...,
    organizationalUnitId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListManagedNotificationChildEventsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: LocaleCodeType](./literals.md#localecodetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListManagedNotificationChildEventsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListManagedNotificationChildEventsRequestPaginateTypeDef = {  # (1)
    "aggregateManagedNotificationEventArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListManagedNotificationChildEventsRequestPaginateTypeDef](./type_defs.md#listmanagednotificationchildeventsrequestpaginatetypedef)
## ListManagedNotificationConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("notifications").get_paginator("list_managed_notification_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/paginator/ListManagedNotificationConfigurations.html#UserNotifications.Paginator.ListManagedNotificationConfigurations)

```python
# ListManagedNotificationConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_notifications.paginator import ListManagedNotificationConfigurationsPaginator

session = get_session()
async with session.create_client("notifications") as client:  # (1)
    paginator: ListManagedNotificationConfigurationsPaginator = client.get_paginator("list_managed_notification_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListManagedNotificationConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [UserNotificationsClient](./client.md)
2. paginator: [ListManagedNotificationConfigurationsPaginator](./paginators.md#listmanagednotificationconfigurationspaginator)
3. item: `AioPageIterator[ListManagedNotificationConfigurationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListManagedNotificationConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    channelIdentifier: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListManagedNotificationConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListManagedNotificationConfigurationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListManagedNotificationConfigurationsRequestPaginateTypeDef = {  # (1)
    "channelIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListManagedNotificationConfigurationsRequestPaginateTypeDef](./type_defs.md#listmanagednotificationconfigurationsrequestpaginatetypedef)
## ListManagedNotificationEventsPaginator

Type annotations and code completion for `#!python session.create_client("notifications").get_paginator("list_managed_notification_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/paginator/ListManagedNotificationEvents.html#UserNotifications.Paginator.ListManagedNotificationEvents)

```python
# ListManagedNotificationEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_notifications.paginator import ListManagedNotificationEventsPaginator

session = get_session()
async with session.create_client("notifications") as client:  # (1)
    paginator: ListManagedNotificationEventsPaginator = client.get_paginator("list_managed_notification_events")  # (2)
    async for item in paginator.paginate(...):
        item: ListManagedNotificationEventsResponseTypeDef
        print(item)  # (3)
```

1. client: [UserNotificationsClient](./client.md)
2. paginator: [ListManagedNotificationEventsPaginator](./paginators.md#listmanagednotificationeventspaginator)
3. item: `AioPageIterator[ListManagedNotificationEventsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListManagedNotificationEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    startTime: TimestampTypeDef = ...,
    endTime: TimestampTypeDef = ...,
    locale: LocaleCodeType = ...,  # (1)
    source: str = ...,
    organizationalUnitId: str = ...,
    relatedAccount: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListManagedNotificationEventsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: LocaleCodeType](./literals.md#localecodetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListManagedNotificationEventsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListManagedNotificationEventsRequestPaginateTypeDef = {  # (1)
    "startTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListManagedNotificationEventsRequestPaginateTypeDef](./type_defs.md#listmanagednotificationeventsrequestpaginatetypedef)
## ListMemberAccountsPaginator

Type annotations and code completion for `#!python session.create_client("notifications").get_paginator("list_member_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/paginator/ListMemberAccounts.html#UserNotifications.Paginator.ListMemberAccounts)

```python
# ListMemberAccountsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_notifications.paginator import ListMemberAccountsPaginator

session = get_session()
async with session.create_client("notifications") as client:  # (1)
    paginator: ListMemberAccountsPaginator = client.get_paginator("list_member_accounts")  # (2)
    async for item in paginator.paginate(...):
        item: ListMemberAccountsResponseTypeDef
        print(item)  # (3)
```

1. client: [UserNotificationsClient](./client.md)
2. paginator: [ListMemberAccountsPaginator](./paginators.md#listmemberaccountspaginator)
3. item: `AioPageIterator[ListMemberAccountsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListMemberAccountsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    notificationConfigurationArn: str,
    memberAccount: str = ...,
    status: MemberAccountNotificationConfigurationStatusType = ...,  # (1)
    organizationalUnitId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListMemberAccountsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: MemberAccountNotificationConfigurationStatusType](./literals.md#memberaccountnotificationconfigurationstatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListMemberAccountsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListMemberAccountsRequestPaginateTypeDef = {  # (1)
    "notificationConfigurationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMemberAccountsRequestPaginateTypeDef](./type_defs.md#listmemberaccountsrequestpaginatetypedef)
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
3. item: `AioPageIterator[ListNotificationConfigurationsResponseTypeDef]`


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
    subtype: NotificationConfigurationSubtypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListNotificationConfigurationsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: NotificationConfigurationStatusType](./literals.md#notificationconfigurationstatustype)
2. See [:material-code-brackets: NotificationConfigurationSubtypeType](./literals.md#notificationconfigurationsubtypetype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListNotificationConfigurationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListNotificationConfigurationsRequestPaginateTypeDef = {  # (1)
    "eventRuleSource": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNotificationConfigurationsRequestPaginateTypeDef](./type_defs.md#listnotificationconfigurationsrequestpaginatetypedef)
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
3. item: `AioPageIterator[ListNotificationEventsResponseTypeDef]`


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
    organizationalUnitId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListNotificationEventsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: LocaleCodeType](./literals.md#localecodetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListNotificationEventsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListNotificationEventsRequestPaginateTypeDef = {  # (1)
    "startTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNotificationEventsRequestPaginateTypeDef](./type_defs.md#listnotificationeventsrequestpaginatetypedef)
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
3. item: `AioPageIterator[ListNotificationHubsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListNotificationHubsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListNotificationHubsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListNotificationHubsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListNotificationHubsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNotificationHubsRequestPaginateTypeDef](./type_defs.md#listnotificationhubsrequestpaginatetypedef)
## ListOrganizationalUnitsPaginator

Type annotations and code completion for `#!python session.create_client("notifications").get_paginator("list_organizational_units")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/paginator/ListOrganizationalUnits.html#UserNotifications.Paginator.ListOrganizationalUnits)

```python
# ListOrganizationalUnitsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_notifications.paginator import ListOrganizationalUnitsPaginator

session = get_session()
async with session.create_client("notifications") as client:  # (1)
    paginator: ListOrganizationalUnitsPaginator = client.get_paginator("list_organizational_units")  # (2)
    async for item in paginator.paginate(...):
        item: ListOrganizationalUnitsResponseTypeDef
        print(item)  # (3)
```

1. client: [UserNotificationsClient](./client.md)
2. paginator: [ListOrganizationalUnitsPaginator](./paginators.md#listorganizationalunitspaginator)
3. item: `AioPageIterator[ListOrganizationalUnitsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListOrganizationalUnitsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    notificationConfigurationArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListOrganizationalUnitsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListOrganizationalUnitsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListOrganizationalUnitsRequestPaginateTypeDef = {  # (1)
    "notificationConfigurationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOrganizationalUnitsRequestPaginateTypeDef](./type_defs.md#listorganizationalunitsrequestpaginatetypedef)
