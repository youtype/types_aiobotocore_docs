# BudgetsClient

> [Index](../README.md) > [Budgets](./README.md) > BudgetsClient

!!! note ""

    Auto-generated documentation for [Budgets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
    type annotations stubs module [types-aiobotocore-budgets](https://pypi.org/project/types-aiobotocore-budgets/).

## BudgetsClient

Type annotations and code completion for `#!python session.create_client("budgets")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client)

```python
# BudgetsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_budgets.client import BudgetsClient

session = get_session()
async with session.create_client("budgets") as client:
    client: BudgetsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("budgets").exceptions` structure.

```python
# BudgetsClient.exceptions usage example

async with session.create_client("budgets") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.CreationLimitExceededException,
        client.DuplicateRecordException,
        client.ExpiredNextTokenException,
        client.InternalErrorException,
        client.InvalidNextTokenException,
        client.InvalidParameterException,
        client.NotFoundException,
        client.ResourceLockedException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
    ) as e:
        print(e)
```

```python
# BudgetsClient usage type checking example

from types_aiobotocore_budgets.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("budgets").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("budgets").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_budget

Creates a budget and, if included, notifications and subscribers.

Type annotations and code completion for `#!python session.create_client("budgets").create_budget` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_budget)

```python
# create_budget method definition

await def create_budget(
    self,
    *,
    AccountId: str,
    Budget: BudgetTypeDef,  # (1)
    NotificationsWithSubscribers: Sequence[NotificationWithSubscribersTypeDef] = ...,  # (2)
    ResourceTags: Sequence[ResourceTagTypeDef] = ...,  # (3)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: BudgetTypeDef](./type_defs.md#budgettypedef) 
2. See [:material-code-braces: NotificationWithSubscribersTypeDef](./type_defs.md#notificationwithsubscriberstypedef) 
3. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 


```python
# create_budget method usage example with argument unpacking

kwargs: CreateBudgetRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Budget": ...,
}

parent.create_budget(**kwargs)
```

1. See [:material-code-braces: CreateBudgetRequestRequestTypeDef](./type_defs.md#createbudgetrequestrequesttypedef) 

### create\_budget\_action

Creates a budget action.

Type annotations and code completion for `#!python session.create_client("budgets").create_budget_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_budget_action)

```python
# create_budget_action method definition

await def create_budget_action(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    NotificationType: NotificationTypeType,  # (1)
    ActionType: ActionTypeType,  # (2)
    ActionThreshold: ActionThresholdTypeDef,  # (3)
    Definition: DefinitionTypeDef,  # (4)
    ExecutionRoleArn: str,
    ApprovalModel: ApprovalModelType,  # (5)
    Subscribers: Sequence[SubscriberTypeDef],  # (6)
    ResourceTags: Sequence[ResourceTagTypeDef] = ...,  # (7)
) -> CreateBudgetActionResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
2. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
3. See [:material-code-braces: ActionThresholdTypeDef](./type_defs.md#actionthresholdtypedef) 
4. See [:material-code-braces: DefinitionTypeDef](./type_defs.md#definitiontypedef) 
5. See [:material-code-brackets: ApprovalModelType](./literals.md#approvalmodeltype) 
6. See [:material-code-braces: SubscriberTypeDef](./type_defs.md#subscribertypedef) 
7. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
8. See [:material-code-braces: CreateBudgetActionResponseTypeDef](./type_defs.md#createbudgetactionresponsetypedef) 


```python
# create_budget_action method usage example with argument unpacking

kwargs: CreateBudgetActionRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
    "NotificationType": ...,
    "ActionType": ...,
    "ActionThreshold": ...,
    "Definition": ...,
    "ExecutionRoleArn": ...,
    "ApprovalModel": ...,
    "Subscribers": ...,
}

