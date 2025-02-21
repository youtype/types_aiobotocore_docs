# Type definitions

> [Index](../README.md) > [IoTEvents](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IoTEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#iotevents)
    type annotations stubs module [types-aiobotocore-iotevents](https://pypi.org/project/types-aiobotocore-iotevents/).

## InputDefinitionUnionTypeDef

```python
# InputDefinitionUnionTypeDef Union usage example

from types_aiobotocore_iotevents.type_defs import InputDefinitionUnionTypeDef


def get_value() -> InputDefinitionUnionTypeDef:
    return ...


# InputDefinitionUnionTypeDef definition

InputDefinitionUnionTypeDef = Union[
    InputDefinitionTypeDef,  # (1)
    InputDefinitionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: InputDefinitionTypeDef](./type_defs.md#inputdefinitiontypedef) 
2. See [:material-code-braces: InputDefinitionOutputTypeDef](./type_defs.md#inputdefinitionoutputtypedef) 

## LoggingOptionsUnionTypeDef

```python
# LoggingOptionsUnionTypeDef Union usage example

from types_aiobotocore_iotevents.type_defs import LoggingOptionsUnionTypeDef


def get_value() -> LoggingOptionsUnionTypeDef:
    return ...


# LoggingOptionsUnionTypeDef definition

LoggingOptionsUnionTypeDef = Union[
    LoggingOptionsTypeDef,  # (1)
    LoggingOptionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: LoggingOptionsTypeDef](./type_defs.md#loggingoptionstypedef) 
2. See [:material-code-braces: LoggingOptionsOutputTypeDef](./type_defs.md#loggingoptionsoutputtypedef) 

## AlarmEventActionsUnionTypeDef

```python
# AlarmEventActionsUnionTypeDef Union usage example

from types_aiobotocore_iotevents.type_defs import AlarmEventActionsUnionTypeDef


def get_value() -> AlarmEventActionsUnionTypeDef:
    return ...


# AlarmEventActionsUnionTypeDef definition

AlarmEventActionsUnionTypeDef = Union[
    AlarmEventActionsTypeDef,  # (1)
    AlarmEventActionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AlarmEventActionsTypeDef](./type_defs.md#alarmeventactionstypedef) 
2. See [:material-code-braces: AlarmEventActionsOutputTypeDef](./type_defs.md#alarmeventactionsoutputtypedef) 

## AlarmNotificationUnionTypeDef

```python
# AlarmNotificationUnionTypeDef Union usage example

from types_aiobotocore_iotevents.type_defs import AlarmNotificationUnionTypeDef


def get_value() -> AlarmNotificationUnionTypeDef:
    return ...


# AlarmNotificationUnionTypeDef definition

AlarmNotificationUnionTypeDef = Union[
    AlarmNotificationTypeDef,  # (1)
    AlarmNotificationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AlarmNotificationTypeDef](./type_defs.md#alarmnotificationtypedef) 
2. See [:material-code-braces: AlarmNotificationOutputTypeDef](./type_defs.md#alarmnotificationoutputtypedef) 

## DetectorModelDefinitionUnionTypeDef

```python
# DetectorModelDefinitionUnionTypeDef Union usage example

from types_aiobotocore_iotevents.type_defs import DetectorModelDefinitionUnionTypeDef


def get_value() -> DetectorModelDefinitionUnionTypeDef:
    return ...


# DetectorModelDefinitionUnionTypeDef definition

DetectorModelDefinitionUnionTypeDef = Union[
    DetectorModelDefinitionTypeDef,  # (1)
    DetectorModelDefinitionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DetectorModelDefinitionTypeDef](./type_defs.md#detectormodeldefinitiontypedef) 
2. See [:material-code-braces: DetectorModelDefinitionOutputTypeDef](./type_defs.md#detectormodeldefinitionoutputtypedef) 



## AcknowledgeFlowTypeDef

```python
# AcknowledgeFlowTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import AcknowledgeFlowTypeDef


def get_value() -> AcknowledgeFlowTypeDef:
    return {
        "enabled": ...,
    }


# AcknowledgeFlowTypeDef definition

class AcknowledgeFlowTypeDef(TypedDict):
    enabled: bool,
```

## ClearTimerActionTypeDef

```python
# ClearTimerActionTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import ClearTimerActionTypeDef


def get_value() -> ClearTimerActionTypeDef:
    return {
        "timerName": ...,
    }


# ClearTimerActionTypeDef definition

class ClearTimerActionTypeDef(TypedDict):
    timerName: str,
```

## ResetTimerActionTypeDef

```python
# ResetTimerActionTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import ResetTimerActionTypeDef


def get_value() -> ResetTimerActionTypeDef:
    return {
        "timerName": ...,
    }


# ResetTimerActionTypeDef definition

class ResetTimerActionTypeDef(TypedDict):
    timerName: str,
```

## SetTimerActionTypeDef

```python
# SetTimerActionTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import SetTimerActionTypeDef


def get_value() -> SetTimerActionTypeDef:
    return {
        "timerName": ...,
    }


# SetTimerActionTypeDef definition

class SetTimerActionTypeDef(TypedDict):
    timerName: str,
    seconds: NotRequired[int],
    durationExpression: NotRequired[str],
```

## SetVariableActionTypeDef

```python
# SetVariableActionTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import SetVariableActionTypeDef


def get_value() -> SetVariableActionTypeDef:
    return {
        "variableName": ...,
    }


# SetVariableActionTypeDef definition

class SetVariableActionTypeDef(TypedDict):
    variableName: str,
    value: str,
```

## InitializationConfigurationTypeDef

```python
# InitializationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import InitializationConfigurationTypeDef


def get_value() -> InitializationConfigurationTypeDef:
    return {
        "disabledOnInitialization": ...,
    }


# InitializationConfigurationTypeDef definition

class InitializationConfigurationTypeDef(TypedDict):
    disabledOnInitialization: bool,
```

## AlarmModelSummaryTypeDef

```python
# AlarmModelSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import AlarmModelSummaryTypeDef


def get_value() -> AlarmModelSummaryTypeDef:
    return {
        "creationTime": ...,
    }


# AlarmModelSummaryTypeDef definition

class AlarmModelSummaryTypeDef(TypedDict):
    creationTime: NotRequired[datetime],
    alarmModelDescription: NotRequired[str],
    alarmModelName: NotRequired[str],
```

## AlarmModelVersionSummaryTypeDef

```python
# AlarmModelVersionSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import AlarmModelVersionSummaryTypeDef


def get_value() -> AlarmModelVersionSummaryTypeDef:
    return {
        "alarmModelName": ...,
    }


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
# SimpleRuleTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import SimpleRuleTypeDef


def get_value() -> SimpleRuleTypeDef:
    return {
        "inputProperty": ...,
    }


# SimpleRuleTypeDef definition

class SimpleRuleTypeDef(TypedDict):
    inputProperty: str,
    comparisonOperator: ComparisonOperatorType,  # (1)
    threshold: str,
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## AnalysisResultLocationTypeDef

```python
# AnalysisResultLocationTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import AnalysisResultLocationTypeDef


def get_value() -> AnalysisResultLocationTypeDef:
    return {
        "path": ...,
    }


# AnalysisResultLocationTypeDef definition

class AnalysisResultLocationTypeDef(TypedDict):
    path: NotRequired[str],
```

## AssetPropertyTimestampTypeDef

```python
# AssetPropertyTimestampTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import AssetPropertyTimestampTypeDef


def get_value() -> AssetPropertyTimestampTypeDef:
    return {
        "timeInSeconds": ...,
    }


# AssetPropertyTimestampTypeDef definition

class AssetPropertyTimestampTypeDef(TypedDict):
    timeInSeconds: str,
    offsetInNanos: NotRequired[str],
```

## AssetPropertyVariantTypeDef

```python
# AssetPropertyVariantTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import AssetPropertyVariantTypeDef


def get_value() -> AssetPropertyVariantTypeDef:
    return {
        "stringValue": ...,
    }


# AssetPropertyVariantTypeDef definition

class AssetPropertyVariantTypeDef(TypedDict):
    stringValue: NotRequired[str],
    integerValue: NotRequired[str],
    doubleValue: NotRequired[str],
    booleanValue: NotRequired[str],
```

## AttributeTypeDef

```python
# AttributeTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import AttributeTypeDef


def get_value() -> AttributeTypeDef:
    return {
        "jsonPath": ...,
    }


# AttributeTypeDef definition

class AttributeTypeDef(TypedDict):
    jsonPath: str,
```

## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import ResponseMetadataTypeDef


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

## DetectorModelConfigurationTypeDef

```python
# DetectorModelConfigurationTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import DetectorModelConfigurationTypeDef


def get_value() -> DetectorModelConfigurationTypeDef:
    return {
        "detectorModelName": ...,
    }


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
# InputConfigurationTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import InputConfigurationTypeDef


def get_value() -> InputConfigurationTypeDef:
    return {
        "inputName": ...,
    }


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
## DeleteAlarmModelRequestTypeDef

```python
# DeleteAlarmModelRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import DeleteAlarmModelRequestTypeDef


def get_value() -> DeleteAlarmModelRequestTypeDef:
    return {
        "alarmModelName": ...,
    }


# DeleteAlarmModelRequestTypeDef definition

class DeleteAlarmModelRequestTypeDef(TypedDict):
    alarmModelName: str,
```

## DeleteDetectorModelRequestTypeDef

```python
# DeleteDetectorModelRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import DeleteDetectorModelRequestTypeDef


def get_value() -> DeleteDetectorModelRequestTypeDef:
    return {
        "detectorModelName": ...,
    }


# DeleteDetectorModelRequestTypeDef definition

class DeleteDetectorModelRequestTypeDef(TypedDict):
    detectorModelName: str,
```

## DeleteInputRequestTypeDef

```python
# DeleteInputRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import DeleteInputRequestTypeDef


def get_value() -> DeleteInputRequestTypeDef:
    return {
        "inputName": ...,
    }


# DeleteInputRequestTypeDef definition

class DeleteInputRequestTypeDef(TypedDict):
    inputName: str,
```

## DescribeAlarmModelRequestTypeDef

```python
# DescribeAlarmModelRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import DescribeAlarmModelRequestTypeDef


def get_value() -> DescribeAlarmModelRequestTypeDef:
    return {
        "alarmModelName": ...,
    }


# DescribeAlarmModelRequestTypeDef definition

class DescribeAlarmModelRequestTypeDef(TypedDict):
    alarmModelName: str,
    alarmModelVersion: NotRequired[str],
```

## DescribeDetectorModelAnalysisRequestTypeDef

```python
# DescribeDetectorModelAnalysisRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import DescribeDetectorModelAnalysisRequestTypeDef


def get_value() -> DescribeDetectorModelAnalysisRequestTypeDef:
    return {
        "analysisId": ...,
    }


# DescribeDetectorModelAnalysisRequestTypeDef definition

class DescribeDetectorModelAnalysisRequestTypeDef(TypedDict):
    analysisId: str,
```

## DescribeDetectorModelRequestTypeDef

```python
# DescribeDetectorModelRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import DescribeDetectorModelRequestTypeDef


def get_value() -> DescribeDetectorModelRequestTypeDef:
    return {
        "detectorModelName": ...,
    }


# DescribeDetectorModelRequestTypeDef definition

class DescribeDetectorModelRequestTypeDef(TypedDict):
    detectorModelName: str,
    detectorModelVersion: NotRequired[str],
```

## DescribeInputRequestTypeDef

```python
# DescribeInputRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import DescribeInputRequestTypeDef


def get_value() -> DescribeInputRequestTypeDef:
    return {
        "inputName": ...,
    }


# DescribeInputRequestTypeDef definition

class DescribeInputRequestTypeDef(TypedDict):
    inputName: str,
```

## DetectorDebugOptionTypeDef

```python
# DetectorDebugOptionTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import DetectorDebugOptionTypeDef


def get_value() -> DetectorDebugOptionTypeDef:
    return {
        "detectorModelName": ...,
    }


# DetectorDebugOptionTypeDef definition

class DetectorDebugOptionTypeDef(TypedDict):
    detectorModelName: str,
    keyValue: NotRequired[str],
```

## DetectorModelSummaryTypeDef

```python
# DetectorModelSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import DetectorModelSummaryTypeDef


def get_value() -> DetectorModelSummaryTypeDef:
    return {
        "detectorModelName": ...,
    }


# DetectorModelSummaryTypeDef definition

class DetectorModelSummaryTypeDef(TypedDict):
    detectorModelName: NotRequired[str],
    detectorModelDescription: NotRequired[str],
    creationTime: NotRequired[datetime],
```

## DetectorModelVersionSummaryTypeDef

```python
# DetectorModelVersionSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import DetectorModelVersionSummaryTypeDef


def get_value() -> DetectorModelVersionSummaryTypeDef:
    return {
        "detectorModelName": ...,
    }


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
# PayloadTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import PayloadTypeDef


def get_value() -> PayloadTypeDef:
    return {
        "contentExpression": ...,
    }


# PayloadTypeDef definition

class PayloadTypeDef(TypedDict):
    contentExpression: str,
    type: PayloadTypeType,  # (1)
```

1. See [:material-code-brackets: PayloadTypeType](./literals.md#payloadtypetype) 
## EmailContentTypeDef

```python
# EmailContentTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import EmailContentTypeDef


def get_value() -> EmailContentTypeDef:
    return {
        "subject": ...,
    }


# EmailContentTypeDef definition

class EmailContentTypeDef(TypedDict):
    subject: NotRequired[str],
    additionalMessage: NotRequired[str],
```

## GetDetectorModelAnalysisResultsRequestTypeDef

```python
# GetDetectorModelAnalysisResultsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import GetDetectorModelAnalysisResultsRequestTypeDef


def get_value() -> GetDetectorModelAnalysisResultsRequestTypeDef:
    return {
        "analysisId": ...,
    }


# GetDetectorModelAnalysisResultsRequestTypeDef definition

class GetDetectorModelAnalysisResultsRequestTypeDef(TypedDict):
    analysisId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## IotEventsInputIdentifierTypeDef

```python
# IotEventsInputIdentifierTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import IotEventsInputIdentifierTypeDef


def get_value() -> IotEventsInputIdentifierTypeDef:
    return {
        "inputName": ...,
    }


# IotEventsInputIdentifierTypeDef definition

class IotEventsInputIdentifierTypeDef(TypedDict):
    inputName: str,
```

## InputSummaryTypeDef

```python
# InputSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import InputSummaryTypeDef


def get_value() -> InputSummaryTypeDef:
    return {
        "inputName": ...,
    }


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
# IotSiteWiseAssetModelPropertyIdentifierTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import IotSiteWiseAssetModelPropertyIdentifierTypeDef


def get_value() -> IotSiteWiseAssetModelPropertyIdentifierTypeDef:
    return {
        "assetModelId": ...,
    }


# IotSiteWiseAssetModelPropertyIdentifierTypeDef definition

class IotSiteWiseAssetModelPropertyIdentifierTypeDef(TypedDict):
    assetModelId: str,
    propertyId: str,
```

## ListAlarmModelVersionsRequestTypeDef

```python
# ListAlarmModelVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import ListAlarmModelVersionsRequestTypeDef


def get_value() -> ListAlarmModelVersionsRequestTypeDef:
    return {
        "alarmModelName": ...,
    }


# ListAlarmModelVersionsRequestTypeDef definition

class ListAlarmModelVersionsRequestTypeDef(TypedDict):
    alarmModelName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListAlarmModelsRequestTypeDef

```python
# ListAlarmModelsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import ListAlarmModelsRequestTypeDef


def get_value() -> ListAlarmModelsRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListAlarmModelsRequestTypeDef definition

class ListAlarmModelsRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDetectorModelVersionsRequestTypeDef

```python
# ListDetectorModelVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import ListDetectorModelVersionsRequestTypeDef


def get_value() -> ListDetectorModelVersionsRequestTypeDef:
    return {
        "detectorModelName": ...,
    }


# ListDetectorModelVersionsRequestTypeDef definition

class ListDetectorModelVersionsRequestTypeDef(TypedDict):
    detectorModelName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDetectorModelsRequestTypeDef

```python
# ListDetectorModelsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import ListDetectorModelsRequestTypeDef


def get_value() -> ListDetectorModelsRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListDetectorModelsRequestTypeDef definition

class ListDetectorModelsRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## RoutedResourceTypeDef

```python
# RoutedResourceTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import RoutedResourceTypeDef


def get_value() -> RoutedResourceTypeDef:
    return {
        "name": ...,
    }


# RoutedResourceTypeDef definition

class RoutedResourceTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
```

## ListInputsRequestTypeDef

```python
# ListInputsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import ListInputsRequestTypeDef


def get_value() -> ListInputsRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListInputsRequestTypeDef definition

class ListInputsRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## SSOIdentityTypeDef

```python
# SSOIdentityTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import SSOIdentityTypeDef


def get_value() -> SSOIdentityTypeDef:
    return {
        "identityStoreId": ...,
    }


# SSOIdentityTypeDef definition

class SSOIdentityTypeDef(TypedDict):
    identityStoreId: str,
    userId: NotRequired[str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## AlarmCapabilitiesTypeDef

```python
# AlarmCapabilitiesTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import AlarmCapabilitiesTypeDef


def get_value() -> AlarmCapabilitiesTypeDef:
    return {
        "initializationConfiguration": ...,
    }


# AlarmCapabilitiesTypeDef definition

class AlarmCapabilitiesTypeDef(TypedDict):
    initializationConfiguration: NotRequired[InitializationConfigurationTypeDef],  # (1)
    acknowledgeFlow: NotRequired[AcknowledgeFlowTypeDef],  # (2)
```

1. See [:material-code-braces: InitializationConfigurationTypeDef](./type_defs.md#initializationconfigurationtypedef) 
2. See [:material-code-braces: AcknowledgeFlowTypeDef](./type_defs.md#acknowledgeflowtypedef) 
## AlarmRuleTypeDef

```python
# AlarmRuleTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import AlarmRuleTypeDef


def get_value() -> AlarmRuleTypeDef:
    return {
        "simpleRule": ...,
    }


# AlarmRuleTypeDef definition

class AlarmRuleTypeDef(TypedDict):
    simpleRule: NotRequired[SimpleRuleTypeDef],  # (1)
```

1. See [:material-code-braces: SimpleRuleTypeDef](./type_defs.md#simpleruletypedef) 
## AnalysisResultTypeDef

```python
# AnalysisResultTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import AnalysisResultTypeDef


def get_value() -> AnalysisResultTypeDef:
    return {
        "type": ...,
    }


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
# AssetPropertyValueTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import AssetPropertyValueTypeDef


def get_value() -> AssetPropertyValueTypeDef:
    return {
        "value": ...,
    }


# AssetPropertyValueTypeDef definition

class AssetPropertyValueTypeDef(TypedDict):
    value: NotRequired[AssetPropertyVariantTypeDef],  # (1)
    timestamp: NotRequired[AssetPropertyTimestampTypeDef],  # (2)
    quality: NotRequired[str],
```

1. See [:material-code-braces: AssetPropertyVariantTypeDef](./type_defs.md#assetpropertyvarianttypedef) 
2. See [:material-code-braces: AssetPropertyTimestampTypeDef](./type_defs.md#assetpropertytimestamptypedef) 
## InputDefinitionOutputTypeDef

```python
# InputDefinitionOutputTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import InputDefinitionOutputTypeDef


def get_value() -> InputDefinitionOutputTypeDef:
    return {
        "attributes": ...,
    }


# InputDefinitionOutputTypeDef definition

class InputDefinitionOutputTypeDef(TypedDict):
    attributes: List[AttributeTypeDef],  # (1)
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
## InputDefinitionTypeDef

```python
# InputDefinitionTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import InputDefinitionTypeDef


def get_value() -> InputDefinitionTypeDef:
    return {
        "attributes": ...,
    }


# InputDefinitionTypeDef definition

class InputDefinitionTypeDef(TypedDict):
    attributes: Sequence[AttributeTypeDef],  # (1)
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateAlarmModelResponseTypeDef

```python
# CreateAlarmModelResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import CreateAlarmModelResponseTypeDef


def get_value() -> CreateAlarmModelResponseTypeDef:
    return {
        "creationTime": ...,
    }


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
# DescribeDetectorModelAnalysisResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import DescribeDetectorModelAnalysisResponseTypeDef


def get_value() -> DescribeDetectorModelAnalysisResponseTypeDef:
    return {
        "status": ...,
    }


# DescribeDetectorModelAnalysisResponseTypeDef definition

class DescribeDetectorModelAnalysisResponseTypeDef(TypedDict):
    status: AnalysisStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AnalysisStatusType](./literals.md#analysisstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAlarmModelVersionsResponseTypeDef

```python
# ListAlarmModelVersionsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import ListAlarmModelVersionsResponseTypeDef


def get_value() -> ListAlarmModelVersionsResponseTypeDef:
    return {
        "alarmModelVersionSummaries": ...,
    }


# ListAlarmModelVersionsResponseTypeDef definition

class ListAlarmModelVersionsResponseTypeDef(TypedDict):
    alarmModelVersionSummaries: List[AlarmModelVersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AlarmModelVersionSummaryTypeDef](./type_defs.md#alarmmodelversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAlarmModelsResponseTypeDef

```python
# ListAlarmModelsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import ListAlarmModelsResponseTypeDef


def get_value() -> ListAlarmModelsResponseTypeDef:
    return {
        "alarmModelSummaries": ...,
    }


# ListAlarmModelsResponseTypeDef definition

class ListAlarmModelsResponseTypeDef(TypedDict):
    alarmModelSummaries: List[AlarmModelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AlarmModelSummaryTypeDef](./type_defs.md#alarmmodelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDetectorModelAnalysisResponseTypeDef

```python
# StartDetectorModelAnalysisResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import StartDetectorModelAnalysisResponseTypeDef


def get_value() -> StartDetectorModelAnalysisResponseTypeDef:
    return {
        "analysisId": ...,
    }


# StartDetectorModelAnalysisResponseTypeDef definition

class StartDetectorModelAnalysisResponseTypeDef(TypedDict):
    analysisId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAlarmModelResponseTypeDef

```python
# UpdateAlarmModelResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import UpdateAlarmModelResponseTypeDef


def get_value() -> UpdateAlarmModelResponseTypeDef:
    return {
        "creationTime": ...,
    }


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
# CreateDetectorModelResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import CreateDetectorModelResponseTypeDef


def get_value() -> CreateDetectorModelResponseTypeDef:
    return {
        "detectorModelConfiguration": ...,
    }


# CreateDetectorModelResponseTypeDef definition

class CreateDetectorModelResponseTypeDef(TypedDict):
    detectorModelConfiguration: DetectorModelConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DetectorModelConfigurationTypeDef](./type_defs.md#detectormodelconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDetectorModelResponseTypeDef

```python
# UpdateDetectorModelResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import UpdateDetectorModelResponseTypeDef


def get_value() -> UpdateDetectorModelResponseTypeDef:
    return {
        "detectorModelConfiguration": ...,
    }


# UpdateDetectorModelResponseTypeDef definition

class UpdateDetectorModelResponseTypeDef(TypedDict):
    detectorModelConfiguration: DetectorModelConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DetectorModelConfigurationTypeDef](./type_defs.md#detectormodelconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInputResponseTypeDef

```python
# CreateInputResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import CreateInputResponseTypeDef


def get_value() -> CreateInputResponseTypeDef:
    return {
        "inputConfiguration": ...,
    }


# CreateInputResponseTypeDef definition

class CreateInputResponseTypeDef(TypedDict):
    inputConfiguration: InputConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InputConfigurationTypeDef](./type_defs.md#inputconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateInputResponseTypeDef

```python
# UpdateInputResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import UpdateInputResponseTypeDef


def get_value() -> UpdateInputResponseTypeDef:
    return {
        "inputConfiguration": ...,
    }


# UpdateInputResponseTypeDef definition

class UpdateInputResponseTypeDef(TypedDict):
    inputConfiguration: InputConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InputConfigurationTypeDef](./type_defs.md#inputconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LoggingOptionsOutputTypeDef

```python
# LoggingOptionsOutputTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import LoggingOptionsOutputTypeDef


def get_value() -> LoggingOptionsOutputTypeDef:
    return {
        "roleArn": ...,
    }


# LoggingOptionsOutputTypeDef definition

class LoggingOptionsOutputTypeDef(TypedDict):
    roleArn: str,
    level: LoggingLevelType,  # (1)
    enabled: bool,
    detectorDebugOptions: NotRequired[List[DetectorDebugOptionTypeDef]],  # (2)
```

1. See [:material-code-brackets: LoggingLevelType](./literals.md#loggingleveltype) 
2. See [:material-code-braces: DetectorDebugOptionTypeDef](./type_defs.md#detectordebugoptiontypedef) 
## LoggingOptionsTypeDef

```python
# LoggingOptionsTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import LoggingOptionsTypeDef


def get_value() -> LoggingOptionsTypeDef:
    return {
        "roleArn": ...,
    }


# LoggingOptionsTypeDef definition

class LoggingOptionsTypeDef(TypedDict):
    roleArn: str,
    level: LoggingLevelType,  # (1)
    enabled: bool,
    detectorDebugOptions: NotRequired[Sequence[DetectorDebugOptionTypeDef]],  # (2)
```

1. See [:material-code-brackets: LoggingLevelType](./literals.md#loggingleveltype) 
2. See [:material-code-braces: DetectorDebugOptionTypeDef](./type_defs.md#detectordebugoptiontypedef) 
## ListDetectorModelsResponseTypeDef

```python
# ListDetectorModelsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import ListDetectorModelsResponseTypeDef


def get_value() -> ListDetectorModelsResponseTypeDef:
    return {
        "detectorModelSummaries": ...,
    }


# ListDetectorModelsResponseTypeDef definition

class ListDetectorModelsResponseTypeDef(TypedDict):
    detectorModelSummaries: List[DetectorModelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DetectorModelSummaryTypeDef](./type_defs.md#detectormodelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDetectorModelVersionsResponseTypeDef

```python
# ListDetectorModelVersionsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import ListDetectorModelVersionsResponseTypeDef


def get_value() -> ListDetectorModelVersionsResponseTypeDef:
    return {
        "detectorModelVersionSummaries": ...,
    }


# ListDetectorModelVersionsResponseTypeDef definition

class ListDetectorModelVersionsResponseTypeDef(TypedDict):
    detectorModelVersionSummaries: List[DetectorModelVersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DetectorModelVersionSummaryTypeDef](./type_defs.md#detectormodelversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DynamoDBActionTypeDef

```python
# DynamoDBActionTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import DynamoDBActionTypeDef


def get_value() -> DynamoDBActionTypeDef:
    return {
        "hashKeyType": ...,
    }


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
# DynamoDBv2ActionTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import DynamoDBv2ActionTypeDef


def get_value() -> DynamoDBv2ActionTypeDef:
    return {
        "tableName": ...,
    }


# DynamoDBv2ActionTypeDef definition

class DynamoDBv2ActionTypeDef(TypedDict):
    tableName: str,
    payload: NotRequired[PayloadTypeDef],  # (1)
```

1. See [:material-code-braces: PayloadTypeDef](./type_defs.md#payloadtypedef) 
## FirehoseActionTypeDef

```python
# FirehoseActionTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import FirehoseActionTypeDef


def get_value() -> FirehoseActionTypeDef:
    return {
        "deliveryStreamName": ...,
    }


# FirehoseActionTypeDef definition

class FirehoseActionTypeDef(TypedDict):
    deliveryStreamName: str,
    separator: NotRequired[str],
    payload: NotRequired[PayloadTypeDef],  # (1)
```

1. See [:material-code-braces: PayloadTypeDef](./type_defs.md#payloadtypedef) 
## IotEventsActionTypeDef

```python
# IotEventsActionTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import IotEventsActionTypeDef


def get_value() -> IotEventsActionTypeDef:
    return {
        "inputName": ...,
    }


# IotEventsActionTypeDef definition

class IotEventsActionTypeDef(TypedDict):
    inputName: str,
    payload: NotRequired[PayloadTypeDef],  # (1)
```

1. See [:material-code-braces: PayloadTypeDef](./type_defs.md#payloadtypedef) 
## IotTopicPublishActionTypeDef

```python
# IotTopicPublishActionTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import IotTopicPublishActionTypeDef


def get_value() -> IotTopicPublishActionTypeDef:
    return {
        "mqttTopic": ...,
    }


# IotTopicPublishActionTypeDef definition

class IotTopicPublishActionTypeDef(TypedDict):
    mqttTopic: str,
    payload: NotRequired[PayloadTypeDef],  # (1)
```

1. See [:material-code-braces: PayloadTypeDef](./type_defs.md#payloadtypedef) 
## LambdaActionTypeDef

```python
# LambdaActionTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import LambdaActionTypeDef


def get_value() -> LambdaActionTypeDef:
    return {
        "functionArn": ...,
    }


# LambdaActionTypeDef definition

class LambdaActionTypeDef(TypedDict):
    functionArn: str,
    payload: NotRequired[PayloadTypeDef],  # (1)
```

1. See [:material-code-braces: PayloadTypeDef](./type_defs.md#payloadtypedef) 
## SNSTopicPublishActionTypeDef

```python
# SNSTopicPublishActionTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import SNSTopicPublishActionTypeDef


def get_value() -> SNSTopicPublishActionTypeDef:
    return {
        "targetArn": ...,
    }


# SNSTopicPublishActionTypeDef definition

class SNSTopicPublishActionTypeDef(TypedDict):
    targetArn: str,
    payload: NotRequired[PayloadTypeDef],  # (1)
```

1. See [:material-code-braces: PayloadTypeDef](./type_defs.md#payloadtypedef) 
## SqsActionTypeDef

```python
# SqsActionTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import SqsActionTypeDef


def get_value() -> SqsActionTypeDef:
    return {
        "queueUrl": ...,
    }


# SqsActionTypeDef definition

class SqsActionTypeDef(TypedDict):
    queueUrl: str,
    useBase64: NotRequired[bool],
    payload: NotRequired[PayloadTypeDef],  # (1)
```

1. See [:material-code-braces: PayloadTypeDef](./type_defs.md#payloadtypedef) 
## ListInputsResponseTypeDef

```python
# ListInputsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import ListInputsResponseTypeDef


def get_value() -> ListInputsResponseTypeDef:
    return {
        "inputSummaries": ...,
    }


# ListInputsResponseTypeDef definition

class ListInputsResponseTypeDef(TypedDict):
    inputSummaries: List[InputSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: InputSummaryTypeDef](./type_defs.md#inputsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IotSiteWiseInputIdentifierTypeDef

```python
# IotSiteWiseInputIdentifierTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import IotSiteWiseInputIdentifierTypeDef


def get_value() -> IotSiteWiseInputIdentifierTypeDef:
    return {
        "iotSiteWiseAssetModelPropertyIdentifier": ...,
    }


# IotSiteWiseInputIdentifierTypeDef definition

class IotSiteWiseInputIdentifierTypeDef(TypedDict):
    iotSiteWiseAssetModelPropertyIdentifier: NotRequired[IotSiteWiseAssetModelPropertyIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: IotSiteWiseAssetModelPropertyIdentifierTypeDef](./type_defs.md#iotsitewiseassetmodelpropertyidentifiertypedef) 
## ListInputRoutingsResponseTypeDef

```python
# ListInputRoutingsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import ListInputRoutingsResponseTypeDef


def get_value() -> ListInputRoutingsResponseTypeDef:
    return {
        "routedResources": ...,
    }


# ListInputRoutingsResponseTypeDef definition

class ListInputRoutingsResponseTypeDef(TypedDict):
    routedResources: List[RoutedResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RoutedResourceTypeDef](./type_defs.md#routedresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RecipientDetailTypeDef

```python
# RecipientDetailTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import RecipientDetailTypeDef


def get_value() -> RecipientDetailTypeDef:
    return {
        "ssoIdentity": ...,
    }


# RecipientDetailTypeDef definition

class RecipientDetailTypeDef(TypedDict):
    ssoIdentity: NotRequired[SSOIdentityTypeDef],  # (1)
```

1. See [:material-code-braces: SSOIdentityTypeDef](./type_defs.md#ssoidentitytypedef) 
## GetDetectorModelAnalysisResultsResponseTypeDef

```python
# GetDetectorModelAnalysisResultsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import GetDetectorModelAnalysisResultsResponseTypeDef


def get_value() -> GetDetectorModelAnalysisResultsResponseTypeDef:
    return {
        "analysisResults": ...,
    }


# GetDetectorModelAnalysisResultsResponseTypeDef definition

class GetDetectorModelAnalysisResultsResponseTypeDef(TypedDict):
    analysisResults: List[AnalysisResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AnalysisResultTypeDef](./type_defs.md#analysisresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IotSiteWiseActionTypeDef

```python
# IotSiteWiseActionTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import IotSiteWiseActionTypeDef


def get_value() -> IotSiteWiseActionTypeDef:
    return {
        "entryId": ...,
    }


# IotSiteWiseActionTypeDef definition

class IotSiteWiseActionTypeDef(TypedDict):
    entryId: NotRequired[str],
    assetId: NotRequired[str],
    propertyId: NotRequired[str],
    propertyAlias: NotRequired[str],
    propertyValue: NotRequired[AssetPropertyValueTypeDef],  # (1)
```

1. See [:material-code-braces: AssetPropertyValueTypeDef](./type_defs.md#assetpropertyvaluetypedef) 
## InputTypeDef

```python
# InputTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import InputTypeDef


def get_value() -> InputTypeDef:
    return {
        "inputConfiguration": ...,
    }


# InputTypeDef definition

class InputTypeDef(TypedDict):
    inputConfiguration: NotRequired[InputConfigurationTypeDef],  # (1)
    inputDefinition: NotRequired[InputDefinitionOutputTypeDef],  # (2)
```

1. See [:material-code-braces: InputConfigurationTypeDef](./type_defs.md#inputconfigurationtypedef) 
2. See [:material-code-braces: InputDefinitionOutputTypeDef](./type_defs.md#inputdefinitionoutputtypedef) 
## DescribeLoggingOptionsResponseTypeDef

```python
# DescribeLoggingOptionsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import DescribeLoggingOptionsResponseTypeDef


def get_value() -> DescribeLoggingOptionsResponseTypeDef:
    return {
        "loggingOptions": ...,
    }


# DescribeLoggingOptionsResponseTypeDef definition

class DescribeLoggingOptionsResponseTypeDef(TypedDict):
    loggingOptions: LoggingOptionsOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingOptionsOutputTypeDef](./type_defs.md#loggingoptionsoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NotificationTargetActionsTypeDef

```python
# NotificationTargetActionsTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import NotificationTargetActionsTypeDef


def get_value() -> NotificationTargetActionsTypeDef:
    return {
        "lambdaAction": ...,
    }


# NotificationTargetActionsTypeDef definition

class NotificationTargetActionsTypeDef(TypedDict):
    lambdaAction: NotRequired[LambdaActionTypeDef],  # (1)
```

1. See [:material-code-braces: LambdaActionTypeDef](./type_defs.md#lambdaactiontypedef) 
## InputIdentifierTypeDef

```python
# InputIdentifierTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import InputIdentifierTypeDef


def get_value() -> InputIdentifierTypeDef:
    return {
        "iotEventsInputIdentifier": ...,
    }


# InputIdentifierTypeDef definition

class InputIdentifierTypeDef(TypedDict):
    iotEventsInputIdentifier: NotRequired[IotEventsInputIdentifierTypeDef],  # (1)
    iotSiteWiseInputIdentifier: NotRequired[IotSiteWiseInputIdentifierTypeDef],  # (2)
```

1. See [:material-code-braces: IotEventsInputIdentifierTypeDef](./type_defs.md#ioteventsinputidentifiertypedef) 
2. See [:material-code-braces: IotSiteWiseInputIdentifierTypeDef](./type_defs.md#iotsitewiseinputidentifiertypedef) 
## EmailRecipientsOutputTypeDef

```python
# EmailRecipientsOutputTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import EmailRecipientsOutputTypeDef


def get_value() -> EmailRecipientsOutputTypeDef:
    return {
        "to": ...,
    }


# EmailRecipientsOutputTypeDef definition

class EmailRecipientsOutputTypeDef(TypedDict):
    to: NotRequired[List[RecipientDetailTypeDef]],  # (1)
```

1. See [:material-code-braces: RecipientDetailTypeDef](./type_defs.md#recipientdetailtypedef) 
## EmailRecipientsTypeDef

```python
# EmailRecipientsTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import EmailRecipientsTypeDef


def get_value() -> EmailRecipientsTypeDef:
    return {
        "to": ...,
    }


# EmailRecipientsTypeDef definition

class EmailRecipientsTypeDef(TypedDict):
    to: NotRequired[Sequence[RecipientDetailTypeDef]],  # (1)
```

1. See [:material-code-braces: RecipientDetailTypeDef](./type_defs.md#recipientdetailtypedef) 
## SMSConfigurationOutputTypeDef

```python
# SMSConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import SMSConfigurationOutputTypeDef


def get_value() -> SMSConfigurationOutputTypeDef:
    return {
        "senderId": ...,
    }


# SMSConfigurationOutputTypeDef definition

class SMSConfigurationOutputTypeDef(TypedDict):
    recipients: List[RecipientDetailTypeDef],  # (1)
    senderId: NotRequired[str],
    additionalMessage: NotRequired[str],
```

1. See [:material-code-braces: RecipientDetailTypeDef](./type_defs.md#recipientdetailtypedef) 
## SMSConfigurationTypeDef

```python
# SMSConfigurationTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import SMSConfigurationTypeDef


def get_value() -> SMSConfigurationTypeDef:
    return {
        "senderId": ...,
    }


# SMSConfigurationTypeDef definition

class SMSConfigurationTypeDef(TypedDict):
    recipients: Sequence[RecipientDetailTypeDef],  # (1)
    senderId: NotRequired[str],
    additionalMessage: NotRequired[str],
```

1. See [:material-code-braces: RecipientDetailTypeDef](./type_defs.md#recipientdetailtypedef) 
## ActionTypeDef

```python
# ActionTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import ActionTypeDef


def get_value() -> ActionTypeDef:
    return {
        "setVariable": ...,
    }


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
# AlarmActionTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import AlarmActionTypeDef


def get_value() -> AlarmActionTypeDef:
    return {
        "sns": ...,
    }


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
# DescribeInputResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import DescribeInputResponseTypeDef


def get_value() -> DescribeInputResponseTypeDef:
    return {
        "input": ...,
    }


# DescribeInputResponseTypeDef definition

class DescribeInputResponseTypeDef(TypedDict):
    input: InputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InputTypeDef](./type_defs.md#inputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInputRequestTypeDef

```python
# CreateInputRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import CreateInputRequestTypeDef


def get_value() -> CreateInputRequestTypeDef:
    return {
        "inputName": ...,
    }


# CreateInputRequestTypeDef definition

class CreateInputRequestTypeDef(TypedDict):
    inputName: str,
    inputDefinition: InputDefinitionUnionTypeDef,  # (1)
    inputDescription: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: InputDefinitionTypeDef](./type_defs.md#inputdefinitiontypedef) [:material-code-braces: InputDefinitionOutputTypeDef](./type_defs.md#inputdefinitionoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateInputRequestTypeDef

```python
# UpdateInputRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import UpdateInputRequestTypeDef


def get_value() -> UpdateInputRequestTypeDef:
    return {
        "inputName": ...,
    }


# UpdateInputRequestTypeDef definition

class UpdateInputRequestTypeDef(TypedDict):
    inputName: str,
    inputDefinition: InputDefinitionUnionTypeDef,  # (1)
    inputDescription: NotRequired[str],
```

1. See [:material-code-braces: InputDefinitionTypeDef](./type_defs.md#inputdefinitiontypedef) [:material-code-braces: InputDefinitionOutputTypeDef](./type_defs.md#inputdefinitionoutputtypedef) 
## PutLoggingOptionsRequestTypeDef

```python
# PutLoggingOptionsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import PutLoggingOptionsRequestTypeDef


def get_value() -> PutLoggingOptionsRequestTypeDef:
    return {
        "loggingOptions": ...,
    }


# PutLoggingOptionsRequestTypeDef definition

class PutLoggingOptionsRequestTypeDef(TypedDict):
    loggingOptions: LoggingOptionsUnionTypeDef,  # (1)
```

1. See [:material-code-braces: LoggingOptionsTypeDef](./type_defs.md#loggingoptionstypedef) [:material-code-braces: LoggingOptionsOutputTypeDef](./type_defs.md#loggingoptionsoutputtypedef) 
## ListInputRoutingsRequestTypeDef

```python
# ListInputRoutingsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import ListInputRoutingsRequestTypeDef


def get_value() -> ListInputRoutingsRequestTypeDef:
    return {
        "inputIdentifier": ...,
    }


# ListInputRoutingsRequestTypeDef definition

class ListInputRoutingsRequestTypeDef(TypedDict):
    inputIdentifier: InputIdentifierTypeDef,  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: InputIdentifierTypeDef](./type_defs.md#inputidentifiertypedef) 
## EmailConfigurationOutputTypeDef

```python
# EmailConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import EmailConfigurationOutputTypeDef


def get_value() -> EmailConfigurationOutputTypeDef:
    return {
        "from": ...,
    }


# EmailConfigurationOutputTypeDef definition

class EmailConfigurationOutputTypeDef(TypedDict):
    from: str,
    recipients: EmailRecipientsOutputTypeDef,  # (2)
    content: NotRequired[EmailContentTypeDef],  # (1)
```

1. See [:material-code-braces: EmailContentTypeDef](./type_defs.md#emailcontenttypedef) 
2. See [:material-code-braces: EmailRecipientsOutputTypeDef](./type_defs.md#emailrecipientsoutputtypedef) 
## EmailConfigurationTypeDef

```python
# EmailConfigurationTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import EmailConfigurationTypeDef


def get_value() -> EmailConfigurationTypeDef:
    return {
        "from": ...,
    }


# EmailConfigurationTypeDef definition

class EmailConfigurationTypeDef(TypedDict):
    from: str,
    recipients: EmailRecipientsTypeDef,  # (2)
    content: NotRequired[EmailContentTypeDef],  # (1)
```

1. See [:material-code-braces: EmailContentTypeDef](./type_defs.md#emailcontenttypedef) 
2. See [:material-code-braces: EmailRecipientsTypeDef](./type_defs.md#emailrecipientstypedef) 
## EventOutputTypeDef

```python
# EventOutputTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import EventOutputTypeDef


def get_value() -> EventOutputTypeDef:
    return {
        "eventName": ...,
    }


# EventOutputTypeDef definition

class EventOutputTypeDef(TypedDict):
    eventName: str,
    condition: NotRequired[str],
    actions: NotRequired[List[ActionTypeDef]],  # (1)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
## EventTypeDef

```python
# EventTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import EventTypeDef


def get_value() -> EventTypeDef:
    return {
        "eventName": ...,
    }


# EventTypeDef definition

class EventTypeDef(TypedDict):
    eventName: str,
    condition: NotRequired[str],
    actions: NotRequired[Sequence[ActionTypeDef]],  # (1)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
## TransitionEventOutputTypeDef

```python
# TransitionEventOutputTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import TransitionEventOutputTypeDef


def get_value() -> TransitionEventOutputTypeDef:
    return {
        "eventName": ...,
    }


# TransitionEventOutputTypeDef definition

class TransitionEventOutputTypeDef(TypedDict):
    eventName: str,
    condition: str,
    nextState: str,
    actions: NotRequired[List[ActionTypeDef]],  # (1)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
## TransitionEventTypeDef

```python
# TransitionEventTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import TransitionEventTypeDef


def get_value() -> TransitionEventTypeDef:
    return {
        "eventName": ...,
    }


# TransitionEventTypeDef definition

class TransitionEventTypeDef(TypedDict):
    eventName: str,
    condition: str,
    nextState: str,
    actions: NotRequired[Sequence[ActionTypeDef]],  # (1)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
## AlarmEventActionsOutputTypeDef

```python
# AlarmEventActionsOutputTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import AlarmEventActionsOutputTypeDef


def get_value() -> AlarmEventActionsOutputTypeDef:
    return {
        "alarmActions": ...,
    }


# AlarmEventActionsOutputTypeDef definition

class AlarmEventActionsOutputTypeDef(TypedDict):
    alarmActions: NotRequired[List[AlarmActionTypeDef]],  # (1)
```

1. See [:material-code-braces: AlarmActionTypeDef](./type_defs.md#alarmactiontypedef) 
## AlarmEventActionsTypeDef

```python
# AlarmEventActionsTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import AlarmEventActionsTypeDef


def get_value() -> AlarmEventActionsTypeDef:
    return {
        "alarmActions": ...,
    }


# AlarmEventActionsTypeDef definition

class AlarmEventActionsTypeDef(TypedDict):
    alarmActions: NotRequired[Sequence[AlarmActionTypeDef]],  # (1)
```

1. See [:material-code-braces: AlarmActionTypeDef](./type_defs.md#alarmactiontypedef) 
## NotificationActionOutputTypeDef

```python
# NotificationActionOutputTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import NotificationActionOutputTypeDef


def get_value() -> NotificationActionOutputTypeDef:
    return {
        "action": ...,
    }


# NotificationActionOutputTypeDef definition

class NotificationActionOutputTypeDef(TypedDict):
    action: NotificationTargetActionsTypeDef,  # (1)
    smsConfigurations: NotRequired[List[SMSConfigurationOutputTypeDef]],  # (2)
    emailConfigurations: NotRequired[List[EmailConfigurationOutputTypeDef]],  # (3)
```

1. See [:material-code-braces: NotificationTargetActionsTypeDef](./type_defs.md#notificationtargetactionstypedef) 
2. See [:material-code-braces: SMSConfigurationOutputTypeDef](./type_defs.md#smsconfigurationoutputtypedef) 
3. See [:material-code-braces: EmailConfigurationOutputTypeDef](./type_defs.md#emailconfigurationoutputtypedef) 
## NotificationActionTypeDef

```python
# NotificationActionTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import NotificationActionTypeDef


def get_value() -> NotificationActionTypeDef:
    return {
        "action": ...,
    }


# NotificationActionTypeDef definition

class NotificationActionTypeDef(TypedDict):
    action: NotificationTargetActionsTypeDef,  # (1)
    smsConfigurations: NotRequired[Sequence[SMSConfigurationTypeDef]],  # (2)
    emailConfigurations: NotRequired[Sequence[EmailConfigurationTypeDef]],  # (3)
```

1. See [:material-code-braces: NotificationTargetActionsTypeDef](./type_defs.md#notificationtargetactionstypedef) 
2. See [:material-code-braces: SMSConfigurationTypeDef](./type_defs.md#smsconfigurationtypedef) 
3. See [:material-code-braces: EmailConfigurationTypeDef](./type_defs.md#emailconfigurationtypedef) 
## OnEnterLifecycleOutputTypeDef

```python
# OnEnterLifecycleOutputTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import OnEnterLifecycleOutputTypeDef


def get_value() -> OnEnterLifecycleOutputTypeDef:
    return {
        "events": ...,
    }


# OnEnterLifecycleOutputTypeDef definition

class OnEnterLifecycleOutputTypeDef(TypedDict):
    events: NotRequired[List[EventOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: EventOutputTypeDef](./type_defs.md#eventoutputtypedef) 
## OnExitLifecycleOutputTypeDef

```python
# OnExitLifecycleOutputTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import OnExitLifecycleOutputTypeDef


def get_value() -> OnExitLifecycleOutputTypeDef:
    return {
        "events": ...,
    }


# OnExitLifecycleOutputTypeDef definition

class OnExitLifecycleOutputTypeDef(TypedDict):
    events: NotRequired[List[EventOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: EventOutputTypeDef](./type_defs.md#eventoutputtypedef) 
## OnEnterLifecycleTypeDef

```python
# OnEnterLifecycleTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import OnEnterLifecycleTypeDef


def get_value() -> OnEnterLifecycleTypeDef:
    return {
        "events": ...,
    }


# OnEnterLifecycleTypeDef definition

class OnEnterLifecycleTypeDef(TypedDict):
    events: NotRequired[Sequence[EventTypeDef]],  # (1)
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
## OnExitLifecycleTypeDef

```python
# OnExitLifecycleTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import OnExitLifecycleTypeDef


def get_value() -> OnExitLifecycleTypeDef:
    return {
        "events": ...,
    }


# OnExitLifecycleTypeDef definition

class OnExitLifecycleTypeDef(TypedDict):
    events: NotRequired[Sequence[EventTypeDef]],  # (1)
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
## OnInputLifecycleOutputTypeDef

```python
# OnInputLifecycleOutputTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import OnInputLifecycleOutputTypeDef


def get_value() -> OnInputLifecycleOutputTypeDef:
    return {
        "events": ...,
    }


# OnInputLifecycleOutputTypeDef definition

class OnInputLifecycleOutputTypeDef(TypedDict):
    events: NotRequired[List[EventOutputTypeDef]],  # (1)
    transitionEvents: NotRequired[List[TransitionEventOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: EventOutputTypeDef](./type_defs.md#eventoutputtypedef) 
2. See [:material-code-braces: TransitionEventOutputTypeDef](./type_defs.md#transitioneventoutputtypedef) 
## OnInputLifecycleTypeDef

```python
# OnInputLifecycleTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import OnInputLifecycleTypeDef


def get_value() -> OnInputLifecycleTypeDef:
    return {
        "events": ...,
    }


# OnInputLifecycleTypeDef definition

class OnInputLifecycleTypeDef(TypedDict):
    events: NotRequired[Sequence[EventTypeDef]],  # (1)
    transitionEvents: NotRequired[Sequence[TransitionEventTypeDef]],  # (2)
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
2. See [:material-code-braces: TransitionEventTypeDef](./type_defs.md#transitioneventtypedef) 
## AlarmNotificationOutputTypeDef

```python
# AlarmNotificationOutputTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import AlarmNotificationOutputTypeDef


def get_value() -> AlarmNotificationOutputTypeDef:
    return {
        "notificationActions": ...,
    }


# AlarmNotificationOutputTypeDef definition

class AlarmNotificationOutputTypeDef(TypedDict):
    notificationActions: NotRequired[List[NotificationActionOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: NotificationActionOutputTypeDef](./type_defs.md#notificationactionoutputtypedef) 
## AlarmNotificationTypeDef

```python
# AlarmNotificationTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import AlarmNotificationTypeDef


def get_value() -> AlarmNotificationTypeDef:
    return {
        "notificationActions": ...,
    }


# AlarmNotificationTypeDef definition

class AlarmNotificationTypeDef(TypedDict):
    notificationActions: NotRequired[Sequence[NotificationActionTypeDef]],  # (1)
```

1. See [:material-code-braces: NotificationActionTypeDef](./type_defs.md#notificationactiontypedef) 
## StateOutputTypeDef

```python
# StateOutputTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import StateOutputTypeDef


def get_value() -> StateOutputTypeDef:
    return {
        "stateName": ...,
    }


# StateOutputTypeDef definition

class StateOutputTypeDef(TypedDict):
    stateName: str,
    onInput: NotRequired[OnInputLifecycleOutputTypeDef],  # (1)
    onEnter: NotRequired[OnEnterLifecycleOutputTypeDef],  # (2)
    onExit: NotRequired[OnExitLifecycleOutputTypeDef],  # (3)
```

1. See [:material-code-braces: OnInputLifecycleOutputTypeDef](./type_defs.md#oninputlifecycleoutputtypedef) 
2. See [:material-code-braces: OnEnterLifecycleOutputTypeDef](./type_defs.md#onenterlifecycleoutputtypedef) 
3. See [:material-code-braces: OnExitLifecycleOutputTypeDef](./type_defs.md#onexitlifecycleoutputtypedef) 
## StateTypeDef

```python
# StateTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import StateTypeDef


def get_value() -> StateTypeDef:
    return {
        "stateName": ...,
    }


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
## DescribeAlarmModelResponseTypeDef

```python
# DescribeAlarmModelResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import DescribeAlarmModelResponseTypeDef


def get_value() -> DescribeAlarmModelResponseTypeDef:
    return {
        "creationTime": ...,
    }


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
    alarmNotification: AlarmNotificationOutputTypeDef,  # (3)
    alarmEventActions: AlarmEventActionsOutputTypeDef,  # (4)
    alarmCapabilities: AlarmCapabilitiesTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: AlarmModelVersionStatusType](./literals.md#alarmmodelversionstatustype) 
2. See [:material-code-braces: AlarmRuleTypeDef](./type_defs.md#alarmruletypedef) 
3. See [:material-code-braces: AlarmNotificationOutputTypeDef](./type_defs.md#alarmnotificationoutputtypedef) 
4. See [:material-code-braces: AlarmEventActionsOutputTypeDef](./type_defs.md#alarmeventactionsoutputtypedef) 
5. See [:material-code-braces: AlarmCapabilitiesTypeDef](./type_defs.md#alarmcapabilitiestypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectorModelDefinitionOutputTypeDef

```python
# DetectorModelDefinitionOutputTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import DetectorModelDefinitionOutputTypeDef


def get_value() -> DetectorModelDefinitionOutputTypeDef:
    return {
        "states": ...,
    }


# DetectorModelDefinitionOutputTypeDef definition

class DetectorModelDefinitionOutputTypeDef(TypedDict):
    states: List[StateOutputTypeDef],  # (1)
    initialStateName: str,
```

1. See [:material-code-braces: StateOutputTypeDef](./type_defs.md#stateoutputtypedef) 
## DetectorModelDefinitionTypeDef

```python
# DetectorModelDefinitionTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import DetectorModelDefinitionTypeDef


def get_value() -> DetectorModelDefinitionTypeDef:
    return {
        "states": ...,
    }


# DetectorModelDefinitionTypeDef definition

class DetectorModelDefinitionTypeDef(TypedDict):
    states: Sequence[StateTypeDef],  # (1)
    initialStateName: str,
```

1. See [:material-code-braces: StateTypeDef](./type_defs.md#statetypedef) 
## CreateAlarmModelRequestTypeDef

```python
# CreateAlarmModelRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import CreateAlarmModelRequestTypeDef


def get_value() -> CreateAlarmModelRequestTypeDef:
    return {
        "alarmModelName": ...,
    }


# CreateAlarmModelRequestTypeDef definition

class CreateAlarmModelRequestTypeDef(TypedDict):
    alarmModelName: str,
    roleArn: str,
    alarmRule: AlarmRuleTypeDef,  # (1)
    alarmModelDescription: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    key: NotRequired[str],
    severity: NotRequired[int],
    alarmNotification: NotRequired[AlarmNotificationUnionTypeDef],  # (3)
    alarmEventActions: NotRequired[AlarmEventActionsUnionTypeDef],  # (4)
    alarmCapabilities: NotRequired[AlarmCapabilitiesTypeDef],  # (5)
```

1. See [:material-code-braces: AlarmRuleTypeDef](./type_defs.md#alarmruletypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: AlarmNotificationTypeDef](./type_defs.md#alarmnotificationtypedef) [:material-code-braces: AlarmNotificationOutputTypeDef](./type_defs.md#alarmnotificationoutputtypedef) 
4. See [:material-code-braces: AlarmEventActionsTypeDef](./type_defs.md#alarmeventactionstypedef) [:material-code-braces: AlarmEventActionsOutputTypeDef](./type_defs.md#alarmeventactionsoutputtypedef) 
5. See [:material-code-braces: AlarmCapabilitiesTypeDef](./type_defs.md#alarmcapabilitiestypedef) 
## UpdateAlarmModelRequestTypeDef

```python
# UpdateAlarmModelRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import UpdateAlarmModelRequestTypeDef


def get_value() -> UpdateAlarmModelRequestTypeDef:
    return {
        "alarmModelName": ...,
    }


# UpdateAlarmModelRequestTypeDef definition

class UpdateAlarmModelRequestTypeDef(TypedDict):
    alarmModelName: str,
    roleArn: str,
    alarmRule: AlarmRuleTypeDef,  # (1)
    alarmModelDescription: NotRequired[str],
    severity: NotRequired[int],
    alarmNotification: NotRequired[AlarmNotificationUnionTypeDef],  # (2)
    alarmEventActions: NotRequired[AlarmEventActionsUnionTypeDef],  # (3)
    alarmCapabilities: NotRequired[AlarmCapabilitiesTypeDef],  # (4)
```

1. See [:material-code-braces: AlarmRuleTypeDef](./type_defs.md#alarmruletypedef) 
2. See [:material-code-braces: AlarmNotificationTypeDef](./type_defs.md#alarmnotificationtypedef) [:material-code-braces: AlarmNotificationOutputTypeDef](./type_defs.md#alarmnotificationoutputtypedef) 
3. See [:material-code-braces: AlarmEventActionsTypeDef](./type_defs.md#alarmeventactionstypedef) [:material-code-braces: AlarmEventActionsOutputTypeDef](./type_defs.md#alarmeventactionsoutputtypedef) 
4. See [:material-code-braces: AlarmCapabilitiesTypeDef](./type_defs.md#alarmcapabilitiestypedef) 
## DetectorModelTypeDef

```python
# DetectorModelTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import DetectorModelTypeDef


def get_value() -> DetectorModelTypeDef:
    return {
        "detectorModelDefinition": ...,
    }


# DetectorModelTypeDef definition

class DetectorModelTypeDef(TypedDict):
    detectorModelDefinition: NotRequired[DetectorModelDefinitionOutputTypeDef],  # (1)
    detectorModelConfiguration: NotRequired[DetectorModelConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: DetectorModelDefinitionOutputTypeDef](./type_defs.md#detectormodeldefinitionoutputtypedef) 
2. See [:material-code-braces: DetectorModelConfigurationTypeDef](./type_defs.md#detectormodelconfigurationtypedef) 
## DescribeDetectorModelResponseTypeDef

```python
# DescribeDetectorModelResponseTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import DescribeDetectorModelResponseTypeDef


def get_value() -> DescribeDetectorModelResponseTypeDef:
    return {
        "detectorModel": ...,
    }


# DescribeDetectorModelResponseTypeDef definition

class DescribeDetectorModelResponseTypeDef(TypedDict):
    detectorModel: DetectorModelTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DetectorModelTypeDef](./type_defs.md#detectormodeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDetectorModelRequestTypeDef

```python
# CreateDetectorModelRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import CreateDetectorModelRequestTypeDef


def get_value() -> CreateDetectorModelRequestTypeDef:
    return {
        "detectorModelName": ...,
    }


# CreateDetectorModelRequestTypeDef definition

class CreateDetectorModelRequestTypeDef(TypedDict):
    detectorModelName: str,
    detectorModelDefinition: DetectorModelDefinitionUnionTypeDef,  # (1)
    roleArn: str,
    detectorModelDescription: NotRequired[str],
    key: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    evaluationMethod: NotRequired[EvaluationMethodType],  # (3)
```

1. See [:material-code-braces: DetectorModelDefinitionTypeDef](./type_defs.md#detectormodeldefinitiontypedef) [:material-code-braces: DetectorModelDefinitionOutputTypeDef](./type_defs.md#detectormodeldefinitionoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: EvaluationMethodType](./literals.md#evaluationmethodtype) 
## StartDetectorModelAnalysisRequestTypeDef

```python
# StartDetectorModelAnalysisRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import StartDetectorModelAnalysisRequestTypeDef


def get_value() -> StartDetectorModelAnalysisRequestTypeDef:
    return {
        "detectorModelDefinition": ...,
    }


# StartDetectorModelAnalysisRequestTypeDef definition

class StartDetectorModelAnalysisRequestTypeDef(TypedDict):
    detectorModelDefinition: DetectorModelDefinitionUnionTypeDef,  # (1)
```

1. See [:material-code-braces: DetectorModelDefinitionTypeDef](./type_defs.md#detectormodeldefinitiontypedef) [:material-code-braces: DetectorModelDefinitionOutputTypeDef](./type_defs.md#detectormodeldefinitionoutputtypedef) 
## UpdateDetectorModelRequestTypeDef

```python
# UpdateDetectorModelRequestTypeDef TypedDict usage example

from types_aiobotocore_iotevents.type_defs import UpdateDetectorModelRequestTypeDef


def get_value() -> UpdateDetectorModelRequestTypeDef:
    return {
        "detectorModelName": ...,
    }


# UpdateDetectorModelRequestTypeDef definition

class UpdateDetectorModelRequestTypeDef(TypedDict):
    detectorModelName: str,
    detectorModelDefinition: DetectorModelDefinitionUnionTypeDef,  # (1)
    roleArn: str,
    detectorModelDescription: NotRequired[str],
    evaluationMethod: NotRequired[EvaluationMethodType],  # (2)
```

1. See [:material-code-braces: DetectorModelDefinitionTypeDef](./type_defs.md#detectormodeldefinitiontypedef) [:material-code-braces: DetectorModelDefinitionOutputTypeDef](./type_defs.md#detectormodeldefinitionoutputtypedef) 
2. See [:material-code-brackets: EvaluationMethodType](./literals.md#evaluationmethodtype) 
