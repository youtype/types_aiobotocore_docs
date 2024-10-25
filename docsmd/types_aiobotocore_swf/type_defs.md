# Type definitions

> [Index](../README.md) > [SWF](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SWF](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
    type annotations stubs module [types-aiobotocore-swf](https://pypi.org/project/types-aiobotocore-swf/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## ActivityTaskCancelRequestedEventAttributesTypeDef

```python
# ActivityTaskCancelRequestedEventAttributesTypeDef definition

class ActivityTaskCancelRequestedEventAttributesTypeDef(TypedDict):
    decisionTaskCompletedEventId: int,
    activityId: str,
```

## ActivityTaskCanceledEventAttributesTypeDef

```python
# ActivityTaskCanceledEventAttributesTypeDef definition

class ActivityTaskCanceledEventAttributesTypeDef(TypedDict):
    scheduledEventId: int,
    startedEventId: int,
    details: NotRequired[str],
    latestCancelRequestedEventId: NotRequired[int],
```

## ActivityTaskCompletedEventAttributesTypeDef

```python
# ActivityTaskCompletedEventAttributesTypeDef definition

class ActivityTaskCompletedEventAttributesTypeDef(TypedDict):
    scheduledEventId: int,
    startedEventId: int,
    result: NotRequired[str],
```

## ActivityTaskFailedEventAttributesTypeDef

```python
# ActivityTaskFailedEventAttributesTypeDef definition

class ActivityTaskFailedEventAttributesTypeDef(TypedDict):
    scheduledEventId: int,
    startedEventId: int,
    reason: NotRequired[str],
    details: NotRequired[str],
```

## ActivityTypeTypeDef

```python
# ActivityTypeTypeDef definition

class ActivityTypeTypeDef(TypedDict):
    name: str,
    version: str,
```

## TaskListTypeDef

```python
# TaskListTypeDef definition

class TaskListTypeDef(TypedDict):
    name: str,
```

## ActivityTaskStartedEventAttributesTypeDef

```python
# ActivityTaskStartedEventAttributesTypeDef definition

class ActivityTaskStartedEventAttributesTypeDef(TypedDict):
    scheduledEventId: int,
    identity: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## ActivityTaskTimedOutEventAttributesTypeDef

```python
# ActivityTaskTimedOutEventAttributesTypeDef definition

class ActivityTaskTimedOutEventAttributesTypeDef(TypedDict):
    timeoutType: ActivityTaskTimeoutTypeType,  # (1)
    scheduledEventId: int,
    startedEventId: int,
    details: NotRequired[str],
```

1. See [:material-code-brackets: ActivityTaskTimeoutTypeType](./literals.md#activitytasktimeouttypetype) 
## WorkflowExecutionTypeDef

```python
# WorkflowExecutionTypeDef definition

class WorkflowExecutionTypeDef(TypedDict):
    workflowId: str,
    runId: str,
```

## CancelTimerDecisionAttributesTypeDef

```python
# CancelTimerDecisionAttributesTypeDef definition

class CancelTimerDecisionAttributesTypeDef(TypedDict):
    timerId: str,
```

## CancelTimerFailedEventAttributesTypeDef

```python
# CancelTimerFailedEventAttributesTypeDef definition

class CancelTimerFailedEventAttributesTypeDef(TypedDict):
    timerId: str,
    cause: CancelTimerFailedCauseType,  # (1)
    decisionTaskCompletedEventId: int,
```

1. See [:material-code-brackets: CancelTimerFailedCauseType](./literals.md#canceltimerfailedcausetype) 
## CancelWorkflowExecutionDecisionAttributesTypeDef

```python
# CancelWorkflowExecutionDecisionAttributesTypeDef definition

class CancelWorkflowExecutionDecisionAttributesTypeDef(TypedDict):
    details: NotRequired[str],
```

## CancelWorkflowExecutionFailedEventAttributesTypeDef

```python
# CancelWorkflowExecutionFailedEventAttributesTypeDef definition

class CancelWorkflowExecutionFailedEventAttributesTypeDef(TypedDict):
    cause: CancelWorkflowExecutionFailedCauseType,  # (1)
    decisionTaskCompletedEventId: int,
```

1. See [:material-code-brackets: CancelWorkflowExecutionFailedCauseType](./literals.md#cancelworkflowexecutionfailedcausetype) 
## WorkflowTypeTypeDef

```python
# WorkflowTypeTypeDef definition

class WorkflowTypeTypeDef(TypedDict):
    name: str,
    version: str,
```

## CloseStatusFilterTypeDef

```python
# CloseStatusFilterTypeDef definition

class CloseStatusFilterTypeDef(TypedDict):
    status: CloseStatusType,  # (1)
```

1. See [:material-code-brackets: CloseStatusType](./literals.md#closestatustype) 
## CompleteWorkflowExecutionDecisionAttributesTypeDef

```python
# CompleteWorkflowExecutionDecisionAttributesTypeDef definition

class CompleteWorkflowExecutionDecisionAttributesTypeDef(TypedDict):
    result: NotRequired[str],
```

## CompleteWorkflowExecutionFailedEventAttributesTypeDef

```python
# CompleteWorkflowExecutionFailedEventAttributesTypeDef definition

class CompleteWorkflowExecutionFailedEventAttributesTypeDef(TypedDict):
    cause: CompleteWorkflowExecutionFailedCauseType,  # (1)
    decisionTaskCompletedEventId: int,
```

1. See [:material-code-brackets: CompleteWorkflowExecutionFailedCauseType](./literals.md#completeworkflowexecutionfailedcausetype) 
## ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef

```python
# ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef definition

class ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef(TypedDict):
    cause: ContinueAsNewWorkflowExecutionFailedCauseType,  # (1)
    decisionTaskCompletedEventId: int,
```

1. See [:material-code-brackets: ContinueAsNewWorkflowExecutionFailedCauseType](./literals.md#continueasnewworkflowexecutionfailedcausetype) 
## TagFilterTypeDef

```python
# TagFilterTypeDef definition

class TagFilterTypeDef(TypedDict):
    tag: str,
```

## WorkflowExecutionFilterTypeDef

```python
# WorkflowExecutionFilterTypeDef definition

class WorkflowExecutionFilterTypeDef(TypedDict):
    workflowId: str,
```

## WorkflowTypeFilterTypeDef

```python
# WorkflowTypeFilterTypeDef definition

class WorkflowTypeFilterTypeDef(TypedDict):
    name: str,
    version: NotRequired[str],
```

## DecisionTaskStartedEventAttributesTypeDef

```python
# DecisionTaskStartedEventAttributesTypeDef definition

class DecisionTaskStartedEventAttributesTypeDef(TypedDict):
    scheduledEventId: int,
    identity: NotRequired[str],
```

## DecisionTaskTimedOutEventAttributesTypeDef

```python
# DecisionTaskTimedOutEventAttributesTypeDef definition

class DecisionTaskTimedOutEventAttributesTypeDef(TypedDict):
    timeoutType: DecisionTaskTimeoutTypeType,  # (1)
    scheduledEventId: int,
    startedEventId: int,
```

1. See [:material-code-brackets: DecisionTaskTimeoutTypeType](./literals.md#decisiontasktimeouttypetype) 
## FailWorkflowExecutionDecisionAttributesTypeDef

```python
# FailWorkflowExecutionDecisionAttributesTypeDef definition

class FailWorkflowExecutionDecisionAttributesTypeDef(TypedDict):
    reason: NotRequired[str],
    details: NotRequired[str],
```

## RecordMarkerDecisionAttributesTypeDef

```python
# RecordMarkerDecisionAttributesTypeDef definition

class RecordMarkerDecisionAttributesTypeDef(TypedDict):
    markerName: str,
    details: NotRequired[str],
```

## RequestCancelActivityTaskDecisionAttributesTypeDef

```python
# RequestCancelActivityTaskDecisionAttributesTypeDef definition

class RequestCancelActivityTaskDecisionAttributesTypeDef(TypedDict):
    activityId: str,
```

## RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef

```python
# RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef definition

class RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef(TypedDict):
    workflowId: str,
    runId: NotRequired[str],
    control: NotRequired[str],
```

## ScheduleLambdaFunctionDecisionAttributesTypeDef

```python
# ScheduleLambdaFunctionDecisionAttributesTypeDef definition

class ScheduleLambdaFunctionDecisionAttributesTypeDef(TypedDict):
    id: str,
    name: str,
    control: NotRequired[str],
    input: NotRequired[str],
    startToCloseTimeout: NotRequired[str],
```

## SignalExternalWorkflowExecutionDecisionAttributesTypeDef

```python
# SignalExternalWorkflowExecutionDecisionAttributesTypeDef definition

class SignalExternalWorkflowExecutionDecisionAttributesTypeDef(TypedDict):
    workflowId: str,
    signalName: str,
    runId: NotRequired[str],
    input: NotRequired[str],
    control: NotRequired[str],
```

## StartTimerDecisionAttributesTypeDef

```python
# StartTimerDecisionAttributesTypeDef definition

class StartTimerDecisionAttributesTypeDef(TypedDict):
    timerId: str,
    startToFireTimeout: str,
    control: NotRequired[str],
```

## DeprecateDomainInputRequestTypeDef

```python
# DeprecateDomainInputRequestTypeDef definition

class DeprecateDomainInputRequestTypeDef(TypedDict):
    name: str,
```

## DescribeDomainInputRequestTypeDef

```python
# DescribeDomainInputRequestTypeDef definition

class DescribeDomainInputRequestTypeDef(TypedDict):
    name: str,
```

## DomainConfigurationTypeDef

```python
# DomainConfigurationTypeDef definition

class DomainConfigurationTypeDef(TypedDict):
    workflowExecutionRetentionPeriodInDays: str,
```

## DomainInfoTypeDef

```python
# DomainInfoTypeDef definition

class DomainInfoTypeDef(TypedDict):
    name: str,
    status: RegistrationStatusType,  # (1)
    description: NotRequired[str],
    arn: NotRequired[str],
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
## FailWorkflowExecutionFailedEventAttributesTypeDef

```python
# FailWorkflowExecutionFailedEventAttributesTypeDef definition

class FailWorkflowExecutionFailedEventAttributesTypeDef(TypedDict):
    cause: FailWorkflowExecutionFailedCauseType,  # (1)
    decisionTaskCompletedEventId: int,
```

1. See [:material-code-brackets: FailWorkflowExecutionFailedCauseType](./literals.md#failworkflowexecutionfailedcausetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## LambdaFunctionCompletedEventAttributesTypeDef

```python
# LambdaFunctionCompletedEventAttributesTypeDef definition

class LambdaFunctionCompletedEventAttributesTypeDef(TypedDict):
    scheduledEventId: int,
    startedEventId: int,
    result: NotRequired[str],
```

## LambdaFunctionFailedEventAttributesTypeDef

```python
# LambdaFunctionFailedEventAttributesTypeDef definition

class LambdaFunctionFailedEventAttributesTypeDef(TypedDict):
    scheduledEventId: int,
    startedEventId: int,
    reason: NotRequired[str],
    details: NotRequired[str],
```

## LambdaFunctionScheduledEventAttributesTypeDef

```python
# LambdaFunctionScheduledEventAttributesTypeDef definition

class LambdaFunctionScheduledEventAttributesTypeDef(TypedDict):
    id: str,
    name: str,
    decisionTaskCompletedEventId: int,
    control: NotRequired[str],
    input: NotRequired[str],
    startToCloseTimeout: NotRequired[str],
```

## LambdaFunctionStartedEventAttributesTypeDef

```python
# LambdaFunctionStartedEventAttributesTypeDef definition

class LambdaFunctionStartedEventAttributesTypeDef(TypedDict):
    scheduledEventId: int,
```

## LambdaFunctionTimedOutEventAttributesTypeDef

```python
# LambdaFunctionTimedOutEventAttributesTypeDef definition

class LambdaFunctionTimedOutEventAttributesTypeDef(TypedDict):
    scheduledEventId: int,
    startedEventId: int,
    timeoutType: NotRequired[LambdaFunctionTimeoutTypeType],  # (1)
```

1. See [:material-code-brackets: LambdaFunctionTimeoutTypeType](./literals.md#lambdafunctiontimeouttypetype) 
## MarkerRecordedEventAttributesTypeDef

```python
# MarkerRecordedEventAttributesTypeDef definition

class MarkerRecordedEventAttributesTypeDef(TypedDict):
    markerName: str,
    decisionTaskCompletedEventId: int,
    details: NotRequired[str],
```

## RecordMarkerFailedEventAttributesTypeDef

```python
# RecordMarkerFailedEventAttributesTypeDef definition

class RecordMarkerFailedEventAttributesTypeDef(TypedDict):
    markerName: str,
    cause: RecordMarkerFailedCauseType,  # (1)
    decisionTaskCompletedEventId: int,
```

1. See [:material-code-brackets: RecordMarkerFailedCauseType](./literals.md#recordmarkerfailedcausetype) 
## RequestCancelActivityTaskFailedEventAttributesTypeDef

```python
# RequestCancelActivityTaskFailedEventAttributesTypeDef definition

class RequestCancelActivityTaskFailedEventAttributesTypeDef(TypedDict):
    activityId: str,
    cause: RequestCancelActivityTaskFailedCauseType,  # (1)
    decisionTaskCompletedEventId: int,
```

1. See [:material-code-brackets: RequestCancelActivityTaskFailedCauseType](./literals.md#requestcancelactivitytaskfailedcausetype) 
## RequestCancelExternalWorkflowExecutionFailedEventAttributesTypeDef

```python
# RequestCancelExternalWorkflowExecutionFailedEventAttributesTypeDef definition

class RequestCancelExternalWorkflowExecutionFailedEventAttributesTypeDef(TypedDict):
    workflowId: str,
    cause: RequestCancelExternalWorkflowExecutionFailedCauseType,  # (1)
    initiatedEventId: int,
    decisionTaskCompletedEventId: int,
    runId: NotRequired[str],
    control: NotRequired[str],
```

1. See [:material-code-brackets: RequestCancelExternalWorkflowExecutionFailedCauseType](./literals.md#requestcancelexternalworkflowexecutionfailedcausetype) 
## RequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef

```python
# RequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef definition

class RequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef(TypedDict):
    workflowId: str,
    decisionTaskCompletedEventId: int,
    runId: NotRequired[str],
    control: NotRequired[str],
```

## ScheduleLambdaFunctionFailedEventAttributesTypeDef

```python
# ScheduleLambdaFunctionFailedEventAttributesTypeDef definition

class ScheduleLambdaFunctionFailedEventAttributesTypeDef(TypedDict):
    id: str,
    name: str,
    cause: ScheduleLambdaFunctionFailedCauseType,  # (1)
    decisionTaskCompletedEventId: int,
```

1. See [:material-code-brackets: ScheduleLambdaFunctionFailedCauseType](./literals.md#schedulelambdafunctionfailedcausetype) 
## SignalExternalWorkflowExecutionFailedEventAttributesTypeDef

```python
# SignalExternalWorkflowExecutionFailedEventAttributesTypeDef definition

class SignalExternalWorkflowExecutionFailedEventAttributesTypeDef(TypedDict):
    workflowId: str,
    cause: SignalExternalWorkflowExecutionFailedCauseType,  # (1)
    initiatedEventId: int,
    decisionTaskCompletedEventId: int,
    runId: NotRequired[str],
    control: NotRequired[str],
```

1. See [:material-code-brackets: SignalExternalWorkflowExecutionFailedCauseType](./literals.md#signalexternalworkflowexecutionfailedcausetype) 
## SignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef

```python
# SignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef definition

class SignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef(TypedDict):
    workflowId: str,
    signalName: str,
    decisionTaskCompletedEventId: int,
    runId: NotRequired[str],
    input: NotRequired[str],
    control: NotRequired[str],
```

## StartLambdaFunctionFailedEventAttributesTypeDef

```python
# StartLambdaFunctionFailedEventAttributesTypeDef definition

class StartLambdaFunctionFailedEventAttributesTypeDef(TypedDict):
    scheduledEventId: NotRequired[int],
    cause: NotRequired[StartLambdaFunctionFailedCauseType],  # (1)
    message: NotRequired[str],
```

1. See [:material-code-brackets: StartLambdaFunctionFailedCauseType](./literals.md#startlambdafunctionfailedcausetype) 
## StartTimerFailedEventAttributesTypeDef

```python
# StartTimerFailedEventAttributesTypeDef definition

class StartTimerFailedEventAttributesTypeDef(TypedDict):
    timerId: str,
    cause: StartTimerFailedCauseType,  # (1)
    decisionTaskCompletedEventId: int,
```

1. See [:material-code-brackets: StartTimerFailedCauseType](./literals.md#starttimerfailedcausetype) 
## TimerCanceledEventAttributesTypeDef

```python
# TimerCanceledEventAttributesTypeDef definition

class TimerCanceledEventAttributesTypeDef(TypedDict):
    timerId: str,
    startedEventId: int,
    decisionTaskCompletedEventId: int,
```

## TimerFiredEventAttributesTypeDef

```python
# TimerFiredEventAttributesTypeDef definition

class TimerFiredEventAttributesTypeDef(TypedDict):
    timerId: str,
    startedEventId: int,
```

## TimerStartedEventAttributesTypeDef

```python
# TimerStartedEventAttributesTypeDef definition

class TimerStartedEventAttributesTypeDef(TypedDict):
    timerId: str,
    startToFireTimeout: str,
    decisionTaskCompletedEventId: int,
    control: NotRequired[str],
```

## WorkflowExecutionCanceledEventAttributesTypeDef

```python
# WorkflowExecutionCanceledEventAttributesTypeDef definition

class WorkflowExecutionCanceledEventAttributesTypeDef(TypedDict):
    decisionTaskCompletedEventId: int,
    details: NotRequired[str],
```

## WorkflowExecutionCompletedEventAttributesTypeDef

```python
# WorkflowExecutionCompletedEventAttributesTypeDef definition

class WorkflowExecutionCompletedEventAttributesTypeDef(TypedDict):
    decisionTaskCompletedEventId: int,
    result: NotRequired[str],
```

## WorkflowExecutionFailedEventAttributesTypeDef

```python
# WorkflowExecutionFailedEventAttributesTypeDef definition

class WorkflowExecutionFailedEventAttributesTypeDef(TypedDict):
    decisionTaskCompletedEventId: int,
    reason: NotRequired[str],
    details: NotRequired[str],
```

## WorkflowExecutionTerminatedEventAttributesTypeDef

```python
# WorkflowExecutionTerminatedEventAttributesTypeDef definition

class WorkflowExecutionTerminatedEventAttributesTypeDef(TypedDict):
    childPolicy: ChildPolicyType,  # (1)
    reason: NotRequired[str],
    details: NotRequired[str],
    cause: NotRequired[WorkflowExecutionTerminatedCauseType],  # (2)
```

1. See [:material-code-brackets: ChildPolicyType](./literals.md#childpolicytype) 
2. See [:material-code-brackets: WorkflowExecutionTerminatedCauseType](./literals.md#workflowexecutionterminatedcausetype) 
## WorkflowExecutionTimedOutEventAttributesTypeDef

```python
# WorkflowExecutionTimedOutEventAttributesTypeDef definition

class WorkflowExecutionTimedOutEventAttributesTypeDef(TypedDict):
    timeoutType: WorkflowExecutionTimeoutTypeType,  # (1)
    childPolicy: ChildPolicyType,  # (2)
```

1. See [:material-code-brackets: WorkflowExecutionTimeoutTypeType](./literals.md#workflowexecutiontimeouttypetype) 
2. See [:material-code-brackets: ChildPolicyType](./literals.md#childpolicytype) 
## ListActivityTypesInputRequestTypeDef

```python
# ListActivityTypesInputRequestTypeDef definition

class ListActivityTypesInputRequestTypeDef(TypedDict):
    domain: str,
    registrationStatus: RegistrationStatusType,  # (1)
    name: NotRequired[str],
    nextPageToken: NotRequired[str],
    maximumPageSize: NotRequired[int],
    reverseOrder: NotRequired[bool],
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
## ListDomainsInputRequestTypeDef

```python
# ListDomainsInputRequestTypeDef definition

class ListDomainsInputRequestTypeDef(TypedDict):
    registrationStatus: RegistrationStatusType,  # (1)
    nextPageToken: NotRequired[str],
    maximumPageSize: NotRequired[int],
    reverseOrder: NotRequired[bool],
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ResourceTagTypeDef

```python
# ResourceTagTypeDef definition

class ResourceTagTypeDef(TypedDict):
    key: str,
    value: NotRequired[str],
```

## ListWorkflowTypesInputRequestTypeDef

```python
# ListWorkflowTypesInputRequestTypeDef definition

class ListWorkflowTypesInputRequestTypeDef(TypedDict):
    domain: str,
    registrationStatus: RegistrationStatusType,  # (1)
    name: NotRequired[str],
    nextPageToken: NotRequired[str],
    maximumPageSize: NotRequired[int],
    reverseOrder: NotRequired[bool],
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
## RecordActivityTaskHeartbeatInputRequestTypeDef

```python
# RecordActivityTaskHeartbeatInputRequestTypeDef definition

class RecordActivityTaskHeartbeatInputRequestTypeDef(TypedDict):
    taskToken: str,
    details: NotRequired[str],
```

## RequestCancelWorkflowExecutionInputRequestTypeDef

```python
# RequestCancelWorkflowExecutionInputRequestTypeDef definition

class RequestCancelWorkflowExecutionInputRequestTypeDef(TypedDict):
    domain: str,
    workflowId: str,
    runId: NotRequired[str],
```

## RespondActivityTaskCanceledInputRequestTypeDef

```python
# RespondActivityTaskCanceledInputRequestTypeDef definition

class RespondActivityTaskCanceledInputRequestTypeDef(TypedDict):
    taskToken: str,
    details: NotRequired[str],
```

## RespondActivityTaskCompletedInputRequestTypeDef

```python
# RespondActivityTaskCompletedInputRequestTypeDef definition

class RespondActivityTaskCompletedInputRequestTypeDef(TypedDict):
    taskToken: str,
    result: NotRequired[str],
```

## RespondActivityTaskFailedInputRequestTypeDef

```python
# RespondActivityTaskFailedInputRequestTypeDef definition

class RespondActivityTaskFailedInputRequestTypeDef(TypedDict):
    taskToken: str,
    reason: NotRequired[str],
    details: NotRequired[str],
```

## SignalWorkflowExecutionInputRequestTypeDef

```python
# SignalWorkflowExecutionInputRequestTypeDef definition

class SignalWorkflowExecutionInputRequestTypeDef(TypedDict):
    domain: str,
    workflowId: str,
    signalName: str,
    runId: NotRequired[str],
    input: NotRequired[str],
```

## TerminateWorkflowExecutionInputRequestTypeDef

```python
# TerminateWorkflowExecutionInputRequestTypeDef definition

class TerminateWorkflowExecutionInputRequestTypeDef(TypedDict):
    domain: str,
    workflowId: str,
    runId: NotRequired[str],
    reason: NotRequired[str],
    details: NotRequired[str],
    childPolicy: NotRequired[ChildPolicyType],  # (1)
```

1. See [:material-code-brackets: ChildPolicyType](./literals.md#childpolicytype) 
## UndeprecateDomainInputRequestTypeDef

```python
# UndeprecateDomainInputRequestTypeDef definition

class UndeprecateDomainInputRequestTypeDef(TypedDict):
    name: str,
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## WorkflowExecutionOpenCountsTypeDef

```python
# WorkflowExecutionOpenCountsTypeDef definition

class WorkflowExecutionOpenCountsTypeDef(TypedDict):
    openActivityTasks: int,
    openDecisionTasks: int,
    openTimers: int,
    openChildWorkflowExecutions: int,
    openLambdaFunctions: NotRequired[int],
```

## ActivityTypeInfoTypeDef

```python
# ActivityTypeInfoTypeDef definition

class ActivityTypeInfoTypeDef(TypedDict):
    activityType: ActivityTypeTypeDef,  # (1)
    status: RegistrationStatusType,  # (2)
    creationDate: datetime,
    description: NotRequired[str],
    deprecationDate: NotRequired[datetime],
```

1. See [:material-code-braces: ActivityTypeTypeDef](./type_defs.md#activitytypetypedef) 
2. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
## DeleteActivityTypeInputRequestTypeDef

```python
# DeleteActivityTypeInputRequestTypeDef definition

class DeleteActivityTypeInputRequestTypeDef(TypedDict):
    domain: str,
    activityType: ActivityTypeTypeDef,  # (1)
```

1. See [:material-code-braces: ActivityTypeTypeDef](./type_defs.md#activitytypetypedef) 
## DeprecateActivityTypeInputRequestTypeDef

```python
# DeprecateActivityTypeInputRequestTypeDef definition

class DeprecateActivityTypeInputRequestTypeDef(TypedDict):
    domain: str,
    activityType: ActivityTypeTypeDef,  # (1)
```

1. See [:material-code-braces: ActivityTypeTypeDef](./type_defs.md#activitytypetypedef) 
## DescribeActivityTypeInputRequestTypeDef

```python
# DescribeActivityTypeInputRequestTypeDef definition

class DescribeActivityTypeInputRequestTypeDef(TypedDict):
    domain: str,
    activityType: ActivityTypeTypeDef,  # (1)
```

1. See [:material-code-braces: ActivityTypeTypeDef](./type_defs.md#activitytypetypedef) 
## ScheduleActivityTaskFailedEventAttributesTypeDef

```python
# ScheduleActivityTaskFailedEventAttributesTypeDef definition

class ScheduleActivityTaskFailedEventAttributesTypeDef(TypedDict):
    activityType: ActivityTypeTypeDef,  # (1)
    activityId: str,
    cause: ScheduleActivityTaskFailedCauseType,  # (2)
    decisionTaskCompletedEventId: int,
```

1. See [:material-code-braces: ActivityTypeTypeDef](./type_defs.md#activitytypetypedef) 
2. See [:material-code-brackets: ScheduleActivityTaskFailedCauseType](./literals.md#scheduleactivitytaskfailedcausetype) 
## UndeprecateActivityTypeInputRequestTypeDef

```python
# UndeprecateActivityTypeInputRequestTypeDef definition

class UndeprecateActivityTypeInputRequestTypeDef(TypedDict):
    domain: str,
    activityType: ActivityTypeTypeDef,  # (1)
```

1. See [:material-code-braces: ActivityTypeTypeDef](./type_defs.md#activitytypetypedef) 
## ActivityTaskScheduledEventAttributesTypeDef

```python
# ActivityTaskScheduledEventAttributesTypeDef definition

class ActivityTaskScheduledEventAttributesTypeDef(TypedDict):
    activityType: ActivityTypeTypeDef,  # (1)
    activityId: str,
    taskList: TaskListTypeDef,  # (2)
    decisionTaskCompletedEventId: int,
    input: NotRequired[str],
    control: NotRequired[str],
    scheduleToStartTimeout: NotRequired[str],
    scheduleToCloseTimeout: NotRequired[str],
    startToCloseTimeout: NotRequired[str],
    taskPriority: NotRequired[str],
    heartbeatTimeout: NotRequired[str],
```

1. See [:material-code-braces: ActivityTypeTypeDef](./type_defs.md#activitytypetypedef) 
2. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
## ActivityTypeConfigurationTypeDef

```python
# ActivityTypeConfigurationTypeDef definition

class ActivityTypeConfigurationTypeDef(TypedDict):
    defaultTaskStartToCloseTimeout: NotRequired[str],
    defaultTaskHeartbeatTimeout: NotRequired[str],
    defaultTaskList: NotRequired[TaskListTypeDef],  # (1)
    defaultTaskPriority: NotRequired[str],
    defaultTaskScheduleToStartTimeout: NotRequired[str],
    defaultTaskScheduleToCloseTimeout: NotRequired[str],
```

1. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
## ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef

```python
# ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef definition

class ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef(TypedDict):
    input: NotRequired[str],
    executionStartToCloseTimeout: NotRequired[str],
    taskList: NotRequired[TaskListTypeDef],  # (1)
    taskPriority: NotRequired[str],
    taskStartToCloseTimeout: NotRequired[str],
    childPolicy: NotRequired[ChildPolicyType],  # (2)
    tagList: NotRequired[Sequence[str]],
    workflowTypeVersion: NotRequired[str],
    lambdaRole: NotRequired[str],
```

1. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
2. See [:material-code-brackets: ChildPolicyType](./literals.md#childpolicytype) 
## CountPendingActivityTasksInputRequestTypeDef

```python
# CountPendingActivityTasksInputRequestTypeDef definition

class CountPendingActivityTasksInputRequestTypeDef(TypedDict):
    domain: str,
    taskList: TaskListTypeDef,  # (1)
```

1. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
## CountPendingDecisionTasksInputRequestTypeDef

```python
# CountPendingDecisionTasksInputRequestTypeDef definition

class CountPendingDecisionTasksInputRequestTypeDef(TypedDict):
    domain: str,
    taskList: TaskListTypeDef,  # (1)
```

1. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
## DecisionTaskCompletedEventAttributesTypeDef

```python
# DecisionTaskCompletedEventAttributesTypeDef definition

class DecisionTaskCompletedEventAttributesTypeDef(TypedDict):
    scheduledEventId: int,
    startedEventId: int,
    executionContext: NotRequired[str],
    taskList: NotRequired[TaskListTypeDef],  # (1)
    taskListScheduleToStartTimeout: NotRequired[str],
```

1. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
## DecisionTaskScheduledEventAttributesTypeDef

```python
# DecisionTaskScheduledEventAttributesTypeDef definition

class DecisionTaskScheduledEventAttributesTypeDef(TypedDict):
    taskList: TaskListTypeDef,  # (1)
    taskPriority: NotRequired[str],
    startToCloseTimeout: NotRequired[str],
    scheduleToStartTimeout: NotRequired[str],
```

1. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
## PollForActivityTaskInputRequestTypeDef

```python
# PollForActivityTaskInputRequestTypeDef definition

class PollForActivityTaskInputRequestTypeDef(TypedDict):
    domain: str,
    taskList: TaskListTypeDef,  # (1)
    identity: NotRequired[str],
```

1. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
## PollForDecisionTaskInputRequestTypeDef

```python
# PollForDecisionTaskInputRequestTypeDef definition

class PollForDecisionTaskInputRequestTypeDef(TypedDict):
    domain: str,
    taskList: TaskListTypeDef,  # (1)
    identity: NotRequired[str],
    nextPageToken: NotRequired[str],
    maximumPageSize: NotRequired[int],
    reverseOrder: NotRequired[bool],
    startAtPreviousStartedEvent: NotRequired[bool],
```

1. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
## RegisterActivityTypeInputRequestTypeDef

```python
# RegisterActivityTypeInputRequestTypeDef definition

class RegisterActivityTypeInputRequestTypeDef(TypedDict):
    domain: str,
    name: str,
    version: str,
    description: NotRequired[str],
    defaultTaskStartToCloseTimeout: NotRequired[str],
    defaultTaskHeartbeatTimeout: NotRequired[str],
    defaultTaskList: NotRequired[TaskListTypeDef],  # (1)
    defaultTaskPriority: NotRequired[str],
    defaultTaskScheduleToStartTimeout: NotRequired[str],
    defaultTaskScheduleToCloseTimeout: NotRequired[str],
```

1. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
## RegisterWorkflowTypeInputRequestTypeDef

```python
# RegisterWorkflowTypeInputRequestTypeDef definition

class RegisterWorkflowTypeInputRequestTypeDef(TypedDict):
    domain: str,
    name: str,
    version: str,
    description: NotRequired[str],
    defaultTaskStartToCloseTimeout: NotRequired[str],
    defaultExecutionStartToCloseTimeout: NotRequired[str],
    defaultTaskList: NotRequired[TaskListTypeDef],  # (1)
    defaultTaskPriority: NotRequired[str],
    defaultChildPolicy: NotRequired[ChildPolicyType],  # (2)
    defaultLambdaRole: NotRequired[str],
```

1. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
2. See [:material-code-brackets: ChildPolicyType](./literals.md#childpolicytype) 
## ScheduleActivityTaskDecisionAttributesTypeDef

```python
# ScheduleActivityTaskDecisionAttributesTypeDef definition

class ScheduleActivityTaskDecisionAttributesTypeDef(TypedDict):
    activityType: ActivityTypeTypeDef,  # (1)
    activityId: str,
    control: NotRequired[str],
    input: NotRequired[str],
    scheduleToCloseTimeout: NotRequired[str],
    taskList: NotRequired[TaskListTypeDef],  # (2)
    taskPriority: NotRequired[str],
    scheduleToStartTimeout: NotRequired[str],
    startToCloseTimeout: NotRequired[str],
    heartbeatTimeout: NotRequired[str],
```

1. See [:material-code-braces: ActivityTypeTypeDef](./type_defs.md#activitytypetypedef) 
2. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
## WorkflowExecutionConfigurationTypeDef

```python
# WorkflowExecutionConfigurationTypeDef definition

class WorkflowExecutionConfigurationTypeDef(TypedDict):
    taskStartToCloseTimeout: str,
    executionStartToCloseTimeout: str,
    taskList: TaskListTypeDef,  # (1)
    childPolicy: ChildPolicyType,  # (2)
    taskPriority: NotRequired[str],
    lambdaRole: NotRequired[str],
```

1. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
2. See [:material-code-brackets: ChildPolicyType](./literals.md#childpolicytype) 
## WorkflowTypeConfigurationTypeDef

```python
# WorkflowTypeConfigurationTypeDef definition

class WorkflowTypeConfigurationTypeDef(TypedDict):
    defaultTaskStartToCloseTimeout: NotRequired[str],
    defaultExecutionStartToCloseTimeout: NotRequired[str],
    defaultTaskList: NotRequired[TaskListTypeDef],  # (1)
    defaultTaskPriority: NotRequired[str],
    defaultChildPolicy: NotRequired[ChildPolicyType],  # (2)
    defaultLambdaRole: NotRequired[str],
```

1. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
2. See [:material-code-brackets: ChildPolicyType](./literals.md#childpolicytype) 
## ActivityTaskStatusTypeDef

```python
# ActivityTaskStatusTypeDef definition

class ActivityTaskStatusTypeDef(TypedDict):
    cancelRequested: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PendingTaskCountTypeDef

```python
# PendingTaskCountTypeDef definition

class PendingTaskCountTypeDef(TypedDict):
    count: int,
    truncated: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RunTypeDef

```python
# RunTypeDef definition

class RunTypeDef(TypedDict):
    runId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkflowExecutionCountTypeDef

```python
# WorkflowExecutionCountTypeDef definition

class WorkflowExecutionCountTypeDef(TypedDict):
    count: int,
    truncated: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ActivityTaskTypeDef

```python
# ActivityTaskTypeDef definition

class ActivityTaskTypeDef(TypedDict):
    taskToken: str,
    activityId: str,
    startedEventId: int,
    workflowExecution: WorkflowExecutionTypeDef,  # (1)
    activityType: ActivityTypeTypeDef,  # (2)
    input: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: WorkflowExecutionTypeDef](./type_defs.md#workflowexecutiontypedef) 
2. See [:material-code-braces: ActivityTypeTypeDef](./type_defs.md#activitytypetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWorkflowExecutionInputRequestTypeDef

```python
# DescribeWorkflowExecutionInputRequestTypeDef definition

class DescribeWorkflowExecutionInputRequestTypeDef(TypedDict):
    domain: str,
    execution: WorkflowExecutionTypeDef,  # (1)
```

1. See [:material-code-braces: WorkflowExecutionTypeDef](./type_defs.md#workflowexecutiontypedef) 
## ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef

```python
# ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef definition

class ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef(TypedDict):
    workflowExecution: WorkflowExecutionTypeDef,  # (1)
    initiatedEventId: int,
```

1. See [:material-code-braces: WorkflowExecutionTypeDef](./type_defs.md#workflowexecutiontypedef) 
## ExternalWorkflowExecutionSignaledEventAttributesTypeDef

```python
# ExternalWorkflowExecutionSignaledEventAttributesTypeDef definition

class ExternalWorkflowExecutionSignaledEventAttributesTypeDef(TypedDict):
    workflowExecution: WorkflowExecutionTypeDef,  # (1)
    initiatedEventId: int,
```

1. See [:material-code-braces: WorkflowExecutionTypeDef](./type_defs.md#workflowexecutiontypedef) 
## GetWorkflowExecutionHistoryInputRequestTypeDef

```python
# GetWorkflowExecutionHistoryInputRequestTypeDef definition

class GetWorkflowExecutionHistoryInputRequestTypeDef(TypedDict):
    domain: str,
    execution: WorkflowExecutionTypeDef,  # (1)
    nextPageToken: NotRequired[str],
    maximumPageSize: NotRequired[int],
    reverseOrder: NotRequired[bool],
```

1. See [:material-code-braces: WorkflowExecutionTypeDef](./type_defs.md#workflowexecutiontypedef) 
## WorkflowExecutionCancelRequestedEventAttributesTypeDef

```python
# WorkflowExecutionCancelRequestedEventAttributesTypeDef definition

class WorkflowExecutionCancelRequestedEventAttributesTypeDef(TypedDict):
    externalWorkflowExecution: NotRequired[WorkflowExecutionTypeDef],  # (1)
    externalInitiatedEventId: NotRequired[int],
    cause: NotRequired[WorkflowExecutionCancelRequestedCauseType],  # (2)
```

1. See [:material-code-braces: WorkflowExecutionTypeDef](./type_defs.md#workflowexecutiontypedef) 
2. See [:material-code-brackets: WorkflowExecutionCancelRequestedCauseType](./literals.md#workflowexecutioncancelrequestedcausetype) 
## WorkflowExecutionSignaledEventAttributesTypeDef

```python
# WorkflowExecutionSignaledEventAttributesTypeDef definition

class WorkflowExecutionSignaledEventAttributesTypeDef(TypedDict):
    signalName: str,
    input: NotRequired[str],
    externalWorkflowExecution: NotRequired[WorkflowExecutionTypeDef],  # (1)
    externalInitiatedEventId: NotRequired[int],
```

1. See [:material-code-braces: WorkflowExecutionTypeDef](./type_defs.md#workflowexecutiontypedef) 
## ChildWorkflowExecutionCanceledEventAttributesTypeDef

```python
# ChildWorkflowExecutionCanceledEventAttributesTypeDef definition

class ChildWorkflowExecutionCanceledEventAttributesTypeDef(TypedDict):
    workflowExecution: WorkflowExecutionTypeDef,  # (1)
    workflowType: WorkflowTypeTypeDef,  # (2)
    initiatedEventId: int,
    startedEventId: int,
    details: NotRequired[str],
```

1. See [:material-code-braces: WorkflowExecutionTypeDef](./type_defs.md#workflowexecutiontypedef) 
2. See [:material-code-braces: WorkflowTypeTypeDef](./type_defs.md#workflowtypetypedef) 
## ChildWorkflowExecutionCompletedEventAttributesTypeDef

```python
# ChildWorkflowExecutionCompletedEventAttributesTypeDef definition

class ChildWorkflowExecutionCompletedEventAttributesTypeDef(TypedDict):
    workflowExecution: WorkflowExecutionTypeDef,  # (1)
    workflowType: WorkflowTypeTypeDef,  # (2)
    initiatedEventId: int,
    startedEventId: int,
    result: NotRequired[str],
```

1. See [:material-code-braces: WorkflowExecutionTypeDef](./type_defs.md#workflowexecutiontypedef) 
2. See [:material-code-braces: WorkflowTypeTypeDef](./type_defs.md#workflowtypetypedef) 
## ChildWorkflowExecutionFailedEventAttributesTypeDef

```python
# ChildWorkflowExecutionFailedEventAttributesTypeDef definition

class ChildWorkflowExecutionFailedEventAttributesTypeDef(TypedDict):
    workflowExecution: WorkflowExecutionTypeDef,  # (1)
    workflowType: WorkflowTypeTypeDef,  # (2)
    initiatedEventId: int,
    startedEventId: int,
    reason: NotRequired[str],
    details: NotRequired[str],
```

1. See [:material-code-braces: WorkflowExecutionTypeDef](./type_defs.md#workflowexecutiontypedef) 
2. See [:material-code-braces: WorkflowTypeTypeDef](./type_defs.md#workflowtypetypedef) 
## ChildWorkflowExecutionStartedEventAttributesTypeDef

```python
# ChildWorkflowExecutionStartedEventAttributesTypeDef definition

class ChildWorkflowExecutionStartedEventAttributesTypeDef(TypedDict):
    workflowExecution: WorkflowExecutionTypeDef,  # (1)
    workflowType: WorkflowTypeTypeDef,  # (2)
    initiatedEventId: int,
```

1. See [:material-code-braces: WorkflowExecutionTypeDef](./type_defs.md#workflowexecutiontypedef) 
2. See [:material-code-braces: WorkflowTypeTypeDef](./type_defs.md#workflowtypetypedef) 
## ChildWorkflowExecutionTerminatedEventAttributesTypeDef

```python
# ChildWorkflowExecutionTerminatedEventAttributesTypeDef definition

class ChildWorkflowExecutionTerminatedEventAttributesTypeDef(TypedDict):
    workflowExecution: WorkflowExecutionTypeDef,  # (1)
    workflowType: WorkflowTypeTypeDef,  # (2)
    initiatedEventId: int,
    startedEventId: int,
```

1. See [:material-code-braces: WorkflowExecutionTypeDef](./type_defs.md#workflowexecutiontypedef) 
2. See [:material-code-braces: WorkflowTypeTypeDef](./type_defs.md#workflowtypetypedef) 
## ChildWorkflowExecutionTimedOutEventAttributesTypeDef

```python
# ChildWorkflowExecutionTimedOutEventAttributesTypeDef definition

class ChildWorkflowExecutionTimedOutEventAttributesTypeDef(TypedDict):
    workflowExecution: WorkflowExecutionTypeDef,  # (1)
    workflowType: WorkflowTypeTypeDef,  # (2)
    timeoutType: WorkflowExecutionTimeoutTypeType,  # (3)
    initiatedEventId: int,
    startedEventId: int,
```

1. See [:material-code-braces: WorkflowExecutionTypeDef](./type_defs.md#workflowexecutiontypedef) 
2. See [:material-code-braces: WorkflowTypeTypeDef](./type_defs.md#workflowtypetypedef) 
3. See [:material-code-brackets: WorkflowExecutionTimeoutTypeType](./literals.md#workflowexecutiontimeouttypetype) 
## DeleteWorkflowTypeInputRequestTypeDef

```python
# DeleteWorkflowTypeInputRequestTypeDef definition

class DeleteWorkflowTypeInputRequestTypeDef(TypedDict):
    domain: str,
    workflowType: WorkflowTypeTypeDef,  # (1)
```

1. See [:material-code-braces: WorkflowTypeTypeDef](./type_defs.md#workflowtypetypedef) 
## DeprecateWorkflowTypeInputRequestTypeDef

```python
# DeprecateWorkflowTypeInputRequestTypeDef definition

class DeprecateWorkflowTypeInputRequestTypeDef(TypedDict):
    domain: str,
    workflowType: WorkflowTypeTypeDef,  # (1)
```

1. See [:material-code-braces: WorkflowTypeTypeDef](./type_defs.md#workflowtypetypedef) 
## DescribeWorkflowTypeInputRequestTypeDef

```python
# DescribeWorkflowTypeInputRequestTypeDef definition

class DescribeWorkflowTypeInputRequestTypeDef(TypedDict):
    domain: str,
    workflowType: WorkflowTypeTypeDef,  # (1)
```

1. See [:material-code-braces: WorkflowTypeTypeDef](./type_defs.md#workflowtypetypedef) 
## StartChildWorkflowExecutionDecisionAttributesTypeDef

```python
# StartChildWorkflowExecutionDecisionAttributesTypeDef definition

class StartChildWorkflowExecutionDecisionAttributesTypeDef(TypedDict):
    workflowType: WorkflowTypeTypeDef,  # (1)
    workflowId: str,
    control: NotRequired[str],
    input: NotRequired[str],
    executionStartToCloseTimeout: NotRequired[str],
    taskList: NotRequired[TaskListTypeDef],  # (2)
    taskPriority: NotRequired[str],
    taskStartToCloseTimeout: NotRequired[str],
    childPolicy: NotRequired[ChildPolicyType],  # (3)
    tagList: NotRequired[Sequence[str]],
    lambdaRole: NotRequired[str],
```

1. See [:material-code-braces: WorkflowTypeTypeDef](./type_defs.md#workflowtypetypedef) 
2. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
3. See [:material-code-brackets: ChildPolicyType](./literals.md#childpolicytype) 
## StartChildWorkflowExecutionFailedEventAttributesTypeDef

```python
# StartChildWorkflowExecutionFailedEventAttributesTypeDef definition

class StartChildWorkflowExecutionFailedEventAttributesTypeDef(TypedDict):
    workflowType: WorkflowTypeTypeDef,  # (1)
    cause: StartChildWorkflowExecutionFailedCauseType,  # (2)
    workflowId: str,
    initiatedEventId: int,
    decisionTaskCompletedEventId: int,
    control: NotRequired[str],
```

1. See [:material-code-braces: WorkflowTypeTypeDef](./type_defs.md#workflowtypetypedef) 
2. See [:material-code-brackets: StartChildWorkflowExecutionFailedCauseType](./literals.md#startchildworkflowexecutionfailedcausetype) 
## StartChildWorkflowExecutionInitiatedEventAttributesTypeDef

```python
# StartChildWorkflowExecutionInitiatedEventAttributesTypeDef definition

class StartChildWorkflowExecutionInitiatedEventAttributesTypeDef(TypedDict):
    workflowId: str,
    workflowType: WorkflowTypeTypeDef,  # (1)
    taskList: TaskListTypeDef,  # (2)
    decisionTaskCompletedEventId: int,
    childPolicy: ChildPolicyType,  # (3)
    control: NotRequired[str],
    input: NotRequired[str],
    executionStartToCloseTimeout: NotRequired[str],
    taskPriority: NotRequired[str],
    taskStartToCloseTimeout: NotRequired[str],
    tagList: NotRequired[List[str]],
    lambdaRole: NotRequired[str],
```

1. See [:material-code-braces: WorkflowTypeTypeDef](./type_defs.md#workflowtypetypedef) 
2. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
3. See [:material-code-brackets: ChildPolicyType](./literals.md#childpolicytype) 
## StartWorkflowExecutionInputRequestTypeDef

```python
# StartWorkflowExecutionInputRequestTypeDef definition

class StartWorkflowExecutionInputRequestTypeDef(TypedDict):
    domain: str,
    workflowId: str,
    workflowType: WorkflowTypeTypeDef,  # (1)
    taskList: NotRequired[TaskListTypeDef],  # (2)
    taskPriority: NotRequired[str],
    input: NotRequired[str],
    executionStartToCloseTimeout: NotRequired[str],
    tagList: NotRequired[Sequence[str]],
    taskStartToCloseTimeout: NotRequired[str],
    childPolicy: NotRequired[ChildPolicyType],  # (3)
    lambdaRole: NotRequired[str],
```

1. See [:material-code-braces: WorkflowTypeTypeDef](./type_defs.md#workflowtypetypedef) 
2. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
3. See [:material-code-brackets: ChildPolicyType](./literals.md#childpolicytype) 
## UndeprecateWorkflowTypeInputRequestTypeDef

```python
# UndeprecateWorkflowTypeInputRequestTypeDef definition

class UndeprecateWorkflowTypeInputRequestTypeDef(TypedDict):
    domain: str,
    workflowType: WorkflowTypeTypeDef,  # (1)
```

1. See [:material-code-braces: WorkflowTypeTypeDef](./type_defs.md#workflowtypetypedef) 
## WorkflowExecutionContinuedAsNewEventAttributesTypeDef

```python
# WorkflowExecutionContinuedAsNewEventAttributesTypeDef definition

class WorkflowExecutionContinuedAsNewEventAttributesTypeDef(TypedDict):
    decisionTaskCompletedEventId: int,
    newExecutionRunId: str,
    taskList: TaskListTypeDef,  # (1)
    childPolicy: ChildPolicyType,  # (2)
    workflowType: WorkflowTypeTypeDef,  # (3)
    input: NotRequired[str],
    executionStartToCloseTimeout: NotRequired[str],
    taskPriority: NotRequired[str],
    taskStartToCloseTimeout: NotRequired[str],
    tagList: NotRequired[List[str]],
    lambdaRole: NotRequired[str],
```

1. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
2. See [:material-code-brackets: ChildPolicyType](./literals.md#childpolicytype) 
3. See [:material-code-braces: WorkflowTypeTypeDef](./type_defs.md#workflowtypetypedef) 
## WorkflowExecutionInfoTypeDef

```python
# WorkflowExecutionInfoTypeDef definition

class WorkflowExecutionInfoTypeDef(TypedDict):
    execution: WorkflowExecutionTypeDef,  # (1)
    workflowType: WorkflowTypeTypeDef,  # (2)
    startTimestamp: datetime,
    executionStatus: ExecutionStatusType,  # (3)
    closeTimestamp: NotRequired[datetime],
    closeStatus: NotRequired[CloseStatusType],  # (4)
    parent: NotRequired[WorkflowExecutionTypeDef],  # (1)
    tagList: NotRequired[List[str]],
    cancelRequested: NotRequired[bool],
```

1. See [:material-code-braces: WorkflowExecutionTypeDef](./type_defs.md#workflowexecutiontypedef) 
2. See [:material-code-braces: WorkflowTypeTypeDef](./type_defs.md#workflowtypetypedef) 
3. See [:material-code-brackets: ExecutionStatusType](./literals.md#executionstatustype) 
4. See [:material-code-brackets: CloseStatusType](./literals.md#closestatustype) 
5. See [:material-code-braces: WorkflowExecutionTypeDef](./type_defs.md#workflowexecutiontypedef) 
## WorkflowExecutionStartedEventAttributesTypeDef

```python
# WorkflowExecutionStartedEventAttributesTypeDef definition

class WorkflowExecutionStartedEventAttributesTypeDef(TypedDict):
    childPolicy: ChildPolicyType,  # (1)
    taskList: TaskListTypeDef,  # (2)
    workflowType: WorkflowTypeTypeDef,  # (3)
    input: NotRequired[str],
    executionStartToCloseTimeout: NotRequired[str],
    taskStartToCloseTimeout: NotRequired[str],
    taskPriority: NotRequired[str],
    tagList: NotRequired[List[str]],
    continuedExecutionRunId: NotRequired[str],
    parentWorkflowExecution: NotRequired[WorkflowExecutionTypeDef],  # (4)
    parentInitiatedEventId: NotRequired[int],
    lambdaRole: NotRequired[str],
```

1. See [:material-code-brackets: ChildPolicyType](./literals.md#childpolicytype) 
2. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
3. See [:material-code-braces: WorkflowTypeTypeDef](./type_defs.md#workflowtypetypedef) 
4. See [:material-code-braces: WorkflowExecutionTypeDef](./type_defs.md#workflowexecutiontypedef) 
## WorkflowTypeInfoTypeDef

```python
# WorkflowTypeInfoTypeDef definition

class WorkflowTypeInfoTypeDef(TypedDict):
    workflowType: WorkflowTypeTypeDef,  # (1)
    status: RegistrationStatusType,  # (2)
    creationDate: datetime,
    description: NotRequired[str],
    deprecationDate: NotRequired[datetime],
```

1. See [:material-code-braces: WorkflowTypeTypeDef](./type_defs.md#workflowtypetypedef) 
2. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
## DomainDetailTypeDef

```python
# DomainDetailTypeDef definition

class DomainDetailTypeDef(TypedDict):
    domainInfo: DomainInfoTypeDef,  # (1)
    configuration: DomainConfigurationTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DomainInfoTypeDef](./type_defs.md#domaininfotypedef) 
2. See [:material-code-braces: DomainConfigurationTypeDef](./type_defs.md#domainconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DomainInfosTypeDef

```python
# DomainInfosTypeDef definition

class DomainInfosTypeDef(TypedDict):
    domainInfos: List[DomainInfoTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainInfoTypeDef](./type_defs.md#domaininfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecutionTimeFilterTypeDef

```python
# ExecutionTimeFilterTypeDef definition

class ExecutionTimeFilterTypeDef(TypedDict):
    oldestDate: TimestampTypeDef,
    latestDate: NotRequired[TimestampTypeDef],
```

## GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef

```python
# GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef definition

class GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef(TypedDict):
    domain: str,
    execution: WorkflowExecutionTypeDef,  # (1)
    reverseOrder: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: WorkflowExecutionTypeDef](./type_defs.md#workflowexecutiontypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListActivityTypesInputListActivityTypesPaginateTypeDef

```python
# ListActivityTypesInputListActivityTypesPaginateTypeDef definition

class ListActivityTypesInputListActivityTypesPaginateTypeDef(TypedDict):
    domain: str,
    registrationStatus: RegistrationStatusType,  # (1)
    name: NotRequired[str],
    reverseOrder: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDomainsInputListDomainsPaginateTypeDef

```python
# ListDomainsInputListDomainsPaginateTypeDef definition

class ListDomainsInputListDomainsPaginateTypeDef(TypedDict):
    registrationStatus: RegistrationStatusType,  # (1)
    reverseOrder: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef

```python
# ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef definition

class ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef(TypedDict):
    domain: str,
    registrationStatus: RegistrationStatusType,  # (1)
    name: NotRequired[str],
    reverseOrder: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef

```python
# PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef definition

class PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef(TypedDict):
    domain: str,
    taskList: TaskListTypeDef,  # (1)
    identity: NotRequired[str],
    reverseOrder: NotRequired[bool],
    startAtPreviousStartedEvent: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    tags: List[ResourceTagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterDomainInputRequestTypeDef

```python
# RegisterDomainInputRequestTypeDef definition

class RegisterDomainInputRequestTypeDef(TypedDict):
    name: str,
    workflowExecutionRetentionPeriodInDays: str,
    description: NotRequired[str],
    tags: NotRequired[Sequence[ResourceTagTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[ResourceTagTypeDef],  # (1)
```

1. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
## ActivityTypeInfosTypeDef

```python
# ActivityTypeInfosTypeDef definition

class ActivityTypeInfosTypeDef(TypedDict):
    typeInfos: List[ActivityTypeInfoTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActivityTypeInfoTypeDef](./type_defs.md#activitytypeinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ActivityTypeDetailTypeDef

```python
# ActivityTypeDetailTypeDef definition

class ActivityTypeDetailTypeDef(TypedDict):
    typeInfo: ActivityTypeInfoTypeDef,  # (1)
    configuration: ActivityTypeConfigurationTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ActivityTypeInfoTypeDef](./type_defs.md#activitytypeinfotypedef) 
2. See [:material-code-braces: ActivityTypeConfigurationTypeDef](./type_defs.md#activitytypeconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DecisionTypeDef

```python
# DecisionTypeDef definition

class DecisionTypeDef(TypedDict):
    decisionType: DecisionTypeType,  # (1)
    scheduleActivityTaskDecisionAttributes: NotRequired[ScheduleActivityTaskDecisionAttributesTypeDef],  # (2)
    requestCancelActivityTaskDecisionAttributes: NotRequired[RequestCancelActivityTaskDecisionAttributesTypeDef],  # (3)
    completeWorkflowExecutionDecisionAttributes: NotRequired[CompleteWorkflowExecutionDecisionAttributesTypeDef],  # (4)
    failWorkflowExecutionDecisionAttributes: NotRequired[FailWorkflowExecutionDecisionAttributesTypeDef],  # (5)
    cancelWorkflowExecutionDecisionAttributes: NotRequired[CancelWorkflowExecutionDecisionAttributesTypeDef],  # (6)
    continueAsNewWorkflowExecutionDecisionAttributes: NotRequired[ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef],  # (7)
    recordMarkerDecisionAttributes: NotRequired[RecordMarkerDecisionAttributesTypeDef],  # (8)
    startTimerDecisionAttributes: NotRequired[StartTimerDecisionAttributesTypeDef],  # (9)
    cancelTimerDecisionAttributes: NotRequired[CancelTimerDecisionAttributesTypeDef],  # (10)
    signalExternalWorkflowExecutionDecisionAttributes: NotRequired[SignalExternalWorkflowExecutionDecisionAttributesTypeDef],  # (11)
    requestCancelExternalWorkflowExecutionDecisionAttributes: NotRequired[RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef],  # (12)
    startChildWorkflowExecutionDecisionAttributes: NotRequired[StartChildWorkflowExecutionDecisionAttributesTypeDef],  # (13)
    scheduleLambdaFunctionDecisionAttributes: NotRequired[ScheduleLambdaFunctionDecisionAttributesTypeDef],  # (14)
```

1. See [:material-code-brackets: DecisionTypeType](./literals.md#decisiontypetype) 
2. See [:material-code-braces: ScheduleActivityTaskDecisionAttributesTypeDef](./type_defs.md#scheduleactivitytaskdecisionattributestypedef) 
3. See [:material-code-braces: RequestCancelActivityTaskDecisionAttributesTypeDef](./type_defs.md#requestcancelactivitytaskdecisionattributestypedef) 
4. See [:material-code-braces: CompleteWorkflowExecutionDecisionAttributesTypeDef](./type_defs.md#completeworkflowexecutiondecisionattributestypedef) 
5. See [:material-code-braces: FailWorkflowExecutionDecisionAttributesTypeDef](./type_defs.md#failworkflowexecutiondecisionattributestypedef) 
6. See [:material-code-braces: CancelWorkflowExecutionDecisionAttributesTypeDef](./type_defs.md#cancelworkflowexecutiondecisionattributestypedef) 
7. See [:material-code-braces: ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef](./type_defs.md#continueasnewworkflowexecutiondecisionattributestypedef) 
8. See [:material-code-braces: RecordMarkerDecisionAttributesTypeDef](./type_defs.md#recordmarkerdecisionattributestypedef) 
9. See [:material-code-braces: StartTimerDecisionAttributesTypeDef](./type_defs.md#starttimerdecisionattributestypedef) 
10. See [:material-code-braces: CancelTimerDecisionAttributesTypeDef](./type_defs.md#canceltimerdecisionattributestypedef) 
11. See [:material-code-braces: SignalExternalWorkflowExecutionDecisionAttributesTypeDef](./type_defs.md#signalexternalworkflowexecutiondecisionattributestypedef) 
12. See [:material-code-braces: RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef](./type_defs.md#requestcancelexternalworkflowexecutiondecisionattributestypedef) 
13. See [:material-code-braces: StartChildWorkflowExecutionDecisionAttributesTypeDef](./type_defs.md#startchildworkflowexecutiondecisionattributestypedef) 
14. See [:material-code-braces: ScheduleLambdaFunctionDecisionAttributesTypeDef](./type_defs.md#schedulelambdafunctiondecisionattributestypedef) 
## WorkflowExecutionDetailTypeDef

```python
# WorkflowExecutionDetailTypeDef definition

class WorkflowExecutionDetailTypeDef(TypedDict):
    executionInfo: WorkflowExecutionInfoTypeDef,  # (1)
    executionConfiguration: WorkflowExecutionConfigurationTypeDef,  # (2)
    openCounts: WorkflowExecutionOpenCountsTypeDef,  # (3)
    latestActivityTaskTimestamp: datetime,
    latestExecutionContext: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: WorkflowExecutionInfoTypeDef](./type_defs.md#workflowexecutioninfotypedef) 
2. See [:material-code-braces: WorkflowExecutionConfigurationTypeDef](./type_defs.md#workflowexecutionconfigurationtypedef) 
3. See [:material-code-braces: WorkflowExecutionOpenCountsTypeDef](./type_defs.md#workflowexecutionopencountstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkflowExecutionInfosTypeDef

```python
# WorkflowExecutionInfosTypeDef definition

class WorkflowExecutionInfosTypeDef(TypedDict):
    executionInfos: List[WorkflowExecutionInfoTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkflowExecutionInfoTypeDef](./type_defs.md#workflowexecutioninfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HistoryEventTypeDef

```python
# HistoryEventTypeDef definition

class HistoryEventTypeDef(TypedDict):
    eventTimestamp: datetime,
    eventType: EventTypeType,  # (1)
    eventId: int,
    workflowExecutionStartedEventAttributes: NotRequired[WorkflowExecutionStartedEventAttributesTypeDef],  # (2)
    workflowExecutionCompletedEventAttributes: NotRequired[WorkflowExecutionCompletedEventAttributesTypeDef],  # (3)
    completeWorkflowExecutionFailedEventAttributes: NotRequired[CompleteWorkflowExecutionFailedEventAttributesTypeDef],  # (4)
    workflowExecutionFailedEventAttributes: NotRequired[WorkflowExecutionFailedEventAttributesTypeDef],  # (5)
    failWorkflowExecutionFailedEventAttributes: NotRequired[FailWorkflowExecutionFailedEventAttributesTypeDef],  # (6)
    workflowExecutionTimedOutEventAttributes: NotRequired[WorkflowExecutionTimedOutEventAttributesTypeDef],  # (7)
    workflowExecutionCanceledEventAttributes: NotRequired[WorkflowExecutionCanceledEventAttributesTypeDef],  # (8)
    cancelWorkflowExecutionFailedEventAttributes: NotRequired[CancelWorkflowExecutionFailedEventAttributesTypeDef],  # (9)
    workflowExecutionContinuedAsNewEventAttributes: NotRequired[WorkflowExecutionContinuedAsNewEventAttributesTypeDef],  # (10)
    continueAsNewWorkflowExecutionFailedEventAttributes: NotRequired[ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef],  # (11)
    workflowExecutionTerminatedEventAttributes: NotRequired[WorkflowExecutionTerminatedEventAttributesTypeDef],  # (12)
    workflowExecutionCancelRequestedEventAttributes: NotRequired[WorkflowExecutionCancelRequestedEventAttributesTypeDef],  # (13)
    decisionTaskScheduledEventAttributes: NotRequired[DecisionTaskScheduledEventAttributesTypeDef],  # (14)
    decisionTaskStartedEventAttributes: NotRequired[DecisionTaskStartedEventAttributesTypeDef],  # (15)
    decisionTaskCompletedEventAttributes: NotRequired[DecisionTaskCompletedEventAttributesTypeDef],  # (16)
    decisionTaskTimedOutEventAttributes: NotRequired[DecisionTaskTimedOutEventAttributesTypeDef],  # (17)
    activityTaskScheduledEventAttributes: NotRequired[ActivityTaskScheduledEventAttributesTypeDef],  # (18)
    activityTaskStartedEventAttributes: NotRequired[ActivityTaskStartedEventAttributesTypeDef],  # (19)
    activityTaskCompletedEventAttributes: NotRequired[ActivityTaskCompletedEventAttributesTypeDef],  # (20)
    activityTaskFailedEventAttributes: NotRequired[ActivityTaskFailedEventAttributesTypeDef],  # (21)
    activityTaskTimedOutEventAttributes: NotRequired[ActivityTaskTimedOutEventAttributesTypeDef],  # (22)
    activityTaskCanceledEventAttributes: NotRequired[ActivityTaskCanceledEventAttributesTypeDef],  # (23)
    activityTaskCancelRequestedEventAttributes: NotRequired[ActivityTaskCancelRequestedEventAttributesTypeDef],  # (24)
    workflowExecutionSignaledEventAttributes: NotRequired[WorkflowExecutionSignaledEventAttributesTypeDef],  # (25)
    markerRecordedEventAttributes: NotRequired[MarkerRecordedEventAttributesTypeDef],  # (26)
    recordMarkerFailedEventAttributes: NotRequired[RecordMarkerFailedEventAttributesTypeDef],  # (27)
    timerStartedEventAttributes: NotRequired[TimerStartedEventAttributesTypeDef],  # (28)
    timerFiredEventAttributes: NotRequired[TimerFiredEventAttributesTypeDef],  # (29)
    timerCanceledEventAttributes: NotRequired[TimerCanceledEventAttributesTypeDef],  # (30)
    startChildWorkflowExecutionInitiatedEventAttributes: NotRequired[StartChildWorkflowExecutionInitiatedEventAttributesTypeDef],  # (31)
    childWorkflowExecutionStartedEventAttributes: NotRequired[ChildWorkflowExecutionStartedEventAttributesTypeDef],  # (32)
    childWorkflowExecutionCompletedEventAttributes: NotRequired[ChildWorkflowExecutionCompletedEventAttributesTypeDef],  # (33)
    childWorkflowExecutionFailedEventAttributes: NotRequired[ChildWorkflowExecutionFailedEventAttributesTypeDef],  # (34)
    childWorkflowExecutionTimedOutEventAttributes: NotRequired[ChildWorkflowExecutionTimedOutEventAttributesTypeDef],  # (35)
    childWorkflowExecutionCanceledEventAttributes: NotRequired[ChildWorkflowExecutionCanceledEventAttributesTypeDef],  # (36)
    childWorkflowExecutionTerminatedEventAttributes: NotRequired[ChildWorkflowExecutionTerminatedEventAttributesTypeDef],  # (37)
    signalExternalWorkflowExecutionInitiatedEventAttributes: NotRequired[SignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef],  # (38)
    externalWorkflowExecutionSignaledEventAttributes: NotRequired[ExternalWorkflowExecutionSignaledEventAttributesTypeDef],  # (39)
    signalExternalWorkflowExecutionFailedEventAttributes: NotRequired[SignalExternalWorkflowExecutionFailedEventAttributesTypeDef],  # (40)
    externalWorkflowExecutionCancelRequestedEventAttributes: NotRequired[ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef],  # (41)
    requestCancelExternalWorkflowExecutionInitiatedEventAttributes: NotRequired[RequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef],  # (42)
    requestCancelExternalWorkflowExecutionFailedEventAttributes: NotRequired[RequestCancelExternalWorkflowExecutionFailedEventAttributesTypeDef],  # (43)
    scheduleActivityTaskFailedEventAttributes: NotRequired[ScheduleActivityTaskFailedEventAttributesTypeDef],  # (44)
    requestCancelActivityTaskFailedEventAttributes: NotRequired[RequestCancelActivityTaskFailedEventAttributesTypeDef],  # (45)
    startTimerFailedEventAttributes: NotRequired[StartTimerFailedEventAttributesTypeDef],  # (46)
    cancelTimerFailedEventAttributes: NotRequired[CancelTimerFailedEventAttributesTypeDef],  # (47)
    startChildWorkflowExecutionFailedEventAttributes: NotRequired[StartChildWorkflowExecutionFailedEventAttributesTypeDef],  # (48)
    lambdaFunctionScheduledEventAttributes: NotRequired[LambdaFunctionScheduledEventAttributesTypeDef],  # (49)
    lambdaFunctionStartedEventAttributes: NotRequired[LambdaFunctionStartedEventAttributesTypeDef],  # (50)
    lambdaFunctionCompletedEventAttributes: NotRequired[LambdaFunctionCompletedEventAttributesTypeDef],  # (51)
    lambdaFunctionFailedEventAttributes: NotRequired[LambdaFunctionFailedEventAttributesTypeDef],  # (52)
    lambdaFunctionTimedOutEventAttributes: NotRequired[LambdaFunctionTimedOutEventAttributesTypeDef],  # (53)
    scheduleLambdaFunctionFailedEventAttributes: NotRequired[ScheduleLambdaFunctionFailedEventAttributesTypeDef],  # (54)
    startLambdaFunctionFailedEventAttributes: NotRequired[StartLambdaFunctionFailedEventAttributesTypeDef],  # (55)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
2. See [:material-code-braces: WorkflowExecutionStartedEventAttributesTypeDef](./type_defs.md#workflowexecutionstartedeventattributestypedef) 
3. See [:material-code-braces: WorkflowExecutionCompletedEventAttributesTypeDef](./type_defs.md#workflowexecutioncompletedeventattributestypedef) 
4. See [:material-code-braces: CompleteWorkflowExecutionFailedEventAttributesTypeDef](./type_defs.md#completeworkflowexecutionfailedeventattributestypedef) 
5. See [:material-code-braces: WorkflowExecutionFailedEventAttributesTypeDef](./type_defs.md#workflowexecutionfailedeventattributestypedef) 
6. See [:material-code-braces: FailWorkflowExecutionFailedEventAttributesTypeDef](./type_defs.md#failworkflowexecutionfailedeventattributestypedef) 
7. See [:material-code-braces: WorkflowExecutionTimedOutEventAttributesTypeDef](./type_defs.md#workflowexecutiontimedouteventattributestypedef) 
8. See [:material-code-braces: WorkflowExecutionCanceledEventAttributesTypeDef](./type_defs.md#workflowexecutioncanceledeventattributestypedef) 
9. See [:material-code-braces: CancelWorkflowExecutionFailedEventAttributesTypeDef](./type_defs.md#cancelworkflowexecutionfailedeventattributestypedef) 
10. See [:material-code-braces: WorkflowExecutionContinuedAsNewEventAttributesTypeDef](./type_defs.md#workflowexecutioncontinuedasneweventattributestypedef) 
11. See [:material-code-braces: ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef](./type_defs.md#continueasnewworkflowexecutionfailedeventattributestypedef) 
12. See [:material-code-braces: WorkflowExecutionTerminatedEventAttributesTypeDef](./type_defs.md#workflowexecutionterminatedeventattributestypedef) 
13. See [:material-code-braces: WorkflowExecutionCancelRequestedEventAttributesTypeDef](./type_defs.md#workflowexecutioncancelrequestedeventattributestypedef) 
14. See [:material-code-braces: DecisionTaskScheduledEventAttributesTypeDef](./type_defs.md#decisiontaskscheduledeventattributestypedef) 
15. See [:material-code-braces: DecisionTaskStartedEventAttributesTypeDef](./type_defs.md#decisiontaskstartedeventattributestypedef) 
16. See [:material-code-braces: DecisionTaskCompletedEventAttributesTypeDef](./type_defs.md#decisiontaskcompletedeventattributestypedef) 
17. See [:material-code-braces: DecisionTaskTimedOutEventAttributesTypeDef](./type_defs.md#decisiontasktimedouteventattributestypedef) 
18. See [:material-code-braces: ActivityTaskScheduledEventAttributesTypeDef](./type_defs.md#activitytaskscheduledeventattributestypedef) 
19. See [:material-code-braces: ActivityTaskStartedEventAttributesTypeDef](./type_defs.md#activitytaskstartedeventattributestypedef) 
20. See [:material-code-braces: ActivityTaskCompletedEventAttributesTypeDef](./type_defs.md#activitytaskcompletedeventattributestypedef) 
21. See [:material-code-braces: ActivityTaskFailedEventAttributesTypeDef](./type_defs.md#activitytaskfailedeventattributestypedef) 
22. See [:material-code-braces: ActivityTaskTimedOutEventAttributesTypeDef](./type_defs.md#activitytasktimedouteventattributestypedef) 
23. See [:material-code-braces: ActivityTaskCanceledEventAttributesTypeDef](./type_defs.md#activitytaskcanceledeventattributestypedef) 
24. See [:material-code-braces: ActivityTaskCancelRequestedEventAttributesTypeDef](./type_defs.md#activitytaskcancelrequestedeventattributestypedef) 
25. See [:material-code-braces: WorkflowExecutionSignaledEventAttributesTypeDef](./type_defs.md#workflowexecutionsignaledeventattributestypedef) 
26. See [:material-code-braces: MarkerRecordedEventAttributesTypeDef](./type_defs.md#markerrecordedeventattributestypedef) 
27. See [:material-code-braces: RecordMarkerFailedEventAttributesTypeDef](./type_defs.md#recordmarkerfailedeventattributestypedef) 
28. See [:material-code-braces: TimerStartedEventAttributesTypeDef](./type_defs.md#timerstartedeventattributestypedef) 
29. See [:material-code-braces: TimerFiredEventAttributesTypeDef](./type_defs.md#timerfiredeventattributestypedef) 
30. See [:material-code-braces: TimerCanceledEventAttributesTypeDef](./type_defs.md#timercanceledeventattributestypedef) 
31. See [:material-code-braces: StartChildWorkflowExecutionInitiatedEventAttributesTypeDef](./type_defs.md#startchildworkflowexecutioninitiatedeventattributestypedef) 
32. See [:material-code-braces: ChildWorkflowExecutionStartedEventAttributesTypeDef](./type_defs.md#childworkflowexecutionstartedeventattributestypedef) 
33. See [:material-code-braces: ChildWorkflowExecutionCompletedEventAttributesTypeDef](./type_defs.md#childworkflowexecutioncompletedeventattributestypedef) 
34. See [:material-code-braces: ChildWorkflowExecutionFailedEventAttributesTypeDef](./type_defs.md#childworkflowexecutionfailedeventattributestypedef) 
35. See [:material-code-braces: ChildWorkflowExecutionTimedOutEventAttributesTypeDef](./type_defs.md#childworkflowexecutiontimedouteventattributestypedef) 
36. See [:material-code-braces: ChildWorkflowExecutionCanceledEventAttributesTypeDef](./type_defs.md#childworkflowexecutioncanceledeventattributestypedef) 
37. See [:material-code-braces: ChildWorkflowExecutionTerminatedEventAttributesTypeDef](./type_defs.md#childworkflowexecutionterminatedeventattributestypedef) 
38. See [:material-code-braces: SignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef](./type_defs.md#signalexternalworkflowexecutioninitiatedeventattributestypedef) 
39. See [:material-code-braces: ExternalWorkflowExecutionSignaledEventAttributesTypeDef](./type_defs.md#externalworkflowexecutionsignaledeventattributestypedef) 
40. See [:material-code-braces: SignalExternalWorkflowExecutionFailedEventAttributesTypeDef](./type_defs.md#signalexternalworkflowexecutionfailedeventattributestypedef) 
41. See [:material-code-braces: ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef](./type_defs.md#externalworkflowexecutioncancelrequestedeventattributestypedef) 
42. See [:material-code-braces: RequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef](./type_defs.md#requestcancelexternalworkflowexecutioninitiatedeventattributestypedef) 
43. See [:material-code-braces: RequestCancelExternalWorkflowExecutionFailedEventAttributesTypeDef](./type_defs.md#requestcancelexternalworkflowexecutionfailedeventattributestypedef) 
44. See [:material-code-braces: ScheduleActivityTaskFailedEventAttributesTypeDef](./type_defs.md#scheduleactivitytaskfailedeventattributestypedef) 
45. See [:material-code-braces: RequestCancelActivityTaskFailedEventAttributesTypeDef](./type_defs.md#requestcancelactivitytaskfailedeventattributestypedef) 
46. See [:material-code-braces: StartTimerFailedEventAttributesTypeDef](./type_defs.md#starttimerfailedeventattributestypedef) 
47. See [:material-code-braces: CancelTimerFailedEventAttributesTypeDef](./type_defs.md#canceltimerfailedeventattributestypedef) 
48. See [:material-code-braces: StartChildWorkflowExecutionFailedEventAttributesTypeDef](./type_defs.md#startchildworkflowexecutionfailedeventattributestypedef) 
49. See [:material-code-braces: LambdaFunctionScheduledEventAttributesTypeDef](./type_defs.md#lambdafunctionscheduledeventattributestypedef) 
50. See [:material-code-braces: LambdaFunctionStartedEventAttributesTypeDef](./type_defs.md#lambdafunctionstartedeventattributestypedef) 
51. See [:material-code-braces: LambdaFunctionCompletedEventAttributesTypeDef](./type_defs.md#lambdafunctioncompletedeventattributestypedef) 
52. See [:material-code-braces: LambdaFunctionFailedEventAttributesTypeDef](./type_defs.md#lambdafunctionfailedeventattributestypedef) 
53. See [:material-code-braces: LambdaFunctionTimedOutEventAttributesTypeDef](./type_defs.md#lambdafunctiontimedouteventattributestypedef) 
54. See [:material-code-braces: ScheduleLambdaFunctionFailedEventAttributesTypeDef](./type_defs.md#schedulelambdafunctionfailedeventattributestypedef) 
55. See [:material-code-braces: StartLambdaFunctionFailedEventAttributesTypeDef](./type_defs.md#startlambdafunctionfailedeventattributestypedef) 
## WorkflowTypeDetailTypeDef

```python
# WorkflowTypeDetailTypeDef definition

class WorkflowTypeDetailTypeDef(TypedDict):
    typeInfo: WorkflowTypeInfoTypeDef,  # (1)
    configuration: WorkflowTypeConfigurationTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: WorkflowTypeInfoTypeDef](./type_defs.md#workflowtypeinfotypedef) 
2. See [:material-code-braces: WorkflowTypeConfigurationTypeDef](./type_defs.md#workflowtypeconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkflowTypeInfosTypeDef

```python
# WorkflowTypeInfosTypeDef definition

class WorkflowTypeInfosTypeDef(TypedDict):
    typeInfos: List[WorkflowTypeInfoTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkflowTypeInfoTypeDef](./type_defs.md#workflowtypeinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CountClosedWorkflowExecutionsInputRequestTypeDef

```python
# CountClosedWorkflowExecutionsInputRequestTypeDef definition

class CountClosedWorkflowExecutionsInputRequestTypeDef(TypedDict):
    domain: str,
    startTimeFilter: NotRequired[ExecutionTimeFilterTypeDef],  # (1)
    closeTimeFilter: NotRequired[ExecutionTimeFilterTypeDef],  # (1)
    executionFilter: NotRequired[WorkflowExecutionFilterTypeDef],  # (3)
    typeFilter: NotRequired[WorkflowTypeFilterTypeDef],  # (4)
    tagFilter: NotRequired[TagFilterTypeDef],  # (5)
    closeStatusFilter: NotRequired[CloseStatusFilterTypeDef],  # (6)
```

1. See [:material-code-braces: ExecutionTimeFilterTypeDef](./type_defs.md#executiontimefiltertypedef) 
2. See [:material-code-braces: ExecutionTimeFilterTypeDef](./type_defs.md#executiontimefiltertypedef) 
3. See [:material-code-braces: WorkflowExecutionFilterTypeDef](./type_defs.md#workflowexecutionfiltertypedef) 
4. See [:material-code-braces: WorkflowTypeFilterTypeDef](./type_defs.md#workflowtypefiltertypedef) 
5. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
6. See [:material-code-braces: CloseStatusFilterTypeDef](./type_defs.md#closestatusfiltertypedef) 
## CountOpenWorkflowExecutionsInputRequestTypeDef

```python
# CountOpenWorkflowExecutionsInputRequestTypeDef definition

class CountOpenWorkflowExecutionsInputRequestTypeDef(TypedDict):
    domain: str,
    startTimeFilter: ExecutionTimeFilterTypeDef,  # (1)
    typeFilter: NotRequired[WorkflowTypeFilterTypeDef],  # (2)
    tagFilter: NotRequired[TagFilterTypeDef],  # (3)
    executionFilter: NotRequired[WorkflowExecutionFilterTypeDef],  # (4)
```

1. See [:material-code-braces: ExecutionTimeFilterTypeDef](./type_defs.md#executiontimefiltertypedef) 
2. See [:material-code-braces: WorkflowTypeFilterTypeDef](./type_defs.md#workflowtypefiltertypedef) 
3. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
4. See [:material-code-braces: WorkflowExecutionFilterTypeDef](./type_defs.md#workflowexecutionfiltertypedef) 
## ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef

```python
# ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef definition

class ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef(TypedDict):
    domain: str,
    startTimeFilter: NotRequired[ExecutionTimeFilterTypeDef],  # (1)
    closeTimeFilter: NotRequired[ExecutionTimeFilterTypeDef],  # (1)
    executionFilter: NotRequired[WorkflowExecutionFilterTypeDef],  # (3)
    closeStatusFilter: NotRequired[CloseStatusFilterTypeDef],  # (4)
    typeFilter: NotRequired[WorkflowTypeFilterTypeDef],  # (5)
    tagFilter: NotRequired[TagFilterTypeDef],  # (6)
    reverseOrder: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (7)
```

1. See [:material-code-braces: ExecutionTimeFilterTypeDef](./type_defs.md#executiontimefiltertypedef) 
2. See [:material-code-braces: ExecutionTimeFilterTypeDef](./type_defs.md#executiontimefiltertypedef) 
3. See [:material-code-braces: WorkflowExecutionFilterTypeDef](./type_defs.md#workflowexecutionfiltertypedef) 
4. See [:material-code-braces: CloseStatusFilterTypeDef](./type_defs.md#closestatusfiltertypedef) 
5. See [:material-code-braces: WorkflowTypeFilterTypeDef](./type_defs.md#workflowtypefiltertypedef) 
6. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
7. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListClosedWorkflowExecutionsInputRequestTypeDef

```python
# ListClosedWorkflowExecutionsInputRequestTypeDef definition

class ListClosedWorkflowExecutionsInputRequestTypeDef(TypedDict):
    domain: str,
    startTimeFilter: NotRequired[ExecutionTimeFilterTypeDef],  # (1)
    closeTimeFilter: NotRequired[ExecutionTimeFilterTypeDef],  # (1)
    executionFilter: NotRequired[WorkflowExecutionFilterTypeDef],  # (3)
    closeStatusFilter: NotRequired[CloseStatusFilterTypeDef],  # (4)
    typeFilter: NotRequired[WorkflowTypeFilterTypeDef],  # (5)
    tagFilter: NotRequired[TagFilterTypeDef],  # (6)
    nextPageToken: NotRequired[str],
    maximumPageSize: NotRequired[int],
    reverseOrder: NotRequired[bool],
```

1. See [:material-code-braces: ExecutionTimeFilterTypeDef](./type_defs.md#executiontimefiltertypedef) 
2. See [:material-code-braces: ExecutionTimeFilterTypeDef](./type_defs.md#executiontimefiltertypedef) 
3. See [:material-code-braces: WorkflowExecutionFilterTypeDef](./type_defs.md#workflowexecutionfiltertypedef) 
4. See [:material-code-braces: CloseStatusFilterTypeDef](./type_defs.md#closestatusfiltertypedef) 
5. See [:material-code-braces: WorkflowTypeFilterTypeDef](./type_defs.md#workflowtypefiltertypedef) 
6. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
## ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef

```python
# ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef definition

class ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef(TypedDict):
    domain: str,
    startTimeFilter: ExecutionTimeFilterTypeDef,  # (1)
    typeFilter: NotRequired[WorkflowTypeFilterTypeDef],  # (2)
    tagFilter: NotRequired[TagFilterTypeDef],  # (3)
    reverseOrder: NotRequired[bool],
    executionFilter: NotRequired[WorkflowExecutionFilterTypeDef],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-braces: ExecutionTimeFilterTypeDef](./type_defs.md#executiontimefiltertypedef) 
2. See [:material-code-braces: WorkflowTypeFilterTypeDef](./type_defs.md#workflowtypefiltertypedef) 
3. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
4. See [:material-code-braces: WorkflowExecutionFilterTypeDef](./type_defs.md#workflowexecutionfiltertypedef) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOpenWorkflowExecutionsInputRequestTypeDef

```python
# ListOpenWorkflowExecutionsInputRequestTypeDef definition

class ListOpenWorkflowExecutionsInputRequestTypeDef(TypedDict):
    domain: str,
    startTimeFilter: ExecutionTimeFilterTypeDef,  # (1)
    typeFilter: NotRequired[WorkflowTypeFilterTypeDef],  # (2)
    tagFilter: NotRequired[TagFilterTypeDef],  # (3)
    nextPageToken: NotRequired[str],
    maximumPageSize: NotRequired[int],
    reverseOrder: NotRequired[bool],
    executionFilter: NotRequired[WorkflowExecutionFilterTypeDef],  # (4)
```

1. See [:material-code-braces: ExecutionTimeFilterTypeDef](./type_defs.md#executiontimefiltertypedef) 
2. See [:material-code-braces: WorkflowTypeFilterTypeDef](./type_defs.md#workflowtypefiltertypedef) 
3. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
4. See [:material-code-braces: WorkflowExecutionFilterTypeDef](./type_defs.md#workflowexecutionfiltertypedef) 
## RespondDecisionTaskCompletedInputRequestTypeDef

```python
# RespondDecisionTaskCompletedInputRequestTypeDef definition

class RespondDecisionTaskCompletedInputRequestTypeDef(TypedDict):
    taskToken: str,
    decisions: NotRequired[Sequence[DecisionTypeDef]],  # (1)
    executionContext: NotRequired[str],
    taskList: NotRequired[TaskListTypeDef],  # (2)
    taskListScheduleToStartTimeout: NotRequired[str],
```

1. See [:material-code-braces: DecisionTypeDef](./type_defs.md#decisiontypedef) 
2. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
## DecisionTaskTypeDef

```python
# DecisionTaskTypeDef definition

class DecisionTaskTypeDef(TypedDict):
    taskToken: str,
    startedEventId: int,
    workflowExecution: WorkflowExecutionTypeDef,  # (1)
    workflowType: WorkflowTypeTypeDef,  # (2)
    events: List[HistoryEventTypeDef],  # (3)
    nextPageToken: str,
    previousStartedEventId: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: WorkflowExecutionTypeDef](./type_defs.md#workflowexecutiontypedef) 
2. See [:material-code-braces: WorkflowTypeTypeDef](./type_defs.md#workflowtypetypedef) 
3. See [:material-code-braces: HistoryEventTypeDef](./type_defs.md#historyeventtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HistoryTypeDef

```python
# HistoryTypeDef definition

class HistoryTypeDef(TypedDict):
    events: List[HistoryEventTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HistoryEventTypeDef](./type_defs.md#historyeventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
