# Bedrock module

> [Index](../README.md) > Bedrock


!!! note ""

    Auto-generated documentation for [Bedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#bedrock)
    type annotations stubs module [types-aiobotocore-bedrock](https://pypi.org/project/types-aiobotocore-bedrock/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Bedrock` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Bedrock` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[bedrock]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[bedrock]'

# standalone installation
python -m pip install types-aiobotocore-bedrock
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-bedrock
```

## Usage

Code samples can be found in [Examples](./usage.md).

## BedrockClient

Type annotations and code completion for  `#!python session.create_client("bedrock")` as [BedrockClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client)

```python
# BedrockClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock.client import BedrockClient


session = get_session()
async with session.create_client("bedrock") as client:
    client: BedrockClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("bedrock").get_paginator("...")`.

```python
# ListCustomModelsPaginator usage example

from types_aiobotocore_bedrock.paginator import ListCustomModelsPaginator

def get_list_custom_models_paginator() -> ListCustomModelsPaginator:
    return client.get_paginator("list_custom_models"))
```

- [ListCustomModelsPaginator](./paginators.md#listcustommodelspaginator)
- [ListEvaluationJobsPaginator](./paginators.md#listevaluationjobspaginator)
- [ListGuardrailsPaginator](./paginators.md#listguardrailspaginator)
- [ListImportedModelsPaginator](./paginators.md#listimportedmodelspaginator)
- [ListInferenceProfilesPaginator](./paginators.md#listinferenceprofilespaginator)
- [ListMarketplaceModelEndpointsPaginator](./paginators.md#listmarketplacemodelendpointspaginator)
- [ListModelCopyJobsPaginator](./paginators.md#listmodelcopyjobspaginator)
- [ListModelCustomizationJobsPaginator](./paginators.md#listmodelcustomizationjobspaginator)
- [ListModelImportJobsPaginator](./paginators.md#listmodelimportjobspaginator)
- [ListModelInvocationJobsPaginator](./paginators.md#listmodelinvocationjobspaginator)
- [ListPromptRoutersPaginator](./paginators.md#listpromptrouterspaginator)
- [ListProvisionedModelThroughputsPaginator](./paginators.md#listprovisionedmodelthroughputspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ApplicationTypeType usage example

from types_aiobotocore_bedrock.literals import ApplicationTypeType

def get_value() -> ApplicationTypeType:
    return "ModelEvaluation"
```

- [ApplicationTypeType](./literals.md#applicationtypetype)
- [CommitmentDurationType](./literals.md#commitmentdurationtype)
- [CustomizationTypeType](./literals.md#customizationtypetype)
- [EvaluationJobStatusType](./literals.md#evaluationjobstatustype)
- [EvaluationJobTypeType](./literals.md#evaluationjobtypetype)
- [EvaluationTaskTypeType](./literals.md#evaluationtasktypetype)
- [ExternalSourceTypeType](./literals.md#externalsourcetypetype)
- [FineTuningJobStatusType](./literals.md#finetuningjobstatustype)
- [FoundationModelLifecycleStatusType](./literals.md#foundationmodellifecyclestatustype)
- [GuardrailContentFilterTypeType](./literals.md#guardrailcontentfiltertypetype)
- [GuardrailContextualGroundingFilterTypeType](./literals.md#guardrailcontextualgroundingfiltertypetype)
- [GuardrailFilterStrengthType](./literals.md#guardrailfilterstrengthtype)
- [GuardrailManagedWordsTypeType](./literals.md#guardrailmanagedwordstypetype)
- [GuardrailModalityType](./literals.md#guardrailmodalitytype)
- [GuardrailPiiEntityTypeType](./literals.md#guardrailpiientitytypetype)
- [GuardrailSensitiveInformationActionType](./literals.md#guardrailsensitiveinformationactiontype)
- [GuardrailStatusType](./literals.md#guardrailstatustype)
- [GuardrailTopicTypeType](./literals.md#guardrailtopictypetype)
- [InferenceProfileStatusType](./literals.md#inferenceprofilestatustype)
- [InferenceProfileTypeType](./literals.md#inferenceprofiletypetype)
- [InferenceTypeType](./literals.md#inferencetypetype)
- [ListCustomModelsPaginatorName](./literals.md#listcustommodelspaginatorname)
- [ListEvaluationJobsPaginatorName](./literals.md#listevaluationjobspaginatorname)
- [ListGuardrailsPaginatorName](./literals.md#listguardrailspaginatorname)
- [ListImportedModelsPaginatorName](./literals.md#listimportedmodelspaginatorname)
- [ListInferenceProfilesPaginatorName](./literals.md#listinferenceprofilespaginatorname)
- [ListMarketplaceModelEndpointsPaginatorName](./literals.md#listmarketplacemodelendpointspaginatorname)
- [ListModelCopyJobsPaginatorName](./literals.md#listmodelcopyjobspaginatorname)
- [ListModelCustomizationJobsPaginatorName](./literals.md#listmodelcustomizationjobspaginatorname)
- [ListModelImportJobsPaginatorName](./literals.md#listmodelimportjobspaginatorname)
- [ListModelInvocationJobsPaginatorName](./literals.md#listmodelinvocationjobspaginatorname)
- [ListPromptRoutersPaginatorName](./literals.md#listpromptrouterspaginatorname)
- [ListProvisionedModelThroughputsPaginatorName](./literals.md#listprovisionedmodelthroughputspaginatorname)
- [ModelCopyJobStatusType](./literals.md#modelcopyjobstatustype)
- [ModelCustomizationJobStatusType](./literals.md#modelcustomizationjobstatustype)
- [ModelCustomizationType](./literals.md#modelcustomizationtype)
- [ModelImportJobStatusType](./literals.md#modelimportjobstatustype)
- [ModelInvocationJobStatusType](./literals.md#modelinvocationjobstatustype)
- [ModelModalityType](./literals.md#modelmodalitytype)
- [PromptRouterStatusType](./literals.md#promptrouterstatustype)
- [PromptRouterTypeType](./literals.md#promptroutertypetype)
- [ProvisionedModelStatusType](./literals.md#provisionedmodelstatustype)
- [QueryTransformationTypeType](./literals.md#querytransformationtypetype)
- [RetrieveAndGenerateTypeType](./literals.md#retrieveandgeneratetypetype)
- [S3InputFormatType](./literals.md#s3inputformattype)
- [SearchTypeType](./literals.md#searchtypetype)
- [SortByProvisionedModelsType](./literals.md#sortbyprovisionedmodelstype)
- [SortJobsByType](./literals.md#sortjobsbytype)
- [SortModelsByType](./literals.md#sortmodelsbytype)
- [SortOrderType](./literals.md#sortordertype)
- [StatusType](./literals.md#statustype)
- [BedrockServiceName](./literals.md#bedrockservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BatchDeleteEvaluationJobErrorTypeDef](./type_defs.md#batchdeleteevaluationjoberrortypedef)
- [BatchDeleteEvaluationJobItemTypeDef](./type_defs.md#batchdeleteevaluationjobitemtypedef)
- [BatchDeleteEvaluationJobRequestRequestTypeDef](./type_defs.md#batchdeleteevaluationjobrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BedrockEvaluatorModelTypeDef](./type_defs.md#bedrockevaluatormodeltypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [ByteContentDocOutputTypeDef](./type_defs.md#bytecontentdocoutputtypedef)
- [S3ConfigTypeDef](./type_defs.md#s3configtypedef)
- [EvaluationOutputDataConfigTypeDef](./type_defs.md#evaluationoutputdataconfigtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [CreateGuardrailVersionRequestRequestTypeDef](./type_defs.md#createguardrailversionrequestrequesttypedef)
- [InferenceProfileModelSourceTypeDef](./type_defs.md#inferenceprofilemodelsourcetypedef)
- [OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef)
- [VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef)
- [CustomModelSummaryTypeDef](./type_defs.md#custommodelsummarytypedef)
- [DeleteCustomModelRequestRequestTypeDef](./type_defs.md#deletecustommodelrequestrequesttypedef)
- [DeleteGuardrailRequestRequestTypeDef](./type_defs.md#deleteguardrailrequestrequesttypedef)
- [DeleteImportedModelRequestRequestTypeDef](./type_defs.md#deleteimportedmodelrequestrequesttypedef)
- [DeleteInferenceProfileRequestRequestTypeDef](./type_defs.md#deleteinferenceprofilerequestrequesttypedef)
- [DeleteMarketplaceModelEndpointRequestRequestTypeDef](./type_defs.md#deletemarketplacemodelendpointrequestrequesttypedef)
- [DeleteProvisionedModelThroughputRequestRequestTypeDef](./type_defs.md#deleteprovisionedmodelthroughputrequestrequesttypedef)
- [DeregisterMarketplaceModelEndpointRequestRequestTypeDef](./type_defs.md#deregistermarketplacemodelendpointrequestrequesttypedef)
- [TeacherModelConfigTypeDef](./type_defs.md#teachermodelconfigtypedef)
- [EvaluationBedrockModelTypeDef](./type_defs.md#evaluationbedrockmodeltypedef)
- [EvaluationDatasetLocationTypeDef](./type_defs.md#evaluationdatasetlocationtypedef)
- [EvaluationSummaryTypeDef](./type_defs.md#evaluationsummarytypedef)
- [S3ObjectDocTypeDef](./type_defs.md#s3objectdoctypedef)
- [GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef)
- [PromptTemplateTypeDef](./type_defs.md#prompttemplatetypedef)
- [FilterAttributeOutputTypeDef](./type_defs.md#filterattributeoutputtypedef)
- [FilterAttributeTypeDef](./type_defs.md#filterattributetypedef)
- [FoundationModelLifecycleTypeDef](./type_defs.md#foundationmodellifecycletypedef)
- [GetCustomModelRequestRequestTypeDef](./type_defs.md#getcustommodelrequestrequesttypedef)
- [TrainingMetricsTypeDef](./type_defs.md#trainingmetricstypedef)
- [ValidatorMetricTypeDef](./type_defs.md#validatormetrictypedef)
- [GetEvaluationJobRequestRequestTypeDef](./type_defs.md#getevaluationjobrequestrequesttypedef)
- [GetFoundationModelRequestRequestTypeDef](./type_defs.md#getfoundationmodelrequestrequesttypedef)
- [GetGuardrailRequestRequestTypeDef](./type_defs.md#getguardrailrequestrequesttypedef)
- [GetImportedModelRequestRequestTypeDef](./type_defs.md#getimportedmodelrequestrequesttypedef)
- [GetInferenceProfileRequestRequestTypeDef](./type_defs.md#getinferenceprofilerequestrequesttypedef)
- [InferenceProfileModelTypeDef](./type_defs.md#inferenceprofilemodeltypedef)
- [GetMarketplaceModelEndpointRequestRequestTypeDef](./type_defs.md#getmarketplacemodelendpointrequestrequesttypedef)
- [GetModelCopyJobRequestRequestTypeDef](./type_defs.md#getmodelcopyjobrequestrequesttypedef)
- [GetModelCustomizationJobRequestRequestTypeDef](./type_defs.md#getmodelcustomizationjobrequestrequesttypedef)
- [VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef)
- [GetModelImportJobRequestRequestTypeDef](./type_defs.md#getmodelimportjobrequestrequesttypedef)
- [GetModelInvocationJobRequestRequestTypeDef](./type_defs.md#getmodelinvocationjobrequestrequesttypedef)
- [GetPromptRouterRequestRequestTypeDef](./type_defs.md#getpromptrouterrequestrequesttypedef)
- [PromptRouterTargetModelTypeDef](./type_defs.md#promptroutertargetmodeltypedef)
- [RoutingCriteriaTypeDef](./type_defs.md#routingcriteriatypedef)
- [GetProvisionedModelThroughputRequestRequestTypeDef](./type_defs.md#getprovisionedmodelthroughputrequestrequesttypedef)
- [GuardrailContentFilterConfigTypeDef](./type_defs.md#guardrailcontentfilterconfigtypedef)
- [GuardrailContentFilterTypeDef](./type_defs.md#guardrailcontentfiltertypedef)
- [GuardrailContextualGroundingFilterConfigTypeDef](./type_defs.md#guardrailcontextualgroundingfilterconfigtypedef)
- [GuardrailContextualGroundingFilterTypeDef](./type_defs.md#guardrailcontextualgroundingfiltertypedef)
- [GuardrailManagedWordsConfigTypeDef](./type_defs.md#guardrailmanagedwordsconfigtypedef)
- [GuardrailManagedWordsTypeDef](./type_defs.md#guardrailmanagedwordstypedef)
- [GuardrailPiiEntityConfigTypeDef](./type_defs.md#guardrailpiientityconfigtypedef)
- [GuardrailPiiEntityTypeDef](./type_defs.md#guardrailpiientitytypedef)
- [GuardrailRegexConfigTypeDef](./type_defs.md#guardrailregexconfigtypedef)
- [GuardrailRegexTypeDef](./type_defs.md#guardrailregextypedef)
- [GuardrailSummaryTypeDef](./type_defs.md#guardrailsummarytypedef)
- [GuardrailTopicConfigTypeDef](./type_defs.md#guardrailtopicconfigtypedef)
- [GuardrailTopicTypeDef](./type_defs.md#guardrailtopictypedef)
- [GuardrailWordConfigTypeDef](./type_defs.md#guardrailwordconfigtypedef)
- [GuardrailWordTypeDef](./type_defs.md#guardrailwordtypedef)
- [HumanEvaluationCustomMetricTypeDef](./type_defs.md#humanevaluationcustommetrictypedef)
- [HumanWorkflowConfigTypeDef](./type_defs.md#humanworkflowconfigtypedef)
- [ImportedModelSummaryTypeDef](./type_defs.md#importedmodelsummarytypedef)
- [InvocationLogSourceTypeDef](./type_defs.md#invocationlogsourcetypedef)
- [TextInferenceConfigOutputTypeDef](./type_defs.md#textinferenceconfigoutputtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ListFoundationModelsRequestRequestTypeDef](./type_defs.md#listfoundationmodelsrequestrequesttypedef)
- [ListGuardrailsRequestRequestTypeDef](./type_defs.md#listguardrailsrequestrequesttypedef)
- [ListInferenceProfilesRequestRequestTypeDef](./type_defs.md#listinferenceprofilesrequestrequesttypedef)
- [ListMarketplaceModelEndpointsRequestRequestTypeDef](./type_defs.md#listmarketplacemodelendpointsrequestrequesttypedef)
- [MarketplaceModelEndpointSummaryTypeDef](./type_defs.md#marketplacemodelendpointsummarytypedef)
- [ModelCustomizationJobSummaryTypeDef](./type_defs.md#modelcustomizationjobsummarytypedef)
- [ModelImportJobSummaryTypeDef](./type_defs.md#modelimportjobsummarytypedef)
- [ListPromptRoutersRequestRequestTypeDef](./type_defs.md#listpromptroutersrequestrequesttypedef)
- [ProvisionedModelSummaryTypeDef](./type_defs.md#provisionedmodelsummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [S3DataSourceTypeDef](./type_defs.md#s3datasourcetypedef)
- [ModelInvocationJobS3InputDataConfigTypeDef](./type_defs.md#modelinvocationjobs3inputdataconfigtypedef)
- [ModelInvocationJobS3OutputDataConfigTypeDef](./type_defs.md#modelinvocationjobs3outputdataconfigtypedef)
- [QueryTransformationConfigurationTypeDef](./type_defs.md#querytransformationconfigurationtypedef)
- [RegisterMarketplaceModelEndpointRequestRequestTypeDef](./type_defs.md#registermarketplacemodelendpointrequestrequesttypedef)
- [RequestMetadataBaseFiltersOutputTypeDef](./type_defs.md#requestmetadatabasefiltersoutputtypedef)
- [RequestMetadataBaseFiltersTypeDef](./type_defs.md#requestmetadatabasefilterstypedef)
- [StopEvaluationJobRequestRequestTypeDef](./type_defs.md#stopevaluationjobrequestrequesttypedef)
- [StopModelCustomizationJobRequestRequestTypeDef](./type_defs.md#stopmodelcustomizationjobrequestrequesttypedef)
- [StopModelInvocationJobRequestRequestTypeDef](./type_defs.md#stopmodelinvocationjobrequestrequesttypedef)
- [TextInferenceConfigTypeDef](./type_defs.md#textinferenceconfigtypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateProvisionedModelThroughputRequestRequestTypeDef](./type_defs.md#updateprovisionedmodelthroughputrequestrequesttypedef)
- [ValidatorTypeDef](./type_defs.md#validatortypedef)
- [BatchDeleteEvaluationJobResponseTypeDef](./type_defs.md#batchdeleteevaluationjobresponsetypedef)
- [CreateEvaluationJobResponseTypeDef](./type_defs.md#createevaluationjobresponsetypedef)
- [CreateGuardrailResponseTypeDef](./type_defs.md#createguardrailresponsetypedef)
- [CreateGuardrailVersionResponseTypeDef](./type_defs.md#createguardrailversionresponsetypedef)
- [CreateInferenceProfileResponseTypeDef](./type_defs.md#createinferenceprofileresponsetypedef)
- [CreateModelCopyJobResponseTypeDef](./type_defs.md#createmodelcopyjobresponsetypedef)
- [CreateModelCustomizationJobResponseTypeDef](./type_defs.md#createmodelcustomizationjobresponsetypedef)
- [CreateModelImportJobResponseTypeDef](./type_defs.md#createmodelimportjobresponsetypedef)
- [CreateModelInvocationJobResponseTypeDef](./type_defs.md#createmodelinvocationjobresponsetypedef)
- [CreateProvisionedModelThroughputResponseTypeDef](./type_defs.md#createprovisionedmodelthroughputresponsetypedef)
- [GetProvisionedModelThroughputResponseTypeDef](./type_defs.md#getprovisionedmodelthroughputresponsetypedef)
- [UpdateGuardrailResponseTypeDef](./type_defs.md#updateguardrailresponsetypedef)
- [EvaluatorModelConfigOutputTypeDef](./type_defs.md#evaluatormodelconfigoutputtypedef)
- [EvaluatorModelConfigTypeDef](./type_defs.md#evaluatormodelconfigtypedef)
- [ByteContentDocTypeDef](./type_defs.md#bytecontentdoctypedef)
- [CloudWatchConfigTypeDef](./type_defs.md#cloudwatchconfigtypedef)
- [CreateModelCopyJobRequestRequestTypeDef](./type_defs.md#createmodelcopyjobrequestrequesttypedef)
- [CreateProvisionedModelThroughputRequestRequestTypeDef](./type_defs.md#createprovisionedmodelthroughputrequestrequesttypedef)
- [GetModelCopyJobResponseTypeDef](./type_defs.md#getmodelcopyjobresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ModelCopyJobSummaryTypeDef](./type_defs.md#modelcopyjobsummarytypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateInferenceProfileRequestRequestTypeDef](./type_defs.md#createinferenceprofilerequestrequesttypedef)
- [ListCustomModelsResponseTypeDef](./type_defs.md#listcustommodelsresponsetypedef)
- [DistillationConfigTypeDef](./type_defs.md#distillationconfigtypedef)
- [EvaluationModelConfigTypeDef](./type_defs.md#evaluationmodelconfigtypedef)
- [EvaluationDatasetTypeDef](./type_defs.md#evaluationdatasettypedef)
- [ListEvaluationJobsResponseTypeDef](./type_defs.md#listevaluationjobsresponsetypedef)
- [ExternalSourceOutputTypeDef](./type_defs.md#externalsourceoutputtypedef)
- [RetrievalFilterOutputTypeDef](./type_defs.md#retrievalfilteroutputtypedef)
- [FilterAttributeUnionTypeDef](./type_defs.md#filterattributeuniontypedef)
- [FoundationModelDetailsTypeDef](./type_defs.md#foundationmodeldetailstypedef)
- [FoundationModelSummaryTypeDef](./type_defs.md#foundationmodelsummarytypedef)
- [GetInferenceProfileResponseTypeDef](./type_defs.md#getinferenceprofileresponsetypedef)
- [InferenceProfileSummaryTypeDef](./type_defs.md#inferenceprofilesummarytypedef)
- [SageMakerEndpointOutputTypeDef](./type_defs.md#sagemakerendpointoutputtypedef)
- [VpcConfigUnionTypeDef](./type_defs.md#vpcconfiguniontypedef)
- [GetPromptRouterResponseTypeDef](./type_defs.md#getpromptrouterresponsetypedef)
- [PromptRouterSummaryTypeDef](./type_defs.md#promptroutersummarytypedef)
- [GuardrailContentPolicyConfigTypeDef](./type_defs.md#guardrailcontentpolicyconfigtypedef)
- [GuardrailContentPolicyTypeDef](./type_defs.md#guardrailcontentpolicytypedef)
- [GuardrailContextualGroundingPolicyConfigTypeDef](./type_defs.md#guardrailcontextualgroundingpolicyconfigtypedef)
- [GuardrailContextualGroundingPolicyTypeDef](./type_defs.md#guardrailcontextualgroundingpolicytypedef)
- [GuardrailSensitiveInformationPolicyConfigTypeDef](./type_defs.md#guardrailsensitiveinformationpolicyconfigtypedef)
- [GuardrailSensitiveInformationPolicyTypeDef](./type_defs.md#guardrailsensitiveinformationpolicytypedef)
- [ListGuardrailsResponseTypeDef](./type_defs.md#listguardrailsresponsetypedef)
- [GuardrailTopicPolicyConfigTypeDef](./type_defs.md#guardrailtopicpolicyconfigtypedef)
- [GuardrailTopicPolicyTypeDef](./type_defs.md#guardrailtopicpolicytypedef)
- [GuardrailWordPolicyConfigTypeDef](./type_defs.md#guardrailwordpolicyconfigtypedef)
- [GuardrailWordPolicyTypeDef](./type_defs.md#guardrailwordpolicytypedef)
- [ListImportedModelsResponseTypeDef](./type_defs.md#listimportedmodelsresponsetypedef)
- [KbInferenceConfigOutputTypeDef](./type_defs.md#kbinferenceconfigoutputtypedef)
- [ListGuardrailsRequestListGuardrailsPaginateTypeDef](./type_defs.md#listguardrailsrequestlistguardrailspaginatetypedef)
- [ListInferenceProfilesRequestListInferenceProfilesPaginateTypeDef](./type_defs.md#listinferenceprofilesrequestlistinferenceprofilespaginatetypedef)
- [ListMarketplaceModelEndpointsRequestListMarketplaceModelEndpointsPaginateTypeDef](./type_defs.md#listmarketplacemodelendpointsrequestlistmarketplacemodelendpointspaginatetypedef)
- [ListPromptRoutersRequestListPromptRoutersPaginateTypeDef](./type_defs.md#listpromptroutersrequestlistpromptrouterspaginatetypedef)
- [ListCustomModelsRequestListCustomModelsPaginateTypeDef](./type_defs.md#listcustommodelsrequestlistcustommodelspaginatetypedef)
- [ListCustomModelsRequestRequestTypeDef](./type_defs.md#listcustommodelsrequestrequesttypedef)
- [ListEvaluationJobsRequestListEvaluationJobsPaginateTypeDef](./type_defs.md#listevaluationjobsrequestlistevaluationjobspaginatetypedef)
- [ListEvaluationJobsRequestRequestTypeDef](./type_defs.md#listevaluationjobsrequestrequesttypedef)
- [ListImportedModelsRequestListImportedModelsPaginateTypeDef](./type_defs.md#listimportedmodelsrequestlistimportedmodelspaginatetypedef)
- [ListImportedModelsRequestRequestTypeDef](./type_defs.md#listimportedmodelsrequestrequesttypedef)
- [ListModelCopyJobsRequestListModelCopyJobsPaginateTypeDef](./type_defs.md#listmodelcopyjobsrequestlistmodelcopyjobspaginatetypedef)
- [ListModelCopyJobsRequestRequestTypeDef](./type_defs.md#listmodelcopyjobsrequestrequesttypedef)
- [ListModelCustomizationJobsRequestListModelCustomizationJobsPaginateTypeDef](./type_defs.md#listmodelcustomizationjobsrequestlistmodelcustomizationjobspaginatetypedef)
- [ListModelCustomizationJobsRequestRequestTypeDef](./type_defs.md#listmodelcustomizationjobsrequestrequesttypedef)
- [ListModelImportJobsRequestListModelImportJobsPaginateTypeDef](./type_defs.md#listmodelimportjobsrequestlistmodelimportjobspaginatetypedef)
- [ListModelImportJobsRequestRequestTypeDef](./type_defs.md#listmodelimportjobsrequestrequesttypedef)
- [ListModelInvocationJobsRequestListModelInvocationJobsPaginateTypeDef](./type_defs.md#listmodelinvocationjobsrequestlistmodelinvocationjobspaginatetypedef)
- [ListModelInvocationJobsRequestRequestTypeDef](./type_defs.md#listmodelinvocationjobsrequestrequesttypedef)
- [ListProvisionedModelThroughputsRequestListProvisionedModelThroughputsPaginateTypeDef](./type_defs.md#listprovisionedmodelthroughputsrequestlistprovisionedmodelthroughputspaginatetypedef)
- [ListProvisionedModelThroughputsRequestRequestTypeDef](./type_defs.md#listprovisionedmodelthroughputsrequestrequesttypedef)
- [ListMarketplaceModelEndpointsResponseTypeDef](./type_defs.md#listmarketplacemodelendpointsresponsetypedef)
- [ListModelCustomizationJobsResponseTypeDef](./type_defs.md#listmodelcustomizationjobsresponsetypedef)
- [ListModelImportJobsResponseTypeDef](./type_defs.md#listmodelimportjobsresponsetypedef)
- [ListProvisionedModelThroughputsResponseTypeDef](./type_defs.md#listprovisionedmodelthroughputsresponsetypedef)
- [ModelDataSourceTypeDef](./type_defs.md#modeldatasourcetypedef)
- [ModelInvocationJobInputDataConfigTypeDef](./type_defs.md#modelinvocationjobinputdataconfigtypedef)
- [ModelInvocationJobOutputDataConfigTypeDef](./type_defs.md#modelinvocationjoboutputdataconfigtypedef)
- [OrchestrationConfigurationTypeDef](./type_defs.md#orchestrationconfigurationtypedef)
- [RequestMetadataFiltersOutputTypeDef](./type_defs.md#requestmetadatafiltersoutputtypedef)
- [RequestMetadataBaseFiltersUnionTypeDef](./type_defs.md#requestmetadatabasefiltersuniontypedef)
- [TextInferenceConfigUnionTypeDef](./type_defs.md#textinferenceconfiguniontypedef)
- [ValidationDataConfigOutputTypeDef](./type_defs.md#validationdataconfigoutputtypedef)
- [ValidationDataConfigTypeDef](./type_defs.md#validationdataconfigtypedef)
- [EvaluatorModelConfigUnionTypeDef](./type_defs.md#evaluatormodelconfiguniontypedef)
- [ByteContentDocUnionTypeDef](./type_defs.md#bytecontentdocuniontypedef)
- [LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef)
- [ListModelCopyJobsResponseTypeDef](./type_defs.md#listmodelcopyjobsresponsetypedef)
- [CustomizationConfigTypeDef](./type_defs.md#customizationconfigtypedef)
- [EvaluationDatasetMetricConfigOutputTypeDef](./type_defs.md#evaluationdatasetmetricconfigoutputtypedef)
- [EvaluationDatasetMetricConfigTypeDef](./type_defs.md#evaluationdatasetmetricconfigtypedef)
- [KnowledgeBaseVectorSearchConfigurationOutputTypeDef](./type_defs.md#knowledgebasevectorsearchconfigurationoutputtypedef)
- [RetrievalFilterTypeDef](./type_defs.md#retrievalfiltertypedef)
- [GetFoundationModelResponseTypeDef](./type_defs.md#getfoundationmodelresponsetypedef)
- [ListFoundationModelsResponseTypeDef](./type_defs.md#listfoundationmodelsresponsetypedef)
- [ListInferenceProfilesResponseTypeDef](./type_defs.md#listinferenceprofilesresponsetypedef)
- [EndpointConfigOutputTypeDef](./type_defs.md#endpointconfigoutputtypedef)
- [SageMakerEndpointTypeDef](./type_defs.md#sagemakerendpointtypedef)
- [ListPromptRoutersResponseTypeDef](./type_defs.md#listpromptroutersresponsetypedef)
- [CreateGuardrailRequestRequestTypeDef](./type_defs.md#createguardrailrequestrequesttypedef)
- [UpdateGuardrailRequestRequestTypeDef](./type_defs.md#updateguardrailrequestrequesttypedef)
- [GetGuardrailResponseTypeDef](./type_defs.md#getguardrailresponsetypedef)
- [ExternalSourcesGenerationConfigurationOutputTypeDef](./type_defs.md#externalsourcesgenerationconfigurationoutputtypedef)
- [GenerationConfigurationOutputTypeDef](./type_defs.md#generationconfigurationoutputtypedef)
- [CreateModelImportJobRequestRequestTypeDef](./type_defs.md#createmodelimportjobrequestrequesttypedef)
- [GetImportedModelResponseTypeDef](./type_defs.md#getimportedmodelresponsetypedef)
- [GetModelImportJobResponseTypeDef](./type_defs.md#getmodelimportjobresponsetypedef)
- [CreateModelInvocationJobRequestRequestTypeDef](./type_defs.md#createmodelinvocationjobrequestrequesttypedef)
- [GetModelInvocationJobResponseTypeDef](./type_defs.md#getmodelinvocationjobresponsetypedef)
- [ModelInvocationJobSummaryTypeDef](./type_defs.md#modelinvocationjobsummarytypedef)
- [InvocationLogsConfigOutputTypeDef](./type_defs.md#invocationlogsconfigoutputtypedef)
- [RequestMetadataFiltersTypeDef](./type_defs.md#requestmetadatafilterstypedef)
- [KbInferenceConfigTypeDef](./type_defs.md#kbinferenceconfigtypedef)
- [ExternalSourceTypeDef](./type_defs.md#externalsourcetypedef)
- [GetModelInvocationLoggingConfigurationResponseTypeDef](./type_defs.md#getmodelinvocationloggingconfigurationresponsetypedef)
- [PutModelInvocationLoggingConfigurationRequestRequestTypeDef](./type_defs.md#putmodelinvocationloggingconfigurationrequestrequesttypedef)
- [AutomatedEvaluationConfigOutputTypeDef](./type_defs.md#automatedevaluationconfigoutputtypedef)
- [HumanEvaluationConfigOutputTypeDef](./type_defs.md#humanevaluationconfigoutputtypedef)
- [EvaluationDatasetMetricConfigUnionTypeDef](./type_defs.md#evaluationdatasetmetricconfiguniontypedef)
- [HumanEvaluationConfigTypeDef](./type_defs.md#humanevaluationconfigtypedef)
- [KnowledgeBaseRetrievalConfigurationOutputTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationoutputtypedef)
- [RetrievalFilterUnionTypeDef](./type_defs.md#retrievalfilteruniontypedef)
- [MarketplaceModelEndpointTypeDef](./type_defs.md#marketplacemodelendpointtypedef)
- [SageMakerEndpointUnionTypeDef](./type_defs.md#sagemakerendpointuniontypedef)
- [ExternalSourcesRetrieveAndGenerateConfigurationOutputTypeDef](./type_defs.md#externalsourcesretrieveandgenerateconfigurationoutputtypedef)
- [ListModelInvocationJobsResponseTypeDef](./type_defs.md#listmodelinvocationjobsresponsetypedef)
- [TrainingDataConfigOutputTypeDef](./type_defs.md#trainingdataconfigoutputtypedef)
- [RequestMetadataFiltersUnionTypeDef](./type_defs.md#requestmetadatafiltersuniontypedef)
- [KbInferenceConfigUnionTypeDef](./type_defs.md#kbinferenceconfiguniontypedef)
- [ExternalSourceUnionTypeDef](./type_defs.md#externalsourceuniontypedef)
- [EvaluationConfigOutputTypeDef](./type_defs.md#evaluationconfigoutputtypedef)
- [AutomatedEvaluationConfigTypeDef](./type_defs.md#automatedevaluationconfigtypedef)
- [HumanEvaluationConfigUnionTypeDef](./type_defs.md#humanevaluationconfiguniontypedef)
- [KnowledgeBaseRetrieveAndGenerateConfigurationOutputTypeDef](./type_defs.md#knowledgebaseretrieveandgenerateconfigurationoutputtypedef)
- [RetrieveConfigOutputTypeDef](./type_defs.md#retrieveconfigoutputtypedef)
- [KnowledgeBaseVectorSearchConfigurationTypeDef](./type_defs.md#knowledgebasevectorsearchconfigurationtypedef)
- [CreateMarketplaceModelEndpointResponseTypeDef](./type_defs.md#createmarketplacemodelendpointresponsetypedef)
- [GetMarketplaceModelEndpointResponseTypeDef](./type_defs.md#getmarketplacemodelendpointresponsetypedef)
- [RegisterMarketplaceModelEndpointResponseTypeDef](./type_defs.md#registermarketplacemodelendpointresponsetypedef)
- [UpdateMarketplaceModelEndpointResponseTypeDef](./type_defs.md#updatemarketplacemodelendpointresponsetypedef)
- [EndpointConfigTypeDef](./type_defs.md#endpointconfigtypedef)
- [GetCustomModelResponseTypeDef](./type_defs.md#getcustommodelresponsetypedef)
- [GetModelCustomizationJobResponseTypeDef](./type_defs.md#getmodelcustomizationjobresponsetypedef)
- [InvocationLogsConfigTypeDef](./type_defs.md#invocationlogsconfigtypedef)
- [ExternalSourcesGenerationConfigurationTypeDef](./type_defs.md#externalsourcesgenerationconfigurationtypedef)
- [GenerationConfigurationTypeDef](./type_defs.md#generationconfigurationtypedef)
- [AutomatedEvaluationConfigUnionTypeDef](./type_defs.md#automatedevaluationconfiguniontypedef)
- [RetrieveAndGenerateConfigurationOutputTypeDef](./type_defs.md#retrieveandgenerateconfigurationoutputtypedef)
- [KnowledgeBaseVectorSearchConfigurationUnionTypeDef](./type_defs.md#knowledgebasevectorsearchconfigurationuniontypedef)
- [CreateMarketplaceModelEndpointRequestRequestTypeDef](./type_defs.md#createmarketplacemodelendpointrequestrequesttypedef)
- [UpdateMarketplaceModelEndpointRequestRequestTypeDef](./type_defs.md#updatemarketplacemodelendpointrequestrequesttypedef)
- [InvocationLogsConfigUnionTypeDef](./type_defs.md#invocationlogsconfiguniontypedef)
- [ExternalSourcesGenerationConfigurationUnionTypeDef](./type_defs.md#externalsourcesgenerationconfigurationuniontypedef)
- [GenerationConfigurationUnionTypeDef](./type_defs.md#generationconfigurationuniontypedef)
- [EvaluationConfigTypeDef](./type_defs.md#evaluationconfigtypedef)
- [KnowledgeBaseConfigOutputTypeDef](./type_defs.md#knowledgebaseconfigoutputtypedef)
- [KnowledgeBaseRetrievalConfigurationTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationtypedef)
- [TrainingDataConfigTypeDef](./type_defs.md#trainingdataconfigtypedef)
- [ExternalSourcesRetrieveAndGenerateConfigurationTypeDef](./type_defs.md#externalsourcesretrieveandgenerateconfigurationtypedef)
- [RAGConfigOutputTypeDef](./type_defs.md#ragconfigoutputtypedef)
- [KnowledgeBaseRetrievalConfigurationUnionTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationuniontypedef)
- [CreateModelCustomizationJobRequestRequestTypeDef](./type_defs.md#createmodelcustomizationjobrequestrequesttypedef)
- [ExternalSourcesRetrieveAndGenerateConfigurationUnionTypeDef](./type_defs.md#externalsourcesretrieveandgenerateconfigurationuniontypedef)
- [EvaluationInferenceConfigOutputTypeDef](./type_defs.md#evaluationinferenceconfigoutputtypedef)
- [KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef](./type_defs.md#knowledgebaseretrieveandgenerateconfigurationtypedef)
- [RetrieveConfigTypeDef](./type_defs.md#retrieveconfigtypedef)
- [GetEvaluationJobResponseTypeDef](./type_defs.md#getevaluationjobresponsetypedef)
- [KnowledgeBaseRetrieveAndGenerateConfigurationUnionTypeDef](./type_defs.md#knowledgebaseretrieveandgenerateconfigurationuniontypedef)
- [RetrieveConfigUnionTypeDef](./type_defs.md#retrieveconfiguniontypedef)
- [RetrieveAndGenerateConfigurationTypeDef](./type_defs.md#retrieveandgenerateconfigurationtypedef)
- [RetrieveAndGenerateConfigurationUnionTypeDef](./type_defs.md#retrieveandgenerateconfigurationuniontypedef)
- [KnowledgeBaseConfigTypeDef](./type_defs.md#knowledgebaseconfigtypedef)
- [KnowledgeBaseConfigUnionTypeDef](./type_defs.md#knowledgebaseconfiguniontypedef)
- [RAGConfigTypeDef](./type_defs.md#ragconfigtypedef)
- [RAGConfigUnionTypeDef](./type_defs.md#ragconfiguniontypedef)
- [EvaluationInferenceConfigTypeDef](./type_defs.md#evaluationinferenceconfigtypedef)
- [CreateEvaluationJobRequestRequestTypeDef](./type_defs.md#createevaluationjobrequestrequesttypedef)

