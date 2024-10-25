# Type definitions

> [Index](../README.md) > [Mgn](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Mgn](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#Mgn)
    type annotations stubs module [types-aiobotocore-mgn](https://pypi.org/project/types-aiobotocore-mgn/).

## SsmDocumentUnionTypeDef

```python
# SsmDocumentUnionTypeDef definition

SsmDocumentUnionTypeDef = Union[
    SsmDocumentTypeDef,  # (1)
    SsmDocumentOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SsmDocumentTypeDef](./type_defs.md#ssmdocumenttypedef) 
2. See [:material-code-braces: SsmDocumentOutputTypeDef](./type_defs.md#ssmdocumentoutputtypedef) 



## ApplicationAggregatedStatusTypeDef

```python
# ApplicationAggregatedStatusTypeDef definition

class ApplicationAggregatedStatusTypeDef(TypedDict):
    healthStatus: NotRequired[ApplicationHealthStatusType],  # (1)
    lastUpdateDateTime: NotRequired[str],
    progressStatus: NotRequired[ApplicationProgressStatusType],  # (2)
    totalSourceServers: NotRequired[int],
```

1. See [:material-code-brackets: ApplicationHealthStatusType](./literals.md#applicationhealthstatustype) 
2. See [:material-code-brackets: ApplicationProgressStatusType](./literals.md#applicationprogressstatustype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## ArchiveApplicationRequestRequestTypeDef

```python
# ArchiveApplicationRequestRequestTypeDef definition

class ArchiveApplicationRequestRequestTypeDef(TypedDict):
    applicationID: str,
    accountID: NotRequired[str],
```

## ArchiveWaveRequestRequestTypeDef

```python
# ArchiveWaveRequestRequestTypeDef definition

class ArchiveWaveRequestRequestTypeDef(TypedDict):
    waveID: str,
    accountID: NotRequired[str],
```

## AssociateApplicationsRequestRequestTypeDef

```python
# AssociateApplicationsRequestRequestTypeDef definition

class AssociateApplicationsRequestRequestTypeDef(TypedDict):
    applicationIDs: Sequence[str],
    waveID: str,
    accountID: NotRequired[str],
```

## AssociateSourceServersRequestRequestTypeDef

```python
# AssociateSourceServersRequestRequestTypeDef definition

class AssociateSourceServersRequestRequestTypeDef(TypedDict):
    applicationID: str,
    sourceServerIDs: Sequence[str],
    accountID: NotRequired[str],
```

## CPUTypeDef

```python
# CPUTypeDef definition

class CPUTypeDef(TypedDict):
    cores: NotRequired[int],
    modelName: NotRequired[str],
```

## ChangeServerLifeCycleStateSourceServerLifecycleTypeDef

```python
# ChangeServerLifeCycleStateSourceServerLifecycleTypeDef definition

class ChangeServerLifeCycleStateSourceServerLifecycleTypeDef(TypedDict):
    state: ChangeServerLifeCycleStateSourceServerLifecycleStateType,  # (1)
```

1. See [:material-code-brackets: ChangeServerLifeCycleStateSourceServerLifecycleStateType](./literals.md#changeserverlifecyclestatesourceserverlifecyclestatetype) 
## ConnectorSsmCommandConfigTypeDef

```python
# ConnectorSsmCommandConfigTypeDef definition

class ConnectorSsmCommandConfigTypeDef(TypedDict):
    cloudWatchOutputEnabled: bool,
    s3OutputEnabled: bool,
    cloudWatchLogGroupName: NotRequired[str],
    outputS3BucketName: NotRequired[str],
```

## CreateApplicationRequestRequestTypeDef

```python
# CreateApplicationRequestRequestTypeDef definition

class CreateApplicationRequestRequestTypeDef(TypedDict):
    name: str,
    accountID: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## LaunchTemplateDiskConfTypeDef

```python
# LaunchTemplateDiskConfTypeDef definition

class LaunchTemplateDiskConfTypeDef(TypedDict):
    iops: NotRequired[int],
    throughput: NotRequired[int],
    volumeType: NotRequired[VolumeTypeType],  # (1)
```

1. See [:material-code-brackets: VolumeTypeType](./literals.md#volumetypetype) 
## LicensingTypeDef

```python
# LicensingTypeDef definition

class LicensingTypeDef(TypedDict):
    osByol: NotRequired[bool],
```

## CreateReplicationConfigurationTemplateRequestRequestTypeDef

```python
# CreateReplicationConfigurationTemplateRequestRequestTypeDef definition

class CreateReplicationConfigurationTemplateRequestRequestTypeDef(TypedDict):
    associateDefaultSecurityGroup: bool,
    bandwidthThrottling: int,
    createPublicIP: bool,
    dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType,  # (1)
    defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType,  # (2)
    ebsEncryption: ReplicationConfigurationEbsEncryptionType,  # (3)
    replicationServerInstanceType: str,
    replicationServersSecurityGroupsIDs: Sequence[str],
    stagingAreaSubnetId: str,
    stagingAreaTags: Mapping[str, str],
    useDedicatedReplicationServer: bool,
    ebsEncryptionKeyArn: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    useFipsEndpoint: NotRequired[bool],
```

1. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype) 
2. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype) 
3. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype) 
## CreateWaveRequestRequestTypeDef

```python
# CreateWaveRequestRequestTypeDef definition

class CreateWaveRequestRequestTypeDef(TypedDict):
    name: str,
    accountID: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## DataReplicationErrorTypeDef

```python
# DataReplicationErrorTypeDef definition

class DataReplicationErrorTypeDef(TypedDict):
    error: NotRequired[DataReplicationErrorStringType],  # (1)
    rawError: NotRequired[str],
```

1. See [:material-code-brackets: DataReplicationErrorStringType](./literals.md#datareplicationerrorstringtype) 
## DataReplicationInfoReplicatedDiskTypeDef

```python
# DataReplicationInfoReplicatedDiskTypeDef definition

class DataReplicationInfoReplicatedDiskTypeDef(TypedDict):
    backloggedStorageBytes: NotRequired[int],
    deviceName: NotRequired[str],
    replicatedStorageBytes: NotRequired[int],
    rescannedStorageBytes: NotRequired[int],
    totalStorageBytes: NotRequired[int],
```

## DataReplicationInitiationStepTypeDef

```python
# DataReplicationInitiationStepTypeDef definition

class DataReplicationInitiationStepTypeDef(TypedDict):
    name: NotRequired[DataReplicationInitiationStepNameType],  # (1)
    status: NotRequired[DataReplicationInitiationStepStatusType],  # (2)
```

1. See [:material-code-brackets: DataReplicationInitiationStepNameType](./literals.md#datareplicationinitiationstepnametype) 
2. See [:material-code-brackets: DataReplicationInitiationStepStatusType](./literals.md#datareplicationinitiationstepstatustype) 
## DeleteApplicationRequestRequestTypeDef

```python
# DeleteApplicationRequestRequestTypeDef definition

class DeleteApplicationRequestRequestTypeDef(TypedDict):
    applicationID: str,
    accountID: NotRequired[str],
```

## DeleteConnectorRequestRequestTypeDef

```python
# DeleteConnectorRequestRequestTypeDef definition

class DeleteConnectorRequestRequestTypeDef(TypedDict):
    connectorID: str,
```

## DeleteJobRequestRequestTypeDef

```python
# DeleteJobRequestRequestTypeDef definition

class DeleteJobRequestRequestTypeDef(TypedDict):
    jobID: str,
    accountID: NotRequired[str],
```

## DeleteLaunchConfigurationTemplateRequestRequestTypeDef

```python
# DeleteLaunchConfigurationTemplateRequestRequestTypeDef definition

class DeleteLaunchConfigurationTemplateRequestRequestTypeDef(TypedDict):
    launchConfigurationTemplateID: str,
```

## DeleteReplicationConfigurationTemplateRequestRequestTypeDef

```python
# DeleteReplicationConfigurationTemplateRequestRequestTypeDef definition

class DeleteReplicationConfigurationTemplateRequestRequestTypeDef(TypedDict):
    replicationConfigurationTemplateID: str,
```

## DeleteSourceServerRequestRequestTypeDef

```python
# DeleteSourceServerRequestRequestTypeDef definition

class DeleteSourceServerRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
```

## DeleteVcenterClientRequestRequestTypeDef

```python
# DeleteVcenterClientRequestRequestTypeDef definition

class DeleteVcenterClientRequestRequestTypeDef(TypedDict):
    vcenterClientID: str,
```

## DeleteWaveRequestRequestTypeDef

```python
# DeleteWaveRequestRequestTypeDef definition

class DeleteWaveRequestRequestTypeDef(TypedDict):
    waveID: str,
    accountID: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeJobLogItemsRequestRequestTypeDef

```python
# DescribeJobLogItemsRequestRequestTypeDef definition

class DescribeJobLogItemsRequestRequestTypeDef(TypedDict):
    jobID: str,
    accountID: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## DescribeJobsRequestFiltersTypeDef

```python
# DescribeJobsRequestFiltersTypeDef definition

class DescribeJobsRequestFiltersTypeDef(TypedDict):
    fromDate: NotRequired[str],
    jobIDs: NotRequired[Sequence[str]],
    toDate: NotRequired[str],
```

## DescribeLaunchConfigurationTemplatesRequestRequestTypeDef

```python
# DescribeLaunchConfigurationTemplatesRequestRequestTypeDef definition

class DescribeLaunchConfigurationTemplatesRequestRequestTypeDef(TypedDict):
    launchConfigurationTemplateIDs: NotRequired[Sequence[str]],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## DescribeReplicationConfigurationTemplatesRequestRequestTypeDef

```python
# DescribeReplicationConfigurationTemplatesRequestRequestTypeDef definition

class DescribeReplicationConfigurationTemplatesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    replicationConfigurationTemplateIDs: NotRequired[Sequence[str]],
```

## ReplicationConfigurationTemplateTypeDef

