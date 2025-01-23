# Type definitions

> [Index](../README.md) > [RuntimeforBedrockDataAutomation](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [RuntimeforBedrockDataAutomation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation-runtime.html#runtimeforbedrockdataautomation)
    type annotations stubs module [types-aiobotocore-bedrock-data-automation-runtime](https://pypi.org/project/types-aiobotocore-bedrock-data-automation-runtime/).



## BlueprintTypeDef

```python
# BlueprintTypeDef definition

class BlueprintTypeDef(TypedDict):
    blueprintArn: str,
    version: NotRequired[str],
    stage: NotRequired[BlueprintStageType],  # (1)
```

1. See [:material-code-brackets: BlueprintStageType](./literals.md#blueprintstagetype) 
## DataAutomationConfigurationTypeDef

```python
# DataAutomationConfigurationTypeDef definition

class DataAutomationConfigurationTypeDef(TypedDict):
    dataAutomationArn: str,
    stage: NotRequired[DataAutomationStageType],  # (1)
```

1. See [:material-code-brackets: DataAutomationStageType](./literals.md#dataautomationstagetype) 
## EncryptionConfigurationTypeDef

```python
# EncryptionConfigurationTypeDef definition

class EncryptionConfigurationTypeDef(TypedDict):
    kmsKeyId: str,
    kmsEncryptionContext: NotRequired[Mapping[str, str]],
```

## EventBridgeConfigurationTypeDef

```python
# EventBridgeConfigurationTypeDef definition

class EventBridgeConfigurationTypeDef(TypedDict):
    eventBridgeEnabled: bool,
```

## GetDataAutomationStatusRequestRequestTypeDef

```python
# GetDataAutomationStatusRequestRequestTypeDef definition

class GetDataAutomationStatusRequestRequestTypeDef(TypedDict):
    invocationArn: str,
```

## OutputConfigurationTypeDef

```python
# OutputConfigurationTypeDef definition

class OutputConfigurationTypeDef(TypedDict):
    s3Uri: str,
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

## InputConfigurationTypeDef

```python
# InputConfigurationTypeDef definition

class InputConfigurationTypeDef(TypedDict):
    s3Uri: str,
```

## NotificationConfigurationTypeDef

```python
# NotificationConfigurationTypeDef definition

class NotificationConfigurationTypeDef(TypedDict):
    eventBridgeConfiguration: EventBridgeConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: EventBridgeConfigurationTypeDef](./type_defs.md#eventbridgeconfigurationtypedef) 
## GetDataAutomationStatusResponseTypeDef

```python
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
# InvokeDataAutomationAsyncResponseTypeDef definition

class InvokeDataAutomationAsyncResponseTypeDef(TypedDict):
    invocationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InvokeDataAutomationAsyncRequestRequestTypeDef

```python
# InvokeDataAutomationAsyncRequestRequestTypeDef definition

class InvokeDataAutomationAsyncRequestRequestTypeDef(TypedDict):
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
