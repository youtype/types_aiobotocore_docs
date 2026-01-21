# IoTEventsData module

> [Index](../README.md) > IoTEventsData


!!! note ""

    Auto-generated documentation for [IoTEventsData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#ioteventsdata)
    type annotations stubs module [types-aiobotocore-iotevents-data](https://pypi.org/project/types-aiobotocore-iotevents-data/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `IoTEventsData` service.
1. Use provided commands to install generated packages.



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

```python
# IoTEventsDataClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotevents_data.client import IoTEventsDataClient


session = get_session()
async with session.create_client("iotevents-data") as client:
    client: IoTEventsDataClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AlarmStateNameType usage example

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




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

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
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [DisableActionConfigurationTypeDef](./type_defs.md#disableactionconfigurationtypedef)
- [EnableActionConfigurationTypeDef](./type_defs.md#enableactionconfigurationtypedef)
- [ResetActionConfigurationTypeDef](./type_defs.md#resetactionconfigurationtypedef)
- [SnoozeActionConfigurationTypeDef](./type_defs.md#snoozeactionconfigurationtypedef)
- [DescribeAlarmRequestTypeDef](./type_defs.md#describealarmrequesttypedef)
- [DescribeDetectorRequestTypeDef](./type_defs.md#describedetectorrequesttypedef)
- [TimerDefinitionTypeDef](./type_defs.md#timerdefinitiontypedef)
- [VariableDefinitionTypeDef](./type_defs.md#variabledefinitiontypedef)
- [DetectorStateSummaryTypeDef](./type_defs.md#detectorstatesummarytypedef)
- [TimerTypeDef](./type_defs.md#timertypedef)
- [VariableTypeDef](./type_defs.md#variabletypedef)
- [ListAlarmsRequestTypeDef](./type_defs.md#listalarmsrequesttypedef)
- [ListDetectorsRequestTypeDef](./type_defs.md#listdetectorsrequesttypedef)
- [TimestampValueTypeDef](./type_defs.md#timestampvaluetypedef)
- [SimpleRuleEvaluationTypeDef](./type_defs.md#simpleruleevaluationtypedef)
- [StateChangeConfigurationTypeDef](./type_defs.md#statechangeconfigurationtypedef)
- [BatchAcknowledgeAlarmRequestTypeDef](./type_defs.md#batchacknowledgealarmrequesttypedef)
- [BatchAcknowledgeAlarmResponseTypeDef](./type_defs.md#batchacknowledgealarmresponsetypedef)
- [BatchDisableAlarmResponseTypeDef](./type_defs.md#batchdisablealarmresponsetypedef)
- [BatchEnableAlarmResponseTypeDef](./type_defs.md#batchenablealarmresponsetypedef)
- [BatchResetAlarmResponseTypeDef](./type_defs.md#batchresetalarmresponsetypedef)
- [BatchSnoozeAlarmResponseTypeDef](./type_defs.md#batchsnoozealarmresponsetypedef)
- [ListAlarmsResponseTypeDef](./type_defs.md#listalarmsresponsetypedef)
- [BatchDeleteDetectorResponseTypeDef](./type_defs.md#batchdeletedetectorresponsetypedef)
- [BatchDeleteDetectorRequestTypeDef](./type_defs.md#batchdeletedetectorrequesttypedef)
- [BatchDisableAlarmRequestTypeDef](./type_defs.md#batchdisablealarmrequesttypedef)
- [BatchEnableAlarmRequestTypeDef](./type_defs.md#batchenablealarmrequesttypedef)
- [BatchPutMessageResponseTypeDef](./type_defs.md#batchputmessageresponsetypedef)
- [BatchResetAlarmRequestTypeDef](./type_defs.md#batchresetalarmrequesttypedef)
- [BatchSnoozeAlarmRequestTypeDef](./type_defs.md#batchsnoozealarmrequesttypedef)
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
- [BatchPutMessageRequestTypeDef](./type_defs.md#batchputmessagerequesttypedef)
- [AlarmStateTypeDef](./type_defs.md#alarmstatetypedef)
- [BatchUpdateDetectorRequestTypeDef](./type_defs.md#batchupdatedetectorrequesttypedef)
- [DescribeDetectorResponseTypeDef](./type_defs.md#describedetectorresponsetypedef)
- [AlarmTypeDef](./type_defs.md#alarmtypedef)
- [DescribeAlarmResponseTypeDef](./type_defs.md#describealarmresponsetypedef)

