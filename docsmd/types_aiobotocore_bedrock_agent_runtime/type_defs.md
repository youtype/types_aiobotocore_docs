# Type definitions

> [Index](../README.md) > [AgentsforBedrockRuntime](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AgentsforBedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime)
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




## AccessDeniedExceptionTypeDef

```python
# AccessDeniedExceptionTypeDef definition

class AccessDeniedExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

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

## FunctionParameterTypeDef

```python
# FunctionParameterTypeDef definition

class FunctionParameterTypeDef(TypedDict):
    name: NotRequired[str],
    type: NotRequired[str],
    value: NotRequired[str],
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
## TextInferenceConfigTypeDef

```python
# TextInferenceConfigTypeDef definition

class TextInferenceConfigTypeDef(TypedDict):
    maxTokens: NotRequired[int],
    stopSequences: NotRequired[Sequence[str]],
    temperature: NotRequired[float],
    topP: NotRequired[float],
```

## InferenceConfigurationTypeDef

```python
# InferenceConfigurationTypeDef definition

class InferenceConfigurationTypeDef(TypedDict):
    maximumLength: NotRequired[int],
    stopSequences: NotRequired[List[str]],
    temperature: NotRequired[float],
    topK: NotRequired[int],
    topP: NotRequired[float],
```

## KnowledgeBaseLookupInputTypeDef

```python
# KnowledgeBaseLookupInputTypeDef definition

class KnowledgeBaseLookupInputTypeDef(TypedDict):
    knowledgeBaseId: NotRequired[str],
    text: NotRequired[str],
```

## KnowledgeBaseQueryTypeDef

```python
# KnowledgeBaseQueryTypeDef definition

class KnowledgeBaseQueryTypeDef(TypedDict):
    text: str,
```

## RetrievalResultContentTypeDef

```python
# RetrievalResultContentTypeDef definition

class RetrievalResultContentTypeDef(TypedDict):
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

## RetrievalResultConfluenceLocationTypeDef

```python
# RetrievalResultConfluenceLocationTypeDef definition

class RetrievalResultConfluenceLocationTypeDef(TypedDict):
    url: NotRequired[str],
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
## ApiResultTypeDef

```python
# ApiResultTypeDef definition

class ApiResultTypeDef(TypedDict):
    actionGroup: str,
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
## FunctionResultTypeDef

```python
# FunctionResultTypeDef definition

class FunctionResultTypeDef(TypedDict):
    actionGroup: str,
    confirmationState: NotRequired[ConfirmationStateType],  # (1)
    function: NotRequired[str],
    responseBody: NotRequired[Mapping[str, ContentBodyTypeDef]],  # (2)
    responseState: NotRequired[ResponseStateType],  # (3)
```

1. See [:material-code-brackets: ConfirmationStateType](./literals.md#confirmationstatetype) 
2. See [:material-code-braces: ContentBodyTypeDef](./type_defs.md#contentbodytypedef) 
3. See [:material-code-brackets: ResponseStateType](./literals.md#responsestatetype) 
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

## FilePartTypeDef

```python
# FilePartTypeDef definition

class FilePartTypeDef(TypedDict):
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
## FunctionInvocationInputTypeDef

```python
# FunctionInvocationInputTypeDef definition

class FunctionInvocationInputTypeDef(TypedDict):
    actionGroup: str,
    actionInvocationType: NotRequired[ActionInvocationTypeType],  # (1)
    function: NotRequired[str],
    parameters: NotRequired[List[FunctionParameterTypeDef]],  # (2)
```

