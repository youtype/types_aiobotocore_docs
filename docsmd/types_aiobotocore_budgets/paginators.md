# Paginators

> [Index](../README.md) > [Budgets](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Budgets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#budgets)
    type annotations stubs module [types-aiobotocore-budgets](https://pypi.org/project/types-aiobotocore-budgets/).

## DescribeBudgetActionHistoriesPaginator

Type annotations and code completion for `#!python session.create_client("budgets").get_paginator("describe_budget_action_histories")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets/paginator/DescribeBudgetActionHistories.html#Budgets.Paginator.DescribeBudgetActionHistories)

```python
# DescribeBudgetActionHistoriesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeBudgetActionHistoriesPaginator

session = get_session()
async with session.create_client("budgets") as client:  # (1)
    paginator: DescribeBudgetActionHistoriesPaginator = client.get_paginator("describe_budget_action_histories")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeBudgetActionHistoriesResponseTypeDef
        print(item)  # (3)
```

1. client: [BudgetsClient](./client.md)
2. paginator: [DescribeBudgetActionHistoriesPaginator](./paginators.md#describebudgetactionhistoriespaginator)
3. item: [:material-code-braces: DescribeBudgetActionHistoriesResponseTypeDef](./type_defs.md#describebudgetactionhistoriesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeBudgetActionHistoriesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    ActionId: str,
    TimePeriod: TimePeriodUnionTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeBudgetActionHistoriesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: TimePeriodTypeDef](./type_defs.md#timeperiodtypedef) [:material-code-braces: TimePeriodOutputTypeDef](./type_defs.md#timeperiodoutputtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeBudgetActionHistoriesResponseTypeDef](./type_defs.md#describebudgetactionhistoriesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeBudgetActionHistoriesRequestPaginateTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
    "ActionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeBudgetActionHistoriesRequestPaginateTypeDef](./type_defs.md#describebudgetactionhistoriesrequestpaginatetypedef) 
## DescribeBudgetActionsForAccountPaginator

Type annotations and code completion for `#!python session.create_client("budgets").get_paginator("describe_budget_actions_for_account")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets/paginator/DescribeBudgetActionsForAccount.html#Budgets.Paginator.DescribeBudgetActionsForAccount)

```python
# DescribeBudgetActionsForAccountPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeBudgetActionsForAccountPaginator

session = get_session()
async with session.create_client("budgets") as client:  # (1)
    paginator: DescribeBudgetActionsForAccountPaginator = client.get_paginator("describe_budget_actions_for_account")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeBudgetActionsForAccountResponseTypeDef
        print(item)  # (3)
```

1. client: [BudgetsClient](./client.md)
2. paginator: [DescribeBudgetActionsForAccountPaginator](./paginators.md#describebudgetactionsforaccountpaginator)
3. item: [:material-code-braces: DescribeBudgetActionsForAccountResponseTypeDef](./type_defs.md#describebudgetactionsforaccountresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeBudgetActionsForAccountPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeBudgetActionsForAccountResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeBudgetActionsForAccountResponseTypeDef](./type_defs.md#describebudgetactionsforaccountresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeBudgetActionsForAccountRequestPaginateTypeDef = {  # (1)
    "AccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeBudgetActionsForAccountRequestPaginateTypeDef](./type_defs.md#describebudgetactionsforaccountrequestpaginatetypedef) 
## DescribeBudgetActionsForBudgetPaginator

Type annotations and code completion for `#!python session.create_client("budgets").get_paginator("describe_budget_actions_for_budget")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets/paginator/DescribeBudgetActionsForBudget.html#Budgets.Paginator.DescribeBudgetActionsForBudget)

```python
# DescribeBudgetActionsForBudgetPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeBudgetActionsForBudgetPaginator

session = get_session()
async with session.create_client("budgets") as client:  # (1)
    paginator: DescribeBudgetActionsForBudgetPaginator = client.get_paginator("describe_budget_actions_for_budget")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeBudgetActionsForBudgetResponseTypeDef
        print(item)  # (3)
```

1. client: [BudgetsClient](./client.md)
2. paginator: [DescribeBudgetActionsForBudgetPaginator](./paginators.md#describebudgetactionsforbudgetpaginator)
3. item: [:material-code-braces: DescribeBudgetActionsForBudgetResponseTypeDef](./type_defs.md#describebudgetactionsforbudgetresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeBudgetActionsForBudgetPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeBudgetActionsForBudgetResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeBudgetActionsForBudgetResponseTypeDef](./type_defs.md#describebudgetactionsforbudgetresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeBudgetActionsForBudgetRequestPaginateTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeBudgetActionsForBudgetRequestPaginateTypeDef](./type_defs.md#describebudgetactionsforbudgetrequestpaginatetypedef) 
## DescribeBudgetNotificationsForAccountPaginator

Type annotations and code completion for `#!python session.create_client("budgets").get_paginator("describe_budget_notifications_for_account")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets/paginator/DescribeBudgetNotificationsForAccount.html#Budgets.Paginator.DescribeBudgetNotificationsForAccount)

```python
# DescribeBudgetNotificationsForAccountPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeBudgetNotificationsForAccountPaginator

session = get_session()
async with session.create_client("budgets") as client:  # (1)
    paginator: DescribeBudgetNotificationsForAccountPaginator = client.get_paginator("describe_budget_notifications_for_account")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeBudgetNotificationsForAccountResponseTypeDef
        print(item)  # (3)
```

1. client: [BudgetsClient](./client.md)
2. paginator: [DescribeBudgetNotificationsForAccountPaginator](./paginators.md#describebudgetnotificationsforaccountpaginator)
3. item: [:material-code-braces: DescribeBudgetNotificationsForAccountResponseTypeDef](./type_defs.md#describebudgetnotificationsforaccountresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeBudgetNotificationsForAccountPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeBudgetNotificationsForAccountResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeBudgetNotificationsForAccountResponseTypeDef](./type_defs.md#describebudgetnotificationsforaccountresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeBudgetNotificationsForAccountRequestPaginateTypeDef = {  # (1)
    "AccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeBudgetNotificationsForAccountRequestPaginateTypeDef](./type_defs.md#describebudgetnotificationsforaccountrequestpaginatetypedef) 
## DescribeBudgetPerformanceHistoryPaginator

Type annotations and code completion for `#!python session.create_client("budgets").get_paginator("describe_budget_performance_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets/paginator/DescribeBudgetPerformanceHistory.html#Budgets.Paginator.DescribeBudgetPerformanceHistory)

```python
# DescribeBudgetPerformanceHistoryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeBudgetPerformanceHistoryPaginator

session = get_session()
async with session.create_client("budgets") as client:  # (1)
    paginator: DescribeBudgetPerformanceHistoryPaginator = client.get_paginator("describe_budget_performance_history")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeBudgetPerformanceHistoryResponseTypeDef
        print(item)  # (3)
```

1. client: [BudgetsClient](./client.md)
2. paginator: [DescribeBudgetPerformanceHistoryPaginator](./paginators.md#describebudgetperformancehistorypaginator)
3. item: [:material-code-braces: DescribeBudgetPerformanceHistoryResponseTypeDef](./type_defs.md#describebudgetperformancehistoryresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeBudgetPerformanceHistoryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    TimePeriod: TimePeriodUnionTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeBudgetPerformanceHistoryResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: TimePeriodTypeDef](./type_defs.md#timeperiodtypedef) [:material-code-braces: TimePeriodOutputTypeDef](./type_defs.md#timeperiodoutputtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeBudgetPerformanceHistoryResponseTypeDef](./type_defs.md#describebudgetperformancehistoryresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeBudgetPerformanceHistoryRequestPaginateTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeBudgetPerformanceHistoryRequestPaginateTypeDef](./type_defs.md#describebudgetperformancehistoryrequestpaginatetypedef) 
## DescribeBudgetsPaginator

Type annotations and code completion for `#!python session.create_client("budgets").get_paginator("describe_budgets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets/paginator/DescribeBudgets.html#Budgets.Paginator.DescribeBudgets)

```python
# DescribeBudgetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeBudgetsPaginator

session = get_session()
async with session.create_client("budgets") as client:  # (1)
    paginator: DescribeBudgetsPaginator = client.get_paginator("describe_budgets")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeBudgetsResponseTypeDef
        print(item)  # (3)
```

1. client: [BudgetsClient](./client.md)
2. paginator: [DescribeBudgetsPaginator](./paginators.md#describebudgetspaginator)
3. item: [:material-code-braces: DescribeBudgetsResponseTypeDef](./type_defs.md#describebudgetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeBudgetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeBudgetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeBudgetsResponseTypeDef](./type_defs.md#describebudgetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeBudgetsRequestPaginateTypeDef = {  # (1)
    "AccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeBudgetsRequestPaginateTypeDef](./type_defs.md#describebudgetsrequestpaginatetypedef) 
## DescribeNotificationsForBudgetPaginator

Type annotations and code completion for `#!python session.create_client("budgets").get_paginator("describe_notifications_for_budget")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets/paginator/DescribeNotificationsForBudget.html#Budgets.Paginator.DescribeNotificationsForBudget)

```python
# DescribeNotificationsForBudgetPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeNotificationsForBudgetPaginator

session = get_session()
async with session.create_client("budgets") as client:  # (1)
    paginator: DescribeNotificationsForBudgetPaginator = client.get_paginator("describe_notifications_for_budget")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeNotificationsForBudgetResponseTypeDef
        print(item)  # (3)
```

1. client: [BudgetsClient](./client.md)
2. paginator: [DescribeNotificationsForBudgetPaginator](./paginators.md#describenotificationsforbudgetpaginator)
3. item: [:material-code-braces: DescribeNotificationsForBudgetResponseTypeDef](./type_defs.md#describenotificationsforbudgetresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeNotificationsForBudgetPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeNotificationsForBudgetResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeNotificationsForBudgetResponseTypeDef](./type_defs.md#describenotificationsforbudgetresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeNotificationsForBudgetRequestPaginateTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeNotificationsForBudgetRequestPaginateTypeDef](./type_defs.md#describenotificationsforbudgetrequestpaginatetypedef) 
## DescribeSubscribersForNotificationPaginator

Type annotations and code completion for `#!python session.create_client("budgets").get_paginator("describe_subscribers_for_notification")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets/paginator/DescribeSubscribersForNotification.html#Budgets.Paginator.DescribeSubscribersForNotification)

```python
# DescribeSubscribersForNotificationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_budgets.paginator import DescribeSubscribersForNotificationPaginator

session = get_session()
async with session.create_client("budgets") as client:  # (1)
    paginator: DescribeSubscribersForNotificationPaginator = client.get_paginator("describe_subscribers_for_notification")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSubscribersForNotificationResponseTypeDef
        print(item)  # (3)
```

1. client: [BudgetsClient](./client.md)
2. paginator: [DescribeSubscribersForNotificationPaginator](./paginators.md#describesubscribersfornotificationpaginator)
3. item: [:material-code-braces: DescribeSubscribersForNotificationResponseTypeDef](./type_defs.md#describesubscribersfornotificationresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSubscribersForNotificationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    Notification: NotificationTypeDef,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeSubscribersForNotificationResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeSubscribersForNotificationResponseTypeDef](./type_defs.md#describesubscribersfornotificationresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSubscribersForNotificationRequestPaginateTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
    "Notification": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSubscribersForNotificationRequestPaginateTypeDef](./type_defs.md#describesubscribersfornotificationrequestpaginatetypedef) 
