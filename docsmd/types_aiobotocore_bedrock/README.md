# Bedrock module

> [Index](../README.md) > Bedrock


!!! note ""

    Auto-generated documentation for [Bedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock)
    type annotations stubs module [types-aiobotocore-bedrock](https://pypi.org/project/types-aiobotocore-bedrock/).

## How to install



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
- [ListModelCopyJobsPaginator](./paginators.md#listmodelcopyjobspaginator)
- [ListModelCustomizationJobsPaginator](./paginators.md#listmodelcustomizationjobspaginator)
- [ListModelImportJobsPaginator](./paginators.md#listmodelimportjobspaginator)
- [ListModelInvocationJobsPaginator](./paginators.md#listmodelinvocationjobspaginator)
- [ListProvisionedModelThroughputsPaginator](./paginators.md#listprovisionedmodelthroughputspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# CommitmentDurationType usage example

from types_aiobotocore_bedrock.literals import CommitmentDurationType

def get_value() -> CommitmentDurationType:
    return "OneMonth"
```

- [CommitmentDurationType](./literals.md#commitmentdurationtype)
- [CustomizationTypeType](./literals.md#customizationtypetype)
- [EvaluationJobStatusType](./literals.md#evaluationjobstatustype)
- [EvaluationJobTypeType](./literals.md#evaluationjobtypetype)
- [EvaluationTaskTypeType](./literals.md#evaluationtasktypetype)
- [FineTuningJobStatusType](./literals.md#finetuningjobstatustype)
- [FoundationModelLifecycleStatusType](./literals.md#foundationmodellifecyclestatustype)
- [GuardrailContentFilterTypeType](./literals.md#guardrailcontentfiltertypetype)
- [GuardrailContextualGroundingFilterTypeType](./literals.md#guardrailcontextualgroundingfiltertypetype)
- [GuardrailFilterStrengthType](./literals.md#guardrailfilterstrengthtype)
- [GuardrailManagedWordsTypeType](./literals.md#guardrailmanagedwordstypetype)
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
- [ListModelCopyJobsPaginatorName](./literals.md#listmodelcopyjobspaginatorname)
- [ListModelCustomizationJobsPaginatorName](./literals.md#listmodelcustomizationjobspaginatorname)
- [ListModelImportJobsPaginatorName](./literals.md#listmodelimportjobspaginatorname)
- [ListModelInvocationJobsPaginatorName](./literals.md#listmodelinvocationjobspaginatorname)
- [ListProvisionedModelThroughputsPaginatorName](./literals.md#listprovisionedmodelthroughputspaginatorname)
- [ModelCopyJobStatusType](./literals.md#modelcopyjobstatustype)
- [ModelCustomizationJobStatusType](./literals.md#modelcustomizationjobstatustype)
- [ModelCustomizationType](./literals.md#modelcustomizationtype)
- [ModelImportJobStatusType](./literals.md#modelimportjobstatustype)
- [ModelInvocationJobStatusType](./literals.md#modelinvocationjobstatustype)
- [ModelModalityType](./literals.md#modelmodalitytype)
- [ProvisionedModelStatusType](./literals.md#provisionedmodelstatustype)
- [S3InputFormatType](./literals.md#s3inputformattype)
- [SortByProvisionedModelsType](./literals.md#sortbyprovisionedmodelstype)
- [SortJobsByType](./literals.md#sortjobsbytype)
- [SortModelsByType](./literals.md#sortmodelsbytype)
- [SortOrderType](./literals.md#sortordertype)
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
- [S3ConfigTypeDef](./type_defs.md#s3configtypedef)
- [EvaluationOutputDataConfigTypeDef](./type_defs.md#evaluationoutputdataconfigtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [CreateGuardrailVersionRequestRequestTypeDef](./type_defs.md#createguardrailversionrequestrequesttypedef)
- [OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef)
- [TrainingDataConfigTypeDef](./type_defs.md#trainingdataconfigtypedef)
- [VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef)
- [CustomModelSummaryTypeDef](./type_defs.md#custommodelsummarytypedef)
- [DeleteCustomModelRequestRequestTypeDef](./type_defs.md#deletecustommodelrequestrequesttypedef)
- [DeleteGuardrailRequestRequestTypeDef](./type_defs.md#deleteguardrailrequestrequesttypedef)
- [DeleteImportedModelRequestRequestTypeDef](./type_defs.md#deleteimportedmodelrequestrequesttypedef)
- [DeleteProvisionedModelThroughputRequestRequestTypeDef](./type_defs.md#deleteprovisionedmodelthroughputrequestrequesttypedef)
- [EvaluationBedrockModelTypeDef](./type_defs.md#evaluationbedrockmodeltypedef)
- [EvaluationDatasetLocationTypeDef](./type_defs.md#evaluationdatasetlocationtypedef)
- [EvaluationSummaryTypeDef](./type_defs.md#evaluationsummarytypedef)
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
- [GetModelCopyJobRequestRequestTypeDef](./type_defs.md#getmodelcopyjobrequestrequesttypedef)
- [GetModelCustomizationJobRequestRequestTypeDef](./type_defs.md#getmodelcustomizationjobrequestrequesttypedef)
- [VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef)
- [GetModelImportJobRequestRequestTypeDef](./type_defs.md#getmodelimportjobrequestrequesttypedef)
- [GetModelInvocationJobRequestRequestTypeDef](./type_defs.md#getmodelinvocationjobrequestrequesttypedef)
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
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ListFoundationModelsRequestRequestTypeDef](./type_defs.md#listfoundationmodelsrequestrequesttypedef)
- [ListGuardrailsRequestRequestTypeDef](./type_defs.md#listguardrailsrequestrequesttypedef)
- [ListInferenceProfilesRequestRequestTypeDef](./type_defs.md#listinferenceprofilesrequestrequesttypedef)
- [ModelCustomizationJobSummaryTypeDef](./type_defs.md#modelcustomizationjobsummarytypedef)
- [ModelImportJobSummaryTypeDef](./type_defs.md#modelimportjobsummarytypedef)
- [ProvisionedModelSummaryTypeDef](./type_defs.md#provisionedmodelsummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [S3DataSourceTypeDef](./type_defs.md#s3datasourcetypedef)
- [ModelInvocationJobS3InputDataConfigTypeDef](./type_defs.md#modelinvocationjobs3inputdataconfigtypedef)
- [ModelInvocationJobS3OutputDataConfigTypeDef](./type_defs.md#modelinvocationjobs3outputdataconfigtypedef)
- [StopEvaluationJobRequestRequestTypeDef](./type_defs.md#stopevaluationjobrequestrequesttypedef)
- [StopModelCustomizationJobRequestRequestTypeDef](./type_defs.md#stopmodelcustomizationjobrequestrequesttypedef)
- [StopModelInvocationJobRequestRequestTypeDef](./type_defs.md#stopmodelinvocationjobrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateProvisionedModelThroughputRequestRequestTypeDef](./type_defs.md#updateprovisionedmodelthroughputrequestrequesttypedef)
- [ValidatorTypeDef](./type_defs.md#validatortypedef)
- [BatchDeleteEvaluationJobResponseTypeDef](./type_defs.md#batchdeleteevaluationjobresponsetypedef)
- [CreateEvaluationJobResponseTypeDef](./type_defs.md#createevaluationjobresponsetypedef)
- [CreateGuardrailResponseTypeDef](./type_defs.md#createguardrailresponsetypedef)
- [CreateGuardrailVersionResponseTypeDef](./type_defs.md#createguardrailversionresponsetypedef)
- [CreateModelCopyJobResponseTypeDef](./type_defs.md#createmodelcopyjobresponsetypedef)
- [CreateModelCustomizationJobResponseTypeDef](./type_defs.md#createmodelcustomizationjobresponsetypedef)
- [CreateModelImportJobResponseTypeDef](./type_defs.md#createmodelimportjobresponsetypedef)
- [CreateModelInvocationJobResponseTypeDef](./type_defs.md#createmodelinvocationjobresponsetypedef)
- [CreateProvisionedModelThroughputResponseTypeDef](./type_defs.md#createprovisionedmodelthroughputresponsetypedef)
- [GetProvisionedModelThroughputResponseTypeDef](./type_defs.md#getprovisionedmodelthroughputresponsetypedef)
- [UpdateGuardrailResponseTypeDef](./type_defs.md#updateguardrailresponsetypedef)
- [CloudWatchConfigTypeDef](./type_defs.md#cloudwatchconfigtypedef)
- [CreateModelCopyJobRequestRequestTypeDef](./type_defs.md#createmodelcopyjobrequestrequesttypedef)
- [CreateProvisionedModelThroughputRequestRequestTypeDef](./type_defs.md#createprovisionedmodelthroughputrequestrequesttypedef)
- [GetModelCopyJobResponseTypeDef](./type_defs.md#getmodelcopyjobresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ModelCopyJobSummaryTypeDef](./type_defs.md#modelcopyjobsummarytypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [ListCustomModelsResponseTypeDef](./type_defs.md#listcustommodelsresponsetypedef)
- [EvaluationModelConfigTypeDef](./type_defs.md#evaluationmodelconfigtypedef)
- [EvaluationDatasetTypeDef](./type_defs.md#evaluationdatasettypedef)
- [ListEvaluationJobsResponseTypeDef](./type_defs.md#listevaluationjobsresponsetypedef)
- [FoundationModelDetailsTypeDef](./type_defs.md#foundationmodeldetailstypedef)
- [FoundationModelSummaryTypeDef](./type_defs.md#foundationmodelsummarytypedef)
- [GetInferenceProfileResponseTypeDef](./type_defs.md#getinferenceprofileresponsetypedef)
- [InferenceProfileSummaryTypeDef](./type_defs.md#inferenceprofilesummarytypedef)
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
- [ListGuardrailsRequestListGuardrailsPaginateTypeDef](./type_defs.md#listguardrailsrequestlistguardrailspaginatetypedef)
- [ListInferenceProfilesRequestListInferenceProfilesPaginateTypeDef](./type_defs.md#listinferenceprofilesrequestlistinferenceprofilespaginatetypedef)
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
- [ListModelCustomizationJobsResponseTypeDef](./type_defs.md#listmodelcustomizationjobsresponsetypedef)
- [ListModelImportJobsResponseTypeDef](./type_defs.md#listmodelimportjobsresponsetypedef)
- [ListProvisionedModelThroughputsResponseTypeDef](./type_defs.md#listprovisionedmodelthroughputsresponsetypedef)
- [ModelDataSourceTypeDef](./type_defs.md#modeldatasourcetypedef)
- [ModelInvocationJobInputDataConfigTypeDef](./type_defs.md#modelinvocationjobinputdataconfigtypedef)
- [ModelInvocationJobOutputDataConfigTypeDef](./type_defs.md#modelinvocationjoboutputdataconfigtypedef)
- [ValidationDataConfigOutputTypeDef](./type_defs.md#validationdataconfigoutputtypedef)
- [ValidationDataConfigTypeDef](./type_defs.md#validationdataconfigtypedef)
- [LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef)
- [ListModelCopyJobsResponseTypeDef](./type_defs.md#listmodelcopyjobsresponsetypedef)
- [EvaluationInferenceConfigOutputTypeDef](./type_defs.md#evaluationinferenceconfigoutputtypedef)
- [EvaluationInferenceConfigTypeDef](./type_defs.md#evaluationinferenceconfigtypedef)
- [EvaluationDatasetMetricConfigOutputTypeDef](./type_defs.md#evaluationdatasetmetricconfigoutputtypedef)
- [EvaluationDatasetMetricConfigTypeDef](./type_defs.md#evaluationdatasetmetricconfigtypedef)
- [GetFoundationModelResponseTypeDef](./type_defs.md#getfoundationmodelresponsetypedef)
- [ListFoundationModelsResponseTypeDef](./type_defs.md#listfoundationmodelsresponsetypedef)
- [ListInferenceProfilesResponseTypeDef](./type_defs.md#listinferenceprofilesresponsetypedef)
- [CreateGuardrailRequestRequestTypeDef](./type_defs.md#createguardrailrequestrequesttypedef)
- [UpdateGuardrailRequestRequestTypeDef](./type_defs.md#updateguardrailrequestrequesttypedef)
- [GetGuardrailResponseTypeDef](./type_defs.md#getguardrailresponsetypedef)
- [CreateModelImportJobRequestRequestTypeDef](./type_defs.md#createmodelimportjobrequestrequesttypedef)
- [GetImportedModelResponseTypeDef](./type_defs.md#getimportedmodelresponsetypedef)
- [GetModelImportJobResponseTypeDef](./type_defs.md#getmodelimportjobresponsetypedef)
- [CreateModelInvocationJobRequestRequestTypeDef](./type_defs.md#createmodelinvocationjobrequestrequesttypedef)
- [GetModelInvocationJobResponseTypeDef](./type_defs.md#getmodelinvocationjobresponsetypedef)
- [ModelInvocationJobSummaryTypeDef](./type_defs.md#modelinvocationjobsummarytypedef)
- [GetCustomModelResponseTypeDef](./type_defs.md#getcustommodelresponsetypedef)
- [GetModelCustomizationJobResponseTypeDef](./type_defs.md#getmodelcustomizationjobresponsetypedef)
- [CreateModelCustomizationJobRequestRequestTypeDef](./type_defs.md#createmodelcustomizationjobrequestrequesttypedef)
- [GetModelInvocationLoggingConfigurationResponseTypeDef](./type_defs.md#getmodelinvocationloggingconfigurationresponsetypedef)
- [PutModelInvocationLoggingConfigurationRequestRequestTypeDef](./type_defs.md#putmodelinvocationloggingconfigurationrequestrequesttypedef)
- [AutomatedEvaluationConfigOutputTypeDef](./type_defs.md#automatedevaluationconfigoutputtypedef)
- [HumanEvaluationConfigOutputTypeDef](./type_defs.md#humanevaluationconfigoutputtypedef)
- [EvaluationDatasetMetricConfigUnionTypeDef](./type_defs.md#evaluationdatasetmetricconfiguniontypedef)
- [HumanEvaluationConfigTypeDef](./type_defs.md#humanevaluationconfigtypedef)
- [ListModelInvocationJobsResponseTypeDef](./type_defs.md#listmodelinvocationjobsresponsetypedef)
- [EvaluationConfigOutputTypeDef](./type_defs.md#evaluationconfigoutputtypedef)
- [AutomatedEvaluationConfigTypeDef](./type_defs.md#automatedevaluationconfigtypedef)
- [HumanEvaluationConfigUnionTypeDef](./type_defs.md#humanevaluationconfiguniontypedef)
- [GetEvaluationJobResponseTypeDef](./type_defs.md#getevaluationjobresponsetypedef)
- [AutomatedEvaluationConfigUnionTypeDef](./type_defs.md#automatedevaluationconfiguniontypedef)
- [EvaluationConfigTypeDef](./type_defs.md#evaluationconfigtypedef)
- [CreateEvaluationJobRequestRequestTypeDef](./type_defs.md#createevaluationjobrequestrequesttypedef)

