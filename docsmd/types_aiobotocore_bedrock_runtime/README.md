# BedrockRuntime module

> [Index](../README.md) > BedrockRuntime


!!! note ""

    Auto-generated documentation for [BedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#bedrockruntime)
    type annotations stubs module [types-aiobotocore-bedrock-runtime](https://pypi.org/project/types-aiobotocore-bedrock-runtime/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.20.0' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `BedrockRuntime` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `BedrockRuntime` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[bedrock-runtime]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[bedrock-runtime]'

# standalone installation
python -m pip install types-aiobotocore-bedrock-runtime
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-bedrock-runtime
```

## Usage

Code samples can be found in [Examples](./usage.md).

## BedrockRuntimeClient

Type annotations and code completion for  `#!python session.create_client("bedrock-runtime")` as [BedrockRuntimeClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client)

```python
# BedrockRuntimeClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_runtime.client import BedrockRuntimeClient


session = get_session()
async with session.create_client("bedrock-runtime") as client:
    client: BedrockRuntimeClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("bedrock-runtime").get_paginator("...")`.

```python
# ListAsyncInvokesPaginator usage example

from types_aiobotocore_bedrock_runtime.paginator import ListAsyncInvokesPaginator

def get_list_async_invokes_paginator() -> ListAsyncInvokesPaginator:
    return client.get_paginator("list_async_invokes"))
```

- [ListAsyncInvokesPaginator](./paginators.md#listasyncinvokespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AsyncInvokeStatusType usage example

from types_aiobotocore_bedrock_runtime.literals import AsyncInvokeStatusType

def get_value() -> AsyncInvokeStatusType:
    return "Completed"
```

- [AsyncInvokeStatusType](./literals.md#asyncinvokestatustype)
- [ConversationRoleType](./literals.md#conversationroletype)
- [DocumentFormatType](./literals.md#documentformattype)
- [GuardrailActionType](./literals.md#guardrailactiontype)
- [GuardrailContentFilterConfidenceType](./literals.md#guardrailcontentfilterconfidencetype)
- [GuardrailContentFilterStrengthType](./literals.md#guardrailcontentfilterstrengthtype)
- [GuardrailContentFilterTypeType](./literals.md#guardrailcontentfiltertypetype)
- [GuardrailContentPolicyActionType](./literals.md#guardrailcontentpolicyactiontype)
- [GuardrailContentQualifierType](./literals.md#guardrailcontentqualifiertype)
- [GuardrailContentSourceType](./literals.md#guardrailcontentsourcetype)
- [GuardrailContextualGroundingFilterTypeType](./literals.md#guardrailcontextualgroundingfiltertypetype)
- [GuardrailContextualGroundingPolicyActionType](./literals.md#guardrailcontextualgroundingpolicyactiontype)
- [GuardrailConverseContentQualifierType](./literals.md#guardrailconversecontentqualifiertype)
- [GuardrailConverseImageFormatType](./literals.md#guardrailconverseimageformattype)
- [GuardrailImageFormatType](./literals.md#guardrailimageformattype)
- [GuardrailManagedWordTypeType](./literals.md#guardrailmanagedwordtypetype)
- [GuardrailPiiEntityTypeType](./literals.md#guardrailpiientitytypetype)
- [GuardrailSensitiveInformationPolicyActionType](./literals.md#guardrailsensitiveinformationpolicyactiontype)
- [GuardrailStreamProcessingModeType](./literals.md#guardrailstreamprocessingmodetype)
- [GuardrailTopicPolicyActionType](./literals.md#guardrailtopicpolicyactiontype)
- [GuardrailTopicTypeType](./literals.md#guardrailtopictypetype)
- [GuardrailTraceType](./literals.md#guardrailtracetype)
- [GuardrailWordPolicyActionType](./literals.md#guardrailwordpolicyactiontype)
- [ImageFormatType](./literals.md#imageformattype)
- [ListAsyncInvokesPaginatorName](./literals.md#listasyncinvokespaginatorname)
- [PerformanceConfigLatencyType](./literals.md#performanceconfiglatencytype)
- [SortAsyncInvocationByType](./literals.md#sortasyncinvocationbytype)
- [SortOrderType](./literals.md#sortordertype)
- [StopReasonType](./literals.md#stopreasontype)
- [ToolResultStatusType](./literals.md#toolresultstatustype)
- [TraceType](./literals.md#tracetype)
- [VideoFormatType](./literals.md#videoformattype)
- [BedrockRuntimeServiceName](./literals.md#bedrockruntimeservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [GuardrailOutputContentTypeDef](./type_defs.md#guardrailoutputcontenttypedef)
- [GuardrailUsageTypeDef](./type_defs.md#guardrailusagetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AsyncInvokeS3OutputDataConfigTypeDef](./type_defs.md#asyncinvokes3outputdataconfigtypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [ToolUseBlockDeltaTypeDef](./type_defs.md#tooluseblockdeltatypedef)
- [ToolUseBlockOutputTypeDef](./type_defs.md#tooluseblockoutputtypedef)
- [ToolUseBlockStartTypeDef](./type_defs.md#tooluseblockstarttypedef)
- [ContentBlockStopEventTypeDef](./type_defs.md#contentblockstopeventtypedef)
- [ConverseMetricsTypeDef](./type_defs.md#conversemetricstypedef)
- [GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef)
- [InferenceConfigurationTypeDef](./type_defs.md#inferenceconfigurationtypedef)
- [PerformanceConfigurationTypeDef](./type_defs.md#performanceconfigurationtypedef)
- [PromptVariableValuesTypeDef](./type_defs.md#promptvariablevaluestypedef)
- [TokenUsageTypeDef](./type_defs.md#tokenusagetypedef)
- [ConverseStreamMetricsTypeDef](./type_defs.md#conversestreammetricstypedef)
- [InternalServerExceptionTypeDef](./type_defs.md#internalserverexceptiontypedef)
- [MessageStartEventTypeDef](./type_defs.md#messagestarteventtypedef)
- [MessageStopEventTypeDef](./type_defs.md#messagestopeventtypedef)
- [ModelStreamErrorExceptionTypeDef](./type_defs.md#modelstreamerrorexceptiontypedef)
- [ServiceUnavailableExceptionTypeDef](./type_defs.md#serviceunavailableexceptiontypedef)
- [ThrottlingExceptionTypeDef](./type_defs.md#throttlingexceptiontypedef)
- [ValidationExceptionTypeDef](./type_defs.md#validationexceptiontypedef)
- [GuardrailStreamConfigurationTypeDef](./type_defs.md#guardrailstreamconfigurationtypedef)
- [PromptRouterTraceTypeDef](./type_defs.md#promptroutertracetypedef)
- [DocumentSourceOutputTypeDef](./type_defs.md#documentsourceoutputtypedef)
- [GetAsyncInvokeRequestTypeDef](./type_defs.md#getasyncinvokerequesttypedef)
- [GuardrailTextBlockTypeDef](./type_defs.md#guardrailtextblocktypedef)
- [GuardrailContentFilterTypeDef](./type_defs.md#guardrailcontentfiltertypedef)
- [GuardrailContextualGroundingFilterTypeDef](./type_defs.md#guardrailcontextualgroundingfiltertypedef)
- [GuardrailConverseTextBlockOutputTypeDef](./type_defs.md#guardrailconversetextblockoutputtypedef)
- [GuardrailConverseImageSourceOutputTypeDef](./type_defs.md#guardrailconverseimagesourceoutputtypedef)
- [GuardrailConverseTextBlockTypeDef](./type_defs.md#guardrailconversetextblocktypedef)
- [GuardrailImageCoverageTypeDef](./type_defs.md#guardrailimagecoveragetypedef)
- [GuardrailTextCharactersCoverageTypeDef](./type_defs.md#guardrailtextcharacterscoveragetypedef)
- [GuardrailCustomWordTypeDef](./type_defs.md#guardrailcustomwordtypedef)
- [GuardrailManagedWordTypeDef](./type_defs.md#guardrailmanagedwordtypedef)
- [GuardrailPiiEntityFilterTypeDef](./type_defs.md#guardrailpiientityfiltertypedef)
- [GuardrailRegexFilterTypeDef](./type_defs.md#guardrailregexfiltertypedef)
- [GuardrailTopicTypeDef](./type_defs.md#guardrailtopictypedef)
- [ImageSourceOutputTypeDef](./type_defs.md#imagesourceoutputtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ModelTimeoutExceptionTypeDef](./type_defs.md#modeltimeoutexceptiontypedef)
- [PayloadPartTypeDef](./type_defs.md#payloadparttypedef)
- [S3LocationTypeDef](./type_defs.md#s3locationtypedef)
- [SpecificToolChoiceTypeDef](./type_defs.md#specifictoolchoicetypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ToolInputSchemaTypeDef](./type_defs.md#toolinputschematypedef)
- [ToolUseBlockTypeDef](./type_defs.md#tooluseblocktypedef)
- [InvokeModelResponseTypeDef](./type_defs.md#invokemodelresponsetypedef)
- [StartAsyncInvokeResponseTypeDef](./type_defs.md#startasyncinvokeresponsetypedef)
- [AsyncInvokeOutputDataConfigTypeDef](./type_defs.md#asyncinvokeoutputdataconfigtypedef)
- [DocumentSourceTypeDef](./type_defs.md#documentsourcetypedef)
- [GuardrailConverseImageSourceTypeDef](./type_defs.md#guardrailconverseimagesourcetypedef)
- [GuardrailImageSourceTypeDef](./type_defs.md#guardrailimagesourcetypedef)
- [ImageSourceTypeDef](./type_defs.md#imagesourcetypedef)
- [InvokeModelRequestTypeDef](./type_defs.md#invokemodelrequesttypedef)
- [InvokeModelWithResponseStreamRequestTypeDef](./type_defs.md#invokemodelwithresponsestreamrequesttypedef)
- [ContentBlockDeltaTypeDef](./type_defs.md#contentblockdeltatypedef)
- [ContentBlockStartTypeDef](./type_defs.md#contentblockstarttypedef)
- [DocumentBlockOutputTypeDef](./type_defs.md#documentblockoutputtypedef)
- [GuardrailContentPolicyAssessmentTypeDef](./type_defs.md#guardrailcontentpolicyassessmenttypedef)
- [GuardrailContextualGroundingPolicyAssessmentTypeDef](./type_defs.md#guardrailcontextualgroundingpolicyassessmenttypedef)
- [GuardrailConverseImageBlockOutputTypeDef](./type_defs.md#guardrailconverseimageblockoutputtypedef)
- [GuardrailConverseTextBlockUnionTypeDef](./type_defs.md#guardrailconversetextblockuniontypedef)
- [GuardrailCoverageTypeDef](./type_defs.md#guardrailcoveragetypedef)
- [GuardrailWordPolicyAssessmentTypeDef](./type_defs.md#guardrailwordpolicyassessmenttypedef)
- [GuardrailSensitiveInformationPolicyAssessmentTypeDef](./type_defs.md#guardrailsensitiveinformationpolicyassessmenttypedef)
- [GuardrailTopicPolicyAssessmentTypeDef](./type_defs.md#guardrailtopicpolicyassessmenttypedef)
- [ImageBlockOutputTypeDef](./type_defs.md#imageblockoutputtypedef)
- [ListAsyncInvokesRequestPaginateTypeDef](./type_defs.md#listasyncinvokesrequestpaginatetypedef)
- [ListAsyncInvokesRequestTypeDef](./type_defs.md#listasyncinvokesrequesttypedef)
- [ResponseStreamTypeDef](./type_defs.md#responsestreamtypedef)
- [VideoSourceOutputTypeDef](./type_defs.md#videosourceoutputtypedef)
- [VideoSourceTypeDef](./type_defs.md#videosourcetypedef)
- [ToolChoiceTypeDef](./type_defs.md#toolchoicetypedef)
- [ToolSpecificationTypeDef](./type_defs.md#toolspecificationtypedef)
- [ToolUseBlockUnionTypeDef](./type_defs.md#tooluseblockuniontypedef)
- [AsyncInvokeSummaryTypeDef](./type_defs.md#asyncinvokesummarytypedef)
- [GetAsyncInvokeResponseTypeDef](./type_defs.md#getasyncinvokeresponsetypedef)
- [StartAsyncInvokeRequestTypeDef](./type_defs.md#startasyncinvokerequesttypedef)
- [DocumentSourceUnionTypeDef](./type_defs.md#documentsourceuniontypedef)
- [GuardrailConverseImageSourceUnionTypeDef](./type_defs.md#guardrailconverseimagesourceuniontypedef)
- [GuardrailImageBlockTypeDef](./type_defs.md#guardrailimageblocktypedef)
- [ImageSourceUnionTypeDef](./type_defs.md#imagesourceuniontypedef)
- [ContentBlockDeltaEventTypeDef](./type_defs.md#contentblockdeltaeventtypedef)
- [ContentBlockStartEventTypeDef](./type_defs.md#contentblockstarteventtypedef)
- [GuardrailConverseContentBlockOutputTypeDef](./type_defs.md#guardrailconversecontentblockoutputtypedef)
- [GuardrailInvocationMetricsTypeDef](./type_defs.md#guardrailinvocationmetricstypedef)
- [InvokeModelWithResponseStreamResponseTypeDef](./type_defs.md#invokemodelwithresponsestreamresponsetypedef)
- [VideoBlockOutputTypeDef](./type_defs.md#videoblockoutputtypedef)
- [VideoSourceUnionTypeDef](./type_defs.md#videosourceuniontypedef)
- [ToolTypeDef](./type_defs.md#tooltypedef)
- [ListAsyncInvokesResponseTypeDef](./type_defs.md#listasyncinvokesresponsetypedef)
- [DocumentBlockTypeDef](./type_defs.md#documentblocktypedef)
- [GuardrailConverseImageBlockTypeDef](./type_defs.md#guardrailconverseimageblocktypedef)
- [GuardrailContentBlockTypeDef](./type_defs.md#guardrailcontentblocktypedef)
- [ImageBlockTypeDef](./type_defs.md#imageblocktypedef)
- [GuardrailAssessmentTypeDef](./type_defs.md#guardrailassessmenttypedef)
- [ToolResultContentBlockOutputTypeDef](./type_defs.md#toolresultcontentblockoutputtypedef)
- [VideoBlockTypeDef](./type_defs.md#videoblocktypedef)
- [ToolConfigurationTypeDef](./type_defs.md#toolconfigurationtypedef)
- [DocumentBlockUnionTypeDef](./type_defs.md#documentblockuniontypedef)
- [GuardrailConverseImageBlockUnionTypeDef](./type_defs.md#guardrailconverseimageblockuniontypedef)
- [ApplyGuardrailRequestTypeDef](./type_defs.md#applyguardrailrequesttypedef)
- [ImageBlockUnionTypeDef](./type_defs.md#imageblockuniontypedef)
- [ApplyGuardrailResponseTypeDef](./type_defs.md#applyguardrailresponsetypedef)
- [GuardrailTraceAssessmentTypeDef](./type_defs.md#guardrailtraceassessmenttypedef)
- [ToolResultBlockOutputTypeDef](./type_defs.md#toolresultblockoutputtypedef)
- [VideoBlockUnionTypeDef](./type_defs.md#videoblockuniontypedef)
- [GuardrailConverseContentBlockTypeDef](./type_defs.md#guardrailconversecontentblocktypedef)
- [ConverseStreamTraceTypeDef](./type_defs.md#conversestreamtracetypedef)
- [ConverseTraceTypeDef](./type_defs.md#conversetracetypedef)
- [ContentBlockOutputTypeDef](./type_defs.md#contentblockoutputtypedef)
- [ToolResultContentBlockTypeDef](./type_defs.md#toolresultcontentblocktypedef)
- [GuardrailConverseContentBlockUnionTypeDef](./type_defs.md#guardrailconversecontentblockuniontypedef)
- [ConverseStreamMetadataEventTypeDef](./type_defs.md#conversestreammetadataeventtypedef)
- [MessageOutputTypeDef](./type_defs.md#messageoutputtypedef)
- [ToolResultContentBlockUnionTypeDef](./type_defs.md#toolresultcontentblockuniontypedef)
- [SystemContentBlockTypeDef](./type_defs.md#systemcontentblocktypedef)
- [ConverseStreamOutputTypeDef](./type_defs.md#conversestreamoutputtypedef)
- [ConverseOutputTypeDef](./type_defs.md#converseoutputtypedef)
- [ToolResultBlockTypeDef](./type_defs.md#toolresultblocktypedef)
- [ConverseStreamResponseTypeDef](./type_defs.md#conversestreamresponsetypedef)
- [ConverseResponseTypeDef](./type_defs.md#converseresponsetypedef)
- [ToolResultBlockUnionTypeDef](./type_defs.md#toolresultblockuniontypedef)
- [ContentBlockTypeDef](./type_defs.md#contentblocktypedef)
- [ContentBlockUnionTypeDef](./type_defs.md#contentblockuniontypedef)
- [MessageTypeDef](./type_defs.md#messagetypedef)
- [MessageUnionTypeDef](./type_defs.md#messageuniontypedef)
- [ConverseRequestTypeDef](./type_defs.md#converserequesttypedef)
- [ConverseStreamRequestTypeDef](./type_defs.md#conversestreamrequesttypedef)

