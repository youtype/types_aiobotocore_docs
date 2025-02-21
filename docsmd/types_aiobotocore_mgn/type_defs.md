# Type definitions

> [Index](../README.md) > [Mgn](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Mgn](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
    type annotations stubs module [types-aiobotocore-mgn](https://pypi.org/project/types-aiobotocore-mgn/).

## PostLaunchActionsUnionTypeDef

```python
# PostLaunchActionsUnionTypeDef Union usage example

from types_aiobotocore_mgn.type_defs import PostLaunchActionsUnionTypeDef


def get_value() -> PostLaunchActionsUnionTypeDef:
    return ...


# PostLaunchActionsUnionTypeDef definition

PostLaunchActionsUnionTypeDef = Union[
    PostLaunchActionsTypeDef,  # (1)
    PostLaunchActionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PostLaunchActionsTypeDef](./type_defs.md#postlaunchactionstypedef) 
2. See [:material-code-braces: PostLaunchActionsOutputTypeDef](./type_defs.md#postlaunchactionsoutputtypedef) 



## ApplicationAggregatedStatusTypeDef

```python
# ApplicationAggregatedStatusTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ApplicationAggregatedStatusTypeDef


def get_value() -> ApplicationAggregatedStatusTypeDef:
    return {
        "healthStatus": ...,
    }


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
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## ArchiveApplicationRequestTypeDef

```python
# ArchiveApplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ArchiveApplicationRequestTypeDef


def get_value() -> ArchiveApplicationRequestTypeDef:
    return {
        "applicationID": ...,
    }


# ArchiveApplicationRequestTypeDef definition

class ArchiveApplicationRequestTypeDef(TypedDict):
    applicationID: str,
    accountID: NotRequired[str],
```

## ArchiveWaveRequestTypeDef

```python
# ArchiveWaveRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ArchiveWaveRequestTypeDef


def get_value() -> ArchiveWaveRequestTypeDef:
    return {
        "waveID": ...,
    }


# ArchiveWaveRequestTypeDef definition

class ArchiveWaveRequestTypeDef(TypedDict):
    waveID: str,
    accountID: NotRequired[str],
```

## AssociateApplicationsRequestTypeDef

```python
# AssociateApplicationsRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import AssociateApplicationsRequestTypeDef


def get_value() -> AssociateApplicationsRequestTypeDef:
    return {
        "applicationIDs": ...,
    }


# AssociateApplicationsRequestTypeDef definition

class AssociateApplicationsRequestTypeDef(TypedDict):
    applicationIDs: Sequence[str],
    waveID: str,
    accountID: NotRequired[str],
```

## AssociateSourceServersRequestTypeDef

```python
# AssociateSourceServersRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import AssociateSourceServersRequestTypeDef


def get_value() -> AssociateSourceServersRequestTypeDef:
    return {
        "applicationID": ...,
    }


# AssociateSourceServersRequestTypeDef definition

class AssociateSourceServersRequestTypeDef(TypedDict):
    applicationID: str,
    sourceServerIDs: Sequence[str],
    accountID: NotRequired[str],
```

## CPUTypeDef

```python
# CPUTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import CPUTypeDef


def get_value() -> CPUTypeDef:
    return {
        "cores": ...,
    }


# CPUTypeDef definition

class CPUTypeDef(TypedDict):
    cores: NotRequired[int],
    modelName: NotRequired[str],
```

## ChangeServerLifeCycleStateSourceServerLifecycleTypeDef

```python
# ChangeServerLifeCycleStateSourceServerLifecycleTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ChangeServerLifeCycleStateSourceServerLifecycleTypeDef


def get_value() -> ChangeServerLifeCycleStateSourceServerLifecycleTypeDef:
    return {
        "state": ...,
    }


# ChangeServerLifeCycleStateSourceServerLifecycleTypeDef definition

class ChangeServerLifeCycleStateSourceServerLifecycleTypeDef(TypedDict):
    state: ChangeServerLifeCycleStateSourceServerLifecycleStateType,  # (1)
```

1. See [:material-code-brackets: ChangeServerLifeCycleStateSourceServerLifecycleStateType](./literals.md#changeserverlifecyclestatesourceserverlifecyclestatetype) 
## ConnectorSsmCommandConfigTypeDef

```python
# ConnectorSsmCommandConfigTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ConnectorSsmCommandConfigTypeDef


def get_value() -> ConnectorSsmCommandConfigTypeDef:
    return {
        "cloudWatchLogGroupName": ...,
    }


# ConnectorSsmCommandConfigTypeDef definition

class ConnectorSsmCommandConfigTypeDef(TypedDict):
    cloudWatchOutputEnabled: bool,
    s3OutputEnabled: bool,
    cloudWatchLogGroupName: NotRequired[str],
    outputS3BucketName: NotRequired[str],
```

## CreateApplicationRequestTypeDef

```python
# CreateApplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import CreateApplicationRequestTypeDef


def get_value() -> CreateApplicationRequestTypeDef:
    return {
        "name": ...,
    }


# CreateApplicationRequestTypeDef definition

class CreateApplicationRequestTypeDef(TypedDict):
    name: str,
    accountID: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## LaunchTemplateDiskConfTypeDef

```python
# LaunchTemplateDiskConfTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import LaunchTemplateDiskConfTypeDef


def get_value() -> LaunchTemplateDiskConfTypeDef:
    return {
        "iops": ...,
    }


# LaunchTemplateDiskConfTypeDef definition

class LaunchTemplateDiskConfTypeDef(TypedDict):
    iops: NotRequired[int],
    throughput: NotRequired[int],
    volumeType: NotRequired[VolumeTypeType],  # (1)
```

1. See [:material-code-brackets: VolumeTypeType](./literals.md#volumetypetype) 
## LicensingTypeDef

```python
# LicensingTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import LicensingTypeDef


def get_value() -> LicensingTypeDef:
    return {
        "osByol": ...,
    }


# LicensingTypeDef definition

class LicensingTypeDef(TypedDict):
    osByol: NotRequired[bool],
```

## CreateReplicationConfigurationTemplateRequestTypeDef

```python
# CreateReplicationConfigurationTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import CreateReplicationConfigurationTemplateRequestTypeDef


def get_value() -> CreateReplicationConfigurationTemplateRequestTypeDef:
    return {
        "associateDefaultSecurityGroup": ...,
    }


# CreateReplicationConfigurationTemplateRequestTypeDef definition

class CreateReplicationConfigurationTemplateRequestTypeDef(TypedDict):
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
## CreateWaveRequestTypeDef

```python
# CreateWaveRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import CreateWaveRequestTypeDef


def get_value() -> CreateWaveRequestTypeDef:
    return {
        "name": ...,
    }


# CreateWaveRequestTypeDef definition

class CreateWaveRequestTypeDef(TypedDict):
    name: str,
    accountID: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## DataReplicationErrorTypeDef

```python
# DataReplicationErrorTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DataReplicationErrorTypeDef


def get_value() -> DataReplicationErrorTypeDef:
    return {
        "error": ...,
    }


# DataReplicationErrorTypeDef definition

class DataReplicationErrorTypeDef(TypedDict):
    error: NotRequired[DataReplicationErrorStringType],  # (1)
    rawError: NotRequired[str],
```

1. See [:material-code-brackets: DataReplicationErrorStringType](./literals.md#datareplicationerrorstringtype) 
## DataReplicationInfoReplicatedDiskTypeDef

```python
# DataReplicationInfoReplicatedDiskTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DataReplicationInfoReplicatedDiskTypeDef


def get_value() -> DataReplicationInfoReplicatedDiskTypeDef:
    return {
        "backloggedStorageBytes": ...,
    }


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
# DataReplicationInitiationStepTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DataReplicationInitiationStepTypeDef


def get_value() -> DataReplicationInitiationStepTypeDef:
    return {
        "name": ...,
    }


# DataReplicationInitiationStepTypeDef definition

class DataReplicationInitiationStepTypeDef(TypedDict):
    name: NotRequired[DataReplicationInitiationStepNameType],  # (1)
    status: NotRequired[DataReplicationInitiationStepStatusType],  # (2)
```

1. See [:material-code-brackets: DataReplicationInitiationStepNameType](./literals.md#datareplicationinitiationstepnametype) 
2. See [:material-code-brackets: DataReplicationInitiationStepStatusType](./literals.md#datareplicationinitiationstepstatustype) 
## DeleteApplicationRequestTypeDef

```python
# DeleteApplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DeleteApplicationRequestTypeDef


def get_value() -> DeleteApplicationRequestTypeDef:
    return {
        "applicationID": ...,
    }


# DeleteApplicationRequestTypeDef definition

class DeleteApplicationRequestTypeDef(TypedDict):
    applicationID: str,
    accountID: NotRequired[str],
```

## DeleteConnectorRequestTypeDef

```python
# DeleteConnectorRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DeleteConnectorRequestTypeDef


def get_value() -> DeleteConnectorRequestTypeDef:
    return {
        "connectorID": ...,
    }


# DeleteConnectorRequestTypeDef definition

class DeleteConnectorRequestTypeDef(TypedDict):
    connectorID: str,
```

## DeleteJobRequestTypeDef

```python
# DeleteJobRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DeleteJobRequestTypeDef


def get_value() -> DeleteJobRequestTypeDef:
    return {
        "jobID": ...,
    }


# DeleteJobRequestTypeDef definition

class DeleteJobRequestTypeDef(TypedDict):
    jobID: str,
    accountID: NotRequired[str],
```

## DeleteLaunchConfigurationTemplateRequestTypeDef

```python
# DeleteLaunchConfigurationTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DeleteLaunchConfigurationTemplateRequestTypeDef


def get_value() -> DeleteLaunchConfigurationTemplateRequestTypeDef:
    return {
        "launchConfigurationTemplateID": ...,
    }


# DeleteLaunchConfigurationTemplateRequestTypeDef definition

class DeleteLaunchConfigurationTemplateRequestTypeDef(TypedDict):
    launchConfigurationTemplateID: str,
```

## DeleteReplicationConfigurationTemplateRequestTypeDef

```python
# DeleteReplicationConfigurationTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DeleteReplicationConfigurationTemplateRequestTypeDef


def get_value() -> DeleteReplicationConfigurationTemplateRequestTypeDef:
    return {
        "replicationConfigurationTemplateID": ...,
    }


# DeleteReplicationConfigurationTemplateRequestTypeDef definition

class DeleteReplicationConfigurationTemplateRequestTypeDef(TypedDict):
    replicationConfigurationTemplateID: str,
```

## DeleteSourceServerRequestTypeDef

```python
# DeleteSourceServerRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DeleteSourceServerRequestTypeDef


def get_value() -> DeleteSourceServerRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# DeleteSourceServerRequestTypeDef definition

class DeleteSourceServerRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
```

## DeleteVcenterClientRequestTypeDef

```python
# DeleteVcenterClientRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DeleteVcenterClientRequestTypeDef


def get_value() -> DeleteVcenterClientRequestTypeDef:
    return {
        "vcenterClientID": ...,
    }


# DeleteVcenterClientRequestTypeDef definition

class DeleteVcenterClientRequestTypeDef(TypedDict):
    vcenterClientID: str,
```

## DeleteWaveRequestTypeDef

```python
# DeleteWaveRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DeleteWaveRequestTypeDef


def get_value() -> DeleteWaveRequestTypeDef:
    return {
        "waveID": ...,
    }


# DeleteWaveRequestTypeDef definition

class DeleteWaveRequestTypeDef(TypedDict):
    waveID: str,
    accountID: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeJobLogItemsRequestTypeDef

```python
# DescribeJobLogItemsRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeJobLogItemsRequestTypeDef


def get_value() -> DescribeJobLogItemsRequestTypeDef:
    return {
        "jobID": ...,
    }


# DescribeJobLogItemsRequestTypeDef definition

class DescribeJobLogItemsRequestTypeDef(TypedDict):
    jobID: str,
    accountID: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## DescribeJobsRequestFiltersTypeDef

```python
# DescribeJobsRequestFiltersTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeJobsRequestFiltersTypeDef


def get_value() -> DescribeJobsRequestFiltersTypeDef:
    return {
        "fromDate": ...,
    }


# DescribeJobsRequestFiltersTypeDef definition

class DescribeJobsRequestFiltersTypeDef(TypedDict):
    fromDate: NotRequired[str],
    jobIDs: NotRequired[Sequence[str]],
    toDate: NotRequired[str],
```

## DescribeLaunchConfigurationTemplatesRequestTypeDef

```python
# DescribeLaunchConfigurationTemplatesRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeLaunchConfigurationTemplatesRequestTypeDef


def get_value() -> DescribeLaunchConfigurationTemplatesRequestTypeDef:
    return {
        "launchConfigurationTemplateIDs": ...,
    }


# DescribeLaunchConfigurationTemplatesRequestTypeDef definition

class DescribeLaunchConfigurationTemplatesRequestTypeDef(TypedDict):
    launchConfigurationTemplateIDs: NotRequired[Sequence[str]],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## DescribeReplicationConfigurationTemplatesRequestTypeDef

```python
# DescribeReplicationConfigurationTemplatesRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeReplicationConfigurationTemplatesRequestTypeDef


def get_value() -> DescribeReplicationConfigurationTemplatesRequestTypeDef:
    return {
        "maxResults": ...,
    }


# DescribeReplicationConfigurationTemplatesRequestTypeDef definition

class DescribeReplicationConfigurationTemplatesRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    replicationConfigurationTemplateIDs: NotRequired[Sequence[str]],
```

## ReplicationConfigurationTemplateTypeDef

```python
# ReplicationConfigurationTemplateTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ReplicationConfigurationTemplateTypeDef


def get_value() -> ReplicationConfigurationTemplateTypeDef:
    return {
        "arn": ...,
    }


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
# DescribeSourceServersRequestFiltersTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeSourceServersRequestFiltersTypeDef


def get_value() -> DescribeSourceServersRequestFiltersTypeDef:
    return {
        "applicationIDs": ...,
    }


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
## DescribeVcenterClientsRequestTypeDef

```python
# DescribeVcenterClientsRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeVcenterClientsRequestTypeDef


def get_value() -> DescribeVcenterClientsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# DescribeVcenterClientsRequestTypeDef definition

class DescribeVcenterClientsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## VcenterClientTypeDef

```python
# VcenterClientTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import VcenterClientTypeDef


def get_value() -> VcenterClientTypeDef:
    return {
        "arn": ...,
    }


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

## DisassociateApplicationsRequestTypeDef

```python
# DisassociateApplicationsRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DisassociateApplicationsRequestTypeDef


def get_value() -> DisassociateApplicationsRequestTypeDef:
    return {
        "applicationIDs": ...,
    }


# DisassociateApplicationsRequestTypeDef definition

class DisassociateApplicationsRequestTypeDef(TypedDict):
    applicationIDs: Sequence[str],
    waveID: str,
    accountID: NotRequired[str],
```

## DisassociateSourceServersRequestTypeDef

```python
# DisassociateSourceServersRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DisassociateSourceServersRequestTypeDef


def get_value() -> DisassociateSourceServersRequestTypeDef:
    return {
        "applicationID": ...,
    }


# DisassociateSourceServersRequestTypeDef definition

class DisassociateSourceServersRequestTypeDef(TypedDict):
    applicationID: str,
    sourceServerIDs: Sequence[str],
    accountID: NotRequired[str],
```

## DisconnectFromServiceRequestTypeDef

```python
# DisconnectFromServiceRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DisconnectFromServiceRequestTypeDef


def get_value() -> DisconnectFromServiceRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# DisconnectFromServiceRequestTypeDef definition

class DisconnectFromServiceRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
```

## DiskTypeDef

```python
# DiskTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DiskTypeDef


def get_value() -> DiskTypeDef:
    return {
        "bytes": ...,
    }


# DiskTypeDef definition

class DiskTypeDef(TypedDict):
    bytes: NotRequired[int],
    deviceName: NotRequired[str],
```

## ExportErrorDataTypeDef

```python
# ExportErrorDataTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ExportErrorDataTypeDef


def get_value() -> ExportErrorDataTypeDef:
    return {
        "rawError": ...,
    }


# ExportErrorDataTypeDef definition

class ExportErrorDataTypeDef(TypedDict):
    rawError: NotRequired[str],
```

## ExportTaskSummaryTypeDef

```python
# ExportTaskSummaryTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ExportTaskSummaryTypeDef


def get_value() -> ExportTaskSummaryTypeDef:
    return {
        "applicationsCount": ...,
    }


# ExportTaskSummaryTypeDef definition

class ExportTaskSummaryTypeDef(TypedDict):
    applicationsCount: NotRequired[int],
    serversCount: NotRequired[int],
    wavesCount: NotRequired[int],
```

## FinalizeCutoverRequestTypeDef

```python
# FinalizeCutoverRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import FinalizeCutoverRequestTypeDef


def get_value() -> FinalizeCutoverRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# FinalizeCutoverRequestTypeDef definition

class FinalizeCutoverRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
```

## GetLaunchConfigurationRequestTypeDef

```python
# GetLaunchConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import GetLaunchConfigurationRequestTypeDef


def get_value() -> GetLaunchConfigurationRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# GetLaunchConfigurationRequestTypeDef definition

class GetLaunchConfigurationRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
```

## GetReplicationConfigurationRequestTypeDef

```python
# GetReplicationConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import GetReplicationConfigurationRequestTypeDef


def get_value() -> GetReplicationConfigurationRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# GetReplicationConfigurationRequestTypeDef definition

class GetReplicationConfigurationRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
```

## IdentificationHintsTypeDef

```python
# IdentificationHintsTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import IdentificationHintsTypeDef


def get_value() -> IdentificationHintsTypeDef:
    return {
        "awsInstanceID": ...,
    }


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
# ImportErrorDataTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ImportErrorDataTypeDef


def get_value() -> ImportErrorDataTypeDef:
    return {
        "accountID": ...,
    }


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
# ImportTaskSummaryApplicationsTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ImportTaskSummaryApplicationsTypeDef


def get_value() -> ImportTaskSummaryApplicationsTypeDef:
    return {
        "createdCount": ...,
    }


# ImportTaskSummaryApplicationsTypeDef definition

class ImportTaskSummaryApplicationsTypeDef(TypedDict):
    createdCount: NotRequired[int],
    modifiedCount: NotRequired[int],
```

## ImportTaskSummaryServersTypeDef

```python
# ImportTaskSummaryServersTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ImportTaskSummaryServersTypeDef


def get_value() -> ImportTaskSummaryServersTypeDef:
    return {
        "createdCount": ...,
    }


# ImportTaskSummaryServersTypeDef definition

class ImportTaskSummaryServersTypeDef(TypedDict):
    createdCount: NotRequired[int],
    modifiedCount: NotRequired[int],
```

## ImportTaskSummaryWavesTypeDef

```python
# ImportTaskSummaryWavesTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ImportTaskSummaryWavesTypeDef


def get_value() -> ImportTaskSummaryWavesTypeDef:
    return {
        "createdCount": ...,
    }


# ImportTaskSummaryWavesTypeDef definition

class ImportTaskSummaryWavesTypeDef(TypedDict):
    createdCount: NotRequired[int],
    modifiedCount: NotRequired[int],
```

## S3BucketSourceTypeDef

```python
# S3BucketSourceTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import S3BucketSourceTypeDef


def get_value() -> S3BucketSourceTypeDef:
    return {
        "s3Bucket": ...,
    }


# S3BucketSourceTypeDef definition

class S3BucketSourceTypeDef(TypedDict):
    s3Bucket: str,
    s3Key: str,
    s3BucketOwner: NotRequired[str],
```

## JobLogEventDataTypeDef

```python
# JobLogEventDataTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import JobLogEventDataTypeDef


def get_value() -> JobLogEventDataTypeDef:
    return {
        "conversionServerID": ...,
    }


# JobLogEventDataTypeDef definition

class JobLogEventDataTypeDef(TypedDict):
    conversionServerID: NotRequired[str],
    rawError: NotRequired[str],
    sourceServerID: NotRequired[str],
    targetInstanceID: NotRequired[str],
```

## LaunchedInstanceTypeDef

```python
# LaunchedInstanceTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import LaunchedInstanceTypeDef


def get_value() -> LaunchedInstanceTypeDef:
    return {
        "ec2InstanceID": ...,
    }


# LaunchedInstanceTypeDef definition

class LaunchedInstanceTypeDef(TypedDict):
    ec2InstanceID: NotRequired[str],
    firstBoot: NotRequired[FirstBootType],  # (1)
    jobID: NotRequired[str],
```

1. See [:material-code-brackets: FirstBootType](./literals.md#firstboottype) 
## LifeCycleLastCutoverFinalizedTypeDef

```python
# LifeCycleLastCutoverFinalizedTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import LifeCycleLastCutoverFinalizedTypeDef


def get_value() -> LifeCycleLastCutoverFinalizedTypeDef:
    return {
        "apiCallDateTime": ...,
    }


# LifeCycleLastCutoverFinalizedTypeDef definition

class LifeCycleLastCutoverFinalizedTypeDef(TypedDict):
    apiCallDateTime: NotRequired[str],
```

## LifeCycleLastCutoverInitiatedTypeDef

```python
# LifeCycleLastCutoverInitiatedTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import LifeCycleLastCutoverInitiatedTypeDef


def get_value() -> LifeCycleLastCutoverInitiatedTypeDef:
    return {
        "apiCallDateTime": ...,
    }


# LifeCycleLastCutoverInitiatedTypeDef definition

class LifeCycleLastCutoverInitiatedTypeDef(TypedDict):
    apiCallDateTime: NotRequired[str],
    jobID: NotRequired[str],
```

## LifeCycleLastCutoverRevertedTypeDef

```python
# LifeCycleLastCutoverRevertedTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import LifeCycleLastCutoverRevertedTypeDef


def get_value() -> LifeCycleLastCutoverRevertedTypeDef:
    return {
        "apiCallDateTime": ...,
    }


# LifeCycleLastCutoverRevertedTypeDef definition

class LifeCycleLastCutoverRevertedTypeDef(TypedDict):
    apiCallDateTime: NotRequired[str],
```

## LifeCycleLastTestFinalizedTypeDef

```python
# LifeCycleLastTestFinalizedTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import LifeCycleLastTestFinalizedTypeDef


def get_value() -> LifeCycleLastTestFinalizedTypeDef:
    return {
        "apiCallDateTime": ...,
    }


# LifeCycleLastTestFinalizedTypeDef definition

class LifeCycleLastTestFinalizedTypeDef(TypedDict):
    apiCallDateTime: NotRequired[str],
```

## LifeCycleLastTestInitiatedTypeDef

```python
# LifeCycleLastTestInitiatedTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import LifeCycleLastTestInitiatedTypeDef


def get_value() -> LifeCycleLastTestInitiatedTypeDef:
    return {
        "apiCallDateTime": ...,
    }


# LifeCycleLastTestInitiatedTypeDef definition

class LifeCycleLastTestInitiatedTypeDef(TypedDict):
    apiCallDateTime: NotRequired[str],
    jobID: NotRequired[str],
```

## LifeCycleLastTestRevertedTypeDef

```python
# LifeCycleLastTestRevertedTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import LifeCycleLastTestRevertedTypeDef


def get_value() -> LifeCycleLastTestRevertedTypeDef:
    return {
        "apiCallDateTime": ...,
    }


# LifeCycleLastTestRevertedTypeDef definition

class LifeCycleLastTestRevertedTypeDef(TypedDict):
    apiCallDateTime: NotRequired[str],
```

## ListApplicationsRequestFiltersTypeDef

```python
# ListApplicationsRequestFiltersTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListApplicationsRequestFiltersTypeDef


def get_value() -> ListApplicationsRequestFiltersTypeDef:
    return {
        "applicationIDs": ...,
    }


# ListApplicationsRequestFiltersTypeDef definition

class ListApplicationsRequestFiltersTypeDef(TypedDict):
    applicationIDs: NotRequired[Sequence[str]],
    isArchived: NotRequired[bool],
    waveIDs: NotRequired[Sequence[str]],
```

## ListConnectorsRequestFiltersTypeDef

```python
# ListConnectorsRequestFiltersTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListConnectorsRequestFiltersTypeDef


def get_value() -> ListConnectorsRequestFiltersTypeDef:
    return {
        "connectorIDs": ...,
    }


# ListConnectorsRequestFiltersTypeDef definition

class ListConnectorsRequestFiltersTypeDef(TypedDict):
    connectorIDs: NotRequired[Sequence[str]],
```

## ListExportErrorsRequestTypeDef

```python
# ListExportErrorsRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListExportErrorsRequestTypeDef


def get_value() -> ListExportErrorsRequestTypeDef:
    return {
        "exportID": ...,
    }


# ListExportErrorsRequestTypeDef definition

class ListExportErrorsRequestTypeDef(TypedDict):
    exportID: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListExportsRequestFiltersTypeDef

```python
# ListExportsRequestFiltersTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListExportsRequestFiltersTypeDef


def get_value() -> ListExportsRequestFiltersTypeDef:
    return {
        "exportIDs": ...,
    }


# ListExportsRequestFiltersTypeDef definition

class ListExportsRequestFiltersTypeDef(TypedDict):
    exportIDs: NotRequired[Sequence[str]],
```

## ListImportErrorsRequestTypeDef

```python
# ListImportErrorsRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListImportErrorsRequestTypeDef


def get_value() -> ListImportErrorsRequestTypeDef:
    return {
        "importID": ...,
    }


# ListImportErrorsRequestTypeDef definition

class ListImportErrorsRequestTypeDef(TypedDict):
    importID: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListImportsRequestFiltersTypeDef

```python
# ListImportsRequestFiltersTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListImportsRequestFiltersTypeDef


def get_value() -> ListImportsRequestFiltersTypeDef:
    return {
        "importIDs": ...,
    }


# ListImportsRequestFiltersTypeDef definition

class ListImportsRequestFiltersTypeDef(TypedDict):
    importIDs: NotRequired[Sequence[str]],
```

## ListManagedAccountsRequestTypeDef

```python
# ListManagedAccountsRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListManagedAccountsRequestTypeDef


def get_value() -> ListManagedAccountsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListManagedAccountsRequestTypeDef definition

class ListManagedAccountsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ManagedAccountTypeDef

```python
# ManagedAccountTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ManagedAccountTypeDef


def get_value() -> ManagedAccountTypeDef:
    return {
        "accountId": ...,
    }


# ManagedAccountTypeDef definition

class ManagedAccountTypeDef(TypedDict):
    accountId: NotRequired[str],
```

## SourceServerActionsRequestFiltersTypeDef

```python
# SourceServerActionsRequestFiltersTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import SourceServerActionsRequestFiltersTypeDef


def get_value() -> SourceServerActionsRequestFiltersTypeDef:
    return {
        "actionIDs": ...,
    }


# SourceServerActionsRequestFiltersTypeDef definition

class SourceServerActionsRequestFiltersTypeDef(TypedDict):
    actionIDs: NotRequired[Sequence[str]],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## TemplateActionsRequestFiltersTypeDef

```python
# TemplateActionsRequestFiltersTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import TemplateActionsRequestFiltersTypeDef


def get_value() -> TemplateActionsRequestFiltersTypeDef:
    return {
        "actionIDs": ...,
    }


# TemplateActionsRequestFiltersTypeDef definition

class TemplateActionsRequestFiltersTypeDef(TypedDict):
    actionIDs: NotRequired[Sequence[str]],
```

## ListWavesRequestFiltersTypeDef

```python
# ListWavesRequestFiltersTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListWavesRequestFiltersTypeDef


def get_value() -> ListWavesRequestFiltersTypeDef:
    return {
        "isArchived": ...,
    }


# ListWavesRequestFiltersTypeDef definition

class ListWavesRequestFiltersTypeDef(TypedDict):
    isArchived: NotRequired[bool],
    waveIDs: NotRequired[Sequence[str]],
```

## MarkAsArchivedRequestTypeDef

```python
# MarkAsArchivedRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import MarkAsArchivedRequestTypeDef


def get_value() -> MarkAsArchivedRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# MarkAsArchivedRequestTypeDef definition

class MarkAsArchivedRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
```

## NetworkInterfaceTypeDef

```python
# NetworkInterfaceTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import NetworkInterfaceTypeDef


def get_value() -> NetworkInterfaceTypeDef:
    return {
        "ips": ...,
    }


# NetworkInterfaceTypeDef definition

class NetworkInterfaceTypeDef(TypedDict):
    ips: NotRequired[List[str]],
    isPrimary: NotRequired[bool],
    macAddress: NotRequired[str],
```

## OSTypeDef

```python
# OSTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import OSTypeDef


def get_value() -> OSTypeDef:
    return {
        "fullString": ...,
    }


# OSTypeDef definition

class OSTypeDef(TypedDict):
    fullString: NotRequired[str],
```

## PauseReplicationRequestTypeDef

```python
# PauseReplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import PauseReplicationRequestTypeDef


def get_value() -> PauseReplicationRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# PauseReplicationRequestTypeDef definition

class PauseReplicationRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
```

## SsmExternalParameterTypeDef

```python
# SsmExternalParameterTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import SsmExternalParameterTypeDef


def get_value() -> SsmExternalParameterTypeDef:
    return {
        "dynamicPath": ...,
    }


# SsmExternalParameterTypeDef definition

class SsmExternalParameterTypeDef(TypedDict):
    dynamicPath: NotRequired[str],
```

## SsmParameterStoreParameterTypeDef

```python
# SsmParameterStoreParameterTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import SsmParameterStoreParameterTypeDef


def get_value() -> SsmParameterStoreParameterTypeDef:
    return {
        "parameterName": ...,
    }


# SsmParameterStoreParameterTypeDef definition

class SsmParameterStoreParameterTypeDef(TypedDict):
    parameterName: str,
    parameterType: SsmParameterStoreParameterTypeType,  # (1)
```

1. See [:material-code-brackets: SsmParameterStoreParameterTypeType](./literals.md#ssmparameterstoreparametertypetype) 
## RemoveSourceServerActionRequestTypeDef

```python
# RemoveSourceServerActionRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import RemoveSourceServerActionRequestTypeDef


def get_value() -> RemoveSourceServerActionRequestTypeDef:
    return {
        "actionID": ...,
    }


# RemoveSourceServerActionRequestTypeDef definition

class RemoveSourceServerActionRequestTypeDef(TypedDict):
    actionID: str,
    sourceServerID: str,
    accountID: NotRequired[str],
```

## RemoveTemplateActionRequestTypeDef

```python
# RemoveTemplateActionRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import RemoveTemplateActionRequestTypeDef


def get_value() -> RemoveTemplateActionRequestTypeDef:
    return {
        "actionID": ...,
    }


# RemoveTemplateActionRequestTypeDef definition

class RemoveTemplateActionRequestTypeDef(TypedDict):
    actionID: str,
    launchConfigurationTemplateID: str,
```

## ReplicationConfigurationReplicatedDiskTypeDef

```python
# ReplicationConfigurationReplicatedDiskTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ReplicationConfigurationReplicatedDiskTypeDef


def get_value() -> ReplicationConfigurationReplicatedDiskTypeDef:
    return {
        "deviceName": ...,
    }


# ReplicationConfigurationReplicatedDiskTypeDef definition

class ReplicationConfigurationReplicatedDiskTypeDef(TypedDict):
    deviceName: NotRequired[str],
    iops: NotRequired[int],
    isBootDisk: NotRequired[bool],
    stagingDiskType: NotRequired[ReplicationConfigurationReplicatedDiskStagingDiskTypeType],  # (1)
    throughput: NotRequired[int],
```

1. See [:material-code-brackets: ReplicationConfigurationReplicatedDiskStagingDiskTypeType](./literals.md#replicationconfigurationreplicateddiskstagingdisktypetype) 
## ResumeReplicationRequestTypeDef

```python
# ResumeReplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ResumeReplicationRequestTypeDef


def get_value() -> ResumeReplicationRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# ResumeReplicationRequestTypeDef definition

class ResumeReplicationRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
```

## RetryDataReplicationRequestTypeDef

```python
# RetryDataReplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import RetryDataReplicationRequestTypeDef


def get_value() -> RetryDataReplicationRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# RetryDataReplicationRequestTypeDef definition

class RetryDataReplicationRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
```

## SourceServerConnectorActionTypeDef

```python
# SourceServerConnectorActionTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import SourceServerConnectorActionTypeDef


def get_value() -> SourceServerConnectorActionTypeDef:
    return {
        "connectorArn": ...,
    }


# SourceServerConnectorActionTypeDef definition

class SourceServerConnectorActionTypeDef(TypedDict):
    connectorArn: NotRequired[str],
    credentialsSecretArn: NotRequired[str],
```

## StartCutoverRequestTypeDef

```python
# StartCutoverRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import StartCutoverRequestTypeDef


def get_value() -> StartCutoverRequestTypeDef:
    return {
        "sourceServerIDs": ...,
    }


# StartCutoverRequestTypeDef definition

class StartCutoverRequestTypeDef(TypedDict):
    sourceServerIDs: Sequence[str],
    accountID: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## StartExportRequestTypeDef

```python
# StartExportRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import StartExportRequestTypeDef


def get_value() -> StartExportRequestTypeDef:
    return {
        "s3Bucket": ...,
    }


# StartExportRequestTypeDef definition

class StartExportRequestTypeDef(TypedDict):
    s3Bucket: str,
    s3Key: str,
    s3BucketOwner: NotRequired[str],
```

## StartReplicationRequestTypeDef

```python
# StartReplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import StartReplicationRequestTypeDef


def get_value() -> StartReplicationRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# StartReplicationRequestTypeDef definition

class StartReplicationRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
```

## StartTestRequestTypeDef

```python
# StartTestRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import StartTestRequestTypeDef


def get_value() -> StartTestRequestTypeDef:
    return {
        "sourceServerIDs": ...,
    }


# StartTestRequestTypeDef definition

class StartTestRequestTypeDef(TypedDict):
    sourceServerIDs: Sequence[str],
    accountID: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## StopReplicationRequestTypeDef

```python
# StopReplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import StopReplicationRequestTypeDef


def get_value() -> StopReplicationRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# StopReplicationRequestTypeDef definition

class StopReplicationRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## TerminateTargetInstancesRequestTypeDef

```python
# TerminateTargetInstancesRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import TerminateTargetInstancesRequestTypeDef


def get_value() -> TerminateTargetInstancesRequestTypeDef:
    return {
        "sourceServerIDs": ...,
    }


# TerminateTargetInstancesRequestTypeDef definition

class TerminateTargetInstancesRequestTypeDef(TypedDict):
    sourceServerIDs: Sequence[str],
    accountID: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## UnarchiveApplicationRequestTypeDef

```python
# UnarchiveApplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import UnarchiveApplicationRequestTypeDef


def get_value() -> UnarchiveApplicationRequestTypeDef:
    return {
        "applicationID": ...,
    }


# UnarchiveApplicationRequestTypeDef definition

class UnarchiveApplicationRequestTypeDef(TypedDict):
    applicationID: str,
    accountID: NotRequired[str],
```

## UnarchiveWaveRequestTypeDef

```python
# UnarchiveWaveRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import UnarchiveWaveRequestTypeDef


def get_value() -> UnarchiveWaveRequestTypeDef:
    return {
        "waveID": ...,
    }


# UnarchiveWaveRequestTypeDef definition

class UnarchiveWaveRequestTypeDef(TypedDict):
    waveID: str,
    accountID: NotRequired[str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateApplicationRequestTypeDef

```python
# UpdateApplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import UpdateApplicationRequestTypeDef


def get_value() -> UpdateApplicationRequestTypeDef:
    return {
        "applicationID": ...,
    }


# UpdateApplicationRequestTypeDef definition

class UpdateApplicationRequestTypeDef(TypedDict):
    applicationID: str,
    accountID: NotRequired[str],
    description: NotRequired[str],
    name: NotRequired[str],
```

## UpdateReplicationConfigurationTemplateRequestTypeDef

```python
# UpdateReplicationConfigurationTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import UpdateReplicationConfigurationTemplateRequestTypeDef


def get_value() -> UpdateReplicationConfigurationTemplateRequestTypeDef:
    return {
        "replicationConfigurationTemplateID": ...,
    }


# UpdateReplicationConfigurationTemplateRequestTypeDef definition

class UpdateReplicationConfigurationTemplateRequestTypeDef(TypedDict):
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
## UpdateSourceServerReplicationTypeRequestTypeDef

```python
# UpdateSourceServerReplicationTypeRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import UpdateSourceServerReplicationTypeRequestTypeDef


def get_value() -> UpdateSourceServerReplicationTypeRequestTypeDef:
    return {
        "replicationType": ...,
    }


# UpdateSourceServerReplicationTypeRequestTypeDef definition

class UpdateSourceServerReplicationTypeRequestTypeDef(TypedDict):
    replicationType: ReplicationTypeType,  # (1)
    sourceServerID: str,
    accountID: NotRequired[str],
```

1. See [:material-code-brackets: ReplicationTypeType](./literals.md#replicationtypetype) 
## UpdateWaveRequestTypeDef

```python
# UpdateWaveRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import UpdateWaveRequestTypeDef


def get_value() -> UpdateWaveRequestTypeDef:
    return {
        "waveID": ...,
    }


# UpdateWaveRequestTypeDef definition

class UpdateWaveRequestTypeDef(TypedDict):
    waveID: str,
    accountID: NotRequired[str],
    description: NotRequired[str],
    name: NotRequired[str],
```

## WaveAggregatedStatusTypeDef

```python
# WaveAggregatedStatusTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import WaveAggregatedStatusTypeDef


def get_value() -> WaveAggregatedStatusTypeDef:
    return {
        "healthStatus": ...,
    }


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
# ApplicationTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ApplicationTypeDef


def get_value() -> ApplicationTypeDef:
    return {
        "applicationAggregatedStatus": ...,
    }


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
# ApplicationResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ApplicationResponseTypeDef


def get_value() -> ApplicationResponseTypeDef:
    return {
        "applicationAggregatedStatus": ...,
    }


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
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReplicationConfigurationTemplateResponseTypeDef

```python
# ReplicationConfigurationTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ReplicationConfigurationTemplateResponseTypeDef


def get_value() -> ReplicationConfigurationTemplateResponseTypeDef:
    return {
        "arn": ...,
    }


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
## ChangeServerLifeCycleStateRequestTypeDef

```python
# ChangeServerLifeCycleStateRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ChangeServerLifeCycleStateRequestTypeDef


def get_value() -> ChangeServerLifeCycleStateRequestTypeDef:
    return {
        "lifeCycle": ...,
    }


# ChangeServerLifeCycleStateRequestTypeDef definition

class ChangeServerLifeCycleStateRequestTypeDef(TypedDict):
    lifeCycle: ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,  # (1)
    sourceServerID: str,
    accountID: NotRequired[str],
```

1. See [:material-code-braces: ChangeServerLifeCycleStateSourceServerLifecycleTypeDef](./type_defs.md#changeserverlifecyclestatesourceserverlifecycletypedef) 
## ConnectorResponseTypeDef

```python
# ConnectorResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ConnectorResponseTypeDef


def get_value() -> ConnectorResponseTypeDef:
    return {
        "arn": ...,
    }


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
# ConnectorTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ConnectorTypeDef


def get_value() -> ConnectorTypeDef:
    return {
        "arn": ...,
    }


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
## CreateConnectorRequestTypeDef

```python
# CreateConnectorRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import CreateConnectorRequestTypeDef


def get_value() -> CreateConnectorRequestTypeDef:
    return {
        "name": ...,
    }


# CreateConnectorRequestTypeDef definition

class CreateConnectorRequestTypeDef(TypedDict):
    name: str,
    ssmInstanceID: str,
    ssmCommandConfig: NotRequired[ConnectorSsmCommandConfigTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ConnectorSsmCommandConfigTypeDef](./type_defs.md#connectorssmcommandconfigtypedef) 
## UpdateConnectorRequestTypeDef

```python
# UpdateConnectorRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import UpdateConnectorRequestTypeDef


def get_value() -> UpdateConnectorRequestTypeDef:
    return {
        "connectorID": ...,
    }


# UpdateConnectorRequestTypeDef definition

class UpdateConnectorRequestTypeDef(TypedDict):
    connectorID: str,
    name: NotRequired[str],
    ssmCommandConfig: NotRequired[ConnectorSsmCommandConfigTypeDef],  # (1)
```

1. See [:material-code-braces: ConnectorSsmCommandConfigTypeDef](./type_defs.md#connectorssmcommandconfigtypedef) 
## DataReplicationInitiationTypeDef

```python
# DataReplicationInitiationTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DataReplicationInitiationTypeDef


def get_value() -> DataReplicationInitiationTypeDef:
    return {
        "nextAttemptDateTime": ...,
    }


# DataReplicationInitiationTypeDef definition

class DataReplicationInitiationTypeDef(TypedDict):
    nextAttemptDateTime: NotRequired[str],
    startDateTime: NotRequired[str],
    steps: NotRequired[List[DataReplicationInitiationStepTypeDef]],  # (1)
```

1. See [:material-code-braces: DataReplicationInitiationStepTypeDef](./type_defs.md#datareplicationinitiationsteptypedef) 
## DescribeJobLogItemsRequestPaginateTypeDef

```python
# DescribeJobLogItemsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeJobLogItemsRequestPaginateTypeDef


def get_value() -> DescribeJobLogItemsRequestPaginateTypeDef:
    return {
        "jobID": ...,
    }


# DescribeJobLogItemsRequestPaginateTypeDef definition

class DescribeJobLogItemsRequestPaginateTypeDef(TypedDict):
    jobID: str,
    accountID: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeLaunchConfigurationTemplatesRequestPaginateTypeDef

```python
# DescribeLaunchConfigurationTemplatesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeLaunchConfigurationTemplatesRequestPaginateTypeDef


def get_value() -> DescribeLaunchConfigurationTemplatesRequestPaginateTypeDef:
    return {
        "launchConfigurationTemplateIDs": ...,
    }


# DescribeLaunchConfigurationTemplatesRequestPaginateTypeDef definition

class DescribeLaunchConfigurationTemplatesRequestPaginateTypeDef(TypedDict):
    launchConfigurationTemplateIDs: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeReplicationConfigurationTemplatesRequestPaginateTypeDef

```python
# DescribeReplicationConfigurationTemplatesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeReplicationConfigurationTemplatesRequestPaginateTypeDef


def get_value() -> DescribeReplicationConfigurationTemplatesRequestPaginateTypeDef:
    return {
        "replicationConfigurationTemplateIDs": ...,
    }


# DescribeReplicationConfigurationTemplatesRequestPaginateTypeDef definition

class DescribeReplicationConfigurationTemplatesRequestPaginateTypeDef(TypedDict):
    replicationConfigurationTemplateIDs: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeVcenterClientsRequestPaginateTypeDef

```python
# DescribeVcenterClientsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeVcenterClientsRequestPaginateTypeDef


def get_value() -> DescribeVcenterClientsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# DescribeVcenterClientsRequestPaginateTypeDef definition

class DescribeVcenterClientsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListExportErrorsRequestPaginateTypeDef

```python
# ListExportErrorsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListExportErrorsRequestPaginateTypeDef


def get_value() -> ListExportErrorsRequestPaginateTypeDef:
    return {
        "exportID": ...,
    }


# ListExportErrorsRequestPaginateTypeDef definition

class ListExportErrorsRequestPaginateTypeDef(TypedDict):
    exportID: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListImportErrorsRequestPaginateTypeDef

```python
# ListImportErrorsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListImportErrorsRequestPaginateTypeDef


def get_value() -> ListImportErrorsRequestPaginateTypeDef:
    return {
        "importID": ...,
    }


# ListImportErrorsRequestPaginateTypeDef definition

class ListImportErrorsRequestPaginateTypeDef(TypedDict):
    importID: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListManagedAccountsRequestPaginateTypeDef

```python
# ListManagedAccountsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListManagedAccountsRequestPaginateTypeDef


def get_value() -> ListManagedAccountsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListManagedAccountsRequestPaginateTypeDef definition

class ListManagedAccountsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeJobsRequestPaginateTypeDef

```python
# DescribeJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeJobsRequestPaginateTypeDef


def get_value() -> DescribeJobsRequestPaginateTypeDef:
    return {
        "accountID": ...,
    }


# DescribeJobsRequestPaginateTypeDef definition

class DescribeJobsRequestPaginateTypeDef(TypedDict):
    accountID: NotRequired[str],
    filters: NotRequired[DescribeJobsRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DescribeJobsRequestFiltersTypeDef](./type_defs.md#describejobsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeJobsRequestTypeDef

```python
# DescribeJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeJobsRequestTypeDef


def get_value() -> DescribeJobsRequestTypeDef:
    return {
        "accountID": ...,
    }


# DescribeJobsRequestTypeDef definition

class DescribeJobsRequestTypeDef(TypedDict):
    accountID: NotRequired[str],
    filters: NotRequired[DescribeJobsRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DescribeJobsRequestFiltersTypeDef](./type_defs.md#describejobsrequestfilterstypedef) 
## DescribeReplicationConfigurationTemplatesResponseTypeDef

```python
# DescribeReplicationConfigurationTemplatesResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeReplicationConfigurationTemplatesResponseTypeDef


def get_value() -> DescribeReplicationConfigurationTemplatesResponseTypeDef:
    return {
        "items": ...,
    }


# DescribeReplicationConfigurationTemplatesResponseTypeDef definition

class DescribeReplicationConfigurationTemplatesResponseTypeDef(TypedDict):
    items: List[ReplicationConfigurationTemplateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ReplicationConfigurationTemplateTypeDef](./type_defs.md#replicationconfigurationtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSourceServersRequestPaginateTypeDef

```python
# DescribeSourceServersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeSourceServersRequestPaginateTypeDef


def get_value() -> DescribeSourceServersRequestPaginateTypeDef:
    return {
        "accountID": ...,
    }


# DescribeSourceServersRequestPaginateTypeDef definition

class DescribeSourceServersRequestPaginateTypeDef(TypedDict):
    accountID: NotRequired[str],
    filters: NotRequired[DescribeSourceServersRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DescribeSourceServersRequestFiltersTypeDef](./type_defs.md#describesourceserversrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSourceServersRequestTypeDef

```python
# DescribeSourceServersRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeSourceServersRequestTypeDef


def get_value() -> DescribeSourceServersRequestTypeDef:
    return {
        "accountID": ...,
    }


# DescribeSourceServersRequestTypeDef definition

class DescribeSourceServersRequestTypeDef(TypedDict):
    accountID: NotRequired[str],
    filters: NotRequired[DescribeSourceServersRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DescribeSourceServersRequestFiltersTypeDef](./type_defs.md#describesourceserversrequestfilterstypedef) 
## DescribeVcenterClientsResponseTypeDef

```python
# DescribeVcenterClientsResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeVcenterClientsResponseTypeDef


def get_value() -> DescribeVcenterClientsResponseTypeDef:
    return {
        "items": ...,
    }


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
# ExportTaskErrorTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ExportTaskErrorTypeDef


def get_value() -> ExportTaskErrorTypeDef:
    return {
        "errorData": ...,
    }


# ExportTaskErrorTypeDef definition

class ExportTaskErrorTypeDef(TypedDict):
    errorData: NotRequired[ExportErrorDataTypeDef],  # (1)
    errorDateTime: NotRequired[str],
```

1. See [:material-code-braces: ExportErrorDataTypeDef](./type_defs.md#exporterrordatatypedef) 
## ExportTaskTypeDef

```python
# ExportTaskTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ExportTaskTypeDef


def get_value() -> ExportTaskTypeDef:
    return {
        "creationDateTime": ...,
    }


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
# ImportTaskErrorTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ImportTaskErrorTypeDef


def get_value() -> ImportTaskErrorTypeDef:
    return {
        "errorData": ...,
    }


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
# ImportTaskSummaryTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ImportTaskSummaryTypeDef


def get_value() -> ImportTaskSummaryTypeDef:
    return {
        "applications": ...,
    }


# ImportTaskSummaryTypeDef definition

class ImportTaskSummaryTypeDef(TypedDict):
    applications: NotRequired[ImportTaskSummaryApplicationsTypeDef],  # (1)
    servers: NotRequired[ImportTaskSummaryServersTypeDef],  # (2)
    waves: NotRequired[ImportTaskSummaryWavesTypeDef],  # (3)
```

1. See [:material-code-braces: ImportTaskSummaryApplicationsTypeDef](./type_defs.md#importtasksummaryapplicationstypedef) 
2. See [:material-code-braces: ImportTaskSummaryServersTypeDef](./type_defs.md#importtasksummaryserverstypedef) 
3. See [:material-code-braces: ImportTaskSummaryWavesTypeDef](./type_defs.md#importtasksummarywavestypedef) 
## StartImportRequestTypeDef

```python
# StartImportRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import StartImportRequestTypeDef


def get_value() -> StartImportRequestTypeDef:
    return {
        "s3BucketSource": ...,
    }


# StartImportRequestTypeDef definition

class StartImportRequestTypeDef(TypedDict):
    s3BucketSource: S3BucketSourceTypeDef,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: S3BucketSourceTypeDef](./type_defs.md#s3bucketsourcetypedef) 
## JobLogTypeDef

```python
# JobLogTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import JobLogTypeDef


def get_value() -> JobLogTypeDef:
    return {
        "event": ...,
    }


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
# LifeCycleLastCutoverTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import LifeCycleLastCutoverTypeDef


def get_value() -> LifeCycleLastCutoverTypeDef:
    return {
        "finalized": ...,
    }


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
# LifeCycleLastTestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import LifeCycleLastTestTypeDef


def get_value() -> LifeCycleLastTestTypeDef:
    return {
        "finalized": ...,
    }


# LifeCycleLastTestTypeDef definition

class LifeCycleLastTestTypeDef(TypedDict):
    finalized: NotRequired[LifeCycleLastTestFinalizedTypeDef],  # (1)
    initiated: NotRequired[LifeCycleLastTestInitiatedTypeDef],  # (2)
    reverted: NotRequired[LifeCycleLastTestRevertedTypeDef],  # (3)
```

1. See [:material-code-braces: LifeCycleLastTestFinalizedTypeDef](./type_defs.md#lifecyclelasttestfinalizedtypedef) 
2. See [:material-code-braces: LifeCycleLastTestInitiatedTypeDef](./type_defs.md#lifecyclelasttestinitiatedtypedef) 
3. See [:material-code-braces: LifeCycleLastTestRevertedTypeDef](./type_defs.md#lifecyclelasttestrevertedtypedef) 
## ListApplicationsRequestPaginateTypeDef

```python
# ListApplicationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListApplicationsRequestPaginateTypeDef


def get_value() -> ListApplicationsRequestPaginateTypeDef:
    return {
        "accountID": ...,
    }


# ListApplicationsRequestPaginateTypeDef definition

class ListApplicationsRequestPaginateTypeDef(TypedDict):
    accountID: NotRequired[str],
    filters: NotRequired[ListApplicationsRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListApplicationsRequestFiltersTypeDef](./type_defs.md#listapplicationsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListApplicationsRequestTypeDef

```python
# ListApplicationsRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListApplicationsRequestTypeDef


def get_value() -> ListApplicationsRequestTypeDef:
    return {
        "accountID": ...,
    }


# ListApplicationsRequestTypeDef definition

class ListApplicationsRequestTypeDef(TypedDict):
    accountID: NotRequired[str],
    filters: NotRequired[ListApplicationsRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ListApplicationsRequestFiltersTypeDef](./type_defs.md#listapplicationsrequestfilterstypedef) 
## ListConnectorsRequestPaginateTypeDef

```python
# ListConnectorsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListConnectorsRequestPaginateTypeDef


def get_value() -> ListConnectorsRequestPaginateTypeDef:
    return {
        "filters": ...,
    }


# ListConnectorsRequestPaginateTypeDef definition

class ListConnectorsRequestPaginateTypeDef(TypedDict):
    filters: NotRequired[ListConnectorsRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListConnectorsRequestFiltersTypeDef](./type_defs.md#listconnectorsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConnectorsRequestTypeDef

```python
# ListConnectorsRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListConnectorsRequestTypeDef


def get_value() -> ListConnectorsRequestTypeDef:
    return {
        "filters": ...,
    }


# ListConnectorsRequestTypeDef definition

class ListConnectorsRequestTypeDef(TypedDict):
    filters: NotRequired[ListConnectorsRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ListConnectorsRequestFiltersTypeDef](./type_defs.md#listconnectorsrequestfilterstypedef) 
## ListExportsRequestPaginateTypeDef

```python
# ListExportsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListExportsRequestPaginateTypeDef


def get_value() -> ListExportsRequestPaginateTypeDef:
    return {
        "filters": ...,
    }


# ListExportsRequestPaginateTypeDef definition

class ListExportsRequestPaginateTypeDef(TypedDict):
    filters: NotRequired[ListExportsRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListExportsRequestFiltersTypeDef](./type_defs.md#listexportsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListExportsRequestTypeDef

```python
# ListExportsRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListExportsRequestTypeDef


def get_value() -> ListExportsRequestTypeDef:
    return {
        "filters": ...,
    }


# ListExportsRequestTypeDef definition

class ListExportsRequestTypeDef(TypedDict):
    filters: NotRequired[ListExportsRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ListExportsRequestFiltersTypeDef](./type_defs.md#listexportsrequestfilterstypedef) 
## ListImportsRequestPaginateTypeDef

```python
# ListImportsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListImportsRequestPaginateTypeDef


def get_value() -> ListImportsRequestPaginateTypeDef:
    return {
        "filters": ...,
    }


# ListImportsRequestPaginateTypeDef definition

class ListImportsRequestPaginateTypeDef(TypedDict):
    filters: NotRequired[ListImportsRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListImportsRequestFiltersTypeDef](./type_defs.md#listimportsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListImportsRequestTypeDef

```python
# ListImportsRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListImportsRequestTypeDef


def get_value() -> ListImportsRequestTypeDef:
    return {
        "filters": ...,
    }


# ListImportsRequestTypeDef definition

class ListImportsRequestTypeDef(TypedDict):
    filters: NotRequired[ListImportsRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ListImportsRequestFiltersTypeDef](./type_defs.md#listimportsrequestfilterstypedef) 
## ListManagedAccountsResponseTypeDef

```python
# ListManagedAccountsResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListManagedAccountsResponseTypeDef


def get_value() -> ListManagedAccountsResponseTypeDef:
    return {
        "items": ...,
    }


# ListManagedAccountsResponseTypeDef definition

class ListManagedAccountsResponseTypeDef(TypedDict):
    items: List[ManagedAccountTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ManagedAccountTypeDef](./type_defs.md#managedaccounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSourceServerActionsRequestPaginateTypeDef

```python
# ListSourceServerActionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListSourceServerActionsRequestPaginateTypeDef


def get_value() -> ListSourceServerActionsRequestPaginateTypeDef:
    return {
        "sourceServerID": ...,
    }


# ListSourceServerActionsRequestPaginateTypeDef definition

class ListSourceServerActionsRequestPaginateTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
    filters: NotRequired[SourceServerActionsRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SourceServerActionsRequestFiltersTypeDef](./type_defs.md#sourceserveractionsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSourceServerActionsRequestTypeDef

```python
# ListSourceServerActionsRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListSourceServerActionsRequestTypeDef


def get_value() -> ListSourceServerActionsRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# ListSourceServerActionsRequestTypeDef definition

class ListSourceServerActionsRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
    filters: NotRequired[SourceServerActionsRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SourceServerActionsRequestFiltersTypeDef](./type_defs.md#sourceserveractionsrequestfilterstypedef) 
## ListTemplateActionsRequestPaginateTypeDef

```python
# ListTemplateActionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListTemplateActionsRequestPaginateTypeDef


def get_value() -> ListTemplateActionsRequestPaginateTypeDef:
    return {
        "launchConfigurationTemplateID": ...,
    }


# ListTemplateActionsRequestPaginateTypeDef definition

class ListTemplateActionsRequestPaginateTypeDef(TypedDict):
    launchConfigurationTemplateID: str,
    filters: NotRequired[TemplateActionsRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: TemplateActionsRequestFiltersTypeDef](./type_defs.md#templateactionsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTemplateActionsRequestTypeDef

```python
# ListTemplateActionsRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListTemplateActionsRequestTypeDef


def get_value() -> ListTemplateActionsRequestTypeDef:
    return {
        "launchConfigurationTemplateID": ...,
    }


# ListTemplateActionsRequestTypeDef definition

class ListTemplateActionsRequestTypeDef(TypedDict):
    launchConfigurationTemplateID: str,
    filters: NotRequired[TemplateActionsRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TemplateActionsRequestFiltersTypeDef](./type_defs.md#templateactionsrequestfilterstypedef) 
## ListWavesRequestPaginateTypeDef

```python
# ListWavesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListWavesRequestPaginateTypeDef


def get_value() -> ListWavesRequestPaginateTypeDef:
    return {
        "accountID": ...,
    }


# ListWavesRequestPaginateTypeDef definition

class ListWavesRequestPaginateTypeDef(TypedDict):
    accountID: NotRequired[str],
    filters: NotRequired[ListWavesRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListWavesRequestFiltersTypeDef](./type_defs.md#listwavesrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWavesRequestTypeDef

```python
# ListWavesRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListWavesRequestTypeDef


def get_value() -> ListWavesRequestTypeDef:
    return {
        "accountID": ...,
    }


# ListWavesRequestTypeDef definition

class ListWavesRequestTypeDef(TypedDict):
    accountID: NotRequired[str],
    filters: NotRequired[ListWavesRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ListWavesRequestFiltersTypeDef](./type_defs.md#listwavesrequestfilterstypedef) 
## SourcePropertiesTypeDef

```python
# SourcePropertiesTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import SourcePropertiesTypeDef


def get_value() -> SourcePropertiesTypeDef:
    return {
        "cpus": ...,
    }


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
## PutSourceServerActionRequestTypeDef

```python
# PutSourceServerActionRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import PutSourceServerActionRequestTypeDef


def get_value() -> PutSourceServerActionRequestTypeDef:
    return {
        "actionID": ...,
    }


# PutSourceServerActionRequestTypeDef definition

class PutSourceServerActionRequestTypeDef(TypedDict):
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
## PutTemplateActionRequestTypeDef

```python
# PutTemplateActionRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import PutTemplateActionRequestTypeDef


def get_value() -> PutTemplateActionRequestTypeDef:
    return {
        "actionID": ...,
    }


# PutTemplateActionRequestTypeDef definition

class PutTemplateActionRequestTypeDef(TypedDict):
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
# SourceServerActionDocumentResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import SourceServerActionDocumentResponseTypeDef


def get_value() -> SourceServerActionDocumentResponseTypeDef:
    return {
        "actionID": ...,
    }


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
# SourceServerActionDocumentTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import SourceServerActionDocumentTypeDef


def get_value() -> SourceServerActionDocumentTypeDef:
    return {
        "actionID": ...,
    }


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
# SsmDocumentOutputTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import SsmDocumentOutputTypeDef


def get_value() -> SsmDocumentOutputTypeDef:
    return {
        "actionName": ...,
    }


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
# SsmDocumentTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import SsmDocumentTypeDef


def get_value() -> SsmDocumentTypeDef:
    return {
        "actionName": ...,
    }


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
# TemplateActionDocumentResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import TemplateActionDocumentResponseTypeDef


def get_value() -> TemplateActionDocumentResponseTypeDef:
    return {
        "actionID": ...,
    }


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
# TemplateActionDocumentTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import TemplateActionDocumentTypeDef


def get_value() -> TemplateActionDocumentTypeDef:
    return {
        "actionID": ...,
    }


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
# ReplicationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ReplicationConfigurationTypeDef


def get_value() -> ReplicationConfigurationTypeDef:
    return {
        "associateDefaultSecurityGroup": ...,
    }


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
## UpdateReplicationConfigurationRequestTypeDef

```python
# UpdateReplicationConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import UpdateReplicationConfigurationRequestTypeDef


def get_value() -> UpdateReplicationConfigurationRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# UpdateReplicationConfigurationRequestTypeDef definition

class UpdateReplicationConfigurationRequestTypeDef(TypedDict):
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
## UpdateSourceServerRequestTypeDef

```python
# UpdateSourceServerRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import UpdateSourceServerRequestTypeDef


def get_value() -> UpdateSourceServerRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# UpdateSourceServerRequestTypeDef definition

class UpdateSourceServerRequestTypeDef(TypedDict):
    sourceServerID: str,
    accountID: NotRequired[str],
    connectorAction: NotRequired[SourceServerConnectorActionTypeDef],  # (1)
```

1. See [:material-code-braces: SourceServerConnectorActionTypeDef](./type_defs.md#sourceserverconnectoractiontypedef) 
## WaveResponseTypeDef

```python
# WaveResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import WaveResponseTypeDef


def get_value() -> WaveResponseTypeDef:
    return {
        "arn": ...,
    }


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
# WaveTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import WaveTypeDef


def get_value() -> WaveTypeDef:
    return {
        "arn": ...,
    }


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
# ListApplicationsResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListApplicationsResponseTypeDef


def get_value() -> ListApplicationsResponseTypeDef:
    return {
        "items": ...,
    }


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
# ListConnectorsResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListConnectorsResponseTypeDef


def get_value() -> ListConnectorsResponseTypeDef:
    return {
        "items": ...,
    }


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
# DataReplicationInfoTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DataReplicationInfoTypeDef


def get_value() -> DataReplicationInfoTypeDef:
    return {
        "dataReplicationError": ...,
    }


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
# ListExportErrorsResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListExportErrorsResponseTypeDef


def get_value() -> ListExportErrorsResponseTypeDef:
    return {
        "items": ...,
    }


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
# ListExportsResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListExportsResponseTypeDef


def get_value() -> ListExportsResponseTypeDef:
    return {
        "items": ...,
    }


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
# StartExportResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import StartExportResponseTypeDef


def get_value() -> StartExportResponseTypeDef:
    return {
        "exportTask": ...,
    }


# StartExportResponseTypeDef definition

class StartExportResponseTypeDef(TypedDict):
    exportTask: ExportTaskTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExportTaskTypeDef](./type_defs.md#exporttasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListImportErrorsResponseTypeDef

```python
# ListImportErrorsResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListImportErrorsResponseTypeDef


def get_value() -> ListImportErrorsResponseTypeDef:
    return {
        "items": ...,
    }


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
# ImportTaskTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ImportTaskTypeDef


def get_value() -> ImportTaskTypeDef:
    return {
        "creationDateTime": ...,
    }


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
# DescribeJobLogItemsResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeJobLogItemsResponseTypeDef


def get_value() -> DescribeJobLogItemsResponseTypeDef:
    return {
        "items": ...,
    }


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
# LifeCycleTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import LifeCycleTypeDef


def get_value() -> LifeCycleTypeDef:
    return {
        "addedToServiceDateTime": ...,
    }


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
# ListSourceServerActionsResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListSourceServerActionsResponseTypeDef


def get_value() -> ListSourceServerActionsResponseTypeDef:
    return {
        "items": ...,
    }


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
# JobPostLaunchActionsLaunchStatusTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import JobPostLaunchActionsLaunchStatusTypeDef


def get_value() -> JobPostLaunchActionsLaunchStatusTypeDef:
    return {
        "executionID": ...,
    }


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
# PostLaunchActionsOutputTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import PostLaunchActionsOutputTypeDef


def get_value() -> PostLaunchActionsOutputTypeDef:
    return {
        "cloudWatchLogGroupName": ...,
    }


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
## PostLaunchActionsTypeDef

```python
# PostLaunchActionsTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import PostLaunchActionsTypeDef


def get_value() -> PostLaunchActionsTypeDef:
    return {
        "cloudWatchLogGroupName": ...,
    }


# PostLaunchActionsTypeDef definition

class PostLaunchActionsTypeDef(TypedDict):
    cloudWatchLogGroupName: NotRequired[str],
    deployment: NotRequired[PostLaunchActionsDeploymentTypeType],  # (1)
    s3LogBucket: NotRequired[str],
    s3OutputKeyPrefix: NotRequired[str],
    ssmDocuments: NotRequired[Sequence[SsmDocumentTypeDef]],  # (2)
```

1. See [:material-code-brackets: PostLaunchActionsDeploymentTypeType](./literals.md#postlaunchactionsdeploymenttypetype) 
2. See [:material-code-braces: SsmDocumentTypeDef](./type_defs.md#ssmdocumenttypedef) 
## ListTemplateActionsResponseTypeDef

```python
# ListTemplateActionsResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListTemplateActionsResponseTypeDef


def get_value() -> ListTemplateActionsResponseTypeDef:
    return {
        "items": ...,
    }


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
# ListWavesResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListWavesResponseTypeDef


def get_value() -> ListWavesResponseTypeDef:
    return {
        "items": ...,
    }


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
# ListImportsResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListImportsResponseTypeDef


def get_value() -> ListImportsResponseTypeDef:
    return {
        "items": ...,
    }


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
# StartImportResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import StartImportResponseTypeDef


def get_value() -> StartImportResponseTypeDef:
    return {
        "importTask": ...,
    }


# StartImportResponseTypeDef definition

class StartImportResponseTypeDef(TypedDict):
    importTask: ImportTaskTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImportTaskTypeDef](./type_defs.md#importtasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SourceServerResponseTypeDef

```python
# SourceServerResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import SourceServerResponseTypeDef


def get_value() -> SourceServerResponseTypeDef:
    return {
        "applicationID": ...,
    }


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
# SourceServerTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import SourceServerTypeDef


def get_value() -> SourceServerTypeDef:
    return {
        "applicationID": ...,
    }


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
# PostLaunchActionsStatusTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import PostLaunchActionsStatusTypeDef


def get_value() -> PostLaunchActionsStatusTypeDef:
    return {
        "postLaunchActionsLaunchStatusList": ...,
    }


# PostLaunchActionsStatusTypeDef definition

class PostLaunchActionsStatusTypeDef(TypedDict):
    postLaunchActionsLaunchStatusList: NotRequired[List[JobPostLaunchActionsLaunchStatusTypeDef]],  # (1)
    ssmAgentDiscoveryDatetime: NotRequired[str],
```

1. See [:material-code-braces: JobPostLaunchActionsLaunchStatusTypeDef](./type_defs.md#jobpostlaunchactionslaunchstatustypedef) 
## LaunchConfigurationTemplateResponseTypeDef

```python
# LaunchConfigurationTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import LaunchConfigurationTemplateResponseTypeDef


def get_value() -> LaunchConfigurationTemplateResponseTypeDef:
    return {
        "arn": ...,
    }


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
# LaunchConfigurationTemplateTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import LaunchConfigurationTemplateTypeDef


def get_value() -> LaunchConfigurationTemplateTypeDef:
    return {
        "arn": ...,
    }


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
# LaunchConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import LaunchConfigurationTypeDef


def get_value() -> LaunchConfigurationTypeDef:
    return {
        "bootMode": ...,
    }


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
## DescribeSourceServersResponseTypeDef

```python
# DescribeSourceServersResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeSourceServersResponseTypeDef


def get_value() -> DescribeSourceServersResponseTypeDef:
    return {
        "items": ...,
    }


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
# ParticipatingServerTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ParticipatingServerTypeDef


def get_value() -> ParticipatingServerTypeDef:
    return {
        "launchStatus": ...,
    }


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
# DescribeLaunchConfigurationTemplatesResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeLaunchConfigurationTemplatesResponseTypeDef


def get_value() -> DescribeLaunchConfigurationTemplatesResponseTypeDef:
    return {
        "items": ...,
    }


# DescribeLaunchConfigurationTemplatesResponseTypeDef definition

class DescribeLaunchConfigurationTemplatesResponseTypeDef(TypedDict):
    items: List[LaunchConfigurationTemplateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LaunchConfigurationTemplateTypeDef](./type_defs.md#launchconfigurationtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLaunchConfigurationTemplateRequestTypeDef

```python
# CreateLaunchConfigurationTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import CreateLaunchConfigurationTemplateRequestTypeDef


def get_value() -> CreateLaunchConfigurationTemplateRequestTypeDef:
    return {
        "associatePublicIpAddress": ...,
    }


# CreateLaunchConfigurationTemplateRequestTypeDef definition

class CreateLaunchConfigurationTemplateRequestTypeDef(TypedDict):
    associatePublicIpAddress: NotRequired[bool],
    bootMode: NotRequired[BootModeType],  # (1)
    copyPrivateIp: NotRequired[bool],
    copyTags: NotRequired[bool],
    enableMapAutoTagging: NotRequired[bool],
    largeVolumeConf: NotRequired[LaunchTemplateDiskConfTypeDef],  # (2)
    launchDisposition: NotRequired[LaunchDispositionType],  # (3)
    licensing: NotRequired[LicensingTypeDef],  # (4)
    mapAutoTaggingMpeID: NotRequired[str],
    postLaunchActions: NotRequired[PostLaunchActionsUnionTypeDef],  # (5)
    smallVolumeConf: NotRequired[LaunchTemplateDiskConfTypeDef],  # (2)
    smallVolumeMaxSize: NotRequired[int],
    tags: NotRequired[Mapping[str, str]],
    targetInstanceTypeRightSizingMethod: NotRequired[TargetInstanceTypeRightSizingMethodType],  # (7)
```

1. See [:material-code-brackets: BootModeType](./literals.md#bootmodetype) 
2. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef) 
3. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype) 
4. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef) 
5. See [:material-code-braces: PostLaunchActionsTypeDef](./type_defs.md#postlaunchactionstypedef) [:material-code-braces: PostLaunchActionsOutputTypeDef](./type_defs.md#postlaunchactionsoutputtypedef) 
6. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef) 
7. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype) 
## UpdateLaunchConfigurationRequestTypeDef

```python
# UpdateLaunchConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import UpdateLaunchConfigurationRequestTypeDef


def get_value() -> UpdateLaunchConfigurationRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# UpdateLaunchConfigurationRequestTypeDef definition

class UpdateLaunchConfigurationRequestTypeDef(TypedDict):
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
    postLaunchActions: NotRequired[PostLaunchActionsUnionTypeDef],  # (4)
    targetInstanceTypeRightSizingMethod: NotRequired[TargetInstanceTypeRightSizingMethodType],  # (5)
```

1. See [:material-code-brackets: BootModeType](./literals.md#bootmodetype) 
2. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype) 
3. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef) 
4. See [:material-code-braces: PostLaunchActionsTypeDef](./type_defs.md#postlaunchactionstypedef) [:material-code-braces: PostLaunchActionsOutputTypeDef](./type_defs.md#postlaunchactionsoutputtypedef) 
5. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype) 
## UpdateLaunchConfigurationTemplateRequestTypeDef

```python
# UpdateLaunchConfigurationTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import UpdateLaunchConfigurationTemplateRequestTypeDef


def get_value() -> UpdateLaunchConfigurationTemplateRequestTypeDef:
    return {
        "launchConfigurationTemplateID": ...,
    }


# UpdateLaunchConfigurationTemplateRequestTypeDef definition

class UpdateLaunchConfigurationTemplateRequestTypeDef(TypedDict):
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
    postLaunchActions: NotRequired[PostLaunchActionsUnionTypeDef],  # (5)
    smallVolumeConf: NotRequired[LaunchTemplateDiskConfTypeDef],  # (2)
    smallVolumeMaxSize: NotRequired[int],
    targetInstanceTypeRightSizingMethod: NotRequired[TargetInstanceTypeRightSizingMethodType],  # (7)
```

1. See [:material-code-brackets: BootModeType](./literals.md#bootmodetype) 
2. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef) 
3. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype) 
4. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef) 
5. See [:material-code-braces: PostLaunchActionsTypeDef](./type_defs.md#postlaunchactionstypedef) [:material-code-braces: PostLaunchActionsOutputTypeDef](./type_defs.md#postlaunchactionsoutputtypedef) 
6. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef) 
7. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype) 
## JobTypeDef

```python
# JobTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import JobTypeDef


def get_value() -> JobTypeDef:
    return {
        "arn": ...,
    }


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
# DescribeJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeJobsResponseTypeDef


def get_value() -> DescribeJobsResponseTypeDef:
    return {
        "items": ...,
    }


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
# StartCutoverResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import StartCutoverResponseTypeDef


def get_value() -> StartCutoverResponseTypeDef:
    return {
        "job": ...,
    }


# StartCutoverResponseTypeDef definition

class StartCutoverResponseTypeDef(TypedDict):
    job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTestResponseTypeDef

```python
# StartTestResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import StartTestResponseTypeDef


def get_value() -> StartTestResponseTypeDef:
    return {
        "job": ...,
    }


# StartTestResponseTypeDef definition

class StartTestResponseTypeDef(TypedDict):
    job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TerminateTargetInstancesResponseTypeDef

```python
# TerminateTargetInstancesResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import TerminateTargetInstancesResponseTypeDef


def get_value() -> TerminateTargetInstancesResponseTypeDef:
    return {
        "job": ...,
    }


# TerminateTargetInstancesResponseTypeDef definition

class TerminateTargetInstancesResponseTypeDef(TypedDict):
    job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