parent.create_budget_action(**kwargs)
```

1. See [:material-code-braces: CreateBudgetActionRequestRequestTypeDef](./type_defs.md#createbudgetactionrequestrequesttypedef) 

### create\_notification

Creates a notification.

Type annotations and code completion for `#!python session.create_client("budgets").create_notification` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_notification)

```python
# create_notification method definition

await def create_notification(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    Notification: NotificationTypeDef,  # (1)
    Subscribers: Sequence[SubscriberTypeDef],  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
2. See [:material-code-braces: SubscriberTypeDef](./type_defs.md#subscribertypedef) 


```python
# create_notification method usage example with argument unpacking

kwargs: CreateNotificationRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
    "Notification": ...,
    "Subscribers": ...,
}

parent.create_notification(**kwargs)
```

1. See [:material-code-braces: CreateNotificationRequestRequestTypeDef](./type_defs.md#createnotificationrequestrequesttypedef) 

### create\_subscriber

Creates a subscriber.

Type annotations and code completion for `#!python session.create_client("budgets").create_subscriber` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_subscriber)

```python
# create_subscriber method definition

await def create_subscriber(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    Notification: NotificationTypeDef,  # (1)
    Subscriber: SubscriberTypeDef,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
2. See [:material-code-braces: SubscriberTypeDef](./type_defs.md#subscribertypedef) 


```python
# create_subscriber method usage example with argument unpacking

kwargs: CreateSubscriberRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
    "Notification": ...,
    "Subscriber": ...,
}

parent.create_subscriber(**kwargs)
```

1. See [:material-code-braces: CreateSubscriberRequestRequestTypeDef](./type_defs.md#createsubscriberrequestrequesttypedef) 

### delete\_budget

Deletes a budget.

Type annotations and code completion for `#!python session.create_client("budgets").delete_budget` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.delete_budget)

```python
# delete_budget method definition

await def delete_budget(
    self,
    *,
    AccountId: str,
    BudgetName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_budget method usage example with argument unpacking

kwargs: DeleteBudgetRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
}

parent.delete_budget(**kwargs)
```

1. See [:material-code-braces: DeleteBudgetRequestRequestTypeDef](./type_defs.md#deletebudgetrequestrequesttypedef) 

### delete\_budget\_action

Deletes a budget action.

Type annotations and code completion for `#!python session.create_client("budgets").delete_budget_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.delete_budget_action)

```python
# delete_budget_action method definition

await def delete_budget_action(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    ActionId: str,
) -> DeleteBudgetActionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteBudgetActionResponseTypeDef](./type_defs.md#deletebudgetactionresponsetypedef) 


```python
# delete_budget_action method usage example with argument unpacking

kwargs: DeleteBudgetActionRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
    "ActionId": ...,
}

parent.delete_budget_action(**kwargs)
```

1. See [:material-code-braces: DeleteBudgetActionRequestRequestTypeDef](./type_defs.md#deletebudgetactionrequestrequesttypedef) 

### delete\_notification

Deletes a notification.

Type annotations and code completion for `#!python session.create_client("budgets").delete_notification` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.delete_notification)

```python
# delete_notification method definition

await def delete_notification(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    Notification: NotificationTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 


```python
# delete_notification method usage example with argument unpacking

kwargs: DeleteNotificationRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
    "Notification": ...,
}

parent.delete_notification(**kwargs)
```

1. See [:material-code-braces: DeleteNotificationRequestRequestTypeDef](./type_defs.md#deletenotificationrequestrequesttypedef) 

### delete\_subscriber

Deletes a subscriber.

Type annotations and code completion for `#!python session.create_client("budgets").delete_subscriber` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.delete_subscriber)

```python
# delete_subscriber method definition

await def delete_subscriber(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    Notification: NotificationTypeDef,  # (1)
    Subscriber: SubscriberTypeDef,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
2. See [:material-code-braces: SubscriberTypeDef](./type_defs.md#subscribertypedef) 


```python
# delete_subscriber method usage example with argument unpacking

