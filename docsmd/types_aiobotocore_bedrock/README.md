# Bedrock module

> [Index](../README.md) > Bedrock


!!! note ""

    Auto-generated documentation for [Bedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#bedrock)
    type annotations stubs module [types-aiobotocore-bedrock](https://pypi.org/project/types-aiobotocore-bedrock/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.23.2' mypy-boto3-builder`
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
# ListCustomModelDeploymentsPaginator usage example

from types_aiobotocore_bedrock.paginator import ListCustomModelDeploymentsPaginator

def get_list_custom_model_deployments_paginator() -> ListCustomModelDeploymentsPaginator:
    return client.get_paginator("list_custom_model_deployments"))
```

- [ListCustomModelDeploymentsPaginator](./paginators.md#listcustommodeldeploymentspaginator)
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
# AgreementStatusType usage example

from types_aiobotocore_bedrock.literals import AgreementStatusType

def get_value() -> AgreementStatusType:
    return "AVAILABLE"
```

- [AgreementStatusType](./literals.md#agreementstatustype)
- [ApplicationTypeType](./literals.md#applicationtypetype)
- [AttributeTypeType](./literals.md#attributetypetype)
- [AuthorizationStatusType](./literals.md#authorizationstatustype)
- [CommitmentDurationType](./literals.md#commitmentdurationtype)
- [CustomModelDeploymentStatusType](./literals.md#custommodeldeploymentstatustype)
- [CustomizationTypeType](./literals.md#customizationtypetype)
- [EntitlementAvailabilityType](./literals.md#entitlementavailabilitytype)
- [EvaluationJobStatusType](./literals.md#evaluationjobstatustype)
- [EvaluationJobTypeType](./literals.md#evaluationjobtypetype)
- [EvaluationTaskTypeType](./literals.md#evaluationtasktypetype)
- [ExternalSourceTypeType](./literals.md#externalsourcetypetype)
- [FineTuningJobStatusType](./literals.md#finetuningjobstatustype)
- [FoundationModelLifecycleStatusType](./literals.md#foundationmodellifecyclestatustype)
- [GuardrailContentFilterActionType](./literals.md#guardrailcontentfilteractiontype)
- [GuardrailContentFilterTypeType](./literals.md#guardrailcontentfiltertypetype)
- [GuardrailContentFiltersTierNameType](./literals.md#guardrailcontentfilterstiernametype)
- [GuardrailContextualGroundingActionType](./literals.md#guardrailcontextualgroundingactiontype)
- [GuardrailContextualGroundingFilterTypeType](./literals.md#guardrailcontextualgroundingfiltertypetype)
- [GuardrailFilterStrengthType](./literals.md#guardrailfilterstrengthtype)
- [GuardrailManagedWordsTypeType](./literals.md#guardrailmanagedwordstypetype)
- [GuardrailModalityType](./literals.md#guardrailmodalitytype)
- [GuardrailPiiEntityTypeType](./literals.md#guardrailpiientitytypetype)
- [GuardrailSensitiveInformationActionType](./literals.md#guardrailsensitiveinformationactiontype)
- [GuardrailStatusType](./literals.md#guardrailstatustype)
- [GuardrailTopicActionType](./literals.md#guardrailtopicactiontype)
- [GuardrailTopicTypeType](./literals.md#guardrailtopictypetype)
- [GuardrailTopicsTierNameType](./literals.md#guardrailtopicstiernametype)
- [GuardrailWordActionType](./literals.md#guardrailwordactiontype)
- [InferenceProfileStatusType](./literals.md#inferenceprofilestatustype)
- [InferenceProfileTypeType](./literals.md#inferenceprofiletypetype)
- [InferenceTypeType](./literals.md#inferencetypetype)
- [JobStatusDetailsType](./literals.md#jobstatusdetailstype)
- [ListCustomModelDeploymentsPaginatorName](./literals.md#listcustommodeldeploymentspaginatorname)
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
- [ModelStatusType](./literals.md#modelstatustype)
- [OfferTypeType](./literals.md#offertypetype)
- [PerformanceConfigLatencyType](./literals.md#performanceconfiglatencytype)
- [PromptRouterStatusType](./literals.md#promptrouterstatustype)
- [PromptRouterTypeType](./literals.md#promptroutertypetype)
- [ProvisionedModelStatusType](./literals.md#provisionedmodelstatustype)
- [QueryTransformationTypeType](./literals.md#querytransformationtypetype)
- [RegionAvailabilityType](./literals.md#regionavailabilitytype)
- [RerankingMetadataSelectionModeType](./literals.md#rerankingmetadataselectionmodetype)
- [RetrieveAndGenerateTypeType](./literals.md#retrieveandgeneratetypetype)
- [S3InputFormatType](./literals.md#s3inputformattype)
- [SearchTypeType](./literals.md#searchtypetype)
- [SortByProvisionedModelsType](./literals.md#sortbyprovisionedmodelstype)
- [SortJobsByType](./literals.md#sortjobsbytype)
- [SortModelsByType](./literals.md#sortmodelsbytype)
- [SortOrderType](./literals.md#sortordertype)
- [StatusType](./literals.md#statustype)
- [VectorSearchRerankingConfigurationTypeType](./literals.md#vectorsearchrerankingconfigurationtypetype)
- [BedrockServiceName](./literals.md#bedrockservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AgreementAvailabilityTypeDef](./type_defs.md#agreementavailabilitytypedef)
- [BatchDeleteEvaluationJobErrorTypeDef](./type_defs.md#batchdeleteevaluationjoberrortypedef)
- [BatchDeleteEvaluationJobItemTypeDef](./type_defs.md#batchdeleteevaluationjobitemtypedef)
- [BatchDeleteEvaluationJobRequestTypeDef](./type_defs.md#batchdeleteevaluationjobrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BedrockEvaluatorModelTypeDef](./type_defs.md#bedrockevaluatormodeltypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [ByteContentDocOutputTypeDef](./type_defs.md#bytecontentdocoutputtypedef)
- [S3ConfigTypeDef](./type_defs.md#s3configtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [EvaluationOutputDataConfigTypeDef](./type_defs.md#evaluationoutputdataconfigtypedef)
- [CreateFoundationModelAgreementRequestTypeDef](./type_defs.md#createfoundationmodelagreementrequesttypedef)
- [GuardrailCrossRegionConfigTypeDef](./type_defs.md#guardrailcrossregionconfigtypedef)
- [CreateGuardrailVersionRequestTypeDef](./type_defs.md#createguardrailversionrequesttypedef)
- [InferenceProfileModelSourceTypeDef](./type_defs.md#inferenceprofilemodelsourcetypedef)
- [OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef)
- [PromptRouterTargetModelTypeDef](./type_defs.md#promptroutertargetmodeltypedef)
- [RoutingCriteriaTypeDef](./type_defs.md#routingcriteriatypedef)
- [CustomMetricBedrockEvaluatorModelTypeDef](./type_defs.md#custommetricbedrockevaluatormodeltypedef)
- [CustomModelDeploymentSummaryTypeDef](./type_defs.md#custommodeldeploymentsummarytypedef)
- [CustomModelSummaryTypeDef](./type_defs.md#custommodelsummarytypedef)
- [CustomModelUnitsTypeDef](./type_defs.md#custommodelunitstypedef)
- [DataProcessingDetailsTypeDef](./type_defs.md#dataprocessingdetailstypedef)
- [DeleteCustomModelDeploymentRequestTypeDef](./type_defs.md#deletecustommodeldeploymentrequesttypedef)
- [DeleteCustomModelRequestTypeDef](./type_defs.md#deletecustommodelrequesttypedef)
- [DeleteFoundationModelAgreementRequestTypeDef](./type_defs.md#deletefoundationmodelagreementrequesttypedef)
- [DeleteGuardrailRequestTypeDef](./type_defs.md#deleteguardrailrequesttypedef)
- [DeleteImportedModelRequestTypeDef](./type_defs.md#deleteimportedmodelrequesttypedef)
- [DeleteInferenceProfileRequestTypeDef](./type_defs.md#deleteinferenceprofilerequesttypedef)
- [DeleteMarketplaceModelEndpointRequestTypeDef](./type_defs.md#deletemarketplacemodelendpointrequesttypedef)
- [DeletePromptRouterRequestTypeDef](./type_defs.md#deletepromptrouterrequesttypedef)
- [DeleteProvisionedModelThroughputRequestTypeDef](./type_defs.md#deleteprovisionedmodelthroughputrequesttypedef)
- [DeregisterMarketplaceModelEndpointRequestTypeDef](./type_defs.md#deregistermarketplacemodelendpointrequesttypedef)
- [DimensionalPriceRateTypeDef](./type_defs.md#dimensionalpriceratetypedef)
- [TeacherModelConfigTypeDef](./type_defs.md#teachermodelconfigtypedef)
- [PerformanceConfigurationTypeDef](./type_defs.md#performanceconfigurationtypedef)
- [EvaluationDatasetLocationTypeDef](./type_defs.md#evaluationdatasetlocationtypedef)
- [EvaluationModelConfigSummaryTypeDef](./type_defs.md#evaluationmodelconfigsummarytypedef)
- [EvaluationRagConfigSummaryTypeDef](./type_defs.md#evaluationragconfigsummarytypedef)
- [EvaluationPrecomputedInferenceSourceTypeDef](./type_defs.md#evaluationprecomputedinferencesourcetypedef)
- [EvaluationPrecomputedRetrieveAndGenerateSourceConfigTypeDef](./type_defs.md#evaluationprecomputedretrieveandgeneratesourceconfigtypedef)
- [EvaluationPrecomputedRetrieveSourceConfigTypeDef](./type_defs.md#evaluationprecomputedretrievesourceconfigtypedef)
- [S3ObjectDocTypeDef](./type_defs.md#s3objectdoctypedef)
- [GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef)
- [PromptTemplateTypeDef](./type_defs.md#prompttemplatetypedef)
- [FieldForRerankingTypeDef](./type_defs.md#fieldforrerankingtypedef)
- [FilterAttributeOutputTypeDef](./type_defs.md#filterattributeoutputtypedef)
- [FilterAttributeTypeDef](./type_defs.md#filterattributetypedef)
- [FoundationModelLifecycleTypeDef](./type_defs.md#foundationmodellifecycletypedef)
- [GetCustomModelDeploymentRequestTypeDef](./type_defs.md#getcustommodeldeploymentrequesttypedef)
- [GetCustomModelRequestTypeDef](./type_defs.md#getcustommodelrequesttypedef)
- [TrainingMetricsTypeDef](./type_defs.md#trainingmetricstypedef)
- [ValidatorMetricTypeDef](./type_defs.md#validatormetrictypedef)
- [GetEvaluationJobRequestTypeDef](./type_defs.md#getevaluationjobrequesttypedef)
- [GetFoundationModelAvailabilityRequestTypeDef](./type_defs.md#getfoundationmodelavailabilityrequesttypedef)
- [GetFoundationModelRequestTypeDef](./type_defs.md#getfoundationmodelrequesttypedef)
- [GetGuardrailRequestTypeDef](./type_defs.md#getguardrailrequesttypedef)
- [GuardrailCrossRegionDetailsTypeDef](./type_defs.md#guardrailcrossregiondetailstypedef)
- [GetImportedModelRequestTypeDef](./type_defs.md#getimportedmodelrequesttypedef)
- [GetInferenceProfileRequestTypeDef](./type_defs.md#getinferenceprofilerequesttypedef)
- [InferenceProfileModelTypeDef](./type_defs.md#inferenceprofilemodeltypedef)
- [GetMarketplaceModelEndpointRequestTypeDef](./type_defs.md#getmarketplacemodelendpointrequesttypedef)
- [GetModelCopyJobRequestTypeDef](./type_defs.md#getmodelcopyjobrequesttypedef)
- [GetModelCustomizationJobRequestTypeDef](./type_defs.md#getmodelcustomizationjobrequesttypedef)
- [VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef)
- [GetModelImportJobRequestTypeDef](./type_defs.md#getmodelimportjobrequesttypedef)
- [GetModelInvocationJobRequestTypeDef](./type_defs.md#getmodelinvocationjobrequesttypedef)
- [GetPromptRouterRequestTypeDef](./type_defs.md#getpromptrouterrequesttypedef)
- [GetProvisionedModelThroughputRequestTypeDef](./type_defs.md#getprovisionedmodelthroughputrequesttypedef)
- [GuardrailContentFilterConfigTypeDef](./type_defs.md#guardrailcontentfilterconfigtypedef)
- [GuardrailContentFilterTypeDef](./type_defs.md#guardrailcontentfiltertypedef)
- [GuardrailContentFiltersTierConfigTypeDef](./type_defs.md#guardrailcontentfilterstierconfigtypedef)
- [GuardrailContentFiltersTierTypeDef](./type_defs.md#guardrailcontentfilterstiertypedef)
- [GuardrailContextualGroundingFilterConfigTypeDef](./type_defs.md#guardrailcontextualgroundingfilterconfigtypedef)
- [GuardrailContextualGroundingFilterTypeDef](./type_defs.md#guardrailcontextualgroundingfiltertypedef)
- [GuardrailManagedWordsConfigTypeDef](./type_defs.md#guardrailmanagedwordsconfigtypedef)
- [GuardrailManagedWordsTypeDef](./type_defs.md#guardrailmanagedwordstypedef)
- [GuardrailPiiEntityConfigTypeDef](./type_defs.md#guardrailpiientityconfigtypedef)
- [GuardrailPiiEntityTypeDef](./type_defs.md#guardrailpiientitytypedef)
- [GuardrailRegexConfigTypeDef](./type_defs.md#guardrailregexconfigtypedef)
- [GuardrailRegexTypeDef](./type_defs.md#guardrailregextypedef)
- [GuardrailTopicConfigTypeDef](./type_defs.md#guardrailtopicconfigtypedef)
- [GuardrailTopicsTierConfigTypeDef](./type_defs.md#guardrailtopicstierconfigtypedef)
- [GuardrailTopicTypeDef](./type_defs.md#guardrailtopictypedef)
- [GuardrailTopicsTierTypeDef](./type_defs.md#guardrailtopicstiertypedef)
- [GuardrailWordConfigTypeDef](./type_defs.md#guardrailwordconfigtypedef)
- [GuardrailWordTypeDef](./type_defs.md#guardrailwordtypedef)
- [HumanEvaluationCustomMetricTypeDef](./type_defs.md#humanevaluationcustommetrictypedef)
- [HumanWorkflowConfigTypeDef](./type_defs.md#humanworkflowconfigtypedef)
- [MetadataAttributeSchemaTypeDef](./type_defs.md#metadataattributeschematypedef)
- [ImportedModelSummaryTypeDef](./type_defs.md#importedmodelsummarytypedef)
- [InvocationLogSourceTypeDef](./type_defs.md#invocationlogsourcetypedef)
- [TextInferenceConfigOutputTypeDef](./type_defs.md#textinferenceconfigoutputtypedef)
- [TextInferenceConfigTypeDef](./type_defs.md#textinferenceconfigtypedef)
- [LegalTermTypeDef](./type_defs.md#legaltermtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ListFoundationModelAgreementOffersRequestTypeDef](./type_defs.md#listfoundationmodelagreementoffersrequesttypedef)
- [ListFoundationModelsRequestTypeDef](./type_defs.md#listfoundationmodelsrequesttypedef)
- [ListGuardrailsRequestTypeDef](./type_defs.md#listguardrailsrequesttypedef)
- [ListInferenceProfilesRequestTypeDef](./type_defs.md#listinferenceprofilesrequesttypedef)
- [ListMarketplaceModelEndpointsRequestTypeDef](./type_defs.md#listmarketplacemodelendpointsrequesttypedef)
- [MarketplaceModelEndpointSummaryTypeDef](./type_defs.md#marketplacemodelendpointsummarytypedef)
- [ModelImportJobSummaryTypeDef](./type_defs.md#modelimportjobsummarytypedef)
- [ListPromptRoutersRequestTypeDef](./type_defs.md#listpromptroutersrequesttypedef)
- [ProvisionedModelSummaryTypeDef](./type_defs.md#provisionedmodelsummarytypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [S3DataSourceTypeDef](./type_defs.md#s3datasourcetypedef)
- [ModelInvocationJobS3InputDataConfigTypeDef](./type_defs.md#modelinvocationjobs3inputdataconfigtypedef)
- [ModelInvocationJobS3OutputDataConfigTypeDef](./type_defs.md#modelinvocationjobs3outputdataconfigtypedef)
- [QueryTransformationConfigurationTypeDef](./type_defs.md#querytransformationconfigurationtypedef)
- [RatingScaleItemValueTypeDef](./type_defs.md#ratingscaleitemvaluetypedef)
- [RegisterMarketplaceModelEndpointRequestTypeDef](./type_defs.md#registermarketplacemodelendpointrequesttypedef)
- [RequestMetadataBaseFiltersOutputTypeDef](./type_defs.md#requestmetadatabasefiltersoutputtypedef)
- [RequestMetadataBaseFiltersTypeDef](./type_defs.md#requestmetadatabasefilterstypedef)
- [VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef)
- [TrainingDetailsTypeDef](./type_defs.md#trainingdetailstypedef)
- [ValidationDetailsTypeDef](./type_defs.md#validationdetailstypedef)
- [StopEvaluationJobRequestTypeDef](./type_defs.md#stopevaluationjobrequesttypedef)
- [StopModelCustomizationJobRequestTypeDef](./type_defs.md#stopmodelcustomizationjobrequesttypedef)
- [StopModelInvocationJobRequestTypeDef](./type_defs.md#stopmodelinvocationjobrequesttypedef)
- [SupportTermTypeDef](./type_defs.md#supporttermtypedef)
- [ValidityTermTypeDef](./type_defs.md#validitytermtypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateProvisionedModelThroughputRequestTypeDef](./type_defs.md#updateprovisionedmodelthroughputrequesttypedef)
- [ValidatorTypeDef](./type_defs.md#validatortypedef)
- [VectorSearchBedrockRerankingModelConfigurationOutputTypeDef](./type_defs.md#vectorsearchbedrockrerankingmodelconfigurationoutputtypedef)
- [VectorSearchBedrockRerankingModelConfigurationTypeDef](./type_defs.md#vectorsearchbedrockrerankingmodelconfigurationtypedef)
- [BatchDeleteEvaluationJobResponseTypeDef](./type_defs.md#batchdeleteevaluationjobresponsetypedef)
- [CreateCustomModelDeploymentResponseTypeDef](./type_defs.md#createcustommodeldeploymentresponsetypedef)
- [CreateCustomModelResponseTypeDef](./type_defs.md#createcustommodelresponsetypedef)
- [CreateEvaluationJobResponseTypeDef](./type_defs.md#createevaluationjobresponsetypedef)
- [CreateFoundationModelAgreementResponseTypeDef](./type_defs.md#createfoundationmodelagreementresponsetypedef)
- [CreateGuardrailResponseTypeDef](./type_defs.md#createguardrailresponsetypedef)
- [CreateGuardrailVersionResponseTypeDef](./type_defs.md#createguardrailversionresponsetypedef)
- [CreateInferenceProfileResponseTypeDef](./type_defs.md#createinferenceprofileresponsetypedef)
- [CreateModelCopyJobResponseTypeDef](./type_defs.md#createmodelcopyjobresponsetypedef)
- [CreateModelCustomizationJobResponseTypeDef](./type_defs.md#createmodelcustomizationjobresponsetypedef)
- [CreateModelImportJobResponseTypeDef](./type_defs.md#createmodelimportjobresponsetypedef)
- [CreateModelInvocationJobResponseTypeDef](./type_defs.md#createmodelinvocationjobresponsetypedef)
- [CreatePromptRouterResponseTypeDef](./type_defs.md#createpromptrouterresponsetypedef)
- [CreateProvisionedModelThroughputResponseTypeDef](./type_defs.md#createprovisionedmodelthroughputresponsetypedef)
- [GetCustomModelDeploymentResponseTypeDef](./type_defs.md#getcustommodeldeploymentresponsetypedef)
- [GetFoundationModelAvailabilityResponseTypeDef](./type_defs.md#getfoundationmodelavailabilityresponsetypedef)
- [GetProvisionedModelThroughputResponseTypeDef](./type_defs.md#getprovisionedmodelthroughputresponsetypedef)
- [GetUseCaseForModelAccessResponseTypeDef](./type_defs.md#getusecaseformodelaccessresponsetypedef)
- [UpdateGuardrailResponseTypeDef](./type_defs.md#updateguardrailresponsetypedef)
- [EvaluatorModelConfigOutputTypeDef](./type_defs.md#evaluatormodelconfigoutputtypedef)
- [EvaluatorModelConfigTypeDef](./type_defs.md#evaluatormodelconfigtypedef)
- [ByteContentDocTypeDef](./type_defs.md#bytecontentdoctypedef)
- [PutUseCaseForModelAccessRequestTypeDef](./type_defs.md#putusecaseformodelaccessrequesttypedef)
- [CloudWatchConfigTypeDef](./type_defs.md#cloudwatchconfigtypedef)
- [CreateCustomModelDeploymentRequestTypeDef](./type_defs.md#createcustommodeldeploymentrequesttypedef)
- [CreateModelCopyJobRequestTypeDef](./type_defs.md#createmodelcopyjobrequesttypedef)
- [CreateProvisionedModelThroughputRequestTypeDef](./type_defs.md#createprovisionedmodelthroughputrequesttypedef)
- [GetModelCopyJobResponseTypeDef](./type_defs.md#getmodelcopyjobresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ModelCopyJobSummaryTypeDef](./type_defs.md#modelcopyjobsummarytypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [CreateInferenceProfileRequestTypeDef](./type_defs.md#createinferenceprofilerequesttypedef)
- [CreatePromptRouterRequestTypeDef](./type_defs.md#createpromptrouterrequesttypedef)
- [GetPromptRouterResponseTypeDef](./type_defs.md#getpromptrouterresponsetypedef)
- [PromptRouterSummaryTypeDef](./type_defs.md#promptroutersummarytypedef)
- [CustomMetricEvaluatorModelConfigOutputTypeDef](./type_defs.md#custommetricevaluatormodelconfigoutputtypedef)
- [CustomMetricEvaluatorModelConfigTypeDef](./type_defs.md#custommetricevaluatormodelconfigtypedef)
- [ListCustomModelDeploymentsResponseTypeDef](./type_defs.md#listcustommodeldeploymentsresponsetypedef)
- [ListCustomModelsResponseTypeDef](./type_defs.md#listcustommodelsresponsetypedef)
- [PricingTermTypeDef](./type_defs.md#pricingtermtypedef)
- [DistillationConfigTypeDef](./type_defs.md#distillationconfigtypedef)
- [EvaluationBedrockModelTypeDef](./type_defs.md#evaluationbedrockmodeltypedef)
- [EvaluationDatasetTypeDef](./type_defs.md#evaluationdatasettypedef)
- [EvaluationInferenceConfigSummaryTypeDef](./type_defs.md#evaluationinferenceconfigsummarytypedef)
- [EvaluationPrecomputedRagSourceConfigTypeDef](./type_defs.md#evaluationprecomputedragsourceconfigtypedef)
- [ExternalSourceOutputTypeDef](./type_defs.md#externalsourceoutputtypedef)
- [RerankingMetadataSelectiveModeConfigurationOutputTypeDef](./type_defs.md#rerankingmetadataselectivemodeconfigurationoutputtypedef)
- [RerankingMetadataSelectiveModeConfigurationTypeDef](./type_defs.md#rerankingmetadataselectivemodeconfigurationtypedef)
- [RetrievalFilterOutputTypeDef](./type_defs.md#retrievalfilteroutputtypedef)
- [RetrievalFilterTypeDef](./type_defs.md#retrievalfiltertypedef)
- [FoundationModelDetailsTypeDef](./type_defs.md#foundationmodeldetailstypedef)
- [FoundationModelSummaryTypeDef](./type_defs.md#foundationmodelsummarytypedef)
- [GuardrailSummaryTypeDef](./type_defs.md#guardrailsummarytypedef)
- [GetInferenceProfileResponseTypeDef](./type_defs.md#getinferenceprofileresponsetypedef)
- [InferenceProfileSummaryTypeDef](./type_defs.md#inferenceprofilesummarytypedef)
- [SageMakerEndpointOutputTypeDef](./type_defs.md#sagemakerendpointoutputtypedef)
- [GuardrailContentPolicyConfigTypeDef](./type_defs.md#guardrailcontentpolicyconfigtypedef)
- [GuardrailContentPolicyTypeDef](./type_defs.md#guardrailcontentpolicytypedef)
- [GuardrailContextualGroundingPolicyConfigTypeDef](./type_defs.md#guardrailcontextualgroundingpolicyconfigtypedef)
- [GuardrailContextualGroundingPolicyTypeDef](./type_defs.md#guardrailcontextualgroundingpolicytypedef)
- [GuardrailSensitiveInformationPolicyConfigTypeDef](./type_defs.md#guardrailsensitiveinformationpolicyconfigtypedef)
- [GuardrailSensitiveInformationPolicyTypeDef](./type_defs.md#guardrailsensitiveinformationpolicytypedef)
- [GuardrailTopicPolicyConfigTypeDef](./type_defs.md#guardrailtopicpolicyconfigtypedef)
- [GuardrailTopicPolicyTypeDef](./type_defs.md#guardrailtopicpolicytypedef)
- [GuardrailWordPolicyConfigTypeDef](./type_defs.md#guardrailwordpolicyconfigtypedef)
- [GuardrailWordPolicyTypeDef](./type_defs.md#guardrailwordpolicytypedef)
- [ImplicitFilterConfigurationOutputTypeDef](./type_defs.md#implicitfilterconfigurationoutputtypedef)
- [ImplicitFilterConfigurationTypeDef](./type_defs.md#implicitfilterconfigurationtypedef)
- [ListImportedModelsResponseTypeDef](./type_defs.md#listimportedmodelsresponsetypedef)
- [KbInferenceConfigOutputTypeDef](./type_defs.md#kbinferenceconfigoutputtypedef)
- [KbInferenceConfigTypeDef](./type_defs.md#kbinferenceconfigtypedef)
- [ListGuardrailsRequestPaginateTypeDef](./type_defs.md#listguardrailsrequestpaginatetypedef)
- [ListInferenceProfilesRequestPaginateTypeDef](./type_defs.md#listinferenceprofilesrequestpaginatetypedef)
- [ListMarketplaceModelEndpointsRequestPaginateTypeDef](./type_defs.md#listmarketplacemodelendpointsrequestpaginatetypedef)
- [ListPromptRoutersRequestPaginateTypeDef](./type_defs.md#listpromptroutersrequestpaginatetypedef)
- [ListCustomModelDeploymentsRequestPaginateTypeDef](./type_defs.md#listcustommodeldeploymentsrequestpaginatetypedef)
- [ListCustomModelDeploymentsRequestTypeDef](./type_defs.md#listcustommodeldeploymentsrequesttypedef)
- [ListCustomModelsRequestPaginateTypeDef](./type_defs.md#listcustommodelsrequestpaginatetypedef)
- [ListCustomModelsRequestTypeDef](./type_defs.md#listcustommodelsrequesttypedef)
- [ListEvaluationJobsRequestPaginateTypeDef](./type_defs.md#listevaluationjobsrequestpaginatetypedef)
- [ListEvaluationJobsRequestTypeDef](./type_defs.md#listevaluationjobsrequesttypedef)
- [ListImportedModelsRequestPaginateTypeDef](./type_defs.md#listimportedmodelsrequestpaginatetypedef)
- [ListImportedModelsRequestTypeDef](./type_defs.md#listimportedmodelsrequesttypedef)
- [ListModelCopyJobsRequestPaginateTypeDef](./type_defs.md#listmodelcopyjobsrequestpaginatetypedef)
- [ListModelCopyJobsRequestTypeDef](./type_defs.md#listmodelcopyjobsrequesttypedef)
- [ListModelCustomizationJobsRequestPaginateTypeDef](./type_defs.md#listmodelcustomizationjobsrequestpaginatetypedef)
- [ListModelCustomizationJobsRequestTypeDef](./type_defs.md#listmodelcustomizationjobsrequesttypedef)
- [ListModelImportJobsRequestPaginateTypeDef](./type_defs.md#listmodelimportjobsrequestpaginatetypedef)
- [ListModelImportJobsRequestTypeDef](./type_defs.md#listmodelimportjobsrequesttypedef)
- [ListModelInvocationJobsRequestPaginateTypeDef](./type_defs.md#listmodelinvocationjobsrequestpaginatetypedef)
- [ListModelInvocationJobsRequestTypeDef](./type_defs.md#listmodelinvocationjobsrequesttypedef)
- [ListProvisionedModelThroughputsRequestPaginateTypeDef](./type_defs.md#listprovisionedmodelthroughputsrequestpaginatetypedef)
- [ListProvisionedModelThroughputsRequestTypeDef](./type_defs.md#listprovisionedmodelthroughputsrequesttypedef)
- [ListMarketplaceModelEndpointsResponseTypeDef](./type_defs.md#listmarketplacemodelendpointsresponsetypedef)
- [ListModelImportJobsResponseTypeDef](./type_defs.md#listmodelimportjobsresponsetypedef)
- [ListProvisionedModelThroughputsResponseTypeDef](./type_defs.md#listprovisionedmodelthroughputsresponsetypedef)
- [ModelDataSourceTypeDef](./type_defs.md#modeldatasourcetypedef)
- [ModelInvocationJobInputDataConfigTypeDef](./type_defs.md#modelinvocationjobinputdataconfigtypedef)
- [ModelInvocationJobOutputDataConfigTypeDef](./type_defs.md#modelinvocationjoboutputdataconfigtypedef)
- [OrchestrationConfigurationTypeDef](./type_defs.md#orchestrationconfigurationtypedef)
- [RatingScaleItemTypeDef](./type_defs.md#ratingscaleitemtypedef)
- [RequestMetadataFiltersOutputTypeDef](./type_defs.md#requestmetadatafiltersoutputtypedef)
- [RequestMetadataFiltersTypeDef](./type_defs.md#requestmetadatafilterstypedef)
- [SageMakerEndpointTypeDef](./type_defs.md#sagemakerendpointtypedef)
- [VpcConfigUnionTypeDef](./type_defs.md#vpcconfiguniontypedef)
- [StatusDetailsTypeDef](./type_defs.md#statusdetailstypedef)
- [ValidationDataConfigOutputTypeDef](./type_defs.md#validationdataconfigoutputtypedef)
- [ValidationDataConfigTypeDef](./type_defs.md#validationdataconfigtypedef)
- [ExternalSourceTypeDef](./type_defs.md#externalsourcetypedef)
- [LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef)
- [ListModelCopyJobsResponseTypeDef](./type_defs.md#listmodelcopyjobsresponsetypedef)
- [ListPromptRoutersResponseTypeDef](./type_defs.md#listpromptroutersresponsetypedef)
- [TermDetailsTypeDef](./type_defs.md#termdetailstypedef)
- [CustomizationConfigTypeDef](./type_defs.md#customizationconfigtypedef)
- [EvaluationModelConfigTypeDef](./type_defs.md#evaluationmodelconfigtypedef)
- [EvaluationDatasetMetricConfigOutputTypeDef](./type_defs.md#evaluationdatasetmetricconfigoutputtypedef)
- [EvaluationDatasetMetricConfigTypeDef](./type_defs.md#evaluationdatasetmetricconfigtypedef)
- [EvaluationSummaryTypeDef](./type_defs.md#evaluationsummarytypedef)
- [MetadataConfigurationForRerankingOutputTypeDef](./type_defs.md#metadataconfigurationforrerankingoutputtypedef)
- [MetadataConfigurationForRerankingTypeDef](./type_defs.md#metadataconfigurationforrerankingtypedef)
- [GetFoundationModelResponseTypeDef](./type_defs.md#getfoundationmodelresponsetypedef)
- [ListFoundationModelsResponseTypeDef](./type_defs.md#listfoundationmodelsresponsetypedef)
- [ListGuardrailsResponseTypeDef](./type_defs.md#listguardrailsresponsetypedef)
- [ListInferenceProfilesResponseTypeDef](./type_defs.md#listinferenceprofilesresponsetypedef)
- [EndpointConfigOutputTypeDef](./type_defs.md#endpointconfigoutputtypedef)
- [CreateGuardrailRequestTypeDef](./type_defs.md#createguardrailrequesttypedef)
- [UpdateGuardrailRequestTypeDef](./type_defs.md#updateguardrailrequesttypedef)
- [GetGuardrailResponseTypeDef](./type_defs.md#getguardrailresponsetypedef)
- [ExternalSourcesGenerationConfigurationOutputTypeDef](./type_defs.md#externalsourcesgenerationconfigurationoutputtypedef)
- [GenerationConfigurationOutputTypeDef](./type_defs.md#generationconfigurationoutputtypedef)
- [ExternalSourcesGenerationConfigurationTypeDef](./type_defs.md#externalsourcesgenerationconfigurationtypedef)
- [GenerationConfigurationTypeDef](./type_defs.md#generationconfigurationtypedef)
- [CreateCustomModelRequestTypeDef](./type_defs.md#createcustommodelrequesttypedef)
- [GetImportedModelResponseTypeDef](./type_defs.md#getimportedmodelresponsetypedef)
- [GetModelImportJobResponseTypeDef](./type_defs.md#getmodelimportjobresponsetypedef)
- [GetModelInvocationJobResponseTypeDef](./type_defs.md#getmodelinvocationjobresponsetypedef)
- [ModelInvocationJobSummaryTypeDef](./type_defs.md#modelinvocationjobsummarytypedef)
- [CustomMetricDefinitionOutputTypeDef](./type_defs.md#custommetricdefinitionoutputtypedef)
- [CustomMetricDefinitionTypeDef](./type_defs.md#custommetricdefinitiontypedef)
- [InvocationLogsConfigOutputTypeDef](./type_defs.md#invocationlogsconfigoutputtypedef)
- [InvocationLogsConfigTypeDef](./type_defs.md#invocationlogsconfigtypedef)
- [EndpointConfigTypeDef](./type_defs.md#endpointconfigtypedef)
- [CreateModelImportJobRequestTypeDef](./type_defs.md#createmodelimportjobrequesttypedef)
- [CreateModelInvocationJobRequestTypeDef](./type_defs.md#createmodelinvocationjobrequesttypedef)
- [ModelCustomizationJobSummaryTypeDef](./type_defs.md#modelcustomizationjobsummarytypedef)
- [ValidationDataConfigUnionTypeDef](./type_defs.md#validationdataconfiguniontypedef)
- [GetModelInvocationLoggingConfigurationResponseTypeDef](./type_defs.md#getmodelinvocationloggingconfigurationresponsetypedef)
- [PutModelInvocationLoggingConfigurationRequestTypeDef](./type_defs.md#putmodelinvocationloggingconfigurationrequesttypedef)
- [OfferTypeDef](./type_defs.md#offertypedef)
- [HumanEvaluationConfigOutputTypeDef](./type_defs.md#humanevaluationconfigoutputtypedef)
- [HumanEvaluationConfigTypeDef](./type_defs.md#humanevaluationconfigtypedef)
- [ListEvaluationJobsResponseTypeDef](./type_defs.md#listevaluationjobsresponsetypedef)
- [VectorSearchBedrockRerankingConfigurationOutputTypeDef](./type_defs.md#vectorsearchbedrockrerankingconfigurationoutputtypedef)
- [VectorSearchBedrockRerankingConfigurationTypeDef](./type_defs.md#vectorsearchbedrockrerankingconfigurationtypedef)
- [MarketplaceModelEndpointTypeDef](./type_defs.md#marketplacemodelendpointtypedef)
- [ExternalSourcesRetrieveAndGenerateConfigurationOutputTypeDef](./type_defs.md#externalsourcesretrieveandgenerateconfigurationoutputtypedef)
- [ExternalSourcesRetrieveAndGenerateConfigurationTypeDef](./type_defs.md#externalsourcesretrieveandgenerateconfigurationtypedef)
- [ListModelInvocationJobsResponseTypeDef](./type_defs.md#listmodelinvocationjobsresponsetypedef)
- [AutomatedEvaluationCustomMetricSourceOutputTypeDef](./type_defs.md#automatedevaluationcustommetricsourceoutputtypedef)
- [AutomatedEvaluationCustomMetricSourceTypeDef](./type_defs.md#automatedevaluationcustommetricsourcetypedef)
- [TrainingDataConfigOutputTypeDef](./type_defs.md#trainingdataconfigoutputtypedef)
- [TrainingDataConfigTypeDef](./type_defs.md#trainingdataconfigtypedef)
- [EndpointConfigUnionTypeDef](./type_defs.md#endpointconfiguniontypedef)
- [ListModelCustomizationJobsResponseTypeDef](./type_defs.md#listmodelcustomizationjobsresponsetypedef)
- [ListFoundationModelAgreementOffersResponseTypeDef](./type_defs.md#listfoundationmodelagreementoffersresponsetypedef)
- [VectorSearchRerankingConfigurationOutputTypeDef](./type_defs.md#vectorsearchrerankingconfigurationoutputtypedef)
- [VectorSearchRerankingConfigurationTypeDef](./type_defs.md#vectorsearchrerankingconfigurationtypedef)
- [CreateMarketplaceModelEndpointResponseTypeDef](./type_defs.md#createmarketplacemodelendpointresponsetypedef)
- [GetMarketplaceModelEndpointResponseTypeDef](./type_defs.md#getmarketplacemodelendpointresponsetypedef)
- [RegisterMarketplaceModelEndpointResponseTypeDef](./type_defs.md#registermarketplacemodelendpointresponsetypedef)
- [UpdateMarketplaceModelEndpointResponseTypeDef](./type_defs.md#updatemarketplacemodelendpointresponsetypedef)
- [AutomatedEvaluationCustomMetricConfigOutputTypeDef](./type_defs.md#automatedevaluationcustommetricconfigoutputtypedef)
- [AutomatedEvaluationCustomMetricConfigTypeDef](./type_defs.md#automatedevaluationcustommetricconfigtypedef)
- [GetCustomModelResponseTypeDef](./type_defs.md#getcustommodelresponsetypedef)
- [GetModelCustomizationJobResponseTypeDef](./type_defs.md#getmodelcustomizationjobresponsetypedef)
- [TrainingDataConfigUnionTypeDef](./type_defs.md#trainingdataconfiguniontypedef)
- [CreateMarketplaceModelEndpointRequestTypeDef](./type_defs.md#createmarketplacemodelendpointrequesttypedef)
- [UpdateMarketplaceModelEndpointRequestTypeDef](./type_defs.md#updatemarketplacemodelendpointrequesttypedef)
- [KnowledgeBaseVectorSearchConfigurationOutputTypeDef](./type_defs.md#knowledgebasevectorsearchconfigurationoutputtypedef)
- [KnowledgeBaseVectorSearchConfigurationTypeDef](./type_defs.md#knowledgebasevectorsearchconfigurationtypedef)
- [AutomatedEvaluationConfigOutputTypeDef](./type_defs.md#automatedevaluationconfigoutputtypedef)
- [AutomatedEvaluationConfigTypeDef](./type_defs.md#automatedevaluationconfigtypedef)
- [CreateModelCustomizationJobRequestTypeDef](./type_defs.md#createmodelcustomizationjobrequesttypedef)
- [KnowledgeBaseRetrievalConfigurationOutputTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationoutputtypedef)
- [KnowledgeBaseRetrievalConfigurationTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationtypedef)
- [EvaluationConfigOutputTypeDef](./type_defs.md#evaluationconfigoutputtypedef)
- [EvaluationConfigTypeDef](./type_defs.md#evaluationconfigtypedef)
- [KnowledgeBaseRetrieveAndGenerateConfigurationOutputTypeDef](./type_defs.md#knowledgebaseretrieveandgenerateconfigurationoutputtypedef)
- [RetrieveConfigOutputTypeDef](./type_defs.md#retrieveconfigoutputtypedef)
- [KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef](./type_defs.md#knowledgebaseretrieveandgenerateconfigurationtypedef)
- [RetrieveConfigTypeDef](./type_defs.md#retrieveconfigtypedef)
- [EvaluationConfigUnionTypeDef](./type_defs.md#evaluationconfiguniontypedef)
- [RetrieveAndGenerateConfigurationOutputTypeDef](./type_defs.md#retrieveandgenerateconfigurationoutputtypedef)
- [RetrieveAndGenerateConfigurationTypeDef](./type_defs.md#retrieveandgenerateconfigurationtypedef)
- [KnowledgeBaseConfigOutputTypeDef](./type_defs.md#knowledgebaseconfigoutputtypedef)
- [KnowledgeBaseConfigTypeDef](./type_defs.md#knowledgebaseconfigtypedef)
- [RAGConfigOutputTypeDef](./type_defs.md#ragconfigoutputtypedef)
- [RAGConfigTypeDef](./type_defs.md#ragconfigtypedef)
- [EvaluationInferenceConfigOutputTypeDef](./type_defs.md#evaluationinferenceconfigoutputtypedef)
- [EvaluationInferenceConfigTypeDef](./type_defs.md#evaluationinferenceconfigtypedef)
- [GetEvaluationJobResponseTypeDef](./type_defs.md#getevaluationjobresponsetypedef)
- [EvaluationInferenceConfigUnionTypeDef](./type_defs.md#evaluationinferenceconfiguniontypedef)
- [CreateEvaluationJobRequestTypeDef](./type_defs.md#createevaluationjobrequesttypedef)

