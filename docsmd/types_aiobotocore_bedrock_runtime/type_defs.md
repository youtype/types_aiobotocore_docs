# Type definitions

> [Index](../README.md) > [BedrockRuntime](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [BedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime)
    type annotations stubs module [types-aiobotocore-bedrock-runtime](https://pypi.org/project/types-aiobotocore-bedrock-runtime/).

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


## GuardrailConverseTextBlockUnionTypeDef

```python
# GuardrailConverseTextBlockUnionTypeDef definition

GuardrailConverseTextBlockUnionTypeDef = Union[
    GuardrailConverseTextBlockTypeDef,  # (1)
    GuardrailConverseTextBlockOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: GuardrailConverseTextBlockTypeDef](./type_defs.md#guardrailconversetextblocktypedef) 
2. See [:material-code-braces: GuardrailConverseTextBlockOutputTypeDef](./type_defs.md#guardrailconversetextblockoutputtypedef) 

## ToolUseBlockUnionTypeDef

```python
# ToolUseBlockUnionTypeDef definition

ToolUseBlockUnionTypeDef = Union[
    ToolUseBlockTypeDef,  # (1)
    ToolUseBlockOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ToolUseBlockTypeDef](./type_defs.md#tooluseblocktypedef) 
2. See [:material-code-braces: ToolUseBlockOutputTypeDef](./type_defs.md#tooluseblockoutputtypedef) 

## DocumentSourceUnionTypeDef

```python
# DocumentSourceUnionTypeDef definition

DocumentSourceUnionTypeDef = Union[
    DocumentSourceTypeDef,  # (1)
    DocumentSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DocumentSourceTypeDef](./type_defs.md#documentsourcetypedef) 
2. See [:material-code-braces: DocumentSourceOutputTypeDef](./type_defs.md#documentsourceoutputtypedef) 

## ImageSourceUnionTypeDef

```python
# ImageSourceUnionTypeDef definition

ImageSourceUnionTypeDef = Union[
    ImageSourceTypeDef,  # (1)
    ImageSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ImageSourceTypeDef](./type_defs.md#imagesourcetypedef) 
2. See [:material-code-braces: ImageSourceOutputTypeDef](./type_defs.md#imagesourceoutputtypedef) 

## GuardrailConverseContentBlockUnionTypeDef

```python
# GuardrailConverseContentBlockUnionTypeDef definition

GuardrailConverseContentBlockUnionTypeDef = Union[
    GuardrailConverseContentBlockTypeDef,  # (1)
    GuardrailConverseContentBlockOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: GuardrailConverseContentBlockTypeDef](./type_defs.md#guardrailconversecontentblocktypedef) 
2. See [:material-code-braces: GuardrailConverseContentBlockOutputTypeDef](./type_defs.md#guardrailconversecontentblockoutputtypedef) 

## DocumentBlockUnionTypeDef

```python
# DocumentBlockUnionTypeDef definition

DocumentBlockUnionTypeDef = Union[
    DocumentBlockTypeDef,  # (1)
    DocumentBlockOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DocumentBlockTypeDef](./type_defs.md#documentblocktypedef) 
2. See [:material-code-braces: DocumentBlockOutputTypeDef](./type_defs.md#documentblockoutputtypedef) 

## ImageBlockUnionTypeDef

```python
# ImageBlockUnionTypeDef definition

ImageBlockUnionTypeDef = Union[
    ImageBlockTypeDef,  # (1)
    ImageBlockOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ImageBlockTypeDef](./type_defs.md#imageblocktypedef) 
2. See [:material-code-braces: ImageBlockOutputTypeDef](./type_defs.md#imageblockoutputtypedef) 

## ToolResultContentBlockUnionTypeDef

```python
# ToolResultContentBlockUnionTypeDef definition

ToolResultContentBlockUnionTypeDef = Union[
    ToolResultContentBlockTypeDef,  # (1)
    ToolResultContentBlockOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ToolResultContentBlockTypeDef](./type_defs.md#toolresultcontentblocktypedef) 
2. See [:material-code-braces: ToolResultContentBlockOutputTypeDef](./type_defs.md#toolresultcontentblockoutputtypedef) 

## ToolResultBlockUnionTypeDef

```python
# ToolResultBlockUnionTypeDef definition

ToolResultBlockUnionTypeDef = Union[
    ToolResultBlockTypeDef,  # (1)
    ToolResultBlockOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ToolResultBlockTypeDef](./type_defs.md#toolresultblocktypedef) 
2. See [:material-code-braces: ToolResultBlockOutputTypeDef](./type_defs.md#toolresultblockoutputtypedef) 

## ContentBlockUnionTypeDef

```python
# ContentBlockUnionTypeDef definition

ContentBlockUnionTypeDef = Union[
    ContentBlockTypeDef,  # (1)
    ContentBlockOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ContentBlockTypeDef](./type_defs.md#contentblocktypedef) 
2. See [:material-code-braces: ContentBlockOutputTypeDef](./type_defs.md#contentblockoutputtypedef) 

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



## GuardrailOutputContentTypeDef

```python
# GuardrailOutputContentTypeDef definition

class GuardrailOutputContentTypeDef(TypedDict):
    text: NotRequired[str],
```

## GuardrailUsageTypeDef

```python
# GuardrailUsageTypeDef definition

class GuardrailUsageTypeDef(TypedDict):
    topicPolicyUnits: int,
    contentPolicyUnits: int,
    wordPolicyUnits: int,
    sensitiveInformationPolicyUnits: int,
    sensitiveInformationPolicyFreeUnits: int,
    contextualGroundingPolicyUnits: int,
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

## ToolUseBlockDeltaTypeDef

```python
# ToolUseBlockDeltaTypeDef definition

class ToolUseBlockDeltaTypeDef(TypedDict):
    input: str,
```

## ToolUseBlockOutputTypeDef

```python
# ToolUseBlockOutputTypeDef definition

class ToolUseBlockOutputTypeDef(TypedDict):
    toolUseId: str,
    name: str,
    input: Dict[str, Any],
```

## ToolUseBlockStartTypeDef

```python
# ToolUseBlockStartTypeDef definition

class ToolUseBlockStartTypeDef(TypedDict):
    toolUseId: str,
    name: str,
```

## ContentBlockStopEventTypeDef

```python
# ContentBlockStopEventTypeDef definition

class ContentBlockStopEventTypeDef(TypedDict):
    contentBlockIndex: int,
```

## ConverseMetricsTypeDef

```python
# ConverseMetricsTypeDef definition

class ConverseMetricsTypeDef(TypedDict):
    latencyMs: int,
```

## GuardrailConfigurationTypeDef

```python
# GuardrailConfigurationTypeDef definition

class GuardrailConfigurationTypeDef(TypedDict):
    guardrailIdentifier: str,
    guardrailVersion: str,
    trace: NotRequired[GuardrailTraceType],  # (1)
```

1. See [:material-code-brackets: GuardrailTraceType](./literals.md#guardrailtracetype) 
## InferenceConfigurationTypeDef

```python
# InferenceConfigurationTypeDef definition

class InferenceConfigurationTypeDef(TypedDict):
    maxTokens: NotRequired[int],
    temperature: NotRequired[float],
    topP: NotRequired[float],
    stopSequences: NotRequired[Sequence[str]],
```

## TokenUsageTypeDef

```python
# TokenUsageTypeDef definition

class TokenUsageTypeDef(TypedDict):
    inputTokens: int,
    outputTokens: int,
    totalTokens: int,
```

## ConverseStreamMetricsTypeDef

```python
# ConverseStreamMetricsTypeDef definition

class ConverseStreamMetricsTypeDef(TypedDict):
    latencyMs: int,
```

## InternalServerExceptionTypeDef

```python
# InternalServerExceptionTypeDef definition

class InternalServerExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## MessageStartEventTypeDef

```python
# MessageStartEventTypeDef definition

class MessageStartEventTypeDef(TypedDict):
    role: ConversationRoleType,  # (1)
```

1. See [:material-code-brackets: ConversationRoleType](./literals.md#conversationroletype) 
## MessageStopEventTypeDef

```python
# MessageStopEventTypeDef definition

class MessageStopEventTypeDef(TypedDict):
    stopReason: StopReasonType,  # (1)
    additionalModelResponseFields: NotRequired[Dict[str, Any]],
```

1. See [:material-code-brackets: StopReasonType](./literals.md#stopreasontype) 
## ModelStreamErrorExceptionTypeDef

```python
# ModelStreamErrorExceptionTypeDef definition

class ModelStreamErrorExceptionTypeDef(TypedDict):
    message: NotRequired[str],
    originalStatusCode: NotRequired[int],
    originalMessage: NotRequired[str],
```

## ServiceUnavailableExceptionTypeDef

```python
# ServiceUnavailableExceptionTypeDef definition

class ServiceUnavailableExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## ThrottlingExceptionTypeDef

```python
# ThrottlingExceptionTypeDef definition

class ThrottlingExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## ValidationExceptionTypeDef

```python
# ValidationExceptionTypeDef definition

class ValidationExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## GuardrailStreamConfigurationTypeDef

```python
# GuardrailStreamConfigurationTypeDef definition

class GuardrailStreamConfigurationTypeDef(TypedDict):
    guardrailIdentifier: str,
    guardrailVersion: str,
    trace: NotRequired[GuardrailTraceType],  # (1)
    streamProcessingMode: NotRequired[GuardrailStreamProcessingModeType],  # (2)
```

1. See [:material-code-brackets: GuardrailTraceType](./literals.md#guardrailtracetype) 
2. See [:material-code-brackets: GuardrailStreamProcessingModeType](./literals.md#guardrailstreamprocessingmodetype) 
## DocumentSourceOutputTypeDef

```python
# DocumentSourceOutputTypeDef definition

class DocumentSourceOutputTypeDef(TypedDict):
    bytes: NotRequired[bytes],
```

## GuardrailTextBlockTypeDef

```python
# GuardrailTextBlockTypeDef definition

class GuardrailTextBlockTypeDef(TypedDict):
    text: str,
    qualifiers: NotRequired[Sequence[GuardrailContentQualifierType]],  # (1)
```

1. See [:material-code-brackets: GuardrailContentQualifierType](./literals.md#guardrailcontentqualifiertype) 
## GuardrailContentFilterTypeDef

```python
# GuardrailContentFilterTypeDef definition

class GuardrailContentFilterTypeDef(TypedDict):
    type: GuardrailContentFilterTypeType,  # (1)
    confidence: GuardrailContentFilterConfidenceType,  # (2)
    action: GuardrailContentPolicyActionType,  # (4)
    filterStrength: NotRequired[GuardrailContentFilterStrengthType],  # (3)
```

1. See [:material-code-brackets: GuardrailContentFilterTypeType](./literals.md#guardrailcontentfiltertypetype) 
2. See [:material-code-brackets: GuardrailContentFilterConfidenceType](./literals.md#guardrailcontentfilterconfidencetype) 
3. See [:material-code-brackets: GuardrailContentFilterStrengthType](./literals.md#guardrailcontentfilterstrengthtype) 
4. See [:material-code-brackets: GuardrailContentPolicyActionType](./literals.md#guardrailcontentpolicyactiontype) 
## GuardrailContextualGroundingFilterTypeDef

```python
# GuardrailContextualGroundingFilterTypeDef definition

class GuardrailContextualGroundingFilterTypeDef(TypedDict):
    type: GuardrailContextualGroundingFilterTypeType,  # (1)
    threshold: float,
    score: float,
    action: GuardrailContextualGroundingPolicyActionType,  # (2)
```

1. See [:material-code-brackets: GuardrailContextualGroundingFilterTypeType](./literals.md#guardrailcontextualgroundingfiltertypetype) 
2. See [:material-code-brackets: GuardrailContextualGroundingPolicyActionType](./literals.md#guardrailcontextualgroundingpolicyactiontype) 
## GuardrailConverseTextBlockOutputTypeDef

```python
# GuardrailConverseTextBlockOutputTypeDef definition

class GuardrailConverseTextBlockOutputTypeDef(TypedDict):
    text: str,
    qualifiers: NotRequired[List[GuardrailConverseContentQualifierType]],  # (1)
```

1. See [:material-code-brackets: GuardrailConverseContentQualifierType](./literals.md#guardrailconversecontentqualifiertype) 
## GuardrailConverseTextBlockTypeDef

```python
# GuardrailConverseTextBlockTypeDef definition

class GuardrailConverseTextBlockTypeDef(TypedDict):
    text: str,
    qualifiers: NotRequired[Sequence[GuardrailConverseContentQualifierType]],  # (1)
```

1. See [:material-code-brackets: GuardrailConverseContentQualifierType](./literals.md#guardrailconversecontentqualifiertype) 
## GuardrailTextCharactersCoverageTypeDef

```python
# GuardrailTextCharactersCoverageTypeDef definition

class GuardrailTextCharactersCoverageTypeDef(TypedDict):
    guarded: NotRequired[int],
    total: NotRequired[int],
```

## GuardrailCustomWordTypeDef

```python
# GuardrailCustomWordTypeDef definition

class GuardrailCustomWordTypeDef(TypedDict):
    match: str,
    action: GuardrailWordPolicyActionType,  # (1)
```

1. See [:material-code-brackets: GuardrailWordPolicyActionType](./literals.md#guardrailwordpolicyactiontype) 
## GuardrailManagedWordTypeDef

```python
# GuardrailManagedWordTypeDef definition

class GuardrailManagedWordTypeDef(TypedDict):
    match: str,
    type: GuardrailManagedWordTypeType,  # (1)
    action: GuardrailWordPolicyActionType,  # (2)
```

1. See [:material-code-brackets: GuardrailManagedWordTypeType](./literals.md#guardrailmanagedwordtypetype) 
2. See [:material-code-brackets: GuardrailWordPolicyActionType](./literals.md#guardrailwordpolicyactiontype) 
## GuardrailPiiEntityFilterTypeDef

```python
# GuardrailPiiEntityFilterTypeDef definition

class GuardrailPiiEntityFilterTypeDef(TypedDict):
    match: str,
    type: GuardrailPiiEntityTypeType,  # (1)
    action: GuardrailSensitiveInformationPolicyActionType,  # (2)
```

1. See [:material-code-brackets: GuardrailPiiEntityTypeType](./literals.md#guardrailpiientitytypetype) 
2. See [:material-code-brackets: GuardrailSensitiveInformationPolicyActionType](./literals.md#guardrailsensitiveinformationpolicyactiontype) 
## GuardrailRegexFilterTypeDef

```python
# GuardrailRegexFilterTypeDef definition

class GuardrailRegexFilterTypeDef(TypedDict):
    action: GuardrailSensitiveInformationPolicyActionType,  # (1)
    name: NotRequired[str],
    match: NotRequired[str],
    regex: NotRequired[str],
```

1. See [:material-code-brackets: GuardrailSensitiveInformationPolicyActionType](./literals.md#guardrailsensitiveinformationpolicyactiontype) 
## GuardrailTopicTypeDef

```python
# GuardrailTopicTypeDef definition

class GuardrailTopicTypeDef(TypedDict):
    name: str,
    type: GuardrailTopicTypeType,  # (1)
    action: GuardrailTopicPolicyActionType,  # (2)
```

1. See [:material-code-brackets: GuardrailTopicTypeType](./literals.md#guardrailtopictypetype) 
2. See [:material-code-brackets: GuardrailTopicPolicyActionType](./literals.md#guardrailtopicpolicyactiontype) 
## ImageSourceOutputTypeDef

```python
# ImageSourceOutputTypeDef definition

class ImageSourceOutputTypeDef(TypedDict):
    bytes: NotRequired[bytes],
```

## ModelTimeoutExceptionTypeDef

```python
# ModelTimeoutExceptionTypeDef definition

class ModelTimeoutExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## PayloadPartTypeDef

```python
# PayloadPartTypeDef definition

class PayloadPartTypeDef(TypedDict):
    bytes: NotRequired[bytes],
```

## SpecificToolChoiceTypeDef

```python
# SpecificToolChoiceTypeDef definition

class SpecificToolChoiceTypeDef(TypedDict):
    name: str,
```

## ToolInputSchemaTypeDef

```python
# ToolInputSchemaTypeDef definition

class ToolInputSchemaTypeDef(TypedDict):
    json: NotRequired[Mapping[str, Any]],
```

## ToolUseBlockTypeDef

```python
# ToolUseBlockTypeDef definition

class ToolUseBlockTypeDef(TypedDict):
    toolUseId: str,
    name: str,
    input: Mapping[str, Any],
```

## InvokeModelResponseTypeDef

```python
# InvokeModelResponseTypeDef definition

class InvokeModelResponseTypeDef(TypedDict):
    body: StreamingBody,
    contentType: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DocumentSourceTypeDef

```python
# DocumentSourceTypeDef definition

class DocumentSourceTypeDef(TypedDict):
    bytes: NotRequired[BlobTypeDef],
```

## ImageSourceTypeDef

```python
# ImageSourceTypeDef definition

class ImageSourceTypeDef(TypedDict):
    bytes: NotRequired[BlobTypeDef],
```

## InvokeModelRequestRequestTypeDef

```python
# InvokeModelRequestRequestTypeDef definition

class InvokeModelRequestRequestTypeDef(TypedDict):
    body: BlobTypeDef,
    modelId: str,
    contentType: NotRequired[str],
    accept: NotRequired[str],
    trace: NotRequired[TraceType],  # (1)
    guardrailIdentifier: NotRequired[str],
    guardrailVersion: NotRequired[str],
```

1. See [:material-code-brackets: TraceType](./literals.md#tracetype) 
## InvokeModelWithResponseStreamRequestRequestTypeDef

```python
# InvokeModelWithResponseStreamRequestRequestTypeDef definition

class InvokeModelWithResponseStreamRequestRequestTypeDef(TypedDict):
    body: BlobTypeDef,
    modelId: str,
    contentType: NotRequired[str],
    accept: NotRequired[str],
    trace: NotRequired[TraceType],  # (1)
    guardrailIdentifier: NotRequired[str],
    guardrailVersion: NotRequired[str],
```

1. See [:material-code-brackets: TraceType](./literals.md#tracetype) 
## ContentBlockDeltaTypeDef

```python
# ContentBlockDeltaTypeDef definition

class ContentBlockDeltaTypeDef(TypedDict):
    text: NotRequired[str],
    toolUse: NotRequired[ToolUseBlockDeltaTypeDef],  # (1)
```

1. See [:material-code-braces: ToolUseBlockDeltaTypeDef](./type_defs.md#tooluseblockdeltatypedef) 
## ContentBlockStartTypeDef

```python
# ContentBlockStartTypeDef definition

class ContentBlockStartTypeDef(TypedDict):
    toolUse: NotRequired[ToolUseBlockStartTypeDef],  # (1)
```

1. See [:material-code-braces: ToolUseBlockStartTypeDef](./type_defs.md#tooluseblockstarttypedef) 
## DocumentBlockOutputTypeDef

```python
# DocumentBlockOutputTypeDef definition

class DocumentBlockOutputTypeDef(TypedDict):
    format: DocumentFormatType,  # (1)
    name: str,
    source: DocumentSourceOutputTypeDef,  # (2)
```

1. See [:material-code-brackets: DocumentFormatType](./literals.md#documentformattype) 
2. See [:material-code-braces: DocumentSourceOutputTypeDef](./type_defs.md#documentsourceoutputtypedef) 
## GuardrailContentBlockTypeDef

```python
# GuardrailContentBlockTypeDef definition

class GuardrailContentBlockTypeDef(TypedDict):
    text: NotRequired[GuardrailTextBlockTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailTextBlockTypeDef](./type_defs.md#guardrailtextblocktypedef) 
## GuardrailContentPolicyAssessmentTypeDef

```python
# GuardrailContentPolicyAssessmentTypeDef definition

class GuardrailContentPolicyAssessmentTypeDef(TypedDict):
    filters: List[GuardrailContentFilterTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailContentFilterTypeDef](./type_defs.md#guardrailcontentfiltertypedef) 
## GuardrailContextualGroundingPolicyAssessmentTypeDef

```python
# GuardrailContextualGroundingPolicyAssessmentTypeDef definition

class GuardrailContextualGroundingPolicyAssessmentTypeDef(TypedDict):
    filters: NotRequired[List[GuardrailContextualGroundingFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: GuardrailContextualGroundingFilterTypeDef](./type_defs.md#guardrailcontextualgroundingfiltertypedef) 
## GuardrailConverseContentBlockOutputTypeDef

```python
# GuardrailConverseContentBlockOutputTypeDef definition

class GuardrailConverseContentBlockOutputTypeDef(TypedDict):
    text: NotRequired[GuardrailConverseTextBlockOutputTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailConverseTextBlockOutputTypeDef](./type_defs.md#guardrailconversetextblockoutputtypedef) 
## GuardrailCoverageTypeDef

```python
# GuardrailCoverageTypeDef definition

class GuardrailCoverageTypeDef(TypedDict):
    textCharacters: NotRequired[GuardrailTextCharactersCoverageTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailTextCharactersCoverageTypeDef](./type_defs.md#guardrailtextcharacterscoveragetypedef) 
## GuardrailWordPolicyAssessmentTypeDef

```python
# GuardrailWordPolicyAssessmentTypeDef definition

class GuardrailWordPolicyAssessmentTypeDef(TypedDict):
    customWords: List[GuardrailCustomWordTypeDef],  # (1)
    managedWordLists: List[GuardrailManagedWordTypeDef],  # (2)
```

1. See [:material-code-braces: GuardrailCustomWordTypeDef](./type_defs.md#guardrailcustomwordtypedef) 
2. See [:material-code-braces: GuardrailManagedWordTypeDef](./type_defs.md#guardrailmanagedwordtypedef) 
## GuardrailSensitiveInformationPolicyAssessmentTypeDef

```python
# GuardrailSensitiveInformationPolicyAssessmentTypeDef definition

class GuardrailSensitiveInformationPolicyAssessmentTypeDef(TypedDict):
    piiEntities: List[GuardrailPiiEntityFilterTypeDef],  # (1)
    regexes: List[GuardrailRegexFilterTypeDef],  # (2)
```

1. See [:material-code-braces: GuardrailPiiEntityFilterTypeDef](./type_defs.md#guardrailpiientityfiltertypedef) 
2. See [:material-code-braces: GuardrailRegexFilterTypeDef](./type_defs.md#guardrailregexfiltertypedef) 
## GuardrailTopicPolicyAssessmentTypeDef

```python
# GuardrailTopicPolicyAssessmentTypeDef definition

class GuardrailTopicPolicyAssessmentTypeDef(TypedDict):
    topics: List[GuardrailTopicTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailTopicTypeDef](./type_defs.md#guardrailtopictypedef) 
## ImageBlockOutputTypeDef

```python
# ImageBlockOutputTypeDef definition

class ImageBlockOutputTypeDef(TypedDict):
    format: ImageFormatType,  # (1)
    source: ImageSourceOutputTypeDef,  # (2)
```

1. See [:material-code-brackets: ImageFormatType](./literals.md#imageformattype) 
2. See [:material-code-braces: ImageSourceOutputTypeDef](./type_defs.md#imagesourceoutputtypedef) 
## ResponseStreamTypeDef

```python
# ResponseStreamTypeDef definition

class ResponseStreamTypeDef(TypedDict):
    chunk: NotRequired[PayloadPartTypeDef],  # (1)
    internalServerException: NotRequired[InternalServerExceptionTypeDef],  # (2)
    modelStreamErrorException: NotRequired[ModelStreamErrorExceptionTypeDef],  # (3)
    validationException: NotRequired[ValidationExceptionTypeDef],  # (4)
    throttlingException: NotRequired[ThrottlingExceptionTypeDef],  # (5)
    modelTimeoutException: NotRequired[ModelTimeoutExceptionTypeDef],  # (6)
    serviceUnavailableException: NotRequired[ServiceUnavailableExceptionTypeDef],  # (7)
```

1. See [:material-code-braces: PayloadPartTypeDef](./type_defs.md#payloadparttypedef) 
2. See [:material-code-braces: InternalServerExceptionTypeDef](./type_defs.md#internalserverexceptiontypedef) 
3. See [:material-code-braces: ModelStreamErrorExceptionTypeDef](./type_defs.md#modelstreamerrorexceptiontypedef) 
4. See [:material-code-braces: ValidationExceptionTypeDef](./type_defs.md#validationexceptiontypedef) 
5. See [:material-code-braces: ThrottlingExceptionTypeDef](./type_defs.md#throttlingexceptiontypedef) 
6. See [:material-code-braces: ModelTimeoutExceptionTypeDef](./type_defs.md#modeltimeoutexceptiontypedef) 
7. See [:material-code-braces: ServiceUnavailableExceptionTypeDef](./type_defs.md#serviceunavailableexceptiontypedef) 
## ToolChoiceTypeDef

```python
# ToolChoiceTypeDef definition

class ToolChoiceTypeDef(TypedDict):
    auto: NotRequired[Mapping[str, Any]],
    any: NotRequired[Mapping[str, Any]],
    tool: NotRequired[SpecificToolChoiceTypeDef],  # (1)
```

1. See [:material-code-braces: SpecificToolChoiceTypeDef](./type_defs.md#specifictoolchoicetypedef) 
## ToolSpecificationTypeDef

```python
# ToolSpecificationTypeDef definition

class ToolSpecificationTypeDef(TypedDict):
    name: str,
    inputSchema: ToolInputSchemaTypeDef,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: ToolInputSchemaTypeDef](./type_defs.md#toolinputschematypedef) 
## ContentBlockDeltaEventTypeDef

```python
# ContentBlockDeltaEventTypeDef definition

class ContentBlockDeltaEventTypeDef(TypedDict):
    delta: ContentBlockDeltaTypeDef,  # (1)
    contentBlockIndex: int,
```

1. See [:material-code-braces: ContentBlockDeltaTypeDef](./type_defs.md#contentblockdeltatypedef) 
## ContentBlockStartEventTypeDef

```python
# ContentBlockStartEventTypeDef definition

class ContentBlockStartEventTypeDef(TypedDict):
    start: ContentBlockStartTypeDef,  # (1)
    contentBlockIndex: int,
```

1. See [:material-code-braces: ContentBlockStartTypeDef](./type_defs.md#contentblockstarttypedef) 
## ApplyGuardrailRequestRequestTypeDef

```python
# ApplyGuardrailRequestRequestTypeDef definition

class ApplyGuardrailRequestRequestTypeDef(TypedDict):
    guardrailIdentifier: str,
    guardrailVersion: str,
    source: GuardrailContentSourceType,  # (1)
    content: Sequence[GuardrailContentBlockTypeDef],  # (2)
```

1. See [:material-code-brackets: GuardrailContentSourceType](./literals.md#guardrailcontentsourcetype) 
2. See [:material-code-braces: GuardrailContentBlockTypeDef](./type_defs.md#guardrailcontentblocktypedef) 
## GuardrailConverseContentBlockTypeDef

```python
# GuardrailConverseContentBlockTypeDef definition

class GuardrailConverseContentBlockTypeDef(TypedDict):
    text: NotRequired[GuardrailConverseTextBlockUnionTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailConverseTextBlockTypeDef](./type_defs.md#guardrailconversetextblocktypedef) [:material-code-braces: GuardrailConverseTextBlockOutputTypeDef](./type_defs.md#guardrailconversetextblockoutputtypedef) 
## GuardrailInvocationMetricsTypeDef

```python
# GuardrailInvocationMetricsTypeDef definition

class GuardrailInvocationMetricsTypeDef(TypedDict):
    guardrailProcessingLatency: NotRequired[int],
    usage: NotRequired[GuardrailUsageTypeDef],  # (1)
    guardrailCoverage: NotRequired[GuardrailCoverageTypeDef],  # (2)
```

1. See [:material-code-braces: GuardrailUsageTypeDef](./type_defs.md#guardrailusagetypedef) 
2. See [:material-code-braces: GuardrailCoverageTypeDef](./type_defs.md#guardrailcoveragetypedef) 
## ToolResultContentBlockOutputTypeDef

```python
# ToolResultContentBlockOutputTypeDef definition

class ToolResultContentBlockOutputTypeDef(TypedDict):
    json: NotRequired[Dict[str, Any]],
    text: NotRequired[str],
    image: NotRequired[ImageBlockOutputTypeDef],  # (1)
    document: NotRequired[DocumentBlockOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ImageBlockOutputTypeDef](./type_defs.md#imageblockoutputtypedef) 
2. See [:material-code-braces: DocumentBlockOutputTypeDef](./type_defs.md#documentblockoutputtypedef) 
## InvokeModelWithResponseStreamResponseTypeDef

```python
# InvokeModelWithResponseStreamResponseTypeDef definition

class InvokeModelWithResponseStreamResponseTypeDef(TypedDict):
    body: AioEventStream[ResponseStreamTypeDef],  # (1)
    contentType: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResponseStreamTypeDef](./type_defs.md#responsestreamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ToolTypeDef

```python
# ToolTypeDef definition

class ToolTypeDef(TypedDict):
    toolSpec: NotRequired[ToolSpecificationTypeDef],  # (1)
```

1. See [:material-code-braces: ToolSpecificationTypeDef](./type_defs.md#toolspecificationtypedef) 
## DocumentBlockTypeDef

```python
# DocumentBlockTypeDef definition

class DocumentBlockTypeDef(TypedDict):
    format: DocumentFormatType,  # (1)
    name: str,
    source: DocumentSourceUnionTypeDef,  # (2)
```

1. See [:material-code-brackets: DocumentFormatType](./literals.md#documentformattype) 
2. See [:material-code-braces: DocumentSourceTypeDef](./type_defs.md#documentsourcetypedef) [:material-code-braces: DocumentSourceOutputTypeDef](./type_defs.md#documentsourceoutputtypedef) 
## ImageBlockTypeDef

```python
# ImageBlockTypeDef definition

class ImageBlockTypeDef(TypedDict):
    format: ImageFormatType,  # (1)
    source: ImageSourceUnionTypeDef,  # (2)
```

1. See [:material-code-brackets: ImageFormatType](./literals.md#imageformattype) 
2. See [:material-code-braces: ImageSourceTypeDef](./type_defs.md#imagesourcetypedef) [:material-code-braces: ImageSourceOutputTypeDef](./type_defs.md#imagesourceoutputtypedef) 
## GuardrailAssessmentTypeDef

```python
# GuardrailAssessmentTypeDef definition

class GuardrailAssessmentTypeDef(TypedDict):
    topicPolicy: NotRequired[GuardrailTopicPolicyAssessmentTypeDef],  # (1)
    contentPolicy: NotRequired[GuardrailContentPolicyAssessmentTypeDef],  # (2)
    wordPolicy: NotRequired[GuardrailWordPolicyAssessmentTypeDef],  # (3)
    sensitiveInformationPolicy: NotRequired[GuardrailSensitiveInformationPolicyAssessmentTypeDef],  # (4)
    contextualGroundingPolicy: NotRequired[GuardrailContextualGroundingPolicyAssessmentTypeDef],  # (5)
    invocationMetrics: NotRequired[GuardrailInvocationMetricsTypeDef],  # (6)
```

1. See [:material-code-braces: GuardrailTopicPolicyAssessmentTypeDef](./type_defs.md#guardrailtopicpolicyassessmenttypedef) 
2. See [:material-code-braces: GuardrailContentPolicyAssessmentTypeDef](./type_defs.md#guardrailcontentpolicyassessmenttypedef) 
3. See [:material-code-braces: GuardrailWordPolicyAssessmentTypeDef](./type_defs.md#guardrailwordpolicyassessmenttypedef) 
4. See [:material-code-braces: GuardrailSensitiveInformationPolicyAssessmentTypeDef](./type_defs.md#guardrailsensitiveinformationpolicyassessmenttypedef) 
5. See [:material-code-braces: GuardrailContextualGroundingPolicyAssessmentTypeDef](./type_defs.md#guardrailcontextualgroundingpolicyassessmenttypedef) 
6. See [:material-code-braces: GuardrailInvocationMetricsTypeDef](./type_defs.md#guardrailinvocationmetricstypedef) 
## ToolResultBlockOutputTypeDef

```python
# ToolResultBlockOutputTypeDef definition

class ToolResultBlockOutputTypeDef(TypedDict):
    toolUseId: str,
    content: List[ToolResultContentBlockOutputTypeDef],  # (1)
    status: NotRequired[ToolResultStatusType],  # (2)
```

1. See [:material-code-braces: ToolResultContentBlockOutputTypeDef](./type_defs.md#toolresultcontentblockoutputtypedef) 
2. See [:material-code-brackets: ToolResultStatusType](./literals.md#toolresultstatustype) 
## ToolConfigurationTypeDef

```python
# ToolConfigurationTypeDef definition

class ToolConfigurationTypeDef(TypedDict):
    tools: Sequence[ToolTypeDef],  # (1)
    toolChoice: NotRequired[ToolChoiceTypeDef],  # (2)
```

1. See [:material-code-braces: ToolTypeDef](./type_defs.md#tooltypedef) 
2. See [:material-code-braces: ToolChoiceTypeDef](./type_defs.md#toolchoicetypedef) 
## SystemContentBlockTypeDef

```python
# SystemContentBlockTypeDef definition

class SystemContentBlockTypeDef(TypedDict):
    text: NotRequired[str],
    guardContent: NotRequired[GuardrailConverseContentBlockUnionTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailConverseContentBlockTypeDef](./type_defs.md#guardrailconversecontentblocktypedef) [:material-code-braces: GuardrailConverseContentBlockOutputTypeDef](./type_defs.md#guardrailconversecontentblockoutputtypedef) 
## ApplyGuardrailResponseTypeDef

```python
# ApplyGuardrailResponseTypeDef definition

class ApplyGuardrailResponseTypeDef(TypedDict):
    usage: GuardrailUsageTypeDef,  # (1)
    action: GuardrailActionType,  # (2)
    outputs: List[GuardrailOutputContentTypeDef],  # (3)
    assessments: List[GuardrailAssessmentTypeDef],  # (4)
    guardrailCoverage: GuardrailCoverageTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: GuardrailUsageTypeDef](./type_defs.md#guardrailusagetypedef) 
2. See [:material-code-brackets: GuardrailActionType](./literals.md#guardrailactiontype) 
3. See [:material-code-braces: GuardrailOutputContentTypeDef](./type_defs.md#guardrailoutputcontenttypedef) 
4. See [:material-code-braces: GuardrailAssessmentTypeDef](./type_defs.md#guardrailassessmenttypedef) 
5. See [:material-code-braces: GuardrailCoverageTypeDef](./type_defs.md#guardrailcoveragetypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GuardrailTraceAssessmentTypeDef

```python
# GuardrailTraceAssessmentTypeDef definition

class GuardrailTraceAssessmentTypeDef(TypedDict):
    modelOutput: NotRequired[List[str]],
    inputAssessment: NotRequired[Dict[str, GuardrailAssessmentTypeDef]],  # (1)
    outputAssessments: NotRequired[Dict[str, List[GuardrailAssessmentTypeDef]]],  # (2)
```

1. See [:material-code-braces: GuardrailAssessmentTypeDef](./type_defs.md#guardrailassessmenttypedef) 
2. See [:material-code-braces: GuardrailAssessmentTypeDef](./type_defs.md#guardrailassessmenttypedef) 
## ContentBlockOutputTypeDef

```python
# ContentBlockOutputTypeDef definition

class ContentBlockOutputTypeDef(TypedDict):
    text: NotRequired[str],
    image: NotRequired[ImageBlockOutputTypeDef],  # (1)
    document: NotRequired[DocumentBlockOutputTypeDef],  # (2)
    toolUse: NotRequired[ToolUseBlockOutputTypeDef],  # (3)
    toolResult: NotRequired[ToolResultBlockOutputTypeDef],  # (4)
    guardContent: NotRequired[GuardrailConverseContentBlockOutputTypeDef],  # (5)
```

1. See [:material-code-braces: ImageBlockOutputTypeDef](./type_defs.md#imageblockoutputtypedef) 
2. See [:material-code-braces: DocumentBlockOutputTypeDef](./type_defs.md#documentblockoutputtypedef) 
3. See [:material-code-braces: ToolUseBlockOutputTypeDef](./type_defs.md#tooluseblockoutputtypedef) 
4. See [:material-code-braces: ToolResultBlockOutputTypeDef](./type_defs.md#toolresultblockoutputtypedef) 
5. See [:material-code-braces: GuardrailConverseContentBlockOutputTypeDef](./type_defs.md#guardrailconversecontentblockoutputtypedef) 
## ToolResultContentBlockTypeDef

```python
# ToolResultContentBlockTypeDef definition

class ToolResultContentBlockTypeDef(TypedDict):
    json: NotRequired[Mapping[str, Any]],
    text: NotRequired[str],
    image: NotRequired[ImageBlockUnionTypeDef],  # (1)
    document: NotRequired[DocumentBlockUnionTypeDef],  # (2)
```

1. See [:material-code-braces: ImageBlockTypeDef](./type_defs.md#imageblocktypedef) [:material-code-braces: ImageBlockOutputTypeDef](./type_defs.md#imageblockoutputtypedef) 
2. See [:material-code-braces: DocumentBlockTypeDef](./type_defs.md#documentblocktypedef) [:material-code-braces: DocumentBlockOutputTypeDef](./type_defs.md#documentblockoutputtypedef) 
## ConverseStreamTraceTypeDef

```python
# ConverseStreamTraceTypeDef definition

class ConverseStreamTraceTypeDef(TypedDict):
    guardrail: NotRequired[GuardrailTraceAssessmentTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailTraceAssessmentTypeDef](./type_defs.md#guardrailtraceassessmenttypedef) 
## ConverseTraceTypeDef

```python
# ConverseTraceTypeDef definition

class ConverseTraceTypeDef(TypedDict):
    guardrail: NotRequired[GuardrailTraceAssessmentTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailTraceAssessmentTypeDef](./type_defs.md#guardrailtraceassessmenttypedef) 
## MessageOutputTypeDef

```python
# MessageOutputTypeDef definition

class MessageOutputTypeDef(TypedDict):
    role: ConversationRoleType,  # (1)
    content: List[ContentBlockOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: ConversationRoleType](./literals.md#conversationroletype) 
2. See [:material-code-braces: ContentBlockOutputTypeDef](./type_defs.md#contentblockoutputtypedef) 
## ConverseStreamMetadataEventTypeDef

```python
# ConverseStreamMetadataEventTypeDef definition

class ConverseStreamMetadataEventTypeDef(TypedDict):
    usage: TokenUsageTypeDef,  # (1)
    metrics: ConverseStreamMetricsTypeDef,  # (2)
    trace: NotRequired[ConverseStreamTraceTypeDef],  # (3)
```

1. See [:material-code-braces: TokenUsageTypeDef](./type_defs.md#tokenusagetypedef) 
2. See [:material-code-braces: ConverseStreamMetricsTypeDef](./type_defs.md#conversestreammetricstypedef) 
3. See [:material-code-braces: ConverseStreamTraceTypeDef](./type_defs.md#conversestreamtracetypedef) 
## ConverseOutputTypeDef

```python
# ConverseOutputTypeDef definition

class ConverseOutputTypeDef(TypedDict):
    message: NotRequired[MessageOutputTypeDef],  # (1)
```

1. See [:material-code-braces: MessageOutputTypeDef](./type_defs.md#messageoutputtypedef) 
## ToolResultBlockTypeDef

```python
# ToolResultBlockTypeDef definition

class ToolResultBlockTypeDef(TypedDict):
    toolUseId: str,
    content: Sequence[ToolResultContentBlockUnionTypeDef],  # (1)
    status: NotRequired[ToolResultStatusType],  # (2)
```

1. See [:material-code-braces: ToolResultContentBlockTypeDef](./type_defs.md#toolresultcontentblocktypedef) [:material-code-braces: ToolResultContentBlockOutputTypeDef](./type_defs.md#toolresultcontentblockoutputtypedef) 
2. See [:material-code-brackets: ToolResultStatusType](./literals.md#toolresultstatustype) 
## ConverseStreamOutputTypeDef

```python
# ConverseStreamOutputTypeDef definition

class ConverseStreamOutputTypeDef(TypedDict):
    messageStart: NotRequired[MessageStartEventTypeDef],  # (1)
    contentBlockStart: NotRequired[ContentBlockStartEventTypeDef],  # (2)
    contentBlockDelta: NotRequired[ContentBlockDeltaEventTypeDef],  # (3)
    contentBlockStop: NotRequired[ContentBlockStopEventTypeDef],  # (4)
    messageStop: NotRequired[MessageStopEventTypeDef],  # (5)
    metadata: NotRequired[ConverseStreamMetadataEventTypeDef],  # (6)
    internalServerException: NotRequired[InternalServerExceptionTypeDef],  # (7)
    modelStreamErrorException: NotRequired[ModelStreamErrorExceptionTypeDef],  # (8)
    validationException: NotRequired[ValidationExceptionTypeDef],  # (9)
    throttlingException: NotRequired[ThrottlingExceptionTypeDef],  # (10)
    serviceUnavailableException: NotRequired[ServiceUnavailableExceptionTypeDef],  # (11)
```

1. See [:material-code-braces: MessageStartEventTypeDef](./type_defs.md#messagestarteventtypedef) 
2. See [:material-code-braces: ContentBlockStartEventTypeDef](./type_defs.md#contentblockstarteventtypedef) 
3. See [:material-code-braces: ContentBlockDeltaEventTypeDef](./type_defs.md#contentblockdeltaeventtypedef) 
4. See [:material-code-braces: ContentBlockStopEventTypeDef](./type_defs.md#contentblockstopeventtypedef) 
5. See [:material-code-braces: MessageStopEventTypeDef](./type_defs.md#messagestopeventtypedef) 
6. See [:material-code-braces: ConverseStreamMetadataEventTypeDef](./type_defs.md#conversestreammetadataeventtypedef) 
7. See [:material-code-braces: InternalServerExceptionTypeDef](./type_defs.md#internalserverexceptiontypedef) 
8. See [:material-code-braces: ModelStreamErrorExceptionTypeDef](./type_defs.md#modelstreamerrorexceptiontypedef) 
9. See [:material-code-braces: ValidationExceptionTypeDef](./type_defs.md#validationexceptiontypedef) 
10. See [:material-code-braces: ThrottlingExceptionTypeDef](./type_defs.md#throttlingexceptiontypedef) 
11. See [:material-code-braces: ServiceUnavailableExceptionTypeDef](./type_defs.md#serviceunavailableexceptiontypedef) 
## ConverseResponseTypeDef

```python
# ConverseResponseTypeDef definition

class ConverseResponseTypeDef(TypedDict):
    output: ConverseOutputTypeDef,  # (1)
    stopReason: StopReasonType,  # (2)
    usage: TokenUsageTypeDef,  # (3)
    metrics: ConverseMetricsTypeDef,  # (4)
    additionalModelResponseFields: Dict[str, Any],
    trace: ConverseTraceTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: ConverseOutputTypeDef](./type_defs.md#converseoutputtypedef) 
2. See [:material-code-brackets: StopReasonType](./literals.md#stopreasontype) 
3. See [:material-code-braces: TokenUsageTypeDef](./type_defs.md#tokenusagetypedef) 
4. See [:material-code-braces: ConverseMetricsTypeDef](./type_defs.md#conversemetricstypedef) 
5. See [:material-code-braces: ConverseTraceTypeDef](./type_defs.md#conversetracetypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConverseStreamResponseTypeDef

```python
# ConverseStreamResponseTypeDef definition

class ConverseStreamResponseTypeDef(TypedDict):
    stream: AioEventStream[ConverseStreamOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConverseStreamOutputTypeDef](./type_defs.md#conversestreamoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ContentBlockTypeDef

```python
# ContentBlockTypeDef definition

class ContentBlockTypeDef(TypedDict):
    text: NotRequired[str],
    image: NotRequired[ImageBlockUnionTypeDef],  # (1)
    document: NotRequired[DocumentBlockUnionTypeDef],  # (2)
    toolUse: NotRequired[ToolUseBlockUnionTypeDef],  # (3)
    toolResult: NotRequired[ToolResultBlockUnionTypeDef],  # (4)
    guardContent: NotRequired[GuardrailConverseContentBlockUnionTypeDef],  # (5)
```

1. See [:material-code-braces: ImageBlockTypeDef](./type_defs.md#imageblocktypedef) [:material-code-braces: ImageBlockOutputTypeDef](./type_defs.md#imageblockoutputtypedef) 
2. See [:material-code-braces: DocumentBlockTypeDef](./type_defs.md#documentblocktypedef) [:material-code-braces: DocumentBlockOutputTypeDef](./type_defs.md#documentblockoutputtypedef) 
3. See [:material-code-braces: ToolUseBlockTypeDef](./type_defs.md#tooluseblocktypedef) [:material-code-braces: ToolUseBlockOutputTypeDef](./type_defs.md#tooluseblockoutputtypedef) 
4. See [:material-code-braces: ToolResultBlockTypeDef](./type_defs.md#toolresultblocktypedef) [:material-code-braces: ToolResultBlockOutputTypeDef](./type_defs.md#toolresultblockoutputtypedef) 
5. See [:material-code-braces: GuardrailConverseContentBlockTypeDef](./type_defs.md#guardrailconversecontentblocktypedef) [:material-code-braces: GuardrailConverseContentBlockOutputTypeDef](./type_defs.md#guardrailconversecontentblockoutputtypedef) 
## MessageTypeDef

```python
# MessageTypeDef definition

class MessageTypeDef(TypedDict):
    role: ConversationRoleType,  # (1)
    content: Sequence[ContentBlockUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: ConversationRoleType](./literals.md#conversationroletype) 
2. See [:material-code-braces: ContentBlockTypeDef](./type_defs.md#contentblocktypedef) [:material-code-braces: ContentBlockOutputTypeDef](./type_defs.md#contentblockoutputtypedef) 
## ConverseStreamRequestRequestTypeDef

```python
# ConverseStreamRequestRequestTypeDef definition

class ConverseStreamRequestRequestTypeDef(TypedDict):
    modelId: str,
    messages: Sequence[MessageTypeDef],  # (1)
    system: NotRequired[Sequence[SystemContentBlockTypeDef]],  # (2)
    inferenceConfig: NotRequired[InferenceConfigurationTypeDef],  # (3)
    toolConfig: NotRequired[ToolConfigurationTypeDef],  # (4)
    guardrailConfig: NotRequired[GuardrailStreamConfigurationTypeDef],  # (5)
    additionalModelRequestFields: NotRequired[Mapping[str, Any]],
    additionalModelResponseFieldPaths: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
2. See [:material-code-braces: SystemContentBlockTypeDef](./type_defs.md#systemcontentblocktypedef) 
3. See [:material-code-braces: InferenceConfigurationTypeDef](./type_defs.md#inferenceconfigurationtypedef) 
4. See [:material-code-braces: ToolConfigurationTypeDef](./type_defs.md#toolconfigurationtypedef) 
5. See [:material-code-braces: GuardrailStreamConfigurationTypeDef](./type_defs.md#guardrailstreamconfigurationtypedef) 
## ConverseRequestRequestTypeDef

```python
# ConverseRequestRequestTypeDef definition

class ConverseRequestRequestTypeDef(TypedDict):
    modelId: str,
    messages: Sequence[MessageUnionTypeDef],  # (1)
    system: NotRequired[Sequence[SystemContentBlockTypeDef]],  # (2)
    inferenceConfig: NotRequired[InferenceConfigurationTypeDef],  # (3)
    toolConfig: NotRequired[ToolConfigurationTypeDef],  # (4)
    guardrailConfig: NotRequired[GuardrailConfigurationTypeDef],  # (5)
    additionalModelRequestFields: NotRequired[Mapping[str, Any]],
    additionalModelResponseFieldPaths: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) [:material-code-braces: MessageOutputTypeDef](./type_defs.md#messageoutputtypedef) 
2. See [:material-code-braces: SystemContentBlockTypeDef](./type_defs.md#systemcontentblocktypedef) 
3. See [:material-code-braces: InferenceConfigurationTypeDef](./type_defs.md#inferenceconfigurationtypedef) 
4. See [:material-code-braces: ToolConfigurationTypeDef](./type_defs.md#toolconfigurationtypedef) 
5. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
