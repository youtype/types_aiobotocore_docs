# Mgn module

> [Index](../README.md) > Mgn


!!! note ""

    Auto-generated documentation for [Mgn](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
    type annotations stubs module [types-aiobotocore-mgn](https://pypi.org/project/types-aiobotocore-mgn/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
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
- [InternetProtocolType](./literals.md#internetprotocoltype)
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
- [ArchiveApplicationRequestTypeDef](./type_defs.md#archiveapplicationrequesttypedef)
- [ArchiveWaveRequestTypeDef](./type_defs.md#archivewaverequesttypedef)
- [AssociateApplicationsRequestTypeDef](./type_defs.md#associateapplicationsrequesttypedef)
- [AssociateSourceServersRequestTypeDef](./type_defs.md#associatesourceserversrequesttypedef)
- [CPUTypeDef](./type_defs.md#cputypedef)
- [ChangeServerLifeCycleStateSourceServerLifecycleTypeDef](./type_defs.md#changeserverlifecyclestatesourceserverlifecycletypedef)
- [ConnectorSsmCommandConfigTypeDef](./type_defs.md#connectorssmcommandconfigtypedef)
- [CreateApplicationRequestTypeDef](./type_defs.md#createapplicationrequesttypedef)
- [LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef)
- [LicensingTypeDef](./type_defs.md#licensingtypedef)
- [CreateReplicationConfigurationTemplateRequestTypeDef](./type_defs.md#createreplicationconfigurationtemplaterequesttypedef)
- [CreateWaveRequestTypeDef](./type_defs.md#createwaverequesttypedef)
- [DataReplicationErrorTypeDef](./type_defs.md#datareplicationerrortypedef)
- [DataReplicationInfoReplicatedDiskTypeDef](./type_defs.md#datareplicationinforeplicateddisktypedef)
- [DataReplicationInitiationStepTypeDef](./type_defs.md#datareplicationinitiationsteptypedef)
- [DeleteApplicationRequestTypeDef](./type_defs.md#deleteapplicationrequesttypedef)
- [DeleteConnectorRequestTypeDef](./type_defs.md#deleteconnectorrequesttypedef)
- [DeleteJobRequestTypeDef](./type_defs.md#deletejobrequesttypedef)
- [DeleteLaunchConfigurationTemplateRequestTypeDef](./type_defs.md#deletelaunchconfigurationtemplaterequesttypedef)
- [DeleteReplicationConfigurationTemplateRequestTypeDef](./type_defs.md#deletereplicationconfigurationtemplaterequesttypedef)
- [DeleteSourceServerRequestTypeDef](./type_defs.md#deletesourceserverrequesttypedef)
- [DeleteVcenterClientRequestTypeDef](./type_defs.md#deletevcenterclientrequesttypedef)
- [DeleteWaveRequestTypeDef](./type_defs.md#deletewaverequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeJobLogItemsRequestTypeDef](./type_defs.md#describejoblogitemsrequesttypedef)
- [DescribeJobsRequestFiltersTypeDef](./type_defs.md#describejobsrequestfilterstypedef)
- [DescribeLaunchConfigurationTemplatesRequestTypeDef](./type_defs.md#describelaunchconfigurationtemplatesrequesttypedef)
- [DescribeReplicationConfigurationTemplatesRequestTypeDef](./type_defs.md#describereplicationconfigurationtemplatesrequesttypedef)
- [ReplicationConfigurationTemplateTypeDef](./type_defs.md#replicationconfigurationtemplatetypedef)
- [DescribeSourceServersRequestFiltersTypeDef](./type_defs.md#describesourceserversrequestfilterstypedef)
- [DescribeVcenterClientsRequestTypeDef](./type_defs.md#describevcenterclientsrequesttypedef)
- [VcenterClientTypeDef](./type_defs.md#vcenterclienttypedef)
- [DisassociateApplicationsRequestTypeDef](./type_defs.md#disassociateapplicationsrequesttypedef)
- [DisassociateSourceServersRequestTypeDef](./type_defs.md#disassociatesourceserversrequesttypedef)
- [DisconnectFromServiceRequestTypeDef](./type_defs.md#disconnectfromservicerequesttypedef)
- [DiskTypeDef](./type_defs.md#disktypedef)
- [ExportErrorDataTypeDef](./type_defs.md#exporterrordatatypedef)
- [ExportTaskSummaryTypeDef](./type_defs.md#exporttasksummarytypedef)
- [FinalizeCutoverRequestTypeDef](./type_defs.md#finalizecutoverrequesttypedef)
- [GetLaunchConfigurationRequestTypeDef](./type_defs.md#getlaunchconfigurationrequesttypedef)
- [GetReplicationConfigurationRequestTypeDef](./type_defs.md#getreplicationconfigurationrequesttypedef)
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
- [ListExportErrorsRequestTypeDef](./type_defs.md#listexporterrorsrequesttypedef)
- [ListExportsRequestFiltersTypeDef](./type_defs.md#listexportsrequestfilterstypedef)
- [ListImportErrorsRequestTypeDef](./type_defs.md#listimporterrorsrequesttypedef)
- [ListImportsRequestFiltersTypeDef](./type_defs.md#listimportsrequestfilterstypedef)
- [ListManagedAccountsRequestTypeDef](./type_defs.md#listmanagedaccountsrequesttypedef)
- [ManagedAccountTypeDef](./type_defs.md#managedaccounttypedef)
- [SourceServerActionsRequestFiltersTypeDef](./type_defs.md#sourceserveractionsrequestfilterstypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [TemplateActionsRequestFiltersTypeDef](./type_defs.md#templateactionsrequestfilterstypedef)
- [ListWavesRequestFiltersTypeDef](./type_defs.md#listwavesrequestfilterstypedef)
- [MarkAsArchivedRequestTypeDef](./type_defs.md#markasarchivedrequesttypedef)
- [NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef)
- [OSTypeDef](./type_defs.md#ostypedef)
- [PauseReplicationRequestTypeDef](./type_defs.md#pausereplicationrequesttypedef)
- [SsmExternalParameterTypeDef](./type_defs.md#ssmexternalparametertypedef)
- [SsmParameterStoreParameterTypeDef](./type_defs.md#ssmparameterstoreparametertypedef)
- [RemoveSourceServerActionRequestTypeDef](./type_defs.md#removesourceserveractionrequesttypedef)
- [RemoveTemplateActionRequestTypeDef](./type_defs.md#removetemplateactionrequesttypedef)
- [ReplicationConfigurationReplicatedDiskTypeDef](./type_defs.md#replicationconfigurationreplicateddisktypedef)
- [ResumeReplicationRequestTypeDef](./type_defs.md#resumereplicationrequesttypedef)
- [RetryDataReplicationRequestTypeDef](./type_defs.md#retrydatareplicationrequesttypedef)
- [SourceServerConnectorActionTypeDef](./type_defs.md#sourceserverconnectoractiontypedef)
- [StartCutoverRequestTypeDef](./type_defs.md#startcutoverrequesttypedef)
- [StartExportRequestTypeDef](./type_defs.md#startexportrequesttypedef)
- [StartReplicationRequestTypeDef](./type_defs.md#startreplicationrequesttypedef)
- [StartTestRequestTypeDef](./type_defs.md#starttestrequesttypedef)
- [StopReplicationRequestTypeDef](./type_defs.md#stopreplicationrequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [TerminateTargetInstancesRequestTypeDef](./type_defs.md#terminatetargetinstancesrequesttypedef)
- [UnarchiveApplicationRequestTypeDef](./type_defs.md#unarchiveapplicationrequesttypedef)
- [UnarchiveWaveRequestTypeDef](./type_defs.md#unarchivewaverequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateApplicationRequestTypeDef](./type_defs.md#updateapplicationrequesttypedef)
- [UpdateReplicationConfigurationTemplateRequestTypeDef](./type_defs.md#updatereplicationconfigurationtemplaterequesttypedef)
- [UpdateSourceServerReplicationTypeRequestTypeDef](./type_defs.md#updatesourceserverreplicationtyperequesttypedef)
- [UpdateWaveRequestTypeDef](./type_defs.md#updatewaverequesttypedef)
- [WaveAggregatedStatusTypeDef](./type_defs.md#waveaggregatedstatustypedef)
- [ApplicationTypeDef](./type_defs.md#applicationtypedef)
- [ApplicationResponseTypeDef](./type_defs.md#applicationresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ReplicationConfigurationTemplateResponseTypeDef](./type_defs.md#replicationconfigurationtemplateresponsetypedef)
- [ChangeServerLifeCycleStateRequestTypeDef](./type_defs.md#changeserverlifecyclestaterequesttypedef)
- [ConnectorResponseTypeDef](./type_defs.md#connectorresponsetypedef)
- [ConnectorTypeDef](./type_defs.md#connectortypedef)
- [CreateConnectorRequestTypeDef](./type_defs.md#createconnectorrequesttypedef)
- [UpdateConnectorRequestTypeDef](./type_defs.md#updateconnectorrequesttypedef)
- [DataReplicationInitiationTypeDef](./type_defs.md#datareplicationinitiationtypedef)
- [DescribeJobLogItemsRequestPaginateTypeDef](./type_defs.md#describejoblogitemsrequestpaginatetypedef)
- [DescribeLaunchConfigurationTemplatesRequestPaginateTypeDef](./type_defs.md#describelaunchconfigurationtemplatesrequestpaginatetypedef)
- [DescribeReplicationConfigurationTemplatesRequestPaginateTypeDef](./type_defs.md#describereplicationconfigurationtemplatesrequestpaginatetypedef)
- [DescribeVcenterClientsRequestPaginateTypeDef](./type_defs.md#describevcenterclientsrequestpaginatetypedef)
- [ListExportErrorsRequestPaginateTypeDef](./type_defs.md#listexporterrorsrequestpaginatetypedef)
- [ListImportErrorsRequestPaginateTypeDef](./type_defs.md#listimporterrorsrequestpaginatetypedef)
- [ListManagedAccountsRequestPaginateTypeDef](./type_defs.md#listmanagedaccountsrequestpaginatetypedef)
- [DescribeJobsRequestPaginateTypeDef](./type_defs.md#describejobsrequestpaginatetypedef)
- [DescribeJobsRequestTypeDef](./type_defs.md#describejobsrequesttypedef)
- [DescribeReplicationConfigurationTemplatesResponseTypeDef](./type_defs.md#describereplicationconfigurationtemplatesresponsetypedef)
- [DescribeSourceServersRequestPaginateTypeDef](./type_defs.md#describesourceserversrequestpaginatetypedef)
- [DescribeSourceServersRequestTypeDef](./type_defs.md#describesourceserversrequesttypedef)
- [DescribeVcenterClientsResponseTypeDef](./type_defs.md#describevcenterclientsresponsetypedef)
- [ExportTaskErrorTypeDef](./type_defs.md#exporttaskerrortypedef)
- [ExportTaskTypeDef](./type_defs.md#exporttasktypedef)
- [ImportTaskErrorTypeDef](./type_defs.md#importtaskerrortypedef)
- [ImportTaskSummaryTypeDef](./type_defs.md#importtasksummarytypedef)
- [StartImportRequestTypeDef](./type_defs.md#startimportrequesttypedef)
- [JobLogTypeDef](./type_defs.md#joblogtypedef)
- [LifeCycleLastCutoverTypeDef](./type_defs.md#lifecyclelastcutovertypedef)
- [LifeCycleLastTestTypeDef](./type_defs.md#lifecyclelasttesttypedef)
- [ListApplicationsRequestPaginateTypeDef](./type_defs.md#listapplicationsrequestpaginatetypedef)
- [ListApplicationsRequestTypeDef](./type_defs.md#listapplicationsrequesttypedef)
- [ListConnectorsRequestPaginateTypeDef](./type_defs.md#listconnectorsrequestpaginatetypedef)
- [ListConnectorsRequestTypeDef](./type_defs.md#listconnectorsrequesttypedef)
- [ListExportsRequestPaginateTypeDef](./type_defs.md#listexportsrequestpaginatetypedef)
- [ListExportsRequestTypeDef](./type_defs.md#listexportsrequesttypedef)
- [ListImportsRequestPaginateTypeDef](./type_defs.md#listimportsrequestpaginatetypedef)
- [ListImportsRequestTypeDef](./type_defs.md#listimportsrequesttypedef)
- [ListManagedAccountsResponseTypeDef](./type_defs.md#listmanagedaccountsresponsetypedef)
- [ListSourceServerActionsRequestPaginateTypeDef](./type_defs.md#listsourceserveractionsrequestpaginatetypedef)
- [ListSourceServerActionsRequestTypeDef](./type_defs.md#listsourceserveractionsrequesttypedef)
- [ListTemplateActionsRequestPaginateTypeDef](./type_defs.md#listtemplateactionsrequestpaginatetypedef)
- [ListTemplateActionsRequestTypeDef](./type_defs.md#listtemplateactionsrequesttypedef)
- [ListWavesRequestPaginateTypeDef](./type_defs.md#listwavesrequestpaginatetypedef)
- [ListWavesRequestTypeDef](./type_defs.md#listwavesrequesttypedef)
- [SourcePropertiesTypeDef](./type_defs.md#sourcepropertiestypedef)
- [PutSourceServerActionRequestTypeDef](./type_defs.md#putsourceserveractionrequesttypedef)
- [PutTemplateActionRequestTypeDef](./type_defs.md#puttemplateactionrequesttypedef)
- [SourceServerActionDocumentResponseTypeDef](./type_defs.md#sourceserveractiondocumentresponsetypedef)
- [SourceServerActionDocumentTypeDef](./type_defs.md#sourceserveractiondocumenttypedef)
- [SsmDocumentOutputTypeDef](./type_defs.md#ssmdocumentoutputtypedef)
- [SsmDocumentTypeDef](./type_defs.md#ssmdocumenttypedef)
- [TemplateActionDocumentResponseTypeDef](./type_defs.md#templateactiondocumentresponsetypedef)
- [TemplateActionDocumentTypeDef](./type_defs.md#templateactiondocumenttypedef)
- [ReplicationConfigurationTypeDef](./type_defs.md#replicationconfigurationtypedef)
- [UpdateReplicationConfigurationRequestTypeDef](./type_defs.md#updatereplicationconfigurationrequesttypedef)
- [UpdateSourceServerRequestTypeDef](./type_defs.md#updatesourceserverrequesttypedef)
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
- [PostLaunchActionsTypeDef](./type_defs.md#postlaunchactionstypedef)
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
- [PostLaunchActionsUnionTypeDef](./type_defs.md#postlaunchactionsuniontypedef)
- [DescribeSourceServersResponseTypeDef](./type_defs.md#describesourceserversresponsetypedef)
- [ParticipatingServerTypeDef](./type_defs.md#participatingservertypedef)
- [DescribeLaunchConfigurationTemplatesResponseTypeDef](./type_defs.md#describelaunchconfigurationtemplatesresponsetypedef)
- [CreateLaunchConfigurationTemplateRequestTypeDef](./type_defs.md#createlaunchconfigurationtemplaterequesttypedef)
- [UpdateLaunchConfigurationRequestTypeDef](./type_defs.md#updatelaunchconfigurationrequesttypedef)
- [UpdateLaunchConfigurationTemplateRequestTypeDef](./type_defs.md#updatelaunchconfigurationtemplaterequesttypedef)
- [JobTypeDef](./type_defs.md#jobtypedef)
- [DescribeJobsResponseTypeDef](./type_defs.md#describejobsresponsetypedef)
- [StartCutoverResponseTypeDef](./type_defs.md#startcutoverresponsetypedef)
- [StartTestResponseTypeDef](./type_defs.md#starttestresponsetypedef)
- [TerminateTargetInstancesResponseTypeDef](./type_defs.md#terminatetargetinstancesresponsetypedef)

