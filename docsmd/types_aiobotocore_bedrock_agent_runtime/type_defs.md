# Type definitions

> [Index](../README.md) > [AgentsforBedrockRuntime](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AgentsforBedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#agentsforbedrockruntime)
    type annotations stubs module [types-aiobotocore-bedrock-agent-runtime](https://pypi.org/project/types-aiobotocore-bedrock-agent-runtime/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


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
# InferenceConfigurationUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InferenceConfigurationUnionTypeDef


def get_value() -> InferenceConfigurationUnionTypeDef:
    return ...


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
# ApiResultUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ApiResultUnionTypeDef


def get_value() -> ApiResultUnionTypeDef:
    return ...


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
# FunctionResultUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FunctionResultUnionTypeDef


def get_value() -> FunctionResultUnionTypeDef:
    return ...


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
# RerankDocumentUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RerankDocumentUnionTypeDef


def get_value() -> RerankDocumentUnionTypeDef:
    return ...


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
# InvocationResultMemberUnionTypeDef Union usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InvocationResultMemberUnionTypeDef


def get_value() -> InvocationResultMemberUnionTypeDef:
    return ...


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
# S3IdentifierTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import S3IdentifierTypeDef


def get_value() -> S3IdentifierTypeDef:
    return {
        "s3BucketName": ...,
    }


# S3IdentifierTypeDef definition

class S3IdentifierTypeDef(TypedDict):
    s3BucketName: NotRequired[str],
    s3ObjectKey: NotRequired[str],
```

## AccessDeniedExceptionTypeDef

```python
# AccessDeniedExceptionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import AccessDeniedExceptionTypeDef


def get_value() -> AccessDeniedExceptionTypeDef:
    return {
        "message": ...,
    }


# AccessDeniedExceptionTypeDef definition

class AccessDeniedExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## ActionGroupExecutorTypeDef

```python
# ActionGroupExecutorTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ActionGroupExecutorTypeDef


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
## ParameterTypeDef

```python
# ParameterTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ParameterTypeDef


def get_value() -> ParameterTypeDef:
    return {
        "name": ...,
    }


# ParameterTypeDef definition

class ParameterTypeDef(TypedDict):
    name: NotRequired[str],
    type: NotRequired[str],
    value: NotRequired[str],
```

## ActionGroupInvocationOutputTypeDef

```python
# ActionGroupInvocationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ActionGroupInvocationOutputTypeDef


def get_value() -> ActionGroupInvocationOutputTypeDef:
    return {
        "text": ...,
    }


# ActionGroupInvocationOutputTypeDef definition

class ActionGroupInvocationOutputTypeDef(TypedDict):
    text: NotRequired[str],
```

## AnalyzePromptEventTypeDef

```python
# AnalyzePromptEventTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import AnalyzePromptEventTypeDef


def get_value() -> AnalyzePromptEventTypeDef:
    return {
        "message": ...,
    }


# AnalyzePromptEventTypeDef definition

class AnalyzePromptEventTypeDef(TypedDict):
    message: NotRequired[str],
```

## ApiParameterTypeDef

```python
# ApiParameterTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ApiParameterTypeDef


def get_value() -> ApiParameterTypeDef:
    return {
        "name": ...,
    }


# ApiParameterTypeDef definition

class ApiParameterTypeDef(TypedDict):
    name: NotRequired[str],
    type: NotRequired[str],
    value: NotRequired[str],
```

## ContentBodyTypeDef

```python
# ContentBodyTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ContentBodyTypeDef


def get_value() -> ContentBodyTypeDef:
    return {
        "body": ...,
    }


# ContentBodyTypeDef definition

class ContentBodyTypeDef(TypedDict):
    body: NotRequired[str],
```

## BadGatewayExceptionTypeDef

```python
# BadGatewayExceptionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import BadGatewayExceptionTypeDef


def get_value() -> BadGatewayExceptionTypeDef:
    return {
        "message": ...,
    }


# BadGatewayExceptionTypeDef definition

class BadGatewayExceptionTypeDef(TypedDict):
    message: NotRequired[str],
    resourceName: NotRequired[str],
```

## PerformanceConfigurationTypeDef

```python
# PerformanceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import PerformanceConfigurationTypeDef


def get_value() -> PerformanceConfigurationTypeDef:
    return {
        "latency": ...,
    }


# PerformanceConfigurationTypeDef definition

class PerformanceConfigurationTypeDef(TypedDict):
    latency: NotRequired[PerformanceConfigLatencyType],  # (1)
```

1. See [:material-code-brackets: PerformanceConfigLatencyType](./literals.md#performanceconfiglatencytype) 
## BedrockRerankingModelConfigurationTypeDef

```python
# BedrockRerankingModelConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import BedrockRerankingModelConfigurationTypeDef


def get_value() -> BedrockRerankingModelConfigurationTypeDef:
    return {
        "additionalModelRequestFields": ...,
    }


# BedrockRerankingModelConfigurationTypeDef definition

class BedrockRerankingModelConfigurationTypeDef(TypedDict):
    modelArn: str,
    additionalModelRequestFields: NotRequired[Mapping[str, Mapping[str, Any]]],
```

## CallerTypeDef

```python
# CallerTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import CallerTypeDef


def get_value() -> CallerTypeDef:
    return {
        "agentAliasArn": ...,
    }


# CallerTypeDef definition

class CallerTypeDef(TypedDict):
    agentAliasArn: NotRequired[str],
```

## CodeInterpreterInvocationInputTypeDef

```python
# CodeInterpreterInvocationInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import CodeInterpreterInvocationInputTypeDef


def get_value() -> CodeInterpreterInvocationInputTypeDef:
    return {
        "code": ...,
    }


# CodeInterpreterInvocationInputTypeDef definition

class CodeInterpreterInvocationInputTypeDef(TypedDict):
    code: NotRequired[str],
    files: NotRequired[List[str]],
```

## CodeInterpreterInvocationOutputTypeDef

```python
# CodeInterpreterInvocationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import CodeInterpreterInvocationOutputTypeDef


def get_value() -> CodeInterpreterInvocationOutputTypeDef:
    return {
        "executionError": ...,
    }


# CodeInterpreterInvocationOutputTypeDef definition

class CodeInterpreterInvocationOutputTypeDef(TypedDict):
    executionError: NotRequired[str],
    executionOutput: NotRequired[str],
    executionTimeout: NotRequired[bool],
    files: NotRequired[List[str]],
```

## ConflictExceptionTypeDef

```python
# ConflictExceptionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ConflictExceptionTypeDef


def get_value() -> ConflictExceptionTypeDef:
    return {
        "message": ...,
    }


# ConflictExceptionTypeDef definition

class ConflictExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## ContentBlockTypeDef

```python
# ContentBlockTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ContentBlockTypeDef


def get_value() -> ContentBlockTypeDef:
    return {
        "text": ...,
    }


# ContentBlockTypeDef definition

class ContentBlockTypeDef(TypedDict):
    text: NotRequired[str],
```

## CustomOrchestrationTraceEventTypeDef

```python
# CustomOrchestrationTraceEventTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import CustomOrchestrationTraceEventTypeDef


def get_value() -> CustomOrchestrationTraceEventTypeDef:
    return {
        "text": ...,
    }


# CustomOrchestrationTraceEventTypeDef definition

class CustomOrchestrationTraceEventTypeDef(TypedDict):
    text: NotRequired[str],
```

## DeleteAgentMemoryRequestTypeDef

```python
# DeleteAgentMemoryRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import DeleteAgentMemoryRequestTypeDef


def get_value() -> DeleteAgentMemoryRequestTypeDef:
    return {
        "agentAliasId": ...,
    }


# DeleteAgentMemoryRequestTypeDef definition

class DeleteAgentMemoryRequestTypeDef(TypedDict):
    agentAliasId: str,
    agentId: str,
    memoryId: NotRequired[str],
    sessionId: NotRequired[str],
```

## DependencyFailedExceptionTypeDef

```python
# DependencyFailedExceptionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import DependencyFailedExceptionTypeDef


def get_value() -> DependencyFailedExceptionTypeDef:
    return {
        "message": ...,
    }


# DependencyFailedExceptionTypeDef definition

class DependencyFailedExceptionTypeDef(TypedDict):
    message: NotRequired[str],
    resourceName: NotRequired[str],
```

## S3ObjectDocTypeDef

```python
# S3ObjectDocTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import S3ObjectDocTypeDef


def get_value() -> S3ObjectDocTypeDef:
    return {
        "uri": ...,
    }


# S3ObjectDocTypeDef definition

class S3ObjectDocTypeDef(TypedDict):
    uri: str,
```

## GuardrailConfigurationTypeDef

```python
# GuardrailConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GuardrailConfigurationTypeDef


def get_value() -> GuardrailConfigurationTypeDef:
    return {
        "guardrailId": ...,
    }


# GuardrailConfigurationTypeDef definition

class GuardrailConfigurationTypeDef(TypedDict):
    guardrailId: str,
    guardrailVersion: str,
```

## PromptTemplateTypeDef

```python
# PromptTemplateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import PromptTemplateTypeDef


def get_value() -> PromptTemplateTypeDef:
    return {
        "textPromptTemplate": ...,
    }


# PromptTemplateTypeDef definition

class PromptTemplateTypeDef(TypedDict):
    textPromptTemplate: NotRequired[str],
```

## FailureTraceTypeDef

```python
# FailureTraceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FailureTraceTypeDef


def get_value() -> FailureTraceTypeDef:
    return {
        "failureReason": ...,
    }


# FailureTraceTypeDef definition

class FailureTraceTypeDef(TypedDict):
    failureReason: NotRequired[str],
    traceId: NotRequired[str],
```

## FieldForRerankingTypeDef

```python
# FieldForRerankingTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FieldForRerankingTypeDef


def get_value() -> FieldForRerankingTypeDef:
    return {
        "fieldName": ...,
    }


# FieldForRerankingTypeDef definition

class FieldForRerankingTypeDef(TypedDict):
    fieldName: str,
```

## OutputFileTypeDef

```python
# OutputFileTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import OutputFileTypeDef


def get_value() -> OutputFileTypeDef:
    return {
        "bytes": ...,
    }


# OutputFileTypeDef definition

class OutputFileTypeDef(TypedDict):
    bytes: NotRequired[bytes],
    name: NotRequired[str],
    type: NotRequired[str],
```

## S3ObjectFileTypeDef

```python
# S3ObjectFileTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import S3ObjectFileTypeDef


def get_value() -> S3ObjectFileTypeDef:
    return {
        "uri": ...,
    }


# S3ObjectFileTypeDef definition

class S3ObjectFileTypeDef(TypedDict):
    uri: str,
```

## FilterAttributeTypeDef

```python
# FilterAttributeTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FilterAttributeTypeDef


def get_value() -> FilterAttributeTypeDef:
    return {
        "key": ...,
    }


# FilterAttributeTypeDef definition

class FilterAttributeTypeDef(TypedDict):
    key: str,
    value: Mapping[str, Any],
```

## FinalResponseTypeDef

```python
# FinalResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FinalResponseTypeDef


def get_value() -> FinalResponseTypeDef:
    return {
        "text": ...,
    }


# FinalResponseTypeDef definition

class FinalResponseTypeDef(TypedDict):
    text: NotRequired[str],
```

## FlowCompletionEventTypeDef

```python
# FlowCompletionEventTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FlowCompletionEventTypeDef


def get_value() -> FlowCompletionEventTypeDef:
    return {
        "completionReason": ...,
    }


# FlowCompletionEventTypeDef definition

class FlowCompletionEventTypeDef(TypedDict):
    completionReason: FlowCompletionReasonType,  # (1)
```

1. See [:material-code-brackets: FlowCompletionReasonType](./literals.md#flowcompletionreasontype) 
## FlowInputContentTypeDef

```python
# FlowInputContentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FlowInputContentTypeDef


def get_value() -> FlowInputContentTypeDef:
    return {
        "document": ...,
    }


# FlowInputContentTypeDef definition

class FlowInputContentTypeDef(TypedDict):
    document: NotRequired[Mapping[str, Any]],
```

## FlowMultiTurnInputContentTypeDef

```python
# FlowMultiTurnInputContentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FlowMultiTurnInputContentTypeDef


def get_value() -> FlowMultiTurnInputContentTypeDef:
    return {
        "document": ...,
    }


# FlowMultiTurnInputContentTypeDef definition

class FlowMultiTurnInputContentTypeDef(TypedDict):
    document: NotRequired[Dict[str, Any]],
```

## FlowOutputContentTypeDef

```python
# FlowOutputContentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FlowOutputContentTypeDef


def get_value() -> FlowOutputContentTypeDef:
    return {
        "document": ...,
    }


# FlowOutputContentTypeDef definition

class FlowOutputContentTypeDef(TypedDict):
    document: NotRequired[Dict[str, Any]],
```

## InternalServerExceptionTypeDef

```python
# InternalServerExceptionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InternalServerExceptionTypeDef


def get_value() -> InternalServerExceptionTypeDef:
    return {
        "message": ...,
    }


# InternalServerExceptionTypeDef definition

class InternalServerExceptionTypeDef(TypedDict):
    message: NotRequired[str],
    reason: NotRequired[str],
```

## ResourceNotFoundExceptionTypeDef

```python
# ResourceNotFoundExceptionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ResourceNotFoundExceptionTypeDef


def get_value() -> ResourceNotFoundExceptionTypeDef:
    return {
        "message": ...,
    }


# ResourceNotFoundExceptionTypeDef definition

class ResourceNotFoundExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## ServiceQuotaExceededExceptionTypeDef

```python
# ServiceQuotaExceededExceptionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ServiceQuotaExceededExceptionTypeDef


def get_value() -> ServiceQuotaExceededExceptionTypeDef:
    return {
        "message": ...,
    }


# ServiceQuotaExceededExceptionTypeDef definition

class ServiceQuotaExceededExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## ThrottlingExceptionTypeDef

```python
# ThrottlingExceptionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ThrottlingExceptionTypeDef


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

from types_aiobotocore_bedrock_agent_runtime.type_defs import ValidationExceptionTypeDef


def get_value() -> ValidationExceptionTypeDef:
    return {
        "message": ...,
    }


# ValidationExceptionTypeDef definition

class ValidationExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## FlowTraceConditionTypeDef

```python
# FlowTraceConditionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FlowTraceConditionTypeDef


def get_value() -> FlowTraceConditionTypeDef:
    return {
        "conditionName": ...,
    }


# FlowTraceConditionTypeDef definition

class FlowTraceConditionTypeDef(TypedDict):
    conditionName: str,
```

## FlowTraceNodeInputContentTypeDef

```python
# FlowTraceNodeInputContentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FlowTraceNodeInputContentTypeDef


def get_value() -> FlowTraceNodeInputContentTypeDef:
    return {
        "document": ...,
    }


# FlowTraceNodeInputContentTypeDef definition

class FlowTraceNodeInputContentTypeDef(TypedDict):
    document: NotRequired[Dict[str, Any]],
```

## FlowTraceNodeOutputContentTypeDef

```python
# FlowTraceNodeOutputContentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FlowTraceNodeOutputContentTypeDef


def get_value() -> FlowTraceNodeOutputContentTypeDef:
    return {
        "document": ...,
    }


# FlowTraceNodeOutputContentTypeDef definition

class FlowTraceNodeOutputContentTypeDef(TypedDict):
    document: NotRequired[Dict[str, Any]],
```

## ParameterDetailTypeDef

```python
# ParameterDetailTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ParameterDetailTypeDef


def get_value() -> ParameterDetailTypeDef:
    return {
        "description": ...,
    }


# ParameterDetailTypeDef definition

class ParameterDetailTypeDef(TypedDict):
    type: ParameterTypeType,  # (1)
    description: NotRequired[str],
    required: NotRequired[bool],
```

1. See [:material-code-brackets: ParameterTypeType](./literals.md#parametertypetype) 
## FunctionParameterTypeDef

```python
# FunctionParameterTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FunctionParameterTypeDef


def get_value() -> FunctionParameterTypeDef:
    return {
        "name": ...,
    }


# FunctionParameterTypeDef definition

class FunctionParameterTypeDef(TypedDict):
    name: NotRequired[str],
    type: NotRequired[str],
    value: NotRequired[str],
```

## QueryGenerationInputTypeDef

```python
# QueryGenerationInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import QueryGenerationInputTypeDef


def get_value() -> QueryGenerationInputTypeDef:
    return {
        "text": ...,
    }


# QueryGenerationInputTypeDef definition

class QueryGenerationInputTypeDef(TypedDict):
    text: str,
    type: InputQueryTypeType,  # (1)
```

1. See [:material-code-brackets: InputQueryTypeType](./literals.md#inputquerytypetype) 
## GeneratedQueryTypeDef

```python
# GeneratedQueryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GeneratedQueryTypeDef


def get_value() -> GeneratedQueryTypeDef:
    return {
        "sql": ...,
    }


# GeneratedQueryTypeDef definition

class GeneratedQueryTypeDef(TypedDict):
    sql: NotRequired[str],
    type: NotRequired[GeneratedQueryTypeType],  # (1)
```

1. See [:material-code-brackets: GeneratedQueryTypeType](./literals.md#generatedquerytypetype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ResponseMetadataTypeDef


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

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import PaginatorConfigTypeDef


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

## GetAgentMemoryRequestTypeDef

```python
# GetAgentMemoryRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GetAgentMemoryRequestTypeDef


def get_value() -> GetAgentMemoryRequestTypeDef:
    return {
        "agentAliasId": ...,
    }


# GetAgentMemoryRequestTypeDef definition

class GetAgentMemoryRequestTypeDef(TypedDict):
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
# GuardrailConfigurationWithArnTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GuardrailConfigurationWithArnTypeDef


def get_value() -> GuardrailConfigurationWithArnTypeDef:
    return {
        "guardrailIdentifier": ...,
    }


# GuardrailConfigurationWithArnTypeDef definition

class GuardrailConfigurationWithArnTypeDef(TypedDict):
    guardrailIdentifier: str,
    guardrailVersion: str,
```

## GuardrailContentFilterTypeDef

```python
# GuardrailContentFilterTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GuardrailContentFilterTypeDef


def get_value() -> GuardrailContentFilterTypeDef:
    return {
        "action": ...,
    }


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
# GuardrailCustomWordTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GuardrailCustomWordTypeDef


def get_value() -> GuardrailCustomWordTypeDef:
    return {
        "action": ...,
    }


# GuardrailCustomWordTypeDef definition

class GuardrailCustomWordTypeDef(TypedDict):
    action: NotRequired[GuardrailWordPolicyActionType],  # (1)
    match: NotRequired[str],
```

1. See [:material-code-brackets: GuardrailWordPolicyActionType](./literals.md#guardrailwordpolicyactiontype) 
## GuardrailEventTypeDef

```python
# GuardrailEventTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GuardrailEventTypeDef


def get_value() -> GuardrailEventTypeDef:
    return {
        "action": ...,
    }


# GuardrailEventTypeDef definition

class GuardrailEventTypeDef(TypedDict):
    action: NotRequired[GuadrailActionType],  # (1)
```

1. See [:material-code-brackets: GuadrailActionType](./literals.md#guadrailactiontype) 
## GuardrailManagedWordTypeDef

```python
# GuardrailManagedWordTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GuardrailManagedWordTypeDef


def get_value() -> GuardrailManagedWordTypeDef:
    return {
        "action": ...,
    }


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
# GuardrailPiiEntityFilterTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GuardrailPiiEntityFilterTypeDef


def get_value() -> GuardrailPiiEntityFilterTypeDef:
    return {
        "action": ...,
    }


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
# GuardrailRegexFilterTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GuardrailRegexFilterTypeDef


def get_value() -> GuardrailRegexFilterTypeDef:
    return {
        "action": ...,
    }


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
# GuardrailTopicTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GuardrailTopicTypeDef


def get_value() -> GuardrailTopicTypeDef:
    return {
        "action": ...,
    }


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
# MetadataAttributeSchemaTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import MetadataAttributeSchemaTypeDef


def get_value() -> MetadataAttributeSchemaTypeDef:
    return {
        "description": ...,
    }


# MetadataAttributeSchemaTypeDef definition

class MetadataAttributeSchemaTypeDef(TypedDict):
    description: str,
    key: str,
    type: AttributeTypeType,  # (1)
```

1. See [:material-code-brackets: AttributeTypeType](./literals.md#attributetypetype) 
## TextInferenceConfigTypeDef

```python
# TextInferenceConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import TextInferenceConfigTypeDef


def get_value() -> TextInferenceConfigTypeDef:
    return {
        "maxTokens": ...,
    }


# TextInferenceConfigTypeDef definition

class TextInferenceConfigTypeDef(TypedDict):
    maxTokens: NotRequired[int],
    stopSequences: NotRequired[Sequence[str]],
    temperature: NotRequired[float],
    topP: NotRequired[float],
```

## InferenceConfigurationOutputTypeDef

```python
# InferenceConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InferenceConfigurationOutputTypeDef


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

from types_aiobotocore_bedrock_agent_runtime.type_defs import InferenceConfigurationTypeDef


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

## TextPromptTypeDef

```python
# TextPromptTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import TextPromptTypeDef


def get_value() -> TextPromptTypeDef:
    return {
        "text": ...,
    }


# TextPromptTypeDef definition

class TextPromptTypeDef(TypedDict):
    text: str,
```

## KnowledgeBaseLookupInputTypeDef

```python
# KnowledgeBaseLookupInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import KnowledgeBaseLookupInputTypeDef


def get_value() -> KnowledgeBaseLookupInputTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# KnowledgeBaseLookupInputTypeDef definition

class KnowledgeBaseLookupInputTypeDef(TypedDict):
    knowledgeBaseId: NotRequired[str],
    text: NotRequired[str],
```

## StreamingConfigurationsTypeDef

```python
# StreamingConfigurationsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import StreamingConfigurationsTypeDef


def get_value() -> StreamingConfigurationsTypeDef:
    return {
        "applyGuardrailInterval": ...,
    }


# StreamingConfigurationsTypeDef definition

class StreamingConfigurationsTypeDef(TypedDict):
    applyGuardrailInterval: NotRequired[int],
    streamFinalResponse: NotRequired[bool],
```

## KnowledgeBaseQueryTypeDef

```python
# KnowledgeBaseQueryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import KnowledgeBaseQueryTypeDef


def get_value() -> KnowledgeBaseQueryTypeDef:
    return {
        "text": ...,
    }


# KnowledgeBaseQueryTypeDef definition

class KnowledgeBaseQueryTypeDef(TypedDict):
    text: str,
```

## MemorySessionSummaryTypeDef

```python
# MemorySessionSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import MemorySessionSummaryTypeDef


def get_value() -> MemorySessionSummaryTypeDef:
    return {
        "memoryId": ...,
    }


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
# UsageTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import UsageTypeDef


def get_value() -> UsageTypeDef:
    return {
        "inputTokens": ...,
    }


# UsageTypeDef definition

class UsageTypeDef(TypedDict):
    inputTokens: NotRequired[int],
    outputTokens: NotRequired[int],
```

## ModelNotReadyExceptionTypeDef

```python
# ModelNotReadyExceptionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ModelNotReadyExceptionTypeDef


def get_value() -> ModelNotReadyExceptionTypeDef:
    return {
        "message": ...,
    }


# ModelNotReadyExceptionTypeDef definition

class ModelNotReadyExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## RepromptResponseTypeDef

```python
# RepromptResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RepromptResponseTypeDef


def get_value() -> RepromptResponseTypeDef:
    return {
        "source": ...,
    }


# RepromptResponseTypeDef definition

class RepromptResponseTypeDef(TypedDict):
    source: NotRequired[SourceType],  # (1)
    text: NotRequired[str],
```

1. See [:material-code-brackets: SourceType](./literals.md#sourcetype) 
## QueryTransformationConfigurationTypeDef

```python
# QueryTransformationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import QueryTransformationConfigurationTypeDef


def get_value() -> QueryTransformationConfigurationTypeDef:
    return {
        "type": ...,
    }


# QueryTransformationConfigurationTypeDef definition

class QueryTransformationConfigurationTypeDef(TypedDict):
    type: QueryTransformationTypeType,  # (1)
```

1. See [:material-code-brackets: QueryTransformationTypeType](./literals.md#querytransformationtypetype) 
## RawResponseTypeDef

```python
# RawResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RawResponseTypeDef


def get_value() -> RawResponseTypeDef:
    return {
        "content": ...,
    }


# RawResponseTypeDef definition

class RawResponseTypeDef(TypedDict):
    content: NotRequired[str],
```

## RationaleTypeDef

```python
# RationaleTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RationaleTypeDef


def get_value() -> RationaleTypeDef:
    return {
        "text": ...,
    }


# RationaleTypeDef definition

class RationaleTypeDef(TypedDict):
    text: NotRequired[str],
    traceId: NotRequired[str],
```

## PostProcessingParsedResponseTypeDef

```python
# PostProcessingParsedResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import PostProcessingParsedResponseTypeDef


def get_value() -> PostProcessingParsedResponseTypeDef:
    return {
        "text": ...,
    }


# PostProcessingParsedResponseTypeDef definition

class PostProcessingParsedResponseTypeDef(TypedDict):
    text: NotRequired[str],
```

## PreProcessingParsedResponseTypeDef

```python
# PreProcessingParsedResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import PreProcessingParsedResponseTypeDef


def get_value() -> PreProcessingParsedResponseTypeDef:
    return {
        "isValid": ...,
    }


# PreProcessingParsedResponseTypeDef definition

class PreProcessingParsedResponseTypeDef(TypedDict):
    isValid: NotRequired[bool],
    rationale: NotRequired[str],
```

## RerankTextDocumentTypeDef

```python
# RerankTextDocumentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RerankTextDocumentTypeDef


def get_value() -> RerankTextDocumentTypeDef:
    return {
        "text": ...,
    }


# RerankTextDocumentTypeDef definition

class RerankTextDocumentTypeDef(TypedDict):
    text: NotRequired[str],
```

## RetrievalResultConfluenceLocationTypeDef

```python
# RetrievalResultConfluenceLocationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrievalResultConfluenceLocationTypeDef


def get_value() -> RetrievalResultConfluenceLocationTypeDef:
    return {
        "url": ...,
    }


# RetrievalResultConfluenceLocationTypeDef definition

class RetrievalResultConfluenceLocationTypeDef(TypedDict):
    url: NotRequired[str],
```

## RetrievalResultContentColumnTypeDef

```python
# RetrievalResultContentColumnTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrievalResultContentColumnTypeDef


def get_value() -> RetrievalResultContentColumnTypeDef:
    return {
        "columnName": ...,
    }


# RetrievalResultContentColumnTypeDef definition

class RetrievalResultContentColumnTypeDef(TypedDict):
    columnName: NotRequired[str],
    columnValue: NotRequired[str],
    type: NotRequired[RetrievalResultContentColumnTypeType],  # (1)
```

1. See [:material-code-brackets: RetrievalResultContentColumnTypeType](./literals.md#retrievalresultcontentcolumntypetype) 
## RetrievalResultCustomDocumentLocationTypeDef

```python
# RetrievalResultCustomDocumentLocationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrievalResultCustomDocumentLocationTypeDef


def get_value() -> RetrievalResultCustomDocumentLocationTypeDef:
    return {
        "id": ...,
    }


# RetrievalResultCustomDocumentLocationTypeDef definition

class RetrievalResultCustomDocumentLocationTypeDef(TypedDict):
    id: NotRequired[str],
```

## RetrievalResultKendraDocumentLocationTypeDef

```python
# RetrievalResultKendraDocumentLocationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrievalResultKendraDocumentLocationTypeDef


def get_value() -> RetrievalResultKendraDocumentLocationTypeDef:
    return {
        "uri": ...,
    }


# RetrievalResultKendraDocumentLocationTypeDef definition

class RetrievalResultKendraDocumentLocationTypeDef(TypedDict):
    uri: NotRequired[str],
```

## RetrievalResultS3LocationTypeDef

```python
# RetrievalResultS3LocationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrievalResultS3LocationTypeDef


def get_value() -> RetrievalResultS3LocationTypeDef:
    return {
        "uri": ...,
    }


# RetrievalResultS3LocationTypeDef definition

class RetrievalResultS3LocationTypeDef(TypedDict):
    uri: NotRequired[str],
```

## RetrievalResultSalesforceLocationTypeDef

```python
# RetrievalResultSalesforceLocationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrievalResultSalesforceLocationTypeDef


def get_value() -> RetrievalResultSalesforceLocationTypeDef:
    return {
        "url": ...,
    }


# RetrievalResultSalesforceLocationTypeDef definition

class RetrievalResultSalesforceLocationTypeDef(TypedDict):
    url: NotRequired[str],
```

## RetrievalResultSharePointLocationTypeDef

```python
# RetrievalResultSharePointLocationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrievalResultSharePointLocationTypeDef


def get_value() -> RetrievalResultSharePointLocationTypeDef:
    return {
        "url": ...,
    }


# RetrievalResultSharePointLocationTypeDef definition

class RetrievalResultSharePointLocationTypeDef(TypedDict):
    url: NotRequired[str],
```

## RetrievalResultSqlLocationTypeDef

```python
# RetrievalResultSqlLocationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrievalResultSqlLocationTypeDef


def get_value() -> RetrievalResultSqlLocationTypeDef:
    return {
        "query": ...,
    }


# RetrievalResultSqlLocationTypeDef definition

class RetrievalResultSqlLocationTypeDef(TypedDict):
    query: NotRequired[str],
```

## RetrievalResultWebLocationTypeDef

```python
# RetrievalResultWebLocationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrievalResultWebLocationTypeDef


def get_value() -> RetrievalResultWebLocationTypeDef:
    return {
        "url": ...,
    }


# RetrievalResultWebLocationTypeDef definition

class RetrievalResultWebLocationTypeDef(TypedDict):
    url: NotRequired[str],
```

## RetrieveAndGenerateInputTypeDef

```python
# RetrieveAndGenerateInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrieveAndGenerateInputTypeDef


def get_value() -> RetrieveAndGenerateInputTypeDef:
    return {
        "text": ...,
    }


# RetrieveAndGenerateInputTypeDef definition

class RetrieveAndGenerateInputTypeDef(TypedDict):
    text: str,
```

## RetrieveAndGenerateOutputEventTypeDef

```python
# RetrieveAndGenerateOutputEventTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrieveAndGenerateOutputEventTypeDef


def get_value() -> RetrieveAndGenerateOutputEventTypeDef:
    return {
        "text": ...,
    }


# RetrieveAndGenerateOutputEventTypeDef definition

class RetrieveAndGenerateOutputEventTypeDef(TypedDict):
    text: str,
```

## RetrieveAndGenerateOutputTypeDef

```python
# RetrieveAndGenerateOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrieveAndGenerateOutputTypeDef


def get_value() -> RetrieveAndGenerateOutputTypeDef:
    return {
        "text": ...,
    }


# RetrieveAndGenerateOutputTypeDef definition

class RetrieveAndGenerateOutputTypeDef(TypedDict):
    text: str,
```

## RetrieveAndGenerateSessionConfigurationTypeDef

```python
# RetrieveAndGenerateSessionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrieveAndGenerateSessionConfigurationTypeDef


def get_value() -> RetrieveAndGenerateSessionConfigurationTypeDef:
    return {
        "kmsKeyArn": ...,
    }


# RetrieveAndGenerateSessionConfigurationTypeDef definition

class RetrieveAndGenerateSessionConfigurationTypeDef(TypedDict):
    kmsKeyArn: str,
```

## SpanTypeDef

```python
# SpanTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import SpanTypeDef


def get_value() -> SpanTypeDef:
    return {
        "end": ...,
    }


# SpanTypeDef definition

class SpanTypeDef(TypedDict):
    end: NotRequired[int],
    start: NotRequired[int],
```

## TextToSqlKnowledgeBaseConfigurationTypeDef

```python
# TextToSqlKnowledgeBaseConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import TextToSqlKnowledgeBaseConfigurationTypeDef


def get_value() -> TextToSqlKnowledgeBaseConfigurationTypeDef:
    return {
        "knowledgeBaseArn": ...,
    }


# TextToSqlKnowledgeBaseConfigurationTypeDef definition

class TextToSqlKnowledgeBaseConfigurationTypeDef(TypedDict):
    knowledgeBaseArn: str,
```

## VectorSearchBedrockRerankingModelConfigurationTypeDef

```python
# VectorSearchBedrockRerankingModelConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import VectorSearchBedrockRerankingModelConfigurationTypeDef


def get_value() -> VectorSearchBedrockRerankingModelConfigurationTypeDef:
    return {
        "additionalModelRequestFields": ...,
    }


# VectorSearchBedrockRerankingModelConfigurationTypeDef definition

class VectorSearchBedrockRerankingModelConfigurationTypeDef(TypedDict):
    modelArn: str,
    additionalModelRequestFields: NotRequired[Mapping[str, Mapping[str, Any]]],
```

## APISchemaTypeDef

```python
# APISchemaTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import APISchemaTypeDef


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
## PropertyParametersTypeDef

```python
# PropertyParametersTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import PropertyParametersTypeDef


def get_value() -> PropertyParametersTypeDef:
    return {
        "properties": ...,
    }


# PropertyParametersTypeDef definition

class PropertyParametersTypeDef(TypedDict):
    properties: NotRequired[List[ParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
## RequestBodyTypeDef

```python
# RequestBodyTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RequestBodyTypeDef


def get_value() -> RequestBodyTypeDef:
    return {
        "content": ...,
    }


# RequestBodyTypeDef definition

class RequestBodyTypeDef(TypedDict):
    content: NotRequired[Dict[str, List[ParameterTypeDef]]],  # (1)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
## ApiResultOutputTypeDef

```python
# ApiResultOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ApiResultOutputTypeDef


def get_value() -> ApiResultOutputTypeDef:
    return {
        "actionGroup": ...,
    }


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
# ApiResultTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ApiResultTypeDef


def get_value() -> ApiResultTypeDef:
    return {
        "actionGroup": ...,
    }


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
# FunctionResultOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FunctionResultOutputTypeDef


def get_value() -> FunctionResultOutputTypeDef:
    return {
        "actionGroup": ...,
    }


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
# FunctionResultTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FunctionResultTypeDef


def get_value() -> FunctionResultTypeDef:
    return {
        "actionGroup": ...,
    }


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
## BedrockModelConfigurationsTypeDef

```python
# BedrockModelConfigurationsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import BedrockModelConfigurationsTypeDef


def get_value() -> BedrockModelConfigurationsTypeDef:
    return {
        "performanceConfig": ...,
    }


# BedrockModelConfigurationsTypeDef definition

class BedrockModelConfigurationsTypeDef(TypedDict):
    performanceConfig: NotRequired[PerformanceConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: PerformanceConfigurationTypeDef](./type_defs.md#performanceconfigurationtypedef) 
## InlineBedrockModelConfigurationsTypeDef

```python
# InlineBedrockModelConfigurationsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InlineBedrockModelConfigurationsTypeDef


def get_value() -> InlineBedrockModelConfigurationsTypeDef:
    return {
        "performanceConfig": ...,
    }


# InlineBedrockModelConfigurationsTypeDef definition

class InlineBedrockModelConfigurationsTypeDef(TypedDict):
    performanceConfig: NotRequired[PerformanceConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: PerformanceConfigurationTypeDef](./type_defs.md#performanceconfigurationtypedef) 
## ModelPerformanceConfigurationTypeDef

```python
# ModelPerformanceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ModelPerformanceConfigurationTypeDef


def get_value() -> ModelPerformanceConfigurationTypeDef:
    return {
        "performanceConfig": ...,
    }


# ModelPerformanceConfigurationTypeDef definition

class ModelPerformanceConfigurationTypeDef(TypedDict):
    performanceConfig: NotRequired[PerformanceConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: PerformanceConfigurationTypeDef](./type_defs.md#performanceconfigurationtypedef) 
## BedrockRerankingConfigurationTypeDef

```python
# BedrockRerankingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import BedrockRerankingConfigurationTypeDef


def get_value() -> BedrockRerankingConfigurationTypeDef:
    return {
        "modelConfiguration": ...,
    }


# BedrockRerankingConfigurationTypeDef definition

class BedrockRerankingConfigurationTypeDef(TypedDict):
    modelConfiguration: BedrockRerankingModelConfigurationTypeDef,  # (1)
    numberOfResults: NotRequired[int],
```

1. See [:material-code-braces: BedrockRerankingModelConfigurationTypeDef](./type_defs.md#bedrockrerankingmodelconfigurationtypedef) 
## ByteContentDocTypeDef

```python
# ByteContentDocTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ByteContentDocTypeDef


def get_value() -> ByteContentDocTypeDef:
    return {
        "contentType": ...,
    }


# ByteContentDocTypeDef definition

class ByteContentDocTypeDef(TypedDict):
    contentType: str,
    data: BlobTypeDef,
    identifier: str,
```

## ByteContentFileTypeDef

```python
# ByteContentFileTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ByteContentFileTypeDef


def get_value() -> ByteContentFileTypeDef:
    return {
        "data": ...,
    }


# ByteContentFileTypeDef definition

class ByteContentFileTypeDef(TypedDict):
    data: BlobTypeDef,
    mediaType: str,
```

## MessageTypeDef

```python
# MessageTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import MessageTypeDef


def get_value() -> MessageTypeDef:
    return {
        "content": ...,
    }


# MessageTypeDef definition

class MessageTypeDef(TypedDict):
    content: Sequence[ContentBlockTypeDef],  # (1)
    role: ConversationRoleType,  # (2)
```

1. See [:material-code-braces: ContentBlockTypeDef](./type_defs.md#contentblocktypedef) 
2. See [:material-code-brackets: ConversationRoleType](./literals.md#conversationroletype) 
## CustomOrchestrationTraceTypeDef

```python
# CustomOrchestrationTraceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import CustomOrchestrationTraceTypeDef


def get_value() -> CustomOrchestrationTraceTypeDef:
    return {
        "event": ...,
    }


# CustomOrchestrationTraceTypeDef definition

class CustomOrchestrationTraceTypeDef(TypedDict):
    event: NotRequired[CustomOrchestrationTraceEventTypeDef],  # (1)
    traceId: NotRequired[str],
```

1. See [:material-code-braces: CustomOrchestrationTraceEventTypeDef](./type_defs.md#customorchestrationtraceeventtypedef) 
## RerankingMetadataSelectiveModeConfigurationTypeDef

```python
# RerankingMetadataSelectiveModeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RerankingMetadataSelectiveModeConfigurationTypeDef


def get_value() -> RerankingMetadataSelectiveModeConfigurationTypeDef:
    return {
        "fieldsToExclude": ...,
    }


# RerankingMetadataSelectiveModeConfigurationTypeDef definition

class RerankingMetadataSelectiveModeConfigurationTypeDef(TypedDict):
    fieldsToExclude: NotRequired[Sequence[FieldForRerankingTypeDef]],  # (1)
    fieldsToInclude: NotRequired[Sequence[FieldForRerankingTypeDef]],  # (1)
```

1. See [:material-code-braces: FieldForRerankingTypeDef](./type_defs.md#fieldforrerankingtypedef) 
2. See [:material-code-braces: FieldForRerankingTypeDef](./type_defs.md#fieldforrerankingtypedef) 
## FilePartTypeDef

```python
# FilePartTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FilePartTypeDef


def get_value() -> FilePartTypeDef:
    return {
        "files": ...,
    }


# FilePartTypeDef definition

class FilePartTypeDef(TypedDict):
    files: NotRequired[List[OutputFileTypeDef]],  # (1)
```

1. See [:material-code-braces: OutputFileTypeDef](./type_defs.md#outputfiletypedef) 
## InlineAgentFilePartTypeDef

```python
# InlineAgentFilePartTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InlineAgentFilePartTypeDef


def get_value() -> InlineAgentFilePartTypeDef:
    return {
        "files": ...,
    }


# InlineAgentFilePartTypeDef definition

class InlineAgentFilePartTypeDef(TypedDict):
    files: NotRequired[List[OutputFileTypeDef]],  # (1)
```

1. See [:material-code-braces: OutputFileTypeDef](./type_defs.md#outputfiletypedef) 
## RetrievalFilterPaginatorTypeDef

```python
# RetrievalFilterPaginatorTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrievalFilterPaginatorTypeDef


def get_value() -> RetrievalFilterPaginatorTypeDef:
    return {
        "andAll": ...,
    }


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
# RetrievalFilterTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrievalFilterTypeDef


def get_value() -> RetrievalFilterTypeDef:
    return {
        "andAll": ...,
    }


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
# FlowInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FlowInputTypeDef


def get_value() -> FlowInputTypeDef:
    return {
        "content": ...,
    }


# FlowInputTypeDef definition

class FlowInputTypeDef(TypedDict):
    content: FlowInputContentTypeDef,  # (1)
    nodeName: str,
    nodeInputName: NotRequired[str],
    nodeOutputName: NotRequired[str],
```

1. See [:material-code-braces: FlowInputContentTypeDef](./type_defs.md#flowinputcontenttypedef) 
## FlowMultiTurnInputRequestEventTypeDef

```python
# FlowMultiTurnInputRequestEventTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FlowMultiTurnInputRequestEventTypeDef


def get_value() -> FlowMultiTurnInputRequestEventTypeDef:
    return {
        "content": ...,
    }


# FlowMultiTurnInputRequestEventTypeDef definition

class FlowMultiTurnInputRequestEventTypeDef(TypedDict):
    content: FlowMultiTurnInputContentTypeDef,  # (1)
    nodeName: str,
    nodeType: NodeTypeType,  # (2)
```

1. See [:material-code-braces: FlowMultiTurnInputContentTypeDef](./type_defs.md#flowmultiturninputcontenttypedef) 
2. See [:material-code-brackets: NodeTypeType](./literals.md#nodetypetype) 
## FlowOutputEventTypeDef

```python
# FlowOutputEventTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FlowOutputEventTypeDef


def get_value() -> FlowOutputEventTypeDef:
    return {
        "content": ...,
    }


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
# FlowTraceConditionNodeResultEventTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FlowTraceConditionNodeResultEventTypeDef


def get_value() -> FlowTraceConditionNodeResultEventTypeDef:
    return {
        "nodeName": ...,
    }


# FlowTraceConditionNodeResultEventTypeDef definition

class FlowTraceConditionNodeResultEventTypeDef(TypedDict):
    nodeName: str,
    satisfiedConditions: List[FlowTraceConditionTypeDef],  # (1)
    timestamp: datetime,
```

1. See [:material-code-braces: FlowTraceConditionTypeDef](./type_defs.md#flowtraceconditiontypedef) 
## FlowTraceNodeInputFieldTypeDef

```python
# FlowTraceNodeInputFieldTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FlowTraceNodeInputFieldTypeDef


def get_value() -> FlowTraceNodeInputFieldTypeDef:
    return {
        "content": ...,
    }


# FlowTraceNodeInputFieldTypeDef definition

class FlowTraceNodeInputFieldTypeDef(TypedDict):
    content: FlowTraceNodeInputContentTypeDef,  # (1)
    nodeInputName: str,
```

1. See [:material-code-braces: FlowTraceNodeInputContentTypeDef](./type_defs.md#flowtracenodeinputcontenttypedef) 
## FlowTraceNodeOutputFieldTypeDef

```python
# FlowTraceNodeOutputFieldTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FlowTraceNodeOutputFieldTypeDef


def get_value() -> FlowTraceNodeOutputFieldTypeDef:
    return {
        "content": ...,
    }


# FlowTraceNodeOutputFieldTypeDef definition

class FlowTraceNodeOutputFieldTypeDef(TypedDict):
    content: FlowTraceNodeOutputContentTypeDef,  # (1)
    nodeOutputName: str,
```

1. See [:material-code-braces: FlowTraceNodeOutputContentTypeDef](./type_defs.md#flowtracenodeoutputcontenttypedef) 
## FunctionDefinitionTypeDef

```python
# FunctionDefinitionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FunctionDefinitionTypeDef


def get_value() -> FunctionDefinitionTypeDef:
    return {
        "description": ...,
    }


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
# FunctionInvocationInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FunctionInvocationInputTypeDef


def get_value() -> FunctionInvocationInputTypeDef:
    return {
        "actionGroup": ...,
    }


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
# GenerateQueryResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GenerateQueryResponseTypeDef


def get_value() -> GenerateQueryResponseTypeDef:
    return {
        "queries": ...,
    }


# GenerateQueryResponseTypeDef definition

class GenerateQueryResponseTypeDef(TypedDict):
    queries: List[GeneratedQueryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GeneratedQueryTypeDef](./type_defs.md#generatedquerytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAgentMemoryRequestPaginateTypeDef

```python
# GetAgentMemoryRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GetAgentMemoryRequestPaginateTypeDef


def get_value() -> GetAgentMemoryRequestPaginateTypeDef:
    return {
        "agentAliasId": ...,
    }


# GetAgentMemoryRequestPaginateTypeDef definition

class GetAgentMemoryRequestPaginateTypeDef(TypedDict):
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
# GuardrailContentPolicyAssessmentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GuardrailContentPolicyAssessmentTypeDef


def get_value() -> GuardrailContentPolicyAssessmentTypeDef:
    return {
        "filters": ...,
    }


# GuardrailContentPolicyAssessmentTypeDef definition

class GuardrailContentPolicyAssessmentTypeDef(TypedDict):
    filters: NotRequired[List[GuardrailContentFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: GuardrailContentFilterTypeDef](./type_defs.md#guardrailcontentfiltertypedef) 
## GuardrailWordPolicyAssessmentTypeDef

```python
# GuardrailWordPolicyAssessmentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GuardrailWordPolicyAssessmentTypeDef


def get_value() -> GuardrailWordPolicyAssessmentTypeDef:
    return {
        "customWords": ...,
    }


# GuardrailWordPolicyAssessmentTypeDef definition

class GuardrailWordPolicyAssessmentTypeDef(TypedDict):
    customWords: NotRequired[List[GuardrailCustomWordTypeDef]],  # (1)
    managedWordLists: NotRequired[List[GuardrailManagedWordTypeDef]],  # (2)
```

1. See [:material-code-braces: GuardrailCustomWordTypeDef](./type_defs.md#guardrailcustomwordtypedef) 
2. See [:material-code-braces: GuardrailManagedWordTypeDef](./type_defs.md#guardrailmanagedwordtypedef) 
## GuardrailSensitiveInformationPolicyAssessmentTypeDef

```python
# GuardrailSensitiveInformationPolicyAssessmentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GuardrailSensitiveInformationPolicyAssessmentTypeDef


def get_value() -> GuardrailSensitiveInformationPolicyAssessmentTypeDef:
    return {
        "piiEntities": ...,
    }


# GuardrailSensitiveInformationPolicyAssessmentTypeDef definition

class GuardrailSensitiveInformationPolicyAssessmentTypeDef(TypedDict):
    piiEntities: NotRequired[List[GuardrailPiiEntityFilterTypeDef]],  # (1)
    regexes: NotRequired[List[GuardrailRegexFilterTypeDef]],  # (2)
```

1. See [:material-code-braces: GuardrailPiiEntityFilterTypeDef](./type_defs.md#guardrailpiientityfiltertypedef) 
2. See [:material-code-braces: GuardrailRegexFilterTypeDef](./type_defs.md#guardrailregexfiltertypedef) 
## GuardrailTopicPolicyAssessmentTypeDef

```python
# GuardrailTopicPolicyAssessmentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GuardrailTopicPolicyAssessmentTypeDef


def get_value() -> GuardrailTopicPolicyAssessmentTypeDef:
    return {
        "topics": ...,
    }


# GuardrailTopicPolicyAssessmentTypeDef definition

class GuardrailTopicPolicyAssessmentTypeDef(TypedDict):
    topics: NotRequired[List[GuardrailTopicTypeDef]],  # (1)
```

1. See [:material-code-braces: GuardrailTopicTypeDef](./type_defs.md#guardrailtopictypedef) 
## ImplicitFilterConfigurationTypeDef

```python
# ImplicitFilterConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ImplicitFilterConfigurationTypeDef


def get_value() -> ImplicitFilterConfigurationTypeDef:
    return {
        "metadataAttributes": ...,
    }


# ImplicitFilterConfigurationTypeDef definition

class ImplicitFilterConfigurationTypeDef(TypedDict):
    metadataAttributes: Sequence[MetadataAttributeSchemaTypeDef],  # (1)
    modelArn: str,
```

1. See [:material-code-braces: MetadataAttributeSchemaTypeDef](./type_defs.md#metadataattributeschematypedef) 
## InferenceConfigTypeDef

```python
# InferenceConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InferenceConfigTypeDef


def get_value() -> InferenceConfigTypeDef:
    return {
        "textInferenceConfig": ...,
    }


# InferenceConfigTypeDef definition

class InferenceConfigTypeDef(TypedDict):
    textInferenceConfig: NotRequired[TextInferenceConfigTypeDef],  # (1)
```

1. See [:material-code-braces: TextInferenceConfigTypeDef](./type_defs.md#textinferenceconfigtypedef) 
## ModelInvocationInputTypeDef

```python
# ModelInvocationInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ModelInvocationInputTypeDef


def get_value() -> ModelInvocationInputTypeDef:
    return {
        "foundationModel": ...,
    }


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
# InputPromptTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InputPromptTypeDef


def get_value() -> InputPromptTypeDef:
    return {
        "textPrompt": ...,
    }


# InputPromptTypeDef definition

class InputPromptTypeDef(TypedDict):
    textPrompt: NotRequired[TextPromptTypeDef],  # (1)
```

1. See [:material-code-braces: TextPromptTypeDef](./type_defs.md#textprompttypedef) 
## OptimizedPromptTypeDef

```python
# OptimizedPromptTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import OptimizedPromptTypeDef


def get_value() -> OptimizedPromptTypeDef:
    return {
        "textPrompt": ...,
    }


# OptimizedPromptTypeDef definition

class OptimizedPromptTypeDef(TypedDict):
    textPrompt: NotRequired[TextPromptTypeDef],  # (1)
```

1. See [:material-code-braces: TextPromptTypeDef](./type_defs.md#textprompttypedef) 
## MemoryTypeDef

```python
# MemoryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import MemoryTypeDef


def get_value() -> MemoryTypeDef:
    return {
        "sessionSummary": ...,
    }


# MemoryTypeDef definition

class MemoryTypeDef(TypedDict):
    sessionSummary: NotRequired[MemorySessionSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: MemorySessionSummaryTypeDef](./type_defs.md#memorysessionsummarytypedef) 
## MetadataTypeDef

```python
# MetadataTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import MetadataTypeDef


def get_value() -> MetadataTypeDef:
    return {
        "usage": ...,
    }


# MetadataTypeDef definition

class MetadataTypeDef(TypedDict):
    usage: NotRequired[UsageTypeDef],  # (1)
```

1. See [:material-code-braces: UsageTypeDef](./type_defs.md#usagetypedef) 
## RerankDocumentOutputTypeDef

```python
# RerankDocumentOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RerankDocumentOutputTypeDef


def get_value() -> RerankDocumentOutputTypeDef:
    return {
        "jsonDocument": ...,
    }


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
# RerankDocumentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RerankDocumentTypeDef


def get_value() -> RerankDocumentTypeDef:
    return {
        "jsonDocument": ...,
    }


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
# RerankQueryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RerankQueryTypeDef


def get_value() -> RerankQueryTypeDef:
    return {
        "textQuery": ...,
    }


# RerankQueryTypeDef definition

class RerankQueryTypeDef(TypedDict):
    textQuery: RerankTextDocumentTypeDef,  # (1)
    type: RerankQueryContentTypeType,  # (2)
```

1. See [:material-code-braces: RerankTextDocumentTypeDef](./type_defs.md#reranktextdocumenttypedef) 
2. See [:material-code-brackets: RerankQueryContentTypeType](./literals.md#rerankquerycontenttypetype) 
## RetrievalResultContentTypeDef

```python
# RetrievalResultContentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrievalResultContentTypeDef


def get_value() -> RetrievalResultContentTypeDef:
    return {
        "byteContent": ...,
    }


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
# RetrievalResultLocationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrievalResultLocationTypeDef


def get_value() -> RetrievalResultLocationTypeDef:
    return {
        "confluenceLocation": ...,
    }


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
# TextResponsePartTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import TextResponsePartTypeDef


def get_value() -> TextResponsePartTypeDef:
    return {
        "span": ...,
    }


# TextResponsePartTypeDef definition

class TextResponsePartTypeDef(TypedDict):
    span: NotRequired[SpanTypeDef],  # (1)
    text: NotRequired[str],
```

1. See [:material-code-braces: SpanTypeDef](./type_defs.md#spantypedef) 
## TextToSqlConfigurationTypeDef

```python
# TextToSqlConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import TextToSqlConfigurationTypeDef


def get_value() -> TextToSqlConfigurationTypeDef:
    return {
        "knowledgeBaseConfiguration": ...,
    }


# TextToSqlConfigurationTypeDef definition

class TextToSqlConfigurationTypeDef(TypedDict):
    type: TextToSqlConfigurationTypeType,  # (2)
    knowledgeBaseConfiguration: NotRequired[TextToSqlKnowledgeBaseConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: TextToSqlKnowledgeBaseConfigurationTypeDef](./type_defs.md#texttosqlknowledgebaseconfigurationtypedef) 
2. See [:material-code-brackets: TextToSqlConfigurationTypeType](./literals.md#texttosqlconfigurationtypetype) 
## ApiRequestBodyTypeDef

```python
# ApiRequestBodyTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ApiRequestBodyTypeDef


def get_value() -> ApiRequestBodyTypeDef:
    return {
        "content": ...,
    }


# ApiRequestBodyTypeDef definition

class ApiRequestBodyTypeDef(TypedDict):
    content: NotRequired[Dict[str, PropertyParametersTypeDef]],  # (1)
```

1. See [:material-code-braces: PropertyParametersTypeDef](./type_defs.md#propertyparameterstypedef) 
## ActionGroupInvocationInputTypeDef

```python
# ActionGroupInvocationInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ActionGroupInvocationInputTypeDef


def get_value() -> ActionGroupInvocationInputTypeDef:
    return {
        "actionGroupName": ...,
    }


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
# InvocationResultMemberOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InvocationResultMemberOutputTypeDef


def get_value() -> InvocationResultMemberOutputTypeDef:
    return {
        "apiResult": ...,
    }


# InvocationResultMemberOutputTypeDef definition

class InvocationResultMemberOutputTypeDef(TypedDict):
    apiResult: NotRequired[ApiResultOutputTypeDef],  # (1)
    functionResult: NotRequired[FunctionResultOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ApiResultOutputTypeDef](./type_defs.md#apiresultoutputtypedef) 
2. See [:material-code-braces: FunctionResultOutputTypeDef](./type_defs.md#functionresultoutputtypedef) 
## RerankingConfigurationTypeDef

```python
# RerankingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RerankingConfigurationTypeDef


def get_value() -> RerankingConfigurationTypeDef:
    return {
        "bedrockRerankingConfiguration": ...,
    }


# RerankingConfigurationTypeDef definition

class RerankingConfigurationTypeDef(TypedDict):
    bedrockRerankingConfiguration: BedrockRerankingConfigurationTypeDef,  # (1)
    type: RerankingConfigurationTypeType,  # (2)
```

1. See [:material-code-braces: BedrockRerankingConfigurationTypeDef](./type_defs.md#bedrockrerankingconfigurationtypedef) 
2. See [:material-code-brackets: RerankingConfigurationTypeType](./literals.md#rerankingconfigurationtypetype) 
## ExternalSourceTypeDef

```python
# ExternalSourceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ExternalSourceTypeDef


def get_value() -> ExternalSourceTypeDef:
    return {
        "byteContent": ...,
    }


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
# FileSourceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FileSourceTypeDef


def get_value() -> FileSourceTypeDef:
    return {
        "byteContent": ...,
    }


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
# ConversationHistoryTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ConversationHistoryTypeDef


def get_value() -> ConversationHistoryTypeDef:
    return {
        "messages": ...,
    }


# ConversationHistoryTypeDef definition

class ConversationHistoryTypeDef(TypedDict):
    messages: NotRequired[Sequence[MessageTypeDef]],  # (1)
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
## MetadataConfigurationForRerankingTypeDef

```python
# MetadataConfigurationForRerankingTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import MetadataConfigurationForRerankingTypeDef


def get_value() -> MetadataConfigurationForRerankingTypeDef:
    return {
        "selectionMode": ...,
    }


# MetadataConfigurationForRerankingTypeDef definition

class MetadataConfigurationForRerankingTypeDef(TypedDict):
    selectionMode: RerankingMetadataSelectionModeType,  # (1)
    selectiveModeConfiguration: NotRequired[RerankingMetadataSelectiveModeConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: RerankingMetadataSelectionModeType](./literals.md#rerankingmetadataselectionmodetype) 
2. See [:material-code-braces: RerankingMetadataSelectiveModeConfigurationTypeDef](./type_defs.md#rerankingmetadataselectivemodeconfigurationtypedef) 
## InvokeFlowRequestTypeDef

```python
# InvokeFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InvokeFlowRequestTypeDef


def get_value() -> InvokeFlowRequestTypeDef:
    return {
        "flowAliasIdentifier": ...,
    }


# InvokeFlowRequestTypeDef definition

class InvokeFlowRequestTypeDef(TypedDict):
    flowAliasIdentifier: str,
    flowIdentifier: str,
    inputs: Sequence[FlowInputTypeDef],  # (1)
    enableTrace: NotRequired[bool],
    executionId: NotRequired[str],
    modelPerformanceConfiguration: NotRequired[ModelPerformanceConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: FlowInputTypeDef](./type_defs.md#flowinputtypedef) 
2. See [:material-code-braces: ModelPerformanceConfigurationTypeDef](./type_defs.md#modelperformanceconfigurationtypedef) 
## FlowTraceNodeInputEventTypeDef

```python
# FlowTraceNodeInputEventTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FlowTraceNodeInputEventTypeDef


def get_value() -> FlowTraceNodeInputEventTypeDef:
    return {
        "fields": ...,
    }


# FlowTraceNodeInputEventTypeDef definition

class FlowTraceNodeInputEventTypeDef(TypedDict):
    fields: List[FlowTraceNodeInputFieldTypeDef],  # (1)
    nodeName: str,
    timestamp: datetime,
```

1. See [:material-code-braces: FlowTraceNodeInputFieldTypeDef](./type_defs.md#flowtracenodeinputfieldtypedef) 
## FlowTraceNodeOutputEventTypeDef

```python
# FlowTraceNodeOutputEventTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FlowTraceNodeOutputEventTypeDef


def get_value() -> FlowTraceNodeOutputEventTypeDef:
    return {
        "fields": ...,
    }


# FlowTraceNodeOutputEventTypeDef definition

class FlowTraceNodeOutputEventTypeDef(TypedDict):
    fields: List[FlowTraceNodeOutputFieldTypeDef],  # (1)
    nodeName: str,
    timestamp: datetime,
```

1. See [:material-code-braces: FlowTraceNodeOutputFieldTypeDef](./type_defs.md#flowtracenodeoutputfieldtypedef) 
## FunctionSchemaTypeDef

```python
# FunctionSchemaTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FunctionSchemaTypeDef


def get_value() -> FunctionSchemaTypeDef:
    return {
        "functions": ...,
    }


# FunctionSchemaTypeDef definition

class FunctionSchemaTypeDef(TypedDict):
    functions: NotRequired[Sequence[FunctionDefinitionTypeDef]],  # (1)
```

1. See [:material-code-braces: FunctionDefinitionTypeDef](./type_defs.md#functiondefinitiontypedef) 
## GuardrailAssessmentTypeDef

```python
# GuardrailAssessmentTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GuardrailAssessmentTypeDef


def get_value() -> GuardrailAssessmentTypeDef:
    return {
        "contentPolicy": ...,
    }


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
# ExternalSourcesGenerationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ExternalSourcesGenerationConfigurationTypeDef


def get_value() -> ExternalSourcesGenerationConfigurationTypeDef:
    return {
        "additionalModelRequestFields": ...,
    }


# ExternalSourcesGenerationConfigurationTypeDef definition

class ExternalSourcesGenerationConfigurationTypeDef(TypedDict):
    additionalModelRequestFields: NotRequired[Mapping[str, Mapping[str, Any]]],
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (1)
    inferenceConfig: NotRequired[InferenceConfigTypeDef],  # (2)
    performanceConfig: NotRequired[PerformanceConfigurationTypeDef],  # (3)
    promptTemplate: NotRequired[PromptTemplateTypeDef],  # (4)
```

1. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
2. See [:material-code-braces: InferenceConfigTypeDef](./type_defs.md#inferenceconfigtypedef) 
3. See [:material-code-braces: PerformanceConfigurationTypeDef](./type_defs.md#performanceconfigurationtypedef) 
4. See [:material-code-braces: PromptTemplateTypeDef](./type_defs.md#prompttemplatetypedef) 
## GenerationConfigurationTypeDef

```python
# GenerationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GenerationConfigurationTypeDef


def get_value() -> GenerationConfigurationTypeDef:
    return {
        "additionalModelRequestFields": ...,
    }


# GenerationConfigurationTypeDef definition

class GenerationConfigurationTypeDef(TypedDict):
    additionalModelRequestFields: NotRequired[Mapping[str, Mapping[str, Any]]],
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (1)
    inferenceConfig: NotRequired[InferenceConfigTypeDef],  # (2)
    performanceConfig: NotRequired[PerformanceConfigurationTypeDef],  # (3)
    promptTemplate: NotRequired[PromptTemplateTypeDef],  # (4)
```

1. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
2. See [:material-code-braces: InferenceConfigTypeDef](./type_defs.md#inferenceconfigtypedef) 
3. See [:material-code-braces: PerformanceConfigurationTypeDef](./type_defs.md#performanceconfigurationtypedef) 
4. See [:material-code-braces: PromptTemplateTypeDef](./type_defs.md#prompttemplatetypedef) 
## OrchestrationConfigurationTypeDef

```python
# OrchestrationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import OrchestrationConfigurationTypeDef


def get_value() -> OrchestrationConfigurationTypeDef:
    return {
        "additionalModelRequestFields": ...,
    }


# OrchestrationConfigurationTypeDef definition

class OrchestrationConfigurationTypeDef(TypedDict):
    additionalModelRequestFields: NotRequired[Mapping[str, Mapping[str, Any]]],
    inferenceConfig: NotRequired[InferenceConfigTypeDef],  # (1)
    performanceConfig: NotRequired[PerformanceConfigurationTypeDef],  # (2)
    promptTemplate: NotRequired[PromptTemplateTypeDef],  # (3)
    queryTransformationConfiguration: NotRequired[QueryTransformationConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: InferenceConfigTypeDef](./type_defs.md#inferenceconfigtypedef) 
2. See [:material-code-braces: PerformanceConfigurationTypeDef](./type_defs.md#performanceconfigurationtypedef) 
3. See [:material-code-braces: PromptTemplateTypeDef](./type_defs.md#prompttemplatetypedef) 
4. See [:material-code-braces: QueryTransformationConfigurationTypeDef](./type_defs.md#querytransformationconfigurationtypedef) 
## PromptConfigurationTypeDef

```python
# PromptConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import PromptConfigurationTypeDef


def get_value() -> PromptConfigurationTypeDef:
    return {
        "additionalModelRequestFields": ...,
    }


# PromptConfigurationTypeDef definition

class PromptConfigurationTypeDef(TypedDict):
    additionalModelRequestFields: NotRequired[Mapping[str, Any]],
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
## OptimizePromptRequestTypeDef

```python
# OptimizePromptRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import OptimizePromptRequestTypeDef


def get_value() -> OptimizePromptRequestTypeDef:
    return {
        "input": ...,
    }


# OptimizePromptRequestTypeDef definition

class OptimizePromptRequestTypeDef(TypedDict):
    input: InputPromptTypeDef,  # (1)
    targetModelId: str,
```

1. See [:material-code-braces: InputPromptTypeDef](./type_defs.md#inputprompttypedef) 
## OptimizedPromptEventTypeDef

```python
# OptimizedPromptEventTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import OptimizedPromptEventTypeDef


def get_value() -> OptimizedPromptEventTypeDef:
    return {
        "optimizedPrompt": ...,
    }


# OptimizedPromptEventTypeDef definition

class OptimizedPromptEventTypeDef(TypedDict):
    optimizedPrompt: NotRequired[OptimizedPromptTypeDef],  # (1)
```

1. See [:material-code-braces: OptimizedPromptTypeDef](./type_defs.md#optimizedprompttypedef) 
## GetAgentMemoryResponseTypeDef

```python
# GetAgentMemoryResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GetAgentMemoryResponseTypeDef


def get_value() -> GetAgentMemoryResponseTypeDef:
    return {
        "memoryContents": ...,
    }


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
# OrchestrationModelInvocationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import OrchestrationModelInvocationOutputTypeDef


def get_value() -> OrchestrationModelInvocationOutputTypeDef:
    return {
        "metadata": ...,
    }


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
# PostProcessingModelInvocationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import PostProcessingModelInvocationOutputTypeDef


def get_value() -> PostProcessingModelInvocationOutputTypeDef:
    return {
        "metadata": ...,
    }


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
# PreProcessingModelInvocationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import PreProcessingModelInvocationOutputTypeDef


def get_value() -> PreProcessingModelInvocationOutputTypeDef:
    return {
        "metadata": ...,
    }


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
# RoutingClassifierModelInvocationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RoutingClassifierModelInvocationOutputTypeDef


def get_value() -> RoutingClassifierModelInvocationOutputTypeDef:
    return {
        "metadata": ...,
    }


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
# RerankResultTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RerankResultTypeDef


def get_value() -> RerankResultTypeDef:
    return {
        "document": ...,
    }


# RerankResultTypeDef definition

class RerankResultTypeDef(TypedDict):
    index: int,
    relevanceScore: float,
    document: NotRequired[RerankDocumentOutputTypeDef],  # (1)
```

1. See [:material-code-braces: RerankDocumentOutputTypeDef](./type_defs.md#rerankdocumentoutputtypedef) 
## KnowledgeBaseRetrievalResultTypeDef

```python
# KnowledgeBaseRetrievalResultTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import KnowledgeBaseRetrievalResultTypeDef


def get_value() -> KnowledgeBaseRetrievalResultTypeDef:
    return {
        "content": ...,
    }


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
# RetrievedReferenceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrievedReferenceTypeDef


def get_value() -> RetrievedReferenceTypeDef:
    return {
        "content": ...,
    }


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
# GeneratedResponsePartTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GeneratedResponsePartTypeDef


def get_value() -> GeneratedResponsePartTypeDef:
    return {
        "textResponsePart": ...,
    }


# GeneratedResponsePartTypeDef definition

class GeneratedResponsePartTypeDef(TypedDict):
    textResponsePart: NotRequired[TextResponsePartTypeDef],  # (1)
```

1. See [:material-code-braces: TextResponsePartTypeDef](./type_defs.md#textresponseparttypedef) 
## TransformationConfigurationTypeDef

```python
# TransformationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import TransformationConfigurationTypeDef


def get_value() -> TransformationConfigurationTypeDef:
    return {
        "mode": ...,
    }


# TransformationConfigurationTypeDef definition

class TransformationConfigurationTypeDef(TypedDict):
    mode: QueryTransformationModeType,  # (1)
    textToSqlConfiguration: NotRequired[TextToSqlConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: QueryTransformationModeType](./literals.md#querytransformationmodetype) 
2. See [:material-code-braces: TextToSqlConfigurationTypeDef](./type_defs.md#texttosqlconfigurationtypedef) 
## ApiInvocationInputTypeDef

```python
# ApiInvocationInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ApiInvocationInputTypeDef


def get_value() -> ApiInvocationInputTypeDef:
    return {
        "actionGroup": ...,
    }


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
# ReturnControlResultsTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ReturnControlResultsTypeDef


def get_value() -> ReturnControlResultsTypeDef:
    return {
        "invocationId": ...,
    }


# ReturnControlResultsTypeDef definition

class ReturnControlResultsTypeDef(TypedDict):
    invocationId: NotRequired[str],
    returnControlInvocationResults: NotRequired[List[InvocationResultMemberOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: InvocationResultMemberOutputTypeDef](./type_defs.md#invocationresultmemberoutputtypedef) 
## InvocationResultMemberTypeDef

```python
# InvocationResultMemberTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InvocationResultMemberTypeDef


def get_value() -> InvocationResultMemberTypeDef:
    return {
        "apiResult": ...,
    }


# InvocationResultMemberTypeDef definition

class InvocationResultMemberTypeDef(TypedDict):
    apiResult: NotRequired[ApiResultUnionTypeDef],  # (1)
    functionResult: NotRequired[FunctionResultUnionTypeDef],  # (2)
```

1. See [:material-code-braces: ApiResultTypeDef](./type_defs.md#apiresulttypedef) [:material-code-braces: ApiResultOutputTypeDef](./type_defs.md#apiresultoutputtypedef) 
2. See [:material-code-braces: FunctionResultTypeDef](./type_defs.md#functionresulttypedef) [:material-code-braces: FunctionResultOutputTypeDef](./type_defs.md#functionresultoutputtypedef) 
## InputFileTypeDef

```python
# InputFileTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InputFileTypeDef


def get_value() -> InputFileTypeDef:
    return {
        "name": ...,
    }


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
# VectorSearchBedrockRerankingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import VectorSearchBedrockRerankingConfigurationTypeDef


def get_value() -> VectorSearchBedrockRerankingConfigurationTypeDef:
    return {
        "metadataConfiguration": ...,
    }


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
# FlowTraceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FlowTraceTypeDef


def get_value() -> FlowTraceTypeDef:
    return {
        "conditionNodeResultTrace": ...,
    }


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
# AgentActionGroupTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import AgentActionGroupTypeDef


def get_value() -> AgentActionGroupTypeDef:
    return {
        "actionGroupExecutor": ...,
    }


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
# GuardrailTraceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GuardrailTraceTypeDef


def get_value() -> GuardrailTraceTypeDef:
    return {
        "action": ...,
    }


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
# ExternalSourcesRetrieveAndGenerateConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ExternalSourcesRetrieveAndGenerateConfigurationTypeDef


def get_value() -> ExternalSourcesRetrieveAndGenerateConfigurationTypeDef:
    return {
        "generationConfiguration": ...,
    }


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
# PromptOverrideConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import PromptOverrideConfigurationTypeDef


def get_value() -> PromptOverrideConfigurationTypeDef:
    return {
        "overrideLambda": ...,
    }


# PromptOverrideConfigurationTypeDef definition

class PromptOverrideConfigurationTypeDef(TypedDict):
    promptConfigurations: Sequence[PromptConfigurationTypeDef],  # (1)
    overrideLambda: NotRequired[str],
```

1. See [:material-code-braces: PromptConfigurationTypeDef](./type_defs.md#promptconfigurationtypedef) 
## OptimizedPromptStreamTypeDef

```python
# OptimizedPromptStreamTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import OptimizedPromptStreamTypeDef


def get_value() -> OptimizedPromptStreamTypeDef:
    return {
        "accessDeniedException": ...,
    }


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
# PostProcessingTraceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import PostProcessingTraceTypeDef


def get_value() -> PostProcessingTraceTypeDef:
    return {
        "modelInvocationInput": ...,
    }


# PostProcessingTraceTypeDef definition

class PostProcessingTraceTypeDef(TypedDict):
    modelInvocationInput: NotRequired[ModelInvocationInputTypeDef],  # (1)
    modelInvocationOutput: NotRequired[PostProcessingModelInvocationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ModelInvocationInputTypeDef](./type_defs.md#modelinvocationinputtypedef) 
2. See [:material-code-braces: PostProcessingModelInvocationOutputTypeDef](./type_defs.md#postprocessingmodelinvocationoutputtypedef) 
## PreProcessingTraceTypeDef

```python
# PreProcessingTraceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import PreProcessingTraceTypeDef


def get_value() -> PreProcessingTraceTypeDef:
    return {
        "modelInvocationInput": ...,
    }


# PreProcessingTraceTypeDef definition

class PreProcessingTraceTypeDef(TypedDict):
    modelInvocationInput: NotRequired[ModelInvocationInputTypeDef],  # (1)
    modelInvocationOutput: NotRequired[PreProcessingModelInvocationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ModelInvocationInputTypeDef](./type_defs.md#modelinvocationinputtypedef) 
2. See [:material-code-braces: PreProcessingModelInvocationOutputTypeDef](./type_defs.md#preprocessingmodelinvocationoutputtypedef) 
## RerankResponseTypeDef

```python
# RerankResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RerankResponseTypeDef


def get_value() -> RerankResponseTypeDef:
    return {
        "nextToken": ...,
    }


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
# RerankSourceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RerankSourceTypeDef


def get_value() -> RerankSourceTypeDef:
    return {
        "inlineDocumentSource": ...,
    }


# RerankSourceTypeDef definition

class RerankSourceTypeDef(TypedDict):
    inlineDocumentSource: RerankDocumentUnionTypeDef,  # (1)
    type: RerankSourceTypeType,  # (2)
```

1. See [:material-code-braces: RerankDocumentTypeDef](./type_defs.md#rerankdocumenttypedef) [:material-code-braces: RerankDocumentOutputTypeDef](./type_defs.md#rerankdocumentoutputtypedef) 
2. See [:material-code-brackets: RerankSourceTypeType](./literals.md#reranksourcetypetype) 
## RetrieveResponseTypeDef

```python
# RetrieveResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrieveResponseTypeDef


def get_value() -> RetrieveResponseTypeDef:
    return {
        "guardrailAction": ...,
    }


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
# KnowledgeBaseLookupOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import KnowledgeBaseLookupOutputTypeDef


def get_value() -> KnowledgeBaseLookupOutputTypeDef:
    return {
        "retrievedReferences": ...,
    }


# KnowledgeBaseLookupOutputTypeDef definition

class KnowledgeBaseLookupOutputTypeDef(TypedDict):
    retrievedReferences: NotRequired[List[RetrievedReferenceTypeDef]],  # (1)
```

1. See [:material-code-braces: RetrievedReferenceTypeDef](./type_defs.md#retrievedreferencetypedef) 
## CitationTypeDef

```python
# CitationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import CitationTypeDef


def get_value() -> CitationTypeDef:
    return {
        "generatedResponsePart": ...,
    }


# CitationTypeDef definition

class CitationTypeDef(TypedDict):
    generatedResponsePart: NotRequired[GeneratedResponsePartTypeDef],  # (1)
    retrievedReferences: NotRequired[List[RetrievedReferenceTypeDef]],  # (2)
```

1. See [:material-code-braces: GeneratedResponsePartTypeDef](./type_defs.md#generatedresponseparttypedef) 
2. See [:material-code-braces: RetrievedReferenceTypeDef](./type_defs.md#retrievedreferencetypedef) 
## GenerateQueryRequestTypeDef

```python
# GenerateQueryRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import GenerateQueryRequestTypeDef


def get_value() -> GenerateQueryRequestTypeDef:
    return {
        "queryGenerationInput": ...,
    }


# GenerateQueryRequestTypeDef definition

class GenerateQueryRequestTypeDef(TypedDict):
    queryGenerationInput: QueryGenerationInputTypeDef,  # (1)
    transformationConfiguration: TransformationConfigurationTypeDef,  # (2)
```

1. See [:material-code-braces: QueryGenerationInputTypeDef](./type_defs.md#querygenerationinputtypedef) 
2. See [:material-code-braces: TransformationConfigurationTypeDef](./type_defs.md#transformationconfigurationtypedef) 
## InvocationInputMemberTypeDef

```python
# InvocationInputMemberTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InvocationInputMemberTypeDef


def get_value() -> InvocationInputMemberTypeDef:
    return {
        "apiInvocationInput": ...,
    }


# InvocationInputMemberTypeDef definition

class InvocationInputMemberTypeDef(TypedDict):
    apiInvocationInput: NotRequired[ApiInvocationInputTypeDef],  # (1)
    functionInvocationInput: NotRequired[FunctionInvocationInputTypeDef],  # (2)
```

1. See [:material-code-braces: ApiInvocationInputTypeDef](./type_defs.md#apiinvocationinputtypedef) 
2. See [:material-code-braces: FunctionInvocationInputTypeDef](./type_defs.md#functioninvocationinputtypedef) 
## AgentCollaboratorInputPayloadTypeDef

```python
# AgentCollaboratorInputPayloadTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import AgentCollaboratorInputPayloadTypeDef


def get_value() -> AgentCollaboratorInputPayloadTypeDef:
    return {
        "returnControlResults": ...,
    }


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
# VectorSearchRerankingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import VectorSearchRerankingConfigurationTypeDef


def get_value() -> VectorSearchRerankingConfigurationTypeDef:
    return {
        "bedrockRerankingConfiguration": ...,
    }


# VectorSearchRerankingConfigurationTypeDef definition

class VectorSearchRerankingConfigurationTypeDef(TypedDict):
    type: VectorSearchRerankingConfigurationTypeType,  # (2)
    bedrockRerankingConfiguration: NotRequired[VectorSearchBedrockRerankingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: VectorSearchBedrockRerankingConfigurationTypeDef](./type_defs.md#vectorsearchbedrockrerankingconfigurationtypedef) 
2. See [:material-code-brackets: VectorSearchRerankingConfigurationTypeType](./literals.md#vectorsearchrerankingconfigurationtypetype) 
## FlowTraceEventTypeDef

```python
# FlowTraceEventTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FlowTraceEventTypeDef


def get_value() -> FlowTraceEventTypeDef:
    return {
        "trace": ...,
    }


# FlowTraceEventTypeDef definition

class FlowTraceEventTypeDef(TypedDict):
    trace: FlowTraceTypeDef,  # (1)
```

1. See [:material-code-braces: FlowTraceTypeDef](./type_defs.md#flowtracetypedef) 
## OptimizePromptResponseTypeDef

```python
# OptimizePromptResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import OptimizePromptResponseTypeDef


def get_value() -> OptimizePromptResponseTypeDef:
    return {
        "optimizedPrompt": ...,
    }


# OptimizePromptResponseTypeDef definition

class OptimizePromptResponseTypeDef(TypedDict):
    optimizedPrompt: AioEventStream[OptimizedPromptStreamTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OptimizedPromptStreamTypeDef](./type_defs.md#optimizedpromptstreamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RerankRequestPaginateTypeDef

```python
# RerankRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RerankRequestPaginateTypeDef


def get_value() -> RerankRequestPaginateTypeDef:
    return {
        "queries": ...,
    }


# RerankRequestPaginateTypeDef definition

class RerankRequestPaginateTypeDef(TypedDict):
    queries: Sequence[RerankQueryTypeDef],  # (1)
    rerankingConfiguration: RerankingConfigurationTypeDef,  # (2)
    sources: Sequence[RerankSourceTypeDef],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: RerankQueryTypeDef](./type_defs.md#rerankquerytypedef) 
2. See [:material-code-braces: RerankingConfigurationTypeDef](./type_defs.md#rerankingconfigurationtypedef) 
3. See [:material-code-braces: RerankSourceTypeDef](./type_defs.md#reranksourcetypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## RerankRequestTypeDef

```python
# RerankRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RerankRequestTypeDef


def get_value() -> RerankRequestTypeDef:
    return {
        "queries": ...,
    }


# RerankRequestTypeDef definition

class RerankRequestTypeDef(TypedDict):
    queries: Sequence[RerankQueryTypeDef],  # (1)
    rerankingConfiguration: RerankingConfigurationTypeDef,  # (2)
    sources: Sequence[RerankSourceTypeDef],  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RerankQueryTypeDef](./type_defs.md#rerankquerytypedef) 
2. See [:material-code-braces: RerankingConfigurationTypeDef](./type_defs.md#rerankingconfigurationtypedef) 
3. See [:material-code-braces: RerankSourceTypeDef](./type_defs.md#reranksourcetypedef) 
## AttributionTypeDef

```python
# AttributionTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import AttributionTypeDef


def get_value() -> AttributionTypeDef:
    return {
        "citations": ...,
    }


# AttributionTypeDef definition

class AttributionTypeDef(TypedDict):
    citations: NotRequired[List[CitationTypeDef]],  # (1)
```

1. See [:material-code-braces: CitationTypeDef](./type_defs.md#citationtypedef) 
## CitationEventTypeDef

```python
# CitationEventTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import CitationEventTypeDef


def get_value() -> CitationEventTypeDef:
    return {
        "citation": ...,
    }


# CitationEventTypeDef definition

class CitationEventTypeDef(TypedDict):
    citation: NotRequired[CitationTypeDef],  # (1)
    generatedResponsePart: NotRequired[GeneratedResponsePartTypeDef],  # (2)
    retrievedReferences: NotRequired[List[RetrievedReferenceTypeDef]],  # (3)
```

1. See [:material-code-braces: CitationTypeDef](./type_defs.md#citationtypedef) 
2. See [:material-code-braces: GeneratedResponsePartTypeDef](./type_defs.md#generatedresponseparttypedef) 
3. See [:material-code-braces: RetrievedReferenceTypeDef](./type_defs.md#retrievedreferencetypedef) 
## RetrieveAndGenerateResponseTypeDef

```python
# RetrieveAndGenerateResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrieveAndGenerateResponseTypeDef


def get_value() -> RetrieveAndGenerateResponseTypeDef:
    return {
        "citations": ...,
    }


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
# InlineAgentReturnControlPayloadTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InlineAgentReturnControlPayloadTypeDef


def get_value() -> InlineAgentReturnControlPayloadTypeDef:
    return {
        "invocationId": ...,
    }


# InlineAgentReturnControlPayloadTypeDef definition

class InlineAgentReturnControlPayloadTypeDef(TypedDict):
    invocationId: NotRequired[str],
    invocationInputs: NotRequired[List[InvocationInputMemberTypeDef]],  # (1)
```

1. See [:material-code-braces: InvocationInputMemberTypeDef](./type_defs.md#invocationinputmembertypedef) 
## ReturnControlPayloadTypeDef

```python
# ReturnControlPayloadTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ReturnControlPayloadTypeDef


def get_value() -> ReturnControlPayloadTypeDef:
    return {
        "invocationId": ...,
    }


# ReturnControlPayloadTypeDef definition

class ReturnControlPayloadTypeDef(TypedDict):
    invocationId: NotRequired[str],
    invocationInputs: NotRequired[List[InvocationInputMemberTypeDef]],  # (1)
```

1. See [:material-code-braces: InvocationInputMemberTypeDef](./type_defs.md#invocationinputmembertypedef) 
## AgentCollaboratorInvocationInputTypeDef

```python
# AgentCollaboratorInvocationInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import AgentCollaboratorInvocationInputTypeDef


def get_value() -> AgentCollaboratorInvocationInputTypeDef:
    return {
        "agentCollaboratorAliasArn": ...,
    }


# AgentCollaboratorInvocationInputTypeDef definition

class AgentCollaboratorInvocationInputTypeDef(TypedDict):
    agentCollaboratorAliasArn: NotRequired[str],
    agentCollaboratorName: NotRequired[str],
    input: NotRequired[AgentCollaboratorInputPayloadTypeDef],  # (1)
```

1. See [:material-code-braces: AgentCollaboratorInputPayloadTypeDef](./type_defs.md#agentcollaboratorinputpayloadtypedef) 
## InlineSessionStateTypeDef

```python
# InlineSessionStateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InlineSessionStateTypeDef


def get_value() -> InlineSessionStateTypeDef:
    return {
        "files": ...,
    }


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
# KnowledgeBaseVectorSearchConfigurationPaginatorTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import KnowledgeBaseVectorSearchConfigurationPaginatorTypeDef


def get_value() -> KnowledgeBaseVectorSearchConfigurationPaginatorTypeDef:
    return {
        "filter": ...,
    }


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
# KnowledgeBaseVectorSearchConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import KnowledgeBaseVectorSearchConfigurationTypeDef


def get_value() -> KnowledgeBaseVectorSearchConfigurationTypeDef:
    return {
        "filter": ...,
    }


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
# FlowResponseStreamTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import FlowResponseStreamTypeDef


def get_value() -> FlowResponseStreamTypeDef:
    return {
        "accessDeniedException": ...,
    }


# FlowResponseStreamTypeDef definition

class FlowResponseStreamTypeDef(TypedDict):
    accessDeniedException: NotRequired[AccessDeniedExceptionTypeDef],  # (1)
    badGatewayException: NotRequired[BadGatewayExceptionTypeDef],  # (2)
    conflictException: NotRequired[ConflictExceptionTypeDef],  # (3)
    dependencyFailedException: NotRequired[DependencyFailedExceptionTypeDef],  # (4)
    flowCompletionEvent: NotRequired[FlowCompletionEventTypeDef],  # (5)
    flowMultiTurnInputRequestEvent: NotRequired[FlowMultiTurnInputRequestEventTypeDef],  # (6)
    flowOutputEvent: NotRequired[FlowOutputEventTypeDef],  # (7)
    flowTraceEvent: NotRequired[FlowTraceEventTypeDef],  # (8)
    internalServerException: NotRequired[InternalServerExceptionTypeDef],  # (9)
    resourceNotFoundException: NotRequired[ResourceNotFoundExceptionTypeDef],  # (10)
    serviceQuotaExceededException: NotRequired[ServiceQuotaExceededExceptionTypeDef],  # (11)
    throttlingException: NotRequired[ThrottlingExceptionTypeDef],  # (12)
    validationException: NotRequired[ValidationExceptionTypeDef],  # (13)
```

1. See [:material-code-braces: AccessDeniedExceptionTypeDef](./type_defs.md#accessdeniedexceptiontypedef) 
2. See [:material-code-braces: BadGatewayExceptionTypeDef](./type_defs.md#badgatewayexceptiontypedef) 
3. See [:material-code-braces: ConflictExceptionTypeDef](./type_defs.md#conflictexceptiontypedef) 
4. See [:material-code-braces: DependencyFailedExceptionTypeDef](./type_defs.md#dependencyfailedexceptiontypedef) 
5. See [:material-code-braces: FlowCompletionEventTypeDef](./type_defs.md#flowcompletioneventtypedef) 
6. See [:material-code-braces: FlowMultiTurnInputRequestEventTypeDef](./type_defs.md#flowmultiturninputrequesteventtypedef) 
7. See [:material-code-braces: FlowOutputEventTypeDef](./type_defs.md#flowoutputeventtypedef) 
8. See [:material-code-braces: FlowTraceEventTypeDef](./type_defs.md#flowtraceeventtypedef) 
9. See [:material-code-braces: InternalServerExceptionTypeDef](./type_defs.md#internalserverexceptiontypedef) 
10. See [:material-code-braces: ResourceNotFoundExceptionTypeDef](./type_defs.md#resourcenotfoundexceptiontypedef) 
11. See [:material-code-braces: ServiceQuotaExceededExceptionTypeDef](./type_defs.md#servicequotaexceededexceptiontypedef) 
12. See [:material-code-braces: ThrottlingExceptionTypeDef](./type_defs.md#throttlingexceptiontypedef) 
13. See [:material-code-braces: ValidationExceptionTypeDef](./type_defs.md#validationexceptiontypedef) 
## InlineAgentPayloadPartTypeDef

```python
# InlineAgentPayloadPartTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InlineAgentPayloadPartTypeDef


def get_value() -> InlineAgentPayloadPartTypeDef:
    return {
        "attribution": ...,
    }


# InlineAgentPayloadPartTypeDef definition

class InlineAgentPayloadPartTypeDef(TypedDict):
    attribution: NotRequired[AttributionTypeDef],  # (1)
    bytes: NotRequired[bytes],
```

1. See [:material-code-braces: AttributionTypeDef](./type_defs.md#attributiontypedef) 
## PayloadPartTypeDef

```python
# PayloadPartTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import PayloadPartTypeDef


def get_value() -> PayloadPartTypeDef:
    return {
        "attribution": ...,
    }


# PayloadPartTypeDef definition

class PayloadPartTypeDef(TypedDict):
    attribution: NotRequired[AttributionTypeDef],  # (1)
    bytes: NotRequired[bytes],
```

1. See [:material-code-braces: AttributionTypeDef](./type_defs.md#attributiontypedef) 
## RetrieveAndGenerateStreamResponseOutputTypeDef

```python
# RetrieveAndGenerateStreamResponseOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrieveAndGenerateStreamResponseOutputTypeDef


def get_value() -> RetrieveAndGenerateStreamResponseOutputTypeDef:
    return {
        "accessDeniedException": ...,
    }


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
# AgentCollaboratorOutputPayloadTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import AgentCollaboratorOutputPayloadTypeDef


def get_value() -> AgentCollaboratorOutputPayloadTypeDef:
    return {
        "returnControlPayload": ...,
    }


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
# InvocationInputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InvocationInputTypeDef


def get_value() -> InvocationInputTypeDef:
    return {
        "actionGroupInvocationInput": ...,
    }


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
# KnowledgeBaseRetrievalConfigurationPaginatorTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import KnowledgeBaseRetrievalConfigurationPaginatorTypeDef


def get_value() -> KnowledgeBaseRetrievalConfigurationPaginatorTypeDef:
    return {
        "vectorSearchConfiguration": ...,
    }


# KnowledgeBaseRetrievalConfigurationPaginatorTypeDef definition

class KnowledgeBaseRetrievalConfigurationPaginatorTypeDef(TypedDict):
    vectorSearchConfiguration: KnowledgeBaseVectorSearchConfigurationPaginatorTypeDef,  # (1)
```

1. See [:material-code-braces: KnowledgeBaseVectorSearchConfigurationPaginatorTypeDef](./type_defs.md#knowledgebasevectorsearchconfigurationpaginatortypedef) 
## KnowledgeBaseRetrievalConfigurationTypeDef

```python
# KnowledgeBaseRetrievalConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import KnowledgeBaseRetrievalConfigurationTypeDef


def get_value() -> KnowledgeBaseRetrievalConfigurationTypeDef:
    return {
        "vectorSearchConfiguration": ...,
    }


# KnowledgeBaseRetrievalConfigurationTypeDef definition

class KnowledgeBaseRetrievalConfigurationTypeDef(TypedDict):
    vectorSearchConfiguration: KnowledgeBaseVectorSearchConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: KnowledgeBaseVectorSearchConfigurationTypeDef](./type_defs.md#knowledgebasevectorsearchconfigurationtypedef) 
## InvokeFlowResponseTypeDef

```python
# InvokeFlowResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InvokeFlowResponseTypeDef


def get_value() -> InvokeFlowResponseTypeDef:
    return {
        "executionId": ...,
    }


# InvokeFlowResponseTypeDef definition

class InvokeFlowResponseTypeDef(TypedDict):
    executionId: str,
    responseStream: AioEventStream[FlowResponseStreamTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlowResponseStreamTypeDef](./type_defs.md#flowresponsestreamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RetrieveAndGenerateStreamResponseTypeDef

```python
# RetrieveAndGenerateStreamResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrieveAndGenerateStreamResponseTypeDef


def get_value() -> RetrieveAndGenerateStreamResponseTypeDef:
    return {
        "sessionId": ...,
    }


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
# AgentCollaboratorInvocationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import AgentCollaboratorInvocationOutputTypeDef


def get_value() -> AgentCollaboratorInvocationOutputTypeDef:
    return {
        "agentCollaboratorAliasArn": ...,
    }


# AgentCollaboratorInvocationOutputTypeDef definition

class AgentCollaboratorInvocationOutputTypeDef(TypedDict):
    agentCollaboratorAliasArn: NotRequired[str],
    agentCollaboratorName: NotRequired[str],
    output: NotRequired[AgentCollaboratorOutputPayloadTypeDef],  # (1)
```

1. See [:material-code-braces: AgentCollaboratorOutputPayloadTypeDef](./type_defs.md#agentcollaboratoroutputpayloadtypedef) 
## RetrieveRequestPaginateTypeDef

```python
# RetrieveRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrieveRequestPaginateTypeDef


def get_value() -> RetrieveRequestPaginateTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# RetrieveRequestPaginateTypeDef definition

class RetrieveRequestPaginateTypeDef(TypedDict):
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
# KnowledgeBaseConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import KnowledgeBaseConfigurationTypeDef


def get_value() -> KnowledgeBaseConfigurationTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# KnowledgeBaseConfigurationTypeDef definition

class KnowledgeBaseConfigurationTypeDef(TypedDict):
    knowledgeBaseId: str,
    retrievalConfiguration: KnowledgeBaseRetrievalConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: KnowledgeBaseRetrievalConfigurationTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationtypedef) 
## KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef

```python
# KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef


def get_value() -> KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef:
    return {
        "generationConfiguration": ...,
    }


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
# KnowledgeBaseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import KnowledgeBaseTypeDef


def get_value() -> KnowledgeBaseTypeDef:
    return {
        "description": ...,
    }


# KnowledgeBaseTypeDef definition

class KnowledgeBaseTypeDef(TypedDict):
    description: str,
    knowledgeBaseId: str,
    retrievalConfiguration: NotRequired[KnowledgeBaseRetrievalConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: KnowledgeBaseRetrievalConfigurationTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationtypedef) 
## RetrieveRequestTypeDef

```python
# RetrieveRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrieveRequestTypeDef


def get_value() -> RetrieveRequestTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# RetrieveRequestTypeDef definition

class RetrieveRequestTypeDef(TypedDict):
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
# ObservationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ObservationTypeDef


def get_value() -> ObservationTypeDef:
    return {
        "actionGroupInvocationOutput": ...,
    }


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
# SessionStateTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import SessionStateTypeDef


def get_value() -> SessionStateTypeDef:
    return {
        "conversationHistory": ...,
    }


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
# RetrieveAndGenerateConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrieveAndGenerateConfigurationTypeDef


def get_value() -> RetrieveAndGenerateConfigurationTypeDef:
    return {
        "externalSourcesConfiguration": ...,
    }


# RetrieveAndGenerateConfigurationTypeDef definition

class RetrieveAndGenerateConfigurationTypeDef(TypedDict):
    type: RetrieveAndGenerateTypeType,  # (3)
    externalSourcesConfiguration: NotRequired[ExternalSourcesRetrieveAndGenerateConfigurationTypeDef],  # (1)
    knowledgeBaseConfiguration: NotRequired[KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ExternalSourcesRetrieveAndGenerateConfigurationTypeDef](./type_defs.md#externalsourcesretrieveandgenerateconfigurationtypedef) 
2. See [:material-code-braces: KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef](./type_defs.md#knowledgebaseretrieveandgenerateconfigurationtypedef) 
3. See [:material-code-brackets: RetrieveAndGenerateTypeType](./literals.md#retrieveandgeneratetypetype) 
## InvokeInlineAgentRequestTypeDef

```python
# InvokeInlineAgentRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InvokeInlineAgentRequestTypeDef


def get_value() -> InvokeInlineAgentRequestTypeDef:
    return {
        "foundationModel": ...,
    }


# InvokeInlineAgentRequestTypeDef definition

class InvokeInlineAgentRequestTypeDef(TypedDict):
    foundationModel: str,
    instruction: str,
    sessionId: str,
    actionGroups: NotRequired[Sequence[AgentActionGroupTypeDef]],  # (1)
    bedrockModelConfigurations: NotRequired[InlineBedrockModelConfigurationsTypeDef],  # (2)
    customerEncryptionKeyArn: NotRequired[str],
    enableTrace: NotRequired[bool],
    endSession: NotRequired[bool],
    guardrailConfiguration: NotRequired[GuardrailConfigurationWithArnTypeDef],  # (3)
    idleSessionTTLInSeconds: NotRequired[int],
    inlineSessionState: NotRequired[InlineSessionStateTypeDef],  # (4)
    inputText: NotRequired[str],
    knowledgeBases: NotRequired[Sequence[KnowledgeBaseTypeDef]],  # (5)
    promptOverrideConfiguration: NotRequired[PromptOverrideConfigurationTypeDef],  # (6)
    streamingConfigurations: NotRequired[StreamingConfigurationsTypeDef],  # (7)
```

1. See [:material-code-braces: AgentActionGroupTypeDef](./type_defs.md#agentactiongrouptypedef) 
2. See [:material-code-braces: InlineBedrockModelConfigurationsTypeDef](./type_defs.md#inlinebedrockmodelconfigurationstypedef) 
3. See [:material-code-braces: GuardrailConfigurationWithArnTypeDef](./type_defs.md#guardrailconfigurationwitharntypedef) 
4. See [:material-code-braces: InlineSessionStateTypeDef](./type_defs.md#inlinesessionstatetypedef) 
5. See [:material-code-braces: KnowledgeBaseTypeDef](./type_defs.md#knowledgebasetypedef) 
6. See [:material-code-braces: PromptOverrideConfigurationTypeDef](./type_defs.md#promptoverrideconfigurationtypedef) 
7. See [:material-code-braces: StreamingConfigurationsTypeDef](./type_defs.md#streamingconfigurationstypedef) 
## OrchestrationTraceTypeDef

```python
# OrchestrationTraceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import OrchestrationTraceTypeDef


def get_value() -> OrchestrationTraceTypeDef:
    return {
        "invocationInput": ...,
    }


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
# RoutingClassifierTraceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RoutingClassifierTraceTypeDef


def get_value() -> RoutingClassifierTraceTypeDef:
    return {
        "invocationInput": ...,
    }


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
## InvokeAgentRequestTypeDef

```python
# InvokeAgentRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InvokeAgentRequestTypeDef


def get_value() -> InvokeAgentRequestTypeDef:
    return {
        "agentAliasId": ...,
    }


# InvokeAgentRequestTypeDef definition

class InvokeAgentRequestTypeDef(TypedDict):
    agentAliasId: str,
    agentId: str,
    sessionId: str,
    bedrockModelConfigurations: NotRequired[BedrockModelConfigurationsTypeDef],  # (1)
    enableTrace: NotRequired[bool],
    endSession: NotRequired[bool],
    inputText: NotRequired[str],
    memoryId: NotRequired[str],
    sessionState: NotRequired[SessionStateTypeDef],  # (2)
    sourceArn: NotRequired[str],
    streamingConfigurations: NotRequired[StreamingConfigurationsTypeDef],  # (3)
```

1. See [:material-code-braces: BedrockModelConfigurationsTypeDef](./type_defs.md#bedrockmodelconfigurationstypedef) 
2. See [:material-code-braces: SessionStateTypeDef](./type_defs.md#sessionstatetypedef) 
3. See [:material-code-braces: StreamingConfigurationsTypeDef](./type_defs.md#streamingconfigurationstypedef) 
## RetrieveAndGenerateRequestTypeDef

```python
# RetrieveAndGenerateRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrieveAndGenerateRequestTypeDef


def get_value() -> RetrieveAndGenerateRequestTypeDef:
    return {
        "input": ...,
    }


# RetrieveAndGenerateRequestTypeDef definition

class RetrieveAndGenerateRequestTypeDef(TypedDict):
    input: RetrieveAndGenerateInputTypeDef,  # (1)
    retrieveAndGenerateConfiguration: NotRequired[RetrieveAndGenerateConfigurationTypeDef],  # (2)
    sessionConfiguration: NotRequired[RetrieveAndGenerateSessionConfigurationTypeDef],  # (3)
    sessionId: NotRequired[str],
```

1. See [:material-code-braces: RetrieveAndGenerateInputTypeDef](./type_defs.md#retrieveandgenerateinputtypedef) 
2. See [:material-code-braces: RetrieveAndGenerateConfigurationTypeDef](./type_defs.md#retrieveandgenerateconfigurationtypedef) 
3. See [:material-code-braces: RetrieveAndGenerateSessionConfigurationTypeDef](./type_defs.md#retrieveandgeneratesessionconfigurationtypedef) 
## RetrieveAndGenerateStreamRequestTypeDef

```python
# RetrieveAndGenerateStreamRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrieveAndGenerateStreamRequestTypeDef


def get_value() -> RetrieveAndGenerateStreamRequestTypeDef:
    return {
        "input": ...,
    }


# RetrieveAndGenerateStreamRequestTypeDef definition

class RetrieveAndGenerateStreamRequestTypeDef(TypedDict):
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
# TraceTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import TraceTypeDef


def get_value() -> TraceTypeDef:
    return {
        "customOrchestrationTrace": ...,
    }


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
# InlineAgentTracePartTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InlineAgentTracePartTypeDef


def get_value() -> InlineAgentTracePartTypeDef:
    return {
        "sessionId": ...,
    }


# InlineAgentTracePartTypeDef definition

class InlineAgentTracePartTypeDef(TypedDict):
    sessionId: NotRequired[str],
    trace: NotRequired[TraceTypeDef],  # (1)
```

1. See [:material-code-braces: TraceTypeDef](./type_defs.md#tracetypedef) 
## TracePartTypeDef

```python
# TracePartTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import TracePartTypeDef


def get_value() -> TracePartTypeDef:
    return {
        "agentAliasId": ...,
    }


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
# InlineAgentResponseStreamTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InlineAgentResponseStreamTypeDef


def get_value() -> InlineAgentResponseStreamTypeDef:
    return {
        "accessDeniedException": ...,
    }


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
# ResponseStreamTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import ResponseStreamTypeDef


def get_value() -> ResponseStreamTypeDef:
    return {
        "accessDeniedException": ...,
    }


# ResponseStreamTypeDef definition

class ResponseStreamTypeDef(TypedDict):
    accessDeniedException: NotRequired[AccessDeniedExceptionTypeDef],  # (1)
    badGatewayException: NotRequired[BadGatewayExceptionTypeDef],  # (2)
    chunk: NotRequired[PayloadPartTypeDef],  # (3)
    conflictException: NotRequired[ConflictExceptionTypeDef],  # (4)
    dependencyFailedException: NotRequired[DependencyFailedExceptionTypeDef],  # (5)
    files: NotRequired[FilePartTypeDef],  # (6)
    internalServerException: NotRequired[InternalServerExceptionTypeDef],  # (7)
    modelNotReadyException: NotRequired[ModelNotReadyExceptionTypeDef],  # (8)
    resourceNotFoundException: NotRequired[ResourceNotFoundExceptionTypeDef],  # (9)
    returnControl: NotRequired[ReturnControlPayloadTypeDef],  # (10)
    serviceQuotaExceededException: NotRequired[ServiceQuotaExceededExceptionTypeDef],  # (11)
    throttlingException: NotRequired[ThrottlingExceptionTypeDef],  # (12)
    trace: NotRequired[TracePartTypeDef],  # (13)
    validationException: NotRequired[ValidationExceptionTypeDef],  # (14)
```

1. See [:material-code-braces: AccessDeniedExceptionTypeDef](./type_defs.md#accessdeniedexceptiontypedef) 
2. See [:material-code-braces: BadGatewayExceptionTypeDef](./type_defs.md#badgatewayexceptiontypedef) 
3. See [:material-code-braces: PayloadPartTypeDef](./type_defs.md#payloadparttypedef) 
4. See [:material-code-braces: ConflictExceptionTypeDef](./type_defs.md#conflictexceptiontypedef) 
5. See [:material-code-braces: DependencyFailedExceptionTypeDef](./type_defs.md#dependencyfailedexceptiontypedef) 
6. See [:material-code-braces: FilePartTypeDef](./type_defs.md#fileparttypedef) 
7. See [:material-code-braces: InternalServerExceptionTypeDef](./type_defs.md#internalserverexceptiontypedef) 
8. See [:material-code-braces: ModelNotReadyExceptionTypeDef](./type_defs.md#modelnotreadyexceptiontypedef) 
9. See [:material-code-braces: ResourceNotFoundExceptionTypeDef](./type_defs.md#resourcenotfoundexceptiontypedef) 
10. See [:material-code-braces: ReturnControlPayloadTypeDef](./type_defs.md#returncontrolpayloadtypedef) 
11. See [:material-code-braces: ServiceQuotaExceededExceptionTypeDef](./type_defs.md#servicequotaexceededexceptiontypedef) 
12. See [:material-code-braces: ThrottlingExceptionTypeDef](./type_defs.md#throttlingexceptiontypedef) 
13. See [:material-code-braces: TracePartTypeDef](./type_defs.md#traceparttypedef) 
14. See [:material-code-braces: ValidationExceptionTypeDef](./type_defs.md#validationexceptiontypedef) 
## InvokeInlineAgentResponseTypeDef

```python
# InvokeInlineAgentResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InvokeInlineAgentResponseTypeDef


def get_value() -> InvokeInlineAgentResponseTypeDef:
    return {
        "completion": ...,
    }


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
# InvokeAgentResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock_agent_runtime.type_defs import InvokeAgentResponseTypeDef


def get_value() -> InvokeAgentResponseTypeDef:
    return {
        "completion": ...,
    }


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