kwargs: DeleteSubscriberRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
    "Notification": ...,
    "Subscriber": ...,
}

parent.delete_subscriber(**kwargs)
```

1. See [:material-code-braces: DeleteSubscriberRequestRequestTypeDef](./type_defs.md#deletesubscriberrequestrequesttypedef) 

### describe\_budget

Describes a budget.

Type annotations and code completion for `#!python session.create_client("budgets").describe_budget` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget)

```python
# describe_budget method definition

await def describe_budget(
    self,
    *,
    AccountId: str,
    BudgetName: str,
) -> DescribeBudgetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBudgetResponseTypeDef](./type_defs.md#describebudgetresponsetypedef) 


```python
# describe_budget method usage example with argument unpacking

kwargs: DescribeBudgetRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
}

parent.describe_budget(**kwargs)
```

1. See [:material-code-braces: DescribeBudgetRequestRequestTypeDef](./type_defs.md#describebudgetrequestrequesttypedef) 

### describe\_budget\_action

Describes a budget action detail.

Type annotations and code completion for `#!python session.create_client("budgets").describe_budget_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_action)

```python
# describe_budget_action method definition

await def describe_budget_action(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    ActionId: str,
) -> DescribeBudgetActionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBudgetActionResponseTypeDef](./type_defs.md#describebudgetactionresponsetypedef) 


```python
# describe_budget_action method usage example with argument unpacking

kwargs: DescribeBudgetActionRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
    "ActionId": ...,
}

parent.describe_budget_action(**kwargs)
```

1. See [:material-code-braces: DescribeBudgetActionRequestRequestTypeDef](./type_defs.md#describebudgetactionrequestrequesttypedef) 

### describe\_budget\_action\_histories

Describes a budget action history detail.

Type annotations and code completion for `#!python session.create_client("budgets").describe_budget_action_histories` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_action_histories)

```python
# describe_budget_action_histories method definition

await def describe_budget_action_histories(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    ActionId: str,
    TimePeriod: TimePeriodTypeDef = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeBudgetActionHistoriesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TimePeriodTypeDef](./type_defs.md#timeperiodtypedef) 
2. See [:material-code-braces: DescribeBudgetActionHistoriesResponseTypeDef](./type_defs.md#describebudgetactionhistoriesresponsetypedef) 


```python
# describe_budget_action_histories method usage example with argument unpacking

kwargs: DescribeBudgetActionHistoriesRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
    "ActionId": ...,
}

parent.describe_budget_action_histories(**kwargs)
```

1. See [:material-code-braces: DescribeBudgetActionHistoriesRequestRequestTypeDef](./type_defs.md#describebudgetactionhistoriesrequestrequesttypedef) 

### describe\_budget\_actions\_for\_account

Describes all of the budget actions for an account.

Type annotations and code completion for `#!python session.create_client("budgets").describe_budget_actions_for_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_actions_for_account)

```python
# describe_budget_actions_for_account method definition

await def describe_budget_actions_for_account(
    self,
    *,
    AccountId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeBudgetActionsForAccountResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBudgetActionsForAccountResponseTypeDef](./type_defs.md#describebudgetactionsforaccountresponsetypedef) 


```python
# describe_budget_actions_for_account method usage example with argument unpacking

kwargs: DescribeBudgetActionsForAccountRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.describe_budget_actions_for_account(**kwargs)
```

1. See [:material-code-braces: DescribeBudgetActionsForAccountRequestRequestTypeDef](./type_defs.md#describebudgetactionsforaccountrequestrequesttypedef) 

### describe\_budget\_actions\_for\_budget

Describes all of the budget actions for a budget.

Type annotations and code completion for `#!python session.create_client("budgets").describe_budget_actions_for_budget` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_actions_for_budget)

```python
# describe_budget_actions_for_budget method definition

await def describe_budget_actions_for_budget(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeBudgetActionsForBudgetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBudgetActionsForBudgetResponseTypeDef](./type_defs.md#describebudgetactionsforbudgetresponsetypedef) 


```python
# describe_budget_actions_for_budget method usage example with argument unpacking

