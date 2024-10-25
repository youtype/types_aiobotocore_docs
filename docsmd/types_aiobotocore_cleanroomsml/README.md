# CleanRoomsML module

> [Index](../README.md) > CleanRoomsML


!!! note ""

    Auto-generated documentation for [CleanRoomsML](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML)
    type annotations stubs module [types-aiobotocore-cleanroomsml](https://pypi.org/project/types-aiobotocore-cleanroomsml/).

## How to install



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
- [ListConfiguredAudienceModelsPaginator](./paginators.md#listconfiguredaudiencemodelspaginator)
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
- [ListAudienceExportJobsPaginatorName](./literals.md#listaudienceexportjobspaginatorname)
- [ListAudienceGenerationJobsPaginatorName](./literals.md#listaudiencegenerationjobspaginatorname)
- [ListAudienceModelsPaginatorName](./literals.md#listaudiencemodelspaginatorname)
- [ListConfiguredAudienceModelsPaginatorName](./literals.md#listconfiguredaudiencemodelspaginatorname)
- [ListTrainingDatasetsPaginatorName](./literals.md#listtrainingdatasetspaginatorname)
- [PolicyExistenceConditionType](./literals.md#policyexistenceconditiontype)
- [SharedAudienceMetricsType](./literals.md#sharedaudiencemetricstype)
- [TagOnCreatePolicyType](./literals.md#tagoncreatepolicytype)
- [TrainingDatasetStatusType](./literals.md#trainingdatasetstatustype)
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
- [ColumnSchemaOutputTypeDef](./type_defs.md#columnschemaoutputtypedef)
- [ColumnSchemaTypeDef](./type_defs.md#columnschematypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GlueDataSourceTypeDef](./type_defs.md#gluedatasourcetypedef)
- [DeleteAudienceGenerationJobRequestRequestTypeDef](./type_defs.md#deleteaudiencegenerationjobrequestrequesttypedef)
- [DeleteAudienceModelRequestRequestTypeDef](./type_defs.md#deleteaudiencemodelrequestrequesttypedef)
- [DeleteConfiguredAudienceModelPolicyRequestRequestTypeDef](./type_defs.md#deleteconfiguredaudiencemodelpolicyrequestrequesttypedef)
- [DeleteConfiguredAudienceModelRequestRequestTypeDef](./type_defs.md#deleteconfiguredaudiencemodelrequestrequesttypedef)
- [DeleteTrainingDatasetRequestRequestTypeDef](./type_defs.md#deletetrainingdatasetrequestrequesttypedef)
- [GetAudienceGenerationJobRequestRequestTypeDef](./type_defs.md#getaudiencegenerationjobrequestrequesttypedef)
- [GetAudienceModelRequestRequestTypeDef](./type_defs.md#getaudiencemodelrequestrequesttypedef)
- [GetConfiguredAudienceModelPolicyRequestRequestTypeDef](./type_defs.md#getconfiguredaudiencemodelpolicyrequestrequesttypedef)
- [GetConfiguredAudienceModelRequestRequestTypeDef](./type_defs.md#getconfiguredaudiencemodelrequestrequesttypedef)
- [GetTrainingDatasetRequestRequestTypeDef](./type_defs.md#gettrainingdatasetrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAudienceExportJobsRequestRequestTypeDef](./type_defs.md#listaudienceexportjobsrequestrequesttypedef)
- [ListAudienceGenerationJobsRequestRequestTypeDef](./type_defs.md#listaudiencegenerationjobsrequestrequesttypedef)
- [ListAudienceModelsRequestRequestTypeDef](./type_defs.md#listaudiencemodelsrequestrequesttypedef)
- [ListConfiguredAudienceModelsRequestRequestTypeDef](./type_defs.md#listconfiguredaudiencemodelsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTrainingDatasetsRequestRequestTypeDef](./type_defs.md#listtrainingdatasetsrequestrequesttypedef)
- [TrainingDatasetSummaryTypeDef](./type_defs.md#trainingdatasetsummarytypedef)
- [ProtectedQuerySQLParametersTypeDef](./type_defs.md#protectedquerysqlparameterstypedef)
- [PutConfiguredAudienceModelPolicyRequestRequestTypeDef](./type_defs.md#putconfiguredaudiencemodelpolicyrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [AudienceDestinationTypeDef](./type_defs.md#audiencedestinationtypedef)
- [RelevanceMetricTypeDef](./type_defs.md#relevancemetrictypedef)
- [StartAudienceExportJobRequestRequestTypeDef](./type_defs.md#startaudienceexportjobrequestrequesttypedef)
- [AudienceExportJobSummaryTypeDef](./type_defs.md#audienceexportjobsummarytypedef)
- [AudienceGenerationJobDataSourceOutputTypeDef](./type_defs.md#audiencegenerationjobdatasourceoutputtypedef)
- [ColumnSchemaUnionTypeDef](./type_defs.md#columnschemauniontypedef)
- [CreateAudienceModelRequestRequestTypeDef](./type_defs.md#createaudiencemodelrequestrequesttypedef)
- [CreateAudienceModelResponseTypeDef](./type_defs.md#createaudiencemodelresponsetypedef)
- [CreateConfiguredAudienceModelResponseTypeDef](./type_defs.md#createconfiguredaudiencemodelresponsetypedef)
- [CreateTrainingDatasetResponseTypeDef](./type_defs.md#createtrainingdatasetresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetAudienceModelResponseTypeDef](./type_defs.md#getaudiencemodelresponsetypedef)
- [GetConfiguredAudienceModelPolicyResponseTypeDef](./type_defs.md#getconfiguredaudiencemodelpolicyresponsetypedef)
- [ListAudienceGenerationJobsResponseTypeDef](./type_defs.md#listaudiencegenerationjobsresponsetypedef)
- [ListAudienceModelsResponseTypeDef](./type_defs.md#listaudiencemodelsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PutConfiguredAudienceModelPolicyResponseTypeDef](./type_defs.md#putconfiguredaudiencemodelpolicyresponsetypedef)
- [StartAudienceGenerationJobResponseTypeDef](./type_defs.md#startaudiencegenerationjobresponsetypedef)
- [UpdateConfiguredAudienceModelResponseTypeDef](./type_defs.md#updateconfiguredaudiencemodelresponsetypedef)
- [DataSourceTypeDef](./type_defs.md#datasourcetypedef)
- [ListAudienceExportJobsRequestListAudienceExportJobsPaginateTypeDef](./type_defs.md#listaudienceexportjobsrequestlistaudienceexportjobspaginatetypedef)
- [ListAudienceGenerationJobsRequestListAudienceGenerationJobsPaginateTypeDef](./type_defs.md#listaudiencegenerationjobsrequestlistaudiencegenerationjobspaginatetypedef)
- [ListAudienceModelsRequestListAudienceModelsPaginateTypeDef](./type_defs.md#listaudiencemodelsrequestlistaudiencemodelspaginatetypedef)
- [ListConfiguredAudienceModelsRequestListConfiguredAudienceModelsPaginateTypeDef](./type_defs.md#listconfiguredaudiencemodelsrequestlistconfiguredaudiencemodelspaginatetypedef)
- [ListTrainingDatasetsRequestListTrainingDatasetsPaginateTypeDef](./type_defs.md#listtrainingdatasetsrequestlisttrainingdatasetspaginatetypedef)
- [ListTrainingDatasetsResponseTypeDef](./type_defs.md#listtrainingdatasetsresponsetypedef)
- [ProtectedQuerySQLParametersUnionTypeDef](./type_defs.md#protectedquerysqlparametersuniontypedef)
- [ConfiguredAudienceModelOutputConfigTypeDef](./type_defs.md#configuredaudiencemodeloutputconfigtypedef)
- [AudienceQualityMetricsTypeDef](./type_defs.md#audiencequalitymetricstypedef)
- [ListAudienceExportJobsResponseTypeDef](./type_defs.md#listaudienceexportjobsresponsetypedef)
- [DatasetInputConfigOutputTypeDef](./type_defs.md#datasetinputconfigoutputtypedef)
- [DatasetInputConfigTypeDef](./type_defs.md#datasetinputconfigtypedef)
- [AudienceGenerationJobDataSourceTypeDef](./type_defs.md#audiencegenerationjobdatasourcetypedef)
- [ConfiguredAudienceModelSummaryTypeDef](./type_defs.md#configuredaudiencemodelsummarytypedef)
- [CreateConfiguredAudienceModelRequestRequestTypeDef](./type_defs.md#createconfiguredaudiencemodelrequestrequesttypedef)
- [GetConfiguredAudienceModelResponseTypeDef](./type_defs.md#getconfiguredaudiencemodelresponsetypedef)
- [UpdateConfiguredAudienceModelRequestRequestTypeDef](./type_defs.md#updateconfiguredaudiencemodelrequestrequesttypedef)
- [GetAudienceGenerationJobResponseTypeDef](./type_defs.md#getaudiencegenerationjobresponsetypedef)
- [DatasetOutputTypeDef](./type_defs.md#datasetoutputtypedef)
- [DatasetInputConfigUnionTypeDef](./type_defs.md#datasetinputconfiguniontypedef)
- [StartAudienceGenerationJobRequestRequestTypeDef](./type_defs.md#startaudiencegenerationjobrequestrequesttypedef)
- [ListConfiguredAudienceModelsResponseTypeDef](./type_defs.md#listconfiguredaudiencemodelsresponsetypedef)
- [GetTrainingDatasetResponseTypeDef](./type_defs.md#gettrainingdatasetresponsetypedef)
- [DatasetTypeDef](./type_defs.md#datasettypedef)
- [DatasetUnionTypeDef](./type_defs.md#datasetuniontypedef)
- [CreateTrainingDatasetRequestRequestTypeDef](./type_defs.md#createtrainingdatasetrequestrequesttypedef)

