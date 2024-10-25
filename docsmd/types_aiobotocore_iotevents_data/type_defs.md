# Type definitions

> [Index](../README.md) > [IoTEventsData](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IoTEventsData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData)
    type annotations stubs module [types-aiobotocore-iotevents-data](https://pypi.org/project/types-aiobotocore-iotevents-data/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```




## AcknowledgeActionConfigurationTypeDef

```python
# AcknowledgeActionConfigurationTypeDef definition

class AcknowledgeActionConfigurationTypeDef(TypedDict):
    note: NotRequired[str],
```

## AcknowledgeAlarmActionRequestTypeDef

```python
# AcknowledgeAlarmActionRequestTypeDef definition

class AcknowledgeAlarmActionRequestTypeDef(TypedDict):
    requestId: str,
    alarmModelName: str,
    keyValue: NotRequired[str],
    note: NotRequired[str],
```

## AlarmSummaryTypeDef

```python
# AlarmSummaryTypeDef definition

class AlarmSummaryTypeDef(TypedDict):
    alarmModelName: NotRequired[str],
    alarmModelVersion: NotRequired[str],
    keyValue: NotRequired[str],
    stateName: NotRequired[AlarmStateNameType],  # (1)
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: AlarmStateNameType](./literals.md#alarmstatenametype) 
## BatchAlarmActionErrorEntryTypeDef

```python
# BatchAlarmActionErrorEntryTypeDef definition

class BatchAlarmActionErrorEntryTypeDef(TypedDict):
    requestId: NotRequired[str],
    errorCode: NotRequired[ErrorCodeType],  # (1)
    errorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
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

## BatchDeleteDetectorErrorEntryTypeDef

```python
# BatchDeleteDetectorErrorEntryTypeDef definition

class BatchDeleteDetectorErrorEntryTypeDef(TypedDict):
    messageId: NotRequired[str],
    errorCode: NotRequired[ErrorCodeType],  # (1)
    errorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## DeleteDetectorRequestTypeDef

```python
# DeleteDetectorRequestTypeDef definition

class DeleteDetectorRequestTypeDef(TypedDict):
    messageId: str,
    detectorModelName: str,
    keyValue: NotRequired[str],
```

## DisableAlarmActionRequestTypeDef

```python
# DisableAlarmActionRequestTypeDef definition

class DisableAlarmActionRequestTypeDef(TypedDict):
    requestId: str,
    alarmModelName: str,
    keyValue: NotRequired[str],
    note: NotRequired[str],
```

## EnableAlarmActionRequestTypeDef

```python
# EnableAlarmActionRequestTypeDef definition

class EnableAlarmActionRequestTypeDef(TypedDict):
    requestId: str,
    alarmModelName: str,
    keyValue: NotRequired[str],
    note: NotRequired[str],
```

## BatchPutMessageErrorEntryTypeDef

```python
# BatchPutMessageErrorEntryTypeDef definition

class BatchPutMessageErrorEntryTypeDef(TypedDict):
    messageId: NotRequired[str],
    errorCode: NotRequired[ErrorCodeType],  # (1)
    errorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## ResetAlarmActionRequestTypeDef

```python
# ResetAlarmActionRequestTypeDef definition

class ResetAlarmActionRequestTypeDef(TypedDict):
    requestId: str,
    alarmModelName: str,
    keyValue: NotRequired[str],
    note: NotRequired[str],
```

## SnoozeAlarmActionRequestTypeDef

```python
# SnoozeAlarmActionRequestTypeDef definition

class SnoozeAlarmActionRequestTypeDef(TypedDict):
    requestId: str,
    alarmModelName: str,
    snoozeDuration: int,
    keyValue: NotRequired[str],
    note: NotRequired[str],
```

## BatchUpdateDetectorErrorEntryTypeDef

```python
# BatchUpdateDetectorErrorEntryTypeDef definition

class BatchUpdateDetectorErrorEntryTypeDef(TypedDict):
    messageId: NotRequired[str],
    errorCode: NotRequired[ErrorCodeType],  # (1)
    errorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## DisableActionConfigurationTypeDef

```python
# DisableActionConfigurationTypeDef definition

class DisableActionConfigurationTypeDef(TypedDict):
    note: NotRequired[str],
```

## EnableActionConfigurationTypeDef

```python
# EnableActionConfigurationTypeDef definition

class EnableActionConfigurationTypeDef(TypedDict):
    note: NotRequired[str],
```

## ResetActionConfigurationTypeDef

```python
# ResetActionConfigurationTypeDef definition

class ResetActionConfigurationTypeDef(TypedDict):
    note: NotRequired[str],
```

## SnoozeActionConfigurationTypeDef

```python
# SnoozeActionConfigurationTypeDef definition

class SnoozeActionConfigurationTypeDef(TypedDict):
    snoozeDuration: NotRequired[int],
    note: NotRequired[str],
```

## DescribeAlarmRequestRequestTypeDef

```python
# DescribeAlarmRequestRequestTypeDef definition

class DescribeAlarmRequestRequestTypeDef(TypedDict):
    alarmModelName: str,
    keyValue: NotRequired[str],
```

## DescribeDetectorRequestRequestTypeDef

```python
# DescribeDetectorRequestRequestTypeDef definition

class DescribeDetectorRequestRequestTypeDef(TypedDict):
    detectorModelName: str,
    keyValue: NotRequired[str],
```

## TimerDefinitionTypeDef

```python
# TimerDefinitionTypeDef definition

class TimerDefinitionTypeDef(TypedDict):
    name: str,
    seconds: int,
```

## VariableDefinitionTypeDef

```python
# VariableDefinitionTypeDef definition

class VariableDefinitionTypeDef(TypedDict):
    name: str,
    value: str,
```

## DetectorStateSummaryTypeDef

```python
# DetectorStateSummaryTypeDef definition

class DetectorStateSummaryTypeDef(TypedDict):
    stateName: NotRequired[str],
```

## TimerTypeDef

```python
# TimerTypeDef definition

class TimerTypeDef(TypedDict):
    name: str,
    timestamp: datetime,
```

## VariableTypeDef

```python
# VariableTypeDef definition

class VariableTypeDef(TypedDict):
    name: str,
    value: str,
```

## ListAlarmsRequestRequestTypeDef

```python
# ListAlarmsRequestRequestTypeDef definition

class ListAlarmsRequestRequestTypeDef(TypedDict):
    alarmModelName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDetectorsRequestRequestTypeDef

```python
# ListDetectorsRequestRequestTypeDef definition

class ListDetectorsRequestRequestTypeDef(TypedDict):
    detectorModelName: str,
    stateName: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## TimestampValueTypeDef

```python
# TimestampValueTypeDef definition

class TimestampValueTypeDef(TypedDict):
    timeInMillis: NotRequired[int],
```

## SimpleRuleEvaluationTypeDef

```python
# SimpleRuleEvaluationTypeDef definition

class SimpleRuleEvaluationTypeDef(TypedDict):
    inputPropertyValue: NotRequired[str],
    operator: NotRequired[ComparisonOperatorType],  # (1)
    thresholdValue: NotRequired[str],
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## StateChangeConfigurationTypeDef

```python
# StateChangeConfigurationTypeDef definition

class StateChangeConfigurationTypeDef(TypedDict):
    triggerType: NotRequired[TriggerTypeType],  # (1)
```

1. See [:material-code-brackets: TriggerTypeType](./literals.md#triggertypetype) 
## BatchAcknowledgeAlarmRequestRequestTypeDef

```python
# BatchAcknowledgeAlarmRequestRequestTypeDef definition

class BatchAcknowledgeAlarmRequestRequestTypeDef(TypedDict):
    acknowledgeActionRequests: Sequence[AcknowledgeAlarmActionRequestTypeDef],  # (1)
```

1. See [:material-code-braces: AcknowledgeAlarmActionRequestTypeDef](./type_defs.md#acknowledgealarmactionrequesttypedef) 
## BatchAcknowledgeAlarmResponseTypeDef

```python
# BatchAcknowledgeAlarmResponseTypeDef definition

class BatchAcknowledgeAlarmResponseTypeDef(TypedDict):
    errorEntries: List[BatchAlarmActionErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchAlarmActionErrorEntryTypeDef](./type_defs.md#batchalarmactionerrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDisableAlarmResponseTypeDef

```python
# BatchDisableAlarmResponseTypeDef definition

class BatchDisableAlarmResponseTypeDef(TypedDict):
    errorEntries: List[BatchAlarmActionErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchAlarmActionErrorEntryTypeDef](./type_defs.md#batchalarmactionerrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchEnableAlarmResponseTypeDef

```python
# BatchEnableAlarmResponseTypeDef definition

class BatchEnableAlarmResponseTypeDef(TypedDict):
    errorEntries: List[BatchAlarmActionErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchAlarmActionErrorEntryTypeDef](./type_defs.md#batchalarmactionerrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchResetAlarmResponseTypeDef

```python
# BatchResetAlarmResponseTypeDef definition

class BatchResetAlarmResponseTypeDef(TypedDict):
    errorEntries: List[BatchAlarmActionErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchAlarmActionErrorEntryTypeDef](./type_defs.md#batchalarmactionerrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchSnoozeAlarmResponseTypeDef

```python
# BatchSnoozeAlarmResponseTypeDef definition

class BatchSnoozeAlarmResponseTypeDef(TypedDict):
    errorEntries: List[BatchAlarmActionErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchAlarmActionErrorEntryTypeDef](./type_defs.md#batchalarmactionerrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAlarmsResponseTypeDef

```python
# ListAlarmsResponseTypeDef definition

class ListAlarmsResponseTypeDef(TypedDict):
    alarmSummaries: List[AlarmSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AlarmSummaryTypeDef](./type_defs.md#alarmsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteDetectorResponseTypeDef

```python
# BatchDeleteDetectorResponseTypeDef definition

class BatchDeleteDetectorResponseTypeDef(TypedDict):
    batchDeleteDetectorErrorEntries: List[BatchDeleteDetectorErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchDeleteDetectorErrorEntryTypeDef](./type_defs.md#batchdeletedetectorerrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteDetectorRequestRequestTypeDef

```python
# BatchDeleteDetectorRequestRequestTypeDef definition

class BatchDeleteDetectorRequestRequestTypeDef(TypedDict):
    detectors: Sequence[DeleteDetectorRequestTypeDef],  # (1)
```

1. See [:material-code-braces: DeleteDetectorRequestTypeDef](./type_defs.md#deletedetectorrequesttypedef) 
## BatchDisableAlarmRequestRequestTypeDef

```python
# BatchDisableAlarmRequestRequestTypeDef definition

class BatchDisableAlarmRequestRequestTypeDef(TypedDict):
    disableActionRequests: Sequence[DisableAlarmActionRequestTypeDef],  # (1)
```

1. See [:material-code-braces: DisableAlarmActionRequestTypeDef](./type_defs.md#disablealarmactionrequesttypedef) 
## BatchEnableAlarmRequestRequestTypeDef

```python
# BatchEnableAlarmRequestRequestTypeDef definition

class BatchEnableAlarmRequestRequestTypeDef(TypedDict):
    enableActionRequests: Sequence[EnableAlarmActionRequestTypeDef],  # (1)
```

1. See [:material-code-braces: EnableAlarmActionRequestTypeDef](./type_defs.md#enablealarmactionrequesttypedef) 
## BatchPutMessageResponseTypeDef

```python
# BatchPutMessageResponseTypeDef definition

class BatchPutMessageResponseTypeDef(TypedDict):
    BatchPutMessageErrorEntries: List[BatchPutMessageErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchPutMessageErrorEntryTypeDef](./type_defs.md#batchputmessageerrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchResetAlarmRequestRequestTypeDef

```python
# BatchResetAlarmRequestRequestTypeDef definition

class BatchResetAlarmRequestRequestTypeDef(TypedDict):
    resetActionRequests: Sequence[ResetAlarmActionRequestTypeDef],  # (1)
```

1. See [:material-code-braces: ResetAlarmActionRequestTypeDef](./type_defs.md#resetalarmactionrequesttypedef) 
## BatchSnoozeAlarmRequestRequestTypeDef

```python
# BatchSnoozeAlarmRequestRequestTypeDef definition

class BatchSnoozeAlarmRequestRequestTypeDef(TypedDict):
    snoozeActionRequests: Sequence[SnoozeAlarmActionRequestTypeDef],  # (1)
```

1. See [:material-code-braces: SnoozeAlarmActionRequestTypeDef](./type_defs.md#snoozealarmactionrequesttypedef) 
## BatchUpdateDetectorResponseTypeDef

```python
# BatchUpdateDetectorResponseTypeDef definition

class BatchUpdateDetectorResponseTypeDef(TypedDict):
    batchUpdateDetectorErrorEntries: List[BatchUpdateDetectorErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchUpdateDetectorErrorEntryTypeDef](./type_defs.md#batchupdatedetectorerrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CustomerActionTypeDef

```python
# CustomerActionTypeDef definition

class CustomerActionTypeDef(TypedDict):
    actionName: NotRequired[CustomerActionNameType],  # (1)
    snoozeActionConfiguration: NotRequired[SnoozeActionConfigurationTypeDef],  # (2)
    enableActionConfiguration: NotRequired[EnableActionConfigurationTypeDef],  # (3)
    disableActionConfiguration: NotRequired[DisableActionConfigurationTypeDef],  # (4)
    acknowledgeActionConfiguration: NotRequired[AcknowledgeActionConfigurationTypeDef],  # (5)
    resetActionConfiguration: NotRequired[ResetActionConfigurationTypeDef],  # (6)
```

1. See [:material-code-brackets: CustomerActionNameType](./literals.md#customeractionnametype) 
2. See [:material-code-braces: SnoozeActionConfigurationTypeDef](./type_defs.md#snoozeactionconfigurationtypedef) 
3. See [:material-code-braces: EnableActionConfigurationTypeDef](./type_defs.md#enableactionconfigurationtypedef) 
4. See [:material-code-braces: DisableActionConfigurationTypeDef](./type_defs.md#disableactionconfigurationtypedef) 
5. See [:material-code-braces: AcknowledgeActionConfigurationTypeDef](./type_defs.md#acknowledgeactionconfigurationtypedef) 
6. See [:material-code-braces: ResetActionConfigurationTypeDef](./type_defs.md#resetactionconfigurationtypedef) 
## DetectorStateDefinitionTypeDef

```python
# DetectorStateDefinitionTypeDef definition

class DetectorStateDefinitionTypeDef(TypedDict):
    stateName: str,
    variables: Sequence[VariableDefinitionTypeDef],  # (1)
    timers: Sequence[TimerDefinitionTypeDef],  # (2)
```

1. See [:material-code-braces: VariableDefinitionTypeDef](./type_defs.md#variabledefinitiontypedef) 
2. See [:material-code-braces: TimerDefinitionTypeDef](./type_defs.md#timerdefinitiontypedef) 
## DetectorSummaryTypeDef

```python
# DetectorSummaryTypeDef definition

class DetectorSummaryTypeDef(TypedDict):
    detectorModelName: NotRequired[str],
    keyValue: NotRequired[str],
    detectorModelVersion: NotRequired[str],
    state: NotRequired[DetectorStateSummaryTypeDef],  # (1)
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
```

1. See [:material-code-braces: DetectorStateSummaryTypeDef](./type_defs.md#detectorstatesummarytypedef) 
## DetectorStateTypeDef

```python
# DetectorStateTypeDef definition

class DetectorStateTypeDef(TypedDict):
    stateName: str,
    variables: List[VariableTypeDef],  # (1)
    timers: List[TimerTypeDef],  # (2)
```

1. See [:material-code-braces: VariableTypeDef](./type_defs.md#variabletypedef) 
2. See [:material-code-braces: TimerTypeDef](./type_defs.md#timertypedef) 
## MessageTypeDef

```python
# MessageTypeDef definition

class MessageTypeDef(TypedDict):
    messageId: str,
    inputName: str,
    payload: BlobTypeDef,
    timestamp: NotRequired[TimestampValueTypeDef],  # (1)
```

1. See [:material-code-braces: TimestampValueTypeDef](./type_defs.md#timestampvaluetypedef) 
## RuleEvaluationTypeDef

```python
# RuleEvaluationTypeDef definition

class RuleEvaluationTypeDef(TypedDict):
    simpleRuleEvaluation: NotRequired[SimpleRuleEvaluationTypeDef],  # (1)
```

1. See [:material-code-braces: SimpleRuleEvaluationTypeDef](./type_defs.md#simpleruleevaluationtypedef) 
## SystemEventTypeDef

```python
# SystemEventTypeDef definition

class SystemEventTypeDef(TypedDict):
    eventType: NotRequired[EventTypeType],  # (1)
    stateChangeConfiguration: NotRequired[StateChangeConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
2. See [:material-code-braces: StateChangeConfigurationTypeDef](./type_defs.md#statechangeconfigurationtypedef) 
## UpdateDetectorRequestTypeDef

```python
# UpdateDetectorRequestTypeDef definition

class UpdateDetectorRequestTypeDef(TypedDict):
    messageId: str,
    detectorModelName: str,
    state: DetectorStateDefinitionTypeDef,  # (1)
    keyValue: NotRequired[str],
```

1. See [:material-code-braces: DetectorStateDefinitionTypeDef](./type_defs.md#detectorstatedefinitiontypedef) 
## ListDetectorsResponseTypeDef

```python
# ListDetectorsResponseTypeDef definition

class ListDetectorsResponseTypeDef(TypedDict):
    detectorSummaries: List[DetectorSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DetectorSummaryTypeDef](./type_defs.md#detectorsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectorTypeDef

```python
# DetectorTypeDef definition

class DetectorTypeDef(TypedDict):
    detectorModelName: NotRequired[str],
    keyValue: NotRequired[str],
    detectorModelVersion: NotRequired[str],
    state: NotRequired[DetectorStateTypeDef],  # (1)
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
```

1. See [:material-code-braces: DetectorStateTypeDef](./type_defs.md#detectorstatetypedef) 
## BatchPutMessageRequestRequestTypeDef

```python
# BatchPutMessageRequestRequestTypeDef definition

class BatchPutMessageRequestRequestTypeDef(TypedDict):
    messages: Sequence[MessageTypeDef],  # (1)
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
## AlarmStateTypeDef

```python
# AlarmStateTypeDef definition

class AlarmStateTypeDef(TypedDict):
    stateName: NotRequired[AlarmStateNameType],  # (1)
    ruleEvaluation: NotRequired[RuleEvaluationTypeDef],  # (2)
    customerAction: NotRequired[CustomerActionTypeDef],  # (3)
    systemEvent: NotRequired[SystemEventTypeDef],  # (4)
```

1. See [:material-code-brackets: AlarmStateNameType](./literals.md#alarmstatenametype) 
2. See [:material-code-braces: RuleEvaluationTypeDef](./type_defs.md#ruleevaluationtypedef) 
3. See [:material-code-braces: CustomerActionTypeDef](./type_defs.md#customeractiontypedef) 
4. See [:material-code-braces: SystemEventTypeDef](./type_defs.md#systemeventtypedef) 
## BatchUpdateDetectorRequestRequestTypeDef

```python
# BatchUpdateDetectorRequestRequestTypeDef definition

class BatchUpdateDetectorRequestRequestTypeDef(TypedDict):
    detectors: Sequence[UpdateDetectorRequestTypeDef],  # (1)
```

1. See [:material-code-braces: UpdateDetectorRequestTypeDef](./type_defs.md#updatedetectorrequesttypedef) 
## DescribeDetectorResponseTypeDef

```python
# DescribeDetectorResponseTypeDef definition

class DescribeDetectorResponseTypeDef(TypedDict):
    detector: DetectorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DetectorTypeDef](./type_defs.md#detectortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AlarmTypeDef

```python
# AlarmTypeDef definition

class AlarmTypeDef(TypedDict):
    alarmModelName: NotRequired[str],
    alarmModelVersion: NotRequired[str],
    keyValue: NotRequired[str],
    alarmState: NotRequired[AlarmStateTypeDef],  # (1)
    severity: NotRequired[int],
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
```

1. See [:material-code-braces: AlarmStateTypeDef](./type_defs.md#alarmstatetypedef) 
## DescribeAlarmResponseTypeDef

```python
# DescribeAlarmResponseTypeDef definition

class DescribeAlarmResponseTypeDef(TypedDict):
    alarm: AlarmTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AlarmTypeDef](./type_defs.md#alarmtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
