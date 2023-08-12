# Type definitions

> [Index](../README.md) > [Budgets](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Budgets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
    type annotations stubs module [types-aiobotocore-budgets](https://pypi.org/project/types-aiobotocore-budgets/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## ActionThresholdTypeDef

```python
# ActionThresholdTypeDef definition

class ActionThresholdTypeDef(TypedDict):
    ActionThresholdValue: float,
    ActionThresholdType: ThresholdTypeType,  # (1)
```

1. See [:material-code-brackets: ThresholdTypeType](./literals.md#thresholdtypetype) 
## SubscriberTypeDef

```python
# SubscriberTypeDef definition

class SubscriberTypeDef(TypedDict):
    SubscriptionType: SubscriptionTypeType,  # (1)
    Address: str,
```

1. See [:material-code-brackets: SubscriptionTypeType](./literals.md#subscriptiontypetype) 
## HistoricalOptionsTypeDef

```python
# HistoricalOptionsTypeDef definition

class HistoricalOptionsTypeDef(TypedDict):
    BudgetAdjustmentPeriod: int,
    LookBackAvailablePeriods: NotRequired[int],
```

## NotificationTypeDef

```python
# NotificationTypeDef definition

class NotificationTypeDef(TypedDict):
    NotificationType: NotificationTypeType,  # (1)
    ComparisonOperator: ComparisonOperatorType,  # (2)
    Threshold: float,
    ThresholdType: NotRequired[ThresholdTypeType],  # (3)
    NotificationState: NotRequired[NotificationStateType],  # (4)
```

1. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
2. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
3. See [:material-code-brackets: ThresholdTypeType](./literals.md#thresholdtypetype) 
4. See [:material-code-brackets: NotificationStateType](./literals.md#notificationstatetype) 
## CostTypesTypeDef

```python
# CostTypesTypeDef definition

class CostTypesTypeDef(TypedDict):
    IncludeTax: NotRequired[bool],
    IncludeSubscription: NotRequired[bool],
    UseBlended: NotRequired[bool],
    IncludeRefund: NotRequired[bool],
    IncludeCredit: NotRequired[bool],
    IncludeUpfront: NotRequired[bool],
    IncludeRecurring: NotRequired[bool],
    IncludeOtherSubscription: NotRequired[bool],
    IncludeSupport: NotRequired[bool],
    IncludeDiscount: NotRequired[bool],
    UseAmortized: NotRequired[bool],
```

## SpendTypeDef

```python
# SpendTypeDef definition

class SpendTypeDef(TypedDict):
    Amount: str,
    Unit: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## IamActionDefinitionTypeDef

```python
# IamActionDefinitionTypeDef definition

class IamActionDefinitionTypeDef(TypedDict):
    PolicyArn: str,
    Roles: NotRequired[Sequence[str]],
    Groups: NotRequired[Sequence[str]],
    Users: NotRequired[Sequence[str]],
```

## ScpActionDefinitionTypeDef

```python
# ScpActionDefinitionTypeDef definition

class ScpActionDefinitionTypeDef(TypedDict):
    PolicyId: str,
    TargetIds: Sequence[str],
```

## SsmActionDefinitionTypeDef

```python
# SsmActionDefinitionTypeDef definition

class SsmActionDefinitionTypeDef(TypedDict):
    ActionSubType: ActionSubTypeType,  # (1)
    Region: str,
    InstanceIds: Sequence[str],
```

1. See [:material-code-brackets: ActionSubTypeType](./literals.md#actionsubtypetype) 
## DeleteBudgetActionRequestRequestTypeDef

```python
# DeleteBudgetActionRequestRequestTypeDef definition

class DeleteBudgetActionRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    ActionId: str,
```

## DeleteBudgetRequestRequestTypeDef

```python
# DeleteBudgetRequestRequestTypeDef definition

class DeleteBudgetRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeBudgetActionRequestRequestTypeDef

```python
# DescribeBudgetActionRequestRequestTypeDef definition

class DescribeBudgetActionRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    ActionId: str,
```

## DescribeBudgetActionsForAccountRequestRequestTypeDef

```python
# DescribeBudgetActionsForAccountRequestRequestTypeDef definition

class DescribeBudgetActionsForAccountRequestRequestTypeDef(TypedDict):
    AccountId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeBudgetActionsForBudgetRequestRequestTypeDef

```python
# DescribeBudgetActionsForBudgetRequestRequestTypeDef definition

class DescribeBudgetActionsForBudgetRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeBudgetNotificationsForAccountRequestRequestTypeDef

```python
# DescribeBudgetNotificationsForAccountRequestRequestTypeDef definition

class DescribeBudgetNotificationsForAccountRequestRequestTypeDef(TypedDict):
    AccountId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeBudgetRequestRequestTypeDef

```python
# DescribeBudgetRequestRequestTypeDef definition

class DescribeBudgetRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
```

## DescribeBudgetsRequestRequestTypeDef

```python
# DescribeBudgetsRequestRequestTypeDef definition

class DescribeBudgetsRequestRequestTypeDef(TypedDict):
    AccountId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeNotificationsForBudgetRequestRequestTypeDef

```python
# DescribeNotificationsForBudgetRequestRequestTypeDef definition

class DescribeNotificationsForBudgetRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ExecuteBudgetActionRequestRequestTypeDef

```python
# ExecuteBudgetActionRequestRequestTypeDef definition

class ExecuteBudgetActionRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    ActionId: str,
    ExecutionType: ExecutionTypeType,  # (1)
```

1. See [:material-code-brackets: ExecutionTypeType](./literals.md#executiontypetype) 
## AutoAdjustDataTypeDef

```python
# AutoAdjustDataTypeDef definition

class AutoAdjustDataTypeDef(TypedDict):
    AutoAdjustType: AutoAdjustTypeType,  # (1)
    HistoricalOptions: NotRequired[HistoricalOptionsTypeDef],  # (2)
    LastAutoAdjustTime: NotRequired[Union[datetime, str]],
```

1. See [:material-code-brackets: AutoAdjustTypeType](./literals.md#autoadjusttypetype) 
2. See [:material-code-braces: HistoricalOptionsTypeDef](./type_defs.md#historicaloptionstypedef) 
## TimePeriodTypeDef

```python
# TimePeriodTypeDef definition

class TimePeriodTypeDef(TypedDict):
    Start: NotRequired[Union[datetime, str]],
    End: NotRequired[Union[datetime, str]],
```

## BudgetNotificationsForAccountTypeDef

```python
# BudgetNotificationsForAccountTypeDef definition

class BudgetNotificationsForAccountTypeDef(TypedDict):
    Notifications: NotRequired[List[NotificationTypeDef]],  # (1)
    BudgetName: NotRequired[str],
```

1. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
## CreateNotificationRequestRequestTypeDef

```python
# CreateNotificationRequestRequestTypeDef definition

class CreateNotificationRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    Notification: NotificationTypeDef,  # (1)
    Subscribers: Sequence[SubscriberTypeDef],  # (2)
```

1. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
2. See [:material-code-braces: SubscriberTypeDef](./type_defs.md#subscribertypedef) 
## CreateSubscriberRequestRequestTypeDef

```python
# CreateSubscriberRequestRequestTypeDef definition

class CreateSubscriberRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    Notification: NotificationTypeDef,  # (1)
    Subscriber: SubscriberTypeDef,  # (2)
```

1. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
2. See [:material-code-braces: SubscriberTypeDef](./type_defs.md#subscribertypedef) 
## DeleteNotificationRequestRequestTypeDef

```python
# DeleteNotificationRequestRequestTypeDef definition

class DeleteNotificationRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    Notification: NotificationTypeDef,  # (1)
```

1. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
## DeleteSubscriberRequestRequestTypeDef

```python
# DeleteSubscriberRequestRequestTypeDef definition

class DeleteSubscriberRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    Notification: NotificationTypeDef,  # (1)
    Subscriber: SubscriberTypeDef,  # (2)
```

1. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
2. See [:material-code-braces: SubscriberTypeDef](./type_defs.md#subscribertypedef) 
## DescribeSubscribersForNotificationRequestRequestTypeDef

```python
# DescribeSubscribersForNotificationRequestRequestTypeDef definition

class DescribeSubscribersForNotificationRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    Notification: NotificationTypeDef,  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
## NotificationWithSubscribersTypeDef

```python
# NotificationWithSubscribersTypeDef definition

class NotificationWithSubscribersTypeDef(TypedDict):
    Notification: NotificationTypeDef,  # (1)
    Subscribers: Sequence[SubscriberTypeDef],  # (2)
```

1. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
2. See [:material-code-braces: SubscriberTypeDef](./type_defs.md#subscribertypedef) 
## UpdateNotificationRequestRequestTypeDef

```python
# UpdateNotificationRequestRequestTypeDef definition

class UpdateNotificationRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    OldNotification: NotificationTypeDef,  # (1)
    NewNotification: NotificationTypeDef,  # (1)
```

1. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
2. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
## UpdateSubscriberRequestRequestTypeDef

```python
# UpdateSubscriberRequestRequestTypeDef definition

class UpdateSubscriberRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    Notification: NotificationTypeDef,  # (1)
    OldSubscriber: SubscriberTypeDef,  # (2)
    NewSubscriber: SubscriberTypeDef,  # (2)
```

1. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
2. See [:material-code-braces: SubscriberTypeDef](./type_defs.md#subscribertypedef) 
3. See [:material-code-braces: SubscriberTypeDef](./type_defs.md#subscribertypedef) 
## CalculatedSpendTypeDef

```python
# CalculatedSpendTypeDef definition

class CalculatedSpendTypeDef(TypedDict):
    ActualSpend: SpendTypeDef,  # (1)
    ForecastedSpend: NotRequired[SpendTypeDef],  # (1)
```

1. See [:material-code-braces: SpendTypeDef](./type_defs.md#spendtypedef) 
2. See [:material-code-braces: SpendTypeDef](./type_defs.md#spendtypedef) 
## CreateBudgetActionResponseTypeDef

```python
# CreateBudgetActionResponseTypeDef definition

class CreateBudgetActionResponseTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    ActionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeNotificationsForBudgetResponseTypeDef

```python
# DescribeNotificationsForBudgetResponseTypeDef definition

class DescribeNotificationsForBudgetResponseTypeDef(TypedDict):
    Notifications: List[NotificationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSubscribersForNotificationResponseTypeDef

```python
# DescribeSubscribersForNotificationResponseTypeDef definition

class DescribeSubscribersForNotificationResponseTypeDef(TypedDict):
    Subscribers: List[SubscriberTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubscriberTypeDef](./type_defs.md#subscribertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteBudgetActionResponseTypeDef

```python
# ExecuteBudgetActionResponseTypeDef definition

class ExecuteBudgetActionResponseTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    ActionId: str,
    ExecutionType: ExecutionTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ExecutionTypeType](./literals.md#executiontypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DefinitionTypeDef

```python
# DefinitionTypeDef definition

class DefinitionTypeDef(TypedDict):
    IamActionDefinition: NotRequired[IamActionDefinitionTypeDef],  # (1)
    ScpActionDefinition: NotRequired[ScpActionDefinitionTypeDef],  # (2)
    SsmActionDefinition: NotRequired[SsmActionDefinitionTypeDef],  # (3)
```

1. See [:material-code-braces: IamActionDefinitionTypeDef](./type_defs.md#iamactiondefinitiontypedef) 
2. See [:material-code-braces: ScpActionDefinitionTypeDef](./type_defs.md#scpactiondefinitiontypedef) 
3. See [:material-code-braces: SsmActionDefinitionTypeDef](./type_defs.md#ssmactiondefinitiontypedef) 
## DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef

```python
# DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef definition

class DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef(TypedDict):
    AccountId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef

```python
# DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef definition

class DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef

```python
# DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef definition

class DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef(TypedDict):
    AccountId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef

```python
# DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef definition

class DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef(TypedDict):
    AccountId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef

```python
# DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef definition

class DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef

```python
# DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef definition

class DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    Notification: NotificationTypeDef,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## BudgetedAndActualAmountsTypeDef

```python
# BudgetedAndActualAmountsTypeDef definition

class BudgetedAndActualAmountsTypeDef(TypedDict):
    BudgetedAmount: NotRequired[SpendTypeDef],  # (1)
    ActualAmount: NotRequired[SpendTypeDef],  # (1)
    TimePeriod: NotRequired[TimePeriodTypeDef],  # (3)
```

1. See [:material-code-braces: SpendTypeDef](./type_defs.md#spendtypedef) 
2. See [:material-code-braces: SpendTypeDef](./type_defs.md#spendtypedef) 
3. See [:material-code-braces: TimePeriodTypeDef](./type_defs.md#timeperiodtypedef) 
## DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef

```python
# DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef definition

class DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    ActionId: str,
    TimePeriod: NotRequired[TimePeriodTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: TimePeriodTypeDef](./type_defs.md#timeperiodtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeBudgetActionHistoriesRequestRequestTypeDef

```python
# DescribeBudgetActionHistoriesRequestRequestTypeDef definition

class DescribeBudgetActionHistoriesRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    ActionId: str,
    TimePeriod: NotRequired[TimePeriodTypeDef],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TimePeriodTypeDef](./type_defs.md#timeperiodtypedef) 
## DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef

```python
# DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef definition

class DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    TimePeriod: NotRequired[TimePeriodTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: TimePeriodTypeDef](./type_defs.md#timeperiodtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeBudgetPerformanceHistoryRequestRequestTypeDef

```python
# DescribeBudgetPerformanceHistoryRequestRequestTypeDef definition

class DescribeBudgetPerformanceHistoryRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    TimePeriod: NotRequired[TimePeriodTypeDef],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TimePeriodTypeDef](./type_defs.md#timeperiodtypedef) 
## DescribeBudgetNotificationsForAccountResponseTypeDef

```python
# DescribeBudgetNotificationsForAccountResponseTypeDef definition

class DescribeBudgetNotificationsForAccountResponseTypeDef(TypedDict):
    BudgetNotificationsForAccount: List[BudgetNotificationsForAccountTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BudgetNotificationsForAccountTypeDef](./type_defs.md#budgetnotificationsforaccounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BudgetTypeDef

```python
# BudgetTypeDef definition

class BudgetTypeDef(TypedDict):
    BudgetName: str,
    TimeUnit: TimeUnitType,  # (4)
    BudgetType: BudgetTypeType,  # (7)
    BudgetLimit: NotRequired[SpendTypeDef],  # (1)
    PlannedBudgetLimits: NotRequired[Mapping[str, SpendTypeDef]],  # (2)
    CostFilters: NotRequired[Mapping[str, Sequence[str]]],
    CostTypes: NotRequired[CostTypesTypeDef],  # (3)
    TimePeriod: NotRequired[TimePeriodTypeDef],  # (5)
    CalculatedSpend: NotRequired[CalculatedSpendTypeDef],  # (6)
    LastUpdatedTime: NotRequired[Union[datetime, str]],
    AutoAdjustData: NotRequired[AutoAdjustDataTypeDef],  # (8)
```

1. See [:material-code-braces: SpendTypeDef](./type_defs.md#spendtypedef) 
2. See [:material-code-braces: SpendTypeDef](./type_defs.md#spendtypedef) 
3. See [:material-code-braces: CostTypesTypeDef](./type_defs.md#costtypestypedef) 
4. See [:material-code-brackets: TimeUnitType](./literals.md#timeunittype) 
5. See [:material-code-braces: TimePeriodTypeDef](./type_defs.md#timeperiodtypedef) 
6. See [:material-code-braces: CalculatedSpendTypeDef](./type_defs.md#calculatedspendtypedef) 
7. See [:material-code-brackets: BudgetTypeType](./literals.md#budgettypetype) 
8. See [:material-code-braces: AutoAdjustDataTypeDef](./type_defs.md#autoadjustdatatypedef) 
## ActionTypeDef

```python
# ActionTypeDef definition

class ActionTypeDef(TypedDict):
    ActionId: str,
    BudgetName: str,
    NotificationType: NotificationTypeType,  # (1)
    ActionType: ActionTypeType,  # (2)
    ActionThreshold: ActionThresholdTypeDef,  # (3)
    Definition: DefinitionTypeDef,  # (4)
    ExecutionRoleArn: str,
    ApprovalModel: ApprovalModelType,  # (5)
    Status: ActionStatusType,  # (6)
    Subscribers: List[SubscriberTypeDef],  # (7)
```

1. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
2. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
3. See [:material-code-braces: ActionThresholdTypeDef](./type_defs.md#actionthresholdtypedef) 
4. See [:material-code-braces: DefinitionTypeDef](./type_defs.md#definitiontypedef) 
5. See [:material-code-brackets: ApprovalModelType](./literals.md#approvalmodeltype) 
6. See [:material-code-brackets: ActionStatusType](./literals.md#actionstatustype) 
7. See [:material-code-braces: SubscriberTypeDef](./type_defs.md#subscribertypedef) 
## CreateBudgetActionRequestRequestTypeDef

```python
# CreateBudgetActionRequestRequestTypeDef definition

class CreateBudgetActionRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    NotificationType: NotificationTypeType,  # (1)
    ActionType: ActionTypeType,  # (2)
    ActionThreshold: ActionThresholdTypeDef,  # (3)
    Definition: DefinitionTypeDef,  # (4)
    ExecutionRoleArn: str,
    ApprovalModel: ApprovalModelType,  # (5)
    Subscribers: Sequence[SubscriberTypeDef],  # (6)
```

1. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
2. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
3. See [:material-code-braces: ActionThresholdTypeDef](./type_defs.md#actionthresholdtypedef) 
4. See [:material-code-braces: DefinitionTypeDef](./type_defs.md#definitiontypedef) 
5. See [:material-code-brackets: ApprovalModelType](./literals.md#approvalmodeltype) 
6. See [:material-code-braces: SubscriberTypeDef](./type_defs.md#subscribertypedef) 
## UpdateBudgetActionRequestRequestTypeDef

```python
# UpdateBudgetActionRequestRequestTypeDef definition

class UpdateBudgetActionRequestRequestTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    ActionId: str,
    NotificationType: NotRequired[NotificationTypeType],  # (1)
    ActionThreshold: NotRequired[ActionThresholdTypeDef],  # (2)
    Definition: NotRequired[DefinitionTypeDef],  # (3)
    ExecutionRoleArn: NotRequired[str],
    ApprovalModel: NotRequired[ApprovalModelType],  # (4)
    Subscribers: NotRequired[Sequence[SubscriberTypeDef]],  # (5)
```

1. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
2. See [:material-code-braces: ActionThresholdTypeDef](./type_defs.md#actionthresholdtypedef) 
3. See [:material-code-braces: DefinitionTypeDef](./type_defs.md#definitiontypedef) 
4. See [:material-code-brackets: ApprovalModelType](./literals.md#approvalmodeltype) 
5. See [:material-code-braces: SubscriberTypeDef](./type_defs.md#subscribertypedef) 
## BudgetPerformanceHistoryTypeDef

```python
# BudgetPerformanceHistoryTypeDef definition

class BudgetPerformanceHistoryTypeDef(TypedDict):
    BudgetName: NotRequired[str],
    BudgetType: NotRequired[BudgetTypeType],  # (1)
    CostFilters: NotRequired[Dict[str, List[str]]],
    CostTypes: NotRequired[CostTypesTypeDef],  # (2)
    TimeUnit: NotRequired[TimeUnitType],  # (3)
    BudgetedAndActualAmountsList: NotRequired[List[BudgetedAndActualAmountsTypeDef]],  # (4)
```

1. See [:material-code-brackets: BudgetTypeType](./literals.md#budgettypetype) 
2. See [:material-code-braces: CostTypesTypeDef](./type_defs.md#costtypestypedef) 
3. See [:material-code-brackets: TimeUnitType](./literals.md#timeunittype) 
4. See [:material-code-braces: BudgetedAndActualAmountsTypeDef](./type_defs.md#budgetedandactualamountstypedef) 
## CreateBudgetRequestRequestTypeDef

```python
# CreateBudgetRequestRequestTypeDef definition

class CreateBudgetRequestRequestTypeDef(TypedDict):
    AccountId: str,
    Budget: BudgetTypeDef,  # (1)
    NotificationsWithSubscribers: NotRequired[Sequence[NotificationWithSubscribersTypeDef]],  # (2)
```

1. See [:material-code-braces: BudgetTypeDef](./type_defs.md#budgettypedef) 
2. See [:material-code-braces: NotificationWithSubscribersTypeDef](./type_defs.md#notificationwithsubscriberstypedef) 
## DescribeBudgetResponseTypeDef

```python
# DescribeBudgetResponseTypeDef definition

class DescribeBudgetResponseTypeDef(TypedDict):
    Budget: BudgetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BudgetTypeDef](./type_defs.md#budgettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBudgetsResponseTypeDef

```python
# DescribeBudgetsResponseTypeDef definition

class DescribeBudgetsResponseTypeDef(TypedDict):
    Budgets: List[BudgetTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BudgetTypeDef](./type_defs.md#budgettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBudgetRequestRequestTypeDef

```python
# UpdateBudgetRequestRequestTypeDef definition

class UpdateBudgetRequestRequestTypeDef(TypedDict):
    AccountId: str,
    NewBudget: BudgetTypeDef,  # (1)
```

1. See [:material-code-braces: BudgetTypeDef](./type_defs.md#budgettypedef) 
## ActionHistoryDetailsTypeDef

```python
# ActionHistoryDetailsTypeDef definition

class ActionHistoryDetailsTypeDef(TypedDict):
    Message: str,
    Action: ActionTypeDef,  # (1)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
## DeleteBudgetActionResponseTypeDef

```python
# DeleteBudgetActionResponseTypeDef definition

class DeleteBudgetActionResponseTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    Action: ActionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBudgetActionResponseTypeDef

```python
# DescribeBudgetActionResponseTypeDef definition

class DescribeBudgetActionResponseTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    Action: ActionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBudgetActionsForAccountResponseTypeDef

```python
# DescribeBudgetActionsForAccountResponseTypeDef definition

class DescribeBudgetActionsForAccountResponseTypeDef(TypedDict):
    Actions: List[ActionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBudgetActionsForBudgetResponseTypeDef

```python
# DescribeBudgetActionsForBudgetResponseTypeDef definition

class DescribeBudgetActionsForBudgetResponseTypeDef(TypedDict):
    Actions: List[ActionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBudgetActionResponseTypeDef

```python
# UpdateBudgetActionResponseTypeDef definition

class UpdateBudgetActionResponseTypeDef(TypedDict):
    AccountId: str,
    BudgetName: str,
    OldAction: ActionTypeDef,  # (1)
    NewAction: ActionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBudgetPerformanceHistoryResponseTypeDef

```python
# DescribeBudgetPerformanceHistoryResponseTypeDef definition

class DescribeBudgetPerformanceHistoryResponseTypeDef(TypedDict):
    BudgetPerformanceHistory: BudgetPerformanceHistoryTypeDef,  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BudgetPerformanceHistoryTypeDef](./type_defs.md#budgetperformancehistorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ActionHistoryTypeDef

```python
# ActionHistoryTypeDef definition

class ActionHistoryTypeDef(TypedDict):
    Timestamp: datetime,
    Status: ActionStatusType,  # (1)
    EventType: EventTypeType,  # (2)
    ActionHistoryDetails: ActionHistoryDetailsTypeDef,  # (3)
```

1. See [:material-code-brackets: ActionStatusType](./literals.md#actionstatustype) 
2. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
3. See [:material-code-braces: ActionHistoryDetailsTypeDef](./type_defs.md#actionhistorydetailstypedef) 
## DescribeBudgetActionHistoriesResponseTypeDef

```python
# DescribeBudgetActionHistoriesResponseTypeDef definition

class DescribeBudgetActionHistoriesResponseTypeDef(TypedDict):
    ActionHistories: List[ActionHistoryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActionHistoryTypeDef](./type_defs.md#actionhistorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
