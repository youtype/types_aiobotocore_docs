# Type definitions

> [Index](../README.md) > [PinpointSMSVoice](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [PinpointSMSVoice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#pinpointsmsvoice)
    type annotations stubs module [types-aiobotocore-pinpoint-sms-voice](https://pypi.org/project/types-aiobotocore-pinpoint-sms-voice/).



## CallInstructionsMessageTypeTypeDef

```python
# CallInstructionsMessageTypeTypeDef definition

class CallInstructionsMessageTypeTypeDef(TypedDict):
    Text: NotRequired[str],
```

## CloudWatchLogsDestinationTypeDef

```python
# CloudWatchLogsDestinationTypeDef definition

class CloudWatchLogsDestinationTypeDef(TypedDict):
    IamRoleArn: NotRequired[str],
    LogGroupArn: NotRequired[str],
```

## CreateConfigurationSetRequestRequestTypeDef

```python
# CreateConfigurationSetRequestRequestTypeDef definition

class CreateConfigurationSetRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: NotRequired[str],
```

## DeleteConfigurationSetEventDestinationRequestRequestTypeDef

```python
# DeleteConfigurationSetEventDestinationRequestRequestTypeDef definition

class DeleteConfigurationSetEventDestinationRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    EventDestinationName: str,
```

## DeleteConfigurationSetRequestRequestTypeDef

```python
# DeleteConfigurationSetRequestRequestTypeDef definition

class DeleteConfigurationSetRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
```

## KinesisFirehoseDestinationTypeDef

```python
# KinesisFirehoseDestinationTypeDef definition

class KinesisFirehoseDestinationTypeDef(TypedDict):
    DeliveryStreamArn: NotRequired[str],
    IamRoleArn: NotRequired[str],
```

## SnsDestinationTypeDef

```python
# SnsDestinationTypeDef definition

class SnsDestinationTypeDef(TypedDict):
    TopicArn: NotRequired[str],
```

## GetConfigurationSetEventDestinationsRequestRequestTypeDef

```python
# GetConfigurationSetEventDestinationsRequestRequestTypeDef definition

class GetConfigurationSetEventDestinationsRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
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

## PlainTextMessageTypeTypeDef

```python
# PlainTextMessageTypeTypeDef definition

class PlainTextMessageTypeTypeDef(TypedDict):
    LanguageCode: NotRequired[str],
    Text: NotRequired[str],
    VoiceId: NotRequired[str],
```

## SSMLMessageTypeTypeDef

```python
# SSMLMessageTypeTypeDef definition

class SSMLMessageTypeTypeDef(TypedDict):
    LanguageCode: NotRequired[str],
    Text: NotRequired[str],
    VoiceId: NotRequired[str],
```

## EventDestinationDefinitionTypeDef

```python
# EventDestinationDefinitionTypeDef definition

class EventDestinationDefinitionTypeDef(TypedDict):
    CloudWatchLogsDestination: NotRequired[CloudWatchLogsDestinationTypeDef],  # (1)
    Enabled: NotRequired[bool],
    KinesisFirehoseDestination: NotRequired[KinesisFirehoseDestinationTypeDef],  # (2)
    MatchingEventTypes: NotRequired[Sequence[EventTypeType]],  # (3)
    SnsDestination: NotRequired[SnsDestinationTypeDef],  # (4)
```

1. See [:material-code-braces: CloudWatchLogsDestinationTypeDef](./type_defs.md#cloudwatchlogsdestinationtypedef) 
2. See [:material-code-braces: KinesisFirehoseDestinationTypeDef](./type_defs.md#kinesisfirehosedestinationtypedef) 
3. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
4. See [:material-code-braces: SnsDestinationTypeDef](./type_defs.md#snsdestinationtypedef) 
## EventDestinationTypeDef

```python
# EventDestinationTypeDef definition

class EventDestinationTypeDef(TypedDict):
    CloudWatchLogsDestination: NotRequired[CloudWatchLogsDestinationTypeDef],  # (1)
    Enabled: NotRequired[bool],
    KinesisFirehoseDestination: NotRequired[KinesisFirehoseDestinationTypeDef],  # (2)
    MatchingEventTypes: NotRequired[List[EventTypeType]],  # (3)
    Name: NotRequired[str],
    SnsDestination: NotRequired[SnsDestinationTypeDef],  # (4)
```

1. See [:material-code-braces: CloudWatchLogsDestinationTypeDef](./type_defs.md#cloudwatchlogsdestinationtypedef) 
2. See [:material-code-braces: KinesisFirehoseDestinationTypeDef](./type_defs.md#kinesisfirehosedestinationtypedef) 
3. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
4. See [:material-code-braces: SnsDestinationTypeDef](./type_defs.md#snsdestinationtypedef) 
## SendVoiceMessageResponseTypeDef

```python
# SendVoiceMessageResponseTypeDef definition

class SendVoiceMessageResponseTypeDef(TypedDict):
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VoiceMessageContentTypeDef

```python
# VoiceMessageContentTypeDef definition

class VoiceMessageContentTypeDef(TypedDict):
    CallInstructionsMessage: NotRequired[CallInstructionsMessageTypeTypeDef],  # (1)
    PlainTextMessage: NotRequired[PlainTextMessageTypeTypeDef],  # (2)
    SSMLMessage: NotRequired[SSMLMessageTypeTypeDef],  # (3)
```

1. See [:material-code-braces: CallInstructionsMessageTypeTypeDef](./type_defs.md#callinstructionsmessagetypetypedef) 
2. See [:material-code-braces: PlainTextMessageTypeTypeDef](./type_defs.md#plaintextmessagetypetypedef) 
3. See [:material-code-braces: SSMLMessageTypeTypeDef](./type_defs.md#ssmlmessagetypetypedef) 
## CreateConfigurationSetEventDestinationRequestRequestTypeDef

```python
# CreateConfigurationSetEventDestinationRequestRequestTypeDef definition

class CreateConfigurationSetEventDestinationRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    EventDestination: NotRequired[EventDestinationDefinitionTypeDef],  # (1)
    EventDestinationName: NotRequired[str],
```

1. See [:material-code-braces: EventDestinationDefinitionTypeDef](./type_defs.md#eventdestinationdefinitiontypedef) 
## UpdateConfigurationSetEventDestinationRequestRequestTypeDef

```python
# UpdateConfigurationSetEventDestinationRequestRequestTypeDef definition

class UpdateConfigurationSetEventDestinationRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    EventDestinationName: str,
    EventDestination: NotRequired[EventDestinationDefinitionTypeDef],  # (1)
```

1. See [:material-code-braces: EventDestinationDefinitionTypeDef](./type_defs.md#eventdestinationdefinitiontypedef) 
## GetConfigurationSetEventDestinationsResponseTypeDef

```python
# GetConfigurationSetEventDestinationsResponseTypeDef definition

class GetConfigurationSetEventDestinationsResponseTypeDef(TypedDict):
    EventDestinations: List[EventDestinationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventDestinationTypeDef](./type_defs.md#eventdestinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendVoiceMessageRequestRequestTypeDef

```python
# SendVoiceMessageRequestRequestTypeDef definition

class SendVoiceMessageRequestRequestTypeDef(TypedDict):
    CallerId: NotRequired[str],
    ConfigurationSetName: NotRequired[str],
    Content: NotRequired[VoiceMessageContentTypeDef],  # (1)
    DestinationPhoneNumber: NotRequired[str],
    OriginationPhoneNumber: NotRequired[str],
```

1. See [:material-code-braces: VoiceMessageContentTypeDef](./type_defs.md#voicemessagecontenttypedef) 
