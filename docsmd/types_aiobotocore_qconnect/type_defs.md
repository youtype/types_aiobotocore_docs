# Type definitions

> [Index](../README.md) > [QConnect](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [QConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#qconnect)
    type annotations stubs module [types-aiobotocore-qconnect](https://pypi.org/project/types-aiobotocore-qconnect/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_qconnect.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## GroupingConfigurationUnionTypeDef

```python
# GroupingConfigurationUnionTypeDef Union usage example

from types_aiobotocore_qconnect.type_defs import GroupingConfigurationUnionTypeDef


def get_value() -> GroupingConfigurationUnionTypeDef:
    return ...


# GroupingConfigurationUnionTypeDef definition

GroupingConfigurationUnionTypeDef = Union[
    GroupingConfigurationTypeDef,  # (1)
    GroupingConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: GroupingConfigurationTypeDef](./type_defs.md#groupingconfigurationtypedef) 
2. See [:material-code-braces: GroupingConfigurationOutputTypeDef](./type_defs.md#groupingconfigurationoutputtypedef) 

## AIGuardrailContentPolicyConfigUnionTypeDef

```python
# AIGuardrailContentPolicyConfigUnionTypeDef Union usage example

from types_aiobotocore_qconnect.type_defs import AIGuardrailContentPolicyConfigUnionTypeDef


def get_value() -> AIGuardrailContentPolicyConfigUnionTypeDef:
    return ...


# AIGuardrailContentPolicyConfigUnionTypeDef definition

AIGuardrailContentPolicyConfigUnionTypeDef = Union[
    AIGuardrailContentPolicyConfigTypeDef,  # (1)
    AIGuardrailContentPolicyConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AIGuardrailContentPolicyConfigTypeDef](./type_defs.md#aiguardrailcontentpolicyconfigtypedef) 
2. See [:material-code-braces: AIGuardrailContentPolicyConfigOutputTypeDef](./type_defs.md#aiguardrailcontentpolicyconfigoutputtypedef) 

## AIGuardrailContextualGroundingPolicyConfigUnionTypeDef

```python
# AIGuardrailContextualGroundingPolicyConfigUnionTypeDef Union usage example

from types_aiobotocore_qconnect.type_defs import AIGuardrailContextualGroundingPolicyConfigUnionTypeDef


def get_value() -> AIGuardrailContextualGroundingPolicyConfigUnionTypeDef:
    return ...


# AIGuardrailContextualGroundingPolicyConfigUnionTypeDef definition

AIGuardrailContextualGroundingPolicyConfigUnionTypeDef = Union[
    AIGuardrailContextualGroundingPolicyConfigTypeDef,  # (1)
    AIGuardrailContextualGroundingPolicyConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AIGuardrailContextualGroundingPolicyConfigTypeDef](./type_defs.md#aiguardrailcontextualgroundingpolicyconfigtypedef) 
2. See [:material-code-braces: AIGuardrailContextualGroundingPolicyConfigOutputTypeDef](./type_defs.md#aiguardrailcontextualgroundingpolicyconfigoutputtypedef) 

## AIGuardrailSensitiveInformationPolicyConfigUnionTypeDef

```python
# AIGuardrailSensitiveInformationPolicyConfigUnionTypeDef Union usage example

from types_aiobotocore_qconnect.type_defs import AIGuardrailSensitiveInformationPolicyConfigUnionTypeDef


def get_value() -> AIGuardrailSensitiveInformationPolicyConfigUnionTypeDef:
    return ...


# AIGuardrailSensitiveInformationPolicyConfigUnionTypeDef definition

AIGuardrailSensitiveInformationPolicyConfigUnionTypeDef = Union[
    AIGuardrailSensitiveInformationPolicyConfigTypeDef,  # (1)
    AIGuardrailSensitiveInformationPolicyConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AIGuardrailSensitiveInformationPolicyConfigTypeDef](./type_defs.md#aiguardrailsensitiveinformationpolicyconfigtypedef) 
2. See [:material-code-braces: AIGuardrailSensitiveInformationPolicyConfigOutputTypeDef](./type_defs.md#aiguardrailsensitiveinformationpolicyconfigoutputtypedef) 

## AIGuardrailTopicPolicyConfigUnionTypeDef

```python
# AIGuardrailTopicPolicyConfigUnionTypeDef Union usage example

from types_aiobotocore_qconnect.type_defs import AIGuardrailTopicPolicyConfigUnionTypeDef


def get_value() -> AIGuardrailTopicPolicyConfigUnionTypeDef:
    return ...


# AIGuardrailTopicPolicyConfigUnionTypeDef definition

AIGuardrailTopicPolicyConfigUnionTypeDef = Union[
    AIGuardrailTopicPolicyConfigTypeDef,  # (1)
    AIGuardrailTopicPolicyConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AIGuardrailTopicPolicyConfigTypeDef](./type_defs.md#aiguardrailtopicpolicyconfigtypedef) 
2. See [:material-code-braces: AIGuardrailTopicPolicyConfigOutputTypeDef](./type_defs.md#aiguardrailtopicpolicyconfigoutputtypedef) 

## AIGuardrailWordPolicyConfigUnionTypeDef

```python
# AIGuardrailWordPolicyConfigUnionTypeDef Union usage example

from types_aiobotocore_qconnect.type_defs import AIGuardrailWordPolicyConfigUnionTypeDef


def get_value() -> AIGuardrailWordPolicyConfigUnionTypeDef:
    return ...


# AIGuardrailWordPolicyConfigUnionTypeDef definition

AIGuardrailWordPolicyConfigUnionTypeDef = Union[
    AIGuardrailWordPolicyConfigTypeDef,  # (1)
    AIGuardrailWordPolicyConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AIGuardrailWordPolicyConfigTypeDef](./type_defs.md#aiguardrailwordpolicyconfigtypedef) 
2. See [:material-code-braces: AIGuardrailWordPolicyConfigOutputTypeDef](./type_defs.md#aiguardrailwordpolicyconfigoutputtypedef) 

## TagFilterUnionTypeDef

```python
# TagFilterUnionTypeDef Union usage example

from types_aiobotocore_qconnect.type_defs import TagFilterUnionTypeDef


def get_value() -> TagFilterUnionTypeDef:
    return ...


# TagFilterUnionTypeDef definition

TagFilterUnionTypeDef = Union[
    TagFilterTypeDef,  # (1)
    TagFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
2. See [:material-code-braces: TagFilterOutputTypeDef](./type_defs.md#tagfilteroutputtypedef) 

## MessageTemplateAttributesUnionTypeDef

```python
# MessageTemplateAttributesUnionTypeDef Union usage example

from types_aiobotocore_qconnect.type_defs import MessageTemplateAttributesUnionTypeDef


def get_value() -> MessageTemplateAttributesUnionTypeDef:
    return ...


# MessageTemplateAttributesUnionTypeDef definition

MessageTemplateAttributesUnionTypeDef = Union[
    MessageTemplateAttributesTypeDef,  # (1)
    MessageTemplateAttributesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MessageTemplateAttributesTypeDef](./type_defs.md#messagetemplateattributestypedef) 
2. See [:material-code-braces: MessageTemplateAttributesOutputTypeDef](./type_defs.md#messagetemplateattributesoutputtypedef) 

## MessageTemplateContentProviderUnionTypeDef

```python
# MessageTemplateContentProviderUnionTypeDef Union usage example

from types_aiobotocore_qconnect.type_defs import MessageTemplateContentProviderUnionTypeDef


def get_value() -> MessageTemplateContentProviderUnionTypeDef:
    return ...


# MessageTemplateContentProviderUnionTypeDef definition

MessageTemplateContentProviderUnionTypeDef = Union[
    MessageTemplateContentProviderTypeDef,  # (1)
    MessageTemplateContentProviderOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MessageTemplateContentProviderTypeDef](./type_defs.md#messagetemplatecontentprovidertypedef) 
2. See [:material-code-braces: MessageTemplateContentProviderOutputTypeDef](./type_defs.md#messagetemplatecontentprovideroutputtypedef) 

## VectorIngestionConfigurationUnionTypeDef

```python
# VectorIngestionConfigurationUnionTypeDef Union usage example

from types_aiobotocore_qconnect.type_defs import VectorIngestionConfigurationUnionTypeDef


def get_value() -> VectorIngestionConfigurationUnionTypeDef:
    return ...


# VectorIngestionConfigurationUnionTypeDef definition

VectorIngestionConfigurationUnionTypeDef = Union[
    VectorIngestionConfigurationTypeDef,  # (1)
    VectorIngestionConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: VectorIngestionConfigurationTypeDef](./type_defs.md#vectoringestionconfigurationtypedef) 
2. See [:material-code-braces: VectorIngestionConfigurationOutputTypeDef](./type_defs.md#vectoringestionconfigurationoutputtypedef) 

## SourceConfigurationUnionTypeDef

```python
# SourceConfigurationUnionTypeDef Union usage example

from types_aiobotocore_qconnect.type_defs import SourceConfigurationUnionTypeDef


def get_value() -> SourceConfigurationUnionTypeDef:
    return ...


# SourceConfigurationUnionTypeDef definition

SourceConfigurationUnionTypeDef = Union[
    SourceConfigurationTypeDef,  # (1)
    SourceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SourceConfigurationTypeDef](./type_defs.md#sourceconfigurationtypedef) 
2. See [:material-code-braces: SourceConfigurationOutputTypeDef](./type_defs.md#sourceconfigurationoutputtypedef) 

## AIAgentConfigurationUnionTypeDef

```python
# AIAgentConfigurationUnionTypeDef Union usage example

from types_aiobotocore_qconnect.type_defs import AIAgentConfigurationUnionTypeDef


def get_value() -> AIAgentConfigurationUnionTypeDef:
    return ...


# AIAgentConfigurationUnionTypeDef definition

AIAgentConfigurationUnionTypeDef = Union[
    AIAgentConfigurationTypeDef,  # (1)
    AIAgentConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AIAgentConfigurationTypeDef](./type_defs.md#aiagentconfigurationtypedef) 
2. See [:material-code-braces: AIAgentConfigurationOutputTypeDef](./type_defs.md#aiagentconfigurationoutputtypedef) 



## AIAgentConfigurationDataTypeDef

```python
# AIAgentConfigurationDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIAgentConfigurationDataTypeDef


def get_value() -> AIAgentConfigurationDataTypeDef:
    return {
        "aiAgentId": ...,
    }


# AIAgentConfigurationDataTypeDef definition

class AIAgentConfigurationDataTypeDef(TypedDict):
    aiAgentId: str,
```

## GuardrailContentFilterConfigTypeDef

```python
# GuardrailContentFilterConfigTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GuardrailContentFilterConfigTypeDef


def get_value() -> GuardrailContentFilterConfigTypeDef:
    return {
        "inputStrength": ...,
    }


# GuardrailContentFilterConfigTypeDef definition

class GuardrailContentFilterConfigTypeDef(TypedDict):
    inputStrength: GuardrailFilterStrengthType,  # (1)
    outputStrength: GuardrailFilterStrengthType,  # (1)
    type: GuardrailContentFilterTypeType,  # (3)
```

1. See [:material-code-brackets: GuardrailFilterStrengthType](./literals.md#guardrailfilterstrengthtype) 
2. See [:material-code-brackets: GuardrailFilterStrengthType](./literals.md#guardrailfilterstrengthtype) 
3. See [:material-code-brackets: GuardrailContentFilterTypeType](./literals.md#guardrailcontentfiltertypetype) 
## GuardrailContextualGroundingFilterConfigTypeDef

```python
# GuardrailContextualGroundingFilterConfigTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GuardrailContextualGroundingFilterConfigTypeDef


def get_value() -> GuardrailContextualGroundingFilterConfigTypeDef:
    return {
        "threshold": ...,
    }


# GuardrailContextualGroundingFilterConfigTypeDef definition

class GuardrailContextualGroundingFilterConfigTypeDef(TypedDict):
    threshold: float,
    type: GuardrailContextualGroundingFilterTypeType,  # (1)
```

1. See [:material-code-brackets: GuardrailContextualGroundingFilterTypeType](./literals.md#guardrailcontextualgroundingfiltertypetype) 
## GuardrailPiiEntityConfigTypeDef

```python
# GuardrailPiiEntityConfigTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GuardrailPiiEntityConfigTypeDef


def get_value() -> GuardrailPiiEntityConfigTypeDef:
    return {
        "action": ...,
    }


# GuardrailPiiEntityConfigTypeDef definition

class GuardrailPiiEntityConfigTypeDef(TypedDict):
    action: GuardrailSensitiveInformationActionType,  # (1)
    type: GuardrailPiiEntityTypeType,  # (2)
```

1. See [:material-code-brackets: GuardrailSensitiveInformationActionType](./literals.md#guardrailsensitiveinformationactiontype) 
2. See [:material-code-brackets: GuardrailPiiEntityTypeType](./literals.md#guardrailpiientitytypetype) 
## GuardrailRegexConfigTypeDef

```python
# GuardrailRegexConfigTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GuardrailRegexConfigTypeDef


def get_value() -> GuardrailRegexConfigTypeDef:
    return {
        "action": ...,
    }


# GuardrailRegexConfigTypeDef definition

class GuardrailRegexConfigTypeDef(TypedDict):
    action: GuardrailSensitiveInformationActionType,  # (1)
    name: str,
    pattern: str,
    description: NotRequired[str],
```

1. See [:material-code-brackets: GuardrailSensitiveInformationActionType](./literals.md#guardrailsensitiveinformationactiontype) 
## AIGuardrailSummaryTypeDef

```python
# AIGuardrailSummaryTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIGuardrailSummaryTypeDef


def get_value() -> AIGuardrailSummaryTypeDef:
    return {
        "aiGuardrailArn": ...,
    }


# AIGuardrailSummaryTypeDef definition

class AIGuardrailSummaryTypeDef(TypedDict):
    aiGuardrailArn: str,
    aiGuardrailId: str,
    assistantArn: str,
    assistantId: str,
    name: str,
    visibilityStatus: VisibilityStatusType,  # (2)
    description: NotRequired[str],
    modifiedTime: NotRequired[datetime],
    status: NotRequired[StatusType],  # (1)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-brackets: VisibilityStatusType](./literals.md#visibilitystatustype) 
## GuardrailTopicConfigOutputTypeDef

```python
# GuardrailTopicConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GuardrailTopicConfigOutputTypeDef


def get_value() -> GuardrailTopicConfigOutputTypeDef:
    return {
        "definition": ...,
    }


# GuardrailTopicConfigOutputTypeDef definition

class GuardrailTopicConfigOutputTypeDef(TypedDict):
    definition: str,
    name: str,
    type: GuardrailTopicTypeType,  # (1)
    examples: NotRequired[List[str]],
```

1. See [:material-code-brackets: GuardrailTopicTypeType](./literals.md#guardrailtopictypetype) 
## GuardrailTopicConfigTypeDef

```python
# GuardrailTopicConfigTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GuardrailTopicConfigTypeDef


def get_value() -> GuardrailTopicConfigTypeDef:
    return {
        "definition": ...,
    }


# GuardrailTopicConfigTypeDef definition

class GuardrailTopicConfigTypeDef(TypedDict):
    definition: str,
    name: str,
    type: GuardrailTopicTypeType,  # (1)
    examples: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: GuardrailTopicTypeType](./literals.md#guardrailtopictypetype) 
## GuardrailManagedWordsConfigTypeDef

```python
# GuardrailManagedWordsConfigTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GuardrailManagedWordsConfigTypeDef


def get_value() -> GuardrailManagedWordsConfigTypeDef:
    return {
        "type": ...,
    }


# GuardrailManagedWordsConfigTypeDef definition

class GuardrailManagedWordsConfigTypeDef(TypedDict):
    type: GuardrailManagedWordsTypeType,  # (1)
```

1. See [:material-code-brackets: GuardrailManagedWordsTypeType](./literals.md#guardrailmanagedwordstypetype) 
## GuardrailWordConfigTypeDef

```python
# GuardrailWordConfigTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GuardrailWordConfigTypeDef


def get_value() -> GuardrailWordConfigTypeDef:
    return {
        "text": ...,
    }


# GuardrailWordConfigTypeDef definition

class GuardrailWordConfigTypeDef(TypedDict):
    text: str,
```

## AIPromptSummaryTypeDef

```python
# AIPromptSummaryTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIPromptSummaryTypeDef


def get_value() -> AIPromptSummaryTypeDef:
    return {
        "aiPromptArn": ...,
    }


# AIPromptSummaryTypeDef definition

class AIPromptSummaryTypeDef(TypedDict):
    aiPromptArn: str,
    aiPromptId: str,
    apiFormat: AIPromptAPIFormatType,  # (1)
    assistantArn: str,
    assistantId: str,
    modelId: str,
    name: str,
    templateType: AIPromptTemplateTypeType,  # (4)
    type: AIPromptTypeType,  # (5)
    visibilityStatus: VisibilityStatusType,  # (6)
    description: NotRequired[str],
    modifiedTime: NotRequired[datetime],
    origin: NotRequired[OriginType],  # (2)
    status: NotRequired[StatusType],  # (3)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: AIPromptAPIFormatType](./literals.md#aipromptapiformattype) 
2. See [:material-code-brackets: OriginType](./literals.md#origintype) 
3. See [:material-code-brackets: StatusType](./literals.md#statustype) 
4. See [:material-code-brackets: AIPromptTemplateTypeType](./literals.md#aiprompttemplatetypetype) 
5. See [:material-code-brackets: AIPromptTypeType](./literals.md#aiprompttypetype) 
6. See [:material-code-brackets: VisibilityStatusType](./literals.md#visibilitystatustype) 
## TextFullAIPromptEditTemplateConfigurationTypeDef

```python
# TextFullAIPromptEditTemplateConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import TextFullAIPromptEditTemplateConfigurationTypeDef


def get_value() -> TextFullAIPromptEditTemplateConfigurationTypeDef:
    return {
        "text": ...,
    }


# TextFullAIPromptEditTemplateConfigurationTypeDef definition

class TextFullAIPromptEditTemplateConfigurationTypeDef(TypedDict):
    text: str,
```

## ActivateMessageTemplateRequestTypeDef

```python
# ActivateMessageTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ActivateMessageTemplateRequestTypeDef


def get_value() -> ActivateMessageTemplateRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# ActivateMessageTemplateRequestTypeDef definition

class ActivateMessageTemplateRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    messageTemplateId: str,
    versionNumber: int,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ResponseMetadataTypeDef


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

## AgentAttributesTypeDef

```python
# AgentAttributesTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AgentAttributesTypeDef


def get_value() -> AgentAttributesTypeDef:
    return {
        "firstName": ...,
    }


# AgentAttributesTypeDef definition

class AgentAttributesTypeDef(TypedDict):
    firstName: NotRequired[str],
    lastName: NotRequired[str],
```

## AmazonConnectGuideAssociationDataTypeDef

```python
# AmazonConnectGuideAssociationDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AmazonConnectGuideAssociationDataTypeDef


def get_value() -> AmazonConnectGuideAssociationDataTypeDef:
    return {
        "flowId": ...,
    }


# AmazonConnectGuideAssociationDataTypeDef definition

class AmazonConnectGuideAssociationDataTypeDef(TypedDict):
    flowId: NotRequired[str],
```

## AppIntegrationsConfigurationOutputTypeDef

```python
# AppIntegrationsConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AppIntegrationsConfigurationOutputTypeDef


def get_value() -> AppIntegrationsConfigurationOutputTypeDef:
    return {
        "appIntegrationArn": ...,
    }


# AppIntegrationsConfigurationOutputTypeDef definition

class AppIntegrationsConfigurationOutputTypeDef(TypedDict):
    appIntegrationArn: str,
    objectFields: NotRequired[List[str]],
```

## AppIntegrationsConfigurationTypeDef

```python
# AppIntegrationsConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AppIntegrationsConfigurationTypeDef


def get_value() -> AppIntegrationsConfigurationTypeDef:
    return {
        "appIntegrationArn": ...,
    }


# AppIntegrationsConfigurationTypeDef definition

class AppIntegrationsConfigurationTypeDef(TypedDict):
    appIntegrationArn: str,
    objectFields: NotRequired[Sequence[str]],
```

## AssistantAssociationInputDataTypeDef

```python
# AssistantAssociationInputDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AssistantAssociationInputDataTypeDef


def get_value() -> AssistantAssociationInputDataTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# AssistantAssociationInputDataTypeDef definition

class AssistantAssociationInputDataTypeDef(TypedDict):
    knowledgeBaseId: NotRequired[str],
```

## KnowledgeBaseAssociationDataTypeDef

```python
# KnowledgeBaseAssociationDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import KnowledgeBaseAssociationDataTypeDef


def get_value() -> KnowledgeBaseAssociationDataTypeDef:
    return {
        "knowledgeBaseArn": ...,
    }


# KnowledgeBaseAssociationDataTypeDef definition

class KnowledgeBaseAssociationDataTypeDef(TypedDict):
    knowledgeBaseArn: NotRequired[str],
    knowledgeBaseId: NotRequired[str],
```

## AssistantCapabilityConfigurationTypeDef

```python
# AssistantCapabilityConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AssistantCapabilityConfigurationTypeDef


def get_value() -> AssistantCapabilityConfigurationTypeDef:
    return {
        "type": ...,
    }


# AssistantCapabilityConfigurationTypeDef definition

class AssistantCapabilityConfigurationTypeDef(TypedDict):
    type: NotRequired[AssistantCapabilityTypeType],  # (1)
```

1. See [:material-code-brackets: AssistantCapabilityTypeType](./literals.md#assistantcapabilitytypetype) 
## AssistantIntegrationConfigurationTypeDef

```python
# AssistantIntegrationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AssistantIntegrationConfigurationTypeDef


def get_value() -> AssistantIntegrationConfigurationTypeDef:
    return {
        "topicIntegrationArn": ...,
    }


# AssistantIntegrationConfigurationTypeDef definition

class AssistantIntegrationConfigurationTypeDef(TypedDict):
    topicIntegrationArn: NotRequired[str],
```

## ServerSideEncryptionConfigurationTypeDef

```python
# ServerSideEncryptionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ServerSideEncryptionConfigurationTypeDef


def get_value() -> ServerSideEncryptionConfigurationTypeDef:
    return {
        "kmsKeyId": ...,
    }


# ServerSideEncryptionConfigurationTypeDef definition

class ServerSideEncryptionConfigurationTypeDef(TypedDict):
    kmsKeyId: NotRequired[str],
```

## ParsingPromptTypeDef

```python
# ParsingPromptTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ParsingPromptTypeDef


def get_value() -> ParsingPromptTypeDef:
    return {
        "parsingPromptText": ...,
    }


# ParsingPromptTypeDef definition

class ParsingPromptTypeDef(TypedDict):
    parsingPromptText: str,
```

## FixedSizeChunkingConfigurationTypeDef

```python
# FixedSizeChunkingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import FixedSizeChunkingConfigurationTypeDef


def get_value() -> FixedSizeChunkingConfigurationTypeDef:
    return {
        "maxTokens": ...,
    }


# FixedSizeChunkingConfigurationTypeDef definition

class FixedSizeChunkingConfigurationTypeDef(TypedDict):
    maxTokens: int,
    overlapPercentage: int,
```

## SemanticChunkingConfigurationTypeDef

```python
# SemanticChunkingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SemanticChunkingConfigurationTypeDef


def get_value() -> SemanticChunkingConfigurationTypeDef:
    return {
        "breakpointPercentileThreshold": ...,
    }


# SemanticChunkingConfigurationTypeDef definition

class SemanticChunkingConfigurationTypeDef(TypedDict):
    breakpointPercentileThreshold: int,
    bufferSize: int,
    maxTokens: int,
```

## CitationSpanTypeDef

```python
# CitationSpanTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CitationSpanTypeDef


def get_value() -> CitationSpanTypeDef:
    return {
        "beginOffsetInclusive": ...,
    }


# CitationSpanTypeDef definition

class CitationSpanTypeDef(TypedDict):
    beginOffsetInclusive: NotRequired[int],
    endOffsetExclusive: NotRequired[int],
```

## ConnectConfigurationTypeDef

```python
# ConnectConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ConnectConfigurationTypeDef


def get_value() -> ConnectConfigurationTypeDef:
    return {
        "instanceId": ...,
    }


# ConnectConfigurationTypeDef definition

class ConnectConfigurationTypeDef(TypedDict):
    instanceId: NotRequired[str],
```

## RankingDataTypeDef

```python
# RankingDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import RankingDataTypeDef


def get_value() -> RankingDataTypeDef:
    return {
        "relevanceLevel": ...,
    }


# RankingDataTypeDef definition

class RankingDataTypeDef(TypedDict):
    relevanceLevel: NotRequired[RelevanceLevelType],  # (1)
    relevanceScore: NotRequired[float],
```

1. See [:material-code-brackets: RelevanceLevelType](./literals.md#relevanceleveltype) 
## ContentDataTypeDef

```python
# ContentDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ContentDataTypeDef


def get_value() -> ContentDataTypeDef:
    return {
        "contentArn": ...,
    }


# ContentDataTypeDef definition

class ContentDataTypeDef(TypedDict):
    contentArn: str,
    contentId: str,
    contentType: str,
    knowledgeBaseArn: str,
    knowledgeBaseId: str,
    metadata: Dict[str, str],
    name: str,
    revisionId: str,
    status: ContentStatusType,  # (1)
    title: str,
    url: str,
    urlExpiry: datetime,
    linkOutUri: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ContentStatusType](./literals.md#contentstatustype) 
## GenerativeContentFeedbackDataTypeDef

```python
# GenerativeContentFeedbackDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GenerativeContentFeedbackDataTypeDef


def get_value() -> GenerativeContentFeedbackDataTypeDef:
    return {
        "relevance": ...,
    }


# GenerativeContentFeedbackDataTypeDef definition

class GenerativeContentFeedbackDataTypeDef(TypedDict):
    relevance: RelevanceType,  # (1)
```

1. See [:material-code-brackets: RelevanceType](./literals.md#relevancetype) 
## ContentReferenceTypeDef

```python
# ContentReferenceTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ContentReferenceTypeDef


def get_value() -> ContentReferenceTypeDef:
    return {
        "contentArn": ...,
    }


# ContentReferenceTypeDef definition

class ContentReferenceTypeDef(TypedDict):
    contentArn: NotRequired[str],
    contentId: NotRequired[str],
    knowledgeBaseArn: NotRequired[str],
    knowledgeBaseId: NotRequired[str],
    referenceType: NotRequired[ReferenceTypeType],  # (1)
    sourceURL: NotRequired[str],
```

1. See [:material-code-brackets: ReferenceTypeType](./literals.md#referencetypetype) 
## ContentSummaryTypeDef

```python
# ContentSummaryTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ContentSummaryTypeDef


def get_value() -> ContentSummaryTypeDef:
    return {
        "contentArn": ...,
    }


# ContentSummaryTypeDef definition

class ContentSummaryTypeDef(TypedDict):
    contentArn: str,
    contentId: str,
    contentType: str,
    knowledgeBaseArn: str,
    knowledgeBaseId: str,
    metadata: Dict[str, str],
    name: str,
    revisionId: str,
    status: ContentStatusType,  # (1)
    title: str,
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ContentStatusType](./literals.md#contentstatustype) 
## SelfServiceConversationHistoryTypeDef

```python
# SelfServiceConversationHistoryTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SelfServiceConversationHistoryTypeDef


def get_value() -> SelfServiceConversationHistoryTypeDef:
    return {
        "botResponse": ...,
    }


# SelfServiceConversationHistoryTypeDef definition

class SelfServiceConversationHistoryTypeDef(TypedDict):
    turnNumber: int,
    botResponse: NotRequired[str],
    inputTranscript: NotRequired[str],
```

## ConversationStateTypeDef

```python
# ConversationStateTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ConversationStateTypeDef


def get_value() -> ConversationStateTypeDef:
    return {
        "reason": ...,
    }


# ConversationStateTypeDef definition

class ConversationStateTypeDef(TypedDict):
    status: ConversationStatusType,  # (2)
    reason: NotRequired[ConversationStatusReasonType],  # (1)
```

1. See [:material-code-brackets: ConversationStatusReasonType](./literals.md#conversationstatusreasontype) 
2. See [:material-code-brackets: ConversationStatusType](./literals.md#conversationstatustype) 
## CreateContentRequestTypeDef

```python
# CreateContentRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateContentRequestTypeDef


def get_value() -> CreateContentRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# CreateContentRequestTypeDef definition

class CreateContentRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    name: str,
    uploadId: str,
    clientToken: NotRequired[str],
    metadata: NotRequired[Mapping[str, str]],
    overrideLinkOutUri: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    title: NotRequired[str],
```

## RenderingConfigurationTypeDef

```python
# RenderingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import RenderingConfigurationTypeDef


def get_value() -> RenderingConfigurationTypeDef:
    return {
        "templateUri": ...,
    }


# RenderingConfigurationTypeDef definition

class RenderingConfigurationTypeDef(TypedDict):
    templateUri: NotRequired[str],
```

## CreateMessageTemplateAttachmentRequestTypeDef

```python
# CreateMessageTemplateAttachmentRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateMessageTemplateAttachmentRequestTypeDef


def get_value() -> CreateMessageTemplateAttachmentRequestTypeDef:
    return {
        "body": ...,
    }


# CreateMessageTemplateAttachmentRequestTypeDef definition

class CreateMessageTemplateAttachmentRequestTypeDef(TypedDict):
    body: str,
    contentDisposition: ContentDispositionType,  # (1)
    knowledgeBaseId: str,
    messageTemplateId: str,
    name: str,
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: ContentDispositionType](./literals.md#contentdispositiontype) 
## MessageTemplateAttachmentTypeDef

```python
# MessageTemplateAttachmentTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import MessageTemplateAttachmentTypeDef


def get_value() -> MessageTemplateAttachmentTypeDef:
    return {
        "attachmentId": ...,
    }


# MessageTemplateAttachmentTypeDef definition

class MessageTemplateAttachmentTypeDef(TypedDict):
    attachmentId: str,
    contentDisposition: ContentDispositionType,  # (1)
    name: str,
    uploadedTime: datetime,
    url: str,
    urlExpiry: datetime,
```

1. See [:material-code-brackets: ContentDispositionType](./literals.md#contentdispositiontype) 
## CreateMessageTemplateVersionRequestTypeDef

```python
# CreateMessageTemplateVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateMessageTemplateVersionRequestTypeDef


def get_value() -> CreateMessageTemplateVersionRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# CreateMessageTemplateVersionRequestTypeDef definition

class CreateMessageTemplateVersionRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    messageTemplateId: str,
    messageTemplateContentSha256: NotRequired[str],
```

## QuickResponseDataProviderTypeDef

```python
# QuickResponseDataProviderTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import QuickResponseDataProviderTypeDef


def get_value() -> QuickResponseDataProviderTypeDef:
    return {
        "content": ...,
    }


# QuickResponseDataProviderTypeDef definition

class QuickResponseDataProviderTypeDef(TypedDict):
    content: NotRequired[str],
```

## CustomerProfileAttributesOutputTypeDef

```python
# CustomerProfileAttributesOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CustomerProfileAttributesOutputTypeDef


def get_value() -> CustomerProfileAttributesOutputTypeDef:
    return {
        "accountNumber": ...,
    }


# CustomerProfileAttributesOutputTypeDef definition

class CustomerProfileAttributesOutputTypeDef(TypedDict):
    accountNumber: NotRequired[str],
    additionalInformation: NotRequired[str],
    address1: NotRequired[str],
    address2: NotRequired[str],
    address3: NotRequired[str],
    address4: NotRequired[str],
    billingAddress1: NotRequired[str],
    billingAddress2: NotRequired[str],
    billingAddress3: NotRequired[str],
    billingAddress4: NotRequired[str],
    billingCity: NotRequired[str],
    billingCountry: NotRequired[str],
    billingCounty: NotRequired[str],
    billingPostalCode: NotRequired[str],
    billingProvince: NotRequired[str],
    billingState: NotRequired[str],
    birthDate: NotRequired[str],
    businessEmailAddress: NotRequired[str],
    businessName: NotRequired[str],
    businessPhoneNumber: NotRequired[str],
    city: NotRequired[str],
    country: NotRequired[str],
    county: NotRequired[str],
    custom: NotRequired[Dict[str, str]],
    emailAddress: NotRequired[str],
    firstName: NotRequired[str],
    gender: NotRequired[str],
    homePhoneNumber: NotRequired[str],
    lastName: NotRequired[str],
    mailingAddress1: NotRequired[str],
    mailingAddress2: NotRequired[str],
    mailingAddress3: NotRequired[str],
    mailingAddress4: NotRequired[str],
    mailingCity: NotRequired[str],
    mailingCountry: NotRequired[str],
    mailingCounty: NotRequired[str],
    mailingPostalCode: NotRequired[str],
    mailingProvince: NotRequired[str],
    mailingState: NotRequired[str],
    middleName: NotRequired[str],
    mobilePhoneNumber: NotRequired[str],
    partyType: NotRequired[str],
    phoneNumber: NotRequired[str],
    postalCode: NotRequired[str],
    profileARN: NotRequired[str],
    profileId: NotRequired[str],
    province: NotRequired[str],
    shippingAddress1: NotRequired[str],
    shippingAddress2: NotRequired[str],
    shippingAddress3: NotRequired[str],
    shippingAddress4: NotRequired[str],
    shippingCity: NotRequired[str],
    shippingCountry: NotRequired[str],
    shippingCounty: NotRequired[str],
    shippingPostalCode: NotRequired[str],
    shippingProvince: NotRequired[str],
    shippingState: NotRequired[str],
    state: NotRequired[str],
```

## CustomerProfileAttributesTypeDef

```python
# CustomerProfileAttributesTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CustomerProfileAttributesTypeDef


def get_value() -> CustomerProfileAttributesTypeDef:
    return {
        "accountNumber": ...,
    }


# CustomerProfileAttributesTypeDef definition

class CustomerProfileAttributesTypeDef(TypedDict):
    accountNumber: NotRequired[str],
    additionalInformation: NotRequired[str],
    address1: NotRequired[str],
    address2: NotRequired[str],
    address3: NotRequired[str],
    address4: NotRequired[str],
    billingAddress1: NotRequired[str],
    billingAddress2: NotRequired[str],
    billingAddress3: NotRequired[str],
    billingAddress4: NotRequired[str],
    billingCity: NotRequired[str],
    billingCountry: NotRequired[str],
    billingCounty: NotRequired[str],
    billingPostalCode: NotRequired[str],
    billingProvince: NotRequired[str],
    billingState: NotRequired[str],
    birthDate: NotRequired[str],
    businessEmailAddress: NotRequired[str],
    businessName: NotRequired[str],
    businessPhoneNumber: NotRequired[str],
    city: NotRequired[str],
    country: NotRequired[str],
    county: NotRequired[str],
    custom: NotRequired[Mapping[str, str]],
    emailAddress: NotRequired[str],
    firstName: NotRequired[str],
    gender: NotRequired[str],
    homePhoneNumber: NotRequired[str],
    lastName: NotRequired[str],
    mailingAddress1: NotRequired[str],
    mailingAddress2: NotRequired[str],
    mailingAddress3: NotRequired[str],
    mailingAddress4: NotRequired[str],
    mailingCity: NotRequired[str],
    mailingCountry: NotRequired[str],
    mailingCounty: NotRequired[str],
    mailingPostalCode: NotRequired[str],
    mailingProvince: NotRequired[str],
    mailingState: NotRequired[str],
    middleName: NotRequired[str],
    mobilePhoneNumber: NotRequired[str],
    partyType: NotRequired[str],
    phoneNumber: NotRequired[str],
    postalCode: NotRequired[str],
    profileARN: NotRequired[str],
    profileId: NotRequired[str],
    province: NotRequired[str],
    shippingAddress1: NotRequired[str],
    shippingAddress2: NotRequired[str],
    shippingAddress3: NotRequired[str],
    shippingAddress4: NotRequired[str],
    shippingCity: NotRequired[str],
    shippingCountry: NotRequired[str],
    shippingCounty: NotRequired[str],
    shippingPostalCode: NotRequired[str],
    shippingProvince: NotRequired[str],
    shippingState: NotRequired[str],
    state: NotRequired[str],
```

## IntentDetectedDataDetailsTypeDef

```python
# IntentDetectedDataDetailsTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import IntentDetectedDataDetailsTypeDef


def get_value() -> IntentDetectedDataDetailsTypeDef:
    return {
        "intent": ...,
    }


# IntentDetectedDataDetailsTypeDef definition

class IntentDetectedDataDetailsTypeDef(TypedDict):
    intent: str,
    intentId: str,
```

## GenerativeReferenceTypeDef

```python
# GenerativeReferenceTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GenerativeReferenceTypeDef


def get_value() -> GenerativeReferenceTypeDef:
    return {
        "generationId": ...,
    }


# GenerativeReferenceTypeDef definition

class GenerativeReferenceTypeDef(TypedDict):
    generationId: NotRequired[str],
    modelId: NotRequired[str],
```

## DeactivateMessageTemplateRequestTypeDef

```python
# DeactivateMessageTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DeactivateMessageTemplateRequestTypeDef


def get_value() -> DeactivateMessageTemplateRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# DeactivateMessageTemplateRequestTypeDef definition

class DeactivateMessageTemplateRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    messageTemplateId: str,
    versionNumber: int,
```

## DeleteAIAgentRequestTypeDef

```python
# DeleteAIAgentRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DeleteAIAgentRequestTypeDef


def get_value() -> DeleteAIAgentRequestTypeDef:
    return {
        "aiAgentId": ...,
    }


# DeleteAIAgentRequestTypeDef definition

class DeleteAIAgentRequestTypeDef(TypedDict):
    aiAgentId: str,
    assistantId: str,
```

## DeleteAIAgentVersionRequestTypeDef

```python
# DeleteAIAgentVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DeleteAIAgentVersionRequestTypeDef


def get_value() -> DeleteAIAgentVersionRequestTypeDef:
    return {
        "aiAgentId": ...,
    }


# DeleteAIAgentVersionRequestTypeDef definition

class DeleteAIAgentVersionRequestTypeDef(TypedDict):
    aiAgentId: str,
    assistantId: str,
    versionNumber: int,
```

## DeleteAIGuardrailRequestTypeDef

```python
# DeleteAIGuardrailRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DeleteAIGuardrailRequestTypeDef


def get_value() -> DeleteAIGuardrailRequestTypeDef:
    return {
        "aiGuardrailId": ...,
    }


# DeleteAIGuardrailRequestTypeDef definition

class DeleteAIGuardrailRequestTypeDef(TypedDict):
    aiGuardrailId: str,
    assistantId: str,
```

## DeleteAIGuardrailVersionRequestTypeDef

```python
# DeleteAIGuardrailVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DeleteAIGuardrailVersionRequestTypeDef


def get_value() -> DeleteAIGuardrailVersionRequestTypeDef:
    return {
        "aiGuardrailId": ...,
    }


# DeleteAIGuardrailVersionRequestTypeDef definition

class DeleteAIGuardrailVersionRequestTypeDef(TypedDict):
    aiGuardrailId: str,
    assistantId: str,
    versionNumber: int,
```

## DeleteAIPromptRequestTypeDef

```python
# DeleteAIPromptRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DeleteAIPromptRequestTypeDef


def get_value() -> DeleteAIPromptRequestTypeDef:
    return {
        "aiPromptId": ...,
    }


# DeleteAIPromptRequestTypeDef definition

class DeleteAIPromptRequestTypeDef(TypedDict):
    aiPromptId: str,
    assistantId: str,
```

## DeleteAIPromptVersionRequestTypeDef

```python
# DeleteAIPromptVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DeleteAIPromptVersionRequestTypeDef


def get_value() -> DeleteAIPromptVersionRequestTypeDef:
    return {
        "aiPromptId": ...,
    }


# DeleteAIPromptVersionRequestTypeDef definition

class DeleteAIPromptVersionRequestTypeDef(TypedDict):
    aiPromptId: str,
    assistantId: str,
    versionNumber: int,
```

## DeleteAssistantAssociationRequestTypeDef

```python
# DeleteAssistantAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DeleteAssistantAssociationRequestTypeDef


def get_value() -> DeleteAssistantAssociationRequestTypeDef:
    return {
        "assistantAssociationId": ...,
    }


# DeleteAssistantAssociationRequestTypeDef definition

class DeleteAssistantAssociationRequestTypeDef(TypedDict):
    assistantAssociationId: str,
    assistantId: str,
```

## DeleteAssistantRequestTypeDef

```python
# DeleteAssistantRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DeleteAssistantRequestTypeDef


def get_value() -> DeleteAssistantRequestTypeDef:
    return {
        "assistantId": ...,
    }


# DeleteAssistantRequestTypeDef definition

class DeleteAssistantRequestTypeDef(TypedDict):
    assistantId: str,
```

## DeleteContentAssociationRequestTypeDef

```python
# DeleteContentAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DeleteContentAssociationRequestTypeDef


def get_value() -> DeleteContentAssociationRequestTypeDef:
    return {
        "contentAssociationId": ...,
    }


# DeleteContentAssociationRequestTypeDef definition

class DeleteContentAssociationRequestTypeDef(TypedDict):
    contentAssociationId: str,
    contentId: str,
    knowledgeBaseId: str,
```

## DeleteContentRequestTypeDef

```python
# DeleteContentRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DeleteContentRequestTypeDef


def get_value() -> DeleteContentRequestTypeDef:
    return {
        "contentId": ...,
    }


# DeleteContentRequestTypeDef definition

class DeleteContentRequestTypeDef(TypedDict):
    contentId: str,
    knowledgeBaseId: str,
```

## DeleteImportJobRequestTypeDef

```python
# DeleteImportJobRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DeleteImportJobRequestTypeDef


def get_value() -> DeleteImportJobRequestTypeDef:
    return {
        "importJobId": ...,
    }


# DeleteImportJobRequestTypeDef definition

class DeleteImportJobRequestTypeDef(TypedDict):
    importJobId: str,
    knowledgeBaseId: str,
```

## DeleteKnowledgeBaseRequestTypeDef

```python
# DeleteKnowledgeBaseRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DeleteKnowledgeBaseRequestTypeDef


def get_value() -> DeleteKnowledgeBaseRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# DeleteKnowledgeBaseRequestTypeDef definition

class DeleteKnowledgeBaseRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
```

## DeleteMessageTemplateAttachmentRequestTypeDef

```python
# DeleteMessageTemplateAttachmentRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DeleteMessageTemplateAttachmentRequestTypeDef


def get_value() -> DeleteMessageTemplateAttachmentRequestTypeDef:
    return {
        "attachmentId": ...,
    }


# DeleteMessageTemplateAttachmentRequestTypeDef definition

class DeleteMessageTemplateAttachmentRequestTypeDef(TypedDict):
    attachmentId: str,
    knowledgeBaseId: str,
    messageTemplateId: str,
```

## DeleteMessageTemplateRequestTypeDef

```python
# DeleteMessageTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DeleteMessageTemplateRequestTypeDef


def get_value() -> DeleteMessageTemplateRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# DeleteMessageTemplateRequestTypeDef definition

class DeleteMessageTemplateRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    messageTemplateId: str,
```

## DeleteQuickResponseRequestTypeDef

```python
# DeleteQuickResponseRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DeleteQuickResponseRequestTypeDef


def get_value() -> DeleteQuickResponseRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# DeleteQuickResponseRequestTypeDef definition

class DeleteQuickResponseRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    quickResponseId: str,
```

## HighlightTypeDef

```python
# HighlightTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import HighlightTypeDef


def get_value() -> HighlightTypeDef:
    return {
        "beginOffsetInclusive": ...,
    }


# HighlightTypeDef definition

class HighlightTypeDef(TypedDict):
    beginOffsetInclusive: NotRequired[int],
    endOffsetExclusive: NotRequired[int],
```

## EmailHeaderTypeDef

```python
# EmailHeaderTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import EmailHeaderTypeDef


def get_value() -> EmailHeaderTypeDef:
    return {
        "name": ...,
    }


# EmailHeaderTypeDef definition

class EmailHeaderTypeDef(TypedDict):
    name: NotRequired[str],
    value: NotRequired[str],
```

## MessageTemplateBodyContentProviderTypeDef

```python
# MessageTemplateBodyContentProviderTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import MessageTemplateBodyContentProviderTypeDef


def get_value() -> MessageTemplateBodyContentProviderTypeDef:
    return {
        "content": ...,
    }


# MessageTemplateBodyContentProviderTypeDef definition

class MessageTemplateBodyContentProviderTypeDef(TypedDict):
    content: NotRequired[str],
```

## GroupingConfigurationOutputTypeDef

```python
# GroupingConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GroupingConfigurationOutputTypeDef


def get_value() -> GroupingConfigurationOutputTypeDef:
    return {
        "criteria": ...,
    }


# GroupingConfigurationOutputTypeDef definition

class GroupingConfigurationOutputTypeDef(TypedDict):
    criteria: NotRequired[str],
    values: NotRequired[List[str]],
```

## FilterTypeDef

```python
# FilterTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import FilterTypeDef


def get_value() -> FilterTypeDef:
    return {
        "field": ...,
    }


# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    field: FilterFieldType,  # (1)
    operator: FilterOperatorType,  # (2)
    value: str,
```

1. See [:material-code-brackets: FilterFieldType](./literals.md#filterfieldtype) 
2. See [:material-code-brackets: FilterOperatorType](./literals.md#filteroperatortype) 
## GetAIAgentRequestTypeDef

```python
# GetAIAgentRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetAIAgentRequestTypeDef


def get_value() -> GetAIAgentRequestTypeDef:
    return {
        "aiAgentId": ...,
    }


# GetAIAgentRequestTypeDef definition

class GetAIAgentRequestTypeDef(TypedDict):
    aiAgentId: str,
    assistantId: str,
```

## GetAIGuardrailRequestTypeDef

```python
# GetAIGuardrailRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetAIGuardrailRequestTypeDef


def get_value() -> GetAIGuardrailRequestTypeDef:
    return {
        "aiGuardrailId": ...,
    }


# GetAIGuardrailRequestTypeDef definition

class GetAIGuardrailRequestTypeDef(TypedDict):
    aiGuardrailId: str,
    assistantId: str,
```

## GetAIPromptRequestTypeDef

```python
# GetAIPromptRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetAIPromptRequestTypeDef


def get_value() -> GetAIPromptRequestTypeDef:
    return {
        "aiPromptId": ...,
    }


# GetAIPromptRequestTypeDef definition

class GetAIPromptRequestTypeDef(TypedDict):
    aiPromptId: str,
    assistantId: str,
```

## GetAssistantAssociationRequestTypeDef

```python
# GetAssistantAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetAssistantAssociationRequestTypeDef


def get_value() -> GetAssistantAssociationRequestTypeDef:
    return {
        "assistantAssociationId": ...,
    }


# GetAssistantAssociationRequestTypeDef definition

class GetAssistantAssociationRequestTypeDef(TypedDict):
    assistantAssociationId: str,
    assistantId: str,
```

## GetAssistantRequestTypeDef

```python
# GetAssistantRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetAssistantRequestTypeDef


def get_value() -> GetAssistantRequestTypeDef:
    return {
        "assistantId": ...,
    }


# GetAssistantRequestTypeDef definition

class GetAssistantRequestTypeDef(TypedDict):
    assistantId: str,
```

## GetContentAssociationRequestTypeDef

```python
# GetContentAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetContentAssociationRequestTypeDef


def get_value() -> GetContentAssociationRequestTypeDef:
    return {
        "contentAssociationId": ...,
    }


# GetContentAssociationRequestTypeDef definition

class GetContentAssociationRequestTypeDef(TypedDict):
    contentAssociationId: str,
    contentId: str,
    knowledgeBaseId: str,
```

## GetContentRequestTypeDef

```python
# GetContentRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetContentRequestTypeDef


def get_value() -> GetContentRequestTypeDef:
    return {
        "contentId": ...,
    }


# GetContentRequestTypeDef definition

class GetContentRequestTypeDef(TypedDict):
    contentId: str,
    knowledgeBaseId: str,
```

## GetContentSummaryRequestTypeDef

```python
# GetContentSummaryRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetContentSummaryRequestTypeDef


def get_value() -> GetContentSummaryRequestTypeDef:
    return {
        "contentId": ...,
    }


# GetContentSummaryRequestTypeDef definition

class GetContentSummaryRequestTypeDef(TypedDict):
    contentId: str,
    knowledgeBaseId: str,
```

## GetImportJobRequestTypeDef

```python
# GetImportJobRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetImportJobRequestTypeDef


def get_value() -> GetImportJobRequestTypeDef:
    return {
        "importJobId": ...,
    }


# GetImportJobRequestTypeDef definition

class GetImportJobRequestTypeDef(TypedDict):
    importJobId: str,
    knowledgeBaseId: str,
```

## GetKnowledgeBaseRequestTypeDef

```python
# GetKnowledgeBaseRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetKnowledgeBaseRequestTypeDef


def get_value() -> GetKnowledgeBaseRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# GetKnowledgeBaseRequestTypeDef definition

class GetKnowledgeBaseRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
```

## GetMessageTemplateRequestTypeDef

```python
# GetMessageTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetMessageTemplateRequestTypeDef


def get_value() -> GetMessageTemplateRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# GetMessageTemplateRequestTypeDef definition

class GetMessageTemplateRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    messageTemplateId: str,
```

## GetNextMessageRequestTypeDef

```python
# GetNextMessageRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetNextMessageRequestTypeDef


def get_value() -> GetNextMessageRequestTypeDef:
    return {
        "assistantId": ...,
    }


# GetNextMessageRequestTypeDef definition

class GetNextMessageRequestTypeDef(TypedDict):
    assistantId: str,
    nextMessageToken: str,
    sessionId: str,
```

## GetQuickResponseRequestTypeDef

```python
# GetQuickResponseRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetQuickResponseRequestTypeDef


def get_value() -> GetQuickResponseRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# GetQuickResponseRequestTypeDef definition

class GetQuickResponseRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    quickResponseId: str,
```

## GetRecommendationsRequestTypeDef

```python
# GetRecommendationsRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetRecommendationsRequestTypeDef


def get_value() -> GetRecommendationsRequestTypeDef:
    return {
        "assistantId": ...,
    }


# GetRecommendationsRequestTypeDef definition

class GetRecommendationsRequestTypeDef(TypedDict):
    assistantId: str,
    sessionId: str,
    maxResults: NotRequired[int],
    waitTimeSeconds: NotRequired[int],
```

## GetSessionRequestTypeDef

```python
# GetSessionRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetSessionRequestTypeDef


def get_value() -> GetSessionRequestTypeDef:
    return {
        "assistantId": ...,
    }


# GetSessionRequestTypeDef definition

class GetSessionRequestTypeDef(TypedDict):
    assistantId: str,
    sessionId: str,
```

## GroupingConfigurationTypeDef

```python
# GroupingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GroupingConfigurationTypeDef


def get_value() -> GroupingConfigurationTypeDef:
    return {
        "criteria": ...,
    }


# GroupingConfigurationTypeDef definition

class GroupingConfigurationTypeDef(TypedDict):
    criteria: NotRequired[str],
    values: NotRequired[Sequence[str]],
```

## HierarchicalChunkingLevelConfigurationTypeDef

```python
# HierarchicalChunkingLevelConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import HierarchicalChunkingLevelConfigurationTypeDef


def get_value() -> HierarchicalChunkingLevelConfigurationTypeDef:
    return {
        "maxTokens": ...,
    }


# HierarchicalChunkingLevelConfigurationTypeDef definition

class HierarchicalChunkingLevelConfigurationTypeDef(TypedDict):
    maxTokens: int,
```

## IntentInputDataTypeDef

```python
# IntentInputDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import IntentInputDataTypeDef


def get_value() -> IntentInputDataTypeDef:
    return {
        "intentId": ...,
    }


# IntentInputDataTypeDef definition

class IntentInputDataTypeDef(TypedDict):
    intentId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import PaginatorConfigTypeDef


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

## ListAIAgentVersionsRequestTypeDef

```python
# ListAIAgentVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAIAgentVersionsRequestTypeDef


def get_value() -> ListAIAgentVersionsRequestTypeDef:
    return {
        "aiAgentId": ...,
    }


# ListAIAgentVersionsRequestTypeDef definition

class ListAIAgentVersionsRequestTypeDef(TypedDict):
    aiAgentId: str,
    assistantId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    origin: NotRequired[OriginType],  # (1)
```

1. See [:material-code-brackets: OriginType](./literals.md#origintype) 
## ListAIAgentsRequestTypeDef

```python
# ListAIAgentsRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAIAgentsRequestTypeDef


def get_value() -> ListAIAgentsRequestTypeDef:
    return {
        "assistantId": ...,
    }


# ListAIAgentsRequestTypeDef definition

class ListAIAgentsRequestTypeDef(TypedDict):
    assistantId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    origin: NotRequired[OriginType],  # (1)
```

1. See [:material-code-brackets: OriginType](./literals.md#origintype) 
## ListAIGuardrailVersionsRequestTypeDef

```python
# ListAIGuardrailVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAIGuardrailVersionsRequestTypeDef


def get_value() -> ListAIGuardrailVersionsRequestTypeDef:
    return {
        "aiGuardrailId": ...,
    }


# ListAIGuardrailVersionsRequestTypeDef definition

class ListAIGuardrailVersionsRequestTypeDef(TypedDict):
    aiGuardrailId: str,
    assistantId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAIGuardrailsRequestTypeDef

```python
# ListAIGuardrailsRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAIGuardrailsRequestTypeDef


def get_value() -> ListAIGuardrailsRequestTypeDef:
    return {
        "assistantId": ...,
    }


# ListAIGuardrailsRequestTypeDef definition

class ListAIGuardrailsRequestTypeDef(TypedDict):
    assistantId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAIPromptVersionsRequestTypeDef

```python
# ListAIPromptVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAIPromptVersionsRequestTypeDef


def get_value() -> ListAIPromptVersionsRequestTypeDef:
    return {
        "aiPromptId": ...,
    }


# ListAIPromptVersionsRequestTypeDef definition

class ListAIPromptVersionsRequestTypeDef(TypedDict):
    aiPromptId: str,
    assistantId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    origin: NotRequired[OriginType],  # (1)
```

1. See [:material-code-brackets: OriginType](./literals.md#origintype) 
## ListAIPromptsRequestTypeDef

```python
# ListAIPromptsRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAIPromptsRequestTypeDef


def get_value() -> ListAIPromptsRequestTypeDef:
    return {
        "assistantId": ...,
    }


# ListAIPromptsRequestTypeDef definition

class ListAIPromptsRequestTypeDef(TypedDict):
    assistantId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    origin: NotRequired[OriginType],  # (1)
```

1. See [:material-code-brackets: OriginType](./literals.md#origintype) 
## ListAssistantAssociationsRequestTypeDef

```python
# ListAssistantAssociationsRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAssistantAssociationsRequestTypeDef


def get_value() -> ListAssistantAssociationsRequestTypeDef:
    return {
        "assistantId": ...,
    }


# ListAssistantAssociationsRequestTypeDef definition

class ListAssistantAssociationsRequestTypeDef(TypedDict):
    assistantId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAssistantsRequestTypeDef

```python
# ListAssistantsRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAssistantsRequestTypeDef


def get_value() -> ListAssistantsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListAssistantsRequestTypeDef definition

class ListAssistantsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListContentAssociationsRequestTypeDef

```python
# ListContentAssociationsRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListContentAssociationsRequestTypeDef


def get_value() -> ListContentAssociationsRequestTypeDef:
    return {
        "contentId": ...,
    }


# ListContentAssociationsRequestTypeDef definition

class ListContentAssociationsRequestTypeDef(TypedDict):
    contentId: str,
    knowledgeBaseId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListContentsRequestTypeDef

```python
# ListContentsRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListContentsRequestTypeDef


def get_value() -> ListContentsRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# ListContentsRequestTypeDef definition

class ListContentsRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListImportJobsRequestTypeDef

```python
# ListImportJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListImportJobsRequestTypeDef


def get_value() -> ListImportJobsRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# ListImportJobsRequestTypeDef definition

class ListImportJobsRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListKnowledgeBasesRequestTypeDef

```python
# ListKnowledgeBasesRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListKnowledgeBasesRequestTypeDef


def get_value() -> ListKnowledgeBasesRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListKnowledgeBasesRequestTypeDef definition

class ListKnowledgeBasesRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListMessageTemplateVersionsRequestTypeDef

```python
# ListMessageTemplateVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListMessageTemplateVersionsRequestTypeDef


def get_value() -> ListMessageTemplateVersionsRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# ListMessageTemplateVersionsRequestTypeDef definition

class ListMessageTemplateVersionsRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    messageTemplateId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## MessageTemplateVersionSummaryTypeDef

```python
# MessageTemplateVersionSummaryTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import MessageTemplateVersionSummaryTypeDef


def get_value() -> MessageTemplateVersionSummaryTypeDef:
    return {
        "channelSubtype": ...,
    }


# MessageTemplateVersionSummaryTypeDef definition

class MessageTemplateVersionSummaryTypeDef(TypedDict):
    channelSubtype: ChannelSubtypeType,  # (1)
    isActive: bool,
    knowledgeBaseArn: str,
    knowledgeBaseId: str,
    messageTemplateArn: str,
    messageTemplateId: str,
    name: str,
    versionNumber: int,
```

1. See [:material-code-brackets: ChannelSubtypeType](./literals.md#channelsubtypetype) 
## ListMessageTemplatesRequestTypeDef

```python
# ListMessageTemplatesRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListMessageTemplatesRequestTypeDef


def get_value() -> ListMessageTemplatesRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# ListMessageTemplatesRequestTypeDef definition

class ListMessageTemplatesRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## MessageTemplateSummaryTypeDef

```python
# MessageTemplateSummaryTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import MessageTemplateSummaryTypeDef


def get_value() -> MessageTemplateSummaryTypeDef:
    return {
        "activeVersionNumber": ...,
    }


# MessageTemplateSummaryTypeDef definition

class MessageTemplateSummaryTypeDef(TypedDict):
    channelSubtype: ChannelSubtypeType,  # (1)
    createdTime: datetime,
    knowledgeBaseArn: str,
    knowledgeBaseId: str,
    lastModifiedBy: str,
    lastModifiedTime: datetime,
    messageTemplateArn: str,
    messageTemplateId: str,
    name: str,
    activeVersionNumber: NotRequired[int],
    description: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ChannelSubtypeType](./literals.md#channelsubtypetype) 
## ListMessagesRequestTypeDef

```python
# ListMessagesRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListMessagesRequestTypeDef


def get_value() -> ListMessagesRequestTypeDef:
    return {
        "assistantId": ...,
    }


# ListMessagesRequestTypeDef definition

class ListMessagesRequestTypeDef(TypedDict):
    assistantId: str,
    sessionId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListQuickResponsesRequestTypeDef

```python
# ListQuickResponsesRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListQuickResponsesRequestTypeDef


def get_value() -> ListQuickResponsesRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# ListQuickResponsesRequestTypeDef definition

class ListQuickResponsesRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## QuickResponseSummaryTypeDef

```python
# QuickResponseSummaryTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import QuickResponseSummaryTypeDef


def get_value() -> QuickResponseSummaryTypeDef:
    return {
        "channels": ...,
    }


# QuickResponseSummaryTypeDef definition

class QuickResponseSummaryTypeDef(TypedDict):
    contentType: str,
    createdTime: datetime,
    knowledgeBaseArn: str,
    knowledgeBaseId: str,
    lastModifiedTime: datetime,
    name: str,
    quickResponseArn: str,
    quickResponseId: str,
    status: QuickResponseStatusType,  # (1)
    channels: NotRequired[List[str]],
    description: NotRequired[str],
    isActive: NotRequired[bool],
    lastModifiedBy: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: QuickResponseStatusType](./literals.md#quickresponsestatustype) 
## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## TextMessageTypeDef

```python
# TextMessageTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import TextMessageTypeDef


def get_value() -> TextMessageTypeDef:
    return {
        "value": ...,
    }


# TextMessageTypeDef definition

class TextMessageTypeDef(TypedDict):
    value: NotRequired[str],
```

## MessageTemplateFilterFieldTypeDef

```python
# MessageTemplateFilterFieldTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import MessageTemplateFilterFieldTypeDef


def get_value() -> MessageTemplateFilterFieldTypeDef:
    return {
        "includeNoExistence": ...,
    }


# MessageTemplateFilterFieldTypeDef definition

class MessageTemplateFilterFieldTypeDef(TypedDict):
    name: str,
    operator: MessageTemplateFilterOperatorType,  # (1)
    includeNoExistence: NotRequired[bool],
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: MessageTemplateFilterOperatorType](./literals.md#messagetemplatefilteroperatortype) 
## MessageTemplateOrderFieldTypeDef

```python
# MessageTemplateOrderFieldTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import MessageTemplateOrderFieldTypeDef


def get_value() -> MessageTemplateOrderFieldTypeDef:
    return {
        "name": ...,
    }


# MessageTemplateOrderFieldTypeDef definition

class MessageTemplateOrderFieldTypeDef(TypedDict):
    name: str,
    order: NotRequired[OrderType],  # (1)
```

1. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
## MessageTemplateQueryFieldTypeDef

```python
# MessageTemplateQueryFieldTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import MessageTemplateQueryFieldTypeDef


def get_value() -> MessageTemplateQueryFieldTypeDef:
    return {
        "allowFuzziness": ...,
    }


# MessageTemplateQueryFieldTypeDef definition

class MessageTemplateQueryFieldTypeDef(TypedDict):
    name: str,
    operator: MessageTemplateQueryOperatorType,  # (1)
    values: Sequence[str],
    allowFuzziness: NotRequired[bool],
    priority: NotRequired[PriorityType],  # (2)
```

1. See [:material-code-brackets: MessageTemplateQueryOperatorType](./literals.md#messagetemplatequeryoperatortype) 
2. See [:material-code-brackets: PriorityType](./literals.md#prioritytype) 
## NotifyRecommendationsReceivedErrorTypeDef

```python
# NotifyRecommendationsReceivedErrorTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import NotifyRecommendationsReceivedErrorTypeDef


def get_value() -> NotifyRecommendationsReceivedErrorTypeDef:
    return {
        "message": ...,
    }


# NotifyRecommendationsReceivedErrorTypeDef definition

class NotifyRecommendationsReceivedErrorTypeDef(TypedDict):
    message: NotRequired[str],
    recommendationId: NotRequired[str],
```

## NotifyRecommendationsReceivedRequestTypeDef

```python
# NotifyRecommendationsReceivedRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import NotifyRecommendationsReceivedRequestTypeDef


def get_value() -> NotifyRecommendationsReceivedRequestTypeDef:
    return {
        "assistantId": ...,
    }


# NotifyRecommendationsReceivedRequestTypeDef definition

class NotifyRecommendationsReceivedRequestTypeDef(TypedDict):
    assistantId: str,
    recommendationIds: Sequence[str],
    sessionId: str,
```

## TagConditionTypeDef

```python
# TagConditionTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import TagConditionTypeDef


def get_value() -> TagConditionTypeDef:
    return {
        "key": ...,
    }


# TagConditionTypeDef definition

class TagConditionTypeDef(TypedDict):
    key: str,
    value: NotRequired[str],
```

## QueryConditionItemTypeDef

```python
# QueryConditionItemTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import QueryConditionItemTypeDef


def get_value() -> QueryConditionItemTypeDef:
    return {
        "comparator": ...,
    }


# QueryConditionItemTypeDef definition

class QueryConditionItemTypeDef(TypedDict):
    comparator: QueryConditionComparisonOperatorType,  # (1)
    field: QueryConditionFieldNameType,  # (2)
    value: str,
```

1. See [:material-code-brackets: QueryConditionComparisonOperatorType](./literals.md#queryconditioncomparisonoperatortype) 
2. See [:material-code-brackets: QueryConditionFieldNameType](./literals.md#queryconditionfieldnametype) 
## QueryTextInputDataTypeDef

```python
# QueryTextInputDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import QueryTextInputDataTypeDef


def get_value() -> QueryTextInputDataTypeDef:
    return {
        "text": ...,
    }


# QueryTextInputDataTypeDef definition

class QueryTextInputDataTypeDef(TypedDict):
    text: str,
```

## QueryRecommendationTriggerDataTypeDef

```python
# QueryRecommendationTriggerDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import QueryRecommendationTriggerDataTypeDef


def get_value() -> QueryRecommendationTriggerDataTypeDef:
    return {
        "text": ...,
    }


# QueryRecommendationTriggerDataTypeDef definition

class QueryRecommendationTriggerDataTypeDef(TypedDict):
    text: NotRequired[str],
```

## QuickResponseContentProviderTypeDef

```python
# QuickResponseContentProviderTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import QuickResponseContentProviderTypeDef


def get_value() -> QuickResponseContentProviderTypeDef:
    return {
        "content": ...,
    }


# QuickResponseContentProviderTypeDef definition

class QuickResponseContentProviderTypeDef(TypedDict):
    content: NotRequired[str],
```

## QuickResponseFilterFieldTypeDef

```python
# QuickResponseFilterFieldTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import QuickResponseFilterFieldTypeDef


def get_value() -> QuickResponseFilterFieldTypeDef:
    return {
        "includeNoExistence": ...,
    }


# QuickResponseFilterFieldTypeDef definition

class QuickResponseFilterFieldTypeDef(TypedDict):
    name: str,
    operator: QuickResponseFilterOperatorType,  # (1)
    includeNoExistence: NotRequired[bool],
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: QuickResponseFilterOperatorType](./literals.md#quickresponsefilteroperatortype) 
## QuickResponseOrderFieldTypeDef

```python
# QuickResponseOrderFieldTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import QuickResponseOrderFieldTypeDef


def get_value() -> QuickResponseOrderFieldTypeDef:
    return {
        "name": ...,
    }


# QuickResponseOrderFieldTypeDef definition

class QuickResponseOrderFieldTypeDef(TypedDict):
    name: str,
    order: NotRequired[OrderType],  # (1)
```

1. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
## QuickResponseQueryFieldTypeDef

```python
# QuickResponseQueryFieldTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import QuickResponseQueryFieldTypeDef


def get_value() -> QuickResponseQueryFieldTypeDef:
    return {
        "allowFuzziness": ...,
    }


# QuickResponseQueryFieldTypeDef definition

class QuickResponseQueryFieldTypeDef(TypedDict):
    name: str,
    operator: QuickResponseQueryOperatorType,  # (1)
    values: Sequence[str],
    allowFuzziness: NotRequired[bool],
    priority: NotRequired[PriorityType],  # (2)
```

1. See [:material-code-brackets: QuickResponseQueryOperatorType](./literals.md#quickresponsequeryoperatortype) 
2. See [:material-code-brackets: PriorityType](./literals.md#prioritytype) 
## RemoveAssistantAIAgentRequestTypeDef

```python
# RemoveAssistantAIAgentRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import RemoveAssistantAIAgentRequestTypeDef


def get_value() -> RemoveAssistantAIAgentRequestTypeDef:
    return {
        "aiAgentType": ...,
    }


# RemoveAssistantAIAgentRequestTypeDef definition

class RemoveAssistantAIAgentRequestTypeDef(TypedDict):
    aiAgentType: AIAgentTypeType,  # (1)
    assistantId: str,
```

1. See [:material-code-brackets: AIAgentTypeType](./literals.md#aiagenttypetype) 
## RemoveKnowledgeBaseTemplateUriRequestTypeDef

```python
# RemoveKnowledgeBaseTemplateUriRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import RemoveKnowledgeBaseTemplateUriRequestTypeDef


def get_value() -> RemoveKnowledgeBaseTemplateUriRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# RemoveKnowledgeBaseTemplateUriRequestTypeDef definition

class RemoveKnowledgeBaseTemplateUriRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
```

## RuntimeSessionDataValueTypeDef

```python
# RuntimeSessionDataValueTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import RuntimeSessionDataValueTypeDef


def get_value() -> RuntimeSessionDataValueTypeDef:
    return {
        "stringValue": ...,
    }


# RuntimeSessionDataValueTypeDef definition

class RuntimeSessionDataValueTypeDef(TypedDict):
    stringValue: NotRequired[str],
```

## SessionSummaryTypeDef

```python
# SessionSummaryTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SessionSummaryTypeDef


def get_value() -> SessionSummaryTypeDef:
    return {
        "assistantArn": ...,
    }


# SessionSummaryTypeDef definition

class SessionSummaryTypeDef(TypedDict):
    assistantArn: str,
    assistantId: str,
    sessionArn: str,
    sessionId: str,
```

## SeedUrlTypeDef

```python
# SeedUrlTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SeedUrlTypeDef


def get_value() -> SeedUrlTypeDef:
    return {
        "url": ...,
    }


# SeedUrlTypeDef definition

class SeedUrlTypeDef(TypedDict):
    url: NotRequired[str],
```

## SessionIntegrationConfigurationTypeDef

```python
# SessionIntegrationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SessionIntegrationConfigurationTypeDef


def get_value() -> SessionIntegrationConfigurationTypeDef:
    return {
        "topicIntegrationArn": ...,
    }


# SessionIntegrationConfigurationTypeDef definition

class SessionIntegrationConfigurationTypeDef(TypedDict):
    topicIntegrationArn: NotRequired[str],
```

## StartContentUploadRequestTypeDef

```python
# StartContentUploadRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import StartContentUploadRequestTypeDef


def get_value() -> StartContentUploadRequestTypeDef:
    return {
        "contentType": ...,
    }


# StartContentUploadRequestTypeDef definition

class StartContentUploadRequestTypeDef(TypedDict):
    contentType: str,
    knowledgeBaseId: str,
    presignedUrlTimeToLive: NotRequired[int],
```

## SystemEndpointAttributesTypeDef

```python
# SystemEndpointAttributesTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SystemEndpointAttributesTypeDef


def get_value() -> SystemEndpointAttributesTypeDef:
    return {
        "address": ...,
    }


# SystemEndpointAttributesTypeDef definition

class SystemEndpointAttributesTypeDef(TypedDict):
    address: NotRequired[str],
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateContentRequestTypeDef

```python
# UpdateContentRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UpdateContentRequestTypeDef


def get_value() -> UpdateContentRequestTypeDef:
    return {
        "contentId": ...,
    }


# UpdateContentRequestTypeDef definition

class UpdateContentRequestTypeDef(TypedDict):
    contentId: str,
    knowledgeBaseId: str,
    metadata: NotRequired[Mapping[str, str]],
    overrideLinkOutUri: NotRequired[str],
    removeOverrideLinkOutUri: NotRequired[bool],
    revisionId: NotRequired[str],
    title: NotRequired[str],
    uploadId: NotRequired[str],
```

## UpdateKnowledgeBaseTemplateUriRequestTypeDef

```python
# UpdateKnowledgeBaseTemplateUriRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UpdateKnowledgeBaseTemplateUriRequestTypeDef


def get_value() -> UpdateKnowledgeBaseTemplateUriRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# UpdateKnowledgeBaseTemplateUriRequestTypeDef definition

class UpdateKnowledgeBaseTemplateUriRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    templateUri: str,
```

## WebCrawlerLimitsTypeDef

```python
# WebCrawlerLimitsTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import WebCrawlerLimitsTypeDef


def get_value() -> WebCrawlerLimitsTypeDef:
    return {
        "rateLimit": ...,
    }


# WebCrawlerLimitsTypeDef definition

class WebCrawlerLimitsTypeDef(TypedDict):
    rateLimit: NotRequired[int],
```

## UpdateAssistantAIAgentRequestTypeDef

```python
# UpdateAssistantAIAgentRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UpdateAssistantAIAgentRequestTypeDef


def get_value() -> UpdateAssistantAIAgentRequestTypeDef:
    return {
        "aiAgentType": ...,
    }


# UpdateAssistantAIAgentRequestTypeDef definition

class UpdateAssistantAIAgentRequestTypeDef(TypedDict):
    aiAgentType: AIAgentTypeType,  # (1)
    assistantId: str,
    configuration: AIAgentConfigurationDataTypeDef,  # (2)
```

1. See [:material-code-brackets: AIAgentTypeType](./literals.md#aiagenttypetype) 
2. See [:material-code-braces: AIAgentConfigurationDataTypeDef](./type_defs.md#aiagentconfigurationdatatypedef) 
## AIGuardrailContentPolicyConfigOutputTypeDef

```python
# AIGuardrailContentPolicyConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIGuardrailContentPolicyConfigOutputTypeDef


def get_value() -> AIGuardrailContentPolicyConfigOutputTypeDef:
    return {
        "filtersConfig": ...,
    }


# AIGuardrailContentPolicyConfigOutputTypeDef definition

class AIGuardrailContentPolicyConfigOutputTypeDef(TypedDict):
    filtersConfig: List[GuardrailContentFilterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailContentFilterConfigTypeDef](./type_defs.md#guardrailcontentfilterconfigtypedef) 
## AIGuardrailContentPolicyConfigTypeDef

```python
# AIGuardrailContentPolicyConfigTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIGuardrailContentPolicyConfigTypeDef


def get_value() -> AIGuardrailContentPolicyConfigTypeDef:
    return {
        "filtersConfig": ...,
    }


# AIGuardrailContentPolicyConfigTypeDef definition

class AIGuardrailContentPolicyConfigTypeDef(TypedDict):
    filtersConfig: Sequence[GuardrailContentFilterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailContentFilterConfigTypeDef](./type_defs.md#guardrailcontentfilterconfigtypedef) 
## AIGuardrailContextualGroundingPolicyConfigOutputTypeDef

```python
# AIGuardrailContextualGroundingPolicyConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIGuardrailContextualGroundingPolicyConfigOutputTypeDef


def get_value() -> AIGuardrailContextualGroundingPolicyConfigOutputTypeDef:
    return {
        "filtersConfig": ...,
    }


# AIGuardrailContextualGroundingPolicyConfigOutputTypeDef definition

class AIGuardrailContextualGroundingPolicyConfigOutputTypeDef(TypedDict):
    filtersConfig: List[GuardrailContextualGroundingFilterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailContextualGroundingFilterConfigTypeDef](./type_defs.md#guardrailcontextualgroundingfilterconfigtypedef) 
## AIGuardrailContextualGroundingPolicyConfigTypeDef

```python
# AIGuardrailContextualGroundingPolicyConfigTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIGuardrailContextualGroundingPolicyConfigTypeDef


def get_value() -> AIGuardrailContextualGroundingPolicyConfigTypeDef:
    return {
        "filtersConfig": ...,
    }


# AIGuardrailContextualGroundingPolicyConfigTypeDef definition

class AIGuardrailContextualGroundingPolicyConfigTypeDef(TypedDict):
    filtersConfig: Sequence[GuardrailContextualGroundingFilterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailContextualGroundingFilterConfigTypeDef](./type_defs.md#guardrailcontextualgroundingfilterconfigtypedef) 
## AIGuardrailSensitiveInformationPolicyConfigOutputTypeDef

```python
# AIGuardrailSensitiveInformationPolicyConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIGuardrailSensitiveInformationPolicyConfigOutputTypeDef


def get_value() -> AIGuardrailSensitiveInformationPolicyConfigOutputTypeDef:
    return {
        "piiEntitiesConfig": ...,
    }


# AIGuardrailSensitiveInformationPolicyConfigOutputTypeDef definition

class AIGuardrailSensitiveInformationPolicyConfigOutputTypeDef(TypedDict):
    piiEntitiesConfig: NotRequired[List[GuardrailPiiEntityConfigTypeDef]],  # (1)
    regexesConfig: NotRequired[List[GuardrailRegexConfigTypeDef]],  # (2)
```

1. See [:material-code-braces: GuardrailPiiEntityConfigTypeDef](./type_defs.md#guardrailpiientityconfigtypedef) 
2. See [:material-code-braces: GuardrailRegexConfigTypeDef](./type_defs.md#guardrailregexconfigtypedef) 
## AIGuardrailSensitiveInformationPolicyConfigTypeDef

```python
# AIGuardrailSensitiveInformationPolicyConfigTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIGuardrailSensitiveInformationPolicyConfigTypeDef


def get_value() -> AIGuardrailSensitiveInformationPolicyConfigTypeDef:
    return {
        "piiEntitiesConfig": ...,
    }


# AIGuardrailSensitiveInformationPolicyConfigTypeDef definition

class AIGuardrailSensitiveInformationPolicyConfigTypeDef(TypedDict):
    piiEntitiesConfig: NotRequired[Sequence[GuardrailPiiEntityConfigTypeDef]],  # (1)
    regexesConfig: NotRequired[Sequence[GuardrailRegexConfigTypeDef]],  # (2)
```

1. See [:material-code-braces: GuardrailPiiEntityConfigTypeDef](./type_defs.md#guardrailpiientityconfigtypedef) 
2. See [:material-code-braces: GuardrailRegexConfigTypeDef](./type_defs.md#guardrailregexconfigtypedef) 
## AIGuardrailVersionSummaryTypeDef

```python
# AIGuardrailVersionSummaryTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIGuardrailVersionSummaryTypeDef


def get_value() -> AIGuardrailVersionSummaryTypeDef:
    return {
        "aiGuardrailSummary": ...,
    }


# AIGuardrailVersionSummaryTypeDef definition

class AIGuardrailVersionSummaryTypeDef(TypedDict):
    aiGuardrailSummary: NotRequired[AIGuardrailSummaryTypeDef],  # (1)
    versionNumber: NotRequired[int],
```

1. See [:material-code-braces: AIGuardrailSummaryTypeDef](./type_defs.md#aiguardrailsummarytypedef) 
## AIGuardrailTopicPolicyConfigOutputTypeDef

```python
# AIGuardrailTopicPolicyConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIGuardrailTopicPolicyConfigOutputTypeDef


def get_value() -> AIGuardrailTopicPolicyConfigOutputTypeDef:
    return {
        "topicsConfig": ...,
    }


# AIGuardrailTopicPolicyConfigOutputTypeDef definition

class AIGuardrailTopicPolicyConfigOutputTypeDef(TypedDict):
    topicsConfig: List[GuardrailTopicConfigOutputTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailTopicConfigOutputTypeDef](./type_defs.md#guardrailtopicconfigoutputtypedef) 
## AIGuardrailTopicPolicyConfigTypeDef

```python
# AIGuardrailTopicPolicyConfigTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIGuardrailTopicPolicyConfigTypeDef


def get_value() -> AIGuardrailTopicPolicyConfigTypeDef:
    return {
        "topicsConfig": ...,
    }


# AIGuardrailTopicPolicyConfigTypeDef definition

class AIGuardrailTopicPolicyConfigTypeDef(TypedDict):
    topicsConfig: Sequence[GuardrailTopicConfigTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailTopicConfigTypeDef](./type_defs.md#guardrailtopicconfigtypedef) 
## AIGuardrailWordPolicyConfigOutputTypeDef

```python
# AIGuardrailWordPolicyConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIGuardrailWordPolicyConfigOutputTypeDef


def get_value() -> AIGuardrailWordPolicyConfigOutputTypeDef:
    return {
        "managedWordListsConfig": ...,
    }


# AIGuardrailWordPolicyConfigOutputTypeDef definition

class AIGuardrailWordPolicyConfigOutputTypeDef(TypedDict):
    managedWordListsConfig: NotRequired[List[GuardrailManagedWordsConfigTypeDef]],  # (1)
    wordsConfig: NotRequired[List[GuardrailWordConfigTypeDef]],  # (2)
```

1. See [:material-code-braces: GuardrailManagedWordsConfigTypeDef](./type_defs.md#guardrailmanagedwordsconfigtypedef) 
2. See [:material-code-braces: GuardrailWordConfigTypeDef](./type_defs.md#guardrailwordconfigtypedef) 
## AIGuardrailWordPolicyConfigTypeDef

```python
# AIGuardrailWordPolicyConfigTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIGuardrailWordPolicyConfigTypeDef


def get_value() -> AIGuardrailWordPolicyConfigTypeDef:
    return {
        "managedWordListsConfig": ...,
    }


# AIGuardrailWordPolicyConfigTypeDef definition

class AIGuardrailWordPolicyConfigTypeDef(TypedDict):
    managedWordListsConfig: NotRequired[Sequence[GuardrailManagedWordsConfigTypeDef]],  # (1)
    wordsConfig: NotRequired[Sequence[GuardrailWordConfigTypeDef]],  # (2)
```

1. See [:material-code-braces: GuardrailManagedWordsConfigTypeDef](./type_defs.md#guardrailmanagedwordsconfigtypedef) 
2. See [:material-code-braces: GuardrailWordConfigTypeDef](./type_defs.md#guardrailwordconfigtypedef) 
## AIPromptVersionSummaryTypeDef

```python
# AIPromptVersionSummaryTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIPromptVersionSummaryTypeDef


def get_value() -> AIPromptVersionSummaryTypeDef:
    return {
        "aiPromptSummary": ...,
    }


# AIPromptVersionSummaryTypeDef definition

class AIPromptVersionSummaryTypeDef(TypedDict):
    aiPromptSummary: NotRequired[AIPromptSummaryTypeDef],  # (1)
    versionNumber: NotRequired[int],
```

1. See [:material-code-braces: AIPromptSummaryTypeDef](./type_defs.md#aipromptsummarytypedef) 
## AIPromptTemplateConfigurationTypeDef

```python
# AIPromptTemplateConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIPromptTemplateConfigurationTypeDef


def get_value() -> AIPromptTemplateConfigurationTypeDef:
    return {
        "textFullAIPromptEditTemplateConfiguration": ...,
    }


# AIPromptTemplateConfigurationTypeDef definition

class AIPromptTemplateConfigurationTypeDef(TypedDict):
    textFullAIPromptEditTemplateConfiguration: NotRequired[TextFullAIPromptEditTemplateConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: TextFullAIPromptEditTemplateConfigurationTypeDef](./type_defs.md#textfullaipromptedittemplateconfigurationtypedef) 
## ActivateMessageTemplateResponseTypeDef

```python
# ActivateMessageTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ActivateMessageTemplateResponseTypeDef


def get_value() -> ActivateMessageTemplateResponseTypeDef:
    return {
        "messageTemplateArn": ...,
    }


# ActivateMessageTemplateResponseTypeDef definition

class ActivateMessageTemplateResponseTypeDef(TypedDict):
    messageTemplateArn: str,
    messageTemplateId: str,
    versionNumber: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeactivateMessageTemplateResponseTypeDef

```python
# DeactivateMessageTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DeactivateMessageTemplateResponseTypeDef


def get_value() -> DeactivateMessageTemplateResponseTypeDef:
    return {
        "messageTemplateArn": ...,
    }


# DeactivateMessageTemplateResponseTypeDef definition

class DeactivateMessageTemplateResponseTypeDef(TypedDict):
    messageTemplateArn: str,
    messageTemplateId: str,
    versionNumber: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAIGuardrailsResponseTypeDef

```python
# ListAIGuardrailsResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAIGuardrailsResponseTypeDef


def get_value() -> ListAIGuardrailsResponseTypeDef:
    return {
        "aiGuardrailSummaries": ...,
    }


# ListAIGuardrailsResponseTypeDef definition

class ListAIGuardrailsResponseTypeDef(TypedDict):
    aiGuardrailSummaries: List[AIGuardrailSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AIGuardrailSummaryTypeDef](./type_defs.md#aiguardrailsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAIPromptsResponseTypeDef

```python
# ListAIPromptsResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAIPromptsResponseTypeDef


def get_value() -> ListAIPromptsResponseTypeDef:
    return {
        "aiPromptSummaries": ...,
    }


# ListAIPromptsResponseTypeDef definition

class ListAIPromptsResponseTypeDef(TypedDict):
    aiPromptSummaries: List[AIPromptSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AIPromptSummaryTypeDef](./type_defs.md#aipromptsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendMessageResponseTypeDef

```python
# SendMessageResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SendMessageResponseTypeDef


def get_value() -> SendMessageResponseTypeDef:
    return {
        "nextMessageToken": ...,
    }


# SendMessageResponseTypeDef definition

class SendMessageResponseTypeDef(TypedDict):
    nextMessageToken: str,
    requestMessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartContentUploadResponseTypeDef

```python
# StartContentUploadResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import StartContentUploadResponseTypeDef


def get_value() -> StartContentUploadResponseTypeDef:
    return {
        "headersToInclude": ...,
    }


# StartContentUploadResponseTypeDef definition

class StartContentUploadResponseTypeDef(TypedDict):
    headersToInclude: Dict[str, str],
    uploadId: str,
    url: str,
    urlExpiry: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ContentAssociationContentsTypeDef

```python
# ContentAssociationContentsTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ContentAssociationContentsTypeDef


def get_value() -> ContentAssociationContentsTypeDef:
    return {
        "amazonConnectGuideAssociation": ...,
    }


# ContentAssociationContentsTypeDef definition

class ContentAssociationContentsTypeDef(TypedDict):
    amazonConnectGuideAssociation: NotRequired[AmazonConnectGuideAssociationDataTypeDef],  # (1)
```

1. See [:material-code-braces: AmazonConnectGuideAssociationDataTypeDef](./type_defs.md#amazonconnectguideassociationdatatypedef) 
## CreateAssistantAssociationRequestTypeDef

```python
# CreateAssistantAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateAssistantAssociationRequestTypeDef


def get_value() -> CreateAssistantAssociationRequestTypeDef:
    return {
        "assistantId": ...,
    }


# CreateAssistantAssociationRequestTypeDef definition

class CreateAssistantAssociationRequestTypeDef(TypedDict):
    assistantId: str,
    association: AssistantAssociationInputDataTypeDef,  # (1)
    associationType: AssociationTypeType,  # (2)
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AssistantAssociationInputDataTypeDef](./type_defs.md#assistantassociationinputdatatypedef) 
2. See [:material-code-brackets: AssociationTypeType](./literals.md#associationtypetype) 
## AssistantAssociationOutputDataTypeDef

```python
# AssistantAssociationOutputDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AssistantAssociationOutputDataTypeDef


def get_value() -> AssistantAssociationOutputDataTypeDef:
    return {
        "knowledgeBaseAssociation": ...,
    }


# AssistantAssociationOutputDataTypeDef definition

class AssistantAssociationOutputDataTypeDef(TypedDict):
    knowledgeBaseAssociation: NotRequired[KnowledgeBaseAssociationDataTypeDef],  # (1)
```

1. See [:material-code-braces: KnowledgeBaseAssociationDataTypeDef](./type_defs.md#knowledgebaseassociationdatatypedef) 
## AssistantDataTypeDef

```python
# AssistantDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AssistantDataTypeDef


def get_value() -> AssistantDataTypeDef:
    return {
        "aiAgentConfiguration": ...,
    }


# AssistantDataTypeDef definition

class AssistantDataTypeDef(TypedDict):
    assistantArn: str,
    assistantId: str,
    name: str,
    status: AssistantStatusType,  # (5)
    type: AssistantTypeType,  # (6)
    aiAgentConfiguration: NotRequired[Dict[AIAgentTypeType, AIAgentConfigurationDataTypeDef]],  # (1)
    capabilityConfiguration: NotRequired[AssistantCapabilityConfigurationTypeDef],  # (2)
    description: NotRequired[str],
    integrationConfiguration: NotRequired[AssistantIntegrationConfigurationTypeDef],  # (3)
    serverSideEncryptionConfiguration: NotRequired[ServerSideEncryptionConfigurationTypeDef],  # (4)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: AIAgentTypeType](./literals.md#aiagenttypetype) [:material-code-braces: AIAgentConfigurationDataTypeDef](./type_defs.md#aiagentconfigurationdatatypedef) 
2. See [:material-code-braces: AssistantCapabilityConfigurationTypeDef](./type_defs.md#assistantcapabilityconfigurationtypedef) 
3. See [:material-code-braces: AssistantIntegrationConfigurationTypeDef](./type_defs.md#assistantintegrationconfigurationtypedef) 
4. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
5. See [:material-code-brackets: AssistantStatusType](./literals.md#assistantstatustype) 
6. See [:material-code-brackets: AssistantTypeType](./literals.md#assistanttypetype) 
## AssistantSummaryTypeDef

```python
# AssistantSummaryTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AssistantSummaryTypeDef


def get_value() -> AssistantSummaryTypeDef:
    return {
        "aiAgentConfiguration": ...,
    }


# AssistantSummaryTypeDef definition

class AssistantSummaryTypeDef(TypedDict):
    assistantArn: str,
    assistantId: str,
    name: str,
    status: AssistantStatusType,  # (5)
    type: AssistantTypeType,  # (6)
    aiAgentConfiguration: NotRequired[Dict[AIAgentTypeType, AIAgentConfigurationDataTypeDef]],  # (1)
    capabilityConfiguration: NotRequired[AssistantCapabilityConfigurationTypeDef],  # (2)
    description: NotRequired[str],
    integrationConfiguration: NotRequired[AssistantIntegrationConfigurationTypeDef],  # (3)
    serverSideEncryptionConfiguration: NotRequired[ServerSideEncryptionConfigurationTypeDef],  # (4)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: AIAgentTypeType](./literals.md#aiagenttypetype) [:material-code-braces: AIAgentConfigurationDataTypeDef](./type_defs.md#aiagentconfigurationdatatypedef) 
2. See [:material-code-braces: AssistantCapabilityConfigurationTypeDef](./type_defs.md#assistantcapabilityconfigurationtypedef) 
3. See [:material-code-braces: AssistantIntegrationConfigurationTypeDef](./type_defs.md#assistantintegrationconfigurationtypedef) 
4. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
5. See [:material-code-brackets: AssistantStatusType](./literals.md#assistantstatustype) 
6. See [:material-code-brackets: AssistantTypeType](./literals.md#assistanttypetype) 
## CreateAssistantRequestTypeDef

```python
# CreateAssistantRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateAssistantRequestTypeDef


def get_value() -> CreateAssistantRequestTypeDef:
    return {
        "name": ...,
    }


# CreateAssistantRequestTypeDef definition

class CreateAssistantRequestTypeDef(TypedDict):
    name: str,
    type: AssistantTypeType,  # (1)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    serverSideEncryptionConfiguration: NotRequired[ServerSideEncryptionConfigurationTypeDef],  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: AssistantTypeType](./literals.md#assistanttypetype) 
2. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
## BedrockFoundationModelConfigurationForParsingTypeDef

```python
# BedrockFoundationModelConfigurationForParsingTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import BedrockFoundationModelConfigurationForParsingTypeDef


def get_value() -> BedrockFoundationModelConfigurationForParsingTypeDef:
    return {
        "modelArn": ...,
    }


# BedrockFoundationModelConfigurationForParsingTypeDef definition

class BedrockFoundationModelConfigurationForParsingTypeDef(TypedDict):
    modelArn: str,
    parsingPrompt: NotRequired[ParsingPromptTypeDef],  # (1)
```

1. See [:material-code-braces: ParsingPromptTypeDef](./type_defs.md#parsingprompttypedef) 
## ConfigurationTypeDef

```python
# ConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ConfigurationTypeDef


def get_value() -> ConfigurationTypeDef:
    return {
        "connectConfiguration": ...,
    }


# ConfigurationTypeDef definition

class ConfigurationTypeDef(TypedDict):
    connectConfiguration: NotRequired[ConnectConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ConnectConfigurationTypeDef](./type_defs.md#connectconfigurationtypedef) 
## GenerativeDataDetailsPaginatorTypeDef

```python
# GenerativeDataDetailsPaginatorTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GenerativeDataDetailsPaginatorTypeDef


def get_value() -> GenerativeDataDetailsPaginatorTypeDef:
    return {
        "completion": ...,
    }


# GenerativeDataDetailsPaginatorTypeDef definition

class GenerativeDataDetailsPaginatorTypeDef(TypedDict):
    completion: str,
    rankingData: RankingDataTypeDef,  # (1)
    references: List[Dict[str, Any]],
```

1. See [:material-code-braces: RankingDataTypeDef](./type_defs.md#rankingdatatypedef) 
## GenerativeDataDetailsTypeDef

```python
# GenerativeDataDetailsTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GenerativeDataDetailsTypeDef


def get_value() -> GenerativeDataDetailsTypeDef:
    return {
        "completion": ...,
    }


# GenerativeDataDetailsTypeDef definition

class GenerativeDataDetailsTypeDef(TypedDict):
    completion: str,
    rankingData: RankingDataTypeDef,  # (1)
    references: List[Dict[str, Any]],
```

1. See [:material-code-braces: RankingDataTypeDef](./type_defs.md#rankingdatatypedef) 
## CreateContentResponseTypeDef

```python
# CreateContentResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateContentResponseTypeDef


def get_value() -> CreateContentResponseTypeDef:
    return {
        "content": ...,
    }


# CreateContentResponseTypeDef definition

class CreateContentResponseTypeDef(TypedDict):
    content: ContentDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContentDataTypeDef](./type_defs.md#contentdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetContentResponseTypeDef

```python
# GetContentResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetContentResponseTypeDef


def get_value() -> GetContentResponseTypeDef:
    return {
        "content": ...,
    }


# GetContentResponseTypeDef definition

class GetContentResponseTypeDef(TypedDict):
    content: ContentDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContentDataTypeDef](./type_defs.md#contentdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateContentResponseTypeDef

```python
# UpdateContentResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UpdateContentResponseTypeDef


def get_value() -> UpdateContentResponseTypeDef:
    return {
        "content": ...,
    }


# UpdateContentResponseTypeDef definition

class UpdateContentResponseTypeDef(TypedDict):
    content: ContentDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContentDataTypeDef](./type_defs.md#contentdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ContentFeedbackDataTypeDef

```python
# ContentFeedbackDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ContentFeedbackDataTypeDef


def get_value() -> ContentFeedbackDataTypeDef:
    return {
        "generativeContentFeedbackData": ...,
    }


# ContentFeedbackDataTypeDef definition

class ContentFeedbackDataTypeDef(TypedDict):
    generativeContentFeedbackData: NotRequired[GenerativeContentFeedbackDataTypeDef],  # (1)
```

1. See [:material-code-braces: GenerativeContentFeedbackDataTypeDef](./type_defs.md#generativecontentfeedbackdatatypedef) 
## GetContentSummaryResponseTypeDef

```python
# GetContentSummaryResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetContentSummaryResponseTypeDef


def get_value() -> GetContentSummaryResponseTypeDef:
    return {
        "contentSummary": ...,
    }


# GetContentSummaryResponseTypeDef definition

class GetContentSummaryResponseTypeDef(TypedDict):
    contentSummary: ContentSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContentSummaryTypeDef](./type_defs.md#contentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListContentsResponseTypeDef

```python
# ListContentsResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListContentsResponseTypeDef


def get_value() -> ListContentsResponseTypeDef:
    return {
        "contentSummaries": ...,
    }


# ListContentsResponseTypeDef definition

class ListContentsResponseTypeDef(TypedDict):
    contentSummaries: List[ContentSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ContentSummaryTypeDef](./type_defs.md#contentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchContentResponseTypeDef

```python
# SearchContentResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SearchContentResponseTypeDef


def get_value() -> SearchContentResponseTypeDef:
    return {
        "contentSummaries": ...,
    }


# SearchContentResponseTypeDef definition

class SearchContentResponseTypeDef(TypedDict):
    contentSummaries: List[ContentSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ContentSummaryTypeDef](./type_defs.md#contentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConversationContextTypeDef

```python
# ConversationContextTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ConversationContextTypeDef


def get_value() -> ConversationContextTypeDef:
    return {
        "selfServiceConversationHistory": ...,
    }


# ConversationContextTypeDef definition

class ConversationContextTypeDef(TypedDict):
    selfServiceConversationHistory: Sequence[SelfServiceConversationHistoryTypeDef],  # (1)
```

1. See [:material-code-braces: SelfServiceConversationHistoryTypeDef](./type_defs.md#selfserviceconversationhistorytypedef) 
## CreateAIAgentVersionRequestTypeDef

```python
# CreateAIAgentVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateAIAgentVersionRequestTypeDef


def get_value() -> CreateAIAgentVersionRequestTypeDef:
    return {
        "aiAgentId": ...,
    }


# CreateAIAgentVersionRequestTypeDef definition

class CreateAIAgentVersionRequestTypeDef(TypedDict):
    aiAgentId: str,
    assistantId: str,
    clientToken: NotRequired[str],
    modifiedTime: NotRequired[TimestampTypeDef],
```

## CreateAIGuardrailVersionRequestTypeDef

```python
# CreateAIGuardrailVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateAIGuardrailVersionRequestTypeDef


def get_value() -> CreateAIGuardrailVersionRequestTypeDef:
    return {
        "aiGuardrailId": ...,
    }


# CreateAIGuardrailVersionRequestTypeDef definition

class CreateAIGuardrailVersionRequestTypeDef(TypedDict):
    aiGuardrailId: str,
    assistantId: str,
    clientToken: NotRequired[str],
    modifiedTime: NotRequired[TimestampTypeDef],
```

## CreateAIPromptVersionRequestTypeDef

```python
# CreateAIPromptVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateAIPromptVersionRequestTypeDef


def get_value() -> CreateAIPromptVersionRequestTypeDef:
    return {
        "aiPromptId": ...,
    }


# CreateAIPromptVersionRequestTypeDef definition

class CreateAIPromptVersionRequestTypeDef(TypedDict):
    aiPromptId: str,
    assistantId: str,
    clientToken: NotRequired[str],
    modifiedTime: NotRequired[TimestampTypeDef],
```

## CreateMessageTemplateAttachmentResponseTypeDef

```python
# CreateMessageTemplateAttachmentResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateMessageTemplateAttachmentResponseTypeDef


def get_value() -> CreateMessageTemplateAttachmentResponseTypeDef:
    return {
        "attachment": ...,
    }


# CreateMessageTemplateAttachmentResponseTypeDef definition

class CreateMessageTemplateAttachmentResponseTypeDef(TypedDict):
    attachment: MessageTemplateAttachmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageTemplateAttachmentTypeDef](./type_defs.md#messagetemplateattachmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataReferenceTypeDef

```python
# DataReferenceTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DataReferenceTypeDef


def get_value() -> DataReferenceTypeDef:
    return {
        "contentReference": ...,
    }


# DataReferenceTypeDef definition

class DataReferenceTypeDef(TypedDict):
    contentReference: NotRequired[ContentReferenceTypeDef],  # (1)
    generativeReference: NotRequired[GenerativeReferenceTypeDef],  # (2)
```

1. See [:material-code-braces: ContentReferenceTypeDef](./type_defs.md#contentreferencetypedef) 
2. See [:material-code-braces: GenerativeReferenceTypeDef](./type_defs.md#generativereferencetypedef) 
## DocumentTextTypeDef

```python
# DocumentTextTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DocumentTextTypeDef


def get_value() -> DocumentTextTypeDef:
    return {
        "highlights": ...,
    }


# DocumentTextTypeDef definition

class DocumentTextTypeDef(TypedDict):
    highlights: NotRequired[List[HighlightTypeDef]],  # (1)
    text: NotRequired[str],
```

1. See [:material-code-braces: HighlightTypeDef](./type_defs.md#highlighttypedef) 
## EmailMessageTemplateContentBodyTypeDef

```python
# EmailMessageTemplateContentBodyTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import EmailMessageTemplateContentBodyTypeDef


def get_value() -> EmailMessageTemplateContentBodyTypeDef:
    return {
        "html": ...,
    }


# EmailMessageTemplateContentBodyTypeDef definition

class EmailMessageTemplateContentBodyTypeDef(TypedDict):
    html: NotRequired[MessageTemplateBodyContentProviderTypeDef],  # (1)
    plainText: NotRequired[MessageTemplateBodyContentProviderTypeDef],  # (1)
```

1. See [:material-code-braces: MessageTemplateBodyContentProviderTypeDef](./type_defs.md#messagetemplatebodycontentprovidertypedef) 
2. See [:material-code-braces: MessageTemplateBodyContentProviderTypeDef](./type_defs.md#messagetemplatebodycontentprovidertypedef) 
## SMSMessageTemplateContentBodyTypeDef

```python
# SMSMessageTemplateContentBodyTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SMSMessageTemplateContentBodyTypeDef


def get_value() -> SMSMessageTemplateContentBodyTypeDef:
    return {
        "plainText": ...,
    }


# SMSMessageTemplateContentBodyTypeDef definition

class SMSMessageTemplateContentBodyTypeDef(TypedDict):
    plainText: NotRequired[MessageTemplateBodyContentProviderTypeDef],  # (1)
```

1. See [:material-code-braces: MessageTemplateBodyContentProviderTypeDef](./type_defs.md#messagetemplatebodycontentprovidertypedef) 
## MessageTemplateSearchResultDataTypeDef

```python
# MessageTemplateSearchResultDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import MessageTemplateSearchResultDataTypeDef


def get_value() -> MessageTemplateSearchResultDataTypeDef:
    return {
        "channelSubtype": ...,
    }


# MessageTemplateSearchResultDataTypeDef definition

class MessageTemplateSearchResultDataTypeDef(TypedDict):
    channelSubtype: ChannelSubtypeType,  # (1)
    createdTime: datetime,
    knowledgeBaseArn: str,
    knowledgeBaseId: str,
    lastModifiedBy: str,
    lastModifiedTime: datetime,
    messageTemplateArn: str,
    messageTemplateId: str,
    name: str,
    description: NotRequired[str],
    groupingConfiguration: NotRequired[GroupingConfigurationOutputTypeDef],  # (2)
    isActive: NotRequired[bool],
    language: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    versionNumber: NotRequired[int],
```

1. See [:material-code-brackets: ChannelSubtypeType](./literals.md#channelsubtypetype) 
2. See [:material-code-braces: GroupingConfigurationOutputTypeDef](./type_defs.md#groupingconfigurationoutputtypedef) 
## SearchExpressionTypeDef

```python
# SearchExpressionTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SearchExpressionTypeDef


def get_value() -> SearchExpressionTypeDef:
    return {
        "filters": ...,
    }


# SearchExpressionTypeDef definition

class SearchExpressionTypeDef(TypedDict):
    filters: Sequence[FilterTypeDef],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## HierarchicalChunkingConfigurationOutputTypeDef

```python
# HierarchicalChunkingConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import HierarchicalChunkingConfigurationOutputTypeDef


def get_value() -> HierarchicalChunkingConfigurationOutputTypeDef:
    return {
        "levelConfigurations": ...,
    }


# HierarchicalChunkingConfigurationOutputTypeDef definition

class HierarchicalChunkingConfigurationOutputTypeDef(TypedDict):
    levelConfigurations: List[HierarchicalChunkingLevelConfigurationTypeDef],  # (1)
    overlapTokens: int,
```

1. See [:material-code-braces: HierarchicalChunkingLevelConfigurationTypeDef](./type_defs.md#hierarchicalchunkinglevelconfigurationtypedef) 
## HierarchicalChunkingConfigurationTypeDef

```python
# HierarchicalChunkingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import HierarchicalChunkingConfigurationTypeDef


def get_value() -> HierarchicalChunkingConfigurationTypeDef:
    return {
        "levelConfigurations": ...,
    }


# HierarchicalChunkingConfigurationTypeDef definition

class HierarchicalChunkingConfigurationTypeDef(TypedDict):
    levelConfigurations: Sequence[HierarchicalChunkingLevelConfigurationTypeDef],  # (1)
    overlapTokens: int,
```

1. See [:material-code-braces: HierarchicalChunkingLevelConfigurationTypeDef](./type_defs.md#hierarchicalchunkinglevelconfigurationtypedef) 
## ListAIAgentVersionsRequestPaginateTypeDef

```python
# ListAIAgentVersionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAIAgentVersionsRequestPaginateTypeDef


def get_value() -> ListAIAgentVersionsRequestPaginateTypeDef:
    return {
        "aiAgentId": ...,
    }


# ListAIAgentVersionsRequestPaginateTypeDef definition

class ListAIAgentVersionsRequestPaginateTypeDef(TypedDict):
    aiAgentId: str,
    assistantId: str,
    origin: NotRequired[OriginType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: OriginType](./literals.md#origintype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAIAgentsRequestPaginateTypeDef

```python
# ListAIAgentsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAIAgentsRequestPaginateTypeDef


def get_value() -> ListAIAgentsRequestPaginateTypeDef:
    return {
        "assistantId": ...,
    }


# ListAIAgentsRequestPaginateTypeDef definition

class ListAIAgentsRequestPaginateTypeDef(TypedDict):
    assistantId: str,
    origin: NotRequired[OriginType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: OriginType](./literals.md#origintype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAIGuardrailVersionsRequestPaginateTypeDef

```python
# ListAIGuardrailVersionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAIGuardrailVersionsRequestPaginateTypeDef


def get_value() -> ListAIGuardrailVersionsRequestPaginateTypeDef:
    return {
        "aiGuardrailId": ...,
    }


# ListAIGuardrailVersionsRequestPaginateTypeDef definition

class ListAIGuardrailVersionsRequestPaginateTypeDef(TypedDict):
    aiGuardrailId: str,
    assistantId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAIGuardrailsRequestPaginateTypeDef

```python
# ListAIGuardrailsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAIGuardrailsRequestPaginateTypeDef


def get_value() -> ListAIGuardrailsRequestPaginateTypeDef:
    return {
        "assistantId": ...,
    }


# ListAIGuardrailsRequestPaginateTypeDef definition

class ListAIGuardrailsRequestPaginateTypeDef(TypedDict):
    assistantId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAIPromptVersionsRequestPaginateTypeDef

```python
# ListAIPromptVersionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAIPromptVersionsRequestPaginateTypeDef


def get_value() -> ListAIPromptVersionsRequestPaginateTypeDef:
    return {
        "aiPromptId": ...,
    }


# ListAIPromptVersionsRequestPaginateTypeDef definition

class ListAIPromptVersionsRequestPaginateTypeDef(TypedDict):
    aiPromptId: str,
    assistantId: str,
    origin: NotRequired[OriginType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: OriginType](./literals.md#origintype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAIPromptsRequestPaginateTypeDef

```python
# ListAIPromptsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAIPromptsRequestPaginateTypeDef


def get_value() -> ListAIPromptsRequestPaginateTypeDef:
    return {
        "assistantId": ...,
    }


# ListAIPromptsRequestPaginateTypeDef definition

class ListAIPromptsRequestPaginateTypeDef(TypedDict):
    assistantId: str,
    origin: NotRequired[OriginType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: OriginType](./literals.md#origintype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssistantAssociationsRequestPaginateTypeDef

```python
# ListAssistantAssociationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAssistantAssociationsRequestPaginateTypeDef


def get_value() -> ListAssistantAssociationsRequestPaginateTypeDef:
    return {
        "assistantId": ...,
    }


# ListAssistantAssociationsRequestPaginateTypeDef definition

class ListAssistantAssociationsRequestPaginateTypeDef(TypedDict):
    assistantId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssistantsRequestPaginateTypeDef

```python
# ListAssistantsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAssistantsRequestPaginateTypeDef


def get_value() -> ListAssistantsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListAssistantsRequestPaginateTypeDef definition

class ListAssistantsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListContentAssociationsRequestPaginateTypeDef

```python
# ListContentAssociationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListContentAssociationsRequestPaginateTypeDef


def get_value() -> ListContentAssociationsRequestPaginateTypeDef:
    return {
        "contentId": ...,
    }


# ListContentAssociationsRequestPaginateTypeDef definition

class ListContentAssociationsRequestPaginateTypeDef(TypedDict):
    contentId: str,
    knowledgeBaseId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListContentsRequestPaginateTypeDef

```python
# ListContentsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListContentsRequestPaginateTypeDef


def get_value() -> ListContentsRequestPaginateTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# ListContentsRequestPaginateTypeDef definition

class ListContentsRequestPaginateTypeDef(TypedDict):
    knowledgeBaseId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListImportJobsRequestPaginateTypeDef

```python
# ListImportJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListImportJobsRequestPaginateTypeDef


def get_value() -> ListImportJobsRequestPaginateTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# ListImportJobsRequestPaginateTypeDef definition

class ListImportJobsRequestPaginateTypeDef(TypedDict):
    knowledgeBaseId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListKnowledgeBasesRequestPaginateTypeDef

```python
# ListKnowledgeBasesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListKnowledgeBasesRequestPaginateTypeDef


def get_value() -> ListKnowledgeBasesRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListKnowledgeBasesRequestPaginateTypeDef definition

class ListKnowledgeBasesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMessageTemplateVersionsRequestPaginateTypeDef

```python
# ListMessageTemplateVersionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListMessageTemplateVersionsRequestPaginateTypeDef


def get_value() -> ListMessageTemplateVersionsRequestPaginateTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# ListMessageTemplateVersionsRequestPaginateTypeDef definition

class ListMessageTemplateVersionsRequestPaginateTypeDef(TypedDict):
    knowledgeBaseId: str,
    messageTemplateId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMessageTemplatesRequestPaginateTypeDef

```python
# ListMessageTemplatesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListMessageTemplatesRequestPaginateTypeDef


def get_value() -> ListMessageTemplatesRequestPaginateTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# ListMessageTemplatesRequestPaginateTypeDef definition

class ListMessageTemplatesRequestPaginateTypeDef(TypedDict):
    knowledgeBaseId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMessagesRequestPaginateTypeDef

```python
# ListMessagesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListMessagesRequestPaginateTypeDef


def get_value() -> ListMessagesRequestPaginateTypeDef:
    return {
        "assistantId": ...,
    }


# ListMessagesRequestPaginateTypeDef definition

class ListMessagesRequestPaginateTypeDef(TypedDict):
    assistantId: str,
    sessionId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQuickResponsesRequestPaginateTypeDef

```python
# ListQuickResponsesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListQuickResponsesRequestPaginateTypeDef


def get_value() -> ListQuickResponsesRequestPaginateTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# ListQuickResponsesRequestPaginateTypeDef definition

class ListQuickResponsesRequestPaginateTypeDef(TypedDict):
    knowledgeBaseId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMessageTemplateVersionsResponseTypeDef

```python
# ListMessageTemplateVersionsResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListMessageTemplateVersionsResponseTypeDef


def get_value() -> ListMessageTemplateVersionsResponseTypeDef:
    return {
        "messageTemplateVersionSummaries": ...,
    }


# ListMessageTemplateVersionsResponseTypeDef definition

class ListMessageTemplateVersionsResponseTypeDef(TypedDict):
    messageTemplateVersionSummaries: List[MessageTemplateVersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MessageTemplateVersionSummaryTypeDef](./type_defs.md#messagetemplateversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMessageTemplatesResponseTypeDef

```python
# ListMessageTemplatesResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListMessageTemplatesResponseTypeDef


def get_value() -> ListMessageTemplatesResponseTypeDef:
    return {
        "messageTemplateSummaries": ...,
    }


# ListMessageTemplatesResponseTypeDef definition

class ListMessageTemplatesResponseTypeDef(TypedDict):
    messageTemplateSummaries: List[MessageTemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MessageTemplateSummaryTypeDef](./type_defs.md#messagetemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQuickResponsesResponseTypeDef

```python
# ListQuickResponsesResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListQuickResponsesResponseTypeDef


def get_value() -> ListQuickResponsesResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListQuickResponsesResponseTypeDef definition

class ListQuickResponsesResponseTypeDef(TypedDict):
    quickResponseSummaries: List[QuickResponseSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: QuickResponseSummaryTypeDef](./type_defs.md#quickresponsesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MessageDataTypeDef

```python
# MessageDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import MessageDataTypeDef


def get_value() -> MessageDataTypeDef:
    return {
        "text": ...,
    }


# MessageDataTypeDef definition

class MessageDataTypeDef(TypedDict):
    text: NotRequired[TextMessageTypeDef],  # (1)
```

1. See [:material-code-braces: TextMessageTypeDef](./type_defs.md#textmessagetypedef) 
## MessageTemplateSearchExpressionTypeDef

```python
# MessageTemplateSearchExpressionTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import MessageTemplateSearchExpressionTypeDef


def get_value() -> MessageTemplateSearchExpressionTypeDef:
    return {
        "filters": ...,
    }


# MessageTemplateSearchExpressionTypeDef definition

class MessageTemplateSearchExpressionTypeDef(TypedDict):
    filters: NotRequired[Sequence[MessageTemplateFilterFieldTypeDef]],  # (1)
    orderOnField: NotRequired[MessageTemplateOrderFieldTypeDef],  # (2)
    queries: NotRequired[Sequence[MessageTemplateQueryFieldTypeDef]],  # (3)
```

1. See [:material-code-braces: MessageTemplateFilterFieldTypeDef](./type_defs.md#messagetemplatefilterfieldtypedef) 
2. See [:material-code-braces: MessageTemplateOrderFieldTypeDef](./type_defs.md#messagetemplateorderfieldtypedef) 
3. See [:material-code-braces: MessageTemplateQueryFieldTypeDef](./type_defs.md#messagetemplatequeryfieldtypedef) 
## NotifyRecommendationsReceivedResponseTypeDef

```python
# NotifyRecommendationsReceivedResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import NotifyRecommendationsReceivedResponseTypeDef


def get_value() -> NotifyRecommendationsReceivedResponseTypeDef:
    return {
        "errors": ...,
    }


# NotifyRecommendationsReceivedResponseTypeDef definition

class NotifyRecommendationsReceivedResponseTypeDef(TypedDict):
    errors: List[NotifyRecommendationsReceivedErrorTypeDef],  # (1)
    recommendationIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NotifyRecommendationsReceivedErrorTypeDef](./type_defs.md#notifyrecommendationsreceivederrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OrConditionOutputTypeDef

```python
# OrConditionOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import OrConditionOutputTypeDef


def get_value() -> OrConditionOutputTypeDef:
    return {
        "andConditions": ...,
    }


# OrConditionOutputTypeDef definition

class OrConditionOutputTypeDef(TypedDict):
    andConditions: NotRequired[List[TagConditionTypeDef]],  # (1)
    tagCondition: NotRequired[TagConditionTypeDef],  # (2)
```

1. See [:material-code-braces: TagConditionTypeDef](./type_defs.md#tagconditiontypedef) 
2. See [:material-code-braces: TagConditionTypeDef](./type_defs.md#tagconditiontypedef) 
## OrConditionTypeDef

```python
# OrConditionTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import OrConditionTypeDef


def get_value() -> OrConditionTypeDef:
    return {
        "andConditions": ...,
    }


# OrConditionTypeDef definition

class OrConditionTypeDef(TypedDict):
    andConditions: NotRequired[Sequence[TagConditionTypeDef]],  # (1)
    tagCondition: NotRequired[TagConditionTypeDef],  # (2)
```

1. See [:material-code-braces: TagConditionTypeDef](./type_defs.md#tagconditiontypedef) 
2. See [:material-code-braces: TagConditionTypeDef](./type_defs.md#tagconditiontypedef) 
## QueryConditionTypeDef

```python
# QueryConditionTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import QueryConditionTypeDef


def get_value() -> QueryConditionTypeDef:
    return {
        "single": ...,
    }


# QueryConditionTypeDef definition

class QueryConditionTypeDef(TypedDict):
    single: NotRequired[QueryConditionItemTypeDef],  # (1)
```

1. See [:material-code-braces: QueryConditionItemTypeDef](./type_defs.md#queryconditionitemtypedef) 
## QueryInputDataTypeDef

```python
# QueryInputDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import QueryInputDataTypeDef


def get_value() -> QueryInputDataTypeDef:
    return {
        "intentInputData": ...,
    }


# QueryInputDataTypeDef definition

class QueryInputDataTypeDef(TypedDict):
    intentInputData: NotRequired[IntentInputDataTypeDef],  # (1)
    queryTextInputData: NotRequired[QueryTextInputDataTypeDef],  # (2)
```

1. See [:material-code-braces: IntentInputDataTypeDef](./type_defs.md#intentinputdatatypedef) 
2. See [:material-code-braces: QueryTextInputDataTypeDef](./type_defs.md#querytextinputdatatypedef) 
## RecommendationTriggerDataTypeDef

```python
# RecommendationTriggerDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import RecommendationTriggerDataTypeDef


def get_value() -> RecommendationTriggerDataTypeDef:
    return {
        "query": ...,
    }


# RecommendationTriggerDataTypeDef definition

class RecommendationTriggerDataTypeDef(TypedDict):
    query: NotRequired[QueryRecommendationTriggerDataTypeDef],  # (1)
```

1. See [:material-code-braces: QueryRecommendationTriggerDataTypeDef](./type_defs.md#queryrecommendationtriggerdatatypedef) 
## QuickResponseContentsTypeDef

```python
# QuickResponseContentsTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import QuickResponseContentsTypeDef


def get_value() -> QuickResponseContentsTypeDef:
    return {
        "markdown": ...,
    }


# QuickResponseContentsTypeDef definition

class QuickResponseContentsTypeDef(TypedDict):
    markdown: NotRequired[QuickResponseContentProviderTypeDef],  # (1)
    plainText: NotRequired[QuickResponseContentProviderTypeDef],  # (1)
```

1. See [:material-code-braces: QuickResponseContentProviderTypeDef](./type_defs.md#quickresponsecontentprovidertypedef) 
2. See [:material-code-braces: QuickResponseContentProviderTypeDef](./type_defs.md#quickresponsecontentprovidertypedef) 
## QuickResponseSearchExpressionTypeDef

```python
# QuickResponseSearchExpressionTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import QuickResponseSearchExpressionTypeDef


def get_value() -> QuickResponseSearchExpressionTypeDef:
    return {
        "filters": ...,
    }


# QuickResponseSearchExpressionTypeDef definition

class QuickResponseSearchExpressionTypeDef(TypedDict):
    filters: NotRequired[Sequence[QuickResponseFilterFieldTypeDef]],  # (1)
    orderOnField: NotRequired[QuickResponseOrderFieldTypeDef],  # (2)
    queries: NotRequired[Sequence[QuickResponseQueryFieldTypeDef]],  # (3)
```

1. See [:material-code-braces: QuickResponseFilterFieldTypeDef](./type_defs.md#quickresponsefilterfieldtypedef) 
2. See [:material-code-braces: QuickResponseOrderFieldTypeDef](./type_defs.md#quickresponseorderfieldtypedef) 
3. See [:material-code-braces: QuickResponseQueryFieldTypeDef](./type_defs.md#quickresponsequeryfieldtypedef) 
## RuntimeSessionDataTypeDef

```python
# RuntimeSessionDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import RuntimeSessionDataTypeDef


def get_value() -> RuntimeSessionDataTypeDef:
    return {
        "key": ...,
    }


# RuntimeSessionDataTypeDef definition

class RuntimeSessionDataTypeDef(TypedDict):
    key: str,
    value: RuntimeSessionDataValueTypeDef,  # (1)
```

1. See [:material-code-braces: RuntimeSessionDataValueTypeDef](./type_defs.md#runtimesessiondatavaluetypedef) 
## SearchSessionsResponseTypeDef

```python
# SearchSessionsResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SearchSessionsResponseTypeDef


def get_value() -> SearchSessionsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# SearchSessionsResponseTypeDef definition

class SearchSessionsResponseTypeDef(TypedDict):
    sessionSummaries: List[SessionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SessionSummaryTypeDef](./type_defs.md#sessionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UrlConfigurationOutputTypeDef

```python
# UrlConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UrlConfigurationOutputTypeDef


def get_value() -> UrlConfigurationOutputTypeDef:
    return {
        "seedUrls": ...,
    }


# UrlConfigurationOutputTypeDef definition

class UrlConfigurationOutputTypeDef(TypedDict):
    seedUrls: NotRequired[List[SeedUrlTypeDef]],  # (1)
```

1. See [:material-code-braces: SeedUrlTypeDef](./type_defs.md#seedurltypedef) 
## UrlConfigurationTypeDef

```python
# UrlConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UrlConfigurationTypeDef


def get_value() -> UrlConfigurationTypeDef:
    return {
        "seedUrls": ...,
    }


# UrlConfigurationTypeDef definition

class UrlConfigurationTypeDef(TypedDict):
    seedUrls: NotRequired[Sequence[SeedUrlTypeDef]],  # (1)
```

1. See [:material-code-braces: SeedUrlTypeDef](./type_defs.md#seedurltypedef) 
## SystemAttributesTypeDef

```python
# SystemAttributesTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SystemAttributesTypeDef


def get_value() -> SystemAttributesTypeDef:
    return {
        "customerEndpoint": ...,
    }


# SystemAttributesTypeDef definition

class SystemAttributesTypeDef(TypedDict):
    customerEndpoint: NotRequired[SystemEndpointAttributesTypeDef],  # (1)
    name: NotRequired[str],
    systemEndpoint: NotRequired[SystemEndpointAttributesTypeDef],  # (1)
```

1. See [:material-code-braces: SystemEndpointAttributesTypeDef](./type_defs.md#systemendpointattributestypedef) 
2. See [:material-code-braces: SystemEndpointAttributesTypeDef](./type_defs.md#systemendpointattributestypedef) 
## ListAIGuardrailVersionsResponseTypeDef

```python
# ListAIGuardrailVersionsResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAIGuardrailVersionsResponseTypeDef


def get_value() -> ListAIGuardrailVersionsResponseTypeDef:
    return {
        "aiGuardrailVersionSummaries": ...,
    }


# ListAIGuardrailVersionsResponseTypeDef definition

class ListAIGuardrailVersionsResponseTypeDef(TypedDict):
    aiGuardrailVersionSummaries: List[AIGuardrailVersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AIGuardrailVersionSummaryTypeDef](./type_defs.md#aiguardrailversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AIGuardrailDataTypeDef

```python
# AIGuardrailDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIGuardrailDataTypeDef


def get_value() -> AIGuardrailDataTypeDef:
    return {
        "aiGuardrailArn": ...,
    }


# AIGuardrailDataTypeDef definition

class AIGuardrailDataTypeDef(TypedDict):
    aiGuardrailArn: str,
    aiGuardrailId: str,
    assistantArn: str,
    assistantId: str,
    blockedInputMessaging: str,
    blockedOutputsMessaging: str,
    name: str,
    visibilityStatus: VisibilityStatusType,  # (6)
    contentPolicyConfig: NotRequired[AIGuardrailContentPolicyConfigOutputTypeDef],  # (1)
    contextualGroundingPolicyConfig: NotRequired[AIGuardrailContextualGroundingPolicyConfigOutputTypeDef],  # (2)
    description: NotRequired[str],
    modifiedTime: NotRequired[datetime],
    sensitiveInformationPolicyConfig: NotRequired[AIGuardrailSensitiveInformationPolicyConfigOutputTypeDef],  # (3)
    status: NotRequired[StatusType],  # (4)
    tags: NotRequired[Dict[str, str]],
    topicPolicyConfig: NotRequired[AIGuardrailTopicPolicyConfigOutputTypeDef],  # (5)
    wordPolicyConfig: NotRequired[AIGuardrailWordPolicyConfigOutputTypeDef],  # (7)
```

1. See [:material-code-braces: AIGuardrailContentPolicyConfigOutputTypeDef](./type_defs.md#aiguardrailcontentpolicyconfigoutputtypedef) 
2. See [:material-code-braces: AIGuardrailContextualGroundingPolicyConfigOutputTypeDef](./type_defs.md#aiguardrailcontextualgroundingpolicyconfigoutputtypedef) 
3. See [:material-code-braces: AIGuardrailSensitiveInformationPolicyConfigOutputTypeDef](./type_defs.md#aiguardrailsensitiveinformationpolicyconfigoutputtypedef) 
4. See [:material-code-brackets: StatusType](./literals.md#statustype) 
5. See [:material-code-braces: AIGuardrailTopicPolicyConfigOutputTypeDef](./type_defs.md#aiguardrailtopicpolicyconfigoutputtypedef) 
6. See [:material-code-brackets: VisibilityStatusType](./literals.md#visibilitystatustype) 
7. See [:material-code-braces: AIGuardrailWordPolicyConfigOutputTypeDef](./type_defs.md#aiguardrailwordpolicyconfigoutputtypedef) 
## ListAIPromptVersionsResponseTypeDef

```python
# ListAIPromptVersionsResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAIPromptVersionsResponseTypeDef


def get_value() -> ListAIPromptVersionsResponseTypeDef:
    return {
        "aiPromptVersionSummaries": ...,
    }


# ListAIPromptVersionsResponseTypeDef definition

class ListAIPromptVersionsResponseTypeDef(TypedDict):
    aiPromptVersionSummaries: List[AIPromptVersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AIPromptVersionSummaryTypeDef](./type_defs.md#aipromptversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AIPromptDataTypeDef

```python
# AIPromptDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIPromptDataTypeDef


def get_value() -> AIPromptDataTypeDef:
    return {
        "aiPromptArn": ...,
    }


# AIPromptDataTypeDef definition

class AIPromptDataTypeDef(TypedDict):
    aiPromptArn: str,
    aiPromptId: str,
    apiFormat: AIPromptAPIFormatType,  # (1)
    assistantArn: str,
    assistantId: str,
    modelId: str,
    name: str,
    templateConfiguration: AIPromptTemplateConfigurationTypeDef,  # (4)
    templateType: AIPromptTemplateTypeType,  # (5)
    type: AIPromptTypeType,  # (6)
    visibilityStatus: VisibilityStatusType,  # (7)
    description: NotRequired[str],
    modifiedTime: NotRequired[datetime],
    origin: NotRequired[OriginType],  # (2)
    status: NotRequired[StatusType],  # (3)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: AIPromptAPIFormatType](./literals.md#aipromptapiformattype) 
2. See [:material-code-brackets: OriginType](./literals.md#origintype) 
3. See [:material-code-brackets: StatusType](./literals.md#statustype) 
4. See [:material-code-braces: AIPromptTemplateConfigurationTypeDef](./type_defs.md#aiprompttemplateconfigurationtypedef) 
5. See [:material-code-brackets: AIPromptTemplateTypeType](./literals.md#aiprompttemplatetypetype) 
6. See [:material-code-brackets: AIPromptTypeType](./literals.md#aiprompttypetype) 
7. See [:material-code-brackets: VisibilityStatusType](./literals.md#visibilitystatustype) 
## CreateAIPromptRequestTypeDef

```python
# CreateAIPromptRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateAIPromptRequestTypeDef


def get_value() -> CreateAIPromptRequestTypeDef:
    return {
        "apiFormat": ...,
    }


# CreateAIPromptRequestTypeDef definition

class CreateAIPromptRequestTypeDef(TypedDict):
    apiFormat: AIPromptAPIFormatType,  # (1)
    assistantId: str,
    modelId: str,
    name: str,
    templateConfiguration: AIPromptTemplateConfigurationTypeDef,  # (2)
    templateType: AIPromptTemplateTypeType,  # (3)
    type: AIPromptTypeType,  # (4)
    visibilityStatus: VisibilityStatusType,  # (5)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: AIPromptAPIFormatType](./literals.md#aipromptapiformattype) 
2. See [:material-code-braces: AIPromptTemplateConfigurationTypeDef](./type_defs.md#aiprompttemplateconfigurationtypedef) 
3. See [:material-code-brackets: AIPromptTemplateTypeType](./literals.md#aiprompttemplatetypetype) 
4. See [:material-code-brackets: AIPromptTypeType](./literals.md#aiprompttypetype) 
5. See [:material-code-brackets: VisibilityStatusType](./literals.md#visibilitystatustype) 
## UpdateAIPromptRequestTypeDef

```python
# UpdateAIPromptRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UpdateAIPromptRequestTypeDef


def get_value() -> UpdateAIPromptRequestTypeDef:
    return {
        "aiPromptId": ...,
    }


# UpdateAIPromptRequestTypeDef definition

class UpdateAIPromptRequestTypeDef(TypedDict):
    aiPromptId: str,
    assistantId: str,
    visibilityStatus: VisibilityStatusType,  # (1)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    templateConfiguration: NotRequired[AIPromptTemplateConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: VisibilityStatusType](./literals.md#visibilitystatustype) 
2. See [:material-code-braces: AIPromptTemplateConfigurationTypeDef](./type_defs.md#aiprompttemplateconfigurationtypedef) 
## ContentAssociationDataTypeDef

```python
# ContentAssociationDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ContentAssociationDataTypeDef


def get_value() -> ContentAssociationDataTypeDef:
    return {
        "associationData": ...,
    }


# ContentAssociationDataTypeDef definition

class ContentAssociationDataTypeDef(TypedDict):
    associationData: ContentAssociationContentsTypeDef,  # (1)
    associationType: ContentAssociationTypeType,  # (2)
    contentArn: str,
    contentAssociationArn: str,
    contentAssociationId: str,
    contentId: str,
    knowledgeBaseArn: str,
    knowledgeBaseId: str,
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ContentAssociationContentsTypeDef](./type_defs.md#contentassociationcontentstypedef) 
2. See [:material-code-brackets: ContentAssociationTypeType](./literals.md#contentassociationtypetype) 
## ContentAssociationSummaryTypeDef

```python
# ContentAssociationSummaryTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ContentAssociationSummaryTypeDef


def get_value() -> ContentAssociationSummaryTypeDef:
    return {
        "associationData": ...,
    }


# ContentAssociationSummaryTypeDef definition

class ContentAssociationSummaryTypeDef(TypedDict):
    associationData: ContentAssociationContentsTypeDef,  # (1)
    associationType: ContentAssociationTypeType,  # (2)
    contentArn: str,
    contentAssociationArn: str,
    contentAssociationId: str,
    contentId: str,
    knowledgeBaseArn: str,
    knowledgeBaseId: str,
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ContentAssociationContentsTypeDef](./type_defs.md#contentassociationcontentstypedef) 
2. See [:material-code-brackets: ContentAssociationTypeType](./literals.md#contentassociationtypetype) 
## CreateContentAssociationRequestTypeDef

```python
# CreateContentAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateContentAssociationRequestTypeDef


def get_value() -> CreateContentAssociationRequestTypeDef:
    return {
        "association": ...,
    }


# CreateContentAssociationRequestTypeDef definition

class CreateContentAssociationRequestTypeDef(TypedDict):
    association: ContentAssociationContentsTypeDef,  # (1)
    associationType: ContentAssociationTypeType,  # (2)
    contentId: str,
    knowledgeBaseId: str,
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ContentAssociationContentsTypeDef](./type_defs.md#contentassociationcontentstypedef) 
2. See [:material-code-brackets: ContentAssociationTypeType](./literals.md#contentassociationtypetype) 
## AssistantAssociationDataTypeDef

```python
# AssistantAssociationDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AssistantAssociationDataTypeDef


def get_value() -> AssistantAssociationDataTypeDef:
    return {
        "assistantArn": ...,
    }


# AssistantAssociationDataTypeDef definition

class AssistantAssociationDataTypeDef(TypedDict):
    assistantArn: str,
    assistantAssociationArn: str,
    assistantAssociationId: str,
    assistantId: str,
    associationData: AssistantAssociationOutputDataTypeDef,  # (1)
    associationType: AssociationTypeType,  # (2)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: AssistantAssociationOutputDataTypeDef](./type_defs.md#assistantassociationoutputdatatypedef) 
2. See [:material-code-brackets: AssociationTypeType](./literals.md#associationtypetype) 
## AssistantAssociationSummaryTypeDef

```python
# AssistantAssociationSummaryTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AssistantAssociationSummaryTypeDef


def get_value() -> AssistantAssociationSummaryTypeDef:
    return {
        "assistantArn": ...,
    }


# AssistantAssociationSummaryTypeDef definition

class AssistantAssociationSummaryTypeDef(TypedDict):
    assistantArn: str,
    assistantAssociationArn: str,
    assistantAssociationId: str,
    assistantId: str,
    associationData: AssistantAssociationOutputDataTypeDef,  # (1)
    associationType: AssociationTypeType,  # (2)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: AssistantAssociationOutputDataTypeDef](./type_defs.md#assistantassociationoutputdatatypedef) 
2. See [:material-code-brackets: AssociationTypeType](./literals.md#associationtypetype) 
## CreateAssistantResponseTypeDef

```python
# CreateAssistantResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateAssistantResponseTypeDef


def get_value() -> CreateAssistantResponseTypeDef:
    return {
        "assistant": ...,
    }


# CreateAssistantResponseTypeDef definition

class CreateAssistantResponseTypeDef(TypedDict):
    assistant: AssistantDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssistantDataTypeDef](./type_defs.md#assistantdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAssistantResponseTypeDef

```python
# GetAssistantResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetAssistantResponseTypeDef


def get_value() -> GetAssistantResponseTypeDef:
    return {
        "assistant": ...,
    }


# GetAssistantResponseTypeDef definition

class GetAssistantResponseTypeDef(TypedDict):
    assistant: AssistantDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssistantDataTypeDef](./type_defs.md#assistantdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAssistantAIAgentResponseTypeDef

```python
# UpdateAssistantAIAgentResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UpdateAssistantAIAgentResponseTypeDef


def get_value() -> UpdateAssistantAIAgentResponseTypeDef:
    return {
        "assistant": ...,
    }


# UpdateAssistantAIAgentResponseTypeDef definition

class UpdateAssistantAIAgentResponseTypeDef(TypedDict):
    assistant: AssistantDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssistantDataTypeDef](./type_defs.md#assistantdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssistantsResponseTypeDef

```python
# ListAssistantsResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAssistantsResponseTypeDef


def get_value() -> ListAssistantsResponseTypeDef:
    return {
        "assistantSummaries": ...,
    }


# ListAssistantsResponseTypeDef definition

class ListAssistantsResponseTypeDef(TypedDict):
    assistantSummaries: List[AssistantSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssistantSummaryTypeDef](./type_defs.md#assistantsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ParsingConfigurationTypeDef

```python
# ParsingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ParsingConfigurationTypeDef


def get_value() -> ParsingConfigurationTypeDef:
    return {
        "bedrockFoundationModelConfiguration": ...,
    }


# ParsingConfigurationTypeDef definition

class ParsingConfigurationTypeDef(TypedDict):
    parsingStrategy: ParsingStrategyType,  # (2)
    bedrockFoundationModelConfiguration: NotRequired[BedrockFoundationModelConfigurationForParsingTypeDef],  # (1)
```

1. See [:material-code-braces: BedrockFoundationModelConfigurationForParsingTypeDef](./type_defs.md#bedrockfoundationmodelconfigurationforparsingtypedef) 
2. See [:material-code-brackets: ParsingStrategyType](./literals.md#parsingstrategytype) 
## ExternalSourceConfigurationTypeDef

```python
# ExternalSourceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ExternalSourceConfigurationTypeDef


def get_value() -> ExternalSourceConfigurationTypeDef:
    return {
        "configuration": ...,
    }


# ExternalSourceConfigurationTypeDef definition

class ExternalSourceConfigurationTypeDef(TypedDict):
    configuration: ConfigurationTypeDef,  # (1)
    source: ExternalSourceType,  # (2)
```

1. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) 
2. See [:material-code-brackets: ExternalSourceType](./literals.md#externalsourcetype) 
## PutFeedbackRequestTypeDef

```python
# PutFeedbackRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import PutFeedbackRequestTypeDef


def get_value() -> PutFeedbackRequestTypeDef:
    return {
        "assistantId": ...,
    }


# PutFeedbackRequestTypeDef definition

class PutFeedbackRequestTypeDef(TypedDict):
    assistantId: str,
    contentFeedback: ContentFeedbackDataTypeDef,  # (1)
    targetId: str,
    targetType: TargetTypeType,  # (2)
```

1. See [:material-code-braces: ContentFeedbackDataTypeDef](./type_defs.md#contentfeedbackdatatypedef) 
2. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
## PutFeedbackResponseTypeDef

```python
# PutFeedbackResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import PutFeedbackResponseTypeDef


def get_value() -> PutFeedbackResponseTypeDef:
    return {
        "assistantArn": ...,
    }


# PutFeedbackResponseTypeDef definition

class PutFeedbackResponseTypeDef(TypedDict):
    assistantArn: str,
    assistantId: str,
    contentFeedback: ContentFeedbackDataTypeDef,  # (1)
    targetId: str,
    targetType: TargetTypeType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ContentFeedbackDataTypeDef](./type_defs.md#contentfeedbackdatatypedef) 
2. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DocumentTypeDef

```python
# DocumentTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DocumentTypeDef


def get_value() -> DocumentTypeDef:
    return {
        "contentReference": ...,
    }


# DocumentTypeDef definition

class DocumentTypeDef(TypedDict):
    contentReference: ContentReferenceTypeDef,  # (1)
    excerpt: NotRequired[DocumentTextTypeDef],  # (2)
    title: NotRequired[DocumentTextTypeDef],  # (2)
```

1. See [:material-code-braces: ContentReferenceTypeDef](./type_defs.md#contentreferencetypedef) 
2. See [:material-code-braces: DocumentTextTypeDef](./type_defs.md#documenttexttypedef) 
3. See [:material-code-braces: DocumentTextTypeDef](./type_defs.md#documenttexttypedef) 
## TextDataTypeDef

```python
# TextDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import TextDataTypeDef


def get_value() -> TextDataTypeDef:
    return {
        "excerpt": ...,
    }


# TextDataTypeDef definition

class TextDataTypeDef(TypedDict):
    excerpt: NotRequired[DocumentTextTypeDef],  # (1)
    title: NotRequired[DocumentTextTypeDef],  # (1)
```

1. See [:material-code-braces: DocumentTextTypeDef](./type_defs.md#documenttexttypedef) 
2. See [:material-code-braces: DocumentTextTypeDef](./type_defs.md#documenttexttypedef) 
## EmailMessageTemplateContentOutputTypeDef

```python
# EmailMessageTemplateContentOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import EmailMessageTemplateContentOutputTypeDef


def get_value() -> EmailMessageTemplateContentOutputTypeDef:
    return {
        "body": ...,
    }


# EmailMessageTemplateContentOutputTypeDef definition

class EmailMessageTemplateContentOutputTypeDef(TypedDict):
    body: NotRequired[EmailMessageTemplateContentBodyTypeDef],  # (1)
    headers: NotRequired[List[EmailHeaderTypeDef]],  # (2)
    subject: NotRequired[str],
```

1. See [:material-code-braces: EmailMessageTemplateContentBodyTypeDef](./type_defs.md#emailmessagetemplatecontentbodytypedef) 
2. See [:material-code-braces: EmailHeaderTypeDef](./type_defs.md#emailheadertypedef) 
## EmailMessageTemplateContentTypeDef

```python
# EmailMessageTemplateContentTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import EmailMessageTemplateContentTypeDef


def get_value() -> EmailMessageTemplateContentTypeDef:
    return {
        "body": ...,
    }


# EmailMessageTemplateContentTypeDef definition

class EmailMessageTemplateContentTypeDef(TypedDict):
    body: NotRequired[EmailMessageTemplateContentBodyTypeDef],  # (1)
    headers: NotRequired[Sequence[EmailHeaderTypeDef]],  # (2)
    subject: NotRequired[str],
```

1. See [:material-code-braces: EmailMessageTemplateContentBodyTypeDef](./type_defs.md#emailmessagetemplatecontentbodytypedef) 
2. See [:material-code-braces: EmailHeaderTypeDef](./type_defs.md#emailheadertypedef) 
## SMSMessageTemplateContentTypeDef

```python
# SMSMessageTemplateContentTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SMSMessageTemplateContentTypeDef


def get_value() -> SMSMessageTemplateContentTypeDef:
    return {
        "body": ...,
    }


# SMSMessageTemplateContentTypeDef definition

class SMSMessageTemplateContentTypeDef(TypedDict):
    body: NotRequired[SMSMessageTemplateContentBodyTypeDef],  # (1)
```

1. See [:material-code-braces: SMSMessageTemplateContentBodyTypeDef](./type_defs.md#smsmessagetemplatecontentbodytypedef) 
## SearchMessageTemplatesResponseTypeDef

```python
# SearchMessageTemplatesResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SearchMessageTemplatesResponseTypeDef


def get_value() -> SearchMessageTemplatesResponseTypeDef:
    return {
        "nextToken": ...,
    }


# SearchMessageTemplatesResponseTypeDef definition

class SearchMessageTemplatesResponseTypeDef(TypedDict):
    results: List[MessageTemplateSearchResultDataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MessageTemplateSearchResultDataTypeDef](./type_defs.md#messagetemplatesearchresultdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchContentRequestPaginateTypeDef

```python
# SearchContentRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SearchContentRequestPaginateTypeDef


def get_value() -> SearchContentRequestPaginateTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# SearchContentRequestPaginateTypeDef definition

class SearchContentRequestPaginateTypeDef(TypedDict):
    knowledgeBaseId: str,
    searchExpression: SearchExpressionTypeDef,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SearchExpressionTypeDef](./type_defs.md#searchexpressiontypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchContentRequestTypeDef

```python
# SearchContentRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SearchContentRequestTypeDef


def get_value() -> SearchContentRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# SearchContentRequestTypeDef definition

class SearchContentRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    searchExpression: SearchExpressionTypeDef,  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchExpressionTypeDef](./type_defs.md#searchexpressiontypedef) 
## SearchSessionsRequestPaginateTypeDef

```python
# SearchSessionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SearchSessionsRequestPaginateTypeDef


def get_value() -> SearchSessionsRequestPaginateTypeDef:
    return {
        "assistantId": ...,
    }


# SearchSessionsRequestPaginateTypeDef definition

class SearchSessionsRequestPaginateTypeDef(TypedDict):
    assistantId: str,
    searchExpression: SearchExpressionTypeDef,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SearchExpressionTypeDef](./type_defs.md#searchexpressiontypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchSessionsRequestTypeDef

```python
# SearchSessionsRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SearchSessionsRequestTypeDef


def get_value() -> SearchSessionsRequestTypeDef:
    return {
        "assistantId": ...,
    }


# SearchSessionsRequestTypeDef definition

class SearchSessionsRequestTypeDef(TypedDict):
    assistantId: str,
    searchExpression: SearchExpressionTypeDef,  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchExpressionTypeDef](./type_defs.md#searchexpressiontypedef) 
## CreateQuickResponseRequestTypeDef

```python
# CreateQuickResponseRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateQuickResponseRequestTypeDef


def get_value() -> CreateQuickResponseRequestTypeDef:
    return {
        "content": ...,
    }


# CreateQuickResponseRequestTypeDef definition

class CreateQuickResponseRequestTypeDef(TypedDict):
    content: QuickResponseDataProviderTypeDef,  # (1)
    knowledgeBaseId: str,
    name: str,
    channels: NotRequired[Sequence[str]],
    clientToken: NotRequired[str],
    contentType: NotRequired[str],
    description: NotRequired[str],
    groupingConfiguration: NotRequired[GroupingConfigurationUnionTypeDef],  # (2)
    isActive: NotRequired[bool],
    language: NotRequired[str],
    shortcutKey: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: QuickResponseDataProviderTypeDef](./type_defs.md#quickresponsedataprovidertypedef) 
2. See [:material-code-braces: GroupingConfigurationTypeDef](./type_defs.md#groupingconfigurationtypedef) [:material-code-braces: GroupingConfigurationOutputTypeDef](./type_defs.md#groupingconfigurationoutputtypedef) 
## UpdateMessageTemplateMetadataRequestTypeDef

```python
# UpdateMessageTemplateMetadataRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UpdateMessageTemplateMetadataRequestTypeDef


def get_value() -> UpdateMessageTemplateMetadataRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# UpdateMessageTemplateMetadataRequestTypeDef definition

class UpdateMessageTemplateMetadataRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    messageTemplateId: str,
    description: NotRequired[str],
    groupingConfiguration: NotRequired[GroupingConfigurationUnionTypeDef],  # (1)
    name: NotRequired[str],
```

1. See [:material-code-braces: GroupingConfigurationTypeDef](./type_defs.md#groupingconfigurationtypedef) [:material-code-braces: GroupingConfigurationOutputTypeDef](./type_defs.md#groupingconfigurationoutputtypedef) 
## UpdateQuickResponseRequestTypeDef

```python
# UpdateQuickResponseRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UpdateQuickResponseRequestTypeDef


def get_value() -> UpdateQuickResponseRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# UpdateQuickResponseRequestTypeDef definition

class UpdateQuickResponseRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    quickResponseId: str,
    channels: NotRequired[Sequence[str]],
    content: NotRequired[QuickResponseDataProviderTypeDef],  # (1)
    contentType: NotRequired[str],
    description: NotRequired[str],
    groupingConfiguration: NotRequired[GroupingConfigurationUnionTypeDef],  # (2)
    isActive: NotRequired[bool],
    language: NotRequired[str],
    name: NotRequired[str],
    removeDescription: NotRequired[bool],
    removeGroupingConfiguration: NotRequired[bool],
    removeShortcutKey: NotRequired[bool],
    shortcutKey: NotRequired[str],
```

1. See [:material-code-braces: QuickResponseDataProviderTypeDef](./type_defs.md#quickresponsedataprovidertypedef) 
2. See [:material-code-braces: GroupingConfigurationTypeDef](./type_defs.md#groupingconfigurationtypedef) [:material-code-braces: GroupingConfigurationOutputTypeDef](./type_defs.md#groupingconfigurationoutputtypedef) 
## ChunkingConfigurationOutputTypeDef

```python
# ChunkingConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ChunkingConfigurationOutputTypeDef


def get_value() -> ChunkingConfigurationOutputTypeDef:
    return {
        "chunkingStrategy": ...,
    }


# ChunkingConfigurationOutputTypeDef definition

class ChunkingConfigurationOutputTypeDef(TypedDict):
    chunkingStrategy: ChunkingStrategyType,  # (1)
    fixedSizeChunkingConfiguration: NotRequired[FixedSizeChunkingConfigurationTypeDef],  # (2)
    hierarchicalChunkingConfiguration: NotRequired[HierarchicalChunkingConfigurationOutputTypeDef],  # (3)
    semanticChunkingConfiguration: NotRequired[SemanticChunkingConfigurationTypeDef],  # (4)
```

1. See [:material-code-brackets: ChunkingStrategyType](./literals.md#chunkingstrategytype) 
2. See [:material-code-braces: FixedSizeChunkingConfigurationTypeDef](./type_defs.md#fixedsizechunkingconfigurationtypedef) 
3. See [:material-code-braces: HierarchicalChunkingConfigurationOutputTypeDef](./type_defs.md#hierarchicalchunkingconfigurationoutputtypedef) 
4. See [:material-code-braces: SemanticChunkingConfigurationTypeDef](./type_defs.md#semanticchunkingconfigurationtypedef) 
## ChunkingConfigurationTypeDef

```python
# ChunkingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ChunkingConfigurationTypeDef


def get_value() -> ChunkingConfigurationTypeDef:
    return {
        "chunkingStrategy": ...,
    }


# ChunkingConfigurationTypeDef definition

class ChunkingConfigurationTypeDef(TypedDict):
    chunkingStrategy: ChunkingStrategyType,  # (1)
    fixedSizeChunkingConfiguration: NotRequired[FixedSizeChunkingConfigurationTypeDef],  # (2)
    hierarchicalChunkingConfiguration: NotRequired[HierarchicalChunkingConfigurationTypeDef],  # (3)
    semanticChunkingConfiguration: NotRequired[SemanticChunkingConfigurationTypeDef],  # (4)
```

1. See [:material-code-brackets: ChunkingStrategyType](./literals.md#chunkingstrategytype) 
2. See [:material-code-braces: FixedSizeChunkingConfigurationTypeDef](./type_defs.md#fixedsizechunkingconfigurationtypedef) 
3. See [:material-code-braces: HierarchicalChunkingConfigurationTypeDef](./type_defs.md#hierarchicalchunkingconfigurationtypedef) 
4. See [:material-code-braces: SemanticChunkingConfigurationTypeDef](./type_defs.md#semanticchunkingconfigurationtypedef) 
## MessageInputTypeDef

```python
# MessageInputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import MessageInputTypeDef


def get_value() -> MessageInputTypeDef:
    return {
        "value": ...,
    }


# MessageInputTypeDef definition

class MessageInputTypeDef(TypedDict):
    value: MessageDataTypeDef,  # (1)
```

1. See [:material-code-braces: MessageDataTypeDef](./type_defs.md#messagedatatypedef) 
## MessageOutputTypeDef

```python
# MessageOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import MessageOutputTypeDef


def get_value() -> MessageOutputTypeDef:
    return {
        "messageId": ...,
    }


# MessageOutputTypeDef definition

class MessageOutputTypeDef(TypedDict):
    messageId: str,
    participant: ParticipantType,  # (1)
    timestamp: datetime,
    value: MessageDataTypeDef,  # (2)
```

1. See [:material-code-brackets: ParticipantType](./literals.md#participanttype) 
2. See [:material-code-braces: MessageDataTypeDef](./type_defs.md#messagedatatypedef) 
## SearchMessageTemplatesRequestPaginateTypeDef

```python
# SearchMessageTemplatesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SearchMessageTemplatesRequestPaginateTypeDef


def get_value() -> SearchMessageTemplatesRequestPaginateTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# SearchMessageTemplatesRequestPaginateTypeDef definition

class SearchMessageTemplatesRequestPaginateTypeDef(TypedDict):
    knowledgeBaseId: str,
    searchExpression: MessageTemplateSearchExpressionTypeDef,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: MessageTemplateSearchExpressionTypeDef](./type_defs.md#messagetemplatesearchexpressiontypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchMessageTemplatesRequestTypeDef

```python
# SearchMessageTemplatesRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SearchMessageTemplatesRequestTypeDef


def get_value() -> SearchMessageTemplatesRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# SearchMessageTemplatesRequestTypeDef definition

class SearchMessageTemplatesRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    searchExpression: MessageTemplateSearchExpressionTypeDef,  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MessageTemplateSearchExpressionTypeDef](./type_defs.md#messagetemplatesearchexpressiontypedef) 
## TagFilterOutputTypeDef

```python
# TagFilterOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import TagFilterOutputTypeDef


def get_value() -> TagFilterOutputTypeDef:
    return {
        "andConditions": ...,
    }


# TagFilterOutputTypeDef definition

class TagFilterOutputTypeDef(TypedDict):
    andConditions: NotRequired[List[TagConditionTypeDef]],  # (1)
    orConditions: NotRequired[List[OrConditionOutputTypeDef]],  # (2)
    tagCondition: NotRequired[TagConditionTypeDef],  # (3)
```

1. See [:material-code-braces: TagConditionTypeDef](./type_defs.md#tagconditiontypedef) 
2. See [:material-code-braces: OrConditionOutputTypeDef](./type_defs.md#orconditionoutputtypedef) 
3. See [:material-code-braces: TagConditionTypeDef](./type_defs.md#tagconditiontypedef) 
## TagFilterTypeDef

```python
# TagFilterTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import TagFilterTypeDef


def get_value() -> TagFilterTypeDef:
    return {
        "andConditions": ...,
    }


# TagFilterTypeDef definition

class TagFilterTypeDef(TypedDict):
    andConditions: NotRequired[Sequence[TagConditionTypeDef]],  # (1)
    orConditions: NotRequired[Sequence[OrConditionTypeDef]],  # (2)
    tagCondition: NotRequired[TagConditionTypeDef],  # (3)
```

1. See [:material-code-braces: TagConditionTypeDef](./type_defs.md#tagconditiontypedef) 
2. See [:material-code-braces: OrConditionTypeDef](./type_defs.md#orconditiontypedef) 
3. See [:material-code-braces: TagConditionTypeDef](./type_defs.md#tagconditiontypedef) 
## QueryAssistantRequestPaginateTypeDef

```python
# QueryAssistantRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import QueryAssistantRequestPaginateTypeDef


def get_value() -> QueryAssistantRequestPaginateTypeDef:
    return {
        "assistantId": ...,
    }


# QueryAssistantRequestPaginateTypeDef definition

class QueryAssistantRequestPaginateTypeDef(TypedDict):
    assistantId: str,
    overrideKnowledgeBaseSearchType: NotRequired[KnowledgeBaseSearchTypeType],  # (1)
    queryCondition: NotRequired[Sequence[QueryConditionTypeDef]],  # (2)
    queryInputData: NotRequired[QueryInputDataTypeDef],  # (3)
    queryText: NotRequired[str],
    sessionId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: KnowledgeBaseSearchTypeType](./literals.md#knowledgebasesearchtypetype) 
2. See [:material-code-braces: QueryConditionTypeDef](./type_defs.md#queryconditiontypedef) 
3. See [:material-code-braces: QueryInputDataTypeDef](./type_defs.md#queryinputdatatypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## QueryAssistantRequestTypeDef

```python
# QueryAssistantRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import QueryAssistantRequestTypeDef


def get_value() -> QueryAssistantRequestTypeDef:
    return {
        "assistantId": ...,
    }


# QueryAssistantRequestTypeDef definition

class QueryAssistantRequestTypeDef(TypedDict):
    assistantId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    overrideKnowledgeBaseSearchType: NotRequired[KnowledgeBaseSearchTypeType],  # (1)
    queryCondition: NotRequired[Sequence[QueryConditionTypeDef]],  # (2)
    queryInputData: NotRequired[QueryInputDataTypeDef],  # (3)
    queryText: NotRequired[str],
    sessionId: NotRequired[str],
```

1. See [:material-code-brackets: KnowledgeBaseSearchTypeType](./literals.md#knowledgebasesearchtypetype) 
2. See [:material-code-braces: QueryConditionTypeDef](./type_defs.md#queryconditiontypedef) 
3. See [:material-code-braces: QueryInputDataTypeDef](./type_defs.md#queryinputdatatypedef) 
## RecommendationTriggerTypeDef

```python
# RecommendationTriggerTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import RecommendationTriggerTypeDef


def get_value() -> RecommendationTriggerTypeDef:
    return {
        "data": ...,
    }


# RecommendationTriggerTypeDef definition

class RecommendationTriggerTypeDef(TypedDict):
    data: RecommendationTriggerDataTypeDef,  # (1)
    id: str,
    recommendationIds: List[str],
    source: RecommendationSourceTypeType,  # (2)
    type: RecommendationTriggerTypeType,  # (3)
```

1. See [:material-code-braces: RecommendationTriggerDataTypeDef](./type_defs.md#recommendationtriggerdatatypedef) 
2. See [:material-code-brackets: RecommendationSourceTypeType](./literals.md#recommendationsourcetypetype) 
3. See [:material-code-brackets: RecommendationTriggerTypeType](./literals.md#recommendationtriggertypetype) 
## QuickResponseDataTypeDef

```python
# QuickResponseDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import QuickResponseDataTypeDef


def get_value() -> QuickResponseDataTypeDef:
    return {
        "channels": ...,
    }


# QuickResponseDataTypeDef definition

class QuickResponseDataTypeDef(TypedDict):
    contentType: str,
    createdTime: datetime,
    knowledgeBaseArn: str,
    knowledgeBaseId: str,
    lastModifiedTime: datetime,
    name: str,
    quickResponseArn: str,
    quickResponseId: str,
    status: QuickResponseStatusType,  # (3)
    channels: NotRequired[List[str]],
    contents: NotRequired[QuickResponseContentsTypeDef],  # (1)
    description: NotRequired[str],
    groupingConfiguration: NotRequired[GroupingConfigurationOutputTypeDef],  # (2)
    isActive: NotRequired[bool],
    language: NotRequired[str],
    lastModifiedBy: NotRequired[str],
    shortcutKey: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: QuickResponseContentsTypeDef](./type_defs.md#quickresponsecontentstypedef) 
2. See [:material-code-braces: GroupingConfigurationOutputTypeDef](./type_defs.md#groupingconfigurationoutputtypedef) 
3. See [:material-code-brackets: QuickResponseStatusType](./literals.md#quickresponsestatustype) 
## QuickResponseSearchResultDataTypeDef

```python
# QuickResponseSearchResultDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import QuickResponseSearchResultDataTypeDef


def get_value() -> QuickResponseSearchResultDataTypeDef:
    return {
        "attributesInterpolated": ...,
    }


# QuickResponseSearchResultDataTypeDef definition

class QuickResponseSearchResultDataTypeDef(TypedDict):
    contentType: str,
    contents: QuickResponseContentsTypeDef,  # (1)
    createdTime: datetime,
    isActive: bool,
    knowledgeBaseArn: str,
    knowledgeBaseId: str,
    lastModifiedTime: datetime,
    name: str,
    quickResponseArn: str,
    quickResponseId: str,
    status: QuickResponseStatusType,  # (3)
    attributesInterpolated: NotRequired[List[str]],
    attributesNotInterpolated: NotRequired[List[str]],
    channels: NotRequired[List[str]],
    description: NotRequired[str],
    groupingConfiguration: NotRequired[GroupingConfigurationOutputTypeDef],  # (2)
    language: NotRequired[str],
    lastModifiedBy: NotRequired[str],
    shortcutKey: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: QuickResponseContentsTypeDef](./type_defs.md#quickresponsecontentstypedef) 
2. See [:material-code-braces: GroupingConfigurationOutputTypeDef](./type_defs.md#groupingconfigurationoutputtypedef) 
3. See [:material-code-brackets: QuickResponseStatusType](./literals.md#quickresponsestatustype) 
## SearchQuickResponsesRequestPaginateTypeDef

```python
# SearchQuickResponsesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SearchQuickResponsesRequestPaginateTypeDef


def get_value() -> SearchQuickResponsesRequestPaginateTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# SearchQuickResponsesRequestPaginateTypeDef definition

class SearchQuickResponsesRequestPaginateTypeDef(TypedDict):
    knowledgeBaseId: str,
    searchExpression: QuickResponseSearchExpressionTypeDef,  # (1)
    attributes: NotRequired[Mapping[str, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: QuickResponseSearchExpressionTypeDef](./type_defs.md#quickresponsesearchexpressiontypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchQuickResponsesRequestTypeDef

```python
# SearchQuickResponsesRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SearchQuickResponsesRequestTypeDef


def get_value() -> SearchQuickResponsesRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# SearchQuickResponsesRequestTypeDef definition

class SearchQuickResponsesRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    searchExpression: QuickResponseSearchExpressionTypeDef,  # (1)
    attributes: NotRequired[Mapping[str, str]],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: QuickResponseSearchExpressionTypeDef](./type_defs.md#quickresponsesearchexpressiontypedef) 
## UpdateSessionDataRequestTypeDef

```python
# UpdateSessionDataRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UpdateSessionDataRequestTypeDef


def get_value() -> UpdateSessionDataRequestTypeDef:
    return {
        "assistantId": ...,
    }


# UpdateSessionDataRequestTypeDef definition

class UpdateSessionDataRequestTypeDef(TypedDict):
    assistantId: str,
    data: Sequence[RuntimeSessionDataTypeDef],  # (1)
    sessionId: str,
    namespace: NotRequired[SessionDataNamespaceType],  # (2)
```

1. See [:material-code-braces: RuntimeSessionDataTypeDef](./type_defs.md#runtimesessiondatatypedef) 
2. See [:material-code-brackets: SessionDataNamespaceType](./literals.md#sessiondatanamespacetype) 
## UpdateSessionDataResponseTypeDef

```python
# UpdateSessionDataResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UpdateSessionDataResponseTypeDef


def get_value() -> UpdateSessionDataResponseTypeDef:
    return {
        "data": ...,
    }


# UpdateSessionDataResponseTypeDef definition

class UpdateSessionDataResponseTypeDef(TypedDict):
    data: List[RuntimeSessionDataTypeDef],  # (1)
    namespace: SessionDataNamespaceType,  # (2)
    sessionArn: str,
    sessionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RuntimeSessionDataTypeDef](./type_defs.md#runtimesessiondatatypedef) 
2. See [:material-code-brackets: SessionDataNamespaceType](./literals.md#sessiondatanamespacetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WebCrawlerConfigurationOutputTypeDef

```python
# WebCrawlerConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import WebCrawlerConfigurationOutputTypeDef


def get_value() -> WebCrawlerConfigurationOutputTypeDef:
    return {
        "crawlerLimits": ...,
    }


# WebCrawlerConfigurationOutputTypeDef definition

class WebCrawlerConfigurationOutputTypeDef(TypedDict):
    urlConfiguration: UrlConfigurationOutputTypeDef,  # (3)
    crawlerLimits: NotRequired[WebCrawlerLimitsTypeDef],  # (1)
    exclusionFilters: NotRequired[List[str]],
    inclusionFilters: NotRequired[List[str]],
    scope: NotRequired[WebScopeTypeType],  # (2)
```

1. See [:material-code-braces: WebCrawlerLimitsTypeDef](./type_defs.md#webcrawlerlimitstypedef) 
2. See [:material-code-brackets: WebScopeTypeType](./literals.md#webscopetypetype) 
3. See [:material-code-braces: UrlConfigurationOutputTypeDef](./type_defs.md#urlconfigurationoutputtypedef) 
## WebCrawlerConfigurationTypeDef

```python
# WebCrawlerConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import WebCrawlerConfigurationTypeDef


def get_value() -> WebCrawlerConfigurationTypeDef:
    return {
        "crawlerLimits": ...,
    }


# WebCrawlerConfigurationTypeDef definition

class WebCrawlerConfigurationTypeDef(TypedDict):
    urlConfiguration: UrlConfigurationTypeDef,  # (3)
    crawlerLimits: NotRequired[WebCrawlerLimitsTypeDef],  # (1)
    exclusionFilters: NotRequired[Sequence[str]],
    inclusionFilters: NotRequired[Sequence[str]],
    scope: NotRequired[WebScopeTypeType],  # (2)
```

1. See [:material-code-braces: WebCrawlerLimitsTypeDef](./type_defs.md#webcrawlerlimitstypedef) 
2. See [:material-code-brackets: WebScopeTypeType](./literals.md#webscopetypetype) 
3. See [:material-code-braces: UrlConfigurationTypeDef](./type_defs.md#urlconfigurationtypedef) 
## MessageTemplateAttributesOutputTypeDef

```python
# MessageTemplateAttributesOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import MessageTemplateAttributesOutputTypeDef


def get_value() -> MessageTemplateAttributesOutputTypeDef:
    return {
        "agentAttributes": ...,
    }


# MessageTemplateAttributesOutputTypeDef definition

class MessageTemplateAttributesOutputTypeDef(TypedDict):
    agentAttributes: NotRequired[AgentAttributesTypeDef],  # (1)
    customAttributes: NotRequired[Dict[str, str]],
    customerProfileAttributes: NotRequired[CustomerProfileAttributesOutputTypeDef],  # (2)
    systemAttributes: NotRequired[SystemAttributesTypeDef],  # (3)
```

1. See [:material-code-braces: AgentAttributesTypeDef](./type_defs.md#agentattributestypedef) 
2. See [:material-code-braces: CustomerProfileAttributesOutputTypeDef](./type_defs.md#customerprofileattributesoutputtypedef) 
3. See [:material-code-braces: SystemAttributesTypeDef](./type_defs.md#systemattributestypedef) 
## MessageTemplateAttributesTypeDef

```python
# MessageTemplateAttributesTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import MessageTemplateAttributesTypeDef


def get_value() -> MessageTemplateAttributesTypeDef:
    return {
        "agentAttributes": ...,
    }


# MessageTemplateAttributesTypeDef definition

class MessageTemplateAttributesTypeDef(TypedDict):
    agentAttributes: NotRequired[AgentAttributesTypeDef],  # (1)
    customAttributes: NotRequired[Mapping[str, str]],
    customerProfileAttributes: NotRequired[CustomerProfileAttributesTypeDef],  # (2)
    systemAttributes: NotRequired[SystemAttributesTypeDef],  # (3)
```

1. See [:material-code-braces: AgentAttributesTypeDef](./type_defs.md#agentattributestypedef) 
2. See [:material-code-braces: CustomerProfileAttributesTypeDef](./type_defs.md#customerprofileattributestypedef) 
3. See [:material-code-braces: SystemAttributesTypeDef](./type_defs.md#systemattributestypedef) 
## CreateAIGuardrailResponseTypeDef

```python
# CreateAIGuardrailResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateAIGuardrailResponseTypeDef


def get_value() -> CreateAIGuardrailResponseTypeDef:
    return {
        "aiGuardrail": ...,
    }


# CreateAIGuardrailResponseTypeDef definition

class CreateAIGuardrailResponseTypeDef(TypedDict):
    aiGuardrail: AIGuardrailDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AIGuardrailDataTypeDef](./type_defs.md#aiguardraildatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAIGuardrailVersionResponseTypeDef

```python
# CreateAIGuardrailVersionResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateAIGuardrailVersionResponseTypeDef


def get_value() -> CreateAIGuardrailVersionResponseTypeDef:
    return {
        "aiGuardrail": ...,
    }


# CreateAIGuardrailVersionResponseTypeDef definition

class CreateAIGuardrailVersionResponseTypeDef(TypedDict):
    aiGuardrail: AIGuardrailDataTypeDef,  # (1)
    versionNumber: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AIGuardrailDataTypeDef](./type_defs.md#aiguardraildatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAIGuardrailResponseTypeDef

```python
# GetAIGuardrailResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetAIGuardrailResponseTypeDef


def get_value() -> GetAIGuardrailResponseTypeDef:
    return {
        "aiGuardrail": ...,
    }


# GetAIGuardrailResponseTypeDef definition

class GetAIGuardrailResponseTypeDef(TypedDict):
    aiGuardrail: AIGuardrailDataTypeDef,  # (1)
    versionNumber: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AIGuardrailDataTypeDef](./type_defs.md#aiguardraildatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAIGuardrailResponseTypeDef

```python
# UpdateAIGuardrailResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UpdateAIGuardrailResponseTypeDef


def get_value() -> UpdateAIGuardrailResponseTypeDef:
    return {
        "aiGuardrail": ...,
    }


# UpdateAIGuardrailResponseTypeDef definition

class UpdateAIGuardrailResponseTypeDef(TypedDict):
    aiGuardrail: AIGuardrailDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AIGuardrailDataTypeDef](./type_defs.md#aiguardraildatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAIGuardrailRequestTypeDef

```python
# CreateAIGuardrailRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateAIGuardrailRequestTypeDef


def get_value() -> CreateAIGuardrailRequestTypeDef:
    return {
        "assistantId": ...,
    }


# CreateAIGuardrailRequestTypeDef definition

class CreateAIGuardrailRequestTypeDef(TypedDict):
    assistantId: str,
    blockedInputMessaging: str,
    blockedOutputsMessaging: str,
    name: str,
    visibilityStatus: VisibilityStatusType,  # (1)
    clientToken: NotRequired[str],
    contentPolicyConfig: NotRequired[AIGuardrailContentPolicyConfigUnionTypeDef],  # (2)
    contextualGroundingPolicyConfig: NotRequired[AIGuardrailContextualGroundingPolicyConfigUnionTypeDef],  # (3)
    description: NotRequired[str],
    sensitiveInformationPolicyConfig: NotRequired[AIGuardrailSensitiveInformationPolicyConfigUnionTypeDef],  # (4)
    tags: NotRequired[Mapping[str, str]],
    topicPolicyConfig: NotRequired[AIGuardrailTopicPolicyConfigUnionTypeDef],  # (5)
    wordPolicyConfig: NotRequired[AIGuardrailWordPolicyConfigUnionTypeDef],  # (6)
```

1. See [:material-code-brackets: VisibilityStatusType](./literals.md#visibilitystatustype) 
2. See [:material-code-braces: AIGuardrailContentPolicyConfigTypeDef](./type_defs.md#aiguardrailcontentpolicyconfigtypedef) [:material-code-braces: AIGuardrailContentPolicyConfigOutputTypeDef](./type_defs.md#aiguardrailcontentpolicyconfigoutputtypedef) 
3. See [:material-code-braces: AIGuardrailContextualGroundingPolicyConfigTypeDef](./type_defs.md#aiguardrailcontextualgroundingpolicyconfigtypedef) [:material-code-braces: AIGuardrailContextualGroundingPolicyConfigOutputTypeDef](./type_defs.md#aiguardrailcontextualgroundingpolicyconfigoutputtypedef) 
4. See [:material-code-braces: AIGuardrailSensitiveInformationPolicyConfigTypeDef](./type_defs.md#aiguardrailsensitiveinformationpolicyconfigtypedef) [:material-code-braces: AIGuardrailSensitiveInformationPolicyConfigOutputTypeDef](./type_defs.md#aiguardrailsensitiveinformationpolicyconfigoutputtypedef) 
5. See [:material-code-braces: AIGuardrailTopicPolicyConfigTypeDef](./type_defs.md#aiguardrailtopicpolicyconfigtypedef) [:material-code-braces: AIGuardrailTopicPolicyConfigOutputTypeDef](./type_defs.md#aiguardrailtopicpolicyconfigoutputtypedef) 
6. See [:material-code-braces: AIGuardrailWordPolicyConfigTypeDef](./type_defs.md#aiguardrailwordpolicyconfigtypedef) [:material-code-braces: AIGuardrailWordPolicyConfigOutputTypeDef](./type_defs.md#aiguardrailwordpolicyconfigoutputtypedef) 
## UpdateAIGuardrailRequestTypeDef

```python
# UpdateAIGuardrailRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UpdateAIGuardrailRequestTypeDef


def get_value() -> UpdateAIGuardrailRequestTypeDef:
    return {
        "aiGuardrailId": ...,
    }


# UpdateAIGuardrailRequestTypeDef definition

class UpdateAIGuardrailRequestTypeDef(TypedDict):
    aiGuardrailId: str,
    assistantId: str,
    blockedInputMessaging: str,
    blockedOutputsMessaging: str,
    visibilityStatus: VisibilityStatusType,  # (1)
    clientToken: NotRequired[str],
    contentPolicyConfig: NotRequired[AIGuardrailContentPolicyConfigUnionTypeDef],  # (2)
    contextualGroundingPolicyConfig: NotRequired[AIGuardrailContextualGroundingPolicyConfigUnionTypeDef],  # (3)
    description: NotRequired[str],
    sensitiveInformationPolicyConfig: NotRequired[AIGuardrailSensitiveInformationPolicyConfigUnionTypeDef],  # (4)
    topicPolicyConfig: NotRequired[AIGuardrailTopicPolicyConfigUnionTypeDef],  # (5)
    wordPolicyConfig: NotRequired[AIGuardrailWordPolicyConfigUnionTypeDef],  # (6)
```

1. See [:material-code-brackets: VisibilityStatusType](./literals.md#visibilitystatustype) 
2. See [:material-code-braces: AIGuardrailContentPolicyConfigTypeDef](./type_defs.md#aiguardrailcontentpolicyconfigtypedef) [:material-code-braces: AIGuardrailContentPolicyConfigOutputTypeDef](./type_defs.md#aiguardrailcontentpolicyconfigoutputtypedef) 
3. See [:material-code-braces: AIGuardrailContextualGroundingPolicyConfigTypeDef](./type_defs.md#aiguardrailcontextualgroundingpolicyconfigtypedef) [:material-code-braces: AIGuardrailContextualGroundingPolicyConfigOutputTypeDef](./type_defs.md#aiguardrailcontextualgroundingpolicyconfigoutputtypedef) 
4. See [:material-code-braces: AIGuardrailSensitiveInformationPolicyConfigTypeDef](./type_defs.md#aiguardrailsensitiveinformationpolicyconfigtypedef) [:material-code-braces: AIGuardrailSensitiveInformationPolicyConfigOutputTypeDef](./type_defs.md#aiguardrailsensitiveinformationpolicyconfigoutputtypedef) 
5. See [:material-code-braces: AIGuardrailTopicPolicyConfigTypeDef](./type_defs.md#aiguardrailtopicpolicyconfigtypedef) [:material-code-braces: AIGuardrailTopicPolicyConfigOutputTypeDef](./type_defs.md#aiguardrailtopicpolicyconfigoutputtypedef) 
6. See [:material-code-braces: AIGuardrailWordPolicyConfigTypeDef](./type_defs.md#aiguardrailwordpolicyconfigtypedef) [:material-code-braces: AIGuardrailWordPolicyConfigOutputTypeDef](./type_defs.md#aiguardrailwordpolicyconfigoutputtypedef) 
## CreateAIPromptResponseTypeDef

```python
# CreateAIPromptResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateAIPromptResponseTypeDef


def get_value() -> CreateAIPromptResponseTypeDef:
    return {
        "aiPrompt": ...,
    }


# CreateAIPromptResponseTypeDef definition

class CreateAIPromptResponseTypeDef(TypedDict):
    aiPrompt: AIPromptDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AIPromptDataTypeDef](./type_defs.md#aipromptdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAIPromptVersionResponseTypeDef

```python
# CreateAIPromptVersionResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateAIPromptVersionResponseTypeDef


def get_value() -> CreateAIPromptVersionResponseTypeDef:
    return {
        "aiPrompt": ...,
    }


# CreateAIPromptVersionResponseTypeDef definition

class CreateAIPromptVersionResponseTypeDef(TypedDict):
    aiPrompt: AIPromptDataTypeDef,  # (1)
    versionNumber: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AIPromptDataTypeDef](./type_defs.md#aipromptdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAIPromptResponseTypeDef

```python
# GetAIPromptResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetAIPromptResponseTypeDef


def get_value() -> GetAIPromptResponseTypeDef:
    return {
        "aiPrompt": ...,
    }


# GetAIPromptResponseTypeDef definition

class GetAIPromptResponseTypeDef(TypedDict):
    aiPrompt: AIPromptDataTypeDef,  # (1)
    versionNumber: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AIPromptDataTypeDef](./type_defs.md#aipromptdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAIPromptResponseTypeDef

```python
# UpdateAIPromptResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UpdateAIPromptResponseTypeDef


def get_value() -> UpdateAIPromptResponseTypeDef:
    return {
        "aiPrompt": ...,
    }


# UpdateAIPromptResponseTypeDef definition

class UpdateAIPromptResponseTypeDef(TypedDict):
    aiPrompt: AIPromptDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AIPromptDataTypeDef](./type_defs.md#aipromptdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateContentAssociationResponseTypeDef

```python
# CreateContentAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateContentAssociationResponseTypeDef


def get_value() -> CreateContentAssociationResponseTypeDef:
    return {
        "contentAssociation": ...,
    }


# CreateContentAssociationResponseTypeDef definition

class CreateContentAssociationResponseTypeDef(TypedDict):
    contentAssociation: ContentAssociationDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContentAssociationDataTypeDef](./type_defs.md#contentassociationdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetContentAssociationResponseTypeDef

```python
# GetContentAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetContentAssociationResponseTypeDef


def get_value() -> GetContentAssociationResponseTypeDef:
    return {
        "contentAssociation": ...,
    }


# GetContentAssociationResponseTypeDef definition

class GetContentAssociationResponseTypeDef(TypedDict):
    contentAssociation: ContentAssociationDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContentAssociationDataTypeDef](./type_defs.md#contentassociationdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListContentAssociationsResponseTypeDef

```python
# ListContentAssociationsResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListContentAssociationsResponseTypeDef


def get_value() -> ListContentAssociationsResponseTypeDef:
    return {
        "contentAssociationSummaries": ...,
    }


# ListContentAssociationsResponseTypeDef definition

class ListContentAssociationsResponseTypeDef(TypedDict):
    contentAssociationSummaries: List[ContentAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ContentAssociationSummaryTypeDef](./type_defs.md#contentassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAssistantAssociationResponseTypeDef

```python
# CreateAssistantAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateAssistantAssociationResponseTypeDef


def get_value() -> CreateAssistantAssociationResponseTypeDef:
    return {
        "assistantAssociation": ...,
    }


# CreateAssistantAssociationResponseTypeDef definition

class CreateAssistantAssociationResponseTypeDef(TypedDict):
    assistantAssociation: AssistantAssociationDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssistantAssociationDataTypeDef](./type_defs.md#assistantassociationdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAssistantAssociationResponseTypeDef

```python
# GetAssistantAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetAssistantAssociationResponseTypeDef


def get_value() -> GetAssistantAssociationResponseTypeDef:
    return {
        "assistantAssociation": ...,
    }


# GetAssistantAssociationResponseTypeDef definition

class GetAssistantAssociationResponseTypeDef(TypedDict):
    assistantAssociation: AssistantAssociationDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssistantAssociationDataTypeDef](./type_defs.md#assistantassociationdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssistantAssociationsResponseTypeDef

```python
# ListAssistantAssociationsResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAssistantAssociationsResponseTypeDef


def get_value() -> ListAssistantAssociationsResponseTypeDef:
    return {
        "assistantAssociationSummaries": ...,
    }


# ListAssistantAssociationsResponseTypeDef definition

class ListAssistantAssociationsResponseTypeDef(TypedDict):
    assistantAssociationSummaries: List[AssistantAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssistantAssociationSummaryTypeDef](./type_defs.md#assistantassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportJobDataTypeDef

```python
# ImportJobDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ImportJobDataTypeDef


def get_value() -> ImportJobDataTypeDef:
    return {
        "createdTime": ...,
    }


# ImportJobDataTypeDef definition

class ImportJobDataTypeDef(TypedDict):
    createdTime: datetime,
    importJobId: str,
    importJobType: ImportJobTypeType,  # (2)
    knowledgeBaseArn: str,
    knowledgeBaseId: str,
    lastModifiedTime: datetime,
    status: ImportJobStatusType,  # (3)
    uploadId: str,
    url: str,
    urlExpiry: datetime,
    externalSourceConfiguration: NotRequired[ExternalSourceConfigurationTypeDef],  # (1)
    failedRecordReport: NotRequired[str],
    metadata: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ExternalSourceConfigurationTypeDef](./type_defs.md#externalsourceconfigurationtypedef) 
2. See [:material-code-brackets: ImportJobTypeType](./literals.md#importjobtypetype) 
3. See [:material-code-brackets: ImportJobStatusType](./literals.md#importjobstatustype) 
## ImportJobSummaryTypeDef

```python
# ImportJobSummaryTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ImportJobSummaryTypeDef


def get_value() -> ImportJobSummaryTypeDef:
    return {
        "createdTime": ...,
    }


# ImportJobSummaryTypeDef definition

class ImportJobSummaryTypeDef(TypedDict):
    createdTime: datetime,
    importJobId: str,
    importJobType: ImportJobTypeType,  # (2)
    knowledgeBaseArn: str,
    knowledgeBaseId: str,
    lastModifiedTime: datetime,
    status: ImportJobStatusType,  # (3)
    uploadId: str,
    externalSourceConfiguration: NotRequired[ExternalSourceConfigurationTypeDef],  # (1)
    metadata: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ExternalSourceConfigurationTypeDef](./type_defs.md#externalsourceconfigurationtypedef) 
2. See [:material-code-brackets: ImportJobTypeType](./literals.md#importjobtypetype) 
3. See [:material-code-brackets: ImportJobStatusType](./literals.md#importjobstatustype) 
## StartImportJobRequestTypeDef

```python
# StartImportJobRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import StartImportJobRequestTypeDef


def get_value() -> StartImportJobRequestTypeDef:
    return {
        "importJobType": ...,
    }


# StartImportJobRequestTypeDef definition

class StartImportJobRequestTypeDef(TypedDict):
    importJobType: ImportJobTypeType,  # (1)
    knowledgeBaseId: str,
    uploadId: str,
    clientToken: NotRequired[str],
    externalSourceConfiguration: NotRequired[ExternalSourceConfigurationTypeDef],  # (2)
    metadata: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ImportJobTypeType](./literals.md#importjobtypetype) 
2. See [:material-code-braces: ExternalSourceConfigurationTypeDef](./type_defs.md#externalsourceconfigurationtypedef) 
## ContentDataDetailsTypeDef

```python
# ContentDataDetailsTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ContentDataDetailsTypeDef


def get_value() -> ContentDataDetailsTypeDef:
    return {
        "rankingData": ...,
    }


# ContentDataDetailsTypeDef definition

class ContentDataDetailsTypeDef(TypedDict):
    rankingData: RankingDataTypeDef,  # (1)
    textData: TextDataTypeDef,  # (2)
```

1. See [:material-code-braces: RankingDataTypeDef](./type_defs.md#rankingdatatypedef) 
2. See [:material-code-braces: TextDataTypeDef](./type_defs.md#textdatatypedef) 
## SourceContentDataDetailsTypeDef

```python
# SourceContentDataDetailsTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SourceContentDataDetailsTypeDef


def get_value() -> SourceContentDataDetailsTypeDef:
    return {
        "citationSpan": ...,
    }


# SourceContentDataDetailsTypeDef definition

class SourceContentDataDetailsTypeDef(TypedDict):
    id: str,
    rankingData: RankingDataTypeDef,  # (2)
    textData: TextDataTypeDef,  # (3)
    type: SourceContentTypeType,  # (4)
    citationSpan: NotRequired[CitationSpanTypeDef],  # (1)
```

1. See [:material-code-braces: CitationSpanTypeDef](./type_defs.md#citationspantypedef) 
2. See [:material-code-braces: RankingDataTypeDef](./type_defs.md#rankingdatatypedef) 
3. See [:material-code-braces: TextDataTypeDef](./type_defs.md#textdatatypedef) 
4. See [:material-code-brackets: SourceContentTypeType](./literals.md#sourcecontenttypetype) 
## MessageTemplateContentProviderOutputTypeDef

```python
# MessageTemplateContentProviderOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import MessageTemplateContentProviderOutputTypeDef


def get_value() -> MessageTemplateContentProviderOutputTypeDef:
    return {
        "email": ...,
    }


# MessageTemplateContentProviderOutputTypeDef definition

class MessageTemplateContentProviderOutputTypeDef(TypedDict):
    email: NotRequired[EmailMessageTemplateContentOutputTypeDef],  # (1)
    sms: NotRequired[SMSMessageTemplateContentTypeDef],  # (2)
```

1. See [:material-code-braces: EmailMessageTemplateContentOutputTypeDef](./type_defs.md#emailmessagetemplatecontentoutputtypedef) 
2. See [:material-code-braces: SMSMessageTemplateContentTypeDef](./type_defs.md#smsmessagetemplatecontenttypedef) 
## MessageTemplateContentProviderTypeDef

```python
# MessageTemplateContentProviderTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import MessageTemplateContentProviderTypeDef


def get_value() -> MessageTemplateContentProviderTypeDef:
    return {
        "email": ...,
    }


# MessageTemplateContentProviderTypeDef definition

class MessageTemplateContentProviderTypeDef(TypedDict):
    email: NotRequired[EmailMessageTemplateContentTypeDef],  # (1)
    sms: NotRequired[SMSMessageTemplateContentTypeDef],  # (2)
```

1. See [:material-code-braces: EmailMessageTemplateContentTypeDef](./type_defs.md#emailmessagetemplatecontenttypedef) 
2. See [:material-code-braces: SMSMessageTemplateContentTypeDef](./type_defs.md#smsmessagetemplatecontenttypedef) 
## VectorIngestionConfigurationOutputTypeDef

```python
# VectorIngestionConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import VectorIngestionConfigurationOutputTypeDef


def get_value() -> VectorIngestionConfigurationOutputTypeDef:
    return {
        "chunkingConfiguration": ...,
    }


# VectorIngestionConfigurationOutputTypeDef definition

class VectorIngestionConfigurationOutputTypeDef(TypedDict):
    chunkingConfiguration: NotRequired[ChunkingConfigurationOutputTypeDef],  # (1)
    parsingConfiguration: NotRequired[ParsingConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ChunkingConfigurationOutputTypeDef](./type_defs.md#chunkingconfigurationoutputtypedef) 
2. See [:material-code-braces: ParsingConfigurationTypeDef](./type_defs.md#parsingconfigurationtypedef) 
## VectorIngestionConfigurationTypeDef

```python
# VectorIngestionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import VectorIngestionConfigurationTypeDef


def get_value() -> VectorIngestionConfigurationTypeDef:
    return {
        "chunkingConfiguration": ...,
    }


# VectorIngestionConfigurationTypeDef definition

class VectorIngestionConfigurationTypeDef(TypedDict):
    chunkingConfiguration: NotRequired[ChunkingConfigurationTypeDef],  # (1)
    parsingConfiguration: NotRequired[ParsingConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ChunkingConfigurationTypeDef](./type_defs.md#chunkingconfigurationtypedef) 
2. See [:material-code-braces: ParsingConfigurationTypeDef](./type_defs.md#parsingconfigurationtypedef) 
## SendMessageRequestTypeDef

```python
# SendMessageRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SendMessageRequestTypeDef


def get_value() -> SendMessageRequestTypeDef:
    return {
        "assistantId": ...,
    }


# SendMessageRequestTypeDef definition

class SendMessageRequestTypeDef(TypedDict):
    assistantId: str,
    message: MessageInputTypeDef,  # (1)
    sessionId: str,
    type: MessageTypeType,  # (2)
    clientToken: NotRequired[str],
    conversationContext: NotRequired[ConversationContextTypeDef],  # (3)
```

1. See [:material-code-braces: MessageInputTypeDef](./type_defs.md#messageinputtypedef) 
2. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
3. See [:material-code-braces: ConversationContextTypeDef](./type_defs.md#conversationcontexttypedef) 
## GetNextMessageResponseTypeDef

```python
# GetNextMessageResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetNextMessageResponseTypeDef


def get_value() -> GetNextMessageResponseTypeDef:
    return {
        "conversationSessionData": ...,
    }


# GetNextMessageResponseTypeDef definition

class GetNextMessageResponseTypeDef(TypedDict):
    conversationSessionData: List[RuntimeSessionDataTypeDef],  # (1)
    conversationState: ConversationStateTypeDef,  # (2)
    nextMessageToken: str,
    requestMessageId: str,
    response: MessageOutputTypeDef,  # (3)
    type: MessageTypeType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: RuntimeSessionDataTypeDef](./type_defs.md#runtimesessiondatatypedef) 
2. See [:material-code-braces: ConversationStateTypeDef](./type_defs.md#conversationstatetypedef) 
3. See [:material-code-braces: MessageOutputTypeDef](./type_defs.md#messageoutputtypedef) 
4. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMessagesResponseTypeDef

```python
# ListMessagesResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListMessagesResponseTypeDef


def get_value() -> ListMessagesResponseTypeDef:
    return {
        "messages": ...,
    }


# ListMessagesResponseTypeDef definition

class ListMessagesResponseTypeDef(TypedDict):
    messages: List[MessageOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MessageOutputTypeDef](./type_defs.md#messageoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## KnowledgeBaseAssociationConfigurationDataOutputTypeDef

```python
# KnowledgeBaseAssociationConfigurationDataOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import KnowledgeBaseAssociationConfigurationDataOutputTypeDef


def get_value() -> KnowledgeBaseAssociationConfigurationDataOutputTypeDef:
    return {
        "contentTagFilter": ...,
    }


# KnowledgeBaseAssociationConfigurationDataOutputTypeDef definition

class KnowledgeBaseAssociationConfigurationDataOutputTypeDef(TypedDict):
    contentTagFilter: NotRequired[TagFilterOutputTypeDef],  # (1)
    maxResults: NotRequired[int],
    overrideKnowledgeBaseSearchType: NotRequired[KnowledgeBaseSearchTypeType],  # (2)
```

1. See [:material-code-braces: TagFilterOutputTypeDef](./type_defs.md#tagfilteroutputtypedef) 
2. See [:material-code-brackets: KnowledgeBaseSearchTypeType](./literals.md#knowledgebasesearchtypetype) 
## SessionDataTypeDef

```python
# SessionDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SessionDataTypeDef


def get_value() -> SessionDataTypeDef:
    return {
        "aiAgentConfiguration": ...,
    }


# SessionDataTypeDef definition

class SessionDataTypeDef(TypedDict):
    name: str,
    sessionArn: str,
    sessionId: str,
    aiAgentConfiguration: NotRequired[Dict[AIAgentTypeType, AIAgentConfigurationDataTypeDef]],  # (1)
    description: NotRequired[str],
    integrationConfiguration: NotRequired[SessionIntegrationConfigurationTypeDef],  # (2)
    tagFilter: NotRequired[TagFilterOutputTypeDef],  # (3)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: AIAgentTypeType](./literals.md#aiagenttypetype) [:material-code-braces: AIAgentConfigurationDataTypeDef](./type_defs.md#aiagentconfigurationdatatypedef) 
2. See [:material-code-braces: SessionIntegrationConfigurationTypeDef](./type_defs.md#sessionintegrationconfigurationtypedef) 
3. See [:material-code-braces: TagFilterOutputTypeDef](./type_defs.md#tagfilteroutputtypedef) 
## KnowledgeBaseAssociationConfigurationDataTypeDef

```python
# KnowledgeBaseAssociationConfigurationDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import KnowledgeBaseAssociationConfigurationDataTypeDef


def get_value() -> KnowledgeBaseAssociationConfigurationDataTypeDef:
    return {
        "contentTagFilter": ...,
    }


# KnowledgeBaseAssociationConfigurationDataTypeDef definition

class KnowledgeBaseAssociationConfigurationDataTypeDef(TypedDict):
    contentTagFilter: NotRequired[TagFilterTypeDef],  # (1)
    maxResults: NotRequired[int],
    overrideKnowledgeBaseSearchType: NotRequired[KnowledgeBaseSearchTypeType],  # (2)
```

1. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
2. See [:material-code-brackets: KnowledgeBaseSearchTypeType](./literals.md#knowledgebasesearchtypetype) 
## CreateQuickResponseResponseTypeDef

```python
# CreateQuickResponseResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateQuickResponseResponseTypeDef


def get_value() -> CreateQuickResponseResponseTypeDef:
    return {
        "quickResponse": ...,
    }


# CreateQuickResponseResponseTypeDef definition

class CreateQuickResponseResponseTypeDef(TypedDict):
    quickResponse: QuickResponseDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QuickResponseDataTypeDef](./type_defs.md#quickresponsedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetQuickResponseResponseTypeDef

```python
# GetQuickResponseResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetQuickResponseResponseTypeDef


def get_value() -> GetQuickResponseResponseTypeDef:
    return {
        "quickResponse": ...,
    }


# GetQuickResponseResponseTypeDef definition

class GetQuickResponseResponseTypeDef(TypedDict):
    quickResponse: QuickResponseDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QuickResponseDataTypeDef](./type_defs.md#quickresponsedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateQuickResponseResponseTypeDef

```python
# UpdateQuickResponseResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UpdateQuickResponseResponseTypeDef


def get_value() -> UpdateQuickResponseResponseTypeDef:
    return {
        "quickResponse": ...,
    }


# UpdateQuickResponseResponseTypeDef definition

class UpdateQuickResponseResponseTypeDef(TypedDict):
    quickResponse: QuickResponseDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QuickResponseDataTypeDef](./type_defs.md#quickresponsedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchQuickResponsesResponseTypeDef

```python
# SearchQuickResponsesResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SearchQuickResponsesResponseTypeDef


def get_value() -> SearchQuickResponsesResponseTypeDef:
    return {
        "nextToken": ...,
    }


# SearchQuickResponsesResponseTypeDef definition

class SearchQuickResponsesResponseTypeDef(TypedDict):
    results: List[QuickResponseSearchResultDataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: QuickResponseSearchResultDataTypeDef](./type_defs.md#quickresponsesearchresultdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ManagedSourceConfigurationOutputTypeDef

```python
# ManagedSourceConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ManagedSourceConfigurationOutputTypeDef


def get_value() -> ManagedSourceConfigurationOutputTypeDef:
    return {
        "webCrawlerConfiguration": ...,
    }


# ManagedSourceConfigurationOutputTypeDef definition

class ManagedSourceConfigurationOutputTypeDef(TypedDict):
    webCrawlerConfiguration: NotRequired[WebCrawlerConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: WebCrawlerConfigurationOutputTypeDef](./type_defs.md#webcrawlerconfigurationoutputtypedef) 
## ManagedSourceConfigurationTypeDef

```python
# ManagedSourceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ManagedSourceConfigurationTypeDef


def get_value() -> ManagedSourceConfigurationTypeDef:
    return {
        "webCrawlerConfiguration": ...,
    }


# ManagedSourceConfigurationTypeDef definition

class ManagedSourceConfigurationTypeDef(TypedDict):
    webCrawlerConfiguration: NotRequired[WebCrawlerConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: WebCrawlerConfigurationTypeDef](./type_defs.md#webcrawlerconfigurationtypedef) 
## GetImportJobResponseTypeDef

```python
# GetImportJobResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetImportJobResponseTypeDef


def get_value() -> GetImportJobResponseTypeDef:
    return {
        "importJob": ...,
    }


# GetImportJobResponseTypeDef definition

class GetImportJobResponseTypeDef(TypedDict):
    importJob: ImportJobDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImportJobDataTypeDef](./type_defs.md#importjobdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartImportJobResponseTypeDef

```python
# StartImportJobResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import StartImportJobResponseTypeDef


def get_value() -> StartImportJobResponseTypeDef:
    return {
        "importJob": ...,
    }


# StartImportJobResponseTypeDef definition

class StartImportJobResponseTypeDef(TypedDict):
    importJob: ImportJobDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImportJobDataTypeDef](./type_defs.md#importjobdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListImportJobsResponseTypeDef

```python
# ListImportJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListImportJobsResponseTypeDef


def get_value() -> ListImportJobsResponseTypeDef:
    return {
        "importJobSummaries": ...,
    }


# ListImportJobsResponseTypeDef definition

class ListImportJobsResponseTypeDef(TypedDict):
    importJobSummaries: List[ImportJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ImportJobSummaryTypeDef](./type_defs.md#importjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataDetailsPaginatorTypeDef

```python
# DataDetailsPaginatorTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DataDetailsPaginatorTypeDef


def get_value() -> DataDetailsPaginatorTypeDef:
    return {
        "contentData": ...,
    }


# DataDetailsPaginatorTypeDef definition

class DataDetailsPaginatorTypeDef(TypedDict):
    contentData: NotRequired[ContentDataDetailsTypeDef],  # (1)
    generativeData: NotRequired[GenerativeDataDetailsPaginatorTypeDef],  # (2)
    intentDetectedData: NotRequired[IntentDetectedDataDetailsTypeDef],  # (3)
    sourceContentData: NotRequired[SourceContentDataDetailsTypeDef],  # (4)
```

1. See [:material-code-braces: ContentDataDetailsTypeDef](./type_defs.md#contentdatadetailstypedef) 
2. See [:material-code-braces: GenerativeDataDetailsPaginatorTypeDef](./type_defs.md#generativedatadetailspaginatortypedef) 
3. See [:material-code-braces: IntentDetectedDataDetailsTypeDef](./type_defs.md#intentdetecteddatadetailstypedef) 
4. See [:material-code-braces: SourceContentDataDetailsTypeDef](./type_defs.md#sourcecontentdatadetailstypedef) 
## DataDetailsTypeDef

```python
# DataDetailsTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DataDetailsTypeDef


def get_value() -> DataDetailsTypeDef:
    return {
        "contentData": ...,
    }


# DataDetailsTypeDef definition

class DataDetailsTypeDef(TypedDict):
    contentData: NotRequired[ContentDataDetailsTypeDef],  # (1)
    generativeData: NotRequired[GenerativeDataDetailsTypeDef],  # (2)
    intentDetectedData: NotRequired[IntentDetectedDataDetailsTypeDef],  # (3)
    sourceContentData: NotRequired[SourceContentDataDetailsTypeDef],  # (4)
```

1. See [:material-code-braces: ContentDataDetailsTypeDef](./type_defs.md#contentdatadetailstypedef) 
2. See [:material-code-braces: GenerativeDataDetailsTypeDef](./type_defs.md#generativedatadetailstypedef) 
3. See [:material-code-braces: IntentDetectedDataDetailsTypeDef](./type_defs.md#intentdetecteddatadetailstypedef) 
4. See [:material-code-braces: SourceContentDataDetailsTypeDef](./type_defs.md#sourcecontentdatadetailstypedef) 
## ExtendedMessageTemplateDataTypeDef

```python
# ExtendedMessageTemplateDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ExtendedMessageTemplateDataTypeDef


def get_value() -> ExtendedMessageTemplateDataTypeDef:
    return {
        "attachments": ...,
    }


# ExtendedMessageTemplateDataTypeDef definition

class ExtendedMessageTemplateDataTypeDef(TypedDict):
    channelSubtype: ChannelSubtypeType,  # (3)
    content: MessageTemplateContentProviderOutputTypeDef,  # (4)
    createdTime: datetime,
    knowledgeBaseArn: str,
    knowledgeBaseId: str,
    lastModifiedBy: str,
    lastModifiedTime: datetime,
    messageTemplateArn: str,
    messageTemplateContentSha256: str,
    messageTemplateId: str,
    name: str,
    attachments: NotRequired[List[MessageTemplateAttachmentTypeDef]],  # (1)
    attributeTypes: NotRequired[List[MessageTemplateAttributeTypeType]],  # (2)
    defaultAttributes: NotRequired[MessageTemplateAttributesOutputTypeDef],  # (5)
    description: NotRequired[str],
    groupingConfiguration: NotRequired[GroupingConfigurationOutputTypeDef],  # (6)
    isActive: NotRequired[bool],
    language: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    versionNumber: NotRequired[int],
```

1. See [:material-code-braces: MessageTemplateAttachmentTypeDef](./type_defs.md#messagetemplateattachmenttypedef) 
2. See [:material-code-brackets: MessageTemplateAttributeTypeType](./literals.md#messagetemplateattributetypetype) 
3. See [:material-code-brackets: ChannelSubtypeType](./literals.md#channelsubtypetype) 
4. See [:material-code-braces: MessageTemplateContentProviderOutputTypeDef](./type_defs.md#messagetemplatecontentprovideroutputtypedef) 
5. See [:material-code-braces: MessageTemplateAttributesOutputTypeDef](./type_defs.md#messagetemplateattributesoutputtypedef) 
6. See [:material-code-braces: GroupingConfigurationOutputTypeDef](./type_defs.md#groupingconfigurationoutputtypedef) 
## MessageTemplateDataTypeDef

```python
# MessageTemplateDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import MessageTemplateDataTypeDef


def get_value() -> MessageTemplateDataTypeDef:
    return {
        "attributeTypes": ...,
    }


# MessageTemplateDataTypeDef definition

class MessageTemplateDataTypeDef(TypedDict):
    channelSubtype: ChannelSubtypeType,  # (2)
    content: MessageTemplateContentProviderOutputTypeDef,  # (3)
    createdTime: datetime,
    knowledgeBaseArn: str,
    knowledgeBaseId: str,
    lastModifiedBy: str,
    lastModifiedTime: datetime,
    messageTemplateArn: str,
    messageTemplateContentSha256: str,
    messageTemplateId: str,
    name: str,
    attributeTypes: NotRequired[List[MessageTemplateAttributeTypeType]],  # (1)
    defaultAttributes: NotRequired[MessageTemplateAttributesOutputTypeDef],  # (4)
    description: NotRequired[str],
    groupingConfiguration: NotRequired[GroupingConfigurationOutputTypeDef],  # (5)
    language: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: MessageTemplateAttributeTypeType](./literals.md#messagetemplateattributetypetype) 
2. See [:material-code-brackets: ChannelSubtypeType](./literals.md#channelsubtypetype) 
3. See [:material-code-braces: MessageTemplateContentProviderOutputTypeDef](./type_defs.md#messagetemplatecontentprovideroutputtypedef) 
4. See [:material-code-braces: MessageTemplateAttributesOutputTypeDef](./type_defs.md#messagetemplateattributesoutputtypedef) 
5. See [:material-code-braces: GroupingConfigurationOutputTypeDef](./type_defs.md#groupingconfigurationoutputtypedef) 
## RenderMessageTemplateResponseTypeDef

```python
# RenderMessageTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import RenderMessageTemplateResponseTypeDef


def get_value() -> RenderMessageTemplateResponseTypeDef:
    return {
        "attachments": ...,
    }


# RenderMessageTemplateResponseTypeDef definition

class RenderMessageTemplateResponseTypeDef(TypedDict):
    attachments: List[MessageTemplateAttachmentTypeDef],  # (1)
    attributesNotInterpolated: List[str],
    content: MessageTemplateContentProviderOutputTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MessageTemplateAttachmentTypeDef](./type_defs.md#messagetemplateattachmenttypedef) 
2. See [:material-code-braces: MessageTemplateContentProviderOutputTypeDef](./type_defs.md#messagetemplatecontentprovideroutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociationConfigurationDataOutputTypeDef

```python
# AssociationConfigurationDataOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AssociationConfigurationDataOutputTypeDef


def get_value() -> AssociationConfigurationDataOutputTypeDef:
    return {
        "knowledgeBaseAssociationConfigurationData": ...,
    }


# AssociationConfigurationDataOutputTypeDef definition

class AssociationConfigurationDataOutputTypeDef(TypedDict):
    knowledgeBaseAssociationConfigurationData: NotRequired[KnowledgeBaseAssociationConfigurationDataOutputTypeDef],  # (1)
```

1. See [:material-code-braces: KnowledgeBaseAssociationConfigurationDataOutputTypeDef](./type_defs.md#knowledgebaseassociationconfigurationdataoutputtypedef) 
## CreateSessionResponseTypeDef

```python
# CreateSessionResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateSessionResponseTypeDef


def get_value() -> CreateSessionResponseTypeDef:
    return {
        "session": ...,
    }


# CreateSessionResponseTypeDef definition

class CreateSessionResponseTypeDef(TypedDict):
    session: SessionDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SessionDataTypeDef](./type_defs.md#sessiondatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSessionResponseTypeDef

```python
# GetSessionResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetSessionResponseTypeDef


def get_value() -> GetSessionResponseTypeDef:
    return {
        "session": ...,
    }


# GetSessionResponseTypeDef definition

class GetSessionResponseTypeDef(TypedDict):
    session: SessionDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SessionDataTypeDef](./type_defs.md#sessiondatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSessionResponseTypeDef

```python
# UpdateSessionResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UpdateSessionResponseTypeDef


def get_value() -> UpdateSessionResponseTypeDef:
    return {
        "session": ...,
    }


# UpdateSessionResponseTypeDef definition

class UpdateSessionResponseTypeDef(TypedDict):
    session: SessionDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SessionDataTypeDef](./type_defs.md#sessiondatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociationConfigurationDataTypeDef

```python
# AssociationConfigurationDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AssociationConfigurationDataTypeDef


def get_value() -> AssociationConfigurationDataTypeDef:
    return {
        "knowledgeBaseAssociationConfigurationData": ...,
    }


# AssociationConfigurationDataTypeDef definition

class AssociationConfigurationDataTypeDef(TypedDict):
    knowledgeBaseAssociationConfigurationData: NotRequired[KnowledgeBaseAssociationConfigurationDataTypeDef],  # (1)
```

1. See [:material-code-braces: KnowledgeBaseAssociationConfigurationDataTypeDef](./type_defs.md#knowledgebaseassociationconfigurationdatatypedef) 
## CreateSessionRequestTypeDef

```python
# CreateSessionRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateSessionRequestTypeDef


def get_value() -> CreateSessionRequestTypeDef:
    return {
        "assistantId": ...,
    }


# CreateSessionRequestTypeDef definition

class CreateSessionRequestTypeDef(TypedDict):
    assistantId: str,
    name: str,
    aiAgentConfiguration: NotRequired[Mapping[AIAgentTypeType, AIAgentConfigurationDataTypeDef]],  # (1)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    tagFilter: NotRequired[TagFilterUnionTypeDef],  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: AIAgentTypeType](./literals.md#aiagenttypetype) [:material-code-braces: AIAgentConfigurationDataTypeDef](./type_defs.md#aiagentconfigurationdatatypedef) 
2. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) [:material-code-braces: TagFilterOutputTypeDef](./type_defs.md#tagfilteroutputtypedef) 
## UpdateSessionRequestTypeDef

```python
# UpdateSessionRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UpdateSessionRequestTypeDef


def get_value() -> UpdateSessionRequestTypeDef:
    return {
        "assistantId": ...,
    }


# UpdateSessionRequestTypeDef definition

class UpdateSessionRequestTypeDef(TypedDict):
    assistantId: str,
    sessionId: str,
    aiAgentConfiguration: NotRequired[Mapping[AIAgentTypeType, AIAgentConfigurationDataTypeDef]],  # (1)
    description: NotRequired[str],
    tagFilter: NotRequired[TagFilterUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: AIAgentTypeType](./literals.md#aiagenttypetype) [:material-code-braces: AIAgentConfigurationDataTypeDef](./type_defs.md#aiagentconfigurationdatatypedef) 
2. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) [:material-code-braces: TagFilterOutputTypeDef](./type_defs.md#tagfilteroutputtypedef) 
## SourceConfigurationOutputTypeDef

```python
# SourceConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SourceConfigurationOutputTypeDef


def get_value() -> SourceConfigurationOutputTypeDef:
    return {
        "appIntegrations": ...,
    }


# SourceConfigurationOutputTypeDef definition

class SourceConfigurationOutputTypeDef(TypedDict):
    appIntegrations: NotRequired[AppIntegrationsConfigurationOutputTypeDef],  # (1)
    managedSourceConfiguration: NotRequired[ManagedSourceConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: AppIntegrationsConfigurationOutputTypeDef](./type_defs.md#appintegrationsconfigurationoutputtypedef) 
2. See [:material-code-braces: ManagedSourceConfigurationOutputTypeDef](./type_defs.md#managedsourceconfigurationoutputtypedef) 
## SourceConfigurationTypeDef

```python
# SourceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SourceConfigurationTypeDef


def get_value() -> SourceConfigurationTypeDef:
    return {
        "appIntegrations": ...,
    }


# SourceConfigurationTypeDef definition

class SourceConfigurationTypeDef(TypedDict):
    appIntegrations: NotRequired[AppIntegrationsConfigurationTypeDef],  # (1)
    managedSourceConfiguration: NotRequired[ManagedSourceConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: AppIntegrationsConfigurationTypeDef](./type_defs.md#appintegrationsconfigurationtypedef) 
2. See [:material-code-braces: ManagedSourceConfigurationTypeDef](./type_defs.md#managedsourceconfigurationtypedef) 
## RenderMessageTemplateRequestTypeDef

```python
# RenderMessageTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import RenderMessageTemplateRequestTypeDef


def get_value() -> RenderMessageTemplateRequestTypeDef:
    return {
        "attributes": ...,
    }


# RenderMessageTemplateRequestTypeDef definition

class RenderMessageTemplateRequestTypeDef(TypedDict):
    attributes: MessageTemplateAttributesUnionTypeDef,  # (1)
    knowledgeBaseId: str,
    messageTemplateId: str,
```

1. See [:material-code-braces: MessageTemplateAttributesTypeDef](./type_defs.md#messagetemplateattributestypedef) [:material-code-braces: MessageTemplateAttributesOutputTypeDef](./type_defs.md#messagetemplateattributesoutputtypedef) 
## DataSummaryPaginatorTypeDef

```python
# DataSummaryPaginatorTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DataSummaryPaginatorTypeDef


def get_value() -> DataSummaryPaginatorTypeDef:
    return {
        "details": ...,
    }


# DataSummaryPaginatorTypeDef definition

class DataSummaryPaginatorTypeDef(TypedDict):
    details: DataDetailsPaginatorTypeDef,  # (1)
    reference: DataReferenceTypeDef,  # (2)
```

1. See [:material-code-braces: DataDetailsPaginatorTypeDef](./type_defs.md#datadetailspaginatortypedef) 
2. See [:material-code-braces: DataReferenceTypeDef](./type_defs.md#datareferencetypedef) 
## DataSummaryTypeDef

```python
# DataSummaryTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import DataSummaryTypeDef


def get_value() -> DataSummaryTypeDef:
    return {
        "details": ...,
    }


# DataSummaryTypeDef definition

class DataSummaryTypeDef(TypedDict):
    details: DataDetailsTypeDef,  # (1)
    reference: DataReferenceTypeDef,  # (2)
```

1. See [:material-code-braces: DataDetailsTypeDef](./type_defs.md#datadetailstypedef) 
2. See [:material-code-braces: DataReferenceTypeDef](./type_defs.md#datareferencetypedef) 
## CreateMessageTemplateVersionResponseTypeDef

```python
# CreateMessageTemplateVersionResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateMessageTemplateVersionResponseTypeDef


def get_value() -> CreateMessageTemplateVersionResponseTypeDef:
    return {
        "messageTemplate": ...,
    }


# CreateMessageTemplateVersionResponseTypeDef definition

class CreateMessageTemplateVersionResponseTypeDef(TypedDict):
    messageTemplate: ExtendedMessageTemplateDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExtendedMessageTemplateDataTypeDef](./type_defs.md#extendedmessagetemplatedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMessageTemplateResponseTypeDef

```python
# GetMessageTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetMessageTemplateResponseTypeDef


def get_value() -> GetMessageTemplateResponseTypeDef:
    return {
        "messageTemplate": ...,
    }


# GetMessageTemplateResponseTypeDef definition

class GetMessageTemplateResponseTypeDef(TypedDict):
    messageTemplate: ExtendedMessageTemplateDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExtendedMessageTemplateDataTypeDef](./type_defs.md#extendedmessagetemplatedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMessageTemplateResponseTypeDef

```python
# CreateMessageTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateMessageTemplateResponseTypeDef


def get_value() -> CreateMessageTemplateResponseTypeDef:
    return {
        "messageTemplate": ...,
    }


# CreateMessageTemplateResponseTypeDef definition

class CreateMessageTemplateResponseTypeDef(TypedDict):
    messageTemplate: MessageTemplateDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageTemplateDataTypeDef](./type_defs.md#messagetemplatedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMessageTemplateMetadataResponseTypeDef

```python
# UpdateMessageTemplateMetadataResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UpdateMessageTemplateMetadataResponseTypeDef


def get_value() -> UpdateMessageTemplateMetadataResponseTypeDef:
    return {
        "messageTemplate": ...,
    }


# UpdateMessageTemplateMetadataResponseTypeDef definition

class UpdateMessageTemplateMetadataResponseTypeDef(TypedDict):
    messageTemplate: MessageTemplateDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageTemplateDataTypeDef](./type_defs.md#messagetemplatedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMessageTemplateResponseTypeDef

```python
# UpdateMessageTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UpdateMessageTemplateResponseTypeDef


def get_value() -> UpdateMessageTemplateResponseTypeDef:
    return {
        "messageTemplate": ...,
    }


# UpdateMessageTemplateResponseTypeDef definition

class UpdateMessageTemplateResponseTypeDef(TypedDict):
    messageTemplate: MessageTemplateDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageTemplateDataTypeDef](./type_defs.md#messagetemplatedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMessageTemplateRequestTypeDef

```python
# CreateMessageTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateMessageTemplateRequestTypeDef


def get_value() -> CreateMessageTemplateRequestTypeDef:
    return {
        "channelSubtype": ...,
    }


# CreateMessageTemplateRequestTypeDef definition

class CreateMessageTemplateRequestTypeDef(TypedDict):
    channelSubtype: ChannelSubtypeType,  # (1)
    content: MessageTemplateContentProviderUnionTypeDef,  # (2)
    knowledgeBaseId: str,
    name: str,
    clientToken: NotRequired[str],
    defaultAttributes: NotRequired[MessageTemplateAttributesUnionTypeDef],  # (3)
    description: NotRequired[str],
    groupingConfiguration: NotRequired[GroupingConfigurationUnionTypeDef],  # (4)
    language: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ChannelSubtypeType](./literals.md#channelsubtypetype) 
2. See [:material-code-braces: MessageTemplateContentProviderTypeDef](./type_defs.md#messagetemplatecontentprovidertypedef) [:material-code-braces: MessageTemplateContentProviderOutputTypeDef](./type_defs.md#messagetemplatecontentprovideroutputtypedef) 
3. See [:material-code-braces: MessageTemplateAttributesTypeDef](./type_defs.md#messagetemplateattributestypedef) [:material-code-braces: MessageTemplateAttributesOutputTypeDef](./type_defs.md#messagetemplateattributesoutputtypedef) 
4. See [:material-code-braces: GroupingConfigurationTypeDef](./type_defs.md#groupingconfigurationtypedef) [:material-code-braces: GroupingConfigurationOutputTypeDef](./type_defs.md#groupingconfigurationoutputtypedef) 
## UpdateMessageTemplateRequestTypeDef

```python
# UpdateMessageTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UpdateMessageTemplateRequestTypeDef


def get_value() -> UpdateMessageTemplateRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# UpdateMessageTemplateRequestTypeDef definition

class UpdateMessageTemplateRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    messageTemplateId: str,
    content: NotRequired[MessageTemplateContentProviderUnionTypeDef],  # (1)
    defaultAttributes: NotRequired[MessageTemplateAttributesUnionTypeDef],  # (2)
    language: NotRequired[str],
```

1. See [:material-code-braces: MessageTemplateContentProviderTypeDef](./type_defs.md#messagetemplatecontentprovidertypedef) [:material-code-braces: MessageTemplateContentProviderOutputTypeDef](./type_defs.md#messagetemplatecontentprovideroutputtypedef) 
2. See [:material-code-braces: MessageTemplateAttributesTypeDef](./type_defs.md#messagetemplateattributestypedef) [:material-code-braces: MessageTemplateAttributesOutputTypeDef](./type_defs.md#messagetemplateattributesoutputtypedef) 
## AssociationConfigurationOutputTypeDef

```python
# AssociationConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AssociationConfigurationOutputTypeDef


def get_value() -> AssociationConfigurationOutputTypeDef:
    return {
        "associationConfigurationData": ...,
    }


# AssociationConfigurationOutputTypeDef definition

class AssociationConfigurationOutputTypeDef(TypedDict):
    associationConfigurationData: NotRequired[AssociationConfigurationDataOutputTypeDef],  # (1)
    associationId: NotRequired[str],
    associationType: NotRequired[AIAgentAssociationConfigurationTypeType],  # (2)
```

1. See [:material-code-braces: AssociationConfigurationDataOutputTypeDef](./type_defs.md#associationconfigurationdataoutputtypedef) 
2. See [:material-code-brackets: AIAgentAssociationConfigurationTypeType](./literals.md#aiagentassociationconfigurationtypetype) 
## AssociationConfigurationTypeDef

```python
# AssociationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AssociationConfigurationTypeDef


def get_value() -> AssociationConfigurationTypeDef:
    return {
        "associationConfigurationData": ...,
    }


# AssociationConfigurationTypeDef definition

class AssociationConfigurationTypeDef(TypedDict):
    associationConfigurationData: NotRequired[AssociationConfigurationDataTypeDef],  # (1)
    associationId: NotRequired[str],
    associationType: NotRequired[AIAgentAssociationConfigurationTypeType],  # (2)
```

1. See [:material-code-braces: AssociationConfigurationDataTypeDef](./type_defs.md#associationconfigurationdatatypedef) 
2. See [:material-code-brackets: AIAgentAssociationConfigurationTypeType](./literals.md#aiagentassociationconfigurationtypetype) 
## KnowledgeBaseDataTypeDef

```python
# KnowledgeBaseDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import KnowledgeBaseDataTypeDef


def get_value() -> KnowledgeBaseDataTypeDef:
    return {
        "description": ...,
    }


# KnowledgeBaseDataTypeDef definition

class KnowledgeBaseDataTypeDef(TypedDict):
    knowledgeBaseArn: str,
    knowledgeBaseId: str,
    knowledgeBaseType: KnowledgeBaseTypeType,  # (2)
    name: str,
    status: KnowledgeBaseStatusType,  # (6)
    description: NotRequired[str],
    ingestionFailureReasons: NotRequired[List[str]],
    ingestionStatus: NotRequired[SyncStatusType],  # (1)
    lastContentModificationTime: NotRequired[datetime],
    renderingConfiguration: NotRequired[RenderingConfigurationTypeDef],  # (3)
    serverSideEncryptionConfiguration: NotRequired[ServerSideEncryptionConfigurationTypeDef],  # (4)
    sourceConfiguration: NotRequired[SourceConfigurationOutputTypeDef],  # (5)
    tags: NotRequired[Dict[str, str]],
    vectorIngestionConfiguration: NotRequired[VectorIngestionConfigurationOutputTypeDef],  # (7)
```

1. See [:material-code-brackets: SyncStatusType](./literals.md#syncstatustype) 
2. See [:material-code-brackets: KnowledgeBaseTypeType](./literals.md#knowledgebasetypetype) 
3. See [:material-code-braces: RenderingConfigurationTypeDef](./type_defs.md#renderingconfigurationtypedef) 
4. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
5. See [:material-code-braces: SourceConfigurationOutputTypeDef](./type_defs.md#sourceconfigurationoutputtypedef) 
6. See [:material-code-brackets: KnowledgeBaseStatusType](./literals.md#knowledgebasestatustype) 
7. See [:material-code-braces: VectorIngestionConfigurationOutputTypeDef](./type_defs.md#vectoringestionconfigurationoutputtypedef) 
## KnowledgeBaseSummaryTypeDef

```python
# KnowledgeBaseSummaryTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import KnowledgeBaseSummaryTypeDef


def get_value() -> KnowledgeBaseSummaryTypeDef:
    return {
        "description": ...,
    }


# KnowledgeBaseSummaryTypeDef definition

class KnowledgeBaseSummaryTypeDef(TypedDict):
    knowledgeBaseArn: str,
    knowledgeBaseId: str,
    knowledgeBaseType: KnowledgeBaseTypeType,  # (1)
    name: str,
    status: KnowledgeBaseStatusType,  # (5)
    description: NotRequired[str],
    renderingConfiguration: NotRequired[RenderingConfigurationTypeDef],  # (2)
    serverSideEncryptionConfiguration: NotRequired[ServerSideEncryptionConfigurationTypeDef],  # (3)
    sourceConfiguration: NotRequired[SourceConfigurationOutputTypeDef],  # (4)
    tags: NotRequired[Dict[str, str]],
    vectorIngestionConfiguration: NotRequired[VectorIngestionConfigurationOutputTypeDef],  # (6)
```

1. See [:material-code-brackets: KnowledgeBaseTypeType](./literals.md#knowledgebasetypetype) 
2. See [:material-code-braces: RenderingConfigurationTypeDef](./type_defs.md#renderingconfigurationtypedef) 
3. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
4. See [:material-code-braces: SourceConfigurationOutputTypeDef](./type_defs.md#sourceconfigurationoutputtypedef) 
5. See [:material-code-brackets: KnowledgeBaseStatusType](./literals.md#knowledgebasestatustype) 
6. See [:material-code-braces: VectorIngestionConfigurationOutputTypeDef](./type_defs.md#vectoringestionconfigurationoutputtypedef) 
## ResultDataPaginatorTypeDef

```python
# ResultDataPaginatorTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ResultDataPaginatorTypeDef


def get_value() -> ResultDataPaginatorTypeDef:
    return {
        "data": ...,
    }


# ResultDataPaginatorTypeDef definition

class ResultDataPaginatorTypeDef(TypedDict):
    resultId: str,
    data: NotRequired[DataSummaryPaginatorTypeDef],  # (1)
    document: NotRequired[DocumentTypeDef],  # (2)
    relevanceScore: NotRequired[float],
    type: NotRequired[QueryResultTypeType],  # (3)
```

1. See [:material-code-braces: DataSummaryPaginatorTypeDef](./type_defs.md#datasummarypaginatortypedef) 
2. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
3. See [:material-code-brackets: QueryResultTypeType](./literals.md#queryresulttypetype) 
## RecommendationDataTypeDef

```python
# RecommendationDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import RecommendationDataTypeDef


def get_value() -> RecommendationDataTypeDef:
    return {
        "data": ...,
    }


# RecommendationDataTypeDef definition

class RecommendationDataTypeDef(TypedDict):
    recommendationId: str,
    data: NotRequired[DataSummaryTypeDef],  # (1)
    document: NotRequired[DocumentTypeDef],  # (2)
    relevanceLevel: NotRequired[RelevanceLevelType],  # (3)
    relevanceScore: NotRequired[float],
    type: NotRequired[RecommendationTypeType],  # (4)
```

1. See [:material-code-braces: DataSummaryTypeDef](./type_defs.md#datasummarytypedef) 
2. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
3. See [:material-code-brackets: RelevanceLevelType](./literals.md#relevanceleveltype) 
4. See [:material-code-brackets: RecommendationTypeType](./literals.md#recommendationtypetype) 
## ResultDataTypeDef

```python
# ResultDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ResultDataTypeDef


def get_value() -> ResultDataTypeDef:
    return {
        "data": ...,
    }


# ResultDataTypeDef definition

class ResultDataTypeDef(TypedDict):
    resultId: str,
    data: NotRequired[DataSummaryTypeDef],  # (1)
    document: NotRequired[DocumentTypeDef],  # (2)
    relevanceScore: NotRequired[float],
    type: NotRequired[QueryResultTypeType],  # (3)
```

1. See [:material-code-braces: DataSummaryTypeDef](./type_defs.md#datasummarytypedef) 
2. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
3. See [:material-code-brackets: QueryResultTypeType](./literals.md#queryresulttypetype) 
## AnswerRecommendationAIAgentConfigurationOutputTypeDef

```python
# AnswerRecommendationAIAgentConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AnswerRecommendationAIAgentConfigurationOutputTypeDef


def get_value() -> AnswerRecommendationAIAgentConfigurationOutputTypeDef:
    return {
        "answerGenerationAIGuardrailId": ...,
    }


# AnswerRecommendationAIAgentConfigurationOutputTypeDef definition

class AnswerRecommendationAIAgentConfigurationOutputTypeDef(TypedDict):
    answerGenerationAIGuardrailId: NotRequired[str],
    answerGenerationAIPromptId: NotRequired[str],
    associationConfigurations: NotRequired[List[AssociationConfigurationOutputTypeDef]],  # (1)
    intentLabelingGenerationAIPromptId: NotRequired[str],
    locale: NotRequired[str],
    queryReformulationAIPromptId: NotRequired[str],
```

1. See [:material-code-braces: AssociationConfigurationOutputTypeDef](./type_defs.md#associationconfigurationoutputtypedef) 
## ManualSearchAIAgentConfigurationOutputTypeDef

```python
# ManualSearchAIAgentConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ManualSearchAIAgentConfigurationOutputTypeDef


def get_value() -> ManualSearchAIAgentConfigurationOutputTypeDef:
    return {
        "answerGenerationAIGuardrailId": ...,
    }


# ManualSearchAIAgentConfigurationOutputTypeDef definition

class ManualSearchAIAgentConfigurationOutputTypeDef(TypedDict):
    answerGenerationAIGuardrailId: NotRequired[str],
    answerGenerationAIPromptId: NotRequired[str],
    associationConfigurations: NotRequired[List[AssociationConfigurationOutputTypeDef]],  # (1)
    locale: NotRequired[str],
```

1. See [:material-code-braces: AssociationConfigurationOutputTypeDef](./type_defs.md#associationconfigurationoutputtypedef) 
## SelfServiceAIAgentConfigurationOutputTypeDef

```python
# SelfServiceAIAgentConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SelfServiceAIAgentConfigurationOutputTypeDef


def get_value() -> SelfServiceAIAgentConfigurationOutputTypeDef:
    return {
        "associationConfigurations": ...,
    }


# SelfServiceAIAgentConfigurationOutputTypeDef definition

class SelfServiceAIAgentConfigurationOutputTypeDef(TypedDict):
    associationConfigurations: NotRequired[List[AssociationConfigurationOutputTypeDef]],  # (1)
    selfServiceAIGuardrailId: NotRequired[str],
    selfServiceAnswerGenerationAIPromptId: NotRequired[str],
    selfServicePreProcessingAIPromptId: NotRequired[str],
```

1. See [:material-code-braces: AssociationConfigurationOutputTypeDef](./type_defs.md#associationconfigurationoutputtypedef) 
## AnswerRecommendationAIAgentConfigurationTypeDef

```python
# AnswerRecommendationAIAgentConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AnswerRecommendationAIAgentConfigurationTypeDef


def get_value() -> AnswerRecommendationAIAgentConfigurationTypeDef:
    return {
        "answerGenerationAIGuardrailId": ...,
    }


# AnswerRecommendationAIAgentConfigurationTypeDef definition

class AnswerRecommendationAIAgentConfigurationTypeDef(TypedDict):
    answerGenerationAIGuardrailId: NotRequired[str],
    answerGenerationAIPromptId: NotRequired[str],
    associationConfigurations: NotRequired[Sequence[AssociationConfigurationTypeDef]],  # (1)
    intentLabelingGenerationAIPromptId: NotRequired[str],
    locale: NotRequired[str],
    queryReformulationAIPromptId: NotRequired[str],
```

1. See [:material-code-braces: AssociationConfigurationTypeDef](./type_defs.md#associationconfigurationtypedef) 
## ManualSearchAIAgentConfigurationTypeDef

```python
# ManualSearchAIAgentConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ManualSearchAIAgentConfigurationTypeDef


def get_value() -> ManualSearchAIAgentConfigurationTypeDef:
    return {
        "answerGenerationAIGuardrailId": ...,
    }


# ManualSearchAIAgentConfigurationTypeDef definition

class ManualSearchAIAgentConfigurationTypeDef(TypedDict):
    answerGenerationAIGuardrailId: NotRequired[str],
    answerGenerationAIPromptId: NotRequired[str],
    associationConfigurations: NotRequired[Sequence[AssociationConfigurationTypeDef]],  # (1)
    locale: NotRequired[str],
```

1. See [:material-code-braces: AssociationConfigurationTypeDef](./type_defs.md#associationconfigurationtypedef) 
## SelfServiceAIAgentConfigurationTypeDef

```python
# SelfServiceAIAgentConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import SelfServiceAIAgentConfigurationTypeDef


def get_value() -> SelfServiceAIAgentConfigurationTypeDef:
    return {
        "associationConfigurations": ...,
    }


# SelfServiceAIAgentConfigurationTypeDef definition

class SelfServiceAIAgentConfigurationTypeDef(TypedDict):
    associationConfigurations: NotRequired[Sequence[AssociationConfigurationTypeDef]],  # (1)
    selfServiceAIGuardrailId: NotRequired[str],
    selfServiceAnswerGenerationAIPromptId: NotRequired[str],
    selfServicePreProcessingAIPromptId: NotRequired[str],
```

1. See [:material-code-braces: AssociationConfigurationTypeDef](./type_defs.md#associationconfigurationtypedef) 
## CreateKnowledgeBaseResponseTypeDef

```python
# CreateKnowledgeBaseResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateKnowledgeBaseResponseTypeDef


def get_value() -> CreateKnowledgeBaseResponseTypeDef:
    return {
        "knowledgeBase": ...,
    }


# CreateKnowledgeBaseResponseTypeDef definition

class CreateKnowledgeBaseResponseTypeDef(TypedDict):
    knowledgeBase: KnowledgeBaseDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KnowledgeBaseDataTypeDef](./type_defs.md#knowledgebasedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetKnowledgeBaseResponseTypeDef

```python
# GetKnowledgeBaseResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetKnowledgeBaseResponseTypeDef


def get_value() -> GetKnowledgeBaseResponseTypeDef:
    return {
        "knowledgeBase": ...,
    }


# GetKnowledgeBaseResponseTypeDef definition

class GetKnowledgeBaseResponseTypeDef(TypedDict):
    knowledgeBase: KnowledgeBaseDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KnowledgeBaseDataTypeDef](./type_defs.md#knowledgebasedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateKnowledgeBaseTemplateUriResponseTypeDef

```python
# UpdateKnowledgeBaseTemplateUriResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UpdateKnowledgeBaseTemplateUriResponseTypeDef


def get_value() -> UpdateKnowledgeBaseTemplateUriResponseTypeDef:
    return {
        "knowledgeBase": ...,
    }


# UpdateKnowledgeBaseTemplateUriResponseTypeDef definition

class UpdateKnowledgeBaseTemplateUriResponseTypeDef(TypedDict):
    knowledgeBase: KnowledgeBaseDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KnowledgeBaseDataTypeDef](./type_defs.md#knowledgebasedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListKnowledgeBasesResponseTypeDef

```python
# ListKnowledgeBasesResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListKnowledgeBasesResponseTypeDef


def get_value() -> ListKnowledgeBasesResponseTypeDef:
    return {
        "knowledgeBaseSummaries": ...,
    }


# ListKnowledgeBasesResponseTypeDef definition

class ListKnowledgeBasesResponseTypeDef(TypedDict):
    knowledgeBaseSummaries: List[KnowledgeBaseSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: KnowledgeBaseSummaryTypeDef](./type_defs.md#knowledgebasesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateKnowledgeBaseRequestTypeDef

```python
# CreateKnowledgeBaseRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateKnowledgeBaseRequestTypeDef


def get_value() -> CreateKnowledgeBaseRequestTypeDef:
    return {
        "knowledgeBaseType": ...,
    }


# CreateKnowledgeBaseRequestTypeDef definition

class CreateKnowledgeBaseRequestTypeDef(TypedDict):
    knowledgeBaseType: KnowledgeBaseTypeType,  # (1)
    name: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    renderingConfiguration: NotRequired[RenderingConfigurationTypeDef],  # (2)
    serverSideEncryptionConfiguration: NotRequired[ServerSideEncryptionConfigurationTypeDef],  # (3)
    sourceConfiguration: NotRequired[SourceConfigurationUnionTypeDef],  # (4)
    tags: NotRequired[Mapping[str, str]],
    vectorIngestionConfiguration: NotRequired[VectorIngestionConfigurationUnionTypeDef],  # (5)
```

1. See [:material-code-brackets: KnowledgeBaseTypeType](./literals.md#knowledgebasetypetype) 
2. See [:material-code-braces: RenderingConfigurationTypeDef](./type_defs.md#renderingconfigurationtypedef) 
3. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
4. See [:material-code-braces: SourceConfigurationTypeDef](./type_defs.md#sourceconfigurationtypedef) [:material-code-braces: SourceConfigurationOutputTypeDef](./type_defs.md#sourceconfigurationoutputtypedef) 
5. See [:material-code-braces: VectorIngestionConfigurationTypeDef](./type_defs.md#vectoringestionconfigurationtypedef) [:material-code-braces: VectorIngestionConfigurationOutputTypeDef](./type_defs.md#vectoringestionconfigurationoutputtypedef) 
## QueryAssistantResponsePaginatorTypeDef

```python
# QueryAssistantResponsePaginatorTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import QueryAssistantResponsePaginatorTypeDef


def get_value() -> QueryAssistantResponsePaginatorTypeDef:
    return {
        "nextToken": ...,
    }


# QueryAssistantResponsePaginatorTypeDef definition

class QueryAssistantResponsePaginatorTypeDef(TypedDict):
    results: List[ResultDataPaginatorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResultDataPaginatorTypeDef](./type_defs.md#resultdatapaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRecommendationsResponseTypeDef

```python
# GetRecommendationsResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetRecommendationsResponseTypeDef


def get_value() -> GetRecommendationsResponseTypeDef:
    return {
        "recommendations": ...,
    }


# GetRecommendationsResponseTypeDef definition

class GetRecommendationsResponseTypeDef(TypedDict):
    recommendations: List[RecommendationDataTypeDef],  # (1)
    triggers: List[RecommendationTriggerTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RecommendationDataTypeDef](./type_defs.md#recommendationdatatypedef) 
2. See [:material-code-braces: RecommendationTriggerTypeDef](./type_defs.md#recommendationtriggertypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## QueryAssistantResponseTypeDef

```python
# QueryAssistantResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import QueryAssistantResponseTypeDef


def get_value() -> QueryAssistantResponseTypeDef:
    return {
        "nextToken": ...,
    }


# QueryAssistantResponseTypeDef definition

class QueryAssistantResponseTypeDef(TypedDict):
    results: List[ResultDataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResultDataTypeDef](./type_defs.md#resultdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AIAgentConfigurationOutputTypeDef

```python
# AIAgentConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIAgentConfigurationOutputTypeDef


def get_value() -> AIAgentConfigurationOutputTypeDef:
    return {
        "answerRecommendationAIAgentConfiguration": ...,
    }


# AIAgentConfigurationOutputTypeDef definition

class AIAgentConfigurationOutputTypeDef(TypedDict):
    answerRecommendationAIAgentConfiguration: NotRequired[AnswerRecommendationAIAgentConfigurationOutputTypeDef],  # (1)
    manualSearchAIAgentConfiguration: NotRequired[ManualSearchAIAgentConfigurationOutputTypeDef],  # (2)
    selfServiceAIAgentConfiguration: NotRequired[SelfServiceAIAgentConfigurationOutputTypeDef],  # (3)
```

1. See [:material-code-braces: AnswerRecommendationAIAgentConfigurationOutputTypeDef](./type_defs.md#answerrecommendationaiagentconfigurationoutputtypedef) 
2. See [:material-code-braces: ManualSearchAIAgentConfigurationOutputTypeDef](./type_defs.md#manualsearchaiagentconfigurationoutputtypedef) 
3. See [:material-code-braces: SelfServiceAIAgentConfigurationOutputTypeDef](./type_defs.md#selfserviceaiagentconfigurationoutputtypedef) 
## AIAgentConfigurationTypeDef

```python
# AIAgentConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIAgentConfigurationTypeDef


def get_value() -> AIAgentConfigurationTypeDef:
    return {
        "answerRecommendationAIAgentConfiguration": ...,
    }


# AIAgentConfigurationTypeDef definition

class AIAgentConfigurationTypeDef(TypedDict):
    answerRecommendationAIAgentConfiguration: NotRequired[AnswerRecommendationAIAgentConfigurationTypeDef],  # (1)
    manualSearchAIAgentConfiguration: NotRequired[ManualSearchAIAgentConfigurationTypeDef],  # (2)
    selfServiceAIAgentConfiguration: NotRequired[SelfServiceAIAgentConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: AnswerRecommendationAIAgentConfigurationTypeDef](./type_defs.md#answerrecommendationaiagentconfigurationtypedef) 
2. See [:material-code-braces: ManualSearchAIAgentConfigurationTypeDef](./type_defs.md#manualsearchaiagentconfigurationtypedef) 
3. See [:material-code-braces: SelfServiceAIAgentConfigurationTypeDef](./type_defs.md#selfserviceaiagentconfigurationtypedef) 
## AIAgentDataTypeDef

```python
# AIAgentDataTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIAgentDataTypeDef


def get_value() -> AIAgentDataTypeDef:
    return {
        "aiAgentArn": ...,
    }


# AIAgentDataTypeDef definition

class AIAgentDataTypeDef(TypedDict):
    aiAgentArn: str,
    aiAgentId: str,
    assistantArn: str,
    assistantId: str,
    configuration: AIAgentConfigurationOutputTypeDef,  # (1)
    name: str,
    type: AIAgentTypeType,  # (4)
    visibilityStatus: VisibilityStatusType,  # (5)
    description: NotRequired[str],
    modifiedTime: NotRequired[datetime],
    origin: NotRequired[OriginType],  # (2)
    status: NotRequired[StatusType],  # (3)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: AIAgentConfigurationOutputTypeDef](./type_defs.md#aiagentconfigurationoutputtypedef) 
2. See [:material-code-brackets: OriginType](./literals.md#origintype) 
3. See [:material-code-brackets: StatusType](./literals.md#statustype) 
4. See [:material-code-brackets: AIAgentTypeType](./literals.md#aiagenttypetype) 
5. See [:material-code-brackets: VisibilityStatusType](./literals.md#visibilitystatustype) 
## AIAgentSummaryTypeDef

```python
# AIAgentSummaryTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIAgentSummaryTypeDef


def get_value() -> AIAgentSummaryTypeDef:
    return {
        "aiAgentArn": ...,
    }


# AIAgentSummaryTypeDef definition

class AIAgentSummaryTypeDef(TypedDict):
    aiAgentArn: str,
    aiAgentId: str,
    assistantArn: str,
    assistantId: str,
    name: str,
    type: AIAgentTypeType,  # (4)
    visibilityStatus: VisibilityStatusType,  # (5)
    configuration: NotRequired[AIAgentConfigurationOutputTypeDef],  # (1)
    description: NotRequired[str],
    modifiedTime: NotRequired[datetime],
    origin: NotRequired[OriginType],  # (2)
    status: NotRequired[StatusType],  # (3)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: AIAgentConfigurationOutputTypeDef](./type_defs.md#aiagentconfigurationoutputtypedef) 
2. See [:material-code-brackets: OriginType](./literals.md#origintype) 
3. See [:material-code-brackets: StatusType](./literals.md#statustype) 
4. See [:material-code-brackets: AIAgentTypeType](./literals.md#aiagenttypetype) 
5. See [:material-code-brackets: VisibilityStatusType](./literals.md#visibilitystatustype) 
## CreateAIAgentResponseTypeDef

```python
# CreateAIAgentResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateAIAgentResponseTypeDef


def get_value() -> CreateAIAgentResponseTypeDef:
    return {
        "aiAgent": ...,
    }


# CreateAIAgentResponseTypeDef definition

class CreateAIAgentResponseTypeDef(TypedDict):
    aiAgent: AIAgentDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AIAgentDataTypeDef](./type_defs.md#aiagentdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAIAgentVersionResponseTypeDef

```python
# CreateAIAgentVersionResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateAIAgentVersionResponseTypeDef


def get_value() -> CreateAIAgentVersionResponseTypeDef:
    return {
        "aiAgent": ...,
    }


# CreateAIAgentVersionResponseTypeDef definition

class CreateAIAgentVersionResponseTypeDef(TypedDict):
    aiAgent: AIAgentDataTypeDef,  # (1)
    versionNumber: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AIAgentDataTypeDef](./type_defs.md#aiagentdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAIAgentResponseTypeDef

```python
# GetAIAgentResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import GetAIAgentResponseTypeDef


def get_value() -> GetAIAgentResponseTypeDef:
    return {
        "aiAgent": ...,
    }


# GetAIAgentResponseTypeDef definition

class GetAIAgentResponseTypeDef(TypedDict):
    aiAgent: AIAgentDataTypeDef,  # (1)
    versionNumber: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AIAgentDataTypeDef](./type_defs.md#aiagentdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAIAgentResponseTypeDef

```python
# UpdateAIAgentResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UpdateAIAgentResponseTypeDef


def get_value() -> UpdateAIAgentResponseTypeDef:
    return {
        "aiAgent": ...,
    }


# UpdateAIAgentResponseTypeDef definition

class UpdateAIAgentResponseTypeDef(TypedDict):
    aiAgent: AIAgentDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AIAgentDataTypeDef](./type_defs.md#aiagentdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AIAgentVersionSummaryTypeDef

```python
# AIAgentVersionSummaryTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import AIAgentVersionSummaryTypeDef


def get_value() -> AIAgentVersionSummaryTypeDef:
    return {
        "aiAgentSummary": ...,
    }


# AIAgentVersionSummaryTypeDef definition

class AIAgentVersionSummaryTypeDef(TypedDict):
    aiAgentSummary: NotRequired[AIAgentSummaryTypeDef],  # (1)
    versionNumber: NotRequired[int],
```

1. See [:material-code-braces: AIAgentSummaryTypeDef](./type_defs.md#aiagentsummarytypedef) 
## ListAIAgentsResponseTypeDef

```python
# ListAIAgentsResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAIAgentsResponseTypeDef


def get_value() -> ListAIAgentsResponseTypeDef:
    return {
        "aiAgentSummaries": ...,
    }


# ListAIAgentsResponseTypeDef definition

class ListAIAgentsResponseTypeDef(TypedDict):
    aiAgentSummaries: List[AIAgentSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AIAgentSummaryTypeDef](./type_defs.md#aiagentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAIAgentRequestTypeDef

```python
# CreateAIAgentRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import CreateAIAgentRequestTypeDef


def get_value() -> CreateAIAgentRequestTypeDef:
    return {
        "assistantId": ...,
    }


# CreateAIAgentRequestTypeDef definition

class CreateAIAgentRequestTypeDef(TypedDict):
    assistantId: str,
    configuration: AIAgentConfigurationUnionTypeDef,  # (1)
    name: str,
    type: AIAgentTypeType,  # (2)
    visibilityStatus: VisibilityStatusType,  # (3)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AIAgentConfigurationTypeDef](./type_defs.md#aiagentconfigurationtypedef) [:material-code-braces: AIAgentConfigurationOutputTypeDef](./type_defs.md#aiagentconfigurationoutputtypedef) 
2. See [:material-code-brackets: AIAgentTypeType](./literals.md#aiagenttypetype) 
3. See [:material-code-brackets: VisibilityStatusType](./literals.md#visibilitystatustype) 
## UpdateAIAgentRequestTypeDef

```python
# UpdateAIAgentRequestTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import UpdateAIAgentRequestTypeDef


def get_value() -> UpdateAIAgentRequestTypeDef:
    return {
        "aiAgentId": ...,
    }


# UpdateAIAgentRequestTypeDef definition

class UpdateAIAgentRequestTypeDef(TypedDict):
    aiAgentId: str,
    assistantId: str,
    visibilityStatus: VisibilityStatusType,  # (1)
    clientToken: NotRequired[str],
    configuration: NotRequired[AIAgentConfigurationUnionTypeDef],  # (2)
    description: NotRequired[str],
```

1. See [:material-code-brackets: VisibilityStatusType](./literals.md#visibilitystatustype) 
2. See [:material-code-braces: AIAgentConfigurationTypeDef](./type_defs.md#aiagentconfigurationtypedef) [:material-code-braces: AIAgentConfigurationOutputTypeDef](./type_defs.md#aiagentconfigurationoutputtypedef) 
## ListAIAgentVersionsResponseTypeDef

```python
# ListAIAgentVersionsResponseTypeDef TypedDict usage example

from types_aiobotocore_qconnect.type_defs import ListAIAgentVersionsResponseTypeDef


def get_value() -> ListAIAgentVersionsResponseTypeDef:
    return {
        "aiAgentVersionSummaries": ...,
    }


# ListAIAgentVersionsResponseTypeDef definition

class ListAIAgentVersionsResponseTypeDef(TypedDict):
    aiAgentVersionSummaries: List[AIAgentVersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AIAgentVersionSummaryTypeDef](./type_defs.md#aiagentversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