```python
# ReplicationConfigurationTemplateTypeDef definition

class ReplicationConfigurationTemplateTypeDef(TypedDict):
    replicationConfigurationTemplateID: str,
    arn: NotRequired[str],
    associateDefaultSecurityGroup: NotRequired[bool],
    bandwidthThrottling: NotRequired[int],
    createPublicIP: NotRequired[bool],
    dataPlaneRouting: NotRequired[ReplicationConfigurationDataPlaneRoutingType],  # (1)
    defaultLargeStagingDiskType: NotRequired[ReplicationConfigurationDefaultLargeStagingDiskTypeType],  # (2)
    ebsEncryption: NotRequired[ReplicationConfigurationEbsEncryptionType],  # (3)
    ebsEncryptionKeyArn: NotRequired[str],
    replicationServerInstanceType: NotRequired[str],
    replicationServersSecurityGroupsIDs: NotRequired[List[str]],
    stagingAreaSubnetId: NotRequired[str],
    stagingAreaTags: NotRequired[Dict[str, str]],
    tags: NotRequired[Dict[str, str]],
    useDedicatedReplicationServer: NotRequired[bool],
    useFipsEndpoint: NotRequired[bool],
```

1. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype) 
2. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype) 
3. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype) 
## DescribeSourceServersRequestFiltersTypeDef

```python
# DescribeSourceServersRequestFiltersTypeDef definition

class DescribeSourceServersRequestFiltersTypeDef(TypedDict):
    applicationIDs: NotRequired[Sequence[str]],
    isArchived: NotRequired[bool],
    lifeCycleStates: NotRequired[Sequence[LifeCycleStateType]],  # (1)
    replicationTypes: NotRequired[Sequence[ReplicationTypeType]],  # (2)
    sourceServerIDs: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: LifeCycleStateType](./literals.md#lifecyclestatetype) 
2. See [:material-code-brackets: ReplicationTypeType](./literals.md#replicationtypetype) 
## DescribeVcenterClientsRequestRequestTypeDef

```python
# DescribeVcenterClientsRequestRequestTypeDef definition

class DescribeVcenterClientsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## VcenterClientTypeDef

```python
# VcenterClientTypeDef definition

class VcenterClientTypeDef(TypedDict):
    arn: NotRequired[str],
    datacenterName: NotRequired[str],
    hostname: NotRequired[str],
    lastSeenDatetime: NotRequired[str],
    sourceServerTags: NotRequired[Dict[str, str]],
    tags: NotRequired[Dict[str, str]],
    vcenterClientID: NotRequired[str],
    vcenterUUID: NotRequired[str],
```

## DisassociateApplicationsRequestRequestTypeDef

```python
# DisassociateApplicationsRequestRequestTypeDef definition

class DisassociateApplicationsRequestRequestTypeDef(TypedDict):
    applicationIDs: Sequence[str],
    waveID: str,
    accountID: NotRequired[str],
```

## DisassociateSourceServersRequestRequestTypeDef

```python
# DisassociateSourceServersRequestRequestTypeDef definition

class DisassociateSourceServersRequestRequestTypeDef(TypedDict):
    applicationID: str,
    sourceServerIDs: Sequence[str],
    accountID: NotRequired[str],
```

## DisconnectFromServiceRequestRequestTypeDef

```python
# DisconnectFromServiceRequestRequestTypeDef definition

class DisconnectFromServiceRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
```

## DiskTypeDef

```python
# DiskTypeDef definition

class DiskTypeDef(TypedDict):
    bytes: NotRequired[int],
    deviceName: NotRequired[str],
```

## ExportErrorDataTypeDef

```python
# ExportErrorDataTypeDef definition

class ExportErrorDataTypeDef(TypedDict):
    rawError: NotRequired[str],
```

## ExportTaskSummaryTypeDef

```python
# ExportTaskSummaryTypeDef definition

class ExportTaskSummaryTypeDef(TypedDict):
    applicationsCount: NotRequired[int],
    serversCount: NotRequired[int],
    wavesCount: NotRequired[int],
```

## FinalizeCutoverRequestRequestTypeDef

```python
# FinalizeCutoverRequestRequestTypeDef definition

class FinalizeCutoverRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
```

## GetLaunchConfigurationRequestRequestTypeDef

```python
# GetLaunchConfigurationRequestRequestTypeDef definition

class GetLaunchConfigurationRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
```

## GetReplicationConfigurationRequestRequestTypeDef

```python
# GetReplicationConfigurationRequestRequestTypeDef definition

class GetReplicationConfigurationRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
```

## IdentificationHintsTypeDef

```python
# IdentificationHintsTypeDef definition

class IdentificationHintsTypeDef(TypedDict):
    awsInstanceID: NotRequired[str],
    fqdn: NotRequired[str],
    hostname: NotRequired[str],
    vmPath: NotRequired[str],
    vmWareUuid: NotRequired[str],
```

## ImportErrorDataTypeDef

```python
# ImportErrorDataTypeDef definition

class ImportErrorDataTypeDef(TypedDict):
    accountID: NotRequired[str],
    applicationID: NotRequired[str],
    ec2LaunchTemplateID: NotRequired[str],
    rawError: NotRequired[str],
    rowNumber: NotRequired[int],
    sourceServerID: NotRequired[str],
    waveID: NotRequired[str],
```

## ImportTaskSummaryApplicationsTypeDef

```python
# ImportTaskSummaryApplicationsTypeDef definition

class ImportTaskSummaryApplicationsTypeDef(TypedDict):
    createdCount: NotRequired[int],
    modifiedCount: NotRequired[int],
```

## ImportTaskSummaryServersTypeDef

```python
# ImportTaskSummaryServersTypeDef definition

class ImportTaskSummaryServersTypeDef(TypedDict):
    createdCount: NotRequired[int],
    modifiedCount: NotRequired[int],
```

## ImportTaskSummaryWavesTypeDef

```python
# ImportTaskSummaryWavesTypeDef definition

class ImportTaskSummaryWavesTypeDef(TypedDict):
    createdCount: NotRequired[int],
    modifiedCount: NotRequired[int],
```

## S3BucketSourceTypeDef

```python
# S3BucketSourceTypeDef definition

class S3BucketSourceTypeDef(TypedDict):
    s3Bucket: str,
    s3Key: str,
    s3BucketOwner: NotRequired[str],
```

## JobLogEventDataTypeDef

```python
# JobLogEventDataTypeDef definition

class JobLogEventDataTypeDef(TypedDict):
    conversionServerID: NotRequired[str],
    rawError: NotRequired[str],
    sourceServerID: NotRequired[str],
    targetInstanceID: NotRequired[str],
```

## LaunchedInstanceTypeDef

```python
# LaunchedInstanceTypeDef definition

class LaunchedInstanceTypeDef(TypedDict):
    ec2InstanceID: NotRequired[str],
    firstBoot: NotRequired[FirstBootType],  # (1)
    jobID: NotRequired[str],
```

