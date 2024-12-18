# IoTEvents module

> [Index](../README.md) > IoTEvents


!!! note ""

    Auto-generated documentation for [IoTEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#iotevents)
    type annotations stubs module [types-aiobotocore-iotevents](https://pypi.org/project/types-aiobotocore-iotevents/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `IoTEvents` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `IoTEvents` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[iotevents]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[iotevents]'

# standalone installation
python -m pip install types-aiobotocore-iotevents
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-iotevents
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IoTEventsClient

Type annotations and code completion for  `#!python session.create_client("iotevents")` as [IoTEventsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client)

```python
# IoTEventsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotevents.client import IoTEventsClient


session = get_session()
async with session.create_client("iotevents") as client:
    client: IoTEventsClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AlarmModelVersionStatusType usage example

from types_aiobotocore_iotevents.literals import AlarmModelVersionStatusType

def get_value() -> AlarmModelVersionStatusType:
    return "ACTIVATING"
```

- [AlarmModelVersionStatusType](./literals.md#alarmmodelversionstatustype)
- [AnalysisResultLevelType](./literals.md#analysisresultleveltype)
- [AnalysisStatusType](./literals.md#analysisstatustype)
- [ComparisonOperatorType](./literals.md#comparisonoperatortype)
- [DetectorModelVersionStatusType](./literals.md#detectormodelversionstatustype)
- [EvaluationMethodType](./literals.md#evaluationmethodtype)
- [InputStatusType](./literals.md#inputstatustype)
- [LoggingLevelType](./literals.md#loggingleveltype)
- [PayloadTypeType](./literals.md#payloadtypetype)
- [IoTEventsServiceName](./literals.md#ioteventsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AcknowledgeFlowTypeDef](./type_defs.md#acknowledgeflowtypedef)
- [ClearTimerActionTypeDef](./type_defs.md#cleartimeractiontypedef)
- [ResetTimerActionTypeDef](./type_defs.md#resettimeractiontypedef)
- [SetTimerActionTypeDef](./type_defs.md#settimeractiontypedef)
- [SetVariableActionTypeDef](./type_defs.md#setvariableactiontypedef)
- [InitializationConfigurationTypeDef](./type_defs.md#initializationconfigurationtypedef)
- [AlarmModelSummaryTypeDef](./type_defs.md#alarmmodelsummarytypedef)
- [AlarmModelVersionSummaryTypeDef](./type_defs.md#alarmmodelversionsummarytypedef)
- [SimpleRuleTypeDef](./type_defs.md#simpleruletypedef)
- [AnalysisResultLocationTypeDef](./type_defs.md#analysisresultlocationtypedef)
- [AssetPropertyTimestampTypeDef](./type_defs.md#assetpropertytimestamptypedef)
- [AssetPropertyVariantTypeDef](./type_defs.md#assetpropertyvarianttypedef)
- [AttributeTypeDef](./type_defs.md#attributetypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DetectorModelConfigurationTypeDef](./type_defs.md#detectormodelconfigurationtypedef)
- [InputConfigurationTypeDef](./type_defs.md#inputconfigurationtypedef)
- [DeleteAlarmModelRequestRequestTypeDef](./type_defs.md#deletealarmmodelrequestrequesttypedef)
- [DeleteDetectorModelRequestRequestTypeDef](./type_defs.md#deletedetectormodelrequestrequesttypedef)
- [DeleteInputRequestRequestTypeDef](./type_defs.md#deleteinputrequestrequesttypedef)
- [DescribeAlarmModelRequestRequestTypeDef](./type_defs.md#describealarmmodelrequestrequesttypedef)
- [DescribeDetectorModelAnalysisRequestRequestTypeDef](./type_defs.md#describedetectormodelanalysisrequestrequesttypedef)
- [DescribeDetectorModelRequestRequestTypeDef](./type_defs.md#describedetectormodelrequestrequesttypedef)
- [DescribeInputRequestRequestTypeDef](./type_defs.md#describeinputrequestrequesttypedef)
- [DetectorDebugOptionTypeDef](./type_defs.md#detectordebugoptiontypedef)
- [DetectorModelSummaryTypeDef](./type_defs.md#detectormodelsummarytypedef)
- [DetectorModelVersionSummaryTypeDef](./type_defs.md#detectormodelversionsummarytypedef)
- [PayloadTypeDef](./type_defs.md#payloadtypedef)
- [EmailContentTypeDef](./type_defs.md#emailcontenttypedef)
- [GetDetectorModelAnalysisResultsRequestRequestTypeDef](./type_defs.md#getdetectormodelanalysisresultsrequestrequesttypedef)
- [IotEventsInputIdentifierTypeDef](./type_defs.md#ioteventsinputidentifiertypedef)
- [InputSummaryTypeDef](./type_defs.md#inputsummarytypedef)
- [IotSiteWiseAssetModelPropertyIdentifierTypeDef](./type_defs.md#iotsitewiseassetmodelpropertyidentifiertypedef)
- [ListAlarmModelVersionsRequestRequestTypeDef](./type_defs.md#listalarmmodelversionsrequestrequesttypedef)
- [ListAlarmModelsRequestRequestTypeDef](./type_defs.md#listalarmmodelsrequestrequesttypedef)
- [ListDetectorModelVersionsRequestRequestTypeDef](./type_defs.md#listdetectormodelversionsrequestrequesttypedef)
- [ListDetectorModelsRequestRequestTypeDef](./type_defs.md#listdetectormodelsrequestrequesttypedef)
- [RoutedResourceTypeDef](./type_defs.md#routedresourcetypedef)
- [ListInputsRequestRequestTypeDef](./type_defs.md#listinputsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [SSOIdentityTypeDef](./type_defs.md#ssoidentitytypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [AlarmCapabilitiesTypeDef](./type_defs.md#alarmcapabilitiestypedef)
- [AlarmRuleTypeDef](./type_defs.md#alarmruletypedef)
- [AnalysisResultTypeDef](./type_defs.md#analysisresulttypedef)
- [AssetPropertyValueTypeDef](./type_defs.md#assetpropertyvaluetypedef)
- [InputDefinitionOutputTypeDef](./type_defs.md#inputdefinitionoutputtypedef)
- [InputDefinitionTypeDef](./type_defs.md#inputdefinitiontypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateAlarmModelResponseTypeDef](./type_defs.md#createalarmmodelresponsetypedef)
- [DescribeDetectorModelAnalysisResponseTypeDef](./type_defs.md#describedetectormodelanalysisresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListAlarmModelVersionsResponseTypeDef](./type_defs.md#listalarmmodelversionsresponsetypedef)
- [ListAlarmModelsResponseTypeDef](./type_defs.md#listalarmmodelsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartDetectorModelAnalysisResponseTypeDef](./type_defs.md#startdetectormodelanalysisresponsetypedef)
- [UpdateAlarmModelResponseTypeDef](./type_defs.md#updatealarmmodelresponsetypedef)
- [CreateDetectorModelResponseTypeDef](./type_defs.md#createdetectormodelresponsetypedef)
- [UpdateDetectorModelResponseTypeDef](./type_defs.md#updatedetectormodelresponsetypedef)
- [CreateInputResponseTypeDef](./type_defs.md#createinputresponsetypedef)
- [UpdateInputResponseTypeDef](./type_defs.md#updateinputresponsetypedef)
- [LoggingOptionsOutputTypeDef](./type_defs.md#loggingoptionsoutputtypedef)
- [LoggingOptionsTypeDef](./type_defs.md#loggingoptionstypedef)
- [ListDetectorModelsResponseTypeDef](./type_defs.md#listdetectormodelsresponsetypedef)
- [ListDetectorModelVersionsResponseTypeDef](./type_defs.md#listdetectormodelversionsresponsetypedef)
- [DynamoDBActionTypeDef](./type_defs.md#dynamodbactiontypedef)
- [DynamoDBv2ActionTypeDef](./type_defs.md#dynamodbv2actiontypedef)
- [FirehoseActionTypeDef](./type_defs.md#firehoseactiontypedef)
- [IotEventsActionTypeDef](./type_defs.md#ioteventsactiontypedef)
- [IotTopicPublishActionTypeDef](./type_defs.md#iottopicpublishactiontypedef)
- [LambdaActionTypeDef](./type_defs.md#lambdaactiontypedef)
- [SNSTopicPublishActionTypeDef](./type_defs.md#snstopicpublishactiontypedef)
- [SqsActionTypeDef](./type_defs.md#sqsactiontypedef)
- [ListInputsResponseTypeDef](./type_defs.md#listinputsresponsetypedef)
- [IotSiteWiseInputIdentifierTypeDef](./type_defs.md#iotsitewiseinputidentifiertypedef)
- [ListInputRoutingsResponseTypeDef](./type_defs.md#listinputroutingsresponsetypedef)
- [RecipientDetailTypeDef](./type_defs.md#recipientdetailtypedef)
- [GetDetectorModelAnalysisResultsResponseTypeDef](./type_defs.md#getdetectormodelanalysisresultsresponsetypedef)
- [IotSiteWiseActionTypeDef](./type_defs.md#iotsitewiseactiontypedef)
- [InputTypeDef](./type_defs.md#inputtypedef)
- [CreateInputRequestRequestTypeDef](./type_defs.md#createinputrequestrequesttypedef)
- [UpdateInputRequestRequestTypeDef](./type_defs.md#updateinputrequestrequesttypedef)
- [DescribeLoggingOptionsResponseTypeDef](./type_defs.md#describeloggingoptionsresponsetypedef)
- [PutLoggingOptionsRequestRequestTypeDef](./type_defs.md#putloggingoptionsrequestrequesttypedef)
- [NotificationTargetActionsTypeDef](./type_defs.md#notificationtargetactionstypedef)
- [InputIdentifierTypeDef](./type_defs.md#inputidentifiertypedef)
- [EmailRecipientsOutputTypeDef](./type_defs.md#emailrecipientsoutputtypedef)
- [EmailRecipientsTypeDef](./type_defs.md#emailrecipientstypedef)
- [SMSConfigurationOutputTypeDef](./type_defs.md#smsconfigurationoutputtypedef)
- [SMSConfigurationTypeDef](./type_defs.md#smsconfigurationtypedef)
- [ActionTypeDef](./type_defs.md#actiontypedef)
- [AlarmActionTypeDef](./type_defs.md#alarmactiontypedef)
- [DescribeInputResponseTypeDef](./type_defs.md#describeinputresponsetypedef)
- [ListInputRoutingsRequestRequestTypeDef](./type_defs.md#listinputroutingsrequestrequesttypedef)
- [EmailConfigurationOutputTypeDef](./type_defs.md#emailconfigurationoutputtypedef)
- [EmailRecipientsUnionTypeDef](./type_defs.md#emailrecipientsuniontypedef)
- [SMSConfigurationUnionTypeDef](./type_defs.md#smsconfigurationuniontypedef)
- [EventOutputTypeDef](./type_defs.md#eventoutputtypedef)
- [EventTypeDef](./type_defs.md#eventtypedef)
- [TransitionEventOutputTypeDef](./type_defs.md#transitioneventoutputtypedef)
- [TransitionEventTypeDef](./type_defs.md#transitioneventtypedef)
- [AlarmEventActionsOutputTypeDef](./type_defs.md#alarmeventactionsoutputtypedef)
- [AlarmEventActionsTypeDef](./type_defs.md#alarmeventactionstypedef)
- [NotificationActionOutputTypeDef](./type_defs.md#notificationactionoutputtypedef)
- [EmailConfigurationTypeDef](./type_defs.md#emailconfigurationtypedef)
- [OnEnterLifecycleOutputTypeDef](./type_defs.md#onenterlifecycleoutputtypedef)
- [OnExitLifecycleOutputTypeDef](./type_defs.md#onexitlifecycleoutputtypedef)
- [EventUnionTypeDef](./type_defs.md#eventuniontypedef)
- [OnEnterLifecycleTypeDef](./type_defs.md#onenterlifecycletypedef)
- [OnExitLifecycleTypeDef](./type_defs.md#onexitlifecycletypedef)
- [OnInputLifecycleOutputTypeDef](./type_defs.md#oninputlifecycleoutputtypedef)
- [TransitionEventUnionTypeDef](./type_defs.md#transitioneventuniontypedef)
- [AlarmNotificationOutputTypeDef](./type_defs.md#alarmnotificationoutputtypedef)
- [EmailConfigurationUnionTypeDef](./type_defs.md#emailconfigurationuniontypedef)
- [OnEnterLifecycleUnionTypeDef](./type_defs.md#onenterlifecycleuniontypedef)
- [OnExitLifecycleUnionTypeDef](./type_defs.md#onexitlifecycleuniontypedef)
- [StateOutputTypeDef](./type_defs.md#stateoutputtypedef)
- [OnInputLifecycleTypeDef](./type_defs.md#oninputlifecycletypedef)
- [DescribeAlarmModelResponseTypeDef](./type_defs.md#describealarmmodelresponsetypedef)
- [NotificationActionTypeDef](./type_defs.md#notificationactiontypedef)
- [DetectorModelDefinitionOutputTypeDef](./type_defs.md#detectormodeldefinitionoutputtypedef)
- [OnInputLifecycleUnionTypeDef](./type_defs.md#oninputlifecycleuniontypedef)
- [NotificationActionUnionTypeDef](./type_defs.md#notificationactionuniontypedef)
- [DetectorModelTypeDef](./type_defs.md#detectormodeltypedef)
- [StateTypeDef](./type_defs.md#statetypedef)
- [AlarmNotificationTypeDef](./type_defs.md#alarmnotificationtypedef)
- [DescribeDetectorModelResponseTypeDef](./type_defs.md#describedetectormodelresponsetypedef)
- [StateUnionTypeDef](./type_defs.md#stateuniontypedef)
- [CreateAlarmModelRequestRequestTypeDef](./type_defs.md#createalarmmodelrequestrequesttypedef)
- [UpdateAlarmModelRequestRequestTypeDef](./type_defs.md#updatealarmmodelrequestrequesttypedef)
- [DetectorModelDefinitionTypeDef](./type_defs.md#detectormodeldefinitiontypedef)
- [CreateDetectorModelRequestRequestTypeDef](./type_defs.md#createdetectormodelrequestrequesttypedef)
- [StartDetectorModelAnalysisRequestRequestTypeDef](./type_defs.md#startdetectormodelanalysisrequestrequesttypedef)
- [UpdateDetectorModelRequestRequestTypeDef](./type_defs.md#updatedetectormodelrequestrequesttypedef)

