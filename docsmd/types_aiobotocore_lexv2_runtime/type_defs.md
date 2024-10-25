# Type definitions

> [Index](../README.md) > [LexRuntimeV2](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LexRuntimeV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
    type annotations stubs module [types-aiobotocore-lexv2-runtime](https://pypi.org/project/types-aiobotocore-lexv2-runtime/).

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


## ElicitSubSlotUnionTypeDef

```python
# ElicitSubSlotUnionTypeDef definition

ElicitSubSlotUnionTypeDef = Union[
    ElicitSubSlotTypeDef,  # (1)
    ElicitSubSlotOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ElicitSubSlotTypeDef](./type_defs.md#elicitsubslottypedef) 
2. See [:material-code-braces: ElicitSubSlotOutputTypeDef](./type_defs.md#elicitsubslotoutputtypedef) 

## ValueUnionTypeDef

```python
# ValueUnionTypeDef definition

ValueUnionTypeDef = Union[
    ValueTypeDef,  # (1)
    ValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ValueTypeDef](./type_defs.md#valuetypedef) 
2. See [:material-code-braces: ValueOutputTypeDef](./type_defs.md#valueoutputtypedef) 

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

## ImageResponseCardUnionTypeDef

```python
# ImageResponseCardUnionTypeDef definition

ImageResponseCardUnionTypeDef = Union[
    ImageResponseCardTypeDef,  # (1)
    ImageResponseCardOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ImageResponseCardTypeDef](./type_defs.md#imageresponsecardtypedef) 
2. See [:material-code-braces: ImageResponseCardOutputTypeDef](./type_defs.md#imageresponsecardoutputtypedef) 

## RuntimeHintDetailsUnionTypeDef

```python
# RuntimeHintDetailsUnionTypeDef definition

RuntimeHintDetailsUnionTypeDef = Union[
    RuntimeHintDetailsTypeDef,  # (1)
    RuntimeHintDetailsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuntimeHintDetailsTypeDef](./type_defs.md#runtimehintdetailstypedef) 
2. See [:material-code-braces: RuntimeHintDetailsOutputTypeDef](./type_defs.md#runtimehintdetailsoutputtypedef) 

## DialogActionUnionTypeDef

```python
# DialogActionUnionTypeDef definition

DialogActionUnionTypeDef = Union[
    DialogActionTypeDef,  # (1)
    DialogActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DialogActionTypeDef](./type_defs.md#dialogactiontypedef) 
2. See [:material-code-braces: DialogActionOutputTypeDef](./type_defs.md#dialogactionoutputtypedef) 

## SlotUnionTypeDef

```python
# SlotUnionTypeDef definition

SlotUnionTypeDef = Union[
    SlotTypeDef,  # (1)
    SlotOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SlotTypeDef](./type_defs.md#slottypedef) 
2. See [:material-code-braces: SlotOutputTypeDef](./type_defs.md#slotoutputtypedef) 

## MessageUnionTypeDef

```python
# MessageUnionTypeDef definition

MessageUnionTypeDef = Union[
    MessageTypeDef,  # (1)
    MessageOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
2. See [:material-code-braces: MessageOutputTypeDef](./type_defs.md#messageoutputtypedef) 

## RuntimeHintsUnionTypeDef

```python
# RuntimeHintsUnionTypeDef definition

RuntimeHintsUnionTypeDef = Union[
    RuntimeHintsTypeDef,  # (1)
    RuntimeHintsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuntimeHintsTypeDef](./type_defs.md#runtimehintstypedef) 
2. See [:material-code-braces: RuntimeHintsOutputTypeDef](./type_defs.md#runtimehintsoutputtypedef) 

## IntentUnionTypeDef

```python
# IntentUnionTypeDef definition

IntentUnionTypeDef = Union[
    IntentTypeDef,  # (1)
    IntentOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IntentTypeDef](./type_defs.md#intenttypedef) 
2. See [:material-code-braces: IntentOutputTypeDef](./type_defs.md#intentoutputtypedef) 



## ActiveContextTimeToLiveTypeDef

```python
# ActiveContextTimeToLiveTypeDef definition

class ActiveContextTimeToLiveTypeDef(TypedDict):
    timeToLiveInSeconds: int,
    turnsToLive: int,
```

## ButtonTypeDef

```python
# ButtonTypeDef definition

class ButtonTypeDef(TypedDict):
    text: str,
    value: str,
```

## ConfidenceScoreTypeDef

```python
# ConfidenceScoreTypeDef definition

class ConfidenceScoreTypeDef(TypedDict):
    score: NotRequired[float],
```

## DeleteSessionRequestRequestTypeDef

```python
# DeleteSessionRequestRequestTypeDef definition

class DeleteSessionRequestRequestTypeDef(TypedDict):
    botId: str,
    botAliasId: str,
    localeId: str,
    sessionId: str,
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

## ElicitSubSlotOutputTypeDef

```python
# ElicitSubSlotOutputTypeDef definition

class ElicitSubSlotOutputTypeDef(TypedDict):
    name: str,
    subSlotToElicit: NotRequired[Dict[str, Any]],
```

## ElicitSubSlotTypeDef

```python
# ElicitSubSlotTypeDef definition

class ElicitSubSlotTypeDef(TypedDict):
    name: str,
    subSlotToElicit: NotRequired[Mapping[str, Any]],
```

## GetSessionRequestRequestTypeDef

```python
# GetSessionRequestRequestTypeDef definition

class GetSessionRequestRequestTypeDef(TypedDict):
    botId: str,
    botAliasId: str,
    localeId: str,
    sessionId: str,
```

## RecognizedBotMemberTypeDef

```python
# RecognizedBotMemberTypeDef definition

class RecognizedBotMemberTypeDef(TypedDict):
    botId: str,
    botName: NotRequired[str],
```

## RuntimeHintValueTypeDef

```python
# RuntimeHintValueTypeDef definition

class RuntimeHintValueTypeDef(TypedDict):
    phrase: str,
```

## SentimentScoreTypeDef

```python
# SentimentScoreTypeDef definition

class SentimentScoreTypeDef(TypedDict):
    positive: NotRequired[float],
    negative: NotRequired[float],
    neutral: NotRequired[float],
    mixed: NotRequired[float],
```

## ValueOutputTypeDef

```python
# ValueOutputTypeDef definition

class ValueOutputTypeDef(TypedDict):
    interpretedValue: str,
    originalValue: NotRequired[str],
    resolvedValues: NotRequired[List[str]],
```

## ValueTypeDef

```python
# ValueTypeDef definition

class ValueTypeDef(TypedDict):
    interpretedValue: str,
    originalValue: NotRequired[str],
    resolvedValues: NotRequired[Sequence[str]],
```

## ActiveContextOutputTypeDef

```python
# ActiveContextOutputTypeDef definition

class ActiveContextOutputTypeDef(TypedDict):
    name: str,
    timeToLive: ActiveContextTimeToLiveTypeDef,  # (1)
    contextAttributes: Dict[str, str],
```

1. See [:material-code-braces: ActiveContextTimeToLiveTypeDef](./type_defs.md#activecontexttimetolivetypedef) 
## ActiveContextTypeDef

```python
# ActiveContextTypeDef definition

class ActiveContextTypeDef(TypedDict):
    name: str,
    timeToLive: ActiveContextTimeToLiveTypeDef,  # (1)
    contextAttributes: Mapping[str, str],
```

1. See [:material-code-braces: ActiveContextTimeToLiveTypeDef](./type_defs.md#activecontexttimetolivetypedef) 
## RecognizeUtteranceRequestRequestTypeDef

```python
# RecognizeUtteranceRequestRequestTypeDef definition

class RecognizeUtteranceRequestRequestTypeDef(TypedDict):
    botId: str,
    botAliasId: str,
    localeId: str,
    sessionId: str,
    requestContentType: str,
    sessionState: NotRequired[str],
    requestAttributes: NotRequired[str],
    responseContentType: NotRequired[str],
    inputStream: NotRequired[BlobTypeDef],
```

## ImageResponseCardOutputTypeDef

```python
# ImageResponseCardOutputTypeDef definition

class ImageResponseCardOutputTypeDef(TypedDict):
    title: str,
    subtitle: NotRequired[str],
    imageUrl: NotRequired[str],
    buttons: NotRequired[List[ButtonTypeDef]],  # (1)
```

1. See [:material-code-braces: ButtonTypeDef](./type_defs.md#buttontypedef) 
## ImageResponseCardTypeDef

```python
# ImageResponseCardTypeDef definition

class ImageResponseCardTypeDef(TypedDict):
    title: str,
    subtitle: NotRequired[str],
    imageUrl: NotRequired[str],
    buttons: NotRequired[Sequence[ButtonTypeDef]],  # (1)
```

1. See [:material-code-braces: ButtonTypeDef](./type_defs.md#buttontypedef) 
## DeleteSessionResponseTypeDef

```python
# DeleteSessionResponseTypeDef definition

class DeleteSessionResponseTypeDef(TypedDict):
    botId: str,
    botAliasId: str,
    localeId: str,
    sessionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutSessionResponseTypeDef

```python
# PutSessionResponseTypeDef definition

class PutSessionResponseTypeDef(TypedDict):
    contentType: str,
    messages: str,
    sessionState: str,
    requestAttributes: str,
    sessionId: str,
    audioStream: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RecognizeUtteranceResponseTypeDef

```python
# RecognizeUtteranceResponseTypeDef definition

class RecognizeUtteranceResponseTypeDef(TypedDict):
    inputMode: str,
    contentType: str,
    messages: str,
    interpretations: str,
    sessionState: str,
    requestAttributes: str,
    sessionId: str,
    inputTranscript: str,
    audioStream: StreamingBody,
    recognizedBotMember: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DialogActionOutputTypeDef

```python
# DialogActionOutputTypeDef definition

class DialogActionOutputTypeDef(TypedDict):
    type: DialogActionTypeType,  # (1)
    slotToElicit: NotRequired[str],
    slotElicitationStyle: NotRequired[StyleTypeType],  # (2)
    subSlotToElicit: NotRequired[ElicitSubSlotOutputTypeDef],  # (3)
```

1. See [:material-code-brackets: DialogActionTypeType](./literals.md#dialogactiontypetype) 
2. See [:material-code-brackets: StyleTypeType](./literals.md#styletypetype) 
3. See [:material-code-braces: ElicitSubSlotOutputTypeDef](./type_defs.md#elicitsubslotoutputtypedef) 
## RuntimeHintDetailsOutputTypeDef

```python
# RuntimeHintDetailsOutputTypeDef definition

class RuntimeHintDetailsOutputTypeDef(TypedDict):
    runtimeHintValues: NotRequired[List[RuntimeHintValueTypeDef]],  # (1)
    subSlotHints: NotRequired[Dict[str, Dict[str, Any]]],
```

1. See [:material-code-braces: RuntimeHintValueTypeDef](./type_defs.md#runtimehintvaluetypedef) 
## RuntimeHintDetailsTypeDef

```python
# RuntimeHintDetailsTypeDef definition

class RuntimeHintDetailsTypeDef(TypedDict):
    runtimeHintValues: NotRequired[Sequence[RuntimeHintValueTypeDef]],  # (1)
    subSlotHints: NotRequired[Mapping[str, Mapping[str, Any]]],
```

1. See [:material-code-braces: RuntimeHintValueTypeDef](./type_defs.md#runtimehintvaluetypedef) 
## SentimentResponseTypeDef

```python
# SentimentResponseTypeDef definition

class SentimentResponseTypeDef(TypedDict):
    sentiment: NotRequired[SentimentTypeType],  # (1)
    sentimentScore: NotRequired[SentimentScoreTypeDef],  # (2)
```

1. See [:material-code-brackets: SentimentTypeType](./literals.md#sentimenttypetype) 
2. See [:material-code-braces: SentimentScoreTypeDef](./type_defs.md#sentimentscoretypedef) 
## SlotOutputTypeDef

```python
# SlotOutputTypeDef definition

class SlotOutputTypeDef(TypedDict):
    value: NotRequired[ValueOutputTypeDef],  # (1)
    shape: NotRequired[ShapeType],  # (2)
    values: NotRequired[List[Dict[str, Any]]],
    subSlots: NotRequired[Dict[str, Dict[str, Any]]],
```

1. See [:material-code-braces: ValueOutputTypeDef](./type_defs.md#valueoutputtypedef) 
2. See [:material-code-brackets: ShapeType](./literals.md#shapetype) 
## MessageOutputTypeDef

```python
# MessageOutputTypeDef definition

class MessageOutputTypeDef(TypedDict):
    contentType: MessageContentTypeType,  # (1)
    content: NotRequired[str],
    imageResponseCard: NotRequired[ImageResponseCardOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: MessageContentTypeType](./literals.md#messagecontenttypetype) 
2. See [:material-code-braces: ImageResponseCardOutputTypeDef](./type_defs.md#imageresponsecardoutputtypedef) 
## DialogActionTypeDef

```python
# DialogActionTypeDef definition

class DialogActionTypeDef(TypedDict):
    type: DialogActionTypeType,  # (1)
    slotToElicit: NotRequired[str],
    slotElicitationStyle: NotRequired[StyleTypeType],  # (2)
    subSlotToElicit: NotRequired[ElicitSubSlotUnionTypeDef],  # (3)
```

1. See [:material-code-brackets: DialogActionTypeType](./literals.md#dialogactiontypetype) 
2. See [:material-code-brackets: StyleTypeType](./literals.md#styletypetype) 
3. See [:material-code-braces: ElicitSubSlotTypeDef](./type_defs.md#elicitsubslottypedef) [:material-code-braces: ElicitSubSlotOutputTypeDef](./type_defs.md#elicitsubslotoutputtypedef) 
## RuntimeHintsOutputTypeDef

```python
# RuntimeHintsOutputTypeDef definition

class RuntimeHintsOutputTypeDef(TypedDict):
    slotHints: NotRequired[Dict[str, Dict[str, RuntimeHintDetailsOutputTypeDef]]],  # (1)
```

1. See [:material-code-braces: RuntimeHintDetailsOutputTypeDef](./type_defs.md#runtimehintdetailsoutputtypedef) 
## IntentOutputTypeDef

```python
# IntentOutputTypeDef definition

class IntentOutputTypeDef(TypedDict):
    name: str,
    slots: NotRequired[Dict[str, SlotOutputTypeDef]],  # (1)
    state: NotRequired[IntentStateType],  # (2)
    confirmationState: NotRequired[ConfirmationStateType],  # (3)
```

1. See [:material-code-braces: SlotOutputTypeDef](./type_defs.md#slotoutputtypedef) 
2. See [:material-code-brackets: IntentStateType](./literals.md#intentstatetype) 
3. See [:material-code-brackets: ConfirmationStateType](./literals.md#confirmationstatetype) 
## SlotTypeDef

```python
# SlotTypeDef definition

class SlotTypeDef(TypedDict):
    value: NotRequired[ValueUnionTypeDef],  # (1)
    shape: NotRequired[ShapeType],  # (2)
    values: NotRequired[Sequence[Mapping[str, Any]]],
    subSlots: NotRequired[Mapping[str, Mapping[str, Any]]],
```

1. See [:material-code-braces: ValueTypeDef](./type_defs.md#valuetypedef) [:material-code-braces: ValueOutputTypeDef](./type_defs.md#valueoutputtypedef) 
2. See [:material-code-brackets: ShapeType](./literals.md#shapetype) 
## MessageTypeDef

```python
# MessageTypeDef definition

class MessageTypeDef(TypedDict):
    contentType: MessageContentTypeType,  # (1)
    content: NotRequired[str],
    imageResponseCard: NotRequired[ImageResponseCardUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: MessageContentTypeType](./literals.md#messagecontenttypetype) 
2. See [:material-code-braces: ImageResponseCardTypeDef](./type_defs.md#imageresponsecardtypedef) [:material-code-braces: ImageResponseCardOutputTypeDef](./type_defs.md#imageresponsecardoutputtypedef) 
## RuntimeHintsTypeDef

```python
# RuntimeHintsTypeDef definition

class RuntimeHintsTypeDef(TypedDict):
    slotHints: NotRequired[Mapping[str, Mapping[str, RuntimeHintDetailsUnionTypeDef]]],  # (1)
```

1. See [:material-code-braces: RuntimeHintDetailsTypeDef](./type_defs.md#runtimehintdetailstypedef) [:material-code-braces: RuntimeHintDetailsOutputTypeDef](./type_defs.md#runtimehintdetailsoutputtypedef) 
## InterpretationTypeDef

```python
# InterpretationTypeDef definition

class InterpretationTypeDef(TypedDict):
    nluConfidence: NotRequired[ConfidenceScoreTypeDef],  # (1)
    sentimentResponse: NotRequired[SentimentResponseTypeDef],  # (2)
    intent: NotRequired[IntentOutputTypeDef],  # (3)
    interpretationSource: NotRequired[InterpretationSourceType],  # (4)
```

1. See [:material-code-braces: ConfidenceScoreTypeDef](./type_defs.md#confidencescoretypedef) 
2. See [:material-code-braces: SentimentResponseTypeDef](./type_defs.md#sentimentresponsetypedef) 
3. See [:material-code-braces: IntentOutputTypeDef](./type_defs.md#intentoutputtypedef) 
4. See [:material-code-brackets: InterpretationSourceType](./literals.md#interpretationsourcetype) 
## SessionStateOutputTypeDef

```python
# SessionStateOutputTypeDef definition

class SessionStateOutputTypeDef(TypedDict):
    dialogAction: NotRequired[DialogActionOutputTypeDef],  # (1)
    intent: NotRequired[IntentOutputTypeDef],  # (2)
    activeContexts: NotRequired[List[ActiveContextOutputTypeDef]],  # (3)
    sessionAttributes: NotRequired[Dict[str, str]],
    originatingRequestId: NotRequired[str],
    runtimeHints: NotRequired[RuntimeHintsOutputTypeDef],  # (4)
```

1. See [:material-code-braces: DialogActionOutputTypeDef](./type_defs.md#dialogactionoutputtypedef) 
2. See [:material-code-braces: IntentOutputTypeDef](./type_defs.md#intentoutputtypedef) 
3. See [:material-code-braces: ActiveContextOutputTypeDef](./type_defs.md#activecontextoutputtypedef) 
4. See [:material-code-braces: RuntimeHintsOutputTypeDef](./type_defs.md#runtimehintsoutputtypedef) 
## GetSessionResponseTypeDef

```python
# GetSessionResponseTypeDef definition

class GetSessionResponseTypeDef(TypedDict):
    sessionId: str,
    messages: List[MessageOutputTypeDef],  # (1)
    interpretations: List[InterpretationTypeDef],  # (2)
    sessionState: SessionStateOutputTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: MessageOutputTypeDef](./type_defs.md#messageoutputtypedef) 
2. See [:material-code-braces: InterpretationTypeDef](./type_defs.md#interpretationtypedef) 
3. See [:material-code-braces: SessionStateOutputTypeDef](./type_defs.md#sessionstateoutputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RecognizeTextResponseTypeDef

```python
# RecognizeTextResponseTypeDef definition

class RecognizeTextResponseTypeDef(TypedDict):
    messages: List[MessageOutputTypeDef],  # (1)
    sessionState: SessionStateOutputTypeDef,  # (2)
    interpretations: List[InterpretationTypeDef],  # (3)
    requestAttributes: Dict[str, str],
    sessionId: str,
    recognizedBotMember: RecognizedBotMemberTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: MessageOutputTypeDef](./type_defs.md#messageoutputtypedef) 
2. See [:material-code-braces: SessionStateOutputTypeDef](./type_defs.md#sessionstateoutputtypedef) 
3. See [:material-code-braces: InterpretationTypeDef](./type_defs.md#interpretationtypedef) 
4. See [:material-code-braces: RecognizedBotMemberTypeDef](./type_defs.md#recognizedbotmembertypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IntentTypeDef

```python
# IntentTypeDef definition

class IntentTypeDef(TypedDict):
    name: str,
    slots: NotRequired[Mapping[str, SlotUnionTypeDef]],  # (1)
    state: NotRequired[IntentStateType],  # (2)
    confirmationState: NotRequired[ConfirmationStateType],  # (3)
```

1. See [:material-code-braces: SlotTypeDef](./type_defs.md#slottypedef) [:material-code-braces: SlotOutputTypeDef](./type_defs.md#slotoutputtypedef) 
2. See [:material-code-brackets: IntentStateType](./literals.md#intentstatetype) 
3. See [:material-code-brackets: ConfirmationStateType](./literals.md#confirmationstatetype) 
## SessionStateTypeDef

```python
# SessionStateTypeDef definition

class SessionStateTypeDef(TypedDict):
    dialogAction: NotRequired[DialogActionUnionTypeDef],  # (1)
    intent: NotRequired[IntentUnionTypeDef],  # (2)
    activeContexts: NotRequired[Sequence[ActiveContextUnionTypeDef]],  # (3)
    sessionAttributes: NotRequired[Mapping[str, str]],
    originatingRequestId: NotRequired[str],
    runtimeHints: NotRequired[RuntimeHintsUnionTypeDef],  # (4)
```

1. See [:material-code-braces: DialogActionTypeDef](./type_defs.md#dialogactiontypedef) [:material-code-braces: DialogActionOutputTypeDef](./type_defs.md#dialogactionoutputtypedef) 
2. See [:material-code-braces: IntentTypeDef](./type_defs.md#intenttypedef) [:material-code-braces: IntentOutputTypeDef](./type_defs.md#intentoutputtypedef) 
3. See [:material-code-braces: ActiveContextTypeDef](./type_defs.md#activecontexttypedef) [:material-code-braces: ActiveContextOutputTypeDef](./type_defs.md#activecontextoutputtypedef) 
4. See [:material-code-braces: RuntimeHintsTypeDef](./type_defs.md#runtimehintstypedef) [:material-code-braces: RuntimeHintsOutputTypeDef](./type_defs.md#runtimehintsoutputtypedef) 
## PutSessionRequestRequestTypeDef

```python
# PutSessionRequestRequestTypeDef definition

class PutSessionRequestRequestTypeDef(TypedDict):
    botId: str,
    botAliasId: str,
    localeId: str,
    sessionId: str,
    sessionState: SessionStateTypeDef,  # (1)
    messages: NotRequired[Sequence[MessageUnionTypeDef]],  # (2)
    requestAttributes: NotRequired[Mapping[str, str]],
    responseContentType: NotRequired[str],
```

1. See [:material-code-braces: SessionStateTypeDef](./type_defs.md#sessionstatetypedef) 
2. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) [:material-code-braces: MessageOutputTypeDef](./type_defs.md#messageoutputtypedef) 
## RecognizeTextRequestRequestTypeDef

```python
# RecognizeTextRequestRequestTypeDef definition

class RecognizeTextRequestRequestTypeDef(TypedDict):
    botId: str,
    botAliasId: str,
    localeId: str,
    sessionId: str,
    text: str,
    sessionState: NotRequired[SessionStateTypeDef],  # (1)
    requestAttributes: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: SessionStateTypeDef](./type_defs.md#sessionstatetypedef) 
