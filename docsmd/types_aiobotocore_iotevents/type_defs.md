# Type definitions

> [Index](../README.md) > [IoTEvents](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IoTEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
    type annotations stubs module [types-aiobotocore-iotevents](https://pypi.org/project/types-aiobotocore-iotevents/).



## AcknowledgeFlowTypeDef

```python
# AcknowledgeFlowTypeDef definition

class AcknowledgeFlowTypeDef(TypedDict):
    enabled: bool,
```

## ClearTimerActionTypeDef

```python
# ClearTimerActionTypeDef definition

class ClearTimerActionTypeDef(TypedDict):
    timerName: str,
```

## ResetTimerActionTypeDef

```python
# ResetTimerActionTypeDef definition

class ResetTimerActionTypeDef(TypedDict):
    timerName: str,
```

## SetTimerActionTypeDef

```python
# SetTimerActionTypeDef definition

class SetTimerActionTypeDef(TypedDict):
    timerName: str,
    seconds: NotRequired[int],
    durationExpression: NotRequired[str],
```

## SetVariableActionTypeDef

```python
# SetVariableActionTypeDef definition

class SetVariableActionTypeDef(TypedDict):
    variableName: str,
    value: str,
```

## InitializationConfigurationTypeDef

```python
# InitializationConfigurationTypeDef definition

class InitializationConfigurationTypeDef(TypedDict):
    disabledOnInitialization: bool,
```

## AlarmModelSummaryTypeDef

```python
# AlarmModelSummaryTypeDef definition

class AlarmModelSummaryTypeDef(TypedDict):
    creationTime: NotRequired[datetime],
    alarmModelDescription: NotRequired[str],
    alarmModelName: NotRequired[str],
```

## AlarmModelVersionSummaryTypeDef

```python
# AlarmModelVersionSummaryTypeDef definition

class AlarmModelVersionSummaryTypeDef(TypedDict):
    alarmModelName: NotRequired[str],
    alarmModelArn: NotRequired[str],
    alarmModelVersion: NotRequired[str],
    roleArn: NotRequired[str],
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
    status: NotRequired[AlarmModelVersionStatusType],  # (1)
    statusMessage: NotRequired[str],
```

1. See [:material-code-brackets: AlarmModelVersionStatusType](./literals.md#alarmmodelversionstatustype) 
## SimpleRuleTypeDef

```python
# SimpleRuleTypeDef definition

class SimpleRuleTypeDef(TypedDict):
    inputProperty: str,
    comparisonOperator: ComparisonOperatorType,  # (1)
    threshold: str,
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## AnalysisResultLocationTypeDef

```python
# AnalysisResultLocationTypeDef definition

class AnalysisResultLocationTypeDef(TypedDict):
    path: NotRequired[str],
```

## AssetPropertyTimestampTypeDef

```python
# AssetPropertyTimestampTypeDef definition

class AssetPropertyTimestampTypeDef(TypedDict):
    timeInSeconds: str,
    offsetInNanos: NotRequired[str],
```

## AssetPropertyVariantTypeDef

```python
# AssetPropertyVariantTypeDef definition

class AssetPropertyVariantTypeDef(TypedDict):
    stringValue: NotRequired[str],
    integerValue: NotRequired[str],
    doubleValue: NotRequired[str],
    booleanValue: NotRequired[str],
```

## AttributeTypeDef

```python
# AttributeTypeDef definition

class AttributeTypeDef(TypedDict):
    jsonPath: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
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

## DetectorModelConfigurationTypeDef

```python
# DetectorModelConfigurationTypeDef definition

class DetectorModelConfigurationTypeDef(TypedDict):
    detectorModelName: NotRequired[str],
    detectorModelVersion: NotRequired[str],
    detectorModelDescription: NotRequired[str],
    detectorModelArn: NotRequired[str],
    roleArn: NotRequired[str],
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
    status: NotRequired[DetectorModelVersionStatusType],  # (1)
    key: NotRequired[str],
    evaluationMethod: NotRequired[EvaluationMethodType],  # (2)
```

1. See [:material-code-brackets: DetectorModelVersionStatusType](./literals.md#detectormodelversionstatustype) 
2. See [:material-code-brackets: EvaluationMethodType](./literals.md#evaluationmethodtype) 
## InputConfigurationTypeDef

```python
# InputConfigurationTypeDef definition

class InputConfigurationTypeDef(TypedDict):
    inputName: str,
    inputArn: str,
    creationTime: datetime,
    lastUpdateTime: datetime,
    status: InputStatusType,  # (1)
    inputDescription: NotRequired[str],
```

1. See [:material-code-brackets: InputStatusType](./literals.md#inputstatustype) 
## DeleteAlarmModelRequestRequestTypeDef

```python
# DeleteAlarmModelRequestRequestTypeDef definition

class DeleteAlarmModelRequestRequestTypeDef(TypedDict):
    alarmModelName: str,
```

## DeleteDetectorModelRequestRequestTypeDef

```python
# DeleteDetectorModelRequestRequestTypeDef definition

class DeleteDetectorModelRequestRequestTypeDef(TypedDict):
    detectorModelName: str,
```

## DeleteInputRequestRequestTypeDef

```python
# DeleteInputRequestRequestTypeDef definition

class DeleteInputRequestRequestTypeDef(TypedDict):
    inputName: str,
```

## DescribeAlarmModelRequestRequestTypeDef

```python
# DescribeAlarmModelRequestRequestTypeDef definition

class DescribeAlarmModelRequestRequestTypeDef(TypedDict):
    alarmModelName: str,
    alarmModelVersion: NotRequired[str],
```

## DescribeDetectorModelAnalysisRequestRequestTypeDef

```python
# DescribeDetectorModelAnalysisRequestRequestTypeDef definition

class DescribeDetectorModelAnalysisRequestRequestTypeDef(TypedDict):
    analysisId: str,
```

## DescribeDetectorModelRequestRequestTypeDef

```python
# DescribeDetectorModelRequestRequestTypeDef definition

class DescribeDetectorModelRequestRequestTypeDef(TypedDict):
    detectorModelName: str,
    detectorModelVersion: NotRequired[str],
```

## DescribeInputRequestRequestTypeDef

```python
# DescribeInputRequestRequestTypeDef definition

class DescribeInputRequestRequestTypeDef(TypedDict):
    inputName: str,
```

## DetectorDebugOptionTypeDef

```python
# DetectorDebugOptionTypeDef definition

class DetectorDebugOptionTypeDef(TypedDict):
    detectorModelName: str,
    keyValue: NotRequired[str],
```

## DetectorModelSummaryTypeDef

```python
# DetectorModelSummaryTypeDef definition

class DetectorModelSummaryTypeDef(TypedDict):
    detectorModelName: NotRequired[str],
    detectorModelDescription: NotRequired[str],
    creationTime: NotRequired[datetime],
```

## DetectorModelVersionSummaryTypeDef

```python
# DetectorModelVersionSummaryTypeDef definition

class DetectorModelVersionSummaryTypeDef(TypedDict):
    detectorModelName: NotRequired[str],
    detectorModelVersion: NotRequired[str],
    detectorModelArn: NotRequired[str],
    roleArn: NotRequired[str],
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
    status: NotRequired[DetectorModelVersionStatusType],  # (1)
    evaluationMethod: NotRequired[EvaluationMethodType],  # (2)
```

1. See [:material-code-brackets: DetectorModelVersionStatusType](./literals.md#detectormodelversionstatustype) 
2. See [:material-code-brackets: EvaluationMethodType](./literals.md#evaluationmethodtype) 
## PayloadTypeDef

```python
# PayloadTypeDef definition

class PayloadTypeDef(TypedDict):
    contentExpression: str,
    type: PayloadTypeType,  # (1)
```

1. See [:material-code-brackets: PayloadTypeType](./literals.md#payloadtypetype) 
## EmailContentTypeDef

```python
# EmailContentTypeDef definition

class EmailContentTypeDef(TypedDict):
    subject: NotRequired[str],
    additionalMessage: NotRequired[str],
```

## GetDetectorModelAnalysisResultsRequestRequestTypeDef

```python
# GetDetectorModelAnalysisResultsRequestRequestTypeDef definition

class GetDetectorModelAnalysisResultsRequestRequestTypeDef(TypedDict):
    analysisId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## IotEventsInputIdentifierTypeDef

```python
# IotEventsInputIdentifierTypeDef definition

class IotEventsInputIdentifierTypeDef(TypedDict):
    inputName: str,
```

## InputSummaryTypeDef

```python
# InputSummaryTypeDef definition

class InputSummaryTypeDef(TypedDict):
    inputName: NotRequired[str],
    inputDescription: NotRequired[str],
    inputArn: NotRequired[str],
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
    status: NotRequired[InputStatusType],  # (1)
```

1. See [:material-code-brackets: InputStatusType](./literals.md#inputstatustype) 
## IotSiteWiseAssetModelPropertyIdentifierTypeDef

```python
# IotSiteWiseAssetModelPropertyIdentifierTypeDef definition

class IotSiteWiseAssetModelPropertyIdentifierTypeDef(TypedDict):
    assetModelId: str,
    propertyId: str,
```

## ListAlarmModelVersionsRequestRequestTypeDef

```python
# ListAlarmModelVersionsRequestRequestTypeDef definition

class ListAlarmModelVersionsRequestRequestTypeDef(TypedDict):
    alarmModelName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListAlarmModelsRequestRequestTypeDef

```python
# ListAlarmModelsRequestRequestTypeDef definition

class ListAlarmModelsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDetectorModelVersionsRequestRequestTypeDef

```python
# ListDetectorModelVersionsRequestRequestTypeDef definition

class ListDetectorModelVersionsRequestRequestTypeDef(TypedDict):
    detectorModelName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDetectorModelsRequestRequestTypeDef

```python
# ListDetectorModelsRequestRequestTypeDef definition

class ListDetectorModelsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## RoutedResourceTypeDef

```python
# RoutedResourceTypeDef definition

class RoutedResourceTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
```

## ListInputsRequestRequestTypeDef

```python
# ListInputsRequestRequestTypeDef definition

class ListInputsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## SSOIdentityTypeDef

```python
# SSOIdentityTypeDef definition

class SSOIdentityTypeDef(TypedDict):
    identityStoreId: str,
    userId: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## AlarmCapabilitiesTypeDef

```python
# AlarmCapabilitiesTypeDef definition

class AlarmCapabilitiesTypeDef(TypedDict):
    initializationConfiguration: NotRequired[InitializationConfigurationTypeDef],  # (1)
    acknowledgeFlow: NotRequired[AcknowledgeFlowTypeDef],  # (2)
```

1. See [:material-code-braces: InitializationConfigurationTypeDef](./type_defs.md#initializationconfigurationtypedef) 
2. See [:material-code-braces: AcknowledgeFlowTypeDef](./type_defs.md#acknowledgeflowtypedef) 
## AlarmRuleTypeDef

```python
# AlarmRuleTypeDef definition

class AlarmRuleTypeDef(TypedDict):
    simpleRule: NotRequired[SimpleRuleTypeDef],  # (1)
```

1. See [:material-code-braces: SimpleRuleTypeDef](./type_defs.md#simpleruletypedef) 
## AnalysisResultTypeDef

```python
# AnalysisResultTypeDef definition

class AnalysisResultTypeDef(TypedDict):
    type: NotRequired[str],
    level: NotRequired[AnalysisResultLevelType],  # (1)
    message: NotRequired[str],
    locations: NotRequired[List[AnalysisResultLocationTypeDef]],  # (2)
```

1. See [:material-code-brackets: AnalysisResultLevelType](./literals.md#analysisresultleveltype) 
2. See [:material-code-braces: AnalysisResultLocationTypeDef](./type_defs.md#analysisresultlocationtypedef) 
## AssetPropertyValueTypeDef

```python
# AssetPropertyValueTypeDef definition

class AssetPropertyValueTypeDef(TypedDict):
    value: NotRequired[AssetPropertyVariantTypeDef],  # (1)
    timestamp: NotRequired[AssetPropertyTimestampTypeDef],  # (2)
    quality: NotRequired[str],
```

1. See [:material-code-braces: AssetPropertyVariantTypeDef](./type_defs.md#assetpropertyvarianttypedef) 
2. See [:material-code-braces: AssetPropertyTimestampTypeDef](./type_defs.md#assetpropertytimestamptypedef) 
## InputDefinitionTypeDef

```python
# InputDefinitionTypeDef definition

class InputDefinitionTypeDef(TypedDict):
    attributes: Sequence[AttributeTypeDef],  # (1)
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateAlarmModelResponseTypeDef

```python
# CreateAlarmModelResponseTypeDef definition

class CreateAlarmModelResponseTypeDef(TypedDict):
    creationTime: datetime,
    alarmModelArn: str,
    alarmModelVersion: str,
    lastUpdateTime: datetime,
    status: AlarmModelVersionStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AlarmModelVersionStatusType](./literals.md#alarmmodelversionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDetectorModelAnalysisResponseTypeDef

```python
# DescribeDetectorModelAnalysisResponseTypeDef definition

class DescribeDetectorModelAnalysisResponseTypeDef(TypedDict):
    status: AnalysisStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AnalysisStatusType](./literals.md#analysisstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAlarmModelVersionsResponseTypeDef

```python
# ListAlarmModelVersionsResponseTypeDef definition

class ListAlarmModelVersionsResponseTypeDef(TypedDict):
    alarmModelVersionSummaries: List[AlarmModelVersionSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AlarmModelVersionSummaryTypeDef](./type_defs.md#alarmmodelversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAlarmModelsResponseTypeDef

```python
# ListAlarmModelsResponseTypeDef definition

class ListAlarmModelsResponseTypeDef(TypedDict):
    alarmModelSummaries: List[AlarmModelSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AlarmModelSummaryTypeDef](./type_defs.md#alarmmodelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDetectorModelAnalysisResponseTypeDef

```python
# StartDetectorModelAnalysisResponseTypeDef definition

class StartDetectorModelAnalysisResponseTypeDef(TypedDict):
    analysisId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAlarmModelResponseTypeDef

```python
# UpdateAlarmModelResponseTypeDef definition

class UpdateAlarmModelResponseTypeDef(TypedDict):
    creationTime: datetime,
    alarmModelArn: str,
    alarmModelVersion: str,
    lastUpdateTime: datetime,
    status: AlarmModelVersionStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AlarmModelVersionStatusType](./literals.md#alarmmodelversionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDetectorModelResponseTypeDef

```python
# CreateDetectorModelResponseTypeDef definition

class CreateDetectorModelResponseTypeDef(TypedDict):
    detectorModelConfiguration: DetectorModelConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DetectorModelConfigurationTypeDef](./type_defs.md#detectormodelconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDetectorModelResponseTypeDef

```python
# UpdateDetectorModelResponseTypeDef definition

class UpdateDetectorModelResponseTypeDef(TypedDict):
    detectorModelConfiguration: DetectorModelConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DetectorModelConfigurationTypeDef](./type_defs.md#detectormodelconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInputResponseTypeDef

```python
# CreateInputResponseTypeDef definition

class CreateInputResponseTypeDef(TypedDict):
    inputConfiguration: InputConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InputConfigurationTypeDef](./type_defs.md#inputconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateInputResponseTypeDef

```python
# UpdateInputResponseTypeDef definition

class UpdateInputResponseTypeDef(TypedDict):
    inputConfiguration: InputConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InputConfigurationTypeDef](./type_defs.md#inputconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LoggingOptionsTypeDef

```python
# LoggingOptionsTypeDef definition

class LoggingOptionsTypeDef(TypedDict):
    roleArn: str,
    level: LoggingLevelType,  # (1)
    enabled: bool,
    detectorDebugOptions: NotRequired[List[DetectorDebugOptionTypeDef]],  # (2)
```

1. See [:material-code-brackets: LoggingLevelType](./literals.md#loggingleveltype) 
2. See [:material-code-braces: DetectorDebugOptionTypeDef](./type_defs.md#detectordebugoptiontypedef) 
## ListDetectorModelsResponseTypeDef

```python
# ListDetectorModelsResponseTypeDef definition

class ListDetectorModelsResponseTypeDef(TypedDict):
    detectorModelSummaries: List[DetectorModelSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DetectorModelSummaryTypeDef](./type_defs.md#detectormodelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDetectorModelVersionsResponseTypeDef

```python
# ListDetectorModelVersionsResponseTypeDef definition

class ListDetectorModelVersionsResponseTypeDef(TypedDict):
    detectorModelVersionSummaries: List[DetectorModelVersionSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DetectorModelVersionSummaryTypeDef](./type_defs.md#detectormodelversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DynamoDBActionTypeDef

```python
# DynamoDBActionTypeDef definition

class DynamoDBActionTypeDef(TypedDict):
    hashKeyField: str,
    hashKeyValue: str,
    tableName: str,
    hashKeyType: NotRequired[str],
    rangeKeyType: NotRequired[str],
    rangeKeyField: NotRequired[str],
    rangeKeyValue: NotRequired[str],
    operation: NotRequired[str],
    payloadField: NotRequired[str],
    payload: NotRequired[PayloadTypeDef],  # (1)
```

1. See [:material-code-braces: PayloadTypeDef](./type_defs.md#payloadtypedef) 
## DynamoDBv2ActionTypeDef

```python
# DynamoDBv2ActionTypeDef definition

class DynamoDBv2ActionTypeDef(TypedDict):
    tableName: str,
    payload: NotRequired[PayloadTypeDef],  # (1)
```

1. See [:material-code-braces: PayloadTypeDef](./type_defs.md#payloadtypedef) 
## FirehoseActionTypeDef

```python
# FirehoseActionTypeDef definition

class FirehoseActionTypeDef(TypedDict):
    deliveryStreamName: str,
    separator: NotRequired[str],
    payload: NotRequired[PayloadTypeDef],  # (1)
```

1. See [:material-code-braces: PayloadTypeDef](./type_defs.md#payloadtypedef) 
## IotEventsActionTypeDef

```python
# IotEventsActionTypeDef definition

class IotEventsActionTypeDef(TypedDict):
    inputName: str,
    payload: NotRequired[PayloadTypeDef],  # (1)
```

1. See [:material-code-braces: PayloadTypeDef](./type_defs.md#payloadtypedef) 
## IotTopicPublishActionTypeDef

```python
# IotTopicPublishActionTypeDef definition

class IotTopicPublishActionTypeDef(TypedDict):
    mqttTopic: str,
    payload: NotRequired[PayloadTypeDef],  # (1)
```

1. See [:material-code-braces: PayloadTypeDef](./type_defs.md#payloadtypedef) 
## LambdaActionTypeDef

```python
# LambdaActionTypeDef definition

class LambdaActionTypeDef(TypedDict):
    functionArn: str,
    payload: NotRequired[PayloadTypeDef],  # (1)
```

1. See [:material-code-braces: PayloadTypeDef](./type_defs.md#payloadtypedef) 
## SNSTopicPublishActionTypeDef

```python
# SNSTopicPublishActionTypeDef definition

class SNSTopicPublishActionTypeDef(TypedDict):
    targetArn: str,
    payload: NotRequired[PayloadTypeDef],  # (1)
```

1. See [:material-code-braces: PayloadTypeDef](./type_defs.md#payloadtypedef) 
## SqsActionTypeDef

```python
# SqsActionTypeDef definition

class SqsActionTypeDef(TypedDict):
    queueUrl: str,
    useBase64: NotRequired[bool],
    payload: NotRequired[PayloadTypeDef],  # (1)
```

1. See [:material-code-braces: PayloadTypeDef](./type_defs.md#payloadtypedef) 
## ListInputsResponseTypeDef

```python
# ListInputsResponseTypeDef definition

class ListInputsResponseTypeDef(TypedDict):
    inputSummaries: List[InputSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InputSummaryTypeDef](./type_defs.md#inputsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IotSiteWiseInputIdentifierTypeDef

```python
# IotSiteWiseInputIdentifierTypeDef definition

class IotSiteWiseInputIdentifierTypeDef(TypedDict):
    iotSiteWiseAssetModelPropertyIdentifier: NotRequired[IotSiteWiseAssetModelPropertyIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: IotSiteWiseAssetModelPropertyIdentifierTypeDef](./type_defs.md#iotsitewiseassetmodelpropertyidentifiertypedef) 
## ListInputRoutingsResponseTypeDef

```python
# ListInputRoutingsResponseTypeDef definition

class ListInputRoutingsResponseTypeDef(TypedDict):
    routedResources: List[RoutedResourceTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoutedResourceTypeDef](./type_defs.md#routedresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RecipientDetailTypeDef

```python
# RecipientDetailTypeDef definition

class RecipientDetailTypeDef(TypedDict):
    ssoIdentity: NotRequired[SSOIdentityTypeDef],  # (1)
```

1. See [:material-code-braces: SSOIdentityTypeDef](./type_defs.md#ssoidentitytypedef) 
## GetDetectorModelAnalysisResultsResponseTypeDef

```python
# GetDetectorModelAnalysisResultsResponseTypeDef definition

class GetDetectorModelAnalysisResultsResponseTypeDef(TypedDict):
    analysisResults: List[AnalysisResultTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalysisResultTypeDef](./type_defs.md#analysisresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IotSiteWiseActionTypeDef

```python
# IotSiteWiseActionTypeDef definition

class IotSiteWiseActionTypeDef(TypedDict):
    entryId: NotRequired[str],
    assetId: NotRequired[str],
    propertyId: NotRequired[str],
    propertyAlias: NotRequired[str],
    propertyValue: NotRequired[AssetPropertyValueTypeDef],  # (1)
```

1. See [:material-code-braces: AssetPropertyValueTypeDef](./type_defs.md#assetpropertyvaluetypedef) 
## CreateInputRequestRequestTypeDef

```python
# CreateInputRequestRequestTypeDef definition

class CreateInputRequestRequestTypeDef(TypedDict):
    inputName: str,
    inputDefinition: InputDefinitionTypeDef,  # (1)
    inputDescription: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: InputDefinitionTypeDef](./type_defs.md#inputdefinitiontypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## InputTypeDef

```python
# InputTypeDef definition

class InputTypeDef(TypedDict):
    inputConfiguration: NotRequired[InputConfigurationTypeDef],  # (1)
    inputDefinition: NotRequired[InputDefinitionTypeDef],  # (2)
```

1. See [:material-code-braces: InputConfigurationTypeDef](./type_defs.md#inputconfigurationtypedef) 
2. See [:material-code-braces: InputDefinitionTypeDef](./type_defs.md#inputdefinitiontypedef) 
## UpdateInputRequestRequestTypeDef

```python
# UpdateInputRequestRequestTypeDef definition

class UpdateInputRequestRequestTypeDef(TypedDict):
    inputName: str,
    inputDefinition: InputDefinitionTypeDef,  # (1)
    inputDescription: NotRequired[str],
```

1. See [:material-code-braces: InputDefinitionTypeDef](./type_defs.md#inputdefinitiontypedef) 
## DescribeLoggingOptionsResponseTypeDef

```python
# DescribeLoggingOptionsResponseTypeDef definition

class DescribeLoggingOptionsResponseTypeDef(TypedDict):
    loggingOptions: LoggingOptionsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingOptionsTypeDef](./type_defs.md#loggingoptionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutLoggingOptionsRequestRequestTypeDef

```python
# PutLoggingOptionsRequestRequestTypeDef definition

class PutLoggingOptionsRequestRequestTypeDef(TypedDict):
    loggingOptions: LoggingOptionsTypeDef,  # (1)
```

1. See [:material-code-braces: LoggingOptionsTypeDef](./type_defs.md#loggingoptionstypedef) 
## NotificationTargetActionsTypeDef

```python
# NotificationTargetActionsTypeDef definition

class NotificationTargetActionsTypeDef(TypedDict):
    lambdaAction: NotRequired[LambdaActionTypeDef],  # (1)
```

1. See [:material-code-braces: LambdaActionTypeDef](./type_defs.md#lambdaactiontypedef) 
## InputIdentifierTypeDef

```python
# InputIdentifierTypeDef definition

class InputIdentifierTypeDef(TypedDict):
    iotEventsInputIdentifier: NotRequired[IotEventsInputIdentifierTypeDef],  # (1)
    iotSiteWiseInputIdentifier: NotRequired[IotSiteWiseInputIdentifierTypeDef],  # (2)
```

1. See [:material-code-braces: IotEventsInputIdentifierTypeDef](./type_defs.md#ioteventsinputidentifiertypedef) 
2. See [:material-code-braces: IotSiteWiseInputIdentifierTypeDef](./type_defs.md#iotsitewiseinputidentifiertypedef) 
## EmailRecipientsTypeDef

```python
# EmailRecipientsTypeDef definition

class EmailRecipientsTypeDef(TypedDict):
    to: NotRequired[Sequence[RecipientDetailTypeDef]],  # (1)
```

1. See [:material-code-braces: RecipientDetailTypeDef](./type_defs.md#recipientdetailtypedef) 
## SMSConfigurationTypeDef

```python
# SMSConfigurationTypeDef definition

class SMSConfigurationTypeDef(TypedDict):
    recipients: Sequence[RecipientDetailTypeDef],  # (1)
    senderId: NotRequired[str],
    additionalMessage: NotRequired[str],
```

1. See [:material-code-braces: RecipientDetailTypeDef](./type_defs.md#recipientdetailtypedef) 
## ActionTypeDef

```python
# ActionTypeDef definition

class ActionTypeDef(TypedDict):
    setVariable: NotRequired[SetVariableActionTypeDef],  # (1)
    sns: NotRequired[SNSTopicPublishActionTypeDef],  # (2)
    iotTopicPublish: NotRequired[IotTopicPublishActionTypeDef],  # (3)
    setTimer: NotRequired[SetTimerActionTypeDef],  # (4)
    clearTimer: NotRequired[ClearTimerActionTypeDef],  # (5)
    resetTimer: NotRequired[ResetTimerActionTypeDef],  # (6)
    lambda: NotRequired[LambdaActionTypeDef],  # (7)
    iotEvents: NotRequired[IotEventsActionTypeDef],  # (8)
    sqs: NotRequired[SqsActionTypeDef],  # (9)
    firehose: NotRequired[FirehoseActionTypeDef],  # (10)
    dynamoDB: NotRequired[DynamoDBActionTypeDef],  # (11)
    dynamoDBv2: NotRequired[DynamoDBv2ActionTypeDef],  # (12)
    iotSiteWise: NotRequired[IotSiteWiseActionTypeDef],  # (13)
```

1. See [:material-code-braces: SetVariableActionTypeDef](./type_defs.md#setvariableactiontypedef) 
2. See [:material-code-braces: SNSTopicPublishActionTypeDef](./type_defs.md#snstopicpublishactiontypedef) 
3. See [:material-code-braces: IotTopicPublishActionTypeDef](./type_defs.md#iottopicpublishactiontypedef) 
4. See [:material-code-braces: SetTimerActionTypeDef](./type_defs.md#settimeractiontypedef) 
5. See [:material-code-braces: ClearTimerActionTypeDef](./type_defs.md#cleartimeractiontypedef) 
6. See [:material-code-braces: ResetTimerActionTypeDef](./type_defs.md#resettimeractiontypedef) 
7. See [:material-code-braces: LambdaActionTypeDef](./type_defs.md#lambdaactiontypedef) 
8. See [:material-code-braces: IotEventsActionTypeDef](./type_defs.md#ioteventsactiontypedef) 
9. See [:material-code-braces: SqsActionTypeDef](./type_defs.md#sqsactiontypedef) 
10. See [:material-code-braces: FirehoseActionTypeDef](./type_defs.md#firehoseactiontypedef) 
11. See [:material-code-braces: DynamoDBActionTypeDef](./type_defs.md#dynamodbactiontypedef) 
12. See [:material-code-braces: DynamoDBv2ActionTypeDef](./type_defs.md#dynamodbv2actiontypedef) 
13. See [:material-code-braces: IotSiteWiseActionTypeDef](./type_defs.md#iotsitewiseactiontypedef) 
## AlarmActionTypeDef

```python
# AlarmActionTypeDef definition

class AlarmActionTypeDef(TypedDict):
    sns: NotRequired[SNSTopicPublishActionTypeDef],  # (1)
    iotTopicPublish: NotRequired[IotTopicPublishActionTypeDef],  # (2)
    lambda: NotRequired[LambdaActionTypeDef],  # (3)
    iotEvents: NotRequired[IotEventsActionTypeDef],  # (4)
    sqs: NotRequired[SqsActionTypeDef],  # (5)
    firehose: NotRequired[FirehoseActionTypeDef],  # (6)
    dynamoDB: NotRequired[DynamoDBActionTypeDef],  # (7)
    dynamoDBv2: NotRequired[DynamoDBv2ActionTypeDef],  # (8)
    iotSiteWise: NotRequired[IotSiteWiseActionTypeDef],  # (9)
```

1. See [:material-code-braces: SNSTopicPublishActionTypeDef](./type_defs.md#snstopicpublishactiontypedef) 
2. See [:material-code-braces: IotTopicPublishActionTypeDef](./type_defs.md#iottopicpublishactiontypedef) 
3. See [:material-code-braces: LambdaActionTypeDef](./type_defs.md#lambdaactiontypedef) 
4. See [:material-code-braces: IotEventsActionTypeDef](./type_defs.md#ioteventsactiontypedef) 
5. See [:material-code-braces: SqsActionTypeDef](./type_defs.md#sqsactiontypedef) 
6. See [:material-code-braces: FirehoseActionTypeDef](./type_defs.md#firehoseactiontypedef) 
7. See [:material-code-braces: DynamoDBActionTypeDef](./type_defs.md#dynamodbactiontypedef) 
8. See [:material-code-braces: DynamoDBv2ActionTypeDef](./type_defs.md#dynamodbv2actiontypedef) 
9. See [:material-code-braces: IotSiteWiseActionTypeDef](./type_defs.md#iotsitewiseactiontypedef) 
## DescribeInputResponseTypeDef

```python
# DescribeInputResponseTypeDef definition

class DescribeInputResponseTypeDef(TypedDict):
    input: InputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InputTypeDef](./type_defs.md#inputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInputRoutingsRequestRequestTypeDef

```python
# ListInputRoutingsRequestRequestTypeDef definition

class ListInputRoutingsRequestRequestTypeDef(TypedDict):
    inputIdentifier: InputIdentifierTypeDef,  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: InputIdentifierTypeDef](./type_defs.md#inputidentifiertypedef) 
## EmailConfigurationTypeDef

```python
# EmailConfigurationTypeDef definition

class EmailConfigurationTypeDef(TypedDict):
    from: str,
    recipients: EmailRecipientsTypeDef,  # (2)
    content: NotRequired[EmailContentTypeDef],  # (1)
```

1. See [:material-code-braces: EmailContentTypeDef](./type_defs.md#emailcontenttypedef) 
2. See [:material-code-braces: EmailRecipientsTypeDef](./type_defs.md#emailrecipientstypedef) 
## EventTypeDef

```python
# EventTypeDef definition

class EventTypeDef(TypedDict):
    eventName: str,
    condition: NotRequired[str],
    actions: NotRequired[Sequence[ActionTypeDef]],  # (1)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
## TransitionEventTypeDef

```python
# TransitionEventTypeDef definition

class TransitionEventTypeDef(TypedDict):
    eventName: str,
    condition: str,
    nextState: str,
    actions: NotRequired[Sequence[ActionTypeDef]],  # (1)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
## AlarmEventActionsTypeDef

```python
# AlarmEventActionsTypeDef definition

class AlarmEventActionsTypeDef(TypedDict):
    alarmActions: NotRequired[Sequence[AlarmActionTypeDef]],  # (1)
```

1. See [:material-code-braces: AlarmActionTypeDef](./type_defs.md#alarmactiontypedef) 
## NotificationActionTypeDef

```python
# NotificationActionTypeDef definition

class NotificationActionTypeDef(TypedDict):
    action: NotificationTargetActionsTypeDef,  # (1)
    smsConfigurations: NotRequired[Sequence[SMSConfigurationTypeDef]],  # (2)
    emailConfigurations: NotRequired[Sequence[EmailConfigurationTypeDef]],  # (3)
```

1. See [:material-code-braces: NotificationTargetActionsTypeDef](./type_defs.md#notificationtargetactionstypedef) 
2. See [:material-code-braces: SMSConfigurationTypeDef](./type_defs.md#smsconfigurationtypedef) 
3. See [:material-code-braces: EmailConfigurationTypeDef](./type_defs.md#emailconfigurationtypedef) 
## OnEnterLifecycleTypeDef

```python
# OnEnterLifecycleTypeDef definition

class OnEnterLifecycleTypeDef(TypedDict):
    events: NotRequired[Sequence[EventTypeDef]],  # (1)
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
## OnExitLifecycleTypeDef

```python
# OnExitLifecycleTypeDef definition

class OnExitLifecycleTypeDef(TypedDict):
    events: NotRequired[Sequence[EventTypeDef]],  # (1)
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
## OnInputLifecycleTypeDef

```python
# OnInputLifecycleTypeDef definition

class OnInputLifecycleTypeDef(TypedDict):
    events: NotRequired[Sequence[EventTypeDef]],  # (1)
    transitionEvents: NotRequired[Sequence[TransitionEventTypeDef]],  # (2)
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
2. See [:material-code-braces: TransitionEventTypeDef](./type_defs.md#transitioneventtypedef) 
## AlarmNotificationTypeDef

```python
# AlarmNotificationTypeDef definition

class AlarmNotificationTypeDef(TypedDict):
    notificationActions: NotRequired[Sequence[NotificationActionTypeDef]],  # (1)
```

1. See [:material-code-braces: NotificationActionTypeDef](./type_defs.md#notificationactiontypedef) 
## StateTypeDef

```python
# StateTypeDef definition

class StateTypeDef(TypedDict):
    stateName: str,
    onInput: NotRequired[OnInputLifecycleTypeDef],  # (1)
    onEnter: NotRequired[OnEnterLifecycleTypeDef],  # (2)
    onExit: NotRequired[OnExitLifecycleTypeDef],  # (3)
```

1. See [:material-code-braces: OnInputLifecycleTypeDef](./type_defs.md#oninputlifecycletypedef) 
2. See [:material-code-braces: OnEnterLifecycleTypeDef](./type_defs.md#onenterlifecycletypedef) 
3. See [:material-code-braces: OnExitLifecycleTypeDef](./type_defs.md#onexitlifecycletypedef) 
## CreateAlarmModelRequestRequestTypeDef

```python
# CreateAlarmModelRequestRequestTypeDef definition

class CreateAlarmModelRequestRequestTypeDef(TypedDict):
    alarmModelName: str,
    roleArn: str,
    alarmRule: AlarmRuleTypeDef,  # (1)
    alarmModelDescription: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    key: NotRequired[str],
    severity: NotRequired[int],
    alarmNotification: NotRequired[AlarmNotificationTypeDef],  # (3)
    alarmEventActions: NotRequired[AlarmEventActionsTypeDef],  # (4)
    alarmCapabilities: NotRequired[AlarmCapabilitiesTypeDef],  # (5)
```

1. See [:material-code-braces: AlarmRuleTypeDef](./type_defs.md#alarmruletypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: AlarmNotificationTypeDef](./type_defs.md#alarmnotificationtypedef) 
4. See [:material-code-braces: AlarmEventActionsTypeDef](./type_defs.md#alarmeventactionstypedef) 
5. See [:material-code-braces: AlarmCapabilitiesTypeDef](./type_defs.md#alarmcapabilitiestypedef) 
## DescribeAlarmModelResponseTypeDef

```python
# DescribeAlarmModelResponseTypeDef definition

class DescribeAlarmModelResponseTypeDef(TypedDict):
    creationTime: datetime,
    alarmModelArn: str,
    alarmModelVersion: str,
    lastUpdateTime: datetime,
    status: AlarmModelVersionStatusType,  # (1)
    statusMessage: str,
    alarmModelName: str,
    alarmModelDescription: str,
    roleArn: str,
    key: str,
    severity: int,
    alarmRule: AlarmRuleTypeDef,  # (2)
    alarmNotification: AlarmNotificationTypeDef,  # (3)
    alarmEventActions: AlarmEventActionsTypeDef,  # (4)
    alarmCapabilities: AlarmCapabilitiesTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: AlarmModelVersionStatusType](./literals.md#alarmmodelversionstatustype) 
2. See [:material-code-braces: AlarmRuleTypeDef](./type_defs.md#alarmruletypedef) 
3. See [:material-code-braces: AlarmNotificationTypeDef](./type_defs.md#alarmnotificationtypedef) 
4. See [:material-code-braces: AlarmEventActionsTypeDef](./type_defs.md#alarmeventactionstypedef) 
5. See [:material-code-braces: AlarmCapabilitiesTypeDef](./type_defs.md#alarmcapabilitiestypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAlarmModelRequestRequestTypeDef

```python
# UpdateAlarmModelRequestRequestTypeDef definition

class UpdateAlarmModelRequestRequestTypeDef(TypedDict):
    alarmModelName: str,
    roleArn: str,
    alarmRule: AlarmRuleTypeDef,  # (1)
    alarmModelDescription: NotRequired[str],
    severity: NotRequired[int],
    alarmNotification: NotRequired[AlarmNotificationTypeDef],  # (2)
    alarmEventActions: NotRequired[AlarmEventActionsTypeDef],  # (3)
    alarmCapabilities: NotRequired[AlarmCapabilitiesTypeDef],  # (4)
```

1. See [:material-code-braces: AlarmRuleTypeDef](./type_defs.md#alarmruletypedef) 
2. See [:material-code-braces: AlarmNotificationTypeDef](./type_defs.md#alarmnotificationtypedef) 
3. See [:material-code-braces: AlarmEventActionsTypeDef](./type_defs.md#alarmeventactionstypedef) 
4. See [:material-code-braces: AlarmCapabilitiesTypeDef](./type_defs.md#alarmcapabilitiestypedef) 
## DetectorModelDefinitionTypeDef

```python
# DetectorModelDefinitionTypeDef definition

class DetectorModelDefinitionTypeDef(TypedDict):
    states: Sequence[StateTypeDef],  # (1)
    initialStateName: str,
```

1. See [:material-code-braces: StateTypeDef](./type_defs.md#statetypedef) 
## CreateDetectorModelRequestRequestTypeDef

```python
# CreateDetectorModelRequestRequestTypeDef definition

class CreateDetectorModelRequestRequestTypeDef(TypedDict):
    detectorModelName: str,
    detectorModelDefinition: DetectorModelDefinitionTypeDef,  # (1)
    roleArn: str,
    detectorModelDescription: NotRequired[str],
    key: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    evaluationMethod: NotRequired[EvaluationMethodType],  # (3)
```

1. See [:material-code-braces: DetectorModelDefinitionTypeDef](./type_defs.md#detectormodeldefinitiontypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: EvaluationMethodType](./literals.md#evaluationmethodtype) 
## DetectorModelTypeDef

```python
# DetectorModelTypeDef definition

class DetectorModelTypeDef(TypedDict):
    detectorModelDefinition: NotRequired[DetectorModelDefinitionTypeDef],  # (1)
    detectorModelConfiguration: NotRequired[DetectorModelConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: DetectorModelDefinitionTypeDef](./type_defs.md#detectormodeldefinitiontypedef) 
2. See [:material-code-braces: DetectorModelConfigurationTypeDef](./type_defs.md#detectormodelconfigurationtypedef) 
## StartDetectorModelAnalysisRequestRequestTypeDef

```python
# StartDetectorModelAnalysisRequestRequestTypeDef definition

class StartDetectorModelAnalysisRequestRequestTypeDef(TypedDict):
    detectorModelDefinition: DetectorModelDefinitionTypeDef,  # (1)
```

1. See [:material-code-braces: DetectorModelDefinitionTypeDef](./type_defs.md#detectormodeldefinitiontypedef) 
## UpdateDetectorModelRequestRequestTypeDef

```python
# UpdateDetectorModelRequestRequestTypeDef definition

class UpdateDetectorModelRequestRequestTypeDef(TypedDict):
    detectorModelName: str,
    detectorModelDefinition: DetectorModelDefinitionTypeDef,  # (1)
    roleArn: str,
    detectorModelDescription: NotRequired[str],
    evaluationMethod: NotRequired[EvaluationMethodType],  # (2)
```

1. See [:material-code-braces: DetectorModelDefinitionTypeDef](./type_defs.md#detectormodeldefinitiontypedef) 
2. See [:material-code-brackets: EvaluationMethodType](./literals.md#evaluationmethodtype) 
## DescribeDetectorModelResponseTypeDef

```python
# DescribeDetectorModelResponseTypeDef definition

class DescribeDetectorModelResponseTypeDef(TypedDict):
    detectorModel: DetectorModelTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DetectorModelTypeDef](./type_defs.md#detectormodeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
