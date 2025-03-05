# Type definitions

> [Index](../README.md) > [AgentsforBedrock](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AgentsforBedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#agentsforbedrock)
    type annotations stubs module [types-aiobotocore-bedrock-agent](https://pypi.org/project/types-aiobotocore-bedrock-agent/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_bedrock_agent.type_defs import BlobTypeDef


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


## PromptModelInferenceConfigurationUnionTypeDef

```python
# PromptModelInferenceConfigurationUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptModelInferenceConfigurationUnionTypeDef


def get_value() -> PromptModelInferenceConfigurationUnionTypeDef:
    return ...


# PromptModelInferenceConfigurationUnionTypeDef definition

PromptModelInferenceConfigurationUnionTypeDef = Union[
    PromptModelInferenceConfigurationTypeDef,  # (1)
    PromptModelInferenceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PromptModelInferenceConfigurationTypeDef](./type_defs.md#promptmodelinferenceconfigurationtypedef)
2. See [:material-code-braces: PromptModelInferenceConfigurationOutputTypeDef](./type_defs.md#promptmodelinferenceconfigurationoutputtypedef)

## ToolInputSchemaUnionTypeDef

```python
# ToolInputSchemaUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent.type_defs import ToolInputSchemaUnionTypeDef


def get_value() -> ToolInputSchemaUnionTypeDef:
    return ...


# ToolInputSchemaUnionTypeDef definition

ToolInputSchemaUnionTypeDef = Union[
    ToolInputSchemaTypeDef,  # (1)
    ToolInputSchemaOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ToolInputSchemaTypeDef](./type_defs.md#toolinputschematypedef)
2. See [:material-code-braces: ToolInputSchemaOutputTypeDef](./type_defs.md#toolinputschemaoutputtypedef)

## TextPromptTemplateConfigurationUnionTypeDef

```python
# TextPromptTemplateConfigurationUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent.type_defs import TextPromptTemplateConfigurationUnionTypeDef


def get_value() -> TextPromptTemplateConfigurationUnionTypeDef:
    return ...


# TextPromptTemplateConfigurationUnionTypeDef definition

TextPromptTemplateConfigurationUnionTypeDef = Union[
    TextPromptTemplateConfigurationTypeDef,  # (1)
    TextPromptTemplateConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TextPromptTemplateConfigurationTypeDef](./type_defs.md#textprompttemplateconfigurationtypedef)
2. See [:material-code-braces: TextPromptTemplateConfigurationOutputTypeDef](./type_defs.md#textprompttemplateconfigurationoutputtypedef)

## MemoryConfigurationUnionTypeDef

```python
# MemoryConfigurationUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent.type_defs import MemoryConfigurationUnionTypeDef


def get_value() -> MemoryConfigurationUnionTypeDef:
    return ...


# MemoryConfigurationUnionTypeDef definition

MemoryConfigurationUnionTypeDef = Union[
    MemoryConfigurationTypeDef,  # (1)
    MemoryConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MemoryConfigurationTypeDef](./type_defs.md#memoryconfigurationtypedef)
2. See [:material-code-braces: MemoryConfigurationOutputTypeDef](./type_defs.md#memoryconfigurationoutputtypedef)

## ToolChoiceUnionTypeDef

```python
# ToolChoiceUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent.type_defs import ToolChoiceUnionTypeDef


def get_value() -> ToolChoiceUnionTypeDef:
    return ...


# ToolChoiceUnionTypeDef definition

ToolChoiceUnionTypeDef = Union[
    ToolChoiceTypeDef,  # (1)
    ToolChoiceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ToolChoiceTypeDef](./type_defs.md#toolchoicetypedef)
2. See [:material-code-braces: ToolChoiceOutputTypeDef](./type_defs.md#toolchoiceoutputtypedef)

## MessageUnionTypeDef

```python
# MessageUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent.type_defs import MessageUnionTypeDef


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

## FunctionSchemaUnionTypeDef

```python
# FunctionSchemaUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent.type_defs import FunctionSchemaUnionTypeDef


def get_value() -> FunctionSchemaUnionTypeDef:
    return ...


# FunctionSchemaUnionTypeDef definition

FunctionSchemaUnionTypeDef = Union[
    FunctionSchemaTypeDef,  # (1)
    FunctionSchemaOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FunctionSchemaTypeDef](./type_defs.md#functionschematypedef)
2. See [:material-code-braces: FunctionSchemaOutputTypeDef](./type_defs.md#functionschemaoutputtypedef)

## PromptOverrideConfigurationUnionTypeDef

```python
# PromptOverrideConfigurationUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptOverrideConfigurationUnionTypeDef


def get_value() -> PromptOverrideConfigurationUnionTypeDef:
    return ...


# PromptOverrideConfigurationUnionTypeDef definition

PromptOverrideConfigurationUnionTypeDef = Union[
    PromptOverrideConfigurationTypeDef,  # (1)
    PromptOverrideConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PromptOverrideConfigurationTypeDef](./type_defs.md#promptoverrideconfigurationtypedef)
2. See [:material-code-braces: PromptOverrideConfigurationOutputTypeDef](./type_defs.md#promptoverrideconfigurationoutputtypedef)

## PromptInferenceConfigurationUnionTypeDef

```python
# PromptInferenceConfigurationUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptInferenceConfigurationUnionTypeDef


def get_value() -> PromptInferenceConfigurationUnionTypeDef:
    return ...


# PromptInferenceConfigurationUnionTypeDef definition

PromptInferenceConfigurationUnionTypeDef = Union[
    PromptInferenceConfigurationTypeDef,  # (1)
    PromptInferenceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PromptInferenceConfigurationTypeDef](./type_defs.md#promptinferenceconfigurationtypedef)
2. See [:material-code-braces: PromptInferenceConfigurationOutputTypeDef](./type_defs.md#promptinferenceconfigurationoutputtypedef)

## ToolSpecificationUnionTypeDef

```python
# ToolSpecificationUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent.type_defs import ToolSpecificationUnionTypeDef


def get_value() -> ToolSpecificationUnionTypeDef:
    return ...


# ToolSpecificationUnionTypeDef definition

ToolSpecificationUnionTypeDef = Union[
    ToolSpecificationTypeDef,  # (1)
    ToolSpecificationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ToolSpecificationTypeDef](./type_defs.md#toolspecificationtypedef)
2. See [:material-code-braces: ToolSpecificationOutputTypeDef](./type_defs.md#toolspecificationoutputtypedef)

## ToolUnionTypeDef

```python
# ToolUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent.type_defs import ToolUnionTypeDef


def get_value() -> ToolUnionTypeDef:
    return ...


# ToolUnionTypeDef definition

ToolUnionTypeDef = Union[
    ToolTypeDef,  # (1)
    ToolOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ToolTypeDef](./type_defs.md#tooltypedef)
2. See [:material-code-braces: ToolOutputTypeDef](./type_defs.md#tooloutputtypedef)

## VectorIngestionConfigurationUnionTypeDef

```python
# VectorIngestionConfigurationUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent.type_defs import VectorIngestionConfigurationUnionTypeDef


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

## DataSourceConfigurationUnionTypeDef

```python
# DataSourceConfigurationUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent.type_defs import DataSourceConfigurationUnionTypeDef


def get_value() -> DataSourceConfigurationUnionTypeDef:
    return ...


# DataSourceConfigurationUnionTypeDef definition

DataSourceConfigurationUnionTypeDef = Union[
    DataSourceConfigurationTypeDef,  # (1)
    DataSourceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef)
2. See [:material-code-braces: DataSourceConfigurationOutputTypeDef](./type_defs.md#datasourceconfigurationoutputtypedef)

## KnowledgeBaseConfigurationUnionTypeDef

```python
# KnowledgeBaseConfigurationUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent.type_defs import KnowledgeBaseConfigurationUnionTypeDef


def get_value() -> KnowledgeBaseConfigurationUnionTypeDef:
    return ...


# KnowledgeBaseConfigurationUnionTypeDef definition

KnowledgeBaseConfigurationUnionTypeDef = Union[
    KnowledgeBaseConfigurationTypeDef,  # (1)
    KnowledgeBaseConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: KnowledgeBaseConfigurationTypeDef](./type_defs.md#knowledgebaseconfigurationtypedef)
2. See [:material-code-braces: KnowledgeBaseConfigurationOutputTypeDef](./type_defs.md#knowledgebaseconfigurationoutputtypedef)

## ToolConfigurationUnionTypeDef

```python
# ToolConfigurationUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent.type_defs import ToolConfigurationUnionTypeDef


def get_value() -> ToolConfigurationUnionTypeDef:
    return ...


# ToolConfigurationUnionTypeDef definition

ToolConfigurationUnionTypeDef = Union[
    ToolConfigurationTypeDef,  # (1)
    ToolConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ToolConfigurationTypeDef](./type_defs.md#toolconfigurationtypedef)
2. See [:material-code-braces: ToolConfigurationOutputTypeDef](./type_defs.md#toolconfigurationoutputtypedef)

## ChatPromptTemplateConfigurationUnionTypeDef

```python
# ChatPromptTemplateConfigurationUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent.type_defs import ChatPromptTemplateConfigurationUnionTypeDef


def get_value() -> ChatPromptTemplateConfigurationUnionTypeDef:
    return ...


# ChatPromptTemplateConfigurationUnionTypeDef definition

ChatPromptTemplateConfigurationUnionTypeDef = Union[
    ChatPromptTemplateConfigurationTypeDef,  # (1)
    ChatPromptTemplateConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ChatPromptTemplateConfigurationTypeDef](./type_defs.md#chatprompttemplateconfigurationtypedef)
2. See [:material-code-braces: ChatPromptTemplateConfigurationOutputTypeDef](./type_defs.md#chatprompttemplateconfigurationoutputtypedef)

## PromptTemplateConfigurationUnionTypeDef

```python
# PromptTemplateConfigurationUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptTemplateConfigurationUnionTypeDef


def get_value() -> PromptTemplateConfigurationUnionTypeDef:
    return ...


# PromptTemplateConfigurationUnionTypeDef definition

PromptTemplateConfigurationUnionTypeDef = Union[
    PromptTemplateConfigurationTypeDef,  # (1)
    PromptTemplateConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PromptTemplateConfigurationTypeDef](./type_defs.md#prompttemplateconfigurationtypedef)
2. See [:material-code-braces: PromptTemplateConfigurationOutputTypeDef](./type_defs.md#prompttemplateconfigurationoutputtypedef)

## PromptVariantUnionTypeDef

```python
# PromptVariantUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptVariantUnionTypeDef


def get_value() -> PromptVariantUnionTypeDef:
    return ...


# PromptVariantUnionTypeDef definition

PromptVariantUnionTypeDef = Union[
    PromptVariantTypeDef,  # (1)
    PromptVariantOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PromptVariantTypeDef](./type_defs.md#promptvarianttypedef)
2. See [:material-code-braces: PromptVariantOutputTypeDef](./type_defs.md#promptvariantoutputtypedef)

## FlowDefinitionUnionTypeDef

```python
# FlowDefinitionUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent.type_defs import FlowDefinitionUnionTypeDef


def get_value() -> FlowDefinitionUnionTypeDef:
    return ...


# FlowDefinitionUnionTypeDef definition

FlowDefinitionUnionTypeDef = Union[
    FlowDefinitionTypeDef,  # (1)
    FlowDefinitionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FlowDefinitionTypeDef](./type_defs.md#flowdefinitiontypedef)
2. See [:material-code-braces: FlowDefinitionOutputTypeDef](./type_defs.md#flowdefinitionoutputtypedef)



## S3IdentifierTypeDef

```python
# S3IdentifierTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import S3IdentifierTypeDef


def get_value() -> S3IdentifierTypeDef:
    return {
        "s3BucketName": ...,
    }


# S3IdentifierTypeDef definition

class S3IdentifierTypeDef(TypedDict):
    s3BucketName: NotRequired[str],
    s3ObjectKey: NotRequired[str],
```


## ActionGroupExecutorTypeDef

```python
# ActionGroupExecutorTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ActionGroupExecutorTypeDef


def get_value() -> ActionGroupExecutorTypeDef:
    return {
        "customControl": ...,
    }


# ActionGroupExecutorTypeDef definition

class ActionGroupExecutorTypeDef(TypedDict):
    customControl: NotRequired[CustomControlMethodType],  # (1)
    lambda: NotRequired[str],
```

1. See [:material-code-brackets: CustomControlMethodType](./literals.md#customcontrolmethodtype)

## ActionGroupSummaryTypeDef

```python
# ActionGroupSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ActionGroupSummaryTypeDef


def get_value() -> ActionGroupSummaryTypeDef:
    return {
        "actionGroupId": ...,
    }


# ActionGroupSummaryTypeDef definition

class ActionGroupSummaryTypeDef(TypedDict):
    actionGroupId: str,
    actionGroupName: str,
    actionGroupState: ActionGroupStateType,  # (1)
    updatedAt: datetime.datetime,
    description: NotRequired[str],
```

1. See [:material-code-brackets: ActionGroupStateType](./literals.md#actiongroupstatetype)

## AgentAliasRoutingConfigurationListItemTypeDef

```python
# AgentAliasRoutingConfigurationListItemTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import AgentAliasRoutingConfigurationListItemTypeDef


def get_value() -> AgentAliasRoutingConfigurationListItemTypeDef:
    return {
        "agentVersion": ...,
    }


# AgentAliasRoutingConfigurationListItemTypeDef definition

class AgentAliasRoutingConfigurationListItemTypeDef(TypedDict):
    agentVersion: NotRequired[str],
    provisionedThroughput: NotRequired[str],
```


## AgentDescriptorTypeDef

```python
# AgentDescriptorTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import AgentDescriptorTypeDef


def get_value() -> AgentDescriptorTypeDef:
    return {
        "aliasArn": ...,
    }


# AgentDescriptorTypeDef definition

class AgentDescriptorTypeDef(TypedDict):
    aliasArn: NotRequired[str],
```


## AgentFlowNodeConfigurationTypeDef

```python
# AgentFlowNodeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import AgentFlowNodeConfigurationTypeDef


def get_value() -> AgentFlowNodeConfigurationTypeDef:
    return {
        "agentAliasArn": ...,
    }


# AgentFlowNodeConfigurationTypeDef definition

class AgentFlowNodeConfigurationTypeDef(TypedDict):
    agentAliasArn: str,
```


## AgentKnowledgeBaseSummaryTypeDef

```python
# AgentKnowledgeBaseSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import AgentKnowledgeBaseSummaryTypeDef


def get_value() -> AgentKnowledgeBaseSummaryTypeDef:
    return {
        "description": ...,
    }


# AgentKnowledgeBaseSummaryTypeDef definition

class AgentKnowledgeBaseSummaryTypeDef(TypedDict):
    knowledgeBaseId: str,
    knowledgeBaseState: KnowledgeBaseStateType,  # (1)
    updatedAt: datetime.datetime,
    description: NotRequired[str],
```

1. See [:material-code-brackets: KnowledgeBaseStateType](./literals.md#knowledgebasestatetype)

## AgentKnowledgeBaseTypeDef

```python
# AgentKnowledgeBaseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import AgentKnowledgeBaseTypeDef


def get_value() -> AgentKnowledgeBaseTypeDef:
    return {
        "agentId": ...,
    }


# AgentKnowledgeBaseTypeDef definition

class AgentKnowledgeBaseTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    createdAt: datetime.datetime,
    description: str,
    knowledgeBaseId: str,
    knowledgeBaseState: KnowledgeBaseStateType,  # (1)
    updatedAt: datetime.datetime,
```

1. See [:material-code-brackets: KnowledgeBaseStateType](./literals.md#knowledgebasestatetype)

## GuardrailConfigurationTypeDef

```python
# GuardrailConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GuardrailConfigurationTypeDef


def get_value() -> GuardrailConfigurationTypeDef:
    return {
        "guardrailIdentifier": ...,
    }


# GuardrailConfigurationTypeDef definition

class GuardrailConfigurationTypeDef(TypedDict):
    guardrailIdentifier: NotRequired[str],
    guardrailVersion: NotRequired[str],
```


## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ResponseMetadataTypeDef


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


## AssociateAgentKnowledgeBaseRequestTypeDef

```python
# AssociateAgentKnowledgeBaseRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import AssociateAgentKnowledgeBaseRequestTypeDef


def get_value() -> AssociateAgentKnowledgeBaseRequestTypeDef:
    return {
        "agentId": ...,
    }


# AssociateAgentKnowledgeBaseRequestTypeDef definition

class AssociateAgentKnowledgeBaseRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    description: str,
    knowledgeBaseId: str,
    knowledgeBaseState: NotRequired[KnowledgeBaseStateType],  # (1)
```

1. See [:material-code-brackets: KnowledgeBaseStateType](./literals.md#knowledgebasestatetype)

## BedrockDataAutomationConfigurationTypeDef

```python
# BedrockDataAutomationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import BedrockDataAutomationConfigurationTypeDef


def get_value() -> BedrockDataAutomationConfigurationTypeDef:
    return {
        "parsingModality": ...,
    }


# BedrockDataAutomationConfigurationTypeDef definition

class BedrockDataAutomationConfigurationTypeDef(TypedDict):
    parsingModality: NotRequired[ParsingModalityType],  # (1)
```

1. See [:material-code-brackets: ParsingModalityType](./literals.md#parsingmodalitytype)

## BedrockEmbeddingModelConfigurationTypeDef

```python
# BedrockEmbeddingModelConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import BedrockEmbeddingModelConfigurationTypeDef


def get_value() -> BedrockEmbeddingModelConfigurationTypeDef:
    return {
        "dimensions": ...,
    }


# BedrockEmbeddingModelConfigurationTypeDef definition

class BedrockEmbeddingModelConfigurationTypeDef(TypedDict):
    dimensions: NotRequired[int],
    embeddingDataType: NotRequired[EmbeddingDataTypeType],  # (1)
```

1. See [:material-code-brackets: EmbeddingDataTypeType](./literals.md#embeddingdatatypetype)

## ParsingPromptTypeDef

```python
# ParsingPromptTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ParsingPromptTypeDef


def get_value() -> ParsingPromptTypeDef:
    return {
        "parsingPromptText": ...,
    }


# ParsingPromptTypeDef definition

class ParsingPromptTypeDef(TypedDict):
    parsingPromptText: str,
```


## CachePointBlockTypeDef

```python
# CachePointBlockTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CachePointBlockTypeDef


def get_value() -> CachePointBlockTypeDef:
    return {
        "type": ...,
    }


# CachePointBlockTypeDef definition

class CachePointBlockTypeDef(TypedDict):
    type: CachePointTypeType,  # (1)
```

1. See [:material-code-brackets: CachePointTypeType](./literals.md#cachepointtypetype)

## PromptInputVariableTypeDef

```python
# PromptInputVariableTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptInputVariableTypeDef


def get_value() -> PromptInputVariableTypeDef:
    return {
        "name": ...,
    }


# PromptInputVariableTypeDef definition

class PromptInputVariableTypeDef(TypedDict):
    name: NotRequired[str],
```


## FixedSizeChunkingConfigurationTypeDef

```python
# FixedSizeChunkingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FixedSizeChunkingConfigurationTypeDef


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

from types_aiobotocore_bedrock_agent.type_defs import SemanticChunkingConfigurationTypeDef


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


## FlowConditionTypeDef

```python
# FlowConditionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FlowConditionTypeDef


def get_value() -> FlowConditionTypeDef:
    return {
        "expression": ...,
    }


# FlowConditionTypeDef definition

class FlowConditionTypeDef(TypedDict):
    name: str,
    expression: NotRequired[str],
```


## ConfluenceSourceConfigurationTypeDef

```python
# ConfluenceSourceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ConfluenceSourceConfigurationTypeDef


def get_value() -> ConfluenceSourceConfigurationTypeDef:
    return {
        "authType": ...,
    }


# ConfluenceSourceConfigurationTypeDef definition

class ConfluenceSourceConfigurationTypeDef(TypedDict):
    authType: ConfluenceAuthTypeType,  # (1)
    credentialsSecretArn: str,
    hostType: ConfluenceHostTypeType,  # (2)
    hostUrl: str,
```

1. See [:material-code-brackets: ConfluenceAuthTypeType](./literals.md#confluenceauthtypetype)
2. See [:material-code-brackets: ConfluenceHostTypeType](./literals.md#confluencehosttypetype)

## ServerSideEncryptionConfigurationTypeDef

```python
# ServerSideEncryptionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ServerSideEncryptionConfigurationTypeDef


def get_value() -> ServerSideEncryptionConfigurationTypeDef:
    return {
        "kmsKeyArn": ...,
    }


# ServerSideEncryptionConfigurationTypeDef definition

class ServerSideEncryptionConfigurationTypeDef(TypedDict):
    kmsKeyArn: NotRequired[str],
```


## FlowAliasRoutingConfigurationListItemTypeDef

```python
# FlowAliasRoutingConfigurationListItemTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FlowAliasRoutingConfigurationListItemTypeDef


def get_value() -> FlowAliasRoutingConfigurationListItemTypeDef:
    return {
        "flowVersion": ...,
    }


# FlowAliasRoutingConfigurationListItemTypeDef definition

class FlowAliasRoutingConfigurationListItemTypeDef(TypedDict):
    flowVersion: NotRequired[str],
```


## CreateFlowVersionRequestTypeDef

```python
# CreateFlowVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CreateFlowVersionRequestTypeDef


def get_value() -> CreateFlowVersionRequestTypeDef:
    return {
        "flowIdentifier": ...,
    }


# CreateFlowVersionRequestTypeDef definition

class CreateFlowVersionRequestTypeDef(TypedDict):
    flowIdentifier: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
```


## CreatePromptVersionRequestTypeDef

```python
# CreatePromptVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CreatePromptVersionRequestTypeDef


def get_value() -> CreatePromptVersionRequestTypeDef:
    return {
        "promptIdentifier": ...,
    }


# CreatePromptVersionRequestTypeDef definition

class CreatePromptVersionRequestTypeDef(TypedDict):
    promptIdentifier: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```


## CuratedQueryTypeDef

```python
# CuratedQueryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CuratedQueryTypeDef


def get_value() -> CuratedQueryTypeDef:
    return {
        "naturalLanguage": ...,
    }


# CuratedQueryTypeDef definition

class CuratedQueryTypeDef(TypedDict):
    naturalLanguage: str,
    sql: str,
```


## CustomDocumentIdentifierTypeDef

```python
# CustomDocumentIdentifierTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CustomDocumentIdentifierTypeDef


def get_value() -> CustomDocumentIdentifierTypeDef:
    return {
        "id": ...,
    }


# CustomDocumentIdentifierTypeDef definition

class CustomDocumentIdentifierTypeDef(TypedDict):
    id: str,
```


## CustomS3LocationTypeDef

```python
# CustomS3LocationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CustomS3LocationTypeDef


def get_value() -> CustomS3LocationTypeDef:
    return {
        "bucketOwnerAccountId": ...,
    }


# CustomS3LocationTypeDef definition

class CustomS3LocationTypeDef(TypedDict):
    uri: str,
    bucketOwnerAccountId: NotRequired[str],
```


## OrchestrationExecutorTypeDef

```python
# OrchestrationExecutorTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import OrchestrationExecutorTypeDef


def get_value() -> OrchestrationExecutorTypeDef:
    return {
        "lambda": ...,
    }


# OrchestrationExecutorTypeDef definition

class OrchestrationExecutorTypeDef(TypedDict):
    lambda: NotRequired[str],
```


## CyclicConnectionFlowValidationDetailsTypeDef

```python
# CyclicConnectionFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CyclicConnectionFlowValidationDetailsTypeDef


def get_value() -> CyclicConnectionFlowValidationDetailsTypeDef:
    return {
        "connection": ...,
    }


# CyclicConnectionFlowValidationDetailsTypeDef definition

class CyclicConnectionFlowValidationDetailsTypeDef(TypedDict):
    connection: str,
```


## S3DataSourceConfigurationOutputTypeDef

```python
# S3DataSourceConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import S3DataSourceConfigurationOutputTypeDef


def get_value() -> S3DataSourceConfigurationOutputTypeDef:
    return {
        "bucketArn": ...,
    }


# S3DataSourceConfigurationOutputTypeDef definition

class S3DataSourceConfigurationOutputTypeDef(TypedDict):
    bucketArn: str,
    bucketOwnerAccountId: NotRequired[str],
    inclusionPrefixes: NotRequired[List[str]],
```


## S3DataSourceConfigurationTypeDef

```python
# S3DataSourceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import S3DataSourceConfigurationTypeDef


def get_value() -> S3DataSourceConfigurationTypeDef:
    return {
        "bucketArn": ...,
    }


# S3DataSourceConfigurationTypeDef definition

class S3DataSourceConfigurationTypeDef(TypedDict):
    bucketArn: str,
    bucketOwnerAccountId: NotRequired[str],
    inclusionPrefixes: NotRequired[Sequence[str]],
```


## DataSourceSummaryTypeDef

```python
# DataSourceSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DataSourceSummaryTypeDef


def get_value() -> DataSourceSummaryTypeDef:
    return {
        "dataSourceId": ...,
    }


# DataSourceSummaryTypeDef definition

class DataSourceSummaryTypeDef(TypedDict):
    dataSourceId: str,
    knowledgeBaseId: str,
    name: str,
    status: DataSourceStatusType,  # (1)
    updatedAt: datetime.datetime,
    description: NotRequired[str],
```

1. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype)

## DeleteAgentActionGroupRequestTypeDef

```python
# DeleteAgentActionGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DeleteAgentActionGroupRequestTypeDef


def get_value() -> DeleteAgentActionGroupRequestTypeDef:
    return {
        "actionGroupId": ...,
    }


# DeleteAgentActionGroupRequestTypeDef definition

class DeleteAgentActionGroupRequestTypeDef(TypedDict):
    actionGroupId: str,
    agentId: str,
    agentVersion: str,
    skipResourceInUseCheck: NotRequired[bool],
```


## DeleteAgentAliasRequestTypeDef

```python
# DeleteAgentAliasRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DeleteAgentAliasRequestTypeDef


def get_value() -> DeleteAgentAliasRequestTypeDef:
    return {
        "agentAliasId": ...,
    }


# DeleteAgentAliasRequestTypeDef definition

class DeleteAgentAliasRequestTypeDef(TypedDict):
    agentAliasId: str,
    agentId: str,
```


## DeleteAgentRequestTypeDef

```python
# DeleteAgentRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DeleteAgentRequestTypeDef


def get_value() -> DeleteAgentRequestTypeDef:
    return {
        "agentId": ...,
    }


# DeleteAgentRequestTypeDef definition

class DeleteAgentRequestTypeDef(TypedDict):
    agentId: str,
    skipResourceInUseCheck: NotRequired[bool],
```


## DeleteAgentVersionRequestTypeDef

```python
# DeleteAgentVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DeleteAgentVersionRequestTypeDef


def get_value() -> DeleteAgentVersionRequestTypeDef:
    return {
        "agentId": ...,
    }


# DeleteAgentVersionRequestTypeDef definition

class DeleteAgentVersionRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    skipResourceInUseCheck: NotRequired[bool],
```


## DeleteDataSourceRequestTypeDef

```python
# DeleteDataSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DeleteDataSourceRequestTypeDef


def get_value() -> DeleteDataSourceRequestTypeDef:
    return {
        "dataSourceId": ...,
    }


# DeleteDataSourceRequestTypeDef definition

class DeleteDataSourceRequestTypeDef(TypedDict):
    dataSourceId: str,
    knowledgeBaseId: str,
```


## DeleteFlowAliasRequestTypeDef

```python
# DeleteFlowAliasRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DeleteFlowAliasRequestTypeDef


def get_value() -> DeleteFlowAliasRequestTypeDef:
    return {
        "aliasIdentifier": ...,
    }


# DeleteFlowAliasRequestTypeDef definition

class DeleteFlowAliasRequestTypeDef(TypedDict):
    aliasIdentifier: str,
    flowIdentifier: str,
```


## DeleteFlowRequestTypeDef

```python
# DeleteFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DeleteFlowRequestTypeDef


def get_value() -> DeleteFlowRequestTypeDef:
    return {
        "flowIdentifier": ...,
    }


# DeleteFlowRequestTypeDef definition

class DeleteFlowRequestTypeDef(TypedDict):
    flowIdentifier: str,
    skipResourceInUseCheck: NotRequired[bool],
```


## DeleteFlowVersionRequestTypeDef

```python
# DeleteFlowVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DeleteFlowVersionRequestTypeDef


def get_value() -> DeleteFlowVersionRequestTypeDef:
    return {
        "flowIdentifier": ...,
    }


# DeleteFlowVersionRequestTypeDef definition

class DeleteFlowVersionRequestTypeDef(TypedDict):
    flowIdentifier: str,
    flowVersion: str,
    skipResourceInUseCheck: NotRequired[bool],
```


## DeleteKnowledgeBaseRequestTypeDef

```python
# DeleteKnowledgeBaseRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DeleteKnowledgeBaseRequestTypeDef


def get_value() -> DeleteKnowledgeBaseRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# DeleteKnowledgeBaseRequestTypeDef definition

class DeleteKnowledgeBaseRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
```


## DeletePromptRequestTypeDef

```python
# DeletePromptRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DeletePromptRequestTypeDef


def get_value() -> DeletePromptRequestTypeDef:
    return {
        "promptIdentifier": ...,
    }


# DeletePromptRequestTypeDef definition

class DeletePromptRequestTypeDef(TypedDict):
    promptIdentifier: str,
    promptVersion: NotRequired[str],
```


## DisassociateAgentCollaboratorRequestTypeDef

```python
# DisassociateAgentCollaboratorRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DisassociateAgentCollaboratorRequestTypeDef


def get_value() -> DisassociateAgentCollaboratorRequestTypeDef:
    return {
        "agentId": ...,
    }


# DisassociateAgentCollaboratorRequestTypeDef definition

class DisassociateAgentCollaboratorRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    collaboratorId: str,
```


## DisassociateAgentKnowledgeBaseRequestTypeDef

```python
# DisassociateAgentKnowledgeBaseRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DisassociateAgentKnowledgeBaseRequestTypeDef


def get_value() -> DisassociateAgentKnowledgeBaseRequestTypeDef:
    return {
        "agentId": ...,
    }


# DisassociateAgentKnowledgeBaseRequestTypeDef definition

class DisassociateAgentKnowledgeBaseRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    knowledgeBaseId: str,
```


## S3LocationTypeDef

```python
# S3LocationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import S3LocationTypeDef


def get_value() -> S3LocationTypeDef:
    return {
        "uri": ...,
    }


# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    uri: str,
```


## DuplicateConditionExpressionFlowValidationDetailsTypeDef

```python
# DuplicateConditionExpressionFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DuplicateConditionExpressionFlowValidationDetailsTypeDef


def get_value() -> DuplicateConditionExpressionFlowValidationDetailsTypeDef:
    return {
        "expression": ...,
    }


# DuplicateConditionExpressionFlowValidationDetailsTypeDef definition

class DuplicateConditionExpressionFlowValidationDetailsTypeDef(TypedDict):
    expression: str,
    node: str,
```


## DuplicateConnectionsFlowValidationDetailsTypeDef

```python
# DuplicateConnectionsFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DuplicateConnectionsFlowValidationDetailsTypeDef


def get_value() -> DuplicateConnectionsFlowValidationDetailsTypeDef:
    return {
        "source": ...,
    }


# DuplicateConnectionsFlowValidationDetailsTypeDef definition

class DuplicateConnectionsFlowValidationDetailsTypeDef(TypedDict):
    source: str,
    target: str,
```


## FlowConditionalConnectionConfigurationTypeDef

```python
# FlowConditionalConnectionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FlowConditionalConnectionConfigurationTypeDef


def get_value() -> FlowConditionalConnectionConfigurationTypeDef:
    return {
        "condition": ...,
    }


# FlowConditionalConnectionConfigurationTypeDef definition

class FlowConditionalConnectionConfigurationTypeDef(TypedDict):
    condition: str,
```


## FlowDataConnectionConfigurationTypeDef

```python
# FlowDataConnectionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FlowDataConnectionConfigurationTypeDef


def get_value() -> FlowDataConnectionConfigurationTypeDef:
    return {
        "sourceOutput": ...,
    }


# FlowDataConnectionConfigurationTypeDef definition

class FlowDataConnectionConfigurationTypeDef(TypedDict):
    sourceOutput: str,
    targetInput: str,
```


## LambdaFunctionFlowNodeConfigurationTypeDef

```python
# LambdaFunctionFlowNodeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import LambdaFunctionFlowNodeConfigurationTypeDef


def get_value() -> LambdaFunctionFlowNodeConfigurationTypeDef:
    return {
        "lambdaArn": ...,
    }


# LambdaFunctionFlowNodeConfigurationTypeDef definition

class LambdaFunctionFlowNodeConfigurationTypeDef(TypedDict):
    lambdaArn: str,
```


## LexFlowNodeConfigurationTypeDef

```python
# LexFlowNodeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import LexFlowNodeConfigurationTypeDef


def get_value() -> LexFlowNodeConfigurationTypeDef:
    return {
        "botAliasArn": ...,
    }


# LexFlowNodeConfigurationTypeDef definition

class LexFlowNodeConfigurationTypeDef(TypedDict):
    botAliasArn: str,
    localeId: str,
```


## FlowNodeInputTypeDef

```python
# FlowNodeInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FlowNodeInputTypeDef


def get_value() -> FlowNodeInputTypeDef:
    return {
        "expression": ...,
    }


# FlowNodeInputTypeDef definition

class FlowNodeInputTypeDef(TypedDict):
    expression: str,
    name: str,
    type: FlowNodeIODataTypeType,  # (1)
```

1. See [:material-code-brackets: FlowNodeIODataTypeType](./literals.md#flownodeiodatatypetype)

## FlowNodeOutputTypeDef

```python
# FlowNodeOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FlowNodeOutputTypeDef


def get_value() -> FlowNodeOutputTypeDef:
    return {
        "name": ...,
    }


# FlowNodeOutputTypeDef definition

class FlowNodeOutputTypeDef(TypedDict):
    name: str,
    type: FlowNodeIODataTypeType,  # (1)
```

1. See [:material-code-brackets: FlowNodeIODataTypeType](./literals.md#flownodeiodatatypetype)

## FlowSummaryTypeDef

```python
# FlowSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FlowSummaryTypeDef


def get_value() -> FlowSummaryTypeDef:
    return {
        "arn": ...,
    }


# FlowSummaryTypeDef definition

class FlowSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime.datetime,
    id: str,
    name: str,
    status: FlowStatusType,  # (1)
    updatedAt: datetime.datetime,
    version: str,
    description: NotRequired[str],
```

1. See [:material-code-brackets: FlowStatusType](./literals.md#flowstatustype)

## IncompatibleConnectionDataTypeFlowValidationDetailsTypeDef

```python
# IncompatibleConnectionDataTypeFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import IncompatibleConnectionDataTypeFlowValidationDetailsTypeDef


def get_value() -> IncompatibleConnectionDataTypeFlowValidationDetailsTypeDef:
    return {
        "connection": ...,
    }


# IncompatibleConnectionDataTypeFlowValidationDetailsTypeDef definition

class IncompatibleConnectionDataTypeFlowValidationDetailsTypeDef(TypedDict):
    connection: str,
```


## MalformedConditionExpressionFlowValidationDetailsTypeDef

```python
# MalformedConditionExpressionFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import MalformedConditionExpressionFlowValidationDetailsTypeDef


def get_value() -> MalformedConditionExpressionFlowValidationDetailsTypeDef:
    return {
        "cause": ...,
    }


# MalformedConditionExpressionFlowValidationDetailsTypeDef definition

class MalformedConditionExpressionFlowValidationDetailsTypeDef(TypedDict):
    cause: str,
    condition: str,
    node: str,
```


## MalformedNodeInputExpressionFlowValidationDetailsTypeDef

```python
# MalformedNodeInputExpressionFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import MalformedNodeInputExpressionFlowValidationDetailsTypeDef


def get_value() -> MalformedNodeInputExpressionFlowValidationDetailsTypeDef:
    return {
        "cause": ...,
    }


# MalformedNodeInputExpressionFlowValidationDetailsTypeDef definition

class MalformedNodeInputExpressionFlowValidationDetailsTypeDef(TypedDict):
    cause: str,
    input: str,
    node: str,
```


## MismatchedNodeInputTypeFlowValidationDetailsTypeDef

```python
# MismatchedNodeInputTypeFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import MismatchedNodeInputTypeFlowValidationDetailsTypeDef


def get_value() -> MismatchedNodeInputTypeFlowValidationDetailsTypeDef:
    return {
        "expectedType": ...,
    }


# MismatchedNodeInputTypeFlowValidationDetailsTypeDef definition

class MismatchedNodeInputTypeFlowValidationDetailsTypeDef(TypedDict):
    expectedType: FlowNodeIODataTypeType,  # (1)
    input: str,
    node: str,
```

1. See [:material-code-brackets: FlowNodeIODataTypeType](./literals.md#flownodeiodatatypetype)

## MismatchedNodeOutputTypeFlowValidationDetailsTypeDef

```python
# MismatchedNodeOutputTypeFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import MismatchedNodeOutputTypeFlowValidationDetailsTypeDef


def get_value() -> MismatchedNodeOutputTypeFlowValidationDetailsTypeDef:
    return {
        "expectedType": ...,
    }


# MismatchedNodeOutputTypeFlowValidationDetailsTypeDef definition

class MismatchedNodeOutputTypeFlowValidationDetailsTypeDef(TypedDict):
    expectedType: FlowNodeIODataTypeType,  # (1)
    node: str,
    output: str,
```

1. See [:material-code-brackets: FlowNodeIODataTypeType](./literals.md#flownodeiodatatypetype)

## MissingConnectionConfigurationFlowValidationDetailsTypeDef

```python
# MissingConnectionConfigurationFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import MissingConnectionConfigurationFlowValidationDetailsTypeDef


def get_value() -> MissingConnectionConfigurationFlowValidationDetailsTypeDef:
    return {
        "connection": ...,
    }


# MissingConnectionConfigurationFlowValidationDetailsTypeDef definition

class MissingConnectionConfigurationFlowValidationDetailsTypeDef(TypedDict):
    connection: str,
```


## MissingDefaultConditionFlowValidationDetailsTypeDef

```python
# MissingDefaultConditionFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import MissingDefaultConditionFlowValidationDetailsTypeDef


def get_value() -> MissingDefaultConditionFlowValidationDetailsTypeDef:
    return {
        "node": ...,
    }


# MissingDefaultConditionFlowValidationDetailsTypeDef definition

class MissingDefaultConditionFlowValidationDetailsTypeDef(TypedDict):
    node: str,
```


## MissingNodeConfigurationFlowValidationDetailsTypeDef

```python
# MissingNodeConfigurationFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import MissingNodeConfigurationFlowValidationDetailsTypeDef


def get_value() -> MissingNodeConfigurationFlowValidationDetailsTypeDef:
    return {
        "node": ...,
    }


# MissingNodeConfigurationFlowValidationDetailsTypeDef definition

class MissingNodeConfigurationFlowValidationDetailsTypeDef(TypedDict):
    node: str,
```


## MissingNodeInputFlowValidationDetailsTypeDef

```python
# MissingNodeInputFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import MissingNodeInputFlowValidationDetailsTypeDef


def get_value() -> MissingNodeInputFlowValidationDetailsTypeDef:
    return {
        "input": ...,
    }


# MissingNodeInputFlowValidationDetailsTypeDef definition

class MissingNodeInputFlowValidationDetailsTypeDef(TypedDict):
    input: str,
    node: str,
```


## MissingNodeOutputFlowValidationDetailsTypeDef

```python
# MissingNodeOutputFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import MissingNodeOutputFlowValidationDetailsTypeDef


def get_value() -> MissingNodeOutputFlowValidationDetailsTypeDef:
    return {
        "node": ...,
    }


# MissingNodeOutputFlowValidationDetailsTypeDef definition

class MissingNodeOutputFlowValidationDetailsTypeDef(TypedDict):
    node: str,
    output: str,
```


## MultipleNodeInputConnectionsFlowValidationDetailsTypeDef

```python
# MultipleNodeInputConnectionsFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import MultipleNodeInputConnectionsFlowValidationDetailsTypeDef


def get_value() -> MultipleNodeInputConnectionsFlowValidationDetailsTypeDef:
    return {
        "input": ...,
    }


# MultipleNodeInputConnectionsFlowValidationDetailsTypeDef definition

class MultipleNodeInputConnectionsFlowValidationDetailsTypeDef(TypedDict):
    input: str,
    node: str,
```


## UnfulfilledNodeInputFlowValidationDetailsTypeDef

```python
# UnfulfilledNodeInputFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UnfulfilledNodeInputFlowValidationDetailsTypeDef


def get_value() -> UnfulfilledNodeInputFlowValidationDetailsTypeDef:
    return {
        "input": ...,
    }


# UnfulfilledNodeInputFlowValidationDetailsTypeDef definition

class UnfulfilledNodeInputFlowValidationDetailsTypeDef(TypedDict):
    input: str,
    node: str,
```


## UnknownConnectionConditionFlowValidationDetailsTypeDef

```python
# UnknownConnectionConditionFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UnknownConnectionConditionFlowValidationDetailsTypeDef


def get_value() -> UnknownConnectionConditionFlowValidationDetailsTypeDef:
    return {
        "connection": ...,
    }


# UnknownConnectionConditionFlowValidationDetailsTypeDef definition

class UnknownConnectionConditionFlowValidationDetailsTypeDef(TypedDict):
    connection: str,
```


## UnknownConnectionSourceFlowValidationDetailsTypeDef

```python
# UnknownConnectionSourceFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UnknownConnectionSourceFlowValidationDetailsTypeDef


def get_value() -> UnknownConnectionSourceFlowValidationDetailsTypeDef:
    return {
        "connection": ...,
    }


# UnknownConnectionSourceFlowValidationDetailsTypeDef definition

class UnknownConnectionSourceFlowValidationDetailsTypeDef(TypedDict):
    connection: str,
```


## UnknownConnectionSourceOutputFlowValidationDetailsTypeDef

```python
# UnknownConnectionSourceOutputFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UnknownConnectionSourceOutputFlowValidationDetailsTypeDef


def get_value() -> UnknownConnectionSourceOutputFlowValidationDetailsTypeDef:
    return {
        "connection": ...,
    }


# UnknownConnectionSourceOutputFlowValidationDetailsTypeDef definition

class UnknownConnectionSourceOutputFlowValidationDetailsTypeDef(TypedDict):
    connection: str,
```


## UnknownConnectionTargetFlowValidationDetailsTypeDef

```python
# UnknownConnectionTargetFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UnknownConnectionTargetFlowValidationDetailsTypeDef


def get_value() -> UnknownConnectionTargetFlowValidationDetailsTypeDef:
    return {
        "connection": ...,
    }


# UnknownConnectionTargetFlowValidationDetailsTypeDef definition

class UnknownConnectionTargetFlowValidationDetailsTypeDef(TypedDict):
    connection: str,
```


## UnknownConnectionTargetInputFlowValidationDetailsTypeDef

```python
# UnknownConnectionTargetInputFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UnknownConnectionTargetInputFlowValidationDetailsTypeDef


def get_value() -> UnknownConnectionTargetInputFlowValidationDetailsTypeDef:
    return {
        "connection": ...,
    }


# UnknownConnectionTargetInputFlowValidationDetailsTypeDef definition

class UnknownConnectionTargetInputFlowValidationDetailsTypeDef(TypedDict):
    connection: str,
```


## UnknownNodeInputFlowValidationDetailsTypeDef

```python
# UnknownNodeInputFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UnknownNodeInputFlowValidationDetailsTypeDef


def get_value() -> UnknownNodeInputFlowValidationDetailsTypeDef:
    return {
        "input": ...,
    }


# UnknownNodeInputFlowValidationDetailsTypeDef definition

class UnknownNodeInputFlowValidationDetailsTypeDef(TypedDict):
    input: str,
    node: str,
```


## UnknownNodeOutputFlowValidationDetailsTypeDef

```python
# UnknownNodeOutputFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UnknownNodeOutputFlowValidationDetailsTypeDef


def get_value() -> UnknownNodeOutputFlowValidationDetailsTypeDef:
    return {
        "node": ...,
    }


# UnknownNodeOutputFlowValidationDetailsTypeDef definition

class UnknownNodeOutputFlowValidationDetailsTypeDef(TypedDict):
    node: str,
    output: str,
```


## UnreachableNodeFlowValidationDetailsTypeDef

```python
# UnreachableNodeFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UnreachableNodeFlowValidationDetailsTypeDef


def get_value() -> UnreachableNodeFlowValidationDetailsTypeDef:
    return {
        "node": ...,
    }


# UnreachableNodeFlowValidationDetailsTypeDef definition

class UnreachableNodeFlowValidationDetailsTypeDef(TypedDict):
    node: str,
```


## UnsatisfiedConnectionConditionsFlowValidationDetailsTypeDef

```python
# UnsatisfiedConnectionConditionsFlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UnsatisfiedConnectionConditionsFlowValidationDetailsTypeDef


def get_value() -> UnsatisfiedConnectionConditionsFlowValidationDetailsTypeDef:
    return {
        "connection": ...,
    }


# UnsatisfiedConnectionConditionsFlowValidationDetailsTypeDef definition

class UnsatisfiedConnectionConditionsFlowValidationDetailsTypeDef(TypedDict):
    connection: str,
```


## FlowVersionSummaryTypeDef

```python
# FlowVersionSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FlowVersionSummaryTypeDef


def get_value() -> FlowVersionSummaryTypeDef:
    return {
        "arn": ...,
    }


# FlowVersionSummaryTypeDef definition

class FlowVersionSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime.datetime,
    id: str,
    status: FlowStatusType,  # (1)
    version: str,
```

1. See [:material-code-brackets: FlowStatusType](./literals.md#flowstatustype)

## ParameterDetailTypeDef

```python
# ParameterDetailTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ParameterDetailTypeDef


def get_value() -> ParameterDetailTypeDef:
    return {
        "description": ...,
    }


# ParameterDetailTypeDef definition

class ParameterDetailTypeDef(TypedDict):
    type: TypeType,  # (1)
    description: NotRequired[str],
    required: NotRequired[bool],
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype)

## GetAgentActionGroupRequestTypeDef

```python
# GetAgentActionGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetAgentActionGroupRequestTypeDef


def get_value() -> GetAgentActionGroupRequestTypeDef:
    return {
        "actionGroupId": ...,
    }


# GetAgentActionGroupRequestTypeDef definition

class GetAgentActionGroupRequestTypeDef(TypedDict):
    actionGroupId: str,
    agentId: str,
    agentVersion: str,
```


## GetAgentAliasRequestTypeDef

```python
# GetAgentAliasRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetAgentAliasRequestTypeDef


def get_value() -> GetAgentAliasRequestTypeDef:
    return {
        "agentAliasId": ...,
    }


# GetAgentAliasRequestTypeDef definition

class GetAgentAliasRequestTypeDef(TypedDict):
    agentAliasId: str,
    agentId: str,
```


## GetAgentCollaboratorRequestTypeDef

```python
# GetAgentCollaboratorRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetAgentCollaboratorRequestTypeDef


def get_value() -> GetAgentCollaboratorRequestTypeDef:
    return {
        "agentId": ...,
    }


# GetAgentCollaboratorRequestTypeDef definition

class GetAgentCollaboratorRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    collaboratorId: str,
```


## GetAgentKnowledgeBaseRequestTypeDef

```python
# GetAgentKnowledgeBaseRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetAgentKnowledgeBaseRequestTypeDef


def get_value() -> GetAgentKnowledgeBaseRequestTypeDef:
    return {
        "agentId": ...,
    }


# GetAgentKnowledgeBaseRequestTypeDef definition

class GetAgentKnowledgeBaseRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    knowledgeBaseId: str,
```


## GetAgentRequestTypeDef

```python
# GetAgentRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetAgentRequestTypeDef


def get_value() -> GetAgentRequestTypeDef:
    return {
        "agentId": ...,
    }


# GetAgentRequestTypeDef definition

class GetAgentRequestTypeDef(TypedDict):
    agentId: str,
```


## GetAgentVersionRequestTypeDef

```python
# GetAgentVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetAgentVersionRequestTypeDef


def get_value() -> GetAgentVersionRequestTypeDef:
    return {
        "agentId": ...,
    }


# GetAgentVersionRequestTypeDef definition

class GetAgentVersionRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
```


## GetDataSourceRequestTypeDef

```python
# GetDataSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetDataSourceRequestTypeDef


def get_value() -> GetDataSourceRequestTypeDef:
    return {
        "dataSourceId": ...,
    }


# GetDataSourceRequestTypeDef definition

class GetDataSourceRequestTypeDef(TypedDict):
    dataSourceId: str,
    knowledgeBaseId: str,
```


## GetFlowAliasRequestTypeDef

```python
# GetFlowAliasRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetFlowAliasRequestTypeDef


def get_value() -> GetFlowAliasRequestTypeDef:
    return {
        "aliasIdentifier": ...,
    }


# GetFlowAliasRequestTypeDef definition

class GetFlowAliasRequestTypeDef(TypedDict):
    aliasIdentifier: str,
    flowIdentifier: str,
```


## GetFlowRequestTypeDef

```python
# GetFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetFlowRequestTypeDef


def get_value() -> GetFlowRequestTypeDef:
    return {
        "flowIdentifier": ...,
    }


# GetFlowRequestTypeDef definition

class GetFlowRequestTypeDef(TypedDict):
    flowIdentifier: str,
```


## GetFlowVersionRequestTypeDef

```python
# GetFlowVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetFlowVersionRequestTypeDef


def get_value() -> GetFlowVersionRequestTypeDef:
    return {
        "flowIdentifier": ...,
    }


# GetFlowVersionRequestTypeDef definition

class GetFlowVersionRequestTypeDef(TypedDict):
    flowIdentifier: str,
    flowVersion: str,
```


## GetIngestionJobRequestTypeDef

```python
# GetIngestionJobRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetIngestionJobRequestTypeDef


def get_value() -> GetIngestionJobRequestTypeDef:
    return {
        "dataSourceId": ...,
    }


# GetIngestionJobRequestTypeDef definition

class GetIngestionJobRequestTypeDef(TypedDict):
    dataSourceId: str,
    ingestionJobId: str,
    knowledgeBaseId: str,
```


## GetKnowledgeBaseRequestTypeDef

```python
# GetKnowledgeBaseRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetKnowledgeBaseRequestTypeDef


def get_value() -> GetKnowledgeBaseRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# GetKnowledgeBaseRequestTypeDef definition

class GetKnowledgeBaseRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
```


## GetPromptRequestTypeDef

```python
# GetPromptRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetPromptRequestTypeDef


def get_value() -> GetPromptRequestTypeDef:
    return {
        "promptIdentifier": ...,
    }


# GetPromptRequestTypeDef definition

class GetPromptRequestTypeDef(TypedDict):
    promptIdentifier: str,
    promptVersion: NotRequired[str],
```


## HierarchicalChunkingLevelConfigurationTypeDef

```python
# HierarchicalChunkingLevelConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import HierarchicalChunkingLevelConfigurationTypeDef


def get_value() -> HierarchicalChunkingLevelConfigurationTypeDef:
    return {
        "maxTokens": ...,
    }


# HierarchicalChunkingLevelConfigurationTypeDef definition

class HierarchicalChunkingLevelConfigurationTypeDef(TypedDict):
    maxTokens: int,
```


## InferenceConfigurationOutputTypeDef

```python
# InferenceConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import InferenceConfigurationOutputTypeDef


def get_value() -> InferenceConfigurationOutputTypeDef:
    return {
        "maximumLength": ...,
    }


# InferenceConfigurationOutputTypeDef definition

class InferenceConfigurationOutputTypeDef(TypedDict):
    maximumLength: NotRequired[int],
    stopSequences: NotRequired[List[str]],
    temperature: NotRequired[float],
    topK: NotRequired[int],
    topP: NotRequired[float],
```


## InferenceConfigurationTypeDef

```python
# InferenceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import InferenceConfigurationTypeDef


def get_value() -> InferenceConfigurationTypeDef:
    return {
        "maximumLength": ...,
    }


# InferenceConfigurationTypeDef definition

class InferenceConfigurationTypeDef(TypedDict):
    maximumLength: NotRequired[int],
    stopSequences: NotRequired[Sequence[str]],
    temperature: NotRequired[float],
    topK: NotRequired[int],
    topP: NotRequired[float],
```


## IngestionJobFilterTypeDef

```python
# IngestionJobFilterTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import IngestionJobFilterTypeDef


def get_value() -> IngestionJobFilterTypeDef:
    return {
        "attribute": ...,
    }


# IngestionJobFilterTypeDef definition

class IngestionJobFilterTypeDef(TypedDict):
    attribute: IngestionJobFilterAttributeType,  # (1)
    operator: IngestionJobFilterOperatorType,  # (2)
    values: Sequence[str],
```

1. See [:material-code-brackets: IngestionJobFilterAttributeType](./literals.md#ingestionjobfilterattributetype)
2. See [:material-code-brackets: IngestionJobFilterOperatorType](./literals.md#ingestionjobfilteroperatortype)

## IngestionJobSortByTypeDef

```python
# IngestionJobSortByTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import IngestionJobSortByTypeDef


def get_value() -> IngestionJobSortByTypeDef:
    return {
        "attribute": ...,
    }


# IngestionJobSortByTypeDef definition

class IngestionJobSortByTypeDef(TypedDict):
    attribute: IngestionJobSortByAttributeType,  # (1)
    order: SortOrderType,  # (2)
```

1. See [:material-code-brackets: IngestionJobSortByAttributeType](./literals.md#ingestionjobsortbyattributetype)
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype)

## IngestionJobStatisticsTypeDef

```python
# IngestionJobStatisticsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import IngestionJobStatisticsTypeDef


def get_value() -> IngestionJobStatisticsTypeDef:
    return {
        "numberOfDocumentsDeleted": ...,
    }


# IngestionJobStatisticsTypeDef definition

class IngestionJobStatisticsTypeDef(TypedDict):
    numberOfDocumentsDeleted: NotRequired[int],
    numberOfDocumentsFailed: NotRequired[int],
    numberOfDocumentsScanned: NotRequired[int],
    numberOfMetadataDocumentsModified: NotRequired[int],
    numberOfMetadataDocumentsScanned: NotRequired[int],
    numberOfModifiedDocumentsIndexed: NotRequired[int],
    numberOfNewDocumentsIndexed: NotRequired[int],
```


## TextContentDocTypeDef

```python
# TextContentDocTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import TextContentDocTypeDef


def get_value() -> TextContentDocTypeDef:
    return {
        "data": ...,
    }


# TextContentDocTypeDef definition

class TextContentDocTypeDef(TypedDict):
    data: str,
```


## KendraKnowledgeBaseConfigurationTypeDef

```python
# KendraKnowledgeBaseConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import KendraKnowledgeBaseConfigurationTypeDef


def get_value() -> KendraKnowledgeBaseConfigurationTypeDef:
    return {
        "kendraIndexArn": ...,
    }


# KendraKnowledgeBaseConfigurationTypeDef definition

class KendraKnowledgeBaseConfigurationTypeDef(TypedDict):
    kendraIndexArn: str,
```


## KnowledgeBaseSummaryTypeDef

```python
# KnowledgeBaseSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import KnowledgeBaseSummaryTypeDef


def get_value() -> KnowledgeBaseSummaryTypeDef:
    return {
        "description": ...,
    }


# KnowledgeBaseSummaryTypeDef definition

class KnowledgeBaseSummaryTypeDef(TypedDict):
    knowledgeBaseId: str,
    name: str,
    status: KnowledgeBaseStatusType,  # (1)
    updatedAt: datetime.datetime,
    description: NotRequired[str],
```

1. See [:material-code-brackets: KnowledgeBaseStatusType](./literals.md#knowledgebasestatustype)

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PaginatorConfigTypeDef


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


## ListAgentActionGroupsRequestTypeDef

```python
# ListAgentActionGroupsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListAgentActionGroupsRequestTypeDef


def get_value() -> ListAgentActionGroupsRequestTypeDef:
    return {
        "agentId": ...,
    }


# ListAgentActionGroupsRequestTypeDef definition

class ListAgentActionGroupsRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListAgentAliasesRequestTypeDef

```python
# ListAgentAliasesRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListAgentAliasesRequestTypeDef


def get_value() -> ListAgentAliasesRequestTypeDef:
    return {
        "agentId": ...,
    }


# ListAgentAliasesRequestTypeDef definition

class ListAgentAliasesRequestTypeDef(TypedDict):
    agentId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListAgentCollaboratorsRequestTypeDef

```python
# ListAgentCollaboratorsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListAgentCollaboratorsRequestTypeDef


def get_value() -> ListAgentCollaboratorsRequestTypeDef:
    return {
        "agentId": ...,
    }


# ListAgentCollaboratorsRequestTypeDef definition

class ListAgentCollaboratorsRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListAgentKnowledgeBasesRequestTypeDef

```python
# ListAgentKnowledgeBasesRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListAgentKnowledgeBasesRequestTypeDef


def get_value() -> ListAgentKnowledgeBasesRequestTypeDef:
    return {
        "agentId": ...,
    }


# ListAgentKnowledgeBasesRequestTypeDef definition

class ListAgentKnowledgeBasesRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListAgentVersionsRequestTypeDef

```python
# ListAgentVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListAgentVersionsRequestTypeDef


def get_value() -> ListAgentVersionsRequestTypeDef:
    return {
        "agentId": ...,
    }


# ListAgentVersionsRequestTypeDef definition

class ListAgentVersionsRequestTypeDef(TypedDict):
    agentId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListAgentsRequestTypeDef

```python
# ListAgentsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListAgentsRequestTypeDef


def get_value() -> ListAgentsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListAgentsRequestTypeDef definition

class ListAgentsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListDataSourcesRequestTypeDef

```python
# ListDataSourcesRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListDataSourcesRequestTypeDef


def get_value() -> ListDataSourcesRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# ListDataSourcesRequestTypeDef definition

class ListDataSourcesRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListFlowAliasesRequestTypeDef

```python
# ListFlowAliasesRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListFlowAliasesRequestTypeDef


def get_value() -> ListFlowAliasesRequestTypeDef:
    return {
        "flowIdentifier": ...,
    }


# ListFlowAliasesRequestTypeDef definition

class ListFlowAliasesRequestTypeDef(TypedDict):
    flowIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListFlowVersionsRequestTypeDef

```python
# ListFlowVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListFlowVersionsRequestTypeDef


def get_value() -> ListFlowVersionsRequestTypeDef:
    return {
        "flowIdentifier": ...,
    }


# ListFlowVersionsRequestTypeDef definition

class ListFlowVersionsRequestTypeDef(TypedDict):
    flowIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListFlowsRequestTypeDef

```python
# ListFlowsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListFlowsRequestTypeDef


def get_value() -> ListFlowsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListFlowsRequestTypeDef definition

class ListFlowsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListKnowledgeBaseDocumentsRequestTypeDef

```python
# ListKnowledgeBaseDocumentsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListKnowledgeBaseDocumentsRequestTypeDef


def get_value() -> ListKnowledgeBaseDocumentsRequestTypeDef:
    return {
        "dataSourceId": ...,
    }


# ListKnowledgeBaseDocumentsRequestTypeDef definition

class ListKnowledgeBaseDocumentsRequestTypeDef(TypedDict):
    dataSourceId: str,
    knowledgeBaseId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListKnowledgeBasesRequestTypeDef

```python
# ListKnowledgeBasesRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListKnowledgeBasesRequestTypeDef


def get_value() -> ListKnowledgeBasesRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListKnowledgeBasesRequestTypeDef definition

class ListKnowledgeBasesRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListPromptsRequestTypeDef

```python
# ListPromptsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListPromptsRequestTypeDef


def get_value() -> ListPromptsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListPromptsRequestTypeDef definition

class ListPromptsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    promptIdentifier: NotRequired[str],
```


## PromptSummaryTypeDef

```python
# PromptSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptSummaryTypeDef


def get_value() -> PromptSummaryTypeDef:
    return {
        "arn": ...,
    }


# PromptSummaryTypeDef definition

class PromptSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime.datetime,
    id: str,
    name: str,
    updatedAt: datetime.datetime,
    version: str,
    description: NotRequired[str],
```


## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```


## SessionSummaryConfigurationTypeDef

```python
# SessionSummaryConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import SessionSummaryConfigurationTypeDef


def get_value() -> SessionSummaryConfigurationTypeDef:
    return {
        "maxRecentSessions": ...,
    }


# SessionSummaryConfigurationTypeDef definition

class SessionSummaryConfigurationTypeDef(TypedDict):
    maxRecentSessions: NotRequired[int],
```


## MetadataAttributeValueTypeDef

```python
# MetadataAttributeValueTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import MetadataAttributeValueTypeDef


def get_value() -> MetadataAttributeValueTypeDef:
    return {
        "booleanValue": ...,
    }


# MetadataAttributeValueTypeDef definition

class MetadataAttributeValueTypeDef(TypedDict):
    type: MetadataValueTypeType,  # (1)
    booleanValue: NotRequired[bool],
    numberValue: NotRequired[float],
    stringListValue: NotRequired[Sequence[str]],
    stringValue: NotRequired[str],
```

1. See [:material-code-brackets: MetadataValueTypeType](./literals.md#metadatavaluetypetype)

## MongoDbAtlasFieldMappingTypeDef

```python
# MongoDbAtlasFieldMappingTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import MongoDbAtlasFieldMappingTypeDef


def get_value() -> MongoDbAtlasFieldMappingTypeDef:
    return {
        "metadataField": ...,
    }


# MongoDbAtlasFieldMappingTypeDef definition

class MongoDbAtlasFieldMappingTypeDef(TypedDict):
    metadataField: str,
    textField: str,
    vectorField: str,
```


## OpenSearchServerlessFieldMappingTypeDef

```python
# OpenSearchServerlessFieldMappingTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import OpenSearchServerlessFieldMappingTypeDef


def get_value() -> OpenSearchServerlessFieldMappingTypeDef:
    return {
        "metadataField": ...,
    }


# OpenSearchServerlessFieldMappingTypeDef definition

class OpenSearchServerlessFieldMappingTypeDef(TypedDict):
    metadataField: str,
    textField: str,
    vectorField: str,
```


## PatternObjectFilterOutputTypeDef

```python
# PatternObjectFilterOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PatternObjectFilterOutputTypeDef


def get_value() -> PatternObjectFilterOutputTypeDef:
    return {
        "exclusionFilters": ...,
    }


# PatternObjectFilterOutputTypeDef definition

class PatternObjectFilterOutputTypeDef(TypedDict):
    objectType: str,
    exclusionFilters: NotRequired[List[str]],
    inclusionFilters: NotRequired[List[str]],
```


## PatternObjectFilterTypeDef

```python
# PatternObjectFilterTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PatternObjectFilterTypeDef


def get_value() -> PatternObjectFilterTypeDef:
    return {
        "exclusionFilters": ...,
    }


# PatternObjectFilterTypeDef definition

class PatternObjectFilterTypeDef(TypedDict):
    objectType: str,
    exclusionFilters: NotRequired[Sequence[str]],
    inclusionFilters: NotRequired[Sequence[str]],
```


## PineconeFieldMappingTypeDef

```python
# PineconeFieldMappingTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PineconeFieldMappingTypeDef


def get_value() -> PineconeFieldMappingTypeDef:
    return {
        "metadataField": ...,
    }


# PineconeFieldMappingTypeDef definition

class PineconeFieldMappingTypeDef(TypedDict):
    metadataField: str,
    textField: str,
```


## PrepareAgentRequestTypeDef

```python
# PrepareAgentRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PrepareAgentRequestTypeDef


def get_value() -> PrepareAgentRequestTypeDef:
    return {
        "agentId": ...,
    }


# PrepareAgentRequestTypeDef definition

class PrepareAgentRequestTypeDef(TypedDict):
    agentId: str,
```


## PrepareFlowRequestTypeDef

```python
# PrepareFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PrepareFlowRequestTypeDef


def get_value() -> PrepareFlowRequestTypeDef:
    return {
        "flowIdentifier": ...,
    }


# PrepareFlowRequestTypeDef definition

class PrepareFlowRequestTypeDef(TypedDict):
    flowIdentifier: str,
```


## PromptAgentResourceTypeDef

```python
# PromptAgentResourceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptAgentResourceTypeDef


def get_value() -> PromptAgentResourceTypeDef:
    return {
        "agentIdentifier": ...,
    }


# PromptAgentResourceTypeDef definition

class PromptAgentResourceTypeDef(TypedDict):
    agentIdentifier: str,
```


## PromptFlowNodeResourceConfigurationTypeDef

```python
# PromptFlowNodeResourceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptFlowNodeResourceConfigurationTypeDef


def get_value() -> PromptFlowNodeResourceConfigurationTypeDef:
    return {
        "promptArn": ...,
    }


# PromptFlowNodeResourceConfigurationTypeDef definition

class PromptFlowNodeResourceConfigurationTypeDef(TypedDict):
    promptArn: str,
```


## PromptModelInferenceConfigurationOutputTypeDef

```python
# PromptModelInferenceConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptModelInferenceConfigurationOutputTypeDef


def get_value() -> PromptModelInferenceConfigurationOutputTypeDef:
    return {
        "maxTokens": ...,
    }


# PromptModelInferenceConfigurationOutputTypeDef definition

class PromptModelInferenceConfigurationOutputTypeDef(TypedDict):
    maxTokens: NotRequired[int],
    stopSequences: NotRequired[List[str]],
    temperature: NotRequired[float],
    topP: NotRequired[float],
```


## PromptMetadataEntryTypeDef

```python
# PromptMetadataEntryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptMetadataEntryTypeDef


def get_value() -> PromptMetadataEntryTypeDef:
    return {
        "key": ...,
    }


# PromptMetadataEntryTypeDef definition

class PromptMetadataEntryTypeDef(TypedDict):
    key: str,
    value: str,
```


## PromptModelInferenceConfigurationTypeDef

```python
# PromptModelInferenceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptModelInferenceConfigurationTypeDef


def get_value() -> PromptModelInferenceConfigurationTypeDef:
    return {
        "maxTokens": ...,
    }


# PromptModelInferenceConfigurationTypeDef definition

class PromptModelInferenceConfigurationTypeDef(TypedDict):
    maxTokens: NotRequired[int],
    stopSequences: NotRequired[Sequence[str]],
    temperature: NotRequired[float],
    topP: NotRequired[float],
```


## QueryGenerationColumnTypeDef

```python
# QueryGenerationColumnTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import QueryGenerationColumnTypeDef


def get_value() -> QueryGenerationColumnTypeDef:
    return {
        "description": ...,
    }


# QueryGenerationColumnTypeDef definition

class QueryGenerationColumnTypeDef(TypedDict):
    description: NotRequired[str],
    inclusion: NotRequired[IncludeExcludeType],  # (1)
    name: NotRequired[str],
```

1. See [:material-code-brackets: IncludeExcludeType](./literals.md#includeexcludetype)

## RdsFieldMappingTypeDef

```python
# RdsFieldMappingTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import RdsFieldMappingTypeDef


def get_value() -> RdsFieldMappingTypeDef:
    return {
        "metadataField": ...,
    }


# RdsFieldMappingTypeDef definition

class RdsFieldMappingTypeDef(TypedDict):
    metadataField: str,
    primaryKeyField: str,
    textField: str,
    vectorField: str,
```


## RedisEnterpriseCloudFieldMappingTypeDef

```python
# RedisEnterpriseCloudFieldMappingTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import RedisEnterpriseCloudFieldMappingTypeDef


def get_value() -> RedisEnterpriseCloudFieldMappingTypeDef:
    return {
        "metadataField": ...,
    }


# RedisEnterpriseCloudFieldMappingTypeDef definition

class RedisEnterpriseCloudFieldMappingTypeDef(TypedDict):
    metadataField: str,
    textField: str,
    vectorField: str,
```


## RedshiftProvisionedAuthConfigurationTypeDef

```python
# RedshiftProvisionedAuthConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import RedshiftProvisionedAuthConfigurationTypeDef


def get_value() -> RedshiftProvisionedAuthConfigurationTypeDef:
    return {
        "databaseUser": ...,
    }


# RedshiftProvisionedAuthConfigurationTypeDef definition

class RedshiftProvisionedAuthConfigurationTypeDef(TypedDict):
    type: RedshiftProvisionedAuthTypeType,  # (1)
    databaseUser: NotRequired[str],
    usernamePasswordSecretArn: NotRequired[str],
```

1. See [:material-code-brackets: RedshiftProvisionedAuthTypeType](./literals.md#redshiftprovisionedauthtypetype)

## RedshiftQueryEngineAwsDataCatalogStorageConfigurationOutputTypeDef

```python
# RedshiftQueryEngineAwsDataCatalogStorageConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import RedshiftQueryEngineAwsDataCatalogStorageConfigurationOutputTypeDef


def get_value() -> RedshiftQueryEngineAwsDataCatalogStorageConfigurationOutputTypeDef:
    return {
        "tableNames": ...,
    }


# RedshiftQueryEngineAwsDataCatalogStorageConfigurationOutputTypeDef definition

class RedshiftQueryEngineAwsDataCatalogStorageConfigurationOutputTypeDef(TypedDict):
    tableNames: List[str],
```


## RedshiftQueryEngineAwsDataCatalogStorageConfigurationTypeDef

```python
# RedshiftQueryEngineAwsDataCatalogStorageConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import RedshiftQueryEngineAwsDataCatalogStorageConfigurationTypeDef


def get_value() -> RedshiftQueryEngineAwsDataCatalogStorageConfigurationTypeDef:
    return {
        "tableNames": ...,
    }


# RedshiftQueryEngineAwsDataCatalogStorageConfigurationTypeDef definition

class RedshiftQueryEngineAwsDataCatalogStorageConfigurationTypeDef(TypedDict):
    tableNames: Sequence[str],
```


## RedshiftQueryEngineRedshiftStorageConfigurationTypeDef

```python
# RedshiftQueryEngineRedshiftStorageConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import RedshiftQueryEngineRedshiftStorageConfigurationTypeDef


def get_value() -> RedshiftQueryEngineRedshiftStorageConfigurationTypeDef:
    return {
        "databaseName": ...,
    }


# RedshiftQueryEngineRedshiftStorageConfigurationTypeDef definition

class RedshiftQueryEngineRedshiftStorageConfigurationTypeDef(TypedDict):
    databaseName: str,
```


## RedshiftServerlessAuthConfigurationTypeDef

```python
# RedshiftServerlessAuthConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import RedshiftServerlessAuthConfigurationTypeDef


def get_value() -> RedshiftServerlessAuthConfigurationTypeDef:
    return {
        "type": ...,
    }


# RedshiftServerlessAuthConfigurationTypeDef definition

class RedshiftServerlessAuthConfigurationTypeDef(TypedDict):
    type: RedshiftServerlessAuthTypeType,  # (1)
    usernamePasswordSecretArn: NotRequired[str],
```

1. See [:material-code-brackets: RedshiftServerlessAuthTypeType](./literals.md#redshiftserverlessauthtypetype)

## RetrievalFlowNodeS3ConfigurationTypeDef

```python
# RetrievalFlowNodeS3ConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import RetrievalFlowNodeS3ConfigurationTypeDef


def get_value() -> RetrievalFlowNodeS3ConfigurationTypeDef:
    return {
        "bucketName": ...,
    }


# RetrievalFlowNodeS3ConfigurationTypeDef definition

class RetrievalFlowNodeS3ConfigurationTypeDef(TypedDict):
    bucketName: str,
```


## SalesforceSourceConfigurationTypeDef

```python
# SalesforceSourceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import SalesforceSourceConfigurationTypeDef


def get_value() -> SalesforceSourceConfigurationTypeDef:
    return {
        "authType": ...,
    }


# SalesforceSourceConfigurationTypeDef definition

class SalesforceSourceConfigurationTypeDef(TypedDict):
    authType: SalesforceAuthTypeType,  # (1)
    credentialsSecretArn: str,
    hostUrl: str,
```

1. See [:material-code-brackets: SalesforceAuthTypeType](./literals.md#salesforceauthtypetype)

## SeedUrlTypeDef

```python
# SeedUrlTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import SeedUrlTypeDef


def get_value() -> SeedUrlTypeDef:
    return {
        "url": ...,
    }


# SeedUrlTypeDef definition

class SeedUrlTypeDef(TypedDict):
    url: NotRequired[str],
```


## SharePointSourceConfigurationOutputTypeDef

```python
# SharePointSourceConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import SharePointSourceConfigurationOutputTypeDef


def get_value() -> SharePointSourceConfigurationOutputTypeDef:
    return {
        "authType": ...,
    }


# SharePointSourceConfigurationOutputTypeDef definition

class SharePointSourceConfigurationOutputTypeDef(TypedDict):
    authType: SharePointAuthTypeType,  # (1)
    credentialsSecretArn: str,
    domain: str,
    hostType: SharePointHostTypeType,  # (2)
    siteUrls: List[str],
    tenantId: NotRequired[str],
```

1. See [:material-code-brackets: SharePointAuthTypeType](./literals.md#sharepointauthtypetype)
2. See [:material-code-brackets: SharePointHostTypeType](./literals.md#sharepointhosttypetype)

## SharePointSourceConfigurationTypeDef

```python
# SharePointSourceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import SharePointSourceConfigurationTypeDef


def get_value() -> SharePointSourceConfigurationTypeDef:
    return {
        "authType": ...,
    }


# SharePointSourceConfigurationTypeDef definition

class SharePointSourceConfigurationTypeDef(TypedDict):
    authType: SharePointAuthTypeType,  # (1)
    credentialsSecretArn: str,
    domain: str,
    hostType: SharePointHostTypeType,  # (2)
    siteUrls: Sequence[str],
    tenantId: NotRequired[str],
```

1. See [:material-code-brackets: SharePointAuthTypeType](./literals.md#sharepointauthtypetype)
2. See [:material-code-brackets: SharePointHostTypeType](./literals.md#sharepointhosttypetype)

## SpecificToolChoiceTypeDef

```python
# SpecificToolChoiceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import SpecificToolChoiceTypeDef


def get_value() -> SpecificToolChoiceTypeDef:
    return {
        "name": ...,
    }


# SpecificToolChoiceTypeDef definition

class SpecificToolChoiceTypeDef(TypedDict):
    name: str,
```


## StartIngestionJobRequestTypeDef

```python
# StartIngestionJobRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import StartIngestionJobRequestTypeDef


def get_value() -> StartIngestionJobRequestTypeDef:
    return {
        "dataSourceId": ...,
    }


# StartIngestionJobRequestTypeDef definition

class StartIngestionJobRequestTypeDef(TypedDict):
    dataSourceId: str,
    knowledgeBaseId: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
```


## StopIngestionJobRequestTypeDef

```python
# StopIngestionJobRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import StopIngestionJobRequestTypeDef


def get_value() -> StopIngestionJobRequestTypeDef:
    return {
        "dataSourceId": ...,
    }


# StopIngestionJobRequestTypeDef definition

class StopIngestionJobRequestTypeDef(TypedDict):
    dataSourceId: str,
    ingestionJobId: str,
    knowledgeBaseId: str,
```


## StorageFlowNodeS3ConfigurationTypeDef

```python
# StorageFlowNodeS3ConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import StorageFlowNodeS3ConfigurationTypeDef


def get_value() -> StorageFlowNodeS3ConfigurationTypeDef:
    return {
        "bucketName": ...,
    }


# StorageFlowNodeS3ConfigurationTypeDef definition

class StorageFlowNodeS3ConfigurationTypeDef(TypedDict):
    bucketName: str,
```


## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```


## ToolInputSchemaOutputTypeDef

```python
# ToolInputSchemaOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ToolInputSchemaOutputTypeDef


def get_value() -> ToolInputSchemaOutputTypeDef:
    return {
        "json": ...,
    }


# ToolInputSchemaOutputTypeDef definition

class ToolInputSchemaOutputTypeDef(TypedDict):
    json: NotRequired[Dict[str, Any]],
```


## ToolInputSchemaTypeDef

```python
# ToolInputSchemaTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ToolInputSchemaTypeDef


def get_value() -> ToolInputSchemaTypeDef:
    return {
        "json": ...,
    }


# ToolInputSchemaTypeDef definition

class ToolInputSchemaTypeDef(TypedDict):
    json: NotRequired[Mapping[str, Any]],
```


## TransformationLambdaConfigurationTypeDef

```python
# TransformationLambdaConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import TransformationLambdaConfigurationTypeDef


def get_value() -> TransformationLambdaConfigurationTypeDef:
    return {
        "lambdaArn": ...,
    }


# TransformationLambdaConfigurationTypeDef definition

class TransformationLambdaConfigurationTypeDef(TypedDict):
    lambdaArn: str,
```


## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```


## UpdateAgentKnowledgeBaseRequestTypeDef

```python
# UpdateAgentKnowledgeBaseRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UpdateAgentKnowledgeBaseRequestTypeDef


def get_value() -> UpdateAgentKnowledgeBaseRequestTypeDef:
    return {
        "agentId": ...,
    }


# UpdateAgentKnowledgeBaseRequestTypeDef definition

class UpdateAgentKnowledgeBaseRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    knowledgeBaseId: str,
    description: NotRequired[str],
    knowledgeBaseState: NotRequired[KnowledgeBaseStateType],  # (1)
```

1. See [:material-code-brackets: KnowledgeBaseStateType](./literals.md#knowledgebasestatetype)

## WebCrawlerLimitsTypeDef

```python
# WebCrawlerLimitsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import WebCrawlerLimitsTypeDef


def get_value() -> WebCrawlerLimitsTypeDef:
    return {
        "maxPages": ...,
    }


# WebCrawlerLimitsTypeDef definition

class WebCrawlerLimitsTypeDef(TypedDict):
    maxPages: NotRequired[int],
    rateLimit: NotRequired[int],
```


## APISchemaTypeDef

```python
# APISchemaTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import APISchemaTypeDef


def get_value() -> APISchemaTypeDef:
    return {
        "payload": ...,
    }


# APISchemaTypeDef definition

class APISchemaTypeDef(TypedDict):
    payload: NotRequired[str],
    s3: NotRequired[S3IdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: S3IdentifierTypeDef](./type_defs.md#s3identifiertypedef)

## AgentAliasHistoryEventTypeDef

```python
# AgentAliasHistoryEventTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import AgentAliasHistoryEventTypeDef


def get_value() -> AgentAliasHistoryEventTypeDef:
    return {
        "endDate": ...,
    }


# AgentAliasHistoryEventTypeDef definition

class AgentAliasHistoryEventTypeDef(TypedDict):
    endDate: NotRequired[datetime.datetime],
    routingConfiguration: NotRequired[List[AgentAliasRoutingConfigurationListItemTypeDef]],  # (1)
    startDate: NotRequired[datetime.datetime],
```

1. See `List[AgentAliasRoutingConfigurationListItemTypeDef]`

## AgentAliasSummaryTypeDef

```python
# AgentAliasSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import AgentAliasSummaryTypeDef


def get_value() -> AgentAliasSummaryTypeDef:
    return {
        "agentAliasId": ...,
    }


# AgentAliasSummaryTypeDef definition

class AgentAliasSummaryTypeDef(TypedDict):
    agentAliasId: str,
    agentAliasName: str,
    agentAliasStatus: AgentAliasStatusType,  # (1)
    createdAt: datetime.datetime,
    updatedAt: datetime.datetime,
    description: NotRequired[str],
    routingConfiguration: NotRequired[List[AgentAliasRoutingConfigurationListItemTypeDef]],  # (2)
```

1. See [:material-code-brackets: AgentAliasStatusType](./literals.md#agentaliasstatustype)
2. See `List[AgentAliasRoutingConfigurationListItemTypeDef]`

## CreateAgentAliasRequestTypeDef

```python
# CreateAgentAliasRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CreateAgentAliasRequestTypeDef


def get_value() -> CreateAgentAliasRequestTypeDef:
    return {
        "agentAliasName": ...,
    }


# CreateAgentAliasRequestTypeDef definition

class CreateAgentAliasRequestTypeDef(TypedDict):
    agentAliasName: str,
    agentId: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    routingConfiguration: NotRequired[Sequence[AgentAliasRoutingConfigurationListItemTypeDef]],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See `Sequence[AgentAliasRoutingConfigurationListItemTypeDef]`

## UpdateAgentAliasRequestTypeDef

```python
# UpdateAgentAliasRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UpdateAgentAliasRequestTypeDef


def get_value() -> UpdateAgentAliasRequestTypeDef:
    return {
        "agentAliasId": ...,
    }


# UpdateAgentAliasRequestTypeDef definition

class UpdateAgentAliasRequestTypeDef(TypedDict):
    agentAliasId: str,
    agentAliasName: str,
    agentId: str,
    description: NotRequired[str],
    routingConfiguration: NotRequired[Sequence[AgentAliasRoutingConfigurationListItemTypeDef]],  # (1)
```

1. See `Sequence[AgentAliasRoutingConfigurationListItemTypeDef]`

## AgentCollaboratorSummaryTypeDef

```python
# AgentCollaboratorSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import AgentCollaboratorSummaryTypeDef


def get_value() -> AgentCollaboratorSummaryTypeDef:
    return {
        "agentDescriptor": ...,
    }


# AgentCollaboratorSummaryTypeDef definition

class AgentCollaboratorSummaryTypeDef(TypedDict):
    agentDescriptor: AgentDescriptorTypeDef,  # (1)
    agentId: str,
    agentVersion: str,
    collaborationInstruction: str,
    collaboratorId: str,
    collaboratorName: str,
    createdAt: datetime.datetime,
    lastUpdatedAt: datetime.datetime,
    relayConversationHistory: RelayConversationHistoryType,  # (2)
```

1. See [:material-code-braces: AgentDescriptorTypeDef](./type_defs.md#agentdescriptortypedef)
2. See [:material-code-brackets: RelayConversationHistoryType](./literals.md#relayconversationhistorytype)

## AgentCollaboratorTypeDef

```python
# AgentCollaboratorTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import AgentCollaboratorTypeDef


def get_value() -> AgentCollaboratorTypeDef:
    return {
        "agentDescriptor": ...,
    }


# AgentCollaboratorTypeDef definition

class AgentCollaboratorTypeDef(TypedDict):
    agentDescriptor: AgentDescriptorTypeDef,  # (1)
    agentId: str,
    agentVersion: str,
    collaborationInstruction: str,
    collaboratorId: str,
    collaboratorName: str,
    createdAt: datetime.datetime,
    lastUpdatedAt: datetime.datetime,
    clientToken: NotRequired[str],
    relayConversationHistory: NotRequired[RelayConversationHistoryType],  # (2)
```

1. See [:material-code-braces: AgentDescriptorTypeDef](./type_defs.md#agentdescriptortypedef)
2. See [:material-code-brackets: RelayConversationHistoryType](./literals.md#relayconversationhistorytype)

## AssociateAgentCollaboratorRequestTypeDef

```python
# AssociateAgentCollaboratorRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import AssociateAgentCollaboratorRequestTypeDef


def get_value() -> AssociateAgentCollaboratorRequestTypeDef:
    return {
        "agentDescriptor": ...,
    }


# AssociateAgentCollaboratorRequestTypeDef definition

class AssociateAgentCollaboratorRequestTypeDef(TypedDict):
    agentDescriptor: AgentDescriptorTypeDef,  # (1)
    agentId: str,
    agentVersion: str,
    collaborationInstruction: str,
    collaboratorName: str,
    clientToken: NotRequired[str],
    relayConversationHistory: NotRequired[RelayConversationHistoryType],  # (2)
```

1. See [:material-code-braces: AgentDescriptorTypeDef](./type_defs.md#agentdescriptortypedef)
2. See [:material-code-brackets: RelayConversationHistoryType](./literals.md#relayconversationhistorytype)

## UpdateAgentCollaboratorRequestTypeDef

```python
# UpdateAgentCollaboratorRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UpdateAgentCollaboratorRequestTypeDef


def get_value() -> UpdateAgentCollaboratorRequestTypeDef:
    return {
        "agentDescriptor": ...,
    }


# UpdateAgentCollaboratorRequestTypeDef definition

class UpdateAgentCollaboratorRequestTypeDef(TypedDict):
    agentDescriptor: AgentDescriptorTypeDef,  # (1)
    agentId: str,
    agentVersion: str,
    collaborationInstruction: str,
    collaboratorId: str,
    collaboratorName: str,
    relayConversationHistory: NotRequired[RelayConversationHistoryType],  # (2)
```

1. See [:material-code-braces: AgentDescriptorTypeDef](./type_defs.md#agentdescriptortypedef)
2. See [:material-code-brackets: RelayConversationHistoryType](./literals.md#relayconversationhistorytype)

## AgentSummaryTypeDef

```python
# AgentSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import AgentSummaryTypeDef


def get_value() -> AgentSummaryTypeDef:
    return {
        "agentId": ...,
    }


# AgentSummaryTypeDef definition

class AgentSummaryTypeDef(TypedDict):
    agentId: str,
    agentName: str,
    agentStatus: AgentStatusType,  # (1)
    updatedAt: datetime.datetime,
    description: NotRequired[str],
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (2)
    latestAgentVersion: NotRequired[str],
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype)
2. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef)

## AgentVersionSummaryTypeDef

```python
# AgentVersionSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import AgentVersionSummaryTypeDef


def get_value() -> AgentVersionSummaryTypeDef:
    return {
        "agentName": ...,
    }


# AgentVersionSummaryTypeDef definition

class AgentVersionSummaryTypeDef(TypedDict):
    agentName: str,
    agentStatus: AgentStatusType,  # (1)
    agentVersion: str,
    createdAt: datetime.datetime,
    updatedAt: datetime.datetime,
    description: NotRequired[str],
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype)
2. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef)

## KnowledgeBaseFlowNodeConfigurationTypeDef

```python
# KnowledgeBaseFlowNodeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import KnowledgeBaseFlowNodeConfigurationTypeDef


def get_value() -> KnowledgeBaseFlowNodeConfigurationTypeDef:
    return {
        "guardrailConfiguration": ...,
    }


# KnowledgeBaseFlowNodeConfigurationTypeDef definition

class KnowledgeBaseFlowNodeConfigurationTypeDef(TypedDict):
    knowledgeBaseId: str,
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (1)
    modelId: NotRequired[str],
```

1. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef)

## AssociateAgentKnowledgeBaseResponseTypeDef

```python
# AssociateAgentKnowledgeBaseResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import AssociateAgentKnowledgeBaseResponseTypeDef


def get_value() -> AssociateAgentKnowledgeBaseResponseTypeDef:
    return {
        "agentKnowledgeBase": ...,
    }


# AssociateAgentKnowledgeBaseResponseTypeDef definition

class AssociateAgentKnowledgeBaseResponseTypeDef(TypedDict):
    agentKnowledgeBase: AgentKnowledgeBaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentKnowledgeBaseTypeDef](./type_defs.md#agentknowledgebasetypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeleteAgentAliasResponseTypeDef

```python
# DeleteAgentAliasResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DeleteAgentAliasResponseTypeDef


def get_value() -> DeleteAgentAliasResponseTypeDef:
    return {
        "agentAliasId": ...,
    }


# DeleteAgentAliasResponseTypeDef definition

class DeleteAgentAliasResponseTypeDef(TypedDict):
    agentAliasId: str,
    agentAliasStatus: AgentAliasStatusType,  # (1)
    agentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AgentAliasStatusType](./literals.md#agentaliasstatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeleteAgentResponseTypeDef

```python
# DeleteAgentResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DeleteAgentResponseTypeDef


def get_value() -> DeleteAgentResponseTypeDef:
    return {
        "agentId": ...,
    }


# DeleteAgentResponseTypeDef definition

class DeleteAgentResponseTypeDef(TypedDict):
    agentId: str,
    agentStatus: AgentStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeleteAgentVersionResponseTypeDef

```python
# DeleteAgentVersionResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DeleteAgentVersionResponseTypeDef


def get_value() -> DeleteAgentVersionResponseTypeDef:
    return {
        "agentId": ...,
    }


# DeleteAgentVersionResponseTypeDef definition

class DeleteAgentVersionResponseTypeDef(TypedDict):
    agentId: str,
    agentStatus: AgentStatusType,  # (1)
    agentVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeleteDataSourceResponseTypeDef

```python
# DeleteDataSourceResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DeleteDataSourceResponseTypeDef


def get_value() -> DeleteDataSourceResponseTypeDef:
    return {
        "dataSourceId": ...,
    }


# DeleteDataSourceResponseTypeDef definition

class DeleteDataSourceResponseTypeDef(TypedDict):
    dataSourceId: str,
    knowledgeBaseId: str,
    status: DataSourceStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeleteFlowAliasResponseTypeDef

```python
# DeleteFlowAliasResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DeleteFlowAliasResponseTypeDef


def get_value() -> DeleteFlowAliasResponseTypeDef:
    return {
        "flowId": ...,
    }


# DeleteFlowAliasResponseTypeDef definition

class DeleteFlowAliasResponseTypeDef(TypedDict):
    flowId: str,
    id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeleteFlowResponseTypeDef

```python
# DeleteFlowResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DeleteFlowResponseTypeDef


def get_value() -> DeleteFlowResponseTypeDef:
    return {
        "id": ...,
    }


# DeleteFlowResponseTypeDef definition

class DeleteFlowResponseTypeDef(TypedDict):
    id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeleteFlowVersionResponseTypeDef

```python
# DeleteFlowVersionResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DeleteFlowVersionResponseTypeDef


def get_value() -> DeleteFlowVersionResponseTypeDef:
    return {
        "id": ...,
    }


# DeleteFlowVersionResponseTypeDef definition

class DeleteFlowVersionResponseTypeDef(TypedDict):
    id: str,
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeleteKnowledgeBaseResponseTypeDef

```python
# DeleteKnowledgeBaseResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DeleteKnowledgeBaseResponseTypeDef


def get_value() -> DeleteKnowledgeBaseResponseTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# DeleteKnowledgeBaseResponseTypeDef definition

class DeleteKnowledgeBaseResponseTypeDef(TypedDict):
    knowledgeBaseId: str,
    status: KnowledgeBaseStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: KnowledgeBaseStatusType](./literals.md#knowledgebasestatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeletePromptResponseTypeDef

```python
# DeletePromptResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DeletePromptResponseTypeDef


def get_value() -> DeletePromptResponseTypeDef:
    return {
        "id": ...,
    }


# DeletePromptResponseTypeDef definition

class DeletePromptResponseTypeDef(TypedDict):
    id: str,
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetAgentKnowledgeBaseResponseTypeDef

```python
# GetAgentKnowledgeBaseResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetAgentKnowledgeBaseResponseTypeDef


def get_value() -> GetAgentKnowledgeBaseResponseTypeDef:
    return {
        "agentKnowledgeBase": ...,
    }


# GetAgentKnowledgeBaseResponseTypeDef definition

class GetAgentKnowledgeBaseResponseTypeDef(TypedDict):
    agentKnowledgeBase: AgentKnowledgeBaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentKnowledgeBaseTypeDef](./type_defs.md#agentknowledgebasetypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListAgentActionGroupsResponseTypeDef

```python
# ListAgentActionGroupsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListAgentActionGroupsResponseTypeDef


def get_value() -> ListAgentActionGroupsResponseTypeDef:
    return {
        "actionGroupSummaries": ...,
    }


# ListAgentActionGroupsResponseTypeDef definition

class ListAgentActionGroupsResponseTypeDef(TypedDict):
    actionGroupSummaries: List[ActionGroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `List[ActionGroupSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListAgentKnowledgeBasesResponseTypeDef

```python
# ListAgentKnowledgeBasesResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListAgentKnowledgeBasesResponseTypeDef


def get_value() -> ListAgentKnowledgeBasesResponseTypeDef:
    return {
        "agentKnowledgeBaseSummaries": ...,
    }


# ListAgentKnowledgeBasesResponseTypeDef definition

class ListAgentKnowledgeBasesResponseTypeDef(TypedDict):
    agentKnowledgeBaseSummaries: List[AgentKnowledgeBaseSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `List[AgentKnowledgeBaseSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListTagsForResourceResponseTypeDef


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

## PrepareAgentResponseTypeDef

```python
# PrepareAgentResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PrepareAgentResponseTypeDef


def get_value() -> PrepareAgentResponseTypeDef:
    return {
        "agentId": ...,
    }


# PrepareAgentResponseTypeDef definition

class PrepareAgentResponseTypeDef(TypedDict):
    agentId: str,
    agentStatus: AgentStatusType,  # (1)
    agentVersion: str,
    preparedAt: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## PrepareFlowResponseTypeDef

```python
# PrepareFlowResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PrepareFlowResponseTypeDef


def get_value() -> PrepareFlowResponseTypeDef:
    return {
        "id": ...,
    }


# PrepareFlowResponseTypeDef definition

class PrepareFlowResponseTypeDef(TypedDict):
    id: str,
    status: FlowStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: FlowStatusType](./literals.md#flowstatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateAgentKnowledgeBaseResponseTypeDef

```python
# UpdateAgentKnowledgeBaseResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UpdateAgentKnowledgeBaseResponseTypeDef


def get_value() -> UpdateAgentKnowledgeBaseResponseTypeDef:
    return {
        "agentKnowledgeBase": ...,
    }


# UpdateAgentKnowledgeBaseResponseTypeDef definition

class UpdateAgentKnowledgeBaseResponseTypeDef(TypedDict):
    agentKnowledgeBase: AgentKnowledgeBaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentKnowledgeBaseTypeDef](./type_defs.md#agentknowledgebasetypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## EmbeddingModelConfigurationTypeDef

```python
# EmbeddingModelConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import EmbeddingModelConfigurationTypeDef


def get_value() -> EmbeddingModelConfigurationTypeDef:
    return {
        "bedrockEmbeddingModelConfiguration": ...,
    }


# EmbeddingModelConfigurationTypeDef definition

class EmbeddingModelConfigurationTypeDef(TypedDict):
    bedrockEmbeddingModelConfiguration: NotRequired[BedrockEmbeddingModelConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: BedrockEmbeddingModelConfigurationTypeDef](./type_defs.md#bedrockembeddingmodelconfigurationtypedef)

## BedrockFoundationModelConfigurationTypeDef

```python
# BedrockFoundationModelConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import BedrockFoundationModelConfigurationTypeDef


def get_value() -> BedrockFoundationModelConfigurationTypeDef:
    return {
        "modelArn": ...,
    }


# BedrockFoundationModelConfigurationTypeDef definition

class BedrockFoundationModelConfigurationTypeDef(TypedDict):
    modelArn: str,
    parsingModality: NotRequired[ParsingModalityType],  # (1)
    parsingPrompt: NotRequired[ParsingPromptTypeDef],  # (2)
```

1. See [:material-code-brackets: ParsingModalityType](./literals.md#parsingmodalitytype)
2. See [:material-code-braces: ParsingPromptTypeDef](./type_defs.md#parsingprompttypedef)

## ByteContentDocTypeDef

```python
# ByteContentDocTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ByteContentDocTypeDef


def get_value() -> ByteContentDocTypeDef:
    return {
        "data": ...,
    }


# ByteContentDocTypeDef definition

class ByteContentDocTypeDef(TypedDict):
    data: BlobTypeDef,
    mimeType: str,
```


## ContentBlockTypeDef

```python
# ContentBlockTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ContentBlockTypeDef


def get_value() -> ContentBlockTypeDef:
    return {
        "cachePoint": ...,
    }


# ContentBlockTypeDef definition

class ContentBlockTypeDef(TypedDict):
    cachePoint: NotRequired[CachePointBlockTypeDef],  # (1)
    text: NotRequired[str],
```

1. See [:material-code-braces: CachePointBlockTypeDef](./type_defs.md#cachepointblocktypedef)

## SystemContentBlockTypeDef

```python
# SystemContentBlockTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import SystemContentBlockTypeDef


def get_value() -> SystemContentBlockTypeDef:
    return {
        "cachePoint": ...,
    }


# SystemContentBlockTypeDef definition

class SystemContentBlockTypeDef(TypedDict):
    cachePoint: NotRequired[CachePointBlockTypeDef],  # (1)
    text: NotRequired[str],
```

1. See [:material-code-braces: CachePointBlockTypeDef](./type_defs.md#cachepointblocktypedef)

## TextPromptTemplateConfigurationOutputTypeDef

```python
# TextPromptTemplateConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import TextPromptTemplateConfigurationOutputTypeDef


def get_value() -> TextPromptTemplateConfigurationOutputTypeDef:
    return {
        "cachePoint": ...,
    }


# TextPromptTemplateConfigurationOutputTypeDef definition

class TextPromptTemplateConfigurationOutputTypeDef(TypedDict):
    text: str,
    cachePoint: NotRequired[CachePointBlockTypeDef],  # (1)
    inputVariables: NotRequired[List[PromptInputVariableTypeDef]],  # (2)
```

1. See [:material-code-braces: CachePointBlockTypeDef](./type_defs.md#cachepointblocktypedef)
2. See `List[PromptInputVariableTypeDef]`

## TextPromptTemplateConfigurationTypeDef

```python
# TextPromptTemplateConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import TextPromptTemplateConfigurationTypeDef


def get_value() -> TextPromptTemplateConfigurationTypeDef:
    return {
        "cachePoint": ...,
    }


# TextPromptTemplateConfigurationTypeDef definition

class TextPromptTemplateConfigurationTypeDef(TypedDict):
    text: str,
    cachePoint: NotRequired[CachePointBlockTypeDef],  # (1)
    inputVariables: NotRequired[Sequence[PromptInputVariableTypeDef]],  # (2)
```

1. See [:material-code-braces: CachePointBlockTypeDef](./type_defs.md#cachepointblocktypedef)
2. See `Sequence[PromptInputVariableTypeDef]`

## ConditionFlowNodeConfigurationOutputTypeDef

```python
# ConditionFlowNodeConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ConditionFlowNodeConfigurationOutputTypeDef


def get_value() -> ConditionFlowNodeConfigurationOutputTypeDef:
    return {
        "conditions": ...,
    }


# ConditionFlowNodeConfigurationOutputTypeDef definition

class ConditionFlowNodeConfigurationOutputTypeDef(TypedDict):
    conditions: List[FlowConditionTypeDef],  # (1)
```

1. See `List[FlowConditionTypeDef]`

## ConditionFlowNodeConfigurationTypeDef

```python
# ConditionFlowNodeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ConditionFlowNodeConfigurationTypeDef


def get_value() -> ConditionFlowNodeConfigurationTypeDef:
    return {
        "conditions": ...,
    }


# ConditionFlowNodeConfigurationTypeDef definition

class ConditionFlowNodeConfigurationTypeDef(TypedDict):
    conditions: Sequence[FlowConditionTypeDef],  # (1)
```

1. See `Sequence[FlowConditionTypeDef]`

## CreateFlowAliasRequestTypeDef

```python
# CreateFlowAliasRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CreateFlowAliasRequestTypeDef


def get_value() -> CreateFlowAliasRequestTypeDef:
    return {
        "flowIdentifier": ...,
    }


# CreateFlowAliasRequestTypeDef definition

class CreateFlowAliasRequestTypeDef(TypedDict):
    flowIdentifier: str,
    name: str,
    routingConfiguration: Sequence[FlowAliasRoutingConfigurationListItemTypeDef],  # (1)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See `Sequence[FlowAliasRoutingConfigurationListItemTypeDef]`

## CreateFlowAliasResponseTypeDef

```python
# CreateFlowAliasResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CreateFlowAliasResponseTypeDef


def get_value() -> CreateFlowAliasResponseTypeDef:
    return {
        "arn": ...,
    }


# CreateFlowAliasResponseTypeDef definition

class CreateFlowAliasResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime.datetime,
    description: str,
    flowId: str,
    id: str,
    name: str,
    routingConfiguration: List[FlowAliasRoutingConfigurationListItemTypeDef],  # (1)
    updatedAt: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `List[FlowAliasRoutingConfigurationListItemTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## FlowAliasSummaryTypeDef

```python
# FlowAliasSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FlowAliasSummaryTypeDef


def get_value() -> FlowAliasSummaryTypeDef:
    return {
        "arn": ...,
    }


# FlowAliasSummaryTypeDef definition

class FlowAliasSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime.datetime,
    flowId: str,
    id: str,
    name: str,
    routingConfiguration: List[FlowAliasRoutingConfigurationListItemTypeDef],  # (1)
    updatedAt: datetime.datetime,
    description: NotRequired[str],
```

1. See `List[FlowAliasRoutingConfigurationListItemTypeDef]`

## GetFlowAliasResponseTypeDef

```python
# GetFlowAliasResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetFlowAliasResponseTypeDef


def get_value() -> GetFlowAliasResponseTypeDef:
    return {
        "arn": ...,
    }


# GetFlowAliasResponseTypeDef definition

class GetFlowAliasResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime.datetime,
    description: str,
    flowId: str,
    id: str,
    name: str,
    routingConfiguration: List[FlowAliasRoutingConfigurationListItemTypeDef],  # (1)
    updatedAt: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `List[FlowAliasRoutingConfigurationListItemTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateFlowAliasRequestTypeDef

```python
# UpdateFlowAliasRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UpdateFlowAliasRequestTypeDef


def get_value() -> UpdateFlowAliasRequestTypeDef:
    return {
        "aliasIdentifier": ...,
    }


# UpdateFlowAliasRequestTypeDef definition

class UpdateFlowAliasRequestTypeDef(TypedDict):
    aliasIdentifier: str,
    flowIdentifier: str,
    name: str,
    routingConfiguration: Sequence[FlowAliasRoutingConfigurationListItemTypeDef],  # (1)
    description: NotRequired[str],
```

1. See `Sequence[FlowAliasRoutingConfigurationListItemTypeDef]`

## UpdateFlowAliasResponseTypeDef

```python
# UpdateFlowAliasResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UpdateFlowAliasResponseTypeDef


def get_value() -> UpdateFlowAliasResponseTypeDef:
    return {
        "arn": ...,
    }


# UpdateFlowAliasResponseTypeDef definition

class UpdateFlowAliasResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime.datetime,
    description: str,
    flowId: str,
    id: str,
    name: str,
    routingConfiguration: List[FlowAliasRoutingConfigurationListItemTypeDef],  # (1)
    updatedAt: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `List[FlowAliasRoutingConfigurationListItemTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CustomOrchestrationTypeDef

```python
# CustomOrchestrationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CustomOrchestrationTypeDef


def get_value() -> CustomOrchestrationTypeDef:
    return {
        "executor": ...,
    }


# CustomOrchestrationTypeDef definition

class CustomOrchestrationTypeDef(TypedDict):
    executor: NotRequired[OrchestrationExecutorTypeDef],  # (1)
```

1. See [:material-code-braces: OrchestrationExecutorTypeDef](./type_defs.md#orchestrationexecutortypedef)

## ListDataSourcesResponseTypeDef

```python
# ListDataSourcesResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListDataSourcesResponseTypeDef


def get_value() -> ListDataSourcesResponseTypeDef:
    return {
        "dataSourceSummaries": ...,
    }


# ListDataSourcesResponseTypeDef definition

class ListDataSourcesResponseTypeDef(TypedDict):
    dataSourceSummaries: List[DataSourceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `List[DataSourceSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DocumentIdentifierTypeDef

```python
# DocumentIdentifierTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DocumentIdentifierTypeDef


def get_value() -> DocumentIdentifierTypeDef:
    return {
        "custom": ...,
    }


# DocumentIdentifierTypeDef definition

class DocumentIdentifierTypeDef(TypedDict):
    dataSourceType: ContentDataSourceTypeType,  # (2)
    custom: NotRequired[CustomDocumentIdentifierTypeDef],  # (1)
    s3: NotRequired[S3LocationTypeDef],  # (3)
```

1. See [:material-code-braces: CustomDocumentIdentifierTypeDef](./type_defs.md#customdocumentidentifiertypedef)
2. See [:material-code-brackets: ContentDataSourceTypeType](./literals.md#contentdatasourcetypetype)
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef)

## IntermediateStorageTypeDef

```python
# IntermediateStorageTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import IntermediateStorageTypeDef


def get_value() -> IntermediateStorageTypeDef:
    return {
        "s3Location": ...,
    }


# IntermediateStorageTypeDef definition

class IntermediateStorageTypeDef(TypedDict):
    s3Location: S3LocationTypeDef,  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef)

## S3ContentTypeDef

```python
# S3ContentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import S3ContentTypeDef


def get_value() -> S3ContentTypeDef:
    return {
        "s3Location": ...,
    }


# S3ContentTypeDef definition

class S3ContentTypeDef(TypedDict):
    s3Location: S3LocationTypeDef,  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef)

## SupplementalDataStorageLocationTypeDef

```python
# SupplementalDataStorageLocationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import SupplementalDataStorageLocationTypeDef


def get_value() -> SupplementalDataStorageLocationTypeDef:
    return {
        "s3Location": ...,
    }


# SupplementalDataStorageLocationTypeDef definition

class SupplementalDataStorageLocationTypeDef(TypedDict):
    type: SupplementalDataStorageLocationTypeType,  # (2)
    s3Location: NotRequired[S3LocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef)
2. See [:material-code-brackets: SupplementalDataStorageLocationTypeType](./literals.md#supplementaldatastoragelocationtypetype)

## FlowConnectionConfigurationTypeDef

```python
# FlowConnectionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FlowConnectionConfigurationTypeDef


def get_value() -> FlowConnectionConfigurationTypeDef:
    return {
        "conditional": ...,
    }


# FlowConnectionConfigurationTypeDef definition

class FlowConnectionConfigurationTypeDef(TypedDict):
    conditional: NotRequired[FlowConditionalConnectionConfigurationTypeDef],  # (1)
    data: NotRequired[FlowDataConnectionConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: FlowConditionalConnectionConfigurationTypeDef](./type_defs.md#flowconditionalconnectionconfigurationtypedef)
2. See [:material-code-braces: FlowDataConnectionConfigurationTypeDef](./type_defs.md#flowdataconnectionconfigurationtypedef)

## ListFlowsResponseTypeDef

```python
# ListFlowsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListFlowsResponseTypeDef


def get_value() -> ListFlowsResponseTypeDef:
    return {
        "flowSummaries": ...,
    }


# ListFlowsResponseTypeDef definition

class ListFlowsResponseTypeDef(TypedDict):
    flowSummaries: List[FlowSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `List[FlowSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## FlowValidationDetailsTypeDef

```python
# FlowValidationDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FlowValidationDetailsTypeDef


def get_value() -> FlowValidationDetailsTypeDef:
    return {
        "cyclicConnection": ...,
    }


# FlowValidationDetailsTypeDef definition

class FlowValidationDetailsTypeDef(TypedDict):
    cyclicConnection: NotRequired[CyclicConnectionFlowValidationDetailsTypeDef],  # (1)
    duplicateConditionExpression: NotRequired[DuplicateConditionExpressionFlowValidationDetailsTypeDef],  # (2)
    duplicateConnections: NotRequired[DuplicateConnectionsFlowValidationDetailsTypeDef],  # (3)
    incompatibleConnectionDataType: NotRequired[IncompatibleConnectionDataTypeFlowValidationDetailsTypeDef],  # (4)
    malformedConditionExpression: NotRequired[MalformedConditionExpressionFlowValidationDetailsTypeDef],  # (5)
    malformedNodeInputExpression: NotRequired[MalformedNodeInputExpressionFlowValidationDetailsTypeDef],  # (6)
    mismatchedNodeInputType: NotRequired[MismatchedNodeInputTypeFlowValidationDetailsTypeDef],  # (7)
    mismatchedNodeOutputType: NotRequired[MismatchedNodeOutputTypeFlowValidationDetailsTypeDef],  # (8)
    missingConnectionConfiguration: NotRequired[MissingConnectionConfigurationFlowValidationDetailsTypeDef],  # (9)
    missingDefaultCondition: NotRequired[MissingDefaultConditionFlowValidationDetailsTypeDef],  # (10)
    missingEndingNodes: NotRequired[Dict[str, Any]],
    missingNodeConfiguration: NotRequired[MissingNodeConfigurationFlowValidationDetailsTypeDef],  # (11)
    missingNodeInput: NotRequired[MissingNodeInputFlowValidationDetailsTypeDef],  # (12)
    missingNodeOutput: NotRequired[MissingNodeOutputFlowValidationDetailsTypeDef],  # (13)
    missingStartingNodes: NotRequired[Dict[str, Any]],
    multipleNodeInputConnections: NotRequired[MultipleNodeInputConnectionsFlowValidationDetailsTypeDef],  # (14)
    unfulfilledNodeInput: NotRequired[UnfulfilledNodeInputFlowValidationDetailsTypeDef],  # (15)
    unknownConnectionCondition: NotRequired[UnknownConnectionConditionFlowValidationDetailsTypeDef],  # (16)
    unknownConnectionSource: NotRequired[UnknownConnectionSourceFlowValidationDetailsTypeDef],  # (17)
    unknownConnectionSourceOutput: NotRequired[UnknownConnectionSourceOutputFlowValidationDetailsTypeDef],  # (18)
    unknownConnectionTarget: NotRequired[UnknownConnectionTargetFlowValidationDetailsTypeDef],  # (19)
    unknownConnectionTargetInput: NotRequired[UnknownConnectionTargetInputFlowValidationDetailsTypeDef],  # (20)
    unknownNodeInput: NotRequired[UnknownNodeInputFlowValidationDetailsTypeDef],  # (21)
    unknownNodeOutput: NotRequired[UnknownNodeOutputFlowValidationDetailsTypeDef],  # (22)
    unreachableNode: NotRequired[UnreachableNodeFlowValidationDetailsTypeDef],  # (23)
    unsatisfiedConnectionConditions: NotRequired[UnsatisfiedConnectionConditionsFlowValidationDetailsTypeDef],  # (24)
    unspecified: NotRequired[Dict[str, Any]],
```

1. See [:material-code-braces: CyclicConnectionFlowValidationDetailsTypeDef](./type_defs.md#cyclicconnectionflowvalidationdetailstypedef)
2. See [:material-code-braces: DuplicateConditionExpressionFlowValidationDetailsTypeDef](./type_defs.md#duplicateconditionexpressionflowvalidationdetailstypedef)
3. See [:material-code-braces: DuplicateConnectionsFlowValidationDetailsTypeDef](./type_defs.md#duplicateconnectionsflowvalidationdetailstypedef)
4. See [:material-code-braces: IncompatibleConnectionDataTypeFlowValidationDetailsTypeDef](./type_defs.md#incompatibleconnectiondatatypeflowvalidationdetailstypedef)
5. See [:material-code-braces: MalformedConditionExpressionFlowValidationDetailsTypeDef](./type_defs.md#malformedconditionexpressionflowvalidationdetailstypedef)
6. See [:material-code-braces: MalformedNodeInputExpressionFlowValidationDetailsTypeDef](./type_defs.md#malformednodeinputexpressionflowvalidationdetailstypedef)
7. See [:material-code-braces: MismatchedNodeInputTypeFlowValidationDetailsTypeDef](./type_defs.md#mismatchednodeinputtypeflowvalidationdetailstypedef)
8. See [:material-code-braces: MismatchedNodeOutputTypeFlowValidationDetailsTypeDef](./type_defs.md#mismatchednodeoutputtypeflowvalidationdetailstypedef)
9. See [:material-code-braces: MissingConnectionConfigurationFlowValidationDetailsTypeDef](./type_defs.md#missingconnectionconfigurationflowvalidationdetailstypedef)
10. See [:material-code-braces: MissingDefaultConditionFlowValidationDetailsTypeDef](./type_defs.md#missingdefaultconditionflowvalidationdetailstypedef)
11. See [:material-code-braces: MissingNodeConfigurationFlowValidationDetailsTypeDef](./type_defs.md#missingnodeconfigurationflowvalidationdetailstypedef)
12. See [:material-code-braces: MissingNodeInputFlowValidationDetailsTypeDef](./type_defs.md#missingnodeinputflowvalidationdetailstypedef)
13. See [:material-code-braces: MissingNodeOutputFlowValidationDetailsTypeDef](./type_defs.md#missingnodeoutputflowvalidationdetailstypedef)
14. See [:material-code-braces: MultipleNodeInputConnectionsFlowValidationDetailsTypeDef](./type_defs.md#multiplenodeinputconnectionsflowvalidationdetailstypedef)
15. See [:material-code-braces: UnfulfilledNodeInputFlowValidationDetailsTypeDef](./type_defs.md#unfulfillednodeinputflowvalidationdetailstypedef)
16. See [:material-code-braces: UnknownConnectionConditionFlowValidationDetailsTypeDef](./type_defs.md#unknownconnectionconditionflowvalidationdetailstypedef)
17. See [:material-code-braces: UnknownConnectionSourceFlowValidationDetailsTypeDef](./type_defs.md#unknownconnectionsourceflowvalidationdetailstypedef)
18. See [:material-code-braces: UnknownConnectionSourceOutputFlowValidationDetailsTypeDef](./type_defs.md#unknownconnectionsourceoutputflowvalidationdetailstypedef)
19. See [:material-code-braces: UnknownConnectionTargetFlowValidationDetailsTypeDef](./type_defs.md#unknownconnectiontargetflowvalidationdetailstypedef)
20. See [:material-code-braces: UnknownConnectionTargetInputFlowValidationDetailsTypeDef](./type_defs.md#unknownconnectiontargetinputflowvalidationdetailstypedef)
21. See [:material-code-braces: UnknownNodeInputFlowValidationDetailsTypeDef](./type_defs.md#unknownnodeinputflowvalidationdetailstypedef)
22. See [:material-code-braces: UnknownNodeOutputFlowValidationDetailsTypeDef](./type_defs.md#unknownnodeoutputflowvalidationdetailstypedef)
23. See [:material-code-braces: UnreachableNodeFlowValidationDetailsTypeDef](./type_defs.md#unreachablenodeflowvalidationdetailstypedef)
24. See [:material-code-braces: UnsatisfiedConnectionConditionsFlowValidationDetailsTypeDef](./type_defs.md#unsatisfiedconnectionconditionsflowvalidationdetailstypedef)

## ListFlowVersionsResponseTypeDef

```python
# ListFlowVersionsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListFlowVersionsResponseTypeDef


def get_value() -> ListFlowVersionsResponseTypeDef:
    return {
        "flowVersionSummaries": ...,
    }


# ListFlowVersionsResponseTypeDef definition

class ListFlowVersionsResponseTypeDef(TypedDict):
    flowVersionSummaries: List[FlowVersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `List[FlowVersionSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## FunctionOutputTypeDef

```python
# FunctionOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FunctionOutputTypeDef


def get_value() -> FunctionOutputTypeDef:
    return {
        "description": ...,
    }


# FunctionOutputTypeDef definition

class FunctionOutputTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    parameters: NotRequired[Dict[str, ParameterDetailTypeDef]],  # (1)
    requireConfirmation: NotRequired[RequireConfirmationType],  # (2)
```

1. See `Dict[str, ParameterDetailTypeDef]`
2. See [:material-code-brackets: RequireConfirmationType](./literals.md#requireconfirmationtype)

## FunctionTypeDef

```python
# FunctionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FunctionTypeDef


def get_value() -> FunctionTypeDef:
    return {
        "description": ...,
    }


# FunctionTypeDef definition

class FunctionTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    parameters: NotRequired[Mapping[str, ParameterDetailTypeDef]],  # (1)
    requireConfirmation: NotRequired[RequireConfirmationType],  # (2)
```

1. See `Mapping[str, ParameterDetailTypeDef]`
2. See [:material-code-brackets: RequireConfirmationType](./literals.md#requireconfirmationtype)

## HierarchicalChunkingConfigurationOutputTypeDef

```python
# HierarchicalChunkingConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import HierarchicalChunkingConfigurationOutputTypeDef


def get_value() -> HierarchicalChunkingConfigurationOutputTypeDef:
    return {
        "levelConfigurations": ...,
    }


# HierarchicalChunkingConfigurationOutputTypeDef definition

class HierarchicalChunkingConfigurationOutputTypeDef(TypedDict):
    levelConfigurations: List[HierarchicalChunkingLevelConfigurationTypeDef],  # (1)
    overlapTokens: int,
```

1. See `List[HierarchicalChunkingLevelConfigurationTypeDef]`

## HierarchicalChunkingConfigurationTypeDef

```python
# HierarchicalChunkingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import HierarchicalChunkingConfigurationTypeDef


def get_value() -> HierarchicalChunkingConfigurationTypeDef:
    return {
        "levelConfigurations": ...,
    }


# HierarchicalChunkingConfigurationTypeDef definition

class HierarchicalChunkingConfigurationTypeDef(TypedDict):
    levelConfigurations: Sequence[HierarchicalChunkingLevelConfigurationTypeDef],  # (1)
    overlapTokens: int,
```

1. See `Sequence[HierarchicalChunkingLevelConfigurationTypeDef]`

## PromptConfigurationOutputTypeDef

```python
# PromptConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptConfigurationOutputTypeDef


def get_value() -> PromptConfigurationOutputTypeDef:
    return {
        "additionalModelRequestFields": ...,
    }


# PromptConfigurationOutputTypeDef definition

class PromptConfigurationOutputTypeDef(TypedDict):
    additionalModelRequestFields: NotRequired[Dict[str, Any]],
    basePromptTemplate: NotRequired[str],
    foundationModel: NotRequired[str],
    inferenceConfiguration: NotRequired[InferenceConfigurationOutputTypeDef],  # (1)
    parserMode: NotRequired[CreationModeType],  # (2)
    promptCreationMode: NotRequired[CreationModeType],  # (2)
    promptState: NotRequired[PromptStateType],  # (4)
    promptType: NotRequired[PromptTypeType],  # (5)
```

1. See [:material-code-braces: InferenceConfigurationOutputTypeDef](./type_defs.md#inferenceconfigurationoutputtypedef)
2. See [:material-code-brackets: CreationModeType](./literals.md#creationmodetype)
3. See [:material-code-brackets: CreationModeType](./literals.md#creationmodetype)
4. See [:material-code-brackets: PromptStateType](./literals.md#promptstatetype)
5. See [:material-code-brackets: PromptTypeType](./literals.md#prompttypetype)

## PromptConfigurationTypeDef

```python
# PromptConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptConfigurationTypeDef


def get_value() -> PromptConfigurationTypeDef:
    return {
        "additionalModelRequestFields": ...,
    }


# PromptConfigurationTypeDef definition

class PromptConfigurationTypeDef(TypedDict):
    additionalModelRequestFields: NotRequired[Mapping[str, Any]],
    basePromptTemplate: NotRequired[str],
    foundationModel: NotRequired[str],
    inferenceConfiguration: NotRequired[InferenceConfigurationTypeDef],  # (1)
    parserMode: NotRequired[CreationModeType],  # (2)
    promptCreationMode: NotRequired[CreationModeType],  # (2)
    promptState: NotRequired[PromptStateType],  # (4)
    promptType: NotRequired[PromptTypeType],  # (5)
```

1. See [:material-code-braces: InferenceConfigurationTypeDef](./type_defs.md#inferenceconfigurationtypedef)
2. See [:material-code-brackets: CreationModeType](./literals.md#creationmodetype)
3. See [:material-code-brackets: CreationModeType](./literals.md#creationmodetype)
4. See [:material-code-brackets: PromptStateType](./literals.md#promptstatetype)
5. See [:material-code-brackets: PromptTypeType](./literals.md#prompttypetype)

## ListIngestionJobsRequestTypeDef

```python
# ListIngestionJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListIngestionJobsRequestTypeDef


def get_value() -> ListIngestionJobsRequestTypeDef:
    return {
        "dataSourceId": ...,
    }


# ListIngestionJobsRequestTypeDef definition

class ListIngestionJobsRequestTypeDef(TypedDict):
    dataSourceId: str,
    knowledgeBaseId: str,
    filters: NotRequired[Sequence[IngestionJobFilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortBy: NotRequired[IngestionJobSortByTypeDef],  # (2)
```

1. See `Sequence[IngestionJobFilterTypeDef]`
2. See [:material-code-braces: IngestionJobSortByTypeDef](./type_defs.md#ingestionjobsortbytypedef)

## IngestionJobSummaryTypeDef

```python
# IngestionJobSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import IngestionJobSummaryTypeDef


def get_value() -> IngestionJobSummaryTypeDef:
    return {
        "dataSourceId": ...,
    }


# IngestionJobSummaryTypeDef definition

class IngestionJobSummaryTypeDef(TypedDict):
    dataSourceId: str,
    ingestionJobId: str,
    knowledgeBaseId: str,
    startedAt: datetime.datetime,
    status: IngestionJobStatusType,  # (2)
    updatedAt: datetime.datetime,
    description: NotRequired[str],
    statistics: NotRequired[IngestionJobStatisticsTypeDef],  # (1)
```

1. See [:material-code-braces: IngestionJobStatisticsTypeDef](./type_defs.md#ingestionjobstatisticstypedef)
2. See [:material-code-brackets: IngestionJobStatusType](./literals.md#ingestionjobstatustype)

## IngestionJobTypeDef

```python
# IngestionJobTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import IngestionJobTypeDef


def get_value() -> IngestionJobTypeDef:
    return {
        "dataSourceId": ...,
    }


# IngestionJobTypeDef definition

class IngestionJobTypeDef(TypedDict):
    dataSourceId: str,
    ingestionJobId: str,
    knowledgeBaseId: str,
    startedAt: datetime.datetime,
    status: IngestionJobStatusType,  # (2)
    updatedAt: datetime.datetime,
    description: NotRequired[str],
    failureReasons: NotRequired[List[str]],
    statistics: NotRequired[IngestionJobStatisticsTypeDef],  # (1)
```

1. See [:material-code-braces: IngestionJobStatisticsTypeDef](./type_defs.md#ingestionjobstatisticstypedef)
2. See [:material-code-brackets: IngestionJobStatusType](./literals.md#ingestionjobstatustype)

## ListKnowledgeBasesResponseTypeDef

```python
# ListKnowledgeBasesResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListKnowledgeBasesResponseTypeDef


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

1. See `List[KnowledgeBaseSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListAgentActionGroupsRequestPaginateTypeDef

```python
# ListAgentActionGroupsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListAgentActionGroupsRequestPaginateTypeDef


def get_value() -> ListAgentActionGroupsRequestPaginateTypeDef:
    return {
        "agentId": ...,
    }


# ListAgentActionGroupsRequestPaginateTypeDef definition

class ListAgentActionGroupsRequestPaginateTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListAgentAliasesRequestPaginateTypeDef

```python
# ListAgentAliasesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListAgentAliasesRequestPaginateTypeDef


def get_value() -> ListAgentAliasesRequestPaginateTypeDef:
    return {
        "agentId": ...,
    }


# ListAgentAliasesRequestPaginateTypeDef definition

class ListAgentAliasesRequestPaginateTypeDef(TypedDict):
    agentId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListAgentCollaboratorsRequestPaginateTypeDef

```python
# ListAgentCollaboratorsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListAgentCollaboratorsRequestPaginateTypeDef


def get_value() -> ListAgentCollaboratorsRequestPaginateTypeDef:
    return {
        "agentId": ...,
    }


# ListAgentCollaboratorsRequestPaginateTypeDef definition

class ListAgentCollaboratorsRequestPaginateTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListAgentKnowledgeBasesRequestPaginateTypeDef

```python
# ListAgentKnowledgeBasesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListAgentKnowledgeBasesRequestPaginateTypeDef


def get_value() -> ListAgentKnowledgeBasesRequestPaginateTypeDef:
    return {
        "agentId": ...,
    }


# ListAgentKnowledgeBasesRequestPaginateTypeDef definition

class ListAgentKnowledgeBasesRequestPaginateTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListAgentVersionsRequestPaginateTypeDef

```python
# ListAgentVersionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListAgentVersionsRequestPaginateTypeDef


def get_value() -> ListAgentVersionsRequestPaginateTypeDef:
    return {
        "agentId": ...,
    }


# ListAgentVersionsRequestPaginateTypeDef definition

class ListAgentVersionsRequestPaginateTypeDef(TypedDict):
    agentId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListAgentsRequestPaginateTypeDef

```python
# ListAgentsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListAgentsRequestPaginateTypeDef


def get_value() -> ListAgentsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListAgentsRequestPaginateTypeDef definition

class ListAgentsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListDataSourcesRequestPaginateTypeDef

```python
# ListDataSourcesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListDataSourcesRequestPaginateTypeDef


def get_value() -> ListDataSourcesRequestPaginateTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# ListDataSourcesRequestPaginateTypeDef definition

class ListDataSourcesRequestPaginateTypeDef(TypedDict):
    knowledgeBaseId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListFlowAliasesRequestPaginateTypeDef

```python
# ListFlowAliasesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListFlowAliasesRequestPaginateTypeDef


def get_value() -> ListFlowAliasesRequestPaginateTypeDef:
    return {
        "flowIdentifier": ...,
    }


# ListFlowAliasesRequestPaginateTypeDef definition

class ListFlowAliasesRequestPaginateTypeDef(TypedDict):
    flowIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListFlowVersionsRequestPaginateTypeDef

```python
# ListFlowVersionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListFlowVersionsRequestPaginateTypeDef


def get_value() -> ListFlowVersionsRequestPaginateTypeDef:
    return {
        "flowIdentifier": ...,
    }


# ListFlowVersionsRequestPaginateTypeDef definition

class ListFlowVersionsRequestPaginateTypeDef(TypedDict):
    flowIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListFlowsRequestPaginateTypeDef

```python
# ListFlowsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListFlowsRequestPaginateTypeDef


def get_value() -> ListFlowsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListFlowsRequestPaginateTypeDef definition

class ListFlowsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListIngestionJobsRequestPaginateTypeDef

```python
# ListIngestionJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListIngestionJobsRequestPaginateTypeDef


def get_value() -> ListIngestionJobsRequestPaginateTypeDef:
    return {
        "dataSourceId": ...,
    }


# ListIngestionJobsRequestPaginateTypeDef definition

class ListIngestionJobsRequestPaginateTypeDef(TypedDict):
    dataSourceId: str,
    knowledgeBaseId: str,
    filters: NotRequired[Sequence[IngestionJobFilterTypeDef]],  # (1)
    sortBy: NotRequired[IngestionJobSortByTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See `Sequence[IngestionJobFilterTypeDef]`
2. See [:material-code-braces: IngestionJobSortByTypeDef](./type_defs.md#ingestionjobsortbytypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListKnowledgeBaseDocumentsRequestPaginateTypeDef

```python
# ListKnowledgeBaseDocumentsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListKnowledgeBaseDocumentsRequestPaginateTypeDef


def get_value() -> ListKnowledgeBaseDocumentsRequestPaginateTypeDef:
    return {
        "dataSourceId": ...,
    }


# ListKnowledgeBaseDocumentsRequestPaginateTypeDef definition

class ListKnowledgeBaseDocumentsRequestPaginateTypeDef(TypedDict):
    dataSourceId: str,
    knowledgeBaseId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListKnowledgeBasesRequestPaginateTypeDef

```python
# ListKnowledgeBasesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListKnowledgeBasesRequestPaginateTypeDef


def get_value() -> ListKnowledgeBasesRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListKnowledgeBasesRequestPaginateTypeDef definition

class ListKnowledgeBasesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListPromptsRequestPaginateTypeDef

```python
# ListPromptsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListPromptsRequestPaginateTypeDef


def get_value() -> ListPromptsRequestPaginateTypeDef:
    return {
        "promptIdentifier": ...,
    }


# ListPromptsRequestPaginateTypeDef definition

class ListPromptsRequestPaginateTypeDef(TypedDict):
    promptIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListPromptsResponseTypeDef

```python
# ListPromptsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListPromptsResponseTypeDef


def get_value() -> ListPromptsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListPromptsResponseTypeDef definition

class ListPromptsResponseTypeDef(TypedDict):
    promptSummaries: List[PromptSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `List[PromptSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## MemoryConfigurationOutputTypeDef

```python
# MemoryConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import MemoryConfigurationOutputTypeDef


def get_value() -> MemoryConfigurationOutputTypeDef:
    return {
        "enabledMemoryTypes": ...,
    }


# MemoryConfigurationOutputTypeDef definition

class MemoryConfigurationOutputTypeDef(TypedDict):
    enabledMemoryTypes: List[MemoryTypeType],  # (1)
    sessionSummaryConfiguration: NotRequired[SessionSummaryConfigurationTypeDef],  # (2)
    storageDays: NotRequired[int],
```

1. See `List[Literal['SESSION_SUMMARY']]`
2. See [:material-code-braces: SessionSummaryConfigurationTypeDef](./type_defs.md#sessionsummaryconfigurationtypedef)

## MemoryConfigurationTypeDef

```python
# MemoryConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import MemoryConfigurationTypeDef


def get_value() -> MemoryConfigurationTypeDef:
    return {
        "enabledMemoryTypes": ...,
    }


# MemoryConfigurationTypeDef definition

class MemoryConfigurationTypeDef(TypedDict):
    enabledMemoryTypes: Sequence[MemoryTypeType],  # (1)
    sessionSummaryConfiguration: NotRequired[SessionSummaryConfigurationTypeDef],  # (2)
    storageDays: NotRequired[int],
```

1. See `Sequence[Literal['SESSION_SUMMARY']]`
2. See [:material-code-braces: SessionSummaryConfigurationTypeDef](./type_defs.md#sessionsummaryconfigurationtypedef)

## MetadataAttributeTypeDef

```python
# MetadataAttributeTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import MetadataAttributeTypeDef


def get_value() -> MetadataAttributeTypeDef:
    return {
        "key": ...,
    }


# MetadataAttributeTypeDef definition

class MetadataAttributeTypeDef(TypedDict):
    key: str,
    value: MetadataAttributeValueTypeDef,  # (1)
```

1. See [:material-code-braces: MetadataAttributeValueTypeDef](./type_defs.md#metadataattributevaluetypedef)

## MongoDbAtlasConfigurationTypeDef

```python
# MongoDbAtlasConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import MongoDbAtlasConfigurationTypeDef


def get_value() -> MongoDbAtlasConfigurationTypeDef:
    return {
        "collectionName": ...,
    }


# MongoDbAtlasConfigurationTypeDef definition

class MongoDbAtlasConfigurationTypeDef(TypedDict):
    collectionName: str,
    credentialsSecretArn: str,
    databaseName: str,
    endpoint: str,
    fieldMapping: MongoDbAtlasFieldMappingTypeDef,  # (1)
    vectorIndexName: str,
    endpointServiceName: NotRequired[str],
```

1. See [:material-code-braces: MongoDbAtlasFieldMappingTypeDef](./type_defs.md#mongodbatlasfieldmappingtypedef)

## OpenSearchServerlessConfigurationTypeDef

```python
# OpenSearchServerlessConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import OpenSearchServerlessConfigurationTypeDef


def get_value() -> OpenSearchServerlessConfigurationTypeDef:
    return {
        "collectionArn": ...,
    }


# OpenSearchServerlessConfigurationTypeDef definition

class OpenSearchServerlessConfigurationTypeDef(TypedDict):
    collectionArn: str,
    fieldMapping: OpenSearchServerlessFieldMappingTypeDef,  # (1)
    vectorIndexName: str,
```

1. See [:material-code-braces: OpenSearchServerlessFieldMappingTypeDef](./type_defs.md#opensearchserverlessfieldmappingtypedef)

## PatternObjectFilterConfigurationOutputTypeDef

```python
# PatternObjectFilterConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PatternObjectFilterConfigurationOutputTypeDef


def get_value() -> PatternObjectFilterConfigurationOutputTypeDef:
    return {
        "filters": ...,
    }


# PatternObjectFilterConfigurationOutputTypeDef definition

class PatternObjectFilterConfigurationOutputTypeDef(TypedDict):
    filters: List[PatternObjectFilterOutputTypeDef],  # (1)
```

1. See `List[PatternObjectFilterOutputTypeDef]`

## PatternObjectFilterConfigurationTypeDef

```python
# PatternObjectFilterConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PatternObjectFilterConfigurationTypeDef


def get_value() -> PatternObjectFilterConfigurationTypeDef:
    return {
        "filters": ...,
    }


# PatternObjectFilterConfigurationTypeDef definition

class PatternObjectFilterConfigurationTypeDef(TypedDict):
    filters: Sequence[PatternObjectFilterTypeDef],  # (1)
```

1. See `Sequence[PatternObjectFilterTypeDef]`

## PineconeConfigurationTypeDef

```python
# PineconeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PineconeConfigurationTypeDef


def get_value() -> PineconeConfigurationTypeDef:
    return {
        "connectionString": ...,
    }


# PineconeConfigurationTypeDef definition

class PineconeConfigurationTypeDef(TypedDict):
    connectionString: str,
    credentialsSecretArn: str,
    fieldMapping: PineconeFieldMappingTypeDef,  # (1)
    namespace: NotRequired[str],
```

1. See [:material-code-braces: PineconeFieldMappingTypeDef](./type_defs.md#pineconefieldmappingtypedef)

## PromptGenAiResourceTypeDef

```python
# PromptGenAiResourceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptGenAiResourceTypeDef


def get_value() -> PromptGenAiResourceTypeDef:
    return {
        "agent": ...,
    }


# PromptGenAiResourceTypeDef definition

class PromptGenAiResourceTypeDef(TypedDict):
    agent: NotRequired[PromptAgentResourceTypeDef],  # (1)
```

1. See [:material-code-braces: PromptAgentResourceTypeDef](./type_defs.md#promptagentresourcetypedef)

## PromptInferenceConfigurationOutputTypeDef

```python
# PromptInferenceConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptInferenceConfigurationOutputTypeDef


def get_value() -> PromptInferenceConfigurationOutputTypeDef:
    return {
        "text": ...,
    }


# PromptInferenceConfigurationOutputTypeDef definition

class PromptInferenceConfigurationOutputTypeDef(TypedDict):
    text: NotRequired[PromptModelInferenceConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: PromptModelInferenceConfigurationOutputTypeDef](./type_defs.md#promptmodelinferenceconfigurationoutputtypedef)

## QueryGenerationTableOutputTypeDef

```python
# QueryGenerationTableOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import QueryGenerationTableOutputTypeDef


def get_value() -> QueryGenerationTableOutputTypeDef:
    return {
        "columns": ...,
    }


# QueryGenerationTableOutputTypeDef definition

class QueryGenerationTableOutputTypeDef(TypedDict):
    name: str,
    columns: NotRequired[List[QueryGenerationColumnTypeDef]],  # (1)
    description: NotRequired[str],
    inclusion: NotRequired[IncludeExcludeType],  # (2)
```

1. See `List[QueryGenerationColumnTypeDef]`
2. See [:material-code-brackets: IncludeExcludeType](./literals.md#includeexcludetype)

## QueryGenerationTableTypeDef

```python
# QueryGenerationTableTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import QueryGenerationTableTypeDef


def get_value() -> QueryGenerationTableTypeDef:
    return {
        "columns": ...,
    }


# QueryGenerationTableTypeDef definition

class QueryGenerationTableTypeDef(TypedDict):
    name: str,
    columns: NotRequired[Sequence[QueryGenerationColumnTypeDef]],  # (1)
    description: NotRequired[str],
    inclusion: NotRequired[IncludeExcludeType],  # (2)
```

1. See `Sequence[QueryGenerationColumnTypeDef]`
2. See [:material-code-brackets: IncludeExcludeType](./literals.md#includeexcludetype)

## RdsConfigurationTypeDef

```python
# RdsConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import RdsConfigurationTypeDef


def get_value() -> RdsConfigurationTypeDef:
    return {
        "credentialsSecretArn": ...,
    }


# RdsConfigurationTypeDef definition

class RdsConfigurationTypeDef(TypedDict):
    credentialsSecretArn: str,
    databaseName: str,
    fieldMapping: RdsFieldMappingTypeDef,  # (1)
    resourceArn: str,
    tableName: str,
```

1. See [:material-code-braces: RdsFieldMappingTypeDef](./type_defs.md#rdsfieldmappingtypedef)

## RedisEnterpriseCloudConfigurationTypeDef

```python
# RedisEnterpriseCloudConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import RedisEnterpriseCloudConfigurationTypeDef


def get_value() -> RedisEnterpriseCloudConfigurationTypeDef:
    return {
        "credentialsSecretArn": ...,
    }


# RedisEnterpriseCloudConfigurationTypeDef definition

class RedisEnterpriseCloudConfigurationTypeDef(TypedDict):
    credentialsSecretArn: str,
    endpoint: str,
    fieldMapping: RedisEnterpriseCloudFieldMappingTypeDef,  # (1)
    vectorIndexName: str,
```

1. See [:material-code-braces: RedisEnterpriseCloudFieldMappingTypeDef](./type_defs.md#redisenterprisecloudfieldmappingtypedef)

## RedshiftProvisionedConfigurationTypeDef

```python
# RedshiftProvisionedConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import RedshiftProvisionedConfigurationTypeDef


def get_value() -> RedshiftProvisionedConfigurationTypeDef:
    return {
        "authConfiguration": ...,
    }


# RedshiftProvisionedConfigurationTypeDef definition

class RedshiftProvisionedConfigurationTypeDef(TypedDict):
    authConfiguration: RedshiftProvisionedAuthConfigurationTypeDef,  # (1)
    clusterIdentifier: str,
```

1. See [:material-code-braces: RedshiftProvisionedAuthConfigurationTypeDef](./type_defs.md#redshiftprovisionedauthconfigurationtypedef)

## RedshiftQueryEngineStorageConfigurationOutputTypeDef

```python
# RedshiftQueryEngineStorageConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import RedshiftQueryEngineStorageConfigurationOutputTypeDef


def get_value() -> RedshiftQueryEngineStorageConfigurationOutputTypeDef:
    return {
        "awsDataCatalogConfiguration": ...,
    }


# RedshiftQueryEngineStorageConfigurationOutputTypeDef definition

class RedshiftQueryEngineStorageConfigurationOutputTypeDef(TypedDict):
    type: RedshiftQueryEngineStorageTypeType,  # (3)
    awsDataCatalogConfiguration: NotRequired[RedshiftQueryEngineAwsDataCatalogStorageConfigurationOutputTypeDef],  # (1)
    redshiftConfiguration: NotRequired[RedshiftQueryEngineRedshiftStorageConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: RedshiftQueryEngineAwsDataCatalogStorageConfigurationOutputTypeDef](./type_defs.md#redshiftqueryengineawsdatacatalogstorageconfigurationoutputtypedef)
2. See [:material-code-braces: RedshiftQueryEngineRedshiftStorageConfigurationTypeDef](./type_defs.md#redshiftqueryengineredshiftstorageconfigurationtypedef)
3. See [:material-code-brackets: RedshiftQueryEngineStorageTypeType](./literals.md#redshiftqueryenginestoragetypetype)

## RedshiftQueryEngineStorageConfigurationTypeDef

```python
# RedshiftQueryEngineStorageConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import RedshiftQueryEngineStorageConfigurationTypeDef


def get_value() -> RedshiftQueryEngineStorageConfigurationTypeDef:
    return {
        "awsDataCatalogConfiguration": ...,
    }


# RedshiftQueryEngineStorageConfigurationTypeDef definition

class RedshiftQueryEngineStorageConfigurationTypeDef(TypedDict):
    type: RedshiftQueryEngineStorageTypeType,  # (3)
    awsDataCatalogConfiguration: NotRequired[RedshiftQueryEngineAwsDataCatalogStorageConfigurationTypeDef],  # (1)
    redshiftConfiguration: NotRequired[RedshiftQueryEngineRedshiftStorageConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: RedshiftQueryEngineAwsDataCatalogStorageConfigurationTypeDef](./type_defs.md#redshiftqueryengineawsdatacatalogstorageconfigurationtypedef)
2. See [:material-code-braces: RedshiftQueryEngineRedshiftStorageConfigurationTypeDef](./type_defs.md#redshiftqueryengineredshiftstorageconfigurationtypedef)
3. See [:material-code-brackets: RedshiftQueryEngineStorageTypeType](./literals.md#redshiftqueryenginestoragetypetype)

## RedshiftServerlessConfigurationTypeDef

```python
# RedshiftServerlessConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import RedshiftServerlessConfigurationTypeDef


def get_value() -> RedshiftServerlessConfigurationTypeDef:
    return {
        "authConfiguration": ...,
    }


# RedshiftServerlessConfigurationTypeDef definition

class RedshiftServerlessConfigurationTypeDef(TypedDict):
    authConfiguration: RedshiftServerlessAuthConfigurationTypeDef,  # (1)
    workgroupArn: str,
```

1. See [:material-code-braces: RedshiftServerlessAuthConfigurationTypeDef](./type_defs.md#redshiftserverlessauthconfigurationtypedef)

## RetrievalFlowNodeServiceConfigurationTypeDef

```python
# RetrievalFlowNodeServiceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import RetrievalFlowNodeServiceConfigurationTypeDef


def get_value() -> RetrievalFlowNodeServiceConfigurationTypeDef:
    return {
        "s3": ...,
    }


# RetrievalFlowNodeServiceConfigurationTypeDef definition

class RetrievalFlowNodeServiceConfigurationTypeDef(TypedDict):
    s3: NotRequired[RetrievalFlowNodeS3ConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: RetrievalFlowNodeS3ConfigurationTypeDef](./type_defs.md#retrievalflownodes3configurationtypedef)

## UrlConfigurationOutputTypeDef

```python
# UrlConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UrlConfigurationOutputTypeDef


def get_value() -> UrlConfigurationOutputTypeDef:
    return {
        "seedUrls": ...,
    }


# UrlConfigurationOutputTypeDef definition

class UrlConfigurationOutputTypeDef(TypedDict):
    seedUrls: NotRequired[List[SeedUrlTypeDef]],  # (1)
```

1. See `List[SeedUrlTypeDef]`

## UrlConfigurationTypeDef

```python
# UrlConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UrlConfigurationTypeDef


def get_value() -> UrlConfigurationTypeDef:
    return {
        "seedUrls": ...,
    }


# UrlConfigurationTypeDef definition

class UrlConfigurationTypeDef(TypedDict):
    seedUrls: NotRequired[Sequence[SeedUrlTypeDef]],  # (1)
```

1. See `Sequence[SeedUrlTypeDef]`

## ToolChoiceOutputTypeDef

```python
# ToolChoiceOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ToolChoiceOutputTypeDef


def get_value() -> ToolChoiceOutputTypeDef:
    return {
        "any": ...,
    }


# ToolChoiceOutputTypeDef definition

class ToolChoiceOutputTypeDef(TypedDict):
    any: NotRequired[Dict[str, Any]],
    auto: NotRequired[Dict[str, Any]],
    tool: NotRequired[SpecificToolChoiceTypeDef],  # (1)
```

1. See [:material-code-braces: SpecificToolChoiceTypeDef](./type_defs.md#specifictoolchoicetypedef)

## ToolChoiceTypeDef

```python
# ToolChoiceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ToolChoiceTypeDef


def get_value() -> ToolChoiceTypeDef:
    return {
        "any": ...,
    }


# ToolChoiceTypeDef definition

class ToolChoiceTypeDef(TypedDict):
    any: NotRequired[Mapping[str, Any]],
    auto: NotRequired[Mapping[str, Any]],
    tool: NotRequired[SpecificToolChoiceTypeDef],  # (1)
```

1. See [:material-code-braces: SpecificToolChoiceTypeDef](./type_defs.md#specifictoolchoicetypedef)

## StorageFlowNodeServiceConfigurationTypeDef

```python
# StorageFlowNodeServiceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import StorageFlowNodeServiceConfigurationTypeDef


def get_value() -> StorageFlowNodeServiceConfigurationTypeDef:
    return {
        "s3": ...,
    }


# StorageFlowNodeServiceConfigurationTypeDef definition

class StorageFlowNodeServiceConfigurationTypeDef(TypedDict):
    s3: NotRequired[StorageFlowNodeS3ConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: StorageFlowNodeS3ConfigurationTypeDef](./type_defs.md#storageflownodes3configurationtypedef)

## ToolSpecificationOutputTypeDef

```python
# ToolSpecificationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ToolSpecificationOutputTypeDef


def get_value() -> ToolSpecificationOutputTypeDef:
    return {
        "description": ...,
    }


# ToolSpecificationOutputTypeDef definition

class ToolSpecificationOutputTypeDef(TypedDict):
    inputSchema: ToolInputSchemaOutputTypeDef,  # (1)
    name: str,
    description: NotRequired[str],
```

1. See [:material-code-braces: ToolInputSchemaOutputTypeDef](./type_defs.md#toolinputschemaoutputtypedef)

## TransformationFunctionTypeDef

```python
# TransformationFunctionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import TransformationFunctionTypeDef


def get_value() -> TransformationFunctionTypeDef:
    return {
        "transformationLambdaConfiguration": ...,
    }


# TransformationFunctionTypeDef definition

class TransformationFunctionTypeDef(TypedDict):
    transformationLambdaConfiguration: TransformationLambdaConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: TransformationLambdaConfigurationTypeDef](./type_defs.md#transformationlambdaconfigurationtypedef)

## WebCrawlerConfigurationOutputTypeDef

```python
# WebCrawlerConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import WebCrawlerConfigurationOutputTypeDef


def get_value() -> WebCrawlerConfigurationOutputTypeDef:
    return {
        "crawlerLimits": ...,
    }


# WebCrawlerConfigurationOutputTypeDef definition

class WebCrawlerConfigurationOutputTypeDef(TypedDict):
    crawlerLimits: NotRequired[WebCrawlerLimitsTypeDef],  # (1)
    exclusionFilters: NotRequired[List[str]],
    inclusionFilters: NotRequired[List[str]],
    scope: NotRequired[WebScopeTypeType],  # (2)
    userAgent: NotRequired[str],
    userAgentHeader: NotRequired[str],
```

1. See [:material-code-braces: WebCrawlerLimitsTypeDef](./type_defs.md#webcrawlerlimitstypedef)
2. See [:material-code-brackets: WebScopeTypeType](./literals.md#webscopetypetype)

## WebCrawlerConfigurationTypeDef

```python
# WebCrawlerConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import WebCrawlerConfigurationTypeDef


def get_value() -> WebCrawlerConfigurationTypeDef:
    return {
        "crawlerLimits": ...,
    }


# WebCrawlerConfigurationTypeDef definition

class WebCrawlerConfigurationTypeDef(TypedDict):
    crawlerLimits: NotRequired[WebCrawlerLimitsTypeDef],  # (1)
    exclusionFilters: NotRequired[Sequence[str]],
    inclusionFilters: NotRequired[Sequence[str]],
    scope: NotRequired[WebScopeTypeType],  # (2)
    userAgent: NotRequired[str],
    userAgentHeader: NotRequired[str],
```

1. See [:material-code-braces: WebCrawlerLimitsTypeDef](./type_defs.md#webcrawlerlimitstypedef)
2. See [:material-code-brackets: WebScopeTypeType](./literals.md#webscopetypetype)

## AgentAliasTypeDef

```python
# AgentAliasTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import AgentAliasTypeDef


def get_value() -> AgentAliasTypeDef:
    return {
        "agentAliasArn": ...,
    }


# AgentAliasTypeDef definition

class AgentAliasTypeDef(TypedDict):
    agentAliasArn: str,
    agentAliasId: str,
    agentAliasName: str,
    agentAliasStatus: AgentAliasStatusType,  # (2)
    agentId: str,
    createdAt: datetime.datetime,
    routingConfiguration: List[AgentAliasRoutingConfigurationListItemTypeDef],  # (3)
    updatedAt: datetime.datetime,
    agentAliasHistoryEvents: NotRequired[List[AgentAliasHistoryEventTypeDef]],  # (1)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    failureReasons: NotRequired[List[str]],
```

1. See `List[AgentAliasHistoryEventTypeDef]`
2. See [:material-code-brackets: AgentAliasStatusType](./literals.md#agentaliasstatustype)
3. See `List[AgentAliasRoutingConfigurationListItemTypeDef]`

## ListAgentAliasesResponseTypeDef

```python
# ListAgentAliasesResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListAgentAliasesResponseTypeDef


def get_value() -> ListAgentAliasesResponseTypeDef:
    return {
        "agentAliasSummaries": ...,
    }


# ListAgentAliasesResponseTypeDef definition

class ListAgentAliasesResponseTypeDef(TypedDict):
    agentAliasSummaries: List[AgentAliasSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `List[AgentAliasSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListAgentCollaboratorsResponseTypeDef

```python
# ListAgentCollaboratorsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListAgentCollaboratorsResponseTypeDef


def get_value() -> ListAgentCollaboratorsResponseTypeDef:
    return {
        "agentCollaboratorSummaries": ...,
    }


# ListAgentCollaboratorsResponseTypeDef definition

class ListAgentCollaboratorsResponseTypeDef(TypedDict):
    agentCollaboratorSummaries: List[AgentCollaboratorSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `List[AgentCollaboratorSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## AssociateAgentCollaboratorResponseTypeDef

```python
# AssociateAgentCollaboratorResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import AssociateAgentCollaboratorResponseTypeDef


def get_value() -> AssociateAgentCollaboratorResponseTypeDef:
    return {
        "agentCollaborator": ...,
    }


# AssociateAgentCollaboratorResponseTypeDef definition

class AssociateAgentCollaboratorResponseTypeDef(TypedDict):
    agentCollaborator: AgentCollaboratorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentCollaboratorTypeDef](./type_defs.md#agentcollaboratortypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetAgentCollaboratorResponseTypeDef

```python
# GetAgentCollaboratorResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetAgentCollaboratorResponseTypeDef


def get_value() -> GetAgentCollaboratorResponseTypeDef:
    return {
        "agentCollaborator": ...,
    }


# GetAgentCollaboratorResponseTypeDef definition

class GetAgentCollaboratorResponseTypeDef(TypedDict):
    agentCollaborator: AgentCollaboratorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentCollaboratorTypeDef](./type_defs.md#agentcollaboratortypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateAgentCollaboratorResponseTypeDef

```python
# UpdateAgentCollaboratorResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UpdateAgentCollaboratorResponseTypeDef


def get_value() -> UpdateAgentCollaboratorResponseTypeDef:
    return {
        "agentCollaborator": ...,
    }


# UpdateAgentCollaboratorResponseTypeDef definition

class UpdateAgentCollaboratorResponseTypeDef(TypedDict):
    agentCollaborator: AgentCollaboratorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentCollaboratorTypeDef](./type_defs.md#agentcollaboratortypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListAgentsResponseTypeDef

```python
# ListAgentsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListAgentsResponseTypeDef


def get_value() -> ListAgentsResponseTypeDef:
    return {
        "agentSummaries": ...,
    }


# ListAgentsResponseTypeDef definition

class ListAgentsResponseTypeDef(TypedDict):
    agentSummaries: List[AgentSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `List[AgentSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListAgentVersionsResponseTypeDef

```python
# ListAgentVersionsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListAgentVersionsResponseTypeDef


def get_value() -> ListAgentVersionsResponseTypeDef:
    return {
        "agentVersionSummaries": ...,
    }


# ListAgentVersionsResponseTypeDef definition

class ListAgentVersionsResponseTypeDef(TypedDict):
    agentVersionSummaries: List[AgentVersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `List[AgentVersionSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ParsingConfigurationTypeDef

```python
# ParsingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ParsingConfigurationTypeDef


def get_value() -> ParsingConfigurationTypeDef:
    return {
        "bedrockDataAutomationConfiguration": ...,
    }


# ParsingConfigurationTypeDef definition

class ParsingConfigurationTypeDef(TypedDict):
    parsingStrategy: ParsingStrategyType,  # (3)
    bedrockDataAutomationConfiguration: NotRequired[BedrockDataAutomationConfigurationTypeDef],  # (1)
    bedrockFoundationModelConfiguration: NotRequired[BedrockFoundationModelConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: BedrockDataAutomationConfigurationTypeDef](./type_defs.md#bedrockdataautomationconfigurationtypedef)
2. See [:material-code-braces: BedrockFoundationModelConfigurationTypeDef](./type_defs.md#bedrockfoundationmodelconfigurationtypedef)
3. See [:material-code-brackets: ParsingStrategyType](./literals.md#parsingstrategytype)

## InlineContentTypeDef

```python
# InlineContentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import InlineContentTypeDef


def get_value() -> InlineContentTypeDef:
    return {
        "byteContent": ...,
    }


# InlineContentTypeDef definition

class InlineContentTypeDef(TypedDict):
    type: InlineContentTypeType,  # (3)
    byteContent: NotRequired[ByteContentDocTypeDef],  # (1)
    textContent: NotRequired[TextContentDocTypeDef],  # (2)
```

1. See [:material-code-braces: ByteContentDocTypeDef](./type_defs.md#bytecontentdoctypedef)
2. See [:material-code-braces: TextContentDocTypeDef](./type_defs.md#textcontentdoctypedef)
3. See [:material-code-brackets: InlineContentTypeType](./literals.md#inlinecontenttypetype)

## MessageOutputTypeDef

```python
# MessageOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import MessageOutputTypeDef


def get_value() -> MessageOutputTypeDef:
    return {
        "content": ...,
    }


# MessageOutputTypeDef definition

class MessageOutputTypeDef(TypedDict):
    content: List[ContentBlockTypeDef],  # (1)
    role: ConversationRoleType,  # (2)
```

1. See `List[ContentBlockTypeDef]`
2. See [:material-code-brackets: ConversationRoleType](./literals.md#conversationroletype)

## MessageTypeDef

```python
# MessageTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import MessageTypeDef


def get_value() -> MessageTypeDef:
    return {
        "content": ...,
    }


# MessageTypeDef definition

class MessageTypeDef(TypedDict):
    content: Sequence[ContentBlockTypeDef],  # (1)
    role: ConversationRoleType,  # (2)
```

1. See `Sequence[ContentBlockTypeDef]`
2. See [:material-code-brackets: ConversationRoleType](./literals.md#conversationroletype)

## ListFlowAliasesResponseTypeDef

```python
# ListFlowAliasesResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListFlowAliasesResponseTypeDef


def get_value() -> ListFlowAliasesResponseTypeDef:
    return {
        "flowAliasSummaries": ...,
    }


# ListFlowAliasesResponseTypeDef definition

class ListFlowAliasesResponseTypeDef(TypedDict):
    flowAliasSummaries: List[FlowAliasSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `List[FlowAliasSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeleteKnowledgeBaseDocumentsRequestTypeDef

```python
# DeleteKnowledgeBaseDocumentsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DeleteKnowledgeBaseDocumentsRequestTypeDef


def get_value() -> DeleteKnowledgeBaseDocumentsRequestTypeDef:
    return {
        "dataSourceId": ...,
    }


# DeleteKnowledgeBaseDocumentsRequestTypeDef definition

class DeleteKnowledgeBaseDocumentsRequestTypeDef(TypedDict):
    dataSourceId: str,
    documentIdentifiers: Sequence[DocumentIdentifierTypeDef],  # (1)
    knowledgeBaseId: str,
    clientToken: NotRequired[str],
```

1. See `Sequence[DocumentIdentifierTypeDef]`

## GetKnowledgeBaseDocumentsRequestTypeDef

```python
# GetKnowledgeBaseDocumentsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetKnowledgeBaseDocumentsRequestTypeDef


def get_value() -> GetKnowledgeBaseDocumentsRequestTypeDef:
    return {
        "dataSourceId": ...,
    }


# GetKnowledgeBaseDocumentsRequestTypeDef definition

class GetKnowledgeBaseDocumentsRequestTypeDef(TypedDict):
    dataSourceId: str,
    documentIdentifiers: Sequence[DocumentIdentifierTypeDef],  # (1)
    knowledgeBaseId: str,
```

1. See `Sequence[DocumentIdentifierTypeDef]`

## KnowledgeBaseDocumentDetailTypeDef

```python
# KnowledgeBaseDocumentDetailTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import KnowledgeBaseDocumentDetailTypeDef


def get_value() -> KnowledgeBaseDocumentDetailTypeDef:
    return {
        "dataSourceId": ...,
    }


# KnowledgeBaseDocumentDetailTypeDef definition

class KnowledgeBaseDocumentDetailTypeDef(TypedDict):
    dataSourceId: str,
    identifier: DocumentIdentifierTypeDef,  # (1)
    knowledgeBaseId: str,
    status: DocumentStatusType,  # (2)
    statusReason: NotRequired[str],
    updatedAt: NotRequired[datetime.datetime],
```

1. See [:material-code-braces: DocumentIdentifierTypeDef](./type_defs.md#documentidentifiertypedef)
2. See [:material-code-brackets: DocumentStatusType](./literals.md#documentstatustype)

## SupplementalDataStorageConfigurationOutputTypeDef

```python
# SupplementalDataStorageConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import SupplementalDataStorageConfigurationOutputTypeDef


def get_value() -> SupplementalDataStorageConfigurationOutputTypeDef:
    return {
        "storageLocations": ...,
    }


# SupplementalDataStorageConfigurationOutputTypeDef definition

class SupplementalDataStorageConfigurationOutputTypeDef(TypedDict):
    storageLocations: List[SupplementalDataStorageLocationTypeDef],  # (1)
```

1. See `List[SupplementalDataStorageLocationTypeDef]`

## SupplementalDataStorageConfigurationTypeDef

```python
# SupplementalDataStorageConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import SupplementalDataStorageConfigurationTypeDef


def get_value() -> SupplementalDataStorageConfigurationTypeDef:
    return {
        "storageLocations": ...,
    }


# SupplementalDataStorageConfigurationTypeDef definition

class SupplementalDataStorageConfigurationTypeDef(TypedDict):
    storageLocations: Sequence[SupplementalDataStorageLocationTypeDef],  # (1)
```

1. See `Sequence[SupplementalDataStorageLocationTypeDef]`

## FlowConnectionTypeDef

```python
# FlowConnectionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FlowConnectionTypeDef


def get_value() -> FlowConnectionTypeDef:
    return {
        "configuration": ...,
    }


# FlowConnectionTypeDef definition

class FlowConnectionTypeDef(TypedDict):
    name: str,
    source: str,
    target: str,
    type: FlowConnectionTypeType,  # (2)
    configuration: NotRequired[FlowConnectionConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: FlowConnectionConfigurationTypeDef](./type_defs.md#flowconnectionconfigurationtypedef)
2. See [:material-code-brackets: FlowConnectionTypeType](./literals.md#flowconnectiontypetype)

## FlowValidationTypeDef

```python
# FlowValidationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FlowValidationTypeDef


def get_value() -> FlowValidationTypeDef:
    return {
        "details": ...,
    }


# FlowValidationTypeDef definition

class FlowValidationTypeDef(TypedDict):
    message: str,
    severity: FlowValidationSeverityType,  # (2)
    details: NotRequired[FlowValidationDetailsTypeDef],  # (1)
    type: NotRequired[FlowValidationTypeType],  # (3)
```

1. See [:material-code-braces: FlowValidationDetailsTypeDef](./type_defs.md#flowvalidationdetailstypedef)
2. See [:material-code-brackets: FlowValidationSeverityType](./literals.md#flowvalidationseveritytype)
3. See [:material-code-brackets: FlowValidationTypeType](./literals.md#flowvalidationtypetype)

## FunctionSchemaOutputTypeDef

```python
# FunctionSchemaOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FunctionSchemaOutputTypeDef


def get_value() -> FunctionSchemaOutputTypeDef:
    return {
        "functions": ...,
    }


# FunctionSchemaOutputTypeDef definition

class FunctionSchemaOutputTypeDef(TypedDict):
    functions: NotRequired[List[FunctionOutputTypeDef]],  # (1)
```

1. See `List[FunctionOutputTypeDef]`

## FunctionSchemaTypeDef

```python
# FunctionSchemaTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FunctionSchemaTypeDef


def get_value() -> FunctionSchemaTypeDef:
    return {
        "functions": ...,
    }


# FunctionSchemaTypeDef definition

class FunctionSchemaTypeDef(TypedDict):
    functions: NotRequired[Sequence[FunctionTypeDef]],  # (1)
```

1. See `Sequence[FunctionTypeDef]`

## ChunkingConfigurationOutputTypeDef

```python
# ChunkingConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ChunkingConfigurationOutputTypeDef


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

from types_aiobotocore_bedrock_agent.type_defs import ChunkingConfigurationTypeDef


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

## PromptOverrideConfigurationOutputTypeDef

```python
# PromptOverrideConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptOverrideConfigurationOutputTypeDef


def get_value() -> PromptOverrideConfigurationOutputTypeDef:
    return {
        "overrideLambda": ...,
    }


# PromptOverrideConfigurationOutputTypeDef definition

class PromptOverrideConfigurationOutputTypeDef(TypedDict):
    promptConfigurations: List[PromptConfigurationOutputTypeDef],  # (1)
    overrideLambda: NotRequired[str],
```

1. See `List[PromptConfigurationOutputTypeDef]`

## PromptOverrideConfigurationTypeDef

```python
# PromptOverrideConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptOverrideConfigurationTypeDef


def get_value() -> PromptOverrideConfigurationTypeDef:
    return {
        "overrideLambda": ...,
    }


# PromptOverrideConfigurationTypeDef definition

class PromptOverrideConfigurationTypeDef(TypedDict):
    promptConfigurations: Sequence[PromptConfigurationTypeDef],  # (1)
    overrideLambda: NotRequired[str],
```

1. See `Sequence[PromptConfigurationTypeDef]`

## ListIngestionJobsResponseTypeDef

```python
# ListIngestionJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListIngestionJobsResponseTypeDef


def get_value() -> ListIngestionJobsResponseTypeDef:
    return {
        "ingestionJobSummaries": ...,
    }


# ListIngestionJobsResponseTypeDef definition

class ListIngestionJobsResponseTypeDef(TypedDict):
    ingestionJobSummaries: List[IngestionJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `List[IngestionJobSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetIngestionJobResponseTypeDef

```python
# GetIngestionJobResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetIngestionJobResponseTypeDef


def get_value() -> GetIngestionJobResponseTypeDef:
    return {
        "ingestionJob": ...,
    }


# GetIngestionJobResponseTypeDef definition

class GetIngestionJobResponseTypeDef(TypedDict):
    ingestionJob: IngestionJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestionJobTypeDef](./type_defs.md#ingestionjobtypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## StartIngestionJobResponseTypeDef

```python
# StartIngestionJobResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import StartIngestionJobResponseTypeDef


def get_value() -> StartIngestionJobResponseTypeDef:
    return {
        "ingestionJob": ...,
    }


# StartIngestionJobResponseTypeDef definition

class StartIngestionJobResponseTypeDef(TypedDict):
    ingestionJob: IngestionJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestionJobTypeDef](./type_defs.md#ingestionjobtypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## StopIngestionJobResponseTypeDef

```python
# StopIngestionJobResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import StopIngestionJobResponseTypeDef


def get_value() -> StopIngestionJobResponseTypeDef:
    return {
        "ingestionJob": ...,
    }


# StopIngestionJobResponseTypeDef definition

class StopIngestionJobResponseTypeDef(TypedDict):
    ingestionJob: IngestionJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestionJobTypeDef](./type_defs.md#ingestionjobtypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DocumentMetadataTypeDef

```python
# DocumentMetadataTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DocumentMetadataTypeDef


def get_value() -> DocumentMetadataTypeDef:
    return {
        "inlineAttributes": ...,
    }


# DocumentMetadataTypeDef definition

class DocumentMetadataTypeDef(TypedDict):
    type: MetadataSourceTypeType,  # (3)
    inlineAttributes: NotRequired[Sequence[MetadataAttributeTypeDef]],  # (1)
    s3Location: NotRequired[CustomS3LocationTypeDef],  # (2)
```

1. See `Sequence[MetadataAttributeTypeDef]`
2. See [:material-code-braces: CustomS3LocationTypeDef](./type_defs.md#customs3locationtypedef)
3. See [:material-code-brackets: MetadataSourceTypeType](./literals.md#metadatasourcetypetype)

## CrawlFilterConfigurationOutputTypeDef

```python
# CrawlFilterConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CrawlFilterConfigurationOutputTypeDef


def get_value() -> CrawlFilterConfigurationOutputTypeDef:
    return {
        "patternObjectFilter": ...,
    }


# CrawlFilterConfigurationOutputTypeDef definition

class CrawlFilterConfigurationOutputTypeDef(TypedDict):
    type: CrawlFilterConfigurationTypeType,  # (2)
    patternObjectFilter: NotRequired[PatternObjectFilterConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: PatternObjectFilterConfigurationOutputTypeDef](./type_defs.md#patternobjectfilterconfigurationoutputtypedef)
2. See [:material-code-brackets: CrawlFilterConfigurationTypeType](./literals.md#crawlfilterconfigurationtypetype)

## CrawlFilterConfigurationTypeDef

```python
# CrawlFilterConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CrawlFilterConfigurationTypeDef


def get_value() -> CrawlFilterConfigurationTypeDef:
    return {
        "patternObjectFilter": ...,
    }


# CrawlFilterConfigurationTypeDef definition

class CrawlFilterConfigurationTypeDef(TypedDict):
    type: CrawlFilterConfigurationTypeType,  # (2)
    patternObjectFilter: NotRequired[PatternObjectFilterConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: PatternObjectFilterConfigurationTypeDef](./type_defs.md#patternobjectfilterconfigurationtypedef)
2. See [:material-code-brackets: CrawlFilterConfigurationTypeType](./literals.md#crawlfilterconfigurationtypetype)

## PromptInferenceConfigurationTypeDef

```python
# PromptInferenceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptInferenceConfigurationTypeDef


def get_value() -> PromptInferenceConfigurationTypeDef:
    return {
        "text": ...,
    }


# PromptInferenceConfigurationTypeDef definition

class PromptInferenceConfigurationTypeDef(TypedDict):
    text: NotRequired[PromptModelInferenceConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: PromptModelInferenceConfigurationUnionTypeDef](#promptmodelinferenceconfigurationuniontypedef)

## QueryGenerationContextOutputTypeDef

```python
# QueryGenerationContextOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import QueryGenerationContextOutputTypeDef


def get_value() -> QueryGenerationContextOutputTypeDef:
    return {
        "curatedQueries": ...,
    }


# QueryGenerationContextOutputTypeDef definition

class QueryGenerationContextOutputTypeDef(TypedDict):
    curatedQueries: NotRequired[List[CuratedQueryTypeDef]],  # (1)
    tables: NotRequired[List[QueryGenerationTableOutputTypeDef]],  # (2)
```

1. See `List[CuratedQueryTypeDef]`
2. See `List[QueryGenerationTableOutputTypeDef]`

## QueryGenerationContextTypeDef

```python
# QueryGenerationContextTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import QueryGenerationContextTypeDef


def get_value() -> QueryGenerationContextTypeDef:
    return {
        "curatedQueries": ...,
    }


# QueryGenerationContextTypeDef definition

class QueryGenerationContextTypeDef(TypedDict):
    curatedQueries: NotRequired[Sequence[CuratedQueryTypeDef]],  # (1)
    tables: NotRequired[Sequence[QueryGenerationTableTypeDef]],  # (2)
```

1. See `Sequence[CuratedQueryTypeDef]`
2. See `Sequence[QueryGenerationTableTypeDef]`

## StorageConfigurationTypeDef

```python
# StorageConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import StorageConfigurationTypeDef


def get_value() -> StorageConfigurationTypeDef:
    return {
        "mongoDbAtlasConfiguration": ...,
    }


# StorageConfigurationTypeDef definition

class StorageConfigurationTypeDef(TypedDict):
    type: KnowledgeBaseStorageTypeType,  # (6)
    mongoDbAtlasConfiguration: NotRequired[MongoDbAtlasConfigurationTypeDef],  # (1)
    opensearchServerlessConfiguration: NotRequired[OpenSearchServerlessConfigurationTypeDef],  # (2)
    pineconeConfiguration: NotRequired[PineconeConfigurationTypeDef],  # (3)
    rdsConfiguration: NotRequired[RdsConfigurationTypeDef],  # (4)
    redisEnterpriseCloudConfiguration: NotRequired[RedisEnterpriseCloudConfigurationTypeDef],  # (5)
```

1. See [:material-code-braces: MongoDbAtlasConfigurationTypeDef](./type_defs.md#mongodbatlasconfigurationtypedef)
2. See [:material-code-braces: OpenSearchServerlessConfigurationTypeDef](./type_defs.md#opensearchserverlessconfigurationtypedef)
3. See [:material-code-braces: PineconeConfigurationTypeDef](./type_defs.md#pineconeconfigurationtypedef)
4. See [:material-code-braces: RdsConfigurationTypeDef](./type_defs.md#rdsconfigurationtypedef)
5. See [:material-code-braces: RedisEnterpriseCloudConfigurationTypeDef](./type_defs.md#redisenterprisecloudconfigurationtypedef)
6. See [:material-code-brackets: KnowledgeBaseStorageTypeType](./literals.md#knowledgebasestoragetypetype)

## RedshiftQueryEngineConfigurationTypeDef

```python
# RedshiftQueryEngineConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import RedshiftQueryEngineConfigurationTypeDef


def get_value() -> RedshiftQueryEngineConfigurationTypeDef:
    return {
        "provisionedConfiguration": ...,
    }


# RedshiftQueryEngineConfigurationTypeDef definition

class RedshiftQueryEngineConfigurationTypeDef(TypedDict):
    type: RedshiftQueryEngineTypeType,  # (3)
    provisionedConfiguration: NotRequired[RedshiftProvisionedConfigurationTypeDef],  # (1)
    serverlessConfiguration: NotRequired[RedshiftServerlessConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: RedshiftProvisionedConfigurationTypeDef](./type_defs.md#redshiftprovisionedconfigurationtypedef)
2. See [:material-code-braces: RedshiftServerlessConfigurationTypeDef](./type_defs.md#redshiftserverlessconfigurationtypedef)
3. See [:material-code-brackets: RedshiftQueryEngineTypeType](./literals.md#redshiftqueryenginetypetype)

## RetrievalFlowNodeConfigurationTypeDef

```python
# RetrievalFlowNodeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import RetrievalFlowNodeConfigurationTypeDef


def get_value() -> RetrievalFlowNodeConfigurationTypeDef:
    return {
        "serviceConfiguration": ...,
    }


# RetrievalFlowNodeConfigurationTypeDef definition

class RetrievalFlowNodeConfigurationTypeDef(TypedDict):
    serviceConfiguration: RetrievalFlowNodeServiceConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: RetrievalFlowNodeServiceConfigurationTypeDef](./type_defs.md#retrievalflownodeserviceconfigurationtypedef)

## WebSourceConfigurationOutputTypeDef

```python
# WebSourceConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import WebSourceConfigurationOutputTypeDef


def get_value() -> WebSourceConfigurationOutputTypeDef:
    return {
        "urlConfiguration": ...,
    }


# WebSourceConfigurationOutputTypeDef definition

class WebSourceConfigurationOutputTypeDef(TypedDict):
    urlConfiguration: UrlConfigurationOutputTypeDef,  # (1)
```

1. See [:material-code-braces: UrlConfigurationOutputTypeDef](./type_defs.md#urlconfigurationoutputtypedef)

## WebSourceConfigurationTypeDef

```python
# WebSourceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import WebSourceConfigurationTypeDef


def get_value() -> WebSourceConfigurationTypeDef:
    return {
        "urlConfiguration": ...,
    }


# WebSourceConfigurationTypeDef definition

class WebSourceConfigurationTypeDef(TypedDict):
    urlConfiguration: UrlConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: UrlConfigurationTypeDef](./type_defs.md#urlconfigurationtypedef)

## StorageFlowNodeConfigurationTypeDef

```python
# StorageFlowNodeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import StorageFlowNodeConfigurationTypeDef


def get_value() -> StorageFlowNodeConfigurationTypeDef:
    return {
        "serviceConfiguration": ...,
    }


# StorageFlowNodeConfigurationTypeDef definition

class StorageFlowNodeConfigurationTypeDef(TypedDict):
    serviceConfiguration: StorageFlowNodeServiceConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: StorageFlowNodeServiceConfigurationTypeDef](./type_defs.md#storageflownodeserviceconfigurationtypedef)

## ToolOutputTypeDef

```python
# ToolOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ToolOutputTypeDef


def get_value() -> ToolOutputTypeDef:
    return {
        "cachePoint": ...,
    }


# ToolOutputTypeDef definition

class ToolOutputTypeDef(TypedDict):
    cachePoint: NotRequired[CachePointBlockTypeDef],  # (1)
    toolSpec: NotRequired[ToolSpecificationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: CachePointBlockTypeDef](./type_defs.md#cachepointblocktypedef)
2. See [:material-code-braces: ToolSpecificationOutputTypeDef](./type_defs.md#toolspecificationoutputtypedef)

## ToolSpecificationTypeDef

```python
# ToolSpecificationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ToolSpecificationTypeDef


def get_value() -> ToolSpecificationTypeDef:
    return {
        "description": ...,
    }


# ToolSpecificationTypeDef definition

class ToolSpecificationTypeDef(TypedDict):
    inputSchema: ToolInputSchemaUnionTypeDef,  # (1)
    name: str,
    description: NotRequired[str],
```

1. See [:material-code-braces: ToolInputSchemaUnionTypeDef](#toolinputschemauniontypedef)

## TransformationTypeDef

```python
# TransformationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import TransformationTypeDef


def get_value() -> TransformationTypeDef:
    return {
        "stepToApply": ...,
    }


# TransformationTypeDef definition

class TransformationTypeDef(TypedDict):
    stepToApply: StepTypeType,  # (1)
    transformationFunction: TransformationFunctionTypeDef,  # (2)
```

1. See [:material-code-brackets: StepTypeType](./literals.md#steptypetype)
2. See [:material-code-braces: TransformationFunctionTypeDef](./type_defs.md#transformationfunctiontypedef)

## CreateAgentAliasResponseTypeDef

```python
# CreateAgentAliasResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CreateAgentAliasResponseTypeDef


def get_value() -> CreateAgentAliasResponseTypeDef:
    return {
        "agentAlias": ...,
    }


# CreateAgentAliasResponseTypeDef definition

class CreateAgentAliasResponseTypeDef(TypedDict):
    agentAlias: AgentAliasTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentAliasTypeDef](./type_defs.md#agentaliastypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetAgentAliasResponseTypeDef

```python
# GetAgentAliasResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetAgentAliasResponseTypeDef


def get_value() -> GetAgentAliasResponseTypeDef:
    return {
        "agentAlias": ...,
    }


# GetAgentAliasResponseTypeDef definition

class GetAgentAliasResponseTypeDef(TypedDict):
    agentAlias: AgentAliasTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentAliasTypeDef](./type_defs.md#agentaliastypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateAgentAliasResponseTypeDef

```python
# UpdateAgentAliasResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UpdateAgentAliasResponseTypeDef


def get_value() -> UpdateAgentAliasResponseTypeDef:
    return {
        "agentAlias": ...,
    }


# UpdateAgentAliasResponseTypeDef definition

class UpdateAgentAliasResponseTypeDef(TypedDict):
    agentAlias: AgentAliasTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentAliasTypeDef](./type_defs.md#agentaliastypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CustomContentTypeDef

```python
# CustomContentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CustomContentTypeDef


def get_value() -> CustomContentTypeDef:
    return {
        "customDocumentIdentifier": ...,
    }


# CustomContentTypeDef definition

class CustomContentTypeDef(TypedDict):
    customDocumentIdentifier: CustomDocumentIdentifierTypeDef,  # (1)
    sourceType: CustomSourceTypeType,  # (4)
    inlineContent: NotRequired[InlineContentTypeDef],  # (2)
    s3Location: NotRequired[CustomS3LocationTypeDef],  # (3)
```

1. See [:material-code-braces: CustomDocumentIdentifierTypeDef](./type_defs.md#customdocumentidentifiertypedef)
2. See [:material-code-braces: InlineContentTypeDef](./type_defs.md#inlinecontenttypedef)
3. See [:material-code-braces: CustomS3LocationTypeDef](./type_defs.md#customs3locationtypedef)
4. See [:material-code-brackets: CustomSourceTypeType](./literals.md#customsourcetypetype)

## DeleteKnowledgeBaseDocumentsResponseTypeDef

```python
# DeleteKnowledgeBaseDocumentsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DeleteKnowledgeBaseDocumentsResponseTypeDef


def get_value() -> DeleteKnowledgeBaseDocumentsResponseTypeDef:
    return {
        "documentDetails": ...,
    }


# DeleteKnowledgeBaseDocumentsResponseTypeDef definition

class DeleteKnowledgeBaseDocumentsResponseTypeDef(TypedDict):
    documentDetails: List[KnowledgeBaseDocumentDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `List[KnowledgeBaseDocumentDetailTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetKnowledgeBaseDocumentsResponseTypeDef

```python
# GetKnowledgeBaseDocumentsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetKnowledgeBaseDocumentsResponseTypeDef


def get_value() -> GetKnowledgeBaseDocumentsResponseTypeDef:
    return {
        "documentDetails": ...,
    }


# GetKnowledgeBaseDocumentsResponseTypeDef definition

class GetKnowledgeBaseDocumentsResponseTypeDef(TypedDict):
    documentDetails: List[KnowledgeBaseDocumentDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `List[KnowledgeBaseDocumentDetailTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## IngestKnowledgeBaseDocumentsResponseTypeDef

```python
# IngestKnowledgeBaseDocumentsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import IngestKnowledgeBaseDocumentsResponseTypeDef


def get_value() -> IngestKnowledgeBaseDocumentsResponseTypeDef:
    return {
        "documentDetails": ...,
    }


# IngestKnowledgeBaseDocumentsResponseTypeDef definition

class IngestKnowledgeBaseDocumentsResponseTypeDef(TypedDict):
    documentDetails: List[KnowledgeBaseDocumentDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `List[KnowledgeBaseDocumentDetailTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListKnowledgeBaseDocumentsResponseTypeDef

```python
# ListKnowledgeBaseDocumentsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ListKnowledgeBaseDocumentsResponseTypeDef


def get_value() -> ListKnowledgeBaseDocumentsResponseTypeDef:
    return {
        "documentDetails": ...,
    }


# ListKnowledgeBaseDocumentsResponseTypeDef definition

class ListKnowledgeBaseDocumentsResponseTypeDef(TypedDict):
    documentDetails: List[KnowledgeBaseDocumentDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `List[KnowledgeBaseDocumentDetailTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## VectorKnowledgeBaseConfigurationOutputTypeDef

```python
# VectorKnowledgeBaseConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import VectorKnowledgeBaseConfigurationOutputTypeDef


def get_value() -> VectorKnowledgeBaseConfigurationOutputTypeDef:
    return {
        "embeddingModelArn": ...,
    }


# VectorKnowledgeBaseConfigurationOutputTypeDef definition

class VectorKnowledgeBaseConfigurationOutputTypeDef(TypedDict):
    embeddingModelArn: str,
    embeddingModelConfiguration: NotRequired[EmbeddingModelConfigurationTypeDef],  # (1)
    supplementalDataStorageConfiguration: NotRequired[SupplementalDataStorageConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: EmbeddingModelConfigurationTypeDef](./type_defs.md#embeddingmodelconfigurationtypedef)
2. See [:material-code-braces: SupplementalDataStorageConfigurationOutputTypeDef](./type_defs.md#supplementaldatastorageconfigurationoutputtypedef)

## VectorKnowledgeBaseConfigurationTypeDef

```python
# VectorKnowledgeBaseConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import VectorKnowledgeBaseConfigurationTypeDef


def get_value() -> VectorKnowledgeBaseConfigurationTypeDef:
    return {
        "embeddingModelArn": ...,
    }


# VectorKnowledgeBaseConfigurationTypeDef definition

class VectorKnowledgeBaseConfigurationTypeDef(TypedDict):
    embeddingModelArn: str,
    embeddingModelConfiguration: NotRequired[EmbeddingModelConfigurationTypeDef],  # (1)
    supplementalDataStorageConfiguration: NotRequired[SupplementalDataStorageConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: EmbeddingModelConfigurationTypeDef](./type_defs.md#embeddingmodelconfigurationtypedef)
2. See [:material-code-braces: SupplementalDataStorageConfigurationTypeDef](./type_defs.md#supplementaldatastorageconfigurationtypedef)

## ValidateFlowDefinitionResponseTypeDef

```python
# ValidateFlowDefinitionResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ValidateFlowDefinitionResponseTypeDef


def get_value() -> ValidateFlowDefinitionResponseTypeDef:
    return {
        "validations": ...,
    }


# ValidateFlowDefinitionResponseTypeDef definition

class ValidateFlowDefinitionResponseTypeDef(TypedDict):
    validations: List[FlowValidationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `List[FlowValidationTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## AgentActionGroupTypeDef

```python
# AgentActionGroupTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import AgentActionGroupTypeDef


def get_value() -> AgentActionGroupTypeDef:
    return {
        "actionGroupExecutor": ...,
    }


# AgentActionGroupTypeDef definition

class AgentActionGroupTypeDef(TypedDict):
    actionGroupId: str,
    actionGroupName: str,
    actionGroupState: ActionGroupStateType,  # (2)
    agentId: str,
    agentVersion: str,
    createdAt: datetime.datetime,
    updatedAt: datetime.datetime,
    actionGroupExecutor: NotRequired[ActionGroupExecutorTypeDef],  # (1)
    apiSchema: NotRequired[APISchemaTypeDef],  # (3)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    functionSchema: NotRequired[FunctionSchemaOutputTypeDef],  # (4)
    parentActionSignature: NotRequired[ActionGroupSignatureType],  # (5)
```

1. See [:material-code-braces: ActionGroupExecutorTypeDef](./type_defs.md#actiongroupexecutortypedef)
2. See [:material-code-brackets: ActionGroupStateType](./literals.md#actiongroupstatetype)
3. See [:material-code-braces: APISchemaTypeDef](./type_defs.md#apischematypedef)
4. See [:material-code-braces: FunctionSchemaOutputTypeDef](./type_defs.md#functionschemaoutputtypedef)
5. See [:material-code-brackets: ActionGroupSignatureType](./literals.md#actiongroupsignaturetype)

## AgentTypeDef

```python
# AgentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import AgentTypeDef


def get_value() -> AgentTypeDef:
    return {
        "agentArn": ...,
    }


# AgentTypeDef definition

class AgentTypeDef(TypedDict):
    agentArn: str,
    agentId: str,
    agentName: str,
    agentResourceRoleArn: str,
    agentStatus: AgentStatusType,  # (2)
    agentVersion: str,
    createdAt: datetime.datetime,
    idleSessionTTLInSeconds: int,
    updatedAt: datetime.datetime,
    agentCollaboration: NotRequired[AgentCollaborationType],  # (1)
    clientToken: NotRequired[str],
    customOrchestration: NotRequired[CustomOrchestrationTypeDef],  # (3)
    customerEncryptionKeyArn: NotRequired[str],
    description: NotRequired[str],
    failureReasons: NotRequired[List[str]],
    foundationModel: NotRequired[str],
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (4)
    instruction: NotRequired[str],
    memoryConfiguration: NotRequired[MemoryConfigurationOutputTypeDef],  # (5)
    orchestrationType: NotRequired[OrchestrationTypeType],  # (6)
    preparedAt: NotRequired[datetime.datetime],
    promptOverrideConfiguration: NotRequired[PromptOverrideConfigurationOutputTypeDef],  # (7)
    recommendedActions: NotRequired[List[str]],
```

1. See [:material-code-brackets: AgentCollaborationType](./literals.md#agentcollaborationtype)
2. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype)
3. See [:material-code-braces: CustomOrchestrationTypeDef](./type_defs.md#customorchestrationtypedef)
4. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef)
5. See [:material-code-braces: MemoryConfigurationOutputTypeDef](./type_defs.md#memoryconfigurationoutputtypedef)
6. See [:material-code-brackets: OrchestrationTypeType](./literals.md#orchestrationtypetype)
7. See [:material-code-braces: PromptOverrideConfigurationOutputTypeDef](./type_defs.md#promptoverrideconfigurationoutputtypedef)

## AgentVersionTypeDef

```python
# AgentVersionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import AgentVersionTypeDef


def get_value() -> AgentVersionTypeDef:
    return {
        "agentArn": ...,
    }


# AgentVersionTypeDef definition

class AgentVersionTypeDef(TypedDict):
    agentArn: str,
    agentId: str,
    agentName: str,
    agentResourceRoleArn: str,
    agentStatus: AgentStatusType,  # (2)
    createdAt: datetime.datetime,
    idleSessionTTLInSeconds: int,
    updatedAt: datetime.datetime,
    version: str,
    agentCollaboration: NotRequired[AgentCollaborationType],  # (1)
    customerEncryptionKeyArn: NotRequired[str],
    description: NotRequired[str],
    failureReasons: NotRequired[List[str]],
    foundationModel: NotRequired[str],
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (3)
    instruction: NotRequired[str],
    memoryConfiguration: NotRequired[MemoryConfigurationOutputTypeDef],  # (4)
    promptOverrideConfiguration: NotRequired[PromptOverrideConfigurationOutputTypeDef],  # (5)
    recommendedActions: NotRequired[List[str]],
```

1. See [:material-code-brackets: AgentCollaborationType](./literals.md#agentcollaborationtype)
2. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype)
3. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef)
4. See [:material-code-braces: MemoryConfigurationOutputTypeDef](./type_defs.md#memoryconfigurationoutputtypedef)
5. See [:material-code-braces: PromptOverrideConfigurationOutputTypeDef](./type_defs.md#promptoverrideconfigurationoutputtypedef)

## ConfluenceCrawlerConfigurationOutputTypeDef

```python
# ConfluenceCrawlerConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ConfluenceCrawlerConfigurationOutputTypeDef


def get_value() -> ConfluenceCrawlerConfigurationOutputTypeDef:
    return {
        "filterConfiguration": ...,
    }


# ConfluenceCrawlerConfigurationOutputTypeDef definition

class ConfluenceCrawlerConfigurationOutputTypeDef(TypedDict):
    filterConfiguration: NotRequired[CrawlFilterConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: CrawlFilterConfigurationOutputTypeDef](./type_defs.md#crawlfilterconfigurationoutputtypedef)

## SalesforceCrawlerConfigurationOutputTypeDef

```python
# SalesforceCrawlerConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import SalesforceCrawlerConfigurationOutputTypeDef


def get_value() -> SalesforceCrawlerConfigurationOutputTypeDef:
    return {
        "filterConfiguration": ...,
    }


# SalesforceCrawlerConfigurationOutputTypeDef definition

class SalesforceCrawlerConfigurationOutputTypeDef(TypedDict):
    filterConfiguration: NotRequired[CrawlFilterConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: CrawlFilterConfigurationOutputTypeDef](./type_defs.md#crawlfilterconfigurationoutputtypedef)

## SharePointCrawlerConfigurationOutputTypeDef

```python
# SharePointCrawlerConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import SharePointCrawlerConfigurationOutputTypeDef


def get_value() -> SharePointCrawlerConfigurationOutputTypeDef:
    return {
        "filterConfiguration": ...,
    }


# SharePointCrawlerConfigurationOutputTypeDef definition

class SharePointCrawlerConfigurationOutputTypeDef(TypedDict):
    filterConfiguration: NotRequired[CrawlFilterConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: CrawlFilterConfigurationOutputTypeDef](./type_defs.md#crawlfilterconfigurationoutputtypedef)

## ConfluenceCrawlerConfigurationTypeDef

```python
# ConfluenceCrawlerConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ConfluenceCrawlerConfigurationTypeDef


def get_value() -> ConfluenceCrawlerConfigurationTypeDef:
    return {
        "filterConfiguration": ...,
    }


# ConfluenceCrawlerConfigurationTypeDef definition

class ConfluenceCrawlerConfigurationTypeDef(TypedDict):
    filterConfiguration: NotRequired[CrawlFilterConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: CrawlFilterConfigurationTypeDef](./type_defs.md#crawlfilterconfigurationtypedef)

## SalesforceCrawlerConfigurationTypeDef

```python
# SalesforceCrawlerConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import SalesforceCrawlerConfigurationTypeDef


def get_value() -> SalesforceCrawlerConfigurationTypeDef:
    return {
        "filterConfiguration": ...,
    }


# SalesforceCrawlerConfigurationTypeDef definition

class SalesforceCrawlerConfigurationTypeDef(TypedDict):
    filterConfiguration: NotRequired[CrawlFilterConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: CrawlFilterConfigurationTypeDef](./type_defs.md#crawlfilterconfigurationtypedef)

## SharePointCrawlerConfigurationTypeDef

```python
# SharePointCrawlerConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import SharePointCrawlerConfigurationTypeDef


def get_value() -> SharePointCrawlerConfigurationTypeDef:
    return {
        "filterConfiguration": ...,
    }


# SharePointCrawlerConfigurationTypeDef definition

class SharePointCrawlerConfigurationTypeDef(TypedDict):
    filterConfiguration: NotRequired[CrawlFilterConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: CrawlFilterConfigurationTypeDef](./type_defs.md#crawlfilterconfigurationtypedef)

## QueryGenerationConfigurationOutputTypeDef

```python
# QueryGenerationConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import QueryGenerationConfigurationOutputTypeDef


def get_value() -> QueryGenerationConfigurationOutputTypeDef:
    return {
        "executionTimeoutSeconds": ...,
    }


# QueryGenerationConfigurationOutputTypeDef definition

class QueryGenerationConfigurationOutputTypeDef(TypedDict):
    executionTimeoutSeconds: NotRequired[int],
    generationContext: NotRequired[QueryGenerationContextOutputTypeDef],  # (1)
```

1. See [:material-code-braces: QueryGenerationContextOutputTypeDef](./type_defs.md#querygenerationcontextoutputtypedef)

## QueryGenerationConfigurationTypeDef

```python
# QueryGenerationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import QueryGenerationConfigurationTypeDef


def get_value() -> QueryGenerationConfigurationTypeDef:
    return {
        "executionTimeoutSeconds": ...,
    }


# QueryGenerationConfigurationTypeDef definition

class QueryGenerationConfigurationTypeDef(TypedDict):
    executionTimeoutSeconds: NotRequired[int],
    generationContext: NotRequired[QueryGenerationContextTypeDef],  # (1)
```

1. See [:material-code-braces: QueryGenerationContextTypeDef](./type_defs.md#querygenerationcontexttypedef)

## WebDataSourceConfigurationOutputTypeDef

```python
# WebDataSourceConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import WebDataSourceConfigurationOutputTypeDef


def get_value() -> WebDataSourceConfigurationOutputTypeDef:
    return {
        "crawlerConfiguration": ...,
    }


# WebDataSourceConfigurationOutputTypeDef definition

class WebDataSourceConfigurationOutputTypeDef(TypedDict):
    sourceConfiguration: WebSourceConfigurationOutputTypeDef,  # (2)
    crawlerConfiguration: NotRequired[WebCrawlerConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: WebCrawlerConfigurationOutputTypeDef](./type_defs.md#webcrawlerconfigurationoutputtypedef)
2. See [:material-code-braces: WebSourceConfigurationOutputTypeDef](./type_defs.md#websourceconfigurationoutputtypedef)

## WebDataSourceConfigurationTypeDef

```python
# WebDataSourceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import WebDataSourceConfigurationTypeDef


def get_value() -> WebDataSourceConfigurationTypeDef:
    return {
        "crawlerConfiguration": ...,
    }


# WebDataSourceConfigurationTypeDef definition

class WebDataSourceConfigurationTypeDef(TypedDict):
    sourceConfiguration: WebSourceConfigurationTypeDef,  # (2)
    crawlerConfiguration: NotRequired[WebCrawlerConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: WebCrawlerConfigurationTypeDef](./type_defs.md#webcrawlerconfigurationtypedef)
2. See [:material-code-braces: WebSourceConfigurationTypeDef](./type_defs.md#websourceconfigurationtypedef)

## ToolConfigurationOutputTypeDef

```python
# ToolConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ToolConfigurationOutputTypeDef


def get_value() -> ToolConfigurationOutputTypeDef:
    return {
        "toolChoice": ...,
    }


# ToolConfigurationOutputTypeDef definition

class ToolConfigurationOutputTypeDef(TypedDict):
    tools: List[ToolOutputTypeDef],  # (2)
    toolChoice: NotRequired[ToolChoiceOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ToolChoiceOutputTypeDef](./type_defs.md#toolchoiceoutputtypedef)
2. See `List[ToolOutputTypeDef]`

## CustomTransformationConfigurationOutputTypeDef

```python
# CustomTransformationConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CustomTransformationConfigurationOutputTypeDef


def get_value() -> CustomTransformationConfigurationOutputTypeDef:
    return {
        "intermediateStorage": ...,
    }


# CustomTransformationConfigurationOutputTypeDef definition

class CustomTransformationConfigurationOutputTypeDef(TypedDict):
    intermediateStorage: IntermediateStorageTypeDef,  # (1)
    transformations: List[TransformationTypeDef],  # (2)
```

1. See [:material-code-braces: IntermediateStorageTypeDef](./type_defs.md#intermediatestoragetypedef)
2. See `List[TransformationTypeDef]`

## CustomTransformationConfigurationTypeDef

```python
# CustomTransformationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CustomTransformationConfigurationTypeDef


def get_value() -> CustomTransformationConfigurationTypeDef:
    return {
        "intermediateStorage": ...,
    }


# CustomTransformationConfigurationTypeDef definition

class CustomTransformationConfigurationTypeDef(TypedDict):
    intermediateStorage: IntermediateStorageTypeDef,  # (1)
    transformations: Sequence[TransformationTypeDef],  # (2)
```

1. See [:material-code-braces: IntermediateStorageTypeDef](./type_defs.md#intermediatestoragetypedef)
2. See `Sequence[TransformationTypeDef]`

## DocumentContentTypeDef

```python
# DocumentContentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DocumentContentTypeDef


def get_value() -> DocumentContentTypeDef:
    return {
        "custom": ...,
    }


# DocumentContentTypeDef definition

class DocumentContentTypeDef(TypedDict):
    dataSourceType: ContentDataSourceTypeType,  # (2)
    custom: NotRequired[CustomContentTypeDef],  # (1)
    s3: NotRequired[S3ContentTypeDef],  # (3)
```

1. See [:material-code-braces: CustomContentTypeDef](./type_defs.md#customcontenttypedef)
2. See [:material-code-brackets: ContentDataSourceTypeType](./literals.md#contentdatasourcetypetype)
3. See [:material-code-braces: S3ContentTypeDef](./type_defs.md#s3contenttypedef)

## CreateAgentActionGroupResponseTypeDef

```python
# CreateAgentActionGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CreateAgentActionGroupResponseTypeDef


def get_value() -> CreateAgentActionGroupResponseTypeDef:
    return {
        "agentActionGroup": ...,
    }


# CreateAgentActionGroupResponseTypeDef definition

class CreateAgentActionGroupResponseTypeDef(TypedDict):
    agentActionGroup: AgentActionGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentActionGroupTypeDef](./type_defs.md#agentactiongrouptypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetAgentActionGroupResponseTypeDef

```python
# GetAgentActionGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetAgentActionGroupResponseTypeDef


def get_value() -> GetAgentActionGroupResponseTypeDef:
    return {
        "agentActionGroup": ...,
    }


# GetAgentActionGroupResponseTypeDef definition

class GetAgentActionGroupResponseTypeDef(TypedDict):
    agentActionGroup: AgentActionGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentActionGroupTypeDef](./type_defs.md#agentactiongrouptypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateAgentActionGroupResponseTypeDef

```python
# UpdateAgentActionGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UpdateAgentActionGroupResponseTypeDef


def get_value() -> UpdateAgentActionGroupResponseTypeDef:
    return {
        "agentActionGroup": ...,
    }


# UpdateAgentActionGroupResponseTypeDef definition

class UpdateAgentActionGroupResponseTypeDef(TypedDict):
    agentActionGroup: AgentActionGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentActionGroupTypeDef](./type_defs.md#agentactiongrouptypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateAgentActionGroupRequestTypeDef

```python
# CreateAgentActionGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CreateAgentActionGroupRequestTypeDef


def get_value() -> CreateAgentActionGroupRequestTypeDef:
    return {
        "actionGroupName": ...,
    }


# CreateAgentActionGroupRequestTypeDef definition

class CreateAgentActionGroupRequestTypeDef(TypedDict):
    actionGroupName: str,
    agentId: str,
    agentVersion: str,
    actionGroupExecutor: NotRequired[ActionGroupExecutorTypeDef],  # (1)
    actionGroupState: NotRequired[ActionGroupStateType],  # (2)
    apiSchema: NotRequired[APISchemaTypeDef],  # (3)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    functionSchema: NotRequired[FunctionSchemaUnionTypeDef],  # (4)
    parentActionGroupSignature: NotRequired[ActionGroupSignatureType],  # (5)
```

1. See [:material-code-braces: ActionGroupExecutorTypeDef](./type_defs.md#actiongroupexecutortypedef)
2. See [:material-code-brackets: ActionGroupStateType](./literals.md#actiongroupstatetype)
3. See [:material-code-braces: APISchemaTypeDef](./type_defs.md#apischematypedef)
4. See [:material-code-braces: FunctionSchemaUnionTypeDef](#functionschemauniontypedef)
5. See [:material-code-brackets: ActionGroupSignatureType](./literals.md#actiongroupsignaturetype)

## UpdateAgentActionGroupRequestTypeDef

```python
# UpdateAgentActionGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UpdateAgentActionGroupRequestTypeDef


def get_value() -> UpdateAgentActionGroupRequestTypeDef:
    return {
        "actionGroupId": ...,
    }


# UpdateAgentActionGroupRequestTypeDef definition

class UpdateAgentActionGroupRequestTypeDef(TypedDict):
    actionGroupId: str,
    actionGroupName: str,
    agentId: str,
    agentVersion: str,
    actionGroupExecutor: NotRequired[ActionGroupExecutorTypeDef],  # (1)
    actionGroupState: NotRequired[ActionGroupStateType],  # (2)
    apiSchema: NotRequired[APISchemaTypeDef],  # (3)
    description: NotRequired[str],
    functionSchema: NotRequired[FunctionSchemaUnionTypeDef],  # (4)
    parentActionGroupSignature: NotRequired[ActionGroupSignatureType],  # (5)
```

1. See [:material-code-braces: ActionGroupExecutorTypeDef](./type_defs.md#actiongroupexecutortypedef)
2. See [:material-code-brackets: ActionGroupStateType](./literals.md#actiongroupstatetype)
3. See [:material-code-braces: APISchemaTypeDef](./type_defs.md#apischematypedef)
4. See [:material-code-braces: FunctionSchemaUnionTypeDef](#functionschemauniontypedef)
5. See [:material-code-brackets: ActionGroupSignatureType](./literals.md#actiongroupsignaturetype)

## CreateAgentResponseTypeDef

```python
# CreateAgentResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CreateAgentResponseTypeDef


def get_value() -> CreateAgentResponseTypeDef:
    return {
        "agent": ...,
    }


# CreateAgentResponseTypeDef definition

class CreateAgentResponseTypeDef(TypedDict):
    agent: AgentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentTypeDef](./type_defs.md#agenttypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetAgentResponseTypeDef

```python
# GetAgentResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetAgentResponseTypeDef


def get_value() -> GetAgentResponseTypeDef:
    return {
        "agent": ...,
    }


# GetAgentResponseTypeDef definition

class GetAgentResponseTypeDef(TypedDict):
    agent: AgentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentTypeDef](./type_defs.md#agenttypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateAgentResponseTypeDef

```python
# UpdateAgentResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UpdateAgentResponseTypeDef


def get_value() -> UpdateAgentResponseTypeDef:
    return {
        "agent": ...,
    }


# UpdateAgentResponseTypeDef definition

class UpdateAgentResponseTypeDef(TypedDict):
    agent: AgentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentTypeDef](./type_defs.md#agenttypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetAgentVersionResponseTypeDef

```python
# GetAgentVersionResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetAgentVersionResponseTypeDef


def get_value() -> GetAgentVersionResponseTypeDef:
    return {
        "agentVersion": ...,
    }


# GetAgentVersionResponseTypeDef definition

class GetAgentVersionResponseTypeDef(TypedDict):
    agentVersion: AgentVersionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentVersionTypeDef](./type_defs.md#agentversiontypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateAgentRequestTypeDef

```python
# CreateAgentRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CreateAgentRequestTypeDef


def get_value() -> CreateAgentRequestTypeDef:
    return {
        "agentName": ...,
    }


# CreateAgentRequestTypeDef definition

class CreateAgentRequestTypeDef(TypedDict):
    agentName: str,
    agentCollaboration: NotRequired[AgentCollaborationType],  # (1)
    agentResourceRoleArn: NotRequired[str],
    clientToken: NotRequired[str],
    customOrchestration: NotRequired[CustomOrchestrationTypeDef],  # (2)
    customerEncryptionKeyArn: NotRequired[str],
    description: NotRequired[str],
    foundationModel: NotRequired[str],
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (3)
    idleSessionTTLInSeconds: NotRequired[int],
    instruction: NotRequired[str],
    memoryConfiguration: NotRequired[MemoryConfigurationUnionTypeDef],  # (4)
    orchestrationType: NotRequired[OrchestrationTypeType],  # (5)
    promptOverrideConfiguration: NotRequired[PromptOverrideConfigurationUnionTypeDef],  # (6)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: AgentCollaborationType](./literals.md#agentcollaborationtype)
2. See [:material-code-braces: CustomOrchestrationTypeDef](./type_defs.md#customorchestrationtypedef)
3. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef)
4. See [:material-code-braces: MemoryConfigurationUnionTypeDef](#memoryconfigurationuniontypedef)
5. See [:material-code-brackets: OrchestrationTypeType](./literals.md#orchestrationtypetype)
6. See [:material-code-braces: PromptOverrideConfigurationUnionTypeDef](#promptoverrideconfigurationuniontypedef)

## UpdateAgentRequestTypeDef

```python
# UpdateAgentRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UpdateAgentRequestTypeDef


def get_value() -> UpdateAgentRequestTypeDef:
    return {
        "agentId": ...,
    }


# UpdateAgentRequestTypeDef definition

class UpdateAgentRequestTypeDef(TypedDict):
    agentId: str,
    agentName: str,
    agentResourceRoleArn: str,
    foundationModel: str,
    agentCollaboration: NotRequired[AgentCollaborationType],  # (1)
    customOrchestration: NotRequired[CustomOrchestrationTypeDef],  # (2)
    customerEncryptionKeyArn: NotRequired[str],
    description: NotRequired[str],
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (3)
    idleSessionTTLInSeconds: NotRequired[int],
    instruction: NotRequired[str],
    memoryConfiguration: NotRequired[MemoryConfigurationUnionTypeDef],  # (4)
    orchestrationType: NotRequired[OrchestrationTypeType],  # (5)
    promptOverrideConfiguration: NotRequired[PromptOverrideConfigurationUnionTypeDef],  # (6)
```

1. See [:material-code-brackets: AgentCollaborationType](./literals.md#agentcollaborationtype)
2. See [:material-code-braces: CustomOrchestrationTypeDef](./type_defs.md#customorchestrationtypedef)
3. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef)
4. See [:material-code-braces: MemoryConfigurationUnionTypeDef](#memoryconfigurationuniontypedef)
5. See [:material-code-brackets: OrchestrationTypeType](./literals.md#orchestrationtypetype)
6. See [:material-code-braces: PromptOverrideConfigurationUnionTypeDef](#promptoverrideconfigurationuniontypedef)

## ConfluenceDataSourceConfigurationOutputTypeDef

```python
# ConfluenceDataSourceConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ConfluenceDataSourceConfigurationOutputTypeDef


def get_value() -> ConfluenceDataSourceConfigurationOutputTypeDef:
    return {
        "crawlerConfiguration": ...,
    }


# ConfluenceDataSourceConfigurationOutputTypeDef definition

class ConfluenceDataSourceConfigurationOutputTypeDef(TypedDict):
    sourceConfiguration: ConfluenceSourceConfigurationTypeDef,  # (2)
    crawlerConfiguration: NotRequired[ConfluenceCrawlerConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ConfluenceCrawlerConfigurationOutputTypeDef](./type_defs.md#confluencecrawlerconfigurationoutputtypedef)
2. See [:material-code-braces: ConfluenceSourceConfigurationTypeDef](./type_defs.md#confluencesourceconfigurationtypedef)

## SalesforceDataSourceConfigurationOutputTypeDef

```python
# SalesforceDataSourceConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import SalesforceDataSourceConfigurationOutputTypeDef


def get_value() -> SalesforceDataSourceConfigurationOutputTypeDef:
    return {
        "crawlerConfiguration": ...,
    }


# SalesforceDataSourceConfigurationOutputTypeDef definition

class SalesforceDataSourceConfigurationOutputTypeDef(TypedDict):
    sourceConfiguration: SalesforceSourceConfigurationTypeDef,  # (2)
    crawlerConfiguration: NotRequired[SalesforceCrawlerConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: SalesforceCrawlerConfigurationOutputTypeDef](./type_defs.md#salesforcecrawlerconfigurationoutputtypedef)
2. See [:material-code-braces: SalesforceSourceConfigurationTypeDef](./type_defs.md#salesforcesourceconfigurationtypedef)

## SharePointDataSourceConfigurationOutputTypeDef

```python
# SharePointDataSourceConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import SharePointDataSourceConfigurationOutputTypeDef


def get_value() -> SharePointDataSourceConfigurationOutputTypeDef:
    return {
        "crawlerConfiguration": ...,
    }


# SharePointDataSourceConfigurationOutputTypeDef definition

class SharePointDataSourceConfigurationOutputTypeDef(TypedDict):
    sourceConfiguration: SharePointSourceConfigurationOutputTypeDef,  # (2)
    crawlerConfiguration: NotRequired[SharePointCrawlerConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: SharePointCrawlerConfigurationOutputTypeDef](./type_defs.md#sharepointcrawlerconfigurationoutputtypedef)
2. See [:material-code-braces: SharePointSourceConfigurationOutputTypeDef](./type_defs.md#sharepointsourceconfigurationoutputtypedef)

## ConfluenceDataSourceConfigurationTypeDef

```python
# ConfluenceDataSourceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ConfluenceDataSourceConfigurationTypeDef


def get_value() -> ConfluenceDataSourceConfigurationTypeDef:
    return {
        "crawlerConfiguration": ...,
    }


# ConfluenceDataSourceConfigurationTypeDef definition

class ConfluenceDataSourceConfigurationTypeDef(TypedDict):
    sourceConfiguration: ConfluenceSourceConfigurationTypeDef,  # (2)
    crawlerConfiguration: NotRequired[ConfluenceCrawlerConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ConfluenceCrawlerConfigurationTypeDef](./type_defs.md#confluencecrawlerconfigurationtypedef)
2. See [:material-code-braces: ConfluenceSourceConfigurationTypeDef](./type_defs.md#confluencesourceconfigurationtypedef)

## SalesforceDataSourceConfigurationTypeDef

```python
# SalesforceDataSourceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import SalesforceDataSourceConfigurationTypeDef


def get_value() -> SalesforceDataSourceConfigurationTypeDef:
    return {
        "crawlerConfiguration": ...,
    }


# SalesforceDataSourceConfigurationTypeDef definition

class SalesforceDataSourceConfigurationTypeDef(TypedDict):
    sourceConfiguration: SalesforceSourceConfigurationTypeDef,  # (2)
    crawlerConfiguration: NotRequired[SalesforceCrawlerConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: SalesforceCrawlerConfigurationTypeDef](./type_defs.md#salesforcecrawlerconfigurationtypedef)
2. See [:material-code-braces: SalesforceSourceConfigurationTypeDef](./type_defs.md#salesforcesourceconfigurationtypedef)

## SharePointDataSourceConfigurationTypeDef

```python
# SharePointDataSourceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import SharePointDataSourceConfigurationTypeDef


def get_value() -> SharePointDataSourceConfigurationTypeDef:
    return {
        "crawlerConfiguration": ...,
    }


# SharePointDataSourceConfigurationTypeDef definition

class SharePointDataSourceConfigurationTypeDef(TypedDict):
    sourceConfiguration: SharePointSourceConfigurationTypeDef,  # (2)
    crawlerConfiguration: NotRequired[SharePointCrawlerConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: SharePointCrawlerConfigurationTypeDef](./type_defs.md#sharepointcrawlerconfigurationtypedef)
2. See [:material-code-braces: SharePointSourceConfigurationTypeDef](./type_defs.md#sharepointsourceconfigurationtypedef)

## RedshiftConfigurationOutputTypeDef

```python
# RedshiftConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import RedshiftConfigurationOutputTypeDef


def get_value() -> RedshiftConfigurationOutputTypeDef:
    return {
        "queryEngineConfiguration": ...,
    }


# RedshiftConfigurationOutputTypeDef definition

class RedshiftConfigurationOutputTypeDef(TypedDict):
    queryEngineConfiguration: RedshiftQueryEngineConfigurationTypeDef,  # (1)
    storageConfigurations: List[RedshiftQueryEngineStorageConfigurationOutputTypeDef],  # (3)
    queryGenerationConfiguration: NotRequired[QueryGenerationConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: RedshiftQueryEngineConfigurationTypeDef](./type_defs.md#redshiftqueryengineconfigurationtypedef)
2. See [:material-code-braces: QueryGenerationConfigurationOutputTypeDef](./type_defs.md#querygenerationconfigurationoutputtypedef)
3. See `List[RedshiftQueryEngineStorageConfigurationOutputTypeDef]`

## RedshiftConfigurationTypeDef

```python
# RedshiftConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import RedshiftConfigurationTypeDef


def get_value() -> RedshiftConfigurationTypeDef:
    return {
        "queryEngineConfiguration": ...,
    }


# RedshiftConfigurationTypeDef definition

class RedshiftConfigurationTypeDef(TypedDict):
    queryEngineConfiguration: RedshiftQueryEngineConfigurationTypeDef,  # (1)
    storageConfigurations: Sequence[RedshiftQueryEngineStorageConfigurationTypeDef],  # (3)
    queryGenerationConfiguration: NotRequired[QueryGenerationConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: RedshiftQueryEngineConfigurationTypeDef](./type_defs.md#redshiftqueryengineconfigurationtypedef)
2. See [:material-code-braces: QueryGenerationConfigurationTypeDef](./type_defs.md#querygenerationconfigurationtypedef)
3. See `Sequence[RedshiftQueryEngineStorageConfigurationTypeDef]`

## ChatPromptTemplateConfigurationOutputTypeDef

```python
# ChatPromptTemplateConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ChatPromptTemplateConfigurationOutputTypeDef


def get_value() -> ChatPromptTemplateConfigurationOutputTypeDef:
    return {
        "inputVariables": ...,
    }


# ChatPromptTemplateConfigurationOutputTypeDef definition

class ChatPromptTemplateConfigurationOutputTypeDef(TypedDict):
    messages: List[MessageOutputTypeDef],  # (2)
    inputVariables: NotRequired[List[PromptInputVariableTypeDef]],  # (1)
    system: NotRequired[List[SystemContentBlockTypeDef]],  # (3)
    toolConfiguration: NotRequired[ToolConfigurationOutputTypeDef],  # (4)
```

1. See `List[PromptInputVariableTypeDef]`
2. See `List[MessageOutputTypeDef]`
3. See `List[SystemContentBlockTypeDef]`
4. See [:material-code-braces: ToolConfigurationOutputTypeDef](./type_defs.md#toolconfigurationoutputtypedef)

## ToolTypeDef

```python
# ToolTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ToolTypeDef


def get_value() -> ToolTypeDef:
    return {
        "cachePoint": ...,
    }


# ToolTypeDef definition

class ToolTypeDef(TypedDict):
    cachePoint: NotRequired[CachePointBlockTypeDef],  # (1)
    toolSpec: NotRequired[ToolSpecificationUnionTypeDef],  # (2)
```

1. See [:material-code-braces: CachePointBlockTypeDef](./type_defs.md#cachepointblocktypedef)
2. See [:material-code-braces: ToolSpecificationUnionTypeDef](#toolspecificationuniontypedef)

## VectorIngestionConfigurationOutputTypeDef

```python
# VectorIngestionConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import VectorIngestionConfigurationOutputTypeDef


def get_value() -> VectorIngestionConfigurationOutputTypeDef:
    return {
        "chunkingConfiguration": ...,
    }


# VectorIngestionConfigurationOutputTypeDef definition

class VectorIngestionConfigurationOutputTypeDef(TypedDict):
    chunkingConfiguration: NotRequired[ChunkingConfigurationOutputTypeDef],  # (1)
    customTransformationConfiguration: NotRequired[CustomTransformationConfigurationOutputTypeDef],  # (2)
    parsingConfiguration: NotRequired[ParsingConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: ChunkingConfigurationOutputTypeDef](./type_defs.md#chunkingconfigurationoutputtypedef)
2. See [:material-code-braces: CustomTransformationConfigurationOutputTypeDef](./type_defs.md#customtransformationconfigurationoutputtypedef)
3. See [:material-code-braces: ParsingConfigurationTypeDef](./type_defs.md#parsingconfigurationtypedef)

## VectorIngestionConfigurationTypeDef

```python
# VectorIngestionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import VectorIngestionConfigurationTypeDef


def get_value() -> VectorIngestionConfigurationTypeDef:
    return {
        "chunkingConfiguration": ...,
    }


# VectorIngestionConfigurationTypeDef definition

class VectorIngestionConfigurationTypeDef(TypedDict):
    chunkingConfiguration: NotRequired[ChunkingConfigurationTypeDef],  # (1)
    customTransformationConfiguration: NotRequired[CustomTransformationConfigurationTypeDef],  # (2)
    parsingConfiguration: NotRequired[ParsingConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: ChunkingConfigurationTypeDef](./type_defs.md#chunkingconfigurationtypedef)
2. See [:material-code-braces: CustomTransformationConfigurationTypeDef](./type_defs.md#customtransformationconfigurationtypedef)
3. See [:material-code-braces: ParsingConfigurationTypeDef](./type_defs.md#parsingconfigurationtypedef)

## KnowledgeBaseDocumentTypeDef

```python
# KnowledgeBaseDocumentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import KnowledgeBaseDocumentTypeDef


def get_value() -> KnowledgeBaseDocumentTypeDef:
    return {
        "content": ...,
    }


# KnowledgeBaseDocumentTypeDef definition

class KnowledgeBaseDocumentTypeDef(TypedDict):
    content: DocumentContentTypeDef,  # (1)
    metadata: NotRequired[DocumentMetadataTypeDef],  # (2)
```

1. See [:material-code-braces: DocumentContentTypeDef](./type_defs.md#documentcontenttypedef)
2. See [:material-code-braces: DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef)

## DataSourceConfigurationOutputTypeDef

```python
# DataSourceConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DataSourceConfigurationOutputTypeDef


def get_value() -> DataSourceConfigurationOutputTypeDef:
    return {
        "confluenceConfiguration": ...,
    }


# DataSourceConfigurationOutputTypeDef definition

class DataSourceConfigurationOutputTypeDef(TypedDict):
    type: DataSourceTypeType,  # (5)
    confluenceConfiguration: NotRequired[ConfluenceDataSourceConfigurationOutputTypeDef],  # (1)
    s3Configuration: NotRequired[S3DataSourceConfigurationOutputTypeDef],  # (2)
    salesforceConfiguration: NotRequired[SalesforceDataSourceConfigurationOutputTypeDef],  # (3)
    sharePointConfiguration: NotRequired[SharePointDataSourceConfigurationOutputTypeDef],  # (4)
    webConfiguration: NotRequired[WebDataSourceConfigurationOutputTypeDef],  # (6)
```

1. See [:material-code-braces: ConfluenceDataSourceConfigurationOutputTypeDef](./type_defs.md#confluencedatasourceconfigurationoutputtypedef)
2. See [:material-code-braces: S3DataSourceConfigurationOutputTypeDef](./type_defs.md#s3datasourceconfigurationoutputtypedef)
3. See [:material-code-braces: SalesforceDataSourceConfigurationOutputTypeDef](./type_defs.md#salesforcedatasourceconfigurationoutputtypedef)
4. See [:material-code-braces: SharePointDataSourceConfigurationOutputTypeDef](./type_defs.md#sharepointdatasourceconfigurationoutputtypedef)
5. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype)
6. See [:material-code-braces: WebDataSourceConfigurationOutputTypeDef](./type_defs.md#webdatasourceconfigurationoutputtypedef)

## DataSourceConfigurationTypeDef

```python
# DataSourceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DataSourceConfigurationTypeDef


def get_value() -> DataSourceConfigurationTypeDef:
    return {
        "confluenceConfiguration": ...,
    }


# DataSourceConfigurationTypeDef definition

class DataSourceConfigurationTypeDef(TypedDict):
    type: DataSourceTypeType,  # (5)
    confluenceConfiguration: NotRequired[ConfluenceDataSourceConfigurationTypeDef],  # (1)
    s3Configuration: NotRequired[S3DataSourceConfigurationTypeDef],  # (2)
    salesforceConfiguration: NotRequired[SalesforceDataSourceConfigurationTypeDef],  # (3)
    sharePointConfiguration: NotRequired[SharePointDataSourceConfigurationTypeDef],  # (4)
    webConfiguration: NotRequired[WebDataSourceConfigurationTypeDef],  # (6)
```

1. See [:material-code-braces: ConfluenceDataSourceConfigurationTypeDef](./type_defs.md#confluencedatasourceconfigurationtypedef)
2. See [:material-code-braces: S3DataSourceConfigurationTypeDef](./type_defs.md#s3datasourceconfigurationtypedef)
3. See [:material-code-braces: SalesforceDataSourceConfigurationTypeDef](./type_defs.md#salesforcedatasourceconfigurationtypedef)
4. See [:material-code-braces: SharePointDataSourceConfigurationTypeDef](./type_defs.md#sharepointdatasourceconfigurationtypedef)
5. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype)
6. See [:material-code-braces: WebDataSourceConfigurationTypeDef](./type_defs.md#webdatasourceconfigurationtypedef)

## SqlKnowledgeBaseConfigurationOutputTypeDef

```python
# SqlKnowledgeBaseConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import SqlKnowledgeBaseConfigurationOutputTypeDef


def get_value() -> SqlKnowledgeBaseConfigurationOutputTypeDef:
    return {
        "redshiftConfiguration": ...,
    }


# SqlKnowledgeBaseConfigurationOutputTypeDef definition

class SqlKnowledgeBaseConfigurationOutputTypeDef(TypedDict):
    type: QueryEngineTypeType,  # (2)
    redshiftConfiguration: NotRequired[RedshiftConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: RedshiftConfigurationOutputTypeDef](./type_defs.md#redshiftconfigurationoutputtypedef)
2. See [:material-code-brackets: QueryEngineTypeType](./literals.md#queryenginetypetype)

## SqlKnowledgeBaseConfigurationTypeDef

```python
# SqlKnowledgeBaseConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import SqlKnowledgeBaseConfigurationTypeDef


def get_value() -> SqlKnowledgeBaseConfigurationTypeDef:
    return {
        "redshiftConfiguration": ...,
    }


# SqlKnowledgeBaseConfigurationTypeDef definition

class SqlKnowledgeBaseConfigurationTypeDef(TypedDict):
    type: QueryEngineTypeType,  # (2)
    redshiftConfiguration: NotRequired[RedshiftConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: RedshiftConfigurationTypeDef](./type_defs.md#redshiftconfigurationtypedef)
2. See [:material-code-brackets: QueryEngineTypeType](./literals.md#queryenginetypetype)

## PromptTemplateConfigurationOutputTypeDef

```python
# PromptTemplateConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptTemplateConfigurationOutputTypeDef


def get_value() -> PromptTemplateConfigurationOutputTypeDef:
    return {
        "chat": ...,
    }


# PromptTemplateConfigurationOutputTypeDef definition

class PromptTemplateConfigurationOutputTypeDef(TypedDict):
    chat: NotRequired[ChatPromptTemplateConfigurationOutputTypeDef],  # (1)
    text: NotRequired[TextPromptTemplateConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ChatPromptTemplateConfigurationOutputTypeDef](./type_defs.md#chatprompttemplateconfigurationoutputtypedef)
2. See [:material-code-braces: TextPromptTemplateConfigurationOutputTypeDef](./type_defs.md#textprompttemplateconfigurationoutputtypedef)

## IngestKnowledgeBaseDocumentsRequestTypeDef

```python
# IngestKnowledgeBaseDocumentsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import IngestKnowledgeBaseDocumentsRequestTypeDef


def get_value() -> IngestKnowledgeBaseDocumentsRequestTypeDef:
    return {
        "dataSourceId": ...,
    }


# IngestKnowledgeBaseDocumentsRequestTypeDef definition

class IngestKnowledgeBaseDocumentsRequestTypeDef(TypedDict):
    dataSourceId: str,
    documents: Sequence[KnowledgeBaseDocumentTypeDef],  # (1)
    knowledgeBaseId: str,
    clientToken: NotRequired[str],
```

1. See `Sequence[KnowledgeBaseDocumentTypeDef]`

## DataSourceTypeDef

```python
# DataSourceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import DataSourceTypeDef


def get_value() -> DataSourceTypeDef:
    return {
        "createdAt": ...,
    }


# DataSourceTypeDef definition

class DataSourceTypeDef(TypedDict):
    createdAt: datetime.datetime,
    dataSourceConfiguration: DataSourceConfigurationOutputTypeDef,  # (2)
    dataSourceId: str,
    knowledgeBaseId: str,
    name: str,
    status: DataSourceStatusType,  # (4)
    updatedAt: datetime.datetime,
    dataDeletionPolicy: NotRequired[DataDeletionPolicyType],  # (1)
    description: NotRequired[str],
    failureReasons: NotRequired[List[str]],
    serverSideEncryptionConfiguration: NotRequired[ServerSideEncryptionConfigurationTypeDef],  # (3)
    vectorIngestionConfiguration: NotRequired[VectorIngestionConfigurationOutputTypeDef],  # (5)
```

1. See [:material-code-brackets: DataDeletionPolicyType](./literals.md#datadeletionpolicytype)
2. See [:material-code-braces: DataSourceConfigurationOutputTypeDef](./type_defs.md#datasourceconfigurationoutputtypedef)
3. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef)
4. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype)
5. See [:material-code-braces: VectorIngestionConfigurationOutputTypeDef](./type_defs.md#vectoringestionconfigurationoutputtypedef)

## KnowledgeBaseConfigurationOutputTypeDef

```python
# KnowledgeBaseConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import KnowledgeBaseConfigurationOutputTypeDef


def get_value() -> KnowledgeBaseConfigurationOutputTypeDef:
    return {
        "kendraKnowledgeBaseConfiguration": ...,
    }


# KnowledgeBaseConfigurationOutputTypeDef definition

class KnowledgeBaseConfigurationOutputTypeDef(TypedDict):
    type: KnowledgeBaseTypeType,  # (3)
    kendraKnowledgeBaseConfiguration: NotRequired[KendraKnowledgeBaseConfigurationTypeDef],  # (1)
    sqlKnowledgeBaseConfiguration: NotRequired[SqlKnowledgeBaseConfigurationOutputTypeDef],  # (2)
    vectorKnowledgeBaseConfiguration: NotRequired[VectorKnowledgeBaseConfigurationOutputTypeDef],  # (4)
```

1. See [:material-code-braces: KendraKnowledgeBaseConfigurationTypeDef](./type_defs.md#kendraknowledgebaseconfigurationtypedef)
2. See [:material-code-braces: SqlKnowledgeBaseConfigurationOutputTypeDef](./type_defs.md#sqlknowledgebaseconfigurationoutputtypedef)
3. See [:material-code-brackets: KnowledgeBaseTypeType](./literals.md#knowledgebasetypetype)
4. See [:material-code-braces: VectorKnowledgeBaseConfigurationOutputTypeDef](./type_defs.md#vectorknowledgebaseconfigurationoutputtypedef)

## KnowledgeBaseConfigurationTypeDef

```python
# KnowledgeBaseConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import KnowledgeBaseConfigurationTypeDef


def get_value() -> KnowledgeBaseConfigurationTypeDef:
    return {
        "kendraKnowledgeBaseConfiguration": ...,
    }


# KnowledgeBaseConfigurationTypeDef definition

class KnowledgeBaseConfigurationTypeDef(TypedDict):
    type: KnowledgeBaseTypeType,  # (3)
    kendraKnowledgeBaseConfiguration: NotRequired[KendraKnowledgeBaseConfigurationTypeDef],  # (1)
    sqlKnowledgeBaseConfiguration: NotRequired[SqlKnowledgeBaseConfigurationTypeDef],  # (2)
    vectorKnowledgeBaseConfiguration: NotRequired[VectorKnowledgeBaseConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: KendraKnowledgeBaseConfigurationTypeDef](./type_defs.md#kendraknowledgebaseconfigurationtypedef)
2. See [:material-code-braces: SqlKnowledgeBaseConfigurationTypeDef](./type_defs.md#sqlknowledgebaseconfigurationtypedef)
3. See [:material-code-brackets: KnowledgeBaseTypeType](./literals.md#knowledgebasetypetype)
4. See [:material-code-braces: VectorKnowledgeBaseConfigurationTypeDef](./type_defs.md#vectorknowledgebaseconfigurationtypedef)

## PromptFlowNodeInlineConfigurationOutputTypeDef

```python
# PromptFlowNodeInlineConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptFlowNodeInlineConfigurationOutputTypeDef


def get_value() -> PromptFlowNodeInlineConfigurationOutputTypeDef:
    return {
        "additionalModelRequestFields": ...,
    }


# PromptFlowNodeInlineConfigurationOutputTypeDef definition

class PromptFlowNodeInlineConfigurationOutputTypeDef(TypedDict):
    modelId: str,
    templateConfiguration: PromptTemplateConfigurationOutputTypeDef,  # (2)
    templateType: PromptTemplateTypeType,  # (3)
    additionalModelRequestFields: NotRequired[Dict[str, Any]],
    inferenceConfiguration: NotRequired[PromptInferenceConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: PromptInferenceConfigurationOutputTypeDef](./type_defs.md#promptinferenceconfigurationoutputtypedef)
2. See [:material-code-braces: PromptTemplateConfigurationOutputTypeDef](./type_defs.md#prompttemplateconfigurationoutputtypedef)
3. See [:material-code-brackets: PromptTemplateTypeType](./literals.md#prompttemplatetypetype)

## PromptVariantOutputTypeDef

```python
# PromptVariantOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptVariantOutputTypeDef


def get_value() -> PromptVariantOutputTypeDef:
    return {
        "additionalModelRequestFields": ...,
    }


# PromptVariantOutputTypeDef definition

class PromptVariantOutputTypeDef(TypedDict):
    name: str,
    templateConfiguration: PromptTemplateConfigurationOutputTypeDef,  # (4)
    templateType: PromptTemplateTypeType,  # (5)
    additionalModelRequestFields: NotRequired[Dict[str, Any]],
    genAiResource: NotRequired[PromptGenAiResourceTypeDef],  # (1)
    inferenceConfiguration: NotRequired[PromptInferenceConfigurationOutputTypeDef],  # (2)
    metadata: NotRequired[List[PromptMetadataEntryTypeDef]],  # (3)
    modelId: NotRequired[str],
```

1. See [:material-code-braces: PromptGenAiResourceTypeDef](./type_defs.md#promptgenairesourcetypedef)
2. See [:material-code-braces: PromptInferenceConfigurationOutputTypeDef](./type_defs.md#promptinferenceconfigurationoutputtypedef)
3. See `List[PromptMetadataEntryTypeDef]`
4. See [:material-code-braces: PromptTemplateConfigurationOutputTypeDef](./type_defs.md#prompttemplateconfigurationoutputtypedef)
5. See [:material-code-brackets: PromptTemplateTypeType](./literals.md#prompttemplatetypetype)

## ToolConfigurationTypeDef

```python
# ToolConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ToolConfigurationTypeDef


def get_value() -> ToolConfigurationTypeDef:
    return {
        "toolChoice": ...,
    }


# ToolConfigurationTypeDef definition

class ToolConfigurationTypeDef(TypedDict):
    tools: Sequence[ToolUnionTypeDef],  # (2)
    toolChoice: NotRequired[ToolChoiceUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ToolChoiceUnionTypeDef](#toolchoiceuniontypedef)
2. See `Sequence[ToolUnionTypeDef]`

## CreateDataSourceResponseTypeDef

```python
# CreateDataSourceResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CreateDataSourceResponseTypeDef


def get_value() -> CreateDataSourceResponseTypeDef:
    return {
        "dataSource": ...,
    }


# CreateDataSourceResponseTypeDef definition

class CreateDataSourceResponseTypeDef(TypedDict):
    dataSource: DataSourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetDataSourceResponseTypeDef

```python
# GetDataSourceResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetDataSourceResponseTypeDef


def get_value() -> GetDataSourceResponseTypeDef:
    return {
        "dataSource": ...,
    }


# GetDataSourceResponseTypeDef definition

class GetDataSourceResponseTypeDef(TypedDict):
    dataSource: DataSourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateDataSourceResponseTypeDef

```python
# UpdateDataSourceResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UpdateDataSourceResponseTypeDef


def get_value() -> UpdateDataSourceResponseTypeDef:
    return {
        "dataSource": ...,
    }


# UpdateDataSourceResponseTypeDef definition

class UpdateDataSourceResponseTypeDef(TypedDict):
    dataSource: DataSourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateDataSourceRequestTypeDef

```python
# CreateDataSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CreateDataSourceRequestTypeDef


def get_value() -> CreateDataSourceRequestTypeDef:
    return {
        "dataSourceConfiguration": ...,
    }


# CreateDataSourceRequestTypeDef definition

class CreateDataSourceRequestTypeDef(TypedDict):
    dataSourceConfiguration: DataSourceConfigurationUnionTypeDef,  # (1)
    knowledgeBaseId: str,
    name: str,
    clientToken: NotRequired[str],
    dataDeletionPolicy: NotRequired[DataDeletionPolicyType],  # (2)
    description: NotRequired[str],
    serverSideEncryptionConfiguration: NotRequired[ServerSideEncryptionConfigurationTypeDef],  # (3)
    vectorIngestionConfiguration: NotRequired[VectorIngestionConfigurationUnionTypeDef],  # (4)
```

1. See [:material-code-braces: DataSourceConfigurationUnionTypeDef](#datasourceconfigurationuniontypedef)
2. See [:material-code-brackets: DataDeletionPolicyType](./literals.md#datadeletionpolicytype)
3. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef)
4. See [:material-code-braces: VectorIngestionConfigurationUnionTypeDef](#vectoringestionconfigurationuniontypedef)

## UpdateDataSourceRequestTypeDef

```python
# UpdateDataSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UpdateDataSourceRequestTypeDef


def get_value() -> UpdateDataSourceRequestTypeDef:
    return {
        "dataSourceConfiguration": ...,
    }


# UpdateDataSourceRequestTypeDef definition

class UpdateDataSourceRequestTypeDef(TypedDict):
    dataSourceConfiguration: DataSourceConfigurationUnionTypeDef,  # (1)
    dataSourceId: str,
    knowledgeBaseId: str,
    name: str,
    dataDeletionPolicy: NotRequired[DataDeletionPolicyType],  # (2)
    description: NotRequired[str],
    serverSideEncryptionConfiguration: NotRequired[ServerSideEncryptionConfigurationTypeDef],  # (3)
    vectorIngestionConfiguration: NotRequired[VectorIngestionConfigurationUnionTypeDef],  # (4)
```

1. See [:material-code-braces: DataSourceConfigurationUnionTypeDef](#datasourceconfigurationuniontypedef)
2. See [:material-code-brackets: DataDeletionPolicyType](./literals.md#datadeletionpolicytype)
3. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef)
4. See [:material-code-braces: VectorIngestionConfigurationUnionTypeDef](#vectoringestionconfigurationuniontypedef)

## KnowledgeBaseTypeDef

```python
# KnowledgeBaseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import KnowledgeBaseTypeDef


def get_value() -> KnowledgeBaseTypeDef:
    return {
        "createdAt": ...,
    }


# KnowledgeBaseTypeDef definition

class KnowledgeBaseTypeDef(TypedDict):
    createdAt: datetime.datetime,
    knowledgeBaseArn: str,
    knowledgeBaseConfiguration: KnowledgeBaseConfigurationOutputTypeDef,  # (1)
    knowledgeBaseId: str,
    name: str,
    roleArn: str,
    status: KnowledgeBaseStatusType,  # (2)
    updatedAt: datetime.datetime,
    description: NotRequired[str],
    failureReasons: NotRequired[List[str]],
    storageConfiguration: NotRequired[StorageConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: KnowledgeBaseConfigurationOutputTypeDef](./type_defs.md#knowledgebaseconfigurationoutputtypedef)
2. See [:material-code-brackets: KnowledgeBaseStatusType](./literals.md#knowledgebasestatustype)
3. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef)

## PromptFlowNodeSourceConfigurationOutputTypeDef

```python
# PromptFlowNodeSourceConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptFlowNodeSourceConfigurationOutputTypeDef


def get_value() -> PromptFlowNodeSourceConfigurationOutputTypeDef:
    return {
        "inline": ...,
    }


# PromptFlowNodeSourceConfigurationOutputTypeDef definition

class PromptFlowNodeSourceConfigurationOutputTypeDef(TypedDict):
    inline: NotRequired[PromptFlowNodeInlineConfigurationOutputTypeDef],  # (1)
    resource: NotRequired[PromptFlowNodeResourceConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: PromptFlowNodeInlineConfigurationOutputTypeDef](./type_defs.md#promptflownodeinlineconfigurationoutputtypedef)
2. See [:material-code-braces: PromptFlowNodeResourceConfigurationTypeDef](./type_defs.md#promptflownoderesourceconfigurationtypedef)

## CreatePromptResponseTypeDef

```python
# CreatePromptResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CreatePromptResponseTypeDef


def get_value() -> CreatePromptResponseTypeDef:
    return {
        "arn": ...,
    }


# CreatePromptResponseTypeDef definition

class CreatePromptResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime.datetime,
    customerEncryptionKeyArn: str,
    defaultVariant: str,
    description: str,
    id: str,
    name: str,
    updatedAt: datetime.datetime,
    variants: List[PromptVariantOutputTypeDef],  # (1)
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `List[PromptVariantOutputTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreatePromptVersionResponseTypeDef

```python
# CreatePromptVersionResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CreatePromptVersionResponseTypeDef


def get_value() -> CreatePromptVersionResponseTypeDef:
    return {
        "arn": ...,
    }


# CreatePromptVersionResponseTypeDef definition

class CreatePromptVersionResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime.datetime,
    customerEncryptionKeyArn: str,
    defaultVariant: str,
    description: str,
    id: str,
    name: str,
    updatedAt: datetime.datetime,
    variants: List[PromptVariantOutputTypeDef],  # (1)
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `List[PromptVariantOutputTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetPromptResponseTypeDef

```python
# GetPromptResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetPromptResponseTypeDef


def get_value() -> GetPromptResponseTypeDef:
    return {
        "arn": ...,
    }


# GetPromptResponseTypeDef definition

class GetPromptResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime.datetime,
    customerEncryptionKeyArn: str,
    defaultVariant: str,
    description: str,
    id: str,
    name: str,
    updatedAt: datetime.datetime,
    variants: List[PromptVariantOutputTypeDef],  # (1)
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `List[PromptVariantOutputTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdatePromptResponseTypeDef

```python
# UpdatePromptResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UpdatePromptResponseTypeDef


def get_value() -> UpdatePromptResponseTypeDef:
    return {
        "arn": ...,
    }


# UpdatePromptResponseTypeDef definition

class UpdatePromptResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime.datetime,
    customerEncryptionKeyArn: str,
    defaultVariant: str,
    description: str,
    id: str,
    name: str,
    updatedAt: datetime.datetime,
    variants: List[PromptVariantOutputTypeDef],  # (1)
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `List[PromptVariantOutputTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateKnowledgeBaseResponseTypeDef

```python
# CreateKnowledgeBaseResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CreateKnowledgeBaseResponseTypeDef


def get_value() -> CreateKnowledgeBaseResponseTypeDef:
    return {
        "knowledgeBase": ...,
    }


# CreateKnowledgeBaseResponseTypeDef definition

class CreateKnowledgeBaseResponseTypeDef(TypedDict):
    knowledgeBase: KnowledgeBaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KnowledgeBaseTypeDef](./type_defs.md#knowledgebasetypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetKnowledgeBaseResponseTypeDef

```python
# GetKnowledgeBaseResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetKnowledgeBaseResponseTypeDef


def get_value() -> GetKnowledgeBaseResponseTypeDef:
    return {
        "knowledgeBase": ...,
    }


# GetKnowledgeBaseResponseTypeDef definition

class GetKnowledgeBaseResponseTypeDef(TypedDict):
    knowledgeBase: KnowledgeBaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KnowledgeBaseTypeDef](./type_defs.md#knowledgebasetypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateKnowledgeBaseResponseTypeDef

```python
# UpdateKnowledgeBaseResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UpdateKnowledgeBaseResponseTypeDef


def get_value() -> UpdateKnowledgeBaseResponseTypeDef:
    return {
        "knowledgeBase": ...,
    }


# UpdateKnowledgeBaseResponseTypeDef definition

class UpdateKnowledgeBaseResponseTypeDef(TypedDict):
    knowledgeBase: KnowledgeBaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KnowledgeBaseTypeDef](./type_defs.md#knowledgebasetypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateKnowledgeBaseRequestTypeDef

```python
# CreateKnowledgeBaseRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CreateKnowledgeBaseRequestTypeDef


def get_value() -> CreateKnowledgeBaseRequestTypeDef:
    return {
        "knowledgeBaseConfiguration": ...,
    }


# CreateKnowledgeBaseRequestTypeDef definition

class CreateKnowledgeBaseRequestTypeDef(TypedDict):
    knowledgeBaseConfiguration: KnowledgeBaseConfigurationUnionTypeDef,  # (1)
    name: str,
    roleArn: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    storageConfiguration: NotRequired[StorageConfigurationTypeDef],  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: KnowledgeBaseConfigurationUnionTypeDef](#knowledgebaseconfigurationuniontypedef)
2. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef)

## UpdateKnowledgeBaseRequestTypeDef

```python
# UpdateKnowledgeBaseRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UpdateKnowledgeBaseRequestTypeDef


def get_value() -> UpdateKnowledgeBaseRequestTypeDef:
    return {
        "knowledgeBaseConfiguration": ...,
    }


# UpdateKnowledgeBaseRequestTypeDef definition

class UpdateKnowledgeBaseRequestTypeDef(TypedDict):
    knowledgeBaseConfiguration: KnowledgeBaseConfigurationUnionTypeDef,  # (1)
    knowledgeBaseId: str,
    name: str,
    roleArn: str,
    description: NotRequired[str],
    storageConfiguration: NotRequired[StorageConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: KnowledgeBaseConfigurationUnionTypeDef](#knowledgebaseconfigurationuniontypedef)
2. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef)

## PromptFlowNodeConfigurationOutputTypeDef

```python
# PromptFlowNodeConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptFlowNodeConfigurationOutputTypeDef


def get_value() -> PromptFlowNodeConfigurationOutputTypeDef:
    return {
        "guardrailConfiguration": ...,
    }


# PromptFlowNodeConfigurationOutputTypeDef definition

class PromptFlowNodeConfigurationOutputTypeDef(TypedDict):
    sourceConfiguration: PromptFlowNodeSourceConfigurationOutputTypeDef,  # (2)
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef)
2. See [:material-code-braces: PromptFlowNodeSourceConfigurationOutputTypeDef](./type_defs.md#promptflownodesourceconfigurationoutputtypedef)

## ChatPromptTemplateConfigurationTypeDef

```python
# ChatPromptTemplateConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ChatPromptTemplateConfigurationTypeDef


def get_value() -> ChatPromptTemplateConfigurationTypeDef:
    return {
        "inputVariables": ...,
    }


# ChatPromptTemplateConfigurationTypeDef definition

class ChatPromptTemplateConfigurationTypeDef(TypedDict):
    messages: Sequence[MessageUnionTypeDef],  # (2)
    inputVariables: NotRequired[Sequence[PromptInputVariableTypeDef]],  # (1)
    system: NotRequired[Sequence[SystemContentBlockTypeDef]],  # (3)
    toolConfiguration: NotRequired[ToolConfigurationUnionTypeDef],  # (4)
```

1. See `Sequence[PromptInputVariableTypeDef]`
2. See `Sequence[MessageUnionTypeDef]`
3. See `Sequence[SystemContentBlockTypeDef]`
4. See [:material-code-braces: ToolConfigurationUnionTypeDef](#toolconfigurationuniontypedef)

## FlowNodeConfigurationOutputTypeDef

```python
# FlowNodeConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FlowNodeConfigurationOutputTypeDef


def get_value() -> FlowNodeConfigurationOutputTypeDef:
    return {
        "agent": ...,
    }


# FlowNodeConfigurationOutputTypeDef definition

class FlowNodeConfigurationOutputTypeDef(TypedDict):
    agent: NotRequired[AgentFlowNodeConfigurationTypeDef],  # (1)
    collector: NotRequired[Dict[str, Any]],
    condition: NotRequired[ConditionFlowNodeConfigurationOutputTypeDef],  # (2)
    input: NotRequired[Dict[str, Any]],
    iterator: NotRequired[Dict[str, Any]],
    knowledgeBase: NotRequired[KnowledgeBaseFlowNodeConfigurationTypeDef],  # (3)
    lambdaFunction: NotRequired[LambdaFunctionFlowNodeConfigurationTypeDef],  # (4)
    lex: NotRequired[LexFlowNodeConfigurationTypeDef],  # (5)
    output: NotRequired[Dict[str, Any]],
    prompt: NotRequired[PromptFlowNodeConfigurationOutputTypeDef],  # (6)
    retrieval: NotRequired[RetrievalFlowNodeConfigurationTypeDef],  # (7)
    storage: NotRequired[StorageFlowNodeConfigurationTypeDef],  # (8)
```

1. See [:material-code-braces: AgentFlowNodeConfigurationTypeDef](./type_defs.md#agentflownodeconfigurationtypedef)
2. See [:material-code-braces: ConditionFlowNodeConfigurationOutputTypeDef](./type_defs.md#conditionflownodeconfigurationoutputtypedef)
3. See [:material-code-braces: KnowledgeBaseFlowNodeConfigurationTypeDef](./type_defs.md#knowledgebaseflownodeconfigurationtypedef)
4. See [:material-code-braces: LambdaFunctionFlowNodeConfigurationTypeDef](./type_defs.md#lambdafunctionflownodeconfigurationtypedef)
5. See [:material-code-braces: LexFlowNodeConfigurationTypeDef](./type_defs.md#lexflownodeconfigurationtypedef)
6. See [:material-code-braces: PromptFlowNodeConfigurationOutputTypeDef](./type_defs.md#promptflownodeconfigurationoutputtypedef)
7. See [:material-code-braces: RetrievalFlowNodeConfigurationTypeDef](./type_defs.md#retrievalflownodeconfigurationtypedef)
8. See [:material-code-braces: StorageFlowNodeConfigurationTypeDef](./type_defs.md#storageflownodeconfigurationtypedef)

## FlowNodeExtraTypeDef

```python
# FlowNodeExtraTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FlowNodeExtraTypeDef


def get_value() -> FlowNodeExtraTypeDef:
    return {
        "configuration": ...,
    }


# FlowNodeExtraTypeDef definition

class FlowNodeExtraTypeDef(TypedDict):
    name: str,
    type: FlowNodeTypeType,  # (4)
    configuration: NotRequired[FlowNodeConfigurationOutputTypeDef],  # (1)
    inputs: NotRequired[List[FlowNodeInputTypeDef]],  # (2)
    outputs: NotRequired[List[FlowNodeOutputTypeDef]],  # (3)
```

1. See [:material-code-braces: FlowNodeConfigurationOutputTypeDef](./type_defs.md#flownodeconfigurationoutputtypedef)
2. See `List[FlowNodeInputTypeDef]`
3. See `List[FlowNodeOutputTypeDef]`
4. See [:material-code-brackets: FlowNodeTypeType](./literals.md#flownodetypetype)

## PromptTemplateConfigurationTypeDef

```python
# PromptTemplateConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptTemplateConfigurationTypeDef


def get_value() -> PromptTemplateConfigurationTypeDef:
    return {
        "chat": ...,
    }


# PromptTemplateConfigurationTypeDef definition

class PromptTemplateConfigurationTypeDef(TypedDict):
    chat: NotRequired[ChatPromptTemplateConfigurationUnionTypeDef],  # (1)
    text: NotRequired[TextPromptTemplateConfigurationUnionTypeDef],  # (2)
```

1. See [:material-code-braces: ChatPromptTemplateConfigurationUnionTypeDef](#chatprompttemplateconfigurationuniontypedef)
2. See [:material-code-braces: TextPromptTemplateConfigurationUnionTypeDef](#textprompttemplateconfigurationuniontypedef)

## FlowDefinitionOutputTypeDef

```python
# FlowDefinitionOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FlowDefinitionOutputTypeDef


def get_value() -> FlowDefinitionOutputTypeDef:
    return {
        "connections": ...,
    }


# FlowDefinitionOutputTypeDef definition

class FlowDefinitionOutputTypeDef(TypedDict):
    connections: NotRequired[List[FlowConnectionTypeDef]],  # (1)
    nodes: NotRequired[List[FlowNodeExtraTypeDef]],  # (2)
```

1. See `List[FlowConnectionTypeDef]`
2. See `List[FlowNodeExtraTypeDef]`

## PromptFlowNodeInlineConfigurationTypeDef

```python
# PromptFlowNodeInlineConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptFlowNodeInlineConfigurationTypeDef


def get_value() -> PromptFlowNodeInlineConfigurationTypeDef:
    return {
        "additionalModelRequestFields": ...,
    }


# PromptFlowNodeInlineConfigurationTypeDef definition

class PromptFlowNodeInlineConfigurationTypeDef(TypedDict):
    modelId: str,
    templateConfiguration: PromptTemplateConfigurationTypeDef,  # (2)
    templateType: PromptTemplateTypeType,  # (3)
    additionalModelRequestFields: NotRequired[Mapping[str, Any]],
    inferenceConfiguration: NotRequired[PromptInferenceConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: PromptInferenceConfigurationTypeDef](./type_defs.md#promptinferenceconfigurationtypedef)
2. See [:material-code-braces: PromptTemplateConfigurationTypeDef](./type_defs.md#prompttemplateconfigurationtypedef)
3. See [:material-code-brackets: PromptTemplateTypeType](./literals.md#prompttemplatetypetype)

## CreateFlowResponseTypeDef

```python
# CreateFlowResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CreateFlowResponseTypeDef


def get_value() -> CreateFlowResponseTypeDef:
    return {
        "arn": ...,
    }


# CreateFlowResponseTypeDef definition

class CreateFlowResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime.datetime,
    customerEncryptionKeyArn: str,
    definition: FlowDefinitionOutputTypeDef,  # (1)
    description: str,
    executionRoleArn: str,
    id: str,
    name: str,
    status: FlowStatusType,  # (2)
    updatedAt: datetime.datetime,
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FlowDefinitionOutputTypeDef](./type_defs.md#flowdefinitionoutputtypedef)
2. See [:material-code-brackets: FlowStatusType](./literals.md#flowstatustype)
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateFlowVersionResponseTypeDef

```python
# CreateFlowVersionResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CreateFlowVersionResponseTypeDef


def get_value() -> CreateFlowVersionResponseTypeDef:
    return {
        "arn": ...,
    }


# CreateFlowVersionResponseTypeDef definition

class CreateFlowVersionResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime.datetime,
    customerEncryptionKeyArn: str,
    definition: FlowDefinitionOutputTypeDef,  # (1)
    description: str,
    executionRoleArn: str,
    id: str,
    name: str,
    status: FlowStatusType,  # (2)
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FlowDefinitionOutputTypeDef](./type_defs.md#flowdefinitionoutputtypedef)
2. See [:material-code-brackets: FlowStatusType](./literals.md#flowstatustype)
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetFlowResponseTypeDef

```python
# GetFlowResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetFlowResponseTypeDef


def get_value() -> GetFlowResponseTypeDef:
    return {
        "arn": ...,
    }


# GetFlowResponseTypeDef definition

class GetFlowResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime.datetime,
    customerEncryptionKeyArn: str,
    definition: FlowDefinitionOutputTypeDef,  # (1)
    description: str,
    executionRoleArn: str,
    id: str,
    name: str,
    status: FlowStatusType,  # (2)
    updatedAt: datetime.datetime,
    validations: List[FlowValidationTypeDef],  # (3)
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: FlowDefinitionOutputTypeDef](./type_defs.md#flowdefinitionoutputtypedef)
2. See [:material-code-brackets: FlowStatusType](./literals.md#flowstatustype)
3. See `List[FlowValidationTypeDef]`
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetFlowVersionResponseTypeDef

```python
# GetFlowVersionResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import GetFlowVersionResponseTypeDef


def get_value() -> GetFlowVersionResponseTypeDef:
    return {
        "arn": ...,
    }


# GetFlowVersionResponseTypeDef definition

class GetFlowVersionResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime.datetime,
    customerEncryptionKeyArn: str,
    definition: FlowDefinitionOutputTypeDef,  # (1)
    description: str,
    executionRoleArn: str,
    id: str,
    name: str,
    status: FlowStatusType,  # (2)
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FlowDefinitionOutputTypeDef](./type_defs.md#flowdefinitionoutputtypedef)
2. See [:material-code-brackets: FlowStatusType](./literals.md#flowstatustype)
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateFlowResponseTypeDef

```python
# UpdateFlowResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UpdateFlowResponseTypeDef


def get_value() -> UpdateFlowResponseTypeDef:
    return {
        "arn": ...,
    }


# UpdateFlowResponseTypeDef definition

class UpdateFlowResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime.datetime,
    customerEncryptionKeyArn: str,
    definition: FlowDefinitionOutputTypeDef,  # (1)
    description: str,
    executionRoleArn: str,
    id: str,
    name: str,
    status: FlowStatusType,  # (2)
    updatedAt: datetime.datetime,
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FlowDefinitionOutputTypeDef](./type_defs.md#flowdefinitionoutputtypedef)
2. See [:material-code-brackets: FlowStatusType](./literals.md#flowstatustype)
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## PromptFlowNodeSourceConfigurationTypeDef

```python
# PromptFlowNodeSourceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptFlowNodeSourceConfigurationTypeDef


def get_value() -> PromptFlowNodeSourceConfigurationTypeDef:
    return {
        "inline": ...,
    }


# PromptFlowNodeSourceConfigurationTypeDef definition

class PromptFlowNodeSourceConfigurationTypeDef(TypedDict):
    inline: NotRequired[PromptFlowNodeInlineConfigurationTypeDef],  # (1)
    resource: NotRequired[PromptFlowNodeResourceConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: PromptFlowNodeInlineConfigurationTypeDef](./type_defs.md#promptflownodeinlineconfigurationtypedef)
2. See [:material-code-braces: PromptFlowNodeResourceConfigurationTypeDef](./type_defs.md#promptflownoderesourceconfigurationtypedef)

## PromptVariantTypeDef

```python
# PromptVariantTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptVariantTypeDef


def get_value() -> PromptVariantTypeDef:
    return {
        "additionalModelRequestFields": ...,
    }


# PromptVariantTypeDef definition

class PromptVariantTypeDef(TypedDict):
    name: str,
    templateConfiguration: PromptTemplateConfigurationUnionTypeDef,  # (4)
    templateType: PromptTemplateTypeType,  # (5)
    additionalModelRequestFields: NotRequired[Mapping[str, Any]],
    genAiResource: NotRequired[PromptGenAiResourceTypeDef],  # (1)
    inferenceConfiguration: NotRequired[PromptInferenceConfigurationUnionTypeDef],  # (2)
    metadata: NotRequired[Sequence[PromptMetadataEntryTypeDef]],  # (3)
    modelId: NotRequired[str],
```

1. See [:material-code-braces: PromptGenAiResourceTypeDef](./type_defs.md#promptgenairesourcetypedef)
2. See [:material-code-braces: PromptInferenceConfigurationUnionTypeDef](#promptinferenceconfigurationuniontypedef)
3. See `Sequence[PromptMetadataEntryTypeDef]`
4. See [:material-code-braces: PromptTemplateConfigurationUnionTypeDef](#prompttemplateconfigurationuniontypedef)
5. See [:material-code-brackets: PromptTemplateTypeType](./literals.md#prompttemplatetypetype)

## PromptFlowNodeConfigurationTypeDef

```python
# PromptFlowNodeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import PromptFlowNodeConfigurationTypeDef


def get_value() -> PromptFlowNodeConfigurationTypeDef:
    return {
        "guardrailConfiguration": ...,
    }


# PromptFlowNodeConfigurationTypeDef definition

class PromptFlowNodeConfigurationTypeDef(TypedDict):
    sourceConfiguration: PromptFlowNodeSourceConfigurationTypeDef,  # (2)
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef)
2. See [:material-code-braces: PromptFlowNodeSourceConfigurationTypeDef](./type_defs.md#promptflownodesourceconfigurationtypedef)

## FlowNodeConfigurationTypeDef

```python
# FlowNodeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FlowNodeConfigurationTypeDef


def get_value() -> FlowNodeConfigurationTypeDef:
    return {
        "agent": ...,
    }


# FlowNodeConfigurationTypeDef definition

class FlowNodeConfigurationTypeDef(TypedDict):
    agent: NotRequired[AgentFlowNodeConfigurationTypeDef],  # (1)
    collector: NotRequired[Mapping[str, Any]],
    condition: NotRequired[ConditionFlowNodeConfigurationTypeDef],  # (2)
    input: NotRequired[Mapping[str, Any]],
    iterator: NotRequired[Mapping[str, Any]],
    knowledgeBase: NotRequired[KnowledgeBaseFlowNodeConfigurationTypeDef],  # (3)
    lambdaFunction: NotRequired[LambdaFunctionFlowNodeConfigurationTypeDef],  # (4)
    lex: NotRequired[LexFlowNodeConfigurationTypeDef],  # (5)
    output: NotRequired[Mapping[str, Any]],
    prompt: NotRequired[PromptFlowNodeConfigurationTypeDef],  # (6)
    retrieval: NotRequired[RetrievalFlowNodeConfigurationTypeDef],  # (7)
    storage: NotRequired[StorageFlowNodeConfigurationTypeDef],  # (8)
```

1. See [:material-code-braces: AgentFlowNodeConfigurationTypeDef](./type_defs.md#agentflownodeconfigurationtypedef)
2. See [:material-code-braces: ConditionFlowNodeConfigurationTypeDef](./type_defs.md#conditionflownodeconfigurationtypedef)
3. See [:material-code-braces: KnowledgeBaseFlowNodeConfigurationTypeDef](./type_defs.md#knowledgebaseflownodeconfigurationtypedef)
4. See [:material-code-braces: LambdaFunctionFlowNodeConfigurationTypeDef](./type_defs.md#lambdafunctionflownodeconfigurationtypedef)
5. See [:material-code-braces: LexFlowNodeConfigurationTypeDef](./type_defs.md#lexflownodeconfigurationtypedef)
6. See [:material-code-braces: PromptFlowNodeConfigurationTypeDef](./type_defs.md#promptflownodeconfigurationtypedef)
7. See [:material-code-braces: RetrievalFlowNodeConfigurationTypeDef](./type_defs.md#retrievalflownodeconfigurationtypedef)
8. See [:material-code-braces: StorageFlowNodeConfigurationTypeDef](./type_defs.md#storageflownodeconfigurationtypedef)

## CreatePromptRequestTypeDef

```python
# CreatePromptRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CreatePromptRequestTypeDef


def get_value() -> CreatePromptRequestTypeDef:
    return {
        "name": ...,
    }


# CreatePromptRequestTypeDef definition

class CreatePromptRequestTypeDef(TypedDict):
    name: str,
    clientToken: NotRequired[str],
    customerEncryptionKeyArn: NotRequired[str],
    defaultVariant: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    variants: NotRequired[Sequence[PromptVariantUnionTypeDef]],  # (1)
```

1. See `Sequence[PromptVariantUnionTypeDef]`

## UpdatePromptRequestTypeDef

```python
# UpdatePromptRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UpdatePromptRequestTypeDef


def get_value() -> UpdatePromptRequestTypeDef:
    return {
        "name": ...,
    }


# UpdatePromptRequestTypeDef definition

class UpdatePromptRequestTypeDef(TypedDict):
    name: str,
    promptIdentifier: str,
    customerEncryptionKeyArn: NotRequired[str],
    defaultVariant: NotRequired[str],
    description: NotRequired[str],
    variants: NotRequired[Sequence[PromptVariantUnionTypeDef]],  # (1)
```

1. See `Sequence[PromptVariantUnionTypeDef]`

## FlowNodeTypeDef

```python
# FlowNodeTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FlowNodeTypeDef


def get_value() -> FlowNodeTypeDef:
    return {
        "configuration": ...,
    }


# FlowNodeTypeDef definition

class FlowNodeTypeDef(TypedDict):
    name: str,
    type: FlowNodeTypeType,  # (4)
    configuration: NotRequired[FlowNodeConfigurationTypeDef],  # (1)
    inputs: NotRequired[Sequence[FlowNodeInputTypeDef]],  # (2)
    outputs: NotRequired[Sequence[FlowNodeOutputTypeDef]],  # (3)
```

1. See [:material-code-braces: FlowNodeConfigurationTypeDef](./type_defs.md#flownodeconfigurationtypedef)
2. See `Sequence[FlowNodeInputTypeDef]`
3. See `Sequence[FlowNodeOutputTypeDef]`
4. See [:material-code-brackets: FlowNodeTypeType](./literals.md#flownodetypetype)

## FlowDefinitionTypeDef

```python
# FlowDefinitionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import FlowDefinitionTypeDef


def get_value() -> FlowDefinitionTypeDef:
    return {
        "connections": ...,
    }


# FlowDefinitionTypeDef definition

class FlowDefinitionTypeDef(TypedDict):
    connections: NotRequired[Sequence[FlowConnectionTypeDef]],  # (1)
    nodes: NotRequired[Sequence[FlowNodeTypeDef]],  # (2)
```

1. See `Sequence[FlowConnectionTypeDef]`
2. See `Sequence[FlowNodeTypeDef]`

## CreateFlowRequestTypeDef

```python
# CreateFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import CreateFlowRequestTypeDef


def get_value() -> CreateFlowRequestTypeDef:
    return {
        "executionRoleArn": ...,
    }


# CreateFlowRequestTypeDef definition

class CreateFlowRequestTypeDef(TypedDict):
    executionRoleArn: str,
    name: str,
    clientToken: NotRequired[str],
    customerEncryptionKeyArn: NotRequired[str],
    definition: NotRequired[FlowDefinitionUnionTypeDef],  # (1)
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: FlowDefinitionUnionTypeDef](#flowdefinitionuniontypedef)

## UpdateFlowRequestTypeDef

```python
# UpdateFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import UpdateFlowRequestTypeDef


def get_value() -> UpdateFlowRequestTypeDef:
    return {
        "executionRoleArn": ...,
    }


# UpdateFlowRequestTypeDef definition

class UpdateFlowRequestTypeDef(TypedDict):
    executionRoleArn: str,
    flowIdentifier: str,
    name: str,
    customerEncryptionKeyArn: NotRequired[str],
    definition: NotRequired[FlowDefinitionUnionTypeDef],  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: FlowDefinitionUnionTypeDef](#flowdefinitionuniontypedef)

## ValidateFlowDefinitionRequestTypeDef

```python
# ValidateFlowDefinitionRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent.type_defs import ValidateFlowDefinitionRequestTypeDef


def get_value() -> ValidateFlowDefinitionRequestTypeDef:
    return {
        "definition": ...,
    }


# ValidateFlowDefinitionRequestTypeDef definition

class ValidateFlowDefinitionRequestTypeDef(TypedDict):
    definition: FlowDefinitionUnionTypeDef,  # (1)
```

1. See [:material-code-braces: FlowDefinitionUnionTypeDef](#flowdefinitionuniontypedef)

