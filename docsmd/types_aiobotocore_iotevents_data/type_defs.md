# Type definitions

> [Index](../README.md) > [IoTEventsData](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IoTEventsData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#ioteventsdata)
    type annotations stubs module [types-aiobotocore-iotevents-data](https://pypi.org/project/types-aiobotocore-iotevents-data/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_iotevents_data.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


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
# AcknowledgeActionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import AcknowledgeActionConfigurationTypeDef


def get_value() -> AcknowledgeActionConfigurationTypeDef:
    return {
        "note": ...,
    }


# AcknowledgeActionConfigurationTypeDef definition

class AcknowledgeActionConfigurationTypeDef(TypedDict):
    note: NotRequired[str],
```

## AcknowledgeAlarmActionRequestTypeDef

```python
# AcknowledgeAlarmActionRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import AcknowledgeAlarmActionRequestTypeDef


def get_value() -> AcknowledgeAlarmActionRequestTypeDef:
    return {
        "requestId": ...,
    }


# AcknowledgeAlarmActionRequestTypeDef definition

class AcknowledgeAlarmActionRequestTypeDef(TypedDict):
    requestId: str,
    alarmModelName: str,
    keyValue: NotRequired[str],
    note: NotRequired[str],
```

## AlarmSummaryTypeDef

```python
# AlarmSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import AlarmSummaryTypeDef


def get_value() -> AlarmSummaryTypeDef:
    return {
        "alarmModelName": ...,
    }


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
# BatchAlarmActionErrorEntryTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import BatchAlarmActionErrorEntryTypeDef


def get_value() -> BatchAlarmActionErrorEntryTypeDef:
    return {
        "requestId": ...,
    }


# BatchAlarmActionErrorEntryTypeDef definition

class BatchAlarmActionErrorEntryTypeDef(TypedDict):
    requestId: NotRequired[str],
    errorCode: NotRequired[ErrorCodeType],  # (1)
    errorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


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
# BatchDeleteDetectorErrorEntryTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import BatchDeleteDetectorErrorEntryTypeDef


def get_value() -> BatchDeleteDetectorErrorEntryTypeDef:
    return {
        "messageId": ...,
    }


# BatchDeleteDetectorErrorEntryTypeDef definition

class BatchDeleteDetectorErrorEntryTypeDef(TypedDict):
    messageId: NotRequired[str],
    errorCode: NotRequired[ErrorCodeType],  # (1)
    errorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## DeleteDetectorRequestTypeDef

```python
# DeleteDetectorRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import DeleteDetectorRequestTypeDef


def get_value() -> DeleteDetectorRequestTypeDef:
    return {
        "messageId": ...,
    }


# DeleteDetectorRequestTypeDef definition

class DeleteDetectorRequestTypeDef(TypedDict):
    messageId: str,
    detectorModelName: str,
    keyValue: NotRequired[str],
```

## DisableAlarmActionRequestTypeDef

```python
# DisableAlarmActionRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import DisableAlarmActionRequestTypeDef


def get_value() -> DisableAlarmActionRequestTypeDef:
    return {
        "requestId": ...,
    }


# DisableAlarmActionRequestTypeDef definition

class DisableAlarmActionRequestTypeDef(TypedDict):
    requestId: str,
    alarmModelName: str,
    keyValue: NotRequired[str],
    note: NotRequired[str],
```

## EnableAlarmActionRequestTypeDef

```python
# EnableAlarmActionRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import EnableAlarmActionRequestTypeDef


def get_value() -> EnableAlarmActionRequestTypeDef:
    return {
        "requestId": ...,
    }


# EnableAlarmActionRequestTypeDef definition

class EnableAlarmActionRequestTypeDef(TypedDict):
    requestId: str,
    alarmModelName: str,
    keyValue: NotRequired[str],
    note: NotRequired[str],
```

## BatchPutMessageErrorEntryTypeDef

```python
# BatchPutMessageErrorEntryTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import BatchPutMessageErrorEntryTypeDef


def get_value() -> BatchPutMessageErrorEntryTypeDef:
    return {
        "messageId": ...,
    }


# BatchPutMessageErrorEntryTypeDef definition

class BatchPutMessageErrorEntryTypeDef(TypedDict):
    messageId: NotRequired[str],
    errorCode: NotRequired[ErrorCodeType],  # (1)
    errorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## ResetAlarmActionRequestTypeDef

```python
# ResetAlarmActionRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import ResetAlarmActionRequestTypeDef


def get_value() -> ResetAlarmActionRequestTypeDef:
    return {
        "requestId": ...,
    }


# ResetAlarmActionRequestTypeDef definition

class ResetAlarmActionRequestTypeDef(TypedDict):
    requestId: str,
    alarmModelName: str,
    keyValue: NotRequired[str],
    note: NotRequired[str],
```

## SnoozeAlarmActionRequestTypeDef

```python
# SnoozeAlarmActionRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import SnoozeAlarmActionRequestTypeDef


def get_value() -> SnoozeAlarmActionRequestTypeDef:
    return {
        "requestId": ...,
    }


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
# BatchUpdateDetectorErrorEntryTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import BatchUpdateDetectorErrorEntryTypeDef


def get_value() -> BatchUpdateDetectorErrorEntryTypeDef:
    return {
        "messageId": ...,
    }


# BatchUpdateDetectorErrorEntryTypeDef definition

class BatchUpdateDetectorErrorEntryTypeDef(TypedDict):
    messageId: NotRequired[str],
    errorCode: NotRequired[ErrorCodeType],  # (1)
    errorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## DisableActionConfigurationTypeDef

```python
# DisableActionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import DisableActionConfigurationTypeDef


def get_value() -> DisableActionConfigurationTypeDef:
    return {
        "note": ...,
    }


# DisableActionConfigurationTypeDef definition

class DisableActionConfigurationTypeDef(TypedDict):
    note: NotRequired[str],
```

## EnableActionConfigurationTypeDef

```python
# EnableActionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import EnableActionConfigurationTypeDef


def get_value() -> EnableActionConfigurationTypeDef:
    return {
        "note": ...,
    }


# EnableActionConfigurationTypeDef definition

class EnableActionConfigurationTypeDef(TypedDict):
    note: NotRequired[str],
```

## ResetActionConfigurationTypeDef

```python
# ResetActionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import ResetActionConfigurationTypeDef


def get_value() -> ResetActionConfigurationTypeDef:
    return {
        "note": ...,
    }


# ResetActionConfigurationTypeDef definition

class ResetActionConfigurationTypeDef(TypedDict):
    note: NotRequired[str],
```

## SnoozeActionConfigurationTypeDef

```python
# SnoozeActionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import SnoozeActionConfigurationTypeDef


def get_value() -> SnoozeActionConfigurationTypeDef:
    return {
        "snoozeDuration": ...,
    }


# SnoozeActionConfigurationTypeDef definition

class SnoozeActionConfigurationTypeDef(TypedDict):
    snoozeDuration: NotRequired[int],
    note: NotRequired[str],
```

## DescribeAlarmRequestTypeDef

```python
# DescribeAlarmRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import DescribeAlarmRequestTypeDef


def get_value() -> DescribeAlarmRequestTypeDef:
    return {
        "alarmModelName": ...,
    }


# DescribeAlarmRequestTypeDef definition

class DescribeAlarmRequestTypeDef(TypedDict):
    alarmModelName: str,
    keyValue: NotRequired[str],
```

## DescribeDetectorRequestTypeDef

```python
# DescribeDetectorRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import DescribeDetectorRequestTypeDef


def get_value() -> DescribeDetectorRequestTypeDef:
    return {
        "detectorModelName": ...,
    }


# DescribeDetectorRequestTypeDef definition

class DescribeDetectorRequestTypeDef(TypedDict):
    detectorModelName: str,
    keyValue: NotRequired[str],
```

## TimerDefinitionTypeDef

```python
# TimerDefinitionTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import TimerDefinitionTypeDef


def get_value() -> TimerDefinitionTypeDef:
    return {
        "name": ...,
    }


# TimerDefinitionTypeDef definition

class TimerDefinitionTypeDef(TypedDict):
    name: str,
    seconds: int,
```

## VariableDefinitionTypeDef

```python
# VariableDefinitionTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import VariableDefinitionTypeDef


def get_value() -> VariableDefinitionTypeDef:
    return {
        "name": ...,
    }


# VariableDefinitionTypeDef definition

class VariableDefinitionTypeDef(TypedDict):
    name: str,
    value: str,
```

## DetectorStateSummaryTypeDef

```python
# DetectorStateSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import DetectorStateSummaryTypeDef


def get_value() -> DetectorStateSummaryTypeDef:
    return {
        "stateName": ...,
    }


# DetectorStateSummaryTypeDef definition

class DetectorStateSummaryTypeDef(TypedDict):
    stateName: NotRequired[str],
```

## TimerTypeDef

```python
# TimerTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import TimerTypeDef


def get_value() -> TimerTypeDef:
    return {
        "name": ...,
    }


# TimerTypeDef definition

class TimerTypeDef(TypedDict):
    name: str,
    timestamp: datetime,
```

## VariableTypeDef

```python
# VariableTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import VariableTypeDef


def get_value() -> VariableTypeDef:
    return {
        "name": ...,
    }


# VariableTypeDef definition

class VariableTypeDef(TypedDict):
    name: str,
    value: str,
```

## ListAlarmsRequestTypeDef

```python
# ListAlarmsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import ListAlarmsRequestTypeDef


def get_value() -> ListAlarmsRequestTypeDef:
    return {
        "alarmModelName": ...,
    }


# ListAlarmsRequestTypeDef definition

class ListAlarmsRequestTypeDef(TypedDict):
    alarmModelName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDetectorsRequestTypeDef

```python
# ListDetectorsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import ListDetectorsRequestTypeDef


def get_value() -> ListDetectorsRequestTypeDef:
    return {
        "detectorModelName": ...,
    }


# ListDetectorsRequestTypeDef definition

class ListDetectorsRequestTypeDef(TypedDict):
    detectorModelName: str,
    stateName: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## TimestampValueTypeDef

```python
# TimestampValueTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import TimestampValueTypeDef


def get_value() -> TimestampValueTypeDef:
    return {
        "timeInMillis": ...,
    }


# TimestampValueTypeDef definition

class TimestampValueTypeDef(TypedDict):
    timeInMillis: NotRequired[int],
```

## SimpleRuleEvaluationTypeDef

```python
# SimpleRuleEvaluationTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import SimpleRuleEvaluationTypeDef


def get_value() -> SimpleRuleEvaluationTypeDef:
    return {
        "inputPropertyValue": ...,
    }


# SimpleRuleEvaluationTypeDef definition

class SimpleRuleEvaluationTypeDef(TypedDict):
    inputPropertyValue: NotRequired[str],
    operator: NotRequired[ComparisonOperatorType],  # (1)
    thresholdValue: NotRequired[str],
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## StateChangeConfigurationTypeDef

```python
# StateChangeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import StateChangeConfigurationTypeDef


def get_value() -> StateChangeConfigurationTypeDef:
    return {
        "triggerType": ...,
    }


# StateChangeConfigurationTypeDef definition

class StateChangeConfigurationTypeDef(TypedDict):
    triggerType: NotRequired[TriggerTypeType],  # (1)
```

1. See [:material-code-brackets: TriggerTypeType](./literals.md#triggertypetype) 
## BatchAcknowledgeAlarmRequestTypeDef

```python
# BatchAcknowledgeAlarmRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import BatchAcknowledgeAlarmRequestTypeDef


def get_value() -> BatchAcknowledgeAlarmRequestTypeDef:
    return {
        "acknowledgeActionRequests": ...,
    }


# BatchAcknowledgeAlarmRequestTypeDef definition

class BatchAcknowledgeAlarmRequestTypeDef(TypedDict):
    acknowledgeActionRequests: Sequence[AcknowledgeAlarmActionRequestTypeDef],  # (1)
```

1. See [:material-code-braces: AcknowledgeAlarmActionRequestTypeDef](./type_defs.md#acknowledgealarmactionrequesttypedef) 
## BatchAcknowledgeAlarmResponseTypeDef

```python
# BatchAcknowledgeAlarmResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import BatchAcknowledgeAlarmResponseTypeDef


def get_value() -> BatchAcknowledgeAlarmResponseTypeDef:
    return {
        "errorEntries": ...,
    }


# BatchAcknowledgeAlarmResponseTypeDef definition

class BatchAcknowledgeAlarmResponseTypeDef(TypedDict):
    errorEntries: List[BatchAlarmActionErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchAlarmActionErrorEntryTypeDef](./type_defs.md#batchalarmactionerrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDisableAlarmResponseTypeDef

```python
# BatchDisableAlarmResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import BatchDisableAlarmResponseTypeDef


def get_value() -> BatchDisableAlarmResponseTypeDef:
    return {
        "errorEntries": ...,
    }


# BatchDisableAlarmResponseTypeDef definition

class BatchDisableAlarmResponseTypeDef(TypedDict):
    errorEntries: List[BatchAlarmActionErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchAlarmActionErrorEntryTypeDef](./type_defs.md#batchalarmactionerrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchEnableAlarmResponseTypeDef

```python
# BatchEnableAlarmResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import BatchEnableAlarmResponseTypeDef


def get_value() -> BatchEnableAlarmResponseTypeDef:
    return {
        "errorEntries": ...,
    }


# BatchEnableAlarmResponseTypeDef definition

class BatchEnableAlarmResponseTypeDef(TypedDict):
    errorEntries: List[BatchAlarmActionErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchAlarmActionErrorEntryTypeDef](./type_defs.md#batchalarmactionerrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchResetAlarmResponseTypeDef

```python
# BatchResetAlarmResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import BatchResetAlarmResponseTypeDef


def get_value() -> BatchResetAlarmResponseTypeDef:
    return {
        "errorEntries": ...,
    }


# BatchResetAlarmResponseTypeDef definition

class BatchResetAlarmResponseTypeDef(TypedDict):
    errorEntries: List[BatchAlarmActionErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchAlarmActionErrorEntryTypeDef](./type_defs.md#batchalarmactionerrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchSnoozeAlarmResponseTypeDef

```python
# BatchSnoozeAlarmResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import BatchSnoozeAlarmResponseTypeDef


def get_value() -> BatchSnoozeAlarmResponseTypeDef:
    return {
        "errorEntries": ...,
    }


# BatchSnoozeAlarmResponseTypeDef definition

class BatchSnoozeAlarmResponseTypeDef(TypedDict):
    errorEntries: List[BatchAlarmActionErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchAlarmActionErrorEntryTypeDef](./type_defs.md#batchalarmactionerrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAlarmsResponseTypeDef

```python
# ListAlarmsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import ListAlarmsResponseTypeDef


def get_value() -> ListAlarmsResponseTypeDef:
    return {
        "alarmSummaries": ...,
    }


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
# BatchDeleteDetectorResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import BatchDeleteDetectorResponseTypeDef


def get_value() -> BatchDeleteDetectorResponseTypeDef:
    return {
        "batchDeleteDetectorErrorEntries": ...,
    }


# BatchDeleteDetectorResponseTypeDef definition

class BatchDeleteDetectorResponseTypeDef(TypedDict):
    batchDeleteDetectorErrorEntries: List[BatchDeleteDetectorErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchDeleteDetectorErrorEntryTypeDef](./type_defs.md#batchdeletedetectorerrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteDetectorRequestTypeDef

```python
# BatchDeleteDetectorRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import BatchDeleteDetectorRequestTypeDef


def get_value() -> BatchDeleteDetectorRequestTypeDef:
    return {
        "detectors": ...,
    }


# BatchDeleteDetectorRequestTypeDef definition

class BatchDeleteDetectorRequestTypeDef(TypedDict):
    detectors: Sequence[DeleteDetectorRequestTypeDef],  # (1)
```

1. See [:material-code-braces: DeleteDetectorRequestTypeDef](./type_defs.md#deletedetectorrequesttypedef) 
## BatchDisableAlarmRequestTypeDef

```python
# BatchDisableAlarmRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import BatchDisableAlarmRequestTypeDef


def get_value() -> BatchDisableAlarmRequestTypeDef:
    return {
        "disableActionRequests": ...,
    }


# BatchDisableAlarmRequestTypeDef definition

class BatchDisableAlarmRequestTypeDef(TypedDict):
    disableActionRequests: Sequence[DisableAlarmActionRequestTypeDef],  # (1)
```

1. See [:material-code-braces: DisableAlarmActionRequestTypeDef](./type_defs.md#disablealarmactionrequesttypedef) 
## BatchEnableAlarmRequestTypeDef

```python
# BatchEnableAlarmRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import BatchEnableAlarmRequestTypeDef


def get_value() -> BatchEnableAlarmRequestTypeDef:
    return {
        "enableActionRequests": ...,
    }


# BatchEnableAlarmRequestTypeDef definition

class BatchEnableAlarmRequestTypeDef(TypedDict):
    enableActionRequests: Sequence[EnableAlarmActionRequestTypeDef],  # (1)
```

1. See [:material-code-braces: EnableAlarmActionRequestTypeDef](./type_defs.md#enablealarmactionrequesttypedef) 
## BatchPutMessageResponseTypeDef

```python
# BatchPutMessageResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import BatchPutMessageResponseTypeDef


def get_value() -> BatchPutMessageResponseTypeDef:
    return {
        "BatchPutMessageErrorEntries": ...,
    }


# BatchPutMessageResponseTypeDef definition

class BatchPutMessageResponseTypeDef(TypedDict):
    BatchPutMessageErrorEntries: List[BatchPutMessageErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchPutMessageErrorEntryTypeDef](./type_defs.md#batchputmessageerrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchResetAlarmRequestTypeDef

```python
# BatchResetAlarmRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import BatchResetAlarmRequestTypeDef


def get_value() -> BatchResetAlarmRequestTypeDef:
    return {
        "resetActionRequests": ...,
    }


# BatchResetAlarmRequestTypeDef definition

class BatchResetAlarmRequestTypeDef(TypedDict):
    resetActionRequests: Sequence[ResetAlarmActionRequestTypeDef],  # (1)
```

1. See [:material-code-braces: ResetAlarmActionRequestTypeDef](./type_defs.md#resetalarmactionrequesttypedef) 
## BatchSnoozeAlarmRequestTypeDef

```python
# BatchSnoozeAlarmRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import BatchSnoozeAlarmRequestTypeDef


def get_value() -> BatchSnoozeAlarmRequestTypeDef:
    return {
        "snoozeActionRequests": ...,
    }


# BatchSnoozeAlarmRequestTypeDef definition

class BatchSnoozeAlarmRequestTypeDef(TypedDict):
    snoozeActionRequests: Sequence[SnoozeAlarmActionRequestTypeDef],  # (1)
```

1. See [:material-code-braces: SnoozeAlarmActionRequestTypeDef](./type_defs.md#snoozealarmactionrequesttypedef) 
## BatchUpdateDetectorResponseTypeDef

```python
# BatchUpdateDetectorResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import BatchUpdateDetectorResponseTypeDef


def get_value() -> BatchUpdateDetectorResponseTypeDef:
    return {
        "batchUpdateDetectorErrorEntries": ...,
    }


# BatchUpdateDetectorResponseTypeDef definition

class BatchUpdateDetectorResponseTypeDef(TypedDict):
    batchUpdateDetectorErrorEntries: List[BatchUpdateDetectorErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchUpdateDetectorErrorEntryTypeDef](./type_defs.md#batchupdatedetectorerrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CustomerActionTypeDef

```python
# CustomerActionTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import CustomerActionTypeDef


def get_value() -> CustomerActionTypeDef:
    return {
        "actionName": ...,
    }


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
# DetectorStateDefinitionTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import DetectorStateDefinitionTypeDef


def get_value() -> DetectorStateDefinitionTypeDef:
    return {
        "stateName": ...,
    }


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
# DetectorSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import DetectorSummaryTypeDef


def get_value() -> DetectorSummaryTypeDef:
    return {
        "detectorModelName": ...,
    }


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
# DetectorStateTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import DetectorStateTypeDef


def get_value() -> DetectorStateTypeDef:
    return {
        "stateName": ...,
    }


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
# MessageTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import MessageTypeDef


def get_value() -> MessageTypeDef:
    return {
        "messageId": ...,
    }


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
# RuleEvaluationTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import RuleEvaluationTypeDef


def get_value() -> RuleEvaluationTypeDef:
    return {
        "simpleRuleEvaluation": ...,
    }


# RuleEvaluationTypeDef definition

class RuleEvaluationTypeDef(TypedDict):
    simpleRuleEvaluation: NotRequired[SimpleRuleEvaluationTypeDef],  # (1)
```

1. See [:material-code-braces: SimpleRuleEvaluationTypeDef](./type_defs.md#simpleruleevaluationtypedef) 
## SystemEventTypeDef

```python
# SystemEventTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import SystemEventTypeDef


def get_value() -> SystemEventTypeDef:
    return {
        "eventType": ...,
    }


# SystemEventTypeDef definition

class SystemEventTypeDef(TypedDict):
    eventType: NotRequired[EventTypeType],  # (1)
    stateChangeConfiguration: NotRequired[StateChangeConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
2. See [:material-code-braces: StateChangeConfigurationTypeDef](./type_defs.md#statechangeconfigurationtypedef) 
## UpdateDetectorRequestTypeDef

```python
# UpdateDetectorRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import UpdateDetectorRequestTypeDef


def get_value() -> UpdateDetectorRequestTypeDef:
    return {
        "messageId": ...,
    }


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
# ListDetectorsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import ListDetectorsResponseTypeDef


def get_value() -> ListDetectorsResponseTypeDef:
    return {
        "detectorSummaries": ...,
    }


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
# DetectorTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import DetectorTypeDef


def get_value() -> DetectorTypeDef:
    return {
        "detectorModelName": ...,
    }


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
## BatchPutMessageRequestTypeDef

```python
# BatchPutMessageRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import BatchPutMessageRequestTypeDef


def get_value() -> BatchPutMessageRequestTypeDef:
    return {
        "messages": ...,
    }


# BatchPutMessageRequestTypeDef definition

class BatchPutMessageRequestTypeDef(TypedDict):
    messages: Sequence[MessageTypeDef],  # (1)
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
## AlarmStateTypeDef

```python
# AlarmStateTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import AlarmStateTypeDef


def get_value() -> AlarmStateTypeDef:
    return {
        "stateName": ...,
    }


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
## BatchUpdateDetectorRequestTypeDef

```python
# BatchUpdateDetectorRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import BatchUpdateDetectorRequestTypeDef


def get_value() -> BatchUpdateDetectorRequestTypeDef:
    return {
        "detectors": ...,
    }


# BatchUpdateDetectorRequestTypeDef definition

class BatchUpdateDetectorRequestTypeDef(TypedDict):
    detectors: Sequence[UpdateDetectorRequestTypeDef],  # (1)
```

1. See [:material-code-braces: UpdateDetectorRequestTypeDef](./type_defs.md#updatedetectorrequesttypedef) 
## DescribeDetectorResponseTypeDef

```python
# DescribeDetectorResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import DescribeDetectorResponseTypeDef


def get_value() -> DescribeDetectorResponseTypeDef:
    return {
        "detector": ...,
    }


# DescribeDetectorResponseTypeDef definition

class DescribeDetectorResponseTypeDef(TypedDict):
    detector: DetectorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DetectorTypeDef](./type_defs.md#detectortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AlarmTypeDef

```python
# AlarmTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import AlarmTypeDef


def get_value() -> AlarmTypeDef:
    return {
        "alarmModelName": ...,
    }


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
# DescribeAlarmResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents_data.type_defs import DescribeAlarmResponseTypeDef


def get_value() -> DescribeAlarmResponseTypeDef:
    return {
        "alarm": ...,
    }


# DescribeAlarmResponseTypeDef definition

class DescribeAlarmResponseTypeDef(TypedDict):
    alarm: AlarmTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AlarmTypeDef](./type_defs.md#alarmtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
