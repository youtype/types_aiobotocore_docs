# Literals

> [Index](../README.md) > [AgentsforBedrockRuntime](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [AgentsforBedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#agentsforbedrockruntime)
    type annotations stubs module [types-aiobotocore-bedrock-agent-runtime](https://pypi.org/project/types-aiobotocore-bedrock-agent-runtime/).

## ActionGroupSignatureType

```python
# ActionGroupSignatureType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import ActionGroupSignatureType

def get_value() -> ActionGroupSignatureType:
    return "AMAZON.CodeInterpreter"
```

```python
# ActionGroupSignatureType definition
ActionGroupSignatureType = Literal[
    "AMAZON.CodeInterpreter",
    "AMAZON.UserInput",
    "ANTHROPIC.Bash",
    "ANTHROPIC.Computer",
    "ANTHROPIC.TextEditor",
]
```
## ActionInvocationTypeType

```python
# ActionInvocationTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import ActionInvocationTypeType

def get_value() -> ActionInvocationTypeType:
    return "RESULT"
```

```python
# ActionInvocationTypeType definition
ActionInvocationTypeType = Literal[
    "RESULT",
    "USER_CONFIRMATION",
    "USER_CONFIRMATION_AND_RESULT",
]
```
## AgentCollaborationType

```python
# AgentCollaborationType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import AgentCollaborationType

def get_value() -> AgentCollaborationType:
    return "DISABLED"
```

```python
# AgentCollaborationType definition
AgentCollaborationType = Literal[
    "DISABLED",
    "SUPERVISOR",
    "SUPERVISOR_ROUTER",
]
```
## AttributeTypeType

```python
# AttributeTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import AttributeTypeType

def get_value() -> AttributeTypeType:
    return "BOOLEAN"
```

```python
# AttributeTypeType definition
AttributeTypeType = Literal[
    "BOOLEAN",
    "NUMBER",
    "STRING",
    "STRING_LIST",
]
```
## ConfirmationStateType

```python
# ConfirmationStateType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import ConfirmationStateType

def get_value() -> ConfirmationStateType:
    return "CONFIRM"
```

```python
# ConfirmationStateType definition
ConfirmationStateType = Literal[
    "CONFIRM",
    "DENY",
]
```
## ConversationRoleType

```python
# ConversationRoleType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import ConversationRoleType

def get_value() -> ConversationRoleType:
    return "assistant"
```

```python
# ConversationRoleType definition
ConversationRoleType = Literal[
    "assistant",
    "user",
]
```
## CreationModeType

```python
# CreationModeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import CreationModeType

def get_value() -> CreationModeType:
    return "DEFAULT"
```

```python
# CreationModeType definition
CreationModeType = Literal[
    "DEFAULT",
    "OVERRIDDEN",
]
```
## CustomControlMethodType

```python
# CustomControlMethodType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import CustomControlMethodType

def get_value() -> CustomControlMethodType:
    return "RETURN_CONTROL"
```

```python
# CustomControlMethodType definition
CustomControlMethodType = Literal[
    "RETURN_CONTROL",
]
```
## ExecutionTypeType

```python
# ExecutionTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import ExecutionTypeType

def get_value() -> ExecutionTypeType:
    return "LAMBDA"
```

```python
# ExecutionTypeType definition
ExecutionTypeType = Literal[
    "LAMBDA",
    "RETURN_CONTROL",
]
```
## ExternalSourceTypeType

```python
# ExternalSourceTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import ExternalSourceTypeType

def get_value() -> ExternalSourceTypeType:
    return "BYTE_CONTENT"
```

```python
# ExternalSourceTypeType definition
ExternalSourceTypeType = Literal[
    "BYTE_CONTENT",
    "S3",
]
```
## FileSourceTypeType

```python
# FileSourceTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import FileSourceTypeType

def get_value() -> FileSourceTypeType:
    return "BYTE_CONTENT"
```

```python
# FileSourceTypeType definition
FileSourceTypeType = Literal[
    "BYTE_CONTENT",
    "S3",
]
```
## FileUseCaseType

```python
# FileUseCaseType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import FileUseCaseType

def get_value() -> FileUseCaseType:
    return "CHAT"
```

```python
# FileUseCaseType definition
FileUseCaseType = Literal[
    "CHAT",
    "CODE_INTERPRETER",
]
```
## FlowCompletionReasonType

```python
# FlowCompletionReasonType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import FlowCompletionReasonType

def get_value() -> FlowCompletionReasonType:
    return "INPUT_REQUIRED"
```

```python
# FlowCompletionReasonType definition
FlowCompletionReasonType = Literal[
    "INPUT_REQUIRED",
    "SUCCESS",
]
```
## FlowControlNodeTypeType

```python
# FlowControlNodeTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import FlowControlNodeTypeType

def get_value() -> FlowControlNodeTypeType:
    return "Iterator"
```

```python
# FlowControlNodeTypeType definition
FlowControlNodeTypeType = Literal[
    "Iterator",
    "Loop",
]
```
## FlowErrorCodeType

```python
# FlowErrorCodeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import FlowErrorCodeType

def get_value() -> FlowErrorCodeType:
    return "INTERNAL_SERVER"
```

```python
# FlowErrorCodeType definition
FlowErrorCodeType = Literal[
    "INTERNAL_SERVER",
    "NODE_EXECUTION_FAILED",
    "VALIDATION",
]
```
## FlowExecutionErrorTypeType

```python
# FlowExecutionErrorTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import FlowExecutionErrorTypeType

def get_value() -> FlowExecutionErrorTypeType:
    return "ExecutionTimedOut"
```

```python
# FlowExecutionErrorTypeType definition
FlowExecutionErrorTypeType = Literal[
    "ExecutionTimedOut",
]
```
## FlowExecutionEventTypeType

```python
# FlowExecutionEventTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import FlowExecutionEventTypeType

def get_value() -> FlowExecutionEventTypeType:
    return "Flow"
```

```python
# FlowExecutionEventTypeType definition
FlowExecutionEventTypeType = Literal[
    "Flow",
    "Node",
]
```
## FlowExecutionStatusType

```python
# FlowExecutionStatusType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import FlowExecutionStatusType

def get_value() -> FlowExecutionStatusType:
    return "Aborted"
```

```python
# FlowExecutionStatusType definition
FlowExecutionStatusType = Literal[
    "Aborted",
    "Failed",
    "Running",
    "Succeeded",
    "TimedOut",
]
```
## FlowNodeIODataTypeType

```python
# FlowNodeIODataTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import FlowNodeIODataTypeType

def get_value() -> FlowNodeIODataTypeType:
    return "Array"
```

```python
# FlowNodeIODataTypeType definition
FlowNodeIODataTypeType = Literal[
    "Array",
    "Boolean",
    "Number",
    "Object",
    "String",
]
```
## FlowNodeInputCategoryType

```python
# FlowNodeInputCategoryType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import FlowNodeInputCategoryType

def get_value() -> FlowNodeInputCategoryType:
    return "ExitLoop"
```

```python
# FlowNodeInputCategoryType definition
FlowNodeInputCategoryType = Literal[
    "ExitLoop",
    "LoopCondition",
    "ReturnValueToLoopStart",
]
```
## GeneratedQueryTypeType

```python
# GeneratedQueryTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import GeneratedQueryTypeType

def get_value() -> GeneratedQueryTypeType:
    return "REDSHIFT_SQL"
```

```python
# GeneratedQueryTypeType definition
GeneratedQueryTypeType = Literal[
    "REDSHIFT_SQL",
]
```
## GetAgentMemoryPaginatorName

```python
# GetAgentMemoryPaginatorName usage example
from types_aiobotocore_bedrock_agent_runtime.literals import GetAgentMemoryPaginatorName

def get_value() -> GetAgentMemoryPaginatorName:
    return "get_agent_memory"
```

```python
# GetAgentMemoryPaginatorName definition
GetAgentMemoryPaginatorName = Literal[
    "get_agent_memory",
]
```
## GuadrailActionType

```python
# GuadrailActionType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import GuadrailActionType

def get_value() -> GuadrailActionType:
    return "INTERVENED"
```

```python
# GuadrailActionType definition
GuadrailActionType = Literal[
    "INTERVENED",
    "NONE",
]
```
## GuardrailActionType

```python
# GuardrailActionType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import GuardrailActionType

def get_value() -> GuardrailActionType:
    return "INTERVENED"
```

```python
# GuardrailActionType definition
GuardrailActionType = Literal[
    "INTERVENED",
    "NONE",
]
```
## GuardrailContentFilterConfidenceType

```python
# GuardrailContentFilterConfidenceType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import GuardrailContentFilterConfidenceType

def get_value() -> GuardrailContentFilterConfidenceType:
    return "HIGH"
```

```python
# GuardrailContentFilterConfidenceType definition
GuardrailContentFilterConfidenceType = Literal[
    "HIGH",
    "LOW",
    "MEDIUM",
    "NONE",
]
```
## GuardrailContentFilterTypeType

```python
# GuardrailContentFilterTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import GuardrailContentFilterTypeType

def get_value() -> GuardrailContentFilterTypeType:
    return "HATE"
```

```python
# GuardrailContentFilterTypeType definition
GuardrailContentFilterTypeType = Literal[
    "HATE",
    "INSULTS",
    "MISCONDUCT",
    "PROMPT_ATTACK",
    "SEXUAL",
    "VIOLENCE",
]
```
## GuardrailContentPolicyActionType

```python
# GuardrailContentPolicyActionType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import GuardrailContentPolicyActionType

def get_value() -> GuardrailContentPolicyActionType:
    return "BLOCKED"
```

```python
# GuardrailContentPolicyActionType definition
GuardrailContentPolicyActionType = Literal[
    "BLOCKED",
]
```
## GuardrailManagedWordTypeType

```python
# GuardrailManagedWordTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import GuardrailManagedWordTypeType

def get_value() -> GuardrailManagedWordTypeType:
    return "PROFANITY"
```

```python
# GuardrailManagedWordTypeType definition
GuardrailManagedWordTypeType = Literal[
    "PROFANITY",
]
```
## GuardrailPiiEntityTypeType

```python
# GuardrailPiiEntityTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import GuardrailPiiEntityTypeType

def get_value() -> GuardrailPiiEntityTypeType:
    return "ADDRESS"
```

```python
# GuardrailPiiEntityTypeType definition
GuardrailPiiEntityTypeType = Literal[
    "ADDRESS",
    "AGE",
    "AWS_ACCESS_KEY",
    "AWS_SECRET_KEY",
    "CA_HEALTH_NUMBER",
    "CA_SOCIAL_INSURANCE_NUMBER",
    "CREDIT_DEBIT_CARD_CVV",
    "CREDIT_DEBIT_CARD_EXPIRY",
    "CREDIT_DEBIT_CARD_NUMBER",
    "DRIVER_ID",
    "EMAIL",
    "INTERNATIONAL_BANK_ACCOUNT_NUMBER",
    "IP_ADDRESS",
    "LICENSE_PLATE",
    "MAC_ADDRESS",
    "NAME",
    "PASSWORD",
    "PHONE",
    "PIN",
    "SWIFT_CODE",
    "UK_NATIONAL_HEALTH_SERVICE_NUMBER",
    "UK_NATIONAL_INSURANCE_NUMBER",
    "UK_UNIQUE_TAXPAYER_REFERENCE_NUMBER",
    "URL",
    "US_BANK_ACCOUNT_NUMBER",
    "US_BANK_ROUTING_NUMBER",
    "US_INDIVIDUAL_TAX_IDENTIFICATION_NUMBER",
    "US_PASSPORT_NUMBER",
    "US_SOCIAL_SECURITY_NUMBER",
    "USERNAME",
    "VEHICLE_IDENTIFICATION_NUMBER",
]
```
## GuardrailSensitiveInformationPolicyActionType

```python
# GuardrailSensitiveInformationPolicyActionType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import GuardrailSensitiveInformationPolicyActionType

def get_value() -> GuardrailSensitiveInformationPolicyActionType:
    return "ANONYMIZED"
```

```python
# GuardrailSensitiveInformationPolicyActionType definition
GuardrailSensitiveInformationPolicyActionType = Literal[
    "ANONYMIZED",
    "BLOCKED",
]
```
## GuardrailTopicPolicyActionType

```python
# GuardrailTopicPolicyActionType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import GuardrailTopicPolicyActionType

def get_value() -> GuardrailTopicPolicyActionType:
    return "BLOCKED"
```

```python
# GuardrailTopicPolicyActionType definition
GuardrailTopicPolicyActionType = Literal[
    "BLOCKED",
]
```
## GuardrailTopicTypeType

```python
# GuardrailTopicTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import GuardrailTopicTypeType

def get_value() -> GuardrailTopicTypeType:
    return "DENY"
```

```python
# GuardrailTopicTypeType definition
GuardrailTopicTypeType = Literal[
    "DENY",
]
```
## GuardrailWordPolicyActionType

```python
# GuardrailWordPolicyActionType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import GuardrailWordPolicyActionType

def get_value() -> GuardrailWordPolicyActionType:
    return "BLOCKED"
```

```python
# GuardrailWordPolicyActionType definition
GuardrailWordPolicyActionType = Literal[
    "BLOCKED",
]
```
## ImageFormatType

```python
# ImageFormatType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import ImageFormatType

def get_value() -> ImageFormatType:
    return "gif"
```

```python
# ImageFormatType definition
ImageFormatType = Literal[
    "gif",
    "jpeg",
    "png",
    "webp",
]
```
## ImageInputFormatType

```python
# ImageInputFormatType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import ImageInputFormatType

def get_value() -> ImageInputFormatType:
    return "gif"
```

```python
# ImageInputFormatType definition
ImageInputFormatType = Literal[
    "gif",
    "jpeg",
    "png",
    "webp",
]
```
## InputImageFormatType

```python
# InputImageFormatType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import InputImageFormatType

def get_value() -> InputImageFormatType:
    return "gif"
```

```python
# InputImageFormatType definition
InputImageFormatType = Literal[
    "gif",
    "jpeg",
    "png",
    "webp",
]
```
## InputQueryTypeType

```python
# InputQueryTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import InputQueryTypeType

def get_value() -> InputQueryTypeType:
    return "TEXT"
```

```python
# InputQueryTypeType definition
InputQueryTypeType = Literal[
    "TEXT",
]
```
## InvocationTypeType

```python
# InvocationTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import InvocationTypeType

def get_value() -> InvocationTypeType:
    return "ACTION_GROUP"
```

```python
# InvocationTypeType definition
InvocationTypeType = Literal[
    "ACTION_GROUP",
    "ACTION_GROUP_CODE_INTERPRETER",
    "AGENT_COLLABORATOR",
    "FINISH",
    "KNOWLEDGE_BASE",
]
```
## KnowledgeBaseQueryTypeType

```python
# KnowledgeBaseQueryTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import KnowledgeBaseQueryTypeType

def get_value() -> KnowledgeBaseQueryTypeType:
    return "IMAGE"
```

```python
# KnowledgeBaseQueryTypeType definition
KnowledgeBaseQueryTypeType = Literal[
    "IMAGE",
    "TEXT",
]
```
## ListFlowExecutionEventsPaginatorName

```python
# ListFlowExecutionEventsPaginatorName usage example
from types_aiobotocore_bedrock_agent_runtime.literals import ListFlowExecutionEventsPaginatorName

def get_value() -> ListFlowExecutionEventsPaginatorName:
    return "list_flow_execution_events"
```

```python
# ListFlowExecutionEventsPaginatorName definition
ListFlowExecutionEventsPaginatorName = Literal[
    "list_flow_execution_events",
]
```
## ListFlowExecutionsPaginatorName

```python
# ListFlowExecutionsPaginatorName usage example
from types_aiobotocore_bedrock_agent_runtime.literals import ListFlowExecutionsPaginatorName

def get_value() -> ListFlowExecutionsPaginatorName:
    return "list_flow_executions"
```

```python
# ListFlowExecutionsPaginatorName definition
ListFlowExecutionsPaginatorName = Literal[
    "list_flow_executions",
]
```
## ListInvocationStepsPaginatorName

```python
# ListInvocationStepsPaginatorName usage example
from types_aiobotocore_bedrock_agent_runtime.literals import ListInvocationStepsPaginatorName

def get_value() -> ListInvocationStepsPaginatorName:
    return "list_invocation_steps"
```

```python
# ListInvocationStepsPaginatorName definition
ListInvocationStepsPaginatorName = Literal[
    "list_invocation_steps",
]
```
## ListInvocationsPaginatorName

```python
# ListInvocationsPaginatorName usage example
from types_aiobotocore_bedrock_agent_runtime.literals import ListInvocationsPaginatorName

def get_value() -> ListInvocationsPaginatorName:
    return "list_invocations"
```

```python
# ListInvocationsPaginatorName definition
ListInvocationsPaginatorName = Literal[
    "list_invocations",
]
```
## ListSessionsPaginatorName

```python
# ListSessionsPaginatorName usage example
from types_aiobotocore_bedrock_agent_runtime.literals import ListSessionsPaginatorName

def get_value() -> ListSessionsPaginatorName:
    return "list_sessions"
```

```python
# ListSessionsPaginatorName definition
ListSessionsPaginatorName = Literal[
    "list_sessions",
]
```
## MemoryTypeType

```python
# MemoryTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import MemoryTypeType

def get_value() -> MemoryTypeType:
    return "SESSION_SUMMARY"
```

```python
# MemoryTypeType definition
MemoryTypeType = Literal[
    "SESSION_SUMMARY",
]
```
## NodeErrorCodeType

```python
# NodeErrorCodeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import NodeErrorCodeType

def get_value() -> NodeErrorCodeType:
    return "BAD_GATEWAY"
```

```python
# NodeErrorCodeType definition
NodeErrorCodeType = Literal[
    "BAD_GATEWAY",
    "DEPENDENCY_FAILED",
    "INTERNAL_SERVER",
    "VALIDATION",
]
```
## NodeTypeType

```python
# NodeTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import NodeTypeType

def get_value() -> NodeTypeType:
    return "ConditionNode"
```

```python
# NodeTypeType definition
NodeTypeType = Literal[
    "ConditionNode",
    "FlowInputNode",
    "FlowOutputNode",
    "KnowledgeBaseNode",
    "LambdaFunctionNode",
    "LexNode",
    "PromptNode",
]
```
## OrchestrationTypeType

```python
# OrchestrationTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import OrchestrationTypeType

def get_value() -> OrchestrationTypeType:
    return "CUSTOM_ORCHESTRATION"
```

```python
# OrchestrationTypeType definition
OrchestrationTypeType = Literal[
    "CUSTOM_ORCHESTRATION",
    "DEFAULT",
]
```
## ParameterTypeType

```python
# ParameterTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import ParameterTypeType

def get_value() -> ParameterTypeType:
    return "array"
```

```python
# ParameterTypeType definition
ParameterTypeType = Literal[
    "array",
    "boolean",
    "integer",
    "number",
    "string",
]
```
## PayloadTypeType

```python
# PayloadTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import PayloadTypeType

def get_value() -> PayloadTypeType:
    return "RETURN_CONTROL"
```

```python
# PayloadTypeType definition
PayloadTypeType = Literal[
    "RETURN_CONTROL",
    "TEXT",
]
```
## PerformanceConfigLatencyType

```python
# PerformanceConfigLatencyType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import PerformanceConfigLatencyType

def get_value() -> PerformanceConfigLatencyType:
    return "optimized"
```

```python
# PerformanceConfigLatencyType definition
PerformanceConfigLatencyType = Literal[
    "optimized",
    "standard",
]
```
## PromptStateType

```python
# PromptStateType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import PromptStateType

def get_value() -> PromptStateType:
    return "DISABLED"
```

```python
# PromptStateType definition
PromptStateType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## PromptTypeType

```python
# PromptTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import PromptTypeType

def get_value() -> PromptTypeType:
    return "KNOWLEDGE_BASE_RESPONSE_GENERATION"
```

```python
# PromptTypeType definition
PromptTypeType = Literal[
    "KNOWLEDGE_BASE_RESPONSE_GENERATION",
    "ORCHESTRATION",
    "POST_PROCESSING",
    "PRE_PROCESSING",
    "ROUTING_CLASSIFIER",
]
```
## QueryTransformationModeType

```python
# QueryTransformationModeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import QueryTransformationModeType

def get_value() -> QueryTransformationModeType:
    return "TEXT_TO_SQL"
```

```python
# QueryTransformationModeType definition
QueryTransformationModeType = Literal[
    "TEXT_TO_SQL",
]
```
## QueryTransformationTypeType

```python
# QueryTransformationTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import QueryTransformationTypeType

def get_value() -> QueryTransformationTypeType:
    return "QUERY_DECOMPOSITION"
```

```python
# QueryTransformationTypeType definition
QueryTransformationTypeType = Literal[
    "QUERY_DECOMPOSITION",
]
```
## RelayConversationHistoryType

```python
# RelayConversationHistoryType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import RelayConversationHistoryType

def get_value() -> RelayConversationHistoryType:
    return "DISABLED"
```

```python
# RelayConversationHistoryType definition
RelayConversationHistoryType = Literal[
    "DISABLED",
    "TO_COLLABORATOR",
]
```
## RequireConfirmationType

```python
# RequireConfirmationType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import RequireConfirmationType

def get_value() -> RequireConfirmationType:
    return "DISABLED"
```

```python
# RequireConfirmationType definition
RequireConfirmationType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## RerankDocumentTypeType

```python
# RerankDocumentTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import RerankDocumentTypeType

def get_value() -> RerankDocumentTypeType:
    return "JSON"
```

```python
# RerankDocumentTypeType definition
RerankDocumentTypeType = Literal[
    "JSON",
    "TEXT",
]
```
## RerankPaginatorName

```python
# RerankPaginatorName usage example
from types_aiobotocore_bedrock_agent_runtime.literals import RerankPaginatorName

def get_value() -> RerankPaginatorName:
    return "rerank"
```

```python
# RerankPaginatorName definition
RerankPaginatorName = Literal[
    "rerank",
]
```
## RerankQueryContentTypeType

```python
# RerankQueryContentTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import RerankQueryContentTypeType

def get_value() -> RerankQueryContentTypeType:
    return "TEXT"
```

```python
# RerankQueryContentTypeType definition
RerankQueryContentTypeType = Literal[
    "TEXT",
]
```
## RerankSourceTypeType

```python
# RerankSourceTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import RerankSourceTypeType

def get_value() -> RerankSourceTypeType:
    return "INLINE"
```

```python
# RerankSourceTypeType definition
RerankSourceTypeType = Literal[
    "INLINE",
]
```
## RerankingConfigurationTypeType

```python
# RerankingConfigurationTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import RerankingConfigurationTypeType

def get_value() -> RerankingConfigurationTypeType:
    return "BEDROCK_RERANKING_MODEL"
```

```python
# RerankingConfigurationTypeType definition
RerankingConfigurationTypeType = Literal[
    "BEDROCK_RERANKING_MODEL",
]
```
## RerankingMetadataSelectionModeType

```python
# RerankingMetadataSelectionModeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import RerankingMetadataSelectionModeType

def get_value() -> RerankingMetadataSelectionModeType:
    return "ALL"
```

```python
# RerankingMetadataSelectionModeType definition
RerankingMetadataSelectionModeType = Literal[
    "ALL",
    "SELECTIVE",
]
```
## ResponseStateType

```python
# ResponseStateType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import ResponseStateType

def get_value() -> ResponseStateType:
    return "FAILURE"
```

```python
# ResponseStateType definition
ResponseStateType = Literal[
    "FAILURE",
    "REPROMPT",
]
```
## RetrievalResultContentColumnTypeType

```python
# RetrievalResultContentColumnTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import RetrievalResultContentColumnTypeType

def get_value() -> RetrievalResultContentColumnTypeType:
    return "BLOB"
```

```python
# RetrievalResultContentColumnTypeType definition
RetrievalResultContentColumnTypeType = Literal[
    "BLOB",
    "BOOLEAN",
    "DOUBLE",
    "LONG",
    "NULL",
    "STRING",
]
```
## RetrievalResultContentTypeType

```python
# RetrievalResultContentTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import RetrievalResultContentTypeType

def get_value() -> RetrievalResultContentTypeType:
    return "AUDIO"
```

```python
# RetrievalResultContentTypeType definition
RetrievalResultContentTypeType = Literal[
    "AUDIO",
    "IMAGE",
    "ROW",
    "TEXT",
    "VIDEO",
]
```
## RetrievalResultLocationTypeType

```python
# RetrievalResultLocationTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import RetrievalResultLocationTypeType

def get_value() -> RetrievalResultLocationTypeType:
    return "CONFLUENCE"
```

```python
# RetrievalResultLocationTypeType definition
RetrievalResultLocationTypeType = Literal[
    "CONFLUENCE",
    "CUSTOM",
    "KENDRA",
    "S3",
    "SALESFORCE",
    "SHAREPOINT",
    "SQL",
    "WEB",
]
```
## RetrieveAndGenerateTypeType

```python
# RetrieveAndGenerateTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import RetrieveAndGenerateTypeType

def get_value() -> RetrieveAndGenerateTypeType:
    return "EXTERNAL_SOURCES"
```

```python
# RetrieveAndGenerateTypeType definition
RetrieveAndGenerateTypeType = Literal[
    "EXTERNAL_SOURCES",
    "KNOWLEDGE_BASE",
]
```
## RetrievePaginatorName

```python
# RetrievePaginatorName usage example
from types_aiobotocore_bedrock_agent_runtime.literals import RetrievePaginatorName

def get_value() -> RetrievePaginatorName:
    return "retrieve"
```

```python
# RetrievePaginatorName definition
RetrievePaginatorName = Literal[
    "retrieve",
]
```
## SearchTypeType

```python
# SearchTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import SearchTypeType

def get_value() -> SearchTypeType:
    return "HYBRID"
```

```python
# SearchTypeType definition
SearchTypeType = Literal[
    "HYBRID",
    "SEMANTIC",
]
```
## SessionStatusType

```python
# SessionStatusType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import SessionStatusType

def get_value() -> SessionStatusType:
    return "ACTIVE"
```

```python
# SessionStatusType definition
SessionStatusType = Literal[
    "ACTIVE",
    "ENDED",
    "EXPIRED",
]
```
## SourceType

```python
# SourceType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import SourceType

def get_value() -> SourceType:
    return "ACTION_GROUP"
```

```python
# SourceType definition
SourceType = Literal[
    "ACTION_GROUP",
    "KNOWLEDGE_BASE",
    "PARSER",
]
```
## TextToSqlConfigurationTypeType

```python
# TextToSqlConfigurationTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import TextToSqlConfigurationTypeType

def get_value() -> TextToSqlConfigurationTypeType:
    return "KNOWLEDGE_BASE"
```

```python
# TextToSqlConfigurationTypeType definition
TextToSqlConfigurationTypeType = Literal[
    "KNOWLEDGE_BASE",
]
```
## TypeType

```python
# TypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import TypeType

def get_value() -> TypeType:
    return "ACTION_GROUP"
```

```python
# TypeType definition
TypeType = Literal[
    "ACTION_GROUP",
    "AGENT_COLLABORATOR",
    "ASK_USER",
    "FINISH",
    "KNOWLEDGE_BASE",
    "REPROMPT",
]
```
## VectorSearchRerankingConfigurationTypeType

```python
# VectorSearchRerankingConfigurationTypeType usage example
from types_aiobotocore_bedrock_agent_runtime.literals import VectorSearchRerankingConfigurationTypeType

def get_value() -> VectorSearchRerankingConfigurationTypeType:
    return "BEDROCK_RERANKING_MODEL"
```

```python
# VectorSearchRerankingConfigurationTypeType definition
VectorSearchRerankingConfigurationTypeType = Literal[
    "BEDROCK_RERANKING_MODEL",
]
```
## AgentsforBedrockRuntimeServiceName

```python
# AgentsforBedrockRuntimeServiceName usage example
from types_aiobotocore_bedrock_agent_runtime.literals import AgentsforBedrockRuntimeServiceName

def get_value() -> AgentsforBedrockRuntimeServiceName:
    return "bedrock-agent-runtime"
```

```python
# AgentsforBedrockRuntimeServiceName definition
AgentsforBedrockRuntimeServiceName = Literal[
    "bedrock-agent-runtime",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_bedrock_agent_runtime.literals import ServiceName

def get_value() -> ServiceName:
    return "accessanalyzer"
```

```python
# ServiceName definition
ServiceName = Literal[
    "accessanalyzer",
    "account",
    "acm",
    "acm-pca",
    "aiops",
    "amp",
    "amplify",
    "amplifybackend",
    "amplifyuibuilder",
    "apigateway",
    "apigatewaymanagementapi",
    "apigatewayv2",
    "appconfig",
    "appconfigdata",
    "appfabric",
    "appflow",
    "appintegrations",
    "application-autoscaling",
    "application-insights",
    "application-signals",
    "applicationcostprofiler",
    "appmesh",
    "apprunner",
    "appstream",
    "appsync",
    "arc-region-switch",
    "arc-zonal-shift",
    "artifact",
    "athena",
    "auditmanager",
    "autoscaling",
    "autoscaling-plans",
    "b2bi",
    "backup",
    "backup-gateway",
    "backupsearch",
    "batch",
    "bcm-dashboards",
    "bcm-data-exports",
    "bcm-pricing-calculator",
    "bcm-recommended-actions",
    "bedrock",
    "bedrock-agent",
    "bedrock-agent-runtime",
    "bedrock-agentcore",
    "bedrock-agentcore-control",
    "bedrock-data-automation",
    "bedrock-data-automation-runtime",
    "bedrock-runtime",
    "billing",
    "billingconductor",
    "braket",
    "budgets",
    "ce",
    "chatbot",
    "chime",
    "chime-sdk-identity",
    "chime-sdk-media-pipelines",
    "chime-sdk-meetings",
    "chime-sdk-messaging",
    "chime-sdk-voice",
    "cleanrooms",
    "cleanroomsml",
    "cloud9",
    "cloudcontrol",
    "clouddirectory",
    "cloudformation",
    "cloudfront",
    "cloudfront-keyvaluestore",
    "cloudhsm",
    "cloudhsmv2",
    "cloudsearch",
    "cloudsearchdomain",
    "cloudtrail",
    "cloudtrail-data",
    "cloudwatch",
    "codeartifact",
    "codebuild",
    "codecatalyst",
    "codecommit",
    "codeconnections",
    "codedeploy",
    "codeguru-reviewer",
    "codeguru-security",
    "codeguruprofiler",
    "codepipeline",
    "codestar-connections",
    "codestar-notifications",
    "cognito-identity",
    "cognito-idp",
    "cognito-sync",
    "comprehend",
    "comprehendmedical",
    "compute-optimizer",
    "compute-optimizer-automation",
    "config",
    "connect",
    "connect-contact-lens",
    "connectcampaigns",
    "connectcampaignsv2",
    "connectcases",
    "connectparticipant",
    "controlcatalog",
    "controltower",
    "cost-optimization-hub",
    "cur",
    "customer-profiles",
    "databrew",
    "dataexchange",
    "datapipeline",
    "datasync",
    "datazone",
    "dax",
    "deadline",
    "detective",
    "devicefarm",
    "devops-guru",
    "directconnect",
    "discovery",
    "dlm",
    "dms",
    "docdb",
    "docdb-elastic",
    "drs",
    "ds",
    "ds-data",
    "dsql",
    "dynamodb",
    "dynamodbstreams",
    "ebs",
    "ec2",
    "ec2-instance-connect",
    "ecr",
    "ecr-public",
    "ecs",
    "efs",
    "eks",
    "eks-auth",
    "elasticache",
    "elasticbeanstalk",
    "elb",
    "elbv2",
    "emr",
    "emr-containers",
    "emr-serverless",
    "entityresolution",
    "es",
    "events",
    "evidently",
    "evs",
    "finspace",
    "finspace-data",
    "firehose",
    "fis",
    "fms",
    "forecast",
    "forecastquery",
    "frauddetector",
    "freetier",
    "fsx",
    "gamelift",
    "gameliftstreams",
    "geo-maps",
    "geo-places",
    "geo-routes",
    "glacier",
    "globalaccelerator",
    "glue",
    "grafana",
    "greengrass",
    "greengrassv2",
    "groundstation",
    "guardduty",
    "health",
    "healthlake",
    "iam",
    "identitystore",
    "imagebuilder",
    "importexport",
    "inspector",
    "inspector-scan",
    "inspector2",
    "internetmonitor",
    "invoicing",
    "iot",
    "iot-data",
    "iot-jobs-data",
    "iot-managed-integrations",
    "iotanalytics",
    "iotdeviceadvisor",
    "iotevents",
    "iotevents-data",
    "iotfleetwise",
    "iotsecuretunneling",
    "iotsitewise",
    "iotthingsgraph",
    "iottwinmaker",
    "iotwireless",
    "ivs",
    "ivs-realtime",
    "ivschat",
    "kafka",
    "kafkaconnect",
    "kendra",
    "kendra-ranking",
    "keyspaces",
    "keyspacesstreams",
    "kinesis",
    "kinesis-video-archived-media",
    "kinesis-video-media",
    "kinesis-video-signaling",
    "kinesis-video-webrtc-storage",
    "kinesisanalytics",
    "kinesisanalyticsv2",
    "kinesisvideo",
    "kms",
    "lakeformation",
    "lambda",
    "launch-wizard",
    "lex-models",
    "lex-runtime",
    "lexv2-models",
    "lexv2-runtime",
    "license-manager",
    "license-manager-linux-subscriptions",
    "license-manager-user-subscriptions",
    "lightsail",
    "location",
    "logs",
    "lookoutequipment",
    "m2",
    "machinelearning",
    "macie2",
    "mailmanager",
    "managedblockchain",
    "managedblockchain-query",
    "marketplace-agreement",
    "marketplace-catalog",
    "marketplace-deployment",
    "marketplace-entitlement",
    "marketplace-reporting",
    "marketplacecommerceanalytics",
    "mediaconnect",
    "mediaconvert",
    "medialive",
    "mediapackage",
    "mediapackage-vod",
    "mediapackagev2",
    "mediastore",
    "mediastore-data",
    "mediatailor",
    "medical-imaging",
    "memorydb",
    "meteringmarketplace",
    "mgh",
    "mgn",
    "migration-hub-refactor-spaces",
    "migrationhub-config",
    "migrationhuborchestrator",
    "migrationhubstrategy",
    "mpa",
    "mq",
    "mturk",
    "mwaa",
    "mwaa-serverless",
    "neptune",
    "neptune-graph",
    "neptunedata",
    "network-firewall",
    "networkflowmonitor",
    "networkmanager",
    "networkmonitor",
    "notifications",
    "notificationscontacts",
    "nova-act",
    "oam",
    "observabilityadmin",
    "odb",
    "omics",
    "opensearch",
    "opensearchserverless",
    "organizations",
    "osis",
    "outposts",
    "panorama",
    "partnercentral-account",
    "partnercentral-benefits",
    "partnercentral-channel",
    "partnercentral-selling",
    "payment-cryptography",
    "payment-cryptography-data",
    "pca-connector-ad",
    "pca-connector-scep",
    "pcs",
    "personalize",
    "personalize-events",
    "personalize-runtime",
    "pi",
    "pinpoint",
    "pinpoint-email",
    "pinpoint-sms-voice",
    "pinpoint-sms-voice-v2",
    "pipes",
    "polly",
    "pricing",
    "proton",
    "qapps",
    "qbusiness",
    "qconnect",
    "quicksight",
    "ram",
    "rbin",
    "rds",
    "rds-data",
    "redshift",
    "redshift-data",
    "redshift-serverless",
    "rekognition",
    "repostspace",
    "resiliencehub",
    "resource-explorer-2",
    "resource-groups",
    "resourcegroupstaggingapi",
    "rolesanywhere",
    "route53",
    "route53-recovery-cluster",
    "route53-recovery-control-config",
    "route53-recovery-readiness",
    "route53domains",
    "route53globalresolver",
    "route53profiles",
    "route53resolver",
    "rtbfabric",
    "rum",
    "s3",
    "s3control",
    "s3outposts",
    "s3tables",
    "s3vectors",
    "sagemaker",
    "sagemaker-a2i-runtime",
    "sagemaker-edge",
    "sagemaker-featurestore-runtime",
    "sagemaker-geospatial",
    "sagemaker-metrics",
    "sagemaker-runtime",
    "savingsplans",
    "scheduler",
    "schemas",
    "sdb",
    "secretsmanager",
    "security-ir",
    "securityhub",
    "securitylake",
    "serverlessrepo",
    "service-quotas",
    "servicecatalog",
    "servicecatalog-appregistry",
    "servicediscovery",
    "ses",
    "sesv2",
    "shield",
    "signer",
    "signin",
    "simspaceweaver",
    "snow-device-management",
    "snowball",
    "sns",
    "socialmessaging",
    "sqs",
    "ssm",
    "ssm-contacts",
    "ssm-guiconnect",
    "ssm-incidents",
    "ssm-quicksetup",
    "ssm-sap",
    "sso",
    "sso-admin",
    "sso-oidc",
    "stepfunctions",
    "storagegateway",
    "sts",
    "supplychain",
    "support",
    "support-app",
    "swf",
    "synthetics",
    "taxsettings",
    "textract",
    "timestream-influxdb",
    "timestream-query",
    "timestream-write",
    "tnb",
    "transcribe",
    "transfer",
    "translate",
    "trustedadvisor",
    "verifiedpermissions",
    "voice-id",
    "vpc-lattice",
    "waf",
    "waf-regional",
    "wafv2",
    "wellarchitected",
    "wickr",
    "wisdom",
    "workdocs",
    "workmail",
    "workmailmessageflow",
    "workspaces",
    "workspaces-instances",
    "workspaces-thin-client",
    "workspaces-web",
    "xray",
]
```
## ResourceServiceName

```python
# ResourceServiceName usage example
from types_aiobotocore_bedrock_agent_runtime.literals import ResourceServiceName

def get_value() -> ResourceServiceName:
    return "cloudformation"
```

```python
# ResourceServiceName definition
ResourceServiceName = Literal[
    "cloudformation",
    "cloudwatch",
    "dynamodb",
    "ec2",
    "glacier",
    "iam",
    "s3",
    "sns",
    "sqs",
]
```
## PaginatorName

```python
# PaginatorName usage example
from types_aiobotocore_bedrock_agent_runtime.literals import PaginatorName

def get_value() -> PaginatorName:
    return "get_agent_memory"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "get_agent_memory",
    "list_flow_execution_events",
    "list_flow_executions",
    "list_invocation_steps",
    "list_invocations",
    "list_sessions",
    "rerank",
    "retrieve",
]
```
