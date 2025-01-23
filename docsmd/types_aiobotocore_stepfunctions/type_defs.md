# Type definitions

> [Index](../README.md) > [SFN](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SFN](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#sfn)
    type annotations stubs module [types-aiobotocore-stepfunctions](https://pypi.org/project/types-aiobotocore-stepfunctions/).



## ActivityFailedEventDetailsTypeDef

```python
# ActivityFailedEventDetailsTypeDef definition

class ActivityFailedEventDetailsTypeDef(TypedDict):
    error: NotRequired[str],
    cause: NotRequired[str],
```

## ActivityListItemTypeDef

```python
# ActivityListItemTypeDef definition

class ActivityListItemTypeDef(TypedDict):
    activityArn: str,
    name: str,
    creationDate: datetime,
```

## ActivityScheduleFailedEventDetailsTypeDef

```python
# ActivityScheduleFailedEventDetailsTypeDef definition

class ActivityScheduleFailedEventDetailsTypeDef(TypedDict):
    error: NotRequired[str],
    cause: NotRequired[str],
```

## HistoryEventExecutionDataDetailsTypeDef

```python
# HistoryEventExecutionDataDetailsTypeDef definition

class HistoryEventExecutionDataDetailsTypeDef(TypedDict):
    truncated: NotRequired[bool],
```

## ActivityStartedEventDetailsTypeDef

```python
# ActivityStartedEventDetailsTypeDef definition

class ActivityStartedEventDetailsTypeDef(TypedDict):
    workerName: NotRequired[str],
```

## ActivityTimedOutEventDetailsTypeDef

```python
# ActivityTimedOutEventDetailsTypeDef definition

class ActivityTimedOutEventDetailsTypeDef(TypedDict):
    error: NotRequired[str],
    cause: NotRequired[str],
```

## AssignedVariablesDetailsTypeDef

```python
# AssignedVariablesDetailsTypeDef definition

class AssignedVariablesDetailsTypeDef(TypedDict):
    truncated: NotRequired[bool],
```

## BillingDetailsTypeDef

```python
# BillingDetailsTypeDef definition

class BillingDetailsTypeDef(TypedDict):
    billedMemoryUsedInMB: NotRequired[int],
    billedDurationInMilliseconds: NotRequired[int],
```

## CloudWatchEventsExecutionDataDetailsTypeDef

```python
# CloudWatchEventsExecutionDataDetailsTypeDef definition

class CloudWatchEventsExecutionDataDetailsTypeDef(TypedDict):
    included: NotRequired[bool],
```

## CloudWatchLogsLogGroupTypeDef

```python
# CloudWatchLogsLogGroupTypeDef definition

class CloudWatchLogsLogGroupTypeDef(TypedDict):
    logGroupArn: NotRequired[str],
```

## EncryptionConfigurationTypeDef

```python
# EncryptionConfigurationTypeDef definition

class EncryptionConfigurationTypeDef(TypedDict):
    type: EncryptionTypeType,  # (1)
    kmsKeyId: NotRequired[str],
    kmsDataKeyReusePeriodSeconds: NotRequired[int],
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[str],
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

## RoutingConfigurationListItemTypeDef

```python
# RoutingConfigurationListItemTypeDef definition

class RoutingConfigurationListItemTypeDef(TypedDict):
    stateMachineVersionArn: str,
    weight: int,
```

## TracingConfigurationTypeDef

```python
# TracingConfigurationTypeDef definition

class TracingConfigurationTypeDef(TypedDict):
    enabled: NotRequired[bool],
```

## DeleteActivityInputRequestTypeDef

```python
# DeleteActivityInputRequestTypeDef definition

class DeleteActivityInputRequestTypeDef(TypedDict):
    activityArn: str,
```

## DeleteStateMachineAliasInputRequestTypeDef

```python
# DeleteStateMachineAliasInputRequestTypeDef definition

class DeleteStateMachineAliasInputRequestTypeDef(TypedDict):
    stateMachineAliasArn: str,
```

## DeleteStateMachineInputRequestTypeDef

```python
# DeleteStateMachineInputRequestTypeDef definition

class DeleteStateMachineInputRequestTypeDef(TypedDict):
    stateMachineArn: str,
```

## DeleteStateMachineVersionInputRequestTypeDef

```python
# DeleteStateMachineVersionInputRequestTypeDef definition

class DeleteStateMachineVersionInputRequestTypeDef(TypedDict):
    stateMachineVersionArn: str,
```

## DescribeActivityInputRequestTypeDef

```python
# DescribeActivityInputRequestTypeDef definition

class DescribeActivityInputRequestTypeDef(TypedDict):
    activityArn: str,
```

## DescribeExecutionInputRequestTypeDef

```python
# DescribeExecutionInputRequestTypeDef definition

class DescribeExecutionInputRequestTypeDef(TypedDict):
    executionArn: str,
    includedData: NotRequired[IncludedDataType],  # (1)
```

1. See [:material-code-brackets: IncludedDataType](./literals.md#includeddatatype) 
## DescribeMapRunInputRequestTypeDef

```python
# DescribeMapRunInputRequestTypeDef definition

class DescribeMapRunInputRequestTypeDef(TypedDict):
    mapRunArn: str,
```

## MapRunExecutionCountsTypeDef

```python
# MapRunExecutionCountsTypeDef definition

class MapRunExecutionCountsTypeDef(TypedDict):
    pending: int,
    running: int,
    succeeded: int,
    failed: int,
    timedOut: int,
    aborted: int,
    total: int,
    resultsWritten: int,
    failuresNotRedrivable: NotRequired[int],
    pendingRedrive: NotRequired[int],
```

## MapRunItemCountsTypeDef

```python
# MapRunItemCountsTypeDef definition

class MapRunItemCountsTypeDef(TypedDict):
    pending: int,
    running: int,
    succeeded: int,
    failed: int,
    timedOut: int,
    aborted: int,
    total: int,
    resultsWritten: int,
    failuresNotRedrivable: NotRequired[int],
    pendingRedrive: NotRequired[int],
```

## DescribeStateMachineAliasInputRequestTypeDef

```python
# DescribeStateMachineAliasInputRequestTypeDef definition

class DescribeStateMachineAliasInputRequestTypeDef(TypedDict):
    stateMachineAliasArn: str,
```

## DescribeStateMachineForExecutionInputRequestTypeDef

```python
# DescribeStateMachineForExecutionInputRequestTypeDef definition

class DescribeStateMachineForExecutionInputRequestTypeDef(TypedDict):
    executionArn: str,
    includedData: NotRequired[IncludedDataType],  # (1)
```

1. See [:material-code-brackets: IncludedDataType](./literals.md#includeddatatype) 
## DescribeStateMachineInputRequestTypeDef

```python
# DescribeStateMachineInputRequestTypeDef definition

class DescribeStateMachineInputRequestTypeDef(TypedDict):
    stateMachineArn: str,
    includedData: NotRequired[IncludedDataType],  # (1)
```

1. See [:material-code-brackets: IncludedDataType](./literals.md#includeddatatype) 
## EvaluationFailedEventDetailsTypeDef

```python
# EvaluationFailedEventDetailsTypeDef definition

class EvaluationFailedEventDetailsTypeDef(TypedDict):
    state: str,
    error: NotRequired[str],
    cause: NotRequired[str],
    location: NotRequired[str],
```

## ExecutionAbortedEventDetailsTypeDef

```python
# ExecutionAbortedEventDetailsTypeDef definition

class ExecutionAbortedEventDetailsTypeDef(TypedDict):
    error: NotRequired[str],
    cause: NotRequired[str],
```

## ExecutionFailedEventDetailsTypeDef

```python
# ExecutionFailedEventDetailsTypeDef definition

class ExecutionFailedEventDetailsTypeDef(TypedDict):
    error: NotRequired[str],
    cause: NotRequired[str],
```

## ExecutionListItemTypeDef

```python
# ExecutionListItemTypeDef definition

class ExecutionListItemTypeDef(TypedDict):
    executionArn: str,
    stateMachineArn: str,
    name: str,
    status: ExecutionStatusType,  # (1)
    startDate: datetime,
    stopDate: NotRequired[datetime],
    mapRunArn: NotRequired[str],
    itemCount: NotRequired[int],
    stateMachineVersionArn: NotRequired[str],
    stateMachineAliasArn: NotRequired[str],
    redriveCount: NotRequired[int],
    redriveDate: NotRequired[datetime],
```

1. See [:material-code-brackets: ExecutionStatusType](./literals.md#executionstatustype) 
## ExecutionRedrivenEventDetailsTypeDef

```python
# ExecutionRedrivenEventDetailsTypeDef definition

class ExecutionRedrivenEventDetailsTypeDef(TypedDict):
    redriveCount: NotRequired[int],
```

## ExecutionTimedOutEventDetailsTypeDef

```python
# ExecutionTimedOutEventDetailsTypeDef definition

class ExecutionTimedOutEventDetailsTypeDef(TypedDict):
    error: NotRequired[str],
    cause: NotRequired[str],
```

## GetActivityTaskInputRequestTypeDef

```python
# GetActivityTaskInputRequestTypeDef definition

class GetActivityTaskInputRequestTypeDef(TypedDict):
    activityArn: str,
    workerName: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetExecutionHistoryInputRequestTypeDef

```python
# GetExecutionHistoryInputRequestTypeDef definition

class GetExecutionHistoryInputRequestTypeDef(TypedDict):
    executionArn: str,
    maxResults: NotRequired[int],
    reverseOrder: NotRequired[bool],
    nextToken: NotRequired[str],
    includeExecutionData: NotRequired[bool],
```

## LambdaFunctionFailedEventDetailsTypeDef

```python
# LambdaFunctionFailedEventDetailsTypeDef definition

class LambdaFunctionFailedEventDetailsTypeDef(TypedDict):
    error: NotRequired[str],
    cause: NotRequired[str],
```

## LambdaFunctionScheduleFailedEventDetailsTypeDef

```python
# LambdaFunctionScheduleFailedEventDetailsTypeDef definition

class LambdaFunctionScheduleFailedEventDetailsTypeDef(TypedDict):
    error: NotRequired[str],
    cause: NotRequired[str],
```

## LambdaFunctionStartFailedEventDetailsTypeDef

```python
# LambdaFunctionStartFailedEventDetailsTypeDef definition

class LambdaFunctionStartFailedEventDetailsTypeDef(TypedDict):
    error: NotRequired[str],
    cause: NotRequired[str],
```

## LambdaFunctionTimedOutEventDetailsTypeDef

```python
# LambdaFunctionTimedOutEventDetailsTypeDef definition

class LambdaFunctionTimedOutEventDetailsTypeDef(TypedDict):
    error: NotRequired[str],
    cause: NotRequired[str],
```

## MapIterationEventDetailsTypeDef

```python
# MapIterationEventDetailsTypeDef definition

class MapIterationEventDetailsTypeDef(TypedDict):
    name: NotRequired[str],
    index: NotRequired[int],
```

## MapRunFailedEventDetailsTypeDef

```python
# MapRunFailedEventDetailsTypeDef definition

class MapRunFailedEventDetailsTypeDef(TypedDict):
    error: NotRequired[str],
    cause: NotRequired[str],
```

## MapRunRedrivenEventDetailsTypeDef

```python
# MapRunRedrivenEventDetailsTypeDef definition

class MapRunRedrivenEventDetailsTypeDef(TypedDict):
    mapRunArn: NotRequired[str],
    redriveCount: NotRequired[int],
```

## MapRunStartedEventDetailsTypeDef

```python
# MapRunStartedEventDetailsTypeDef definition

class MapRunStartedEventDetailsTypeDef(TypedDict):
    mapRunArn: NotRequired[str],
```

## MapStateStartedEventDetailsTypeDef

```python
# MapStateStartedEventDetailsTypeDef definition

class MapStateStartedEventDetailsTypeDef(TypedDict):
    length: NotRequired[int],
```

## TaskFailedEventDetailsTypeDef

```python
# TaskFailedEventDetailsTypeDef definition

class TaskFailedEventDetailsTypeDef(TypedDict):
    resourceType: str,
    resource: str,
    error: NotRequired[str],
    cause: NotRequired[str],
```

## TaskStartFailedEventDetailsTypeDef

```python
# TaskStartFailedEventDetailsTypeDef definition

class TaskStartFailedEventDetailsTypeDef(TypedDict):
    resourceType: str,
    resource: str,
    error: NotRequired[str],
    cause: NotRequired[str],
```

## TaskStartedEventDetailsTypeDef

```python
# TaskStartedEventDetailsTypeDef definition

class TaskStartedEventDetailsTypeDef(TypedDict):
    resourceType: str,
    resource: str,
```

## TaskSubmitFailedEventDetailsTypeDef

```python
# TaskSubmitFailedEventDetailsTypeDef definition

class TaskSubmitFailedEventDetailsTypeDef(TypedDict):
    resourceType: str,
    resource: str,
    error: NotRequired[str],
    cause: NotRequired[str],
```

## TaskTimedOutEventDetailsTypeDef

```python
# TaskTimedOutEventDetailsTypeDef definition

class TaskTimedOutEventDetailsTypeDef(TypedDict):
    resourceType: str,
    resource: str,
    error: NotRequired[str],
    cause: NotRequired[str],
```

## InspectionDataRequestTypeDef

```python
# InspectionDataRequestTypeDef definition

class InspectionDataRequestTypeDef(TypedDict):
    protocol: NotRequired[str],
    method: NotRequired[str],
    url: NotRequired[str],
    headers: NotRequired[str],
    body: NotRequired[str],
```

## InspectionDataResponseTypeDef

```python
# InspectionDataResponseTypeDef definition

class InspectionDataResponseTypeDef(TypedDict):
    protocol: NotRequired[str],
    statusCode: NotRequired[str],
    statusMessage: NotRequired[str],
    headers: NotRequired[str],
    body: NotRequired[str],
```

## TaskCredentialsTypeDef

```python
# TaskCredentialsTypeDef definition

class TaskCredentialsTypeDef(TypedDict):
    roleArn: NotRequired[str],
```

## ListActivitiesInputRequestTypeDef

```python
# ListActivitiesInputRequestTypeDef definition

class ListActivitiesInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListExecutionsInputRequestTypeDef

```python
# ListExecutionsInputRequestTypeDef definition

class ListExecutionsInputRequestTypeDef(TypedDict):
    stateMachineArn: NotRequired[str],
    statusFilter: NotRequired[ExecutionStatusType],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    mapRunArn: NotRequired[str],
    redriveFilter: NotRequired[ExecutionRedriveFilterType],  # (2)
```

1. See [:material-code-brackets: ExecutionStatusType](./literals.md#executionstatustype) 
2. See [:material-code-brackets: ExecutionRedriveFilterType](./literals.md#executionredrivefiltertype) 
## ListMapRunsInputRequestTypeDef

```python
# ListMapRunsInputRequestTypeDef definition

class ListMapRunsInputRequestTypeDef(TypedDict):
    executionArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## MapRunListItemTypeDef

```python
# MapRunListItemTypeDef definition

class MapRunListItemTypeDef(TypedDict):
    executionArn: str,
    mapRunArn: str,
    stateMachineArn: str,
    startDate: datetime,
    stopDate: NotRequired[datetime],
```

## ListStateMachineAliasesInputRequestTypeDef

```python
# ListStateMachineAliasesInputRequestTypeDef definition

class ListStateMachineAliasesInputRequestTypeDef(TypedDict):
    stateMachineArn: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## StateMachineAliasListItemTypeDef

```python
# StateMachineAliasListItemTypeDef definition

class StateMachineAliasListItemTypeDef(TypedDict):
    stateMachineAliasArn: str,
    creationDate: datetime,
```

## ListStateMachineVersionsInputRequestTypeDef

```python
# ListStateMachineVersionsInputRequestTypeDef definition

class ListStateMachineVersionsInputRequestTypeDef(TypedDict):
    stateMachineArn: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## StateMachineVersionListItemTypeDef

```python
# StateMachineVersionListItemTypeDef definition

class StateMachineVersionListItemTypeDef(TypedDict):
    stateMachineVersionArn: str,
    creationDate: datetime,
```

## ListStateMachinesInputRequestTypeDef

```python
# ListStateMachinesInputRequestTypeDef definition

class ListStateMachinesInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## StateMachineListItemTypeDef

```python
# StateMachineListItemTypeDef definition

class StateMachineListItemTypeDef(TypedDict):
    stateMachineArn: str,
    name: str,
    type: StateMachineTypeType,  # (1)
    creationDate: datetime,
```

1. See [:material-code-brackets: StateMachineTypeType](./literals.md#statemachinetypetype) 
## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
```

## PublishStateMachineVersionInputRequestTypeDef

```python
# PublishStateMachineVersionInputRequestTypeDef definition

class PublishStateMachineVersionInputRequestTypeDef(TypedDict):
    stateMachineArn: str,
    revisionId: NotRequired[str],
    description: NotRequired[str],
```

## RedriveExecutionInputRequestTypeDef

```python
# RedriveExecutionInputRequestTypeDef definition

class RedriveExecutionInputRequestTypeDef(TypedDict):
    executionArn: str,
    clientToken: NotRequired[str],
```

## SendTaskFailureInputRequestTypeDef

```python
# SendTaskFailureInputRequestTypeDef definition

class SendTaskFailureInputRequestTypeDef(TypedDict):
    taskToken: str,
    error: NotRequired[str],
    cause: NotRequired[str],
```

## SendTaskHeartbeatInputRequestTypeDef

```python
# SendTaskHeartbeatInputRequestTypeDef definition

class SendTaskHeartbeatInputRequestTypeDef(TypedDict):
    taskToken: str,
```

## SendTaskSuccessInputRequestTypeDef

```python
# SendTaskSuccessInputRequestTypeDef definition

class SendTaskSuccessInputRequestTypeDef(TypedDict):
    taskToken: str,
    output: str,
```

## StartExecutionInputRequestTypeDef

```python
# StartExecutionInputRequestTypeDef definition

class StartExecutionInputRequestTypeDef(TypedDict):
    stateMachineArn: str,
    name: NotRequired[str],
    input: NotRequired[str],
    traceHeader: NotRequired[str],
```

## StartSyncExecutionInputRequestTypeDef

```python
# StartSyncExecutionInputRequestTypeDef definition

class StartSyncExecutionInputRequestTypeDef(TypedDict):
    stateMachineArn: str,
    name: NotRequired[str],
    input: NotRequired[str],
    traceHeader: NotRequired[str],
    includedData: NotRequired[IncludedDataType],  # (1)
```

1. See [:material-code-brackets: IncludedDataType](./literals.md#includeddatatype) 
## StopExecutionInputRequestTypeDef

```python
# StopExecutionInputRequestTypeDef definition

class StopExecutionInputRequestTypeDef(TypedDict):
    executionArn: str,
    error: NotRequired[str],
    cause: NotRequired[str],
```

## TestStateInputRequestTypeDef

```python
# TestStateInputRequestTypeDef definition

class TestStateInputRequestTypeDef(TypedDict):
    definition: str,
    roleArn: NotRequired[str],
    input: NotRequired[str],
    inspectionLevel: NotRequired[InspectionLevelType],  # (1)
    revealSecrets: NotRequired[bool],
    variables: NotRequired[str],
```

1. See [:material-code-brackets: InspectionLevelType](./literals.md#inspectionleveltype) 
## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateMapRunInputRequestTypeDef

```python
# UpdateMapRunInputRequestTypeDef definition

class UpdateMapRunInputRequestTypeDef(TypedDict):
    mapRunArn: str,
    maxConcurrency: NotRequired[int],
    toleratedFailurePercentage: NotRequired[float],
    toleratedFailureCount: NotRequired[int],
```

## ValidateStateMachineDefinitionDiagnosticTypeDef

```python
# ValidateStateMachineDefinitionDiagnosticTypeDef definition

class ValidateStateMachineDefinitionDiagnosticTypeDef(TypedDict):
    severity: ValidateStateMachineDefinitionSeverityType,  # (1)
    code: str,
    message: str,
    location: NotRequired[str],
```

1. See [:material-code-brackets: ValidateStateMachineDefinitionSeverityType](./literals.md#validatestatemachinedefinitionseveritytype) 
## ValidateStateMachineDefinitionInputRequestTypeDef

```python
# ValidateStateMachineDefinitionInputRequestTypeDef definition

class ValidateStateMachineDefinitionInputRequestTypeDef(TypedDict):
    definition: str,
    type: NotRequired[StateMachineTypeType],  # (1)
    severity: NotRequired[ValidateStateMachineDefinitionSeverityType],  # (2)
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: StateMachineTypeType](./literals.md#statemachinetypetype) 
2. See [:material-code-brackets: ValidateStateMachineDefinitionSeverityType](./literals.md#validatestatemachinedefinitionseveritytype) 
## ActivityScheduledEventDetailsTypeDef

```python
# ActivityScheduledEventDetailsTypeDef definition

class ActivityScheduledEventDetailsTypeDef(TypedDict):
    resource: str,
    input: NotRequired[str],
    inputDetails: NotRequired[HistoryEventExecutionDataDetailsTypeDef],  # (1)
    timeoutInSeconds: NotRequired[int],
    heartbeatInSeconds: NotRequired[int],
```

1. See [:material-code-braces: HistoryEventExecutionDataDetailsTypeDef](./type_defs.md#historyeventexecutiondatadetailstypedef) 
## ActivitySucceededEventDetailsTypeDef

```python
# ActivitySucceededEventDetailsTypeDef definition

class ActivitySucceededEventDetailsTypeDef(TypedDict):
    output: NotRequired[str],
    outputDetails: NotRequired[HistoryEventExecutionDataDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: HistoryEventExecutionDataDetailsTypeDef](./type_defs.md#historyeventexecutiondatadetailstypedef) 
## ExecutionStartedEventDetailsTypeDef

```python
# ExecutionStartedEventDetailsTypeDef definition

class ExecutionStartedEventDetailsTypeDef(TypedDict):
    input: NotRequired[str],
    inputDetails: NotRequired[HistoryEventExecutionDataDetailsTypeDef],  # (1)
    roleArn: NotRequired[str],
    stateMachineAliasArn: NotRequired[str],
    stateMachineVersionArn: NotRequired[str],
```

1. See [:material-code-braces: HistoryEventExecutionDataDetailsTypeDef](./type_defs.md#historyeventexecutiondatadetailstypedef) 
## ExecutionSucceededEventDetailsTypeDef

```python
# ExecutionSucceededEventDetailsTypeDef definition

class ExecutionSucceededEventDetailsTypeDef(TypedDict):
    output: NotRequired[str],
    outputDetails: NotRequired[HistoryEventExecutionDataDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: HistoryEventExecutionDataDetailsTypeDef](./type_defs.md#historyeventexecutiondatadetailstypedef) 
## LambdaFunctionSucceededEventDetailsTypeDef

```python
# LambdaFunctionSucceededEventDetailsTypeDef definition

class LambdaFunctionSucceededEventDetailsTypeDef(TypedDict):
    output: NotRequired[str],
    outputDetails: NotRequired[HistoryEventExecutionDataDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: HistoryEventExecutionDataDetailsTypeDef](./type_defs.md#historyeventexecutiondatadetailstypedef) 
## StateEnteredEventDetailsTypeDef

```python
# StateEnteredEventDetailsTypeDef definition

class StateEnteredEventDetailsTypeDef(TypedDict):
    name: str,
    input: NotRequired[str],
    inputDetails: NotRequired[HistoryEventExecutionDataDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: HistoryEventExecutionDataDetailsTypeDef](./type_defs.md#historyeventexecutiondatadetailstypedef) 
## TaskSubmittedEventDetailsTypeDef

```python
# TaskSubmittedEventDetailsTypeDef definition

class TaskSubmittedEventDetailsTypeDef(TypedDict):
    resourceType: str,
    resource: str,
    output: NotRequired[str],
    outputDetails: NotRequired[HistoryEventExecutionDataDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: HistoryEventExecutionDataDetailsTypeDef](./type_defs.md#historyeventexecutiondatadetailstypedef) 
## TaskSucceededEventDetailsTypeDef

```python
# TaskSucceededEventDetailsTypeDef definition

class TaskSucceededEventDetailsTypeDef(TypedDict):
    resourceType: str,
    resource: str,
    output: NotRequired[str],
    outputDetails: NotRequired[HistoryEventExecutionDataDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: HistoryEventExecutionDataDetailsTypeDef](./type_defs.md#historyeventexecutiondatadetailstypedef) 
## StateExitedEventDetailsTypeDef

```python
# StateExitedEventDetailsTypeDef definition

class StateExitedEventDetailsTypeDef(TypedDict):
    name: str,
    output: NotRequired[str],
    outputDetails: NotRequired[HistoryEventExecutionDataDetailsTypeDef],  # (1)
    assignedVariables: NotRequired[Dict[str, str]],
    assignedVariablesDetails: NotRequired[AssignedVariablesDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: HistoryEventExecutionDataDetailsTypeDef](./type_defs.md#historyeventexecutiondatadetailstypedef) 
2. See [:material-code-braces: AssignedVariablesDetailsTypeDef](./type_defs.md#assignedvariablesdetailstypedef) 
## LogDestinationTypeDef

```python
# LogDestinationTypeDef definition

class LogDestinationTypeDef(TypedDict):
    cloudWatchLogsLogGroup: NotRequired[CloudWatchLogsLogGroupTypeDef],  # (1)
```

1. See [:material-code-braces: CloudWatchLogsLogGroupTypeDef](./type_defs.md#cloudwatchlogsloggrouptypedef) 
## CreateActivityInputRequestTypeDef

```python
# CreateActivityInputRequestTypeDef definition

class CreateActivityInputRequestTypeDef(TypedDict):
    name: str,
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    encryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateActivityOutputTypeDef

```python
# CreateActivityOutputTypeDef definition

class CreateActivityOutputTypeDef(TypedDict):
    activityArn: str,
    creationDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStateMachineAliasOutputTypeDef

```python
# CreateStateMachineAliasOutputTypeDef definition

class CreateStateMachineAliasOutputTypeDef(TypedDict):
    stateMachineAliasArn: str,
    creationDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStateMachineOutputTypeDef

```python
# CreateStateMachineOutputTypeDef definition

class CreateStateMachineOutputTypeDef(TypedDict):
    stateMachineArn: str,
    creationDate: datetime,
    stateMachineVersionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeActivityOutputTypeDef

```python
# DescribeActivityOutputTypeDef definition

class DescribeActivityOutputTypeDef(TypedDict):
    activityArn: str,
    name: str,
    creationDate: datetime,
    encryptionConfiguration: EncryptionConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeExecutionOutputTypeDef

```python
# DescribeExecutionOutputTypeDef definition

class DescribeExecutionOutputTypeDef(TypedDict):
    executionArn: str,
    stateMachineArn: str,
    name: str,
    status: ExecutionStatusType,  # (1)
    startDate: datetime,
    input: str,
    inputDetails: CloudWatchEventsExecutionDataDetailsTypeDef,  # (2)
    redriveCount: int,
    redriveStatus: ExecutionRedriveStatusType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
    stopDate: NotRequired[datetime],
    output: NotRequired[str],
    outputDetails: NotRequired[CloudWatchEventsExecutionDataDetailsTypeDef],  # (2)
    traceHeader: NotRequired[str],
    mapRunArn: NotRequired[str],
    error: NotRequired[str],
    cause: NotRequired[str],
    stateMachineVersionArn: NotRequired[str],
    stateMachineAliasArn: NotRequired[str],
    redriveDate: NotRequired[datetime],
    redriveStatusReason: NotRequired[str],
```

1. See [:material-code-brackets: ExecutionStatusType](./literals.md#executionstatustype) 
2. See [:material-code-braces: CloudWatchEventsExecutionDataDetailsTypeDef](./type_defs.md#cloudwatcheventsexecutiondatadetailstypedef) 
3. See [:material-code-braces: CloudWatchEventsExecutionDataDetailsTypeDef](./type_defs.md#cloudwatcheventsexecutiondatadetailstypedef) 
4. See [:material-code-brackets: ExecutionRedriveStatusType](./literals.md#executionredrivestatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetActivityTaskOutputTypeDef

```python
# GetActivityTaskOutputTypeDef definition

class GetActivityTaskOutputTypeDef(TypedDict):
    taskToken: str,
    input: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListActivitiesOutputTypeDef

```python
# ListActivitiesOutputTypeDef definition

class ListActivitiesOutputTypeDef(TypedDict):
    activities: List[ActivityListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ActivityListItemTypeDef](./type_defs.md#activitylistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PublishStateMachineVersionOutputTypeDef

```python
# PublishStateMachineVersionOutputTypeDef definition

class PublishStateMachineVersionOutputTypeDef(TypedDict):
    creationDate: datetime,
    stateMachineVersionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RedriveExecutionOutputTypeDef

```python
# RedriveExecutionOutputTypeDef definition

class RedriveExecutionOutputTypeDef(TypedDict):
    redriveDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartExecutionOutputTypeDef

```python
# StartExecutionOutputTypeDef definition

class StartExecutionOutputTypeDef(TypedDict):
    executionArn: str,
    startDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSyncExecutionOutputTypeDef

```python
# StartSyncExecutionOutputTypeDef definition

class StartSyncExecutionOutputTypeDef(TypedDict):
    executionArn: str,
    stateMachineArn: str,
    name: str,
    startDate: datetime,
    stopDate: datetime,
    status: SyncExecutionStatusType,  # (1)
    error: str,
    cause: str,
    input: str,
    inputDetails: CloudWatchEventsExecutionDataDetailsTypeDef,  # (2)
    output: str,
    outputDetails: CloudWatchEventsExecutionDataDetailsTypeDef,  # (2)
    traceHeader: str,
    billingDetails: BillingDetailsTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: SyncExecutionStatusType](./literals.md#syncexecutionstatustype) 
2. See [:material-code-braces: CloudWatchEventsExecutionDataDetailsTypeDef](./type_defs.md#cloudwatcheventsexecutiondatadetailstypedef) 
3. See [:material-code-braces: CloudWatchEventsExecutionDataDetailsTypeDef](./type_defs.md#cloudwatcheventsexecutiondatadetailstypedef) 
4. See [:material-code-braces: BillingDetailsTypeDef](./type_defs.md#billingdetailstypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopExecutionOutputTypeDef

```python
# StopExecutionOutputTypeDef definition

class StopExecutionOutputTypeDef(TypedDict):
    stopDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateStateMachineAliasOutputTypeDef

```python
# UpdateStateMachineAliasOutputTypeDef definition

class UpdateStateMachineAliasOutputTypeDef(TypedDict):
    updateDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateStateMachineOutputTypeDef

```python
# UpdateStateMachineOutputTypeDef definition

class UpdateStateMachineOutputTypeDef(TypedDict):
    updateDate: datetime,
    revisionId: str,
    stateMachineVersionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStateMachineAliasInputRequestTypeDef

```python
# CreateStateMachineAliasInputRequestTypeDef definition

class CreateStateMachineAliasInputRequestTypeDef(TypedDict):
    name: str,
    routingConfiguration: Sequence[RoutingConfigurationListItemTypeDef],  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: RoutingConfigurationListItemTypeDef](./type_defs.md#routingconfigurationlistitemtypedef) 
## DescribeStateMachineAliasOutputTypeDef

```python
# DescribeStateMachineAliasOutputTypeDef definition

class DescribeStateMachineAliasOutputTypeDef(TypedDict):
    stateMachineAliasArn: str,
    name: str,
    description: str,
    routingConfiguration: List[RoutingConfigurationListItemTypeDef],  # (1)
    creationDate: datetime,
    updateDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoutingConfigurationListItemTypeDef](./type_defs.md#routingconfigurationlistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateStateMachineAliasInputRequestTypeDef

```python
# UpdateStateMachineAliasInputRequestTypeDef definition

class UpdateStateMachineAliasInputRequestTypeDef(TypedDict):
    stateMachineAliasArn: str,
    description: NotRequired[str],
    routingConfiguration: NotRequired[Sequence[RoutingConfigurationListItemTypeDef]],  # (1)
```

1. See [:material-code-braces: RoutingConfigurationListItemTypeDef](./type_defs.md#routingconfigurationlistitemtypedef) 
## DescribeMapRunOutputTypeDef

```python
# DescribeMapRunOutputTypeDef definition

class DescribeMapRunOutputTypeDef(TypedDict):
    mapRunArn: str,
    executionArn: str,
    status: MapRunStatusType,  # (1)
    startDate: datetime,
    stopDate: datetime,
    maxConcurrency: int,
    toleratedFailurePercentage: float,
    toleratedFailureCount: int,
    itemCounts: MapRunItemCountsTypeDef,  # (2)
    executionCounts: MapRunExecutionCountsTypeDef,  # (3)
    redriveCount: int,
    redriveDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: MapRunStatusType](./literals.md#maprunstatustype) 
2. See [:material-code-braces: MapRunItemCountsTypeDef](./type_defs.md#maprunitemcountstypedef) 
3. See [:material-code-braces: MapRunExecutionCountsTypeDef](./type_defs.md#maprunexecutioncountstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListExecutionsOutputTypeDef

```python
# ListExecutionsOutputTypeDef definition

class ListExecutionsOutputTypeDef(TypedDict):
    executions: List[ExecutionListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ExecutionListItemTypeDef](./type_defs.md#executionlistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetExecutionHistoryInputPaginateTypeDef

```python
# GetExecutionHistoryInputPaginateTypeDef definition

class GetExecutionHistoryInputPaginateTypeDef(TypedDict):
    executionArn: str,
    reverseOrder: NotRequired[bool],
    includeExecutionData: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListActivitiesInputPaginateTypeDef

```python
# ListActivitiesInputPaginateTypeDef definition

class ListActivitiesInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListExecutionsInputPaginateTypeDef

```python
# ListExecutionsInputPaginateTypeDef definition

class ListExecutionsInputPaginateTypeDef(TypedDict):
    stateMachineArn: NotRequired[str],
    statusFilter: NotRequired[ExecutionStatusType],  # (1)
    mapRunArn: NotRequired[str],
    redriveFilter: NotRequired[ExecutionRedriveFilterType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ExecutionStatusType](./literals.md#executionstatustype) 
2. See [:material-code-brackets: ExecutionRedriveFilterType](./literals.md#executionredrivefiltertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMapRunsInputPaginateTypeDef

```python
# ListMapRunsInputPaginateTypeDef definition

class ListMapRunsInputPaginateTypeDef(TypedDict):
    executionArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStateMachinesInputPaginateTypeDef

```python
# ListStateMachinesInputPaginateTypeDef definition

class ListStateMachinesInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## InspectionDataTypeDef

```python
# InspectionDataTypeDef definition

class InspectionDataTypeDef(TypedDict):
    input: NotRequired[str],
    afterArguments: NotRequired[str],
    afterInputPath: NotRequired[str],
    afterParameters: NotRequired[str],
    result: NotRequired[str],
    afterResultSelector: NotRequired[str],
    afterResultPath: NotRequired[str],
    request: NotRequired[InspectionDataRequestTypeDef],  # (1)
    response: NotRequired[InspectionDataResponseTypeDef],  # (2)
    variables: NotRequired[str],
```

1. See [:material-code-braces: InspectionDataRequestTypeDef](./type_defs.md#inspectiondatarequesttypedef) 
2. See [:material-code-braces: InspectionDataResponseTypeDef](./type_defs.md#inspectiondataresponsetypedef) 
## LambdaFunctionScheduledEventDetailsTypeDef

```python
# LambdaFunctionScheduledEventDetailsTypeDef definition

class LambdaFunctionScheduledEventDetailsTypeDef(TypedDict):
    resource: str,
    input: NotRequired[str],
    inputDetails: NotRequired[HistoryEventExecutionDataDetailsTypeDef],  # (1)
    timeoutInSeconds: NotRequired[int],
    taskCredentials: NotRequired[TaskCredentialsTypeDef],  # (2)
```

1. See [:material-code-braces: HistoryEventExecutionDataDetailsTypeDef](./type_defs.md#historyeventexecutiondatadetailstypedef) 
2. See [:material-code-braces: TaskCredentialsTypeDef](./type_defs.md#taskcredentialstypedef) 
## TaskScheduledEventDetailsTypeDef

```python
# TaskScheduledEventDetailsTypeDef definition

class TaskScheduledEventDetailsTypeDef(TypedDict):
    resourceType: str,
    resource: str,
    region: str,
    parameters: str,
    timeoutInSeconds: NotRequired[int],
    heartbeatInSeconds: NotRequired[int],
    taskCredentials: NotRequired[TaskCredentialsTypeDef],  # (1)
```

1. See [:material-code-braces: TaskCredentialsTypeDef](./type_defs.md#taskcredentialstypedef) 
## ListMapRunsOutputTypeDef

```python
# ListMapRunsOutputTypeDef definition

class ListMapRunsOutputTypeDef(TypedDict):
    mapRuns: List[MapRunListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MapRunListItemTypeDef](./type_defs.md#maprunlistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStateMachineAliasesOutputTypeDef

```python
# ListStateMachineAliasesOutputTypeDef definition

class ListStateMachineAliasesOutputTypeDef(TypedDict):
    stateMachineAliases: List[StateMachineAliasListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: StateMachineAliasListItemTypeDef](./type_defs.md#statemachinealiaslistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStateMachineVersionsOutputTypeDef

```python
# ListStateMachineVersionsOutputTypeDef definition

class ListStateMachineVersionsOutputTypeDef(TypedDict):
    stateMachineVersions: List[StateMachineVersionListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: StateMachineVersionListItemTypeDef](./type_defs.md#statemachineversionlistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStateMachinesOutputTypeDef

```python
# ListStateMachinesOutputTypeDef definition

class ListStateMachinesOutputTypeDef(TypedDict):
    stateMachines: List[StateMachineListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: StateMachineListItemTypeDef](./type_defs.md#statemachinelistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ValidateStateMachineDefinitionOutputTypeDef

```python
# ValidateStateMachineDefinitionOutputTypeDef definition

class ValidateStateMachineDefinitionOutputTypeDef(TypedDict):
    result: ValidateStateMachineDefinitionResultCodeType,  # (1)
    diagnostics: List[ValidateStateMachineDefinitionDiagnosticTypeDef],  # (2)
    truncated: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ValidateStateMachineDefinitionResultCodeType](./literals.md#validatestatemachinedefinitionresultcodetype) 
2. See [:material-code-braces: ValidateStateMachineDefinitionDiagnosticTypeDef](./type_defs.md#validatestatemachinedefinitiondiagnostictypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LoggingConfigurationOutputTypeDef

```python
# LoggingConfigurationOutputTypeDef definition

class LoggingConfigurationOutputTypeDef(TypedDict):
    level: NotRequired[LogLevelType],  # (1)
    includeExecutionData: NotRequired[bool],
    destinations: NotRequired[List[LogDestinationTypeDef]],  # (2)
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
2. See [:material-code-braces: LogDestinationTypeDef](./type_defs.md#logdestinationtypedef) 
## LoggingConfigurationTypeDef

```python
# LoggingConfigurationTypeDef definition

class LoggingConfigurationTypeDef(TypedDict):
    level: NotRequired[LogLevelType],  # (1)
    includeExecutionData: NotRequired[bool],
    destinations: NotRequired[Sequence[LogDestinationTypeDef]],  # (2)
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
2. See [:material-code-braces: LogDestinationTypeDef](./type_defs.md#logdestinationtypedef) 
## TestStateOutputTypeDef

```python
# TestStateOutputTypeDef definition

class TestStateOutputTypeDef(TypedDict):
    output: str,
    error: str,
    cause: str,
    inspectionData: InspectionDataTypeDef,  # (1)
    nextState: str,
    status: TestExecutionStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: InspectionDataTypeDef](./type_defs.md#inspectiondatatypedef) 
2. See [:material-code-brackets: TestExecutionStatusType](./literals.md#testexecutionstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HistoryEventTypeDef

```python
# HistoryEventTypeDef definition

class HistoryEventTypeDef(TypedDict):
    timestamp: datetime,
    type: HistoryEventTypeType,  # (1)
    id: int,
    previousEventId: NotRequired[int],
    activityFailedEventDetails: NotRequired[ActivityFailedEventDetailsTypeDef],  # (2)
    activityScheduleFailedEventDetails: NotRequired[ActivityScheduleFailedEventDetailsTypeDef],  # (3)
    activityScheduledEventDetails: NotRequired[ActivityScheduledEventDetailsTypeDef],  # (4)
    activityStartedEventDetails: NotRequired[ActivityStartedEventDetailsTypeDef],  # (5)
    activitySucceededEventDetails: NotRequired[ActivitySucceededEventDetailsTypeDef],  # (6)
    activityTimedOutEventDetails: NotRequired[ActivityTimedOutEventDetailsTypeDef],  # (7)
    taskFailedEventDetails: NotRequired[TaskFailedEventDetailsTypeDef],  # (8)
    taskScheduledEventDetails: NotRequired[TaskScheduledEventDetailsTypeDef],  # (9)
    taskStartFailedEventDetails: NotRequired[TaskStartFailedEventDetailsTypeDef],  # (10)
    taskStartedEventDetails: NotRequired[TaskStartedEventDetailsTypeDef],  # (11)
    taskSubmitFailedEventDetails: NotRequired[TaskSubmitFailedEventDetailsTypeDef],  # (12)
    taskSubmittedEventDetails: NotRequired[TaskSubmittedEventDetailsTypeDef],  # (13)
    taskSucceededEventDetails: NotRequired[TaskSucceededEventDetailsTypeDef],  # (14)
    taskTimedOutEventDetails: NotRequired[TaskTimedOutEventDetailsTypeDef],  # (15)
    executionFailedEventDetails: NotRequired[ExecutionFailedEventDetailsTypeDef],  # (16)
    executionStartedEventDetails: NotRequired[ExecutionStartedEventDetailsTypeDef],  # (17)
    executionSucceededEventDetails: NotRequired[ExecutionSucceededEventDetailsTypeDef],  # (18)
    executionAbortedEventDetails: NotRequired[ExecutionAbortedEventDetailsTypeDef],  # (19)
    executionTimedOutEventDetails: NotRequired[ExecutionTimedOutEventDetailsTypeDef],  # (20)
    executionRedrivenEventDetails: NotRequired[ExecutionRedrivenEventDetailsTypeDef],  # (21)
    mapStateStartedEventDetails: NotRequired[MapStateStartedEventDetailsTypeDef],  # (22)
    mapIterationStartedEventDetails: NotRequired[MapIterationEventDetailsTypeDef],  # (23)
    mapIterationSucceededEventDetails: NotRequired[MapIterationEventDetailsTypeDef],  # (23)
    mapIterationFailedEventDetails: NotRequired[MapIterationEventDetailsTypeDef],  # (23)
    mapIterationAbortedEventDetails: NotRequired[MapIterationEventDetailsTypeDef],  # (23)
    lambdaFunctionFailedEventDetails: NotRequired[LambdaFunctionFailedEventDetailsTypeDef],  # (27)
    lambdaFunctionScheduleFailedEventDetails: NotRequired[LambdaFunctionScheduleFailedEventDetailsTypeDef],  # (28)
    lambdaFunctionScheduledEventDetails: NotRequired[LambdaFunctionScheduledEventDetailsTypeDef],  # (29)
    lambdaFunctionStartFailedEventDetails: NotRequired[LambdaFunctionStartFailedEventDetailsTypeDef],  # (30)
    lambdaFunctionSucceededEventDetails: NotRequired[LambdaFunctionSucceededEventDetailsTypeDef],  # (31)
    lambdaFunctionTimedOutEventDetails: NotRequired[LambdaFunctionTimedOutEventDetailsTypeDef],  # (32)
    stateEnteredEventDetails: NotRequired[StateEnteredEventDetailsTypeDef],  # (33)
    stateExitedEventDetails: NotRequired[StateExitedEventDetailsTypeDef],  # (34)
    mapRunStartedEventDetails: NotRequired[MapRunStartedEventDetailsTypeDef],  # (35)
    mapRunFailedEventDetails: NotRequired[MapRunFailedEventDetailsTypeDef],  # (36)
    mapRunRedrivenEventDetails: NotRequired[MapRunRedrivenEventDetailsTypeDef],  # (37)
    evaluationFailedEventDetails: NotRequired[EvaluationFailedEventDetailsTypeDef],  # (38)
```

1. See [:material-code-brackets: HistoryEventTypeType](./literals.md#historyeventtypetype) 
2. See [:material-code-braces: ActivityFailedEventDetailsTypeDef](./type_defs.md#activityfailedeventdetailstypedef) 
3. See [:material-code-braces: ActivityScheduleFailedEventDetailsTypeDef](./type_defs.md#activityschedulefailedeventdetailstypedef) 
4. See [:material-code-braces: ActivityScheduledEventDetailsTypeDef](./type_defs.md#activityscheduledeventdetailstypedef) 
5. See [:material-code-braces: ActivityStartedEventDetailsTypeDef](./type_defs.md#activitystartedeventdetailstypedef) 
6. See [:material-code-braces: ActivitySucceededEventDetailsTypeDef](./type_defs.md#activitysucceededeventdetailstypedef) 
7. See [:material-code-braces: ActivityTimedOutEventDetailsTypeDef](./type_defs.md#activitytimedouteventdetailstypedef) 
8. See [:material-code-braces: TaskFailedEventDetailsTypeDef](./type_defs.md#taskfailedeventdetailstypedef) 
9. See [:material-code-braces: TaskScheduledEventDetailsTypeDef](./type_defs.md#taskscheduledeventdetailstypedef) 
10. See [:material-code-braces: TaskStartFailedEventDetailsTypeDef](./type_defs.md#taskstartfailedeventdetailstypedef) 
11. See [:material-code-braces: TaskStartedEventDetailsTypeDef](./type_defs.md#taskstartedeventdetailstypedef) 
12. See [:material-code-braces: TaskSubmitFailedEventDetailsTypeDef](./type_defs.md#tasksubmitfailedeventdetailstypedef) 
13. See [:material-code-braces: TaskSubmittedEventDetailsTypeDef](./type_defs.md#tasksubmittedeventdetailstypedef) 
14. See [:material-code-braces: TaskSucceededEventDetailsTypeDef](./type_defs.md#tasksucceededeventdetailstypedef) 
15. See [:material-code-braces: TaskTimedOutEventDetailsTypeDef](./type_defs.md#tasktimedouteventdetailstypedef) 
16. See [:material-code-braces: ExecutionFailedEventDetailsTypeDef](./type_defs.md#executionfailedeventdetailstypedef) 
17. See [:material-code-braces: ExecutionStartedEventDetailsTypeDef](./type_defs.md#executionstartedeventdetailstypedef) 
18. See [:material-code-braces: ExecutionSucceededEventDetailsTypeDef](./type_defs.md#executionsucceededeventdetailstypedef) 
19. See [:material-code-braces: ExecutionAbortedEventDetailsTypeDef](./type_defs.md#executionabortedeventdetailstypedef) 
20. See [:material-code-braces: ExecutionTimedOutEventDetailsTypeDef](./type_defs.md#executiontimedouteventdetailstypedef) 
21. See [:material-code-braces: ExecutionRedrivenEventDetailsTypeDef](./type_defs.md#executionredriveneventdetailstypedef) 
22. See [:material-code-braces: MapStateStartedEventDetailsTypeDef](./type_defs.md#mapstatestartedeventdetailstypedef) 
23. See [:material-code-braces: MapIterationEventDetailsTypeDef](./type_defs.md#mapiterationeventdetailstypedef) 
24. See [:material-code-braces: MapIterationEventDetailsTypeDef](./type_defs.md#mapiterationeventdetailstypedef) 
25. See [:material-code-braces: MapIterationEventDetailsTypeDef](./type_defs.md#mapiterationeventdetailstypedef) 
26. See [:material-code-braces: MapIterationEventDetailsTypeDef](./type_defs.md#mapiterationeventdetailstypedef) 
27. See [:material-code-braces: LambdaFunctionFailedEventDetailsTypeDef](./type_defs.md#lambdafunctionfailedeventdetailstypedef) 
28. See [:material-code-braces: LambdaFunctionScheduleFailedEventDetailsTypeDef](./type_defs.md#lambdafunctionschedulefailedeventdetailstypedef) 
29. See [:material-code-braces: LambdaFunctionScheduledEventDetailsTypeDef](./type_defs.md#lambdafunctionscheduledeventdetailstypedef) 
30. See [:material-code-braces: LambdaFunctionStartFailedEventDetailsTypeDef](./type_defs.md#lambdafunctionstartfailedeventdetailstypedef) 
31. See [:material-code-braces: LambdaFunctionSucceededEventDetailsTypeDef](./type_defs.md#lambdafunctionsucceededeventdetailstypedef) 
32. See [:material-code-braces: LambdaFunctionTimedOutEventDetailsTypeDef](./type_defs.md#lambdafunctiontimedouteventdetailstypedef) 
33. See [:material-code-braces: StateEnteredEventDetailsTypeDef](./type_defs.md#stateenteredeventdetailstypedef) 
34. See [:material-code-braces: StateExitedEventDetailsTypeDef](./type_defs.md#stateexitedeventdetailstypedef) 
35. See [:material-code-braces: MapRunStartedEventDetailsTypeDef](./type_defs.md#maprunstartedeventdetailstypedef) 
36. See [:material-code-braces: MapRunFailedEventDetailsTypeDef](./type_defs.md#maprunfailedeventdetailstypedef) 
37. See [:material-code-braces: MapRunRedrivenEventDetailsTypeDef](./type_defs.md#maprunredriveneventdetailstypedef) 
38. See [:material-code-braces: EvaluationFailedEventDetailsTypeDef](./type_defs.md#evaluationfailedeventdetailstypedef) 
## DescribeStateMachineForExecutionOutputTypeDef

```python
# DescribeStateMachineForExecutionOutputTypeDef definition

class DescribeStateMachineForExecutionOutputTypeDef(TypedDict):
    stateMachineArn: str,
    name: str,
    definition: str,
    roleArn: str,
    updateDate: datetime,
    loggingConfiguration: LoggingConfigurationOutputTypeDef,  # (1)
    tracingConfiguration: TracingConfigurationTypeDef,  # (2)
    mapRunArn: str,
    label: str,
    revisionId: str,
    encryptionConfiguration: EncryptionConfigurationTypeDef,  # (3)
    variableReferences: Dict[str, List[str]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: LoggingConfigurationOutputTypeDef](./type_defs.md#loggingconfigurationoutputtypedef) 
2. See [:material-code-braces: TracingConfigurationTypeDef](./type_defs.md#tracingconfigurationtypedef) 
3. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeStateMachineOutputTypeDef

```python
# DescribeStateMachineOutputTypeDef definition

class DescribeStateMachineOutputTypeDef(TypedDict):
    stateMachineArn: str,
    name: str,
    status: StateMachineStatusType,  # (1)
    definition: str,
    roleArn: str,
    type: StateMachineTypeType,  # (2)
    creationDate: datetime,
    loggingConfiguration: LoggingConfigurationOutputTypeDef,  # (3)
    tracingConfiguration: TracingConfigurationTypeDef,  # (4)
    label: str,
    revisionId: str,
    description: str,
    encryptionConfiguration: EncryptionConfigurationTypeDef,  # (5)
    variableReferences: Dict[str, List[str]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: StateMachineStatusType](./literals.md#statemachinestatustype) 
2. See [:material-code-brackets: StateMachineTypeType](./literals.md#statemachinetypetype) 
3. See [:material-code-braces: LoggingConfigurationOutputTypeDef](./type_defs.md#loggingconfigurationoutputtypedef) 
4. See [:material-code-braces: TracingConfigurationTypeDef](./type_defs.md#tracingconfigurationtypedef) 
5. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStateMachineInputRequestTypeDef

```python
# CreateStateMachineInputRequestTypeDef definition

class CreateStateMachineInputRequestTypeDef(TypedDict):
    name: str,
    definition: str,
    roleArn: str,
    type: NotRequired[StateMachineTypeType],  # (1)
    loggingConfiguration: NotRequired[LoggingConfigurationTypeDef],  # (2)
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    tracingConfiguration: NotRequired[TracingConfigurationTypeDef],  # (4)
    publish: NotRequired[bool],
    versionDescription: NotRequired[str],
    encryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (5)
```

1. See [:material-code-brackets: StateMachineTypeType](./literals.md#statemachinetypetype) 
2. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: TracingConfigurationTypeDef](./type_defs.md#tracingconfigurationtypedef) 
5. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
## UpdateStateMachineInputRequestTypeDef

```python
# UpdateStateMachineInputRequestTypeDef definition

class UpdateStateMachineInputRequestTypeDef(TypedDict):
    stateMachineArn: str,
    definition: NotRequired[str],
    roleArn: NotRequired[str],
    loggingConfiguration: NotRequired[LoggingConfigurationTypeDef],  # (1)
    tracingConfiguration: NotRequired[TracingConfigurationTypeDef],  # (2)
    publish: NotRequired[bool],
    versionDescription: NotRequired[str],
    encryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
2. See [:material-code-braces: TracingConfigurationTypeDef](./type_defs.md#tracingconfigurationtypedef) 
3. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
## GetExecutionHistoryOutputTypeDef

```python
# GetExecutionHistoryOutputTypeDef definition

class GetExecutionHistoryOutputTypeDef(TypedDict):
    events: List[HistoryEventTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: HistoryEventTypeDef](./type_defs.md#historyeventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
