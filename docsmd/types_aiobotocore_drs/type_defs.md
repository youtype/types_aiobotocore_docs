# Type definitions

> [Index](../README.md) > [Drs](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Drs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#Drs)
    type annotations stubs module [types-aiobotocore-drs](https://pypi.org/project/types-aiobotocore-drs/).



## AccountTypeDef

```python
# AccountTypeDef definition

class AccountTypeDef(TypedDict):
    accountID: NotRequired[str],
```

## AssociateSourceNetworkStackRequestRequestTypeDef

```python
# AssociateSourceNetworkStackRequestRequestTypeDef definition

class AssociateSourceNetworkStackRequestRequestTypeDef(TypedDict):
    cfnStackName: str,
    sourceNetworkID: str,
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

## CPUTypeDef

```python
# CPUTypeDef definition

class CPUTypeDef(TypedDict):
    cores: NotRequired[int],
    modelName: NotRequired[str],
```

## ProductCodeTypeDef

```python
# ProductCodeTypeDef definition

class ProductCodeTypeDef(TypedDict):
    productCodeId: NotRequired[str],
    productCodeMode: NotRequired[ProductCodeModeType],  # (1)
```

1. See [:material-code-brackets: ProductCodeModeType](./literals.md#productcodemodetype) 
## CreateExtendedSourceServerRequestRequestTypeDef

```python
# CreateExtendedSourceServerRequestRequestTypeDef definition

class CreateExtendedSourceServerRequestRequestTypeDef(TypedDict):
    sourceServerArn: str,
    tags: NotRequired[Mapping[str, str]],
```

## LicensingTypeDef

```python
# LicensingTypeDef definition

class LicensingTypeDef(TypedDict):
    osByol: NotRequired[bool],
```

## PITPolicyRuleTypeDef

```python
# PITPolicyRuleTypeDef definition

class PITPolicyRuleTypeDef(TypedDict):
    interval: int,
    retentionDuration: int,
    units: PITPolicyRuleUnitsType,  # (1)
    enabled: NotRequired[bool],
    ruleID: NotRequired[int],
```

1. See [:material-code-brackets: PITPolicyRuleUnitsType](./literals.md#pitpolicyruleunitstype) 
## CreateSourceNetworkRequestRequestTypeDef

```python
# CreateSourceNetworkRequestRequestTypeDef definition

class CreateSourceNetworkRequestRequestTypeDef(TypedDict):
    originAccountID: str,
    originRegion: str,
    vpcID: str,
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
    volumeStatus: NotRequired[VolumeStatusType],  # (1)
```

1. See [:material-code-brackets: VolumeStatusType](./literals.md#volumestatustype) 
## DataReplicationInitiationStepTypeDef

```python
# DataReplicationInitiationStepTypeDef definition

class DataReplicationInitiationStepTypeDef(TypedDict):
    name: NotRequired[DataReplicationInitiationStepNameType],  # (1)
    status: NotRequired[DataReplicationInitiationStepStatusType],  # (2)
```

1. See [:material-code-brackets: DataReplicationInitiationStepNameType](./literals.md#datareplicationinitiationstepnametype) 
2. See [:material-code-brackets: DataReplicationInitiationStepStatusType](./literals.md#datareplicationinitiationstepstatustype) 
## DeleteJobRequestRequestTypeDef

```python
# DeleteJobRequestRequestTypeDef definition

class DeleteJobRequestRequestTypeDef(TypedDict):
    jobID: str,
```

## DeleteLaunchActionRequestRequestTypeDef

```python
# DeleteLaunchActionRequestRequestTypeDef definition

class DeleteLaunchActionRequestRequestTypeDef(TypedDict):
    actionId: str,
    resourceId: str,
```

## DeleteLaunchConfigurationTemplateRequestRequestTypeDef

```python
# DeleteLaunchConfigurationTemplateRequestRequestTypeDef definition

class DeleteLaunchConfigurationTemplateRequestRequestTypeDef(TypedDict):
    launchConfigurationTemplateID: str,
```

## DeleteRecoveryInstanceRequestRequestTypeDef

```python
# DeleteRecoveryInstanceRequestRequestTypeDef definition

class DeleteRecoveryInstanceRequestRequestTypeDef(TypedDict):
    recoveryInstanceID: str,
```

## DeleteReplicationConfigurationTemplateRequestRequestTypeDef

```python
# DeleteReplicationConfigurationTemplateRequestRequestTypeDef definition

class DeleteReplicationConfigurationTemplateRequestRequestTypeDef(TypedDict):
    replicationConfigurationTemplateID: str,
```

## DeleteSourceNetworkRequestRequestTypeDef

```python
# DeleteSourceNetworkRequestRequestTypeDef definition

class DeleteSourceNetworkRequestRequestTypeDef(TypedDict):
    sourceNetworkID: str,
```

## DeleteSourceServerRequestRequestTypeDef

```python
# DeleteSourceServerRequestRequestTypeDef definition

class DeleteSourceServerRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
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

## DescribeRecoveryInstancesRequestFiltersTypeDef

```python
# DescribeRecoveryInstancesRequestFiltersTypeDef definition

class DescribeRecoveryInstancesRequestFiltersTypeDef(TypedDict):
    recoveryInstanceIDs: NotRequired[Sequence[str]],
    sourceServerIDs: NotRequired[Sequence[str]],
```

## DescribeRecoverySnapshotsRequestFiltersTypeDef

```python
# DescribeRecoverySnapshotsRequestFiltersTypeDef definition

class DescribeRecoverySnapshotsRequestFiltersTypeDef(TypedDict):
    fromDateTime: NotRequired[str],
    toDateTime: NotRequired[str],
```

## RecoverySnapshotTypeDef

```python
# RecoverySnapshotTypeDef definition

class RecoverySnapshotTypeDef(TypedDict):
    expectedTimestamp: str,
    snapshotID: str,
    sourceServerID: str,
    ebsSnapshots: NotRequired[List[str]],
    timestamp: NotRequired[str],
```

## DescribeReplicationConfigurationTemplatesRequestRequestTypeDef

```python
# DescribeReplicationConfigurationTemplatesRequestRequestTypeDef definition

class DescribeReplicationConfigurationTemplatesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    replicationConfigurationTemplateIDs: NotRequired[Sequence[str]],
```

## DescribeSourceNetworksRequestFiltersTypeDef

```python
# DescribeSourceNetworksRequestFiltersTypeDef definition

class DescribeSourceNetworksRequestFiltersTypeDef(TypedDict):
    originAccountID: NotRequired[str],
    originRegion: NotRequired[str],
    sourceNetworkIDs: NotRequired[Sequence[str]],
```

## DescribeSourceServersRequestFiltersTypeDef

```python
# DescribeSourceServersRequestFiltersTypeDef definition

class DescribeSourceServersRequestFiltersTypeDef(TypedDict):
    hardwareId: NotRequired[str],
    sourceServerIDs: NotRequired[Sequence[str]],
    stagingAccountIDs: NotRequired[Sequence[str]],
```

## DisconnectRecoveryInstanceRequestRequestTypeDef

```python
# DisconnectRecoveryInstanceRequestRequestTypeDef definition

class DisconnectRecoveryInstanceRequestRequestTypeDef(TypedDict):
    recoveryInstanceID: str,
```

## DisconnectSourceServerRequestRequestTypeDef

```python
# DisconnectSourceServerRequestRequestTypeDef definition

class DisconnectSourceServerRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
```

## DiskTypeDef

```python
# DiskTypeDef definition

class DiskTypeDef(TypedDict):
    bytes: NotRequired[int],
    deviceName: NotRequired[str],
```

## SourceNetworkDataTypeDef

```python
# SourceNetworkDataTypeDef definition

class SourceNetworkDataTypeDef(TypedDict):
    sourceNetworkID: NotRequired[str],
    sourceVpc: NotRequired[str],
    stackName: NotRequired[str],
    targetVpc: NotRequired[str],
```

## ExportSourceNetworkCfnTemplateRequestRequestTypeDef

```python
# ExportSourceNetworkCfnTemplateRequestRequestTypeDef definition

class ExportSourceNetworkCfnTemplateRequestRequestTypeDef(TypedDict):
    sourceNetworkID: str,
```

## GetFailbackReplicationConfigurationRequestRequestTypeDef

```python
# GetFailbackReplicationConfigurationRequestRequestTypeDef definition

class GetFailbackReplicationConfigurationRequestRequestTypeDef(TypedDict):
    recoveryInstanceID: str,
```

## GetLaunchConfigurationRequestRequestTypeDef

```python
# GetLaunchConfigurationRequestRequestTypeDef definition

class GetLaunchConfigurationRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
```

## GetReplicationConfigurationRequestRequestTypeDef

```python
# GetReplicationConfigurationRequestRequestTypeDef definition

class GetReplicationConfigurationRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
```

## IdentificationHintsTypeDef

```python
# IdentificationHintsTypeDef definition

class IdentificationHintsTypeDef(TypedDict):
    awsInstanceID: NotRequired[str],
    fqdn: NotRequired[str],
    hostname: NotRequired[str],
    vmWareUuid: NotRequired[str],
```

## LaunchActionParameterTypeDef

```python
# LaunchActionParameterTypeDef definition

class LaunchActionParameterTypeDef(TypedDict):
    type: NotRequired[LaunchActionParameterTypeType],  # (1)
    value: NotRequired[str],
```

1. See [:material-code-brackets: LaunchActionParameterTypeType](./literals.md#launchactionparametertypetype) 
## LaunchActionsRequestFiltersTypeDef

```python
# LaunchActionsRequestFiltersTypeDef definition

class LaunchActionsRequestFiltersTypeDef(TypedDict):
    actionIds: NotRequired[Sequence[str]],
```

## LaunchIntoInstancePropertiesTypeDef

```python
# LaunchIntoInstancePropertiesTypeDef definition

class LaunchIntoInstancePropertiesTypeDef(TypedDict):
    launchIntoEC2InstanceID: NotRequired[str],
```

## LifeCycleLastLaunchInitiatedTypeDef

```python
# LifeCycleLastLaunchInitiatedTypeDef definition

class LifeCycleLastLaunchInitiatedTypeDef(TypedDict):
    apiCallDateTime: NotRequired[str],
    jobID: NotRequired[str],
    type: NotRequired[LastLaunchTypeType],  # (1)
```

1. See [:material-code-brackets: LastLaunchTypeType](./literals.md#lastlaunchtypetype) 
## ListExtensibleSourceServersRequestRequestTypeDef

```python
# ListExtensibleSourceServersRequestRequestTypeDef definition

class ListExtensibleSourceServersRequestRequestTypeDef(TypedDict):
    stagingAccountID: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## StagingSourceServerTypeDef

```python
# StagingSourceServerTypeDef definition

class StagingSourceServerTypeDef(TypedDict):
    arn: NotRequired[str],
    hostname: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## ListStagingAccountsRequestRequestTypeDef

```python
# ListStagingAccountsRequestRequestTypeDef definition

class ListStagingAccountsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
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

## ParticipatingResourceIDTypeDef

```python
# ParticipatingResourceIDTypeDef definition

class ParticipatingResourceIDTypeDef(TypedDict):
    sourceNetworkID: NotRequired[str],
```

## RecoveryInstanceDataReplicationErrorTypeDef

```python
# RecoveryInstanceDataReplicationErrorTypeDef definition

class RecoveryInstanceDataReplicationErrorTypeDef(TypedDict):
    error: NotRequired[FailbackReplicationErrorType],  # (1)
    rawError: NotRequired[str],
```

1. See [:material-code-brackets: FailbackReplicationErrorType](./literals.md#failbackreplicationerrortype) 
## RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef

```python
# RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef definition

class RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef(TypedDict):
    backloggedStorageBytes: NotRequired[int],
    deviceName: NotRequired[str],
    replicatedStorageBytes: NotRequired[int],
    rescannedStorageBytes: NotRequired[int],
    totalStorageBytes: NotRequired[int],
```

## RecoveryInstanceDataReplicationInitiationStepTypeDef

```python
# RecoveryInstanceDataReplicationInitiationStepTypeDef definition

class RecoveryInstanceDataReplicationInitiationStepTypeDef(TypedDict):
    name: NotRequired[RecoveryInstanceDataReplicationInitiationStepNameType],  # (1)
    status: NotRequired[RecoveryInstanceDataReplicationInitiationStepStatusType],  # (2)
```

1. See [:material-code-brackets: RecoveryInstanceDataReplicationInitiationStepNameType](./literals.md#recoveryinstancedatareplicationinitiationstepnametype) 
2. See [:material-code-brackets: RecoveryInstanceDataReplicationInitiationStepStatusType](./literals.md#recoveryinstancedatareplicationinitiationstepstatustype) 
## RecoveryInstanceDiskTypeDef

```python
# RecoveryInstanceDiskTypeDef definition

class RecoveryInstanceDiskTypeDef(TypedDict):
    bytes: NotRequired[int],
    ebsVolumeID: NotRequired[str],
    internalDeviceName: NotRequired[str],
```

## RecoveryInstanceFailbackTypeDef

```python
# RecoveryInstanceFailbackTypeDef definition

class RecoveryInstanceFailbackTypeDef(TypedDict):
    agentLastSeenByServiceDateTime: NotRequired[str],
    elapsedReplicationDuration: NotRequired[str],
    failbackClientID: NotRequired[str],
    failbackClientLastSeenByServiceDateTime: NotRequired[str],
    failbackInitiationTime: NotRequired[str],
    failbackJobID: NotRequired[str],
    failbackLaunchType: NotRequired[FailbackLaunchTypeType],  # (1)
    failbackToOriginalServer: NotRequired[bool],
    firstByteDateTime: NotRequired[str],
    state: NotRequired[FailbackStateType],  # (2)
```

1. See [:material-code-brackets: FailbackLaunchTypeType](./literals.md#failbacklaunchtypetype) 
2. See [:material-code-brackets: FailbackStateType](./literals.md#failbackstatetype) 
## RecoveryLifeCycleTypeDef

```python
# RecoveryLifeCycleTypeDef definition

class RecoveryLifeCycleTypeDef(TypedDict):
    apiCallDateTime: NotRequired[datetime],
    jobID: NotRequired[str],
    lastRecoveryResult: NotRequired[RecoveryResultType],  # (1)
```

1. See [:material-code-brackets: RecoveryResultType](./literals.md#recoveryresulttype) 
## ReplicationConfigurationReplicatedDiskTypeDef

```python
# ReplicationConfigurationReplicatedDiskTypeDef definition

class ReplicationConfigurationReplicatedDiskTypeDef(TypedDict):
    deviceName: NotRequired[str],
    iops: NotRequired[int],
    isBootDisk: NotRequired[bool],
    optimizedStagingDiskType: NotRequired[ReplicationConfigurationReplicatedDiskStagingDiskTypeType],  # (1)
    stagingDiskType: NotRequired[ReplicationConfigurationReplicatedDiskStagingDiskTypeType],  # (1)
    throughput: NotRequired[int],
```

1. See [:material-code-brackets: ReplicationConfigurationReplicatedDiskStagingDiskTypeType](./literals.md#replicationconfigurationreplicateddiskstagingdisktypetype) 
2. See [:material-code-brackets: ReplicationConfigurationReplicatedDiskStagingDiskTypeType](./literals.md#replicationconfigurationreplicateddiskstagingdisktypetype) 
## RetryDataReplicationRequestRequestTypeDef

```python
# RetryDataReplicationRequestRequestTypeDef definition

class RetryDataReplicationRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
```

## ReverseReplicationRequestRequestTypeDef

```python
# ReverseReplicationRequestRequestTypeDef definition

class ReverseReplicationRequestRequestTypeDef(TypedDict):
    recoveryInstanceID: str,
```

## SourceCloudPropertiesTypeDef

```python
# SourceCloudPropertiesTypeDef definition

class SourceCloudPropertiesTypeDef(TypedDict):
    originAccountID: NotRequired[str],
    originAvailabilityZone: NotRequired[str],
    originRegion: NotRequired[str],
    sourceOutpostArn: NotRequired[str],
```

## StagingAreaTypeDef

```python
# StagingAreaTypeDef definition

class StagingAreaTypeDef(TypedDict):
    errorMessage: NotRequired[str],
    stagingAccountID: NotRequired[str],
    stagingSourceServerArn: NotRequired[str],
    status: NotRequired[ExtensionStatusType],  # (1)
```

1. See [:material-code-brackets: ExtensionStatusType](./literals.md#extensionstatustype) 
## StartFailbackLaunchRequestRequestTypeDef

```python
# StartFailbackLaunchRequestRequestTypeDef definition

class StartFailbackLaunchRequestRequestTypeDef(TypedDict):
    recoveryInstanceIDs: Sequence[str],
    tags: NotRequired[Mapping[str, str]],
```

## StartRecoveryRequestSourceServerTypeDef

```python
# StartRecoveryRequestSourceServerTypeDef definition

class StartRecoveryRequestSourceServerTypeDef(TypedDict):
    sourceServerID: str,
    recoverySnapshotID: NotRequired[str],
```

## StartReplicationRequestRequestTypeDef

```python
# StartReplicationRequestRequestTypeDef definition

class StartReplicationRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
```

## StartSourceNetworkRecoveryRequestNetworkEntryTypeDef

```python
# StartSourceNetworkRecoveryRequestNetworkEntryTypeDef definition

class StartSourceNetworkRecoveryRequestNetworkEntryTypeDef(TypedDict):
    sourceNetworkID: str,
    cfnStackName: NotRequired[str],
```

## StartSourceNetworkReplicationRequestRequestTypeDef

```python
# StartSourceNetworkReplicationRequestRequestTypeDef definition

class StartSourceNetworkReplicationRequestRequestTypeDef(TypedDict):
    sourceNetworkID: str,
```

## StopFailbackRequestRequestTypeDef

```python
# StopFailbackRequestRequestTypeDef definition

class StopFailbackRequestRequestTypeDef(TypedDict):
    recoveryInstanceID: str,
```

## StopReplicationRequestRequestTypeDef

```python
# StopReplicationRequestRequestTypeDef definition

class StopReplicationRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
```

## StopSourceNetworkReplicationRequestRequestTypeDef

```python
# StopSourceNetworkReplicationRequestRequestTypeDef definition

class StopSourceNetworkReplicationRequestRequestTypeDef(TypedDict):
    sourceNetworkID: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## TerminateRecoveryInstancesRequestRequestTypeDef

```python
# TerminateRecoveryInstancesRequestRequestTypeDef definition

class TerminateRecoveryInstancesRequestRequestTypeDef(TypedDict):
    recoveryInstanceIDs: Sequence[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateFailbackReplicationConfigurationRequestRequestTypeDef

```python
# UpdateFailbackReplicationConfigurationRequestRequestTypeDef definition

class UpdateFailbackReplicationConfigurationRequestRequestTypeDef(TypedDict):
    recoveryInstanceID: str,
    bandwidthThrottling: NotRequired[int],
    name: NotRequired[str],
    usePrivateIP: NotRequired[bool],
```

## CreateSourceNetworkResponseTypeDef

```python
# CreateSourceNetworkResponseTypeDef definition

class CreateSourceNetworkResponseTypeDef(TypedDict):
    sourceNetworkID: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportSourceNetworkCfnTemplateResponseTypeDef

```python
# ExportSourceNetworkCfnTemplateResponseTypeDef definition

class ExportSourceNetworkCfnTemplateResponseTypeDef(TypedDict):
    s3DestinationUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFailbackReplicationConfigurationResponseTypeDef

```python
# GetFailbackReplicationConfigurationResponseTypeDef definition

class GetFailbackReplicationConfigurationResponseTypeDef(TypedDict):
    bandwidthThrottling: int,
    name: str,
    recoveryInstanceID: str,
    usePrivateIP: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStagingAccountsResponseTypeDef

```python
# ListStagingAccountsResponseTypeDef definition

class ListStagingAccountsResponseTypeDef(TypedDict):
    accounts: List[AccountTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReverseReplicationResponseTypeDef

```python
# ReverseReplicationResponseTypeDef definition

class ReverseReplicationResponseTypeDef(TypedDict):
    reversedDirectionSourceServerArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConversionPropertiesTypeDef

```python
# ConversionPropertiesTypeDef definition

class ConversionPropertiesTypeDef(TypedDict):
    dataTimestamp: NotRequired[str],
    forceUefi: NotRequired[bool],
    rootVolumeName: NotRequired[str],
    volumeToConversionMap: NotRequired[Dict[str, Dict[str, str]]],
    volumeToProductCodes: NotRequired[Dict[str, List[ProductCodeTypeDef]]],  # (1)
    volumeToVolumeSize: NotRequired[Dict[str, int]],
```

1. See [:material-code-braces: ProductCodeTypeDef](./type_defs.md#productcodetypedef) 
## CreateLaunchConfigurationTemplateRequestRequestTypeDef

```python
# CreateLaunchConfigurationTemplateRequestRequestTypeDef definition

class CreateLaunchConfigurationTemplateRequestRequestTypeDef(TypedDict):
    copyPrivateIp: NotRequired[bool],
    copyTags: NotRequired[bool],
    exportBucketArn: NotRequired[str],
    launchDisposition: NotRequired[LaunchDispositionType],  # (1)
    launchIntoSourceInstance: NotRequired[bool],
    licensing: NotRequired[LicensingTypeDef],  # (2)
    postLaunchEnabled: NotRequired[bool],
    tags: NotRequired[Mapping[str, str]],
    targetInstanceTypeRightSizingMethod: NotRequired[TargetInstanceTypeRightSizingMethodType],  # (3)
```

1. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype) 
2. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef) 
3. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype) 
## LaunchConfigurationTemplateTypeDef

```python
# LaunchConfigurationTemplateTypeDef definition

class LaunchConfigurationTemplateTypeDef(TypedDict):
    arn: NotRequired[str],
    copyPrivateIp: NotRequired[bool],
    copyTags: NotRequired[bool],
    exportBucketArn: NotRequired[str],
    launchConfigurationTemplateID: NotRequired[str],
    launchDisposition: NotRequired[LaunchDispositionType],  # (1)
    launchIntoSourceInstance: NotRequired[bool],
    licensing: NotRequired[LicensingTypeDef],  # (2)
    postLaunchEnabled: NotRequired[bool],
    tags: NotRequired[Dict[str, str]],
    targetInstanceTypeRightSizingMethod: NotRequired[TargetInstanceTypeRightSizingMethodType],  # (3)
```

1. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype) 
2. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef) 
3. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype) 
## UpdateLaunchConfigurationTemplateRequestRequestTypeDef

