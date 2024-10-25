# AgentsforBedrockRuntime module

> [Index](../README.md) > AgentsforBedrockRuntime


!!! note ""

    Auto-generated documentation for [AgentsforBedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime)
    type annotations stubs module [types-aiobotocore-bedrock-agent-runtime](https://pypi.org/project/types-aiobotocore-bedrock-agent-runtime/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `AgentsforBedrockRuntime` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[bedrock-agent-runtime]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[bedrock-agent-runtime]'


# standalone installation
python -m pip install types-aiobotocore-bedrock-agent-runtime
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-bedrock-agent-runtime
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AgentsforBedrockRuntimeClient

Type annotations and code completion for  `#!python session.create_client("bedrock-agent-runtime")` as [AgentsforBedrockRuntimeClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime.Client)

```python
# AgentsforBedrockRuntimeClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent_runtime.client import AgentsforBedrockRuntimeClient


session = get_session()
async with session.create_client("bedrock-agent-runtime") as client:
    client: AgentsforBedrockRuntimeClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("bedrock-agent-runtime").get_paginator("...")`.

```python
# GetAgentMemoryPaginator usage example

from types_aiobotocore_bedrock_agent_runtime.paginator import GetAgentMemoryPaginator

def get_get_agent_memory_paginator() -> GetAgentMemoryPaginator:
    return client.get_paginator("get_agent_memory"))
```

- [GetAgentMemoryPaginator](./paginators.md#getagentmemorypaginator)
- [RetrievePaginator](./paginators.md#retrievepaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActionInvocationTypeType usage example

from types_aiobotocore_bedrock_agent_runtime.literals import ActionInvocationTypeType

def get_value() -> ActionInvocationTypeType:
    return "RESULT"
```

- [ActionInvocationTypeType](./literals.md#actioninvocationtypetype)
- [ConfirmationStateType](./literals.md#confirmationstatetype)
- [CreationModeType](./literals.md#creationmodetype)
- [ExecutionTypeType](./literals.md#executiontypetype)
- [ExternalSourceTypeType](./literals.md#externalsourcetypetype)
- [FileSourceTypeType](./literals.md#filesourcetypetype)
- [FileUseCaseType](./literals.md#fileusecasetype)
- [FlowCompletionReasonType](./literals.md#flowcompletionreasontype)
- [GetAgentMemoryPaginatorName](./literals.md#getagentmemorypaginatorname)
- [GuadrailActionType](./literals.md#guadrailactiontype)
- [GuardrailActionType](./literals.md#guardrailactiontype)
- [GuardrailContentFilterConfidenceType](./literals.md#guardrailcontentfilterconfidencetype)
- [GuardrailContentFilterTypeType](./literals.md#guardrailcontentfiltertypetype)
- [GuardrailContentPolicyActionType](./literals.md#guardrailcontentpolicyactiontype)
- [GuardrailManagedWordTypeType](./literals.md#guardrailmanagedwordtypetype)
- [GuardrailPiiEntityTypeType](./literals.md#guardrailpiientitytypetype)
- [GuardrailSensitiveInformationPolicyActionType](./literals.md#guardrailsensitiveinformationpolicyactiontype)
- [GuardrailTopicPolicyActionType](./literals.md#guardrailtopicpolicyactiontype)
- [GuardrailTopicTypeType](./literals.md#guardrailtopictypetype)
- [GuardrailWordPolicyActionType](./literals.md#guardrailwordpolicyactiontype)
- [InvocationTypeType](./literals.md#invocationtypetype)
- [MemoryTypeType](./literals.md#memorytypetype)
- [NodeTypeType](./literals.md#nodetypetype)
- [PromptTypeType](./literals.md#prompttypetype)
- [QueryTransformationTypeType](./literals.md#querytransformationtypetype)
- [ResponseStateType](./literals.md#responsestatetype)
- [RetrievalResultLocationTypeType](./literals.md#retrievalresultlocationtypetype)
- [RetrieveAndGenerateTypeType](./literals.md#retrieveandgeneratetypetype)
- [RetrievePaginatorName](./literals.md#retrievepaginatorname)
- [SearchTypeType](./literals.md#searchtypetype)
- [SourceType](./literals.md#sourcetype)
- [TypeType](./literals.md#typetype)
- [AgentsforBedrockRuntimeServiceName](./literals.md#agentsforbedrockruntimeservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccessDeniedExceptionTypeDef](./type_defs.md#accessdeniedexceptiontypedef)
- [ParameterTypeDef](./type_defs.md#parametertypedef)
- [ActionGroupInvocationOutputTypeDef](./type_defs.md#actiongroupinvocationoutputtypedef)
- [ApiParameterTypeDef](./type_defs.md#apiparametertypedef)
- [ContentBodyTypeDef](./type_defs.md#contentbodytypedef)
- [BadGatewayExceptionTypeDef](./type_defs.md#badgatewayexceptiontypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CodeInterpreterInvocationInputTypeDef](./type_defs.md#codeinterpreterinvocationinputtypedef)
- [CodeInterpreterInvocationOutputTypeDef](./type_defs.md#codeinterpreterinvocationoutputtypedef)
- [ConflictExceptionTypeDef](./type_defs.md#conflictexceptiontypedef)
- [DeleteAgentMemoryRequestRequestTypeDef](./type_defs.md#deleteagentmemoryrequestrequesttypedef)
- [DependencyFailedExceptionTypeDef](./type_defs.md#dependencyfailedexceptiontypedef)
- [S3ObjectDocTypeDef](./type_defs.md#s3objectdoctypedef)
- [GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef)
- [PromptTemplateTypeDef](./type_defs.md#prompttemplatetypedef)
- [FailureTraceTypeDef](./type_defs.md#failuretracetypedef)
- [OutputFileTypeDef](./type_defs.md#outputfiletypedef)
- [S3ObjectFileTypeDef](./type_defs.md#s3objectfiletypedef)
- [FilterAttributeTypeDef](./type_defs.md#filterattributetypedef)
- [FinalResponseTypeDef](./type_defs.md#finalresponsetypedef)
- [FlowCompletionEventTypeDef](./type_defs.md#flowcompletioneventtypedef)
- [FlowInputContentTypeDef](./type_defs.md#flowinputcontenttypedef)
- [FlowOutputContentTypeDef](./type_defs.md#flowoutputcontenttypedef)
- [InternalServerExceptionTypeDef](./type_defs.md#internalserverexceptiontypedef)
- [ResourceNotFoundExceptionTypeDef](./type_defs.md#resourcenotfoundexceptiontypedef)
- [ServiceQuotaExceededExceptionTypeDef](./type_defs.md#servicequotaexceededexceptiontypedef)
- [ThrottlingExceptionTypeDef](./type_defs.md#throttlingexceptiontypedef)
- [ValidationExceptionTypeDef](./type_defs.md#validationexceptiontypedef)
- [FunctionParameterTypeDef](./type_defs.md#functionparametertypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetAgentMemoryRequestRequestTypeDef](./type_defs.md#getagentmemoryrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GuardrailContentFilterTypeDef](./type_defs.md#guardrailcontentfiltertypedef)
- [GuardrailCustomWordTypeDef](./type_defs.md#guardrailcustomwordtypedef)
- [GuardrailManagedWordTypeDef](./type_defs.md#guardrailmanagedwordtypedef)
- [GuardrailPiiEntityFilterTypeDef](./type_defs.md#guardrailpiientityfiltertypedef)
- [GuardrailRegexFilterTypeDef](./type_defs.md#guardrailregexfiltertypedef)
- [GuardrailTopicTypeDef](./type_defs.md#guardrailtopictypedef)
- [TextInferenceConfigTypeDef](./type_defs.md#textinferenceconfigtypedef)
- [InferenceConfigurationTypeDef](./type_defs.md#inferenceconfigurationtypedef)
- [KnowledgeBaseLookupInputTypeDef](./type_defs.md#knowledgebaselookupinputtypedef)
- [KnowledgeBaseQueryTypeDef](./type_defs.md#knowledgebasequerytypedef)
- [RetrievalResultContentTypeDef](./type_defs.md#retrievalresultcontenttypedef)
- [MemorySessionSummaryTypeDef](./type_defs.md#memorysessionsummarytypedef)
- [UsageTypeDef](./type_defs.md#usagetypedef)
- [RepromptResponseTypeDef](./type_defs.md#repromptresponsetypedef)
- [QueryTransformationConfigurationTypeDef](./type_defs.md#querytransformationconfigurationtypedef)
- [RawResponseTypeDef](./type_defs.md#rawresponsetypedef)
- [RationaleTypeDef](./type_defs.md#rationaletypedef)
- [PostProcessingParsedResponseTypeDef](./type_defs.md#postprocessingparsedresponsetypedef)
- [PreProcessingParsedResponseTypeDef](./type_defs.md#preprocessingparsedresponsetypedef)
- [RetrievalResultConfluenceLocationTypeDef](./type_defs.md#retrievalresultconfluencelocationtypedef)
- [RetrievalResultS3LocationTypeDef](./type_defs.md#retrievalresults3locationtypedef)
- [RetrievalResultSalesforceLocationTypeDef](./type_defs.md#retrievalresultsalesforcelocationtypedef)
- [RetrievalResultSharePointLocationTypeDef](./type_defs.md#retrievalresultsharepointlocationtypedef)
- [RetrievalResultWebLocationTypeDef](./type_defs.md#retrievalresultweblocationtypedef)
- [RetrieveAndGenerateInputTypeDef](./type_defs.md#retrieveandgenerateinputtypedef)
- [RetrieveAndGenerateOutputTypeDef](./type_defs.md#retrieveandgenerateoutputtypedef)
- [RetrieveAndGenerateSessionConfigurationTypeDef](./type_defs.md#retrieveandgeneratesessionconfigurationtypedef)
- [SpanTypeDef](./type_defs.md#spantypedef)
- [PropertyParametersTypeDef](./type_defs.md#propertyparameterstypedef)
- [RequestBodyTypeDef](./type_defs.md#requestbodytypedef)
- [ApiResultTypeDef](./type_defs.md#apiresulttypedef)
- [FunctionResultTypeDef](./type_defs.md#functionresulttypedef)
- [ByteContentDocTypeDef](./type_defs.md#bytecontentdoctypedef)
- [ByteContentFileTypeDef](./type_defs.md#bytecontentfiletypedef)
- [FilePartTypeDef](./type_defs.md#fileparttypedef)
- [RetrievalFilterPaginatorTypeDef](./type_defs.md#retrievalfilterpaginatortypedef)
- [RetrievalFilterTypeDef](./type_defs.md#retrievalfiltertypedef)
- [FlowInputTypeDef](./type_defs.md#flowinputtypedef)
- [FlowOutputEventTypeDef](./type_defs.md#flowoutputeventtypedef)
- [FunctionInvocationInputTypeDef](./type_defs.md#functioninvocationinputtypedef)
- [GetAgentMemoryRequestGetAgentMemoryPaginateTypeDef](./type_defs.md#getagentmemoryrequestgetagentmemorypaginatetypedef)
- [GuardrailContentPolicyAssessmentTypeDef](./type_defs.md#guardrailcontentpolicyassessmenttypedef)
- [GuardrailWordPolicyAssessmentTypeDef](./type_defs.md#guardrailwordpolicyassessmenttypedef)
- [GuardrailSensitiveInformationPolicyAssessmentTypeDef](./type_defs.md#guardrailsensitiveinformationpolicyassessmenttypedef)
- [GuardrailTopicPolicyAssessmentTypeDef](./type_defs.md#guardrailtopicpolicyassessmenttypedef)
- [InferenceConfigTypeDef](./type_defs.md#inferenceconfigtypedef)
- [ModelInvocationInputTypeDef](./type_defs.md#modelinvocationinputtypedef)
- [MemoryTypeDef](./type_defs.md#memorytypedef)
- [MetadataTypeDef](./type_defs.md#metadatatypedef)
- [RetrievalResultLocationTypeDef](./type_defs.md#retrievalresultlocationtypedef)
- [TextResponsePartTypeDef](./type_defs.md#textresponseparttypedef)
- [ApiRequestBodyTypeDef](./type_defs.md#apirequestbodytypedef)
- [ActionGroupInvocationInputTypeDef](./type_defs.md#actiongroupinvocationinputtypedef)
- [InvocationResultMemberTypeDef](./type_defs.md#invocationresultmembertypedef)
- [ExternalSourceTypeDef](./type_defs.md#externalsourcetypedef)
- [FileSourceTypeDef](./type_defs.md#filesourcetypedef)
- [KnowledgeBaseVectorSearchConfigurationPaginatorTypeDef](./type_defs.md#knowledgebasevectorsearchconfigurationpaginatortypedef)
- [KnowledgeBaseVectorSearchConfigurationTypeDef](./type_defs.md#knowledgebasevectorsearchconfigurationtypedef)
- [InvokeFlowRequestRequestTypeDef](./type_defs.md#invokeflowrequestrequesttypedef)
- [FlowResponseStreamTypeDef](./type_defs.md#flowresponsestreamtypedef)
- [GuardrailAssessmentTypeDef](./type_defs.md#guardrailassessmenttypedef)
- [ExternalSourcesGenerationConfigurationTypeDef](./type_defs.md#externalsourcesgenerationconfigurationtypedef)
- [GenerationConfigurationTypeDef](./type_defs.md#generationconfigurationtypedef)
- [OrchestrationConfigurationTypeDef](./type_defs.md#orchestrationconfigurationtypedef)
- [GetAgentMemoryResponseTypeDef](./type_defs.md#getagentmemoryresponsetypedef)
- [OrchestrationModelInvocationOutputTypeDef](./type_defs.md#orchestrationmodelinvocationoutputtypedef)
- [PostProcessingModelInvocationOutputTypeDef](./type_defs.md#postprocessingmodelinvocationoutputtypedef)
- [PreProcessingModelInvocationOutputTypeDef](./type_defs.md#preprocessingmodelinvocationoutputtypedef)
- [KnowledgeBaseRetrievalResultTypeDef](./type_defs.md#knowledgebaseretrievalresulttypedef)
- [RetrievedReferenceTypeDef](./type_defs.md#retrievedreferencetypedef)
- [GeneratedResponsePartTypeDef](./type_defs.md#generatedresponseparttypedef)
- [ApiInvocationInputTypeDef](./type_defs.md#apiinvocationinputtypedef)
- [InvocationInputTypeDef](./type_defs.md#invocationinputtypedef)
- [InputFileTypeDef](./type_defs.md#inputfiletypedef)
- [KnowledgeBaseRetrievalConfigurationPaginatorTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationpaginatortypedef)
- [KnowledgeBaseRetrievalConfigurationTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationtypedef)
- [InvokeFlowResponseTypeDef](./type_defs.md#invokeflowresponsetypedef)
- [GuardrailTraceTypeDef](./type_defs.md#guardrailtracetypedef)
- [ExternalSourcesRetrieveAndGenerateConfigurationTypeDef](./type_defs.md#externalsourcesretrieveandgenerateconfigurationtypedef)
- [PostProcessingTraceTypeDef](./type_defs.md#postprocessingtracetypedef)
- [PreProcessingTraceTypeDef](./type_defs.md#preprocessingtracetypedef)
- [RetrieveResponseTypeDef](./type_defs.md#retrieveresponsetypedef)
- [KnowledgeBaseLookupOutputTypeDef](./type_defs.md#knowledgebaselookupoutputtypedef)
- [CitationTypeDef](./type_defs.md#citationtypedef)
- [InvocationInputMemberTypeDef](./type_defs.md#invocationinputmembertypedef)
- [RetrieveRequestRetrievePaginateTypeDef](./type_defs.md#retrieverequestretrievepaginatetypedef)
- [KnowledgeBaseConfigurationTypeDef](./type_defs.md#knowledgebaseconfigurationtypedef)
- [KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef](./type_defs.md#knowledgebaseretrieveandgenerateconfigurationtypedef)
- [RetrieveRequestRequestTypeDef](./type_defs.md#retrieverequestrequesttypedef)
- [ObservationTypeDef](./type_defs.md#observationtypedef)
- [AttributionTypeDef](./type_defs.md#attributiontypedef)
- [RetrieveAndGenerateResponseTypeDef](./type_defs.md#retrieveandgenerateresponsetypedef)
- [ReturnControlPayloadTypeDef](./type_defs.md#returncontrolpayloadtypedef)
- [SessionStateTypeDef](./type_defs.md#sessionstatetypedef)
- [RetrieveAndGenerateConfigurationTypeDef](./type_defs.md#retrieveandgenerateconfigurationtypedef)
- [OrchestrationTraceTypeDef](./type_defs.md#orchestrationtracetypedef)
- [PayloadPartTypeDef](./type_defs.md#payloadparttypedef)
- [InvokeAgentRequestRequestTypeDef](./type_defs.md#invokeagentrequestrequesttypedef)
- [RetrieveAndGenerateRequestRequestTypeDef](./type_defs.md#retrieveandgeneraterequestrequesttypedef)
- [TraceTypeDef](./type_defs.md#tracetypedef)
- [TracePartTypeDef](./type_defs.md#traceparttypedef)
- [ResponseStreamTypeDef](./type_defs.md#responsestreamtypedef)
- [InvokeAgentResponseTypeDef](./type_defs.md#invokeagentresponsetypedef)

