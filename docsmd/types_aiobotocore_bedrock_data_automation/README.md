# DataAutomationforBedrock module

> [Index](../README.md) > DataAutomationforBedrock


!!! note ""

    Auto-generated documentation for [DataAutomationforBedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation.html#dataautomationforbedrock)
    type annotations stubs module [types-aiobotocore-bedrock-data-automation](https://pypi.org/project/types-aiobotocore-bedrock-data-automation/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `DataAutomationforBedrock` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `DataAutomationforBedrock` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[bedrock-data-automation]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[bedrock-data-automation]'

# standalone installation
python -m pip install types-aiobotocore-bedrock-data-automation
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-bedrock-data-automation
```

## Usage

Code samples can be found in [Examples](./usage.md).

## DataAutomationforBedrockClient

Type annotations and code completion for  `#!python session.create_client("bedrock-data-automation")` as [DataAutomationforBedrockClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation.html#DataAutomationforBedrock.Client)

```python
# DataAutomationforBedrockClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_data_automation.client import DataAutomationforBedrockClient


session = get_session()
async with session.create_client("bedrock-data-automation") as client:
    client: DataAutomationforBedrockClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("bedrock-data-automation").get_paginator("...")`.

```python
# ListBlueprintsPaginator usage example

from types_aiobotocore_bedrock_data_automation.paginator import ListBlueprintsPaginator

def get_list_blueprints_paginator() -> ListBlueprintsPaginator:
    return client.get_paginator("list_blueprints"))
```

- [ListBlueprintsPaginator](./paginators.md#listblueprintspaginator)
- [ListDataAutomationProjectsPaginator](./paginators.md#listdataautomationprojectspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AudioExtractionCategoryTypeType usage example

from types_aiobotocore_bedrock_data_automation.literals import AudioExtractionCategoryTypeType

def get_value() -> AudioExtractionCategoryTypeType:
    return "AUDIO_CONTENT_MODERATION"
```

- [AudioExtractionCategoryTypeType](./literals.md#audioextractioncategorytypetype)
- [AudioGenerativeOutputLanguageType](./literals.md#audiogenerativeoutputlanguagetype)
- [AudioStandardGenerativeFieldTypeType](./literals.md#audiostandardgenerativefieldtypetype)
- [BlueprintOptimizationJobStatusType](./literals.md#blueprintoptimizationjobstatustype)
- [BlueprintStageFilterType](./literals.md#blueprintstagefiltertype)
- [BlueprintStageType](./literals.md#blueprintstagetype)
- [DataAutomationProjectStageFilterType](./literals.md#dataautomationprojectstagefiltertype)
- [DataAutomationProjectStageType](./literals.md#dataautomationprojectstagetype)
- [DataAutomationProjectStatusType](./literals.md#dataautomationprojectstatustype)
- [DataAutomationProjectTypeType](./literals.md#dataautomationprojecttypetype)
- [DesiredModalityType](./literals.md#desiredmodalitytype)
- [DocumentExtractionGranularityTypeType](./literals.md#documentextractiongranularitytypetype)
- [DocumentOutputTextFormatTypeType](./literals.md#documentoutputtextformattypetype)
- [ImageExtractionCategoryTypeType](./literals.md#imageextractioncategorytypetype)
- [ImageStandardGenerativeFieldTypeType](./literals.md#imagestandardgenerativefieldtypetype)
- [LanguageType](./literals.md#languagetype)
- [ListBlueprintsPaginatorName](./literals.md#listblueprintspaginatorname)
- [ListDataAutomationProjectsPaginatorName](./literals.md#listdataautomationprojectspaginatorname)
- [PIIEntityTypeType](./literals.md#piientitytypetype)
- [PIIRedactionMaskModeType](./literals.md#piiredactionmaskmodetype)
- [ResourceOwnerType](./literals.md#resourceownertype)
- [SensitiveDataDetectionModeType](./literals.md#sensitivedatadetectionmodetype)
- [SensitiveDataDetectionScopeTypeType](./literals.md#sensitivedatadetectionscopetypetype)
- [StateType](./literals.md#statetype)
- [TypeType](./literals.md#typetype)
- [VideoExtractionCategoryTypeType](./literals.md#videoextractioncategorytypetype)
- [VideoStandardGenerativeFieldTypeType](./literals.md#videostandardgenerativefieldtypetype)
- [DataAutomationforBedrockServiceName](./literals.md#dataautomationforbedrockservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AudioLanguageConfigurationOutputTypeDef](./type_defs.md#audiolanguageconfigurationoutputtypedef)
- [AudioLanguageConfigurationTypeDef](./type_defs.md#audiolanguageconfigurationtypedef)
- [ModalityProcessingConfigurationTypeDef](./type_defs.md#modalityprocessingconfigurationtypedef)
- [AudioStandardGenerativeFieldOutputTypeDef](./type_defs.md#audiostandardgenerativefieldoutputtypedef)
- [AudioStandardGenerativeFieldTypeDef](./type_defs.md#audiostandardgenerativefieldtypedef)
- [BlueprintFilterTypeDef](./type_defs.md#blueprintfiltertypedef)
- [BlueprintItemTypeDef](./type_defs.md#blueprintitemtypedef)
- [BlueprintOptimizationObjectTypeDef](./type_defs.md#blueprintoptimizationobjecttypedef)
- [S3ObjectTypeDef](./type_defs.md#s3objecttypedef)
- [BlueprintSummaryTypeDef](./type_defs.md#blueprintsummarytypedef)
- [ChannelLabelingConfigurationTypeDef](./type_defs.md#channellabelingconfigurationtypedef)
- [CopyBlueprintStageRequestTypeDef](./type_defs.md#copyblueprintstagerequesttypedef)
- [EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateBlueprintVersionRequestTypeDef](./type_defs.md#createblueprintversionrequesttypedef)
- [DataAutomationProjectFilterTypeDef](./type_defs.md#dataautomationprojectfiltertypedef)
- [DataAutomationProjectSummaryTypeDef](./type_defs.md#dataautomationprojectsummarytypedef)
- [DeleteBlueprintRequestTypeDef](./type_defs.md#deleteblueprintrequesttypedef)
- [DeleteDataAutomationProjectRequestTypeDef](./type_defs.md#deletedataautomationprojectrequesttypedef)
- [DocumentBoundingBoxTypeDef](./type_defs.md#documentboundingboxtypedef)
- [DocumentExtractionGranularityOutputTypeDef](./type_defs.md#documentextractiongranularityoutputtypedef)
- [DocumentExtractionGranularityTypeDef](./type_defs.md#documentextractiongranularitytypedef)
- [DocumentOutputAdditionalFileFormatTypeDef](./type_defs.md#documentoutputadditionalfileformattypedef)
- [DocumentOutputTextFormatOutputTypeDef](./type_defs.md#documentoutputtextformatoutputtypedef)
- [DocumentOutputTextFormatTypeDef](./type_defs.md#documentoutputtextformattypedef)
- [SplitterConfigurationTypeDef](./type_defs.md#splitterconfigurationtypedef)
- [DocumentStandardGenerativeFieldTypeDef](./type_defs.md#documentstandardgenerativefieldtypedef)
- [GetBlueprintOptimizationStatusRequestTypeDef](./type_defs.md#getblueprintoptimizationstatusrequesttypedef)
- [GetBlueprintRequestTypeDef](./type_defs.md#getblueprintrequesttypedef)
- [GetDataAutomationProjectRequestTypeDef](./type_defs.md#getdataautomationprojectrequesttypedef)
- [ImageBoundingBoxTypeDef](./type_defs.md#imageboundingboxtypedef)
- [ImageExtractionCategoryOutputTypeDef](./type_defs.md#imageextractioncategoryoutputtypedef)
- [ImageExtractionCategoryTypeDef](./type_defs.md#imageextractioncategorytypedef)
- [ImageStandardGenerativeFieldOutputTypeDef](./type_defs.md#imagestandardgenerativefieldoutputtypedef)
- [ImageStandardGenerativeFieldTypeDef](./type_defs.md#imagestandardgenerativefieldtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [ModalityRoutingConfigurationTypeDef](./type_defs.md#modalityroutingconfigurationtypedef)
- [PIIEntitiesConfigurationOutputTypeDef](./type_defs.md#piientitiesconfigurationoutputtypedef)
- [PIIEntitiesConfigurationTypeDef](./type_defs.md#piientitiesconfigurationtypedef)
- [SpeakerLabelingConfigurationTypeDef](./type_defs.md#speakerlabelingconfigurationtypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [VideoBoundingBoxTypeDef](./type_defs.md#videoboundingboxtypedef)
- [VideoExtractionCategoryOutputTypeDef](./type_defs.md#videoextractioncategoryoutputtypedef)
- [VideoExtractionCategoryTypeDef](./type_defs.md#videoextractioncategorytypedef)
- [VideoStandardGenerativeFieldOutputTypeDef](./type_defs.md#videostandardgenerativefieldoutputtypedef)
- [VideoStandardGenerativeFieldTypeDef](./type_defs.md#videostandardgenerativefieldtypedef)
- [ListDataAutomationProjectsRequestTypeDef](./type_defs.md#listdataautomationprojectsrequesttypedef)
- [CustomOutputConfigurationOutputTypeDef](./type_defs.md#customoutputconfigurationoutputtypedef)
- [CustomOutputConfigurationTypeDef](./type_defs.md#customoutputconfigurationtypedef)
- [BlueprintOptimizationOutputConfigurationTypeDef](./type_defs.md#blueprintoptimizationoutputconfigurationtypedef)
- [BlueprintOptimizationSampleTypeDef](./type_defs.md#blueprintoptimizationsampletypedef)
- [UpdateBlueprintRequestTypeDef](./type_defs.md#updateblueprintrequesttypedef)
- [CreateBlueprintRequestTypeDef](./type_defs.md#createblueprintrequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [CreateDataAutomationProjectResponseTypeDef](./type_defs.md#createdataautomationprojectresponsetypedef)
- [DeleteDataAutomationProjectResponseTypeDef](./type_defs.md#deletedataautomationprojectresponsetypedef)
- [InvokeBlueprintOptimizationAsyncResponseTypeDef](./type_defs.md#invokeblueprintoptimizationasyncresponsetypedef)
- [ListBlueprintsResponseTypeDef](./type_defs.md#listblueprintsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdateDataAutomationProjectResponseTypeDef](./type_defs.md#updatedataautomationprojectresponsetypedef)
- [ListBlueprintsRequestTypeDef](./type_defs.md#listblueprintsrequesttypedef)
- [ListDataAutomationProjectsResponseTypeDef](./type_defs.md#listdataautomationprojectsresponsetypedef)
- [DocumentStandardExtractionOutputTypeDef](./type_defs.md#documentstandardextractionoutputtypedef)
- [DocumentStandardExtractionTypeDef](./type_defs.md#documentstandardextractiontypedef)
- [DocumentOutputFormatOutputTypeDef](./type_defs.md#documentoutputformatoutputtypedef)
- [DocumentOutputFormatTypeDef](./type_defs.md#documentoutputformattypedef)
- [ImageStandardExtractionOutputTypeDef](./type_defs.md#imagestandardextractionoutputtypedef)
- [ImageStandardExtractionTypeDef](./type_defs.md#imagestandardextractiontypedef)
- [ListBlueprintsRequestPaginateTypeDef](./type_defs.md#listblueprintsrequestpaginatetypedef)
- [ListDataAutomationProjectsRequestPaginateTypeDef](./type_defs.md#listdataautomationprojectsrequestpaginatetypedef)
- [SensitiveDataConfigurationOutputTypeDef](./type_defs.md#sensitivedataconfigurationoutputtypedef)
- [SensitiveDataConfigurationTypeDef](./type_defs.md#sensitivedataconfigurationtypedef)
- [TranscriptConfigurationTypeDef](./type_defs.md#transcriptconfigurationtypedef)
- [VideoStandardExtractionOutputTypeDef](./type_defs.md#videostandardextractionoutputtypedef)
- [VideoStandardExtractionTypeDef](./type_defs.md#videostandardextractiontypedef)
- [CustomOutputConfigurationUnionTypeDef](./type_defs.md#customoutputconfigurationuniontypedef)
- [GetBlueprintOptimizationStatusResponseTypeDef](./type_defs.md#getblueprintoptimizationstatusresponsetypedef)
- [BlueprintTypeDef](./type_defs.md#blueprinttypedef)
- [InvokeBlueprintOptimizationAsyncRequestTypeDef](./type_defs.md#invokeblueprintoptimizationasyncrequesttypedef)
- [DocumentStandardOutputConfigurationOutputTypeDef](./type_defs.md#documentstandardoutputconfigurationoutputtypedef)
- [DocumentStandardOutputConfigurationTypeDef](./type_defs.md#documentstandardoutputconfigurationtypedef)
- [ImageStandardOutputConfigurationOutputTypeDef](./type_defs.md#imagestandardoutputconfigurationoutputtypedef)
- [ImageStandardOutputConfigurationTypeDef](./type_defs.md#imagestandardoutputconfigurationtypedef)
- [AudioOverrideConfigurationOutputTypeDef](./type_defs.md#audiooverrideconfigurationoutputtypedef)
- [DocumentOverrideConfigurationOutputTypeDef](./type_defs.md#documentoverrideconfigurationoutputtypedef)
- [ImageOverrideConfigurationOutputTypeDef](./type_defs.md#imageoverrideconfigurationoutputtypedef)
- [VideoOverrideConfigurationOutputTypeDef](./type_defs.md#videooverrideconfigurationoutputtypedef)
- [AudioOverrideConfigurationTypeDef](./type_defs.md#audiooverrideconfigurationtypedef)
- [DocumentOverrideConfigurationTypeDef](./type_defs.md#documentoverrideconfigurationtypedef)
- [ImageOverrideConfigurationTypeDef](./type_defs.md#imageoverrideconfigurationtypedef)
- [VideoOverrideConfigurationTypeDef](./type_defs.md#videooverrideconfigurationtypedef)
- [AudioExtractionCategoryTypeConfigurationTypeDef](./type_defs.md#audioextractioncategorytypeconfigurationtypedef)
- [VideoStandardOutputConfigurationOutputTypeDef](./type_defs.md#videostandardoutputconfigurationoutputtypedef)
- [VideoStandardOutputConfigurationTypeDef](./type_defs.md#videostandardoutputconfigurationtypedef)
- [CreateBlueprintResponseTypeDef](./type_defs.md#createblueprintresponsetypedef)
- [CreateBlueprintVersionResponseTypeDef](./type_defs.md#createblueprintversionresponsetypedef)
- [GetBlueprintResponseTypeDef](./type_defs.md#getblueprintresponsetypedef)
- [UpdateBlueprintResponseTypeDef](./type_defs.md#updateblueprintresponsetypedef)
- [OverrideConfigurationOutputTypeDef](./type_defs.md#overrideconfigurationoutputtypedef)
- [OverrideConfigurationTypeDef](./type_defs.md#overrideconfigurationtypedef)
- [AudioExtractionCategoryOutputTypeDef](./type_defs.md#audioextractioncategoryoutputtypedef)
- [AudioExtractionCategoryTypeDef](./type_defs.md#audioextractioncategorytypedef)
- [OverrideConfigurationUnionTypeDef](./type_defs.md#overrideconfigurationuniontypedef)
- [AudioStandardExtractionOutputTypeDef](./type_defs.md#audiostandardextractionoutputtypedef)
- [AudioStandardExtractionTypeDef](./type_defs.md#audiostandardextractiontypedef)
- [AudioStandardOutputConfigurationOutputTypeDef](./type_defs.md#audiostandardoutputconfigurationoutputtypedef)
- [AudioStandardOutputConfigurationTypeDef](./type_defs.md#audiostandardoutputconfigurationtypedef)
- [StandardOutputConfigurationOutputTypeDef](./type_defs.md#standardoutputconfigurationoutputtypedef)
- [StandardOutputConfigurationTypeDef](./type_defs.md#standardoutputconfigurationtypedef)
- [DataAutomationProjectTypeDef](./type_defs.md#dataautomationprojecttypedef)
- [StandardOutputConfigurationUnionTypeDef](./type_defs.md#standardoutputconfigurationuniontypedef)
- [GetDataAutomationProjectResponseTypeDef](./type_defs.md#getdataautomationprojectresponsetypedef)
- [CreateDataAutomationProjectRequestTypeDef](./type_defs.md#createdataautomationprojectrequesttypedef)
- [UpdateDataAutomationProjectRequestTypeDef](./type_defs.md#updatedataautomationprojectrequesttypedef)