```python
# UpdateLaunchConfigurationTemplateRequestRequestTypeDef definition

class UpdateLaunchConfigurationTemplateRequestRequestTypeDef(TypedDict):
    launchConfigurationTemplateID: str,
    copyPrivateIp: NotRequired[bool],
    copyTags: NotRequired[bool],
    exportBucketArn: NotRequired[str],
    launchDisposition: NotRequired[LaunchDispositionType],  # (1)
    launchIntoSourceInstance: NotRequired[bool],
    licensing: NotRequired[LicensingTypeDef],  # (2)
    postLaunchEnabled: NotRequired[bool],
    targetInstanceTypeRightSizingMethod: NotRequired[TargetInstanceTypeRightSizingMethodType],  # (3)
```

1. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype) 
2. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef) 
3. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype) 
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
    pitPolicy: Sequence[PITPolicyRuleTypeDef],  # (4)
    replicationServerInstanceType: str,
    replicationServersSecurityGroupsIDs: Sequence[str],
    stagingAreaSubnetId: str,
    stagingAreaTags: Mapping[str, str],
    useDedicatedReplicationServer: bool,
    autoReplicateNewDisks: NotRequired[bool],
    ebsEncryptionKeyArn: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype) 
2. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype) 
3. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype) 
4. See [:material-code-braces: PITPolicyRuleTypeDef](./type_defs.md#pitpolicyruletypedef) 
## ReplicationConfigurationTemplateResponseTypeDef

```python
# ReplicationConfigurationTemplateResponseTypeDef definition

class ReplicationConfigurationTemplateResponseTypeDef(TypedDict):
    arn: str,
    associateDefaultSecurityGroup: bool,
    autoReplicateNewDisks: bool,
    bandwidthThrottling: int,
    createPublicIP: bool,
    dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType,  # (1)
    defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType,  # (2)
    ebsEncryption: ReplicationConfigurationEbsEncryptionType,  # (3)
    ebsEncryptionKeyArn: str,
    pitPolicy: List[PITPolicyRuleTypeDef],  # (4)
    replicationConfigurationTemplateID: str,
    replicationServerInstanceType: str,
    replicationServersSecurityGroupsIDs: List[str],
    stagingAreaSubnetId: str,
    stagingAreaTags: Dict[str, str],
    tags: Dict[str, str],
    useDedicatedReplicationServer: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype) 
2. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype) 
3. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype) 
4. See [:material-code-braces: PITPolicyRuleTypeDef](./type_defs.md#pitpolicyruletypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReplicationConfigurationTemplateTypeDef

```python
# ReplicationConfigurationTemplateTypeDef definition

class ReplicationConfigurationTemplateTypeDef(TypedDict):
    replicationConfigurationTemplateID: str,
    arn: NotRequired[str],
    associateDefaultSecurityGroup: NotRequired[bool],
    autoReplicateNewDisks: NotRequired[bool],
    bandwidthThrottling: NotRequired[int],
    createPublicIP: NotRequired[bool],
    dataPlaneRouting: NotRequired[ReplicationConfigurationDataPlaneRoutingType],  # (1)
    defaultLargeStagingDiskType: NotRequired[ReplicationConfigurationDefaultLargeStagingDiskTypeType],  # (2)
    ebsEncryption: NotRequired[ReplicationConfigurationEbsEncryptionType],  # (3)
    ebsEncryptionKeyArn: NotRequired[str],
    pitPolicy: NotRequired[List[PITPolicyRuleTypeDef]],  # (4)
    replicationServerInstanceType: NotRequired[str],
    replicationServersSecurityGroupsIDs: NotRequired[List[str]],
    stagingAreaSubnetId: NotRequired[str],
    stagingAreaTags: NotRequired[Dict[str, str]],
    tags: NotRequired[Dict[str, str]],
    useDedicatedReplicationServer: NotRequired[bool],
```

1. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype) 
2. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype) 
3. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype) 
4. See [:material-code-braces: PITPolicyRuleTypeDef](./type_defs.md#pitpolicyruletypedef) 
## UpdateReplicationConfigurationTemplateRequestRequestTypeDef

```python
# UpdateReplicationConfigurationTemplateRequestRequestTypeDef definition

class UpdateReplicationConfigurationTemplateRequestRequestTypeDef(TypedDict):
    replicationConfigurationTemplateID: str,
    arn: NotRequired[str],
    associateDefaultSecurityGroup: NotRequired[bool],
    autoReplicateNewDisks: NotRequired[bool],
    bandwidthThrottling: NotRequired[int],
    createPublicIP: NotRequired[bool],
    dataPlaneRouting: NotRequired[ReplicationConfigurationDataPlaneRoutingType],  # (1)
    defaultLargeStagingDiskType: NotRequired[ReplicationConfigurationDefaultLargeStagingDiskTypeType],  # (2)
    ebsEncryption: NotRequired[ReplicationConfigurationEbsEncryptionType],  # (3)
    ebsEncryptionKeyArn: NotRequired[str],
    pitPolicy: NotRequired[Sequence[PITPolicyRuleTypeDef]],  # (4)
    replicationServerInstanceType: NotRequired[str],
    replicationServersSecurityGroupsIDs: NotRequired[Sequence[str]],
    stagingAreaSubnetId: NotRequired[str],
    stagingAreaTags: NotRequired[Mapping[str, str]],
    useDedicatedReplicationServer: NotRequired[bool],
```

1. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype) 
2. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype) 
3. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype) 
4. See [:material-code-braces: PITPolicyRuleTypeDef](./type_defs.md#pitpolicyruletypedef) 
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
## ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef

```python
# ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef definition

class ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef(TypedDict):
    stagingAccountID: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStagingAccountsRequestListStagingAccountsPaginateTypeDef

```python
# ListStagingAccountsRequestListStagingAccountsPaginateTypeDef definition

class ListStagingAccountsRequestListStagingAccountsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeJobsRequestDescribeJobsPaginateTypeDef

```python
# DescribeJobsRequestDescribeJobsPaginateTypeDef definition

class DescribeJobsRequestDescribeJobsPaginateTypeDef(TypedDict):
    filters: NotRequired[DescribeJobsRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DescribeJobsRequestFiltersTypeDef](./type_defs.md#describejobsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeJobsRequestRequestTypeDef

```python
# DescribeJobsRequestRequestTypeDef definition

class DescribeJobsRequestRequestTypeDef(TypedDict):
    filters: NotRequired[DescribeJobsRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DescribeJobsRequestFiltersTypeDef](./type_defs.md#describejobsrequestfilterstypedef) 
## DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef

```python
# DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef definition

class DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef(TypedDict):
    filters: NotRequired[DescribeRecoveryInstancesRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DescribeRecoveryInstancesRequestFiltersTypeDef](./type_defs.md#describerecoveryinstancesrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeRecoveryInstancesRequestRequestTypeDef

```python
# DescribeRecoveryInstancesRequestRequestTypeDef definition

class DescribeRecoveryInstancesRequestRequestTypeDef(TypedDict):
    filters: NotRequired[DescribeRecoveryInstancesRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DescribeRecoveryInstancesRequestFiltersTypeDef](./type_defs.md#describerecoveryinstancesrequestfilterstypedef) 
## DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef

```python
# DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef definition

class DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef(TypedDict):
    sourceServerID: str,
    filters: NotRequired[DescribeRecoverySnapshotsRequestFiltersTypeDef],  # (1)
    order: NotRequired[RecoverySnapshotsOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: DescribeRecoverySnapshotsRequestFiltersTypeDef](./type_defs.md#describerecoverysnapshotsrequestfilterstypedef) 
2. See [:material-code-brackets: RecoverySnapshotsOrderType](./literals.md#recoverysnapshotsordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeRecoverySnapshotsRequestRequestTypeDef

```python
# DescribeRecoverySnapshotsRequestRequestTypeDef definition

class DescribeRecoverySnapshotsRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
    filters: NotRequired[DescribeRecoverySnapshotsRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    order: NotRequired[RecoverySnapshotsOrderType],  # (2)
```

1. See [:material-code-braces: DescribeRecoverySnapshotsRequestFiltersTypeDef](./type_defs.md#describerecoverysnapshotsrequestfilterstypedef) 
2. See [:material-code-brackets: RecoverySnapshotsOrderType](./literals.md#recoverysnapshotsordertype) 
## DescribeRecoverySnapshotsResponseTypeDef

```python
# DescribeRecoverySnapshotsResponseTypeDef definition

class DescribeRecoverySnapshotsResponseTypeDef(TypedDict):
    items: List[RecoverySnapshotTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RecoverySnapshotTypeDef](./type_defs.md#recoverysnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef

```python
# DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef definition

class DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef(TypedDict):
    filters: NotRequired[DescribeSourceNetworksRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DescribeSourceNetworksRequestFiltersTypeDef](./type_defs.md#describesourcenetworksrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSourceNetworksRequestRequestTypeDef

```python
# DescribeSourceNetworksRequestRequestTypeDef definition

class DescribeSourceNetworksRequestRequestTypeDef(TypedDict):
    filters: NotRequired[DescribeSourceNetworksRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DescribeSourceNetworksRequestFiltersTypeDef](./type_defs.md#describesourcenetworksrequestfilterstypedef) 
## DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef

```python
# DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef definition

class DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef(TypedDict):
    filters: NotRequired[DescribeSourceServersRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DescribeSourceServersRequestFiltersTypeDef](./type_defs.md#describesourceserversrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSourceServersRequestRequestTypeDef

```python
# DescribeSourceServersRequestRequestTypeDef definition

class DescribeSourceServersRequestRequestTypeDef(TypedDict):
    filters: NotRequired[DescribeSourceServersRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DescribeSourceServersRequestFiltersTypeDef](./type_defs.md#describesourceserversrequestfilterstypedef) 
## EventResourceDataTypeDef

```python
# EventResourceDataTypeDef definition

class EventResourceDataTypeDef(TypedDict):
    sourceNetworkData: NotRequired[SourceNetworkDataTypeDef],  # (1)
```

1. See [:material-code-braces: SourceNetworkDataTypeDef](./type_defs.md#sourcenetworkdatatypedef) 
## LaunchActionTypeDef

```python
# LaunchActionTypeDef definition

class LaunchActionTypeDef(TypedDict):
    actionCode: NotRequired[str],
    actionId: NotRequired[str],
    actionVersion: NotRequired[str],
    active: NotRequired[bool],
    category: NotRequired[LaunchActionCategoryType],  # (1)
    description: NotRequired[str],
    name: NotRequired[str],
    optional: NotRequired[bool],
    order: NotRequired[int],
    parameters: NotRequired[Dict[str, LaunchActionParameterTypeDef]],  # (2)
    type: NotRequired[LaunchActionTypeType],  # (3)
```

1. See [:material-code-brackets: LaunchActionCategoryType](./literals.md#launchactioncategorytype) 
2. See [:material-code-braces: LaunchActionParameterTypeDef](./type_defs.md#launchactionparametertypedef) 
3. See [:material-code-brackets: LaunchActionTypeType](./literals.md#launchactiontypetype) 
## PutLaunchActionRequestRequestTypeDef

```python
# PutLaunchActionRequestRequestTypeDef definition

class PutLaunchActionRequestRequestTypeDef(TypedDict):
    actionCode: str,
    actionId: str,
    actionVersion: str,
    active: bool,
    category: LaunchActionCategoryType,  # (1)
    description: str,
    name: str,
    optional: bool,
    order: int,
    resourceId: str,
    parameters: NotRequired[Mapping[str, LaunchActionParameterTypeDef]],  # (2)
```

1. See [:material-code-brackets: LaunchActionCategoryType](./literals.md#launchactioncategorytype) 
2. See [:material-code-braces: LaunchActionParameterTypeDef](./type_defs.md#launchactionparametertypedef) 
## PutLaunchActionResponseTypeDef

```python
# PutLaunchActionResponseTypeDef definition

class PutLaunchActionResponseTypeDef(TypedDict):
    actionCode: str,
    actionId: str,
    actionVersion: str,
    active: bool,
    category: LaunchActionCategoryType,  # (1)
    description: str,
    name: str,
    optional: bool,
    order: int,
    parameters: Dict[str, LaunchActionParameterTypeDef],  # (2)
    resourceId: str,
    type: LaunchActionTypeType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: LaunchActionCategoryType](./literals.md#launchactioncategorytype) 
2. See [:material-code-braces: LaunchActionParameterTypeDef](./type_defs.md#launchactionparametertypedef) 
3. See [:material-code-brackets: LaunchActionTypeType](./literals.md#launchactiontypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLaunchActionsRequestListLaunchActionsPaginateTypeDef

```python
# ListLaunchActionsRequestListLaunchActionsPaginateTypeDef definition

class ListLaunchActionsRequestListLaunchActionsPaginateTypeDef(TypedDict):
    resourceId: str,
    filters: NotRequired[LaunchActionsRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: LaunchActionsRequestFiltersTypeDef](./type_defs.md#launchactionsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLaunchActionsRequestRequestTypeDef

```python
# ListLaunchActionsRequestRequestTypeDef definition

class ListLaunchActionsRequestRequestTypeDef(TypedDict):
    resourceId: str,
    filters: NotRequired[LaunchActionsRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LaunchActionsRequestFiltersTypeDef](./type_defs.md#launchactionsrequestfilterstypedef) 
## LaunchConfigurationTypeDef

```python
# LaunchConfigurationTypeDef definition

class LaunchConfigurationTypeDef(TypedDict):
    copyPrivateIp: bool,
    copyTags: bool,
    ec2LaunchTemplateID: str,
    launchDisposition: LaunchDispositionType,  # (1)
    launchIntoInstanceProperties: LaunchIntoInstancePropertiesTypeDef,  # (2)
    licensing: LicensingTypeDef,  # (3)
    name: str,
    postLaunchEnabled: bool,
    sourceServerID: str,
    targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype) 
2. See [:material-code-braces: LaunchIntoInstancePropertiesTypeDef](./type_defs.md#launchintoinstancepropertiestypedef) 
3. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef) 
4. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLaunchConfigurationRequestRequestTypeDef

```python
# UpdateLaunchConfigurationRequestRequestTypeDef definition

class UpdateLaunchConfigurationRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
    copyPrivateIp: NotRequired[bool],
    copyTags: NotRequired[bool],
    launchDisposition: NotRequired[LaunchDispositionType],  # (1)
    launchIntoInstanceProperties: NotRequired[LaunchIntoInstancePropertiesTypeDef],  # (2)
    licensing: NotRequired[LicensingTypeDef],  # (3)
    name: NotRequired[str],
    postLaunchEnabled: NotRequired[bool],
    targetInstanceTypeRightSizingMethod: NotRequired[TargetInstanceTypeRightSizingMethodType],  # (4)
```

1. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype) 
2. See [:material-code-braces: LaunchIntoInstancePropertiesTypeDef](./type_defs.md#launchintoinstancepropertiestypedef) 
3. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef) 
4. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype) 
## LifeCycleLastLaunchTypeDef

```python
# LifeCycleLastLaunchTypeDef definition

class LifeCycleLastLaunchTypeDef(TypedDict):
    initiated: NotRequired[LifeCycleLastLaunchInitiatedTypeDef],  # (1)
    status: NotRequired[LaunchStatusType],  # (2)
```

1. See [:material-code-braces: LifeCycleLastLaunchInitiatedTypeDef](./type_defs.md#lifecyclelastlaunchinitiatedtypedef) 
2. See [:material-code-brackets: LaunchStatusType](./literals.md#launchstatustype) 
## ListExtensibleSourceServersResponseTypeDef

```python
# ListExtensibleSourceServersResponseTypeDef definition

class ListExtensibleSourceServersResponseTypeDef(TypedDict):
    items: List[StagingSourceServerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: StagingSourceServerTypeDef](./type_defs.md#stagingsourceservertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    supportsNitroInstances: NotRequired[bool],
```

1. See [:material-code-braces: CPUTypeDef](./type_defs.md#cputypedef) 
2. See [:material-code-braces: DiskTypeDef](./type_defs.md#disktypedef) 
3. See [:material-code-braces: IdentificationHintsTypeDef](./type_defs.md#identificationhintstypedef) 
4. See [:material-code-braces: NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef) 
5. See [:material-code-braces: OSTypeDef](./type_defs.md#ostypedef) 
## ParticipatingResourceTypeDef

```python
# ParticipatingResourceTypeDef definition

class ParticipatingResourceTypeDef(TypedDict):
    launchStatus: NotRequired[LaunchStatusType],  # (1)
    participatingResourceID: NotRequired[ParticipatingResourceIDTypeDef],  # (2)
```

1. See [:material-code-brackets: LaunchStatusType](./literals.md#launchstatustype) 
2. See [:material-code-braces: ParticipatingResourceIDTypeDef](./type_defs.md#participatingresourceidtypedef) 
## RecoveryInstanceDataReplicationInitiationTypeDef

```python
# RecoveryInstanceDataReplicationInitiationTypeDef definition

class RecoveryInstanceDataReplicationInitiationTypeDef(TypedDict):
    startDateTime: NotRequired[str],
    steps: NotRequired[List[RecoveryInstanceDataReplicationInitiationStepTypeDef]],  # (1)
```

1. See [:material-code-braces: RecoveryInstanceDataReplicationInitiationStepTypeDef](./type_defs.md#recoveryinstancedatareplicationinitiationsteptypedef) 
## RecoveryInstancePropertiesTypeDef

```python
# RecoveryInstancePropertiesTypeDef definition

class RecoveryInstancePropertiesTypeDef(TypedDict):
    cpus: NotRequired[List[CPUTypeDef]],  # (1)
    disks: NotRequired[List[RecoveryInstanceDiskTypeDef]],  # (2)
    identificationHints: NotRequired[IdentificationHintsTypeDef],  # (3)
    lastUpdatedDateTime: NotRequired[str],
    networkInterfaces: NotRequired[List[NetworkInterfaceTypeDef]],  # (4)
    os: NotRequired[OSTypeDef],  # (5)
    ramBytes: NotRequired[int],
```

1. See [:material-code-braces: CPUTypeDef](./type_defs.md#cputypedef) 
2. See [:material-code-braces: RecoveryInstanceDiskTypeDef](./type_defs.md#recoveryinstancedisktypedef) 
3. See [:material-code-braces: IdentificationHintsTypeDef](./type_defs.md#identificationhintstypedef) 
4. See [:material-code-braces: NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef) 
5. See [:material-code-braces: OSTypeDef](./type_defs.md#ostypedef) 
## SourceNetworkTypeDef

```python
# SourceNetworkTypeDef definition

class SourceNetworkTypeDef(TypedDict):
    arn: NotRequired[str],
    cfnStackName: NotRequired[str],
    lastRecovery: NotRequired[RecoveryLifeCycleTypeDef],  # (1)
    launchedVpcID: NotRequired[str],
    replicationStatus: NotRequired[ReplicationStatusType],  # (2)
    replicationStatusDetails: NotRequired[str],
    sourceAccountID: NotRequired[str],
    sourceNetworkID: NotRequired[str],
    sourceRegion: NotRequired[str],
    sourceVpcID: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: RecoveryLifeCycleTypeDef](./type_defs.md#recoverylifecycletypedef) 
2. See [:material-code-brackets: ReplicationStatusType](./literals.md#replicationstatustype) 
## ReplicationConfigurationTypeDef

```python
# ReplicationConfigurationTypeDef definition

class ReplicationConfigurationTypeDef(TypedDict):
    associateDefaultSecurityGroup: bool,
    autoReplicateNewDisks: bool,
    bandwidthThrottling: int,
    createPublicIP: bool,
    dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType,  # (1)
    defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType,  # (2)
    ebsEncryption: ReplicationConfigurationEbsEncryptionType,  # (3)
    ebsEncryptionKeyArn: str,
    name: str,
    pitPolicy: List[PITPolicyRuleTypeDef],  # (4)
    replicatedDisks: List[ReplicationConfigurationReplicatedDiskTypeDef],  # (5)
    replicationServerInstanceType: str,
    replicationServersSecurityGroupsIDs: List[str],
    sourceServerID: str,
    stagingAreaSubnetId: str,
    stagingAreaTags: Dict[str, str],
    useDedicatedReplicationServer: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype) 
2. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype) 
3. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype) 
4. See [:material-code-braces: PITPolicyRuleTypeDef](./type_defs.md#pitpolicyruletypedef) 
5. See [:material-code-braces: ReplicationConfigurationReplicatedDiskTypeDef](./type_defs.md#replicationconfigurationreplicateddisktypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateReplicationConfigurationRequestRequestTypeDef

```python
# UpdateReplicationConfigurationRequestRequestTypeDef definition

class UpdateReplicationConfigurationRequestRequestTypeDef(TypedDict):
    sourceServerID: str,
    associateDefaultSecurityGroup: NotRequired[bool],
    autoReplicateNewDisks: NotRequired[bool],
    bandwidthThrottling: NotRequired[int],
    createPublicIP: NotRequired[bool],
    dataPlaneRouting: NotRequired[ReplicationConfigurationDataPlaneRoutingType],  # (1)
    defaultLargeStagingDiskType: NotRequired[ReplicationConfigurationDefaultLargeStagingDiskTypeType],  # (2)
    ebsEncryption: NotRequired[ReplicationConfigurationEbsEncryptionType],  # (3)
    ebsEncryptionKeyArn: NotRequired[str],
    name: NotRequired[str],
    pitPolicy: NotRequired[Sequence[PITPolicyRuleTypeDef]],  # (4)
    replicatedDisks: NotRequired[Sequence[ReplicationConfigurationReplicatedDiskTypeDef]],  # (5)
    replicationServerInstanceType: NotRequired[str],
    replicationServersSecurityGroupsIDs: NotRequired[Sequence[str]],
    stagingAreaSubnetId: NotRequired[str],
    stagingAreaTags: NotRequired[Mapping[str, str]],
    useDedicatedReplicationServer: NotRequired[bool],
```

1. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype) 
2. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype) 
3. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype) 
4. See [:material-code-braces: PITPolicyRuleTypeDef](./type_defs.md#pitpolicyruletypedef) 
5. See [:material-code-braces: ReplicationConfigurationReplicatedDiskTypeDef](./type_defs.md#replicationconfigurationreplicateddisktypedef) 
## StartRecoveryRequestRequestTypeDef

```python
# StartRecoveryRequestRequestTypeDef definition

class StartRecoveryRequestRequestTypeDef(TypedDict):
    sourceServers: Sequence[StartRecoveryRequestSourceServerTypeDef],  # (1)
    isDrill: NotRequired[bool],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: StartRecoveryRequestSourceServerTypeDef](./type_defs.md#startrecoveryrequestsourceservertypedef) 
## StartSourceNetworkRecoveryRequestRequestTypeDef

```python
# StartSourceNetworkRecoveryRequestRequestTypeDef definition

class StartSourceNetworkRecoveryRequestRequestTypeDef(TypedDict):
    sourceNetworks: Sequence[StartSourceNetworkRecoveryRequestNetworkEntryTypeDef],  # (1)
    deployAsNew: NotRequired[bool],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: StartSourceNetworkRecoveryRequestNetworkEntryTypeDef](./type_defs.md#startsourcenetworkrecoveryrequestnetworkentrytypedef) 
## CreateLaunchConfigurationTemplateResponseTypeDef

```python
# CreateLaunchConfigurationTemplateResponseTypeDef definition

class CreateLaunchConfigurationTemplateResponseTypeDef(TypedDict):
    launchConfigurationTemplate: LaunchConfigurationTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchConfigurationTemplateTypeDef](./type_defs.md#launchconfigurationtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## UpdateLaunchConfigurationTemplateResponseTypeDef

```python
# UpdateLaunchConfigurationTemplateResponseTypeDef definition

class UpdateLaunchConfigurationTemplateResponseTypeDef(TypedDict):
    launchConfigurationTemplate: LaunchConfigurationTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchConfigurationTemplateTypeDef](./type_defs.md#launchconfigurationtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## DataReplicationInfoTypeDef

```python
# DataReplicationInfoTypeDef definition

class DataReplicationInfoTypeDef(TypedDict):
    dataReplicationError: NotRequired[DataReplicationErrorTypeDef],  # (1)
    dataReplicationInitiation: NotRequired[DataReplicationInitiationTypeDef],  # (2)
    dataReplicationState: NotRequired[DataReplicationStateType],  # (3)
    etaDateTime: NotRequired[str],
    lagDuration: NotRequired[str],
    replicatedDisks: NotRequired[List[DataReplicationInfoReplicatedDiskTypeDef]],  # (4)
    stagingAvailabilityZone: NotRequired[str],
    stagingOutpostArn: NotRequired[str],
```

1. See [:material-code-braces: DataReplicationErrorTypeDef](./type_defs.md#datareplicationerrortypedef) 
2. See [:material-code-braces: DataReplicationInitiationTypeDef](./type_defs.md#datareplicationinitiationtypedef) 
3. See [:material-code-brackets: DataReplicationStateType](./literals.md#datareplicationstatetype) 
4. See [:material-code-braces: DataReplicationInfoReplicatedDiskTypeDef](./type_defs.md#datareplicationinforeplicateddisktypedef) 
## JobLogEventDataTypeDef

```python
# JobLogEventDataTypeDef definition

class JobLogEventDataTypeDef(TypedDict):
    conversionProperties: NotRequired[ConversionPropertiesTypeDef],  # (1)
    conversionServerID: NotRequired[str],
    eventResourceData: NotRequired[EventResourceDataTypeDef],  # (2)
    rawError: NotRequired[str],
    sourceServerID: NotRequired[str],
    targetInstanceID: NotRequired[str],
```

1. See [:material-code-braces: ConversionPropertiesTypeDef](./type_defs.md#conversionpropertiestypedef) 
2. See [:material-code-braces: EventResourceDataTypeDef](./type_defs.md#eventresourcedatatypedef) 
## LaunchActionRunTypeDef

```python
# LaunchActionRunTypeDef definition

class LaunchActionRunTypeDef(TypedDict):
    action: NotRequired[LaunchActionTypeDef],  # (1)
    failureReason: NotRequired[str],
    runId: NotRequired[str],
    status: NotRequired[LaunchActionRunStatusType],  # (2)
```

1. See [:material-code-braces: LaunchActionTypeDef](./type_defs.md#launchactiontypedef) 
2. See [:material-code-brackets: LaunchActionRunStatusType](./literals.md#launchactionrunstatustype) 
## ListLaunchActionsResponseTypeDef

```python
# ListLaunchActionsResponseTypeDef definition

class ListLaunchActionsResponseTypeDef(TypedDict):
    items: List[LaunchActionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LaunchActionTypeDef](./type_defs.md#launchactiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LifeCycleTypeDef

```python
# LifeCycleTypeDef definition

class LifeCycleTypeDef(TypedDict):
    addedToServiceDateTime: NotRequired[str],
    elapsedReplicationDuration: NotRequired[str],
    firstByteDateTime: NotRequired[str],
    lastLaunch: NotRequired[LifeCycleLastLaunchTypeDef],  # (1)
    lastSeenByServiceDateTime: NotRequired[str],
```

1. See [:material-code-braces: LifeCycleLastLaunchTypeDef](./type_defs.md#lifecyclelastlaunchtypedef) 
## RecoveryInstanceDataReplicationInfoTypeDef

```python
# RecoveryInstanceDataReplicationInfoTypeDef definition

class RecoveryInstanceDataReplicationInfoTypeDef(TypedDict):
    dataReplicationError: NotRequired[RecoveryInstanceDataReplicationErrorTypeDef],  # (1)
    dataReplicationInitiation: NotRequired[RecoveryInstanceDataReplicationInitiationTypeDef],  # (2)
    dataReplicationState: NotRequired[RecoveryInstanceDataReplicationStateType],  # (3)
    etaDateTime: NotRequired[str],
    lagDuration: NotRequired[str],
    replicatedDisks: NotRequired[List[RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef]],  # (4)
    stagingAvailabilityZone: NotRequired[str],
    stagingOutpostArn: NotRequired[str],
```

1. See [:material-code-braces: RecoveryInstanceDataReplicationErrorTypeDef](./type_defs.md#recoveryinstancedatareplicationerrortypedef) 
2. See [:material-code-braces: RecoveryInstanceDataReplicationInitiationTypeDef](./type_defs.md#recoveryinstancedatareplicationinitiationtypedef) 
3. See [:material-code-brackets: RecoveryInstanceDataReplicationStateType](./literals.md#recoveryinstancedatareplicationstatetype) 
4. See [:material-code-braces: RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef](./type_defs.md#recoveryinstancedatareplicationinforeplicateddisktypedef) 
## DescribeSourceNetworksResponseTypeDef

```python
# DescribeSourceNetworksResponseTypeDef definition

class DescribeSourceNetworksResponseTypeDef(TypedDict):
    items: List[SourceNetworkTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SourceNetworkTypeDef](./type_defs.md#sourcenetworktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSourceNetworkReplicationResponseTypeDef

```python
# StartSourceNetworkReplicationResponseTypeDef definition

class StartSourceNetworkReplicationResponseTypeDef(TypedDict):
    sourceNetwork: SourceNetworkTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SourceNetworkTypeDef](./type_defs.md#sourcenetworktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopSourceNetworkReplicationResponseTypeDef

```python
# StopSourceNetworkReplicationResponseTypeDef definition

class StopSourceNetworkReplicationResponseTypeDef(TypedDict):
    sourceNetwork: SourceNetworkTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SourceNetworkTypeDef](./type_defs.md#sourcenetworktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## LaunchActionsStatusTypeDef

```python
# LaunchActionsStatusTypeDef definition

class LaunchActionsStatusTypeDef(TypedDict):
    runs: NotRequired[List[LaunchActionRunTypeDef]],  # (1)
    ssmAgentDiscoveryDatetime: NotRequired[str],
```

1. See [:material-code-braces: LaunchActionRunTypeDef](./type_defs.md#launchactionruntypedef) 
## SourceServerResponseTypeDef

```python
# SourceServerResponseTypeDef definition

class SourceServerResponseTypeDef(TypedDict):
    agentVersion: str,
    arn: str,
    dataReplicationInfo: DataReplicationInfoTypeDef,  # (1)
    lastLaunchResult: LastLaunchResultType,  # (2)
    lifeCycle: LifeCycleTypeDef,  # (3)
    recoveryInstanceId: str,
    replicationDirection: ReplicationDirectionType,  # (4)
    reversedDirectionSourceServerArn: str,
    sourceCloudProperties: SourceCloudPropertiesTypeDef,  # (5)
    sourceNetworkID: str,
    sourceProperties: SourcePropertiesTypeDef,  # (6)
    sourceServerID: str,
    stagingArea: StagingAreaTypeDef,  # (7)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-braces: DataReplicationInfoTypeDef](./type_defs.md#datareplicationinfotypedef) 
2. See [:material-code-brackets: LastLaunchResultType](./literals.md#lastlaunchresulttype) 
3. See [:material-code-braces: LifeCycleTypeDef](./type_defs.md#lifecycletypedef) 
4. See [:material-code-brackets: ReplicationDirectionType](./literals.md#replicationdirectiontype) 
5. See [:material-code-braces: SourceCloudPropertiesTypeDef](./type_defs.md#sourcecloudpropertiestypedef) 
6. See [:material-code-braces: SourcePropertiesTypeDef](./type_defs.md#sourcepropertiestypedef) 
7. See [:material-code-braces: StagingAreaTypeDef](./type_defs.md#stagingareatypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SourceServerTypeDef

```python
# SourceServerTypeDef definition

class SourceServerTypeDef(TypedDict):
    agentVersion: NotRequired[str],
    arn: NotRequired[str],
    dataReplicationInfo: NotRequired[DataReplicationInfoTypeDef],  # (1)
    lastLaunchResult: NotRequired[LastLaunchResultType],  # (2)
    lifeCycle: NotRequired[LifeCycleTypeDef],  # (3)
    recoveryInstanceId: NotRequired[str],
    replicationDirection: NotRequired[ReplicationDirectionType],  # (4)
    reversedDirectionSourceServerArn: NotRequired[str],
    sourceCloudProperties: NotRequired[SourceCloudPropertiesTypeDef],  # (5)
    sourceNetworkID: NotRequired[str],
    sourceProperties: NotRequired[SourcePropertiesTypeDef],  # (6)
    sourceServerID: NotRequired[str],
    stagingArea: NotRequired[StagingAreaTypeDef],  # (7)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: DataReplicationInfoTypeDef](./type_defs.md#datareplicationinfotypedef) 
2. See [:material-code-brackets: LastLaunchResultType](./literals.md#lastlaunchresulttype) 
3. See [:material-code-braces: LifeCycleTypeDef](./type_defs.md#lifecycletypedef) 
4. See [:material-code-brackets: ReplicationDirectionType](./literals.md#replicationdirectiontype) 
5. See [:material-code-braces: SourceCloudPropertiesTypeDef](./type_defs.md#sourcecloudpropertiestypedef) 
6. See [:material-code-braces: SourcePropertiesTypeDef](./type_defs.md#sourcepropertiestypedef) 
7. See [:material-code-braces: StagingAreaTypeDef](./type_defs.md#stagingareatypedef) 
## RecoveryInstanceTypeDef

```python
# RecoveryInstanceTypeDef definition

class RecoveryInstanceTypeDef(TypedDict):
    agentVersion: NotRequired[str],
    arn: NotRequired[str],
    dataReplicationInfo: NotRequired[RecoveryInstanceDataReplicationInfoTypeDef],  # (1)
    ec2InstanceID: NotRequired[str],
    ec2InstanceState: NotRequired[EC2InstanceStateType],  # (2)
    failback: NotRequired[RecoveryInstanceFailbackTypeDef],  # (3)
    isDrill: NotRequired[bool],
    jobID: NotRequired[str],
    originAvailabilityZone: NotRequired[str],
    originEnvironment: NotRequired[OriginEnvironmentType],  # (4)
    pointInTimeSnapshotDateTime: NotRequired[str],
    recoveryInstanceID: NotRequired[str],
    recoveryInstanceProperties: NotRequired[RecoveryInstancePropertiesTypeDef],  # (5)
    sourceOutpostArn: NotRequired[str],
    sourceServerID: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: RecoveryInstanceDataReplicationInfoTypeDef](./type_defs.md#recoveryinstancedatareplicationinfotypedef) 
2. See [:material-code-brackets: EC2InstanceStateType](./literals.md#ec2instancestatetype) 
3. See [:material-code-braces: RecoveryInstanceFailbackTypeDef](./type_defs.md#recoveryinstancefailbacktypedef) 
4. See [:material-code-brackets: OriginEnvironmentType](./literals.md#originenvironmenttype) 
5. See [:material-code-braces: RecoveryInstancePropertiesTypeDef](./type_defs.md#recoveryinstancepropertiestypedef) 
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
## ParticipatingServerTypeDef

```python
# ParticipatingServerTypeDef definition

class ParticipatingServerTypeDef(TypedDict):
    launchActionsStatus: NotRequired[LaunchActionsStatusTypeDef],  # (1)
    launchStatus: NotRequired[LaunchStatusType],  # (2)
    recoveryInstanceID: NotRequired[str],
    sourceServerID: NotRequired[str],
```

1. See [:material-code-braces: LaunchActionsStatusTypeDef](./type_defs.md#launchactionsstatustypedef) 
2. See [:material-code-brackets: LaunchStatusType](./literals.md#launchstatustype) 
## CreateExtendedSourceServerResponseTypeDef

```python
# CreateExtendedSourceServerResponseTypeDef definition

class CreateExtendedSourceServerResponseTypeDef(TypedDict):
    sourceServer: SourceServerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SourceServerTypeDef](./type_defs.md#sourceservertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## StartReplicationResponseTypeDef

```python
# StartReplicationResponseTypeDef definition

class StartReplicationResponseTypeDef(TypedDict):
    sourceServer: SourceServerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SourceServerTypeDef](./type_defs.md#sourceservertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopReplicationResponseTypeDef

```python
# StopReplicationResponseTypeDef definition

class StopReplicationResponseTypeDef(TypedDict):
    sourceServer: SourceServerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SourceServerTypeDef](./type_defs.md#sourceservertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRecoveryInstancesResponseTypeDef

```python
# DescribeRecoveryInstancesResponseTypeDef definition

class DescribeRecoveryInstancesResponseTypeDef(TypedDict):
    items: List[RecoveryInstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RecoveryInstanceTypeDef](./type_defs.md#recoveryinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JobTypeDef

```python
# JobTypeDef definition

class JobTypeDef(TypedDict):
    jobID: str,
    arn: NotRequired[str],
    creationDateTime: NotRequired[str],
    endDateTime: NotRequired[str],
    initiatedBy: NotRequired[InitiatedByType],  # (1)
    participatingResources: NotRequired[List[ParticipatingResourceTypeDef]],  # (2)
    participatingServers: NotRequired[List[ParticipatingServerTypeDef]],  # (3)
    status: NotRequired[JobStatusType],  # (4)
    tags: NotRequired[Dict[str, str]],
    type: NotRequired[JobTypeType],  # (5)
```

1. See [:material-code-brackets: InitiatedByType](./literals.md#initiatedbytype) 
2. See [:material-code-braces: ParticipatingResourceTypeDef](./type_defs.md#participatingresourcetypedef) 
3. See [:material-code-braces: ParticipatingServerTypeDef](./type_defs.md#participatingservertypedef) 
4. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
5. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
## AssociateSourceNetworkStackResponseTypeDef

```python
# AssociateSourceNetworkStackResponseTypeDef definition

class AssociateSourceNetworkStackResponseTypeDef(TypedDict):
    job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## StartFailbackLaunchResponseTypeDef

```python
# StartFailbackLaunchResponseTypeDef definition

class StartFailbackLaunchResponseTypeDef(TypedDict):
    job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartRecoveryResponseTypeDef

```python
# StartRecoveryResponseTypeDef definition

class StartRecoveryResponseTypeDef(TypedDict):
    job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSourceNetworkRecoveryResponseTypeDef

```python
# StartSourceNetworkRecoveryResponseTypeDef definition

class StartSourceNetworkRecoveryResponseTypeDef(TypedDict):
    job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TerminateRecoveryInstancesResponseTypeDef

```python
# TerminateRecoveryInstancesResponseTypeDef definition

class TerminateRecoveryInstancesResponseTypeDef(TypedDict):
    job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
