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
    return "IMAGE"
```

```python
# RetrievalResultContentTypeType definition
RetrievalResultContentTypeType = Literal[
    "IMAGE",
    "ROW",
    "TEXT",
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
    "apptest",
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
    "bcm-data-exports",
    "bcm-pricing-calculator",
    "bedrock",
    "bedrock-agent",
    "bedrock-agent-runtime",
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
    "elastic-inference",
    "elasticache",
    "elasticbeanstalk",
    "elastictranscoder",
    "elb",
    "elbv2",
    "emr",
    "emr-containers",
    "emr-serverless",
    "entityresolution",
    "es",
    "events",
    "evidently",
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
    "iotanalytics",
    "iotdeviceadvisor",
    "iotevents",
    "iotevents-data",
    "iotfleethub",
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
    "lookoutmetrics",
    "lookoutvision",
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
    "mq",
    "mturk",
    "mwaa",
    "neptune",
    "neptune-graph",
    "neptunedata",
    "network-firewall",
    "networkflowmonitor",
    "networkmanager",
    "networkmonitor",
    "notifications",
    "notificationscontacts",
    "oam",
    "observabilityadmin",
    "omics",
    "opensearch",
    "opensearchserverless",
    "opsworks",
    "opsworkscm",
    "organizations",
    "osis",
    "outposts",
    "panorama",
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
    "privatenetworks",
    "proton",
    "qapps",
    "qbusiness",
    "qconnect",
    "qldb",
    "qldb-session",
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
    "robomaker",
    "rolesanywhere",
    "route53",
    "route53-recovery-cluster",
    "route53-recovery-control-config",
    "route53-recovery-readiness",
    "route53domains",
    "route53profiles",
    "route53resolver",
    "rum",
    "s3",
    "s3control",
    "s3outposts",
    "s3tables",
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
    "simspaceweaver",
    "sms",
    "sms-voice",
    "snow-device-management",
    "snowball",
    "sns",
    "socialmessaging",
    "sqs",
    "ssm",
    "ssm-contacts",
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
    "wisdom",
    "workdocs",
    "workmail",
    "workmailmessageflow",
    "workspaces",
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
    "opsworks",
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
    "rerank",
    "retrieve",
]
```