kwargs: DescribeBudgetActionsForBudgetRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
}

parent.describe_budget_actions_for_budget(**kwargs)
```

1. See [:material-code-braces: DescribeBudgetActionsForBudgetRequestRequestTypeDef](./type_defs.md#describebudgetactionsforbudgetrequestrequesttypedef) 

### describe\_budget\_notifications\_for\_account

Lists the budget names and notifications that are associated with an account.

Type annotations and code completion for `#!python session.create_client("budgets").describe_budget_notifications_for_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_notifications_for_account)

```python
# describe_budget_notifications_for_account method definition

await def describe_budget_notifications_for_account(
    self,
    *,
    AccountId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeBudgetNotificationsForAccountResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBudgetNotificationsForAccountResponseTypeDef](./type_defs.md#describebudgetnotificationsforaccountresponsetypedef) 


```python
# describe_budget_notifications_for_account method usage example with argument unpacking

kwargs: DescribeBudgetNotificationsForAccountRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.describe_budget_notifications_for_account(**kwargs)
```

1. See [:material-code-braces: DescribeBudgetNotificationsForAccountRequestRequestTypeDef](./type_defs.md#describebudgetnotificationsforaccountrequestrequesttypedef) 

### describe\_budget\_performance\_history

Describes the history for `DAILY`, `MONTHLY`, and `QUARTERLY` budgets.

Type annotations and code completion for `#!python session.create_client("budgets").describe_budget_performance_history` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_performance_history)

```python
# describe_budget_performance_history method definition

await def describe_budget_performance_history(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    TimePeriod: TimePeriodTypeDef = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeBudgetPerformanceHistoryResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TimePeriodTypeDef](./type_defs.md#timeperiodtypedef) 
2. See [:material-code-braces: DescribeBudgetPerformanceHistoryResponseTypeDef](./type_defs.md#describebudgetperformancehistoryresponsetypedef) 


```python
# describe_budget_performance_history method usage example with argument unpacking

kwargs: DescribeBudgetPerformanceHistoryRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
}

parent.describe_budget_performance_history(**kwargs)
```

1. See [:material-code-braces: DescribeBudgetPerformanceHistoryRequestRequestTypeDef](./type_defs.md#describebudgetperformancehistoryrequestrequesttypedef) 

### describe\_budgets

Lists the budgets that are associated with an account.

Type annotations and code completion for `#!python session.create_client("budgets").describe_budgets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budgets)

```python
# describe_budgets method definition

await def describe_budgets(
    self,
    *,
    AccountId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeBudgetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBudgetsResponseTypeDef](./type_defs.md#describebudgetsresponsetypedef) 


```python
# describe_budgets method usage example with argument unpacking

kwargs: DescribeBudgetsRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.describe_budgets(**kwargs)
```

1. See [:material-code-braces: DescribeBudgetsRequestRequestTypeDef](./type_defs.md#describebudgetsrequestrequesttypedef) 

### describe\_notifications\_for\_budget

Lists the notifications that are associated with a budget.

Type annotations and code completion for `#!python session.create_client("budgets").describe_notifications_for_budget` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_notifications_for_budget)

```python
# describe_notifications_for_budget method definition

await def describe_notifications_for_budget(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeNotificationsForBudgetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeNotificationsForBudgetResponseTypeDef](./type_defs.md#describenotificationsforbudgetresponsetypedef) 


```python
# describe_notifications_for_budget method usage example with argument unpacking

kwargs: DescribeNotificationsForBudgetRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
}

parent.describe_notifications_for_budget(**kwargs)
```

1. See [:material-code-braces: DescribeNotificationsForBudgetRequestRequestTypeDef](./type_defs.md#describenotificationsforbudgetrequestrequesttypedef) 

### describe\_subscribers\_for\_notification

Lists the subscribers that are associated with a notification.

Type annotations and code completion for `#!python session.create_client("budgets").describe_subscribers_for_notification` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_subscribers_for_notification)

