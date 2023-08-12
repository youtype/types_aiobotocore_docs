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
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## DialogActionTypeDef

```python
# DialogActionTypeDef definition

class DialogActionTypeDef(TypedDict):
    type: DialogActionTypeType,  # (1)
    slotToElicit: NotRequired[str],
    slotElicitationStyle: NotRequired[StyleTypeType],  # (2)
    subSlotToElicit: NotRequired[ElicitSubSlotTypeDef],  # (3)
```

1. See [:material-code-brackets: DialogActionTypeType](./literals.md#dialogactiontypetype) 
2. See [:material-code-brackets: StyleTypeType](./literals.md#styletypetype) 
3. See [:material-code-braces: ElicitSubSlotTypeDef](./type_defs.md#elicitsubslottypedef) 
## ElicitSubSlotTypeDef

```python
# ElicitSubSlotTypeDef definition

class ElicitSubSlotTypeDef(TypedDict):
    name: str,
    subSlotToElicit: NotRequired[ElicitSubSlotTypeDef],  # (1)
```

1. See [:material-code-braces: ElicitSubSlotTypeDef](./type_defs.md#elicitsubslottypedef) 
## GetSessionRequestRequestTypeDef

```python
# GetSessionRequestRequestTypeDef definition

class GetSessionRequestRequestTypeDef(TypedDict):
    botId: str,
    botAliasId: str,
    localeId: str,
    sessionId: str,
```

## IntentTypeDef

```python
# IntentTypeDef definition

class IntentTypeDef(TypedDict):
    name: str,
    slots: NotRequired[Dict[str, SlotTypeDef]],  # (1)
    state: NotRequired[IntentStateType],  # (2)
    confirmationState: NotRequired[ConfirmationStateType],  # (3)
```

1. See [:material-code-braces: SlotTypeDef](./type_defs.md#slottypedef) 
2. See [:material-code-brackets: IntentStateType](./literals.md#intentstatetype) 
3. See [:material-code-brackets: ConfirmationStateType](./literals.md#confirmationstatetype) 
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

## RuntimeHintsTypeDef

```python
# RuntimeHintsTypeDef definition

class RuntimeHintsTypeDef(TypedDict):
    slotHints: NotRequired[Dict[str, Dict[str, RuntimeHintDetailsTypeDef]]],  # (1)
```

1. See [:material-code-braces: RuntimeHintDetailsTypeDef](./type_defs.md#runtimehintdetailstypedef) 
## SentimentScoreTypeDef

```python
# SentimentScoreTypeDef definition

class SentimentScoreTypeDef(TypedDict):
    positive: NotRequired[float],
    negative: NotRequired[float],
    neutral: NotRequired[float],
    mixed: NotRequired[float],
```

## ValueTypeDef

```python
# ValueTypeDef definition

class ValueTypeDef(TypedDict):
    interpretedValue: str,
    originalValue: NotRequired[str],
    resolvedValues: NotRequired[List[str]],
```

## ActiveContextTypeDef

```python
# ActiveContextTypeDef definition

class ActiveContextTypeDef(TypedDict):
    name: str,
    timeToLive: ActiveContextTimeToLiveTypeDef,  # (1)
    contextAttributes: Dict[str, str],
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
    inputStream: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
```

## ImageResponseCardTypeDef

```python
# ImageResponseCardTypeDef definition

class ImageResponseCardTypeDef(TypedDict):
    title: str,
    subtitle: NotRequired[str],
    imageUrl: NotRequired[str],
    buttons: NotRequired[List[ButtonTypeDef]],  # (1)
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
## RuntimeHintDetailsTypeDef

```python
# RuntimeHintDetailsTypeDef definition

class RuntimeHintDetailsTypeDef(TypedDict):
    runtimeHintValues: NotRequired[List[RuntimeHintValueTypeDef]],  # (1)
    subSlotHints: NotRequired[Dict[str, RuntimeHintDetailsTypeDef]],  # (2)
```

1. See [:material-code-braces: RuntimeHintValueTypeDef](./type_defs.md#runtimehintvaluetypedef) 
2. See [:material-code-braces: RuntimeHintDetailsTypeDef](./type_defs.md#runtimehintdetailstypedef) 
## SentimentResponseTypeDef

```python
# SentimentResponseTypeDef definition

class SentimentResponseTypeDef(TypedDict):
    sentiment: NotRequired[SentimentTypeType],  # (1)
    sentimentScore: NotRequired[SentimentScoreTypeDef],  # (2)
```

1. See [:material-code-brackets: SentimentTypeType](./literals.md#sentimenttypetype) 
2. See [:material-code-braces: SentimentScoreTypeDef](./type_defs.md#sentimentscoretypedef) 
## SlotTypeDef

```python
# SlotTypeDef definition

class SlotTypeDef(TypedDict):
    value: NotRequired[ValueTypeDef],  # (1)
    shape: NotRequired[ShapeType],  # (2)
    values: NotRequired[List[SlotTypeDef]],  # (3)
    subSlots: NotRequired[Dict[str, SlotTypeDef]],  # (4)
```

1. See [:material-code-braces: ValueTypeDef](./type_defs.md#valuetypedef) 
2. See [:material-code-brackets: ShapeType](./literals.md#shapetype) 
3. See [:material-code-braces: SlotTypeDef](./type_defs.md#slottypedef) 
4. See [:material-code-braces: SlotTypeDef](./type_defs.md#slottypedef) 
## SessionStateTypeDef

```python
# SessionStateTypeDef definition

class SessionStateTypeDef(TypedDict):
    dialogAction: NotRequired[DialogActionTypeDef],  # (1)
    intent: NotRequired[IntentTypeDef],  # (2)
    activeContexts: NotRequired[List[ActiveContextTypeDef]],  # (3)
    sessionAttributes: NotRequired[Dict[str, str]],
    originatingRequestId: NotRequired[str],
    runtimeHints: NotRequired[RuntimeHintsTypeDef],  # (4)
```

1. See [:material-code-braces: DialogActionTypeDef](./type_defs.md#dialogactiontypedef) 
2. See [:material-code-braces: IntentTypeDef](./type_defs.md#intenttypedef) 
3. See [:material-code-braces: ActiveContextTypeDef](./type_defs.md#activecontexttypedef) 
4. See [:material-code-braces: RuntimeHintsTypeDef](./type_defs.md#runtimehintstypedef) 
## MessageTypeDef

```python
# MessageTypeDef definition

class MessageTypeDef(TypedDict):
    contentType: MessageContentTypeType,  # (1)
    content: NotRequired[str],
    imageResponseCard: NotRequired[ImageResponseCardTypeDef],  # (2)
```

1. See [:material-code-brackets: MessageContentTypeType](./literals.md#messagecontenttypetype) 
2. See [:material-code-braces: ImageResponseCardTypeDef](./type_defs.md#imageresponsecardtypedef) 
## InterpretationTypeDef

```python
# InterpretationTypeDef definition

class InterpretationTypeDef(TypedDict):
    nluConfidence: NotRequired[ConfidenceScoreTypeDef],  # (1)
    sentimentResponse: NotRequired[SentimentResponseTypeDef],  # (2)
    intent: NotRequired[IntentTypeDef],  # (3)
```

1. See [:material-code-braces: ConfidenceScoreTypeDef](./type_defs.md#confidencescoretypedef) 
2. See [:material-code-braces: SentimentResponseTypeDef](./type_defs.md#sentimentresponsetypedef) 
3. See [:material-code-braces: IntentTypeDef](./type_defs.md#intenttypedef) 
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
## PutSessionRequestRequestTypeDef

```python
# PutSessionRequestRequestTypeDef definition

class PutSessionRequestRequestTypeDef(TypedDict):
    botId: str,
    botAliasId: str,
    localeId: str,
    sessionId: str,
    sessionState: SessionStateTypeDef,  # (1)
    messages: NotRequired[Sequence[MessageTypeDef]],  # (2)
    requestAttributes: NotRequired[Mapping[str, str]],
    responseContentType: NotRequired[str],
```

1. See [:material-code-braces: SessionStateTypeDef](./type_defs.md#sessionstatetypedef) 
2. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
## GetSessionResponseTypeDef

```python
# GetSessionResponseTypeDef definition

class GetSessionResponseTypeDef(TypedDict):
    sessionId: str,
    messages: List[MessageTypeDef],  # (1)
    interpretations: List[InterpretationTypeDef],  # (2)
    sessionState: SessionStateTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
2. See [:material-code-braces: InterpretationTypeDef](./type_defs.md#interpretationtypedef) 
3. See [:material-code-braces: SessionStateTypeDef](./type_defs.md#sessionstatetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RecognizeTextResponseTypeDef

```python
# RecognizeTextResponseTypeDef definition

class RecognizeTextResponseTypeDef(TypedDict):
    messages: List[MessageTypeDef],  # (1)
    sessionState: SessionStateTypeDef,  # (2)
    interpretations: List[InterpretationTypeDef],  # (3)
    requestAttributes: Dict[str, str],
    sessionId: str,
    recognizedBotMember: RecognizedBotMemberTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
2. See [:material-code-braces: SessionStateTypeDef](./type_defs.md#sessionstatetypedef) 
3. See [:material-code-braces: InterpretationTypeDef](./type_defs.md#interpretationtypedef) 
4. See [:material-code-braces: RecognizedBotMemberTypeDef](./type_defs.md#recognizedbotmembertypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
