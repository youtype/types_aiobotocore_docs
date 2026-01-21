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
        "lastUpdateDateTime": ...,
    }


# ApplicationAggregatedStatusTypeDef definition

class ApplicationAggregatedStatusTypeDef(TypedDict):
    lastUpdateDateTime: NotRequired[str],
    healthStatus: NotRequired[ApplicationHealthStatusType],  # (1)
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
    HTTPHeaders: dict[str, str],
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
        "waveID": ...,
    }


# AssociateApplicationsRequestTypeDef definition

class AssociateApplicationsRequestTypeDef(TypedDict):
    waveID: str,
    applicationIDs: Sequence[str],
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
        "s3OutputEnabled": ...,
    }


# ConnectorSsmCommandConfigTypeDef definition

class ConnectorSsmCommandConfigTypeDef(TypedDict):
    s3OutputEnabled: bool,
    cloudWatchOutputEnabled: bool,
    outputS3BucketName: NotRequired[str],
    cloudWatchLogGroupName: NotRequired[str],
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
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    accountID: NotRequired[str],
```


## LaunchTemplateDiskConfTypeDef

```python
# LaunchTemplateDiskConfTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import LaunchTemplateDiskConfTypeDef


def get_value() -> LaunchTemplateDiskConfTypeDef:
    return {
        "volumeType": ...,
    }


# LaunchTemplateDiskConfTypeDef definition

class LaunchTemplateDiskConfTypeDef(TypedDict):
    volumeType: NotRequired[VolumeTypeType],  # (1)
    iops: NotRequired[int],
    throughput: NotRequired[int],
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
        "stagingAreaSubnetId": ...,
    }


# CreateReplicationConfigurationTemplateRequestTypeDef definition

class CreateReplicationConfigurationTemplateRequestTypeDef(TypedDict):
    stagingAreaSubnetId: str,
    associateDefaultSecurityGroup: bool,
    replicationServersSecurityGroupsIDs: Sequence[str],
    replicationServerInstanceType: str,
    useDedicatedReplicationServer: bool,
    defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType,  # (1)
    ebsEncryption: ReplicationConfigurationEbsEncryptionType,  # (2)
    bandwidthThrottling: int,
    dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType,  # (3)
    createPublicIP: bool,
    stagingAreaTags: Mapping[str, str],
    ebsEncryptionKeyArn: NotRequired[str],
    useFipsEndpoint: NotRequired[bool],
    tags: NotRequired[Mapping[str, str]],
    internetProtocol: NotRequired[InternetProtocolType],  # (4)
```

1. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype)
2. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype)
3. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype)
4. See [:material-code-brackets: InternetProtocolType](./literals.md#internetprotocoltype)

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
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    accountID: NotRequired[str],
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
        "deviceName": ...,
    }


# DataReplicationInfoReplicatedDiskTypeDef definition

class DataReplicationInfoReplicatedDiskTypeDef(TypedDict):
    deviceName: NotRequired[str],
    totalStorageBytes: NotRequired[int],
    replicatedStorageBytes: NotRequired[int],
    rescannedStorageBytes: NotRequired[int],
    backloggedStorageBytes: NotRequired[int],
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
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    accountID: NotRequired[str],
```


## DescribeJobsRequestFiltersTypeDef

```python
# DescribeJobsRequestFiltersTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeJobsRequestFiltersTypeDef


def get_value() -> DescribeJobsRequestFiltersTypeDef:
    return {
        "jobIDs": ...,
    }


# DescribeJobsRequestFiltersTypeDef definition

class DescribeJobsRequestFiltersTypeDef(TypedDict):
    jobIDs: NotRequired[Sequence[str]],
    fromDate: NotRequired[str],
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
        "replicationConfigurationTemplateIDs": ...,
    }


# DescribeReplicationConfigurationTemplatesRequestTypeDef definition

class DescribeReplicationConfigurationTemplatesRequestTypeDef(TypedDict):
    replicationConfigurationTemplateIDs: NotRequired[Sequence[str]],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ReplicationConfigurationTemplateTypeDef

```python
# ReplicationConfigurationTemplateTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ReplicationConfigurationTemplateTypeDef


def get_value() -> ReplicationConfigurationTemplateTypeDef:
    return {
        "replicationConfigurationTemplateID": ...,
    }


# ReplicationConfigurationTemplateTypeDef definition

class ReplicationConfigurationTemplateTypeDef(TypedDict):
    replicationConfigurationTemplateID: str,
    arn: NotRequired[str],
    stagingAreaSubnetId: NotRequired[str],
    associateDefaultSecurityGroup: NotRequired[bool],
    replicationServersSecurityGroupsIDs: NotRequired[list[str]],
    replicationServerInstanceType: NotRequired[str],
    useDedicatedReplicationServer: NotRequired[bool],
    defaultLargeStagingDiskType: NotRequired[ReplicationConfigurationDefaultLargeStagingDiskTypeType],  # (1)
    ebsEncryption: NotRequired[ReplicationConfigurationEbsEncryptionType],  # (2)
    ebsEncryptionKeyArn: NotRequired[str],
    bandwidthThrottling: NotRequired[int],
    dataPlaneRouting: NotRequired[ReplicationConfigurationDataPlaneRoutingType],  # (3)
    createPublicIP: NotRequired[bool],
    stagingAreaTags: NotRequired[dict[str, str]],
    useFipsEndpoint: NotRequired[bool],
    tags: NotRequired[dict[str, str]],
    internetProtocol: NotRequired[InternetProtocolType],  # (4)
```

1. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype)
2. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype)
3. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype)
4. See [:material-code-brackets: InternetProtocolType](./literals.md#internetprotocoltype)

## DescribeSourceServersRequestFiltersTypeDef

```python
# DescribeSourceServersRequestFiltersTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeSourceServersRequestFiltersTypeDef


def get_value() -> DescribeSourceServersRequestFiltersTypeDef:
    return {
        "sourceServerIDs": ...,
    }


# DescribeSourceServersRequestFiltersTypeDef definition

class DescribeSourceServersRequestFiltersTypeDef(TypedDict):
    sourceServerIDs: NotRequired[Sequence[str]],
    isArchived: NotRequired[bool],
    replicationTypes: NotRequired[Sequence[ReplicationTypeType]],  # (1)
    lifeCycleStates: NotRequired[Sequence[LifeCycleStateType]],  # (2)
    applicationIDs: NotRequired[Sequence[str]],
```

1. See `Sequence[ReplicationTypeType]`
2. See `Sequence[LifeCycleStateType]`

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
        "vcenterClientID": ...,
    }


# VcenterClientTypeDef definition

class VcenterClientTypeDef(TypedDict):
    vcenterClientID: NotRequired[str],
    arn: NotRequired[str],
    hostname: NotRequired[str],
    vcenterUUID: NotRequired[str],
    datacenterName: NotRequired[str],
    lastSeenDatetime: NotRequired[str],
    sourceServerTags: NotRequired[dict[str, str]],
    tags: NotRequired[dict[str, str]],
```


## DisassociateApplicationsRequestTypeDef