```python
# describe_subscribers_for_notification method definition

await def describe_subscribers_for_notification(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    Notification: NotificationTypeDef,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeSubscribersForNotificationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
2. See [:material-code-braces: DescribeSubscribersForNotificationResponseTypeDef](./type_defs.md#describesubscribersfornotificationresponsetypedef) 


```python
# describe_subscribers_for_notification method usage example with argument unpacking

kwargs: DescribeSubscribersForNotificationRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
    "Notification": ...,
}

parent.describe_subscribers_for_notification(**kwargs)
```

1. See [:material-code-braces: DescribeSubscribersForNotificationRequestRequestTypeDef](./type_defs.md#describesubscribersfornotificationrequestrequesttypedef) 

### execute\_budget\_action

Executes a budget action.

Type annotations and code completion for `#!python session.create_client("budgets").execute_budget_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.execute_budget_action)

```python
# execute_budget_action method definition

await def execute_budget_action(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    ActionId: str,
    ExecutionType: ExecutionTypeType,  # (1)
) -> ExecuteBudgetActionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ExecutionTypeType](./literals.md#executiontypetype) 
2. See [:material-code-braces: ExecuteBudgetActionResponseTypeDef](./type_defs.md#executebudgetactionresponsetypedef) 


```python
# execute_budget_action method usage example with argument unpacking

kwargs: ExecuteBudgetActionRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
    "ActionId": ...,
    "ExecutionType": ...,
}

parent.execute_budget_action(**kwargs)
```

1. See [:material-code-braces: ExecuteBudgetActionRequestRequestTypeDef](./type_defs.md#executebudgetactionrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("budgets").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.generate_presigned_url)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### list\_tags\_for\_resource

Lists tags associated with a budget or budget action resource.

Type annotations and code completion for `#!python session.create_client("budgets").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### tag\_resource

Creates tags for a budget or budget action resource.

Type annotations and code completion for `#!python session.create_client("budgets").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceARN: str,
    ResourceTags: Sequence[ResourceTagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "ResourceTags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Deletes tags associated with a budget or budget action resource.

Type annotations and code completion for `#!python session.create_client("budgets").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceARN: str,
    ResourceTagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "ResourceTagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_budget

Updates a budget.

Type annotations and code completion for `#!python session.create_client("budgets").update_budget` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_budget)

```python
# update_budget method definition

await def update_budget(
    self,
    *,
    AccountId: str,
    NewBudget: BudgetTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: BudgetTypeDef](./type_defs.md#budgettypedef) 


```python
# update_budget method usage example with argument unpacking

kwargs: UpdateBudgetRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "NewBudget": ...,
}

parent.update_budget(**kwargs)
```

1. See [:material-code-braces: UpdateBudgetRequestRequestTypeDef](./type_defs.md#updatebudgetrequestrequesttypedef) 

### update\_budget\_action

Updates a budget action.

Type annotations and code completion for `#!python session.create_client("budgets").update_budget_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_budget_action)

```python
# update_budget_action method definition

await def update_budget_action(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    ActionId: str,
    NotificationType: NotificationTypeType = ...,  # (1)
    ActionThreshold: ActionThresholdTypeDef = ...,  # (2)
    Definition: DefinitionTypeDef = ...,  # (3)
    ExecutionRoleArn: str = ...,
    ApprovalModel: ApprovalModelType = ...,  # (4)
    Subscribers: Sequence[SubscriberTypeDef] = ...,  # (5)
) -> UpdateBudgetActionResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
2. See [:material-code-braces: ActionThresholdTypeDef](./type_defs.md#actionthresholdtypedef) 
3. See [:material-code-braces: DefinitionTypeDef](./type_defs.md#definitiontypedef) 
4. See [:material-code-brackets: ApprovalModelType](./literals.md#approvalmodeltype) 
5. See [:material-code-braces: SubscriberTypeDef](./type_defs.md#subscribertypedef) 
6. See [:material-code-braces: UpdateBudgetActionResponseTypeDef](./type_defs.md#updatebudgetactionresponsetypedef) 


```python
# update_budget_action method usage example with argument unpacking

