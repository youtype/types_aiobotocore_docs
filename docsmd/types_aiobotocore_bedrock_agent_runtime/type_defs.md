# Type definitions

> [Index](../README.md) > [AgentsforBedrockRuntime](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AgentsforBedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#agentsforbedrockruntime)
    type annotations stubs module [types-aiobotocore-bedrock-agent-runtime](https://pypi.org/project/types-aiobotocore-bedrock-agent-runtime/).

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


## InferenceConfigurationUnionTypeDef

```python
# InferenceConfigurationUnionTypeDef definition

InferenceConfigurationUnionTypeDef = Union[
    InferenceConfigurationTypeDef,  # (1)
    InferenceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: InferenceConfigurationTypeDef](./type_defs.md#inferenceconfigurationtypedef) 
2. See [:material-code-braces: InferenceConfigurationOutputTypeDef](./type_defs.md#inferenceconfigurationoutputtypedef) 

## ApiResultUnionTypeDef

```python
# ApiResultUnionTypeDef definition

ApiResultUnionTypeDef = Union[
    ApiResultTypeDef,  # (1)
    ApiResultOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ApiResultTypeDef](./type_defs.md#apiresulttypedef) 
2. See [:material-code-braces: ApiResultOutputTypeDef](./type_defs.md#apiresultoutputtypedef) 

## FunctionResultUnionTypeDef

```python
# FunctionResultUnionTypeDef definition

FunctionResultUnionTypeDef = Union[
    FunctionResultTypeDef,  # (1)
    FunctionResultOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FunctionResultTypeDef](./type_defs.md#functionresulttypedef) 
2. See [:material-code-braces: FunctionResultOutputTypeDef](./type_defs.md#functionresultoutputtypedef) 

## RerankDocumentUnionTypeDef

```python
# RerankDocumentUnionTypeDef definition

RerankDocumentUnionTypeDef = Union[
    RerankDocumentTypeDef,  # (1)
    RerankDocumentOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RerankDocumentTypeDef](./type_defs.md#rerankdocumenttypedef) 
2. See [:material-code-braces: RerankDocumentOutputTypeDef](./type_defs.md#rerankdocumentoutputtypedef) 

## InvocationResultMemberUnionTypeDef

```python
# InvocationResultMemberUnionTypeDef definition

InvocationResultMemberUnionTypeDef = Union[
    InvocationResultMemberTypeDef,  # (1)
    InvocationResultMemberOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: InvocationResultMemberTypeDef](./type_defs.md#invocationresultmembertypedef) 
2. See [:material-code-braces: InvocationResultMemberOutputTypeDef](./type_defs.md#invocationresultmemberoutputtypedef) 



## S3IdentifierTypeDef

```python
# S3IdentifierTypeDef definition

class S3IdentifierTypeDef(TypedDict):
    s3BucketName: NotRequired[str],
    s3ObjectKey: NotRequired[str],
```

## AccessDeniedExceptionTypeDef

```python
# AccessDeniedExceptionTypeDef definition

class AccessDeniedExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## ActionGroupExecutorTypeDef

```python
# ActionGroupExecutorTypeDef definition

class ActionGroupExecutorTypeDef(TypedDict):
    customControl: NotRequired[CustomControlMethodType],  # (1)
    lambda: NotRequired[str],
```

1. See [:material-code-brackets: CustomControlMethodType](./literals.md#customcontrolmethodtype) 
## ParameterTypeDef

```python
# ParameterTypeDef definition

class ParameterTypeDef(TypedDict):
    name: NotRequired[str],
    type: NotRequired[str],
    value: NotRequired[str],
```

## ActionGroupInvocationOutputTypeDef

```python
# ActionGroupInvocationOutputTypeDef definition

class ActionGroupInvocationOutputTypeDef(TypedDict):
    text: NotRequired[str],
```

## AnalyzePromptEventTypeDef

```python
# AnalyzePromptEventTypeDef definition

class AnalyzePromptEventTypeDef(TypedDict):
    message: NotRequired[str],
```

## ApiParameterTypeDef

```python
# ApiParameterTypeDef definition

class ApiParameterTypeDef(TypedDict):
    name: NotRequired[str],
    type: NotRequired[str],
    value: NotRequired[str],
```

## ContentBodyTypeDef

```python
# ContentBodyTypeDef definition

class ContentBodyTypeDef(TypedDict):
    body: NotRequired[str],
```

## BadGatewayExceptionTypeDef

```python
# BadGatewayExceptionTypeDef definition

class BadGatewayExceptionTypeDef(TypedDict):
    message: NotRequired[str],
    resourceName: NotRequired[str],
```

## BedrockRerankingModelConfigurationTypeDef

```python
# BedrockRerankingModelConfigurationTypeDef definition

class BedrockRerankingModelConfigurationTypeDef(TypedDict):
    modelArn: str,
    additionalModelRequestFields: NotRequired[Mapping[str, Mapping[str, Any]]],
```

## CallerTypeDef

```python
# CallerTypeDef definition

class CallerTypeDef(TypedDict):
    agentAliasArn: NotRequired[str],
```

## CodeInterpreterInvocationInputTypeDef

```python
# CodeInterpreterInvocationInputTypeDef definition

class CodeInterpreterInvocationInputTypeDef(TypedDict):
    code: NotRequired[str],
    files: NotRequired[List[str]],
```

## CodeInterpreterInvocationOutputTypeDef

```python
# CodeInterpreterInvocationOutputTypeDef definition

class CodeInterpreterInvocationOutputTypeDef(TypedDict):
    executionError: NotRequired[str],
    executionOutput: NotRequired[str],
    executionTimeout: NotRequired[bool],
    files: NotRequired[List[str]],
```

## ConflictExceptionTypeDef

```python
# ConflictExceptionTypeDef definition

class ConflictExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## ContentBlockTypeDef

```python
# ContentBlockTypeDef definition

class ContentBlockTypeDef(TypedDict):
    text: NotRequired[str],
```

## CustomOrchestrationTraceEventTypeDef

```python
# CustomOrchestrationTraceEventTypeDef definition

class CustomOrchestrationTraceEventTypeDef(TypedDict):
    text: NotRequired[str],
```

## DeleteAgentMemoryRequestRequestTypeDef

```python
# DeleteAgentMemoryRequestRequestTypeDef definition

class DeleteAgentMemoryRequestRequestTypeDef(TypedDict):
    agentAliasId: str,
    agentId: str,
    memoryId: NotRequired[str],
```

## DependencyFailedExceptionTypeDef

```python
# DependencyFailedExceptionTypeDef definition

class DependencyFailedExceptionTypeDef(TypedDict):
    message: NotRequired[str],
    resourceName: NotRequired[str],
```

## S3ObjectDocTypeDef

```python
# S3ObjectDocTypeDef definition

class S3ObjectDocTypeDef(TypedDict):
    uri: str,
```

## GuardrailConfigurationTypeDef

```python
# GuardrailConfigurationTypeDef definition

class GuardrailConfigurationTypeDef(TypedDict):
    guardrailId: str,
    guardrailVersion: str,
```

## PromptTemplateTypeDef

```python
# PromptTemplateTypeDef definition

class PromptTemplateTypeDef(TypedDict):
    textPromptTemplate: NotRequired[str],
```

## FailureTraceTypeDef

```python
# FailureTraceTypeDef definition

class FailureTraceTypeDef(TypedDict):
    failureReason: NotRequired[str],
    traceId: NotRequired[str],
```

## FieldForRerankingTypeDef

```python
# FieldForRerankingTypeDef definition

class FieldForRerankingTypeDef(TypedDict):
    fieldName: str,
```

## OutputFileTypeDef

```python
# OutputFileTypeDef definition

class OutputFileTypeDef(TypedDict):
    bytes: NotRequired[bytes],
    name: NotRequired[str],
    type: NotRequired[str],
```

## S3ObjectFileTypeDef

```python
# S3ObjectFileTypeDef definition

class S3ObjectFileTypeDef(TypedDict):
    uri: str,
```

## FilterAttributeTypeDef

```python
# FilterAttributeTypeDef definition

class FilterAttributeTypeDef(TypedDict):
    key: str,
    value: Mapping[str, Any],
```

## FinalResponseTypeDef

```python
# FinalResponseTypeDef definition

class FinalResponseTypeDef(TypedDict):
    text: NotRequired[str],
```

## FlowCompletionEventTypeDef

```python
# FlowCompletionEventTypeDef definition

class FlowCompletionEventTypeDef(TypedDict):
    completionReason: FlowCompletionReasonType,  # (1)
```

1. See [:material-code-brackets: FlowCompletionReasonType](./literals.md#flowcompletionreasontype) 
## FlowInputContentTypeDef

```python
# FlowInputContentTypeDef definition

class FlowInputContentTypeDef(TypedDict):
    document: NotRequired[Mapping[str, Any]],
```

## FlowOutputContentTypeDef

```python
# FlowOutputContentTypeDef definition

class FlowOutputContentTypeDef(TypedDict):
    document: NotRequired[Dict[str, Any]],
```

## InternalServerExceptionTypeDef

```python
# InternalServerExceptionTypeDef definition

class InternalServerExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## ResourceNotFoundExceptionTypeDef

```python
# ResourceNotFoundExceptionTypeDef definition

class ResourceNotFoundExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## ServiceQuotaExceededExceptionTypeDef

```python
# ServiceQuotaExceededExceptionTypeDef definition

class ServiceQuotaExceededExceptionTypeDef(TypedDict):
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

## FlowTraceConditionTypeDef

```python
# FlowTraceConditionTypeDef definition

class FlowTraceConditionTypeDef(TypedDict):
    conditionName: str,
```

## FlowTraceNodeInputContentTypeDef

```python
# FlowTraceNodeInputContentTypeDef definition

class FlowTraceNodeInputContentTypeDef(TypedDict):
    document: NotRequired[Dict[str, Any]],
```

## FlowTraceNodeOutputContentTypeDef

```python
# FlowTraceNodeOutputContentTypeDef definition

class FlowTraceNodeOutputContentTypeDef(TypedDict):
    document: NotRequired[Dict[str, Any]],
```

## ParameterDetailTypeDef

```python
# ParameterDetailTypeDef definition

class ParameterDetailTypeDef(TypedDict):
    type: ParameterTypeType,  # (1)
    description: NotRequired[str],
    required: NotRequired[bool],
```

1. See [:material-code-brackets: ParameterTypeType](./literals.md#parametertypetype) 
## FunctionParameterTypeDef

```python
# FunctionParameterTypeDef definition

class FunctionParameterTypeDef(TypedDict):
    name: NotRequired[str],
    type: NotRequired[str],
    value: NotRequired[str],
```

## QueryGenerationInputTypeDef

```python
# QueryGenerationInputTypeDef definition

class QueryGenerationInputTypeDef(TypedDict):
    text: str,
    type: InputQueryTypeType,  # (1)
```

1. See [:material-code-brackets: InputQueryTypeType](./literals.md#inputquerytypetype) 
## GeneratedQueryTypeDef

```python
# GeneratedQueryTypeDef definition

class GeneratedQueryTypeDef(TypedDict):
    sql: NotRequired[str],
    type: NotRequired[GeneratedQueryTypeType],  # (1)
```

1. See [:material-code-brackets: GeneratedQueryTypeType](./literals.md#generatedquerytypetype) 
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

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetAgentMemoryRequestRequestTypeDef

```python
# GetAgentMemoryRequestRequestTypeDef definition

class GetAgentMemoryRequestRequestTypeDef(TypedDict):
    agentAliasId: str,
    agentId: str,
    memoryId: str,
    memoryType: MemoryTypeType,  # (1)
    maxItems: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: MemoryTypeType](./literals.md#memorytypetype) 
## GuardrailConfigurationWithArnTypeDef

```python
# GuardrailConfigurationWithArnTypeDef definition

class GuardrailConfigurationWithArnTypeDef(TypedDict):
    guardrailIdentifier: str,
    guardrailVersion: str,
```

## GuardrailContentFilterTypeDef

```python
# GuardrailContentFilterTypeDef definition

class GuardrailContentFilterTypeDef(TypedDict):
    action: NotRequired[GuardrailContentPolicyActionType],  # (1)
    confidence: NotRequired[GuardrailContentFilterConfidenceType],  # (2)
    type: NotRequired[GuardrailContentFilterTypeType],  # (3)
```

1. See [:material-code-brackets: GuardrailContentPolicyActionType](./literals.md#guardrailcontentpolicyactiontype) 
2. See [:material-code-brackets: GuardrailContentFilterConfidenceType](./literals.md#guardrailcontentfilterconfidencetype) 
3. See [:material-code-brackets: GuardrailContentFilterTypeType](./literals.md#guardrailcontentfiltertypetype) 
## GuardrailCustomWordTypeDef

```python
# GuardrailCustomWordTypeDef definition

class GuardrailCustomWordTypeDef(TypedDict):
    action: NotRequired[GuardrailWordPolicyActionType],  # (1)
    match: NotRequired[str],
```

1. See [:material-code-brackets: GuardrailWordPolicyActionType](./literals.md#guardrailwordpolicyactiontype) 
## GuardrailEventTypeDef

```python
# GuardrailEventTypeDef definition

class GuardrailEventTypeDef(TypedDict):
    action: NotRequired[GuadrailActionType],  # (1)
```

1. See [:material-code-brackets: GuadrailActionType](./literals.md#guadrailactiontype) 
## GuardrailManagedWordTypeDef

```python
# GuardrailManagedWordTypeDef definition

class GuardrailManagedWordTypeDef(TypedDict):
    action: NotRequired[GuardrailWordPolicyActionType],  # (1)
    match: NotRequired[str],
    type: NotRequired[GuardrailManagedWordTypeType],  # (2)
```

1. See [:material-code-brackets: GuardrailWordPolicyActionType](./literals.md#guardrailwordpolicyactiontype) 
2. See [:material-code-brackets: GuardrailManagedWordTypeType](./literals.md#guardrailmanagedwordtypetype) 
## GuardrailPiiEntityFilterTypeDef

```python
# GuardrailPiiEntityFilterTypeDef definition

class GuardrailPiiEntityFilterTypeDef(TypedDict):
    action: NotRequired[GuardrailSensitiveInformationPolicyActionType],  # (1)
    match: NotRequired[str],
    type: NotRequired[GuardrailPiiEntityTypeType],  # (2)
```

1. See [:material-code-brackets: GuardrailSensitiveInformationPolicyActionType](./literals.md#guardrailsensitiveinformationpolicyactiontype) 
2. See [:material-code-brackets: GuardrailPiiEntityTypeType](./literals.md#guardrailpiientitytypetype) 
## GuardrailRegexFilterTypeDef

```python
# GuardrailRegexFilterTypeDef definition

class GuardrailRegexFilterTypeDef(TypedDict):
    action: NotRequired[GuardrailSensitiveInformationPolicyActionType],  # (1)
    match: NotRequired[str],
    name: NotRequired[str],
    regex: NotRequired[str],
```

1. See [:material-code-brackets: GuardrailSensitiveInformationPolicyActionType](./literals.md#guardrailsensitiveinformationpolicyactiontype) 
## GuardrailTopicTypeDef

```python
# GuardrailTopicTypeDef definition

class GuardrailTopicTypeDef(TypedDict):
    action: NotRequired[GuardrailTopicPolicyActionType],  # (1)
    name: NotRequired[str],
    type: NotRequired[GuardrailTopicTypeType],  # (2)
```

1. See [:material-code-brackets: GuardrailTopicPolicyActionType](./literals.md#guardrailtopicpolicyactiontype) 
2. See [:material-code-brackets: GuardrailTopicTypeType](./literals.md#guardrailtopictypetype) 
## MetadataAttributeSchemaTypeDef

```python
# MetadataAttributeSchemaTypeDef definition

class MetadataAttributeSchemaTypeDef(TypedDict):
    description: str,
    key: str,
    type: AttributeTypeType,  # (1)
```

1. See [:material-code-brackets: AttributeTypeType](./literals.md#attributetypetype) 
## TextInferenceConfigTypeDef

```python
# TextInferenceConfigTypeDef definition

class TextInferenceConfigTypeDef(TypedDict):
    maxTokens: NotRequired[int],
    stopSequences: NotRequired[Sequence[str]],
    temperature: NotRequired[float],
    topP: NotRequired[float],
```

## InferenceConfigurationOutputTypeDef

```python
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
# InferenceConfigurationTypeDef definition

class InferenceConfigurationTypeDef(TypedDict):
    maximumLength: NotRequired[int],
    stopSequences: NotRequired[Sequence[str]],
    temperature: NotRequired[float],
    topK: NotRequired[int],
    topP: NotRequired[float],
```

## TextPromptTypeDef

```python
# TextPromptTypeDef definition

class TextPromptTypeDef(TypedDict):
    text: str,
```

## KnowledgeBaseLookupInputTypeDef

```python
# KnowledgeBaseLookupInputTypeDef definition

class KnowledgeBaseLookupInputTypeDef(TypedDict):
    knowledgeBaseId: NotRequired[str],
    text: NotRequired[str],
```

## StreamingConfigurationsTypeDef

```python
# StreamingConfigurationsTypeDef definition

class StreamingConfigurationsTypeDef(TypedDict):
    applyGuardrailInterval: NotRequired[int],
    streamFinalResponse: NotRequired[bool],
```

## KnowledgeBaseQueryTypeDef

```python
# KnowledgeBaseQueryTypeDef definition

class KnowledgeBaseQueryTypeDef(TypedDict):
    text: str,
```

## MemorySessionSummaryTypeDef

```python
# MemorySessionSummaryTypeDef definition

class MemorySessionSummaryTypeDef(TypedDict):
    memoryId: NotRequired[str],
    sessionExpiryTime: NotRequired[datetime],
    sessionId: NotRequired[str],
    sessionStartTime: NotRequired[datetime],
    summaryText: NotRequired[str],
```

## UsageTypeDef

```python
# UsageTypeDef definition

class UsageTypeDef(TypedDict):
    inputTokens: NotRequired[int],
    outputTokens: NotRequired[int],
```

## RepromptResponseTypeDef

```python
# RepromptResponseTypeDef definition

class RepromptResponseTypeDef(TypedDict):
    source: NotRequired[SourceType],  # (1)
    text: NotRequired[str],
```

1. See [:material-code-brackets: SourceType](./literals.md#sourcetype) 
## QueryTransformationConfigurationTypeDef

```python
# QueryTransformationConfigurationTypeDef definition

class QueryTransformationConfigurationTypeDef(TypedDict):
    type: QueryTransformationTypeType,  # (1)
```

1. See [:material-code-brackets: QueryTransformationTypeType](./literals.md#querytransformationtypetype) 
## RawResponseTypeDef

```python
# RawResponseTypeDef definition

class RawResponseTypeDef(TypedDict):
    content: NotRequired[str],
```

## RationaleTypeDef

```python
# RationaleTypeDef definition

class RationaleTypeDef(TypedDict):
    text: NotRequired[str],
    traceId: NotRequired[str],
```

## PostProcessingParsedResponseTypeDef

```python
# PostProcessingParsedResponseTypeDef definition

class PostProcessingParsedResponseTypeDef(TypedDict):
    text: NotRequired[str],
```

## PreProcessingParsedResponseTypeDef

```python
# PreProcessingParsedResponseTypeDef definition

class PreProcessingParsedResponseTypeDef(TypedDict):
    isValid: NotRequired[bool],
    rationale: NotRequired[str],
```

## RerankTextDocumentTypeDef

```python
# RerankTextDocumentTypeDef definition

class RerankTextDocumentTypeDef(TypedDict):
    text: NotRequired[str],
```

## RetrievalResultConfluenceLocationTypeDef

```python
# RetrievalResultConfluenceLocationTypeDef definition

class RetrievalResultConfluenceLocationTypeDef(TypedDict):
    url: NotRequired[str],
```

## RetrievalResultContentColumnTypeDef

```python
# RetrievalResultContentColumnTypeDef definition

class RetrievalResultContentColumnTypeDef(TypedDict):
    columnName: NotRequired[str],
    columnValue: NotRequired[str],
    type: NotRequired[RetrievalResultContentColumnTypeType],  # (1)
```

1. See [:material-code-brackets: RetrievalResultContentColumnTypeType](./literals.md#retrievalresultcontentcolumntypetype) 
## RetrievalResultCustomDocumentLocationTypeDef

```python
# RetrievalResultCustomDocumentLocationTypeDef definition

class RetrievalResultCustomDocumentLocationTypeDef(TypedDict):
    id: NotRequired[str],
```

## RetrievalResultKendraDocumentLocationTypeDef

```python
# RetrievalResultKendraDocumentLocationTypeDef definition

class RetrievalResultKendraDocumentLocationTypeDef(TypedDict):
    uri: NotRequired[str],
```

## RetrievalResultS3LocationTypeDef

```python
# RetrievalResultS3LocationTypeDef definition

class RetrievalResultS3LocationTypeDef(TypedDict):
    uri: NotRequired[str],
```

## RetrievalResultSalesforceLocationTypeDef

```python
# RetrievalResultSalesforceLocationTypeDef definition

class RetrievalResultSalesforceLocationTypeDef(TypedDict):
    url: NotRequired[str],
```

## RetrievalResultSharePointLocationTypeDef

```python
# RetrievalResultSharePointLocationTypeDef definition

class RetrievalResultSharePointLocationTypeDef(TypedDict):
    url: NotRequired[str],
```

## RetrievalResultSqlLocationTypeDef

```python
# RetrievalResultSqlLocationTypeDef definition

class RetrievalResultSqlLocationTypeDef(TypedDict):
    query: NotRequired[str],
```

## RetrievalResultWebLocationTypeDef

```python
# RetrievalResultWebLocationTypeDef definition

class RetrievalResultWebLocationTypeDef(TypedDict):
    url: NotRequired[str],
```

## RetrieveAndGenerateInputTypeDef

```python
# RetrieveAndGenerateInputTypeDef definition

class RetrieveAndGenerateInputTypeDef(TypedDict):
    text: str,
```

## RetrieveAndGenerateOutputEventTypeDef

```python
# RetrieveAndGenerateOutputEventTypeDef definition

class RetrieveAndGenerateOutputEventTypeDef(TypedDict):
    text: str,
```

## RetrieveAndGenerateOutputTypeDef

```python
# RetrieveAndGenerateOutputTypeDef definition

class RetrieveAndGenerateOutputTypeDef(TypedDict):
    text: str,
```

## RetrieveAndGenerateSessionConfigurationTypeDef

```python
# RetrieveAndGenerateSessionConfigurationTypeDef definition

class RetrieveAndGenerateSessionConfigurationTypeDef(TypedDict):
    kmsKeyArn: str,
```

## SpanTypeDef

```python
# SpanTypeDef definition

class SpanTypeDef(TypedDict):
    end: NotRequired[int],
    start: NotRequired[int],
```

## TextToSqlKnowledgeBaseConfigurationTypeDef

```python
# TextToSqlKnowledgeBaseConfigurationTypeDef definition

class TextToSqlKnowledgeBaseConfigurationTypeDef(TypedDict):
    knowledgeBaseArn: str,
```

## VectorSearchBedrockRerankingModelConfigurationTypeDef

```python
# VectorSearchBedrockRerankingModelConfigurationTypeDef definition

class VectorSearchBedrockRerankingModelConfigurationTypeDef(TypedDict):
    modelArn: str,
    additionalModelRequestFields: NotRequired[Mapping[str, Mapping[str, Any]]],
```

## APISchemaTypeDef

```python
# APISchemaTypeDef definition

class APISchemaTypeDef(TypedDict):
    payload: NotRequired[str],
    s3: NotRequired[S3IdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: S3IdentifierTypeDef](./type_defs.md#s3identifiertypedef) 
## PropertyParametersTypeDef

```python
# PropertyParametersTypeDef definition

class PropertyParametersTypeDef(TypedDict):
    properties: NotRequired[List[ParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
## RequestBodyTypeDef

```python
# RequestBodyTypeDef definition

class RequestBodyTypeDef(TypedDict):
    content: NotRequired[Dict[str, List[ParameterTypeDef]]],  # (1)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
## ApiResultOutputTypeDef

```python
# ApiResultOutputTypeDef definition

class ApiResultOutputTypeDef(TypedDict):
    actionGroup: str,
    agentId: NotRequired[str],
    apiPath: NotRequired[str],
    confirmationState: NotRequired[ConfirmationStateType],  # (1)
    httpMethod: NotRequired[str],
    httpStatusCode: NotRequired[int],
    responseBody: NotRequired[Dict[str, ContentBodyTypeDef]],  # (2)
    responseState: NotRequired[ResponseStateType],  # (3)
```

1. See [:material-code-brackets: ConfirmationStateType](./literals.md#confirmationstatetype) 
2. See [:material-code-braces: ContentBodyTypeDef](./type_defs.md#contentbodytypedef) 
3. See [:material-code-brackets: ResponseStateType](./literals.md#responsestatetype) 
## ApiResultTypeDef

```python
# ApiResultTypeDef definition

class ApiResultTypeDef(TypedDict):
    actionGroup: str,
    agentId: NotRequired[str],
    apiPath: NotRequired[str],
    confirmationState: NotRequired[ConfirmationStateType],  # (1)
    httpMethod: NotRequired[str],
    httpStatusCode: NotRequired[int],
    responseBody: NotRequired[Mapping[str, ContentBodyTypeDef]],  # (2)
    responseState: NotRequired[ResponseStateType],  # (3)
```

1. See [:material-code-brackets: ConfirmationStateType](./literals.md#confirmationstatetype) 
2. See [:material-code-braces: ContentBodyTypeDef](./type_defs.md#contentbodytypedef) 
3. See [:material-code-brackets: ResponseStateType](./literals.md#responsestatetype) 
## FunctionResultOutputTypeDef

```python
# FunctionResultOutputTypeDef definition

class FunctionResultOutputTypeDef(TypedDict):
    actionGroup: str,
    agentId: NotRequired[str],
    confirmationState: NotRequired[ConfirmationStateType],  # (1)
    function: NotRequired[str],
    responseBody: NotRequired[Dict[str, ContentBodyTypeDef]],  # (2)
    responseState: NotRequired[ResponseStateType],  # (3)
```

1. See [:material-code-brackets: ConfirmationStateType](./literals.md#confirmationstatetype) 
2. See [:material-code-braces: ContentBodyTypeDef](./type_defs.md#contentbodytypedef) 
3. See [:material-code-brackets: ResponseStateType](./literals.md#responsestatetype) 
## FunctionResultTypeDef

```python
# FunctionResultTypeDef definition

class FunctionResultTypeDef(TypedDict):
    actionGroup: str,
    agentId: NotRequired[str],
    confirmationState: NotRequired[ConfirmationStateType],  # (1)
    function: NotRequired[str],
    responseBody: NotRequired[Mapping[str, ContentBodyTypeDef]],  # (2)
    responseState: NotRequired[ResponseStateType],  # (3)
```

1. See [:material-code-brackets: ConfirmationStateType](./literals.md#confirmationstatetype) 
2. See [:material-code-braces: ContentBodyTypeDef](./type_defs.md#contentbodytypedef) 
3. See [:material-code-brackets: ResponseStateType](./literals.md#responsestatetype) 
## BedrockRerankingConfigurationTypeDef

```python
# BedrockRerankingConfigurationTypeDef definition

class BedrockRerankingConfigurationTypeDef(TypedDict):
    modelConfiguration: BedrockRerankingModelConfigurationTypeDef,  # (1)
    numberOfResults: NotRequired[int],
```

1. See [:material-code-braces: BedrockRerankingModelConfigurationTypeDef](./type_defs.md#bedrockrerankingmodelconfigurationtypedef) 
## ByteContentDocTypeDef

```python
# ByteContentDocTypeDef definition

class ByteContentDocTypeDef(TypedDict):
    contentType: str,
    data: BlobTypeDef,
    identifier: str,
```

## ByteContentFileTypeDef

```python
# ByteContentFileTypeDef definition

class ByteContentFileTypeDef(TypedDict):
    data: BlobTypeDef,
    mediaType: str,
```

## MessageTypeDef

```python
# MessageTypeDef definition

class MessageTypeDef(TypedDict):
    content: Sequence[ContentBlockTypeDef],  # (1)
    role: ConversationRoleType,  # (2)
```

1. See [:material-code-braces: ContentBlockTypeDef](./type_defs.md#contentblocktypedef) 
2. See [:material-code-brackets: ConversationRoleType](./literals.md#conversationroletype) 
## CustomOrchestrationTraceTypeDef

```python
# CustomOrchestrationTraceTypeDef definition

class CustomOrchestrationTraceTypeDef(TypedDict):
    event: NotRequired[CustomOrchestrationTraceEventTypeDef],  # (1)
    traceId: NotRequired[str],
```

1. See [:material-code-braces: CustomOrchestrationTraceEventTypeDef](./type_defs.md#customorchestrationtraceeventtypedef) 
## RerankingMetadataSelectiveModeConfigurationTypeDef

```python
# RerankingMetadataSelectiveModeConfigurationTypeDef definition

class RerankingMetadataSelectiveModeConfigurationTypeDef(TypedDict):
    fieldsToExclude: NotRequired[Sequence[FieldForRerankingTypeDef]],  # (1)
    fieldsToInclude: NotRequired[Sequence[FieldForRerankingTypeDef]],  # (1)
```

1. See [:material-code-braces: FieldForRerankingTypeDef](./type_defs.md#fieldforrerankingtypedef) 
2. See [:material-code-braces: FieldForRerankingTypeDef](./type_defs.md#fieldforrerankingtypedef) 
## FilePartTypeDef

```python
# FilePartTypeDef definition

class FilePartTypeDef(TypedDict):
    files: NotRequired[List[OutputFileTypeDef]],  # (1)
```

1. See [:material-code-braces: OutputFileTypeDef](./type_defs.md#outputfiletypedef) 
## InlineAgentFilePartTypeDef

```python
# InlineAgentFilePartTypeDef definition

class InlineAgentFilePartTypeDef(TypedDict):
    files: NotRequired[List[OutputFileTypeDef]],  # (1)
```

1. See [:material-code-braces: OutputFileTypeDef](./type_defs.md#outputfiletypedef) 
## RetrievalFilterPaginatorTypeDef

```python
# RetrievalFilterPaginatorTypeDef definition

class RetrievalFilterPaginatorTypeDef(TypedDict):
    andAll: NotRequired[Sequence[Mapping[str, Any]]],
    equals: NotRequired[FilterAttributeTypeDef],  # (1)
    greaterThan: NotRequired[FilterAttributeTypeDef],  # (1)
    greaterThanOrEquals: NotRequired[FilterAttributeTypeDef],  # (1)
    in: NotRequired[FilterAttributeTypeDef],  # (1)
    lessThan: NotRequired[FilterAttributeTypeDef],  # (1)
    lessThanOrEquals: NotRequired[FilterAttributeTypeDef],  # (1)
    listContains: NotRequired[FilterAttributeTypeDef],  # (1)
    notEquals: NotRequired[FilterAttributeTypeDef],  # (1)
    notIn: NotRequired[FilterAttributeTypeDef],  # (1)
    orAll: NotRequired[Sequence[Mapping[str, Any]]],
    startsWith: NotRequired[FilterAttributeTypeDef],  # (1)
    stringContains: NotRequired[FilterAttributeTypeDef],  # (1)
```

1. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
2. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
3. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
4. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
5. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
6. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
7. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
8. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
9. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
10. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
11. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
## RetrievalFilterTypeDef

```python
# RetrievalFilterTypeDef definition

class RetrievalFilterTypeDef(TypedDict):
    andAll: NotRequired[Sequence[Mapping[str, Any]]],
    equals: NotRequired[FilterAttributeTypeDef],  # (1)
    greaterThan: NotRequired[FilterAttributeTypeDef],  # (1)
    greaterThanOrEquals: NotRequired[FilterAttributeTypeDef],  # (1)
    in: NotRequired[FilterAttributeTypeDef],  # (1)
    lessThan: NotRequired[FilterAttributeTypeDef],  # (1)
    lessThanOrEquals: NotRequired[FilterAttributeTypeDef],  # (1)
    listContains: NotRequired[FilterAttributeTypeDef],  # (1)
    notEquals: NotRequired[FilterAttributeTypeDef],  # (1)
    notIn: NotRequired[FilterAttributeTypeDef],  # (1)
    orAll: NotRequired[Sequence[Mapping[str, Any]]],
    startsWith: NotRequired[FilterAttributeTypeDef],  # (1)
    stringContains: NotRequired[FilterAttributeTypeDef],  # (1)
```

1. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
2. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
3. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
4. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
5. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
6. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
7. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
8. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
9. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
10. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
11. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
## FlowInputTypeDef

```python
# FlowInputTypeDef definition

class FlowInputTypeDef(TypedDict):
    content: FlowInputContentTypeDef,  # (1)
    nodeName: str,
    nodeOutputName: str,
```

1. See [:material-code-braces: FlowInputContentTypeDef](./type_defs.md#flowinputcontenttypedef) 
## FlowOutputEventTypeDef

```python
# FlowOutputEventTypeDef definition

class FlowOutputEventTypeDef(TypedDict):
    content: FlowOutputContentTypeDef,  # (1)
    nodeName: str,
    nodeType: NodeTypeType,  # (2)
```

1. See [:material-code-braces: FlowOutputContentTypeDef](./type_defs.md#flowoutputcontenttypedef) 
2. See [:material-code-brackets: NodeTypeType](./literals.md#nodetypetype) 
## FlowTraceConditionNodeResultEventTypeDef

```python
# FlowTraceConditionNodeResultEventTypeDef definition

class FlowTraceConditionNodeResultEventTypeDef(TypedDict):
    nodeName: str,
    satisfiedConditions: List[FlowTraceConditionTypeDef],  # (1)
    timestamp: datetime,
```

1. See [:material-code-braces: FlowTraceConditionTypeDef](./type_defs.md#flowtraceconditiontypedef) 
## FlowTraceNodeInputFieldTypeDef

```python
# FlowTraceNodeInputFieldTypeDef definition

class FlowTraceNodeInputFieldTypeDef(TypedDict):
    content: FlowTraceNodeInputContentTypeDef,  # (1)
    nodeInputName: str,
```

1. See [:material-code-braces: FlowTraceNodeInputContentTypeDef](./type_defs.md#flowtracenodeinputcontenttypedef) 
## FlowTraceNodeOutputFieldTypeDef

```python
# FlowTraceNodeOutputFieldTypeDef definition

class FlowTraceNodeOutputFieldTypeDef(TypedDict):
    content: FlowTraceNodeOutputContentTypeDef,  # (1)
    nodeOutputName: str,
```

1. See [:material-code-braces: FlowTraceNodeOutputContentTypeDef](./type_defs.md#flowtracenodeoutputcontenttypedef) 
## FunctionDefinitionTypeDef

```python
# FunctionDefinitionTypeDef definition

class FunctionDefinitionTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    parameters: NotRequired[Mapping[str, ParameterDetailTypeDef]],  # (1)
    requireConfirmation: NotRequired[RequireConfirmationType],  # (2)
```

1. See [:material-code-braces: ParameterDetailTypeDef](./type_defs.md#parameterdetailtypedef) 
2. See [:material-code-brackets: RequireConfirmationType](./literals.md#requireconfirmationtype) 
## FunctionInvocationInputTypeDef

```python
# FunctionInvocationInputTypeDef definition

class FunctionInvocationInputTypeDef(TypedDict):
    actionGroup: str,
    actionInvocationType: NotRequired[ActionInvocationTypeType],  # (1)
    agentId: NotRequired[str],
    collaboratorName: NotRequired[str],
    function: NotRequired[str],
    parameters: NotRequired[List[FunctionParameterTypeDef]],  # (2)
```

1. See [:material-code-brackets: ActionInvocationTypeType](./literals.md#actioninvocationtypetype) 
2. See [:material-code-braces: FunctionParameterTypeDef](./type_defs.md#functionparametertypedef) 
## GenerateQueryResponseTypeDef

```python
# GenerateQueryResponseTypeDef definition

class GenerateQueryResponseTypeDef(TypedDict):
    queries: List[GeneratedQueryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GeneratedQueryTypeDef](./type_defs.md#generatedquerytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAgentMemoryRequestGetAgentMemoryPaginateTypeDef

```python
# GetAgentMemoryRequestGetAgentMemoryPaginateTypeDef definition

class GetAgentMemoryRequestGetAgentMemoryPaginateTypeDef(TypedDict):
    agentAliasId: str,
    agentId: str,
    memoryId: str,
    memoryType: MemoryTypeType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: MemoryTypeType](./literals.md#memorytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GuardrailContentPolicyAssessmentTypeDef

```python
# GuardrailContentPolicyAssessmentTypeDef definition

class GuardrailContentPolicyAssessmentTypeDef(TypedDict):
    filters: NotRequired[List[GuardrailContentFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: GuardrailContentFilterTypeDef](./type_defs.md#guardrailcontentfiltertypedef) 
## GuardrailWordPolicyAssessmentTypeDef

```python
# GuardrailWordPolicyAssessmentTypeDef definition

class GuardrailWordPolicyAssessmentTypeDef(TypedDict):
    customWords: NotRequired[List[GuardrailCustomWordTypeDef]],  # (1)
    managedWordLists: NotRequired[List[GuardrailManagedWordTypeDef]],  # (2)
```

1. See [:material-code-braces: GuardrailCustomWordTypeDef](./type_defs.md#guardrailcustomwordtypedef) 
2. See [:material-code-braces: GuardrailManagedWordTypeDef](./type_defs.md#guardrailmanagedwordtypedef) 
## GuardrailSensitiveInformationPolicyAssessmentTypeDef

```python
# GuardrailSensitiveInformationPolicyAssessmentTypeDef definition

class GuardrailSensitiveInformationPolicyAssessmentTypeDef(TypedDict):
    piiEntities: NotRequired[List[GuardrailPiiEntityFilterTypeDef]],  # (1)
    regexes: NotRequired[List[GuardrailRegexFilterTypeDef]],  # (2)
```

1. See [:material-code-braces: GuardrailPiiEntityFilterTypeDef](./type_defs.md#guardrailpiientityfiltertypedef) 
2. See [:material-code-braces: GuardrailRegexFilterTypeDef](./type_defs.md#guardrailregexfiltertypedef) 
## GuardrailTopicPolicyAssessmentTypeDef

```python
# GuardrailTopicPolicyAssessmentTypeDef definition

class GuardrailTopicPolicyAssessmentTypeDef(TypedDict):
    topics: NotRequired[List[GuardrailTopicTypeDef]],  # (1)
```

1. See [:material-code-braces: GuardrailTopicTypeDef](./type_defs.md#guardrailtopictypedef) 
## ImplicitFilterConfigurationTypeDef

```python
# ImplicitFilterConfigurationTypeDef definition

class ImplicitFilterConfigurationTypeDef(TypedDict):
    metadataAttributes: Sequence[MetadataAttributeSchemaTypeDef],  # (1)
    modelArn: str,
```

1. See [:material-code-braces: MetadataAttributeSchemaTypeDef](./type_defs.md#metadataattributeschematypedef) 
## InferenceConfigTypeDef

```python
# InferenceConfigTypeDef definition

class InferenceConfigTypeDef(TypedDict):
    textInferenceConfig: NotRequired[TextInferenceConfigTypeDef],  # (1)
```

1. See [:material-code-braces: TextInferenceConfigTypeDef](./type_defs.md#textinferenceconfigtypedef) 
## ModelInvocationInputTypeDef

```python
# ModelInvocationInputTypeDef definition

class ModelInvocationInputTypeDef(TypedDict):
    foundationModel: NotRequired[str],
    inferenceConfiguration: NotRequired[InferenceConfigurationOutputTypeDef],  # (1)
    overrideLambda: NotRequired[str],
    parserMode: NotRequired[CreationModeType],  # (2)
    promptCreationMode: NotRequired[CreationModeType],  # (2)
    text: NotRequired[str],
    traceId: NotRequired[str],
    type: NotRequired[PromptTypeType],  # (4)
```

1. See [:material-code-braces: InferenceConfigurationOutputTypeDef](./type_defs.md#inferenceconfigurationoutputtypedef) 
2. See [:material-code-brackets: CreationModeType](./literals.md#creationmodetype) 
3. See [:material-code-brackets: CreationModeType](./literals.md#creationmodetype) 
4. See [:material-code-brackets: PromptTypeType](./literals.md#prompttypetype) 
## InputPromptTypeDef

```python
# InputPromptTypeDef definition

class InputPromptTypeDef(TypedDict):
    textPrompt: NotRequired[TextPromptTypeDef],  # (1)
```

1. See [:material-code-braces: TextPromptTypeDef](./type_defs.md#textprompttypedef) 
## OptimizedPromptTypeDef

```python
# OptimizedPromptTypeDef definition

class OptimizedPromptTypeDef(TypedDict):
    textPrompt: NotRequired[TextPromptTypeDef],  # (1)
```

1. See [:material-code-braces: TextPromptTypeDef](./type_defs.md#textprompttypedef) 
## MemoryTypeDef

```python
# MemoryTypeDef definition

class MemoryTypeDef(TypedDict):
    sessionSummary: NotRequired[MemorySessionSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: MemorySessionSummaryTypeDef](./type_defs.md#memorysessionsummarytypedef) 
## MetadataTypeDef

```python
# MetadataTypeDef definition

class MetadataTypeDef(TypedDict):
    usage: NotRequired[UsageTypeDef],  # (1)
```

1. See [:material-code-braces: UsageTypeDef](./type_defs.md#usagetypedef) 
## RerankDocumentOutputTypeDef

```python
# RerankDocumentOutputTypeDef definition

class RerankDocumentOutputTypeDef(TypedDict):
    type: RerankDocumentTypeType,  # (2)
    jsonDocument: NotRequired[Dict[str, Any]],
    textDocument: NotRequired[RerankTextDocumentTypeDef],  # (1)
```

1. See [:material-code-braces: RerankTextDocumentTypeDef](./type_defs.md#reranktextdocumenttypedef) 
2. See [:material-code-brackets: RerankDocumentTypeType](./literals.md#rerankdocumenttypetype) 
## RerankDocumentTypeDef

```python
# RerankDocumentTypeDef definition

class RerankDocumentTypeDef(TypedDict):
    type: RerankDocumentTypeType,  # (2)
    jsonDocument: NotRequired[Mapping[str, Any]],
    textDocument: NotRequired[RerankTextDocumentTypeDef],  # (1)
```

1. See [:material-code-braces: RerankTextDocumentTypeDef](./type_defs.md#reranktextdocumenttypedef) 
2. See [:material-code-brackets: RerankDocumentTypeType](./literals.md#rerankdocumenttypetype) 
## RerankQueryTypeDef

```python
# RerankQueryTypeDef definition

class RerankQueryTypeDef(TypedDict):
    textQuery: RerankTextDocumentTypeDef,  # (1)
    type: RerankQueryContentTypeType,  # (2)
```

1. See [:material-code-braces: RerankTextDocumentTypeDef](./type_defs.md#reranktextdocumenttypedef) 
2. See [:material-code-brackets: RerankQueryContentTypeType](./literals.md#rerankquerycontenttypetype) 
## RetrievalResultContentTypeDef

```python
# RetrievalResultContentTypeDef definition

class RetrievalResultContentTypeDef(TypedDict):
    byteContent: NotRequired[str],
    row: NotRequired[List[RetrievalResultContentColumnTypeDef]],  # (1)
    text: NotRequired[str],
    type: NotRequired[RetrievalResultContentTypeType],  # (2)
```

1. See [:material-code-braces: RetrievalResultContentColumnTypeDef](./type_defs.md#retrievalresultcontentcolumntypedef) 
2. See [:material-code-brackets: RetrievalResultContentTypeType](./literals.md#retrievalresultcontenttypetype) 
## RetrievalResultLocationTypeDef

```python
# RetrievalResultLocationTypeDef definition

class RetrievalResultLocationTypeDef(TypedDict):
    type: RetrievalResultLocationTypeType,  # (8)
    confluenceLocation: NotRequired[RetrievalResultConfluenceLocationTypeDef],  # (1)
    customDocumentLocation: NotRequired[RetrievalResultCustomDocumentLocationTypeDef],  # (2)
    kendraDocumentLocation: NotRequired[RetrievalResultKendraDocumentLocationTypeDef],  # (3)
    s3Location: NotRequired[RetrievalResultS3LocationTypeDef],  # (4)
    salesforceLocation: NotRequired[RetrievalResultSalesforceLocationTypeDef],  # (5)
    sharePointLocation: NotRequired[RetrievalResultSharePointLocationTypeDef],  # (6)
    sqlLocation: NotRequired[RetrievalResultSqlLocationTypeDef],  # (7)
    webLocation: NotRequired[RetrievalResultWebLocationTypeDef],  # (9)
```

1. See [:material-code-braces: RetrievalResultConfluenceLocationTypeDef](./type_defs.md#retrievalresultconfluencelocationtypedef) 
2. See [:material-code-braces: RetrievalResultCustomDocumentLocationTypeDef](./type_defs.md#retrievalresultcustomdocumentlocationtypedef) 
3. See [:material-code-braces: RetrievalResultKendraDocumentLocationTypeDef](./type_defs.md#retrievalresultkendradocumentlocationtypedef) 
4. See [:material-code-braces: RetrievalResultS3LocationTypeDef](./type_defs.md#retrievalresults3locationtypedef) 
5. See [:material-code-braces: RetrievalResultSalesforceLocationTypeDef](./type_defs.md#retrievalresultsalesforcelocationtypedef) 
6. See [:material-code-braces: RetrievalResultSharePointLocationTypeDef](./type_defs.md#retrievalresultsharepointlocationtypedef) 
7. See [:material-code-braces: RetrievalResultSqlLocationTypeDef](./type_defs.md#retrievalresultsqllocationtypedef) 
8. See [:material-code-brackets: RetrievalResultLocationTypeType](./literals.md#retrievalresultlocationtypetype) 
9. See [:material-code-braces: RetrievalResultWebLocationTypeDef](./type_defs.md#retrievalresultweblocationtypedef) 
## TextResponsePartTypeDef

```python
# TextResponsePartTypeDef definition

class TextResponsePartTypeDef(TypedDict):
    span: NotRequired[SpanTypeDef],  # (1)
    text: NotRequired[str],
```

1. See [:material-code-braces: SpanTypeDef](./type_defs.md#spantypedef) 
## TextToSqlConfigurationTypeDef

```python
# TextToSqlConfigurationTypeDef definition

class TextToSqlConfigurationTypeDef(TypedDict):
    type: TextToSqlConfigurationTypeType,  # (2)
    knowledgeBaseConfiguration: NotRequired[TextToSqlKnowledgeBaseConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: TextToSqlKnowledgeBaseConfigurationTypeDef](./type_defs.md#texttosqlknowledgebaseconfigurationtypedef) 
2. See [:material-code-brackets: TextToSqlConfigurationTypeType](./literals.md#texttosqlconfigurationtypetype) 
## ApiRequestBodyTypeDef

```python
# ApiRequestBodyTypeDef definition

class ApiRequestBodyTypeDef(TypedDict):
    content: NotRequired[Dict[str, PropertyParametersTypeDef]],  # (1)
```

1. See [:material-code-braces: PropertyParametersTypeDef](./type_defs.md#propertyparameterstypedef) 
## ActionGroupInvocationInputTypeDef

```python
# ActionGroupInvocationInputTypeDef definition

class ActionGroupInvocationInputTypeDef(TypedDict):
    actionGroupName: NotRequired[str],
    apiPath: NotRequired[str],
    executionType: NotRequired[ExecutionTypeType],  # (1)
    function: NotRequired[str],
    invocationId: NotRequired[str],
    parameters: NotRequired[List[ParameterTypeDef]],  # (2)
    requestBody: NotRequired[RequestBodyTypeDef],  # (3)
    verb: NotRequired[str],
```

1. See [:material-code-brackets: ExecutionTypeType](./literals.md#executiontypetype) 
2. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
3. See [:material-code-braces: RequestBodyTypeDef](./type_defs.md#requestbodytypedef) 
## InvocationResultMemberOutputTypeDef

```python
# InvocationResultMemberOutputTypeDef definition

class InvocationResultMemberOutputTypeDef(TypedDict):
    apiResult: NotRequired[ApiResultOutputTypeDef],  # (1)
    functionResult: NotRequired[FunctionResultOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ApiResultOutputTypeDef](./type_defs.md#apiresultoutputtypedef) 
2. See [:material-code-braces: FunctionResultOutputTypeDef](./type_defs.md#functionresultoutputtypedef) 
## RerankingConfigurationTypeDef

```python
# RerankingConfigurationTypeDef definition

class RerankingConfigurationTypeDef(TypedDict):
    bedrockRerankingConfiguration: BedrockRerankingConfigurationTypeDef,  # (1)
    type: RerankingConfigurationTypeType,  # (2)
```

1. See [:material-code-braces: BedrockRerankingConfigurationTypeDef](./type_defs.md#bedrockrerankingconfigurationtypedef) 
2. See [:material-code-brackets: RerankingConfigurationTypeType](./literals.md#rerankingconfigurationtypetype) 
## ExternalSourceTypeDef

```python
# ExternalSourceTypeDef definition

class ExternalSourceTypeDef(TypedDict):
    sourceType: ExternalSourceTypeType,  # (3)
    byteContent: NotRequired[ByteContentDocTypeDef],  # (1)
    s3Location: NotRequired[S3ObjectDocTypeDef],  # (2)
```

1. See [:material-code-braces: ByteContentDocTypeDef](./type_defs.md#bytecontentdoctypedef) 
2. See [:material-code-braces: S3ObjectDocTypeDef](./type_defs.md#s3objectdoctypedef) 
3. See [:material-code-brackets: ExternalSourceTypeType](./literals.md#externalsourcetypetype) 
## FileSourceTypeDef

```python
# FileSourceTypeDef definition

class FileSourceTypeDef(TypedDict):
    sourceType: FileSourceTypeType,  # (3)
    byteContent: NotRequired[ByteContentFileTypeDef],  # (1)
    s3Location: NotRequired[S3ObjectFileTypeDef],  # (2)
```

1. See [:material-code-braces: ByteContentFileTypeDef](./type_defs.md#bytecontentfiletypedef) 
2. See [:material-code-braces: S3ObjectFileTypeDef](./type_defs.md#s3objectfiletypedef) 
3. See [:material-code-brackets: FileSourceTypeType](./literals.md#filesourcetypetype) 
## ConversationHistoryTypeDef

```python
# ConversationHistoryTypeDef definition

class ConversationHistoryTypeDef(TypedDict):
    messages: NotRequired[Sequence[MessageTypeDef]],  # (1)
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
## MetadataConfigurationForRerankingTypeDef

```python
# MetadataConfigurationForRerankingTypeDef definition

class MetadataConfigurationForRerankingTypeDef(TypedDict):
    selectionMode: RerankingMetadataSelectionModeType,  # (1)
    selectiveModeConfiguration: NotRequired[RerankingMetadataSelectiveModeConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: RerankingMetadataSelectionModeType](./literals.md#rerankingmetadataselectionmodetype) 
2. See [:material-code-braces: RerankingMetadataSelectiveModeConfigurationTypeDef](./type_defs.md#rerankingmetadataselectivemodeconfigurationtypedef) 
## InvokeFlowRequestRequestTypeDef

```python
# InvokeFlowRequestRequestTypeDef definition

class InvokeFlowRequestRequestTypeDef(TypedDict):
    flowAliasIdentifier: str,
    flowIdentifier: str,
    inputs: Sequence[FlowInputTypeDef],  # (1)
    enableTrace: NotRequired[bool],
```

1. See [:material-code-braces: FlowInputTypeDef](./type_defs.md#flowinputtypedef) 
## FlowTraceNodeInputEventTypeDef

```python
# FlowTraceNodeInputEventTypeDef definition

class FlowTraceNodeInputEventTypeDef(TypedDict):
    fields: List[FlowTraceNodeInputFieldTypeDef],  # (1)
    nodeName: str,
    timestamp: datetime,
```

1. See [:material-code-braces: FlowTraceNodeInputFieldTypeDef](./type_defs.md#flowtracenodeinputfieldtypedef) 
## FlowTraceNodeOutputEventTypeDef

```python
# FlowTraceNodeOutputEventTypeDef definition

class FlowTraceNodeOutputEventTypeDef(TypedDict):
    fields: List[FlowTraceNodeOutputFieldTypeDef],  # (1)
    nodeName: str,
    timestamp: datetime,
```

1. See [:material-code-braces: FlowTraceNodeOutputFieldTypeDef](./type_defs.md#flowtracenodeoutputfieldtypedef) 
## FunctionSchemaTypeDef

```python
# FunctionSchemaTypeDef definition

class FunctionSchemaTypeDef(TypedDict):
    functions: NotRequired[Sequence[FunctionDefinitionTypeDef]],  # (1)
```

1. See [:material-code-braces: FunctionDefinitionTypeDef](./type_defs.md#functiondefinitiontypedef) 
## GuardrailAssessmentTypeDef

```python
# GuardrailAssessmentTypeDef definition

class GuardrailAssessmentTypeDef(TypedDict):
    contentPolicy: NotRequired[GuardrailContentPolicyAssessmentTypeDef],  # (1)
    sensitiveInformationPolicy: NotRequired[GuardrailSensitiveInformationPolicyAssessmentTypeDef],  # (2)
    topicPolicy: NotRequired[GuardrailTopicPolicyAssessmentTypeDef],  # (3)
    wordPolicy: NotRequired[GuardrailWordPolicyAssessmentTypeDef],  # (4)
```

1. See [:material-code-braces: GuardrailContentPolicyAssessmentTypeDef](./type_defs.md#guardrailcontentpolicyassessmenttypedef) 
2. See [:material-code-braces: GuardrailSensitiveInformationPolicyAssessmentTypeDef](./type_defs.md#guardrailsensitiveinformationpolicyassessmenttypedef) 
3. See [:material-code-braces: GuardrailTopicPolicyAssessmentTypeDef](./type_defs.md#guardrailtopicpolicyassessmenttypedef) 
4. See [:material-code-braces: GuardrailWordPolicyAssessmentTypeDef](./type_defs.md#guardrailwordpolicyassessmenttypedef) 
## ExternalSourcesGenerationConfigurationTypeDef

```python
# ExternalSourcesGenerationConfigurationTypeDef definition

class ExternalSourcesGenerationConfigurationTypeDef(TypedDict):
    additionalModelRequestFields: NotRequired[Mapping[str, Mapping[str, Any]]],
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (1)
    inferenceConfig: NotRequired[InferenceConfigTypeDef],  # (2)
    promptTemplate: NotRequired[PromptTemplateTypeDef],  # (3)
```

1. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
2. See [:material-code-braces: InferenceConfigTypeDef](./type_defs.md#inferenceconfigtypedef) 
3. See [:material-code-braces: PromptTemplateTypeDef](./type_defs.md#prompttemplatetypedef) 
## GenerationConfigurationTypeDef

```python
# GenerationConfigurationTypeDef definition

class GenerationConfigurationTypeDef(TypedDict):
    additionalModelRequestFields: NotRequired[Mapping[str, Mapping[str, Any]]],
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (1)
    inferenceConfig: NotRequired[InferenceConfigTypeDef],  # (2)
    promptTemplate: NotRequired[PromptTemplateTypeDef],  # (3)
```

1. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
2. See [:material-code-braces: InferenceConfigTypeDef](./type_defs.md#inferenceconfigtypedef) 
3. See [:material-code-braces: PromptTemplateTypeDef](./type_defs.md#prompttemplatetypedef) 
## OrchestrationConfigurationTypeDef

```python
# OrchestrationConfigurationTypeDef definition

class OrchestrationConfigurationTypeDef(TypedDict):
    additionalModelRequestFields: NotRequired[Mapping[str, Mapping[str, Any]]],
    inferenceConfig: NotRequired[InferenceConfigTypeDef],  # (1)
    promptTemplate: NotRequired[PromptTemplateTypeDef],  # (2)
    queryTransformationConfiguration: NotRequired[QueryTransformationConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: InferenceConfigTypeDef](./type_defs.md#inferenceconfigtypedef) 
2. See [:material-code-braces: PromptTemplateTypeDef](./type_defs.md#prompttemplatetypedef) 
3. See [:material-code-braces: QueryTransformationConfigurationTypeDef](./type_defs.md#querytransformationconfigurationtypedef) 
## PromptConfigurationTypeDef

```python
# PromptConfigurationTypeDef definition

class PromptConfigurationTypeDef(TypedDict):
    basePromptTemplate: NotRequired[str],
    inferenceConfiguration: NotRequired[InferenceConfigurationUnionTypeDef],  # (1)
    parserMode: NotRequired[CreationModeType],  # (2)
    promptCreationMode: NotRequired[CreationModeType],  # (2)
    promptState: NotRequired[PromptStateType],  # (4)
    promptType: NotRequired[PromptTypeType],  # (5)
```

1. See [:material-code-braces: InferenceConfigurationTypeDef](./type_defs.md#inferenceconfigurationtypedef) [:material-code-braces: InferenceConfigurationOutputTypeDef](./type_defs.md#inferenceconfigurationoutputtypedef) 
2. See [:material-code-brackets: CreationModeType](./literals.md#creationmodetype) 
3. See [:material-code-brackets: CreationModeType](./literals.md#creationmodetype) 
4. See [:material-code-brackets: PromptStateType](./literals.md#promptstatetype) 
5. See [:material-code-brackets: PromptTypeType](./literals.md#prompttypetype) 
## OptimizePromptRequestRequestTypeDef

```python
# OptimizePromptRequestRequestTypeDef definition

class OptimizePromptRequestRequestTypeDef(TypedDict):
    input: InputPromptTypeDef,  # (1)
    targetModelId: str,
```

1. See [:material-code-braces: InputPromptTypeDef](./type_defs.md#inputprompttypedef) 
## OptimizedPromptEventTypeDef

```python
# OptimizedPromptEventTypeDef definition

class OptimizedPromptEventTypeDef(TypedDict):
    optimizedPrompt: NotRequired[OptimizedPromptTypeDef],  # (1)
```

1. See [:material-code-braces: OptimizedPromptTypeDef](./type_defs.md#optimizedprompttypedef) 
## GetAgentMemoryResponseTypeDef

```python
# GetAgentMemoryResponseTypeDef definition

class GetAgentMemoryResponseTypeDef(TypedDict):
    memoryContents: List[MemoryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MemoryTypeDef](./type_defs.md#memorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OrchestrationModelInvocationOutputTypeDef

```python
# OrchestrationModelInvocationOutputTypeDef definition

class OrchestrationModelInvocationOutputTypeDef(TypedDict):
    metadata: NotRequired[MetadataTypeDef],  # (1)
    rawResponse: NotRequired[RawResponseTypeDef],  # (2)
    traceId: NotRequired[str],
```

1. See [:material-code-braces: MetadataTypeDef](./type_defs.md#metadatatypedef) 
2. See [:material-code-braces: RawResponseTypeDef](./type_defs.md#rawresponsetypedef) 
## PostProcessingModelInvocationOutputTypeDef

```python
# PostProcessingModelInvocationOutputTypeDef definition

class PostProcessingModelInvocationOutputTypeDef(TypedDict):
    metadata: NotRequired[MetadataTypeDef],  # (1)
    parsedResponse: NotRequired[PostProcessingParsedResponseTypeDef],  # (2)
    rawResponse: NotRequired[RawResponseTypeDef],  # (3)
    traceId: NotRequired[str],
```

1. See [:material-code-braces: MetadataTypeDef](./type_defs.md#metadatatypedef) 
2. See [:material-code-braces: PostProcessingParsedResponseTypeDef](./type_defs.md#postprocessingparsedresponsetypedef) 
3. See [:material-code-braces: RawResponseTypeDef](./type_defs.md#rawresponsetypedef) 
## PreProcessingModelInvocationOutputTypeDef

```python
# PreProcessingModelInvocationOutputTypeDef definition

class PreProcessingModelInvocationOutputTypeDef(TypedDict):
    metadata: NotRequired[MetadataTypeDef],  # (1)
    parsedResponse: NotRequired[PreProcessingParsedResponseTypeDef],  # (2)
    rawResponse: NotRequired[RawResponseTypeDef],  # (3)
    traceId: NotRequired[str],
```

1. See [:material-code-braces: MetadataTypeDef](./type_defs.md#metadatatypedef) 
2. See [:material-code-braces: PreProcessingParsedResponseTypeDef](./type_defs.md#preprocessingparsedresponsetypedef) 
3. See [:material-code-braces: RawResponseTypeDef](./type_defs.md#rawresponsetypedef) 
## RoutingClassifierModelInvocationOutputTypeDef

```python
# RoutingClassifierModelInvocationOutputTypeDef definition

class RoutingClassifierModelInvocationOutputTypeDef(TypedDict):
    metadata: NotRequired[MetadataTypeDef],  # (1)
    rawResponse: NotRequired[RawResponseTypeDef],  # (2)
    traceId: NotRequired[str],
```

1. See [:material-code-braces: MetadataTypeDef](./type_defs.md#metadatatypedef) 
2. See [:material-code-braces: RawResponseTypeDef](./type_defs.md#rawresponsetypedef) 
## RerankResultTypeDef

```python
# RerankResultTypeDef definition

class RerankResultTypeDef(TypedDict):
    index: int,
    relevanceScore: float,
    document: NotRequired[RerankDocumentOutputTypeDef],  # (1)
```

1. See [:material-code-braces: RerankDocumentOutputTypeDef](./type_defs.md#rerankdocumentoutputtypedef) 
## KnowledgeBaseRetrievalResultTypeDef

```python
# KnowledgeBaseRetrievalResultTypeDef definition

class KnowledgeBaseRetrievalResultTypeDef(TypedDict):
    content: RetrievalResultContentTypeDef,  # (1)
    location: NotRequired[RetrievalResultLocationTypeDef],  # (2)
    metadata: NotRequired[Dict[str, Dict[str, Any]]],
    score: NotRequired[float],
```

1. See [:material-code-braces: RetrievalResultContentTypeDef](./type_defs.md#retrievalresultcontenttypedef) 
2. See [:material-code-braces: RetrievalResultLocationTypeDef](./type_defs.md#retrievalresultlocationtypedef) 
## RetrievedReferenceTypeDef

```python
# RetrievedReferenceTypeDef definition

class RetrievedReferenceTypeDef(TypedDict):
    content: NotRequired[RetrievalResultContentTypeDef],  # (1)
    location: NotRequired[RetrievalResultLocationTypeDef],  # (2)
    metadata: NotRequired[Dict[str, Dict[str, Any]]],
```

1. See [:material-code-braces: RetrievalResultContentTypeDef](./type_defs.md#retrievalresultcontenttypedef) 
2. See [:material-code-braces: RetrievalResultLocationTypeDef](./type_defs.md#retrievalresultlocationtypedef) 
## GeneratedResponsePartTypeDef

```python
# GeneratedResponsePartTypeDef definition

class GeneratedResponsePartTypeDef(TypedDict):
    textResponsePart: NotRequired[TextResponsePartTypeDef],  # (1)
```

1. See [:material-code-braces: TextResponsePartTypeDef](./type_defs.md#textresponseparttypedef) 
## TransformationConfigurationTypeDef

```python
# TransformationConfigurationTypeDef definition

class TransformationConfigurationTypeDef(TypedDict):
    mode: QueryTransformationModeType,  # (1)
    textToSqlConfiguration: NotRequired[TextToSqlConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: QueryTransformationModeType](./literals.md#querytransformationmodetype) 
2. See [:material-code-braces: TextToSqlConfigurationTypeDef](./type_defs.md#texttosqlconfigurationtypedef) 
## ApiInvocationInputTypeDef

```python
# ApiInvocationInputTypeDef definition

class ApiInvocationInputTypeDef(TypedDict):
    actionGroup: str,
    actionInvocationType: NotRequired[ActionInvocationTypeType],  # (1)
    agentId: NotRequired[str],
    apiPath: NotRequired[str],
    collaboratorName: NotRequired[str],
    httpMethod: NotRequired[str],
    parameters: NotRequired[List[ApiParameterTypeDef]],  # (2)
    requestBody: NotRequired[ApiRequestBodyTypeDef],  # (3)
```

1. See [:material-code-brackets: ActionInvocationTypeType](./literals.md#actioninvocationtypetype) 
2. See [:material-code-braces: ApiParameterTypeDef](./type_defs.md#apiparametertypedef) 
3. See [:material-code-braces: ApiRequestBodyTypeDef](./type_defs.md#apirequestbodytypedef) 
## ReturnControlResultsTypeDef

```python
# ReturnControlResultsTypeDef definition

class ReturnControlResultsTypeDef(TypedDict):
    invocationId: NotRequired[str],
    returnControlInvocationResults: NotRequired[List[InvocationResultMemberOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: InvocationResultMemberOutputTypeDef](./type_defs.md#invocationresultmemberoutputtypedef) 
## InvocationResultMemberTypeDef

```python
# InvocationResultMemberTypeDef definition

class InvocationResultMemberTypeDef(TypedDict):
    apiResult: NotRequired[ApiResultUnionTypeDef],  # (1)
    functionResult: NotRequired[FunctionResultUnionTypeDef],  # (2)
```

1. See [:material-code-braces: ApiResultTypeDef](./type_defs.md#apiresulttypedef) [:material-code-braces: ApiResultOutputTypeDef](./type_defs.md#apiresultoutputtypedef) 
2. See [:material-code-braces: FunctionResultTypeDef](./type_defs.md#functionresulttypedef) [:material-code-braces: FunctionResultOutputTypeDef](./type_defs.md#functionresultoutputtypedef) 
## InputFileTypeDef

```python
# InputFileTypeDef definition

class InputFileTypeDef(TypedDict):
    name: str,
    source: FileSourceTypeDef,  # (1)
    useCase: FileUseCaseType,  # (2)
```

1. See [:material-code-braces: FileSourceTypeDef](./type_defs.md#filesourcetypedef) 
2. See [:material-code-brackets: FileUseCaseType](./literals.md#fileusecasetype) 
## VectorSearchBedrockRerankingConfigurationTypeDef

```python
# VectorSearchBedrockRerankingConfigurationTypeDef definition

class VectorSearchBedrockRerankingConfigurationTypeDef(TypedDict):
    modelConfiguration: VectorSearchBedrockRerankingModelConfigurationTypeDef,  # (2)
    metadataConfiguration: NotRequired[MetadataConfigurationForRerankingTypeDef],  # (1)
    numberOfRerankedResults: NotRequired[int],
```

1. See [:material-code-braces: MetadataConfigurationForRerankingTypeDef](./type_defs.md#metadataconfigurationforrerankingtypedef) 
2. See [:material-code-braces: VectorSearchBedrockRerankingModelConfigurationTypeDef](./type_defs.md#vectorsearchbedrockrerankingmodelconfigurationtypedef) 
## FlowTraceTypeDef

```python
# FlowTraceTypeDef definition

class FlowTraceTypeDef(TypedDict):
    conditionNodeResultTrace: NotRequired[FlowTraceConditionNodeResultEventTypeDef],  # (1)
    nodeInputTrace: NotRequired[FlowTraceNodeInputEventTypeDef],  # (2)
    nodeOutputTrace: NotRequired[FlowTraceNodeOutputEventTypeDef],  # (3)
```

1. See [:material-code-braces: FlowTraceConditionNodeResultEventTypeDef](./type_defs.md#flowtraceconditionnoderesulteventtypedef) 
2. See [:material-code-braces: FlowTraceNodeInputEventTypeDef](./type_defs.md#flowtracenodeinputeventtypedef) 
3. See [:material-code-braces: FlowTraceNodeOutputEventTypeDef](./type_defs.md#flowtracenodeoutputeventtypedef) 
## AgentActionGroupTypeDef

```python
# AgentActionGroupTypeDef definition

class AgentActionGroupTypeDef(TypedDict):
    actionGroupName: str,
    actionGroupExecutor: NotRequired[ActionGroupExecutorTypeDef],  # (1)
    apiSchema: NotRequired[APISchemaTypeDef],  # (2)
    description: NotRequired[str],
    functionSchema: NotRequired[FunctionSchemaTypeDef],  # (3)
    parentActionGroupSignature: NotRequired[ActionGroupSignatureType],  # (4)
```

1. See [:material-code-braces: ActionGroupExecutorTypeDef](./type_defs.md#actiongroupexecutortypedef) 
2. See [:material-code-braces: APISchemaTypeDef](./type_defs.md#apischematypedef) 
3. See [:material-code-braces: FunctionSchemaTypeDef](./type_defs.md#functionschematypedef) 
4. See [:material-code-brackets: ActionGroupSignatureType](./literals.md#actiongroupsignaturetype) 
## GuardrailTraceTypeDef

```python
# GuardrailTraceTypeDef definition

class GuardrailTraceTypeDef(TypedDict):
    action: NotRequired[GuardrailActionType],  # (1)
    inputAssessments: NotRequired[List[GuardrailAssessmentTypeDef]],  # (2)
    outputAssessments: NotRequired[List[GuardrailAssessmentTypeDef]],  # (2)
    traceId: NotRequired[str],
```

1. See [:material-code-brackets: GuardrailActionType](./literals.md#guardrailactiontype) 
2. See [:material-code-braces: GuardrailAssessmentTypeDef](./type_defs.md#guardrailassessmenttypedef) 
3. See [:material-code-braces: GuardrailAssessmentTypeDef](./type_defs.md#guardrailassessmenttypedef) 
## ExternalSourcesRetrieveAndGenerateConfigurationTypeDef

```python
# ExternalSourcesRetrieveAndGenerateConfigurationTypeDef definition

class ExternalSourcesRetrieveAndGenerateConfigurationTypeDef(TypedDict):
    modelArn: str,
    sources: Sequence[ExternalSourceTypeDef],  # (2)
    generationConfiguration: NotRequired[ExternalSourcesGenerationConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ExternalSourcesGenerationConfigurationTypeDef](./type_defs.md#externalsourcesgenerationconfigurationtypedef) 
2. See [:material-code-braces: ExternalSourceTypeDef](./type_defs.md#externalsourcetypedef) 
## PromptOverrideConfigurationTypeDef

```python
# PromptOverrideConfigurationTypeDef definition

class PromptOverrideConfigurationTypeDef(TypedDict):
    promptConfigurations: Sequence[PromptConfigurationTypeDef],  # (1)
    overrideLambda: NotRequired[str],
```

1. See [:material-code-braces: PromptConfigurationTypeDef](./type_defs.md#promptconfigurationtypedef) 
## OptimizedPromptStreamTypeDef

```python
# OptimizedPromptStreamTypeDef definition

class OptimizedPromptStreamTypeDef(TypedDict):
    accessDeniedException: NotRequired[AccessDeniedExceptionTypeDef],  # (1)
    analyzePromptEvent: NotRequired[AnalyzePromptEventTypeDef],  # (2)
    badGatewayException: NotRequired[BadGatewayExceptionTypeDef],  # (3)
    dependencyFailedException: NotRequired[DependencyFailedExceptionTypeDef],  # (4)
    internalServerException: NotRequired[InternalServerExceptionTypeDef],  # (5)
    optimizedPromptEvent: NotRequired[OptimizedPromptEventTypeDef],  # (6)
    throttlingException: NotRequired[ThrottlingExceptionTypeDef],  # (7)
    validationException: NotRequired[ValidationExceptionTypeDef],  # (8)
```

1. See [:material-code-braces: AccessDeniedExceptionTypeDef](./type_defs.md#accessdeniedexceptiontypedef) 
2. See [:material-code-braces: AnalyzePromptEventTypeDef](./type_defs.md#analyzeprompteventtypedef) 
3. See [:material-code-braces: BadGatewayExceptionTypeDef](./type_defs.md#badgatewayexceptiontypedef) 
4. See [:material-code-braces: DependencyFailedExceptionTypeDef](./type_defs.md#dependencyfailedexceptiontypedef) 
5. See [:material-code-braces: InternalServerExceptionTypeDef](./type_defs.md#internalserverexceptiontypedef) 
6. See [:material-code-braces: OptimizedPromptEventTypeDef](./type_defs.md#optimizedprompteventtypedef) 
7. See [:material-code-braces: ThrottlingExceptionTypeDef](./type_defs.md#throttlingexceptiontypedef) 
8. See [:material-code-braces: ValidationExceptionTypeDef](./type_defs.md#validationexceptiontypedef) 
## PostProcessingTraceTypeDef

```python
# PostProcessingTraceTypeDef definition

class PostProcessingTraceTypeDef(TypedDict):
    modelInvocationInput: NotRequired[ModelInvocationInputTypeDef],  # (1)
    modelInvocationOutput: NotRequired[PostProcessingModelInvocationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ModelInvocationInputTypeDef](./type_defs.md#modelinvocationinputtypedef) 
2. See [:material-code-braces: PostProcessingModelInvocationOutputTypeDef](./type_defs.md#postprocessingmodelinvocationoutputtypedef) 
## PreProcessingTraceTypeDef

```python
# PreProcessingTraceTypeDef definition

class PreProcessingTraceTypeDef(TypedDict):
    modelInvocationInput: NotRequired[ModelInvocationInputTypeDef],  # (1)
    modelInvocationOutput: NotRequired[PreProcessingModelInvocationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ModelInvocationInputTypeDef](./type_defs.md#modelinvocationinputtypedef) 
2. See [:material-code-braces: PreProcessingModelInvocationOutputTypeDef](./type_defs.md#preprocessingmodelinvocationoutputtypedef) 
## RerankResponseTypeDef

```python
# RerankResponseTypeDef definition

class RerankResponseTypeDef(TypedDict):
    results: List[RerankResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RerankResultTypeDef](./type_defs.md#rerankresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RerankSourceTypeDef

```python
# RerankSourceTypeDef definition

class RerankSourceTypeDef(TypedDict):
    inlineDocumentSource: RerankDocumentUnionTypeDef,  # (1)
    type: RerankSourceTypeType,  # (2)
```

1. See [:material-code-braces: RerankDocumentTypeDef](./type_defs.md#rerankdocumenttypedef) [:material-code-braces: RerankDocumentOutputTypeDef](./type_defs.md#rerankdocumentoutputtypedef) 
2. See [:material-code-brackets: RerankSourceTypeType](./literals.md#reranksourcetypetype) 
## RetrieveResponseTypeDef

```python
# RetrieveResponseTypeDef definition

class RetrieveResponseTypeDef(TypedDict):
    guardrailAction: GuadrailActionType,  # (1)
    retrievalResults: List[KnowledgeBaseRetrievalResultTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: GuadrailActionType](./literals.md#guadrailactiontype) 
2. See [:material-code-braces: KnowledgeBaseRetrievalResultTypeDef](./type_defs.md#knowledgebaseretrievalresulttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## KnowledgeBaseLookupOutputTypeDef

```python
# KnowledgeBaseLookupOutputTypeDef definition

class KnowledgeBaseLookupOutputTypeDef(TypedDict):
    retrievedReferences: NotRequired[List[RetrievedReferenceTypeDef]],  # (1)
```

1. See [:material-code-braces: RetrievedReferenceTypeDef](./type_defs.md#retrievedreferencetypedef) 
## CitationTypeDef

```python
# CitationTypeDef definition

class CitationTypeDef(TypedDict):
    generatedResponsePart: NotRequired[GeneratedResponsePartTypeDef],  # (1)
    retrievedReferences: NotRequired[List[RetrievedReferenceTypeDef]],  # (2)
```

1. See [:material-code-braces: GeneratedResponsePartTypeDef](./type_defs.md#generatedresponseparttypedef) 
2. See [:material-code-braces: RetrievedReferenceTypeDef](./type_defs.md#retrievedreferencetypedef) 
## GenerateQueryRequestRequestTypeDef

```python
# GenerateQueryRequestRequestTypeDef definition

class GenerateQueryRequestRequestTypeDef(TypedDict):
    queryGenerationInput: QueryGenerationInputTypeDef,  # (1)
    transformationConfiguration: TransformationConfigurationTypeDef,  # (2)
```

1. See [:material-code-braces: QueryGenerationInputTypeDef](./type_defs.md#querygenerationinputtypedef) 
2. See [:material-code-braces: TransformationConfigurationTypeDef](./type_defs.md#transformationconfigurationtypedef) 
## InvocationInputMemberTypeDef

```python
# InvocationInputMemberTypeDef definition

class InvocationInputMemberTypeDef(TypedDict):
    apiInvocationInput: NotRequired[ApiInvocationInputTypeDef],  # (1)
    functionInvocationInput: NotRequired[FunctionInvocationInputTypeDef],  # (2)
```

1. See [:material-code-braces: ApiInvocationInputTypeDef](./type_defs.md#apiinvocationinputtypedef) 
2. See [:material-code-braces: FunctionInvocationInputTypeDef](./type_defs.md#functioninvocationinputtypedef) 
## AgentCollaboratorInputPayloadTypeDef

```python
# AgentCollaboratorInputPayloadTypeDef definition

class AgentCollaboratorInputPayloadTypeDef(TypedDict):
    returnControlResults: NotRequired[ReturnControlResultsTypeDef],  # (1)
    text: NotRequired[str],
    type: NotRequired[PayloadTypeType],  # (2)
```

1. See [:material-code-braces: ReturnControlResultsTypeDef](./type_defs.md#returncontrolresultstypedef) 
2. See [:material-code-brackets: PayloadTypeType](./literals.md#payloadtypetype) 
## VectorSearchRerankingConfigurationTypeDef

```python
# VectorSearchRerankingConfigurationTypeDef definition

class VectorSearchRerankingConfigurationTypeDef(TypedDict):
    type: VectorSearchRerankingConfigurationTypeType,  # (2)
    bedrockRerankingConfiguration: NotRequired[VectorSearchBedrockRerankingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: VectorSearchBedrockRerankingConfigurationTypeDef](./type_defs.md#vectorsearchbedrockrerankingconfigurationtypedef) 
2. See [:material-code-brackets: VectorSearchRerankingConfigurationTypeType](./literals.md#vectorsearchrerankingconfigurationtypetype) 
## FlowTraceEventTypeDef

```python
# FlowTraceEventTypeDef definition

class FlowTraceEventTypeDef(TypedDict):
    trace: FlowTraceTypeDef,  # (1)
```

1. See [:material-code-braces: FlowTraceTypeDef](./type_defs.md#flowtracetypedef) 
## OptimizePromptResponseTypeDef

```python
# OptimizePromptResponseTypeDef definition

class OptimizePromptResponseTypeDef(TypedDict):
    optimizedPrompt: AioEventStream[OptimizedPromptStreamTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OptimizedPromptStreamTypeDef](./type_defs.md#optimizedpromptstreamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RerankRequestRequestTypeDef

```python
# RerankRequestRequestTypeDef definition

class RerankRequestRequestTypeDef(TypedDict):
    queries: Sequence[RerankQueryTypeDef],  # (1)
    rerankingConfiguration: RerankingConfigurationTypeDef,  # (2)
    sources: Sequence[RerankSourceTypeDef],  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RerankQueryTypeDef](./type_defs.md#rerankquerytypedef) 
2. See [:material-code-braces: RerankingConfigurationTypeDef](./type_defs.md#rerankingconfigurationtypedef) 
3. See [:material-code-braces: RerankSourceTypeDef](./type_defs.md#reranksourcetypedef) 
## RerankRequestRerankPaginateTypeDef

```python
# RerankRequestRerankPaginateTypeDef definition

class RerankRequestRerankPaginateTypeDef(TypedDict):
    queries: Sequence[RerankQueryTypeDef],  # (1)
    rerankingConfiguration: RerankingConfigurationTypeDef,  # (2)
    sources: Sequence[RerankSourceTypeDef],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: RerankQueryTypeDef](./type_defs.md#rerankquerytypedef) 
2. See [:material-code-braces: RerankingConfigurationTypeDef](./type_defs.md#rerankingconfigurationtypedef) 
3. See [:material-code-braces: RerankSourceTypeDef](./type_defs.md#reranksourcetypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## AttributionTypeDef

```python
# AttributionTypeDef definition

class AttributionTypeDef(TypedDict):
    citations: NotRequired[List[CitationTypeDef]],  # (1)
```

1. See [:material-code-braces: CitationTypeDef](./type_defs.md#citationtypedef) 
## CitationEventTypeDef

```python
# CitationEventTypeDef definition

class CitationEventTypeDef(TypedDict):
    citation: NotRequired[CitationTypeDef],  # (1)
```

1. See [:material-code-braces: CitationTypeDef](./type_defs.md#citationtypedef) 
## RetrieveAndGenerateResponseTypeDef

```python
# RetrieveAndGenerateResponseTypeDef definition

class RetrieveAndGenerateResponseTypeDef(TypedDict):
    citations: List[CitationTypeDef],  # (1)
    guardrailAction: GuadrailActionType,  # (2)
    output: RetrieveAndGenerateOutputTypeDef,  # (3)
    sessionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: CitationTypeDef](./type_defs.md#citationtypedef) 
2. See [:material-code-brackets: GuadrailActionType](./literals.md#guadrailactiontype) 
3. See [:material-code-braces: RetrieveAndGenerateOutputTypeDef](./type_defs.md#retrieveandgenerateoutputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InlineAgentReturnControlPayloadTypeDef

```python
# InlineAgentReturnControlPayloadTypeDef definition

class InlineAgentReturnControlPayloadTypeDef(TypedDict):
    invocationId: NotRequired[str],
    invocationInputs: NotRequired[List[InvocationInputMemberTypeDef]],  # (1)
```

1. See [:material-code-braces: InvocationInputMemberTypeDef](./type_defs.md#invocationinputmembertypedef) 
## ReturnControlPayloadTypeDef

```python
# ReturnControlPayloadTypeDef definition

class ReturnControlPayloadTypeDef(TypedDict):
    invocationId: NotRequired[str],
    invocationInputs: NotRequired[List[InvocationInputMemberTypeDef]],  # (1)
```

1. See [:material-code-braces: InvocationInputMemberTypeDef](./type_defs.md#invocationinputmembertypedef) 
## AgentCollaboratorInvocationInputTypeDef

```python
# AgentCollaboratorInvocationInputTypeDef definition

class AgentCollaboratorInvocationInputTypeDef(TypedDict):
    agentCollaboratorAliasArn: NotRequired[str],
    agentCollaboratorName: NotRequired[str],
    input: NotRequired[AgentCollaboratorInputPayloadTypeDef],  # (1)
```

1. See [:material-code-braces: AgentCollaboratorInputPayloadTypeDef](./type_defs.md#agentcollaboratorinputpayloadtypedef) 
## InlineSessionStateTypeDef

```python
# InlineSessionStateTypeDef definition

class InlineSessionStateTypeDef(TypedDict):
    files: NotRequired[Sequence[InputFileTypeDef]],  # (1)
    invocationId: NotRequired[str],
    promptSessionAttributes: NotRequired[Mapping[str, str]],
    returnControlInvocationResults: NotRequired[Sequence[InvocationResultMemberUnionTypeDef]],  # (2)
    sessionAttributes: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: InputFileTypeDef](./type_defs.md#inputfiletypedef) 
2. See [:material-code-braces: InvocationResultMemberTypeDef](./type_defs.md#invocationresultmembertypedef) [:material-code-braces: InvocationResultMemberOutputTypeDef](./type_defs.md#invocationresultmemberoutputtypedef) 
## KnowledgeBaseVectorSearchConfigurationPaginatorTypeDef

```python
# KnowledgeBaseVectorSearchConfigurationPaginatorTypeDef definition

class KnowledgeBaseVectorSearchConfigurationPaginatorTypeDef(TypedDict):
    filter: NotRequired[RetrievalFilterPaginatorTypeDef],  # (1)
    implicitFilterConfiguration: NotRequired[ImplicitFilterConfigurationTypeDef],  # (2)
    numberOfResults: NotRequired[int],
    overrideSearchType: NotRequired[SearchTypeType],  # (3)
    rerankingConfiguration: NotRequired[VectorSearchRerankingConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: RetrievalFilterPaginatorTypeDef](./type_defs.md#retrievalfilterpaginatortypedef) 
2. See [:material-code-braces: ImplicitFilterConfigurationTypeDef](./type_defs.md#implicitfilterconfigurationtypedef) 
3. See [:material-code-brackets: SearchTypeType](./literals.md#searchtypetype) 
4. See [:material-code-braces: VectorSearchRerankingConfigurationTypeDef](./type_defs.md#vectorsearchrerankingconfigurationtypedef) 
## KnowledgeBaseVectorSearchConfigurationTypeDef

```python
# KnowledgeBaseVectorSearchConfigurationTypeDef definition

class KnowledgeBaseVectorSearchConfigurationTypeDef(TypedDict):
    filter: NotRequired[RetrievalFilterTypeDef],  # (1)
    implicitFilterConfiguration: NotRequired[ImplicitFilterConfigurationTypeDef],  # (2)
    numberOfResults: NotRequired[int],
    overrideSearchType: NotRequired[SearchTypeType],  # (3)
    rerankingConfiguration: NotRequired[VectorSearchRerankingConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: RetrievalFilterTypeDef](./type_defs.md#retrievalfiltertypedef) 
2. See [:material-code-braces: ImplicitFilterConfigurationTypeDef](./type_defs.md#implicitfilterconfigurationtypedef) 
3. See [:material-code-brackets: SearchTypeType](./literals.md#searchtypetype) 
4. See [:material-code-braces: VectorSearchRerankingConfigurationTypeDef](./type_defs.md#vectorsearchrerankingconfigurationtypedef) 
## FlowResponseStreamTypeDef

```python
# FlowResponseStreamTypeDef definition

class FlowResponseStreamTypeDef(TypedDict):
    accessDeniedException: NotRequired[AccessDeniedExceptionTypeDef],  # (1)
    badGatewayException: NotRequired[BadGatewayExceptionTypeDef],  # (2)
    conflictException: NotRequired[ConflictExceptionTypeDef],  # (3)
    dependencyFailedException: NotRequired[DependencyFailedExceptionTypeDef],  # (4)
    flowCompletionEvent: NotRequired[FlowCompletionEventTypeDef],  # (5)
    flowOutputEvent: NotRequired[FlowOutputEventTypeDef],  # (6)
    flowTraceEvent: NotRequired[FlowTraceEventTypeDef],  # (7)
    internalServerException: NotRequired[InternalServerExceptionTypeDef],  # (8)
    resourceNotFoundException: NotRequired[ResourceNotFoundExceptionTypeDef],  # (9)
    serviceQuotaExceededException: NotRequired[ServiceQuotaExceededExceptionTypeDef],  # (10)
    throttlingException: NotRequired[ThrottlingExceptionTypeDef],  # (11)
    validationException: NotRequired[ValidationExceptionTypeDef],  # (12)
```

1. See [:material-code-braces: AccessDeniedExceptionTypeDef](./type_defs.md#accessdeniedexceptiontypedef) 
2. See [:material-code-braces: BadGatewayExceptionTypeDef](./type_defs.md#badgatewayexceptiontypedef) 
3. See [:material-code-braces: ConflictExceptionTypeDef](./type_defs.md#conflictexceptiontypedef) 
4. See [:material-code-braces: DependencyFailedExceptionTypeDef](./type_defs.md#dependencyfailedexceptiontypedef) 
5. See [:material-code-braces: FlowCompletionEventTypeDef](./type_defs.md#flowcompletioneventtypedef) 
6. See [:material-code-braces: FlowOutputEventTypeDef](./type_defs.md#flowoutputeventtypedef) 
7. See [:material-code-braces: FlowTraceEventTypeDef](./type_defs.md#flowtraceeventtypedef) 
8. See [:material-code-braces: InternalServerExceptionTypeDef](./type_defs.md#internalserverexceptiontypedef) 
9. See [:material-code-braces: ResourceNotFoundExceptionTypeDef](./type_defs.md#resourcenotfoundexceptiontypedef) 
10. See [:material-code-braces: ServiceQuotaExceededExceptionTypeDef](./type_defs.md#servicequotaexceededexceptiontypedef) 
11. See [:material-code-braces: ThrottlingExceptionTypeDef](./type_defs.md#throttlingexceptiontypedef) 
12. See [:material-code-braces: ValidationExceptionTypeDef](./type_defs.md#validationexceptiontypedef) 
## InlineAgentPayloadPartTypeDef

```python
# InlineAgentPayloadPartTypeDef definition

class InlineAgentPayloadPartTypeDef(TypedDict):
    attribution: NotRequired[AttributionTypeDef],  # (1)
    bytes: NotRequired[bytes],
```

1. See [:material-code-braces: AttributionTypeDef](./type_defs.md#attributiontypedef) 
## PayloadPartTypeDef

```python
# PayloadPartTypeDef definition

class PayloadPartTypeDef(TypedDict):
    attribution: NotRequired[AttributionTypeDef],  # (1)
    bytes: NotRequired[bytes],
```

1. See [:material-code-braces: AttributionTypeDef](./type_defs.md#attributiontypedef) 
## RetrieveAndGenerateStreamResponseOutputTypeDef

```python
# RetrieveAndGenerateStreamResponseOutputTypeDef definition

class RetrieveAndGenerateStreamResponseOutputTypeDef(TypedDict):
    accessDeniedException: NotRequired[AccessDeniedExceptionTypeDef],  # (1)
    badGatewayException: NotRequired[BadGatewayExceptionTypeDef],  # (2)
    citation: NotRequired[CitationEventTypeDef],  # (3)
    conflictException: NotRequired[ConflictExceptionTypeDef],  # (4)
    dependencyFailedException: NotRequired[DependencyFailedExceptionTypeDef],  # (5)
    guardrail: NotRequired[GuardrailEventTypeDef],  # (6)
    internalServerException: NotRequired[InternalServerExceptionTypeDef],  # (7)
    output: NotRequired[RetrieveAndGenerateOutputEventTypeDef],  # (8)
    resourceNotFoundException: NotRequired[ResourceNotFoundExceptionTypeDef],  # (9)
    serviceQuotaExceededException: NotRequired[ServiceQuotaExceededExceptionTypeDef],  # (10)
    throttlingException: NotRequired[ThrottlingExceptionTypeDef],  # (11)
    validationException: NotRequired[ValidationExceptionTypeDef],  # (12)
```

1. See [:material-code-braces: AccessDeniedExceptionTypeDef](./type_defs.md#accessdeniedexceptiontypedef) 
2. See [:material-code-braces: BadGatewayExceptionTypeDef](./type_defs.md#badgatewayexceptiontypedef) 
3. See [:material-code-braces: CitationEventTypeDef](./type_defs.md#citationeventtypedef) 
4. See [:material-code-braces: ConflictExceptionTypeDef](./type_defs.md#conflictexceptiontypedef) 
5. See [:material-code-braces: DependencyFailedExceptionTypeDef](./type_defs.md#dependencyfailedexceptiontypedef) 
6. See [:material-code-braces: GuardrailEventTypeDef](./type_defs.md#guardraileventtypedef) 
7. See [:material-code-braces: InternalServerExceptionTypeDef](./type_defs.md#internalserverexceptiontypedef) 
8. See [:material-code-braces: RetrieveAndGenerateOutputEventTypeDef](./type_defs.md#retrieveandgenerateoutputeventtypedef) 
9. See [:material-code-braces: ResourceNotFoundExceptionTypeDef](./type_defs.md#resourcenotfoundexceptiontypedef) 
10. See [:material-code-braces: ServiceQuotaExceededExceptionTypeDef](./type_defs.md#servicequotaexceededexceptiontypedef) 
11. See [:material-code-braces: ThrottlingExceptionTypeDef](./type_defs.md#throttlingexceptiontypedef) 
12. See [:material-code-braces: ValidationExceptionTypeDef](./type_defs.md#validationexceptiontypedef) 
## AgentCollaboratorOutputPayloadTypeDef

```python
# AgentCollaboratorOutputPayloadTypeDef definition

class AgentCollaboratorOutputPayloadTypeDef(TypedDict):
    returnControlPayload: NotRequired[ReturnControlPayloadTypeDef],  # (1)
    text: NotRequired[str],
    type: NotRequired[PayloadTypeType],  # (2)
```

1. See [:material-code-braces: ReturnControlPayloadTypeDef](./type_defs.md#returncontrolpayloadtypedef) 
2. See [:material-code-brackets: PayloadTypeType](./literals.md#payloadtypetype) 
## InvocationInputTypeDef

```python
# InvocationInputTypeDef definition

class InvocationInputTypeDef(TypedDict):
    actionGroupInvocationInput: NotRequired[ActionGroupInvocationInputTypeDef],  # (1)
    agentCollaboratorInvocationInput: NotRequired[AgentCollaboratorInvocationInputTypeDef],  # (2)
    codeInterpreterInvocationInput: NotRequired[CodeInterpreterInvocationInputTypeDef],  # (3)
    invocationType: NotRequired[InvocationTypeType],  # (4)
    knowledgeBaseLookupInput: NotRequired[KnowledgeBaseLookupInputTypeDef],  # (5)
    traceId: NotRequired[str],
```

1. See [:material-code-braces: ActionGroupInvocationInputTypeDef](./type_defs.md#actiongroupinvocationinputtypedef) 
2. See [:material-code-braces: AgentCollaboratorInvocationInputTypeDef](./type_defs.md#agentcollaboratorinvocationinputtypedef) 
3. See [:material-code-braces: CodeInterpreterInvocationInputTypeDef](./type_defs.md#codeinterpreterinvocationinputtypedef) 
4. See [:material-code-brackets: InvocationTypeType](./literals.md#invocationtypetype) 
5. See [:material-code-braces: KnowledgeBaseLookupInputTypeDef](./type_defs.md#knowledgebaselookupinputtypedef) 
## KnowledgeBaseRetrievalConfigurationPaginatorTypeDef

```python
# KnowledgeBaseRetrievalConfigurationPaginatorTypeDef definition

class KnowledgeBaseRetrievalConfigurationPaginatorTypeDef(TypedDict):
    vectorSearchConfiguration: KnowledgeBaseVectorSearchConfigurationPaginatorTypeDef,  # (1)
```

1. See [:material-code-braces: KnowledgeBaseVectorSearchConfigurationPaginatorTypeDef](./type_defs.md#knowledgebasevectorsearchconfigurationpaginatortypedef) 
## KnowledgeBaseRetrievalConfigurationTypeDef

```python
# KnowledgeBaseRetrievalConfigurationTypeDef definition

class KnowledgeBaseRetrievalConfigurationTypeDef(TypedDict):
    vectorSearchConfiguration: KnowledgeBaseVectorSearchConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: KnowledgeBaseVectorSearchConfigurationTypeDef](./type_defs.md#knowledgebasevectorsearchconfigurationtypedef) 
## InvokeFlowResponseTypeDef

```python
# InvokeFlowResponseTypeDef definition

class InvokeFlowResponseTypeDef(TypedDict):
    responseStream: AioEventStream[FlowResponseStreamTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlowResponseStreamTypeDef](./type_defs.md#flowresponsestreamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RetrieveAndGenerateStreamResponseTypeDef

```python
# RetrieveAndGenerateStreamResponseTypeDef definition

class RetrieveAndGenerateStreamResponseTypeDef(TypedDict):
    sessionId: str,
    stream: AioEventStream[RetrieveAndGenerateStreamResponseOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RetrieveAndGenerateStreamResponseOutputTypeDef](./type_defs.md#retrieveandgeneratestreamresponseoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AgentCollaboratorInvocationOutputTypeDef

```python
# AgentCollaboratorInvocationOutputTypeDef definition

class AgentCollaboratorInvocationOutputTypeDef(TypedDict):
    agentCollaboratorAliasArn: NotRequired[str],
    agentCollaboratorName: NotRequired[str],
    output: NotRequired[AgentCollaboratorOutputPayloadTypeDef],  # (1)
```

1. See [:material-code-braces: AgentCollaboratorOutputPayloadTypeDef](./type_defs.md#agentcollaboratoroutputpayloadtypedef) 
## RetrieveRequestRetrievePaginateTypeDef

```python
# RetrieveRequestRetrievePaginateTypeDef definition

class RetrieveRequestRetrievePaginateTypeDef(TypedDict):
    knowledgeBaseId: str,
    retrievalQuery: KnowledgeBaseQueryTypeDef,  # (1)
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (2)
    retrievalConfiguration: NotRequired[KnowledgeBaseRetrievalConfigurationPaginatorTypeDef],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: KnowledgeBaseQueryTypeDef](./type_defs.md#knowledgebasequerytypedef) 
2. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
3. See [:material-code-braces: KnowledgeBaseRetrievalConfigurationPaginatorTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationpaginatortypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## KnowledgeBaseConfigurationTypeDef

```python
# KnowledgeBaseConfigurationTypeDef definition

class KnowledgeBaseConfigurationTypeDef(TypedDict):
    knowledgeBaseId: str,
    retrievalConfiguration: KnowledgeBaseRetrievalConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: KnowledgeBaseRetrievalConfigurationTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationtypedef) 
## KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef

```python
# KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef definition

class KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef(TypedDict):
    knowledgeBaseId: str,
    modelArn: str,
    generationConfiguration: NotRequired[GenerationConfigurationTypeDef],  # (1)
    orchestrationConfiguration: NotRequired[OrchestrationConfigurationTypeDef],  # (2)
    retrievalConfiguration: NotRequired[KnowledgeBaseRetrievalConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: GenerationConfigurationTypeDef](./type_defs.md#generationconfigurationtypedef) 
2. See [:material-code-braces: OrchestrationConfigurationTypeDef](./type_defs.md#orchestrationconfigurationtypedef) 
3. See [:material-code-braces: KnowledgeBaseRetrievalConfigurationTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationtypedef) 
## KnowledgeBaseTypeDef

```python
# KnowledgeBaseTypeDef definition

class KnowledgeBaseTypeDef(TypedDict):
    description: str,
    knowledgeBaseId: str,
    retrievalConfiguration: NotRequired[KnowledgeBaseRetrievalConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: KnowledgeBaseRetrievalConfigurationTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationtypedef) 
## RetrieveRequestRequestTypeDef

```python
# RetrieveRequestRequestTypeDef definition

class RetrieveRequestRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    retrievalQuery: KnowledgeBaseQueryTypeDef,  # (1)
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (2)
    nextToken: NotRequired[str],
    retrievalConfiguration: NotRequired[KnowledgeBaseRetrievalConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: KnowledgeBaseQueryTypeDef](./type_defs.md#knowledgebasequerytypedef) 
2. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
3. See [:material-code-braces: KnowledgeBaseRetrievalConfigurationTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationtypedef) 
## ObservationTypeDef

```python
# ObservationTypeDef definition

class ObservationTypeDef(TypedDict):
    actionGroupInvocationOutput: NotRequired[ActionGroupInvocationOutputTypeDef],  # (1)
    agentCollaboratorInvocationOutput: NotRequired[AgentCollaboratorInvocationOutputTypeDef],  # (2)
    codeInterpreterInvocationOutput: NotRequired[CodeInterpreterInvocationOutputTypeDef],  # (3)
    finalResponse: NotRequired[FinalResponseTypeDef],  # (4)
    knowledgeBaseLookupOutput: NotRequired[KnowledgeBaseLookupOutputTypeDef],  # (5)
    repromptResponse: NotRequired[RepromptResponseTypeDef],  # (6)
    traceId: NotRequired[str],
    type: NotRequired[TypeType],  # (7)
```

1. See [:material-code-braces: ActionGroupInvocationOutputTypeDef](./type_defs.md#actiongroupinvocationoutputtypedef) 
2. See [:material-code-braces: AgentCollaboratorInvocationOutputTypeDef](./type_defs.md#agentcollaboratorinvocationoutputtypedef) 
3. See [:material-code-braces: CodeInterpreterInvocationOutputTypeDef](./type_defs.md#codeinterpreterinvocationoutputtypedef) 
4. See [:material-code-braces: FinalResponseTypeDef](./type_defs.md#finalresponsetypedef) 
5. See [:material-code-braces: KnowledgeBaseLookupOutputTypeDef](./type_defs.md#knowledgebaselookupoutputtypedef) 
6. See [:material-code-braces: RepromptResponseTypeDef](./type_defs.md#repromptresponsetypedef) 
7. See [:material-code-brackets: TypeType](./literals.md#typetype) 
## SessionStateTypeDef

```python
# SessionStateTypeDef definition

class SessionStateTypeDef(TypedDict):
    conversationHistory: NotRequired[ConversationHistoryTypeDef],  # (1)
    files: NotRequired[Sequence[InputFileTypeDef]],  # (2)
    invocationId: NotRequired[str],
    knowledgeBaseConfigurations: NotRequired[Sequence[KnowledgeBaseConfigurationTypeDef]],  # (3)
    promptSessionAttributes: NotRequired[Mapping[str, str]],
    returnControlInvocationResults: NotRequired[Sequence[InvocationResultMemberUnionTypeDef]],  # (4)
    sessionAttributes: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ConversationHistoryTypeDef](./type_defs.md#conversationhistorytypedef) 
2. See [:material-code-braces: InputFileTypeDef](./type_defs.md#inputfiletypedef) 
3. See [:material-code-braces: KnowledgeBaseConfigurationTypeDef](./type_defs.md#knowledgebaseconfigurationtypedef) 
4. See [:material-code-braces: InvocationResultMemberTypeDef](./type_defs.md#invocationresultmembertypedef) [:material-code-braces: InvocationResultMemberOutputTypeDef](./type_defs.md#invocationresultmemberoutputtypedef) 
## RetrieveAndGenerateConfigurationTypeDef

```python
# RetrieveAndGenerateConfigurationTypeDef definition

class RetrieveAndGenerateConfigurationTypeDef(TypedDict):
    type: RetrieveAndGenerateTypeType,  # (3)
    externalSourcesConfiguration: NotRequired[ExternalSourcesRetrieveAndGenerateConfigurationTypeDef],  # (1)
    knowledgeBaseConfiguration: NotRequired[KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ExternalSourcesRetrieveAndGenerateConfigurationTypeDef](./type_defs.md#externalsourcesretrieveandgenerateconfigurationtypedef) 
2. See [:material-code-braces: KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef](./type_defs.md#knowledgebaseretrieveandgenerateconfigurationtypedef) 
3. See [:material-code-brackets: RetrieveAndGenerateTypeType](./literals.md#retrieveandgeneratetypetype) 
## InvokeInlineAgentRequestRequestTypeDef

```python
# InvokeInlineAgentRequestRequestTypeDef definition

class InvokeInlineAgentRequestRequestTypeDef(TypedDict):
    foundationModel: str,
    instruction: str,
    sessionId: str,
    actionGroups: NotRequired[Sequence[AgentActionGroupTypeDef]],  # (1)
    customerEncryptionKeyArn: NotRequired[str],
    enableTrace: NotRequired[bool],
    endSession: NotRequired[bool],
    guardrailConfiguration: NotRequired[GuardrailConfigurationWithArnTypeDef],  # (2)
    idleSessionTTLInSeconds: NotRequired[int],
    inlineSessionState: NotRequired[InlineSessionStateTypeDef],  # (3)
    inputText: NotRequired[str],
    knowledgeBases: NotRequired[Sequence[KnowledgeBaseTypeDef]],  # (4)
    promptOverrideConfiguration: NotRequired[PromptOverrideConfigurationTypeDef],  # (5)
```

1. See [:material-code-braces: AgentActionGroupTypeDef](./type_defs.md#agentactiongrouptypedef) 
2. See [:material-code-braces: GuardrailConfigurationWithArnTypeDef](./type_defs.md#guardrailconfigurationwitharntypedef) 
3. See [:material-code-braces: InlineSessionStateTypeDef](./type_defs.md#inlinesessionstatetypedef) 
4. See [:material-code-braces: KnowledgeBaseTypeDef](./type_defs.md#knowledgebasetypedef) 
5. See [:material-code-braces: PromptOverrideConfigurationTypeDef](./type_defs.md#promptoverrideconfigurationtypedef) 
## OrchestrationTraceTypeDef

```python
# OrchestrationTraceTypeDef definition

class OrchestrationTraceTypeDef(TypedDict):
    invocationInput: NotRequired[InvocationInputTypeDef],  # (1)
    modelInvocationInput: NotRequired[ModelInvocationInputTypeDef],  # (2)
    modelInvocationOutput: NotRequired[OrchestrationModelInvocationOutputTypeDef],  # (3)
    observation: NotRequired[ObservationTypeDef],  # (4)
    rationale: NotRequired[RationaleTypeDef],  # (5)
```

1. See [:material-code-braces: InvocationInputTypeDef](./type_defs.md#invocationinputtypedef) 
2. See [:material-code-braces: ModelInvocationInputTypeDef](./type_defs.md#modelinvocationinputtypedef) 
3. See [:material-code-braces: OrchestrationModelInvocationOutputTypeDef](./type_defs.md#orchestrationmodelinvocationoutputtypedef) 
4. See [:material-code-braces: ObservationTypeDef](./type_defs.md#observationtypedef) 
5. See [:material-code-braces: RationaleTypeDef](./type_defs.md#rationaletypedef) 
## RoutingClassifierTraceTypeDef

```python
# RoutingClassifierTraceTypeDef definition

class RoutingClassifierTraceTypeDef(TypedDict):
    invocationInput: NotRequired[InvocationInputTypeDef],  # (1)
    modelInvocationInput: NotRequired[ModelInvocationInputTypeDef],  # (2)
    modelInvocationOutput: NotRequired[RoutingClassifierModelInvocationOutputTypeDef],  # (3)
    observation: NotRequired[ObservationTypeDef],  # (4)
```

1. See [:material-code-braces: InvocationInputTypeDef](./type_defs.md#invocationinputtypedef) 
2. See [:material-code-braces: ModelInvocationInputTypeDef](./type_defs.md#modelinvocationinputtypedef) 
3. See [:material-code-braces: RoutingClassifierModelInvocationOutputTypeDef](./type_defs.md#routingclassifiermodelinvocationoutputtypedef) 
4. See [:material-code-braces: ObservationTypeDef](./type_defs.md#observationtypedef) 
## InvokeAgentRequestRequestTypeDef

```python
# InvokeAgentRequestRequestTypeDef definition

class InvokeAgentRequestRequestTypeDef(TypedDict):
    agentAliasId: str,
    agentId: str,
    sessionId: str,
    enableTrace: NotRequired[bool],
    endSession: NotRequired[bool],
    inputText: NotRequired[str],
    memoryId: NotRequired[str],
    sessionState: NotRequired[SessionStateTypeDef],  # (1)
    sourceArn: NotRequired[str],
    streamingConfigurations: NotRequired[StreamingConfigurationsTypeDef],  # (2)
```

1. See [:material-code-braces: SessionStateTypeDef](./type_defs.md#sessionstatetypedef) 
2. See [:material-code-braces: StreamingConfigurationsTypeDef](./type_defs.md#streamingconfigurationstypedef) 
## RetrieveAndGenerateRequestRequestTypeDef

```python
# RetrieveAndGenerateRequestRequestTypeDef definition

class RetrieveAndGenerateRequestRequestTypeDef(TypedDict):
    input: RetrieveAndGenerateInputTypeDef,  # (1)
    retrieveAndGenerateConfiguration: NotRequired[RetrieveAndGenerateConfigurationTypeDef],  # (2)
    sessionConfiguration: NotRequired[RetrieveAndGenerateSessionConfigurationTypeDef],  # (3)
    sessionId: NotRequired[str],
```

1. See [:material-code-braces: RetrieveAndGenerateInputTypeDef](./type_defs.md#retrieveandgenerateinputtypedef) 
2. See [:material-code-braces: RetrieveAndGenerateConfigurationTypeDef](./type_defs.md#retrieveandgenerateconfigurationtypedef) 
3. See [:material-code-braces: RetrieveAndGenerateSessionConfigurationTypeDef](./type_defs.md#retrieveandgeneratesessionconfigurationtypedef) 
## RetrieveAndGenerateStreamRequestRequestTypeDef

```python
# RetrieveAndGenerateStreamRequestRequestTypeDef definition

class RetrieveAndGenerateStreamRequestRequestTypeDef(TypedDict):
    input: RetrieveAndGenerateInputTypeDef,  # (1)
    retrieveAndGenerateConfiguration: NotRequired[RetrieveAndGenerateConfigurationTypeDef],  # (2)
    sessionConfiguration: NotRequired[RetrieveAndGenerateSessionConfigurationTypeDef],  # (3)
    sessionId: NotRequired[str],
```

1. See [:material-code-braces: RetrieveAndGenerateInputTypeDef](./type_defs.md#retrieveandgenerateinputtypedef) 
2. See [:material-code-braces: RetrieveAndGenerateConfigurationTypeDef](./type_defs.md#retrieveandgenerateconfigurationtypedef) 
3. See [:material-code-braces: RetrieveAndGenerateSessionConfigurationTypeDef](./type_defs.md#retrieveandgeneratesessionconfigurationtypedef) 
## TraceTypeDef

```python
# TraceTypeDef definition

class TraceTypeDef(TypedDict):
    customOrchestrationTrace: NotRequired[CustomOrchestrationTraceTypeDef],  # (1)
    failureTrace: NotRequired[FailureTraceTypeDef],  # (2)
    guardrailTrace: NotRequired[GuardrailTraceTypeDef],  # (3)
    orchestrationTrace: NotRequired[OrchestrationTraceTypeDef],  # (4)
    postProcessingTrace: NotRequired[PostProcessingTraceTypeDef],  # (5)
    preProcessingTrace: NotRequired[PreProcessingTraceTypeDef],  # (6)
    routingClassifierTrace: NotRequired[RoutingClassifierTraceTypeDef],  # (7)
```

1. See [:material-code-braces: CustomOrchestrationTraceTypeDef](./type_defs.md#customorchestrationtracetypedef) 
2. See [:material-code-braces: FailureTraceTypeDef](./type_defs.md#failuretracetypedef) 
3. See [:material-code-braces: GuardrailTraceTypeDef](./type_defs.md#guardrailtracetypedef) 
4. See [:material-code-braces: OrchestrationTraceTypeDef](./type_defs.md#orchestrationtracetypedef) 
5. See [:material-code-braces: PostProcessingTraceTypeDef](./type_defs.md#postprocessingtracetypedef) 
6. See [:material-code-braces: PreProcessingTraceTypeDef](./type_defs.md#preprocessingtracetypedef) 
7. See [:material-code-braces: RoutingClassifierTraceTypeDef](./type_defs.md#routingclassifiertracetypedef) 
## InlineAgentTracePartTypeDef

```python
# InlineAgentTracePartTypeDef definition

class InlineAgentTracePartTypeDef(TypedDict):
    sessionId: NotRequired[str],
    trace: NotRequired[TraceTypeDef],  # (1)
```

1. See [:material-code-braces: TraceTypeDef](./type_defs.md#tracetypedef) 
## TracePartTypeDef

```python
# TracePartTypeDef definition

class TracePartTypeDef(TypedDict):
    agentAliasId: NotRequired[str],
    agentId: NotRequired[str],
    agentVersion: NotRequired[str],
    callerChain: NotRequired[List[CallerTypeDef]],  # (1)
    collaboratorName: NotRequired[str],
    sessionId: NotRequired[str],
    trace: NotRequired[TraceTypeDef],  # (2)
```

1. See [:material-code-braces: CallerTypeDef](./type_defs.md#callertypedef) 
2. See [:material-code-braces: TraceTypeDef](./type_defs.md#tracetypedef) 
## InlineAgentResponseStreamTypeDef

```python
# InlineAgentResponseStreamTypeDef definition

class InlineAgentResponseStreamTypeDef(TypedDict):
    accessDeniedException: NotRequired[AccessDeniedExceptionTypeDef],  # (1)
    badGatewayException: NotRequired[BadGatewayExceptionTypeDef],  # (2)
    chunk: NotRequired[InlineAgentPayloadPartTypeDef],  # (3)
    conflictException: NotRequired[ConflictExceptionTypeDef],  # (4)
    dependencyFailedException: NotRequired[DependencyFailedExceptionTypeDef],  # (5)
    files: NotRequired[InlineAgentFilePartTypeDef],  # (6)
    internalServerException: NotRequired[InternalServerExceptionTypeDef],  # (7)
    resourceNotFoundException: NotRequired[ResourceNotFoundExceptionTypeDef],  # (8)
    returnControl: NotRequired[InlineAgentReturnControlPayloadTypeDef],  # (9)
    serviceQuotaExceededException: NotRequired[ServiceQuotaExceededExceptionTypeDef],  # (10)
    throttlingException: NotRequired[ThrottlingExceptionTypeDef],  # (11)
    trace: NotRequired[InlineAgentTracePartTypeDef],  # (12)
    validationException: NotRequired[ValidationExceptionTypeDef],  # (13)
```

1. See [:material-code-braces: AccessDeniedExceptionTypeDef](./type_defs.md#accessdeniedexceptiontypedef) 
2. See [:material-code-braces: BadGatewayExceptionTypeDef](./type_defs.md#badgatewayexceptiontypedef) 
3. See [:material-code-braces: InlineAgentPayloadPartTypeDef](./type_defs.md#inlineagentpayloadparttypedef) 
4. See [:material-code-braces: ConflictExceptionTypeDef](./type_defs.md#conflictexceptiontypedef) 
5. See [:material-code-braces: DependencyFailedExceptionTypeDef](./type_defs.md#dependencyfailedexceptiontypedef) 
6. See [:material-code-braces: InlineAgentFilePartTypeDef](./type_defs.md#inlineagentfileparttypedef) 
7. See [:material-code-braces: InternalServerExceptionTypeDef](./type_defs.md#internalserverexceptiontypedef) 
8. See [:material-code-braces: ResourceNotFoundExceptionTypeDef](./type_defs.md#resourcenotfoundexceptiontypedef) 
9. See [:material-code-braces: InlineAgentReturnControlPayloadTypeDef](./type_defs.md#inlineagentreturncontrolpayloadtypedef) 
10. See [:material-code-braces: ServiceQuotaExceededExceptionTypeDef](./type_defs.md#servicequotaexceededexceptiontypedef) 
11. See [:material-code-braces: ThrottlingExceptionTypeDef](./type_defs.md#throttlingexceptiontypedef) 
12. See [:material-code-braces: InlineAgentTracePartTypeDef](./type_defs.md#inlineagenttraceparttypedef) 
13. See [:material-code-braces: ValidationExceptionTypeDef](./type_defs.md#validationexceptiontypedef) 
## ResponseStreamTypeDef

```python
# ResponseStreamTypeDef definition

class ResponseStreamTypeDef(TypedDict):
    accessDeniedException: NotRequired[AccessDeniedExceptionTypeDef],  # (1)
    badGatewayException: NotRequired[BadGatewayExceptionTypeDef],  # (2)
    chunk: NotRequired[PayloadPartTypeDef],  # (3)
    conflictException: NotRequired[ConflictExceptionTypeDef],  # (4)
    dependencyFailedException: NotRequired[DependencyFailedExceptionTypeDef],  # (5)
    files: NotRequired[FilePartTypeDef],  # (6)
    internalServerException: NotRequired[InternalServerExceptionTypeDef],  # (7)
    resourceNotFoundException: NotRequired[ResourceNotFoundExceptionTypeDef],  # (8)
    returnControl: NotRequired[ReturnControlPayloadTypeDef],  # (9)
    serviceQuotaExceededException: NotRequired[ServiceQuotaExceededExceptionTypeDef],  # (10)
    throttlingException: NotRequired[ThrottlingExceptionTypeDef],  # (11)
    trace: NotRequired[TracePartTypeDef],  # (12)
    validationException: NotRequired[ValidationExceptionTypeDef],  # (13)
```

1. See [:material-code-braces: AccessDeniedExceptionTypeDef](./type_defs.md#accessdeniedexceptiontypedef) 
2. See [:material-code-braces: BadGatewayExceptionTypeDef](./type_defs.md#badgatewayexceptiontypedef) 
3. See [:material-code-braces: PayloadPartTypeDef](./type_defs.md#payloadparttypedef) 
4. See [:material-code-braces: ConflictExceptionTypeDef](./type_defs.md#conflictexceptiontypedef) 
5. See [:material-code-braces: DependencyFailedExceptionTypeDef](./type_defs.md#dependencyfailedexceptiontypedef) 
6. See [:material-code-braces: FilePartTypeDef](./type_defs.md#fileparttypedef) 
7. See [:material-code-braces: InternalServerExceptionTypeDef](./type_defs.md#internalserverexceptiontypedef) 
8. See [:material-code-braces: ResourceNotFoundExceptionTypeDef](./type_defs.md#resourcenotfoundexceptiontypedef) 
9. See [:material-code-braces: ReturnControlPayloadTypeDef](./type_defs.md#returncontrolpayloadtypedef) 
10. See [:material-code-braces: ServiceQuotaExceededExceptionTypeDef](./type_defs.md#servicequotaexceededexceptiontypedef) 
11. See [:material-code-braces: ThrottlingExceptionTypeDef](./type_defs.md#throttlingexceptiontypedef) 
12. See [:material-code-braces: TracePartTypeDef](./type_defs.md#traceparttypedef) 
13. See [:material-code-braces: ValidationExceptionTypeDef](./type_defs.md#validationexceptiontypedef) 
## InvokeInlineAgentResponseTypeDef

```python
# InvokeInlineAgentResponseTypeDef definition

class InvokeInlineAgentResponseTypeDef(TypedDict):
    completion: AioEventStream[InlineAgentResponseStreamTypeDef],  # (1)
    contentType: str,
    sessionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InlineAgentResponseStreamTypeDef](./type_defs.md#inlineagentresponsestreamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InvokeAgentResponseTypeDef

```python
# InvokeAgentResponseTypeDef definition

class InvokeAgentResponseTypeDef(TypedDict):
    completion: AioEventStream[ResponseStreamTypeDef],  # (1)
    contentType: str,
    memoryId: str,
    sessionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResponseStreamTypeDef](./type_defs.md#responsestreamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
