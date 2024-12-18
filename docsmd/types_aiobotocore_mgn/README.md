# Mgn module

> [Index](../README.md) > Mgn


!!! note ""

    Auto-generated documentation for [Mgn](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
    type annotations stubs module [types-aiobotocore-mgn](https://pypi.org/project/types-aiobotocore-mgn/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Mgn` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Mgn` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[mgn]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[mgn]'

# standalone installation
python -m pip install types-aiobotocore-mgn
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-mgn
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MgnClient

Type annotations and code completion for  `#!python session.create_client("mgn")` as [MgnClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#Mgn.Client)

```python
# MgnClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgn.client import MgnClient


session = get_session()
async with session.create_client("mgn") as client:
    client: MgnClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("mgn").get_paginator("...")`.

```python
# DescribeJobLogItemsPaginator usage example

from types_aiobotocore_mgn.paginator import DescribeJobLogItemsPaginator

def get_describe_job_log_items_paginator() -> DescribeJobLogItemsPaginator:
    return client.get_paginator("describe_job_log_items"))
```

- [DescribeJobLogItemsPaginator](./paginators.md#describejoblogitemspaginator)
- [DescribeJobsPaginator](./paginators.md#describejobspaginator)
- [DescribeLaunchConfigurationTemplatesPaginator](./paginators.md#describelaunchconfigurationtemplatespaginator)
- [DescribeReplicationConfigurationTemplatesPaginator](./paginators.md#describereplicationconfigurationtemplatespaginator)
- [DescribeSourceServersPaginator](./paginators.md#describesourceserverspaginator)
- [DescribeVcenterClientsPaginator](./paginators.md#describevcenterclientspaginator)
- [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
- [ListConnectorsPaginator](./paginators.md#listconnectorspaginator)
- [ListExportErrorsPaginator](./paginators.md#listexporterrorspaginator)
- [ListExportsPaginator](./paginators.md#listexportspaginator)
- [ListImportErrorsPaginator](./paginators.md#listimporterrorspaginator)
- [ListImportsPaginator](./paginators.md#listimportspaginator)
- [ListManagedAccountsPaginator](./paginators.md#listmanagedaccountspaginator)
- [ListSourceServerActionsPaginator](./paginators.md#listsourceserveractionspaginator)
- [ListTemplateActionsPaginator](./paginators.md#listtemplateactionspaginator)
- [ListWavesPaginator](./paginators.md#listwavespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActionCategoryType usage example

from types_aiobotocore_mgn.literals import ActionCategoryType

def get_value() -> ActionCategoryType:
    return "BACKUP"
```

- [ActionCategoryType](./literals.md#actioncategorytype)
- [ApplicationHealthStatusType](./literals.md#applicationhealthstatustype)
- [ApplicationProgressStatusType](./literals.md#applicationprogressstatustype)
- [BootModeType](./literals.md#bootmodetype)
- [ChangeServerLifeCycleStateSourceServerLifecycleStateType](./literals.md#changeserverlifecyclestatesourceserverlifecyclestatetype)
- [DataReplicationErrorStringType](./literals.md#datareplicationerrorstringtype)
- [DataReplicationInitiationStepNameType](./literals.md#datareplicationinitiationstepnametype)
- [DataReplicationInitiationStepStatusType](./literals.md#datareplicationinitiationstepstatustype)
- [DataReplicationStateType](./literals.md#datareplicationstatetype)
- [DescribeJobLogItemsPaginatorName](./literals.md#describejoblogitemspaginatorname)
- [DescribeJobsPaginatorName](./literals.md#describejobspaginatorname)
- [DescribeLaunchConfigurationTemplatesPaginatorName](./literals.md#describelaunchconfigurationtemplatespaginatorname)
- [DescribeReplicationConfigurationTemplatesPaginatorName](./literals.md#describereplicationconfigurationtemplatespaginatorname)
- [DescribeSourceServersPaginatorName](./literals.md#describesourceserverspaginatorname)
- [DescribeVcenterClientsPaginatorName](./literals.md#describevcenterclientspaginatorname)
- [ExportStatusType](./literals.md#exportstatustype)
- [FirstBootType](./literals.md#firstboottype)
- [ImportErrorTypeType](./literals.md#importerrortypetype)
- [ImportStatusType](./literals.md#importstatustype)
- [InitiatedByType](./literals.md#initiatedbytype)
- [JobLogEventType](./literals.md#joblogeventtype)
- [JobStatusType](./literals.md#jobstatustype)
- [JobTypeType](./literals.md#jobtypetype)
- [LaunchDispositionType](./literals.md#launchdispositiontype)
- [LaunchStatusType](./literals.md#launchstatustype)
- [LifeCycleStateType](./literals.md#lifecyclestatetype)
- [ListApplicationsPaginatorName](./literals.md#listapplicationspaginatorname)
- [ListConnectorsPaginatorName](./literals.md#listconnectorspaginatorname)
- [ListExportErrorsPaginatorName](./literals.md#listexporterrorspaginatorname)
- [ListExportsPaginatorName](./literals.md#listexportspaginatorname)
- [ListImportErrorsPaginatorName](./literals.md#listimporterrorspaginatorname)
- [ListImportsPaginatorName](./literals.md#listimportspaginatorname)
- [ListManagedAccountsPaginatorName](./literals.md#listmanagedaccountspaginatorname)
- [ListSourceServerActionsPaginatorName](./literals.md#listsourceserveractionspaginatorname)
- [ListTemplateActionsPaginatorName](./literals.md#listtemplateactionspaginatorname)
- [ListWavesPaginatorName](./literals.md#listwavespaginatorname)
- [PostLaunchActionExecutionStatusType](./literals.md#postlaunchactionexecutionstatustype)
- [PostLaunchActionsDeploymentTypeType](./literals.md#postlaunchactionsdeploymenttypetype)
- [ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype)
- [ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype)
- [ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype)
- [ReplicationConfigurationReplicatedDiskStagingDiskTypeType](./literals.md#replicationconfigurationreplicateddiskstagingdisktypetype)
- [ReplicationTypeType](./literals.md#replicationtypetype)
- [SsmDocumentTypeType](./literals.md#ssmdocumenttypetype)
- [SsmParameterStoreParameterTypeType](./literals.md#ssmparameterstoreparametertypetype)
- [TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype)
- [VolumeTypeType](./literals.md#volumetypetype)
- [WaveHealthStatusType](./literals.md#wavehealthstatustype)
- [WaveProgressStatusType](./literals.md#waveprogressstatustype)
- [MgnServiceName](./literals.md#mgnservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ApplicationAggregatedStatusTypeDef](./type_defs.md#applicationaggregatedstatustypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ArchiveApplicationRequestRequestTypeDef](./type_defs.md#archiveapplicationrequestrequesttypedef)
- [ArchiveWaveRequestRequestTypeDef](./type_defs.md#archivewaverequestrequesttypedef)
- [AssociateApplicationsRequestRequestTypeDef](./type_defs.md#associateapplicationsrequestrequesttypedef)
- [AssociateSourceServersRequestRequestTypeDef](./type_defs.md#associatesourceserversrequestrequesttypedef)
- [CPUTypeDef](./type_defs.md#cputypedef)
- [ChangeServerLifeCycleStateSourceServerLifecycleTypeDef](./type_defs.md#changeserverlifecyclestatesourceserverlifecycletypedef)
- [ConnectorSsmCommandConfigTypeDef](./type_defs.md#connectorssmcommandconfigtypedef)
- [CreateApplicationRequestRequestTypeDef](./type_defs.md#createapplicationrequestrequesttypedef)
- [LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef)
- [LicensingTypeDef](./type_defs.md#licensingtypedef)
- [CreateReplicationConfigurationTemplateRequestRequestTypeDef](./type_defs.md#createreplicationconfigurationtemplaterequestrequesttypedef)
- [CreateWaveRequestRequestTypeDef](./type_defs.md#createwaverequestrequesttypedef)
- [DataReplicationErrorTypeDef](./type_defs.md#datareplicationerrortypedef)
- [DataReplicationInfoReplicatedDiskTypeDef](./type_defs.md#datareplicationinforeplicateddisktypedef)
- [DataReplicationInitiationStepTypeDef](./type_defs.md#datareplicationinitiationsteptypedef)
- [DeleteApplicationRequestRequestTypeDef](./type_defs.md#deleteapplicationrequestrequesttypedef)
- [DeleteConnectorRequestRequestTypeDef](./type_defs.md#deleteconnectorrequestrequesttypedef)
- [DeleteJobRequestRequestTypeDef](./type_defs.md#deletejobrequestrequesttypedef)
- [DeleteLaunchConfigurationTemplateRequestRequestTypeDef](./type_defs.md#deletelaunchconfigurationtemplaterequestrequesttypedef)
- [DeleteReplicationConfigurationTemplateRequestRequestTypeDef](./type_defs.md#deletereplicationconfigurationtemplaterequestrequesttypedef)
- [DeleteSourceServerRequestRequestTypeDef](./type_defs.md#deletesourceserverrequestrequesttypedef)
- [DeleteVcenterClientRequestRequestTypeDef](./type_defs.md#deletevcenterclientrequestrequesttypedef)
- [DeleteWaveRequestRequestTypeDef](./type_defs.md#deletewaverequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeJobLogItemsRequestRequestTypeDef](./type_defs.md#describejoblogitemsrequestrequesttypedef)
- [DescribeJobsRequestFiltersTypeDef](./type_defs.md#describejobsrequestfilterstypedef)
- [DescribeLaunchConfigurationTemplatesRequestRequestTypeDef](./type_defs.md#describelaunchconfigurationtemplatesrequestrequesttypedef)
- [DescribeReplicationConfigurationTemplatesRequestRequestTypeDef](./type_defs.md#describereplicationconfigurationtemplatesrequestrequesttypedef)
- [ReplicationConfigurationTemplateTypeDef](./type_defs.md#replicationconfigurationtemplatetypedef)
- [DescribeSourceServersRequestFiltersTypeDef](./type_defs.md#describesourceserversrequestfilterstypedef)
- [DescribeVcenterClientsRequestRequestTypeDef](./type_defs.md#describevcenterclientsrequestrequesttypedef)
- [VcenterClientTypeDef](./type_defs.md#vcenterclienttypedef)
- [DisassociateApplicationsRequestRequestTypeDef](./type_defs.md#disassociateapplicationsrequestrequesttypedef)
- [DisassociateSourceServersRequestRequestTypeDef](./type_defs.md#disassociatesourceserversrequestrequesttypedef)
- [DisconnectFromServiceRequestRequestTypeDef](./type_defs.md#disconnectfromservicerequestrequesttypedef)
- [DiskTypeDef](./type_defs.md#disktypedef)
- [ExportErrorDataTypeDef](./type_defs.md#exporterrordatatypedef)
- [ExportTaskSummaryTypeDef](./type_defs.md#exporttasksummarytypedef)
- [FinalizeCutoverRequestRequestTypeDef](./type_defs.md#finalizecutoverrequestrequesttypedef)
- [GetLaunchConfigurationRequestRequestTypeDef](./type_defs.md#getlaunchconfigurationrequestrequesttypedef)
- [GetReplicationConfigurationRequestRequestTypeDef](./type_defs.md#getreplicationconfigurationrequestrequesttypedef)
- [IdentificationHintsTypeDef](./type_defs.md#identificationhintstypedef)
- [ImportErrorDataTypeDef](./type_defs.md#importerrordatatypedef)
- [ImportTaskSummaryApplicationsTypeDef](./type_defs.md#importtasksummaryapplicationstypedef)
- [ImportTaskSummaryServersTypeDef](./type_defs.md#importtasksummaryserverstypedef)
- [ImportTaskSummaryWavesTypeDef](./type_defs.md#importtasksummarywavestypedef)
- [S3BucketSourceTypeDef](./type_defs.md#s3bucketsourcetypedef)
- [JobLogEventDataTypeDef](./type_defs.md#joblogeventdatatypedef)
- [LaunchedInstanceTypeDef](./type_defs.md#launchedinstancetypedef)
- [LifeCycleLastCutoverFinalizedTypeDef](./type_defs.md#lifecyclelastcutoverfinalizedtypedef)
- [LifeCycleLastCutoverInitiatedTypeDef](./type_defs.md#lifecyclelastcutoverinitiatedtypedef)
- [LifeCycleLastCutoverRevertedTypeDef](./type_defs.md#lifecyclelastcutoverrevertedtypedef)
- [LifeCycleLastTestFinalizedTypeDef](./type_defs.md#lifecyclelasttestfinalizedtypedef)
- [LifeCycleLastTestInitiatedTypeDef](./type_defs.md#lifecyclelasttestinitiatedtypedef)
- [LifeCycleLastTestRevertedTypeDef](./type_defs.md#lifecyclelasttestrevertedtypedef)
- [ListApplicationsRequestFiltersTypeDef](./type_defs.md#listapplicationsrequestfilterstypedef)
- [ListConnectorsRequestFiltersTypeDef](./type_defs.md#listconnectorsrequestfilterstypedef)
- [ListExportErrorsRequestRequestTypeDef](./type_defs.md#listexporterrorsrequestrequesttypedef)
- [ListExportsRequestFiltersTypeDef](./type_defs.md#listexportsrequestfilterstypedef)
- [ListImportErrorsRequestRequestTypeDef](./type_defs.md#listimporterrorsrequestrequesttypedef)
- [ListImportsRequestFiltersTypeDef](./type_defs.md#listimportsrequestfilterstypedef)
- [ListManagedAccountsRequestRequestTypeDef](./type_defs.md#listmanagedaccountsrequestrequesttypedef)
- [ManagedAccountTypeDef](./type_defs.md#managedaccounttypedef)
- [SourceServerActionsRequestFiltersTypeDef](./type_defs.md#sourceserveractionsrequestfilterstypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [TemplateActionsRequestFiltersTypeDef](./type_defs.md#templateactionsrequestfilterstypedef)
- [ListWavesRequestFiltersTypeDef](./type_defs.md#listwavesrequestfilterstypedef)
- [MarkAsArchivedRequestRequestTypeDef](./type_defs.md#markasarchivedrequestrequesttypedef)
- [NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef)
- [OSTypeDef](./type_defs.md#ostypedef)
- [PauseReplicationRequestRequestTypeDef](./type_defs.md#pausereplicationrequestrequesttypedef)
- [SsmExternalParameterTypeDef](./type_defs.md#ssmexternalparametertypedef)
- [SsmParameterStoreParameterTypeDef](./type_defs.md#ssmparameterstoreparametertypedef)
- [RemoveSourceServerActionRequestRequestTypeDef](./type_defs.md#removesourceserveractionrequestrequesttypedef)
- [RemoveTemplateActionRequestRequestTypeDef](./type_defs.md#removetemplateactionrequestrequesttypedef)
- [ReplicationConfigurationReplicatedDiskTypeDef](./type_defs.md#replicationconfigurationreplicateddisktypedef)
- [ResumeReplicationRequestRequestTypeDef](./type_defs.md#resumereplicationrequestrequesttypedef)
- [RetryDataReplicationRequestRequestTypeDef](./type_defs.md#retrydatareplicationrequestrequesttypedef)
- [SourceServerConnectorActionTypeDef](./type_defs.md#sourceserverconnectoractiontypedef)
- [StartCutoverRequestRequestTypeDef](./type_defs.md#startcutoverrequestrequesttypedef)
- [StartExportRequestRequestTypeDef](./type_defs.md#startexportrequestrequesttypedef)
- [StartReplicationRequestRequestTypeDef](./type_defs.md#startreplicationrequestrequesttypedef)
- [StartTestRequestRequestTypeDef](./type_defs.md#starttestrequestrequesttypedef)
- [StopReplicationRequestRequestTypeDef](./type_defs.md#stopreplicationrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [TerminateTargetInstancesRequestRequestTypeDef](./type_defs.md#terminatetargetinstancesrequestrequesttypedef)
- [UnarchiveApplicationRequestRequestTypeDef](./type_defs.md#unarchiveapplicationrequestrequesttypedef)
- [UnarchiveWaveRequestRequestTypeDef](./type_defs.md#unarchivewaverequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateApplicationRequestRequestTypeDef](./type_defs.md#updateapplicationrequestrequesttypedef)
- [UpdateReplicationConfigurationTemplateRequestRequestTypeDef](./type_defs.md#updatereplicationconfigurationtemplaterequestrequesttypedef)
- [UpdateSourceServerReplicationTypeRequestRequestTypeDef](./type_defs.md#updatesourceserverreplicationtyperequestrequesttypedef)
- [UpdateWaveRequestRequestTypeDef](./type_defs.md#updatewaverequestrequesttypedef)
- [WaveAggregatedStatusTypeDef](./type_defs.md#waveaggregatedstatustypedef)
- [ApplicationTypeDef](./type_defs.md#applicationtypedef)
- [ApplicationResponseTypeDef](./type_defs.md#applicationresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ReplicationConfigurationTemplateResponseTypeDef](./type_defs.md#replicationconfigurationtemplateresponsetypedef)
- [ChangeServerLifeCycleStateRequestRequestTypeDef](./type_defs.md#changeserverlifecyclestaterequestrequesttypedef)
- [ConnectorResponseTypeDef](./type_defs.md#connectorresponsetypedef)
- [ConnectorTypeDef](./type_defs.md#connectortypedef)
- [CreateConnectorRequestRequestTypeDef](./type_defs.md#createconnectorrequestrequesttypedef)
- [UpdateConnectorRequestRequestTypeDef](./type_defs.md#updateconnectorrequestrequesttypedef)
- [DataReplicationInitiationTypeDef](./type_defs.md#datareplicationinitiationtypedef)
- [DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef](./type_defs.md#describejoblogitemsrequestdescribejoblogitemspaginatetypedef)
- [DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef](./type_defs.md#describelaunchconfigurationtemplatesrequestdescribelaunchconfigurationtemplatespaginatetypedef)
- [DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef](./type_defs.md#describereplicationconfigurationtemplatesrequestdescribereplicationconfigurationtemplatespaginatetypedef)
- [DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef](./type_defs.md#describevcenterclientsrequestdescribevcenterclientspaginatetypedef)
- [ListExportErrorsRequestListExportErrorsPaginateTypeDef](./type_defs.md#listexporterrorsrequestlistexporterrorspaginatetypedef)
- [ListImportErrorsRequestListImportErrorsPaginateTypeDef](./type_defs.md#listimporterrorsrequestlistimporterrorspaginatetypedef)
- [ListManagedAccountsRequestListManagedAccountsPaginateTypeDef](./type_defs.md#listmanagedaccountsrequestlistmanagedaccountspaginatetypedef)
- [DescribeJobsRequestDescribeJobsPaginateTypeDef](./type_defs.md#describejobsrequestdescribejobspaginatetypedef)
- [DescribeJobsRequestRequestTypeDef](./type_defs.md#describejobsrequestrequesttypedef)
- [DescribeReplicationConfigurationTemplatesResponseTypeDef](./type_defs.md#describereplicationconfigurationtemplatesresponsetypedef)
- [DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef](./type_defs.md#describesourceserversrequestdescribesourceserverspaginatetypedef)
- [DescribeSourceServersRequestRequestTypeDef](./type_defs.md#describesourceserversrequestrequesttypedef)
- [DescribeVcenterClientsResponseTypeDef](./type_defs.md#describevcenterclientsresponsetypedef)
- [ExportTaskErrorTypeDef](./type_defs.md#exporttaskerrortypedef)
- [ExportTaskTypeDef](./type_defs.md#exporttasktypedef)
- [ImportTaskErrorTypeDef](./type_defs.md#importtaskerrortypedef)
- [ImportTaskSummaryTypeDef](./type_defs.md#importtasksummarytypedef)
- [StartImportRequestRequestTypeDef](./type_defs.md#startimportrequestrequesttypedef)
- [JobLogTypeDef](./type_defs.md#joblogtypedef)
- [LifeCycleLastCutoverTypeDef](./type_defs.md#lifecyclelastcutovertypedef)
- [LifeCycleLastTestTypeDef](./type_defs.md#lifecyclelasttesttypedef)
- [ListApplicationsRequestListApplicationsPaginateTypeDef](./type_defs.md#listapplicationsrequestlistapplicationspaginatetypedef)
- [ListApplicationsRequestRequestTypeDef](./type_defs.md#listapplicationsrequestrequesttypedef)
- [ListConnectorsRequestListConnectorsPaginateTypeDef](./type_defs.md#listconnectorsrequestlistconnectorspaginatetypedef)
- [ListConnectorsRequestRequestTypeDef](./type_defs.md#listconnectorsrequestrequesttypedef)
- [ListExportsRequestListExportsPaginateTypeDef](./type_defs.md#listexportsrequestlistexportspaginatetypedef)
- [ListExportsRequestRequestTypeDef](./type_defs.md#listexportsrequestrequesttypedef)
- [ListImportsRequestListImportsPaginateTypeDef](./type_defs.md#listimportsrequestlistimportspaginatetypedef)
- [ListImportsRequestRequestTypeDef](./type_defs.md#listimportsrequestrequesttypedef)
- [ListManagedAccountsResponseTypeDef](./type_defs.md#listmanagedaccountsresponsetypedef)
- [ListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef](./type_defs.md#listsourceserveractionsrequestlistsourceserveractionspaginatetypedef)
- [ListSourceServerActionsRequestRequestTypeDef](./type_defs.md#listsourceserveractionsrequestrequesttypedef)
- [ListTemplateActionsRequestListTemplateActionsPaginateTypeDef](./type_defs.md#listtemplateactionsrequestlisttemplateactionspaginatetypedef)
- [ListTemplateActionsRequestRequestTypeDef](./type_defs.md#listtemplateactionsrequestrequesttypedef)
- [ListWavesRequestListWavesPaginateTypeDef](./type_defs.md#listwavesrequestlistwavespaginatetypedef)
- [ListWavesRequestRequestTypeDef](./type_defs.md#listwavesrequestrequesttypedef)
- [SourcePropertiesTypeDef](./type_defs.md#sourcepropertiestypedef)
- [PutSourceServerActionRequestRequestTypeDef](./type_defs.md#putsourceserveractionrequestrequesttypedef)
- [PutTemplateActionRequestRequestTypeDef](./type_defs.md#puttemplateactionrequestrequesttypedef)
- [SourceServerActionDocumentResponseTypeDef](./type_defs.md#sourceserveractiondocumentresponsetypedef)
- [SourceServerActionDocumentTypeDef](./type_defs.md#sourceserveractiondocumenttypedef)
- [SsmDocumentOutputTypeDef](./type_defs.md#ssmdocumentoutputtypedef)
- [SsmDocumentTypeDef](./type_defs.md#ssmdocumenttypedef)
- [TemplateActionDocumentResponseTypeDef](./type_defs.md#templateactiondocumentresponsetypedef)
- [TemplateActionDocumentTypeDef](./type_defs.md#templateactiondocumenttypedef)
- [ReplicationConfigurationTypeDef](./type_defs.md#replicationconfigurationtypedef)
- [UpdateReplicationConfigurationRequestRequestTypeDef](./type_defs.md#updatereplicationconfigurationrequestrequesttypedef)
- [UpdateSourceServerRequestRequestTypeDef](./type_defs.md#updatesourceserverrequestrequesttypedef)
- [WaveResponseTypeDef](./type_defs.md#waveresponsetypedef)
- [WaveTypeDef](./type_defs.md#wavetypedef)
- [ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef)
- [ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef)
- [DataReplicationInfoTypeDef](./type_defs.md#datareplicationinfotypedef)
- [ListExportErrorsResponseTypeDef](./type_defs.md#listexporterrorsresponsetypedef)
- [ListExportsResponseTypeDef](./type_defs.md#listexportsresponsetypedef)
- [StartExportResponseTypeDef](./type_defs.md#startexportresponsetypedef)
- [ListImportErrorsResponseTypeDef](./type_defs.md#listimporterrorsresponsetypedef)
- [ImportTaskTypeDef](./type_defs.md#importtasktypedef)
- [DescribeJobLogItemsResponseTypeDef](./type_defs.md#describejoblogitemsresponsetypedef)
- [LifeCycleTypeDef](./type_defs.md#lifecycletypedef)
- [ListSourceServerActionsResponseTypeDef](./type_defs.md#listsourceserveractionsresponsetypedef)
- [JobPostLaunchActionsLaunchStatusTypeDef](./type_defs.md#jobpostlaunchactionslaunchstatustypedef)
- [PostLaunchActionsOutputTypeDef](./type_defs.md#postlaunchactionsoutputtypedef)
- [SsmDocumentUnionTypeDef](./type_defs.md#ssmdocumentuniontypedef)
- [ListTemplateActionsResponseTypeDef](./type_defs.md#listtemplateactionsresponsetypedef)
- [ListWavesResponseTypeDef](./type_defs.md#listwavesresponsetypedef)
- [ListImportsResponseTypeDef](./type_defs.md#listimportsresponsetypedef)
- [StartImportResponseTypeDef](./type_defs.md#startimportresponsetypedef)
- [SourceServerResponseTypeDef](./type_defs.md#sourceserverresponsetypedef)
- [SourceServerTypeDef](./type_defs.md#sourceservertypedef)
- [PostLaunchActionsStatusTypeDef](./type_defs.md#postlaunchactionsstatustypedef)
- [LaunchConfigurationTemplateResponseTypeDef](./type_defs.md#launchconfigurationtemplateresponsetypedef)
- [LaunchConfigurationTemplateTypeDef](./type_defs.md#launchconfigurationtemplatetypedef)
- [LaunchConfigurationTypeDef](./type_defs.md#launchconfigurationtypedef)
- [PostLaunchActionsTypeDef](./type_defs.md#postlaunchactionstypedef)
- [DescribeSourceServersResponseTypeDef](./type_defs.md#describesourceserversresponsetypedef)
- [ParticipatingServerTypeDef](./type_defs.md#participatingservertypedef)
- [DescribeLaunchConfigurationTemplatesResponseTypeDef](./type_defs.md#describelaunchconfigurationtemplatesresponsetypedef)
- [CreateLaunchConfigurationTemplateRequestRequestTypeDef](./type_defs.md#createlaunchconfigurationtemplaterequestrequesttypedef)
- [UpdateLaunchConfigurationRequestRequestTypeDef](./type_defs.md#updatelaunchconfigurationrequestrequesttypedef)
- [UpdateLaunchConfigurationTemplateRequestRequestTypeDef](./type_defs.md#updatelaunchconfigurationtemplaterequestrequesttypedef)
- [JobTypeDef](./type_defs.md#jobtypedef)
- [DescribeJobsResponseTypeDef](./type_defs.md#describejobsresponsetypedef)
- [StartCutoverResponseTypeDef](./type_defs.md#startcutoverresponsetypedef)
- [StartTestResponseTypeDef](./type_defs.md#starttestresponsetypedef)
- [TerminateTargetInstancesResponseTypeDef](./type_defs.md#terminatetargetinstancesresponsetypedef)

