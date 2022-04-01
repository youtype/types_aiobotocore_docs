# Paginators

> [Index](../README.md) > [Budgets](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Budgets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
    type annotations stubs module [types-aiobotocore-budgets](https://pypi.org/project/types-aiobotocore-budgets/).

## DescribeBudgetActionHistoriesPaginator

Type annotations and code completion for `#!python session.create_client("budgets").get_paginator("describe_budget_action_histories")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionHistories)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeBudgetActionHistoriesPaginator

session = get_session()
async with session.create_client("budgets") as client:
    client: BudgetsClient
    paginator: DescribeBudgetActionHistoriesPaginator = client.get_paginator("describe_budget_action_histories")
```


### paginate

Type annotations and code completion for `#!python DescribeBudgetActionHistoriesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    ActionId: str,
    TimePeriod: TimePeriodTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeBudgetActionHistoriesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: TimePeriodTypeDef](./type_defs.md#timeperiodtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeBudgetActionHistoriesResponseTypeDef](./type_defs.md#describebudgetactionhistoriesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
    "ActionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef](./type_defs.md#describebudgetactionhistoriesrequestdescribebudgetactionhistoriespaginatetypedef) 
## DescribeBudgetActionsForAccountPaginator

Type annotations and code completion for `#!python session.create_client("budgets").get_paginator("describe_budget_actions_for_account")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForAccount)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeBudgetActionsForAccountPaginator

session = get_session()
async with session.create_client("budgets") as client:
    client: BudgetsClient
    paginator: DescribeBudgetActionsForAccountPaginator = client.get_paginator("describe_budget_actions_for_account")
```


### paginate

Type annotations and code completion for `#!python DescribeBudgetActionsForAccountPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeBudgetActionsForAccountResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeBudgetActionsForAccountResponseTypeDef](./type_defs.md#describebudgetactionsforaccountresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef = {  # (1)
    "AccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef](./type_defs.md#describebudgetactionsforaccountrequestdescribebudgetactionsforaccountpaginatetypedef) 
## DescribeBudgetActionsForBudgetPaginator

Type annotations and code completion for `#!python session.create_client("budgets").get_paginator("describe_budget_actions_for_budget")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForBudget)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeBudgetActionsForBudgetPaginator

session = get_session()
async with session.create_client("budgets") as client:
    client: BudgetsClient
    paginator: DescribeBudgetActionsForBudgetPaginator = client.get_paginator("describe_budget_actions_for_budget")
```


### paginate

Type annotations and code completion for `#!python DescribeBudgetActionsForBudgetPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeBudgetActionsForBudgetResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeBudgetActionsForBudgetResponseTypeDef](./type_defs.md#describebudgetactionsforbudgetresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef](./type_defs.md#describebudgetactionsforbudgetrequestdescribebudgetactionsforbudgetpaginatetypedef) 
## DescribeBudgetNotificationsForAccountPaginator

Type annotations and code completion for `#!python session.create_client("budgets").get_paginator("describe_budget_notifications_for_account")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetNotificationsForAccount)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeBudgetNotificationsForAccountPaginator

session = get_session()
async with session.create_client("budgets") as client:
    client: BudgetsClient
    paginator: DescribeBudgetNotificationsForAccountPaginator = client.get_paginator("describe_budget_notifications_for_account")
```


### paginate

Type annotations and code completion for `#!python DescribeBudgetNotificationsForAccountPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeBudgetNotificationsForAccountResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeBudgetNotificationsForAccountResponseTypeDef](./type_defs.md#describebudgetnotificationsforaccountresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef = {  # (1)
    "AccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef](./type_defs.md#describebudgetnotificationsforaccountrequestdescribebudgetnotificationsforaccountpaginatetypedef) 
## DescribeBudgetPerformanceHistoryPaginator

Type annotations and code completion for `#!python session.create_client("budgets").get_paginator("describe_budget_performance_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetPerformanceHistory)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeBudgetPerformanceHistoryPaginator

session = get_session()
async with session.create_client("budgets") as client:
    client: BudgetsClient
    paginator: DescribeBudgetPerformanceHistoryPaginator = client.get_paginator("describe_budget_performance_history")
```


### paginate

Type annotations and code completion for `#!python DescribeBudgetPerformanceHistoryPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    TimePeriod: TimePeriodTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeBudgetPerformanceHistoryResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: TimePeriodTypeDef](./type_defs.md#timeperiodtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeBudgetPerformanceHistoryResponseTypeDef](./type_defs.md#describebudgetperformancehistoryresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef](./type_defs.md#describebudgetperformancehistoryrequestdescribebudgetperformancehistorypaginatetypedef) 
## DescribeBudgetsPaginator

Type annotations and code completion for `#!python session.create_client("budgets").get_paginator("describe_budgets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgets)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeBudgetsPaginator

session = get_session()
async with session.create_client("budgets") as client:
    client: BudgetsClient
    paginator: DescribeBudgetsPaginator = client.get_paginator("describe_budgets")
```


### paginate

Type annotations and code completion for `#!python DescribeBudgetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeBudgetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeBudgetsResponseTypeDef](./type_defs.md#describebudgetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef = {  # (1)
    "AccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef](./type_defs.md#describebudgetsrequestdescribebudgetspaginatetypedef) 
## DescribeNotificationsForBudgetPaginator

Type annotations and code completion for `#!python session.create_client("budgets").get_paginator("describe_notifications_for_budget")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeNotificationsForBudget)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeNotificationsForBudgetPaginator

session = get_session()
async with session.create_client("budgets") as client:
    client: BudgetsClient
    paginator: DescribeNotificationsForBudgetPaginator = client.get_paginator("describe_notifications_for_budget")
```


### paginate

Type annotations and code completion for `#!python DescribeNotificationsForBudgetPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeNotificationsForBudgetResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeNotificationsForBudgetResponseTypeDef](./type_defs.md#describenotificationsforbudgetresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef](./type_defs.md#describenotificationsforbudgetrequestdescribenotificationsforbudgetpaginatetypedef) 
## DescribeSubscribersForNotificationPaginator

Type annotations and code completion for `#!python session.create_client("budgets").get_paginator("describe_subscribers_for_notification")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeSubscribersForNotification)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeSubscribersForNotificationPaginator

session = get_session()
async with session.create_client("budgets") as client:
    client: BudgetsClient
    paginator: DescribeSubscribersForNotificationPaginator = client.get_paginator("describe_subscribers_for_notification")
```


### paginate

Type annotations and code completion for `#!python DescribeSubscribersForNotificationPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    Notification: NotificationTypeDef,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeSubscribersForNotificationResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeSubscribersForNotificationResponseTypeDef](./type_defs.md#describesubscribersfornotificationresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
    "Notification": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef](./type_defs.md#describesubscribersfornotificationrequestdescribesubscribersfornotificationpaginatetypedef) 