```python
# DisassociateApplicationsRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DisassociateApplicationsRequestTypeDef


def get_value() -> DisassociateApplicationsRequestTypeDef:
    return {
        "waveID": ...,
    }


# DisassociateApplicationsRequestTypeDef definition

class DisassociateApplicationsRequestTypeDef(TypedDict):
    waveID: str,
    applicationIDs: Sequence[str],
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
        "deviceName": ...,
    }


# DiskTypeDef definition

class DiskTypeDef(TypedDict):
    deviceName: NotRequired[str],
    bytes: NotRequired[int],
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
        "serversCount": ...,
    }


# ExportTaskSummaryTypeDef definition

class ExportTaskSummaryTypeDef(TypedDict):
    serversCount: NotRequired[int],
    applicationsCount: NotRequired[int],
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
        "fqdn": ...,
    }


# IdentificationHintsTypeDef definition

class IdentificationHintsTypeDef(TypedDict):
    fqdn: NotRequired[str],
    hostname: NotRequired[str],
    vmWareUuid: NotRequired[str],
    awsInstanceID: NotRequired[str],
    vmPath: NotRequired[str],
```


## ImportErrorDataTypeDef

```python
# ImportErrorDataTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ImportErrorDataTypeDef


def get_value() -> ImportErrorDataTypeDef:
    return {
        "sourceServerID": ...,
    }


# ImportErrorDataTypeDef definition

class ImportErrorDataTypeDef(TypedDict):
    sourceServerID: NotRequired[str],
    applicationID: NotRequired[str],
    waveID: NotRequired[str],
    ec2LaunchTemplateID: NotRequired[str],
    rowNumber: NotRequired[int],
    rawError: NotRequired[str],
    accountID: NotRequired[str],
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
        "sourceServerID": ...,
    }


# JobLogEventDataTypeDef definition

class JobLogEventDataTypeDef(TypedDict):
    sourceServerID: NotRequired[str],
    conversionServerID: NotRequired[str],
    targetInstanceID: NotRequired[str],
    rawError: NotRequired[str],
    attemptCount: NotRequired[int],
    maxAttemptsCount: NotRequired[int],
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
    jobID: NotRequired[str],
    firstBoot: NotRequired[FirstBootType],  # (1)
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
        "waveIDs": ...,
    }


# ListWavesRequestFiltersTypeDef definition

class ListWavesRequestFiltersTypeDef(TypedDict):
    waveIDs: NotRequired[Sequence[str]],
    isArchived: NotRequired[bool],
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
        "macAddress": ...,
    }


# NetworkInterfaceTypeDef definition

class NetworkInterfaceTypeDef(TypedDict):
    macAddress: NotRequired[str],
    ips: NotRequired[list[str]],
    isPrimary: NotRequired[bool],
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
        "parameterType": ...,
    }


# SsmParameterStoreParameterTypeDef definition

class SsmParameterStoreParameterTypeDef(TypedDict):
    parameterType: SsmParameterStoreParameterTypeType,  # (1)
    parameterName: str,
```

1. See [:material-code-brackets: SsmParameterStoreParameterTypeType](./literals.md#ssmparameterstoreparametertypetype)

## RemoveSourceServerActionRequestTypeDef

```python
# RemoveSourceServerActionRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import RemoveSourceServerActionRequestTypeDef


def get_value() -> RemoveSourceServerActionRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# RemoveSourceServerActionRequestTypeDef definition

class RemoveSourceServerActionRequestTypeDef(TypedDict):
    sourceServerID: str,
    actionID: str,
    accountID: NotRequired[str],
```


## RemoveTemplateActionRequestTypeDef

```python
# RemoveTemplateActionRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import RemoveTemplateActionRequestTypeDef


def get_value() -> RemoveTemplateActionRequestTypeDef:
    return {
        "launchConfigurationTemplateID": ...,
    }


# RemoveTemplateActionRequestTypeDef definition

class RemoveTemplateActionRequestTypeDef(TypedDict):
    launchConfigurationTemplateID: str,
    actionID: str,
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
    isBootDisk: NotRequired[bool],
    stagingDiskType: NotRequired[ReplicationConfigurationReplicatedDiskStagingDiskTypeType],  # (1)
    iops: NotRequired[int],
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
        "credentialsSecretArn": ...,
    }


# SourceServerConnectorActionTypeDef definition

class SourceServerConnectorActionTypeDef(TypedDict):
    credentialsSecretArn: NotRequired[str],
    connectorArn: NotRequired[str],
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
    tags: NotRequired[Mapping[str, str]],
    accountID: NotRequired[str],
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
    tags: NotRequired[Mapping[str, str]],
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
    tags: NotRequired[Mapping[str, str]],
    accountID: NotRequired[str],
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
    tags: NotRequired[Mapping[str, str]],
    accountID: NotRequired[str],
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
    name: NotRequired[str],
    description: NotRequired[str],
    accountID: NotRequired[str],
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
    stagingAreaSubnetId: NotRequired[str],
    associateDefaultSecurityGroup: NotRequired[bool],
    replicationServersSecurityGroupsIDs: NotRequired[Sequence[str]],
    replicationServerInstanceType: NotRequired[str],
    useDedicatedReplicationServer: NotRequired[bool],
    defaultLargeStagingDiskType: NotRequired[ReplicationConfigurationDefaultLargeStagingDiskTypeType],  # (1)
    ebsEncryption: NotRequired[ReplicationConfigurationEbsEncryptionType],  # (2)
    ebsEncryptionKeyArn: NotRequired[str],
    bandwidthThrottling: NotRequired[int],
    dataPlaneRouting: NotRequired[ReplicationConfigurationDataPlaneRoutingType],  # (3)
    createPublicIP: NotRequired[bool],
    stagingAreaTags: NotRequired[Mapping[str, str]],
    useFipsEndpoint: NotRequired[bool],
    internetProtocol: NotRequired[InternetProtocolType],  # (4)
```

1. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype)
2. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype)
3. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype)
4. See [:material-code-brackets: InternetProtocolType](./literals.md#internetprotocoltype)

## UpdateSourceServerReplicationTypeRequestTypeDef

```python
# UpdateSourceServerReplicationTypeRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import UpdateSourceServerReplicationTypeRequestTypeDef


def get_value() -> UpdateSourceServerReplicationTypeRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# UpdateSourceServerReplicationTypeRequestTypeDef definition

class UpdateSourceServerReplicationTypeRequestTypeDef(TypedDict):
    sourceServerID: str,
    replicationType: ReplicationTypeType,  # (1)
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
    name: NotRequired[str],
    description: NotRequired[str],
    accountID: NotRequired[str],
```


## WaveAggregatedStatusTypeDef

```python
# WaveAggregatedStatusTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import WaveAggregatedStatusTypeDef


def get_value() -> WaveAggregatedStatusTypeDef:
    return {
        "lastUpdateDateTime": ...,
    }


# WaveAggregatedStatusTypeDef definition

class WaveAggregatedStatusTypeDef(TypedDict):
    lastUpdateDateTime: NotRequired[str],
    replicationStartedDateTime: NotRequired[str],
    healthStatus: NotRequired[WaveHealthStatusType],  # (1)
    progressStatus: NotRequired[WaveProgressStatusType],  # (2)
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
        "applicationID": ...,
    }


# ApplicationTypeDef definition

class ApplicationTypeDef(TypedDict):
    applicationID: NotRequired[str],
    arn: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    isArchived: NotRequired[bool],
    applicationAggregatedStatus: NotRequired[ApplicationAggregatedStatusTypeDef],  # (1)
    creationDateTime: NotRequired[str],
    lastModifiedDateTime: NotRequired[str],
    tags: NotRequired[dict[str, str]],
    waveID: NotRequired[str],
```

1. See [:material-code-braces: ApplicationAggregatedStatusTypeDef](./type_defs.md#applicationaggregatedstatustypedef)

## ApplicationResponseTypeDef

```python
# ApplicationResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ApplicationResponseTypeDef


def get_value() -> ApplicationResponseTypeDef:
    return {
        "applicationID": ...,
    }


# ApplicationResponseTypeDef definition

class ApplicationResponseTypeDef(TypedDict):
    applicationID: str,
    arn: str,
    name: str,
    description: str,
    isArchived: bool,
    applicationAggregatedStatus: ApplicationAggregatedStatusTypeDef,  # (1)
    creationDateTime: str,
    lastModifiedDateTime: str,
    tags: dict[str, str],
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
    tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ReplicationConfigurationTemplateResponseTypeDef

```python
# ReplicationConfigurationTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ReplicationConfigurationTemplateResponseTypeDef


def get_value() -> ReplicationConfigurationTemplateResponseTypeDef:
    return {
        "replicationConfigurationTemplateID": ...,
    }


# ReplicationConfigurationTemplateResponseTypeDef definition

class ReplicationConfigurationTemplateResponseTypeDef(TypedDict):
    replicationConfigurationTemplateID: str,
    arn: str,
    stagingAreaSubnetId: str,
    associateDefaultSecurityGroup: bool,
    replicationServersSecurityGroupsIDs: list[str],
    replicationServerInstanceType: str,
    useDedicatedReplicationServer: bool,
    defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType,  # (1)
    ebsEncryption: ReplicationConfigurationEbsEncryptionType,  # (2)
    ebsEncryptionKeyArn: str,
    bandwidthThrottling: int,
    dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType,  # (3)
    createPublicIP: bool,
    stagingAreaTags: dict[str, str],
    useFipsEndpoint: bool,
    tags: dict[str, str],
    internetProtocol: InternetProtocolType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype)
2. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype)
3. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype)
4. See [:material-code-brackets: InternetProtocolType](./literals.md#internetprotocoltype)
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ChangeServerLifeCycleStateRequestTypeDef

```python
# ChangeServerLifeCycleStateRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ChangeServerLifeCycleStateRequestTypeDef


def get_value() -> ChangeServerLifeCycleStateRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# ChangeServerLifeCycleStateRequestTypeDef definition

class ChangeServerLifeCycleStateRequestTypeDef(TypedDict):
    sourceServerID: str,
    lifeCycle: ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,  # (1)
    accountID: NotRequired[str],
```

1. See [:material-code-braces: ChangeServerLifeCycleStateSourceServerLifecycleTypeDef](./type_defs.md#changeserverlifecyclestatesourceserverlifecycletypedef)

## ConnectorResponseTypeDef

```python
# ConnectorResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ConnectorResponseTypeDef


def get_value() -> ConnectorResponseTypeDef:
    return {
        "connectorID": ...,
    }


# ConnectorResponseTypeDef definition

class ConnectorResponseTypeDef(TypedDict):
    connectorID: str,
    name: str,
    ssmInstanceID: str,
    arn: str,
    tags: dict[str, str],
    ssmCommandConfig: ConnectorSsmCommandConfigTypeDef,  # (1)
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
        "connectorID": ...,
    }


# ConnectorTypeDef definition

class ConnectorTypeDef(TypedDict):
    connectorID: NotRequired[str],
    name: NotRequired[str],
    ssmInstanceID: NotRequired[str],
    arn: NotRequired[str],
    tags: NotRequired[dict[str, str]],
    ssmCommandConfig: NotRequired[ConnectorSsmCommandConfigTypeDef],  # (1)
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
    tags: NotRequired[Mapping[str, str]],
    ssmCommandConfig: NotRequired[ConnectorSsmCommandConfigTypeDef],  # (1)
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
        "startDateTime": ...,
    }


# DataReplicationInitiationTypeDef definition

class DataReplicationInitiationTypeDef(TypedDict):
    startDateTime: NotRequired[str],
    nextAttemptDateTime: NotRequired[str],
    steps: NotRequired[list[DataReplicationInitiationStepTypeDef]],  # (1)
```

1. See `list[DataReplicationInitiationStepTypeDef]`

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
        "filters": ...,
    }


# DescribeJobsRequestPaginateTypeDef definition

class DescribeJobsRequestPaginateTypeDef(TypedDict):
    filters: NotRequired[DescribeJobsRequestFiltersTypeDef],  # (1)
    accountID: NotRequired[str],
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
        "filters": ...,
    }