1. See [:material-code-brackets: FirstBootType](./literals.md#firstboottype) 
## LifeCycleLastCutoverFinalizedTypeDef

```python
# LifeCycleLastCutoverFinalizedTypeDef definition

class LifeCycleLastCutoverFinalizedTypeDef(TypedDict):
    apiCallDateTime: NotRequired[str],
```

## LifeCycleLastCutoverInitiatedTypeDef

```python
# LifeCycleLastCutoverInitiatedTypeDef definition

class LifeCycleLastCutoverInitiatedTypeDef(TypedDict):
    apiCallDateTime: NotRequired[str],
    jobID: NotRequired[str],
```

## LifeCycleLastCutoverRevertedTypeDef

```python
# LifeCycleLastCutoverRevertedTypeDef definition

class LifeCycleLastCutoverRevertedTypeDef(TypedDict):
    apiCallDateTime: NotRequired[str],
```

## LifeCycleLastTestFinalizedTypeDef

```python
# LifeCycleLastTestFinalizedTypeDef definition

class LifeCycleLastTestFinalizedTypeDef(TypedDict):
    apiCallDateTime: NotRequired[str],
```

## LifeCycleLastTestInitiatedTypeDef

```python
# LifeCycleLastTestInitiatedTypeDef definition

class LifeCycleLastTestInitiatedTypeDef(TypedDict):
    apiCallDateTime: NotRequired[str],
    jobID: NotRequired[str],
```

## LifeCycleLastTestRevertedTypeDef

```python
# LifeCycleLastTestRevertedTypeDef definition

class LifeCycleLastTestRevertedTypeDef(TypedDict):
    apiCallDateTime: NotRequired[str],
```

## ListApplicationsRequestFiltersTypeDef

```python
# ListApplicationsRequestFiltersTypeDef definition

class ListApplicationsRequestFiltersTypeDef(TypedDict):
    applicationIDs: NotRequired[Sequence[str]],
    isArchived: NotRequired[bool],
    waveIDs: NotRequired[Sequence[str]],
```

## ListConnectorsRequestFiltersTypeDef

```python
# ListConnectorsRequestFiltersTypeDef definition

class ListConnectorsRequestFiltersTypeDef(TypedDict):
    connectorIDs: NotRequired[Sequence[str]],
```

## ListExportErrorsRequestRequestTypeDef

```python
# ListExportErrorsRequestRequestTypeDef definition

class ListExportErrorsRequestRequestTypeDef(TypedDict):
    exportID: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListExportsRequestFiltersTypeDef

```python
# ListExportsRequestFiltersTypeDef definition

class ListExportsRequestFiltersTypeDef(TypedDict):
    exportIDs: NotRequired[Sequence[str]],
```

## ListImportErrorsRequestRequestTypeDef

```python
# ListImportErrorsRequestRequestTypeDef definition

class ListImportErrorsRequestRequestTypeDef(TypedDict):
    importID: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListImportsRequestFiltersTypeDef

```python
# ListImportsRequestFiltersTypeDef definition

class ListImportsRequestFiltersTypeDef(TypedDict):
    importIDs: NotRequired[Sequence[str]],
```

## ListManagedAccountsRequestRequestTypeDef

```python
# ListManagedAccountsRequestRequestTypeDef definition

class ListManagedAccountsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ManagedAccountTypeDef

```python
# ManagedAccountTypeDef definition

class ManagedAccountTypeDef(TypedDict):
    accountId: NotRequired[str],
```

## SourceServerActionsRequestFiltersTypeDef

```python
# SourceServerActionsRequestFiltersTypeDef definition

class SourceServerActionsRequestFiltersTypeDef(TypedDict):
    actionIDs: NotRequired[Sequence[str]],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## TemplateActionsRequestFiltersTypeDef

```python
# TemplateActionsRequestFiltersTypeDef definition

class TemplateActionsRequestFiltersTypeDef(TypedDict):
    actionIDs: NotRequired[Sequence[str]],
```

## ListWavesRequestFiltersTypeDef

```python
# ListWavesRequestFiltersTypeDef definition

class ListWavesRequestFiltersTypeDef(TypedDict):
    isArchived: NotRequired[bool],
    waveIDs: NotRequired[Sequence[str]],
```

## MarkAsArchivedRequestRequestTypeDef

```python
# MarkAsArchivedRequestRequestTypeDef definition

class MarkAsArchivedRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
```

## NetworkInterfaceTypeDef

```python
# NetworkInterfaceTypeDef definition

class NetworkInterfaceTypeDef(TypedDict):
    ips: NotRequired[List[str]],
    isPrimary: NotRequired[bool],
    macAddress: NotRequired[str],
```

## OSTypeDef

```python
# OSTypeDef definition

class OSTypeDef(TypedDict):
    fullString: NotRequired[str],
```

## PauseReplicationRequestRequestTypeDef

```python
# PauseReplicationRequestRequestTypeDef definition

class PauseReplicationRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
```

## SsmExternalParameterTypeDef

```python
# SsmExternalParameterTypeDef definition

class SsmExternalParameterTypeDef(TypedDict):
    dynamicPath: NotRequired[str],
```

## SsmParameterStoreParameterTypeDef

```python
# SsmParameterStoreParameterTypeDef definition

class SsmParameterStoreParameterTypeDef(TypedDict):
    parameterName: str,
    parameterType: SsmParameterStoreParameterTypeType,  # (1)
```

1. See [:material-code-brackets: SsmParameterStoreParameterTypeType](./literals.md#ssmparameterstoreparametertypetype) 
## RemoveSourceServerActionRequestRequestTypeDef

```python
# RemoveSourceServerActionRequestRequestTypeDef definition

class RemoveSourceServerActionRequestRequestTypeDef(TypedDict):
    actionID: str,
    sourceServerID: str,
    accountID: NotRequired[str],
```

## RemoveTemplateActionRequestRequestTypeDef

```python
# RemoveTemplateActionRequestRequestTypeDef definition

class RemoveTemplateActionRequestRequestTypeDef(TypedDict):
    actionID: str,
    launchConfigurationTemplateID: str,
```

## ReplicationConfigurationReplicatedDiskTypeDef

```python
# ReplicationConfigurationReplicatedDiskTypeDef definition

class ReplicationConfigurationReplicatedDiskTypeDef(TypedDict):
    deviceName: NotRequired[str],
    iops: NotRequired[int],
    isBootDisk: NotRequired[bool],
    stagingDiskType: NotRequired[ReplicationConfigurationReplicatedDiskStagingDiskTypeType],  # (1)
    throughput: NotRequired[int],
```

1. See [:material-code-brackets: ReplicationConfigurationReplicatedDiskStagingDiskTypeType](./literals.md#replicationconfigurationreplicateddiskstagingdisktypetype) 
## ResumeReplicationRequestRequestTypeDef

```python
# ResumeReplicationRequestRequestTypeDef definition

class ResumeReplicationRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
```

## RetryDataReplicationRequestRequestTypeDef

```python
# RetryDataReplicationRequestRequestTypeDef definition

class RetryDataReplicationRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
```

## SourceServerConnectorActionTypeDef

```python
# SourceServerConnectorActionTypeDef definition

class SourceServerConnectorActionTypeDef(TypedDict):
    connectorArn: NotRequired[str],
    credentialsSecretArn: NotRequired[str],
```

## StartCutoverRequestRequestTypeDef

```python
# StartCutoverRequestRequestTypeDef definition

class StartCutoverRequestRequestTypeDef(TypedDict):
    sourceServerIDs: Sequence[str],
    accountID: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## StartExportRequestRequestTypeDef

```python
# StartExportRequestRequestTypeDef definition

class StartExportRequestRequestTypeDef(TypedDict):
    s3Bucket: str,
    s3Key: str,
    s3BucketOwner: NotRequired[str],
```

## StartReplicationRequestRequestTypeDef

```python
# StartReplicationRequestRequestTypeDef definition

class StartReplicationRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
```

## StartTestRequestRequestTypeDef

```python
# StartTestRequestRequestTypeDef definition

class StartTestRequestRequestTypeDef(TypedDict):
    sourceServerIDs: Sequence[str],
    accountID: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## StopReplicationRequestRequestTypeDef

```python
# StopReplicationRequestRequestTypeDef definition

class StopReplicationRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## TerminateTargetInstancesRequestRequestTypeDef

```python
# TerminateTargetInstancesRequestRequestTypeDef definition

class TerminateTargetInstancesRequestRequestTypeDef(TypedDict):
    sourceServerIDs: Sequence[str],
    accountID: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## UnarchiveApplicationRequestRequestTypeDef

```python
# UnarchiveApplicationRequestRequestTypeDef definition

class UnarchiveApplicationRequestRequestTypeDef(TypedDict):
    applicationID: str,
    accountID: NotRequired[str],
```

## UnarchiveWaveRequestRequestTypeDef

```python
# UnarchiveWaveRequestRequestTypeDef definition

class UnarchiveWaveRequestRequestTypeDef(TypedDict):
    waveID: str,
    accountID: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateApplicationRequestRequestTypeDef

```python
# UpdateApplicationRequestRequestTypeDef definition

class UpdateApplicationRequestRequestTypeDef(TypedDict):
    applicationID: str,
    accountID: NotRequired[str],
    description: NotRequired[str],
    name: NotRequired[str],
```

## UpdateReplicationConfigurationTemplateRequestRequestTypeDef

```python
# UpdateReplicationConfigurationTemplateRequestRequestTypeDef definition

class UpdateReplicationConfigurationTemplateRequestRequestTypeDef(TypedDict):
    replicationConfigurationTemplateID: str,
    arn: NotRequired[str],
    associateDefaultSecurityGroup: NotRequired[bool],
    bandwidthThrottling: NotRequired[int],
    createPublicIP: NotRequired[bool],
    dataPlaneRouting: NotRequired[ReplicationConfigurationDataPlaneRoutingType],  # (1)
    defaultLargeStagingDiskType: NotRequired[ReplicationConfigurationDefaultLargeStagingDiskTypeType],  # (2)
    ebsEncryption: NotRequired[ReplicationConfigurationEbsEncryptionType],  # (3)
    ebsEncryptionKeyArn: NotRequired[str],
    replicationServerInstanceType: NotRequired[str],
    replicationServersSecurityGroupsIDs: NotRequired[Sequence[str]],
    stagingAreaSubnetId: NotRequired[str],
    stagingAreaTags: NotRequired[Mapping[str, str]],
    useDedicatedReplicationServer: NotRequired[bool],
    useFipsEndpoint: NotRequired[bool],
```

1. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype) 
2. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype) 
3. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype) 
## UpdateSourceServerReplicationTypeRequestRequestTypeDef

```python
# UpdateSourceServerReplicationTypeRequestRequestTypeDef definition

class UpdateSourceServerReplicationTypeRequestRequestTypeDef(TypedDict):
    replicationType: ReplicationTypeType,  # (1)
    sourceServerID: str,
    accountID: NotRequired[str],
```

1. See [:material-code-brackets: ReplicationTypeType](./literals.md#replicationtypetype) 
## UpdateWaveRequestRequestTypeDef

```python
# UpdateWaveRequestRequestTypeDef definition

class UpdateWaveRequestRequestTypeDef(TypedDict):
    waveID: str,
    accountID: NotRequired[str],
    description: NotRequired[str],
    name: NotRequired[str],
```

## WaveAggregatedStatusTypeDef

```python
# WaveAggregatedStatusTypeDef definition

class WaveAggregatedStatusTypeDef(TypedDict):
    healthStatus: NotRequired[WaveHealthStatusType],  # (1)
    lastUpdateDateTime: NotRequired[str],
    progressStatus: NotRequired[WaveProgressStatusType],  # (2)
    replicationStartedDateTime: NotRequired[str],
    totalApplications: NotRequired[int],
```

1. See [:material-code-brackets: WaveHealthStatusType](./literals.md#wavehealthstatustype) 
2. See [:material-code-brackets: WaveProgressStatusType](./literals.md#waveprogressstatustype) 
## ApplicationTypeDef

```python
# ApplicationTypeDef definition

class ApplicationTypeDef(TypedDict):
    applicationAggregatedStatus: NotRequired[ApplicationAggregatedStatusTypeDef],  # (1)
    applicationID: NotRequired[str],
    arn: NotRequired[str],
    creationDateTime: NotRequired[str],
    description: NotRequired[str],
    isArchived: NotRequired[bool],
    lastModifiedDateTime: NotRequired[str],
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    waveID: NotRequired[str],
```

1. See [:material-code-braces: ApplicationAggregatedStatusTypeDef](./type_defs.md#applicationaggregatedstatustypedef) 
## ApplicationResponseTypeDef

```python
# ApplicationResponseTypeDef definition

class ApplicationResponseTypeDef(TypedDict):
    applicationAggregatedStatus: ApplicationAggregatedStatusTypeDef,  # (1)
    applicationID: str,
    arn: str,
    creationDateTime: str,
    description: str,
    isArchived: bool,
    lastModifiedDateTime: str,
    name: str,
    tags: Dict[str, str],
    waveID: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationAggregatedStatusTypeDef](./type_defs.md#applicationaggregatedstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReplicationConfigurationTemplateResponseTypeDef

```python
# ReplicationConfigurationTemplateResponseTypeDef definition

class ReplicationConfigurationTemplateResponseTypeDef(TypedDict):
    arn: str,
    associateDefaultSecurityGroup: bool,
    bandwidthThrottling: int,
    createPublicIP: bool,
    dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType,  # (1)
    defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType,  # (2)
    ebsEncryption: ReplicationConfigurationEbsEncryptionType,  # (3)
    ebsEncryptionKeyArn: str,
    replicationConfigurationTemplateID: str,
    replicationServerInstanceType: str,
    replicationServersSecurityGroupsIDs: List[str],
    stagingAreaSubnetId: str,
    stagingAreaTags: Dict[str, str],
    tags: Dict[str, str],
    useDedicatedReplicationServer: bool,
    useFipsEndpoint: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype) 
2. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype) 
3. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ChangeServerLifeCycleStateRequestRequestTypeDef

```python
# ChangeServerLifeCycleStateRequestRequestTypeDef definition

class ChangeServerLifeCycleStateRequestRequestTypeDef(TypedDict):
    lifeCycle: ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,  # (1)
    sourceServerID: str,
    accountID: NotRequired[str],
```

1. See [:material-code-braces: ChangeServerLifeCycleStateSourceServerLifecycleTypeDef](./type_defs.md#changeserverlifecyclestatesourceserverlifecycletypedef) 
## ConnectorResponseTypeDef

```python
# ConnectorResponseTypeDef definition

class ConnectorResponseTypeDef(TypedDict):
    arn: str,
    connectorID: str,
    name: str,
    ssmCommandConfig: ConnectorSsmCommandConfigTypeDef,  # (1)
    ssmInstanceID: str,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConnectorSsmCommandConfigTypeDef](./type_defs.md#connectorssmcommandconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConnectorTypeDef

```python
# ConnectorTypeDef definition

class ConnectorTypeDef(TypedDict):
    arn: NotRequired[str],
    connectorID: NotRequired[str],
    name: NotRequired[str],
    ssmCommandConfig: NotRequired[ConnectorSsmCommandConfigTypeDef],  # (1)
    ssmInstanceID: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ConnectorSsmCommandConfigTypeDef](./type_defs.md#connectorssmcommandconfigtypedef) 
## CreateConnectorRequestRequestTypeDef

```python
# CreateConnectorRequestRequestTypeDef definition

class CreateConnectorRequestRequestTypeDef(TypedDict):
    name: str,
    ssmInstanceID: str,
    ssmCommandConfig: NotRequired[ConnectorSsmCommandConfigTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ConnectorSsmCommandConfigTypeDef](./type_defs.md#connectorssmcommandconfigtypedef) 
## UpdateConnectorRequestRequestTypeDef

```python
# UpdateConnectorRequestRequestTypeDef definition

class UpdateConnectorRequestRequestTypeDef(TypedDict):
    connectorID: str,
    name: NotRequired[str],
    ssmCommandConfig: NotRequired[ConnectorSsmCommandConfigTypeDef],  # (1)
```

1. See [:material-code-braces: ConnectorSsmCommandConfigTypeDef](./type_defs.md#connectorssmcommandconfigtypedef) 
## DataReplicationInitiationTypeDef

```python
# DataReplicationInitiationTypeDef definition

class DataReplicationInitiationTypeDef(TypedDict):
    nextAttemptDateTime: NotRequired[str],
    startDateTime: NotRequired[str],
    steps: NotRequired[List[DataReplicationInitiationStepTypeDef]],  # (1)
```

1. See [:material-code-braces: DataReplicationInitiationStepTypeDef](./type_defs.md#datareplicationinitiationsteptypedef) 
## DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef

```python
# DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef definition

class DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef(TypedDict):
    jobID: str,
    accountID: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef

```python
# DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef definition

class DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef(TypedDict):
    launchConfigurationTemplateIDs: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef

```python
# DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef definition

class DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef(TypedDict):
    replicationConfigurationTemplateIDs: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef

```python
# DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef definition

class DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListExportErrorsRequestListExportErrorsPaginateTypeDef

```python
# ListExportErrorsRequestListExportErrorsPaginateTypeDef definition

class ListExportErrorsRequestListExportErrorsPaginateTypeDef(TypedDict):
    exportID: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListImportErrorsRequestListImportErrorsPaginateTypeDef

```python
# ListImportErrorsRequestListImportErrorsPaginateTypeDef definition

class ListImportErrorsRequestListImportErrorsPaginateTypeDef(TypedDict):
    importID: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListManagedAccountsRequestListManagedAccountsPaginateTypeDef

```python
# ListManagedAccountsRequestListManagedAccountsPaginateTypeDef definition

class ListManagedAccountsRequestListManagedAccountsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeJobsRequestDescribeJobsPaginateTypeDef

```python
# DescribeJobsRequestDescribeJobsPaginateTypeDef definition

class DescribeJobsRequestDescribeJobsPaginateTypeDef(TypedDict):
    accountID: NotRequired[str],
    filters: NotRequired[DescribeJobsRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DescribeJobsRequestFiltersTypeDef](./type_defs.md#describejobsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeJobsRequestRequestTypeDef

```python
# DescribeJobsRequestRequestTypeDef definition

class DescribeJobsRequestRequestTypeDef(TypedDict):
    accountID: NotRequired[str],
    filters: NotRequired[DescribeJobsRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DescribeJobsRequestFiltersTypeDef](./type_defs.md#describejobsrequestfilterstypedef) 
## DescribeReplicationConfigurationTemplatesResponseTypeDef

```python
# DescribeReplicationConfigurationTemplatesResponseTypeDef definition

class DescribeReplicationConfigurationTemplatesResponseTypeDef(TypedDict):
    items: List[ReplicationConfigurationTemplateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ReplicationConfigurationTemplateTypeDef](./type_defs.md#replicationconfigurationtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef

```python
# DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef definition

class DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef(TypedDict):
    accountID: NotRequired[str],
    filters: NotRequired[DescribeSourceServersRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DescribeSourceServersRequestFiltersTypeDef](./type_defs.md#describesourceserversrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSourceServersRequestRequestTypeDef

```python
# DescribeSourceServersRequestRequestTypeDef definition

class DescribeSourceServersRequestRequestTypeDef(TypedDict):
    accountID: NotRequired[str],
    filters: NotRequired[DescribeSourceServersRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DescribeSourceServersRequestFiltersTypeDef](./type_defs.md#describesourceserversrequestfilterstypedef) 
## DescribeVcenterClientsResponseTypeDef

```python
# DescribeVcenterClientsResponseTypeDef definition

class DescribeVcenterClientsResponseTypeDef(TypedDict):
    items: List[VcenterClientTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: VcenterClientTypeDef](./type_defs.md#vcenterclienttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportTaskErrorTypeDef

```python
# ExportTaskErrorTypeDef definition

class ExportTaskErrorTypeDef(TypedDict):
    errorData: NotRequired[ExportErrorDataTypeDef],  # (1)
    errorDateTime: NotRequired[str],
```

1. See [:material-code-braces: ExportErrorDataTypeDef](./type_defs.md#exporterrordatatypedef) 
## ExportTaskTypeDef

```python
# ExportTaskTypeDef definition

class ExportTaskTypeDef(TypedDict):
    creationDateTime: NotRequired[str],
    endDateTime: NotRequired[str],
    exportID: NotRequired[str],
    progressPercentage: NotRequired[float],
    s3Bucket: NotRequired[str],
    s3BucketOwner: NotRequired[str],
    s3Key: NotRequired[str],
    status: NotRequired[ExportStatusType],  # (1)
    summary: NotRequired[ExportTaskSummaryTypeDef],  # (2)
```

1. See [:material-code-brackets: ExportStatusType](./literals.md#exportstatustype) 
2. See [:material-code-braces: ExportTaskSummaryTypeDef](./type_defs.md#exporttasksummarytypedef) 
## ImportTaskErrorTypeDef

```python
# ImportTaskErrorTypeDef definition

class ImportTaskErrorTypeDef(TypedDict):
    errorData: NotRequired[ImportErrorDataTypeDef],  # (1)
    errorDateTime: NotRequired[str],
    errorType: NotRequired[ImportErrorTypeType],  # (2)
```

1. See [:material-code-braces: ImportErrorDataTypeDef](./type_defs.md#importerrordatatypedef) 
2. See [:material-code-brackets: ImportErrorTypeType](./literals.md#importerrortypetype) 
## ImportTaskSummaryTypeDef

```python
# ImportTaskSummaryTypeDef definition

class ImportTaskSummaryTypeDef(TypedDict):
    applications: NotRequired[ImportTaskSummaryApplicationsTypeDef],  # (1)
    servers: NotRequired[ImportTaskSummaryServersTypeDef],  # (2)
    waves: NotRequired[ImportTaskSummaryWavesTypeDef],  # (3)
```

1. See [:material-code-braces: ImportTaskSummaryApplicationsTypeDef](./type_defs.md#importtasksummaryapplicationstypedef) 
2. See [:material-code-braces: ImportTaskSummaryServersTypeDef](./type_defs.md#importtasksummaryserverstypedef) 
3. See [:material-code-braces: ImportTaskSummaryWavesTypeDef](./type_defs.md#importtasksummarywavestypedef) 
## StartImportRequestRequestTypeDef

```python
# StartImportRequestRequestTypeDef definition

class StartImportRequestRequestTypeDef(TypedDict):
    s3BucketSource: S3BucketSourceTypeDef,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: S3BucketSourceTypeDef](./type_defs.md#s3bucketsourcetypedef) 
## JobLogTypeDef

```python
# JobLogTypeDef definition

class JobLogTypeDef(TypedDict):
    event: NotRequired[JobLogEventType],  # (1)
    eventData: NotRequired[JobLogEventDataTypeDef],  # (2)
    logDateTime: NotRequired[str],
```

1. See [:material-code-brackets: JobLogEventType](./literals.md#joblogeventtype) 
2. See [:material-code-braces: JobLogEventDataTypeDef](./type_defs.md#joblogeventdatatypedef) 
## LifeCycleLastCutoverTypeDef

```python
# LifeCycleLastCutoverTypeDef definition

class LifeCycleLastCutoverTypeDef(TypedDict):
    finalized: NotRequired[LifeCycleLastCutoverFinalizedTypeDef],  # (1)
    initiated: NotRequired[LifeCycleLastCutoverInitiatedTypeDef],  # (2)
    reverted: NotRequired[LifeCycleLastCutoverRevertedTypeDef],  # (3)
```

1. See [:material-code-braces: LifeCycleLastCutoverFinalizedTypeDef](./type_defs.md#lifecyclelastcutoverfinalizedtypedef) 
2. See [:material-code-braces: LifeCycleLastCutoverInitiatedTypeDef](./type_defs.md#lifecyclelastcutoverinitiatedtypedef) 
3. See [:material-code-braces: LifeCycleLastCutoverRevertedTypeDef](./type_defs.md#lifecyclelastcutoverrevertedtypedef) 
## LifeCycleLastTestTypeDef

```python
# LifeCycleLastTestTypeDef definition

class LifeCycleLastTestTypeDef(TypedDict):
    finalized: NotRequired[LifeCycleLastTestFinalizedTypeDef],  # (1)
    initiated: NotRequired[LifeCycleLastTestInitiatedTypeDef],  # (2)
    reverted: NotRequired[LifeCycleLastTestRevertedTypeDef],  # (3)
```

1. See [:material-code-braces: LifeCycleLastTestFinalizedTypeDef](./type_defs.md#lifecyclelasttestfinalizedtypedef) 
2. See [:material-code-braces: LifeCycleLastTestInitiatedTypeDef](./type_defs.md#lifecyclelasttestinitiatedtypedef) 
3. See [:material-code-braces: LifeCycleLastTestRevertedTypeDef](./type_defs.md#lifecyclelasttestrevertedtypedef) 
## ListApplicationsRequestListApplicationsPaginateTypeDef

```python
# ListApplicationsRequestListApplicationsPaginateTypeDef definition

class ListApplicationsRequestListApplicationsPaginateTypeDef(TypedDict):
    accountID: NotRequired[str],
    filters: NotRequired[ListApplicationsRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListApplicationsRequestFiltersTypeDef](./type_defs.md#listapplicationsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListApplicationsRequestRequestTypeDef

```python
# ListApplicationsRequestRequestTypeDef definition

class ListApplicationsRequestRequestTypeDef(TypedDict):
    accountID: NotRequired[str],
    filters: NotRequired[ListApplicationsRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ListApplicationsRequestFiltersTypeDef](./type_defs.md#listapplicationsrequestfilterstypedef) 
## ListConnectorsRequestListConnectorsPaginateTypeDef

```python
# ListConnectorsRequestListConnectorsPaginateTypeDef definition

class ListConnectorsRequestListConnectorsPaginateTypeDef(TypedDict):
    filters: NotRequired[ListConnectorsRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListConnectorsRequestFiltersTypeDef](./type_defs.md#listconnectorsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConnectorsRequestRequestTypeDef

```python
# ListConnectorsRequestRequestTypeDef definition

class ListConnectorsRequestRequestTypeDef(TypedDict):
    filters: NotRequired[ListConnectorsRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ListConnectorsRequestFiltersTypeDef](./type_defs.md#listconnectorsrequestfilterstypedef) 
## ListExportsRequestListExportsPaginateTypeDef

```python
# ListExportsRequestListExportsPaginateTypeDef definition

class ListExportsRequestListExportsPaginateTypeDef(TypedDict):
    filters: NotRequired[ListExportsRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListExportsRequestFiltersTypeDef](./type_defs.md#listexportsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListExportsRequestRequestTypeDef

```python
# ListExportsRequestRequestTypeDef definition

class ListExportsRequestRequestTypeDef(TypedDict):
    filters: NotRequired[ListExportsRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ListExportsRequestFiltersTypeDef](./type_defs.md#listexportsrequestfilterstypedef) 
## ListImportsRequestListImportsPaginateTypeDef

```python
# ListImportsRequestListImportsPaginateTypeDef definition

class ListImportsRequestListImportsPaginateTypeDef(TypedDict):
    filters: NotRequired[ListImportsRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListImportsRequestFiltersTypeDef](./type_defs.md#listimportsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListImportsRequestRequestTypeDef

```python
# ListImportsRequestRequestTypeDef definition

class ListImportsRequestRequestTypeDef(TypedDict):
    filters: NotRequired[ListImportsRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ListImportsRequestFiltersTypeDef](./type_defs.md#listimportsrequestfilterstypedef) 
## ListManagedAccountsResponseTypeDef

```python
# ListManagedAccountsResponseTypeDef definition

class ListManagedAccountsResponseTypeDef(TypedDict):
    items: List[ManagedAccountTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ManagedAccountTypeDef](./type_defs.md#managedaccounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef

```python
# ListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef definition

class ListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
    filters: NotRequired[SourceServerActionsRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SourceServerActionsRequestFiltersTypeDef](./type_defs.md#sourceserveractionsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSourceServerActionsRequestRequestTypeDef

```python
# ListSourceServerActionsRequestRequestTypeDef definition

class ListSourceServerActionsRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
    filters: NotRequired[SourceServerActionsRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SourceServerActionsRequestFiltersTypeDef](./type_defs.md#sourceserveractionsrequestfilterstypedef) 
## ListTemplateActionsRequestListTemplateActionsPaginateTypeDef

```python
# ListTemplateActionsRequestListTemplateActionsPaginateTypeDef definition

class ListTemplateActionsRequestListTemplateActionsPaginateTypeDef(TypedDict):
    launchConfigurationTemplateID: str,
    filters: NotRequired[TemplateActionsRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: TemplateActionsRequestFiltersTypeDef](./type_defs.md#templateactionsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTemplateActionsRequestRequestTypeDef

```python
# ListTemplateActionsRequestRequestTypeDef definition

class ListTemplateActionsRequestRequestTypeDef(TypedDict):
    launchConfigurationTemplateID: str,
    filters: NotRequired[TemplateActionsRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TemplateActionsRequestFiltersTypeDef](./type_defs.md#templateactionsrequestfilterstypedef) 
## ListWavesRequestListWavesPaginateTypeDef

```python
# ListWavesRequestListWavesPaginateTypeDef definition

class ListWavesRequestListWavesPaginateTypeDef(TypedDict):
    accountID: NotRequired[str],
    filters: NotRequired[ListWavesRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListWavesRequestFiltersTypeDef](./type_defs.md#listwavesrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWavesRequestRequestTypeDef

```python
# ListWavesRequestRequestTypeDef definition

class ListWavesRequestRequestTypeDef(TypedDict):
    accountID: NotRequired[str],
    filters: NotRequired[ListWavesRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ListWavesRequestFiltersTypeDef](./type_defs.md#listwavesrequestfilterstypedef) 
## SourcePropertiesTypeDef

```python
# SourcePropertiesTypeDef definition

class SourcePropertiesTypeDef(TypedDict):
    cpus: NotRequired[List[CPUTypeDef]],  # (1)
    disks: NotRequired[List[DiskTypeDef]],  # (2)
    identificationHints: NotRequired[IdentificationHintsTypeDef],  # (3)
    lastUpdatedDateTime: NotRequired[str],
    networkInterfaces: NotRequired[List[NetworkInterfaceTypeDef]],  # (4)
    os: NotRequired[OSTypeDef],  # (5)
    ramBytes: NotRequired[int],
    recommendedInstanceType: NotRequired[str],
```

1. See [:material-code-braces: CPUTypeDef](./type_defs.md#cputypedef) 
2. See [:material-code-braces: DiskTypeDef](./type_defs.md#disktypedef) 
3. See [:material-code-braces: IdentificationHintsTypeDef](./type_defs.md#identificationhintstypedef) 
4. See [:material-code-braces: NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef) 
5. See [:material-code-braces: OSTypeDef](./type_defs.md#ostypedef) 
## PutSourceServerActionRequestRequestTypeDef

```python
# PutSourceServerActionRequestRequestTypeDef definition

class PutSourceServerActionRequestRequestTypeDef(TypedDict):
    actionID: str,
    actionName: str,
    documentIdentifier: str,
    order: int,
    sourceServerID: str,
    accountID: NotRequired[str],
    active: NotRequired[bool],
    category: NotRequired[ActionCategoryType],  # (1)
    description: NotRequired[str],
    documentVersion: NotRequired[str],
    externalParameters: NotRequired[Mapping[str, SsmExternalParameterTypeDef]],  # (2)
    mustSucceedForCutover: NotRequired[bool],
    parameters: NotRequired[Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]]],  # (3)
    timeoutSeconds: NotRequired[int],
```

1. See [:material-code-brackets: ActionCategoryType](./literals.md#actioncategorytype) 
2. See [:material-code-braces: SsmExternalParameterTypeDef](./type_defs.md#ssmexternalparametertypedef) 
3. See [:material-code-braces: SsmParameterStoreParameterTypeDef](./type_defs.md#ssmparameterstoreparametertypedef) 
## PutTemplateActionRequestRequestTypeDef

```python
# PutTemplateActionRequestRequestTypeDef definition

class PutTemplateActionRequestRequestTypeDef(TypedDict):
    actionID: str,
    actionName: str,
    documentIdentifier: str,
    launchConfigurationTemplateID: str,
    order: int,
    active: NotRequired[bool],
    category: NotRequired[ActionCategoryType],  # (1)
    description: NotRequired[str],
    documentVersion: NotRequired[str],
    externalParameters: NotRequired[Mapping[str, SsmExternalParameterTypeDef]],  # (2)
    mustSucceedForCutover: NotRequired[bool],
    operatingSystem: NotRequired[str],
    parameters: NotRequired[Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]]],  # (3)
    timeoutSeconds: NotRequired[int],
```

1. See [:material-code-brackets: ActionCategoryType](./literals.md#actioncategorytype) 
2. See [:material-code-braces: SsmExternalParameterTypeDef](./type_defs.md#ssmexternalparametertypedef) 
3. See [:material-code-braces: SsmParameterStoreParameterTypeDef](./type_defs.md#ssmparameterstoreparametertypedef) 
## SourceServerActionDocumentResponseTypeDef

```python
# SourceServerActionDocumentResponseTypeDef definition

class SourceServerActionDocumentResponseTypeDef(TypedDict):
    actionID: str,
    actionName: str,
    active: bool,
    category: ActionCategoryType,  # (1)
    description: str,
    documentIdentifier: str,
    documentVersion: str,
    externalParameters: Dict[str, SsmExternalParameterTypeDef],  # (2)
    mustSucceedForCutover: bool,
    order: int,
    parameters: Dict[str, List[SsmParameterStoreParameterTypeDef]],  # (3)
    timeoutSeconds: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ActionCategoryType](./literals.md#actioncategorytype) 
2. See [:material-code-braces: SsmExternalParameterTypeDef](./type_defs.md#ssmexternalparametertypedef) 
3. See [:material-code-braces: SsmParameterStoreParameterTypeDef](./type_defs.md#ssmparameterstoreparametertypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SourceServerActionDocumentTypeDef

```python
# SourceServerActionDocumentTypeDef definition

class SourceServerActionDocumentTypeDef(TypedDict):
    actionID: NotRequired[str],
    actionName: NotRequired[str],
    active: NotRequired[bool],
    category: NotRequired[ActionCategoryType],  # (1)
    description: NotRequired[str],
    documentIdentifier: NotRequired[str],
    documentVersion: NotRequired[str],
    externalParameters: NotRequired[Dict[str, SsmExternalParameterTypeDef]],  # (2)
    mustSucceedForCutover: NotRequired[bool],
    order: NotRequired[int],
    parameters: NotRequired[Dict[str, List[SsmParameterStoreParameterTypeDef]]],  # (3)
    timeoutSeconds: NotRequired[int],
```

1. See [:material-code-brackets: ActionCategoryType](./literals.md#actioncategorytype) 
2. See [:material-code-braces: SsmExternalParameterTypeDef](./type_defs.md#ssmexternalparametertypedef) 
3. See [:material-code-braces: SsmParameterStoreParameterTypeDef](./type_defs.md#ssmparameterstoreparametertypedef) 
## SsmDocumentOutputTypeDef

```python
# SsmDocumentOutputTypeDef definition

class SsmDocumentOutputTypeDef(TypedDict):
    actionName: str,
    ssmDocumentName: str,
    externalParameters: NotRequired[Dict[str, SsmExternalParameterTypeDef]],  # (1)
    mustSucceedForCutover: NotRequired[bool],
    parameters: NotRequired[Dict[str, List[SsmParameterStoreParameterTypeDef]]],  # (2)
    timeoutSeconds: NotRequired[int],
```

1. See [:material-code-braces: SsmExternalParameterTypeDef](./type_defs.md#ssmexternalparametertypedef) 
2. See [:material-code-braces: SsmParameterStoreParameterTypeDef](./type_defs.md#ssmparameterstoreparametertypedef) 
## SsmDocumentTypeDef

```python
# SsmDocumentTypeDef definition

class SsmDocumentTypeDef(TypedDict):
    actionName: str,
    ssmDocumentName: str,
    externalParameters: NotRequired[Mapping[str, SsmExternalParameterTypeDef]],  # (1)
    mustSucceedForCutover: NotRequired[bool],
    parameters: NotRequired[Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]]],  # (2)
    timeoutSeconds: NotRequired[int],
```

1. See [:material-code-braces: SsmExternalParameterTypeDef](./type_defs.md#ssmexternalparametertypedef) 
2. See [:material-code-braces: SsmParameterStoreParameterTypeDef](./type_defs.md#ssmparameterstoreparametertypedef) 
## TemplateActionDocumentResponseTypeDef

```python
# TemplateActionDocumentResponseTypeDef definition

class TemplateActionDocumentResponseTypeDef(TypedDict):
    actionID: str,
    actionName: str,
    active: bool,
    category: ActionCategoryType,  # (1)
    description: str,
    documentIdentifier: str,
    documentVersion: str,
    externalParameters: Dict[str, SsmExternalParameterTypeDef],  # (2)
    mustSucceedForCutover: bool,
    operatingSystem: str,
    order: int,
    parameters: Dict[str, List[SsmParameterStoreParameterTypeDef]],  # (3)
    timeoutSeconds: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ActionCategoryType](./literals.md#actioncategorytype) 
2. See [:material-code-braces: SsmExternalParameterTypeDef](./type_defs.md#ssmexternalparametertypedef) 
3. See [:material-code-braces: SsmParameterStoreParameterTypeDef](./type_defs.md#ssmparameterstoreparametertypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TemplateActionDocumentTypeDef

```python
# TemplateActionDocumentTypeDef definition

class TemplateActionDocumentTypeDef(TypedDict):
    actionID: NotRequired[str],
    actionName: NotRequired[str],
    active: NotRequired[bool],
    category: NotRequired[ActionCategoryType],  # (1)
    description: NotRequired[str],
    documentIdentifier: NotRequired[str],
    documentVersion: NotRequired[str],
    externalParameters: NotRequired[Dict[str, SsmExternalParameterTypeDef]],  # (2)
    mustSucceedForCutover: NotRequired[bool],
    operatingSystem: NotRequired[str],
    order: NotRequired[int],
    parameters: NotRequired[Dict[str, List[SsmParameterStoreParameterTypeDef]]],  # (3)
    timeoutSeconds: NotRequired[int],
```

1. See [:material-code-brackets: ActionCategoryType](./literals.md#actioncategorytype) 
2. See [:material-code-braces: SsmExternalParameterTypeDef](./type_defs.md#ssmexternalparametertypedef) 
3. See [:material-code-braces: SsmParameterStoreParameterTypeDef](./type_defs.md#ssmparameterstoreparametertypedef) 
## ReplicationConfigurationTypeDef

```python
# ReplicationConfigurationTypeDef definition

class ReplicationConfigurationTypeDef(TypedDict):
    associateDefaultSecurityGroup: bool,
    bandwidthThrottling: int,
    createPublicIP: bool,
    dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType,  # (1)
    defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType,  # (2)
    ebsEncryption: ReplicationConfigurationEbsEncryptionType,  # (3)
    ebsEncryptionKeyArn: str,
    name: str,
    replicatedDisks: List[ReplicationConfigurationReplicatedDiskTypeDef],  # (4)
    replicationServerInstanceType: str,
    replicationServersSecurityGroupsIDs: List[str],
    sourceServerID: str,
    stagingAreaSubnetId: str,
    stagingAreaTags: Dict[str, str],
    useDedicatedReplicationServer: bool,
    useFipsEndpoint: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype) 
2. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype) 
3. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype) 
4. See [:material-code-braces: ReplicationConfigurationReplicatedDiskTypeDef](./type_defs.md#replicationconfigurationreplicateddisktypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateReplicationConfigurationRequestRequestTypeDef

```python
# UpdateReplicationConfigurationRequestRequestTypeDef definition

class UpdateReplicationConfigurationRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
    associateDefaultSecurityGroup: NotRequired[bool],
    bandwidthThrottling: NotRequired[int],
    createPublicIP: NotRequired[bool],
    dataPlaneRouting: NotRequired[ReplicationConfigurationDataPlaneRoutingType],  # (1)
    defaultLargeStagingDiskType: NotRequired[ReplicationConfigurationDefaultLargeStagingDiskTypeType],  # (2)
    ebsEncryption: NotRequired[ReplicationConfigurationEbsEncryptionType],  # (3)
    ebsEncryptionKeyArn: NotRequired[str],
    name: NotRequired[str],
    replicatedDisks: NotRequired[Sequence[ReplicationConfigurationReplicatedDiskTypeDef]],  # (4)
    replicationServerInstanceType: NotRequired[str],
    replicationServersSecurityGroupsIDs: NotRequired[Sequence[str]],
    stagingAreaSubnetId: NotRequired[str],
    stagingAreaTags: NotRequired[Mapping[str, str]],
    useDedicatedReplicationServer: NotRequired[bool],
    useFipsEndpoint: NotRequired[bool],
```

1. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype) 
2. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype) 
3. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype) 
4. See [:material-code-braces: ReplicationConfigurationReplicatedDiskTypeDef](./type_defs.md#replicationconfigurationreplicateddisktypedef) 
## UpdateSourceServerRequestRequestTypeDef

```python
# UpdateSourceServerRequestRequestTypeDef definition

class UpdateSourceServerRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
    connectorAction: NotRequired[SourceServerConnectorActionTypeDef],  # (1)
```

1. See [:material-code-braces: SourceServerConnectorActionTypeDef](./type_defs.md#sourceserverconnectoractiontypedef) 
## WaveResponseTypeDef

```python
# WaveResponseTypeDef definition

class WaveResponseTypeDef(TypedDict):
    arn: str,
    creationDateTime: str,
    description: str,
    isArchived: bool,
    lastModifiedDateTime: str,
    name: str,
    tags: Dict[str, str],
    waveAggregatedStatus: WaveAggregatedStatusTypeDef,  # (1)
    waveID: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WaveAggregatedStatusTypeDef](./type_defs.md#waveaggregatedstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WaveTypeDef

```python
# WaveTypeDef definition

class WaveTypeDef(TypedDict):
    arn: NotRequired[str],
    creationDateTime: NotRequired[str],
    description: NotRequired[str],
    isArchived: NotRequired[bool],
    lastModifiedDateTime: NotRequired[str],
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    waveAggregatedStatus: NotRequired[WaveAggregatedStatusTypeDef],  # (1)
    waveID: NotRequired[str],
```

1. See [:material-code-braces: WaveAggregatedStatusTypeDef](./type_defs.md#waveaggregatedstatustypedef) 
## ListApplicationsResponseTypeDef

```python
# ListApplicationsResponseTypeDef definition

class ListApplicationsResponseTypeDef(TypedDict):
    items: List[ApplicationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConnectorsResponseTypeDef

```python
# ListConnectorsResponseTypeDef definition

class ListConnectorsResponseTypeDef(TypedDict):
    items: List[ConnectorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ConnectorTypeDef](./type_defs.md#connectortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataReplicationInfoTypeDef

```python
# DataReplicationInfoTypeDef definition

class DataReplicationInfoTypeDef(TypedDict):
    dataReplicationError: NotRequired[DataReplicationErrorTypeDef],  # (1)
    dataReplicationInitiation: NotRequired[DataReplicationInitiationTypeDef],  # (2)
    dataReplicationState: NotRequired[DataReplicationStateType],  # (3)
    etaDateTime: NotRequired[str],
    lagDuration: NotRequired[str],
    lastSnapshotDateTime: NotRequired[str],
    replicatedDisks: NotRequired[List[DataReplicationInfoReplicatedDiskTypeDef]],  # (4)
```

1. See [:material-code-braces: DataReplicationErrorTypeDef](./type_defs.md#datareplicationerrortypedef) 
2. See [:material-code-braces: DataReplicationInitiationTypeDef](./type_defs.md#datareplicationinitiationtypedef) 
3. See [:material-code-brackets: DataReplicationStateType](./literals.md#datareplicationstatetype) 
4. See [:material-code-braces: DataReplicationInfoReplicatedDiskTypeDef](./type_defs.md#datareplicationinforeplicateddisktypedef) 
## ListExportErrorsResponseTypeDef

```python
# ListExportErrorsResponseTypeDef definition

class ListExportErrorsResponseTypeDef(TypedDict):
    items: List[ExportTaskErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ExportTaskErrorTypeDef](./type_defs.md#exporttaskerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListExportsResponseTypeDef

```python
# ListExportsResponseTypeDef definition

class ListExportsResponseTypeDef(TypedDict):
    items: List[ExportTaskTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ExportTaskTypeDef](./type_defs.md#exporttasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartExportResponseTypeDef

```python
# StartExportResponseTypeDef definition

class StartExportResponseTypeDef(TypedDict):
    exportTask: ExportTaskTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExportTaskTypeDef](./type_defs.md#exporttasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListImportErrorsResponseTypeDef

```python
# ListImportErrorsResponseTypeDef definition

class ListImportErrorsResponseTypeDef(TypedDict):
    items: List[ImportTaskErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ImportTaskErrorTypeDef](./type_defs.md#importtaskerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportTaskTypeDef

```python
# ImportTaskTypeDef definition

class ImportTaskTypeDef(TypedDict):
    creationDateTime: NotRequired[str],
    endDateTime: NotRequired[str],
    importID: NotRequired[str],
    progressPercentage: NotRequired[float],
    s3BucketSource: NotRequired[S3BucketSourceTypeDef],  # (1)
    status: NotRequired[ImportStatusType],  # (2)
    summary: NotRequired[ImportTaskSummaryTypeDef],  # (3)
```

1. See [:material-code-braces: S3BucketSourceTypeDef](./type_defs.md#s3bucketsourcetypedef) 
2. See [:material-code-brackets: ImportStatusType](./literals.md#importstatustype) 
3. See [:material-code-braces: ImportTaskSummaryTypeDef](./type_defs.md#importtasksummarytypedef) 
## DescribeJobLogItemsResponseTypeDef

```python
# DescribeJobLogItemsResponseTypeDef definition

class DescribeJobLogItemsResponseTypeDef(TypedDict):
    items: List[JobLogTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: JobLogTypeDef](./type_defs.md#joblogtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LifeCycleTypeDef

```python
# LifeCycleTypeDef definition

class LifeCycleTypeDef(TypedDict):
    addedToServiceDateTime: NotRequired[str],
    elapsedReplicationDuration: NotRequired[str],
    firstByteDateTime: NotRequired[str],
    lastCutover: NotRequired[LifeCycleLastCutoverTypeDef],  # (1)
    lastSeenByServiceDateTime: NotRequired[str],
    lastTest: NotRequired[LifeCycleLastTestTypeDef],  # (2)
    state: NotRequired[LifeCycleStateType],  # (3)
```

1. See [:material-code-braces: LifeCycleLastCutoverTypeDef](./type_defs.md#lifecyclelastcutovertypedef) 
2. See [:material-code-braces: LifeCycleLastTestTypeDef](./type_defs.md#lifecyclelasttesttypedef) 
3. See [:material-code-brackets: LifeCycleStateType](./literals.md#lifecyclestatetype) 
## ListSourceServerActionsResponseTypeDef

```python
# ListSourceServerActionsResponseTypeDef definition

class ListSourceServerActionsResponseTypeDef(TypedDict):
    items: List[SourceServerActionDocumentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SourceServerActionDocumentTypeDef](./type_defs.md#sourceserveractiondocumenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JobPostLaunchActionsLaunchStatusTypeDef

```python
# JobPostLaunchActionsLaunchStatusTypeDef definition

class JobPostLaunchActionsLaunchStatusTypeDef(TypedDict):
    executionID: NotRequired[str],
    executionStatus: NotRequired[PostLaunchActionExecutionStatusType],  # (1)
    failureReason: NotRequired[str],
    ssmDocument: NotRequired[SsmDocumentOutputTypeDef],  # (2)
    ssmDocumentType: NotRequired[SsmDocumentTypeType],  # (3)
```

1. See [:material-code-brackets: PostLaunchActionExecutionStatusType](./literals.md#postlaunchactionexecutionstatustype) 
2. See [:material-code-braces: SsmDocumentOutputTypeDef](./type_defs.md#ssmdocumentoutputtypedef) 
3. See [:material-code-brackets: SsmDocumentTypeType](./literals.md#ssmdocumenttypetype) 
## PostLaunchActionsOutputTypeDef

```python
# PostLaunchActionsOutputTypeDef definition

class PostLaunchActionsOutputTypeDef(TypedDict):
    cloudWatchLogGroupName: NotRequired[str],
    deployment: NotRequired[PostLaunchActionsDeploymentTypeType],  # (1)
    s3LogBucket: NotRequired[str],
    s3OutputKeyPrefix: NotRequired[str],
    ssmDocuments: NotRequired[List[SsmDocumentOutputTypeDef]],  # (2)
```

1. See [:material-code-brackets: PostLaunchActionsDeploymentTypeType](./literals.md#postlaunchactionsdeploymenttypetype) 
2. See [:material-code-braces: SsmDocumentOutputTypeDef](./type_defs.md#ssmdocumentoutputtypedef) 
## ListTemplateActionsResponseTypeDef

```python
# ListTemplateActionsResponseTypeDef definition

class ListTemplateActionsResponseTypeDef(TypedDict):
    items: List[TemplateActionDocumentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TemplateActionDocumentTypeDef](./type_defs.md#templateactiondocumenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWavesResponseTypeDef

```python
# ListWavesResponseTypeDef definition

class ListWavesResponseTypeDef(TypedDict):
    items: List[WaveTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WaveTypeDef](./type_defs.md#wavetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListImportsResponseTypeDef

```python
# ListImportsResponseTypeDef definition

class ListImportsResponseTypeDef(TypedDict):
    items: List[ImportTaskTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ImportTaskTypeDef](./type_defs.md#importtasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartImportResponseTypeDef

```python
# StartImportResponseTypeDef definition

class StartImportResponseTypeDef(TypedDict):
    importTask: ImportTaskTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImportTaskTypeDef](./type_defs.md#importtasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SourceServerResponseTypeDef

```python
# SourceServerResponseTypeDef definition

class SourceServerResponseTypeDef(TypedDict):
    applicationID: str,
    arn: str,
    connectorAction: SourceServerConnectorActionTypeDef,  # (1)
    dataReplicationInfo: DataReplicationInfoTypeDef,  # (2)
    fqdnForActionFramework: str,
    isArchived: bool,
    launchedInstance: LaunchedInstanceTypeDef,  # (3)
    lifeCycle: LifeCycleTypeDef,  # (4)
    replicationType: ReplicationTypeType,  # (5)
    sourceProperties: SourcePropertiesTypeDef,  # (6)
    sourceServerID: str,
    tags: Dict[str, str],
    userProvidedID: str,
    vcenterClientID: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-braces: SourceServerConnectorActionTypeDef](./type_defs.md#sourceserverconnectoractiontypedef) 
2. See [:material-code-braces: DataReplicationInfoTypeDef](./type_defs.md#datareplicationinfotypedef) 
3. See [:material-code-braces: LaunchedInstanceTypeDef](./type_defs.md#launchedinstancetypedef) 
4. See [:material-code-braces: LifeCycleTypeDef](./type_defs.md#lifecycletypedef) 
5. See [:material-code-brackets: ReplicationTypeType](./literals.md#replicationtypetype) 
6. See [:material-code-braces: SourcePropertiesTypeDef](./type_defs.md#sourcepropertiestypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SourceServerTypeDef

```python
# SourceServerTypeDef definition

class SourceServerTypeDef(TypedDict):
    applicationID: NotRequired[str],
    arn: NotRequired[str],
    connectorAction: NotRequired[SourceServerConnectorActionTypeDef],  # (1)
    dataReplicationInfo: NotRequired[DataReplicationInfoTypeDef],  # (2)
    fqdnForActionFramework: NotRequired[str],
    isArchived: NotRequired[bool],
    launchedInstance: NotRequired[LaunchedInstanceTypeDef],  # (3)
    lifeCycle: NotRequired[LifeCycleTypeDef],  # (4)
    replicationType: NotRequired[ReplicationTypeType],  # (5)
    sourceProperties: NotRequired[SourcePropertiesTypeDef],  # (6)
    sourceServerID: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    userProvidedID: NotRequired[str],
    vcenterClientID: NotRequired[str],
```

1. See [:material-code-braces: SourceServerConnectorActionTypeDef](./type_defs.md#sourceserverconnectoractiontypedef) 
2. See [:material-code-braces: DataReplicationInfoTypeDef](./type_defs.md#datareplicationinfotypedef) 
3. See [:material-code-braces: LaunchedInstanceTypeDef](./type_defs.md#launchedinstancetypedef) 
4. See [:material-code-braces: LifeCycleTypeDef](./type_defs.md#lifecycletypedef) 
5. See [:material-code-brackets: ReplicationTypeType](./literals.md#replicationtypetype) 
6. See [:material-code-braces: SourcePropertiesTypeDef](./type_defs.md#sourcepropertiestypedef) 
## PostLaunchActionsStatusTypeDef

```python
# PostLaunchActionsStatusTypeDef definition

class PostLaunchActionsStatusTypeDef(TypedDict):
    postLaunchActionsLaunchStatusList: NotRequired[List[JobPostLaunchActionsLaunchStatusTypeDef]],  # (1)
    ssmAgentDiscoveryDatetime: NotRequired[str],
```

1. See [:material-code-braces: JobPostLaunchActionsLaunchStatusTypeDef](./type_defs.md#jobpostlaunchactionslaunchstatustypedef) 
## LaunchConfigurationTemplateResponseTypeDef

```python
# LaunchConfigurationTemplateResponseTypeDef definition

class LaunchConfigurationTemplateResponseTypeDef(TypedDict):
    arn: str,
    associatePublicIpAddress: bool,
    bootMode: BootModeType,  # (1)
    copyPrivateIp: bool,
    copyTags: bool,
    ec2LaunchTemplateID: str,
    enableMapAutoTagging: bool,
    largeVolumeConf: LaunchTemplateDiskConfTypeDef,  # (2)
    launchConfigurationTemplateID: str,
    launchDisposition: LaunchDispositionType,  # (3)
    licensing: LicensingTypeDef,  # (4)
    mapAutoTaggingMpeID: str,
    postLaunchActions: PostLaunchActionsOutputTypeDef,  # (5)
    smallVolumeConf: LaunchTemplateDiskConfTypeDef,  # (2)
    smallVolumeMaxSize: int,
    tags: Dict[str, str],
    targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: BootModeType](./literals.md#bootmodetype) 
2. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef) 
3. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype) 
4. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef) 
5. See [:material-code-braces: PostLaunchActionsOutputTypeDef](./type_defs.md#postlaunchactionsoutputtypedef) 
6. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef) 
7. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LaunchConfigurationTemplateTypeDef

```python
# LaunchConfigurationTemplateTypeDef definition

class LaunchConfigurationTemplateTypeDef(TypedDict):
    launchConfigurationTemplateID: str,
    arn: NotRequired[str],
    associatePublicIpAddress: NotRequired[bool],
    bootMode: NotRequired[BootModeType],  # (1)
    copyPrivateIp: NotRequired[bool],
    copyTags: NotRequired[bool],
    ec2LaunchTemplateID: NotRequired[str],
    enableMapAutoTagging: NotRequired[bool],
    largeVolumeConf: NotRequired[LaunchTemplateDiskConfTypeDef],  # (2)
    launchDisposition: NotRequired[LaunchDispositionType],  # (3)
    licensing: NotRequired[LicensingTypeDef],  # (4)
    mapAutoTaggingMpeID: NotRequired[str],
    postLaunchActions: NotRequired[PostLaunchActionsOutputTypeDef],  # (5)
    smallVolumeConf: NotRequired[LaunchTemplateDiskConfTypeDef],  # (2)
    smallVolumeMaxSize: NotRequired[int],
    tags: NotRequired[Dict[str, str]],
    targetInstanceTypeRightSizingMethod: NotRequired[TargetInstanceTypeRightSizingMethodType],  # (7)
```

1. See [:material-code-brackets: BootModeType](./literals.md#bootmodetype) 
2. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef) 
3. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype) 
4. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef) 
5. See [:material-code-braces: PostLaunchActionsOutputTypeDef](./type_defs.md#postlaunchactionsoutputtypedef) 
6. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef) 
7. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype) 
## LaunchConfigurationTypeDef

```python
# LaunchConfigurationTypeDef definition

class LaunchConfigurationTypeDef(TypedDict):
    bootMode: BootModeType,  # (1)
    copyPrivateIp: bool,
    copyTags: bool,
    ec2LaunchTemplateID: str,
    enableMapAutoTagging: bool,
    launchDisposition: LaunchDispositionType,  # (2)
    licensing: LicensingTypeDef,  # (3)
    mapAutoTaggingMpeID: str,
    name: str,
    postLaunchActions: PostLaunchActionsOutputTypeDef,  # (4)
    sourceServerID: str,
    targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: BootModeType](./literals.md#bootmodetype) 
2. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype) 
3. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef) 
4. See [:material-code-braces: PostLaunchActionsOutputTypeDef](./type_defs.md#postlaunchactionsoutputtypedef) 
5. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PostLaunchActionsTypeDef

```python
# PostLaunchActionsTypeDef definition

class PostLaunchActionsTypeDef(TypedDict):
    cloudWatchLogGroupName: NotRequired[str],
    deployment: NotRequired[PostLaunchActionsDeploymentTypeType],  # (1)
    s3LogBucket: NotRequired[str],
    s3OutputKeyPrefix: NotRequired[str],
    ssmDocuments: NotRequired[Sequence[SsmDocumentUnionTypeDef]],  # (2)
```

1. See [:material-code-brackets: PostLaunchActionsDeploymentTypeType](./literals.md#postlaunchactionsdeploymenttypetype) 
2. See [:material-code-braces: SsmDocumentTypeDef](./type_defs.md#ssmdocumenttypedef) [:material-code-braces: SsmDocumentOutputTypeDef](./type_defs.md#ssmdocumentoutputtypedef) 
## DescribeSourceServersResponseTypeDef

```python
# DescribeSourceServersResponseTypeDef definition

class DescribeSourceServersResponseTypeDef(TypedDict):
    items: List[SourceServerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SourceServerTypeDef](./type_defs.md#sourceservertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ParticipatingServerTypeDef

```python
# ParticipatingServerTypeDef definition

class ParticipatingServerTypeDef(TypedDict):
    sourceServerID: str,
    launchStatus: NotRequired[LaunchStatusType],  # (1)
    launchedEc2InstanceID: NotRequired[str],
    postLaunchActionsStatus: NotRequired[PostLaunchActionsStatusTypeDef],  # (2)
```

1. See [:material-code-brackets: LaunchStatusType](./literals.md#launchstatustype) 
2. See [:material-code-braces: PostLaunchActionsStatusTypeDef](./type_defs.md#postlaunchactionsstatustypedef) 
## DescribeLaunchConfigurationTemplatesResponseTypeDef

```python
# DescribeLaunchConfigurationTemplatesResponseTypeDef definition

class DescribeLaunchConfigurationTemplatesResponseTypeDef(TypedDict):
    items: List[LaunchConfigurationTemplateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LaunchConfigurationTemplateTypeDef](./type_defs.md#launchconfigurationtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLaunchConfigurationTemplateRequestRequestTypeDef

```python
# CreateLaunchConfigurationTemplateRequestRequestTypeDef definition

class CreateLaunchConfigurationTemplateRequestRequestTypeDef(TypedDict):
    associatePublicIpAddress: NotRequired[bool],
    bootMode: NotRequired[BootModeType],  # (1)
    copyPrivateIp: NotRequired[bool],
    copyTags: NotRequired[bool],
    enableMapAutoTagging: NotRequired[bool],
    largeVolumeConf: NotRequired[LaunchTemplateDiskConfTypeDef],  # (2)
    launchDisposition: NotRequired[LaunchDispositionType],  # (3)
    licensing: NotRequired[LicensingTypeDef],  # (4)
    mapAutoTaggingMpeID: NotRequired[str],
    postLaunchActions: NotRequired[PostLaunchActionsTypeDef],  # (5)
    smallVolumeConf: NotRequired[LaunchTemplateDiskConfTypeDef],  # (2)
    smallVolumeMaxSize: NotRequired[int],
    tags: NotRequired[Mapping[str, str]],
    targetInstanceTypeRightSizingMethod: NotRequired[TargetInstanceTypeRightSizingMethodType],  # (7)
```

1. See [:material-code-brackets: BootModeType](./literals.md#bootmodetype) 
2. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef) 
3. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype) 
4. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef) 
5. See [:material-code-braces: PostLaunchActionsTypeDef](./type_defs.md#postlaunchactionstypedef) 
6. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef) 
7. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype) 
## UpdateLaunchConfigurationRequestRequestTypeDef

```python
# UpdateLaunchConfigurationRequestRequestTypeDef definition

class UpdateLaunchConfigurationRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
    bootMode: NotRequired[BootModeType],  # (1)
    copyPrivateIp: NotRequired[bool],
    copyTags: NotRequired[bool],
    enableMapAutoTagging: NotRequired[bool],
    launchDisposition: NotRequired[LaunchDispositionType],  # (2)
    licensing: NotRequired[LicensingTypeDef],  # (3)
    mapAutoTaggingMpeID: NotRequired[str],
    name: NotRequired[str],
    postLaunchActions: NotRequired[PostLaunchActionsTypeDef],  # (4)
    targetInstanceTypeRightSizingMethod: NotRequired[TargetInstanceTypeRightSizingMethodType],  # (5)
```

1. See [:material-code-brackets: BootModeType](./literals.md#bootmodetype) 
2. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype) 
3. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef) 
4. See [:material-code-braces: PostLaunchActionsTypeDef](./type_defs.md#postlaunchactionstypedef) 
5. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype) 
## UpdateLaunchConfigurationTemplateRequestRequestTypeDef

```python
# UpdateLaunchConfigurationTemplateRequestRequestTypeDef definition

class UpdateLaunchConfigurationTemplateRequestRequestTypeDef(TypedDict):
    launchConfigurationTemplateID: str,
    associatePublicIpAddress: NotRequired[bool],
    bootMode: NotRequired[BootModeType],  # (1)
    copyPrivateIp: NotRequired[bool],
    copyTags: NotRequired[bool],
    enableMapAutoTagging: NotRequired[bool],
    largeVolumeConf: NotRequired[LaunchTemplateDiskConfTypeDef],  # (2)
    launchDisposition: NotRequired[LaunchDispositionType],  # (3)
    licensing: NotRequired[LicensingTypeDef],  # (4)
    mapAutoTaggingMpeID: NotRequired[str],
    postLaunchActions: NotRequired[PostLaunchActionsTypeDef],  # (5)
    smallVolumeConf: NotRequired[LaunchTemplateDiskConfTypeDef],  # (2)
    smallVolumeMaxSize: NotRequired[int],
    targetInstanceTypeRightSizingMethod: NotRequired[TargetInstanceTypeRightSizingMethodType],  # (7)
```

1. See [:material-code-brackets: BootModeType](./literals.md#bootmodetype) 
2. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef) 
3. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype) 
4. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef) 
5. See [:material-code-braces: PostLaunchActionsTypeDef](./type_defs.md#postlaunchactionstypedef) 
6. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef) 
7. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype) 
## JobTypeDef

```python
# JobTypeDef definition

class JobTypeDef(TypedDict):
    jobID: str,
    arn: NotRequired[str],
    creationDateTime: NotRequired[str],
    endDateTime: NotRequired[str],
    initiatedBy: NotRequired[InitiatedByType],  # (1)
    participatingServers: NotRequired[List[ParticipatingServerTypeDef]],  # (2)
    status: NotRequired[JobStatusType],  # (3)
    tags: NotRequired[Dict[str, str]],
    type: NotRequired[JobTypeType],  # (4)
```

1. See [:material-code-brackets: InitiatedByType](./literals.md#initiatedbytype) 
2. See [:material-code-braces: ParticipatingServerTypeDef](./type_defs.md#participatingservertypedef) 
3. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
4. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
## DescribeJobsResponseTypeDef

```python
# DescribeJobsResponseTypeDef definition

class DescribeJobsResponseTypeDef(TypedDict):
    items: List[JobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartCutoverResponseTypeDef

```python
# StartCutoverResponseTypeDef definition

class StartCutoverResponseTypeDef(TypedDict):
    job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTestResponseTypeDef

```python
# StartTestResponseTypeDef definition

class StartTestResponseTypeDef(TypedDict):
    job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TerminateTargetInstancesResponseTypeDef

```python
# TerminateTargetInstancesResponseTypeDef definition

class TerminateTargetInstancesResponseTypeDef(TypedDict):
    job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
