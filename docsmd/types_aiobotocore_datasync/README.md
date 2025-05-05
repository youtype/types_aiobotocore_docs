# DataSync module

> [Index](../README.md) > DataSync


!!! note ""

    Auto-generated documentation for [DataSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#datasync)
    type annotations stubs module [types-aiobotocore-datasync](https://pypi.org/project/types-aiobotocore-datasync/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.22.0' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `DataSync` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `DataSync` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[datasync]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[datasync]'

# standalone installation
python -m pip install types-aiobotocore-datasync
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-datasync
```

## Usage

Code samples can be found in [Examples](./usage.md).

## DataSyncClient

Type annotations and code completion for  `#!python session.create_client("datasync")` as [DataSyncClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client)

```python
# DataSyncClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_datasync.client import DataSyncClient


session = get_session()
async with session.create_client("datasync") as client:
    client: DataSyncClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("datasync").get_paginator("...")`.

```python
# DescribeStorageSystemResourceMetricsPaginator usage example

from types_aiobotocore_datasync.paginator import DescribeStorageSystemResourceMetricsPaginator

def get_describe_storage_system_resource_metrics_paginator() -> DescribeStorageSystemResourceMetricsPaginator:
    return client.get_paginator("describe_storage_system_resource_metrics"))
```

- [DescribeStorageSystemResourceMetricsPaginator](./paginators.md#describestoragesystemresourcemetricspaginator)
- [ListAgentsPaginator](./paginators.md#listagentspaginator)
- [ListDiscoveryJobsPaginator](./paginators.md#listdiscoveryjobspaginator)
- [ListLocationsPaginator](./paginators.md#listlocationspaginator)
- [ListStorageSystemsPaginator](./paginators.md#liststoragesystemspaginator)
- [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
- [ListTaskExecutionsPaginator](./paginators.md#listtaskexecutionspaginator)
- [ListTasksPaginator](./paginators.md#listtaskspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AgentStatusType usage example

from types_aiobotocore_datasync.literals import AgentStatusType

def get_value() -> AgentStatusType:
    return "OFFLINE"
```

- [AgentStatusType](./literals.md#agentstatustype)
- [AtimeType](./literals.md#atimetype)
- [AzureAccessTierType](./literals.md#azureaccesstiertype)
- [AzureBlobAuthenticationTypeType](./literals.md#azureblobauthenticationtypetype)
- [AzureBlobTypeType](./literals.md#azureblobtypetype)
- [DescribeStorageSystemResourceMetricsPaginatorName](./literals.md#describestoragesystemresourcemetricspaginatorname)
- [DiscoveryJobStatusType](./literals.md#discoveryjobstatustype)
- [DiscoveryResourceFilterType](./literals.md#discoveryresourcefiltertype)
- [DiscoveryResourceTypeType](./literals.md#discoveryresourcetypetype)
- [DiscoverySystemTypeType](./literals.md#discoverysystemtypetype)
- [EfsInTransitEncryptionType](./literals.md#efsintransitencryptiontype)
- [EndpointTypeType](./literals.md#endpointtypetype)
- [FilterTypeType](./literals.md#filtertypetype)
- [GidType](./literals.md#gidtype)
- [HdfsAuthenticationTypeType](./literals.md#hdfsauthenticationtypetype)
- [HdfsDataTransferProtectionType](./literals.md#hdfsdatatransferprotectiontype)
- [HdfsRpcProtectionType](./literals.md#hdfsrpcprotectiontype)
- [ListAgentsPaginatorName](./literals.md#listagentspaginatorname)
- [ListDiscoveryJobsPaginatorName](./literals.md#listdiscoveryjobspaginatorname)
- [ListLocationsPaginatorName](./literals.md#listlocationspaginatorname)
- [ListStorageSystemsPaginatorName](./literals.md#liststoragesystemspaginatorname)
- [ListTagsForResourcePaginatorName](./literals.md#listtagsforresourcepaginatorname)
- [ListTaskExecutionsPaginatorName](./literals.md#listtaskexecutionspaginatorname)
- [ListTasksPaginatorName](./literals.md#listtaskspaginatorname)
- [LocationFilterNameType](./literals.md#locationfilternametype)
- [LogLevelType](./literals.md#logleveltype)
- [ManifestActionType](./literals.md#manifestactiontype)
- [ManifestFormatType](./literals.md#manifestformattype)
- [MtimeType](./literals.md#mtimetype)
- [NfsVersionType](./literals.md#nfsversiontype)
- [ObjectStorageServerProtocolType](./literals.md#objectstorageserverprotocoltype)
- [ObjectTagsType](./literals.md#objecttagstype)
- [ObjectVersionIdsType](./literals.md#objectversionidstype)
- [OperatorType](./literals.md#operatortype)
- [OverwriteModeType](./literals.md#overwritemodetype)
- [PhaseStatusType](./literals.md#phasestatustype)
- [PosixPermissionsType](./literals.md#posixpermissionstype)
- [PreserveDeletedFilesType](./literals.md#preservedeletedfilestype)
- [PreserveDevicesType](./literals.md#preservedevicestype)
- [RecommendationStatusType](./literals.md#recommendationstatustype)
- [ReportLevelType](./literals.md#reportleveltype)
- [ReportOutputTypeType](./literals.md#reportoutputtypetype)
- [S3StorageClassType](./literals.md#s3storageclasstype)
- [ScheduleDisabledByType](./literals.md#scheduledisabledbytype)
- [ScheduleStatusType](./literals.md#schedulestatustype)
- [SmbAuthenticationTypeType](./literals.md#smbauthenticationtypetype)
- [SmbSecurityDescriptorCopyFlagsType](./literals.md#smbsecuritydescriptorcopyflagstype)
- [SmbVersionType](./literals.md#smbversiontype)
- [StorageSystemConnectivityStatusType](./literals.md#storagesystemconnectivitystatustype)
- [TaskExecutionStatusType](./literals.md#taskexecutionstatustype)
- [TaskFilterNameType](./literals.md#taskfilternametype)
- [TaskModeType](./literals.md#taskmodetype)
- [TaskQueueingType](./literals.md#taskqueueingtype)
- [TaskStatusType](./literals.md#taskstatustype)
- [TransferModeType](./literals.md#transfermodetype)
- [UidType](./literals.md#uidtype)
- [VerifyModeType](./literals.md#verifymodetype)
- [DataSyncServiceName](./literals.md#datasyncservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CredentialsTypeDef](./type_defs.md#credentialstypedef)
- [DiscoveryServerConfigurationTypeDef](./type_defs.md#discoveryserverconfigurationtypedef)
- [TagListEntryTypeDef](./type_defs.md#taglistentrytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [PlatformTypeDef](./type_defs.md#platformtypedef)
- [AzureBlobSasConfigurationTypeDef](./type_defs.md#azureblobsasconfigurationtypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CancelTaskExecutionRequestTypeDef](./type_defs.md#canceltaskexecutionrequesttypedef)
- [CapacityTypeDef](./type_defs.md#capacitytypedef)
- [HdfsNameNodeTypeDef](./type_defs.md#hdfsnamenodetypedef)
- [QopConfigurationTypeDef](./type_defs.md#qopconfigurationtypedef)
- [NfsMountOptionsTypeDef](./type_defs.md#nfsmountoptionstypedef)
- [S3ConfigTypeDef](./type_defs.md#s3configtypedef)
- [SmbMountOptionsTypeDef](./type_defs.md#smbmountoptionstypedef)
- [FilterRuleTypeDef](./type_defs.md#filterruletypedef)
- [OptionsTypeDef](./type_defs.md#optionstypedef)
- [TaskScheduleTypeDef](./type_defs.md#taskscheduletypedef)
- [DeleteAgentRequestTypeDef](./type_defs.md#deleteagentrequesttypedef)
- [DeleteLocationRequestTypeDef](./type_defs.md#deletelocationrequesttypedef)
- [DeleteTaskRequestTypeDef](./type_defs.md#deletetaskrequesttypedef)
- [DescribeAgentRequestTypeDef](./type_defs.md#describeagentrequesttypedef)
- [PrivateLinkConfigTypeDef](./type_defs.md#privatelinkconfigtypedef)
- [DescribeDiscoveryJobRequestTypeDef](./type_defs.md#describediscoveryjobrequesttypedef)
- [DescribeLocationAzureBlobRequestTypeDef](./type_defs.md#describelocationazureblobrequesttypedef)
- [DescribeLocationEfsRequestTypeDef](./type_defs.md#describelocationefsrequesttypedef)
- [Ec2ConfigOutputTypeDef](./type_defs.md#ec2configoutputtypedef)
- [DescribeLocationFsxLustreRequestTypeDef](./type_defs.md#describelocationfsxlustrerequesttypedef)
- [DescribeLocationFsxOntapRequestTypeDef](./type_defs.md#describelocationfsxontaprequesttypedef)
- [DescribeLocationFsxOpenZfsRequestTypeDef](./type_defs.md#describelocationfsxopenzfsrequesttypedef)
- [DescribeLocationFsxWindowsRequestTypeDef](./type_defs.md#describelocationfsxwindowsrequesttypedef)
- [DescribeLocationHdfsRequestTypeDef](./type_defs.md#describelocationhdfsrequesttypedef)
- [DescribeLocationNfsRequestTypeDef](./type_defs.md#describelocationnfsrequesttypedef)
- [OnPremConfigOutputTypeDef](./type_defs.md#onpremconfigoutputtypedef)
- [DescribeLocationObjectStorageRequestTypeDef](./type_defs.md#describelocationobjectstoragerequesttypedef)
- [DescribeLocationS3RequestTypeDef](./type_defs.md#describelocations3requesttypedef)
- [DescribeLocationSmbRequestTypeDef](./type_defs.md#describelocationsmbrequesttypedef)
- [DescribeStorageSystemRequestTypeDef](./type_defs.md#describestoragesystemrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [DescribeStorageSystemResourcesRequestTypeDef](./type_defs.md#describestoragesystemresourcesrequesttypedef)
- [DescribeTaskExecutionRequestTypeDef](./type_defs.md#describetaskexecutionrequesttypedef)
- [ReportResultTypeDef](./type_defs.md#reportresulttypedef)
- [TaskExecutionFilesFailedDetailTypeDef](./type_defs.md#taskexecutionfilesfaileddetailtypedef)
- [TaskExecutionFilesListedDetailTypeDef](./type_defs.md#taskexecutionfileslisteddetailtypedef)
- [TaskExecutionResultDetailTypeDef](./type_defs.md#taskexecutionresultdetailtypedef)
- [DescribeTaskRequestTypeDef](./type_defs.md#describetaskrequesttypedef)
- [TaskScheduleDetailsTypeDef](./type_defs.md#taskscheduledetailstypedef)
- [DiscoveryJobListEntryTypeDef](./type_defs.md#discoveryjoblistentrytypedef)
- [Ec2ConfigTypeDef](./type_defs.md#ec2configtypedef)
- [GenerateRecommendationsRequestTypeDef](./type_defs.md#generaterecommendationsrequesttypedef)
- [IOPSTypeDef](./type_defs.md#iopstypedef)
- [LatencyTypeDef](./type_defs.md#latencytypedef)
- [ListAgentsRequestTypeDef](./type_defs.md#listagentsrequesttypedef)
- [ListDiscoveryJobsRequestTypeDef](./type_defs.md#listdiscoveryjobsrequesttypedef)
- [LocationFilterTypeDef](./type_defs.md#locationfiltertypedef)
- [LocationListEntryTypeDef](./type_defs.md#locationlistentrytypedef)
- [ListStorageSystemsRequestTypeDef](./type_defs.md#liststoragesystemsrequesttypedef)
- [StorageSystemListEntryTypeDef](./type_defs.md#storagesystemlistentrytypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [ListTaskExecutionsRequestTypeDef](./type_defs.md#listtaskexecutionsrequesttypedef)
- [TaskExecutionListEntryTypeDef](./type_defs.md#taskexecutionlistentrytypedef)
- [TaskFilterTypeDef](./type_defs.md#taskfiltertypedef)
- [TaskListEntryTypeDef](./type_defs.md#tasklistentrytypedef)
- [MaxP95PerformanceTypeDef](./type_defs.md#maxp95performancetypedef)
- [RecommendationTypeDef](./type_defs.md#recommendationtypedef)
- [OnPremConfigTypeDef](./type_defs.md#onpremconfigtypedef)
- [ThroughputTypeDef](./type_defs.md#throughputtypedef)
- [RemoveStorageSystemRequestTypeDef](./type_defs.md#removestoragesystemrequesttypedef)
- [ReportDestinationS3TypeDef](./type_defs.md#reportdestinations3typedef)
- [ReportOverrideTypeDef](./type_defs.md#reportoverridetypedef)
- [S3ManifestConfigTypeDef](./type_defs.md#s3manifestconfigtypedef)
- [StopDiscoveryJobRequestTypeDef](./type_defs.md#stopdiscoveryjobrequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateAgentRequestTypeDef](./type_defs.md#updateagentrequesttypedef)
- [UpdateDiscoveryJobRequestTypeDef](./type_defs.md#updatediscoveryjobrequesttypedef)
- [UpdateLocationEfsRequestTypeDef](./type_defs.md#updatelocationefsrequesttypedef)
- [UpdateLocationFsxLustreRequestTypeDef](./type_defs.md#updatelocationfsxlustrerequesttypedef)
- [UpdateLocationFsxWindowsRequestTypeDef](./type_defs.md#updatelocationfsxwindowsrequesttypedef)
- [UpdateStorageSystemRequestTypeDef](./type_defs.md#updatestoragesystemrequesttypedef)
- [AddStorageSystemRequestTypeDef](./type_defs.md#addstoragesystemrequesttypedef)
- [CreateAgentRequestTypeDef](./type_defs.md#createagentrequesttypedef)
- [CreateLocationFsxLustreRequestTypeDef](./type_defs.md#createlocationfsxlustrerequesttypedef)
- [CreateLocationFsxWindowsRequestTypeDef](./type_defs.md#createlocationfsxwindowsrequesttypedef)
- [StartDiscoveryJobRequestTypeDef](./type_defs.md#startdiscoveryjobrequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [AddStorageSystemResponseTypeDef](./type_defs.md#addstoragesystemresponsetypedef)
- [CreateAgentResponseTypeDef](./type_defs.md#createagentresponsetypedef)
- [CreateLocationAzureBlobResponseTypeDef](./type_defs.md#createlocationazureblobresponsetypedef)
- [CreateLocationEfsResponseTypeDef](./type_defs.md#createlocationefsresponsetypedef)
- [CreateLocationFsxLustreResponseTypeDef](./type_defs.md#createlocationfsxlustreresponsetypedef)
- [CreateLocationFsxOntapResponseTypeDef](./type_defs.md#createlocationfsxontapresponsetypedef)
- [CreateLocationFsxOpenZfsResponseTypeDef](./type_defs.md#createlocationfsxopenzfsresponsetypedef)
- [CreateLocationFsxWindowsResponseTypeDef](./type_defs.md#createlocationfsxwindowsresponsetypedef)
- [CreateLocationHdfsResponseTypeDef](./type_defs.md#createlocationhdfsresponsetypedef)
- [CreateLocationNfsResponseTypeDef](./type_defs.md#createlocationnfsresponsetypedef)
- [CreateLocationObjectStorageResponseTypeDef](./type_defs.md#createlocationobjectstorageresponsetypedef)
- [CreateLocationS3ResponseTypeDef](./type_defs.md#createlocations3responsetypedef)
- [CreateLocationSmbResponseTypeDef](./type_defs.md#createlocationsmbresponsetypedef)
- [CreateTaskResponseTypeDef](./type_defs.md#createtaskresponsetypedef)
- [DescribeDiscoveryJobResponseTypeDef](./type_defs.md#describediscoveryjobresponsetypedef)
- [DescribeLocationAzureBlobResponseTypeDef](./type_defs.md#describelocationazureblobresponsetypedef)
- [DescribeLocationFsxLustreResponseTypeDef](./type_defs.md#describelocationfsxlustreresponsetypedef)
- [DescribeLocationFsxWindowsResponseTypeDef](./type_defs.md#describelocationfsxwindowsresponsetypedef)
- [DescribeLocationObjectStorageResponseTypeDef](./type_defs.md#describelocationobjectstorageresponsetypedef)
- [DescribeStorageSystemResponseTypeDef](./type_defs.md#describestoragesystemresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartDiscoveryJobResponseTypeDef](./type_defs.md#startdiscoveryjobresponsetypedef)
- [StartTaskExecutionResponseTypeDef](./type_defs.md#starttaskexecutionresponsetypedef)
- [AgentListEntryTypeDef](./type_defs.md#agentlistentrytypedef)
- [CreateLocationAzureBlobRequestTypeDef](./type_defs.md#createlocationazureblobrequesttypedef)
- [UpdateLocationAzureBlobRequestTypeDef](./type_defs.md#updatelocationazureblobrequesttypedef)
- [CreateLocationObjectStorageRequestTypeDef](./type_defs.md#createlocationobjectstoragerequesttypedef)
- [UpdateLocationObjectStorageRequestTypeDef](./type_defs.md#updatelocationobjectstoragerequesttypedef)
- [CreateLocationHdfsRequestTypeDef](./type_defs.md#createlocationhdfsrequesttypedef)
- [DescribeLocationHdfsResponseTypeDef](./type_defs.md#describelocationhdfsresponsetypedef)
- [UpdateLocationHdfsRequestTypeDef](./type_defs.md#updatelocationhdfsrequesttypedef)
- [FsxProtocolNfsTypeDef](./type_defs.md#fsxprotocolnfstypedef)
- [CreateLocationS3RequestTypeDef](./type_defs.md#createlocations3requesttypedef)
- [DescribeLocationS3ResponseTypeDef](./type_defs.md#describelocations3responsetypedef)
- [UpdateLocationS3RequestTypeDef](./type_defs.md#updatelocations3requesttypedef)
- [CreateLocationSmbRequestTypeDef](./type_defs.md#createlocationsmbrequesttypedef)
- [DescribeLocationSmbResponseTypeDef](./type_defs.md#describelocationsmbresponsetypedef)
- [FsxProtocolSmbTypeDef](./type_defs.md#fsxprotocolsmbtypedef)
- [FsxUpdateProtocolSmbTypeDef](./type_defs.md#fsxupdateprotocolsmbtypedef)
- [UpdateLocationSmbRequestTypeDef](./type_defs.md#updatelocationsmbrequesttypedef)
- [UpdateTaskExecutionRequestTypeDef](./type_defs.md#updatetaskexecutionrequesttypedef)
- [DescribeAgentResponseTypeDef](./type_defs.md#describeagentresponsetypedef)
- [DescribeLocationEfsResponseTypeDef](./type_defs.md#describelocationefsresponsetypedef)
- [DescribeLocationNfsResponseTypeDef](./type_defs.md#describelocationnfsresponsetypedef)
- [ListAgentsRequestPaginateTypeDef](./type_defs.md#listagentsrequestpaginatetypedef)
- [ListDiscoveryJobsRequestPaginateTypeDef](./type_defs.md#listdiscoveryjobsrequestpaginatetypedef)
- [ListStorageSystemsRequestPaginateTypeDef](./type_defs.md#liststoragesystemsrequestpaginatetypedef)
- [ListTagsForResourceRequestPaginateTypeDef](./type_defs.md#listtagsforresourcerequestpaginatetypedef)
- [ListTaskExecutionsRequestPaginateTypeDef](./type_defs.md#listtaskexecutionsrequestpaginatetypedef)
- [DescribeStorageSystemResourceMetricsRequestPaginateTypeDef](./type_defs.md#describestoragesystemresourcemetricsrequestpaginatetypedef)
- [DescribeStorageSystemResourceMetricsRequestTypeDef](./type_defs.md#describestoragesystemresourcemetricsrequesttypedef)
- [ListDiscoveryJobsResponseTypeDef](./type_defs.md#listdiscoveryjobsresponsetypedef)
- [Ec2ConfigUnionTypeDef](./type_defs.md#ec2configuniontypedef)
- [ListLocationsRequestPaginateTypeDef](./type_defs.md#listlocationsrequestpaginatetypedef)
- [ListLocationsRequestTypeDef](./type_defs.md#listlocationsrequesttypedef)
- [ListLocationsResponseTypeDef](./type_defs.md#listlocationsresponsetypedef)
- [ListStorageSystemsResponseTypeDef](./type_defs.md#liststoragesystemsresponsetypedef)
- [ListTaskExecutionsResponseTypeDef](./type_defs.md#listtaskexecutionsresponsetypedef)
- [ListTasksRequestPaginateTypeDef](./type_defs.md#listtasksrequestpaginatetypedef)
- [ListTasksRequestTypeDef](./type_defs.md#listtasksrequesttypedef)
- [ListTasksResponseTypeDef](./type_defs.md#listtasksresponsetypedef)
- [NetAppONTAPClusterTypeDef](./type_defs.md#netappontapclustertypedef)
- [NetAppONTAPSVMTypeDef](./type_defs.md#netappontapsvmtypedef)
- [NetAppONTAPVolumeTypeDef](./type_defs.md#netappontapvolumetypedef)
- [OnPremConfigUnionTypeDef](./type_defs.md#onpremconfiguniontypedef)
- [P95MetricsTypeDef](./type_defs.md#p95metricstypedef)
- [ReportDestinationTypeDef](./type_defs.md#reportdestinationtypedef)
- [ReportOverridesTypeDef](./type_defs.md#reportoverridestypedef)
- [SourceManifestConfigTypeDef](./type_defs.md#sourcemanifestconfigtypedef)
- [ListAgentsResponseTypeDef](./type_defs.md#listagentsresponsetypedef)
- [FsxProtocolTypeDef](./type_defs.md#fsxprotocoltypedef)
- [FsxUpdateProtocolTypeDef](./type_defs.md#fsxupdateprotocoltypedef)
- [CreateLocationEfsRequestTypeDef](./type_defs.md#createlocationefsrequesttypedef)
- [ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef)
- [CreateLocationNfsRequestTypeDef](./type_defs.md#createlocationnfsrequesttypedef)
- [UpdateLocationNfsRequestTypeDef](./type_defs.md#updatelocationnfsrequesttypedef)
- [ResourceMetricsTypeDef](./type_defs.md#resourcemetricstypedef)
- [TaskReportConfigTypeDef](./type_defs.md#taskreportconfigtypedef)
- [ManifestConfigTypeDef](./type_defs.md#manifestconfigtypedef)
- [CreateLocationFsxOntapRequestTypeDef](./type_defs.md#createlocationfsxontaprequesttypedef)
- [CreateLocationFsxOpenZfsRequestTypeDef](./type_defs.md#createlocationfsxopenzfsrequesttypedef)
- [DescribeLocationFsxOntapResponseTypeDef](./type_defs.md#describelocationfsxontapresponsetypedef)
- [DescribeLocationFsxOpenZfsResponseTypeDef](./type_defs.md#describelocationfsxopenzfsresponsetypedef)
- [UpdateLocationFsxOpenZfsRequestTypeDef](./type_defs.md#updatelocationfsxopenzfsrequesttypedef)
- [UpdateLocationFsxOntapRequestTypeDef](./type_defs.md#updatelocationfsxontaprequesttypedef)
- [DescribeStorageSystemResourcesResponseTypeDef](./type_defs.md#describestoragesystemresourcesresponsetypedef)
- [DescribeStorageSystemResourceMetricsResponseTypeDef](./type_defs.md#describestoragesystemresourcemetricsresponsetypedef)
- [CreateTaskRequestTypeDef](./type_defs.md#createtaskrequesttypedef)
- [DescribeTaskExecutionResponseTypeDef](./type_defs.md#describetaskexecutionresponsetypedef)
- [DescribeTaskResponseTypeDef](./type_defs.md#describetaskresponsetypedef)
- [StartTaskExecutionRequestTypeDef](./type_defs.md#starttaskexecutionrequesttypedef)
- [UpdateTaskRequestTypeDef](./type_defs.md#updatetaskrequesttypedef)