# DescribeJobsRequestTypeDef definition

class DescribeJobsRequestTypeDef(TypedDict):
    filters: NotRequired[DescribeJobsRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    accountID: NotRequired[str],
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
    items: list[ReplicationConfigurationTemplateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[ReplicationConfigurationTemplateTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DescribeSourceServersRequestPaginateTypeDef

```python
# DescribeSourceServersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DescribeSourceServersRequestPaginateTypeDef


def get_value() -> DescribeSourceServersRequestPaginateTypeDef:
    return {
        "filters": ...,
    }


# DescribeSourceServersRequestPaginateTypeDef definition

class DescribeSourceServersRequestPaginateTypeDef(TypedDict):
    filters: NotRequired[DescribeSourceServersRequestFiltersTypeDef],  # (1)
    accountID: NotRequired[str],
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
        "filters": ...,
    }


# DescribeSourceServersRequestTypeDef definition

class DescribeSourceServersRequestTypeDef(TypedDict):
    filters: NotRequired[DescribeSourceServersRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    accountID: NotRequired[str],
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
    items: list[VcenterClientTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[VcenterClientTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ExportTaskErrorTypeDef

```python
# ExportTaskErrorTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ExportTaskErrorTypeDef


def get_value() -> ExportTaskErrorTypeDef:
    return {
        "errorDateTime": ...,
    }


# ExportTaskErrorTypeDef definition

class ExportTaskErrorTypeDef(TypedDict):
    errorDateTime: NotRequired[str],
    errorData: NotRequired[ExportErrorDataTypeDef],  # (1)
```

1. See [:material-code-braces: ExportErrorDataTypeDef](./type_defs.md#exporterrordatatypedef)

## ExportTaskTypeDef

```python
# ExportTaskTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ExportTaskTypeDef


def get_value() -> ExportTaskTypeDef:
    return {
        "exportID": ...,
    }


# ExportTaskTypeDef definition

class ExportTaskTypeDef(TypedDict):
    exportID: NotRequired[str],
    arn: NotRequired[str],
    s3Bucket: NotRequired[str],
    s3Key: NotRequired[str],
    s3BucketOwner: NotRequired[str],
    creationDateTime: NotRequired[str],
    endDateTime: NotRequired[str],
    status: NotRequired[ExportStatusType],  # (1)
    progressPercentage: NotRequired[float],
    summary: NotRequired[ExportTaskSummaryTypeDef],  # (2)
    tags: NotRequired[dict[str, str]],
```

1. See [:material-code-brackets: ExportStatusType](./literals.md#exportstatustype)
2. See [:material-code-braces: ExportTaskSummaryTypeDef](./type_defs.md#exporttasksummarytypedef)

## ImportTaskErrorTypeDef

```python
# ImportTaskErrorTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ImportTaskErrorTypeDef


def get_value() -> ImportTaskErrorTypeDef:
    return {
        "errorDateTime": ...,
    }


# ImportTaskErrorTypeDef definition

class ImportTaskErrorTypeDef(TypedDict):
    errorDateTime: NotRequired[str],
    errorType: NotRequired[ImportErrorTypeType],  # (1)
    errorData: NotRequired[ImportErrorDataTypeDef],  # (2)
```

1. See [:material-code-brackets: ImportErrorTypeType](./literals.md#importerrortypetype)
2. See [:material-code-braces: ImportErrorDataTypeDef](./type_defs.md#importerrordatatypedef)

## ImportTaskSummaryTypeDef

```python
# ImportTaskSummaryTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ImportTaskSummaryTypeDef


def get_value() -> ImportTaskSummaryTypeDef:
    return {
        "waves": ...,
    }


# ImportTaskSummaryTypeDef definition

class ImportTaskSummaryTypeDef(TypedDict):
    waves: NotRequired[ImportTaskSummaryWavesTypeDef],  # (1)
    applications: NotRequired[ImportTaskSummaryApplicationsTypeDef],  # (2)
    servers: NotRequired[ImportTaskSummaryServersTypeDef],  # (3)
```

1. See [:material-code-braces: ImportTaskSummaryWavesTypeDef](./type_defs.md#importtasksummarywavestypedef)
2. See [:material-code-braces: ImportTaskSummaryApplicationsTypeDef](./type_defs.md#importtasksummaryapplicationstypedef)
3. See [:material-code-braces: ImportTaskSummaryServersTypeDef](./type_defs.md#importtasksummaryserverstypedef)

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
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: S3BucketSourceTypeDef](./type_defs.md#s3bucketsourcetypedef)

## JobLogTypeDef

```python
# JobLogTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import JobLogTypeDef


def get_value() -> JobLogTypeDef:
    return {
        "logDateTime": ...,
    }


# JobLogTypeDef definition

class JobLogTypeDef(TypedDict):
    logDateTime: NotRequired[str],
    event: NotRequired[JobLogEventType],  # (1)
    eventData: NotRequired[JobLogEventDataTypeDef],  # (2)
```

1. See [:material-code-brackets: JobLogEventType](./literals.md#joblogeventtype)
2. See [:material-code-braces: JobLogEventDataTypeDef](./type_defs.md#joblogeventdatatypedef)

## LifeCycleLastCutoverTypeDef

```python
# LifeCycleLastCutoverTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import LifeCycleLastCutoverTypeDef


def get_value() -> LifeCycleLastCutoverTypeDef:
    return {
        "initiated": ...,
    }


# LifeCycleLastCutoverTypeDef definition

class LifeCycleLastCutoverTypeDef(TypedDict):
    initiated: NotRequired[LifeCycleLastCutoverInitiatedTypeDef],  # (1)
    reverted: NotRequired[LifeCycleLastCutoverRevertedTypeDef],  # (2)
    finalized: NotRequired[LifeCycleLastCutoverFinalizedTypeDef],  # (3)
```

1. See [:material-code-braces: LifeCycleLastCutoverInitiatedTypeDef](./type_defs.md#lifecyclelastcutoverinitiatedtypedef)
2. See [:material-code-braces: LifeCycleLastCutoverRevertedTypeDef](./type_defs.md#lifecyclelastcutoverrevertedtypedef)
3. See [:material-code-braces: LifeCycleLastCutoverFinalizedTypeDef](./type_defs.md#lifecyclelastcutoverfinalizedtypedef)

## LifeCycleLastTestTypeDef

```python
# LifeCycleLastTestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import LifeCycleLastTestTypeDef


def get_value() -> LifeCycleLastTestTypeDef:
    return {
        "initiated": ...,
    }


# LifeCycleLastTestTypeDef definition

class LifeCycleLastTestTypeDef(TypedDict):
    initiated: NotRequired[LifeCycleLastTestInitiatedTypeDef],  # (1)
    reverted: NotRequired[LifeCycleLastTestRevertedTypeDef],  # (2)
    finalized: NotRequired[LifeCycleLastTestFinalizedTypeDef],  # (3)
```

1. See [:material-code-braces: LifeCycleLastTestInitiatedTypeDef](./type_defs.md#lifecyclelasttestinitiatedtypedef)
2. See [:material-code-braces: LifeCycleLastTestRevertedTypeDef](./type_defs.md#lifecyclelasttestrevertedtypedef)
3. See [:material-code-braces: LifeCycleLastTestFinalizedTypeDef](./type_defs.md#lifecyclelasttestfinalizedtypedef)

## ListApplicationsRequestPaginateTypeDef

```python
# ListApplicationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ListApplicationsRequestPaginateTypeDef


def get_value() -> ListApplicationsRequestPaginateTypeDef:
    return {
        "filters": ...,
    }


# ListApplicationsRequestPaginateTypeDef definition

class ListApplicationsRequestPaginateTypeDef(TypedDict):
    filters: NotRequired[ListApplicationsRequestFiltersTypeDef],  # (1)
    accountID: NotRequired[str],
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
        "filters": ...,
    }


# ListApplicationsRequestTypeDef definition

class ListApplicationsRequestTypeDef(TypedDict):
    filters: NotRequired[ListApplicationsRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    accountID: NotRequired[str],
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
    items: list[ManagedAccountTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[ManagedAccountTypeDef]`
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
    filters: NotRequired[SourceServerActionsRequestFiltersTypeDef],  # (1)
    accountID: NotRequired[str],
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
    filters: NotRequired[SourceServerActionsRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    accountID: NotRequired[str],
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
        "filters": ...,
    }


# ListWavesRequestPaginateTypeDef definition

class ListWavesRequestPaginateTypeDef(TypedDict):
    filters: NotRequired[ListWavesRequestFiltersTypeDef],  # (1)
    accountID: NotRequired[str],
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
        "filters": ...,
    }


# ListWavesRequestTypeDef definition

class ListWavesRequestTypeDef(TypedDict):
    filters: NotRequired[ListWavesRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    accountID: NotRequired[str],
```

1. See [:material-code-braces: ListWavesRequestFiltersTypeDef](./type_defs.md#listwavesrequestfilterstypedef)

## SourcePropertiesTypeDef

```python
# SourcePropertiesTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import SourcePropertiesTypeDef


def get_value() -> SourcePropertiesTypeDef:
    return {
        "lastUpdatedDateTime": ...,
    }


# SourcePropertiesTypeDef definition

class SourcePropertiesTypeDef(TypedDict):
    lastUpdatedDateTime: NotRequired[str],
    recommendedInstanceType: NotRequired[str],
    identificationHints: NotRequired[IdentificationHintsTypeDef],  # (1)
    networkInterfaces: NotRequired[list[NetworkInterfaceTypeDef]],  # (2)
    disks: NotRequired[list[DiskTypeDef]],  # (3)
    cpus: NotRequired[list[CPUTypeDef]],  # (4)
    ramBytes: NotRequired[int],
    os: NotRequired[OSTypeDef],  # (5)
```

1. See [:material-code-braces: IdentificationHintsTypeDef](./type_defs.md#identificationhintstypedef)
2. See `list[NetworkInterfaceTypeDef]`
3. See `list[DiskTypeDef]`
4. See `list[CPUTypeDef]`
5. See [:material-code-braces: OSTypeDef](./type_defs.md#ostypedef)

## PutSourceServerActionRequestTypeDef

```python
# PutSourceServerActionRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import PutSourceServerActionRequestTypeDef


def get_value() -> PutSourceServerActionRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# PutSourceServerActionRequestTypeDef definition

class PutSourceServerActionRequestTypeDef(TypedDict):
    sourceServerID: str,
    actionName: str,
    documentIdentifier: str,
    order: int,
    actionID: str,
    documentVersion: NotRequired[str],
    active: NotRequired[bool],
    timeoutSeconds: NotRequired[int],
    mustSucceedForCutover: NotRequired[bool],
    parameters: NotRequired[Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]]],  # (1)
    externalParameters: NotRequired[Mapping[str, SsmExternalParameterTypeDef]],  # (2)
    description: NotRequired[str],
    category: NotRequired[ActionCategoryType],  # (3)
    accountID: NotRequired[str],
```

1. See `Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]]`
2. See `Mapping[str, SsmExternalParameterTypeDef]`
3. See [:material-code-brackets: ActionCategoryType](./literals.md#actioncategorytype)

## PutTemplateActionRequestTypeDef

```python
# PutTemplateActionRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import PutTemplateActionRequestTypeDef


def get_value() -> PutTemplateActionRequestTypeDef:
    return {
        "launchConfigurationTemplateID": ...,
    }


# PutTemplateActionRequestTypeDef definition

class PutTemplateActionRequestTypeDef(TypedDict):
    launchConfigurationTemplateID: str,
    actionName: str,
    documentIdentifier: str,
    order: int,
    actionID: str,
    documentVersion: NotRequired[str],
    active: NotRequired[bool],
    timeoutSeconds: NotRequired[int],
    mustSucceedForCutover: NotRequired[bool],
    parameters: NotRequired[Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]]],  # (1)
    operatingSystem: NotRequired[str],
    externalParameters: NotRequired[Mapping[str, SsmExternalParameterTypeDef]],  # (2)
    description: NotRequired[str],
    category: NotRequired[ActionCategoryType],  # (3)
```

1. See `Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]]`
2. See `Mapping[str, SsmExternalParameterTypeDef]`
3. See [:material-code-brackets: ActionCategoryType](./literals.md#actioncategorytype)

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
    documentIdentifier: str,
    order: int,
    documentVersion: str,
    active: bool,
    timeoutSeconds: int,
    mustSucceedForCutover: bool,
    parameters: dict[str, list[SsmParameterStoreParameterTypeDef]],  # (1)
    externalParameters: dict[str, SsmExternalParameterTypeDef],  # (2)
    description: str,
    category: ActionCategoryType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See `dict[str, list[SsmParameterStoreParameterTypeDef]]`
2. See `dict[str, SsmExternalParameterTypeDef]`
3. See [:material-code-brackets: ActionCategoryType](./literals.md#actioncategorytype)
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
    documentIdentifier: NotRequired[str],
    order: NotRequired[int],
    documentVersion: NotRequired[str],
    active: NotRequired[bool],
    timeoutSeconds: NotRequired[int],
    mustSucceedForCutover: NotRequired[bool],
    parameters: NotRequired[dict[str, list[SsmParameterStoreParameterTypeDef]]],  # (1)
    externalParameters: NotRequired[dict[str, SsmExternalParameterTypeDef]],  # (2)
    description: NotRequired[str],
    category: NotRequired[ActionCategoryType],  # (3)
```

1. See `dict[str, list[SsmParameterStoreParameterTypeDef]]`
2. See `dict[str, SsmExternalParameterTypeDef]`
3. See [:material-code-brackets: ActionCategoryType](./literals.md#actioncategorytype)

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
    timeoutSeconds: NotRequired[int],
    mustSucceedForCutover: NotRequired[bool],
    parameters: NotRequired[dict[str, list[SsmParameterStoreParameterTypeDef]]],  # (1)
    externalParameters: NotRequired[dict[str, SsmExternalParameterTypeDef]],  # (2)
```

1. See `dict[str, list[SsmParameterStoreParameterTypeDef]]`
2. See `dict[str, SsmExternalParameterTypeDef]`

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
    timeoutSeconds: NotRequired[int],
    mustSucceedForCutover: NotRequired[bool],
    parameters: NotRequired[Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]]],  # (1)
    externalParameters: NotRequired[Mapping[str, SsmExternalParameterTypeDef]],  # (2)
```

1. See `Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]]`
2. See `Mapping[str, SsmExternalParameterTypeDef]`

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
    documentIdentifier: str,
    order: int,
    documentVersion: str,
    active: bool,
    timeoutSeconds: int,
    mustSucceedForCutover: bool,
    parameters: dict[str, list[SsmParameterStoreParameterTypeDef]],  # (1)
    operatingSystem: str,
    externalParameters: dict[str, SsmExternalParameterTypeDef],  # (2)
    description: str,
    category: ActionCategoryType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See `dict[str, list[SsmParameterStoreParameterTypeDef]]`
2. See `dict[str, SsmExternalParameterTypeDef]`
3. See [:material-code-brackets: ActionCategoryType](./literals.md#actioncategorytype)
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
    documentIdentifier: NotRequired[str],
    order: NotRequired[int],
    documentVersion: NotRequired[str],
    active: NotRequired[bool],
    timeoutSeconds: NotRequired[int],
    mustSucceedForCutover: NotRequired[bool],
    parameters: NotRequired[dict[str, list[SsmParameterStoreParameterTypeDef]]],  # (1)
    operatingSystem: NotRequired[str],
    externalParameters: NotRequired[dict[str, SsmExternalParameterTypeDef]],  # (2)
    description: NotRequired[str],
    category: NotRequired[ActionCategoryType],  # (3)
```

1. See `dict[str, list[SsmParameterStoreParameterTypeDef]]`
2. See `dict[str, SsmExternalParameterTypeDef]`
3. See [:material-code-brackets: ActionCategoryType](./literals.md#actioncategorytype)

## ReplicationConfigurationTypeDef

```python
# ReplicationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ReplicationConfigurationTypeDef


def get_value() -> ReplicationConfigurationTypeDef:
    return {
        "sourceServerID": ...,
    }


# ReplicationConfigurationTypeDef definition

class ReplicationConfigurationTypeDef(TypedDict):
    sourceServerID: str,
    name: str,
    stagingAreaSubnetId: str,
    associateDefaultSecurityGroup: bool,
    replicationServersSecurityGroupsIDs: list[str],
    replicationServerInstanceType: str,
    useDedicatedReplicationServer: bool,
    defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType,  # (1)
    replicatedDisks: list[ReplicationConfigurationReplicatedDiskTypeDef],  # (2)
    ebsEncryption: ReplicationConfigurationEbsEncryptionType,  # (3)
    ebsEncryptionKeyArn: str,
    bandwidthThrottling: int,
    dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType,  # (4)
    createPublicIP: bool,
    stagingAreaTags: dict[str, str],
    useFipsEndpoint: bool,
    internetProtocol: InternetProtocolType,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype)
2. See `list[ReplicationConfigurationReplicatedDiskTypeDef]`
3. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype)
4. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype)
5. See [:material-code-brackets: InternetProtocolType](./literals.md#internetprotocoltype)
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

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
    name: NotRequired[str],
    stagingAreaSubnetId: NotRequired[str],
    associateDefaultSecurityGroup: NotRequired[bool],
    replicationServersSecurityGroupsIDs: NotRequired[Sequence[str]],
    replicationServerInstanceType: NotRequired[str],
    useDedicatedReplicationServer: NotRequired[bool],
    defaultLargeStagingDiskType: NotRequired[ReplicationConfigurationDefaultLargeStagingDiskTypeType],  # (1)
    replicatedDisks: NotRequired[Sequence[ReplicationConfigurationReplicatedDiskTypeDef]],  # (2)
    ebsEncryption: NotRequired[ReplicationConfigurationEbsEncryptionType],  # (3)
    ebsEncryptionKeyArn: NotRequired[str],
    bandwidthThrottling: NotRequired[int],
    dataPlaneRouting: NotRequired[ReplicationConfigurationDataPlaneRoutingType],  # (4)
    createPublicIP: NotRequired[bool],
    stagingAreaTags: NotRequired[Mapping[str, str]],
    useFipsEndpoint: NotRequired[bool],
    accountID: NotRequired[str],
    internetProtocol: NotRequired[InternetProtocolType],  # (5)
```

1. See [:material-code-brackets: ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype)
2. See `Sequence[ReplicationConfigurationReplicatedDiskTypeDef]`
3. See [:material-code-brackets: ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype)
4. See [:material-code-brackets: ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype)
5. See [:material-code-brackets: InternetProtocolType](./literals.md#internetprotocoltype)

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
        "waveID": ...,
    }


# WaveResponseTypeDef definition

class WaveResponseTypeDef(TypedDict):
    waveID: str,
    arn: str,
    name: str,
    description: str,
    isArchived: bool,
    waveAggregatedStatus: WaveAggregatedStatusTypeDef,  # (1)
    creationDateTime: str,
    lastModifiedDateTime: str,
    tags: dict[str, str],
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
        "waveID": ...,
    }


# WaveTypeDef definition

class WaveTypeDef(TypedDict):
    waveID: NotRequired[str],
    arn: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    isArchived: NotRequired[bool],
    waveAggregatedStatus: NotRequired[WaveAggregatedStatusTypeDef],  # (1)
    creationDateTime: NotRequired[str],
    lastModifiedDateTime: NotRequired[str],
    tags: NotRequired[dict[str, str]],
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
    items: list[ApplicationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[ApplicationTypeDef]`
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
    items: list[ConnectorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[ConnectorTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DataReplicationInfoTypeDef

```python
# DataReplicationInfoTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import DataReplicationInfoTypeDef


def get_value() -> DataReplicationInfoTypeDef:
    return {
        "lagDuration": ...,
    }


# DataReplicationInfoTypeDef definition

class DataReplicationInfoTypeDef(TypedDict):
    lagDuration: NotRequired[str],
    etaDateTime: NotRequired[str],
    replicatedDisks: NotRequired[list[DataReplicationInfoReplicatedDiskTypeDef]],  # (1)
    dataReplicationState: NotRequired[DataReplicationStateType],  # (2)
    dataReplicationInitiation: NotRequired[DataReplicationInitiationTypeDef],  # (3)
    dataReplicationError: NotRequired[DataReplicationErrorTypeDef],  # (4)
    lastSnapshotDateTime: NotRequired[str],
    replicatorId: NotRequired[str],
```

1. See `list[DataReplicationInfoReplicatedDiskTypeDef]`
2. See [:material-code-brackets: DataReplicationStateType](./literals.md#datareplicationstatetype)
3. See [:material-code-braces: DataReplicationInitiationTypeDef](./type_defs.md#datareplicationinitiationtypedef)
4. See [:material-code-braces: DataReplicationErrorTypeDef](./type_defs.md#datareplicationerrortypedef)

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
    items: list[ExportTaskErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[ExportTaskErrorTypeDef]`
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
    items: list[ExportTaskTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[ExportTaskTypeDef]`
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
    items: list[ImportTaskErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[ImportTaskErrorTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ImportTaskTypeDef

```python
# ImportTaskTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ImportTaskTypeDef


def get_value() -> ImportTaskTypeDef:
    return {
        "importID": ...,
    }


# ImportTaskTypeDef definition

class ImportTaskTypeDef(TypedDict):
    importID: NotRequired[str],
    arn: NotRequired[str],
    s3BucketSource: NotRequired[S3BucketSourceTypeDef],  # (1)
    creationDateTime: NotRequired[str],
    endDateTime: NotRequired[str],
    status: NotRequired[ImportStatusType],  # (2)
    progressPercentage: NotRequired[float],
    summary: NotRequired[ImportTaskSummaryTypeDef],  # (3)
    tags: NotRequired[dict[str, str]],
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
    items: list[JobLogTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[JobLogTypeDef]`
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
    firstByteDateTime: NotRequired[str],
    elapsedReplicationDuration: NotRequired[str],
    lastSeenByServiceDateTime: NotRequired[str],
    lastTest: NotRequired[LifeCycleLastTestTypeDef],  # (1)
    lastCutover: NotRequired[LifeCycleLastCutoverTypeDef],  # (2)
    state: NotRequired[LifeCycleStateType],  # (3)
```

1. See [:material-code-braces: LifeCycleLastTestTypeDef](./type_defs.md#lifecyclelasttesttypedef)
2. See [:material-code-braces: LifeCycleLastCutoverTypeDef](./type_defs.md#lifecyclelastcutovertypedef)
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
    items: list[SourceServerActionDocumentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[SourceServerActionDocumentTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## JobPostLaunchActionsLaunchStatusTypeDef

```python
# JobPostLaunchActionsLaunchStatusTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import JobPostLaunchActionsLaunchStatusTypeDef


def get_value() -> JobPostLaunchActionsLaunchStatusTypeDef:
    return {
        "ssmDocument": ...,
    }


# JobPostLaunchActionsLaunchStatusTypeDef definition

class JobPostLaunchActionsLaunchStatusTypeDef(TypedDict):
    ssmDocument: NotRequired[SsmDocumentOutputTypeDef],  # (1)
    ssmDocumentType: NotRequired[SsmDocumentTypeType],  # (2)
    executionID: NotRequired[str],
    executionStatus: NotRequired[PostLaunchActionExecutionStatusType],  # (3)
    failureReason: NotRequired[str],
```

1. See [:material-code-braces: SsmDocumentOutputTypeDef](./type_defs.md#ssmdocumentoutputtypedef)
2. See [:material-code-brackets: SsmDocumentTypeType](./literals.md#ssmdocumenttypetype)
3. See [:material-code-brackets: PostLaunchActionExecutionStatusType](./literals.md#postlaunchactionexecutionstatustype)

## PostLaunchActionsOutputTypeDef

```python
# PostLaunchActionsOutputTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import PostLaunchActionsOutputTypeDef


def get_value() -> PostLaunchActionsOutputTypeDef:
    return {
        "deployment": ...,
    }


# PostLaunchActionsOutputTypeDef definition

class PostLaunchActionsOutputTypeDef(TypedDict):
    deployment: NotRequired[PostLaunchActionsDeploymentTypeType],  # (1)
    s3LogBucket: NotRequired[str],
    s3OutputKeyPrefix: NotRequired[str],
    cloudWatchLogGroupName: NotRequired[str],
    ssmDocuments: NotRequired[list[SsmDocumentOutputTypeDef]],  # (2)
```

1. See [:material-code-brackets: PostLaunchActionsDeploymentTypeType](./literals.md#postlaunchactionsdeploymenttypetype)
2. See `list[SsmDocumentOutputTypeDef]`

## PostLaunchActionsTypeDef

```python
# PostLaunchActionsTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import PostLaunchActionsTypeDef


def get_value() -> PostLaunchActionsTypeDef:
    return {
        "deployment": ...,
    }


# PostLaunchActionsTypeDef definition

class PostLaunchActionsTypeDef(TypedDict):
    deployment: NotRequired[PostLaunchActionsDeploymentTypeType],  # (1)
    s3LogBucket: NotRequired[str],
    s3OutputKeyPrefix: NotRequired[str],
    cloudWatchLogGroupName: NotRequired[str],
    ssmDocuments: NotRequired[Sequence[SsmDocumentTypeDef]],  # (2)
```

1. See [:material-code-brackets: PostLaunchActionsDeploymentTypeType](./literals.md#postlaunchactionsdeploymenttypetype)
2. See `Sequence[SsmDocumentTypeDef]`

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
    items: list[TemplateActionDocumentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[TemplateActionDocumentTypeDef]`
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
    items: list[WaveTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[WaveTypeDef]`
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
    items: list[ImportTaskTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[ImportTaskTypeDef]`
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
        "sourceServerID": ...,
    }


# SourceServerResponseTypeDef definition

class SourceServerResponseTypeDef(TypedDict):
    sourceServerID: str,
    arn: str,
    isArchived: bool,
    tags: dict[str, str],
    launchedInstance: LaunchedInstanceTypeDef,  # (1)
    dataReplicationInfo: DataReplicationInfoTypeDef,  # (2)
    lifeCycle: LifeCycleTypeDef,  # (3)
    sourceProperties: SourcePropertiesTypeDef,  # (4)
    replicationType: ReplicationTypeType,  # (5)
    vcenterClientID: str,
    applicationID: str,
    userProvidedID: str,
    fqdnForActionFramework: str,
    connectorAction: SourceServerConnectorActionTypeDef,  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-braces: LaunchedInstanceTypeDef](./type_defs.md#launchedinstancetypedef)
2. See [:material-code-braces: DataReplicationInfoTypeDef](./type_defs.md#datareplicationinfotypedef)
3. See [:material-code-braces: LifeCycleTypeDef](./type_defs.md#lifecycletypedef)
4. See [:material-code-braces: SourcePropertiesTypeDef](./type_defs.md#sourcepropertiestypedef)
5. See [:material-code-brackets: ReplicationTypeType](./literals.md#replicationtypetype)
6. See [:material-code-braces: SourceServerConnectorActionTypeDef](./type_defs.md#sourceserverconnectoractiontypedef)
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## SourceServerTypeDef

```python
# SourceServerTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import SourceServerTypeDef


def get_value() -> SourceServerTypeDef:
    return {
        "sourceServerID": ...,
    }


# SourceServerTypeDef definition

class SourceServerTypeDef(TypedDict):
    sourceServerID: NotRequired[str],
    arn: NotRequired[str],
    isArchived: NotRequired[bool],
    tags: NotRequired[dict[str, str]],
    launchedInstance: NotRequired[LaunchedInstanceTypeDef],  # (1)
    dataReplicationInfo: NotRequired[DataReplicationInfoTypeDef],  # (2)
    lifeCycle: NotRequired[LifeCycleTypeDef],  # (3)
    sourceProperties: NotRequired[SourcePropertiesTypeDef],  # (4)
    replicationType: NotRequired[ReplicationTypeType],  # (5)
    vcenterClientID: NotRequired[str],
    applicationID: NotRequired[str],
    userProvidedID: NotRequired[str],
    fqdnForActionFramework: NotRequired[str],
    connectorAction: NotRequired[SourceServerConnectorActionTypeDef],  # (6)
```

1. See [:material-code-braces: LaunchedInstanceTypeDef](./type_defs.md#launchedinstancetypedef)
2. See [:material-code-braces: DataReplicationInfoTypeDef](./type_defs.md#datareplicationinfotypedef)
3. See [:material-code-braces: LifeCycleTypeDef](./type_defs.md#lifecycletypedef)
4. See [:material-code-braces: SourcePropertiesTypeDef](./type_defs.md#sourcepropertiestypedef)
5. See [:material-code-brackets: ReplicationTypeType](./literals.md#replicationtypetype)
6. See [:material-code-braces: SourceServerConnectorActionTypeDef](./type_defs.md#sourceserverconnectoractiontypedef)

## PostLaunchActionsStatusTypeDef

```python
# PostLaunchActionsStatusTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import PostLaunchActionsStatusTypeDef


def get_value() -> PostLaunchActionsStatusTypeDef:
    return {
        "ssmAgentDiscoveryDatetime": ...,
    }


# PostLaunchActionsStatusTypeDef definition

class PostLaunchActionsStatusTypeDef(TypedDict):
    ssmAgentDiscoveryDatetime: NotRequired[str],
    postLaunchActionsLaunchStatusList: NotRequired[list[JobPostLaunchActionsLaunchStatusTypeDef]],  # (1)
```

1. See `list[JobPostLaunchActionsLaunchStatusTypeDef]`

## LaunchConfigurationTemplateResponseTypeDef

```python
# LaunchConfigurationTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import LaunchConfigurationTemplateResponseTypeDef


def get_value() -> LaunchConfigurationTemplateResponseTypeDef:
    return {
        "launchConfigurationTemplateID": ...,
    }


# LaunchConfigurationTemplateResponseTypeDef definition

class LaunchConfigurationTemplateResponseTypeDef(TypedDict):
    launchConfigurationTemplateID: str,
    arn: str,
    postLaunchActions: PostLaunchActionsOutputTypeDef,  # (1)
    enableMapAutoTagging: bool,
    mapAutoTaggingMpeID: str,
    tags: dict[str, str],
    ec2LaunchTemplateID: str,
    launchDisposition: LaunchDispositionType,  # (2)
    targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType,  # (3)
    copyPrivateIp: bool,
    associatePublicIpAddress: bool,
    copyTags: bool,
    licensing: LicensingTypeDef,  # (4)
    bootMode: BootModeType,  # (5)
    smallVolumeMaxSize: int,
    smallVolumeConf: LaunchTemplateDiskConfTypeDef,  # (6)
    largeVolumeConf: LaunchTemplateDiskConfTypeDef,  # (6)
    enableParametersEncryption: bool,
    parametersEncryptionKey: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-braces: PostLaunchActionsOutputTypeDef](./type_defs.md#postlaunchactionsoutputtypedef)
2. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype)
3. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype)
4. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef)
5. See [:material-code-brackets: BootModeType](./literals.md#bootmodetype)
6. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef)
7. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef)
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## LaunchConfigurationTemplateTypeDef

```python
# LaunchConfigurationTemplateTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import LaunchConfigurationTemplateTypeDef


def get_value() -> LaunchConfigurationTemplateTypeDef:
    return {
        "launchConfigurationTemplateID": ...,
    }


# LaunchConfigurationTemplateTypeDef definition

class LaunchConfigurationTemplateTypeDef(TypedDict):
    launchConfigurationTemplateID: str,
    arn: NotRequired[str],
    postLaunchActions: NotRequired[PostLaunchActionsOutputTypeDef],  # (1)
    enableMapAutoTagging: NotRequired[bool],
    mapAutoTaggingMpeID: NotRequired[str],
    tags: NotRequired[dict[str, str]],
    ec2LaunchTemplateID: NotRequired[str],
    launchDisposition: NotRequired[LaunchDispositionType],  # (2)
    targetInstanceTypeRightSizingMethod: NotRequired[TargetInstanceTypeRightSizingMethodType],  # (3)
    copyPrivateIp: NotRequired[bool],
    associatePublicIpAddress: NotRequired[bool],
    copyTags: NotRequired[bool],
    licensing: NotRequired[LicensingTypeDef],  # (4)
    bootMode: NotRequired[BootModeType],  # (5)
    smallVolumeMaxSize: NotRequired[int],
    smallVolumeConf: NotRequired[LaunchTemplateDiskConfTypeDef],  # (6)
    largeVolumeConf: NotRequired[LaunchTemplateDiskConfTypeDef],  # (6)
    enableParametersEncryption: NotRequired[bool],
    parametersEncryptionKey: NotRequired[str],
```

1. See [:material-code-braces: PostLaunchActionsOutputTypeDef](./type_defs.md#postlaunchactionsoutputtypedef)
2. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype)
3. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype)
4. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef)
5. See [:material-code-brackets: BootModeType](./literals.md#bootmodetype)
6. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef)
7. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef)

## LaunchConfigurationTypeDef

```python
# LaunchConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import LaunchConfigurationTypeDef


def get_value() -> LaunchConfigurationTypeDef:
    return {
        "sourceServerID": ...,
    }


# LaunchConfigurationTypeDef definition

class LaunchConfigurationTypeDef(TypedDict):
    sourceServerID: str,
    name: str,
    ec2LaunchTemplateID: str,
    launchDisposition: LaunchDispositionType,  # (1)
    targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType,  # (2)
    copyPrivateIp: bool,
    copyTags: bool,
    licensing: LicensingTypeDef,  # (3)
    bootMode: BootModeType,  # (4)
    postLaunchActions: PostLaunchActionsOutputTypeDef,  # (5)
    enableMapAutoTagging: bool,
    mapAutoTaggingMpeID: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype)
2. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype)
3. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef)
4. See [:material-code-brackets: BootModeType](./literals.md#bootmodetype)
5. See [:material-code-braces: PostLaunchActionsOutputTypeDef](./type_defs.md#postlaunchactionsoutputtypedef)
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
    items: list[SourceServerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[SourceServerTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ParticipatingServerTypeDef

```python
# ParticipatingServerTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import ParticipatingServerTypeDef


def get_value() -> ParticipatingServerTypeDef:
    return {
        "sourceServerID": ...,
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
    items: list[LaunchConfigurationTemplateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[LaunchConfigurationTemplateTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateLaunchConfigurationTemplateRequestTypeDef

```python
# CreateLaunchConfigurationTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import CreateLaunchConfigurationTemplateRequestTypeDef


def get_value() -> CreateLaunchConfigurationTemplateRequestTypeDef:
    return {
        "postLaunchActions": ...,
    }


# CreateLaunchConfigurationTemplateRequestTypeDef definition

class CreateLaunchConfigurationTemplateRequestTypeDef(TypedDict):
    postLaunchActions: NotRequired[PostLaunchActionsUnionTypeDef],  # (1)
    enableMapAutoTagging: NotRequired[bool],
    mapAutoTaggingMpeID: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    launchDisposition: NotRequired[LaunchDispositionType],  # (2)
    targetInstanceTypeRightSizingMethod: NotRequired[TargetInstanceTypeRightSizingMethodType],  # (3)
    copyPrivateIp: NotRequired[bool],
    associatePublicIpAddress: NotRequired[bool],
    copyTags: NotRequired[bool],
    licensing: NotRequired[LicensingTypeDef],  # (4)
    bootMode: NotRequired[BootModeType],  # (5)
    smallVolumeMaxSize: NotRequired[int],
    smallVolumeConf: NotRequired[LaunchTemplateDiskConfTypeDef],  # (6)
    largeVolumeConf: NotRequired[LaunchTemplateDiskConfTypeDef],  # (6)
    enableParametersEncryption: NotRequired[bool],
    parametersEncryptionKey: NotRequired[str],
```

1. See [:material-code-braces: PostLaunchActionsUnionTypeDef](#postlaunchactionsuniontypedef)
2. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype)
3. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype)
4. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef)
5. See [:material-code-brackets: BootModeType](./literals.md#bootmodetype)
6. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef)
7. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef)

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
    name: NotRequired[str],
    launchDisposition: NotRequired[LaunchDispositionType],  # (1)
    targetInstanceTypeRightSizingMethod: NotRequired[TargetInstanceTypeRightSizingMethodType],  # (2)
    copyPrivateIp: NotRequired[bool],
    copyTags: NotRequired[bool],
    licensing: NotRequired[LicensingTypeDef],  # (3)
    bootMode: NotRequired[BootModeType],  # (4)
    postLaunchActions: NotRequired[PostLaunchActionsUnionTypeDef],  # (5)
    enableMapAutoTagging: NotRequired[bool],
    mapAutoTaggingMpeID: NotRequired[str],
    accountID: NotRequired[str],
```

1. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype)
2. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype)
3. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef)
4. See [:material-code-brackets: BootModeType](./literals.md#bootmodetype)
5. See [:material-code-braces: PostLaunchActionsUnionTypeDef](#postlaunchactionsuniontypedef)

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
    postLaunchActions: NotRequired[PostLaunchActionsUnionTypeDef],  # (1)
    enableMapAutoTagging: NotRequired[bool],
    mapAutoTaggingMpeID: NotRequired[str],
    launchDisposition: NotRequired[LaunchDispositionType],  # (2)
    targetInstanceTypeRightSizingMethod: NotRequired[TargetInstanceTypeRightSizingMethodType],  # (3)
    copyPrivateIp: NotRequired[bool],
    associatePublicIpAddress: NotRequired[bool],
    copyTags: NotRequired[bool],
    licensing: NotRequired[LicensingTypeDef],  # (4)
    bootMode: NotRequired[BootModeType],  # (5)
    smallVolumeMaxSize: NotRequired[int],
    smallVolumeConf: NotRequired[LaunchTemplateDiskConfTypeDef],  # (6)
    largeVolumeConf: NotRequired[LaunchTemplateDiskConfTypeDef],  # (6)
    enableParametersEncryption: NotRequired[bool],
    parametersEncryptionKey: NotRequired[str],
```

1. See [:material-code-braces: PostLaunchActionsUnionTypeDef](#postlaunchactionsuniontypedef)
2. See [:material-code-brackets: LaunchDispositionType](./literals.md#launchdispositiontype)
3. See [:material-code-brackets: TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype)
4. See [:material-code-braces: LicensingTypeDef](./type_defs.md#licensingtypedef)
5. See [:material-code-brackets: BootModeType](./literals.md#bootmodetype)
6. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef)
7. See [:material-code-braces: LaunchTemplateDiskConfTypeDef](./type_defs.md#launchtemplatediskconftypedef)

## JobTypeDef

```python
# JobTypeDef TypedDict usage example

from types_aiobotocore_mgn.type_defs import JobTypeDef


def get_value() -> JobTypeDef:
    return {
        "jobID": ...,
    }


# JobTypeDef definition

class JobTypeDef(TypedDict):
    jobID: str,
    arn: NotRequired[str],
    type: NotRequired[JobTypeType],  # (1)
    initiatedBy: NotRequired[InitiatedByType],  # (2)
    creationDateTime: NotRequired[str],
    endDateTime: NotRequired[str],
    status: NotRequired[JobStatusType],  # (3)
    participatingServers: NotRequired[list[ParticipatingServerTypeDef]],  # (4)
    tags: NotRequired[dict[str, str]],
```

1. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype)
2. See [:material-code-brackets: InitiatedByType](./literals.md#initiatedbytype)
3. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype)
4. See `list[ParticipatingServerTypeDef]`

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
    items: list[JobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[JobTypeDef]`
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

