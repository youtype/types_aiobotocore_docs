# DataSync module

> [Index](../README.md) > DataSync


!!! note ""

    Auto-generated documentation for [DataSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#datasync)
    type annotations stubs module [types-aiobotocore-datasync](https://pypi.org/project/types-aiobotocore-datasync/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
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
- [CancelTaskExecutionRequestRequestTypeDef](./type_defs.md#canceltaskexecutionrequestrequesttypedef)
- [CapacityTypeDef](./type_defs.md#capacitytypedef)
- [Ec2ConfigTypeDef](./type_defs.md#ec2configtypedef)
- [HdfsNameNodeTypeDef](./type_defs.md#hdfsnamenodetypedef)
- [QopConfigurationTypeDef](./type_defs.md#qopconfigurationtypedef)
- [NfsMountOptionsTypeDef](./type_defs.md#nfsmountoptionstypedef)
- [OnPremConfigTypeDef](./type_defs.md#onpremconfigtypedef)
- [S3ConfigTypeDef](./type_defs.md#s3configtypedef)
- [SmbMountOptionsTypeDef](./type_defs.md#smbmountoptionstypedef)
- [FilterRuleTypeDef](./type_defs.md#filterruletypedef)
- [OptionsTypeDef](./type_defs.md#optionstypedef)
- [TaskScheduleTypeDef](./type_defs.md#taskscheduletypedef)
- [DeleteAgentRequestRequestTypeDef](./type_defs.md#deleteagentrequestrequesttypedef)
- [DeleteLocationRequestRequestTypeDef](./type_defs.md#deletelocationrequestrequesttypedef)
- [DeleteTaskRequestRequestTypeDef](./type_defs.md#deletetaskrequestrequesttypedef)
- [DescribeAgentRequestRequestTypeDef](./type_defs.md#describeagentrequestrequesttypedef)
- [PrivateLinkConfigTypeDef](./type_defs.md#privatelinkconfigtypedef)
- [DescribeDiscoveryJobRequestRequestTypeDef](./type_defs.md#describediscoveryjobrequestrequesttypedef)
- [DescribeLocationAzureBlobRequestRequestTypeDef](./type_defs.md#describelocationazureblobrequestrequesttypedef)
- [DescribeLocationEfsRequestRequestTypeDef](./type_defs.md#describelocationefsrequestrequesttypedef)
- [Ec2ConfigOutputTypeDef](./type_defs.md#ec2configoutputtypedef)
- [DescribeLocationFsxLustreRequestRequestTypeDef](./type_defs.md#describelocationfsxlustrerequestrequesttypedef)
- [DescribeLocationFsxOntapRequestRequestTypeDef](./type_defs.md#describelocationfsxontaprequestrequesttypedef)
- [DescribeLocationFsxOpenZfsRequestRequestTypeDef](./type_defs.md#describelocationfsxopenzfsrequestrequesttypedef)
- [DescribeLocationFsxWindowsRequestRequestTypeDef](./type_defs.md#describelocationfsxwindowsrequestrequesttypedef)
- [DescribeLocationHdfsRequestRequestTypeDef](./type_defs.md#describelocationhdfsrequestrequesttypedef)
- [DescribeLocationNfsRequestRequestTypeDef](./type_defs.md#describelocationnfsrequestrequesttypedef)
- [OnPremConfigOutputTypeDef](./type_defs.md#onpremconfigoutputtypedef)
- [DescribeLocationObjectStorageRequestRequestTypeDef](./type_defs.md#describelocationobjectstoragerequestrequesttypedef)
- [DescribeLocationS3RequestRequestTypeDef](./type_defs.md#describelocations3requestrequesttypedef)
- [DescribeLocationSmbRequestRequestTypeDef](./type_defs.md#describelocationsmbrequestrequesttypedef)
- [DescribeStorageSystemRequestRequestTypeDef](./type_defs.md#describestoragesystemrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [DescribeStorageSystemResourcesRequestRequestTypeDef](./type_defs.md#describestoragesystemresourcesrequestrequesttypedef)
- [DescribeTaskExecutionRequestRequestTypeDef](./type_defs.md#describetaskexecutionrequestrequesttypedef)
- [ReportResultTypeDef](./type_defs.md#reportresulttypedef)
- [TaskExecutionFilesFailedDetailTypeDef](./type_defs.md#taskexecutionfilesfaileddetailtypedef)
- [TaskExecutionFilesListedDetailTypeDef](./type_defs.md#taskexecutionfileslisteddetailtypedef)
- [TaskExecutionResultDetailTypeDef](./type_defs.md#taskexecutionresultdetailtypedef)
- [DescribeTaskRequestRequestTypeDef](./type_defs.md#describetaskrequestrequesttypedef)
- [TaskScheduleDetailsTypeDef](./type_defs.md#taskscheduledetailstypedef)
- [DiscoveryJobListEntryTypeDef](./type_defs.md#discoveryjoblistentrytypedef)
- [GenerateRecommendationsRequestRequestTypeDef](./type_defs.md#generaterecommendationsrequestrequesttypedef)
- [IOPSTypeDef](./type_defs.md#iopstypedef)
- [LatencyTypeDef](./type_defs.md#latencytypedef)
- [ListAgentsRequestRequestTypeDef](./type_defs.md#listagentsrequestrequesttypedef)
- [ListDiscoveryJobsRequestRequestTypeDef](./type_defs.md#listdiscoveryjobsrequestrequesttypedef)
- [LocationFilterTypeDef](./type_defs.md#locationfiltertypedef)
- [LocationListEntryTypeDef](./type_defs.md#locationlistentrytypedef)
- [ListStorageSystemsRequestRequestTypeDef](./type_defs.md#liststoragesystemsrequestrequesttypedef)
- [StorageSystemListEntryTypeDef](./type_defs.md#storagesystemlistentrytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTaskExecutionsRequestRequestTypeDef](./type_defs.md#listtaskexecutionsrequestrequesttypedef)
- [TaskExecutionListEntryTypeDef](./type_defs.md#taskexecutionlistentrytypedef)
- [TaskFilterTypeDef](./type_defs.md#taskfiltertypedef)
- [TaskListEntryTypeDef](./type_defs.md#tasklistentrytypedef)
- [MaxP95PerformanceTypeDef](./type_defs.md#maxp95performancetypedef)
- [RecommendationTypeDef](./type_defs.md#recommendationtypedef)
- [ThroughputTypeDef](./type_defs.md#throughputtypedef)
- [RemoveStorageSystemRequestRequestTypeDef](./type_defs.md#removestoragesystemrequestrequesttypedef)
- [ReportDestinationS3TypeDef](./type_defs.md#reportdestinations3typedef)
- [ReportOverrideTypeDef](./type_defs.md#reportoverridetypedef)
- [S3ManifestConfigTypeDef](./type_defs.md#s3manifestconfigtypedef)
- [StopDiscoveryJobRequestRequestTypeDef](./type_defs.md#stopdiscoveryjobrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateAgentRequestRequestTypeDef](./type_defs.md#updateagentrequestrequesttypedef)
- [UpdateDiscoveryJobRequestRequestTypeDef](./type_defs.md#updatediscoveryjobrequestrequesttypedef)
- [UpdateLocationEfsRequestRequestTypeDef](./type_defs.md#updatelocationefsrequestrequesttypedef)
- [UpdateLocationFsxLustreRequestRequestTypeDef](./type_defs.md#updatelocationfsxlustrerequestrequesttypedef)
- [UpdateLocationFsxWindowsRequestRequestTypeDef](./type_defs.md#updatelocationfsxwindowsrequestrequesttypedef)
- [UpdateStorageSystemRequestRequestTypeDef](./type_defs.md#updatestoragesystemrequestrequesttypedef)
- [AddStorageSystemRequestRequestTypeDef](./type_defs.md#addstoragesystemrequestrequesttypedef)
- [CreateAgentRequestRequestTypeDef](./type_defs.md#createagentrequestrequesttypedef)
- [CreateLocationFsxLustreRequestRequestTypeDef](./type_defs.md#createlocationfsxlustrerequestrequesttypedef)
- [CreateLocationFsxWindowsRequestRequestTypeDef](./type_defs.md#createlocationfsxwindowsrequestrequesttypedef)
- [StartDiscoveryJobRequestRequestTypeDef](./type_defs.md#startdiscoveryjobrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
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
- [CreateLocationAzureBlobRequestRequestTypeDef](./type_defs.md#createlocationazureblobrequestrequesttypedef)
- [UpdateLocationAzureBlobRequestRequestTypeDef](./type_defs.md#updatelocationazureblobrequestrequesttypedef)
- [CreateLocationObjectStorageRequestRequestTypeDef](./type_defs.md#createlocationobjectstoragerequestrequesttypedef)
- [UpdateLocationObjectStorageRequestRequestTypeDef](./type_defs.md#updatelocationobjectstoragerequestrequesttypedef)
- [CreateLocationEfsRequestRequestTypeDef](./type_defs.md#createlocationefsrequestrequesttypedef)
- [CreateLocationHdfsRequestRequestTypeDef](./type_defs.md#createlocationhdfsrequestrequesttypedef)
- [DescribeLocationHdfsResponseTypeDef](./type_defs.md#describelocationhdfsresponsetypedef)
- [UpdateLocationHdfsRequestRequestTypeDef](./type_defs.md#updatelocationhdfsrequestrequesttypedef)
- [FsxProtocolNfsTypeDef](./type_defs.md#fsxprotocolnfstypedef)
- [CreateLocationNfsRequestRequestTypeDef](./type_defs.md#createlocationnfsrequestrequesttypedef)
- [UpdateLocationNfsRequestRequestTypeDef](./type_defs.md#updatelocationnfsrequestrequesttypedef)
- [CreateLocationS3RequestRequestTypeDef](./type_defs.md#createlocations3requestrequesttypedef)
- [DescribeLocationS3ResponseTypeDef](./type_defs.md#describelocations3responsetypedef)
- [UpdateLocationS3RequestRequestTypeDef](./type_defs.md#updatelocations3requestrequesttypedef)
- [CreateLocationSmbRequestRequestTypeDef](./type_defs.md#createlocationsmbrequestrequesttypedef)
- [DescribeLocationSmbResponseTypeDef](./type_defs.md#describelocationsmbresponsetypedef)
- [FsxProtocolSmbTypeDef](./type_defs.md#fsxprotocolsmbtypedef)
- [FsxUpdateProtocolSmbTypeDef](./type_defs.md#fsxupdateprotocolsmbtypedef)
- [UpdateLocationSmbRequestRequestTypeDef](./type_defs.md#updatelocationsmbrequestrequesttypedef)
- [UpdateTaskExecutionRequestRequestTypeDef](./type_defs.md#updatetaskexecutionrequestrequesttypedef)
- [DescribeAgentResponseTypeDef](./type_defs.md#describeagentresponsetypedef)
- [DescribeLocationEfsResponseTypeDef](./type_defs.md#describelocationefsresponsetypedef)
- [DescribeLocationNfsResponseTypeDef](./type_defs.md#describelocationnfsresponsetypedef)
- [ListAgentsRequestPaginateTypeDef](./type_defs.md#listagentsrequestpaginatetypedef)
- [ListDiscoveryJobsRequestPaginateTypeDef](./type_defs.md#listdiscoveryjobsrequestpaginatetypedef)
- [ListStorageSystemsRequestPaginateTypeDef](./type_defs.md#liststoragesystemsrequestpaginatetypedef)
- [ListTagsForResourceRequestPaginateTypeDef](./type_defs.md#listtagsforresourcerequestpaginatetypedef)
- [ListTaskExecutionsRequestPaginateTypeDef](./type_defs.md#listtaskexecutionsrequestpaginatetypedef)
- [DescribeStorageSystemResourceMetricsRequestPaginateTypeDef](./type_defs.md#describestoragesystemresourcemetricsrequestpaginatetypedef)
- [DescribeStorageSystemResourceMetricsRequestRequestTypeDef](./type_defs.md#describestoragesystemresourcemetricsrequestrequesttypedef)
- [ListDiscoveryJobsResponseTypeDef](./type_defs.md#listdiscoveryjobsresponsetypedef)
- [ListLocationsRequestPaginateTypeDef](./type_defs.md#listlocationsrequestpaginatetypedef)
- [ListLocationsRequestRequestTypeDef](./type_defs.md#listlocationsrequestrequesttypedef)
- [ListLocationsResponseTypeDef](./type_defs.md#listlocationsresponsetypedef)
- [ListStorageSystemsResponseTypeDef](./type_defs.md#liststoragesystemsresponsetypedef)
- [ListTaskExecutionsResponseTypeDef](./type_defs.md#listtaskexecutionsresponsetypedef)
- [ListTasksRequestPaginateTypeDef](./type_defs.md#listtasksrequestpaginatetypedef)
- [ListTasksRequestRequestTypeDef](./type_defs.md#listtasksrequestrequesttypedef)
- [ListTasksResponseTypeDef](./type_defs.md#listtasksresponsetypedef)
- [NetAppONTAPClusterTypeDef](./type_defs.md#netappontapclustertypedef)
- [NetAppONTAPSVMTypeDef](./type_defs.md#netappontapsvmtypedef)
- [NetAppONTAPVolumeTypeDef](./type_defs.md#netappontapvolumetypedef)
- [P95MetricsTypeDef](./type_defs.md#p95metricstypedef)
- [ReportDestinationTypeDef](./type_defs.md#reportdestinationtypedef)
- [ReportOverridesTypeDef](./type_defs.md#reportoverridestypedef)
- [SourceManifestConfigTypeDef](./type_defs.md#sourcemanifestconfigtypedef)
- [ListAgentsResponseTypeDef](./type_defs.md#listagentsresponsetypedef)
- [FsxProtocolTypeDef](./type_defs.md#fsxprotocoltypedef)
- [FsxUpdateProtocolTypeDef](./type_defs.md#fsxupdateprotocoltypedef)
- [ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef)
- [ResourceMetricsTypeDef](./type_defs.md#resourcemetricstypedef)
- [TaskReportConfigTypeDef](./type_defs.md#taskreportconfigtypedef)
- [ManifestConfigTypeDef](./type_defs.md#manifestconfigtypedef)
- [CreateLocationFsxOntapRequestRequestTypeDef](./type_defs.md#createlocationfsxontaprequestrequesttypedef)
- [CreateLocationFsxOpenZfsRequestRequestTypeDef](./type_defs.md#createlocationfsxopenzfsrequestrequesttypedef)
- [DescribeLocationFsxOntapResponseTypeDef](./type_defs.md#describelocationfsxontapresponsetypedef)
- [DescribeLocationFsxOpenZfsResponseTypeDef](./type_defs.md#describelocationfsxopenzfsresponsetypedef)
- [UpdateLocationFsxOpenZfsRequestRequestTypeDef](./type_defs.md#updatelocationfsxopenzfsrequestrequesttypedef)
- [UpdateLocationFsxOntapRequestRequestTypeDef](./type_defs.md#updatelocationfsxontaprequestrequesttypedef)
- [DescribeStorageSystemResourcesResponseTypeDef](./type_defs.md#describestoragesystemresourcesresponsetypedef)
- [DescribeStorageSystemResourceMetricsResponseTypeDef](./type_defs.md#describestoragesystemresourcemetricsresponsetypedef)
- [CreateTaskRequestRequestTypeDef](./type_defs.md#createtaskrequestrequesttypedef)
- [DescribeTaskExecutionResponseTypeDef](./type_defs.md#describetaskexecutionresponsetypedef)
- [DescribeTaskResponseTypeDef](./type_defs.md#describetaskresponsetypedef)
- [StartTaskExecutionRequestRequestTypeDef](./type_defs.md#starttaskexecutionrequestrequesttypedef)
- [UpdateTaskRequestRequestTypeDef](./type_defs.md#updatetaskrequestrequesttypedef)

