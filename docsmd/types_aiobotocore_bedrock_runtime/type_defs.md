# Type definitions

> [Index](../README.md) > [BedrockRuntime](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [BedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#bedrockruntime)
    type annotations stubs module [types-aiobotocore-bedrock-runtime](https://pypi.org/project/types-aiobotocore-bedrock-runtime/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_bedrock_runtime.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    aiobotocore.response.StreamingBody,
]
```


## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_bedrock_runtime.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime.datetime,
    str,
]
```


## GuardrailConverseTextBlockUnionTypeDef

```python
# GuardrailConverseTextBlockUnionTypeDef Union usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailConverseTextBlockUnionTypeDef


def get_value() -> GuardrailConverseTextBlockUnionTypeDef:
    return ...


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
# ToolUseBlockUnionTypeDef Union usage example

from types_aiobotocore_bedrock_runtime.type_defs import ToolUseBlockUnionTypeDef


def get_value() -> ToolUseBlockUnionTypeDef:
    return ...


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
# DocumentSourceUnionTypeDef Union usage example

from types_aiobotocore_bedrock_runtime.type_defs import DocumentSourceUnionTypeDef


def get_value() -> DocumentSourceUnionTypeDef:
    return ...


# DocumentSourceUnionTypeDef definition

DocumentSourceUnionTypeDef = Union[
    DocumentSourceTypeDef,  # (1)
    DocumentSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DocumentSourceTypeDef](./type_defs.md#documentsourcetypedef)
2. See [:material-code-braces: DocumentSourceOutputTypeDef](./type_defs.md#documentsourceoutputtypedef)

## GuardrailConverseImageSourceUnionTypeDef

```python
# GuardrailConverseImageSourceUnionTypeDef Union usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailConverseImageSourceUnionTypeDef


def get_value() -> GuardrailConverseImageSourceUnionTypeDef:
    return ...


# GuardrailConverseImageSourceUnionTypeDef definition

GuardrailConverseImageSourceUnionTypeDef = Union[
    GuardrailConverseImageSourceTypeDef,  # (1)
    GuardrailConverseImageSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: GuardrailConverseImageSourceTypeDef](./type_defs.md#guardrailconverseimagesourcetypedef)
2. See [:material-code-braces: GuardrailConverseImageSourceOutputTypeDef](./type_defs.md#guardrailconverseimagesourceoutputtypedef)

## ImageSourceUnionTypeDef

```python
# ImageSourceUnionTypeDef Union usage example

from types_aiobotocore_bedrock_runtime.type_defs import ImageSourceUnionTypeDef


def get_value() -> ImageSourceUnionTypeDef:
    return ...


# ImageSourceUnionTypeDef definition

ImageSourceUnionTypeDef = Union[
    ImageSourceTypeDef,  # (1)
    ImageSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ImageSourceTypeDef](./type_defs.md#imagesourcetypedef)
2. See [:material-code-braces: ImageSourceOutputTypeDef](./type_defs.md#imagesourceoutputtypedef)

## ReasoningContentBlockUnionTypeDef

```python
# ReasoningContentBlockUnionTypeDef Union usage example

from types_aiobotocore_bedrock_runtime.type_defs import ReasoningContentBlockUnionTypeDef


def get_value() -> ReasoningContentBlockUnionTypeDef:
    return ...


# ReasoningContentBlockUnionTypeDef definition

ReasoningContentBlockUnionTypeDef = Union[
    ReasoningContentBlockTypeDef,  # (1)
    ReasoningContentBlockOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ReasoningContentBlockTypeDef](./type_defs.md#reasoningcontentblocktypedef)
2. See [:material-code-braces: ReasoningContentBlockOutputTypeDef](./type_defs.md#reasoningcontentblockoutputtypedef)

## VideoSourceUnionTypeDef

```python
# VideoSourceUnionTypeDef Union usage example

from types_aiobotocore_bedrock_runtime.type_defs import VideoSourceUnionTypeDef


def get_value() -> VideoSourceUnionTypeDef:
    return ...


# VideoSourceUnionTypeDef definition

VideoSourceUnionTypeDef = Union[
    VideoSourceTypeDef,  # (1)
    VideoSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: VideoSourceTypeDef](./type_defs.md#videosourcetypedef)
2. See [:material-code-braces: VideoSourceOutputTypeDef](./type_defs.md#videosourceoutputtypedef)

## DocumentBlockUnionTypeDef

```python
# DocumentBlockUnionTypeDef Union usage example

from types_aiobotocore_bedrock_runtime.type_defs import DocumentBlockUnionTypeDef


def get_value() -> DocumentBlockUnionTypeDef:
    return ...


# DocumentBlockUnionTypeDef definition

DocumentBlockUnionTypeDef = Union[
    DocumentBlockTypeDef,  # (1)
    DocumentBlockOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DocumentBlockTypeDef](./type_defs.md#documentblocktypedef)
2. See [:material-code-braces: DocumentBlockOutputTypeDef](./type_defs.md#documentblockoutputtypedef)

## GuardrailConverseImageBlockUnionTypeDef

```python
# GuardrailConverseImageBlockUnionTypeDef Union usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailConverseImageBlockUnionTypeDef


def get_value() -> GuardrailConverseImageBlockUnionTypeDef:
    return ...


# GuardrailConverseImageBlockUnionTypeDef definition

GuardrailConverseImageBlockUnionTypeDef = Union[
    GuardrailConverseImageBlockTypeDef,  # (1)
    GuardrailConverseImageBlockOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: GuardrailConverseImageBlockTypeDef](./type_defs.md#guardrailconverseimageblocktypedef)
2. See [:material-code-braces: GuardrailConverseImageBlockOutputTypeDef](./type_defs.md#guardrailconverseimageblockoutputtypedef)

## ImageBlockUnionTypeDef

```python
# ImageBlockUnionTypeDef Union usage example

from types_aiobotocore_bedrock_runtime.type_defs import ImageBlockUnionTypeDef


def get_value() -> ImageBlockUnionTypeDef:
    return ...


# ImageBlockUnionTypeDef definition

ImageBlockUnionTypeDef = Union[
    ImageBlockTypeDef,  # (1)
    ImageBlockOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ImageBlockTypeDef](./type_defs.md#imageblocktypedef)
2. See [:material-code-braces: ImageBlockOutputTypeDef](./type_defs.md#imageblockoutputtypedef)

## VideoBlockUnionTypeDef

```python
# VideoBlockUnionTypeDef Union usage example

from types_aiobotocore_bedrock_runtime.type_defs import VideoBlockUnionTypeDef


def get_value() -> VideoBlockUnionTypeDef:
    return ...


# VideoBlockUnionTypeDef definition

VideoBlockUnionTypeDef = Union[
    VideoBlockTypeDef,  # (1)
    VideoBlockOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: VideoBlockTypeDef](./type_defs.md#videoblocktypedef)
2. See [:material-code-braces: VideoBlockOutputTypeDef](./type_defs.md#videoblockoutputtypedef)

## GuardrailConverseContentBlockUnionTypeDef

```python
# GuardrailConverseContentBlockUnionTypeDef Union usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailConverseContentBlockUnionTypeDef


def get_value() -> GuardrailConverseContentBlockUnionTypeDef:
    return ...


# GuardrailConverseContentBlockUnionTypeDef definition

GuardrailConverseContentBlockUnionTypeDef = Union[
    GuardrailConverseContentBlockTypeDef,  # (1)
    GuardrailConverseContentBlockOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: GuardrailConverseContentBlockTypeDef](./type_defs.md#guardrailconversecontentblocktypedef)
2. See [:material-code-braces: GuardrailConverseContentBlockOutputTypeDef](./type_defs.md#guardrailconversecontentblockoutputtypedef)

## ToolResultContentBlockUnionTypeDef

```python
# ToolResultContentBlockUnionTypeDef Union usage example

from types_aiobotocore_bedrock_runtime.type_defs import ToolResultContentBlockUnionTypeDef


def get_value() -> ToolResultContentBlockUnionTypeDef:
    return ...


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
# ToolResultBlockUnionTypeDef Union usage example

from types_aiobotocore_bedrock_runtime.type_defs import ToolResultBlockUnionTypeDef


def get_value() -> ToolResultBlockUnionTypeDef:
    return ...


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
# ContentBlockUnionTypeDef Union usage example

from types_aiobotocore_bedrock_runtime.type_defs import ContentBlockUnionTypeDef


def get_value() -> ContentBlockUnionTypeDef:
    return ...


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
# MessageUnionTypeDef Union usage example

from types_aiobotocore_bedrock_runtime.type_defs import MessageUnionTypeDef


def get_value() -> MessageUnionTypeDef:
    return ...


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
# GuardrailOutputContentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailOutputContentTypeDef


def get_value() -> GuardrailOutputContentTypeDef:
    return {
        "text": ...,
    }


# GuardrailOutputContentTypeDef definition

class GuardrailOutputContentTypeDef(TypedDict):
    text: NotRequired[str],
```


## GuardrailUsageTypeDef

```python
# GuardrailUsageTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailUsageTypeDef


def get_value() -> GuardrailUsageTypeDef:
    return {
        "topicPolicyUnits": ...,
    }


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
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ResponseMetadataTypeDef


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


## AsyncInvokeS3OutputDataConfigTypeDef

```python
# AsyncInvokeS3OutputDataConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import AsyncInvokeS3OutputDataConfigTypeDef


def get_value() -> AsyncInvokeS3OutputDataConfigTypeDef:
    return {
        "s3Uri": ...,
    }


# AsyncInvokeS3OutputDataConfigTypeDef definition

class AsyncInvokeS3OutputDataConfigTypeDef(TypedDict):
    s3Uri: str,
    kmsKeyId: NotRequired[str],
    bucketOwner: NotRequired[str],
```


## ReasoningContentBlockDeltaTypeDef

```python
# ReasoningContentBlockDeltaTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ReasoningContentBlockDeltaTypeDef


def get_value() -> ReasoningContentBlockDeltaTypeDef:
    return {
        "text": ...,
    }


# ReasoningContentBlockDeltaTypeDef definition

class ReasoningContentBlockDeltaTypeDef(TypedDict):
    text: NotRequired[str],
    redactedContent: NotRequired[bytes],
    signature: NotRequired[str],
```


## ToolUseBlockDeltaTypeDef

```python
# ToolUseBlockDeltaTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ToolUseBlockDeltaTypeDef


def get_value() -> ToolUseBlockDeltaTypeDef:
    return {
        "input": ...,
    }


# ToolUseBlockDeltaTypeDef definition

class ToolUseBlockDeltaTypeDef(TypedDict):
    input: str,
```


## ToolUseBlockOutputTypeDef

```python
# ToolUseBlockOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ToolUseBlockOutputTypeDef


def get_value() -> ToolUseBlockOutputTypeDef:
    return {
        "toolUseId": ...,
    }


# ToolUseBlockOutputTypeDef definition

class ToolUseBlockOutputTypeDef(TypedDict):
    toolUseId: str,
    name: str,
    input: Dict[str, Any],
```


## ToolUseBlockStartTypeDef

```python
# ToolUseBlockStartTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ToolUseBlockStartTypeDef


def get_value() -> ToolUseBlockStartTypeDef:
    return {
        "toolUseId": ...,
    }


# ToolUseBlockStartTypeDef definition

class ToolUseBlockStartTypeDef(TypedDict):
    toolUseId: str,
    name: str,
```


## ContentBlockStopEventTypeDef

```python
# ContentBlockStopEventTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ContentBlockStopEventTypeDef


def get_value() -> ContentBlockStopEventTypeDef:
    return {
        "contentBlockIndex": ...,
    }


# ContentBlockStopEventTypeDef definition

class ContentBlockStopEventTypeDef(TypedDict):
    contentBlockIndex: int,
```


## ConverseMetricsTypeDef

```python
# ConverseMetricsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ConverseMetricsTypeDef


def get_value() -> ConverseMetricsTypeDef:
    return {
        "latencyMs": ...,
    }


# ConverseMetricsTypeDef definition

class ConverseMetricsTypeDef(TypedDict):
    latencyMs: int,
```


## GuardrailConfigurationTypeDef

```python
# GuardrailConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailConfigurationTypeDef


def get_value() -> GuardrailConfigurationTypeDef:
    return {
        "guardrailIdentifier": ...,
    }


# GuardrailConfigurationTypeDef definition

class GuardrailConfigurationTypeDef(TypedDict):
    guardrailIdentifier: str,
    guardrailVersion: str,
    trace: NotRequired[GuardrailTraceType],  # (1)
```

1. See [:material-code-brackets: GuardrailTraceType](./literals.md#guardrailtracetype)

## InferenceConfigurationTypeDef

```python
# InferenceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import InferenceConfigurationTypeDef


def get_value() -> InferenceConfigurationTypeDef:
    return {
        "maxTokens": ...,
    }


# InferenceConfigurationTypeDef definition

class InferenceConfigurationTypeDef(TypedDict):
    maxTokens: NotRequired[int],
    temperature: NotRequired[float],
    topP: NotRequired[float],
    stopSequences: NotRequired[Sequence[str]],
```


## PerformanceConfigurationTypeDef

```python
# PerformanceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import PerformanceConfigurationTypeDef


def get_value() -> PerformanceConfigurationTypeDef:
    return {
        "latency": ...,
    }


# PerformanceConfigurationTypeDef definition

class PerformanceConfigurationTypeDef(TypedDict):
    latency: NotRequired[PerformanceConfigLatencyType],  # (1)
```

1. See [:material-code-brackets: PerformanceConfigLatencyType](./literals.md#performanceconfiglatencytype)

## PromptVariableValuesTypeDef

```python
# PromptVariableValuesTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import PromptVariableValuesTypeDef


def get_value() -> PromptVariableValuesTypeDef:
    return {
        "text": ...,
    }


# PromptVariableValuesTypeDef definition

class PromptVariableValuesTypeDef(TypedDict):
    text: NotRequired[str],
```


## TokenUsageTypeDef

```python
# TokenUsageTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import TokenUsageTypeDef


def get_value() -> TokenUsageTypeDef:
    return {
        "inputTokens": ...,
    }


# TokenUsageTypeDef definition

class TokenUsageTypeDef(TypedDict):
    inputTokens: int,
    outputTokens: int,
    totalTokens: int,
```


## ConverseStreamMetricsTypeDef

```python
# ConverseStreamMetricsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ConverseStreamMetricsTypeDef


def get_value() -> ConverseStreamMetricsTypeDef:
    return {
        "latencyMs": ...,
    }


# ConverseStreamMetricsTypeDef definition

class ConverseStreamMetricsTypeDef(TypedDict):
    latencyMs: int,
```


## InternalServerExceptionTypeDef

```python
# InternalServerExceptionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import InternalServerExceptionTypeDef


def get_value() -> InternalServerExceptionTypeDef:
    return {
        "message": ...,
    }


# InternalServerExceptionTypeDef definition

class InternalServerExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```


## MessageStartEventTypeDef

```python
# MessageStartEventTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import MessageStartEventTypeDef


def get_value() -> MessageStartEventTypeDef:
    return {
        "role": ...,
    }


# MessageStartEventTypeDef definition

class MessageStartEventTypeDef(TypedDict):
    role: ConversationRoleType,  # (1)
```

1. See [:material-code-brackets: ConversationRoleType](./literals.md#conversationroletype)

## MessageStopEventTypeDef

```python
# MessageStopEventTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import MessageStopEventTypeDef


def get_value() -> MessageStopEventTypeDef:
    return {
        "stopReason": ...,
    }


# MessageStopEventTypeDef definition

class MessageStopEventTypeDef(TypedDict):
    stopReason: StopReasonType,  # (1)
    additionalModelResponseFields: NotRequired[Dict[str, Any]],
```

1. See [:material-code-brackets: StopReasonType](./literals.md#stopreasontype)

## ModelStreamErrorExceptionTypeDef

```python
# ModelStreamErrorExceptionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ModelStreamErrorExceptionTypeDef


def get_value() -> ModelStreamErrorExceptionTypeDef:
    return {
        "message": ...,
    }


# ModelStreamErrorExceptionTypeDef definition

class ModelStreamErrorExceptionTypeDef(TypedDict):
    message: NotRequired[str],
    originalStatusCode: NotRequired[int],
    originalMessage: NotRequired[str],
```


## ServiceUnavailableExceptionTypeDef

```python
# ServiceUnavailableExceptionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ServiceUnavailableExceptionTypeDef


def get_value() -> ServiceUnavailableExceptionTypeDef:
    return {
        "message": ...,
    }


# ServiceUnavailableExceptionTypeDef definition

class ServiceUnavailableExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```


## ThrottlingExceptionTypeDef

```python
# ThrottlingExceptionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ThrottlingExceptionTypeDef


def get_value() -> ThrottlingExceptionTypeDef:
    return {
        "message": ...,
    }


# ThrottlingExceptionTypeDef definition

class ThrottlingExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```


## ValidationExceptionTypeDef

```python
# ValidationExceptionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ValidationExceptionTypeDef


def get_value() -> ValidationExceptionTypeDef:
    return {
        "message": ...,
    }


# ValidationExceptionTypeDef definition

class ValidationExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```


## GuardrailStreamConfigurationTypeDef

```python
# GuardrailStreamConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailStreamConfigurationTypeDef


def get_value() -> GuardrailStreamConfigurationTypeDef:
    return {
        "guardrailIdentifier": ...,
    }


# GuardrailStreamConfigurationTypeDef definition

class GuardrailStreamConfigurationTypeDef(TypedDict):
    guardrailIdentifier: str,
    guardrailVersion: str,
    trace: NotRequired[GuardrailTraceType],  # (1)
    streamProcessingMode: NotRequired[GuardrailStreamProcessingModeType],  # (2)
```

1. See [:material-code-brackets: GuardrailTraceType](./literals.md#guardrailtracetype)
2. See [:material-code-brackets: GuardrailStreamProcessingModeType](./literals.md#guardrailstreamprocessingmodetype)

## PromptRouterTraceTypeDef

```python
# PromptRouterTraceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import PromptRouterTraceTypeDef


def get_value() -> PromptRouterTraceTypeDef:
    return {
        "invokedModelId": ...,
    }


# PromptRouterTraceTypeDef definition

class PromptRouterTraceTypeDef(TypedDict):
    invokedModelId: NotRequired[str],
```


## DocumentSourceOutputTypeDef

```python
# DocumentSourceOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import DocumentSourceOutputTypeDef


def get_value() -> DocumentSourceOutputTypeDef:
    return {
        "bytes": ...,
    }


# DocumentSourceOutputTypeDef definition

class DocumentSourceOutputTypeDef(TypedDict):
    bytes: NotRequired[bytes],
```


## GetAsyncInvokeRequestTypeDef

```python
# GetAsyncInvokeRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GetAsyncInvokeRequestTypeDef


def get_value() -> GetAsyncInvokeRequestTypeDef:
    return {
        "invocationArn": ...,
    }


# GetAsyncInvokeRequestTypeDef definition

class GetAsyncInvokeRequestTypeDef(TypedDict):
    invocationArn: str,
```


## GuardrailTextBlockTypeDef

```python
# GuardrailTextBlockTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailTextBlockTypeDef


def get_value() -> GuardrailTextBlockTypeDef:
    return {
        "text": ...,
    }


# GuardrailTextBlockTypeDef definition

class GuardrailTextBlockTypeDef(TypedDict):
    text: str,
    qualifiers: NotRequired[Sequence[GuardrailContentQualifierType]],  # (1)
```

1. See `Sequence[GuardrailContentQualifierType]`

## GuardrailContentFilterTypeDef

```python
# GuardrailContentFilterTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailContentFilterTypeDef


def get_value() -> GuardrailContentFilterTypeDef:
    return {
        "type": ...,
    }


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
# GuardrailContextualGroundingFilterTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailContextualGroundingFilterTypeDef


def get_value() -> GuardrailContextualGroundingFilterTypeDef:
    return {
        "type": ...,
    }


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
# GuardrailConverseTextBlockOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailConverseTextBlockOutputTypeDef


def get_value() -> GuardrailConverseTextBlockOutputTypeDef:
    return {
        "text": ...,
    }


# GuardrailConverseTextBlockOutputTypeDef definition

class GuardrailConverseTextBlockOutputTypeDef(TypedDict):
    text: str,
    qualifiers: NotRequired[List[GuardrailConverseContentQualifierType]],  # (1)
```

1. See `List[GuardrailConverseContentQualifierType]`

## GuardrailConverseImageSourceOutputTypeDef

```python
# GuardrailConverseImageSourceOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailConverseImageSourceOutputTypeDef


def get_value() -> GuardrailConverseImageSourceOutputTypeDef:
    return {
        "bytes": ...,
    }


# GuardrailConverseImageSourceOutputTypeDef definition

class GuardrailConverseImageSourceOutputTypeDef(TypedDict):
    bytes: NotRequired[bytes],
```


## GuardrailConverseTextBlockTypeDef

```python
# GuardrailConverseTextBlockTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailConverseTextBlockTypeDef


def get_value() -> GuardrailConverseTextBlockTypeDef:
    return {
        "text": ...,
    }


# GuardrailConverseTextBlockTypeDef definition

class GuardrailConverseTextBlockTypeDef(TypedDict):
    text: str,
    qualifiers: NotRequired[Sequence[GuardrailConverseContentQualifierType]],  # (1)
```

1. See `Sequence[GuardrailConverseContentQualifierType]`

## GuardrailImageCoverageTypeDef

```python
# GuardrailImageCoverageTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailImageCoverageTypeDef


def get_value() -> GuardrailImageCoverageTypeDef:
    return {
        "guarded": ...,
    }


# GuardrailImageCoverageTypeDef definition

class GuardrailImageCoverageTypeDef(TypedDict):
    guarded: NotRequired[int],
    total: NotRequired[int],
```


## GuardrailTextCharactersCoverageTypeDef

```python
# GuardrailTextCharactersCoverageTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailTextCharactersCoverageTypeDef


def get_value() -> GuardrailTextCharactersCoverageTypeDef:
    return {
        "guarded": ...,
    }


# GuardrailTextCharactersCoverageTypeDef definition

class GuardrailTextCharactersCoverageTypeDef(TypedDict):
    guarded: NotRequired[int],
    total: NotRequired[int],
```


## GuardrailCustomWordTypeDef

```python
# GuardrailCustomWordTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailCustomWordTypeDef


def get_value() -> GuardrailCustomWordTypeDef:
    return {
        "match": ...,
    }


# GuardrailCustomWordTypeDef definition

class GuardrailCustomWordTypeDef(TypedDict):
    match: str,
    action: GuardrailWordPolicyActionType,  # (1)
```

1. See [:material-code-brackets: GuardrailWordPolicyActionType](./literals.md#guardrailwordpolicyactiontype)

## GuardrailManagedWordTypeDef

```python
# GuardrailManagedWordTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailManagedWordTypeDef


def get_value() -> GuardrailManagedWordTypeDef:
    return {
        "match": ...,
    }


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
# GuardrailPiiEntityFilterTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailPiiEntityFilterTypeDef


def get_value() -> GuardrailPiiEntityFilterTypeDef:
    return {
        "match": ...,
    }


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
# GuardrailRegexFilterTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailRegexFilterTypeDef


def get_value() -> GuardrailRegexFilterTypeDef:
    return {
        "name": ...,
    }


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
# GuardrailTopicTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailTopicTypeDef


def get_value() -> GuardrailTopicTypeDef:
    return {
        "name": ...,
    }


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
# ImageSourceOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ImageSourceOutputTypeDef


def get_value() -> ImageSourceOutputTypeDef:
    return {
        "bytes": ...,
    }


# ImageSourceOutputTypeDef definition

class ImageSourceOutputTypeDef(TypedDict):
    bytes: NotRequired[bytes],
```


## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```


## ModelTimeoutExceptionTypeDef

```python
# ModelTimeoutExceptionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ModelTimeoutExceptionTypeDef


def get_value() -> ModelTimeoutExceptionTypeDef:
    return {
        "message": ...,
    }


# ModelTimeoutExceptionTypeDef definition

class ModelTimeoutExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```


## PayloadPartTypeDef

```python
# PayloadPartTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import PayloadPartTypeDef


def get_value() -> PayloadPartTypeDef:
    return {
        "bytes": ...,
    }


# PayloadPartTypeDef definition

class PayloadPartTypeDef(TypedDict):
    bytes: NotRequired[bytes],
```


## ReasoningTextBlockTypeDef

```python
# ReasoningTextBlockTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ReasoningTextBlockTypeDef


def get_value() -> ReasoningTextBlockTypeDef:
    return {
        "text": ...,
    }


# ReasoningTextBlockTypeDef definition

class ReasoningTextBlockTypeDef(TypedDict):
    text: str,
    signature: NotRequired[str],
```


## S3LocationTypeDef

```python
# S3LocationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import S3LocationTypeDef


def get_value() -> S3LocationTypeDef:
    return {
        "uri": ...,
    }


# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    uri: str,
    bucketOwner: NotRequired[str],
```


## SpecificToolChoiceTypeDef

```python
# SpecificToolChoiceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import SpecificToolChoiceTypeDef


def get_value() -> SpecificToolChoiceTypeDef:
    return {
        "name": ...,
    }


# SpecificToolChoiceTypeDef definition

class SpecificToolChoiceTypeDef(TypedDict):
    name: str,
```


## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
```


## ToolInputSchemaTypeDef

```python
# ToolInputSchemaTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ToolInputSchemaTypeDef


def get_value() -> ToolInputSchemaTypeDef:
    return {
        "json": ...,
    }


# ToolInputSchemaTypeDef definition

class ToolInputSchemaTypeDef(TypedDict):
    json: NotRequired[Mapping[str, Any]],
```


## ToolUseBlockTypeDef

```python
# ToolUseBlockTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ToolUseBlockTypeDef


def get_value() -> ToolUseBlockTypeDef:
    return {
        "toolUseId": ...,
    }


# ToolUseBlockTypeDef definition

class ToolUseBlockTypeDef(TypedDict):
    toolUseId: str,
    name: str,
    input: Mapping[str, Any],
```


## InvokeModelResponseTypeDef

```python
# InvokeModelResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import InvokeModelResponseTypeDef


def get_value() -> InvokeModelResponseTypeDef:
    return {
        "body": ...,
    }


# InvokeModelResponseTypeDef definition

class InvokeModelResponseTypeDef(TypedDict):
    body: aiobotocore.response.StreamingBody,
    contentType: str,
    performanceConfigLatency: PerformanceConfigLatencyType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: PerformanceConfigLatencyType](./literals.md#performanceconfiglatencytype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## StartAsyncInvokeResponseTypeDef

```python
# StartAsyncInvokeResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import StartAsyncInvokeResponseTypeDef


def get_value() -> StartAsyncInvokeResponseTypeDef:
    return {
        "invocationArn": ...,
    }


# StartAsyncInvokeResponseTypeDef definition

class StartAsyncInvokeResponseTypeDef(TypedDict):
    invocationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## AsyncInvokeOutputDataConfigTypeDef

```python
# AsyncInvokeOutputDataConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import AsyncInvokeOutputDataConfigTypeDef


def get_value() -> AsyncInvokeOutputDataConfigTypeDef:
    return {
        "s3OutputDataConfig": ...,
    }


# AsyncInvokeOutputDataConfigTypeDef definition

class AsyncInvokeOutputDataConfigTypeDef(TypedDict):
    s3OutputDataConfig: NotRequired[AsyncInvokeS3OutputDataConfigTypeDef],  # (1)
```

1. See [:material-code-braces: AsyncInvokeS3OutputDataConfigTypeDef](./type_defs.md#asyncinvokes3outputdataconfigtypedef)

## DocumentSourceTypeDef

```python
# DocumentSourceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import DocumentSourceTypeDef


def get_value() -> DocumentSourceTypeDef:
    return {
        "bytes": ...,
    }


# DocumentSourceTypeDef definition

class DocumentSourceTypeDef(TypedDict):
    bytes: NotRequired[BlobTypeDef],
```


## GuardrailConverseImageSourceTypeDef

```python
# GuardrailConverseImageSourceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailConverseImageSourceTypeDef


def get_value() -> GuardrailConverseImageSourceTypeDef:
    return {
        "bytes": ...,
    }


# GuardrailConverseImageSourceTypeDef definition

class GuardrailConverseImageSourceTypeDef(TypedDict):
    bytes: NotRequired[BlobTypeDef],
```


## GuardrailImageSourceTypeDef

```python
# GuardrailImageSourceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailImageSourceTypeDef


def get_value() -> GuardrailImageSourceTypeDef:
    return {
        "bytes": ...,
    }


# GuardrailImageSourceTypeDef definition

class GuardrailImageSourceTypeDef(TypedDict):
    bytes: NotRequired[BlobTypeDef],
```


## ImageSourceTypeDef

```python
# ImageSourceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ImageSourceTypeDef


def get_value() -> ImageSourceTypeDef:
    return {
        "bytes": ...,
    }


# ImageSourceTypeDef definition

class ImageSourceTypeDef(TypedDict):
    bytes: NotRequired[BlobTypeDef],
```


## InvokeModelRequestTypeDef

```python
# InvokeModelRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import InvokeModelRequestTypeDef


def get_value() -> InvokeModelRequestTypeDef:
    return {
        "modelId": ...,
    }


# InvokeModelRequestTypeDef definition

class InvokeModelRequestTypeDef(TypedDict):
    modelId: str,
    body: NotRequired[BlobTypeDef],
    contentType: NotRequired[str],
    accept: NotRequired[str],
    trace: NotRequired[TraceType],  # (1)
    guardrailIdentifier: NotRequired[str],
    guardrailVersion: NotRequired[str],
    performanceConfigLatency: NotRequired[PerformanceConfigLatencyType],  # (2)
```

1. See [:material-code-brackets: TraceType](./literals.md#tracetype)
2. See [:material-code-brackets: PerformanceConfigLatencyType](./literals.md#performanceconfiglatencytype)

## InvokeModelWithResponseStreamRequestTypeDef

```python
# InvokeModelWithResponseStreamRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import InvokeModelWithResponseStreamRequestTypeDef


def get_value() -> InvokeModelWithResponseStreamRequestTypeDef:
    return {
        "modelId": ...,
    }


# InvokeModelWithResponseStreamRequestTypeDef definition

class InvokeModelWithResponseStreamRequestTypeDef(TypedDict):
    modelId: str,
    body: NotRequired[BlobTypeDef],
    contentType: NotRequired[str],
    accept: NotRequired[str],
    trace: NotRequired[TraceType],  # (1)
    guardrailIdentifier: NotRequired[str],
    guardrailVersion: NotRequired[str],
    performanceConfigLatency: NotRequired[PerformanceConfigLatencyType],  # (2)
```

1. See [:material-code-brackets: TraceType](./literals.md#tracetype)
2. See [:material-code-brackets: PerformanceConfigLatencyType](./literals.md#performanceconfiglatencytype)

## ContentBlockDeltaTypeDef

```python
# ContentBlockDeltaTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ContentBlockDeltaTypeDef


def get_value() -> ContentBlockDeltaTypeDef:
    return {
        "text": ...,
    }


# ContentBlockDeltaTypeDef definition

class ContentBlockDeltaTypeDef(TypedDict):
    text: NotRequired[str],
    toolUse: NotRequired[ToolUseBlockDeltaTypeDef],  # (1)
    reasoningContent: NotRequired[ReasoningContentBlockDeltaTypeDef],  # (2)
```

1. See [:material-code-braces: ToolUseBlockDeltaTypeDef](./type_defs.md#tooluseblockdeltatypedef)
2. See [:material-code-braces: ReasoningContentBlockDeltaTypeDef](./type_defs.md#reasoningcontentblockdeltatypedef)

## ContentBlockStartTypeDef

```python
# ContentBlockStartTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ContentBlockStartTypeDef


def get_value() -> ContentBlockStartTypeDef:
    return {
        "toolUse": ...,
    }


# ContentBlockStartTypeDef definition

class ContentBlockStartTypeDef(TypedDict):
    toolUse: NotRequired[ToolUseBlockStartTypeDef],  # (1)
```

1. See [:material-code-braces: ToolUseBlockStartTypeDef](./type_defs.md#tooluseblockstarttypedef)

## DocumentBlockOutputTypeDef

```python
# DocumentBlockOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import DocumentBlockOutputTypeDef


def get_value() -> DocumentBlockOutputTypeDef:
    return {
        "format": ...,
    }


# DocumentBlockOutputTypeDef definition

class DocumentBlockOutputTypeDef(TypedDict):
    format: DocumentFormatType,  # (1)
    name: str,
    source: DocumentSourceOutputTypeDef,  # (2)
```

1. See [:material-code-brackets: DocumentFormatType](./literals.md#documentformattype)
2. See [:material-code-braces: DocumentSourceOutputTypeDef](./type_defs.md#documentsourceoutputtypedef)

## GuardrailContentPolicyAssessmentTypeDef

```python
# GuardrailContentPolicyAssessmentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailContentPolicyAssessmentTypeDef


def get_value() -> GuardrailContentPolicyAssessmentTypeDef:
    return {
        "filters": ...,
    }


# GuardrailContentPolicyAssessmentTypeDef definition

class GuardrailContentPolicyAssessmentTypeDef(TypedDict):
    filters: List[GuardrailContentFilterTypeDef],  # (1)
```

1. See `List[GuardrailContentFilterTypeDef]`

## GuardrailContextualGroundingPolicyAssessmentTypeDef

```python
# GuardrailContextualGroundingPolicyAssessmentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailContextualGroundingPolicyAssessmentTypeDef


def get_value() -> GuardrailContextualGroundingPolicyAssessmentTypeDef:
    return {
        "filters": ...,
    }


# GuardrailContextualGroundingPolicyAssessmentTypeDef definition

class GuardrailContextualGroundingPolicyAssessmentTypeDef(TypedDict):
    filters: NotRequired[List[GuardrailContextualGroundingFilterTypeDef]],  # (1)
```

1. See `List[GuardrailContextualGroundingFilterTypeDef]`

## GuardrailConverseImageBlockOutputTypeDef

```python
# GuardrailConverseImageBlockOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailConverseImageBlockOutputTypeDef


def get_value() -> GuardrailConverseImageBlockOutputTypeDef:
    return {
        "format": ...,
    }


# GuardrailConverseImageBlockOutputTypeDef definition

class GuardrailConverseImageBlockOutputTypeDef(TypedDict):
    format: GuardrailConverseImageFormatType,  # (1)
    source: GuardrailConverseImageSourceOutputTypeDef,  # (2)
```

1. See [:material-code-brackets: GuardrailConverseImageFormatType](./literals.md#guardrailconverseimageformattype)
2. See [:material-code-braces: GuardrailConverseImageSourceOutputTypeDef](./type_defs.md#guardrailconverseimagesourceoutputtypedef)

## GuardrailCoverageTypeDef

```python
# GuardrailCoverageTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailCoverageTypeDef


def get_value() -> GuardrailCoverageTypeDef:
    return {
        "textCharacters": ...,
    }


# GuardrailCoverageTypeDef definition

class GuardrailCoverageTypeDef(TypedDict):
    textCharacters: NotRequired[GuardrailTextCharactersCoverageTypeDef],  # (1)
    images: NotRequired[GuardrailImageCoverageTypeDef],  # (2)
```

1. See [:material-code-braces: GuardrailTextCharactersCoverageTypeDef](./type_defs.md#guardrailtextcharacterscoveragetypedef)
2. See [:material-code-braces: GuardrailImageCoverageTypeDef](./type_defs.md#guardrailimagecoveragetypedef)

## GuardrailWordPolicyAssessmentTypeDef

```python
# GuardrailWordPolicyAssessmentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailWordPolicyAssessmentTypeDef


def get_value() -> GuardrailWordPolicyAssessmentTypeDef:
    return {
        "customWords": ...,
    }


# GuardrailWordPolicyAssessmentTypeDef definition

class GuardrailWordPolicyAssessmentTypeDef(TypedDict):
    customWords: List[GuardrailCustomWordTypeDef],  # (1)
    managedWordLists: List[GuardrailManagedWordTypeDef],  # (2)
```

1. See `List[GuardrailCustomWordTypeDef]`
2. See `List[GuardrailManagedWordTypeDef]`

## GuardrailSensitiveInformationPolicyAssessmentTypeDef

```python
# GuardrailSensitiveInformationPolicyAssessmentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailSensitiveInformationPolicyAssessmentTypeDef


def get_value() -> GuardrailSensitiveInformationPolicyAssessmentTypeDef:
    return {
        "piiEntities": ...,
    }


# GuardrailSensitiveInformationPolicyAssessmentTypeDef definition

class GuardrailSensitiveInformationPolicyAssessmentTypeDef(TypedDict):
    piiEntities: List[GuardrailPiiEntityFilterTypeDef],  # (1)
    regexes: List[GuardrailRegexFilterTypeDef],  # (2)
```

1. See `List[GuardrailPiiEntityFilterTypeDef]`
2. See `List[GuardrailRegexFilterTypeDef]`

## GuardrailTopicPolicyAssessmentTypeDef

```python
# GuardrailTopicPolicyAssessmentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailTopicPolicyAssessmentTypeDef


def get_value() -> GuardrailTopicPolicyAssessmentTypeDef:
    return {
        "topics": ...,
    }


# GuardrailTopicPolicyAssessmentTypeDef definition

class GuardrailTopicPolicyAssessmentTypeDef(TypedDict):
    topics: List[GuardrailTopicTypeDef],  # (1)
```

1. See `List[GuardrailTopicTypeDef]`

## ImageBlockOutputTypeDef

```python
# ImageBlockOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ImageBlockOutputTypeDef


def get_value() -> ImageBlockOutputTypeDef:
    return {
        "format": ...,
    }


# ImageBlockOutputTypeDef definition

class ImageBlockOutputTypeDef(TypedDict):
    format: ImageFormatType,  # (1)
    source: ImageSourceOutputTypeDef,  # (2)
```

1. See [:material-code-brackets: ImageFormatType](./literals.md#imageformattype)
2. See [:material-code-braces: ImageSourceOutputTypeDef](./type_defs.md#imagesourceoutputtypedef)

## ListAsyncInvokesRequestPaginateTypeDef

```python
# ListAsyncInvokesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ListAsyncInvokesRequestPaginateTypeDef


def get_value() -> ListAsyncInvokesRequestPaginateTypeDef:
    return {
        "submitTimeAfter": ...,
    }


# ListAsyncInvokesRequestPaginateTypeDef definition

class ListAsyncInvokesRequestPaginateTypeDef(TypedDict):
    submitTimeAfter: NotRequired[TimestampTypeDef],
    submitTimeBefore: NotRequired[TimestampTypeDef],
    statusEquals: NotRequired[AsyncInvokeStatusType],  # (1)
    sortBy: NotRequired[SortAsyncInvocationByType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: AsyncInvokeStatusType](./literals.md#asyncinvokestatustype)
2. See [:material-code-brackets: SortAsyncInvocationByType](./literals.md#sortasyncinvocationbytype)
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListAsyncInvokesRequestTypeDef

```python
# ListAsyncInvokesRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ListAsyncInvokesRequestTypeDef


def get_value() -> ListAsyncInvokesRequestTypeDef:
    return {
        "submitTimeAfter": ...,
    }


# ListAsyncInvokesRequestTypeDef definition

class ListAsyncInvokesRequestTypeDef(TypedDict):
    submitTimeAfter: NotRequired[TimestampTypeDef],
    submitTimeBefore: NotRequired[TimestampTypeDef],
    statusEquals: NotRequired[AsyncInvokeStatusType],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortBy: NotRequired[SortAsyncInvocationByType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
```

1. See [:material-code-brackets: AsyncInvokeStatusType](./literals.md#asyncinvokestatustype)
2. See [:material-code-brackets: SortAsyncInvocationByType](./literals.md#sortasyncinvocationbytype)
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype)

## ResponseStreamTypeDef

```python
# ResponseStreamTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ResponseStreamTypeDef


def get_value() -> ResponseStreamTypeDef:
    return {
        "chunk": ...,
    }


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

## ReasoningContentBlockOutputTypeDef

```python
# ReasoningContentBlockOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ReasoningContentBlockOutputTypeDef


def get_value() -> ReasoningContentBlockOutputTypeDef:
    return {
        "reasoningText": ...,
    }


# ReasoningContentBlockOutputTypeDef definition

class ReasoningContentBlockOutputTypeDef(TypedDict):
    reasoningText: NotRequired[ReasoningTextBlockTypeDef],  # (1)
    redactedContent: NotRequired[bytes],
```

1. See [:material-code-braces: ReasoningTextBlockTypeDef](./type_defs.md#reasoningtextblocktypedef)

## ReasoningContentBlockTypeDef

```python
# ReasoningContentBlockTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ReasoningContentBlockTypeDef


def get_value() -> ReasoningContentBlockTypeDef:
    return {
        "reasoningText": ...,
    }


# ReasoningContentBlockTypeDef definition

class ReasoningContentBlockTypeDef(TypedDict):
    reasoningText: NotRequired[ReasoningTextBlockTypeDef],  # (1)
    redactedContent: NotRequired[BlobTypeDef],
```

1. See [:material-code-braces: ReasoningTextBlockTypeDef](./type_defs.md#reasoningtextblocktypedef)

## VideoSourceOutputTypeDef

```python
# VideoSourceOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import VideoSourceOutputTypeDef


def get_value() -> VideoSourceOutputTypeDef:
    return {
        "bytes": ...,
    }


# VideoSourceOutputTypeDef definition

class VideoSourceOutputTypeDef(TypedDict):
    bytes: NotRequired[bytes],
    s3Location: NotRequired[S3LocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef)

## VideoSourceTypeDef

```python
# VideoSourceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import VideoSourceTypeDef


def get_value() -> VideoSourceTypeDef:
    return {
        "bytes": ...,
    }


# VideoSourceTypeDef definition

class VideoSourceTypeDef(TypedDict):
    bytes: NotRequired[BlobTypeDef],
    s3Location: NotRequired[S3LocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef)

## ToolChoiceTypeDef

```python
# ToolChoiceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ToolChoiceTypeDef


def get_value() -> ToolChoiceTypeDef:
    return {
        "auto": ...,
    }


# ToolChoiceTypeDef definition

class ToolChoiceTypeDef(TypedDict):
    auto: NotRequired[Mapping[str, Any]],
    any: NotRequired[Mapping[str, Any]],
    tool: NotRequired[SpecificToolChoiceTypeDef],  # (1)
```

1. See [:material-code-braces: SpecificToolChoiceTypeDef](./type_defs.md#specifictoolchoicetypedef)

## ToolSpecificationTypeDef

```python
# ToolSpecificationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ToolSpecificationTypeDef


def get_value() -> ToolSpecificationTypeDef:
    return {
        "name": ...,
    }


# ToolSpecificationTypeDef definition

class ToolSpecificationTypeDef(TypedDict):
    name: str,
    inputSchema: ToolInputSchemaTypeDef,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: ToolInputSchemaTypeDef](./type_defs.md#toolinputschematypedef)

## AsyncInvokeSummaryTypeDef

```python
# AsyncInvokeSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import AsyncInvokeSummaryTypeDef


def get_value() -> AsyncInvokeSummaryTypeDef:
    return {
        "invocationArn": ...,
    }


# AsyncInvokeSummaryTypeDef definition

class AsyncInvokeSummaryTypeDef(TypedDict):
    invocationArn: str,
    modelArn: str,
    submitTime: datetime.datetime,
    outputDataConfig: AsyncInvokeOutputDataConfigTypeDef,  # (2)
    clientRequestToken: NotRequired[str],
    status: NotRequired[AsyncInvokeStatusType],  # (1)
    failureMessage: NotRequired[str],
    lastModifiedTime: NotRequired[datetime.datetime],
    endTime: NotRequired[datetime.datetime],
```

1. See [:material-code-brackets: AsyncInvokeStatusType](./literals.md#asyncinvokestatustype)
2. See [:material-code-braces: AsyncInvokeOutputDataConfigTypeDef](./type_defs.md#asyncinvokeoutputdataconfigtypedef)

## GetAsyncInvokeResponseTypeDef

```python
# GetAsyncInvokeResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GetAsyncInvokeResponseTypeDef


def get_value() -> GetAsyncInvokeResponseTypeDef:
    return {
        "invocationArn": ...,
    }


# GetAsyncInvokeResponseTypeDef definition

class GetAsyncInvokeResponseTypeDef(TypedDict):
    invocationArn: str,
    modelArn: str,
    clientRequestToken: str,
    status: AsyncInvokeStatusType,  # (1)
    failureMessage: str,
    submitTime: datetime.datetime,
    lastModifiedTime: datetime.datetime,
    endTime: datetime.datetime,
    outputDataConfig: AsyncInvokeOutputDataConfigTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AsyncInvokeStatusType](./literals.md#asyncinvokestatustype)
2. See [:material-code-braces: AsyncInvokeOutputDataConfigTypeDef](./type_defs.md#asyncinvokeoutputdataconfigtypedef)
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## StartAsyncInvokeRequestTypeDef

```python
# StartAsyncInvokeRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import StartAsyncInvokeRequestTypeDef


def get_value() -> StartAsyncInvokeRequestTypeDef:
    return {
        "modelId": ...,
    }


# StartAsyncInvokeRequestTypeDef definition

class StartAsyncInvokeRequestTypeDef(TypedDict):
    modelId: str,
    modelInput: Mapping[str, Any],
    outputDataConfig: AsyncInvokeOutputDataConfigTypeDef,  # (1)
    clientRequestToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: AsyncInvokeOutputDataConfigTypeDef](./type_defs.md#asyncinvokeoutputdataconfigtypedef)
2. See `Sequence[TagTypeDef]`

## GuardrailImageBlockTypeDef

```python
# GuardrailImageBlockTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailImageBlockTypeDef


def get_value() -> GuardrailImageBlockTypeDef:
    return {
        "format": ...,
    }


# GuardrailImageBlockTypeDef definition

class GuardrailImageBlockTypeDef(TypedDict):
    format: GuardrailImageFormatType,  # (1)
    source: GuardrailImageSourceTypeDef,  # (2)
```

1. See [:material-code-brackets: GuardrailImageFormatType](./literals.md#guardrailimageformattype)
2. See [:material-code-braces: GuardrailImageSourceTypeDef](./type_defs.md#guardrailimagesourcetypedef)

## ContentBlockDeltaEventTypeDef

```python
# ContentBlockDeltaEventTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ContentBlockDeltaEventTypeDef


def get_value() -> ContentBlockDeltaEventTypeDef:
    return {
        "delta": ...,
    }


# ContentBlockDeltaEventTypeDef definition

class ContentBlockDeltaEventTypeDef(TypedDict):
    delta: ContentBlockDeltaTypeDef,  # (1)
    contentBlockIndex: int,
```

1. See [:material-code-braces: ContentBlockDeltaTypeDef](./type_defs.md#contentblockdeltatypedef)

## ContentBlockStartEventTypeDef

```python
# ContentBlockStartEventTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ContentBlockStartEventTypeDef


def get_value() -> ContentBlockStartEventTypeDef:
    return {
        "start": ...,
    }


# ContentBlockStartEventTypeDef definition

class ContentBlockStartEventTypeDef(TypedDict):
    start: ContentBlockStartTypeDef,  # (1)
    contentBlockIndex: int,
```

1. See [:material-code-braces: ContentBlockStartTypeDef](./type_defs.md#contentblockstarttypedef)

## GuardrailConverseContentBlockOutputTypeDef

```python
# GuardrailConverseContentBlockOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailConverseContentBlockOutputTypeDef


def get_value() -> GuardrailConverseContentBlockOutputTypeDef:
    return {
        "text": ...,
    }


# GuardrailConverseContentBlockOutputTypeDef definition

class GuardrailConverseContentBlockOutputTypeDef(TypedDict):
    text: NotRequired[GuardrailConverseTextBlockOutputTypeDef],  # (1)
    image: NotRequired[GuardrailConverseImageBlockOutputTypeDef],  # (2)
```

1. See [:material-code-braces: GuardrailConverseTextBlockOutputTypeDef](./type_defs.md#guardrailconversetextblockoutputtypedef)
2. See [:material-code-braces: GuardrailConverseImageBlockOutputTypeDef](./type_defs.md#guardrailconverseimageblockoutputtypedef)

## GuardrailInvocationMetricsTypeDef

```python
# GuardrailInvocationMetricsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailInvocationMetricsTypeDef


def get_value() -> GuardrailInvocationMetricsTypeDef:
    return {
        "guardrailProcessingLatency": ...,
    }


# GuardrailInvocationMetricsTypeDef definition

class GuardrailInvocationMetricsTypeDef(TypedDict):
    guardrailProcessingLatency: NotRequired[int],
    usage: NotRequired[GuardrailUsageTypeDef],  # (1)
    guardrailCoverage: NotRequired[GuardrailCoverageTypeDef],  # (2)
```

1. See [:material-code-braces: GuardrailUsageTypeDef](./type_defs.md#guardrailusagetypedef)
2. See [:material-code-braces: GuardrailCoverageTypeDef](./type_defs.md#guardrailcoveragetypedef)

## InvokeModelWithResponseStreamResponseTypeDef

```python
# InvokeModelWithResponseStreamResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import InvokeModelWithResponseStreamResponseTypeDef


def get_value() -> InvokeModelWithResponseStreamResponseTypeDef:
    return {
        "body": ...,
    }


# InvokeModelWithResponseStreamResponseTypeDef definition

class InvokeModelWithResponseStreamResponseTypeDef(TypedDict):
    body: aiobotocore.eventstream.AioEventStream[ResponseStreamTypeDef],  # (1)
    contentType: str,
    performanceConfigLatency: PerformanceConfigLatencyType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See `AioEventStream[ResponseStreamTypeDef]`
2. See [:material-code-brackets: PerformanceConfigLatencyType](./literals.md#performanceconfiglatencytype)
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## VideoBlockOutputTypeDef

```python
# VideoBlockOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import VideoBlockOutputTypeDef


def get_value() -> VideoBlockOutputTypeDef:
    return {
        "format": ...,
    }


# VideoBlockOutputTypeDef definition

class VideoBlockOutputTypeDef(TypedDict):
    format: VideoFormatType,  # (1)
    source: VideoSourceOutputTypeDef,  # (2)
```

1. See [:material-code-brackets: VideoFormatType](./literals.md#videoformattype)
2. See [:material-code-braces: VideoSourceOutputTypeDef](./type_defs.md#videosourceoutputtypedef)

## ToolTypeDef

```python
# ToolTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ToolTypeDef


def get_value() -> ToolTypeDef:
    return {
        "toolSpec": ...,
    }


# ToolTypeDef definition

class ToolTypeDef(TypedDict):
    toolSpec: NotRequired[ToolSpecificationTypeDef],  # (1)
```

1. See [:material-code-braces: ToolSpecificationTypeDef](./type_defs.md#toolspecificationtypedef)

## ListAsyncInvokesResponseTypeDef

```python
# ListAsyncInvokesResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ListAsyncInvokesResponseTypeDef


def get_value() -> ListAsyncInvokesResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListAsyncInvokesResponseTypeDef definition

class ListAsyncInvokesResponseTypeDef(TypedDict):
    asyncInvokeSummaries: List[AsyncInvokeSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `List[AsyncInvokeSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DocumentBlockTypeDef

```python
# DocumentBlockTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import DocumentBlockTypeDef


def get_value() -> DocumentBlockTypeDef:
    return {
        "format": ...,
    }


# DocumentBlockTypeDef definition

class DocumentBlockTypeDef(TypedDict):
    format: DocumentFormatType,  # (1)
    name: str,
    source: DocumentSourceUnionTypeDef,  # (2)
```

1. See [:material-code-brackets: DocumentFormatType](./literals.md#documentformattype)
2. See [:material-code-braces: DocumentSourceUnionTypeDef](#documentsourceuniontypedef)

## GuardrailConverseImageBlockTypeDef

```python
# GuardrailConverseImageBlockTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailConverseImageBlockTypeDef


def get_value() -> GuardrailConverseImageBlockTypeDef:
    return {
        "format": ...,
    }


# GuardrailConverseImageBlockTypeDef definition

class GuardrailConverseImageBlockTypeDef(TypedDict):
    format: GuardrailConverseImageFormatType,  # (1)
    source: GuardrailConverseImageSourceUnionTypeDef,  # (2)
```

1. See [:material-code-brackets: GuardrailConverseImageFormatType](./literals.md#guardrailconverseimageformattype)
2. See [:material-code-braces: GuardrailConverseImageSourceUnionTypeDef](#guardrailconverseimagesourceuniontypedef)

## GuardrailContentBlockTypeDef

```python
# GuardrailContentBlockTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailContentBlockTypeDef


def get_value() -> GuardrailContentBlockTypeDef:
    return {
        "text": ...,
    }


# GuardrailContentBlockTypeDef definition

class GuardrailContentBlockTypeDef(TypedDict):
    text: NotRequired[GuardrailTextBlockTypeDef],  # (1)
    image: NotRequired[GuardrailImageBlockTypeDef],  # (2)
```

1. See [:material-code-braces: GuardrailTextBlockTypeDef](./type_defs.md#guardrailtextblocktypedef)
2. See [:material-code-braces: GuardrailImageBlockTypeDef](./type_defs.md#guardrailimageblocktypedef)

## ImageBlockTypeDef

```python
# ImageBlockTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ImageBlockTypeDef


def get_value() -> ImageBlockTypeDef:
    return {
        "format": ...,
    }


# ImageBlockTypeDef definition

class ImageBlockTypeDef(TypedDict):
    format: ImageFormatType,  # (1)
    source: ImageSourceUnionTypeDef,  # (2)
```

1. See [:material-code-brackets: ImageFormatType](./literals.md#imageformattype)
2. See [:material-code-braces: ImageSourceUnionTypeDef](#imagesourceuniontypedef)

## GuardrailAssessmentTypeDef

```python
# GuardrailAssessmentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailAssessmentTypeDef


def get_value() -> GuardrailAssessmentTypeDef:
    return {
        "topicPolicy": ...,
    }


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

## ToolResultContentBlockOutputTypeDef

```python
# ToolResultContentBlockOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ToolResultContentBlockOutputTypeDef


def get_value() -> ToolResultContentBlockOutputTypeDef:
    return {
        "json": ...,
    }


# ToolResultContentBlockOutputTypeDef definition

class ToolResultContentBlockOutputTypeDef(TypedDict):
    json: NotRequired[Dict[str, Any]],
    text: NotRequired[str],
    image: NotRequired[ImageBlockOutputTypeDef],  # (1)
    document: NotRequired[DocumentBlockOutputTypeDef],  # (2)
    video: NotRequired[VideoBlockOutputTypeDef],  # (3)
```

1. See [:material-code-braces: ImageBlockOutputTypeDef](./type_defs.md#imageblockoutputtypedef)
2. See [:material-code-braces: DocumentBlockOutputTypeDef](./type_defs.md#documentblockoutputtypedef)
3. See [:material-code-braces: VideoBlockOutputTypeDef](./type_defs.md#videoblockoutputtypedef)

## VideoBlockTypeDef

```python
# VideoBlockTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import VideoBlockTypeDef


def get_value() -> VideoBlockTypeDef:
    return {
        "format": ...,
    }


# VideoBlockTypeDef definition

class VideoBlockTypeDef(TypedDict):
    format: VideoFormatType,  # (1)
    source: VideoSourceUnionTypeDef,  # (2)
```

1. See [:material-code-brackets: VideoFormatType](./literals.md#videoformattype)
2. See [:material-code-braces: VideoSourceUnionTypeDef](#videosourceuniontypedef)

## ToolConfigurationTypeDef

```python
# ToolConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ToolConfigurationTypeDef


def get_value() -> ToolConfigurationTypeDef:
    return {
        "tools": ...,
    }


# ToolConfigurationTypeDef definition

class ToolConfigurationTypeDef(TypedDict):
    tools: Sequence[ToolTypeDef],  # (1)
    toolChoice: NotRequired[ToolChoiceTypeDef],  # (2)
```

1. See `Sequence[ToolTypeDef]`
2. See [:material-code-braces: ToolChoiceTypeDef](./type_defs.md#toolchoicetypedef)

## ApplyGuardrailRequestTypeDef

```python
# ApplyGuardrailRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ApplyGuardrailRequestTypeDef


def get_value() -> ApplyGuardrailRequestTypeDef:
    return {
        "guardrailIdentifier": ...,
    }


# ApplyGuardrailRequestTypeDef definition

class ApplyGuardrailRequestTypeDef(TypedDict):
    guardrailIdentifier: str,
    guardrailVersion: str,
    source: GuardrailContentSourceType,  # (1)
    content: Sequence[GuardrailContentBlockTypeDef],  # (2)
```

1. See [:material-code-brackets: GuardrailContentSourceType](./literals.md#guardrailcontentsourcetype)
2. See `Sequence[GuardrailContentBlockTypeDef]`

## ApplyGuardrailResponseTypeDef

```python
# ApplyGuardrailResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ApplyGuardrailResponseTypeDef


def get_value() -> ApplyGuardrailResponseTypeDef:
    return {
        "usage": ...,
    }


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
3. See `List[GuardrailOutputContentTypeDef]`
4. See `List[GuardrailAssessmentTypeDef]`
5. See [:material-code-braces: GuardrailCoverageTypeDef](./type_defs.md#guardrailcoveragetypedef)
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GuardrailTraceAssessmentTypeDef

```python
# GuardrailTraceAssessmentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailTraceAssessmentTypeDef


def get_value() -> GuardrailTraceAssessmentTypeDef:
    return {
        "modelOutput": ...,
    }


# GuardrailTraceAssessmentTypeDef definition

class GuardrailTraceAssessmentTypeDef(TypedDict):
    modelOutput: NotRequired[List[str]],
    inputAssessment: NotRequired[Dict[str, GuardrailAssessmentTypeDef]],  # (1)
    outputAssessments: NotRequired[Dict[str, List[GuardrailAssessmentTypeDef]]],  # (2)
```

1. See `Dict[str, GuardrailAssessmentTypeDef]`
2. See `Dict[str, List[GuardrailAssessmentTypeDef]]`

## ToolResultBlockOutputTypeDef

```python
# ToolResultBlockOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ToolResultBlockOutputTypeDef


def get_value() -> ToolResultBlockOutputTypeDef:
    return {
        "toolUseId": ...,
    }


# ToolResultBlockOutputTypeDef definition

class ToolResultBlockOutputTypeDef(TypedDict):
    toolUseId: str,
    content: List[ToolResultContentBlockOutputTypeDef],  # (1)
    status: NotRequired[ToolResultStatusType],  # (2)
```

1. See `List[ToolResultContentBlockOutputTypeDef]`
2. See [:material-code-brackets: ToolResultStatusType](./literals.md#toolresultstatustype)

## GuardrailConverseContentBlockTypeDef

```python
# GuardrailConverseContentBlockTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import GuardrailConverseContentBlockTypeDef


def get_value() -> GuardrailConverseContentBlockTypeDef:
    return {
        "text": ...,
    }


# GuardrailConverseContentBlockTypeDef definition

class GuardrailConverseContentBlockTypeDef(TypedDict):
    text: NotRequired[GuardrailConverseTextBlockUnionTypeDef],  # (1)
    image: NotRequired[GuardrailConverseImageBlockUnionTypeDef],  # (2)
```

1. See [:material-code-braces: GuardrailConverseTextBlockUnionTypeDef](#guardrailconversetextblockuniontypedef)
2. See [:material-code-braces: GuardrailConverseImageBlockUnionTypeDef](#guardrailconverseimageblockuniontypedef)

## ConverseStreamTraceTypeDef

```python
# ConverseStreamTraceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ConverseStreamTraceTypeDef


def get_value() -> ConverseStreamTraceTypeDef:
    return {
        "guardrail": ...,
    }


# ConverseStreamTraceTypeDef definition

class ConverseStreamTraceTypeDef(TypedDict):
    guardrail: NotRequired[GuardrailTraceAssessmentTypeDef],  # (1)
    promptRouter: NotRequired[PromptRouterTraceTypeDef],  # (2)
```

1. See [:material-code-braces: GuardrailTraceAssessmentTypeDef](./type_defs.md#guardrailtraceassessmenttypedef)
2. See [:material-code-braces: PromptRouterTraceTypeDef](./type_defs.md#promptroutertracetypedef)

## ConverseTraceTypeDef

```python
# ConverseTraceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ConverseTraceTypeDef


def get_value() -> ConverseTraceTypeDef:
    return {
        "guardrail": ...,
    }


# ConverseTraceTypeDef definition

class ConverseTraceTypeDef(TypedDict):
    guardrail: NotRequired[GuardrailTraceAssessmentTypeDef],  # (1)
    promptRouter: NotRequired[PromptRouterTraceTypeDef],  # (2)
```

1. See [:material-code-braces: GuardrailTraceAssessmentTypeDef](./type_defs.md#guardrailtraceassessmenttypedef)
2. See [:material-code-braces: PromptRouterTraceTypeDef](./type_defs.md#promptroutertracetypedef)

## ContentBlockOutputTypeDef

```python
# ContentBlockOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ContentBlockOutputTypeDef


def get_value() -> ContentBlockOutputTypeDef:
    return {
        "text": ...,
    }


# ContentBlockOutputTypeDef definition

class ContentBlockOutputTypeDef(TypedDict):
    text: NotRequired[str],
    image: NotRequired[ImageBlockOutputTypeDef],  # (1)
    document: NotRequired[DocumentBlockOutputTypeDef],  # (2)
    video: NotRequired[VideoBlockOutputTypeDef],  # (3)
    toolUse: NotRequired[ToolUseBlockOutputTypeDef],  # (4)
    toolResult: NotRequired[ToolResultBlockOutputTypeDef],  # (5)
    guardContent: NotRequired[GuardrailConverseContentBlockOutputTypeDef],  # (6)
    reasoningContent: NotRequired[ReasoningContentBlockOutputTypeDef],  # (7)
```

1. See [:material-code-braces: ImageBlockOutputTypeDef](./type_defs.md#imageblockoutputtypedef)
2. See [:material-code-braces: DocumentBlockOutputTypeDef](./type_defs.md#documentblockoutputtypedef)
3. See [:material-code-braces: VideoBlockOutputTypeDef](./type_defs.md#videoblockoutputtypedef)
4. See [:material-code-braces: ToolUseBlockOutputTypeDef](./type_defs.md#tooluseblockoutputtypedef)
5. See [:material-code-braces: ToolResultBlockOutputTypeDef](./type_defs.md#toolresultblockoutputtypedef)
6. See [:material-code-braces: GuardrailConverseContentBlockOutputTypeDef](./type_defs.md#guardrailconversecontentblockoutputtypedef)
7. See [:material-code-braces: ReasoningContentBlockOutputTypeDef](./type_defs.md#reasoningcontentblockoutputtypedef)

## ToolResultContentBlockTypeDef

```python
# ToolResultContentBlockTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ToolResultContentBlockTypeDef


def get_value() -> ToolResultContentBlockTypeDef:
    return {
        "json": ...,
    }


# ToolResultContentBlockTypeDef definition

class ToolResultContentBlockTypeDef(TypedDict):
    json: NotRequired[Mapping[str, Any]],
    text: NotRequired[str],
    image: NotRequired[ImageBlockUnionTypeDef],  # (1)
    document: NotRequired[DocumentBlockUnionTypeDef],  # (2)
    video: NotRequired[VideoBlockUnionTypeDef],  # (3)
```

1. See [:material-code-braces: ImageBlockUnionTypeDef](#imageblockuniontypedef)
2. See [:material-code-braces: DocumentBlockUnionTypeDef](#documentblockuniontypedef)
3. See [:material-code-braces: VideoBlockUnionTypeDef](#videoblockuniontypedef)

## ConverseStreamMetadataEventTypeDef

```python
# ConverseStreamMetadataEventTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ConverseStreamMetadataEventTypeDef


def get_value() -> ConverseStreamMetadataEventTypeDef:
    return {
        "usage": ...,
    }


# ConverseStreamMetadataEventTypeDef definition

class ConverseStreamMetadataEventTypeDef(TypedDict):
    usage: TokenUsageTypeDef,  # (1)
    metrics: ConverseStreamMetricsTypeDef,  # (2)
    trace: NotRequired[ConverseStreamTraceTypeDef],  # (3)
    performanceConfig: NotRequired[PerformanceConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: TokenUsageTypeDef](./type_defs.md#tokenusagetypedef)
2. See [:material-code-braces: ConverseStreamMetricsTypeDef](./type_defs.md#conversestreammetricstypedef)
3. See [:material-code-braces: ConverseStreamTraceTypeDef](./type_defs.md#conversestreamtracetypedef)
4. See [:material-code-braces: PerformanceConfigurationTypeDef](./type_defs.md#performanceconfigurationtypedef)

## MessageOutputTypeDef

```python
# MessageOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import MessageOutputTypeDef


def get_value() -> MessageOutputTypeDef:
    return {
        "role": ...,
    }


# MessageOutputTypeDef definition

class MessageOutputTypeDef(TypedDict):
    role: ConversationRoleType,  # (1)
    content: List[ContentBlockOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: ConversationRoleType](./literals.md#conversationroletype)
2. See `List[ContentBlockOutputTypeDef]`

## SystemContentBlockTypeDef

```python
# SystemContentBlockTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import SystemContentBlockTypeDef


def get_value() -> SystemContentBlockTypeDef:
    return {
        "text": ...,
    }


# SystemContentBlockTypeDef definition

class SystemContentBlockTypeDef(TypedDict):
    text: NotRequired[str],
    guardContent: NotRequired[GuardrailConverseContentBlockUnionTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailConverseContentBlockUnionTypeDef](#guardrailconversecontentblockuniontypedef)

## ConverseStreamOutputTypeDef

```python
# ConverseStreamOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ConverseStreamOutputTypeDef


def get_value() -> ConverseStreamOutputTypeDef:
    return {
        "messageStart": ...,
    }


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

## ConverseOutputTypeDef

```python
# ConverseOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ConverseOutputTypeDef


def get_value() -> ConverseOutputTypeDef:
    return {
        "message": ...,
    }


# ConverseOutputTypeDef definition

class ConverseOutputTypeDef(TypedDict):
    message: NotRequired[MessageOutputTypeDef],  # (1)
```

1. See [:material-code-braces: MessageOutputTypeDef](./type_defs.md#messageoutputtypedef)

## ToolResultBlockTypeDef

```python
# ToolResultBlockTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ToolResultBlockTypeDef


def get_value() -> ToolResultBlockTypeDef:
    return {
        "toolUseId": ...,
    }


# ToolResultBlockTypeDef definition

class ToolResultBlockTypeDef(TypedDict):
    toolUseId: str,
    content: Sequence[ToolResultContentBlockUnionTypeDef],  # (1)
    status: NotRequired[ToolResultStatusType],  # (2)
```

1. See `Sequence[ToolResultContentBlockUnionTypeDef]`
2. See [:material-code-brackets: ToolResultStatusType](./literals.md#toolresultstatustype)

## ConverseStreamResponseTypeDef

```python
# ConverseStreamResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ConverseStreamResponseTypeDef


def get_value() -> ConverseStreamResponseTypeDef:
    return {
        "stream": ...,
    }


# ConverseStreamResponseTypeDef definition

class ConverseStreamResponseTypeDef(TypedDict):
    stream: aiobotocore.eventstream.AioEventStream[ConverseStreamOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `AioEventStream[ConverseStreamOutputTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ConverseResponseTypeDef

```python
# ConverseResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ConverseResponseTypeDef


def get_value() -> ConverseResponseTypeDef:
    return {
        "output": ...,
    }


# ConverseResponseTypeDef definition

class ConverseResponseTypeDef(TypedDict):
    output: ConverseOutputTypeDef,  # (1)
    stopReason: StopReasonType,  # (2)
    usage: TokenUsageTypeDef,  # (3)
    metrics: ConverseMetricsTypeDef,  # (4)
    additionalModelResponseFields: Dict[str, Any],
    trace: ConverseTraceTypeDef,  # (5)
    performanceConfig: PerformanceConfigurationTypeDef,  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-braces: ConverseOutputTypeDef](./type_defs.md#converseoutputtypedef)
2. See [:material-code-brackets: StopReasonType](./literals.md#stopreasontype)
3. See [:material-code-braces: TokenUsageTypeDef](./type_defs.md#tokenusagetypedef)
4. See [:material-code-braces: ConverseMetricsTypeDef](./type_defs.md#conversemetricstypedef)
5. See [:material-code-braces: ConverseTraceTypeDef](./type_defs.md#conversetracetypedef)
6. See [:material-code-braces: PerformanceConfigurationTypeDef](./type_defs.md#performanceconfigurationtypedef)
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ContentBlockTypeDef

```python
# ContentBlockTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ContentBlockTypeDef


def get_value() -> ContentBlockTypeDef:
    return {
        "text": ...,
    }


# ContentBlockTypeDef definition

class ContentBlockTypeDef(TypedDict):
    text: NotRequired[str],
    image: NotRequired[ImageBlockUnionTypeDef],  # (1)
    document: NotRequired[DocumentBlockUnionTypeDef],  # (2)
    video: NotRequired[VideoBlockUnionTypeDef],  # (3)
    toolUse: NotRequired[ToolUseBlockUnionTypeDef],  # (4)
    toolResult: NotRequired[ToolResultBlockUnionTypeDef],  # (5)
    guardContent: NotRequired[GuardrailConverseContentBlockUnionTypeDef],  # (6)
    reasoningContent: NotRequired[ReasoningContentBlockUnionTypeDef],  # (7)
```

1. See [:material-code-braces: ImageBlockUnionTypeDef](#imageblockuniontypedef)
2. See [:material-code-braces: DocumentBlockUnionTypeDef](#documentblockuniontypedef)
3. See [:material-code-braces: VideoBlockUnionTypeDef](#videoblockuniontypedef)
4. See [:material-code-braces: ToolUseBlockUnionTypeDef](#tooluseblockuniontypedef)
5. See [:material-code-braces: ToolResultBlockUnionTypeDef](#toolresultblockuniontypedef)
6. See [:material-code-braces: GuardrailConverseContentBlockUnionTypeDef](#guardrailconversecontentblockuniontypedef)
7. See [:material-code-braces: ReasoningContentBlockUnionTypeDef](#reasoningcontentblockuniontypedef)

## MessageTypeDef

```python
# MessageTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import MessageTypeDef


def get_value() -> MessageTypeDef:
    return {
        "role": ...,
    }


# MessageTypeDef definition

class MessageTypeDef(TypedDict):
    role: ConversationRoleType,  # (1)
    content: Sequence[ContentBlockUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: ConversationRoleType](./literals.md#conversationroletype)
2. See `Sequence[ContentBlockUnionTypeDef]`

## ConverseRequestTypeDef

```python
# ConverseRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ConverseRequestTypeDef


def get_value() -> ConverseRequestTypeDef:
    return {
        "modelId": ...,
    }


# ConverseRequestTypeDef definition

class ConverseRequestTypeDef(TypedDict):
    modelId: str,
    messages: NotRequired[Sequence[MessageUnionTypeDef]],  # (1)
    system: NotRequired[Sequence[SystemContentBlockTypeDef]],  # (2)
    inferenceConfig: NotRequired[InferenceConfigurationTypeDef],  # (3)
    toolConfig: NotRequired[ToolConfigurationTypeDef],  # (4)
    guardrailConfig: NotRequired[GuardrailConfigurationTypeDef],  # (5)
    additionalModelRequestFields: NotRequired[Mapping[str, Any]],
    promptVariables: NotRequired[Mapping[str, PromptVariableValuesTypeDef]],  # (6)
    additionalModelResponseFieldPaths: NotRequired[Sequence[str]],
    requestMetadata: NotRequired[Mapping[str, str]],
    performanceConfig: NotRequired[PerformanceConfigurationTypeDef],  # (7)
```

1. See `Sequence[MessageUnionTypeDef]`
2. See `Sequence[SystemContentBlockTypeDef]`
3. See [:material-code-braces: InferenceConfigurationTypeDef](./type_defs.md#inferenceconfigurationtypedef)
4. See [:material-code-braces: ToolConfigurationTypeDef](./type_defs.md#toolconfigurationtypedef)
5. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef)
6. See `Mapping[str, PromptVariableValuesTypeDef]`
7. See [:material-code-braces: PerformanceConfigurationTypeDef](./type_defs.md#performanceconfigurationtypedef)

## ConverseStreamRequestTypeDef

```python
# ConverseStreamRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_runtime.type_defs import ConverseStreamRequestTypeDef


def get_value() -> ConverseStreamRequestTypeDef:
    return {
        "modelId": ...,
    }


# ConverseStreamRequestTypeDef definition

class ConverseStreamRequestTypeDef(TypedDict):
    modelId: str,
    messages: NotRequired[Sequence[MessageUnionTypeDef]],  # (1)
    system: NotRequired[Sequence[SystemContentBlockTypeDef]],  # (2)
    inferenceConfig: NotRequired[InferenceConfigurationTypeDef],  # (3)
    toolConfig: NotRequired[ToolConfigurationTypeDef],  # (4)
    guardrailConfig: NotRequired[GuardrailStreamConfigurationTypeDef],  # (5)
    additionalModelRequestFields: NotRequired[Mapping[str, Any]],
    promptVariables: NotRequired[Mapping[str, PromptVariableValuesTypeDef]],  # (6)
    additionalModelResponseFieldPaths: NotRequired[Sequence[str]],
    requestMetadata: NotRequired[Mapping[str, str]],
    performanceConfig: NotRequired[PerformanceConfigurationTypeDef],  # (7)
```

1. See `Sequence[MessageUnionTypeDef]`
2. See `Sequence[SystemContentBlockTypeDef]`
3. See [:material-code-braces: InferenceConfigurationTypeDef](./type_defs.md#inferenceconfigurationtypedef)
4. See [:material-code-braces: ToolConfigurationTypeDef](./type_defs.md#toolconfigurationtypedef)
5. See [:material-code-braces: GuardrailStreamConfigurationTypeDef](./type_defs.md#guardrailstreamconfigurationtypedef)
6. See `Mapping[str, PromptVariableValuesTypeDef]`
7. See [:material-code-braces: PerformanceConfigurationTypeDef](./type_defs.md#performanceconfigurationtypedef)

