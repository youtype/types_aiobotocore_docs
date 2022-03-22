<a id="budgetsclient-for-aiobotocore-budgets-module"></a>

# BudgetsClient for aiobotocore Budgets module

> [Index](../README.md) > [Budgets](./README.md) > BudgetsClient

Auto-generated documentation for
[Budgets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
type annotations stubs module
[types-aiobotocore-budgets](https://pypi.org/project/types-aiobotocore-budgets/).

- [BudgetsClient for aiobotocore Budgets module](#budgetsclient-for-aiobotocore-budgets-module)
  - [BudgetsClient](#budgetsclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_budget](#create_budget)
    - [create_budget_action](#create_budget_action)
    - [create_notification](#create_notification)
    - [create_subscriber](#create_subscriber)
    - [delete_budget](#delete_budget)
    - [delete_budget_action](#delete_budget_action)
    - [delete_notification](#delete_notification)
    - [delete_subscriber](#delete_subscriber)
    - [describe_budget](#describe_budget)
    - [describe_budget_action](#describe_budget_action)
    - [describe_budget_action_histories](#describe_budget_action_histories)
    - [describe_budget_actions_for_account](#describe_budget_actions_for_account)
    - [describe_budget_actions_for_budget](#describe_budget_actions_for_budget)
    - [describe_budget_notifications_for_account](#describe_budget_notifications_for_account)
    - [describe_budget_performance_history](#describe_budget_performance_history)
    - [describe_budgets](#describe_budgets)
    - [describe_notifications_for_budget](#describe_notifications_for_budget)
    - [describe_subscribers_for_notification](#describe_subscribers_for_notification)
    - [execute_budget_action](#execute_budget_action)
    - [generate_presigned_url](#generate_presigned_url)
    - [update_budget](#update_budget)
    - [update_budget_action](#update_budget_action)
    - [update_notification](#update_notification)
    - [update_subscriber](#update_subscriber)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="budgetsclient"></a>

## BudgetsClient

Type annotations for `session.create_client("budgets")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_budgets.client import BudgetsClient

session = get_session()
async with session.create_client("budgets") as client:
    client: BudgetsClient
```

Boto3 documentation:
[Budgets.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_budgets.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.CreationLimitExceededException`
- `Exceptions.DuplicateRecordException`
- `Exceptions.ExpiredNextTokenException`
- `Exceptions.InternalErrorException`
- `Exceptions.InvalidNextTokenException`
- `Exceptions.InvalidParameterException`
- `Exceptions.NotFoundException`
- `Exceptions.ResourceLockedException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

BudgetsClient exceptions.

Type annotations for `session.create_client("budgets").exceptions` method.

Boto3 documentation:
[Budgets.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("budgets").can_paginate` method.

Boto3 documentation:
[Budgets.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create\_budget"></a>

### create_budget

Creates a budget and, if included, notifications and subscribers.

Type annotations for `session.create_client("budgets").create_budget` method.

Boto3 documentation:
[Budgets.Client.create_budget](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_budget)

Asynchronous method. Use `await create_budget(...)` for a synchronous call.

Arguments mapping described in
[CreateBudgetRequestRequestTypeDef](./type_defs.md#createbudgetrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `Budget`: [BudgetTypeDef](./type_defs.md#budgettypedef) *(required)*
- `NotificationsWithSubscribers`:
  `Sequence`\[[NotificationWithSubscribersTypeDef](./type_defs.md#notificationwithsubscriberstypedef)\]

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="create\_budget\_action"></a>

### create_budget_action

Creates a budget action.

Type annotations for `session.create_client("budgets").create_budget_action`
method.

Boto3 documentation:
[Budgets.Client.create_budget_action](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_budget_action)

Asynchronous method. Use `await create_budget_action(...)` for a synchronous
call.

Arguments mapping described in
[CreateBudgetActionRequestRequestTypeDef](./type_defs.md#createbudgetactionrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*
- `NotificationType`:
  [NotificationTypeType](./literals.md#notificationtypetype) *(required)*
- `ActionType`: [ActionTypeType](./literals.md#actiontypetype) *(required)*
- `ActionThreshold`:
  [ActionThresholdTypeDef](./type_defs.md#actionthresholdtypedef) *(required)*
- `Definition`: [DefinitionTypeDef](./type_defs.md#definitiontypedef)
  *(required)*
- `ExecutionRoleArn`: `str` *(required)*
- `ApprovalModel`: [ApprovalModelType](./literals.md#approvalmodeltype)
  *(required)*
- `Subscribers`:
  `Sequence`\[[SubscriberTypeDef](./type_defs.md#subscribertypedef)\]
  *(required)*

Returns a `Coroutine` for
[CreateBudgetActionResponseTypeDef](./type_defs.md#createbudgetactionresponsetypedef).

<a id="create\_notification"></a>

### create_notification

Creates a notification.

Type annotations for `session.create_client("budgets").create_notification`
method.

Boto3 documentation:
[Budgets.Client.create_notification](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_notification)

Asynchronous method. Use `await create_notification(...)` for a synchronous
call.

Arguments mapping described in
[CreateNotificationRequestRequestTypeDef](./type_defs.md#createnotificationrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*
- `Notification`: [NotificationTypeDef](./type_defs.md#notificationtypedef)
  *(required)*
- `Subscribers`:
  `Sequence`\[[SubscriberTypeDef](./type_defs.md#subscribertypedef)\]
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="create\_subscriber"></a>

### create_subscriber

Creates a subscriber.

Type annotations for `session.create_client("budgets").create_subscriber`
method.

Boto3 documentation:
[Budgets.Client.create_subscriber](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_subscriber)

Asynchronous method. Use `await create_subscriber(...)` for a synchronous call.

Arguments mapping described in
[CreateSubscriberRequestRequestTypeDef](./type_defs.md#createsubscriberrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*
- `Notification`: [NotificationTypeDef](./type_defs.md#notificationtypedef)
  *(required)*
- `Subscriber`: [SubscriberTypeDef](./type_defs.md#subscribertypedef)
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_budget"></a>

### delete_budget

Deletes a budget.

Type annotations for `session.create_client("budgets").delete_budget` method.

Boto3 documentation:
[Budgets.Client.delete_budget](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.delete_budget)

Asynchronous method. Use `await delete_budget(...)` for a synchronous call.

Arguments mapping described in
[DeleteBudgetRequestRequestTypeDef](./type_defs.md#deletebudgetrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_budget\_action"></a>

### delete_budget_action

Deletes a budget action.

Type annotations for `session.create_client("budgets").delete_budget_action`
method.

Boto3 documentation:
[Budgets.Client.delete_budget_action](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.delete_budget_action)

Asynchronous method. Use `await delete_budget_action(...)` for a synchronous
call.

Arguments mapping described in
[DeleteBudgetActionRequestRequestTypeDef](./type_defs.md#deletebudgetactionrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*
- `ActionId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteBudgetActionResponseTypeDef](./type_defs.md#deletebudgetactionresponsetypedef).

<a id="delete\_notification"></a>

### delete_notification

Deletes a notification.

Type annotations for `session.create_client("budgets").delete_notification`
method.

Boto3 documentation:
[Budgets.Client.delete_notification](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.delete_notification)

Asynchronous method. Use `await delete_notification(...)` for a synchronous
call.

Arguments mapping described in
[DeleteNotificationRequestRequestTypeDef](./type_defs.md#deletenotificationrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*
- `Notification`: [NotificationTypeDef](./type_defs.md#notificationtypedef)
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_subscriber"></a>

### delete_subscriber

Deletes a subscriber.

Type annotations for `session.create_client("budgets").delete_subscriber`
method.

Boto3 documentation:
[Budgets.Client.delete_subscriber](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.delete_subscriber)

Asynchronous method. Use `await delete_subscriber(...)` for a synchronous call.

Arguments mapping described in
[DeleteSubscriberRequestRequestTypeDef](./type_defs.md#deletesubscriberrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*
- `Notification`: [NotificationTypeDef](./type_defs.md#notificationtypedef)
  *(required)*
- `Subscriber`: [SubscriberTypeDef](./type_defs.md#subscribertypedef)
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe\_budget"></a>

### describe_budget

Describes a budget.

Type annotations for `session.create_client("budgets").describe_budget` method.

Boto3 documentation:
[Budgets.Client.describe_budget](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget)

Asynchronous method. Use `await describe_budget(...)` for a synchronous call.

Arguments mapping described in
[DescribeBudgetRequestRequestTypeDef](./type_defs.md#describebudgetrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeBudgetResponseTypeDef](./type_defs.md#describebudgetresponsetypedef).

<a id="describe\_budget\_action"></a>

### describe_budget_action

Describes a budget action detail.

Type annotations for `session.create_client("budgets").describe_budget_action`
method.

Boto3 documentation:
[Budgets.Client.describe_budget_action](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_action)

Asynchronous method. Use `await describe_budget_action(...)` for a synchronous
call.

Arguments mapping described in
[DescribeBudgetActionRequestRequestTypeDef](./type_defs.md#describebudgetactionrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*
- `ActionId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeBudgetActionResponseTypeDef](./type_defs.md#describebudgetactionresponsetypedef).

<a id="describe\_budget\_action\_histories"></a>

### describe_budget_action_histories

Describes a budget action history detail.

Type annotations for
`session.create_client("budgets").describe_budget_action_histories` method.

Boto3 documentation:
[Budgets.Client.describe_budget_action_histories](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_action_histories)

Asynchronous method. Use `await describe_budget_action_histories(...)` for a
synchronous call.

Arguments mapping described in
[DescribeBudgetActionHistoriesRequestRequestTypeDef](./type_defs.md#describebudgetactionhistoriesrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*
- `ActionId`: `str` *(required)*
- `TimePeriod`: [TimePeriodTypeDef](./type_defs.md#timeperiodtypedef)
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[DescribeBudgetActionHistoriesResponseTypeDef](./type_defs.md#describebudgetactionhistoriesresponsetypedef).

<a id="describe\_budget\_actions\_for\_account"></a>

### describe_budget_actions_for_account

Describes all of the budget actions for an account.

Type annotations for
`session.create_client("budgets").describe_budget_actions_for_account` method.

Boto3 documentation:
[Budgets.Client.describe_budget_actions_for_account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_actions_for_account)

Asynchronous method. Use `await describe_budget_actions_for_account(...)` for a
synchronous call.

Arguments mapping described in
[DescribeBudgetActionsForAccountRequestRequestTypeDef](./type_defs.md#describebudgetactionsforaccountrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[DescribeBudgetActionsForAccountResponseTypeDef](./type_defs.md#describebudgetactionsforaccountresponsetypedef).

<a id="describe\_budget\_actions\_for\_budget"></a>

### describe_budget_actions_for_budget

Describes all of the budget actions for a budget.

Type annotations for
`session.create_client("budgets").describe_budget_actions_for_budget` method.

Boto3 documentation:
[Budgets.Client.describe_budget_actions_for_budget](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_actions_for_budget)

Asynchronous method. Use `await describe_budget_actions_for_budget(...)` for a
synchronous call.

Arguments mapping described in
[DescribeBudgetActionsForBudgetRequestRequestTypeDef](./type_defs.md#describebudgetactionsforbudgetrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[DescribeBudgetActionsForBudgetResponseTypeDef](./type_defs.md#describebudgetactionsforbudgetresponsetypedef).

<a id="describe\_budget\_notifications\_for\_account"></a>

### describe_budget_notifications_for_account

Lists the budget names and notifications that are associated with an account.

Type annotations for
`session.create_client("budgets").describe_budget_notifications_for_account`
method.

Boto3 documentation:
[Budgets.Client.describe_budget_notifications_for_account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_notifications_for_account)

Asynchronous method. Use `await describe_budget_notifications_for_account(...)`
for a synchronous call.

Arguments mapping described in
[DescribeBudgetNotificationsForAccountRequestRequestTypeDef](./type_defs.md#describebudgetnotificationsforaccountrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[DescribeBudgetNotificationsForAccountResponseTypeDef](./type_defs.md#describebudgetnotificationsforaccountresponsetypedef).

<a id="describe\_budget\_performance\_history"></a>

### describe_budget_performance_history

Describes the history for `DAILY` , `MONTHLY` , and `QUARTERLY` budgets.

Type annotations for
`session.create_client("budgets").describe_budget_performance_history` method.

Boto3 documentation:
[Budgets.Client.describe_budget_performance_history](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_performance_history)

Asynchronous method. Use `await describe_budget_performance_history(...)` for a
synchronous call.

Arguments mapping described in
[DescribeBudgetPerformanceHistoryRequestRequestTypeDef](./type_defs.md#describebudgetperformancehistoryrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*
- `TimePeriod`: [TimePeriodTypeDef](./type_defs.md#timeperiodtypedef)
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[DescribeBudgetPerformanceHistoryResponseTypeDef](./type_defs.md#describebudgetperformancehistoryresponsetypedef).

<a id="describe\_budgets"></a>

### describe_budgets

Lists the budgets that are associated with an account.

Type annotations for `session.create_client("budgets").describe_budgets`
method.

Boto3 documentation:
[Budgets.Client.describe_budgets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budgets)

Asynchronous method. Use `await describe_budgets(...)` for a synchronous call.

Arguments mapping described in
[DescribeBudgetsRequestRequestTypeDef](./type_defs.md#describebudgetsrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[DescribeBudgetsResponseTypeDef](./type_defs.md#describebudgetsresponsetypedef).

<a id="describe\_notifications\_for\_budget"></a>

### describe_notifications_for_budget

Lists the notifications that are associated with a budget.

Type annotations for
`session.create_client("budgets").describe_notifications_for_budget` method.

Boto3 documentation:
[Budgets.Client.describe_notifications_for_budget](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_notifications_for_budget)

Asynchronous method. Use `await describe_notifications_for_budget(...)` for a
synchronous call.

Arguments mapping described in
[DescribeNotificationsForBudgetRequestRequestTypeDef](./type_defs.md#describenotificationsforbudgetrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[DescribeNotificationsForBudgetResponseTypeDef](./type_defs.md#describenotificationsforbudgetresponsetypedef).

<a id="describe\_subscribers\_for\_notification"></a>

### describe_subscribers_for_notification

Lists the subscribers that are associated with a notification.

Type annotations for
`session.create_client("budgets").describe_subscribers_for_notification`
method.

Boto3 documentation:
[Budgets.Client.describe_subscribers_for_notification](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_subscribers_for_notification)

Asynchronous method. Use `await describe_subscribers_for_notification(...)` for
a synchronous call.

Arguments mapping described in
[DescribeSubscribersForNotificationRequestRequestTypeDef](./type_defs.md#describesubscribersfornotificationrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*
- `Notification`: [NotificationTypeDef](./type_defs.md#notificationtypedef)
  *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[DescribeSubscribersForNotificationResponseTypeDef](./type_defs.md#describesubscribersfornotificationresponsetypedef).

<a id="execute\_budget\_action"></a>

### execute_budget_action

Executes a budget action.

Type annotations for `session.create_client("budgets").execute_budget_action`
method.

Boto3 documentation:
[Budgets.Client.execute_budget_action](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.execute_budget_action)

Asynchronous method. Use `await execute_budget_action(...)` for a synchronous
call.

Arguments mapping described in
[ExecuteBudgetActionRequestRequestTypeDef](./type_defs.md#executebudgetactionrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*
- `ActionId`: `str` *(required)*
- `ExecutionType`: [ExecutionTypeType](./literals.md#executiontypetype)
  *(required)*

Returns a `Coroutine` for
[ExecuteBudgetActionResponseTypeDef](./type_defs.md#executebudgetactionresponsetypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("budgets").generate_presigned_url`
method.

Boto3 documentation:
[Budgets.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="update\_budget"></a>

### update_budget

Updates a budget.

Type annotations for `session.create_client("budgets").update_budget` method.

Boto3 documentation:
[Budgets.Client.update_budget](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_budget)

Asynchronous method. Use `await update_budget(...)` for a synchronous call.

Arguments mapping described in
[UpdateBudgetRequestRequestTypeDef](./type_defs.md#updatebudgetrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `NewBudget`: [BudgetTypeDef](./type_defs.md#budgettypedef) *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_budget\_action"></a>

### update_budget_action

Updates a budget action.

Type annotations for `session.create_client("budgets").update_budget_action`
method.

Boto3 documentation:
[Budgets.Client.update_budget_action](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_budget_action)

Asynchronous method. Use `await update_budget_action(...)` for a synchronous
call.

Arguments mapping described in
[UpdateBudgetActionRequestRequestTypeDef](./type_defs.md#updatebudgetactionrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*
- `ActionId`: `str` *(required)*
- `NotificationType`:
  [NotificationTypeType](./literals.md#notificationtypetype)
- `ActionThreshold`:
  [ActionThresholdTypeDef](./type_defs.md#actionthresholdtypedef)
- `Definition`: [DefinitionTypeDef](./type_defs.md#definitiontypedef)
- `ExecutionRoleArn`: `str`
- `ApprovalModel`: [ApprovalModelType](./literals.md#approvalmodeltype)
- `Subscribers`:
  `Sequence`\[[SubscriberTypeDef](./type_defs.md#subscribertypedef)\]

Returns a `Coroutine` for
[UpdateBudgetActionResponseTypeDef](./type_defs.md#updatebudgetactionresponsetypedef).

<a id="update\_notification"></a>

### update_notification

Updates a notification.

Type annotations for `session.create_client("budgets").update_notification`
method.

Boto3 documentation:
[Budgets.Client.update_notification](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_notification)

Asynchronous method. Use `await update_notification(...)` for a synchronous
call.

Arguments mapping described in
[UpdateNotificationRequestRequestTypeDef](./type_defs.md#updatenotificationrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*
- `OldNotification`: [NotificationTypeDef](./type_defs.md#notificationtypedef)
  *(required)*
- `NewNotification`: [NotificationTypeDef](./type_defs.md#notificationtypedef)
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_subscriber"></a>

### update_subscriber

Updates a subscriber.

Type annotations for `session.create_client("budgets").update_subscriber`
method.

Boto3 documentation:
[Budgets.Client.update_subscriber](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_subscriber)

Asynchronous method. Use `await update_subscriber(...)` for a synchronous call.

Arguments mapping described in
[UpdateSubscriberRequestRequestTypeDef](./type_defs.md#updatesubscriberrequestrequesttypedef).

Keyword-only arguments:

- `AccountId`: `str` *(required)*
- `BudgetName`: `str` *(required)*
- `Notification`: [NotificationTypeDef](./type_defs.md#notificationtypedef)
  *(required)*
- `OldSubscriber`: [SubscriberTypeDef](./type_defs.md#subscribertypedef)
  *(required)*
- `NewSubscriber`: [SubscriberTypeDef](./type_defs.md#subscribertypedef)
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("budgets").__aenter__` method.

Boto3 documentation:
[Budgets.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [BudgetsClient](#budgetsclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("budgets").__aexit__` method.

Boto3 documentation:
[Budgets.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("budgets").get_paginator` method
with overloads.

- `client.get_paginator("describe_budget_action_histories")` ->
  [DescribeBudgetActionHistoriesPaginator](./paginators.md#describebudgetactionhistoriespaginator)
- `client.get_paginator("describe_budget_actions_for_account")` ->
  [DescribeBudgetActionsForAccountPaginator](./paginators.md#describebudgetactionsforaccountpaginator)
- `client.get_paginator("describe_budget_actions_for_budget")` ->
  [DescribeBudgetActionsForBudgetPaginator](./paginators.md#describebudgetactionsforbudgetpaginator)
- `client.get_paginator("describe_budget_notifications_for_account")` ->
  [DescribeBudgetNotificationsForAccountPaginator](./paginators.md#describebudgetnotificationsforaccountpaginator)
- `client.get_paginator("describe_budget_performance_history")` ->
  [DescribeBudgetPerformanceHistoryPaginator](./paginators.md#describebudgetperformancehistorypaginator)
- `client.get_paginator("describe_budgets")` ->
  [DescribeBudgetsPaginator](./paginators.md#describebudgetspaginator)
- `client.get_paginator("describe_notifications_for_budget")` ->
  [DescribeNotificationsForBudgetPaginator](./paginators.md#describenotificationsforbudgetpaginator)
- `client.get_paginator("describe_subscribers_for_notification")` ->
  [DescribeSubscribersForNotificationPaginator](./paginators.md#describesubscribersfornotificationpaginator)
