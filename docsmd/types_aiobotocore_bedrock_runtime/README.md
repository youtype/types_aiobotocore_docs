# BedrockRuntime module

> [Index](../README.md) > BedrockRuntime


!!! note ""

    Auto-generated documentation for [BedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime)
    type annotations stubs module [types-aiobotocore-bedrock-runtime](https://pypi.org/project/types-aiobotocore-bedrock-runtime/).

## How to install



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








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ConversationRoleType usage example

from types_aiobotocore_bedrock_runtime.literals import ConversationRoleType

def get_value() -> ConversationRoleType:
    return "assistant"
```

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
- [GuardrailManagedWordTypeType](./literals.md#guardrailmanagedwordtypetype)
- [GuardrailPiiEntityTypeType](./literals.md#guardrailpiientitytypetype)
- [GuardrailSensitiveInformationPolicyActionType](./literals.md#guardrailsensitiveinformationpolicyactiontype)
- [GuardrailStreamProcessingModeType](./literals.md#guardrailstreamprocessingmodetype)
- [GuardrailTopicPolicyActionType](./literals.md#guardrailtopicpolicyactiontype)
- [GuardrailTopicTypeType](./literals.md#guardrailtopictypetype)
- [GuardrailTraceType](./literals.md#guardrailtracetype)
- [GuardrailWordPolicyActionType](./literals.md#guardrailwordpolicyactiontype)
- [ImageFormatType](./literals.md#imageformattype)
- [StopReasonType](./literals.md#stopreasontype)
- [ToolResultStatusType](./literals.md#toolresultstatustype)
- [TraceType](./literals.md#tracetype)
- [BedrockRuntimeServiceName](./literals.md#bedrockruntimeservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [GuardrailOutputContentTypeDef](./type_defs.md#guardrailoutputcontenttypedef)
- [GuardrailUsageTypeDef](./type_defs.md#guardrailusagetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [ToolUseBlockDeltaTypeDef](./type_defs.md#tooluseblockdeltatypedef)
- [ToolUseBlockOutputTypeDef](./type_defs.md#tooluseblockoutputtypedef)
- [ToolUseBlockStartTypeDef](./type_defs.md#tooluseblockstarttypedef)
- [ContentBlockStopEventTypeDef](./type_defs.md#contentblockstopeventtypedef)
- [ConverseMetricsTypeDef](./type_defs.md#conversemetricstypedef)
- [GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef)
- [InferenceConfigurationTypeDef](./type_defs.md#inferenceconfigurationtypedef)
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
- [DocumentSourceOutputTypeDef](./type_defs.md#documentsourceoutputtypedef)
- [GuardrailTextBlockTypeDef](./type_defs.md#guardrailtextblocktypedef)
- [GuardrailContentFilterTypeDef](./type_defs.md#guardrailcontentfiltertypedef)
- [GuardrailContextualGroundingFilterTypeDef](./type_defs.md#guardrailcontextualgroundingfiltertypedef)
- [GuardrailConverseTextBlockOutputTypeDef](./type_defs.md#guardrailconversetextblockoutputtypedef)
- [GuardrailConverseTextBlockTypeDef](./type_defs.md#guardrailconversetextblocktypedef)
- [GuardrailTextCharactersCoverageTypeDef](./type_defs.md#guardrailtextcharacterscoveragetypedef)
- [GuardrailCustomWordTypeDef](./type_defs.md#guardrailcustomwordtypedef)
- [GuardrailManagedWordTypeDef](./type_defs.md#guardrailmanagedwordtypedef)
- [GuardrailPiiEntityFilterTypeDef](./type_defs.md#guardrailpiientityfiltertypedef)
- [GuardrailRegexFilterTypeDef](./type_defs.md#guardrailregexfiltertypedef)
- [GuardrailTopicTypeDef](./type_defs.md#guardrailtopictypedef)
- [ImageSourceOutputTypeDef](./type_defs.md#imagesourceoutputtypedef)
- [ModelTimeoutExceptionTypeDef](./type_defs.md#modeltimeoutexceptiontypedef)
- [PayloadPartTypeDef](./type_defs.md#payloadparttypedef)
- [SpecificToolChoiceTypeDef](./type_defs.md#specifictoolchoicetypedef)
- [ToolInputSchemaTypeDef](./type_defs.md#toolinputschematypedef)
- [ToolUseBlockTypeDef](./type_defs.md#tooluseblocktypedef)
- [InvokeModelResponseTypeDef](./type_defs.md#invokemodelresponsetypedef)
- [DocumentSourceTypeDef](./type_defs.md#documentsourcetypedef)
- [ImageSourceTypeDef](./type_defs.md#imagesourcetypedef)
- [InvokeModelRequestRequestTypeDef](./type_defs.md#invokemodelrequestrequesttypedef)
- [InvokeModelWithResponseStreamRequestRequestTypeDef](./type_defs.md#invokemodelwithresponsestreamrequestrequesttypedef)
- [ContentBlockDeltaTypeDef](./type_defs.md#contentblockdeltatypedef)
- [ContentBlockStartTypeDef](./type_defs.md#contentblockstarttypedef)
- [DocumentBlockOutputTypeDef](./type_defs.md#documentblockoutputtypedef)
- [GuardrailContentBlockTypeDef](./type_defs.md#guardrailcontentblocktypedef)
- [GuardrailContentPolicyAssessmentTypeDef](./type_defs.md#guardrailcontentpolicyassessmenttypedef)
- [GuardrailContextualGroundingPolicyAssessmentTypeDef](./type_defs.md#guardrailcontextualgroundingpolicyassessmenttypedef)
- [GuardrailConverseContentBlockOutputTypeDef](./type_defs.md#guardrailconversecontentblockoutputtypedef)
- [GuardrailConverseTextBlockUnionTypeDef](./type_defs.md#guardrailconversetextblockuniontypedef)
- [GuardrailCoverageTypeDef](./type_defs.md#guardrailcoveragetypedef)
- [GuardrailWordPolicyAssessmentTypeDef](./type_defs.md#guardrailwordpolicyassessmenttypedef)
- [GuardrailSensitiveInformationPolicyAssessmentTypeDef](./type_defs.md#guardrailsensitiveinformationpolicyassessmenttypedef)
- [GuardrailTopicPolicyAssessmentTypeDef](./type_defs.md#guardrailtopicpolicyassessmenttypedef)
- [ImageBlockOutputTypeDef](./type_defs.md#imageblockoutputtypedef)
- [ResponseStreamTypeDef](./type_defs.md#responsestreamtypedef)
- [ToolChoiceTypeDef](./type_defs.md#toolchoicetypedef)
- [ToolSpecificationTypeDef](./type_defs.md#toolspecificationtypedef)
- [ToolUseBlockUnionTypeDef](./type_defs.md#tooluseblockuniontypedef)
- [DocumentSourceUnionTypeDef](./type_defs.md#documentsourceuniontypedef)
- [ImageSourceUnionTypeDef](./type_defs.md#imagesourceuniontypedef)
- [ContentBlockDeltaEventTypeDef](./type_defs.md#contentblockdeltaeventtypedef)
- [ContentBlockStartEventTypeDef](./type_defs.md#contentblockstarteventtypedef)
- [ApplyGuardrailRequestRequestTypeDef](./type_defs.md#applyguardrailrequestrequesttypedef)
- [GuardrailConverseContentBlockTypeDef](./type_defs.md#guardrailconversecontentblocktypedef)
- [GuardrailInvocationMetricsTypeDef](./type_defs.md#guardrailinvocationmetricstypedef)
- [ToolResultContentBlockOutputTypeDef](./type_defs.md#toolresultcontentblockoutputtypedef)
- [InvokeModelWithResponseStreamResponseTypeDef](./type_defs.md#invokemodelwithresponsestreamresponsetypedef)
- [ToolTypeDef](./type_defs.md#tooltypedef)
- [DocumentBlockTypeDef](./type_defs.md#documentblocktypedef)
- [ImageBlockTypeDef](./type_defs.md#imageblocktypedef)
- [GuardrailConverseContentBlockUnionTypeDef](./type_defs.md#guardrailconversecontentblockuniontypedef)
- [GuardrailAssessmentTypeDef](./type_defs.md#guardrailassessmenttypedef)
- [ToolResultBlockOutputTypeDef](./type_defs.md#toolresultblockoutputtypedef)
- [ToolConfigurationTypeDef](./type_defs.md#toolconfigurationtypedef)
- [DocumentBlockUnionTypeDef](./type_defs.md#documentblockuniontypedef)
- [ImageBlockUnionTypeDef](./type_defs.md#imageblockuniontypedef)
- [SystemContentBlockTypeDef](./type_defs.md#systemcontentblocktypedef)
- [ApplyGuardrailResponseTypeDef](./type_defs.md#applyguardrailresponsetypedef)
- [GuardrailTraceAssessmentTypeDef](./type_defs.md#guardrailtraceassessmenttypedef)
- [ContentBlockOutputTypeDef](./type_defs.md#contentblockoutputtypedef)
- [ToolResultContentBlockTypeDef](./type_defs.md#toolresultcontentblocktypedef)
- [ConverseStreamTraceTypeDef](./type_defs.md#conversestreamtracetypedef)
- [ConverseTraceTypeDef](./type_defs.md#conversetracetypedef)
- [MessageOutputTypeDef](./type_defs.md#messageoutputtypedef)
- [ToolResultContentBlockUnionTypeDef](./type_defs.md#toolresultcontentblockuniontypedef)
- [ConverseStreamMetadataEventTypeDef](./type_defs.md#conversestreammetadataeventtypedef)
- [ConverseOutputTypeDef](./type_defs.md#converseoutputtypedef)
- [ToolResultBlockTypeDef](./type_defs.md#toolresultblocktypedef)
- [ConverseStreamOutputTypeDef](./type_defs.md#conversestreamoutputtypedef)
- [ConverseResponseTypeDef](./type_defs.md#converseresponsetypedef)
- [ToolResultBlockUnionTypeDef](./type_defs.md#toolresultblockuniontypedef)
- [ConverseStreamResponseTypeDef](./type_defs.md#conversestreamresponsetypedef)
- [ContentBlockTypeDef](./type_defs.md#contentblocktypedef)
- [ContentBlockUnionTypeDef](./type_defs.md#contentblockuniontypedef)
- [MessageTypeDef](./type_defs.md#messagetypedef)
- [ConverseStreamRequestRequestTypeDef](./type_defs.md#conversestreamrequestrequesttypedef)
- [MessageUnionTypeDef](./type_defs.md#messageuniontypedef)
- [ConverseRequestRequestTypeDef](./type_defs.md#converserequestrequesttypedef)

