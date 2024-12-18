# Type definitions

> [Index](../README.md) > [LexRuntimeService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LexRuntimeService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#lexruntimeservice)
    type annotations stubs module [types-aiobotocore-lex-runtime](https://pypi.org/project/types-aiobotocore-lex-runtime/).

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


## IntentSummaryUnionTypeDef

```python
# IntentSummaryUnionTypeDef definition

IntentSummaryUnionTypeDef = Union[
    IntentSummaryTypeDef,  # (1)
    IntentSummaryOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IntentSummaryTypeDef](./type_defs.md#intentsummarytypedef) 
2. See [:material-code-braces: IntentSummaryOutputTypeDef](./type_defs.md#intentsummaryoutputtypedef) 

## ActiveContextUnionTypeDef

```python
# ActiveContextUnionTypeDef definition

ActiveContextUnionTypeDef = Union[
    ActiveContextTypeDef,  # (1)
    ActiveContextOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ActiveContextTypeDef](./type_defs.md#activecontexttypedef) 
2. See [:material-code-braces: ActiveContextOutputTypeDef](./type_defs.md#activecontextoutputtypedef) 



## ActiveContextTimeToLiveTypeDef

```python
# ActiveContextTimeToLiveTypeDef definition

class ActiveContextTimeToLiveTypeDef(TypedDict):
    timeToLiveInSeconds: NotRequired[int],
    turnsToLive: NotRequired[int],
```

## ButtonTypeDef

```python
# ButtonTypeDef definition

class ButtonTypeDef(TypedDict):
    text: str,
    value: str,
```

## DeleteSessionRequestRequestTypeDef

```python
# DeleteSessionRequestRequestTypeDef definition

class DeleteSessionRequestRequestTypeDef(TypedDict):
    botName: str,
    botAlias: str,
    userId: str,
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

## DialogActionOutputTypeDef

```python
# DialogActionOutputTypeDef definition

class DialogActionOutputTypeDef(TypedDict):
    type: DialogActionTypeType,  # (1)
    intentName: NotRequired[str],
    slots: NotRequired[Dict[str, str]],
    slotToElicit: NotRequired[str],
    fulfillmentState: NotRequired[FulfillmentStateType],  # (2)
    message: NotRequired[str],
    messageFormat: NotRequired[MessageFormatTypeType],  # (3)
```

1. See [:material-code-brackets: DialogActionTypeType](./literals.md#dialogactiontypetype) 
2. See [:material-code-brackets: FulfillmentStateType](./literals.md#fulfillmentstatetype) 
3. See [:material-code-brackets: MessageFormatTypeType](./literals.md#messageformattypetype) 
## DialogActionTypeDef

```python
# DialogActionTypeDef definition

class DialogActionTypeDef(TypedDict):
    type: DialogActionTypeType,  # (1)
    intentName: NotRequired[str],
    slots: NotRequired[Mapping[str, str]],
    slotToElicit: NotRequired[str],
    fulfillmentState: NotRequired[FulfillmentStateType],  # (2)
    message: NotRequired[str],
    messageFormat: NotRequired[MessageFormatTypeType],  # (3)
```

1. See [:material-code-brackets: DialogActionTypeType](./literals.md#dialogactiontypetype) 
2. See [:material-code-brackets: FulfillmentStateType](./literals.md#fulfillmentstatetype) 
3. See [:material-code-brackets: MessageFormatTypeType](./literals.md#messageformattypetype) 
## GetSessionRequestRequestTypeDef

```python
# GetSessionRequestRequestTypeDef definition

class GetSessionRequestRequestTypeDef(TypedDict):
    botName: str,
    botAlias: str,
    userId: str,
    checkpointLabelFilter: NotRequired[str],
```

## IntentSummaryOutputTypeDef

```python
# IntentSummaryOutputTypeDef definition

class IntentSummaryOutputTypeDef(TypedDict):
    dialogActionType: DialogActionTypeType,  # (2)
    intentName: NotRequired[str],
    checkpointLabel: NotRequired[str],
    slots: NotRequired[Dict[str, str]],
    confirmationStatus: NotRequired[ConfirmationStatusType],  # (1)
    fulfillmentState: NotRequired[FulfillmentStateType],  # (3)
    slotToElicit: NotRequired[str],
```

1. See [:material-code-brackets: ConfirmationStatusType](./literals.md#confirmationstatustype) 
2. See [:material-code-brackets: DialogActionTypeType](./literals.md#dialogactiontypetype) 
3. See [:material-code-brackets: FulfillmentStateType](./literals.md#fulfillmentstatetype) 
## IntentConfidenceTypeDef

```python
# IntentConfidenceTypeDef definition

class IntentConfidenceTypeDef(TypedDict):
    score: NotRequired[float],
```

## IntentSummaryTypeDef

```python
# IntentSummaryTypeDef definition

class IntentSummaryTypeDef(TypedDict):
    dialogActionType: DialogActionTypeType,  # (2)
    intentName: NotRequired[str],
    checkpointLabel: NotRequired[str],
    slots: NotRequired[Mapping[str, str]],
    confirmationStatus: NotRequired[ConfirmationStatusType],  # (1)
    fulfillmentState: NotRequired[FulfillmentStateType],  # (3)
    slotToElicit: NotRequired[str],
```

1. See [:material-code-brackets: ConfirmationStatusType](./literals.md#confirmationstatustype) 
2. See [:material-code-brackets: DialogActionTypeType](./literals.md#dialogactiontypetype) 
3. See [:material-code-brackets: FulfillmentStateType](./literals.md#fulfillmentstatetype) 
## SentimentResponseTypeDef

```python
# SentimentResponseTypeDef definition

class SentimentResponseTypeDef(TypedDict):
    sentimentLabel: NotRequired[str],
    sentimentScore: NotRequired[str],
```

## ActiveContextOutputTypeDef

```python
# ActiveContextOutputTypeDef definition

class ActiveContextOutputTypeDef(TypedDict):
    name: str,
    timeToLive: ActiveContextTimeToLiveTypeDef,  # (1)
    parameters: Dict[str, str],
```

1. See [:material-code-braces: ActiveContextTimeToLiveTypeDef](./type_defs.md#activecontexttimetolivetypedef) 
## ActiveContextTypeDef

```python
# ActiveContextTypeDef definition

class ActiveContextTypeDef(TypedDict):
    name: str,
    timeToLive: ActiveContextTimeToLiveTypeDef,  # (1)
    parameters: Mapping[str, str],
```

1. See [:material-code-braces: ActiveContextTimeToLiveTypeDef](./type_defs.md#activecontexttimetolivetypedef) 
## PostContentRequestRequestTypeDef

```python
# PostContentRequestRequestTypeDef definition

class PostContentRequestRequestTypeDef(TypedDict):
    botName: str,
    botAlias: str,
    userId: str,
    contentType: str,
    inputStream: BlobTypeDef,
    sessionAttributes: NotRequired[str],
    requestAttributes: NotRequired[str],
    accept: NotRequired[str],
    activeContexts: NotRequired[str],
```

## GenericAttachmentTypeDef

```python
# GenericAttachmentTypeDef definition

class GenericAttachmentTypeDef(TypedDict):
    title: NotRequired[str],
    subTitle: NotRequired[str],
    attachmentLinkUrl: NotRequired[str],
    imageUrl: NotRequired[str],
    buttons: NotRequired[List[ButtonTypeDef]],  # (1)
```

1. See [:material-code-braces: ButtonTypeDef](./type_defs.md#buttontypedef) 
## DeleteSessionResponseTypeDef

```python
# DeleteSessionResponseTypeDef definition

class DeleteSessionResponseTypeDef(TypedDict):
    botName: str,
    botAlias: str,
    userId: str,
    sessionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PostContentResponseTypeDef

```python
# PostContentResponseTypeDef definition

class PostContentResponseTypeDef(TypedDict):
    contentType: str,
    intentName: str,
    nluIntentConfidence: str,
    alternativeIntents: str,
    slots: str,
    sessionAttributes: str,
    sentimentResponse: str,
    message: str,
    encodedMessage: str,
    messageFormat: MessageFormatTypeType,  # (1)
    dialogState: DialogStateType,  # (2)
    slotToElicit: str,
    inputTranscript: str,
    encodedInputTranscript: str,
    audioStream: StreamingBody,
    botVersion: str,
    sessionId: str,
    activeContexts: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: MessageFormatTypeType](./literals.md#messageformattypetype) 
2. See [:material-code-brackets: DialogStateType](./literals.md#dialogstatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutSessionResponseTypeDef

```python
# PutSessionResponseTypeDef definition

class PutSessionResponseTypeDef(TypedDict):
    contentType: str,
    intentName: str,
    slots: str,
    sessionAttributes: str,
    message: str,
    encodedMessage: str,
    messageFormat: MessageFormatTypeType,  # (1)
    dialogState: DialogStateType,  # (2)
    slotToElicit: str,
    audioStream: StreamingBody,
    sessionId: str,
    activeContexts: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: MessageFormatTypeType](./literals.md#messageformattypetype) 
2. See [:material-code-brackets: DialogStateType](./literals.md#dialogstatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PredictedIntentTypeDef

```python
# PredictedIntentTypeDef definition

class PredictedIntentTypeDef(TypedDict):
    intentName: NotRequired[str],
    nluIntentConfidence: NotRequired[IntentConfidenceTypeDef],  # (1)
    slots: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: IntentConfidenceTypeDef](./type_defs.md#intentconfidencetypedef) 
## GetSessionResponseTypeDef

```python
# GetSessionResponseTypeDef definition

class GetSessionResponseTypeDef(TypedDict):
    recentIntentSummaryView: List[IntentSummaryOutputTypeDef],  # (1)
    sessionAttributes: Dict[str, str],
    sessionId: str,
    dialogAction: DialogActionOutputTypeDef,  # (2)
    activeContexts: List[ActiveContextOutputTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: IntentSummaryOutputTypeDef](./type_defs.md#intentsummaryoutputtypedef) 
2. See [:material-code-braces: DialogActionOutputTypeDef](./type_defs.md#dialogactionoutputtypedef) 
3. See [:material-code-braces: ActiveContextOutputTypeDef](./type_defs.md#activecontextoutputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResponseCardTypeDef

```python
# ResponseCardTypeDef definition

class ResponseCardTypeDef(TypedDict):
    version: NotRequired[str],
    contentType: NotRequired[ContentTypeType],  # (1)
    genericAttachments: NotRequired[List[GenericAttachmentTypeDef]],  # (2)
```

1. See [:material-code-brackets: ContentTypeType](./literals.md#contenttypetype) 
2. See [:material-code-braces: GenericAttachmentTypeDef](./type_defs.md#genericattachmenttypedef) 
## PutSessionRequestRequestTypeDef

```python
# PutSessionRequestRequestTypeDef definition

class PutSessionRequestRequestTypeDef(TypedDict):
    botName: str,
    botAlias: str,
    userId: str,
    sessionAttributes: NotRequired[Mapping[str, str]],
    dialogAction: NotRequired[DialogActionTypeDef],  # (1)
    recentIntentSummaryView: NotRequired[Sequence[IntentSummaryUnionTypeDef]],  # (2)
    accept: NotRequired[str],
    activeContexts: NotRequired[Sequence[ActiveContextTypeDef]],  # (3)
```

1. See [:material-code-braces: DialogActionTypeDef](./type_defs.md#dialogactiontypedef) 
2. See [:material-code-braces: IntentSummaryTypeDef](./type_defs.md#intentsummarytypedef) [:material-code-braces: IntentSummaryOutputTypeDef](./type_defs.md#intentsummaryoutputtypedef) 
3. See [:material-code-braces: ActiveContextTypeDef](./type_defs.md#activecontexttypedef) 
## PostTextRequestRequestTypeDef

```python
# PostTextRequestRequestTypeDef definition

class PostTextRequestRequestTypeDef(TypedDict):
    botName: str,
    botAlias: str,
    userId: str,
    inputText: str,
    sessionAttributes: NotRequired[Mapping[str, str]],
    requestAttributes: NotRequired[Mapping[str, str]],
    activeContexts: NotRequired[Sequence[ActiveContextUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: ActiveContextTypeDef](./type_defs.md#activecontexttypedef) [:material-code-braces: ActiveContextOutputTypeDef](./type_defs.md#activecontextoutputtypedef) 
## PostTextResponseTypeDef

```python
# PostTextResponseTypeDef definition

class PostTextResponseTypeDef(TypedDict):
    intentName: str,
    nluIntentConfidence: IntentConfidenceTypeDef,  # (1)
    alternativeIntents: List[PredictedIntentTypeDef],  # (2)
    slots: Dict[str, str],
    sessionAttributes: Dict[str, str],
    message: str,
    sentimentResponse: SentimentResponseTypeDef,  # (3)
    messageFormat: MessageFormatTypeType,  # (4)
    dialogState: DialogStateType,  # (5)
    slotToElicit: str,
    responseCard: ResponseCardTypeDef,  # (6)
    sessionId: str,
    botVersion: str,
    activeContexts: List[ActiveContextOutputTypeDef],  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-braces: IntentConfidenceTypeDef](./type_defs.md#intentconfidencetypedef) 
2. See [:material-code-braces: PredictedIntentTypeDef](./type_defs.md#predictedintenttypedef) 
3. See [:material-code-braces: SentimentResponseTypeDef](./type_defs.md#sentimentresponsetypedef) 
4. See [:material-code-brackets: MessageFormatTypeType](./literals.md#messageformattypetype) 
5. See [:material-code-brackets: DialogStateType](./literals.md#dialogstatetype) 
6. See [:material-code-braces: ResponseCardTypeDef](./type_defs.md#responsecardtypedef) 
7. See [:material-code-braces: ActiveContextOutputTypeDef](./type_defs.md#activecontextoutputtypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
