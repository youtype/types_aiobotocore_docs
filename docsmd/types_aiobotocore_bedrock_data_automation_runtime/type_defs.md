# Type definitions

> [Index](../README.md) > [RuntimeforBedrockDataAutomation](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [RuntimeforBedrockDataAutomation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation-runtime.html#runtimeforbedrockdataautomation)
    type annotations stubs module [types-aiobotocore-bedrock-data-automation-runtime](https://pypi.org/project/types-aiobotocore-bedrock-data-automation-runtime/).



## BlueprintTypeDef

```python
# BlueprintTypeDef TypedDict usage example

from types_aiobotocore_bedrock_data_automation_runtime.type_defs import BlueprintTypeDef


def get_value() -> BlueprintTypeDef:
    return {
        "blueprintArn": ...,
    }


# BlueprintTypeDef definition

class BlueprintTypeDef(TypedDict):
    blueprintArn: str,
    version: NotRequired[str],
    stage: NotRequired[BlueprintStageType],  # (1)
```

1. See [:material-code-brackets: BlueprintStageType](./literals.md#blueprintstagetype) 
## DataAutomationConfigurationTypeDef

```python
# DataAutomationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_data_automation_runtime.type_defs import DataAutomationConfigurationTypeDef


def get_value() -> DataAutomationConfigurationTypeDef:
    return {
        "dataAutomationArn": ...,
    }


# DataAutomationConfigurationTypeDef definition

class DataAutomationConfigurationTypeDef(TypedDict):
    dataAutomationArn: str,
    stage: NotRequired[DataAutomationStageType],  # (1)
```

1. See [:material-code-brackets: DataAutomationStageType](./literals.md#dataautomationstagetype) 
## EncryptionConfigurationTypeDef

```python
# EncryptionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_data_automation_runtime.type_defs import EncryptionConfigurationTypeDef


def get_value() -> EncryptionConfigurationTypeDef:
    return {
        "kmsKeyId": ...,
    }


# EncryptionConfigurationTypeDef definition

class EncryptionConfigurationTypeDef(TypedDict):
    kmsKeyId: str,
    kmsEncryptionContext: NotRequired[Mapping[str, str]],
```

## EventBridgeConfigurationTypeDef

```python
# EventBridgeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_data_automation_runtime.type_defs import EventBridgeConfigurationTypeDef


def get_value() -> EventBridgeConfigurationTypeDef:
    return {
        "eventBridgeEnabled": ...,
    }


# EventBridgeConfigurationTypeDef definition

class EventBridgeConfigurationTypeDef(TypedDict):
    eventBridgeEnabled: bool,
```

## GetDataAutomationStatusRequestTypeDef

```python
# GetDataAutomationStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_data_automation_runtime.type_defs import GetDataAutomationStatusRequestTypeDef


def get_value() -> GetDataAutomationStatusRequestTypeDef:
    return {
        "invocationArn": ...,
    }


# GetDataAutomationStatusRequestTypeDef definition

class GetDataAutomationStatusRequestTypeDef(TypedDict):
    invocationArn: str,
```

## OutputConfigurationTypeDef

```python
# OutputConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_data_automation_runtime.type_defs import OutputConfigurationTypeDef


def get_value() -> OutputConfigurationTypeDef:
    return {
        "s3Uri": ...,
    }


# OutputConfigurationTypeDef definition

class OutputConfigurationTypeDef(TypedDict):
    s3Uri: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_bedrock_data_automation_runtime.type_defs import ResponseMetadataTypeDef


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

## InputConfigurationTypeDef

```python
# InputConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_data_automation_runtime.type_defs import InputConfigurationTypeDef


def get_value() -> InputConfigurationTypeDef:
    return {
        "s3Uri": ...,
    }


# InputConfigurationTypeDef definition

class InputConfigurationTypeDef(TypedDict):
    s3Uri: str,
```

## NotificationConfigurationTypeDef

```python
# NotificationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_data_automation_runtime.type_defs import NotificationConfigurationTypeDef


def get_value() -> NotificationConfigurationTypeDef:
    return {
        "eventBridgeConfiguration": ...,
    }


# NotificationConfigurationTypeDef definition

class NotificationConfigurationTypeDef(TypedDict):
    eventBridgeConfiguration: EventBridgeConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: EventBridgeConfigurationTypeDef](./type_defs.md#eventbridgeconfigurationtypedef) 
## GetDataAutomationStatusResponseTypeDef

```python
# GetDataAutomationStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_data_automation_runtime.type_defs import GetDataAutomationStatusResponseTypeDef


def get_value() -> GetDataAutomationStatusResponseTypeDef:
    return {
        "status": ...,
    }


# GetDataAutomationStatusResponseTypeDef definition

class GetDataAutomationStatusResponseTypeDef(TypedDict):
    status: AutomationJobStatusType,  # (1)
    errorType: str,
    errorMessage: str,
    outputConfiguration: OutputConfigurationTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AutomationJobStatusType](./literals.md#automationjobstatustype) 
2. See [:material-code-braces: OutputConfigurationTypeDef](./type_defs.md#outputconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InvokeDataAutomationAsyncResponseTypeDef

```python
# InvokeDataAutomationAsyncResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_data_automation_runtime.type_defs import InvokeDataAutomationAsyncResponseTypeDef


def get_value() -> InvokeDataAutomationAsyncResponseTypeDef:
    return {
        "invocationArn": ...,
    }


# InvokeDataAutomationAsyncResponseTypeDef definition

class InvokeDataAutomationAsyncResponseTypeDef(TypedDict):
    invocationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InvokeDataAutomationAsyncRequestTypeDef

```python
# InvokeDataAutomationAsyncRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_data_automation_runtime.type_defs import InvokeDataAutomationAsyncRequestTypeDef


def get_value() -> InvokeDataAutomationAsyncRequestTypeDef:
    return {
        "inputConfiguration": ...,
    }


# InvokeDataAutomationAsyncRequestTypeDef definition

class InvokeDataAutomationAsyncRequestTypeDef(TypedDict):
    inputConfiguration: InputConfigurationTypeDef,  # (1)
    outputConfiguration: OutputConfigurationTypeDef,  # (2)
    clientToken: NotRequired[str],
    dataAutomationConfiguration: NotRequired[DataAutomationConfigurationTypeDef],  # (3)
    encryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (4)
    notificationConfiguration: NotRequired[NotificationConfigurationTypeDef],  # (5)
    blueprints: NotRequired[Sequence[BlueprintTypeDef]],  # (6)
```

1. See [:material-code-braces: InputConfigurationTypeDef](./type_defs.md#inputconfigurationtypedef) 
2. See [:material-code-braces: OutputConfigurationTypeDef](./type_defs.md#outputconfigurationtypedef) 
3. See [:material-code-braces: DataAutomationConfigurationTypeDef](./type_defs.md#dataautomationconfigurationtypedef) 
4. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
5. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 
6. See [:material-code-braces: BlueprintTypeDef](./type_defs.md#blueprinttypedef) 
