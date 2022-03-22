<a id="paginators-for-aiobotocore-budgets-module"></a>

# Paginators for aiobotocore Budgets module

> [Index](../README.md) > [Budgets](./README.md) > Paginators

Auto-generated documentation for
[Budgets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
type annotations stubs module
[types-aiobotocore-budgets](https://pypi.org/project/types-aiobotocore-budgets/).

- [Paginators for aiobotocore Budgets module](#paginators-for-aiobotocore-budgets-module)
  - [DescribeBudgetActionHistoriesPaginator](#describebudgetactionhistoriespaginator)
  - [DescribeBudgetActionsForAccountPaginator](#describebudgetactionsforaccountpaginator)
  - [DescribeBudgetActionsForBudgetPaginator](#describebudgetactionsforbudgetpaginator)
  - [DescribeBudgetNotificationsForAccountPaginator](#describebudgetnotificationsforaccountpaginator)
  - [DescribeBudgetPerformanceHistoryPaginator](#describebudgetperformancehistorypaginator)
  - [DescribeBudgetsPaginator](#describebudgetspaginator)
  - [DescribeNotificationsForBudgetPaginator](#describenotificationsforbudgetpaginator)
  - [DescribeSubscribersForNotificationPaginator](#describesubscribersfornotificationpaginator)

<a id="describebudgetactionhistoriespaginator"></a>

## DescribeBudgetActionHistoriesPaginator

Type annotations for
`session.create_client("budgets").get_paginator("describe_budget_action_histories")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeBudgetActionHistoriesPaginator

session = get_session()
async with session.create_client("budgets") as client:
    client: BudgetsClient
    paginator: DescribeBudgetActionHistoriesPaginator = client.get_paginator("describe_budget_action_histories")
```

Boto3 documentation:
[Budgets.Paginator.DescribeBudgetActionHistories](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionHistories)

Arguments for `DescribeBudgetActionHistoriesPaginator.paginate` method:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*
- `ActionId`: `str` *(required)*
- `TimePeriod`: [TimePeriodTypeDef](./type_defs.md#timeperiodtypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeBudgetActionHistoriesPaginator.paginate` returns
`AsyncIterator`\[[DescribeBudgetActionHistoriesResponseTypeDef](./type_defs.md#describebudgetactionhistoriesresponsetypedef)\].

<a id="describebudgetactionsforaccountpaginator"></a>

## DescribeBudgetActionsForAccountPaginator

Type annotations for
`session.create_client("budgets").get_paginator("describe_budget_actions_for_account")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeBudgetActionsForAccountPaginator

session = get_session()
async with session.create_client("budgets") as client:
    client: BudgetsClient
    paginator: DescribeBudgetActionsForAccountPaginator = client.get_paginator("describe_budget_actions_for_account")
```

Boto3 documentation:
[Budgets.Paginator.DescribeBudgetActionsForAccount](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForAccount)

Arguments for `DescribeBudgetActionsForAccountPaginator.paginate` method:

- `AccountId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeBudgetActionsForAccountPaginator.paginate` returns
`AsyncIterator`\[[DescribeBudgetActionsForAccountResponseTypeDef](./type_defs.md#describebudgetactionsforaccountresponsetypedef)\].

<a id="describebudgetactionsforbudgetpaginator"></a>

## DescribeBudgetActionsForBudgetPaginator

Type annotations for
`session.create_client("budgets").get_paginator("describe_budget_actions_for_budget")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeBudgetActionsForBudgetPaginator

session = get_session()
async with session.create_client("budgets") as client:
    client: BudgetsClient
    paginator: DescribeBudgetActionsForBudgetPaginator = client.get_paginator("describe_budget_actions_for_budget")
```

Boto3 documentation:
[Budgets.Paginator.DescribeBudgetActionsForBudget](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForBudget)

Arguments for `DescribeBudgetActionsForBudgetPaginator.paginate` method:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeBudgetActionsForBudgetPaginator.paginate` returns
`AsyncIterator`\[[DescribeBudgetActionsForBudgetResponseTypeDef](./type_defs.md#describebudgetactionsforbudgetresponsetypedef)\].

<a id="describebudgetnotificationsforaccountpaginator"></a>

## DescribeBudgetNotificationsForAccountPaginator

Type annotations for
`session.create_client("budgets").get_paginator("describe_budget_notifications_for_account")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeBudgetNotificationsForAccountPaginator

session = get_session()
async with session.create_client("budgets") as client:
    client: BudgetsClient
    paginator: DescribeBudgetNotificationsForAccountPaginator = client.get_paginator("describe_budget_notifications_for_account")
```

Boto3 documentation:
[Budgets.Paginator.DescribeBudgetNotificationsForAccount](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetNotificationsForAccount)

Arguments for `DescribeBudgetNotificationsForAccountPaginator.paginate` method:

- `AccountId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeBudgetNotificationsForAccountPaginator.paginate` returns
`AsyncIterator`\[[DescribeBudgetNotificationsForAccountResponseTypeDef](./type_defs.md#describebudgetnotificationsforaccountresponsetypedef)\].

<a id="describebudgetperformancehistorypaginator"></a>

## DescribeBudgetPerformanceHistoryPaginator

Type annotations for
`session.create_client("budgets").get_paginator("describe_budget_performance_history")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeBudgetPerformanceHistoryPaginator

session = get_session()
async with session.create_client("budgets") as client:
    client: BudgetsClient
    paginator: DescribeBudgetPerformanceHistoryPaginator = client.get_paginator("describe_budget_performance_history")
```

Boto3 documentation:
[Budgets.Paginator.DescribeBudgetPerformanceHistory](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetPerformanceHistory)

Arguments for `DescribeBudgetPerformanceHistoryPaginator.paginate` method:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*
- `TimePeriod`: [TimePeriodTypeDef](./type_defs.md#timeperiodtypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeBudgetPerformanceHistoryPaginator.paginate` returns
`AsyncIterator`\[[DescribeBudgetPerformanceHistoryResponseTypeDef](./type_defs.md#describebudgetperformancehistoryresponsetypedef)\].

<a id="describebudgetspaginator"></a>

## DescribeBudgetsPaginator

Type annotations for
`session.create_client("budgets").get_paginator("describe_budgets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeBudgetsPaginator

session = get_session()
async with session.create_client("budgets") as client:
    client: BudgetsClient
    paginator: DescribeBudgetsPaginator = client.get_paginator("describe_budgets")
```

Boto3 documentation:
[Budgets.Paginator.DescribeBudgets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgets)

Arguments for `DescribeBudgetsPaginator.paginate` method:

- `AccountId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeBudgetsPaginator.paginate` returns
`AsyncIterator`\[[DescribeBudgetsResponseTypeDef](./type_defs.md#describebudgetsresponsetypedef)\].

<a id="describenotificationsforbudgetpaginator"></a>

## DescribeNotificationsForBudgetPaginator

Type annotations for
`session.create_client("budgets").get_paginator("describe_notifications_for_budget")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeNotificationsForBudgetPaginator

session = get_session()
async with session.create_client("budgets") as client:
    client: BudgetsClient
    paginator: DescribeNotificationsForBudgetPaginator = client.get_paginator("describe_notifications_for_budget")
```

Boto3 documentation:
[Budgets.Paginator.DescribeNotificationsForBudget](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeNotificationsForBudget)

Arguments for `DescribeNotificationsForBudgetPaginator.paginate` method:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeNotificationsForBudgetPaginator.paginate` returns
`AsyncIterator`\[[DescribeNotificationsForBudgetResponseTypeDef](./type_defs.md#describenotificationsforbudgetresponsetypedef)\].

<a id="describesubscribersfornotificationpaginator"></a>

## DescribeSubscribersForNotificationPaginator

Type annotations for
`session.create_client("budgets").get_paginator("describe_subscribers_for_notification")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeSubscribersForNotificationPaginator

session = get_session()
async with session.create_client("budgets") as client:
    client: BudgetsClient
    paginator: DescribeSubscribersForNotificationPaginator = client.get_paginator("describe_subscribers_for_notification")
```

Boto3 documentation:
[Budgets.Paginator.DescribeSubscribersForNotification](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeSubscribersForNotification)

Arguments for `DescribeSubscribersForNotificationPaginator.paginate` method:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*
- `Notification`: [NotificationTypeDef](./type_defs.md#notificationtypedef)
  *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeSubscribersForNotificationPaginator.paginate` returns
`AsyncIterator`\[[DescribeSubscribersForNotificationResponseTypeDef](./type_defs.md#describesubscribersfornotificationresponsetypedef)\].