1. See [:material-code-brackets: ActionInvocationTypeType](./literals.md#actioninvocationtypetype) 
2. See [:material-code-braces: FunctionParameterTypeDef](./type_defs.md#functionparametertypedef) 
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
    inferenceConfiguration: NotRequired[InferenceConfigurationTypeDef],  # (1)
    overrideLambda: NotRequired[str],
    parserMode: NotRequired[CreationModeType],  # (2)
    promptCreationMode: NotRequired[CreationModeType],  # (2)
    text: NotRequired[str],
    traceId: NotRequired[str],
    type: NotRequired[PromptTypeType],  # (4)
```

1. See [:material-code-braces: InferenceConfigurationTypeDef](./type_defs.md#inferenceconfigurationtypedef) 
2. See [:material-code-brackets: CreationModeType](./literals.md#creationmodetype) 
3. See [:material-code-brackets: CreationModeType](./literals.md#creationmodetype) 
4. See [:material-code-brackets: PromptTypeType](./literals.md#prompttypetype) 
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
## RetrievalResultLocationTypeDef

```python
# RetrievalResultLocationTypeDef definition

class RetrievalResultLocationTypeDef(TypedDict):
    type: RetrievalResultLocationTypeType,  # (5)
    confluenceLocation: NotRequired[RetrievalResultConfluenceLocationTypeDef],  # (1)
    s3Location: NotRequired[RetrievalResultS3LocationTypeDef],  # (2)
    salesforceLocation: NotRequired[RetrievalResultSalesforceLocationTypeDef],  # (3)
    sharePointLocation: NotRequired[RetrievalResultSharePointLocationTypeDef],  # (4)
    webLocation: NotRequired[RetrievalResultWebLocationTypeDef],  # (6)
```

1. See [:material-code-braces: RetrievalResultConfluenceLocationTypeDef](./type_defs.md#retrievalresultconfluencelocationtypedef) 
2. See [:material-code-braces: RetrievalResultS3LocationTypeDef](./type_defs.md#retrievalresults3locationtypedef) 
3. See [:material-code-braces: RetrievalResultSalesforceLocationTypeDef](./type_defs.md#retrievalresultsalesforcelocationtypedef) 
4. See [:material-code-braces: RetrievalResultSharePointLocationTypeDef](./type_defs.md#retrievalresultsharepointlocationtypedef) 
5. See [:material-code-brackets: RetrievalResultLocationTypeType](./literals.md#retrievalresultlocationtypetype) 
6. See [:material-code-braces: RetrievalResultWebLocationTypeDef](./type_defs.md#retrievalresultweblocationtypedef) 
## TextResponsePartTypeDef

```python
# TextResponsePartTypeDef definition

class TextResponsePartTypeDef(TypedDict):
    span: NotRequired[SpanTypeDef],  # (1)
    text: NotRequired[str],
```

1. See [:material-code-braces: SpanTypeDef](./type_defs.md#spantypedef) 
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
## InvocationResultMemberTypeDef

```python
# InvocationResultMemberTypeDef definition

class InvocationResultMemberTypeDef(TypedDict):
    apiResult: NotRequired[ApiResultTypeDef],  # (1)
    functionResult: NotRequired[FunctionResultTypeDef],  # (2)
```

1. See [:material-code-braces: ApiResultTypeDef](./type_defs.md#apiresulttypedef) 
2. See [:material-code-braces: FunctionResultTypeDef](./type_defs.md#functionresulttypedef) 
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
## KnowledgeBaseVectorSearchConfigurationPaginatorTypeDef

```python
# KnowledgeBaseVectorSearchConfigurationPaginatorTypeDef definition

class KnowledgeBaseVectorSearchConfigurationPaginatorTypeDef(TypedDict):
    filter: NotRequired[RetrievalFilterPaginatorTypeDef],  # (1)
    numberOfResults: NotRequired[int],
    overrideSearchType: NotRequired[SearchTypeType],  # (2)
```

1. See [:material-code-braces: RetrievalFilterPaginatorTypeDef](./type_defs.md#retrievalfilterpaginatortypedef) 
2. See [:material-code-brackets: SearchTypeType](./literals.md#searchtypetype) 
## KnowledgeBaseVectorSearchConfigurationTypeDef

```python
# KnowledgeBaseVectorSearchConfigurationTypeDef definition

class KnowledgeBaseVectorSearchConfigurationTypeDef(TypedDict):
    filter: NotRequired[RetrievalFilterTypeDef],  # (1)
    numberOfResults: NotRequired[int],
    overrideSearchType: NotRequired[SearchTypeType],  # (2)
```

1. See [:material-code-braces: RetrievalFilterTypeDef](./type_defs.md#retrievalfiltertypedef) 
2. See [:material-code-brackets: SearchTypeType](./literals.md#searchtypetype) 
## InvokeFlowRequestRequestTypeDef

```python
# InvokeFlowRequestRequestTypeDef definition

class InvokeFlowRequestRequestTypeDef(TypedDict):
    flowAliasIdentifier: str,
    flowIdentifier: str,
    inputs: Sequence[FlowInputTypeDef],  # (1)
```

1. See [:material-code-braces: FlowInputTypeDef](./type_defs.md#flowinputtypedef) 
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
    internalServerException: NotRequired[InternalServerExceptionTypeDef],  # (7)
    resourceNotFoundException: NotRequired[ResourceNotFoundExceptionTypeDef],  # (8)
    serviceQuotaExceededException: NotRequired[ServiceQuotaExceededExceptionTypeDef],  # (9)
    throttlingException: NotRequired[ThrottlingExceptionTypeDef],  # (10)
    validationException: NotRequired[ValidationExceptionTypeDef],  # (11)
```

1. See [:material-code-braces: AccessDeniedExceptionTypeDef](./type_defs.md#accessdeniedexceptiontypedef) 
2. See [:material-code-braces: BadGatewayExceptionTypeDef](./type_defs.md#badgatewayexceptiontypedef) 
3. See [:material-code-braces: ConflictExceptionTypeDef](./type_defs.md#conflictexceptiontypedef) 
4. See [:material-code-braces: DependencyFailedExceptionTypeDef](./type_defs.md#dependencyfailedexceptiontypedef) 
5. See [:material-code-braces: FlowCompletionEventTypeDef](./type_defs.md#flowcompletioneventtypedef) 
6. See [:material-code-braces: FlowOutputEventTypeDef](./type_defs.md#flowoutputeventtypedef) 
7. See [:material-code-braces: InternalServerExceptionTypeDef](./type_defs.md#internalserverexceptiontypedef) 
8. See [:material-code-braces: ResourceNotFoundExceptionTypeDef](./type_defs.md#resourcenotfoundexceptiontypedef) 
9. See [:material-code-braces: ServiceQuotaExceededExceptionTypeDef](./type_defs.md#servicequotaexceededexceptiontypedef) 
10. See [:material-code-braces: ThrottlingExceptionTypeDef](./type_defs.md#throttlingexceptiontypedef) 
11. See [:material-code-braces: ValidationExceptionTypeDef](./type_defs.md#validationexceptiontypedef) 
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
## ApiInvocationInputTypeDef

```python
# ApiInvocationInputTypeDef definition

class ApiInvocationInputTypeDef(TypedDict):
    actionGroup: str,
    actionInvocationType: NotRequired[ActionInvocationTypeType],  # (1)
    apiPath: NotRequired[str],
    httpMethod: NotRequired[str],
    parameters: NotRequired[List[ApiParameterTypeDef]],  # (2)
    requestBody: NotRequired[ApiRequestBodyTypeDef],  # (3)
```

1. See [:material-code-brackets: ActionInvocationTypeType](./literals.md#actioninvocationtypetype) 
2. See [:material-code-braces: ApiParameterTypeDef](./type_defs.md#apiparametertypedef) 
3. See [:material-code-braces: ApiRequestBodyTypeDef](./type_defs.md#apirequestbodytypedef) 
## InvocationInputTypeDef

```python
# InvocationInputTypeDef definition

class InvocationInputTypeDef(TypedDict):
    actionGroupInvocationInput: NotRequired[ActionGroupInvocationInputTypeDef],  # (1)
    codeInterpreterInvocationInput: NotRequired[CodeInterpreterInvocationInputTypeDef],  # (2)
    invocationType: NotRequired[InvocationTypeType],  # (3)
    knowledgeBaseLookupInput: NotRequired[KnowledgeBaseLookupInputTypeDef],  # (4)
    traceId: NotRequired[str],
```

1. See [:material-code-braces: ActionGroupInvocationInputTypeDef](./type_defs.md#actiongroupinvocationinputtypedef) 
2. See [:material-code-braces: CodeInterpreterInvocationInputTypeDef](./type_defs.md#codeinterpreterinvocationinputtypedef) 
3. See [:material-code-brackets: InvocationTypeType](./literals.md#invocationtypetype) 
4. See [:material-code-braces: KnowledgeBaseLookupInputTypeDef](./type_defs.md#knowledgebaselookupinputtypedef) 
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
## RetrieveResponseTypeDef

```python
# RetrieveResponseTypeDef definition

class RetrieveResponseTypeDef(TypedDict):
    retrievalResults: List[KnowledgeBaseRetrievalResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: KnowledgeBaseRetrievalResultTypeDef](./type_defs.md#knowledgebaseretrievalresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## InvocationInputMemberTypeDef

```python
# InvocationInputMemberTypeDef definition

class InvocationInputMemberTypeDef(TypedDict):
    apiInvocationInput: NotRequired[ApiInvocationInputTypeDef],  # (1)
    functionInvocationInput: NotRequired[FunctionInvocationInputTypeDef],  # (2)
```

1. See [:material-code-braces: ApiInvocationInputTypeDef](./type_defs.md#apiinvocationinputtypedef) 
2. See [:material-code-braces: FunctionInvocationInputTypeDef](./type_defs.md#functioninvocationinputtypedef) 
## RetrieveRequestRetrievePaginateTypeDef

```python
# RetrieveRequestRetrievePaginateTypeDef definition

class RetrieveRequestRetrievePaginateTypeDef(TypedDict):
    knowledgeBaseId: str,
    retrievalQuery: KnowledgeBaseQueryTypeDef,  # (1)
    retrievalConfiguration: NotRequired[KnowledgeBaseRetrievalConfigurationPaginatorTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: KnowledgeBaseQueryTypeDef](./type_defs.md#knowledgebasequerytypedef) 
2. See [:material-code-braces: KnowledgeBaseRetrievalConfigurationPaginatorTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationpaginatortypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
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
## RetrieveRequestRequestTypeDef

```python
# RetrieveRequestRequestTypeDef definition

class RetrieveRequestRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    retrievalQuery: KnowledgeBaseQueryTypeDef,  # (1)
    nextToken: NotRequired[str],
    retrievalConfiguration: NotRequired[KnowledgeBaseRetrievalConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: KnowledgeBaseQueryTypeDef](./type_defs.md#knowledgebasequerytypedef) 
2. See [:material-code-braces: KnowledgeBaseRetrievalConfigurationTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationtypedef) 
## ObservationTypeDef

```python
# ObservationTypeDef definition

class ObservationTypeDef(TypedDict):
    actionGroupInvocationOutput: NotRequired[ActionGroupInvocationOutputTypeDef],  # (1)
    codeInterpreterInvocationOutput: NotRequired[CodeInterpreterInvocationOutputTypeDef],  # (2)
    finalResponse: NotRequired[FinalResponseTypeDef],  # (3)
    knowledgeBaseLookupOutput: NotRequired[KnowledgeBaseLookupOutputTypeDef],  # (4)
    repromptResponse: NotRequired[RepromptResponseTypeDef],  # (5)
    traceId: NotRequired[str],
    type: NotRequired[TypeType],  # (6)
```

1. See [:material-code-braces: ActionGroupInvocationOutputTypeDef](./type_defs.md#actiongroupinvocationoutputtypedef) 
2. See [:material-code-braces: CodeInterpreterInvocationOutputTypeDef](./type_defs.md#codeinterpreterinvocationoutputtypedef) 
3. See [:material-code-braces: FinalResponseTypeDef](./type_defs.md#finalresponsetypedef) 
4. See [:material-code-braces: KnowledgeBaseLookupOutputTypeDef](./type_defs.md#knowledgebaselookupoutputtypedef) 
5. See [:material-code-braces: RepromptResponseTypeDef](./type_defs.md#repromptresponsetypedef) 
6. See [:material-code-brackets: TypeType](./literals.md#typetype) 
## AttributionTypeDef

```python
# AttributionTypeDef definition

class AttributionTypeDef(TypedDict):
    citations: NotRequired[List[CitationTypeDef]],  # (1)
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
## ReturnControlPayloadTypeDef

```python
# ReturnControlPayloadTypeDef definition

class ReturnControlPayloadTypeDef(TypedDict):
    invocationId: NotRequired[str],
    invocationInputs: NotRequired[List[InvocationInputMemberTypeDef]],  # (1)
```

1. See [:material-code-braces: InvocationInputMemberTypeDef](./type_defs.md#invocationinputmembertypedef) 
## SessionStateTypeDef

```python
# SessionStateTypeDef definition

class SessionStateTypeDef(TypedDict):
    files: NotRequired[Sequence[InputFileTypeDef]],  # (1)
    invocationId: NotRequired[str],
    knowledgeBaseConfigurations: NotRequired[Sequence[KnowledgeBaseConfigurationTypeDef]],  # (2)
    promptSessionAttributes: NotRequired[Mapping[str, str]],
    returnControlInvocationResults: NotRequired[Sequence[InvocationResultMemberTypeDef]],  # (3)
    sessionAttributes: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: InputFileTypeDef](./type_defs.md#inputfiletypedef) 
2. See [:material-code-braces: KnowledgeBaseConfigurationTypeDef](./type_defs.md#knowledgebaseconfigurationtypedef) 
3. See [:material-code-braces: InvocationResultMemberTypeDef](./type_defs.md#invocationresultmembertypedef) 
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
## PayloadPartTypeDef

```python
# PayloadPartTypeDef definition

class PayloadPartTypeDef(TypedDict):
    attribution: NotRequired[AttributionTypeDef],  # (1)
    bytes: NotRequired[bytes],
```

1. See [:material-code-braces: AttributionTypeDef](./type_defs.md#attributiontypedef) 
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
```

1. See [:material-code-braces: SessionStateTypeDef](./type_defs.md#sessionstatetypedef) 
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
## TraceTypeDef

```python
# TraceTypeDef definition

class TraceTypeDef(TypedDict):
    failureTrace: NotRequired[FailureTraceTypeDef],  # (1)
    guardrailTrace: NotRequired[GuardrailTraceTypeDef],  # (2)
    orchestrationTrace: NotRequired[OrchestrationTraceTypeDef],  # (3)
    postProcessingTrace: NotRequired[PostProcessingTraceTypeDef],  # (4)
    preProcessingTrace: NotRequired[PreProcessingTraceTypeDef],  # (5)
```

1. See [:material-code-braces: FailureTraceTypeDef](./type_defs.md#failuretracetypedef) 
2. See [:material-code-braces: GuardrailTraceTypeDef](./type_defs.md#guardrailtracetypedef) 
3. See [:material-code-braces: OrchestrationTraceTypeDef](./type_defs.md#orchestrationtracetypedef) 
4. See [:material-code-braces: PostProcessingTraceTypeDef](./type_defs.md#postprocessingtracetypedef) 
5. See [:material-code-braces: PreProcessingTraceTypeDef](./type_defs.md#preprocessingtracetypedef) 
## TracePartTypeDef

```python
# TracePartTypeDef definition

class TracePartTypeDef(TypedDict):
    agentAliasId: NotRequired[str],
    agentId: NotRequired[str],
    agentVersion: NotRequired[str],
    sessionId: NotRequired[str],
    trace: NotRequired[TraceTypeDef],  # (1)
```

1. See [:material-code-braces: TraceTypeDef](./type_defs.md#tracetypedef) 
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
