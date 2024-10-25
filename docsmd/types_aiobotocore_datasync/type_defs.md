# Type definitions

> [Index](../README.md) > [DataSync](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [DataSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
    type annotations stubs module [types-aiobotocore-datasync](https://pypi.org/project/types-aiobotocore-datasync/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## CredentialsTypeDef

```python
# CredentialsTypeDef definition

class CredentialsTypeDef(TypedDict):
    Username: str,
    Password: str,
```

## DiscoveryServerConfigurationTypeDef

```python
# DiscoveryServerConfigurationTypeDef definition

class DiscoveryServerConfigurationTypeDef(TypedDict):
    ServerHostname: str,
    ServerPort: NotRequired[int],
```

## TagListEntryTypeDef

```python
# TagListEntryTypeDef definition

class TagListEntryTypeDef(TypedDict):
    Key: str,
    Value: NotRequired[str],
```

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

## PlatformTypeDef

```python
# PlatformTypeDef definition

class PlatformTypeDef(TypedDict):
    Version: NotRequired[str],
```

## AzureBlobSasConfigurationTypeDef

```python
# AzureBlobSasConfigurationTypeDef definition

class AzureBlobSasConfigurationTypeDef(TypedDict):
    Token: str,
```

## CancelTaskExecutionRequestRequestTypeDef

```python
# CancelTaskExecutionRequestRequestTypeDef definition

class CancelTaskExecutionRequestRequestTypeDef(TypedDict):
    TaskExecutionArn: str,
```

## CapacityTypeDef

```python
# CapacityTypeDef definition

class CapacityTypeDef(TypedDict):
    Used: NotRequired[int],
    Provisioned: NotRequired[int],
    LogicalUsed: NotRequired[int],
    ClusterCloudStorageUsed: NotRequired[int],
```

## Ec2ConfigTypeDef

```python
# Ec2ConfigTypeDef definition

class Ec2ConfigTypeDef(TypedDict):
    SubnetArn: str,
    SecurityGroupArns: Sequence[str],
```

## HdfsNameNodeTypeDef

```python
# HdfsNameNodeTypeDef definition

class HdfsNameNodeTypeDef(TypedDict):
    Hostname: str,
    Port: int,
```

## QopConfigurationTypeDef

```python
# QopConfigurationTypeDef definition

class QopConfigurationTypeDef(TypedDict):
    RpcProtection: NotRequired[HdfsRpcProtectionType],  # (1)
    DataTransferProtection: NotRequired[HdfsDataTransferProtectionType],  # (2)
```

1. See [:material-code-brackets: HdfsRpcProtectionType](./literals.md#hdfsrpcprotectiontype) 
2. See [:material-code-brackets: HdfsDataTransferProtectionType](./literals.md#hdfsdatatransferprotectiontype) 
## NfsMountOptionsTypeDef

```python
# NfsMountOptionsTypeDef definition

class NfsMountOptionsTypeDef(TypedDict):
    Version: NotRequired[NfsVersionType],  # (1)
```

1. See [:material-code-brackets: NfsVersionType](./literals.md#nfsversiontype) 
## OnPremConfigTypeDef

```python
# OnPremConfigTypeDef definition

class OnPremConfigTypeDef(TypedDict):
    AgentArns: Sequence[str],
```

## S3ConfigTypeDef

```python
# S3ConfigTypeDef definition

class S3ConfigTypeDef(TypedDict):
    BucketAccessRoleArn: str,
```

## SmbMountOptionsTypeDef

```python
# SmbMountOptionsTypeDef definition

class SmbMountOptionsTypeDef(TypedDict):
    Version: NotRequired[SmbVersionType],  # (1)
```

1. See [:material-code-brackets: SmbVersionType](./literals.md#smbversiontype) 
## FilterRuleTypeDef

```python
# FilterRuleTypeDef definition

class FilterRuleTypeDef(TypedDict):
    FilterType: NotRequired[FilterTypeType],  # (1)
    Value: NotRequired[str],
```

1. See [:material-code-brackets: FilterTypeType](./literals.md#filtertypetype) 
## OptionsTypeDef

```python
# OptionsTypeDef definition

class OptionsTypeDef(TypedDict):
    VerifyMode: NotRequired[VerifyModeType],  # (1)
    OverwriteMode: NotRequired[OverwriteModeType],  # (2)
    Atime: NotRequired[AtimeType],  # (3)
    Mtime: NotRequired[MtimeType],  # (4)
    Uid: NotRequired[UidType],  # (5)
    Gid: NotRequired[GidType],  # (6)
    PreserveDeletedFiles: NotRequired[PreserveDeletedFilesType],  # (7)
    PreserveDevices: NotRequired[PreserveDevicesType],  # (8)
    PosixPermissions: NotRequired[PosixPermissionsType],  # (9)
    BytesPerSecond: NotRequired[int],
    TaskQueueing: NotRequired[TaskQueueingType],  # (10)
    LogLevel: NotRequired[LogLevelType],  # (11)
    TransferMode: NotRequired[TransferModeType],  # (12)
    SecurityDescriptorCopyFlags: NotRequired[SmbSecurityDescriptorCopyFlagsType],  # (13)
    ObjectTags: NotRequired[ObjectTagsType],  # (14)
```

1. See [:material-code-brackets: VerifyModeType](./literals.md#verifymodetype) 
2. See [:material-code-brackets: OverwriteModeType](./literals.md#overwritemodetype) 
3. See [:material-code-brackets: AtimeType](./literals.md#atimetype) 
4. See [:material-code-brackets: MtimeType](./literals.md#mtimetype) 
5. See [:material-code-brackets: UidType](./literals.md#uidtype) 
6. See [:material-code-brackets: GidType](./literals.md#gidtype) 
7. See [:material-code-brackets: PreserveDeletedFilesType](./literals.md#preservedeletedfilestype) 
8. See [:material-code-brackets: PreserveDevicesType](./literals.md#preservedevicestype) 
9. See [:material-code-brackets: PosixPermissionsType](./literals.md#posixpermissionstype) 
10. See [:material-code-brackets: TaskQueueingType](./literals.md#taskqueueingtype) 
11. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
12. See [:material-code-brackets: TransferModeType](./literals.md#transfermodetype) 
13. See [:material-code-brackets: SmbSecurityDescriptorCopyFlagsType](./literals.md#smbsecuritydescriptorcopyflagstype) 
14. See [:material-code-brackets: ObjectTagsType](./literals.md#objecttagstype) 
## TaskScheduleTypeDef

```python
# TaskScheduleTypeDef definition

class TaskScheduleTypeDef(TypedDict):
    ScheduleExpression: str,
    Status: NotRequired[ScheduleStatusType],  # (1)
```

1. See [:material-code-brackets: ScheduleStatusType](./literals.md#schedulestatustype) 
## DeleteAgentRequestRequestTypeDef

```python
# DeleteAgentRequestRequestTypeDef definition

class DeleteAgentRequestRequestTypeDef(TypedDict):
    AgentArn: str,
```

## DeleteLocationRequestRequestTypeDef

```python
# DeleteLocationRequestRequestTypeDef definition

class DeleteLocationRequestRequestTypeDef(TypedDict):
    LocationArn: str,
```

## DeleteTaskRequestRequestTypeDef

```python
# DeleteTaskRequestRequestTypeDef definition

class DeleteTaskRequestRequestTypeDef(TypedDict):
    TaskArn: str,
```

## DescribeAgentRequestRequestTypeDef

```python
# DescribeAgentRequestRequestTypeDef definition

class DescribeAgentRequestRequestTypeDef(TypedDict):
    AgentArn: str,
```

## PrivateLinkConfigTypeDef

```python
# PrivateLinkConfigTypeDef definition

class PrivateLinkConfigTypeDef(TypedDict):
    VpcEndpointId: NotRequired[str],
    PrivateLinkEndpoint: NotRequired[str],
    SubnetArns: NotRequired[List[str]],
    SecurityGroupArns: NotRequired[List[str]],
```

## DescribeDiscoveryJobRequestRequestTypeDef

```python
# DescribeDiscoveryJobRequestRequestTypeDef definition

class DescribeDiscoveryJobRequestRequestTypeDef(TypedDict):
    DiscoveryJobArn: str,
```

## DescribeLocationAzureBlobRequestRequestTypeDef

```python
# DescribeLocationAzureBlobRequestRequestTypeDef definition

class DescribeLocationAzureBlobRequestRequestTypeDef(TypedDict):
    LocationArn: str,
```

## DescribeLocationEfsRequestRequestTypeDef

```python
# DescribeLocationEfsRequestRequestTypeDef definition

class DescribeLocationEfsRequestRequestTypeDef(TypedDict):
    LocationArn: str,
```

## Ec2ConfigOutputTypeDef

```python
# Ec2ConfigOutputTypeDef definition

class Ec2ConfigOutputTypeDef(TypedDict):
    SubnetArn: str,
    SecurityGroupArns: List[str],
```

## DescribeLocationFsxLustreRequestRequestTypeDef

```python
# DescribeLocationFsxLustreRequestRequestTypeDef definition

class DescribeLocationFsxLustreRequestRequestTypeDef(TypedDict):
    LocationArn: str,
```

## DescribeLocationFsxOntapRequestRequestTypeDef

```python
# DescribeLocationFsxOntapRequestRequestTypeDef definition

class DescribeLocationFsxOntapRequestRequestTypeDef(TypedDict):
    LocationArn: str,
```

## DescribeLocationFsxOpenZfsRequestRequestTypeDef

```python
# DescribeLocationFsxOpenZfsRequestRequestTypeDef definition

class DescribeLocationFsxOpenZfsRequestRequestTypeDef(TypedDict):
    LocationArn: str,
```

## DescribeLocationFsxWindowsRequestRequestTypeDef

```python
# DescribeLocationFsxWindowsRequestRequestTypeDef definition

class DescribeLocationFsxWindowsRequestRequestTypeDef(TypedDict):
    LocationArn: str,
```

## DescribeLocationHdfsRequestRequestTypeDef

```python
# DescribeLocationHdfsRequestRequestTypeDef definition

class DescribeLocationHdfsRequestRequestTypeDef(TypedDict):
    LocationArn: str,
```

## DescribeLocationNfsRequestRequestTypeDef

```python
# DescribeLocationNfsRequestRequestTypeDef definition

class DescribeLocationNfsRequestRequestTypeDef(TypedDict):
    LocationArn: str,
```

## OnPremConfigOutputTypeDef

```python
# OnPremConfigOutputTypeDef definition

class OnPremConfigOutputTypeDef(TypedDict):
    AgentArns: List[str],
```

## DescribeLocationObjectStorageRequestRequestTypeDef

```python
# DescribeLocationObjectStorageRequestRequestTypeDef definition

class DescribeLocationObjectStorageRequestRequestTypeDef(TypedDict):
    LocationArn: str,
```

## DescribeLocationS3RequestRequestTypeDef

```python
# DescribeLocationS3RequestRequestTypeDef definition

class DescribeLocationS3RequestRequestTypeDef(TypedDict):
    LocationArn: str,
```

## DescribeLocationSmbRequestRequestTypeDef

```python
# DescribeLocationSmbRequestRequestTypeDef definition

class DescribeLocationSmbRequestRequestTypeDef(TypedDict):
    LocationArn: str,
```

## DescribeStorageSystemRequestRequestTypeDef

```python
# DescribeStorageSystemRequestRequestTypeDef definition

class DescribeStorageSystemRequestRequestTypeDef(TypedDict):
    StorageSystemArn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeStorageSystemResourcesRequestRequestTypeDef

```python
# DescribeStorageSystemResourcesRequestRequestTypeDef definition

class DescribeStorageSystemResourcesRequestRequestTypeDef(TypedDict):
    DiscoveryJobArn: str,
    ResourceType: DiscoveryResourceTypeType,  # (1)
    ResourceIds: NotRequired[Sequence[str]],
    Filter: NotRequired[Mapping[DiscoveryResourceFilterType, Sequence[str]]],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: DiscoveryResourceTypeType](./literals.md#discoveryresourcetypetype) 
2. See [:material-code-brackets: DiscoveryResourceFilterType](./literals.md#discoveryresourcefiltertype) 
## DescribeTaskExecutionRequestRequestTypeDef

```python
# DescribeTaskExecutionRequestRequestTypeDef definition

class DescribeTaskExecutionRequestRequestTypeDef(TypedDict):
    TaskExecutionArn: str,
```

## ReportResultTypeDef

```python
# ReportResultTypeDef definition

class ReportResultTypeDef(TypedDict):
    Status: NotRequired[PhaseStatusType],  # (1)
    ErrorCode: NotRequired[str],
    ErrorDetail: NotRequired[str],
```

1. See [:material-code-brackets: PhaseStatusType](./literals.md#phasestatustype) 
## TaskExecutionResultDetailTypeDef

```python
# TaskExecutionResultDetailTypeDef definition

class TaskExecutionResultDetailTypeDef(TypedDict):
    PrepareDuration: NotRequired[int],
    PrepareStatus: NotRequired[PhaseStatusType],  # (1)
    TotalDuration: NotRequired[int],
    TransferDuration: NotRequired[int],
    TransferStatus: NotRequired[PhaseStatusType],  # (1)
    VerifyDuration: NotRequired[int],
    VerifyStatus: NotRequired[PhaseStatusType],  # (1)
    ErrorCode: NotRequired[str],
    ErrorDetail: NotRequired[str],
```

1. See [:material-code-brackets: PhaseStatusType](./literals.md#phasestatustype) 
2. See [:material-code-brackets: PhaseStatusType](./literals.md#phasestatustype) 
3. See [:material-code-brackets: PhaseStatusType](./literals.md#phasestatustype) 
## DescribeTaskRequestRequestTypeDef

```python
# DescribeTaskRequestRequestTypeDef definition

class DescribeTaskRequestRequestTypeDef(TypedDict):
    TaskArn: str,
```

## TaskScheduleDetailsTypeDef

```python
# TaskScheduleDetailsTypeDef definition

class TaskScheduleDetailsTypeDef(TypedDict):
    StatusUpdateTime: NotRequired[datetime],
    DisabledReason: NotRequired[str],
    DisabledBy: NotRequired[ScheduleDisabledByType],  # (1)
```

1. See [:material-code-brackets: ScheduleDisabledByType](./literals.md#scheduledisabledbytype) 
## DiscoveryJobListEntryTypeDef

```python
# DiscoveryJobListEntryTypeDef definition

class DiscoveryJobListEntryTypeDef(TypedDict):
    DiscoveryJobArn: NotRequired[str],
    Status: NotRequired[DiscoveryJobStatusType],  # (1)
```

1. See [:material-code-brackets: DiscoveryJobStatusType](./literals.md#discoveryjobstatustype) 
## GenerateRecommendationsRequestRequestTypeDef

```python
# GenerateRecommendationsRequestRequestTypeDef definition

class GenerateRecommendationsRequestRequestTypeDef(TypedDict):
    DiscoveryJobArn: str,
    ResourceIds: Sequence[str],
    ResourceType: DiscoveryResourceTypeType,  # (1)
```

1. See [:material-code-brackets: DiscoveryResourceTypeType](./literals.md#discoveryresourcetypetype) 
## IOPSTypeDef

```python
# IOPSTypeDef definition

class IOPSTypeDef(TypedDict):
    Read: NotRequired[float],
    Write: NotRequired[float],
    Other: NotRequired[float],
    Total: NotRequired[float],
```

## LatencyTypeDef

```python
# LatencyTypeDef definition

class LatencyTypeDef(TypedDict):
    Read: NotRequired[float],
    Write: NotRequired[float],
    Other: NotRequired[float],
```

## ListAgentsRequestRequestTypeDef

```python
# ListAgentsRequestRequestTypeDef definition

class ListAgentsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListDiscoveryJobsRequestRequestTypeDef

```python
# ListDiscoveryJobsRequestRequestTypeDef definition

class ListDiscoveryJobsRequestRequestTypeDef(TypedDict):
    StorageSystemArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## LocationFilterTypeDef

```python
# LocationFilterTypeDef definition

class LocationFilterTypeDef(TypedDict):
    Name: LocationFilterNameType,  # (1)
    Values: Sequence[str],
    Operator: OperatorType,  # (2)
```

1. See [:material-code-brackets: LocationFilterNameType](./literals.md#locationfilternametype) 
2. See [:material-code-brackets: OperatorType](./literals.md#operatortype) 
## LocationListEntryTypeDef

```python
# LocationListEntryTypeDef definition

class LocationListEntryTypeDef(TypedDict):
    LocationArn: NotRequired[str],
    LocationUri: NotRequired[str],
```

## ListStorageSystemsRequestRequestTypeDef

```python
# ListStorageSystemsRequestRequestTypeDef definition

class ListStorageSystemsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## StorageSystemListEntryTypeDef

```python
# StorageSystemListEntryTypeDef definition

class StorageSystemListEntryTypeDef(TypedDict):
    StorageSystemArn: NotRequired[str],
    Name: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTaskExecutionsRequestRequestTypeDef

```python
# ListTaskExecutionsRequestRequestTypeDef definition

class ListTaskExecutionsRequestRequestTypeDef(TypedDict):
    TaskArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## TaskExecutionListEntryTypeDef

```python
# TaskExecutionListEntryTypeDef definition

class TaskExecutionListEntryTypeDef(TypedDict):
    TaskExecutionArn: NotRequired[str],
    Status: NotRequired[TaskExecutionStatusType],  # (1)
```

1. See [:material-code-brackets: TaskExecutionStatusType](./literals.md#taskexecutionstatustype) 
## TaskFilterTypeDef

```python
# TaskFilterTypeDef definition

class TaskFilterTypeDef(TypedDict):
    Name: TaskFilterNameType,  # (1)
    Values: Sequence[str],
    Operator: OperatorType,  # (2)
```

1. See [:material-code-brackets: TaskFilterNameType](./literals.md#taskfilternametype) 
2. See [:material-code-brackets: OperatorType](./literals.md#operatortype) 
## TaskListEntryTypeDef

```python
# TaskListEntryTypeDef definition

class TaskListEntryTypeDef(TypedDict):
    TaskArn: NotRequired[str],
    Status: NotRequired[TaskStatusType],  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
## MaxP95PerformanceTypeDef

```python
# MaxP95PerformanceTypeDef definition

class MaxP95PerformanceTypeDef(TypedDict):
    IopsRead: NotRequired[float],
    IopsWrite: NotRequired[float],
    IopsOther: NotRequired[float],
    IopsTotal: NotRequired[float],
    ThroughputRead: NotRequired[float],
    ThroughputWrite: NotRequired[float],
    ThroughputOther: NotRequired[float],
    ThroughputTotal: NotRequired[float],
    LatencyRead: NotRequired[float],
    LatencyWrite: NotRequired[float],
    LatencyOther: NotRequired[float],
```

## RecommendationTypeDef

```python
# RecommendationTypeDef definition

class RecommendationTypeDef(TypedDict):
    StorageType: NotRequired[str],
    StorageConfiguration: NotRequired[Dict[str, str]],
    EstimatedMonthlyStorageCost: NotRequired[str],
```

## ThroughputTypeDef

```python
# ThroughputTypeDef definition

class ThroughputTypeDef(TypedDict):
    Read: NotRequired[float],
    Write: NotRequired[float],
    Other: NotRequired[float],
    Total: NotRequired[float],
```

## RemoveStorageSystemRequestRequestTypeDef

```python
# RemoveStorageSystemRequestRequestTypeDef definition

class RemoveStorageSystemRequestRequestTypeDef(TypedDict):
    StorageSystemArn: str,
```

## ReportDestinationS3TypeDef

```python
# ReportDestinationS3TypeDef definition

class ReportDestinationS3TypeDef(TypedDict):
    S3BucketArn: str,
    BucketAccessRoleArn: str,
    Subdirectory: NotRequired[str],
```

## ReportOverrideTypeDef

```python
# ReportOverrideTypeDef definition

class ReportOverrideTypeDef(TypedDict):
    ReportLevel: NotRequired[ReportLevelType],  # (1)
```

1. See [:material-code-brackets: ReportLevelType](./literals.md#reportleveltype) 
## S3ManifestConfigTypeDef

```python
# S3ManifestConfigTypeDef definition

class S3ManifestConfigTypeDef(TypedDict):
    ManifestObjectPath: str,
    BucketAccessRoleArn: str,
    S3BucketArn: str,
    ManifestObjectVersionId: NotRequired[str],
```

## StopDiscoveryJobRequestRequestTypeDef

```python
# StopDiscoveryJobRequestRequestTypeDef definition

class StopDiscoveryJobRequestRequestTypeDef(TypedDict):
    DiscoveryJobArn: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Keys: Sequence[str],
```

## UpdateAgentRequestRequestTypeDef

```python
# UpdateAgentRequestRequestTypeDef definition

class UpdateAgentRequestRequestTypeDef(TypedDict):
    AgentArn: str,
    Name: NotRequired[str],
```

## UpdateDiscoveryJobRequestRequestTypeDef

```python
# UpdateDiscoveryJobRequestRequestTypeDef definition

class UpdateDiscoveryJobRequestRequestTypeDef(TypedDict):
    DiscoveryJobArn: str,
    CollectionDurationMinutes: int,
```

## UpdateStorageSystemRequestRequestTypeDef

```python
# UpdateStorageSystemRequestRequestTypeDef definition

class UpdateStorageSystemRequestRequestTypeDef(TypedDict):
    StorageSystemArn: str,
    ServerConfiguration: NotRequired[DiscoveryServerConfigurationTypeDef],  # (1)
    AgentArns: NotRequired[Sequence[str]],
    Name: NotRequired[str],
    CloudWatchLogGroupArn: NotRequired[str],
    Credentials: NotRequired[CredentialsTypeDef],  # (2)
```

1. See [:material-code-braces: DiscoveryServerConfigurationTypeDef](./type_defs.md#discoveryserverconfigurationtypedef) 
2. See [:material-code-braces: CredentialsTypeDef](./type_defs.md#credentialstypedef) 
## AddStorageSystemRequestRequestTypeDef

```python
# AddStorageSystemRequestRequestTypeDef definition

class AddStorageSystemRequestRequestTypeDef(TypedDict):
    ServerConfiguration: DiscoveryServerConfigurationTypeDef,  # (1)
    SystemType: DiscoverySystemTypeType,  # (2)
    AgentArns: Sequence[str],
    ClientToken: str,
    Credentials: CredentialsTypeDef,  # (3)
    CloudWatchLogGroupArn: NotRequired[str],
    Tags: NotRequired[Sequence[TagListEntryTypeDef]],  # (4)
    Name: NotRequired[str],
```

1. See [:material-code-braces: DiscoveryServerConfigurationTypeDef](./type_defs.md#discoveryserverconfigurationtypedef) 
2. See [:material-code-brackets: DiscoverySystemTypeType](./literals.md#discoverysystemtypetype) 
3. See [:material-code-braces: CredentialsTypeDef](./type_defs.md#credentialstypedef) 
4. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
## CreateAgentRequestRequestTypeDef

```python
# CreateAgentRequestRequestTypeDef definition

class CreateAgentRequestRequestTypeDef(TypedDict):
    ActivationKey: str,
    AgentName: NotRequired[str],
    Tags: NotRequired[Sequence[TagListEntryTypeDef]],  # (1)
    VpcEndpointId: NotRequired[str],
    SubnetArns: NotRequired[Sequence[str]],
    SecurityGroupArns: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
## CreateLocationFsxLustreRequestRequestTypeDef

```python
# CreateLocationFsxLustreRequestRequestTypeDef definition

class CreateLocationFsxLustreRequestRequestTypeDef(TypedDict):
    FsxFilesystemArn: str,
    SecurityGroupArns: Sequence[str],
    Subdirectory: NotRequired[str],
    Tags: NotRequired[Sequence[TagListEntryTypeDef]],  # (1)
```

1. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
## CreateLocationFsxWindowsRequestRequestTypeDef

```python
# CreateLocationFsxWindowsRequestRequestTypeDef definition

class CreateLocationFsxWindowsRequestRequestTypeDef(TypedDict):
    FsxFilesystemArn: str,
    SecurityGroupArns: Sequence[str],
    User: str,
    Password: str,
    Subdirectory: NotRequired[str],
    Tags: NotRequired[Sequence[TagListEntryTypeDef]],  # (1)
    Domain: NotRequired[str],
```

1. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
## StartDiscoveryJobRequestRequestTypeDef

```python
# StartDiscoveryJobRequestRequestTypeDef definition

class StartDiscoveryJobRequestRequestTypeDef(TypedDict):
    StorageSystemArn: str,
    CollectionDurationMinutes: int,
    ClientToken: str,
    Tags: NotRequired[Sequence[TagListEntryTypeDef]],  # (1)
```

1. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagListEntryTypeDef],  # (1)
```

1. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
## AddStorageSystemResponseTypeDef

```python
# AddStorageSystemResponseTypeDef definition

class AddStorageSystemResponseTypeDef(TypedDict):
    StorageSystemArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAgentResponseTypeDef

```python
# CreateAgentResponseTypeDef definition

class CreateAgentResponseTypeDef(TypedDict):
    AgentArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLocationAzureBlobResponseTypeDef

```python
# CreateLocationAzureBlobResponseTypeDef definition

class CreateLocationAzureBlobResponseTypeDef(TypedDict):
    LocationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLocationEfsResponseTypeDef

```python
# CreateLocationEfsResponseTypeDef definition

class CreateLocationEfsResponseTypeDef(TypedDict):
    LocationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLocationFsxLustreResponseTypeDef

```python
# CreateLocationFsxLustreResponseTypeDef definition

class CreateLocationFsxLustreResponseTypeDef(TypedDict):
    LocationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLocationFsxOntapResponseTypeDef

```python
# CreateLocationFsxOntapResponseTypeDef definition

class CreateLocationFsxOntapResponseTypeDef(TypedDict):
    LocationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLocationFsxOpenZfsResponseTypeDef

```python
# CreateLocationFsxOpenZfsResponseTypeDef definition

class CreateLocationFsxOpenZfsResponseTypeDef(TypedDict):
    LocationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLocationFsxWindowsResponseTypeDef

```python
# CreateLocationFsxWindowsResponseTypeDef definition

class CreateLocationFsxWindowsResponseTypeDef(TypedDict):
    LocationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLocationHdfsResponseTypeDef

```python
# CreateLocationHdfsResponseTypeDef definition

class CreateLocationHdfsResponseTypeDef(TypedDict):
    LocationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLocationNfsResponseTypeDef

```python
# CreateLocationNfsResponseTypeDef definition

class CreateLocationNfsResponseTypeDef(TypedDict):
    LocationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLocationObjectStorageResponseTypeDef

```python
# CreateLocationObjectStorageResponseTypeDef definition

class CreateLocationObjectStorageResponseTypeDef(TypedDict):
    LocationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLocationS3ResponseTypeDef

```python
# CreateLocationS3ResponseTypeDef definition

class CreateLocationS3ResponseTypeDef(TypedDict):
    LocationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLocationSmbResponseTypeDef

```python
# CreateLocationSmbResponseTypeDef definition

class CreateLocationSmbResponseTypeDef(TypedDict):
    LocationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTaskResponseTypeDef

```python
# CreateTaskResponseTypeDef definition

class CreateTaskResponseTypeDef(TypedDict):
    TaskArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDiscoveryJobResponseTypeDef

```python
# DescribeDiscoveryJobResponseTypeDef definition

class DescribeDiscoveryJobResponseTypeDef(TypedDict):
    StorageSystemArn: str,
    DiscoveryJobArn: str,
    CollectionDurationMinutes: int,
    Status: DiscoveryJobStatusType,  # (1)
    JobStartTime: datetime,
    JobEndTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DiscoveryJobStatusType](./literals.md#discoveryjobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLocationAzureBlobResponseTypeDef

```python
# DescribeLocationAzureBlobResponseTypeDef definition

class DescribeLocationAzureBlobResponseTypeDef(TypedDict):
    LocationArn: str,
    LocationUri: str,
    AuthenticationType: AzureBlobAuthenticationTypeType,  # (1)
    BlobType: AzureBlobTypeType,  # (2)
    AccessTier: AzureAccessTierType,  # (3)
    AgentArns: List[str],
    CreationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: AzureBlobAuthenticationTypeType](./literals.md#azureblobauthenticationtypetype) 
2. See [:material-code-brackets: AzureBlobTypeType](./literals.md#azureblobtypetype) 
3. See [:material-code-brackets: AzureAccessTierType](./literals.md#azureaccesstiertype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLocationFsxLustreResponseTypeDef

```python
# DescribeLocationFsxLustreResponseTypeDef definition

class DescribeLocationFsxLustreResponseTypeDef(TypedDict):
    LocationArn: str,
    LocationUri: str,
    SecurityGroupArns: List[str],
    CreationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLocationFsxWindowsResponseTypeDef

```python
# DescribeLocationFsxWindowsResponseTypeDef definition

class DescribeLocationFsxWindowsResponseTypeDef(TypedDict):
    LocationArn: str,
    LocationUri: str,
    SecurityGroupArns: List[str],
    CreationTime: datetime,
    User: str,
    Domain: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLocationObjectStorageResponseTypeDef

```python
# DescribeLocationObjectStorageResponseTypeDef definition

class DescribeLocationObjectStorageResponseTypeDef(TypedDict):
    LocationArn: str,
    LocationUri: str,
    AccessKey: str,
    ServerPort: int,
    ServerProtocol: ObjectStorageServerProtocolType,  # (1)
    AgentArns: List[str],
    CreationTime: datetime,
    ServerCertificate: bytes,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ObjectStorageServerProtocolType](./literals.md#objectstorageserverprotocoltype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeStorageSystemResponseTypeDef

```python
# DescribeStorageSystemResponseTypeDef definition

class DescribeStorageSystemResponseTypeDef(TypedDict):
    StorageSystemArn: str,
    ServerConfiguration: DiscoveryServerConfigurationTypeDef,  # (1)
    SystemType: DiscoverySystemTypeType,  # (2)
    AgentArns: List[str],
    Name: str,
    ErrorMessage: str,
    ConnectivityStatus: StorageSystemConnectivityStatusType,  # (3)
    CloudWatchLogGroupArn: str,
    CreationTime: datetime,
    SecretsManagerArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: DiscoveryServerConfigurationTypeDef](./type_defs.md#discoveryserverconfigurationtypedef) 
2. See [:material-code-brackets: DiscoverySystemTypeType](./literals.md#discoverysystemtypetype) 
3. See [:material-code-brackets: StorageSystemConnectivityStatusType](./literals.md#storagesystemconnectivitystatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagListEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDiscoveryJobResponseTypeDef

```python
# StartDiscoveryJobResponseTypeDef definition

class StartDiscoveryJobResponseTypeDef(TypedDict):
    DiscoveryJobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTaskExecutionResponseTypeDef

```python
# StartTaskExecutionResponseTypeDef definition

class StartTaskExecutionResponseTypeDef(TypedDict):
    TaskExecutionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AgentListEntryTypeDef

```python
# AgentListEntryTypeDef definition

class AgentListEntryTypeDef(TypedDict):
    AgentArn: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[AgentStatusType],  # (1)
    Platform: NotRequired[PlatformTypeDef],  # (2)
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype) 
2. See [:material-code-braces: PlatformTypeDef](./type_defs.md#platformtypedef) 
## CreateLocationAzureBlobRequestRequestTypeDef

```python
# CreateLocationAzureBlobRequestRequestTypeDef definition

class CreateLocationAzureBlobRequestRequestTypeDef(TypedDict):
    ContainerUrl: str,
    AuthenticationType: AzureBlobAuthenticationTypeType,  # (1)
    AgentArns: Sequence[str],
    SasConfiguration: NotRequired[AzureBlobSasConfigurationTypeDef],  # (2)
    BlobType: NotRequired[AzureBlobTypeType],  # (3)
    AccessTier: NotRequired[AzureAccessTierType],  # (4)
    Subdirectory: NotRequired[str],
    Tags: NotRequired[Sequence[TagListEntryTypeDef]],  # (5)
```

1. See [:material-code-brackets: AzureBlobAuthenticationTypeType](./literals.md#azureblobauthenticationtypetype) 
2. See [:material-code-braces: AzureBlobSasConfigurationTypeDef](./type_defs.md#azureblobsasconfigurationtypedef) 
3. See [:material-code-brackets: AzureBlobTypeType](./literals.md#azureblobtypetype) 
4. See [:material-code-brackets: AzureAccessTierType](./literals.md#azureaccesstiertype) 
5. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
## UpdateLocationAzureBlobRequestRequestTypeDef

```python
# UpdateLocationAzureBlobRequestRequestTypeDef definition

class UpdateLocationAzureBlobRequestRequestTypeDef(TypedDict):
    LocationArn: str,
    Subdirectory: NotRequired[str],
    AuthenticationType: NotRequired[AzureBlobAuthenticationTypeType],  # (1)
    SasConfiguration: NotRequired[AzureBlobSasConfigurationTypeDef],  # (2)
    BlobType: NotRequired[AzureBlobTypeType],  # (3)
    AccessTier: NotRequired[AzureAccessTierType],  # (4)
    AgentArns: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: AzureBlobAuthenticationTypeType](./literals.md#azureblobauthenticationtypetype) 
2. See [:material-code-braces: AzureBlobSasConfigurationTypeDef](./type_defs.md#azureblobsasconfigurationtypedef) 
3. See [:material-code-brackets: AzureBlobTypeType](./literals.md#azureblobtypetype) 
4. See [:material-code-brackets: AzureAccessTierType](./literals.md#azureaccesstiertype) 
## CreateLocationObjectStorageRequestRequestTypeDef

```python
# CreateLocationObjectStorageRequestRequestTypeDef definition

class CreateLocationObjectStorageRequestRequestTypeDef(TypedDict):
    ServerHostname: str,
    BucketName: str,
    AgentArns: Sequence[str],
    ServerPort: NotRequired[int],
    ServerProtocol: NotRequired[ObjectStorageServerProtocolType],  # (1)
    Subdirectory: NotRequired[str],
    AccessKey: NotRequired[str],
    SecretKey: NotRequired[str],
    Tags: NotRequired[Sequence[TagListEntryTypeDef]],  # (2)
    ServerCertificate: NotRequired[BlobTypeDef],
```

1. See [:material-code-brackets: ObjectStorageServerProtocolType](./literals.md#objectstorageserverprotocoltype) 
2. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
## UpdateLocationObjectStorageRequestRequestTypeDef

```python
# UpdateLocationObjectStorageRequestRequestTypeDef definition

class UpdateLocationObjectStorageRequestRequestTypeDef(TypedDict):
    LocationArn: str,
    ServerPort: NotRequired[int],
    ServerProtocol: NotRequired[ObjectStorageServerProtocolType],  # (1)
    Subdirectory: NotRequired[str],
    AccessKey: NotRequired[str],
    SecretKey: NotRequired[str],
    AgentArns: NotRequired[Sequence[str]],
    ServerCertificate: NotRequired[BlobTypeDef],
```

1. See [:material-code-brackets: ObjectStorageServerProtocolType](./literals.md#objectstorageserverprotocoltype) 
## CreateLocationEfsRequestRequestTypeDef

```python
# CreateLocationEfsRequestRequestTypeDef definition

class CreateLocationEfsRequestRequestTypeDef(TypedDict):
    EfsFilesystemArn: str,
    Ec2Config: Ec2ConfigTypeDef,  # (1)
    Subdirectory: NotRequired[str],
    Tags: NotRequired[Sequence[TagListEntryTypeDef]],  # (2)
    AccessPointArn: NotRequired[str],
    FileSystemAccessRoleArn: NotRequired[str],
    InTransitEncryption: NotRequired[EfsInTransitEncryptionType],  # (3)
```

1. See [:material-code-braces: Ec2ConfigTypeDef](./type_defs.md#ec2configtypedef) 
2. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
3. See [:material-code-brackets: EfsInTransitEncryptionType](./literals.md#efsintransitencryptiontype) 
## CreateLocationHdfsRequestRequestTypeDef

```python
# CreateLocationHdfsRequestRequestTypeDef definition

class CreateLocationHdfsRequestRequestTypeDef(TypedDict):
    NameNodes: Sequence[HdfsNameNodeTypeDef],  # (1)
    AuthenticationType: HdfsAuthenticationTypeType,  # (2)
    AgentArns: Sequence[str],
    Subdirectory: NotRequired[str],
    BlockSize: NotRequired[int],
    ReplicationFactor: NotRequired[int],
    KmsKeyProviderUri: NotRequired[str],
    QopConfiguration: NotRequired[QopConfigurationTypeDef],  # (3)
    SimpleUser: NotRequired[str],
    KerberosPrincipal: NotRequired[str],
    KerberosKeytab: NotRequired[BlobTypeDef],
    KerberosKrb5Conf: NotRequired[BlobTypeDef],
    Tags: NotRequired[Sequence[TagListEntryTypeDef]],  # (4)
```

1. See [:material-code-braces: HdfsNameNodeTypeDef](./type_defs.md#hdfsnamenodetypedef) 
2. See [:material-code-brackets: HdfsAuthenticationTypeType](./literals.md#hdfsauthenticationtypetype) 
3. See [:material-code-braces: QopConfigurationTypeDef](./type_defs.md#qopconfigurationtypedef) 
4. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
## DescribeLocationHdfsResponseTypeDef

```python
# DescribeLocationHdfsResponseTypeDef definition

class DescribeLocationHdfsResponseTypeDef(TypedDict):
    LocationArn: str,
    LocationUri: str,
    NameNodes: List[HdfsNameNodeTypeDef],  # (1)
    BlockSize: int,
    ReplicationFactor: int,
    KmsKeyProviderUri: str,
    QopConfiguration: QopConfigurationTypeDef,  # (2)
    AuthenticationType: HdfsAuthenticationTypeType,  # (3)
    SimpleUser: str,
    KerberosPrincipal: str,
    AgentArns: List[str],
    CreationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: HdfsNameNodeTypeDef](./type_defs.md#hdfsnamenodetypedef) 
2. See [:material-code-braces: QopConfigurationTypeDef](./type_defs.md#qopconfigurationtypedef) 
3. See [:material-code-brackets: HdfsAuthenticationTypeType](./literals.md#hdfsauthenticationtypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLocationHdfsRequestRequestTypeDef

```python
# UpdateLocationHdfsRequestRequestTypeDef definition

class UpdateLocationHdfsRequestRequestTypeDef(TypedDict):
    LocationArn: str,
    Subdirectory: NotRequired[str],
    NameNodes: NotRequired[Sequence[HdfsNameNodeTypeDef]],  # (1)
    BlockSize: NotRequired[int],
    ReplicationFactor: NotRequired[int],
    KmsKeyProviderUri: NotRequired[str],
    QopConfiguration: NotRequired[QopConfigurationTypeDef],  # (2)
    AuthenticationType: NotRequired[HdfsAuthenticationTypeType],  # (3)
    SimpleUser: NotRequired[str],
    KerberosPrincipal: NotRequired[str],
    KerberosKeytab: NotRequired[BlobTypeDef],
    KerberosKrb5Conf: NotRequired[BlobTypeDef],
    AgentArns: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: HdfsNameNodeTypeDef](./type_defs.md#hdfsnamenodetypedef) 
2. See [:material-code-braces: QopConfigurationTypeDef](./type_defs.md#qopconfigurationtypedef) 
3. See [:material-code-brackets: HdfsAuthenticationTypeType](./literals.md#hdfsauthenticationtypetype) 
## FsxProtocolNfsTypeDef

```python
# FsxProtocolNfsTypeDef definition

class FsxProtocolNfsTypeDef(TypedDict):
    MountOptions: NotRequired[NfsMountOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: NfsMountOptionsTypeDef](./type_defs.md#nfsmountoptionstypedef) 
## CreateLocationNfsRequestRequestTypeDef

```python
# CreateLocationNfsRequestRequestTypeDef definition

class CreateLocationNfsRequestRequestTypeDef(TypedDict):
    Subdirectory: str,
    ServerHostname: str,
    OnPremConfig: OnPremConfigTypeDef,  # (1)
    MountOptions: NotRequired[NfsMountOptionsTypeDef],  # (2)
    Tags: NotRequired[Sequence[TagListEntryTypeDef]],  # (3)
```

1. See [:material-code-braces: OnPremConfigTypeDef](./type_defs.md#onpremconfigtypedef) 
2. See [:material-code-braces: NfsMountOptionsTypeDef](./type_defs.md#nfsmountoptionstypedef) 
3. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
## UpdateLocationNfsRequestRequestTypeDef

```python
# UpdateLocationNfsRequestRequestTypeDef definition

class UpdateLocationNfsRequestRequestTypeDef(TypedDict):
    LocationArn: str,
    Subdirectory: NotRequired[str],
    OnPremConfig: NotRequired[OnPremConfigTypeDef],  # (1)
    MountOptions: NotRequired[NfsMountOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: OnPremConfigTypeDef](./type_defs.md#onpremconfigtypedef) 
2. See [:material-code-braces: NfsMountOptionsTypeDef](./type_defs.md#nfsmountoptionstypedef) 
## CreateLocationS3RequestRequestTypeDef

```python
# CreateLocationS3RequestRequestTypeDef definition

class CreateLocationS3RequestRequestTypeDef(TypedDict):
    S3BucketArn: str,
    S3Config: S3ConfigTypeDef,  # (1)
    Subdirectory: NotRequired[str],
    S3StorageClass: NotRequired[S3StorageClassType],  # (2)
    AgentArns: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagListEntryTypeDef]],  # (3)
```

1. See [:material-code-braces: S3ConfigTypeDef](./type_defs.md#s3configtypedef) 
2. See [:material-code-brackets: S3StorageClassType](./literals.md#s3storageclasstype) 
3. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
## DescribeLocationS3ResponseTypeDef

```python
# DescribeLocationS3ResponseTypeDef definition

class DescribeLocationS3ResponseTypeDef(TypedDict):
    LocationArn: str,
    LocationUri: str,
    S3StorageClass: S3StorageClassType,  # (1)
    S3Config: S3ConfigTypeDef,  # (2)
    AgentArns: List[str],
    CreationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: S3StorageClassType](./literals.md#s3storageclasstype) 
2. See [:material-code-braces: S3ConfigTypeDef](./type_defs.md#s3configtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLocationSmbRequestRequestTypeDef

```python
# CreateLocationSmbRequestRequestTypeDef definition

class CreateLocationSmbRequestRequestTypeDef(TypedDict):
    Subdirectory: str,
    ServerHostname: str,
    User: str,
    Password: str,
    AgentArns: Sequence[str],
    Domain: NotRequired[str],
    MountOptions: NotRequired[SmbMountOptionsTypeDef],  # (1)
    Tags: NotRequired[Sequence[TagListEntryTypeDef]],  # (2)
```

1. See [:material-code-braces: SmbMountOptionsTypeDef](./type_defs.md#smbmountoptionstypedef) 
2. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
## DescribeLocationSmbResponseTypeDef

```python
# DescribeLocationSmbResponseTypeDef definition

class DescribeLocationSmbResponseTypeDef(TypedDict):
    LocationArn: str,
    LocationUri: str,
    AgentArns: List[str],
    User: str,
    Domain: str,
    MountOptions: SmbMountOptionsTypeDef,  # (1)
    CreationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SmbMountOptionsTypeDef](./type_defs.md#smbmountoptionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FsxProtocolSmbTypeDef

```python
# FsxProtocolSmbTypeDef definition

class FsxProtocolSmbTypeDef(TypedDict):
    Password: str,
    User: str,
    Domain: NotRequired[str],
    MountOptions: NotRequired[SmbMountOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: SmbMountOptionsTypeDef](./type_defs.md#smbmountoptionstypedef) 
## UpdateLocationSmbRequestRequestTypeDef

```python
# UpdateLocationSmbRequestRequestTypeDef definition

class UpdateLocationSmbRequestRequestTypeDef(TypedDict):
    LocationArn: str,
    Subdirectory: NotRequired[str],
    User: NotRequired[str],
    Domain: NotRequired[str],
    Password: NotRequired[str],
    AgentArns: NotRequired[Sequence[str]],
    MountOptions: NotRequired[SmbMountOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: SmbMountOptionsTypeDef](./type_defs.md#smbmountoptionstypedef) 
## UpdateTaskExecutionRequestRequestTypeDef

```python
# UpdateTaskExecutionRequestRequestTypeDef definition

class UpdateTaskExecutionRequestRequestTypeDef(TypedDict):
    TaskExecutionArn: str,
    Options: OptionsTypeDef,  # (1)
```

1. See [:material-code-braces: OptionsTypeDef](./type_defs.md#optionstypedef) 
## DescribeAgentResponseTypeDef

```python
# DescribeAgentResponseTypeDef definition

class DescribeAgentResponseTypeDef(TypedDict):
    AgentArn: str,
    Name: str,
    Status: AgentStatusType,  # (1)
    LastConnectionTime: datetime,
    CreationTime: datetime,
    EndpointType: EndpointTypeType,  # (2)
    PrivateLinkConfig: PrivateLinkConfigTypeDef,  # (3)
    Platform: PlatformTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype) 
2. See [:material-code-brackets: EndpointTypeType](./literals.md#endpointtypetype) 
3. See [:material-code-braces: PrivateLinkConfigTypeDef](./type_defs.md#privatelinkconfigtypedef) 
4. See [:material-code-braces: PlatformTypeDef](./type_defs.md#platformtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLocationEfsResponseTypeDef

```python
# DescribeLocationEfsResponseTypeDef definition

class DescribeLocationEfsResponseTypeDef(TypedDict):
    LocationArn: str,
    LocationUri: str,
    Ec2Config: Ec2ConfigOutputTypeDef,  # (1)
    CreationTime: datetime,
    AccessPointArn: str,
    FileSystemAccessRoleArn: str,
    InTransitEncryption: EfsInTransitEncryptionType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: Ec2ConfigOutputTypeDef](./type_defs.md#ec2configoutputtypedef) 
2. See [:material-code-brackets: EfsInTransitEncryptionType](./literals.md#efsintransitencryptiontype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLocationNfsResponseTypeDef

```python
# DescribeLocationNfsResponseTypeDef definition

class DescribeLocationNfsResponseTypeDef(TypedDict):
    LocationArn: str,
    LocationUri: str,
    OnPremConfig: OnPremConfigOutputTypeDef,  # (1)
    MountOptions: NfsMountOptionsTypeDef,  # (2)
    CreationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: OnPremConfigOutputTypeDef](./type_defs.md#onpremconfigoutputtypedef) 
2. See [:material-code-braces: NfsMountOptionsTypeDef](./type_defs.md#nfsmountoptionstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAgentsRequestListAgentsPaginateTypeDef

```python
# ListAgentsRequestListAgentsPaginateTypeDef definition

class ListAgentsRequestListAgentsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef

```python
# ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef definition

class ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef(TypedDict):
    StorageSystemArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStorageSystemsRequestListStorageSystemsPaginateTypeDef

```python
# ListStorageSystemsRequestListStorageSystemsPaginateTypeDef definition

class ListStorageSystemsRequestListStorageSystemsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceRequestListTagsForResourcePaginateTypeDef

```python
# ListTagsForResourceRequestListTagsForResourcePaginateTypeDef definition

class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(TypedDict):
    ResourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef

```python
# ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef definition

class ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef(TypedDict):
    TaskArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef

```python
# DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef definition

class DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef(TypedDict):
    DiscoveryJobArn: str,
    ResourceType: DiscoveryResourceTypeType,  # (1)
    ResourceId: str,
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DiscoveryResourceTypeType](./literals.md#discoveryresourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeStorageSystemResourceMetricsRequestRequestTypeDef

```python
# DescribeStorageSystemResourceMetricsRequestRequestTypeDef definition

class DescribeStorageSystemResourceMetricsRequestRequestTypeDef(TypedDict):
    DiscoveryJobArn: str,
    ResourceType: DiscoveryResourceTypeType,  # (1)
    ResourceId: str,
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: DiscoveryResourceTypeType](./literals.md#discoveryresourcetypetype) 
## ListDiscoveryJobsResponseTypeDef

```python
# ListDiscoveryJobsResponseTypeDef definition

class ListDiscoveryJobsResponseTypeDef(TypedDict):
    DiscoveryJobs: List[DiscoveryJobListEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DiscoveryJobListEntryTypeDef](./type_defs.md#discoveryjoblistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLocationsRequestListLocationsPaginateTypeDef

```python
# ListLocationsRequestListLocationsPaginateTypeDef definition

class ListLocationsRequestListLocationsPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[LocationFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: LocationFilterTypeDef](./type_defs.md#locationfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLocationsRequestRequestTypeDef

```python
# ListLocationsRequestRequestTypeDef definition

class ListLocationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[LocationFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: LocationFilterTypeDef](./type_defs.md#locationfiltertypedef) 
## ListLocationsResponseTypeDef

```python
# ListLocationsResponseTypeDef definition

class ListLocationsResponseTypeDef(TypedDict):
    Locations: List[LocationListEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LocationListEntryTypeDef](./type_defs.md#locationlistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStorageSystemsResponseTypeDef

```python
# ListStorageSystemsResponseTypeDef definition

class ListStorageSystemsResponseTypeDef(TypedDict):
    StorageSystems: List[StorageSystemListEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: StorageSystemListEntryTypeDef](./type_defs.md#storagesystemlistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTaskExecutionsResponseTypeDef

```python
# ListTaskExecutionsResponseTypeDef definition

class ListTaskExecutionsResponseTypeDef(TypedDict):
    TaskExecutions: List[TaskExecutionListEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TaskExecutionListEntryTypeDef](./type_defs.md#taskexecutionlistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTasksRequestListTasksPaginateTypeDef

```python
# ListTasksRequestListTasksPaginateTypeDef definition

class ListTasksRequestListTasksPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[TaskFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: TaskFilterTypeDef](./type_defs.md#taskfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTasksRequestRequestTypeDef

```python
# ListTasksRequestRequestTypeDef definition

class ListTasksRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[TaskFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: TaskFilterTypeDef](./type_defs.md#taskfiltertypedef) 
## ListTasksResponseTypeDef

```python
# ListTasksResponseTypeDef definition

class ListTasksResponseTypeDef(TypedDict):
    Tasks: List[TaskListEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TaskListEntryTypeDef](./type_defs.md#tasklistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NetAppONTAPClusterTypeDef

```python
# NetAppONTAPClusterTypeDef definition

class NetAppONTAPClusterTypeDef(TypedDict):
    CifsShareCount: NotRequired[int],
    NfsExportedVolumes: NotRequired[int],
    ResourceId: NotRequired[str],
    ClusterName: NotRequired[str],
    MaxP95Performance: NotRequired[MaxP95PerformanceTypeDef],  # (1)
    ClusterBlockStorageSize: NotRequired[int],
    ClusterBlockStorageUsed: NotRequired[int],
    ClusterBlockStorageLogicalUsed: NotRequired[int],
    Recommendations: NotRequired[List[RecommendationTypeDef]],  # (2)
    RecommendationStatus: NotRequired[RecommendationStatusType],  # (3)
    LunCount: NotRequired[int],
    ClusterCloudStorageUsed: NotRequired[int],
```

1. See [:material-code-braces: MaxP95PerformanceTypeDef](./type_defs.md#maxp95performancetypedef) 
2. See [:material-code-braces: RecommendationTypeDef](./type_defs.md#recommendationtypedef) 
3. See [:material-code-brackets: RecommendationStatusType](./literals.md#recommendationstatustype) 
## NetAppONTAPSVMTypeDef

```python
# NetAppONTAPSVMTypeDef definition

class NetAppONTAPSVMTypeDef(TypedDict):
    ClusterUuid: NotRequired[str],
    ResourceId: NotRequired[str],
    SvmName: NotRequired[str],
    CifsShareCount: NotRequired[int],
    EnabledProtocols: NotRequired[List[str]],
    TotalCapacityUsed: NotRequired[int],
    TotalCapacityProvisioned: NotRequired[int],
    TotalLogicalCapacityUsed: NotRequired[int],
    MaxP95Performance: NotRequired[MaxP95PerformanceTypeDef],  # (1)
    Recommendations: NotRequired[List[RecommendationTypeDef]],  # (2)
    NfsExportedVolumes: NotRequired[int],
    RecommendationStatus: NotRequired[RecommendationStatusType],  # (3)
    TotalSnapshotCapacityUsed: NotRequired[int],
    LunCount: NotRequired[int],
```

1. See [:material-code-braces: MaxP95PerformanceTypeDef](./type_defs.md#maxp95performancetypedef) 
2. See [:material-code-braces: RecommendationTypeDef](./type_defs.md#recommendationtypedef) 
3. See [:material-code-brackets: RecommendationStatusType](./literals.md#recommendationstatustype) 
## NetAppONTAPVolumeTypeDef

```python
# NetAppONTAPVolumeTypeDef definition

class NetAppONTAPVolumeTypeDef(TypedDict):
    VolumeName: NotRequired[str],
    ResourceId: NotRequired[str],
    CifsShareCount: NotRequired[int],
    SecurityStyle: NotRequired[str],
    SvmUuid: NotRequired[str],
    SvmName: NotRequired[str],
    CapacityUsed: NotRequired[int],
    CapacityProvisioned: NotRequired[int],
    LogicalCapacityUsed: NotRequired[int],
    NfsExported: NotRequired[bool],
    SnapshotCapacityUsed: NotRequired[int],
    MaxP95Performance: NotRequired[MaxP95PerformanceTypeDef],  # (1)
    Recommendations: NotRequired[List[RecommendationTypeDef]],  # (2)
    RecommendationStatus: NotRequired[RecommendationStatusType],  # (3)
    LunCount: NotRequired[int],
```

1. See [:material-code-braces: MaxP95PerformanceTypeDef](./type_defs.md#maxp95performancetypedef) 
2. See [:material-code-braces: RecommendationTypeDef](./type_defs.md#recommendationtypedef) 
3. See [:material-code-brackets: RecommendationStatusType](./literals.md#recommendationstatustype) 
## P95MetricsTypeDef

```python
# P95MetricsTypeDef definition

class P95MetricsTypeDef(TypedDict):
    IOPS: NotRequired[IOPSTypeDef],  # (1)
    Throughput: NotRequired[ThroughputTypeDef],  # (2)
    Latency: NotRequired[LatencyTypeDef],  # (3)
```

1. See [:material-code-braces: IOPSTypeDef](./type_defs.md#iopstypedef) 
2. See [:material-code-braces: ThroughputTypeDef](./type_defs.md#throughputtypedef) 
3. See [:material-code-braces: LatencyTypeDef](./type_defs.md#latencytypedef) 
## ReportDestinationTypeDef

```python
# ReportDestinationTypeDef definition

class ReportDestinationTypeDef(TypedDict):
    S3: NotRequired[ReportDestinationS3TypeDef],  # (1)
```

1. See [:material-code-braces: ReportDestinationS3TypeDef](./type_defs.md#reportdestinations3typedef) 
## ReportOverridesTypeDef

```python
# ReportOverridesTypeDef definition

class ReportOverridesTypeDef(TypedDict):
    Transferred: NotRequired[ReportOverrideTypeDef],  # (1)
    Verified: NotRequired[ReportOverrideTypeDef],  # (1)
    Deleted: NotRequired[ReportOverrideTypeDef],  # (1)
    Skipped: NotRequired[ReportOverrideTypeDef],  # (1)
```

1. See [:material-code-braces: ReportOverrideTypeDef](./type_defs.md#reportoverridetypedef) 
2. See [:material-code-braces: ReportOverrideTypeDef](./type_defs.md#reportoverridetypedef) 
3. See [:material-code-braces: ReportOverrideTypeDef](./type_defs.md#reportoverridetypedef) 
4. See [:material-code-braces: ReportOverrideTypeDef](./type_defs.md#reportoverridetypedef) 
## SourceManifestConfigTypeDef

```python
# SourceManifestConfigTypeDef definition

class SourceManifestConfigTypeDef(TypedDict):
    S3: S3ManifestConfigTypeDef,  # (1)
```

1. See [:material-code-braces: S3ManifestConfigTypeDef](./type_defs.md#s3manifestconfigtypedef) 
## ListAgentsResponseTypeDef

```python
# ListAgentsResponseTypeDef definition

class ListAgentsResponseTypeDef(TypedDict):
    Agents: List[AgentListEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AgentListEntryTypeDef](./type_defs.md#agentlistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FsxProtocolTypeDef

```python
# FsxProtocolTypeDef definition

class FsxProtocolTypeDef(TypedDict):
    NFS: NotRequired[FsxProtocolNfsTypeDef],  # (1)
    SMB: NotRequired[FsxProtocolSmbTypeDef],  # (2)
```

1. See [:material-code-braces: FsxProtocolNfsTypeDef](./type_defs.md#fsxprotocolnfstypedef) 
2. See [:material-code-braces: FsxProtocolSmbTypeDef](./type_defs.md#fsxprotocolsmbtypedef) 
## ResourceDetailsTypeDef

```python
# ResourceDetailsTypeDef definition

class ResourceDetailsTypeDef(TypedDict):
    NetAppONTAPSVMs: NotRequired[List[NetAppONTAPSVMTypeDef]],  # (1)
    NetAppONTAPVolumes: NotRequired[List[NetAppONTAPVolumeTypeDef]],  # (2)
    NetAppONTAPClusters: NotRequired[List[NetAppONTAPClusterTypeDef]],  # (3)
```

1. See [:material-code-braces: NetAppONTAPSVMTypeDef](./type_defs.md#netappontapsvmtypedef) 
2. See [:material-code-braces: NetAppONTAPVolumeTypeDef](./type_defs.md#netappontapvolumetypedef) 
3. See [:material-code-braces: NetAppONTAPClusterTypeDef](./type_defs.md#netappontapclustertypedef) 
## ResourceMetricsTypeDef

```python
# ResourceMetricsTypeDef definition

class ResourceMetricsTypeDef(TypedDict):
    Timestamp: NotRequired[datetime],
    P95Metrics: NotRequired[P95MetricsTypeDef],  # (1)
    Capacity: NotRequired[CapacityTypeDef],  # (2)
    ResourceId: NotRequired[str],
    ResourceType: NotRequired[DiscoveryResourceTypeType],  # (3)
```

1. See [:material-code-braces: P95MetricsTypeDef](./type_defs.md#p95metricstypedef) 
2. See [:material-code-braces: CapacityTypeDef](./type_defs.md#capacitytypedef) 
3. See [:material-code-brackets: DiscoveryResourceTypeType](./literals.md#discoveryresourcetypetype) 
## TaskReportConfigTypeDef

```python
# TaskReportConfigTypeDef definition

class TaskReportConfigTypeDef(TypedDict):
    Destination: NotRequired[ReportDestinationTypeDef],  # (1)
    OutputType: NotRequired[ReportOutputTypeType],  # (2)
    ReportLevel: NotRequired[ReportLevelType],  # (3)
    ObjectVersionIds: NotRequired[ObjectVersionIdsType],  # (4)
    Overrides: NotRequired[ReportOverridesTypeDef],  # (5)
```

1. See [:material-code-braces: ReportDestinationTypeDef](./type_defs.md#reportdestinationtypedef) 
2. See [:material-code-brackets: ReportOutputTypeType](./literals.md#reportoutputtypetype) 
3. See [:material-code-brackets: ReportLevelType](./literals.md#reportleveltype) 
4. See [:material-code-brackets: ObjectVersionIdsType](./literals.md#objectversionidstype) 
5. See [:material-code-braces: ReportOverridesTypeDef](./type_defs.md#reportoverridestypedef) 
## ManifestConfigTypeDef

```python
# ManifestConfigTypeDef definition

class ManifestConfigTypeDef(TypedDict):
    Action: NotRequired[ManifestActionType],  # (1)
    Format: NotRequired[ManifestFormatType],  # (2)
    Source: NotRequired[SourceManifestConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ManifestActionType](./literals.md#manifestactiontype) 
2. See [:material-code-brackets: ManifestFormatType](./literals.md#manifestformattype) 
3. See [:material-code-braces: SourceManifestConfigTypeDef](./type_defs.md#sourcemanifestconfigtypedef) 
## CreateLocationFsxOntapRequestRequestTypeDef

```python
# CreateLocationFsxOntapRequestRequestTypeDef definition

class CreateLocationFsxOntapRequestRequestTypeDef(TypedDict):
    Protocol: FsxProtocolTypeDef,  # (1)
    SecurityGroupArns: Sequence[str],
    StorageVirtualMachineArn: str,
    Subdirectory: NotRequired[str],
    Tags: NotRequired[Sequence[TagListEntryTypeDef]],  # (2)
```

1. See [:material-code-braces: FsxProtocolTypeDef](./type_defs.md#fsxprotocoltypedef) 
2. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
## CreateLocationFsxOpenZfsRequestRequestTypeDef

```python
# CreateLocationFsxOpenZfsRequestRequestTypeDef definition

class CreateLocationFsxOpenZfsRequestRequestTypeDef(TypedDict):
    FsxFilesystemArn: str,
    Protocol: FsxProtocolTypeDef,  # (1)
    SecurityGroupArns: Sequence[str],
    Subdirectory: NotRequired[str],
    Tags: NotRequired[Sequence[TagListEntryTypeDef]],  # (2)
```

1. See [:material-code-braces: FsxProtocolTypeDef](./type_defs.md#fsxprotocoltypedef) 
2. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
## DescribeLocationFsxOntapResponseTypeDef

```python
# DescribeLocationFsxOntapResponseTypeDef definition

class DescribeLocationFsxOntapResponseTypeDef(TypedDict):
    CreationTime: datetime,
    LocationArn: str,
    LocationUri: str,
    Protocol: FsxProtocolTypeDef,  # (1)
    SecurityGroupArns: List[str],
    StorageVirtualMachineArn: str,
    FsxFilesystemArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FsxProtocolTypeDef](./type_defs.md#fsxprotocoltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLocationFsxOpenZfsResponseTypeDef

```python
# DescribeLocationFsxOpenZfsResponseTypeDef definition

class DescribeLocationFsxOpenZfsResponseTypeDef(TypedDict):
    LocationArn: str,
    LocationUri: str,
    SecurityGroupArns: List[str],
    Protocol: FsxProtocolTypeDef,  # (1)
    CreationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FsxProtocolTypeDef](./type_defs.md#fsxprotocoltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeStorageSystemResourcesResponseTypeDef

```python
# DescribeStorageSystemResourcesResponseTypeDef definition

class DescribeStorageSystemResourcesResponseTypeDef(TypedDict):
    ResourceDetails: ResourceDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeStorageSystemResourceMetricsResponseTypeDef

```python
# DescribeStorageSystemResourceMetricsResponseTypeDef definition

class DescribeStorageSystemResourceMetricsResponseTypeDef(TypedDict):
    Metrics: List[ResourceMetricsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceMetricsTypeDef](./type_defs.md#resourcemetricstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTaskRequestRequestTypeDef

```python
# CreateTaskRequestRequestTypeDef definition

class CreateTaskRequestRequestTypeDef(TypedDict):
    SourceLocationArn: str,
    DestinationLocationArn: str,
    CloudWatchLogGroupArn: NotRequired[str],
    Name: NotRequired[str],
    Options: NotRequired[OptionsTypeDef],  # (1)
    Excludes: NotRequired[Sequence[FilterRuleTypeDef]],  # (2)
    Schedule: NotRequired[TaskScheduleTypeDef],  # (3)
    Tags: NotRequired[Sequence[TagListEntryTypeDef]],  # (4)
    Includes: NotRequired[Sequence[FilterRuleTypeDef]],  # (2)
    ManifestConfig: NotRequired[ManifestConfigTypeDef],  # (6)
    TaskReportConfig: NotRequired[TaskReportConfigTypeDef],  # (7)
```

1. See [:material-code-braces: OptionsTypeDef](./type_defs.md#optionstypedef) 
2. See [:material-code-braces: FilterRuleTypeDef](./type_defs.md#filterruletypedef) 
3. See [:material-code-braces: TaskScheduleTypeDef](./type_defs.md#taskscheduletypedef) 
4. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
5. See [:material-code-braces: FilterRuleTypeDef](./type_defs.md#filterruletypedef) 
6. See [:material-code-braces: ManifestConfigTypeDef](./type_defs.md#manifestconfigtypedef) 
7. See [:material-code-braces: TaskReportConfigTypeDef](./type_defs.md#taskreportconfigtypedef) 
## DescribeTaskExecutionResponseTypeDef

```python
# DescribeTaskExecutionResponseTypeDef definition

class DescribeTaskExecutionResponseTypeDef(TypedDict):
    TaskExecutionArn: str,
    Status: TaskExecutionStatusType,  # (1)
    Options: OptionsTypeDef,  # (2)
    Excludes: List[FilterRuleTypeDef],  # (3)
    Includes: List[FilterRuleTypeDef],  # (3)
    ManifestConfig: ManifestConfigTypeDef,  # (5)
    StartTime: datetime,
    EstimatedFilesToTransfer: int,
    EstimatedBytesToTransfer: int,
    FilesTransferred: int,
    BytesWritten: int,
    BytesTransferred: int,
    BytesCompressed: int,
    Result: TaskExecutionResultDetailTypeDef,  # (6)
    TaskReportConfig: TaskReportConfigTypeDef,  # (7)
    FilesDeleted: int,
    FilesSkipped: int,
    FilesVerified: int,
    ReportResult: ReportResultTypeDef,  # (8)
    EstimatedFilesToDelete: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (9)
```

1. See [:material-code-brackets: TaskExecutionStatusType](./literals.md#taskexecutionstatustype) 
2. See [:material-code-braces: OptionsTypeDef](./type_defs.md#optionstypedef) 
3. See [:material-code-braces: FilterRuleTypeDef](./type_defs.md#filterruletypedef) 
4. See [:material-code-braces: FilterRuleTypeDef](./type_defs.md#filterruletypedef) 
5. See [:material-code-braces: ManifestConfigTypeDef](./type_defs.md#manifestconfigtypedef) 
6. See [:material-code-braces: TaskExecutionResultDetailTypeDef](./type_defs.md#taskexecutionresultdetailtypedef) 
7. See [:material-code-braces: TaskReportConfigTypeDef](./type_defs.md#taskreportconfigtypedef) 
8. See [:material-code-braces: ReportResultTypeDef](./type_defs.md#reportresulttypedef) 
9. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTaskResponseTypeDef

```python
# DescribeTaskResponseTypeDef definition

class DescribeTaskResponseTypeDef(TypedDict):
    TaskArn: str,
    Status: TaskStatusType,  # (1)
    Name: str,
    CurrentTaskExecutionArn: str,
    SourceLocationArn: str,
    DestinationLocationArn: str,
    CloudWatchLogGroupArn: str,
    SourceNetworkInterfaceArns: List[str],
    DestinationNetworkInterfaceArns: List[str],
    Options: OptionsTypeDef,  # (2)
    Excludes: List[FilterRuleTypeDef],  # (3)
    Schedule: TaskScheduleTypeDef,  # (4)
    ErrorCode: str,
    ErrorDetail: str,
    CreationTime: datetime,
    Includes: List[FilterRuleTypeDef],  # (3)
    ManifestConfig: ManifestConfigTypeDef,  # (6)
    TaskReportConfig: TaskReportConfigTypeDef,  # (7)
    ScheduleDetails: TaskScheduleDetailsTypeDef,  # (8)
    ResponseMetadata: ResponseMetadataTypeDef,  # (9)
```

1. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
2. See [:material-code-braces: OptionsTypeDef](./type_defs.md#optionstypedef) 
3. See [:material-code-braces: FilterRuleTypeDef](./type_defs.md#filterruletypedef) 
4. See [:material-code-braces: TaskScheduleTypeDef](./type_defs.md#taskscheduletypedef) 
5. See [:material-code-braces: FilterRuleTypeDef](./type_defs.md#filterruletypedef) 
6. See [:material-code-braces: ManifestConfigTypeDef](./type_defs.md#manifestconfigtypedef) 
7. See [:material-code-braces: TaskReportConfigTypeDef](./type_defs.md#taskreportconfigtypedef) 
8. See [:material-code-braces: TaskScheduleDetailsTypeDef](./type_defs.md#taskscheduledetailstypedef) 
9. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTaskExecutionRequestRequestTypeDef

```python
# StartTaskExecutionRequestRequestTypeDef definition

class StartTaskExecutionRequestRequestTypeDef(TypedDict):
    TaskArn: str,
    OverrideOptions: NotRequired[OptionsTypeDef],  # (1)
    Includes: NotRequired[Sequence[FilterRuleTypeDef]],  # (2)
    Excludes: NotRequired[Sequence[FilterRuleTypeDef]],  # (2)
    ManifestConfig: NotRequired[ManifestConfigTypeDef],  # (4)
    TaskReportConfig: NotRequired[TaskReportConfigTypeDef],  # (5)
    Tags: NotRequired[Sequence[TagListEntryTypeDef]],  # (6)
```

1. See [:material-code-braces: OptionsTypeDef](./type_defs.md#optionstypedef) 
2. See [:material-code-braces: FilterRuleTypeDef](./type_defs.md#filterruletypedef) 
3. See [:material-code-braces: FilterRuleTypeDef](./type_defs.md#filterruletypedef) 
4. See [:material-code-braces: ManifestConfigTypeDef](./type_defs.md#manifestconfigtypedef) 
5. See [:material-code-braces: TaskReportConfigTypeDef](./type_defs.md#taskreportconfigtypedef) 
6. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
## UpdateTaskRequestRequestTypeDef

```python
# UpdateTaskRequestRequestTypeDef definition

class UpdateTaskRequestRequestTypeDef(TypedDict):
    TaskArn: str,
    Options: NotRequired[OptionsTypeDef],  # (1)
    Excludes: NotRequired[Sequence[FilterRuleTypeDef]],  # (2)
    Schedule: NotRequired[TaskScheduleTypeDef],  # (3)
    Name: NotRequired[str],
    CloudWatchLogGroupArn: NotRequired[str],
    Includes: NotRequired[Sequence[FilterRuleTypeDef]],  # (2)
    ManifestConfig: NotRequired[ManifestConfigTypeDef],  # (5)
    TaskReportConfig: NotRequired[TaskReportConfigTypeDef],  # (6)
```

1. See [:material-code-braces: OptionsTypeDef](./type_defs.md#optionstypedef) 
2. See [:material-code-braces: FilterRuleTypeDef](./type_defs.md#filterruletypedef) 
3. See [:material-code-braces: TaskScheduleTypeDef](./type_defs.md#taskscheduletypedef) 
4. See [:material-code-braces: FilterRuleTypeDef](./type_defs.md#filterruletypedef) 
5. See [:material-code-braces: ManifestConfigTypeDef](./type_defs.md#manifestconfigtypedef) 
6. See [:material-code-braces: TaskReportConfigTypeDef](./type_defs.md#taskreportconfigtypedef) 
