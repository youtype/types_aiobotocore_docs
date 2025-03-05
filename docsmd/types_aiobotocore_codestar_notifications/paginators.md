# Paginators

> [Index](../README.md) > [CodeStarNotifications](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CodeStarNotifications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#codestarnotifications)
    type annotations stubs module [types-aiobotocore-codestar-notifications](https://pypi.org/project/types-aiobotocore-codestar-notifications/).

## ListEventTypesPaginator

Type annotations and code completion for `#!python session.create_client("codestar-notifications").get_paginator("list_event_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications/paginator/ListEventTypes.html#CodeStarNotifications.Paginator.ListEventTypes)

```python
# ListEventTypesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codestar_notifications.paginator import ListEventTypesPaginator

session = get_session()
async with session.create_client("codestar-notifications") as client:  # (1)
    paginator: ListEventTypesPaginator = client.get_paginator("list_event_types")  # (2)
    async for item in paginator.paginate(...):
        item: ListEventTypesResultTypeDef
        print(item)  # (3)
```

1. client: [CodeStarNotificationsClient](./client.md)
2. paginator: [ListEventTypesPaginator](./paginators.md#listeventtypespaginator)
3. item: `AioPageIterator[ListEventTypesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListEventTypesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[ListEventTypesFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListEventTypesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[ListEventTypesFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListEventTypesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListEventTypesRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventTypesRequestPaginateTypeDef](./type_defs.md#listeventtypesrequestpaginatetypedef)
## ListNotificationRulesPaginator

Type annotations and code completion for `#!python session.create_client("codestar-notifications").get_paginator("list_notification_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications/paginator/ListNotificationRules.html#CodeStarNotifications.Paginator.ListNotificationRules)

```python
# ListNotificationRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codestar_notifications.paginator import ListNotificationRulesPaginator

session = get_session()
async with session.create_client("codestar-notifications") as client:  # (1)
    paginator: ListNotificationRulesPaginator = client.get_paginator("list_notification_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListNotificationRulesResultTypeDef
        print(item)  # (3)
```

1. client: [CodeStarNotificationsClient](./client.md)
2. paginator: [ListNotificationRulesPaginator](./paginators.md#listnotificationrulespaginator)
3. item: `AioPageIterator[ListNotificationRulesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListNotificationRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[ListNotificationRulesFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListNotificationRulesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[ListNotificationRulesFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListNotificationRulesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListNotificationRulesRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNotificationRulesRequestPaginateTypeDef](./type_defs.md#listnotificationrulesrequestpaginatetypedef)
## ListTargetsPaginator

Type annotations and code completion for `#!python session.create_client("codestar-notifications").get_paginator("list_targets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications/paginator/ListTargets.html#CodeStarNotifications.Paginator.ListTargets)

```python
# ListTargetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codestar_notifications.paginator import ListTargetsPaginator

session = get_session()
async with session.create_client("codestar-notifications") as client:  # (1)
    paginator: ListTargetsPaginator = client.get_paginator("list_targets")  # (2)
    async for item in paginator.paginate(...):
        item: ListTargetsResultTypeDef
        print(item)  # (3)
```

1. client: [CodeStarNotificationsClient](./client.md)
2. paginator: [ListTargetsPaginator](./paginators.md#listtargetspaginator)
3. item: `AioPageIterator[ListTargetsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTargetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[ListTargetsFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListTargetsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[ListTargetsFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListTargetsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTargetsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTargetsRequestPaginateTypeDef](./type_defs.md#listtargetsrequestpaginatetypedef)
