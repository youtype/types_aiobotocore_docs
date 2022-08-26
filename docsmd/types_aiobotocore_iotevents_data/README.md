# IoTEventsData module

> [Index](../README.md) > IoTEventsData


!!! note ""

    Auto-generated documentation for [IoTEventsData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData)
    type annotations stubs module [types-aiobotocore-iotevents-data](https://pypi.org/project/types-aiobotocore-iotevents-data/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `IoTEventsData` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[iotevents-data]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[iotevents-data]'


# standalone installation
python -m pip install types-aiobotocore-iotevents-data
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-iotevents-data
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IoTEventsDataClient

Type annotations and code completion for  `#!python session.create_client("iotevents-data")` as [IoTEventsDataClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_iotevents_data.client import IoTEventsDataClient


session = get_session()
async with session.create_client("iotevents-data") as client:
    client: IoTEventsDataClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_iotevents_data.literals import AlarmStateNameType

def get_value() -> AlarmStateNameType:
    return "ACKNOWLEDGED"
```

- [AlarmStateNameType](./literals.md#alarmstatenametype)
- [ComparisonOperatorType](./literals.md#comparisonoperatortype)
- [CustomerActionNameType](./literals.md#customeractionnametype)
- [ErrorCodeType](./literals.md#errorcodetype)
- [EventTypeType](./literals.md#eventtypetype)
- [TriggerTypeType](./literals.md#triggertypetype)
- [IoTEventsDataServiceName](./literals.md#ioteventsdataservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_iotevents_data.type_defs import AcknowledgeActionConfigurationTypeDef

def get_value() -> AcknowledgeActionConfigurationTypeDef:
    return {
        "note": ...,
    }
```

- [AcknowledgeActionConfigurationTypeDef](./type_defs.md#acknowledgeactionconfigurationtypedef)
- [AcknowledgeAlarmActionRequestTypeDef](./type_defs.md#acknowledgealarmactionrequesttypedef)
- [AlarmSummaryTypeDef](./type_defs.md#alarmsummarytypedef)
- [BatchAlarmActionErrorEntryTypeDef](./type_defs.md#batchalarmactionerrorentrytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BatchDeleteDetectorErrorEntryTypeDef](./type_defs.md#batchdeletedetectorerrorentrytypedef)
- [DeleteDetectorRequestTypeDef](./type_defs.md#deletedetectorrequesttypedef)
- [DisableAlarmActionRequestTypeDef](./type_defs.md#disablealarmactionrequesttypedef)
- [EnableAlarmActionRequestTypeDef](./type_defs.md#enablealarmactionrequesttypedef)
- [BatchPutMessageErrorEntryTypeDef](./type_defs.md#batchputmessageerrorentrytypedef)
- [ResetAlarmActionRequestTypeDef](./type_defs.md#resetalarmactionrequesttypedef)
- [SnoozeAlarmActionRequestTypeDef](./type_defs.md#snoozealarmactionrequesttypedef)
- [BatchUpdateDetectorErrorEntryTypeDef](./type_defs.md#batchupdatedetectorerrorentrytypedef)
- [DisableActionConfigurationTypeDef](./type_defs.md#disableactionconfigurationtypedef)
- [EnableActionConfigurationTypeDef](./type_defs.md#enableactionconfigurationtypedef)
- [ResetActionConfigurationTypeDef](./type_defs.md#resetactionconfigurationtypedef)
- [SnoozeActionConfigurationTypeDef](./type_defs.md#snoozeactionconfigurationtypedef)
- [DescribeAlarmRequestRequestTypeDef](./type_defs.md#describealarmrequestrequesttypedef)
- [DescribeDetectorRequestRequestTypeDef](./type_defs.md#describedetectorrequestrequesttypedef)
- [TimerDefinitionTypeDef](./type_defs.md#timerdefinitiontypedef)
- [VariableDefinitionTypeDef](./type_defs.md#variabledefinitiontypedef)
- [DetectorStateSummaryTypeDef](./type_defs.md#detectorstatesummarytypedef)
- [TimerTypeDef](./type_defs.md#timertypedef)
- [VariableTypeDef](./type_defs.md#variabletypedef)
- [ListAlarmsRequestRequestTypeDef](./type_defs.md#listalarmsrequestrequesttypedef)
- [ListDetectorsRequestRequestTypeDef](./type_defs.md#listdetectorsrequestrequesttypedef)
- [TimestampValueTypeDef](./type_defs.md#timestampvaluetypedef)
- [SimpleRuleEvaluationTypeDef](./type_defs.md#simpleruleevaluationtypedef)
- [StateChangeConfigurationTypeDef](./type_defs.md#statechangeconfigurationtypedef)
- [BatchAcknowledgeAlarmRequestRequestTypeDef](./type_defs.md#batchacknowledgealarmrequestrequesttypedef)
- [BatchAcknowledgeAlarmResponseTypeDef](./type_defs.md#batchacknowledgealarmresponsetypedef)
- [BatchDisableAlarmResponseTypeDef](./type_defs.md#batchdisablealarmresponsetypedef)
- [BatchEnableAlarmResponseTypeDef](./type_defs.md#batchenablealarmresponsetypedef)
- [BatchResetAlarmResponseTypeDef](./type_defs.md#batchresetalarmresponsetypedef)
- [BatchSnoozeAlarmResponseTypeDef](./type_defs.md#batchsnoozealarmresponsetypedef)
- [ListAlarmsResponseTypeDef](./type_defs.md#listalarmsresponsetypedef)
- [BatchDeleteDetectorResponseTypeDef](./type_defs.md#batchdeletedetectorresponsetypedef)
- [BatchDeleteDetectorRequestRequestTypeDef](./type_defs.md#batchdeletedetectorrequestrequesttypedef)
- [BatchDisableAlarmRequestRequestTypeDef](./type_defs.md#batchdisablealarmrequestrequesttypedef)
- [BatchEnableAlarmRequestRequestTypeDef](./type_defs.md#batchenablealarmrequestrequesttypedef)
- [BatchPutMessageResponseTypeDef](./type_defs.md#batchputmessageresponsetypedef)
- [BatchResetAlarmRequestRequestTypeDef](./type_defs.md#batchresetalarmrequestrequesttypedef)
- [BatchSnoozeAlarmRequestRequestTypeDef](./type_defs.md#batchsnoozealarmrequestrequesttypedef)
- [BatchUpdateDetectorResponseTypeDef](./type_defs.md#batchupdatedetectorresponsetypedef)
- [CustomerActionTypeDef](./type_defs.md#customeractiontypedef)
- [DetectorStateDefinitionTypeDef](./type_defs.md#detectorstatedefinitiontypedef)
- [DetectorSummaryTypeDef](./type_defs.md#detectorsummarytypedef)
- [DetectorStateTypeDef](./type_defs.md#detectorstatetypedef)
- [MessageTypeDef](./type_defs.md#messagetypedef)
- [RuleEvaluationTypeDef](./type_defs.md#ruleevaluationtypedef)
- [SystemEventTypeDef](./type_defs.md#systemeventtypedef)
- [UpdateDetectorRequestTypeDef](./type_defs.md#updatedetectorrequesttypedef)
- [ListDetectorsResponseTypeDef](./type_defs.md#listdetectorsresponsetypedef)
- [DetectorTypeDef](./type_defs.md#detectortypedef)
- [BatchPutMessageRequestRequestTypeDef](./type_defs.md#batchputmessagerequestrequesttypedef)
- [AlarmStateTypeDef](./type_defs.md#alarmstatetypedef)
- [BatchUpdateDetectorRequestRequestTypeDef](./type_defs.md#batchupdatedetectorrequestrequesttypedef)
- [DescribeDetectorResponseTypeDef](./type_defs.md#describedetectorresponsetypedef)
- [AlarmTypeDef](./type_defs.md#alarmtypedef)
- [DescribeAlarmResponseTypeDef](./type_defs.md#describealarmresponsetypedef)

