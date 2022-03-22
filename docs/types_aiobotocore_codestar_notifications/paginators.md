<a id="paginators-for-aiobotocore-codestarnotifications-module"></a>

# Paginators for aiobotocore CodeStarNotifications module

> [Index](../README.md) > [CodeStarNotifications](./README.md) > Paginators

Auto-generated documentation for
[CodeStarNotifications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
type annotations stubs module
[types-aiobotocore-codestar-notifications](https://pypi.org/project/types-aiobotocore-codestar-notifications/).

- [Paginators for aiobotocore CodeStarNotifications module](#paginators-for-aiobotocore-codestarnotifications-module)
  - [ListEventTypesPaginator](#listeventtypespaginator)
  - [ListNotificationRulesPaginator](#listnotificationrulespaginator)
  - [ListTargetsPaginator](#listtargetspaginator)

<a id="listeventtypespaginator"></a>

## ListEventTypesPaginator

Type annotations for
`session.create_client("codestar-notifications").get_paginator("list_event_types")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codestar_notifications.paginator import ListEventTypesPaginator

session = get_session()
async with session.create_client("codestar-notifications") as client:
    client: CodeStarNotificationsClient
    paginator: ListEventTypesPaginator = client.get_paginator("list_event_types")
```

Boto3 documentation:
[CodeStarNotifications.Paginator.ListEventTypes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListEventTypes)

Arguments for `ListEventTypesPaginator.paginate` method:

- `Filters`:
  `Sequence`\[[ListEventTypesFilterTypeDef](./type_defs.md#listeventtypesfiltertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListEventTypesPaginator.paginate` returns
`AsyncIterator`\[[ListEventTypesResultTypeDef](./type_defs.md#listeventtypesresulttypedef)\].

<a id="listnotificationrulespaginator"></a>

## ListNotificationRulesPaginator

Type annotations for
`session.create_client("codestar-notifications").get_paginator("list_notification_rules")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codestar_notifications.paginator import ListNotificationRulesPaginator

session = get_session()
async with session.create_client("codestar-notifications") as client:
    client: CodeStarNotificationsClient
    paginator: ListNotificationRulesPaginator = client.get_paginator("list_notification_rules")
```

Boto3 documentation:
[CodeStarNotifications.Paginator.ListNotificationRules](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListNotificationRules)

Arguments for `ListNotificationRulesPaginator.paginate` method:

- `Filters`:
  `Sequence`\[[ListNotificationRulesFilterTypeDef](./type_defs.md#listnotificationrulesfiltertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListNotificationRulesPaginator.paginate` returns
`AsyncIterator`\[[ListNotificationRulesResultTypeDef](./type_defs.md#listnotificationrulesresulttypedef)\].

<a id="listtargetspaginator"></a>

## ListTargetsPaginator

Type annotations for
`session.create_client("codestar-notifications").get_paginator("list_targets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codestar_notifications.paginator import ListTargetsPaginator

session = get_session()
async with session.create_client("codestar-notifications") as client:
    client: CodeStarNotificationsClient
    paginator: ListTargetsPaginator = client.get_paginator("list_targets")
```

Boto3 documentation:
[CodeStarNotifications.Paginator.ListTargets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListTargets)

Arguments for `ListTargetsPaginator.paginate` method:

- `Filters`:
  `Sequence`\[[ListTargetsFilterTypeDef](./type_defs.md#listtargetsfiltertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTargetsPaginator.paginate` returns
`AsyncIterator`\[[ListTargetsResultTypeDef](./type_defs.md#listtargetsresulttypedef)\].
