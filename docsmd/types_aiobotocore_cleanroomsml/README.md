# CleanRoomsML module

> [Index](../README.md) > CleanRoomsML


!!! note ""

    Auto-generated documentation for [CleanRoomsML](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#cleanroomsml)
    type annotations stubs module [types-aiobotocore-cleanroomsml](https://pypi.org/project/types-aiobotocore-cleanroomsml/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `CleanRoomsML` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `CleanRoomsML` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[cleanroomsml]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[cleanroomsml]'

# standalone installation
python -m pip install types-aiobotocore-cleanroomsml
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-cleanroomsml
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CleanRoomsMLClient

Type annotations and code completion for  `#!python session.create_client("cleanroomsml")` as [CleanRoomsMLClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client)

```python
# CleanRoomsMLClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanroomsml.client import CleanRoomsMLClient


session = get_session()
async with session.create_client("cleanroomsml") as client:
    client: CleanRoomsMLClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("cleanroomsml").get_paginator("...")`.

```python
# ListAudienceExportJobsPaginator usage example

from types_aiobotocore_cleanroomsml.paginator import ListAudienceExportJobsPaginator

def get_list_audience_export_jobs_paginator() -> ListAudienceExportJobsPaginator:
    return client.get_paginator("list_audience_export_jobs"))
```

- [ListAudienceExportJobsPaginator](./paginators.md#listaudienceexportjobspaginator)
- [ListAudienceGenerationJobsPaginator](./paginators.md#listaudiencegenerationjobspaginator)
- [ListAudienceModelsPaginator](./paginators.md#listaudiencemodelspaginator)
- [ListCollaborationConfiguredModelAlgorithmAssociationsPaginator](./paginators.md#listcollaborationconfiguredmodelalgorithmassociationspaginator)
- [ListCollaborationMLInputChannelsPaginator](./paginators.md#listcollaborationmlinputchannelspaginator)
- [ListCollaborationTrainedModelExportJobsPaginator](./paginators.md#listcollaborationtrainedmodelexportjobspaginator)
- [ListCollaborationTrainedModelInferenceJobsPaginator](./paginators.md#listcollaborationtrainedmodelinferencejobspaginator)
- [ListCollaborationTrainedModelsPaginator](./paginators.md#listcollaborationtrainedmodelspaginator)
- [ListConfiguredAudienceModelsPaginator](./paginators.md#listconfiguredaudiencemodelspaginator)
- [ListConfiguredModelAlgorithmAssociationsPaginator](./paginators.md#listconfiguredmodelalgorithmassociationspaginator)
- [ListConfiguredModelAlgorithmsPaginator](./paginators.md#listconfiguredmodelalgorithmspaginator)
- [ListMLInputChannelsPaginator](./paginators.md#listmlinputchannelspaginator)
- [ListTrainedModelInferenceJobsPaginator](./paginators.md#listtrainedmodelinferencejobspaginator)
- [ListTrainedModelsPaginator](./paginators.md#listtrainedmodelspaginator)
- [ListTrainingDatasetsPaginator](./paginators.md#listtrainingdatasetspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AudienceExportJobStatusType usage example

from types_aiobotocore_cleanroomsml.literals import AudienceExportJobStatusType

def get_value() -> AudienceExportJobStatusType:
    return "ACTIVE"
```

- [AudienceExportJobStatusType](./literals.md#audienceexportjobstatustype)
- [AudienceGenerationJobStatusType](./literals.md#audiencegenerationjobstatustype)
- [AudienceModelStatusType](./literals.md#audiencemodelstatustype)
- [AudienceSizeTypeType](./literals.md#audiencesizetypetype)
- [ColumnTypeType](./literals.md#columntypetype)
- [ConfiguredAudienceModelStatusType](./literals.md#configuredaudiencemodelstatustype)
- [DatasetTypeType](./literals.md#datasettypetype)
- [InferenceInstanceTypeType](./literals.md#inferenceinstancetypetype)
- [InstanceTypeType](./literals.md#instancetypetype)
- [ListAudienceExportJobsPaginatorName](./literals.md#listaudienceexportjobspaginatorname)
- [ListAudienceGenerationJobsPaginatorName](./literals.md#listaudiencegenerationjobspaginatorname)
- [ListAudienceModelsPaginatorName](./literals.md#listaudiencemodelspaginatorname)
- [ListCollaborationConfiguredModelAlgorithmAssociationsPaginatorName](./literals.md#listcollaborationconfiguredmodelalgorithmassociationspaginatorname)
- [ListCollaborationMLInputChannelsPaginatorName](./literals.md#listcollaborationmlinputchannelspaginatorname)
- [ListCollaborationTrainedModelExportJobsPaginatorName](./literals.md#listcollaborationtrainedmodelexportjobspaginatorname)
- [ListCollaborationTrainedModelInferenceJobsPaginatorName](./literals.md#listcollaborationtrainedmodelinferencejobspaginatorname)
- [ListCollaborationTrainedModelsPaginatorName](./literals.md#listcollaborationtrainedmodelspaginatorname)
- [ListConfiguredAudienceModelsPaginatorName](./literals.md#listconfiguredaudiencemodelspaginatorname)
- [ListConfiguredModelAlgorithmAssociationsPaginatorName](./literals.md#listconfiguredmodelalgorithmassociationspaginatorname)
- [ListConfiguredModelAlgorithmsPaginatorName](./literals.md#listconfiguredmodelalgorithmspaginatorname)
- [ListMLInputChannelsPaginatorName](./literals.md#listmlinputchannelspaginatorname)
- [ListTrainedModelInferenceJobsPaginatorName](./literals.md#listtrainedmodelinferencejobspaginatorname)
- [ListTrainedModelsPaginatorName](./literals.md#listtrainedmodelspaginatorname)
- [ListTrainingDatasetsPaginatorName](./literals.md#listtrainingdatasetspaginatorname)
- [LogsStatusType](./literals.md#logsstatustype)
- [MLInputChannelStatusType](./literals.md#mlinputchannelstatustype)
- [MetricsStatusType](./literals.md#metricsstatustype)
- [NoiseLevelTypeType](./literals.md#noiseleveltypetype)
- [PolicyExistenceConditionType](./literals.md#policyexistenceconditiontype)
- [SharedAudienceMetricsType](./literals.md#sharedaudiencemetricstype)
- [TagOnCreatePolicyType](./literals.md#tagoncreatepolicytype)
- [TrainedModelExportFileTypeType](./literals.md#trainedmodelexportfiletypetype)
- [TrainedModelExportJobStatusType](./literals.md#trainedmodelexportjobstatustype)
- [TrainedModelExportsMaxSizeUnitTypeType](./literals.md#trainedmodelexportsmaxsizeunittypetype)
- [TrainedModelInferenceJobStatusType](./literals.md#trainedmodelinferencejobstatustype)
- [TrainedModelInferenceMaxOutputSizeUnitTypeType](./literals.md#trainedmodelinferencemaxoutputsizeunittypetype)
- [TrainedModelStatusType](./literals.md#trainedmodelstatustype)
- [TrainingDatasetStatusType](./literals.md#trainingdatasetstatustype)
- [WorkerComputeTypeType](./literals.md#workercomputetypetype)
- [CleanRoomsMLServiceName](./literals.md#cleanroomsmlservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [S3ConfigMapTypeDef](./type_defs.md#s3configmaptypedef)
- [AudienceSizeTypeDef](./type_defs.md#audiencesizetypedef)
- [StatusDetailsTypeDef](./type_defs.md#statusdetailstypedef)
- [ProtectedQuerySQLParametersOutputTypeDef](./type_defs.md#protectedquerysqlparametersoutputtypedef)
- [AudienceGenerationJobSummaryTypeDef](./type_defs.md#audiencegenerationjobsummarytypedef)
- [AudienceModelSummaryTypeDef](./type_defs.md#audiencemodelsummarytypedef)
- [AudienceSizeConfigOutputTypeDef](./type_defs.md#audiencesizeconfigoutputtypedef)
- [AudienceSizeConfigTypeDef](./type_defs.md#audiencesizeconfigtypedef)
- [CancelTrainedModelInferenceJobRequestRequestTypeDef](./type_defs.md#canceltrainedmodelinferencejobrequestrequesttypedef)
- [CancelTrainedModelRequestRequestTypeDef](./type_defs.md#canceltrainedmodelrequestrequesttypedef)
- [CollaborationConfiguredModelAlgorithmAssociationSummaryTypeDef](./type_defs.md#collaborationconfiguredmodelalgorithmassociationsummarytypedef)
- [CollaborationMLInputChannelSummaryTypeDef](./type_defs.md#collaborationmlinputchannelsummarytypedef)
- [CollaborationTrainedModelSummaryTypeDef](./type_defs.md#collaborationtrainedmodelsummarytypedef)
- [ColumnSchemaOutputTypeDef](./type_defs.md#columnschemaoutputtypedef)
- [ColumnSchemaTypeDef](./type_defs.md#columnschematypedef)
- [WorkerComputeConfigurationTypeDef](./type_defs.md#workercomputeconfigurationtypedef)
- [ConfiguredModelAlgorithmAssociationSummaryTypeDef](./type_defs.md#configuredmodelalgorithmassociationsummarytypedef)
- [ConfiguredModelAlgorithmSummaryTypeDef](./type_defs.md#configuredmodelalgorithmsummarytypedef)
- [MetricDefinitionTypeDef](./type_defs.md#metricdefinitiontypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [InferenceContainerConfigTypeDef](./type_defs.md#inferencecontainerconfigtypedef)
- [ModelTrainingDataChannelTypeDef](./type_defs.md#modeltrainingdatachanneltypedef)
- [ResourceConfigTypeDef](./type_defs.md#resourceconfigtypedef)
- [StoppingConditionTypeDef](./type_defs.md#stoppingconditiontypedef)
- [GlueDataSourceTypeDef](./type_defs.md#gluedatasourcetypedef)
- [DeleteAudienceGenerationJobRequestRequestTypeDef](./type_defs.md#deleteaudiencegenerationjobrequestrequesttypedef)
- [DeleteAudienceModelRequestRequestTypeDef](./type_defs.md#deleteaudiencemodelrequestrequesttypedef)
- [DeleteConfiguredAudienceModelPolicyRequestRequestTypeDef](./type_defs.md#deleteconfiguredaudiencemodelpolicyrequestrequesttypedef)
- [DeleteConfiguredAudienceModelRequestRequestTypeDef](./type_defs.md#deleteconfiguredaudiencemodelrequestrequesttypedef)
- [DeleteConfiguredModelAlgorithmAssociationRequestRequestTypeDef](./type_defs.md#deleteconfiguredmodelalgorithmassociationrequestrequesttypedef)
- [DeleteConfiguredModelAlgorithmRequestRequestTypeDef](./type_defs.md#deleteconfiguredmodelalgorithmrequestrequesttypedef)
- [DeleteMLConfigurationRequestRequestTypeDef](./type_defs.md#deletemlconfigurationrequestrequesttypedef)
- [DeleteMLInputChannelDataRequestRequestTypeDef](./type_defs.md#deletemlinputchanneldatarequestrequesttypedef)
- [DeleteTrainedModelOutputRequestRequestTypeDef](./type_defs.md#deletetrainedmodeloutputrequestrequesttypedef)
- [DeleteTrainingDatasetRequestRequestTypeDef](./type_defs.md#deletetrainingdatasetrequestrequesttypedef)
- [GetAudienceGenerationJobRequestRequestTypeDef](./type_defs.md#getaudiencegenerationjobrequestrequesttypedef)
- [GetAudienceModelRequestRequestTypeDef](./type_defs.md#getaudiencemodelrequestrequesttypedef)
- [GetCollaborationConfiguredModelAlgorithmAssociationRequestRequestTypeDef](./type_defs.md#getcollaborationconfiguredmodelalgorithmassociationrequestrequesttypedef)
- [GetCollaborationMLInputChannelRequestRequestTypeDef](./type_defs.md#getcollaborationmlinputchannelrequestrequesttypedef)
- [GetCollaborationTrainedModelRequestRequestTypeDef](./type_defs.md#getcollaborationtrainedmodelrequestrequesttypedef)
- [GetConfiguredAudienceModelPolicyRequestRequestTypeDef](./type_defs.md#getconfiguredaudiencemodelpolicyrequestrequesttypedef)
- [GetConfiguredAudienceModelRequestRequestTypeDef](./type_defs.md#getconfiguredaudiencemodelrequestrequesttypedef)
- [GetConfiguredModelAlgorithmAssociationRequestRequestTypeDef](./type_defs.md#getconfiguredmodelalgorithmassociationrequestrequesttypedef)
- [GetConfiguredModelAlgorithmRequestRequestTypeDef](./type_defs.md#getconfiguredmodelalgorithmrequestrequesttypedef)
- [GetMLConfigurationRequestRequestTypeDef](./type_defs.md#getmlconfigurationrequestrequesttypedef)
- [GetMLInputChannelRequestRequestTypeDef](./type_defs.md#getmlinputchannelrequestrequesttypedef)
- [GetTrainedModelInferenceJobRequestRequestTypeDef](./type_defs.md#gettrainedmodelinferencejobrequestrequesttypedef)
- [InferenceContainerExecutionParametersTypeDef](./type_defs.md#inferencecontainerexecutionparameterstypedef)
- [InferenceResourceConfigTypeDef](./type_defs.md#inferenceresourceconfigtypedef)
- [ModelInferenceDataSourceTypeDef](./type_defs.md#modelinferencedatasourcetypedef)
- [GetTrainedModelRequestRequestTypeDef](./type_defs.md#gettrainedmodelrequestrequesttypedef)
- [GetTrainingDatasetRequestRequestTypeDef](./type_defs.md#gettrainingdatasetrequestrequesttypedef)
- [InferenceReceiverMemberTypeDef](./type_defs.md#inferencereceivermembertypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAudienceExportJobsRequestRequestTypeDef](./type_defs.md#listaudienceexportjobsrequestrequesttypedef)
- [ListAudienceGenerationJobsRequestRequestTypeDef](./type_defs.md#listaudiencegenerationjobsrequestrequesttypedef)
- [ListAudienceModelsRequestRequestTypeDef](./type_defs.md#listaudiencemodelsrequestrequesttypedef)
- [ListCollaborationConfiguredModelAlgorithmAssociationsRequestRequestTypeDef](./type_defs.md#listcollaborationconfiguredmodelalgorithmassociationsrequestrequesttypedef)
- [ListCollaborationMLInputChannelsRequestRequestTypeDef](./type_defs.md#listcollaborationmlinputchannelsrequestrequesttypedef)
- [ListCollaborationTrainedModelExportJobsRequestRequestTypeDef](./type_defs.md#listcollaborationtrainedmodelexportjobsrequestrequesttypedef)
- [ListCollaborationTrainedModelInferenceJobsRequestRequestTypeDef](./type_defs.md#listcollaborationtrainedmodelinferencejobsrequestrequesttypedef)
- [ListCollaborationTrainedModelsRequestRequestTypeDef](./type_defs.md#listcollaborationtrainedmodelsrequestrequesttypedef)
- [ListConfiguredAudienceModelsRequestRequestTypeDef](./type_defs.md#listconfiguredaudiencemodelsrequestrequesttypedef)
- [ListConfiguredModelAlgorithmAssociationsRequestRequestTypeDef](./type_defs.md#listconfiguredmodelalgorithmassociationsrequestrequesttypedef)
- [ListConfiguredModelAlgorithmsRequestRequestTypeDef](./type_defs.md#listconfiguredmodelalgorithmsrequestrequesttypedef)
- [ListMLInputChannelsRequestRequestTypeDef](./type_defs.md#listmlinputchannelsrequestrequesttypedef)
- [MLInputChannelSummaryTypeDef](./type_defs.md#mlinputchannelsummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTrainedModelInferenceJobsRequestRequestTypeDef](./type_defs.md#listtrainedmodelinferencejobsrequestrequesttypedef)
- [ListTrainedModelsRequestRequestTypeDef](./type_defs.md#listtrainedmodelsrequestrequesttypedef)
- [TrainedModelSummaryTypeDef](./type_defs.md#trainedmodelsummarytypedef)
- [ListTrainingDatasetsRequestRequestTypeDef](./type_defs.md#listtrainingdatasetsrequestrequesttypedef)
- [TrainingDatasetSummaryTypeDef](./type_defs.md#trainingdatasetsummarytypedef)
- [LogsConfigurationPolicyOutputTypeDef](./type_defs.md#logsconfigurationpolicyoutputtypedef)
- [LogsConfigurationPolicyTypeDef](./type_defs.md#logsconfigurationpolicytypedef)
- [MetricsConfigurationPolicyTypeDef](./type_defs.md#metricsconfigurationpolicytypedef)
- [ProtectedQuerySQLParametersTypeDef](./type_defs.md#protectedquerysqlparameterstypedef)
- [PutConfiguredAudienceModelPolicyRequestRequestTypeDef](./type_defs.md#putconfiguredaudiencemodelpolicyrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [TrainedModelExportReceiverMemberTypeDef](./type_defs.md#trainedmodelexportreceivermembertypedef)
- [TrainedModelExportsMaxSizeTypeDef](./type_defs.md#trainedmodelexportsmaxsizetypedef)
- [TrainedModelInferenceMaxOutputSizeTypeDef](./type_defs.md#trainedmodelinferencemaxoutputsizetypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [AudienceDestinationTypeDef](./type_defs.md#audiencedestinationtypedef)
- [DestinationTypeDef](./type_defs.md#destinationtypedef)
- [RelevanceMetricTypeDef](./type_defs.md#relevancemetrictypedef)
- [StartAudienceExportJobRequestRequestTypeDef](./type_defs.md#startaudienceexportjobrequestrequesttypedef)
- [AudienceExportJobSummaryTypeDef](./type_defs.md#audienceexportjobsummarytypedef)
- [ColumnSchemaUnionTypeDef](./type_defs.md#columnschemauniontypedef)
- [ComputeConfigurationTypeDef](./type_defs.md#computeconfigurationtypedef)
- [ContainerConfigOutputTypeDef](./type_defs.md#containerconfigoutputtypedef)
- [ContainerConfigTypeDef](./type_defs.md#containerconfigtypedef)
- [CreateAudienceModelRequestRequestTypeDef](./type_defs.md#createaudiencemodelrequestrequesttypedef)
- [CreateAudienceModelResponseTypeDef](./type_defs.md#createaudiencemodelresponsetypedef)
- [CreateConfiguredAudienceModelResponseTypeDef](./type_defs.md#createconfiguredaudiencemodelresponsetypedef)
- [CreateConfiguredModelAlgorithmAssociationResponseTypeDef](./type_defs.md#createconfiguredmodelalgorithmassociationresponsetypedef)
- [CreateConfiguredModelAlgorithmResponseTypeDef](./type_defs.md#createconfiguredmodelalgorithmresponsetypedef)
- [CreateMLInputChannelResponseTypeDef](./type_defs.md#createmlinputchannelresponsetypedef)
- [CreateTrainedModelResponseTypeDef](./type_defs.md#createtrainedmodelresponsetypedef)
- [CreateTrainingDatasetResponseTypeDef](./type_defs.md#createtrainingdatasetresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetAudienceModelResponseTypeDef](./type_defs.md#getaudiencemodelresponsetypedef)
- [GetCollaborationMLInputChannelResponseTypeDef](./type_defs.md#getcollaborationmlinputchannelresponsetypedef)
- [GetConfiguredAudienceModelPolicyResponseTypeDef](./type_defs.md#getconfiguredaudiencemodelpolicyresponsetypedef)
- [ListAudienceGenerationJobsResponseTypeDef](./type_defs.md#listaudiencegenerationjobsresponsetypedef)
- [ListAudienceModelsResponseTypeDef](./type_defs.md#listaudiencemodelsresponsetypedef)
- [ListCollaborationConfiguredModelAlgorithmAssociationsResponseTypeDef](./type_defs.md#listcollaborationconfiguredmodelalgorithmassociationsresponsetypedef)
- [ListCollaborationMLInputChannelsResponseTypeDef](./type_defs.md#listcollaborationmlinputchannelsresponsetypedef)
- [ListCollaborationTrainedModelsResponseTypeDef](./type_defs.md#listcollaborationtrainedmodelsresponsetypedef)
- [ListConfiguredModelAlgorithmAssociationsResponseTypeDef](./type_defs.md#listconfiguredmodelalgorithmassociationsresponsetypedef)
- [ListConfiguredModelAlgorithmsResponseTypeDef](./type_defs.md#listconfiguredmodelalgorithmsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PutConfiguredAudienceModelPolicyResponseTypeDef](./type_defs.md#putconfiguredaudiencemodelpolicyresponsetypedef)
- [StartAudienceGenerationJobResponseTypeDef](./type_defs.md#startaudiencegenerationjobresponsetypedef)
- [StartTrainedModelInferenceJobResponseTypeDef](./type_defs.md#starttrainedmodelinferencejobresponsetypedef)
- [UpdateConfiguredAudienceModelResponseTypeDef](./type_defs.md#updateconfiguredaudiencemodelresponsetypedef)
- [CreateTrainedModelRequestRequestTypeDef](./type_defs.md#createtrainedmodelrequestrequesttypedef)
- [GetCollaborationTrainedModelResponseTypeDef](./type_defs.md#getcollaborationtrainedmodelresponsetypedef)
- [GetTrainedModelResponseTypeDef](./type_defs.md#gettrainedmodelresponsetypedef)
- [DataSourceTypeDef](./type_defs.md#datasourcetypedef)
- [InferenceOutputConfigurationOutputTypeDef](./type_defs.md#inferenceoutputconfigurationoutputtypedef)
- [InferenceOutputConfigurationTypeDef](./type_defs.md#inferenceoutputconfigurationtypedef)
- [ListAudienceExportJobsRequestPaginateTypeDef](./type_defs.md#listaudienceexportjobsrequestpaginatetypedef)
- [ListAudienceGenerationJobsRequestPaginateTypeDef](./type_defs.md#listaudiencegenerationjobsrequestpaginatetypedef)
- [ListAudienceModelsRequestPaginateTypeDef](./type_defs.md#listaudiencemodelsrequestpaginatetypedef)
- [ListCollaborationConfiguredModelAlgorithmAssociationsRequestPaginateTypeDef](./type_defs.md#listcollaborationconfiguredmodelalgorithmassociationsrequestpaginatetypedef)
- [ListCollaborationMLInputChannelsRequestPaginateTypeDef](./type_defs.md#listcollaborationmlinputchannelsrequestpaginatetypedef)
- [ListCollaborationTrainedModelExportJobsRequestPaginateTypeDef](./type_defs.md#listcollaborationtrainedmodelexportjobsrequestpaginatetypedef)
- [ListCollaborationTrainedModelInferenceJobsRequestPaginateTypeDef](./type_defs.md#listcollaborationtrainedmodelinferencejobsrequestpaginatetypedef)
- [ListCollaborationTrainedModelsRequestPaginateTypeDef](./type_defs.md#listcollaborationtrainedmodelsrequestpaginatetypedef)
- [ListConfiguredAudienceModelsRequestPaginateTypeDef](./type_defs.md#listconfiguredaudiencemodelsrequestpaginatetypedef)
- [ListConfiguredModelAlgorithmAssociationsRequestPaginateTypeDef](./type_defs.md#listconfiguredmodelalgorithmassociationsrequestpaginatetypedef)
- [ListConfiguredModelAlgorithmsRequestPaginateTypeDef](./type_defs.md#listconfiguredmodelalgorithmsrequestpaginatetypedef)
- [ListMLInputChannelsRequestPaginateTypeDef](./type_defs.md#listmlinputchannelsrequestpaginatetypedef)
- [ListTrainedModelInferenceJobsRequestPaginateTypeDef](./type_defs.md#listtrainedmodelinferencejobsrequestpaginatetypedef)
- [ListTrainedModelsRequestPaginateTypeDef](./type_defs.md#listtrainedmodelsrequestpaginatetypedef)
- [ListTrainingDatasetsRequestPaginateTypeDef](./type_defs.md#listtrainingdatasetsrequestpaginatetypedef)
- [ListMLInputChannelsResponseTypeDef](./type_defs.md#listmlinputchannelsresponsetypedef)
- [ListTrainedModelsResponseTypeDef](./type_defs.md#listtrainedmodelsresponsetypedef)
- [ListTrainingDatasetsResponseTypeDef](./type_defs.md#listtrainingdatasetsresponsetypedef)
- [LogsConfigurationPolicyUnionTypeDef](./type_defs.md#logsconfigurationpolicyuniontypedef)
- [TrainedModelsConfigurationPolicyOutputTypeDef](./type_defs.md#trainedmodelsconfigurationpolicyoutputtypedef)
- [TrainedModelsConfigurationPolicyTypeDef](./type_defs.md#trainedmodelsconfigurationpolicytypedef)
- [ProtectedQuerySQLParametersUnionTypeDef](./type_defs.md#protectedquerysqlparametersuniontypedef)
- [TrainedModelExportOutputConfigurationOutputTypeDef](./type_defs.md#trainedmodelexportoutputconfigurationoutputtypedef)
- [TrainedModelExportOutputConfigurationTypeDef](./type_defs.md#trainedmodelexportoutputconfigurationtypedef)
- [TrainedModelExportsConfigurationPolicyOutputTypeDef](./type_defs.md#trainedmodelexportsconfigurationpolicyoutputtypedef)
- [TrainedModelExportsConfigurationPolicyTypeDef](./type_defs.md#trainedmodelexportsconfigurationpolicytypedef)
- [TrainedModelInferenceJobsConfigurationPolicyOutputTypeDef](./type_defs.md#trainedmodelinferencejobsconfigurationpolicyoutputtypedef)
- [ConfiguredAudienceModelOutputConfigTypeDef](./type_defs.md#configuredaudiencemodeloutputconfigtypedef)
- [MLOutputConfigurationTypeDef](./type_defs.md#mloutputconfigurationtypedef)
- [AudienceQualityMetricsTypeDef](./type_defs.md#audiencequalitymetricstypedef)
- [ListAudienceExportJobsResponseTypeDef](./type_defs.md#listaudienceexportjobsresponsetypedef)
- [AudienceGenerationJobDataSourceOutputTypeDef](./type_defs.md#audiencegenerationjobdatasourceoutputtypedef)
- [ProtectedQueryInputParametersOutputTypeDef](./type_defs.md#protectedqueryinputparametersoutputtypedef)
- [GetConfiguredModelAlgorithmResponseTypeDef](./type_defs.md#getconfiguredmodelalgorithmresponsetypedef)
- [CreateConfiguredModelAlgorithmRequestRequestTypeDef](./type_defs.md#createconfiguredmodelalgorithmrequestrequesttypedef)
- [DatasetInputConfigOutputTypeDef](./type_defs.md#datasetinputconfigoutputtypedef)
- [DatasetInputConfigTypeDef](./type_defs.md#datasetinputconfigtypedef)
- [CollaborationTrainedModelInferenceJobSummaryTypeDef](./type_defs.md#collaborationtrainedmodelinferencejobsummarytypedef)
- [GetTrainedModelInferenceJobResponseTypeDef](./type_defs.md#gettrainedmodelinferencejobresponsetypedef)
- [TrainedModelInferenceJobSummaryTypeDef](./type_defs.md#trainedmodelinferencejobsummarytypedef)
- [StartTrainedModelInferenceJobRequestRequestTypeDef](./type_defs.md#starttrainedmodelinferencejobrequestrequesttypedef)
- [TrainedModelInferenceJobsConfigurationPolicyTypeDef](./type_defs.md#trainedmodelinferencejobsconfigurationpolicytypedef)
- [TrainedModelsConfigurationPolicyUnionTypeDef](./type_defs.md#trainedmodelsconfigurationpolicyuniontypedef)
- [AudienceGenerationJobDataSourceTypeDef](./type_defs.md#audiencegenerationjobdatasourcetypedef)
- [ProtectedQueryInputParametersTypeDef](./type_defs.md#protectedqueryinputparameterstypedef)
- [CollaborationTrainedModelExportJobSummaryTypeDef](./type_defs.md#collaborationtrainedmodelexportjobsummarytypedef)
- [StartTrainedModelExportJobRequestRequestTypeDef](./type_defs.md#starttrainedmodelexportjobrequestrequesttypedef)
- [TrainedModelExportsConfigurationPolicyUnionTypeDef](./type_defs.md#trainedmodelexportsconfigurationpolicyuniontypedef)
- [PrivacyConfigurationPoliciesOutputTypeDef](./type_defs.md#privacyconfigurationpoliciesoutputtypedef)
- [ConfiguredAudienceModelSummaryTypeDef](./type_defs.md#configuredaudiencemodelsummarytypedef)
- [CreateConfiguredAudienceModelRequestRequestTypeDef](./type_defs.md#createconfiguredaudiencemodelrequestrequesttypedef)
- [GetConfiguredAudienceModelResponseTypeDef](./type_defs.md#getconfiguredaudiencemodelresponsetypedef)
- [UpdateConfiguredAudienceModelRequestRequestTypeDef](./type_defs.md#updateconfiguredaudiencemodelrequestrequesttypedef)
- [GetMLConfigurationResponseTypeDef](./type_defs.md#getmlconfigurationresponsetypedef)
- [PutMLConfigurationRequestRequestTypeDef](./type_defs.md#putmlconfigurationrequestrequesttypedef)
- [GetAudienceGenerationJobResponseTypeDef](./type_defs.md#getaudiencegenerationjobresponsetypedef)
- [InputChannelDataSourceOutputTypeDef](./type_defs.md#inputchanneldatasourceoutputtypedef)
- [DatasetOutputTypeDef](./type_defs.md#datasetoutputtypedef)
- [DatasetInputConfigUnionTypeDef](./type_defs.md#datasetinputconfiguniontypedef)
- [ListCollaborationTrainedModelInferenceJobsResponseTypeDef](./type_defs.md#listcollaborationtrainedmodelinferencejobsresponsetypedef)
- [ListTrainedModelInferenceJobsResponseTypeDef](./type_defs.md#listtrainedmodelinferencejobsresponsetypedef)
- [TrainedModelInferenceJobsConfigurationPolicyUnionTypeDef](./type_defs.md#trainedmodelinferencejobsconfigurationpolicyuniontypedef)
- [StartAudienceGenerationJobRequestRequestTypeDef](./type_defs.md#startaudiencegenerationjobrequestrequesttypedef)
- [ProtectedQueryInputParametersUnionTypeDef](./type_defs.md#protectedqueryinputparametersuniontypedef)
- [ListCollaborationTrainedModelExportJobsResponseTypeDef](./type_defs.md#listcollaborationtrainedmodelexportjobsresponsetypedef)
- [PrivacyConfigurationOutputTypeDef](./type_defs.md#privacyconfigurationoutputtypedef)
- [ListConfiguredAudienceModelsResponseTypeDef](./type_defs.md#listconfiguredaudiencemodelsresponsetypedef)
- [InputChannelOutputTypeDef](./type_defs.md#inputchanneloutputtypedef)
- [GetTrainingDatasetResponseTypeDef](./type_defs.md#gettrainingdatasetresponsetypedef)
- [DatasetTypeDef](./type_defs.md#datasettypedef)
- [PrivacyConfigurationPoliciesTypeDef](./type_defs.md#privacyconfigurationpoliciestypedef)
- [InputChannelDataSourceTypeDef](./type_defs.md#inputchanneldatasourcetypedef)
- [GetCollaborationConfiguredModelAlgorithmAssociationResponseTypeDef](./type_defs.md#getcollaborationconfiguredmodelalgorithmassociationresponsetypedef)
- [GetConfiguredModelAlgorithmAssociationResponseTypeDef](./type_defs.md#getconfiguredmodelalgorithmassociationresponsetypedef)
- [GetMLInputChannelResponseTypeDef](./type_defs.md#getmlinputchannelresponsetypedef)
- [DatasetUnionTypeDef](./type_defs.md#datasetuniontypedef)
- [PrivacyConfigurationPoliciesUnionTypeDef](./type_defs.md#privacyconfigurationpoliciesuniontypedef)
- [InputChannelDataSourceUnionTypeDef](./type_defs.md#inputchanneldatasourceuniontypedef)
- [CreateTrainingDatasetRequestRequestTypeDef](./type_defs.md#createtrainingdatasetrequestrequesttypedef)
- [PrivacyConfigurationTypeDef](./type_defs.md#privacyconfigurationtypedef)
- [InputChannelTypeDef](./type_defs.md#inputchanneltypedef)
- [CreateConfiguredModelAlgorithmAssociationRequestRequestTypeDef](./type_defs.md#createconfiguredmodelalgorithmassociationrequestrequesttypedef)
- [CreateMLInputChannelRequestRequestTypeDef](./type_defs.md#createmlinputchannelrequestrequesttypedef)