kwargs: UpdateBudgetActionRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
    "ActionId": ...,
}

parent.update_budget_action(**kwargs)
```

1. See [:material-code-braces: UpdateBudgetActionRequestRequestTypeDef](./type_defs.md#updatebudgetactionrequestrequesttypedef) 

### update\_notification

Updates a notification.

Type annotations and code completion for `#!python session.create_client("budgets").update_notification` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_notification)

```python
# update_notification method definition

await def update_notification(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    OldNotification: NotificationTypeDef,  # (1)
    NewNotification: NotificationTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
2. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 


```python
# update_notification method usage example with argument unpacking

kwargs: UpdateNotificationRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
    "OldNotification": ...,
    "NewNotification": ...,
}

parent.update_notification(**kwargs)
```

1. See [:material-code-braces: UpdateNotificationRequestRequestTypeDef](./type_defs.md#updatenotificationrequestrequesttypedef) 

### update\_subscriber

Updates a subscriber.

Type annotations and code completion for `#!python session.create_client("budgets").update_subscriber` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_subscriber)

```python
# update_subscriber method definition

await def update_subscriber(
    self,
    *,
    AccountId: str,
    BudgetName: str,
    Notification: NotificationTypeDef,  # (1)
    OldSubscriber: SubscriberTypeDef,  # (2)
    NewSubscriber: SubscriberTypeDef,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
2. See [:material-code-braces: SubscriberTypeDef](./type_defs.md#subscribertypedef) 
3. See [:material-code-braces: SubscriberTypeDef](./type_defs.md#subscribertypedef) 


```python
# update_subscriber method usage example with argument unpacking

kwargs: UpdateSubscriberRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BudgetName": ...,
    "Notification": ...,
    "OldSubscriber": ...,
    "NewSubscriber": ...,
}

parent.update_subscriber(**kwargs)
```

1. See [:material-code-braces: UpdateSubscriberRequestRequestTypeDef](./type_defs.md#updatesubscriberrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("budgets").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "BudgetsClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("budgets").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("budgets").get_paginator` method with overloads.

- `client.get_paginator("describe_budget_action_histories")` -> [DescribeBudgetActionHistoriesPaginator](./paginators.md#describebudgetactionhistoriespaginator)
- `client.get_paginator("describe_budget_actions_for_account")` -> [DescribeBudgetActionsForAccountPaginator](./paginators.md#describebudgetactionsforaccountpaginator)
- `client.get_paginator("describe_budget_actions_for_budget")` -> [DescribeBudgetActionsForBudgetPaginator](./paginators.md#describebudgetactionsforbudgetpaginator)
- `client.get_paginator("describe_budget_notifications_for_account")` -> [DescribeBudgetNotificationsForAccountPaginator](./paginators.md#describebudgetnotificationsforaccountpaginator)
- `client.get_paginator("describe_budget_performance_history")` -> [DescribeBudgetPerformanceHistoryPaginator](./paginators.md#describebudgetperformancehistorypaginator)
- `client.get_paginator("describe_budgets")` -> [DescribeBudgetsPaginator](./paginators.md#describebudgetspaginator)
- `client.get_paginator("describe_notifications_for_budget")` -> [DescribeNotificationsForBudgetPaginator](./paginators.md#describenotificationsforbudgetpaginator)
- `client.get_paginator("describe_subscribers_for_notification")` -> [DescribeSubscribersForNotificationPaginator](./paginators.md#describesubscribersfornotificationpaginator)



